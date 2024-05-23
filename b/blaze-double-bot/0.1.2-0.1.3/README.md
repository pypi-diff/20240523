# Comparing `tmp/blaze_double_bot-0.1.2.tar.gz` & `tmp/blaze_double_bot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze_double_bot-0.1.2.tar", last modified: Thu May 23 01:43:07 2024, max compression
+gzip compressed data, was "blaze_double_bot-0.1.3.tar", last modified: Thu May 23 11:55:40 2024, max compression
```

## Comparing `blaze_double_bot-0.1.2.tar` & `blaze_double_bot-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 01:43:07.128605 blaze_double_bot-0.1.2/
--rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3037 2024-05-23 01:43:07.128605 blaze_double_bot-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2558 2024-05-23 01:40:43.000000 blaze_double_bot-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 01:43:07.077810 blaze_double_bot-0.1.2/blaze_double_bot/
--rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.1.2/blaze_double_bot/__init__.py
--rw-rw-rw-   0        0        0     8981 2024-05-23 01:41:05.000000 blaze_double_bot-0.1.2/blaze_double_bot/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-23 01:43:07.128605 blaze_double_bot-0.1.2/blaze_double_bot.egg-info/
--rw-rw-rw-   0        0        0     3037 2024-05-23 01:43:06.000000 blaze_double_bot-0.1.2/blaze_double_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-23 01:43:06.000000 blaze_double_bot-0.1.2/blaze_double_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 01:43:06.000000 blaze_double_bot-0.1.2/blaze_double_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 01:43:06.000000 blaze_double_bot-0.1.2/blaze_double_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-23 01:43:06.000000 blaze_double_bot-0.1.2/blaze_double_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 01:43:07.133605 blaze_double_bot-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      585 2024-05-23 01:41:31.000000 blaze_double_bot-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:55:40.670087 blaze_double_bot-0.1.3/
+-rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3103 2024-05-23 11:55:40.670087 blaze_double_bot-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2596 2024-05-23 11:37:29.000000 blaze_double_bot-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 11:55:40.621775 blaze_double_bot-0.1.3/blaze_double_bot/
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.1.3/blaze_double_bot/__init__.py
+-rw-rw-rw-   0        0        0     8981 2024-05-23 01:41:05.000000 blaze_double_bot-0.1.3/blaze_double_bot/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:55:40.670087 blaze_double_bot-0.1.3/blaze_double_bot.egg-info/
+-rw-rw-rw-   0        0        0     3103 2024-05-23 11:55:40.000000 blaze_double_bot-0.1.3/blaze_double_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-23 11:55:40.000000 blaze_double_bot-0.1.3/blaze_double_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 11:55:40.000000 blaze_double_bot-0.1.3/blaze_double_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 11:55:40.000000 blaze_double_bot-0.1.3/blaze_double_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-23 11:55:40.000000 blaze_double_bot-0.1.3/blaze_double_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 11:55:40.670087 blaze_double_bot-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      618 2024-05-23 11:45:48.000000 blaze_double_bot-0.1.3/setup.py
```

### Comparing `blaze_double_bot-0.1.2/LICENSE` & `blaze_double_bot-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.1.2/PKG-INFO` & `blaze_double_bot-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.1.2
+Version: 0.1.3
 Summary: This Python library automates the betting process on the Blaze Double
 Author: Rafael de Oliveira Ribeiro
 Author-email: ror74559@gmail.com
 License: MIT License
+Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: undetected_chromedriver
 Requires-Dist: selenium
 Requires-Dist: requests
 
 # Blaze Double Bot
 
 ---
 
 ## Description
 
-This Python script automates the betting process on the Blaze Double website using Selenium and undetected-chromedriver. It monitors the game state, places bets according to a predefined strategy, and handles winnings and losses.
+This Python script automates the betting process on the Blaze Double website using Selenium and undetected-chromedriver. It monitors the game state, places bets according to a predefined strategy, and handles winnings and losses. Google Chrome browser required.
 
 ---
 
 ## Installation
 
 ```bash
 
@@ -75,15 +76,15 @@
         config = json.load(f)
 
 bot = BlazeDoubleBot(config)
 
 bot.run()
 
 ```
