# Comparing `tmp/ai_games-0.1.tar.gz` & `tmp/ai_games-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_games-0.1.tar", last modified: Thu May 23 14:34:11 2024, max compression
+gzip compressed data, was "ai_games-0.1.1.tar", last modified: Thu May 23 14:36:38 2024, max compression
```

## Comparing `ai_games-0.1.tar` & `ai_games-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 14:34:11.720000 ai_games-0.1/
--rwx------   0 benjamin   (501) staff       (20)     1425 2024-05-23 14:34:11.830000 ai_games-0.1/PKG-INFO
--rwx------   0 benjamin   (501) staff       (20)     1191 2024-05-23 14:30:53.000000 ai_games-0.1/README.md
-drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 14:34:11.730000 ai_games-0.1/ai_games.egg-info/
--rwx------   0 benjamin   (501) staff       (20)     1425 2024-05-23 14:34:11.000000 ai_games-0.1/ai_games.egg-info/PKG-INFO
--rwx------   0 benjamin   (501) staff       (20)      177 2024-05-23 14:34:11.000000 ai_games-0.1/ai_games.egg-info/SOURCES.txt
--rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 14:34:11.000000 ai_games-0.1/ai_games.egg-info/dependency_links.txt
--rwx------   0 benjamin   (501) staff       (20)       13 2024-05-23 14:34:11.000000 ai_games-0.1/ai_games.egg-info/requires.txt
--rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 14:34:11.000000 ai_games-0.1/ai_games.egg-info/top_level.txt
--rwx------   0 benjamin   (501) staff       (20)       38 2024-05-23 14:34:11.830000 ai_games-0.1/setup.cfg
--rwx------   0 benjamin   (501) staff       (20)      522 2024-05-23 14:20:30.000000 ai_games-0.1/setup.py
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 14:36:38.720000 ai_games-0.1.1/
+-rwx------   0 benjamin   (501) staff       (20)     1476 2024-05-23 14:36:38.760000 ai_games-0.1.1/PKG-INFO
+-rwx------   0 benjamin   (501) staff       (20)     1191 2024-05-23 14:30:53.000000 ai_games-0.1.1/README.md
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 14:36:38.730000 ai_games-0.1.1/ai_games.egg-info/
+-rwx------   0 benjamin   (501) staff       (20)     1476 2024-05-23 14:36:38.000000 ai_games-0.1.1/ai_games.egg-info/PKG-INFO
+-rwx------   0 benjamin   (501) staff       (20)      177 2024-05-23 14:36:38.000000 ai_games-0.1.1/ai_games.egg-info/SOURCES.txt
+-rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 14:36:38.000000 ai_games-0.1.1/ai_games.egg-info/dependency_links.txt
+-rwx------   0 benjamin   (501) staff       (20)       13 2024-05-23 14:36:38.000000 ai_games-0.1.1/ai_games.egg-info/requires.txt
+-rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 14:36:38.000000 ai_games-0.1.1/ai_games.egg-info/top_level.txt
+-rwx------   0 benjamin   (501) staff       (20)       38 2024-05-23 14:36:38.770000 ai_games-0.1.1/setup.cfg
+-rwx------   0 benjamin   (501) staff       (20)      573 2024-05-23 14:36:28.000000 ai_games-0.1.1/setup.py
```

### Comparing `ai_games-0.1/PKG-INFO` & `ai_games-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ai_games
-Version: 0.1
-Summary: Description of your package
+Version: 0.1.1
+Summary: AI Games: Collection of interactive games with AI opponents for Python.
 Home-page: https://github.com/bzm10/ai_games
-Author: Your Name
+Author: Coding with BM
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pygame
 
 # AI Games
 
 Welcome to AI Games, a Python package featuring various games with AI opponents.
```

### Comparing `ai_games-0.1/README.md` & `ai_games-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ai_games-0.1/ai_games.egg-info/PKG-INFO` & `ai_games-0.1.1/ai_games.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ai_games
-Version: 0.1
-Summary: Description of your package
+Version: 0.1.1
+Summary: AI Games: Collection of interactive games with AI opponents for Python.
 Home-page: https://github.com/bzm10/ai_games
-Author: Your Name
+Author: Coding with BM
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pygame
 
 # AI Games
 
 Welcome to AI Games, a Python package featuring various games with AI opponents.
```

### Comparing `ai_games-0.1/setup.py` & `ai_games-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='ai_games',
-    version='0.1',
-    author='Your Name',
-    description='Description of your package',
+    version='0.1.1',
+    author='Coding with BM',
+    description='AI Games: Collection of interactive games with AI opponents for Python.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/bzm10/ai_games',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pygame'
```

