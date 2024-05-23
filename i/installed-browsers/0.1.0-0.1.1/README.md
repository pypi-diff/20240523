# Comparing `tmp/installed_browsers-0.1.0.tar.gz` & `tmp/installed_browsers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "installed_browsers-0.1.0.tar", max compression
+gzip compressed data, was "installed_browsers-0.1.1.tar", max compression
```

## Comparing `installed_browsers-0.1.0.tar` & `installed_browsers-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-01-21 09:31:02.412911 installed_browsers-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2024-01-21 09:31:02.412911 installed_browsers-0.1.0/README.md
--rw-r--r--   0        0        0     5271 2024-01-21 09:31:02.412911 installed_browsers-0.1.0/installed_browsers/__init__.py
--rw-r--r--   0        0        0      342 2024-01-21 09:31:02.412911 installed_browsers-0.1.0/installed_browsers/common.py
--rw-r--r--   0        0        0     5114 2024-01-21 09:31:02.412911 installed_browsers-0.1.0/installed_browsers/linux.py
--rw-r--r--   0        0        0     5098 2024-01-21 09:31:02.412911 installed_browsers-0.1.0/installed_browsers/mac.py
--rw-r--r--   0        0        0     2983 2024-01-21 09:31:02.412911 installed_browsers-0.1.0/installed_browsers/windows.py
--rw-r--r--   0        0        0     1936 2024-01-21 09:31:02.412911 installed_browsers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 installed_browsers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-23 19:29:54.356359 installed_browsers-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3350 2024-05-23 19:29:54.356359 installed_browsers-0.1.1/README.md
+-rw-r--r--   0        0        0     6053 2024-05-23 19:29:54.356359 installed_browsers-0.1.1/installed_browsers/__init__.py
+-rw-r--r--   0        0        0      285 2024-05-23 19:29:54.356359 installed_browsers-0.1.1/installed_browsers/common.py
+-rw-r--r--   0        0        0     5756 2024-05-23 19:29:54.356359 installed_browsers-0.1.1/installed_browsers/linux.py
+-rw-r--r--   0        0        0     6818 2024-05-23 19:29:54.356359 installed_browsers-0.1.1/installed_browsers/mac.py
+-rw-r--r--   0        0        0    14130 2024-05-23 19:29:54.356359 installed_browsers-0.1.1/installed_browsers/windows.py
+-rw-r--r--   0        0        0     1962 2024-05-23 19:29:54.356359 installed_browsers-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4192 1970-01-01 00:00:00.000000 installed_browsers-0.1.1/PKG-INFO
```

### Comparing `installed_browsers-0.1.0/LICENSE` & `installed_browsers-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `installed_browsers-0.1.0/installed_browsers/__init__.py` & `installed_browsers-0.1.1/installed_browsers/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,150 @@
-import fnmatch
 import sys
 from typing import Iterator, Optional
 
 from . import linux, mac, windows
 from .common import Browser, Version, OS
 
 __all__ = ["Browser",
            "browsers",
+           "what_is_the_default_browser",
            "do_i_have_installed",
            "give_me_details_of",
-           "get_version_of",
-           "what_is_the_default_browser"]
+           "get_version_of"]
 
 
+# get all installed browsers
 def browsers() -> Iterator[Browser]:
     """
-    Iterates over installed browsers.
+    Iterates over installed browsers.\n
+    Locally installed browser versions (portable) are not considered.
 
-    :return: Iterator of Tuple of browser key and browser information.
+    :return: Iterator of dictionary of browser key and information.
     """
     match sys.platform:
         case OS.LINUX:
             yield from linux.browsers()
-        case OS.WINDOWS:
-            yield from windows.browsers()
         case OS.MAC:
             yield from mac.browsers()
+        case OS.WINDOWS:
+            yield from windows.browsers()
         case _:
-            print("This operation system is not yet supported.")
+            yield Browser(
+                name="exception", description="This operating system is not yet supported.", version="", location=""
+            )
+
+
+# get default browser
+def what_is_the_default_browser():
+    """
+    Shows the default browser in system - if there is any.
+
+    :return: Default browser description.
+    """
+    match sys.platform:
+        case OS.LINUX:
+            return linux.what_is_the_default_browser()
+        case OS.MAC:
+            return mac.what_is_the_default_browser()
+        case OS.WINDOWS:
+            return windows.what_is_the_default_browser()
 
 
+# check if the given browser is installed
 def do_i_have_installed(name: str):
     """
     Checks if the provided browser is installed in system.
 
     Parameters:
                 Possible browser entries / parameters\n
                 for Linux:\n
-                chrome, chromium, firefox, ms-edge, opera, opera-beta, opera-developer,
+                chrome, chromium, firefox, opera, opera-beta, opera-developer, msedge, msedge-beta, msedge-dev
                 brave, brave-beta, brave-nightly\n
                 for macOS:\n
                 chrome, chrome-canary, chromium, firefox, firefox-developer, firefox-nightly,
-                safari, opera, opera-beta, opera-developer, ms-edge, ms-edge-beta, ms-edge-dev, ms-edge-canary,
-                brave, brave-beta, brave-dev, brave-nightly\n
+                safari, opera, opera-beta, opera-developer, msedge, msedge-beta, msedge-dev, msedge-canary,
+                brave, brave-beta, brave-nightly\n
                 for Windows:\n
                 chrome, chrome-canary, chromium, firefox, firefox-developer, firefox-nightly,
-                opera, opera-beta, opera-developer, ms-edge, ms-edge-beta, ms-edge-dev, ms-edge-canary, ms-ie,
+                opera-stable, opera-beta, opera-developer, msedge, msedge-beta, msedge-dev, msedge-canary, msie,
                 brave, brave-beta, brave-nightly
     :return: True or False depending on the browser is installed or not.
     """
     match sys.platform:
         case OS.LINUX:
             return linux.do_i_have_installed(name)
         case OS.MAC:
             return mac.do_i_have_installed(name)
-        # case OS.WINDOWS: Windows is not yet supported.
+        case OS.WINDOWS:
+            return windows.do_i_have_installed(name)
 
 
-def give_me_details_of(name: str) -> Optional[Browser]:
+# retrieve browser details
+def give_me_details_of(name: str) -> Optional[Browser | str]:
     """
-    Retrieve browser details if the provided browser is installed in system.
+    Retrieve browser details if the provided browser is installed in system.\n
+    Browser details are: name\n
+                         description\n
+                         version\n
+                         location\n
 
     Parameters:
                 Possible browser entries / parameters\n
                 for Linux:\n
-                chrome, chromium, firefox, ms-edge, opera, opera-beta, opera-developer,
+                chrome, chromium, firefox, opera, opera-beta, opera-developer, msedge, msedge-beta, msedge-dev
                 brave, brave-beta, brave-nightly\n
                 for macOS:\n
                 chrome, chrome-canary, chromium, firefox, firefox-developer, firefox-nightly,
-                safari, opera, opera-beta, opera-developer, ms-edge, ms-edge-beta, ms-edge-dev, ms-edge-canary,
-                brave, brave-beta, brave-dev, brave-nightly\n
+                safari, opera, opera-beta, opera-developer, msedge, msedge-beta, msedge-dev, msedge-canary,
+                brave, brave-beta, brave-nightly\n
                 for Windows:\n
                 chrome, chrome-canary, chromium, firefox, firefox-developer, firefox-nightly,
-                opera, opera-beta, opera-developer, ms-edge, ms-edge-beta, ms-edge-dev, ms-edge-canary, ms-ie,
+                opera-stable, opera-beta, opera-developer, msedge, msedge-beta, msedge-dev, msedge-canary, msie,
                 brave, brave-beta, brave-nightly
     :return: Dictionary containing browser name, description, desktop version and location.
     """
     match sys.platform:
         case OS.LINUX:
             for found in (entity for entity in linux.get_details_of(name) if entity is not None):
                 return found
         case OS.MAC:
             for found in (entity for entity in mac.get_details_of(name) if entity is not None):
                 return found
-        # case OS.WINDOWS: Windows is not yet supported.
+        case OS.WINDOWS:
+            for found in windows.get_details_of(name):
+                for details in found:
+                    return details
+            return "Browser is not installed."
 
 
-def get_version_of(name: str) -> Optional[Version]:
+# retrieve browser version
+def get_version_of(name: str) -> Optional[Version | str]:
     """
     Retrieve browser version if the provided browser is installed in system.
 
     Parameters:
                 Possible browser entries / parameters\n
                 for Linux:\n
-                chrome, chromium, firefox, ms-edge, opera, opera-beta, opera-developer,
+                chrome, chromium, firefox, opera, opera-beta, opera-developer, msedge, msedge-beta, msedge-dev
                 brave, brave-beta, brave-nightly\n
                 for macOS:\n
                 chrome, chrome-canary, chromium, firefox, firefox-developer, firefox-nightly,
-                safari, opera, opera-beta, opera-developer, ms-edge, ms-edge-beta, ms-edge-dev, ms-edge-canary,
-                brave, brave-beta, brave-dev, brave-nightly\n
+                safari, opera, opera-beta, opera-developer, msedge, msedge-beta, msedge-dev, msedge-canary,
+                brave, brave-beta, brave-nightly\n
                 for Windows:\n
                 chrome, chrome-canary, chromium, firefox, firefox-developer, firefox-nightly,
-                opera, opera-beta, opera-developer, ms-edge, ms-edge-beta, ms-edge-dev, ms-edge-canary, ms-ie,
+                opera-stable, opera-beta, opera-developer, msedge, msedge-beta, msedge-dev, msedge-canary, msie,
                 brave, brave-beta, brave-nightly
     :return: Browser description and version.
     """
     match sys.platform:
         case OS.LINUX:
             for found in (entity for entity in linux.get_version_of(name) if entity is not None):
                 return found
         case OS.MAC:
             for found in (entity for entity in mac.get_version_of(name) if entity is not None):
                 return found
-        # case OS.WINDOWS: Windows is not yet supported.
-
-
-def what_is_the_default_browser():
-    """
-    Shows the default browser in system - if there is any.
-
-    :return: Default browser information.
-    """
-    match sys.platform:
-        case OS.LINUX:
-            return linux.what_is_the_default_browser()
-        # case OS.MAC: Mac is not yet supported.
-        #     return mac.what_is_the_default_browser()
-        # case OS.WINDOWS: Windows is not yet supported.
+        case OS.WINDOWS:
+            for found in windows.get_version_of(name):
+                for version in found:
+                    return version
+            return "Browser is not installed."
```

