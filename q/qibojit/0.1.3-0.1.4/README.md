# Comparing `tmp/qibojit-0.1.3.tar.gz` & `tmp/qibojit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibojit-0.1.3.tar", max compression
+gzip compressed data, was "qibojit-0.1.4.tar", max compression
```

## Comparing `qibojit-0.1.3.tar` & `qibojit-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2024-03-02 08:56:38.045294 qibojit-0.1.3/LICENSE
--rw-r--r--   0        0        0     1045 2024-03-02 08:56:38.045294 qibojit-0.1.3/README.md
--rw-r--r--   0        0        0     1367 2024-03-02 08:56:38.045294 qibojit-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       71 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/__init__.py
--rw-r--r--   0        0        0      109 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/backends/__init__.py
--rw-r--r--   0        0        0    12903 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/backends/clifford_operations_cpu.py
--rw-r--r--   0        0        0    26506 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/backends/clifford_operations_gpu.py
--rw-r--r--   0        0        0    12153 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/backends/cpu.py
--rw-r--r--   0        0        0    33143 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/backends/gpu.py
--rw-r--r--   0        0        0     2095 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/backends/matrices.py
--rw-r--r--   0        0        0        0 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/custom_operators/__init__.py
--rw-r--r--   0        0        0    19104 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/custom_operators/gates.py
--rw-r--r--   0        0        0     4922 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/custom_operators/ops.py
--rw-r--r--   0        0        0    15861 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/custom_operators/raw_kernels.py
--rw-r--r--   0        0        0        0 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/tests/__init__.py
--rw-r--r--   0        0        0      812 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/tests/conftest.py
--rw-r--r--   0        0        0     4241 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/tests/test_backends.py
--rw-r--r--   0        0        0    16331 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/tests/test_gates.py
--rw-r--r--   0        0        0     9202 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/tests/test_ops.py
--rw-r--r--   0        0        0      568 2024-03-02 08:56:38.049294 qibojit-0.1.3/src/qibojit/tests/utils.py
--rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 qibojit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 05:49:10.391207 qibojit-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1045 2024-05-23 05:49:10.391207 qibojit-0.1.4/README.md
+-rw-r--r--   0        0        0     1567 2024-05-23 05:49:10.391207 qibojit-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-05-23 05:49:10.391207 qibojit-0.1.4/src/qibojit/__init__.py
+-rw-r--r--   0        0        0     1450 2024-05-23 05:49:10.391207 qibojit-0.1.4/src/qibojit/backends/__init__.py
+-rw-r--r--   0        0        0    11754 2024-05-23 05:49:10.391207 qibojit-0.1.4/src/qibojit/backends/clifford_operations_cpu.py
+-rw-r--r--   0        0        0    28337 2024-05-23 05:49:10.391207 qibojit-0.1.4/src/qibojit/backends/clifford_operations_gpu.py
+-rw-r--r--   0        0        0    12153 2024-05-23 05:49:10.391207 qibojit-0.1.4/src/qibojit/backends/cpu.py
+-rw-r--r--   0        0        0    33244 2024-05-23 05:49:10.391207 qibojit-0.1.4/src/qibojit/backends/gpu.py
+-rw-r--r--   0        0        0     2158 2024-05-23 05:49:10.391207 qibojit-0.1.4/src/qibojit/backends/matrices.py
+-rw-r--r--   0        0        0        0 2024-05-23 05:49:10.395207 qibojit-0.1.4/src/qibojit/custom_operators/__init__.py
+-rw-r--r--   0        0        0    19104 2024-05-23 05:49:10.395207 qibojit-0.1.4/src/qibojit/custom_operators/gates.py
+-rw-r--r--   0        0        0     4958 2024-05-23 05:49:10.395207 qibojit-0.1.4/src/qibojit/custom_operators/ops.py
+-rw-r--r--   0        0        0    15861 2024-05-23 05:49:10.395207 qibojit-0.1.4/src/qibojit/custom_operators/raw_kernels.py
+-rw-r--r--   0        0        0        0 2024-05-23 05:49:10.395207 qibojit-0.1.4/src/qibojit/tests/__init__.py
+-rw-r--r--   0        0        0      812 2024-05-23 05:49:10.395207 qibojit-0.1.4/src/qibojit/tests/conftest.py
+-rw-r--r--   0        0        0     4477 2024-05-23 05:49:10.395207 qibojit-0.1.4/src/qibojit/tests/test_backends.py
+-rw-r--r--   0        0        0    16331 2024-05-23 05:49:10.395207 qibojit-0.1.4/src/qibojit/tests/test_gates.py
+-rw-r--r--   0        0        0     9202 2024-05-23 05:49:10.395207 qibojit-0.1.4/src/qibojit/tests/test_ops.py
+-rw-r--r--   0        0        0      568 2024-05-23 05:49:10.395207 qibojit-0.1.4/src/qibojit/tests/utils.py
+-rw-r--r--   0        0        0     2120 1970-01-01 00:00:00.000000 qibojit-0.1.4/PKG-INFO
```

### Comparing `qibojit-0.1.3/LICENSE` & `qibojit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qibojit-0.1.3/README.md` & `qibojit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `qibojit-0.1.3/pyproject.toml` & `qibojit-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qibojit"
-version = "0.1.3"
+version = "0.1.4"
 description = "Simulation tools based on numba and cupy."
 authors = ["The Qibo team"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://qibo.science"
 repository = "https://github.com/qiboteam/qibojit"
 documentation = "https://qibo.science/docs/qibo/stable"
@@ -16,45 +16,49 @@
 packages = [{ include = "qibojit", from = "src" }]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 
 [tool.poetry.dependencies]
-python=">=3.9.0,<3.12"
-numba=">=0.51.0"
-qibo=">=0.2.5"
+python = "^3.9,<3.13"
+numba = ">=0.59.0"
+qibo = ">=0.2.8"
 scipy = "^1.10.1"
 psutil = "^5.9.5"
+cupy-cuda12x = { version = "^13.1.0", optional = true }
+cuquantum-python-cu12 = { version = "^23.10.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^7.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
-pylint = "^2.17.4"
+pylint = "^3.0.3"
 pytest-cov = "^4.1.0"
 pytest-env = "^0.8.1"
 
+[tool.poetry.extras]
+cupy = ["cupy-cuda12x"]
+cuquantum = ["cuquantum-python-cu12"]
+
 [tool.poe.tasks]
 test = "pytest"
 lint = "pylint src/**/*.py -E"
 lint-warnings = "pylint src/**/*.py --exit-zero"
 
 [tool.pylint.master]
 output-format = "colorized"
 
 [tool.pylint.reports]
 output-format = "colorized"
 
 [tool.coverage.run]
-omit = [
-     "src/qibojit/backends/clifford_operations*",
-]
+omit = ["src/qibojit/backends/clifford_operations*"]
 
 [tool.pytest.ini_options]
 testpaths = ['src/qibojit/tests/']
 addopts = ['--cov=qibojit', '--cov-report=xml']
 env = ["D:NUMBA_DISABLE_JIT=1"]
```

