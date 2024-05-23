# Comparing `tmp/mask_key-0.2.8.tar.gz` & `tmp/mask_key-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask_key-0.2.8.tar", last modified: Thu May 23 07:05:07 2024, max compression
+gzip compressed data, was "mask_key-0.3.1.tar", last modified: Thu May 23 08:25:42 2024, max compression
```

## Comparing `mask_key-0.2.8.tar` & `mask_key-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 07:05:07.707563 mask_key-0.2.8/
--rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.2.8/LICENSE
--rw-rw-rw-   0        0        0       34 2024-05-23 04:58:08.000000 mask_key-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0      473 2024-05-23 07:05:07.707563 mask_key-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 07:05:07.671009 mask_key-0.2.8/mask_key/
--rw-rw-rw-   0        0        0       47 2024-05-23 04:58:08.000000 mask_key-0.2.8/mask_key/__init__.py
--rw-rw-rw-   0        0        0      373 2024-05-23 06:17:22.000000 mask_key-0.2.8/mask_key/api.py
--rw-rw-rw-   0        0        0     1237 2024-05-23 06:51:24.000000 mask_key-0.2.8/mask_key/main.py
--rw-rw-rw-   0        0        0       73 2024-05-23 06:18:02.000000 mask_key-0.2.8/mask_key/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:05:07.705570 mask_key-0.2.8/mask_key.egg-info/
--rw-rw-rw-   0        0        0      473 2024-05-23 07:05:07.000000 mask_key-0.2.8/mask_key.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-05-23 07:05:07.000000 mask_key-0.2.8/mask_key.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 07:05:07.000000 mask_key-0.2.8/mask_key.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-23 07:05:07.000000 mask_key-0.2.8/mask_key.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2024-05-23 07:05:07.000000 mask_key-0.2.8/mask_key.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 07:05:07.000000 mask_key-0.2.8/mask_key.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 07:05:07.708563 mask_key-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1668 2024-05-23 07:05:02.000000 mask_key-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 08:25:42.230969 mask_key-0.3.1/
+-rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-05-23 04:58:08.000000 mask_key-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      473 2024-05-23 08:25:42.229955 mask_key-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 08:25:42.194847 mask_key-0.3.1/mask_key/
+-rw-rw-rw-   0        0        0       47 2024-05-23 04:58:08.000000 mask_key-0.3.1/mask_key/__init__.py
+-rw-rw-rw-   0        0        0      373 2024-05-23 06:17:22.000000 mask_key-0.3.1/mask_key/api.py
+-rw-rw-rw-   0        0        0     1237 2024-05-23 06:51:24.000000 mask_key-0.3.1/mask_key/main.py
+-rw-rw-rw-   0        0        0       73 2024-05-23 06:18:02.000000 mask_key-0.3.1/mask_key/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 08:25:42.222946 mask_key-0.3.1/mask_key.egg-info/
+-rw-rw-rw-   0        0        0      473 2024-05-23 08:25:42.000000 mask_key-0.3.1/mask_key.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-05-23 08:25:42.000000 mask_key-0.3.1/mask_key.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 08:25:42.000000 mask_key-0.3.1/mask_key.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-23 08:25:42.000000 mask_key-0.3.1/mask_key.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2024-05-23 08:25:42.000000 mask_key-0.3.1/mask_key.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 08:25:42.000000 mask_key-0.3.1/mask_key.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 08:25:42.230969 mask_key-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1651 2024-05-23 08:20:34.000000 mask_key-0.3.1/setup.py
```

### Comparing `mask_key-0.2.8/mask_key/main.py` & `mask_key-0.3.1/mask_key/main.py`

 * *Files identical despite different names*

### Comparing `mask_key-0.2.8/setup.py` & `mask_key-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import subprocess
 import sys
 
 class PostInstallCommand(install):
     def run(self):
-        install.run(self)
-        # Inform the user about the post-install script
-        print("Running post-installation script...")
+        install.run(self)  # Ensures that the install proceeds as normal
         try:
-            subprocess.run([sys.executable, '-m', 'mask_key.main'], check=True)
-        except subprocess.CalledProcessError as e:
-            print(f"Error during post install script execution: {e}")
-            print("Please run `mask-key` manually after installation to complete setup.")
-        except Exception as e:
-            print(f"Unexpected error during post install: {e}")
-            print("Please run `mask-key` manually after installation to complete setup.")
+            # Calling the main function directly if possible
+            # Make sure 'mask_key.main' has 'main' function accessible
+            from mask_key.main import main
+            main()
+        except ImportError as e:
+            # If the direct call isn't feasible, fall back to subprocess
+            try:
+                subprocess.run([sys.executable, '-m', 'mask_key.main'], check=True)
+            except subprocess.CalledProcessError as e:
+                print(f"Error running mask_key.main: {e}")
 
 setup(
     name='mask_key',
-    version='0.2.8',
+    version='0.3.1',
     author='krishna agarwal',
     author_email='krishnacool781@gmail.com',
     description='A Python package to generate mask keys.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/krishnaagarwal781/mask_keys_server',
     packages=find_packages(),
     install_requires=[
         'requests',
         'python-dotenv',
     ],
     entry_points={
         'console_scripts': [
-            'mask-key=mask_key.main:main',
+            'mask-key-setup=mask_key.main:main',
         ],
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
     cmdclass={
         'install': PostInstallCommand,
-    },
+    }
 )
```

