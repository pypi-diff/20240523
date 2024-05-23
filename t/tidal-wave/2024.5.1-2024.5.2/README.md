# Comparing `tmp/tidal_wave-2024.5.1.tar.gz` & `tmp/tidal_wave-2024.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidal_wave-2024.5.1.tar", last modified: Wed May  1 21:54:49 2024, max compression
+gzip compressed data, was "tidal_wave-2024.5.2.tar", last modified: Thu May 23 18:05:04 2024, max compression
```

## Comparing `tidal_wave-2024.5.1.tar` & `tidal_wave-2024.5.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:54:49.607175 tidal_wave-2024.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41707 2024-05-01 21:54:49.607175 tidal_wave-2024.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27550 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:54:49.607175 tidal_wave-2024.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:54:49.607175 tidal_wave-2024.5.1/tidal_wave/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/album.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/hls.py
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    20082 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/mix.py
--rw-r--r--   0 runner    (1001) docker     (127)    26637 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    23923 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    18725 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/requesting.py
--rw-r--r--   0 runner    (1001) docker     (127)    37440 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:54:49.607175 tidal_wave-2024.5.1/tidal_wave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41707 2024-05-01 21:54:49.000000 tidal_wave-2024.5.1/tidal_wave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-01 21:54:49.000000 tidal_wave-2024.5.1/tidal_wave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:54:49.000000 tidal_wave-2024.5.1/tidal_wave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 21:54:49.000000 tidal_wave-2024.5.1/tidal_wave.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 21:54:49.000000 tidal_wave-2024.5.1/tidal_wave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 21:54:49.000000 tidal_wave-2024.5.1/tidal_wave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-23 18:05:04.373895 tidal_wave-2024.5.2/
+-rw-r--r--   0 runner    (1001) docker     (118)    11357 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (118)    41758 2024-05-23 18:05:04.372894 tidal_wave-2024.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (118)    27550 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (118)     1393 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (118)       38 2024-05-23 18:05:04.373895 tidal_wave-2024.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (118)       93 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-23 18:05:04.370895 tidal_wave-2024.5.2/tidal_wave/
+-rw-r--r--   0 runner    (1001) docker     (118)       52 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)       29 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9900 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/album.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6084 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/artist.py
+-rw-r--r--   0 runner    (1001) docker     (118)     7599 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/dash.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3760 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/hls.py
+-rw-r--r--   0 runner    (1001) docker     (118)    12144 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/login.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6659 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/main.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2352 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/media.py
+-rw-r--r--   0 runner    (1001) docker     (118)    20082 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/mix.py
+-rw-r--r--   0 runner    (1001) docker     (118)    26637 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/models.py
+-rw-r--r--   0 runner    (1001) docker     (118)    11863 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (118)    23923 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (118)    18725 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/requesting.py
+-rw-r--r--   0 runner    (1001) docker     (118)    37440 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/track.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5392 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/utils.py
+-rw-r--r--   0 runner    (1001) docker     (118)    14928 2024-05-23 18:04:57.000000 tidal_wave-2024.5.2/tidal_wave/video.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-23 18:05:04.372894 tidal_wave-2024.5.2/tidal_wave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (118)    41758 2024-05-23 18:05:04.000000 tidal_wave-2024.5.2/tidal_wave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (118)      597 2024-05-23 18:05:04.000000 tidal_wave-2024.5.2/tidal_wave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (118)        1 2024-05-23 18:05:04.000000 tidal_wave-2024.5.2/tidal_wave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (118)       51 2024-05-23 18:05:04.000000 tidal_wave-2024.5.2/tidal_wave.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (118)      189 2024-05-23 18:05:04.000000 tidal_wave-2024.5.2/tidal_wave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (118)       11 2024-05-23 18:05:04.000000 tidal_wave-2024.5.2/tidal_wave.egg-info/top_level.txt
```

### Comparing `tidal_wave-2024.5.1/LICENSE` & `tidal_wave-2024.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/PKG-INFO` & `tidal_wave-2024.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal-wave
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: A tool to wave at the TIDAL music service.
 Author-email: colinho <pypi@colin.technology>
 Maintainer-email: colinho <pypi@colin.technology>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -210,29 +210,30 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: backoff==2.2.1
 Requires-Dist: cachecontrol==0.14.0
 Requires-Dist: dataclass-wizard==0.22.3
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: mutagen==1.47.0
-Requires-Dist: m3u8==4.1.0
-Requires-Dist: platformdirs==4.2.1
+Requires-Dist: m3u8==5.0.0
+Requires-Dist: platformdirs==4.2.2
 Requires-Dist: pycryptodome==3.20.0
