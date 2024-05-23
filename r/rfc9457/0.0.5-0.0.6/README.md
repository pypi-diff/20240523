# Comparing `tmp/rfc9457-0.0.5.tar.gz` & `tmp/rfc9457-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfc9457-0.0.5.tar", max compression
+gzip compressed data, was "rfc9457-0.0.6.tar", max compression
```

## Comparing `rfc9457-0.0.5.tar` & `rfc9457-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11307 2024-05-21 16:54:09.801519 rfc9457-0.0.5/LICENSE
--rw-r--r--   0        0        0     1789 2024-05-21 16:54:09.801519 rfc9457-0.0.5/README.md
--rw-r--r--   0        0        0     2021 2024-05-21 16:54:09.801519 rfc9457-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2777 2024-05-21 16:54:09.801519 rfc9457-0.0.5/src/rfc9457/__init__.py
--rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 rfc9457-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-05-22 10:51:50.872209 rfc9457-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1789 2024-05-22 10:51:50.872209 rfc9457-0.0.6/README.md
+-rw-r--r--   0        0        0     2021 2024-05-22 10:51:50.872209 rfc9457-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2884 2024-05-22 10:51:50.872209 rfc9457-0.0.6/src/rfc9457/__init__.py
+-rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 rfc9457-0.0.6/PKG-INFO
```

### Comparing `rfc9457-0.0.5/LICENSE` & `rfc9457-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.5/README.md` & `rfc9457-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.5/pyproject.toml` & `rfc9457-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rfc9457"
-version = "0.0.5"
+version = "0.0.6"
 description = "Implementation of RFC9457 problems."
 authors = ["Daniel Edgecombe <daniel@nrwl.co>"]
 license = "Apache-2.0"
 repository="https://github.com/NRWLDev/rfc9457/"
 homepage="https://github.com/NRWLDev/rfc9457/"
 readme = "README.md"
 
@@ -19,15 +19,15 @@
 pytest-random-order = "^1.0"
 
 # Style
 ruff = "^0.3"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.0.5"
+current_version = "0.0.6"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `rfc9457-0.0.5/src/rfc9457/__init__.py` & `rfc9457-0.0.6/src/rfc9457/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,18 @@
         self.title = title
         self.details = details
         self.status = status
         self.status_code = status  # work around for sentry integrations that expect status_code attr
         self.extras = kwargs
 
     def __str__(self: t.Self) -> str:
-        return f"{self.title}: {self.details}"
+        return self.title
+
+    def __repr__(self: t.Self) -> str:
+        return f"{self.__class__.__name__}<title={self.title}; details={self.details}>"
 
     @property
     def type(self: t.Self) -> str:
         type_ = error_class_to_type(self)
         return self._type if self._type else type_
 
     def marshal(self: t.Self, *, strip_debug: bool = False) -> dict[str, t.Any]:
```

### Comparing `rfc9457-0.0.5/PKG-INFO` & `rfc9457-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfc9457
-Version: 0.0.5
+Version: 0.0.6
 Summary: Implementation of RFC9457 problems.
 Home-page: https://github.com/NRWLDev/rfc9457/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: daniel@nrwl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

