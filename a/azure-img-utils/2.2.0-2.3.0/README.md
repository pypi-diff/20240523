# Comparing `tmp/azure-img-utils-2.2.0.tar.gz` & `tmp/azure_img_utils-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-img-utils-2.2.0.tar", last modified: Fri Mar  8 19:10:44 2024, max compression
+gzip compressed data, was "azure_img_utils-2.3.0.tar", last modified: Thu May 23 20:26:05 2024, max compression
```

## Comparing `azure-img-utils-2.2.0.tar` & `azure_img_utils-2.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:10:44.197136 azure-img-utils-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    32403 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20688 2024-03-08 19:10:44.197136 azure-img-utils-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19076 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:10:44.193136 azure-img-utils-2.2.0/azure_img_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    27152 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/azure_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:10:44.193136 azure-img-utils-2.2.0/azure_img_utils/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/cli/blob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/cli/gallery_image_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11567 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/cli/offer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/cloud_partner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/azure_img_utils/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:10:44.197136 azure-img-utils-2.2.0/azure_img_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20688 2024-03-08 19:10:44.000000 azure-img-utils-2.2.0/azure_img_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-08 19:10:44.000000 azure-img-utils-2.2.0/azure_img_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 19:10:44.000000 azure-img-utils-2.2.0/azure_img_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-08 19:10:44.000000 azure-img-utils-2.2.0/azure_img_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 19:10:44.000000 azure-img-utils-2.2.0/azure_img_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-08 19:10:44.000000 azure-img-utils-2.2.0/azure_img_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-08 19:10:44.000000 azure-img-utils-2.2.0/azure_img_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-08 19:10:44.197136 azure-img-utils-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:10:44.197136 azure-img-utils-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/creds.json
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/example_file.img.xz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/image.raw
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/test_azure_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/test_azure_cloud_partner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/test_azure_gallery_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/test_azure_image_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/test_azure_image_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    55523 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/test_cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/test_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-08 19:10:35.000000 azure-img-utils-2.2.0/tests/unknown_keyword.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:26:05.341546 azure_img_utils-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32403 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-23 20:26:05.341546 azure_img_utils-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19076 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:26:05.333546 azure_img_utils-2.3.0/azure_img_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27152 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/azure_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:26:05.337546 azure_img_utils-2.3.0/azure_img_utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/cli/blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/cli/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/cli/gallery_image_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11567 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/cli/offer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/cloud_partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/azure_img_utils/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:26:05.341546 azure_img_utils-2.3.0/azure_img_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-23 20:26:05.000000 azure_img_utils-2.3.0/azure_img_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-23 20:26:05.000000 azure_img_utils-2.3.0/azure_img_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:26:05.000000 azure_img_utils-2.3.0/azure_img_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-23 20:26:05.000000 azure_img_utils-2.3.0/azure_img_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:26:05.000000 azure_img_utils-2.3.0/azure_img_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-23 20:26:05.000000 azure_img_utils-2.3.0/azure_img_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 20:26:05.000000 azure_img_utils-2.3.0/azure_img_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-23 20:26:05.341546 azure_img_utils-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:26:05.341546 azure_img_utils-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/creds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/example_file.img.xz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/image.raw
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/test_azure_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/test_azure_cloud_partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/test_azure_gallery_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/test_azure_image_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/test_azure_image_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55523 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/test_cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/test_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-23 20:25:56.000000 azure_img_utils-2.3.0/tests/unknown_keyword.yaml
```

### Comparing `azure-img-utils-2.2.0/CHANGES.md` & `azure_img_utils-2.3.0/CHANGES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v2.3.0 (2024-05-23)
+===================
+
+- Update spec for python 3.11 build
+
 v2.2.0 (2024-03-08)
 ===================
 
 - Add optional wait arg to submit_request
 - Do not wait on publish or go live operations
 
 v2.1.0 (2024-03-06)
```

### Comparing `azure-img-utils-2.2.0/CONTRIBUTING.md` & `azure_img_utils-2.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/LICENSE` & `azure_img_utils-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/PKG-INFO` & `azure_img_utils-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: azure-img-utils
-Version: 2.2.0
+Version: 2.3.0
 Summary: Package that provides utilities for handling images in Azure Cloud.
 Home-page: https://github.com/SUSE-Enceladus/azure-img-utils
 Author: SUSE
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Keywords: azure-img-utils azure_img_utils
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Software Distribution
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: msal
 Requires-Dist: azure-identity
 Requires-Dist: azure-mgmt-compute>=26.1.0
 Requires-Dist: azure-mgmt-storage
