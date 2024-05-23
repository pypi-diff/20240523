# Comparing `tmp/model_resolver-0.4.0.tar.gz` & `tmp/model_resolver-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_resolver-0.4.0.tar", max compression
+gzip compressed data, was "model_resolver-0.5.0.tar", max compression
```

## Comparing `model_resolver-0.4.0.tar` & `model_resolver-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2024-05-13 15:53:53.609718 model_resolver-0.4.0/LICENSE
--rw-r--r--   0        0        0     1752 2024-05-13 15:53:53.609718 model_resolver-0.4.0/README.md
--rw-r--r--   0        0        0       36 2024-05-13 15:53:53.609718 model_resolver-0.4.0/model_resolver/__init__.py
--rw-r--r--   0        0        0       59 2024-05-13 15:53:53.609718 model_resolver-0.4.0/model_resolver/__main__.py
--rw-r--r--   0        0        0     1623 2024-05-13 15:53:53.609718 model_resolver-0.4.0/model_resolver/cli.py
--rw-r--r--   0        0        0     1474 2024-05-13 15:53:53.609718 model_resolver-0.4.0/model_resolver/my_glutinit.py
--rw-r--r--   0        0        0    13881 2024-05-13 15:53:53.609718 model_resolver-0.4.0/model_resolver/plugin.py
--rw-r--r--   0        0        0    19633 2024-05-13 15:53:53.609718 model_resolver-0.4.0/model_resolver/render.py
--rw-r--r--   0        0        0     1248 2024-05-13 15:53:53.609718 model_resolver-0.4.0/model_resolver/utils.py
--rw-r--r--   0        0        0      715 2024-05-13 15:54:10.165751 model_resolver-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-23 12:22:08.095643 model_resolver-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1752 2024-05-23 12:22:08.095643 model_resolver-0.5.0/README.md
+-rw-r--r--   0        0        0       36 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/__main__.py
+-rw-r--r--   0        0        0     1951 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/cli.py
+-rw-r--r--   0        0        0     1474 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/my_glutinit.py
+-rw-r--r--   0        0        0    14567 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/plugin.py
+-rw-r--r--   0        0        0    19793 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/render.py
+-rw-r--r--   0        0        0     1248 2024-05-23 12:22:08.099643 model_resolver-0.5.0/model_resolver/utils.py
+-rw-r--r--   0        0        0      756 2024-05-23 12:22:25.683667 model_resolver-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.5.0/PKG-INFO
```

### Comparing `model_resolver-0.4.0/LICENSE` & `model_resolver-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `model_resolver-0.4.0/README.md` & `model_resolver-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `model_resolver-0.4.0/model_resolver/my_glutinit.py` & `model_resolver-0.5.0/model_resolver/my_glutinit.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.4.0/model_resolver/plugin.py` & `model_resolver-0.5.0/model_resolver/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,36 +7,45 @@
 from copy import deepcopy
 from typing import TypedDict
 from PIL import Image
 import json
 from model_resolver.utils import load_textures
 import numpy as np
 import hashlib
+import logging
+
+logger = logging.getLogger("model_resolver")
 
 
 def beet_default(ctx: Context):
     load_vanilla = ctx.meta.get("model_resolver", {}).get("load_vanilla", False)
+    resolve_vanilla_atlas = ctx.meta.get("model_resolver", {}).get("resolve_vanilla_atlas", False)
+    if load_vanilla:
+        resolve_vanilla_atlas = True
     use_cache = ctx.meta.get("model_resolver", {}).get("use_cache", False)
     render_size = ctx.meta.get("model_resolver", {}).get("render_size", 1024)
     minecraft_version = ctx.meta.get("model_resolver", {}).get(
         "minecraft_version", "latest"
     )
+    vanilla_filter = ctx.meta.get("model_resolver", {}).get("vanilla_filter", None)
 
     vanilla = ctx.inject(Vanilla)
     if not minecraft_version == "latest":
         vanilla = vanilla.releases[minecraft_version]
     generated_models = set()
     generated_textures = set()
 
     for atlas in ctx.assets.atlases:
         resolve_atlas(ctx, vanilla, ctx, atlas, generated_textures)
-    if load_vanilla:
+    if resolve_vanilla_atlas:
         for atlas in vanilla.assets.atlases:
             resolve_atlas(ctx, vanilla, vanilla, atlas, generated_textures)
-        render_vanilla(ctx, vanilla, generated_models)
+    if load_vanilla:
+        render_vanilla(ctx, vanilla, generated_models, vanilla_filter)
+    
 
     cache = ctx.cache.get("model_resolver")
     if not "models" in cache.json:
         cache.json["models"] = {}
         cache.json["render_size"] = render_size
         cache.json["minecraft_version"] = minecraft_version
         use_cache = False
