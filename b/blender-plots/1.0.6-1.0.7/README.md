# Comparing `tmp/blender-plots-1.0.6.tar.gz` & `tmp/blender-plots-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blender-plots-1.0.6.tar", last modified: Mon May  6 16:38:00 2024, max compression
+gzip compressed data, was "blender-plots-1.0.7.tar", last modified: Thu May 23 12:51:37 2024, max compression
```

## Comparing `blender-plots-1.0.6.tar` & `blender-plots-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-06 16:38:00.528768 blender-plots-1.0.6/
--rw-rw-r--   0 linus     (1000) linus     (1000)    35149 2023-08-26 09:18:57.000000 blender-plots-1.0.6/LICENSE
--rw-rw-r--   0 linus     (1000) linus     (1000)      268 2024-05-06 16:38:00.528768 blender-plots-1.0.6/PKG-INFO
--rw-rw-r--   0 linus     (1000) linus     (1000)    12333 2024-02-10 13:48:12.000000 blender-plots-1.0.6/README.md
-drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-06 16:38:00.528768 blender-plots-1.0.6/blender_plots/
--rw-rw-r--   0 linus     (1000) linus     (1000)      216 2024-05-06 16:17:21.000000 blender-plots-1.0.6/blender_plots/__init__.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     5645 2024-02-02 20:12:46.000000 blender-plots-1.0.6/blender_plots/arrows.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     9481 2024-05-06 15:10:45.000000 blender-plots-1.0.6/blender_plots/blender_utils.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     2269 2024-05-06 16:34:56.000000 blender-plots-1.0.6/blender_plots/marker_utils.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     5453 2024-05-06 15:17:02.000000 blender-plots-1.0.6/blender_plots/plots_base.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     9484 2024-05-06 15:54:55.000000 blender-plots-1.0.6/blender_plots/scatter.py
--rw-rw-r--   0 linus     (1000) linus     (1000)     3133 2023-12-05 22:14:57.000000 blender-plots-1.0.6/blender_plots/surface.py
-drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-06 16:38:00.528768 blender-plots-1.0.6/blender_plots.egg-info/
--rw-r--r--   0 linus     (1000) linus     (1000)      268 2024-05-06 16:38:00.000000 blender-plots-1.0.6/blender_plots.egg-info/PKG-INFO
--rw-rw-r--   0 linus     (1000) linus     (1000)      363 2024-05-06 16:38:00.000000 blender-plots-1.0.6/blender_plots.egg-info/SOURCES.txt
--rw-rw-r--   0 linus     (1000) linus     (1000)        1 2024-05-06 16:38:00.000000 blender-plots-1.0.6/blender_plots.egg-info/dependency_links.txt
--rw-rw-r--   0 linus     (1000) linus     (1000)       14 2024-05-06 16:38:00.000000 blender-plots-1.0.6/blender_plots.egg-info/top_level.txt
--rw-rw-r--   0 linus     (1000) linus     (1000)       38 2024-05-06 16:38:00.528768 blender-plots-1.0.6/setup.cfg
--rw-rw-r--   0 linus     (1000) linus     (1000)      283 2024-05-06 16:21:03.000000 blender-plots-1.0.6/setup.py
+drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-23 12:51:37.806628 blender-plots-1.0.7/
+-rw-rw-r--   0 linus     (1000) linus     (1000)    35149 2023-08-26 09:18:57.000000 blender-plots-1.0.7/LICENSE
+-rw-rw-r--   0 linus     (1000) linus     (1000)      268 2024-05-23 12:51:37.806628 blender-plots-1.0.7/PKG-INFO
+-rw-rw-r--   0 linus     (1000) linus     (1000)    12333 2024-02-10 13:48:12.000000 blender-plots-1.0.7/README.md
+drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-23 12:51:37.806628 blender-plots-1.0.7/blender_plots/
+-rw-rw-r--   0 linus     (1000) linus     (1000)      216 2024-05-06 16:17:21.000000 blender-plots-1.0.7/blender_plots/__init__.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     5645 2024-02-02 20:12:46.000000 blender-plots-1.0.7/blender_plots/arrows.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)    10320 2024-05-23 12:50:22.000000 blender-plots-1.0.7/blender_plots/blender_utils.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     2269 2024-05-06 16:34:56.000000 blender-plots-1.0.7/blender_plots/marker_utils.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     5453 2024-05-06 15:17:02.000000 blender-plots-1.0.7/blender_plots/plots_base.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     9484 2024-05-06 15:54:55.000000 blender-plots-1.0.7/blender_plots/scatter.py
+-rw-rw-r--   0 linus     (1000) linus     (1000)     3133 2023-12-05 22:14:57.000000 blender-plots-1.0.7/blender_plots/surface.py
+drwxrwxr-x   0 linus     (1000) linus     (1000)        0 2024-05-23 12:51:37.806628 blender-plots-1.0.7/blender_plots.egg-info/
+-rw-r--r--   0 linus     (1000) linus     (1000)      268 2024-05-23 12:51:37.000000 blender-plots-1.0.7/blender_plots.egg-info/PKG-INFO
+-rw-rw-r--   0 linus     (1000) linus     (1000)      363 2024-05-23 12:51:37.000000 blender-plots-1.0.7/blender_plots.egg-info/SOURCES.txt
+-rw-rw-r--   0 linus     (1000) linus     (1000)        1 2024-05-23 12:51:37.000000 blender-plots-1.0.7/blender_plots.egg-info/dependency_links.txt
+-rw-rw-r--   0 linus     (1000) linus     (1000)       14 2024-05-23 12:51:37.000000 blender-plots-1.0.7/blender_plots.egg-info/top_level.txt
+-rw-rw-r--   0 linus     (1000) linus     (1000)       38 2024-05-23 12:51:37.806628 blender-plots-1.0.7/setup.cfg
+-rw-rw-r--   0 linus     (1000) linus     (1000)      283 2024-05-23 12:50:41.000000 blender-plots-1.0.7/setup.py
```

### Comparing `blender-plots-1.0.6/LICENSE` & `blender-plots-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.6/README.md` & `blender-plots-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.6/blender_plots/arrows.py` & `blender-plots-1.0.7/blender_plots/arrows.py`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.6/blender_plots/blender_utils.py` & `blender-plots-1.0.7/blender_plots/blender_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,27 +90,30 @@
 def new_collection(name):
     if name in bpy.data.collections:
         delete(bpy.data.collections[name], with_children=True)
     collection = bpy.data.collections.new(name)
     bpy.context.collection.children.link(collection)
     return collection
 
-def new_empty(name, object_data=None, select=True, collection=None):
+def new_empty(name, object_data=None, select=True, collection=None, location=None, rotation_euler=None):
     """Create new empty blender object with specified name and data, deletes any previous object with the same name."""
     if name in bpy.data.objects:
         delete(bpy.data.objects[name], with_children=True)
 
     new_object = bpy.data.objects.new(name, object_data)
     if collection is None:
         collection = bpy.context.collection
     collection.objects.link(new_object)
 
     if select:
         bpy.context.view_layer.objects.active = new_object
-
+    if location is not None:
+        new_object.location = location
+    if rotation_euler is not None:
+        new_object.rotation_euler = rotation_euler
     return new_object
 
 
 def add_modifier(base_object, modifier_type, **kwargs):
     modifier = base_object.modifiers.new(name=modifier_type.lower(), type=modifier_type)
     for key, value in kwargs.items():
         setattr(modifier, key, value)
@@ -214,7 +217,26 @@
     fcurve.keyframe_points.foreach_set("co", [0, 0, n_frames, n_frames])
     bpy.context.scene.frame_end = n_frames - 1
 
     modifier.node_group.animation_data_create()
     modifier.node_group.animation_data.action = action
 
     return frame_selection_node
+
+def new_mesh(vertices, faces, name='mesh', color=None, location=None, rotation_euler=None):
+    """Create mesh with uniform color."""
+    bmesh = bpy.data.meshes.new(name=name)
+    bmesh.from_pydata(vertices, [], faces)
+    mesh_object = new_empty(
+        name,
+        bmesh,
+        location=location,
+        rotation_euler=rotation_euler,
+    )
+
+    if color is not None:
+        material = bpy.data.materials.new(name)
+        material.use_nodes = True
+        bsdf = material.node_tree.nodes['Principled BSDF']
+        bsdf.inputs['Base Color'].default_value = color
+        mesh_object.data.materials.append(material)
+    return mesh_object
```

### Comparing `blender-plots-1.0.6/blender_plots/marker_utils.py` & `blender-plots-1.0.7/blender_plots/marker_utils.py`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.6/blender_plots/plots_base.py` & `blender-plots-1.0.7/blender_plots/plots_base.py`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.6/blender_plots/scatter.py` & `blender-plots-1.0.7/blender_plots/scatter.py`

 * *Files identical despite different names*

### Comparing `blender-plots-1.0.6/blender_plots/surface.py` & `blender-plots-1.0.7/blender_plots/surface.py`

 * *Files identical despite different names*

