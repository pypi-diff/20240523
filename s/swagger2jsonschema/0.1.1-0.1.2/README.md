# Comparing `tmp/swagger2jsonschema-0.1.1-py3-none-any.whl.zip` & `tmp/swagger2jsonschema-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9570 bytes, number of entries: 13
+Zip file size: 9661 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 04:09 swagger2jsonschema/__init__.py
--rw-r--r--  2.0 unx    10217 b- defN 24-May-03 03:02 swagger2jsonschema/command.py
+-rw-r--r--  2.0 unx    10251 b- defN 24-May-23 09:47 swagger2jsonschema/command.py
 -rw-r--r--  2.0 unx      707 b- defN 24-Mar-30 04:09 swagger2jsonschema/definitions.py
 -rw-r--r--  2.0 unx       68 b- defN 24-Mar-30 04:09 swagger2jsonschema/errors.py
 -rw-r--r--  2.0 unx      247 b- defN 24-Mar-30 04:09 swagger2jsonschema/log.py
 -rw-r--r--  2.0 unx     6161 b- defN 24-Mar-30 04:09 swagger2jsonschema/test_command.py
--rw-r--r--  2.0 unx     7841 b- defN 24-May-16 02:01 swagger2jsonschema/util.py
--rw-r--r--  2.0 unx      654 b- defN 24-May-16 02:20 swagger2jsonschema-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1486 b- defN 24-May-16 02:20 swagger2jsonschema-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 02:20 swagger2jsonschema-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       74 b- defN 24-May-16 02:20 swagger2jsonschema-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 24-May-16 02:20 swagger2jsonschema-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1144 b- defN 24-May-16 02:20 swagger2jsonschema-0.1.1.dist-info/RECORD
-13 files, 28719 bytes uncompressed, 7620 bytes compressed:  73.5%
+-rw-r--r--  2.0 unx     8532 b- defN 24-May-23 09:47 swagger2jsonschema/util.py
+-rw-r--r--  2.0 unx      654 b- defN 24-May-23 09:52 swagger2jsonschema-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1486 b- defN 24-May-23 09:52 swagger2jsonschema-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-23 09:52 swagger2jsonschema-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       74 b- defN 24-May-23 09:52 swagger2jsonschema-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 24-May-23 09:52 swagger2jsonschema-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1144 b- defN 24-May-23 09:52 swagger2jsonschema-0.1.2.dist-info/RECORD
+13 files, 29444 bytes uncompressed, 7711 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: swagger2jsonschema/test_command.py
 Comment: 
 
 Filename: swagger2jsonschema/util.py
 Comment: 
 
-Filename: swagger2jsonschema-0.1.1.dist-info/LICENSE
+Filename: swagger2jsonschema-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: swagger2jsonschema-0.1.1.dist-info/METADATA
+Filename: swagger2jsonschema-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: swagger2jsonschema-0.1.1.dist-info/WHEEL
+Filename: swagger2jsonschema-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: swagger2jsonschema-0.1.1.dist-info/entry_points.txt
+Filename: swagger2jsonschema-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: swagger2jsonschema-0.1.1.dist-info/top_level.txt
+Filename: swagger2jsonschema-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: swagger2jsonschema-0.1.1.dist-info/RECORD
+Filename: swagger2jsonschema-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swagger2jsonschema/command.py

```diff
@@ -196,15 +196,15 @@
     if include_bodies:
         components.update(
             get_request_and_response_body_components_from_paths(data["paths"]),
         )
 
     if include_parameters:
         debug("Processing request parameters")
-        components.update(get_request_parameters_from_paths(data["paths"]))
+        components.update(get_request_parameters_from_paths(data["paths"], data["components"]["parameters"]))
 
     for title in components:
         kind = title.split(".")[-1].lower()
         if kubernetes:
             # If it is a Kubernetes object, use a simplified group name
             if title.startswith("io.k8s"):
                 group = title.split(".")[-3].lower()
```

## swagger2jsonschema/util.py

