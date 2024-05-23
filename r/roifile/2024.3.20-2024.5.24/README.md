# Comparing `tmp/roifile-2024.3.20.tar.gz` & `tmp/roifile-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roifile-2024.3.20.tar", last modified: Wed Mar 20 16:39:13 2024, max compression
+gzip compressed data, was "roifile-2024.5.24.tar", last modified: Thu May 23 19:22:09 2024, max compression
```

## Comparing `roifile-2024.3.20.tar` & `roifile-2024.5.24.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 16:39:13.314646 roifile-2024.3.20/
--rw-rw-rw-   0        0        0     1431 2024-03-20 16:39:12.000000 roifile-2024.3.20/CHANGES.rst
--rw-rw-rw-   0        0        0     1559 2024-03-20 16:39:12.000000 roifile-2024.3.20/LICENSE
--rw-rw-rw-   0        0        0      325 2024-01-11 01:59:53.000000 roifile-2024.3.20/MANIFEST.in
--rw-rw-rw-   0        0        0     4564 2024-03-20 16:39:13.314646 roifile-2024.3.20/PKG-INFO
--rw-rw-rw-   0        0        0     3488 2024-03-20 16:39:12.000000 roifile-2024.3.20/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-20 16:39:13.309558 roifile-2024.3.20/roifile/
--rw-rw-rw-   0        0        0      101 2020-02-14 04:28:42.000000 roifile-2024.3.20/roifile/__init__.py
--rw-rw-rw-   0        0        0      132 2020-02-14 04:32:59.000000 roifile-2024.3.20/roifile/__main__.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 roifile-2024.3.20/roifile/py.typed
--rw-rw-rw-   0        0        0    47036 2024-03-20 16:18:25.000000 roifile-2024.3.20/roifile/roifile.py
-drwxrwxrwx   0        0        0        0 2024-03-20 16:39:13.309558 roifile-2024.3.20/roifile.egg-info/
--rw-rw-rw-   0        0        0     4564 2024-03-20 16:39:13.000000 roifile-2024.3.20/roifile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-03-20 16:39:13.000000 roifile-2024.3.20/roifile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 16:39:13.000000 roifile-2024.3.20/roifile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-03-20 16:39:13.000000 roifile-2024.3.20/roifile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-03-20 16:39:13.000000 roifile-2024.3.20/roifile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-20 16:39:13.000000 roifile-2024.3.20/roifile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1821 2024-03-20 15:00:55.000000 roifile-2024.3.20/roifile_demo.py
--rw-rw-rw-   0        0        0       42 2024-03-20 16:39:13.314646 roifile-2024.3.20/setup.cfg
--rw-rw-rw-   0        0        0     3046 2024-01-11 01:58:05.000000 roifile-2024.3.20/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:22:09.016891 roifile-2024.5.24/
+-rw-rw-rw-   0        0        0     1504 2024-05-23 19:22:07.000000 roifile-2024.5.24/CHANGES.rst
+-rw-rw-rw-   0        0        0     1559 2024-05-23 19:22:07.000000 roifile-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      325 2024-01-11 01:59:53.000000 roifile-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     4637 2024-05-23 19:22:09.016891 roifile-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     3791 2024-05-23 19:22:07.000000 roifile-2024.5.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-23 19:22:09.015326 roifile-2024.5.24/roifile/
+-rw-rw-rw-   0        0        0      101 2020-02-14 04:28:42.000000 roifile-2024.5.24/roifile/__init__.py
+-rw-rw-rw-   0        0        0      132 2020-02-14 04:32:59.000000 roifile-2024.5.24/roifile/__main__.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 roifile-2024.5.24/roifile/py.typed
+-rw-rw-rw-   0        0        0    47109 2024-05-23 19:20:57.000000 roifile-2024.5.24/roifile/roifile.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:22:09.016891 roifile-2024.5.24/roifile.egg-info/
+-rw-rw-rw-   0        0        0     4637 2024-05-23 19:22:08.000000 roifile-2024.5.24/roifile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-05-23 19:22:08.000000 roifile-2024.5.24/roifile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:22:08.000000 roifile-2024.5.24/roifile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-23 19:22:08.000000 roifile-2024.5.24/roifile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-23 19:22:08.000000 roifile-2024.5.24/roifile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 19:22:08.000000 roifile-2024.5.24/roifile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1819 2024-05-23 19:18:46.000000 roifile-2024.5.24/roifile_demo.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:22:09.016891 roifile-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     3677 2024-05-20 16:40:19.000000 roifile-2024.5.24/setup.py
```

### Comparing `roifile-2024.3.20/CHANGES.rst` & `roifile-2024.5.24/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.3.20
 
 - Fix writing generator of ROIs (#9).
 
 2024.1.10
 
 - Support text rotation.
```

### Comparing `roifile-2024.3.20/LICENSE` & `roifile-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `roifile-2024.3.20/PKG-INFO` & `roifile-2024.5.24/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roifile
-Version: 2024.3.20
+Version: 2024.5.24
 Summary: Read and write ImageJ ROI format
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/roifile/issues
 Project-URL: Source Code, https://github.com/cgohlke/roifile
@@ -34,15 +34,15 @@
 an undocumented and ImageJ application specific format to store regions of
 interest, geometric shapes, paths, text, and whatnot for image overlays.
 
 .. _ImageJ: https://imagej.net
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.3.20
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.6941603 <https://doi.org/10.5281/zenodo.6941603>`_
 
 Quickstart
 ----------
 
 Install the roifile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/roifile/>`_::
@@ -60,22 +60,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `Numpy <https://pypi.org/project/numpy/>`_ 1.26.4
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.2.12 (optional)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.3 (optional)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22 (optional)
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4 (optional)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.3.20
 
 - Fix writing generator of ROIs (#9).
 
 2024.1.10
 
 - Support text rotation.
```

### Comparing `roifile-2024.3.20/README.rst` & `roifile-2024.5.24/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+..
+  This file is generated by setup.py
+
 Read and write ImageJ ROI format
 ================================
 
 Roifile is a Python library to read, write, create, and plot `ImageJ`_ ROIs,
 an undocumented and ImageJ application specific format to store regions of
 interest, geometric shapes, paths, text, and whatnot for image overlays.
 
 .. _ImageJ: https://imagej.net
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.3.20
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.6941603 <https://doi.org/10.5281/zenodo.6941603>`_
 
 Quickstart
 ----------
 
 Install the roifile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/roifile/>`_::
@@ -31,22 +34,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `Numpy <https://pypi.org/project/numpy/>`_ 1.26.4
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.2.12 (optional)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.3 (optional)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22 (optional)
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4 (optional)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.3.20
 
 - Fix writing generator of ROIs (#9).
 
 2024.1.10
 
 - Support text rotation.
@@ -97,41 +104,49 @@
 - `napari_jroitools <https://github.com/jayunruh/napari_jroitools>`_
 
 Examples
 --------
 
 Create a new ImagejRoi instance from an array of x, y coordinates:
 
->>> roi = ImagejRoi.frompoints([[1.1, 2.2], [3.3, 4.4], [5.5, 6.6]])
->>> roi.roitype = ROI_TYPE.POINT
->>> roi.options |= ROI_OPTIONS.SHOW_LABELS
+.. code-block:: python
+
+    >>> roi = ImagejRoi.frompoints([[1.1, 2.2], [3.3, 4.4], [5.5, 6.6]])
+    >>> roi.roitype = ROI_TYPE.POINT
+    >>> roi.options |= ROI_OPTIONS.SHOW_LABELS
 
 Export the instance to an ImageJ ROI formatted byte string or file:
 
->>> out = roi.tobytes()
->>> out[:4]
-b'Iout'
->>> roi.tofile('_test.roi')
+.. code-block:: python
+
+    >>> out = roi.tobytes()
+    >>> out[:4]
+    b'Iout'
+    >>> roi.tofile('_test.roi')
 
 Read the ImageJ ROI from the file and verify the content:
 
->>> roi2 = ImagejRoi.fromfile('_test.roi')
->>> roi2 == roi
-True
->>> roi.roitype == ROI_TYPE.POINT
-True
->>> roi.subpixelresolution
-True
->>> roi.coordinates()
-array([[1.1, 2.2],
-       [3.3, 4.4],
-       [5.5, 6.6]], dtype=float32)
->>> roi.left, roi.top, roi.right, roi.bottom
-(1, 2, 7, 8)
+.. code-block:: python
+
+    >>> roi2 = ImagejRoi.fromfile('_test.roi')
+    >>> roi2 == roi
+    True
+    >>> roi.roitype == ROI_TYPE.POINT
+    True
+    >>> roi.subpixelresolution
+    True
+    >>> roi.coordinates()
+    array([[1.1, 2.2],
+           [3.3, 4.4],
+           [5.5, 6.6]], dtype=float32)
+    >>> roi.left, roi.top, roi.right, roi.bottom
+    (1, 2, 7, 8)
 
 Plot the ROI using matplotlib:
 
->>> roi.plot()
+.. code-block:: python
+
+    >>> roi.plot()
 
 View the overlays stored in a ROI, ZIP, or TIFF file from a command line::
 
-    python -m roifile _test.roi
+    python -m roifile _test.roi
```

### Comparing `roifile-2024.3.20/roifile/roifile.py` & `roifile-2024.5.24/roifile/roifile.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 an undocumented and ImageJ application specific format to store regions of
 interest, geometric shapes, paths, text, and whatnot for image overlays.
 
 .. _ImageJ: https://imagej.net
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.3.20
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.6941603 <https://doi.org/10.5281/zenodo.6941603>`_
 
 Quickstart
 ----------
 
 Install the roifile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/roifile/>`_::
@@ -61,22 +61,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `Numpy <https://pypi.org/project/numpy/>`_ 1.26.4
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.2.12 (optional)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.3 (optional)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22 (optional)
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4 (optional)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.3.20
 
 - Fix writing generator of ROIs (#9).
 
 2024.1.10
 
 - Support text rotation.
@@ -166,15 +170,15 @@
 
     python -m roifile _test.roi
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.3.20'
+__version__ = '2024.5.24'
 
 __all__ = [
     'roiread',
     'roiwrite',
     'ImagejRoi',
     'ROI_TYPE',
     'ROI_SUBTYPE',
```

### Comparing `roifile-2024.3.20/roifile.egg-info/PKG-INFO` & `roifile-2024.5.24/roifile.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roifile
-Version: 2024.3.20
+Version: 2024.5.24
 Summary: Read and write ImageJ ROI format
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/roifile/issues
 Project-URL: Source Code, https://github.com/cgohlke/roifile
@@ -34,15 +34,15 @@
 an undocumented and ImageJ application specific format to store regions of
 interest, geometric shapes, paths, text, and whatnot for image overlays.
 
 .. _ImageJ: https://imagej.net
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.3.20
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.6941603 <https://doi.org/10.5281/zenodo.6941603>`_
 
 Quickstart
 ----------
 
 Install the roifile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/roifile/>`_::
@@ -60,22 +60,26 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `Numpy <https://pypi.org/project/numpy/>`_ 1.26.4
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.2.12 (optional)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.3 (optional)
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22 (optional)
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4 (optional)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.3.20
 
 - Fix writing generator of ROIs (#9).
 
 2024.1.10
 
 - Support text rotation.
```

### Comparing `roifile-2024.3.20/roifile_demo.py` & `roifile-2024.5.24/roifile_demo.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 Use the roifile and tifffile modules to read and write the results of image
 segmentation from/to ImageJ TIFF files.
 
 """
 
 import numpy
 from matplotlib import pyplot
+from roifile import ImagejRoi
 from skimage.measure import find_contours, label, regionprops
 from tifffile import TiffFile, imwrite
 
-from roifile import ImagejRoi
-
 
 def plot_image_overlays(image, overlays, **kwargs):
     """Plot image and overlays (bytes) using matplotlib."""
     fig, ax = pyplot.subplots()
     ax.imshow(image, cmap='gray')
     if not isinstance(overlays, list):
         overlays = [overlays]
```

### Comparing `roifile-2024.3.20/setup.py` & `roifile-2024.5.24/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,22 +4,40 @@
 
 import re
 import sys
 
 from setuptools import setup
 
 
-def search(pattern, code, flags=0):
-    # return first match for pattern in code
-    match = re.search(pattern, code, flags)
+def search(pattern, string, flags=0):
+    """Return first match of pattern in string."""
+    match = re.search(pattern, string, flags)
     if match is None:
         raise ValueError(f'{pattern!r} not found')
     return match.groups()[0]
 
 
+def fix_docstring_examples(docstring):
+    """Return docstring with examples fixed for GitHub."""
+    start = True
+    indent = False
+    lines = ['..', '  This file is generated by setup.py', '']
+    for line in docstring.splitlines():
+        if not line.strip():
+            start = True
+            indent = False
+        if line.startswith('>>> '):
+            indent = True
+            if start:
+                lines.extend(['.. code-block:: python', ''])
+                start = False
+        lines.append(('    ' if indent else '') + line)
+    return '\n'.join(lines)
+
+
 with open('roifile/roifile.py', encoding='utf-8') as fh:
     code = fh.read().replace('\r\n', '\n').replace('\r', '\n')
 
 version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev0')
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
@@ -32,15 +50,15 @@
     [description, '=' * len(description)] + readme.splitlines()[1:]
 )
 
 if 'sdist' in sys.argv:
     # update README, LICENSE, and CHANGES files
 
     with open('README.rst', 'w', encoding='utf-8') as fh:
-        fh.write(readme)
+        fh.write(fix_docstring_examples(readme))
 
     license = search(
         r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+""',
         code,
         re.MULTILINE | re.DOTALL,
     )
     license = license.replace('# ', '').replace('#', '')
```

