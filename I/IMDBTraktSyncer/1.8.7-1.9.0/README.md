# Comparing `tmp/IMDBTraktSyncer-1.8.7.tar.gz` & `tmp/imdbtraktsyncer-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.8.7.tar", last modified: Fri Dec  8 04:17:27 2023, max compression
+gzip compressed data, was "imdbtraktsyncer-1.9.0.tar", last modified: Thu May 23 12:11:47 2024, max compression
```

## Comparing `IMDBTraktSyncer-1.8.7.tar` & `imdbtraktsyncer-1.9.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-12-08 04:17:27.717341 IMDBTraktSyncer-1.8.7/
-drwxrwxrwx   0        0        0        0 2023-12-08 04:17:27.683356 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    41809 2023-12-08 04:11:06.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     6398 2023-11-09 08:08:16.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4274 2023-08-08 21:16:45.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     6946 2023-08-02 06:46:34.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1669 2023-11-28 23:00:15.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0    11546 2023-08-02 05:50:14.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10587 2023-10-13 00:03:11.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    13226 2023-11-09 06:40:06.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-12-08 04:17:27.714350 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12838 2023-12-08 04:17:27.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-12-08 04:17:27.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-08 04:17:27.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-12-08 04:17:27.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-12-08 04:17:27.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-12-08 04:17:27.000000 IMDBTraktSyncer-1.8.7/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.8.7/LICENSE
--rw-rw-rw-   0        0        0    12838 2023-12-08 04:17:27.715341 IMDBTraktSyncer-1.8.7/PKG-INFO
--rw-rw-rw-   0        0        0    11988 2023-12-04 01:46:57.000000 IMDBTraktSyncer-1.8.7/README.md
--rw-rw-rw-   0        0        0       42 2023-12-08 04:17:27.717341 IMDBTraktSyncer-1.8.7/setup.cfg
--rw-rw-rw-   0        0        0     1390 2023-12-08 04:14:16.000000 IMDBTraktSyncer-1.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:47.079138 imdbtraktsyncer-1.9.0/
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:47.054137 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    42098 2024-05-23 11:42:40.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     6398 2023-11-09 08:08:16.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4274 2023-08-08 21:16:45.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     1952 2024-05-23 11:35:10.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/checkVersion.py
+-rw-rw-rw-   0        0        0     6946 2023-08-02 06:46:34.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2024-05-19 13:42:35.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0    15966 2024-05-23 11:15:28.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10587 2023-10-13 00:03:11.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    13298 2024-05-23 11:30:12.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:47.076138 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12838 2024-05-23 12:11:46.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2024-05-23 12:11:46.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 12:11:46.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-23 12:11:46.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-05-23 12:11:46.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 12:11:46.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 imdbtraktsyncer-1.9.0/LICENSE
+-rw-rw-rw-   0        0        0    12838 2024-05-23 12:11:47.077137 imdbtraktsyncer-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11988 2024-05-23 12:10:15.000000 imdbtraktsyncer-1.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 12:11:47.079138 imdbtraktsyncer-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1390 2024-05-23 11:47:49.000000 imdbtraktsyncer-1.9.0/setup.py
```

### Comparing `IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/IMDBTraktSyncer.py` & `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,59 @@
-import os
-import json
-import requests
-import time
-from datetime import datetime, timezone, timedelta
-from selenium import webdriver
-from selenium.webdriver.chrome.service import Service
-from selenium.webdriver.common.by import By
-from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.support.ui import WebDriverWait
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.common.exceptions import SessionNotCreatedException
-try:
-    from IMDBTraktSyncer import checkChromedriver
-    from IMDBTraktSyncer import verifyCredentials as VC
-    from IMDBTraktSyncer import traktData
-    from IMDBTraktSyncer import imdbData
-    from IMDBTraktSyncer import errorHandling as EH
-    from IMDBTraktSyncer import errorLogger as EL
-except ImportError:
-    import checkChromedriver
-    import verifyCredentials as VC
-    import traktData
-    import imdbData
-    import errorHandling as EH
-    import errorLogger as EL
-from chromedriver_py import binary_path
+def main():
+    print("Starting IMDBTraktSyncer....")
+    import os
+    import json
+    import requests
+    import time
+    from datetime import datetime, timezone, timedelta
+    from selenium import webdriver
+    from selenium.webdriver.chrome.service import Service
+    from selenium.webdriver.common.by import By
+    from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
+    from selenium.webdriver.chrome.options import Options
+    from selenium.webdriver.support.ui import WebDriverWait
+    from selenium.webdriver.support import expected_conditions as EC
+    from selenium.common.exceptions import SessionNotCreatedException
 
