# Comparing `tmp/surface_construct-0.5.8.tar.gz` & `tmp/surface_construct-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surface_construct-0.5.8.tar", last modified: Thu Feb 29 13:50:09 2024, max compression
+gzip compressed data, was "surface_construct-0.5.9.tar", last modified: Sun Mar  3 11:32:49 2024, max compression
```

## Comparing `surface_construct-0.5.8.tar` & `surface_construct-0.5.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2024-02-29 13:50:09.357841 surface_construct-0.5.8/
--rwxrwxrwx   0 ren       (1000) ren       (1000)    35163 2022-02-12 15:31:24.000000 surface_construct-0.5.8/LICENSE
--rw-r--r--   0 ren       (1000) ren       (1000)      678 2024-02-29 13:50:09.357841 surface_construct-0.5.8/PKG-INFO
--rwxrwxrwx   0 ren       (1000) ren       (1000)     8329 2022-08-16 07:09:58.000000 surface_construct-0.5.8/README.md
--rw-rw-r--   0 ren       (1000) ren       (1000)       38 2024-02-29 13:50:09.357841 surface_construct-0.5.8/setup.cfg
--rwxrwxrwx   0 ren       (1000) ren       (1000)      792 2024-02-29 13:47:21.000000 surface_construct-0.5.8/setup.py
-drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2024-02-29 13:50:09.353841 surface_construct-0.5.8/surface_construct/
--rwxrwxrwx   0 ren       (1000) ren       (1000)      196 2022-02-14 13:01:56.000000 surface_construct-0.5.8/surface_construct/__init__.py
--rwxrwxrwx   0 ren       (1000) ren       (1000)    16789 2023-10-15 11:59:46.000000 surface_construct-0.5.8/surface_construct/atoms.py
--rw-rw-r--   0 ren       (1000) ren       (1000)    13838 2024-02-29 11:58:06.000000 surface_construct-0.5.8/surface_construct/db.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     1844 2024-02-29 11:58:06.000000 surface_construct-0.5.8/surface_construct/default_parameter.py
--rwxrwxrwx   0 ren       (1000) ren       (1000)    10767 2022-08-01 14:13:59.000000 surface_construct-0.5.8/surface_construct/sampling.py
--rwxrwxrwx   0 ren       (1000) ren       (1000)    18953 2023-03-19 05:08:54.000000 surface_construct-0.5.8/surface_construct/structure.py
--rwxrwxrwx   0 ren       (1000) ren       (1000)    26664 2022-05-29 11:21:07.000000 surface_construct-0.5.8/surface_construct/surface.py
--rw-rw-r--   0 ren       (1000) ren       (1000)    29916 2024-02-29 12:13:36.000000 surface_construct-0.5.8/surface_construct/surface_grid.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     1043 2023-09-04 14:47:01.000000 surface_construct-0.5.8/surface_construct/utils.py
-drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2024-02-29 13:50:09.353841 surface_construct-0.5.8/surface_construct.egg-info/
--rw-r--r--   0 ren       (1000) ren       (1000)      678 2024-02-29 13:50:09.000000 surface_construct-0.5.8/surface_construct.egg-info/PKG-INFO
--rwxrwxrwx   0 ren       (1000) ren       (1000)      557 2024-02-29 13:50:09.000000 surface_construct-0.5.8/surface_construct.egg-info/SOURCES.txt
--rwxrwxrwx   0 ren       (1000) ren       (1000)        1 2024-02-29 13:50:09.000000 surface_construct-0.5.8/surface_construct.egg-info/dependency_links.txt
--rwxrwxrwx   0 ren       (1000) ren       (1000)       68 2024-02-29 13:50:09.000000 surface_construct-0.5.8/surface_construct.egg-info/requires.txt
--rwxrwxrwx   0 ren       (1000) ren       (1000)       18 2024-02-29 13:50:09.000000 surface_construct-0.5.8/surface_construct.egg-info/top_level.txt
-drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2024-02-29 13:50:09.357841 surface_construct-0.5.8/tests/
--rwxrwxrwx   0 ren       (1000) ren       (1000)      922 2022-05-29 04:16:24.000000 surface_construct-0.5.8/tests/test_surface_grid.py
--rw-rw-r--   0 ren       (1000) ren       (1000)      460 2023-09-15 17:55:23.000000 surface_construct-0.5.8/tests/test_systematic_opt.py
+drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2024-03-03 11:32:49.825657 surface_construct-0.5.9/
+-rwxrwxrwx   0 ren       (1000) ren       (1000)    35163 2022-02-12 15:31:24.000000 surface_construct-0.5.9/LICENSE
+-rw-r--r--   0 ren       (1000) ren       (1000)     8841 2024-03-03 11:32:49.825657 surface_construct-0.5.9/PKG-INFO
+-rwxrwxrwx   0 ren       (1000) ren       (1000)     8376 2024-02-29 14:38:51.000000 surface_construct-0.5.9/README.md
+-rw-rw-r--   0 ren       (1000) ren       (1000)       38 2024-03-03 11:32:49.825657 surface_construct-0.5.9/setup.cfg
+-rwxrwxrwx   0 ren       (1000) ren       (1000)      972 2024-03-03 11:32:20.000000 surface_construct-0.5.9/setup.py
+drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2024-03-03 11:32:49.825657 surface_construct-0.5.9/surface_construct/
+-rwxrwxrwx   0 ren       (1000) ren       (1000)      196 2022-02-14 13:01:56.000000 surface_construct-0.5.9/surface_construct/__init__.py
+-rwxrwxrwx   0 ren       (1000) ren       (1000)    16789 2023-10-15 11:59:46.000000 surface_construct-0.5.9/surface_construct/atoms.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)    13838 2024-02-29 11:58:06.000000 surface_construct-0.5.9/surface_construct/db.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     1844 2024-02-29 11:58:06.000000 surface_construct-0.5.9/surface_construct/default_parameter.py
+-rwxrwxrwx   0 ren       (1000) ren       (1000)    10767 2022-08-01 14:13:59.000000 surface_construct-0.5.9/surface_construct/sampling.py
+-rwxrwxrwx   0 ren       (1000) ren       (1000)    18953 2023-03-19 05:08:54.000000 surface_construct-0.5.9/surface_construct/structure.py
+-rwxrwxrwx   0 ren       (1000) ren       (1000)    26664 2022-05-29 11:21:07.000000 surface_construct-0.5.9/surface_construct/surface.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)    29952 2024-03-03 11:22:07.000000 surface_construct-0.5.9/surface_construct/surface_grid.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     1043 2023-09-04 14:47:01.000000 surface_construct-0.5.9/surface_construct/utils.py
+drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2024-03-03 11:32:49.825657 surface_construct-0.5.9/surface_construct.egg-info/
+-rw-r--r--   0 ren       (1000) ren       (1000)     8841 2024-03-03 11:32:49.000000 surface_construct-0.5.9/surface_construct.egg-info/PKG-INFO
+-rwxrwxrwx   0 ren       (1000) ren       (1000)      557 2024-03-03 11:32:49.000000 surface_construct-0.5.9/surface_construct.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ren       (1000) ren       (1000)        1 2024-03-03 11:32:49.000000 surface_construct-0.5.9/surface_construct.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ren       (1000) ren       (1000)       68 2024-03-03 11:32:49.000000 surface_construct-0.5.9/surface_construct.egg-info/requires.txt
+-rwxrwxrwx   0 ren       (1000) ren       (1000)       18 2024-03-03 11:32:49.000000 surface_construct-0.5.9/surface_construct.egg-info/top_level.txt
+drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2024-03-03 11:32:49.825657 surface_construct-0.5.9/tests/
+-rwxrwxrwx   0 ren       (1000) ren       (1000)      922 2022-05-29 04:16:24.000000 surface_construct-0.5.9/tests/test_surface_grid.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)      460 2023-09-15 17:55:23.000000 surface_construct-0.5.9/tests/test_systematic_opt.py
```

### Comparing `surface_construct-0.5.8/LICENSE` & `surface_construct-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `surface_construct-0.5.8/README.md` & `surface_construct-0.5.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 
   ![stratified sampling](docs/stratified_sampling.jpg)
 
 * 吸附结构
 
   ![adsorption structure](docs/adsorption_structure.jpg)
 
+## 安装
 
+`pip install -U surface-construct`
 
 ## 使用方法 Manual
 
 ### 所需文件 Required Files
 
 * `surface_reaction_sample.py`: 主流程文件
```

