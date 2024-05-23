# Comparing `tmp/twiss-0.2.5.tar.gz` & `tmp/twiss-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twiss-0.2.5.tar", last modified: Fri Apr 19 18:06:08 2024, max compression
+gzip compressed data, was "twiss-0.2.6.tar", last modified: Thu May 23 15:19:29 2024, max compression
```

## Comparing `twiss-0.2.5.tar` & `twiss-0.2.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:08.356995 twiss-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:08.344995 twiss-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:08.348995 twiss-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-19 18:04:36.000000 twiss-0.2.5/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-19 18:04:36.000000 twiss-0.2.5/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-19 18:04:36.000000 twiss-0.2.5/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-19 18:04:36.000000 twiss-0.2.5/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-19 18:04:36.000000 twiss-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 18:04:36.000000 twiss-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 18:04:36.000000 twiss-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-19 18:06:08.356995 twiss-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-19 18:04:36.000000 twiss-0.2.5/README.MD
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:08.348995 twiss-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:08.348995 twiss-0.2.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:08.348995 twiss-0.2.5/docs/source/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)   864937 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/source/examples/twiss.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:08.352995 twiss-0.2.5/docs/source/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/source/modules/convert.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/source/modules/distribution.rst
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/source/modules/invariant.rst
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/source/modules/matrix.rst
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/source/modules/normal.rst
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/source/modules/transport.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/source/modules/util.rst
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 18:04:36.000000 twiss-0.2.5/docs/source/modules/wolski.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-19 18:04:36.000000 twiss-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:06:08.356995 twiss-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:08.352995 twiss-0.2.5/twiss/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-19 18:04:36.000000 twiss-0.2.5/twiss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-19 18:04:36.000000 twiss-0.2.5/twiss/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-19 18:04:36.000000 twiss-0.2.5/twiss/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-19 18:04:36.000000 twiss-0.2.5/twiss/invariant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-19 18:04:36.000000 twiss-0.2.5/twiss/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-19 18:04:36.000000 twiss-0.2.5/twiss/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-19 18:04:36.000000 twiss-0.2.5/twiss/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-19 18:04:36.000000 twiss-0.2.5/twiss/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-04-19 18:04:36.000000 twiss-0.2.5/twiss/wolski.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:06:08.352995 twiss-0.2.5/twiss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-19 18:06:08.000000 twiss-0.2.5/twiss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-19 18:06:08.000000 twiss-0.2.5/twiss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:06:08.000000 twiss-0.2.5/twiss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-19 18:06:08.000000 twiss-0.2.5/twiss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 18:06:08.000000 twiss-0.2.5/twiss.egg-info/top_level.txt
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2024-05-23 15:19:29.480618 twiss-0.2.6/
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2024-05-23 15:19:29.472618 twiss-0.2.6/.github/
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2024-05-23 15:19:29.472618 twiss-0.2.6/.github/workflows/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      860 2024-03-05 01:41:55.000000 twiss-0.2.6/.github/workflows/docs.yaml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      756 2024-03-05 01:41:55.000000 twiss-0.2.6/.github/workflows/lint.yaml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      646 2024-03-05 01:41:55.000000 twiss-0.2.6/.github/workflows/pypi.yaml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      805 2024-03-05 01:41:55.000000 twiss-0.2.6/.github/workflows/test.yaml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1799 2024-03-05 01:41:55.000000 twiss-0.2.6/.gitignore
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       97 2024-04-19 17:53:51.000000 twiss-0.2.6/.pre-commit-config.yaml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1069 2024-03-05 01:41:55.000000 twiss-0.2.6/LICENSE
+-rw-r--r--   0 imorozov  (1000) imorozov  (1000)     4129 2024-05-23 15:19:29.480618 twiss-0.2.6/PKG-INFO
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2530 2024-05-23 15:09:14.000000 twiss-0.2.6/README.MD
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2024-05-23 15:19:29.472618 twiss-0.2.6/docs/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      638 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/Makefile
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      804 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/make.bat
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2024-05-23 15:19:29.476618 twiss-0.2.6/docs/source/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1993 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/source/conf.py
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2024-05-23 15:19:29.476618 twiss-0.2.6/docs/source/examples/
+-rwxrwxr-x   0 imorozov  (1000) imorozov  (1000)   864937 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/source/examples/twiss.ipynb
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      568 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/source/index.rst
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2024-05-23 15:19:29.476618 twiss-0.2.6/docs/source/modules/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       43 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/source/modules/convert.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       49 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/source/modules/distribution.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       45 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/source/modules/invariant.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/source/modules/matrix.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/source/modules/normal.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       45 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/source/modules/transport.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/source/modules/util.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2024-03-05 01:41:55.000000 twiss-0.2.6/docs/source/modules/wolski.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1810 2024-04-19 17:53:41.000000 twiss-0.2.6/pyproject.toml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       38 2024-05-23 15:19:29.480618 twiss-0.2.6/setup.cfg
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2024-05-23 15:19:29.476618 twiss-0.2.6/twiss/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1560 2024-05-23 15:08:33.000000 twiss-0.2.6/twiss/__init__.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     4446 2024-03-05 01:41:55.000000 twiss-0.2.6/twiss/convert.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1420 2024-04-19 17:55:44.000000 twiss-0.2.6/twiss/distribution.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     3178 2024-03-05 01:41:55.000000 twiss-0.2.6/twiss/invariant.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     6680 2024-05-23 15:16:55.000000 twiss-0.2.6/twiss/matrix.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     6000 2024-03-05 01:41:55.000000 twiss-0.2.6/twiss/normal.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     6909 2024-03-05 01:41:55.000000 twiss-0.2.6/twiss/transport.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      692 2024-03-05 01:41:55.000000 twiss-0.2.6/twiss/util.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7574 2024-04-19 17:51:50.000000 twiss-0.2.6/twiss/wolski.py
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2024-05-23 15:19:29.476618 twiss-0.2.6/twiss.egg-info/
+-rw-r--r--   0 imorozov  (1000) imorozov  (1000)     4129 2024-05-23 15:19:29.000000 twiss-0.2.6/twiss.egg-info/PKG-INFO
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      842 2024-05-23 15:19:29.000000 twiss-0.2.6/twiss.egg-info/SOURCES.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        1 2024-05-23 15:19:29.000000 twiss-0.2.6/twiss.egg-info/dependency_links.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      234 2024-05-23 15:19:29.000000 twiss-0.2.6/twiss.egg-info/requires.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        6 2024-05-23 15:19:29.000000 twiss-0.2.6/twiss.egg-info/top_level.txt
```

### Comparing `twiss-0.2.5/.github/workflows/docs.yaml` & `twiss-0.2.6/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/.github/workflows/lint.yaml` & `twiss-0.2.6/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/.github/workflows/pypi.yaml` & `twiss-0.2.6/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/.github/workflows/test.yaml` & `twiss-0.2.6/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/.gitignore` & `twiss-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/LICENSE` & `twiss-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/PKG-INFO` & `twiss-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twiss
-Version: 0.2.5
+Version: 0.2.6
 Summary: Differentiable Wolski twiss matrices computation for arbitrary dimension stable symplectic matrices
 Author: Ivan Morozov
 License: MIT
 Project-URL: documentation, https://i-a-morozov.github.io/twiss/
 Project-URL: repository, https://github.com/i-a-morozov/twiss
 Keywords: torch,twiss,differentiable,symplectic,matrix
 Classifier: Development Status :: 4 - Beta
