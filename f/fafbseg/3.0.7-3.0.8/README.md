# Comparing `tmp/fafbseg-3.0.7.tar.gz` & `tmp/fafbseg-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fafbseg-3.0.7.tar", last modified: Thu May 16 08:52:49 2024, max compression
+gzip compressed data, was "fafbseg-3.0.8.tar", last modified: Thu May 23 19:34:33 2024, max compression
```

## Comparing `fafbseg-3.0.7.tar` & `fafbseg-3.0.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.817164 fafbseg-3.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 08:52:47.000000 fafbseg-3.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-16 08:52:47.000000 fafbseg-3.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-16 08:52:49.817164 fafbseg-3.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-16 08:52:47.000000 fafbseg-3.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.797164 fafbseg-3.0.7/fafbseg/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.809164 fafbseg-3.0.7/fafbseg/data/
--rw-r--r--   0 runner    (1001) docker     (127)  2425791 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/data/JFRC2NP.surf.fw.zip
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)  6675604 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/data/global_area_ids.npy.zip
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/data/ngl_scenes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/data/volume_name_dict.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.813164 fafbseg-3.0.7/fafbseg/flywire/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18713 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/_synapses_spine.py
--rw-r--r--   0 runner    (1001) docker     (127)    91701 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.813164 fafbseg-3.0.7/fafbseg/flywire/blender/
--rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/blender/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.813164 fafbseg-3.0.7/fafbseg/flywire/blender/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/blender/templates/blender_render.py.template
--rw-r--r--   0 runner    (1001) docker     (127)    34585 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/l2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/meshes.py
--rw-r--r--   0 runner    (1001) docker     (127)    31311 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/neuroglancer.py
--rw-r--r--   0 runner    (1001) docker     (127)    63928 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26185 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/skeletonize.py
--rw-r--r--   0 runner    (1001) docker     (127)    57617 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/synapses.py
--rw-r--r--   0 runner    (1001) docker     (127)    26338 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/flywire/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.813164 fafbseg-3.0.7/fafbseg/google/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/google/meshes.py
--rw-r--r--   0 runner    (1001) docker     (127)    31298 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/google/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/google/synapses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.813164 fafbseg-3.0.7/fafbseg/move/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/move/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/move/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    24195 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/move/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/move/merge_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.813164 fafbseg-3.0.7/fafbseg/spine/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/spine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26285 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/spine/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.817164 fafbseg-3.0.7/fafbseg/synapses/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/synapses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25192 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/synapses/offline.py
--rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/synapses/online.py
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/synapses/transmitters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/synapses/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.817164 fafbseg-3.0.7/fafbseg/xform/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/xform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-05-16 08:52:47.000000 fafbseg-3.0.7/fafbseg/xform/xform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:52:49.817164 fafbseg-3.0.7/fafbseg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-16 08:52:49.000000 fafbseg-3.0.7/fafbseg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-16 08:52:49.000000 fafbseg-3.0.7/fafbseg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:52:49.000000 fafbseg-3.0.7/fafbseg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:52:49.000000 fafbseg-3.0.7/fafbseg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 08:52:49.000000 fafbseg-3.0.7/fafbseg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 08:52:49.000000 fafbseg-3.0.7/fafbseg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 08:52:49.817164 fafbseg-3.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-16 08:52:47.000000 fafbseg-3.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:34:33.791128 fafbseg-3.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 19:34:31.000000 fafbseg-3.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-23 19:34:31.000000 fafbseg-3.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-23 19:34:33.791128 fafbseg-3.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-23 19:34:31.000000 fafbseg-3.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:34:33.767128 fafbseg-3.0.8/fafbseg/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:34:33.783128 fafbseg-3.0.8/fafbseg/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  2425791 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/data/JFRC2NP.surf.fw.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)  6675604 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/data/global_area_ids.npy.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/data/ngl_scenes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/data/volume_name_dict.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:34:33.783128 fafbseg-3.0.8/fafbseg/flywire/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18713 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/_synapses_spine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91701 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:34:33.783128 fafbseg-3.0.8/fafbseg/flywire/blender/
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/blender/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:34:33.783128 fafbseg-3.0.8/fafbseg/flywire/blender/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/blender/templates/blender_render.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)    34585 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/l2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31311 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/neuroglancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63928 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26185 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/skeletonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57617 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/synapses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26338 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/flywire/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:34:33.787128 fafbseg-3.0.8/fafbseg/google/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/google/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31298 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/google/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/google/synapses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:34:33.787128 fafbseg-3.0.8/fafbseg/move/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/move/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/move/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24195 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/move/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/move/merge_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:34:33.787128 fafbseg-3.0.8/fafbseg/spine/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/spine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26285 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/spine/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:34:33.787128 fafbseg-3.0.8/fafbseg/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/synapses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25192 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/synapses/offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/synapses/online.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/synapses/transmitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/synapses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:34:33.787128 fafbseg-3.0.8/fafbseg/xform/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/xform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-05-23 19:34:31.000000 fafbseg-3.0.8/fafbseg/xform/xform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:34:33.787128 fafbseg-3.0.8/fafbseg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-23 19:34:33.000000 fafbseg-3.0.8/fafbseg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-23 19:34:33.000000 fafbseg-3.0.8/fafbseg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:34:33.000000 fafbseg-3.0.8/fafbseg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:34:33.000000 fafbseg-3.0.8/fafbseg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 19:34:33.000000 fafbseg-3.0.8/fafbseg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 19:34:33.000000 fafbseg-3.0.8/fafbseg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:34:33.791128 fafbseg-3.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-23 19:34:31.000000 fafbseg-3.0.8/setup.py
```

### Comparing `fafbseg-3.0.7/LICENSE` & `fafbseg-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/PKG-INFO` & `fafbseg-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fafbseg
-Version: 3.0.7
+Version: 3.0.8
 Summary: Tools to work with the FlyWire and Google segmentations of the FAFB EM dataset
 Home-page: https://fafbseg-py.readthedocs.io
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, https://fafbseg-py.readthedocs.io
 Project-URL: Source, https://github.com/navis-org/fafbseg-py
