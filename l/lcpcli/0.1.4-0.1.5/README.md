# Comparing `tmp/lcpcli-0.1.4.tar.gz` & `tmp/lcpcli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri May 17 15:31:23 2024, max compression
+gzip compressed data, last modified: Thu May 23 14:14:49 2024, max compression
```

## Comparing `lcpcli-0.1.4.tar` & `lcpcli-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       64 2024-05-17 15:31:05.345346 lcpcli-0.1.4/lcpcli/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      161 2024-05-14 08:47:56.898196 lcpcli-0.1.4/lcpcli/__main__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     3204 2024-05-17 13:57:47.026392 lcpcli-0.1.4/lcpcli/cli.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    18686 2024-05-17 08:35:50.371521 lcpcli-0.1.4/lcpcli/corpert.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    14826 2024-05-17 13:58:07.910331 lcpcli-0.1.4/lcpcli/lcp_upload.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2379 2024-05-14 08:47:56.898196 lcpcli-0.1.4/lcpcli/lcpcli.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    16619 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/utils.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    13554 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/data/lcp_corpus_template.json
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2453 2024-05-02 11:39:20.926734 lcpcli-0.1.4/lcpcli/data/input/in.conllu
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      669 2024-05-02 11:39:20.926734 lcpcli-0.1.4/lcpcli/data/input/in.vert
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)   581704 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/data/input/in_tei_spoken.xml
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        0 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/parsers/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    32245 2024-05-17 08:20:09.846874 lcpcli-0.1.4/lcpcli/parsers/_parser.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    14009 2024-05-17 08:20:14.054914 lcpcli-0.1.4/lcpcli/parsers/conllu.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      370 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/parsers/json.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10547 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/parsers/tei.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5885 2024-05-02 11:39:20.930734 lcpcli-0.1.4/lcpcli/parsers/vert.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       81 2023-12-06 14:33:04.945962 lcpcli-0.1.4/.gitignore
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1058 2023-12-13 14:52:19.083400 lcpcli-0.1.4/LICENSE.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    14025 2024-05-17 15:26:55.848466 lcpcli-0.1.4/README.md
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2474 2024-05-02 11:39:20.930734 lcpcli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    15173 2024-05-17 15:31:23.000000 lcpcli-0.1.4/PKG-INFO
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       64 2024-05-23 14:14:44.252187 lcpcli-0.1.5/lcpcli/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      161 2024-05-14 08:47:56.898196 lcpcli-0.1.5/lcpcli/__main__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     3204 2024-05-22 11:44:07.093721 lcpcli-0.1.5/lcpcli/cli.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    18787 2024-05-22 13:26:09.265429 lcpcli-0.1.5/lcpcli/corpert.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    14826 2024-05-17 13:58:07.910331 lcpcli-0.1.5/lcpcli/lcp_upload.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2379 2024-05-14 08:47:56.898196 lcpcli-0.1.5/lcpcli/lcpcli.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    17057 2024-05-22 15:45:45.767905 lcpcli-0.1.5/lcpcli/utils.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    13554 2024-05-02 11:39:20.930734 lcpcli-0.1.5/lcpcli/data/lcp_corpus_template.json
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2453 2024-05-02 11:39:20.926734 lcpcli-0.1.5/lcpcli/data/input/in.conllu
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      669 2024-05-02 11:39:20.926734 lcpcli-0.1.5/lcpcli/data/input/in.vert
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)   581704 2024-05-02 11:39:20.930734 lcpcli-0.1.5/lcpcli/data/input/in_tei_spoken.xml
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        0 2024-05-02 11:39:20.930734 lcpcli-0.1.5/lcpcli/parsers/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    32593 2024-05-22 15:44:36.654925 lcpcli-0.1.5/lcpcli/parsers/_parser.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    14009 2024-05-22 11:42:40.765964 lcpcli-0.1.5/lcpcli/parsers/conllu.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      370 2024-05-02 11:39:20.930734 lcpcli-0.1.5/lcpcli/parsers/json.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10547 2024-05-02 11:39:20.930734 lcpcli-0.1.5/lcpcli/parsers/tei.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5885 2024-05-02 11:39:20.930734 lcpcli-0.1.5/lcpcli/parsers/vert.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       81 2023-12-06 14:33:04.945962 lcpcli-0.1.5/.gitignore
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1058 2023-12-13 14:52:19.083400 lcpcli-0.1.5/LICENSE.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    14025 2024-05-17 15:26:55.848466 lcpcli-0.1.5/README.md
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2474 2024-05-02 11:39:20.930734 lcpcli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    15173 2024-05-23 14:14:49.000000 lcpcli-0.1.5/PKG-INFO
```

### Comparing `lcpcli-0.1.4/lcpcli/cli.py` & `lcpcli-0.1.5/lcpcli/cli.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/lcpcli/corpert.py` & `lcpcli-0.1.5/lcpcli/corpert.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,14 +366,16 @@
                                 times = [
                                     float(input_cols[x]) for x in (start_idx, end_idx)
                                 ]
                                 start, end = [
                                     str(int(times[n] * 25.0) + doc_frames[n])
                                     for n in (0, 1)
                                 ]
