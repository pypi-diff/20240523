# Comparing `tmp/cdt_path-2.0.1.tar.gz` & `tmp/cdt_path-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdt_path-2.0.1.tar", last modified: Thu May 23 07:27:50 2024, max compression
+gzip compressed data, was "cdt_path-2.1.1.tar", last modified: Thu May 23 14:57:38 2024, max compression
```

## Comparing `cdt_path-2.0.1.tar` & `cdt_path-2.1.1.tar`

### file list

```diff
@@ -1,59 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 07:27:50.328597 cdt_path-2.0.1/
--rw-rw-rw-   0        0        0      810 2024-05-23 07:27:50.326912 cdt_path-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      100 2024-05-23 07:09:32.000000 cdt_path-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 07:27:50.284720 cdt_path-2.0.1/cdt_path/
--rw-rw-rw-   0        0        0      546 2024-05-23 03:29:44.000000 cdt_path-2.0.1/cdt_path/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:27:50.284720 cdt_path-2.0.1/cdt_path/baseDCEL/
--rw-rw-rw-   0        0        0        0 2024-05-09 12:33:53.000000 cdt_path-2.0.1/cdt_path/baseDCEL/__init__.py
--rw-rw-rw-   0        0        0     2696 2024-05-10 05:21:14.000000 cdt_path-2.0.1/cdt_path/baseDCEL/definition.py
--rw-rw-rw-   0        0        0     2418 2024-05-09 12:53:27.000000 cdt_path-2.0.1/cdt_path/baseDCEL/test.py
--rw-rw-rw-   0        0        0     2548 2024-05-10 05:26:14.000000 cdt_path-2.0.1/cdt_path/baseDCEL/test2.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:27:50.284720 cdt_path-2.0.1/cdt_path/circumcircle/
--rw-rw-rw-   0        0        0        0 2024-05-14 14:48:14.000000 cdt_path-2.0.1/cdt_path/circumcircle/__init__.py
--rw-rw-rw-   0        0        0      648 2024-05-15 06:54:49.000000 cdt_path-2.0.1/cdt_path/circumcircle/calculate.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:27:50.296355 cdt_path-2.0.1/cdt_path/constrained_delaunay/
--rw-rw-rw-   0        0        0        0 2024-05-06 01:15:42.000000 cdt_path-2.0.1/cdt_path/constrained_delaunay/__init__.py
--rw-rw-rw-   0        0        0      117 2024-05-09 06:46:10.000000 cdt_path-2.0.1/cdt_path/constrained_delaunay/cdt_edge_additions.py
--rw-rw-rw-   0        0        0      352 2024-05-06 01:33:01.000000 cdt_path-2.0.1/cdt_path/constrained_delaunay/definition.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:27:50.305852 cdt_path-2.0.1/cdt_path/convex_hull/
--rw-rw-rw-   0        0        0      181 2024-04-13 02:40:26.000000 cdt_path-2.0.1/cdt_path/convex_hull/__init__.py
--rw-rw-rw-   0        0        0      202 2024-04-11 22:13:16.000000 cdt_path-2.0.1/cdt_path/convex_hull/display.py
--rw-rw-rw-   0        0        0     4543 2024-04-11 22:13:16.000000 cdt_path-2.0.1/cdt_path/convex_hull/divide_and_conquer.py
--rw-rw-rw-   0        0        0     1321 2024-04-11 22:13:16.000000 cdt_path-2.0.1/cdt_path/convex_hull/extreme_edge.py
--rw-rw-rw-   0        0        0     1225 2024-04-11 22:13:16.000000 cdt_path-2.0.1/cdt_path/convex_hull/gift_wrap.py
--rw-rw-rw-   0        0        0     4325 2024-05-06 15:05:43.000000 cdt_path-2.0.1/cdt_path/convex_hull/incremental.py
--rw-rw-rw-   0        0        0     1238 2024-04-11 22:13:16.000000 cdt_path-2.0.1/cdt_path/convex_hull/quick_hull.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:27:50.310343 cdt_path-2.0.1/cdt_path/delaunay/
--rw-rw-rw-   0        0        0       78 2024-04-18 11:20:20.000000 cdt_path-2.0.1/cdt_path/delaunay/__init__.py
--rw-rw-rw-   0        0        0     1219 2024-05-06 01:27:54.000000 cdt_path-2.0.1/cdt_path/delaunay/definition.py
--rw-rw-rw-   0        0        0     1080 2024-04-14 14:36:46.000000 cdt_path-2.0.1/cdt_path/delaunay/definition_Old_2.py
--rw-rw-rw-   0        0        0       75 2024-04-18 11:17:22.000000 cdt_path-2.0.1/cdt_path/delaunay/hhh.py
--rw-rw-rw-   0        0        0     3577 2024-04-15 03:58:05.000000 cdt_path-2.0.1/cdt_path/delaunay/incremental.py
--rw-rw-rw-   0        0        0     8444 2024-04-14 14:34:03.000000 cdt_path-2.0.1/cdt_path/delaunay/incremental_Old.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:27:50.311985 cdt_path-2.0.1/cdt_path/file/
--rw-rw-rw-   0        0        0       19 2024-05-22 13:26:45.000000 cdt_path-2.0.1/cdt_path/file/__init__.py
--rw-rw-rw-   0        0        0      116 2024-05-22 13:28:55.000000 cdt_path-2.0.1/cdt_path/file/load.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:27:50.320431 cdt_path-2.0.1/cdt_path/interact/
--rw-rw-rw-   0        0        0       42 2024-05-23 03:24:46.000000 cdt_path-2.0.1/cdt_path/interact/__init__.py
--rw-rw-rw-   0        0        0     3490 2024-05-23 03:28:26.000000 cdt_path-2.0.1/cdt_path/interact/base.py
--rw-rw-rw-   0        0        0      257 2024-05-23 03:30:04.000000 cdt_path-2.0.1/cdt_path/interact/border.py
--rw-rw-rw-   0        0        0     1523 2024-05-16 08:58:29.000000 cdt_path-2.0.1/cdt_path/interact/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:27:50.322090 cdt_path-2.0.1/cdt_path/manipulate/
--rw-rw-rw-   0        0        0       22 2024-05-21 13:38:19.000000 cdt_path-2.0.1/cdt_path/manipulate/__init__.py
--rw-rw-rw-   0        0        0     1000 2024-05-21 13:44:41.000000 cdt_path-2.0.1/cdt_path/manipulate/combine.py
--rw-rw-rw-   0        0        0       14 2024-05-12 06:05:36.000000 cdt_path-2.0.1/cdt_path/manipulate/save.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:27:50.325910 cdt_path-2.0.1/cdt_path/pathplan/
--rw-rw-rw-   0        0        0     2124 2024-05-22 07:13:12.000000 cdt_path-2.0.1/cdt_path/pathplan/A_star.py
--rw-rw-rw-   0        0        0     1373 2024-05-05 11:19:13.000000 cdt_path-2.0.1/cdt_path/pathplan/A_star_O.py
--rw-rw-rw-   0        0        0       68 2024-05-22 13:51:17.000000 cdt_path-2.0.1/cdt_path/pathplan/__init__.py
--rw-rw-rw-   0        0        0     1300 2024-05-22 13:01:38.000000 cdt_path-2.0.1/cdt_path/pathplan/funnel - 副本.py
--rw-rw-rw-   0        0        0     1300 2024-05-22 13:01:38.000000 cdt_path-2.0.1/cdt_path/pathplan/funnel.py
--rw-rw-rw-   0        0        0     1293 2024-05-22 13:51:02.000000 cdt_path-2.0.1/cdt_path/pathplan/utils.py
--rw-rw-rw-   0        0        0     2328 2024-04-11 22:13:16.000000 cdt_path-2.0.1/cdt_path/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:27:50.284720 cdt_path-2.0.1/cdt_path.egg-info/
--rw-rw-rw-   0        0        0      810 2024-05-23 07:27:50.000000 cdt_path-2.0.1/cdt_path.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1382 2024-05-23 07:27:50.000000 cdt_path-2.0.1/cdt_path.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 07:27:50.000000 cdt_path-2.0.1/cdt_path.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 07:27:50.000000 cdt_path-2.0.1/cdt_path.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 07:27:50.328597 cdt_path-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1036 2024-05-23 07:25:33.000000 cdt_path-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.953777 cdt_path-2.1.1/
+-rw-rw-rw-   0        0        0      795 2024-05-23 14:57:38.953777 cdt_path-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2024-05-23 07:09:32.000000 cdt_path-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.922524 cdt_path-2.1.1/cdt_path/
+-rw-rw-rw-   0        0        0      546 2024-05-23 03:29:44.000000 cdt_path-2.1.1/cdt_path/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.922524 cdt_path-2.1.1/cdt_path/circumcircle/
+-rw-rw-rw-   0        0        0        0 2024-05-14 14:48:14.000000 cdt_path-2.1.1/cdt_path/circumcircle/__init__.py
+-rw-rw-rw-   0        0        0      648 2024-05-15 06:54:49.000000 cdt_path-2.1.1/cdt_path/circumcircle/calculate.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.922524 cdt_path-2.1.1/cdt_path/constrained_delaunay/
+-rw-rw-rw-   0        0        0        0 2024-05-06 01:15:42.000000 cdt_path-2.1.1/cdt_path/constrained_delaunay/__init__.py
+-rw-rw-rw-   0        0        0      117 2024-05-09 06:46:10.000000 cdt_path-2.1.1/cdt_path/constrained_delaunay/cdt_edge_additions.py
+-rw-rw-rw-   0        0        0      352 2024-05-06 01:33:01.000000 cdt_path-2.1.1/cdt_path/constrained_delaunay/definition.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.938151 cdt_path-2.1.1/cdt_path/convex_hull/
+-rw-rw-rw-   0        0        0      181 2024-04-13 02:40:26.000000 cdt_path-2.1.1/cdt_path/convex_hull/__init__.py
+-rw-rw-rw-   0        0        0      202 2024-04-11 22:13:16.000000 cdt_path-2.1.1/cdt_path/convex_hull/display.py
+-rw-rw-rw-   0        0        0     4543 2024-04-11 22:13:16.000000 cdt_path-2.1.1/cdt_path/convex_hull/divide_and_conquer.py
+-rw-rw-rw-   0        0        0     1321 2024-04-11 22:13:16.000000 cdt_path-2.1.1/cdt_path/convex_hull/extreme_edge.py
+-rw-rw-rw-   0        0        0     1225 2024-04-11 22:13:16.000000 cdt_path-2.1.1/cdt_path/convex_hull/gift_wrap.py
+-rw-rw-rw-   0        0        0     4325 2024-05-06 15:05:43.000000 cdt_path-2.1.1/cdt_path/convex_hull/incremental.py
+-rw-rw-rw-   0        0        0     1238 2024-04-11 22:13:16.000000 cdt_path-2.1.1/cdt_path/convex_hull/quick_hull.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.938151 cdt_path-2.1.1/cdt_path/delaunay/
+-rw-rw-rw-   0        0        0       78 2024-04-18 11:20:20.000000 cdt_path-2.1.1/cdt_path/delaunay/__init__.py
+-rw-rw-rw-   0        0        0     1219 2024-05-06 01:27:54.000000 cdt_path-2.1.1/cdt_path/delaunay/definition.py
+-rw-rw-rw-   0        0        0     1080 2024-04-14 14:36:46.000000 cdt_path-2.1.1/cdt_path/delaunay/definition_Old_2.py
+-rw-rw-rw-   0        0        0       75 2024-04-18 11:17:22.000000 cdt_path-2.1.1/cdt_path/delaunay/hhh.py
+-rw-rw-rw-   0        0        0     3577 2024-04-15 03:58:05.000000 cdt_path-2.1.1/cdt_path/delaunay/incremental.py
+-rw-rw-rw-   0        0        0     8444 2024-04-14 14:34:03.000000 cdt_path-2.1.1/cdt_path/delaunay/incremental_Old.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.938151 cdt_path-2.1.1/cdt_path/file/
+-rw-rw-rw-   0        0        0       19 2024-05-22 13:26:45.000000 cdt_path-2.1.1/cdt_path/file/__init__.py
+-rw-rw-rw-   0        0        0      116 2024-05-22 13:28:55.000000 cdt_path-2.1.1/cdt_path/file/load.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.938151 cdt_path-2.1.1/cdt_path/interact/
+-rw-rw-rw-   0        0        0       66 2024-05-23 14:55:55.000000 cdt_path-2.1.1/cdt_path/interact/__init__.py
+-rw-rw-rw-   0        0        0     3628 2024-05-23 12:04:51.000000 cdt_path-2.1.1/cdt_path/interact/base.py
+-rw-rw-rw-   0        0        0      257 2024-05-23 03:30:04.000000 cdt_path-2.1.1/cdt_path/interact/border.py
+-rw-rw-rw-   0        0        0     1285 2024-05-23 14:54:44.000000 cdt_path-2.1.1/cdt_path/interact/draw.py
+-rw-rw-rw-   0        0        0     1523 2024-05-16 08:58:29.000000 cdt_path-2.1.1/cdt_path/interact/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.953777 cdt_path-2.1.1/cdt_path/manipulate/
+-rw-rw-rw-   0        0        0       22 2024-05-21 13:38:19.000000 cdt_path-2.1.1/cdt_path/manipulate/__init__.py
+-rw-rw-rw-   0        0        0     1000 2024-05-21 13:44:41.000000 cdt_path-2.1.1/cdt_path/manipulate/combine.py
+-rw-rw-rw-   0        0        0       14 2024-05-12 06:05:36.000000 cdt_path-2.1.1/cdt_path/manipulate/save.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.953777 cdt_path-2.1.1/cdt_path/pathplan/
+-rw-rw-rw-   0        0        0     3452 2024-05-23 11:51:41.000000 cdt_path-2.1.1/cdt_path/pathplan/A_star.py
+-rw-rw-rw-   0        0        0     1373 2024-05-05 11:19:13.000000 cdt_path-2.1.1/cdt_path/pathplan/A_star_O.py
+-rw-rw-rw-   0        0        0       68 2024-05-22 13:51:17.000000 cdt_path-2.1.1/cdt_path/pathplan/__init__.py
+-rw-rw-rw-   0        0        0     1300 2024-05-22 13:01:38.000000 cdt_path-2.1.1/cdt_path/pathplan/funnel - 副本.py
+-rw-rw-rw-   0        0        0     1300 2024-05-22 13:01:38.000000 cdt_path-2.1.1/cdt_path/pathplan/funnel.py
+-rw-rw-rw-   0        0        0     1293 2024-05-22 13:51:02.000000 cdt_path-2.1.1/cdt_path/pathplan/utils.py
+-rw-rw-rw-   0        0        0     2328 2024-04-11 22:13:16.000000 cdt_path-2.1.1/cdt_path/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.922524 cdt_path-2.1.1/cdt_path.egg-info/
+-rw-rw-rw-   0        0        0      795 2024-05-23 14:57:38.000000 cdt_path-2.1.1/cdt_path.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1324 2024-05-23 14:57:38.000000 cdt_path-2.1.1/cdt_path.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:57:38.000000 cdt_path-2.1.1/cdt_path.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-23 14:57:38.000000 cdt_path-2.1.1/cdt_path.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 14:57:38.000000 cdt_path-2.1.1/cdt_path.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:57:38.953777 cdt_path-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1073 2024-05-23 14:56:45.000000 cdt_path-2.1.1/setup.py
```

### Comparing `cdt_path-2.0.1/PKG-INFO` & `cdt_path-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: cdt_path
-Version: 2.0.1
-Summary: CDT for path-planning
+Version: 2.1.1
+Summary: Constrainted Delaunay Triangle for path-planning
 Author: CaiShu
 Author-email: caiyi@mail.ustc.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires: matplotlib
