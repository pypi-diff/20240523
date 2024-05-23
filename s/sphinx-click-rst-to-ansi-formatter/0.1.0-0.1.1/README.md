# Comparing `tmp/sphinx_click_rst_to_ansi_formatter-0.1.0.tar.gz` & `tmp/sphinx_click_rst_to_ansi_formatter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_click_rst_to_ansi_formatter-0.1.0.tar", max compression
+gzip compressed data, was "sphinx_click_rst_to_ansi_formatter-0.1.1.tar", max compression
```

## Comparing `sphinx_click_rst_to_ansi_formatter-0.1.0.tar` & `sphinx_click_rst_to_ansi_formatter-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-03-12 19:23:59.018894 sphinx_click_rst_to_ansi_formatter-0.1.0/LICENSE
--rw-r--r--   0        0        0      381 2024-03-22 21:23:43.545981 sphinx_click_rst_to_ansi_formatter-0.1.0/README.md
--rw-r--r--   0        0        0     1351 2024-03-23 14:16:25.290289 sphinx_click_rst_to_ansi_formatter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      387 2024-03-24 18:29:46.198835 sphinx_click_rst_to_ansi_formatter-0.1.0/src/sphinx_click/rst_to_ansi_formatter/__init__.py
--rw-r--r--   0        0        0      924 2024-03-17 23:44:59.578898 sphinx_click_rst_to_ansi_formatter-0.1.0/src/sphinx_click/rst_to_ansi_formatter/colors.py
--rw-r--r--   0        0        0    16373 2024-03-25 21:04:20.955187 sphinx_click_rst_to_ansi_formatter-0.1.0/src/sphinx_click/rst_to_ansi_formatter/formatter.py
--rw-r--r--   0        0        0        0 2024-03-17 21:09:46.440382 sphinx_click_rst_to_ansi_formatter-0.1.0/src/sphinx_click/rst_to_ansi_formatter/py.typed
--rw-r--r--   0        0        0       62 2024-03-17 23:19:03.684209 sphinx_click_rst_to_ansi_formatter-0.1.0/src/sphinx_click/rst_to_ansi_formatter/types.py
--rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 sphinx_click_rst_to_ansi_formatter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-03-12 19:23:59.018894 sphinx_click_rst_to_ansi_formatter-0.1.1/LICENSE
+-rw-r--r--   0        0        0      381 2024-03-22 21:23:43.545981 sphinx_click_rst_to_ansi_formatter-0.1.1/README.md
+-rw-r--r--   0        0        0     1351 2024-05-23 10:21:15.412597 sphinx_click_rst_to_ansi_formatter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      387 2024-03-24 18:29:46.198835 sphinx_click_rst_to_ansi_formatter-0.1.1/src/sphinx_click/rst_to_ansi_formatter/__init__.py
+-rw-r--r--   0        0        0      924 2024-03-17 23:44:59.578898 sphinx_click_rst_to_ansi_formatter-0.1.1/src/sphinx_click/rst_to_ansi_formatter/colors.py
+-rw-r--r--   0        0        0    16799 2024-05-22 18:53:47.404067 sphinx_click_rst_to_ansi_formatter-0.1.1/src/sphinx_click/rst_to_ansi_formatter/formatter.py
+-rw-r--r--   0        0        0        0 2024-03-17 21:09:46.440382 sphinx_click_rst_to_ansi_formatter-0.1.1/src/sphinx_click/rst_to_ansi_formatter/py.typed
+-rw-r--r--   0        0        0       62 2024-03-17 23:19:03.684209 sphinx_click_rst_to_ansi_formatter-0.1.1/src/sphinx_click/rst_to_ansi_formatter/types.py
+-rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 sphinx_click_rst_to_ansi_formatter-0.1.1/PKG-INFO
```

### Comparing `sphinx_click_rst_to_ansi_formatter-0.1.0/LICENSE` & `sphinx_click_rst_to_ansi_formatter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_click_rst_to_ansi_formatter-0.1.0/pyproject.toml` & `sphinx_click_rst_to_ansi_formatter-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx-click-rst-to-ansi-formatter"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Håkon Hægland <hakon.hagland@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sphinx_click", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sphinx_click_rst_to_ansi_formatter-0.1.0/src/sphinx_click/rst_to_ansi_formatter/colors.py` & `sphinx_click_rst_to_ansi_formatter-0.1.1/src/sphinx_click/rst_to_ansi_formatter/colors.py`

 * *Files identical despite different names*

### Comparing `sphinx_click_rst_to_ansi_formatter-0.1.0/src/sphinx_click/rst_to_ansi_formatter/formatter.py` & `sphinx_click_rst_to_ansi_formatter-0.1.1/src/sphinx_click/rst_to_ansi_formatter/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,24 @@
         if self.urls:
             self.parts.append(
                 "\n\n" + self.color_heading("Referenced URLs:") + "\n\n\b\n"
             )
             for index, url in enumerate(self.urls, start=1):
                 self.parts.append(self.color_url(f"{index}.") + f" {url}\n")
 
