# Comparing `tmp/quantumwerewolf-3.1.1.tar.gz` & `tmp/quantumwerewolf-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantumwerewolf-3.1.1.tar", last modified: Thu Dec 21 20:20:32 2023, max compression
+gzip compressed data, was "quantumwerewolf-3.2.1.tar", last modified: Thu May 23 18:58:36 2024, max compression
```

## Comparing `quantumwerewolf-3.1.1.tar` & `quantumwerewolf-3.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 fvdbosch  (1000) fvdbosch  (1000)        0 2023-12-21 20:20:32.963337 quantumwerewolf-3.1.1/
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)     1069 2022-12-13 20:44:48.000000 quantumwerewolf-3.1.1/LICENSE
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)     6080 2023-12-21 20:20:32.962337 quantumwerewolf-3.1.1/PKG-INFO
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)     4335 2023-11-16 20:31:57.000000 quantumwerewolf-3.1.1/README.md
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)      662 2023-12-21 20:11:28.000000 quantumwerewolf-3.1.1/pyproject.toml
-drwxr-xr-x   0 fvdbosch  (1000) fvdbosch  (1000)        0 2023-12-21 20:20:32.961337 quantumwerewolf-3.1.1/quantumwerewolf/
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)    21983 2023-11-14 18:25:54.000000 quantumwerewolf-3.1.1/quantumwerewolf/backend.py
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)    13396 2023-11-30 15:07:12.000000 quantumwerewolf-3.1.1/quantumwerewolf/cli.py
-drwxr-xr-x   0 fvdbosch  (1000) fvdbosch  (1000)        0 2023-12-21 20:20:32.962337 quantumwerewolf-3.1.1/quantumwerewolf.egg-info/
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)     6080 2023-12-21 20:20:32.000000 quantumwerewolf-3.1.1/quantumwerewolf.egg-info/PKG-INFO
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)      302 2023-12-21 20:20:32.000000 quantumwerewolf-3.1.1/quantumwerewolf.egg-info/SOURCES.txt
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)        1 2023-12-21 20:20:32.000000 quantumwerewolf-3.1.1/quantumwerewolf.egg-info/dependency_links.txt
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)       60 2023-12-21 20:20:32.000000 quantumwerewolf-3.1.1/quantumwerewolf.egg-info/entry_points.txt
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)       16 2023-12-21 20:20:32.000000 quantumwerewolf-3.1.1/quantumwerewolf.egg-info/top_level.txt
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)       38 2023-12-21 20:20:32.963337 quantumwerewolf-3.1.1/setup.cfg
-drwxr-xr-x   0 fvdbosch  (1000) fvdbosch  (1000)        0 2023-12-21 20:20:32.962337 quantumwerewolf-3.1.1/tests/
--rw-r--r--   0 fvdbosch  (1000) fvdbosch  (1000)     5742 2023-11-14 18:25:54.000000 quantumwerewolf-3.1.1/tests/test_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:58:36.462491 quantumwerewolf-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 18:58:32.000000 quantumwerewolf-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-05-23 18:58:36.462491 quantumwerewolf-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-23 18:58:32.000000 quantumwerewolf-3.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-23 18:58:32.000000 quantumwerewolf-3.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:58:36.458491 quantumwerewolf-3.2.1/quantumwerewolf/
+-rw-r--r--   0 runner    (1001) docker     (127)    22229 2024-05-23 18:58:32.000000 quantumwerewolf-3.2.1/quantumwerewolf/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13618 2024-05-23 18:58:32.000000 quantumwerewolf-3.2.1/quantumwerewolf/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:58:36.462491 quantumwerewolf-3.2.1/quantumwerewolf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-05-23 18:58:36.000000 quantumwerewolf-3.2.1/quantumwerewolf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-23 18:58:36.000000 quantumwerewolf-3.2.1/quantumwerewolf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:58:36.000000 quantumwerewolf-3.2.1/quantumwerewolf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 18:58:36.000000 quantumwerewolf-3.2.1/quantumwerewolf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 18:58:36.000000 quantumwerewolf-3.2.1/quantumwerewolf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:58:36.462491 quantumwerewolf-3.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:58:36.462491 quantumwerewolf-3.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-23 18:58:32.000000 quantumwerewolf-3.2.1/tests/test_backend.py
```

### Comparing `quantumwerewolf-3.1.1/LICENSE` & `quantumwerewolf-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quantumwerewolf-3.1.1/PKG-INFO` & `quantumwerewolf-3.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumwerewolf
-Version: 3.1.1
+Version: 3.2.1
 Summary: Quantum version of the werewolves party game.
 License: MIT License
         
         Copyright (c) 2022 Jesse Straat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,39 +20,41 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/JesseStraat/Quantum-Werewolf