-Requires: triangle
 Description-Content-Type: text/markdown
 
 ### 使用约束Delaunay三角来寻路
 
 ### Using Constrained Delaunay Triangle for path-planning
```

### Comparing `cdt_path-2.0.1/cdt_path/__init__.py` & `cdt_path-2.1.1/cdt_path/__init__.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/circumcircle/calculate.py` & `cdt_path-2.1.1/cdt_path/circumcircle/calculate.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/convex_hull/divide_and_conquer.py` & `cdt_path-2.1.1/cdt_path/convex_hull/divide_and_conquer.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/convex_hull/extreme_edge.py` & `cdt_path-2.1.1/cdt_path/convex_hull/extreme_edge.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/convex_hull/gift_wrap.py` & `cdt_path-2.1.1/cdt_path/convex_hull/gift_wrap.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/convex_hull/incremental.py` & `cdt_path-2.1.1/cdt_path/convex_hull/incremental.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/convex_hull/quick_hull.py` & `cdt_path-2.1.1/cdt_path/convex_hull/quick_hull.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/delaunay/definition.py` & `cdt_path-2.1.1/cdt_path/delaunay/definition.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/delaunay/definition_Old_2.py` & `cdt_path-2.1.1/cdt_path/delaunay/definition_Old_2.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/delaunay/incremental.py` & `cdt_path-2.1.1/cdt_path/delaunay/incremental.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/delaunay/incremental_Old.py` & `cdt_path-2.1.1/cdt_path/delaunay/incremental_Old.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/interact/base.py` & `cdt_path-2.1.1/cdt_path/interact/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,18 +97,20 @@
 		
 	def on_click(self, event):
 		if event.inaxes is None or self.trifinder(event.xdata, event.ydata) == -1:
 			return
 		if event.button is MouseButton.LEFT:
 			if self._click_state==0:
 				self._start_point=(event.xdata, event.ydata)
