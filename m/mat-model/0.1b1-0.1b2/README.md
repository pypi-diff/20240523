# Comparing `tmp/mat_model-0.1b1.tar.gz` & `tmp/mat_model-0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat_model-0.1b1.tar", last modified: Tue Apr 16 13:30:26 2024, max compression
+gzip compressed data, was "mat_model-0.1b2.tar", last modified: Thu May 23 15:19:45 2024, max compression
```

## Comparing `mat_model-0.1b1.tar` & `mat_model-0.1b2.tar`

### file list

```diff
@@ -1,37 +1,54 @@
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-16 13:30:26.163372 mat_model-0.1b1/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      106 2024-04-10 16:16:51.000000 mat_model-0.1b1/CHANGELOG.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b1/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat_model-0.1b1/MANIFEST.in
--rw-------   0 tarlisportela   (501) staff       (20)    31070 2024-04-15 18:13:37.000000 mat_model-0.1b1/MAT-Tools.drawio
--rwx------   0 tarlisportela   (501) staff       (20)     3081 2024-04-16 13:28:59.000000 mat_model-0.1b1/MAT-model-Tutorial.ipynb
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5015 2024-04-16 13:30:26.163159 mat_model-0.1b1/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b1/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)      719 2024-04-10 16:09:56.000000 mat_model-0.1b1/Steps to Build.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-16 13:30:26.162429 mat_model-0.1b1/mat_model.egg-info/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5015 2024-04-16 13:30:26.000000 mat_model-0.1b1/mat_model.egg-info/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)      688 2024-04-16 13:30:26.000000 mat_model-0.1b1/mat_model.egg-info/SOURCES.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-16 13:30:26.000000 mat_model-0.1b1/mat_model.egg-info/dependency_links.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)      139 2024-04-16 13:30:26.000000 mat_model-0.1b1/mat_model.egg-info/requires.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        9 2024-04-16 13:30:26.000000 mat_model-0.1b1/mat_model.egg-info/top_level.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-16 13:30:26.160029 mat_model-0.1b1/matmodel/
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b1/matmodel/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b1/matmodel/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_model-0.1b1/matmodel/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-16 13:30:26.161543 mat_model-0.1b1/matmodel/base/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3749 2023-09-03 21:43:34.000000 mat_model-0.1b1/matmodel/base/Aspect.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      811 2024-04-16 12:05:57.000000 mat_model-0.1b1/matmodel/base/Feature.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1271 2024-04-16 12:05:30.000000 mat_model-0.1b1/matmodel/base/Movelet.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3654 2024-04-16 12:06:50.000000 mat_model-0.1b1/matmodel/base/MultipleAspectSequence.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4220 2024-04-16 12:05:44.000000 mat_model-0.1b1/matmodel/base/Subtrajectory.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      781 2024-04-16 12:05:49.000000 mat_model-0.1b1/matmodel/base/Trajectory.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-05-02 00:25:10.000000 mat_model-0.1b1/matmodel/base/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-16 13:30:26.162058 mat_model-0.1b1/matmodel/distance/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     8987 2023-09-03 21:18:52.000000 mat_model-0.1b1/matmodel/distance/Comparator.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_model-0.1b1/matmodel/distance/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-16 13:30:26.162278 mat_model-0.1b1/matmodel/evaluation/
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-09-02 21:02:56.000000 mat_model-0.1b1/matmodel/evaluation/Quality.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_model-0.1b1/matmodel/evaluation/__init__.py
--rw-------   0 tarlisportela   (501) staff       (20)    58933 2024-04-12 14:57:32.000000 mat_model-0.1b1/matmodel.drawio
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2117 2024-04-16 13:30:17.000000 mat_model-0.1b1/pyproject.toml
--rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-04-16 13:30:26.163409 mat_model-0.1b1/setup.cfg
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2209 2024-04-10 16:09:27.000000 mat_model-0.1b1/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.226677 mat_model-0.1b2/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      106 2024-04-10 16:16:51.000000 mat_model-0.1b2/CHANGELOG.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b2/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat_model-0.1b2/MANIFEST.in
+-rw-------   0 tarlisportela   (501) staff       (20)    41157 2024-04-19 21:04:47.000000 mat_model-0.1b2/MAT-Tools.drawio
+-rwx------   0 tarlisportela   (501) staff       (20)    26766 2024-05-23 14:21:15.000000 mat_model-0.1b2/MAT-model-Tutorial.ipynb
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5015 2024-05-23 15:19:45.226279 mat_model-0.1b2/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b2/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      719 2024-04-10 16:09:56.000000 mat_model-0.1b2/Steps to Build.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.225401 mat_model-0.1b2/mat_model.egg-info/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5015 2024-05-23 15:19:45.000000 mat_model-0.1b2/mat_model.egg-info/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1126 2024-05-23 15:19:45.000000 mat_model-0.1b2/mat_model.egg-info/SOURCES.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-05-23 15:19:45.000000 mat_model-0.1b2/mat_model.egg-info/dependency_links.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      139 2024-05-23 15:19:45.000000 mat_model-0.1b2/mat_model.egg-info/requires.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        9 2024-05-23 15:19:45.000000 mat_model-0.1b2/mat_model.egg-info/top_level.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.219472 mat_model-0.1b2/matmodel/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b2/matmodel/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b2/matmodel/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_model-0.1b2/matmodel/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.221025 mat_model-0.1b2/matmodel/base/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5094 2024-05-23 15:02:02.000000 mat_model-0.1b2/matmodel/base/Aspect.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2429 2024-04-19 21:37:21.000000 mat_model-0.1b2/matmodel/base/Movelet.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     6959 2024-05-22 19:03:55.000000 mat_model-0.1b2/matmodel/base/MultipleAspectSequence.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       83 2024-04-19 21:39:58.000000 mat_model-0.1b2/matmodel/base/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4430 2024-04-19 15:20:13.000000 mat_model-0.1b2/matmodel/base/xSubtrajectory.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      937 2024-04-19 21:33:09.000000 mat_model-0.1b2/matmodel/base/xTrajectory.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.221519 mat_model-0.1b2/matmodel/descriptor/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       25 2024-04-18 16:09:57.000000 mat_model-0.1b2/matmodel/descriptor/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-05-22 17:16:27.000000 mat_model-0.1b2/matmodel/descriptor/descriptor.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.222632 mat_model-0.1b2/matmodel/distance/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       47 2024-04-18 16:21:07.000000 mat_model-0.1b2/matmodel/distance/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    10303 2024-05-22 19:37:32.000000 mat_model-0.1b2/matmodel/distance/comparator.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-18 16:20:36.000000 mat_model-0.1b2/matmodel/distance/helper.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.223198 mat_model-0.1b2/matmodel/evaluation/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      742 2024-04-19 21:36:51.000000 mat_model-0.1b2/matmodel/evaluation/Feature.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      193 2024-04-17 15:21:31.000000 mat_model-0.1b2/matmodel/evaluation/Quality.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       45 2024-04-19 21:37:58.000000 mat_model-0.1b2/matmodel/evaluation/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.223425 mat_model-0.1b2/matmodel/index/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-19 18:35:46.000000 mat_model-0.1b2/matmodel/index/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.223773 mat_model-0.1b2/matmodel/method/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      701 2024-04-29 14:35:26.000000 mat_model-0.1b2/matmodel/method/MethodWrapper.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      100 2024-04-28 16:21:33.000000 mat_model-0.1b2/matmodel/method/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.224464 mat_model-0.1b2/matmodel/method/classification/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      884 2024-04-29 14:32:53.000000 mat_model-0.1b2/matmodel/method/classification/HiperMovelets.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      567 2024-04-28 16:18:41.000000 mat_model-0.1b2/matmodel/method/classification/MasterMovelets.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      143 2024-05-18 05:05:30.000000 mat_model-0.1b2/matmodel/method/classification/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.225084 mat_model-0.1b2/matmodel/util/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-16 19:42:44.000000 mat_model-0.1b2/matmodel/util/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      271 2024-04-16 20:08:42.000000 mat_model-0.1b2/matmodel/util/filters.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3247 2024-04-19 21:58:05.000000 mat_model-0.1b2/matmodel/util/parsers.py
+-rw-------   0 tarlisportela   (501) staff       (20)    87313 2024-05-23 14:55:08.000000 mat_model-0.1b2/matmodel.drawio
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2117 2024-05-23 15:18:38.000000 mat_model-0.1b2/pyproject.toml
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-05-23 15:19:45.226776 mat_model-0.1b2/setup.cfg
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2209 2024-04-10 16:09:27.000000 mat_model-0.1b2/setup.py
```

### Comparing `mat_model-0.1b1/LICENSE` & `mat_model-0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b1/MAT-Tools.drawio` & `mat_model-0.1b2/MAT-Tools.drawio`

 * *Files 16% similar despite different names*

```diff
@@ -1,160 +1,43 @@
-<mxfile host="app.diagrams.net" modified="2024-04-15T18:13:37.867Z" agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36" etag="GOhE4i7AqAaWFN0QtzYx" version="23.1.5" type="device">
+<mxfile host="app.diagrams.net" modified="2024-04-19T21:04:47.091Z" agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36" etag="ta_-VXOWRiMJUBJplRkV" version="23.1.5" type="device">
   <diagram name="Página-1" id="NjSdwOmiIwXVztQAF8Lo">
-    <mxGraphModel dx="1156" dy="212" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="827" pageHeight="1169" math="0" shadow="0">
+    <mxGraphModel dx="1736" dy="1755" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="827" pageHeight="1169" math="0" shadow="0">
       <root>
         <mxCell id="0" />
         <mxCell id="1" parent="0" />
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-17" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;dashed=1;endArrow=open;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-12" target="n9qyGrMY-b-BzYaa1yog-2" edge="1">
+          <mxGeometry relative="1" as="geometry" />
+        </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-61" value="&lt;h4&gt;Trajectory Input&lt;/h4&gt;" style="rounded=1;whiteSpace=wrap;html=1;fillColor=none;verticalAlign=top;labelPosition=right;verticalLabelPosition=bottom;align=left;spacing=-15;spacingTop=0;spacingLeft=-100;spacingRight=0;fontColor=#0000CC;labelBorderColor=none;strokeColor=#0000CC;arcSize=5;" parent="1" vertex="1">
           <mxGeometry x="2170" y="168" width="180" height="240" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-62" value="&lt;h4&gt;Mixed Input / Ensemble&lt;/h4&gt;" style="rounded=1;whiteSpace=wrap;html=1;fillColor=none;verticalAlign=top;labelPosition=center;verticalLabelPosition=bottom;align=center;spacing=-15;spacingTop=1;spacingLeft=0;spacingRight=0;fontColor=#EBC75E;labelBorderColor=none;strokeColor=#EBC75E;arcSize=12;" parent="1" vertex="1">
           <mxGeometry x="1996" y="254" width="140" height="154" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-60" value="&lt;h4&gt;Feature Input&lt;/h4&gt;" style="rounded=1;whiteSpace=wrap;html=1;fillColor=none;verticalAlign=top;labelPosition=left;verticalLabelPosition=bottom;align=right;spacing=-15;spacingTop=1;spacingLeft=0;spacingRight=-80;fontColor=#009900;labelBorderColor=none;strokeColor=#009900;arcSize=6;" parent="1" vertex="1">
           <mxGeometry x="1670" y="247" width="300" height="160" as="geometry" />
         </mxCell>
