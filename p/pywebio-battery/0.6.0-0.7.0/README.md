# Comparing `tmp/pywebio_battery-0.6.0.tar.gz` & `tmp/pywebio_battery-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywebio_battery-0.6.0.tar", last modified: Sat Apr 20 15:26:03 2024, max compression
+gzip compressed data, was "pywebio_battery-0.7.0.tar", last modified: Thu May 23 03:08:11 2024, max compression
```

## Comparing `pywebio_battery-0.6.0.tar` & `pywebio_battery-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:26:03.327672 pywebio_battery-0.6.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-20 15:26:03.327672 pywebio_battery-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:26:03.327672 pywebio_battery-0.6.0/pywebio_battery/
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/pywebio_battery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/pywebio_battery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/pywebio_battery/file_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14717 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/pywebio_battery/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/pywebio_battery/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:26:03.327672 pywebio_battery-0.6.0/pywebio_battery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-20 15:26:03.000000 pywebio_battery-0.6.0/pywebio_battery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-20 15:26:03.000000 pywebio_battery-0.6.0/pywebio_battery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 15:26:03.000000 pywebio_battery-0.6.0/pywebio_battery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 15:26:03.000000 pywebio_battery-0.6.0/pywebio_battery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 15:26:03.000000 pywebio_battery-0.6.0/pywebio_battery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 15:26:03.327672 pywebio_battery-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-20 15:25:57.000000 pywebio_battery-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:11.418110 pywebio_battery-0.7.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-05-23 03:08:04.000000 pywebio_battery-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-23 03:08:11.418110 pywebio_battery-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-23 03:08:04.000000 pywebio_battery-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:11.414110 pywebio_battery-0.7.0/pywebio_battery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-23 03:08:04.000000 pywebio_battery-0.7.0/pywebio_battery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 03:08:04.000000 pywebio_battery-0.7.0/pywebio_battery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-23 03:08:04.000000 pywebio_battery-0.7.0/pywebio_battery/file_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14819 2024-05-23 03:08:04.000000 pywebio_battery-0.7.0/pywebio_battery/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-05-23 03:08:04.000000 pywebio_battery-0.7.0/pywebio_battery/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:08:11.418110 pywebio_battery-0.7.0/pywebio_battery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-23 03:08:11.000000 pywebio_battery-0.7.0/pywebio_battery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-23 03:08:11.000000 pywebio_battery-0.7.0/pywebio_battery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:08:11.000000 pywebio_battery-0.7.0/pywebio_battery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 03:08:11.000000 pywebio_battery-0.7.0/pywebio_battery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 03:08:11.000000 pywebio_battery-0.7.0/pywebio_battery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 03:08:11.418110 pywebio_battery-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 03:08:04.000000 pywebio_battery-0.7.0/setup.py
```

### Comparing `pywebio_battery-0.6.0/LICENSE` & `pywebio_battery-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywebio_battery-0.6.0/PKG-INFO` & `pywebio_battery-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebio_battery
-Version: 0.6.0
+Version: 0.7.0
 Summary: Utilities that help write PyWebIO apps quickly and easily.
 Home-page: https://pywebio.readthedocs.io/en/latest/battery.html
 Author: WeiminWang
 Author-email: wang0.618@qq.com
 License: MIT
 Project-URL: Documentation, https://pywebio.readthedocs.io/en/latest/battery.html
 Project-URL: Source, https://github.com/wang0618/pywebio-battery
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pywebio_battery Version: 0.6.0 Summary: Utilities
+Metadata-Version: 2.1 Name: pywebio_battery Version: 0.7.0 Summary: Utilities
 that help write PyWebIO apps quickly and easily. Home-page: https://
 pywebio.readthedocs.io/en/latest/battery.html Author: WeiminWang Author-email:
 wang0.618@qq.com License: MIT Project-URL: Documentation, https://
 pywebio.readthedocs.io/en/latest/battery.html Project-URL: Source, https://
 github.com/wang0618/pywebio-battery Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

### Comparing `pywebio_battery-0.6.0/README.md` & `pywebio_battery-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pywebio_battery-0.6.0/pywebio_battery/__init__.py` & `pywebio_battery-0.7.0/pywebio_battery/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,17 @@
      - Logbox widget
 
    * - `put_video <pywebio_battery.put_video>`
      - Output video
 
    * - `put_audio <pywebio_battery.put_audio>`
      - Output audio
-
+   
+   * - `wait_scroll_to_bottom <pywebio_battery.wait_scroll_to_bottom>`
+     - Wait the page is scrolled to bottom
 
 Web application related
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. list-table::
 
    * - Function name
