# Comparing `tmp/cae_cli-0.2.9.1.tar.gz` & `tmp/cae_cli-0.2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.2.9.1.tar", last modified: Thu May 23 07:36:59 2024, max compression
+gzip compressed data, was "cae_cli-0.2.9.2.tar", last modified: Thu May 23 07:42:29 2024, max compression
```

## Comparing `cae_cli-0.2.9.1.tar` & `cae_cli-0.2.9.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 07:36:59.926611 cae_cli-0.2.9.1/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.9.1/LICENSE
--rw-rw-rw-   0        0        0      417 2024-05-23 07:36:59.925611 cae_cli-0.2.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.9.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 07:36:59.786083 cae_cli-0.2.9.1/cae/
--rw-rw-rw-   0        0        0     9506 2024-05-09 22:42:15.000000 cae_cli-0.2.9.1/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.9.1/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.9.1/cae/__init__.py
--rw-rw-rw-   0        0        0    10247 2024-05-09 22:46:38.000000 cae_cli-0.2.9.1/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-23 07:36:59.913602 cae_cli-0.2.9.1/cae/templates/
--rw-rw-rw-   0        0        0     1000 2024-05-14 19:33:43.000000 cae_cli-0.2.9.1/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.9.1/cae/templates/dependency_wrapper.txt
--rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.9.1/cae/templates/entity.txt
--rw-rw-rw-   0        0        0      770 2024-05-09 02:30:03.000000 cae_cli-0.2.9.1/cae/templates/entityFactory.txt
--rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.9.1/cae/templates/entityImplementation.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.9.1/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.9.1/cae/templates/implementation_ruc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.9.1/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1737 2024-05-14 19:27:43.000000 cae_cli-0.2.9.1/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.9.1/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1945 2024-05-09 22:31:57.000000 cae_cli-0.2.9.1/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.9.1/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-09 02:30:03.000000 cae_cli-0.2.9.1/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.9.1/cae/templates/use_case_factory.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.9.1/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.9.1/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.9.1/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      236 2024-05-09 02:34:53.000000 cae_cli-0.2.9.1/cae/templates/use_case_ruc.txt
--rw-rw-rw-   0        0        0      408 2024-05-09 02:34:53.000000 cae_cli-0.2.9.1/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 07:36:59.924614 cae_cli-0.2.9.1/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      417 2024-05-23 07:36:59.000000 cae_cli-0.2.9.1/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      869 2024-05-23 07:36:59.000000 cae_cli-0.2.9.1/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 07:36:59.000000 cae_cli-0.2.9.1/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-23 07:36:59.000000 cae_cli-0.2.9.1/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-23 07:36:59.000000 cae_cli-0.2.9.1/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 07:36:59.926611 cae_cli-0.2.9.1/setup.cfg
--rw-rw-rw-   0        0        0      612 2024-05-23 07:36:56.000000 cae_cli-0.2.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:42:29.217714 cae_cli-0.2.9.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.9.2/LICENSE
+-rw-rw-rw-   0        0        0      419 2024-05-23 07:42:29.216714 cae_cli-0.2.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.9.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 07:42:29.181204 cae_cli-0.2.9.2/cae/
+-rw-rw-rw-   0        0        0     9506 2024-05-09 22:42:15.000000 cae_cli-0.2.9.2/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.9.2/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.9.2/cae/__init__.py
+-rw-rw-rw-   0        0        0    10247 2024-05-09 22:46:38.000000 cae_cli-0.2.9.2/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-23 07:42:29.200206 cae_cli-0.2.9.2/cae/templates/
+-rw-rw-rw-   0        0        0     1000 2024-05-14 19:33:43.000000 cae_cli-0.2.9.2/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.9.2/cae/templates/dependency_wrapper.txt
+-rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.9.2/cae/templates/entity.txt
+-rw-rw-rw-   0        0        0      770 2024-05-09 02:30:03.000000 cae_cli-0.2.9.2/cae/templates/entityFactory.txt
+-rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.9.2/cae/templates/entityImplementation.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.9.2/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.9.2/cae/templates/implementation_ruc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.9.2/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1737 2024-05-14 19:27:43.000000 cae_cli-0.2.9.2/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.9.2/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-09 22:31:57.000000 cae_cli-0.2.9.2/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.9.2/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-09 02:30:03.000000 cae_cli-0.2.9.2/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.9.2/cae/templates/use_case_factory.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.9.2/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.9.2/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.9.2/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      236 2024-05-09 02:34:53.000000 cae_cli-0.2.9.2/cae/templates/use_case_ruc.txt
+-rw-rw-rw-   0        0        0      408 2024-05-09 02:34:53.000000 cae_cli-0.2.9.2/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 07:42:29.215713 cae_cli-0.2.9.2/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      419 2024-05-23 07:42:29.000000 cae_cli-0.2.9.2/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      869 2024-05-23 07:42:29.000000 cae_cli-0.2.9.2/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 07:42:29.000000 cae_cli-0.2.9.2/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-23 07:42:29.000000 cae_cli-0.2.9.2/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-23 07:42:29.000000 cae_cli-0.2.9.2/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 07:42:29.217714 cae_cli-0.2.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      614 2024-05-23 07:42:22.000000 cae_cli-0.2.9.2/setup.py
```

### Comparing `cae_cli-0.2.9.1/LICENSE` & `cae_cli-0.2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/README.md` & `cae_cli-0.2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/ArchFlowJavaWeb.py` & `cae_cli-0.2.9.2/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/db.json` & `cae_cli-0.2.9.2/cae/db.json`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/templates/assembler.txt` & `cae_cli-0.2.9.2/cae/templates/assembler.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/templates/entityFactory.txt` & `cae_cli-0.2.9.2/cae/templates/entityFactory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/templates/implementation_cuc.txt` & `cae_cli-0.2.9.2/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/templates/implementation_ruc.txt` & `cae_cli-0.2.9.2/cae/templates/implementation_ruc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/templates/implementation_suc.txt` & `cae_cli-0.2.9.2/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/templates/pom-adapters.txt` & `cae_cli-0.2.9.2/cae/templates/pom-adapters.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/templates/pom-assemblers.txt` & `cae_cli-0.2.9.2/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/templates/pom-core.txt` & `cae_cli-0.2.9.2/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/templates/use_case.txt` & `cae_cli-0.2.9.2/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/templates/use_case_factory.txt` & `cae_cli-0.2.9.2/cae/templates/use_case_factory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae/templates/use_case_implementation.txt` & `cae_cli-0.2.9.2/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.2.9.2/cae_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.1/setup.py` & `cae_cli-0.2.9.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.2.9.1',
+    version='0.2.9.2',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
     packages=['cae'],
     package_data={
           'cae': ['templates/*.txt', '*.json']
     },
     install_requires=[
-        'arch-flow>=0.1.8',
+        'arch-flow>=0.1.8.1',
         'colorama'
       ],
 )
```