+				self._start_point_in_axes = self.ax.scatter(event.xdata, event.ydata, color='k', marker='*')
 				self._click_state+=1
 				
 			elif self._click_state==1:
 				self._end_point=(event.xdata, event.ydata)
+				self._start_point_in_axes.remove()
 				if self.trifinder(*self._start_point) == self.trifinder(*self._end_point):
 					self._click_state==0
 					return
 				self.updata_path(np.array(self._start_point), np.array(self._end_point))
 				self._click_state+=1
 			elif self._click_state ==2:
 				self.polygon2.set_visible(False)
```

### Comparing `cdt_path-2.0.1/cdt_path/interact/utils.py` & `cdt_path-2.1.1/cdt_path/interact/utils.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/manipulate/combine.py` & `cdt_path-2.1.1/cdt_path/manipulate/combine.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/pathplan/A_star.py` & `cdt_path-2.1.1/cdt_path/pathplan/A_star.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,17 +43,14 @@
 	frontier = PriorityQueue()
 	frontier.put((0,start))
 	graph = Graph_Path(triang)
 	came_from={}
 	cost_so_far={}
 	came_from[start]=None
 	cost_so_far[start]=0
-	trigo = triang.triangles[goal]
-	print(trigo)
-	# goal_cg3 = (graph.x[trigo[0]]+graph.x[trigo[1]]+graph.x[trigo[2]],graph.y[trigo[0]]+graph.y[trigo[1]]+graph.y[trigo[2]])
 	goal_cg3 = graph.cg3(goal)
 	def heuristic(i):
 		cg1=graph.cg3(i)
 		dcgx = cg1[0]-goal_cg3[0]
 		dcgy = cg1[1]-goal_cg3[1]
 		return (dcgx**2 + dcgy**2)**(0.5)
 	
