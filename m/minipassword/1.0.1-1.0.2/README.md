# Comparing `tmp/minipassword-1.0.1.tar.gz` & `tmp/minipassword-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minipassword-1.0.1.tar", last modified: Wed May 15 07:05:23 2024, max compression
+gzip compressed data, was "minipassword-1.0.2.tar", last modified: Thu May 23 06:26:55 2024, max compression
```

## Comparing `minipassword-1.0.1.tar` & `minipassword-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-15 07:05:23.782304 minipassword-1.0.1/
--rw-r--r--   0 Alan       (501) staff       (20)     1063 2024-04-18 07:30:55.000000 minipassword-1.0.1/LICENSE
--rw-r--r--   0 Alan       (501) staff       (20)     4493 2024-05-15 07:05:23.782111 minipassword-1.0.1/PKG-INFO
--rw-r--r--   0 Alan       (501) staff       (20)     3871 2024-05-13 06:18:57.000000 minipassword-1.0.1/README.md
--rw-r--r--   0 Alan       (501) staff       (20)       84 2022-04-22 08:08:10.000000 minipassword-1.0.1/pyproject.toml
--rw-r--r--   0 Alan       (501) staff       (20)       38 2024-05-15 07:05:23.782361 minipassword-1.0.1/setup.cfg
--rw-r--r--   0 Alan       (501) staff       (20)     1004 2024-05-15 06:59:16.000000 minipassword-1.0.1/setup.py
-drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-15 07:05:23.779612 minipassword-1.0.1/src/
-drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-15 07:05:23.780509 minipassword-1.0.1/src/minipassword/
--rw-r--r--   0 Alan       (501) staff       (20)        0 2024-05-10 03:57:36.000000 minipassword-1.0.1/src/minipassword/__init__.py
--rw-r--r--   0 Alan       (501) staff       (20)     7004 2024-05-13 04:10:22.000000 minipassword-1.0.1/src/minipassword/box.py
--rw-r--r--   0 Alan       (501) staff       (20)    12705 2024-05-15 06:57:19.000000 minipassword-1.0.1/src/minipassword/commands.py
-drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-15 07:05:23.781895 minipassword-1.0.1/src/minipassword.egg-info/
--rw-r--r--   0 Alan       (501) staff       (20)     4493 2024-05-15 07:05:23.000000 minipassword-1.0.1/src/minipassword.egg-info/PKG-INFO
--rw-r--r--   0 Alan       (501) staff       (20)      420 2024-05-15 07:05:23.000000 minipassword-1.0.1/src/minipassword.egg-info/SOURCES.txt
--rw-r--r--   0 Alan       (501) staff       (20)        1 2024-05-15 07:05:23.000000 minipassword-1.0.1/src/minipassword.egg-info/dependency_links.txt
--rw-r--r--   0 Alan       (501) staff       (20)       62 2024-05-15 07:05:23.000000 minipassword-1.0.1/src/minipassword.egg-info/requires.txt
--rw-r--r--   0 Alan       (501) staff       (20)       13 2024-05-15 07:05:23.000000 minipassword-1.0.1/src/minipassword.egg-info/top_level.txt
--rw-r--r--   0 Alan       (501) staff       (20)        1 2024-05-10 04:26:04.000000 minipassword-1.0.1/src/minipassword.egg-info/zip-safe
-drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-15 07:05:23.781707 minipassword-1.0.1/tests/
--rw-r--r--   0 Alan       (501) staff       (20)      538 2024-05-10 06:27:51.000000 minipassword-1.0.1/tests/test_conf.py
--rw-r--r--   0 Alan       (501) staff       (20)     1722 2024-05-10 07:07:49.000000 minipassword-1.0.1/tests/test_manager.py
--rw-r--r--   0 Alan       (501) staff       (20)      114 2024-05-10 07:34:17.000000 minipassword-1.0.1/tests/testcommands.py
+drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-23 06:26:55.174933 minipassword-1.0.2/
+-rw-r--r--   0 Alan       (501) staff       (20)     1063 2024-04-18 07:30:55.000000 minipassword-1.0.2/LICENSE
+-rw-r--r--   0 Alan       (501) staff       (20)     4493 2024-05-23 06:26:55.174701 minipassword-1.0.2/PKG-INFO
+-rw-r--r--   0 Alan       (501) staff       (20)     3871 2024-05-13 06:18:57.000000 minipassword-1.0.2/README.md
+-rw-r--r--   0 Alan       (501) staff       (20)       84 2022-04-22 08:08:10.000000 minipassword-1.0.2/pyproject.toml
+-rw-r--r--   0 Alan       (501) staff       (20)       38 2024-05-23 06:26:55.174977 minipassword-1.0.2/setup.cfg
+-rw-r--r--   0 Alan       (501) staff       (20)     1004 2024-05-23 06:20:46.000000 minipassword-1.0.2/setup.py
+drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-23 06:26:55.171134 minipassword-1.0.2/src/
+drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-23 06:26:55.172441 minipassword-1.0.2/src/minipassword/
+-rw-r--r--   0 Alan       (501) staff       (20)        0 2024-05-10 03:57:36.000000 minipassword-1.0.2/src/minipassword/__init__.py
+-rw-r--r--   0 Alan       (501) staff       (20)     7004 2024-05-13 04:10:22.000000 minipassword-1.0.2/src/minipassword/box.py
+-rw-r--r--   0 Alan       (501) staff       (20)    12710 2024-05-23 06:22:14.000000 minipassword-1.0.2/src/minipassword/commands.py
+drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-23 06:26:55.174452 minipassword-1.0.2/src/minipassword.egg-info/
+-rw-r--r--   0 Alan       (501) staff       (20)     4493 2024-05-23 06:26:55.000000 minipassword-1.0.2/src/minipassword.egg-info/PKG-INFO
+-rw-r--r--   0 Alan       (501) staff       (20)      420 2024-05-23 06:26:55.000000 minipassword-1.0.2/src/minipassword.egg-info/SOURCES.txt
+-rw-r--r--   0 Alan       (501) staff       (20)        1 2024-05-23 06:26:55.000000 minipassword-1.0.2/src/minipassword.egg-info/dependency_links.txt
+-rw-r--r--   0 Alan       (501) staff       (20)       62 2024-05-23 06:26:55.000000 minipassword-1.0.2/src/minipassword.egg-info/requires.txt
+-rw-r--r--   0 Alan       (501) staff       (20)       13 2024-05-23 06:26:55.000000 minipassword-1.0.2/src/minipassword.egg-info/top_level.txt
+-rw-r--r--   0 Alan       (501) staff       (20)        1 2024-05-10 04:26:04.000000 minipassword-1.0.2/src/minipassword.egg-info/zip-safe
+drwxr-xr-x   0 Alan       (501) staff       (20)        0 2024-05-23 06:26:55.174126 minipassword-1.0.2/tests/
+-rw-r--r--   0 Alan       (501) staff       (20)      538 2024-05-10 06:27:51.000000 minipassword-1.0.2/tests/test_conf.py
+-rw-r--r--   0 Alan       (501) staff       (20)     1722 2024-05-10 07:07:49.000000 minipassword-1.0.2/tests/test_manager.py
+-rw-r--r--   0 Alan       (501) staff       (20)      114 2024-05-10 07:34:17.000000 minipassword-1.0.2/tests/testcommands.py
```

### Comparing `minipassword-1.0.1/LICENSE` & `minipassword-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `minipassword-1.0.1/PKG-INFO` & `minipassword-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minipassword
-Version: 1.0.1
+Version: 1.0.2
 Summary: Mini Password is a command-line password manager.
 Home-page: https://github.com/laonan/minipassword
 Author: Laonan
 Author-email: hello@laonan.net
 Project-URL: Bug Tracker, https://github.com/laonan/minipassword/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `minipassword-1.0.1/README.md` & `minipassword-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `minipassword-1.0.1/setup.py` & `minipassword-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="minipassword",
-    version="1.0.1",
+    version="1.0.2",
     author="Laonan",
     author_email="hello@laonan.net",
     description="Mini Password is a command-line password manager.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/laonan/minipassword",  # github url
     project_urls={
```

