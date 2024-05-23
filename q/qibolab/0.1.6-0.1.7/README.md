# Comparing `tmp/qibolab-0.1.6.tar.gz` & `tmp/qibolab-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibolab-0.1.6.tar", max compression
+gzip compressed data, was "qibolab-0.1.7.tar", max compression
```

## Comparing `qibolab-0.1.6.tar` & `qibolab-0.1.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    11357 2024-03-29 09:35:05.829734 qibolab-0.1.6/LICENSE
--rw-r--r--   0        0        0     3144 2024-03-29 09:35:05.829734 qibolab-0.1.6/README.md
--rw-r--r--   0        0        0     2802 2024-03-29 09:35:05.857734 qibolab-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2463 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/__init__.py
--rw-r--r--   0        0        0     6638 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/backends.py
--rw-r--r--   0        0        0     5034 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/channels.py
--rw-r--r--   0        0        0       48 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/compilers/__init__.py
--rw-r--r--   0        0        0     6023 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/compilers/compiler.py
--rw-r--r--   0        0        0     2932 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/compilers/default.py
--rw-r--r--   0        0        0     1526 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/couplers.py
--rw-r--r--   0        0        0       35 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/dummy/__init__.py
--rw-r--r--   0        0        0       22 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/dummy/kernels.npz
--rw-r--r--   0        0        0    22145 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/dummy/parameters.json
--rw-r--r--   0        0        0     2996 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/dummy/platform.py
--rw-r--r--   0        0        0     2276 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/execution_parameters.py
--rw-r--r--   0        0        0        0 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/instruments/__init__.py
--rw-r--r--   0        0        0     3487 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/instruments/abstract.py
--rw-r--r--   0        0        0     2352 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/instruments/bluefors.py
--rw-r--r--   0        0        0     4563 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/instruments/dummy.py
--rw-r--r--   0        0        0     4690 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/instruments/erasynth.py
--rw-r--r--   0        0        0     1030 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/instruments/icarusq.py
--rw-r--r--   0        0        0    15702 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/instruments/icarusqfpga.py
--rw-r--r--   0        0        0     4521 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/instruments/oscillator.py
--rw-r--r--   0        0        0     1251 2024-03-29 09:35:05.857734 qibolab-0.1.6/src/qibolab/instruments/port.py
--rw-r--r--   0        0        0        0 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qblox/__init__.py
--rw-r--r--   0        0        0     4842 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qblox/acquisition.py
--rw-r--r--   0        0        0    37313 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qblox/cluster_qcm_bb.py
--rw-r--r--   0        0        0    38067 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qblox/cluster_qcm_rf.py
--rw-r--r--   0        0        0    53345 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qblox/cluster_qrm_rf.py
--rw-r--r--   0        0        0    22513 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qblox/controller.py
--rw-r--r--   0        0        0     2409 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qblox/debug.py
--rw-r--r--   0        0        0     2373 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qblox/module.py
--rw-r--r--   0        0        0     9890 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qblox/port.py
--rw-r--r--   0        0        0    12582 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qblox/q1asm.py
--rw-r--r--   0        0        0    10720 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qblox/sequencer.py
--rw-r--r--   0        0        0    17588 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qblox/sweeper.py
--rw-r--r--   0        0        0       74 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qm/__init__.py
--rw-r--r--   0        0        0    10002 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qm/acquisition.py
--rw-r--r--   0        0        0    15236 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qm/config.py
--rw-r--r--   0        0        0    14801 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qm/controller.py
--rw-r--r--   0        0        0     4030 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qm/devices.py
--rw-r--r--   0        0        0     5067 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qm/ports.py
--rw-r--r--   0        0        0    10157 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qm/sequence.py
--rw-r--r--   0        0        0     8062 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/qm/sweepers.py
--rw-r--r--   0        0        0       66 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/rfsoc/__init__.py
--rw-r--r--   0        0        0     7321 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/rfsoc/convert.py
--rw-r--r--   0        0        0    22176 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/rfsoc/driver.py
--rw-r--r--   0        0        0      561 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/rohde_schwarz.py
--rw-r--r--   0        0        0      171 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/zhinst/__init__.py
--rw-r--r--   0        0        0    29485 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/zhinst/executor.py
--rw-r--r--   0        0        0     3790 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/zhinst/pulse.py
--rw-r--r--   0        0        0     7500 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/zhinst/sweep.py
--rw-r--r--   0        0        0      846 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/instruments/zhinst/util.py
--rw-r--r--   0        0        0     1092 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/kernels.py
--rw-r--r--   0        0        0    12326 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/native.py
--rw-r--r--   0        0        0    15944 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/platform.py
--rw-r--r--   0        0        0    57357 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/pulses.py
--rw-r--r--   0        0        0     5208 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/qubits.py
--rw-r--r--   0        0        0     5589 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/result.py
--rw-r--r--   0        0        0     8492 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/serialize.py
--rw-r--r--   0        0        0     4088 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/sweeper.py
--rw-r--r--   0        0        0     2656 2024-03-29 09:35:05.861734 qibolab-0.1.6/src/qibolab/unrolling.py
--rw-r--r--   0        0        0     4654 1970-01-01 00:00:00.000000 qibolab-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 08:22:19.654842 qibolab-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3144 2024-05-23 08:22:19.654842 qibolab-0.1.7/README.md
+-rw-r--r--   0        0        0     2802 2024-05-23 08:22:19.682842 qibolab-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3505 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/__init__.py
+-rw-r--r--   0        0        0     5814 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/backends.py
+-rw-r--r--   0        0        0     5034 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/channels.py
+-rw-r--r--   0        0        0       48 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/compilers/__init__.py
+-rw-r--r--   0        0        0     6023 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/compilers/compiler.py
+-rw-r--r--   0        0        0     2932 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/compilers/default.py
+-rw-r--r--   0        0        0     1526 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/couplers.py
+-rw-r--r--   0        0        0       35 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/dummy/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/dummy/kernels.npz
+-rw-r--r--   0        0        0    22145 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/dummy/parameters.json
+-rw-r--r--   0        0        0     2996 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/dummy/platform.py
+-rw-r--r--   0        0        0     2276 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/execution_parameters.py
+-rw-r--r--   0        0        0        0 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/__init__.py
+-rw-r--r--   0        0        0     3487 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/abstract.py
+-rw-r--r--   0        0        0     2352 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/bluefors.py
+-rw-r--r--   0        0        0     4563 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/dummy.py
+-rw-r--r--   0        0        0     4690 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/erasynth.py
+-rw-r--r--   0        0        0     1030 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/icarusq.py
+-rw-r--r--   0        0        0    15702 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/icarusqfpga.py
+-rw-r--r--   0        0        0     4521 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/oscillator.py
+-rw-r--r--   0        0        0     1251 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/port.py
+-rw-r--r--   0        0        0        0 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/qblox/__init__.py
+-rw-r--r--   0        0        0     4842 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/qblox/acquisition.py
+-rw-r--r--   0        0        0    37359 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/qblox/cluster_qcm_bb.py
+-rw-r--r--   0        0        0    38112 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/qblox/cluster_qcm_rf.py
+-rw-r--r--   0        0        0    53408 2024-05-23 08:22:19.682842 qibolab-0.1.7/src/qibolab/instruments/qblox/cluster_qrm_rf.py
+-rw-r--r--   0        0        0    23199 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qblox/controller.py
+-rw-r--r--   0        0        0     2409 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qblox/debug.py
+-rw-r--r--   0        0        0     2373 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qblox/module.py
+-rw-r--r--   0        0        0     9890 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qblox/port.py
+-rw-r--r--   0        0        0    12582 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qblox/q1asm.py
+-rw-r--r--   0        0        0    10720 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qblox/sequencer.py
+-rw-r--r--   0        0        0    17588 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qblox/sweeper.py
+-rw-r--r--   0        0        0       74 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qm/__init__.py
+-rw-r--r--   0        0        0    10035 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qm/acquisition.py
+-rw-r--r--   0        0        0    15757 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qm/config.py
+-rw-r--r--   0        0        0    14838 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qm/controller.py
+-rw-r--r--   0        0        0     4030 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qm/devices.py
+-rw-r--r--   0        0        0     5957 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qm/ports.py
+-rw-r--r--   0        0        0    10189 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qm/sequence.py
+-rw-r--r--   0        0        0     8062 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/qm/sweepers.py
+-rw-r--r--   0        0        0       66 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/rfsoc/__init__.py
+-rw-r--r--   0        0        0     7320 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/rfsoc/convert.py
+-rw-r--r--   0        0        0    23517 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/rfsoc/driver.py
+-rw-r--r--   0        0        0      561 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/rohde_schwarz.py
+-rw-r--r--   0        0        0      171 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/zhinst/__init__.py
+-rw-r--r--   0        0        0    29485 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/zhinst/executor.py
+-rw-r--r--   0        0        0     3790 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/zhinst/pulse.py
+-rw-r--r--   0        0        0     7500 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/zhinst/sweep.py
+-rw-r--r--   0        0        0      846 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/instruments/zhinst/util.py
+-rw-r--r--   0        0        0     1092 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/kernels.py
+-rw-r--r--   0        0        0    12326 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/native.py
+-rw-r--r--   0        0        0    15944 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/platform.py
+-rw-r--r--   0        0        0    57326 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/pulses.py
+-rw-r--r--   0        0        0     5246 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/qubits.py
+-rw-r--r--   0        0        0     6187 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/result.py
+-rw-r--r--   0        0        0     8492 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/serialize.py
+-rw-r--r--   0        0        0     4088 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/sweeper.py
+-rw-r--r--   0        0        0     2656 2024-05-23 08:22:19.686842 qibolab-0.1.7/src/qibolab/unrolling.py
+-rw-r--r--   0        0        0     4654 1970-01-01 00:00:00.000000 qibolab-0.1.7/PKG-INFO
```

### Comparing `qibolab-0.1.6/LICENSE` & `qibolab-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/README.md` & `qibolab-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/pyproject.toml` & `qibolab-0.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qibolab"
-version = "0.1.6"
+version = "0.1.7"
 description = "Quantum hardware module and drivers for Qibo"
 authors = ["The Qibo team"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://qibo.science/"
 repository = "https://github.com/qiboteam/qibolab/"
 documentation = "https://qibo.science/docs/qibolab/stable"
@@ -22,23 +22,23 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 qibo = ">=0.2.6"
 networkx = "^3.0"
 numpy = "^1.26.4"
 more-itertools = "^9.1.0"
-qblox-instruments = { version = "0.11.0", optional = true }
+qblox-instruments = { version = "0.12.0", optional = true }
 qcodes = { version = "^0.37.0", optional = true }
 qcodes_contrib_drivers = { version = "0.18.0", optional = true }
 pyvisa-py = { version = "0.5.3", optional = true }
 qm-qua = { version = "==1.1.6", optional = true }
 qualang-tools = { version = "^0.15.0", optional = true}
 setuptools = { version = ">67.0.0", optional = true }
 laboneq = { version = "==2.25.0", optional = true }
-qibosoq = { version = ">=0.0.4,<0.2", optional = true }
+qibosoq = { version = ">=0.1.2,<0.2", optional = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pdbpp = "^0.10.3"
 ipython = "^8.12.0"
@@ -52,18 +52,18 @@
 recommonmark = "^0.7.1"
 sphinxcontrib-bibtex = "^2.5.0"
 sphinx-markdown-tables = "^0.0.17"
 nbsphinx = "^0.9.1"
 ipython = "^8.12.0"
 sphinx-copybutton = "^0.5.1"
 # extras
-qblox-instruments = "0.11.0"
+qblox-instruments = "0.12.0"
 qcodes = "^0.37.0"
 qcodes_contrib_drivers = "0.18.0"
-qibosoq = ">=0.0.4,<0.2"
+qibosoq = ">=0.1.2,<0.2"
 qualang-tools = "^0.15.0"
 laboneq = "==2.25.0"
 
 [tool.poetry.group.tests]
 optional = true
 
 [tool.poetry.group.tests.dependencies]
```

### Comparing `qibolab-0.1.6/src/qibolab/__init__.py` & `qibolab-0.1.7/src/qibolab/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -44,15 +44,18 @@
     if name == "dummy" or name == "dummy_couplers":
         from qibolab.dummy import create_dummy
 
         return create_dummy(with_couplers=name == "dummy_couplers")
 
     platform = get_platforms_path() / f"{name}"
     if not platform.exists():
-        raise_error(ValueError, f"Platform {name} does not exist.")
+        raise_error(
+            ValueError,
+            f"Platform {name} does not exist. Please pick one within the platforms found available {get_available_platforms()}.",
+        )
 
     spec = importlib.util.spec_from_file_location("platform", platform / PLATFORM)
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     return module.create()
 
 
@@ -71,7 +74,38 @@
     """
     from qibolab.backends import QibolabBackend
 
     circuit = Circuit.from_qasm(circuit)
     return QibolabBackend(platform).execute_circuit(
         circuit, initial_state=initial_state, nshots=nshots
     )
+
+
+def get_available_platforms() -> list[str]:
+    """Returns the platforms found in the $QIBOLAB_PLATFORMS directory."""
+    return [
+        d.name
+        for d in get_platforms_path().iterdir()
+        if d.is_dir()
+        and Path(f"{os.environ.get(PLATFORMS)}/{d.name}/platform.py") in d.iterdir()
+    ]
+
+
+class MetaBackend:
+    """Meta-backend class which takes care of loading the qibolab backend."""
+
+    @staticmethod
+    def load(platform: str):
+        """Loads the backend.
+
+        Args:
+            platform (str): Name of the platform to load.
+        Returns:
+            qibo.backends.abstract.Backend: The loaded backend.
+        """
+        from qibolab.backends import QibolabBackend
+
+        return QibolabBackend(platform=platform)
+
+    def list_available(self) -> dict:
+        """Lists all the available qibolab platforms."""
+        return {platform: True for platform in get_available_platforms()}
```

### Comparing `qibolab-0.1.6/src/qibolab/backends.py` & `qibolab-0.1.7/src/qibolab/backends.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from collections import deque
-from typing import Callable, Optional
 
 import numpy as np
 from qibo import __version__ as qibo_version
 from qibo.backends import NumpyBackend
 from qibo.config import raise_error
 from qibo.models import Circuit
 from qibo.result import MeasurementOutcomes
@@ -25,36 +24,21 @@
             self.platform = create_platform(platform)
         self.versions = {
             "qibo": qibo_version,
             "numpy": self.np.__version__,
             "qibolab": qibolab_version,
         }
         self.compiler = Compiler.default()
-        self.transpiler: Optional[Callable] = None
 
     def apply_gate(self, gate, state, nqubits):  # pragma: no cover
         raise_error(NotImplementedError, "Qibolab cannot apply gates directly.")
 
     def apply_gate_density_matrix(self, gate, state, nqubits):  # pragma: no cover
         raise_error(NotImplementedError, "Qibolab cannot apply gates directly.")
 
-    def transpile(self, circuit):
-        """Applies the transpiler to a single circuit.
-
-        This transforms the circuit into proper connectivity and native
-        gates.
-        """
-        # TODO: Move this method to transpilers
-        if self.transpiler is None or self.transpiler.is_satisfied(circuit):
-            native = circuit
-            qubit_map = {q: q for q in range(circuit.nqubits)}
-        else:
-            native, qubit_map = self.transpiler(circuit)  # pylint: disable=E1102
-        return native, qubit_map
-
     def assign_measurements(self, measurement_map, readout):
         """Assigning measurement outcomes to
         :class:`qibo.states.MeasurementResult` for each gate.
 
         This allows properly obtaining the measured shots from the :class:`qibolab.pulses.ReadoutPulse` object obtaned after pulse sequence execution.
 
         Args:
@@ -88,16 +72,15 @@
             )
         if initial_state is not None:
             raise_error(
                 ValueError,
                 "Hardware backend only supports circuits as initial states.",
             )
 
-        native_circuit, qubit_map = self.transpile(circuit)
-        sequence, measurement_map = self.compiler.compile(native_circuit, self.platform)
+        sequence, measurement_map = self.compiler.compile(circuit, self.platform)
 
         if not self.platform.is_connected:
             self.platform.connect()
 
         readout = self.platform.execute_pulse_sequence(
             sequence,
             ExecutionParameters(nshots=nshots),
@@ -105,47 +88,43 @@
 
         self.platform.disconnect()
 
         result = MeasurementOutcomes(circuit.measurements, self, nshots=nshots)
         self.assign_measurements(measurement_map, readout)
         return result
 
-    def execute_circuits(self, circuits, initial_state=None, nshots=1000):
+    def execute_circuits(self, circuits, initial_states=None, nshots=1000):
         """Executes multiple quantum circuits with a single communication with
         the control electronics.
 
         Circuits are unrolled to a single pulse sequence.
 
         Args:
             circuits (list): List of circuits to execute.
-            initial_state (:class:`qibo.models.circuit.Circuit`): Circuit to prepare the initial state.
+            initial_states (:class:`qibo.models.circuit.Circuit`): Circuit to prepare the initial state.
                 If ``None`` the default ``|00...0>`` state is used.
             nshots (int): Number of shots to sample from the experiment.
 
         Returns:
             List of ``MeasurementOutcomes`` objects containing the results acquired from the execution of each circuit.
         """
-        if isinstance(initial_state, Circuit):
+        if isinstance(initial_states, Circuit):
             return self.execute_circuits(
-                circuit=[initial_state + circuit for circuit in circuits],
+                circuits=[initial_states + circuit for circuit in circuits],
                 nshots=nshots,
             )
-        if initial_state is not None:
+        if initial_states is not None:
             raise_error(
                 ValueError,
                 "Hardware backend only supports circuits as initial states.",
             )
 
         # TODO: Maybe these loops can be parallelized
-        native_circuits, _ = zip(*(self.transpile(circuit) for circuit in circuits))
         sequences, measurement_maps = zip(
-            *(
-                self.compiler.compile(circuit, self.platform)
-                for circuit in native_circuits
-            )
+            *(self.compiler.compile(circuit, self.platform) for circuit in circuits)
         )
 
         if not self.platform.is_connected:
             self.platform.connect()
 
         readout = self.platform.execute_pulse_sequences(
             sequences,
```

### Comparing `qibolab-0.1.6/src/qibolab/channels.py` & `qibolab-0.1.7/src/qibolab/channels.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/compilers/compiler.py` & `qibolab-0.1.7/src/qibolab/compilers/compiler.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/compilers/default.py` & `qibolab-0.1.7/src/qibolab/compilers/default.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/couplers.py` & `qibolab-0.1.7/src/qibolab/couplers.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/dummy/parameters.json` & `qibolab-0.1.7/src/qibolab/dummy/parameters.json`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/dummy/platform.py` & `qibolab-0.1.7/src/qibolab/dummy/platform.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/execution_parameters.py` & `qibolab-0.1.7/src/qibolab/execution_parameters.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/abstract.py` & `qibolab-0.1.7/src/qibolab/instruments/abstract.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/bluefors.py` & `qibolab-0.1.7/src/qibolab/instruments/bluefors.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/dummy.py` & `qibolab-0.1.7/src/qibolab/instruments/dummy.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/erasynth.py` & `qibolab-0.1.7/src/qibolab/instruments/erasynth.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/icarusq.py` & `qibolab-0.1.7/src/qibolab/instruments/icarusq.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/icarusqfpga.py` & `qibolab-0.1.7/src/qibolab/instruments/icarusqfpga.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/oscillator.py` & `qibolab-0.1.7/src/qibolab/instruments/oscillator.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/port.py` & `qibolab-0.1.7/src/qibolab/instruments/port.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qblox/acquisition.py` & `qibolab-0.1.7/src/qibolab/instruments/qblox/acquisition.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qblox/cluster_qcm_bb.py` & `qibolab-0.1.7/src/qibolab/instruments/qblox/cluster_qcm_bb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Qblox Cluster QCM driver."""
 
 import json
 
-from qblox_instruments.qcodes_drivers.cluster import Cluster as QbloxCluster
-from qblox_instruments.qcodes_drivers.qcm_qrm import QcmQrm as QbloxQrmQcm
+from qblox_instruments.native.generic_func import SequencerStates
+from qblox_instruments.qcodes_drivers.cluster import Cluster
+from qblox_instruments.qcodes_drivers.module import Module
 from qibo.config import log
 
 from qibolab.instruments.qblox.module import ClusterModule
 from qibolab.instruments.qblox.q1asm import (
     Block,
     Register,
     convert_phase,
@@ -111,15 +112,15 @@
         Example:
         To create a QcmBb instance named 'qcm_bb' connected to slot 2 of a Cluster at address '192.168.0.100':
         >>> cluster_instance = Cluster("cluster","192.168.1.100", settings)
         >>> qcm_module = QcmBb(name="qcm_bb", address="192.168.1.100:2", cluster=cluster_instance)
         """
         super().__init__(name, address)
         self._ports: dict = {}
-        self.device: QbloxQrmQcm = None
+        self.device: Module = None
 
         self._debug_folder: str = ""
         self._sequencers: dict[Sequencer] = {}
         self.channel_map: dict = {}
         self._device_num_output_ports = 2
         self._device_num_sequencers: int
         self._free_sequencers_numbers: list[int] = (
@@ -145,15 +146,15 @@
             for name, value in self.DEFAULT_SEQUENCERS_VALUES.items():
                 target.set(name, value)
 
         # connect the default sequencers to the out ports
         for port_num, value in self.OUT_PORT_PATH.items():
             self.device.sequencers[port_num].set(f"connect_out{port_num}", value)
 
-    def connect(self, cluster: QbloxCluster = None):
+    def connect(self, cluster: Cluster = None):
         """Connects to the instrument using the instrument settings in the
         runcard.
 
         Once connected, it creates port classes with properties mapped
         to various instrument parameters, and initialises the the
         underlying device parameters. It uploads to the module the port
         settings loaded from the runcard.
@@ -744,17 +745,17 @@
 
     def disconnect(self):
         """Stops all sequencers, disconnect all the outputs from the AWG paths
         of the sequencers."""
         if not self.is_connected:
             return
         for sequencer_number in self._used_sequencers_numbers:
-            state = self.device.get_sequencer_state(sequencer_number)
-            if state.status != "STOPPED":
+            status = self.device.get_sequencer_status(sequencer_number)
+            if status.state is not SequencerStates.STOPPED:
                 log.warning(
-                    f"Device {self.device.sequencers[sequencer_number].name} did not stop normally\nstate: {state}"
+                    f"Device {self.device.sequencers[sequencer_number].name} did not stop normally\nstatus: {status}"
                 )
 
         self.device.stop_sequencer()
         self.device.disconnect_outputs()
         self.is_connected = False
         self.device = None
```

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qblox/cluster_qcm_rf.py` & `qibolab-0.1.7/src/qibolab/instruments/qblox/cluster_qcm_rf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Qblox Cluster QCM-RF driver."""
 
 import json
 
-from qblox_instruments.qcodes_drivers.cluster import Cluster as QbloxCluster
-from qblox_instruments.qcodes_drivers.qcm_qrm import QcmQrm as QbloxQrmQcm
+from qblox_instruments.native.generic_func import SequencerStates
+from qblox_instruments.qcodes_drivers.cluster import Cluster
+from qblox_instruments.qcodes_drivers.module import Module
 from qibo.config import log
 
 from qibolab.instruments.qblox.module import ClusterModule
 from qibolab.instruments.qblox.q1asm import (
     Block,
     Register,
     convert_phase,
@@ -126,15 +127,15 @@
 
         Example:
         To create a QcmRf instance named 'qcm_rf' connected to slot 2 of a Cluster at address '192.168.0.100':
         >>> cluster_instance = Cluster("cluster","192.168.1.100", settings)
         >>> qcm_module = QcmRf(name="qcm_rf", address="192.168.1.100:2", cluster=cluster_instance)
         """
         super().__init__(name, address)
-        self.device: QbloxQrmQcm = None
+        self.device: Module = None
         self.settings = {}
 
         self._debug_folder: str = ""
         self._sequencers: dict[Sequencer] = {}
         self.channel_map: dict = {}
         self._device_num_output_ports = 2
         self._device_num_sequencers: int
@@ -161,15 +162,15 @@
 
         # connect the  default sequencers to the out port
         self.device.sequencers[self.DEFAULT_SEQUENCERS["o1"]].set("connect_out0", "IQ")
         self.device.sequencers[self.DEFAULT_SEQUENCERS["o1"]].set("connect_out1", "off")
         self.device.sequencers[self.DEFAULT_SEQUENCERS["o2"]].set("connect_out1", "IQ")
         self.device.sequencers[self.DEFAULT_SEQUENCERS["o2"]].set("connect_out0", "off")
 
-    def connect(self, cluster: QbloxCluster = None):
+    def connect(self, cluster: Cluster = None):
         """Connects to the instrument using the instrument settings in the
         runcard.
 
         Once connected, it creates port classes with properties mapped
         to various instrument parameters, and initialises the the
         underlying device parameters. It uploads to the module the port
         settings loaded from the runcard.
@@ -742,18 +743,18 @@
 
     def disconnect(self):
         """Stops all sequencers, disconnect all the outputs from the AWG paths
         of the sequencers."""
         if not self.is_connected:
             return
         for sequencer_number in self._used_sequencers_numbers:
-            state = self.device.get_sequencer_state(sequencer_number)
-            if state.status != "STOPPED":
+            status = self.device.get_sequencer_status(sequencer_number)
+            if status.state is not SequencerStates.STOPPED:
                 log.warning(
-                    f"Device {self.device.sequencers[sequencer_number].name} did not stop normally\nstate: {state}"
+                    f"Device {self.device.sequencers[sequencer_number].name} did not stop normally\nstate: {status}"
                 )
 
         self.device.stop_sequencer()
         self.device.disconnect_outputs()
 
         self.is_connected = False
         self.device = None
```

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qblox/cluster_qrm_rf.py` & `qibolab-0.1.7/src/qibolab/instruments/qblox/cluster_qrm_rf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Qblox Cluster QRM-RF driver."""
 
 import json
 import time
 
 import numpy as np
-from qblox_instruments.qcodes_drivers.cluster import Cluster as QbloxCluster
-from qblox_instruments.qcodes_drivers.qcm_qrm import QcmQrm as QbloxQrmQcm
+from qblox_instruments.native.generic_func import SequencerStates
+from qblox_instruments.qcodes_drivers.cluster import Cluster
+from qblox_instruments.qcodes_drivers.module import Module
 from qibo.config import log
 
 from qibolab.pulses import Pulse, PulseSequence, PulseType
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from .acquisition import AveragedAcquisition, DemodulatedAcquisition
 from .module import ClusterModule
@@ -134,15 +135,15 @@
         Example:
         To create a QrmRf instance named 'qrm_rf' connected to slot 2 of a Cluster at address '192.168.0.100':
         >>> cluster_instance = Cluster("cluster","192.168.1.100", settings)
         >>> qrm_module = QrmRf(name="qrm_rf", address="192.168.1.100:2", cluster=cluster_instance)
         """
 
         super().__init__(name, address)
-        self.device: QbloxQrmQcm = None
+        self.device: Module = None
         self.classification_parameters: dict = {}
         self.settings: dict = {}
 
         self._debug_folder: str = ""
         self._input_ports_keys = ["i1"]
         self._output_ports_keys = ["o1"]
         self._sequencers: dict[Sequencer] = {"o1": []}
@@ -177,15 +178,15 @@
         for name, value in self.DEFAULT_SEQUENCERS_VALUES.items():
             target.set(name, value)
 
         # connect sequencer to out/in ports
         target.set("connect_out0", "IQ")
         target.set("connect_acq", "in0")
 
-    def connect(self, cluster: QbloxCluster = None):
+    def connect(self, cluster: Cluster = None):
         """Connects to the instrument using the instrument settings in the
         runcard.
 
         Once connected, it creates port classes with properties mapped
         to various instrument parameters, and initialises the the
         underlying device parameters. It uploads to the module the port
         settings loaded from the runcard.
@@ -944,22 +945,21 @@
         more details
         """
         # wait until all sequencers stop
         time_out = int(self._execution_time) + 60
         t = time.time()
         for sequencer_number in self._used_sequencers_numbers:
             while True:
-                state = self.device.get_sequencer_state(sequencer_number)
-
-                if state.status == "STOPPED":
+                status = self.device.get_sequencer_status(sequencer_number)
+                if status.state is SequencerStates.STOPPED:
                     # TODO: check flags for errors
                     break
                 elif time.time() - t > time_out:
                     log.info(
-                        f"Timeout - {self.device.sequencers[sequencer_number].name} state: {state}"
+                        f"Timeout - {self.device.sequencers[sequencer_number].name} status: {status}"
                     )
                     self.device.stop_sequencer(sequencer_number)
                     break
                 time.sleep(0.5)
 
         # Qblox qrm modules only have one memory for scope acquisition.
         # Only one sequencer can save data to that memory.
@@ -1017,18 +1017,18 @@
         of the sequencers and disconnect all the inputs from the acquisition
         paths of the sequencers."""
 
         if not self.is_connected:
             return
 
         for sequencer_number in self._used_sequencers_numbers:
-            state = self.device.get_sequencer_state(sequencer_number)
-            if state.status != "STOPPED":
+            status = self.device.get_sequencer_status(sequencer_number)
+            if status.state is not SequencerStates.STOPPED:
                 log.warning(
-                    f"Device {self.device.sequencers[sequencer_number].name} did not stop normally\nstate: {state}"
+                    f"Device {self.device.sequencers[sequencer_number].name} did not stop normally\nstatus: {status}"
                 )
         self.device.stop_sequencer()
         self.device.disconnect_outputs()
         self.device.disconnect_inputs()
 
         self.is_connected = False
         self.device = None
```

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qblox/controller.py` & `qibolab-0.1.7/src/qibolab/instruments/qblox/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,28 @@
 from qibolab.instruments.qblox.cluster_qrm_rf import QrmRf
 from qibolab.instruments.qblox.sequencer import SAMPLING_RATE
 from qibolab.pulses import PulseSequence, PulseType
 from qibolab.result import SampleResults
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from qibolab.unrolling import Bounds
 
-SEQUENCER_MEMORY = 2**17
+MAX_NUM_BINS = 98304
+"""Maximum number of bins that should be used per sequencer in a readout
+module.
+
+One sequencer can have up to 2 ** 17 bins, however the 6 sequencers in
+module allocate bins from a shared memory, and this memory is smaller
+than 6 * 2 ** 17. Hence, if all sequencers are used at once, each cannot
+support 2 ** 17 bins. In fact, the total bin memory for the module is 3
+* (2 ** 17 + 2 ** 16). This means up to three sequencers used at once
+can support 2 ** 17 bins each, but four or more sequencers cannot. So
+the limitation on the number of bins technically depends on the number
+of sequencers used, but to keep things simple we limit ourselves to max
+number of bins that works regardless of situation.
+"""
 
 
 class QbloxController(Controller):
     """A controller to manage qblox devices.
 
     Attributes:
         is_connected (bool): .
@@ -451,15 +464,15 @@
                     else 1
                 )
                 num_bins = nshots
                 for sweeper in sweepers:
                     num_bins *= len(sweeper.values)
 
                     # split the sweep if the number of bins is larget than the memory of the sequencer (2**17)
-                if num_bins < SEQUENCER_MEMORY:
+                if num_bins < MAX_NUM_BINS:
                     # for sweeper in sweepers:
                     #     if sweeper.parameter is Parameter.amplitude:
                     #         # qblox cannot sweep amplitude in real time, but sweeping gain is quivalent
                     #         for pulse in sweeper.pulses:
                     #             pulse.amplitude = 1
 
                     #     elif sweeper.parameter is Parameter.gain:
@@ -476,21 +489,21 @@
                         qubits, sequence, options, sweepers
                     )
                     self._add_to_results(sequence, results, result)
                 else:
                     sweepers_repetitions = 1
                     for sweeper in sweepers:
                         sweepers_repetitions *= len(sweeper.values)
-                    if sweepers_repetitions > SEQUENCER_MEMORY:
+                    if sweepers_repetitions > MAX_NUM_BINS:
                         raise ValueError(
                             f"Requested sweep has {sweepers_repetitions} total number of sweep points. "
-                            f"Maximum supported is {SEQUENCER_MEMORY}"
+                            f"Maximum supported is {MAX_NUM_BINS}"
                         )
 
-                    max_rt_nshots = SEQUENCER_MEMORY // sweepers_repetitions
+                    max_rt_nshots = MAX_NUM_BINS // sweepers_repetitions
                     num_full_sft_iterations = nshots // max_rt_nshots
                     result_chunks = []
                     for sft_iteration in range(num_full_sft_iterations + 1):
                         _nshots = min(
                             max_rt_nshots, nshots - sft_iteration * max_rt_nshots
                         )
```

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qblox/debug.py` & `qibolab-0.1.7/src/qibolab/instruments/qblox/debug.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qblox/module.py` & `qibolab-0.1.7/src/qibolab/instruments/qblox/module.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qblox/port.py` & `qibolab-0.1.7/src/qibolab/instruments/qblox/port.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qblox/q1asm.py` & `qibolab-0.1.7/src/qibolab/instruments/qblox/q1asm.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qblox/sequencer.py` & `qibolab-0.1.7/src/qibolab/instruments/qblox/sequencer.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qblox/sweeper.py` & `qibolab-0.1.7/src/qibolab/instruments/qblox/sweeper.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qm/acquisition.py` & `qibolab-0.1.7/src/qibolab/instruments/qm/acquisition.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     RESULT_CLS = RawWaveformResults
     AVERAGED_RESULT_CLS = AveragedRawWaveformResults
 
     def assign_element(self, element):
         pass
 
     def measure(self, operation, element):
+        qua.reset_phase(element)
         qua.measure(operation, element, self.adc_stream)
 
     def download(self, *dimensions):
         istream = self.adc_stream.input1()
         qstream = self.adc_stream.input2()
         if self.average:
             istream = istream.average()
```

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qm/config.py` & `qibolab-0.1.7/src/qibolab/instruments/qm/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass, field
 
 import numpy as np
 from qibo.config import raise_error
 
 from qibolab.pulses import PulseType, Rectangular
 
-from .ports import OPXIQ, OctaveInput, OctaveOutput
+from .ports import OPXIQ, OctaveInput, OctaveOutput, OPXOutput
 
 SAMPLING_RATE = 1
 """Sampling rate of Quantum Machines OPX in GSps."""
 
 DEFAULT_INPUTS = {1: {}, 2: {}}
 """Default controller config section.
 
@@ -46,26 +46,34 @@
         if isinstance(port, OPXIQ):
             self.register_port(port.i)
             self.register_port(port.q)
         else:
             is_octave = isinstance(port, (OctaveOutput, OctaveInput))
             controllers = self.octaves if is_octave else self.controllers
             if port.device not in controllers:
-                controllers[port.device] = {}
-                if not is_octave:
-                    controllers[port.device]["analog_inputs"] = DEFAULT_INPUTS
+                if is_octave:
+                    controllers[port.device] = {}
+                else:
+                    controllers[port.device] = {
+                        "analog_inputs": DEFAULT_INPUTS,
+                        "digital_outputs": {},
+                    }
 
             device = controllers[port.device]
             if port.key in device:
                 device[port.key].update(port.config)
             else:
                 device[port.key] = port.config
+
             if is_octave:
-                device["connectivity"] = port.opx_port.i.device
+                con = port.opx_port.i.device
+                number = port.opx_port.i.number
+                device["connectivity"] = con
                 self.register_port(port.opx_port)
+                self.controllers[con]["digital_outputs"][number] = {}
 
     @staticmethod
     def iq_imbalance(g, phi):
         """Creates the correction matrix for the mixer imbalance caused by the
         gain and phase imbalances.
 
         More information here:
@@ -80,161 +88,174 @@
         c = np.cos(phi)
         s = np.sin(phi)
         N = 1 / ((1 - g**2) * (2 * c**2 - 1))
         return [
             float(N * x) for x in [(1 - g) * c, (1 + g) * s, (1 - g) * s, (1 + g) * c]
         ]
 
+    def _new_frequency_element(self, qubit, intermediate_frequency, mode="drive"):
+        """Register element on existing port but with different frequency."""
+        element = f"{mode}{qubit.name}"
+        current_if = self.elements[element]["intermediate_frequency"]
+        if intermediate_frequency == current_if:
+            return element
+
+        if isinstance(getattr(qubit, mode).port, (OPXIQ, OPXOutput)):
+            raise NotImplementedError(
+                f"Cannot play two different frequencies on the same {mode} line."
+            )
+        new_element = f"{element}_{intermediate_frequency}"
+        self.elements[new_element] = dict(self.elements[f"drive{qubit.name}"])
+        self.elements[new_element]["intermediate_frequency"] = intermediate_frequency
+        return new_element
+
     def register_drive_element(self, qubit, intermediate_frequency=0):
         """Register qubit drive elements and controllers in the QM config.
 
         Args:
             qubit (:class:`qibolab.platforms.utils.Qubit`): Qubit to add elements for.
             intermediate_frequency (int): Intermediate frequency that the OPX
                 will send to this qubit. This frequency will be mixed with the
                 LO connected to the same channel.
         """
-        if f"drive{qubit.name}" not in self.elements:
-            if isinstance(qubit.drive.port, OPXIQ):
-                lo_frequency = math.floor(qubit.drive.lo_frequency)
-                self.elements[f"drive{qubit.name}"] = {
-                    "mixInputs": {
-                        "I": qubit.drive.port.i.pair,
-                        "Q": qubit.drive.port.q.pair,
-                        "lo_frequency": lo_frequency,
-                        "mixer": f"mixer_drive{qubit.name}",
-                    },
-                }
-                drive_g = qubit.mixer_drive_g
-                drive_phi = qubit.mixer_drive_phi
-                self.mixers[f"mixer_drive{qubit.name}"] = [
-                    {
-                        "intermediate_frequency": intermediate_frequency,
-                        "lo_frequency": lo_frequency,
-                        "correction": self.iq_imbalance(drive_g, drive_phi),
-                    }
-                ]
-            else:
-                self.elements[f"drive{qubit.name}"] = {
-                    "RF_inputs": {"port": qubit.drive.port.pair},
-                }
-            self.elements[f"drive{qubit.name}"].update(
+        element = f"drive{qubit.name}"
+        if element in self.elements:
+            return self._new_frequency_element(qubit, intermediate_frequency, "drive")
+
+        if isinstance(qubit.drive.port, OPXIQ):
+            lo_frequency = math.floor(qubit.drive.lo_frequency)
+            self.elements[element] = {
+                "mixInputs": {
+                    "I": qubit.drive.port.i.pair,
+                    "Q": qubit.drive.port.q.pair,
+                    "lo_frequency": lo_frequency,
+                    "mixer": f"mixer_drive{qubit.name}",
+                },
+            }
+            drive_g = qubit.mixer_drive_g
+            drive_phi = qubit.mixer_drive_phi
+            self.mixers[f"mixer_drive{qubit.name}"] = [
                 {
                     "intermediate_frequency": intermediate_frequency,
-                    "operations": {},
+                    "lo_frequency": lo_frequency,
+                    "correction": self.iq_imbalance(drive_g, drive_phi),
                 }
-            )
+            ]
         else:
-            self.elements[f"drive{qubit.name}"][
-                "intermediate_frequency"
-            ] = intermediate_frequency
-            if isinstance(qubit.drive.port, OPXIQ):
-                self.mixers[f"mixer_drive{qubit.name}"][0][
-                    "intermediate_frequency"
-                ] = intermediate_frequency
+            self.elements[element] = {
+                "RF_inputs": {"port": qubit.drive.port.pair},
+                "digitalInputs": qubit.drive.port.digital_inputs,
+            }
+        self.elements[element].update(
+            {
+                "intermediate_frequency": intermediate_frequency,
+                "operations": {},
+            }
+        )
+        return element
 
     def register_readout_element(
         self, qubit, intermediate_frequency=0, time_of_flight=0, smearing=0
     ):
         """Register resonator elements and controllers in the QM config.
 
         Args:
             qubit (:class:`qibolab.platforms.utils.Qubit`): Qubit to add elements for.
             intermediate_frequency (int): Intermediate frequency that the OPX
                 will send to this qubit. This frequency will be mixed with the
                 LO connected to the same channel.
         """
-        if f"readout{qubit.name}" not in self.elements:
-            if isinstance(qubit.readout.port, OPXIQ):
-                lo_frequency = math.floor(qubit.readout.lo_frequency)
-                self.elements[f"readout{qubit.name}"] = {
-                    "mixInputs": {
-                        "I": qubit.readout.port.i.pair,
-                        "Q": qubit.readout.port.q.pair,
-                        "lo_frequency": lo_frequency,
-                        "mixer": f"mixer_readout{qubit.name}",
-                    },
-                    "outputs": {
-                        "out1": qubit.feedback.port.i.pair,
-                        "out2": qubit.feedback.port.q.pair,
-                    },
-                }
-                readout_g = qubit.mixer_readout_g
-                readout_phi = qubit.mixer_readout_phi
-                self.mixers[f"mixer_readout{qubit.name}"] = [
-                    {
-                        "intermediate_frequency": intermediate_frequency,
-                        "lo_frequency": lo_frequency,
-                        "correction": self.iq_imbalance(readout_g, readout_phi),
-                    }
-                ]
-            else:
-                self.elements[f"readout{qubit.name}"] = {
-                    "RF_inputs": {"port": qubit.readout.port.pair},
-                    "RF_outputs": {"port": qubit.feedback.port.pair},
-                }
-            self.elements[f"readout{qubit.name}"].update(
+        element = f"readout{qubit.name}"
+        if element in self.elements:
+            return self._new_frequency_element(qubit, intermediate_frequency, "readout")
+
+        if isinstance(qubit.readout.port, OPXIQ):
+            lo_frequency = math.floor(qubit.readout.lo_frequency)
+            self.elements[element] = {
+                "mixInputs": {
+                    "I": qubit.readout.port.i.pair,
+                    "Q": qubit.readout.port.q.pair,
+                    "lo_frequency": lo_frequency,
+                    "mixer": f"mixer_readout{qubit.name}",
+                },
+                "outputs": {
+                    "out1": qubit.feedback.port.i.pair,
+                    "out2": qubit.feedback.port.q.pair,
+                },
+            }
+            readout_g = qubit.mixer_readout_g
+            readout_phi = qubit.mixer_readout_phi
+            self.mixers[f"mixer_readout{qubit.name}"] = [
                 {
                     "intermediate_frequency": intermediate_frequency,
-                    "operations": {},
-                    "time_of_flight": time_of_flight,
-                    "smearing": smearing,
+                    "lo_frequency": lo_frequency,
+                    "correction": self.iq_imbalance(readout_g, readout_phi),
                 }
-            )
+            ]
         else:
-            self.elements[f"readout{qubit.name}"][
-                "intermediate_frequency"
-            ] = intermediate_frequency
-            if isinstance(qubit.readout.port, OPXIQ):
-                self.mixers[f"mixer_readout{qubit.name}"][0][
-                    "intermediate_frequency"
-                ] = intermediate_frequency
+            self.elements[element] = {
+                "RF_inputs": {"port": qubit.readout.port.pair},
+                "RF_outputs": {"port": qubit.feedback.port.pair},
+                "digitalInputs": qubit.readout.port.digital_inputs,
+            }
+        self.elements[element].update(
+            {
+                "intermediate_frequency": intermediate_frequency,
+                "operations": {},
+                "time_of_flight": time_of_flight,
+                "smearing": smearing,
+            }
+        )
+        return element
 
     def register_flux_element(self, qubit, intermediate_frequency=0):
         """Register qubit flux elements and controllers in the QM config.
 
         Args:
             qubit (:class:`qibolab.platforms.utils.Qubit`): Qubit to add elements for.
             intermediate_frequency (int): Intermediate frequency that the OPX
                 will send to this qubit. This frequency will be mixed with the
                 LO connected to the same channel.
         """
-        if f"flux{qubit.name}" not in self.elements:
-            self.elements[f"flux{qubit.name}"] = {
-                "singleInput": {
-                    "port": qubit.flux.port.pair,
-                },
-                "intermediate_frequency": intermediate_frequency,
-                "operations": {},
-            }
-        else:
-            self.elements[f"flux{qubit.name}"][
-                "intermediate_frequency"
-            ] = intermediate_frequency
+        element = f"flux{qubit.name}"
+        if element in self.elements:
+            return self._new_frequency_element(qubit, intermediate_frequency, "flux")
+
+        self.elements[element] = {
+            "singleInput": {
+                "port": qubit.flux.port.pair,
+            },
+            "intermediate_frequency": intermediate_frequency,
+            "operations": {},
+        }
+        return element
 
     def register_element(self, qubit, pulse, time_of_flight=0, smearing=0):
         if pulse.type is PulseType.DRIVE:
             # register drive element
             if_frequency = pulse.frequency - math.floor(qubit.drive.lo_frequency)
-            self.register_drive_element(qubit, if_frequency)
+            element = self.register_drive_element(qubit, if_frequency)
             # register flux element (if available)
             if qubit.flux:
                 self.register_flux_element(qubit)
         elif pulse.type is PulseType.READOUT:
             # register readout element (if it does not already exist)
             if_frequency = pulse.frequency - math.floor(qubit.readout.lo_frequency)
-            self.register_readout_element(qubit, if_frequency, time_of_flight, smearing)
+            element = self.register_readout_element(
+                qubit, if_frequency, time_of_flight, smearing
+            )
             # register flux element (if available)
             if qubit.flux:
                 self.register_flux_element(qubit)
         else:
             # register flux element
-            self.register_flux_element(qubit, pulse.frequency)
+            element = self.register_flux_element(qubit, pulse.frequency)
+        return element
 
-    def register_pulse(self, qubit, qmpulse):
+    def register_pulse(self, qubit, qmpulse, element=None):
         """Registers pulse, waveforms and integration weights in QM config.
 
         Args:
             qubit (:class:`qibolab.platforms.utils.Qubit`): Qubit that the pulse acts on.
             pulse (:class:`qibolab.pulses.Pulse`): Pulse object to register.
 
         Returns:
@@ -248,31 +269,32 @@
             if pulse.type is PulseType.DRIVE:
                 serial_i = self.register_waveform(pulse, "i")
                 serial_q = self.register_waveform(pulse, "q")
                 self.pulses[qmpulse.operation] = {
                     "operation": "control",
                     "length": pulse.duration,
                     "waveforms": {"I": serial_i, "Q": serial_q},
+                    "digital_marker": "ON",
                 }
                 # register drive pulse in elements
-                self.elements[f"drive{qubit.name}"]["operations"][
+                self.elements[qmpulse.element]["operations"][
                     qmpulse.operation
                 ] = qmpulse.operation
 
             elif pulse.type is PulseType.FLUX:
                 serial = self.register_waveform(pulse)
                 self.pulses[qmpulse.operation] = {
                     "operation": "control",
                     "length": pulse.duration,
                     "waveforms": {
                         "single": serial,
                     },
                 }
                 # register flux pulse in elements
-                self.elements[f"flux{qubit.name}"]["operations"][
+                self.elements[qmpulse.element]["operations"][
                     qmpulse.operation
                 ] = qmpulse.operation
 
             elif pulse.type is PulseType.READOUT:
                 serial_i = self.register_waveform(pulse, "i")
                 serial_q = self.register_waveform(pulse, "q")
                 self.register_integration_weights(qubit, pulse.duration)
@@ -287,15 +309,15 @@
                         "cos": f"cosine_weights{qubit.name}",
                         "sin": f"sine_weights{qubit.name}",
                         "minus_sin": f"minus_sine_weights{qubit.name}",
                     },
                     "digital_marker": "ON",
                 }
                 # register readout pulse in elements
-                self.elements[f"readout{qubit.name}"]["operations"][
+                self.elements[qmpulse.element]["operations"][
                     qmpulse.operation
                 ] = qmpulse.operation
 
             else:
                 raise_error(TypeError, f"Unknown pulse type {pulse.type.name}.")
 
     def register_waveform(self, pulse, mode="i"):
```

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qm/controller.py` & `qibolab-0.1.7/src/qibolab/instruments/qm/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,29 +294,29 @@
         ):
             qubit = qubits[pulse.qubit]
 
             self.config.register_port(getattr(qubit, pulse.type.name.lower()).port)
             if pulse.type is PulseType.READOUT:
                 self.config.register_port(qubit.feedback.port)
 
-            self.config.register_element(
+            element = self.config.register_element(
                 qubit, pulse, self.time_of_flight, self.smearing
             )
             if (
                 pulse.duration % 4 != 0
                 or pulse.duration < 16
                 or pulse.serial in pulses_to_bake
             ):
-                qmpulse = BakedPulse(pulse)
+                qmpulse = BakedPulse(pulse, element)
                 qmpulse.bake(self.config, durations=[pulse.duration])
             else:
-                qmpulse = QMPulse(pulse)
+                qmpulse = QMPulse(pulse, element)
                 if pulse.type is PulseType.READOUT:
                     ro_pulses.append(qmpulse)
-                self.config.register_pulse(qubit, qmpulse)
+                self.config.register_pulse(qubit, qmpulse, element)
             qmsequence.add(qmpulse)
 
         qmsequence.shift()
         return qmsequence, ro_pulses
 
     def play(self, qubits, couplers, sequence, options):
         return self.sweep(qubits, couplers, sequence, options)
```

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qm/devices.py` & `qibolab-0.1.7/src/qibolab/instruments/qm/devices.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qm/ports.py` & `qibolab-0.1.7/src/qibolab/instruments/qm/ports.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 from dataclasses import dataclass, field, fields
 from typing import ClassVar, Dict, Optional, Union
 
+DIGITAL_DELAY = 57
+DIGITAL_BUFFER = 18
+"""Default calibration parameters for digital pulses.
+
+https://docs.quantum-machines.co/1.1.7/qm-qua-sdk/docs/Guides/octave/#calibrating-the-digital-pulse
+
+Digital markers are used for LO triggering.
+"""
+
 
 @dataclass
 class QMPort:
     """Abstract representation of Quantum Machine instrument ports.
 
     Contains the ports settings for each device.
     """
@@ -136,20 +145,40 @@
     Can be in the range [-20 : 0.5 : 20] dB.
     """
     lo_source: str = field(default="internal", metadata={"config": "LO_source"})
     """Local oscillator clock source.
 
     Can be external or internal.
     """
-    output_mode: str = field(default="always_on", metadata={"config": "output_mode"})
+    output_mode: str = field(default="triggered", metadata={"config": "output_mode"})
     """Can be: "always_on" / "always_off"/ "triggered" / "triggered_reversed"."""
+    digital_delay: int = DIGITAL_DELAY
+    """Delay for digital output channel."""
+    digital_buffer: int = DIGITAL_BUFFER
+    """Buffer for digital output channel."""
 
     opx_port: Optional[OPXOutput] = None
     """OPX+ port that is connected to the Octave port."""
 
+    @property
+    def digital_inputs(self):
+        """Generates `digitalInputs` entry for elements in QM config.
+
+        Digital markers are used to switch LOs on in triggered mode.
+        """
+        opx = self.opx_port.i.device
+        number = self.opx_port.i.number
+        return {
+            "output_switch": {
+                "port": (opx, number),
+                "delay": self.digital_delay,
+                "buffer": self.digital_buffer,
+            }
+        }
+
 
 @dataclass
 class OctaveInput(QMInput):
     key: ClassVar[str] = "RF_inputs"
 
     lo_frequency: float = field(
         default=0.0, metadata={"config": "LO_frequency", "settings": True}
```

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qm/sequence.py` & `qibolab-0.1.7/src/qibolab/instruments/qm/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,16 @@
     duration.
     """
     elements_to_align: Set[str] = field(default_factory=set)
 
     def __post_init__(self):
         pulse_type = self.pulse.type.name.lower()
         amplitude = format(self.pulse.amplitude, ".6f").rstrip("0").rstrip(".")
-        self.element: str = f"{pulse_type}{self.pulse.qubit}"
+        if self.element is None:
+            self.element = f"{pulse_type}{self.pulse.qubit}"
         self.operation: str = (
             f"{pulse_type}({self.pulse.duration}, {amplitude}, {self.pulse.shape})"
         )
         self.relative_phase: float = self.pulse.relative_phase / (2 * np.pi)
         self.elements_to_align.add(self.element)
 
     def __hash__(self):
```

### Comparing `qibolab-0.1.6/src/qibolab/instruments/qm/sweepers.py` & `qibolab-0.1.7/src/qibolab/instruments/qm/sweepers.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/rfsoc/convert.py` & `qibolab-0.1.7/src/qibolab/instruments/rfsoc/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,14 @@
     stops = []
     indexes = []
 
     if sweeper.parameter is BIAS:
         for qubit in sweeper.qubits:
             parameters.append(rfsoc.Parameter.BIAS)
             indexes.append(list(qubits.values()).index(qubit))
-
             base_value = qubit.flux.offset
             values = sweeper.get_values(base_value)
             starts.append(values[0])
             stops.append(values[-1])
 
         if max(np.abs(starts)) > 1 or max(np.abs(stops)) > 1:
             raise ValueError("Sweeper amplitude is set to reach values higher than 1")
```

### Comparing `qibolab-0.1.6/src/qibolab/instruments/rfsoc/driver.py` & `qibolab-0.1.7/src/qibolab/instruments/rfsoc/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """RFSoC FPGA driver."""
 
+import re
 from dataclasses import asdict, dataclass
 from typing import Union
 
 import numpy as np
 import numpy.typing as npt
 import qibosoq.components.base as rfsoc
+from qibo.config import log
 from qibosoq import client
 
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.instruments.abstract import Controller
 from qibolab.instruments.port import Port
 from qibolab.platform import Coupler, Qubit
 from qibolab.pulses import PulseSequence, PulseType
@@ -65,14 +67,31 @@
 
     def connect(self):
         """Empty method to comply with Instrument interface."""
 
     def disconnect(self):
         """Empty method to comply with Instrument interface."""
 
+    @staticmethod
+    def _try_to_execute(server_commands, host, port):
+        try:
+            return client.connect(server_commands, host, port)
+        except RuntimeError as e:
+            if "exception in readout loop" in str(e):
+                log.warning(
+                    "%s %s",
+                    "Exception in readout loop. Attempting again",
+                    "You may want to increase the relaxation time.",
+                )
+                return client.connect(server_commands, host, port)
+            buffer_overflow = r"buffer length must be \d+ samples or less"
+            if re.search(buffer_overflow, str(e)) is not None:
+                log.warning("Buffer full! Use shorter pulses.")
+            raise e
+
     def _execute_pulse_sequence(
         self,
         sequence: PulseSequence,
         qubits: dict[int, Qubit],
         opcode: rfsoc.OperationCode,
     ) -> tuple[list, list]:
         """Prepare the commands dictionary to send to the qibosoq server.
@@ -86,15 +105,15 @@
         """
         server_commands = {
             "operation_code": opcode,
             "cfg": asdict(self.cfg),
             "sequence": convert(sequence, qubits, self.sampling_rate),
             "qubits": [asdict(convert(qubits[idx])) for idx in qubits],
         }
-        return client.connect(server_commands, self.host, self.port)
+        return self._try_to_execute(server_commands, self.host, self.port)
 
     def _execute_sweeps(
         self,
         sequence: PulseSequence,
         qubits: dict[int, Qubit],
         sweepers: list[rfsoc.Sweeper],
     ) -> tuple[list, list]:
@@ -112,15 +131,15 @@
         server_commands = {
             "operation_code": rfsoc.OperationCode.EXECUTE_SWEEPS,
             "cfg": asdict(self.cfg),
             "sequence": convert(sequence, qubits, self.sampling_rate),
             "qubits": [asdict(convert(qubits[idx])) for idx in qubits],
             "sweepers": [sweeper.serialized for sweeper in sweepers],
         }
-        return client.connect(server_commands, self.host, self.port)
+        return self._try_to_execute(server_commands, self.host, self.port)
 
     def play(
         self,
         qubits: dict[int, Qubit],
         couplers: dict[int, Coupler],
         sequence: PulseSequence,
         execution_parameters: ExecutionParameters,
@@ -139,14 +158,19 @@
                                                         acquisition_type,
                                                         averaging_mode)
             sequence (`qibolab.pulses.PulseSequence`): Pulse sequence to play.
         Returns:
             A dictionary mapping the readout pulses serial and respective qubits to
             qibolab results objects
         """
+        if couplers != {}:
+            raise NotImplementedError(
+                "The RFSoC driver currently does not support couplers."
+            )
+
         self.validate_input_command(sequence, execution_parameters, sweep=False)
         self.update_cfg(execution_parameters)
 
         if execution_parameters.acquisition_type is AcquisitionType.DISCRIMINATION:
             self.cfg.average = False
         else:
             self.cfg.average = (
@@ -203,17 +227,15 @@
             raise NotImplementedError("Fast reset is not supported")
 
     def update_cfg(self, execution_parameters: ExecutionParameters):
         """Update rfsoc.Config object with new parameters."""
         if execution_parameters.nshots is not None:
             self.cfg.reps = execution_parameters.nshots
         if execution_parameters.relaxation_time is not None:
-            self.cfg.repetition_duration = (
-                execution_parameters.relaxation_time * NS_TO_US
-            )
+            self.cfg.relaxation_time = execution_parameters.relaxation_time * NS_TO_US
 
     def classify_shots(
         self,
         i_values: npt.NDArray[np.float64],
         q_values: npt.NDArray[np.float64],
         qubit: Qubit,
     ) -> npt.NDArray[np.float64]:
@@ -328,15 +350,14 @@
                         "duration",
                     }
                 ):
                     setattr(
                         sequence[kdx], sweeper_parameter.name.lower(), values[jdx][idx]
                     )
                 elif sweeper is rfsoc.Parameter.DELAY:
-                    start_delay = values[jdx][idx]
                     sequence[kdx].start_delay = values[jdx][idx]
 
             res = self.recursive_python_sweep(
                 qubits,
                 couplers,
                 sequence,
                 or_sequence,
@@ -360,15 +381,22 @@
             dict_a (dict): dict mapping ro pulses serial to qibolab res objects
             dict_b (dict): dict mapping ro pulses serial to qibolab res objects
         Returns:
             A dict mapping the readout pulses serial to qibolab results objects
         """
         for serial in dict_b:
             if serial in dict_a:
-                dict_a[serial] = dict_a[serial] + dict_b[serial]
+                cls = dict_a[serial].__class__
+                if isinstance(dict_a[serial], IntegratedResults):
+                    new_data = np.column_stack(
+                        [dict_a[serial].voltage, dict_b[serial].voltage]
+                    )
+                elif isinstance(dict_a[serial], SampleResults):
+                    new_data = np.append(dict_a[serial].samples, dict_b[serial].samples)
+                dict_a[serial] = cls(new_data)
             else:
                 dict_a[serial] = dict_b[serial]
         return dict_a
 
     def get_if_python_sweep(
         self, sequence: PulseSequence, *sweepers: rfsoc.Sweeper
     ) -> bool:
@@ -450,35 +478,35 @@
         adcs = np.unique([qubits[p.qubit].feedback.port.name for p in original_ro])
         for k, k_val in enumerate(adcs):
             adc_ro = [
                 pulse
                 for pulse in original_ro
                 if qubits[pulse.qubit].feedback.port.name == k_val
             ]
-            for i, (ro_pulse, original_ro_pulse) in enumerate(zip(adc_ro, original_ro)):
+            for i, ro_pulse in enumerate(adc_ro):
                 i_vals = np.array(toti[k][i])
                 q_vals = np.array(totq[k][i])
 
                 if not self.cfg.average:
                     i_vals = np.reshape(i_vals, (self.cfg.reps, *i_vals.shape[:-1]))
                     q_vals = np.reshape(q_vals, (self.cfg.reps, *q_vals.shape[:-1]))
 
                 if (
                     execution_parameters.acquisition_type
                     is AcquisitionType.DISCRIMINATION
                 ):
-                    qubit = qubits[original_ro_pulse.qubit]
+                    qubit = qubits[ro_pulse.qubit]
                     discriminated_shots = self.classify_shots(i_vals, q_vals, qubit)
                     if execution_parameters.averaging_mode is AveragingMode.CYCLIC:
                         discriminated_shots = np.mean(discriminated_shots, axis=0)
                     result = execution_parameters.results_type(discriminated_shots)
                 else:
                     result = execution_parameters.results_type(i_vals + 1j * q_vals)
 
-                results[original_ro_pulse.qubit] = results[ro_pulse.serial] = result
+                results[ro_pulse.qubit] = results[ro_pulse.serial] = result
         return results
 
     def sweep(
         self,
         qubits: dict[int, Qubit],
         couplers: dict[int, Coupler],
         sequence: PulseSequence,
@@ -500,14 +528,19 @@
                                                         averaging_mode)
             sequence (`qibolab.pulses.PulseSequence`). Pulse sequence to play.
             *sweepers (`qibolab.Sweeper`): Sweeper objects.
         Returns:
             A dictionary mapping the readout pulses serial and respective qubits to
             results objects
         """
+        if couplers != {}:
+            raise NotImplementedError(
+                "The RFSoC driver currently does not support couplers."
+            )
+
         self.validate_input_command(sequence, execution_parameters, sweep=True)
         self.update_cfg(execution_parameters)
 
         if execution_parameters.acquisition_type is AcquisitionType.DISCRIMINATION:
             self.cfg.average = False
         else:
             self.cfg.average = (
```

### Comparing `qibolab-0.1.6/src/qibolab/instruments/rohde_schwarz.py` & `qibolab-0.1.7/src/qibolab/instruments/rohde_schwarz.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/zhinst/executor.py` & `qibolab-0.1.7/src/qibolab/instruments/zhinst/executor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -698,17 +698,17 @@
 
         exp.play(signal=channel_name, pulse=pulse.zhpulse, **play_parameters)
 
     def sweep(self, qubits, couplers, sequence: PulseSequence, options, *sweepers):
         """Play pulse and sweepers sequence."""
 
         self.signal_map = {}
+        self.frequency_from_pulses(qubits, sequence)
         self.processed_sweeps = ProcessedSweeps(sweepers, qubits)
         self.nt_sweeps, self.rt_sweeps = classify_sweepers(sweepers)
-        self.frequency_from_pulses(qubits, sequence)
 
         self.acquisition_type = None
         for sweeper in sweepers:
             if sweeper.parameter in {Parameter.frequency, Parameter.amplitude}:
                 for pulse in sweeper.pulses:
                     if pulse.type is PulseType.READOUT:
                         self.acquisition_type = lo.AcquisitionType.SPECTROSCOPY
```

### Comparing `qibolab-0.1.6/src/qibolab/instruments/zhinst/pulse.py` & `qibolab-0.1.7/src/qibolab/instruments/zhinst/pulse.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/zhinst/sweep.py` & `qibolab-0.1.7/src/qibolab/instruments/zhinst/sweep.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/instruments/zhinst/util.py` & `qibolab-0.1.7/src/qibolab/instruments/zhinst/util.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/kernels.py` & `qibolab-0.1.7/src/qibolab/kernels.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/native.py` & `qibolab-0.1.7/src/qibolab/native.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/platform.py` & `qibolab-0.1.7/src/qibolab/platform.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/pulses.py` & `qibolab-0.1.7/src/qibolab/pulses.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         .. todo::
 
             To be replaced by proper serialization.
         """
         shape_name = re.findall(r"(\w+)", value)[0]
         if shape_name not in globals():
             raise ValueError(f"shape {value} not found")
-        shape_parameters = re.findall(r"[\w+\d\.\d]+", value)[1:]
+        shape_parameters = re.findall(r"[-\w+\d\.\d]+", value)[1:]
         # TODO: create multiple tests to prove regex working correctly
         return globals()[shape_name](*shape_parameters)
 
 
 class Rectangular(PulseShape):
     """Rectangular pulse shape."""
 
@@ -487,15 +487,14 @@
                     / (((num_samples) / self.rel_sigma) ** 2)
                 )
             )
             q = (
                 self.beta
                 * (-(x - (num_samples - 1) / 2) / ((num_samples / self.rel_sigma) ** 2))
                 * i
-                * sampling_rate
             )
             waveform = Waveform(q)
             waveform.serial = f"Envelope_Waveform_Q(num_samples = {num_samples}, amplitude = {format(self.pulse.amplitude, '.6f').rstrip('0').rstrip('.')}, shape = {repr(self)})"
             return waveform
         raise ShapeInitError
 
     def __repr__(self):
```

### Comparing `qibolab-0.1.6/src/qibolab/qubits.py` & `qibolab-0.1.7/src/qibolab/qubits.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     """Assignment fidelity."""
     readout_fidelity: float = 0.0
     """Readout fidelity."""
     effective_temperature: float = 0.0
     """Effective temperature."""
     peak_voltage: float = 0
     pi_pulse_amplitude: float = 0
+    resonator_depletion_time: int = 0
     T1: int = 0
     T2: int = 0
     T2_spin_echo: int = 0
     state0_voltage: int = 0
     state1_voltage: int = 0
     mean_gnd_states: List[float] = field(default_factory=lambda: [0, 0])
     mean_exc_states: List[float] = field(default_factory=lambda: [0, 0])
```

### Comparing `qibolab-0.1.6/src/qibolab/result.py` & `qibolab-0.1.7/src/qibolab/result.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,20 @@
     def magnitude(self):
         """Signal magnitude in volts."""
         return np.sqrt(self.voltage_i**2 + self.voltage_q**2)
 
     @cached_property
     def phase(self):
         """Signal phase in radians."""
-        return np.angle(self.voltage_i + 1.0j * self.voltage_q)
+        return np.unwrap(np.arctan2(self.voltage_i, self.voltage_q))
+
+    @cached_property
+    def phase_std(self):
+        """Signal phase in radians."""
+        return np.std(self.phase, axis=0, ddof=1) / np.sqrt(self.phase.shape[0])
 
     @property
     def serialize(self):
         """Serialize as a dictionary."""
         serialized_dict = {
             "MSR[V]": self.magnitude.flatten(),
             "i[V]": self.voltage_i.flatten(),
@@ -64,23 +69,38 @@
     act.AbstractPlatform.execute_pulse_sequence`
     :func:`qibolab.platforms.abstract.AbstractPlatform.sweep`
 
     Associated with AcquisitionType.INTEGRATION and AveragingMode.CYCLIC
     or the averages of ``IntegratedResults``
     """
 
-    def __init__(self, data: np.ndarray, std: np.ndarray = np.array([])):
+    def __init__(self, data: np.ndarray, std: Optional[np.ndarray] = None):
         super().__init__(data)
         self.std: Optional[npt.NDArray[np.float64]] = std
 
     def __add__(self, data):
         new_res = super().__add__(data)
         new_res.std = np.append(self.std, data.std)
         return new_res
 
+    @property
+    def average(self):
+        """Average on AveragedIntegratedResults is itself."""
+        return self
+
+    @cached_property
+    def phase_std(self):
+        """Standard deviation is None for AveragedIntegratedResults."""
+        return None
+
+    @cached_property
+    def phase(self):
+        """Phase not unwrapped because it is a single value."""
+        return np.arctan2(self.voltage_i, self.voltage_q)
+
 
 class RawWaveformResults(IntegratedResults):
     """Data structure to deal with the output of :func:`qibolab.platforms.abstr
     act.AbstractPlatform.execute_pulse_sequence`
     :func:`qibolab.platforms.abstract.AbstractPlatform.sweep`
 
     Associated with AcquisitionType.RAW and AveragingMode.SINGLESHOT may
```

### Comparing `qibolab-0.1.6/src/qibolab/serialize.py` & `qibolab-0.1.7/src/qibolab/serialize.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/sweeper.py` & `qibolab-0.1.7/src/qibolab/sweeper.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/src/qibolab/unrolling.py` & `qibolab-0.1.7/src/qibolab/unrolling.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.1.6/PKG-INFO` & `qibolab-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qibolab
-Version: 0.1.6
+Version: 0.1.7
 Summary: Quantum hardware module and drivers for Qibo
 Home-page: https://qibo.science/
 License: Apache-2.0
 Author: The Qibo team
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -18,19 +18,19 @@
 Provides-Extra: rfsoc
 Provides-Extra: zh
 Requires-Dist: laboneq (==2.25.0) ; extra == "zh"
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pyvisa-py (==0.5.3) ; extra == "qblox" or extra == "los"
-Requires-Dist: qblox-instruments (==0.11.0) ; extra == "qblox"
+Requires-Dist: qblox-instruments (==0.12.0) ; extra == "qblox"
 Requires-Dist: qcodes (>=0.37.0,<0.38.0) ; extra == "qblox" or extra == "los"
 Requires-Dist: qcodes_contrib_drivers (==0.18.0) ; extra == "qblox" or extra == "los"
 Requires-Dist: qibo (>=0.2.6)
-Requires-Dist: qibosoq (>=0.0.4,<0.2) ; extra == "rfsoc"
+Requires-Dist: qibosoq (>=0.1.2,<0.2) ; extra == "rfsoc"
 Requires-Dist: qm-qua (==1.1.6) ; extra == "qm"
 Requires-Dist: qualang-tools (>=0.15.0,<0.16.0) ; extra == "qm"
 Requires-Dist: setuptools (>67.0.0)
 Project-URL: Documentation, https://qibo.science/docs/qibolab/stable
 Project-URL: Repository, https://github.com/qiboteam/qibolab/
 Description-Content-Type: text/markdown
```

