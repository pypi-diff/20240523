# Comparing `tmp/csle_attacker-0.5.3.tar.gz` & `tmp/csle_attacker-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_attacker-0.5.3.tar", last modified: Mon May 13 17:19:42 2024, max compression
+gzip compressed data, was "csle_attacker-0.6.0.tar", last modified: Thu May 23 17:43:11 2024, max compression
```

## Comparing `csle_attacker-0.5.3.tar` & `csle_attacker-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.162508 csle_attacker-0.5.3/
--rw-rw-r--   0 kim       (1000) kim       (1000)      649 2024-05-13 17:19:42.162508 csle_attacker-0.5.3/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3866 2024-01-29 11:24:00.000000 csle_attacker-0.5.3/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      673 2023-08-08 14:54:06.000000 csle_attacker-0.5.3/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1734 2024-05-13 17:19:42.162508 csle_attacker-0.5.3/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.158508 csle_attacker-0.5.3/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.158508 csle_attacker-0.5.3/src/csle_attacker/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_attacker-0.5.3/src/csle_attacker/__version__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      941 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/attacker.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.162508 csle_attacker-0.5.3/src/csle_attacker/emulation/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      994 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/attacker_stopping_middleware.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11411 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/emulated_attacker.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11564 2023-07-28 08:44:18.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/exploit_middleware.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4678 2023-07-28 08:44:18.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/post_exploit_middleware.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5951 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/recon_middleware.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.162508 csle_attacker-0.5.3/src/csle_attacker/emulation/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    45676 2024-01-29 11:24:00.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/util/exploit_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7720 2023-07-28 08:44:18.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/util/nikto_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    34952 2024-01-29 11:24:00.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/util/nmap_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    30139 2023-07-28 08:44:18.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/util/shell_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.158508 csle_attacker-0.5.3/src/csle_attacker.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      649 2024-05-13 17:19:42.000000 csle_attacker-0.5.3/src/csle_attacker.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      941 2024-05-13 17:19:42.000000 csle_attacker-0.5.3/src/csle_attacker.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:19:42.000000 csle_attacker-0.5.3/src/csle_attacker.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:55.000000 csle_attacker-0.5.3/src/csle_attacker.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      475 2024-05-13 17:19:42.000000 csle_attacker-0.5.3/src/csle_attacker.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       14 2024-05-13 17:19:42.000000 csle_attacker-0.5.3/src/csle_attacker.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.162508 csle_attacker-0.5.3/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)     1790 2024-01-29 11:24:00.000000 csle_attacker-0.5.3/tests/test_shell_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:11.354811 csle_attacker-0.6.0/
+-rw-r--r--   0 kim        (501) staff       (20)      649 2024-05-23 17:43:11.354854 csle_attacker-0.6.0/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     3866 2024-02-13 12:24:16.000000 csle_attacker-0.6.0/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      673 2023-08-15 10:44:03.000000 csle_attacker-0.6.0/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     1734 2024-05-23 17:43:11.355086 csle_attacker-0.6.0/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_attacker-0.6.0/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:11.342110 csle_attacker-0.6.0/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:11.345748 csle_attacker-0.6.0/src/csle_attacker/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_attacker-0.6.0/src/csle_attacker/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 17:42:57.000000 csle_attacker-0.6.0/src/csle_attacker/__version__.py
+-rw-r--r--   0 kim        (501) staff       (20)      941 2023-08-15 10:44:03.000000 csle_attacker-0.6.0/src/csle_attacker/attacker.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:11.348013 csle_attacker-0.6.0/src/csle_attacker/emulation/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_attacker-0.6.0/src/csle_attacker/emulation/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)      994 2023-08-15 10:44:03.000000 csle_attacker-0.6.0/src/csle_attacker/emulation/attacker_stopping_middleware.py
+-rw-r--r--   0 kim        (501) staff       (20)    11411 2023-08-15 10:44:03.000000 csle_attacker-0.6.0/src/csle_attacker/emulation/emulated_attacker.py
+-rw-r--r--   0 kim        (501) staff       (20)    11564 2023-08-15 10:44:03.000000 csle_attacker-0.6.0/src/csle_attacker/emulation/exploit_middleware.py
+-rw-r--r--   0 kim        (501) staff       (20)     4678 2023-08-15 10:44:03.000000 csle_attacker-0.6.0/src/csle_attacker/emulation/post_exploit_middleware.py
+-rw-r--r--   0 kim        (501) staff       (20)     5951 2023-08-15 10:44:03.000000 csle_attacker-0.6.0/src/csle_attacker/emulation/recon_middleware.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:11.354358 csle_attacker-0.6.0/src/csle_attacker/emulation/util/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_attacker-0.6.0/src/csle_attacker/emulation/util/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    45676 2023-10-10 07:21:48.000000 csle_attacker-0.6.0/src/csle_attacker/emulation/util/exploit_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     7720 2023-08-15 10:44:03.000000 csle_attacker-0.6.0/src/csle_attacker/emulation/util/nikto_util.py
+-rw-r--r--   0 kim        (501) staff       (20)    34952 2024-02-13 12:24:16.000000 csle_attacker-0.6.0/src/csle_attacker/emulation/util/nmap_util.py
+-rw-r--r--   0 kim        (501) staff       (20)    30139 2023-10-10 07:21:48.000000 csle_attacker-0.6.0/src/csle_attacker/emulation/util/shell_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:11.346821 csle_attacker-0.6.0/src/csle_attacker.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      649 2024-05-23 17:43:11.000000 csle_attacker-0.6.0/src/csle_attacker.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)      941 2024-05-23 17:43:11.000000 csle_attacker-0.6.0/src/csle_attacker.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 17:43:11.000000 csle_attacker-0.6.0/src/csle_attacker.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:41.000000 csle_attacker-0.6.0/src/csle_attacker.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      475 2024-05-23 17:43:11.000000 csle_attacker-0.6.0/src/csle_attacker.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       14 2024-05-23 17:43:11.000000 csle_attacker-0.6.0/src/csle_attacker.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 17:43:11.354550 csle_attacker-0.6.0/tests/
+-rw-r--r--   0 kim        (501) staff       (20)     1790 2023-08-17 14:41:23.000000 csle_attacker-0.6.0/tests/test_shell_util.py
```

### Comparing `csle_attacker-0.5.3/PKG-INFO` & `csle_attacker-0.6.0/src/csle_attacker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: csle_attacker
-Version: 0.5.3
+Name: csle-attacker
+Version: 0.6.0
 Summary: Scripts for emulated cyber attacks in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attacker-0.5.3/README.md` & `csle_attacker-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/pyproject.toml` & `csle_attacker-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/setup.cfg` & `csle_attacker-0.6.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-base>=0.5.3
