# Comparing `tmp/node.ext.directory-0.8.tar.gz` & `tmp/node_ext_directory-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/node.ext.directory-0.8.tar", last modified: Mon Mar 21 08:01:15 2022, max compression
+gzip compressed data, was "node_ext_directory-0.8.1.tar", last modified: Thu May 23 13:59:29 2024, max compression
```

## Comparing `node.ext.directory-0.8.tar` & `node_ext_directory-0.8.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-03-21 08:01:15.000000 node.ext.directory-0.8/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2962 2022-03-21 08:01:15.000000 node.ext.directory-0.8/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1378 2022-03-21 08:01:15.000000 node.ext.directory-0.8/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       86 2022-03-21 08:01:15.000000 node.ext.directory-0.8/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)    10834 2022-03-21 08:01:15.000000 node.ext.directory-0.8/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3068 2022-03-21 08:01:15.000000 node.ext.directory-0.8/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)      632 2022-03-21 08:01:15.000000 node.ext.directory-0.8/TODO.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2022-03-21 08:01:15.000000 node.ext.directory-0.8/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1472 2022-03-21 08:01:15.000000 node.ext.directory-0.8/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node/ext/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node/ext/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node/ext/directory/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      370 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node/ext/directory/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    10216 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node/ext/directory/directory.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      288 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node/ext/directory/events.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1639 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node/ext/directory/interfaces.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    19346 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node/ext/directory/tests.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node.ext.directory.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    10834 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node.ext.directory.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)      618 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node.ext.directory.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node.ext.directory.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       14 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node.ext.directory.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       21 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node.ext.directory.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node.ext.directory.egg-info/top_level.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-03-21 08:01:15.000000 node.ext.directory-0.8/src/node.ext.directory.egg-info/zip-safe
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:59:29.063201 node_ext_directory-0.8.1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3084 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1378 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       86 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8582 2024-05-23 13:59:29.063201 node_ext_directory-0.8.1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3262 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      632 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/TODO.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2024-05-23 13:59:29.063201 node_ext_directory-0.8.1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1474 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:59:29.059201 node_ext_directory-0.8.1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:59:29.059201 node_ext_directory-0.8.1/src/node/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/src/node/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:59:29.063201 node_ext_directory-0.8.1/src/node/ext/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/src/node/ext/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:59:29.063201 node_ext_directory-0.8.1/src/node/ext/directory/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      370 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/src/node/ext/directory/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10237 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/src/node/ext/directory/directory.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      288 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/src/node/ext/directory/events.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1639 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/src/node/ext/directory/interfaces.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    19599 2024-05-23 13:59:28.000000 node_ext_directory-0.8.1/src/node/ext/directory/tests.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:59:29.063201 node_ext_directory-0.8.1/src/node.ext.directory.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8582 2024-05-23 13:59:29.000000 node_ext_directory-0.8.1/src/node.ext.directory.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      618 2024-05-23 13:59:29.000000 node_ext_directory-0.8.1/src/node.ext.directory.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-23 13:59:29.000000 node_ext_directory-0.8.1/src/node.ext.directory.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       14 2024-05-23 13:59:29.000000 node_ext_directory-0.8.1/src/node.ext.directory.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       21 2024-05-23 13:59:29.000000 node_ext_directory-0.8.1/src/node.ext.directory.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2024-05-23 13:59:29.000000 node_ext_directory-0.8.1/src/node.ext.directory.egg-info/top_level.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-23 13:59:29.000000 node_ext_directory-0.8.1/src/node.ext.directory.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `node.ext.directory-0.8/CHANGES.rst` & `node_ext_directory-0.8.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changes
 =======
 
+0.8.1 (2024-05-23)
+------------------
+
+- Fix deprecated imports.
+  [rnix]
+
+- Add note about successor package.
+  [rnix]
+
+
 0.8 (2022-03-21)
 ----------------
 
 - Replace deprecated use of ``Nodify`` by ``MappingNode``.
   [rnix]
 
 - Replace deprecated use of ``Adopt`` by ``MappingAdopt``.
```

