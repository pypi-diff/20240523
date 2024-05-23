# Comparing `tmp/wagtail_translatableforms-0.1.0.tar.gz` & `tmp/wagtail_translatableforms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_translatableforms-0.1.0.tar", max compression
+gzip compressed data, was "wagtail_translatableforms-0.1.1.tar", max compression
```

## Comparing `wagtail_translatableforms-0.1.0.tar` & `wagtail_translatableforms-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1069 2024-05-21 15:01:21.958783 wagtail_translatableforms-0.1.0/LICENSE
--rw-r--r--   0        0        0     2940 2024-05-22 14:27:52.018211 wagtail_translatableforms-0.1.0/README.md
--rw-r--r--   0        0        0      567 2024-05-22 14:50:33.257507 wagtail_translatableforms-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      977 2024-05-22 11:16:42.552643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/__init__.py
--rw-r--r--   0        0        0     4656 2024-05-22 14:05:58.582858 wagtail_translatableforms-0.1.0/wagtail_translatableforms/apps.py
--rw-r--r--   0        0        0     1467 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/blocks.py
--rw-r--r--   0        0        0     8600 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/migrations/__init__.py
--rw-r--r--   0        0        0     5689 2024-05-22 11:16:42.560643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/models.py
--rw-r--r--   0        0        0     1777 2024-05-22 11:32:03.624558 wagtail_translatableforms-0.1.0/wagtail_translatableforms/serializers.py
--rw-r--r--   0        0        0     1046 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/templates/customforms/confirm_delete.html
--rw-r--r--   0        0        0     4945 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/templates/customforms/index.html
--rw-r--r--   0        0        0     4124 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/templates/customforms/index_submissions.html
--rw-r--r--   0        0        0     1047 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/templates/customforms/result_list.html
--rw-r--r--   0        0        0        0 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/templatetags/__init__.py
--rw-r--r--   0        0        0     4593 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/templatetags/custom_tags.py
--rw-r--r--   0        0        0      405 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/urls.py
--rw-r--r--   0        0        0     1155 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/utils.py
--rw-r--r--   0        0        0     4137 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.0/wagtail_translatableforms/views.py
--rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 wagtail_translatableforms-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-21 15:01:21.958783 wagtail_translatableforms-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2665 2024-05-22 14:52:37.224227 wagtail_translatableforms-0.1.1/README.md
+-rw-r--r--   0        0        0      567 2024-05-22 14:52:07.159544 wagtail_translatableforms-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      977 2024-05-22 11:16:42.552643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/__init__.py
+-rw-r--r--   0        0        0     4656 2024-05-22 14:05:58.582858 wagtail_translatableforms-0.1.1/wagtail_translatableforms/apps.py
+-rw-r--r--   0        0        0     1467 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/blocks.py
+-rw-r--r--   0        0        0     8600 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/migrations/__init__.py
+-rw-r--r--   0        0        0     5689 2024-05-22 11:16:42.560643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/models.py
+-rw-r--r--   0        0        0     1777 2024-05-22 11:32:03.624558 wagtail_translatableforms-0.1.1/wagtail_translatableforms/serializers.py
+-rw-r--r--   0        0        0     1046 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/confirm_delete.html
+-rw-r--r--   0        0        0     4945 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/index.html
+-rw-r--r--   0        0        0     4124 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/index_submissions.html
+-rw-r--r--   0        0        0     1047 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/result_list.html
+-rw-r--r--   0        0        0        0 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/templatetags/__init__.py
+-rw-r--r--   0        0        0     4593 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/templatetags/custom_tags.py
+-rw-r--r--   0        0        0      405 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/urls.py
+-rw-r--r--   0        0        0     1155 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/utils.py
+-rw-r--r--   0        0        0     4137 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/views.py
+-rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 wagtail_translatableforms-0.1.1/PKG-INFO
```

### Comparing `wagtail_translatableforms-0.1.0/LICENSE` & `wagtail_translatableforms-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/README.md` & `wagtail_translatableforms-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 Wagtail Translatableforms is an additional plagin for [Wagtail CMS](https://wagtail.org/).
 It is based on [Wagtail Localize](https://pypi.org/project/wagtail-localize/), [Wagtailstreamforms](https://pypi.org/project/wagtailstreamforms/) and [Django](https://www.djangoproject.com/).
 
 The main idea is to transform wagtailstreamform into translatable wagtail snippet and at the same time maintain wagtailstreamform fuctionality.
 
 ## Table of Contents
 
-- [Requirements](https://pypi.org/project/wagtail_translatableforms/#requirements)
-- [Installation](https://test.pypi.org/project/wagtail_translatableforms/#installation)
-- [Usage](https://test.pypi.org/project/wagtail_translatableforms/#usage)
-- [License](https://test.pypi.org/project/wagtail_translatableforms/#license)
+- Requirements
+- Installation
+- Usage
+- License
 
 
 ## Requirements
 
 * django = "^4.2.11";
 * djangorestframework = ^3.15.0";
 * drf_spectacular = "^0.27.1"
```

### Comparing `wagtail_translatableforms-0.1.0/pyproject.toml` & `wagtail_translatableforms-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "wagtail_translatableforms"
-version = "0.1.0"
+version = "0.1.1"
 description = "Add translatableforms to wagtail projects"
 authors = ["Egor Nikitin <eanikitin90@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/BenderEg/wagtail-translatableforms"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/__init__.py` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/apps.py` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/apps.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/blocks.py` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/migrations/0001_initial.py` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/models.py` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/serializers.py` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/serializers.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/templates/customforms/confirm_delete.html` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/templates/customforms/index.html` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/index.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/templates/customforms/index_submissions.html` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/index_submissions.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/templates/customforms/result_list.html` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/result_list.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/templatetags/custom_tags.py` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/templatetags/custom_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/utils.py` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/wagtail_translatableforms/views.py` & `wagtail_translatableforms-0.1.1/wagtail_translatableforms/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.0/PKG-INFO` & `wagtail_translatableforms-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_translatableforms
-Version: 0.1.0
+Version: 0.1.1
 Summary: Add translatableforms to wagtail projects
 Home-page: https://github.com/BenderEg/wagtail-translatableforms
 License: MIT
 Author: Egor Nikitin
 Author-email: eanikitin90@gmail.com
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -24,18 +24,18 @@
 Wagtail Translatableforms is an additional plagin for [Wagtail CMS](https://wagtail.org/).
 It is based on [Wagtail Localize](https://pypi.org/project/wagtail-localize/), [Wagtailstreamforms](https://pypi.org/project/wagtailstreamforms/) and [Django](https://www.djangoproject.com/).
 
 The main idea is to transform wagtailstreamform into translatable wagtail snippet and at the same time maintain wagtailstreamform fuctionality.
 
 ## Table of Contents
 
-- [Requirements](https://pypi.org/project/wagtail_translatableforms/#requirements)
-- [Installation](https://test.pypi.org/project/wagtail_translatableforms/#installation)
-- [Usage](https://test.pypi.org/project/wagtail_translatableforms/#usage)
-- [License](https://test.pypi.org/project/wagtail_translatableforms/#license)
+- Requirements
+- Installation
+- Usage
+- License
 
 
 ## Requirements
 
 * django = "^4.2.11";
 * djangorestframework = ^3.15.0";
 * drf_spectacular = "^0.27.1"
```