-class PageLoadException(Exception):
-    pass
+    try:
+        from IMDBTraktSyncer import checkVersion
+        from IMDBTraktSyncer import checkChromedriver
+        from IMDBTraktSyncer import verifyCredentials as VC
+        from IMDBTraktSyncer import traktData
+        from IMDBTraktSyncer import imdbData
+        from IMDBTraktSyncer import errorHandling as EH
+        from IMDBTraktSyncer import errorLogger as EL
+    except ImportError:
+        import checkVersion
+        import checkChromedriver
+        import verifyCredentials as VC
+        import traktData
+        import imdbData
+        import errorHandling as EH
+        import errorLogger as EL
+    from chromedriver_py import binary_path
 
-def main():
+    class PageLoadException(Exception):
+        pass
+        
     try:
 
         #Get credentials
         imdb_username = VC.imdb_username
         imdb_password = VC.imdb_password
         
         directory = os.path.dirname(os.path.realpath(__file__))
                 
         #Start web driver
         print('Starting webdriver...')
         options = Options()
         options.add_argument("--headless=new")
         options.add_argument('--user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3')
         options.add_experimental_option("prefs", {"download.default_directory": directory, "download.directory_upgrade": True, "download.prompt_for_download": False, "credentials_enable_service": False, "profile.password_manager_enabled": False})
-        options.add_argument('--window-size=1920,1080')
+        options.add_argument('--start-maximized')
         options.add_argument("--disable-save-password-bubble")
         options.add_argument("--disable-infobars")
         options.add_argument("--disable-autofill-for-password-fields")
         options.add_argument('--disable-notifications')
         options.add_argument("--disable-third-party-cookies")
         options.add_argument("--disable-dev-shm-usage")
         options.add_argument("--no-sandbox")
@@ -699,14 +703,15 @@
                 print('No Watched Items To Remove From IMDB Watchlist')
         
         #Close web driver
         print("Closing webdriver...")
         driver.close()
         driver.quit()
         service.stop()
+        print("IMDBTraktSyncer Complete")
     
     except Exception as e:
         error_message = "An error occurred while running the script."
         EH.report_error(error_message)
         EL.logger.error(error_message, exc_info=True)
         
         # Close the driver and stop the service if they were initialized
```

### Comparing `IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/authTrakt.py` & `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/checkChromedriver.py` & `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/errorHandling.py` & `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/errorLogger.py` & `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/imdbData.py` & `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/imdbData.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,35 +22,110 @@
 class PageLoadException(Exception):
     pass
 
 def getImdbData(imdb_username, imdb_password, driver, directory, wait):
     # Process IMDB Ratings Reviews & Watchlist
     print('Processing IMDB Data')
     
