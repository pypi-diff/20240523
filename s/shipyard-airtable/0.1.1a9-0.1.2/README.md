# Comparing `tmp/shipyard_airtable-0.1.1a9.tar.gz` & `tmp/shipyard_airtable-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_airtable-0.1.1a9.tar", max compression
+gzip compressed data, was "shipyard_airtable-0.1.2.tar", max compression
```

## Comparing `shipyard_airtable-0.1.1a9.tar` & `shipyard_airtable-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-01-26 20:55:51.413290 shipyard_airtable-0.1.1a9/README.md
--rw-r--r--   0        0        0      480 2024-02-01 16:41:21.494216 shipyard_airtable-0.1.1a9/pyproject.toml
--rw-r--r--   0        0        0       37 2023-05-12 18:48:21.821888 shipyard_airtable-0.1.1a9/shipyard_airtable/__init__.py
--rw-r--r--   0        0        0     4254 2024-02-01 04:01:01.089009 shipyard_airtable-0.1.1a9/shipyard_airtable/airtable.py
--rw-r--r--   0        0        0        0 2024-01-26 21:10:32.047918 shipyard_airtable-0.1.1a9/shipyard_airtable/cli/__init__.py
--rw-r--r--   0        0        0      368 2024-02-01 04:01:01.089462 shipyard_airtable-0.1.1a9/shipyard_airtable/cli/authtest.py
--rw-r--r--   0        0        0     2966 2024-02-01 04:40:50.261531 shipyard_airtable-0.1.1a9/shipyard_airtable/cli/download_file.py
--rw-r--r--   0        0        0     3948 2024-02-01 16:40:33.048627 shipyard_airtable-0.1.1a9/shipyard_airtable/cli/upload.py
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 shipyard_airtable-0.1.1a9/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-26 20:55:51.413290 shipyard_airtable-0.1.2/README.md
+-rw-r--r--   0        0        0      530 2024-05-23 14:43:35.188071 shipyard_airtable-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-05-12 18:48:21.821888 shipyard_airtable-0.1.2/shipyard_airtable/__init__.py
+-rw-r--r--   0        0        0     9664 2024-02-15 14:35:00.350657 shipyard_airtable-0.1.2/shipyard_airtable/airtable.py
+-rw-r--r--   0        0        0        0 2024-01-26 21:10:32.047918 shipyard_airtable-0.1.2/shipyard_airtable/cli/__init__.py
+-rw-r--r--   0        0        0      203 2024-05-23 14:43:35.188735 shipyard_airtable-0.1.2/shipyard_airtable/cli/authtest.py
+-rw-r--r--   0        0        0     2989 2024-04-01 15:54:40.968086 shipyard_airtable-0.1.2/shipyard_airtable/cli/download_file.py
+-rw-r--r--   0        0        0     5403 2024-02-07 15:09:08.396357 shipyard_airtable-0.1.2/shipyard_airtable/cli/upload.py
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 shipyard_airtable-0.1.2/PKG-INFO
```

### Comparing `shipyard_airtable-0.1.1a9/shipyard_airtable/cli/download_file.py` & `shipyard_airtable-0.1.2/shipyard_airtable/cli/download_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,23 +39,22 @@
         default="TRUE",
         required=False,
     )
     return parser.parse_args()
 
 
 def main():
-    artifact = Artifact("airtable")
-
-    args = get_args()
-    api_key = args.api_key
-    table_name = args.table_name
-    base_id = args.base_id
-    view_name = args.view_name
-
     try:
+        artifact = Artifact("airtable")
+
+        args = get_args()
+        api_key = args.api_key
+        table_name = args.table_name
+        base_id = args.base_id
+        view_name = args.view_name
         include_record_id = convert_to_boolean(args.include_record_id)
 
         destination_file_name = clean_folder_name(args.destination_file_name)
         destination_folder_name = clean_folder_name(args.destination_folder_name)
 
         destination_full_path = combine_folder_and_file_name(
             folder_name=destination_folder_name, file_name=destination_file_name
```

### Comparing `shipyard_airtable-0.1.1a9/shipyard_airtable/cli/upload.py` & `shipyard_airtable-0.1.2/shipyard_airtable/cli/upload.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,64 +24,100 @@
     )
     parser.add_argument(
         "--source-file-name-match-type",
         dest="source_file_name_match_type",
         required=True,
         default="exact_match",
     )
-    parser.add_argument("--key-fields", dest="key_fields", required=True)
+    parser.add_argument("--key-fields", dest="key_fields", required=False)
     parser.add_argument("--typecast", dest="typecast", required=False, default="FALSE")
+    parser.add_argument("--insert-method", dest="insert_method", required=True)
     return parser.parse_args()
 
 
