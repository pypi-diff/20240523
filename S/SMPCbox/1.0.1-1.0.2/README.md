# Comparing `tmp/SMPCbox-1.0.1.tar.gz` & `tmp/SMPCbox-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMPCbox-1.0.1.tar", last modified: Thu May 23 11:49:45 2024, max compression
+gzip compressed data, was "SMPCbox-1.0.2.tar", last modified: Thu May 23 11:55:52 2024, max compression
```

## Comparing `SMPCbox-1.0.1.tar` & `SMPCbox-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 bj        (1000) bj        (1000)        0 2024-05-23 11:49:45.080002 SMPCbox-1.0.1/
--rw-rw-r--   0 bj        (1000) bj        (1000)    35229 2024-05-23 11:25:03.000000 SMPCbox-1.0.1/LICENCE
--rw-rw-r--   0 bj        (1000) bj        (1000)      772 2024-05-23 11:49:45.080002 SMPCbox-1.0.1/PKG-INFO
--rw-rw-r--   0 bj        (1000) bj        (1000)     1187 2024-04-21 11:14:58.000000 SMPCbox-1.0.1/README.md
-drwxrwxr-x   0 bj        (1000) bj        (1000)        0 2024-05-23 11:49:45.076004 SMPCbox-1.0.1/SMPCbox/
--rw-rw-r--   0 bj        (1000) bj        (1000)    23822 2024-05-23 10:08:56.000000 SMPCbox-1.0.1/SMPCbox/AbstractProtocol.py
--rw-rw-r--   0 bj        (1000) bj        (1000)     6203 2024-05-23 10:15:57.000000 SMPCbox-1.0.1/SMPCbox/ProtocolParty.py
--rw-rw-r--   0 bj        (1000) bj        (1000)      721 2024-05-23 10:09:18.000000 SMPCbox-1.0.1/SMPCbox/ProtocolStep.py
--rw-rw-r--   0 bj        (1000) bj        (1000)     7733 2024-05-23 10:17:36.000000 SMPCbox-1.0.1/SMPCbox/SMPCSocket.py
--rw-rw-r--   0 bj        (1000) bj        (1000)      219 2024-05-23 11:48:27.000000 SMPCbox-1.0.1/SMPCbox/__init__.py
--rw-rw-r--   0 bj        (1000) bj        (1000)     8649 2024-05-21 14:20:35.000000 SMPCbox-1.0.1/SMPCbox/dynamic_loading.py
-drwxrwxr-x   0 bj        (1000) bj        (1000)        0 2024-05-23 11:49:45.080002 SMPCbox-1.0.1/SMPCbox.egg-info/
--rw-rw-r--   0 bj        (1000) bj        (1000)      772 2024-05-23 11:49:45.000000 SMPCbox-1.0.1/SMPCbox.egg-info/PKG-INFO
--rw-rw-r--   0 bj        (1000) bj        (1000)      296 2024-05-23 11:49:45.000000 SMPCbox-1.0.1/SMPCbox.egg-info/SOURCES.txt
--rw-rw-r--   0 bj        (1000) bj        (1000)        1 2024-05-23 11:49:45.000000 SMPCbox-1.0.1/SMPCbox.egg-info/dependency_links.txt
--rw-rw-r--   0 bj        (1000) bj        (1000)        8 2024-05-23 11:49:45.000000 SMPCbox-1.0.1/SMPCbox.egg-info/top_level.txt
--rw-rw-r--   0 bj        (1000) bj        (1000)       38 2024-05-23 11:49:45.080002 SMPCbox-1.0.1/setup.cfg
--rw-rw-r--   0 bj        (1000) bj        (1000)      948 2024-05-23 11:49:39.000000 SMPCbox-1.0.1/setup.py
+drwxrwxr-x   0 bj        (1000) bj        (1000)        0 2024-05-23 11:55:52.503905 SMPCbox-1.0.2/
+-rw-rw-r--   0 bj        (1000) bj        (1000)    35229 2024-05-23 11:25:03.000000 SMPCbox-1.0.2/LICENCE
+-rw-rw-r--   0 bj        (1000) bj        (1000)      772 2024-05-23 11:55:52.503905 SMPCbox-1.0.2/PKG-INFO
+-rw-rw-r--   0 bj        (1000) bj        (1000)     1187 2024-04-21 11:14:58.000000 SMPCbox-1.0.2/README.md
+drwxrwxr-x   0 bj        (1000) bj        (1000)        0 2024-05-23 11:55:52.503905 SMPCbox-1.0.2/SMPCbox/
+-rw-rw-r--   0 bj        (1000) bj        (1000)    23822 2024-05-23 10:08:56.000000 SMPCbox-1.0.2/SMPCbox/AbstractProtocol.py
+-rw-rw-r--   0 bj        (1000) bj        (1000)     6203 2024-05-23 10:15:57.000000 SMPCbox-1.0.2/SMPCbox/ProtocolParty.py
+-rw-rw-r--   0 bj        (1000) bj        (1000)      721 2024-05-23 10:09:18.000000 SMPCbox-1.0.2/SMPCbox/ProtocolStep.py
+-rw-rw-r--   0 bj        (1000) bj        (1000)     7733 2024-05-23 11:53:25.000000 SMPCbox-1.0.2/SMPCbox/SMPCSocket.py
+-rw-rw-r--   0 bj        (1000) bj        (1000)      221 2024-05-23 11:54:55.000000 SMPCbox-1.0.2/SMPCbox/__init__.py
+-rw-rw-r--   0 bj        (1000) bj        (1000)     8649 2024-05-21 14:20:35.000000 SMPCbox-1.0.2/SMPCbox/dynamic_loading.py
+drwxrwxr-x   0 bj        (1000) bj        (1000)        0 2024-05-23 11:55:52.503905 SMPCbox-1.0.2/SMPCbox.egg-info/
+-rw-rw-r--   0 bj        (1000) bj        (1000)      772 2024-05-23 11:55:52.000000 SMPCbox-1.0.2/SMPCbox.egg-info/PKG-INFO
+-rw-rw-r--   0 bj        (1000) bj        (1000)      296 2024-05-23 11:55:52.000000 SMPCbox-1.0.2/SMPCbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 bj        (1000) bj        (1000)        1 2024-05-23 11:55:52.000000 SMPCbox-1.0.2/SMPCbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 bj        (1000) bj        (1000)        8 2024-05-23 11:55:52.000000 SMPCbox-1.0.2/SMPCbox.egg-info/top_level.txt
+-rw-rw-r--   0 bj        (1000) bj        (1000)       38 2024-05-23 11:55:52.503905 SMPCbox-1.0.2/setup.cfg
+-rw-rw-r--   0 bj        (1000) bj        (1000)      948 2024-05-23 11:55:47.000000 SMPCbox-1.0.2/setup.py
```

### Comparing `SMPCbox-1.0.1/LICENCE` & `SMPCbox-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `SMPCbox-1.0.1/PKG-INFO` & `SMPCbox-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMPCbox
-Version: 1.0.1
+Version: 1.0.2
 Summary: A framework for implementation of secure multi party computation protocols
 Home-page: UNKNOWN
 Author: Bas Jansweijer, Luuk Jonker, Zoltan Mann
 Author-email: bas.jansweijer@student.uva.nl, luuk.jonker@student.uva.nl
 License: UNKNOWN
 Keywords: python,protocols,multi party computation,MPC,secure multi party computation,SMPC
 Platform: UNKNOWN
```