+    
+    # Generate watchlist export
+    success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/list/watchlist', driver, wait)
+    if not success:
+        # Page failed to load, raise an exception
+        raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
+
+    export_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "div[data-testid*='hero-list-subnav-export-button'] button")))
+    export_button.click()
+    time.sleep(3)
+    
+    # Generate ratings export
+    success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/list/ratings', driver, wait)
+    if not success:
+        # Page failed to load, raise an exception
+        raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
+
+    export_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "div[data-testid*='hero-list-subnav-export-button'] button")))
+    export_button.click()
+    time.sleep(3)
+    
+    # Wait for export processing to finish
+    # Function to check if any summary item contains "in progress"
+    def check_in_progress(summary_items):
+        for item in summary_items:
+            if "in progress" in item.text.lower():
+                return True
+        return False
+    # Maximum time to wait in seconds
+    max_wait_time = 1200
+    start_time = time.time()
+
+    while time.time() - start_time < max_wait_time:
+        # Wait for export processing to finish
+        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/exports/', driver, wait)
+        if not success:
+            # Page failed to load, raise an exception
+            raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
+        
+        # Locate all elements with the selector
+        summary_items = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".ipc-metadata-list-summary-item")))
+
+        # Check if any summary item contains "in progress"
+        if not check_in_progress(summary_items):
+            #print("No 'in progress' found. Proceeding.")
+            break
+        else:
+            #print("'In progress' found. Waiting for 30 seconds before retrying.")
+            time.sleep(30)
+    else:
+        raise TimeoutError("IMDB data processing did not complete within the allotted 20 minutes.")
+    
     #Get IMDB Watchlist Items
     try:
         # Load page
-        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/list/watchlist', driver, wait)
+        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/exports/', driver, wait)
         if not success:
             # Page failed to load, raise an exception
             raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
 
-        csv_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".export a")))
-        driver.execute_script("arguments[0].scrollIntoView(true);", csv_link)
-        csv_link.click()
+        # Locate all elements with the selector
+        summary_items = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".ipc-metadata-list-summary-item")))
+
+        # Iterate through the located elements to find the one containing the text "watchlist"
+        csv_link = None
+        for item in summary_items:
+            if "watchlist" in item.text.lower():
+                # Try to find the button inside this item
+                button = item.find_element(By.CSS_SELECTOR, "button[data-testid*='export-status-button']")
+                if button:
+                    csv_link = button
+                    break
+
+        # Check if the csv_link was found and then perform the actions
+        if csv_link:
+            driver.execute_script("arguments[0].scrollIntoView(true);", csv_link)
+            csv_link.click()
+        else:
+            print("Unable to fetch IMDB watchlist data.")
 
         #Wait for csv download to complete
         time.sleep(8)
 
         imdb_watchlist = []
 
-        # Read the watchlist items from the CSV file
         here = os.path.abspath(os.path.dirname(__file__))
-        watchlist_path = os.path.join(here, 'WATCHLIST.csv')
+        here = directory
+        
         try:
+            # Find any CSV file in the directory
+            csv_files = [f for f in os.listdir(directory) if f.endswith('.csv')]
+            if not csv_files:
+                raise FileNotFoundError("Watchlist data not found. No CSV files found in the directory")
+            
+            # Use the first CSV file found 
+            watchlist_path = os.path.join(directory, csv_files[0])
             with open(watchlist_path, 'r', encoding='utf-8') as file:
                 reader = csv.reader(file)
                 header = next(reader)  # skip the header row
                 for row in reader:
                     title = row[5]
                     year = row[10]
                     imdb_id = row[1]
@@ -62,52 +137,72 @@
                     elif "tvEpisode" in row[7]:
                         media_type = "episode"
                     elif "movie" in row[7] or "tvSpecial" in row[7] or "tvMovie" in row[7] or "tvShort" in row[7] or "video" in row[7]:
                         media_type = "movie"
                     else:
                         media_type = "unknown"
                     imdb_watchlist.append({'Title': title, 'Year': year, 'IMDB_ID': imdb_id, 'Date_Added': date_added, 'Type': media_type})
-        except FileNotFoundError:
-            error_message = "Ratings file not found"
-            print(f"{error_message}")
+        except FileNotFoundError as e:
+            print(f"Error: {error_message}", exc_info=True)
             EL.logger.error(error_message, exc_info=True)
-            
+
         # Delete csv files
         for file in os.listdir(directory):
