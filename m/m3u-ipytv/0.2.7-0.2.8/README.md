# Comparing `tmp/m3u-ipytv-0.2.7.tar.gz` & `tmp/m3u-ipytv-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3u-ipytv-0.2.7.tar", last modified: Wed Nov 22 17:12:46 2023, max compression
+gzip compressed data, was "m3u-ipytv-0.2.8.tar", last modified: Thu May 23 11:40:49 2024, max compression
```

## Comparing `m3u-ipytv-0.2.7.tar` & `m3u-ipytv-0.2.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-22 17:12:46.547494 m3u-ipytv-0.2.7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1073 2023-11-22 17:12:36.000000 m3u-ipytv-0.2.7/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-11-22 17:12:36.000000 m3u-ipytv-0.2.7/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14118 2023-11-22 17:12:46.547494 m3u-ipytv-0.2.7/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12940 2023-11-22 17:12:36.000000 m3u-ipytv-0.2.7/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-22 17:12:46.543494 m3u-ipytv-0.2.7/ipytv/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-11-22 17:12:36.000000 m3u-ipytv-0.2.7/ipytv/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11182 2023-11-22 17:12:36.000000 m3u-ipytv-0.2.7/ipytv/channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5025 2023-11-22 17:12:36.000000 m3u-ipytv-0.2.7/ipytv/doctor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      714 2023-11-22 17:12:36.000000 m3u-ipytv-0.2.7/ipytv/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3309 2023-11-22 17:12:36.000000 m3u-ipytv-0.2.7/ipytv/m3u.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21076 2023-11-22 17:12:36.000000 m3u-ipytv-0.2.7/ipytv/playlist.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-22 17:12:46.547494 m3u-ipytv-0.2.7/m3u_ipytv.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14118 2023-11-22 17:12:46.000000 m3u-ipytv-0.2.7/m3u_ipytv.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-11-22 17:12:46.000000 m3u-ipytv-0.2.7/m3u_ipytv.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-11-22 17:12:46.000000 m3u-ipytv-0.2.7/m3u_ipytv.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       17 2023-11-22 17:12:46.000000 m3u-ipytv-0.2.7/m3u_ipytv.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-11-22 17:12:46.000000 m3u-ipytv-0.2.7/m3u_ipytv.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2023-11-22 17:12:45.000000 m3u-ipytv-0.2.7/pkgdata.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2023-11-22 17:12:36.000000 m3u-ipytv-0.2.7/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2023-11-22 17:12:46.547494 m3u-ipytv-0.2.7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2330 2023-11-22 17:12:36.000000 m3u-ipytv-0.2.7/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-22 17:12:46.547494 m3u-ipytv-0.2.7/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5792 2023-11-22 17:12:36.000000 m3u-ipytv-0.2.7/tests/test_data.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 11:40:49.572810 m3u-ipytv-0.2.8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1073 2024-05-23 11:40:39.000000 m3u-ipytv-0.2.8/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2024-05-23 11:40:39.000000 m3u-ipytv-0.2.8/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14150 2024-05-23 11:40:49.572810 m3u-ipytv-0.2.8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12940 2024-05-23 11:40:39.000000 m3u-ipytv-0.2.8/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 11:40:49.572810 m3u-ipytv-0.2.8/ipytv/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-23 11:40:39.000000 m3u-ipytv-0.2.8/ipytv/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11182 2024-05-23 11:40:39.000000 m3u-ipytv-0.2.8/ipytv/channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5903 2024-05-23 11:40:39.000000 m3u-ipytv-0.2.8/ipytv/doctor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      714 2024-05-23 11:40:39.000000 m3u-ipytv-0.2.8/ipytv/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3303 2024-05-23 11:40:39.000000 m3u-ipytv-0.2.8/ipytv/m3u.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21076 2024-05-23 11:40:39.000000 m3u-ipytv-0.2.8/ipytv/playlist.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 11:40:49.572810 m3u-ipytv-0.2.8/m3u_ipytv.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14150 2024-05-23 11:40:49.000000 m3u-ipytv-0.2.8/m3u_ipytv.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2024-05-23 11:40:49.000000 m3u-ipytv-0.2.8/m3u_ipytv.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-23 11:40:49.000000 m3u-ipytv-0.2.8/m3u_ipytv.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       17 2024-05-23 11:40:49.000000 m3u-ipytv-0.2.8/m3u_ipytv.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-23 11:40:49.000000 m3u-ipytv-0.2.8/m3u_ipytv.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-05-23 11:40:48.000000 m3u-ipytv-0.2.8/pkgdata.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-05-23 11:40:39.000000 m3u-ipytv-0.2.8/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-05-23 11:40:49.572810 m3u-ipytv-0.2.8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2330 2024-05-23 11:40:39.000000 m3u-ipytv-0.2.8/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 11:40:49.572810 m3u-ipytv-0.2.8/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6228 2024-05-23 11:40:39.000000 m3u-ipytv-0.2.8/tests/test_data.py
```

### Comparing `m3u-ipytv-0.2.7/LICENSE.txt` & `m3u-ipytv-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `m3u-ipytv-0.2.7/PKG-INFO` & `m3u-ipytv-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3u-ipytv
-Version: 0.2.7
+Version: 0.2.8
 Summary: A library for handling M3U playlists for IPTV (AKA m3u_plus)
 Home-page: https://github.com/Beer4Ever83/ipytv
 Author: Francesco Rainone
 Author-email: beer4evah@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/Beer4Ever83/ipytv/issues
 Project-URL: Funding, https://www.buymeacoffee.com/beer4ever83
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: requests>=2.25.1
 
 ![IPyTV logo](doc/logo_hd.png "IPyTV logo")
 
 A python3 library to parse IPTV playlists in the M3U Plus format.
 
 [![Downloads](https://pepy.tech/badge/m3u-ipytv)](https://pepy.tech/project/m3u-ipytv)
 [![Downloads](https://pepy.tech/badge/m3u-ipytv/month)](https://pepy.tech/project/m3u-ipytv)
```

