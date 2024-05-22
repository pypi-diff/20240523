# Comparing `tmp/madokami-0.1.4.tar.gz` & `tmp/madokami-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madokami-0.1.4.tar", max compression
+gzip compressed data, was "madokami-0.1.5.tar", max compression
```

## Comparing `madokami-0.1.4.tar` & `madokami-0.1.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0       26 2024-05-18 20:36:30.412937 madokami-0.1.4/README.md
--rw-r--r--   0        0        0      160 2024-04-21 19:50:38.326411 madokami-0.1.4/madokami/__init__.py
--rw-r--r--   0        0        0      602 2024-05-18 07:22:56.118748 madokami-0.1.4/madokami/api/__init__.py
--rw-r--r--   0        0        0      525 2024-05-18 07:23:24.607036 madokami-0.1.4/madokami/api/app.py
--rw-r--r--   0        0        0     4074 2024-05-18 01:58:36.106403 madokami-0.1.4/madokami/api/downloads.py
--rw-r--r--   0        0        0     1171 2024-05-13 02:49:57.491222 madokami-0.1.4/madokami/api/engines.py
--rw-r--r--   0        0        0      517 2024-05-17 02:48:25.866035 madokami-0.1.4/madokami/api/logs.py
--rw-r--r--   0        0        0     2189 2024-04-30 05:00:11.850809 madokami-0.1.4/madokami/api/media.py
--rw-r--r--   0        0        0     3015 2024-05-18 07:01:02.388989 madokami-0.1.4/madokami/api/models.py
--rw-r--r--   0        0        0     1948 2024-05-12 13:33:26.276521 madokami-0.1.4/madokami/api/plugins.py
--rw-r--r--   0        0        0     1496 2024-05-17 23:53:16.295962 madokami-0.1.4/madokami/api/register.py
--rw-r--r--   0        0        0     2627 2024-05-18 06:58:58.825707 madokami-0.1.4/madokami/api/scheduler.py
--rw-r--r--   0        0        0     1957 2024-05-15 16:19:59.207775 madokami-0.1.4/madokami/api/settings.py
--rw-r--r--   0        0        0     3021 2024-05-17 04:28:28.426201 madokami-0.1.4/madokami/api/subscribe.py
--rw-r--r--   0        0        0        0 2024-04-29 01:48:06.182046 madokami-0.1.4/madokami/api/utils.py
--rw-r--r--   0        0        0      215 2024-04-21 19:50:38.330738 madokami-0.1.4/madokami/app.py
--rw-r--r--   0        0        0     1088 2024-05-18 18:47:45.951393 madokami-0.1.4/madokami/config.py
--rw-r--r--   0        0        0     7854 2024-05-18 06:56:28.905698 madokami-0.1.4/madokami/crud.py
--rw-r--r--   0        0        0      748 2024-04-18 18:55:51.445120 madokami-0.1.4/madokami/db.py
--rw-r--r--   0        0        0       58 2024-04-19 16:00:57.987815 madokami-0.1.4/madokami/drivers/__init__.py
--rw-r--r--   0        0        0     1143 2024-05-18 22:04:37.489617 madokami-0.1.4/madokami/drivers/app.py
--rw-r--r--   0        0        0      691 2024-05-18 22:07:18.555001 madokami-0.1.4/madokami/drivers/deps.py
--rw-r--r--   0        0        0     1150 2024-04-19 15:58:56.300037 madokami-0.1.4/madokami/drivers/hooks.py
--rw-r--r--   0        0        0     3317 2024-05-18 07:22:56.125901 madokami-0.1.4/madokami/drivers/madokami.py
--rw-r--r--   0        0        0      276 2024-04-21 20:05:51.108606 madokami-0.1.4/madokami/drivers/router.py
--rw-r--r--   0        0        0        0 2024-04-17 21:56:18.236636 madokami-0.1.4/madokami/internal/__init__.py
--rw-r--r--   0        0        0     1082 2024-05-17 04:02:26.686931 madokami-0.1.4/madokami/internal/core_config.py
--rw-r--r--   0        0        0        0 2024-04-29 09:24:55.711542 madokami-0.1.4/madokami/internal/default_plugins/__init__.py
--rw-r--r--   0        0        0     2103 2024-04-29 09:27:02.804424 madokami-0.1.4/madokami/internal/default_plugins/bangumi_requester.py
--rw-r--r--   0        0        0     8975 2024-05-20 05:37:25.593524 madokami-0.1.4/madokami/internal/default_plugins/default_downloader.py
--rw-r--r--   0        0        0     1220 2024-05-18 15:15:17.837703 madokami-0.1.4/madokami/internal/default_plugins/default_requester.py
--rw-r--r--   0        0        0     1569 2024-04-29 03:28:47.980966 madokami-0.1.4/madokami/internal/downloader.py
--rw-r--r--   0        0        0     2337 2024-05-16 22:38:56.274073 madokami-0.1.4/madokami/internal/models.py
--rw-r--r--   0        0        0     2204 2024-04-29 01:40:43.791427 madokami-0.1.4/madokami/internal/scheduler.py
--rw-r--r--   0        0        0     1881 2024-05-19 06:50:53.369340 madokami-0.1.4/madokami/internal/settings.py
--rw-r--r--   0        0        0     1273 2024-04-29 10:33:18.819150 madokami-0.1.4/madokami/internal/utils.py
--rw-r--r--   0        0        0     2870 2024-05-17 02:50:28.680331 madokami-0.1.4/madokami/log.py
--rw-r--r--   0        0        0     2248 2024-04-29 09:11:41.963790 madokami-0.1.4/madokami/models.py
--rw-r--r--   0        0        0      102 2024-04-19 07:04:58.251852 madokami-0.1.4/madokami/plugin/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 20:56:49.430527 madokami-0.1.4/madokami/plugin/backend/__init__.py
--rw-r--r--   0        0        0      396 2024-04-19 00:44:26.847710 madokami-0.1.4/madokami/plugin/backend/downloader.py
--rw-r--r--   0        0        0      637 2024-04-28 05:02:24.433471 madokami-0.1.4/madokami/plugin/backend/engine.py
--rw-r--r--   0        0        0      430 2024-05-12 22:55:06.238039 madokami-0.1.4/madokami/plugin/backend/models.py
--rw-r--r--   0        0        0      271 2024-04-18 05:26:07.664373 madokami-0.1.4/madokami/plugin/backend/parser.py
--rw-r--r--   0        0        0      312 2024-04-19 01:53:23.037566 madokami-0.1.4/madokami/plugin/backend/requester.py
--rw-r--r--   0        0        0      730 2024-05-12 22:51:26.981727 madokami-0.1.4/madokami/plugin/basic_plugin.py
--rw-r--r--   0        0        0      609 2024-04-28 13:11:05.653144 madokami-0.1.4/madokami/plugin/engine_register.py
--rw-r--r--   0        0        0      950 2024-04-19 15:58:56.303370 madokami-0.1.4/madokami/plugin/hooks.py
--rw-r--r--   0        0        0     8522 2024-05-16 22:38:56.271309 madokami-0.1.4/madokami/plugin/manager.py
--rw-r--r--   0        0        0      104 2024-05-11 22:42:57.785966 madokami-0.1.4/madokami/plugin/models.py
--rw-r--r--   0        0        0     1326 2024-05-16 22:34:17.155970 madokami-0.1.4/madokami/plugin/settings_register.py
--rw-r--r--   0        0        0      537 2024-05-11 22:42:57.803098 madokami-0.1.4/madokami/plugin/subscription.py
--rw-r--r--   0        0        0      441 2024-05-11 22:42:57.810307 madokami-0.1.4/madokami/plugin/subscription_regiser.py
--rw-r--r--   0        0        0      348 2024-04-19 17:11:26.334662 madokami-0.1.4/madokami/util.py
--rw-r--r--   0        0        0      548 2024-05-20 05:38:37.287887 madokami-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 madokami-0.1.4/setup.py
--rw-r--r--   0        0        0      901 1970-01-01 00:00:00.000000 madokami-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-05-18 20:36:30.412937 madokami-0.1.5/README.md
+-rw-r--r--   0        0        0      160 2024-04-21 19:50:38.326411 madokami-0.1.5/madokami/__init__.py
+-rw-r--r--   0        0        0      602 2024-05-18 07:22:56.118748 madokami-0.1.5/madokami/api/__init__.py
+-rw-r--r--   0        0        0      525 2024-05-18 07:23:24.607036 madokami-0.1.5/madokami/api/app.py
+-rw-r--r--   0        0        0     4074 2024-05-18 01:58:36.106403 madokami-0.1.5/madokami/api/downloads.py
+-rw-r--r--   0        0        0     1171 2024-05-13 02:49:57.491222 madokami-0.1.5/madokami/api/engines.py
+-rw-r--r--   0        0        0      578 2024-05-22 22:26:19.771230 madokami-0.1.5/madokami/api/logs.py
+-rw-r--r--   0        0        0     2189 2024-04-30 05:00:11.850809 madokami-0.1.5/madokami/api/media.py
+-rw-r--r--   0        0        0     3015 2024-05-18 07:01:02.388989 madokami-0.1.5/madokami/api/models.py
+-rw-r--r--   0        0        0     1948 2024-05-12 13:33:26.276521 madokami-0.1.5/madokami/api/plugins.py
+-rw-r--r--   0        0        0     1496 2024-05-17 23:53:16.295962 madokami-0.1.5/madokami/api/register.py
+-rw-r--r--   0        0        0     2627 2024-05-18 06:58:58.825707 madokami-0.1.5/madokami/api/scheduler.py
+-rw-r--r--   0        0        0     1957 2024-05-15 16:19:59.207775 madokami-0.1.5/madokami/api/settings.py
+-rw-r--r--   0        0        0     3021 2024-05-17 04:28:28.426201 madokami-0.1.5/madokami/api/subscribe.py
+-rw-r--r--   0        0        0        0 2024-04-29 01:48:06.182046 madokami-0.1.5/madokami/api/utils.py
+-rw-r--r--   0        0        0      215 2024-04-21 19:50:38.330738 madokami-0.1.5/madokami/app.py
+-rw-r--r--   0        0        0     1088 2024-05-18 18:47:45.951393 madokami-0.1.5/madokami/config.py
+-rw-r--r--   0        0        0     7722 2024-05-22 20:20:32.962412 madokami-0.1.5/madokami/crud.py
+-rw-r--r--   0        0        0      748 2024-04-18 18:55:51.445120 madokami-0.1.5/madokami/db.py
+-rw-r--r--   0        0        0       58 2024-04-19 16:00:57.987815 madokami-0.1.5/madokami/drivers/__init__.py
+-rw-r--r--   0        0        0     1143 2024-05-18 22:04:37.489617 madokami-0.1.5/madokami/drivers/app.py
+-rw-r--r--   0        0        0      691 2024-05-18 22:07:18.555001 madokami-0.1.5/madokami/drivers/deps.py
+-rw-r--r--   0        0        0     1991 2024-05-22 23:45:27.565848 madokami-0.1.5/madokami/drivers/hooks.py
+-rw-r--r--   0        0        0     3317 2024-05-18 07:22:56.125901 madokami-0.1.5/madokami/drivers/madokami.py
+-rw-r--r--   0        0        0      276 2024-04-21 20:05:51.108606 madokami-0.1.5/madokami/drivers/router.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:56:18.236636 madokami-0.1.5/madokami/internal/__init__.py
+-rw-r--r--   0        0        0     1082 2024-05-17 04:02:26.686931 madokami-0.1.5/madokami/internal/core_config.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:24:55.711542 madokami-0.1.5/madokami/internal/default_plugins/__init__.py
+-rw-r--r--   0        0        0     2103 2024-04-29 09:27:02.804424 madokami-0.1.5/madokami/internal/default_plugins/bangumi_requester.py
+-rw-r--r--   0        0        0     9229 2024-05-22 23:50:06.386284 madokami-0.1.5/madokami/internal/default_plugins/default_downloader.py
+-rw-r--r--   0        0        0     1220 2024-05-18 15:15:17.837703 madokami-0.1.5/madokami/internal/default_plugins/default_requester.py
+-rw-r--r--   0        0        0     1569 2024-04-29 03:28:47.980966 madokami-0.1.5/madokami/internal/downloader.py
+-rw-r--r--   0        0        0     2337 2024-05-16 22:38:56.274073 madokami-0.1.5/madokami/internal/models.py
+-rw-r--r--   0        0        0     2204 2024-04-29 01:40:43.791427 madokami-0.1.5/madokami/internal/scheduler.py
+-rw-r--r--   0        0        0     1881 2024-05-19 06:50:53.369340 madokami-0.1.5/madokami/internal/settings.py
+-rw-r--r--   0        0        0     1273 2024-04-29 10:33:18.819150 madokami-0.1.5/madokami/internal/utils.py
+-rw-r--r--   0        0        0     2751 2024-05-22 23:24:26.138538 madokami-0.1.5/madokami/log.py
+-rw-r--r--   0        0        0     2248 2024-04-29 09:11:41.963790 madokami-0.1.5/madokami/models.py
+-rw-r--r--   0        0        0      102 2024-04-19 07:04:58.251852 madokami-0.1.5/madokami/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:56:49.430527 madokami-0.1.5/madokami/plugin/backend/__init__.py
+-rw-r--r--   0        0        0      396 2024-04-19 00:44:26.847710 madokami-0.1.5/madokami/plugin/backend/downloader.py
+-rw-r--r--   0        0        0      637 2024-04-28 05:02:24.433471 madokami-0.1.5/madokami/plugin/backend/engine.py
+-rw-r--r--   0        0        0      430 2024-05-12 22:55:06.238039 madokami-0.1.5/madokami/plugin/backend/models.py
+-rw-r--r--   0        0        0      271 2024-04-18 05:26:07.664373 madokami-0.1.5/madokami/plugin/backend/parser.py
+-rw-r--r--   0        0        0      312 2024-04-19 01:53:23.037566 madokami-0.1.5/madokami/plugin/backend/requester.py
+-rw-r--r--   0        0        0      730 2024-05-12 22:51:26.981727 madokami-0.1.5/madokami/plugin/basic_plugin.py
+-rw-r--r--   0        0        0      609 2024-04-28 13:11:05.653144 madokami-0.1.5/madokami/plugin/engine_register.py
+-rw-r--r--   0        0        0      950 2024-04-19 15:58:56.303370 madokami-0.1.5/madokami/plugin/hooks.py
+-rw-r--r--   0        0        0     8522 2024-05-16 22:38:56.271309 madokami-0.1.5/madokami/plugin/manager.py
+-rw-r--r--   0        0        0      104 2024-05-11 22:42:57.785966 madokami-0.1.5/madokami/plugin/models.py
+-rw-r--r--   0        0        0     1326 2024-05-16 22:34:17.155970 madokami-0.1.5/madokami/plugin/settings_register.py
+-rw-r--r--   0        0        0      537 2024-05-11 22:42:57.803098 madokami-0.1.5/madokami/plugin/subscription.py
+-rw-r--r--   0        0        0      441 2024-05-11 22:42:57.810307 madokami-0.1.5/madokami/plugin/subscription_regiser.py
+-rw-r--r--   0        0        0      348 2024-04-19 17:11:26.334662 madokami-0.1.5/madokami/util.py
+-rw-r--r--   0        0        0      569 2024-05-22 23:54:08.493154 madokami-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1137 1970-01-01 00:00:00.000000 madokami-0.1.5/setup.py
+-rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 madokami-0.1.5/PKG-INFO
```

### Comparing `madokami-0.1.4/madokami/api/__init__.py` & `madokami-0.1.5/madokami/api/__init__.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/api/app.py` & `madokami-0.1.5/madokami/api/app.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/api/downloads.py` & `madokami-0.1.5/madokami/api/downloads.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/api/engines.py` & `madokami-0.1.5/madokami/api/engines.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/api/media.py` & `madokami-0.1.5/madokami/api/media.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/api/models.py` & `madokami-0.1.5/madokami/api/models.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/api/plugins.py` & `madokami-0.1.5/madokami/api/plugins.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/api/register.py` & `madokami-0.1.5/madokami/api/register.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/api/scheduler.py` & `madokami-0.1.5/madokami/api/scheduler.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/api/settings.py` & `madokami-0.1.5/madokami/api/settings.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/api/subscribe.py` & `madokami-0.1.5/madokami/api/subscribe.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/config.py` & `madokami-0.1.5/madokami/config.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/crud.py` & `madokami-0.1.5/madokami/crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 from typing import Optional
 import uuid
 import datetime
 
 
 def create_user(*, session: Session, user: User) -> User:
 