+def prepare_data_from_csv(file):
+    logger.debug(f"Preparing data from file: {file}")
+    records = []
+    df = pandas.read_csv(file)
+
+    for index, row in df.iterrows():
+        record = {"fields": row.to_dict()}
+        if "id" in record["fields"]:
+            del record["fields"]["id"]
+        records.append(record)
+    logger.debug(f"Following records are prepared: \n {records}")
+    return records
+
+
 def main():
     try:
         artifact = Artifact("airtable")
+        responses = []
+
         args = get_args()
+        client = AirtableClient(api_key=args.api_key)
 
         typecast = convert_to_boolean(args.typecast) if args.typecast else False
         search_for = args.filename_or_pattern
         match_type = args.source_file_name_match_type
         source_folder = args.source_folder_name or "."
-        
         if args.key_fields:
             key_fields = args.key_fields = args.key_fields.split(",")
         else:
             key_fields = None
+        upload_method = args.insert_method.lower()
 
-        
+        if upload_method not in {"append", "upsert", "replace"}:
+            logger.error(
+                "Invalid upload method. Please choose from 'append', 'upsert', or 'replace'"
+            )
+            sys.exit(client.EXIT_CODE_INVALID_INPUT)
+        if upload_method == "upsert" and not key_fields:
+            logger.error("Key fields are required for upsert method.")
+            sys.exit(client.EXIT_CODE_INVALID_INPUT)
+
+        if upload_method == "append" and key_fields:
+            logger.warning(
+                "Key fields are not required for append method, ignoring the key fields"
+            )
 
-        client = AirtableClient(api_key=args.api_key)
-        file_matches = files.find_matching_files(
+        files_found = files.find_matching_files(
             args.filename_or_pattern, source_folder, match_type
         )
-        if len(file_matches) == 0:
+
+        if upload_method == "replace":
+            client.clear_table(args.base_id, args.table_id)
+            upload_method = "append"
+
+        if len(files_found) == 0:
             logger.error(
-                f"No files found matching search criteria: {search_for} in {source_folder} with match type: {match_type}"
+                f"No files found matching search criteria: {search_for} in {source_folder} "
+                f"with match type: {match_type}"
             )
             sys.exit(client.EXIT_CODE_FILE_NOT_FOUND)
+
         failed, success = [], []
-        logger.info(f"Uploading {len(file_matches)} file(s) to Airtable...")
-        for file in file_matches:
-            try:
-                records = []
-                df = pandas.read_csv(file)
+        logger.info(f"Uploading {len(files_found)} file(s) to Airtable...")
 
-                for index, row in df.iterrows():
-                    record = {"fields": row.to_dict()}
-                    if "id" in record["fields"]:
-                        del record["fields"]["id"]
-                    records.append(record)
-
-                if key_fields:
-                    client.upload(
-                        args.base_id, args.table_id, records, key_fields, typecast
-                    )
+        for file in files_found:
+            try:
+                upload_args = {
+                    "base": args.base_id,
+                    "table": args.table_id,
+                    "typecast": typecast,
+                    "upload_method": upload_method,
+                }
+                if upload_method == "upsert":
+                    upload_args["key_fields"] = key_fields
+                    upload_args["data"] = prepare_data_from_csv(file)
                 else:
-                    client.upload(args.base_id, args.table_id, records, typecast)
+                    upload_args["data"] = pandas.read_csv(file).to_dict(
+                        orient="records"
+                    )
+                responses.append(client.upload(**upload_args))
 
             except Exception as e:
                 logger.error(f"Error uploading file: {file} to Airtable: {e}")
                 failed.append(
                     {
                         "file": file,
                         "error": f"Error uploading file: {file} to Airtable: {e}",
@@ -96,14 +132,16 @@
         logger.error(err.message)
         sys.exit(err.exit_code)
     except Exception as e:
         logger.error(f"Unexpected error occurred: {e}")
         sys.exit(1)
 
     else:
+        if responses:
+            artifact.responses.write_json("airtable_upload_responses", responses)
         artifact.logs.write_json(
             "airtable_upload_status", {"success": success, "failed": failed}
         )
         if success:
             logger.info(f"Uploaded {len(success)} file(s) to Airtable successfully.")
         if failed:
             logger.error(f"Failed to upload {len(failed)} file(s) to Airtable.")
```

### Comparing `shipyard_airtable-0.1.1a9/PKG-INFO` & `shipyard_airtable-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: shipyard-airtable
-Version: 0.1.1a9
+Version: 0.1.2
 Summary: A local client to work with Airtable
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pyairtable (==2.2.2)
-Requires-Dist: shipyard-bp-utils (==1.0.1a3)
-Requires-Dist: shipyard-templates (==0.6.1a1)
+Requires-Dist: shipyard-bp-utils (==1.0.1)
+Requires-Dist: shipyard-templates (==0.6.1)
 Description-Content-Type: text/markdown
```