```

### Comparing `fafbseg-3.0.7/README.md` & `fafbseg-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/__init__.py` & `fafbseg-3.0.8/fafbseg/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/data/JFRC2NP.surf.fw.zip` & `fafbseg-3.0.8/fafbseg/data/JFRC2NP.surf.fw.zip`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/data/global_area_ids.npy.zip` & `fafbseg-3.0.8/fafbseg/data/global_area_ids.npy.zip`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/data/ngl_scenes.json` & `fafbseg-3.0.8/fafbseg/data/ngl_scenes.json`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/data/volume_name_dict.json` & `fafbseg-3.0.8/fafbseg/data/volume_name_dict.json`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/__init__.py` & `fafbseg-3.0.8/fafbseg/flywire/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/_synapses_spine.py` & `fafbseg-3.0.8/fafbseg/flywire/_synapses_spine.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/annotations.py` & `fafbseg-3.0.8/fafbseg/flywire/annotations.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/blender/__init__.py` & `fafbseg-3.0.8/fafbseg/flywire/blender/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/blender/templates/blender_render.py.template` & `fafbseg-3.0.8/fafbseg/flywire/blender/templates/blender_render.py.template`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/l2.py` & `fafbseg-3.0.8/fafbseg/flywire/l2.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/merge.py` & `fafbseg-3.0.8/fafbseg/flywire/merge.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/meshes.py` & `fafbseg-3.0.8/fafbseg/flywire/meshes.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/neuroglancer.py` & `fafbseg-3.0.8/fafbseg/flywire/neuroglancer.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/segmentation.py` & `fafbseg-3.0.8/fafbseg/flywire/segmentation.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/skeletonize.py` & `fafbseg-3.0.8/fafbseg/flywire/skeletonize.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/synapses.py` & `fafbseg-3.0.8/fafbseg/flywire/synapses.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/flywire/utils.py` & `fafbseg-3.0.8/fafbseg/flywire/utils.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/google/__init__.py` & `fafbseg-3.0.8/fafbseg/google/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/google/meshes.py` & `fafbseg-3.0.8/fafbseg/google/meshes.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/google/segmentation.py` & `fafbseg-3.0.8/fafbseg/google/segmentation.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/google/synapses.py` & `fafbseg-3.0.8/fafbseg/google/synapses.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/move/__init__.py` & `fafbseg-3.0.8/fafbseg/move/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/move/interfaces.py` & `fafbseg-3.0.8/fafbseg/move/interfaces.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/move/merge.py` & `fafbseg-3.0.8/fafbseg/move/merge.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/move/merge_utils.py` & `fafbseg-3.0.8/fafbseg/move/merge_utils.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/spine/__init__.py` & `fafbseg-3.0.8/fafbseg/spine/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/spine/base.py` & `fafbseg-3.0.8/fafbseg/spine/base.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/synapses/__init__.py` & `fafbseg-3.0.8/fafbseg/synapses/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/synapses/offline.py` & `fafbseg-3.0.8/fafbseg/synapses/offline.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/synapses/online.py` & `fafbseg-3.0.8/fafbseg/synapses/online.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/synapses/transmitters.py` & `fafbseg-3.0.8/fafbseg/synapses/transmitters.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/synapses/utils.py` & `fafbseg-3.0.8/fafbseg/synapses/utils.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/utils.py` & `fafbseg-3.0.8/fafbseg/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,19 +93,19 @@
     url :       str
 
     """
     # Generate the URL
     url = args[0]
     for arg in args[1:]:
         arg_str = str(arg)
-        joiner = '' if url.endswith('/') else '/'
-        relative = arg_str[1:] if arg_str.startswith('/') else arg_str
+        joiner = "" if url.endswith("/") else "/"
+        relative = arg_str[1:] if arg_str.startswith("/") else arg_str
         url = requests.compat.urljoin(url + joiner, relative)
     if GET:
-        url += '?{}'.format(urlencode(GET))
+        url += "?{}".format(urlencode(GET))
     return url
 
 
 def make_iterable(x, force_type=None) -> np.ndarray:
     """Force input into a numpy array.
 
     For dicts, keys will be turned into array.
@@ -153,31 +153,33 @@
         points = np.asarray(points)
 
         if isinstance(self._points, type(None)):
             self._points = points
         else:
             self._points = np.concat(self._points, points)
 
-        resolution = np.array(self._volume.scale['resolution'])
-        chunk_size = np.array(self._volume.scale['chunk_sizes'])
+        resolution = np.array(self._volume.scale["resolution"])
+        chunk_size = np.array(self._volume.scale["chunk_sizes"])
         chunk_starts = (points // resolution).astype(int) // chunk_size * chunk_size
         for point, chunk_start in zip(points, chunk_starts):
             self._chunk_map[tuple(chunk_start)].add(tuple(point))
 
     def _load_chunk(self, chunk_start, chunk_end):
         # (No validation that this is a valid chunk_start.)
-        return self._volume[chunk_start[0]:chunk_end[0],
-                            chunk_start[1]:chunk_end[1],
-                            chunk_start[2]:chunk_end[2]]
+        return self._volume[
+            chunk_start[0] : chunk_end[0],
+            chunk_start[1] : chunk_end[1],
+            chunk_start[2] : chunk_end[2],
+        ]
 
     def _load_points(self, chunk_map_key):
         chunk_start = np.array(chunk_map_key)
         points = np.array(list(self._chunk_map[chunk_map_key]))
 
-        resolution = np.array(self._volume.scale['resolution'])
+        resolution = np.array(self._volume.scale["resolution"])
         indices = (points // resolution).astype(int) - chunk_start
 
         # We don't really need to load the whole chunk here:
         # Instead, we subset the chunk to the part that contains our points
         # This should at the very least save memory
         mn, mx = indices.min(axis=0), indices.max(axis=0)
 
@@ -208,29 +210,37 @@
                         Parallel Numpy arrays of the requested points from all
                         cumulative calls to add_points, and the corresponding
                         data loaded from volume.
 
         """
         progress_state = self._volume.progress
         self._volume.progress = False
-        with tqdm(total=len(self._chunk_map),
-                  desc='Segmentation IDs',
-                  leave=False,
-                  disable=not progress) as pbar:
+        with tqdm(
+            total=len(self._chunk_map),
+            desc="Segmentation IDs",
+            leave=False,
+            disable=not progress,
+        ) as pbar:
             with futures.ProcessPoolExecutor(max_workers=max_workers) as ex:
-                point_futures = [ex.submit(self._load_points, k) for k in self._chunk_map]
+                point_futures = [
+                    ex.submit(self._load_points, k) for k in self._chunk_map
+                ]
                 for f in futures.as_completed(point_futures):
                     pbar.update(1)
         self._volume.progress = progress_state
 
         results = [f.result() for f in point_futures]
 
         if return_sorted:
-            points_dict = dict(zip([tuple(p) for result in results for p in result[0]],
-                                   [i for result in results for i in result[1]]))
+            points_dict = dict(
+                zip(
+                    [tuple(p) for result in results for p in result[0]],
+                    [i for result in results for i in result[1]],
+                )
+            )
 
             data = np.array([points_dict[tuple(p)] for p in self._points])
             points = self._points
         else:
             points = np.concatenate([result[0] for result in results])
             data = np.concatenate([result[1] for result in results])
 
@@ -276,13 +286,13 @@
             print(
                 f"Caching {fp.name} from {urlparse(url).netloc}... ", end="", flush=True
             )
         r = requests.get(url, allow_redirects=True)
         r.raise_for_status()
         content_type = r.headers.get("content-type", "").lower()
         is_text = "text" in content_type or "html" in content_type
-        with open(fp, mode="w" if is_text else "w") as f:
-            f.write(r.content.decode())
+        with open(fp, mode="w" if is_text else "w", encoding="utf-8") as f:
+            f.write(r.content.decode("utf-8"))
         if verbose and not os.environ.get("FAFBSEG_TESTING", False):
             print("Done.")
 
-    return fp
+    return fp
```

### Comparing `fafbseg-3.0.7/fafbseg/xform/__init__.py` & `fafbseg-3.0.8/fafbseg/xform/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg/xform/xform.py` & `fafbseg-3.0.8/fafbseg/xform/xform.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/fafbseg.egg-info/PKG-INFO` & `fafbseg-3.0.8/fafbseg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fafbseg
-Version: 3.0.7
+Version: 3.0.8
 Summary: Tools to work with the FlyWire and Google segmentations of the FAFB EM dataset
 Home-page: https://fafbseg-py.readthedocs.io
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, https://fafbseg-py.readthedocs.io
 Project-URL: Source, https://github.com/navis-org/fafbseg-py
```

### Comparing `fafbseg-3.0.7/fafbseg.egg-info/SOURCES.txt` & `fafbseg-3.0.8/fafbseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.7/setup.py` & `fafbseg-3.0.8/setup.py`

 * *Files identical despite different names*