### Comparing `installed_browsers-0.1.0/installed_browsers/linux.py` & `installed_browsers-0.1.1/installed_browsers/linux.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 from typing import Iterator, Optional
 
 from xdg.DesktopEntry import DesktopEntry
 
 from .common import Browser, Version
 
 # tuple of possible browsers
-# desktop entry name may be different: "chromium_chromium.desktop" or "chromium-browser.desktop"
+# desktop entry name may be different for different architectures:
+# for example "chromium_chromium.desktop" or "chromium-browser.desktop"
 POSSIBLE_BROWSERS = (
     ("chrome", ("google-chrome",)),
     ("chromium", ("chromium", "chromium_chromium", "chromium-browser")),
     ("firefox", ("firefox", "firefox_firefox")),
-    ("ms-edge", ("microsoft-edge",)),
-    ("opera", ("opera_opera",)),
-    ("opera-beta", ("opera-beta_opera-beta",)),
-    ("opera-developer", ("opera-developer_opera-developer",)),
+    ("opera", ("opera",)),
+    ("opera-beta", ("opera-beta",)),
+    ("opera-developer", ("opera-developer",)),
+    ("msedge", ("microsoft-edge",)),
+    ("msedge-beta", ("microsoft-edge-beta",)),
+    ("msedge-dev", ("microsoft-edge-dev",)),
     ("brave", ("brave-browser", "brave_brave")),
     ("brave-beta", ("brave-browser-beta",)),
     ("brave-nightly", ("brave-browser-nightly",))
 )
 
 # tuple of browser locations
 # $XDG_DATA_HOME and $XDG_DATA_DIRS are not always set
