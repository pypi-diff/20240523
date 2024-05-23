# Comparing `tmp/arch_flow-0.1.7.4.tar.gz` & `tmp/arch_flow-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_flow-0.1.7.4.tar", last modified: Tue May 21 02:57:58 2024, max compression
+gzip compressed data, was "arch_flow-0.1.8.tar", last modified: Thu May 23 07:33:34 2024, max compression
```

## Comparing `arch_flow-0.1.7.4.tar` & `arch_flow-0.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 02:57:58.212275 arch_flow-0.1.7.4/
--rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.7.4/LICENCE
--rw-rw-rw-   0        0        0      983 2024-05-21 02:57:58.211275 arch_flow-0.1.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     6622 2024-04-25 23:30:53.000000 arch_flow-0.1.7.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 02:57:58.182271 arch_flow-0.1.7.4/arch_flow/
--rw-rw-rw-   0        0        0     5165 2024-05-21 02:24:38.000000 arch_flow-0.1.7.4/arch_flow/ArchFlow.py
--rw-rw-rw-   0        0        0      260 2024-05-21 02:57:55.000000 arch_flow-0.1.7.4/arch_flow/ArchFlowCli.py
--rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.7.4/arch_flow/DirectoryCreator.py
--rw-rw-rw-   0        0        0     3301 2024-05-04 03:27:18.000000 arch_flow-0.1.7.4/arch_flow/DirectoryExplorer.py
--rw-rw-rw-   0        0        0      363 2024-05-21 01:57:35.000000 arch_flow-0.1.7.4/arch_flow/Run.py
--rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.7.4/arch_flow/StringManipulator.py
--rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.7.4/arch_flow/__init__.py
--rw-rw-rw-   0        0        0      102 2024-05-21 02:57:55.000000 arch_flow-0.1.7.4/arch_flow/db.json
-drwxrwxrwx   0        0        0        0 2024-05-21 02:57:58.201970 arch_flow-0.1.7.4/arch_flow/exceptions/
--rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.7.4/arch_flow/exceptions/ExceptionHandler.py
--rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.7.4/arch_flow/exceptions/FileOrDirectoryExistsError.py
--rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.7.4/arch_flow/exceptions/NotFoundException.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:57:58.205972 arch_flow-0.1.7.4/arch_flow/implementations/
--rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.7.4/arch_flow/implementations/DirectoryCreatorImplementation.py
--rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.7.4/arch_flow/implementations/DirectoryExplorerImplementation.py
--rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.7.4/arch_flow/implementations/StringManipulatorImplementation.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:57:58.207278 arch_flow-0.1.7.4/arch_flow/output/
--rw-rw-rw-   0        0        0     2372 2024-03-15 22:56:29.000000 arch_flow-0.1.7.4/arch_flow/output/OutputHandler.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:57:58.209278 arch_flow-0.1.7.4/arch_flow/utils/
--rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.7.4/arch_flow/utils/DirectoryExplorerUtil.py
--rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.7.4/arch_flow/utils/Filter.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:57:58.210276 arch_flow-0.1.7.4/arch_flow.egg-info/
--rw-rw-rw-   0        0        0      983 2024-05-21 02:57:58.000000 arch_flow-0.1.7.4/arch_flow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      803 2024-05-21 02:57:58.000000 arch_flow-0.1.7.4/arch_flow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 02:57:58.000000 arch_flow-0.1.7.4/arch_flow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-21 02:57:58.000000 arch_flow-0.1.7.4/arch_flow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-21 02:57:58.000000 arch_flow-0.1.7.4/arch_flow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 02:57:58.213275 arch_flow-0.1.7.4/setup.cfg
--rw-rw-rw-   0        0        0     1246 2024-05-21 02:57:55.000000 arch_flow-0.1.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:33:34.654294 arch_flow-0.1.8/
+-rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.8/LICENCE
+-rw-rw-rw-   0        0        0     1002 2024-05-23 07:33:34.653294 arch_flow-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6622 2024-04-25 23:30:53.000000 arch_flow-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 07:33:34.577001 arch_flow-0.1.8/arch_flow/
+-rw-rw-rw-   0        0        0     5165 2024-05-21 02:24:38.000000 arch_flow-0.1.8/arch_flow/ArchFlow.py
+-rw-rw-rw-   0        0        0      260 2024-05-21 02:57:55.000000 arch_flow-0.1.8/arch_flow/ArchFlowCli.py
+-rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.8/arch_flow/DirectoryCreator.py
+-rw-rw-rw-   0        0        0     3301 2024-05-04 03:27:18.000000 arch_flow-0.1.8/arch_flow/DirectoryExplorer.py
+-rw-rw-rw-   0        0        0      363 2024-05-21 01:57:35.000000 arch_flow-0.1.8/arch_flow/Run.py
+-rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.8/arch_flow/StringManipulator.py
+-rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.8/arch_flow/__init__.py
+-rw-rw-rw-   0        0        0      102 2024-05-21 02:57:55.000000 arch_flow-0.1.8/arch_flow/db.json
+drwxrwxrwx   0        0        0        0 2024-05-23 07:33:34.618005 arch_flow-0.1.8/arch_flow/exceptions/
+-rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.8/arch_flow/exceptions/ExceptionHandler.py
+-rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.8/arch_flow/exceptions/FileOrDirectoryExistsError.py
+-rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.8/arch_flow/exceptions/NotFoundException.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:33:34.636293 arch_flow-0.1.8/arch_flow/implementations/
+-rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.8/arch_flow/implementations/DirectoryCreatorImplementation.py
+-rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.8/arch_flow/implementations/DirectoryExplorerImplementation.py
+-rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.8/arch_flow/implementations/StringManipulatorImplementation.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:33:34.637294 arch_flow-0.1.8/arch_flow/output/
+-rw-rw-rw-   0        0        0     4127 2024-05-23 07:33:32.000000 arch_flow-0.1.8/arch_flow/output/OutputHandler.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:33:34.651292 arch_flow-0.1.8/arch_flow/utils/
+-rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.8/arch_flow/utils/DirectoryExplorerUtil.py
+-rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.8/arch_flow/utils/Filter.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:33:34.652294 arch_flow-0.1.8/arch_flow.egg-info/
+-rw-rw-rw-   0        0        0     1002 2024-05-23 07:33:34.000000 arch_flow-0.1.8/arch_flow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      803 2024-05-23 07:33:34.000000 arch_flow-0.1.8/arch_flow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 07:33:34.000000 arch_flow-0.1.8/arch_flow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 07:33:34.000000 arch_flow-0.1.8/arch_flow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 07:33:34.000000 arch_flow-0.1.8/arch_flow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 07:33:34.654294 arch_flow-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2024-05-23 07:33:32.000000 arch_flow-0.1.8/setup.py
```

### Comparing `arch_flow-0.1.7.4/LICENCE` & `arch_flow-0.1.8/LICENCE`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/PKG-INFO` & `arch_flow-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.7.4
+Version: 0.1.8
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: colorama
+Requires-Dist: rich
 
 O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações. Inspirado no conceito de peças de Lego, o ArchFlow oferece uma variedade de módulos independentes, cada um com funcionalidades específicas. Esses módulos podem ser combinados de forma flexível para atender às necessidades de automação de diferentes projetos. Com uma arquitetura modular e uma ampla gama de funções, o ArchFlow permite aos desenvolvedores criar soluções eficientes e personalizadas, reduzindo o tempo e esforço necessários para o desenvolvimento de software.
```