### Comparing `m3u-ipytv-0.2.7/README.md` & `m3u-ipytv-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `m3u-ipytv-0.2.7/ipytv/channel.py` & `m3u-ipytv-0.2.8/ipytv/channel.py`

 * *Files identical despite different names*

### Comparing `m3u-ipytv-0.2.7/ipytv/doctor.py` & `m3u-ipytv-0.2.8/ipytv/doctor.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,17 +55,38 @@
                     name = match.group("name_g")
                     value = match.group("value_g")
                     new_row = new_row.replace(attribute, f" {name}=\"{value}\"")
             fixed_m3u_rows.append(new_row)
         return fixed_m3u_rows
 
     @staticmethod
+    def _fix_space_before_comma(m3u_rows: List[str]) -> List:
+        """
+        This covers the case of EXTINF rows with no attributes, but with one or more spaces between the comma and the
+        channel name.
+        Example:
+            #EXTINF:-1 ,Channel 22
+        """
+        spaces_before_comma_regex = r"^#EXTINF:(?P<duration_g>[-0-9\.]+)(?P<spaces_g>\s)+,(?P<name_g>.*)"
+        fixed_m3u_rows: List = []
+        for current_row in m3u_rows:
+            new_row = current_row
+            if m3u.is_extinf_row(current_row):
+                match = re.match(spaces_before_comma_regex, current_row)
+                if match:
+                    new_row = f"#EXTINF:{match.group('duration_g')},{match.group('name_g')}"
+            fixed_m3u_rows.append(new_row)
+        return fixed_m3u_rows
+
+
+    @staticmethod
     def sanitize(m3u_rows: List) -> List:
         fixed = M3UDoctor._fix_split_quoted_string(m3u_rows)
         fixed = M3UDoctor._fix_unquoted_numeric_attributes(fixed)
+        fixed = M3UDoctor._fix_space_before_comma(fixed)
         return fixed
 
 
 class IPTVChannelDoctor:
     @staticmethod
     def _urlencode_value(chan: IPTVChannel, attribute_name: str) -> None:
         """
```

### Comparing `m3u-ipytv-0.2.7/ipytv/exceptions.py` & `m3u-ipytv-0.2.8/ipytv/exceptions.py`

 * *Files identical despite different names*

### Comparing `m3u-ipytv-0.2.7/ipytv/m3u.py` & `m3u-ipytv-0.2.8/ipytv/m3u.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,12 +85,12 @@
 
 
 def is_comment_or_tag_row(row: str) -> bool:
     return row.startswith('#')
 
 
 def is_empty_row(row: str) -> bool:
-    return len(row.strip()) == 0
+    return not row.strip()
 
 
 def is_url_row(row: str) -> bool:
     return not is_m3u_header_row(row) and not is_comment_or_tag_row(row) and not is_empty_row(row)
```

### Comparing `m3u-ipytv-0.2.7/ipytv/playlist.py` & `m3u-ipytv-0.2.8/ipytv/playlist.py`

 * *Files identical despite different names*

### Comparing `m3u-ipytv-0.2.7/m3u_ipytv.egg-info/PKG-INFO` & `m3u-ipytv-0.2.8/m3u_ipytv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3u-ipytv
-Version: 0.2.7
+Version: 0.2.8
 Summary: A library for handling M3U playlists for IPTV (AKA m3u_plus)
 Home-page: https://github.com/Beer4Ever83/ipytv
 Author: Francesco Rainone
 Author-email: beer4evah@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/Beer4Ever83/ipytv/issues
 Project-URL: Funding, https://www.buymeacoffee.com/beer4ever83
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: requests>=2.25.1
 
 ![IPyTV logo](doc/logo_hd.png "IPyTV logo")
 
 A python3 library to parse IPTV playlists in the M3U Plus format.
 
 [![Downloads](https://pepy.tech/badge/m3u-ipytv)](https://pepy.tech/project/m3u-ipytv)
 [![Downloads](https://pepy.tech/badge/m3u-ipytv/month)](https://pepy.tech/project/m3u-ipytv)
```

### Comparing `m3u-ipytv-0.2.7/setup.py` & `m3u-ipytv-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `m3u-ipytv-0.2.7/tests/test_data.py` & `m3u-ipytv-0.2.8/tests/test_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -150,7 +150,19 @@
 broken_extinf_row = """#EXTINF:-1 tvg-id="" tvg-name=""AR || Wonderful! || "RR" tvg-logo="https://img.mysite.net/5425.jpg" group-title="free, stream","AR || Wonderful! || "RR"""
 expected_attributes_broken_extinf_row = {
     'tvg-id': '',
     'tvg-name': '_AR || Wonderful! || _RR',
     'tvg-logo': 'https://img.mysite.net/5425.jpg',
     'group-title': 'free, stream'
 }
+
+space_before_comma = """#EXTM3U url-tvg="http://epg.51zmt.top:8000/e.xml" catchup="append" catchup-source="?playseek=${(b)yyyyMMddHHmmss}-${(e)yyyyMMddHHmmss}"
+
+#EXTINF:10 ,channel name 0
+http://myown.link:80/luke/109163/78280
+#EXTINF:-11  ,channel name 1
+http://myown.link:80/luke/109163/78281
+#EXTINF:12 ,channel name 2
+http://myown.link:80/luke/109163/78282
+#EXTINF:13.0   ,channel name 3
+http://myown.link:80/luke/109163/78283
+"""
```

