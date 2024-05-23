# Comparing `tmp/wagtail_translatableforms-0.1.1.tar.gz` & `tmp/wagtail_translatableforms-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_translatableforms-0.1.1.tar", max compression
+gzip compressed data, was "wagtail_translatableforms-0.1.2.tar", max compression
```

## Comparing `wagtail_translatableforms-0.1.1.tar` & `wagtail_translatableforms-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1069 2024-05-21 15:01:21.958783 wagtail_translatableforms-0.1.1/LICENSE
--rw-r--r--   0        0        0     2665 2024-05-22 14:52:37.224227 wagtail_translatableforms-0.1.1/README.md
--rw-r--r--   0        0        0      567 2024-05-22 14:52:07.159544 wagtail_translatableforms-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      977 2024-05-22 11:16:42.552643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/__init__.py
--rw-r--r--   0        0        0     4656 2024-05-22 14:05:58.582858 wagtail_translatableforms-0.1.1/wagtail_translatableforms/apps.py
--rw-r--r--   0        0        0     1467 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/blocks.py
--rw-r--r--   0        0        0     8600 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/migrations/__init__.py
--rw-r--r--   0        0        0     5689 2024-05-22 11:16:42.560643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/models.py
--rw-r--r--   0        0        0     1777 2024-05-22 11:32:03.624558 wagtail_translatableforms-0.1.1/wagtail_translatableforms/serializers.py
--rw-r--r--   0        0        0     1046 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/confirm_delete.html
--rw-r--r--   0        0        0     4945 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/index.html
--rw-r--r--   0        0        0     4124 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/index_submissions.html
--rw-r--r--   0        0        0     1047 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/result_list.html
--rw-r--r--   0        0        0        0 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/templatetags/__init__.py
--rw-r--r--   0        0        0     4593 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/templatetags/custom_tags.py
--rw-r--r--   0        0        0      405 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/urls.py
--rw-r--r--   0        0        0     1155 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/utils.py
--rw-r--r--   0        0        0     4137 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.1/wagtail_translatableforms/views.py
--rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 wagtail_translatableforms-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-21 15:01:21.958783 wagtail_translatableforms-0.1.2/LICENSE
+-rw-r--r--   0        0        0    10792 2024-05-23 07:15:10.620068 wagtail_translatableforms-0.1.2/README.md
+-rw-r--r--   0        0        0      567 2024-05-23 07:16:09.733059 wagtail_translatableforms-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      977 2024-05-22 11:16:42.552643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/__init__.py
+-rw-r--r--   0        0        0     4656 2024-05-22 14:05:58.582858 wagtail_translatableforms-0.1.2/wagtail_translatableforms/apps.py
+-rw-r--r--   0        0        0     1467 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/blocks.py
+-rw-r--r--   0        0        0     8600 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/migrations/__init__.py
+-rw-r--r--   0        0        0     5689 2024-05-22 11:16:42.560643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/models.py
+-rw-r--r--   0        0        0     1777 2024-05-22 11:32:03.624558 wagtail_translatableforms-0.1.2/wagtail_translatableforms/serializers.py
+-rw-r--r--   0        0        0     1046 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/confirm_delete.html
+-rw-r--r--   0        0        0     4945 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/index.html
+-rw-r--r--   0        0        0     4124 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/index_submissions.html
+-rw-r--r--   0        0        0     1047 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/result_list.html
+-rw-r--r--   0        0        0        0 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/templatetags/__init__.py
+-rw-r--r--   0        0        0     4593 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/templatetags/custom_tags.py
+-rw-r--r--   0        0        0      405 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/urls.py
+-rw-r--r--   0        0        0     1155 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/utils.py
+-rw-r--r--   0        0        0     4137 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/views.py
+-rw-r--r--   0        0        0    11597 1970-01-01 00:00:00.000000 wagtail_translatableforms-0.1.2/PKG-INFO
```

### Comparing `wagtail_translatableforms-0.1.1/LICENSE` & `wagtail_translatableforms-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/pyproject.toml` & `wagtail_translatableforms-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "wagtail_translatableforms"
-version = "0.1.1"
+version = "0.1.2"
 description = "Add translatableforms to wagtail projects"
 authors = ["Egor Nikitin <eanikitin90@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/BenderEg/wagtail-translatableforms"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/__init__.py` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/apps.py` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/apps.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/blocks.py` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/migrations/0001_initial.py` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/models.py` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/serializers.py` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/serializers.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/confirm_delete.html` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/index.html` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/index.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/index_submissions.html` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/index_submissions.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/templates/customforms/result_list.html` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/result_list.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/templatetags/custom_tags.py` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/templatetags/custom_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/utils.py` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.1/wagtail_translatableforms/views.py` & `wagtail_translatableforms-0.1.2/wagtail_translatableforms/views.py`

 * *Files identical despite different names*