-Project-URL: Bug Tracker, https://github.com/JesseStraat/Quantum-Werewolf/issues
+Project-URL: Homepage, https://github.com/ProodjePindakaas/Quantum-Werewolf
+Project-URL: Bug Tracker, https://github.com/ProodjePindakaas/Quantum-Werewolf/issues
+Keywords: quantum,werewolf,werewolves,game
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Quantum Werewolf
 
 Quantum Werewolf is a game based on the party game "The Werewolves of Millers Hollow" (known as "Weerwolven van Wakkerdam" to Dutch audiences) with a quantum mechanical twist: Players play all possible games of werewolf at the same time.
 
 Original puzzle:
 https://web.archive.org/web/20080719133809/http://puzzle.cisra.com.au/D-5-Schroedingers-Wolves.pdf
+
 Solution and original explanation:
 https://web.archive.org/web/20181116123708/https://puzzle.cisra.com.au/2008/quantumwerewolf.html
 
 ## Installation
 
-`$ pip install git+https://github.com/ProodjePindakaas/Quantum-Werewolf`
+`$ pip install quantumwerewolf`
 
 ## Usage
 
-Start the game in a terminal by running the `quantum-werewolf` command.
+Start the game in a terminal by running the `quantumwerewolf` command.
 
 ## About
 
 ### What is "The Werewolves of Millers Hollow"?
 
 The Werewolves of Millers Hollow is a classical party game where each player (save the game master) gets a secret role card assigned to them. There are two teams: the werewolves
 and the village (consisting of all roles except the werewolves). At night, each player secretly takes an action corresponding to their role -- the seer gets to see another player's card,
```

### Comparing `quantumwerewolf-3.1.1/README.md` & `quantumwerewolf-3.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Quantum Werewolf
 
 Quantum Werewolf is a game based on the party game "The Werewolves of Millers Hollow" (known as "Weerwolven van Wakkerdam" to Dutch audiences) with a quantum mechanical twist: Players play all possible games of werewolf at the same time.
 
 Original puzzle:
 https://web.archive.org/web/20080719133809/http://puzzle.cisra.com.au/D-5-Schroedingers-Wolves.pdf
+
 Solution and original explanation:
 https://web.archive.org/web/20181116123708/https://puzzle.cisra.com.au/2008/quantumwerewolf.html
 
 ## Installation
 
-`$ pip install git+https://github.com/ProodjePindakaas/Quantum-Werewolf`
+`$ pip install quantumwerewolf`
 
 ## Usage
 
-Start the game in a terminal by running the `quantum-werewolf` command.
+Start the game in a terminal by running the `quantumwerewolf` command.
 
 ## About
 
 ### What is "The Werewolves of Millers Hollow"?
 
 The Werewolves of Millers Hollow is a classical party game where each player (save the game master) gets a secret role card assigned to them. There are two teams: the werewolves
 and the village (consisting of all roles except the werewolves). At night, each player secretly takes an action corresponding to their role -- the seer gets to see another player's card,
```

### Comparing `quantumwerewolf-3.1.1/pyproject.toml` & `quantumwerewolf-3.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quantumwerewolf"
-version = "3.1.1"
+version = "3.2.1"
+requires-python = ">=3.8"
 description = "Quantum version of the werewolves party game."
 readme = "README.md"
 license = {file = "LICENSE"}
