# Comparing `tmp/fitz_utils-0.0.17.tar.gz` & `tmp/fitz_utils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitz_utils-0.0.17.tar", max compression
+gzip compressed data, was "fitz_utils-0.1.0.tar", max compression
```

## Comparing `fitz_utils-0.0.17.tar` & `fitz_utils-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      131 2024-05-17 02:55:06.955851 fitz_utils-0.0.17/fitz_utils/__init__.py
--rw-r--r--   0        0        0     1252 2024-05-17 02:55:06.955851 fitz_utils-0.0.17/fitz_utils/processed_doc.py
--rw-r--r--   0        0        0    15172 2024-05-17 02:55:06.955851 fitz_utils-0.0.17/fitz_utils/processed_page.py
--rw-r--r--   0        0        0       30 2024-05-17 02:55:06.955851 fitz_utils-0.0.17/LICENSE
--rw-r--r--   0        0        0      511 2024-05-17 02:56:20.336367 fitz_utils-0.0.17/pyproject.toml
--rw-r--r--   0        0        0      364 2024-05-17 02:55:06.955851 fitz_utils-0.0.17/README.md
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 fitz_utils-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0      131 2024-05-17 02:55:06.955851 fitz_utils-0.1.0/fitz_utils/__init__.py
+-rw-r--r--   0        0        0     1252 2024-05-17 02:55:06.955851 fitz_utils-0.1.0/fitz_utils/processed_doc.py
+-rw-r--r--   0        0        0    15651 2024-05-23 09:30:07.211198 fitz_utils-0.1.0/fitz_utils/processed_page.py
+-rw-r--r--   0        0        0       30 2024-05-17 02:55:06.955851 fitz_utils-0.1.0/LICENSE
+-rw-r--r--   0        0        0      622 2024-05-23 09:30:38.530596 fitz_utils-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      364 2024-05-17 02:55:06.955851 fitz_utils-0.1.0/README.md
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 fitz_utils-0.1.0/PKG-INFO
```

### Comparing `fitz_utils-0.0.17/fitz_utils/processed_doc.py` & `fitz_utils-0.1.0/fitz_utils/processed_doc.py`

 * *Files identical despite different names*

### Comparing `fitz_utils-0.0.17/fitz_utils/processed_page.py` & `fitz_utils-0.1.0/fitz_utils/processed_page.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,20 +44,23 @@
             pd.DataFrame: Columns - ["x0", "y0", "x1", "y1", "text", "fixed_text", "rect"]
         """
         # Block data format: (x0, y0, x1, y1, "lines in the block", block_no, #
         # block_type) #
         blocks: list = self.page.get_text("blocks")
         cols = ["x0", "y0", "x1", "y1", "text", "fixed_text", "rect"]
 
+        rotation_matrix = self.page.rotation_matrix
         block_data = []
         for block in blocks:
+            block = list(block)
             # If block type is image, continue #
             if block[-1] == 1:
                 continue
-            rect = fitz.Rect(block[:4])
+            rect = fitz.Rect(block[:4]).transform(rotation_matrix)
+            block[:4] = list(rect.round())
             block = list(block[:5]) + [rect]
             block.insert(5, ftfy.fix_text(block[4]))
             block_data.append(block)
 
         block_df = pd.DataFrame(block_data, columns=cols)
         float_dtypes = block_df.select_dtypes("float64")
         block_df[float_dtypes.columns] = float_dtypes.astype("int")
@@ -80,26 +83,27 @@
             "text",
             "fixed_text",
             "block_no",
             "line_no",
             "rect",
         ]
 
+        rotation_matrix = self.page.rotation_matrix
         data = []
         for block_num, block in enumerate(blocks):
             if "image" in block.keys():
                 continue
 
             for line_num, line in enumerate(block["lines"]):
                 span_text = list()
 
-                line_bbox = [int(loc) for loc in list(line["bbox"])]
-                line_rect = fitz.Rect(line["bbox"])
+                line_rect = fitz.Rect(line["bbox"]).transform(rotation_matrix)
+                line_bbox = list(line_rect.round())
 
-                for span_num, span in enumerate(line["spans"]):
+                for _, span in enumerate(line["spans"]):
                     rect = fitz.Rect(span["bbox"])
                     if rect not in self.page.rect or set(span["text"]) == {" "}:
                         continue
                     span_text.append(span["text"])
 
                 line_text = " ".join(span_text)
                 fixed_line_text = ftfy.fix_text(line_text)
@@ -127,25 +131,27 @@
             pd.DataFrame: Columns - ["x0", "y0", "x1", "y1", "text", "fixed_text", "size",
             "flags","color", "font", "block_num", "line_num", "span_num", "rect"]
         """
         blocks = self.page.get_text("dict")["blocks"]
         cols = ["x0", "y0", "x1", "y1", "text", "fixed_text", "size", "flags"]
         cols += ["color", "font", "block_num", "line_num", "span_num", "rect"]
 
+        rotation_matrix = self.page.rotation_matrix
         data = []
         for block_num, block in enumerate(blocks):
             if "image" in block.keys():
                 continue
             for line_num, line in enumerate(block["lines"]):
                 for span_num, span in enumerate(line["spans"]):
                     rect = fitz.Rect(span["bbox"])
                     if rect not in self.page.rect or set(span["text"]) == {" "}:
                         continue
 
-                    span_data = list(span["bbox"])
+                    rect = rect.transform(rotation_matrix)
+                    span_data = list(rect.round())
                     span_data.append(span["text"])
                     span_data.append(ftfy.fix_text(span["text"]))
                     span_data.append(span["size"])
                     span_data.append(span["flags"])
                     span_data.append(fitz.sRGB_to_pdf(span["color"]))
                     span_data.append(span["font"])
                     span_data += [block_num, line_num, span_num, rect]
@@ -174,28 +180,31 @@
             "fixed_text",
             "block_no",
             "line_no",
             "word_no",
         ]
         cols += ["rect"]
 
+        rotation_matrix = self.page.rotation_matrix
         word_data = []
         for word in words:
-            rect = fitz.Rect(word[:4])
+            word = list(word)
+            rect = fitz.Rect(word[:4]).transform(rotation_matrix)
+            word[:4] = list(rect.round())
             word = list(word) + [rect]
             word.insert(5, ftfy.fix_text(word[4]))
             word_data.append(word)
 
         word_df = pd.DataFrame(word_data, columns=cols)
         float_dtypes = word_df.select_dtypes("float64")
         word_df[float_dtypes.columns] = float_dtypes.astype("int")
         return word_df
 
     def get_opencv_img(
-        self, scale: fitz.Matrix = fitz.Matrix(1, 1), dpi: int or None = None
+        self, scale: fitz.Matrix = fitz.Matrix(1, 1), dpi: int | None = None
     ) -> np.ndarray:
         """Get opencv image from page
 
         Args:
             scale (fitz.Matrix): scaling matrix for generating pixmap
             dpi: dots per inch which can be used in place of Matrix
```

### Comparing `fitz_utils-0.0.17/PKG-INFO` & `fitz_utils-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitz-utils
-Version: 0.0.17
+Version: 0.1.0
 Summary: Extra functions for use with pymupdf module
 Author: The Walnut AI
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

