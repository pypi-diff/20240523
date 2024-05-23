# Comparing `tmp/Audio_SpectraCLI-3.2.tar.gz` & `tmp/Audio_SpectraCLI-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Audio_SpectraCLI-3.2.tar", last modified: Thu May 16 15:31:10 2024, max compression
+gzip compressed data, was "Audio_SpectraCLI-4.0.tar", last modified: Thu May 23 12:15:21 2024, max compression
```

## Comparing `Audio_SpectraCLI-3.2.tar` & `Audio_SpectraCLI-4.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:31:10.154417 Audio_SpectraCLI-3.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:31:10.154417 Audio_SpectraCLI-3.2/Audio_SpectraCLI/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 15:30:51.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-16 15:31:07.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:31:10.154417 Audio_SpectraCLI-3.2/Audio_SpectraCLI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-16 15:31:10.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-16 15:31:10.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:31:10.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 15:31:10.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 15:31:10.000000 Audio_SpectraCLI-3.2/Audio_SpectraCLI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-16 15:30:51.000000 Audio_SpectraCLI-3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-16 15:31:10.154417 Audio_SpectraCLI-3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-16 15:31:10.154417 Audio_SpectraCLI-3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-16 15:31:07.000000 Audio_SpectraCLI-3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:15:21.153789 Audio_SpectraCLI-4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:15:21.153789 Audio_SpectraCLI-4.0/Audio_SpectraCLI/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 12:14:56.000000 Audio_SpectraCLI-4.0/Audio_SpectraCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-23 12:15:18.000000 Audio_SpectraCLI-4.0/Audio_SpectraCLI/main-old.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-05-23 12:15:18.000000 Audio_SpectraCLI-4.0/Audio_SpectraCLI/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:15:21.153789 Audio_SpectraCLI-4.0/Audio_SpectraCLI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-23 12:15:21.000000 Audio_SpectraCLI-4.0/Audio_SpectraCLI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-23 12:15:21.000000 Audio_SpectraCLI-4.0/Audio_SpectraCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:15:21.000000 Audio_SpectraCLI-4.0/Audio_SpectraCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-23 12:15:21.000000 Audio_SpectraCLI-4.0/Audio_SpectraCLI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 12:15:21.000000 Audio_SpectraCLI-4.0/Audio_SpectraCLI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-05-23 12:14:56.000000 Audio_SpectraCLI-4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-23 12:15:21.153789 Audio_SpectraCLI-4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-23 12:15:21.153789 Audio_SpectraCLI-4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-23 12:15:18.000000 Audio_SpectraCLI-4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:15:21.153789 Audio_SpectraCLI-4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-23 12:15:18.000000 Audio_SpectraCLI-4.0/tests/test-old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-23 12:15:18.000000 Audio_SpectraCLI-4.0/tests/test.py
```

### Comparing `Audio_SpectraCLI-3.2/Audio_SpectraCLI/main.py` & `Audio_SpectraCLI-4.0/Audio_SpectraCLI/main-old.py`

 * *Files identical despite different names*

### Comparing `Audio_SpectraCLI-3.2/setup.py` & `Audio_SpectraCLI-4.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Audio_SpectraCLI",
-    version="3.2",
+    version="4.0",
     author="Aditya Seth",
     long_description=open("Readme.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "matplotlib",
         "sounddevice",
         "tabulate",
         "setuptools",
         "twine",
         "wheel",
+        "pyqt5",
         "pyaudio",
     ],
-    license="MIT",
+    license="Apache License 2.0",
     url="https://github.com/AdityaSeth777/Audio-SpectraCLI",
 )
```

