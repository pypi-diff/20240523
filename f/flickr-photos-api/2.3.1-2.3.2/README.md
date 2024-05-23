# Comparing `tmp/flickr_photos_api-2.3.1.tar.gz` & `tmp/flickr_photos_api-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flickr_photos_api-2.3.1.tar", last modified: Tue May 21 08:21:04 2024, max compression
+gzip compressed data, was "flickr_photos_api-2.3.2.tar", last modified: Thu May 23 09:42:54 2024, max compression
```

## Comparing `flickr_photos_api-2.3.1.tar` & `flickr_photos_api-2.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.899435 flickr_photos_api-2.3.1/
--rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.3.1/LICENSE-APACHE
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.3.1/LICENSE-MIT
--rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-21 08:21:04.899246 flickr_photos_api-2.3.1/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 12:06:13.000000 flickr_photos_api-2.3.1/README.md
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 14:50:54.000000 flickr_photos_api-2.3.1/pyproject.toml
--rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-05-21 08:21:04.899476 flickr_photos_api-2.3.1/setup.cfg
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.891410 flickr_photos_api-2.3.1/src/
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.892957 flickr_photos_api-2.3.1/src/flickr_photos_api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1378 2024-05-21 08:20:14.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/__init__.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.898109 flickr_photos_api-2.3.1/src/flickr_photos_api/api/
--rw-r--r--   0 alexwlchan   (501) staff       (20)      640 2024-05-01 09:51:49.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/__init__.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5822 2024-05-21 08:19:52.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/base.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    13443 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/collection_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2174 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/comment_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1862 2024-05-01 09:51:49.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/commons_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     2234 2024-04-30 14:50:54.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/from_url_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 12:06:13.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/license_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)    14939 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/single_photo_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     8514 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/api/user_methods.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1836 2024-05-01 12:03:23.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/exceptions.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/py.typed
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.898514 flickr_photos_api-2.3.1/src/flickr_photos_api/types/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     3016 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/types/__init__.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      767 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/types/contexts.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     1063 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/types/users.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.3.1/src/flickr_photos_api/utils.py
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.899039 flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-21 08:21:04.000000 flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/PKG-INFO
--rw-r--r--   0 alexwlchan   (501) staff       (20)      958 2024-05-21 08:21:04.000000 flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/SOURCES.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-05-21 08:21:04.000000 flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/dependency_links.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-05-21 08:21:04.000000 flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/requires.txt
--rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-05-21 08:21:04.000000 flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/top_level.txt
-drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-21 08:21:04.898757 flickr_photos_api-2.3.1/tests/
--rw-r--r--   0 alexwlchan   (501) staff       (20)     7788 2024-05-21 08:17:56.000000 flickr_photos_api-2.3.1/tests/test_errors.py
--rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.3.1/tests/test_utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-23 09:42:54.670489 flickr_photos_api-2.3.2/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    11356 2023-11-05 12:32:45.000000 flickr_photos_api-2.3.2/LICENSE-APACHE
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1074 2023-11-05 12:32:47.000000 flickr_photos_api-2.3.2/LICENSE-MIT
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-23 09:42:54.670275 flickr_photos_api-2.3.2/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3172 2024-04-30 12:06:13.000000 flickr_photos_api-2.3.2/README.md
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1856 2024-04-30 14:50:54.000000 flickr_photos_api-2.3.2/pyproject.toml
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       38 2024-05-23 09:42:54.670557 flickr_photos_api-2.3.2/setup.cfg
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-23 09:42:54.664166 flickr_photos_api-2.3.2/src/
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-23 09:42:54.666291 flickr_photos_api-2.3.2/src/flickr_photos_api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1378 2024-05-23 09:42:50.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/__init__.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-23 09:42:54.669045 flickr_photos_api-2.3.2/src/flickr_photos_api/api/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      640 2024-05-01 09:51:49.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/api/__init__.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     6173 2024-05-23 09:42:50.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/api/base.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    13443 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/api/collection_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2174 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/api/comment_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1862 2024-05-01 09:51:49.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/api/commons_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     2234 2024-04-30 14:50:54.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/api/from_url_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3052 2024-04-30 12:06:13.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/api/license_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)    14939 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/api/single_photo_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     8514 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/api/user_methods.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1836 2024-05-01 12:03:23.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/exceptions.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       93 2023-11-05 13:33:57.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/py.typed
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-23 09:42:54.669406 flickr_photos_api-2.3.2/src/flickr_photos_api/types/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     3016 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/types/__init__.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      767 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/types/contexts.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     1063 2024-05-01 13:51:00.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/types/users.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     5547 2024-03-21 12:08:35.000000 flickr_photos_api-2.3.2/src/flickr_photos_api/utils.py
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-23 09:42:54.669999 flickr_photos_api-2.3.2/src/flickr_photos_api.egg-info/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     4070 2024-05-23 09:42:54.000000 flickr_photos_api-2.3.2/src/flickr_photos_api.egg-info/PKG-INFO
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      958 2024-05-23 09:42:54.000000 flickr_photos_api-2.3.2/src/flickr_photos_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)        1 2024-05-23 09:42:54.000000 flickr_photos_api-2.3.2/src/flickr_photos_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       62 2024-05-23 09:42:54.000000 flickr_photos_api-2.3.2/src/flickr_photos_api.egg-info/requires.txt
+-rw-r--r--   0 alexwlchan   (501) staff       (20)       18 2024-05-23 09:42:54.000000 flickr_photos_api-2.3.2/src/flickr_photos_api.egg-info/top_level.txt
+drwxr-xr-x   0 alexwlchan   (501) staff       (20)        0 2024-05-23 09:42:54.669623 flickr_photos_api-2.3.2/tests/
+-rw-r--r--   0 alexwlchan   (501) staff       (20)     8494 2024-05-23 09:42:50.000000 flickr_photos_api-2.3.2/tests/test_errors.py
+-rw-r--r--   0 alexwlchan   (501) staff       (20)      472 2024-01-09 14:51:31.000000 flickr_photos_api-2.3.2/tests/test_utils.py
```

### Comparing `flickr_photos_api-2.3.1/LICENSE-APACHE` & `flickr_photos_api-2.3.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/LICENSE-MIT` & `flickr_photos_api-2.3.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/PKG-INFO` & `flickr_photos_api-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 2.3.1
+Version: 2.3.2
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr_photos_api-2.3.1/README.md` & `flickr_photos_api-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/pyproject.toml` & `flickr_photos_api-2.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/__init__.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     GroupContext,
     GroupInfo,
     PhotoContext,
     SinglePhotoInfo,
 )
 
 
