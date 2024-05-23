# Comparing `tmp/pkscreener-0.45.20240522.399.tar.gz` & `tmp/pkscreener-0.45.20240522.400.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240522.399.tar", last modified: Wed May 22 20:05:44 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240522.400.tar", last modified: Wed May 22 21:05:58 2024, max compression
```

## Comparing `pkscreener-0.45.20240522.399.tar` & `pkscreener-0.45.20240522.400.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 20:05:44.779197 pkscreener-0.45.20240522.399/
--rw-rw-rw-   0        0        0     1086 2024-05-22 20:01:54.000000 pkscreener-0.45.20240522.399/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-22 20:01:54.000000 pkscreener-0.45.20240522.399/LICENSE-Others
--rw-rw-rw-   0        0        0    27918 2024-05-22 20:05:44.779197 pkscreener-0.45.20240522.399/PKG-INFO
--rw-rw-rw-   0        0        0    26979 2024-05-22 20:01:54.000000 pkscreener-0.45.20240522.399/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 20:05:44.763570 pkscreener-0.45.20240522.399/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:05:44.779197 pkscreener-0.45.20240522.399/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5641 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34244 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10305 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    13424 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    45614 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24598 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22819 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8313 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   156748 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56838 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    86151 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-22 20:05:36.000000 pkscreener-0.45.20240522.399/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   147505 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1092 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    54014 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    34564 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:05:44.763570 pkscreener-0.45.20240522.399/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27918 2024-05-22 20:05:44.000000 pkscreener-0.45.20240522.399/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-22 20:05:44.000000 pkscreener-0.45.20240522.399/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 20:05:44.000000 pkscreener-0.45.20240522.399/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-22 20:05:44.000000 pkscreener-0.45.20240522.399/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-22 20:05:44.000000 pkscreener-0.45.20240522.399/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-22 20:05:44.000000 pkscreener-0.45.20240522.399/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-22 20:05:44.779197 pkscreener-0.45.20240522.399/setup.cfg
--rw-rw-rw-   0        0        0     5728 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:05:58.911579 pkscreener-0.45.20240522.400/
+-rw-rw-rw-   0        0        0     1086 2024-05-22 21:01:58.000000 pkscreener-0.45.20240522.400/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-22 21:01:58.000000 pkscreener-0.45.20240522.400/LICENSE-Others
+-rw-rw-rw-   0        0        0    27918 2024-05-22 21:05:58.911579 pkscreener-0.45.20240522.400/PKG-INFO
+-rw-rw-rw-   0        0        0    26979 2024-05-22 21:01:58.000000 pkscreener-0.45.20240522.400/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 21:05:58.895960 pkscreener-0.45.20240522.400/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:05:58.911579 pkscreener-0.45.20240522.400/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5641 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34244 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10305 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    13424 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    45614 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24598 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22819 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8313 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   156748 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56838 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    86151 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-22 21:05:51.000000 pkscreener-0.45.20240522.400/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   147505 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1092 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    54496 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    34564 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:05:58.895960 pkscreener-0.45.20240522.400/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27918 2024-05-22 21:05:58.000000 pkscreener-0.45.20240522.400/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-22 21:05:58.000000 pkscreener-0.45.20240522.400/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 21:05:58.000000 pkscreener-0.45.20240522.400/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-22 21:05:58.000000 pkscreener-0.45.20240522.400/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-22 21:05:58.000000 pkscreener-0.45.20240522.400/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-22 21:05:58.000000 pkscreener-0.45.20240522.400/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-22 21:05:58.911579 pkscreener-0.45.20240522.400/setup.cfg
+-rw-rw-rw-   0        0        0     5728 2024-05-22 21:01:59.000000 pkscreener-0.45.20240522.400/setup.py
```

### Comparing `pkscreener-0.45.20240522.399/LICENSE` & `pkscreener-0.45.20240522.400/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/LICENSE-Others` & `pkscreener-0.45.20240522.400/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/PKG-INFO` & `pkscreener-0.45.20240522.400/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240522.399
+Version: 0.45.20240522.400
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240522.399.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240522.400.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.399/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.399/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.399/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240522.399/README.md` & `pkscreener-0.45.20240522.400/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.399/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.399/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.399/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240522.399/pkscreener/__init__.py` & `pkscreener-0.45.20240522.400/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/classes/keys.py` & `pkscreener-0.45.20240522.400/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/courbd.ttf` & `pkscreener-0.45.20240522.400/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/globals.py` & `pkscreener-0.45.20240522.400/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240522.400/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240522.400/pkscreener/pkscreenerbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -989,18 +989,32 @@
         skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
         asList=True,
         renderStyle=MenuRenderStyle.STANDALONE,
     )
     cmdText = ""
     for cmd in cmds:
         cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
+    mns = m0.renderForMenu(asList=True)
+    inlineMenus = []
+    for mnu in mns:
+        if mnu.menuKey[0:2] in TOP_LEVEL_SCANNER_MENUS:
+            inlineMenus.append(
+                InlineKeyboardButton(
+                    mnu.menuText.split("(")[0],
+                    callback_data="C" + str(mnu.menuKey),
+                )
+            )
+    keyboard = [inlineMenus]
+    reply_markup = InlineKeyboardMarkup(keyboard)
+    
     """Send a message when the command /help is issued."""
     if update is not None and update.message is not None:
         await update.message.reply_text(
-            f"You can begin by typing in /start and hit send!\n\nOR\n\nChoose an option:\n{cmdText}"
+            f"You can begin by typing in /start and hit send!\n\nOR\n\nChoose an option:\n{cmdText}",
+            reply_markup=reply_markup
         )  #  \n\nThis bot restarts every hour starting at 5:30am IST until 10:30pm IST to keep it running on free servers. If it does not respond, please try again in a minutes to avoid the restart duration!
         query = update.message
         message = f"Name: <b>{query.from_user.first_name}</b>, Username:@{query.from_user.username} with ID: <b>@{str(query.from_user.id)}</b> began using the bot!"
         await context.bot.send_message(
             chat_id=int(f"-{Channel_Id}"), text=message, parse_mode=ParseMode.HTML
         )
```

### Comparing `pkscreener-0.45.20240522.399/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240522.400/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240522.400/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240522.399
+Version: 0.45.20240522.400
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240522.399.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240522.400.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.399/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.399/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.399/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240522.399/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240522.400/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.399/setup.py` & `pkscreener-0.45.20240522.400/setup.py`

 * *Files identical despite different names*

