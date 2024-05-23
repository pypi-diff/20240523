# Comparing `tmp/pyTelegramWalletApi-0.2.3.tar.gz` & `tmp/pyTelegramWalletApi-0.2.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTelegramWalletApi-0.2.3.tar", last modified: Mon May 20 02:14:37 2024, max compression
+gzip compressed data, was "pyTelegramWalletApi-0.2.31.tar", last modified: Thu May 23 16:31:08 2024, max compression
```

## Comparing `pyTelegramWalletApi-0.2.3.tar` & `pyTelegramWalletApi-0.2.31.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 02:14:37.089371 pyTelegramWalletApi-0.2.3/
--rw-rw-rw-   0        0        0     4828 2024-05-20 02:14:37.089371 pyTelegramWalletApi-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4620 2024-05-20 02:11:16.000000 pyTelegramWalletApi-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 02:14:36.996367 pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/
--rw-rw-rw-   0        0        0     4828 2024-05-20 02:14:36.000000 pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2024-05-20 02:14:36.000000 pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 02:14:36.000000 pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-20 02:14:36.000000 pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-20 02:14:36.000000 pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 02:14:37.099372 pyTelegramWalletApi-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      571 2024-05-20 00:11:57.000000 pyTelegramWalletApi-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 02:14:37.041369 pyTelegramWalletApi-0.2.3/tests/
--rw-rw-rw-   0        0        0        0 2023-10-02 22:55:55.000000 pyTelegramWalletApi-0.2.3/tests/__init__.py
--rw-rw-rw-   0        0        0      902 2024-05-20 00:04:34.000000 pyTelegramWalletApi-0.2.3/tests/test_account.py
--rw-rw-rw-   0        0        0     2680 2024-05-20 00:04:34.000000 pyTelegramWalletApi-0.2.3/tests/test_p2p.py
--rw-rw-rw-   0        0        0      733 2024-05-20 00:05:20.000000 pyTelegramWalletApi-0.2.3/tests/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 02:14:37.048369 pyTelegramWalletApi-0.2.3/wallet/
--rw-rw-rw-   0        0        0       70 2023-10-02 23:59:27.000000 pyTelegramWalletApi-0.2.3/wallet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 02:14:37.052369 pyTelegramWalletApi-0.2.3/wallet/rest/
--rw-rw-rw-   0        0        0    18205 2024-05-20 02:07:30.000000 pyTelegramWalletApi-0.2.3/wallet/rest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 02:14:37.086371 pyTelegramWalletApi-0.2.3/wallet/types/
--rw-rw-rw-   0        0        0      184 2024-05-19 04:12:35.000000 pyTelegramWalletApi-0.2.3/wallet/types/__init__.py
--rw-rw-rw-   0        0        0      975 2024-05-18 18:26:30.000000 pyTelegramWalletApi-0.2.3/wallet/types/balances.py
--rw-rw-rw-   0        0        0     4987 2024-05-19 20:06:10.000000 pyTelegramWalletApi-0.2.3/wallet/types/offers.py
--rw-rw-rw-   0        0        0     3128 2024-05-18 23:18:10.000000 pyTelegramWalletApi-0.2.3/wallet/types/transactions.py
--rw-rw-rw-   0        0        0     4201 2024-05-19 19:38:34.000000 pyTelegramWalletApi-0.2.3/wallet/web_client.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:31:08.462126 pyTelegramWalletApi-0.2.31/
+-rw-rw-rw-   0        0        0     4829 2024-05-23 16:31:08.462126 pyTelegramWalletApi-0.2.31/PKG-INFO
+-rw-rw-rw-   0        0        0     4620 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 16:31:08.422129 pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/
+-rw-rw-rw-   0        0        0     4829 2024-05-23 16:31:08.000000 pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2024-05-23 16:31:08.000000 pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:31:08.000000 pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-23 16:31:08.000000 pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-23 16:31:08.000000 pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 16:31:08.465128 pyTelegramWalletApi-0.2.31/setup.cfg
+-rw-rw-rw-   0        0        0      572 2024-05-23 16:29:37.000000 pyTelegramWalletApi-0.2.31/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:31:08.434130 pyTelegramWalletApi-0.2.31/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-02 22:55:55.000000 pyTelegramWalletApi-0.2.31/tests/__init__.py
+-rw-rw-rw-   0        0        0      902 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/tests/test_account.py
+-rw-rw-rw-   0        0        0     2680 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/tests/test_p2p.py
+-rw-rw-rw-   0        0        0      733 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/tests/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:31:08.439128 pyTelegramWalletApi-0.2.31/wallet/
+-rw-rw-rw-   0        0        0       70 2023-10-02 23:59:27.000000 pyTelegramWalletApi-0.2.31/wallet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:31:08.442127 pyTelegramWalletApi-0.2.31/wallet/rest/
+-rw-rw-rw-   0        0        0    18205 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/wallet/rest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:31:08.458127 pyTelegramWalletApi-0.2.31/wallet/types/
+-rw-rw-rw-   0        0        0      184 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/wallet/types/__init__.py
+-rw-rw-rw-   0        0        0      975 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/wallet/types/balances.py
+-rw-rw-rw-   0        0        0     4987 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/wallet/types/offers.py
+-rw-rw-rw-   0        0        0     3128 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/wallet/types/transactions.py
+-rw-rw-rw-   0        0        0     4530 2024-05-23 16:26:30.000000 pyTelegramWalletApi-0.2.31/wallet/web_client.py
```

### Comparing `pyTelegramWalletApi-0.2.3/PKG-INFO` & `pyTelegramWalletApi-0.2.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTelegramWalletApi
-Version: 0.2.3
+Version: 0.2.31
 Summary: Telegram Wallet API
 Author: no-name-user-name
 Author-email: dimazver61@gmail.com
 Description-Content-Type: text/markdown
 
 <br/>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyTelegramWalletApi Version: 0.2.3 Summary:
+Metadata-Version: 2.1 Name: pyTelegramWalletApi Version: 0.2.31 Summary:
 Telegram Wallet API Author: no-name-user-name Author-email:
 dimazver61@gmail.com Description-Content-Type: text/markdown
                                     _[_L_o_g_o_]
                          ******** TTeelleeggrraamm WWaalllleett AAPPII ********
          Unofficial library for managing your personal Wallet account
 
 ## Table Of Contents * [About the Project](#about-the-project) * [Built With]
```

### Comparing `pyTelegramWalletApi-0.2.3/README.md` & `pyTelegramWalletApi-0.2.31/README.md`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.3/pyTelegramWalletApi.egg-info/PKG-INFO` & `pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTelegramWalletApi
-Version: 0.2.3
+Version: 0.2.31
 Summary: Telegram Wallet API
 Author: no-name-user-name
 Author-email: dimazver61@gmail.com
 Description-Content-Type: text/markdown
 
 <br/>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyTelegramWalletApi Version: 0.2.3 Summary:
+Metadata-Version: 2.1 Name: pyTelegramWalletApi Version: 0.2.31 Summary:
 Telegram Wallet API Author: no-name-user-name Author-email:
 dimazver61@gmail.com Description-Content-Type: text/markdown
                                     _[_L_o_g_o_]
                          ******** TTeelleeggrraamm WWaalllleett AAPPII ********
          Unofficial library for managing your personal Wallet account
 
 ## Table Of Contents * [About the Project](#about-the-project) * [Built With]
```

### Comparing `pyTelegramWalletApi-0.2.3/tests/test_account.py` & `pyTelegramWalletApi-0.2.31/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.3/tests/test_p2p.py` & `pyTelegramWalletApi-0.2.31/tests/test_p2p.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.3/tests/utils.py` & `pyTelegramWalletApi-0.2.31/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.3/wallet/rest/__init__.py` & `pyTelegramWalletApi-0.2.31/wallet/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.3/wallet/types/balances.py` & `pyTelegramWalletApi-0.2.31/wallet/types/balances.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.3/wallet/types/offers.py` & `pyTelegramWalletApi-0.2.31/wallet/types/offers.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.3/wallet/types/transactions.py` & `pyTelegramWalletApi-0.2.31/wallet/types/transactions.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.3/wallet/web_client.py` & `pyTelegramWalletApi-0.2.31/wallet/web_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,21 +40,35 @@
 
         self.driver = webdriver.Chrome(chrome_options=options)
         self.driver.implicitly_wait(7)
 
     @classmethod
     def auth(cls, profile, temp_dir_path=None):
         c = Client(headless=False, profile=profile, temp_dir_path=temp_dir_path)
+        start_page = "https://web.telegram.org/a/#1985737506"
+        c.driver.get(start_page)
         print("Connect Telegram Account")
 
-        while True:
-            if c.driver.current_url == 'https://web.telegram.org/k/#1985737506':
-                return c
-            else:
-                time.sleep(1)
+        try:
+            WebDriverWait(c.driver, 5).until(
+                EC.presence_of_element_located((By.ID, 'auth-qr-form'))
+            )
+            print('Auth by QR')
+
+            while True:
+                if c.driver.current_url == start_page:
+                    return c
+                else:
+                    time.sleep(1)
+
+        except Exception as e:
+            pass
+
+
+
 
     def _parse_token(self, wallet_endpoint):
         try:
             iframe = WebDriverWait(self.driver, 10).until(
                 EC.presence_of_element_located((By.TAG_NAME, 'iframe'))
             )
         except Exception as e:
```