+                                if end <= start:
+                                    end = start + 1
                                 output_cols.append(f"[{start},{end})")
                             output_file.write("\t".join(output_cols) + "\n")
 
             print(f"outfiles written to '{self._path}'.")
             json_str = json.dumps(json_obj, indent=4)
             json_path = os.path.join(self.output or ".", "meta.json")
             open(json_path, "w").write(json_str)
```

### Comparing `lcpcli-0.1.4/lcpcli/lcp_upload.py` & `lcpcli-0.1.5/lcpcli/lcp_upload.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/lcpcli/lcpcli.py` & `lcpcli-0.1.5/lcpcli/lcpcli.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/lcpcli/utils.py` & `lcpcli-0.1.5/lcpcli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,14 +317,16 @@
                 if parse_misc := re.search(Sentence._space_after, misc):
                     if parse_misc[1] == "No":
                         self.parser.cur_idx -= 1
                 if frame_range := re.search(Sentence._frame_range, misc):
                     start, end = frame_range[1].split("|")
                     start = round(25.0 * float(start))
                     end = round(25.0 * float(end.lstrip("end=")))
+                    if end <= start:
+                        end = start + 1
                     token_dict[w_id].append([start, end])
                 jsonbMisc = {}
                 for bit in misc.split("|"):
                     if "=" not in bit:
                         continue
                     key, value = bit.split("=")
                     if key in ("SpaceAfter", "start", "end"):
@@ -396,26 +398,40 @@
 class Table:
     def __init__(self, name, path, config={}):
         self.name = name
         self.path = os.path.join(path, f"{name}.csv")
         self.file = open(self.path, "a")
         self.config = config
         self.cursor = 1
-        self.currentEntity = dict()
-        self.previousEntity = None
+        self.current_entity = dict()
+        self.previous_entity = None
         self.colNames = ([],)
         self.labels = dict()
         self.texts = dict()
         self.deps = dict()
         self.anchor_right = 0
         self.non_null_attributes = {}
         self.sep = "\t"
+        self.quote = f"\b"
+        self.trigger_character = "'"
 
     def write(self, row: list):
-        self.file.write(self.sep.join([str(x) for x in row]) + "\n")
+        self.file.write(
+            self.sep.join(
+                [
+                    (
+                        f"{self.quote}{str(x)}{self.quote}"
+                        if self.trigger_character in str(x)
+                        else str(x)
+                    )
+                    for x in row
+                ]
+            )
+            + "\n"
+        )
 
 
 class Attribute:
     def __init__(self, name, value):
         self.name = name
         self._value = value