+    def process_url(self, url: str) -> str:
+        if url not in self.urls:
+            self.urls.append(url)
+            idx = len(self.urls)
+        else:
+            idx = self.urls.index(url)
+        # Replace the URL with a placeholder
+        replacement_txt = f"[{idx}]"
+        return replacement_txt
+
     def visit_bullet_list(self, node: docutils.nodes.bullet_list) -> None:
         # Prepend with backspace and a newline to ensure the list is not rewrapped by Click
         # and to maintain the desired spacing. See comment for visit_literal_block() for
         # more information.
         self.in_bullet_list = True
         self.parts.append("\n\n\b\n")
         pass
@@ -113,21 +123,16 @@
     def visit_emphasis(self, node: docutils.nodes.emphasis) -> None:
         # This method is called for each emphasis node in the document. That is, for
         # text in asterisks or underscores (e.g. *text* or _text_).
         txt = node.astext()
         # check if the emphasis is a URL
         if txt.startswith("http://") or txt.startswith("https://"):
             # Check if the URL is already in the list
-            if txt not in self.urls:
-                self.urls.append(txt)
-                idx = len(self.urls)
-            else:
-                idx = self.urls.index(txt)
-            # Replace the URL with a placeholder
-            txt = f"[{idx}]"
+            replacement_idx = self.process_url(txt)
+            txt = replacement_idx
         # Prepend and append the emphasis with ANSI color codes
         self.current_buffer.append(self.color_code(txt))
         # Skip further processing of children by docutils since we've manually
         #  processed the text
         raise docutils.nodes.SkipNode
 
     def visit_list_item(self, node: docutils.nodes.list_item) -> None:
@@ -162,15 +167,20 @@
         # - Internal references:
         txt = node.astext()
         if txt.startswith("http://") or txt.startswith("https://"):
             # No special colors for URLs yet
             self.current_buffer.append(txt)
         else:
             # No special colors for internal references yet
-            self.current_buffer.append(txt)  # pragma: no cover
+            if "refuri" in node:
+                replacement_idx = self.process_url(node["refuri"])
+                self.current_buffer.append(f'"{txt}"')  # pragma: no cover
+                self.current_buffer.append(f" {self.color_code(replacement_idx)}")
+            else:
+                self.current_buffer.append(txt)  # pragma: no cover
         raise docutils.nodes.SkipNode
 
     def visit_Text(self, node: docutils.nodes.Text) -> None:
         txt = node.astext()
         if self.in_literal:
             # Wrap the text in ANSI codes for bright cyan
             self.current_buffer.append(self.color_code(txt))
```

### Comparing `sphinx_click_rst_to_ansi_formatter-0.1.0/PKG-INFO` & `sphinx_click_rst_to_ansi_formatter-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-click-rst-to-ansi-formatter
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Håkon Hægland
 Author-email: hakon.hagland@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