```

### Comparing `pywebio_battery-0.6.0/pywebio_battery/file_picker.py` & `pywebio_battery-0.7.0/pywebio_battery/file_picker.py`

 * *Files identical despite different names*

### Comparing `pywebio_battery-0.6.0/pywebio_battery/interaction.py` & `pywebio_battery-0.7.0/pywebio_battery/interaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,19 +196,21 @@
 def put_logbox(name: str, height=400, keep_bottom=True) -> Output:
     r"""Output a logbox widget
 
     .. exportable-codeblock::
         :name: battery-put-logbox
         :summary: Logbox widget
 
-        from pywebio_battery import put_logbox, logbox_append   # ..demo-only
+        from pywebio.output import put_button
+        from pywebio_battery import put_logbox, logbox_append, logbox_clear   # ..demo-only
         # ..demo-only
         import time
 
         put_logbox("log")
+        put_button('Clear', lambda: logbox_clear("log"))
         while True:
             logbox_append("log", f"{time.time()}\n")
             time.sleep(0.2)
 
     :param str name: the name of the widget, must unique in session-wide.
     :param int height: the height of the widget in pixel
     :param bool keep_bottom: Whether to scroll to bottom when new content is appended
@@ -238,15 +240,15 @@
 def logbox_append(name: str, text: str):
     """Append text to a logbox widget"""
     run_js('$("#webio-logbox-%s").append(document.createTextNode(text))' % name, text=str(text))
 
 
 def logbox_clear(name: str):
     """Clear all contents of a logbox widget"""
-    pywebio.session.run_js('$("#webio-logbox-%s").empty()' % name)
+    run_js('$("#webio-logbox-%s").empty()' % name)
 
 
 def put_video(src: Union[str, bytes], autoplay: bool = False, loop: bool = False,
               height: int = None, width: int = None, muted: bool = False, poster: str = None,
               scope: str = None, position: int = OutputPosition.BOTTOM) -> Output:
     """Output video
 
@@ -330,15 +332,15 @@
     tags = ' '.join(t for t in tag_fields if kwargs[t])
 
     tag = r'<audio src="{src}" {tags} controls preload="metadata"><audio/>'.format(src=src, tags=tags)
     return put_html(tag, scope=scope, position=position)
 
 
 def wait_scroll_to_bottom(threshold: float = 10, timeout: float = None) -> bool:
-    """Wait until the page is scrolled to bottom.
+    r"""Wait until the page is scrolled to bottom.
 
     This function is useful to achieve infinite scrolling.
 
     :param float threshold: If the distance (in pixels) of the browser's viewport from the bottom of the page is less
         than the threshold, it is considered to reach the bottom
     :param float timeout: Timeout in seconds. The maximum time to wait for the page to scroll to bottom.
         Default is None, which means no timeout.
```

### Comparing `pywebio_battery-0.6.0/pywebio_battery/web.py` & `pywebio_battery-0.7.0/pywebio_battery/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pywebio.input import *
 from pywebio.output import *
 from pywebio.session import *
 from pywebio.session import get_current_session
 from tornado.web import create_signed_value, decode_signed_value
 from typing import *
 
-__all__ = ['get_all_query', 'get_query', 'set_localstorage', 'get_localstorage', 'set_cookie', 'get_cookie',
+__all__ = ['get_all_query', 'get_query', 'set_localstorage', 'get_localstorage', 'clear_localstorage', 'set_cookie', 'get_cookie',
            'basic_auth', 'custom_auth', 'revoke_auth']
 
 
 def get_all_query():
     """Get URL parameter (also known as "query strings" or "URL query parameters") as a dict"""
     query = eval_js("Object.fromEntries(new URLSearchParams(window.location.search))")
     return query
@@ -36,14 +36,19 @@
 
 
 def get_localstorage(key: str) -> str:
     """Get the key's value in user's web browser local storage"""
     return eval_js("localStorage.getItem(key)", key=key)
 
 
+def clear_localstorage():
+    """Clear user's web browser local storage"""
+    return eval_js("localStorage.clear()")
+
+
 def _init_cookie_client():
     session = get_current_session()
     if 'cookie_client_flag' not in session.internal_save:
         session.internal_save['cookie_client_flag'] = True
         # Credit: https://stackoverflow.com/questions/14573223/set-cookie-and-get-cookie-with-javascript
         run_js("""
         window.setCookie = function(name,value,days) {
```

### Comparing `pywebio_battery-0.6.0/pywebio_battery.egg-info/PKG-INFO` & `pywebio_battery-0.7.0/pywebio_battery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebio-battery
-Version: 0.6.0
+Version: 0.7.0
 Summary: Utilities that help write PyWebIO apps quickly and easily.
 Home-page: https://pywebio.readthedocs.io/en/latest/battery.html
 Author: WeiminWang
 Author-email: wang0.618@qq.com
 License: MIT
 Project-URL: Documentation, https://pywebio.readthedocs.io/en/latest/battery.html
 Project-URL: Source, https://github.com/wang0618/pywebio-battery
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pywebio-battery Version: 0.6.0 Summary: Utilities
+Metadata-Version: 2.1 Name: pywebio-battery Version: 0.7.0 Summary: Utilities
 that help write PyWebIO apps quickly and easily. Home-page: https://
 pywebio.readthedocs.io/en/latest/battery.html Author: WeiminWang Author-email:
 wang0.618@qq.com License: MIT Project-URL: Documentation, https://
 pywebio.readthedocs.io/en/latest/battery.html Project-URL: Source, https://
 github.com/wang0618/pywebio-battery Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

### Comparing `pywebio_battery-0.6.0/setup.py` & `pywebio_battery-0.7.0/setup.py`

 * *Files identical despite different names*