```

### Comparing `lcpcli-0.1.4/lcpcli/data/lcp_corpus_template.json` & `lcpcli-0.1.5/lcpcli/data/lcp_corpus_template.json`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/lcpcli/data/input/in.conllu` & `lcpcli-0.1.5/lcpcli/data/input/in.conllu`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/lcpcli/data/input/in.vert` & `lcpcli-0.1.5/lcpcli/data/input/in.vert`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/lcpcli/data/input/in_tei_spoken.xml` & `lcpcli-0.1.5/lcpcli/data/input/in_tei_spoken.xml`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/lcpcli/parsers/_parser.py` & `lcpcli-0.1.5/lcpcli/parsers/_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,20 +215,20 @@
                 # TODO: form will need a lookup table here too
                 # if 'form' not in entity_col_names:
                 #     entity_col_names.append('form')
                 entity_col_names.append("char_range")
                 table.write(entity_col_names)
         table = self._tables[aname_low]
         fk = attribute.value.strip()
-        ce = table.currentEntity
+        ce = table.current_entity
         if fk == ce.get("id", ""):
             # TODO: form will need a lookup table here too
             # if 'form' in ce and 'form' not in self._tables[aname_low]['col_names']:
             #     ce['form'] += token.attributes['form'].value + (' ' if token.spaceAfter else '')
-            table.previousEntity = entity
+            table.previous_entity = entity
             pass
         else:
             if ce:
                 entity_cols = [table.cursor]
                 table.cursor += 1
                 entity_cols += ce["cols"]
                 # Process labels
@@ -266,22 +266,22 @@
                         if line[0].strip() == fk:
                             ce["cols"] = line[1:]
                             # TODO: form will need a lookup table here too
                             # if 'form' not in self._tables[aname_low]['col_names']:
                             #     ce['form'] = token.attributes['form'].value + (' ' if token.spaceAfter else '')
                             ce["range_low"] = str(self.char_range_cur)
                             break
-            table.currentEntity = ce
+            table.current_entity = ce
 
     def close_aligned_entity(self, name, path, aligned_entities={}):
         dummy_entity = EntityType()
         dummy_attribute = Text(name, "dummy")
         self.aligned_entity(dummy_entity, path, dummy_attribute, aligned_entities)
         if name in self._tables:
-            self._tables[name].currentEntity = {}
+            self._tables[name].current_entity = {}
 
     def close_upload_files(self, path="./"):
         if self._tables is None:
             return
         # Write label files
         for n, tab in self._tables.items():
             tab.file.close()
@@ -426,30 +426,30 @@
 
                     if aname_low in aligned_entities and isinstance(attribute, Text):
                         self.aligned_entity(token, path, attribute, aligned_entities)
                         # if aname_low not in self._tables:
                         #     self._tables[aname_low] = {
                         #         'file': open(os.path.join(path,f"{aname_low}.csv"), "a"),
                         #         'cursor': 1,
-                        #         'currentEntity': {},
+                        #         'current_entity': {},
                         #         'previousToken': None
                         #     }
                         #     with open(aligned_entities[aname_low]['fn'], "r") as aligned_file:
                         #         ne_col_names = [f"{aname_low}_id"]
                         #         ne_col_names += aligned_file.readline().split()[1:]
                         #         self._tables[aname_low]['col_names'] = [*ne_col_names]
                         #         # TODO: form will need a lookup table here too
                         #         # if 'form' not in ne_col_names:
                         #         #     ne_col_names.append('form')
                         #         ne_col_names.append("char_range")
                         #         self._tables[aname_low]['file'].write(
                         #             "\t".join(ne_col_names) + "\n"
                         #         )
                         # fk = attribute.value.strip()
-                        # ce = self._tables[aname_low].get("currentEntity", {})
+                        # ce = self._tables[aname_low].get("current_entity", {})
                         # if fk == ce.get("id", ""):
                         #     # TODO: form will need a lookup table here too
                         #     # if 'form' in ce and 'form' not in self._tables[aname_low]['col_names']:
                         #     #     ce['form'] += token.attributes['form'].value + (' ' if token.spaceAfter else '')
                         #     self._tables[aname_low]['previousToken'] = token
                         #     pass
                         # else:
@@ -480,15 +480,15 @@
                         #                 if line[0].strip() == fk:
                         #                     ce['cols'] = line[1:]
                         #                     # TODO: form will need a lookup table here too
                         #                     # if 'form' not in self._tables[aname_low]['col_names']:
                         #                     #     ce['form'] = token.attributes['form'].value + (' ' if token.spaceAfter else '')
                         #                     ce['range_low'] = str(self.char_range_cur)
                         #                     break
