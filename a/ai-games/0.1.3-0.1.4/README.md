# Comparing `tmp/ai_games-0.1.3.tar.gz` & `tmp/ai_games-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_games-0.1.3.tar", last modified: Thu May 23 15:31:46 2024, max compression
+gzip compressed data, was "ai_games-0.1.4.tar", last modified: Thu May 23 16:09:02 2024, max compression
```

## Comparing `ai_games-0.1.3.tar` & `ai_games-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 15:31:46.230000 ai_games-0.1.3/
--rwx------   0 benjamin   (501) staff       (20)     1601 2024-05-23 15:31:46.300000 ai_games-0.1.3/PKG-INFO
--rwx------   0 benjamin   (501) staff       (20)     1191 2024-05-23 14:30:53.000000 ai_games-0.1.3/README.md
-drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 15:31:46.240000 ai_games-0.1.3/ai_games/
--rwx------   0 benjamin   (501) staff       (20)       81 2024-05-23 15:07:56.000000 ai_games-0.1.3/ai_games/__init__.py
--rwx------   0 benjamin   (501) staff       (20)    11161 2024-05-23 14:11:18.000000 ai_games-0.1.3/ai_games/connect4.py
-drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 15:31:46.240000 ai_games-0.1.3/ai_games.egg-info/
--rwx------   0 benjamin   (501) staff       (20)     1601 2024-05-23 15:31:46.000000 ai_games-0.1.3/ai_games.egg-info/PKG-INFO
--rwx------   0 benjamin   (501) staff       (20)      219 2024-05-23 15:31:46.000000 ai_games-0.1.3/ai_games.egg-info/SOURCES.txt
--rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 15:31:46.000000 ai_games-0.1.3/ai_games.egg-info/dependency_links.txt
--rwx------   0 benjamin   (501) staff       (20)        7 2024-05-23 15:31:46.000000 ai_games-0.1.3/ai_games.egg-info/requires.txt
--rwx------   0 benjamin   (501) staff       (20)        9 2024-05-23 15:31:46.000000 ai_games-0.1.3/ai_games.egg-info/top_level.txt
--rwx------   0 benjamin   (501) staff       (20)       38 2024-05-23 15:31:46.310000 ai_games-0.1.3/setup.cfg
--rwx------   0 benjamin   (501) staff       (20)      723 2024-05-23 15:31:33.000000 ai_games-0.1.3/setup.py
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 16:09:02.040000 ai_games-0.1.4/
+-rwx------   0 benjamin   (501) staff       (20)     1601 2024-05-23 16:09:02.210000 ai_games-0.1.4/PKG-INFO
+-rwx------   0 benjamin   (501) staff       (20)     1191 2024-05-23 14:30:53.000000 ai_games-0.1.4/README.md
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 16:09:02.050000 ai_games-0.1.4/ai_games/
+-rwx------   0 benjamin   (501) staff       (20)       81 2024-05-23 15:07:56.000000 ai_games-0.1.4/ai_games/__init__.py
+-rwx------   0 benjamin   (501) staff       (20)    11450 2024-05-23 16:08:04.000000 ai_games-0.1.4/ai_games/connect4.py
+drwx------   0 benjamin   (501) staff       (20)        0 2024-05-23 16:09:02.060000 ai_games-0.1.4/ai_games.egg-info/
+-rwx------   0 benjamin   (501) staff       (20)     1601 2024-05-23 16:09:01.000000 ai_games-0.1.4/ai_games.egg-info/PKG-INFO
+-rwx------   0 benjamin   (501) staff       (20)      219 2024-05-23 16:09:02.000000 ai_games-0.1.4/ai_games.egg-info/SOURCES.txt
+-rwx------   0 benjamin   (501) staff       (20)        1 2024-05-23 16:09:01.000000 ai_games-0.1.4/ai_games.egg-info/dependency_links.txt
+-rwx------   0 benjamin   (501) staff       (20)        7 2024-05-23 16:09:01.000000 ai_games-0.1.4/ai_games.egg-info/requires.txt
+-rwx------   0 benjamin   (501) staff       (20)        9 2024-05-23 16:09:01.000000 ai_games-0.1.4/ai_games.egg-info/top_level.txt
+-rwx------   0 benjamin   (501) staff       (20)       38 2024-05-23 16:09:02.210000 ai_games-0.1.4/setup.cfg
+-rwx------   0 benjamin   (501) staff       (20)      723 2024-05-23 16:08:53.000000 ai_games-0.1.4/setup.py
```

### Comparing `ai_games-0.1.3/PKG-INFO` & `ai_games-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai_games
-Version: 0.1.3
+Version: 0.1.4
 Summary: AI Games: Collection of interactive games with AI opponents for Python.
 Home-page: https://github.com/bzm10/ai_games
 Author: Coding with BM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ai_games-0.1.3/README.md` & `ai_games-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ai_games-0.1.3/ai_games/connect4.py` & `ai_games-0.1.4/ai_games/connect4.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,27 +14,34 @@
 
 class Connect4Game:
     BLUE = (0, 0, 255)
     BLACK = (0, 0, 0)
     RED = (255, 0, 0)
     YELLOW = (255, 255, 0)
 
