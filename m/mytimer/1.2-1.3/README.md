# Comparing `tmp/mytimer-1.2.tar.gz` & `tmp/mytimer-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mytimer-1.2.tar", last modified: Mon Feb  5 15:48:58 2024, max compression
+gzip compressed data, was "mytimer-1.3.tar", last modified: Thu May 23 16:45:00 2024, max compression
```

## Comparing `mytimer-1.2.tar` & `mytimer-1.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:48:58.760978 mytimer-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-05 15:48:46.000000 mytimer-1.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-02-05 15:48:46.000000 mytimer-1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11907 2024-02-05 15:48:46.000000 mytimer-1.2/FACES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-05 15:48:46.000000 mytimer-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-05 15:48:46.000000 mytimer-1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-02-05 15:48:58.760978 mytimer-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-02-05 15:48:46.000000 mytimer-1.2/PROGRAMS.md
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-02-05 15:48:46.000000 mytimer-1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-02-05 15:48:46.000000 mytimer-1.2/TONES.md
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-05 15:48:46.000000 mytimer-1.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:48:58.756978 mytimer-1.2/mytimer/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:48:58.760978 mytimer-1.2/mytimer/sounds/
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/sounds/1.wav
--rw-r--r--   0 runner    (1001) docker     (127)    32940 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/sounds/10.wav
--rw-r--r--   0 runner    (1001) docker     (127)    34316 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/sounds/11.wav
--rw-r--r--   0 runner    (1001) docker     (127)   602412 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/sounds/2.wav
--rw-r--r--   0 runner    (1001) docker     (127)    41052 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/sounds/3.wav
--rw-r--r--   0 runner    (1001) docker     (127)    37410 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/sounds/4.wav
--rw-r--r--   0 runner    (1001) docker     (127)    45470 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/sounds/5.wav
--rw-r--r--   0 runner    (1001) docker     (127)    39828 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/sounds/6.wav
--rw-r--r--   0 runner    (1001) docker     (127)    42884 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/sounds/7.wav
--rw-r--r--   0 runner    (1001) docker     (127)    42876 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/sounds/8.wav
--rw-r--r--   0 runner    (1001) docker     (127)    49044 2024-02-05 15:48:46.000000 mytimer-1.2/mytimer/sounds/9.wav
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 15:48:58.760978 mytimer-1.2/mytimer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-02-05 15:48:58.000000 mytimer-1.2/mytimer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-05 15:48:58.000000 mytimer-1.2/mytimer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 15:48:58.000000 mytimer-1.2/mytimer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-05 15:48:58.000000 mytimer-1.2/mytimer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-05 15:48:58.000000 mytimer-1.2/mytimer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 15:48:58.000000 mytimer-1.2/mytimer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-05 15:48:46.000000 mytimer-1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 15:48:58.760978 mytimer-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-02-05 15:48:46.000000 mytimer-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:45:00.978965 mytimer-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-23 16:44:52.000000 mytimer-1.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-23 16:44:52.000000 mytimer-1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11907 2024-05-23 16:44:52.000000 mytimer-1.3/FACES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-23 16:44:52.000000 mytimer-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-23 16:44:52.000000 mytimer-1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-05-23 16:45:00.978965 mytimer-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-23 16:44:52.000000 mytimer-1.3/PROGRAMS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-23 16:44:52.000000 mytimer-1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 16:44:52.000000 mytimer-1.3/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-23 16:44:52.000000 mytimer-1.3/TONES.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 16:44:52.000000 mytimer-1.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:45:00.974965 mytimer-1.3/mytimer/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:45:00.978965 mytimer-1.3/mytimer/sounds/
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/sounds/1.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    32940 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/sounds/10.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    34316 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/sounds/11.wav
+-rw-r--r--   0 runner    (1001) docker     (127)   602412 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/sounds/2.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    41052 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/sounds/3.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    37410 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/sounds/4.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    45470 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/sounds/5.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    39828 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/sounds/6.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    42884 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/sounds/7.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    42876 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/sounds/8.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    49044 2024-05-23 16:44:52.000000 mytimer-1.3/mytimer/sounds/9.wav
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:45:00.978965 mytimer-1.3/mytimer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-05-23 16:45:00.000000 mytimer-1.3/mytimer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-23 16:45:00.000000 mytimer-1.3/mytimer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:45:00.000000 mytimer-1.3/mytimer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 16:45:00.000000 mytimer-1.3/mytimer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 16:45:00.000000 mytimer-1.3/mytimer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 16:45:00.000000 mytimer-1.3/mytimer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 16:44:52.000000 mytimer-1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 16:45:00.978965 mytimer-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-23 16:44:52.000000 mytimer-1.3/setup.py
```

### Comparing `mytimer-1.2/CHANGELOG.md` & `mytimer-1.3/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,36 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [1.3] - 2024-05-23
+### Added
+- 1 new program
+	1. `animedoro`
+- `two_step_timer` function
+- `print_message` function
+- `SECURITY.md`
+### Changed
+- Test system modified
+- `nava` added to `requirements.txt`
+- Sound playing system updated
+- Python 3.5 dropped
+- `short-break` program duration changed from `10 minutes` to `5 minutes`
+- `long-break` program duration changed from `30 minutes` to `15 minutes`
+- `pomodoro` program updated
+- `pomodoro_timer` function modified
+- `load_params` function modified
+- `README.md` updated
+### Removed
+- `animedoro_timer` function
+- `_112_26_timer` function
+- `_52_17_timer` function
 ## [1.2] - 2024-02-05
 ### Added
 - `feature_request.yml` template
 - `config.yml` for issue template
 - 2 new programs
 	1. `52-17`
 	2. `112-26`
@@ -106,15 +128,16 @@
 - `countup_timer` function modified
 ## [0.1] - 2022-10-18
 ### Added
 - Countdown mode
 - Count-up mode
 - Alarm
 
