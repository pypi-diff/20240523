# Comparing `tmp/tinyticker-0.6.3.tar.gz` & `tmp/tinyticker-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.6.3.tar", max compression
+gzip compressed data, was "tinyticker-0.6.4.tar", max compression
```

## Comparing `tinyticker-0.6.3.tar` & `tinyticker-0.6.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1068 2024-05-22 21:05:12.232667 tinyticker-0.6.3/LICENSE
--rw-r--r--   0        0        0     3787 2024-05-22 21:05:12.232667 tinyticker-0.6.3/README.md
--rw-r--r--   0        0        0      917 2024-05-22 21:05:12.236667 tinyticker-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      465 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/__init__.py
--rw-r--r--   0        0        0     5893 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/__main__.py
--rw-r--r--   0        0        0     2496 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/config.py
--rw-r--r--   0        0        0     9000 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/paths.py
--rw-r--r--   0        0        0     4235 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/sequence.py
--rw-r--r--   0        0        0     1112 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/tickers/__init__.py
--rw-r--r--   0        0        0     3618 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/tickers/_base.py
--rw-r--r--   0        0        0     4620 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/tickers/crypto.py
--rw-r--r--   0        0        0     2915 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/tickers/stock.py
--rw-r--r--   0        0        0     2391 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0    21091 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in7.py
--rw-r--r--   0        0        0    19697 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in7_V2.py
--rw-r--r--   0        0        0     1551 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2583 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6750 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/app.py
--rw-r--r--   0        0        0     3021 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    15682 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1904 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     2349 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 tinyticker-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-22 22:44:39.118936 tinyticker-0.6.4/LICENSE
+-rw-r--r--   0        0        0     3787 2024-05-22 22:44:39.118936 tinyticker-0.6.4/README.md
+-rw-r--r--   0        0        0      917 2024-05-22 22:44:39.118936 tinyticker-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      465 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/__init__.py
+-rw-r--r--   0        0        0     6582 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/__main__.py
+-rw-r--r--   0        0        0     2496 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/config.py
+-rw-r--r--   0        0        0     9000 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/paths.py
+-rw-r--r--   0        0        0     4653 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/sequence.py
+-rw-r--r--   0        0        0     1112 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/tickers/__init__.py
+-rw-r--r--   0        0        0     3618 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/tickers/_base.py
+-rw-r--r--   0        0        0     4620 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/tickers/crypto.py
+-rw-r--r--   0        0        0     2915 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/tickers/stock.py
+-rw-r--r--   0        0        0     2391 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0    21091 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in7.py
+-rw-r--r--   0        0        0    19697 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in7_V2.py
+-rw-r--r--   0        0        0     1551 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2583 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6750 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/web/app.py
+-rw-r--r--   0        0        0     3393 2024-05-22 22:44:39.122936 tinyticker-0.6.4/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    15682 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1904 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2349 2024-05-22 22:44:39.126937 tinyticker-0.6.4/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 tinyticker-0.6.4/PKG-INFO
```

### Comparing `tinyticker-0.6.3/LICENSE` & `tinyticker-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/README.md` & `tinyticker-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/pyproject.toml` & `tinyticker-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.6.3"
+version = "0.6.4"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.6.3/tinyticker/__main__.py` & `tinyticker-0.6.4/tinyticker/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,22 @@
 def start_ticker(config_file: Path) -> None:
     """Start ticking.
 
     Args:
         config_file: config file path.
     """
     logger.info("Starting ticker process")
+
+    def skip_current(*_):
+        logger.info("Skip current ticker.")
+        if sequence is not None:
+            sequence._skip_current = True
+
+    signal.signal(signal.SIGUSR1, skip_current)
+
     # Read config values
     tt_config = load_config_safe(config_file)
 
     display = Display.from_tinyticker_config(tt_config)
     sequence = Sequence.from_tinyticker_config(tt_config)
     logger.debug(sequence)
 
@@ -180,15 +188,28 @@
         observer.stop()
         observer.join()
         tick_process.kill()
         tick_process.join()
 
     atexit.register(cleanup)
 
-    # start ticking
+    def skip_ticker(*_):
+        """Skip the current ticker."""
+        logger.info("Sending signal to skip the current ticker.")
+        # forward the signal to the ticker process
+        if (
+            tick_process is not None
+            and tick_process.is_alive()
+            and tick_process.pid is not None
+        ):
+            os.kill(tick_process.pid, signal.SIGUSR1)
+
+    signal.signal(signal.SIGUSR1, skip_ticker)
+
+    # start ticking, we pass the config file so that is can be reloaded on refresh
     tick_process = start_ticker_process(config_file)
     while True:
         if tick_process._closed or not tick_process.is_alive():  # type: ignore
             tick_process = start_ticker_process(config_file)
         else:
             sleep(1)