### Comparing `node.ext.directory-0.8/LICENSE.rst` & `node_ext_directory-0.8.1/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 License
 =======
 
 Copyright (c) 2010-2021, BlueDynamics Alliance, Austria
-Copyright (c) 2021-2022, Node Contributors
+Copyright (c) 2021-2024, Node Contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `node.ext.directory-0.8/README.rst` & `node_ext_directory-0.8.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,29 @@
     :alt: Number of PyPI downloads
 
 .. image:: https://github.com/conestack/node.ext.directory/actions/workflows/test.yaml/badge.svg
     :target: https://github.com/conestack/node.ext.directory/actions/workflows/test.yaml
     :alt: Test node.ext.directory
 
 
+Maintenance mode
+----------------
+
+This package is in maintenance mode. The successor of this package is
+`https://pypi.python.org/pypi/node.ext.fs <https://pypi.python.org/pypi/node.ext.fs>`_.
+
+
 Overview
 --------
 
 ``node.ext.directory`` is a node implementation for file system directories.
 
 For more information about ``node`` see
 `https://pypi.python.org/pypi/node <https://pypi.python.org/pypi/node>`_.
 
-
 Usage
 -----
 
 Create new file:
 
 .. code-block:: python
```

### Comparing `node.ext.directory-0.8/TODO.rst` & `node_ext_directory-0.8.1/TODO.rst`

 * *Files identical despite different names*

### Comparing `node.ext.directory-0.8/setup.py` & `node_ext_directory-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '0.8'
+version = '0.8.1'
 shortdesc = 'Filesystem directory abstraction based on nodes'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
```

### Comparing `node.ext.directory-0.8/src/node/ext/directory/directory.py` & `node_ext_directory-0.8.1/src/node/ext/directory/directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from node.behaviors import DefaultInit
 from node.behaviors import DictStorage
 from node.behaviors import MappingAdopt
 from node.behaviors import MappingNode
-from node.behaviors import Reference
+from node.behaviors import MappingReference
 from node.compat import IS_PY2
 from node.ext.directory.events import FileAddedEvent
 from node.ext.directory.interfaces import IDirectory
 from node.ext.directory.interfaces import IFile
 from node.ext.directory.interfaces import MODE_BINARY
 from node.ext.directory.interfaces import MODE_TEXT
 from node.locking import locktree
@@ -130,15 +130,15 @@
         if fs_mode is not None:
             os.chmod(file_path, fs_mode)
 
 
 @plumbing(
     MappingAdopt,
     DefaultInit,
-    Reference,  # XXX: remove from default file
+    MappingReference,  # XXX: remove from default file
     MappingNode,
     FileStorage)
 class File(object):
     pass
 
 
 # global file factories
@@ -320,13 +320,13 @@
             return self.file_factories[factory_keys[0]]
         if factory_keys[1]:
             return file_factories[factory_keys[1]]
 
 
 @plumbing(
     MappingAdopt,
-    Reference,  # XXX: remove from default file
+    MappingReference,  # XXX: remove from default file
     MappingNode,
     DirectoryStorage)
 class Directory(object):
     """Object mapping a file system directory.
     """
```

### Comparing `node.ext.directory-0.8/src/node/ext/directory/interfaces.py` & `node_ext_directory-0.8.1/src/node/ext/directory/interfaces.py`

 * *Files identical despite different names*

### Comparing `node.ext.directory-0.8/src/node/ext/directory/tests.py` & `node_ext_directory-0.8.1/src/node/ext/directory/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from node.behaviors import DefaultInit
 from node.behaviors import DictStorage
 from node.behaviors import MappingAdopt
 from node.behaviors import MappingNode
-from node.behaviors import Reference
+from node.behaviors import MappingReference
 from node.compat import IS_PY2
 from node.ext.directory import Directory
 from node.ext.directory import directory
 from node.ext.directory import File
 from node.ext.directory import MODE_BINARY
 from node.ext.directory import MODE_TEXT
 from node.ext.directory.events import IFileAddedEvent
