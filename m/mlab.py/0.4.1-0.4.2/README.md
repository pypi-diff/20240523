# Comparing `tmp/mlab_py-0.4.1.tar.gz` & `tmp/mlab_py-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlab_py-0.4.1.tar", max compression
+gzip compressed data, was "mlab_py-0.4.2.tar", max compression
```

## Comparing `mlab_py-0.4.1.tar` & `mlab_py-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        8 2024-05-22 22:06:07.525956 mlab_py-0.4.1/README.md
--rw-r--r--   0        0        0      183 2024-05-22 23:41:07.584992 mlab_py-0.4.1/pymlab/__init__.py
--rw-r--r--   0        0        0     2628 2024-05-22 23:41:33.152267 mlab_py-0.4.1/pymlab/m_test.py
--rw-r--r--   0        0        0     2579 2024-05-23 07:44:35.413735 mlab_py-0.4.1/pymlab/m_train.py
--rw-r--r--   0        0        0     2337 2024-05-23 07:44:20.219924 mlab_py-0.4.1/pymlab/m_utils.py
--rw-r--r--   0        0        0      372 2024-05-23 07:45:07.768539 mlab_py-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 mlab_py-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0        8 2024-05-22 22:06:07.525956 mlab_py-0.4.2/README.md
+-rw-r--r--   0        0        0      183 2024-05-22 23:41:07.584992 mlab_py-0.4.2/pymlab/__init__.py
+-rw-r--r--   0        0        0     2628 2024-05-22 23:41:33.152267 mlab_py-0.4.2/pymlab/m_test.py
+-rw-r--r--   0        0        0     2579 2024-05-23 07:44:35.413735 mlab_py-0.4.2/pymlab/m_train.py
+-rw-r--r--   0        0        0     2337 2024-05-23 07:44:20.219924 mlab_py-0.4.2/pymlab/m_utils.py
+-rw-r--r--   0        0        0      371 2024-05-23 08:13:16.609174 mlab_py-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 mlab_py-0.4.2/PKG-INFO
```

### Comparing `mlab_py-0.4.1/pymlab/m_test.py` & `mlab_py-0.4.2/pymlab/m_test.py`

 * *Files identical despite different names*

### Comparing `mlab_py-0.4.1/pymlab/m_train.py` & `mlab_py-0.4.2/pymlab/m_train.py`

 * *Files identical despite different names*

### Comparing `mlab_py-0.4.1/pymlab/m_utils.py` & `mlab_py-0.4.2/pymlab/m_utils.py`

 * *Files identical despite different names*