```

### Comparing `tinyticker-0.6.3/tinyticker/config.py` & `tinyticker-0.6.4/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/display.py` & `tinyticker-0.6.4/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/sequence.py` & `tinyticker-0.6.4/tinyticker/sequence.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,14 +52,15 @@
                 ticker. This typically happens when the stock market closes.
         """
         if len(tickers) == 0:
             raise ValueError("No tickers provided.")
         self.tickers = tickers
         self.skip_empty = skip_empty
         self.skip_outdated = skip_outdated
+        self._skip_current = False
 
     def start(self) -> Iterator[Tuple[TickerBase, TickerResponse]]:
         """Start iterating through the tickers.
 
         Returns:
             The `Ticker` instance and its response.
         """
@@ -83,27 +84,36 @@
                 ):
                     LOGGER.debug(f"{ticker} response empty, skipping.")
                     continue
                 if self.skip_outdated:
                     # we want to skip the ticker if the last candle is too old, but because running
                     # this code takes some time, we relax the min constraint a bit.
                     outdated_min_delta = max(pd.to_timedelta("5m"), ticker.interval_dt)
-                    # when fetching daily data from yfinance, the timestamps are 00:00:00 of the day in question
-                    # which covers the full day's trade from open to close, so we relax the outdated constraint.
+                    # when fetching daily data from yfinance, the timestamps are 00:00:00
+                    # of the day in question which covers the full day's trade from open
+                    # to close, so we relax the outdated constraint.
                     if outdated_min_delta == pd.to_timedelta("1d"):
                         outdated_min_delta *= 2
                     if (
                         (utils.now() - response.historical.index[-1])  # type: ignore
                         > outdated_min_delta
                     ):
                         LOGGER.debug(f"{ticker} response outdated, skipping.")
                         continue
                 all_skipped = False
                 yield (ticker, response)
+
                 LOGGER.info(f"Sleeping {ticker.wait_time}s.")
-                time.sleep(ticker.wait_time)
+                # we want to sleep for the ticker's wait time and check every second if we
+                # should skip the next ticker.
+                for _ in range(ticker.wait_time):
+                    if self._skip_current:
+                        LOGGER.info(f"Skipping {ticker}.")
+                        self._skip_current = False
+                        break
+                    time.sleep(1)
 
     def __str__(self):
         return (
             f"Sequence(skip_outdated={self.skip_outdated}, skip_empty={self.skip_empty}): \n"
             + "\n".join([ticker.__str__() for ticker in self.tickers])
         )
```

### Comparing `tinyticker-0.6.3/tinyticker/tickers/__init__.py` & `tinyticker-0.6.4/tinyticker/tickers/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/tickers/_base.py` & `tinyticker-0.6.4/tinyticker/tickers/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/tickers/crypto.py` & `tinyticker-0.6.4/tinyticker/tickers/crypto.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/tickers/stock.py` & `tinyticker-0.6.4/tinyticker/tickers/stock.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/utils.py` & `tinyticker-0.6.4/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.6.4/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/waveshare_lib/device.py` & `tinyticker-0.6.4/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in7.py` & `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in7.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in7_V2.py` & `tinyticker-0.6.4/tinyticker/waveshare_lib/epd2in7_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/waveshare_lib/models.py` & `tinyticker-0.6.4/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/web/__main__.py` & `tinyticker-0.6.4/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/web/app.py` & `tinyticker-0.6.4/tinyticker/web/app.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/web/command.py` & `tinyticker-0.6.4/tinyticker/web/command.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,14 +53,26 @@
     """Restart the tinyticker and tinyticker-web systemd services."""
     LOGGER.info("Restarting services.")
     try_command("systemctl --user restart tinyticker")
     try_command("systemctl --user restart tinyticker-web")
 
 
 @register
+def skip_current() -> None:
+    """Skip over the current ticker and display the next on."""
+    if PID_FILE.is_file():
+        LOGGER.info("Sending SIGUSR2 to tinyticker.")
+        with open(PID_FILE, "r") as pid_file:
+            pid = int(pid_file.readline())
+        os.kill(pid, signal.SIGUSR1)
+    else:
+        LOGGER.info("tinyticker is not runnning.")
+
+
+@register
 def refresh() -> None:
     """Refresh tinyticker's ticker process."""
     if PID_FILE.is_file():
         LOGGER.info("Sending SIGUSR2 to tinyticker.")
         with open(PID_FILE, "r") as pid_file:
             pid = int(pid_file.readline())
         os.kill(pid, signal.SIGUSR2)
```

### Comparing `tinyticker-0.6.3/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.6.4/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.6.4/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.6.4/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.6.4/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/web/templates/index.html` & `tinyticker-0.6.4/tinyticker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/web/templates/js/index.js` & `tinyticker-0.6.4/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.6.4/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.6.4/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/tinyticker/web/templates/logfiles.html` & `tinyticker-0.6.4/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.3/PKG-INFO` & `tinyticker-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.6.3
+Version: 0.6.4
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.6.3 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.6.4 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

