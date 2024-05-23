# Comparing `tmp/xrvoyage-0.0.0.tar.gz` & `tmp/xrvoyage-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrvoyage-0.0.0.tar", max compression
+gzip compressed data, was "xrvoyage-1.0.1.tar", max compression
```

## Comparing `xrvoyage-0.0.0.tar` & `xrvoyage-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1086 2024-05-23 12:58:22.222996 xrvoyage-0.0.0/LICENSE
--rw-r--r--   0        0        0      461 2024-05-23 13:34:04.347418 xrvoyage-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1182 2024-05-23 13:30:09.535403 xrvoyage-0.0.0/xrvoyage/.github/workflows/publish.yml
--rw-r--r--   0        0        0      174 2024-05-23 13:25:09.279168 xrvoyage-0.0.0/xrvoyage/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 13:24:44.438093 xrvoyage-0.0.0/xrvoyage/handlers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 13:24:51.278643 xrvoyage-0.0.0/xrvoyage/models/__init__.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 xrvoyage-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-23 14:33:39.451999 xrvoyage-1.0.1/LICENSE
+-rw-r--r--   0        0        0      444 2024-05-23 14:33:51.196142 xrvoyage-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      167 2024-05-23 14:33:39.451999 xrvoyage-1.0.1/xrvoyage/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 14:33:39.451999 xrvoyage-1.0.1/xrvoyage/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 14:33:39.451999 xrvoyage-1.0.1/xrvoyage/models/__init__.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 xrvoyage-1.0.1/PKG-INFO
```

### Comparing `xrvoyage-0.0.0/LICENSE` & `xrvoyage-1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 XrVoyage
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 XrVoyage
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `xrvoyage-0.0.0/PKG-INFO` & `xrvoyage-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrvoyage
-Version: 0.0.0
+Version: 1.0.1
 Summary: XR Voyage Python Package
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

