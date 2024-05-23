# Comparing `tmp/scanlha-0.5.tar.gz` & `tmp/scanlha-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanlha-0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "scanlha-0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `scanlha-0.5.tar` & `scanlha-0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       19 2018-11-19 19:22:15.413651 scanlha-0.5/.gitattributes
--rw-r--r--   0        0        0       69 2024-05-16 20:51:45.959722 scanlha-0.5/.gitignore
--rw-r--r--   0        0        0       13 2018-07-21 00:32:14.277115 scanlha-0.5/.pylintrc
--rw-r--r--   0        0        0    32422 2018-08-04 11:55:53.638442 scanlha-0.5/LICENSE
--rw-r--r--   0        0        0     8540 2018-11-19 20:18:13.295416 scanlha-0.5/README.md
--rw-r--r--   0        0        0     1965 2021-04-29 07:22:05.208171 scanlha-0.5/ScanLHA/EditLHA.py
--rw-r--r--   0        0        0     2254 2024-04-05 22:53:33.065780 scanlha-0.5/ScanLHA/MergeLHA.py
--rw-r--r--   0        0        0    19235 2024-04-05 22:53:33.065780 scanlha-0.5/ScanLHA/PlotLHA.py
--rw-r--r--   0        0        0     5317 2018-12-01 16:18:46.019182 scanlha-0.5/ScanLHA/ScanLHA.py
--rw-r--r--   0        0        0     8947 2024-05-16 20:49:18.459726 scanlha-0.5/ScanLHA/__init__.py
--rw-r--r--   0        0        0    14569 2024-04-05 22:53:33.065780 scanlha-0.5/ScanLHA/config.py
--rw-r--r--   0        0        0     2126 2018-10-27 18:59:54.551599 scanlha-0.5/ScanLHA/configs/SPheno.yml
--rw-r--r--   0        0        0    14960 2021-04-29 07:22:05.211504 scanlha-0.5/ScanLHA/runner.py
--rw-r--r--   0        0        0    11935 2021-04-29 07:22:05.211504 scanlha-0.5/ScanLHA/scan.py
--rw-r--r--   0        0        0     4856 2024-04-05 22:53:33.065780 scanlha-0.5/ScanLHA/slha.py
--rw-r--r--   0        0        0    36811 2018-11-19 20:18:14.118738 scanlha-0.5/docs/EditLHA.m.html
--rw-r--r--   0        0        0    41750 2018-11-19 20:18:14.128737 scanlha-0.5/docs/MergeLHA.m.html
--rw-r--r--   0        0        0   173820 2018-11-19 20:18:14.222069 scanlha-0.5/docs/PlotLHA.m.html
--rw-r--r--   0        0        0    66298 2018-11-19 20:18:14.245402 scanlha-0.5/docs/ScanLHA.m.html
--rw-r--r--   0        0        0   180179 2018-11-19 20:18:14.342068 scanlha-0.5/docs/config.m.html
--rw-r--r--   0        0        0    47921 2018-11-19 20:18:14.108738 scanlha-0.5/docs/index.html
--rw-r--r--   0        0        0   277823 2018-11-19 20:18:14.528731 scanlha-0.5/docs/runner.m.html
--rw-r--r--   0        0        0   178199 2018-11-19 20:18:14.618730 scanlha-0.5/docs/scan.m.html
--rw-r--r--   0        0        0    57629 2018-11-19 20:18:14.638730 scanlha-0.5/docs/slha.m.html
--rwxr-xr-x   0        0        0      214 2018-11-19 19:18:33.567929 scanlha-0.5/makedocs
--rw-r--r--   0        0        0      647 2018-11-19 20:56:27.058492 scanlha-0.5/pyproject.toml
--rw-r--r--   0        0        0     9078 1970-01-01 00:00:00.000000 scanlha-0.5/PKG-INFO
+-rw-r--r--   0        0        0       19 2018-11-19 19:22:15.413651 scanlha-0.6/.gitattributes
+-rw-r--r--   0        0        0       82 2024-05-23 19:57:21.369862 scanlha-0.6/.gitignore
+-rw-r--r--   0        0        0       13 2018-07-21 00:32:14.277115 scanlha-0.6/.pylintrc
+-rw-r--r--   0        0        0    32422 2018-08-04 11:55:53.638442 scanlha-0.6/LICENSE
+-rw-r--r--   0        0        0     8540 2018-11-19 20:18:13.295416 scanlha-0.6/README.md
+-rw-r--r--   0        0        0     1965 2021-04-29 07:22:05.208171 scanlha-0.6/ScanLHA/EditLHA.py
+-rw-r--r--   0        0        0     2254 2024-04-05 22:53:33.065780 scanlha-0.6/ScanLHA/MergeLHA.py
+-rw-r--r--   0        0        0    19235 2024-04-05 22:53:33.065780 scanlha-0.6/ScanLHA/PlotLHA.py
+-rw-r--r--   0        0        0     5317 2018-12-01 16:18:46.019182 scanlha-0.6/ScanLHA/ScanLHA.py
+-rw-r--r--   0        0        0     8947 2024-05-23 19:56:40.796529 scanlha-0.6/ScanLHA/__init__.py
+-rw-r--r--   0        0        0    14569 2024-04-05 22:53:33.065780 scanlha-0.6/ScanLHA/config.py
+-rw-r--r--   0        0        0     2126 2018-10-27 18:59:54.551599 scanlha-0.6/ScanLHA/configs/SPheno.yml
+-rw-r--r--   0        0        0    14960 2021-04-29 07:22:05.211504 scanlha-0.6/ScanLHA/runner.py
+-rw-r--r--   0        0        0    11935 2021-04-29 07:22:05.211504 scanlha-0.6/ScanLHA/scan.py
+-rw-r--r--   0        0        0     4849 2024-05-23 19:56:40.799863 scanlha-0.6/ScanLHA/slha.py
+-rw-r--r--   0        0        0    36811 2018-11-19 20:18:14.118738 scanlha-0.6/docs/EditLHA.m.html
+-rw-r--r--   0        0        0    41750 2018-11-19 20:18:14.128737 scanlha-0.6/docs/MergeLHA.m.html
+-rw-r--r--   0        0        0   173820 2018-11-19 20:18:14.222069 scanlha-0.6/docs/PlotLHA.m.html
+-rw-r--r--   0        0        0    66298 2018-11-19 20:18:14.245402 scanlha-0.6/docs/ScanLHA.m.html
+-rw-r--r--   0        0        0   180179 2018-11-19 20:18:14.342068 scanlha-0.6/docs/config.m.html
+-rw-r--r--   0        0        0    47921 2018-11-19 20:18:14.108738 scanlha-0.6/docs/index.html
+-rw-r--r--   0        0        0   277823 2018-11-19 20:18:14.528731 scanlha-0.6/docs/runner.m.html
+-rw-r--r--   0        0        0   178199 2018-11-19 20:18:14.618730 scanlha-0.6/docs/scan.m.html
+-rw-r--r--   0        0        0    57629 2018-11-19 20:18:14.638730 scanlha-0.6/docs/slha.m.html
+-rwxr-xr-x   0        0        0      214 2018-11-19 19:18:33.567929 scanlha-0.6/makedocs
+-rw-r--r--   0        0        0      647 2018-11-19 20:56:27.058492 scanlha-0.6/pyproject.toml
+-rw-r--r--   0        0        0     9078 1970-01-01 00:00:00.000000 scanlha-0.6/PKG-INFO
```

### Comparing `scanlha-0.5/LICENSE` & `scanlha-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/README.md` & `scanlha-0.6/README.md`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/ScanLHA/EditLHA.py` & `scanlha-0.6/ScanLHA/EditLHA.py`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/ScanLHA/MergeLHA.py` & `scanlha-0.6/ScanLHA/MergeLHA.py`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/ScanLHA/PlotLHA.py` & `scanlha-0.6/ScanLHA/PlotLHA.py`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/ScanLHA/ScanLHA.py` & `scanlha-0.6/ScanLHA/ScanLHA.py`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/ScanLHA/__init__.py` & `scanlha-0.6/ScanLHA/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,9 +163,9 @@
  * ask me if you wish to be listed here
 
 """
 from .scan import Scan, RandomScan, FileScan
 from .config import Config
 from  .runner import RUNNERS
 from  .slha import genSLHA, parseSLHA
-__version__ = '0.5'
+__version__ = '0.6'
 __all__ = []
```