@@ -36,15 +36,15 @@
 Requires-Dist: pandas; extra == "examples"
 Requires-Dist: matplotlib; extra == "examples"
 Requires-Dist: seaborn; extra == "examples"
 Requires-Dist: ndmap; extra == "examples"
 Provides-Extra: all
 Requires-Dist: twiss[build,docs,examples,test]; extra == "all"
 
-# twiss, 2022-2023
+# twiss, 2022-2024
 
 Coupled twiss parameters (Wolski twiss matrices) computation for arbitrary even dimension.
 
 # Install & build
 
 ```
 $ pip install git+https://github.com/i-a-morozov/twiss.git@main
```

### Comparing `twiss-0.2.5/README.MD` & `twiss-0.2.6/README.MD`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# twiss, 2022-2023
+# twiss, 2022-2024
 
 Coupled twiss parameters (Wolski twiss matrices) computation for arbitrary even dimension.
 
 # Install & build
 
 ```
 $ pip install git+https://github.com/i-a-morozov/twiss.git@main
```

### Comparing `twiss-0.2.5/docs/Makefile` & `twiss-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/docs/make.bat` & `twiss-0.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/docs/source/conf.py` & `twiss-0.2.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/docs/source/examples/twiss.ipynb` & `twiss-0.2.6/docs/source/examples/twiss.ipynb`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/docs/source/index.rst` & `twiss-0.2.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/pyproject.toml` & `twiss-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/twiss/__init__.py` & `twiss-0.2.6/twiss/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Version and aliases
 
 """
-__version__ = '0.2.5'
+__version__ = '0.2.6'
 
 __all__ = [
     'symplectify',
     'is_symplectic',
+    'symplectic_conjugate',
     'rotation',
     'twiss',
     'is_stable',
     'propagate',
     'advance',
     'normal_to_wolski',
     'wolski_to_normal',
@@ -28,14 +29,15 @@
     'wolski_transport',
     'lb_transport',
     'cs_transport',
     'momenta',
     'normal'
 ]
 
+from twiss.matrix import symplectic_conjugate
 from twiss.matrix import symplectify
 from twiss.matrix import is_symplectic
 from twiss.matrix import rotation
 
 from twiss.wolski import twiss
 from twiss.wolski import is_stable
 from twiss.wolski import propagate
```

### Comparing `twiss-0.2.5/twiss/convert.py` & `twiss-0.2.6/twiss/convert.py`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/twiss/distribution.py` & `twiss-0.2.6/twiss/distribution.py`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/twiss/invariant.py` & `twiss-0.2.6/twiss/invariant.py`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/twiss/matrix.py` & `twiss-0.2.6/twiss/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,40 @@
             [ 0.,  0., -1.,  0.]], dtype=torch.float64)
 
     """
     block = symplectic_block(dtype=dtype, device=device)
     return torch.block_diag(*[block for _ in range(d)])
 
 
