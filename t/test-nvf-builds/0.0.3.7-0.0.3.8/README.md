# Comparing `tmp/test_nvf_builds-0.0.3.7.tar.gz` & `tmp/test_nvf_builds-0.0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_nvf_builds-0.0.3.7.tar", last modified: Thu May 23 08:43:35 2024, max compression
+gzip compressed data, was "test_nvf_builds-0.0.3.8.tar", last modified: Thu May 23 10:55:54 2024, max compression
```

## Comparing `test_nvf_builds-0.0.3.7.tar` & `test_nvf_builds-0.0.3.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.872050 test_nvf_builds-0.0.3.7/
--rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-07 07:57:47.000000 test_nvf_builds-0.0.3.7/LICENSE
--rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-23 08:43:35.871952 test_nvf_builds-0.0.3.7/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.3.7/README.md
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.868681 test_nvf_builds-0.0.3.7/oasysnow/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.3.7/oasysnow/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.868776 test_nvf_builds-0.0.3.7/oasysnow/federated/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.868872 test_nvf_builds-0.0.3.7/oasysnow/federated/client/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/client/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.869198 test_nvf_builds-0.0.3.7/oasysnow/federated/client/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/client/filters/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2241 2024-05-23 08:40:50.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/client/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2190 2024-05-23 08:41:25.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/client/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.869418 test_nvf_builds-0.0.3.7/oasysnow/federated/client/trainer/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/client/trainer/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4477 2024-05-23 08:41:46.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/client/trainer/trainer.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.869547 test_nvf_builds-0.0.3.7/oasysnow/federated/common/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-15 14:50:33.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.869868 test_nvf_builds-0.0.3.7/oasysnow/federated/common/attestation_service/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/attestation_service/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1707 2024-05-23 08:37:40.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/attestation_service/server.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1338 2024-05-23 08:42:14.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/attestation_service/verification.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.870199 test_nvf_builds-0.0.3.7/oasysnow/federated/common/model/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/model/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1803 2024-05-15 14:55:57.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/model/gennet_model.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1288 2024-05-15 14:55:47.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/model/global_model.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.870321 test_nvf_builds-0.0.3.7/oasysnow/federated/server/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/server/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.870657 test_nvf_builds-0.0.3.7/oasysnow/federated/server/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/server/filters/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2311 2024-05-23 08:42:28.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/server/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2132 2024-05-23 08:42:43.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/server/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.870875 test_nvf_builds-0.0.3.7/oasysnow/federated/server/model_runner/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/server/model_runner/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4843 2024-05-15 14:56:24.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/server/model_runner/model_runner.py
--rw-r--r--   0 mostafa    (501) staff       (20)       29 2024-05-15 14:24:19.000000 test_nvf_builds-0.0.3.7/requirements.txt
--rw-r--r--   0 mostafa    (501) staff       (20)      479 2024-05-23 08:43:35.872558 test_nvf_builds-0.0.3.7/setup.cfg
--rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.3.7/setup.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.871721 test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/
--rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-23 08:43:35.000000 test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)     1220 2024-05-23 08:43:35.000000 test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-23 08:43:35.000000 test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       28 2024-05-23 08:43:35.000000 test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/requires.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-23 08:43:35.000000 test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/top_level.txt
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.888802 test_nvf_builds-0.0.3.8/
+-rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-07 07:57:47.000000 test_nvf_builds-0.0.3.8/LICENSE
+-rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-23 10:55:54.888727 test_nvf_builds-0.0.3.8/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.3.8/README.md
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.883512 test_nvf_builds-0.0.3.8/oasysnow/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.3.8/oasysnow/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.883617 test_nvf_builds-0.0.3.8/oasysnow/federated/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.883719 test_nvf_builds-0.0.3.8/oasysnow/federated/client/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/client/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.884227 test_nvf_builds-0.0.3.8/oasysnow/federated/client/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/client/filters/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2241 2024-05-23 08:40:50.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/client/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2190 2024-05-23 08:41:25.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/client/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.884610 test_nvf_builds-0.0.3.8/oasysnow/federated/client/trainer/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/client/trainer/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4477 2024-05-23 08:41:46.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/client/trainer/trainer.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.884887 test_nvf_builds-0.0.3.8/oasysnow/federated/common/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-15 14:50:33.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/common/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.885446 test_nvf_builds-0.0.3.8/oasysnow/federated/common/attestation_service/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/common/attestation_service/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1707 2024-05-23 08:37:40.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/common/attestation_service/server.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1338 2024-05-23 08:42:14.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/common/attestation_service/verification.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.886069 test_nvf_builds-0.0.3.8/oasysnow/federated/common/model/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/common/model/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1803 2024-05-15 14:55:57.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/common/model/gennet_model.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1288 2024-05-15 14:55:47.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/common/model/global_model.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.886460 test_nvf_builds-0.0.3.8/oasysnow/federated/server/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/server/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.887119 test_nvf_builds-0.0.3.8/oasysnow/federated/server/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/server/filters/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2311 2024-05-23 08:42:28.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/server/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2132 2024-05-23 08:42:43.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/server/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.887555 test_nvf_builds-0.0.3.8/oasysnow/federated/server/model_runner/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/server/model_runner/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4843 2024-05-15 14:56:24.000000 test_nvf_builds-0.0.3.8/oasysnow/federated/server/model_runner/model_runner.py
+-rw-r--r--   0 mostafa    (501) staff       (20)       29 2024-05-15 14:24:19.000000 test_nvf_builds-0.0.3.8/requirements.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)      479 2024-05-23 10:55:54.889050 test_nvf_builds-0.0.3.8/setup.cfg
+-rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.3.8/setup.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 10:55:54.888484 test_nvf_builds-0.0.3.8/test_nvf_builds.egg-info/
+-rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-23 10:55:54.000000 test_nvf_builds-0.0.3.8/test_nvf_builds.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)     1220 2024-05-23 10:55:54.000000 test_nvf_builds-0.0.3.8/test_nvf_builds.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-23 10:55:54.000000 test_nvf_builds-0.0.3.8/test_nvf_builds.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       28 2024-05-23 10:55:54.000000 test_nvf_builds-0.0.3.8/test_nvf_builds.egg-info/requires.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-23 10:55:54.000000 test_nvf_builds-0.0.3.8/test_nvf_builds.egg-info/top_level.txt
```

### Comparing `test_nvf_builds-0.0.3.7/LICENSE` & `test_nvf_builds-0.0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.7/oasysnow/federated/client/filters/filter_data.py` & `test_nvf_builds-0.0.3.8/oasysnow/federated/client/filters/filter_data.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.7/oasysnow/federated/client/filters/filter_results.py` & `test_nvf_builds-0.0.3.8/oasysnow/federated/client/filters/filter_results.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.7/oasysnow/federated/client/trainer/trainer.py` & `test_nvf_builds-0.0.3.8/oasysnow/federated/client/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.7/oasysnow/federated/common/attestation_service/server.py` & `test_nvf_builds-0.0.3.8/oasysnow/federated/common/attestation_service/server.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.7/oasysnow/federated/common/attestation_service/verification.py` & `test_nvf_builds-0.0.3.8/oasysnow/federated/common/attestation_service/verification.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.7/oasysnow/federated/common/model/gennet_model.py` & `test_nvf_builds-0.0.3.8/oasysnow/federated/common/model/gennet_model.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.7/oasysnow/federated/common/model/global_model.py` & `test_nvf_builds-0.0.3.8/oasysnow/federated/common/model/global_model.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.7/oasysnow/federated/server/filters/filter_data.py` & `test_nvf_builds-0.0.3.8/oasysnow/federated/server/filters/filter_data.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.7/oasysnow/federated/server/filters/filter_results.py` & `test_nvf_builds-0.0.3.8/oasysnow/federated/server/filters/filter_results.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.7/oasysnow/federated/server/model_runner/model_runner.py` & `test_nvf_builds-0.0.3.8/oasysnow/federated/server/model_runner/model_runner.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/SOURCES.txt` & `test_nvf_builds-0.0.3.8/test_nvf_builds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