### Comparing `qibojit-0.1.3/src/qibojit/backends/clifford_operations_cpu.py` & `qibojit-0.1.4/src/qibojit/backends/clifford_operations_cpu.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,182 +1,178 @@
 """Set of custom Numba operations for the Clifford backend."""
 
 import numpy as np
 from numba import njit, prange, uint64
 
+PARALLEL = False
 
-@njit("b1[:,:](b1[:,:], u8, u8)", parallel=True, cache=True)
+
+@njit("Tuple((u1[:], u1[:,:], u1[:,:]))(u1[:,:], u8)", parallel=PARALLEL, cache=True)
+def _get_rxz(symplectic_matrix, nqubits):
+    return (
+        symplectic_matrix[:, -1],
+        symplectic_matrix[:, :nqubits],
+        symplectic_matrix[:, nqubits:-1],
+    )
+
+
+@njit("u1[:,:](u1[:,:], u8, u8)", parallel=PARALLEL, cache=True)
 def H(symplectic_matrix, q, nqubits):
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = r[i] ^ (x[i, q] & z[i, q])
         tmp = symplectic_matrix[i, q]
         symplectic_matrix[i, q] = symplectic_matrix[i, nqubits + q]
         symplectic_matrix[i, nqubits + q] = tmp
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8, u8)", parallel=PARALLEL, cache=True)
 def CNOT(symplectic_matrix, control_q, target_q, nqubits):
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
 
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
-        symplectic_matrix[i, -1] = r[i] ^ (x[i, control_q] & z[i, target_q]) & (
+        r[i] = r[i] ^ (x[i, control_q] & z[i, target_q]) & (
             x[i, target_q] ^ ~z[i, control_q]
         )
-        symplectic_matrix[i, target_q] = x[i, target_q] ^ x[i, control_q]
-        symplectic_matrix[i, nqubits + control_q] = z[i, control_q] ^ z[i, target_q]
+        x[i, target_q] = x[i, target_q] ^ x[i, control_q]
+        z[i, control_q] = z[i, control_q] ^ z[i, target_q]
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8, u8)", parallel=PARALLEL, cache=True)
 def CZ(symplectic_matrix, control_q, target_q, nqubits):
     """Decomposition --> H-CNOT-H"""
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
 
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = (
             r[i]
             ^ (x[i, target_q] & z[i, target_q])
             ^ (x[i, control_q] & x[i, target_q] & (z[i, target_q] ^ ~z[i, control_q]))
             ^ (x[i, target_q] & (z[i, target_q] ^ x[i, control_q]))
         )
         z_control_q = x[i, target_q] ^ z[i, control_q]
         z_target_q = z[i, target_q] ^ x[i, control_q]
