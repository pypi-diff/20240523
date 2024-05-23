# Comparing `tmp/direnumerate-4.0a2.tar.gz` & `tmp/direnumerate-4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-4.0a2.tar", last modified: Wed May 22 15:10:30 2024, max compression
+gzip compressed data, was "direnumerate-4.0a3.tar", last modified: Thu May 23 03:03:05 2024, max compression
```

## Comparing `direnumerate-4.0a2.tar` & `direnumerate-4.0a3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-22 15:10:30.477868 direnumerate-4.0a2/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-22 13:02:07.000000 direnumerate-4.0a2/LICENSE
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3707 2024-05-22 15:10:30.473868 direnumerate-4.0a2/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2282 2024-05-22 13:03:37.000000 direnumerate-4.0a2/README.md
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-22 15:10:30.469868 direnumerate-4.0a2/direnumerate/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     7822 2024-05-22 15:08:55.000000 direnumerate-4.0a2/direnumerate/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-05-22 15:09:05.000000 direnumerate-4.0a2/direnumerate/banner.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3401 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/colors.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/createlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      229 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/exceptions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      981 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/help.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2013 2024-05-22 15:09:00.000000 direnumerate-4.0a2/direnumerate/port_scan.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       73 2024-05-22 13:04:21.000000 direnumerate-4.0a2/direnumerate/version.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      334 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/warning.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-22 15:10:30.473868 direnumerate-4.0a2/direnumerate.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3707 2024-05-22 15:10:30.000000 direnumerate-4.0a2/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      515 2024-05-22 15:10:30.000000 direnumerate-4.0a2/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-22 15:10:30.000000 direnumerate-4.0a2/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-05-22 15:10:30.000000 direnumerate-4.0a2/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-05-22 15:10:30.000000 direnumerate-4.0a2/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-05-22 15:10:30.000000 direnumerate-4.0a2/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1567 2024-05-22 15:09:12.000000 direnumerate-4.0a2/pyproject.toml
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-22 15:10:30.477868 direnumerate-4.0a2/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-23 03:03:05.984969 direnumerate-4.0a3/
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18092 2024-05-23 02:01:45.000000 direnumerate-4.0a3/LICENSE
+-rw-r--r--   0 juan      (1000) juan      (1000)     3286 2024-05-23 03:03:05.980969 direnumerate-4.0a3/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1861 2024-05-23 03:01:51.000000 direnumerate-4.0a3/README.md
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-23 03:03:05.980969 direnumerate-4.0a3/direnumerate/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      421 2024-05-23 03:01:34.000000 direnumerate-4.0a3/direnumerate/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     7925 2024-05-23 02:51:58.000000 direnumerate-4.0a3/direnumerate/__main__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      125 2024-05-23 02:01:45.000000 direnumerate-4.0a3/direnumerate/banner.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2686 2024-05-23 03:02:03.000000 direnumerate-4.0a3/direnumerate/cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      394 2024-05-23 02:01:45.000000 direnumerate-4.0a3/direnumerate/colors.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    23461 2024-05-23 02:01:45.000000 direnumerate-4.0a3/direnumerate/createlist.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      229 2024-05-23 02:01:45.000000 direnumerate-4.0a3/direnumerate/exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      981 2024-05-23 02:01:45.000000 direnumerate-4.0a3/direnumerate/help.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2021 2024-05-23 03:01:45.000000 direnumerate-4.0a3/direnumerate/port_scan.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)       73 2024-05-23 02:13:03.000000 direnumerate-4.0a3/direnumerate/version.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      334 2024-05-23 02:01:45.000000 direnumerate-4.0a3/direnumerate/warning.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-23 03:03:05.980969 direnumerate-4.0a3/direnumerate.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     3286 2024-05-23 03:03:05.000000 direnumerate-4.0a3/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)      515 2024-05-23 03:03:05.000000 direnumerate-4.0a3/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-23 03:03:05.000000 direnumerate-4.0a3/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       55 2024-05-23 03:03:05.000000 direnumerate-4.0a3/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        9 2024-05-23 03:03:05.000000 direnumerate-4.0a3/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       13 2024-05-23 03:03:05.000000 direnumerate-4.0a3/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1567 2024-05-23 02:12:55.000000 direnumerate-4.0a3/pyproject.toml
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-23 03:03:05.984969 direnumerate-4.0a3/setup.cfg
```

### Comparing `direnumerate-4.0a2/LICENSE` & `direnumerate-4.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a2/PKG-INFO` & `direnumerate-4.0a3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 4.0a2
+Version: 4.0a3
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
@@ -71,73 +71,35 @@
 
     direnumerate -t testphp.vulnweb.com -w wordlist.txt
 
 ### Post Scan:
 
     direnumerate -t 44.228.249.3 -p 22 80 443
 
