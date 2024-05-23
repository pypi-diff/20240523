# Comparing `tmp/BingImageCreator-fork-0.7.6.tar.gz` & `tmp/bingimagecreator_fork-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BingImageCreator-fork-0.7.6.tar", last modified: Fri Jan 12 05:05:15 2024, max compression
+gzip compressed data, was "bingimagecreator_fork-0.8.0.tar", last modified: Thu May 23 14:11:51 2024, max compression
```

## Comparing `BingImageCreator-fork-0.7.6.tar` & `bingimagecreator_fork-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-01-12 05:05:15.881861 BingImageCreator-fork-0.7.6/
--rw-r--r--   0 hyi        (502) staff       (20)     1211 2023-10-22 14:23:52.000000 BingImageCreator-fork-0.7.6/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)     1899 2024-01-12 05:05:15.881425 BingImageCreator-fork-0.7.6/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      935 2023-11-03 11:10:12.000000 BingImageCreator-fork-0.7.6/README.md
--rw-r--r--   0 hyi        (502) staff       (20)      103 2024-01-12 05:05:15.883869 BingImageCreator-fork-0.7.6/setup.cfg
--rw-r--r--   0 hyi        (502) staff       (20)     1248 2024-01-12 05:04:51.000000 BingImageCreator-fork-0.7.6/setup.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-01-12 05:05:15.869192 BingImageCreator-fork-0.7.6/src/
--rw-r--r--   0 hyi        (502) staff       (20)    18398 2024-01-12 05:04:41.000000 BingImageCreator-fork-0.7.6/src/BingImageCreator.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-01-12 05:05:15.878607 BingImageCreator-fork-0.7.6/src/BingImageCreator_fork.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)     1899 2024-01-12 05:05:15.000000 BingImageCreator-fork-0.7.6/src/BingImageCreator_fork.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      325 2024-01-12 05:05:15.000000 BingImageCreator-fork-0.7.6/src/BingImageCreator_fork.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2024-01-12 05:05:15.000000 BingImageCreator-fork-0.7.6/src/BingImageCreator_fork.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       36 2024-01-12 05:05:15.000000 BingImageCreator-fork-0.7.6/src/BingImageCreator_fork.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)       17 2024-01-12 05:05:15.000000 BingImageCreator-fork-0.7.6/src/BingImageCreator_fork.egg-info/top_level.txt
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-01-12 05:05:15.877120 BingImageCreator-fork-0.7.6/test/
--rw-r--r--   0 hyi        (502) staff       (20)      752 2023-10-22 14:23:52.000000 BingImageCreator-fork-0.7.6/test/test_example.py
+drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-23 14:11:51.673313 bingimagecreator_fork-0.8.0/
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)     1211 2024-05-23 10:51:02.000000 bingimagecreator_fork-0.8.0/LICENSE
+-rw-r--r--   0 yihong    (1000) yihong    (1000)     1936 2024-05-23 14:11:51.673313 bingimagecreator_fork-0.8.0/PKG-INFO
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)      935 2024-05-23 10:51:02.000000 bingimagecreator_fork-0.8.0/README.md
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)      103 2024-05-23 14:11:51.673313 bingimagecreator_fork-0.8.0/setup.cfg
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)     1281 2024-05-23 14:11:13.000000 bingimagecreator_fork-0.8.0/setup.py
+drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-23 14:11:51.669314 bingimagecreator_fork-0.8.0/src/
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)    18412 2024-05-23 14:11:28.000000 bingimagecreator_fork-0.8.0/src/BingImageCreator.py
+drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-23 14:11:51.673313 bingimagecreator_fork-0.8.0/src/BingImageCreator_fork.egg-info/
+-rw-r--r--   0 yihong    (1000) yihong    (1000)     1936 2024-05-23 14:11:51.000000 bingimagecreator_fork-0.8.0/src/BingImageCreator_fork.egg-info/PKG-INFO
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)      325 2024-05-23 14:11:51.000000 bingimagecreator_fork-0.8.0/src/BingImageCreator_fork.egg-info/SOURCES.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)        1 2024-05-23 14:11:51.000000 bingimagecreator_fork-0.8.0/src/BingImageCreator_fork.egg-info/dependency_links.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)       46 2024-05-23 14:11:51.000000 bingimagecreator_fork-0.8.0/src/BingImageCreator_fork.egg-info/requires.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)       17 2024-05-23 14:11:51.000000 bingimagecreator_fork-0.8.0/src/BingImageCreator_fork.egg-info/top_level.txt
+drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-05-23 14:11:51.673313 bingimagecreator_fork-0.8.0/test/
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)      752 2024-05-23 10:51:02.000000 bingimagecreator_fork-0.8.0/test/test_example.py
```

### Comparing `BingImageCreator-fork-0.7.6/LICENSE` & `bingimagecreator_fork-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BingImageCreator-fork-0.7.6/PKG-INFO` & `bingimagecreator_fork-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: BingImageCreator-fork
-Version: 0.7.6
+Version: 0.8.0
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/yihong0618/BingImageCreator
-Author: Antonio Cheong
+Author: Antonio Cheong, yihong0618
 Author-email: acheong@student.dalat.org, zouzou0208@gmail.com
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/yihong0618/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: regex
 Requires-Dist: requests
 Requires-Dist: fake-useragent