-	csle-common>=0.5.3
+	csle-base>=0.6.0
+	csle-common>=0.6.0
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_attacker-0.5.3/src/csle_attacker/attacker.py` & `csle_attacker-0.6.0/src/csle_attacker/attacker.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/src/csle_attacker/emulation/attacker_stopping_middleware.py` & `csle_attacker-0.6.0/src/csle_attacker/emulation/attacker_stopping_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/src/csle_attacker/emulation/emulated_attacker.py` & `csle_attacker-0.6.0/src/csle_attacker/emulation/emulated_attacker.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/src/csle_attacker/emulation/exploit_middleware.py` & `csle_attacker-0.6.0/src/csle_attacker/emulation/exploit_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/src/csle_attacker/emulation/post_exploit_middleware.py` & `csle_attacker-0.6.0/src/csle_attacker/emulation/post_exploit_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/src/csle_attacker/emulation/recon_middleware.py` & `csle_attacker-0.6.0/src/csle_attacker/emulation/recon_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/src/csle_attacker/emulation/util/exploit_util.py` & `csle_attacker-0.6.0/src/csle_attacker/emulation/util/exploit_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/src/csle_attacker/emulation/util/nikto_util.py` & `csle_attacker-0.6.0/src/csle_attacker/emulation/util/nikto_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/src/csle_attacker/emulation/util/nmap_util.py` & `csle_attacker-0.6.0/src/csle_attacker/emulation/util/nmap_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/src/csle_attacker/emulation/util/shell_util.py` & `csle_attacker-0.6.0/src/csle_attacker/emulation/util/shell_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/src/csle_attacker.egg-info/PKG-INFO` & `csle_attacker-0.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: csle-attacker
-Version: 0.5.3
+Name: csle_attacker
+Version: 0.6.0
 Summary: Scripts for emulated cyber attacks in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attacker-0.5.3/src/csle_attacker.egg-info/SOURCES.txt` & `csle_attacker-0.6.0/src/csle_attacker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.3/tests/test_shell_util.py` & `csle_attacker-0.6.0/tests/test_shell_util.py`

 * *Files identical despite different names*