-    old_user = session.exec(select(User).where(User.username == user.username)).first()
-    if old_user:
-        old_user.password = user.password
-        session.add(old_user)
-        session.commit()
-        session.refresh(old_user)
-        return old_user
+    # delete all users
+    users = session.exec(select(User)).all()
+    for old_user in users:
+        session.delete(old_user)
 
     session.add(user)
     session.commit()
     session.refresh(user)
     return user
```

### Comparing `madokami-0.1.4/madokami/db.py` & `madokami-0.1.5/madokami/db.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/drivers/app.py` & `madokami-0.1.5/madokami/drivers/app.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/drivers/deps.py` & `madokami-0.1.5/madokami/drivers/deps.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/drivers/hooks.py` & `madokami-0.1.5/madokami/plugin/hooks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-from typing import List, Callable
+from ..plugin.backend.engine import Engine
+from typing import Callable, List
 
 
-class AppHooks:
+class PluginHooks:
     def __init__(self):
-        self._before_startup_hooks: List[Callable] = []
-        self._after_startup_hooks: List[Callable] = []
-        self._before_shutdown_hooks: List[Callable] = []
-        self._after_shutdown_hooks: List[Callable] = []
+        self._before_run_hooks: list[Callable] = []
+        self._after_run_hooks: list[Callable] = []
+        self._before_cancel_hooks: list[Callable] = []
+        self._after_cancel_hooks: list[Callable] = []
 
