# Comparing `tmp/acdh-tei-pyutils-1.2.tar.gz` & `tmp/acdh-tei-pyutils-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acdh-tei-pyutils-1.2.tar", last modified: Fri May 17 13:15:59 2024, max compression
+gzip compressed data, was "acdh-tei-pyutils-1.3.tar", last modified: Thu May 23 10:49:55 2024, max compression
```

## Comparing `acdh-tei-pyutils-1.2.tar` & `acdh-tei-pyutils-1.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:15:59.094220 acdh-tei-pyutils-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-17 13:15:59.094220 acdh-tei-pyutils-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:15:59.090220 acdh-tei-pyutils-1.2/acdh_tei_pyutils/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16811 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:15:59.094220 acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/clean_markup.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei_no_id.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei_no_ids.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei_trailing_slash.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/tei.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:15:59.094220 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-17 13:15:58.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 13:15:59.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:15:58.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-17 13:15:58.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:15:58.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-17 13:15:58.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 13:15:58.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 13:15:59.094220 acdh-tei-pyutils-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:15:59.094220 acdh-tei-pyutils-1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/tests/test_tei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:49:55.127192 acdh-tei-pyutils-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-23 10:49:55.127192 acdh-tei-pyutils-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:49:55.123192 acdh-tei-pyutils-1.3/acdh_tei_pyutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17020 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:49:55.127192 acdh-tei-pyutils-1.3/acdh_tei_pyutils/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils/files/clean_markup.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils/files/tei.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils/files/tei_no_id.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils/files/tei_no_ids.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils/files/tei_trailing_slash.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils/tei.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:49:55.123192 acdh-tei-pyutils-1.3/acdh_tei_pyutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-23 10:49:55.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-23 10:49:55.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:49:55.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-23 10:49:55.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:49:55.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-23 10:49:55.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 10:49:55.000000 acdh-tei-pyutils-1.3/acdh_tei_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 10:49:55.127192 acdh-tei-pyutils-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:49:55.127192 acdh-tei-pyutils-1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-05-23 10:49:37.000000 acdh-tei-pyutils-1.3/tests/test_tei.py
```

### Comparing `acdh-tei-pyutils-1.2/LICENSE` & `acdh-tei-pyutils-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.2/PKG-INFO` & `acdh-tei-pyutils-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acdh-tei-pyutils
-Version: 1.2
+Version: 1.3
 Summary: Utilty functions to work with TEI Documents
 Home-page: https://github.com/acdh-oeaw/acdh-tei-pyutils
 Author: Peter Andorfer, Daniel Stoxreiter
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT
 Keywords: acdh-tei-pyutils
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `acdh-tei-pyutils-1.2/README.md` & `acdh-tei-pyutils-1.3/README.md`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.2/acdh_tei_pyutils/cli.py` & `acdh-tei-pyutils-1.3/acdh_tei_pyutils/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,30 +139,37 @@
         doc_uri = f"{doc_base}/{doc_id}"
         doc_title = doc.any_xpath(title_xpath)[0]
         refs = doc.any_xpath(mention_xpath)
         for ref in set(refs):
             if ref.startswith("#"):
                 ref = ref[1:]
             ref_doc_dict[ref].append(
-                {"doc_uri": doc_uri, "doc_path": x, "doc_title": doc_title}
+                {
+                    "doc_uri": doc_uri,
+                    "doc_path": x,
+                    "doc_title": doc_title,
+                    "doc_id": doc_id,
+                    "doc_date": None,
+                    "doc_title_sec": None
+                }
             )
             doc_ref_dict[filename].append(ref)
     click.echo(
         click.style(
             f"collected {len(ref_doc_dict.keys())} of mentioned entities from {len(files)} docs",
             fg="green",
         )
     )
     for x in index_files:
         doc = TeiEnricher(x)
         ent_nodes = doc.any_xpath(".//tei:body//*[@xml:id]")
         for ent in ent_nodes:
