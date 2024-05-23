# Comparing `tmp/thema-0.1.0.tar.gz` & `tmp/thema-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thema-0.1.0.tar", max compression
+gzip compressed data, was "thema-0.1.1.tar", max compression
```

## Comparing `thema-0.1.0.tar` & `thema-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    13690 2024-05-15 22:54:34.714820 thema-0.1.0/LICENSE.md
--rw-r--r--   0        0        0       56 2024-05-20 21:04:36.076772 thema-0.1.0/README.md
--rw-r--r--   0        0        0      857 2024-05-20 21:04:36.081161 thema-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       67 2024-05-20 21:04:36.092285 thema-0.1.0/thema/__init__.py
--rw-r--r--   0        0        0     5513 2024-05-20 21:04:36.093771 thema-0.1.0/thema/config.py
--rw-r--r--   0        0        0     9151 2024-05-20 21:04:36.094484 thema-0.1.0/thema/core.py
--rw-r--r--   0        0        0      185 2024-05-20 21:04:36.094663 thema-0.1.0/thema/multiverse/__init__.py
--rw-r--r--   0        0        0     9864 2024-05-20 21:04:36.095872 thema-0.1.0/thema/multiverse/system/inner/inner_utils.py
--rw-r--r--   0        0        0     7190 2024-05-20 21:04:36.096553 thema-0.1.0/thema/multiverse/system/inner/moon.py
--rw-r--r--   0        0        0    21301 2024-05-20 21:04:36.097282 thema-0.1.0/thema/multiverse/system/inner/planet.py
--rw-r--r--   0        0        0     2749 2024-05-20 21:04:36.097892 thema-0.1.0/thema/multiverse/system/outer/comet.py
--rw-r--r--   0        0        0    13750 2024-05-20 21:04:36.098622 thema-0.1.0/thema/multiverse/system/outer/oort.py
--rw-r--r--   0        0        0     2323 2024-05-20 21:04:36.099577 thema-0.1.0/thema/multiverse/system/outer/projectiles/pcaProj.py
--rw-r--r--   0        0        0     2463 2024-05-20 21:04:36.100216 thema-0.1.0/thema/multiverse/system/outer/projectiles/tsneProj.py
--rw-r--r--   0        0        0     2811 2024-05-20 21:04:36.100763 thema-0.1.0/thema/multiverse/system/outer/projectiles/umapProj.py
--rw-r--r--   0        0        0    17189 2024-05-20 21:04:36.102031 thema-0.1.0/thema/multiverse/universe/galaxy.py
--rw-r--r--   0        0        0     3216 2024-05-20 21:04:36.103184 thema-0.1.0/thema/multiverse/universe/geodesics.py
--rw-r--r--   0        0        0     2283 2024-05-20 21:04:36.103934 thema-0.1.0/thema/multiverse/universe/star.py
--rw-r--r--   0        0        0     6526 2024-05-20 21:04:36.104883 thema-0.1.0/thema/multiverse/universe/starGraph.py
--rw-r--r--   0        0        0      169 2024-05-20 21:04:36.105938 thema-0.1.0/thema/multiverse/universe/starSelectors.py
--rw-r--r--   0        0        0    11388 2024-05-20 21:04:36.106873 thema-0.1.0/thema/multiverse/universe/stars/jmapStar.py
--rw-r--r--   0        0        0      166 2024-05-20 21:04:36.107111 thema-0.1.0/thema/probe/__init__.py
--rw-r--r--   0        0        0     9678 2024-05-20 21:04:36.108167 thema-0.1.0/thema/probe/data_utils.py
--rw-r--r--   0        0        0    22921 2024-05-20 21:04:36.109063 thema-0.1.0/thema/probe/observatories/jmapObservatory.py
--rw-r--r--   0        0        0     4932 2024-05-20 21:04:36.110248 thema-0.1.0/thema/probe/observatory.py
--rw-r--r--   0        0        0    22100 2024-05-20 21:04:36.111781 thema-0.1.0/thema/probe/telescope.py
--rw-r--r--   0        0        0     7151 2024-05-20 21:04:36.112304 thema-0.1.0/thema/probe/visual_utils.py
--rw-r--r--   0        0        0     5923 2024-05-20 21:04:36.112933 thema-0.1.0/thema/utils.py
--rw-r--r--   0        0        0     1234 1970-01-01 00:00:00.000000 thema-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    13690 2024-05-15 22:54:34.714820 thema-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     3862 2024-05-23 06:39:05.671417 thema-0.1.1/README.md
+-rw-r--r--   0        0        0      857 2024-05-23 06:41:43.325832 thema-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       67 2024-05-20 21:04:36.092285 thema-0.1.1/thema/__init__.py
+-rw-r--r--   0        0        0     5513 2024-05-20 21:04:36.093771 thema-0.1.1/thema/config.py
+-rw-r--r--   0        0        0     9151 2024-05-20 21:04:36.094484 thema-0.1.1/thema/core.py
+-rw-r--r--   0        0        0      185 2024-05-20 21:04:36.094663 thema-0.1.1/thema/multiverse/__init__.py
+-rw-r--r--   0        0        0     9864 2024-05-20 21:04:36.095872 thema-0.1.1/thema/multiverse/system/inner/inner_utils.py
+-rw-r--r--   0        0        0     7190 2024-05-20 21:04:36.096553 thema-0.1.1/thema/multiverse/system/inner/moon.py
+-rw-r--r--   0        0        0    21301 2024-05-20 21:04:36.097282 thema-0.1.1/thema/multiverse/system/inner/planet.py
+-rw-r--r--   0        0        0     2749 2024-05-20 21:04:36.097892 thema-0.1.1/thema/multiverse/system/outer/comet.py
+-rw-r--r--   0        0        0    13750 2024-05-20 21:04:36.098622 thema-0.1.1/thema/multiverse/system/outer/oort.py
+-rw-r--r--   0        0        0     2323 2024-05-20 21:04:36.099577 thema-0.1.1/thema/multiverse/system/outer/projectiles/pcaProj.py
+-rw-r--r--   0        0        0     2463 2024-05-20 21:04:36.100216 thema-0.1.1/thema/multiverse/system/outer/projectiles/tsneProj.py
+-rw-r--r--   0        0        0     2811 2024-05-20 21:04:36.100763 thema-0.1.1/thema/multiverse/system/outer/projectiles/umapProj.py
+-rw-r--r--   0        0        0    17189 2024-05-20 21:04:36.102031 thema-0.1.1/thema/multiverse/universe/galaxy.py
+-rw-r--r--   0        0        0     3216 2024-05-20 21:04:36.103184 thema-0.1.1/thema/multiverse/universe/geodesics.py
+-rw-r--r--   0        0        0     2283 2024-05-20 21:04:36.103934 thema-0.1.1/thema/multiverse/universe/star.py
+-rw-r--r--   0        0        0     6526 2024-05-20 21:04:36.104883 thema-0.1.1/thema/multiverse/universe/starGraph.py
+-rw-r--r--   0        0        0      169 2024-05-20 21:04:36.105938 thema-0.1.1/thema/multiverse/universe/starSelectors.py
+-rw-r--r--   0        0        0    11388 2024-05-20 21:04:36.106873 thema-0.1.1/thema/multiverse/universe/stars/jmapStar.py
+-rw-r--r--   0        0        0      166 2024-05-20 21:04:36.107111 thema-0.1.1/thema/probe/__init__.py
+-rw-r--r--   0        0        0     9678 2024-05-20 21:04:36.108167 thema-0.1.1/thema/probe/data_utils.py
+-rw-r--r--   0        0        0    22921 2024-05-20 21:04:36.109063 thema-0.1.1/thema/probe/observatories/jmapObservatory.py
+-rw-r--r--   0        0        0     4932 2024-05-20 21:04:36.110248 thema-0.1.1/thema/probe/observatory.py
+-rw-r--r--   0        0        0    22100 2024-05-20 21:04:36.111781 thema-0.1.1/thema/probe/telescope.py
+-rw-r--r--   0        0        0     7151 2024-05-20 21:04:36.112304 thema-0.1.1/thema/probe/visual_utils.py
+-rw-r--r--   0        0        0     5923 2024-05-20 21:04:36.112933 thema-0.1.1/thema/utils.py
+-rw-r--r--   0        0        0     5040 1970-01-01 00:00:00.000000 thema-0.1.1/PKG-INFO
```

### Comparing `thema-0.1.0/LICENSE.md` & `thema-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/pyproject.toml` & `thema-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thema"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = [
     "jeremy.wayland <jeremy.don.wayland@gmail.com>",
     "stuart.wayland <swayland@ucsc.edu>",
     "sid.gathrid <sgathrid@yahoo.com>",
 ]
 readme = "README.md"