### Comparing `minipassword-1.0.1/src/minipassword/box.py` & `minipassword-1.0.2/src/minipassword/box.py`

 * *Files identical despite different names*

### Comparing `minipassword-1.0.1/src/minipassword/commands.py` & `minipassword-1.0.2/src/minipassword/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,16 @@
             else:
                 if self.password_manager.get_password_by_name(name) and name != password_obj[1]:
                     print(f'Password already exists! (name is {name})')
                     return
             original_login_name = self.password_manager.aes_decrypt(password_obj[2])
             login_name = input(f'Enter the login name ({original_login_name}): ')
             if login_name == '':
-                login_name = password_obj[2]
+                login_name = original_login_name
+
             password = input('Enter the password: ')
             if password == '':
                 password = self.password_manager.aes_decrypt(password_obj[3])
             memo = input(f'\n\n({password_obj[4]})\n\nEnter the memo: ')
             if memo == '':
                 memo = password_obj[4]
             url = input(f'Enter the url ({password_obj[5]}): ')
```

### Comparing `minipassword-1.0.1/src/minipassword.egg-info/PKG-INFO` & `minipassword-1.0.2/src/minipassword.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minipassword
-Version: 1.0.1
+Version: 1.0.2
 Summary: Mini Password is a command-line password manager.
 Home-page: https://github.com/laonan/minipassword
 Author: Laonan
 Author-email: hello@laonan.net
 Project-URL: Bug Tracker, https://github.com/laonan/minipassword/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `minipassword-1.0.1/tests/test_conf.py` & `minipassword-1.0.2/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `minipassword-1.0.1/tests/test_manager.py` & `minipassword-1.0.2/tests/test_manager.py`

 * *Files identical despite different names*

