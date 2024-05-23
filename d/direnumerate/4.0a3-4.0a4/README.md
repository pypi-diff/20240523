# Comparing `tmp/direnumerate-4.0a3.tar.gz` & `tmp/direnumerate-4.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-4.0a3.tar", last modified: Thu May 23 03:03:05 2024, max compression
+gzip compressed data, was "direnumerate-4.0a4.tar", last modified: Thu May 23 16:43:05 2024, max compression
```

## Comparing `direnumerate-4.0a3.tar` & `direnumerate-4.0a4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-23 03:03:05.984969 direnumerate-4.0a3/
--rw-rw-r--   0 juan      (1000) juan      (1000)    18092 2024-05-23 02:01:45.000000 direnumerate-4.0a3/LICENSE
--rw-r--r--   0 juan      (1000) juan      (1000)     3286 2024-05-23 03:03:05.980969 direnumerate-4.0a3/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     1861 2024-05-23 03:01:51.000000 direnumerate-4.0a3/README.md
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-23 03:03:05.980969 direnumerate-4.0a3/direnumerate/
--rw-rw-r--   0 juan      (1000) juan      (1000)      421 2024-05-23 03:01:34.000000 direnumerate-4.0a3/direnumerate/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     7925 2024-05-23 02:51:58.000000 direnumerate-4.0a3/direnumerate/__main__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      125 2024-05-23 02:01:45.000000 direnumerate-4.0a3/direnumerate/banner.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2686 2024-05-23 03:02:03.000000 direnumerate-4.0a3/direnumerate/cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      394 2024-05-23 02:01:45.000000 direnumerate-4.0a3/direnumerate/colors.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    23461 2024-05-23 02:01:45.000000 direnumerate-4.0a3/direnumerate/createlist.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      229 2024-05-23 02:01:45.000000 direnumerate-4.0a3/direnumerate/exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      981 2024-05-23 02:01:45.000000 direnumerate-4.0a3/direnumerate/help.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2021 2024-05-23 03:01:45.000000 direnumerate-4.0a3/direnumerate/port_scan.py
--rw-rw-r--   0 juan      (1000) juan      (1000)       73 2024-05-23 02:13:03.000000 direnumerate-4.0a3/direnumerate/version.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      334 2024-05-23 02:01:45.000000 direnumerate-4.0a3/direnumerate/warning.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-23 03:03:05.980969 direnumerate-4.0a3/direnumerate.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     3286 2024-05-23 03:03:05.000000 direnumerate-4.0a3/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)      515 2024-05-23 03:03:05.000000 direnumerate-4.0a3/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-23 03:03:05.000000 direnumerate-4.0a3/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       55 2024-05-23 03:03:05.000000 direnumerate-4.0a3/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        9 2024-05-23 03:03:05.000000 direnumerate-4.0a3/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       13 2024-05-23 03:03:05.000000 direnumerate-4.0a3/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)     1567 2024-05-23 02:12:55.000000 direnumerate-4.0a3/pyproject.toml
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-23 03:03:05.984969 direnumerate-4.0a3/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-23 16:43:05.614849 direnumerate-4.0a4/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-23 14:34:30.000000 direnumerate-4.0a4/LICENSE
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3286 2024-05-23 16:43:05.614849 direnumerate-4.0a4/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1861 2024-05-23 16:36:50.000000 direnumerate-4.0a4/README.md
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-23 16:43:05.610849 direnumerate-4.0a4/direnumerate/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      421 2024-05-23 16:36:50.000000 direnumerate-4.0a4/direnumerate/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     7925 2024-05-23 16:36:50.000000 direnumerate-4.0a4/direnumerate/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-05-23 14:34:30.000000 direnumerate-4.0a4/direnumerate/banner.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2624 2024-05-23 16:40:42.000000 direnumerate-4.0a4/direnumerate/cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-05-23 14:34:30.000000 direnumerate-4.0a4/direnumerate/colors.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-05-23 14:34:30.000000 direnumerate-4.0a4/direnumerate/createlist.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      229 2024-05-23 14:34:30.000000 direnumerate-4.0a4/direnumerate/exceptions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      981 2024-05-23 14:34:30.000000 direnumerate-4.0a4/direnumerate/help.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2021 2024-05-23 16:36:50.000000 direnumerate-4.0a4/direnumerate/port_scan.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       73 2024-05-23 16:40:51.000000 direnumerate-4.0a4/direnumerate/version.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      334 2024-05-23 14:34:30.000000 direnumerate-4.0a4/direnumerate/warning.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-23 16:43:05.614849 direnumerate-4.0a4/direnumerate.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3286 2024-05-23 16:43:05.000000 direnumerate-4.0a4/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      515 2024-05-23 16:43:05.000000 direnumerate-4.0a4/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-23 16:43:05.000000 direnumerate-4.0a4/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-05-23 16:43:05.000000 direnumerate-4.0a4/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-05-23 16:43:05.000000 direnumerate-4.0a4/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-05-23 16:43:05.000000 direnumerate-4.0a4/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1567 2024-05-23 16:39:54.000000 direnumerate-4.0a4/pyproject.toml
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-23 16:43:05.614849 direnumerate-4.0a4/setup.cfg
```

### Comparing `direnumerate-4.0a3/LICENSE` & `direnumerate-4.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a3/PKG-INFO` & `direnumerate-4.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 4.0a3
+Version: 4.0a4
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 4.0a3 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0a4 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-4.0a3/README.md` & `direnumerate-4.0a4/README.md`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a3/direnumerate/__main__.py` & `direnumerate-4.0a4/direnumerate/__main__.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a3/direnumerate/cli.py` & `direnumerate-4.0a4/direnumerate/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         pass
 
     try:
         url = args.target
         wordlist_file = args.wordlist
 
         enum = Scan(url)
-        enum.show_dirs(wordlist_file)
+        enum.show_dirs(wordlist_file=wordlist_file)
     except TypeError:
         print(Color.GREEN + "-------------------- Scan Finished --------------------" + Color.RESET)
     except KeyboardInterrupt:
         print(Color.GREEN + "-------------- Attempt interrupted by user ------------" + Color.RESET)
 
 
 def port_scan(args):
@@ -49,36 +49,33 @@
     """
     show_banner()
     try:
         host = args.target
         ports = args.ports
 
         scanner = Scan()
-        scanner.port_scan(host, ports)
+        scanner.port_scan(ip=host, ports=ports)
     except KeyboardInterrupt:
         print(Color.GREEN + "-------------- Port scan interrupted by user ------------" + Color.RESET)
 
 
 def main():
     """
     The main function for the Direnumerate application.
 
     Parses command-line arguments and options, and executes the appropriate function.
     """
     parser = argparse.ArgumentParser(description="Direnumerate - Directory Enumeration on Web Servers")
     
-    # Add arguments for directory enumeration
     parser.add_argument("-v", "--verbose", required=False, action="store_true", help="Verbose output")
     parser.add_argument("-t", "--target", required=False, help="Target URL (including scheme, e.g. http://www.example.com)")
     parser.add_argument("-w", "--wordlist", required=False, help="Wordlist file")
     
-    # Add arguments for port scanning
     parser.add_argument("-p", "--ports", nargs='+', type=int, help="Ports to scan (e.g., 22 80 443)")
     
-
     args = parser.parse_args()
 
     if args.ports:
         port_scan(args)
     else:
         dir_scan(args)
```

### Comparing `direnumerate-4.0a3/direnumerate/createlist.py` & `direnumerate-4.0a4/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a3/direnumerate/help.py` & `direnumerate-4.0a4/direnumerate/help.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a3/direnumerate/port_scan.py` & `direnumerate-4.0a4/direnumerate/port_scan.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a3/direnumerate.egg-info/PKG-INFO` & `direnumerate-4.0a4/direnumerate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 4.0a3
+Version: 4.0a4
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 4.0a3 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0a4 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-4.0a3/direnumerate.egg-info/SOURCES.txt` & `direnumerate-4.0a4/direnumerate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a3/pyproject.toml` & `direnumerate-4.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "4.0a3"
+version = "4.0a4"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

