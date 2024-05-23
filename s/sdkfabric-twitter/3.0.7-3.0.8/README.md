# Comparing `tmp/sdkfabric_twitter-3.0.7.tar.gz` & `tmp/sdkfabric_twitter-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_twitter-3.0.7.tar", last modified: Sun May 19 18:03:32 2024, max compression
+gzip compressed data, was "sdkfabric_twitter-3.0.8.tar", last modified: Thu May 23 21:16:45 2024, max compression
```

## Comparing `sdkfabric_twitter-3.0.7.tar` & `sdkfabric_twitter-3.0.8.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:03:32.847501 sdkfabric_twitter-3.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 18:03:32.847501 sdkfabric_twitter-3.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 18:03:25.000000 sdkfabric_twitter-3.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:03:32.847501 sdkfabric_twitter-3.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:03:32.839501 sdkfabric_twitter-3.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:03:32.847501 sdkfabric_twitter-3.0.7/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/bookmark_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/bookmark_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/hide_reply.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/hide_reply_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/like.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/like_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/quote_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/search_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/single_tweet.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/trend.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/trend_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/trends_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_delete_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_media.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_reply.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/tweet_usage_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/usage_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/user_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-19 18:03:23.000000 sdkfabric_twitter-3.0.7/src/sdk/user_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:03:32.847501 sdkfabric_twitter-3.0.7/src/sdkfabric_twitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 18:03:32.000000 sdkfabric_twitter-3.0.7/src/sdkfabric_twitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-19 18:03:32.000000 sdkfabric_twitter-3.0.7/src/sdkfabric_twitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:03:32.000000 sdkfabric_twitter-3.0.7/src/sdkfabric_twitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 18:03:32.000000 sdkfabric_twitter-3.0.7/src/sdkfabric_twitter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 18:03:32.000000 sdkfabric_twitter-3.0.7/src/sdkfabric_twitter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:16:45.459597 sdkfabric_twitter-3.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 21:16:45.459597 sdkfabric_twitter-3.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-23 21:16:36.000000 sdkfabric_twitter-3.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:16:45.459597 sdkfabric_twitter-3.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:16:45.447597 sdkfabric_twitter-3.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:16:45.455597 sdkfabric_twitter-3.0.8/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/bookmark_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/bookmark_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/hide_reply.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/hide_reply_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/like.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/like_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/quote_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/retweet_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/search_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/single_tweet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/trend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/trend_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/trends_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_reply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/tweet_usage_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/usage_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/user_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-05-23 21:16:35.000000 sdkfabric_twitter-3.0.8/src/sdk/user_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:16:45.459597 sdkfabric_twitter-3.0.8/src/sdkfabric_twitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 21:16:45.000000 sdkfabric_twitter-3.0.8/src/sdkfabric_twitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-23 21:16:45.000000 sdkfabric_twitter-3.0.8/src/sdkfabric_twitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:16:45.000000 sdkfabric_twitter-3.0.8/src/sdkfabric_twitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 21:16:45.000000 sdkfabric_twitter-3.0.8/src/sdkfabric_twitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 21:16:45.000000 sdkfabric_twitter-3.0.8/src/sdkfabric_twitter.egg-info/top_level.txt
```

### Comparing `sdkfabric_twitter-3.0.7/LICENSE` & `sdkfabric_twitter-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/PKG-INFO` & `sdkfabric_twitter-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-twitter
-Version: 3.0.7
+Version: 3.0.8
 Summary: Twitter Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/twitter-python
 Project-URL: Issues, https://github.com/sdk-fabric/twitter-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_twitter-3.0.7/README.md` & `sdkfabric_twitter-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/pyproject.toml` & `sdkfabric_twitter-3.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-twitter"
-version = "3.0.7"
+version = "3.0.8"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Twitter Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/bookmark_tag.py` & `sdkfabric_twitter-3.0.8/src/sdk/bookmark_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/client.py` & `sdkfabric_twitter-3.0.8/src/sdk/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .tweet_tag import TweetTag
 from .usage_tag import UsageTag
 from .user_tag import UserTag
 from .bookmark_tag import BookmarkTag
 from .search_tag import SearchTag
 from .quote_tag import QuoteTag
 from .trends_tag import TrendsTag