-Requires-Dist: requests[socks]==2.31.0
+Requires-Dist: requests[socks]==2.32.2
 Requires-Dist: typer==0.12.3
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Version](https://img.shields.io/pypi/v/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![Build Python package](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml/badge.svg?branch=trunk&event=release)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml)
 [![Docker Image CI](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml)
@@ -314,24 +315,24 @@
 $ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave.git
 $ cd tidal-wave
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ (.venv) pip install .
 ```
 ### PyInstaller executable
-The release artifacts for this project are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it. **Please make sure that the SHA256 checksum of the file that you have downloaded matches the corresponding `.sha256` file on the releases page!**
+The release artifacts for this project are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.3, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it. **Please make sure that the SHA256 checksum of the file that you have downloaded matches the corresponding `.sha256` file on the releases page!**
 #### On Unix-Like
 ```bash
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64.sha256
-$ sha256sum --check tidal-wave_ubuntu_22.04_amd64.sha256
-# ONLY CONTINUE IF THE OUTPUT IS THE FOLLOWING: 'tidal-wave_ubuntu_22.04_amd64.sha256: OK'
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_24.04_amd64
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_24.04_amd64.sha256
+$ sha256sum --check tidal-wave_ubuntu_24.04_amd64.sha256
+# ONLY CONTINUE IF THE OUTPUT IS THE FOLLOWING: 'tidal-wave_ubuntu_24.04_amd64.sha256: OK'
 # Otherwise, delete the downloaded binary and try to download it again
-$ chmod +x ./tidal-wave_ubuntu_22.04_amd64
-$ ./tidal-wave_ubuntu_22.04_amd64 --help
+$ chmod +x ./tidal-wave_ubuntu_24.04_amd64
+$ ./tidal-wave_ubuntu_24.04_amd64 --help
 ```
 #### On Windows
 ```powershell
 # For just the lifetime of this PowerShell process, don't block the download from GitHub
 PS > Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
 PS > Invoke-WebRequest "https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe" -OutFile "tidal-wave_windows.exe"
 PS > Invoke-WebRequest "https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe.sha256" -OutFile "tidal-wave_windows.exe.sha256"
```

### Comparing `tidal_wave-2024.5.1/README.md` & `tidal_wave-2024.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -81,24 +81,24 @@
 $ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave.git
 $ cd tidal-wave
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ (.venv) pip install .
 ```
 ### PyInstaller executable
-The release artifacts for this project are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it. **Please make sure that the SHA256 checksum of the file that you have downloaded matches the corresponding `.sha256` file on the releases page!**
+The release artifacts for this project are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.3, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it. **Please make sure that the SHA256 checksum of the file that you have downloaded matches the corresponding `.sha256` file on the releases page!**
 #### On Unix-Like
 ```bash
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64.sha256
-$ sha256sum --check tidal-wave_ubuntu_22.04_amd64.sha256
-# ONLY CONTINUE IF THE OUTPUT IS THE FOLLOWING: 'tidal-wave_ubuntu_22.04_amd64.sha256: OK'
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_24.04_amd64
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_24.04_amd64.sha256
+$ sha256sum --check tidal-wave_ubuntu_24.04_amd64.sha256
+# ONLY CONTINUE IF THE OUTPUT IS THE FOLLOWING: 'tidal-wave_ubuntu_24.04_amd64.sha256: OK'
 # Otherwise, delete the downloaded binary and try to download it again
-$ chmod +x ./tidal-wave_ubuntu_22.04_amd64
-$ ./tidal-wave_ubuntu_22.04_amd64 --help
+$ chmod +x ./tidal-wave_ubuntu_24.04_amd64
+$ ./tidal-wave_ubuntu_24.04_amd64 --help
 ```
 #### On Windows
 ```powershell
 # For just the lifetime of this PowerShell process, don't block the download from GitHub
 PS > Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
 PS > Invoke-WebRequest "https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe" -OutFile "tidal-wave_windows.exe"
 PS > Invoke-WebRequest "https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe.sha256" -OutFile "tidal-wave_windows.exe.sha256"
```

### Comparing `tidal_wave-2024.5.1/pyproject.toml` & `tidal_wave-2024.5.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 [bdist_wheel]
 universal = 0  # Make the generated wheels have "py3" tag
 [project]
 name = "tidal-wave"
-version = "2024.5.1"
+version = "2024.5.2"
 description = "A tool to wave at the TIDAL music service."
 authors = [
     {name = "colinho", email = "pypi@colin.technology"}
 ]
 maintainers = [
     {name = "colinho", email = "pypi@colin.technology"}
 ]
@@ -19,27 +19,28 @@
     "Intended Audience :: End Users/Desktop",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Operating System :: OS Independent",
     "Topic :: Multimedia :: Sound/Audio",
     "Topic :: Multimedia :: Video",
 ]
 dependencies = [
     "backoff==2.2.1",
     "cachecontrol==0.14.0",
     "dataclass-wizard==0.22.3",
     "ffmpeg-python==0.2.0",
     "mutagen==1.47.0",
-    "m3u8==4.1.0",
-    "platformdirs==4.2.1",
+    "m3u8==5.0.0",
+    "platformdirs==4.2.2",
     "pycryptodome==3.20.0",
-    "requests[socks]==2.31.0",
+    "requests[socks]==2.32.2",
     "typer==0.12.3"
 ]
 [project.scripts]
 tidal-wave = "tidal_wave.main:app"
 [project.urls]
 Homepage = "https://github.com/ebb-earl-co/tidal-wave"
```

### Comparing `tidal_wave-2024.5.1/tidal_wave/album.py` & `tidal_wave-2024.5.2/tidal_wave/album.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/artist.py` & `tidal_wave-2024.5.2/tidal_wave/artist.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/dash.py` & `tidal_wave-2024.5.2/tidal_wave/dash.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/hls.py` & `tidal_wave-2024.5.2/tidal_wave/hls.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/login.py` & `tidal_wave-2024.5.2/tidal_wave/login.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/main.py` & `tidal_wave-2024.5.2/tidal_wave/main.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/media.py` & `tidal_wave-2024.5.2/tidal_wave/media.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/mix.py` & `tidal_wave-2024.5.2/tidal_wave/mix.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/models.py` & `tidal_wave-2024.5.2/tidal_wave/models.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/oauth.py` & `tidal_wave-2024.5.2/tidal_wave/oauth.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/playlist.py` & `tidal_wave-2024.5.2/tidal_wave/playlist.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/requesting.py` & `tidal_wave-2024.5.2/tidal_wave/requesting.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/track.py` & `tidal_wave-2024.5.2/tidal_wave/track.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/utils.py` & `tidal_wave-2024.5.2/tidal_wave/utils.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave/video.py` & `tidal_wave-2024.5.2/tidal_wave/video.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.5.1/tidal_wave.egg-info/PKG-INFO` & `tidal_wave-2024.5.2/tidal_wave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal-wave
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: A tool to wave at the TIDAL music service.
 Author-email: colinho <pypi@colin.technology>
 Maintainer-email: colinho <pypi@colin.technology>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -210,29 +210,30 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: backoff==2.2.1
 Requires-Dist: cachecontrol==0.14.0
 Requires-Dist: dataclass-wizard==0.22.3
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: mutagen==1.47.0
-Requires-Dist: m3u8==4.1.0
-Requires-Dist: platformdirs==4.2.1
+Requires-Dist: m3u8==5.0.0
+Requires-Dist: platformdirs==4.2.2
 Requires-Dist: pycryptodome==3.20.0
-Requires-Dist: requests[socks]==2.31.0
+Requires-Dist: requests[socks]==2.32.2
 Requires-Dist: typer==0.12.3
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Version](https://img.shields.io/pypi/v/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![Build Python package](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml/badge.svg?branch=trunk&event=release)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml)
 [![Docker Image CI](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml)
@@ -314,24 +315,24 @@
 $ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave.git
 $ cd tidal-wave
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ (.venv) pip install .
 ```
 ### PyInstaller executable
-The release artifacts for this project are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it. **Please make sure that the SHA256 checksum of the file that you have downloaded matches the corresponding `.sha256` file on the releases page!**
+The release artifacts for this project are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.3, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it. **Please make sure that the SHA256 checksum of the file that you have downloaded matches the corresponding `.sha256` file on the releases page!**
 #### On Unix-Like
 ```bash
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64
-$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64.sha256
-$ sha256sum --check tidal-wave_ubuntu_22.04_amd64.sha256
-# ONLY CONTINUE IF THE OUTPUT IS THE FOLLOWING: 'tidal-wave_ubuntu_22.04_amd64.sha256: OK'
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_24.04_amd64
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_24.04_amd64.sha256
+$ sha256sum --check tidal-wave_ubuntu_24.04_amd64.sha256
+# ONLY CONTINUE IF THE OUTPUT IS THE FOLLOWING: 'tidal-wave_ubuntu_24.04_amd64.sha256: OK'
 # Otherwise, delete the downloaded binary and try to download it again
-$ chmod +x ./tidal-wave_ubuntu_22.04_amd64
-$ ./tidal-wave_ubuntu_22.04_amd64 --help
+$ chmod +x ./tidal-wave_ubuntu_24.04_amd64
+$ ./tidal-wave_ubuntu_24.04_amd64 --help
 ```
 #### On Windows
 ```powershell
 # For just the lifetime of this PowerShell process, don't block the download from GitHub
 PS > Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
 PS > Invoke-WebRequest "https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe" -OutFile "tidal-wave_windows.exe"
 PS > Invoke-WebRequest "https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe.sha256" -OutFile "tidal-wave_windows.exe.sha256"
```

### Comparing `tidal_wave-2024.5.1/tidal_wave.egg-info/SOURCES.txt` & `tidal_wave-2024.5.2/tidal_wave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

