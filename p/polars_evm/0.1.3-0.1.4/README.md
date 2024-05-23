# Comparing `tmp/polars_evm-0.1.3.tar.gz` & `tmp/polars_evm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polars_evm-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "polars_evm-0.1.4.tar", last modified: Thu May 23 00:09:54 2024, max compression
```

## Comparing `polars_evm-0.1.3.tar` & `polars_evm-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      217 2023-08-20 17:36:17.412935 polars_evm-0.1.3/.gitignore
--rw-r--r--   0        0        0    10847 2023-08-20 16:04:24.951709 polars_evm-0.1.3/LICENSE-APACHE
--rw-r--r--   0        0        0     1095 2023-08-20 16:04:35.396495 polars_evm-0.1.3/LICENSE-MIT
--rw-r--r--   0        0        0     3168 2023-08-21 16:32:15.670708 polars_evm-0.1.3/README.md
--rw-r--r--   0        0        0      160 2023-10-23 20:52:04.496721 polars_evm-0.1.3/polars_evm/__init__.py
--rw-r--r--   0        0        0       84 2023-08-21 16:29:09.180640 polars_evm-0.1.3/polars_evm/_helpers/__init__.py
--rw-r--r--   0        0        0     2426 2023-10-23 20:50:39.812373 polars_evm-0.1.3/polars_evm/_helpers/encoding_conversions.py
--rw-r--r--   0        0        0      155 2023-08-21 16:28:55.361066 polars_evm-0.1.3/polars_evm/_helpers/formatting.py
--rw-r--r--   0        0        0     1093 2023-08-20 17:07:51.854297 polars_evm-0.1.3/polars_evm/_helpers/hashes.py
--rw-r--r--   0        0        0      121 2023-08-20 16:30:41.414067 polars_evm-0.1.3/polars_evm/namespaces/__init__.py
--rw-r--r--   0        0        0      935 2023-08-20 18:11:42.833213 polars_evm-0.1.3/polars_evm/namespaces/df_namespace.py
--rw-r--r--   0        0        0     1067 2023-08-20 18:11:47.548448 polars_evm-0.1.3/polars_evm/namespaces/expr_namespace.py
--rw-r--r--   0        0        0     1614 2023-08-20 17:23:50.999032 polars_evm-0.1.3/polars_evm/namespaces/lazyframe_namespace.py
--rw-r--r--   0        0        0     1001 2023-08-20 18:11:56.365258 polars_evm-0.1.3/polars_evm/namespaces/series_namespace.py
--rw-r--r--   0        0        0      445 2023-08-21 02:26:24.874448 polars_evm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 polars_evm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      217 2024-05-22 22:10:59.193667 polars_evm-0.1.4/.gitignore
+-rw-r--r--   0        0        0    10847 2024-05-22 22:10:59.193667 polars_evm-0.1.4/LICENSE-APACHE
+-rw-r--r--   0        0        0     1095 2024-05-22 22:10:59.193667 polars_evm-0.1.4/LICENSE-MIT
+-rw-r--r--   0        0        0     3168 2024-05-22 22:10:59.193667 polars_evm-0.1.4/README.md
+-rw-r--r--   0        0        0      160 2024-05-23 00:04:36.549539 polars_evm-0.1.4/polars_evm/__init__.py
+-rw-r--r--   0        0        0       84 2024-05-22 22:10:59.193667 polars_evm-0.1.4/polars_evm/_helpers/__init__.py
+-rw-r--r--   0        0        0     2426 2024-05-22 22:10:59.193667 polars_evm-0.1.4/polars_evm/_helpers/encoding_conversions.py
+-rw-r--r--   0        0        0      155 2024-05-22 22:10:59.193667 polars_evm-0.1.4/polars_evm/_helpers/formatting.py
+-rw-r--r--   0        0        0     1093 2024-05-22 22:10:59.193667 polars_evm-0.1.4/polars_evm/_helpers/hashes.py
+-rw-r--r--   0        0        0      121 2024-05-22 22:10:59.193667 polars_evm-0.1.4/polars_evm/namespaces/__init__.py
+-rw-r--r--   0        0        0      935 2024-05-22 22:10:59.193667 polars_evm-0.1.4/polars_evm/namespaces/df_namespace.py
+-rw-r--r--   0        0        0     1067 2024-05-22 22:10:59.193667 polars_evm-0.1.4/polars_evm/namespaces/expr_namespace.py
+-rw-r--r--   0        0        0     1614 2024-05-22 22:10:59.193667 polars_evm-0.1.4/polars_evm/namespaces/lazyframe_namespace.py
+-rw-r--r--   0        0        0     1001 2024-05-22 22:10:59.193667 polars_evm-0.1.4/polars_evm/namespaces/series_namespace.py
+-rw-r--r--   0        0        0        0 2024-05-22 22:12:24.777515 polars_evm-0.1.4/polars_evm/py.typed
+-rw-r--r--   0        0        0      445 2024-05-22 22:10:59.193667 polars_evm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 polars_evm-0.1.4/PKG-INFO
```

### Comparing `polars_evm-0.1.3/LICENSE-APACHE` & `polars_evm-0.1.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `polars_evm-0.1.3/LICENSE-MIT` & `polars_evm-0.1.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `polars_evm-0.1.3/README.md` & `polars_evm-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `polars_evm-0.1.3/polars_evm/_helpers/encoding_conversions.py` & `polars_evm-0.1.4/polars_evm/_helpers/encoding_conversions.py`

 * *Files identical despite different names*

### Comparing `polars_evm-0.1.3/polars_evm/_helpers/hashes.py` & `polars_evm-0.1.4/polars_evm/_helpers/hashes.py`

 * *Files identical despite different names*

### Comparing `polars_evm-0.1.3/polars_evm/namespaces/df_namespace.py` & `polars_evm-0.1.4/polars_evm/namespaces/df_namespace.py`

 * *Files identical despite different names*

### Comparing `polars_evm-0.1.3/polars_evm/namespaces/expr_namespace.py` & `polars_evm-0.1.4/polars_evm/namespaces/expr_namespace.py`

 * *Files identical despite different names*

### Comparing `polars_evm-0.1.3/polars_evm/namespaces/lazyframe_namespace.py` & `polars_evm-0.1.4/polars_evm/namespaces/lazyframe_namespace.py`

 * *Files identical despite different names*

### Comparing `polars_evm-0.1.3/polars_evm/namespaces/series_namespace.py` & `polars_evm-0.1.4/polars_evm/namespaces/series_namespace.py`

 * *Files identical despite different names*

### Comparing `polars_evm-0.1.3/PKG-INFO` & `polars_evm-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_evm
-Version: 0.1.3
+Version: 0.1.4
 Summary: Utilities for working with EVM data in polars
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pycryptodome >=3.9.1, <4
 Project-URL: Source, https://github.com/sslivkoff/polars_evm
```