### Comparing `scanlha-0.5/ScanLHA/config.py` & `scanlha-0.6/ScanLHA/config.py`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/ScanLHA/configs/SPheno.yml` & `scanlha-0.6/ScanLHA/configs/SPheno.yml`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/ScanLHA/runner.py` & `scanlha-0.6/ScanLHA/runner.py`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/ScanLHA/scan.py` & `scanlha-0.6/ScanLHA/scan.py`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/ScanLHA/slha.py` & `scanlha-0.6/ScanLHA/slha.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     try:
         with open(slhafile,'r') as f:
             if separator:
                 contents = f.read().split(separator)
                 slha = [pylha.load(c.replace('DECAY1L', 'NLODECAY')) for c in contents if c.strip()]
             else:
-                slha = [pylha.load(slhafile)]
+                slha = [pylha.load(f)]
     except FileNotFoundError:
         logging.error('File %s not found.' % slhafile)
         return {}
     except:
         logging.error('Could not parse %s !' % slhafile)
         return {}
```

### Comparing `scanlha-0.5/docs/EditLHA.m.html` & `scanlha-0.6/docs/EditLHA.m.html`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/docs/MergeLHA.m.html` & `scanlha-0.6/docs/MergeLHA.m.html`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/docs/PlotLHA.m.html` & `scanlha-0.6/docs/PlotLHA.m.html`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/docs/ScanLHA.m.html` & `scanlha-0.6/docs/ScanLHA.m.html`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/docs/config.m.html` & `scanlha-0.6/docs/config.m.html`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/docs/index.html` & `scanlha-0.6/docs/index.html`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/docs/runner.m.html` & `scanlha-0.6/docs/runner.m.html`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/docs/scan.m.html` & `scanlha-0.6/docs/scan.m.html`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/docs/slha.m.html` & `scanlha-0.6/docs/slha.m.html`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/pyproject.toml` & `scanlha-0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scanlha-0.5/PKG-INFO` & `scanlha-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScanLHA
-Version: 0.5
+Version: 0.6
 Summary: Perform parameter scans with HEP tools that use (not only) (S)LHA in- and output.
 Home-page: https://github.com/martingabelmann/ScanLHA
 Author: Martin Gabelmann
 Author-email: martin@gabelmann.biz
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: pylha
```