-        <mxCell id="mgZLQg_ETMRa4hPbAOP7-5" value="methods" style="shape=folder;fontStyle=1;spacingTop=10;tabWidth=40;tabHeight=14;tabPosition=left;html=1;whiteSpace=wrap;horizontal=1;verticalAlign=top;fillColor=none;" parent="1" vertex="1">
-          <mxGeometry x="260" y="307" width="160" height="436" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-2" value="mat-data" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=110;height=30;" parent="1" vertex="1">
-          <mxGeometry x="150" y="20" width="170" height="190" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-4" value="preprocess" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
-          <mxGeometry x="170" y="96" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-5" value="generator" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
-          <mxGeometry x="170" y="60" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-6" value="mat-view" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=120;height=26;" parent="1" vertex="1">
-          <mxGeometry x="-160" y="274" width="170" height="130" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-7" value="web-app &lt;br&gt;&lt;i&gt;(Movelets &amp;amp; MAT)&lt;/i&gt;" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
-          <mxGeometry x="-140" y="350" width="130" height="41" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-8" value="graphics" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
-          <mxGeometry x="-140" y="314" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-35" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;dashed=1;endFill=0;exitX=0.512;exitY=0;exitDx=0;exitDy=0;exitPerimeter=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-9" target="n9qyGrMY-b-BzYaa1yog-2" edge="1">
-          <mxGeometry relative="1" as="geometry" />
-        </mxCell>
-        <mxCell id="ncjso_DGpGOnADHclqbK-1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;dashed=1;strokeColor=default;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=open;endFill=0;" edge="1" parent="1" source="n9qyGrMY-b-BzYaa1yog-9" target="BebV0c_RTAwMKaFlxQ5s-1">
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-35" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;dashed=1;endFill=0;exitX=0.573;exitY=0.004;exitDx=0;exitDy=0;exitPerimeter=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-9" target="n9qyGrMY-b-BzYaa1yog-2" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-9" value="movelets" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=120;height=25;" parent="1" vertex="1">
-          <mxGeometry x="490" y="285.5" width="170" height="190" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-10" value="MLP (movelets)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="1" vertex="1">
-          <mxGeometry x="270" y="599" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="mgZLQg_ETMRa4hPbAOP7-8" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=1;entryY=0.5;entryDx=0;entryDy=0;endArrow=open;dashed=1;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-11" target="n9qyGrMY-b-BzYaa1yog-21" edge="1">
-          <mxGeometry relative="1" as="geometry">
-            <Array as="points">
-              <mxPoint x="410" y="723" />
-              <mxPoint x="410" y="540" />
-            </Array>
-          </mxGeometry>
-        </mxCell>
-        <mxCell id="mgZLQg_ETMRa4hPbAOP7-9" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=1;entryY=0.5;entryDx=0;entryDy=0;endArrow=open;dashed=1;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-11" target="n9qyGrMY-b-BzYaa1yog-20" edge="1">
-          <mxGeometry relative="1" as="geometry">
-            <Array as="points">
-              <mxPoint x="410" y="723" />
-              <mxPoint x="410" y="577" />
-            </Array>
-          </mxGeometry>
-        </mxCell>
-        <mxCell id="mgZLQg_ETMRa4hPbAOP7-10" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=1;entryY=0.5;entryDx=0;entryDy=0;endArrow=open;dashed=1;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-11" target="n9qyGrMY-b-BzYaa1yog-10" edge="1">
-          <mxGeometry relative="1" as="geometry">
-            <Array as="points">
-              <mxPoint x="410" y="723" />
-              <mxPoint x="410" y="614" />
-            </Array>
-          </mxGeometry>
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-11" value="TEC" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#fff2cc;strokeColor=#d6b656;" parent="1" vertex="1">
-          <mxGeometry x="270" y="708" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-17" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;dashed=1;endArrow=open;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-12" target="n9qyGrMY-b-BzYaa1yog-2" edge="1">
-          <mxGeometry relative="1" as="geometry" />
+          <mxGeometry x="460" y="499" width="170" height="190" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-23" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;dashed=1;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-12" target="n9qyGrMY-b-BzYaa1yog-6" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-33" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;dashed=1;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-12" target="n9qyGrMY-b-BzYaa1yog-19" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-12" value="automatize" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=120;height=27;" parent="1" vertex="1">
-          <mxGeometry x="40" y="273" width="170" height="235" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-13" value="run" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
-          <mxGeometry x="60" y="350" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-14" value="results" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
-          <mxGeometry x="60" y="313" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-16" value="datasets" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
-          <mxGeometry x="60" y="387" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-32" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;dashed=1;endFill=0;exitX=1;exitY=0.202;exitDx=0;exitDy=0;exitPerimeter=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-19" target="n9qyGrMY-b-BzYaa1yog-9" edge="1">
-          <mxGeometry relative="1" as="geometry">
-            <mxPoint x="460" y="362.1250000000001" as="sourcePoint" />
-            <mxPoint x="502.70491803278696" y="297" as="targetPoint" />
-          </mxGeometry>
-        </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-34" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;dashed=1;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-19" target="n9qyGrMY-b-BzYaa1yog-2" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-19" value="mat-classification" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=130;height=27;" parent="1" vertex="1">
-          <mxGeometry x="250" y="273" width="190" height="520" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-20" value="POI-S" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="1" vertex="1">
-          <mxGeometry x="271" y="562" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-21" value="MARC" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
-          <mxGeometry x="271" y="525" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-22" value="web-app" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
-          <mxGeometry x="60" y="425" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-24" value="RF&amp;nbsp; (movelets)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="1" vertex="1">
-          <mxGeometry x="270" y="635" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-25" value="SVM&amp;nbsp;(movelets)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="1" vertex="1">
-          <mxGeometry x="270" y="671" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-26" value="DeepestST" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
-          <mxGeometry x="270" y="341" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-27" value="MAT RF" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
-          <mxGeometry x="270" y="378" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-28" value="MAT XGBoost" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
-          <mxGeometry x="270" y="414" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-29" value="TULVAE" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
-          <mxGeometry x="270" y="451" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-30" value="BITULER" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
-          <mxGeometry x="270" y="488" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-36" value="converter" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
-          <mxGeometry x="170" y="132" width="130" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="mgZLQg_ETMRa4hPbAOP7-1" value="datasets" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
-          <mxGeometry x="170" y="167" width="130" height="30" as="geometry" />
-        </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-2" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;dashed=1;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-6" target="n9qyGrMY-b-BzYaa1yog-2" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
-        <mxCell id="mgZLQg_ETMRa4hPbAOP7-6" value="scripts" style="shape=folder;fontStyle=1;spacingTop=10;tabWidth=40;tabHeight=10;tabPosition=left;html=1;whiteSpace=wrap;" parent="1" vertex="1">
-          <mxGeometry x="274" y="753" width="126" height="30" as="geometry" />
-        </mxCell>
-        <mxCell id="mgZLQg_ETMRa4hPbAOP7-7" value="scripts" style="shape=folder;fontStyle=1;spacingTop=10;tabWidth=40;tabHeight=10;tabPosition=left;html=1;whiteSpace=wrap;" parent="1" vertex="1">
-          <mxGeometry x="65" y="469" width="125" height="30" as="geometry" />
-        </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-38" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-11" target="mgZLQg_ETMRa4hPbAOP7-26" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
               <mxPoint x="1980" y="271" />
             </Array>
           </mxGeometry>
         </mxCell>
@@ -321,23 +204,227 @@
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-66" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-65" target="mgZLQg_ETMRa4hPbAOP7-12" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-65" value="MSTEC" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#fff2cc;strokeColor=#d6b656;" parent="1" vertex="1">
           <mxGeometry x="2001" y="358" width="130" height="30" as="geometry" />
         </mxCell>
-        <mxCell id="BebV0c_RTAwMKaFlxQ5s-1" value="mat-model" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=110;height=30;" parent="1" vertex="1">
-          <mxGeometry x="480" y="66" width="170" height="60" as="geometry" />
+        <mxCell id="ncjso_DGpGOnADHclqbK-24" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;dashed=1;strokeColor=default;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=open;endFill=0;exitX=0.539;exitY=0.001;exitDx=0;exitDy=0;exitPerimeter=0;" edge="1" parent="1" source="ncjso_DGpGOnADHclqbK-2" target="n9qyGrMY-b-BzYaa1yog-2">
+          <mxGeometry relative="1" as="geometry" />
         </mxCell>
