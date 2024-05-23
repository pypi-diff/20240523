# Comparing `tmp/ai_games-0.1.4.tar.gz` & `tmp/ai_games-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_games-0.1.4.tar", last modified: Thu May 23 16:09:02 2024, max compression
+gzip compressed data, was "ai_games-0.1.5.tar", last modified: Thu May 23 16:10:18 2024, max compression
```

## Comparing `ai_games-0.1.4.tar` & `ai_games-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 16:09:02.040000 ai_games-0.1.4/
--rwx------   0 benjamin   (501) staff       (20)     1601 2024-05-23 16:09:02.210000 ai_games-0.1.4/PKG-INFO
--rwx------   0 benjamin   (501) staff       (20)     1191 2024-05-23 14:30:53.000000 ai_games-0.1.4/README.md
-drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 16:09:02.050000 ai_games-0.1.4/ai_games/
--rwx------   0 benjamin   (501) staff       (20)       81 2024-05-23 15:07:56.000000 ai_games-0.1.4/ai_games/__init__.py
--rwx------   0 benjamin   (501) staff       (20)    11450 2024-05-23 16:08:04.000000 ai_games-0.1.4/ai_games/connect4.py
-drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 16:09:02.060000 ai_games-0.1.4/ai_games.egg-info/
--rwx------   0 benjamin   (501) staff       (20)     1601 2024-05-23 16:09:01.000000 ai_games-0.1.4/ai_games.egg-info/PKG-INFO
--rwx------   0 benjamin   (501) staff       (20)      219 2024-05-23 16:09:02.000000 ai_games-0.1.4/ai_games.egg-info/SOURCES.txt
--rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 16:09:01.000000 ai_games-0.1.4/ai_games.egg-info/dependency_links.txt
--rwx------   0 benjamin   (501) staff       (20)        7 2024-05-23 16:09:01.000000 ai_games-0.1.4/ai_games.egg-info/requires.txt
--rwx------   0 benjamin   (501) staff       (20)        9 2024-05-23 16:09:01.000000 ai_games-0.1.4/ai_games.egg-info/top_level.txt
--rwx------   0 benjamin   (501) staff       (20)       38 2024-05-23 16:09:02.210000 ai_games-0.1.4/setup.cfg
--rwx------   0 benjamin   (501) staff       (20)      723 2024-05-23 16:08:53.000000 ai_games-0.1.4/setup.py
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 16:10:18.150000 ai_games-0.1.5/
+-rwx------   0 benjamin   (501) staff       (20)     1573 2024-05-23 16:10:18.250000 ai_games-0.1.5/PKG-INFO
+-rwx------   0 benjamin   (501) staff       (20)     1163 2024-05-23 16:09:52.000000 ai_games-0.1.5/README.md
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 16:10:18.160000 ai_games-0.1.5/ai_games/
+-rwx------   0 benjamin   (501) staff       (20)       81 2024-05-23 15:07:56.000000 ai_games-0.1.5/ai_games/__init__.py
+-rwx------   0 benjamin   (501) staff       (20)    11450 2024-05-23 16:08:04.000000 ai_games-0.1.5/ai_games/connect4.py
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 16:10:18.160000 ai_games-0.1.5/ai_games.egg-info/
+-rwx------   0 benjamin   (501) staff       (20)     1573 2024-05-23 16:10:18.000000 ai_games-0.1.5/ai_games.egg-info/PKG-INFO
+-rwx------   0 benjamin   (501) staff       (20)      219 2024-05-23 16:10:18.000000 ai_games-0.1.5/ai_games.egg-info/SOURCES.txt
+-rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 16:10:18.000000 ai_games-0.1.5/ai_games.egg-info/dependency_links.txt
+-rwx------   0 benjamin   (501) staff       (20)        7 2024-05-23 16:10:18.000000 ai_games-0.1.5/ai_games.egg-info/requires.txt
+-rwx------   0 benjamin   (501) staff       (20)        9 2024-05-23 16:10:18.000000 ai_games-0.1.5/ai_games.egg-info/top_level.txt
+-rwx------   0 benjamin   (501) staff       (20)       38 2024-05-23 16:10:18.250000 ai_games-0.1.5/setup.cfg
+-rwx------   0 benjamin   (501) staff       (20)      723 2024-05-23 16:10:07.000000 ai_games-0.1.5/setup.py
```

### Comparing `ai_games-0.1.4/PKG-INFO` & `ai_games-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai_games
-Version: 0.1.4
+Version: 0.1.5
 Summary: AI Games: Collection of interactive games with AI opponents for Python.
 Home-page: https://github.com/bzm10/ai_games
 Author: Coding with BM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -27,15 +27,15 @@
 The Connect Four with AI game in this package is adapted from a tutorial on YouTube created by [Keith Galli](https://www.youtube.com/@KeithGalli). 
 
 
 ```python
 from connect4_ai import Connect4Game, Config
 
 # Custom configuration
-config = Config(row_count=6, column_count=7, player_piece=1, ai_piece=2)
+config = Config(row_count=6, column_count=7)
 
 # Initialize the game
 game = Connect4Game(config=config)
 
 # Start playing
 game.play()
 ```
```

### Comparing `ai_games-0.1.4/README.md` & `ai_games-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 The Connect Four with AI game in this package is adapted from a tutorial on YouTube created by [Keith Galli](https://www.youtube.com/@KeithGalli). 
 
 
 ```python
 from connect4_ai import Connect4Game, Config
 
 # Custom configuration
-config = Config(row_count=6, column_count=7, player_piece=1, ai_piece=2)
+config = Config(row_count=6, column_count=7)
 
 # Initialize the game
 game = Connect4Game(config=config)
 
 # Start playing
 game.play()
 ```
```

### Comparing `ai_games-0.1.4/ai_games/connect4.py` & `ai_games-0.1.5/ai_games/connect4.py`

 * *Files identical despite different names*

### Comparing `ai_games-0.1.4/ai_games.egg-info/PKG-INFO` & `ai_games-0.1.5/ai_games.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai_games
-Version: 0.1.4
+Version: 0.1.5
 Summary: AI Games: Collection of interactive games with AI opponents for Python.
 Home-page: https://github.com/bzm10/ai_games
 Author: Coding with BM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -27,15 +27,15 @@
 The Connect Four with AI game in this package is adapted from a tutorial on YouTube created by [Keith Galli](https://www.youtube.com/@KeithGalli). 
 
 
 ```python
 from connect4_ai import Connect4Game, Config
 
 # Custom configuration
-config = Config(row_count=6, column_count=7, player_piece=1, ai_piece=2)
+config = Config(row_count=6, column_count=7)
 
 # Initialize the game
 game = Connect4Game(config=config)
 
 # Start playing
 game.play()
 ```
```

### Comparing `ai_games-0.1.4/setup.py` & `ai_games-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='ai_games',
-    version='0.1.4',
+    version='0.1.5',
     author='Coding with BM',
     description='AI Games: Collection of interactive games with AI opponents for Python.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/bzm10/ai_games',
     packages=find_packages(),
     install_requires=[
```

