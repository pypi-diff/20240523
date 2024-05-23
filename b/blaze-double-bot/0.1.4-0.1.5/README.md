# Comparing `tmp/blaze_double_bot-0.1.4.tar.gz` & `tmp/blaze_double_bot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze_double_bot-0.1.4.tar", last modified: Thu May 23 12:07:04 2024, max compression
+gzip compressed data, was "blaze_double_bot-0.1.5.tar", last modified: Thu May 23 13:30:10 2024, max compression
```

## Comparing `blaze_double_bot-0.1.4.tar` & `blaze_double_bot-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 12:07:04.218964 blaze_double_bot-0.1.4/
--rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     3164 2024-05-23 12:07:04.213290 blaze_double_bot-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2657 2024-05-23 12:04:16.000000 blaze_double_bot-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 12:07:04.142916 blaze_double_bot-0.1.4/blaze_double_bot/
--rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.1.4/blaze_double_bot/__init__.py
--rw-rw-rw-   0        0        0     8981 2024-05-23 01:41:05.000000 blaze_double_bot-0.1.4/blaze_double_bot/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-23 12:07:04.211546 blaze_double_bot-0.1.4/blaze_double_bot.egg-info/
--rw-rw-rw-   0        0        0     3164 2024-05-23 12:07:03.000000 blaze_double_bot-0.1.4/blaze_double_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-23 12:07:03.000000 blaze_double_bot-0.1.4/blaze_double_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 12:07:03.000000 blaze_double_bot-0.1.4/blaze_double_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 12:07:03.000000 blaze_double_bot-0.1.4/blaze_double_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-23 12:07:03.000000 blaze_double_bot-0.1.4/blaze_double_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 12:07:04.220052 blaze_double_bot-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      618 2024-05-23 12:06:24.000000 blaze_double_bot-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:30:10.087317 blaze_double_bot-0.1.5/
+-rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     3164 2024-05-23 13:30:10.078796 blaze_double_bot-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2657 2024-05-23 12:04:16.000000 blaze_double_bot-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 13:30:09.937962 blaze_double_bot-0.1.5/blaze_double_bot/
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-0.1.5/blaze_double_bot/__init__.py
+-rw-rw-rw-   0        0        0     9343 2024-05-23 13:29:06.000000 blaze_double_bot-0.1.5/blaze_double_bot/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:30:10.077773 blaze_double_bot-0.1.5/blaze_double_bot.egg-info/
+-rw-rw-rw-   0        0        0     3164 2024-05-23 13:30:09.000000 blaze_double_bot-0.1.5/blaze_double_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-23 13:30:09.000000 blaze_double_bot-0.1.5/blaze_double_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 13:30:09.000000 blaze_double_bot-0.1.5/blaze_double_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 13:30:09.000000 blaze_double_bot-0.1.5/blaze_double_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-23 13:30:09.000000 blaze_double_bot-0.1.5/blaze_double_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 13:30:10.087317 blaze_double_bot-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      618 2024-05-23 13:29:32.000000 blaze_double_bot-0.1.5/setup.py
```

### Comparing `blaze_double_bot-0.1.4/LICENSE` & `blaze_double_bot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.1.4/PKG-INFO` & `blaze_double_bot-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.1.4
+Version: 0.1.5
 Summary: This Python library automates the betting process on the Blaze Double
 Author: Rafael de Oliveira Ribeiro
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-0.1.4/README.md` & `blaze_double_bot-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-0.1.4/blaze_double_bot/bot.py` & `blaze_double_bot-0.1.5/blaze_double_bot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             print('Error getting history:', e)
             return ['n'] * size
 
     def get_history_api(self, size):
         colors = {0: 'W', 1: 'R', 2: 'B'}
         history = requests.get('https://blaze1.space/api/roulette_games/recent').json()
         history_list = [h['color'] for h in history][:size]
-        return [colors[n] for n in history_list]
+        return [colors[n] for n in history_list][::-1]
 
     def choose_color(self, color):
         bet_buttons = self.driver.find_elements(By.CLASS_NAME, color)
         for btn in bet_buttons:
             if 'x2' in btn.text:
                 btn.click()
                 break
@@ -114,15 +114,15 @@
 Bet on {"Red" if color == "red" else "Black"}
 Completed
 Waiting for result ...
 
 ''')
 
     def print_bet_result(self, history, color):
-        print("Green" if history[0] == self.color_dict[color] else "Red")
+        print("Win" if history[0] == self.color_dict[color] else "Loss")
 
     def get_balance(self):
         return float(self.driver.find_element(By.CLASS_NAME, 'amount').text.replace(',', '.').split(' ')[-1])
 
     def strategy(self, history):
         for color, sequences in self.strategies.items():
             for sequence in sequences:
@@ -190,38 +190,46 @@
             strategy_size = self.get_strategy_size()
             while True:
                 if self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
                     if self.wait_for_next_round():
                         history = self.get_history_api(strategy_size)
                         color = self.strategy(history)
                         if color:
+                            print(history)
+                            print()
                             self.choose_color(color)
                             self.place_bet(self.bet_amount)
                             self.print_bet(color)
                             self.wait_for_next_round()
                             sleep(1)
                             history = self.get_history_api(strategy_size)
                             if history[0] != self.color_dict[color] and self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
+                                print(history)
+                                print()
                                 print('Gale 1')
                                 self.place_bet(2 * self.bet_amount)
                                 self.wait_for_next_round()
                                 sleep(1)
                                 history = self.get_history_api(strategy_size)
                                 if history[0] != self.color_dict[color] and self.stop_loss <= self.current_balance <= self.stop_win and self.current_balance - self.bet_amount >= 0:
+                                    print(history)
+                                    print()
                                     print('Gale 2')
                                     self.place_bet(4 * self.bet_amount)
                                     self.wait_for_next_round()
                                     sleep(1)
                                     history = self.get_history_api(strategy_size)
                             self.print_bet_result(history, color)
                             sleep(8)
                             self.current_balance = self.get_balance()
-                            print(self.current_balance)
+                            print('Balance: ',self.current_balance)
                             print('Waiting 5 rounds to restart analysis ...')
+                            print(50*'*')
                             sleep(150)
+                            print(50*'*')
                             print('Analyzes restarted!\n\n')
                 else:
                     self.print_final_text()
                     self.close_driver()
                     break
                 sleep(2)
         except Exception as e:
```

### Comparing `blaze_double_bot-0.1.4/blaze_double_bot.egg-info/PKG-INFO` & `blaze_double_bot-0.1.5/blaze_double_bot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 0.1.4
+Version: 0.1.5
 Summary: This Python library automates the betting process on the Blaze Double
 Author: Rafael de Oliveira Ribeiro
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-0.1.4/setup.py` & `blaze_double_bot-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as f:
           readme =f.read()
 
 setup(
     name='blaze_double_bot',
     licence='MIT License',
-    version='0.1.4',
+    version='0.1.5',
     author='Rafael de Oliveira Ribeiro',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='ror74559@gmail.com',
     keywords='blaze double bot',
     description='This Python library automates the betting process on the Blaze Double',
     packages=['blaze_double_bot'],
```

