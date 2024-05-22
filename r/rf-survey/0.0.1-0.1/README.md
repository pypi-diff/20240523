# Comparing `tmp/rf_survey-0.0.1.tar.gz` & `tmp/rf_survey-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rf_survey-0.0.1.tar", last modified: Mon May  6 17:57:59 2024, max compression
+gzip compressed data, was "rf_survey-0.1.tar", last modified: Wed May 22 23:36:17 2024, max compression
```

## Comparing `rf_survey-0.0.1.tar` & `rf_survey-0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:59.041073 rf_survey-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-03-11 17:38:40.000000 rf_survey-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3528 2024-05-06 17:57:59.037045 rf_survey-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2955 2024-03-11 17:44:03.000000 rf_survey-0.0.1/README.md
--rw-rw-rw-   0        0        0      553 2024-03-11 17:38:12.000000 rf_survey-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 17:57:59.042049 rf_survey-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:58.965414 rf_survey-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:59.034049 rf_survey-0.0.1/src/rf_survey.egg-info/
--rw-rw-rw-   0        0        0     3528 2024-05-06 17:57:58.000000 rf_survey-0.0.1/src/rf_survey.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2024-05-06 17:57:58.000000 rf_survey-0.0.1/src/rf_survey.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 17:57:58.000000 rf_survey-0.0.1/src/rf_survey.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-06 17:57:58.000000 rf_survey-0.0.1/src/rf_survey.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:58.968419 rf_survey-0.0.1/src/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:59.003132 rf_survey-0.0.1/src/src/monitoring/
--rw-rw-rw-   0        0        0        0 2024-05-06 17:57:29.000000 rf_survey-0.0.1/src/src/monitoring/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:59.006141 rf_survey-0.0.1/src/src/monitoring/logins/
--rw-rw-rw-   0        0        0     2639 2024-03-08 19:15:58.000000 rf_survey-0.0.1/src/src/monitoring/logins/ip_mailer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:59.032048 rf_survey-0.0.1/src/src/rf_survey/
--rw-rw-rw-   0        0        0     1659 2024-03-08 19:15:58.000000 rf_survey-0.0.1/src/src/rf_survey/Cronify.py
--rw-rw-rw-   0        0        0      652 2024-03-08 19:15:58.000000 rf_survey-0.0.1/src/src/rf_survey/GracefulKiller.py
--rw-rw-rw-   0        0        0     2052 2024-03-08 19:15:58.000000 rf_survey-0.0.1/src/src/rf_survey/Logger.py
--rw-rw-rw-   0        0        0     3818 2024-03-08 19:15:58.000000 rf_survey-0.0.1/src/src/rf_survey/Restoration.py
--rw-rw-rw-   0        0        0        0 2024-05-06 17:57:08.000000 rf_survey-0.0.1/src/src/rf_survey/__init__.py
--rw-rw-rw-   0        0        0     3990 2024-03-08 19:15:58.000000 rf_survey-0.0.1/src/src/rf_survey/hardware.py
--rw-rw-rw-   0        0        0      970 2024-03-08 19:15:58.000000 rf_survey-0.0.1/src/src/rf_survey/kill.py
--rw-rw-rw-   0        0        0    13755 2024-03-08 19:15:58.000000 rf_survey-0.0.1/src/src/rf_survey/rf_survey.py
--rw-rw-rw-   0        0        0    13278 2024-03-11 17:25:40.000000 rf_survey-0.0.1/src/src/rf_survey/sweeps.py
--rw-rw-rw-   0        0        0     1740 2024-03-08 19:15:58.000000 rf_survey-0.0.1/src/src/rf_survey/wr_boot.py
--rw-rw-rw-   0        0        0     2785 2024-03-08 19:15:58.000000 rf_survey-0.0.1/src/src/rf_survey/wr_poll.py
+drwxrwxrwx   0        0        0        0 2024-05-22 23:36:17.549829 rf_survey-0.1/
+-rw-rw-rw-   0        0        0     1091 2024-03-11 17:38:40.000000 rf_survey-0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3526 2024-05-22 23:36:17.548829 rf_survey-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2955 2024-03-11 17:44:03.000000 rf_survey-0.1/README.md
+-rw-rw-rw-   0        0        0      551 2024-05-22 23:34:22.000000 rf_survey-0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 23:36:17.550834 rf_survey-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 23:36:17.496671 rf_survey-0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 23:36:17.545719 rf_survey-0.1/src/rf_survey.egg-info/
+-rw-rw-rw-   0        0        0     3526 2024-05-22 23:36:17.000000 rf_survey-0.1/src/rf_survey.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2024-05-22 23:36:17.000000 rf_survey-0.1/src/rf_survey.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 23:36:17.000000 rf_survey-0.1/src/rf_survey.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-22 23:36:17.000000 rf_survey-0.1/src/rf_survey.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 23:36:17.498730 rf_survey-0.1/src/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 23:36:17.519714 rf_survey-0.1/src/src/monitoring/
+-rw-rw-rw-   0        0        0        0 2024-05-06 17:57:29.000000 rf_survey-0.1/src/src/monitoring/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 23:36:17.519714 rf_survey-0.1/src/src/monitoring/logins/
+-rw-rw-rw-   0        0        0     2639 2024-03-08 19:15:58.000000 rf_survey-0.1/src/src/monitoring/logins/ip_mailer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 23:36:17.545719 rf_survey-0.1/src/src/rf_survey/
+-rw-rw-rw-   0        0        0     1659 2024-03-08 19:15:58.000000 rf_survey-0.1/src/src/rf_survey/Cronify.py
+-rw-rw-rw-   0        0        0      652 2024-03-08 19:15:58.000000 rf_survey-0.1/src/src/rf_survey/GracefulKiller.py
+-rw-rw-rw-   0        0        0     2052 2024-03-08 19:15:58.000000 rf_survey-0.1/src/src/rf_survey/Logger.py
+-rw-rw-rw-   0        0        0     3818 2024-03-08 19:15:58.000000 rf_survey-0.1/src/src/rf_survey/Restoration.py
+-rw-rw-rw-   0        0        0        0 2024-05-06 17:57:08.000000 rf_survey-0.1/src/src/rf_survey/__init__.py
+-rw-rw-rw-   0        0        0     3990 2024-03-08 19:15:58.000000 rf_survey-0.1/src/src/rf_survey/hardware.py
+-rw-rw-rw-   0        0        0      970 2024-03-08 19:15:58.000000 rf_survey-0.1/src/src/rf_survey/kill.py
+-rw-rw-rw-   0        0        0    13755 2024-03-08 19:15:58.000000 rf_survey-0.1/src/src/rf_survey/rf_survey.py
+-rw-rw-rw-   0        0        0    13278 2024-03-11 17:25:40.000000 rf_survey-0.1/src/src/rf_survey/sweeps.py
+-rw-rw-rw-   0        0        0     1740 2024-03-08 19:15:58.000000 rf_survey-0.1/src/src/rf_survey/wr_boot.py
+-rw-rw-rw-   0        0        0     2785 2024-03-08 19:15:58.000000 rf_survey-0.1/src/src/rf_survey/wr_poll.py
```

### Comparing `rf_survey-0.0.1/LICENSE.txt` & `rf_survey-0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/PKG-INFO` & `rf_survey-0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rf-survey
-Version: 0.0.1
+Name: rf_survey
+Version: 0.1
 Summary: An open source tool for measuring baseline radio frequency interference
 Author-email: WIRG lab <NSFCUSWIFTPASS@gmail.com>
 Project-URL: Homepage, https://github.com/NSFCUSWIFTPASS/RF_survey
 Project-URL: Issues, https://github.com/NSFCUSWIFTPASS/RF_survey/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rf_survey-0.0.1/README.md` & `rf_survey-0.1/README.md`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/pyproject.toml` & `rf_survey-0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "rf-survey"