@@ -142,14 +142,15 @@
 
         file.data = b'\x00\x00'
         file()
         with open(filepath) as f:
             out = f.read()
         self.assertEqual(out, '\x00\x00')
 
+    @unittest.skipIf(os.name == 'nt', 'This test is written for *nix platforms')
     def test_file_permissions(self):
         filepath = os.path.join(self.tempdir, 'file.txt')
         file = File(name=filepath)
         self.assertEqual(file.fs_mode, None)
 
         file.fs_mode = 0o644
         file.direct_sync = True
@@ -312,14 +313,15 @@
 
         self.assertFalse(os.path.exists(dirpath))
 
         directory()
         self.assertTrue(os.path.exists(dirpath))
         self.assertTrue(os.path.isdir(dirpath))
 
+    @unittest.skipIf(os.name == 'nt', 'This test is written for *nix platforms')
     def test_directory_permissions(self):
         dirpath = os.path.join(self.tempdir, 'root')
         directory = Directory(name=dirpath)
         self.assertEqual(directory.fs_mode, None)
 
         directory.fs_mode = 0o750
         directory()
@@ -341,15 +343,15 @@
         err = self.expectError(KeyError, add_directory_fails)
         self.assertEqual(str(err), '\'Empty key not allowed in directories\'')
 
         directory['subdir1'] = Directory()
         directory['subdir2'] = Directory()
 
         self.checkOutput("""\
-        <class 'node.ext.directory.directory.Directory'>: /.../root
+        <class 'node.ext.directory.directory.Directory'>: ...root
           <class 'node.ext.directory.directory.Directory'>: subdir1
           <class 'node.ext.directory.directory.Directory'>: subdir2
         """, directory.treerepr())
 
         fs_path = os.path.join(*directory.path)
         self.assertEqual(sorted(directory.keys()), ['subdir1', 'subdir2'])
         self.assertFalse(os.path.exists(fs_path))
@@ -358,15 +360,15 @@
         self.assertEqual(
             sorted(os.listdir(fs_path)),
             ['subdir1', 'subdir2']
         )
 
         directory = Directory(name=os.path.join(self.tempdir, 'root'))
         self.checkOutput("""\
-        <class 'node.ext.directory.directory.Directory'>: /.../root
+        <class 'node.ext.directory.directory.Directory'>: ...root
           <class 'node.ext.directory.directory.Directory'>: subdir1
           <class 'node.ext.directory.directory.Directory'>: subdir2
         """, directory.treerepr())
 
     def test_delete_from_directory(self):
         directory = Directory(name=os.path.join(self.tempdir))
         directory['file.txt'] = File()
@@ -412,14 +414,15 @@
         self.assertTrue(str(directory['subdir']).startswith(expected))
 
         def __getitem__fails():
             directory['inexistent']
         err = self.expectError(KeyError, __getitem__fails)
         self.assertEqual(str(err), '\'inexistent\'')
 
+    @unittest.skipIf(os.name == 'nt', 'This test is written for *nix platforms')
     def test_sub_directory_permissions(self):
         directory = Directory(name=os.path.join(self.tempdir, 'root'))
         directory.fs_mode = 0o777
 
         subdir1 = directory['subdir1'] = Directory()
         subdir1.fs_mode = 0o770
 
@@ -443,15 +446,15 @@
         self.assertEqual(directory['subdir2'].fs_mode, 0o755)
 
     def test_add_invalid_child(self):
         # Add invalid child node
         @plumbing(
             MappingAdopt,
             DefaultInit,
-            Reference,
+            MappingReference,
             MappingNode,
             DictStorage)
         class NoFile(object):
             pass
 
         directory = Directory(name=os.path.join(self.tempdir, 'root'))
```

### Comparing `node.ext.directory-0.8/src/node.ext.directory.egg-info/SOURCES.txt` & `node_ext_directory-0.8.1/src/node.ext.directory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

