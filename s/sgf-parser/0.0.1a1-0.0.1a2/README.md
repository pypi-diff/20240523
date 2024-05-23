# Comparing `tmp/sgf_parser-0.0.1a1.tar.gz` & `tmp/sgf_parser-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgf_parser-0.0.1a1.tar", max compression
+gzip compressed data, was "sgf_parser-0.0.1a2.tar", max compression
```

## Comparing `sgf_parser-0.0.1a1.tar` & `sgf_parser-0.0.1a2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1095 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     2183 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/README.md
--rw-r--r--   0        0        0     1642 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0       36 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/__init__.py
--rw-r--r--   0        0        0     1162 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/datetime_parser.py
--rw-r--r--   0        0        0      494 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/models/__init__.py
--rw-r--r--   0        0        0    14654 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/models/method.py
--rw-r--r--   0        0        0    10787 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/models/method_cpt.py
--rw-r--r--   0        0        0     2170 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/models/method_rp.py
--rw-r--r--   0        0        0     6388 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/models/method_srs.py
--rw-r--r--   0        0        0     2048 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/models/method_svt.py
--rw-r--r--   0        0        0     6198 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/models/method_tot.py
--rw-r--r--   0        0        0      173 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/models/method_type.py
--rw-r--r--   0        0        0        0 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/models/method_wst.py
--rw-r--r--   0        0        0     2556 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/models/types.py
--rw-r--r--   0        0        0     4738 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/parser.py
--rw-r--r--   0        0        0      102 2024-04-03 12:55:28.227770 sgf_parser-0.0.1a1/src/sgf_parser/units.py
--rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 sgf_parser-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     2165 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/README.md
+-rw-r--r--   0        0        0     1642 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/__init__.py
+-rw-r--r--   0        0        0     1162 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/datetime_parser.py
+-rw-r--r--   0        0        0      557 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/models/__init__.py
+-rw-r--r--   0        0        0    14654 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/models/method.py
+-rw-r--r--   0        0        0    10787 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/models/method_cpt.py
+-rw-r--r--   0        0        0      911 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/models/method_dt.py
+-rw-r--r--   0        0        0     2170 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/models/method_rp.py
+-rw-r--r--   0        0        0     6388 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/models/method_srs.py
+-rw-r--r--   0        0        0     2048 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/models/method_svt.py
+-rw-r--r--   0        0        0     6198 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/models/method_tot.py
+-rw-r--r--   0        0        0      187 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/models/method_type.py
+-rw-r--r--   0        0        0        0 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/models/method_wst.py
+-rw-r--r--   0        0        0     2556 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/models/types.py
+-rw-r--r--   0        0        0     4769 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/parser.py
+-rw-r--r--   0        0        0      102 2024-05-23 13:45:18.674417 sgf_parser-0.0.1a2/src/sgf_parser/units.py
+-rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 sgf_parser-0.0.1a2/PKG-INFO
```

### Comparing `sgf_parser-0.0.1a1/LICENSE` & `sgf_parser-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `sgf_parser-0.0.1a1/README.md` & `sgf_parser-0.0.1a2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ```
 
 ## Basic usage
 
 ```python
 from sgf_parser import Parser
 
-with open("c:/dev/sgf-parser/tests/data/cpt-test-3.cpt", "rt") as file:
+with open("tests/data/cpt-test-3.cpt", "rt") as file:
     # The test file only contains one method
     [method] = Parser().parse(file)
 
 print(repr(method))
 # <MethodCPT CPT method_data=[<MethodCPTData 1.000>, <MethodCPTData 1.020>, <MethodCPTData 1.040>, 
 # <MethodCPTData 1.060>, <MethodCPTData 1.080>, <MethodCPTData 1.100>, <MethodCPTData 1.120>, ...,
 # <MethodCPTData 24.940>, <MethodCPTData 24.960>, <MethodCPTData 24.980>]>
```

