# Comparing `tmp/dynabench-0.3.1.tar.gz` & `tmp/dynabench-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynabench-0.3.1.tar", max compression
+gzip compressed data, was "dynabench-0.3.2.tar", max compression
```

## Comparing `dynabench-0.3.1.tar` & `dynabench-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,17 @@
--rw-r--r--   0        0        0     1074 2024-05-03 10:30:50.861280 dynabench-0.3.1/LICENCE
--rw-r--r--   0        0        0    18657 2024-05-03 10:30:50.861280 dynabench-0.3.1/LICENCE_data
--rw-r--r--   0        0        0    11415 2024-05-03 10:30:50.861280 dynabench-0.3.1/README.md
--rw-r--r--   0        0        0     1054 2024-05-06 19:10:28.406476 dynabench-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      131 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/_init_.py
--rw-r--r--   0        0        0      266 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/dataset/__init__.py
--rw-r--r--   0        0        0      504 2024-05-03 10:42:03.414598 dynabench-0.3.1/src/dynabench/dataset/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8924 2024-05-03 10:42:03.417931 dynabench-0.3.1/src/dynabench/dataset/__pycache__/_download.cpython-311.pyc
--rw-r--r--   0        0        0     5826 2024-05-03 10:42:03.431264 dynabench-0.3.1/src/dynabench/dataset/__pycache__/_iterator.cpython-311.pyc
--rw-r--r--   0        0        0     4744 2024-05-03 10:42:03.601265 dynabench-0.3.1/src/dynabench/dataset/__pycache__/_simulation_iterator.cpython-311.pyc
--rw-r--r--   0        0        0     6087 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/dataset/_download.py
--rw-r--r--   0        0        0     3119 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/dataset/_iterator.py
--rw-r--r--   0        0        0     2466 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/dataset/_simulation_iterator.py
--rw-r--r--   0        0        0      201 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/equation/__init__.py
--rw-r--r--   0        0        0      457 2024-05-03 10:42:03.607931 dynabench-0.3.1/src/dynabench/equation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2061 2024-05-03 10:42:03.607931 dynabench-0.3.1/src/dynabench/equation/__pycache__/_advection.cpython-311.pyc
--rw-r--r--   0        0        0     2662 2024-05-03 10:42:03.607931 dynabench-0.3.1/src/dynabench/equation/__pycache__/_base.cpython-311.pyc
--rw-r--r--   0        0        0     1224 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/equation/_advection.py
--rw-r--r--   0        0        0     1456 2024-05-03 10:30:50.887947 dynabench-0.3.1/src/dynabench/equation/_base.py
--rw-r--r--   0        0        0      212 2024-05-03 14:26:34.974287 dynabench-0.3.1/src/dynabench/model/__init__.py
--rw-r--r--   0        0        0      492 2024-05-03 14:28:35.757618 dynabench-0.3.1/src/dynabench/model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      357 2024-05-03 10:42:03.621265 dynabench-0.3.1/src/dynabench/model/_grid/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4029 2024-05-06 17:33:04.099867 dynabench-0.3.1/src/dynabench/model/_grid/__pycache__/cnn.cpython-311.pyc
--rw-r--r--   0        0        0     4149 2024-05-06 19:11:02.933142 dynabench-0.3.1/src/dynabench/model/_grid/__pycache__/neuralpde.cpython-311.pyc
--rw-r--r--   0        0        0     9525 2024-05-06 17:33:04.099867 dynabench-0.3.1/src/dynabench/model/_grid/__pycache__/resnet.cpython-311.pyc
--rw-r--r--   0        0        0     2600 2024-05-06 17:33:00.063201 dynabench-0.3.1/src/dynabench/model/_grid/cnn.py
--rw-r--r--   0        0        0     2851 2024-05-06 19:04:54.813145 dynabench-0.3.1/src/dynabench/model/_grid/neuralpde.py
--rwxr-xr-x   0        0        0     7407 2024-05-06 17:32:52.209867 dynabench-0.3.1/src/dynabench/model/_grid/resnet.py
--rw-r--r--   0        0        0    12209 1970-01-01 00:00:00.000000 dynabench-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-23 12:33:31.260630 dynabench-0.3.2/LICENCE
+-rw-r--r--   0        0        0    18657 2024-05-23 12:33:31.260630 dynabench-0.3.2/LICENCE_data
+-rw-r--r--   0        0        0    11415 2024-05-23 12:33:43.580575 dynabench-0.3.2/README.md
+-rw-r--r--   0        0        0     1054 2024-05-23 20:03:50.763083 dynabench-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-05-23 12:33:43.723907 dynabench-0.3.2/src/dynabench/_init_.py
+-rw-r--r--   0        0        0      266 2024-05-23 12:33:43.727241 dynabench-0.3.2/src/dynabench/dataset/__init__.py
+-rw-r--r--   0        0        0     6087 2024-05-23 12:33:43.727241 dynabench-0.3.2/src/dynabench/dataset/_download.py
+-rw-r--r--   0        0        0     3119 2024-05-23 12:33:43.727241 dynabench-0.3.2/src/dynabench/dataset/_iterator.py
+-rw-r--r--   0        0        0     2466 2024-05-23 12:33:43.727241 dynabench-0.3.2/src/dynabench/dataset/_simulation_iterator.py
+-rw-r--r--   0        0        0      201 2024-05-23 12:33:43.727241 dynabench-0.3.2/src/dynabench/equation/__init__.py
+-rw-r--r--   0        0        0     1224 2024-05-23 12:33:43.727241 dynabench-0.3.2/src/dynabench/equation/_advection.py
+-rw-r--r--   0        0        0     1456 2024-05-23 12:33:43.727241 dynabench-0.3.2/src/dynabench/equation/_base.py
+-rw-r--r--   0        0        0      212 2024-05-23 12:33:43.727241 dynabench-0.3.2/src/dynabench/model/__init__.py
+-rw-r--r--   0        0        0     2615 2024-05-23 20:01:46.387699 dynabench-0.3.2/src/dynabench/model/_grid/cnn.py
+-rw-r--r--   0        0        0     2922 2024-05-23 20:01:46.391032 dynabench-0.3.2/src/dynabench/model/_grid/neuralpde.py
+-rwxr-xr-x   0        0        0     7407 2024-05-23 12:33:43.727241 dynabench-0.3.2/src/dynabench/model/_grid/resnet.py
+-rw-r--r--   0        0        0    12209 1970-01-01 00:00:00.000000 dynabench-0.3.2/PKG-INFO
```

### Comparing `dynabench-0.3.1/LICENCE` & `dynabench-0.3.2/LICENCE`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.1/LICENCE_data` & `dynabench-0.3.2/LICENCE_data`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.1/README.md` & `dynabench-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.1/pyproject.toml` & `dynabench-0.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dynabench"
-version = "0.3.1"
+version = "0.3.2"
 description = "Benchmark dataset for learning dynamical systems from data"
 authors = ["Andrzej Dulny <andzej.dulny@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://dynabench.github.io/about.html"
 documentation = "https://dynabench.github.io/"
 repository = "https://github.com/badulion/dynabench/"
```

### Comparing `dynabench-0.3.1/src/dynabench/dataset/_download.py` & `dynabench-0.3.2/src/dynabench/dataset/_download.py`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.1/src/dynabench/dataset/_iterator.py` & `dynabench-0.3.2/src/dynabench/dataset/_iterator.py`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.1/src/dynabench/dataset/_simulation_iterator.py` & `dynabench-0.3.2/src/dynabench/dataset/_simulation_iterator.py`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.1/src/dynabench/equation/_advection.py` & `dynabench-0.3.2/src/dynabench/equation/_advection.py`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.1/src/dynabench/equation/_base.py` & `dynabench-0.3.2/src/dynabench/equation/_base.py`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.1/src/dynabench/model/_grid/cnn.py` & `dynabench-0.3.2/src/dynabench/model/_grid/cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                  hidden_channels: int = 64,
                  padding: int | str | Tuple[int] = 'same',
                  padding_mode: str = 'circular',
                  kernel_size: int = 3,
                  activation: str = 'ReLU'):
         super().__init__()
         self.input_layer = nn.Conv2d(input_size, hidden_channels, kernel_size, padding=padding, padding_mode=padding_mode)
-        self.hidden_layers = [nn.Conv2d(hidden_channels, hidden_channels, kernel_size, padding=padding, padding_mode=padding_mode) for _ in range(hidden_layers)]
+        self.hidden_layers = nn.ModuleList([nn.Conv2d(hidden_channels, hidden_channels, kernel_size, padding=padding, padding_mode=padding_mode) for _ in range(hidden_layers)])
         self.output_layer = nn.Conv2d(hidden_channels, output_size, kernel_size, padding=padding, padding_mode=padding_mode)
             
         self.activation = getattr(nn, activation)()  
 
     def forward(self, x: torch.Tensor):
         """
             Forward pass of the model. Should not be called directly, instead call the model instance.
```

### Comparing `dynabench-0.3.1/src/dynabench/model/_grid/neuralpde.py` & `dynabench-0.3.2/src/dynabench/model/_grid/neuralpde.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,16 +61,18 @@
                 Input tensor of shape (batch_size, input_size, height, width).
             t_eval : List[float], default [0.0, 1.0]
                 List of times to evaluate the ODE solver at. Default is [0.0, 1.0].
 
             Returns
             -------
             torch.Tensor
-                Output tensor of shape (batch_size, output_size, height, width).
+                Output tensor of shape (batch_size, rollout, output_size, height, width).
         """
 
         t_eval = torch.tensor(t_eval, dtype=x.dtype, device=x.device)
         if self.use_adjoint:
-            return odeint_adjoint(self._ode, x, t_eval, **self.solver, adjoint_params=self.cnn.parameters())[1:]
+            pred = odeint_adjoint(self._ode, x, t_eval, **self.solver, adjoint_params=self.cnn.parameters())[1:]
         else:
-            return odeint(self._ode, x, t_eval, **self.solver)[1:]
+            pred =  odeint(self._ode, x, t_eval, **self.solver)[1:]
         
+        pred = torch.swapaxes(pred, 0, 1)
+        return pred
```

### Comparing `dynabench-0.3.1/src/dynabench/model/_grid/resnet.py` & `dynabench-0.3.2/src/dynabench/model/_grid/resnet.py`

 * *Files identical despite different names*

### Comparing `dynabench-0.3.1/PKG-INFO` & `dynabench-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynabench
-Version: 0.3.1
+Version: 0.3.2
 Summary: Benchmark dataset for learning dynamical systems from data
 Home-page: https://dynabench.github.io/about.html
 License: MIT
 Author: Andrzej Dulny
 Author-email: andzej.dulny@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