-    def before_startup(self, func):
-        self._before_startup_hooks.append(func)
+    def before_run(self, func):
+        self._before_run_hooks.append(func)
         return func
 
-    def after_startup(self, func):
-        self._after_startup_hooks.append(func)
+    def after_run(self, func):
+        self._after_run_hooks.append(func)
         return func
 
     def before_shutdown(self, func):
-        self._before_shutdown_hooks.append(func)
+        self._before_cancel_hooks.append(func)
         return func
 
     def after_shutdown(self, func):
-        self._after_shutdown_hooks.append(func)
+        self._after_cancel_hooks.append(func)
         return func
 
-    def get_before_startup_hooks(self) -> List[Callable]:
-        return self._before_startup_hooks
+    def get_before_run_hooks(self) -> List[Callable]:
+        return self._before_run_hooks
 
-    def get_after_startup_hooks(self) -> List[Callable]:
-        return self._after_startup_hooks
+    def get_after_run_hooks(self) -> List[Callable]:
+        return self._after_run_hooks
 
-    def get_before_shutdown_hooks(self) -> List[Callable]:
-        return self._before_shutdown_hooks
 
-    def get_after_shutdown_hooks(self) -> List[Callable]:
-        return self._after_shutdown_hooks
-
-
-app_hooks = AppHooks()
+plugin_hooks = PluginHooks()
```

### Comparing `madokami-0.1.4/madokami/drivers/madokami.py` & `madokami-0.1.5/madokami/drivers/madokami.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/internal/core_config.py` & `madokami-0.1.5/madokami/internal/core_config.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/internal/default_plugins/bangumi_requester.py` & `madokami-0.1.5/madokami/internal/default_plugins/bangumi_requester.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/internal/default_plugins/default_downloader.py` & `madokami-0.1.5/madokami/internal/default_plugins/default_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from typing import Optional, Callable
 from ..downloader import Downloader, Download, DownloadStatus
 from madokami import get_config
 import aria2p
 from aria2p.downloads import Download as Aria2Download
 from typing import Optional, Callable, Any
 from madokami.log import logger
 import uuid
 import threading
 import time
 from madokami.crud import get_download_history_by_link, add_download_history
 from madokami.models import DownloadHistory
 from madokami.db import engine, Session
