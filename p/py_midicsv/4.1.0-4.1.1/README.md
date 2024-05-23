# Comparing `tmp/py_midicsv-4.1.0.tar.gz` & `tmp/py_midicsv-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_midicsv-4.1.0.tar", max compression
+gzip compressed data, was "py_midicsv-4.1.1.tar", max compression
```

## Comparing `py_midicsv-4.1.0.tar` & `py_midicsv-4.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2024-05-19 15:41:25.593467 py_midicsv-4.1.0/LICENSE
--rw-r--r--   0        0        0     3882 2024-05-19 15:41:25.593467 py_midicsv-4.1.0/README.md
--rw-r--r--   0        0        0      174 2024-05-19 15:41:25.593467 py_midicsv-4.1.0/py_midicsv/__init__.py
--rw-r--r--   0        0        0     2707 2024-05-19 15:41:25.593467 py_midicsv-4.1.0/py_midicsv/cli.py
--rw-r--r--   0        0        0     5018 2024-05-19 15:41:25.593467 py_midicsv-4.1.0/py_midicsv/csv_converters.py
--rw-r--r--   0        0        0     1357 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/csvmidi.py
--rw-r--r--   0        0        0     2480 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/events.py
--rw-r--r--   0        0        0        0 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi/__init__.py
--rw-r--r--   0        0        0     1571 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi/constants.py
--rw-r--r--   0        0        0     2550 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi/containers.py
--rw-r--r--   0        0        0    11220 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi/events.py
--rw-r--r--   0        0        0     9796 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi/fileio.py
--rw-r--r--   0        0        0      877 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi/util.py
--rw-r--r--   0        0        0     4534 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi_converters.py
--rw-r--r--   0        0        0     1019 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midicsv.py
--rw-r--r--   0        0        0     1148 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     4648 1970-01-01 00:00:00.000000 py_midicsv-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/LICENSE
+-rw-r--r--   0        0        0     3882 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/README.md
+-rw-r--r--   0        0        0      174 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/__init__.py
+-rw-r--r--   0        0        0     2707 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/cli.py
+-rw-r--r--   0        0        0     5018 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/csv_converters.py
+-rw-r--r--   0        0        0     1357 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/csvmidi.py
+-rw-r--r--   0        0        0     2480 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/events.py
+-rw-r--r--   0        0        0        0 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/midi/__init__.py
+-rw-r--r--   0        0        0     1571 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/midi/constants.py
+-rw-r--r--   0        0        0     2550 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/midi/containers.py
+-rw-r--r--   0        0        0    11235 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/midi/events.py
+-rw-r--r--   0        0        0     9796 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/midi/fileio.py
+-rw-r--r--   0        0        0      877 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/midi/util.py
+-rw-r--r--   0        0        0     4534 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/midi_converters.py
+-rw-r--r--   0        0        0     1019 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/py_midicsv/midicsv.py
+-rw-r--r--   0        0        0     1148 2024-05-23 14:54:46.081286 py_midicsv-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4648 1970-01-01 00:00:00.000000 py_midicsv-4.1.1/PKG-INFO
```

### Comparing `py_midicsv-4.1.0/LICENSE` & `py_midicsv-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.1.0/README.md` & `py_midicsv-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.1.0/py_midicsv/cli.py` & `py_midicsv-4.1.1/py_midicsv/cli.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.1.0/py_midicsv/csv_converters.py` & `py_midicsv-4.1.1/py_midicsv/csv_converters.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.1.0/py_midicsv/csvmidi.py` & `py_midicsv-4.1.1/py_midicsv/csvmidi.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.1.0/py_midicsv/events.py` & `py_midicsv-4.1.1/py_midicsv/events.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.1.0/py_midicsv/midi/constants.py` & `py_midicsv-4.1.1/py_midicsv/midi/constants.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.1.0/py_midicsv/midi/containers.py` & `py_midicsv-4.1.1/py_midicsv/midi/containers.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.1.0/py_midicsv/midi/events.py` & `py_midicsv-4.1.1/py_midicsv/midi/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,14 +338,15 @@
     metacommand = 0x20
     length = 1
 
 
 class PortEvent(MetaEvent):
     name = "MIDI Port/Cable"
     metacommand = 0x21
+    length = 1
 
 
 class TrackLoopEvent(MetaEvent):
     name = "Track Loop"
     metacommand = 0x2E
```

### Comparing `py_midicsv-4.1.0/py_midicsv/midi/fileio.py` & `py_midicsv-4.1.1/py_midicsv/midi/fileio.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.1.0/py_midicsv/midi/util.py` & `py_midicsv-4.1.1/py_midicsv/midi/util.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.1.0/py_midicsv/midi_converters.py` & `py_midicsv-4.1.1/py_midicsv/midi_converters.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.1.0/py_midicsv/midicsv.py` & `py_midicsv-4.1.1/py_midicsv/midicsv.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.1.0/pyproject.toml` & `py_midicsv-4.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py_midicsv"
-version = "4.1.0"
+version = "4.1.1"
 description = "A library for converting MIDI files from and to CSV format"
 authors = ["Tim Wedde <timwedde@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/timwedde/py_midicsv"
 homepage = "https://github.com/timwedde/py_midicsv"
```

### Comparing `py_midicsv-4.1.0/PKG-INFO` & `py_midicsv-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_midicsv
-Version: 4.1.0
+Version: 4.1.1
 Summary: A library for converting MIDI files from and to CSV format
 Home-page: https://github.com/timwedde/py_midicsv
 License: MIT
 Author: Tim Wedde
 Author-email: timwedde@icloud.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

