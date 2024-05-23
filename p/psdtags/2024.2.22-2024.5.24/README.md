# Comparing `tmp/psdtags-2024.2.22.tar.gz` & `tmp/psdtags-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdtags-2024.2.22.tar", last modified: Thu Feb 22 21:28:39 2024, max compression
+gzip compressed data, was "psdtags-2024.5.24.tar", last modified: Thu May 23 19:31:57 2024, max compression
```

## Comparing `psdtags-2024.2.22.tar` & `psdtags-2024.5.24.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-02-22 21:28:39.384445 psdtags-2024.2.22/
--rw-rw-rw-   0        0        0     1559 2024-02-22 21:28:38.000000 psdtags-2024.2.22/LICENSE
--rw-rw-rw-   0        0        0      440 2023-08-11 02:59:01.000000 psdtags-2024.2.22/MANIFEST.in
--rw-rw-rw-   0        0        0     6857 2024-02-22 21:28:39.384445 psdtags-2024.2.22/PKG-INFO
--rw-rw-rw-   0        0        0     5752 2024-02-22 21:28:38.000000 psdtags-2024.2.22/README.rst
-drwxrwxrwx   0        0        0        0 2024-02-22 21:28:39.384445 psdtags-2024.2.22/examples/
--rw-rw-rw-   0        0        0    10124 2024-01-09 06:39:52.000000 psdtags-2024.2.22/examples/layered_tiff.py
--rw-rw-rw-   0        0        0     1685 2023-02-08 17:59:20.000000 psdtags-2024.2.22/examples/product.png
--rw-rw-rw-   0        0        0     2368 2023-02-08 18:00:10.000000 psdtags-2024.2.22/examples/reflection.png
--rw-rw-rw-   0        0        0      875 2023-02-08 17:59:29.000000 psdtags-2024.2.22/examples/shadow.png
-drwxrwxrwx   0        0        0        0 2024-02-22 21:28:39.384445 psdtags-2024.2.22/psdtags/
--rw-rw-rw-   0        0        0      101 2024-01-09 06:23:52.000000 psdtags-2024.2.22/psdtags/__init__.py
--rw-rw-rw-   0        0        0      132 2022-01-14 16:45:31.000000 psdtags-2024.2.22/psdtags/__main__.py
--rw-rw-rw-   0        0        0   128768 2024-02-22 21:27:27.000000 psdtags-2024.2.22/psdtags/psdtags.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 psdtags-2024.2.22/psdtags/py.typed
-drwxrwxrwx   0        0        0        0 2024-02-22 21:28:39.384445 psdtags-2024.2.22/psdtags.egg-info/
--rw-rw-rw-   0        0        0     6857 2024-02-22 21:28:39.000000 psdtags-2024.2.22/psdtags.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-02-22 21:28:39.000000 psdtags-2024.2.22/psdtags.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-22 21:28:39.000000 psdtags-2024.2.22/psdtags.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-02-22 21:28:39.000000 psdtags-2024.2.22/psdtags.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2024-02-22 21:28:39.000000 psdtags-2024.2.22/psdtags.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-22 21:28:39.000000 psdtags-2024.2.22/psdtags.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-22 21:28:39.384445 psdtags-2024.2.22/setup.cfg
--rw-rw-rw-   0        0        0     2497 2024-01-09 06:57:24.000000 psdtags-2024.2.22/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:31:57.632146 psdtags-2024.5.24/
+-rw-rw-rw-   0        0        0     1559 2024-05-23 19:31:56.000000 psdtags-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      440 2023-08-11 02:59:01.000000 psdtags-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     6939 2024-05-23 19:31:57.632146 psdtags-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     6112 2024-05-23 19:31:56.000000 psdtags-2024.5.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-23 19:31:57.627148 psdtags-2024.5.24/examples/
+-rw-rw-rw-   0        0        0    10124 2024-01-09 06:39:52.000000 psdtags-2024.5.24/examples/layered_tiff.py
+-rw-rw-rw-   0        0        0     1685 2023-02-08 17:59:20.000000 psdtags-2024.5.24/examples/product.png
+-rw-rw-rw-   0        0        0     2368 2023-02-08 18:00:10.000000 psdtags-2024.5.24/examples/reflection.png
+-rw-rw-rw-   0        0        0      875 2023-02-08 17:59:29.000000 psdtags-2024.5.24/examples/shadow.png
+drwxrwxrwx   0        0        0        0 2024-05-23 19:31:57.629146 psdtags-2024.5.24/psdtags/
+-rw-rw-rw-   0        0        0      101 2024-01-09 06:23:52.000000 psdtags-2024.5.24/psdtags/__init__.py
+-rw-rw-rw-   0        0        0      132 2022-01-14 16:45:31.000000 psdtags-2024.5.24/psdtags/__main__.py
+-rw-rw-rw-   0        0        0   128850 2024-05-23 19:28:20.000000 psdtags-2024.5.24/psdtags/psdtags.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 psdtags-2024.5.24/psdtags/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-23 19:31:57.631147 psdtags-2024.5.24/psdtags.egg-info/
+-rw-rw-rw-   0        0        0     6939 2024-05-23 19:31:57.000000 psdtags-2024.5.24/psdtags.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-05-23 19:31:57.000000 psdtags-2024.5.24/psdtags.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:31:57.000000 psdtags-2024.5.24/psdtags.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-23 19:31:57.000000 psdtags-2024.5.24/psdtags.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2024-05-23 19:31:57.000000 psdtags-2024.5.24/psdtags.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 19:31:57.000000 psdtags-2024.5.24/psdtags.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:31:57.633147 psdtags-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     3203 2024-05-20 18:39:13.000000 psdtags-2024.5.24/setup.py
```

### Comparing `psdtags-2024.2.22/LICENSE` & `psdtags-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `psdtags-2024.2.22/PKG-INFO` & `psdtags-2024.5.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdtags
-Version: 2024.2.22
+Version: 2024.5.24
 Summary: Read and write layered TIFF ImageSourceData and ImageResources tags
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/psdtags/issues
 Project-URL: Source Code, https://github.com/cgohlke/psdtags
@@ -42,15 +42,15 @@
 `Adobe Photoshop File Formats Specification (November 2019)
 <https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/>`_.
 
 Adobe Photoshop is a registered trademark of Adobe Systems Inc.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.2.22
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.7879187 <https://doi.org/10.5281/zenodo.7879187>`_
 
 Quickstart
 ----------
 
 Install the psdtags package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psdtags/>`_::
@@ -68,26 +68,30 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2024.1.1
   (required for compressing/decompressing image data)
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.2.12
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22
   (required for reading/writing tags from/to TIFF files)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.3
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (required for plotting)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.2.22
 
 - Fix reading PsdBoolean (#10).
 - Fix order of PsdReferencePoint coordinates (breaking).
 - Allow reading unaligned PsdLayer blending_ranges.
 
 2024.1.15
@@ -165,28 +169,29 @@
 Consider `psd-tools <https://github.com/psd-tools/psd-tools>`_ and
 `pytoshop <https://github.com/mdboom/pytoshop>`_  for working with
 Adobe Photoshop PSD files.
 
 Layered TIFF files can be read or written by Photoshop, Affinity Photo, and
 Krita.
 