### Comparing `sgf_parser-0.0.1a1/pyproject.toml` & `sgf_parser-0.0.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "sgf-parser"
-version = "0.0.1a1"
+version = "0.0.1a2"
 description = "Parser for the Swedish Geotechnical Society / Svenska Geotekniska Föreningen (SGF) data format"
 license = "MIT"
 authors = ["Jostein Leira <jostein@leira.net>"]
 maintainers = ["Jostein Leira <jostein@leira.net>"]
 readme = "README.md"
 homepage = "https://github.com/norwegian-geotechnical-institute/sgf-parser"
 repository = "https://github.com/norwegian-geotechnical-institute/sgf-parser"
```

### Comparing `sgf_parser-0.0.1a1/src/sgf_parser/datetime_parser.py` & `sgf_parser-0.0.1a2/src/sgf_parser/datetime_parser.py`

 * *Files identical despite different names*

### Comparing `sgf_parser-0.0.1a1/src/sgf_parser/models/method.py` & `sgf_parser-0.0.1a2/src/sgf_parser/models/method.py`

 * *Files identical despite different names*

### Comparing `sgf_parser-0.0.1a1/src/sgf_parser/models/method_cpt.py` & `sgf_parser-0.0.1a2/src/sgf_parser/models/method_cpt.py`

 * *Files identical despite different names*

### Comparing `sgf_parser-0.0.1a1/src/sgf_parser/models/method_rp.py` & `sgf_parser-0.0.1a2/src/sgf_parser/models/method_rp.py`

 * *Files identical despite different names*

### Comparing `sgf_parser-0.0.1a1/src/sgf_parser/models/method_srs.py` & `sgf_parser-0.0.1a2/src/sgf_parser/models/method_srs.py`

 * *Files identical despite different names*

### Comparing `sgf_parser-0.0.1a1/src/sgf_parser/models/method_svt.py` & `sgf_parser-0.0.1a2/src/sgf_parser/models/method_svt.py`

 * *Files identical despite different names*

### Comparing `sgf_parser-0.0.1a1/src/sgf_parser/models/method_tot.py` & `sgf_parser-0.0.1a2/src/sgf_parser/models/method_tot.py`

 * *Files identical despite different names*

### Comparing `sgf_parser-0.0.1a1/src/sgf_parser/models/types.py` & `sgf_parser-0.0.1a2/src/sgf_parser/models/types.py`

 * *Files identical despite different names*

### Comparing `sgf_parser-0.0.1a1/src/sgf_parser/parser.py` & `sgf_parser-0.0.1a2/src/sgf_parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         "23": models.MethodRP,
         "24": models.MethodTOT,
         "12": models.MethodSRS,
         "41": models.MethodSRS,
         "42": models.MethodSRS,
         "73": models.MethodSRS,
         "13": models.MethodSVT,
+        "35": models.MethodDT,
     }
 
     def parse(self, file: TextIO) -> list[Method]:
         """
         Parse the SGF file
 
         The file parameter must be an opened file in text mode (with correct character encoding), pointing at the start
```

### Comparing `sgf_parser-0.0.1a1/PKG-INFO` & `sgf_parser-0.0.1a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgf-parser
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Parser for the Swedish Geotechnical Society / Svenska Geotekniska Föreningen (SGF) data format
 Home-page: https://github.com/norwegian-geotechnical-institute/sgf-parser
 License: MIT
 Author: Jostein Leira
 Author-email: jostein@leira.net
 Maintainer: Jostein Leira
 Maintainer-email: jostein@leira.net
@@ -41,15 +41,15 @@
 ```
 
 ## Basic usage
 
 ```python
 from sgf_parser import Parser
 
-with open("c:/dev/sgf-parser/tests/data/cpt-test-3.cpt", "rt") as file:
+with open("tests/data/cpt-test-3.cpt", "rt") as file:
     # The test file only contains one method
     [method] = Parser().parse(file)
 
 print(repr(method))
 # <MethodCPT CPT method_data=[<MethodCPTData 1.000>, <MethodCPTData 1.020>, <MethodCPTData 1.040>, 
 # <MethodCPTData 1.060>, <MethodCPTData 1.080>, <MethodCPTData 1.100>, <MethodCPTData 1.120>, ...,
 # <MethodCPTData 24.940>, <MethodCPTData 24.960>, <MethodCPTData 24.980>]>
```