```

### Comparing `thema-0.1.0/thema/config.py` & `thema-0.1.1/thema/config.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/core.py` & `thema-0.1.1/thema/core.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/system/inner/inner_utils.py` & `thema-0.1.1/thema/multiverse/system/inner/inner_utils.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/system/inner/moon.py` & `thema-0.1.1/thema/multiverse/system/inner/moon.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/system/inner/planet.py` & `thema-0.1.1/thema/multiverse/system/inner/planet.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/system/outer/comet.py` & `thema-0.1.1/thema/multiverse/system/outer/comet.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/system/outer/oort.py` & `thema-0.1.1/thema/multiverse/system/outer/oort.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/system/outer/projectiles/pcaProj.py` & `thema-0.1.1/thema/multiverse/system/outer/projectiles/pcaProj.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/system/outer/projectiles/tsneProj.py` & `thema-0.1.1/thema/multiverse/system/outer/projectiles/tsneProj.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/system/outer/projectiles/umapProj.py` & `thema-0.1.1/thema/multiverse/system/outer/projectiles/umapProj.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/universe/galaxy.py` & `thema-0.1.1/thema/multiverse/universe/galaxy.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/universe/geodesics.py` & `thema-0.1.1/thema/multiverse/universe/geodesics.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/universe/star.py` & `thema-0.1.1/thema/multiverse/universe/star.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/universe/starGraph.py` & `thema-0.1.1/thema/multiverse/universe/starGraph.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/multiverse/universe/stars/jmapStar.py` & `thema-0.1.1/thema/multiverse/universe/stars/jmapStar.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/probe/data_utils.py` & `thema-0.1.1/thema/probe/data_utils.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/probe/observatories/jmapObservatory.py` & `thema-0.1.1/thema/probe/observatories/jmapObservatory.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/probe/observatory.py` & `thema-0.1.1/thema/probe/observatory.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/probe/telescope.py` & `thema-0.1.1/thema/probe/telescope.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/probe/visual_utils.py` & `thema-0.1.1/thema/probe/visual_utils.py`

 * *Files identical despite different names*

### Comparing `thema-0.1.0/thema/utils.py` & `thema-0.1.1/thema/utils.py`

 * *Files identical despite different names*