-                        #     self._tables[aname_low]['currentEntity'] = ce
+                        #     self._tables[aname_low]['current_entity'] = ce
 
                     elif isinstance(attribute, Categorical):
                         cols.append(str(attribute.value))
 
                     # if isinstance(attribute, Meta):
                     #     cols.append( json.dumps(attribute.value) )
 
@@ -519,15 +519,15 @@
                         name = attribute.name
                         if name not in self._tables:
                             self._tables[name] = Table(name, path)
                             self._tables[name].write(
                                 [
                                     "head",
                                     "dependent",
-                                    "label",
+                                    "udep",
                                     "left_anchor",
                                     "right_anchor",
                                 ]
                             )
                         table = self._tables[name]
                         if str(segment.id) not in table.deps:
                             table.deps[str(segment.id)] = {}
@@ -560,14 +560,16 @@
                 cols.append(f"[{str(left_char_range)},{str(self.char_range_cur)})")
                 self.char_range_cur += 1
                 if token.frame_range:
                     has_frame_range = True  # Keep it here too for iterations where non_null_attributes is already set
                     left_frame_range, right_frame_range = token.frame_range
                     left_frame_range += offset_frame_range
                     right_frame_range += offset_frame_range
+                    if right_frame_range <= left_frame_range:
+                        right_frame_range = left_frame_range + 1
                     cols.append(f"[{str(left_frame_range)},{str(right_frame_range)})")
                     if current_document:
                         if current_document.frame_range[0] == 0:
                             current_document.frame_range[0] = (
                                 offset_frame_range + token.frame_range[0]
                             )
                         current_document.frame_range[1] = (
@@ -592,16 +594,19 @@
                     if a in aligned_entities_segment:
                         continue
                     col_names.append(a)
                 segment_table.write(col_names)
             cols = [str(segment.id)]
             cols.append(f"[{char_range_segment_start},{self.char_range_cur-1})")
             if has_frame_range:
+                frame_range_segment_end = self.frame_range_cur
+                if frame_range_segment_end <= frame_range_segment_start:
+                    frame_range_segment_end = frame_range_segment_start + 1
                 cols.append(
-                    f"[{str(frame_range_segment_start)},{str(self.frame_range_cur)})"
+                    f"[{str(frame_range_segment_start)},{str(frame_range_segment_end)})"
                 )
             # Add all segment attributes
             for a in segment.attributes.values():
                 aname_low = a.name.lower()
                 if aname_low in aligned_entities_segment:
                     self.aligned_entity(segment, path, a, aligned_entities_segment)
                 else:
```

### Comparing `lcpcli-0.1.4/lcpcli/parsers/conllu.py` & `lcpcli-0.1.5/lcpcli/parsers/conllu.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/lcpcli/parsers/tei.py` & `lcpcli-0.1.5/lcpcli/parsers/tei.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/lcpcli/parsers/vert.py` & `lcpcli-0.1.5/lcpcli/parsers/vert.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/LICENSE.txt` & `lcpcli-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/README.md` & `lcpcli-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/pyproject.toml` & `lcpcli-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.4/PKG-INFO` & `lcpcli-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lcpcli
-Version: 0.1.4
+Version: 0.1.5
 Summary: Helper for converting CONLLU files and uploading the corpus to LiRI Corpus Platform (LCP)
 Project-URL: Homepage, https://github.com/liri-uzh/lcpcli/issues
 Project-URL: Issues, https://github.com/liri-uzh/lcpcli/issues
 Author-email: Danny McDonald <daniel.mcdonald@uzh.ch>, Igor Mustač <igor.mustac@uzh.ch>, Jeremy Zehr <jeremy.zehr@uzh.ch>, Jonathan Schaber <jeremy.schaber@uzh.ch>
 License: MIT
 License-File: LICENSE.txt
 Keywords: CONLL,TEI,VERT,corpora,corpus,linguistics
```