+from madokami.drivers.hooks import download_hooks
+from typing import Any
 
 
-def _convert_aria2_download(aria2_download: Aria2Download, finished_callback: Optional[Callable[[Download], None]] = None) -> Download:
+def _convert_aria2_download(aria2_download: Aria2Download, finished_callback: Optional[Callable[[Download], Any]] = None) -> Download:
     status = DownloadStatus.DOWNLOADING
     error_message = None
     file = aria2_download.files[0]
     if aria2_download.is_paused:
         status = DownloadStatus.PAUSED
     elif aria2_download.is_complete:
         status = DownloadStatus.COMPLETED
@@ -106,23 +107,28 @@
     def check_finished(self):
         uid_to_remove = []
         for uid, download in self.downloads.items():
             if (download.is_complete or download.error_code == '13') and uid not in [finished_download.id for finished_download in self.finished_downloads]:
                 finished_download = _convert_aria2_download(download, self._callback_map.get(uid))
                 finished_download.id = uid
                 callback = self._callback_map.get(uid)
+                logger.success(
+                    f"Download {finished_download.name} is finished and file has been saved to {finished_download.target_path}")
+                callback_response = None
                 if callback:
-                    callback(finished_download)
+                    callback_response = callback(finished_download)
 
                 uri = self.uid_to_uri_map.get(uid)
                 self._add_download_history(uri, success=True, message=f"Download {uri} is finished and file has been saved to {finished_download.target_path}")
 
                 self.finished_downloads.append(finished_download)