-### Finds patterns in logs:
-
-    direnumerate -log test.log -key ERROR
-
-### IP Info:
-
-    direnumerate -t 8.8.8.8 -i
-
 
 ## Scripts usage:
 
 ### Directory Scan in Websites:
 
 ```python
 
-from direnumerate import DirScan
+from direnumerate import Scan
 
 url = "testphp.vulnweb.com"
 wordlist = "wordlist.txt"
 
-enum = DirScan(url)
-enum.dir_enum(wordlist)
+enum = Scan(url)
+print(enum.show_dirs(wordlist))
 ```
 ----------
 
 ### Port Scan:
 
 ```python
 
-from direnumerate import PortScan
-
-ip = "44.228.249.3"
-list_ports = [22, 80, 443]
-
-scan = PortScan(ip)
-scan.scan_ports(list_ports)
-
-```
-----------
-
-### Finds patterns in logs:
-
-```python
-
-from direnumerate import FindPatterns
-
-log = "test.log"
-key = "ERROR"
-
-fp = FindPatterns(log)
-fp.find_in_log(keyword=key)
-```
-
-### IP Info:
-
-```python
-
-from direnumerate import InfoIp
-
-ip = "8.8.8.8"
+from direnumerate import Scan
 
-ipinfo = InfoIp(ip)
-ipinfo.show_info()
+enum = Scan()
+print(enum.port_scan(ip='44.228.249.3', ports=[22, 443, 8080, 8280, 80, 25]))
 
 ```
 ----------
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 4.0a2 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0a3 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -32,18 +32,13 @@
 and assess the security of web applications. ## Key Features - Enumeration of
 directories and files on web servers. - Creates a wordlist automatically -
 Wordlist customization. - Detailed output of findings. - Support for multiple
 URL schemes (http, https, etc.). ## install: pip install direnumerate ---------
 -------- ## install in ubuntu: pip install direnumerate --break-system-packages
 ---------- ## Command line usage: ### Directory Scan: direnumerate -
 t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate -
-t 44.228.249.3 -p 22 80 443 ### Finds patterns in logs: direnumerate -log
-test.log -key ERROR ### IP Info: direnumerate -t 8.8.8.8 -i ## Scripts usage:
-### Directory Scan in Websites: ```python from direnumerate import DirScan url
-= "testphp.vulnweb.com" wordlist = "wordlist.txt" enum = DirScan(url)
-enum.dir_enum(wordlist) ``` ---------- ### Port Scan: ```python from
-direnumerate import PortScan ip = "44.228.249.3" list_ports = [22, 80, 443]
-scan = PortScan(ip) scan.scan_ports(list_ports) ``` ---------- ### Finds
-patterns in logs: ```python from direnumerate import FindPatterns log =
-"test.log" key = "ERROR" fp = FindPatterns(log) fp.find_in_log(keyword=key) ```
-### IP Info: ```python from direnumerate import InfoIp ip = "8.8.8.8" ipinfo =
-InfoIp(ip) ipinfo.show_info() ``` ----------
+t 44.228.249.3 -p 22 80 443 ## Scripts usage: ### Directory Scan in Websites:
+```python from direnumerate import Scan url = "testphp.vulnweb.com" wordlist =
+"wordlist.txt" enum = Scan(url) print(enum.show_dirs(wordlist)) ``` ---------
+- ### Port Scan: ```python from direnumerate import Scan enum = Scan() print
+(enum.port_scan(ip='44.228.249.3', ports=[22, 443, 8080, 8280, 80, 25])) ``` --
+--------
```

