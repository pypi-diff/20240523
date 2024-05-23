# Comparing `tmp/htmltools-0.5.0.tar.gz` & `tmp/htmltools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htmltools-0.5.0.tar", last modified: Thu Dec  7 21:59:45 2023, max compression
+gzip compressed data, was "htmltools-0.5.1.tar", last modified: Mon Dec 18 23:35:46 2023, max compression
```

## Comparing `htmltools-0.5.0.tar` & `htmltools-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:59:45.428011 htmltools-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-07 21:59:32.000000 htmltools-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-07 21:59:32.000000 htmltools-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2023-12-07 21:59:45.428011 htmltools-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-12-07 21:59:32.000000 htmltools-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:59:45.424011 htmltools-0.5.0/htmltools/
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-12-07 21:59:32.000000 htmltools-0.5.0/htmltools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53389 2023-12-07 21:59:32.000000 htmltools-0.5.0/htmltools/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2023-12-07 21:59:32.000000 htmltools-0.5.0/htmltools/_jsx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2023-12-07 21:59:32.000000 htmltools-0.5.0/htmltools/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-07 21:59:32.000000 htmltools-0.5.0/htmltools/_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:59:45.420011 htmltools-0.5.0/htmltools/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:59:45.424011 htmltools-0.5.0/htmltools/lib/react/
--rw-r--r--   0 runner    (1001) docker     (127)    11440 2023-12-07 21:59:32.000000 htmltools-0.5.0/htmltools/lib/react/react.production.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:59:45.424011 htmltools-0.5.0/htmltools/lib/react-dom/
--rw-r--r--   0 runner    (1001) docker     (127)   120585 2023-12-07 21:59:32.000000 htmltools-0.5.0/htmltools/lib/react-dom/react-dom.production.min.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 21:59:32.000000 htmltools-0.5.0/htmltools/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    44033 2023-12-07 21:59:32.000000 htmltools-0.5.0/htmltools/svg.py
--rw-r--r--   0 runner    (1001) docker     (127)    91828 2023-12-07 21:59:32.000000 htmltools-0.5.0/htmltools/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:59:45.424011 htmltools-0.5.0/htmltools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2023-12-07 21:59:45.000000 htmltools-0.5.0/htmltools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-12-07 21:59:45.000000 htmltools-0.5.0/htmltools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 21:59:45.000000 htmltools-0.5.0/htmltools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 21:59:45.000000 htmltools-0.5.0/htmltools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-07 21:59:45.000000 htmltools-0.5.0/htmltools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-07 21:59:45.000000 htmltools-0.5.0/htmltools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-12-07 21:59:32.000000 htmltools-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 21:59:45.428011 htmltools-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:59:45.424011 htmltools-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11290 2023-12-07 21:59:32.000000 htmltools-0.5.0/tests/test_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2023-12-07 21:59:32.000000 htmltools-0.5.0/tests/test_html_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2023-12-07 21:59:32.000000 htmltools-0.5.0/tests/test_jsx_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    22231 2023-12-07 21:59:32.000000 htmltools-0.5.0/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2023-12-07 21:59:32.000000 htmltools-0.5.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:35:46.551574 htmltools-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-18 23:35:32.000000 htmltools-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-18 23:35:32.000000 htmltools-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2023-12-18 23:35:46.551574 htmltools-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2023-12-18 23:35:32.000000 htmltools-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:35:46.547573 htmltools-0.5.1/htmltools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2023-12-18 23:35:32.000000 htmltools-0.5.1/htmltools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55034 2023-12-18 23:35:32.000000 htmltools-0.5.1/htmltools/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2023-12-18 23:35:32.000000 htmltools-0.5.1/htmltools/_jsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2023-12-18 23:35:32.000000 htmltools-0.5.1/htmltools/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-18 23:35:32.000000 htmltools-0.5.1/htmltools/_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:35:46.543573 htmltools-0.5.1/htmltools/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:35:46.547573 htmltools-0.5.1/htmltools/lib/react/
+-rw-r--r--   0 runner    (1001) docker     (127)    11440 2023-12-18 23:35:32.000000 htmltools-0.5.1/htmltools/lib/react/react.production.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:35:46.547573 htmltools-0.5.1/htmltools/lib/react-dom/
+-rw-r--r--   0 runner    (1001) docker     (127)   120585 2023-12-18 23:35:32.000000 htmltools-0.5.1/htmltools/lib/react-dom/react-dom.production.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 23:35:32.000000 htmltools-0.5.1/htmltools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    44033 2023-12-18 23:35:32.000000 htmltools-0.5.1/htmltools/svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91828 2023-12-18 23:35:32.000000 htmltools-0.5.1/htmltools/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:35:46.547573 htmltools-0.5.1/htmltools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2023-12-18 23:35:46.000000 htmltools-0.5.1/htmltools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-18 23:35:46.000000 htmltools-0.5.1/htmltools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 23:35:46.000000 htmltools-0.5.1/htmltools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 23:35:46.000000 htmltools-0.5.1/htmltools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-18 23:35:46.000000 htmltools-0.5.1/htmltools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-18 23:35:46.000000 htmltools-0.5.1/htmltools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-12-18 23:35:32.000000 htmltools-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 23:35:46.551574 htmltools-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 23:35:46.547573 htmltools-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11290 2023-12-18 23:35:32.000000 htmltools-0.5.1/tests/test_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2023-12-18 23:35:32.000000 htmltools-0.5.1/tests/test_html_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2023-12-18 23:35:32.000000 htmltools-0.5.1/tests/test_jsx_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22231 2023-12-18 23:35:32.000000 htmltools-0.5.1/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-12-18 23:35:32.000000 htmltools-0.5.1/tests/test_tags_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2023-12-18 23:35:32.000000 htmltools-0.5.1/tests/test_util.py
```

### Comparing `htmltools-0.5.0/LICENSE` & `htmltools-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `htmltools-0.5.0/PKG-INFO` & `htmltools-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htmltools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tools for HTML generation and output.
 Author-email: Carson Sievert <carson@rstudio.com>
 License: MIT License
         
         Copyright (c) 2023 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `htmltools-0.5.0/htmltools/__init__.py` & `htmltools-0.5.1/htmltools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 from . import svg, tags
 from ._core import TagAttrArg  # pyright: ignore[reportUnusedImport]  # noqa: F401
 from ._core import TagChildArg  # pyright: ignore[reportUnusedImport]  # noqa: F401
 from ._core import (
     HTML,
     HTMLDependency,
@@ -15,14 +15,15 @@
     TagAttrValue,
     TagChild,
     TagFunction,
     Tagifiable,
     TagList,
     TagNode,
     head_content,
+    wrap_displayhook_handler,
 )
 from ._util import css, html_escape
 from .tags import (
     a,
     br,
     code,
     div,
@@ -55,14 +56,15 @@
     "TagAttrValue",
     "TagChild",
     "TagFunction",
     "Tagifiable",
     "TagList",
     "TagNode",
     "head_content",
+    "wrap_displayhook_handler",
     "css",
     "html_escape",
     "a",
     "br",
     "code",
     "div",
     "em",
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_wbd3liae_/tmpg87q1w8m_TarContainer/0/6.py", line 89, column 0: CDATA terminal not found*

```diff
@@ -1,15 +1,16 @@
-__version__ = "0.5.0" from . import svg, tags from ._core import TagAttrArg #
+__version__ = "0.5.1" from . import svg, tags from ._core import TagAttrArg #
 pyright: ignore[reportUnusedImport] # noqa: F401 from ._core import TagChildArg
 # pyright: ignore[reportUnusedImport] # noqa: F401 from ._core import ( HTML,
 HTMLDependency, HTMLDocument, HTMLTextDocument, MetadataNode, RenderedHTML,
 Tag, TagAttrs, TagAttrValue, TagChild, TagFunction, Tagifiable, TagList,
-TagNode, head_content, ) from ._util import css, html_escape from .tags import
-( a, br, code, div, em, h1, h2, h3, h4, h5, h6, hr, img, p, pre, span, strong,
-) __all__ = ( "svg", "tags", "HTML", "HTMLDependency", "HTMLDocument",
-"HTMLTextDocument", "MetadataNode", "RenderedHTML", "Tag", "TagAttrs",
-"TagAttrValue", "TagChild", "TagFunction", "Tagifiable", "TagList", "TagNode",
-"head_content", "css", "html_escape", "a", "br", "code", "div", "em", "h1",
-"h2", "h3", "h4", "h5", "h6", "hr", "img", "p", "pre", "span", "strong", )
-import typing as _typing # Setting this will control how HTML dependencies are
-rendered. Normally they are not # visible, but if set to "json", they will be
-serialized as JSON in a
+TagNode, head_content, wrap_displayhook_handler, ) from ._util import css,
+html_escape from .tags import ( a, br, code, div, em, h1, h2, h3, h4, h5, h6,
+hr, img, p, pre, span, strong, ) __all__ = ( "svg", "tags", "HTML",
+"HTMLDependency", "HTMLDocument", "HTMLTextDocument", "MetadataNode",
+"RenderedHTML", "Tag", "TagAttrs", "TagAttrValue", "TagChild", "TagFunction",
+"Tagifiable", "TagList", "TagNode", "head_content", "wrap_displayhook_handler",
+"css", "html_escape", "a", "br", "code", "div", "em", "h1", "h2", "h3", "h4",
+"h5", "h6", "hr", "img", "p", "pre", "span", "strong", ) import typing as
+_typing # Setting this will control how HTML dependencies are rendered.
+Normally they are not # visible, but if set to "json", they will be serialized
+as JSON in a
```

### Comparing `htmltools-0.5.0/htmltools/_core.py` & `htmltools-0.5.1/htmltools/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import tempfile
 import urllib.parse
 import webbrowser
 from copy import copy, deepcopy
 from pathlib import Path
 from typing import (
     Any,
+    Callable,
     Dict,
     Iterable,
     List,
     Mapping,
     Optional,
     Sequence,
     TypeVar,
@@ -58,14 +59,15 @@
     "TagAttrs",
     "TagAttrValue",
     "TagChild",
     "TagNode",
     "TagFunction",
     "Tagifiable",
     "head_content",
+    "wrap_displayhook_handler",
 )
 
 
 class RenderedHTML(TypedDict):
     dependencies: list["HTMLDependency"]
     html: str
 
@@ -557,23 +559,42 @@
 
         attrs = [x for x in args if isinstance(x, dict)]
         self.attrs = TagAttrDict(*attrs, **kwargs)
 
         kids = [x for x in args if not isinstance(x, dict)]
         self.children = TagList(*kids)
 
+        self.prev_displayhook: Callable[[object], None] | None = None
+
     def __copy__(self: TagT) -> TagT:
         cls = self.__class__
         cp = cls.__new__(cls)
         # Any instance fields (like .children, and _attrs for the tag subclass) are
         # shallow-copied.
         new_dict = {key: copy(value) for key, value in self.__dict__.items()}
         cp.__dict__.update(new_dict)
         return cp
 
+    def __enter__(self) -> None:
+        if self.prev_displayhook is not None:
+            raise RuntimeError(
+                "Attempted to enter a Tag object's context manager, but it has already been entered."
+            )
+        self.prev_displayhook = sys.displayhook
+        sys.displayhook = wrap_displayhook_handler(
+            # self.append takes a TagChild, but the wrapper expects a function that
+            # takes a object.
+            self.append  # pyright: ignore[reportGeneralTypeIssues]
+        )
+
+    def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
+        # If we got here, then self.prev_displayhook must be not None.
+        sys.displayhook = cast(Callable[[object], None], self.prev_displayhook)
+        sys.displayhook(self)
+
     def insert(self, index: SupportsIndex, x: TagChild) -> None:
         """
         Insert tag children before a given index.
         """
 
         self.children.insert(index, x)
 
@@ -872,14 +893,36 @@
             for x in rendered["dependencies"]
         ]
         res += "\n".join(dep_html)
 
     return str(res)
 
 