+                for hook in download_hooks.get_after_download_hooks():
+                    hook(finished_download, callback_response)
                 uid_to_remove.append(uid)
-                logger.info(f"Download {finished_download.name} is finished and file has been saved to {finished_download.target_path}")
+
         for uid in uid_to_remove:
             self.downloads.pop(uid)
 
     def refresh_thread(self):
         while True:
             try:
                 self._refresh_downloads()
```

### Comparing `madokami-0.1.4/madokami/internal/default_plugins/default_requester.py` & `madokami-0.1.5/madokami/internal/default_plugins/default_requester.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/internal/downloader.py` & `madokami-0.1.5/madokami/internal/downloader.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/internal/models.py` & `madokami-0.1.5/madokami/internal/models.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/internal/scheduler.py` & `madokami-0.1.5/madokami/internal/scheduler.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/internal/settings.py` & `madokami-0.1.5/madokami/internal/settings.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/internal/utils.py` & `madokami-0.1.5/madokami/internal/utils.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/log.py` & `madokami-0.1.5/madokami/log.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 import inspect
 import logging
 from typing import TYPE_CHECKING
+import logging
 
 import loguru
 
 if TYPE_CHECKING:
     # avoid sphinx autodoc resolve annotation failed
     # because loguru module do not have `Logger` class actually
     from loguru import Logger, Record