-            ent_id = ent.xpath("@xml:id")[0]
-            mention = ref_doc_dict[ent_id]
-            event_list = doc.create_mention_list(mention, event_title=event_title)
+            ent_id = ent.xpath("@xml:id", namespaces=doc.nsmap)[0]
+            mentions = ref_doc_dict[ent_id]
+            event_list = doc.create_mention_list(mentions, event_title)
             try:
                 list(event_list[0])
                 ent.append(event_list)
             except IndexError:
                 pass
         doc.tree_to_file(file=x)
```

### Comparing `acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/clean_markup.xsl` & `acdh-tei-pyutils-1.3/acdh_tei_pyutils/files/clean_markup.xsl`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei.xml` & `acdh-tei-pyutils-1.3/acdh_tei_pyutils/files/tei.xml`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei_no_id.xml` & `acdh-tei-pyutils-1.3/acdh_tei_pyutils/files/tei_no_id.xml`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei_no_ids.xml` & `acdh-tei-pyutils-1.3/acdh_tei_pyutils/files/tei_no_ids.xml`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei_trailing_slash.xml` & `acdh-tei-pyutils-1.3/acdh_tei_pyutils/files/tei_trailing_slash.xml`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.2/acdh_tei_pyutils/tei.py` & `acdh-tei-pyutils-1.3/acdh_tei_pyutils/tei.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             idno_node = ET.Element(f"{{{tei_ns}}}idno")
             idno_node.set("type", "handle")
             idno_node.text = handle
             insert_node = self.any_xpath(insert_xpath)[0]
             insert_node.append(idno_node)
             return idno_node
 
-    def create_mention_list(self, mentions):
+    def create_mention_list(self, mentions, event_title=""):
         """creates a tei element with notes of mentions
 
         :param mentions: a list of dicts with keys `doc_id` and `doc_title`
         :type mentions: noteGrp
 
         :return: a etree.element
         """
@@ -262,13 +262,13 @@
             except KeyError:
                 note = ET.Element(f"{{{tei_ns}}}note")
                 note.attrib['target'] = x['doc_id']
                 note.attrib['type'] = "mentions"
                 if x['doc_date'] is not None:
                     note.attrib['corresp'] = x['doc_date']
                 if x['doc_title_sec'] is not None:
-                    note.text = f"{x['doc_title']} {x['doc_title_sec']}"
+                    note.text = event_title + f"{x['doc_title']} {x['doc_title_sec']}"
                 else:
                     note.text = x['doc_title']
                 node_root.append(note)
                 mentions_added[slugify(x['doc_id'])] = True
         return node_root
```

### Comparing `acdh-tei-pyutils-1.2/acdh_tei_pyutils/utils.py` & `acdh-tei-pyutils-1.3/acdh_tei_pyutils/utils.py`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/PKG-INFO` & `acdh-tei-pyutils-1.3/acdh_tei_pyutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acdh-tei-pyutils
-Version: 1.2
+Version: 1.3
 Summary: Utilty functions to work with TEI Documents
 Home-page: https://github.com/acdh-oeaw/acdh-tei-pyutils
 Author: Peter Andorfer, Daniel Stoxreiter
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT
 Keywords: acdh-tei-pyutils
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/SOURCES.txt` & `acdh-tei-pyutils-1.3/acdh_tei_pyutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 acdh_tei_pyutils.egg-info/top_level.txt
 acdh_tei_pyutils/files/clean_markup.xsl
 acdh_tei_pyutils/files/tei.xml
 acdh_tei_pyutils/files/tei_no_id.xml
 acdh_tei_pyutils/files/tei_no_ids.xml
 acdh_tei_pyutils/files/tei_trailing_slash.xml
 tests/__init__.py
+tests/test_cli.py
 tests/test_tei.py
```

### Comparing `acdh-tei-pyutils-1.2/setup.py` & `acdh-tei-pyutils-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,10 +66,10 @@
     package_data={
         module.__name__: walker(os.path.dirname(module.__file__), "files"),
     },
     setup_requires=dev_requirements,
     test_suite="tests",
     tests_require=dev_requirements,
     url="https://github.com/acdh-oeaw/acdh-tei-pyutils",
-    version="v1.2",
+    version="v1.3",
     zip_safe=False,
 )
```

### Comparing `acdh-tei-pyutils-1.2/tests/test_tei.py` & `acdh-tei-pyutils-1.3/tests/test_tei.py`

 * *Files identical despite different names*

