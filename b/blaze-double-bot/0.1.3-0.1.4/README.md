# Comparing `tmp/blaze_double_bot-0.1.3.tar.gz` & `tmp/blaze_double_bot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze_double_bot-0.1.3.tar", last modified: Thu May 23 11:55:40 2024, max compression
+gzip compressed data, was "blaze_double_bot-0.1.4.tar", last modified: Thu May 23 12:07:04 2024, max compression
```

## Comparing `blaze_double_bot-0.1.3.tar` & `blaze_double_bot-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 11:55:40.670087 blaze_double_bot-0.1.3/
--rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3103 2024-05-23 11:55:40.670087 blaze_double_bot-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2596 2024-05-23 11:37:29.000000 blaze_double_bot-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 11:55:40.621775 blaze_double_bot-0.1.3/blaze_double_bot/
--rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.1.3/blaze_double_bot/__init__.py
--rw-rw-rw-   0        0        0     8981 2024-05-23 01:41:05.000000 blaze_double_bot-0.1.3/blaze_double_bot/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:55:40.670087 blaze_double_bot-0.1.3/blaze_double_bot.egg-info/
--rw-rw-rw-   0        0        0     3103 2024-05-23 11:55:40.000000 blaze_double_bot-0.1.3/blaze_double_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-23 11:55:40.000000 blaze_double_bot-0.1.3/blaze_double_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 11:55:40.000000 blaze_double_bot-0.1.3/blaze_double_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 11:55:40.000000 blaze_double_bot-0.1.3/blaze_double_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-23 11:55:40.000000 blaze_double_bot-0.1.3/blaze_double_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 11:55:40.670087 blaze_double_bot-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      618 2024-05-23 11:45:48.000000 blaze_double_bot-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:07:04.218964 blaze_double_bot-0.1.4/
+-rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3164 2024-05-23 12:07:04.213290 blaze_double_bot-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2657 2024-05-23 12:04:16.000000 blaze_double_bot-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 12:07:04.142916 blaze_double_bot-0.1.4/blaze_double_bot/
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.1.4/blaze_double_bot/__init__.py
+-rw-rw-rw-   0        0        0     8981 2024-05-23 01:41:05.000000 blaze_double_bot-0.1.4/blaze_double_bot/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:07:04.211546 blaze_double_bot-0.1.4/blaze_double_bot.egg-info/
+-rw-rw-rw-   0        0        0     3164 2024-05-23 12:07:03.000000 blaze_double_bot-0.1.4/blaze_double_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-23 12:07:03.000000 blaze_double_bot-0.1.4/blaze_double_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 12:07:03.000000 blaze_double_bot-0.1.4/blaze_double_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 12:07:03.000000 blaze_double_bot-0.1.4/blaze_double_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-23 12:07:03.000000 blaze_double_bot-0.1.4/blaze_double_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 12:07:04.220052 blaze_double_bot-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      618 2024-05-23 12:06:24.000000 blaze_double_bot-0.1.4/setup.py
```

### Comparing `blaze_double_bot-0.1.3/LICENSE` & `blaze_double_bot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.1.3/PKG-INFO` & `blaze_double_bot-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.1.3
+Version: 0.1.4
 Summary: This Python library automates the betting process on the Blaze Double
 Author: Rafael de Oliveira Ribeiro
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -58,15 +58,15 @@
 ```
 
 - **username**: Your username or email registered on Blaze Double.
 - **password**: Your password to access Blaze Double.
 - **bet_amount**: The amount of the bet to be placed in each round.
 - **stop_loss_ratio**: The multiplication factor of the initial balance indicating the loss limit. The bot will stop betting if the balance drops below this limit.
 - **stop_win_ratio**: The multiplication factor of the initial balance indicating the win limit. The bot will stop betting if the balance reaches or exceeds this limit.
-- **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.
+- **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.Lists must be the same length and have a maximum of 20 items.
 
 2. **Create a `blazeBot.py` file** with the following content:
 
 ```python
 
 from blaze_double_bot import BlazeDoubleBot
```

### Comparing `blaze_double_bot-0.1.3/README.md` & `blaze_double_bot-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ```
 
 - **username**: Your username or email registered on Blaze Double.
 - **password**: Your password to access Blaze Double.
 - **bet_amount**: The amount of the bet to be placed in each round.
 - **stop_loss_ratio**: The multiplication factor of the initial balance indicating the loss limit. The bot will stop betting if the balance drops below this limit.
 - **stop_win_ratio**: The multiplication factor of the initial balance indicating the win limit. The bot will stop betting if the balance reaches or exceeds this limit.
-- **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.
+- **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.Lists must be the same length and have a maximum of 20 items.
 
 2. **Create a `blazeBot.py` file** with the following content:
 
 ```python
 
 from blaze_double_bot import BlazeDoubleBot
```

### Comparing `blaze_double_bot-0.1.3/blaze_double_bot/bot.py` & `blaze_double_bot-0.1.4/blaze_double_bot/bot.py`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.1.3/blaze_double_bot.egg-info/PKG-INFO` & `blaze_double_bot-0.1.4/blaze_double_bot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.1.3
+Version: 0.1.4
 Summary: This Python library automates the betting process on the Blaze Double
 Author: Rafael de Oliveira Ribeiro
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -58,15 +58,15 @@
 ```
 
 - **username**: Your username or email registered on Blaze Double.
 - **password**: Your password to access Blaze Double.
 - **bet_amount**: The amount of the bet to be placed in each round.
 - **stop_loss_ratio**: The multiplication factor of the initial balance indicating the loss limit. The bot will stop betting if the balance drops below this limit.
 - **stop_win_ratio**: The multiplication factor of the initial balance indicating the win limit. The bot will stop betting if the balance reaches or exceeds this limit.
-- **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.
+- **strategies**: Pre-defined betting strategies with sequences of colors (black = "B", red = "R"). You can add as many strategies as you want here.Lists must be the same length and have a maximum of 20 items.
 
 2. **Create a `blazeBot.py` file** with the following content:
 
 ```python
 
 from blaze_double_bot import BlazeDoubleBot
```

### Comparing `blaze_double_bot-0.1.3/setup.py` & `blaze_double_bot-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as f:
           readme =f.read()
 
 setup(
     name='blaze_double_bot',
     licence='MIT License',
-    version='0.1.3',
+    version='0.1.4',
     author='Rafael de Oliveira Ribeiro',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='ror74559@gmail.com',
     keywords='blaze double bot',
     description='This Python library automates the betting process on the Blaze Double',
     packages=['blaze_double_bot'],
```

