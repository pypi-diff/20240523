# Comparing `tmp/gspread_models-1.0.5.tar.gz` & `tmp/gspread_models-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspread_models-1.0.5.tar", last modified: Mon May 20 21:46:46 2024, max compression
+gzip compressed data, was "gspread_models-1.0.6.tar", last modified: Thu May 23 03:00:29 2024, max compression
```

## Comparing `gspread_models-1.0.5.tar` & `gspread_models-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:46:46.752837 gspread_models-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 21:46:42.000000 gspread_models-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-20 21:46:46.752837 gspread_models-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-20 21:46:42.000000 gspread_models-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:46:46.752837 gspread_models-1.0.5/gspread_models/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 21:46:42.000000 gspread_models-1.0.5/gspread_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-20 21:46:42.000000 gspread_models-1.0.5/gspread_models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-20 21:46:42.000000 gspread_models-1.0.5/gspread_models/date_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-20 21:46:42.000000 gspread_models-1.0.5/gspread_models/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:46:46.752837 gspread_models-1.0.5/gspread_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-20 21:46:46.000000 gspread_models-1.0.5/gspread_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-20 21:46:46.000000 gspread_models-1.0.5/gspread_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:46:46.000000 gspread_models-1.0.5/gspread_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 21:46:46.000000 gspread_models-1.0.5/gspread_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 21:46:46.000000 gspread_models-1.0.5/gspread_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:46:46.752837 gspread_models-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-20 21:46:42.000000 gspread_models-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:00:29.100620 gspread_models-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 03:00:24.000000 gspread_models-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-05-23 03:00:29.100620 gspread_models-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-23 03:00:24.000000 gspread_models-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:00:29.096620 gspread_models-1.0.6/gspread_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 03:00:24.000000 gspread_models-1.0.6/gspread_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-23 03:00:24.000000 gspread_models-1.0.6/gspread_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-23 03:00:24.000000 gspread_models-1.0.6/gspread_models/date_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-23 03:00:24.000000 gspread_models-1.0.6/gspread_models/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:00:29.100620 gspread_models-1.0.6/gspread_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-05-23 03:00:29.000000 gspread_models-1.0.6/gspread_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 03:00:29.000000 gspread_models-1.0.6/gspread_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:00:29.000000 gspread_models-1.0.6/gspread_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 03:00:29.000000 gspread_models-1.0.6/gspread_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 03:00:29.000000 gspread_models-1.0.6/gspread_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 03:00:29.100620 gspread_models-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-23 03:00:24.000000 gspread_models-1.0.6/setup.py
```

### Comparing `gspread_models-1.0.5/LICENSE` & `gspread_models-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gspread_models-1.0.5/gspread_models/base.py` & `gspread_models-1.0.6/gspread_models/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 
 #from abc import abstractmethod
 from typing import List, Dict
 from functools import lru_cache #,cached_property
 from datetime import datetime
 
 from gspread import Worksheet #, Spreadsheet
-#from gspread_models.service import SpreadsheetService
+from gspread_models.service import SpreadsheetService
+#from pandas import DataFrame
 
 
 class BaseModel:
 
     SHEET_NAME = None # abstract constant (str) to be set in child class
 
     COLUMNS = [] # abstract constant to be set in child class
@@ -71,30 +72,39 @@
             if isinstance(val, datetime):
                 val = str(val)
             values.append(val)
         values.append(str(self.created_at))
         #values.append(str(self.updated_at))
         return values
 
-    def save(self):
-        print("SAVING RECORD TO SHEET:")
-        print(dict(self))
-        #if self.id:
-        #    self.attrs["updated_at"] = self.service.generate_timestamp()
-        #    self.update(dict(self))
-        #return self.create(dict(self))
+    #def save(self):
+    #    print("SAVING RECORD TO SHEET:")
+    #    print(dict(self))
+    #    #if self.id:
+    #    #    self.attrs["updated_at"] = self.service.generate_timestamp()
+    #    #    self.update(dict(self))
+    #    #return self.create(dict(self))
         return self.create_all([dict(self)])
 
     #
     # CLASS METHODS
     #
 
     @classmethod
-    def set_document_id(cls, document_id):
-        cls.service.document_id = document_id
+    def bind(cls, document_id, credentials_filepath=None, credentials=None, creds=None):
+        cls.service = SpreadsheetService(
+            document_id=document_id,
+            credentials_filepath=credentials_filepath,
+            credentials=credentials,
+            creds=creds
+        )
+
+    #@classmethod
+    #def set_document_id(cls, document_id):
+    #    cls.service.document_id = document_id
 
     @classmethod
     def get_sheet(cls) -> Worksheet:
        print(f"GET SHEET ('{cls.SHEET_NAME}')...")
        return cls.service.get_sheet(sheet_name=cls.SHEET_NAME)
 
     # using @property + @lru_cache because @cached_property throws:
@@ -102,31 +112,48 @@
     @classmethod
     @property
     @lru_cache(maxsize=None)
     def sheet(cls) -> Worksheet:
         """Caches the sheet to avoid unnecessary API requests."""
         return cls.get_sheet()
 
-    # ... API
+    # ... QUERY INTERFACE (API)
 
     @classmethod
     def find(cls, by_id):