@@ -51,14 +54,43 @@
                 if match:
                     version = match[0]
                 yield Browser(
                     name=browser, description=entry.getName(), version=version, location=executable_path
                 )
 
 
+# get default browser
+def what_is_the_default_browser() -> Optional[str]:
+    cmd = "xdg-settings get default-web-browser".split()
+    try:
+        default_browser = subprocess.check_output(cmd, stderr=subprocess.DEVNULL).decode().strip()
+    except subprocess.CalledProcessError:   # pragma: no cover
+        default_browser = "No browser is set to default."
+    if not default_browser:
+        default_browser = "No browser is set to default."
+    else:
+        default_browser = _get_browser_description(default_browser)
+    return default_browser
+
+
+# check if the given browser is installed
+def do_i_have_installed(name):
+    for browser, desktop_names in (browser_record for browser_record in POSSIBLE_BROWSERS
+                                   if browser_record[0] == name):
+        for desktop_name in desktop_names:
+            for application_dir in BROWSER_LOCATIONS:
+                path = os.path.join(application_dir, f"{desktop_name}.desktop")
+                if not os.path.isfile(path):
+                    continue
+                entry = DesktopEntry(path)
+                if entry:
+                    return True
+    return False
+
+
 # get details of a browser
 def get_details_of(name) -> Optional[Browser]:
     for browser, desktop_names in (browser_record for browser_record in POSSIBLE_BROWSERS
                                    if browser_record[0] == name):
         for desktop_name in desktop_names:
             for application_dir in BROWSER_LOCATIONS:
                 path = os.path.join(application_dir, f"{desktop_name}.desktop")