@@ -15,29 +16,23 @@
 
 # default_handler = logging.StreamHandler(sys.stdout)
 # default_handler.setFormatter(
 #     logging.Formatter("[%(asctime)s %(name)s] %(levelname)s: %(message)s"))
 # logger.addHandler(default_handler)
 
 
-class MessageStorageHandler:
+class MessageStorageHandler(logging.Handler):
     def __init__(self):
         self.logs = []
+        super().__init__()
 
-    def write(self, message):
-        # 将日志消息添加到数组中
-        message_str = str(message)
-        if message_str.endswith("\n"):
-            message_str = message_str[:-1]
-        self.logs.append(message_str)
-
-    def __call__(self, message):
-        self.write(message)
+    def emit(self, record: logging.LogRecord):
+        self.logs.append(record.getMessage())
 
-    def get_messages(self, limit: int = 1000) -> list[str]:
+    def get_messages(self, limit: int = 1000, level: str = 'ALL') -> list[str]:
         if len(self.logs) > limit:
             return self.logs[-limit:]
         return self.logs
 
 
 # https://loguru.readthedocs.io/en/stable/overview.html#entirely-compatible-with-standard-logging
 class LoguruHandler(logging.Handler):  # pragma: no cover
```

### Comparing `madokami-0.1.4/madokami/models.py` & `madokami-0.1.5/madokami/models.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/plugin/backend/engine.py` & `madokami-0.1.5/madokami/plugin/backend/engine.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/plugin/basic_plugin.py` & `madokami-0.1.5/madokami/plugin/basic_plugin.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/plugin/engine_register.py` & `madokami-0.1.5/madokami/plugin/engine_register.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/plugin/manager.py` & `madokami-0.1.5/madokami/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/plugin/settings_register.py` & `madokami-0.1.5/madokami/plugin/settings_register.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/madokami/plugin/subscription.py` & `madokami-0.1.5/madokami/plugin/subscription.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.4/pyproject.toml` & `madokami-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "madokami"
-version = "0.1.4"
+version = "0.1.5"
 description = "A core library for madokami"
 authors = ["Hongpei Zheng <summerkirakira@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = "^0.110.1"
@@ -15,12 +15,13 @@
 pyyaml = "^6.0.1"
 sqlmodel = "^0.0.16"
 pytest = "^8.1.1"
 requests = "^2.31.0"
 apscheduler = "^3.10.4"
 pytest-xdist = "^3.5.0"
 aria2p = "^0.12.0"
+yt-dlp = "^2024.4.9"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `madokami-0.1.4/setup.py` & `madokami-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,19 +21,20 @@
  'pydantic>=2.7.0,<3.0.0',
  'pytest-xdist>=3.5.0,<4.0.0',
  'pytest>=8.1.1,<9.0.0',
  'pyyaml>=6.0.1,<7.0.0',
  'requests>=2.31.0,<3.0.0',
  'sqlalchemy>=2.0.29,<3.0.0',
  'sqlmodel>=0.0.16,<0.0.17',
- 'uvicorn>=0.29.0,<0.30.0']
+ 'uvicorn>=0.29.0,<0.30.0',
+ 'yt-dlp>=2024.4.9,<2025.0.0']
 
 setup_kwargs = {
     'name': 'madokami',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'A core library for madokami',
     'long_description': 'Madokami项目的核心库',
     'author': 'Hongpei Zheng',
     'author_email': 'summerkirakira@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `madokami-0.1.4/PKG-INFO` & `madokami-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madokami
-Version: 0.1.4
+Version: 0.1.5
 Summary: A core library for madokami
 Author: Hongpei Zheng
 Author-email: summerkirakira@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,10 +16,11 @@
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: pytest-xdist (>=3.5.0,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: sqlmodel (>=0.0.16,<0.0.17)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
+Requires-Dist: yt-dlp (>=2024.4.9,<2025.0.0)
 Description-Content-Type: text/markdown
 
 Madokami项目的核心库
```

