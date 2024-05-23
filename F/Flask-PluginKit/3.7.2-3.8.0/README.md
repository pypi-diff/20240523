# Comparing `tmp/Flask-PluginKit-3.7.2.tar.gz` & `tmp/flask_pluginkit-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-PluginKit-3.7.2.tar", last modified: Wed May 17 03:26:26 2023, max compression
+gzip compressed data, was "flask_pluginkit-3.8.0.tar", last modified: Thu May 23 13:07:57 2024, max compression
```

## Comparing `Flask-PluginKit-3.7.2.tar` & `flask_pluginkit-3.8.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:26.404666 Flask-PluginKit-3.7.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:26.394666 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3470 2023-05-17 03:26:26.000000 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      614 2023-05-17 03:26:26.000000 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:26:26.000000 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 02:59:12.000000 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-17 03:26:26.000000 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-17 03:26:26.000000 Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1507 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       88 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3470 2023-05-17 03:26:26.404666 Flask-PluginKit-3.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2004 2023-05-15 03:29:18.000000 Flask-PluginKit-3.7.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:26.394666 Flask-PluginKit-3.7.2/flask_pluginkit/
--rw-r--r--   0 root         (0) root         (0)      653 2023-05-17 02:45:19.000000 Flask-PluginKit-3.7.2/flask_pluginkit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1056 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/flask_pluginkit/_compat.py
--rw-r--r--   0 root         (0) root         (0)    10767 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/flask_pluginkit/_installer.py
--rw-r--r--   0 root         (0) root         (0)    10148 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/flask_pluginkit/_web.py
--rw-r--r--   0 root         (0) root         (0)      558 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/flask_pluginkit/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    48626 2023-05-17 02:46:28.000000 Flask-PluginKit-3.7.2/flask_pluginkit/pluginkit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:26.404666 Flask-PluginKit-3.7.2/flask_pluginkit/static/
--rw-r--r--   0 root         (0) root         (0)      820 2023-05-15 03:29:18.000000 Flask-PluginKit-3.7.2/flask_pluginkit/static/translations.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:26.404666 Flask-PluginKit-3.7.2/flask_pluginkit/templates/
--rw-r--r--   0 root         (0) root         (0)    14880 2023-05-15 03:29:18.000000 Flask-PluginKit-3.7.2/flask_pluginkit/templates/manager.html
--rw-r--r--   0 root         (0) root         (0)    12095 2023-05-15 03:29:18.000000 Flask-PluginKit-3.7.2/flask_pluginkit/utils.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-17 03:26:26.404666 Flask-PluginKit-3.7.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4196 2023-05-17 02:57:23.000000 Flask-PluginKit-3.7.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:26:26.404666 Flask-PluginKit-3.7.2/tests/
--rw-r--r--   0 root         (0) root         (0)     2490 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/tests/test_installer.py
--rw-r--r--   0 root         (0) root         (0)     8485 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/tests/test_pm.py
--rw-r--r--   0 root         (0) root         (0)     5584 2021-09-06 01:47:42.000000 Flask-PluginKit-3.7.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:57.270044 flask_pluginkit-3.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:57.270044 flask_pluginkit-3.8.0/Flask_PluginKit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-23 13:07:57.000000 flask_pluginkit-3.8.0/Flask_PluginKit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-23 13:07:57.000000 flask_pluginkit-3.8.0/Flask_PluginKit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:07:57.000000 flask_pluginkit-3.8.0/Flask_PluginKit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:07:32.000000 flask_pluginkit-3.8.0/Flask_PluginKit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 13:07:57.000000 flask_pluginkit-3.8.0/Flask_PluginKit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 13:07:57.000000 flask_pluginkit-3.8.0/Flask_PluginKit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-23 13:07:57.270044 flask_pluginkit-3.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:57.270044 flask_pluginkit-3.8.0/flask_pluginkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/flask_pluginkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/flask_pluginkit/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/flask_pluginkit/_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9957 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/flask_pluginkit/_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/flask_pluginkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46619 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/flask_pluginkit/pluginkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:57.270044 flask_pluginkit-3.8.0/flask_pluginkit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/flask_pluginkit/static/translations.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:57.270044 flask_pluginkit-3.8.0/flask_pluginkit/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/flask_pluginkit/templates/manager.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11035 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/flask_pluginkit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:07:57.270044 flask_pluginkit-3.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:57.270044 flask_pluginkit-3.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/tests/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/tests/test_pm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-23 13:07:23.000000 flask_pluginkit-3.8.0/tests/test_utils.py
```

### Comparing `Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/PKG-INFO` & `flask_pluginkit-3.8.0/Flask_PluginKit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: Flask-PluginKit
-Version: 3.7.2
+Version: 3.8.0
 Summary: Load and run plugins for your Flask application
 Home-page: https://github.com/staugur/Flask-PluginKit
-Download-URL: https://github.com/staugur/Flask-PluginKit/releases/tag/v3.7.2
+Download-URL: https://github.com/staugur/Flask-PluginKit/releases/tag/v3.8.0
 Author: Hiroshi.tao
 Author-email: me@tcw.im
 License: BSD 3-Clause
 Project-URL: Code, https://github.com/staugur/Flask-PluginKit
 Project-URL: Issue tracker, https://github.com/staugur/Flask-PluginKit/issues
 Project-URL: Documentation, https://flask-pluginkit.rtfd.vip
 Keywords: flask plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Flask
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.3.*,!=3.5.*
+Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: Flask>=3.0.0
+Requires-Dist: semver>=3.0.0
+Provides-Extra: redis
+Requires-Dist: redis>=5.0.0; extra == "redis"
 
 Flask-PluginKit
 ===============
 
 Web program plugin development kit based on Flask.
 
 |Build Status| |Documentation Status| |codecov| |PyPI|
```

### Comparing `Flask-PluginKit-3.7.2/Flask_PluginKit.egg-info/SOURCES.txt` & `flask_pluginkit-3.8.0/Flask_PluginKit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.rst
-setup.cfg
 setup.py
 Flask_PluginKit.egg-info/PKG-INFO
 Flask_PluginKit.egg-info/SOURCES.txt
 Flask_PluginKit.egg-info/dependency_links.txt
 Flask_PluginKit.egg-info/not-zip-safe
 Flask_PluginKit.egg-info/requires.txt
 Flask_PluginKit.egg-info/top_level.txt
```

### Comparing `Flask-PluginKit-3.7.2/LICENSE` & `flask_pluginkit-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.2/PKG-INFO` & `flask_pluginkit-3.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: Flask-PluginKit
-Version: 3.7.2
+Version: 3.8.0
 Summary: Load and run plugins for your Flask application
 Home-page: https://github.com/staugur/Flask-PluginKit
-Download-URL: https://github.com/staugur/Flask-PluginKit/releases/tag/v3.7.2
+Download-URL: https://github.com/staugur/Flask-PluginKit/releases/tag/v3.8.0
 Author: Hiroshi.tao
 Author-email: me@tcw.im
 License: BSD 3-Clause
 Project-URL: Code, https://github.com/staugur/Flask-PluginKit
 Project-URL: Issue tracker, https://github.com/staugur/Flask-PluginKit/issues
 Project-URL: Documentation, https://flask-pluginkit.rtfd.vip
 Keywords: flask plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Flask
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.3.*,!=3.5.*
+Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: Flask>=3.0.0
+Requires-Dist: semver>=3.0.0
+Provides-Extra: redis
+Requires-Dist: redis>=5.0.0; extra == "redis"
 
 Flask-PluginKit
 ===============
 
 Web program plugin development kit based on Flask.
 
 |Build Status| |Documentation Status| |codecov| |PyPI|