@@ -74,8 +71,61 @@
 				cost_so_far[next]=new_cost
 				#Change heuristic
 				priority = new_cost + heuristic(next)
 				# print("priority ", priority )
 				frontier.put((priority, next))
 				came_from[next] = current
 				
+	return came_from, cost_so_far
+	
+def a_star_P(triang, start_point, goal_point, start=None, goal=None):
+	if start==None or goal==None:
+		trifinder = triang.get_trifinder()
+		start = int(trifinder(*start_point))
+		goal = int(trifinder(*goal_point))
+		del trifinder
+	
+	frontier = PriorityQueue()
+	graph = Graph_Path(triang)
+	
+	def heuristic(i):
+		cg1=graph.cg3(i)
+		dcgx = cg1[0]-goal_point3[0]
+		dcgy = cg1[1]-goal_point3[1]
+		return (dcgx**2 + dcgy**2)**(0.5)
+		
+	came_from={}
+	cost_so_far={}
+	came_from[start]=None
+	cost_so_far[start]=0
+	start_point3 = (start_point[0]*3, start_point[1]*3)
+	goal_point3 = (goal_point[0]*3, goal_point[1]*3)
+	
+	for next in graph.neighbors[start]:
+		if next == -1:
+			continue
+		ncg3=graph.cg3(next)
+		new_cost = ((start_point3[0]-ncg3[0])**2+(start_point3[1]-ncg3[1])**2)**(0.5)
+		cost_so_far[next]=new_cost
+		#Change heuristic
+		priority = new_cost + heuristic(next)
+		frontier.put((priority, next))
+		came_from[next] = start
+			
+	while not frontier.empty():
+		current= frontier.get()[1]
+			
+		if current==goal:
+			break
+			
+		for next in graph.neighbors[current]:
+			if came_from[current]==next or next == -1:
+				continue
+			new_cost = cost_so_far[current] + graph.cost_3(current,next)
+			if next not in cost_so_far or new_cost< cost_so_far[next]:
+				cost_so_far[next]=new_cost
+				#Change heuristic
+				priority = new_cost + heuristic(next)
+				frontier.put((priority, next))
+				came_from[next] = current
+				
 	return came_from, cost_so_far