-See also `Reading and writing a Photoshop TIFF <https://www.amyspark.me/blog/
-posts/2021/11/14/reading-and-writing-tiff-psds.html>`_.
+See also `Reading and writing a Photoshop TIFF
+<https://www.amyspark.me/blog/posts/2021/11/14/reading-and-writing-tiff-psds.html>`_.
 
 Examples
 --------
 
 Read the ImageSourceData tag value from a layered TIFF file and iterate over
 all the channels:
 
 >>> isd = TiffImageSourceData.fromtiff('layered.tif')
 >>> for layer in isd.layers:
 ...     layer.name
 ...     for channel in layer.channels:
 ...         ch = channel.data  # a numpy array
+...
 'Background'
 'Reflect1'
 'Reflect2'
 'image'
 'Layer 1'
 'ORight'
 'I'
@@ -195,14 +200,15 @@
 
 Read the ImageResources tag value from the TIFF file, iterate over the blocks,
 and get the thumbnail image:
 
 >>> res = TiffImageResources.fromtiff('layered.tif')
 >>> for block in res.blocks:
 ...     blockname = block.name
+...
 >>> res.thumbnail().shape
 (90, 160, 3)
 
 Write the image, ImageSourceData and ImageResources to a new layered TIFF file:
 
 >>> from tifffile import imread, imwrite
 >>> image = imread('layered.tif')