+def symplectic_conjugate(m:Tensor) -> Tensor:
+    """
+    Compute symplectic conjugate of a given input matrix
+
+    Parameters
+    ----------
+    m: Tensor, even-dimension
+        input matrix
+
+    Returns
+    -------
+    Tensor
+
+    Examples
+    --------
+    >> import torch
+    >> symplectic_conjugate(torch.tensor([[1.0, 0.1], [0.0, 1.0]], dtype=torch.float64))
+    tensor([[ 1.0000, -0.1000],
+            [ 0.0000,  1.0000]], dtype=torch.float64)
+
+    """
+    d = len(m) // 2
+    s = symplectic_identity(d, dtype=m.dtype, device=m.device)
+    return - s @ m.T @ s
+
+
 def symplectify(m:Tensor) -> Tensor:
     """
     Perform symplectification of a given input matrix
 
     Parameters
     ----------
     m: Tensor, even-dimension
```

### Comparing `twiss-0.2.5/twiss/normal.py` & `twiss-0.2.6/twiss/normal.py`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/twiss/transport.py` & `twiss-0.2.6/twiss/transport.py`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/twiss/util.py` & `twiss-0.2.6/twiss/util.py`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/twiss/wolski.py` & `twiss-0.2.6/twiss/wolski.py`

 * *Files identical despite different names*

### Comparing `twiss-0.2.5/twiss.egg-info/PKG-INFO` & `twiss-0.2.6/twiss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twiss
-Version: 0.2.5
+Version: 0.2.6
 Summary: Differentiable Wolski twiss matrices computation for arbitrary dimension stable symplectic matrices
 Author: Ivan Morozov
 License: MIT
 Project-URL: documentation, https://i-a-morozov.github.io/twiss/
 Project-URL: repository, https://github.com/i-a-morozov/twiss
 Keywords: torch,twiss,differentiable,symplectic,matrix
 Classifier: Development Status :: 4 - Beta
@@ -36,15 +36,15 @@
 Requires-Dist: pandas; extra == "examples"
 Requires-Dist: matplotlib; extra == "examples"
 Requires-Dist: seaborn; extra == "examples"
 Requires-Dist: ndmap; extra == "examples"
 Provides-Extra: all
 Requires-Dist: twiss[build,docs,examples,test]; extra == "all"
 
-# twiss, 2022-2023
+# twiss, 2022-2024
 
 Coupled twiss parameters (Wolski twiss matrices) computation for arbitrary even dimension.
 
 # Install & build
 
 ```
 $ pip install git+https://github.com/i-a-morozov/twiss.git@main
```

### Comparing `twiss-0.2.5/twiss.egg-info/SOURCES.txt` & `twiss-0.2.6/twiss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

