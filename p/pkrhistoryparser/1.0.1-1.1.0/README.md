# Comparing `tmp/pkrhistoryparser-1.0.1.tar.gz` & `tmp/pkrhistoryparser-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrhistoryparser-1.0.1.tar", last modified: Tue May 21 23:18:27 2024, max compression
+gzip compressed data, was "pkrhistoryparser-1.1.0.tar", last modified: Thu May 23 02:05:41 2024, max compression
```

## Comparing `pkrhistoryparser-1.0.1.tar` & `pkrhistoryparser-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-21 23:18:27.832361 pkrhistoryparser-1.0.1/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-21 23:18:27.660654 pkrhistoryparser-1.0.1/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-05-21 11:12:27.000000 pkrhistoryparser-1.0.1/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2024-05-21 10:03:22.000000 pkrhistoryparser-1.0.1/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      878 2024-05-21 23:16:45.000000 pkrhistoryparser-1.0.1/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      816 2024-05-21 23:18:27.832361 pkrhistoryparser-1.0.1/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       94 2024-05-21 10:05:17.000000 pkrhistoryparser-1.0.1/Readme.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      480 2024-05-21 23:16:56.000000 pkrhistoryparser-1.0.1/coverage.txt
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-21 23:18:27.692977 pkrhistoryparser-1.0.1/pkrhistoryparser/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       65 2024-05-21 22:15:01.000000 pkrhistoryparser-1.0.1/pkrhistoryparser/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13602 2024-05-21 22:56:20.000000 pkrhistoryparser-1.0.1/pkrhistoryparser/parser.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-21 23:18:27.722544 pkrhistoryparser-1.0.1/pkrhistoryparser/patterns/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-21 22:08:32.000000 pkrhistoryparser-1.0.1/pkrhistoryparser/patterns/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1755 2024-05-21 21:55:25.000000 pkrhistoryparser-1.0.1/pkrhistoryparser/patterns/winamax.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-21 23:18:27.814756 pkrhistoryparser-1.0.1/pkrhistoryparser/pkrhistoryparser.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      816 2024-05-21 23:17:58.000000 pkrhistoryparser-1.0.1/pkrhistoryparser/pkrhistoryparser.egg-info/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      511 2024-05-21 23:18:27.000000 pkrhistoryparser-1.0.1/pkrhistoryparser/pkrhistoryparser.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        1 2024-05-21 23:17:58.000000 pkrhistoryparser-1.0.1/pkrhistoryparser/pkrhistoryparser.egg-info/dependency_links.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       70 2024-05-21 23:17:58.000000 pkrhistoryparser-1.0.1/pkrhistoryparser/pkrhistoryparser.egg-info/requires.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        9 2024-05-21 23:17:58.000000 pkrhistoryparser-1.0.1/pkrhistoryparser/pkrhistoryparser.egg-info/top_level.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      658 2024-05-21 10:02:01.000000 pkrhistoryparser-1.0.1/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-21 23:18:27.832361 pkrhistoryparser-1.0.1/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1381 2024-05-21 23:15:42.000000 pkrhistoryparser-1.0.1/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-23 02:05:41.646966 pkrhistoryparser-1.1.0/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2024-05-21 10:03:22.000000 pkrhistoryparser-1.1.0/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      930 2024-05-22 08:56:50.000000 pkrhistoryparser-1.1.0/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      816 2024-05-23 02:05:41.646966 pkrhistoryparser-1.1.0/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       94 2024-05-21 10:05:17.000000 pkrhistoryparser-1.1.0/Readme.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      480 2024-05-23 02:03:37.000000 pkrhistoryparser-1.1.0/coverage.txt
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-23 02:05:41.506424 pkrhistoryparser-1.1.0/pkrhistoryparser/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       65 2024-05-21 22:15:01.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    17871 2024-05-23 02:02:33.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/parser.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-23 02:05:41.537640 pkrhistoryparser-1.1.0/pkrhistoryparser/patterns/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-21 22:08:32.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/patterns/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1847 2024-05-23 00:04:19.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/patterns/winamax.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-23 02:05:41.615708 pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      816 2024-05-23 02:04:54.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      487 2024-05-23 02:05:40.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        1 2024-05-23 02:04:54.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/dependency_links.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       70 2024-05-23 02:04:54.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/requires.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        9 2024-05-23 02:04:54.000000 pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/top_level.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      658 2024-05-21 10:02:01.000000 pkrhistoryparser-1.1.0/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-23 02:05:41.646966 pkrhistoryparser-1.1.0/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1381 2024-05-21 23:15:42.000000 pkrhistoryparser-1.1.0/setup.py
```

### Comparing `pkrhistoryparser-1.0.1/LICENSE.txt` & `pkrhistoryparser-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrhistoryparser-1.0.1/MANIFEST.in` & `pkrhistoryparser-1.1.0/MANIFEST.in`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 prune docs
 prune tests
 prune scripts
 prune .github
 prune .git
 prune .gitignore
 prune .idea
+prune .vscode
+prune .pytest_cache
+prune coverage
 
 global-exclude *.py[cod]  # Exclure les fichiers de bytecode Python
 global-exclude *.swp      # Exclure les fichiers swap de Vim
 global-exclude *.bak      # Exclure les fichiers de sauvegarde
 global-exclude *.tmp      # Exclure les fichiers temporaires
 global-exclude .DS_Store  # Exclure les fichiers système spécifiques à MacOS
 global-exclude *.log      # Exclure les fichiers log
```

