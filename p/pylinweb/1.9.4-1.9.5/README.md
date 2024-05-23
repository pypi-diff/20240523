# Comparing `tmp/pylinweb-1.9.4.tar.gz` & `tmp/pylinweb-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinweb-1.9.4.tar", last modified: Thu May  2 21:30:54 2024, max compression
+gzip compressed data, was "pylinweb-1.9.5.tar", last modified: Thu May 23 14:47:00 2024, max compression
```

## Comparing `pylinweb-1.9.4.tar` & `pylinweb-1.9.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 21:30:54.547089 pylinweb-1.9.4/
--rw-rw-rw-   0        0        0       46 2024-04-30 04:05:30.000000 pylinweb-1.9.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3042 2024-05-02 21:30:54.544726 pylinweb-1.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     2103 2024-05-02 20:43:22.000000 pylinweb-1.9.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 21:30:54.510985 pylinweb-1.9.4/pylinweb/
--rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 pylinweb-1.9.4/pylinweb/__init__.py
--rw-rw-rw-   0        0        0     4315 2024-05-02 21:27:42.000000 pylinweb-1.9.4/pylinweb/functions.py
--rw-rw-rw-   0        0        0     1686 2024-05-02 20:47:00.000000 pylinweb-1.9.4/pylinweb/main.py
--rw-rw-rw-   0        0        0       99 2024-05-02 21:30:12.000000 pylinweb-1.9.4/pylinweb/variables.py
-drwxrwxrwx   0        0        0        0 2024-05-02 21:30:54.543709 pylinweb-1.9.4/pylinweb.egg-info/
--rw-rw-rw-   0        0        0     3042 2024-05-02 21:30:54.000000 pylinweb-1.9.4/pylinweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-05-02 21:30:54.000000 pylinweb-1.9.4/pylinweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 21:30:54.000000 pylinweb-1.9.4/pylinweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-02 21:30:54.000000 pylinweb-1.9.4/pylinweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2024-05-02 21:30:54.000000 pylinweb-1.9.4/pylinweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 21:30:54.000000 pylinweb-1.9.4/pylinweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 21:30:54.547089 pylinweb-1.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1460 2024-04-30 03:40:44.000000 pylinweb-1.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:47:00.000196 pylinweb-1.9.5/
+-rw-rw-rw-   0        0        0       46 2024-05-21 20:57:03.000000 pylinweb-1.9.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3144 2024-05-23 14:46:59.999190 pylinweb-1.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2103 2024-05-21 20:57:03.000000 pylinweb-1.9.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:46:59.991491 pylinweb-1.9.5/pylinweb/
+-rw-rw-rw-   0        0        0       63 2024-05-21 20:57:03.000000 pylinweb-1.9.5/pylinweb/__init__.py
+-rw-rw-rw-   0        0        0     4888 2024-05-23 14:46:00.000000 pylinweb-1.9.5/pylinweb/functions.py
+-rw-rw-rw-   0        0        0     1798 2024-05-21 21:07:32.000000 pylinweb-1.9.5/pylinweb/main.py
+-rw-rw-rw-   0        0        0       99 2024-05-21 21:08:29.000000 pylinweb-1.9.5/pylinweb/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:46:59.995399 pylinweb-1.9.5/pylinweb.egg-info/
+-rw-rw-rw-   0        0        0     3144 2024-05-23 14:46:59.000000 pylinweb-1.9.5/pylinweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-23 14:46:59.000000 pylinweb-1.9.5/pylinweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:46:59.000000 pylinweb-1.9.5/pylinweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-23 14:46:59.000000 pylinweb-1.9.5/pylinweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      338 2024-05-23 14:46:59.000000 pylinweb-1.9.5/pylinweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 14:46:59.000000 pylinweb-1.9.5/pylinweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:47:00.000196 pylinweb-1.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1550 2024-05-23 14:44:39.000000 pylinweb-1.9.5/setup.py
```

### Comparing `pylinweb-1.9.4/PKG-INFO` & `pylinweb-1.9.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylinweb
-Version: 1.9.4
+Version: 1.9.5
 Summary: A simple functional test library using Python and Selenium
 Author: Linda Lopez
 Keywords: selenium,testing,web,chrome
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,19 +14,22 @@
 Requires-Dist: behave==1.2.6
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
 Requires-Dist: playwright==1.42.0
 Requires-Dist: psutil==5.9.2