```diff
@@ -169,31 +169,44 @@
                         response,
                         prefix=name_prefix_fmt.format(response_name_part),
                     )
                 )
     return components
 
 
-def get_request_parameters_from_paths(paths):
+def get_request_parameters_from_paths(paths, parameters):
     components = {}
     for path, path_definition in paths.items():
         for http_method, http_method_definition in path_definition.items():
             component = {}
             if "parameters" in http_method_definition:
                 component["properties"] = {}
                 required = []
                 for param_value in http_method_definition["parameters"]:
-                    name = param_value["name"]
-                    component["properties"][name] = {"in": param_value["in"]}
+                    if "$ref" in param_value:
+                        tmp = param_value["$ref"]
+                        tmp = tmp.replace("#/components/parameters/", "")
+                        external_param = parameters[tmp]
+                        name = external_param["name"]
+                        component["properties"][name] = {"in": external_param["in"]}
 
-                    for key in param_value["schema"]:
-                        component["properties"][name][key] = param_value["schema"][key]
+                        for key in external_param["schema"]:
+                            component["properties"][name][key] = external_param["schema"][key]
 
-                    if param_value["required"]:
-                        required.append(name)
+                        if external_param["required"]:
+                            required.append(name)
+                    else:
+                        name = param_value["name"]
+                        component["properties"][name] = {"in": param_value["in"]}
+
+                        for key in param_value["schema"]:
+                            component["properties"][name][key] = param_value["schema"][key]
+
+                        if param_value["required"]:
+                            required.append(name)
                 if required:
                     component["required"] = required
             if "requestBody" in http_method_definition:
                 content = http_method_definition["requestBody"]["content"]
                 schema = content["application/json"]["schema"]
                 if "$ref" in schema:
                     tmp = schema["$ref"]
```

## Comparing `swagger2jsonschema-0.1.1.dist-info/LICENSE` & `swagger2jsonschema-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `swagger2jsonschema-0.1.1.dist-info/METADATA` & `swagger2jsonschema-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swagger2jsonschema
-Version: 0.1.1
+Version: 0.1.2
 Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: attrs ==23.2.0
 Requires-Dist: click ==8.1.7
 Requires-Dist: jsonref ==1.1.0
 Requires-Dist: jsonschema ==4.21.1
 Requires-Dist: jsonschema-specifications ==2023.12.1
```

## Comparing `swagger2jsonschema-0.1.1.dist-info/RECORD` & `swagger2jsonschema-0.1.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 swagger2jsonschema/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-swagger2jsonschema/command.py,sha256=2HPZW9u5T02ruVn5OwkPtay4yVpR_zhVbxgtFdyzElw,10217
+swagger2jsonschema/command.py,sha256=BZ3dQqrdwRATC7SMtyflPqMLisS71UR3qJ_IpSUDQdo,10251
 swagger2jsonschema/definitions.py,sha256=INDqIV7rCuRtjV73Va5TlGp5sZUPVJY2PodQbcuj600,707
 swagger2jsonschema/errors.py,sha256=T7VZfl3FnHPHoqXFn-QmAXwlwOnPnyo3lcbCYXI_jpQ,68
 swagger2jsonschema/log.py,sha256=TVtGYLJkLhZpgQqe6PUxtSbGVg0RKZvMEvPcsAr0htQ,247
 swagger2jsonschema/test_command.py,sha256=oItmY5OAehwwhGonkD-XTXhEpskt9dp83E_aZrDVk6I,6161
-swagger2jsonschema/util.py,sha256=FSt0-PNVjGtjAaLMCVRIR8f7fBGUjZTVm-w35ranUw0,7841
-swagger2jsonschema-0.1.1.dist-info/LICENSE,sha256=6nn0TvfOBUFH__8Aqqhe6RfDCI_--Js0Jab8oZkAipE,654
-swagger2jsonschema-0.1.1.dist-info/METADATA,sha256=wJZwmgvjRXTHxE1zHpre-1TdRscB42ohNg7bYour1pk,1486
-swagger2jsonschema-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-swagger2jsonschema-0.1.1.dist-info/entry_points.txt,sha256=LXKu_O5s2NeA6Ga5NQ0N4quSMB52LTXs0580KiO6a5s,74
-swagger2jsonschema-0.1.1.dist-info/top_level.txt,sha256=T3u6MolDviqt4JENl6aZ0civpLecmX1vds1ASwe_n80,28
-swagger2jsonschema-0.1.1.dist-info/RECORD,,
+swagger2jsonschema/util.py,sha256=T7s_KuhHZFmEDgJBfmrtIkPsV9dgst2-4SQV_aW0N04,8532
+swagger2jsonschema-0.1.2.dist-info/LICENSE,sha256=6nn0TvfOBUFH__8Aqqhe6RfDCI_--Js0Jab8oZkAipE,654
+swagger2jsonschema-0.1.2.dist-info/METADATA,sha256=a5gBlZAEYwT8LfnK8LTLj6oF3o9wChxp9_1GF5ayAO4,1486
+swagger2jsonschema-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+swagger2jsonschema-0.1.2.dist-info/entry_points.txt,sha256=LXKu_O5s2NeA6Ga5NQ0N4quSMB52LTXs0580KiO6a5s,74
+swagger2jsonschema-0.1.2.dist-info/top_level.txt,sha256=T3u6MolDviqt4JENl6aZ0civpLecmX1vds1ASwe_n80,28
+swagger2jsonschema-0.1.2.dist-info/RECORD,,
```

