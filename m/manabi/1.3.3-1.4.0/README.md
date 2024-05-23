# Comparing `tmp/manabi-1.3.3.tar.gz` & `tmp/manabi-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manabi-1.3.3.tar", max compression
+gzip compressed data, was "manabi-1.4.0.tar", max compression
```

## Comparing `manabi-1.3.3.tar` & `manabi-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3722 2024-02-28 09:16:44.888912 manabi-1.3.3/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-02-28 09:16:44.888912 manabi-1.3.3/LICENSE
--rw-r--r--   0        0        0     5507 2024-02-28 09:16:44.888912 manabi-1.3.3/README.md
--rw-r--r--   0        0        0     1372 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi/__init__.py
--rw-r--r--   0        0        0     9996 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi/__snapshots__/filesystem_test.ambr
--rw-r--r--   0        0        0     4373 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi/auth.py
--rw-r--r--   0        0        0     9711 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi/filesystem.py
--rw-r--r--   0        0        0    10021 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi/lock.py
--rw-r--r--   0        0        0     2681 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi/log.py
--rw-r--r--   0        0        0      468 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi/mypy_fix.py
--rw-r--r--   0        0        0     5263 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi/token.py
--rw-r--r--   0        0        0      521 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi/type_alias.py
--rw-r--r--   0        0        0     3374 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi/util.py
--rw-r--r--   0        0        0        0 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi_django/manabi_migrations/__init__.py
--rw-r--r--   0        0        0      165 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi_django/manabi_migrations/apps.py
--rw-r--r--   0        0        0      585 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi_django/manabi_migrations/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi_django/manabi_migrations/migrations/__init__.py
--rw-r--r--   0        0        0      200 2024-02-28 09:16:44.888912 manabi-1.3.3/manabi_django/manabi_migrations/models.py
--rw-r--r--   0        0        0     2815 2024-02-28 09:16:44.892912 manabi-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     6895 1970-01-01 00:00:00.000000 manabi-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     3870 2024-05-23 09:45:54.104150 manabi-1.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-05-23 09:33:17.261753 manabi-1.4.0/LICENSE
+-rw-r--r--   0        0        0     5507 2024-05-23 09:33:17.261917 manabi-1.4.0/README.md
+-rw-r--r--   0        0        0     1372 2024-05-23 09:33:17.262333 manabi-1.4.0/manabi/__init__.py
+-rw-r--r--   0        0        0     9996 2024-05-23 09:33:17.262503 manabi-1.4.0/manabi/__snapshots__/filesystem_test.ambr
+-rw-r--r--   0        0        0     4373 2024-05-23 09:33:17.262574 manabi-1.4.0/manabi/auth.py
+-rw-r--r--   0        0        0     9711 2024-05-23 09:33:17.263216 manabi-1.4.0/manabi/filesystem.py
+-rw-r--r--   0        0        0    10021 2024-05-23 09:33:17.263396 manabi-1.4.0/manabi/lock.py
+-rw-r--r--   0        0        0     2681 2024-05-23 09:33:17.263573 manabi-1.4.0/manabi/log.py
+-rw-r--r--   0        0        0      468 2024-05-23 09:33:17.263747 manabi-1.4.0/manabi/mypy_fix.py
+-rw-r--r--   0        0        0     5263 2024-05-23 09:33:17.263826 manabi-1.4.0/manabi/token.py
+-rw-r--r--   0        0        0      521 2024-05-23 09:33:17.263979 manabi-1.4.0/manabi/type_alias.py
+-rw-r--r--   0        0        0     3374 2024-05-23 09:33:17.264056 manabi-1.4.0/manabi/util.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:33:17.264505 manabi-1.4.0/manabi_django/manabi_migrations/__init__.py
+-rw-r--r--   0        0        0      165 2024-05-23 09:33:17.264577 manabi-1.4.0/manabi_django/manabi_migrations/apps.py
+-rw-r--r--   0        0        0      585 2024-05-23 09:33:17.264678 manabi-1.4.0/manabi_django/manabi_migrations/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:33:17.264709 manabi-1.4.0/manabi_django/manabi_migrations/migrations/__init__.py
+-rw-r--r--   0        0        0      200 2024-05-23 09:33:17.264778 manabi-1.4.0/manabi_django/manabi_migrations/models.py
+-rw-r--r--   0        0        0     2836 2024-05-23 09:43:27.776561 manabi-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6886 1970-01-01 00:00:00.000000 manabi-1.4.0/PKG-INFO
```

### Comparing `manabi-1.3.3/CHANGELOG.md` & `manabi-1.4.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## v1.4.0
+### Chore
+
+* update to django 4.x ([`3e9084b`](https://github.com/projectcaluma/manabi/commit/3e9084b0774bfa06c6229311ae927f86d426a6ed))
+
 ## v1.3.3
 ### Fix
 
 * Move methods from `ManabiFileResource` to `ManabiFileResourceMixin` ([`acc3193`](https://github.com/projectcaluma/manabi/commit/acc31932047bd75bc75ef9681fe84308fb98ad7c))
 
 ## v1.3.2
 ### Fix
```

### Comparing `manabi-1.3.3/LICENSE` & `manabi-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manabi-1.3.3/README.md` & `manabi-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `manabi-1.3.3/manabi/__init__.py` & `manabi-1.4.0/manabi/__init__.py`

 * *Files identical despite different names*

### Comparing `manabi-1.3.3/manabi/__snapshots__/filesystem_test.ambr` & `manabi-1.4.0/manabi/__snapshots__/filesystem_test.ambr`

 * *Files identical despite different names*

### Comparing `manabi-1.3.3/manabi/auth.py` & `manabi-1.4.0/manabi/auth.py`

 * *Files identical despite different names*

### Comparing `manabi-1.3.3/manabi/filesystem.py` & `manabi-1.4.0/manabi/filesystem.py`

 * *Files identical despite different names*

### Comparing `manabi-1.3.3/manabi/lock.py` & `manabi-1.4.0/manabi/lock.py`

 * *Files identical despite different names*

### Comparing `manabi-1.3.3/manabi/log.py` & `manabi-1.4.0/manabi/log.py`

 * *Files identical despite different names*

### Comparing `manabi-1.3.3/manabi/token.py` & `manabi-1.4.0/manabi/token.py`

 * *Files identical despite different names*

### Comparing `manabi-1.3.3/manabi/type_alias.py` & `manabi-1.4.0/manabi/type_alias.py`

 * *Files identical despite different names*

### Comparing `manabi-1.3.3/manabi/util.py` & `manabi-1.4.0/manabi/util.py`

 * *Files identical despite different names*

### Comparing `manabi-1.3.3/manabi_django/manabi_migrations/migrations/0001_initial.py` & `manabi-1.4.0/manabi_django/manabi_migrations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `manabi-1.3.3/pyproject.toml` & `manabi-1.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "manabi"
-version = "1.3.3"
+version = "1.4.0"
 description = "Provide WebDAV access for documents."
 homepage = "https://github.com/projectcaluma/manabi"
 repository = "https://github.com/projectcaluma/manabi"
 authors = ["Adfinis AG"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
@@ -31,35 +31,35 @@
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 WsgiDAV = "^4.3.0"
 pybranca = "^0.5.0"
 pybase62 = "^1.0.0"
 attrs = "^23.1.0"
-django = "^3.2.15"
+django = ">=3.0,<5.0"
 psycopg2-binary = "^2.9.3"
 u-msgpack-python = "^2.8.0"
 boto3 = "^1.34.21"
-smart-open = {extras = ["s3"], version = "^6.4.0"}
+smart-open = {extras = ["s3"], version = ">=6.4,<8.0"}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 cheroot = "^10.0.0"
 flake8 = "^6.0.0"
 flake8-bugbear = "^23.5.9"
 flake8-debugger = "^4.1.2"
 flake8-docstrings = "^1.7.0"
 flake8-isort = "^6.0.0"
 flake8-string-format = "^0.3.0"
 flake8-tuple = "^0.4.1"
 hypothesis = "^6.54.6"
 mypy = "^1.3.0"
 pdbpp = "^0.10.3"
-pytest = "^7.3.1"
-python-semantic-release = "^7.32.0"
+pytest = ">=7.3.1,<9.0.0"
+python-semantic-release = ">=7.32,<10.0"
 requests = "^2.28.1"
 types-psycopg2 = "^2.9.21"
 types-requests = "^2.28.11"
 python-lsp-server = "^1.7.3"
 python-lsp-black = "^1.3.0"
 python-lsp-isort = "^0.1"
 flake8-pyproject = "^1.2.3"
@@ -109,8 +109,8 @@
     E203,
 """
 max_line_length = 88
 doctests = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `manabi-1.3.3/PKG-INFO` & `manabi-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manabi
-Version: 1.3.3
+Version: 1.4.0
 Summary: Provide WebDAV access for documents.
 Home-page: https://github.com/projectcaluma/manabi
 License: AGPL-3.0-or-later
 Author: Adfinis AG
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -17,19 +17,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: WsgiDAV (>=4.3.0,<5.0.0)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: boto3 (>=1.34.21,<2.0.0)
-Requires-Dist: django (>=3.2.15,<4.0.0)
+Requires-Dist: django (>=3.0,<5.0)
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
 Requires-Dist: pybase62 (>=1.0.0,<2.0.0)
 Requires-Dist: pybranca (>=0.5.0,<0.6.0)
-Requires-Dist: smart-open[s3] (>=6.4.0,<7.0.0)
+Requires-Dist: smart-open[s3] (>=6.4,<8.0)
 Requires-Dist: u-msgpack-python (>=2.8.0,<3.0.0)
 Project-URL: Repository, https://github.com/projectcaluma/manabi
 Description-Content-Type: text/markdown
 
 # Manabi
 
 ```
```