+Requires-Dist: curl_cffi
 
 # BingImageCreator
 
 High quality image generation by Microsoft. Reverse engineered API.
 Fork from https://github.com/acheong08/BingImageCreator
 
 `pip3 install .`
```

### Comparing `BingImageCreator-fork-0.7.6/README.md` & `bingimagecreator_fork-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `BingImageCreator-fork-0.7.6/setup.py` & `bingimagecreator_fork-0.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import find_packages, setup
 
 setup(
     name="BingImageCreator-fork",
-    version="0.7.6",
+    version="0.8.0",
     license="GNU General Public License v2.0",
-    author="Antonio Cheong",
+    author="Antonio Cheong, yihong0618",
     author_email="acheong@student.dalat.org, zouzou0208@gmail.com",
     description="High quality image generation by Microsoft. Reverse engineered API.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/yihong0618/BingImageCreator",
     project_urls={
         "Bug Report": "https://github.com/yihong0618/BingImageCreator/issues/new",
     },
     install_requires=[
         "httpx",
         "regex",
         "requests",
         "fake-useragent",
+        "curl_cffi",
     ],
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["BingImageCreator"],
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Intended Audience :: Developers",
```

### Comparing `BingImageCreator-fork-0.7.6/src/BingImageCreator.py` & `bingimagecreator_fork-0.8.0/src/BingImageCreator.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 import time
 from functools import partial
 from http.cookies import SimpleCookie
 from typing import Dict, List, Union
 
 import httpx
 import regex
-import requests
+import requests as req
 from fake_useragent import UserAgent
-from requests.utils import cookiejar_from_dict
+
+from curl_cffi import requests
+from curl_cffi.requests import Cookies
 
 ua = UserAgent(browsers=["edge"])
 BING_URL = os.getenv("BING_URL", "https://www.bing.com")
 # Generate random IP between range 13.104.0.0/14
 FORWARDED_IP = (
     f"13.{random.randint(104, 107)}.{random.randint(0, 255)}.{random.randint(0, 255)}"
 )
@@ -45,14 +47,16 @@
 error_bad_images = "Bad images"
 error_no_images = "No images"
 # Action messages
 sending_message = "Sending request..."
 wait_message = "Waiting for results..."
 download_message = "\nDownloading images..."
 
+browser_version = "edge101"
+
 
 def debug(debug_file, text_var):
     """helper function for debug"""
     with open(f"{debug_file}", "a", encoding="utf-8") as f:
         f.write(str(text_var))
         f.write("\n")
 
@@ -87,27 +91,21 @@
             self.debug = partial(debug, self.debug_file)
 
     @staticmethod
     def parse_cookie_string(cookie_string):
         cookie = SimpleCookie()
         cookie.load(cookie_string)
         cookies_dict = {}
-        cookiejar = None
         for key, morsel in cookie.items():
-            if key == "USRLOC":
-                continue
             cookies_dict[key] = morsel.value
-            cookiejar = cookiejar_from_dict(
-                cookies_dict, cookiejar=None, overwrite=True
-            )
-        return cookiejar
+        return Cookies(cookies_dict)
 
     def get_limit_left(self) -> int:
         self.session.headers["user-agent"] = ua.random