+def wrap_displayhook_handler(
+    handler: Callable[[object], None]
+) -> Callable[[object], None]:
+    """
+    Wrap a displayhook function to handle different types of input objects
+
+    This function takes a function ``handler`` that would be used as a displayhook, and
+    returns a function which filters/transforms the input object depending on its type,
+    before passing it to ``handler()``.
+    """
+
+    def handler_wrapper(value: object) -> None:
+        if isinstance(value, (Tag, TagList, Tagifiable)):
+            handler(value)
+        elif hasattr(value, "_repr_html_"):
+            handler(HTML(value._repr_html_()))  # pyright: ignore
+        elif value not in (None, ...):
+            handler(value)
+
+    return handler_wrapper
+
+
 # =============================================================================
 # HTMLDocument class
 # =============================================================================
 class HTMLDocument:
     """
     Create an HTML document from Tag objects.
```

### Comparing `htmltools-0.5.0/htmltools/_jsx.py` & `htmltools-0.5.1/htmltools/_jsx.py`

 * *Files identical despite different names*

### Comparing `htmltools-0.5.0/htmltools/_util.py` & `htmltools-0.5.1/htmltools/_util.py`

 * *Files identical despite different names*

### Comparing `htmltools-0.5.0/htmltools/lib/react/react.production.min.js` & `htmltools-0.5.1/htmltools/lib/react/react.production.min.js`

 * *Files identical despite different names*

### Comparing `htmltools-0.5.0/htmltools/lib/react-dom/react-dom.production.min.js` & `htmltools-0.5.1/htmltools/lib/react-dom/react-dom.production.min.js`

 * *Files identical despite different names*

### Comparing `htmltools-0.5.0/htmltools/svg.py` & `htmltools-0.5.1/htmltools/svg.py`

 * *Files identical despite different names*

### Comparing `htmltools-0.5.0/htmltools/tags.py` & `htmltools-0.5.1/htmltools/tags.py`

 * *Files identical despite different names*

### Comparing `htmltools-0.5.0/htmltools.egg-info/PKG-INFO` & `htmltools-0.5.1/htmltools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htmltools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tools for HTML generation and output.
 Author-email: Carson Sievert <carson@rstudio.com>
 License: MIT License
         
         Copyright (c) 2023 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `htmltools-0.5.0/htmltools.egg-info/SOURCES.txt` & `htmltools-0.5.1/htmltools.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 htmltools.egg-info/top_level.txt
 htmltools/lib/react/react.production.min.js
 htmltools/lib/react-dom/react-dom.production.min.js
 tests/test_deps.py
 tests/test_html_document.py
 tests/test_jsx_tags.py
 tests/test_tags.py
+tests/test_tags_context.py
 tests/test_util.py
```

### Comparing `htmltools-0.5.0/pyproject.toml` & `htmltools-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `htmltools-0.5.0/tests/test_deps.py` & `htmltools-0.5.1/tests/test_deps.py`

 * *Files identical despite different names*

### Comparing `htmltools-0.5.0/tests/test_html_document.py` & `htmltools-0.5.1/tests/test_html_document.py`

 * *Files identical despite different names*

### Comparing `htmltools-0.5.0/tests/test_jsx_tags.py` & `htmltools-0.5.1/tests/test_jsx_tags.py`

 * *Files identical despite different names*

### Comparing `htmltools-0.5.0/tests/test_tags.py` & `htmltools-0.5.1/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `htmltools-0.5.0/tests/test_util.py` & `htmltools-0.5.1/tests/test_util.py`

 * *Files identical despite different names*

