# Comparing `tmp/projectreadme-0.1.tar.gz` & `tmp/projectreadme-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projectreadme-0.1.tar", last modified: Thu May 23 02:14:00 2024, max compression
+gzip compressed data, was "projectreadme-0.2.tar", last modified: Thu May 23 03:39:43 2024, max compression
```

## Comparing `projectreadme-0.1.tar` & `projectreadme-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 02:14:00.802428 projectreadme-0.1/
--rw-rw-rw-   0        0        0      556 2024-05-23 02:14:00.791770 projectreadme-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       21 2024-05-22 23:10:06.000000 projectreadme-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 02:14:00.786002 projectreadme-0.1/projectreadme.egg-info/
--rw-rw-rw-   0        0        0      556 2024-05-23 02:14:00.000000 projectreadme-0.1/projectreadme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-05-23 02:14:00.000000 projectreadme-0.1/projectreadme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 02:14:00.000000 projectreadme-0.1/projectreadme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-05-23 02:14:00.000000 projectreadme-0.1/projectreadme.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-05-23 02:14:00.000000 projectreadme-0.1/projectreadme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-23 02:14:00.000000 projectreadme-0.1/projectreadme.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 02:14:00.775940 projectreadme-0.1/projectreadmegenerator/
--rw-rw-rw-   0        0        0      155 2024-05-22 23:10:06.000000 projectreadme-0.1/projectreadmegenerator/__init__.py
--rw-rw-rw-   0        0        0     1062 2024-05-22 21:03:46.000000 projectreadme-0.1/projectreadmegenerator/customuserinput.py
--rw-rw-rw-   0        0        0     2064 2024-05-23 02:13:48.000000 projectreadme-0.1/projectreadmegenerator/generator.py
--rw-rw-rw-   0        0        0      547 2024-05-22 23:10:06.000000 projectreadme-0.1/projectreadmegenerator/storage.py
--rw-rw-rw-   0        0        0       42 2024-05-23 02:14:00.802428 projectreadme-0.1/setup.cfg
--rw-rw-rw-   0        0        0      904 2024-05-22 20:56:17.000000 projectreadme-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:39:43.725496 projectreadme-0.2/
+-rw-rw-rw-   0        0        0     2441 2024-05-23 03:39:43.716161 projectreadme-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1906 2024-05-23 02:23:25.000000 projectreadme-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 03:39:43.711498 projectreadme-0.2/projectreadme.egg-info/
+-rw-rw-rw-   0        0        0     2441 2024-05-23 03:39:43.000000 projectreadme-0.2/projectreadme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2024-05-23 03:39:43.000000 projectreadme-0.2/projectreadme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 03:39:43.000000 projectreadme-0.2/projectreadme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-05-23 03:39:43.000000 projectreadme-0.2/projectreadme.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-05-23 03:39:43.000000 projectreadme-0.2/projectreadme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-23 03:39:43.000000 projectreadme-0.2/projectreadme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 03:39:43.702491 projectreadme-0.2/projectreadmegenerator/
+-rw-rw-rw-   0        0        0      155 2024-05-22 23:10:06.000000 projectreadme-0.2/projectreadmegenerator/__init__.py
+-rw-rw-rw-   0        0        0     1062 2024-05-22 21:03:46.000000 projectreadme-0.2/projectreadmegenerator/customuserinput.py
+-rw-rw-rw-   0        0        0     2111 2024-05-23 03:31:28.000000 projectreadme-0.2/projectreadmegenerator/generator.py
+-rw-rw-rw-   0        0        0      985 2024-05-23 03:37:01.000000 projectreadme-0.2/projectreadmegenerator/storage.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 03:39:43.725496 projectreadme-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      923 2024-05-23 02:34:36.000000 projectreadme-0.2/setup.py
```

### Comparing `projectreadme-0.1/projectreadmegenerator/customuserinput.py` & `projectreadme-0.2/projectreadmegenerator/customuserinput.py`

 * *Files identical despite different names*

### Comparing `projectreadme-0.1/projectreadmegenerator/generator.py` & `projectreadme-0.2/projectreadmegenerator/generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from dotenv import load_dotenv
 
 class generate:
     def generatereadmefile():
         STORAGE = Storage
         CUSTOMER_INPUT = custominput
 
-        load_dotenv()
-
+        load_dotenv(dotenv_path=STORAGE.env_module_loader())
+        
         API_KEY = os.getenv("API_KEY")
         MODEL_USING = os.getenv("MODEL")
 
         if not API_KEY or not MODEL_USING:
             print('Value not provided')
             API_KEY = API_KEY or CUSTOMER_INPUT.askfortheapikey().strip().replace(' ', '')
             MODEL_USING = MODEL_USING or CUSTOMER_INPUT.askforthemodel().strip().replace(' ', '')
```

### Comparing `projectreadme-0.1/projectreadmegenerator/storage.py` & `projectreadme-0.2/projectreadmegenerator/storage.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,8 +7,21 @@
     """
     @staticmethod 
     def storetheapikey(api_key , project_model):
         content = f'API_KEY = {api_key} \nMODEL = {project_model}'
         env_file_path = os.path.join(os.getcwd(), '.env')   
         with open(env_file_path, 'w') as envfile:
             envfile.write(content)
-            
+    
+        """
+        If the environment file is stored (.env), the function loads that env file corresponding 
+        to the working directory 
+
+        Returns:
+            DOTENV_PATH: Returns the path for environment file under the working directory 
+        """
+    
+    @staticmethod
+    def env_module_loader() -> str:
+        working_path = os.getcwd()
+        dotenv_path = f'{working_path}\\.env'
+        return dotenv_path
```

### Comparing `projectreadme-0.1/setup.py` & `projectreadme-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='projectreadme',
-    version='0.1',
+    version='0.2',
     packages= find_packages(),
     install_requires=[
         'google-generativeai',
         'python-dotenv',
     ],
     entry_points={
         'console_scripts': [
             'generate-readme = projectreadmegenerator.generator:generatereadmefile'
         ]
     },
     author='Anmol Dhiman',
     author_email='anmoldhimand666@gmail.com',
     description='A package for generating Project README files for a github project',
-    long_description= open('README.md').read(),
+    long_description= open('README.md', encoding= "utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Anmol-STRS/projectreadmegenerator',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