-#For each round won or lost, the bot will only perform the analyzes again after 5 rounds. The bot follows MartinGale's strategy of doubling the bet after a loss. He will repeat this procedure 2 times, or 1 time if he wins.
+# For each round won or lost, the bot will only perform the analyzes again after 5 rounds. The bot follows MartinGale's strategy of doubling the bet after a loss. The bot will repeat this procedure 2 times, or 1 time if it wins.
 ---
 
 ## Support This Project
 
 If you find this project helpful, consider supporting it by making a donation. Your contribution will help me maintain and improve this bot.
 
 [Donate via PayPal](https://www.paypal.com/donate/?hosted_button_id=928TRAX74TYSA)
```

### Comparing `blaze_double_bot-0.1.2/README.md` & `blaze_double_bot-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Blaze Double Bot
 
 ---
 
 ## Description
 
-This Python script automates the betting process on the Blaze Double website using Selenium and undetected-chromedriver. It monitors the game state, places bets according to a predefined strategy, and handles winnings and losses.
+This Python script automates the betting process on the Blaze Double website using Selenium and undetected-chromedriver. It monitors the game state, places bets according to a predefined strategy, and handles winnings and losses. Google Chrome browser required.
 
 ---
 
 ## Installation
 
 ```bash
 
@@ -62,15 +62,15 @@
         config = json.load(f)
 
 bot = BlazeDoubleBot(config)
 
 bot.run()
 
 ```
-#For each round won or lost, the bot will only perform the analyzes again after 5 rounds. The bot follows MartinGale's strategy of doubling the bet after a loss. He will repeat this procedure 2 times, or 1 time if he wins.
+# For each round won or lost, the bot will only perform the analyzes again after 5 rounds. The bot follows MartinGale's strategy of doubling the bet after a loss. The bot will repeat this procedure 2 times, or 1 time if it wins.
 ---
 
 ## Support This Project
 
 If you find this project helpful, consider supporting it by making a donation. Your contribution will help me maintain and improve this bot.
 
 [Donate via PayPal](https://www.paypal.com/donate/?hosted_button_id=928TRAX74TYSA)
```

### Comparing `blaze_double_bot-0.1.2/blaze_double_bot/bot.py` & `blaze_double_bot-0.1.3/blaze_double_bot/bot.py`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.1.2/blaze_double_bot.egg-info/PKG-INFO` & `blaze_double_bot-0.1.3/blaze_double_bot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.1.2
+Version: 0.1.3
 Summary: This Python library automates the betting process on the Blaze Double
 Author: Rafael de Oliveira Ribeiro
 Author-email: ror74559@gmail.com
 License: MIT License
+Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: undetected_chromedriver
 Requires-Dist: selenium
 Requires-Dist: requests
 
 # Blaze Double Bot
 
 ---
 
 ## Description
 
-This Python script automates the betting process on the Blaze Double website using Selenium and undetected-chromedriver. It monitors the game state, places bets according to a predefined strategy, and handles winnings and losses.
+This Python script automates the betting process on the Blaze Double website using Selenium and undetected-chromedriver. It monitors the game state, places bets according to a predefined strategy, and handles winnings and losses. Google Chrome browser required.
 
 ---
 
 ## Installation
 
 ```bash
 
@@ -75,15 +76,15 @@
         config = json.load(f)
 
 bot = BlazeDoubleBot(config)
 
 bot.run()
 
 ```
-#For each round won or lost, the bot will only perform the analyzes again after 5 rounds. The bot follows MartinGale's strategy of doubling the bet after a loss. He will repeat this procedure 2 times, or 1 time if he wins.
+# For each round won or lost, the bot will only perform the analyzes again after 5 rounds. The bot follows MartinGale's strategy of doubling the bet after a loss. The bot will repeat this procedure 2 times, or 1 time if it wins.
 ---
 
 ## Support This Project
 
 If you find this project helpful, consider supporting it by making a donation. Your contribution will help me maintain and improve this bot.
 
 [Donate via PayPal](https://www.paypal.com/donate/?hosted_button_id=928TRAX74TYSA)
```

### Comparing `blaze_double_bot-0.1.2/setup.py` & `blaze_double_bot-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as f:
           readme =f.read()
 
 setup(
     name='blaze_double_bot',
     licence='MIT License',
-    version='0.1.2',
+    version='0.1.3',
     author='Rafael de Oliveira Ribeiro',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='ror74559@gmail.com',
+    keywords='blaze double bot',
     description='This Python library automates the betting process on the Blaze Double',
     packages=['blaze_double_bot'],
     install_requires=[
         'undetected_chromedriver',
         'selenium',
         'requests'
     ],
```