-        <mxCell id="ncjso_DGpGOnADHclqbK-2" value="mat-similarity" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=140;height=31;" vertex="1" parent="1">
-          <mxGeometry x="670" y="499" width="170" height="190" as="geometry" />
+        <mxCell id="ncjso_DGpGOnADHclqbK-23" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;dashed=1;strokeColor=default;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=open;endFill=0;" edge="1" parent="1" source="ncjso_DGpGOnADHclqbK-3" target="ncjso_DGpGOnADHclqbK-2">
+          <mxGeometry relative="1" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-25" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;dashed=1;strokeColor=default;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=open;endFill=0;exitX=0.561;exitY=-0.009;exitDx=0;exitDy=0;exitPerimeter=0;" edge="1" parent="1" source="ncjso_DGpGOnADHclqbK-3" target="n9qyGrMY-b-BzYaa1yog-2">
+          <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="ncjso_DGpGOnADHclqbK-3" value="mat-summarization" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=133;height=26;" vertex="1" parent="1">
-          <mxGeometry x="490" y="499" width="170" height="190" as="geometry" />
+          <mxGeometry x="840" y="270" width="170" height="190" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-20" value="" style="group" vertex="1" connectable="0" parent="1">
+          <mxGeometry x="460" y="270" width="170" height="212" as="geometry" />
+        </mxCell>
+        <mxCell id="BebV0c_RTAwMKaFlxQ5s-1" value="mat-model" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=110;height=30;" parent="ncjso_DGpGOnADHclqbK-20" vertex="1">
+          <mxGeometry width="170" height="212" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-15" value="base (MAT)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-20">
+          <mxGeometry x="20" y="38.5" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-16" value="corals" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-20">
+          <mxGeometry x="20" y="72.5" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-17" value="distance" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-20">
+          <mxGeometry x="20" y="107.5" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-18" value="evaluation" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-20">
+          <mxGeometry x="20" y="141.5" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-19" value="index" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-20">
+          <mxGeometry x="20" y="175" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-21" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;dashed=1;strokeColor=default;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=open;endFill=0;exitX=0.545;exitY=-0.001;exitDx=0;exitDy=0;exitPerimeter=0;" edge="1" parent="1" source="BebV0c_RTAwMKaFlxQ5s-1" target="n9qyGrMY-b-BzYaa1yog-2">
+          <mxGeometry relative="1" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-22" value="" style="group" vertex="1" connectable="0" parent="1">
+          <mxGeometry x="1021" y="270" width="170" height="386" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-4" value="mat-clustering" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=133;height=26;" vertex="1" parent="ncjso_DGpGOnADHclqbK-22">
+          <mxGeometry width="170" height="386" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-5" value="agglomerative" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-22">
+          <mxGeometry x="20" y="34.5" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-6" value="corals" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-22">
+          <mxGeometry x="20" y="68.5" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-7" value="dbscan" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-22">
+          <mxGeometry x="20" y="103.5" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-8" value="dhillon" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-22">
+          <mxGeometry x="20" y="137.5" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-9" value="kluger" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-22">
+          <mxGeometry x="20" y="171" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-10" value="kmeans" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-22">
+          <mxGeometry x="20" y="205" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-11" value="mattree" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-22">
+          <mxGeometry x="20" y="240" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-12" value="ococlus" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-22">
+          <mxGeometry x="20" y="274" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-13" value="panda" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-22">
+          <mxGeometry x="20" y="308" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-14" value="tracoclus" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-22">
+          <mxGeometry x="20" y="342" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-26" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;dashed=1;strokeColor=default;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=open;endFill=0;exitX=0.598;exitY=-0.002;exitDx=0;exitDy=0;exitPerimeter=0;" edge="1" parent="1" source="ncjso_DGpGOnADHclqbK-4" target="n9qyGrMY-b-BzYaa1yog-2">
+          <mxGeometry relative="1" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-27" value="" style="group" vertex="1" connectable="0" parent="1">
+          <mxGeometry x="490" y="-50" width="170" height="190" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-2" value="mat-data" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=110;height=30;" parent="ncjso_DGpGOnADHclqbK-27" vertex="1">
+          <mxGeometry width="170" height="190" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-4" value="preprocess" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="ncjso_DGpGOnADHclqbK-27" vertex="1">
+          <mxGeometry x="20" y="73" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-5" value="generator" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="ncjso_DGpGOnADHclqbK-27" vertex="1">
+          <mxGeometry x="20" y="37" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-36" value="converter" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="ncjso_DGpGOnADHclqbK-27" vertex="1">
+          <mxGeometry x="20" y="109" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="mgZLQg_ETMRa4hPbAOP7-1" value="datasets" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="ncjso_DGpGOnADHclqbK-27" vertex="1">
+          <mxGeometry x="20" y="144" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-28" value="" style="group" vertex="1" connectable="0" parent="1">
+          <mxGeometry x="250" y="273" width="190" height="520" as="geometry" />
+        </mxCell>
+        <mxCell id="mgZLQg_ETMRa4hPbAOP7-5" value="methods" style="shape=folder;fontStyle=1;spacingTop=10;tabWidth=40;tabHeight=14;tabPosition=left;html=1;whiteSpace=wrap;horizontal=1;verticalAlign=top;fillColor=none;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="10" y="34" width="160" height="436" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-10" value="MLP (movelets)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="20" y="326" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="mgZLQg_ETMRa4hPbAOP7-10" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=1;entryY=0.5;entryDx=0;entryDy=0;endArrow=open;dashed=1;endFill=0;" parent="ncjso_DGpGOnADHclqbK-28" source="n9qyGrMY-b-BzYaa1yog-11" target="n9qyGrMY-b-BzYaa1yog-10" edge="1">
+          <mxGeometry relative="1" as="geometry">
+            <Array as="points">
+              <mxPoint x="160" y="450" />
+              <mxPoint x="160" y="341" />
+            </Array>
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-11" value="TEC" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#fff2cc;strokeColor=#d6b656;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="20" y="435" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-19" value="mat-classification" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=130;height=27;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry width="190" height="520" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-20" value="POI-S" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="21" y="289" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="mgZLQg_ETMRa4hPbAOP7-9" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=1;entryY=0.5;entryDx=0;entryDy=0;endArrow=open;dashed=1;endFill=0;" parent="ncjso_DGpGOnADHclqbK-28" source="n9qyGrMY-b-BzYaa1yog-11" target="n9qyGrMY-b-BzYaa1yog-20" edge="1">
+          <mxGeometry relative="1" as="geometry">
+            <Array as="points">
+              <mxPoint x="160" y="450" />
+              <mxPoint x="160" y="304" />
+            </Array>
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-21" value="MARC" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="21" y="252" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="mgZLQg_ETMRa4hPbAOP7-8" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=1;entryY=0.5;entryDx=0;entryDy=0;endArrow=open;dashed=1;endFill=0;" parent="ncjso_DGpGOnADHclqbK-28" source="n9qyGrMY-b-BzYaa1yog-11" target="n9qyGrMY-b-BzYaa1yog-21" edge="1">
+          <mxGeometry relative="1" as="geometry">
+            <Array as="points">
+              <mxPoint x="160" y="450" />
+              <mxPoint x="160" y="267" />
+            </Array>
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-24" value="RF&amp;nbsp; (movelets)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="20" y="362" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-25" value="SVM&amp;nbsp;(movelets)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="20" y="398" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-26" value="DeepestST" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="20" y="68" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-27" value="MAT RF" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="20" y="105" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-28" value="MAT XGBoost" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="20" y="141" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-29" value="TULVAE" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="20" y="178" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-30" value="BITULER" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="20" y="215" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="mgZLQg_ETMRa4hPbAOP7-6" value="scripts" style="shape=folder;fontStyle=1;spacingTop=10;tabWidth=40;tabHeight=10;tabPosition=left;html=1;whiteSpace=wrap;" parent="ncjso_DGpGOnADHclqbK-28" vertex="1">
+          <mxGeometry x="24" y="480" width="126" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-29" value="" style="group" vertex="1" connectable="0" parent="1">
+          <mxGeometry x="-130" y="277" width="170" height="235" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-12" value="automatize" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=120;height=27;" parent="ncjso_DGpGOnADHclqbK-29" vertex="1">
+          <mxGeometry width="170" height="235" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-13" value="run" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="ncjso_DGpGOnADHclqbK-29" vertex="1">
+          <mxGeometry x="20" y="77" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-14" value="results" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="ncjso_DGpGOnADHclqbK-29" vertex="1">
+          <mxGeometry x="20" y="40" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-16" value="datasets" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="ncjso_DGpGOnADHclqbK-29" vertex="1">
+          <mxGeometry x="20" y="114" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-22" value="web-app" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="ncjso_DGpGOnADHclqbK-29" vertex="1">
+          <mxGeometry x="20" y="152" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="mgZLQg_ETMRa4hPbAOP7-7" value="scripts" style="shape=folder;fontStyle=1;spacingTop=10;tabWidth=40;tabHeight=10;tabPosition=left;html=1;whiteSpace=wrap;" parent="ncjso_DGpGOnADHclqbK-29" vertex="1">
+          <mxGeometry x="25" y="196" width="125" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-30" value="" style="group" vertex="1" connectable="0" parent="1">
+          <mxGeometry x="70" y="277" width="170" height="130" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-6" value="mat-view" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=120;height=26;" parent="ncjso_DGpGOnADHclqbK-30" vertex="1">
+          <mxGeometry width="170" height="130" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-7" value="web-app &lt;br&gt;&lt;i&gt;(Movelets &amp;amp; MAT)&lt;/i&gt;" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="ncjso_DGpGOnADHclqbK-30" vertex="1">
+          <mxGeometry x="20" y="73" width="130" height="41" as="geometry" />
+        </mxCell>
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-8" value="view / graphics" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="ncjso_DGpGOnADHclqbK-30" vertex="1">
+          <mxGeometry x="20" y="37" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-39" value="" style="group" vertex="1" connectable="0" parent="1">
+          <mxGeometry x="640" y="270" width="170" height="220" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-2" value="mat-similarity" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=140;height=31;" vertex="1" parent="ncjso_DGpGOnADHclqbK-39">
+          <mxGeometry width="170" height="220" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-31" value="muitas" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-39">
+          <mxGeometry x="20" y="42" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-32" value="ftsm" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-39">
+          <mxGeometry x="20" y="76" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-33" value="ums" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-39">
+          <mxGeometry x="20" y="110" width="130" height="30" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-34" value="msm" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-39">
+          <mxGeometry x="20" y="144" width="130" height="30" as="geometry" />
         </mxCell>
-        <mxCell id="ncjso_DGpGOnADHclqbK-4" value="mat-clustering" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=133;height=26;" vertex="1" parent="1">
-          <mxGeometry x="670" y="285.5" width="170" height="190" as="geometry" />
+        <mxCell id="ncjso_DGpGOnADHclqbK-35" value="smsm" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" vertex="1" parent="ncjso_DGpGOnADHclqbK-39">
+          <mxGeometry x="20" y="178" width="130" height="30" as="geometry" />
         </mxCell>
       </root>
     </mxGraphModel>
   </diagram>
 </mxfile>
```

### Comparing `mat_model-0.1b1/PKG-INFO` & `mat_model-0.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat-model
-Version: 0.1b1
+Version: 0.1b2
 Summary: MAT-model: Model Classes for Multiple Aspect Trajectory Data Mining
 Home-page: https://github.com/ttportela/mat-model
 Author: Tarlis Tortelli Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/ttportela/mat-model
```

### Comparing `mat_model-0.1b1/README.md` & `mat_model-0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b1/Steps to Build.txt` & `mat_model-0.1b2/Steps to Build.txt`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b1/mat_model.egg-info/PKG-INFO` & `mat_model-0.1b2/mat_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat-model
-Version: 0.1b1
+Version: 0.1b2
 Summary: MAT-model: Model Classes for Multiple Aspect Trajectory Data Mining
 Home-page: https://github.com/ttportela/mat-model
 Author: Tarlis Tortelli Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/ttportela/mat-model
```

### Comparing `mat_model-0.1b1/matmodel/LICENSE` & `mat_model-0.1b2/matmodel/LICENSE`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b1/matmodel/README.md` & `mat_model-0.1b2/matmodel/README.md`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b1/matmodel/base/Aspect.py` & `mat_model-0.1b2/matmodel/base/Aspect.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,45 +10,74 @@
         return str(self.value)
     
     def match(self, asp1, asp2):
         return asp1.__eq__(asp2)
     
     def __eq__(self, other):
         return self._value == other._value