```

### Comparing `psdtags-2024.2.22/README.rst` & `psdtags-2024.5.24/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+..
+  This file is generated by setup.py
+
 Read and write layered TIFF ImageSourceData and ImageResources tags
 ===================================================================
 
 Psdtags is a Python library to read and write the Adobe Photoshop(r) specific
 ImageResources (#34377) and ImageSourceData (#37724) TIFF tags, which contain
 image resource blocks, layer and mask information found in a typical layered
 TIFF file created by Photoshop.
@@ -13,15 +16,15 @@
 `Adobe Photoshop File Formats Specification (November 2019)
 <https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/>`_.
 
 Adobe Photoshop is a registered trademark of Adobe Systems Inc.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.2.22
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.7879187 <https://doi.org/10.5281/zenodo.7879187>`_
 
 Quickstart
 ----------
 
 Install the psdtags package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psdtags/>`_::
@@ -39,26 +42,30 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2024.1.1
   (required for compressing/decompressing image data)
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.2.12
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22
   (required for reading/writing tags from/to TIFF files)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.3
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (required for plotting)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.2.22
 
 - Fix reading PsdBoolean (#10).
 - Fix order of PsdReferencePoint coordinates (breaking).
 - Allow reading unaligned PsdLayer blending_ranges.
 
 2024.1.15
@@ -136,65 +143,75 @@
 Consider `psd-tools <https://github.com/psd-tools/psd-tools>`_ and
 `pytoshop <https://github.com/mdboom/pytoshop>`_  for working with
 Adobe Photoshop PSD files.
 
 Layered TIFF files can be read or written by Photoshop, Affinity Photo, and
 Krita.
 
-See also `Reading and writing a Photoshop TIFF <https://www.amyspark.me/blog/
-posts/2021/11/14/reading-and-writing-tiff-psds.html>`_.
+See also `Reading and writing a Photoshop TIFF
+<https://www.amyspark.me/blog/posts/2021/11/14/reading-and-writing-tiff-psds.html>`_.
 
 Examples
 --------
 
 Read the ImageSourceData tag value from a layered TIFF file and iterate over
 all the channels:
 
->>> isd = TiffImageSourceData.fromtiff('layered.tif')
->>> for layer in isd.layers:
-...     layer.name
-...     for channel in layer.channels:
-...         ch = channel.data  # a numpy array
-'Background'
-'Reflect1'
-'Reflect2'
-'image'
-'Layer 1'
-'ORight'
-'I'
-'IShadow'
-'O'
+.. code-block:: python
+
+    >>> isd = TiffImageSourceData.fromtiff('layered.tif')
+    >>> for layer in isd.layers:
+    ...     layer.name
+    ...     for channel in layer.channels:
+    ...         ch = channel.data  # a numpy array
+    ...
+    'Background'
+    'Reflect1'
+    'Reflect2'
+    'image'
+    'Layer 1'
+    'ORight'
+    'I'
+    'IShadow'
+    'O'
 
 Read the ImageResources tag value from the TIFF file, iterate over the blocks,
 and get the thumbnail image:
 
->>> res = TiffImageResources.fromtiff('layered.tif')
->>> for block in res.blocks:
-...     blockname = block.name
->>> res.thumbnail().shape
-(90, 160, 3)
+.. code-block:: python
+
+    >>> res = TiffImageResources.fromtiff('layered.tif')
+    >>> for block in res.blocks:
+    ...     blockname = block.name
+    ...
+    >>> res.thumbnail().shape
+    (90, 160, 3)
 
 Write the image, ImageSourceData and ImageResources to a new layered TIFF file:
 
->>> from tifffile import imread, imwrite
->>> image = imread('layered.tif')
->>> imwrite(
-...     '_layered.tif',
-...     image,
-...     byteorder=isd.byteorder,  # must match ImageSourceData
-...     photometric='rgb',  # must match ImageSourceData
-...     metadata=None,  # do not write any tifffile specific metadata
-...     extratags=[isd.tifftag(maxworkers=4), res.tifftag()],
-... )
+.. code-block:: python
+
+    >>> from tifffile import imread, imwrite
+    >>> image = imread('layered.tif')
+    >>> imwrite(
+    ...     '_layered.tif',
+    ...     image,
+    ...     byteorder=isd.byteorder,  # must match ImageSourceData
+    ...     photometric='rgb',  # must match ImageSourceData
+    ...     metadata=None,  # do not write any tifffile specific metadata
+    ...     extratags=[isd.tifftag(maxworkers=4), res.tifftag()],
+    ... )
 
 Verify that the new layered TIFF file contains readable ImageSourceData:
 
->>> assert isd == TiffImageSourceData.fromtiff('_layered.tif')
->>> assert res == TiffImageResources.fromtiff('_layered.tif')
+.. code-block:: python
+
+    >>> assert isd == TiffImageSourceData.fromtiff('_layered.tif')
+    >>> assert res == TiffImageResources.fromtiff('_layered.tif')
 
 View the layer and mask information as well as the image resource blocks in
 a layered TIFF file from a command line::
 
     python -m psdtags layered.tif
 
 Refer to the `layered_tiff.py` example in the source distribution for
-creating a layered TIFF file from individual layer images.
+creating a layered TIFF file from individual layer images.
```

### Comparing `psdtags-2024.2.22/examples/layered_tiff.py` & `psdtags-2024.5.24/examples/layered_tiff.py`

 * *Files identical despite different names*

### Comparing `psdtags-2024.2.22/examples/product.png` & `psdtags-2024.5.24/examples/product.png`

 * *Files identical despite different names*

### Comparing `psdtags-2024.2.22/examples/reflection.png` & `psdtags-2024.5.24/examples/reflection.png`

 * *Files identical despite different names*

### Comparing `psdtags-2024.2.22/examples/shadow.png` & `psdtags-2024.5.24/examples/shadow.png`

 * *Files identical despite different names*

### Comparing `psdtags-2024.2.22/psdtags/psdtags.py` & `psdtags-2024.5.24/psdtags/psdtags.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 `Adobe Photoshop File Formats Specification (November 2019)
 <https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/>`_.
 
 Adobe Photoshop is a registered trademark of Adobe Systems Inc.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.2.22
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.7879187 <https://doi.org/10.5281/zenodo.7879187>`_
 
 Quickstart
 ----------
 
 Install the psdtags package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psdtags/>`_::
@@ -69,26 +69,30 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2024.1.1
   (required for compressing/decompressing image data)
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.2.12
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22
   (required for reading/writing tags from/to TIFF files)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.3
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (required for plotting)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.2.22
 
 - Fix reading PsdBoolean (#10).
 - Fix order of PsdReferencePoint coordinates (breaking).
 - Allow reading unaligned PsdLayer blending_ranges.
 
 2024.1.15
@@ -166,28 +170,29 @@
 Consider `psd-tools <https://github.com/psd-tools/psd-tools>`_ and
 `pytoshop <https://github.com/mdboom/pytoshop>`_  for working with
 Adobe Photoshop PSD files.
 
 Layered TIFF files can be read or written by Photoshop, Affinity Photo, and
 Krita.
 
-See also `Reading and writing a Photoshop TIFF <https://www.amyspark.me/blog/
-posts/2021/11/14/reading-and-writing-tiff-psds.html>`_.
+See also `Reading and writing a Photoshop TIFF
+<https://www.amyspark.me/blog/posts/2021/11/14/reading-and-writing-tiff-psds.html>`_.
 
 Examples
 --------
 
 Read the ImageSourceData tag value from a layered TIFF file and iterate over
 all the channels:
 
 >>> isd = TiffImageSourceData.fromtiff('layered.tif')
 >>> for layer in isd.layers:
 ...     layer.name
 ...     for channel in layer.channels:
 ...         ch = channel.data  # a numpy array
+...
 'Background'
 'Reflect1'
 'Reflect2'
 'image'
 'Layer 1'
 'ORight'
 'I'
@@ -196,14 +201,15 @@
 
 Read the ImageResources tag value from the TIFF file, iterate over the blocks,
 and get the thumbnail image:
 
 >>> res = TiffImageResources.fromtiff('layered.tif')
 >>> for block in res.blocks:
 ...     blockname = block.name
+...
 >>> res.thumbnail().shape
 (90, 160, 3)
 
 Write the image, ImageSourceData and ImageResources to a new layered TIFF file:
 
 >>> from tifffile import imread, imwrite
 >>> image = imread('layered.tif')
@@ -229,15 +235,15 @@
 Refer to the `layered_tiff.py` example in the source distribution for
 creating a layered TIFF file from individual layer images.
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.2.22'
+__version__ = '2024.5.24'
 
 __all__ = [
     'PsdBlendMode',
     'PsdBoolean',
     'PsdBytesBlock',
     'PsdChannel',
     'PsdChannelId',
```

### Comparing `psdtags-2024.2.22/psdtags.egg-info/PKG-INFO` & `psdtags-2024.5.24/psdtags.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdtags
-Version: 2024.2.22
+Version: 2024.5.24
 Summary: Read and write layered TIFF ImageSourceData and ImageResources tags
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/psdtags/issues
 Project-URL: Source Code, https://github.com/cgohlke/psdtags
@@ -42,15 +42,15 @@
 `Adobe Photoshop File Formats Specification (November 2019)
 <https://www.adobe.com/devnet-apps/photoshop/fileformatashtml/>`_.
 
 Adobe Photoshop is a registered trademark of Adobe Systems Inc.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.2.22
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.7879187 <https://doi.org/10.5281/zenodo.7879187>`_
 
 Quickstart
 ----------
 
 Install the psdtags package and all dependencies from the
 `Python Package Index <https://pypi.org/project/psdtags/>`_::
@@ -68,26 +68,30 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2024.1.1
   (required for compressing/decompressing image data)
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.2.12
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2024.5.22
   (required for reading/writing tags from/to TIFF files)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.3
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (required for plotting)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.2.22
 
 - Fix reading PsdBoolean (#10).
 - Fix order of PsdReferencePoint coordinates (breaking).
 - Allow reading unaligned PsdLayer blending_ranges.
 
 2024.1.15
@@ -165,28 +169,29 @@
 Consider `psd-tools <https://github.com/psd-tools/psd-tools>`_ and
 `pytoshop <https://github.com/mdboom/pytoshop>`_  for working with
 Adobe Photoshop PSD files.
 
 Layered TIFF files can be read or written by Photoshop, Affinity Photo, and
 Krita.
 
-See also `Reading and writing a Photoshop TIFF <https://www.amyspark.me/blog/
-posts/2021/11/14/reading-and-writing-tiff-psds.html>`_.
+See also `Reading and writing a Photoshop TIFF
+<https://www.amyspark.me/blog/posts/2021/11/14/reading-and-writing-tiff-psds.html>`_.
 
 Examples
 --------
 
 Read the ImageSourceData tag value from a layered TIFF file and iterate over
 all the channels:
 
 >>> isd = TiffImageSourceData.fromtiff('layered.tif')
 >>> for layer in isd.layers:
 ...     layer.name
 ...     for channel in layer.channels:
 ...         ch = channel.data  # a numpy array
+...
 'Background'
 'Reflect1'
 'Reflect2'
 'image'
 'Layer 1'
 'ORight'
 'I'
@@ -195,14 +200,15 @@
 
 Read the ImageResources tag value from the TIFF file, iterate over the blocks,
 and get the thumbnail image:
 
 >>> res = TiffImageResources.fromtiff('layered.tif')
 >>> for block in res.blocks:
 ...     blockname = block.name
+...
 >>> res.thumbnail().shape
 (90, 160, 3)
 
 Write the image, ImageSourceData and ImageResources to a new layered TIFF file:
 
 >>> from tifffile import imread, imwrite
 >>> image = imread('layered.tif')
```

### Comparing `psdtags-2024.2.22/setup.py` & `psdtags-2024.5.24/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,76 @@
 # psdtags/setup.py
 
 """Psdtags package setuptools script."""
 
-import sys
 import re
+import sys
 
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
 with open('psdtags/psdtags.py', encoding='utf-8') as fh:
     code = fh.read()
 
 version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev0')
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
 readme = search(
     r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}from __future__',
     code,
     re.MULTILINE | re.DOTALL,
 )
-
 readme = '\n'.join(
     [description, '=' * len(description)] + readme.splitlines()[1:]
 )
 
-license = search(
-    r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+""',
-    code,
-    re.MULTILINE | re.DOTALL,
-)
-
-license = license.replace('# ', '').replace('#', '')
 
 if 'sdist' in sys.argv:
+    # update README, LICENSE, and CHANGES files
+
+    with open('README.rst', 'w', encoding='utf-8') as fh:
+        fh.write(fix_docstring_examples(readme))
+
+    license = search(
+        r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+""',
+        code,
+        re.MULTILINE | re.DOTALL,
+    )
+    license = license.replace('# ', '').replace('#', '')
+
     with open('LICENSE', 'w', encoding='utf-8') as fh:
         fh.write('BSD 3-Clause License\n\n')
         fh.write(license)
-    with open('README.rst', 'w', encoding='utf-8') as fh:
-        fh.write(readme)
 
 setup(
     name='psdtags',
     version=version,
     license='BSD',
     description=description,
     long_description=readme,
```