```

### Comparing `azure-img-utils-2.2.0/README.md` & `azure_img_utils-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/__init__.py` & `azure_img_utils-2.3.0/azure_img_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __author__ = """SUSE"""
 __email__ = 'public-cloud-dev@susecloud.net'
-__version__ = '2.2.0'
+__version__ = '2.3.0'
```

### Comparing `azure-img-utils-2.2.0/azure_img_utils/auth.py` & `azure_img_utils-2.3.0/azure_img_utils/auth.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/azure_image.py` & `azure_img_utils-2.3.0/azure_img_utils/azure_image.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/cli/blob.py` & `azure_img_utils-2.3.0/azure_img_utils/cli/blob.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/cli/cli.py` & `azure_img_utils-2.3.0/azure_img_utils/cli/cli.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/cli/cli_utils.py` & `azure_img_utils-2.3.0/azure_img_utils/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/cli/gallery_image_version.py` & `azure_img_utils-2.3.0/azure_img_utils/cli/gallery_image_version.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/cli/image.py` & `azure_img_utils-2.3.0/azure_img_utils/cli/image.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/cli/offer.py` & `azure_img_utils-2.3.0/azure_img_utils/cli/offer.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/cloud_partner.py` & `azure_img_utils-2.3.0/azure_img_utils/cloud_partner.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/compute.py` & `azure_img_utils-2.3.0/azure_img_utils/compute.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/exceptions.py` & `azure_img_utils-2.3.0/azure_img_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/filetype.py` & `azure_img_utils-2.3.0/azure_img_utils/filetype.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils/storage.py` & `azure_img_utils-2.3.0/azure_img_utils/storage.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/azure_img_utils.egg-info/PKG-INFO` & `azure_img_utils-2.3.0/azure_img_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: azure-img-utils
-Version: 2.2.0
+Version: 2.3.0
 Summary: Package that provides utilities for handling images in Azure Cloud.
 Home-page: https://github.com/SUSE-Enceladus/azure-img-utils
 Author: SUSE
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Keywords: azure-img-utils azure_img_utils
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Software Distribution
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: msal
 Requires-Dist: azure-identity
 Requires-Dist: azure-mgmt-compute>=26.1.0
 Requires-Dist: azure-mgmt-storage
```

### Comparing `azure-img-utils-2.2.0/azure_img_utils.egg-info/SOURCES.txt` & `azure_img_utils-2.3.0/azure_img_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/setup.py` & `azure_img_utils-2.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 with open('requirements-dev.txt') as req_file:
     dev_requirements = test_requirements + req_file.read().splitlines()[2:]
 
 
 setup(
     name='azure-img-utils',
-    version='2.2.0',
+    version='2.3.0',
     description='Package that provides utilities for '
                 'handling images in Azure Cloud.',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='SUSE',
     author_email='public-cloud-dev@susecloud.net',
     url='https://github.com/SUSE-Enceladus/azure-img-utils',
@@ -52,15 +52,15 @@
     },
     entry_points={
         'console_scripts': [
             'azure-img-utils=azure_img_utils.cli.cli:az_img_utils'
         ]
     },
     include_package_data=True,
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     install_requires=requirements,
     extras_require={
         'dev': dev_requirements,
         'test': test_requirements
     },
     license='GPLv3+',
     zip_safe=False,
@@ -70,13 +70,15 @@
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Topic :: System :: Software Distribution',
         'License :: OSI Approved :: '
         'GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

### Comparing `azure-img-utils-2.2.0/tests/creds.json` & `azure_img_utils-2.3.0/tests/creds.json`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/tests/test_azure_auth.py` & `azure_img_utils-2.3.0/tests/test_azure_auth.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/tests/test_azure_cloud_partner.py` & `azure_img_utils-2.3.0/tests/test_azure_cloud_partner.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/tests/test_azure_gallery_images.py` & `azure_img_utils-2.3.0/tests/test_azure_gallery_images.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/tests/test_azure_image_compute.py` & `azure_img_utils-2.3.0/tests/test_azure_image_compute.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/tests/test_azure_image_storage.py` & `azure_img_utils-2.3.0/tests/test_azure_image_storage.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/tests/test_cli.py` & `azure_img_utils-2.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/tests/test_cli_utils.py` & `azure_img_utils-2.3.0/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `azure-img-utils-2.2.0/tests/test_storage_utils.py` & `azure_img_utils-2.3.0/tests/test_storage_utils.py`

 * *Files identical despite different names*

