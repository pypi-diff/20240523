# Comparing `tmp/mibanco_auto_web-1.0.1.tar.gz` & `tmp/mibanco_auto_web-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mibanco_auto_web-1.0.1.tar", last modified: Wed May  8 21:22:17 2024, max compression
+gzip compressed data, was "mibanco_auto_web-1.0.2.tar", last modified: Thu May 23 16:43:08 2024, max compression
```

## Comparing `mibanco_auto_web-1.0.1.tar` & `mibanco_auto_web-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 21:22:17.014733 mibanco_auto_web-1.0.1/
--rw-rw-rw-   0        0        0       46 2024-04-30 04:05:30.000000 mibanco_auto_web-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3256 2024-05-08 21:22:17.008476 mibanco_auto_web-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2231 2024-05-06 17:12:14.000000 mibanco_auto_web-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 21:22:16.906823 mibanco_auto_web-1.0.1/mibanco_auto_web/
--rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 mibanco_auto_web-1.0.1/mibanco_auto_web/__init__.py
--rw-rw-rw-   0        0        0     4346 2024-05-08 21:17:28.000000 mibanco_auto_web-1.0.1/mibanco_auto_web/functions.py
--rw-rw-rw-   0        0        0     1686 2024-05-02 20:47:00.000000 mibanco_auto_web-1.0.1/mibanco_auto_web/main.py
--rw-rw-rw-   0        0        0      102 2024-05-08 21:16:35.000000 mibanco_auto_web-1.0.1/mibanco_auto_web/variables.py
-drwxrwxrwx   0        0        0        0 2024-05-08 21:22:17.003342 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/
--rw-rw-rw-   0        0        0     3256 2024-05-08 21:22:15.000000 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-05-08 21:22:15.000000 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 21:22:15.000000 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-08 21:22:15.000000 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      322 2024-05-08 21:22:15.000000 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-08 21:22:15.000000 mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 21:22:17.014733 mibanco_auto_web-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1563 2024-05-08 21:16:24.000000 mibanco_auto_web-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:43:08.875437 mibanco_auto_web-1.0.2/
+-rw-rw-rw-   0        0        0       46 2024-05-21 20:44:35.000000 mibanco_auto_web-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3439 2024-05-23 16:43:08.875437 mibanco_auto_web-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2364 2024-05-23 16:28:02.000000 mibanco_auto_web-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 16:43:08.867915 mibanco_auto_web-1.0.2/mibanco_auto_web/
+-rw-rw-rw-   0        0        0       63 2024-05-21 20:44:35.000000 mibanco_auto_web-1.0.2/mibanco_auto_web/__init__.py
+-rw-rw-rw-   0        0        0     4936 2024-05-23 16:33:38.000000 mibanco_auto_web-1.0.2/mibanco_auto_web/functions.py
+-rw-rw-rw-   0        0        0     1798 2024-05-23 16:22:52.000000 mibanco_auto_web-1.0.2/mibanco_auto_web/main.py
+-rw-rw-rw-   0        0        0      102 2024-05-23 16:43:00.000000 mibanco_auto_web-1.0.2/mibanco_auto_web/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:43:08.875437 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/
+-rw-rw-rw-   0        0        0     3439 2024-05-23 16:43:08.000000 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2024-05-23 16:43:08.000000 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:43:08.000000 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-23 16:43:08.000000 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      338 2024-05-23 16:43:08.000000 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-23 16:43:08.000000 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 16:43:08.875437 mibanco_auto_web-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1609 2024-05-21 20:47:45.000000 mibanco_auto_web-1.0.2/setup.py
```

### Comparing `mibanco_auto_web-1.0.1/PKG-INFO` & `mibanco_auto_web-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mibanco_auto_web
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple functional test library using Python and Selenium
-Author: Linda Lopez
+Author: Automation & Performance Team
 Keywords: selenium,testing,web,chrome
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: allure-behave==2.13.5
@@ -15,14 +15,15 @@
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
 Requires-Dist: playwright==1.42.0
 Requires-Dist: psutil==5.9.2
 Requires-Dist: pillow==10.3.0
+Requires-Dist: openpyxl==3.1.2
 Requires-Dist: customtkinter==5.2.2
 Requires-Dist: PyPDF2==3.0.1
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: pycparser==2.21
 Requires-Dist: screeninfo==0.8
 Requires-Dist: selenium==4.20.0
 Requires-Dist: keyboard==0.13.5
@@ -60,15 +61,17 @@
 |-------------|-------------------------------------------------------|
 | --version   | Imprime la versión de mibanco_auto_web.                       |
 | --setup     | Copia el directorio de la aplicación e instala las dependencias. |
 | --run-tests | Ejecuta las pruebas.                                  |
 | --report-html    | Genera un informe en html.                                    |
 | --report-word      | Genera un informe en formato word. |
 | --reset      | Elimina directorios innecesarios.  |
-| --open-app   | Ejecuta y abre la aplicación del framework  |
+| --open-app   | Abre la interfaz de ejecución de pruebas.  |
+| --open-logs   | Abre archivo excel con los logs de ejecución. |
+| --modify-data   | Abre archivo excel con la data de pruebas. |
 | --help  -h    | Muestra la ayuda y explica cómo usar los argumentos.  |
 
 Por ejemplo, para imprimir la versión de mibanco_auto_web, puedes usar:
 
 ```bash
 mibanco_auto_web --version
 ```