### Comparing `arch_flow-0.1.7.4/README.md` & `arch_flow-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/arch_flow/ArchFlow.py` & `arch_flow-0.1.8/arch_flow/ArchFlow.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/arch_flow/DirectoryCreator.py` & `arch_flow-0.1.8/arch_flow/DirectoryCreator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/arch_flow/DirectoryExplorer.py` & `arch_flow-0.1.8/arch_flow/DirectoryExplorer.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/arch_flow/StringManipulator.py` & `arch_flow-0.1.8/arch_flow/StringManipulator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/arch_flow/exceptions/ExceptionHandler.py` & `arch_flow-0.1.8/arch_flow/exceptions/ExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/arch_flow/exceptions/FileOrDirectoryExistsError.py` & `arch_flow-0.1.8/arch_flow/exceptions/FileOrDirectoryExistsError.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/arch_flow/exceptions/NotFoundException.py` & `arch_flow-0.1.8/arch_flow/exceptions/NotFoundException.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/arch_flow/implementations/DirectoryCreatorImplementation.py` & `arch_flow-0.1.8/arch_flow/implementations/DirectoryCreatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/arch_flow/implementations/DirectoryExplorerImplementation.py` & `arch_flow-0.1.8/arch_flow/implementations/DirectoryExplorerImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/arch_flow/implementations/StringManipulatorImplementation.py` & `arch_flow-0.1.8/arch_flow/implementations/StringManipulatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/arch_flow/utils/Filter.py` & `arch_flow-0.1.8/arch_flow/utils/Filter.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/arch_flow.egg-info/PKG-INFO` & `arch_flow-0.1.8/arch_flow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.7.4
+Version: 0.1.8
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: colorama
+Requires-Dist: rich
 
 O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações. Inspirado no conceito de peças de Lego, o ArchFlow oferece uma variedade de módulos independentes, cada um com funcionalidades específicas. Esses módulos podem ser combinados de forma flexível para atender às necessidades de automação de diferentes projetos. Com uma arquitetura modular e uma ampla gama de funções, o ArchFlow permite aos desenvolvedores criar soluções eficientes e personalizadas, reduzindo o tempo e esforço necessários para o desenvolvimento de software.
```

### Comparing `arch_flow-0.1.7.4/arch_flow.egg-info/SOURCES.txt` & `arch_flow-0.1.8/arch_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.4/setup.py` & `arch_flow-0.1.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 
 setup(name='arch-flow',
-    version='0.1.7.4',
+    version='0.1.8',
     license='MIT License',
     author='Carlos Vinicius Da Silva',
     long_description="O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações. Inspirado no conceito de peças de Lego, o ArchFlow oferece uma variedade de módulos independentes, cada um com funcionalidades específicas. Esses módulos podem ser combinados de forma flexível para atender às necessidades de automação de diferentes projetos. Com uma arquitetura modular e uma ampla gama de funções, o ArchFlow permite aos desenvolvedores criar soluções eficientes e personalizadas, reduzindo o tempo e esforço necessários para o desenvolvimento de software.",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='arch flow',
     description=u'O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.',
     package_data={
         'arch_flow':['*.json']
       },
     packages=['arch_flow', 'arch_flow.exceptions', 'arch_flow.implementations', 'arch_flow.output', 'arch_flow.utils'],
-    install_requires=['colorama'],)
+    install_requires=['colorama', 'rich'],)
```

