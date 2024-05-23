# Comparing `tmp/qibo_client-0.0.4.tar.gz` & `tmp/qibo_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibo_client-0.0.4.tar", max compression
+gzip compressed data, was "qibo_client-0.0.5.tar", max compression
```

## Comparing `qibo_client-0.0.4.tar` & `qibo_client-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-04-01 10:19:46.253145 qibo_client-0.0.4/LICENSE
--rw-r--r--   0        0        0     1280 2024-04-01 10:19:46.253145 qibo_client-0.0.4/README.md
--rw-r--r--   0        0        0     1357 2024-04-01 10:19:46.253145 qibo_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      132 2024-04-01 10:19:46.253145 qibo_client-0.0.4/src/qibo_client/__init__.py
--rw-r--r--   0        0        0      750 2024-04-01 10:19:46.253145 qibo_client-0.0.4/src/qibo_client/config.py
--rw-r--r--   0        0        0      257 2024-04-01 10:19:46.253145 qibo_client-0.0.4/src/qibo_client/config_logging.py
--rw-r--r--   0        0        0      245 2024-04-01 10:19:46.253145 qibo_client-0.0.4/src/qibo_client/constants.py
--rw-r--r--   0        0        0     8085 2024-04-01 10:19:46.253145 qibo_client-0.0.4/src/qibo_client/qibo_client.py
--rw-r--r--   0        0        0      366 2024-04-01 10:19:46.253145 qibo_client-0.0.4/src/qibo_client/tii.py
--rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 qibo_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 06:00:15.858188 qibo_client-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1280 2024-05-23 06:00:15.858188 qibo_client-0.0.5/README.md
+-rw-r--r--   0        0        0     1420 2024-05-23 06:00:15.862189 qibo_client-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-05-23 06:00:15.862189 qibo_client-0.0.5/src/qibo_client/__init__.py
+-rw-r--r--   0        0        0      750 2024-05-23 06:00:15.862189 qibo_client-0.0.5/src/qibo_client/config.py
+-rw-r--r--   0        0        0      257 2024-05-23 06:00:15.862189 qibo_client-0.0.5/src/qibo_client/config_logging.py
+-rw-r--r--   0        0        0      245 2024-05-23 06:00:15.862189 qibo_client-0.0.5/src/qibo_client/constants.py
+-rw-r--r--   0        0        0     8187 2024-05-23 06:00:15.862189 qibo_client-0.0.5/src/qibo_client/qibo_client.py
+-rw-r--r--   0        0        0      384 2024-05-23 06:00:15.862189 qibo_client-0.0.5/src/qibo_client/tii.py
+-rw-r--r--   0        0        0     2088 1970-01-01 00:00:00.000000 qibo_client-0.0.5/PKG-INFO
```

### Comparing `qibo_client-0.0.4/LICENSE` & `qibo_client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qibo_client-0.0.4/README.md` & `qibo_client-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `qibo_client-0.0.4/pyproject.toml` & `qibo_client-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qibo-client"
-version = "0.0.4"
+version = "0.0.5"
 description = "Qibo client interface."
 authors = ["The Qibo team"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://qibo.science/"
 repository = "https://github.com/qiboteam/qibo-client/"
 documentation = "https://qibo.science/qibo-client/stable"
@@ -16,19 +16,23 @@
 classifiers = [
   "Programming Language :: Python :: 3",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 packages = [{ include = "qibo_client", from = "src" }]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.9,<3.13"
 qibo = ">=0.2.4"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
+ipython = "^7"
+pdbpp = "^0.10.3"
+
+[tool.poetry.group.test.dependencies]
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 pylint = "^3.0.3"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.2.6"
 recommonmark = "^0.7.1"
@@ -46,12 +50,8 @@
 
 [tool.pylint.reports]
 output-format = "colorized"
 
 [tool.pytest.ini_options]
 testpaths = ['tests/']
 filterwarnings = ['ignore::RuntimeWarning']
-addopts = [
-  '--cov=src/qibo_client',
-  '--cov-report=xml',
-  '--cov-report=html',
-]
+addopts = ['--cov=src/qibo_client', '--cov-report=xml', '--cov-report=html']
```

### Comparing `qibo_client-0.0.4/src/qibo_client/config.py` & `qibo_client-0.0.5/src/qibo_client/config.py`

 * *Files identical despite different names*

### Comparing `qibo_client-0.0.4/src/qibo_client/qibo_client.py` & `qibo_client-0.0.5/src/qibo_client/qibo_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,23 +175,28 @@
             "Check results every %d seconds ...", constants.SECONDS_BETWEEN_CHECKS
         )
         result = self._get_result()
 
         return result
 
     def _post_circuit(
-        self, circuit: qibo.Circuit, nshots: int = 100, device: str = "sim"
+        self,
+        circuit: qibo.Circuit,
+        nshots: int = 100,
+        device: str = "sim",
+        lab_location: str = "tii",
     ):
         # HTTP request
         url = self.url + "run_circuit/"
         payload = {
             "token": self.token,
             "circuit": circuit.raw,
             "nshots": nshots,
             "device": device,
+            "lab_location": lab_location,
         }
         response = requests.post(url, json=payload, timeout=constants.TIMEOUT)
 
         # checks
         response.raise_for_status()
         check_response_has_keys(response, ["pid", "message"])
```

### Comparing `qibo_client-0.0.4/PKG-INFO` & `qibo_client-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: qibo-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Qibo client interface.
 Home-page: https://qibo.science/
 License: Apache-2.0
 Author: The Qibo team
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: qibo (>=0.2.4)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://qibo.science/qibo-client/stable
 Project-URL: Repository, https://github.com/qiboteam/qibo-client/
 Description-Content-Type: text/markdown
```