### Comparing `direnumerate-4.0a2/README.md` & `direnumerate-4.0a3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -38,73 +38,35 @@
 
     direnumerate -t testphp.vulnweb.com -w wordlist.txt
 
 ### Post Scan:
 
     direnumerate -t 44.228.249.3 -p 22 80 443
 
-### Finds patterns in logs:
-
-    direnumerate -log test.log -key ERROR
-
-### IP Info:
-
-    direnumerate -t 8.8.8.8 -i
-
 
 ## Scripts usage:
 
 ### Directory Scan in Websites:
 
 ```python
 
-from direnumerate import DirScan
+from direnumerate import Scan
 
 url = "testphp.vulnweb.com"
 wordlist = "wordlist.txt"
 
-enum = DirScan(url)
-enum.dir_enum(wordlist)
+enum = Scan(url)
+print(enum.show_dirs(wordlist))
 ```
 ----------
 
 ### Port Scan:
 
 ```python
 
-from direnumerate import PortScan
-
-ip = "44.228.249.3"
-list_ports = [22, 80, 443]
-
-scan = PortScan(ip)
-scan.scan_ports(list_ports)
-
-```
-----------
-
-### Finds patterns in logs:
-
-```python
-
-from direnumerate import FindPatterns
-
-log = "test.log"
-key = "ERROR"
-
-fp = FindPatterns(log)
-fp.find_in_log(keyword=key)
-```
-
-### IP Info:
-
-```python
-
-from direnumerate import InfoIp
-
-ip = "8.8.8.8"
+from direnumerate import Scan
 
-ipinfo = InfoIp(ip)
-ipinfo.show_info()
+enum = Scan()
+print(enum.port_scan(ip='44.228.249.3', ports=[22, 443, 8080, 8280, 80, 25]))
 
 ```
 ----------
```

#### html2text {}

```diff
@@ -12,18 +12,13 @@
 and assess the security of web applications. ## Key Features - Enumeration of
 directories and files on web servers. - Creates a wordlist automatically -
 Wordlist customization. - Detailed output of findings. - Support for multiple
 URL schemes (http, https, etc.). ## install: pip install direnumerate ---------
 -------- ## install in ubuntu: pip install direnumerate --break-system-packages
 ---------- ## Command line usage: ### Directory Scan: direnumerate -
 t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate -
-t 44.228.249.3 -p 22 80 443 ### Finds patterns in logs: direnumerate -log
-test.log -key ERROR ### IP Info: direnumerate -t 8.8.8.8 -i ## Scripts usage:
-### Directory Scan in Websites: ```python from direnumerate import DirScan url
-= "testphp.vulnweb.com" wordlist = "wordlist.txt" enum = DirScan(url)
-enum.dir_enum(wordlist) ``` ---------- ### Port Scan: ```python from
-direnumerate import PortScan ip = "44.228.249.3" list_ports = [22, 80, 443]
-scan = PortScan(ip) scan.scan_ports(list_ports) ``` ---------- ### Finds
-patterns in logs: ```python from direnumerate import FindPatterns log =
-"test.log" key = "ERROR" fp = FindPatterns(log) fp.find_in_log(keyword=key) ```
-### IP Info: ```python from direnumerate import InfoIp ip = "8.8.8.8" ipinfo =
-InfoIp(ip) ipinfo.show_info() ``` ----------
+t 44.228.249.3 -p 22 80 443 ## Scripts usage: ### Directory Scan in Websites:
+```python from direnumerate import Scan url = "testphp.vulnweb.com" wordlist =
+"wordlist.txt" enum = Scan(url) print(enum.show_dirs(wordlist)) ``` ---------
+- ### Port Scan: ```python from direnumerate import Scan enum = Scan() print
+(enum.port_scan(ip='44.228.249.3', ports=[22, 443, 8080, 8280, 80, 25])) ``` --
+--------
```