+from .retweet_tag import RetweetTag
 
 class Client(sdkgen.ClientAbstract):
     def __init__(self, base_url: str, credentials: sdkgen.CredentialsInterface):
         super().__init__(base_url, credentials)
 
     def tweet(self) -> TweetTag:
         return TweetTag(
@@ -58,13 +59,19 @@
 
     def trends(self) -> TrendsTag:
         return TrendsTag(
             self.http_client,
             self.parser
         )
 
+    def retweet(self) -> RetweetTag:
+        return RetweetTag(
+            self.http_client,
+            self.parser
+        )
+
 
 
     @staticmethod
     def build(token: str):
         return Client("https://api.twitter.com", sdkgen.HttpBearer(token))
```

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/fields.py` & `sdkfabric_twitter-3.0.8/src/sdk/fields.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/pagination.py` & `sdkfabric_twitter-3.0.8/src/sdk/pagination.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/quote_tag.py` & `sdkfabric_twitter-3.0.8/src/sdk/quote_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/search_tag.py` & `sdkfabric_twitter-3.0.8/src/sdk/search_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/trends_tag.py` & `sdkfabric_twitter-3.0.8/src/sdk/trends_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/tweet.py` & `sdkfabric_twitter-3.0.8/src/sdk/tweet.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/tweet_details.py` & `sdkfabric_twitter-3.0.8/src/sdk/tweet_details.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/tweet_reply.py` & `sdkfabric_twitter-3.0.8/src/sdk/tweet_reply.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/tweet_tag.py` & `sdkfabric_twitter-3.0.8/src/sdk/tweet_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/tweet_usage.py` & `sdkfabric_twitter-3.0.8/src/sdk/tweet_usage.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/usage_tag.py` & `sdkfabric_twitter-3.0.8/src/sdk/usage_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/user.py` & `sdkfabric_twitter-3.0.8/src/sdk/user.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_twitter-3.0.7/src/sdk/user_tag.py` & `sdkfabric_twitter-3.0.8/src/sdk/user_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -221,8 +221,35 @@
                 return UserCollection.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
+    def get_me(self, expansions: str, fields: str) -> User:
+        """
+        Returns information about an authorized user.
+        """
+        try:
+            path_params = {}
+
+            query_params = {}
+            query_params["expansions"] = expansions
+            query_params["fields"] = fields
+
+            query_struct_names = []
+
+            url = self.parser.url("/2/users/me", path_params)
+
+            headers = {}
+
+            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
+
+            if response.status_code >= 200 and response.status_code < 300:
+                return User.model_validate_json(json_data=response.content)
+
+
+            raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
+        except RequestException as e:
+            raise sdkgen.ClientException("An unknown error occurred: " + str(e))
+
```

### Comparing `sdkfabric_twitter-3.0.7/src/sdkfabric_twitter.egg-info/PKG-INFO` & `sdkfabric_twitter-3.0.8/src/sdkfabric_twitter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-twitter
-Version: 3.0.7
+Version: 3.0.8
 Summary: Twitter Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/twitter-python
 Project-URL: Issues, https://github.com/sdk-fabric/twitter-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_twitter-3.0.7/src/sdkfabric_twitter.egg-info/SOURCES.txt` & `sdkfabric_twitter-3.0.8/src/sdkfabric_twitter.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/sdk/fields.py
 src/sdk/hide_reply.py
 src/sdk/hide_reply_response.py
 src/sdk/like.py
 src/sdk/like_response.py
 src/sdk/pagination.py
 src/sdk/quote_tag.py
+src/sdk/retweet_tag.py
 src/sdk/search_tag.py
 src/sdk/single_tweet.py
 src/sdk/trend.py
 src/sdk/trend_collection.py
 src/sdk/trends_tag.py
 src/sdk/tweet.py
 src/sdk/tweet_collection.py
```

