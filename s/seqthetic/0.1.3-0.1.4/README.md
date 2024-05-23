# Comparing `tmp/seqthetic-0.1.3.tar.gz` & `tmp/seqthetic-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqthetic-0.1.3.tar", max compression
+gzip compressed data, was "seqthetic-0.1.4.tar", max compression
```

## Comparing `seqthetic-0.1.3.tar` & `seqthetic-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      741 2024-05-23 06:46:15.396075 seqthetic-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    12058 2024-05-14 07:00:49.209241 seqthetic-0.1.3/readme.md
--rw-r--r--   0        0        0      162 2024-05-23 06:46:04.206673 seqthetic-0.1.3/seqthetic/__init__.py
--rw-r--r--   0        0        0     2934 2024-05-23 06:44:17.166835 seqthetic-0.1.3/seqthetic/dataset.py
--rw-r--r--   0        0        0      562 2024-05-14 04:17:11.407174 seqthetic-0.1.3/seqthetic/dependencies/__init__.py
--rw-r--r--   0        0        0      883 2024-05-14 03:57:53.546887 seqthetic-0.1.3/seqthetic/dependencies/adapter.py
--rw-r--r--   0        0        0     1795 2024-05-14 04:32:16.874428 seqthetic-0.1.3/seqthetic/dependencies/base.py
--rw-r--r--   0        0        0     2534 2024-05-08 02:35:11.698745 seqthetic-0.1.3/seqthetic/dependencies/fbm.py
--rw-r--r--   0        0        0     1882 2024-05-07 07:27:35.421846 seqthetic-0.1.3/seqthetic/dependencies/function.py
--rw-r--r--   0        0        0     1500 2024-05-07 07:27:35.425272 seqthetic-0.1.3/seqthetic/dependencies/random.py
--rw-r--r--   0        0        0     2798 2024-05-07 07:27:35.369313 seqthetic-0.1.3/seqthetic/mapping.py
--rw-r--r--   0        0        0     1305 2024-05-08 11:53:41.162062 seqthetic-0.1.3/seqthetic/range.py
--rw-r--r--   0        0        0     1246 2024-05-15 02:19:29.918718 seqthetic-0.1.3/seqthetic/seed.py
--rw-r--r--   0        0        0     4075 2024-05-09 06:40:31.603486 seqthetic-0.1.3/seqthetic/spec_variation.py
--rw-r--r--   0        0        0     5704 2024-05-15 02:55:53.636248 seqthetic-0.1.3/seqthetic/synthesis_spec.py
--rw-r--r--   0        0        0     3647 2024-05-15 02:51:58.490011 seqthetic-0.1.3/seqthetic/synthesizer.py
--rw-r--r--   0        0        0     1349 2024-05-09 06:38:18.422069 seqthetic-0.1.3/seqthetic/utils.py
--rw-r--r--   0        0        0        0 2024-05-07 12:03:34.624527 seqthetic-0.1.3/seqthetic/vary/__init__.py
--rw-r--r--   0        0        0      709 2024-05-09 04:33:48.215716 seqthetic-0.1.3/seqthetic/vary/compose_ops.py
--rw-r--r--   0        0        0     1475 2024-05-07 16:38:49.316467 seqthetic-0.1.3/seqthetic/vary/compute_ops.py
--rw-r--r--   0        0        0     1232 2024-05-08 12:19:45.887199 seqthetic-0.1.3/seqthetic/vary/domain_ops.py
--rw-r--r--   0        0        0     5426 2024-05-14 04:32:16.874428 seqthetic-0.1.3/seqthetic/vary/transform.py
--rw-r--r--   0        0        0      954 2024-05-08 03:02:01.961163 seqthetic-0.1.3/seqthetic/vary/variation.py
--rw-r--r--   0        0        0     4102 2024-05-14 04:41:06.866213 seqthetic-0.1.3/seqthetic/vary/variator.py
--rw-r--r--   0        0        0     4526 2024-05-15 03:27:39.863802 seqthetic-0.1.3/seqthetic/vocabulary.py
--rw-r--r--   0        0        0    12500 1970-01-01 00:00:00.000000 seqthetic-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      741 2024-05-23 06:48:36.385826 seqthetic-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    12058 2024-05-14 07:00:49.209241 seqthetic-0.1.4/readme.md
+-rw-r--r--   0        0        0      216 2024-05-23 06:48:22.854947 seqthetic-0.1.4/seqthetic/__init__.py
+-rw-r--r--   0        0        0     2934 2024-05-23 06:44:17.166835 seqthetic-0.1.4/seqthetic/dataset.py
+-rw-r--r--   0        0        0      562 2024-05-14 04:17:11.407174 seqthetic-0.1.4/seqthetic/dependencies/__init__.py
+-rw-r--r--   0        0        0      883 2024-05-14 03:57:53.546887 seqthetic-0.1.4/seqthetic/dependencies/adapter.py
+-rw-r--r--   0        0        0     1795 2024-05-14 04:32:16.874428 seqthetic-0.1.4/seqthetic/dependencies/base.py
+-rw-r--r--   0        0        0     2534 2024-05-08 02:35:11.698745 seqthetic-0.1.4/seqthetic/dependencies/fbm.py
+-rw-r--r--   0        0        0     1882 2024-05-07 07:27:35.421846 seqthetic-0.1.4/seqthetic/dependencies/function.py
+-rw-r--r--   0        0        0     1500 2024-05-07 07:27:35.425272 seqthetic-0.1.4/seqthetic/dependencies/random.py
+-rw-r--r--   0        0        0     2798 2024-05-07 07:27:35.369313 seqthetic-0.1.4/seqthetic/mapping.py
+-rw-r--r--   0        0        0     1305 2024-05-08 11:53:41.162062 seqthetic-0.1.4/seqthetic/range.py
+-rw-r--r--   0        0        0     1246 2024-05-15 02:19:29.918718 seqthetic-0.1.4/seqthetic/seed.py
+-rw-r--r--   0        0        0     4075 2024-05-09 06:40:31.603486 seqthetic-0.1.4/seqthetic/spec_variation.py
+-rw-r--r--   0        0        0     5704 2024-05-15 02:55:53.636248 seqthetic-0.1.4/seqthetic/synthesis_spec.py
+-rw-r--r--   0        0        0     3647 2024-05-15 02:51:58.490011 seqthetic-0.1.4/seqthetic/synthesizer.py
+-rw-r--r--   0        0        0     1349 2024-05-09 06:38:18.422069 seqthetic-0.1.4/seqthetic/utils.py
+-rw-r--r--   0        0        0        0 2024-05-07 12:03:34.624527 seqthetic-0.1.4/seqthetic/vary/__init__.py
+-rw-r--r--   0        0        0      709 2024-05-09 04:33:48.215716 seqthetic-0.1.4/seqthetic/vary/compose_ops.py
+-rw-r--r--   0        0        0     1475 2024-05-07 16:38:49.316467 seqthetic-0.1.4/seqthetic/vary/compute_ops.py
+-rw-r--r--   0        0        0     1232 2024-05-08 12:19:45.887199 seqthetic-0.1.4/seqthetic/vary/domain_ops.py
+-rw-r--r--   0        0        0     5426 2024-05-14 04:32:16.874428 seqthetic-0.1.4/seqthetic/vary/transform.py
+-rw-r--r--   0        0        0      954 2024-05-08 03:02:01.961163 seqthetic-0.1.4/seqthetic/vary/variation.py
+-rw-r--r--   0        0        0     4102 2024-05-14 04:41:06.866213 seqthetic-0.1.4/seqthetic/vary/variator.py
+-rw-r--r--   0        0        0     4526 2024-05-15 03:27:39.863802 seqthetic-0.1.4/seqthetic/vocabulary.py
+-rw-r--r--   0        0        0    12500 1970-01-01 00:00:00.000000 seqthetic-0.1.4/PKG-INFO
```

### Comparing `seqthetic-0.1.3/pyproject.toml` & `seqthetic-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seqthetic"
-version = "0.1.3"
+version = "0.1.4"
 description = "Creates sequence data for pretraining and benchmarking sequence models"
 authors = ["Shom <shaomi_lin@126.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple/"
```

### Comparing `seqthetic-0.1.3/readme.md` & `seqthetic-0.1.4/readme.md`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/dataset.py` & `seqthetic-0.1.4/seqthetic/dataset.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/dependencies/__init__.py` & `seqthetic-0.1.4/seqthetic/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/dependencies/adapter.py` & `seqthetic-0.1.4/seqthetic/dependencies/adapter.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/dependencies/base.py` & `seqthetic-0.1.4/seqthetic/dependencies/base.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/dependencies/fbm.py` & `seqthetic-0.1.4/seqthetic/dependencies/fbm.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/dependencies/function.py` & `seqthetic-0.1.4/seqthetic/dependencies/function.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/dependencies/random.py` & `seqthetic-0.1.4/seqthetic/dependencies/random.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/mapping.py` & `seqthetic-0.1.4/seqthetic/mapping.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/range.py` & `seqthetic-0.1.4/seqthetic/range.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/seed.py` & `seqthetic-0.1.4/seqthetic/seed.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/spec_variation.py` & `seqthetic-0.1.4/seqthetic/spec_variation.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/synthesis_spec.py` & `seqthetic-0.1.4/seqthetic/synthesis_spec.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/synthesizer.py` & `seqthetic-0.1.4/seqthetic/synthesizer.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/utils.py` & `seqthetic-0.1.4/seqthetic/utils.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/vary/compose_ops.py` & `seqthetic-0.1.4/seqthetic/vary/compose_ops.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/vary/compute_ops.py` & `seqthetic-0.1.4/seqthetic/vary/compute_ops.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/vary/domain_ops.py` & `seqthetic-0.1.4/seqthetic/vary/domain_ops.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/vary/transform.py` & `seqthetic-0.1.4/seqthetic/vary/transform.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/vary/variation.py` & `seqthetic-0.1.4/seqthetic/vary/variation.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/vary/variator.py` & `seqthetic-0.1.4/seqthetic/vary/variator.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/seqthetic/vocabulary.py` & `seqthetic-0.1.4/seqthetic/vocabulary.py`

 * *Files identical despite different names*

### Comparing `seqthetic-0.1.3/PKG-INFO` & `seqthetic-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqthetic
-Version: 0.1.3
+Version: 0.1.4
 Summary: Creates sequence data for pretraining and benchmarking sequence models
 Author: Shom
 Author-email: shaomi_lin@126.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: flake8 (>=7.0.0,<8.0.0)
```