```

### Comparing `cdt_path-2.0.1/cdt_path/pathplan/A_star_O.py` & `cdt_path-2.1.1/cdt_path/pathplan/A_star_O.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/pathplan/funnel - 副本.py` & `cdt_path-2.1.1/cdt_path/pathplan/funnel - 副本.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/pathplan/funnel.py` & `cdt_path-2.1.1/cdt_path/pathplan/funnel.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/pathplan/utils.py` & `cdt_path-2.1.1/cdt_path/pathplan/utils.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path/utils.py` & `cdt_path-2.1.1/cdt_path/utils.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.0.1/cdt_path.egg-info/PKG-INFO` & `cdt_path-2.1.1/cdt_path.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: cdt-path
-Version: 2.0.1
-Summary: CDT for path-planning
+Version: 2.1.1
+Summary: Constrainted Delaunay Triangle for path-planning
 Author: CaiShu
 Author-email: caiyi@mail.ustc.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires: matplotlib
-Requires: triangle
 Description-Content-Type: text/markdown
 
 ### 使用约束Delaunay三角来寻路
 
 ### Using Constrained Delaunay Triangle for path-planning
```

### Comparing `cdt_path-2.0.1/cdt_path.egg-info/SOURCES.txt` & `cdt_path-2.1.1/cdt_path.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 README.md
 setup.py
 cdt_path/__init__.py
 cdt_path/utils.py
 cdt_path.egg-info/PKG-INFO
 cdt_path.egg-info/SOURCES.txt
 cdt_path.egg-info/dependency_links.txt
