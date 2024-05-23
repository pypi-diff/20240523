# Comparing `tmp/cardstock-0.99.5.tar.gz` & `tmp/cardstock-0.99.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardstock-0.99.5.tar", last modified: Tue Jan 30 20:25:14 2024, max compression
+gzip compressed data, was "cardstock-0.99.6.tar", last modified: Thu May 23 19:48:17 2024, max compression
```

## Comparing `cardstock-0.99.5.tar` & `cardstock-0.99.6.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 benjie     (501) staff       (20)        0 2024-01-30 20:25:14.074550 cardstock-0.99.5/
--rw-r--r--   0 benjie     (501) staff       (20)    16725 2021-11-02 20:40:58.000000 cardstock-0.99.5/LICENSE
--rw-r--r--   0 benjie     (501) staff       (20)     7631 2024-01-30 20:25:14.074502 cardstock-0.99.5/PKG-INFO
--rw-r--r--   0 benjie     (501) staff       (20)     6895 2024-01-30 20:21:39.000000 cardstock-0.99.5/README.md
-drwxr-xr-x   0 benjie     (501) staff       (20)        0 2024-01-30 20:25:14.066933 cardstock-0.99.5/cardstock/
--rw-r--r--   0 benjie     (501) staff       (20)     1715 2023-10-19 22:56:17.000000 cardstock-0.99.5/cardstock/CardStock_Designer_mac.spec
--rw-r--r--   0 benjie     (501) staff       (20)     1613 2021-11-02 20:40:58.000000 cardstock-0.99.5/cardstock/CardStock_Viewer_mac.spec
--rw-r--r--   0 benjie     (501) staff       (20)      521 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/__init__.py
--rw-r--r--   0 benjie     (501) staff       (20)      418 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/__main__.py
--rw-r--r--   0 benjie     (501) staff       (20)     6207 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/allCodeWindow.py
--rw-r--r--   0 benjie     (501) staff       (20)    14901 2023-10-19 17:00:19.000000 cardstock-0.99.5/cardstock/analyzer.py
--rw-r--r--   0 benjie     (501) staff       (20)    17077 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/appCommands.py
--rw-r--r--   0 benjie     (501) staff       (20)     4627 2023-10-19 23:02:59.000000 cardstock-0.99.5/cardstock/build.py
--rw-r--r--   0 benjie     (501) staff       (20)     5299 2023-10-19 17:00:19.000000 cardstock-0.99.5/cardstock/cardstockFrameParts.py
--rw-r--r--   0 benjie     (501) staff       (20)     6737 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/codeInspector.py
--rw-r--r--   0 benjie     (501) staff       (20)    23974 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/codeInspectorMulti.py
--rw-r--r--   0 benjie     (501) staff       (20)     5455 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/codeRunnerThread.py
--rw-r--r--   0 benjie     (501) staff       (20)    14906 2023-10-19 17:00:19.000000 cardstock-0.99.5/cardstock/consoleWindow.py
--rw-r--r--   0 benjie     (501) staff       (20)    19831 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/controlPanel.py
--rw-r--r--   0 benjie     (501) staff       (20)    57867 2024-01-30 20:21:39.000000 cardstock-0.99.5/cardstock/designer.py
--rw-r--r--   0 benjie     (501) staff       (20)   141197 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/embeddedImages.py
--rw-r--r--   0 benjie     (501) staff       (20)     3956 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/errorListWindow.py
-drwxr-xr-x   0 benjie     (501) staff       (20)        0 2024-01-30 20:25:14.073238 cardstock-0.99.5/cardstock/examples/
--rw-r--r--   0 benjie     (501) staff       (20)     7829 2023-10-19 17:00:19.000000 cardstock-0.99.5/cardstock/examples/Asteroids.cds
--rw-r--r--   0 benjie     (501) staff       (20)     4787 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Browser.cds
--rw-r--r--   0 benjie     (501) staff       (20)     9975 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Calculator.cds
--rw-r--r--   0 benjie     (501) staff       (20)     4003 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Catch.cds
--rw-r--r--   0 benjie     (501) staff       (20)     5667 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Diary.cds
--rw-r--r--   0 benjie     (501) staff       (20)     7872 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Dice-stats.cds
--rw-r--r--   0 benjie     (501) staff       (20)     4422 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Dice.cds
--rw-r--r--   0 benjie     (501) staff       (20)     3451 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Factor.cds
--rw-r--r--   0 benjie     (501) staff       (20)    33761 2022-12-28 00:38:48.000000 cardstock-0.99.5/cardstock/examples/Fifteen.cds
--rw-r--r--   0 benjie     (501) staff       (20)     4907 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Flappy.cds
--rw-r--r--   0 benjie     (501) staff       (20)     7885 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Graph.cds
--rw-r--r--   0 benjie     (501) staff       (20)     8049 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Guess.cds
--rw-r--r--   0 benjie     (501) staff       (20)     9259 2022-12-28 00:38:48.000000 cardstock-0.99.5/cardstock/examples/Hanoi.cds
--rw-r--r--   0 benjie     (501) staff       (20)    29879 2023-10-19 17:01:18.000000 cardstock-0.99.5/cardstock/examples/Logo.cds
--rw-r--r--   0 benjie     (501) staff       (20)     3083 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Magic.cds
--rw-r--r--   0 benjie     (501) staff       (20)    16438 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Mastermind.cds
--rw-r--r--   0 benjie     (501) staff       (20)     9318 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Maze.cds
--rw-r--r--   0 benjie     (501) staff       (20)    25585 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Morph.cds
--rw-r--r--   0 benjie     (501) staff       (20)    22300 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Navigation.cds
--rw-r--r--   0 benjie     (501) staff       (20)     8298 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Number-puzzle.cds
--rw-r--r--   0 benjie     (501) staff       (20)     4042 2023-10-19 17:01:18.000000 cardstock-0.99.5/cardstock/examples/Pong.cds
--rw-r--r--   0 benjie     (501) staff       (20)     2032 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Requests.cds
--rw-r--r--   0 benjie     (501) staff       (20)     5108 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Scene.cds
--rw-r--r--   0 benjie     (501) staff       (20)     3328 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Serial.cds
--rw-r--r--   0 benjie     (501) staff       (20)    10074 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Snake.cds
--rw-r--r--   0 benjie     (501) staff       (20)     8889 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Tanks.cds
--rw-r--r--   0 benjie     (501) staff       (20)    12616 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/examples/Tetris.cds
--rw-r--r--   0 benjie     (501) staff       (20)    14073 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/TicTacToe.cds
--rw-r--r--   0 benjie     (501) staff       (20)    84929 2022-09-14 20:33:21.000000 cardstock-0.99.5/cardstock/examples/Welcome.cds
--rw-r--r--   0 benjie     (501) staff       (20)    24364 2022-12-28 00:38:48.000000 cardstock-0.99.5/cardstock/examples/Wordel.cds
--rw-r--r--   0 benjie     (501) staff       (20)   103912 2021-11-02 20:40:58.000000 cardstock-0.99.5/cardstock/examples/click.wav
--rw-r--r--   0 benjie     (501) staff       (20)    17826 2021-11-02 20:40:58.000000 cardstock-0.99.5/cardstock/examples/puff.wav
--rw-r--r--   0 benjie     (501) staff       (20)    20544 2021-11-02 20:40:58.000000 cardstock-0.99.5/cardstock/examples/ship-off.png
--rw-r--r--   0 benjie     (501) staff       (20)    20749 2021-11-02 20:40:58.000000 cardstock-0.99.5/cardstock/examples/ship-on.png
--rw-r--r--   0 benjie     (501) staff       (20)    16127 2022-02-18 23:23:29.000000 cardstock-0.99.5/cardstock/examples/simple-red-apple.png
--rw-r--r--   0 benjie     (501) staff       (20)   451172 2021-11-02 20:40:58.000000 cardstock-0.99.5/cardstock/examples/yay.wav
--rw-r--r--   0 benjie     (501) staff       (20)     8247 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/findEngineDesigner.py
--rw-r--r--   0 benjie     (501) staff       (20)     6255 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/findEngineViewer.py
--rw-r--r--   0 benjie     (501) staff       (20)     1929 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/flippedGCDC.py
--rw-r--r--   0 benjie     (501) staff       (20)     3391 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/generator.py
--rw-r--r--   0 benjie     (501) staff       (20)   103190 2024-01-30 20:21:39.000000 cardstock-0.99.5/cardstock/helpData.py
--rw-r--r--   0 benjie     (501) staff       (20)    35857 2024-01-30 20:21:39.000000 cardstock-0.99.5/cardstock/helpDialogs.py
--rw-r--r--   0 benjie     (501) staff       (20)     1403 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/imageFactory.py
--rw-r--r--   0 benjie     (501) staff       (20)     7614 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/mediaSearchDialogs.py
--rw-r--r--   0 benjie     (501) staff       (20)    22848 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/migrations.py
--rw-r--r--   0 benjie     (501) staff       (20)    24777 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/propertyInspector.py
--rw-r--r--   0 benjie     (501) staff       (20)    13307 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/pythonEditor.py
--rw-r--r--   0 benjie     (501) staff       (20)     1792 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/resourcePathManager.py
--rw-r--r--   0 benjie     (501) staff       (20)    47879 2024-01-30 20:21:39.000000 cardstock-0.99.5/cardstock/runner.py
--rw-r--r--   0 benjie     (501) staff       (20)     1797 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/sanitizer.py
--rw-r--r--   0 benjie     (501) staff       (20)     6625 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/simpleListBox.py
--rw-r--r--   0 benjie     (501) staff       (20)    25803 2024-01-30 20:21:39.000000 cardstock-0.99.5/cardstock/stackExporter.py
--rw-r--r--   0 benjie     (501) staff       (20)    52175 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/stackManager.py
--rw-r--r--   0 benjie     (501) staff       (20)     4747 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/stackModel.py
--rw-r--r--   0 benjie     (501) staff       (20)     3219 2024-01-30 20:21:39.000000 cardstock-0.99.5/cardstock/standalone.py
--rw-r--r--   0 benjie     (501) staff       (20)    38367 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/tools.py
--rw-r--r--   0 benjie     (501) staff       (20)    12828 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/uiButton.py
--rw-r--r--   0 benjie     (501) staff       (20)    18732 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/uiCard.py
--rw-r--r--   0 benjie     (501) staff       (20)    12370 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/uiGroup.py
--rw-r--r--   0 benjie     (501) staff       (20)     7536 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/uiImage.py
--rw-r--r--   0 benjie     (501) staff       (20)    25234 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/uiShape.py
--rw-r--r--   0 benjie     (501) staff       (20)    12212 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/uiTextBase.py
--rw-r--r--   0 benjie     (501) staff       (20)    14645 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/uiTextField.py
--rw-r--r--   0 benjie     (501) staff       (20)     8698 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/uiTextLabel.py
--rw-r--r--   0 benjie     (501) staff       (20)    71647 2023-10-19 17:00:19.000000 cardstock-0.99.5/cardstock/uiView.py
--rw-r--r--   0 benjie     (501) staff       (20)     8654 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/uiWebView.py
--rw-r--r--   0 benjie     (501) staff       (20)    10190 2023-05-28 23:12:56.000000 cardstock-0.99.5/cardstock/variablesWindow.py
--rw-r--r--   0 benjie     (501) staff       (20)      360 2024-01-30 20:21:39.000000 cardstock-0.99.5/cardstock/version.py
--rw-r--r--   0 benjie     (501) staff       (20)    26397 2024-01-30 20:21:39.000000 cardstock-0.99.5/cardstock/viewer.py
-drwxr-xr-x   0 benjie     (501) staff       (20)        0 2024-01-30 20:25:14.074194 cardstock-0.99.5/cardstock.egg-info/
--rw-r--r--   0 benjie     (501) staff       (20)     7631 2024-01-30 20:25:14.000000 cardstock-0.99.5/cardstock.egg-info/PKG-INFO
--rw-r--r--   0 benjie     (501) staff       (20)     2793 2024-01-30 20:25:14.000000 cardstock-0.99.5/cardstock.egg-info/SOURCES.txt
--rw-r--r--   0 benjie     (501) staff       (20)        1 2024-01-30 20:25:14.000000 cardstock-0.99.5/cardstock.egg-info/dependency_links.txt
--rw-r--r--   0 benjie     (501) staff       (20)      102 2024-01-30 20:25:14.000000 cardstock-0.99.5/cardstock.egg-info/entry_points.txt
--rw-r--r--   0 benjie     (501) staff       (20)       68 2024-01-30 20:25:14.000000 cardstock-0.99.5/cardstock.egg-info/requires.txt
--rw-r--r--   0 benjie     (501) staff       (20)       10 2024-01-30 20:25:14.000000 cardstock-0.99.5/cardstock.egg-info/top_level.txt
--rw-r--r--   0 benjie     (501) staff       (20)      103 2021-11-02 20:40:58.000000 cardstock-0.99.5/pyproject.toml
--rw-r--r--   0 benjie     (501) staff       (20)     1019 2024-01-30 20:25:14.074768 cardstock-0.99.5/setup.cfg
+drwxr-xr-x   0 benjie     (501) staff       (20)        0 2024-05-23 19:48:17.079574 cardstock-0.99.6/
+-rw-r--r--   0 benjie     (501) staff       (20)    16725 2021-11-02 20:40:58.000000 cardstock-0.99.6/LICENSE
+-rw-r--r--   0 benjie     (501) staff       (20)     8533 2024-05-23 19:48:17.079422 cardstock-0.99.6/PKG-INFO
+-rw-r--r--   0 benjie     (501) staff       (20)     7797 2024-05-23 19:47:28.000000 cardstock-0.99.6/README.md
+drwxr-xr-x   0 benjie     (501) staff       (20)        0 2024-05-23 19:48:17.069597 cardstock-0.99.6/cardstock/
+-rw-r--r--   0 benjie     (501) staff       (20)     1715 2023-10-19 22:56:17.000000 cardstock-0.99.6/cardstock/CardStock_Designer_mac.spec
+-rw-r--r--   0 benjie     (501) staff       (20)     1613 2021-11-02 20:40:58.000000 cardstock-0.99.6/cardstock/CardStock_Viewer_mac.spec
+-rw-r--r--   0 benjie     (501) staff       (20)      521 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/__init__.py
+-rw-r--r--   0 benjie     (501) staff       (20)      418 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/__main__.py
+-rw-r--r--   0 benjie     (501) staff       (20)     6207 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/allCodeWindow.py
+-rw-r--r--   0 benjie     (501) staff       (20)    15371 2024-05-21 05:22:24.000000 cardstock-0.99.6/cardstock/analyzer.py
+-rw-r--r--   0 benjie     (501) staff       (20)    16943 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/appCommands.py
+-rw-r--r--   0 benjie     (501) staff       (20)     4627 2023-10-19 23:02:59.000000 cardstock-0.99.6/cardstock/build.py
+-rw-r--r--   0 benjie     (501) staff       (20)     5299 2023-10-19 17:00:19.000000 cardstock-0.99.6/cardstock/cardstockFrameParts.py
+-rw-r--r--   0 benjie     (501) staff       (20)     6793 2024-05-21 05:22:24.000000 cardstock-0.99.6/cardstock/codeInspector.py
+-rw-r--r--   0 benjie     (501) staff       (20)    24120 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/codeInspectorMulti.py
+-rw-r--r--   0 benjie     (501) staff       (20)     5455 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/codeRunnerThread.py
+-rw-r--r--   0 benjie     (501) staff       (20)    14906 2023-10-19 17:00:19.000000 cardstock-0.99.6/cardstock/consoleWindow.py
+-rw-r--r--   0 benjie     (501) staff       (20)    19840 2024-05-21 05:22:24.000000 cardstock-0.99.6/cardstock/controlPanel.py
+-rw-r--r--   0 benjie     (501) staff       (20)    58408 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/designer.py
+-rw-r--r--   0 benjie     (501) staff       (20)      625 2024-05-21 05:22:24.000000 cardstock-0.99.6/cardstock/easing.py
+-rw-r--r--   0 benjie     (501) staff       (20)   142630 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/embeddedImages.py
+-rw-r--r--   0 benjie     (501) staff       (20)     4274 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/errorListWindow.py
+drwxr-xr-x   0 benjie     (501) staff       (20)        0 2024-05-23 19:48:17.078137 cardstock-0.99.6/cardstock/examples/
+-rw-r--r--   0 benjie     (501) staff       (20)     7914 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/examples/Asteroids.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     4787 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Browser.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     9975 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Calculator.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     4003 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Catch.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     5751 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/examples/Diary.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     7872 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Dice-stats.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     4422 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Dice.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     3451 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Factor.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    34464 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/examples/Fifteen.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     4907 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Flappy.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     7885 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Graph.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     8049 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Guess.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     6002 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/examples/Hanoi.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    18325 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/examples/Logo.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     3083 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Magic.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    16438 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Mastermind.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     9318 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Maze.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    25585 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Morph.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    22300 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Navigation.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     8298 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Number-puzzle.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     4042 2023-10-19 17:01:18.000000 cardstock-0.99.6/cardstock/examples/Pong.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     2032 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Requests.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     5397 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/examples/Scene.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     3328 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Serial.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    10074 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Snake.cds
+-rw-r--r--   0 benjie     (501) staff       (20)     8889 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Tanks.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    12616 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/examples/Tetris.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    14073 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/TicTacToe.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    84929 2022-09-14 20:33:21.000000 cardstock-0.99.6/cardstock/examples/Welcome.cds
+-rw-r--r--   0 benjie     (501) staff       (20)    24364 2022-12-28 00:38:48.000000 cardstock-0.99.6/cardstock/examples/Wordel.cds
+-rw-r--r--   0 benjie     (501) staff       (20)   103912 2021-11-02 20:40:58.000000 cardstock-0.99.6/cardstock/examples/click.wav
+-rw-r--r--   0 benjie     (501) staff       (20)    17826 2021-11-02 20:40:58.000000 cardstock-0.99.6/cardstock/examples/puff.wav
+-rw-r--r--   0 benjie     (501) staff       (20)    20544 2021-11-02 20:40:58.000000 cardstock-0.99.6/cardstock/examples/ship-off.png
+-rw-r--r--   0 benjie     (501) staff       (20)    20749 2021-11-02 20:40:58.000000 cardstock-0.99.6/cardstock/examples/ship-on.png
+-rw-r--r--   0 benjie     (501) staff       (20)    16127 2022-02-18 23:23:29.000000 cardstock-0.99.6/cardstock/examples/simple-red-apple.png
+-rw-r--r--   0 benjie     (501) staff       (20)   451172 2021-11-02 20:40:58.000000 cardstock-0.99.6/cardstock/examples/yay.wav
+-rw-r--r--   0 benjie     (501) staff       (20)     8238 2024-05-21 05:22:24.000000 cardstock-0.99.6/cardstock/findEngineDesigner.py
+-rw-r--r--   0 benjie     (501) staff       (20)     6255 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/findEngineViewer.py
+-rw-r--r--   0 benjie     (501) staff       (20)     1929 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/flippedGCDC.py
+-rw-r--r--   0 benjie     (501) staff       (20)     3391 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/generator.py
+-rw-r--r--   0 benjie     (501) staff       (20)   128227 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/helpData.py
+-rw-r--r--   0 benjie     (501) staff       (20)    13829 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/helpDataGen.py
+-rw-r--r--   0 benjie     (501) staff       (20)    35953 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/helpDialogs.py
+-rw-r--r--   0 benjie     (501) staff       (20)     1403 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/imageFactory.py
+-rw-r--r--   0 benjie     (501) staff       (20)     7614 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/mediaSearchDialogs.py
+-rw-r--r--   0 benjie     (501) staff       (20)    24269 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/migrations.py
+-rw-r--r--   0 benjie     (501) staff       (20)    25161 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/propertyInspector.py
+-rw-r--r--   0 benjie     (501) staff       (20)    13316 2024-05-21 05:22:24.000000 cardstock-0.99.6/cardstock/pythonEditor.py
+-rw-r--r--   0 benjie     (501) staff       (20)     1792 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/resourcePathManager.py
+-rw-r--r--   0 benjie     (501) staff       (20)    47727 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/runner.py
+-rw-r--r--   0 benjie     (501) staff       (20)     1797 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/sanitizer.py
+-rw-r--r--   0 benjie     (501) staff       (20)     6625 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/simpleListBox.py
+-rw-r--r--   0 benjie     (501) staff       (20)    25803 2024-01-30 20:21:39.000000 cardstock-0.99.6/cardstock/stackExporter.py
+-rw-r--r--   0 benjie     (501) staff       (20)    53308 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/stackManager.py
+-rw-r--r--   0 benjie     (501) staff       (20)     6010 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/stackModel.py
+-rw-r--r--   0 benjie     (501) staff       (20)     3219 2024-01-30 20:21:39.000000 cardstock-0.99.6/cardstock/standalone.py
+-rw-r--r--   0 benjie     (501) staff       (20)    38661 2024-05-21 05:22:24.000000 cardstock-0.99.6/cardstock/tools.py
+-rw-r--r--   0 benjie     (501) staff       (20)    12815 2024-05-21 05:22:24.000000 cardstock-0.99.6/cardstock/uiButton.py
+-rw-r--r--   0 benjie     (501) staff       (20)    18857 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/uiCard.py
+-rw-r--r--   0 benjie     (501) staff       (20)    12370 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/uiGroup.py
+-rw-r--r--   0 benjie     (501) staff       (20)     7536 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/uiImage.py
+-rw-r--r--   0 benjie     (501) staff       (20)    26867 2024-05-21 05:22:24.000000 cardstock-0.99.6/cardstock/uiShape.py
+-rw-r--r--   0 benjie     (501) staff       (20)    12637 2024-05-21 05:22:24.000000 cardstock-0.99.6/cardstock/uiTextBase.py
+-rw-r--r--   0 benjie     (501) staff       (20)    14645 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/uiTextField.py
+-rw-r--r--   0 benjie     (501) staff       (20)     8698 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/uiTextLabel.py
+-rw-r--r--   0 benjie     (501) staff       (20)    72183 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/uiView.py
+-rw-r--r--   0 benjie     (501) staff       (20)     8654 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/uiWebView.py
+-rw-r--r--   0 benjie     (501) staff       (20)    10190 2023-05-28 23:12:56.000000 cardstock-0.99.6/cardstock/variablesWindow.py
+-rw-r--r--   0 benjie     (501) staff       (20)      360 2024-05-21 05:22:24.000000 cardstock-0.99.6/cardstock/version.py
+-rw-r--r--   0 benjie     (501) staff       (20)    27030 2024-05-23 19:47:28.000000 cardstock-0.99.6/cardstock/viewer.py
+drwxr-xr-x   0 benjie     (501) staff       (20)        0 2024-05-23 19:48:17.079203 cardstock-0.99.6/cardstock.egg-info/
+-rw-r--r--   0 benjie     (501) staff       (20)     8533 2024-05-23 19:48:17.000000 cardstock-0.99.6/cardstock.egg-info/PKG-INFO
+-rw-r--r--   0 benjie     (501) staff       (20)     2842 2024-05-23 19:48:17.000000 cardstock-0.99.6/cardstock.egg-info/SOURCES.txt
+-rw-r--r--   0 benjie     (501) staff       (20)        1 2024-05-23 19:48:17.000000 cardstock-0.99.6/cardstock.egg-info/dependency_links.txt
+-rw-r--r--   0 benjie     (501) staff       (20)      102 2024-05-23 19:48:17.000000 cardstock-0.99.6/cardstock.egg-info/entry_points.txt
+-rw-r--r--   0 benjie     (501) staff       (20)       68 2024-05-23 19:48:17.000000 cardstock-0.99.6/cardstock.egg-info/requires.txt
+-rw-r--r--   0 benjie     (501) staff       (20)       10 2024-05-23 19:48:17.000000 cardstock-0.99.6/cardstock.egg-info/top_level.txt
+-rw-r--r--   0 benjie     (501) staff       (20)      103 2021-11-02 20:40:58.000000 cardstock-0.99.6/pyproject.toml
+-rw-r--r--   0 benjie     (501) staff       (20)     1019 2024-05-23 19:48:17.079769 cardstock-0.99.6/setup.cfg
```

### Comparing `cardstock-0.99.5/LICENSE` & `cardstock-0.99.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/PKG-INFO` & `cardstock-0.99.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: cardstock
-Version: 0.99.5
+Version: 0.99.6
 Summary: A simple development and rapid prototyping tool for quickly building multi-platform desktop programs and web apps.
 Home-page: https://github.com/benjie-git/CardStock/wiki
 Author: Ben Levitt
 Author-email: benjie@gmail.com
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.12,>=3.7
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrdict3
 Requires-Dist: wxpython
 Requires-Dist: PyInstaller
 Requires-Dist: requests
 Requires-Dist: simpleaudio
@@ -70,38 +70,62 @@
 * Stacks can only import additional modules, and export stacks that include them, when running from source.  Not when running from the prebuilt applications. (The prebuilt applications are built with a few additional libraries: requests, pyserial, and more could be added by request.)
 * Ironically, WebViews do not work in the web-based viewer on https://cardstock.run.
 * For performance reasons, currently mouse events don't propagate through all overlapping objects when running on the web-viewer, just the topmost object under the mouse, any containing groups, and the card.
 
 ## Requirements
 The prebuilt applications for Mac and Windows have no external dependencies.
 
-Running CardStock from source requires Python 3.7 or newer (3.11 recommended), and wxPython 4.1 or newer (wxPython 4.2.x recommended).
+Running CardStock from source requires Python 3.9 or newer (3.11 recommended), and wxPython 4.1 or newer (wxPython 4.2.x recommended).
 CardStock requires installing the python modules attrdict3(linux-only), wxpython, simpleaudio, PyInstaller, and requests.  
 For mp3 playback support, you'll need to install the lame package (mp3 decoder), and python's streamp3. 
-Note that Python 3.12 is currently incompatible with wxpython, and so will not run CardStock until
+Note that Python 3.12 is currently incompatible with released versions of wxpython, and so will not run CardStock until
 wxPython receives an update.
 
 ## Installation
 You can either:
 
 ### 1. Run it from source:
 1. install python3  # Note: Python3.12 is incompatible with wxpython, so 3.11 is recommended
 2. Linux-only: apt install libasound2-dev lame libwebkit2gtk-4.0-dev  # or equivalent on non-debian/ubuntu distros
-3. Linux-only: pip3 install attrdict3
-4. Mac-only: brew install lame
+3. Mac-only: brew install lame
+4. pip3 install attrdict3
 5. pip3 install wxpython PyInstaller simpleaudio requests  # note that wxpython can take a long time to build
-6. download or clone this repository
-7. run designer.py and viewer.py as desired
-8. optionally run build.py to create your own standalone applications for the Designer and Viewer applications.
+6. To include mp3 support: pip3 install streamp3
+
+   (Note that this may require setting LDFLAGS and CPPFLAGS to allow finding the lame header and library files.
+
+    You may need to run this as something like
+
+   `CPPFLAGS=-I/opt/homebrew/include LDFLAGS=-L/opt/homebrew/lib pip3 install streamp3` or 
+
+    `CPPFLAGS=-I/usr/local/include LDFLAGS=-L/usr/local/lib pip3 install streamp3`
+
+    depending on where the lame library was installed.)
+   
+7. download or clone this repository
+8. run designer.py and viewer.py as desired
+9. optionally run build.py to create your own standalone applications for the Designer and Viewer applications.
 
 ### 2. Install using pip/pypi:
 1. Linux-only: apt install libasound2-dev lame libwebkit2gtk-4.0-dev  # or equivalent on non-debian/ubuntu distros
 2. Mac-only: brew install lame
-3. pip3 install cardstock  # note that the dependency wxpython can take a very long time to build
-4. run using the newly installed commands cardstock and cardstock_viewer
+3. To include mp3 support: pip3 install streamp3
+
+   (Note that this may require setting LDFLAGS and CPPFLAGS to allow finding the lame header and library files.
+
+    You may need to run this as something like
+
+   `CPPFLAGS=-I/opt/homebrew/include LDFLAGS=-L/opt/homebrew/lib pip3 install streamp3` or 
+
+    `CPPFLAGS=-I/usr/local/include LDFLAGS=-L/usr/local/lib pip3 install streamp3`
+
+    depending on where the lame library was installed.)
+
+4. pip3 install cardstock  # note that the dependency wxpython can take a very long time to build
+5. run using the newly installed commands cardstock and cardstock_viewer
 
 ### 3. Or download the latest, pre-built CardStock application for Mac or Windows
 1. Download CardStock for Mac or Windows here: https://github.com/benjie-git/CardStock/releases/latest
 2. Note that the pre-built Windows app is not yet code-signed, so Windows will complain the first time you open the app. If a window appears saying "Windows protected your PC", click the More Info link at the end of the warning paragraph, and then the "Run Anyway" button that appears at the bottom of the window.
 
 
 ## Reference
```

### Comparing `cardstock-0.99.5/README.md` & `cardstock-0.99.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -49,38 +49,62 @@
 * Stacks can only import additional modules, and export stacks that include them, when running from source.  Not when running from the prebuilt applications. (The prebuilt applications are built with a few additional libraries: requests, pyserial, and more could be added by request.)
 * Ironically, WebViews do not work in the web-based viewer on https://cardstock.run.
 * For performance reasons, currently mouse events don't propagate through all overlapping objects when running on the web-viewer, just the topmost object under the mouse, any containing groups, and the card.
 
 ## Requirements
 The prebuilt applications for Mac and Windows have no external dependencies.
 
-Running CardStock from source requires Python 3.7 or newer (3.11 recommended), and wxPython 4.1 or newer (wxPython 4.2.x recommended).
+Running CardStock from source requires Python 3.9 or newer (3.11 recommended), and wxPython 4.1 or newer (wxPython 4.2.x recommended).
 CardStock requires installing the python modules attrdict3(linux-only), wxpython, simpleaudio, PyInstaller, and requests.  
 For mp3 playback support, you'll need to install the lame package (mp3 decoder), and python's streamp3. 
-Note that Python 3.12 is currently incompatible with wxpython, and so will not run CardStock until
+Note that Python 3.12 is currently incompatible with released versions of wxpython, and so will not run CardStock until
 wxPython receives an update.
 
 ## Installation
 You can either:
 
 ### 1. Run it from source:
 1. install python3  # Note: Python3.12 is incompatible with wxpython, so 3.11 is recommended
 2. Linux-only: apt install libasound2-dev lame libwebkit2gtk-4.0-dev  # or equivalent on non-debian/ubuntu distros
-3. Linux-only: pip3 install attrdict3
-4. Mac-only: brew install lame
+3. Mac-only: brew install lame
+4. pip3 install attrdict3
 5. pip3 install wxpython PyInstaller simpleaudio requests  # note that wxpython can take a long time to build
-6. download or clone this repository
-7. run designer.py and viewer.py as desired
-8. optionally run build.py to create your own standalone applications for the Designer and Viewer applications.
+6. To include mp3 support: pip3 install streamp3
+
+   (Note that this may require setting LDFLAGS and CPPFLAGS to allow finding the lame header and library files.
+
+    You may need to run this as something like
+
+   `CPPFLAGS=-I/opt/homebrew/include LDFLAGS=-L/opt/homebrew/lib pip3 install streamp3` or 
+
+    `CPPFLAGS=-I/usr/local/include LDFLAGS=-L/usr/local/lib pip3 install streamp3`
+
+    depending on where the lame library was installed.)
+   
+7. download or clone this repository
+8. run designer.py and viewer.py as desired
+9. optionally run build.py to create your own standalone applications for the Designer and Viewer applications.
 
 ### 2. Install using pip/pypi:
 1. Linux-only: apt install libasound2-dev lame libwebkit2gtk-4.0-dev  # or equivalent on non-debian/ubuntu distros
 2. Mac-only: brew install lame
-3. pip3 install cardstock  # note that the dependency wxpython can take a very long time to build
-4. run using the newly installed commands cardstock and cardstock_viewer
+3. To include mp3 support: pip3 install streamp3
+
+   (Note that this may require setting LDFLAGS and CPPFLAGS to allow finding the lame header and library files.
+
+    You may need to run this as something like
+
+   `CPPFLAGS=-I/opt/homebrew/include LDFLAGS=-L/opt/homebrew/lib pip3 install streamp3` or 
+
+    `CPPFLAGS=-I/usr/local/include LDFLAGS=-L/usr/local/lib pip3 install streamp3`
+
+    depending on where the lame library was installed.)
+
+4. pip3 install cardstock  # note that the dependency wxpython can take a very long time to build
+5. run using the newly installed commands cardstock and cardstock_viewer
 
 ### 3. Or download the latest, pre-built CardStock application for Mac or Windows
 1. Download CardStock for Mac or Windows here: https://github.com/benjie-git/CardStock/releases/latest
 2. Note that the pre-built Windows app is not yet code-signed, so Windows will complain the first time you open the app. If a window appears saying "Windows protected your PC", click the More Info link at the end of the warning paragraph, and then the "Run Anyway" button that appears at the bottom of the window.
 
 
 ## Reference
```

### Comparing `cardstock-0.99.5/cardstock/CardStock_Designer_mac.spec` & `cardstock-0.99.6/cardstock/CardStock_Designer_mac.spec`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/CardStock_Viewer_mac.spec` & `cardstock-0.99.6/cardstock/CardStock_Viewer_mac.spec`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/__init__.py` & `cardstock-0.99.6/cardstock/__init__.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/allCodeWindow.py` & `cardstock-0.99.6/cardstock/allCodeWindow.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/analyzer.py` & `cardstock-0.99.6/cardstock/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright Ben Levitt 2020-2023
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
 # of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import wx
 import ast
-import helpData
+import helpDataGen
 import threading
 import re
 import types
 
 ANALYSIS_TIMEOUT = 1000  # in ms
 NAME_CHARS = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789_"
 
@@ -29,51 +29,55 @@
         self.analysisTimer.Bind(wx.EVT_TIMER, self.OnAnalysisTimer)
         self.analysisPending = False
         self.analysisRunning = False
         self.disableAC = False
 
         self.varNames = set()
         self.funcNames = set()
-        self.globalVars = helpData.HelpDataGlobals.variables.keys()
-        self.globalFuncs = helpData.HelpDataGlobals.functions.keys()
-        self.builtinFuncs = helpData.HelpDataBuiltins.functions.keys()
+        self.globalVars = helpDataGen.HelpDataGlobals.variables.keys()
+        self.globalFuncs = helpDataGen.HelpDataGlobals.functions.keys()
+        self.builtinFuncs = helpDataGen.HelpDataBuiltins.functions.keys()
         self.cardNames = []
         self.objNames = {}
         self.objProps = {}
         self.objMethods = {}
         self.handlerVars = {}
         self.syntaxErrors = {}
         self.lastHandlerObj = None
         self.lastHandlerName = None
         self.notifyList = []
 
         for t in ["bool", "int", "float", "string", "list", "dictionary", "point", "size", "other"]: self.objProps[t] = []
         for t in ["bool", "int", "float", "string", "list", "dictionary", "point", "size", "other"]: self.objMethods[t] = []
 
         # Create list of known properties and methods for each object type
-        for cls in helpData.helpClasses:
+        for cls in helpDataGen.helpClasses:
             types = ["any"]
             types.extend(cls.types)
             for t in types:
                 self.objProps[t] = []
                 self.objMethods[t] = []
-        for cls in helpData.helpClasses:
+        for cls in helpDataGen.helpClasses:
             c = cls
             types = ["any", "object"]
             types.extend(cls.types)
             while c:
                 for t in types:
                     self.objProps[t] += c.properties.keys()
                     self.objMethods[t] += c.methods.keys()
                 c = c.parent
 
         self.objProps["point"] += ["x", "y"]
         self.objProps["size"] += ["width", "height"]
         self.objProps["any"] += ["x", "y", "width", "height"]
 
+        for t in ["file", "bytes"]:
+            self.objProps[t] = []
+            self.objMethods[t] = []
+
         self.objProps = {key:list(set(l)) for (key, l) in self.objProps.items()}  # unique the items
         self.objMethods = {key:list(set(l)) for (key, l) in self.objMethods.items()}  # unique the items
 
         self.built_in = ["False", "True", "None"]
         self.built_in.extend("else import pass break except in raise finally is return and continue for lambda try "
                              "as def from while del global not with elif if or yield input()".split(" "))
 
@@ -124,19 +128,19 @@
                 elif p == "self" and handlerObj:
                     retVals = (objType, p, handlerObj.type, handlerObj)
                 elif p == "card":
                     retVals = (objType, p, "card", thisCard)
                 elif p == "stack":
                     retVals = (objType, p, "stack", self.stackManager.stackModel)
                 elif p in self.globalVars:
-                    retVals = (objType, p, helpData.HelpDataGlobals.variables[p]["type"], None)
+                    retVals = (objType, p, helpDataGen.HelpDataGlobals.variables[p]["type"], None)
                 elif p in self.globalFuncs:
-                    retVals = (objType, p, helpData.HelpDataGlobals.functions[p]["return"], None)
+                    retVals = (objType, p, helpDataGen.HelpDataGlobals.functions[p]["return"], None)
                 elif p in self.builtinFuncs:
-                    retVals = (objType, p, helpData.HelpDataBuiltins.functions[p]["return"], None)
+                    retVals = (objType, p, helpDataGen.HelpDataBuiltins.functions[p]["return"], None)
                 elif p in self.varNames or p in self.funcNames:
                     # Later, track the actual type of each user variable
                     retVals = (objType, p, "any", None)
                 elif p == "mouse_pos":
                     retVals = (objType, p, "bool", None)
                 elif p == "elapsed_time":
                     retVals = (objType, p, "float", None)
@@ -147,24 +151,28 @@
                 elif len(parts[0]) and parts[0][-1] == "]":
                     openPos = leadingStr.rfind('[')
                     if openPos > 0 and leadingStr[openPos-1] in NAME_CHARS:
                         retVals = (objType, p, "any", None)  # list index
                     else:
                         retVals = (objType, p, "list", None)  # list literal
                 elif len(parts[0]) and parts[0][-1] == "}":  # dict literal
-                    retVals = (objType, p, "dict", None)
+                    retVals = (objType, p, "dictionary", None)
                 elif parts[0] == '':  # nothing
                     retVals = (objType, p, None, None)
                 else:
                     retVals = (objType, p, "any", None)
             else:
-                if p in self.objProps["any"]:
-                    retVals = (objType, p, helpData.HelpData.GetTypeForProp(p), None)
+                if objType and p in self.objProps[objType]:
+                    retVals = (objType, p, helpDataGen.HelpData.GetTypeForProp(p, objType), None)
+                elif objType and p in self.objMethods[objType]:
+                    retVals = (objType, p, helpDataGen.HelpData.GetTypeForMethod(p, objType), None)
+                elif p in self.objProps["any"]:
+                    retVals = (objType, p, helpDataGen.HelpData.GetTypeForProp(p), None)
                 elif p in self.objMethods["any"]:
-                    retVals = (objType, p, helpData.HelpData.GetTypeForMethod(p), None)
+                    retVals = (objType, p, helpDataGen.HelpData.GetTypeForMethod(p), None)
                 elif p in self.built_in:
                     retVals = (objType, p, None, None)
                 if obj:
                     objChild = obj.GetChildModelByName(p)
                     if objChild:
                         retVals = (objType, p, objChild.type, objChild)
```

### Comparing `cardstock-0.99.5/cardstock/appCommands.py` & `cardstock-0.99.6/cardstock/appCommands.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,23 +55,23 @@
         self.stackManager = args[2]
         self.cardIndex = args[3]
         self.viewModel = args[4]
         self.delta = args[5]
 
     def Do(self):
         self.stackManager.LoadCardAtIndex(self.cardIndex)
-        sizeModel = self.stackManager.stackModel if self.viewModel.type == "card" else self.viewModel
+        sizeModel = self.viewModel
         viewSize = sizeModel.GetProperty("size")
         sizeModel.SetProperty("size", (viewSize[0]+self.delta[0], viewSize[1]+self.delta[1]))
         self.stackManager.SelectUiView(self.stackManager.GetUiViewByModel(self.viewModel))
         return True
 
     def Undo(self):
         self.stackManager.LoadCardAtIndex(self.cardIndex)
-        sizeModel = self.stackManager.stackModel if self.viewModel.type == "card" else self.viewModel
+        sizeModel = self.viewModel
         viewSize = sizeModel.GetProperty("size")
         sizeModel.SetProperty("size", (viewSize[0]-self.delta[0], viewSize[1]-self.delta[1]))
         self.stackManager.SelectUiView(self.stackManager.GetUiViewByModel(self.viewModel))
         return True
 
 
 class FlipShapeCommand(Command):
```

### Comparing `cardstock-0.99.5/cardstock/build.py` & `cardstock-0.99.6/cardstock/build.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/cardstockFrameParts.py` & `cardstock-0.99.6/cardstock/cardstockFrameParts.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/codeInspector.py` & `cardstock-0.99.6/cardstock/codeInspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
 # of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import wx
 import pythonEditor
 import wx.stc
-import helpData
+import helpDataGen
 import appCommands
 from uiView import UiView
 
 
 class CodeInspectorContainer(wx.Window):
     def __init__(self, cPanel, stackManager):
         super().__init__(cPanel)
@@ -136,23 +136,24 @@
         displayName = self.handlerPicker.GetItems()[self.handlerPicker.GetSelection()]
         displayName = displayName.strip().replace("def ", "")
         keys = list(UiView.handlerDisplayNames.keys())
         vals = list(UiView.handlerDisplayNames.values())
         self.SaveCurrentHandler()
         self.UpdateHandlerForUiView(self.stackManager.GetSelectedUiViews()[0], keys[vals.index(displayName)])
         self.codeEditor.SetFocus()
-        self.updateHelpTextFunc(helpData.HelpData.GetHandlerHelp(self.currentUiView, self.currentHandler))
+        if self.currentUiView:
+            self.updateHelpTextFunc(helpDataGen.HelpData.GetHandlerHelp(self.currentUiView.model, self.currentHandler))
 
 
     # Internal
 
     def CodeEditorFocused(self, event):
         helpText = None
         if self.currentUiView:
-            self.updateHelpTextFunc(helpData.HelpData.GetHandlerHelp(self.currentUiView, self.currentHandler))
+            self.updateHelpTextFunc(helpDataGen.HelpData.GetHandlerHelp(self.currentUiView.model, self.currentHandler))
         event.Skip()
 
     def CodeEditorOnIdle(self, event):
         if self.currentHandler:
             self.SaveCurrentHandler()
         event.Skip()
```

### Comparing `cardstock-0.99.5/cardstock/codeInspectorMulti.py` & `cardstock-0.99.6/cardstock/codeInspectorMulti.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
 # of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import wx
 import pythonEditor
 import wx.stc
-import helpData
+import helpDataGen
 import appCommands
 from uiView import UiView
 from simpleListBox import SimpleListBox
 
 HEADER_HEIGHT = 30
 
 class CodeInspectorContainer(wx.Window):
@@ -140,25 +140,26 @@
                 editorBlock.line.Show()
                 lastBlock = editorBlock
                 numShown += 1
                 editorBlock.Show()
             else:
                 editorBlock.Hide()
 
-        if numShown == 0:
+        if numShown == 0 and len(self.blocks):
             initial = self.currentUiView.model.initialEditHandler
             self.currentUiView.model.visibleHandlers.add(initial)
             lastBlock = self.blocks[initial]
             lastBlock.SetCanShowCloseButton(False)
             lastBlock.Show()
             numShown += 1
 
         if numShown == 1:
             lastBlock.SetCanShowCloseButton(False)
-        lastBlock.line.Hide()  # Hide last block's bottom-line
+        if numShown > 0:
+            lastBlock.line.Hide()  # Hide last block's bottom-line
 
         self.visibleBlocks = []
         for handlerName, block in self.blocks.items():
             if block.IsShown():
                 self.visibleBlocks.append(block)
                 block.UpdateLabelState(handlerName)
                 block.UpdateEditorSize()
@@ -318,17 +319,17 @@
             self.container.addButton.Show()
             if wx.Platform == "__WXMSW__":
                 self.container.Enable()
             hp.DestroyLater()
             self.Refresh(True)
 
     def OnHandlerPickerSelectionChanged(self, index, text):
-        if index is not None:
+        if index is not None and self.currentUiView:
             handlerName = self.DisplayNameToRawName(text)
-            self.updateHelpTextFunc(helpData.HelpData.GetHandlerHelp(self.currentUiView, handlerName))
+            self.updateHelpTextFunc(helpDataGen.HelpData.GetHandlerHelp(self.currentUiView.model, handlerName))
 
     def OnMouseDown(self, event):
         """
         Clicked in the codeInspector, outside of any block, so focus the first or last block's editor and select the
         first or last position, if the user clicked either above or below the editor blocks.
         """
         firstBlock = lastBlock = None
@@ -355,16 +356,17 @@
         mouse_pos = event.GetPosition()
         editorBlock = event.GetEventObject()
         if isinstance(editorBlock, wx.StaticText):
             editorBlock = editorBlock.GetParent()
         editorBlock.codeEditor.SetFocus()
         if mouse_pos.y < editorBlock.codeEditor.GetPosition().y:
             editorBlock.codeEditor.SetSelection(0, 0)
-            self.updateHelpTextFunc(helpData.HelpData.GetHandlerHelp(self.currentUiView,
-                                                                     editorBlock.codeEditor.currentHandler))
+            if self.currentUiView:
+                self.updateHelpTextFunc(helpDataGen.HelpData.GetHandlerHelp(self.currentUiView.model,
+                                                                         editorBlock.codeEditor.currentHandler))
         else:
             end = editorBlock.codeEditor.GetLastPosition()
             editorBlock.codeEditor.SetSelection(end, end)
 
         editorBlock.codeEditor.SetFocus()
 
     def CloseBlock(self, handlerName):
@@ -380,15 +382,15 @@
     def CodeEditorFocused(self, event):
         """ When focusing a codeEditor, scroll it into view. """
         if self.currentUiView:
             codeEditor = event.GetEventObject()
             handlerName = codeEditor.currentHandler
             if handlerName in self.blocks and self.blocks[handlerName].IsShown():
                 wx.CallAfter(self.blocks[handlerName].ScrollParentIfNeeded)
-                self.updateHelpTextFunc(helpData.HelpData.GetHandlerHelp(self.currentUiView, handlerName))
+                self.updateHelpTextFunc(helpDataGen.HelpData.GetHandlerHelp(self.currentUiView.model, handlerName))
                 self.lastFocusedHandler = handlerName
         event.Skip()
 
 
 class EditorBlock(wx.Window):
     """ One block of handlerName label and code editor. """
     closeBmp = None
```

### Comparing `cardstock-0.99.5/cardstock/codeRunnerThread.py` & `cardstock-0.99.6/cardstock/codeRunnerThread.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/consoleWindow.py` & `cardstock-0.99.6/cardstock/consoleWindow.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/controlPanel.py` & `cardstock-0.99.6/cardstock/controlPanel.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from tools import *
 from appCommands import *
 from wx.lib import buttons # for generic button classes
 from wx.lib.resizewidget import ResizeWidget, EVT_RW_LAYOUT_NEEDED
 from pythonEditor import PythonEditor
 from uiView import UiView
 from embeddedImages import embeddedToolImages
-from helpData import HelpData
+from helpDataGen import HelpData
 
 
 class ControlPanel(wx.Panel):
     """
     This class implements the control panel for the designer app.  It includes a tool palette for choosing a tool.
     It includes thickness and pen and fill colors for drawing shapes, and an inspector and code editor for editing
     objects.
@@ -212,15 +212,15 @@
 
     def OnGridCellSelected(self, event):
         if not self.inspector.isSettingUp:
             if len(self.lastSelectedUiViews) > 0:
                 uiView = self.lastSelectedUiViews[0]
                 if uiView:
                     key = self.inspector.GetCellValue(event.GetRow(), 0)
-                    helpText = HelpData.GetPropertyHelp(uiView, key)
+                    helpText = HelpData.GetPropertyHelp(uiView.model, key)
                     self.UpdateHelpText(helpText)
         else:
             self.UpdateHelpText("")
         event.Skip()
 
     def UpdateForUiViews(self, uiViews):
         self.Freeze()
```

### Comparing `cardstock-0.99.5/cardstock/designer.py` & `cardstock-0.99.6/cardstock/designer.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
 HERE = os.path.dirname(os.path.realpath(__file__))
 
 # ----------------------------------------------------------------------
 
 ID_OPEN_EXAMPLE = wx.NewIdRef()
 ID_EXPORT = wx.NewIdRef()
+ID_EDIT_STACK = wx.NewIdRef()
 ID_RUN = wx.NewIdRef()
 ID_RUN_FROM = wx.NewIdRef()
 ID_SEARCH_IMAGE = wx.NewIdRef()
 ID_SEARCH_SOUND = wx.NewIdRef()
 ID_EDIT = wx.NewIdRef()
 ID_MENU_FIND = wx.NewIdRef()
 ID_MENU_FIND_SEL = wx.NewIdRef()
@@ -118,28 +119,30 @@
         self.MakeMenuBar()
         self.filename = None
         self.app = None
         # self.lastStats = {}
 
         self.toolbar = self.CreateToolBar(style=wx.TB_TEXT)
         icn = embeddedImages.run.GetBitmap()
+        self.toolbar.AddTool(ID_EDIT_STACK, 'Stack', embeddedImages.stack.GetBitmap(), wx.NullBitmap)
         self.toolbar.AddTool(ID_RUN, 'Run Stack', icn, wx.NullBitmap)
 
         self.toolbar.AddStretchableSpace()
 
         self.cardPicker = wx.Choice(parent=self.toolbar)
         self.cardPicker.Bind(wx.EVT_CHOICE, self.OnPickCard)
         self.cardPickerToolId = self.toolbar.AddControl(self.cardPicker).GetId()
 
         self.toolbar.AddTool(ID_PREV_CARD, 'Previous Card', wx.ArtProvider.GetBitmap(wx.ART_GO_BACK), wx.NullBitmap)
         self.toolbar.AddTool(ID_ADD_CARD, 'Add Card', wx.ArtProvider.GetBitmap(wx.ART_PLUS), wx.NullBitmap)
         self.toolbar.AddTool(ID_NEXT_CARD, 'Next Card', wx.ArtProvider.GetBitmap(wx.ART_GO_FORWARD), wx.NullBitmap)
 
         self.toolbar.Realize()
 
+        self.Bind(wx.EVT_TOOL, self.OnMenuEditStack, id=ID_EDIT_STACK)
         self.Bind(wx.EVT_TOOL, self.OnMenuRun, id=ID_RUN)
         self.Bind(wx.EVT_FIND, self.OnFindEvent)
         self.Bind(wx.EVT_FIND_NEXT, self.OnFindEvent)
         self.Bind(wx.EVT_FIND_REPLACE, self.OnReplaceEvent)
         self.Bind(wx.EVT_FIND_REPLACE_ALL, self.OnReplaceAllEvent)
 
         self.splitter = wx.SplitterWindow(self, style=wx.SP_3DSASH | wx.SP_LIVE_UPDATE)
@@ -273,15 +276,15 @@
                     self.allCodeWindow = None
                 if self.errorListWindow:
                     self.errorListWindow.Destroy()
                     self.errorListWindow = None
                 self.lastRunErrors = []
 
     def SetFrameSizeFromModel(self):
-        size = self.stackManager.stackModel.GetProperty("size")
+        size = self.stackManager.uiCard.model.GetProperty("size")
         self.stackManager.uiCard.ResizeCardView(size)
         size = self.FromDIP(size)
         self.stackManager.UpdateBuffer()
         cPanelWidth = max(self.FromDIP(self.cPanel.defaultPanelWidth), self.cPanel.GetSize().Width)
         clientSize = (size.Width + self.splitter.GetSashSize() + cPanelWidth,
                       max(size.Height, self.FromDIP(500)))
         def updateSize():
@@ -515,17 +518,14 @@
                 hasGroups = True
                 break
 
         if len(uiViews) == 1 and uiViews[0].model.type == "card":
             contextMenu.AppendSeparator()
             contextMenu.Append(ID_DUPLICATE_CARD, "&Duplicate Card\tCtrl-Alt-+", "Duplicate Card")
             contextMenu.Append(ID_REMOVE_CARD, "&Remove Card", "Remove Card")
-            contextMenu.AppendSeparator()
-            contextMenu.Append(ID_MOVE_CARD_FWD, "Move Card &Forward\tCtrl-Shift-]", "Move Card Forward")
-            contextMenu.Append(ID_MOVE_CARD_BACK, "Move Card Bac&k\tCtrl-Shift-[", "Move Card Back")
 
         if len(uiViews) > 1:
             contextMenu.AppendSeparator()
             contextMenu.Append(ID_GROUP, "&Group Objects\tCtrl-Alt-G", "Group Objects")
             if hasGroups:
                 contextMenu.Append(ID_UNGROUP, "&Ungroup Objects\tCtrl-Alt-U", "Ungroup Objects")
             contextMenu.AppendSeparator()
@@ -550,19 +550,25 @@
         elif hasGroups:
             contextMenu.AppendSeparator()
             contextMenu.Append(ID_UNGROUP, "&Ungroup Objects\tCtrl-Alt-U", "Ungroup Objects")
 
         contextMenu.AppendSeparator()
         contextMenu.Append(ID_FLIP_HORIZ, "Flip Horizontal\tCtrl-Alt-H", "Flip Horizontal")
         contextMenu.Append(ID_FLIP_VERT, "Flip Vertical\tCtrl-Alt-V", "Flip Vertical")
-        contextMenu.AppendSeparator()
-        contextMenu.Append(ID_MOVE_VIEW_FRONT, "Move to Front\tCtrl-Alt-Shift-F", "Move to Front")
-        contextMenu.Append(ID_MOVE_VIEW_FWD, "Move &Forward\tCtrl-Alt-F", "Move Forward")
-        contextMenu.Append(ID_MOVE_VIEW_BACK, "Move Bac&kward\tCtrl-Alt-B", "Move Back")
-        contextMenu.Append(ID_MOVE_VIEW_END, "Move to Back\tCtrl-Alt-Shift-B", "Move to Back")
+
+        if len(uiViews) == 1 and uiViews[0].model.type == "card":
+            contextMenu.AppendSeparator()
+            contextMenu.Append(ID_MOVE_CARD_FWD, "Move Card &Forward\tCtrl-Shift-]", "Move Card Forward")
+            contextMenu.Append(ID_MOVE_CARD_BACK, "Move Card Bac&k\tCtrl-Shift-[", "Move Card Back")
+        else:
+            contextMenu.AppendSeparator()
+            contextMenu.Append(ID_MOVE_VIEW_FRONT, "Move to Front\tCtrl-Alt-Shift-F", "Move to Front")
+            contextMenu.Append(ID_MOVE_VIEW_FWD, "Move &Forward\tCtrl-Alt-F", "Move Forward")
+            contextMenu.Append(ID_MOVE_VIEW_BACK, "Move Bac&kward\tCtrl-Alt-B", "Move Back")
+            contextMenu.Append(ID_MOVE_VIEW_END, "Move to Back\tCtrl-Alt-Shift-B", "Move to Back")
 
         return contextMenu
 
     wildcard = "CardStock files (*.cds)|*.cds"
 
     def OnMenuNew(self, event):
         if wx.GetMouseState().LeftIsDown():
@@ -662,14 +668,17 @@
             return
         def doSave():
             self.OnMenuSave(None)
         exporter = StackExporter(self.stackManager)
         exporter.StartExport(doSave)
 
     def RunFromCard(self, cardIndex, generateThumbnail=False):
+        self.stackManager.view.SetFocus()  # Blur any active property editor, to commit its new value
+        wx.YieldIfNeeded()
+
         if self.isStartingViewer:
             return
         self.isStartingViewer = True
 
         if self.viewer:
             self.viewer.Destroy()
 
@@ -704,14 +713,17 @@
         self.viewer.designer = self
 
         self.viewer.PushStack(stackModel, self.filename, cardIndex)
         self.viewer.Show(not generateThumbnail)
         self.viewer.Refresh()
         self.isStartingViewer = False
 
+    def OnMenuEditStack(self, event):
+        self.stackManager.SelectUiView(self.stackManager.uiStack)
+
     def OnMenuRun(self, event):
         if wx.GetMouseState().LeftIsDown():
             return
         self.RunFromCard(0)
 
     def OnMenuRunFrom(self, event):
         if wx.GetMouseState().LeftIsDown():
```

### Comparing `cardstock-0.99.5/cardstock/embeddedImages.py` & `cardstock-0.99.6/cardstock/embeddedImages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1823,7 +1823,29 @@
     b'nsZ+JfjfW1RVhKzdFWBbaxQTxN+Fl4KFw7G3VKoII9lz7Z5NEZwR7fJecLa0kH3ItpS0ilB7'
     b'siXhs0B/ktErAXlSqPxJdmQJ8YVA9gixwYBg8Il7GrNpJXkQ9GuyOQv0Rlh3QDKKLfQ6+cRb'
     b'yk1VhJvygIDs/gi/0vyjNMJB435sVO618I1JkrzSXYE2lml6DnGFukUuC/OdT2dd6hBP2JNH'
     b'vFI2fEo2X+kPzRdZkMRqHL7S3cJltMrLCJeTs4O+0+BEOBBeYJTMFCp/xqI5l2UrrREbDEgV'
     b'oYtpYIMmLoTa24LD8N787h4HZn49aBOuurbGd2GRqUkb/bRFInFmHaHWj3dXAbmiVSEKvdXI'
     b'z1NfgSFs/AfYVbefCNvSjf3FUOzbMm9pzCfMTY6u/U+UYubiiqSJe0JXaOxvomLnMvJVkBWb'
     b'r7zwqvHpRndI2sKZ2za2/gt+0YIMN1o1aQAAAABJRU5ErkJggg==')
+
+#----------------------------------------------------------------------
+stack = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAABkAAAAZCAQAAABu4E3oAAAAIGNIUk0AAHomAACAhAAA+gAA'
+    b'AIDoAAB1MAAA6mAAADqYAAAXcJy6UTwAAAACYktHRAAAqo0jMgAAAAlwSFlzAAAuIwAALiMB'
+    b'eKU/dgAAAAd0SU1FB+gFFBUsF4FX8wUAAAIqSURBVDjLrZJNaBNRFIVPjUabIIIxFirFLqrQ'
+    b'lbipCCLVShcupBFaFBSCIv6s6qK7rIy4ECvUjQgVbJGKSq2If1il1eCqtQu1SCVpZpKZZN5M'
+    b'nHRCM83vXBdpk0wSbQS/3Xucc989913gv2FBBzb9i6Edny4LO77DhYZ65FZ4jks/RMrFtGtB'
+    b'fMTB9QwdmBsJpZNUwOBCV6N4gj1/ktsxeIZxApnJzstuGUNwVhu6WxYm+FyKapBP+/ydHAbM'
+    b'yTyXohKjvxD1Ny0VXtqwatm8zcjlQbU7pswHodPCzkMx3x/C9M1FVa2uL0lXJAxje61iTnyz'
+    b'qo9iSa0kz6Weh0/E3QrG0V4pb8CpZm6SzyTeywekl+GMRkTEC2eV4VAqYaRmlZ447sFSbrnu'
+    b'kVWlUFmPjYWOyNOBh5FeFiyOJMI1qeb4wq8VNQEDABodp1smNi7a7Lkxe+tOADD0N9F9GnNV'
+    b'xm/DY29UilfHFyJuhhtoXBOWulMxN9Xjs2e1vekttrXL7PJTZdS6m6Zs+ArR/IYF/V3yl7Cx'
+    b'MsNcyhivMyKin2IfeyXmlynvD1wUMY6t5Zah27y+tLpU+ttgF3sXuyv2S3Ixvp9vFrGr3NJ3'
+    b'kpuVjeKG6eoLxScY6cIplbgfxiTaKn/GgVvn+AWespXx58PdQVwozraCVox6YxGlJE9qgyE8'
+    b'MzdUzX7r6ztCnBFRdoY/HEAv6uKY8/NIwMvwAI76DIWtcOFo/fJ1+A0/LbhAOScBfwAAABl0'
+    b'RVh0Q29tbWVudABDcmVhdGVkIHdpdGggR0lNUFeBDhcAAAAldEVYdGRhdGU6Y3JlYXRlADIw'
+    b'MjQtMDUtMTRUMjE6MzM6NTcrMDA6MDD+Sg9MAAAAJXRFWHRkYXRlOm1vZGlmeQAyMDI0LTA1'
+    b'LTE0VDIxOjMzOjQ2KzAwOjAw5cq82gAAACh0RVh0ZGF0ZTp0aW1lc3RhbXAAMjAyNC0wNS0y'
+    b'MFQyMTo0NDoyMyswMDowMGrEotwAAAAASUVORK5CYII=')
+
+
```

### Comparing `cardstock-0.99.5/cardstock/errorListWindow.py` & `cardstock-0.99.6/cardstock/errorListWindow.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,15 +85,21 @@
                         if obj.GetProperty("name") == objName:
                             e.obj = obj
                             break
                     else:
                         e.card = None
 
     def JumpToError(self, error):
-        if error.card:
+        if error.obj and error.obj.type == "stack":
+            self.designer.stackManager.SelectUiView(self.designer.stackManager.uiStack)
+            if error.lineNum:
+                self.designer.cPanel.codeInspector.SelectAndScrollToLine(error.handlerName, error.lineNum - 1)
+            self.designer.Raise()
+
+        elif error.card:
             self.designer.cPanel.SetToolByName("hand")
             self.designer.stackManager.LoadCardAtIndex(error.card.parent.childModels.index(error.card))
             if error.obj:
                 uiView = self.designer.stackManager.GetUiViewByModel(error.obj)
                 self.designer.stackManager.SelectUiView(uiView)
                 self.designer.cPanel.UpdateHandlerForUiViews([uiView], None)
                 if error.lineNum:
```

### Comparing `cardstock-0.99.5/cardstock/examples/Asteroids.cds` & `cardstock-0.99.6/cardstock/examples/Asteroids.cds`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7606660604056437%*

 * *Differences: {"'CardStock_stack_format'": '9',*

 * * "'CardStock_stack_version'": "'0.99.6'",*

 * * "'cards'": "{0: {'handlers': {'on_setup': 'from random import "*

 * *            "randint\\n\\ntry_again.hide()\\nasteroid.hide()\\nisGameOver = False'}, 'properties': "*

 * *            "{'size': [800, 800], 'can_resize': True}, 'childModels': {0: {'properties': "*

 * *            "{'pen_style': 'Solid'}}}}}",*

 * * "'properties'": "{'author': '', 'info': '', delete: ['size', 'can_resize']}"}*

```diff
@@ -1,10 +1,10 @@
 {
-    "CardStock_stack_format": 7,
-    "CardStock_stack_version": "0.99.4",
+    "CardStock_stack_format": 9,
+    "CardStock_stack_version": "0.99.6",
     "cards": [
         {
             "childModels": [
                 {
                     "handlers": {
                         "on_message": "if message == \"hit\":\n   # Then split in half\n   angle = randint(0, 360)\n   dSpeed = randint(10, 30)\n   # Create 2 new asteroids\n   ratio1 = randint(35, 50)/100.0\n   ratio2 = 1.1-ratio1\n   \n   child.hide()  # Just hide the shot, since it will be Deleted within a couple seconds\n   \n   if self.size.width * ratio1 >= 12:\n      sub1 = self.clone(size=self.size*ratio1)\n      sub1.speed += rotate_point((0, dSpeed/ratio1), angle)\n      numAsteroids += 1\n   if self.size.width * ratio2 >= 12:\n      sub2 = self.clone(size=self.size*ratio2)\n      sub2.speed -= rotate_point((0, dSpeed/ratio2), angle)\n      numAsteroids += 1\n   \n   self.delete()  # Delete this asteroid\n   numAsteroids -= 1\n",
                         "on_periodic": "if not self.is_visible:\n   return\n\n# Wrap this asteroid around the edges of the card\nif self.center.y <= 0 and self.speed.y < 0:\n   # Off the Bottom edge\n   self.center = [self.center.x, card.size.height]\nelif self.center.y >= card.size.height and self.speed.y > 0:\n   # Off the Top edge\n   self.center = [self.center.x, 0]\nelif self.center.x <= 0 and self.speed.x < 0:\n   # Off the Left edge\n   self.center = [card.size.width, self.center.y]\nelif self.center.x >= card.size.width and self.speed.x > 0:\n   # Off the Right edge\n   self.center = [0, self.center.y]\n\n# Did any shot objects touch me?\nhits = []\nfor child in card.children:\n   if child.name.startswith(\"shot\") and child.is_visible:\n      d = distance(self.center, child.center)\n      if d <= self.size.width/2 + child.size.width/2:\n         self.send_message(\"hit\")\n         if numAsteroids == 0:\n            card.send_message(\"gameOver\")\n"
@@ -23,14 +23,15 @@
                         "fill_color": "#DEE2DBCC",
                         "name": "asteroid",
                         "originalSize": [
                             69,
                             69
                         ],
                         "pen_color": "#000000CC",
+                        "pen_style": "Solid",
                         "pen_thickness": 4,
                         "position": [
                             96.0,
                             625.0
                         ],
                         "rotation": 0.0,
                         "size": [
@@ -90,28 +91,30 @@
             ],
             "handlers": {
                 "on_key_hold": "if not isGameOver:\n   # Respond to these keys continuously while pressed\n   if key_name == \"Left\":\n      ship.rotation -= 180*elapsed_time\n   elif key_name == \"Right\":\n      ship.rotation += 180*elapsed_time\n   \n   elif key_name == \"Up\":\n      ship.speed += rotate_point((0, 450*elapsed_time), ship.rotation)\n      play_sound(\"puff.wav\")",
                 "on_key_press": "# Respond to these keys once per press, on KeyDown\nif key_name == \"Space\" and not isGameOver:\n   self.send_message(\"shoot\")\nelif key_name == \"Return\" and isGameOver:\n   self.send_message(\"start\")",
                 "on_message": "if message == \"start\":\n   # Delete all asteroids\n   for c in card.children.copy():\n      if c.name.startswith(\"asteroid_\"):\n         c.delete()\n   \n   # Set up the first asteroid, as a clone of the original, hidden one\n   ast = asteroid.clone()\n   if randint(0, 1):\n      ast.position = (100,randint(50, card.size.height-100))\n   else:\n      ast.position = (randint(50, card.size.width-100),100)\n   \n   ast.speed += (randint(-100,100), randint(-100,100))\n   ast.show()\n   numAsteroids = 1\n   isGameOver = False\n   ship.rotation = 0\n   ship.center = card.center\n   try_again.hide()\n\nelif message == \"shoot\":\n   # Create shot\n   shot = card.add_oval(\"shot\",\n      center=(ship.center+rotate_point((0, 50), ship.rotation)),\n      size=(10,10),\n      fill_color='red',\n      speed=ship.speed+rotate_point((0, 150), ship.rotation))\n   # Delete after 2 seconds\n   run_after_delay(2, shot.delete)\n   # recoil the ship\n   ship.speed -= rotate_point((0, 3), ship.rotation)\n\nelif message == \"gameOver\":\n   # Stop the ship\n   ship.speed = (0,0)\n   \n   # Stop all asteroids, and Delete shots\n   for c in card.children.copy():\n      if c.name.startswith(\"asteroid_\"):\n         c.speed = (0, 0)\n      if c.name.startswith(\"shot\"):\n         c.delete()\n   isGameOver = True\n   try_again.show()\n",
                 "on_mouse_press": "if is_using_touch_screen():\n   if not isGameOver:\n      if not ship.is_touching_point(mouse_pos):\n         ship.rotation = angle_from_points(ship.center, mouse_pos)\n         self.send_message(\"shoot\")\n   else:\n      self.send_message(\"start\")\n",
                 "on_resize": "try_again.center = [card.center.x, card.size.height-40]",
-                "on_setup": "from random import randint\n   \ntry_again.hide()\nasteroid.hide()\nisGameOver = False",
+                "on_setup": "from random import randint\n\ntry_again.hide()\nasteroid.hide()\nisGameOver = False",
                 "on_show_card": "self.send_message(\"start\")"
             },
             "properties": {
+                "can_resize": true,
                 "fill_color": "#000000",
-                "name": "card_1"
+                "name": "card_1",
+                "size": [
+                    800,
+                    800
+                ]
             },
             "type": "card"
         }
     ],
     "handlers": {},
     "properties": {
-        "can_resize": true,
+        "author": "",
         "can_save": false,
-        "size": [
-            800,
-            800
-        ]
+        "info": ""
     },
     "type": "stack"
 }
```

### Comparing `cardstock-0.99.5/cardstock/examples/Browser.cds` & `cardstock-0.99.6/cardstock/examples/Browser.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Calculator.cds` & `cardstock-0.99.6/cardstock/examples/Calculator.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Catch.cds` & `cardstock-0.99.6/cardstock/examples/Catch.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Diary.cds` & `cardstock-0.99.6/cardstock/examples/Diary.cds`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7612419377176322%*

 * *Differences: {"'CardStock_stack_format'": '9',*

 * * "'CardStock_stack_version'": "'0.99.6'",*

 * * "'cards'": "{0: {'properties': {'size': [500, 500], 'can_resize': False}, 'childModels': {1: "*

 * *            "{'properties': {'pen_style': 'Solid'}}, 2: {'properties': {'text': '>', delete: "*

 * *            "['title']}}, 3: {'properties': {'text': '<', delete: ['title']}}, 5: {'properties': "*

 * *            "{'text': 'Add', delete: ['title']}}, 6: {'properties': {'text': '1/2'}}, 7: "*

 * *            "{'properties': {'text': 'Del', delete: ['t […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "CardStock_stack_format": 6,
-    "CardStock_stack_version": "0.99.1",
+    "CardStock_stack_format": 9,
+    "CardStock_stack_version": "0.99.6",
     "cards": [
         {
             "childModels": [
                 {
                     "handlers": {},
                     "properties": {
                         "alignment": "Center",
@@ -45,14 +45,15 @@
                         "fill_color": "#FFFFFF",
                         "name": "shape_1",
                         "originalSize": [
                             480,
                             450
                         ],
                         "pen_color": "#000000",
+                        "pen_style": "Solid",
                         "pen_thickness": 4,
                         "position": [
                             10.0,
                             10.0
                         ],
                         "rotation": 0.0,
                         "size": [
@@ -75,15 +76,15 @@
                         ],
                         "rotation": 0.0,
                         "size": [
                             53,
                             29
                         ],
                         "style": "Border",
-                        "title": ">"
+                        "text": ">"
                     },
                     "type": "button"
                 },
                 {
                     "handlers": {
                         "on_click": "goto_previous_card()"
                     },
@@ -96,15 +97,15 @@
                         ],
                         "rotation": 0.0,
                         "size": [
                             53,
                             29
                         ],
                         "style": "Border",
-                        "title": "<"
+                        "text": "<"
                     },
                     "type": "button"
                 },
                 {
                     "handlers": {},
                     "properties": {
                         "alignment": "Left",
@@ -142,15 +143,15 @@
                         ],
                         "rotation": 0.0,
                         "size": [
                             44,
                             28
                         ],
                         "style": "Border",
-                        "title": "Add"
+                        "text": "Add"
                     },
                     "type": "button"
                 },
                 {
                     "handlers": {},
                     "properties": {
                         "alignment": "Right",
@@ -166,15 +167,15 @@
                             466.0
                         ],
                         "rotation": 0.0,
                         "size": [
                             76,
                             26
                         ],
-                        "text": "1/1",
+                        "text": "1/2",
                         "text_color": "black"
                     },
                     "type": "textlabel"
                 },
                 {
                     "handlers": {
                         "on_click": "card.delete()\n"
@@ -188,15 +189,15 @@
                         ],
                         "rotation": 0.0,
                         "size": [
                             44,
                             28
                         ],
                         "style": "Border",
-                        "title": "Del"
+                        "text": "Del"
                     },
                     "type": "button"
                 },
                 {
                     "handlers": {},
                     "properties": {
                         "alignment": "Center",
@@ -222,24 +223,26 @@
                     "type": "textfield"
                 }
             ],
             "handlers": {
                 "on_show_card": "i = card.number\ntotal = stack.num_cards\ncardNum.text = str(i) + '/' + str(total)\nfield.focus()\n"
             },
             "properties": {
+                "can_resize": false,
                 "fill_color": "#C4ACA9",
-                "name": "card_1"
+                "name": "card_1",
+                "size": [
+                    500,
+                    500
+                ]
             },
             "type": "card"
         }
     ],
     "handlers": {},
     "properties": {
-        "can_resize": false,
+        "author": "",
         "can_save": true,
-        "size": [
-            500,
-            500
-        ]
+        "info": ""
     },
     "type": "stack"
 }
```

### Comparing `cardstock-0.99.5/cardstock/examples/Dice-stats.cds` & `cardstock-0.99.6/cardstock/examples/Dice-stats.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Dice.cds` & `cardstock-0.99.6/cardstock/examples/Dice.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Factor.cds` & `cardstock-0.99.6/cardstock/examples/Factor.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Fifteen.cds` & `cardstock-0.99.6/cardstock/examples/Fifteen.cds`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7588291675177015%*

 * *Differences: {"'CardStock_stack_format'": '9',*

 * * "'CardStock_stack_version'": "'0.99.6'",*

 * * "'cards'": "{0: {'handlers': {'on_setup': 'from random import randint\\n\\nisMoving = "*

 * *            'False\\nspace.hide() # hide the space piece\\n\\npieces = [c for c in card.children '*

 * *            'if c.name.startswith("group")]\\npieces.append(space)\\n\\norigPieces = '*

 * *            'pieces.copy()\\n\\ndef Shuffle():\\n   # Switch each piece with a random other '*

 * *            "piece.\\n   # Make one more swap so it\\'s an even num […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "CardStock_stack_format": 6,
-    "CardStock_stack_version": "0.99.2",
+    "CardStock_stack_format": 9,
+    "CardStock_stack_version": "0.99.6",
     "cards": [
         {
             "childModels": [
                 {
                     "handlers": {},
                     "points": [
                         [
@@ -20,14 +20,15 @@
                         "fill_color": "#E7E5E8",
                         "name": "shape_2",
                         "originalSize": [
                             438,
                             438
                         ],
                         "pen_color": "black",
+                        "pen_style": "Solid",
                         "pen_thickness": 4,
                         "position": [
                             30.0,
                             30.0
                         ],
                         "rotation": 0.0,
                         "size": [
@@ -53,14 +54,15 @@
                         "fill_color": "#FFFFFF00",
                         "name": "space",
                         "originalSize": [
                             103,
                             102
                         ],
                         "pen_color": "black",
+                        "pen_style": "Solid",
                         "pen_thickness": 4,
                         "position": [
                             330.0,
                             30.0
                         ],
                         "rotation": 0.0,
                         "size": [
@@ -88,14 +90,15 @@
                                 "fill_color": "white",
                                 "name": "shape_1",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -166,14 +169,15 @@
                                 "fill_color": "white",
                                 "name": "shape_3",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -244,14 +248,15 @@
                                 "fill_color": "white",
                                 "name": "shape_4",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -322,14 +327,15 @@
                                 "fill_color": "white",
                                 "name": "shape_5",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -400,14 +406,15 @@
                                 "fill_color": "white",
                                 "name": "shape_6",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -478,14 +485,15 @@
                                 "fill_color": "white",
                                 "name": "shape_7",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -556,14 +564,15 @@
                                 "fill_color": "white",
                                 "name": "shape_8",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -634,14 +643,15 @@
                                 "fill_color": "white",
                                 "name": "shape_9",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -712,14 +722,15 @@
                                 "fill_color": "white",
                                 "name": "shape_10",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -790,14 +801,15 @@
                                 "fill_color": "white",
                                 "name": "shape_11",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -868,14 +880,15 @@
                                 "fill_color": "white",
                                 "name": "shape_12",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -946,14 +959,15 @@
                                 "fill_color": "white",
                                 "name": "shape_13",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -1024,14 +1038,15 @@
                                 "fill_color": "white",
                                 "name": "shape_14",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -1102,14 +1117,15 @@
                                 "fill_color": "white",
                                 "name": "shape_15",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -1180,14 +1196,15 @@
                                 "fill_color": "white",
                                 "name": "shape_16",
                                 "originalSize": [
                                     81,
                                     81
                                 ],
                                 "pen_color": "black",
+                                "pen_style": "Solid",
                                 "pen_thickness": 4,
                                 "position": [
                                     0.0,
                                     0.0
                                 ],
                                 "rotation": 0.0,
                                 "size": [
@@ -1239,27 +1256,29 @@
                         ]
                     },
                     "type": "group"
                 }
             ],
             "handlers": {
                 "on_key_press": "if key_name in [\"Left\", \"Right\", \"Up\", \"Down\"]:\n   MoveDir(key_name, 1)",
-                "on_setup": "from random import randint\n\nisMoving = False\nspace.hide() # hide the space piece\n\npieces = [c for c in card.children if c.name.startswith(\"group\")]\npieces.append(space)\n\norigPieces = pieces.copy()\n\ndef Shuffle():\n   # Switch each piece with a random other piece.\n   # Make one more swap so it's an even number of swaps\n   # otherwise it would be unsolvable.\n   shuffleList = list(range(len(pieces)-1))\n   shuffleList.append(randint(0,14))\n   for i in shuffleList:\n      j = i\n      while j == i:\n         # make sure we're not swapping a piece with itself\n         j = randint(0,len(pieces)-2)\n      pieces[i], pieces[j] = pieces[j], pieces[i]\n      tmp = pieces[j].position\n      pieces[j].position = pieces[i].position\n      pieces[i].position = tmp\n\ndef SlideSpots(moves):\n   # Animate sliding\n   global isMoving\n   if not isMoving:\n      tmpPieces = {}\n      tmpPositions = {}\n      for i,j in moves:\n         tmpPieces[i] = pieces[i]\n         tmpPositions[i] = pieces[i].position\n      for i,j in moves:\n         pieces[i].animate_position(0.15, tmpPositions[j], DoneMoving)\n      for i,j in moves:\n         pieces[j] = tmpPieces[i]\n      isMoving = True\n\ndef DoneMoving():\n   global isMoving\n   isMoving = False\n   CheckForWin()\n\ndef CheckForWin():\n   if pieces == origPieces:\n      play_sound(\"yay.wav\")\n      wait(3)\n      Shuffle()\n\ndef BuildCycleList(start, offset, n):\n   # Create move list that moves n peices, and swaps the space piece to the other end of the list\n   spots = list(reversed([start + offset*i for i in range(n+1)]))\n   moves = []\n   for i in range(len(spots)-1):\n      moves.append((spots[i], spots[i+1]))\n   moves.append((spots[-1], spots[0]))\n   return moves\n\ndef MoveDir(dir, n):\n   # Move n pieces in direction\n   i = pieces.index(space)\n   if dir == \"Right\" and i%4 != 0:\n      SlideSpots(BuildCycleList(i, -1, n))\n   elif dir == \"Left\" and i%4 != 3:\n      SlideSpots(BuildCycleList(i, 1, n))\n   elif dir == \"Up\" and i<12:\n      SlideSpots(BuildCycleList(i, 4, n))\n   elif dir == \"Down\" and i>=4:\n      SlideSpots(BuildCycleList(i, -4, n))\n\ndef MoveFrom(obj):\n   # Slide pieces from the clicked object obj, to the space piece, if they are in the same row/col\n   global isMoving\n   s = pieces.index(space)\n   o = pieces.index(obj)\n   sx, sy = s%4, int(s/4)\n   ox, oy = o%4, int(o/4)\n   if sx == ox and sy < oy:\n      MoveDir(\"Up\", oy-sy)\n   elif sx == ox and sy > oy:\n      MoveDir(\"Down\", sy-oy)\n   elif sy == oy and sx < ox:\n      MoveDir(\"Left\", ox-sx)\n   elif sy == oy and sx > ox:\n      MoveDir(\"Right\", sx-ox)\n\n# Shuffle when we start the stack\nShuffle()"
+                "on_setup": "from random import randint\n\nisMoving = False\nspace.hide() # hide the space piece\n\npieces = [c for c in card.children if c.name.startswith(\"group\")]\npieces.append(space)\n\norigPieces = pieces.copy()\n\ndef Shuffle():\n   # Switch each piece with a random other piece.\n   # Make one more swap so it's an even number of swaps\n   # otherwise it would be unsolvable.\n   shuffleList = list(range(len(pieces)-1))\n   shuffleList.append(randint(0,14))\n   for i in shuffleList:\n      j = i\n      while j == i:\n         # make sure we're not swapping a piece with itself\n         j = randint(0,len(pieces)-2)\n      pieces[i], pieces[j] = pieces[j], pieces[i]\n      tmp = pieces[j].position\n      pieces[j].position = pieces[i].position\n      pieces[i].position = tmp\n\ndef SlideSpots(moves):\n   # Animate sliding\n   global isMoving\n   if not isMoving:\n      tmpPieces = {}\n      tmpPositions = {}\n      for i,j in moves:\n         tmpPieces[i] = pieces[i]\n         tmpPositions[i] = pieces[i].position\n      for i,j in moves:\n         pieces[i].animate_position(0.15, tmpPositions[j], \"InOut\", DoneMoving)\n      for i,j in moves:\n         pieces[j] = tmpPieces[i]\n      isMoving = True\n\ndef DoneMoving():\n   global isMoving\n   isMoving = False\n   CheckForWin()\n\ndef CheckForWin():\n   if pieces == origPieces:\n      play_sound(\"yay.wav\")\n      wait(3)\n      Shuffle()\n\ndef BuildCycleList(start, offset, n):\n   # Create move list that moves n peices, and swaps the space piece to the other end of the list\n   spots = list(reversed([start + offset*i for i in range(n+1)]))\n   moves = []\n   for i in range(len(spots)-1):\n      moves.append((spots[i], spots[i+1]))\n   moves.append((spots[-1], spots[0]))\n   return moves\n\ndef MoveDir(dir, n):\n   # Move n pieces in direction\n   i = pieces.index(space)\n   if dir == \"Right\" and i%4 != 0:\n      SlideSpots(BuildCycleList(i, -1, n))\n   elif dir == \"Left\" and i%4 != 3:\n      SlideSpots(BuildCycleList(i, 1, n))\n   elif dir == \"Up\" and i<12:\n      SlideSpots(BuildCycleList(i, 4, n))\n   elif dir == \"Down\" and i>=4:\n      SlideSpots(BuildCycleList(i, -4, n))\n\ndef MoveFrom(obj):\n   # Slide pieces from the clicked object obj, to the space piece, if they are in the same row/col\n   global isMoving\n   s = pieces.index(space)\n   o = pieces.index(obj)\n   sx, sy = s%4, int(s/4)\n   ox, oy = o%4, int(o/4)\n   if sx == ox and sy < oy:\n      MoveDir(\"Up\", oy-sy)\n   elif sx == ox and sy > oy:\n      MoveDir(\"Down\", sy-oy)\n   elif sy == oy and sx < ox:\n      MoveDir(\"Left\", ox-sx)\n   elif sy == oy and sx > ox:\n      MoveDir(\"Right\", sx-ox)\n\n# Shuffle when we start the stack\nShuffle()"
             },
             "properties": {
+                "can_resize": false,
                 "fill_color": "#BBD4BF",
-                "name": "card_1"
+                "name": "card_1",
+                "size": [
+                    455,
+                    455
+                ]
             },
             "type": "card"
         }
     ],
     "handlers": {},
     "properties": {
-        "can_resize": false,
+        "author": "",
         "can_save": false,
-        "size": [
-            455,
-            455
-        ]
+        "info": ""
     },
     "type": "stack"
 }
```

### Comparing `cardstock-0.99.5/cardstock/examples/Flappy.cds` & `cardstock-0.99.6/cardstock/examples/Flappy.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Graph.cds` & `cardstock-0.99.6/cardstock/examples/Graph.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Guess.cds` & `cardstock-0.99.6/cardstock/examples/Guess.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Magic.cds` & `cardstock-0.99.6/cardstock/examples/Magic.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Mastermind.cds` & `cardstock-0.99.6/cardstock/examples/Mastermind.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Maze.cds` & `cardstock-0.99.6/cardstock/examples/Maze.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Morph.cds` & `cardstock-0.99.6/cardstock/examples/Morph.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Navigation.cds` & `cardstock-0.99.6/cardstock/examples/Navigation.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Number-puzzle.cds` & `cardstock-0.99.6/cardstock/examples/Number-puzzle.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Pong.cds` & `cardstock-0.99.6/cardstock/examples/Pong.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Requests.cds` & `cardstock-0.99.6/cardstock/examples/Requests.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Scene.cds` & `cardstock-0.99.6/cardstock/examples/Scene.cds`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7761477623456791%*

 * *Differences: {"'CardStock_stack_format'": '9',*

 * * "'CardStock_stack_version'": "'0.99.6'",*

 * * "'cards'": '{0: {\'handlers\': {\'on_periodic\': "# Create a new piece of snow every 30th of a '*

 * *            'second, if we can keep up!\\no = card.add_oval(\\n   size = (10,10),\\n   position = '*

 * *            "(randint(0,490),490),\\n   fill_color = 'white',\\n   pen_thickness = 1)\\n\\n# "*

 * *            'Animate it to the bottom of the stack, moving slightly on the x axis too, for '*

 * *            'fun.\\n# When the animation is comple […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "CardStock_stack_format": 6,
-    "CardStock_stack_version": "0.99.1",
+    "CardStock_stack_format": 9,
+    "CardStock_stack_version": "0.99.6",
     "cards": [
         {
             "childModels": [
                 {
                     "handlers": {
                         "on_click": "card.stop_animating()\ncard.animate_fill_color(1,\"#88AAFF\")\n\ncircle.stop_animating()\ncircle.animate_fill_color(1,\"yellow\")"
                     },
@@ -17,15 +17,15 @@
                         ],
                         "rotation": 0.0,
                         "size": [
                             124,
                             24
                         ],
                         "style": "Border",
-                        "title": "Day"
+                        "text": "Day"
                     },
                     "type": "button"
                 },
                 {
                     "handlers": {},
                     "points": [
                         [
@@ -41,14 +41,15 @@
                         "fill_color": "brown",
                         "name": "shape_1",
                         "originalSize": [
                             143,
                             147
                         ],
                         "pen_color": "black",
+                        "pen_style": "Solid",
                         "pen_thickness": 4,
                         "position": [
                             178.0,
                             0.0
                         ],
                         "rotation": 0.0,
                         "size": [
@@ -74,14 +75,15 @@
                         "fill_color": "yellow",
                         "name": "circle",
                         "originalSize": [
                             97,
                             94
                         ],
                         "pen_color": "black",
+                        "pen_style": "Solid",
                         "pen_thickness": 0,
                         "position": [
                             386.0,
                             373.0
                         ],
                         "rotation": 0.0,
                         "size": [
@@ -111,14 +113,15 @@
                         "fill_color": "brown",
                         "name": "shape_2",
                         "originalSize": [
                             232,
                             136
                         ],
                         "pen_color": "black",
+                        "pen_style": "Solid",
                         "pen_thickness": 4,
                         "position": [
                             136.0,
                             148.0
                         ],
                         "rotation": 0.0,
                         "size": [
@@ -144,14 +147,15 @@
                         "fill_color": "#A47D5D",
                         "name": "shape_3",
                         "originalSize": [
                             37,
                             58
                         ],
                         "pen_color": "black",
+                        "pen_style": "Solid",
                         "pen_thickness": 2,
                         "position": [
                             247.0,
                             1.0
                         ],
                         "rotation": 0.0,
                         "size": [
@@ -174,35 +178,41 @@
                         ],
                         "rotation": 0.0,
                         "size": [
                             124,
                             24
                         ],
                         "style": "Border",
-                        "title": "Night"
+                        "text": "Night"
                     },
                     "type": "button"
                 }
             ],
             "handlers": {
                 "on_key_press": "if key_name == \"N\":\n   night.click()\nelif key_name == \"D\":\n   day.click()",
-                "on_periodic": "# Create a new piece of snow every 30th of a second, if we can keep up!\no = card.add_oval(\n   size = (10,10),\n   position = (randint(0,490),490),\n   fill_color = 'white',\n   pen_thickness = 1)\n\n# Animate it to the bottom of the stack, moing slightly on the x axis too, for fun.\n# When the animation is complete, run o.delete() to remove the new snow from\n# the card, so we don't accumulate old snow, which would slow down the stack and waste memory.\no.animate_position(\n   randint(300,450)/100.0,\n   (o.position.x + randint(-20,20), -10),\n   o.delete)\n",
+                "on_periodic": "# Create a new piece of snow every 30th of a second, if we can keep up!\no = card.add_oval(\n   size = (10,10),\n   position = (randint(0,490),490),\n   fill_color = 'white',\n   pen_thickness = 1)\n\n# Animate it to the bottom of the stack, moving slightly on the x axis too, for fun.\n# When the animation is complete, run o.delete() to remove the new snow from\n# the card, so we don't accumulate old snow, which would slow down the stack and waste memory.\no.animate_position(\n   randint(300,450)/100.0,\n   (o.position.x + randint(-20,20), -10),\n   on_finished=o.delete)\n",
                 "on_setup": "from random import randint"
             },
             "properties": {
+                "can_resize": false,
                 "fill_color": "#88AAFF",
-                "name": "card_1"
+                "name": "card_1",
+                "size": [
+                    500,
+                    500
+                ]
             },
             "type": "card"
         }
     ],
     "handlers": {},
     "properties": {
-        "can_resize": false,
+        "author": "",
         "can_save": false,
+        "notes": "lots of notes\n\n\ngo here\n\n\n\n\nand here.",
         "size": [
             500,
             500
         ]
     },
     "type": "stack"
 }
```

### Comparing `cardstock-0.99.5/cardstock/examples/Serial.cds` & `cardstock-0.99.6/cardstock/examples/Serial.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Snake.cds` & `cardstock-0.99.6/cardstock/examples/Snake.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Tanks.cds` & `cardstock-0.99.6/cardstock/examples/Tanks.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Tetris.cds` & `cardstock-0.99.6/cardstock/examples/Tetris.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/TicTacToe.cds` & `cardstock-0.99.6/cardstock/examples/TicTacToe.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Welcome.cds` & `cardstock-0.99.6/cardstock/examples/Welcome.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/Wordel.cds` & `cardstock-0.99.6/cardstock/examples/Wordel.cds`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/click.wav` & `cardstock-0.99.6/cardstock/examples/click.wav`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/puff.wav` & `cardstock-0.99.6/cardstock/examples/puff.wav`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/ship-off.png` & `cardstock-0.99.6/cardstock/examples/ship-off.png`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/ship-on.png` & `cardstock-0.99.6/cardstock/examples/ship-on.png`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/simple-red-apple.png` & `cardstock-0.99.6/cardstock/examples/simple-red-apple.png`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/examples/yay.wav` & `cardstock-0.99.6/cardstock/examples/yay.wav`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/findEngineDesigner.py` & `cardstock-0.99.6/cardstock/findEngineDesigner.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import wx
 import stackManager
 from uiView import ViewModel
 from appCommands import SetPropertyCommand, SetHandlerCommand, CommandGroup
 import re
 
-SEARCHABLE_PROPERTIES = ["name", "text", "title", "file", "text_color", "pen_color", "fill_color"]
+SEARCHABLE_PROPERTIES = ["name", "text", "file", "text_color", "pen_color", "fill_color"]
 
 """
 Find and Replace logic.
 The search order is:
 - Cards, first to last
   - Recursively find cardModel's childModels (obj1, obj2, obj2.child1, obj2.child2, obj3, etc.)
     - Property text, in model.PropertyKeys() order (this is display order in the inspector)
```

### Comparing `cardstock-0.99.5/cardstock/findEngineViewer.py` & `cardstock-0.99.6/cardstock/findEngineViewer.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/flippedGCDC.py` & `cardstock-0.99.6/cardstock/flippedGCDC.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/generator.py` & `cardstock-0.99.6/cardstock/generator.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/helpData.py` & `cardstock-0.99.6/cardstock/helpData.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,428 +2,152 @@
 #     https://github.com/benjie-git/CardStock
 #
 # Copyright Ben Levitt 2020-2023
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
 # of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-import uiView
-import keyword
-
 """
 This file includes descriptions of all CardStock objects, properties, methods, and event handlers for use in
 context help, reference docs, and in the future, code completion.
 """
 
-
-class HelpData():
-    reservedNames = None
-
-    @classmethod
-    def ForObject(cls, obj):
-        return cls.ForType(obj.model.type)
-
-    @classmethod
-    def ForType(cls, typeStr):
-        if typeStr == "button":                   return HelpDataButton
-        elif typeStr == "textfield":              return HelpDataTextField
-        elif typeStr == "textlabel":              return HelpDataTextLabel
-        elif typeStr == "image":                  return HelpDataImage
-        elif typeStr == "webview":                return HelpDataWebView
-        elif typeStr == "group":                  return HelpDataGroup
-        elif typeStr in ["line", "pen"]:          return HelpDataLine
-        elif typeStr in ["shape", "oval", "rect", "polygon"]:return HelpDataShape
-        elif typeStr == "roundrect":              return HelpDataRoundRectangle
-        elif typeStr == "card":                   return HelpDataCard
-        elif typeStr == "stack":                  return HelpDataStack
-        return HelpDataObject
-
-    @classmethod
-    def GetTypeForProp(cls, propName):
-        for c in helpClasses:
-            if propName in c.properties:
-                return c.properties[propName]["type"]
-        return None
-
-    @classmethod
-    def GetTypeForMethod(cls, methodName):
-        for c in helpClasses:
-            if methodName in c.methods:
-                return c.methods[methodName]["return"]
-        return None
-
-    @classmethod
-    def GetPropertyHelp(cls, obj, key):
-        data = cls.ForObject(obj)
-        while data:
-            if key in data.properties:
-                prop = data.properties[key]
-                text = "<b>"+key+"</b>:<i>" + prop["type"] + "</i> - " + prop["info"]
-                return text
-            data = data.parent
-        return None
-
-    @classmethod
-    def GetHelpForName(cls, key, objType):
-        isFunc = key.endswith("()")
-        if objType is None:
-            return None
-        elif objType == "global":
-            allClasses = [HelpDataGlobals]
-        elif objType != "any":
-            allClasses = []
-            c = cls.ForType(objType)
-            while c:
-                allClasses.append(c)
-                c = c.parent
-        else:
-            allClasses = [HelpDataGlobals]
-            allClasses.extend(helpClasses)
-            allClasses.remove(HelpDataString)
-            allClasses.remove(HelpDataList)
-        if not isFunc:
-            for c in allClasses:
-                if key in c.properties:
-                    prop = c.properties[key]
-                    text = "<b>" + key + "</b>:<i>" + prop["type"] + "</i> - " + prop["info"]
-                    return text
-        else:
-            key = key[:-2]
-            for c in allClasses:
-                if key in c.methods:
-                    method = c.methods[key]
-                    argText = ""
-                    for name, arg in method["args"].items():
-                        typeText = (":<i>" + arg["type"] + " </i>") if "type" in arg else ""
-                        argText += "&nbsp;&nbsp;&nbsp;&nbsp;<b>" + name + "</b>" + typeText + " - " + arg[
-                            "info"] + "<br/>"
-                    ret = ("Returns: <i>" + method["return"] + "</i><br/>") if method["return"] else ""
-                    name = key + "(" + ', '.join(method["args"].keys()) + ")"
-                    text = f"<b>{name}</b><br/>{argText}{ret}<br/>{method['info']}"
-                    return text
-        return None
-
-    @classmethod
-    def HtmlTableFromLists(cls, rows):
-        if len(rows) < 2:
-            return ""
-
-        text =  "<table border='0' cellpadding='5' cellspacing='0'>\n"
-
-        text += "<tr>"
-        for cell in rows[0]:
-            text += "<th align='left' valign='top'>" + cell + "</th>"
-        text += "</tr>\n"
-
-        bgcolors = [" bgcolor='#D0DFEE'", " bgcolor='#CCCCCC'"]
-        bg = bgcolors[0]
-        for row in rows[1:]:
-            bg = bgcolors[0 if bg==bgcolors[1] else 1]
-            text += "<tr>"
-            text += "<th align='left' valign='top'"+bg+">" + row[0] + "</th>"
-            for cell in row[1:]:
-                text += "<td align='left' valign='top'"+bg+">" + cell + "</td>"
-            text += "</tr>\n"
-        text += "</table>"
-        return text
-
-
-    @classmethod
-    def PropertyTable(cls, typeStr):
-        data = cls.ForType(typeStr)
-        rows = []
-        rows.append(["Property", "Type", "Description"])
-        while data:
-            for key in sorted(data.properties):
-                prop = data.properties[key]
-                rows.append([key, "<i>" + prop["type"] + "</i>", prop["info"]])
-            data = data.parent
-            if data == HelpDataObject:
-                break
-        if len(rows) >= 2:
-            return cls.HtmlTableFromLists(rows)
-        else:
-            return "<p>No additional properties for this object type.</p>"
-
-    @classmethod
-    def GetHandlerHelp(cls, obj, key):
-        data = cls.ForObject(obj)
-        while data:
-            if key in data.handlers:
-                handler = data.handlers[key]
-                argText = ""
-                for name, arg in handler["args"].items():
-                    argText += "&nbsp;&nbsp;&nbsp;&nbsp;<b>" + name + "</b>:<i>" + arg["type"] + " </i> - " + arg["info"] + "<br/>"
-                text = "<b>" + uiView.UiView.handlerDisplayNames[key] + "</b><br/>" + argText + "<br/>" + handler["info"]
-                return text
-            data = data.parent
-        return None
-
-    @classmethod
-    def HandlerTable(cls, typeStr):
-        data = cls.ForType(typeStr)
-        rows = []
-        rows.append(["Event", "Arguments", "Description"])
-        while data:
-            for key in sorted(data.handlers):
-                handler = data.handlers[key]
-                argText = ""
-                for name, arg in handler["args"].items():
-                    argText += "<b>" + name + "</b>:<i>" + arg["type"] + " </i> - " + arg["info"] + "<br/>"
-                rows.append([uiView.UiView.handlerDisplayNames[key], argText, handler["info"]])
-            data = data.parent
-            if data == HelpDataObject:
-                break
-        if len(rows) >= 2:
-            return cls.HtmlTableFromLists(rows)
-        else:
-            return "<p>No additional events for this object type.</p>"
-
-    @classmethod
-    def MethodTable(cls, typeStr):
-        data = cls.ForType(typeStr)
-        rows = []
-        rows.append(["Method", "Arguments", "Return", "Description"])
-        while data:
-            for key in sorted(data.methods):
-                method = data.methods[key]
-                argText = ""
-                for name, arg in method["args"].items():
-                    typeText = (":<i>" + arg["type"] + " </i>") if "type" in arg else ""
-                    argText += "<b>" + name + "</b>" + typeText + " - " + arg["info"] + "<br/>"
-                ret = method["return"] if method["return"] else ""
-                name = key + "(" + ', '.join(method["args"].keys()) + ")"
-                rows.append([name, argText, "<i>"+ret+"</i>", method["info"]])
-            data = data.parent
-            if data == HelpDataObject:
-                break
-        if len(rows) >= 2:
-            return cls.HtmlTableFromLists(rows)
-        else:
-            return "<p>No additional methods for this object type.</p>"
-
-    @classmethod
-    def GlobalVariablesTable(cls):
-        data = HelpDataGlobals
-        rows = []
-        rows.append(["Variable", "Type", "Description"])
-        for key in sorted(data.variables):
-            var = data.variables[key]
-            rows.append([key, "<i>" + var["type"] + "</i>", var["info"]])
-        return cls.HtmlTableFromLists(rows)
-
-    @classmethod
-    def GlobalFunctionsTable(cls):
-        data = HelpDataGlobals
-        rows = []
-        rows.append(["Method", "Arguments", "Return", "Description"])
-        for key in sorted(data.functions):
-            func = data.functions[key]
-            argText = ""
-            for name, arg in func["args"].items():
-                argText += "<b>" + name + "</b>:<i>" + arg["type"] + " </i> - " + arg["info"] + "<br/>"
-            ret = func["return"] if func["return"] else ""
-            name = key+"(" + ', '.join(func["args"].keys())  + ")"
-            rows.append([name, argText, "<i>"+ret+"</i>", func["info"]])
-        return cls.HtmlTableFromLists(rows)
-
-    @classmethod
-    def ObjectSection(cls, typeStr, title, description):
-        text = ""
-        if description:
-            text = "<p>" + description + "</p>\n"
-        return f"""
-<a name="#{typeStr}"/>
-<h2>{title}</h2>
-{text}
-<br/><br/>
-<a name="#{typeStr}.props"/>
-<h3>Properties</h3>
-{HelpData.PropertyTable(typeStr)}
-<br/><br/>
-<a name="#{typeStr}.methods"/>
-<h3>Methods</h3>
-{HelpData.MethodTable(typeStr)}
-<br/><br/>
-<a name="#{typeStr}.events"/>
-<h3>Events</h3>
-{HelpData.HandlerTable(typeStr)}
-<br/><br/>
-"""
-
-    @classmethod
-    def TOCPage(cls):
-        types = [["All Objects", "object"], ["Stack", "stack"], ["Card", "card"], ["Button", "button"],
-                 ["Text Field", "textfield"], ["Text Label", "textlabel"], ["Web View", "webview"],
-                 ["Image", "image"], ["Line & Pen", "line"],
-                 ["Oval & Rectangle", "shape"], ["Round Rectangle", "roundrect"], ["Group", "group"]]
-        text = """
-<html>
-<body bgcolor="#EEEEEE">
-<h2>Contents</h2>
-<li><a href="#top">Reference</a><br>
-<ul>
-<li><a href="#dataTypes">Data Types</a>
-<li><a href="#globalVars">Global Variables</a>
-<li><a href="#globalFuncs">Global Functions</a>
-"""
-        for type in types:
-            text += f"""
-<li><a href="#{type[1]}">{type[0]}</a><br/>
-<ul>
-<li><a href="#{type[1]}">Properties</a></li>
-<li><a href="#{type[1]+".methods"}">Methods</a></li>
-<li><a href="#{type[1]+".events"}">Events</a></li>
-</ul>
-</li>
-"""
-        text += """
-</ul>
-</ul>
-</body></html>
-        """
-        return text
-
-    @classmethod
-    def ReservedNames(cls):
-        if not cls.reservedNames:
-            cls.reservedNames = ["key_name", "mouse_pos", "message", "URL", "did_load", "other_object", "edge", "elapsed_time"]
-            cls.reservedNames.extend(HelpDataGlobals.variables.keys())
-            cls.reservedNames.extend(HelpDataGlobals.functions.keys())
-            cls.reservedNames.extend(HelpDataObject.properties.keys())
-            cls.reservedNames.extend(HelpDataObject.methods.keys())
-            cls.reservedNames.extend(HelpDataCard.properties.keys())
-            cls.reservedNames.extend(HelpDataCard.methods.keys())
-            cls.reservedNames.extend(HelpDataStack.properties.keys())
-            cls.reservedNames.extend(keyword.kwlist)
-        return cls.reservedNames
-
 HelpDataTypes = [["Type", "Description"],
                  ["<i>bool</i>", "A bool or boolean value holds a simple True or False."],
                  ["<i>int</i>", "An int or integer value holds any whole number, positive or negative."],
                  ["<i>float</i>", "A float or floating point value holds any number, including with a decimal point."],
                  ["<i>string</i>", "A string value holds text."],
                  ["<i>list</i>", "A list value is a container that holds a list of other values."],
-                 ["<i>dictionary</i>", "A dictionary value is a container that holds named items, as key, value pairs."],
+                 ["<i>dictionary</i>",
+                  "A dictionary value is a container that holds named items, as key, value pairs."],
                  ["<i>point</i>", "A point value is like a list of two numbers, x and y, that describes a location in "
                                   "the card.  For a point variable p, you can access the x value as p[0] or p.x, and "
                                   "the y value as either p[1] or p.y."],
                  ["<i>size</i>", "A size value is like a list of two numbers, width and height, that describes the "
                                  "size of an object in the card.  For a size variable s, you can access the width "
                                  "value as s[0] or s.width, and the height value as either s[1] or s.height"],
                  ["<i>object</i>", "An object value can hold any CardStock object, like a button, card, or oval."],
-                 ["<i>button, textfield, textlabel, webview, image, oval, rect, roundrect, polygon, line</i>",
-                  "A value of any of these types holds a CardStock object of that specific type."],
+                 [
+                     "<i>stack, card, button, textfield, textlabel, webview, image, oval, rect, roundrect, polygon, line</i>",
+                     "A value of any of these types holds a CardStock object of that specific type.  (Note that webview objects are not currently available on cardstock.run.)"],
                  ]
 
 
 class HelpDataGlobals():
+    types = []
     variables = {
         "self": {"type": "object",
-                  "info": "In any object's event code, <b>self</b> always refers to the object that contains this code."},
+                 "info": "In any object's event code, <b>self</b> always refers to the object that contains this code."},
         "stack": {"type": "stack",
                   "info": "The <b>stack</b> is the object that represents your whole program.  You can access cards "
                           "in this stack as stack.cardName."},
         "card": {"type": "card",
                  "info": "The <b>card</b> is the object that represents the currently loaded card in your stack.  You "
                          "can access the objects on this card as card.objectName."},
     }
     properties = variables
 
     functions = {
         "wait": {"args": {"duration": {"type": "float", "info": "Number of seconds to delay."}}, "return": None,
-                 "info": "Delays the program from running for <b>duration</b> seconds.  No movements or animations "
-                         "will happen during this time."},
+                 "info": "Delays the program from running for <b>duration</b> seconds.  Object animations that are "
+                         "already in progress or queued up will continue during this time."},
         "distance": {"args": {"pointA": {"type": "point", "info": "One location on the card."},
                               "pointB": {"type": "point", "info": "Another location on the card."}}, "return": "float",
                      "info": "Return the distance between <b>pointA</b> and <b>pointB</b>."},
         "angle_from_points": {"args": {"pointA": {"type": "point", "info": "One location on the card."},
-                              "pointB": {"type": "point", "info": "Another location on the card."}}, "return": "float",
-                     "info": "Return the angle between the bottom edge of the card, and the line from <b>pointA</b> to "
-                             "<b>pointB</b>, rotating clockwise.  This can be useful to find the rotation angle to use "
-                             "to point an object at <b>pointA</b> towards <b>pointB</b>."},
+                                       "pointB": {"type": "point", "info": "Another location on the card."}},
+                              "return": "float",
+                              "info": "Return the angle between the bottom edge of the card, and the line from <b>pointA</b> to "
+                                      "<b>pointB</b>, rotating clockwise.  This can be useful to find the rotation angle to use "
+                                      "to point an object at <b>pointA</b> towards <b>pointB</b>."},
         "rotate_point": {"args": {"point": {"type": "point", "info": "A distance in x and y, from (0,0)."},
-                              "angle": {"type": "float", "info": "An angle in degrees to rotate the point around (0,0)."}}, "return": "point",
-                     "info": "Returns a new point, calculated by rotating <b>point</b> by <b>angle</b> degrees, "
-                             "clockwise around the point (0,0).  This is useful to, for example, set the speed of a "
-                             "cannonball that should be moving in the direction that a cannon is already pointing."},
+                                  "angle": {"type": "float",
+                                            "info": "An angle in degrees to rotate the point around (0,0)."}},
+                         "return": "point",
+                         "info": "Returns a new point, calculated by rotating <b>point</b> by <b>angle</b> degrees, "
+                                 "clockwise around the point (0,0).  This is useful to, for example, set the speed of a "
+                                 "cannonball that should be moving in the direction that a cannon is already pointing."},
         "run_after_delay": {"args": {"duration": {"type": "float", "info": "Number of seconds to delay."},
-                                   "func": {"type": "function", "info": "A function to call after the delay."},
-                                   "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>func</b>."}}, "return": None,
-                          "info": "This function lets your program continue running while a timer waits for <b>duration</b> seconds, "
-                                  "and then runs the functions <b>func</b>, passing it any additional arguments you add "
-                                  "after <b>func</b>.  Movements, animations, and user interaction "
-                                  "will all continue during this time."},
+                                     "func": {"type": "function", "info": "A function to call after the delay."}},
+                            "return": None,
+                            "info": "This function lets your program continue running while a timer waits for <b>duration</b> seconds, "
+                                    "and then runs the functions <b>func</b>, passing it any additional arguments you add "
+                                    "after <b>func</b>.  Movements, animations, and user interaction "
+                                    "will all continue during this time."},
         "time": {"args": {}, "return": "float",
                  "info": "Returns the time in seconds since 'The Unix Epoch', midnight UTC on January 1st, 1970.  That "
                          "date doesn't usually matter, since most often, you'll store the time at one point in your "
                          "program, and then compare it to the new time somewhere else, to determine the difference."},
-        "paste": {"args": {}, "return": "list",
-                  "info": "Pastes any CardStock objects in the clipboard from a previous Copy or Cut command onto the "
-                          "current card, and returns a list of these pasted objects."},
         "alert": {"args": {"message": {"type": "any", "info": "Text to show in the alert dialog."}}, "return": None,
                   "info": "Shows an alert dialog to the user, with the <b>message</b> you provide, and offers an OK button."},
         "ask_yes_no": {"args": {"message": {"type": "any", "info": "Text to show in the dialog."}}, "return": "bool",
-                "info": "Shows an alert dialog to the user, with the <b>message</b> you provide, and offers Yes and No "
-                        "buttons.  Returns True if Yes is clicked, and False if No is clicked."},
+                       "info": "Shows an alert dialog to the user, with the <b>message</b> you provide, and offers Yes and No "
+                               "buttons.  Returns True if Yes is clicked, and False if No is clicked."},
         "ask_text": {"args": {"message": {"type": "any", "info": "alert text to show in the dialog."},
-                             "defaultResponse": {"type": "any", "info": "An optional default value to pre-fill the result field."}},
-                    "return": "string",
-                "info": "Shows an alert dialog to the user, with the <b>message</b> you provide, and a text field "
-                        "to enter a response, along with Ok and Cancel buttons.  Returns the user-entered text in the "
-                        "response field if the Ok button is clicked, or None if Cancel is clicked."},
-        "goto_card": {"args": {"card": {"type": "(object, string, or int)", "info": "A card object, a card name, or the number of a card to go to."}}, "return": None,
-                     "info": "Goes to the card passed in as <b>card</b>, the card with the name passed in as <b>card</b>, "
-                             "or the card number passed in as <b>card</b>.  This sends the on_hide_card event "
-                             "for the current card, and then the on_show_card event for the new card, or does nothing if "
-                             "there is no card with that name or number."},
+                              "defaultResponse": {"type": "any",
+                                                  "info": "An optional default value to pre-fill the result field."}},
+                     "return": "string",
+                     "info": "Shows an alert dialog to the user, with the <b>message</b> you provide, and a text field "
+                             "to enter a response, along with Ok and Cancel buttons.  Returns the user-entered text in the "
+                             "response field if the Ok button is clicked, or None if Cancel is clicked."},
+        "goto_card": {"args": {"card": {"type": "(object, string, or int)",
+                                        "info": "A card object, a card name, or the number of a card to go to."}},
+                      "return": None,
+                      "info": "Goes to the card passed in as <b>card</b>, the card with the name passed in as <b>card</b>, "
+                              "or the card number passed in as <b>card</b>.  This sends the on_hide_card event "
+                              "for the current card, and then the on_show_card event for the new card, or does nothing if "
+                              "there is no card with that name or number."},
         "goto_next_card": {"args": {}, "return": None,
-                         "info": "Goes to the next card in the stack.  If we're already on the last card, then loop back to "
-                                 "the first card.  This sends the on_hide_card event for the current card, and then the "
-                                 "on_show_card event for the new card."},
+                           "info": "Goes to the next card in the stack.  If we're already on the last card, then loop back to "
+                                   "the first card.  This sends the on_hide_card event for the current card, and then the "
+                                   "on_show_card event for the new card."},
         "goto_previous_card": {"args": {}, "return": None,
-                             "info": "Goes to the previous card in the stack.  If we're already on the first card, then loop back to "
-                                     "the last card.  This sends the on_hide_card event for the current card, and then the "
-                                     "on_show_card event for the new card."},
-        "run_stack": {"args": {"filename": {"type": "string", "info": "The path to a stack file to run"},
-                               "cardNumber": {"type": "int", "info": "An optional card number of the new stack to start on.  This defaults to card number 1, the first card."},
-                               "setupValue": {"type": "any", "info": "An optional value to pass into the new stack."}},
-                      "return": "any",
-                      "info": "Opens the stack at the path given by the <b>filename</b> argument, and optionally starts on "
-                              "the card number specified by the <b>cardNumber</b> argument.  If you include a "
-                              "<b>setupValue</b> argument, this will be passed into the new stack, which can access it by "
-                              "calling <b>stack.get_setup_value()</b>.  The <b>run_stack()</b> call waits "
-                              "until the new stack exits by calling <b>stack.return_from_stack(returnVal)</b>, and then "
-                              "this <b>run_stack()</b> call returns that returnVal value, or None if no returnValue was given."},
+                               "info": "Goes to the previous card in the stack.  If we're already on the first card, then loop back to "
+                                       "the last card.  This sends the on_hide_card event for the current card, and then the "
+                                       "on_show_card event for the new card."},
+        "run_stack": {
+            "args": {"filename": {"type": "string", "info": "The path to a stack file to run.  On cardstock.run, a "
+                                                            "filename can be a stack name owned by the same user as the current stack, or a full "
+                                                            "path \"username/StackName\", like \"examples/Pong\"."},
+                     "cardNumber": {"type": "int",
+                                    "info": "An optional card number of the new stack to start on.  This defaults to card number 1, the first card."},
+                     "setupValue": {"type": "any", "info": "An optional value to pass into the new stack."}},
+            "return": "any",
+            "info": "Opens the stack at the path given by the <b>filename</b> argument.  Optionally starts on "
+                    "the card number specified by the <b>cardNumber</b> argument.  If you include a "
+                    "<b>setupValue</b> argument, this will be passed into the new stack, which can access it by "
+                    "calling <b>stack.get_setup_value()</b>.  The <b>run_stack()</b> call waits "
+                    "until the new stack exits by calling <b>stack.return_from_stack(returnVal)</b>, and then "
+                    "this <b>run_stack()</b> call returns that returnVal value, or None if no returnValue was given."},
         "open_url": {"args": {"URL": {"type": "string",
-                                        "info": "This is the URL to open."},
+                                      "info": "This is the URL to open."},
                               "in_place": {"type": "bool",
-                                      "info": "Optional parameter: When running in-browser after uploading your stack, if this is set to "
-                                              "True, the <b>URL</b> will open in the current tab, instead of opening a new tab.  Defaults to False."}
+                                           "info": "Optional parameter: When running in-browser after uploading your stack, if this is set to "
+                                                   "True, the <b>URL</b> will open in the current tab, instead of opening a new tab.  Defaults to False."}
                               },
-                      "return": None,
-                      "info": "Opens the given <b>URL</b> in the default browser."},
+                     "return": None,
+                     "info": "Opens the given <b>URL</b> in the default browser."},
         "request_url": {"args": {"URL": {"type": "string",
                                          "info": "This is the URL to request."},
                                  "params": {"type": "dictionary",
-                                         "info": "This optionally holds query parameters for your request."},
+                                            "info": "This optionally holds query parameters for your request."},
                                  "headers": {"type": "dictionary",
-                                         "info": "This optionally holds HTTP headers for your request."},
+                                             "info": "This optionally holds HTTP headers for your request."},
                                  "method": {"type": "string",
-                                         "info": "This optionally holds an HTTP method name like \"GET\" or \"POST\".  "
-                                                 "Requests default to \"GET\"."},
+                                            "info": "This optionally holds an HTTP method name like \"GET\" or \"POST\".  "
+                                                    "Requests default to \"GET\"."},
                                  "timeout": {"type": "float",
-                                         "info": "This optionally allows setting a timeout in seconds, after which the "
-                                                 "request will be cancelled."},
+                                             "info": "This optionally allows setting a timeout in seconds, after which the "
+                                                     "request will be cancelled."},
                                  "on_done": {"type": "function",
-                                         "info": "This optional function is called when the request has received a "
-                                                 "response.  This callback function receives 2 arguments: an HTTP "
-                                                 "status code as an int, and the response as a string, or as binary "
-                                                 "data if the response is not text."},
-                                },
+                                             "info": "This optional function is called when the request has received a "
+                                                     "response.  This callback function receives 2 arguments: an HTTP "
+                                                     "status code as an int, and the response as a string, or as binary "
+                                                     "data if the response is not text."},
+                                 },
                         "return": None,
                         "info": "Requests the given <b>URL</b>.  If an <b>on_done function</b> is provided, this request_url() "
                                 "function will return immediately, and when the response is received, the given "
                                 "<b>on_done(status, result)</b> function will run.  If no <b>on_done</b> function is provided, "
                                 "this request_url() will wait until it gets a response, and will return the response "
                                 "data as text or binary data.  Optional <b>headers</b> and query <b>params</b> can be "
                                 "provided as dictionaries, and <b>method</b> and <b>timeout</b> can be provided as well, "
@@ -434,83 +158,84 @@
                                 "def got_result(status, text):<br/>"
                                 "&nbsp;&nbsp;&nbsp;&nbsp;if status == 200:<br/>"
                                 "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;print(text)<br/>"
                                 "request_url(\"https://google.com/\", on_done=got_result)<br/><br/>"
                                 "# Request the text from a URL, with parameters, and wait until we get it back<br/>"
                                 "jokeJson = request_url(\"https://geek-jokes.sameerkumar.website/api\", params={\"format\": \"json\"})"},
         "play_sound": {"args": {"file": {"type": "string",
-                                        "info": "This is the filename of the .wav format audio file to play, relative to where the stack file lives."}},
-                      "return": None,
-                      "info": "Starts playing the .wav formatted sound file at location <b>file</b>."},
+                                         "info": "This is the filename of the .wav format audio file to play, relative to where the stack file lives."}},
+                       "return": None,
+                       "info": "Starts playing the .wav formatted sound file at location <b>file</b>."},
         "stop_sound": {"args": {},
-                      "return": None,
-                      "info": "Stops all currently playing sounds."},
-        "broadcast_message": {"args": {"message": {"type": "string",
-                                        "info": "This is the message to send."}},
-                      "return": None,
-                      "info": "Sends the <b>message</b> to this card, and all objects on this card, causing each of their "
-                              "on_message events to run with this <b>message</b>."},
+                       "return": None,
+                       "info": "Stops all currently playing sounds."},
         "is_key_pressed": {"args": {"key_name": {"type": "string", "info": "The name of the key to check."}},
-                         "return": "bool",
-                         "info": "Returns <b>True</b> if the named keyboard key is currently pressed down, otherwise "
-                                 "returns <b>False</b>."},
+                           "return": "bool",
+                           "info": "Returns <b>True</b> if the named keyboard key is currently pressed down, otherwise "
+                                   "returns <b>False</b>."},
         "is_mouse_pressed": {"args": {},
-                         "return": "bool",
-                         "info": "Returns <b>True</b> if the main mouse button is currently pressed down, or the user "
-                                 "is touching a touch screen, otherwise returns <b>False</b>."},
+                             "return": "bool",
+                             "info": "Returns <b>True</b> if the main mouse button is currently pressed down, or the user "
+                                     "is touching a touch screen, otherwise returns <b>False</b>."},
         "is_using_touch_screen": {"args": {},
-                         "return": "bool",
-                         "info": "Returns <b>True</b> if the most recent 'mouse' event came from a touch "
-                                 "screen, otherwise returns <b>False</b>."},
+                                  "return": "bool",
+                                  "info": "Returns <b>True</b> if the most recent 'mouse' event came from a touch "
+                                          "screen, otherwise returns <b>False</b>."},
         "get_mouse_pos": {"args": {},
-                         "return": "point",
-                         "info": "Returns the current position of the mouse, whether or not it is inside of the stack "
-                                 "window.  This point's x and y values can be negative, if the mouse is to the left "
-                                 "or below the bottom left corner of the stack window."},
+                          "return": "point",
+                          "info": "Returns the current position of the mouse, whether or not it is inside of the stack "
+                                  "window.  This point's x and y values can be negative, if the mouse is to the left "
+                                  "or below the bottom left corner of the stack window."},
         "clear_focus": {"args": {},
-                             "return": None,
-                             "info": "If any TextField has focus, unfocus it, so that any typing will no longer be entered there."},
-        "ColorRGB": {"args": {"red": {"type": "float", "info": "The red component of the color as a number from 0.0 to 1.0."},
-                               "green": {"type": "float", "info": "The green component of the color as a number from 0.0 to 1.0."},
-                               "blue": {"type": "float", "info": "The blue component of the color as a number from 0.0 to 1.0."}},
-                         "return": "string",
-                         "info": "Returns an HTML color string of the form '#rrggbb' based on the red, green, and blue values given.  For example "
-                                 "<b>ColorRGB(1, 0, 0)</b> returns '#FF0000' which is bright red."},
-        "ColorHSB": {"args": {"hue": {"type": "float", "info": "The hue of the color as a number from 0.0 to 1.0, where 0 means red, and goes up through the rainbow, back to red again at 1.0."},
-                               "saturation": {"type": "float", "info": "The saturation of the color as a number from 0.0 to 1.0, where 0 means gray and 1 means fully saturated color."},
-                               "brightness": {"type": "float", "info": "The brightness component of the color as a number from 0.0 to 1.0, where 0 means black."}},
-                         "return": "string",
-                         "info": "Returns an HTML color string of the form '#rrggbb'.  For example "
-                                 "<b>ColorHSB(0, 1, 1)</b> returns '#FF0000' which is bright red."},
+                        "return": None,
+                        "info": "If any TextField has focus, unfocus it, so that any typing will no longer be entered there."},
+        "color_rgb": {
+            "args": {"red": {"type": "float", "info": "The red component of the color as a number from 0.0 to 1.0."},
+                     "green": {"type": "float",
+                               "info": "The green component of the color as a number from 0.0 to 1.0."},
+                     "blue": {"type": "float", "info": "The blue component of the color as a number from 0.0 to 1.0."}},
+            "return": "string",
+            "info": "Returns an HTML color string of the form '#rrggbb' based on the red, green, and blue values given.  For example "
+                    "<b>color_rgb(1, 0, 0)</b> returns '#FF0000' which is bright red."},
+        "color_hsb": {"args": {"hue": {"type": "float",
+                                       "info": "The hue of the color as a number from 0.0 to 1.0, where 0 means red, and goes up through the rainbow, back to red again at 1.0."},
+                               "saturation": {"type": "float",
+                                              "info": "The saturation of the color as a number from 0.0 to 1.0, where 0 means gray and 1 means fully saturated color."},
+                               "brightness": {"type": "float",
+                                              "info": "The brightness component of the color as a number from 0.0 to 1.0, where 0 means black."}},
+                      "return": "string",
+                      "info": "Returns an HTML color string of the form '#rrggbb'.  For example "
+                              "<b>color_hsb(0, 1, 1)</b> returns '#FF0000' which is bright red."},
         "Point": {"args": {"x": {"type": "float", "info": "The x (horizontal) part of this point."},
                            "y": {"type": "float", "info": "The y (vertical) part of this point."}},
-                         "return": "point",
-                         "info": "Returns a point object."},
+                  "return": "point",
+                  "info": "Returns a point object."},
         "Size": {"args": {"width": {"type": "int", "info": "The width (horizontal) part of this size."},
-                           "height": {"type": "int", "info": "The height (vertical) part of this size."}},
-                         "return": "size",
-                         "info": "Returns a size object."},
+                          "height": {"type": "int", "info": "The height (vertical) part of this size."}},
+                 "return": "size",
+                 "info": "Returns a size object."},
         "quit": {"args": {},
-                      "return": None,
-                      "info": "Stops running the stack, closes the stack window, and exits the stack viewer program."},
+                 "return": None,
+                 "info": "Stops running the stack, closes the stack window, and exits the stack viewer program."},
     }
     methods = functions
 
+
 class HelpDataObject():
     parent = None
     types = ["object"]
     properties = {
         "name": {"type": "string",
                  "info": "Every object has a <b>name</b> property.  These are forced to be unique within each card, "
                          "since these become the names of your object variables that you access from your code.  From "
                          "your code, you can get an object's name, but you can not set it."},
         "type": {"type": "string",
                  "info": "Every object has a <b>type</b> property.  It will be one of 'button', 'textfield', 'textlabel', "
-                         "'webview', 'image', 'line', 'oval', 'rect, 'roundrect', 'polygon', 'stack', 'card', 'group'.  Your code can get "
-                         "this value, but not set it."},
+                         "'webview', 'image', 'line', 'oval', 'rect, 'roundrect', 'polygon', 'stack', 'card', 'group'.  "
+                         "Your code can get this value, but not set it.  (Note that webview objects are not currently available on cardstock.run.)"},
         "data": {"type": "dictionary",
                  "info": "Every object has a <b>data</b> property.  It is a dictionary that allows you to persistently "
                          "store arbitrary data in any object within a stack that has <b>can_save</b> set to True."},
         "position": {"type": "point",
                      "info": "The <b>position</b> property is a point value that describes where on the "
                              "card this object's bottom-left corner is.  The first number, <b>x</b>, is how many pixels the object is "
                              "from the left edge of the card.  The second number, <b>y</b>, is how far up from the bottom."},
@@ -519,276 +244,305 @@
                          "The first number, <b>width</b>, is how wide the object is, and the second number, <b>height</b>, is how tall."},
         "center": {"type": "point",
                    "info": "The <b>center</b> property is a point value that describes where on the card this "
                            "object's center point is.  The first number, <b>x</b>, is how many pixels the object's center "
                            "is from the left edge of the card.  The second number, <b>y</b>, is how far up from the bottom.  "
                            "This value is not stored, but computed based on position and size."},
         "rotation": {"type": "float",
-                     "info": "This is the angle in degrees clockwise to rotate this object.  0 is upright.  Note that "
-                             "not all objects can be rotated.  Card and stack objects can not rotate, and text fields "
-                             "and web views can't rotate either."},
+                     "info": "This is the angle in degrees clockwise to rotate this object around its center.  0 is "
+                             "normal/upright.  Note that not all objects can be rotated, for example cards and stacks."},
         "speed": {"type": "point",
                   "info": "This is a point value corresponding to the current speed of the object, in pixels/second "
                           "in both the <b>x</b> and <b>y</b> directions."},
         "is_visible": {"type": "bool",
-                    "info": "<b>True</b> if this object <b>is_visible</b>, or <b>False</b> if it is hidden.  If this "
-                            "object is in a group that has been hidden, this object's <b>is_visible</b> property will be "
-                            "<b>False</b> as well."},
+                       "info": "<b>True</b> if this object <b>is_visible</b>, or <b>False</b> if it is hidden.  If this "
+                               "object is in a group that has been hidden, this object's <b>is_visible</b> property will be "
+                               "<b>False</b> as well."},
         "parent": {"type": "object",
                    "info": "<b>parent</b> is the object that contains this object.  For most objects, it is the card, unless this "
                            "object has been grouped, in which case its <b>parent</b> is the group object  A card's "
                            "<b>parent</b> is the stack.  The stack has no <b>parent</b>, so stack.parent is <b>None</b>."},
         "children": {"type": "list",
                      "info": "<b>children</b> is the list of objects that this object contains.  A stack has children "
                              "that are cards.  A card and a group can both have children objects. Other objects have "
                              "no children."},
     }
 
     methods = {
-        "copy": {"args": {},
-                 "return": None,
-                 "info": "Copies this object onto the clipboard, just like the Edit menu Copy command."},
-        "cut": {"args": {},
-                "return": None,
-                "info": "Copies this object onto the clipboard and then deletes it, just like the Edit menu Cut command."},
         "clone": {"args": {"...": {"type": "Any", "info": "optionally set more properties here.  For example, "
-                                           "include position=(10,10)"}},
+                                                          "include position=(10,10)"}},
                   "return": "object",
                   "info": "Duplicates this object, and updates the new object's name to be unique, and then returns "
                           "the new object for you to store into a variable."},
         "delete": {"args": {},
                    "return": None,
-                   "info": "Deletes this object.  Like Cut, but the object does not get copied to the clipboard."},
+                   "info": "Deletes this object."},
         "send_message": {"args": {"message": {"type": "string", "info": "The message being sent to this object."}},
-                        "return": None,
-                        "info": "Sends a <b>message</b> to this object, that the object can handle in its on_message event code.  For "
-                                "example, you could send the message 'reset' to an object, and in its on_message code, "
-                                "it could check for whether <b>message</b> == 'reset', and then set some variables back to their initial values."},
+                         "return": None,
+                         "info": "Sends a <b>message</b> to this object, that the object can handle in its on_message event code.  For "
+                                 "example, you could send the message 'reset' to an object, and in its on_message code, "
+                                 "it could check for whether <b>message</b> == 'reset', and then set some variables back to their initial values."},
         "show": {"args": {},
                  "return": None,
                  "info": "Shows this object if it was not visible."},
         "hide": {"args": {},
                  "return": None,
                  "info": "Hides this object if it was visible."},
-        "child_with_base_name": {"args": {"baseName": {"type": "string", "info": "The beginning of the name of the child object to find."}},
-                              "return": "object",
-                              "info": "Returns this object's first child object whose name starts with <b>baseName</b>.  For example, "
-                                      "if you have multiple group objects that each contain one button, named button_1, button_2, etc.,"
-                                      "then you can call each group's group.child_with_base_name('button') to get that group's button object."},
+        "child_with_base_name": {
+            "args": {"baseName": {"type": "string", "info": "The beginning of the name of the child object to find."}},
+            "return": "object",
+            "info": "Returns this object's first child object whose name starts with <b>baseName</b>.  For example, "
+                    "if you have multiple group objects that each contain one button, named button_1, button_2, etc.,"
+                    "then you can call each group's group.child_with_base_name('button') to get that group's button object."},
         "flip_horizontal": {"args": {},
-                 "return": None,
-                 "info": "Flips the object horizontally.  This only visibly changes cards, images, groups, and some shapes."},
+                            "return": None,
+                            "info": "Flips the object horizontally.  This only visibly changes cards, images, groups, and some shapes."},
         "flip_vertical": {"args": {},
-                 "return": None,
-                 "info": "Flips the object vertically.  This only visibly changes cards, images, groups, and some shapes."},
+                          "return": None,
+                          "info": "Flips the object vertically.  This only visibly changes cards, images, groups, and some shapes."},
         "order_to_front": {"args": {},
-                 "return": None,
-                 "info": "Moves this object to the front of the card or group it is contained in, in front of all other objects.  But note that "
-                         "currently, all text fields and web views will be displayed in front of other objects."},
+                           "return": None,
+                           "info": "Moves this object to the front of the card or group it is contained in, in front of all other objects."},
         "order_forward": {"args": {},
-                 "return": None,
-                 "info": "Moves this object one position closer to the front of the card or group it is contained in.  But note that "
-                         "currently, all text fields and web views will be displayed in front of other objects."},
+                          "return": None,
+                          "info": "Moves this object one position closer to the front of the card or group it is contained in."},
         "order_backward": {"args": {},
-                 "return": None,
-                 "info": "Moves this object one position closer to the back of the card or group it is contained in.  But note that "
-                         "currently, all text fields and web views will be displayed in front of other objects."},
+                           "return": None,
+                           "info": "Moves this object one position closer to the back of the card or group it is contained in."},
         "order_to_back": {"args": {},
-                 "return": None,
-                 "info": "Moves this object to the back of the card or group it is contained in, behind all other objects.  But note that "
-                         "currently, all text fields and web views will be displayed in front of other objects."},
-        "order_to_index": {"args": {"toIndex": {"type": "int", "info": "The index to move this object to, in the list of "
-                                 "the card or group's children.  Index 0 is at the back."}},
-                       "return": None,
-                         "info": "Moves this object to the given index, in the list of "
-                                 "its parent's children, with 0 being at the back.  But note that "
-                         "currently, all text fields and web views will be displayed in front of other objects."},
+                          "return": None,
+                          "info": "Moves this object to the back of the card or group it is contained in, behind all other objects."},
+        "order_to_index": {
+            "args": {"toIndex": {"type": "int", "info": "The index to move this object to, in the list of "
+                                                        "the card or group's children.  Index 0 is at the back."}},
+            "return": None,
+            "info": "Moves this object to the given index, in the list of "
+                    "its parent's children, with 0 being at the back."},
         "get_code_for_event": {"args": {"eventName": {"type": "string", "info": "The name of the event to look up."}},
-                            "return": "string",
-                            "info": "Returns a string containing this object's event code for the given "
-                                    "<b>eventName</b>.  For example, button_1.get_code_for_event('on_click') will "
-                                    "return the code in the object named button_1 for the 'on_click' event."},
+                               "return": "string",
+                               "info": "Returns a string containing this object's event code for the given "
+                                       "<b>eventName</b>.  For example, button_1.get_code_for_event('on_click') will "
+                                       "return the code in the object named button_1 for the 'on_click' event."},
         "set_code_for_event": {"args": {"eventName": {"type": "string", "info": "The name of the event to set."},
-                                     "code": {"type": "string", "info": "The code to run on this event."}},
-                            "return": None,
-                            "info": "Sets the <b>code</b> to be run when the event named <b>eventName</b> triggers for this object.  "
-                                    "For example, button_1.set_code_for_event('on_click', 'alert(\"Hello\")') will set up "
-                                    "button_1 to show an alert when clicked."},
+                                        "code": {"type": "string", "info": "The code to run on this event."}},
+                               "return": None,
+                               "info": "Sets the <b>code</b> to be run when the event named <b>eventName</b> triggers for this object.  "
+                                       "For example, button_1.set_code_for_event('on_click', 'alert(\"Hello\")') will set up "
+                                       "button_1 to show an alert when clicked."},
         "stop_handling_mouse_event": {"args": {},
-                                   "return": None,
-                                   "info": "If you call this method from your event code for any on_mouse_press(), on_mouse_move(), "
-                                           "or on_mouse_release() event, CardStock will skip running code for this event "
-                                           "for any overlapping objects underneath this object, which would otherwise "
-                                           "be run immediately after this object's event code finishes.  Calling "
-                                           "this method from any non-mouse event code does nothing.  Should be run as self.stop_handling_mouse_event()."},
+                                      "return": None,
+                                      "info": "If you call this method from your event code for any on_mouse_press(), on_mouse_move(), "
+                                              "or on_mouse_release() event, CardStock will skip running code for this event "
+                                              "for any overlapping objects underneath this object, which would otherwise "
+                                              "be run immediately after this object's event code finishes.  Calling "
+                                              "this method from any non-mouse event code does nothing.  Should be run as self.stop_handling_mouse_event()."},
         "is_touching": {"args": {"other": {"type": "object", "info": "The other object to compare to this one"}},
-                       "return": "bool",
-                       "info": "Returns <b>True</b> if this object is touching the <b>other</b> object passed into "
-                               "this function, otherwise returns <b>False</b>."},
-        "set_bounce_objects": {"args": {"objects": {"type": "list", "info": "A list of objects that this object should bounce off of"}},
-                             "return": None,
-                             "info": "Sets up this object so that it will automatically bounce off "
-                                     "of the given objects, if it intersects with an edge of "
-                                     "any of the objects in the list, while this object's speed is non-zero.  When an "
-                                     "object bounces, its on_bounce() event will run."},
-        "is_touching_point": {"args": {"point": {"type": "point", "info": "Checks whether this point is inside the object."}},
-                       "return": "bool",
-                       "info": "Returns <b>True</b> if this object is touching the <b>point</b> passed into "
-                               "this function, otherwise returns <b>False</b>."},
-        "is_touching_edge": {"args": {"other": {"type": "object", "info":"The other object to compare to this one"}},
-                           "return": "list",
-                           "info": "Returns an empty list if this object is not touching any edges of the <b>other</b> "
-                                   "object passed into this function.  If this object is touching any edges of the "
-                                   "other object, the return value will be a list including one or more of the strings:"
-                                   " 'Top', 'Bottom', 'Left', or 'Right', accordingly."},
+                        "return": "bool",
+                        "info": "Returns <b>True</b> if this object is touching the <b>other</b> object passed into "
+                                "this function, otherwise returns <b>False</b>."},
+        "set_bounce_objects": {
+            "args": {"objects": {"type": "list", "info": "A list of objects that this object should bounce off of"}},
+            "return": None,
+            "info": "Sets up this object so that it will automatically bounce off "
+                    "of the given objects, if it intersects with an edge of "
+                    "any of the objects in the list, while this object's speed is non-zero.  When an "
+                    "object bounces, its on_bounce() event will run."},
+        "is_touching_point": {
+            "args": {"point": {"type": "point", "info": "Checks whether this point is inside the object."}},
+            "return": "bool",
+            "info": "Returns <b>True</b> if this object is touching the <b>point</b> passed into "
+                    "this function, otherwise returns <b>False</b>."},
+        "is_touching_edge": {"args": {"other": {"type": "object", "info": "The other object to compare to this one"}},
+                             "return": "list",
+                             "info": "Returns an empty list if this object is not touching any edges of the <b>other</b> "
+                                     "object passed into this function.  If this object is touching any edges of the "
+                                     "other object, the return value will be a list including one or more of the strings:"
+                                     " 'Top', 'Bottom', 'Left', or 'Right', accordingly."},
         "animate_position": {"args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
-                                     "end_position": {"type": "point",
-                                                     "info": "the destination bottom-left corner position at the end of the animation"},
-                                     "on_finished": {"type": "function",
-                                                    "info": "an optional function to run when the animation finishes"},
-                                     "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>on_finished</b>."}},
-                            "return": None,
-                            "info": "Visually animates the movement of this object from its current position to <b>end_position</b>, "
-                                    "over <b>duration</b> seconds.  When the animation completes, runs the "
-                                    "<b>on_finished</b> function, if one was passed in."},
+                                      "end_position": {"type": "point",
+                                                       "info": "the destination bottom-left corner position at the end of the animation, "
+                                                               "as a 2-item list representing an x and y location, like (100,140)."},
+                                      "easing": {"type": "string",
+                                                 "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                                         "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                                         "instead of starting the animation at full speed. "
+                                                         "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                                         "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                                         "which can look abrupt, but is sometimes what you want."},
+                                      "on_finished": {"type": "function",
+                                                      "info": "an optional function to run when the animation finishes."}},
+                             "return": None,
+                             "info": "Visually animates the movement of this object from its current position to <b>end_position</b>, "
+                                     "over <b>duration</b> seconds.  When the animation completes, runs the "
+                                     "<b>on_finished</b> function, if one was passed in."},
 
         "animate_center": {"args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
-                                   "end_position": {"type": "point",
-                                                   "info": "the destination center position at the end of the animation"},
-                                   "on_finished": {"type": "function",
-                                                  "info": "an optional function to run when the animation finishes"},
-                                   "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>on_finished</b>."}},
-                          "return": None,
-                          "info": "Visually animates the movement of this object from its current position to have its center at <b>end_center</b>, "
-                                  "over <b>duration</b> seconds.  When the animation completes, runs the "
-                                  "<b>on_finished</b> function, if one was passed in."},
+                                    "end_position": {"type": "point",
+                                                     "info": "the destination center position at the end of the animation, "
+                                                             "as a 2-item list representing an x and y location, like (100,140)."},
+                                    "easing": {"type": "string",
+                                               "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                                       "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                                       "instead of starting the animation at full speed. "
+                                                       "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                                       "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                                       "which can look abrupt, but is sometimes what you want."},
+                                    "on_finished": {"type": "function",
+                                                    "info": "an optional function to run when the animation finishes"}},
+                           "return": None,
+                           "info": "Visually animates the movement of this object from its current position to have its center at <b>end_center</b>, "
+                                   "over <b>duration</b> seconds.  When the animation completes, runs the "
+                                   "<b>on_finished</b> function, if one was passed in."},
 
         "animate_size": {"args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
-                                 "end_size": {"type": "size", "info": "the final size of this object at the end of the animation"},
-                                 "on_finished": {"type": "function", "info": "an optional function to run when the animation finishes"},
-                                 "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>on_finished</b>."}},
-                        "return": None,
-                        "info": "Visually animates the <b>size</b> of this object from its current size to <b>end_size</b>, "
-                                "over <b>duration</b> seconds.  When the animation completes, runs the "
-                                "<b>on_finished</b> function, if one was passed in."},
+                                  "end_size": {"type": "size",
+                                               "info": "the final size of this object at the end of the animation, "
+                                                       "as a 2-item list representing the width, and height, like (100,50)."},
+                                  "easing": {"type": "string",
+                                             "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                                     "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                                     "instead of starting the animation at full speed. "
+                                                     "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                                     "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                                     "which can look abrupt, but is sometimes what you want."},
+                                  "on_finished": {"type": "function",
+                                                  "info": "an optional function to run when the animation finishes"}},
+                         "return": None,
+                         "info": "Visually animates the <b>size</b> of this object from its current size to <b>end_size</b>, "
+                                 "over <b>duration</b> seconds.  When the animation completes, runs the "
+                                 "<b>on_finished</b> function, if one was passed in."},
         "animate_rotation": {"args": {"duration": {"type": "float", "info": "time in seconds to run the animation"},
-                                     "end_rotation": {"type": "int",
-                                                             "info": "the final rotation angle in degrees clockwise at "
-                                                                     "the end of the animation"},
-                                     "force_direction":{"type": "int",
-                                                               "info": "an optional hint to tell CardStock which direction "
-                                                                       "you want the object to rotate.  A positive value forces "
-                                                                       "clockwise rotation, and a negative value forces counter-clockwise."},
-                                     "on_finished": {"type": "function",
-                                                    "info": "an optional function to run when the animation finishes."},
-                                     "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>on_finished</b>."}},
-                            "return": None,
-                            "info": "Visually animates changing this object's <b>rotation</b> angle to <b>end_rotation</b>, "
-                                    "over <b>duration</b> seconds.  When the animation completes, runs the "
-                                    "<b>on_finished</b> function, if one was passed in."},
+                                      "end_rotation": {"type": "int",
+                                                       "info": "the final rotation angle in degrees clockwise at "
+                                                               "the end of the animation"},
+                                      "force_direction": {"type": "int",
+                                                          "info": "an optional hint to tell CardStock which direction "
+                                                                  "you want the object to rotate.  A positive value forces "
+                                                                  "clockwise rotation, and a negative value forces counter-clockwise."},
+                                      "easing": {"type": "string",
+                                                 "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                                         "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                                         "instead of starting the animation at full speed. "
+                                                         "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                                         "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                                         "which can look abrupt, but is sometimes what you want."},
+                                      "on_finished": {"type": "function",
+                                                      "info": "an optional function to run when the animation finishes."}},
+                             "return": None,
+                             "info": "Visually animates changing this object's <b>rotation</b> angle to <b>end_rotation</b>, "
+                                     "over <b>duration</b> seconds.  When the animation completes, runs the "
+                                     "<b>on_finished</b> function, if one was passed in."},
         "stop_animating": {"args": {"property_name": {"type": "string",
-                                                    "info": "optional name of the property to stop animating, for "
-                                                            "example: \"size\" or \"position\".  If left blank, stops "
-                                                            "all animations of properties of this object."}},
+                                                      "info": "optional name of the property to stop animating, for "
+                                                              "example: \"size\" or \"position\".  If left blank, stops "
+                                                              "all animations of properties of this object."}},
                            "return": None,
                            "info": "Stops the animation specified by <b>property_name</b> from running on this object, "
                                    "or if no <b>property_name</b> is specified, stops all running animations on this "
                                    "object.  Any animated properties are left at their current, mid-animation values."},
     }
 
     handlers = {
         "on_setup": {"args": {},
-                    "info": "The <b>on_setup</b> event is run once for every object in your stack, immediately when the stack "
-                            "starts running, before showing the first card.  This is a great place to run any imports that your "
-                            "program needs, and to define functions, and set up any variables with their initial values."},
-        "on_mouse_press": {"args": {"mouse_pos": {"type": "point", "info": "This is the current position of the mouse pointer on the card."}},
-                        "info": "The <b>on_mouse_press</b> event is run when the mouse button gets pressed down inside of this object, "
-                                "and gives you the current mouse position as the point <b>mouse_pos</b>.  This event will be "
-                                "run for all objects underneath the mouse pointer, from the topmost object, down to the card "
-                                "itself, unless this propagation is stopped by calling self.stop_handling_mouse_event() from your code.  "
-                                "Note that Mouse events are run whether you use a mouse, trackpad, touchscreen, or any other pointing device."},
-        "on_mouse_move": {"args": {"mouse_pos": {"type": "point", "info": "This is the current position of the mouse pointer on the card."}},
-                        "info": "The <b>on_mouse_move</b> event is run every time the mouse moves, while over this object, whether "
-                                "or not the mouse button is down, and gives you the current mouse position as the point <b>mouse_pos</b>.  "
-                                "This event will be "
-                                "run for all objects underneath the mouse pointer, from the topmost object, down to the card "
-                                "itself, unless this propagation is stopped by calling self.stop_handling_mouse_event() from your code.  "
-                                "Note that Mouse events are run whether you use a mouse, trackpad, touchscreen, or any other pointing device."},
-        "on_mouse_release": {"args": {"mouse_pos": {"type": "point", "info": "This is the current position of the mouse pointer on the card."}},
-                      "info": "The <b>on_mouse_release</b> event is run when the mouse button is released over this object, and "
-                              "gives you the current mouse position as the point <b>mouse_pos</b>.  This event will be "
-                                "run for all objects underneath the mouse pointer, from the topmost object, down to the card "
-                                "itself, unless this propagation is stopped by calling self.stop_handling_mouse_event() from your code.  "
-                                "Note that Mouse events are run whether you use a mouse, trackpad, touchscreen, or any other pointing device."},
-        "on_mouse_enter": {"args": {"mouse_pos": {"type": "point", "info": "This is the current position of the mouse pointer on the card."}},
-                         "info": "The <b>on_mouse_enter</b> event is run when the mouse pointer moves onto this object."},
-        "on_mouse_exit": {"args": {"mouse_pos": {"type": "point", "info": "This is the current position of the mouse pointer on the card."}},
-                        "info": "The <b>on_mouse_exit</b> event is run when the mouse pointer moves back off of this object."},
-        "on_bounce": {"args": {"other_object": {"type": "object", "info": "The other object that this object just bounced off of.",},
-                              "edge": {"type": "string", "info": "The edge of the other object that we just bounced off of ('Left', 'Right', 'Top', or 'Bottom')."}},
-                     "info": "The <b>on_bounce</b> event is run whenever this object collides with an object that it "
-                             "knows to bounce off of.  Set up the list of objects that this object will bounce off "
-                             "of by calling object.set_bounce_objects(list) with that list of objects.  For example, if "
-                             "you have called ball.set_bounce_objects([card]), then the ball object will bounce off of "
-                             "the edges of the card.  And when the ball touches the top of the card, ball.speed.y will "
-                             "flip from positive to negative, so that the ball will start moving downwards, and the "
-                             "<b>on_bounce(other_object, edge)</b> event will run with other_object=card and edge='Top'."},
+                     "info": "The <b>on_setup</b> event is run once for every object in your stack, immediately when the stack "
+                             "starts running, before showing the first card.  This is a great place to run any imports that your "
+                             "program needs, and to define functions, and set up any variables with their initial values."},
+        "on_mouse_press": {"args": {
+            "mouse_pos": {"type": "point", "info": "This is the current position of the mouse pointer on the card."}},
+            "info": "The <b>on_mouse_press</b> event is run when the mouse button gets pressed down inside of this object, "
+                    "and gives you the current mouse position as the point <b>mouse_pos</b>.  This event will be "
+                    "run for all objects underneath the mouse pointer, from the topmost object, down to the card "
+                    "itself, unless this propagation is stopped by calling self.stop_handling_mouse_event() from your code.  "
+                    "Note that Mouse events are run whether you use a mouse, trackpad, touchscreen, or any other pointing device."},
+        "on_mouse_move": {"args": {
+            "mouse_pos": {"type": "point", "info": "This is the current position of the mouse pointer on the card."}},
+            "info": "The <b>on_mouse_move</b> event is run every time the mouse moves, while over this object, whether "
+                    "or not the mouse button is down, and gives you the current mouse position as the point <b>mouse_pos</b>.  "
+                    "This event will be "
+                    "run for all objects underneath the mouse pointer, from the topmost object, down to the card "
+                    "itself, unless this propagation is stopped by calling self.stop_handling_mouse_event() from your code.  "
+                    "Note that Mouse events are run whether you use a mouse, trackpad, touchscreen, or any other pointing device."},
+        "on_mouse_release": {"args": {
+            "mouse_pos": {"type": "point", "info": "This is the current position of the mouse pointer on the card."}},
+            "info": "The <b>on_mouse_release</b> event is run when the mouse button is released over this object, and "
+                    "gives you the current mouse position as the point <b>mouse_pos</b>.  This event will be "
+                    "run for all objects underneath the mouse pointer, from the topmost object, down to the card "
+                    "itself, unless this propagation is stopped by calling self.stop_handling_mouse_event() from your code.  "
+                    "Note that Mouse events are run whether you use a mouse, trackpad, touchscreen, or any other pointing device."},
+        "on_mouse_enter": {"args": {
+            "mouse_pos": {"type": "point", "info": "This is the current position of the mouse pointer on the card."}},
+            "info": "The <b>on_mouse_enter</b> event is run when the mouse pointer moves onto this object."},
+        "on_mouse_exit": {"args": {
+            "mouse_pos": {"type": "point", "info": "This is the current position of the mouse pointer on the card."}},
+            "info": "The <b>on_mouse_exit</b> event is run when the mouse pointer moves back off of this object."},
+        "on_bounce": {"args": {
+            "other_object": {"type": "object", "info": "The other object that this object just bounced off of.", },
+            "edge": {"type": "string",
+                     "info": "The edge of the other object that we just bounced off of ('Left', 'Right', 'Top', or 'Bottom')."}},
+            "info": "The <b>on_bounce</b> event is run whenever this object collides with an object that it "
+                    "knows to bounce off of.  Set up the list of objects that this object will bounce off "
+                    "of by calling object.set_bounce_objects(list) with that list of objects.  For example, if "
+                    "you have called ball.set_bounce_objects([card]), then the ball object will bounce off of "
+                    "the edges of the card.  And when the ball touches the top of the card, ball.speed.y will "
+                    "flip from positive to negative, so that the ball will start moving downwards, and the "
+                    "<b>on_bounce(other_object, edge)</b> event will run with other_object=card and edge='Top'."},
         "on_message": {"args": {"message": {"type": "string", "info": "This is the message string that was passed into "
-                                                                     "a send_message() or broadcast_message() call."}},
-                      "info": "The <b>on_message</b> event is run when broadcast_message() is called, or send_message() "
-                              "is called on this object.  The <b>message</b> string passed into send_message() or "
-                              "broadcast_message() is delivered here."},
-        "on_periodic": {"args": {"elapsed_time": {"type": "float", "info": "This is the number of seconds since the last time this event was run, normally about 0.03."}},
-                   "info": "The <b>on_periodic</b> event is run approximately 30 times per second on every object on the current page, "
-                           "and gives your object a chance to run periodic checks, for example checking for collisions using is_touching()."},
+                                                                      "a send_message() or broadcast_message() call."}},
+                       "info": "The <b>on_message</b> event is run when broadcast_message() is called, or send_message() "
+                               "is called on this object.  The <b>message</b> string passed into send_message() or "
+                               "broadcast_message() is delivered here."},
+        "on_periodic": {"args": {"elapsed_time": {"type": "float",
+                                                  "info": "This is the number of seconds since the last time this event was run, normally about 0.03."}},
+                        "info": "The <b>on_periodic</b> event is run approximately 30 times per second on every object on the current page, "
+                                "and gives your object a chance to run periodic checks, for example checking for collisions using is_touching()."},
     }
 
 
 class HelpDataButton():
     parent = HelpDataObject
     types = ["button"]
 
     properties = {
-        "title": {"type": "string",
-                  "info": "The <b>title</b> property is the visible text on the button."},
+        "text": {"type": "string",
+                 "info": "The <b>text</b> property holds the text content of this button, text label, or text field."},
         "style": {"type": "[Border, Borderless, Checkbox, Radio]",
-                   "info": "Buttons with style <b>Border</b> show a rounded rectangular border, "
-                           "depending on your computer's operating system.  This is the most commonly seen style of "
-                           "button.  The <b>Borderless</b> style behaves the same, but is drawn without a border."
-                           "You can also set style to be <b>Checkbox</b>, which allows users to alternately select and "
-                           "deselect this button, and it is drawn with a checkbox to show the selection state.  "
-                           "You can set the style to <b>Radio</b>, which allows selecting only one button at a time from a "
-                           "group of Radio buttons, and is drawn with a round selection indicator.  All <b>Radio</b> "
-                           "buttons with the same immediate parent (the Card, or a Group) are considered to be in the "
-                           "same Radio button group, and selecting any of these will automatically deselect all of the "
-                           "rest in the group."},
+                  "info": "Buttons with style <b>Border</b> show a rounded rectangular border, "
+                          "depending on your computer's operating system.  This is the most commonly seen style of "
+                          "button.  The <b>Borderless</b> style behaves the same, but is drawn without a border."
+                          "You can also set style to be <b>Checkbox</b>, which allows users to alternately select and "
+                          "deselect this button, and it is drawn with a checkbox to show the selection state.  "
+                          "You can set the style to <b>Radio</b>, which allows selecting only one button at a time from a "
+                          "group of Radio buttons, and is drawn with a round selection indicator.  All <b>Radio</b> "
+                          "buttons with the same immediate parent (the Card, or a Group) are considered to be in the "
+                          "same Radio button group, and selecting any of these will automatically deselect all of the "
+                          "rest in the group."},
         "is_selected": {"type": "bool",
                         "info": "For Border and Borderless style buttons, this is always False.  For Checkbox style "
                                 "buttons, this is True when the Checkbox is checked.  For Radio buttons, this is True "
                                 "when this Radio button is the selected button in its group."}
     }
 
     methods = {
         "click": {"args": {}, "return": None,
-                    "info": "Runs this button's on_click event code."},
+                  "info": "Runs this button's on_click event code."},
         "get_radio_group": {"args": {}, "return": "list",
-                  "info": "If this button is a Radio button, then return a list of all Radio buttons in this button's "
-                          "Radio group, which is defined as all Radio buttons with the same direct parent (Card or "
-                          "Group).  Otherwise returns an empty list."},
+                            "info": "If this button is a Radio button, then return a list of all Radio buttons in this button's "
+                                    "Radio group, which is defined as all Radio buttons with the same direct parent (Card or "
+                                    "Group).  Otherwise returns an empty list."},
         "get_radio_group_selection": {"args": {}, "return": "button",
-                  "info": "If this button is a Radio button, then return the selected Radio button in this button's "
-                          "Radio group. If this button is not a Radio button, or if none of the buttons in the group are "
-                          "selected, returns None."},
+                                      "info": "If this button is a Radio button, then return the selected Radio button in this button's "
+                                              "Radio group. If this button is not a Radio button, or if none of the buttons in the group are "
+                                              "selected, returns None."},
     }
 
     handlers = {
         "on_click": {"args": {},
-                    "info": "The <b>on_click</b> event is run when a user clicks down on this button, and releases the "
-                            "mouse, while still inside the button.  It is also run when the button's click() "
-                            "method is called."},
+                     "info": "The <b>on_click</b> event is run when a user clicks down on this button, and releases the "
+                             "mouse, while still inside the button.  It is also run when the button's click() "
+                             "method is called."},
         "on_selection_changed": {"args": {"is_selected": {"type": "bool",
                                                           "info": "The new selection state of this button.  True "
                                                                   "if this button was just selected, otherwise False."}},
                                  "info": "Used by Checkbox and Radio style buttons only, the <b>on_selection_changed</b> event "
                                          "is run when a user selects or deselects this button. When a Radio button is "
                                          "selected, this event will be run first for any previously selected Radio "
                                          "button, with <b>is_selected</b> = False to deselect the old choice, and then "
@@ -798,188 +552,217 @@
 
 class HelpDataTextField():
     parent = HelpDataObject
     types = ["textfield"]
 
     properties = {
         "text": {"type": "string",
-                 "info": "The <b>text</b> property holds the contents of this field as a string."},
+                 "info": "The <b>text</b> property holds the text content of this button, text label, or text field."},
         "alignment": {"type": "[Left, Center, Right]",
-                      "info": "By default, text fields start aligned to the left, but you can change this property to make "
-                              "your text centered, or aligned to the right."},
+                      "info": "By default, text labels and text fields start aligned to the left, but you can change "
+                              "this property to make your text centered, or aligned to the right."},
         "text_color": {"type": "string",
-                      "info": "The color used for the text in this field.  This can be a color word like red, or an "
-                              "HTML color like #333333 for dark gray."},
+                       "info": "The color used for the text in this text label or text field.  This can be a color "
+                               "word like red, or an HTML color like #333333 for dark gray."},
         "font": {"type": "[Default, Serif, Sans-Serif, Mono]",
-                 "info": "The <b>font</b> used for the text in this field."},
+                 "info": "The <b>font</b> used for the text in this label or field."},
         "font_size": {"type": "int",
-                     "info": "The point size for the font used for the text in this field."},
+                      "info": "The point size for the font used for the text in this label or field."},
         "is_bold": {"type": "bool",
-                 "info": "Set to True if this object's text is bold."},
+                    "info": "Set to True if this object's text is bold."},
         "is_italic": {"type": "bool",
-                   "info": "Set to True if this object's text is italic."},
+                      "info": "Set to True if this object's text is italic."},
         "has_focus": {"type": "bool",
-                     "info": "<b>True</b> if this TextField is focused (if it is selected for typing into), otherwise "
-                             "<b>False</b>. This value is not settable, but you can call the method focus() to try to "
-                             "focus this Field."},
+                      "info": "<b>True</b> if this TextField is focused (if it is selected for typing into), otherwise "
+                              "<b>False</b>. This value is not settable, but you can call the method focus() to try to "
+                              "focus this Field."},
         "selection": {"type": "list",
                       "info": "A text field's <b>selection</b> value is a list of 2 numbers.  The first is the start position "
                               "of the selection within the field's text, and the second is the position of the end "
                               "of the selection.  For example, if the text is 'Hello', and the 'He' is selected, then "
                               "the value of <b>selection</b> would be (0, 2)."},
         "selected_text": {"type": "string",
-                         "info": "A text field's <b>selected_text</b> value is the string that is currently selected within "
-                                 "the field's text.  For example, if the text is 'Hello', and the 'He' is selected, "
-                                 "then the <b>selected_text</b> value would be 'He'."},
+                          "info": "A text field's <b>selected_text</b> value is the string that is currently selected within "
+                                  "the field's text.  For example, if the text is 'Hello', and the 'He' is selected, "
+                                  "then the <b>selected_text</b> value would be 'He'."},
         "is_editable": {"type": "bool",
-                     "info": "By default text fields can be edited by the user.  But you can set this to <b>False</b> "
-                             "so that the text can not be edited."},
+                        "info": "By default text fields can be edited by the user.  But you can set this to <b>False</b> "
+                                "so that the text can not be edited."},
         "is_multiline": {"type": "bool",
-                      "info": "By default, text fields hold only one line of text.  But you can set the "
-                              "<b>is_multiline</b> property to <b>True</b> to let them hold multiple lines of text."},
+                         "info": "By default, text fields hold only one line of text.  But you can set the "
+                                 "<b>is_multiline</b> property to <b>True</b> to let them hold multiple lines of text."},
     }
 
     methods = {
-        "animate_font_size": {"args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
-                                      "end_size": {"type": "string",
-                                                   "info": "the final font_size at the end of the animation"},
-                                      "on_finished": {"type": "function",
-                                                     "info": "an optional function to run when the animation finishes."},
-                                      "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>on_finished</b>."}},
-                             "return": None,
-                             "info": "Visually animates changing this object's <b>font_size</b> to <b>end_size</b>, "
-                                     "over <b>duration</b> seconds.  When the animation completes, runs the "
-                                     "<b>on_finished</b> function, if one was passed in."},
-        "animate_text_color": {"args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
-                                      "end_color": {"type": "string",
-                                                   "info": "the final text_color at the end of the animation"},
-                                      "on_finished": {"type": "function",
-                                                     "info": "an optional function to run when the animation finishes."},
-                                      "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>on_finished</b>."}},
-                             "return": None,
-                             "info": "Visually animates fading this object's <b>text_color</b> to <b>end_color</b>, "
-                                     "over <b>duration</b> seconds.  When the animation completes, runs the "
-                                     "<b>on_finished</b> function, if one was passed in."},
+        "animate_font_size": {
+            "args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
+                     "end_size": {"type": "string",
+                                  "info": "the final font_size at the end of the animation"},
+                     "easing": {"type": "string",
+                                "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                        "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                        "instead of starting the animation at full speed. "
+                                        "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                        "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                        "which can look abrupt, but is sometimes what you want."},
+                     "on_finished": {"type": "function",
+                                     "info": "an optional function to run when the animation finishes."}},
+            "return": None,
+            "info": "Visually animates changing this object's <b>font_size</b> to <b>end_size</b>, "
+                    "over <b>duration</b> seconds.  When the animation completes, runs the "
+                    "<b>on_finished</b> function, if one was passed in."},
+        "animate_text_color": {
+            "args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
+                     "end_color": {"type": "string",
+                                   "info": "the final text_color at the end of the animation"},
+                     "easing": {"type": "string",
+                                "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                        "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                        "instead of starting the animation at full speed. "
+                                        "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                        "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                        "which can look abrupt, but is sometimes what you want."},
+                     "on_finished": {"type": "function",
+                                     "info": "an optional function to run when the animation finishes."}},
+            "return": None,
+            "info": "Visually animates fading this object's <b>text_color</b> to <b>end_color</b>, "
+                    "over <b>duration</b> seconds.  When the animation completes, runs the "
+                    "<b>on_finished</b> function, if one was passed in."},
         "enter": {"args": {}, "return": None,
-                    "info": "Runs this text field's on_text_enter event code."},
+                  "info": "Runs this text field's on_text_enter event code."},
         "select_all": {"args": {}, "return": None,
-                      "info": "Selects all text in this text field."},
+                       "info": "Selects all text in this text field."},
         "focus": {"args": {},
                   "return": None,
                   "info": "Selects this TextField so that it will handle key presses.  Typed words will get entered "
                           "into the currently focused TextField."},
     }
 
     handlers = {
         "on_text_changed": {"args": {},
-                          "info": "The <b>on_text_changed</b> event is run every time the user makes any change to the text in this text field."},
+                            "info": "The <b>on_text_changed</b> event is run every time the user makes any change to the text in this text field."},
         "on_text_enter": {"args": {},
-                        "info": "The <b>on_text_enter</b> event is run when the user types the Enter key in this text field."},
+                          "info": "The <b>on_text_enter</b> event is run when the user types the Enter key in this text field."},
     }
 
 
 class HelpDataTextLabel():
     parent = HelpDataObject
     types = ["textlabel"]
 
     properties = {
         "text": {"type": "string",
-                 "info": "The <b>text</b> property is the text contents of this label."},
+                 "info": "The <b>text</b> property holds the text content of this button, text label, or text field."},
         "alignment": {"type": "[Left, Center, Right]",
-                      "info": "By default text fields start aligned to the left, but you can change this property to make "
-                              "your text centered, or aligned to the right."},
+                      "info": "By default, text labels and text fields start aligned to the left, but you can change "
+                              "this property to make your text centered, or aligned to the right."},
         "can_auto_shrink": {"type": "bool",
-                       "info": "When the <b>can_auto_shrink</b> property is True, the <b>font_size</b> of the text in this "
-                               "label will shrink if needed, to fit into the label object's current size."},
+                            "info": "When the <b>can_auto_shrink</b> property is True, the <b>font_size</b> of the text in this "
+                                    "label will shrink if needed, to fit into the label object's current size."},
         "text_color": {"type": "string",
-                      "info": "The color used for the text in this label.  This can be a color word like red, or an "
-                              "HTML color like #333333 for dark gray."},
+                       "info": "The color used for the text in this text label or text field.  This can be a color "
+                               "word like red, or an HTML color like #333333 for dark gray."},
         "font": {"type": "[Default, Serif, Sans-Serif, Mono]",
-                 "info": "The <b>font</b> used for the text in this label."},
+                 "info": "The <b>font</b> used for the text in this label or field."},
         "font_size": {"type": "int",
-                     "info": "The point size for the font used for the text in this label."},
+                      "info": "The point size for the font used for the text in this label or field."},
         "is_bold": {"type": "bool",
-                 "info": "Set to True if this object's text is bold."},
+                    "info": "Set to True if this object's text is bold."},
         "is_italic": {"type": "bool",
-                   "info": "Set to True if this object's text is italic."},
+                      "info": "Set to True if this object's text is italic."},
         "is_underlined": {"type": "bool",
-                       "info": "Set to True if this object's text is underlined."},
+                          "info": "Set to True if this object's text is underlined."},
     }
 
     methods = {
-        "animate_font_size": {"args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
-                                      "end_size": {"type": "string",
-                                                   "info": "the final font_size at the end of the animation"},
-                                      "on_finished": {"type": "function",
-                                                     "info": "an optional function to run when the animation finishes."},
-                                      "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>on_finished</b>."}},
-                             "return": None,
-                             "info": "Visually animates changing this object's <b>font_size</b> to <b>end_size</b>, "
-                                     "over <b>duration</b> seconds.  When the animation completes, runs the "
-                                     "<b>on_finished</b> function, if one was passed in."},
-        "animate_text_color": {"args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
-                                      "end_color": {"type": "string",
-                                                   "info": "the final text_color at the end of the animation"},
-                                      "on_finished": {"type": "function",
-                                                     "info": "an optional function to run when the animation finishes."},
-                                      "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>on_finished</b>."}},
-                             "return": None,
-                             "info": "Visually animates fading this object's <b>text_color</b> to <b>end_color</b>, "
-                                     "over <b>duration</b> seconds.  When the animation completes, runs the "
-                                     "<b>on_finished</b> function, if one was passed in."},
+        "animate_font_size": {
+            "args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
+                     "end_size": {"type": "string",
+                                  "info": "the final font_size at the end of the animation"},
+                     "easing": {"type": "string",
+                                "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                        "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                        "instead of starting the animation at full speed. "
+                                        "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                        "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                        "which can look abrupt, but is sometimes what you want."},
+                     "on_finished": {"type": "function",
+                                     "info": "an optional function to run when the animation finishes."}},
+            "return": None,
+            "info": "Visually animates changing this object's <b>font_size</b> to <b>end_size</b>, "
+                    "over <b>duration</b> seconds.  When the animation completes, runs the "
+                    "<b>on_finished</b> function, if one was passed in."},
+        "animate_text_color": {
+            "args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
+                     "end_color": {"type": "string",
+                                   "info": "the final text_color at the end of the animation"},
+                     "easing": {"type": "string",
+                                "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                        "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                        "instead of starting the animation at full speed. "
+                                        "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                        "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                        "which can look abrupt, but is sometimes what you want."},
+                     "on_finished": {"type": "function",
+                                     "info": "an optional function to run when the animation finishes."}},
+            "return": None,
+            "info": "Visually animates fading this object's <b>text_color</b> to <b>end_color</b>, "
+                    "over <b>duration</b> seconds.  When the animation completes, runs the "
+                    "<b>on_finished</b> function, if one was passed in."},
     }
 
     handlers = {}
 
 
 class HelpDataWebView():
     parent = HelpDataObject
     types = ["webview"]
 
     properties = {
         "URL": {"type": "string",
                 "info": "This is the current URL being shown by the Web View.  Set this property to go to a web page."},
         "HTML": {"type": "string",
-                "info": "This is the current HTML content of the webview."},
+                 "info": "This is the current HTML content of the webview."},
         "can_go_back": {"type": "bool",
-                "info": "This is True if the webview has pages in its history to go back to, otherwise it is False. "
-                        "This value can be read but not set."},
+                        "info": "This is True if the webview has pages in its history to go back to, otherwise it is False. "
+                                "This value can be read but not set."},
         "can_go_forward": {"type": "bool",
-                "info": "This is True if the webview has gone back, and has history pages available to go forward to, "
-                        "otherwise it is False.  This value can be read but not set."},
+                           "info": "This is True if the webview has gone back, and has history pages available to go forward to, "
+                                   "otherwise it is False.  This value can be read but not set."},
         "allowed_hosts": {"type": "list",
-                 "info": "If the <b>allowed_hosts</b> list is empty, then this WebView will be allowed to load any URL. "
-                         "If this list contains hostnames like 'google.com', then the WebView will only be allowed to "
-                         "load URLs from these web hosts, and attempts to load other URLs, either by setting the "
-                         "<b>URL</b> property directly, or by clicking a link, will fail."},
+                          "info": "If the <b>allowed_hosts</b> list is empty, then this WebView will be allowed to load any URL. "
+                                  "If this list contains hostnames like 'google.com', then the WebView will only be allowed to "
+                                  "load URLs from these web hosts, and attempts to load other URLs, either by setting the "
+                                  "<b>URL</b> property directly, or by clicking a link, will fail."},
     }
 
     methods = {
         "run_java_script": {"args": {"code": {"type": "string", "info": "The JavaScript code to run in this Web View"}},
                             "return": "string",
                             "info": "Runs the given JavaScript <b>code</b> and returns any result."},
         "go_forward": {"args": {},
-                      "return": None,
-                      "info": "Make the WebView go forward through its history list."},
+                       "return": None,
+                       "info": "Make the WebView go forward through its history list."},
         "go_back": {"args": {},
-                   "return": None,
-                   "info": "Make the WebView go back through its history list."},
+                    "return": None,
+                    "info": "Make the WebView go back through its history list."},
     }
 
     handlers = {
-        "on_done_loading": {"args": {"URL": {"type": "string", "info": "This is the URL of the web page that just loaded."},
-                                   "did_load": {"type": "bool", "info": "True if the URL loaded successfully, otherwise False."}},
-                          "info": "The <b>on_done_loading</b> event is run whenever a web page finishes loading.",
-                          },
+        "on_done_loading": {
+            "args": {"URL": {"type": "string", "info": "This is the URL of the web page that just loaded."},
+                     "did_load": {"type": "bool", "info": "True if the URL loaded successfully, otherwise False."}},
+            "info": "The <b>on_done_loading</b> event is run whenever a web page finishes loading.",
+        },
         "on_card_stock_link": {
             "args": {"message": {"type": "string", "info": "This is the message part of a 'cardstock:message' URL."}},
             "info": "The <b>on_card_stock_link</b> event is run whenever a web page tries to load a URL of the form "
                     "cardstock:message.  You can add code in this event to respond to actions in a web page that call "
                     "a cardstock: URL.",
-            },
+        },
     }
 
 
 class HelpDataImage():
     parent = HelpDataObject
     types = ["image"]
 
@@ -1003,598 +786,1118 @@
 class HelpDataGroup():
     parent = HelpDataObject
     types = ["group"]
 
     properties = {}
 
     methods = {
-        "ungroup":{"args": {},
-                   "return": None,
-                   "info": "Ungroups this group.  Removes the group object from the card, and adds all of its "
-                           "children back onto the card as individual objects."},
+        "ungroup": {"args": {},
+                    "return": None,
+                    "info": "Ungroups this group.  Removes the group object from the card, and adds all of its "
+                            "children back onto the card as individual objects."},
         "stop_all_animating": {"args": {"property_name": {"type": "string",
-                                       "info": "optional name of the property to stop animating, for "
-                                               "example: \"size\" or \"position\".  If left blank, stops "
-                                               "all animations of properties of this group and its children."}},
-                              "return": None,
-                              "info": "Stops the animation specified by <b>property_name</b> from running on this group "
-                                      "and on all objects in this group, or if no <b>property_name</b> is specified, "
-                                      "stops all running animations on this group and on all objects in this group.  "
-                                      "Any animated properties are left at their current, mid-animation values."},
+                                                          "info": "optional name of the property to stop animating, for "
+                                                                  "example: \"size\" or \"position\".  If left blank, stops "
+                                                                  "all animations of properties of this group and its children."}},
+                               "return": None,
+                               "info": "Stops the animation specified by <b>property_name</b> from running on this group "
+                                       "and on all objects in this group, or if no <b>property_name</b> is specified, "
+                                       "stops all running animations on this group and on all objects in this group.  "
+                                       "Any animated properties are left at their current, mid-animation values."},
     }
 
     handlers = {}
 
 
 class HelpDataLine():
     parent = HelpDataObject
     types = ["line", "pen"]
 
     properties = {
         "pen_thickness": {"type": "int",
-                         "info": "The thickness of the line or shape border in pixels."},
+                          "info": "The thickness of the line or shape border in pixels."},
+        "pen_style": {"type": "[Solid, Long-Dashes, Dashes, Dots]",
+                      "info": "The pen style of this line or shape border."},
         "pen_color": {"type": "string",
-                     "info": "The color used for the line or shape border.  This can be a color word like red, or an "
-                             "HTML color like #FF0000 for pure red."},
-        "points":   {"type": "list",
-                     "info": "This is the list of points that define this line, pen, or polygon object.  The other "
-                             "shape types do not provide access to this list."},
+                      "info": "The color used for the line or shape border.  This can be a color word like red, or an "
+                              "HTML color like #FF0000 for pure red."},
+        "points": {"type": "list",
+                   "info": "This is the list of points that define this line, pen, or polygon object.  The other "
+                           "shape types do not provide access to this list."},
     }
 
     methods = {
-        "animate_pen_thickness": {"args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
-                                 "end_thickness": {"type": "int",
-                                                 "info": "the final pen_thickness at the end of the animation"},
-                                 "on_finished": {"type": "function",
-                                                "info": "an optional function to run when the animation finishes."},
-                                         "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>on_finished</b>."}},
-                        "return": None,
-                        "info": "Visually animates changing this object's <b>pen_thickness</b> to <b>end_thickness</b>, "
-                                "over <b>duration</b> seconds.  When the animation completes, runs the "
-                                "<b>on_finished</b> function, if one was passed in."},
-
-        "animate_pen_color": {"args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
-                                 "end_color": {"type": "string",
-                                                 "info": "the final pen color at the end of the animation"},
-                                 "on_finished": {"type": "function",
-                                                "info": "an optional function to run when the animation finishes."},
-                                     "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>on_finished</b>."}},
-                        "return": None,
-                        "info": "Visually animates fading this object's <b>pen_color</b> to <b>end_color</b>, "
-                                "over <b>duration</b> seconds.  When the animation completes, runs the "
-                                "<b>on_finished</b> function, if one was passed in."},
+        "animate_pen_thickness": {
+            "args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
+                     "end_thickness": {"type": "int",
+                                       "info": "the final pen_thickness at the end of the animation"},
+                     "easing": {"type": "string",
+                                "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                        "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                        "instead of starting the animation at full speed. "
+                                        "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                        "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                        "which can look abrupt, but is sometimes what you want."},
+                     "on_finished": {"type": "function",
+                                     "info": "an optional function to run when the animation finishes."}},
+            "return": None,
+            "info": "Visually animates changing this object's <b>pen_thickness</b> to <b>end_thickness</b>, "
+                    "over <b>duration</b> seconds.  When the animation completes, runs the "
+                    "<b>on_finished</b> function, if one was passed in."},
+
+        "animate_pen_color": {
+            "args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
+                     "end_color": {"type": "string",
+                                   "info": "the final pen color at the end of the animation"},
+                     "easing": {"type": "string",
+                                "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                        "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                        "instead of starting the animation at full speed. "
+                                        "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                        "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                        "which can look abrupt, but is sometimes what you want."},
+                     "on_finished": {"type": "function",
+                                     "info": "an optional function to run when the animation finishes."}},
+            "return": None,
+            "info": "Visually animates fading this object's <b>pen_color</b> to <b>end_color</b>, "
+                    "over <b>duration</b> seconds.  When the animation completes, runs the "
+                    "<b>on_finished</b> function, if one was passed in."},
     }
 
     handlers = {}
 
 
 class HelpDataShape():
     parent = HelpDataLine
     types = ["oval", "rect", "polygon"]
 
     properties = {
         "fill_color": {"type": "string",
-                      "info": "The color used to fill the inside area of the shape.  This can be a color word like "
-                              "red, or an HTML color like #FF0000 for pure red."},
+                       "info": "The color used to fill in a shape, or the background of a card.  This can be a color word like "
+                               "red, or an HTML color like #FF0000 for pure red."},
     }
 
     methods = {
-        "animate_fill_color": {"args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
-                                     "end_color": {"type": "string",
-                                                  "info": "the final fill_color at the end of the animation"},
-                                     "on_finished": {"type": "function",
-                                                    "info": "an optional function to run when the animation finishes."},
-                                      "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>on_finished</b>."}},
-                            "return": None,
-                            "info": "Visually animates fading this object's <b>fill_color</b> to <b>end_color</b>, "
-                                    "over <b>duration</b> seconds.  When the animation completes, runs the "
-                                    "<b>on_finished</b> function, if one was passed in."},
+        "animate_fill_color": {
+            "args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
+                     "end_color": {"type": "string",
+                                   "info": "the final fill_color at the end of the animation"},
+                     "easing": {"type": "string",
+                                "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                        "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                        "instead of starting the animation at full speed. "
+                                        "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                        "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                        "which can look abrupt, but is sometimes what you want."},
+                     "on_finished": {"type": "function",
+                                     "info": "an optional function to run when the animation finishes."}},
+            "return": None,
+            "info": "Visually animates fading this object's <b>fill_color</b> to <b>end_color</b>, "
+                    "over <b>duration</b> seconds.  When the animation completes, runs the "
+                    "<b>on_finished</b> function, if one was passed in."},
     }
 
     handlers = {}
 
 
 class HelpDataRoundRectangle():
     parent = HelpDataShape
     types = ["roundrect"]
 
     properties = {
         "corner_radius": {"type": "int",
-                         "info": "The radius used to draw this round rectangle's rounded corners."},
+                          "info": "The radius used to draw this round rectangle's rounded corners."},
     }
 
     methods = {
-        "animate_corner_radius": {"args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
-                                         "end_corner_radius": {"type": "int",
-                                                          "info": "the final corner_radius at the end of the animation"},
-                                         "on_finished": {"type": "function",
-                                                        "info": "an optional function to run when the animation finishes."},
-                                         "*args": {"type": "any", "info": "0 or more arguments and/or keyword arguments to pass into <b>on_finished</b>."}},
-                                "return": None,
-                                "info": "Visually animates changing this round rectangle's <b>corner_radius</b> to <b>end_corner_radius</b>, "
-                                        "over <b>duration</b> seconds.  When the animation completes, runs the <b>on_finished</b> function, "
-                                        "if one was passed in."},
+        "animate_corner_radius": {
+            "args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
+                     "end_corner_radius": {"type": "int",
+                                           "info": "the final corner_radius at the end of the animation"},
+                     "easing": {"type": "string",
+                                "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                        "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                        "instead of starting the animation at full speed. "
+                                        "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                        "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                        "which can look abrupt, but is sometimes what you want."},
+                     "on_finished": {"type": "function",
+                                     "info": "an optional function to run when the animation finishes."}},
+            "return": None,
+            "info": "Visually animates changing this round rectangle's <b>corner_radius</b> to <b>end_corner_radius</b>, "
+                    "over <b>duration</b> seconds.  When the animation completes, runs the <b>on_finished</b> function, "
+                    "if one was passed in."},
     }
 
     handlers = {}
 
 
 class HelpDataCard():
     parent = HelpDataObject
     types = ["card"]
 
     properties = {
         "fill_color": {"type": "string",
-                    "info": "The fill_color is used to fill in the background of this card.  This can be a color word like white, "
-                            "or an HTML color like #EEEEEE for a light grey."},
+                       "info": "The fill_color is used to fill in a shape, or the background of a card.  This can be a color word like white, "
+                               "or an HTML color like #EEEEEE for a light grey."},
         "number": {"type": "int",
-                  "info": "This is the card number of this card.  The first card is <b>number</b> 1.  You can "
-                          "read this value, but not set it."},
-        "can_save": {"type": "bool",
-                    "info": "If <b>can_save</b> is <b>True</b>, the user can save the stack while running it. "
-                            "If it's <b>False</b>, the user can't save, so the stack will always start out in the same "
-                            "state."},
+                   "info": "This is the card number of this card.  The first card is <b>number</b> 1.  You can "
+                           "read this value, but not set it."},
         "can_resize": {"type": "bool",
-                      "info": "If <b>can_resize</b> is <b>True</b>, the user can resize the stack window while running it. "
-                              "If it's <b>False</b>, the user can't resize the window while the stack runs."},
+                       "info": "If <b>can_resize</b> is <b>True</b>, then when running, the card will automatically adjust its size "
+                               "to fill the browser window on cardstock.run, or on desktop, will allow the user to "
+                               "manually resize the window."},
     }
 
     methods = {
-        "add_button": {"args": {"name": {"type": "string", "info": "an optional argument giving the name to use for this "
-                                                                "new Button object.  If omitted, the name will be "
-                                                                "'button_{N}'."},
-                               "...": {"type": "Any", "info": "optionally set more properties here.  For example, "
-                                                              "include position=(10,10)"}},
-                    "return": "button",
-                    "info": "Adds a new Button to the card, and returns the new object."},
-        "add_text_field": {"args": {"name": {"type": "string", "info": "an optional argument giving the name to use for this "
-                                                                "new Text Field object.  If omitted, the name will be "
-                                                                "'field_{N}'."},
-                                  "...": {"type": "Any", "info": "optionally set more properties here.  For example, "
-                                                                 "include position=(10,10)"}},
-                    "return": "textfield",
-                    "info": "Adds a new Text Field to the card, and returns the new object."},
-        "add_text_label": {"args": {"name": {"type": "string", "info": "an optional argument giving the name to use for this "
-                                                                "new Text Label object.  If omitted, the name will be "
-                                                                "'label_{N}'."},
-                                  "...": {"type": "Any", "info": "optionally set more properties here.  For example, "
-                                                                 "include position=(10,10)"}},
-                         "return": "textlabel",
-                    "info": "Adds a new Text Label object to the card, and returns the new object."},
-        "add_image": {"args": {"name": {"type": "string", "info": "an optional argument giving the name to use for this "
-                                                                "new Image object.  If omitted, the name will be "
-                                                                "'image_{N}'."},
-                              "...": {"type": "Any", "info": "optionally set more properties here.  For example, "
-                                                             "include position=(10,10)"}},
-                     "return": "image",
+        "broadcast_message": {"args": {"message": {"type": "string",
+                                                   "info": "This is the message to send."}},
+                              "return": None,
+                              "info": "Sends the <b>message</b> to all objects on this card, or to all objects on all cards if called on the stack, causing each of the objects' "
+                                      "on_message events to run with this <b>message</b>."},
+        "add_button": {
+            "args": {
+                "...": {"type": "Any", "info": "optionally set any of the new object's properties here.  For example: "
+                                               "name=\"thingy\", position=(20,200), size=(100,50)"}},
+            "return": "button",
+            "info": "Adds a new Button to the card, and returns the new object."},
+        "add_text_field": {
+            "args": {"...": {"type": "Any", "info": "optionally set more properties here.  For example: "
+                                                    "name=\"thingy\", position=(20,200), size=(100,50)"}},
+            "return": "textfield",
+            "info": "Adds a new Text Field to the card, and returns the new object."},
+        "add_text_label": {
+            "args": {"...": {"type": "Any", "info": "optionally set more properties here.  For example: "
+                                                    "name=\"thingy\", position=(20,200), size=(100,50)"}},
+            "return": "textlabel",
+            "info": "Adds a new Text Label object to the card, and returns the new object."},
+        "add_image": {
+            "args": {"...": {"type": "Any", "info": "optionally set more properties here.  For example: "
+                                                    "name=\"thingy\", position=(20,200), size=(100,50)"}},
+            "return": "image",
+            "info": "Adds a new Image to the card, and returns the new object."},
+        "add_oval": {"args": {"...": {"type": "Any", "info": "optionally set more properties here.  For example: "
+                                                             "name=\"thingy\", position=(20,200), size=(100,50)"}},
+                     "return": "oval",
                      "info": "Adds a new Image to the card, and returns the new object."},
-        "add_oval": {"args": {"name": {"type": "string", "info": "an optional argument giving the name to use for this "
-                                                                "new Oval object.  If omitted, the name will be "
-                                                                "'shape_{N}'."},
-                             "...": {"type": "Any", "info": "optionally set more properties here.  For example, "
-                                                            "include position=(10,10)"}},
-                    "return": "oval",
-                    "info": "Adds a new Image to the card, and returns the new object."},
-        "add_rectangle": {"args": {"name": {"type": "string", "info": "an optional argument giving the name to use for this "
-                                                                "new Rectangle object.  If omitted, the name will be "
-                                                                "'shape_{N}'."},
-                                  "...": {"type": "Any", "info": "optionally set more properties here.  For example, "
-                                                                 "include position=(10,10)"}},
-                         "return": "rect",
-                    "info": "Adds a new Rectangle to the card, and returns the new object."},
-        "add_round_rectangle": {"args": {"name": {"type": "string", "info": "an optional argument giving the name to use for this "
-                                                                "new Round Rectangle object.  If omitted, the name will be "
-                                                                "'shape_{N}'."},
-                                       "...": {"type": "Any", "info": "optionally set more properties here.  For example, "
-                                                       "include position=(10,10)"}},
-                              "return": "roundrect",
-                    "info": "Adds a new Round Rectangle to the card, and returns the new object."},
+        "add_rectangle": {
+            "args": {"...": {"type": "Any", "info": "optionally set more properties here.  For example: "
+                                                    "name=\"thingy\", position=(20,200), size=(100,50)"}},
+            "return": "rect",
+            "info": "Adds a new Rectangle to the card, and returns the new object."},
+        "add_round_rectangle": {
+            "args": {"...": {"type": "Any", "info": "optionally set more properties here.  For example: "
+                                                    "name=\"thingy\", position=(20,200), size=(100,50)"}},
+            "return": "roundrect",
+            "info": "Adds a new Round Rectangle to the card, and returns the new object."},
         "add_line": {"args": {"points": {"type": "list", "info": "a list of points, that are the locations of each "
-                                                                "vertex along the line, relative to the bottom-left "
-                                                                "corner of the card.  It can hold just two points "
-                                                                "to create a simple line segment, or more to create a "
-                                                                "more complex multi-segment line."},
-                             "name": {"type": "string", "info": "an optional argument giving the name to use for this "
-                                                                "new Line object.  If omitted, the name will be "
-                                                                "'shape_{N}'."},
-                             "...": {"type": "Any", "info": "optionally set more properties here.  For example, "
-                                                            "include position=(10,10)"}},
-                    "return": "line",
-                    "info": "Adds a new Line to the card, and returns the new object."},
+                                                                 "vertex along the line, relative to the bottom-left "
+                                                                 "corner of the card.  It can hold just two points "
+                                                                 "to create a simple line segment, or more to create a "
+                                                                 "more complex multi-segment line."},
+                              "...": {"type": "Any", "info": "optionally set more properties here.  For example: "
+                                                             "name=\"thingy\", position=(20,200), size=(100,50)"}},
+                     "return": "line",
+                     "info": "Adds a new Line to the card, and returns the new object."},
         "add_polygon": {"args": {"points": {"type": "list", "info": "a list of points, that are the locations of each "
-                                                                   "vertex along the outline of the polygon, relative "
-                                                                   "to the bottom-left corner of the card.  It must hold "
-                                                                   "three or more points to display properly as a "
-                                                                   "polygon."},
-                             "name": {"type": "string", "info": "an optional argument giving the name to use for this "
-                                                                "new Line object.  If omitted, the name will be "
-                                                                "'shape_{N}'."},
-                                "...": {"type": "Any", "info": "optionally set more properties here.  For example, "
-                                                               "include position=(10,10)"}},
-                       "return": "polygon",
-                    "info": "Adds a new Polygon shape to the card, and returns the new object."},
+                                                                    "vertex along the outline of the polygon, relative "
+                                                                    "to the bottom-left corner of the card.  It must hold "
+                                                                    "three or more points to display properly as a "
+                                                                    "polygon."},
+                                 "...": {"type": "Any", "info": "optionally set more properties here.  For example: "
+                                                                "name=\"thingy\", position=(20,200), size=(100,50)"}},
+                        "return": "polygon",
+                        "info": "Adds a new Polygon shape to the card, and returns the new object."},
         "add_group": {"args": {"objects": {"type": "list", "info": "a list of object, all on the same card, to include "
-                                                                  "in the new group object."},
-                             "name": {"type": "string", "info": "an optional argument giving the name to use for this "
-                                                                "new Group object.  If omitted, the name will be "
-                                                                "'group_{N}'."}
-                             },
-                    "return": "group",
-                    "info": "Adds a new Group to the card, and returns the new object."},
-        "animate_fill_color": {"args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
-                                      "end_color": {"type": "string",
-                                                   "info": "the final fill_color at the end of the animation"},
-                                      "on_finished": {"type": "function",
-                                                     "info": "an optional function to run when the animation finishes."}},
-                             "return": None,
-                             "info": "Visually animates this card's <b>fill_color</b> to <b>end_color</b>, "
-                                     "over <b>duration</b> seconds.  When the animation completes, runs the <b>on_finished</b> function, "
-                                     "if one was passed in."},
+                                                                   "in the new group object."},
+                               "...": {"type": "Any", "info": "optionally set more properties here.  For example: "
+                                                              "name=\"bundle\""}},
+                      "return": "group",
+                      "info": "Adds a new Group to the card, and returns the new object."},
+        "animate_fill_color": {
+            "args": {"duration": {"type": "float", "info": "time in seconds for the animation to run"},
+                     "end_color": {"type": "string",
+                                   "info": "the final fill_color at the end of the animation"},
+                     "easing": {"type": "string",
+                                "info": "an optional argument to allow controlling the animation's start and end accelerations. "
+                                        "Using \"In\" or \"InOut\" will ramp up the animation speed smoothly at the start, "
+                                        "instead of starting the animation at full speed. "
+                                        "Using \"Out\" or \"InOut\" will ramp down the animation speed smoothly at the end. "
+                                        "Setting easing to None or skipping this argument will use simple, linear animation, "
+                                        "which can look abrupt, but is sometimes what you want."},
+                     "on_finished": {"type": "function",
+                                     "info": "an optional function to run when the animation finishes."}},
+            "return": None,
+            "info": "Visually animates this card's <b>fill_color</b> to <b>end_color</b>, "
+                    "over <b>duration</b> seconds.  When the animation completes, runs the <b>on_finished</b> function, "
+                    "if one was passed in."},
         "stop_all_animating": {"args": {"property_name": {"type": "string",
-                                       "info": "optional name of the property to stop animating, for "
-                                               "example: \"size\" or \"position\".  If left blank, stops "
-                                              "animations of all properties of this card and its children."}},
-                              "return": None,
-                              "info": "Stops the animation specified by <b>property_name</b> from running on this card "
-                                      "and on all objects on this card, or if no <b>property_name</b> is specified, "
-                                      "stops all running animations on this card and on all objects on this card.  "
-                                      "Any animated properties are left at their current, mid-animation values."},
+                                                          "info": "optional name of the property to stop animating, for "
+                                                                  "example: \"size\" or \"position\".  If left blank, stops "
+                                                                  "animations of all properties of this card and its children."}},
+                               "return": None,
+                               "info": "Stops the animation specified by <b>property_name</b> from running on this card "
+                                       "and on all objects on this card, or if no <b>property_name</b> is specified, "
+                                       "stops all running animations on this card and on all objects on this card.  "
+                                       "Any animated properties are left at their current, mid-animation values."},
     }
 
     handlers = {
         "on_show_card": {"args": {},
-                       "info": "The <b>on_show_card</b> event is run any time a card is shown, including when the "
-                               "first card is initially shown when the stack starts running."},
+                         "info": "The <b>on_show_card</b> event is run any time a card is shown, including when the "
+                                 "first card is initially shown when the stack starts running."},
         "on_hide_card": {"args": {},
-                       "info": "The <b>on_hide_card</b> event is run when a card is hidden, right before the new "
-                               "card's on_show_card event is run, when going to another card."},
-        "on_exit_stack": {"args": {},
-                        "info": "The <b>on_exit_stack</b> event is run for all cards when the stack exits, whether "
-                                "from the File Close menu item, the quit() function, the stack.return_from_stack() method,"
-                                "or closing the stack viewer window.  You can use this to clean up any external "
-                                "resources -- for example, closing files.  This event needs to run quickly, so it's "
-                                "not able to call functions like alert(), ask_text(), ask_yes_no(), run_stack(), etc."},
-        "on_resize": {"args": {"is_initial": {"type": "bool", "info": "True if this event is running due to showing the "
-                                                                      "card.  False if this event is running due to the "
-                                                                      "card being resized."}},
-                     "info": "The <b>on_resize</b> event is run on the currently visible card when the stack window is "
-                             "resized.  It is also run each time a card is shown, to give the card a chance to set up "
-                             "its initial layout for the current size.  Your code can distinguish between these two "
-                             "cases by checking the value of <b>is_initial</b>."},
+                         "info": "The <b>on_hide_card</b> event is run when a card is hidden, right before the new "
+                                 "card's on_show_card event is run, when going to another card."},
+        "on_resize": {
+            "args": {"is_initial": {"type": "bool", "info": "True if this event is running due to showing the "
+                                                            "card.  False if this event is running due to the "
+                                                            "card being resized."}},
+            "info": "The <b>on_resize</b> event is run on the currently visible card when the stack window is "
+                    "resized.  It is also run each time a card is shown, to give the card a chance to set up "
+                    "its initial layout for the current size.  Your code can distinguish between these two "
+                    "cases by checking the value of <b>is_initial</b>."},
         "on_key_press": {"args": {"key_name": {"type": "string", "info": "The name of the pressed key"}},
-                      "info": "The <b>on_key_press</b> event is run any time a keyboard key is pressed down.  Regular "
-                              "keys are named as capital letters and digits, like 'A' or '1', and other keys have "
-                              "keyNames like 'Shift', 'Return', 'Escape', 'Left', and 'Right'."},
-        "on_key_hold": {"args": {"key_name": {"type": "string", "info": "The name of the key that is still being held down"},
-                               "elapsed_time": {"type": "float", "info": "This is the number of seconds since the key "
-                                                                        "press started, or since the last time this "
-                                                                        "event was run, normally about 0.03."}},
-                      "info": "The <b>on_key_hold</b> event is run repeatedly, while any keyboard key is pressed down.  "
-                              "Regular keys are named as capital letters and digits, like 'A' or '1', and other keys "
-                              "have keyNames like 'Shift', 'Return', 'Escape', 'Left', and 'Right'."},
+                         "info": "The <b>on_key_press</b> event is run any time a keyboard key is pressed down.  Regular "
+                                 "keys are named as capital letters and digits, like 'A' or '1', and other keys have "
+                                 "keyNames like 'Shift', 'Return', 'Escape', 'Left', and 'Right'."},
+        "on_key_hold": {
+            "args": {"key_name": {"type": "string", "info": "The name of the key that is still being held down"},
+                     "elapsed_time": {"type": "float", "info": "This is the number of seconds since the key "
+                                                               "press started, or since the last time this "
+                                                               "event was run, normally about 0.03."}},
+            "info": "The <b>on_key_hold</b> event is run repeatedly, while any keyboard key is pressed down.  "
+                    "Regular keys are named as capital letters and digits, like 'A' or '1', and other keys "
+                    "have keyNames like 'Shift', 'Return', 'Escape', 'Left', and 'Right'."},
         "on_key_release": {"args": {"key_name": {"type": "string", "info": "The name of the released key"}},
-                    "info": "The <b>on_key_release</b> event is run any time a pressed keyboard key is released.  Regular "
-                            "keys are named as capital letters and digits, like 'A' or '1', and other keys have "
-                            "keyNames like 'Shift', 'Return', 'Escape', 'Left', and 'Right'."},
+                           "info": "The <b>on_key_release</b> event is run any time a pressed keyboard key is released.  Regular "
+                                   "keys are named as capital letters and digits, like 'A' or '1', and other keys have "
+                                   "keyNames like 'Shift', 'Return', 'Escape', 'Left', and 'Right'."},
     }
 
 
 class HelpDataStack():
     parent = HelpDataObject
     types = ["stack"]
 
     properties = {
         "num_cards": {"type": "int",
-                     "info": "This is the number of cards in this stack.  You can "
-                             "read this value, but not set it."},
+                      "info": "This is the number of cards in this stack.  You can "
+                              "read this value, but not set it."},
         "current_card": {"type": "object",
-                        "info": "This is the card object that is currently visible.  stack.<b>current_card</b>.number will "
-                                "give you the number of the current card."},
+                         "info": "This is the card object that is currently visible.  stack.<b>current_card</b>.number will "
+                                 "give you the number of the current card."},
+        "can_save": {"type": "bool",
+                     "info": "If <b>can_save</b> is <b>True</b>, the user can save the stack while running it. "
+                             "If it's <b>False</b>, the user can't save, so the stack will always start out in the same "
+                             "state.  (Not currently supported on cardstock.run.)"},
+        "info": {"type": "string",
+                 "info": "You can enter info about your stack here, for example, instructions, explanation, a Change "
+                         "Log, License information, etc.  This <b>info</b> is accessible from your code, but not "
+                         "settable.  It's also viewable to anyone running this stack via the [Info] button when running "
+                         "on cardstock.run, or via the Stack Info menu item when running in the desktop app."},
+    }
+
+    properties_inspector_only = {
+        "author": {"type": "string",
+                   "info": "You can enter your name as the author here.  This property is not accessible from the stack's code."},
+        "username": {"type": "string",
+                     "info": "The username of the user who created this stack.  This property is not accessible from the stack's code."},
+        "stack_name": {"type": "string",
+                       "info": "The name of this stack.  This property is not accessible from the stack's code."},
+        "created": {"type": "string",
+                    "info": "The date and time that this stack was first saved.  This property is not accessible from the stack's code."},
+        "last_saved": {"type": "string",
+                       "info": "The date and time that this stack was most recently saved.  This property is not accessible from the stack's code."},
     }
 
     methods = {
+        "broadcast_message": {"args": {"message": {"type": "string",
+                                                   "info": "This is the message to send."}},
+                              "return": None,
+                              "info": "Sends the <b>message</b> to all objects on this card, or to all objects on all cards if called on the stack, causing each of the objects' "
+                                      "on_message events to run with this <b>message</b>."},
         "add_card": {"args": {"name": {"type": "string", "info": "an optional argument giving the name to use for this "
-                                                                "new card object.  If omitted, the name will be "
-                                                                "'card_{N}'."},
-                             "atNumber": {"type": "int", "info": "an optional argument giving the card number in "
-                                                                "the stack where the card should be added.  Number 1 is "
-                                                                "at the beginning.  If omitted, the card will be added "
-                                                                "at the end of the stack."},
-                             },
-                            "return": "card",
-                            "info": "Adds a new empty card to the stack, and returns the card object."},
+                                                                 "new card object.  If omitted, the name will be "
+                                                                 "'card_{N}'."},
+                              "atNumber": {"type": "int", "info": "an optional argument giving the card number in "
+                                                                  "the stack where the card should be added.  Number 1 is "
+                                                                  "at the beginning.  If omitted, the card will be added "
+                                                                  "at the end of the stack."},
+                              },
+                     "return": "card",
+                     "info": "Adds a new empty card to the stack, and returns the card object."},
+        "show_info": {"args": {},
+                      "return": None,
+                      "info": "Shows the stack's info property."},
         "card_with_number": {"args": {"number": {"type": "int",
-                                    "info": "the card number of the card to get."}},
-                           "return": "card",
-                           "info": "Returns the card at card <b>number</b>.  The first card is <b>number</b> 1."},
+                                                 "info": "the card number of the card to get."}},
+                             "return": "card",
+                             "info": "Returns the card at card <b>number</b>.  The first card is <b>number</b> 1."},
         "return_from_stack": {"args": {"returnValue": {"type": "any",
-                                            "info": "An optional value to pass back to the previous stack, that we are returning to."}},
+                                                       "info": "An optional value to pass back to the previous stack, that we are returning to."}},
+                              "return": None,
+                              "info": "If this stack was started from within another stack, by calling <b>run_stack()</b>, this "
+                                      "function will immediately stop the current event without returning, exit this stack, and return to the "
+                                      "previous stack. If you include a <b>returnValue</b>, this value will "
+                                      "be returned by the calling stack's <b>run_stack()</b> call, which will now finally return. "
+                                      "If the current stack was not started by a <b>run_stack()</b> call, this function does "
+                                      "nothing, and returns normally."},
+        "get_setup_value": {"args": {},
                             "return": None,
-                            "info": "If this stack was started from within another stack, by calling <b>run_stack()</b>, this "
-                                    "function will immediately stop the current event without returning, exit this stack, and return to the "
-                                    "previous stack. If you include a <b>returnValue</b>, this value will "
-                                    "be returned by the calling stack's <b>run_stack()</b> call, which will now finally return. "
-                                    "If the current stack was not started by a <b>run_stack()</b> call, this function does "
-                                    "nothing, and returns normally."},
-        "get_setup_value": {"args": {}, "return": None,
-                               "info": "If this stack was started by another stack calling run_stack() with a setupValue argument, "
-                                       "you can call this <b>get_setup_value()</b> method "
-                                       "to get the setupValue that was passed in from the calling stack.  Otherwise this "
-                                       "will return None."},
+                            "info": "If this stack was started by another stack calling run_stack() with a setupValue argument, "
+                                    "you can call this <b>get_setup_value()</b> method "
+                                    "to get the setupValue that was passed in from the calling stack.  Otherwise this "
+                                    "will return None."},
     }
 
-    handlers = {}
+    handlers = {
+        "on_exit_stack": {"args": {},
+                          "info": "The <b>on_exit_stack</b> event is run when the stack exits, whether "
+                                  "from the File Close menu item, the quit() function, the stack.return_from_stack() method, "
+                                  "or closing the running stack window.  You can use this to clean up any external "
+                                  "resources -- for example, closing files.  This event needs to run quickly, so it's "
+                                  "not able to call functions like alert(), ask_text(), ask_yes_no(), run_stack(), etc."},
+    }
 
 
 class HelpDataString():
-    """ Just method names and return types, for better autocomplete handling """
     parent = None
     types = ["string"]
     properties = {}
 
     methods = {
-        "capitalize": {"args": {},
-                    "return": "string",
-                    "info": ""},
-        "casefold": {"args": {},
-                       "return": "string",
-                       "info": ""},
-        "count": {"args": {},
-                       "return": "int",
-                       "info": ""},
-        "encode": {"args": {},
-                       "return": "string",
-                       "info": ""},
-        "endswith": {"args": {},
-                   "return": "bool",
-                   "info": ""},
-        "expandtabs": {"args": {},
-                   "return": "string",
-                   "info": ""},
-        "find": {"args": {},
-                   "return": "int",
-                   "info": ""},
-        "format": {"args": {},
-                   "return": "string",
-                   "info": ""},
-        "format_map": {"args": {},
-                   "return": "string",
-                   "info": ""},
-        "index": {"args": {},
-                   "return": "int",
-                   "info": ""},
-        "isalnum": {"args": {},
-                  "return": "bool",
-                  "info": ""},
-        "isalpha": {"args": {},
-                  "return": "bool",
-                  "info": ""},
-        "isascii": {"args": {},
-                  "return": "bool",
-                  "info": ""},
-        "isdecimat": {"args": {},
-                  "return": "bool",
-                  "info": ""},
-        "isidentifier": {"args": {},
-                  "return": "bool",
-                  "info": ""},
-        "islower": {"args": {},
-                    "return": "bool",
-                    "info": ""},
-        "isnumeric": {"args": {},
-                    "return": "bool",
-                    "info": ""},
-        "isprintable": {"args": {},
-                    "return": "bool",
-                    "info": ""},
-        "isspace": {"args": {},
-                    "return": "bool",
-                    "info": ""},
-        "istitle": {"args": {},
-                    "return": "bool",
-                    "info": ""},
-        "isupper": {"args": {},
-                    "return": "bool",
-                    "info": ""},
-        "join": {"args": {},
-                    "return": "string",
-                    "info": ""},
-        "ljust": {"args": {},
-                    "return": "string",
-                    "info": ""},
-        "lower": {"args": {},
-                  "return": "string",
-                  "info": ""},
-        "lstrip": {"args": {},
-                  "return": "string",
-                  "info": ""},
-        "maketrans": {"args": {},
-                  "return": "other",
-                  "info": ""},
-        "partition": {"args": {},
-                  "return": "other",
-                  "info": ""},
-        "replace": {"args": {},
-                  "return": "string",
-                  "info": ""},
-        "rfind": {"args": {},
-                  "return": "int",
-                  "info": ""},
-        "rindex": {"args": {},
-                  "return": "int",
-                  "info": ""},
-        "rjust": {"args": {},
-                  "return": "string",
-                  "info": ""},
-        "rpartition": {"args": {},
-                  "return": "other",
-                  "info": ""},
-        "rsplit": {"args": {},
-                  "return": "list",
-                  "info": ""},
-        "rstrip": {"args": {},
-                  "return": "string",
-                  "info": ""},
-        "split": {"args": {},
-                  "return": "list",
-                  "info": ""},
-        "splitlines": {"args": {},
-                  "return": "list",
-                  "info": ""},
-        "startswith": {"args": {},
-                  "return": "bool",
-                  "info": ""},
-        "strip": {"args": {},
-                       "return": "string",
-                       "info": ""},
-        "swapcase": {"args": {},
-                       "return": "string",
-                       "info": ""},
-        "title": {"args": {},
-                       "return": "string",
-                       "info": ""},
-        "translate": {"args": {},
-                       "return": "string",
-                       "info": ""},
-        "upper": {"args": {},
-                       "return": "string",
-                       "info": ""},
-        "zfill": {"args": {},
-                  "return": "string",
-                  "info": ""},
+        "capitalize": {
+            "args": {},
+            "return": "string",
+            "info": "Returns a copy of the original string with its first character converted to uppercase and all other characters converted to lowercase."
+        },
+        "casefold": {
+            "args": {},
+            "return": "string",
+            "info": "Returns a copy of the original string, normalized and in lower case. This method is more aggressive than <b>lower()</b> in terms of normalization."
+        },
+        "count": {
+            "args": {
+                "substring": {
+                    "type": "string",
+                    "info": "The substring to search for in the string."
+                },
+                "start": {
+                    "type": "int",
+                    "info": "The index at which to start counting (default is 0)."
+                },
+                "end": {
+                    "type": "int",
+                    "info": "The index at which to stop counting (default is the end of the string)."
+                }
+            },
+            "return": "int",
+            "info": "Returns the number of occurrences of <b>substring</b> in the string, optionally starting from <b>start</b> and ending at <b>end</b>."
+        },
+        "encode": {
+            "args": {
+                "encoding": {
+                    "type": "string",
+                    "info": "The character encoding to use for the resulting bytes object."
+                },
+                "errors": {
+                    "type": "string",
+                    "info": "How to handle errors that occur during encoding (e.g., 'strict', 'ignore', 'replace'). Default is 'strict'."
+                }
+            },
+            "return": "bytes",
+            "info": "Returns a bytes object representing the original string, encoded using <b>encoding</b> and handling errors according to <b>errors</b>."
+        },
+        "endswith": {
+            "args": {
+                "suffix": {
+                    "type": "string",
+                    "info": "The suffix to search for in the string."
+                },
+                "start": {
+                    "type": "int",
+                    "info": "The index at which to start searching (default is 0)."
+                },
+                "end": {
+                    "type": "int",
+                    "info": "The index at which to stop searching (default is the end of the string)."
+                }
+            },
+            "return": "bool",
+            "info": "Returns <b>True</b> if the string ends with <b>suffix</b>, starting from <b>start</b> and ending at <b>end</b>. Otherwise, returns <b>False</b>."
+        },
+        "expandtabs": {
+            "args": {
+                "tabsize": {
+                    "type": "int",
+                    "info": "The number of spaces to replace each tab character with. Default is 8."
+                }
+            },
+            "return": "string",
+            "info": "Returns a copy of the original string, replacing all tab characters with enough spaces to fill up <b>tabsize</b> columns."
+        },
+        "find": {
+            "args": {
+                "substring": {
+                    "type": "string",
+                    "info": "The substring to search for in the string."
+                },
+                "start": {
+                    "type": "int",
+                    "info": "The index at which to start searching (default is 0)."
+                },
+                "end": {
+                    "type": "int",
+                    "info": "The index at which to stop searching (default is the end of the string)."
+                }
+            },
+            "return": "int",
+            "info": "Returns the first index in the string where <b>substring</b> is found, starting from <b>start</b> and ending at <b>end</b>. Returns -1 if not found."
+        },
+        "format": {
+            "args": {
+                "format_spec": {
+                    "type": "string",
+                    "info": "A string containing format specification for the substitutions."
+                }
+            },
+            "return": "string",
+            "info": "Returns a copy of the original string with its placeholders replaced by their corresponding values, according to <b>format_spec</b>."
+        },
+
+        "index": {
+            "args": {
+                "sub": {
+                    "type": "string",
+                    "info": "The substring to search for."
+                },
+                "start": {
+                    "type": "int",
+                    "info": "The starting index of the search. Default is 0."
+                },
+                "end": {
+                    "type": "int",
+                    "info": "The ending index of the search. Default is the length of the string."
+                }
+            },
+            "return": "int",
+            "info": "Returns the index of the first occurrence of <b>sub</b> in the string, or -1 if not found.<br>" +
+                    "If <b>start</b> or <b>end</b> are specified, the search is limited to the indicated range."
+        },
+        "isalnum": {
+            "args": {},
+            "return": "bool",
+            "info": "Returns True if all characters in the string are alphanumeric (letters or digits), otherwise False.<br>" +
+                    "Spaces, punctuation, and other special characters will return False."
+        },
+        "isalpha": {
+            "args": {},
+            "return": "bool",
+            "info": "Returns True if all characters in the string are alphabetic (letters), otherwise False.<br>" +
+                    "Spaces, digits, punctuation, and other special characters will return False."
+        },
+        "isascii": {
+            "args": {},
+            "return": "bool",
+            "info": "Returns True if all characters in the string are ASCII-encoded, otherwise False.<br>" +
+                    "ASCII is a standard that defines the first 128 characters of the Unicode character set."
+        },
+        "isdecimal": {
+            "args": {},
+            "return": "bool",
+            "info": "Returns True if all characters in the string are decimal digits (0-9), otherwise False.<br>" +
+                    "This method is similar to <b>isdigit()</b>, but it checks for decimal digits only."
+        },
+        "isidentifier": {
+            "args": {},
+            "return": "bool",
+            "info": "Returns True if the string can be used as a valid Python identifier (variable name), otherwise False.<br>" +
+                    "Valid identifiers cannot start with a number or contain spaces, punctuation, or special characters."
+        },
+        "islower": {
+            "args": {},
+            "return": "bool",
+            "info": "Returns True if all characters in the string are lowercase letters, otherwise False.<br>" +
+                    "Spaces, digits, punctuation, and other special characters will return False."
+        },
+        "isnumeric": {
+            "args": {},
+            "return": "bool",
+            "info": "Returns True if all characters in the string are numeric (digits), otherwise False.<br>" +
+                    "This method is similar to <b>isdigit()</b>, but it checks for any numeric character, not just digits."
+        },
+        "isprintable": {
+            "args": {},
+            "return": "bool",
+            "info": "Returns True if all characters in the string can be printed (displayed), otherwise False.<br>" +
+                    "Spaces, punctuation, and other special characters will return True, but control characters will return False."
+        },
+        "format_map": {
+            "args": {
+                "mapping": {
+                    "type": "dictionary",
+                    "info": "A dictionary of replacement fields."
+                }
+            },
+            "return": "string",
+            "info": "Returns a copy of the string where each occurrence of a key in <b>mapping</b> is replaced with its corresponding value. Spaces are added between replacement fields if needed."
+        },
+        "isspace": {
+            "args": {},
+            "return": "bool",
+            "info": "Returns <b>True</b> if the string contains only whitespace characters, otherwise returns <b>False</b>."
+        },
+        "istitle": {
+            "args": {},
+            "return": "bool",
+            "info": "Returns <b>True</b> if each word in the string starts with a character that is uppercase and there are no other characters that are uppercase, otherwise returns <b>False</b>."
+        },
+        "isupper": {
+            "args": {},
+            "return": "bool",
+            "info": "Returns <b>True</b> if all the cased characters in the string are uppercase and there is at least one cased character, otherwise returns <b>False</b>."
+        },
+        "join": {
+            "args": {
+                "parts": {
+                    "type": "list",
+                    "info": "The list of parts to join into one string."
+                }
+            },
+            "return": "string",
+            "info": "Uses this string as the separator between each part of <b>parts</b>, and joins it all together into one string.  For example:<br/>"
+                    "\"::\".join(['1', '2', '3']) returns \"1::2::3\""
+        },
+        "ljust": {
+            "args": {
+                "width": {
+                    "type": "int",
+                    "info": "The total length of the result."
+                }
+            },
+            "return": "string",
+            "info": "Returns a left-justified string of length <b>width</b>. Padding is done using the specified fill character, which defaults to a space ' '."
+        },
+        "lower": {
+            "args": {},
+            "return": "string",
+            "info": "Returns a copy of the original string converted to all lowercase letters."
+        },
+        "lstrip": {
+            "args": {
+                "chars": {
+                    "type": "string",
+                    "info": "<b>chars</b>: The set of characters to remove. Defaults to removing whitespace."
+                }
+            },
+            "return": "string",
+            "info": "Returns a copy of the original string with leading characters removed from the <b>chars</b> argument. If no argument is given, it removes leading whitespace."
+        },
+        "maketrans": {
+            "args": {
+                "table1": {
+                    "type": "string",
+                    "info": "<b>table1</b>: The first table for the translation."
+                },
+                "table2": {
+                    "type": "string",
+                    "info": "<b>table2</b>: The second table for the translation."
+                }
+            },
+            "return": "dictionary",
+            "info": "Returns a translation table that can be used with <b>str.translate()</b>. You can define this table by specifying two strings of equal length, where each character in the first string maps to its corresponding character in the second string.<br><br>" +
+                    "For example, if you want to map 'a' to '4', 'e' to '3', and leave all other characters unchanged, then you can define <b>table1</b> as 'ae' and <b>table2</b> as '43'."
+        },
+        "partition": {
+            "args": {
+                "sep": {
+                    "type": "string",
+                    "info": "The separator character to use when partitioning the string."
+                }
+            },
+            "return": "tuple",
+            "info": "Returns a tuple containing three elements: the part before the separator, the separator itself, and the part after the separator. If the separator is not found, returns a tuple containing the original string and two empty strings."
+        },
+        "replace": {
+            "args": {
+                "old": {
+                    "type": "string",
+                    "info": "The string to search for."
+                },
+                "new": {
+                    "type": "string",
+                    "info": "The string to replace the old one with."
+                },
+                "count": {
+                    "type": "int",
+                    "info": "The maximum number of replacements to make. Default is unlimited."
+                }
+            },
+            "return": "string",
+            "info": "Returns a copy of the string with all occurrences of the old string replaced by the new one, up to the specified count. If count is not provided, all occurrences are replaced."
+        },
+        "rfind": {
+            "args": {
+                "sub": {
+                    "type": "string",
+                    "info": "The substring to search for."
+                },
+                "start": {
+                    "type": "int",
+                    "info": "The index at which to start the search. Default is -1, meaning the entire string is searched."
+                },
+                "end": {
+                    "type": "int",
+                    "info": "The index at which to stop the search. Default is -1, meaning the entire string is searched."
+                }
+            },
+            "return": "int",
+            "info": "Returns the index of the last occurrence of the substring in the string, or -1 if not found. The search starts from the right end of the string and stops at the specified end index (which can be negative to count from the end). If start is provided, the search starts from that index instead."
+        },
+        "rindex": {
+            "args": {
+                "sub": {
+                    "type": "string",
+                    "info": "The substring to search for."
+                },
+                "start": {
+                    "type": "int",
+                    "info": "The index at which to start the search. Default is -1, meaning the entire string is searched."
+                },
+                "end": {
+                    "type": "int",
+                    "info": "The index at which to stop the search. Default is -1, meaning the entire string is searched."
+                }
+            },
+            "return": "int",
+            "info": "Returns the index of the last occurrence of the substring in the string. Raises a ValueError if not found. The search starts from the right end of the string and stops at the specified end index (which can be negative to count from the end). If start is provided, the search starts from that index instead."
+        },
+        "rjust": {
+            "args": {
+                "width": {
+                    "type": "int",
+                    "info": "The total width of the result string."
+                },
+                "fillchar": {
+                    "type": "string",
+                    "info": "The character to use for padding. Default is a space."
+                }
+            },
+            "return": "string",
+            "info": "Returns a copy of the string right-justified to the specified width, using the fill character to pad on the left. If the string is already longer than the width, it is returned unchanged."
+        },
+        "rpartition": {
+            "args": {
+                "sep": {
+                    "type": "string",
+                    "info": "The separator character to use when partitioning the string."
+                }
+            },
+            "return": "tuple",
+            "info": "Returns a tuple containing three elements: the part before the separator, the separator itself, and the part after the separator. If the separator is not found, returns a tuple containing two empty strings and the original string."
+        },
+        "rstrip": {
+            "args": {
+                "chars": {
+                    "type": "string",
+                    "info": "A single character or a string of characters to be removed from the end of the string."
+                }
+            },
+            "return": "string",
+            "info": "Returns a copy of the original string with trailing whitespace and any specified <b>chars</b> removed. If no argument is given, only whitespace is removed."
+        },
+        "split": {
+            "args": {
+                "sep": {
+                    "type": "string",
+                    "info": "The delimiter separating the string into multiple substrings. Defaults to a space (' ')."
+                },
+                "maxsplit": {
+                    "type": "int",
+                    "info": "The maximum number of splits. Defaults to -1 (no limit)."
+                }
+            },
+            "return": "list",
+            "info": "Splits the string into a list of substrings at each occurrence of the <b>sep</b> delimiter. Returns up to <b>maxsplit</b> substrings, or all substrings if <b>maxsplit</b> is -1."
+        },
+        "splitlines": {
+            "args": {},
+            "return": "list",
+            "info": "Splits the string into a list of substrings at each newline character ('\n'). Equivalent to calling <b>str.split('\n')</b>, but preserves newlines as empty strings in the resulting list."
+        },
+        "startswith": {
+            "args": {
+                "prefix": {
+                    "type": "string",
+                    "info": "The string to check for at the beginning of this string."
+                }
+            },
+            "return": "bool",
+            "info": "Returns <b>True</b> if this string starts with the specified <b>prefix</b>, and <b>False</b> otherwise. Case-sensitive."
+        },
+        "strip": {
+            "args": {},
+            "return": "string",
+            "info": "Returns a copy of the original string with leading and trailing whitespace removed. Equivalent to calling both <b>lstrip()</b> and <b>rstrip()</b>."
+        },
+        "swapcase": {
+            "args": {},
+            "return": "string",
+            "info": "Converts all lowercase characters in the string to uppercase, and vice versa. For example, 'Hello World!' becomes 'hELLO wORLD!'."
+        },
+        "title": {
+            "args": {},
+            "return": "string",
+            "info": "Converts the first character of each word in the string to uppercase, and all other characters to lowercase. For example, 'hello world' becomes 'Hello World'."
+        },
+        "translate": {
+            "args": {
+                "table": {
+                    "type": "dictionary",
+                    "info": "A translation table mapping Unicode ordinals or characters (<b>int</b>/<b>str</b>) to replacement characters (also <b>str</b>)."
+                },
+                "deletechars": {
+                    "type": "string",
+                    "info": "An optional string of characters to be deleted from the input."
+                }
+            },
+            "return": "string",
+            "info": "Returns a copy of the original string with specified characters replaced or deleted. The <b>table</b> argument specifies which characters are replaced, and how. If the <b>deletechars</b> argument is given, any character in it will be removed from the input."
+        },
+        "upper": {
+            "args": {},
+            "return": "string",
+            "info": "Converts all lowercase characters in the string to uppercase. For example, 'hello world' becomes 'HELLO WORLD'."
+        },
+        "zfill": {
+            "args": {
+                "width": {
+                    "type": "int",
+                    "info": "Minimum width of the resulting string."
+                }
+            },
+            "return": "string",
+            "info": "Returns a copy of the original string left filled with <b>ascii</b> '0' digits until the given <b>width</b> is reached. If <b>width</b> is less than the length of the string, it returns the original string."
+        }
     }
 
 
 class HelpDataList():
-    """ Just method names and return types, for better autocomplete handling """
     parent = None
     types = ["list"]
     properties = {}
 
     methods = {
-        "append": {"args": {},
-                    "return": None,
-                    "info": ""},
+        "append": {
+            "args": {
+                "element": {
+                    "type": "object",
+                    "info": "The element to add to the end of the list."
+                }
+            },
+            "return": None,
+            "info": "Adds <b>element</b> to the end of the list."
+        },
+        "clear": {
+            "args": {},
+            "return": None,
+            "info": "Removes all elements from the list."
+        },
+        "copy": {
+            "args": {},
+            "return": "list",
+            "info": "Returns a shallow copy of the list."
+        },
+        "count": {
+            "args": {
+                "element": {
+                    "type": "any",
+                    "info": "The element to search for in the list."
+                }
+            },
+            "return": "int",
+            "info": "Returns the number of <b>element</b> occurrences in the list."
+        },
+        "extend": {
+            "args": {
+                "iterable": {
+                    "type": "any",
+                    "info": "An iterable object to add elements from to the end of the list."
+                }
+            },
+            "return": None,
+            "info": "Adds elements from <b>iterable</b> to the end of the list."
+        },
+        "index": {
+            "args": {
+                "element": {
+                    "type": "any",
+                    "info": "The element to search for in the list."
+                }
+            },
+            "return": "int",
+            "info": "Returns the index of the first occurrence of <b>element</b> in the list, or -1 if not found."
+        },
+        "insert": {
+            "args": {
+                "index": {
+                    "type": "int",
+                    "info": "The index at which to insert <b>element</b>."
+                },
+                "element": {
+                    "type": "any",
+                    "info": "The element to insert into the list."
+                }
+            },
+            "return": None,
+            "info": "Inserts <b>element</b> at position <b>index</b> in the list."
+        },
+        "pop": {
+            "args": {
+                "index": {
+                    "type": "int",
+                    "info": "The index of the element to remove and return (default -1, which removes and returns the last element)."
+                }
+            },
+            "return": "any",
+            "info": "Removes and returns the element at position <b>index</b> in the list.  If no index is specified, removes and returns the last element."
+        },
+        "remove": {
+            "args": {
+                "element": {
+                    "type": "any",
+                    "info": "The element to remove from the list."
+                }
+            },
+            "return": None,
+            "info": "Removes the first occurrence of <b>element</b> from the list."
+        },
+        "reverse": {
+            "args": {},
+            "return": None,
+            "info": "Reverses the order of elements in the list."
+        },
+        "sort": {
+            "args": {
+                "key": {
+                    "type": "callable",
+                    "info": "A function to customize sorting (default None, which uses the standard comparison operation)."
+                },
+                "reverse": {
+                    "type": "bool",
+                    "info": "Whether to sort in descending order (default False, which sorts in ascending order)."
+                }
+            },
+            "return": None,
+            "info": "Sorts the elements of the list in place."
+        }
+    }
+
+
+class HelpDataTuple():
+    parent = None
+    types = ["tuple"]
+    properties = {}
+
+    methods = {
+        "count": {
+            "args": {
+                "element": {
+                    "type": "any",
+                    "info": "The element to search for in the list."
+                }
+            },
+            "return": "int",
+            "info": "Returns the number of <b>element</b> occurrences in the list."
+        },
+        "index": {
+            "args": {
+                "element": {
+                    "type": "any",
+                    "info": "The element to search for in the list."
+                }
+            },
+            "return": "int",
+            "info": "Returns the index of the first occurrence of <b>element</b> in the list, or -1 if not found."
+        }
+    }
+
+
+class HelpDataDict():
+    parent = None
+    types = ["dictionary"]
+    properties = {}
+
+    methods = {
         "clear": {"args": {},
-                   "return": None,
-                   "info": ""},
+                  "return": None,
+                  "info": "<b>Clear</b> removes all items from the dictionary.  This method does not return any value."},
         "copy": {"args": {},
+                 "return": "dictionary",
+                 "info": "Returns a <b>copy</b> of the dictionary, leaving the original unchanged.  This is useful if you want to create a temporary copy without affecting the original data."},
+        "get": {"args": {"key": {"type": "str or anyhashable", "info": "<b>Key</b> to retrieve from the dictionary."}},
+                "return": "any",
+                "info": "Retrieves the value associated with <b>key</b> in the dictionary.  If the key does not exist, it returns None."},
+        "items": {"args": {},
+                  "return": "list",
+                  "info": "Returns a list of tuples containing all key-value pairs from the dictionary."},
+        "keys": {"args": {},
+                 "return": "list",
+                 "info": "Returns a list of all keys in the dictionary."},
+        "pop": {"args": {"key": {"type": "any", "info": "<b>Key</b> to remove from the dictionary."}},
+                "return": "any",
+                "info": "Removes and returns the value associated with <b>key</b> in the dictionary.  If the key does not exist, it raises a KeyError."},
+        "popitem": {"args": {},
+                    "return": "tuple",
+                    "info": "Removes and returns an arbitrary item from the dictionary.  This method raises a KeyError if the dictionary is empty."},
+        "setdefault": {"args": {"key": {"type": "any", "info": "<b>Key</b> to set default value for."},
+                                "default": {"type": "any", "info": "Default value to use if key does not exist."}},
+                       "return": "any",
+                       "info": "Sets the value associated with <b>key</b> in the dictionary to the specified default value.  If the key already exists, it returns the original value."},
+        "update": {
+            "args": {"other_dict": {"type": "dictionary", "info": "The other dictionary to update from."}},
+            "return": None,
+            "info": "Updates the dictionary with all key-value pairs from <b>other_dict</b>."},
+        "values": {"args": {},
                    "return": "list",
-                   "info": ""},
-        "count": {"args": {},
-                   "return": "int",
-                   "info": ""},
-        "extend": {"args": {},
-                   "return": None,
-                   "info": ""},
-        "index": {"args": {},
-                   "return": "int",
-                   "info": ""},
-        "insert": {"args": {},
-                   "return": None,
-                   "info": ""},
-        "pop": {"args": {},
-                   "return": "any",
-                   "info": ""},
-        "remove": {"args": {},
-                   "return": None,
-                   "info": ""},
-        "reverse": {"args": {},
-                   "return": None,
-                   "info": ""},
-        "sort": {"args": {},
-                   "return": None,
-                   "info": ""},
+                   "info": "Returns a list of all values in the dictionary."}
     }
 
 
 class HelpDataBuiltins():
-    """ Just function names and return types, for better autocomplete handling """
     parent = None
     types = []
     properties = {}
 
     functions = {
-        "abs": {"args": {},
-                    "return": "int",
-                    "info": ""},
-        "str": {"args": {},
-                   "return": "string",
-                   "info": ""},
-        "bool": {"args": {},
-                   "return": "bool",
-                   "info": ""},
-        "list": {"args": {},
-                   "return": "list",
-                   "info": ""},
-        "int": {"args": {},
-                   "return": "int",
-                   "info": ""},
-        "float": {"args": {},
-                   "return": "float",
-                   "info": ""},
-        "dict": {"args": {},
-                   "return": "dict",
-                   "info": ""},
-        "tuple": {"args": {},
-                   "return": "other",
-                   "info": ""},
-        "len": {"args": {},
-                   "return": "int",
-                   "info": ""},
-        "min": {"args": {},
-                   "return": "int",
-                   "info": ""},
-        "max": {"args": {},
-                   "return": "int",
-                   "info": ""},
-        "print": {"args": {},
-                "return": None,
-                "info": ""},
-        "range": {"args": {},
-                "return": "other",
-                "info": ""},
-        "sorted": {"args": {},
-                "return": "list",
-                "info": ""},
-        "filter": {"args": {},
-                "return": "other",
-                "info": ""},
-        "format": {"args": {},
-                "return": "string",
-                "info": ""},
-        "hex": {"args": {},
+        "abs": {"args": {}, "return": "float",
+                "info": "<b>abs</b> returns the absolute value of a number."},
+
+        "str": {"args": {"object": {"type": "any", "info": "The object to convert to a string."}},
                 "return": "string",
-                "info": ""},
-        "oct": {"args": {},
+                "info": "<b>str</b> converts an object into a human-readable string.  This is often used for outputting text or combining strings together."},
+
+        "bool": {"args": {"value": {"type": "any", "info": "The value to convert to a boolean."}},
+                 "return": "bool",
+                 "info": "<b>bool</b> converts an object into a boolean value (True or False).  This is often used for conditional statements and logical operations."},
+
+        "list": {"args": {"elements": {"type": "any", "info": "The elements to include in the list."}},
+                 "return": "list",
+                 "info": "<b>list</b> creates a new, ordered collection of objects that can be accessed by their index.  You can add or remove items from the list as needed."},
+
+        "int": {"args": {"value": {"type": "any", "info": "The value to convert into an integer."}},
+                "return": "int",
+                "info": "<b>int</b> converts an object into a whole number (integer).  This is often used for counting, indexing, and numerical calculations."},
+
+        "float": {"args": {"value": {"type": "any", "info": "The value to convert into a floating-point number."}},
+                  "return": "float",
+                  "info": "<b>float</b> converts an object into a decimal number (floating-point).  This is often used for mathematical calculations and precise measurements."},
+
+        "dict": {
+            "args": {"key-value pairs": {"type": "any", "info": "The key-value pairs to include in the dictionary."}},
+            "return": "dictionary",
+            "info": "<b>dict</b> creates a new, unordered collection of objects that are accessed by their keys.  You can add or remove items from the dictionary as needed."},
+
+        "tuple": {"args": {"elements": {"type": "any", "info": "The elements to include in the tuple."}},
+                  "return": "tuple",
+                  "info": "<b>tuple</b> creates a new, ordered collection of objects that cannot be changed once created.  You can use tuples for collections where you want to keep the same items but not modify them."},
+
+        "len": {"args": {"collection": {"type": "list|str|dict|set", "info": "The collection to get the length of."}},
+                "return": "int",
+                "info": "<b>len</b> returns the number of items in a given collection (such as a list, string, dictionary, or set)."},
+
+        "min": {
+            "args": {"collection": {"type": "list|tuple|str", "info": "The collection to find the minimum value from."},
+                     "key": {"type": "function",
+                             "info": "An optional function to apply to each element before comparing."}},
+            "return": "any",
+            "info": "<b>min</b> returns the smallest item in a given collection (such as a list, tuple, or string).  You can also specify a key function to determine which value is considered 'smallest'."},
+
+        "max": {
+            "args": {"collection": {"type": "list|tuple|str", "info": "The collection to find the maximum value from."},
+                     "key": {"type": "function",
+                             "info": "An optional function to apply to each element before comparing."}},
+            "return": "any",
+            "info": "<b>max</b> returns the largest item in a given collection (such as a list, tuple, or string).  You can also specify a key function to determine which value is considered 'largest'."},
+
+        "print": {"args": {"objects, ...": {"type": "any", "info": "The objects to print to the console."}},
+                  "return": None,
+                  "info": "<b>print</b> outputs one or more objects to the console, followed by a newline character.  This is often used for debugging and displaying output to the user."},
+
+        "input": {"args": {
+            "prompt": {"type": "string", "info": "Text to print to the console before waiting for user input."}},
+            "return": "string",
+            "info": "Wait for the user to type text into the console.  When the user types the Return/Enter key, this function returns the string that the user typed."},
+
+        "range": {
+            "args": {"start": {"type": "int", "info": "The starting value of the range (optional, default=0)"},
+                     "stop": {"type": "int", "info": "The ending value of the range (exclusive)"}},
+            "return": "tuple",
+            "info": "<b>range</b> creates an iterator that produces a sequence of numbers from <b>start</b> up to, but not including, <b>stop</b>.  This is often used for iterating over a range of values in a loop."},
+
+        "sorted": {"args": {"collection": {"type": "list|tuple|str", "info": "The collection to sort."},
+                            "key": {"type": "function",
+                                    "info": "An optional function to apply to each element before comparing."}},
+                   "return": "list",
+                   "info": "<b>sorted</b> returns a new, sorted copy of the given collection (such as a list, tuple, or string).  You can also specify a key function to determine how the items should be ordered."},
+
+        "filter": {
+            "args": {"function": {"type": "function", "info": "The function to apply to each item in the collection"},
+                     "collection": {"type": "list|tuple", "info": "The collection to filter."}},
+            "return": "tuple",
+            "info": "<b>filter</b> creates an iterator that produces a sequence of items from the given collection, where each item passes a specified test (function).  This is often used for selecting specific items from a collection."},
+
+        "format": {"args": {"string": {"type": "string", "info": "The string to format."},
+                            "*values": {"type": "any", "info": "The values to insert into the string"}},
+                   "return": "string",
+                   "info": "<b>format</b> replaces placeholders in a string with provided values, allowing you to create formatted output.  This is often used for displaying data in a human-readable format."},
+
+        "hex": {"args": {"number": {"type": "int|float", "info": "The number to convert to hexadecimal."}},
                 "return": "string",
-                "info": ""},
-        "map": {"args": {},
-                "return": "other",
-                "info": ""},
-        "ord": {"args": {},
+                "info": "<b>hex</b> converts an integer or floating-point number into its hexadecimal representation as a string."},
+
+        "oct": {"args": {"number": {"type": "int|float", "info": "The number to convert to octal."}},
                 "return": "string",
-                "info": ""},
-        "open": {"args": {},
-                "return": "other",
-                "info": ""},
-        "pow": {"args": {},
+                "info": "<b>oct</b> converts an integer or floating-point number into its octal representation as a string."},
+
+        "map": {
+            "args": {"function": {"type": "function", "info": "The function to apply to each item in the collection"},
+                     "collection": {"type": "list|tuple", "info": "The collection to map."}},
+            "return": "tuple",
+            "info": "<b>map</b> creates an iterator that produces a sequence of items from the given collection, where each item has been processed by a specified function.  This is often used for transforming or processing data in bulk."},
+
+        "ord": {"args": {"character": {"type": "string", "info": "The character to convert to its ASCII value."}},
                 "return": "int",
-                "info": ""},
-        "reversed": {"args": {},
-                "return": "other",
-                "info": ""},
-        "round": {"args": {},
+                "info": "<b>ord</b> returns the ASCII value of a single character as an integer.  This is often used for converting characters into numerical codes."},
+
+        "open": {"args": {"file_name": {"type": "string", "info": "The name of the file to open"},
+                          "mode": {"type": "string",
+                                   "info": "The mode in which to open the file (e.g., 'r' for read-only, 'w' for write-only)"}},
+                 "return": "file",
+                 "info": "<b>open</b> opens a file and returns a file object that allows you to read from or write to the file.  This is often used for reading or writing files in your program."},
+
+        "pow": {"args": {"base": {"type": "float", "info": "The base number"},
+                         "exponent": {"type": "float", "info": "The exponent to raise the base to"}},
                 "return": "float",
-                "info": ""},
-        "sum": {"args": {},
+                "info": "<b>pow</b> returns the result of raising a given base number to an exponent.  This is often used for calculating powers and exponents."},
+
+        "reversed": {"args": {"collection": {"type": "list|tuple", "info": "The collection to reverse."}},
+                     "return": "tuple",
+                     "info": "<b>reversed</b> creates an iterator that produces the elements of a given collection in reverse order.  This is often used for processing or iterating over data in reverse."},
+
+        "round": {"args": {"number": {"type": "float", "info": "The number to round"},
+                           "ndigits": {"type": "int",
+                                       "info": "The number of digits after the decimal point to round to (optional, default=0)"}},
+                  "return": "float",
+                  "info": "<b>round</b> rounds a floating-point number to the nearest integer or to a specified precision.  This is often used for converting decimal values into whole numbers."},
+
+        "sum": {"args": {"collection": {"type": "list|tuple", "info": "The collection to sum up"}},
                 "return": "float",
-                "info": ""},
-        "zip": {"args": {},
-                "return": "other",
-                "info": ""},
-    }
+                "info": "<b>sum</b> returns the total sum of all items in a given collection (such as a list, tuple, or string).  This is often used for calculating totals and aggregations."},
 
+        "zip": {"args": {"*collections": {"type": "list|tuple", "info": "The collections to combine"}},
+                "return": "tuple",
+                "info": "<b>zip</b> creates an iterator that produces tuples containing one item from each of the given collections.  This is often used for combining data from multiple sources into a single collection."}
+    }
 
-helpClasses = [HelpDataObject, HelpDataCard, HelpDataStack, HelpDataButton, HelpDataTextLabel, HelpDataTextField,
-               HelpDataWebView, HelpDataImage, HelpDataGroup, HelpDataLine, HelpDataShape, HelpDataRoundRectangle,
-               HelpDataString, HelpDataList]
+    methods = functions
```

### Comparing `cardstock-0.99.5/cardstock/helpDialogs.py` & `cardstock-0.99.6/cardstock/helpDialogs.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
 # of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import wx
 import wx.html
 import version
 import platform
-from helpData import HelpData, HelpDataTypes
+from helpDataGen import HelpData, HelpDataTypes
 
 OUTPUT_HTML = False
 
 
 class CardStockAbout(wx.Dialog):
     """ An about box that uses an HTML view. """
 
@@ -95,40 +95,40 @@
 as one piece, and that group becomes a new object itself.</p>
 
 <br/><br/>
 
 <h2>Designer Layout</h2>
 <p>The CardStock Designer application is where you design, build, draw, and code your CardStock programs.  The Designer
 window is split into two main parts.  On the left is your stack, that shows the currently selected card and its objects.
-On the right
-is the control panel.  The top of the control panel lets you choose an editing tool.</p>
-<p>The first is the hand tool, which
+On the right is the control panel.  Along the top are controls that let you move between cards, test-run your stack, 
+and choose an editing tool.</p>
+<p>The first tool is the selection/hand tool, which
 lets you select, move, rotate, and resize objects, and edit their properties and code.  Select an object by clicking it, and add 
 or remove objects from the selection by Shift-clicking them.  You can also drag out a selection rectangle to select all objects
 whose centers it contains.  You can also cycle forwards and backwards through objects on the current card using Tab and
 Shift-Tab.  While objects are selected, you can use the Object menu items to group them, flip them, align or distribute 
 them, or re-order them to adjust which
 objects are in front of, or behind, which others.  But note that currently, Text Fields and Web Views are always displayed in 
 front of other objects.  When an object is selected, you can resize it by dragging the rectangular, blue resize knobs in the 
 corners of the selected object.  Holding down the Shift key while resizing will keep the object's aspect
 ratio stable.  You can drag selected objects to move them, or use the arrow keys to move selected objects by 1 pixel at
 a time, or by 5 or 20 pixels at a time by holding down Shift or Alt/Option, respectively.  You can also rotate an object 
 by dragging the round, blue rotation knob at the top of the selected object, and can constrain rotation to multiples of
 5 degrees by holding down the Shift key.</p>
-<p>The next five tools are the button, text field, web view, image, and text label tools.  These each 
-let you create that type of object, by drawing out the new object's shape on the card on the left.  You can double-click
-a text field or text label to edit its text in-place on the card.  Note that you can set a Button object's style, to 
-make it it appear and behave as either a regular button with a Border, a Borderless button, a Checkbox, or a Radio button.  
+<p>The next five tools are the button, text field, web view, image, and text label tools.  (Note that web-views are not 
+currently supported on cardstock.run.)  These tools each let you create that type of object, by drawing out the new 
+object's shape on the card on the left.  You can also double-click a text field or text label to edit its text in-place 
+on the card.  Note that you can set a Button object's style, to make it it appear and behave as either a regular button 
+with a Border, a Borderless button, a Checkbox, or a Radio button.
 </p>
-<p>The next six tools
-are the drawing tools, which let you draw with a pen, drag out an oval, a rectangle, a rounded rectangle, a polygon, 
-or a line.
-While creating a shape, you can hold down the Shift key to constrain ovals and rectangles to being circles and squares, 
-and to make new lines stay perfectly horizontal, vertical, or 45° diagonal. After creating an object, CardStock will 
-switch back to the Hand tool.  Pressing Escape in the Designer will also always return you to the Hand tool.</p>
+<p>The next six tools are the drawing tools, which let you draw with a pen, drag out an oval, a rectangle, a 
+rounded rectangle, a polygon, or a line.  While creating a shape, you can hold down the Shift key to constrain ovals 
+and rectangles to being circles and squares, and to make new lines stay perfectly horizontal, vertical, or 45° 
+diagonal. After creating an object, CardStock will switch back to the Hand tool.  Pressing Escape in the Designer will 
+also always return you to the Hand tool.</p>
  
 <p>Additionally there are keyboard shortcuts for selecting all of the tools.  Those shortcuts are shown when the mouse 
 is over that tool's button in the control panel.  They are:<br/>
 <ul>
 <li>H (or Escape) for <b>H</b>and
 <li>B for <b>B</b>utton
 <li>F for Text <b>F</b>ield
@@ -139,36 +139,33 @@
 <li>O for <b>O</b>val
 <li>R for <b>R</b>ectangle
 <li>D for Roun<b>D</b> Rectangle
 <li>G for Poly<b>G</b>on
 <li>L for <b>L</b>ine
 </ul>
 </p>
-<p>The area in the control panel below the tools changes depending on which tool you're using, and which objects are 
-selected in the card.  When a drawing tool is selected, the control panel offers you settings to choose the pen color,
-pen thickness, and fill color for the shapes you draw next.  Then click and drag out the shape you want to add to the 
-card.</p>
-<p>When you select a single object 
+<p>To the right of your card editor is the control panel.  When you select a single object 
 in your card, the control panel will show the two main object editing areas:  The property editor shows, and lets you edit, a
 list of the selected object's properties, like name, size, position on the card, colors, etc.  Below the property editor is 
 the code editor.  The code editor lets you view and edit the code that runs when events are triggered for this object.
 For example, if you select a button object,
 you could edit the code for its <b>on_click</b> event, which runs when that button is clicked.  In between the two editors is 
-the Context Help box.  This shows information about the most recently selected property or event, or the last 
+the Context Help box.  (On cardstock.run, this is actually located on the bottom left of the page.)  This shows 
+information about the most recently selected property or event, or the last 
 autocompleted term in the code editor.  You can resize the Context Help box by dragging the bottom-right, blue corner,
 and can hide it using the command in CardStock's Help Menu if you already know the info it's telling you, you want the
 space back, or its incessant helpfulness otherwise offends your sensibilities.</p>
 
 <br/><br/>
 
 <h2>Property Editor</h2>
 <p>Each object in your stack, including each card, button, text field, shape, group, etc., has properties that
 you can change in the property editor when that object is selected. You can change things like the object's
 position and size. And each type of object also has its own specific properties.  For example, a card has a <b>fill_color</b>, 
-and a button has a <b>title</b>.  Each object also has a name, which is how you control it from your python code. 
+and a button has a <b>text</b> property.  Each object also has a name, which is how you control it from your python code. 
 CardStock makes sure that these names are unique within each card. See the CardStock Reference for a description of each
 property, for each type of object.</p>
 
 <br/><br/>
 
 <h2>Code Editor</h2>
 <p>The real fun begins when you start adding python code into your objects!  Your CardStock program works by running
@@ -178,15 +175,15 @@
 "on_click()".  Then add your code into the button's on_click event in the code editor, and now when you run your 
 stack, whenever that button is clicked, this code will run.  The "+ Add Event" popup shows all of the events that apply to the
 selected object.  For example, only buttons have an on_click() event, and only cards have an on_show_card() event.
 See the CardStock Reference for a description of each type of event, and when they each get run.</p>
 
 <p>In your python event-handling code, you have access to all of the objects in your stack, including their
 properties and methods, and some global variables and functions that are always available.  So if your button is called 
-yes_button, you could write <b>yes_button.title = "Done"</b> to change your button's title to the string "Done".  You can 
+yes_button, you could write <b>yes_button.text = "Done"</b> to change your button's text to the string "Done".  You can 
 also use the variables that are passed into each event function, which are listed inside the parentheses after the event
 name.  All events receive a variable called self, which refers to the object who's event is being run.  
 So in a button's on_click(self) code, self refers to that button object.  In a card's on_show_card(self) code, self will 
 refer to that card object.  Some events also receive other relevant information, for example, on_key_press(self, key_name)
 includes key_name, so that your code can see which key was pressed, and on_mouse_move(self, mouse_pos) includes the current 
 mouse position as a variable called mouse_pos.  See the CardStock Reference for a list of all 
 variables that are automatically provided to your code.  You can of course also create your own variables as well.  It 
@@ -198,16 +195,16 @@
 Then the first card's on_show_card() event will run.  Any time you go to another card, the current card's on_hide_card() 
 event will run, immediately followed by the new card's on_show_card() event.  After your stack is done starting up, all 
 of the current card's objects (including the card itself) will start running their on_periodic() events, approximately every 
 1/30th of a second.  This is a 
 great place to run any periodic checks that need to keep happening often.  The on_resize() event runs on a card object 
 when the stack window is resized while that card is shown, to give your stack a chance to re-layout objects based on 
 the new card size.  The on_message() event runs on an object when any of your other code calls that object's 
-object.send_message() method, or calls the broadcast_message() function, which sends the message to all objects in the 
-stack.</p>
+object.send_message() method, or calls the broadcast_message() method on this object's card, or on the stack, which sends the 
+message to all objects on the card or the whole stack, respectively.</p>
 
 <p>The on_key_press() and on_key_release() events of the current card run when a keyboard key is pressed down, and released, 
 respectively.  And on_key_hold() is called approximately every 1/30th of a second for each key that remains held pressed 
 down.</p>
 
 <p>The on_mouse_enter() and on_mouse_exit() events for an object are run when the mouse enters and exits screen space that 
 overlaps that object.  The on_mouse_press() and on_mouse_release() events of an object are run when the main mouse button is 
@@ -274,16 +271,16 @@
 then add a line like <b>self.speed.y -= 30</b> into the object's on_periodic() event.</p>
 
 <br/><br/>
 
 <h2>Web Views</h2>
 
 <p>CardStock also allows you to embed web pages into your stacks, using Web View objects.  But note that currently 
-WebViews only work when your stack is run as a program on your computer, and not when uploaded and run through the
-cardstock.run site.  You can set the URL property
+Web Views only work when your stack is run as a program on your computer, and not on the cardstock.run website.  
+You can set the URL property
 of a Web View, and it will load the web page at that URL.  Or you can set the HTML property of a Web View, and it will 
 display that HTML.  You can restrict a Web View to only allow loading pages from a specific set of hosts, by setting its allowed_hosts
 property.  For example, if you only want to allow loading pages from my-fun-game.com, then you can set webview_1.URL to
 https://my-fun-game.com/starting-page.html, and set webview_1.allowed_hosts to ['my-fun-game.com'].  This way it will 
 not allow users to navigate off of the my-fun-game.com site.</p>
 
 <p>When a page loads, either because you set the Web View's URL, or because the user clicked a link to navigate to 
@@ -310,24 +307,24 @@
 
 <p>CardStock also offers a Variable inspector window while your stack is running.  You can open it using the 
 "Show/Hide Variables" menu item.  This window shows you a list of all variables in use by your stack, and allows you to open 
 object and list variables hierarchically to see their items and properties, by clicking the right-arrow button on a row.  
 For example, you could click the right arrow on the "card" row to see your current card's properties, and then on the 
 "children" row to see all objects on that card.  Then on a button's row to see all the properties of that button.  For 
 rows representing numbers, strings, boolean values, etc., you can click on the row's value to edit it live, while your 
-stack is running.</p>
+stack is running.  (This feature is not currently available on cardstock.run.)</p>
 
 <p>If any errors occur while running your stack, error messages will be written to the console window, and then after 
 you return to the Designer, they will be listed in the red-colored Error List window that will
 appear.  You can also open this window from the Help menu.  Clicking on an error in this list will take you to the 
 offending line in the code editor for that event.</p>
 
 <p>If you want to look at all of your code at once, instead of only at one object's code at a time,
 you can open the All Code window from the Help menu.  Clicking a line in the All Code editor will take you to that
-line of that object's event code in the code editor.</p>
+line of that object's event code in the code editor.  (This feature is not currently available on cardstock.run.)</p>
 
 <p>Note that CardStock has a full Find and Replace system, that lets you find, and optionally replace, strings in your
 code and properties throughout your whole stack.  It allows finding using python style regular expression syntax, if you
 want to use that to search for more complex expressions.</p>
 
 <br/><br/>
 
@@ -432,21 +429,21 @@
                                          "its own code for handling events.  The below properties, methods, and "
                                          "events, in addition to those in the All Objects section, apply to card "
                                          "objects.  Access an object's properties or methods as, for example, "
                                          "object_name.size or object_name.show().  You can also access a child object "
                                          "of this card as card.object_name.")}
 <hr/>
 {HelpData.ObjectSection("button", "Button", "Buttons in CardStock come in 4 styles.  <b>Border</b> style buttons "
-                                            "show their title centered inside of a rounded rectangle border, and when clicked, "
+                                            "show their <b>text</b> centered inside of a rounded rectangle border, and when clicked, "
                                             "run their on_click() event code.  <b>Borderless</b> buttons behave the same, but "
                                             "are transparent and do not display a border.  A <b>Checkbox</b> button shows its "
-                                            "title left-justified, after a checkbox that shows a check when it is selected. "
+                                            "text left-justified, after a checkbox that shows a check when it is selected. "
                                             "When a user clicks a Checkbox, its selection state toggles between selected and not,"
                                             "and the object's on_selection_changed() event is run.  A <b>Radio</b> button shows its "
-                                            "title left-justified, after an indicator circle, that shows a dot inside when it is selected. "
+                                            "text left-justified, after an indicator circle, that shows a dot inside when it is selected. "
                                             "When a user clicks a Radio button, it is selected, and any other Radio "
                                             "buttons in the same Radio group are deselected, "
                                             "and both objects' on_selection_changed() events is run, first the deselection, "
                                             "and then the selection.  All Radio buttons directly on the card are in one Radio group. "
                                             "All Radio buttons that have been grouped together into the same Group object are in their own "
                                             "Radio group. "
                                             "The below properties, methods, and events, in addition to those "
```

### Comparing `cardstock-0.99.5/cardstock/imageFactory.py` & `cardstock-0.99.6/cardstock/imageFactory.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/mediaSearchDialogs.py` & `cardstock-0.99.6/cardstock/mediaSearchDialogs.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/migrations.py` & `cardstock-0.99.6/cardstock/migrations.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,31 @@
                 dataDict['properties']["style"] = ("Border" if dataDict['properties'].pop("has_border") else "Borderless")
             if 'childModels' in dataDict:
                 for child in dataDict['childModels']:
                     replaceNames(child)
         for c in dataDict['cards']:
             replaceNames(c)
 
+    if fromVer <= 8:
+        """
+        In File Format Version 9, button.title changed to button.text
+        """
+        def replaceNames(d):
+            if "title" in d['properties']:
+                d['properties']["text"] = d['properties'].pop("title")
+            if 'childModels' in d:
+                for child in d['childModels']:
+                    replaceNames(child)
+        for c in dataDict['cards']:
+            c['properties']['size'] = dataDict['properties']['size']
+            c['properties']['can_resize'] = dataDict['properties']['can_resize']
+            replaceNames(c)
+        dataDict['properties'].pop('size')
+        dataDict['properties'].pop('can_resize')
+
 
 def MigrateModelFromFormatVersion(fromVer, stackModel):
     # Migration code to run after loading the json into models
 
     if fromVer <= 1:
         """
         In File Format Version 1, the cards used the top-left corner as the origin, y increased while moving down.
@@ -365,7 +382,24 @@
                     val = v
                     val = val.replace(".get_event_code(", ".get_code_for_event(")
                     val = val.replace(".set_event_code(", ".set_code_for_event(")
                     obj.handlers[k] = val
             for child in obj.childModels:
                 replaceNames(child)
         replaceNames(stackModel)
+
+    if fromVer <= 8:
+        """
+        In File Format Version 9, broadcast_message() changed from a global func to a method on stacks and cards
+        """
+        def replaceNames(obj):
+            for k ,v in obj.handlers.items():
+                if len(v):
+                    val = v
+                    val = re.sub(r"\bbroadcast_message\(", "card.broadcast_message(", val)
+                    val = re.sub(r"\bColorRGB\(", "color_rgb(", val)
+                    val = re.sub(r"\bColorHSB\(", "color_hsb(", val)
+                    val = re.sub(r"\.title\b", ".text", val)
+                    obj.handlers[k] = val
+            for child in obj.childModels:
+                replaceNames(child)
+        replaceNames(stackModel)
```

### Comparing `cardstock-0.99.5/cardstock/propertyInspector.py` & `cardstock-0.99.6/cardstock/propertyInspector.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,18 @@
             if not self.IsCellEditControlShown():
                 if not self.IsReadOnly(self.GetGridCursorRow(), 1):
                     if self.GetGridCursorCol() == 0:
                         self.SetGridCursor(self.GetGridCursorRow(), 1)
                     self.EnableCellEditControl(True)
             else:
                 ed = self.GetCellEditor(self.GetGridCursorRow(), 1)
-                if isinstance(ed, GridCellCustomChoiceEditor):
+                if isinstance(ed, wx.grid.GridCellAutoWrapStringEditor):
+                    event.EventObject.WriteText('\n')
+                    return
+                elif isinstance(ed, GridCellCustomChoiceEditor):
                     ed.GetControl().DoClose(True)
                 else:
                     self.DisableCellEditControl()
                 ed.DecRef()
                 event.StopPropagation()
                 return
         elif event.GetKeyCode() in (wx.WXK_UP, wx.WXK_DOWN) and self.IsCellEditControlShown():
@@ -170,18 +173,22 @@
                 editor = GridCellCustomChoiceEditor(ViewModel.GetPropertyChoices(k))
             elif valType == "color":
                 editor = GridCellColorEditor(self)
                 renderer = GridCellColorRenderer()
             elif valType == "file":
                 editor = GridCellImageFileEditor(self, self.stackManager.runner is None)
                 renderer = GridCellImageFileRenderer(self.stackManager.runner is None)
-            elif valType in ("obj", "list", "static_list", "dict", "set"):
-                editable = (valType not in ("obj", "static_list"))
+            elif valType in ("obj", "list", "static_list", "dict", "set", "static"):
+                editable = (valType not in ("obj", "static_list", "static"))
                 editor = GridCellObjectEditor(self, editable)
                 renderer = GridCellObjectRenderer()
+            elif valType == "text":
+                editor = wx.grid.GridCellAutoWrapStringEditor()
+                renderer = wx.grid.GridCellAutoWrapStringRenderer()
+                self.SetRowSize(r, 200)
             if renderer:
                 self.SetCellRenderer(r, 1, renderer)
             if editor:
                 self.SetCellEditor(r, 1, editor)
             r += 1
 
         if len(keys) >= oldRow:
```

### Comparing `cardstock-0.99.5/cardstock/pythonEditor.py` & `cardstock-0.99.6/cardstock/pythonEditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
 # of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import wx
 import wx.stc as stc
 import keyword
-import helpData
+import helpDataGen
 
 """
 The PythonEditor is used for the CodeEditor in the Designer's ControlPanel.
 It offers syntax highlighting, brace pairing, and simple code autocompletion.
 """
 
 TAB_WIDTH = 3
@@ -164,15 +164,15 @@
             wordEndPos = self.WordEndPosition(currentPos, True)
             lineNum = self.LineFromPosition(currentPos)
             lineStartPos = self.GetLineEndPosition(lineNum) - self.GetLineLength(lineNum)
             leadingStr = self.GetRange(lineStartPos, wordEndPos)
             (parentType, name, objType, obj) = self.analyzer.GetTypeFromLeadingString(self.currentModel, leadingStr)
             if self.GetRange(wordEndPos, wordEndPos+1) == "(":
                 name += "()"
-            helpText = helpData.HelpData.GetHelpForName(name, parentType)
+            helpText = helpDataGen.HelpData.GetHelpForName(name, parentType)
             if helpText:
                 self.cPanel.UpdateHelpText(helpText)
         event.Skip()
 
     def PyEditorOnZoom(self, event):
         # Disable Zoom
         z = event.GetEventObject().GetZoom()
@@ -296,15 +296,15 @@
 
     def OnACSelectionChange(self, event):
         if not self.cPanel:
             return
 
         s = event.GetString()
         if s:
-            helpText = helpData.HelpData.GetHelpForName(s, "any")
+            helpText = helpDataGen.HelpData.GetHelpForName(s, "any")
             if helpText:
                 self.cPanel.UpdateHelpText(helpText)
                 return
         self.cPanel.UpdateHelpText("")
         event.Skip()
 
     def IsInCommentOrString(self):
```

### Comparing `cardstock-0.99.5/cardstock/resourcePathManager.py` & `cardstock-0.99.6/cardstock/resourcePathManager.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/runner.py` & `cardstock-0.99.6/cardstock/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,48 +94,47 @@
         # 0-item list means just wake up to check if the thread is supposed to stop
         self.handlerQueue = queue.Queue()
 
         self.runnerThread = CodeRunnerThread(target=self.StartRunLoop)
         self.runnerThread.start()
         self.stopRunnerThread = False
         self.generatingThumbnail = False
+        self.compileCache = {}
 
         self.soundCache = {}
 
         self.stackStartTime = time()
 
         self.initialClientVars = {
             "wait": self.wait,
             "run_after_delay": self.run_after_delay,
             "time": self.time,
             "distance": self.distance,
             "angle_from_points": self.angle_from_points,
             "rotate_point": self.rotate_point,
-            "paste": self.paste,
             "alert": self.alert,
             "ask_yes_no": self.ask_yes_no,
             "ask_text": self.ask_text,
             "input": self.input,
             "goto_card": self.goto_card,
             "goto_next_card": self.goto_next_card,
             "goto_previous_card": self.goto_previous_card,
             "run_stack": self.run_stack,
             "open_url": self.open_url,
             "request_url": self.request_url,
             "play_sound": self.play_sound,
             "stop_sound": self.stop_sound,
-            "broadcast_message": self.broadcast_message,
             "is_key_pressed": self.is_key_pressed,
             "is_mouse_pressed": self.is_mouse_pressed,
             "is_using_touch_screen": self.is_using_touch_screen,
             "get_mouse_pos": self.get_mouse_pos,
             "clear_focus": self.clear_focus,
             "quit":self.quit,
-            "ColorRGB": self.MakeColorRGB,
-            "ColorHSB": self.MakeColorHSB,
+            "color_rgb": self.color_rgb,
+            "color_hsb": self.color_hsb,
             "Point": self.MakePoint,
             "Size": self.MakeSize,
         }
 
         self.clientVars = self.initialClientVars.copy()
 
         self.keyCodeStringMap = {
@@ -205,29 +204,32 @@
 
     def IsRunningHandler(self):
         return len(self.lastHandlerStack) > 0
 
     def EnableUpdateVars(self, enable):
         self.shouldUpdateVars = enable
 
+    def HandlerChanged(self, model, handlerName):
+        path = model.GetPath() + "." + handlerName
+        if path in self.compileCache:
+            del self.compileCache[path]
+
     def StopTimers(self):
         for t in self.timers:
             t.Stop()
         self.timers = []
 
     def DoReturnFromStack(self, stackReturnVal):
         self.stackReturnQueue.put(stackReturnVal)
 
     def CleanupFromRun(self):
         # On Main thread
         if self.runnerThread:
             self.stopRunnerThread = True
             self.StopTimers()
-            for card in self.stackManager.stackModel.childModels:
-                self.RunHandler(card, "on_exit_stack", None)
             self.stackReturnQueue.put(None)  # Stop waiting for a run_stack() call to return
             self.handlerQueue.put((TaskType.Wake, )) # Wake up the runner thread get() call so it can see that we're stopping
 
             def waitAndYield(duration):
                 # wait up to duration seconds for the stack to finish running
                 # run wx.YieldIfNeeded() to process main thread events while waiting, to allow @RunOnMainSync* methods to complete
                 if self.generatingThumbnail: return
@@ -511,41 +513,53 @@
                 oldVars["edge"] = self.clientVars["edge"]
             else:
                 oldVars["edge"] = noValue
             self.clientVars["edge"] = arg[1]
 
         # rewrite handlers that use return outside of a function, and replace with an exception that we catch, to
         # act like a return.
-        handlerStr = self.RewriteHandler(handlerStr)
+        path = uiModel.GetPath() + "." + handlerName
 
         self.lastHandlerStack.append((uiModel, handlerName))
 
         error = None
         error_class = None
         line_number = None
         errModel = None
         errHandlerName = None
         in_func = []
         detail = None
 
-        # Use this for noticing user-definitions of new functions
-        oldClientVars = self.clientVars.copy()
-
         try:
-            exec(handlerStr, self.clientVars)
-            self.ScrapeNewFuncDefs(oldClientVars, self.clientVars, uiModel, handlerName)
+            isNew = False
+            if path in self.compileCache:
+                ast = self.compileCache[path]
+            else:
+                handlerStr = self.RewriteHandler(handlerStr)
+                ast = compile(handlerStr, "<string>", "exec")
+                self.compileCache[path] = ast
+                isNew = True
+            # Use this for noticing user-definitions of new functions
+            if isNew:
+                oldClientVars = self.clientVars.copy()
+
+            exec(ast, self.clientVars)
+            if isNew:
+                self.ScrapeNewFuncDefs(oldClientVars, self.clientVars, uiModel, handlerName)
         except SyntaxError as err:
-            self.ScrapeNewFuncDefs(oldClientVars, self.clientVars, uiModel, handlerName)
+            if isNew:
+                self.ScrapeNewFuncDefs(oldClientVars, self.clientVars, uiModel, handlerName)
             detail = err.msg
             error_class = err.__class__.__name__
             line_number = err.lineno
             errModel = uiModel
             errHandlerName = handlerName
         except Exception as err:
-            self.ScrapeNewFuncDefs(oldClientVars, self.clientVars, uiModel, handlerName)
+            if isNew:
+                self.ScrapeNewFuncDefs(oldClientVars, self.clientVars, uiModel, handlerName)
             if err.__class__.__name__ == "RuntimeError" and err.args[0] == "Return":
                 # Catch our exception-based return calls
                 pass
             else:
                 error_class = err.__class__.__name__
                 detail = err.args[0]
                 cl, exc, tb = sys.exc_info()
@@ -731,15 +745,15 @@
         # Keep track of where each user function has been defined, so we can send you to the right handler's code in
         # the Designer when the user clicks on an error in the ErrorList.
         for (k, v) in newVars.items():
             if isinstance(v, types.FunctionType) and (k not in oldVars or oldVars[k] != v):
                 self.funcDefs[k] = (model, handlerName)
 
     def HandlerPath(self, model, handlerName, card=None):
-        if model.type == "card":
+        if model.type in ["card", "stack"]:
             return f"{model.GetProperty('name')}.{handlerName}()"
         else:
             if card is None:
                 card = model.GetCard()
             return f"{model.GetProperty('name')}.{handlerName}() on card '{card.GetProperty('name')}'"
 
     def KeyNameForEvent(self, event):
@@ -812,23 +826,14 @@
                     uiView.view.SetSelection(sel[0], sel[1])
         else:
             self.stackManager.uiCard.view.SetFocus()
 
 
     # --------- User-accessible view functions -----------
 
-    def broadcast_message(self, message):
-        if not isinstance(message, str):
-            raise TypeError("broadcast_message(): message must be a string")
-
-        self.RunHandler(self.stackManager.uiCard.model, "on_message", None, message)
-        for ui in self.stackManager.uiCard.GetAllUiViews():
-            if not ui.model.didDelete:
-                self.RunHandler(ui.model, "on_message", None, message)
-
     def goto_card(self, card):
         index = None
         if isinstance(card, str):
             cardName = card
         elif isinstance(card, Card):
             cardName = card._model.GetProperty("name")
         elif isinstance(card, int):
@@ -870,14 +875,15 @@
                 raise RuntimeError("Return")
         else:
             raise RuntimeError(f"run_stack(): Couldn't find stack '{filename}'.")
 
     def return_from_stack(self, result=None):
         if not self.viewer:
             return
+        self.RunHandler(self.stackManager.stackModel, "on_exit_stack", None)
         stackReturnValue = sanitizer.SanitizeValue(result, [])
         if self.viewer.GosubStack(None,-1, stackReturnValue):
             raise RuntimeError('Return')
 
     def GetStackSetupValue(self):
         return self.stackSetupValue
 
@@ -1060,21 +1066,14 @@
 
         if s:
             s.play()
 
     def stop_sound(self):
         simpleaudio.stop_all()
 
-    @RunOnMainSync
-    def paste(self):
-        models = self.stackManager.Paste(False)
-        for model in models:
-            model.RunSetup(self)
-        return [m.GetProxy() for m in models]
-
     def is_key_pressed(self, name):
         if not isinstance(name, str):
             raise TypeError("is_key_pressed(): name must be a string")
 
         return name in self.pressedKeys
 
     @RunOnMainSync
@@ -1088,32 +1087,32 @@
     def get_mouse_pos(self):
         return wx.RealPoint(*self.stackManager.view.ScreenToClient(*wx.GetMousePosition()))
 
     def clear_focus(self):
         self.SetFocus(None)
 
     @staticmethod
-    def MakeColorRGB(red, green, blue):
+    def color_rgb(red, green, blue):
         if not isinstance(red, (float, int)) or not 0 <= red <= 1:
-            raise TypeError("ColorRGB(): red must be a number between 0 and 1")
+            raise TypeError("color_rgb(): red must be a number between 0 and 1")
         if not isinstance(green, (float, int)) or not 0 <= green <= 1:
-            raise TypeError("ColorRGB(): green must be a number between 0 and 1")
+            raise TypeError("color_rgb(): green must be a number between 0 and 1")
         if not isinstance(blue, (float, int)) or not 0 <= blue <= 1:
-            raise TypeError("ColorRGB(): blue must be a number between 0 and 1")
+            raise TypeError("color_rgb(): blue must be a number between 0 and 1")
         red, green, blue = (int(red * 255), int(green * 255), int(blue * 255))
         return f"#{red:02X}{green:02X}{blue:02X}"
 
     @staticmethod
-    def MakeColorHSB(hue, saturation, brightness):
+    def color_hsb(hue, saturation, brightness):
         if not isinstance(hue, (float, int)) or not 0 <= hue <= 1:
-            raise TypeError("ColorHSB(): hue must be a number between 0 and 1")
+            raise TypeError("color_hsb(): hue must be a number between 0 and 1")
         if not isinstance(saturation, (float, int)) or not 0 <= saturation <= 1:
-            raise TypeError("ColorHSB(): saturation must be a number between 0 and 1")
+            raise TypeError("color_hsb(): saturation must be a number between 0 and 1")
         if not isinstance(brightness, (float, int)) or not 0 <= brightness <= 1:
-            raise TypeError("ColorHSB(): brightness must be a number between 0 and 1")
+            raise TypeError("color_hsb(): brightness must be a number between 0 and 1")
         red, green, blue = colorsys.hsv_to_rgb(hue, saturation, brightness)
         red, green, blue = (int(red * 255), int(green * 255), int(blue * 255))
         return f"#{red:02X}{green:02X}{blue:02X}"
 
     @staticmethod
     def MakePoint(x, y):
         if not isinstance(x, (float, int)):
@@ -1126,15 +1125,15 @@
     def MakeSize(width, height):
         if not isinstance(width, (float, int)):
             raise TypeError("Size(): width must be a number")
         if not isinstance(height, (float, int)):
             raise TypeError("Size(): height must be a number")
         return wx.Size(width, height)
 
-    def run_after_delay(self, duration, func, *args, **kwargs):
+    def run_after_delay(self, duration, func):
         try:
             duration = float(duration)
         except ValueError:
             raise TypeError("run_after_delay(): duration must be a number")
 
         startTime = time()
 
@@ -1143,20 +1142,20 @@
             if self.stopRunnerThread or self.generatingThumbnail: return
 
             adjustedDuration = duration + startTime - time()
             if adjustedDuration > 0.010:
                 timer = wx.Timer()
                 def onTimer(event):
                     if self.stopRunnerThread: return
-                    self.EnqueueFunction(func, *args, **kwargs)
+                    self.EnqueueFunction(func)
                 timer.Bind(wx.EVT_TIMER, onTimer)
                 timer.StartOnce(int(adjustedDuration*1000))
                 self.timers.append(timer)
             else:
-                self.EnqueueFunction(func, *args, **kwargs)
+                self.EnqueueFunction(func)
 
         f()
 
     @RunOnMainAsync
     def quit(self):
         if self.stopRunnerThread or self.stackManager.isEditing: return
         self.stackManager.view.TopLevelParent.OnMenuClose(None)
```

### Comparing `cardstock-0.99.5/cardstock/sanitizer.py` & `cardstock-0.99.6/cardstock/sanitizer.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/simpleListBox.py` & `cardstock-0.99.6/cardstock/simpleListBox.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/stackExporter.py` & `cardstock-0.99.6/cardstock/stackExporter.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/stackManager.py` & `cardstock-0.99.6/cardstock/stackManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from tools import *
 from appCommands import *
 import generator
 import findEngineDesigner
 import resourcePathManager
 import analyzer
 from stackModel import StackModel
-from uiCard import UiCard, CardModel
+from uiCard import UiCard, UiView, CardModel
 from uiButton import UiButton
 from uiTextField import UiTextField
 from uiTextLabel import UiTextLabel
 from uiImage import UiImage, ImageModel
 from uiWebView import UiWebView
 from uiShape import UiShape
 from uiGroup import UiGroup, GroupModel
@@ -118,14 +118,15 @@
         self.selectedViews = []
         self.modelToViewMap = {}
         self.cardIndex = None
 
         # This is the only UiCard in the designer or viewer.  It gets re-set-up with each card model, one at a time.
         self.uiCard = None
         self.uiCard = UiCard(None, self, self.stackModel.childModels[0])
+        self.uiStack = UiView(None, self, self.stackModel, None)
 
         self.uiCard.model.SetDirty(False)
         self.command_processor.ClearCommands()
 
         if wx.Platform != '__WXMAC__':
             # Skip double-buffering on Mac, as it's much faster without it, and looks great
             self.buffer = None
@@ -280,18 +281,19 @@
         if model == self.stackModel:
             return
         self.ClearAllViews()
         if not skipSetDown:
             self.stackModel.SetDown()
         model.SetStackManager(self)
         self.stackModel = model
+        self.uiStack = UiView(None, self, self.stackModel, None)
         self.cardIndex = None
         if self.isEditing:
             wx.CallAfter(self.analyzer.RunAnalysis)
-            self.uiCard.ResizeCardView(self.stackModel.GetProperty("size"))
+            self.uiCard.ResizeCardView(self.uiCard.model.GetProperty("size"))
         if not skipSetDown:
             self.command_processor.ClearCommands()
             self.stackModel.SetDirty(False)
         self.UpdateCursor()
 
     @RunOnMainSync
     def LoadCardAtIndex(self, index, reload=False):
@@ -313,16 +315,18 @@
                 if self.designer:
                     self.designer.UpdateCardList()
                 if self.runner:
                     self.runner.SetupForCard(cardModel)
                     if not self.isEditing and not reload:
                         if self.uiCard.model.GetHandler("on_show_card"):
                             self.runner.RunHandler(self.uiCard.model, "on_show_card", None)
-                        if self.stackModel.GetProperty("can_resize"):
+                        if self.uiCard.model.GetProperty("can_resize"):
                             self.runner.RunHandler(self.uiCard.model, "on_resize", None, True)
+                if self.designer:
+                    self.designer.SetFrameSizeFromModel()
                 self.view.Refresh()
             if self.designer:
                 self.designer.Thaw()
 
     def SetDesigner(self, designer):
         self.designer = designer
 
@@ -664,14 +668,19 @@
         self.AddUiViewsFromModels([im], True)
 
     def GetSelectedUiViews(self):
         return self.selectedViews.copy()
 
     def SelectUiView(self, uiView, extend=False):
         if self.isEditing:
+            selectStack = False
+            if uiView == self.uiStack:
+                selectStack = True
+                uiView = None
+
             if extend and uiView and uiView.parent and uiView.parent.model.type == "group":
                 extend = False
             if extend and len(self.selectedViews) and self.selectedViews[0].parent and self.selectedViews[0].parent.model.type == "group":
                 extend = False
             if extend and uiView and ((uiView.model.type == "card") != (len(self.selectedViews) and self.selectedViews[0].model.type == "card")):
                 extend = False
             if len(self.selectedViews) and not extend:
@@ -684,33 +693,36 @@
                     self.selectedViews.remove(uiView)
                 else:
                     uiView.SetSelected(True)
                     self.selectedViews.append(uiView)
             if self.designer:
                 self.designer.SetSelectedUiViews(self.selectedViews)
 
+            if selectStack:
+                self.designer.cPanel.UpdateForUiViews([self.uiStack])
+
     @RunOnMainAsync
     def OnPropertyChanged(self, model, key):
         uiView = self.GetUiViewByModel(model)
-        if model == self.stackModel:
-            uiView = self.uiCard
-            if key == "size":
-                s = model.GetProperty(key)
-                if self.designer:
-                    self.uiCard.ResizeCardView(s)
-                else:
-                    self.view.GetTopLevelParent().SetClientSize(self.view.FromDIP(s))
+        if model.type == "card" and key == "size":
+            s = model.GetProperty(key)
+            if self.designer:
+                self.uiCard.ResizeCardView(s)
+            else:
+                self.view.GetTopLevelParent().SetClientSize(self.view.FromDIP(s))
         if uiView:
             uiView.OnPropertyChanged(model, key)
         if uiView and self.designer:
             self.designer.cPanel.UpdatedProperty(uiView, key)
 
     def GetUiViewByModel(self, model):
         if not self.uiCard:
             return None
+        if model == self.stackModel:
+            return self.uiStack
         if model == self.uiCard.model:
             return self.uiCard
         if model in self.modelToViewMap:
             return self.modelToViewMap[model]
         return None
 
     def GetUiViewByName(self, name):
@@ -789,14 +801,16 @@
             command = ReorderCardCommand(True, "Reorder Card", self, self.cardIndex, newIndex)
             self.command_processor.Submit(command)
 
     def AddCard(self):
         newCard = CardModel(self)
         newCard.SetProperty("name", newCard.DeduplicateName("card_1",
                                                             [m.GetProperty("name") for m in self.stackModel.childModels]))
+        newCard.SetProperty("size", self.uiCard.model.GetProperty("size"))
+        newCard.SetProperty("can_resize", self.uiCard.model.GetProperty("can_resize"))
         command = AddNewUiViewCommand(True, "Add Card", self, self.cardIndex+1, "card", newCard)
         self.command_processor.Submit(command)
 
     def DuplicateCard(self, card=None):
         newCard = CardModel(self)
         if not card:
             card = self.stackModel.childModels[self.cardIndex]
@@ -842,33 +856,39 @@
                 # Flag this is a double-click  On mouseUp, we'll start the inline editor.
                 self.isDoubleClick = True
             if self.tool.name != "polygon" or wx.Platform == "__WXGTK__":
                 return
 
         pos = self.view.ScreenToClient(event.GetEventObject().ClientToScreen(event.GetPosition()))
         if self.isEditing:
-            uiView = self.HitTest(pos, not event.ShiftDown())
-            uiViews = [uiView] if uiView else None
+            if uiView == self.uiCard and (pos.y < 0 or pos.x > self.uiCard.model.GetProperty("size").width):
+                # Don't select card when a click starts outside of the card.
+                self.SelectUiView(None)
+                uiViews = []
+            else:
+                uiView = self.HitTest(pos, not event.ShiftDown())
+                uiViews = [uiView] if uiView else None
         else:
             uiViews = self.HitTestAll(pos)
 
         if self.inlineEditingView:
             if uiViews and uiViews[0] == self.inlineEditingView:
                 # Let the inline editor handle clicks while it's enabled
                 event.Skip()
                 return
             else:
                 self.inlineEditingView.StopInlineEditing()
 
-        if self.tool and self.isEditing:
+        if self.isEditing:
             if uiViews and uiViews[0].model.type.startswith("text") and event.LeftDClick():
                 # Flag this is a double-click  On mouseUp, we'll start the inline editor.
                 self.isDoubleClick = True
             else:
-                self.tool.OnMouseDown(uiViews[0], event)
+                # We need to pass in a view, even when click starts outside the card
+                self.tool.OnMouseDown(uiViews[0] if uiViews else self.uiCard, event)
         else:
             self.lastMouseDownView = uiViews[0]
             self.runner.ResetStopHandlingMouseEvent()
             for uiView in uiViews:
                 uiView.OnMouseDown(event)
             event.Skip()
 
@@ -1163,14 +1183,18 @@
                 self.varUpdateTimer.StartOnce(int(ms))
 
     def OnUpdateVarsTimer(self, event=None):
         if self.runner and not self.isEditing:
             self.runner.viewer.UpdateVars()
         self.lastVarUpdateTime = time()
 
+    def ShowStackInfo(self):
+        if self.runner and self.runner.viewer:
+            self.runner.viewer.OnMenuInfo()
+
     def GetDesignerFindPath(self):
         cPanel = self.designer.cPanel
         cardModel = self.uiCard.model
         cardIndex = self.stackModel.childModels.index(cardModel)
         uiView = None
         if len(cPanel.lastSelectedUiViews) == 1:
             uiView = cPanel.lastSelectedUiViews[0]
```

### Comparing `cardstock-0.99.5/cardstock/stackModel.py` & `cardstock-0.99.6/cardstock/stackModel.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,68 +7,84 @@
 # of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import wx
 from uiView import ViewModel, ViewProxy
 from uiCard import CardModel
 import version
 import migrations
-from codeRunnerThread import RunOnMainSync
+from codeRunnerThread import RunOnMainSync, RunOnMainAsync
+
 
 class StackModel(ViewModel):
     """
     This is the model for the stack.  It mostly just contains the cards as its children.
     """
 
     minSize = wx.Size(200, 200)
 
     def __init__(self, stackManager):
         super().__init__(stackManager)
         self.type = "stack"
         self.proxyClass = Stack
 
-        self.properties["size"] = wx.Size(500, 500)
         self.properties["name"] = "stack"
         self.properties["can_save"] = False
-        self.properties["can_resize"] = False
+        self.properties["author"] = ""
+        self.properties["info"] = ""
 
+        self.propertyTypes["stack_name"] = 'static'
         self.propertyTypes["can_save"] = 'bool'
-        self.propertyTypes["can_resize"] = 'bool'
+        self.propertyTypes["author"] = 'string'
+        self.propertyTypes["info"] = 'text'
+
+        self.propertyKeys = ["stack_name", "author", "can_save", "info"]
 
-        self.propertyKeys = []
+        self.handlers = {"on_setup": "", "on_exit_stack": ""}
+        self.initialEditHandler = "on_setup"
 
-        self.handlers = {}
+    def GetProperty(self, key):
+        if key == "stack_name":
+            if self.stackManager.designer and self.stackManager.designer.filename:
+                return self.stackManager.designer.filename
+            return ""
+        else:
+            return super().GetProperty(key)
 
     def AppendCardModel(self, cardModel):
         cardModel.parent = self
         self.childModels.append(cardModel)
 
     def InsertCardModel(self, index, cardModel):
         cardModel.parent = self
         self.childModels.insert(index, cardModel)
 
     def InsertNewCard(self, name, atIndex):
-        card = CardModel(self.stackManager)
-        card.SetProperty("name", self.DeduplicateName(name, [m.GetProperty("name") for m in self.childModels]))
+        newCard = CardModel(self.stackManager)
+        newCard.SetProperty("name", self.DeduplicateName(name, [m.GetProperty("name") for m in self.childModels]))
+        newCard.SetProperty("size", self.stackManager.uiCard.model.GetProperty("size"))
+        newCard.SetProperty("can_resize", self.stackManager.uiCard.model.GetProperty("can_resize"))
         if atIndex == -1:
-            self.AppendCardModel(card)
+            self.AppendCardModel(newCard)
         else:
-            self.InsertCardModel(atIndex, card)
+            self.InsertCardModel(atIndex, newCard)
             newIndex = self.childModels.index(self.stackManager.uiCard.model)
             self.stackManager.cardIndex = newIndex
-        return card
+        return newCard
 
     def RemoveCardModel(self, cardModel):
         cardModel.parent = None
         self.childModels.remove(cardModel)
 
     def GetCardModel(self, i):
         return self.childModels[i]
 
     def GetModelFromPath(self, path):
         parts = path.split('.')
+        if len(parts) and parts[0] == "":
+            return self
         m = self
         for p in parts:
             found = False
             for c in m.childModels:
                 if c.properties['name'] == p:
                     m = c
                     found = True
@@ -77,14 +93,15 @@
                 return None
         return m
 
     def GetData(self):
         data = super().GetData()
         data["cards"] = [m.GetData() for m in self.childModels]
         data["properties"].pop("position")
+        data["properties"].pop("size")
         data["properties"].pop("name")
         data["CardStock_stack_format"] = version.FILE_FORMAT_VERSION
         data["CardStock_stack_version"] = version.VERSION
         return data
 
     def SetData(self, stackData):
         formatVer = stackData["CardStock_stack_format"]
@@ -105,14 +122,18 @@
 
 class Stack(ViewProxy):
     @property
     def num_cards(self):
         return len(self._model.childModels)
 
     @property
+    def info(self):
+        return self._model.GetProperty("info")
+
+    @property
     def current_card(self):
         if self._model.didSetDown: return None
         return self._model.stackManager.uiCard.model.GetProxy()
 
     def card_with_number(self, number):
         model = self._model
         if model.didSetDown: return None
@@ -124,14 +145,26 @@
 
     def return_from_stack(self, result=None):
         self._model.stackManager.runner.return_from_stack(result)
 
     def get_setup_value(self):
         return self._model.stackManager.runner.GetStackSetupValue()
 
+    def broadcast_message(self, message):
+        if not self._model: return
+        if not isinstance(message, str):
+            raise TypeError("broadcast_message(): message must be a string")
+
+        for c in self._model.childModels:
+            c.broadcast_message(message)
+
+    @RunOnMainAsync
+    def show_info(self):
+        self._model.stackManager.ShowStackInfo()
+
     def add_card(self, name="card", atNumber=0):
         if not isinstance(name, str):
             raise TypeError("add_card(): name is not a string")
         atNumber = int(atNumber)
         if atNumber < 0 or atNumber > len(self._model.childModels)+1:
             raise ValueError("add_card(): atNumber is out of bounds")
```

### Comparing `cardstock-0.99.5/cardstock/standalone.py` & `cardstock-0.99.6/cardstock/standalone.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/tools.py` & `cardstock-0.99.6/cardstock/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,19 @@
         self.relOrigin = self.absOrigin - wx.Point(tuple(int(x) for x in self.targetUi.model.GetAbsolutePosition()))
         self.stackManager.view.CaptureMouse()
 
         if self.targetUi.isSelected and self.shiftDown:
             self.deselectTarget = True
 
         if not selectedGroupSubview and not self.targetUi.isSelected:
-            self.stackManager.SelectUiView(self.targetUi, self.shiftDown)
+            if self.targetUi.model.type == "card" and (self.absOrigin.y < 0 or self.absOrigin.x > self.targetUi.model.GetProperty("size").width):
+                # Don't select card when a click starts outside of the card.
+                pass
+            else:
+                self.stackManager.SelectUiView(self.targetUi, self.shiftDown)
 
         self.oldFrames = {}
         selected = self.stackManager.GetSelectedUiViews()
         if self.targetUi not in selected:
             selected.append(self.targetUi)
         for ui in selected:
             frame = ui.model.GetFrame()
@@ -239,15 +243,15 @@
                 self.stackManager.view.Refresh()
                 self.UpdateBoxSelection()
                 return
 
             if self.mode == "move":
                 # We're dragging/moving an object
                 selectedViews = self.stackManager.GetSelectedUiViews()
-                if len(selectedViews) == 1 and selectedViews[0].parent.model.type == "group":
+                if len(selectedViews) == 1 and selectedViews[0].parent and selectedViews[0].parent.model.type == "group":
                     selectedViews = [self.targetUi]
                 pos = self.ConstrainDragPoint("drag", self.absOrigin, event)
                 for ui in selectedViews:
                     offset = (pos.x - self.absOrigin.x, pos.y - self.absOrigin.y)
                     origPos = self.oldFrames[ui.model.GetProperty("name")].Position
                     ui.model.SetProperty("position", [origPos.x + offset[0], origPos.y + offset[1]])
```

### Comparing `cardstock-0.99.5/cardstock/uiButton.py` & `cardstock-0.99.6/cardstock/uiButton.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 UiButton.checkboxOffBmp = rescale(UiButton.checkboxOffBmp)
 
     def GetCursor(self):
         return wx.CURSOR_HAND
 
     def OnPropertyChanged(self, model, key):
         super().OnPropertyChanged(model, key)
-        if key == "title":
+        if key == "text":
             self.stackManager.view.Refresh()
         elif key == "style":
             sm = self.stackManager
             sm.SelectUiView(None)
             sm.LoadCardAtIndex(sm.cardIndex, reload=True)
             sm.SelectUiView(sm.GetUiViewByModel(model))
         elif key == "is_selected":
@@ -116,15 +116,15 @@
             gc.SetBrush(wx.Brush('#00000044'))
             gc.DrawRoundedRectangle(wx.Rect(1, 0, width-1, height-1), 5)
             # Draw foreground round rect
             gc.SetPen(wx.Pen('#444444', fd(1)))
             gc.SetBrush(wx.Brush('#CCCCCC' if hilighted else 'white'))
             gc.DrawRoundedRectangle(wx.Rect(0, 1, width-1, height-1), 5)
 
-            title = self.model.GetProperty("title")
+            title = self.model.GetProperty("text")
             if len(title):
                 font = wx.Font(wx.FontInfo(wx.Size(0, fd(fd(16)))).Family(wx.FONTFAMILY_DEFAULT))
                 lineHeight = td(font.GetPixelSize().height)
                 (startX, startY) = (0, (height+lineHeight)/2 + (1 if fd(100) == 100 else fd(-3)))
 
                 lines = wordwrap(title, fd(width), gc)
                 line = lines.split("\n")[0]
@@ -132,15 +132,15 @@
                 gc.SetFont(font)
                 gc.SetTextForeground(wx.Colour('black'))
                 textWidth = gc.GetTextExtent(line).Width
                 xPos = (startX + (width - td(textWidth)) / 2)
                 gc.DrawText(line, wx.Point(int(xPos), int(startY)))
 
         elif style == "Borderless":
-            title = self.model.GetProperty("title")
+            title = self.model.GetProperty("text")
             if len(title):
                 (width, height) = self.model.GetProperty("size")
                 font = wx.Font(wx.FontInfo(wx.Size(0, fd(fd(16)))).Family(wx.FONTFAMILY_DEFAULT))
                 lineHeight = td(font.GetPixelSize().height)
                 (startX, startY) = (0, (height+lineHeight)/2 + (1 if fd(100) == 100 else fd(-3)))
 
                 lines = wordwrap(title, fd(width), gc)
@@ -158,15 +158,15 @@
             if style == "Radio":
                 iconBmp = UiButton.radioOnBmp if self.model.GetProperty("is_selected") else UiButton.radioOffBmp
             else:
                 iconBmp = UiButton.checkboxOnBmp if self.model.GetProperty("is_selected") else UiButton.checkboxOffBmp
             startY = int((height + iconBmp.Height) / 2) + (1 if fd(100) == 100 else fd(-3))
             gc.DrawBitmap(iconBmp, fd(2), startY)
 
-            title = self.model.GetProperty("title")
+            title = self.model.GetProperty("text")
             if len(title):
                 font = wx.Font(wx.FontInfo(wx.Size(0, fd(fd(16)))).Family(wx.FONTFAMILY_DEFAULT))
                 lineHeight = td(font.GetPixelSize().height)
                 startY = int((height + lineHeight) / 2) + (1 if fd(100) == 100 else fd(-3))
                 startPos = (25, startY)
                 gc.SetFont(font)
                 gc.SetTextForeground(wx.Colour('black'))
@@ -195,20 +195,20 @@
                     "on_selection_changed": ""}
         for k,v in self.handlers.items():
             handlers[k] = v
         self.handlers = handlers
         self.initialEditHandler = "on_click"
 
         self.properties["name"] = "button_1"
-        self.properties["title"] = "Button"
+        self.properties["text"] = "Button"
         self.properties["style"] = "Border"
         self.properties["is_selected"] = False
         self.properties["rotation"] = 0.0
 
-        self.propertyTypes["title"] = "string"
+        self.propertyTypes["text"] = "string"
         self.propertyTypes["style"] = "choice"
         self.propertyTypes["is_selected"] = "bool"
         self.propertyTypes["rotation"] = "float"
 
         self.UpdatePropKeys(self.properties["style"])
 
     def SetProperty(self, key, value, notify=True):
@@ -224,22 +224,22 @@
                     if not self.stackManager.isEditing and self.stackManager.runner and self.GetHandler("on_selection_changed"):
                         self.stackManager.runner.RunHandler(self, "on_selection_changed", None, value)
         super().SetProperty(key, value, notify)
 
     def UpdatePropKeys(self, style):
         # Custom property order and mask for the inspector
         if style in ("Border", "Borderless"):
-            self.propertyKeys = ["name", "title", "style", "rotation", "position", "size"]
+            self.propertyKeys = ["name", "text", "style", "rotation", "position", "size"]
             self.initialEditHandler = "on_click"
             if "on_click" not in self.visibleHandlers:
                 self.visibleHandlers.add("on_click")
             if "on_selection_changed" in self.visibleHandlers and len(self.handlers["on_selection_changed"]) == 0:
                 self.visibleHandlers.remove("on_selection_changed")
         else:
-            self.propertyKeys = ["name", "title", "style", "is_selected", "rotation", "position", "size"]
+            self.propertyKeys = ["name", "text", "style", "is_selected", "rotation", "position", "size"]
             self.initialEditHandler = "on_selection_changed"
             if "on_selection_changed" not in self.visibleHandlers:
                 self.visibleHandlers.add("on_selection_changed")
             if "on_click" in self.visibleHandlers and len(self.handlers["on_click"]) == 0:
                 self.visibleHandlers.remove("on_click")
 
     def get_radio_group(self):
@@ -261,23 +261,23 @@
 class Button(ViewProxy):
     """
     Button proxy objects are the user-accessible objects exposed to event handler code for button objects.
     Based on ProxyView, and adds title, border, and Click().
     """
 
     @property
-    def title(self):
+    def text(self):
         model = self._model
         if not model: return ""
-        return model.GetProperty("title")
-    @title.setter
-    def title(self, val):
+        return model.GetProperty("text")
+    @text.setter
+    def text(self, val):
         model = self._model
         if not model: return
-        model.SetProperty("title", str(val))
+        model.SetProperty("text", str(val))
 
     @property
     def style(self):
         model = self._model
         if not model: return False
         return model.GetProperty("style")
     @style.setter
```

### Comparing `cardstock-0.99.5/cardstock/uiCard.py` & `cardstock-0.99.6/cardstock/uiCard.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self.view.SetSize(size)
         self.view.SetPosition((0,0))
         self.runningInternalResize = False
 
     def OnResize(self, event):
         didEnqueue = False
         self.stackManager.view.didResize = True
-        if not self.stackManager.isEditing and self.stackManager.runner and self.stackManager.stackModel.GetProperty("can_resize"):
+        if not self.stackManager.isEditing and self.stackManager.runner and self.model.GetProperty("can_resize"):
             didEnqueue = self.stackManager.runner.RunHandler(self.model, "on_resize", None, False)
         if self.stackManager.isEditing or not didEnqueue:
             self.stackManager.view.Refresh()
             self.stackManager.view.RefreshIfNeeded()
         event.Skip()
 
     def Paint(self, gc):
@@ -145,42 +145,26 @@
         handlers = {"on_setup": "", "on_show_card": "", "on_key_press": "", "on_key_hold": "", "on_key_release": ""}
         del self.handlers["on_bounce"]
         for k,v in self.handlers.items():
             handlers[k] = v
         self.handlers = handlers
         self.handlers["on_resize"] = ""
         self.handlers["on_hide_card"] = ""
-        self.handlers["on_exit_stack"] = ""
         self.initialEditHandler = "on_setup"
 
         # Custom property order and mask for the inspector
         self.properties["name"] = "card_1"
         self.properties["fill_color"] = "white"
-        self.propertyKeys = ["name", "fill_color", "size", "can_save", "can_resize"]
+        self.properties["size"] = wx.Size(500, 500)
+        self.properties["can_resize"] = False
+        self.propertyKeys = ["name", "fill_color", "size", "can_resize"]
 
         self.propertyTypes["fill_color"] = "color"
-        self.propertyTypes["can_save"] = 'bool'
         self.propertyTypes["can_resize"] = 'bool'
 
-    def SetProperty(self, key, value, notify=True):
-        if key in ["size", "can_save", "can_resize"]:
-            self.parent.SetProperty(key, value, notify)
-        else:
-            super().SetProperty(key, value, notify)
-
-    def GetProperty(self, key):
-        if key in ["size", "can_save", "can_resize"]:
-            return self.parent.GetProperty(key)
-        else:
-            return super().GetProperty(key)
-
-    def GetFrame(self):
-        s = self.parent.GetProperty("size")
-        return wx.Rect((0,0), s)
-
     def GetAbsoluteFrame(self):
         return self.GetFrame()
 
     def GetAllChildModels(self):
         allModels = []
         for child in self.childModels:
             allModels.append(child)
@@ -189,15 +173,14 @@
         return allModels
 
     def GetData(self):
         data = super().GetData()
         data["childModels"] = []
         for m in self.childModels:
             data["childModels"].append(m.GetData())
-        data["properties"].pop("size")
         data["properties"].pop("position")
         return data
 
     def SetData(self, data):
         super().SetData(data)
         for childData in data["childModels"]:
             m = generator.StackGenerator.ModelFromData(self.stackManager, childData)
@@ -274,14 +257,21 @@
                 size = m.GetProperty("size")
                 pos = wx.Point(int((cardSize.width - (pos.x + size.width)) if fx else pos.x),
                                int((cardSize.height - (pos.y + size.height)) if fy else pos.y))
                 m.SetProperty("position", pos, notify=notify)
         if notify:
             self.Notify("size")
 
+    def broadcast_message(self, message):
+        def r_broadcast(model):
+            self.stackManager.runner.RunHandler(model, "on_message", None, message)
+            for m in model.childModels:
+                r_broadcast(m)
+        r_broadcast(self)
+
     def GetDedupNameList(self, exclude):
         names = [m.properties["name"] for m in self.GetAllChildModels()]
         for n in exclude:
             if n in names:
                 names.remove(n)
         return names
 
@@ -334,37 +324,48 @@
 
     @property
     def number(self):
         model = self._model
         if not model: return -1
         return model.parent.childModels.index(model)+1
 
-    def animate_fill_color(self, duration, endVal, on_finished=None, *args, **kwargs):
+    def broadcast_message(self, message):
+        if not self._model: return
+        if not isinstance(message, str):
+            raise TypeError("broadcast_message(): message must be a string")
+        self._model.broadcast_message(message)
+
+    def animate_fill_color(self, duration, endVal, easing=None, on_finished=None):
         if not isinstance(duration, (int, float)):
             raise TypeError("animate_fill_color(): duration must be a number")
         if not isinstance(endVal, str):
             raise TypeError("animate_fill_color(): end_color must be a string")
+        if easing and not isinstance(easing, str):
+            raise TypeError('animate_fill_color(): easing, if provided, must be one of "In", "Out", or "InOut"')
 
         model = self._model
         if not model: return
 
+        if easing:
+            easing = easing.lower()
+
         end_color = wx.Colour(endVal)
         if end_color.IsOk():
             def onStart(animDict):
                 origVal = wx.Colour(self.fill_color)
                 origParts = [origVal.Red(), origVal.Green(), origVal.Blue(), origVal.Alpha()]
                 animDict["origParts"] = origParts
                 endParts = [end_color.Red(), end_color.Green(), end_color.Blue(), end_color.Alpha()]
                 animDict["offsets"] = [endParts[i]-origParts[i] for i in range(4)]
 
             def onUpdate(progress, animDict):
-                model.SetProperty("fill_color", wx.Colour([int(animDict["origParts"][i] + animDict["offsets"][i] * progress) for i in range(4)]))
+                model.SetProperty("fill_color", wx.Colour([int(animDict["origParts"][i] + animDict["offsets"][i] * ease(progress, easing)) for i in range(4)]))
 
             def internalOnFinished(animDict):
-                if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished, *args, **kwargs)
+                if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished)
 
             model.AddAnimation("fill_color", duration, onUpdate, onStart, internalOnFinished)
 
     def add_button(self, name="button", **kwargs):
         model = self._model
         if not model: return None
         obj = model.AddNewObject("button", name, (100,24), kwargs=kwargs)
```

### Comparing `cardstock-0.99.5/cardstock/uiGroup.py` & `cardstock-0.99.6/cardstock/uiGroup.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/uiImage.py` & `cardstock-0.99.6/cardstock/uiImage.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/uiShape.py` & `cardstock-0.99.6/cardstock/uiShape.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 # This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
 # of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import wx
 from uiView import *
 from imageFactory import ImageFactory
 
+DASHES = {"Solid": wx.PENSTYLE_SOLID,
+          "Long-Dashes": wx.PENSTYLE_LONG_DASH,
+          "Dashes": wx.PENSTYLE_SHORT_DASH,
+          "Dots": wx.PENSTYLE_DOT}
+
 
 class UiShape(UiView):
     """
     This class is a controller that coordinates management of a shape view, based on data from an LineModel, ShapeModel,
     or RoundRectModel.
     A shape does not use its own wx.Window as a view, but instead draws itself onto the stack view.
     """
@@ -82,15 +87,15 @@
 
         pen_color = wx.Colour(pen_color)
         if not pen_color:
             pen_color = wx.Colour('black')
         if thickness == 0:
             pen = wx.TRANSPARENT_PEN
         else:
-            pen = wx.Pen(pen_color, self.stackManager.view.FromDIP(int(thickness)), wx.PENSTYLE_SOLID)
+            pen = wx.Pen(pen_color, self.stackManager.view.FromDIP(int(thickness)), DASHES[self.model.properties["pen_style"]])
         gc.cachedGC.SetPen(pen)
 
         if hasFill:
             pen.SetJoin(wx.JOIN_MITER)
             fill_color = wx.Colour(fill_color)
             if not fill_color:
                 fill_color = wx.Colour('white')
@@ -212,15 +217,15 @@
         for k,p in resizerPoints.items():
                 p += (thicknessOffset-2 if p.x > 0 else -thicknessOffset-2,
                       thicknessOffset-2 if p.y > 0 else -thicknessOffset-2)
         return resizerPoints
 
     def OnPropertyChanged(self, model, key):
         super().OnPropertyChanged(model, key)
-        if key in ["size", "shape", "pen_color", "pen_thickness", "fill_color", "corner_radius", "rotation"]:
+        if key in ["size", "shape", "pen_color", "pen_thickness", "pen_style",  "fill_color", "corner_radius", "rotation"]:
             self.ClearHitRegion()
             self.stackManager.view.Refresh()
         if key in ["size", "shape", "pen_thickness", "corner_radius", "rotation"]:
             self.cachedPaths = {}
 
     @staticmethod
     def CreateModelForType(stackManager, name):
@@ -251,24 +256,26 @@
         elif shapeType == "polygon":
             self.properties["name"] = "polygon_1"
         else:
             self.properties["name"] = f"{shapeType}_1"
 
         self.properties["originalSize"] = None
         self.properties["pen_color"] = "black"
+        self.properties["pen_style"] = "Solid"
         self.properties["pen_thickness"] = 2
         self.properties["rotation"] = 0.0
 
         self.propertyTypes["originalSize"] = "size"
         self.propertyTypes["pen_color"] = "color"
+        self.propertyTypes["pen_style"] = "choice"
         self.propertyTypes["pen_thickness"] = "uint"
         self.propertyTypes["rotation"] = "float"
 
         # Custom property order and mask for the inspector
-        self.propertyKeys = ["name", "pen_color", "pen_thickness", "position", "size", "rotation"]
+        self.propertyKeys = ["name", "pen_color", "pen_thickness", "pen_style", "position", "size", "rotation"]
 
     def GetData(self):
         data = super().GetData()
         data["points"] = self.points.copy()
         return data
 
     def SetData(self, data):
@@ -411,14 +418,27 @@
         if not isinstance(val, str):
             raise TypeError("pen_color must be a string")
         model = self._model
         if not model: return
         model.SetProperty("pen_color", val)
 
     @property
+    def pen_style(self):
+        model = self._model
+        if not model: return ""
+        return model.GetProperty("pen_style")
+    @pen_style.setter
+    def pen_style(self, val):
+        if not isinstance(val, str):
+            raise TypeError("pen_style must be one of 'Solid', 'Long-Dashes', 'Dashes', 'Dots'")
+        model = self._model
+        if not model: return
+        model.SetProperty("pen_style", val)
+
+    @property
     def pen_thickness(self):
         model = self._model
         if not model: return 0
         return model.GetProperty("pen_thickness")
     @pen_thickness.setter
     def pen_thickness(self, val):
         if not isinstance(val, (int, float)):
@@ -440,59 +460,69 @@
         try:
             points = [wx.RealPoint(p[0], p[1]) for p in points]
         except:
             raise ValueError("points must be either a list of points, or a list of lists of two numbers")
 
         model.SetPoints(points)
 
-    def animate_pen_thickness(self, duration, endVal, on_finished=None, *args, **kwargs):
+    def animate_pen_thickness(self, duration, endVal, easing=None, on_finished=None):
         if not isinstance(duration, (int, float)):
             raise TypeError("animate_pen_thickness(): duration must be a number")
         if not isinstance(endVal, (int, float)):
             raise TypeError("animate_pen_thickness(): end_thickness must be a number")
+        if easing and not isinstance(easing, str):
+            raise TypeError('animate_pen_thickness(): easing, if provided, must be one of "In", "Out", or "InOut"')
 
         model = self._model
         if not model: return
 
+        if easing:
+            easing = easing.lower()
+
         def onStart(animDict):
             origVal = self.pen_thickness
             animDict["origVal"] = origVal
             animDict["offset"] = endVal - origVal
 
         def onUpdate(progress, animDict):
-            model.SetProperty("pen_thickness", animDict["origVal"] + animDict["offset"] * progress)
+            model.SetProperty("pen_thickness", animDict["origVal"] + animDict["offset"] * ease(progress, easing))
 
         def internalOnFinished(animDict):
-            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished, *args, **kwargs)
+            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished)
 
         model.AddAnimation("pen_thickness", duration, onUpdate, onStart, internalOnFinished)
 
-    def animate_pen_color(self, duration, endVal, on_finished=None, *args, **kwargs):
+    def animate_pen_color(self, duration, endVal, easing=None, on_finished=None):
         if not isinstance(duration, (int, float)):
             raise TypeError("animate_pen_color(): duration must be a number")
         if not isinstance(endVal, str):
             raise TypeError("animate_pen_color(): end_color must be a string")
+        if easing and not isinstance(easing, str):
+            raise TypeError('animate_pen_color(): easing, if provided, must be one of "In", "Out", or "InOut"')
 
         model = self._model
         if not model: return
 
+        if easing:
+            easing = easing.lower()
+
         end_color = wx.Colour(endVal)
         if end_color.IsOk():
             def onStart(animDict):
                 origVal = wx.Colour(self.pen_color)
                 origParts = [origVal.Red(), origVal.Green(), origVal.Blue(), origVal.Alpha()]
                 animDict["origParts"] = origParts
                 endParts = [end_color.Red(), end_color.Green(), end_color.Blue(), end_color.Alpha()]
                 animDict["offsets"] = [endParts[i]-origParts[i] for i in range(4)]
 
             def onUpdate(progress, animDict):
-                model.SetProperty("pen_color", wx.Colour([int(animDict["origParts"][i] + animDict["offsets"][i] * progress) for i in range(4)]))
+                model.SetProperty("pen_color", wx.Colour([int(animDict["origParts"][i] + animDict["offsets"][i] * ease(progress, easing)) for i in range(4)]))
 
             def internalOnFinished(animDict):
-                if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished, *args, **kwargs)
+                if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished)
 
             model.AddAnimation("pen_color", duration, onUpdate, onStart, internalOnFinished)
 
 
 class ShapeModel(LineModel):
     """
     This is the model class for Oval and Rectangle objects, and the superclass for models for round-rects.
@@ -502,15 +532,15 @@
         super().__init__(stackManager, shapeType)
         self.proxyClass = Shape
 
         self.properties["fill_color"] = "white"
         self.propertyTypes["fill_color"] = "color"
 
         # Custom property order and mask for the inspector
-        self.propertyKeys = ["name", "pen_color", "pen_thickness", "fill_color", "position", "size", "rotation"]
+        self.propertyKeys = ["name", "pen_color", "pen_thickness", "pen_style",  "fill_color", "position", "size", "rotation"]
 
     def SetShape(self, shape):
         self.properties["fill_color"] = shape["fill_color"]
         super().SetShape(shape)
 
 
 class Shape(Line):
@@ -549,37 +579,42 @@
     def fill_color(self, val):
         if not isinstance(val, str):
             raise TypeError("fill_color must be a string")
         model = self._model
         if not model: return
         model.SetProperty("fill_color", val)
 
-    def animate_fill_color(self, duration, endVal, on_finished=None, *args, **kwargs):
+    def animate_fill_color(self, duration, endVal, easing=None, on_finished=None):
         if not isinstance(duration, (int, float)):
             raise TypeError("animate_fill_color(): duration must be a number")
         if not isinstance(endVal, str):
             raise TypeError("animate_fill_color(): end_color must be a string")
+        if easing and not isinstance(easing, str):
+            raise TypeError('animate_fill_color(): easing, if provided, must be one of "In", "Out", or "InOut"')
 
         model = self._model
         if not model: return
 
+        if easing:
+            easing = easing.lower()
+
         end_color = wx.Colour(endVal)
         if end_color.IsOk():
             def onStart(animDict):
                 origVal = wx.Colour(self.fill_color)
                 origParts = [origVal.Red(), origVal.Green(), origVal.Blue(), origVal.Alpha()]
                 animDict["origParts"] = origParts
                 endParts = [end_color.Red(), end_color.Green(), end_color.Blue(), end_color.Alpha()]
                 animDict["offsets"] = [endParts[i]-origParts[i] for i in range(4)]
 
             def onUpdate(progress, animDict):
-                model.SetProperty("fill_color", wx.Colour([int(animDict["origParts"][i] + animDict["offsets"][i] * progress) for i in range(4)]))
+                model.SetProperty("fill_color", wx.Colour([int(animDict["origParts"][i] + animDict["offsets"][i] * ease(progress, easing)) for i in range(4)]))
 
             def internalOnFinished(animDict):
-                if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished, *args, **kwargs)
+                if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished)
 
             model.AddAnimation("fill_color", duration, onUpdate, onStart, internalOnFinished)
 
 
 class RoundRectModel(ShapeModel):
     """
     This is the model class for Round Rectangle objects.
@@ -589,15 +624,15 @@
         super().__init__(stackManager, shapeType)
         self.proxyClass = RoundRect
 
         self.properties["corner_radius"] = 8
         self.propertyTypes["corner_radius"] = "uint"
 
         # Custom property order and mask for the inspector
-        self.propertyKeys = ["name", "pen_color", "pen_thickness", "fill_color", "corner_radius", "position", "size", "rotation"]
+        self.propertyKeys = ["name", "pen_color", "pen_thickness", "pen_style", "fill_color", "corner_radius", "position", "size", "rotation"]
 
     def SetShape(self, shape):
         self.properties["corner_radius"] = shape["corner_radius"] if "corner_radius" in shape else 8
         super().SetShape(shape)
 
 
 class RoundRect(Shape):
@@ -615,28 +650,33 @@
     def corner_radius(self, val):
         if not isinstance(val, (int, float)):
             raise TypeError("corner_radius must be a number")
         model = self._model
         if not model: return
         model.SetProperty("corner_radius", val)
 
-    def animate_corner_radius(self, duration, endVal, on_finished=None, *args, **kwargs):
+    def animate_corner_radius(self, duration, endVal, easing=None, on_finished=None):
         if not isinstance(duration, (int, float)):
             raise TypeError("animate_corner_radius(): duration must be a number")
         if not isinstance(endVal, (int, float)):
             raise TypeError("animate_corner_radius(): end_corner_radius must be a number")
+        if easing and not isinstance(easing, str):
+            raise TypeError('animate_corner_radius(): easing, if provided, must be one of "In", "Out", or "InOut"')
 
         model = self._model
         if not model: return
 
+        if easing:
+            easing = easing.lower()
+
         def onStart(animDict):
             origVal = self.corner_radius
             animDict["origVal"] = origVal
             animDict["offset"] = endVal - origVal
 
         def onUpdate(progress, animDict):
-            model.SetProperty("corner_radius", animDict["origVal"] + animDict["offset"] * progress)
+            model.SetProperty("corner_radius", animDict["origVal"] + animDict["offset"] * ease(progress, easing))
 
         def internalOnFinished(animDict):
-            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished, *args, **kwargs)
+            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished)
 
         model.AddAnimation("corner_radius", duration, onUpdate, onStart, internalOnFinished)
```

### Comparing `cardstock-0.99.5/cardstock/uiTextBase.py` & `cardstock-0.99.6/cardstock/uiTextBase.py`

 * *Files 3% similar despite different names*

```diff
@@ -284,54 +284,64 @@
             raise TypeError("is_underlined must be True or False")
         model = self._model
         if not model: return
         if model.type == "textfield":
             raise TypeError("Text Field objects do not support underlined text.")
         model.SetProperty("is_underlined", val)
 
-    def animate_font_size(self, duration, endVal, on_finished=None, *args, **kwargs):
+    def animate_font_size(self, duration, endVal, easing=None, on_finished=None):
         if not isinstance(duration, (int, float)):
             raise TypeError("animate_font_size(): duration must be a number")
         if not isinstance(endVal, (int, float)):
             raise TypeError("animate_font_size(): end_thickness must be a number")
+        if easing and not isinstance(easing, str):
+            raise TypeError('animate_font_size(): easing, if provided, must be one of "In", "Out", or "InOut"')
 
         model = self._model
         if not model: return
 
+        if easing:
+            easing = easing.lower()
+
         def onStart(animDict):
             origVal = self.font_size
             animDict["origVal"] = origVal
             animDict["offset"] = endVal - origVal
 
         def onUpdate(progress, animDict):
-            model.SetProperty("font_size", animDict["origVal"] + animDict["offset"] * progress)
+            model.SetProperty("font_size", animDict["origVal"] + animDict["offset"] * ease(progress, easing))
 
         def internalOnFinished(animDict):
-            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished, *args, **kwargs)
+            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished)
 
         model.AddAnimation("font_size", duration, onUpdate, onStart, internalOnFinished)
 
-    def animate_text_color(self, duration, endVal, on_finished=None, *args, **kwargs):
+    def animate_text_color(self, duration, endVal, easing=None, on_finished=None):
         if not isinstance(duration, (int, float)):
             raise TypeError("animate_text_color(): duration must be a number")
         if not isinstance(endVal, str):
             raise TypeError("animate_text_color(): end_color must be a string")
+        if easing and not isinstance(easing, str):
+            raise TypeError('animate_text_color(): easing, if provided, must be one of "In", "Out", or "InOut"')
 
         model = self._model
         if not model: return
 
+        if easing:
+            easing = easing.lower()
+
         end_color = wx.Colour(endVal)
         if end_color.IsOk():
             def onStart(animDict):
                 origVal = wx.Colour(self.text_color)
                 origParts = [origVal.Red(), origVal.Green(), origVal.Blue(), origVal.Alpha()]
                 animDict["origParts"] = origParts
                 endParts = [end_color.Red(), end_color.Green(), end_color.Blue(), end_color.Alpha()]
                 animDict["offsets"] = [endParts[i]-origParts[i] for i in range(4)]
 
             def onUpdate(progress, animDict):
-                model.SetProperty("text_color", wx.Colour([int(animDict["origParts"][i] + animDict["offsets"][i] * progress) for i in range(4)]))
+                model.SetProperty("text_color", wx.Colour([int(animDict["origParts"][i] + animDict["offsets"][i] * ease(progress, easing)) for i in range(4)]))
 
             def internalOnFinished(animDict):
-                if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished, *args, **kwargs)
+                if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished)
 
             model.AddAnimation("text_color", duration, onUpdate, onStart, internalOnFinished)
```

### Comparing `cardstock-0.99.5/cardstock/uiTextField.py` & `cardstock-0.99.6/cardstock/uiTextField.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/uiTextLabel.py` & `cardstock-0.99.6/cardstock/uiTextLabel.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/uiView.py` & `cardstock-0.99.6/cardstock/uiView.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 # This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.  If a copy
 # of the MPL was not distributed with this file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import wx
 import threading
 import ast
 import re
+from easing import ease
 import generator
-import helpData
+import helpDataGen
 from time import time
 from codeRunnerThread import RunOnMainSync, RunOnMainAsync
 from cardstockFrameParts import *
 import sanitizer
 import math
 from imageFactory import ImageFactory
 
@@ -106,15 +107,15 @@
         else:
             return None
 
     def OnPropertyChanged(self, model, key):
         if key in ["position", "size", "rotation"]:
             if self.view:
                 s = model.GetProperty("size")
-                if model.type in ("stack", "card"):
+                if model.type == "card":
                     self.stackManager.uiCard.ResizeCardView(s)
                     pos = (0,0)
                 else:
                     c = self.stackManager.ConvPoint(wx.Point(model.GetCenter()))
                     s = self.view.FromDIP(model.GetProperty("size"))
                     pos = c - s / 2
                     self.view.SetSize(s)
@@ -373,15 +374,15 @@
             self.PaintSelectionBox(gc)
         for ui in self.uiViews:
             ui.DoPaintSelectionBoxes(gc)
         self.PostPaint(gc)
 
     def PrePaint(self, gc):
         # Rotate and Translate the GC, such that we can draw this object in local coords
-        stackSize = self.stackManager.stackModel.properties["size"]
+        stackSize = self.stackManager.uiCard.model.GetProperty("size")
         pos = self.model.properties["position"]
         rot = self.model.GetProperty("rotation")
         rot = math.radians(rot) if rot else None
         gc.cachedGC.PushState()
         scale = self.stackManager.view.FromDIP(1000)/1000.0
 
         if rot:
@@ -623,15 +624,15 @@
     This is the abstract base class for the other model classes.
     The model holds the property values and event handler text for each object.
     It also holds the type of each property, and the ordered list of properties to display in the inspector.
     It also handles animating properties of the object, like position, size, or color.
     """
 
     minSize = wx.Size(20, 20)
-    reservedNames = helpData.HelpData.ReservedNames()
+    reservedNames = helpDataGen.HelpData.ReservedNames()
 
     def __init__(self, stackManager):
         super().__init__()
         self.type = None
         self.parent = None
         self.handlers = {"on_setup": "",
                          "on_mouse_enter": "",
@@ -962,14 +963,16 @@
             return ["Left", "Center", "Right"]
         elif key == "font":
             return ["Default", "Serif", "Sans-Serif", "Mono"]
         elif key == "fit":
             return ["Center", "Stretch", "Contain", "Fill"]
         elif key == "style":
             return ["Border", "Borderless", "Checkbox", "Radio"]
+        elif key == "pen_style":
+            return ["Solid", "Long-Dashes", "Dashes", "Dots"]
         return []
 
     def GetProperty(self, key):
         if key == "center":
             return self.GetAbsoluteCenter()
         elif key in self.properties:
             return self.properties[key]
@@ -1178,14 +1181,16 @@
                     del self.animations[key]
                 if "startTime" in animDict and animDict["onFinish"]:
                     animDict["onFinish"](animDict)
 
     def StopAnimation(self, key=None):
         # On Runner thread
         if key:
+            if key == "center":
+                key = "position"
             # Stop animating this one property
             with self.animLock:
                 if key in self.animations:
                     animDict = self.animations[key][0]
                     if "startTime" in animDict and animDict["onCancel"]:
                         animDict["onCancel"](animDict)
                     del self.animations[key]
@@ -1220,16 +1225,15 @@
         if not self.proxy:
             self.proxy = self.proxyClass(self)
         return self.proxy
 
     def RunSetup(self, runner):
         if self.type == "card":
             runner.SetupForCard(self)
-        if self.GetHandler("on_setup"):
-            runner.RunHandler(self, "on_setup", None)
+        runner.RunHandler(self, "on_setup", None)
         for m in self.childModels:
             m.RunSetup(runner)
 
 
 class ViewProxy(object):
     """
     This class and its subclasses are the user-accessible objects exposed to event handler code.
@@ -1334,32 +1338,14 @@
         else:
             @RunOnMainSync
             def func():
                 # When cloning a card, update the model and view together in a rare synchronous call to the main thread
                 sm.RemoveCardRaw(model)
             func()
 
-    @RunOnMainSync
-    def cut(self):
-        # update the model and view together in a rare synchronous call to the main thread
-        model = self._model
-        if not model: return
-
-        model.stackManager.CutModels([model], False)
-
-    @RunOnMainSync
-    def copy(self):
-        # update the model and view together in a rare synchronous call to the main thread
-        model = self._model
-        if not model: return
-
-        model.stackManager.CopyModels([model])
-
-    # Paste is in the runner
-
     @property
     def name(self):
         model = self._model
         if not model: return ""
         return model.GetProperty("name")
 
     @property
@@ -1552,14 +1538,15 @@
             raise TypeError("set_code_for_event(): eventName must be a string")
         if not isinstance(code, str):
             raise TypeError("set_code_for_event(): code must be a string")
         if eventName not in model.handlers:
             raise TypeError(f"set_code_for_event(): this object has no event called '{eventName}'")
 
         model.handlers[eventName] = code
+        model.stackManager.runner.HandlerChanged(model, eventName)
 
     def set_bounce_objects(self, objects):
         if not isinstance(objects, (list, tuple)):
             raise TypeError("set_bounce_objects(): objects needs to be a list of cardstock objects")
         models = [o._model for o in objects if isinstance(o, ViewProxy)]
         self._model.SetBounceModels(models)
 
@@ -1674,115 +1661,135 @@
                 edges.remove("Bottom")
             if len(edges) == 3 and "Left" in edges and "Right" in edges:
                 edges.remove("Left")
                 edges.remove("Right")
             return edges
         return f()
 
-    def animate_position(self, duration, end_position, on_finished=None, *args, **kwargs):
+    def animate_position(self, duration, end_position, easing=None, on_finished=None):
         if not isinstance(duration, (int, float)):
             raise TypeError("animate_position(): duration must be a number")
         try:
             end_position = wx.RealPoint(*end_position)
         except:
             raise ValueError("animate_position(): end_position must be a point or a list of two numbers")
+        if easing and not isinstance(easing, str):
+            raise TypeError('animate_position(): easing, if provided, must be one of "In", "Out", or "InOut"')
 
         model = self._model
         if not model: return
 
+        if easing:
+            easing = easing.lower()
+
         def onStart(animDict):
             origPosition = model.GetAbsolutePosition()
             offsetPt = end_position - tuple(origPosition)
             offset = wx.RealPoint(offsetPt[0], offsetPt[1])
             animDict["origPosition"] = origPosition
             animDict["offset"] = offset
             model.SetProperty("speed", offset*(1.0/duration))
 
         def onUpdate(progress, animDict):
-            model.SetAbsolutePosition(animDict["origPosition"] + tuple(animDict["offset"] * progress))
+            model.SetAbsolutePosition(animDict["origPosition"] + tuple(animDict["offset"] * ease(progress, easing)))
 
         def internalOnFinished(animDict):
             model.SetProperty("speed", (0,0), notify=False)
-            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished, *args, **kwargs)
+            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished)
 
         def onCanceled(animDict):
             model.SetProperty("speed", (0,0))
 
         model.AddAnimation("position", duration, onUpdate, onStart, internalOnFinished, onCanceled)
 
-    def animate_center(self, duration, end_center, on_finished=None, *args, **kwargs):
+    def animate_center(self, duration, end_center, easing=None, on_finished=None):
         if not isinstance(duration, (int, float)):
             raise TypeError("animate_center(): duration must be a number")
         try:
             end_center = wx.RealPoint(*end_center)
         except:
             raise ValueError("animate_center(): end_center must be a point or a list of two numbers")
+        if easing and not isinstance(easing, str):
+            raise TypeError('animate_center(): easing, if provided, must be one of "In", "Out", or "InOut"')
 
         model = self._model
         if not model: return
 
+        if easing:
+            easing = easing.lower()
+
         def onStart(animDict):
             origCenter = model.GetCenter()
             offsetPt = end_center - tuple(origCenter)
             offset = wx.RealPoint(offsetPt[0], offsetPt[1])
             animDict["origCenter"] = origCenter
             animDict["offset"] = offset
             self._model.SetProperty("speed", offset*(1.0/duration))
 
         def onUpdate(progress, animDict):
-            model.SetCenter(animDict["origCenter"] + tuple(animDict["offset"] * progress))
+            model.SetCenter(animDict["origCenter"] + tuple(animDict["offset"] * ease(progress, easing)))
 
         def internalOnFinished(animDict):
             model.SetProperty("speed", (0,0), notify=False)
-            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished, *args, **kwargs)
+            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished)
 
         def onCanceled(animDict):
             model.SetProperty("speed", (0,0))
 
         model.AddAnimation("position", duration, onUpdate, onStart, internalOnFinished, onCanceled)
 
-    def animate_size(self, duration, end_size, on_finished=None, *args, **kwargs):
+    def animate_size(self, duration, end_size, easing=None, on_finished=None):
         if not isinstance(duration, (int, float)):
             raise TypeError("animate_size(): duration must be a number")
         try:
             end_size = wx.Size(end_size)
         except:
             raise ValueError("animate_size(): end_size must be a size or a list of two numbers")
+        if easing and not isinstance(easing, str):
+            raise TypeError('animate_size(): easing, if provided, must be one of "In", "Out", or "InOut"')
 
         model = self._model
         if not model: return
 
+        if easing:
+            easing = easing.lower()
+
         def onStart(animDict):
             origSize = model.GetProperty("size")
             offset = wx.Size(end_size-tuple(origSize))
             animDict["origSize"] = origSize
             animDict["offset"] = offset
 
         def onUpdate(progress, animDict):
-            model.SetProperty("size", animDict["origSize"] + tuple(animDict["offset"] * progress))
+            model.SetProperty("size", animDict["origSize"] + tuple(animDict["offset"] * ease(progress, easing)))
 
         def internalOnFinished(animDict):
-            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished, *args, **kwargs)
+            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished)
 
         model.AddAnimation("size", duration, onUpdate, onStart, internalOnFinished)
 
-    def animate_rotation(self, duration, end_rotation, force_direction=0, on_finished=None, *args, **kwargs):
+    def animate_rotation(self, duration, end_rotation, force_direction=0, easing=None, on_finished=None):
         if self._model.GetProperty("rotation") is None:
             raise TypeError("animate_rotation(): object does not support rotation")
 
         if not isinstance(duration, (int, float)):
             raise TypeError("animate_rotation(): duration must be a number")
         if not isinstance(end_rotation, (int, float)):
             raise TypeError("animate_rotation(): end_rotation must be a number")
         if not isinstance(force_direction, (int, float)):
             raise TypeError("animate_rotation(): force_direction must be a number")
+        if easing and not isinstance(easing, str):
+            raise TypeError('animate_rotation(): easing, if provided, must be one of "In", "Out", or "InOut"')
 
         model = self._model
         if not model: return
 
+        if easing:
+            easing = easing.lower()
+
         end_rotation = end_rotation
 
         def onStart(animDict):
             origVal = self.rotation
             animDict["origVal"] = origVal
             offset = end_rotation - origVal
             if force_direction:
@@ -1792,18 +1799,18 @@
                     if offset >= 0: offset -= 360
             else:
                 if offset > 180: offset -= 360
                 if offset < -180: offset += 360
             animDict["offset"] = offset
 
         def onUpdate(progress, animDict):
-            model.SetProperty("rotation", (animDict["origVal"] + animDict["offset"] * progress)%360)
+            model.SetProperty("rotation", (animDict["origVal"] + animDict["offset"] * ease(progress, easing))%360)
 
         def internalOnFinished(animDict):
-            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished, *args, **kwargs)
+            if on_finished: self._model.stackManager.runner.EnqueueFunction(on_finished)
 
         model.AddAnimation("rotation", duration, onUpdate, onStart, internalOnFinished)
 
     def stop_animating(self, property_name=None):
         model = self._model
         if not model: return
         model.StopAnimation(property_name)
```

### Comparing `cardstock-0.99.5/cardstock/uiWebView.py` & `cardstock-0.99.6/cardstock/uiWebView.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/variablesWindow.py` & `cardstock-0.99.6/cardstock/variablesWindow.py`

 * *Files identical despite different names*

### Comparing `cardstock-0.99.5/cardstock/viewer.py` & `cardstock-0.99.6/cardstock/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from findEngineViewer import FindEngine
 from consoleWindow import ConsoleWindow
 from variablesWindow import VariablesWindow
 from codeRunnerThread import RunOnMainSync, RunOnMainAsync
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
+ID_SHOW_INFO = wx.NewIdRef()
 ID_MENU_FIND = wx.NewIdRef()
 ID_MENU_FIND_SEL = wx.NewIdRef()
 ID_MENU_FIND_NEXT = wx.NewIdRef()
 ID_MENU_FIND_PREV = wx.NewIdRef()
 ID_MENU_REPLACE = wx.NewIdRef()
 ID_SHOW_VARIABLES = wx.NewIdRef()
 ID_SHOW_CONSOLE = wx.NewIdRef()
@@ -91,20 +92,19 @@
             self.findEngine.stackManager = None
             self.findEngine = None
         self.designer = None
         self.stackManager = None
         return super().Destroy()
 
     def OnResize(self, event):
-        if self.stackManager:
-            if self.stackManager.stackModel.GetProperty("can_resize"):
-                if not self.stackManager.uiCard.runningInternalResize:
-                    size = self.stackManager.view.GetTopLevelParent().GetClientSize()
-                    size = self.stackManager.view.ToDIP(size)
-                    self.stackManager.uiCard.model.SetProperty("size", size)
+        if self.stackManager and self.stackManager.uiCard.model.GetProperty("can_resize"):
+            if not self.stackManager.uiCard.runningInternalResize:
+                size = self.stackManager.view.GetTopLevelParent().GetClientSize()
+                size = self.stackManager.view.ToDIP(size)
+                self.stackManager.uiCard.model.SetProperty("size", size)
         event.Skip()
 
     def SaveFile(self):
         if self.designer:
             self.designer.OnViewerSave(self.stackManager.stackModel)
 
         if self.stackManager.filename:
@@ -118,14 +118,19 @@
                 # e = sys.exc_info()
                 # print(e)
                 wx.MessageDialog(None, str("Couldn't save file"), "", wx.OK).ShowModal()
 
     def MakeMenuBar(self):
         # create the file menu
         fileMenu = wx.Menu()
+
+        if self.stackManager.stackModel.GetProperty("info").strip():
+            fileMenu.Append(ID_SHOW_INFO, "Stack &Info\tCtrl-I", "Stack Info")
+            fileMenu.AppendSeparator()
+
         if not self.isStandalone and not self.designer:
             fileMenu.Append(wx.ID_OPEN, "&Open\tCtrl-O", "Open Stack")
         if self.stackManager.filename and self.stackManager.stackModel.GetProperty("can_save"):
             fileMenu.Append(wx.ID_SAVE, "&Save\tCtrl-S", "Save Stack")
         if self.designer:
             fileMenu.Append(wx.ID_CLOSE, "&Close\tCtrl-W", "Close Stack")
         else:
@@ -156,14 +161,16 @@
         menuBar = wx.MenuBar()
         if self.designer or fileMenu.GetMenuItemCount() > 1:
             menuBar.Append(fileMenu, "&File")
         menuBar.Append(editMenu, "&Edit")
         menuBar.Append(helpMenu, "&Help")
         self.SetMenuBar(menuBar)
 
+        self.Bind(wx.EVT_MENU,  self.OnMenuInfo, id=ID_SHOW_INFO)
+
         self.Bind(wx.EVT_MENU,   self.OnMenuOpen, id=wx.ID_OPEN)
         self.Bind(wx.EVT_MENU,   self.OnMenuSave, id=wx.ID_SAVE)
         self.Bind(wx.EVT_MENU,   self.OnMenuClose, id=wx.ID_CLOSE)
         self.Bind(wx.EVT_MENU,   self.OnMenuClose, id=wx.ID_EXIT)
 
         self.Bind(wx.EVT_MENU,  self.OnMenuAbout, id=wx.ID_ABOUT)
 
@@ -301,15 +308,17 @@
             if r == wx.ID_CANCEL:
                 event.Veto()
                 return
             if r == wx.ID_YES:
                 self.SaveFile()
 
         if not self.stackManager.runner.stopRunnerThread:
-            for l in range(len(self.stackStack)-1):
+            self.stackManager.runner.RunHandler(self.stackManager.stackModel, "on_exit_stack", None)
+
+            for _ in range(len(self.stackStack)-1):
                 self.PopStack(None, True)
 
             self.stackManager.SetDown()
             if self.consoleWindow:
                 self.consoleWindow.Destroy()
                 self.consoleWindow = None
             event.Skip()
@@ -417,14 +426,18 @@
 
     def OnReplaceEvent(self, event):
         self.findEngine.Replace()
 
     def OnReplaceAllEvent(self, event):
         self.findEngine.ReplaceAll()
 
+    def OnMenuInfo(self, event=None):
+        info = self.stackManager.stackModel.GetProperty("info")
+        wx.MessageDialog(None, info, "Stack Info", wx.OK).ShowModal()
+
     def OnMenuAbout(self, event):
         dlg = helpDialogs.CardStockAbout(self)
         dlg.ShowModal()
         dlg.Destroy()
 
     def OnMenuShowVariablesWindow(self, event):
         if self.variablesWindow.IsShown():
@@ -520,21 +533,21 @@
     def SetupViewerSize(self):
         # Size the stack viewer window for the new stack, and allow resizing only if can_resize==True
 
         if wx.Platform != "__WXGTK__":
             self.SetMaxClientSize(wx.DefaultSize)
             self.SetMinClientSize(wx.DefaultSize)
 
-        cs = self.FromDIP(self.stackManager.stackModel.GetProperty("size"))
+        cs = self.FromDIP(self.stackManager.uiCard.model.GetProperty("size"))
 
         self.stackManager.view.SetSize(cs)
         self.stackManager.UpdateBuffer()
         self.SetClientSize(cs)
 
-        if self.stackManager.stackModel.GetProperty("can_resize"):
+        if self.stackManager.uiCard.model.GetProperty("can_resize"):
             self.SetMinClientSize(self.FromDIP(wx.Size(200,200)))
         else:
             self.SetMaxClientSize(cs)
             self.SetMinClientSize(cs)
 
     def RunViewer(self, runner, stackModel, filename, cardIndex, ioValue, isGoingBack):
         # Load the model, start the runner, and handle ioValues(setup and return values) for pushed/popped stacks
@@ -547,24 +560,25 @@
             runner.stackSetupValue = ioValue
         self.stackManager.runner = runner
         self.MakeMenuBar()
         if self.consoleWindow:
             self.MakeConsoleMenuBar()
         if self.variablesWindow:
             self.MakeVariablesMenuBar()
-        self.SetupViewerSize()
 
         if self.designer:
             runner.AddSyntaxErrors(self.designer.stackManager.analyzer.syntaxErrors)
         if not isGoingBack:
+            self.stackManager.runner.SetupForCard(self.stackManager.stackModel.childModels[0])
             self.stackManager.stackModel.RunSetup(runner)
         self.stackManager.LoadCardAtIndex(None)
         if not (0 <= cardIndex < len(self.stackManager.stackModel.childModels)):
             cardIndex = 0
         self.stackManager.LoadCardAtIndex(cardIndex)
+        self.SetupViewerSize()
         if self.generateThumbnail:
             # Once loading has finished, we'll call MakeThumbnail
             runner.AddCallbackToMain(self.MakeThumbnail)
 
         if isGoingBack:
             runner.DoReturnFromStack(ioValue)
```

### Comparing `cardstock-0.99.5/cardstock.egg-info/PKG-INFO` & `cardstock-0.99.6/cardstock.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: cardstock
-Version: 0.99.5
+Version: 0.99.6
 Summary: A simple development and rapid prototyping tool for quickly building multi-platform desktop programs and web apps.
 Home-page: https://github.com/benjie-git/CardStock/wiki
 Author: Ben Levitt
 Author-email: benjie@gmail.com
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.12,>=3.7
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrdict3
 Requires-Dist: wxpython
 Requires-Dist: PyInstaller
 Requires-Dist: requests
 Requires-Dist: simpleaudio
@@ -70,38 +70,62 @@
 * Stacks can only import additional modules, and export stacks that include them, when running from source.  Not when running from the prebuilt applications. (The prebuilt applications are built with a few additional libraries: requests, pyserial, and more could be added by request.)
 * Ironically, WebViews do not work in the web-based viewer on https://cardstock.run.
 * For performance reasons, currently mouse events don't propagate through all overlapping objects when running on the web-viewer, just the topmost object under the mouse, any containing groups, and the card.
 
 ## Requirements
 The prebuilt applications for Mac and Windows have no external dependencies.
 
-Running CardStock from source requires Python 3.7 or newer (3.11 recommended), and wxPython 4.1 or newer (wxPython 4.2.x recommended).
+Running CardStock from source requires Python 3.9 or newer (3.11 recommended), and wxPython 4.1 or newer (wxPython 4.2.x recommended).
 CardStock requires installing the python modules attrdict3(linux-only), wxpython, simpleaudio, PyInstaller, and requests.  
 For mp3 playback support, you'll need to install the lame package (mp3 decoder), and python's streamp3. 
-Note that Python 3.12 is currently incompatible with wxpython, and so will not run CardStock until
+Note that Python 3.12 is currently incompatible with released versions of wxpython, and so will not run CardStock until
 wxPython receives an update.
 
 ## Installation
 You can either:
 
 ### 1. Run it from source:
 1. install python3  # Note: Python3.12 is incompatible with wxpython, so 3.11 is recommended
 2. Linux-only: apt install libasound2-dev lame libwebkit2gtk-4.0-dev  # or equivalent on non-debian/ubuntu distros
-3. Linux-only: pip3 install attrdict3
-4. Mac-only: brew install lame
+3. Mac-only: brew install lame
+4. pip3 install attrdict3
 5. pip3 install wxpython PyInstaller simpleaudio requests  # note that wxpython can take a long time to build
-6. download or clone this repository
-7. run designer.py and viewer.py as desired
-8. optionally run build.py to create your own standalone applications for the Designer and Viewer applications.
+6. To include mp3 support: pip3 install streamp3
+
+   (Note that this may require setting LDFLAGS and CPPFLAGS to allow finding the lame header and library files.
+
+    You may need to run this as something like
+
+   `CPPFLAGS=-I/opt/homebrew/include LDFLAGS=-L/opt/homebrew/lib pip3 install streamp3` or 
+
+    `CPPFLAGS=-I/usr/local/include LDFLAGS=-L/usr/local/lib pip3 install streamp3`
+
+    depending on where the lame library was installed.)
+   
+7. download or clone this repository
+8. run designer.py and viewer.py as desired
+9. optionally run build.py to create your own standalone applications for the Designer and Viewer applications.
 
 ### 2. Install using pip/pypi:
 1. Linux-only: apt install libasound2-dev lame libwebkit2gtk-4.0-dev  # or equivalent on non-debian/ubuntu distros
 2. Mac-only: brew install lame
-3. pip3 install cardstock  # note that the dependency wxpython can take a very long time to build
-4. run using the newly installed commands cardstock and cardstock_viewer
+3. To include mp3 support: pip3 install streamp3
+
+   (Note that this may require setting LDFLAGS and CPPFLAGS to allow finding the lame header and library files.
+
+    You may need to run this as something like
+
+   `CPPFLAGS=-I/opt/homebrew/include LDFLAGS=-L/opt/homebrew/lib pip3 install streamp3` or 
+
+    `CPPFLAGS=-I/usr/local/include LDFLAGS=-L/usr/local/lib pip3 install streamp3`
+
+    depending on where the lame library was installed.)
+
+4. pip3 install cardstock  # note that the dependency wxpython can take a very long time to build
+5. run using the newly installed commands cardstock and cardstock_viewer
 
 ### 3. Or download the latest, pre-built CardStock application for Mac or Windows
 1. Download CardStock for Mac or Windows here: https://github.com/benjie-git/CardStock/releases/latest
 2. Note that the pre-built Windows app is not yet code-signed, so Windows will complain the first time you open the app. If a window appears saying "Windows protected your PC", click the More Info link at the end of the warning paragraph, and then the "Run Anyway" button that appears at the bottom of the window.
 
 
 ## Reference
```

### Comparing `cardstock-0.99.5/cardstock.egg-info/SOURCES.txt` & `cardstock-0.99.6/cardstock.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,21 +13,23 @@
 ./cardstock/cardstockFrameParts.py
 ./cardstock/codeInspector.py
 ./cardstock/codeInspectorMulti.py
 ./cardstock/codeRunnerThread.py
 ./cardstock/consoleWindow.py
 ./cardstock/controlPanel.py
 ./cardstock/designer.py
+./cardstock/easing.py
 ./cardstock/embeddedImages.py
 ./cardstock/errorListWindow.py
 ./cardstock/findEngineDesigner.py
 ./cardstock/findEngineViewer.py
 ./cardstock/flippedGCDC.py
 ./cardstock/generator.py
 ./cardstock/helpData.py
+./cardstock/helpDataGen.py
 ./cardstock/helpDialogs.py
 ./cardstock/imageFactory.py
 ./cardstock/mediaSearchDialogs.py
 ./cardstock/migrations.py
 ./cardstock/propertyInspector.py
 ./cardstock/pythonEditor.py
 ./cardstock/resourcePathManager.py
```

### Comparing `cardstock-0.99.5/setup.cfg` & `cardstock-0.99.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [metadata]
 name = cardstock
-version = 0.99.5
+version = 0.99.6
 author = Ben Levitt
 author_email = benjie@gmail.com
 description = A simple development and rapid prototyping tool for quickly building multi-platform desktop programs and web apps.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/benjie-git/CardStock/wiki
 classifiers = 
-	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.9
 	License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= .
 packages = find:
 install_requires = 
 	attrdict3
 	wxpython
 	PyInstaller
 	requests
 	simpleaudio
-python_requires = >=3.7,<3.12
+python_requires = >=3.9,<3.12
 
 [options.extras_require]
 mp3 = 
 	streamp3
 
 [options.packages.find]
 where = .
```

