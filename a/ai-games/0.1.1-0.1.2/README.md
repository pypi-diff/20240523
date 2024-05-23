# Comparing `tmp/ai_games-0.1.1.tar.gz` & `tmp/ai_games-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_games-0.1.1.tar", last modified: Thu May 23 14:36:38 2024, max compression
+gzip compressed data, was "ai_games-0.1.2.tar", last modified: Thu May 23 14:38:43 2024, max compression
```

## Comparing `ai_games-0.1.1.tar` & `ai_games-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 14:36:38.720000 ai_games-0.1.1/
--rwx------   0 benjamin   (501) staff       (20)     1476 2024-05-23 14:36:38.760000 ai_games-0.1.1/PKG-INFO
--rwx------   0 benjamin   (501) staff       (20)     1191 2024-05-23 14:30:53.000000 ai_games-0.1.1/README.md
-drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 14:36:38.730000 ai_games-0.1.1/ai_games.egg-info/
--rwx------   0 benjamin   (501) staff       (20)     1476 2024-05-23 14:36:38.000000 ai_games-0.1.1/ai_games.egg-info/PKG-INFO
--rwx------   0 benjamin   (501) staff       (20)      177 2024-05-23 14:36:38.000000 ai_games-0.1.1/ai_games.egg-info/SOURCES.txt
--rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 14:36:38.000000 ai_games-0.1.1/ai_games.egg-info/dependency_links.txt
--rwx------   0 benjamin   (501) staff       (20)       13 2024-05-23 14:36:38.000000 ai_games-0.1.1/ai_games.egg-info/requires.txt
--rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 14:36:38.000000 ai_games-0.1.1/ai_games.egg-info/top_level.txt
--rwx------   0 benjamin   (501) staff       (20)       38 2024-05-23 14:36:38.770000 ai_games-0.1.1/setup.cfg
--rwx------   0 benjamin   (501) staff       (20)      573 2024-05-23 14:36:28.000000 ai_games-0.1.1/setup.py
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 14:38:43.550000 ai_games-0.1.2/
+-rwx------   0 benjamin   (501) staff       (20)     1651 2024-05-23 14:38:43.640000 ai_games-0.1.2/PKG-INFO
+-rwx------   0 benjamin   (501) staff       (20)     1191 2024-05-23 14:30:53.000000 ai_games-0.1.2/README.md
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 14:38:43.560000 ai_games-0.1.2/ai_games.egg-info/
+-rwx------   0 benjamin   (501) staff       (20)     1651 2024-05-23 14:38:43.000000 ai_games-0.1.2/ai_games.egg-info/PKG-INFO
+-rwx------   0 benjamin   (501) staff       (20)      177 2024-05-23 14:38:43.000000 ai_games-0.1.2/ai_games.egg-info/SOURCES.txt
+-rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 14:38:43.000000 ai_games-0.1.2/ai_games.egg-info/dependency_links.txt
+-rwx------   0 benjamin   (501) staff       (20)       13 2024-05-23 14:38:43.000000 ai_games-0.1.2/ai_games.egg-info/requires.txt
+-rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 14:38:43.000000 ai_games-0.1.2/ai_games.egg-info/top_level.txt
+-rwx------   0 benjamin   (501) staff       (20)       38 2024-05-23 14:38:43.640000 ai_games-0.1.2/setup.cfg
+-rwx------   0 benjamin   (501) staff       (20)      775 2024-05-23 14:38:01.000000 ai_games-0.1.2/setup.py
```

### Comparing `ai_games-0.1.1/PKG-INFO` & `ai_games-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: ai_games
-Version: 0.1.1
+Version: 0.1.2
 Summary: AI Games: Collection of interactive games with AI opponents for Python.
 Home-page: https://github.com/bzm10/ai_games
 Author: Coding with BM
+Author-email: your@email.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pygame
 
 # AI Games
 
 Welcome to AI Games, a Python package featuring various games with AI opponents.
```

### Comparing `ai_games-0.1.1/README.md` & `ai_games-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ai_games-0.1.1/ai_games.egg-info/PKG-INFO` & `ai_games-0.1.2/ai_games.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: ai_games
-Version: 0.1.1
+Version: 0.1.2
 Summary: AI Games: Collection of interactive games with AI opponents for Python.
 Home-page: https://github.com/bzm10/ai_games
 Author: Coding with BM
+Author-email: your@email.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pygame
 
 # AI Games
 
 Welcome to AI Games, a Python package featuring various games with AI opponents.
```

### Comparing `ai_games-0.1.1/setup.py` & `ai_games-0.1.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,20 +2,25 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='ai_games',
-    version='0.1.1',
+    version='0.1.2',
     author='Coding with BM',
+    author_email='your@email.com',
     description='AI Games: Collection of interactive games with AI opponents for Python.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/bzm10/ai_games',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pygame'
     ],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
 )
-
```

