# Comparing `tmp/dfds_ds_toolbox-0.9.1.tar.gz` & `tmp/dfds_ds_toolbox-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfds_ds_toolbox-0.9.1.tar", last modified: Wed Mar  2 09:36:49 2022, max compression
+gzip compressed data, was "dfds_ds_toolbox-0.9.2.tar", last modified: Wed Mar  2 12:42:35 2022, max compression
```

## Comparing `dfds_ds_toolbox-0.9.1.tar` & `dfds_ds_toolbox-0.9.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:49.559444 dfds_ds_toolbox-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4669 2022-03-02 09:36:49.559444 dfds_ds_toolbox-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4042 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:49.555443 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:49.555443 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/analysis/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9868 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/analysis/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)    10792 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/analysis/plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/exeptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:49.555443 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/feature_extraction/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/feature_extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:49.555443 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11233 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/feature_selection/feat_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:49.555443 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/logging/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:49.555443 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/model_selection/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/model_selection/model_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:49.559444 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/profiling/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/profiling/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 09:36:49.555443 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4669 2022-03-02 09:36:49.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-03-02 09:36:49.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-02 09:36:49.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-03-02 09:36:49.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-02 09:36:49.000000 dfds_ds_toolbox-0.9.1/dfds_ds_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-02 09:36:49.559444 dfds_ds_toolbox-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-03-02 09:36:27.000000 dfds_ds_toolbox-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:35.767310 dfds_ds_toolbox-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4669 2022-03-02 12:42:35.767310 dfds_ds_toolbox-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4042 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:35.763311 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:35.767310 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/analysis/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9868 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/analysis/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10792 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/analysis/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/exeptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:35.767310 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/feature_extraction/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/feature_extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:35.767310 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11233 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/feature_selection/feat_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:35.767310 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/logging/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3614 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:35.767310 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/model_selection/model_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:35.767310 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/profiling/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/profiling/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 12:42:35.767310 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4669 2022-03-02 12:42:35.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2022-03-02 12:42:35.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-02 12:42:35.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-03-02 12:42:35.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-02 12:42:35.000000 dfds_ds_toolbox-0.9.2/dfds_ds_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-02 12:42:35.767310 dfds_ds_toolbox-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      919 2022-03-02 12:42:22.000000 dfds_ds_toolbox-0.9.2/setup.py
```

### Comparing `dfds_ds_toolbox-0.9.1/LICENSE` & `dfds_ds_toolbox-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dfds_ds_toolbox-0.9.1/PKG-INFO` & `dfds_ds_toolbox-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfds_ds_toolbox
-Version: 0.9.1
+Version: 0.9.2
 Summary: A collection of tools for data science used at DFDS.
 Author: Data Science Chapter at DFDS
 Author-email: urcha@dfds.com
 License: UNKNOWN
 Keywords: dfds_ds_toolbox,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dfds_ds_toolbox-0.9.1/README.md` & `dfds_ds_toolbox-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/analysis/plotting.py` & `dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/analysis/plotting.py`

 * *Files identical despite different names*

### Comparing `dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/analysis/plotting_utils.py` & `dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/analysis/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/feature_selection/feat_selector.py` & `dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/feature_selection/feat_selector.py`

 * *Files identical despite different names*

### Comparing `dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/logging/logging.py` & `dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/logging/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         >>> logger = init_logger(stream_level="INFO", log_format="%(module)s - %(message)s", rich_handler_enabled=False)
         >>> logger.info("Custom log format.")
 
     """
 
     # Set up logger
     logger = logging.getLogger(name)
+    # Setting logger root level (it could be override by specific handler levels)
     logger.setLevel(logging.DEBUG)
     if rich_handler_enabled and log_format is not None:
         raise ValueError("Rich handler and custom log format cannot be used together")
     if log_format is None:
         log_format = LOG_FORMATS["STANDARD_FORMAT"]
 
     # Remove all attached handlers, in case there was
@@ -87,10 +88,11 @@
             level=stream_level, rich_tracebacks=True, log_time_format="[%Y-%m-%d %H:%M:%S,%f]"
         )
 
         handler.setFormatter(logging.Formatter(LOG_FORMATS["RICH_FORMAT"]))
     else:
         handler = logging.StreamHandler()
         handler.setFormatter(logging.Formatter(log_format))
+        handler.setLevel(level=stream_level)
     logger.addHandler(handler)
 
     return logger
```

### Comparing `dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/model_selection/model_selection.py` & `dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/model_selection/model_selection.py`

 * *Files identical despite different names*

### Comparing `dfds_ds_toolbox-0.9.1/dfds_ds_toolbox/profiling/profiling.py` & `dfds_ds_toolbox-0.9.2/dfds_ds_toolbox/profiling/profiling.py`

 * *Files identical despite different names*

### Comparing `dfds_ds_toolbox-0.9.1/dfds_ds_toolbox.egg-info/PKG-INFO` & `dfds_ds_toolbox-0.9.2/dfds_ds_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfds-ds-toolbox
-Version: 0.9.1
+Version: 0.9.2
 Summary: A collection of tools for data science used at DFDS.
 Author: Data Science Chapter at DFDS
 Author-email: urcha@dfds.com
 License: UNKNOWN
 Keywords: dfds_ds_toolbox,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dfds_ds_toolbox-0.9.1/dfds_ds_toolbox.egg-info/SOURCES.txt` & `dfds_ds_toolbox-0.9.2/dfds_ds_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dfds_ds_toolbox-0.9.1/setup.py` & `dfds_ds_toolbox-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="dfds_ds_toolbox",
     packages=find_packages(exclude=["*tests*"]),
     keywords=["dfds_ds_toolbox", "data science"],
-    version="0.9.1",
+    version="0.9.2",
     description="A collection of tools for data science used at DFDS.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Data Science Chapter at DFDS",
     author_email="urcha@dfds.com",
     install_requires=["scikit-learn", "pandas", "numpy", "matplotlib", "statsmodels", "rich"],
     classifiers=[
```