-        """Fetches a record by its unique identifier."""
+        """Fetches a record by its unique identifier.
+        """
         records = cls.sheet.get_all_records()
         for record in records:
             if record.get("id") == by_id:
                 return cls(record)
         return None
 
     @classmethod
-    def all(cls):
-        """Fetches all records from a given sheet."""
+    def all(cls): # as_df=False
+        """Fetches all records from a given sheet.
+        """
         records = cls.sheet.get_all_records()
+        # we can consider passing the data back in dataframe format:
+        # see: https://github.com/s2t2/gspread-models-py/issues/12
+        #if as_df:
+        #    #df = DataFrame(records)
+        #    # use model conversion to take advantage of datetime-conversion, etc:
+        #    df = DataFrame([dict(cls(record)) for record in records])
+        #    df.index = df["id"]
+        #    return df
+        #else:
+        #    return [cls(record) for record in records]
         return [cls(record) for record in records]
 
+    #@classmethod
+    #def find_all(cls):
+    #    """alias method"""
+    #    return cls.all()
+
     @classmethod
     def destroy_all(cls):
         """Removes all records from a given sheet, except the header row."""
         records = cls.sheet.get_all_records()
         # start on the second row, and delete one more than the number of records (to account for header row)
         return cls.sheet.delete_rows(start_index=2, end_index=len(records)+1)
 
@@ -176,8 +203,9 @@
         """Appends new records (list of dictionaries) to the sheet.
             Adds auto-incrementing unique identifiers, and timestamp columns.
         """
         return cls.create_all([new_record])
 
     @classmethod
     def seed(cls):
+        """Convenience method, if you would like to set SEEDS."""
         return cls.create_all(new_records=cls.SEEDS)
```

### Comparing `gspread_models-1.0.5/gspread_models/date_parser.py` & `gspread_models-1.0.6/gspread_models/date_parser.py`

 * *Files identical despite different names*

### Comparing `gspread_models-1.0.5/gspread_models/service.py` & `gspread_models-1.0.6/gspread_models/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,26 +14,36 @@
 
 DEFAULT_FILEPATH = os.path.join(os.path.dirname(__file__), "..", "google-credentials.json")
 GOOGLE_CREDENTIALS_FILEPATH = os.getenv("GOOGLE_CREDENTIALS_FILEPATH", default=DEFAULT_FILEPATH)
 GOOGLE_SHEETS_DOCUMENT_ID = os.getenv("GOOGLE_SHEETS_DOCUMENT_ID", default="OOPS, Please get the spreadsheet identifier from its URL, and set the 'GOOGLE_SHEETS_DOCUMENT_ID' environment variable accordingly...")
 
 class SpreadsheetService(DateParser):
 
-    def __init__(self, credentials_filepath=GOOGLE_CREDENTIALS_FILEPATH, document_id=GOOGLE_SHEETS_DOCUMENT_ID, creds=None):
-        """Params:
-            Optionally pass creds (google.auth.compute_engine.credentials.Credentials) for example for use in colab notebook:
+    def __init__(self, credentials_filepath=GOOGLE_CREDENTIALS_FILEPATH, document_id=GOOGLE_SHEETS_DOCUMENT_ID, creds=None, credentials=None):
+        """The Spreadsheet Service provides a connection to a specified Google Sheets document.
 
-                    from google.colab import auth
-                    from google.auth import default
+            Params:
 
-                    auth.authenticate_user()
-                    creds, _ = default()
+                credentials_filepath : path to local service account JSON file
 
-                    service = SpreadsheetService(creds=creds)
+                document_id : google sheets document identifier (obtained from the URL)
+
+                creds or credentials : optionally pass credentials (google.auth.compute_engine.credentials.Credentials)
+
+                for example for use in colab notebook:
+
+                        from google.colab import auth
+                        from google.auth import default
+
+                        auth.authenticate_user()
+                        creds, _ = default()
+
+                        service = SpreadsheetService(creds=creds)
         """
+        creds = creds or credentials
         if creds:
             self.client = authorize(creds)
         else:
             self.client = service_account(filename=credentials_filepath)
 
         self.document_id = document_id
```

### Comparing `gspread_models-1.0.5/setup.py` & `gspread_models-1.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,10 +16,13 @@
     author_email="datacreativellc@gmail.com",
     description="An Object Relational Mapper (ORM) for the Google Sheets API. Provides a straightforward and intuitive model-based query interface, making it easy to interact with Google Sheets as if it were more like a database. Offers a fast and flexible way to get up and running with a Google Sheets database, for rapid prototyping and development in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown", # required if using a md file for long desc
     license="MIT",
     url="https://github.com/s2t2/gspread-models-py",
     keywords="google sheets gspread models orm spreadsheet google-sheets google-sheets-api gspread-models gspread_models",
-    install_requires=["python-dotenv", "gspread>=6.0.2"],  # install_requires
+    install_requires=["python-dotenv", "gspread>=6.0.2"],
+    #extras_require={
+    #    'pandas': ['pandas>=2.2.0']
+    #}, # pip install gspread-models[pandas]
     packages=["gspread_models"], # find_packages()
 )
```