-    def __init__(self, config=Config()):
+    def __init__(self, config=Config(), starting_player="player"):
         self.config = config
         self.board = self.create_board()
         self.SQUARESIZE = 100
         self.width = self.config.COLUMN_COUNT * self.SQUARESIZE
         self.height = (self.config.ROW_COUNT + 1) * self.SQUARESIZE
         self.size = (self.width, self.height)
         self.RADIUS = int(self.SQUARESIZE / 2 - 5)
         self.screen = None
         self.myfont = None
-        self.turn = random.randint(0, 1)
         self.game_over = False
 
+        # Set the starting player
+        if starting_player == "player":
+            self.turn = 0
+        elif starting_player == "ai":
+            self.turn = 1
+        else:
+            raise ValueError("Invalid starting player. Choose 'player' or 'ai'.")
+
     def create_board(self):
         return np.zeros((self.config.ROW_COUNT, self.config.COLUMN_COUNT))
 
     def drop_piece(self, board, row, col, piece):
         board[row][col] = piece
 
     def is_valid_location(self, board, col):
@@ -170,16 +177,14 @@
             self.drop_piece(temp_board, row, col, piece)
             score = self.score_position(temp_board, piece)
             if score > best_score:
                 best_score = score
                 best_col = col
         return best_col
 
-    # ... continued from the previous code snippet ...
-
     def draw_board(self, board):
         for c in range(self.config.COLUMN_COUNT):
             for r in range(self.config.ROW_COUNT):
                 pygame.draw.rect(self.screen, self.BLUE, (c * self.SQUARESIZE, r * self.SQUARESIZE + self.SQUARESIZE, self.SQUARESIZE, self.SQUARESIZE))
                 pygame.draw.circle(self.screen, self.BLACK, (int(c * self.SQUARESIZE + self.SQUARESIZE / 2), int(r * self.SQUARESIZE + self.SQUARESIZE + self.SQUARESIZE / 2)), self.RADIUS)
         for c in range(self.config.COLUMN_COUNT):
             for r in range(self.config.ROW_COUNT):        
@@ -215,15 +220,15 @@
                     col = int(math.floor(posx / self.SQUARESIZE))
 
                     if self.is_valid_location(self.board, col):
                         row = self.get_next_open_row(self.board, col)
                         self.drop_piece(self.board, row, col, self.config.PLAYER_PIECE)
 
                         if self.winning_move(self.board, self.config.PLAYER_PIECE):
-                            label = self.myfont.render("Player 1 wins!!", 1, self.RED)
+                            label = self.myfont.render("You win!!", 1, self.RED)
                             self.screen.blit(label, (40, 10))
                             self.game_over = True
 
                         self.turn += 1
                         self.turn = self.turn % 2
 
                         self.draw_board(self.board)
@@ -232,24 +237,25 @@
             if self.turn == 1 and not self.game_over:
                 col, minimax_score = self.minimax(self.board, 5, -math.inf, math.inf, True)
 
                 if self.is_valid_location(self.board, col):
                     row = self.get_next_open_row(self.board, col)
                     self.drop_piece(self.board, row, col, self.config.AI_PIECE)
 
-                    if self.winning_move(self.board, self.config.AI_PIECE):
-                        label = self.myfont.render("Player 2 wins!!", 1, self.YELLOW)
+                    if self.winning_move(self.board, self.config.AI_PIECE): 
+                        label = self.myfont.render("AI wins!!", 1, self.YELLOW)
                         self.screen.blit(label, (40, 10))
                         self.game_over = True
 
                     self.draw_board(self.board)
                     pygame.display.update()
 
                     self.turn += 1
                     self.turn = self.turn % 2
 
             if self.game_over:
                 pygame.time.wait(3000)
 
 if __name__ == "__main__":
-    game = Connect4Game()
+    starting_player = input("Who starts first? (player/ai): ").strip().lower()
+    game = Connect4Game(starting_player=starting_player)
     game.play()
```

### Comparing `ai_games-0.1.3/ai_games.egg-info/PKG-INFO` & `ai_games-0.1.4/ai_games.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai_games
-Version: 0.1.3
+Version: 0.1.4
 Summary: AI Games: Collection of interactive games with AI opponents for Python.
 Home-page: https://github.com/bzm10/ai_games
 Author: Coding with BM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ai_games-0.1.3/setup.py` & `ai_games-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='ai_games',
-    version='0.1.3',
+    version='0.1.4',
     author='Coding with BM',
     description='AI Games: Collection of interactive games with AI opponents for Python.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/bzm10/ai_games',
     packages=find_packages(),
     install_requires=[
```