### Comparing `surface_construct-0.5.8/setup.py` & `surface_construct-0.5.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from setuptools import setup
 
+with open("README.md", "r", encoding='utf-8') as f:
+    long_description = f.read()
+
 install_requires = [
     'ase',
     'networkx',
     'numpy',
     'spglib',
     'pandas',
     'tqdm',
     'matplotlib',
     'scipy',
     'scikit-learn',
 ]
 
 setup(
     name='surface_construct',
-    version='0.5.8',
+    version='0.5.9',
     packages=['surface_construct'],
     url='https://gitee.com/pjren/surface_construct/',
     license='GPL',
     author='ren',
     author_email='0403114076@163.com',
     description='Surface termination construction especially for complex model, such as oxides or carbides.',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     install_requires=install_requires,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `surface_construct-0.5.8/surface_construct/atoms.py` & `surface_construct-0.5.9/surface_construct/atoms.py`

 * *Files identical despite different names*

### Comparing `surface_construct-0.5.8/surface_construct/db.py` & `surface_construct-0.5.9/surface_construct/db.py`

 * *Files identical despite different names*

### Comparing `surface_construct-0.5.8/surface_construct/default_parameter.py` & `surface_construct-0.5.9/surface_construct/default_parameter.py`

 * *Files identical despite different names*

### Comparing `surface_construct-0.5.8/surface_construct/sampling.py` & `surface_construct-0.5.9/surface_construct/sampling.py`

 * *Files identical despite different names*

### Comparing `surface_construct-0.5.8/surface_construct/structure.py` & `surface_construct-0.5.9/surface_construct/structure.py`

 * *Files identical despite different names*

### Comparing `surface_construct-0.5.8/surface_construct/surface.py` & `surface_construct-0.5.9/surface_construct/surface.py`

 * *Files identical despite different names*

### Comparing `surface_construct-0.5.8/surface_construct/surface_grid.py` & `surface_construct-0.5.9/surface_construct/surface_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,16 @@
             grid_dist = np.take_along_axis(grid_dist, index_array, axis=-1)
             # grid_dist_array = np.take_along_axis(grid_dist_array, index_array, axis=-1)
             # 设定距离向量长度
             vlen = min(self.vlen, atomcount)
             r0 = self.rads + self.radii[atomnum]
             v = grid_dist[:, :vlen]
             kwargs.update({'r0': r0})
-            v_w = np.concatenate([wf(v, **kwargs), np.zeros((v.shape[0], self.vlen-vlen))], axis=1)
+            # v_w = np.concatenate([wf(v, **kwargs), np.zeros((v.shape[0], self.vlen-vlen))], axis=1)
+            v_w = wf(v, **kwargs)
             vector.append(v_w)
         vector = np.concatenate(vector, axis=1)
         self._raw_vector = vector
         if not pca:  # 用于 debug
             self._vector_dim = vector.shape[1]
             if return_vector:
                 return vector
```

### Comparing `surface_construct-0.5.8/surface_construct/utils.py` & `surface_construct-0.5.9/surface_construct/utils.py`

 * *Files identical despite different names*

### Comparing `surface_construct-0.5.8/surface_construct.egg-info/SOURCES.txt` & `surface_construct-0.5.9/surface_construct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `surface_construct-0.5.8/tests/test_surface_grid.py` & `surface_construct-0.5.9/tests/test_surface_grid.py`

 * *Files identical despite different names*

