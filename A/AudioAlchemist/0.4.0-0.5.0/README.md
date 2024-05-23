# Comparing `tmp/audioalchemist-0.4.0.tar.gz` & `tmp/audioalchemist-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioalchemist-0.4.0.tar", last modified: Wed May 22 14:11:02 2024, max compression
+gzip compressed data, was "audioalchemist-0.5.0.tar", last modified: Thu May 23 00:15:02 2024, max compression
```

## Comparing `audioalchemist-0.4.0.tar` & `audioalchemist-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 14:11:02.410075 audioalchemist-0.4.0/
-drwxrwxrwx   0        0        0        0 2024-05-22 14:11:02.394437 audioalchemist-0.4.0/AudioAlchemist/
--rw-rw-rw-   0        0        0       43 2024-05-22 12:04:05.000000 audioalchemist-0.4.0/AudioAlchemist/__int__.py
--rw-rw-rw-   0        0        0     2412 2024-05-22 14:10:21.000000 audioalchemist-0.4.0/AudioAlchemist/audio_alchemist.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:11:02.410075 audioalchemist-0.4.0/AudioAlchemist.egg-info/
--rw-rw-rw-   0        0        0     2233 2024-05-22 14:11:02.000000 audioalchemist-0.4.0/AudioAlchemist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-22 14:11:02.000000 audioalchemist-0.4.0/AudioAlchemist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 14:11:02.000000 audioalchemist-0.4.0/AudioAlchemist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-22 14:11:02.000000 audioalchemist-0.4.0/AudioAlchemist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-22 14:11:02.000000 audioalchemist-0.4.0/AudioAlchemist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2233 2024-05-22 14:11:02.410075 audioalchemist-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 14:11:02.410075 audioalchemist-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1421 2024-05-22 14:06:27.000000 audioalchemist-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:15:02.477763 audioalchemist-0.5.0/
+drwxrwxrwx   0        0        0        0 2024-05-23 00:15:02.477763 audioalchemist-0.5.0/AudioAlchemist/
+-rw-rw-rw-   0        0        0       45 2024-05-23 00:11:59.000000 audioalchemist-0.5.0/AudioAlchemist/__init__.py
+-rw-rw-rw-   0        0        0     2412 2024-05-22 14:10:21.000000 audioalchemist-0.5.0/AudioAlchemist/audio_alchemist.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:15:02.477763 audioalchemist-0.5.0/AudioAlchemist.egg-info/
+-rw-rw-rw-   0        0        0     2233 2024-05-23 00:15:02.000000 audioalchemist-0.5.0/AudioAlchemist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-23 00:15:02.000000 audioalchemist-0.5.0/AudioAlchemist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 00:15:02.000000 audioalchemist-0.5.0/AudioAlchemist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-23 00:15:02.000000 audioalchemist-0.5.0/AudioAlchemist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-23 00:15:02.000000 audioalchemist-0.5.0/AudioAlchemist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2233 2024-05-23 00:15:02.477763 audioalchemist-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-23 00:15:02.477763 audioalchemist-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1421 2024-05-23 00:14:45.000000 audioalchemist-0.5.0/setup.py
```

### Comparing `audioalchemist-0.4.0/AudioAlchemist/audio_alchemist.py` & `audioalchemist-0.5.0/AudioAlchemist/audio_alchemist.py`

 * *Files identical despite different names*

### Comparing `audioalchemist-0.4.0/AudioAlchemist.egg-info/PKG-INFO` & `audioalchemist-0.5.0/AudioAlchemist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAlchemist
-Version: 0.4.0
+Version: 0.5.0
 Summary: Convert all files directly under the directory to any music file.
 Home-page: https://github.com/Ryomo0797/AudioAlchemist.git
 Download-URL: https://github.com/Ryomo0797/AudioAlchemist.git
 Author: Kohki Suto
 Author-email: s2222019@stu.musashino-u.ac.jp
 Maintainer: Kohki Suto
 Maintainer-email: s2222019@stu.musashino-u.ac.jp
@@ -61,8 +61,8 @@
 
 ## ライセンス
 
 このプログラムは [MIT License](https://choosealicense.com/licenses/mit/) でライセンスされています。
 
 ## バージョン
 
-0.4.0
+0.5.0
```

### Comparing `audioalchemist-0.4.0/PKG-INFO` & `audioalchemist-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AudioAlchemist
-Version: 0.4.0
+Version: 0.5.0
 Summary: Convert all files directly under the directory to any music file.
 Home-page: https://github.com/Ryomo0797/AudioAlchemist.git
 Download-URL: https://github.com/Ryomo0797/AudioAlchemist.git
 Author: Kohki Suto
 Author-email: s2222019@stu.musashino-u.ac.jp
 Maintainer: Kohki Suto
 Maintainer-email: s2222019@stu.musashino-u.ac.jp
@@ -61,8 +61,8 @@
 
 ## ライセンス
 
 このプログラムは [MIT License](https://choosealicense.com/licenses/mit/) でライセンスされています。
 
 ## バージョン
 
-0.4.0
+0.5.0
```

### Comparing `audioalchemist-0.4.0/setup.py` & `audioalchemist-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DESCRIPTION = 'Convert all files directly under the directory to any music file.'
 NAME = 'AudioAlchemist'
 AUTHOR = 'Kohki Suto'
 AUTHOR_EMAIL = 's2222019@stu.musashino-u.ac.jp'
 URL = 'https://github.com/Ryomo0797/AudioAlchemist.git'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '0.4.0'
+VERSION = '0.5.0'
 PYTHON_REQUIRES = '>=3.6'
 INSTALL_REQUIRES = [
     "pandas>=2.2.2",
     "pydub>=0.25.1",
     "ffmpeg>=1.4"
     #ffmpeg-python==0.2.0
 ]
```