```

### Comparing `Flask-PluginKit-3.7.2/README.rst` & `flask_pluginkit-3.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.2/flask_pluginkit/__init__.py` & `flask_pluginkit-3.8.0/flask_pluginkit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,26 @@
 
     :copyright: (c) 2019 by staugur.
     :license: BSD 3-Clause, see LICENSE for more details.
 """
 
 from .pluginkit import PluginManager, push_dcp
 from .utils import (
-    Flask,
     LocalStorage,
     RedisStorage,
     JsonResponse,
 )
 from ._installer import PluginInstaller
 from ._web import blueprint
 
 __author__ = "Hiroshi.tao <me@tcw.im>"
 
-__version__ = "3.7.2"
+__version__ = "3.8.0"
 
 __all__ = [
-    "Flask",
     "PluginManager",
     "LocalStorage",
     "RedisStorage",
     "JsonResponse",
     "PluginInstaller",
     "push_dcp",
     "blueprint",
```

### Comparing `Flask-PluginKit-3.7.2/flask_pluginkit/_installer.py` & `flask_pluginkit-3.8.0/flask_pluginkit/_installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from os.path import join, abspath, isdir, isfile, basename
 from sys import executable
 from subprocess import call
 from cgi import parse_header
 from posixpath import basename as posixbasename
 from tempfile import NamedTemporaryFile
 from .exceptions import PluginError, TarError, ZipError, InstallError
-from ._compat import PY2, string_types, urllib2, urlsplit, parse_qs
+from ._compat import string_types, urllib2, urlsplit, parse_qs
 from .utils import check_url
 
 
 class PluginInstaller(object):
     """plugin installer for installing a compressed local/remote plugin"""
 
     def __init__(self, plugin_abspath, **kwargs):
@@ -63,35 +63,26 @@
         scene value see `remote_download` in 1, 2, 3, 4
         """
         filename = None
         try:
             if scene == 1:
                 plugin_filename = [
                     i
-                    for i in parse_qs(urlsplit(data).query).get(
-                        "plugin_filename"
-                    )
-                    or []
+                    for i in parse_qs(urlsplit(data).query).get("plugin_filename") or []
                     if i
                 ]
                 if plugin_filename and len(plugin_filename) == 1:
                     filename = plugin_filename[0]
             elif scene == 2:
                 filename = posixbasename(urlsplit(data).path)
             elif scene == 3:
-                if PY2:
-                    cd = data.headers.getheader("Content-Disposition", "")
-                else:
-                    cd = data.getheader("Content-Disposition", "")
+                cd = data.getheader("Content-Disposition", "")
                 filename = parse_header(cd)[-1].get("filename")
             elif scene == 4:
-                if PY2:
-                    cd = data.info().subtype
-                else:
-                    cd = data.info().get_content_subtype()
+                cd = data.info().get_content_subtype()
                 mt = {
                     "zip": "zip",
                     "x-compressed-tar": "tar.gz",
                     "x-gzip": "tar.gz",
                 }
                 subtype = mt.get(cd)
                 if subtype:
@@ -251,17 +242,15 @@
             Add pip method, with package_or_url param.
         """
         res = dict(code=1, msg=None)
         try:
             if method == "remote":
                 self._remote_download(kwargs["url"])
             elif method == "local":
-                self._local_upload(
-                    kwargs["filepath"], kwargs.get("remove", False)
-                )
+                self._local_upload(kwargs["filepath"], kwargs.get("remove", False))
             elif method == "pip":  # pragma: nocover
                 res = self._pip_install(kwargs["package_or_url"])
             else:
                 res.update(msg="Invalid method")
         except Exception as e:
             res.update(msg=str(e))
         else:
```

### Comparing `Flask-PluginKit-3.7.2/flask_pluginkit/_web.py` & `flask_pluginkit-3.8.0/flask_pluginkit/_web.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,35 +5,32 @@
 
     The server-side plugin management blueprint.
 
     :copyright: (c) 2019 by staugur.
     :license: BSD 3-Clause, see LICENSE for more details.
 """
 
+import _thread as thread
 from time import sleep
 from collections import OrderedDict, deque
 from werkzeug.utils import secure_filename
 from tempfile import NamedTemporaryFile
 from flask import (
     Blueprint,
     current_app,
     g,
     request,
     jsonify,
     render_template,
     make_response,
     Response,
 )
-from .utils import PY2, allowed_uploaded_plugin_suffix, check_url
+from .utils import allowed_uploaded_plugin_suffix, check_url
 from ._installer import PluginInstaller
 