+Requires-Dist: pillow==10.3.0
+Requires-Dist: openpyxl==3.1.2
+Requires-Dist: customtkinter==5.2.2
 Requires-Dist: PyPDF2==3.0.1
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: pycparser==2.21
 Requires-Dist: screeninfo==0.8
-Requires-Dist: selenium==4.12
+Requires-Dist: selenium==4.20.0
 Requires-Dist: keyboard==0.13.5
 
 # Pylinweb
 
 Pylinweb es una biblioteca de pruebas funcionales simple que utiliza Python, Selenium y Chrome driver.
 
 ## Pre-requisitos
```

### Comparing `pylinweb-1.9.4/README.md` & `pylinweb-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `pylinweb-1.9.4/pylinweb/functions.py` & `pylinweb-1.9.5/pylinweb/functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,23 +24,24 @@
         subprocess.run('npm install -g allure-commandline', shell=True)
         subprocess.run('allure --version', shell=True)
 
     print('Dependencias instaladas exitosamente.')
 
 def execute_tests():
     print('Ejecutando pruebas...')
-    subprocess.run('behave --no-skipped', shell=True)
+    subprocess.run('behave --no-skipped --no-capture', shell=True)
 
 def generate_report_html():
     print('Generando reporte...')
     subprocess.run('allure generate', shell=True)
     subprocess.run('allure open', shell=True)
 
 def generate_report_word():
     subprocess.run('python ./src/test/config/generate_word_web.py', shell=True)
+    print("El reporte word se ha generado en la carpeta Evidencias")
 
 def reset_files():
     folders = ["allure-report", "allure-results", "screenshots", "Evidencias"]
     current_dir = os.getcwd()
 
     for folder in folders:
         folder_path = os.path.join(current_dir, folder)
@@ -57,15 +58,15 @@
     if repository_type == "Github":
         repository_name = select_repository_name()
         branch_name = select_brach_name()
         url_repository = f"https://github.com/aariverar/{repository_name}.git"
     elif repository_type == "Azure Repos":
         repository_name = select_repository_name()
         branch_name = select_brach_name()
-        url_repository = f"https://github.com/aariverar/{repository_name}.git"
+        url_repository = f"https://mibanco-devops@dev.azure.com/mibanco-devops/DevOps/_git/{repository_name}"
     else: 
         url_repository = None
 
     if url_repository is not None:
         # Verificar si la rama existe en el repositorio remoto
         result = subprocess.run(f'git ls-remote --heads {url_repository} {branch_name}', shell=True, capture_output=True, text=True)
         if branch_name in result.stdout:
@@ -102,8 +103,24 @@
     return repository_name
 
 def select_brach_name():
     branch_name = input('Escribe el nombre de la rama (La rama debe existir en el repositorio): ')
     return branch_name
 
 def open_application():
-    subprocess.run('python ./src/test/config/app_run.py', shell=True)
+    subprocess.run('python ./src/test/config/app_run.py', shell=True) #modified
+
+#######################################################
+
+def open_log_file():
+    current_dir = os.getcwd()
+    excel_file = "src/test/resources/log/log.xlsx"
+    excel_path = os.path.join(current_dir, excel_file)
+    subprocess.run(f'start {excel_path}', shell=True)
+
+def open_excel_data():
+    current_path = os.getcwd()
+    excel_file = os.path.join(current_path, 'src/test/resources/data/excel')
+    os.startfile(excel_file)
+
+
+
```