+cdt_path.egg-info/requires.txt
 cdt_path.egg-info/top_level.txt
-cdt_path/baseDCEL/__init__.py
-cdt_path/baseDCEL/definition.py
-cdt_path/baseDCEL/test.py
-cdt_path/baseDCEL/test2.py
 cdt_path/circumcircle/__init__.py
 cdt_path/circumcircle/calculate.py
 cdt_path/constrained_delaunay/__init__.py
 cdt_path/constrained_delaunay/cdt_edge_additions.py
 cdt_path/constrained_delaunay/definition.py
 cdt_path/convex_hull/__init__.py
 cdt_path/convex_hull/display.py
@@ -29,14 +26,15 @@
 cdt_path/delaunay/incremental.py
 cdt_path/delaunay/incremental_Old.py
 cdt_path/file/__init__.py
 cdt_path/file/load.py
 cdt_path/interact/__init__.py
 cdt_path/interact/base.py
 cdt_path/interact/border.py
+cdt_path/interact/draw.py
 cdt_path/interact/utils.py
 cdt_path/manipulate/__init__.py
 cdt_path/manipulate/combine.py
 cdt_path/manipulate/save.py
 cdt_path/pathplan/A_star.py
 cdt_path/pathplan/A_star_O.py
 cdt_path/pathplan/__init__.py
```

### Comparing `cdt_path-2.0.1/setup.py` & `cdt_path-2.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="cdt_path",
-    version='2.0.1',
+    version='2.1.1',
     author="CaiShu",
     author_email="caiyi@mail.ustc.edu.cn",
-    description="CDT for path-planning",
+    description="Constrainted Delaunay Triangle for path-planning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # license="MIT",
     # url="https://gitee.com/DerrickChiu/function_tool.git",
     packages=find_packages(),
-    requires=[	'matplotlib',
-				'triangle',
+    install_requires=[	'matplotlib',
+						'triangle',
         ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