-[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v1.2...dev
+[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v1.3...dev
+[1.3]: https://github.com/sepandhaghighi/mytimer/compare/v1.2...v1.3
 [1.2]: https://github.com/sepandhaghighi/mytimer/compare/v1.1...v1.2
 [1.1]: https://github.com/sepandhaghighi/mytimer/compare/v1.0...v1.1
 [1.0]: https://github.com/sepandhaghighi/mytimer/compare/v0.9...v1.0
 [0.9]: https://github.com/sepandhaghighi/mytimer/compare/v0.8...v0.9
 [0.8]: https://github.com/sepandhaghighi/mytimer/compare/v0.7...v0.8
 [0.7]: https://github.com/sepandhaghighi/mytimer/compare/v0.6...v0.7
 [0.6]: https://github.com/sepandhaghighi/mytimer/compare/v0.5...v0.6
```

### Comparing `mytimer-1.2/FACES.md` & `mytimer-1.3/FACES.md`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/LICENSE` & `mytimer-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/PKG-INFO` & `mytimer-1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,50 @@
 Metadata-Version: 2.1
 Name: mytimer
-Version: 1.2
+Version: 1.3
 Summary: A Geeky Timer for Terminal Enthusiasts
 Home-page: https://github.com/sepandhaghighi/mytimer
-Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v1.2
+Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v1.3
 Author: Sepand Haghighi
-Author-email: sepand@pyrgg.ir
+Author-email: me@sepand.tech
 License: MIT
 Project-URL: Source, https://github.com/sepandhaghighi/mytimer
 Keywords: python3 python timer terminal stopwatch cli
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Utilities
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: art>=5.3
+Requires-Dist: nava>=0.4
 
 
 <div align="center">
 <img src="https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/logo.png" width="500">
 <h1>MyTimer: A Geeky Timer for Terminal Enthusiasts</h1>
 <br/>
 <a href="https://badge.fury.io/py/mytimer"><img src="https://badge.fury.io/py/mytimer.svg" alt="PyPI version" height="18"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3"></a>
-</div>	
-
-## Table of contents					
-   * [Overview](https://github.com/sepandhaghighi/mytimer#overview)
-   * [Installation](https://github.com/sepandhaghighi/mytimer#installation)
-   * [Usage](https://github.com/sepandhaghighi/mytimer#usage)
-   * [Issues & Bug Reports](https://github.com/sepandhaghighi/mytimer#issues--bug-reports)
-   * [Contribution](https://github.com/sepandhaghighi/mytimer/blob/main/.github/CONTRIBUTING.md)
-   * [References](https://github.com/sepandhaghighi/mytimer#references)
-   * [Authors](https://github.com/sepandhaghighi/mytimer/blob/main/AUTHORS.md)
-   * [License](https://github.com/sepandhaghighi/mytimer/blob/main/LICENSE)
-   * [Show Your Support](https://github.com/sepandhaghighi/mytimer#show-your-support)
-   * [Changelog](https://github.com/sepandhaghighi/mytimer/blob/main/CHANGELOG.md)
-   * [Code of Conduct](https://github.com/sepandhaghighi/mytimer/blob/main/.github/CODE_OF_CONDUCT.md)			
+</div>			
 				
 ## Overview	
 
 <p align="justify">					
 <strong>MyTimer</strong> is a Python project that aims to provide a simple yet efficient timer for terminal users, particularly targeting the geek community. This project allows users to set timers directly from their command line interface, making it convenient for those who spend a significant amount of time working in the terminal!
 
 The main objective of <strong>MyTimer</strong> is to offer a minimalistic and distraction-free timer experience. It provides a clean and straightforward interface, ensuring that users can focus solely on tracking time without any unnecessary clutter or distractions.
@@ -80,16 +67,16 @@
 	<tr> 
 		<td align="center">Branch</td>
 		<td align="center">main</td>	
 		<td align="center">dev</td>	
 	</tr>
 	<tr>
 		<td align="center">CI</td>
-		<td align="center"><img src="https://github.com/sepandhaghighi/mytimer/workflows/CI/badge.svg?branch=main"></td>
-		<td align="center"><img src="https://github.com/sepandhaghighi/mytimer/workflows/CI/badge.svg?branch=dev"></td>
+		<td align="center"><img src="https://github.com/sepandhaghighi/mytimer/actions/workflows/test.yml/badge.svg?branch=main"></td>
+		<td align="center"><img src="https://github.com/sepandhaghighi/mytimer/actions/workflows/test.yml/badge.svg?branch=dev"></td>
 	</tr>
 </table>
 
 
 <table>
 	<tr> 
 		<td align="center">Code Quality</td>
@@ -99,21 +86,21 @@
 	</tr>
 </table>
 
 
 ## Installation		
 
 ### Source Code
-- Download [Version 1.2](https://github.com/sepandhaghighi/mytimer/archive/v1.2.zip) or [Latest Source](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
+- Download [Version 1.3](https://github.com/sepandhaghighi/mytimer/archive/v1.3.zip) or [Latest Source](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
 - `pip install .`				
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- `pip install mytimer==1.2`						
+- `pip install mytimer==1.3`						
 
 
 ## Usage
 
 ⚠️ You can use `mytimer` or `python -m mytimer` to run this program
 
 ### Version
@@ -237,14 +224,16 @@
 
 <blockquote>4- <a href="https://en.wikipedia.org/wiki/Pomodoro_Technique">Pomodoro Technique</a></blockquote>
 
 <blockquote>5- <a href="https://www.themuse.com/advice/the-rule-of-52-and-17-its-random-but-it-ups-your-productivity">The Rule of 52 and 17: It's Random, But it Ups Your Productivity</a></blockquote>
 
 <blockquote>6- <a href="https://desktime.com/blog/productivity-research">Desktime’s Productivity Research: An Overview of Our Finds Throughout the Years</a></blockquote>
 
+<blockquote>7- <a href="https://ankushkun.github.io/animedoro-timer/Animedoro/">AnimeDoro Timer</a></blockquote>
+
 ## Show your support
 								
 <h3>Star this repo</h3>					
 
 Give a ⭐️ if this project helped you!
 
 <h3>Donate to our project</h3>	
@@ -280,14 +269,36 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [1.3] - 2024-05-23
+### Added
+- 1 new program
+	1. `animedoro`
+- `two_step_timer` function
+- `print_message` function
+- `SECURITY.md`
+### Changed
+- Test system modified
+- `nava` added to `requirements.txt`
+- Sound playing system updated
+- Python 3.5 dropped
+- `short-break` program duration changed from `10 minutes` to `5 minutes`
+- `long-break` program duration changed from `30 minutes` to `15 minutes`
+- `pomodoro` program updated
+- `pomodoro_timer` function modified
+- `load_params` function modified
+- `README.md` updated
+### Removed
+- `animedoro_timer` function
+- `_112_26_timer` function
+- `_52_17_timer` function
 ## [1.2] - 2024-02-05
 ### Added
 - `feature_request.yml` template
 - `config.yml` for issue template
 - 2 new programs
 	1. `52-17`
 	2. `112-26`
@@ -385,15 +396,16 @@
 - `countup_timer` function modified
 ## [0.1] - 2022-10-18
 ### Added
 - Countdown mode
 - Count-up mode
 - Alarm
 
-[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v1.2...dev
+[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v1.3...dev
+[1.3]: https://github.com/sepandhaghighi/mytimer/compare/v1.2...v1.3
 [1.2]: https://github.com/sepandhaghighi/mytimer/compare/v1.1...v1.2
 [1.1]: https://github.com/sepandhaghighi/mytimer/compare/v1.0...v1.1
 [1.0]: https://github.com/sepandhaghighi/mytimer/compare/v0.9...v1.0
 [0.9]: https://github.com/sepandhaghighi/mytimer/compare/v0.8...v0.9
 [0.8]: https://github.com/sepandhaghighi/mytimer/compare/v0.7...v0.8
 [0.7]: https://github.com/sepandhaghighi/mytimer/compare/v0.6...v0.7
 [0.6]: https://github.com/sepandhaghighi/mytimer/compare/v0.5...v0.6
```

#### html2text {}

```diff
@@ -1,66 +1,54 @@
-Metadata-Version: 2.1 Name: mytimer Version: 1.2 Summary: A Geeky Timer for
+Metadata-Version: 2.1 Name: mytimer Version: 1.3 Summary: A Geeky Timer for
 Terminal Enthusiasts Home-page: https://github.com/sepandhaghighi/mytimer
-Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v1.2 Author:
-Sepand Haghighi Author-email: sepand@pyrgg.ir License: MIT Project-URL: Source,
+Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v1.3 Author:
+Sepand Haghighi Author-email: me@sepand.tech License: MIT Project-URL: Source,
 https://github.com/sepandhaghighi/mytimer Keywords: python3 python timer
 terminal stopwatch cli Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3.5 Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Other Audience Classifier: Topic :: Games/
-Entertainment Classifier: Topic :: Utilities Requires-Python: >=3.5
-Description-Content-Type: text/markdown License-File: LICENSE License-File:
-AUTHORS.md Requires-Dist: art>=5.3
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Education Classifier: Intended
+Audience :: End Users/Desktop Classifier: Intended Audience :: Other Audience
+Classifier: Topic :: Games/Entertainment Classifier: Topic :: Utilities
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE License-File: AUTHORS.md Requires-Dist: art>=5.3 Requires-Dist:
+nava>=0.4
    [https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/logo.png]
          ************ MMyyTTiimmeerr:: AA GGeeeekkyy TTiimmeerr ffoorr TTeerrmmiinnaall EEnntthhuussiiaassttss ************
 
                       _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_b_u_i_l_t_ _w_i_t_h_ _P_y_t_h_o_n_3_]
-## Table of contents * [Overview](https://github.com/sepandhaghighi/
-mytimer#overview) * [Installation](https://github.com/sepandhaghighi/
-mytimer#installation) * [Usage](https://github.com/sepandhaghighi/
-mytimer#usage) * [Issues & Bug Reports](https://github.com/sepandhaghighi/
-mytimer#issues--bug-reports) * [Contribution](https://github.com/
-sepandhaghighi/mytimer/blob/main/.github/CONTRIBUTING.md) * [References](https:
-//github.com/sepandhaghighi/mytimer#references) * [Authors](https://github.com/
-sepandhaghighi/mytimer/blob/main/AUTHORS.md) * [License](https://github.com/
-sepandhaghighi/mytimer/blob/main/LICENSE) * [Show Your Support](https://
-github.com/sepandhaghighi/mytimer#show-your-support) * [Changelog](https://
-github.com/sepandhaghighi/mytimer/blob/main/CHANGELOG.md) * [Code of Conduct]
-(https://github.com/sepandhaghighi/mytimer/blob/main/.github/
-CODE_OF_CONDUCT.md) ## Overview
+## Overview
 MMyyTTiimmeerr is a Python project that aims to provide a simple yet efficient timer
 for terminal users, particularly targeting the geek community. This project
 allows users to set timers directly from their command line interface, making
 it convenient for those who spend a significant amount of time working in the
 terminal! The main objective of MMyyTTiimmeerr is to offer a minimalistic and
 distraction-free timer experience. It provides a clean and straightforward
 interface, ensuring that users can focus solely on tracking time without any
 unnecessary clutter or distractions.
 PyPI Counter                _[_h_t_t_p_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_m_y_t_i_m_e_r_]
 Github Stars _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_s_e_p_a_n_d_h_a_g_h_i_g_h_i_/
                     _m_y_t_i_m_e_r_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_a_b_e_l_=_S_t_a_r_s_]
 Branch                        main                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
-   CI         mytimer/workflows/CI/               mytimer/workflows/CI/
+   CI  mytimer/actions/workflows/test.yml/ mytimer/actions/workflows/test.yml/
              badge.svg?branch=main]               badge.svg?branch=dev]
                           _[_h_t_t_p_s_:_/_/_a_p_p_._c_o_d_a_c_y_._c_o_m_/_p_r_o_j_e_c_t_/
 Code Quality _[_C_o_d_e_F_a_c_t_o_r_]           _b_a_d_g_e_/_G_r_a_d_e_/            _[_c_o_d_e_b_e_a_t_ _b_a_d_g_e_]
                           _1_b_f_2_8_5_0_0_4_3_1_a_4_9_8_9_9_8_a_c_7_9_8_9_1_c_d_7_9_c_d_a_]
-## Installation ### Source Code - Download [Version 1.2](https://github.com/
-sepandhaghighi/mytimer/archive/v1.2.zip) or [Latest Source](https://github.com/
+## Installation ### Source Code - Download [Version 1.3](https://github.com/
+sepandhaghighi/mytimer/archive/v1.3.zip) or [Latest Source](https://github.com/
 sepandhaghighi/mytimer/archive/dev.zip) - `pip install .` ### PyPI - Check
 [Python Packaging User Guide](https://packaging.python.org/installing/) - `pip
-install mytimer==1.2` ## Usage â ï¸ You can use `mytimer` or `python -
+install mytimer==1.3` ## Usage â ï¸ You can use `mytimer` or `python -
 m mytimer` to run this program ### Version ```console mytimer --version ``` ###
 Basic â ï¸ Press `Ctrl + C` to exit ```console mytimer ``` ### Time Limit
 ```console mytimer --minute=7 --second=30 ``` ```console mytimer --hour=2 --
 minute=20 ``` ### Timer Mode â ï¸ The default mode is `count-up` ```console
 mytimer --minute=7 --second=30 --countdown ``` ```console mytimer --minute=7 --
 second=30 --countup ``` ### Alarm â ï¸ This mode may not be supported on all
 systems ```console mytimer --minute=7 --second=30 --alarm ``` ### Alarm Repeat
@@ -83,14 +71,15 @@
      1- _M_i_x_k_i_t_ _F_r_e_e_ _A_l_a_r_m_ _S_o_u_n_d_ _E_f_f_e_c_t_s
      2- _O_n_l_i_n_e_ _T_i_m_e_r
      3- _M_e_d_i_a_ _C_o_l_l_e_g_e
      4- _P_o_m_o_d_o_r_o_ _T_e_c_h_n_i_q_u_e
      5- _T_h_e_ _R_u_l_e_ _o_f_ _5_2_ _a_n_d_ _1_7_:_ _I_t_'_s_ _R_a_n_d_o_m_,_ _B_u_t_ _i_t_ _U_p_s_ _Y_o_u_r_ _P_r_o_d_u_c_t_i_v_i_t_y
      6- _D_e_s_k_t_i_m_e_â___s_ _P_r_o_d_u_c_t_i_v_i_t_y_ _R_e_s_e_a_r_c_h_:_ _A_n_ _O_v_e_r_v_i_e_w_ _o_f_ _O_u_r_ _F_i_n_d_s
      _T_h_r_o_u_g_h_o_u_t_ _t_h_e_ _Y_e_a_r_s
+     7- _A_n_i_m_e_D_o_r_o_ _T_i_m_e_r
 ## Show your support
 ******** SSttaarr tthhiiss rreeppoo ********
 Give a â­ï¸ if this project helped you!
 ******** DDoonnaattee ttoo oouurr pprroojjeecctt ********
 ****** BBiittccooiinn ******
 1KtNLEEeUbTEK9PdN6Ya3ZAKXaqoKUuxCy
 ****** EEtthheerreeuumm ******
@@ -114,45 +103,54 @@
 ****** ZZiilllliiqqaa ******
 zil1knmz8zj88cf0exr2ry7nav9elehxfcgqu3c5e5
 ****** CCooffffeeeettee ******
 _[_h_t_t_p_:_/_/_w_w_w_._c_o_f_f_e_e_t_e_._i_r_/_i_m_a_g_e_s_/_b_u_t_t_o_n_s_/_l_e_m_o_n_c_h_i_f_f_o_n_._p_n_g_]# Changelog All notable
 changes to this project will be documented in this file. The format is based on
 [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this project
 adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html). ##
-[Unreleased] ## [1.2] - 2024-02-05 ### Added - `feature_request.yml` template -
-`config.yml` for issue template - 2 new programs 1. `52-17` 2. `112-26` ###
-Changed - Bug report template modified - `run_timer` function modified ## [1.1]
-- 2023-12-20 ### Added - 1 new program 1. `pomodoro` ### Changed -
-`TIME_PRINT_TEMPLATE` changed - `KeyboardInterrupt` exit handling updated -
-`ADDITIONAL_INFO` added to argparser epilog - `Python 3.12` added to `test.yml`
-## [1.0] - 2023-11-08 ### Added - `--programs-list` argument - `--faces-list`
-argument - `--v-shift` argument - `--h-shift` argument - `DEFAULT_PARAMS`
-parameter - `PROGRAMS_DEFAULTS` parameter - `load_program_params` function ###
-Changed - `japanese-green-tea` program bug fixed - `README.md` updated ## [0.9]
-- 2023-10-04 ### Added - 4 new faces - 4 new programs 1. `work` 2. `short-
-break` 3. `long-break` 4. `noodle` ### Changed - `PROGRAMS.md` updated ## [0.8]
-- 2023-08-07 ### Added - Logo - `--alarm-repeat` argument ### Changed - Tones
-length modified - `README.md` updated ## [0.7] - 2023-07-23 ### Added - `--
-tone` argument - `TONES.md` - 9 new tones ### Changed - Test system modified -
-`input_check` decorator renamed to `input_handler` - `countup_timer` function
-inputs modified - `countdown_timer` function inputs modified - `PROGRAMS.md`
-updated - `FACES.md` updated ## [0.6] - 2023-07-04 ### Added - `--program`
-argument - `PROGRAMS.md` - `run_timer` function ### Changed - Inputs type
-changed to `int` - `README.md` updated - `WRONG_INPUT_ERROR` renamed to
-`INPUT_ERROR_MESSAGE` - Alarm tone changed ## [0.5] - 2023-05-25 ### Added - 5
-new faces - `--message` argument ### Changed - `play_sound` function modified -
-`playsound` removed from `requirements.txt` - `README.md` updated ## [0.4] -
-2023-02-10 ### Added - 4 new faces - Infinite timer mode ### Changed -
-`README.md` updated - Parameters moved to `params.py` ## [0.3] - 2022-11-25 ###
-Added - `--face` argument - `FACES.md` ### Changed - `README.md` updated -
-Minimum `art` library version changed from `1.8` to `2.9` ## [0.2] - 2022-11-03
-### Added - `--version` flag ### Changed - Test system modified -
-`countdown_timer` function modified - `countup_timer` function modified ##
-[0.1] - 2022-10-18 ### Added - Countdown mode - Count-up mode - Alarm
-[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v1.2...dev
+[Unreleased] ## [1.3] - 2024-05-23 ### Added - 1 new program 1. `animedoro` -
+`two_step_timer` function - `print_message` function - `SECURITY.md` ###
+Changed - Test system modified - `nava` added to `requirements.txt` - Sound
+playing system updated - Python 3.5 dropped - `short-break` program duration
+changed from `10 minutes` to `5 minutes` - `long-break` program duration
+changed from `30 minutes` to `15 minutes` - `pomodoro` program updated -
+`pomodoro_timer` function modified - `load_params` function modified -
+`README.md` updated ### Removed - `animedoro_timer` function - `_112_26_timer`
+function - `_52_17_timer` function ## [1.2] - 2024-02-05 ### Added -
+`feature_request.yml` template - `config.yml` for issue template - 2 new
+programs 1. `52-17` 2. `112-26` ### Changed - Bug report template modified -
+`run_timer` function modified ## [1.1] - 2023-12-20 ### Added - 1 new program
+1. `pomodoro` ### Changed - `TIME_PRINT_TEMPLATE` changed - `KeyboardInterrupt`
+exit handling updated - `ADDITIONAL_INFO` added to argparser epilog - `Python
+3.12` added to `test.yml` ## [1.0] - 2023-11-08 ### Added - `--programs-list`
+argument - `--faces-list` argument - `--v-shift` argument - `--h-shift`
+argument - `DEFAULT_PARAMS` parameter - `PROGRAMS_DEFAULTS` parameter -
+`load_program_params` function ### Changed - `japanese-green-tea` program bug
+fixed - `README.md` updated ## [0.9] - 2023-10-04 ### Added - 4 new faces - 4
+new programs 1. `work` 2. `short-break` 3. `long-break` 4. `noodle` ### Changed
+- `PROGRAMS.md` updated ## [0.8] - 2023-08-07 ### Added - Logo - `--alarm-
+repeat` argument ### Changed - Tones length modified - `README.md` updated ##
+[0.7] - 2023-07-23 ### Added - `--tone` argument - `TONES.md` - 9 new tones ###
+Changed - Test system modified - `input_check` decorator renamed to
+`input_handler` - `countup_timer` function inputs modified - `countdown_timer`
+function inputs modified - `PROGRAMS.md` updated - `FACES.md` updated ## [0.6]
+- 2023-07-04 ### Added - `--program` argument - `PROGRAMS.md` - `run_timer`
+function ### Changed - Inputs type changed to `int` - `README.md` updated -
+`WRONG_INPUT_ERROR` renamed to `INPUT_ERROR_MESSAGE` - Alarm tone changed ##
+[0.5] - 2023-05-25 ### Added - 5 new faces - `--message` argument ### Changed -
+`play_sound` function modified - `playsound` removed from `requirements.txt` -
+`README.md` updated ## [0.4] - 2023-02-10 ### Added - 4 new faces - Infinite
+timer mode ### Changed - `README.md` updated - Parameters moved to `params.py`
+## [0.3] - 2022-11-25 ### Added - `--face` argument - `FACES.md` ### Changed -
+`README.md` updated - Minimum `art` library version changed from `1.8` to `2.9`
+## [0.2] - 2022-11-03 ### Added - `--version` flag ### Changed - Test system
+modified - `countdown_timer` function modified - `countup_timer` function
+modified ## [0.1] - 2022-10-18 ### Added - Countdown mode - Count-up mode -
+Alarm [Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/
+v1.3...dev [1.3]: https://github.com/sepandhaghighi/mytimer/compare/v1.2...v1.3
 [1.2]: https://github.com/sepandhaghighi/mytimer/compare/v1.1...v1.2 [1.1]:
 https://github.com/sepandhaghighi/mytimer/compare/v1.0...v1.1 [1.0]: https://
 github.com/sepandhaghighi/mytimer/compare/v0.9...v1.0 [0.9]: https://
 github.com/sepandhaghighi/mytimer/compare/v0.8...v0.9 [0.8]: https://
 github.com/sepandhaghighi/mytimer/compare/v0.7...v0.8 [0.7]: https://
 github.com/sepandhaghighi/mytimer/compare/v0.6...v0.7 [0.6]: https://
 github.com/sepandhaghighi/mytimer/compare/v0.5...v0.6 [0.5]: https://
```

### Comparing `mytimer-1.2/PROGRAMS.md` & `mytimer-1.3/PROGRAMS.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,43 +92,49 @@
 		<td><code>work</code></td>
 		<td>00:25:00</td>
 		<td>>=0.9</td>
 	</tr>
 	<tr align="center">
 		<td>Short break</td>
 		<td><code>short-break</code></td>
-		<td>00:10:00</td>
+		<td>00:05:00</td>
 		<td>>=0.9</td>
 	</tr>
 	<tr align="center">
 		<td>Long break</td>
 		<td><code>long-break</code></td>
-		<td>00:30:00</td>
+		<td>00:15:00</td>
 		<td>>=0.9</td>
 	</tr>
 	<tr align="center">
 		<td>Instant noodle</td>
 		<td><code>noodle</code></td>
 		<td>00:03:00</td>
 		<td>>=0.9</td>
 	</tr>
 	<tr align="center">
 		<td>Pomodoro</td>
 		<td><code>pomodoro</code></td>
-		<td>02:40:00</td>
+		<td>02:10:00</td>
 		<td>>=1.1</td>
 	</tr>
 	<tr align="center">
 		<td>52/17</td>
 		<td><code>52-17</code></td>
 		<td>01:09:00</td>
 		<td>>=1.2</td>
 	</tr>
 	<tr align="center">
 		<td>112/26</td>
 		<td><code>112-26</code></td>
 		<td>02:18:00</td>
 		<td>>=1.2</td>
 	</tr>
+	<tr align="center">
+		<td>AnimeDoro</td>
+		<td><code>animedoro</code></td>
+		<td>01:00:00</td>
+		<td>>=1.3</td>
+	</tr>
 </table>
```

#### html2text {}

```diff
@@ -10,13 +10,14 @@
         Tea bag            tea-bag    00:02:00  >=0.6
 Chinese green tea  chinese-green-tea  00:05:00  >=0.6
       Black tea          black-tea    00:05:00  >=0.6
       Oolong tea         oolong-tea   00:05:00  >=0.6
       Fruit tea          fruit-tea    00:08:00  >=0.6
       White tea          white-tea    00:10:00  >=0.6
           Work               work     00:25:00  >=0.9
-     Short break        short-break   00:10:00  >=0.9
-      Long break         long-break   00:30:00  >=0.9
+     Short break        short-break   00:05:00  >=0.9
+      Long break         long-break   00:15:00  >=0.9
    Instant noodle           noodle    00:03:00  >=0.9
-       Pomodoro           pomodoro    02:40:00  >=1.1
+       Pomodoro           pomodoro    02:10:00  >=1.1
          52/17              52-17     01:09:00  >=1.2
          112/26             112-26    02:18:00  >=1.2
+      AnimeDoro          animedoro    01:00:00  >=1.3
```

### Comparing `mytimer-1.2/README.md` & `mytimer-1.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,14 @@
 <div align="center">
 <img src="https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/logo.png" width="500">
 <h1>MyTimer: A Geeky Timer for Terminal Enthusiasts</h1>
 <br/>
 <a href="https://badge.fury.io/py/mytimer"><img src="https://badge.fury.io/py/mytimer.svg" alt="PyPI version" height="18"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3"></a>
-</div>	
-
-## Table of contents					
-   * [Overview](https://github.com/sepandhaghighi/mytimer#overview)
-   * [Installation](https://github.com/sepandhaghighi/mytimer#installation)
-   * [Usage](https://github.com/sepandhaghighi/mytimer#usage)
-   * [Issues & Bug Reports](https://github.com/sepandhaghighi/mytimer#issues--bug-reports)
-   * [Contribution](https://github.com/sepandhaghighi/mytimer/blob/main/.github/CONTRIBUTING.md)
-   * [References](https://github.com/sepandhaghighi/mytimer#references)
-   * [Authors](https://github.com/sepandhaghighi/mytimer/blob/main/AUTHORS.md)
-   * [License](https://github.com/sepandhaghighi/mytimer/blob/main/LICENSE)
-   * [Show Your Support](https://github.com/sepandhaghighi/mytimer#show-your-support)
-   * [Changelog](https://github.com/sepandhaghighi/mytimer/blob/main/CHANGELOG.md)
-   * [Code of Conduct](https://github.com/sepandhaghighi/mytimer/blob/main/.github/CODE_OF_CONDUCT.md)			
+</div>			
 				
 ## Overview	
 
 <p align="justify">					
 <strong>MyTimer</strong> is a Python project that aims to provide a simple yet efficient timer for terminal users, particularly targeting the geek community. This project allows users to set timers directly from their command line interface, making it convenient for those who spend a significant amount of time working in the terminal!
 
 The main objective of <strong>MyTimer</strong> is to offer a minimalistic and distraction-free timer experience. It provides a clean and straightforward interface, ensuring that users can focus solely on tracking time without any unnecessary clutter or distractions.
@@ -44,16 +31,16 @@
 	<tr> 
 		<td align="center">Branch</td>
 		<td align="center">main</td>	
 		<td align="center">dev</td>	
 	</tr>
 	<tr>
 		<td align="center">CI</td>
-		<td align="center"><img src="https://github.com/sepandhaghighi/mytimer/workflows/CI/badge.svg?branch=main"></td>
-		<td align="center"><img src="https://github.com/sepandhaghighi/mytimer/workflows/CI/badge.svg?branch=dev"></td>
+		<td align="center"><img src="https://github.com/sepandhaghighi/mytimer/actions/workflows/test.yml/badge.svg?branch=main"></td>
+		<td align="center"><img src="https://github.com/sepandhaghighi/mytimer/actions/workflows/test.yml/badge.svg?branch=dev"></td>
 	</tr>
 </table>
 
 
 <table>
 	<tr> 
 		<td align="center">Code Quality</td>
@@ -63,21 +50,21 @@
 	</tr>
 </table>
 
 
 ## Installation		
 
 ### Source Code
-- Download [Version 1.2](https://github.com/sepandhaghighi/mytimer/archive/v1.2.zip) or [Latest Source](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
+- Download [Version 1.3](https://github.com/sepandhaghighi/mytimer/archive/v1.3.zip) or [Latest Source](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
 - `pip install .`				
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- `pip install mytimer==1.2`						
+- `pip install mytimer==1.3`						
 
 
 ## Usage
 
 ⚠️ You can use `mytimer` or `python -m mytimer` to run this program
 
 ### Version
@@ -201,14 +188,16 @@
 
 <blockquote>4- <a href="https://en.wikipedia.org/wiki/Pomodoro_Technique">Pomodoro Technique</a></blockquote>
 
 <blockquote>5- <a href="https://www.themuse.com/advice/the-rule-of-52-and-17-its-random-but-it-ups-your-productivity">The Rule of 52 and 17: It's Random, But it Ups Your Productivity</a></blockquote>
 
 <blockquote>6- <a href="https://desktime.com/blog/productivity-research">Desktime’s Productivity Research: An Overview of Our Finds Throughout the Years</a></blockquote>
 
+<blockquote>7- <a href="https://ankushkun.github.io/animedoro-timer/Animedoro/">AnimeDoro Timer</a></blockquote>
+
 ## Show your support
 								
 <h3>Star this repo</h3>					
 
 Give a ⭐️ if this project helped you!
 
 <h3>Donate to our project</h3>
```

#### html2text {}

```diff
@@ -1,47 +1,35 @@
    [https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/logo.png]
          ************ MMyyTTiimmeerr:: AA GGeeeekkyy TTiimmeerr ffoorr TTeerrmmiinnaall EEnntthhuussiiaassttss ************
 
                       _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_b_u_i_l_t_ _w_i_t_h_ _P_y_t_h_o_n_3_]
-## Table of contents * [Overview](https://github.com/sepandhaghighi/
-mytimer#overview) * [Installation](https://github.com/sepandhaghighi/
-mytimer#installation) * [Usage](https://github.com/sepandhaghighi/
-mytimer#usage) * [Issues & Bug Reports](https://github.com/sepandhaghighi/
-mytimer#issues--bug-reports) * [Contribution](https://github.com/
-sepandhaghighi/mytimer/blob/main/.github/CONTRIBUTING.md) * [References](https:
-//github.com/sepandhaghighi/mytimer#references) * [Authors](https://github.com/
-sepandhaghighi/mytimer/blob/main/AUTHORS.md) * [License](https://github.com/
-sepandhaghighi/mytimer/blob/main/LICENSE) * [Show Your Support](https://
-github.com/sepandhaghighi/mytimer#show-your-support) * [Changelog](https://
-github.com/sepandhaghighi/mytimer/blob/main/CHANGELOG.md) * [Code of Conduct]
-(https://github.com/sepandhaghighi/mytimer/blob/main/.github/
-CODE_OF_CONDUCT.md) ## Overview
+## Overview
 MMyyTTiimmeerr is a Python project that aims to provide a simple yet efficient timer
 for terminal users, particularly targeting the geek community. This project
 allows users to set timers directly from their command line interface, making
 it convenient for those who spend a significant amount of time working in the
 terminal! The main objective of MMyyTTiimmeerr is to offer a minimalistic and
 distraction-free timer experience. It provides a clean and straightforward
 interface, ensuring that users can focus solely on tracking time without any
 unnecessary clutter or distractions.
 PyPI Counter                _[_h_t_t_p_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_m_y_t_i_m_e_r_]
 Github Stars _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_s_e_p_a_n_d_h_a_g_h_i_g_h_i_/
                     _m_y_t_i_m_e_r_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_a_b_e_l_=_S_t_a_r_s_]
 Branch                        main                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
-   CI         mytimer/workflows/CI/               mytimer/workflows/CI/
+   CI  mytimer/actions/workflows/test.yml/ mytimer/actions/workflows/test.yml/
              badge.svg?branch=main]               badge.svg?branch=dev]
                           _[_h_t_t_p_s_:_/_/_a_p_p_._c_o_d_a_c_y_._c_o_m_/_p_r_o_j_e_c_t_/
 Code Quality _[_C_o_d_e_F_a_c_t_o_r_]           _b_a_d_g_e_/_G_r_a_d_e_/            _[_c_o_d_e_b_e_a_t_ _b_a_d_g_e_]
                           _1_b_f_2_8_5_0_0_4_3_1_a_4_9_8_9_9_8_a_c_7_9_8_9_1_c_d_7_9_c_d_a_]
-## Installation ### Source Code - Download [Version 1.2](https://github.com/
-sepandhaghighi/mytimer/archive/v1.2.zip) or [Latest Source](https://github.com/
+## Installation ### Source Code - Download [Version 1.3](https://github.com/
+sepandhaghighi/mytimer/archive/v1.3.zip) or [Latest Source](https://github.com/
 sepandhaghighi/mytimer/archive/dev.zip) - `pip install .` ### PyPI - Check
 [Python Packaging User Guide](https://packaging.python.org/installing/) - `pip
-install mytimer==1.2` ## Usage â ï¸ You can use `mytimer` or `python -
+install mytimer==1.3` ## Usage â ï¸ You can use `mytimer` or `python -
 m mytimer` to run this program ### Version ```console mytimer --version ``` ###
 Basic â ï¸ Press `Ctrl + C` to exit ```console mytimer ``` ### Time Limit
 ```console mytimer --minute=7 --second=30 ``` ```console mytimer --hour=2 --
 minute=20 ``` ### Timer Mode â ï¸ The default mode is `count-up` ```console
 mytimer --minute=7 --second=30 --countdown ``` ```console mytimer --minute=7 --
 second=30 --countup ``` ### Alarm â ï¸ This mode may not be supported on all
 systems ```console mytimer --minute=7 --second=30 --alarm ``` ### Alarm Repeat
@@ -64,14 +52,15 @@
      1- _M_i_x_k_i_t_ _F_r_e_e_ _A_l_a_r_m_ _S_o_u_n_d_ _E_f_f_e_c_t_s
      2- _O_n_l_i_n_e_ _T_i_m_e_r
      3- _M_e_d_i_a_ _C_o_l_l_e_g_e
      4- _P_o_m_o_d_o_r_o_ _T_e_c_h_n_i_q_u_e
      5- _T_h_e_ _R_u_l_e_ _o_f_ _5_2_ _a_n_d_ _1_7_:_ _I_t_'_s_ _R_a_n_d_o_m_,_ _B_u_t_ _i_t_ _U_p_s_ _Y_o_u_r_ _P_r_o_d_u_c_t_i_v_i_t_y
      6- _D_e_s_k_t_i_m_e_â___s_ _P_r_o_d_u_c_t_i_v_i_t_y_ _R_e_s_e_a_r_c_h_:_ _A_n_ _O_v_e_r_v_i_e_w_ _o_f_ _O_u_r_ _F_i_n_d_s
      _T_h_r_o_u_g_h_o_u_t_ _t_h_e_ _Y_e_a_r_s
+     7- _A_n_i_m_e_D_o_r_o_ _T_i_m_e_r
 ## Show your support
 ******** SSttaarr tthhiiss rreeppoo ********
 Give a â­ï¸ if this project helped you!
 ******** DDoonnaattee ttoo oouurr pprroojjeecctt ********
 ****** BBiittccooiinn ******
 1KtNLEEeUbTEK9PdN6Ya3ZAKXaqoKUuxCy
 ****** EEtthheerreeuumm ******
```

### Comparing `mytimer-1.2/TONES.md` & `mytimer-1.3/TONES.md`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer/__main__.py` & `mytimer-1.3/mytimer/__main__.py`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer/functions.py` & `mytimer-1.3/mytimer/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,65 @@
 # -*- coding: utf-8 -*-
 """mytimer functions."""
 import os
 import sys
-import subprocess
 import time
+from nava import play
 from mytimer.params import INPUT_ERROR_MESSAGE, SOUND_ERROR_MESSAGE
 from mytimer.params import INPUT_EXAMPLE, TIME_ELEMENTS, MESSAGE_TEMPLATE
-from mytimer.params import FACES_MAP, PROGRAMS_MAP, TONES_MAP
+from mytimer.params import FACES_MAP, PROGRAMS_MAP, BREAKS_MAP, TONES_MAP
 from mytimer.params import MY_TIMER_VERSION, PROGRAMS_LIST_TEMPLATE
 from mytimer.params import FACES_LIST_EXAMPLE_MESSAGE, TIME_PRINT_TEMPLATE
-from mytimer.params import DEFAULT_PARAMS, PROGRAMS_DEFAULTS
+from mytimer.params import DEFAULT_PARAMS, PROGRAMS_DEFAULTS, BREAKS_DEFAULTS
 from mytimer.params import NEXT_PROGRAM_MESSAGE
 from art import tprint
 
 
-def load_program_params(program_name):
+def print_message(message, v_shift=0, h_shift=0, confirm=False):
     """
-    Load program params.
+    Print message.
+
+    :param message: message text
+    :type message: str
+    :param v_shift: vertical shift
+    :type v_shift: int
+    :param h_shift: horizontal shift
+    :type h_shift: int
+    :param confirm: confirm flag
+    :type confirm: bool
+    :return: None
+    """
+    func = print
+    if confirm:
+        func = input
+    print('\n' * v_shift, end='')
+    func(h_shift * " " + message)
+
+
+def load_program_params(program_name, is_break=False):
+    """
+    Load program/break params.
 
     :param program_name: program name
     :type program_name: str
-    :return: program params as dict
+    :param is_break: break flag
+    :type is_break: bool
+    :return: program/break params as dict
     """
     program_params = dict()
+    ref_map = PROGRAMS_MAP
+    ref_defaults = PROGRAMS_DEFAULTS
+    if is_break:
+        ref_map = BREAKS_MAP
+        ref_defaults = BREAKS_DEFAULTS
     for item in DEFAULT_PARAMS:
-        if item in PROGRAMS_MAP[program_name]:
-            program_params[item] = PROGRAMS_MAP[program_name][item]
-        elif item in PROGRAMS_DEFAULTS:
-            program_params[item] = PROGRAMS_DEFAULTS[item]
+        if item in ref_map[program_name]:
+            program_params[item] = ref_map[program_name][item]
+        elif item in ref_defaults:
+            program_params[item] = ref_defaults[item]
         else:
             program_params[item] = DEFAULT_PARAMS[item]
     return program_params
 
 
 def show_programs_list():
     """
@@ -71,25 +99,31 @@
     """
     for item in TIME_ELEMENTS:
         if getattr(args, item) is not None:
             return False
     return True
 
 
-def load_params(args):
+def load_params(args, program=None, is_break=False):
     """
     Load params.
 
     :param args: input arguments
     :type args: argparse.Namespace
+    :param program: program name
+    :type program: str
+    :param is_break: break flag
+    :type is_break: bool
     :return: params as dict
     """
     params = DEFAULT_PARAMS.copy()
-    if args.program:
-        params = load_program_params(args.program)
+    if program is not None:
+        params = load_program_params(program, is_break=is_break)
+    elif args.program:
+        params = load_program_params(args.program, is_break=is_break)
     for item in params:
         if getattr(args, item) is not None:
             if item not in TIME_ELEMENTS:
                 params[item] = getattr(args, item)
             else:
                 if not args.program:
                     params[item] = getattr(args, item)
@@ -206,32 +240,15 @@
     Play sound.
 
     :param sound_path: sound path
     :type sound_path: str
     :return: None
     """
     try:
-        sys_platform = sys.platform
-        if sys_platform == "win32":
-            import winsound
-            winsound.PlaySound(sound_path, winsound.SND_FILENAME)
-        elif sys_platform == "darwin":
-            _ = subprocess.check_call(["afplay",
-                                       sound_path],
-                                      shell=False,
-                                      stderr=subprocess.PIPE,
-                                      stdin=subprocess.PIPE,
-                                      stdout=subprocess.PIPE)
-        else:
-            _ = subprocess.check_call(["aplay",
-                                       sound_path],
-                                      shell=False,
-                                      stderr=subprocess.PIPE,
-                                      stdin=subprocess.PIPE,
-                                      stdout=subprocess.PIPE)
+        play(sound_path)
     except Exception:
         print(SOUND_ERROR_MESSAGE)
 
 
 @input_handler
 def countup_timer(
         hour,
@@ -373,74 +390,59 @@
                 for _ in range(alarm_repeat):
                     play_sound(get_sound_path(tone))
             break
         end = time.perf_counter()
         time.sleep(max(0, 1 - (end - start)))
 
 
-def pomodoro_timer(timer_func, **params):
+def pomodoro_timer(timer_func, params, long_break_params, short_break_params):
     """
     Pomodoro timer function.
 
     :param timer_func: timer function
     :type timer_func: function
-    :param params: counter parameters
+    :param params: program params
     :type params: dict
+    :param long_break_params: long break params
+    :type long_break_params: dict
+    :param short_break_params: short break params
+    :type short_break_params: dict
     :return: None
     """
-    short_break_params = load_program_params("short-break")
-    long_break_params = load_program_params("long-break")
+    h_shift = params["h_shift"]
     for index in range(4):
         work_params = params.copy()
         work_params["message"] += " {0}/{1}".format(index + 1, 4)
         timer_func(**work_params)
         if index == 3:
             break
-        _ = input(NEXT_PROGRAM_MESSAGE.format("Short break"))
+        print_message(message=NEXT_PROGRAM_MESSAGE.format("Short break"), h_shift=h_shift, confirm=True)
         timer_func(**short_break_params)
-        _ = input(NEXT_PROGRAM_MESSAGE.format(
-            "Work {0}/{1}".format(index + 2, 4)))
-    _ = input(NEXT_PROGRAM_MESSAGE.format("Long break"))
+        print_message(message=NEXT_PROGRAM_MESSAGE.format(
+            "Work {0}/{1}".format(index + 2, 4)), h_shift=h_shift, confirm=True)
+    print_message(message=NEXT_PROGRAM_MESSAGE.format("Long break"), h_shift=h_shift, confirm=True)
     timer_func(**long_break_params)
 
 
-def _52_17_timer(timer_func, **params):
+def two_step_timer(timer_func, params1, params2):
     """
-    52/17 timer function.
+    Two step timer function.
 
     :param timer_func: timer function
     :type timer_func: function
-    :param params: counter parameters
-    :type params: dict
-    :return: None
-    """
-    short_break_params = load_program_params("short-break")
-    short_break_params['minute'] = 17
-    short_break_params['message'] = "Short break (17 mins)"
-    timer_func(**params)
-    _ = input(NEXT_PROGRAM_MESSAGE.format("Short break"))
-    timer_func(**short_break_params)
-
-
-def _112_26_timer(timer_func, **params):
-    """
-    112/26 timer function.
-
-    :param timer_func: timer function
-    :type timer_func: function
-    :param params: counter parameters
-    :type params: dict
+    :param params1: program-1 params
+    :type params1: dict
+    :param params2: program-2 params
+    :type params2: dict
     :return: None
     """
-    short_break_params = load_program_params("short-break")
-    short_break_params['minute'] = 26
-    short_break_params['message'] = "Short break (26 mins)"
-    timer_func(**params)
-    _ = input(NEXT_PROGRAM_MESSAGE.format("Short break"))
-    timer_func(**short_break_params)
+    h_shift = params1["h_shift"]
+    timer_func(**params1)
+    print_message(message=NEXT_PROGRAM_MESSAGE.format("Break"), h_shift=h_shift, confirm=True)
+    timer_func(**params2)
 
 
 def run_timer(args):
     """
     Run timer.
 
     :param args: input arguments
@@ -454,14 +456,19 @@
     if args.version:
         print(MY_TIMER_VERSION)
     elif args.faces_list:
         show_faces_list()
     elif args.programs_list:
         show_programs_list()
     elif args.program == "pomodoro":
-        pomodoro_timer(timer_func, **params)
-    elif args.program == "52-17":
-        _52_17_timer(timer_func, **params)
-    elif args.program == "112-26":
-        _112_26_timer(timer_func, **params)
+        short_break_params = load_params(args, program="pomodoro-short-break", is_break=True)
+        long_break_params = load_params(args, program="pomodoro-long-break", is_break=True)
+        pomodoro_timer(
+            timer_func,
+            params=params,
+            long_break_params=long_break_params,
+            short_break_params=short_break_params)
+    elif args.program in ["52-17", "112-26", "animedoro"]:
+        break_params = load_params(args, is_break=True)
+        two_step_timer(timer_func, params1=params, params2=break_params)
     else:
         timer_func(**params)
```

### Comparing `mytimer-1.2/mytimer/params.py` & `mytimer-1.3/mytimer/params.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """mytimer params."""
 
-MY_TIMER_VERSION = "1.2"
+MY_TIMER_VERSION = "1.3"
 ADDITIONAL_INFO = "Additional information: Press `Ctrl+C` to exit."
 INPUT_ERROR_MESSAGE = "[Error] Wrong input"
 SOUND_ERROR_MESSAGE = "[Error] Unable to play sound"
 EXIT_MESSAGE = "See you. Bye!"
 NEXT_PROGRAM_MESSAGE = "Press `Enter` to continue (Next: {0})"
 PROGRAMS_LIST_TEMPLATE = "{0}. `{1}` - {2}"
 TIME_PRINT_TEMPLATE = "{0:02} : {1:02} : {2:02}"
@@ -68,14 +68,19 @@
     "h_shift": 0,
 }
 
 PROGRAMS_DEFAULTS = {
     "alarm": 1
 }
 
+BREAKS_DEFAULTS = {
+    "alarm": 1,
+    "tone": 2
+}
+
 PROGRAMS_MAP = {
     "poached-egg": {
         "hour": 0,
         "minute": 1,
         "second": 30,
         "message": "Poached egg (1.5 mins)",
     },
@@ -171,26 +176,65 @@
     },
     "112-26": {
         "hour": 1,
         "minute": 52,
         "second": 0,
         "message": "Time to work (112 mins)",
     },
+    "animedoro": {
+        "hour": 0,
+        "minute": 40,
+        "second": 0,
+        "message": "Time to work (40 mins)",
+    },
     "short-break": {
         "hour": 0,
-        "minute": 10,
+        "minute": 5,
         "second": 0,
-        "message": "Short break (10 mins)",
+        "message": "Short break (5 mins)",
     },
     "long-break": {
         "hour": 0,
-        "minute": 30,
+        "minute": 15,
         "second": 0,
-        "message": "Long break (30 mins)",
+        "message": "Long break (15 mins)",
     },
     "noodle": {
         "hour": 0,
         "minute": 3,
         "second": 0,
         "message": "Instant noodle (3 mins)",
     }
 }
+
+BREAKS_MAP = {
+    "52-17": {
+        "hour": 0,
+        "minute": 17,
+        "second": 0,
+        "message": "52-17 break (17 mins)",
+    },
+    "112-26": {
+        "hour": 0,
+        "minute": 26,
+        "second": 0,
+        "message": "112-26 break (26 mins)",
+    },
+    "animedoro": {
+        "hour": 0,
+        "minute": 20,
+        "second": 0,
+        "message": "Animedoro break (20 mins)",
+    },
+    "pomodoro-short-break": {
+        "hour": 0,
+        "minute": 5,
+        "second": 0,
+        "message": "Pomodoro short break (5 mins)",
+    },
+    "pomodoro-long-break": {
+        "hour": 0,
+        "minute": 15,
+        "second": 0,
+        "message": "Pomodoro long break (15 mins)",
+    },
+}
```

### Comparing `mytimer-1.2/mytimer/sounds/1.wav` & `mytimer-1.3/mytimer/sounds/1.wav`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer/sounds/10.wav` & `mytimer-1.3/mytimer/sounds/10.wav`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer/sounds/11.wav` & `mytimer-1.3/mytimer/sounds/11.wav`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer/sounds/2.wav` & `mytimer-1.3/mytimer/sounds/2.wav`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer/sounds/3.wav` & `mytimer-1.3/mytimer/sounds/3.wav`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer/sounds/4.wav` & `mytimer-1.3/mytimer/sounds/4.wav`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer/sounds/5.wav` & `mytimer-1.3/mytimer/sounds/5.wav`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer/sounds/6.wav` & `mytimer-1.3/mytimer/sounds/6.wav`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer/sounds/7.wav` & `mytimer-1.3/mytimer/sounds/7.wav`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer/sounds/8.wav` & `mytimer-1.3/mytimer/sounds/8.wav`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer/sounds/9.wav` & `mytimer-1.3/mytimer/sounds/9.wav`

 * *Files identical despite different names*

### Comparing `mytimer-1.2/mytimer.egg-info/PKG-INFO` & `mytimer-1.3/mytimer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,50 @@
 Metadata-Version: 2.1
 Name: mytimer
-Version: 1.2
+Version: 1.3
 Summary: A Geeky Timer for Terminal Enthusiasts
 Home-page: https://github.com/sepandhaghighi/mytimer
-Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v1.2
+Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v1.3
 Author: Sepand Haghighi
-Author-email: sepand@pyrgg.ir
+Author-email: me@sepand.tech
 License: MIT
 Project-URL: Source, https://github.com/sepandhaghighi/mytimer
 Keywords: python3 python timer terminal stopwatch cli
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Utilities
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: art>=5.3
+Requires-Dist: nava>=0.4
 
 
 <div align="center">
 <img src="https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/logo.png" width="500">
 <h1>MyTimer: A Geeky Timer for Terminal Enthusiasts</h1>
 <br/>
 <a href="https://badge.fury.io/py/mytimer"><img src="https://badge.fury.io/py/mytimer.svg" alt="PyPI version" height="18"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3"></a>
-</div>	
-
-## Table of contents					
-   * [Overview](https://github.com/sepandhaghighi/mytimer#overview)
-   * [Installation](https://github.com/sepandhaghighi/mytimer#installation)
-   * [Usage](https://github.com/sepandhaghighi/mytimer#usage)
-   * [Issues & Bug Reports](https://github.com/sepandhaghighi/mytimer#issues--bug-reports)
-   * [Contribution](https://github.com/sepandhaghighi/mytimer/blob/main/.github/CONTRIBUTING.md)
-   * [References](https://github.com/sepandhaghighi/mytimer#references)
-   * [Authors](https://github.com/sepandhaghighi/mytimer/blob/main/AUTHORS.md)
-   * [License](https://github.com/sepandhaghighi/mytimer/blob/main/LICENSE)
-   * [Show Your Support](https://github.com/sepandhaghighi/mytimer#show-your-support)
-   * [Changelog](https://github.com/sepandhaghighi/mytimer/blob/main/CHANGELOG.md)
-   * [Code of Conduct](https://github.com/sepandhaghighi/mytimer/blob/main/.github/CODE_OF_CONDUCT.md)			
+</div>			
 				
 ## Overview	
 
 <p align="justify">					
 <strong>MyTimer</strong> is a Python project that aims to provide a simple yet efficient timer for terminal users, particularly targeting the geek community. This project allows users to set timers directly from their command line interface, making it convenient for those who spend a significant amount of time working in the terminal!
 
 The main objective of <strong>MyTimer</strong> is to offer a minimalistic and distraction-free timer experience. It provides a clean and straightforward interface, ensuring that users can focus solely on tracking time without any unnecessary clutter or distractions.
@@ -80,16 +67,16 @@
 	<tr> 
 		<td align="center">Branch</td>
 		<td align="center">main</td>	
 		<td align="center">dev</td>	
 	</tr>
 	<tr>
 		<td align="center">CI</td>
-		<td align="center"><img src="https://github.com/sepandhaghighi/mytimer/workflows/CI/badge.svg?branch=main"></td>
-		<td align="center"><img src="https://github.com/sepandhaghighi/mytimer/workflows/CI/badge.svg?branch=dev"></td>
+		<td align="center"><img src="https://github.com/sepandhaghighi/mytimer/actions/workflows/test.yml/badge.svg?branch=main"></td>
+		<td align="center"><img src="https://github.com/sepandhaghighi/mytimer/actions/workflows/test.yml/badge.svg?branch=dev"></td>
 	</tr>
 </table>
 
 
 <table>
 	<tr> 
 		<td align="center">Code Quality</td>
@@ -99,21 +86,21 @@
 	</tr>
 </table>
 
 
 ## Installation		
 
 ### Source Code
-- Download [Version 1.2](https://github.com/sepandhaghighi/mytimer/archive/v1.2.zip) or [Latest Source](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
+- Download [Version 1.3](https://github.com/sepandhaghighi/mytimer/archive/v1.3.zip) or [Latest Source](https://github.com/sepandhaghighi/mytimer/archive/dev.zip)
 - `pip install .`				
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- `pip install mytimer==1.2`						
+- `pip install mytimer==1.3`						
 
 
 ## Usage
 
 ⚠️ You can use `mytimer` or `python -m mytimer` to run this program
 
 ### Version
@@ -237,14 +224,16 @@
 
 <blockquote>4- <a href="https://en.wikipedia.org/wiki/Pomodoro_Technique">Pomodoro Technique</a></blockquote>
 
 <blockquote>5- <a href="https://www.themuse.com/advice/the-rule-of-52-and-17-its-random-but-it-ups-your-productivity">The Rule of 52 and 17: It's Random, But it Ups Your Productivity</a></blockquote>
 
 <blockquote>6- <a href="https://desktime.com/blog/productivity-research">Desktime’s Productivity Research: An Overview of Our Finds Throughout the Years</a></blockquote>
 
+<blockquote>7- <a href="https://ankushkun.github.io/animedoro-timer/Animedoro/">AnimeDoro Timer</a></blockquote>
+
 ## Show your support
 								
 <h3>Star this repo</h3>					
 
 Give a ⭐️ if this project helped you!
 
 <h3>Donate to our project</h3>	
@@ -280,14 +269,36 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [1.3] - 2024-05-23
+### Added
+- 1 new program
+	1. `animedoro`
+- `two_step_timer` function
+- `print_message` function
+- `SECURITY.md`
+### Changed
+- Test system modified
+- `nava` added to `requirements.txt`
+- Sound playing system updated
+- Python 3.5 dropped
+- `short-break` program duration changed from `10 minutes` to `5 minutes`
+- `long-break` program duration changed from `30 minutes` to `15 minutes`
+- `pomodoro` program updated
+- `pomodoro_timer` function modified
+- `load_params` function modified
+- `README.md` updated
+### Removed
+- `animedoro_timer` function
+- `_112_26_timer` function
+- `_52_17_timer` function
 ## [1.2] - 2024-02-05
 ### Added
 - `feature_request.yml` template
 - `config.yml` for issue template
 - 2 new programs
 	1. `52-17`
 	2. `112-26`
@@ -385,15 +396,16 @@
 - `countup_timer` function modified
 ## [0.1] - 2022-10-18
 ### Added
 - Countdown mode
 - Count-up mode
 - Alarm
 
-[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v1.2...dev
+[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v1.3...dev
+[1.3]: https://github.com/sepandhaghighi/mytimer/compare/v1.2...v1.3
 [1.2]: https://github.com/sepandhaghighi/mytimer/compare/v1.1...v1.2
 [1.1]: https://github.com/sepandhaghighi/mytimer/compare/v1.0...v1.1
 [1.0]: https://github.com/sepandhaghighi/mytimer/compare/v0.9...v1.0
 [0.9]: https://github.com/sepandhaghighi/mytimer/compare/v0.8...v0.9
 [0.8]: https://github.com/sepandhaghighi/mytimer/compare/v0.7...v0.8
 [0.7]: https://github.com/sepandhaghighi/mytimer/compare/v0.6...v0.7
 [0.6]: https://github.com/sepandhaghighi/mytimer/compare/v0.5...v0.6
```

#### html2text {}

```diff
@@ -1,66 +1,54 @@
-Metadata-Version: 2.1 Name: mytimer Version: 1.2 Summary: A Geeky Timer for
+Metadata-Version: 2.1 Name: mytimer Version: 1.3 Summary: A Geeky Timer for
 Terminal Enthusiasts Home-page: https://github.com/sepandhaghighi/mytimer
-Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v1.2 Author:
-Sepand Haghighi Author-email: sepand@pyrgg.ir License: MIT Project-URL: Source,
+Download-URL: https://github.com/sepandhaghighi/mytimer/tarball/v1.3 Author:
+Sepand Haghighi Author-email: me@sepand.tech License: MIT Project-URL: Source,
 https://github.com/sepandhaghighi/mytimer Keywords: python3 python timer
 terminal stopwatch cli Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3.5 Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Other Audience Classifier: Topic :: Games/
-Entertainment Classifier: Topic :: Utilities Requires-Python: >=3.5
-Description-Content-Type: text/markdown License-File: LICENSE License-File:
-AUTHORS.md Requires-Dist: art>=5.3
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Education Classifier: Intended
+Audience :: End Users/Desktop Classifier: Intended Audience :: Other Audience
+Classifier: Topic :: Games/Entertainment Classifier: Topic :: Utilities
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE License-File: AUTHORS.md Requires-Dist: art>=5.3 Requires-Dist:
+nava>=0.4
    [https://github.com/sepandhaghighi/mytimer/raw/main/otherfiles/logo.png]
          ************ MMyyTTiimmeerr:: AA GGeeeekkyy TTiimmeerr ffoorr TTeerrmmiinnaall EEnntthhuussiiaassttss ************
 
                       _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_b_u_i_l_t_ _w_i_t_h_ _P_y_t_h_o_n_3_]
-## Table of contents * [Overview](https://github.com/sepandhaghighi/
-mytimer#overview) * [Installation](https://github.com/sepandhaghighi/
-mytimer#installation) * [Usage](https://github.com/sepandhaghighi/
-mytimer#usage) * [Issues & Bug Reports](https://github.com/sepandhaghighi/
-mytimer#issues--bug-reports) * [Contribution](https://github.com/
-sepandhaghighi/mytimer/blob/main/.github/CONTRIBUTING.md) * [References](https:
-//github.com/sepandhaghighi/mytimer#references) * [Authors](https://github.com/
-sepandhaghighi/mytimer/blob/main/AUTHORS.md) * [License](https://github.com/
-sepandhaghighi/mytimer/blob/main/LICENSE) * [Show Your Support](https://
-github.com/sepandhaghighi/mytimer#show-your-support) * [Changelog](https://
-github.com/sepandhaghighi/mytimer/blob/main/CHANGELOG.md) * [Code of Conduct]
-(https://github.com/sepandhaghighi/mytimer/blob/main/.github/
-CODE_OF_CONDUCT.md) ## Overview
+## Overview
 MMyyTTiimmeerr is a Python project that aims to provide a simple yet efficient timer
 for terminal users, particularly targeting the geek community. This project
 allows users to set timers directly from their command line interface, making
 it convenient for those who spend a significant amount of time working in the
 terminal! The main objective of MMyyTTiimmeerr is to offer a minimalistic and
 distraction-free timer experience. It provides a clean and straightforward
 interface, ensuring that users can focus solely on tracking time without any
 unnecessary clutter or distractions.
 PyPI Counter                _[_h_t_t_p_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_m_y_t_i_m_e_r_]
 Github Stars _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_s_e_p_a_n_d_h_a_g_h_i_g_h_i_/
                     _m_y_t_i_m_e_r_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_a_b_e_l_=_S_t_a_r_s_]
 Branch                        main                                 dev
        [https://github.com/sepandhaghighi/ [https://github.com/sepandhaghighi/
-   CI         mytimer/workflows/CI/               mytimer/workflows/CI/
+   CI  mytimer/actions/workflows/test.yml/ mytimer/actions/workflows/test.yml/
              badge.svg?branch=main]               badge.svg?branch=dev]
                           _[_h_t_t_p_s_:_/_/_a_p_p_._c_o_d_a_c_y_._c_o_m_/_p_r_o_j_e_c_t_/
 Code Quality _[_C_o_d_e_F_a_c_t_o_r_]           _b_a_d_g_e_/_G_r_a_d_e_/            _[_c_o_d_e_b_e_a_t_ _b_a_d_g_e_]
                           _1_b_f_2_8_5_0_0_4_3_1_a_4_9_8_9_9_8_a_c_7_9_8_9_1_c_d_7_9_c_d_a_]
-## Installation ### Source Code - Download [Version 1.2](https://github.com/
-sepandhaghighi/mytimer/archive/v1.2.zip) or [Latest Source](https://github.com/
+## Installation ### Source Code - Download [Version 1.3](https://github.com/
+sepandhaghighi/mytimer/archive/v1.3.zip) or [Latest Source](https://github.com/
 sepandhaghighi/mytimer/archive/dev.zip) - `pip install .` ### PyPI - Check
 [Python Packaging User Guide](https://packaging.python.org/installing/) - `pip
-install mytimer==1.2` ## Usage â ï¸ You can use `mytimer` or `python -
+install mytimer==1.3` ## Usage â ï¸ You can use `mytimer` or `python -
 m mytimer` to run this program ### Version ```console mytimer --version ``` ###
 Basic â ï¸ Press `Ctrl + C` to exit ```console mytimer ``` ### Time Limit
 ```console mytimer --minute=7 --second=30 ``` ```console mytimer --hour=2 --
 minute=20 ``` ### Timer Mode â ï¸ The default mode is `count-up` ```console
 mytimer --minute=7 --second=30 --countdown ``` ```console mytimer --minute=7 --
 second=30 --countup ``` ### Alarm â ï¸ This mode may not be supported on all
 systems ```console mytimer --minute=7 --second=30 --alarm ``` ### Alarm Repeat
@@ -83,14 +71,15 @@
      1- _M_i_x_k_i_t_ _F_r_e_e_ _A_l_a_r_m_ _S_o_u_n_d_ _E_f_f_e_c_t_s
      2- _O_n_l_i_n_e_ _T_i_m_e_r
      3- _M_e_d_i_a_ _C_o_l_l_e_g_e
      4- _P_o_m_o_d_o_r_o_ _T_e_c_h_n_i_q_u_e
      5- _T_h_e_ _R_u_l_e_ _o_f_ _5_2_ _a_n_d_ _1_7_:_ _I_t_'_s_ _R_a_n_d_o_m_,_ _B_u_t_ _i_t_ _U_p_s_ _Y_o_u_r_ _P_r_o_d_u_c_t_i_v_i_t_y
      6- _D_e_s_k_t_i_m_e_â___s_ _P_r_o_d_u_c_t_i_v_i_t_y_ _R_e_s_e_a_r_c_h_:_ _A_n_ _O_v_e_r_v_i_e_w_ _o_f_ _O_u_r_ _F_i_n_d_s
      _T_h_r_o_u_g_h_o_u_t_ _t_h_e_ _Y_e_a_r_s
+     7- _A_n_i_m_e_D_o_r_o_ _T_i_m_e_r
 ## Show your support
 ******** SSttaarr tthhiiss rreeppoo ********
 Give a â­ï¸ if this project helped you!
 ******** DDoonnaattee ttoo oouurr pprroojjeecctt ********
 ****** BBiittccooiinn ******
 1KtNLEEeUbTEK9PdN6Ya3ZAKXaqoKUuxCy
 ****** EEtthheerreeuumm ******
@@ -114,45 +103,54 @@
 ****** ZZiilllliiqqaa ******
 zil1knmz8zj88cf0exr2ry7nav9elehxfcgqu3c5e5
 ****** CCooffffeeeettee ******
 _[_h_t_t_p_:_/_/_w_w_w_._c_o_f_f_e_e_t_e_._i_r_/_i_m_a_g_e_s_/_b_u_t_t_o_n_s_/_l_e_m_o_n_c_h_i_f_f_o_n_._p_n_g_]# Changelog All notable
 changes to this project will be documented in this file. The format is based on
 [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this project
 adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html). ##
-[Unreleased] ## [1.2] - 2024-02-05 ### Added - `feature_request.yml` template -
-`config.yml` for issue template - 2 new programs 1. `52-17` 2. `112-26` ###
-Changed - Bug report template modified - `run_timer` function modified ## [1.1]
-- 2023-12-20 ### Added - 1 new program 1. `pomodoro` ### Changed -
-`TIME_PRINT_TEMPLATE` changed - `KeyboardInterrupt` exit handling updated -
-`ADDITIONAL_INFO` added to argparser epilog - `Python 3.12` added to `test.yml`
-## [1.0] - 2023-11-08 ### Added - `--programs-list` argument - `--faces-list`
-argument - `--v-shift` argument - `--h-shift` argument - `DEFAULT_PARAMS`
-parameter - `PROGRAMS_DEFAULTS` parameter - `load_program_params` function ###
-Changed - `japanese-green-tea` program bug fixed - `README.md` updated ## [0.9]
-- 2023-10-04 ### Added - 4 new faces - 4 new programs 1. `work` 2. `short-
-break` 3. `long-break` 4. `noodle` ### Changed - `PROGRAMS.md` updated ## [0.8]
-- 2023-08-07 ### Added - Logo - `--alarm-repeat` argument ### Changed - Tones
-length modified - `README.md` updated ## [0.7] - 2023-07-23 ### Added - `--
-tone` argument - `TONES.md` - 9 new tones ### Changed - Test system modified -
-`input_check` decorator renamed to `input_handler` - `countup_timer` function
-inputs modified - `countdown_timer` function inputs modified - `PROGRAMS.md`
-updated - `FACES.md` updated ## [0.6] - 2023-07-04 ### Added - `--program`
-argument - `PROGRAMS.md` - `run_timer` function ### Changed - Inputs type
-changed to `int` - `README.md` updated - `WRONG_INPUT_ERROR` renamed to
-`INPUT_ERROR_MESSAGE` - Alarm tone changed ## [0.5] - 2023-05-25 ### Added - 5
-new faces - `--message` argument ### Changed - `play_sound` function modified -
-`playsound` removed from `requirements.txt` - `README.md` updated ## [0.4] -
-2023-02-10 ### Added - 4 new faces - Infinite timer mode ### Changed -
-`README.md` updated - Parameters moved to `params.py` ## [0.3] - 2022-11-25 ###
-Added - `--face` argument - `FACES.md` ### Changed - `README.md` updated -
-Minimum `art` library version changed from `1.8` to `2.9` ## [0.2] - 2022-11-03
-### Added - `--version` flag ### Changed - Test system modified -
-`countdown_timer` function modified - `countup_timer` function modified ##
-[0.1] - 2022-10-18 ### Added - Countdown mode - Count-up mode - Alarm
-[Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/v1.2...dev
+[Unreleased] ## [1.3] - 2024-05-23 ### Added - 1 new program 1. `animedoro` -
+`two_step_timer` function - `print_message` function - `SECURITY.md` ###
+Changed - Test system modified - `nava` added to `requirements.txt` - Sound
+playing system updated - Python 3.5 dropped - `short-break` program duration
+changed from `10 minutes` to `5 minutes` - `long-break` program duration
+changed from `30 minutes` to `15 minutes` - `pomodoro` program updated -
+`pomodoro_timer` function modified - `load_params` function modified -
+`README.md` updated ### Removed - `animedoro_timer` function - `_112_26_timer`
+function - `_52_17_timer` function ## [1.2] - 2024-02-05 ### Added -
+`feature_request.yml` template - `config.yml` for issue template - 2 new
+programs 1. `52-17` 2. `112-26` ### Changed - Bug report template modified -
+`run_timer` function modified ## [1.1] - 2023-12-20 ### Added - 1 new program
+1. `pomodoro` ### Changed - `TIME_PRINT_TEMPLATE` changed - `KeyboardInterrupt`
+exit handling updated - `ADDITIONAL_INFO` added to argparser epilog - `Python
+3.12` added to `test.yml` ## [1.0] - 2023-11-08 ### Added - `--programs-list`
+argument - `--faces-list` argument - `--v-shift` argument - `--h-shift`
+argument - `DEFAULT_PARAMS` parameter - `PROGRAMS_DEFAULTS` parameter -
+`load_program_params` function ### Changed - `japanese-green-tea` program bug
+fixed - `README.md` updated ## [0.9] - 2023-10-04 ### Added - 4 new faces - 4
+new programs 1. `work` 2. `short-break` 3. `long-break` 4. `noodle` ### Changed
+- `PROGRAMS.md` updated ## [0.8] - 2023-08-07 ### Added - Logo - `--alarm-
+repeat` argument ### Changed - Tones length modified - `README.md` updated ##
+[0.7] - 2023-07-23 ### Added - `--tone` argument - `TONES.md` - 9 new tones ###
+Changed - Test system modified - `input_check` decorator renamed to
+`input_handler` - `countup_timer` function inputs modified - `countdown_timer`
+function inputs modified - `PROGRAMS.md` updated - `FACES.md` updated ## [0.6]
+- 2023-07-04 ### Added - `--program` argument - `PROGRAMS.md` - `run_timer`
+function ### Changed - Inputs type changed to `int` - `README.md` updated -
+`WRONG_INPUT_ERROR` renamed to `INPUT_ERROR_MESSAGE` - Alarm tone changed ##
+[0.5] - 2023-05-25 ### Added - 5 new faces - `--message` argument ### Changed -
+`play_sound` function modified - `playsound` removed from `requirements.txt` -
+`README.md` updated ## [0.4] - 2023-02-10 ### Added - 4 new faces - Infinite
+timer mode ### Changed - `README.md` updated - Parameters moved to `params.py`
+## [0.3] - 2022-11-25 ### Added - `--face` argument - `FACES.md` ### Changed -
+`README.md` updated - Minimum `art` library version changed from `1.8` to `2.9`
+## [0.2] - 2022-11-03 ### Added - `--version` flag ### Changed - Test system
+modified - `countdown_timer` function modified - `countup_timer` function
+modified ## [0.1] - 2022-10-18 ### Added - Countdown mode - Count-up mode -
+Alarm [Unreleased]: https://github.com/sepandhaghighi/mytimer/compare/
+v1.3...dev [1.3]: https://github.com/sepandhaghighi/mytimer/compare/v1.2...v1.3
 [1.2]: https://github.com/sepandhaghighi/mytimer/compare/v1.1...v1.2 [1.1]:
 https://github.com/sepandhaghighi/mytimer/compare/v1.0...v1.1 [1.0]: https://
 github.com/sepandhaghighi/mytimer/compare/v0.9...v1.0 [0.9]: https://
 github.com/sepandhaghighi/mytimer/compare/v0.8...v0.9 [0.8]: https://
 github.com/sepandhaghighi/mytimer/compare/v0.7...v0.8 [0.7]: https://
 github.com/sepandhaghighi/mytimer/compare/v0.6...v0.7 [0.6]: https://
 github.com/sepandhaghighi/mytimer/compare/v0.5...v0.6 [0.5]: https://
```

### Comparing `mytimer-1.2/mytimer.egg-info/SOURCES.txt` & `mytimer-1.3/mytimer.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 AUTHORS.md
 CHANGELOG.md
 FACES.md
 LICENSE
 MANIFEST.in
 PROGRAMS.md
 README.md
+SECURITY.md
 TONES.md
 dev-requirements.txt
 requirements.txt
 setup.py
 mytimer/__init__.py
 mytimer/__main__.py
 mytimer/functions.py
```

### Comparing `mytimer-1.2/setup.py` & `mytimer-1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,35 +25,34 @@
     except Exception:
         return '''A Geeky Timer for Terminal Enthusiasts'''
 
 
 setup(
     name='mytimer',
     packages=['mytimer'],
-    version='1.2',
+    version='1.3',
     description='A Geeky Timer for Terminal Enthusiasts',
     long_description=read_description(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     author='Sepand Haghighi',
-    author_email='sepand@pyrgg.ir',
+    author_email='me@sepand.tech',
     url='https://github.com/sepandhaghighi/mytimer',
-    download_url='https://github.com/sepandhaghighi/mytimer/tarball/v1.2',
+    download_url='https://github.com/sepandhaghighi/mytimer/tarball/v1.3',
     keywords="python3 python timer terminal stopwatch cli",
     project_urls={
         'Source': 'https://github.com/sepandhaghighi/mytimer'
     },
     install_requires=get_requires(),
-    python_requires='>=3.5',
+    python_requires='>=3.6',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Natural Language :: English',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
```