-__version__ = "2.3.1"
+__version__ = "2.3.2"
 
 
 __all__ = [
     "FlickrApi",
     "FlickrApiException",
     "ResourceNotFound",
     "InvalidApiKey",
```

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/api/__init__.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/api/base.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/api/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,22 @@
 
     if isinstance(exc, httpx.ReadTimeout):
         return True
 
     if isinstance(exc, InvalidXmlException):
         return True
 
+    # This is a particular class of slightly flaky error that's difficult
+    # to reproduce -- relying on matching the text of the error is a bit
+    # fragile, but that's all we get from httpx.
+    if isinstance(exc, (httpx.ReadError, httpx.ConnectError)) and exc.args == (
+        "[Errno 54] Connection reset by peer",
+    ):
+        return True
+
     # Sometimes we get an error from the Flickr API like:
     #
     #     <err
     #       code="201"
     #       msg="Sorry, the Flickr API service is not currently available."
     #     />
     #
```

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/api/collection_methods.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/api/collection_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/api/comment_methods.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/api/comment_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/api/commons_methods.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/api/commons_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/api/from_url_methods.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/api/from_url_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/api/license_methods.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/api/license_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/api/single_photo_methods.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/api/single_photo_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/api/user_methods.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/api/user_methods.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/exceptions.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/types/__init__.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/types/contexts.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/types/contexts.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/types/users.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/types/users.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api/utils.py` & `flickr_photos_api-2.3.2/src/flickr_photos_api/utils.py`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/PKG-INFO` & `flickr_photos_api-2.3.2/src/flickr_photos_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flickr-photos-api
-Version: 2.3.1
+Version: 2.3.2
 Summary: Look up information about photos and collections of photos from Flickr
 Author-email: Flickr Foundation <hello@flickr.org>
 Maintainer-email: Alex Chan <alex@flickr.org>
 Project-URL: Homepage, https://github.com/Flickr-Foundation/flickr-photos-api
 Project-URL: Changelog, https://github.com/Flickr-Foundation/flickr-photos-api/blob/main/CHANGELOG.md
 Keywords: flickr
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flickr_photos_api-2.3.1/src/flickr_photos_api.egg-info/SOURCES.txt` & `flickr_photos_api-2.3.2/src/flickr_photos_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flickr_photos_api-2.3.1/tests/test_errors.py` & `flickr_photos_api-2.3.2/tests/test_errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,37 +130,63 @@
     #
     #     ResourceWarning: unclosed <ssl.SSLSocket fd=13, family=2,
     #     type=1, proto=0, laddr=('…', 58686), raddr=('…', 443)>
     #
     api.client.close()
 
 
+class FlakyClient:
+    """
+    This is a version of the Flickr API client that will throw the
+    given exception on the first request, then fall back to the
+    working client.
+    """
+
+    def __init__(self, underlying: httpx.Client, exc: Exception):
+        self.underlying = underlying
+        self.exception = exc
+        self.get_request_count = 0
+
+    def get(self, url: str, params: dict[str, str], timeout: int) -> httpx.Response:
+        self.get_request_count += 1
+
+        if self.get_request_count == 1:
+            raise self.exception
+        else:
+            return self.underlying.get(url=url, params=params, timeout=timeout)
+
+
 def test_a_timeout_is_retried(api: FlickrApi) -> None:
-    # This client throws a timeout error on the first GET request,
-    # and then makes regular HTTP requests after that.
-    class FlakyClient:
-        def __init__(self, underlying: httpx.Client):
-            self.underlying = underlying
-            self.get_request_count = 0
-
-        def get(self, url: str, params: dict[str, str], timeout: int) -> httpx.Response:
-            self.get_request_count += 1
-
-            if self.get_request_count == 1:
-                raise httpx.ReadTimeout("The read operation timed out")
-            else:
-                return self.underlying.get(url=url, params=params, timeout=timeout)
+    api.client = FlakyClient(
+        underlying=api.client, exc=httpx.ReadTimeout("The read operation timed out")
+    )  # type: ignore
+
+    resp = api.get_photos_in_user_photostream(user_id="61270229@N05")
+
+    assert len(resp["photos"]) == 10
+
 
-    api.client = FlakyClient(underlying=api.client)  # type: ignore
+def test_a_reset_connection_is_retried(api: FlickrApi) -> None:
+    api.client = FlakyClient(
+        underlying=api.client,
+        exc=httpx.ConnectError("[Errno 54] Connection reset by peer"),
+    )  # type: ignore
 
     resp = api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert len(resp["photos"]) == 10
 
 
+def test_an_unexplained_connecterror_fails(api: FlickrApi) -> None:
+    api.client = FlakyClient(underlying=api.client, exc=httpx.ConnectError(message="BOOM!"))  # type: ignore
+
+    with pytest.raises(httpx.ConnectError):
+        api.get_photos_in_user_photostream(user_id="61270229@N05")
+
+
 def test_retries_5xx_error(api: FlickrApi) -> None:
     # The cassette for this test was constructed manually: I edited
     # an existing cassette to add a 500 response as the first response,
     # then we want to see it make a second request to retry it.
     resp = api.get_photos_in_user_photostream(user_id="61270229@N05")
 
     assert len(resp["photos"]) == 10
```