-        r = self.session.get("https://www.bing.com/create")
+        r = self.session.get("https://www.bing.com/create", impersonate=browser_version)
         if not r.ok:
             raise Exception("Can not get limit left from this `cookie` please check")
         value = re.search(
             r'<div id="token_bal" aria-label="[0-9]+.*">([0-9]+)</div>', r.text
         )
         if not value:
             return 0
@@ -123,24 +121,25 @@
         Parameters:
             prompt: str
         """
         if not self.quiet:
             print(sending_message)
         if self.debug_file:
             self.debug(sending_message)
-        url_encoded_prompt = requests.utils.quote(prompt)
+        url_encoded_prompt = req.utils.quote(prompt)
         payload = f"q={url_encoded_prompt}&qs=ds"
         # https://www.bing.com/images/create?q=<PROMPT>&rt=3&FORM=GENCRE
         url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=4&FORM=GENCRE"
         self.session.headers["user-agent"] = ua.random
         response = self.session.post(
             url,
             allow_redirects=False,
             data=payload,
             timeout=600,
+            impersonate=browser_version,
         )
         # check for content waring message
         if "this prompt is being reviewed" in response.text.lower():
             if self.debug_file:
                 self.debug(f"ERROR: {error_being_reviewed_prompt}")
             raise Exception(
                 error_being_reviewed_prompt,
@@ -157,15 +156,17 @@
         ):
             if self.debug_file:
                 self.debug(f"ERROR: {error_unsupported_lang}")
             raise Exception(error_unsupported_lang)
         if response.status_code != 302:
             # if rt4 fails, try rt3
             url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=3&FORM=GENCRE"
-            response = self.session.post(url, allow_redirects=False, timeout=600)
+            response = self.session.post(
+                url, allow_redirects=False, timeout=600, impersonate=browser_version
+            )
             if response.status_code != 302:
                 if self.debug_file:
                     self.debug(f"ERROR: {error_redirect}")
                 print(f"ERROR: {response.text}")
                 raise Exception(error_redirect)
         # Get redirect URL
         redirect_url = response.headers["Location"].replace("&nfy=1", "")
@@ -182,15 +183,15 @@
         while True:
             if int(time.time() - start_wait) > 600:
                 if self.debug_file:
                     self.debug(f"ERROR: {error_timeout}")
                 raise Exception(error_timeout)
             if not self.quiet:
                 print(".", end="", flush=True)
-            response = self.session.get(polling_url)
+            response = self.session.get(polling_url, impersonate=browser_version)
             if response.status_code != 200:
                 if self.debug_file:
                     self.debug(f"ERROR: {error_noresults}")
                 raise Exception(error_noresults)
             if not response.text or response.text.find("errorMessage") != -1:
                 time.sleep(1)
                 continue
@@ -246,15 +247,15 @@
                 links = links[:download_count]
 
             for link in links:
                 while os.path.exists(
                     os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg")
                 ):
                     jpeg_index += 1
-                response = self.session.get(link)
+                response = req.get(link)
                 if response.status_code != 200:
                     raise Exception("Could not download image")
                 # save response to file
                 with open(
                     os.path.join(output_dir, f"{fn}{jpeg_index}.jpeg"), "wb"
                 ) as output_file:
                     output_file.write(response.content)
```

### Comparing `BingImageCreator-fork-0.7.6/src/BingImageCreator_fork.egg-info/PKG-INFO` & `bingimagecreator_fork-0.8.0/src/BingImageCreator_fork.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: BingImageCreator-fork
-Version: 0.7.6
+Version: 0.8.0
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/yihong0618/BingImageCreator
-Author: Antonio Cheong
+Author: Antonio Cheong, yihong0618
 Author-email: acheong@student.dalat.org, zouzou0208@gmail.com
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/yihong0618/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: regex
 Requires-Dist: requests
 Requires-Dist: fake-useragent
+Requires-Dist: curl_cffi
 
 # BingImageCreator
 
 High quality image generation by Microsoft. Reverse engineered API.
 Fork from https://github.com/acheong08/BingImageCreator
 
 `pip3 install .`
```

### Comparing `BingImageCreator-fork-0.7.6/test/test_example.py` & `bingimagecreator_fork-0.8.0/test/test_example.py`

 * *Files identical despite different names*