-if PY2:
-    import thread
-else:
-    import _thread as thread
 
 #: Blueprint instance for managing plugins
 #:
 #: ..versionadded:: 3.3.0
 blueprint = Blueprint(
     "flask_pluginkit",
     "flask_pluginkit",
@@ -72,16 +69,15 @@
             authResult.update(code=0)
 
     elif authMethod == "BASIC":
         #: the realm parameter is reserved for defining protection spaces and
         #: it's used by the authentication schemes to indicate a scope of
         #: protection.
         AUTHREALM = (
-            _get_conf("PLUGINKIT_AUTH_REALM")
-            or "Flask-PluginKit Login Required"
+            _get_conf("PLUGINKIT_AUTH_REALM") or "Flask-PluginKit Login Required"
         )
 
         #: User and password configuration, format {user:pass, user:pass},
         #: if format error, all authentication failure by default.
         AUTHUSERS = _get_conf("PLUGINKIT_AUTH_USERS")
 
         def verify_auth(username, password):
@@ -126,18 +122,15 @@
         WHITELIST = _get_conf("PLUGINKIT_AUTH_IP_WHITELIST") or []
         if isinstance(BLACKLIST, (list, tuple)) and isinstance(
             WHITELIST, (list, tuple)
         ):
             if ip in WHITELIST and ip not in BLACKLIST:
                 authResult.update(code=0)
 
-    if (
-        hasattr(current_app, "extensions")
-        and "pluginkit" in current_app.extensions
-    ):
+    if hasattr(current_app, "extensions") and "pluginkit" in current_app.extensions:
         from flask_pluginkit import __version__ as version
 
         g.pluginkit = current_app.extensions["pluginkit"]
         metadata = OrderedDict()
         metadata["version"] = version
         metadata["plugins_count"] = len(g.pluginkit.get_all_plugins)
         g.pluginkit_metadata = metadata
@@ -192,17 +185,15 @@
                     PLUGINKIT_UWSGI_ENABLED=True
             """
             try:
                 import os
                 import signal
                 import psutil
             except ImportError:
-                res.update(
-                    code=20000, msg="No dependent modules(psutil) installed"
-                )
+                res.update(code=20000, msg="No dependent modules(psutil) installed")
             else:
                 ENV = _get_conf("ENV")
                 PROCESSNAME = _get_conf("PLUGINKIT_PROCESSNAME")
                 UWSGI_ENABLED = _get_conf("PLUGINKIT_UWSGI_ENABLED")
                 GUNICORN_ENABLED = _get_conf("PLUGINKIT_GUNICORN_ENABLED")
 
                 #: get gunicorn or uwsgi masterpid
@@ -243,17 +234,15 @@
                 suffix = "." + secure_filename(f.filename).split(".")[-1]
                 with NamedTemporaryFile(
                     mode="w+b", prefix="fpk-web-", suffix=suffix, delete=False
                 ) as fp:
                     fp.write(f.stream.read())
                     filename = fp.name
                 pi = PluginInstaller(pm.plugins_abspath)
-                res = pi.addPlugin(
-                    method="local", filepath=filename, remove=True
-                )
+                res = pi.addPlugin(method="local", filepath=filename, remove=True)
             else:
                 msg = "Unsuccessfully obtained file or format is not allowed"
                 res.update(code=50000, msg=msg)
         elif Action == "downloadPlugin":
             url = request.form.get("url")
             if check_url(url):
                 pi = PluginInstaller(pm.plugins_abspath)
@@ -261,17 +250,15 @@
             else:
                 res.update(code=60000, msg="Please fill in the correct URL")
         elif Action == "installPackage":
             package_or_url = request.form.get("package_or_url")
 
             def _install(package_or_url):
                 pi = PluginInstaller(pm.plugins_abspath)
-                resp = pi.addPlugin(
-                    method="pip", package_or_url=package_or_url
-                )
+                resp = pi.addPlugin(method="pip", package_or_url=package_or_url)
                 if resp["code"] == 0:
                     _queue.append("Install is successful")
                 else:
                     _queue.append(resp["msg"])
 
             thread.start_new_thread(_install, (package_or_url,))
             res.update(code=0)
```

### Comparing `Flask-PluginKit-3.7.2/flask_pluginkit/exceptions.py` & `flask_pluginkit-3.8.0/flask_pluginkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.2/flask_pluginkit/pluginkit.py` & `flask_pluginkit-3.8.0/flask_pluginkit/pluginkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,37 +6,37 @@
     Load and run plugins.
 
     :copyright: (c) 2019 by staugur.
     :license: BSD 3-Clause, see LICENSE for more details.
 """
 
 import logging
-import warnings
 from os import getcwd, listdir, remove
 from os.path import join, dirname, abspath, isdir, isfile, splitext
 from itertools import chain
 from jinja2 import ChoiceLoader, FileSystemLoader
 from flask import (
     Blueprint,
     render_template,
     render_template_string,
     send_from_directory,
     abort,
     url_for,
-    Markup,
     current_app,
 )
+from markupsafe import Markup
 from .utils import isValidPrefix, isValidSemver, Attribution, DcpManager
 from ._compat import string_types, iteritems, text_type
 from .exceptions import PluginError, VersionError, PEPError, TemplateNotFound
 
-try:
-    from flask import _app_ctx_stack as stack
-except ImportError:
-    from flask import _request_ctx_stack as stack
+from typing import Optional, Dict, Union, Any, Sequence, List, Callable
+from flask import Flask
+from logging import Logger
+
+META = Attribution[Dict[str, Union[None, str, list, dict]]]
 
 
 class PluginManager(object):
     """Flask Plugin Manager Extension, collects all plugins and
     maps the metadata to the plugin.
 
     The plugin is a directory or a locally importable module,
@@ -69,27 +69,27 @@
     the PluginManager via a factory::
 
         from flask_pluginkit import Flask, PluginManager
         app = Flask(__name__)
         pm = PluginManager()
         pm.init_app(app)
 
-    :param app: flask application.
+    :param Flask app: flask application.
 
-    :param plugins_base: plugin folder where the plugins resides.
+    :param str plugins_base: plugin folder where the plugins resides.
 
-    :param plugins_folder: base folder for the application.
-                           It is used to build the plugins package name.
+    :param str plugins_folder: base folder for the application.
+                               It is used to build the plugins package name.
 
-    :param logger: logging instance, for debug.
+    :param Logger logger: logging instance, for debug.
 
-    :param stpl: turn on template sorting when the value is True, ASC, DESC.
-                 Sorting rules can be used, DESC or ASC(default).
+    :param str stpl: turn on template sorting when the value is True, ASC, DESC.
+                     Sorting rules can be used, DESC or ASC(default).
 
-    :param plugin_packages: list of third-party plugin packages.
+    :param str plugin_packages: list of third-party plugin packages.
 
     :param static_url_path: can be used to specify a different path for the
                             static files on the plugins. Defaults to the name
                             of the `static_endpoint` folder.
 
     :param static_endpoint: the endpoint name of plugins static files
                             that should be served at `static_url_path`.
@@ -124,103 +124,100 @@
         a warning will be issued.
 
     .. versionchanged:: 3.7.0
         Add ``p3`` feature for beta.
 
     .. deprecated:: 3.7.2
         Remove `before_first_request` hep
+
+    .. deprecated:: 3.8.0
+        Remove `stpl_reverse` and `try_compatible` param.
     """
 
     def __init__(
-        self, app=None, plugins_base=None, plugins_folder="plugins", **options
+        self,
+        app: Optional[Flask] = None,
+        plugins_base: Optional[str] = None,
+        plugins_folder: Optional[str] = "plugins",
+        **options: Dict[str, Any],
     ):
         """Receive initialization parameters and
         pass options to :meth:`init_app` method.
         """
         #: logging Logger instance
-        self.logger = options.get("logger", logging.getLogger(__name__))
+        self.logger: Logger = options.get("logger", logging.getLogger(__name__))
 
         #: Template sorting
-        self.stpl = options.get("stpl", False)
+        self.stpl: Union[str, bool] = options.get("stpl", False)
 
         #: Template sort order, True descending, False ascending (default).
-        if "stpl_reverse" in options:
-            warnings.warn(
-                "stpl_reverse: will be removed in the next minor version,"
-                " please use `stpl` instead.",
-            )
-        self.stpl_reverse = options.get("stpl_reverse", False)
         if self.stpl in ("asc", "desc", "ASC", "DESC"):
             self.stpl = True
-            self.stpl_reverse = False if self.stpl in ("asc", "ASC") else True
+            self.stpl_reverse: bool = False if self.stpl in ("asc", "ASC") else True
 
         #: Third-party plugin package
         self.plugin_packages = options.get("plugin_packages") or []
         if not isinstance(self.plugin_packages, (tuple, list)):
             raise PluginError("Invalid plugin_packages")
 
         #: Static endpoint
-        self.static_endpoint = options.get("static_endpoint") or "assets"
+        self.static_endpoint: str = options.get("static_endpoint") or "assets"
 
         #: Static url prefix
-        self.static_url_path = (
-            options.get("static_url_path") or "/%s" % self.static_endpoint
+        self.static_url_path: str = (
+            options.get("static_url_path") or f"/{self.static_endpoint}"
         )
         if not isValidPrefix(self.static_url_path):
             raise PluginError("Invalid static_url_path")
 
         #: Configuration Dictionary of Flask-PLuginKit in Project
-        self.pluginkit_config = options.get("pluginkit_config") or {}
+        self.pluginkit_config: Dict[str, Any] = options.get("pluginkit_config") or {}
         if not isinstance(self.pluginkit_config, dict):
             raise PluginError("Invalid pluginkit_config")
 
         #: Plugins Extended Processor
-        self.__pet_handlers = {
+        self.__pet_handlers: Dict[str, Callable] = {
             "tep": self._tep_handler,
             "hep": self._hep_handler,
             "bep": self._bep_handler,
             "vep": self._vep_handler,
             "cvep": self._cvep_handler,
             "errhandler": self._error_handler,
             "filter": self._filter_handler,
             "tcp": self._context_processor_handler,
             "p3": self._p3_handler,
         }
 
         #: Hook extension type handlers
-        self.__het_allow_hooks = {
+        self.__het_allow_hooks: Dict[str, Callable] = {
             "before_request": self.__before_request_hook_handler,
             "after_request": self.__after_request_hook_handler,
             "teardown_request": self.__teardown_request_hook_handler,
         }
 
         #: Dynamic Connection Point
         #:
         #: .. versionadded:: 3.2.0
         self._dcp_manager = DcpManager()
 
-        #: Compatibility loading
-        #:
-        #: .. versionadded:: 3.3.1
-        if "try_compatible" in options:
-            warnings.warn(
-                "try_compatible: will be removed in the next minor version"
-            )
-        self._try_compatible = options.get("try_compatible", True)
-
         #: All locally stored plugins
-        self.__plugins = []
+        self.__plugins: List = []
 
         #: Initialize app via a factory
         if app is not None:
             self.init_app(app, plugins_base, plugins_folder)
 
-    def init_app(self, app, plugins_base=None, plugins_folder="plugins"):
-        self.plugins_folder = plugins_folder
-        self.plugins_abspath = join(
+    def init_app(
+        self,
+        app: Flask,
+        plugins_base: Optional[str] = None,
+        plugins_folder: Optional[str] = "plugins",
+    ):
+        self.plugins_folder: str = plugins_folder
+        self.plugins_abspath: str = join(
             plugins_base or getattr(app, "root_path", getcwd()),
             self.plugins_folder,
         )
 
         #: Scan and load plugins for :attr:`plugins_folder` and third-plugins
         self.logger.debug(
             "Start plugins initialization, local plugins path: %s, third party"
@@ -323,40 +320,32 @@
         for tf in self.get_enabled_filters:
             if tf and tf[0] not in app.jinja_env.filters:
                 app.add_template_filter(tf[-1], tf[0])
 
         #: Register the error handlers
         #:
         #: .. versionadded:: 3.2.0
-        for (err_code_exc, errview) in self.get_enabled_errhandlers:
+        for err_code_exc, errview in self.get_enabled_errhandlers:
             app.register_error_handler(err_code_exc, errview)
 
         #: Register the template context processors
         #:
         #: .. versionadded:: 3.2.0
         app.template_context_processors[None].append(
-            lambda: {
-                k: v
-                for tcp in self.get_enabled_tcps
-                for k, v in iteritems(tcp)
-            }
+            lambda: {k: v for tcp in self.get_enabled_tcps for k, v in iteritems(tcp)}
         )
 
         #: register extension with app
         app.extensions = getattr(app, "extensions", None) or {}
         app.extensions["pluginkit"] = self
 
     def __scan_third_plugins(self):
-        if self.plugin_packages and isinstance(
-            self.plugin_packages, (list, tuple)
-        ):
+        if self.plugin_packages and isinstance(self.plugin_packages, (list, tuple)):
             for package_name in self.plugin_packages:
-                self.logger.debug(
-                    "find third plugin package: %s" % package_name
-                )
+                self.logger.debug("find third plugin package: %s" % package_name)
                 try:
                     plugin = __import__(package_name)
                 except ImportError as e:
                     raise PluginError(e)
                 else:
                     plugin_abspath = dirname(abspath(plugin.__file__))
                     self.__load_plugin(plugin, plugin_abspath, package_name)
@@ -366,74 +355,26 @@
             join(self.plugins_abspath, "__init__.py")
         ):
             for package_name in listdir(self.plugins_abspath):
                 package_abspath = join(self.plugins_abspath, package_name)
                 if isdir(package_abspath) and isfile(
                     join(package_abspath, "__init__.py")
                 ):
-                    self.logger.debug(
-                        "find local plugin package: %s" % package_name
-                    )
+                    self.logger.debug("find local plugin package: %s" % package_name)
                     #: Dynamic load module (plugins.package):
                     #: you can query custom information and get the plugin's
                     #: class definition through `register` function.
                     plugin = __import__(
                         "%s.%s" % (self.plugins_folder, package_name),
                         fromlist=[
                             self.plugins_folder,
                         ],
                     )
                     self.__load_plugin(plugin, package_abspath, package_name)
 
-    def __try_load_oldmeta(self, p_obj):
-        """Try compatible with the old version
-
-        :param p_obj: dynamically loaded plugin modules
-
-        .. versionadded:: 3.3.1
-
-        .. versionchanged:: 3.4.0
-            Check, if no getPluginClass, raise PluginError
-        """
-        if hasattr(p_obj, "register"):
-            return
-
-        #: Set resp
-        resp = {}
-
-        #: Detection plugin information
-        if hasattr(p_obj, "getPluginClass"):
-            #: Get the plugin main class and instantiate it
-            p = p_obj.getPluginClass()()
-
-            #: Register the template extension point
-            if hasattr(p, "register_tep"):
-                resp["tep"] = p.register_tep()
-
-            #: Register context extension points
-            if hasattr(p, "register_hep"):
-                heps = p.register_hep()
-                if isinstance(heps, dict):
-                    resp["hep"] = {
-                        hep_name.replace("_hook", ""): hep_func
-                        for hep_name, hep_func in iteritems(heps)
-                    }
-                else:
-                    resp["hep"] = heps
-
-            #: Register the blueprint extension point
-            if hasattr(p, "register_bep"):
-                resp["bep"] = p.register_bep()
-
-        else:
-            raise PluginError("Legacy plugin metadata error")
-
-        #: Dynamically add a function
-        p_obj.register = lambda: resp
-
     def __load_plugin(self, p_obj, package_abspath, package_name):
         """Try to load the plugin.
 
         :param p_obj: dynamically loaded plugin modules
 
         :param package_abspath: absolute path to the module directory
 
@@ -445,31 +386,29 @@
 
         .. versionchanged:: 3.0.1
             Do not check whether it is empty or not.
 
         .. versionchanged:: 3.3.1
             Read and convert the method of getPluginClass in the old version.
         """
-        if self._try_compatible:
-            self.__try_load_oldmeta(p_obj)
         #: Detection plugin information
         if (
             hasattr(p_obj, "__plugin_name__")
             and hasattr(p_obj, "__version__")
             and hasattr(p_obj, "__author__")
             and hasattr(p_obj, "register")
         ):
             #: Plugin extension point.
             #: It should return a dictionary type,
             #: and each element is an extension point, like this:
             #: {"tep":{}, "hep":{}, "bep":{}, "vep":[]}
             pets = p_obj.register()
             if isinstance(pets, dict):
                 #: Get plugin information
-                plugin_info = self._get_plugin_meta(
+                plugin_info: META = self._get_plugin_meta(
                     p_obj, package_abspath, package_name
                 )
                 if plugin_info.plugin_state == "enabled":
                     for pet, value in iteritems(pets):
                         try:
                             self.__pet_handlers[pet](plugin_info, value)
                         except KeyError:
@@ -487,15 +426,15 @@
                 )
         else:
             raise PEPError(
                 "The plugin %s metadata error"
                 % getattr(p_obj, "__plugin_name__", package_name)
             )
 
-    def _get_plugin_meta(self, p_obj, package_abspath, package_name):
+    def _get_plugin_meta(self, p_obj, package_abspath, package_name) -> META:
         """Organize plugin information.
 
         :returns: dict: plugin info
 
         .. versionchanged:: 3.4.0
             plugin_errhandler format change: {} -> []
 
@@ -530,17 +469,15 @@
                 "plugin_package_name": package_name,
                 "plugin_package_abspath": package_abspath,
                 "plugin_description": getattr(p_obj, "__description__", None),
                 "plugin_version": p_obj.__version__,
                 "plugin_author": p_obj.__author__,
                 "plugin_url": getattr(p_obj, "__url__", None),
                 "plugin_license": getattr(p_obj, "__license__", None),
-                "plugin_license_file": getattr(
-                    p_obj, "__license_file__", None
-                ),
+                "plugin_license_file": getattr(p_obj, "__license_file__", None),
                 "plugin_readme_file": getattr(p_obj, "__readme_file__", None),
                 "plugin_state": plugin_state,
                 "plugin_tpl_path": join(package_abspath, "templates"),
                 "plugin_ats_path": join(package_abspath, "static"),
                 "plugin_tep": {},
                 "plugin_hep": {},
                 "plugin_bep": {},
@@ -549,20 +486,20 @@
                 "plugin_filter": [],
                 "plugin_errhandler": [],
                 "plugin_tcp": {},
                 "plugin_p3": {},
             }
         )
 
-    def _tep_handler(self, plugin_info, tep_rule):
+    def _tep_handler(self, plugin_info: META, tep_rule: Dict[str, str]):
         """Template extension point handler.
 
-        :param plugin_info: if tep is valid, will update it.
+        :param META plugin_info: if tep is valid, will update it.
 
-        :param tep_rule: look like {tep_name: your_html_file_or_code}
+        :param dict tep_rule: look like {tep_name: your_html_file_or_code}
 
                         1. This must be dict, where key means that tep is
                         the extension point identifier, and each extension
                         point can contain only one template type, either HTML
                         or string, which requires string,
                         and other types trigger exceptions.
 
@@ -580,44 +517,45 @@
             plugin_tep = {}
             for event, tpl in iteritems(tep_rule):
                 if isinstance(tpl, string_types):
                     if splitext(tpl)[-1] in (".html", ".htm", ".xhtml"):
                         if isfile(
                             join(
                                 plugin_info.plugin_tpl_path,
-                                tpl.split("@")[-1]
-                                if "@" in tpl and self.stpl is True
-                                else tpl,
+                                (
+                                    tpl.split("@")[-1]
+                                    if "@" in tpl and self.stpl is True
+                                    else tpl
+                                ),
                             )
                         ):
                             plugin_tep[event] = dict(fil=tpl)
                         else:
                             raise TemplateNotFound(
                                 "TEP Template File Not Found: %s" % tpl
                             )
                     else:
                         #: Keep Unicode encoding
                         if not isinstance(tpl, text_type):
                             tpl = tpl.decode("utf-8")
                         plugin_tep[event] = dict(cod=tpl)
                 else:
                     raise PEPError(
-                        "The tep content is invalid for %s"
-                        % plugin_info.plugin_name
+                        "The tep content is invalid for %s" % plugin_info.plugin_name
                     )
             #: result look like {tep_name:dict(HTMLFile=str, HTMLString=str)}
             plugin_info["plugin_tep"] = plugin_tep
             self.logger.debug("Register TEP Success")
         else:
             raise PEPError(
                 "The tep rule is invalid for %s, "
                 "it should be a dict." % plugin_info.plugin_name
             )
 
-    def _hep_handler(self, plugin_info, hep_rule):
+    def _hep_handler(self, plugin_info: META, hep_rule: Dict[str, Callable]):
         """Hook extension point handler.
 
         :param hep_rule: look like {hook: func}, the supporting hooks:
 
                         1. before_request, Before request
                         (intercept requests are allowed)
 
@@ -638,27 +576,26 @@
                     else:
                         raise PEPError(
                             "The hep content cannot be called back "
                             "for %s" % plugin_info.plugin_name
                         )
                 else:
                     raise PEPError(
-                        "The hep type is invalid for %s"
-                        % plugin_info.plugin_name
+                        "The hep type is invalid for %s" % plugin_info.plugin_name
                     )
             #: plugin_hep, look like {hep_name:callable, and so on}
             plugin_info["plugin_hep"] = plugin_hep
             self.logger.debug("Register HEP Success")
         else:
             raise PEPError(
                 "The hep rule is invalid for %s, "
                 "it should be a dict." % plugin_info.plugin_name
             )
 
-    def _bep_handler(self, plugin_info, bep_rule):
+    def _bep_handler(self, plugin_info: META, bep_rule: Dict[str, str]):
         """Blueprint extension point handler.
 
         :param bep_rule: look like {blueprint=, prefix=, parent=}
 
         :raises PEPError: if bep rule or content is invalid.
         """
         if (
@@ -671,32 +608,36 @@
                 prefix = bep_rule["prefix"]
             except KeyError:
                 raise PEPError(
                     "The bep rule is invalid for %s" % plugin_info.plugin_name
                 )
             if not isinstance(bp, Blueprint):
                 raise PEPError(
-                    "The bep blueprint is invalid for %s"
-                    % plugin_info.plugin_name
+                    "The bep blueprint is invalid for %s" % plugin_info.plugin_name
                 )
             if not isValidPrefix(prefix, allow_none=True):
                 raise PEPError(
-                    "The bep prefix is invalid for %s"
-                    % plugin_info.plugin_name
+                    "The bep prefix is invalid for %s" % plugin_info.plugin_name
                 )
             #: result look like {blueprint:Blueprint instance, prefix='/xxx'}
             plugin_info["plugin_bep"] = bep_rule
             self.logger.debug("Register BEP Success")
         else:
             raise PEPError(
                 "The bep rule is invalid for %s, "
                 "it should be a dict." % plugin_info.plugin_name
             )
 
-    def _vep_handler(self, plugin_info, vep_rule):
+    def _vep_handler(
+        self,
+        plugin_info: META,
+        vep_rule: Union[
+            Dict[str, Union[str, Callable]], Sequence[Dict[str, Union[str, Callable]]]
+        ],
+    ):
         """Viewfunc extension point handler.
 
         :param vep_rule: look like [{rule=, view_func=, _blurprint=, opts}, ]
 
         :raises PEPError: if vep rule or content is invalid.
 
         .. versionadded:: 3.1.0
@@ -710,38 +651,35 @@
             plugin_vep = []
             for options in vep_rule:
                 try:
                     rule = options.pop("rule")
                     view_func = options.pop("view_func")
                 except KeyError:
                     raise PEPError(
-                        "The vep rule is invalid for %s"
-                        % plugin_info.plugin_name
+                        "The vep rule is invalid for %s" % plugin_info.plugin_name
                     )
                 else:
                     endpoint = options.pop("endpoint", None)
                     #: If it is not None,
                     #: it means that vep is bound to the blueprint
                     #:
                     #: .. versionadded:: 3.6.0
                     _bp = options.pop("_blueprint", None)
 
-                    plugin_vep.append(
-                        (rule, view_func, endpoint, options, _bp)
-                    )
+                    plugin_vep.append((rule, view_func, endpoint, options, _bp))
             #: look like [(rule, view_func, endpoint, opts, bp), (), (), etc.]
             plugin_info["plugin_vep"] = plugin_vep
             self.logger.debug("Register VEP Success")
         else:
             raise PEPError(
                 "The vep rule is invalid for %s, it should be "
                 "a list or tuple." % plugin_info.plugin_name
             )
 
-    def _cvep_handler(self, plugin_info, cvep_rule):
+    def _cvep_handler(self, plugin_info: META, cvep_rule: Sequence[Dict[str, Any]]):
         """Class-based views extension point handler.
 
         :param cvep_rule: look like [{view_class=, other options}, etc.]
 
         :raises PEPError: if cvep rule or content is invalid.
 
         .. versionadded:: 3.5.0
@@ -751,29 +689,32 @@
         if isinstance(cvep_rule, (list, tuple)):
             plugin_cvep = []
             for options in cvep_rule:
                 try:
                     view_class = options.pop("view_class")
                 except KeyError:
                     raise PEPError(
-                        "The cvep rule is invalid for %s"
-                        % plugin_info.plugin_name
+                        "The cvep rule is invalid for %s" % plugin_info.plugin_name
                     )
                 else:
                     plugin_cvep.append((view_class, options))
             #: look like [(view_class, other options), (), (), etc.]
             plugin_info["plugin_cvep"] = plugin_cvep
             self.logger.debug("Register CVEP Success")
         else:
             raise PEPError(
                 "The cvep rule is invalid for %s, it should be "
                 "a list or tuple." % plugin_info.plugin_name
             )
 
-    def _filter_handler(self, plugin_info, filter_rule):
+    def _filter_handler(
+        self,
+        plugin_info: META,
+        filter_rule: Union[Dict[str, Callable], Sequence[Union[Callable, Sequence]]],
+    ):
         """Template filter handler.
 
         :param filter_rule: e.g. {filter_name=func,} or [func, (name,func)]
 
         :raises PEPError: if filter rule or content is invalid.
 
         .. versionadded:: 3.2.0
@@ -797,16 +738,15 @@
         if isinstance(filter_rule, dict):
             plugin_filter = []
             for name, func in iteritems(filter_rule):
                 if callable(func):
                     plugin_filter.append((name, func))
                 else:
                     raise PEPError(
-                        "The filter cannot be called for %s."
-                        % plugin_info.plugin_name
+                        "The filter cannot be called for %s." % plugin_info.plugin_name
                     )
             plugin_info["plugin_filter"] = plugin_filter
         else:
             raise PEPError(
                 "The filter rule is invalid for %s, "
                 "it should be a dict." % plugin_info.plugin_name
             )
@@ -834,33 +774,27 @@
                     )
                 _errhandler_rule.append(dict(error=code, handler=func))
             errhandler_rule = _errhandler_rule
         if isinstance(errhandler_rule, (tuple, list)):
             plugin_errhandler_rules = []
             for eh in errhandler_rule:
                 #: eh is dict, look like {error: code_or_class, handler: func}
-                if (
-                    not isinstance(eh, dict)
-                    or "error" not in eh
-                    or "handler" not in eh
-                ):
+                if not isinstance(eh, dict) or "error" not in eh or "handler" not in eh:
                     raise PEPError(
-                        "The errhandler format error for %s"
-                        % plugin_info.plugin_name
+                        "The errhandler format error for %s" % plugin_info.plugin_name
                     )
                 code_or_exc = eh["error"]
                 func = eh["handler"]
                 if not isinstance(code_or_exc, int):
                     try:
                         _is_ok_exc = issubclass(code_or_exc, Exception)
                     except TypeError:
                         raise PEPError(
                             "The errhandler custom error class requires"
-                            " inheritance of Exception for %s"
-                            % plugin_info.plugin_name
+                            " inheritance of Exception for %s" % plugin_info.plugin_name
                         )
                     else:
                         if not _is_ok_exc:
                             raise PEPError(
                                 "The errhandler exc is not a subclass of"
                                 " Exception for %s" % plugin_info.plugin_name
                             )
@@ -971,16 +905,15 @@
                         if pet in petns:
                             obj = "plugin_" + pet
                             try:
                                 ov = p[obj]
                                 nv = func(ov)
                                 if type(ov) != type(nv):
                                     raise PluginError(
-                                        "Illegal extension point"
-                                        " data type(%s)" % pet
+                                        "Illegal extension point" " data type(%s)" % pet
                                     )
                             except Exception as e:
                                 self.logger.debug(e)
                                 raise PEPError(from_pname, str(e))
                             else:
                                 p[obj] = nv
             nplugins.append(p)
@@ -1080,19 +1013,15 @@
 
         :returns: List of nested tuples, like [(filter_name, filter_func),]
 
         .. versionadded:: 3.2.0
         """
         return list(
             chain.from_iterable(
-                [
-                    p.plugin_filter
-                    for p in self.get_enabled_plugins
-                    if p.plugin_filter
-                ]
+                [p.plugin_filter for p in self.get_enabled_plugins if p.plugin_filter]
             )
         )
 
     @property
     def get_enabled_errhandlers(self):
         """Get all error handlers for the enabled plugins.
 
@@ -1128,19 +1057,15 @@
             if p.plugin_tcp
         ]
 
     def get_plugin_info(self, plugin_name):
         """Get plugin information from all plugins"""
         try:
             return next(
-                (
-                    p
-                    for p in self.get_all_plugins
-                    if p.plugin_name == plugin_name
-                )
+                (p for p in self.get_all_plugins if p.plugin_name == plugin_name)
             )
         except StopIteration:
             raise PluginError("No plugin named %s was found" % plugin_name)
 
     def disable_plugin(self, plugin_name):
         """Disable a plugin (that is, create a DISABLED empty file)
         and restart the application to take effect.
@@ -1221,20 +1146,15 @@
             tep_result["fil"] = _sort_refresh("fil")
             tep_result["cod"] = _sort_refresh("cod")
 
         mtf = Markup(
             "".join([render_template(i, **context) for i in tep_result["fil"]])
         )
         mtc = Markup(
-            "".join(
-                [
-                    render_template_string(i, **context)
-                    for i in tep_result["cod"]
-                ]
-            )
+            "".join([render_template_string(i, **context) for i in tep_result["cod"]])
         )
 
         typ = "all" if typ not in ("fil", "cod") else typ
         if typ == "fil":
             return mtf
         elif typ == "cod":
             return mtc
@@ -1332,11 +1252,8 @@
 
     Example usage::
 
         push_dcp('demo', lambda:'Hello dcp')
 
     .. versionadded:: 3.2.0
     """
-    ctx = stack.top
-    ctx.app.extensions.get("pluginkit")._dcp_manager.push(
-        event, callback, position
-    )
+    current_app.extensions.get("pluginkit")._dcp_manager.push(event, callback, position)
```

### Comparing `Flask-PluginKit-3.7.2/flask_pluginkit/static/translations.ini` & `flask_pluginkit-3.8.0/flask_pluginkit/static/translations.ini`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.2/flask_pluginkit/templates/manager.html` & `flask_pluginkit-3.8.0/flask_pluginkit/templates/manager.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <title>Plugins Web Manager based Flask-PluginKit!</title>
     <link href="https://static.saintic.com/cdn/flask-pluginkit/favicon.ico" rel="icon" type="image/x-icon" />
     <link href="https://static.saintic.com/cdn/flask-pluginkit/favicon.ico" rel="shortcut icon" type="image/x-icon" />
     <link rel="prefetch" type="application/l10n" href="{{ url_for('.static', filename='translations.ini') }}" />
-    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@0.9.3/css/bulma.min.css">
+    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@1.0.0/css/bulma.min.css">
     <link rel="stylesheet" type="text/css" href="https://static.saintic.com/cdn/iconfont/iconfont.css">
     <style type="text/css">
         .notification>button.delete {
             border: none;
         }
 
         .is-hidden {
@@ -35,15 +35,16 @@
                         <span class="tag is-black" data-l10n-id="{{ k }}">{{ k }}</span>
                         <span class="tag">{{ v }}</span>
                     </div>
                 </div>
                 {% endfor %}
                 <div class="control">
                     <div class="select is-success is-small">
-                        <select onchange="document.webL10n.setLanguage(this.value || this.options[this.selectedIndex].text);">
+                        <select
+                            onchange="document.webL10n.setLanguage(this.value || this.options[this.selectedIndex].text);">
                             <option disabled selected>Language</option>
                             <option>en</option>
                             <option>zh-cn</option>
                         </select>
                     </div>
                 </div>
             </div>
@@ -123,16 +124,16 @@
                     {% for p in g.pluginkit.get_all_plugins %}
                     <tr>
                         <th>{{ loop.index }}</th>
                         <th><abbr title="{{ p.plugin_package_name }}">{{ p.plugin_name }}</abbr></th>
                         <th>{{ p.plugin_description or '' }}</th>
                         <th>{{ p.plugin_version }}</th>
                         <th>{{ p.plugin_author }}</th>
-                        <th>{% if p.plugin_url %}<a href="{{ p.plugin_url }}"
-                                target="_blank">{{ p.plugin_url }}</a>{% else %}{{ p.plugin_url or '' }}{% endif %}</th>
+                        <th>{% if p.plugin_url %}<a href="{{ p.plugin_url }}" target="_blank">{{ p.plugin_url }}</a>{%
+                            else %}{{ p.plugin_url or '' }}{% endif %}</th>
                         <th>{{ p.plugin_license or '' }}</th>
                         <th>
                             <scan
                                 class="{% if p.plugin_state == 'enabled' %}has-text-primary{% else %}has-text-warning{% endif %}">
                                 {{ p.plugin_state }}</scan>
                         </th>
                         <th>
@@ -150,15 +151,15 @@
             </table>
             <div class="notification" id="notification" style="display: none;">
                 <button class="delete"></button>
                 <div id="message"></div>
             </div>
         </div>
     </section>
-    <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/jquery@3.6.0/dist/jquery.min.js"></script>
+    <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/jquery@3.7.1/dist/jquery.min.js"></script>
     <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/webl10n@1.0.0/l10n.min.js"></script>
     <script type="text/javascript">
         function showNotification() {
             document.getElementById("notification").style.display = 'block';
         }
 
         function hideNotification() {
@@ -191,15 +192,15 @@
                 options = {};
             }
             return $.ajax({
                 url: url,
                 method: options.method || 'post',
                 dataType: options.dataType || 'json',
                 data: options.data || {},
-                beforeSend: options.beforeSend ? options.beforeSend : function () {},
+                beforeSend: options.beforeSend ? options.beforeSend : function () { },
                 success: function (res) {
                     if (res.code === 0 || res.success === true) {
                         success && success(res);
                     } else {
                         if (options.msgprefix != false) {
                             setMessage("<scan class='has-text-danger'>" + (options.msgprefix || '') + (res
                                 .msg || res.code) + "</scan>");
@@ -208,15 +209,15 @@
                     }
                 },
                 error: function (XMLHttpRequest, textStatus, errorThrown) {
                     setMessage(
                         "<scan class='has-text-danger'>System exception, please try again later</scan>. Status code:" +
                         XMLHttpRequest.status + "," + textStatus);
                 },
-                complete: options.complete ? options.complete : function () {}
+                complete: options.complete ? options.complete : function () { }
             });
         }
 
         function enablePlugin(plugin_name) {
             ajax("{{ url_for('.api', Action='enablePlugin') }}&plugin_name=" + plugin_name, function (res) {
                 setMessage(
                     "<scan class='has-text-success'>Enabled. Restart the application and take effect.</scan>"
@@ -251,15 +252,15 @@
         let isLoop = 0;
         function getLoopMsg() {
             if (isLoop === 1) {
                 return;
             }
             isLoop = 1;
             let sse = new EventSource("{{ url_for('.msg') }}");
-            sse.onmessage = function(e) {
+            sse.onmessage = function (e) {
                 if (e.data !== "") {
                     setMessage("<scan>" + e.data + "</scan>");
                 }
             }
         }
 
         $('#upload-plugin-submit').click(function () {
```

### Comparing `Flask-PluginKit-3.7.2/flask_pluginkit/utils.py` & `flask_pluginkit-3.8.0/flask_pluginkit/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,62 +7,58 @@
 
     :copyright: (c) 2019 by staugur.
     :license: BSD 3-Clause, see LICENSE for more details.
 """
 
 import json
 import shelve
-from semver import VersionInfo
+from semver.version import Version
+from functools import cmp_to_key
 from os.path import join, abspath
 from tempfile import gettempdir
 from collections import deque
-from flask import Markup, Response, jsonify
-from flask.app import setupmethod, Flask as _BaseFlask
-from ._compat import PY2, string_types, text_type, iteritems
+from markupsafe import Markup
+from flask import Response, jsonify
+from ._compat import string_types, text_type, iteritems
 from .exceptions import PluginError, NotCallableError
+from typing import List, Any, Optional, Dict
 
 
-def isValidPrefix(prefix, allow_none=False):
+def isValidPrefix(prefix: str, allow_none: bool = False) -> bool:
     """Check if it can be used for blueprint prefix"""
     if prefix is None and allow_none is True:
         return True
     if isinstance(prefix, string_types):
         return (
             prefix.startswith("/")
             and not prefix.endswith("/")
             and "//" not in prefix
             and " " not in prefix
         )
     return False
 
 
-def isValidSemver(version):
+def isValidSemver(version: str) -> bool:
     """Semantic version number - determines whether the version is qualified.
     The format is MAJOR.Minor.PATCH, more with https://semver.org
     """
     if version and isinstance(version, string_types):
-        return VersionInfo.isvalid(version)
+        return Version.is_valid(version)
     return False
 
 
-def sortedSemver(versions, sort="ASC"):
+def sortedSemver(versions: List[str], sort: str = "ASC") -> List[str]:
     """Semantically sort the list of version Numbers"""
     reverse = True if sort.upper() == "DESC" else False
     if versions and isinstance(versions, (list, tuple)):
-
-        def compare(ver1, ver2):
-            v1 = VersionInfo.parse(ver1)
-            return v1.compare(ver2)
-
-        if PY2:
-            return sorted(versions, cmp=compare, reverse=reverse)
-        else:
-            from functools import cmp_to_key
-
-            return sorted(versions, key=cmp_to_key(compare), reverse=reverse)
+        return sorted(
+            versions,
+            key=cmp_to_key(lambda v1, v2: Version.parse(v1).compare(v2)),
+            reverse=reverse,
+        )
     else:
         raise TypeError("Invaild versions, a list or tuple is right.")
 
 
 class BaseStorage(object):
     """This is the base class for storage.
     The available storage classes need to inherit from :class:`~BaseStorage`
@@ -73,45 +69,45 @@
     and `__delitem__` methods so that the user can call it like a dict.
 
     .. versionchanged:: 3.4.1
         Change :attr:`index` to :attr:`DEFAULT_INDEX`
     """
 
     #: The default index, as the only key, you can override it.
-    DEFAULT_INDEX = "flask_pluginkit_dat"
+    DEFAULT_INDEX: str = "flask_pluginkit_dat"
 
     @property
     def index(self):
         """Get the final index
 
         .. versionadded:: 3.4.1
         """
         return getattr(self, "COVERED_INDEX", None) or self.DEFAULT_INDEX
 
     @index.setter
-    def index(self, _covered_index):
+    def index(self, _covered_index: str):
         """Set the covered index
 
         .. versionadded:: 3.6.0
         """
         self.COVERED_INDEX = _covered_index
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str):
         if hasattr(self, "get"):
             return self.get(key)
         else:
             raise AttributeError("Please override the get method")
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: str, value: Any):
         if hasattr(self, "set"):
             return self.set(key, value)
         else:
             raise AttributeError("Please override the set method")
 
-    def __delitem__(self, key):
+    def __delitem__(self, key: str):
         if hasattr(self, "remove"):
             return self.remove(key)
         else:
             return False
 
     def __str__(self):
         return "<%s object at %s, index is %s>" % (
@@ -122,27 +118,27 @@
 
     __repr__ = __str__
 
 
 class LocalStorage(BaseStorage):
     """Local file system storage based on the shelve module."""
 
-    def __init__(self, path=None):
+    def __init__(self, path: Optional[str] = None):
         self.COVERED_INDEX = path or join(gettempdir(), self.DEFAULT_INDEX)
 
-    def _open(self, flag="c"):
+    def _open(self, flag: str = "c") -> shelve.Shelf:
         return shelve.open(
             filename=abspath(self.index),
             flag=flag,
             protocol=2,
             writeback=False,
         )
 
     @property
-    def list(self):
+    def list(self) -> Dict[str, Any]:
         """list all data
 
         :returns: dict
         """
         db = None
         try:
             db = self._open(flag="r")
@@ -150,22 +146,20 @@
             return dict()
         else:
             return dict(db)
         finally:
             if db:
                 db.close()
 
-    def __ck(self, key):
-        if PY2 and isinstance(key, text_type):
-            key = key.encode("utf-8")
-        if not PY2 and not isinstance(key, text_type):
+    def __ck(self, key: str) -> str:
+        if not isinstance(key, text_type):
             key = key.decode("utf-8")
         return key
 
-    def set(self, key, value):
+    def set(self, key: str, value: Any):
         """Set persistent data with shelve.
 
         :param key: str: Index key
 
         :param value: All supported data types in python
 
         :raises:
@@ -176,40 +170,40 @@
         try:
             db = self._open()
             db[self.__ck(key)] = value
         finally:
             if db:
                 db.close()
 
-    def setmany(self, **mapping):
+    def setmany(self, **mapping: Dict[str, Any]):
         """Set more data
 
         :param mapping: the more k=v
 
         .. versionadded:: 3.4.1
         """
         if mapping and isinstance(mapping, dict):
             db = self._open()
             for k, v in iteritems(mapping):
                 db[self.__ck(k)] = v
             db.close()
 
-    def get(self, key, default=None):
+    def get(self, key: str, default: Any = None):
         """Get persistent data from shelve.
 
         :returns: data
         """
         try:
             value = self.list[key]
         except KeyError:
             return default
         else:
             return value
 
-    def remove(self, key):
+    def remove(self, key: str):
         db = self._open()
         del db[key]
 
     def __len__(self):
         return len(self.list)
 
 
@@ -219,53 +213,48 @@
     def __init__(self, redis_url=None, redis_connection=None):
         self._db = self._open(redis_url) if redis_url else redis_connection
 
     def _open(self, redis_url):
         try:
             from redis import from_url
         except ImportError:
-            raise ImportError(
-                "Please install the redis module, eg: pip install redis"
-            )
+            raise ImportError("Please install the redis module, eg: pip install redis")
         else:
             return from_url(redis_url)
 
     @property
-    def list(self):
+    def list(self) -> Dict[str, Any]:
         """list redis hash data"""
-        return {
-            k: json.loads(v)
-            for k, v in iteritems(self._db.hgetall(self.index))
-        }
+        return {k: json.loads(v) for k, v in iteritems(self._db.hgetall(self.index))}
 
-    def set(self, key, value):
+    def set(self, key: str, value: Any):
         """set key data"""
         return self._db.hset(self.index, key, json.dumps(value))
 
-    def setmany(self, **mapping):
+    def setmany(self, **mapping: Dict[str, Any]):
         """Set more data
 
         :param mapping: the more k=v
 
         .. versionadded:: 3.4.1
         """
         if mapping and isinstance(mapping, dict):
             mapping = {k: json.dumps(v) for k, v in iteritems(mapping)}
             return self._db.hmset(self.index, mapping)
 
-    def get(self, key, default=None):
+    def get(self, key: str, default: Any = None) -> Any:
         """get key original data from redis"""
         v = self._db.hget(self.index, key)
         if v:
-            if not PY2 and not isinstance(v, text_type):
+            if not isinstance(v, text_type):
                 v = v.decode("utf-8")
             return json.loads(v)
         return default
 
-    def remove(self, key):
+    def remove(self, key: str):
         """delete key from redis"""
         return self._db.hdel(self.index, key)
 
     def __len__(self):
         return self._db.hlen(self.index)
 
 
@@ -279,39 +268,14 @@
     @classmethod
     def force_type(cls, rv, environ=None):
         if isinstance(rv, dict):
             rv = jsonify(rv)
         return super(JsonResponse, cls).force_type(rv, environ)
 
 
-class Flask(_BaseFlask):
-    @setupmethod
-    def before_request_top(self, f):
-        """Registers a function to run before each request. Priority First.
-
-        The usage is equivalent to the :meth:`flask.Flask.before_request`
-        decorator, and before_request registers the function at the end of
-        the before_request_funcs, while this decorator registers the function
-        at the top of the before_request_funcs (index 0).
-
-        Because flask-pluginkit has registered all cep into the app
-        at load time, if your web application uses before_request and plugins
-        depend on one of them (like g), the plugin will not run properly,
-        so your web application should use this decorator at this time.
-        """
-        self.before_request_funcs.setdefault(None, []).insert(0, f)
-        return f
-
-    @setupmethod
-    def before_request_second(self, f):
-        """Registers a function to run before each request. Priority Second."""
-        self.before_request_funcs.setdefault(None, []).insert(1, f)
-        return f
-
-
 class Attribution(dict):
     """A dict that allows for object-like property access syntax."""
 
     def __getattr__(self, name):
         try:
             return self[name]
         except KeyError:
@@ -381,28 +345,28 @@
             if rv:
                 if not isinstance(rv, text_type):
                     rv = rv.decode("utf-8")
                 results.append(rv)
         return Markup("".join(results))
 
 
-def allowed_uploaded_plugin_suffix(filename):
+def allowed_uploaded_plugin_suffix(filename: str) -> bool:
     """Check suffix for uploaded filename
 
     .. versionadded:: 3.3.0
     """
     allow_suffix = [".tar.gz", ".tgz", ".zip"]
     if isinstance(filename, string_types):
         for suffix in allow_suffix:
             if filename.endswith(suffix):
                 return True
     return False
 
 
-def check_url(addr):
+def check_url(addr: str) -> bool:
     """Check whether UrlAddr is in a valid format, for example::
 
         http://ip:port
         https://abc.com
 
     .. versionadded:: 3.3.0
     """
```

### Comparing `Flask-PluginKit-3.7.2/tests/test_installer.py` & `flask_pluginkit-3.8.0/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `Flask-PluginKit-3.7.2/tests/test_pm.py` & `flask_pluginkit-3.8.0/tests/test_pm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 
 import os
 import sys
 import time
 import json
 import unittest
-from flask import Flask, request, Markup, g
+from flask import Flask, request, g
+from markupsafe import Markup
 from flask_pluginkit import (
-    Flask as ExFlask,
     PluginManager,
     LocalStorage,
     push_dcp,
     blueprint,
 )
 from flask_pluginkit.exceptions import PluginError, NotCallableError
-from flask_pluginkit._compat import PY2, iteritems
+from flask_pluginkit._compat import iteritems
 from jinja2 import ChoiceLoader
 
 EXAMPLE_DIR = os.path.join(
     os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
     "examples/fulldemo",
 )
 sys.path.append(EXAMPLE_DIR)
@@ -36,96 +36,66 @@
 app1.register_blueprint(blueprint)
 
 #: app2 without flask-pluginkit
 app2 = Flask("app2")
 app2.config["TESTING"] = True
 app2.register_blueprint(blueprint)
 
-#: app3 with flask-pluginkit and exflask
-def create_app3():
-    app3 = ExFlask("app3")
-    app3.config["TESTING"] = True
-    pm = PluginManager(pluginkit_config=dict(whoami="app3"))
-    pm.init_app(app3)
-    return app3
-
-
-app3 = create_app3()
-
 #: app4 with flask-pluginkit full example
 from app import app as app4
 
 app4.testing = True
 
 
 class PMTest(unittest.TestCase):
     def setUp(self):
         self.app1_pm = app1.extensions.get("pluginkit")
-        self.app3_pm = app3.extensions.get("pluginkit")
         self.app4_pm = app4.extensions.get("pluginkit")
 
     def test_extself(self):
         self.assertIsInstance(self.app1_pm, PluginManager)
-        self.assertIsInstance(self.app3_pm, PluginManager)
         self.assertIsInstance(self.app4_pm, PluginManager)
         self.assertIsInstance(app1.jinja_loader, ChoiceLoader)
 
     def test_extself_params(self):
         self.assertFalse(os.path.isdir(self.app1_pm.plugins_abspath))
-        self.assertFalse(os.path.isdir(self.app3_pm.plugins_abspath))
         self.assertTrue(os.path.isdir(self.app4_pm.plugins_abspath))
         self.assertIsInstance(self.app1_pm.plugin_packages, (tuple, list))
-        self.assertTrue(self.app3_pm.static_url_path.startswith("/"))
         self.assertIsInstance(self.app4_pm.pluginkit_config, dict)
 
     def test_extself_raise(self):
         with self.assertRaises(PluginError) as cm:
             PluginManager(Flask(__name__), plugin_packages=123)
             PluginManager(Flask(__name__), plugin_packages=["non_ppk"])
 
     def test_extself_tpl_global(self):
         self.assertIn("emit_tep", app1.jinja_env.globals)
-        self.assertIn("emit_assets", app3.jinja_env.globals)
         self.assertIn("emit_config", app4.jinja_env.globals)
 
-    def test_exflask(self):
-        @app3.before_request
-        def my_test():
-            pass
-
-        self.assertTrue(hasattr(app3, "before_request_top"))
-        self.assertTrue(hasattr(app3, "before_request_second"))
-
     def test_config(self):
-        self.assertEqual(self.app3_pm.pluginkit_config["whoami"], "app3")
         self.assertTrue("emit_config" in app1.jinja_env.globals)
         with app1.test_request_context():
             self.assertTrue(self.app1_pm.emit_config("PLUGINKIT_TEST"))
 
     def test_hook(self):
         with app4.test_request_context("/"):
             app4.preprocess_request()
             local = LocalStorage()
             self.assertTrue("nowtime" in local.list)
-            nowhour = time.strftime(
-                "%Y-%m-%d %H:", time.localtime(time.time())
-            )
+            nowhour = time.strftime("%Y-%m-%d %H:", time.localtime(time.time()))
             self.assertIn(nowhour, local.get("nowtime"))
             del local["nowtime"]
 
     def test_example(self):
-        if not PY2:
-            with app4.test_client() as c:
-                rv = c.get("/")
-                data = rv.data.decode("utf-8")
-                self.assertTrue("css/style.css" in data)
-                self.assertTrue("js/hello.js" in data)
-                self.assertTrue(
-                    self.app4_pm.pluginkit_config["whoami"] in data
-                )
+        with app4.test_client() as c:
+            rv = c.get("/")
+            data = rv.data.decode("utf-8")
+            self.assertTrue("css/style.css" in data)
+            self.assertTrue("js/hello.js" in data)
+            self.assertTrue(self.app4_pm.pluginkit_config["whoami"] in data)
         self.assertEqual(len(app4.blueprints), 3)
         self.assertEqual(len(self.app4_pm.get_all_plugins), 3)
         self.assertEqual(len(self.app4_pm.get_enabled_beps), 2)
         self.assertIn(self.app4_pm.static_endpoint, app4.view_functions)
         with app4.test_request_context():
             link = self.app4_pm.emit_assets("localdemo", "css/style.css")
             self.assertTrue("stylesheet" in link)
@@ -147,17 +117,15 @@
 
     def test_filter(self):
         self.assertIn("repeat_filter", app4.jinja_env.filters)
         self.assertIn("demo_filter2", app4.jinja_env.filters)
         self.assertEqual(
             "test-filter-repeat", app4.jinja_env.filters["repeat_filter"]("x")
         )
-        self.assertEqual(
-            "test-filter", app4.jinja_env.filters["demo_filter2"]("x")
-        )
+        self.assertEqual("test-filter", app4.jinja_env.filters["demo_filter2"]("x"))
 
     def test_errhandler(self):
         ehs = app4.error_handler_spec[None]
         self.assertIsInstance(ehs, dict)
         self.assertIn(403, ehs)
         self.assertIn(404, ehs)
         with app4.test_client() as c:
@@ -165,21 +133,18 @@
             self.assertEqual(404, resp404.status_code)
             self.assertIn(b"Not Found Page", resp404.data)
             resp403 = c.get("/403")
             self.assertEqual(403, resp403.status_code)
             self.assertIn(b"permission deny", resp403.data)
             #: raise apierror
             respapierror = c.get("/api_error")
-            if PY2:
-                data = json.loads(respapierror.data)
+            if isinstance(respapierror.data, bytes):
+                data = json.loads(respapierror.data.decode("utf-8"))
             else:
-                if isinstance(respapierror.data, bytes):
-                    data = json.loads(respapierror.data.decode("utf-8"))
-                else:
-                    data = json.loads(respapierror.data)
+                data = json.loads(respapierror.data)
             self.assertIsInstance(data, dict)
             self.assertIn("msg", data)
             self.assertEqual("test_err_class_handler", data["msg"])
             self.assertEqual(10000, data["code"])
 
     def test_tcp(self):
         context = {
@@ -190,34 +155,35 @@
         self.assertIsInstance(context, dict)
         self.assertIn("timestamp", context)
         self.assertIn("change_to_str", context)
         self.assertTrue(context["change_to_str"], str)
         # test p3
         self.assertIn("im", context)
 
+    """
     def test_dcp(self):
         def callback():
             return "test"
 
         self.assertRaises(AttributeError, push_dcp, "raise", callback)
         with app4.app_context():
             push_dcp("test", callback)
             result = [f() for f in self.app4_pm._dcp_manager.list["test"]]
             ft = self.app4_pm._dcp_manager.emit("test")
             self.assertRaises(PluginError, push_dcp, ["raise"], callback)
             self.assertRaises(NotCallableError, push_dcp, "raise", "abc")
             self.assertIsInstance(ft, Markup)
             self.assertEqual(ft, Markup("test"))
             self.assertEqual(result, ["test"])
+    """
 
     def test_web(self):
         with app1.test_client() as c1:
             data = c1.post("/api").data
-            if not PY2 and isinstance(data, bytes):
-                data = data.decode("utf-8")
+            data = data.decode("utf-8")
             res = json.loads(data)
             self.assertIsInstance(res, dict)
             self.assertEqual(res["code"], 1)
         with app2.test_client() as c2:
             res = c2.post("/api").data
             self.assertIn(b"Authentication failed", res)
```

### Comparing `Flask-PluginKit-3.7.2/tests/test_utils.py` & `flask_pluginkit-3.8.0/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # -*- coding: utf-8 -*-
 
 import unittest
 from os import getenv
-from sys import version_info
 from flask_pluginkit.utils import (
     isValidSemver,
     sortedSemver,
     isValidPrefix,
     LocalStorage,
     RedisStorage,
     BaseStorage,
     allowed_uploaded_plugin_suffix,
     Attribution,
     check_url,
     DcpManager,
 )
-from flask import Markup
-
-PY35 = (version_info.major, version_info.minor) == (3, 5)
+from markupsafe import Markup
 
 
 class UtilsTest(unittest.TestCase):
     def test_isVer(self):
         self.assertTrue(isValidSemver("0.0.1"))
         self.assertTrue(isValidSemver("1.1.1-beta"))
         self.assertTrue(isValidSemver("1.1.1-beta+compile10"))
@@ -71,15 +68,14 @@
         # Invalid, LocalStorage did not implement this method
         del storage["test"]
         self.assertIsNone(storage.get("test"))
         self.assertIsNone(storage["_non_existent_key_"])
         self.assertEqual(1, storage.get("_non_existent_key_", 1))
         self.assertEqual(0, len(storage))
 
-    @unittest.skipIf(PY35, "Damn py3.5 anomaly.")
     def test_redisstorage(self):
         """Run this test when it detects that the environment variable
         FLASK_PLUGINKIT_TEST_REDISURL is valid
         """
         redis_url = getenv("FLASK_PLUGINKIT_TEST_REDISURL")
         if redis_url:
             storage = RedisStorage(redis_url=redis_url)
@@ -132,16 +128,15 @@
         self.assertEqual(d.a, 1)
         self.assertIsInstance(d, dict)
 
     def test_dcp(self):
         dcp = DcpManager()
         self.assertIsInstance(dcp.list, dict)
 
-        def f():
-            return "test"
+        f = lambda: "test"
 
         dcp.push("f", f)
         self.assertEqual(len(dcp.list), 1)
         self.assertEqual(dcp.emit("f"), Markup("test"))
         self.assertTrue(dcp.remove("f", f))
         self.assertEqual(len(dcp.list), 1)
```