+    
+class Numeric(Aspect):
+    def __init__(self, value):
+        value = float(value)
+        Aspect.__init__(self, value)
+    
+class Categoric(Aspect):
+    def __init__(self, value):
+        Aspect.__init__(self, value)
 
 class Space2D(Aspect):
-    def __init__(self, x, y):
+    def __init__(self, value):
+        x, y = value.split(' ')
         Aspect.__init__(self, str((x,y)))
+        x, y = float(x), float(y)
         self.x = x
         self.y = y
 
-    @Aspect.value.getter
+    @Space2D.value.getter
     def value(self):
         return (self.x, self.y)
     
+    def __repr__(self):
+        return "({:.3f} {:.3f})".format(self.x, self.y)
+    
     def __eq__(self, other):
         return self.x == other.x and self.y == other.y
 
-
 class Space3D(Space2D):
-    def __init__(self, x, y, z):
-        Space2D.__init__(x, y)
+    def __init__(self, x, y, z):        
+        x, y, z = v.split(' ')
         Aspect.__init__(self, str((x,y,z)))
+        
+        x, y, z = float(x), float(y), float(z)
+        self.x = x
+        self.y = y
         self.z = z
 
-    @Aspect.value.getter
+    @Space3D.value.getter
     def value(self):
         return (self.x, self.y, self.z)
     
+    def __repr__(self):
+        return "({:.3f} {:.3f} {:.3f})".format(self.x, self.y, self.z)
+    
     def __eq__(self, other):
         return self.x == other.x and self.y == other.y and self.z == other.z
 
-class DateTimeAspect(Aspect):
-    def __init__(self, value):
-        Aspect.__init__(self, value)
+class DateTime(Aspect):
+    def __init__(self, start):     
+#            from datetime import datetime
+#            #Format like: "YYYY-MM-DD HH:MM:SS.ffffff"
+#            return DateTimeAspect( datetime.fromisoformat(v) )
+        
+        # TODO Converter datetime
+        Aspect.__init__(self, start)
+    
+    @DateTime.start.getter
+    def start(self):
+        return self._value
     
     def day(self): #Just the day (1..30|31*)
         return self._value.day
     
     def month(self): #Just the month (1..12)
         return self._value.month
     
@@ -72,16 +101,16 @@
     
     def seconds(self):
         return self.minutes()*60 + self._value.second
     
     def microseconds(self):
         return self.seconds()*1000000 + self._value.microsecond
     
-    @Aspect.value.getter
-    def value(self, units=None):
+    @DateTime.value.getter
+    def value(self, units=None): # TODO for interval?
         if units == None:
             return self._value
         elif units == 'D':
             return self.day()
         elif units == 'M':
             return self.month()
         elif units == 'Y':
@@ -93,36 +122,56 @@
         elif units == 'm':
             return self.minutes()
         elif units == 's':
             return self.seconds()
         elif units == 'ms':
             return self.microseconds()
         else:
-            raise Exception('[ERROR DateTimeAspect]: invalid \'units='+str(units)+'\' conversion.')
+            raise Exception('[ERROR DateTime Aspect]: invalid \'units='+str(units)+'\' conversion.')
     
-#    def __eq__(self, other):
-#        return self._value == other._value
+class Interval(DateTime):
+    def __init__(self, start, end):
+        DateTime.__init__(self, start)
+        # TODO Converter datetime
+        self.end = end
+
+class Rank(Aspect):
+    def __init__(self, descriptor):
+        Aspect.__init__(self, descriptor)
+        self.rank_values = [] # ->RankValue
+        
+    @Rank.descriptor.getter
+    def descriptor(self):
+        return self._value
+    
+    def add(self, aspect, proportion):
+        self.rank_values.append(RankValue(aspect, proportion))
+    
+class RankValue:
+    def __init__(self, value, proportion):
+        self.value = value
+        self.proportion = proportion
 
 # ------------------------------------------------------------------------------------------------------------
 def instantiateAspect(k,v):
     try:
-        if k['type'] == 'nominal':
-            return Aspect( str(v) )
-        elif k['type'] == 'numeric':
-            return Aspect( float(v) )
-        elif k['type'] == 'space2d':
+        if k.dtype == 'nominal':
+            return Categorical( str(v) )
+        elif k.dtype == 'numeric':
+            return Numeric( v )
+        elif k.dtype == 'time' or k.dtype == 'datetime':
+            return DateTime( v )
+        elif k.dtype == 'space2d':
             x, y = v.split(' ')
-            return Space2D(float(x), float(y))
-        elif k['type'] == 'space3d':
+            return Space2D( v )
+        elif k.dtype == 'space3d':
             x, y, z = v.split(' ')
-            return Space3D(float(x), float(y), float(z))
-        elif k['type'] == 'boolean':
-            return Aspect( bool(v) )
-        elif k['type'] == 'datetime':
-            from datetime import datetime
-            #Format like: "YYYY-MM-DD HH:MM:SS.ffffff"
-            return DateTimeAspect( datetime.fromisoformat(v) )
+            return Space3D( v )
+        elif k.dtype == 'rank':
+            return Rank( v )
+#        elif k.dtype == 'boolean':
+#            return Aspect( bool(v) )
         else:
             return Aspect( v )
     except:
-        raise Exception("[ERROR Aspect.py]: Filed to load value " + str(v) \
+        raise Exception("[ERROR Aspect.py]: Failed to load value " + str(v) \
                         + " as type " + str(k['type']) + ' attr#' + str(k['order']))
```

### Comparing `mat_model-0.1b1/matmodel/base/Feature.py` & `mat_model-0.1b2/matmodel/evaluation/Feature.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from matmodel.base.Aspect import Aspect
-
-class Quality:
-    def __init__(self, value):
-        self.value = value
+from matmodel.base import Aspect
 
 class Feature:
     def __init__(self, quality=None):
         self.quality = quality
         
-class IntervalFeature(Feature):
-    def __init__(self, quality=None):
-        Feature.__init__(self, quality)
-        
-class CellFeature(IntervalFeature):
-    def __init__(self, quality=None):
-        Feature.__init__(self, quality)
-        
-class AspectFeature(Feature):
-    def __init__(self, aspect, quality=None):
-        Feature.__init__(self, quality)
-        self.aspect = aspect
+#class IntervalFeature(Feature):
+#    def __init__(self, quality=None):
+#        Feature.__init__(self, quality)
+#        
+#class CellFeature(IntervalFeature):
+#    def __init__(self, quality=None):
+#        Feature.__init__(self, quality)
+#        
+#class AspectFeature(Feature):
+#    def __init__(self, aspect, quality=None):
+#        Feature.__init__(self, quality)
+#        self.aspect = aspect
         
 class DerrivedFeature(Feature, Aspect):
     def __init__(self, value, original_aspect, quality=None):
         Feature.__init__(self, quality)
         Aspect.__init__(self, value)
         self.aspect = aspect
```

### Comparing `mat_model-0.1b1/matmodel/base/Subtrajectory.py` & `mat_model-0.1b2/matmodel/base/xSubtrajectory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 # ------------------------------------------------------------------------------------------------------------
 # SUBTRAJECTORIES 
 # ------------------------------------------------------------------------------------------------------------
 from matmodel.base.MultipleAspectSequence import MultipleAspectSequence
 
 class Subtrajectory(MultipleAspectSequence):
-    def __init__(self, trajectory, start, size, points, attributes_index):
+    def __init__(self, trajectory, start, points, attributes_index):
         MultipleAspectSequence.__init__(self, trajectory.tid)
         self.sid     = 0 # TODO generate unique sid
         self.start   = start
-        self.size   = size
+#        self.size   = size
         self.trajectory   = trajectory
         self.points       = points # list contains instances of Point class
         self._attributes   = attributes_index # Just the index of attributes (from points) that belong to the analysis
         
+    @property
+    def s(self):
+        return '𝓈⟨{},{}⟩'.format(self.start, (self.start+self.size-1))
+    @property
+    def S(self):
+        return '𝓈⟨{},{}⟩'.format(self.start, (self.start+self.size-1))+'{'+','.join(map(lambda x: str(x), self._attributes))+'}'
+    
     def __repr__(self):
-        return 'T'+str(self.trajectory.tid)+'.S('+str(self.start)+','+str(self.start+self.size-1)+').['+','.join(map(lambda x: str(x), self._attributes))+']'
+        return self.S+'𐄁'+self.trajectory.T+' '+MultipleAspectSequence.__repr__(self)
         
     def attribute(self, index):
         return self.trajectory.attributes[index]
 
     @property
     def attributes(self):
         return list(map(lambda index: self.trajectory.attributes[index], self._attributes))
     
     def values(self):
         return super().valuesOf(self._attributes)
     
     def valuesOf(self, attributes_index):
         return super().valuesOf(attributes_index)
     
-    def asString(self):
-        return self.__repr__()+':'+super().asString(self._attributes)
-    
+#    def asString(self):
+#        return self.__repr__()+':'+super().asString(self._attributes)
+#    
 #    def attributes(self):
 #        return self.data[0].keys()
 #    
 #    def add_point(self, point):
 #        assert isinstance(point, dict)
 #        self.data.append(self.point_dict(point))
 #
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mat_model-0.1b1/matmodel/distance/Comparator.py` & `mat_model-0.1b2/matmodel/distance/comparator.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,92 +3,113 @@
 
     Properties:
     max_value=None  - Maximum possible value for distance, default: Comparator.MAX_VALUE = float('inf').
     '''
     
     MAX_VALUE = float('inf')
     
-    def __init__(self):
-        self.max_value = Comparator.MAX_VALUE
+    def __init__(self, max_value=None):
+        self.max_value = max_value
+        self.min_value = 0
     
     def distance(self, asp1, asp2):
         '''Calculates the distance.
 
         Arguments:
         asp1 (Aspect<?>) - value 1 to compare
         asp2 (Aspect<?>) - value 2 to compare
         
         Return:
         distance - distance equality value (0 for equal values, 1 for different).
         '''
         return 0 if asp1.__eq__(asp2) else 1
-    def match(self, asp1, asp2):
-        return True
+    
     def normalize(self, distance):
-        if self.max_value == -1:
+        if not self.max_value:
             return distance
-        if distance >= self.max_value:
-            return self.max_value
-        return distance / self.max_value
+        
+        return (distance - self.min_value) / (self.max_value - self.min_value)
+    
     def enhance(self, distance):
         distance = (distance * distance)
-        return distance if distance < self.max_value else self.max_value
+        if self.max_value and distance > self.max_value:
+            return self.max_value
+        else:
+            return distance
     
+    @staticmethod
+    def instantiate(json_obj):
+        # TODO: new distances and specific cases:
+        max_value = json_obj['comparator']['maxValue'] if 'maxValue' in json_obj['comparator'].keys() else -1
+        if max_value == -1:
+            max_value = None
+        
+        if json_obj['comparator']['distance'] == 'difference' and  json_obj['type'] == 'time':
+            units = json_obj['comparator']['units'] if 'units' in json_obj['comparator'].keys() else 'm'
+            return TimeDistance(max_value, units)
+        
+        elif json_obj['comparator']['distance'] == 'diffnotneg' or json_obj['comparator']['distance'] == 'difference':
+            return AbsoluteDistance(max_value)
+        
+        else:
+            cname = eval( str(json_obj['comparator']['distance']).capitalize()+'Distance' )
+            return cname(max_value)
+
 class EqualsDistance(Comparator):
-    def __init__(self):
-        self.max_value = 1
+    def __init__(self, max_value=None):
+        Comparator.__init__(self, max_value)
         
     def distance(self, asp1, asp2):
         '''Calculates the distance for eqality ignoring case.
 
         Arguments:
         asp1 (Aspect<nominal>) - value 1 to compare
         asp2 (Aspect<nominal>) - value 2 to compare
         
         Return:
         distance - distance equality value (0 for equal values, 1 for different).
         '''
         return 0 if asp1._value.upper() == asp2._value.upper() else 1
 
 class CaselessDistance(Comparator):
-    def __init__(self):
-        self.max_value = 1
+    def __init__(self, max_value=None):
+        Comparator.__init__(self, max_value)
     
 class NumericDistance(Comparator):
-    def __init__(self):
-        pass
+    def __init__(self, max_value=None):
+        Comparator.__init__(self, max_value)
 
     def distance(self, asp1, asp2):
         '''Calculates the numeric distance.
 
         Arguments:
         asp1 (Aspect<numeric>) - value 1 to compare
         asp2 (Aspect<numeric>) - value 2 to compare
         
         Return:
         distance - distance difference value (asp1 - asp2).
         '''
         return asp1._value - asp2._value
     
 class AbsoluteDistance(NumericDistance):
-    def __init__(self):
-        pass
+    def __init__(self, max_value=None):
+        Comparator.__init__(self, max_value)
 
     def distance(self, asp1, asp2):
         '''Calculates the absolute distance.
 
         Arguments:
         asp1 (Aspect<numeric>) - value 1 to compare
         asp2 (Aspect<numeric>) - value 2 to compare
         
         Return:
         distance - distance difference value, abs(asp1 - asp2).
         '''
         return abs(asp1._value - asp2._value)
-      
+
 class DateDistance(Comparator): 
     '''Calculates the date distance in one of the following units:
     D - days
     M - months
     Y - years
     w - weeks
     h - hours
@@ -99,18 +120,18 @@
     '=weekday'  - equal weekday (0 for equal values, 1 for different)
     'isweekday' - equal if both are weekdays or both are weekends (0 for equal values, 1 for different)
 
     Properties:
     units='ms'      - Unit measure to get distance.
     max_value=None  - Maximum possible value for distance, default: Comparator.MAX_VALUE = float('inf')
     '''
-    def __init__(self, units=None, max_value=None):
+    
+    def __init__(self, max_value=None, units=None):
+        Comparator.__init__(self, max_value)
         self.units = units
-        if max_value:
-            self.max_value = max_value
     
     def distance(self, asp1, asp2):
         dt1 = max(asp1._value - asp2._value)
         dt2 = min(asp1._value - asp2._value)
 #        delta = abs(asp1._value - asp2._value)
         if self.units == None or self.units == 's':
             return (dt1 - dt2).total_seconds()
@@ -141,15 +162,16 @@
     '''Calculates the closest time distance.
     Only works for time in hours, minutes, seconds, and microseconds. Ex.: difference between 22h and 2h is 3h.
 
     Properties:
     units='ms'      - Unit measure to get distance: h (hours), m (minutes), s (seconds), ms (microseconds)
     max_value=None  - Maximum possible value for distance (Ex.: hours = 24)
     '''
-    def __init__(self, units='ms', max_value=None): 
+    
+    def __init__(self, max_value=None, units='m'): 
         # Works for time in hours, minutes or seconds. Ex.: difference between 22h and 2h is 3h.
         self.units = units
         if max_value:
             self.max_value = max_value
         elif units == 'h':
             self.max_value = 23
         elif units == 'm':
@@ -172,16 +194,16 @@
         v1 = asp1.value(self.units)
         v2 = asp2.value(self.units)
         v1 = max(v1, v2)
         v2 = min(v1, v2)
         return min( ((self.max_value - v1) + v2 +1), (v1 - v2) )
     
 class EuclideanDistance(Comparator):
-    def __init__(self):
-        pass
+    def __init__(self, max_value=None):
+        Comparator.__init__(self, max_value)
 
     def distance(self, asp1, asp2):
         '''Calculates the Euclidean distance (works for points of 2D, 3D, and more).
         
         Arguments:
         asp1 (Space2D, Space3D) - value 1 to compare
         asp2 (Space2D, Space3D) - value 2 to compare
@@ -202,32 +224,32 @@
 #        if isinstance(asp1, Space3D):
 #            diffZ = abs(asp1.z - asp2.z)
 #            return math.sqrt( diffX * diffX + diffY * diffY + diffZ * diffZ )
 #        else:
 #            return math.sqrt( diffX * diffX + diffY * diffY )
     
 class ManhattanDistance(Comparator):
-    def __init__(self):
-        pass
+    def __init__(self, max_value=None):
+        Comparator.__init__(self, max_value)
 
     def distance(self, asp1, asp2):
         '''Calculates the Manhattan distance (works for points of 2D, 3D, and more).
         
         Arguments:
         asp1 (Space2D, Space3D) - value 1 to compare
         asp2 (Space2D, Space3D) - value 2 to compare
         
         Return:
         distance - distance value.
         '''
         return sum(map(lambda v1, v2: abs(v1 - v2), asp1.value, asp2.value))
     
 class LcsDistance(Comparator):
-    def __init__(self):
-        pass
+    def __init__(self, max_value=None):
+        Comparator.__init__(self, max_value)
     
     def lcs(self, X, Y):
         m = len(X)
         n = len(Y)
 
         L = list(map(lambda i: [None]*(n + 1), range(m + 1)))
 
@@ -240,30 +262,33 @@
                 L[i][j] = max(L[i-1][j], L[i][j-1])
 
             return L[i][j]
 
         list(map(lambda i: list(map(lambda j: sublcs(i, j), range(n + 1))), range(m + 1)))            
 
         return L[m][n]
+    
+    def lcs_distance(self, X, Y):
+        return max(len(X),len(Y)) - self.lcs(X, Y) 
 
     def distance(self, asp1, asp2):
         '''Calculates the Longest Common Subsequence difference.
         
         Arguments:
         asp1 (Aspect<nominal>) - value 1 to compare
         asp2 (Aspect<nominal>) - value 2 to compare
         
         Return:
         distance - LCS distance value.
         '''
-        return self.lcs(asp1._value, asp2._value)
+        return self.lcs_distance(asp1._value, asp2._value)
     
 class EditlcsDistance(LcsDistance):
-    def __init__(self):
-        pass
+    def __init__(self, max_value=None):
+        Comparator.__init__(self, max_value)
 
     def distance(self, asp1, asp2):
         '''Calculates the Longest Common Subsequence difference.
         
         Arguments:
         asp1 (Aspect<nominal>) - value 1 to compare
         asp2 (Aspect<nominal>) - value 2 to compare
```

### Comparing `mat_model-0.1b1/matmodel.drawio` & `mat_model-0.1b2/matmodel.drawio`

 * *Files 23% similar despite different names*

```diff
@@ -1,119 +1,143 @@
-<mxfile host="app.diagrams.net" modified="2024-04-12T14:57:32.263Z" agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36" etag="blJMUS1FKUra21bA0XFC" version="23.1.5" type="device">
+<mxfile host="app.diagrams.net" modified="2024-05-23T14:55:08.743Z" agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36" etag="S5ZcHV_cwoiQNoxT-Row" version="24.4.0" type="device">
   <diagram id="C5RBs43oDa-KdzZeNtuy" name="Page-1">
-    <mxGraphModel dx="954" dy="615" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="827" pageHeight="1169" math="0" shadow="0">
+    <mxGraphModel dx="1831" dy="1753" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="827" pageHeight="1169" math="0" shadow="0">
       <root>
         <mxCell id="WIyWlLk6GJQsqaUBKTNV-0" />
         <mxCell id="WIyWlLk6GJQsqaUBKTNV-1" parent="WIyWlLk6GJQsqaUBKTNV-0" />
-        <mxCell id="lsfipmTJbNCapsntxlYZ-0" value="MultipleAspectSequence" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="230" y="84" width="160" height="132" as="geometry" />
+        <mxCell id="wUrawppS3UO5J027udKO-70" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-0" target="wUrawppS3UO5J027udKO-7" edge="1">
+          <mxGeometry relative="1" as="geometry">
+            <Array as="points">
+              <mxPoint x="310" y="-120" />
+            </Array>
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-71" value="- descriptor" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="wUrawppS3UO5J027udKO-70" vertex="1" connectable="0">
+          <mxGeometry x="-0.9495" relative="1" as="geometry">
+            <mxPoint x="30" y="12" as="offset" />
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-72" value="1" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="wUrawppS3UO5J027udKO-70" vertex="1" connectable="0">
+          <mxGeometry x="0.9593" y="2" relative="1" as="geometry">
+            <mxPoint x="8" y="-8" as="offset" />
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="lsfipmTJbNCapsntxlYZ-0" value="MultipleAspectSequence" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#1ba1e2;fontColor=#ffffff;strokeColor=#006EAF;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="230" y="84" width="160" height="108" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-11" value="- tid: int/str" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-0" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-12" value="-&amp;nbsp;size: int" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-0" vertex="1">
           <mxGeometry y="50" width="160" height="24" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-1" value="-&amp;nbsp;attributes: dict" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-0" vertex="1">
-          <mxGeometry y="74" width="160" height="24" as="geometry" />
-        </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-2" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-0" vertex="1">
-          <mxGeometry y="98" width="160" height="8" as="geometry" />
+          <mxGeometry y="74" width="160" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-3" value="+&amp;nbsp;addPoint&lt;span style=&quot;background-color: initial;&quot;&gt;(type): type&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-0" vertex="1">
-          <mxGeometry y="106" width="160" height="26" as="geometry" />
+          <mxGeometry y="82" width="160" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-13" value="Point" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-13" value="Point" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
           <mxGeometry x="500" y="104" width="160" height="84" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-14" value="-&amp;nbsp;seq&lt;span style=&quot;background-color: initial;&quot;&gt;: int&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-13" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-17" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-13" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-18" value="+&amp;nbsp;getL&lt;span style=&quot;background-color: initial;&quot;&gt;(): int&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-13" vertex="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-18" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-13" vertex="1">
           <mxGeometry y="58" width="160" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-19" value="Aspect" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="782" y="100" width="160" height="84" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-19" value="Aspect" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#60a917;fontColor=#ffffff;strokeColor=#2D7600;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="1003" y="100" width="160" height="84" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-20" value="-&amp;nbsp;value&lt;span style=&quot;background-color: initial;&quot;&gt;: ?&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-19" vertex="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-20" value="-&amp;nbsp;value&lt;span style=&quot;background-color: initial;&quot;&gt;: object or str&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-19" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-21" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-19" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-22" value="+&amp;nbsp;addPoint&lt;span style=&quot;background-color: initial;&quot;&gt;(type): type&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-19" vertex="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-22" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-19" vertex="1">
           <mxGeometry y="58" width="160" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-34" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-23" target="lsfipmTJbNCapsntxlYZ-19" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-23" value="Space2D" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="782" y="236" width="160" height="108" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-23" value="Space2D" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="1003" y="236" width="160" height="108" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-27" value="-&amp;nbsp;x&lt;span style=&quot;background-color: initial;&quot;&gt;: int&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-23" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-24" value="- y&lt;span style=&quot;background-color: initial;&quot;&gt;: int&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-23" vertex="1">
           <mxGeometry y="50" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-25" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-23" vertex="1">
           <mxGeometry y="74" width="160" height="8" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-26" value="+ getValue&lt;span style=&quot;background-color: initial;&quot;&gt;(): tuple&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-23" vertex="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-26" value="+" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-23" vertex="1">
           <mxGeometry y="82" width="160" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-33" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-28" target="lsfipmTJbNCapsntxlYZ-23" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-28" value="Space3D" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="782" y="400" width="160" height="84" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-28" value="Space3D" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="1003" y="400" width="160" height="84" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-29" value="- z&lt;span style=&quot;background-color: initial;&quot;&gt;: int&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-28" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-31" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-28" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-32" value="+ getValue&lt;span style=&quot;background-color: initial;&quot;&gt;(): tuple&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-28" vertex="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-32" value="+" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-28" vertex="1">
           <mxGeometry y="58" width="160" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-35" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;shadow=0;strokeWidth=1;endFill=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-14" target="lsfipmTJbNCapsntxlYZ-19" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
               <mxPoint x="690" y="130" />
               <mxPoint x="690" y="130" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-36" value="- aspects" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="lsfipmTJbNCapsntxlYZ-35" vertex="1" connectable="0">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-36" value="*&lt;br&gt;- aspects" style="edgeLabel;html=1;align=left;verticalAlign=middle;resizable=0;points=[];" parent="lsfipmTJbNCapsntxlYZ-35" vertex="1" connectable="0">
           <mxGeometry x="-0.5" y="1" relative="1" as="geometry">
-            <mxPoint x="-1" y="-9" as="offset" />
+            <mxPoint x="-76" y="-15" as="offset" />
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-0" value="1..*" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="lsfipmTJbNCapsntxlYZ-35" vertex="1" connectable="0">
+          <mxGeometry x="0.623" y="3" relative="1" as="geometry">
+            <mxPoint x="42" y="-7" as="offset" />
           </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-37" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;shadow=0;strokeWidth=1;endFill=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-12" target="lsfipmTJbNCapsntxlYZ-13" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-38" value="- points" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="lsfipmTJbNCapsntxlYZ-37" vertex="1" connectable="0">
           <mxGeometry x="-0.0182" y="-1" relative="1" as="geometry">
             <mxPoint x="-31" y="-13" as="offset" />
           </mxGeometry>
         </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-1" value="1..*" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="lsfipmTJbNCapsntxlYZ-37" vertex="1" connectable="0">
+          <mxGeometry x="0.6545" y="4" relative="1" as="geometry">
+            <mxPoint y="-7" as="offset" />
+          </mxGeometry>
+        </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-43" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-39" target="lsfipmTJbNCapsntxlYZ-0" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
               <mxPoint x="460" y="250" />
               <mxPoint x="310" y="250" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-39" value="Trajectory" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="380" y="310" width="160" height="84" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-39" value="Trajectory" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#1ba1e2;strokeColor=#006EAF;fontColor=#ffffff;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="380" y="290" width="160" height="84" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-40" value="-&amp;nbsp;label&lt;span style=&quot;background-color: initial;&quot;&gt;: object&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-39" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-41" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-39" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
@@ -124,38 +148,40 @@
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
               <mxPoint x="160" y="250" />
               <mxPoint x="310" y="250" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-44" value="Subtrajectory" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="80" y="290" width="160" height="108" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-44" value="Subtrajectory" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#1ba1e2;strokeColor=#006EAF;fontColor=#ffffff;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="80" y="290" width="160" height="84" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-49" value="-&amp;nbsp;start&lt;span style=&quot;background-color: initial;&quot;&gt;: int&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-44" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-45" value="-&amp;nbsp;size&lt;span style=&quot;background-color: initial;&quot;&gt;: int&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-44" vertex="1">
-          <mxGeometry y="50" width="160" height="24" as="geometry" />
-        </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-46" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-44" vertex="1">
-          <mxGeometry y="74" width="160" height="8" as="geometry" />
+          <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-47" value="+&amp;nbsp;addPoint&lt;span style=&quot;background-color: initial;&quot;&gt;(type): type&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-44" vertex="1">
-          <mxGeometry y="82" width="160" height="26" as="geometry" />
+          <mxGeometry y="58" width="160" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-50" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;shadow=0;strokeWidth=1;endFill=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-45" target="lsfipmTJbNCapsntxlYZ-39" edge="1">
-          <mxGeometry relative="1" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-50" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;shadow=0;strokeWidth=1;endFill=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" target="lsfipmTJbNCapsntxlYZ-39" edge="1">
+          <mxGeometry relative="1" as="geometry">
+            <mxPoint x="240" y="352" as="sourcePoint" />
+            <Array as="points">
+              <mxPoint x="240" y="332" />
+            </Array>
+          </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-51" value="- trajectory" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="lsfipmTJbNCapsntxlYZ-50" vertex="1" connectable="0">
           <mxGeometry x="-0.3143" y="1" relative="1" as="geometry">
-            <mxPoint x="-18" y="-7" as="offset" />
+            <mxPoint x="-5" y="-10" as="offset" />
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-55" value="Comparator" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-55" value="Comparator" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#d80073;fontColor=#ffffff;strokeColor=#A50040;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
           <mxGeometry x="1775" y="77" width="220" height="162" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-56" value="#&amp;nbsp;MAX_VALUE: float" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-55" vertex="1">
           <mxGeometry y="26" width="220" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-57" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-55" vertex="1">
           <mxGeometry y="50" width="220" height="8" as="geometry" />
@@ -171,185 +197,185 @@
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-60" value="+&amp;nbsp;enhance&lt;span style=&quot;background-color: initial;&quot;&gt;(distance): float&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-55" vertex="1">
           <mxGeometry y="136" width="220" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-61" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;shadow=0;strokeWidth=1;endFill=1;dashed=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-58" target="lsfipmTJbNCapsntxlYZ-19" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1220" y="160" />
-              <mxPoint x="1220" y="160" />
+              <mxPoint x="1885" y="120" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-63" value="(asp1, asp2)" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="lsfipmTJbNCapsntxlYZ-61" vertex="1" connectable="0">
           <mxGeometry x="-0.2297" y="-3" relative="1" as="geometry">
             <mxPoint x="127" y="-7" as="offset" />
           </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-93" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-65" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1455" y="260" />
+              <mxPoint x="1586" y="260" />
               <mxPoint x="1885" y="260" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-65" value="NumericDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1390" y="290" width="130" height="60" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-65" value="NumericDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="1521" y="290" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-67" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-65" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-70" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-65" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-94" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-81" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1600" y="260" />
+              <mxPoint x="1727" y="260" />
               <mxPoint x="1885" y="260" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-81" value="EuclideanDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1531" y="290" width="130" height="60" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-81" value="EuclideanDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="1662" y="290" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-82" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-81" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-83" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-81" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-95" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-84" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1735" y="260" />
+              <mxPoint x="1866" y="260" />
               <mxPoint x="1885" y="260" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-84" value="ManhattanDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1670" y="290" width="130" height="60" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-84" value="ManhattanDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="1801" y="290" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-85" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-84" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-86" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-84" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-96" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;exitX=0.5;exitY=0;exitDx=0;exitDy=0;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-87" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-96" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;exitDx=0;exitDy=0;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-87" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1885" y="290" />
+              <mxPoint x="2004" y="260" />
+              <mxPoint x="1885" y="260" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-87" value="EqualsDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1808" y="290" width="130" height="60" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-87" value="EqualsDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="1939" y="290" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-88" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-87" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-89" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-87" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-97" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;exitX=0.5;exitY=0;exitDx=0;exitDy=0;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-90" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-97" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;exitDx=0;exitDy=0;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-90" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="2036" y="260" />
+              <mxPoint x="2144" y="260" />
               <mxPoint x="1885" y="260" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-90" value="DateDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1948" y="290" width="130" height="60" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-90" value="DateDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="2079" y="290" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-91" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-90" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-92" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-90" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-104" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-101" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-104" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;exitDx=0;exitDy=0;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-101" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="2140" y="260" />
+              <mxPoint x="2276" y="260" />
               <mxPoint x="1885" y="260" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-101" value="TimeDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="2090" y="290" width="110" height="60" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-101" value="TimeDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="2221" y="290" width="110" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-102" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-101" vertex="1">
           <mxGeometry y="26" width="110" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-103" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-101" vertex="1">
           <mxGeometry y="34" width="110" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-117" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-114" target="lsfipmTJbNCapsntxlYZ-87" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1802" y="380" />
-              <mxPoint x="1873" y="380" />
+              <mxPoint x="1933" y="380" />
+              <mxPoint x="2004" y="380" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-114" value="LCSDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1737" y="398" width="130" height="60" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-114" value="LcsDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="1868" y="398" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-115" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-114" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-116" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-114" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-121" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-118" target="lsfipmTJbNCapsntxlYZ-87" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1942" y="380" />
-              <mxPoint x="1873" y="380" />
+              <mxPoint x="2073" y="380" />
+              <mxPoint x="2004" y="380" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-118" value="CaselessDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1877" y="398" width="130" height="60" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-118" value="CaselessDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="2008" y="398" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-119" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-118" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-120" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-118" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-125" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-122" target="lsfipmTJbNCapsntxlYZ-65" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-122" value="AbsoluteDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1390" y="390" width="130" height="60" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-122" value="AbsoluteDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="1521" y="390" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-123" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-122" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-124" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-122" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-126" value="&lt;i&gt;FeatureExtractor&lt;/i&gt;" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="520" y="860" width="160" height="84" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-126" value="&lt;i&gt;MethodWrapper&lt;/i&gt;" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="-230" y="290" width="160" height="84" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-127" value="-" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-126" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-128" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-126" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-129" value="+" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-126" vertex="1">
           <mxGeometry y="58" width="160" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-130" value="Point" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="850" y="890" width="160" height="84" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-130" value="Class" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="-390" y="680" width="160" height="84" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-131" value="-" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-130" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-132" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-130" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
@@ -358,35 +384,35 @@
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-138" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-134" target="lsfipmTJbNCapsntxlYZ-44" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-148" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-134" target="lsfipmTJbNCapsntxlYZ-143" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="160" y="570" />
-              <mxPoint x="380" y="570" />
+              <mxPoint x="160" y="650" />
+              <mxPoint x="337" y="650" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-134" value="Movelet" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="80" y="600" width="160" height="84" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-134" value="Movelet" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#fff2cc;strokeColor=#d6b656;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="80" y="680" width="160" height="84" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-135" value="-" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-134" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-136" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-134" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-137" value="+" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-134" vertex="1">
           <mxGeometry y="58" width="160" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-139" value="FeatureQuality" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="560" y="450" width="160" height="84" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-139" value="Quality" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#fff2cc;strokeColor=#d6b656;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="480" y="530" width="160" height="84" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-140" value="-" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-139" vertex="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-140" value="- value" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-139" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-141" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-139" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-142" value="+" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-139" vertex="1">
           <mxGeometry y="58" width="160" height="26" as="geometry" />
@@ -395,120 +421,341 @@
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-149" value="- quality" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="lsfipmTJbNCapsntxlYZ-147" vertex="1" connectable="0">
           <mxGeometry x="-0.3778" y="2" relative="1" as="geometry">
             <mxPoint y="-6" as="offset" />
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-143" value="&lt;i&gt;Feature&lt;/i&gt;" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="297" y="450" width="160" height="84" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-143" value="&lt;i&gt;Feature&lt;/i&gt;" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e3c800;fontColor=#000000;strokeColor=#B09500;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="257" y="530" width="160" height="84" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-144" value="-&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-143" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-145" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-143" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-146" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-143" vertex="1">
           <mxGeometry y="58" width="160" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-157" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;exitX=0.5;exitY=0;exitDx=0;exitDy=0;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-151" target="lsfipmTJbNCapsntxlYZ-143" edge="1">
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-5" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=open;endFill=1;endSize=10;" edge="1" parent="WIyWlLk6GJQsqaUBKTNV-1" source="wUrawppS3UO5J027udKO-11" target="lsfipmTJbNCapsntxlYZ-162">
+          <mxGeometry relative="1" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-25" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=open;endFill=0;endSize=10;" edge="1" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-162" target="lsfipmTJbNCapsntxlYZ-13">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="584" y="570" />
-              <mxPoint x="380" y="570" />
+              <mxPoint x="730" y="432" />
+              <mxPoint x="730" y="170" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-151" value="AspectFeature" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="504" y="600" width="160" height="84" as="geometry" />
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-26" value="*" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;" vertex="1" connectable="0" parent="CCnf-G1CkggKAS8I-f5b-25">
+          <mxGeometry x="0.8842" relative="1" as="geometry">
+            <mxPoint as="offset" />
+          </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-152" value="-&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-151" vertex="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-162" value="RepresentativeCell" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#fad9d5;strokeColor=#ae4132;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="562.5" y="390" width="135" height="84" as="geometry" />
+        </mxCell>
+        <mxCell id="lsfipmTJbNCapsntxlYZ-163" value="-&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-162" vertex="1">
+          <mxGeometry y="26" width="135" height="24" as="geometry" />
+        </mxCell>
+        <mxCell id="lsfipmTJbNCapsntxlYZ-164" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-162" vertex="1">
+          <mxGeometry y="50" width="135" height="8" as="geometry" />
+        </mxCell>
+        <mxCell id="lsfipmTJbNCapsntxlYZ-165" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-162" vertex="1">
+          <mxGeometry y="58" width="135" height="26" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-6" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=block;endFill=0;endSize=10;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="wUrawppS3UO5J027udKO-2" target="lsfipmTJbNCapsntxlYZ-19" edge="1">
+          <mxGeometry relative="1" as="geometry">
+            <Array as="points">
+              <mxPoint x="1260" y="210" />
+              <mxPoint x="1083" y="210" />
+            </Array>
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-2" value="DateTime" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="1180" y="237" width="160" height="84" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-3" value="- start : timestamp" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-2" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-153" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-151" vertex="1">
+        <mxCell id="wUrawppS3UO5J027udKO-4" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="wUrawppS3UO5J027udKO-2" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-154" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-151" vertex="1">
+        <mxCell id="wUrawppS3UO5J027udKO-5" value="+" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-2" vertex="1">
           <mxGeometry y="58" width="160" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-155" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;shadow=0;strokeWidth=1;endFill=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-151" target="lsfipmTJbNCapsntxlYZ-19" edge="1">
+        <mxCell id="wUrawppS3UO5J027udKO-63" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" edge="1">
           <mxGeometry relative="1" as="geometry">
-            <mxPoint x="660" y="610" as="sourcePoint" />
+            <mxPoint x="1691" y="-140" as="sourcePoint" />
+            <mxPoint x="1805" y="-140" as="targetPoint" />
             <Array as="points">
-              <mxPoint x="610" y="580" />
-              <mxPoint x="750" y="580" />
-              <mxPoint x="750" y="160" />
+              <mxPoint x="1790" y="-140" />
+              <mxPoint x="1790" y="-140" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-156" value="- aspect" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="lsfipmTJbNCapsntxlYZ-155" vertex="1" connectable="0">
-          <mxGeometry x="-0.8809" y="2" relative="1" as="geometry">
-            <mxPoint x="15" y="8" as="offset" />
+        <mxCell id="wUrawppS3UO5J027udKO-65" value="- attributes" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="wUrawppS3UO5J027udKO-63" vertex="1" connectable="0">
+          <mxGeometry x="-0.7544" y="1" relative="1" as="geometry">
+            <mxPoint x="16" y="-10" as="offset" />
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-167" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-158" target="lsfipmTJbNCapsntxlYZ-143" edge="1">
+        <mxCell id="wUrawppS3UO5J027udKO-68" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" target="wUrawppS3UO5J027udKO-55" edge="1">
           <mxGeometry relative="1" as="geometry">
+            <mxPoint x="1691" y="-94" as="sourcePoint" />
             <Array as="points">
-              <mxPoint x="380" y="560" />
-              <mxPoint x="380" y="560" />
+              <mxPoint x="1720" y="-94" />
+              <mxPoint x="1720" y="-94" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-158" value="IntervalFeature" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="300" y="600" width="160" height="84" as="geometry" />
+        <mxCell id="wUrawppS3UO5J027udKO-69" value="- labelDesc" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="wUrawppS3UO5J027udKO-68" vertex="1" connectable="0">
+          <mxGeometry x="-0.7368" y="2" relative="1" as="geometry">
+            <mxPoint x="22" y="-6" as="offset" />
+          </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-159" value="-&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-158" vertex="1">
+        <mxCell id="wUrawppS3UO5J027udKO-7" value="DataDescriptor" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="1531" y="-170" width="160" height="84" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-8" value="-&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-7" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-160" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-158" vertex="1">
+        <mxCell id="wUrawppS3UO5J027udKO-9" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="wUrawppS3UO5J027udKO-7" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-161" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-158" vertex="1">
+        <mxCell id="wUrawppS3UO5J027udKO-10" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-7" vertex="1">
           <mxGeometry y="58" width="160" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-166" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-162" target="lsfipmTJbNCapsntxlYZ-158" edge="1">
-          <mxGeometry relative="1" as="geometry" />
+        <mxCell id="wUrawppS3UO5J027udKO-15" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=block;endFill=0;endSize=10;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="wUrawppS3UO5J027udKO-11" target="lsfipmTJbNCapsntxlYZ-13" edge="1">
+          <mxGeometry relative="1" as="geometry">
+            <Array as="points">
+              <mxPoint x="560" y="230" />
+              <mxPoint x="560" y="230" />
+            </Array>
+          </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-162" value="CellFeature" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="300" y="730" width="160" height="84" as="geometry" />
+        <mxCell id="wUrawppS3UO5J027udKO-16" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=open;endFill=0;endSize=10;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="wUrawppS3UO5J027udKO-11" target="lsfipmTJbNCapsntxlYZ-13" edge="1">
+          <mxGeometry relative="1" as="geometry">
+            <Array as="points">
+              <mxPoint x="630" y="240" />
+              <mxPoint x="630" y="240" />
+            </Array>
+          </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-163" value="-&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-162" vertex="1">
+        <mxCell id="wUrawppS3UO5J027udKO-32" value="*" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];rounded=0;shadow=0;strokeColor=default;strokeWidth=1;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;" parent="wUrawppS3UO5J027udKO-16" vertex="1" connectable="0">
+          <mxGeometry x="0.6846" y="1" relative="1" as="geometry">
+            <mxPoint x="11" y="1" as="offset" />
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-11" value="RepresentativePoint" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#fad9d5;strokeColor=#ae4132;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="550" y="260" width="160" height="84" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-12" value="-&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-11" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-164" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-162" vertex="1">
+        <mxCell id="wUrawppS3UO5J027udKO-13" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="wUrawppS3UO5J027udKO-11" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-165" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-162" vertex="1">
+        <mxCell id="wUrawppS3UO5J027udKO-14" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-11" vertex="1">
           <mxGeometry y="58" width="160" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-172" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-168" target="lsfipmTJbNCapsntxlYZ-19" edge="1">
+        <mxCell id="wUrawppS3UO5J027udKO-31" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=block;endFill=0;endSize=10;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="wUrawppS3UO5J027udKO-17" target="lsfipmTJbNCapsntxlYZ-19" edge="1">
+          <mxGeometry relative="1" as="geometry">
+            <Array as="points">
+              <mxPoint x="970" y="350" />
+              <mxPoint x="970" y="210" />
+              <mxPoint x="1040" y="210" />
+            </Array>
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-17" value="Rank" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="785" y="314" width="150" height="84" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-30" value="- desc: FeatureDescriptor" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-17" vertex="1">
+          <mxGeometry y="26" width="150" height="24" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-19" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="wUrawppS3UO5J027udKO-17" vertex="1">
+          <mxGeometry y="50" width="150" height="8" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-20" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-17" vertex="1">
+          <mxGeometry y="58" width="150" height="26" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-6" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=open;endFill=0;endSize=10;" edge="1" parent="WIyWlLk6GJQsqaUBKTNV-1" source="wUrawppS3UO5J027udKO-17" target="wUrawppS3UO5J027udKO-33">
+          <mxGeometry relative="1" as="geometry">
+            <Array as="points">
+              <mxPoint x="860" y="310" />
+              <mxPoint x="860" y="310" />
+            </Array>
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-9" value="1..*" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;" vertex="1" connectable="0" parent="CCnf-G1CkggKAS8I-f5b-6">
+          <mxGeometry x="0.821" y="1" relative="1" as="geometry">
+            <mxPoint x="21" y="2" as="offset" />
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-7" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=open;endFill=1;endSize=10;exitX=0.5;exitY=0;exitDx=0;exitDy=0;" edge="1" parent="WIyWlLk6GJQsqaUBKTNV-1" source="wUrawppS3UO5J027udKO-33" target="lsfipmTJbNCapsntxlYZ-19">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="760" y="142" />
+              <mxPoint x="860" y="160" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-173" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;jumpStyle=arc;endArrow=block;endSize=10;endFill=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-168" target="lsfipmTJbNCapsntxlYZ-143" edge="1">
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-8" value="1" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;" vertex="1" connectable="0" parent="CCnf-G1CkggKAS8I-f5b-7">
+          <mxGeometry x="0.7674" y="2" relative="1" as="geometry">
+            <mxPoint y="-8" as="offset" />
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-31" value="-value" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;" vertex="1" connectable="0" parent="CCnf-G1CkggKAS8I-f5b-7">
+          <mxGeometry x="-0.6138" y="2" relative="1" as="geometry">
+            <mxPoint as="offset" />
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-33" value="RankValue" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#b0e3e6;strokeColor=#0e8088;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="790" y="176" width="140" height="84" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-34" value="- proportion:float" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-33" vertex="1">
+          <mxGeometry y="26" width="140" height="24" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-35" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="wUrawppS3UO5J027udKO-33" vertex="1">
+          <mxGeometry y="50" width="140" height="8" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-36" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-33" vertex="1">
+          <mxGeometry y="58" width="140" height="26" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-61" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="wUrawppS3UO5J027udKO-55" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
+          <mxGeometry relative="1" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-62" value="- comparator" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="wUrawppS3UO5J027udKO-61" vertex="1" connectable="0">
+          <mxGeometry x="-0.6571" y="3" relative="1" as="geometry">
+            <mxPoint x="32" y="-3" as="offset" />
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-55" value="FeatureDescriptor" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="1805" y="-160" width="160" height="132" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-56" value="- order: int" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-55" vertex="1">
+          <mxGeometry y="26" width="160" height="24" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-59" value="- dtype: str" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-55" vertex="1">
+          <mxGeometry y="50" width="160" height="24" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-60" value="- text: str" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-55" vertex="1">
+          <mxGeometry y="74" width="160" height="24" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-57" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="wUrawppS3UO5J027udKO-55" vertex="1">
+          <mxGeometry y="98" width="160" height="8" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-58" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-55" vertex="1">
+          <mxGeometry y="106" width="160" height="26" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-66" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="wUrawppS3UO5J027udKO-7" target="wUrawppS3UO5J027udKO-55" edge="1">
           <mxGeometry relative="1" as="geometry">
+            <mxPoint x="1701" y="-130" as="sourcePoint" />
+            <mxPoint x="1815" y="-130" as="targetPoint" />
             <Array as="points">
-              <mxPoint x="760" y="560" />
-              <mxPoint x="410" y="560" />
+              <mxPoint x="1750" y="-110" />
+              <mxPoint x="1750" y="-110" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-168" value="DerrivedFeature" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="690" y="600" width="160" height="84" as="geometry" />
+        <mxCell id="wUrawppS3UO5J027udKO-67" value="- idDesc" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="wUrawppS3UO5J027udKO-66" vertex="1" connectable="0">
+          <mxGeometry x="-0.7544" y="1" relative="1" as="geometry">
+            <mxPoint x="16" y="-10" as="offset" />
+          </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-169" value="-&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-168" vertex="1">
+        <mxCell id="wUrawppS3UO5J027udKO-77" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=block;endFill=0;endSize=10;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="wUrawppS3UO5J027udKO-73" target="lsfipmTJbNCapsntxlYZ-39" edge="1">
+          <mxGeometry relative="1" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-73" value="RepresentativeTrajectory" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e51400;strokeColor=#B20000;fontColor=#ffffff;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="380" y="400" width="160" height="84" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-74" value="-&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-73" vertex="1">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-170" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-168" vertex="1">
+        <mxCell id="wUrawppS3UO5J027udKO-75" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="wUrawppS3UO5J027udKO-73" vertex="1">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-171" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-168" vertex="1">
+        <mxCell id="wUrawppS3UO5J027udKO-76" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-73" vertex="1">
           <mxGeometry y="58" width="160" height="26" as="geometry" />
         </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-79" value="NovoMovelets" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="-390" y="400" width="160" height="84" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-80" value="-" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-79" vertex="1">
+          <mxGeometry y="26" width="160" height="24" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-81" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="wUrawppS3UO5J027udKO-79" vertex="1">
+          <mxGeometry y="50" width="160" height="8" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-82" value="+" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="wUrawppS3UO5J027udKO-79" vertex="1">
+          <mxGeometry y="58" width="160" height="26" as="geometry" />
+        </mxCell>
+        <mxCell id="wUrawppS3UO5J027udKO-83" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=block;endFill=0;endSize=10;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="wUrawppS3UO5J027udKO-80" target="lsfipmTJbNCapsntxlYZ-126" edge="1">
+          <mxGeometry relative="1" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-28" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=block;endFill=0;endSize=10;" edge="1" parent="WIyWlLk6GJQsqaUBKTNV-1" source="CCnf-G1CkggKAS8I-f5b-0" target="wUrawppS3UO5J027udKO-2">
+          <mxGeometry relative="1" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-0" value="Interval" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#d5e8d4;strokeColor=#82b366;" vertex="1" parent="WIyWlLk6GJQsqaUBKTNV-1">
+          <mxGeometry x="1190" y="400" width="140" height="84" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-1" value="- end: timestamp" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-0">
+          <mxGeometry y="26" width="140" height="24" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-2" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-0">
+          <mxGeometry y="50" width="140" height="8" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-3" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-0">
+          <mxGeometry y="58" width="140" height="26" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-30" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=block;endFill=0;endSize=10;" edge="1" parent="WIyWlLk6GJQsqaUBKTNV-1" source="CCnf-G1CkggKAS8I-f5b-13" target="lsfipmTJbNCapsntxlYZ-19">
+          <mxGeometry relative="1" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-13" value="Numeric" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fontFamily=Helvetica;fontSize=12;strokeColor=#82b366;fontColor=default;fillColor=#d5e8d4;" vertex="1" parent="WIyWlLk6GJQsqaUBKTNV-1">
+          <mxGeometry x="1470" y="140" width="160" height="84" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-14" value="&lt;span style=&quot;font-weight: normal;&quot;&gt;&lt;i&gt;-&amp;nbsp;value&lt;span style=&quot;background-color: initial;&quot;&gt;: float&lt;/span&gt;&lt;/i&gt;&lt;/span&gt;" style="text;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;fontFamily=Helvetica;fontSize=12;fontStyle=1;fontColor=default;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-13">
+          <mxGeometry y="26" width="160" height="24" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-15" value="" style="line;strokeWidth=1;align=center;verticalAlign=top;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;fillColor=#d5e8d4;strokeColor=#82b366;fontFamily=Helvetica;fontSize=12;fontColor=default;fontStyle=1;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-13">
+          <mxGeometry y="50" width="160" height="8" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-16" value="+&amp;nbsp;" style="text;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;fontFamily=Helvetica;fontSize=12;fontStyle=1;fontColor=default;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-13">
+          <mxGeometry y="58" width="160" height="26" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-29" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=block;endFill=0;endSize=10;" edge="1" parent="WIyWlLk6GJQsqaUBKTNV-1" source="CCnf-G1CkggKAS8I-f5b-17" target="lsfipmTJbNCapsntxlYZ-19">
+          <mxGeometry relative="1" as="geometry">
+            <Array as="points">
+              <mxPoint x="1430" y="210" />
+              <mxPoint x="1083" y="210" />
+            </Array>
+          </mxGeometry>
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-17" value="Categoric" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fontFamily=Helvetica;fontSize=12;strokeColor=#82b366;fontColor=default;fillColor=#d5e8d4;" vertex="1" parent="WIyWlLk6GJQsqaUBKTNV-1">
+          <mxGeometry x="1350" y="236" width="160" height="84" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-18" value="&lt;span style=&quot;font-weight: normal;&quot;&gt;&lt;i&gt;-&amp;nbsp;value&lt;span style=&quot;background-color: initial;&quot;&gt;: str&lt;/span&gt;&lt;/i&gt;&lt;/span&gt;" style="text;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;fontFamily=Helvetica;fontSize=12;fontStyle=1;fontColor=default;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-17">
+          <mxGeometry y="26" width="160" height="24" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-19" value="" style="line;strokeWidth=1;align=center;verticalAlign=top;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;fillColor=#d5e8d4;strokeColor=#82b366;fontFamily=Helvetica;fontSize=12;fontColor=default;fontStyle=1;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-17">
+          <mxGeometry y="50" width="160" height="8" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-20" value="+&amp;nbsp;" style="text;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;fontFamily=Helvetica;fontSize=12;fontStyle=1;fontColor=default;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-17">
+          <mxGeometry y="58" width="160" height="26" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-24" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=block;endFill=0;endSize=10;" edge="1" parent="WIyWlLk6GJQsqaUBKTNV-1" source="CCnf-G1CkggKAS8I-f5b-21" target="lsfipmTJbNCapsntxlYZ-114">
+          <mxGeometry relative="1" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-21" value="Editl&lt;span style=&quot;background-color: initial;&quot;&gt;csDistance&lt;/span&gt;" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" vertex="1" parent="WIyWlLk6GJQsqaUBKTNV-1">
+          <mxGeometry x="1868" y="495" width="130" height="60" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-22" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-21">
+          <mxGeometry y="26" width="130" height="8" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-23" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-21">
+          <mxGeometry y="34" width="130" height="26" as="geometry" />
+        </mxCell>
       </root>
     </mxGraphModel>
   </diagram>
 </mxfile>
```

### Comparing `mat_model-0.1b1/pyproject.toml` & `mat_model-0.1b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 [project]
 name = "mat-model"
-version = "0.1b1"
+version = "0.1b2"
 description = "MAT-model: Model Classes for Multiple Aspect Trajectory Data Mining"
 authors = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
 maintainers = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
```

### Comparing `mat_model-0.1b1/setup.py` & `mat_model-0.1b2/setup.py`

 * *Files identical despite different names*