-        symplectic_matrix[i, nqubits + control_q] = z_control_q
-        symplectic_matrix[i, nqubits + target_q] = z_target_q
+        z[i, control_q] = z_control_q
+        z[i, target_q] = z_target_q
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8)", parallel=PARALLEL, cache=True)
 def S(symplectic_matrix, q, nqubits):
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = r[i] ^ (x[i, q] & z[i, q])
         symplectic_matrix[i, nqubits + q] = z[i, q] ^ x[i, q]
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8)", parallel=PARALLEL, cache=True)
 def Z(symplectic_matrix, q, nqubits):
     """Decomposition --> S-S"""
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = r[i] ^ (
             (x[i, q] & z[i, q]) ^ x[i, q] & (z[i, q] ^ x[i, q])
         )
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8)", parallel=PARALLEL, cache=True)
 def X(symplectic_matrix, q, nqubits):
     """Decomposition --> H-S-S-H"""
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = (
             r[i] ^ (z[i, q] & (z[i, q] ^ x[i, q])) ^ (z[i, q] & x[i, q])
         )
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8)", parallel=PARALLEL, cache=True)
 def Y(symplectic_matrix, q, nqubits):
     """Decomposition --> S-S-H-S-S-H"""
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = (
             r[i] ^ (z[i, q] & (z[i, q] ^ x[i, q])) ^ (x[i, q] & (z[i, q] ^ x[i, q]))
         )
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8)", parallel=PARALLEL, cache=True)
 def SX(symplectic_matrix, q, nqubits):
     """Decomposition --> H-S-H"""
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = r[i] ^ (z[i, q] & (z[i, q] ^ x[i, q]))
         symplectic_matrix[i, q] = z[i, q] ^ x[i, q]
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8)", parallel=PARALLEL, cache=True)
 def SDG(symplectic_matrix, q, nqubits):
     """Decomposition --> S-S-S"""
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = r[i] ^ (x[i, q] & (z[i, q] ^ x[i, q]))
         symplectic_matrix[i, nqubits + q] = z[i, q] ^ x[i, q]
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8)", parallel=PARALLEL, cache=True)
 def SXDG(symplectic_matrix, q, nqubits):
     """Decomposition --> H-S-S-S-H"""
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = r[i] ^ (z[i, q] & x[i, q])
         symplectic_matrix[i, q] = z[i, q] ^ x[i, q]
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8)", parallel=PARALLEL, cache=True)
 def RY_pi(symplectic_matrix, q, nqubits):
     """Decomposition --> H-S-S"""
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = r[i] ^ (x[i, q] & (z[i, q] ^ x[i, q]))
         zq = symplectic_matrix[i, nqubits + q]
         symplectic_matrix[i, nqubits + q] = symplectic_matrix[i, q]
         symplectic_matrix[i, q] = zq
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8)", parallel=PARALLEL, cache=True)
 def RY_3pi_2(symplectic_matrix, q, nqubits):
     """Decomposition --> H-S-S"""
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = r[i] ^ (z[i, q] & (z[i, q] ^ x[i, q]))
         zq = symplectic_matrix[i, nqubits + q]
         symplectic_matrix[i, nqubits + q] = symplectic_matrix[i, q]
         symplectic_matrix[i, q] = zq
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8, u8)", parallel=PARALLEL, cache=True)
 def SWAP(symplectic_matrix, control_q, target_q, nqubits):
     """Decomposition --> CNOT-CNOT-CNOT"""
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = (
             r[i]
             ^ (x[i, control_q] & z[i, target_q] & (x[i, target_q] ^ ~z[i, control_q]))
             ^ (
                 (x[i, target_q] ^ x[i, control_q])
                 & (z[i, target_q] ^ z[i, control_q])
@@ -195,20 +191,19 @@
         symplectic_matrix[i, control_q] = x_tq
         symplectic_matrix[i, target_q] = x_cq
         symplectic_matrix[i, nqubits + control_q] = z_tq
         symplectic_matrix[i, nqubits + target_q] = z_cq
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8, u8)", parallel=PARALLEL, cache=True)
 def iSWAP(symplectic_matrix, control_q, target_q, nqubits):
     """Decomposition --> H-CNOT-CNOT-H-S-S"""
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = (
             r[i]
             ^ (x[i, target_q] & z[i, target_q])
             ^ (x[i, control_q] & z[i, control_q])
             ^ (x[i, control_q] & (z[i, control_q] ^ x[i, control_q]))
             ^ (
@@ -229,20 +224,19 @@
         symplectic_matrix[i, nqubits + target_q] = z_target_q
         tmp = symplectic_matrix[i, control_q]
         symplectic_matrix[i, control_q] = symplectic_matrix[i, target_q]
         symplectic_matrix[i, target_q] = tmp
     return symplectic_matrix
 
 
-@njit("b1[:,:](b1[:,:], u8, u8, u8)", parallel=True, cache=True)
+@njit("u1[:,:](u1[:,:], u8, u8, u8)", parallel=PARALLEL, cache=True)
 def CY(symplectic_matrix, control_q, target_q, nqubits):
     """Decomposition --> S-CNOT-SDG"""
-    r = symplectic_matrix[:-1, -1]
-    x = symplectic_matrix[:-1, :nqubits]
-    z = symplectic_matrix[:-1, nqubits:-1]
+    r, x, z = _get_rxz(symplectic_matrix, nqubits)
+
     for i in prange(symplectic_matrix.shape[0]):  # pylint: disable=not-an-iterable
         symplectic_matrix[i, -1] = (
             r[i]
             ^ (x[i, target_q] & (z[i, target_q] ^ x[i, target_q]))
             ^ (
                 x[i, control_q]
                 & (x[i, target_q] ^ z[i, target_q])
@@ -257,41 +251,34 @@
         symplectic_matrix[i, nqubits + control_q] = z_control_q
         symplectic_matrix[i, nqubits + target_q] = z_target_q
     return symplectic_matrix
 
 
 @njit(
     [
-        "b1[:,:](b1[:,:], u8[:], u8[:], u8, b1)",
-        "b1[:,:](b1[:,:], u4[:], u4[:], u4, b1)",
+        "u1[:,:](u1[:,:], u8[:], u8[:], u8, b1)",
+        "u1[:,:](u1[:,:], u4[:], u4[:], u4, b1)",
     ],
-    parallel=True,
+    parallel=PARALLEL,
     cache=True,
     fastmath=True,
 )
 def _rowsum(symplectic_matrix, h, i, nqubits, determined=False):
-    xi, xh = symplectic_matrix[i, :nqubits], symplectic_matrix[h, :nqubits]
-    zi, zh = symplectic_matrix[i, nqubits:-1], symplectic_matrix[h, nqubits:-1]
+    xi, zi = symplectic_matrix[i, :nqubits], symplectic_matrix[i, nqubits:-1]
+    xh, zh = symplectic_matrix[h, :nqubits], symplectic_matrix[h, nqubits:-1]
     if determined:
-        g_r = np.array([False for _ in range(h.shape[0])])
+        g_r = np.zeros(h.shape[0], dtype=np.uint8)
         g_xi_xh = xi.copy()
         g_zi_zh = xi.copy()
     for j in prange(len(h)):  # pylint: disable=not-an-iterable
-        exp = np.zeros(nqubits, dtype=uint64)
-        x1_eq_z1 = (xi[j] ^ zi[j]) == False
-        x1_neq_z1 = ~x1_eq_z1
-        x1_eq_0 = xi[j] == False
-        x1_eq_1 = ~x1_eq_0
-        ind2 = x1_eq_z1 & x1_eq_1
-        ind3 = x1_eq_1 & x1_neq_z1
-        ind4 = x1_eq_0 & x1_neq_z1
-        exp[ind2] = zh[j, ind2].astype(uint64) - xh[j, ind2].astype(uint64)
-        exp[ind3] = zh[j, ind3].astype(uint64) * (2 * xh[j, ind3].astype(uint64) - 1)
-        exp[ind4] = xh[j, ind4].astype(uint64) * (1 - 2 * zh[j, ind4].astype(uint64))
-
+        exp = (
+            2 * (xi[j] * xh[j] * (zh[j] - zi[j]) + zi[j] * zh[j] * (xi[j] - xh[j]))
+            - xi[j] * zh[j]
+            + xh[j] * zi[j]
+        )
         r = (
             2 * symplectic_matrix[h[j], -1]
             + 2 * symplectic_matrix[i[j], -1]
             + np.sum(exp)
         ) % 4 != 0
         xi_xh = xi[j] ^ xh[j]
         zi_zh = zi[j] ^ zh[j]
```

### Comparing `qibojit-0.1.3/src/qibojit/backends/cpu.py` & `qibojit-0.1.4/src/qibojit/backends/cpu.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.1.3/src/qibojit/backends/gpu.py` & `qibojit-0.1.4/src/qibojit/backends/gpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,17 +498,20 @@
         else:
             return self.cp.linalg.eigh(matrix)
 
     def calculate_matrix_exp(self, a, matrix, eigenvectors=None, eigenvalues=None):
         if eigenvectors is None or self.issparse(matrix):
             if self.issparse(matrix):
                 from scipy.sparse.linalg import expm
+
+                return self.cast(expm(-1j * a * matrix.get()))
             else:
-                from scipy.linalg import expm
-            return self.cast(expm(-1j * a * matrix.get()))
+                from cupyx.scipy.linalg import expm  # pylint: disable=import-error
+
+                return self.cast(expm(-1j * a * matrix))
         else:
             expd = self.cp.diag(self.cp.exp(-1j * a * eigenvalues))
             ud = self.cp.transpose(self.cp.conj(eigenvectors))
             return self.cp.matmul(eigenvectors, self.cp.matmul(expd, ud))
 
 
 class CuQuantumBackend(CupyBackend):  # pragma: no cover
```

### Comparing `qibojit-0.1.3/src/qibojit/backends/matrices.py` & `qibojit-0.1.4/src/qibojit/backends/matrices.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,18 @@
     def CU3(self, theta, phi, lam):
         return self.U3(theta, phi, lam)
 
     @cached_property
     def TOFFOLI(self):
         return self.X
 
+    @cached_property
+    def CCZ(self):
+        return self.Z
+
     def DEUTSCH(self, theta):
         return 1j * self.RX(2 * theta)
 
 
 class CustomMatrices(CuQuantumMatrices):
     # These matrices are used by the custom operators and may
     # not correspond to the mathematical representation of each gate
```

### Comparing `qibojit-0.1.3/src/qibojit/custom_operators/gates.py` & `qibojit-0.1.4/src/qibojit/custom_operators/gates.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.1.3/src/qibojit/custom_operators/ops.py` & `qibojit-0.1.4/src/qibojit/custom_operators/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,18 +105,19 @@
     np.random.seed(seed)
     thread_seed = [np.random.randint(0, int(1e8)) for _ in range(nthreads)]
 
     thread_frequencies = np.zeros(shape=(nthreads, nstates), dtype=frequencies.dtype)
     for n in prange(nthreads):  # pylint: disable=not-an-iterable
         frequencies_private = thread_frequencies[n]
         np.random.seed(thread_seed[n])
+        shot = probs.argmax()
         for i in range(thread_nshots[n]):
-            if i == 0:
-                # Initial bitstring is the one with the maximum probability
-                shot = probs.argmax()
+            # if i == 0:
+            #     # Initial bitstring is the one with the maximum probability
+            #     shot = probs.argmax()
             new_shot = (shot + np.random.randint(0, nstates)) % nstates
             # accept or reject move
             if probs[new_shot] / probs[shot] > np.random.random():
                 shot = new_shot
             # update frequencies
             frequencies_private[shot] += 1
     frequencies += thread_frequencies.sum(axis=0)
```

### Comparing `qibojit-0.1.3/src/qibojit/custom_operators/raw_kernels.py` & `qibojit-0.1.4/src/qibojit/custom_operators/raw_kernels.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.1.3/src/qibojit/tests/conftest.py` & `qibojit-0.1.4/src/qibojit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.1.3/src/qibojit/tests/test_backends.py` & `qibojit-0.1.4/src/qibojit/tests/test_backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 import pytest
 
+from qibojit.backends import MetaBackend
+
 
 def test_device_setter(backend):
     if backend.platform == "numba":
         device = "/CPU:0"
     else:  # pragma: no cover
         # CI does not have GPUs
         device = "/GPU:0"
@@ -110,7 +112,12 @@
     ham = hamiltonians.TFIM(6, h=1.0, backend=backend)
     m = getattr(sparse, f"{sparse_type}_matrix")(backend.to_numpy(ham.matrix))
     eigvals1, eigvecs1 = backend.calculate_eigenvectors(backend.cast(m), k)
     eigvals2, eigvecs2 = eigsh(m, k, which="SA")
     eigvals1 = backend.to_numpy(eigvals1)
     eigvals2 = backend.to_numpy(eigvals2)
     backend.assert_allclose(sorted(eigvals1), sorted(eigvals2))
+
+
+def test_metabackend_list_available():
+    available_backends = dict(zip(("numba", "cupy", "cuquantum"), (True, False, False)))
+    assert MetaBackend().list_available() == available_backends
```

### Comparing `qibojit-0.1.3/src/qibojit/tests/test_gates.py` & `qibojit-0.1.4/src/qibojit/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.1.3/src/qibojit/tests/test_ops.py` & `qibojit-0.1.4/src/qibojit/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.1.3/src/qibojit/tests/utils.py` & `qibojit-0.1.4/src/qibojit/tests/utils.py`

 * *Files identical despite different names*

### Comparing `qibojit-0.1.3/PKG-INFO` & `qibojit-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: qibojit
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simulation tools based on numba and cupy.
 Home-page: https://qibo.science
 License: Apache-2.0
 Author: The Qibo team
-Requires-Python: >=3.9.0,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: numba (>=0.51.0)
+Provides-Extra: cupy
+Provides-Extra: cuquantum
+Requires-Dist: cupy-cuda12x (>=13.1.0,<14.0.0) ; extra == "cupy"
+Requires-Dist: cuquantum-python-cu12 (>=23.10.0,<24.0.0) ; extra == "cuquantum"
+Requires-Dist: numba (>=0.59.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
-Requires-Dist: qibo (>=0.2.5)
+Requires-Dist: qibo (>=0.2.8)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Project-URL: Documentation, https://qibo.science/docs/qibo/stable
 Project-URL: Repository, https://github.com/qiboteam/qibojit
 Description-Content-Type: text/markdown
 
 # qibojit
```