### Comparing `SMPCbox-1.0.1/README.md` & `SMPCbox-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `SMPCbox-1.0.1/SMPCbox/AbstractProtocol.py` & `SMPCbox-1.0.2/SMPCbox/AbstractProtocol.py`

 * *Files identical despite different names*

### Comparing `SMPCbox-1.0.1/SMPCbox/ProtocolParty.py` & `SMPCbox-1.0.2/SMPCbox/ProtocolParty.py`

 * *Files identical despite different names*

### Comparing `SMPCbox-1.0.1/SMPCbox/ProtocolStep.py` & `SMPCbox-1.0.2/SMPCbox/ProtocolStep.py`

 * *Files identical despite different names*

### Comparing `SMPCbox-1.0.1/SMPCbox/SMPCSocket.py` & `SMPCbox-1.0.2/SMPCbox/SMPCSocket.py`

 * *Files identical despite different names*

### Comparing `SMPCbox-1.0.1/SMPCbox/dynamic_loading.py` & `SMPCbox-1.0.2/SMPCbox/dynamic_loading.py`

 * *Files identical despite different names*

### Comparing `SMPCbox-1.0.1/SMPCbox.egg-info/PKG-INFO` & `SMPCbox-1.0.2/SMPCbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMPCbox
-Version: 1.0.1
+Version: 1.0.2
 Summary: A framework for implementation of secure multi party computation protocols
 Home-page: UNKNOWN
 Author: Bas Jansweijer, Luuk Jonker, Zoltan Mann
 Author-email: bas.jansweijer@student.uva.nl, luuk.jonker@student.uva.nl
 License: UNKNOWN
 Keywords: python,protocols,multi party computation,MPC,secure multi party computation,SMPC
 Platform: UNKNOWN
```

### Comparing `SMPCbox-1.0.1/setup.py` & `SMPCbox-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 SMPCbox is a framework which can be used to implement Secure Multi Party Computation (SMPC) protocols.
 The idea behind the project is to provide a way to easily test protocols, visualise protocol execution
 and gather statistics on protocol execution.
 This framework is meant to help researchers and students to better understand SMPC protocols.
 """
 
 setup(name='SMPCbox',
-      version='1.0.1',
+      version='1.0.2',
       description='A framework for implementation of secure multi party computation protocols',
       author='Bas Jansweijer, Luuk Jonker, Zoltan Mann',
       author_email='bas.jansweijer@student.uva.nl, luuk.jonker@student.uva.nl',
       long_description=LONG_DESCRIPTION,
       packages=find_packages(),
     #   url='https://www.python.org/sigs/distutils-sig/',
       keywords=['python', 'protocols', 'multi party computation', 'MPC', 'secure multi party computation', 'SMPC']
```