@@ -71,14 +103,15 @@
                 version = subprocess.getoutput(f"{executable_path} --version 2>&1").strip()
                 match = VERSION_PATTERN.search(version)
                 if match:
                     version = match[0]
                 yield Browser(
                     name=browser, description=entry.getName(), version=version, location=executable_path
                 )
+    yield "Browser is not installed."
 
 
 # retrieve browser version
 def get_version_of(name) -> Optional[Version]:
     for browser, desktop_names in (browser_record for browser_record in POSSIBLE_BROWSERS
                                    if browser_record[0] == name):
         for desktop_name in desktop_names:
@@ -96,30 +129,14 @@
                     version = match[0]
                 yield Version(
                     version=version
                 )
     yield "Browser is not installed."
 
 
-# check if the given browser is installed
-def do_i_have_installed(name):
-    for browser, desktop_names in (browser_record for browser_record in POSSIBLE_BROWSERS
-                                   if browser_record[0] == name):
-        for desktop_name in desktop_names:
-            for application_dir in BROWSER_LOCATIONS:
-                path = os.path.join(application_dir, f"{desktop_name}.desktop")
-                if not os.path.isfile(path):
-                    continue
-                entry = DesktopEntry(path)
-                if entry:
-                    return True
-    return False
-
-
-# get default browser
-def what_is_the_default_browser() -> Optional[str]:
-    cmd = "xdg-settings get default-web-browser".split()
-    if cmd:
-        default_browser = subprocess.check_output(cmd, stderr=subprocess.DEVNULL).decode().strip()
-    else:
-        default_browser = "No browser is set to default."
-    return default_browser
+# determine browser description
+def _get_browser_description(desktop_name):
+    for application_dir in BROWSER_LOCATIONS:
+        path = os.path.join(application_dir, desktop_name)
+        if os.path.isfile(path):
+            entry = DesktopEntry(path)
+            return entry.getName()
```

### Comparing `installed_browsers-0.1.0/pyproject.toml` & `installed_browsers-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "installed-browsers"
-version = "0.1.0"
+version = "0.1.1"
 repository = "https://github.com/undeflorate/installed_browsers"
 description = "Python library to check installed browsers"
 authors = ["undeflorate <swanslayer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
-    "Development Status :: 1 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Topic :: Internet :: WWW/HTTP :: Browsers",
-    "Topic :: Software Development :: Library :: Python Module",
+    "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3.10",
-    "programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.11",
 ]
 
 packages = [
     { include = "installed_browsers"},
 ]
 
 [tool.poetry.dependencies]
@@ -68,15 +68,15 @@
 extend-ignore = ["E203"]
 extend-exclude = """
 setup.py,
 """
 
 [tool.pytest.ini_options]
 addopts = """\
-    --cov=browsers \
+    --cov=installed_browsers \
     --cov-report=term-missing \
     --cov-report=xml \
     --cov-report=html \
     -vv \
     -x \
     -s \
 """
```