-            if file.endswith('.csv') and 'WATCHLIST' in file:
+            if file.endswith('.csv'):
                 os.remove(os.path.join(directory, file))
 
     except (NoSuchElementException, TimeoutException):
         # No IMDB Watchlist Items
         imdb_watchlist = []
         pass
     
     # Get IMDB Ratings
     try:
         # Load page
-        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/list/ratings', driver, wait)
+        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/exports/', driver, wait)
         if not success:
             # Page failed to load, raise an exception
             raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
-
-        dropdown = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, ".circle")))
-        dropdown.click()
-
-        csv_link = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, ".pop-up-menu-list-items a.pop-up-menu-list-item-link")))
-        csv_link.click()
+        
+        # Locate all elements with the selector
+        summary_items = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".ipc-metadata-list-summary-item")))
+
+        # Iterate through the located elements to find the one containing the text "ratings"
+        csv_link = None
+        for item in summary_items:
+            if "ratings" in item.text.lower():
+                # Try to find the button inside this item
+                button = item.find_element(By.CSS_SELECTOR, "button[data-testid*='export-status-button']")
+                if button:
+                    csv_link = button
+                    break
+
+        # Check if the csv_link was found and then perform the actions
+        if csv_link:
+            driver.execute_script("arguments[0].scrollIntoView(true);", csv_link)
+            csv_link.click()
+        else:
+            print("Unable to fetch IMDB ratings data.")
 
         #Wait for csv download to complete
         time.sleep(8)
 
         imdb_ratings = []
 
-        # Read the ratings from the CSV file
         here = os.path.abspath(os.path.dirname(__file__))
-        ratings_path = os.path.join(here, 'ratings.csv')
+        directory = here
+
         try:
+            # Find any CSV file in the directory
+            csv_files = [f for f in os.listdir(directory) if f.endswith('.csv')]
+            if not csv_files:
+                raise FileNotFoundError("Ratings data not found. No CSV files found in the directory")
+                
+            # Use the first CSV file found 
+            ratings_path = os.path.join(directory, csv_files[0])
             with open(ratings_path, 'r', encoding='utf-8') as file:
                 reader = csv.reader(file)
                 header = next(reader)  # skip the header row
                 for row in reader:
                     title = row[3]
                     year = row[8]
                     rating = row[1]
@@ -121,20 +216,22 @@
                         media_type = "episode"
                     elif "movie" in row[5] or "tvSpecial" in row[5] or "tvMovie" in row[5] or "tvShort" in row[5] or "video" in row[5]:
                         media_type = "movie"
                     else:
                         media_type = "unknown"
                     imdb_ratings.append({'Title': title, 'Year': year, 'Rating': int(rating), 'IMDB_ID': imdb_id, 'Date_Added': date_added, 'Type': media_type})
         except FileNotFoundError:
-            print('Ratings file not found')
+            print(f"Error: {error_message}", exc_info=True)
+            EL.logger.error(error_message, exc_info=True)
             
         # Delete csv files
         for file in os.listdir(directory):
-            if file.endswith('.csv') and 'ratings' in file:
+            if file.endswith('.csv'):
                 os.remove(os.path.join(directory, file))
+
     except (NoSuchElementException, TimeoutException):
         # No IMDB Ratings
         imdb_ratings = []
         error_message = "No IMDB Ratings"
         EL.logger.error(error_message, exc_info=True)
         pass
```

### Comparing `IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/traktData.py` & `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.8.7/IMDBTraktSyncer/verifyCredentials.py` & `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/verifyCredentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     import authTrakt
     import errorLogger as EL
 
 def prompt_get_credentials():
     # Define the file path
     here = os.path.abspath(os.path.dirname(__file__))
     file_path = os.path.join(here, 'credentials.txt')