### Comparing `pkrhistoryparser-1.0.1/PKG-INFO` & `pkrhistoryparser-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrhistoryparser
-Version: 1.0.1
+Version: 1.1.0
 Summary: A poker package to parse Hand histories into json objects
 Home-page: https://github.com/manggy94/PokerHistoryParser
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/manggy94/PokerHistoryParser/issues
 Platform: UNKNOWN
```

### Comparing `pkrhistoryparser-1.0.1/pkrhistoryparser/parser.py` & `pkrhistoryparser-1.1.0/pkrhistoryparser/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,102 @@
-""" This module contains the HandHistoryParser class which is used to parse poker hand histories. """
+"""
+This module contains the HandHistoryParser class which is used to parse poker hand histories.
+This doc is destined for developers who will work on the pkrhistoryparser module.
+"""
+import json
 import re
-import os
 from datetime import datetime
 from .patterns import winamax as patterns
 
 
 class HandHistoryParser:
+    """
+    A class to parse poker hand histories.
 
+    Methods
+    -------
+    get_raw_text(history_path)
+        Get the raw text from a history file.
+    to_float(txt_num)
+        Transform a string number into a float.
+    extract_game_type(hand_txt)
+        Extract the type of the game from the hand text.
+    parse_to_json(history_path, destination_path)
+        Parse a poker hand history to a JSON format.
+
+    Examples
+    --------
+    1. Parse a poker hand history to a dict to be used in a program:
+
+        >>> parser = HandHistoryParser()
+        >>> hand_text = parser.get_raw_text("path/to/hand/history.txt")
+        >>> hand_info = parser.parse_hand(hand_text)
+
+    2. Parse a poker hand history to a JSON file:
+
+        >>> history_parser = HandHistoryParser()
+        >>> history_parser.parse_to_json('path/to/hand/history.txt', 'path/to/save/json/file.json')
+    """
     @staticmethod
     def get_raw_text(history_path) -> str:
         """
         Get the raw text from a history file
-        :param history_path:
-        :return: The text of the hand history file
+
+        Parameters:
+            history_path (str): The path to the history file.
+
+        Returns:
+            str: The text of the hand history file.
         """
         with open(history_path, "r", encoding="utf-8") as file:
             hand_text = file.read()
         return hand_text
 
     @staticmethod
     def to_float(txt_num: str) -> float:
         """
         Transforms any written str number into a float
-        :param txt_num: number to transform
-        :return: float number
+
+        Parameters:
+            txt_num(str): The number to transform
+
+        Returns:
+            float: The float number
+
         """
         try:
             return float(txt_num.replace(",", "."))
         except (TypeError, AttributeError, ValueError):
             return 0.0
 
     @staticmethod
     def extract_game_type(hand_txt: str) -> dict:
         """
         Extract the type of the game (Tournament or CashGame).
+
+        Parameters:
+            hand_txt (str): The raw poker hand text as a string.
+
+        Returns:
+            dict: A dictionary containing the game type extracted from the poker hand history(game_type).
         """
         game_types = {"Tournament": "Tournament", "CashGame": "CashGame"}
         game_type = next((game_types[key] for key in game_types if key in hand_txt), "Unknown")
         return {"game_type": game_type}
 
     def extract_players(self, hand_txt: str) -> dict:
         """
         Extract player information from a raw poker hand history and return as a dictionary.
 
         Parameters:
-            hand_txt (str): The hand history as a string.
+            hand_txt (str): The raw poker hand history as a string.
 
         Returns:
-            dict: A dictionary containing player information (seat, pseudo, stack, and bounty if available).
+            dict: A dictionary containing player information(seat, pseudo, stack, bounty).
+
         """
         matches = re.findall(pattern=patterns.PLAYER_PATTERN, string=hand_txt)
         players_info = {int(seat): {
             "seat": int(seat),
             "pseudo": pseudo,
             "stack": self.to_float(stack),
             "bounty": self.to_float(bounty) if bounty else None
@@ -62,25 +107,34 @@
         """
         Extract blinds and antes posted information from a  poker hand history and return as a dictionary.
 
         Parameters:
             hand_txt (str): The raw poker hand history as a string.
 
         Returns:
-            list: A dictionary containing blinds and antes information.
+            list: A list of dictionaries containing blinds and antes information(pseudo, amount, blind_type).
+
         """
         matches = re.findall(pattern=patterns.BLINDS_PATTERN, string=hand_txt)
         blinds_antes_info = [{"pseudo": pseudo.strip(), "amount": self.to_float(amount), "blind_type": blind_type} for
                              pseudo, blind_type, amount in matches]
 
         return blinds_antes_info
 
     def extract_buy_in(self, hand_txt: str) -> dict:
         """
         Extract the buy-in and rake information.
+
+        Parameters:
+            hand_txt (str): The raw poker hand text as a string.
+
+        Returns:
+            dict: A dict containing the buy-in and rake extracted
+            from the poker hand history(prize_pool_contribution, bounty, rake).
+
         """
         ko_buy_in_match = re.search(pattern=patterns.KO_BUY_IN_PATTERN, string=hand_txt)
         buy_in_match = re.search(pattern=patterns.NORMAL_BUY_IN_PATTERN, string=hand_txt)
         free_roll_match = re.search(pattern=patterns.FREE_ROLL_PATTERN, string=hand_txt)
         if ko_buy_in_match:
             prize_pool_contribution, bounty, rake = (ko_buy_in_match.group(1), ko_buy_in_match.group(2),
                                                      ko_buy_in_match.group(3))
@@ -94,22 +148,35 @@
         return {"prize_pool_contribution": self.to_float(prize_pool_contribution), "bounty": self.to_float(bounty),
                 "rake": self.to_float(rake)}
 
     @staticmethod
     def extract_datetime(hand_txt: str) -> dict:
         """
         Extract the datetime information.
+
+        Parameters:
+            hand_txt (str): The raw poker hand text as a string.
+
+        Returns:
+            dict: A dictionary containing the datetime extracted from the poker hand history(datetime).
         """
         datetime_match = re.search(pattern=patterns.DATETIME_PATTERN, string=hand_txt)
         dt = datetime.strptime(datetime_match.group(1), "%Y/%m/%d %H:%M:%S")
-        return {"datetime": dt}
+        dt_str = dt.strftime("%d-%m-%Y %H:%M:%S")
+        return {"datetime": dt_str}
 
     def extract_blinds(self, hand_txt: str) -> dict:
         """
         Extract the blind levels and ante.
+
+        Parameters:
+            hand_txt (str): The raw poker hand text as a string.
+
+        Returns:
+            dict: A dictionary containing the blind levels and ante extracted from the poker hand history(ante, sb, bb).
         """
         tour_blinds_match = re.search(pattern=patterns.TOURNAMENT_BLINDS_PATTERN, string=hand_txt)
         other_blinds_match = re.search(pattern=patterns.OTHER_BLINDS_PATTERN, string=hand_txt)
         if tour_blinds_match:
             ante, sb, bb = tour_blinds_match.group(1), tour_blinds_match.group(2), tour_blinds_match.group(3)
         elif other_blinds_match:
             sb, bb = (other_blinds_match.group(1).replace("€", ""),
@@ -119,133 +186,165 @@
             ante, sb, bb = None, None, None
         return {"ante": self.to_float(ante), "sb": self.to_float(sb), "bb": self.to_float(bb)}
 
     @staticmethod
     def extract_level(hand_txt: str) -> dict:
         """
         Extract the level information.
+
+        Parameters:
+            hand_txt (str): The raw poker hand text as a string.
+
+        Returns:
+            dict: A dictionary containing the level extracted from the poker hand history(level).
         """
         level_match = re.search(pattern=patterns.LEVEL_PATTERN, string=hand_txt)
         return {"level": int(level_match.group(1)) if level_match else 0}
 
     @staticmethod
     def extract_max_players(hand_txt: str) -> dict:
         """
         Extract the max players at the table.
+
+        Parameters:
+            hand_txt (str): The raw poker hand text as a string.
+
+        Returns:
+            dict: A dictionary containing the max players extracted from the poker hand history(max_players).
         """
         max_players = re.search(pattern=patterns.MAX_PLAYERS_PATTERN, string=hand_txt).group(1)
         return {"max_players": int(max_players)}
 
     @staticmethod
     def extract_button_seat(hand_txt: str) -> dict:
         """
         Extract the button seat information.
+
+        Parameters:
+            hand_txt (str): The raw poker hand text as a string.
+
+        Returns:
+            dict: A dictionary containing the button seat extracted from the poker hand history(button).
         """
         button = re.search(pattern=patterns.BUTTON_SEAT_PATTERN, string=hand_txt).group(1)
         return {"button": int(button)}
 
     @staticmethod
     def extract_table_name(hand_txt: str) -> dict:
         """
         Extract the table name information.
+
+        Parameters:
+            hand_txt (str): The raw poker hand text as a string.
+
+        Returns:
+            dict: A dictionary containing the table name extracted from the poker hand history(table_name).
         """
         table_name = re.search(pattern=patterns.TABLE_NAME_PATTERN, string=hand_txt).group(1)
         return {"table_name": table_name}
 
     @staticmethod
     def extract_table_ident(hand_txt: str) -> dict:
         """
         Extract the table ident information.
+
+        Parameters:
+            hand_txt (str): The raw poker hand text as a string.
+
+        Returns:
+            dict: A dictionary containing the table ident extracted from the poker hand history(table_ident).
         """
         table_ident = re.search(pattern=patterns.TABLE_IDENT_PATTERN, string=hand_txt).group(1)
         return {"table_ident": table_ident}
 
     @staticmethod
     def extract_hero_hand(hand_txt: str) -> dict:
         """
         Extract the hero's hand (hole cards) from a single poker hand text and return as a string.
 
         Parameters:
             hand_txt (str): The raw poker hand text as a string.
 
         Returns:
-            str: A string representing the hero's hand (hole cards).
+            dict: A dictionary containing the hero's hand extracted from the poker hand history(hero, first_card, second_card).
         """
         hero, card1, card2 = re.search(pattern=patterns.HERO_HAND_PATTERN, string=hand_txt, flags=re.UNICODE).groups()
         return {"hero": hero, "first_card": card1, "second_card": card2}
 
     @staticmethod
     def extract_flop(hand_txt: str) -> dict:
         """
         Extract the cards on the Flop from a single poker hand text and return as a string.
 
         Parameters:
             hand_txt (str): The raw poker hand text as a string.
 
         Returns:
-            str: A string representing the cards on the Flop.
+            dict: A dictionary representing the cards on the Flop(flop_card_1, flop_card_2, flop_card_3).
         """
         flop_match = re.search(pattern=patterns.FLOP_PATTERN, string=hand_txt, flags=re.UNICODE)
         card1, card2, card3 = flop_match.groups() if flop_match else (None, None, None)
         return {"flop_card_1": card1, "flop_card_2": card2, "flop_card_3": card3}
 
     @staticmethod
     def extract_turn(hand_txt: str) -> dict:
         """
         Extract the card on the Turn from a single poker hand text and return as a string.
 
         Parameters:
             hand_txt (str): The raw poker hand text as a string.
 
         Returns:
-            dict: A dictionary representing the card on the Turn.
+            dict: A dictionary representing the card on the Turn(turn_card).
         """
         turn_match = re.search(pattern=patterns.TURN_PATTERN, string=hand_txt, flags=re.UNICODE)
         card = turn_match.group(1) if turn_match else None
         return {"turn_card": card}
 
     @staticmethod
     def extract_river(hand_txt: str) -> dict:
         """
         Extract the card on the River from a single poker hand text and return as a string.
 
         Parameters:
             hand_txt (str): The raw poker hand text as a string.
 
         Returns:
-            dict: A dictionary representing the card on the River.
+            dict: A dictionary representing the card on the River(river_card).
         """
         river_match = re.search(pattern=patterns.RIVER_PATTERN, string=hand_txt, flags=re.UNICODE)
         card = river_match.group(1) if river_match else None
         return {"river_card": card}
 
     def parse_actions(self, actions_txt: str) -> list:
         """
         Parse the actions text from a poker hand history for a specific street
         and return a list of dictionaries containing the actions.
 
         Parameters:
             actions_txt (str): The raw actions text for a specific street.
 
         Returns:
-            list: A list of dictionaries, each representing an action.
+            list: A list of dictionaries(player, action, amount), each representing an action.
         """
         actions = re.findall(pattern=patterns.ACTION_PATTERN, string=actions_txt)
         parsed_actions = [{'player': player.strip(), 'action': action_type, 'amount': self.to_float(amount)}
                           for player, action_type, amount in actions]
         return parsed_actions
 
-    def extract_actions(self, hand_txt: str):
+    def extract_actions(self, hand_txt: str) -> dict:
         """
         Extract the actions information from a poker hand history and return as a nested dictionary.
+
         Parameters:
             hand_txt (str): The raw poker hand text as a string.
 
         Returns:
-            dict: A dictionary containing all the actions extracted from the poker hand history.
+            dict: A dictionary containing all the actions extracted for each street
+            of the poker hand history(preflop, flop, turn, river).
         """
         actions_dict = {
             street: self.parse_actions(re.search(pattern, string=hand_txt, flags=re.DOTALL).group(1))
             if re.search(pattern, string=hand_txt, flags=re.DOTALL) else []
             for pattern, street in zip(patterns.STREET_ACTION_PATTERNS, ['preflop', 'flop', 'turn', 'river'])}
         return actions_dict
 
@@ -254,57 +353,61 @@
         """
         Extract the showdown information from a poker hand history.
 
         Parameters:
             hand_txt (str): The raw poker hand text as a string.
 
         Returns:
-            showdown_info: A dict of dictionaries, each containing the player's shown cards.
+            dict: A dict containing the showdown information extracted
+            from the poker hand history(first_card, second_card).
         """
         showdown_info = {player.strip(): {"first_card": card1, "second_card": card2}
                          for player, card1, card2 in re.findall(pattern=patterns.SHOWDOWN_PATTERN, string=hand_txt)}
         return showdown_info
 
     def extract_winners(self, hand_txt: str) -> dict:
         """
         Extract the winners information from a poker hand history and return it as a nested dictionary.
 
         Parameters:
             hand_txt (str): The raw poker hand text as a string.
 
         Returns:
-            dict: A nested dictionary with pl_names as keys, each containing a dictionary with the amount and pot type.
+            dict: A dictionary containing the winners information extracted
+            from the poker hand history(winner_name(amount, pot_type)).
         """
         winners_info = {winner: {"amount": self.to_float(amount), "pot_type": pot_type}
                         for winner, amount, pot_type in re.findall(pattern=patterns.WINNERS_PATTERN, string=hand_txt)}
         return winners_info
 
     @staticmethod
     def extract_hand_id(hand_txt: str) -> dict:
         """
         Extract the hand id information from a poker hand history.
 
         Parameters:
             hand_txt (str): The raw poker hand text as a string.
 
         Returns:
-            dict: A dictionary containing the hand id extracted from the poker hand history.
+            dict: A dictionary containing the hand id extracted from the poker hand history(hand_id).
         """
         hand_id = re.search(pattern=patterns.HAND_ID_PATTERN, string=hand_txt).group(1)
         return {"hand_id": hand_id}
 
     def parse_hand(self, hand_txt: str) -> dict:
         """
         Extract all information from a poker hand history and return as a dictionary.
 
         Parameters:
             hand_txt (str): The raw poker hand text as a string.
 
         Returns:
-            dict: A dictionary containing all the information extracted from the poker hand history.
+            dict: A dictionary containing all the information extracted from the poker hand history
+        (hand_id, datetime, game_type, buy_in, blinds, level, max_players, button_seat, table_name, table_ident,
+        players, hero_hand, postings, actions, flop, turn, river, showdown, winners).
         """
         hand_history_dict = {
             "hand_id": self.extract_hand_id(hand_txt)["hand_id"],
             "datetime": self.extract_datetime(hand_txt)["datetime"],
             "game_type": self.extract_game_type(hand_txt)["game_type"],
             "buy_in": self.extract_buy_in(hand_txt),
             "blinds": self.extract_blinds(hand_txt),
@@ -320,7 +423,20 @@
             "flop": self.extract_flop(hand_txt),
             "turn": self.extract_turn(hand_txt),
             "river": self.extract_river(hand_txt),
             "showdown": self.extract_showdown(hand_txt),
             "winners": self.extract_winners(hand_txt)
         }
         return hand_history_dict
+
+    def parse_to_json(self, history_path: str, destination_path: str) -> None:
+        """
+        Parse a poker hand history to a JSON format.
+
+        Parameters:
+            history_path (str): The path to the poker hand history file.
+            destination_path (str): The path to save the JSON file.
+        """
+        hand_text = self.get_raw_text(history_path)
+        hand_info = self.parse_hand(hand_text)
+        with open(destination_path, "w", encoding="utf-8") as file:
+            json.dump(hand_info, file, indent=4)
```

### Comparing `pkrhistoryparser-1.0.1/pkrhistoryparser/patterns/winamax.py` & `pkrhistoryparser-1.1.0/pkrhistoryparser/patterns/winamax.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This module contains regular expressions used to parse Winamax hand histories.
+"""
+
 PLAYER_PATTERN = r"Seat (\d+): ([\w\s.\-&]{3,12}) \((\d+)(?:, ([\d\.]+)\D)?"
 BLINDS_PATTERN = r"(\n[\w\s\-&.]{3,12})\s+posts\s+(small blind|big blind|ante)\s+([\d.,]+)"
 NORMAL_BUY_IN_PATTERN = r"buyIn:\s+([\d.,]+)€\s+\+\s+([\d.,]+)€"
 KO_BUY_IN_PATTERN = r"buyIn: ([\d.,]+)€ \+ ([\d.,]+)€ \+ ([\d.,]+)€"
 FREE_ROLL_PATTERN = r"buyIn: Free"
 DATETIME_PATTERN = r"- (\d{4}/\d{2}/\d{2} \d{2}:\d{2}:\d{2}) UTC"
 TOURNAMENT_BLINDS_PATTERN = r"\((\d+)/(\d+)/(\d+)\)"
```

### Comparing `pkrhistoryparser-1.0.1/pkrhistoryparser/pkrhistoryparser.egg-info/PKG-INFO` & `pkrhistoryparser-1.1.0/pkrhistoryparser/pkrhistoryparser.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrhistoryparser
-Version: 1.0.1
+Version: 1.1.0
 Summary: A poker package to parse Hand histories into json objects
 Home-page: https://github.com/manggy94/PokerHistoryParser
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/manggy94/PokerHistoryParser/issues
 Platform: UNKNOWN
```

### Comparing `pkrhistoryparser-1.0.1/requirements.txt` & `pkrhistoryparser-1.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `pkrhistoryparser-1.0.1/setup.py` & `pkrhistoryparser-1.1.0/setup.py`

 * *Files identical despite different names*