```

### Comparing `mibanco_auto_web-1.0.1/README.md` & `mibanco_auto_web-1.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 |-------------|-------------------------------------------------------|
 | --version   | Imprime la versión de mibanco_auto_web.                       |
 | --setup     | Copia el directorio de la aplicación e instala las dependencias. |
 | --run-tests | Ejecuta las pruebas.                                  |
 | --report-html    | Genera un informe en html.                                    |
 | --report-word      | Genera un informe en formato word. |
 | --reset      | Elimina directorios innecesarios.  |
-| --open-app   | Ejecuta y abre la aplicación del framework  |
+| --open-app   | Abre la interfaz de ejecución de pruebas.  |
+| --open-logs   | Abre archivo excel con los logs de ejecución. |
+| --modify-data   | Abre archivo excel con la data de pruebas. |
 | --help  -h    | Muestra la ayuda y explica cómo usar los argumentos.  |
 
 Por ejemplo, para imprimir la versión de mibanco_auto_web, puedes usar:
 
 ```bash
 mibanco_auto_web --version
 ```
```

### Comparing `mibanco_auto_web-1.0.1/mibanco_auto_web/functions.py` & `mibanco_auto_web-1.0.2/mibanco_auto_web/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,23 +24,28 @@
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
-    subprocess.run('python ./src/test/config/generate_word_web.py', shell=True)
+    current_path = os.getcwd()
+    evidencias_path = os.path.join(current_path,'Evidencias')
+    if os.path.exists(evidencias_path):
+        os.startfile(evidencias_path)
+    else:       
+        print("¡Debe realizar una ejecución de pruebas para generar el reporte Word!")
 
 def reset_files():
     folders = ["allure-report", "allure-results", "screenshots", "Evidencias"]
     current_dir = os.getcwd()
 
     for folder in folders:
         folder_path = os.path.join(current_dir, folder)
@@ -102,8 +107,19 @@
     return repository_name
 
 def select_brach_name():
     branch_name = input('Escribe el nombre de la rama (La rama debe existir en el repositorio): ')
     return branch_name
 
 def open_application():
-    subprocess.run('python ./src/test/config/app_run.py', shell=True)
+    subprocess.run('python ./src/test/app/app.py', shell=True)
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
```

### Comparing `mibanco_auto_web-1.0.1/mibanco_auto_web/main.py` & `mibanco_auto_web-1.0.2/mibanco_auto_web/main.py`

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

### Comparing `mibanco_auto_web-1.0.1/mibanco_auto_web.egg-info/PKG-INFO` & `mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mibanco_auto_web
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple functional test library using Python and Selenium
-Author: Linda Lopez
+Author: Automation & Performance Team
 Keywords: selenium,testing,web,chrome
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: allure-behave==2.13.5
@@ -15,14 +15,15 @@
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
 Requires-Dist: playwright==1.42.0
 Requires-Dist: psutil==5.9.2
 Requires-Dist: pillow==10.3.0
+Requires-Dist: openpyxl==3.1.2
 Requires-Dist: customtkinter==5.2.2
 Requires-Dist: PyPDF2==3.0.1
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: pycparser==2.21
 Requires-Dist: screeninfo==0.8
 Requires-Dist: selenium==4.20.0
 Requires-Dist: keyboard==0.13.5
@@ -60,15 +61,17 @@
 |-------------|-------------------------------------------------------|
 | --version   | Imprime la versión de mibanco_auto_web.                       |
 | --setup     | Copia el directorio de la aplicación e instala las dependencias. |
 | --run-tests | Ejecuta las pruebas.                                  |
 | --report-html    | Genera un informe en html.                                    |
 | --report-word      | Genera un informe en formato word. |
 | --reset      | Elimina directorios innecesarios.  |
-| --open-app   | Ejecuta y abre la aplicación del framework  |
+| --open-app   | Abre la interfaz de ejecución de pruebas.  |
+| --open-logs   | Abre archivo excel con los logs de ejecución. |
+| --modify-data   | Abre archivo excel con la data de pruebas. |
 | --help  -h    | Muestra la ayuda y explica cómo usar los argumentos.  |
 
 Por ejemplo, para imprimir la versión de mibanco_auto_web, puedes usar:
 
 ```bash
 mibanco_auto_web --version
 ```
```

### Comparing `mibanco_auto_web-1.0.1/setup.py` & `mibanco_auto_web-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mibanco_auto_web',
     version= version,
     description='A simple functional test library using Python and Selenium',
-    author='Linda Lopez',
+    author='Automation & Performance Team',
     packages=find_packages(),
     include_package_data=True, #Esto hace que setuptools lea el archivo MANIFEST.in
     install_requires=[
         "allure-behave==2.13.5",
         "allure-python-commons==2.13.5",
         "behave==1.2.6",
         "behave-html-formatter==0.9.10",
         "behave2cucumber==1.0.3",
         "docxcompose==1.4.0",
         "docxtpl==0.16.8",
         "playwright==1.42.0",
         "psutil==5.9.2",
         "pillow==10.3.0",
+        "openpyxl==3.1.2",
         "customtkinter==5.2.2",
         "PyPDF2==3.0.1",
         "python-docx==1.1.0",
         "pycparser==2.21",
         "screeninfo==0.8",
         "selenium==4.20.0",
         "keyboard==0.13.5"
```