@@ -44,14 +53,15 @@
         not cache.json["render_size"] == render_size
         or not cache.json["minecraft_version"] == minecraft_version
     ):
         use_cache = False
         cache.json["render_size"] = render_size
         cache.json["minecraft_version"] = minecraft_version
 
+    logger.info(f"Resolving models...")
     models = {}
     for model in set(ctx.assets.models.keys()):
         resolved_model = resolve_model(ctx.assets.models[model], vanilla.assets.models)
         resolved_model = bake_model(
             resolved_model, ctx, vanilla, model, generated_textures
         )
         if not "textures" in resolved_model.data:
@@ -63,19 +73,22 @@
                 model_name = model.split(":")
                 texture_path = f"{model_name[0]}:render/{model_name[1]}"
                 ctx.assets.textures[texture_path] = Texture(img)
                 continue
 
         models[model] = resolved_model.data
 
+    logger.info(f"Handling animations...")
     models = handle_animations(models, ctx, vanilla, generated_textures)
 
     if len(models) > 0:
+        logger.info(f"Rendering models...")
         Render(models, ctx, vanilla).render()
 
+    logger.info(f"Cleaning up...")
     clean_generated(ctx, generated_textures, generated_models)
 
 
 def handle_cache(cache: Cache, model, resolved_model, ctx, vanilla):
     model_hash = hashlib.sha256(str(resolved_model.data).encode()).hexdigest()
     cached_model_hash = cache.json["models"][model]["model"]
     if model_hash != cached_model_hash:
@@ -91,18 +104,21 @@
 
     # load cached image
     img_path = cache.get_path(f"{model}.png")
     img = Image.open(img_path)
     return img
 
 
-def render_vanilla(ctx: Context, vanilla: Vanilla, models: set[str]):
+def render_vanilla(ctx: Context, vanilla: Vanilla, models: set[str], vanilla_filter : list[str] | None):
     vanilla_models = vanilla.assets.models
 
     for model in vanilla_models.match("minecraft:*"):
+        if vanilla_filter is not None and len(vanilla_filter) > 0:
+            if not model in vanilla_filter:
+                continue
         if "parent" in vanilla_models[model].data:
             if vanilla_models[model].data["parent"] == "builtin/entity":
                 continue
         if model not in ctx.assets.models:
             ctx.assets.models[model] = vanilla_models[model]
             models.add(model)
```

### Comparing `model_resolver-0.4.0/model_resolver/render.py` & `model_resolver-0.5.0/model_resolver/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from beet import Context, Texture
 from beet.contrib.vanilla import Vanilla
 
 from math import cos, sin, pi, sqrt
 from rich import print
 import hashlib
 from model_resolver.utils import load_textures
+import logging
 
 
 class RenderError(Exception):
     pass
 
 
 class Render:
@@ -78,14 +79,15 @@
         self.textures = load_textures(
             self.models[self.model_list[self.current_model_index]]["textures"],
             self.ctx,
             self.vanilla,
         )
         self.reset_camera()
         self.frame_count = 0
+        self.logger = logging.getLogger("model_resolver")
 
     def reset_camera(self):
         self.translate = [0, 0, 0]
         self.rotate = [0, 0, 0]
 
     def reload(self):
         self.textures_bindings = {}
@@ -181,14 +183,15 @@
             self.ctx.assets.textures[texture_path] = Texture(img)
 
             self.cache_in_ctx(img)
             self.current_model_index += 1
             if self.current_model_index >= len(self.model_list):
                 glutLeaveMainLoop()
                 return
+            self.logger.info(f"Rendering {self.model_list[self.current_model_index]}")
             self.reload()
             self.reset_camera()
 
             # glutSwapBuffers()
         except BaseException as e:
             glutLeaveMainLoop()
             raise e
```

### Comparing `model_resolver-0.4.0/model_resolver/utils.py` & `model_resolver-0.5.0/model_resolver/utils.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.4.0/pyproject.toml` & `model_resolver-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "model-resolver"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["edayot <pro.e.dayot@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -34,10 +34,11 @@
 
 [tool.beet.resource_pack]
 load = "."
 
 [tool.beet.meta.model_resolver]
 load_vanilla = true
 use_cache = false
-render_size = 1024
+render_size = 256
 minecraft_version = "latest"
+vanilla_filter = ["minecraft:item/stone"]
```

### Comparing `model_resolver-0.4.0/PKG-INFO` & `model_resolver-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-resolver
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 License: MIT
 Author: edayot
 Author-email: pro.e.dayot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