### Comparing `direnumerate-4.0a2/direnumerate/__main__.py` & `direnumerate-4.0a3/direnumerate/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,21 +22,18 @@
 
 from direnumerate.createlist import create_wordlist
 from direnumerate.colors import Color
 from direnumerate.banner import *
 from direnumerate.help import help_direnumerate
 import direnumerate.exceptions as exception
 from direnumerate.warning import deprecated
+from direnumerate.port_scan import PortScan
 
 
-class Dire:
-    pass
-
-
-class DirScan:
+class Scan:
     """
     A class for directory scanning.
 
     Attributes:
         url (str): The URL to scan.
         wordlist_file (str): The path to the wordlist file.
     """
@@ -53,25 +50,23 @@
 
         try:
             url_verify = url[4]
         
             if url_verify == ":":
                 url = url.replace("http://", "https://")
                 self.url = url
-
             elif url_verify == "s":
                 self.url = url
-
             else:
                 self.url = "https://" + url
                 
         except IndexError:
             raise exception.DirenumerateError("[error] expected an argument")
 
-    def dir_enum(self, 
+    def show_dirs(self, 
                  wordlist_file, 
                  verbose_only_found: bool = False,
                  verbose: bool = False
                  ) -> list:
         """
         Perform directory enumeration.
 
@@ -141,15 +136,14 @@
                         full_url = f"{self.url}/{path}"
                         response = requests.get(full_url)
                         
                         if response.status_code == 200:
                             results_list.append(f'[Found] {full_url}')
                             if verbose:
                                 print(f"{Color.GREEN}[Found]:{Color.RESET} {full_url}")
-                            
                         elif response.status_code == 204:
                             results_list.append(f'[No Content] {full_url}')
                             if verbose:
                                 print(f"{Color.BLUE}[No Content]:{Color.RESET} {full_url}")
                         elif response.status_code == 400:
                             results_list.append(f'[Bad Request] {full_url}')
                             if verbose:
@@ -174,8 +168,12 @@
             except FileNotFoundError:
                 print(f"{Color.RED}Word list file not found.{Color.RESET}")
             except KeyboardInterrupt:
                 print(f"{Color.GREEN}Attempt interrupted by user.{Color.RESET}")
             except requests.exceptions.ConnectionError as rec:
                 print(f"{Color.RED}[Error] {rec}{Color.RESET}")
             
-        return results_list
+        return results_list
+    
+    def port_scan(self, ip, ports) -> list:
+        scan = PortScan(ip)
+        return scan.scan_ports(ports)
```

### Comparing `direnumerate-4.0a2/direnumerate/cli.py` & `direnumerate-4.0a3/direnumerate/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from direnumerate.__main__ import DirScan, PortScan, FindPattern, InfoIp
+from direnumerate.__main__ import Scan
 from direnumerate.colors import Color
 from direnumerate.banner import *
 from direnumerate.version import __version__
 
 
 def dir_scan(args):
     """
@@ -15,29 +15,29 @@
     show_banner()
 
     if args.verbose:
             try:
                 url = args.target
                 wordlist_file = args.wordlist
 
-                enum = DirScan(url)
-                enum.dir_enum(wordlist_file, verbose=True)
+                enum = Scan(url)
+                enum.show_dirs(wordlist_file, verbose=True)
             except TypeError:
                 print(Color.GREEN + "-------------------- Scan Finished --------------------" + Color.RESET)
             except KeyboardInterrupt:
                 print(Color.GREEN + "-------------- Attempt interrupted by user ------------" + Color.RESET)
     else:
         pass
 
     try:
         url = args.target
         wordlist_file = args.wordlist
 
-        enum = DirScan(url)
-        enum.dir_enum(wordlist_file)
+        enum = Scan(url)
+        enum.show_dirs(wordlist_file)
     except TypeError:
         print(Color.GREEN + "-------------------- Scan Finished --------------------" + Color.RESET)
     except KeyboardInterrupt:
         print(Color.GREEN + "-------------- Attempt interrupted by user ------------" + Color.RESET)
 
 
 def port_scan(args):
@@ -48,65 +48,39 @@
         args (argparse.Namespace): Command-line arguments and options.
     """
     show_banner()
     try:
         host = args.target
         ports = args.ports
 
-        scanner = PortScan(host)
-        scanner.scan_ports(ports)
+        scanner = Scan()
+        scanner.port_scan(host, ports)
     except KeyboardInterrupt:
         print(Color.GREEN + "-------------- Port scan interrupted by user ------------" + Color.RESET)
 
 
-def find_pattern(args):
-    show_banner()
-    file_name_log = args.logname
-    key = args.keyword
-
-    fp = FindPattern(file_name_log)
-    fp.find_in_log(keyword=key)
-
-
-def show_info_ip(args):
-    show_banner()
-    ip_address = args.info
-
-    ipinfo = InfoIp(ip_address)
-    ipinfo.show_info()
-
-
 def main():
     """
     The main function for the Direnumerate application.
 
     Parses command-line arguments and options, and executes the appropriate function.
     """
     parser = argparse.ArgumentParser(description="Direnumerate - Directory Enumeration on Web Servers")
     
     # Add arguments for directory enumeration
     parser.add_argument("-v", "--verbose", required=False, action="store_true", help="Verbose output")
     parser.add_argument("-t", "--target", required=False, help="Target URL (including scheme, e.g. http://www.example.com)")
     parser.add_argument("-w", "--wordlist", required=False, help="Wordlist file")
-    parser.add_argument("-i", "--info", required=False, help="Target host for info scanning")
     
     # Add arguments for port scanning
     parser.add_argument("-p", "--ports", nargs='+', type=int, help="Ports to scan (e.g., 22 80 443)")
     
-    # Add arguments for log scanning
-    parser.add_argument("-log", "--logname", help="Log Name")
-    parser.add_argument("-key", "--keyword", help="Key Word")
-    
 
     args = parser.parse_args()
-    
-    if args.logname and args.keyword:
-        find_pattern(args)
-    elif args.ports:
+
+    if args.ports:
         port_scan(args)
-    elif args.info:
-        show_info_ip(args)
     else:
         dir_scan(args)
 
 if __name__ == "__main__":
     main()
```

### Comparing `direnumerate-4.0a2/direnumerate/createlist.py` & `direnumerate-4.0a3/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a2/direnumerate/help.py` & `direnumerate-4.0a3/direnumerate/help.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a2/direnumerate/port_scan.py` & `direnumerate-4.0a3/direnumerate/port_scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Args:
             host (str): The host to scan for open ports.
             ports (list): A list of ports to scan.
         """
         self.host = host.replace("https://", "")
         self.open_ports = []
 
-    def scan_ports(self, ports):
+    def scan_ports(self, ports) -> list:
         """
         Scan the specified ports on the target host.
 
         This method attempts to establish a TCP connection to each port in the list of ports on the target host.
         If the connection is successful (result == 0), the port is considered open, and it is added to the open_ports list.
         If the connection fails, the port is considered closed.
```

### Comparing `direnumerate-4.0a2/direnumerate.egg-info/PKG-INFO` & `direnumerate-4.0a3/direnumerate.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 4.0a2
+Version: 4.0a3
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
@@ -71,73 +71,35 @@
 
     direnumerate -t testphp.vulnweb.com -w wordlist.txt
 
 ### Post Scan:
 
     direnumerate -t 44.228.249.3 -p 22 80 443
 
-### Finds patterns in logs:
-
-    direnumerate -log test.log -key ERROR
-
-### IP Info:
-
-    direnumerate -t 8.8.8.8 -i
-
 
 ## Scripts usage:
 
 ### Directory Scan in Websites:
 
 ```python
 
-from direnumerate import DirScan
+from direnumerate import Scan
 
 url = "testphp.vulnweb.com"
 wordlist = "wordlist.txt"
 
-enum = DirScan(url)
-enum.dir_enum(wordlist)
+enum = Scan(url)
+print(enum.show_dirs(wordlist))
 ```
 ----------
 
 ### Port Scan:
 
 ```python
 
-from direnumerate import PortScan
-
-ip = "44.228.249.3"
-list_ports = [22, 80, 443]
-
-scan = PortScan(ip)
-scan.scan_ports(list_ports)
-
-```
-----------
-
-### Finds patterns in logs:
-
-```python
-
-from direnumerate import FindPatterns
-
-log = "test.log"
-key = "ERROR"
-
-fp = FindPatterns(log)
-fp.find_in_log(keyword=key)
-```
-
-### IP Info:
-
-```python
-
-from direnumerate import InfoIp
-
-ip = "8.8.8.8"
+from direnumerate import Scan
 
-ipinfo = InfoIp(ip)
-ipinfo.show_info()
+enum = Scan()
+print(enum.port_scan(ip='44.228.249.3', ports=[22, 443, 8080, 8280, 80, 25]))
 
 ```
 ----------
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 4.0a2 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0a3 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -32,18 +32,13 @@
 and assess the security of web applications. ## Key Features - Enumeration of
 directories and files on web servers. - Creates a wordlist automatically -
 Wordlist customization. - Detailed output of findings. - Support for multiple
 URL schemes (http, https, etc.). ## install: pip install direnumerate ---------
 -------- ## install in ubuntu: pip install direnumerate --break-system-packages
 ---------- ## Command line usage: ### Directory Scan: direnumerate -
 t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate -
-t 44.228.249.3 -p 22 80 443 ### Finds patterns in logs: direnumerate -log
-test.log -key ERROR ### IP Info: direnumerate -t 8.8.8.8 -i ## Scripts usage:
-### Directory Scan in Websites: ```python from direnumerate import DirScan url
-= "testphp.vulnweb.com" wordlist = "wordlist.txt" enum = DirScan(url)
-enum.dir_enum(wordlist) ``` ---------- ### Port Scan: ```python from
-direnumerate import PortScan ip = "44.228.249.3" list_ports = [22, 80, 443]
-scan = PortScan(ip) scan.scan_ports(list_ports) ``` ---------- ### Finds
-patterns in logs: ```python from direnumerate import FindPatterns log =
-"test.log" key = "ERROR" fp = FindPatterns(log) fp.find_in_log(keyword=key) ```
-### IP Info: ```python from direnumerate import InfoIp ip = "8.8.8.8" ipinfo =
-InfoIp(ip) ipinfo.show_info() ``` ----------
+t 44.228.249.3 -p 22 80 443 ## Scripts usage: ### Directory Scan in Websites:
+```python from direnumerate import Scan url = "testphp.vulnweb.com" wordlist =
+"wordlist.txt" enum = Scan(url) print(enum.show_dirs(wordlist)) ``` ---------
+- ### Port Scan: ```python from direnumerate import Scan enum = Scan() print
+(enum.port_scan(ip='44.228.249.3', ports=[22, 443, 8080, 8280, 80, 25])) ``` --
+--------
```

### Comparing `direnumerate-4.0a2/direnumerate.egg-info/SOURCES.txt` & `direnumerate-4.0a3/direnumerate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a2/pyproject.toml` & `direnumerate-4.0a3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "4.0a2"
+version = "4.0a3"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

