# Comparing `tmp/icad_tone_detection-1.3.tar.gz` & `tmp/icad_tone_detection-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icad_tone_detection-1.3.tar", last modified: Wed May 15 23:39:45 2024, max compression
+gzip compressed data, was "icad_tone_detection-1.4.tar", last modified: Thu May 23 21:06:24 2024, max compression
```

## Comparing `icad_tone_detection-1.3.tar` & `icad_tone_detection-1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.563603 icad_tone_detection-1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.555603 icad_tone_detection-1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.559603 icad_tone_detection-1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-15 23:39:45.563603 icad_tone_detection-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.559603 icad_tone_detection-1.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/examples/detect_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.559603 icad_tone_detection-1.3/examples/example_audio/
--rw-r--r--   0 runner    (1001) docker     (127)   282092 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/examples/example_audio/hi_low_tone_example.wav
--rw-r--r--   0 runner    (1001) docker     (127)   799686 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/examples/example_audio/long_tone_example.wav
--rw-r--r--   0 runner    (1001) docker     (127)   805000 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/examples/example_audio/two_tone_example.wav
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 23:39:45.563603 icad_tone_detection-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.555603 icad_tone_detection-1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.563603 icad_tone_detection-1.3/src/icad_tone_detection/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/src/icad_tone_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/src/icad_tone_detection/audio_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/src/icad_tone_detection/frequency_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/src/icad_tone_detection/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/src/icad_tone_detection/tone_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.563603 icad_tone_detection-1.3/src/icad_tone_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-15 23:39:45.000000 icad_tone_detection-1.3/src/icad_tone_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-15 23:39:45.000000 icad_tone_detection-1.3/src/icad_tone_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:39:45.000000 icad_tone_detection-1.3/src/icad_tone_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 23:39:45.000000 icad_tone_detection-1.3/src/icad_tone_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 23:39:45.000000 icad_tone_detection-1.3/src/icad_tone_detection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:24.967977 icad_tone_detection-1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:24.959977 icad_tone_detection-1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:24.963977 icad_tone_detection-1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-23 21:06:24.967977 icad_tone_detection-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:24.963977 icad_tone_detection-1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/examples/detect_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:24.963977 icad_tone_detection-1.4/examples/example_audio/
+-rw-r--r--   0 runner    (1001) docker     (127)   282092 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/examples/example_audio/hi_low_tone_example.wav
+-rw-r--r--   0 runner    (1001) docker     (127)   799686 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/examples/example_audio/long_tone_example.wav
+-rw-r--r--   0 runner    (1001) docker     (127)   805000 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/examples/example_audio/two_tone_example.wav
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:06:24.967977 icad_tone_detection-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:24.959977 icad_tone_detection-1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:24.967977 icad_tone_detection-1.4/src/icad_tone_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/src/icad_tone_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/src/icad_tone_detection/audio_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/src/icad_tone_detection/frequency_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/src/icad_tone_detection/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-23 21:06:13.000000 icad_tone_detection-1.4/src/icad_tone_detection/tone_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:24.967977 icad_tone_detection-1.4/src/icad_tone_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-23 21:06:24.000000 icad_tone_detection-1.4/src/icad_tone_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-23 21:06:24.000000 icad_tone_detection-1.4/src/icad_tone_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:06:24.000000 icad_tone_detection-1.4/src/icad_tone_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 21:06:24.000000 icad_tone_detection-1.4/src/icad_tone_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 21:06:24.000000 icad_tone_detection-1.4/src/icad_tone_detection.egg-info/top_level.txt
```

### Comparing `icad_tone_detection-1.3/.github/workflows/python-package.yml` & `icad_tone_detection-1.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.3/.gitignore` & `icad_tone_detection-1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.3/LICENSE` & `icad_tone_detection-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.3/PKG-INFO` & `icad_tone_detection-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icad_tone_detection
-Version: 1.3
+Version: 1.4
 Summary: A Python library for extracting scanner radio tones from scanner audio.
 Author-email: TheGreatCodeholio <ian@icarey.net>
 Project-URL: Homepage, https://github.com/thegreatcodeholio/icad_tone_detection
 Project-URL: Issues, https://github.com/thegreatcodeholio/icad_tone_detection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `icad_tone_detection-1.3/examples/example_audio/hi_low_tone_example.wav` & `icad_tone_detection-1.4/examples/example_audio/hi_low_tone_example.wav`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.3/examples/example_audio/long_tone_example.wav` & `icad_tone_detection-1.4/examples/example_audio/long_tone_example.wav`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.3/examples/example_audio/two_tone_example.wav` & `icad_tone_detection-1.4/examples/example_audio/two_tone_example.wav`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.3/pyproject.toml` & `icad_tone_detection-1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icad_tone_detection"
-version = "1.3"
+version = "1.4"
 authors = [
   {name = "TheGreatCodeholio", email = "ian@icarey.net"},
 ]
 description = "A Python library for extracting scanner radio tones from scanner audio."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `icad_tone_detection-1.3/src/icad_tone_detection/audio_loader.py` & `icad_tone_detection-1.4/src/icad_tone_detection/audio_loader.py`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.3/src/icad_tone_detection/frequency_extraction.py` & `icad_tone_detection-1.4/src/icad_tone_detection/frequency_extraction.py`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.3/src/icad_tone_detection/tone_detection.py` & `icad_tone_detection-1.4/src/icad_tone_detection/tone_detection.py`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.3/src/icad_tone_detection.egg-info/PKG-INFO` & `icad_tone_detection-1.4/src/icad_tone_detection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icad_tone_detection
-Version: 1.3
+Version: 1.4
 Summary: A Python library for extracting scanner radio tones from scanner audio.
 Author-email: TheGreatCodeholio <ian@icarey.net>
 Project-URL: Homepage, https://github.com/thegreatcodeholio/icad_tone_detection
 Project-URL: Issues, https://github.com/thegreatcodeholio/icad_tone_detection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `icad_tone_detection-1.3/src/icad_tone_detection.egg-info/SOURCES.txt` & `icad_tone_detection-1.4/src/icad_tone_detection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