-requires-python = ">=3.7"
+keywords = ["quantum", "werewolf", "werewolves", "game"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = []
 
 [project.scripts]
 quantumwerewolf = "quantumwerewolf.cli:cli"
 
 [project.urls]
-"Homepage" = "https://github.com/JesseStraat/Quantum-Werewolf"
-"Bug Tracker" = "https://github.com/JesseStraat/Quantum-Werewolf/issues"
+"Homepage" = "https://github.com/ProodjePindakaas/Quantum-Werewolf"
+"Bug Tracker" = "https://github.com/ProodjePindakaas/Quantum-Werewolf/issues"
```

### Comparing `quantumwerewolf-3.1.1/quantumwerewolf/backend.py` & `quantumwerewolf-3.2.1/quantumwerewolf/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """The Module's docstring"""
 
 from itertools import permutations
 from random import shuffle, choice
 from functools import wraps
 from typing import Callable, List, Tuple, Union
-from math import sqrt
+from math import factorial
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class Player:
 
@@ -34,15 +34,15 @@
         self.players = []
         self.role_count = Game.default_roles.copy()
         self.player_count = 0
         self.started = False
         self.logger = logging.getLogger(__name__)
         # optional rules
         self.werewolf_cannot_eat_werewolf = False
-        self.max_permutations = 20
+        self.start_with_subset = True
 
     # HELPER FUNCTIONS
 
     def started(value: bool = True) -> Callable:
         """Return decorator that return decorated function that only runs when the game has started (or not).
 
         Arguments:
@@ -70,23 +70,14 @@
         """Return the name of a player index.
 
         Arguments:
             player_id: str -- index of player in Game.add_players
         """
         return self.players[player_id]
 
-    def expected_total_deviation(self):
-        """Return the total expected role ratio deviation.
-
-            $$ TD = \\sum_{role} \\sqrt{p_{role} (1 - p_{role})} $$
-        """
-        ratios = [count / self.player_count for count in self.role_count.values()]
-        deviations = [sqrt(p * (1 - p)) for p in ratios]
-        return sum(deviations)
-
     # SETUP METHODS
 
     @started(False)
     def add_players(self, *names: Union[str, List[str]]) -> None:
         """Add players to the Game.players list.
 
         Arguments:
@@ -117,14 +108,40 @@
             role: str -- name of a role
             amount: int -- the amount of players with the given role
         """
         self.logger.debug(f"running set_role({role}, {amount})")
         self.role_count[role] = amount
         self.logger.info(f'Setting amount of {role} role to {amount}')
 
+    def generate_all_permutations(self):
+        self.logger.info('Generating all role permutations')
+        roles = [role for role, count in self.role_count.items() for _ in range(count)]
+        self.logger.debug(f'role frequencies: {roles}')
+        self.permutations = {p: True for p in permutations(roles)}
+
+    def _max_permutations(self):
+        number = factorial(self.player_count)
+        for n in self.role_count.values():
+            number /= factorial(n)
+        return number
+
+    def _subset_size(self):
+        max_subset_size = self._max_permutations()
+        return min(self.player_count + 2, max_subset_size)
+
+    def generate_subset_permutations(self):
+        self.logger.info('Generating subset of role permutations')
+        roles = [role for role, count in self.role_count.items() for _ in range(count)]
+        self.logger.debug(f'role frequencies: {roles}')
+        n_permutations = self._subset_size()
+        self.permutations = {}
+        while len(self.permutations) < n_permutations:
+            shuffle(roles)
+            self.permutations[tuple(roles)] = True
+
     @started(False)
     def start(self) -> bool:
         """Start the game and return succes boolean."""
         self.logger.debug("running start()")
 
         # Determine playercount
         self.player_count = len(self.players)
@@ -153,25 +170,20 @@
         # Sets the list of roles
         self.used_roles = [role for role, count in self.role_count.items() if count > 0]
         self.logger.info(f'Roles used in game are {self.used_roles}')
 
         self.werewolf_count = self.role_count['werewolf']
         self.logger.info(f'Number of live werewolves is {self.werewolf_count}')
 
-        # Generates the list of all role permutations
-        self.logger.info('Generating all role permutations')
-        roles = [role for role, count in self.role_count.items() for _ in range(count)]
-        self.logger.debug(f'role frequencies: {roles}')
-        # full permutation game
-        self.permutations = {p: True for p in permutations(roles)}
-        # random subset game
-        # self.permutations = {p: True for p in permutations(roles) if random() < self.permutation_fraction}
-        # optimal deviation game
-        # n_permutations =  (self.expected_total_deviation() / optimal_total_deviation) ** 2
-        # self.permutations = {shuffle(roles).copy(): True for _ in range(n_permutations)}
+        # Generates the list of role permutations
+        if self.start_with_subset:
+            self.generate_subset_permutations()
+        else:
+            self.generate_all_permutations()
+
         self.logger.debug(f'number of permutations: {len(self.permutations)}')
 
         # Set all players to be fully alive
         self.logger.info('Initializing attacked and killed list')
         self.deaths = []
         for i in range(self.player_count):
             self.deaths += [[0] * self.player_count]
```

### Comparing `quantumwerewolf-3.1.1/quantumwerewolf/cli.py` & `quantumwerewolf-3.2.1/quantumwerewolf/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         'villager': 'a ',
         'werewolf': 'a ',
         'seer': 'the ',
         'hunter': 'the ',
         'cupid': '',
         }
 
-    bar_length = 24
+    bar_length = 36
     name_length = 12
 
     def ask_yesno(self, query, yes, no):
         answer = input(query + ' (yes/no) ')
         if answer == 'yes' or answer == 'y':
             if isinstance(yes, str):
                 print(yes)
@@ -66,15 +66,15 @@
         else:
             print('invalid answer')
             self.ask_yesno(query, yes, no)
 
     def ask_player(self, query, invalid_players=[]):
         answer = input(query + 'Name: ')
 
-        if answer.isdigit():
+        if answer.isdecimal():
             i = int(answer) - 1
             if i in range(self.player_count):
                 answer = self.players[i]
 
         valid_players = self.living_players()
         for player in invalid_players:
             valid_players.remove(player)
@@ -126,18 +126,23 @@
 
         for i in self.print_permutation:
             p = probabilities[i]
             name = '???'
             if p['dead'] == 1 or game_over:
                 name = p['name']
             line = f"{str(name):>{self.name_length}}    "
+            total_chance = 0.0
+            total_length = 0
             for role in self.used_roles:
-                chance = p[role]
                 letter = role[0].capitalize()
-                length = round(chance * self.bar_length)
+                chance = p[role]
+                total_chance += chance
+                total_length_new = round(total_chance * self.bar_length)
+                length = total_length_new - total_length
+                total_length = total_length_new
                 line += f"{self.role_style_bold[role]}{letter * length}"
             line += f"{self.normal}{100*p['dead']:11.0f}% dead"
             print(line)
 
     def print_kill(self, player, cause=''):
         player_role = self.kill(player)
         print(f'\n  {player} was killed {cause}')
```

### Comparing `quantumwerewolf-3.1.1/quantumwerewolf.egg-info/PKG-INFO` & `quantumwerewolf-3.2.1/quantumwerewolf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumwerewolf
-Version: 3.1.1
+Version: 3.2.1
 Summary: Quantum version of the werewolves party game.
 License: MIT License
         
         Copyright (c) 2022 Jesse Straat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,39 +20,41 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/JesseStraat/Quantum-Werewolf
-Project-URL: Bug Tracker, https://github.com/JesseStraat/Quantum-Werewolf/issues
+Project-URL: Homepage, https://github.com/ProodjePindakaas/Quantum-Werewolf
+Project-URL: Bug Tracker, https://github.com/ProodjePindakaas/Quantum-Werewolf/issues
+Keywords: quantum,werewolf,werewolves,game
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Quantum Werewolf
 
 Quantum Werewolf is a game based on the party game "The Werewolves of Millers Hollow" (known as "Weerwolven van Wakkerdam" to Dutch audiences) with a quantum mechanical twist: Players play all possible games of werewolf at the same time.
 
 Original puzzle:
 https://web.archive.org/web/20080719133809/http://puzzle.cisra.com.au/D-5-Schroedingers-Wolves.pdf
+
 Solution and original explanation:
 https://web.archive.org/web/20181116123708/https://puzzle.cisra.com.au/2008/quantumwerewolf.html
 
 ## Installation
 
-`$ pip install git+https://github.com/ProodjePindakaas/Quantum-Werewolf`
+`$ pip install quantumwerewolf`
 
 ## Usage
 
-Start the game in a terminal by running the `quantum-werewolf` command.
+Start the game in a terminal by running the `quantumwerewolf` command.
 
 ## About
 
 ### What is "The Werewolves of Millers Hollow"?
 
 The Werewolves of Millers Hollow is a classical party game where each player (save the game master) gets a secret role card assigned to them. There are two teams: the werewolves
 and the village (consisting of all roles except the werewolves). At night, each player secretly takes an action corresponding to their role -- the seer gets to see another player's card,
```

### Comparing `quantumwerewolf-3.1.1/tests/test_backend.py` & `quantumwerewolf-3.2.1/tests/test_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 - test cupid action
     - test computation of lovers
 - test win condition check
 
 """
 
 from quantumwerewolf.backend import Game
-from math import factorial
 from unittest import TestCase, main
 import logging
 
 
 class TestGame(TestCase):
 
     def setUp(self):
@@ -61,14 +60,15 @@
             self.game.set_role(r, 683)
             self.assertEqual(self.game.role_count[r], 683)
 
     def test_start_succesful(self):
         # test succesful start
         names = ['Alice', 'Bob', 'Craig', 'David']
         self.game.add_players(names)
+        self.game.start_with_subset = False
         self.assertTrue(self.game.start())
 
         # test state of game
         self.assertTrue(self.game.started)
 
         # test assignment of player count
         self.assertEqual(self.game.player_count, len(names))
@@ -86,17 +86,15 @@
         self.assertEqual(self.game.role_count['werewolf'], 2)
         self.assertEqual(self.game.role_count['seer'], 1)
         self.assertEqual(self.game.role_count['hunter'], 0)
         self.assertEqual(self.game.role_count['cupid'], 0)
         self.assertEqual(self.game.role_count['villager'], 1)
 
         # test number of permutations
-        n_perm = factorial(self.game.player_count)
-        for i in self.game.role_count.values():
-            n_perm /= factorial(i)
+        n_perm = self.game._max_permutations()
 
         self.assertEqual(len(self.game.permutations), n_perm)
 
     def test_start_fail(self):
         # test no players
         self.assertFalse(self.game.start())
         # test too few players
@@ -107,14 +105,15 @@
 class TestGameStarted(TestCase):
 
     def setUp(self):
         logging.basicConfig(level=logging.WARNING)
         self.game = Game()
         self.names = ['Alice', 'Bob', 'Craig', 'David']
         self.game.add_players(self.names)
+        self.game.start_with_subset = False
         self.game.start()
 
     def tearDown(self):
         del self.game
 
     def test_add_players_error(self):
         self.assertRaises(ValueError, self.game.add_players, 'Alice')
@@ -150,15 +149,15 @@
         # test without lovers
 
         # test with lovers
         pass
 
     def test_calculate_probabilities(self):
         # check results at start of the a game
-        result_start = self.game.calculate_probabilities()
+        result_start = self.game.role_probabilities()
         for player_result in result_start:
             self.assertIn('name', player_result)
             self.assertIn(player_result['name'], self.game.players)
             self.assertEqual(player_result['werewolf'], 2/4)
             self.assertEqual(player_result['seer'], 1/4)
             # self.assertEqual(player_result['hunter'], 0)
             # self.assertEqual(player_result['cupid'], 0)
```