### Comparing `pylinweb-1.9.4/pylinweb/main.py` & `pylinweb-1.9.5/pylinweb/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 # main.py
 import argparse
 from .variables import *
-from .functions import (
-print_version, reset_files, 
-generate_report_html, 
-generate_report_word,
-install_dependencies, 
-execute_tests,
-clone_repository,
-open_application)
+from .functions import *
 
 def main():
     parser = argparse.ArgumentParser(description='Testing utility for web applications.')
     
     # Define arguments
     parser.add_argument('--setup', action='store_true', help=f'Copy {app} directory and install dependencies')
     parser.add_argument('--version', action='store_true', help='Show version')
     parser.add_argument('--run-tests', action='store_true', help='Run tests')
     parser.add_argument('--report-html', action='store_true', help='Generate html report')
     parser.add_argument('--report-word', action='store_true', help='Generate word report')
     parser.add_argument('--reset', action='store_true', help='Delete innecesary directories and files')
     parser.add_argument('--open-app', action='store_true', help='Open application')
+    parser.add_argument('--open-logs', action='store_true', help='Open logs in excel file')
+    parser.add_argument('--modify-data', action='store_true', help='Modify data in excel file')
 
     args = parser.parse_args()
     
     #Define actions and their corresponding functions
     actions = {
         'setup': lambda: (clone_repository(), install_dependencies()),
         'version': print_version,
         'run_tests': execute_tests,
         'report_html': generate_report_html,
         'report_word': generate_report_word,
         'reset': reset_files,
-        'open_app': open_application
+        'open_app': open_application,
+        'open_logs':open_log_file,
+        'modify_data': open_excel_data
     }
 
     # Get the first truthy argument
     arg = next((arg for arg in vars(args) if getattr(args, arg)), None)
 
     if arg in actions:
         actions[arg]()
```

### Comparing `pylinweb-1.9.4/pylinweb.egg-info/PKG-INFO` & `pylinweb-1.9.5/pylinweb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylinweb
-Version: 1.9.4
+Version: 1.9.5
 Summary: A simple functional test library using Python and Selenium
 Author: Linda Lopez
 Keywords: selenium,testing,web,chrome
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,19 +14,22 @@
 Requires-Dist: behave==1.2.6
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
 Requires-Dist: playwright==1.42.0
 Requires-Dist: psutil==5.9.2
+Requires-Dist: pillow==10.3.0
+Requires-Dist: openpyxl==3.1.2
+Requires-Dist: customtkinter==5.2.2
 Requires-Dist: PyPDF2==3.0.1
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: pycparser==2.21
 Requires-Dist: screeninfo==0.8
-Requires-Dist: selenium==4.12
+Requires-Dist: selenium==4.20.0
 Requires-Dist: keyboard==0.13.5
 
 # Pylinweb
 
 Pylinweb es una biblioteca de pruebas funcionales simple que utiliza Python, Selenium y Chrome driver.
 
 ## Pre-requisitos
```

### Comparing `pylinweb-1.9.4/setup.py` & `pylinweb-1.9.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,22 @@
         "behave==1.2.6",
         "behave-html-formatter==0.9.10",
         "behave2cucumber==1.0.3",
         "docxcompose==1.4.0",
         "docxtpl==0.16.8",
         "playwright==1.42.0",
         "psutil==5.9.2",
+        "pillow==10.3.0",
+        "openpyxl==3.1.2",
+        "customtkinter==5.2.2",
         "PyPDF2==3.0.1",
         "python-docx==1.1.0",
         "pycparser==2.21",
         "screeninfo==0.8",
-        "selenium==4.12",
+        "selenium==4.20.0",
         "keyboard==0.13.5"
     ],
     entry_points={
         'console_scripts': [
             'pylinweb=pylinweb.main:main',
         ],
     },
```