+    print(f"Your credentials and error log files are saved at:\n{here}")
     
     default_values = {
         "trakt_client_id": "empty",
         "trakt_client_secret": "empty",
         "trakt_access_token": "empty",
         "trakt_refresh_token": "empty",
         "imdb_username": "empty",
@@ -236,16 +237,16 @@
     except FileNotFoundError:
         error_message = "File not found error"
         EL.logger.error(error_message, exc_info=True)
         pass
 
     while True:
         # Prompt the user for input
-        print("Please note: comments synced to IMDB will use \"My Review\" as the title field.")
-        print("Do you want to sync comments? (y/n)")
+        print("Please note: reviews synced to IMDB will use \"My Review\" as the title field.")
+        print("Do you want to sync reviews? (y/n)")
         user_input = input("Enter your choice: ")
 
         # Validate user input
         if user_input.lower() == 'y':
             sync_reviews_value = True
             break
         elif user_input.lower() == 'n':
```

### Comparing `IMDBTraktSyncer-1.8.7/IMDBTraktSyncer.egg-info/PKG-INFO` & `imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.8.7
+Version: 1.9.0
 Summary: A python script that syncs user watchlist, ratings and reviews for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -70,17 +70,17 @@
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook
-- If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step once or twice if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
-- If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
+- If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step several times if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
+- If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - Due to IMDB's lack of API and rating import ability, this script uses an unconventional method that mimics using a web browser to set ratings on IMDB. Therefore, there are many points of failure that could arise. The script will be updated as best as possible.
 
 ## Screenshot
 ![Demo](https://i.imgur.com/QXCtGrr.png)
 
 ## Sponsorships, Donations, and Custom Projects
 If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
```

### Comparing `IMDBTraktSyncer-1.8.7/IMDBTraktSyncer.egg-info/SOURCES.txt` & `imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 IMDBTraktSyncer/IMDBTraktSyncer.py
 IMDBTraktSyncer/__init__.py
 IMDBTraktSyncer/authTrakt.py
 IMDBTraktSyncer/checkChromedriver.py
+IMDBTraktSyncer/checkVersion.py
 IMDBTraktSyncer/errorHandling.py
 IMDBTraktSyncer/errorLogger.py
 IMDBTraktSyncer/imdbData.py
 IMDBTraktSyncer/traktData.py
 IMDBTraktSyncer/verifyCredentials.py
 IMDBTraktSyncer.egg-info/PKG-INFO
 IMDBTraktSyncer.egg-info/SOURCES.txt
```

### Comparing `IMDBTraktSyncer-1.8.7/LICENSE` & `imdbtraktsyncer-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.8.7/PKG-INFO` & `imdbtraktsyncer-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.8.7
+Version: 1.9.0
 Summary: A python script that syncs user watchlist, ratings and reviews for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -70,17 +70,17 @@
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook
-- If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step once or twice if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
-- If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
+- If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step several times if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
+- If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - Due to IMDB's lack of API and rating import ability, this script uses an unconventional method that mimics using a web browser to set ratings on IMDB. Therefore, there are many points of failure that could arise. The script will be updated as best as possible.
 
 ## Screenshot
 ![Demo](https://i.imgur.com/QXCtGrr.png)
 
 ## Sponsorships, Donations, and Custom Projects
 If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
```

### Comparing `IMDBTraktSyncer-1.8.7/README.md` & `imdbtraktsyncer-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook
-- If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step once or twice if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
-- If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
+- If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step several times if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
+- If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - Due to IMDB's lack of API and rating import ability, this script uses an unconventional method that mimics using a web browser to set ratings on IMDB. Therefore, there are many points of failure that could arise. The script will be updated as best as possible.
 
 ## Screenshot
 ![Demo](https://i.imgur.com/QXCtGrr.png)
 
 ## Sponsorships, Donations, and Custom Projects
 If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
```

### Comparing `IMDBTraktSyncer-1.8.7/setup.py` & `imdbtraktsyncer-1.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.8.7'
+VERSION = '1.9.0'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and reviews for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

