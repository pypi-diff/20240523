# Comparing `tmp/ai_games-0.1.2.tar.gz` & `tmp/ai_games-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_games-0.1.2.tar", last modified: Thu May 23 14:38:43 2024, max compression
+gzip compressed data, was "ai_games-0.1.3.tar", last modified: Thu May 23 15:31:46 2024, max compression
```

## Comparing `ai_games-0.1.2.tar` & `ai_games-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 14:38:43.550000 ai_games-0.1.2/
--rwx------   0 benjamin   (501) staff       (20)     1651 2024-05-23 14:38:43.640000 ai_games-0.1.2/PKG-INFO
--rwx------   0 benjamin   (501) staff       (20)     1191 2024-05-23 14:30:53.000000 ai_games-0.1.2/README.md
-drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 14:38:43.560000 ai_games-0.1.2/ai_games.egg-info/
--rwx------   0 benjamin   (501) staff       (20)     1651 2024-05-23 14:38:43.000000 ai_games-0.1.2/ai_games.egg-info/PKG-INFO
--rwx------   0 benjamin   (501) staff       (20)      177 2024-05-23 14:38:43.000000 ai_games-0.1.2/ai_games.egg-info/SOURCES.txt
--rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 14:38:43.000000 ai_games-0.1.2/ai_games.egg-info/dependency_links.txt
--rwx------   0 benjamin   (501) staff       (20)       13 2024-05-23 14:38:43.000000 ai_games-0.1.2/ai_games.egg-info/requires.txt
--rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 14:38:43.000000 ai_games-0.1.2/ai_games.egg-info/top_level.txt
--rwx------   0 benjamin   (501) staff       (20)       38 2024-05-23 14:38:43.640000 ai_games-0.1.2/setup.cfg
--rwx------   0 benjamin   (501) staff       (20)      775 2024-05-23 14:38:01.000000 ai_games-0.1.2/setup.py
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 15:31:46.230000 ai_games-0.1.3/
+-rwx------   0 benjamin   (501) staff       (20)     1601 2024-05-23 15:31:46.300000 ai_games-0.1.3/PKG-INFO
+-rwx------   0 benjamin   (501) staff       (20)     1191 2024-05-23 14:30:53.000000 ai_games-0.1.3/README.md
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 15:31:46.240000 ai_games-0.1.3/ai_games/
+-rwx------   0 benjamin   (501) staff       (20)       81 2024-05-23 15:07:56.000000 ai_games-0.1.3/ai_games/__init__.py
+-rwx------   0 benjamin   (501) staff       (20)    11161 2024-05-23 14:11:18.000000 ai_games-0.1.3/ai_games/connect4.py
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 15:31:46.240000 ai_games-0.1.3/ai_games.egg-info/
+-rwx------   0 benjamin   (501) staff       (20)     1601 2024-05-23 15:31:46.000000 ai_games-0.1.3/ai_games.egg-info/PKG-INFO
+-rwx------   0 benjamin   (501) staff       (20)      219 2024-05-23 15:31:46.000000 ai_games-0.1.3/ai_games.egg-info/SOURCES.txt
+-rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 15:31:46.000000 ai_games-0.1.3/ai_games.egg-info/dependency_links.txt
+-rwx------   0 benjamin   (501) staff       (20)        7 2024-05-23 15:31:46.000000 ai_games-0.1.3/ai_games.egg-info/requires.txt
+-rwx------   0 benjamin   (501) staff       (20)        9 2024-05-23 15:31:46.000000 ai_games-0.1.3/ai_games.egg-info/top_level.txt
+-rwx------   0 benjamin   (501) staff       (20)       38 2024-05-23 15:31:46.310000 ai_games-0.1.3/setup.cfg
+-rwx------   0 benjamin   (501) staff       (20)      723 2024-05-23 15:31:33.000000 ai_games-0.1.3/setup.py
```

### Comparing `ai_games-0.1.2/PKG-INFO` & `ai_games-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: ai_games
-Version: 0.1.2
+Version: 0.1.3
 Summary: AI Games: Collection of interactive games with AI opponents for Python.
 Home-page: https://github.com/bzm10/ai_games
 Author: Coding with BM
-Author-email: your@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: numpy
 Requires-Dist: pygame
 
 # AI Games
 
 Welcome to AI Games, a Python package featuring various games with AI opponents.
 
 ## Installation
```

### Comparing `ai_games-0.1.2/README.md` & `ai_games-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ai_games-0.1.2/ai_games.egg-info/PKG-INFO` & `ai_games-0.1.3/ai_games.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: ai_games
-Version: 0.1.2
+Version: 0.1.3
 Summary: AI Games: Collection of interactive games with AI opponents for Python.
 Home-page: https://github.com/bzm10/ai_games
 Author: Coding with BM
-Author-email: your@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: numpy
 Requires-Dist: pygame
 
 # AI Games
 
 Welcome to AI Games, a Python package featuring various games with AI opponents.
 
 ## Installation
```

### Comparing `ai_games-0.1.2/setup.py` & `ai_games-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='ai_games',
-    version='0.1.2',
+    version='0.1.3',
     author='Coding with BM',
-    author_email='your@email.com',
     description='AI Games: Collection of interactive games with AI opponents for Python.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/bzm10/ai_games',
     packages=find_packages(),
     install_requires=[
-        'numpy',
         'pygame'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