-version = "0.0.1"
+name = "rf_survey"
+version = "0.1"
 authors = [
   { name="WIRG lab", email="NSFCUSWIFTPASS@gmail.com" },
 ]
 description = "An open source tool for measuring baseline radio frequency interference"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `rf_survey-0.0.1/src/rf_survey.egg-info/PKG-INFO` & `rf_survey-0.1/src/rf_survey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rf-survey
-Version: 0.0.1
+Name: rf_survey
+Version: 0.1
 Summary: An open source tool for measuring baseline radio frequency interference
 Author-email: WIRG lab <NSFCUSWIFTPASS@gmail.com>
 Project-URL: Homepage, https://github.com/NSFCUSWIFTPASS/RF_survey
 Project-URL: Issues, https://github.com/NSFCUSWIFTPASS/RF_survey/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rf_survey-0.0.1/src/rf_survey.egg-info/SOURCES.txt` & `rf_survey-0.1/src/rf_survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/src/src/monitoring/logins/ip_mailer.py` & `rf_survey-0.1/src/src/monitoring/logins/ip_mailer.py`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/src/src/rf_survey/Cronify.py` & `rf_survey-0.1/src/src/rf_survey/Cronify.py`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/src/src/rf_survey/GracefulKiller.py` & `rf_survey-0.1/src/src/rf_survey/GracefulKiller.py`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/src/src/rf_survey/Logger.py` & `rf_survey-0.1/src/src/rf_survey/Logger.py`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/src/src/rf_survey/Restoration.py` & `rf_survey-0.1/src/src/rf_survey/Restoration.py`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/src/src/rf_survey/hardware.py` & `rf_survey-0.1/src/src/rf_survey/hardware.py`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/src/src/rf_survey/kill.py` & `rf_survey-0.1/src/src/rf_survey/kill.py`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/src/src/rf_survey/rf_survey.py` & `rf_survey-0.1/src/src/rf_survey/rf_survey.py`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/src/src/rf_survey/sweeps.py` & `rf_survey-0.1/src/src/rf_survey/sweeps.py`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/src/src/rf_survey/wr_boot.py` & `rf_survey-0.1/src/src/rf_survey/wr_boot.py`

 * *Files identical despite different names*

### Comparing `rf_survey-0.0.1/src/src/rf_survey/wr_poll.py` & `rf_survey-0.1/src/src/rf_survey/wr_poll.py`

 * *Files identical despite different names*

