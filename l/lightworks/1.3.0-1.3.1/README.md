# Comparing `tmp/lightworks-1.3.0.tar.gz` & `tmp/lightworks-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightworks-1.3.0.tar", last modified: Wed May 22 12:58:39 2024, max compression
+gzip compressed data, was "lightworks-1.3.1.tar", last modified: Thu May 23 12:54:31 2024, max compression
```

## Comparing `lightworks-1.3.0.tar` & `lightworks-1.3.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.592154 lightworks-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 12:58:13.000000 lightworks-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-22 12:58:39.592154 lightworks-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-22 12:58:13.000000 lightworks-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.576154 lightworks-1.3.0/lightworks/
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/__version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.580154 lightworks-1.3.0/lightworks/emulator/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.580154 lightworks-1.3.0/lightworks/emulator/annotated_state/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/annotated_state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/annotated_state/annotated_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.580154 lightworks-1.3.0/lightworks/emulator/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/backend/permanent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/backend/slos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.580154 lightworks-1.3.0/lightworks/emulator/components/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/components/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/components/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.580154 lightworks-1.3.0/lightworks/emulator/results/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/results/sampling_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/results/simulation_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.580154 lightworks-1.3.0/lightworks/emulator/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/simulation/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/simulation/probability_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/simulation/quick_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18633 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/simulation/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/simulation/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/emulator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/emulator/utils/state_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/qubit/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/qubit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/qubit/gates/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/qubit/gates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/qubit/gates/single_qubit_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/qubit/gates/two_qubit_gates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/sdk/circuit/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29551 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/circuit/circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/circuit/circuit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/circuit/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/circuit/unitary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/sdk/optimisation/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/optimisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/optimisation/optimisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.584154 lightworks-1.3.0/lightworks/sdk/state/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/state/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.588154 lightworks-1.3.0/lightworks/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/circuit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/heralding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/matrix_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/permutation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/utils/state_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.588154 lightworks-1.3.0/lightworks/sdk/visualisation/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/visualisation/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    15875 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/visualisation/display_components_mpl.py
--rw-r--r--   0 runner    (1001) docker     (127)    17005 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/visualisation/display_components_svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/visualisation/draw_circuit_mpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-05-22 12:58:13.000000 lightworks-1.3.0/lightworks/sdk/visualisation/draw_circuit_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.592154 lightworks-1.3.0/lightworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-22 12:58:39.000000 lightworks-1.3.0/lightworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-22 12:58:39.000000 lightworks-1.3.0/lightworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:58:39.000000 lightworks-1.3.0/lightworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 12:58:39.000000 lightworks-1.3.0/lightworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 12:58:39.000000 lightworks-1.3.0/lightworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-22 12:58:13.000000 lightworks-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:58:39.592154 lightworks-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-22 12:58:13.000000 lightworks-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.576154 lightworks-1.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.588154 lightworks-1.3.0/tests/emulator/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/analyzer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/annotatedstate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/cnot_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/detector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/quicksampler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/result_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23566 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/simulator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/emulator/source_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:58:39.592154 lightworks-1.3.0/tests/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27061 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/circuit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/compiledcircuit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/display_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/parameter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/qubit_gate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/state_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-22 12:58:13.000000 lightworks-1.3.0/tests/sdk/util_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.747483 lightworks-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 12:54:27.000000 lightworks-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-23 12:54:31.747483 lightworks-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-23 12:54:27.000000 lightworks-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.735483 lightworks-1.3.1/lightworks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/__version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.735483 lightworks-1.3.1/lightworks/emulator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.735483 lightworks-1.3.1/lightworks/emulator/annotated_state/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/annotated_state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/annotated_state/annotated_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.735483 lightworks-1.3.1/lightworks/emulator/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/backend/permanent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/backend/slos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.735483 lightworks-1.3.1/lightworks/emulator/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/components/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/components/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.735483 lightworks-1.3.1/lightworks/emulator/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/results/sampling_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18822 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/results/simulation_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.739483 lightworks-1.3.1/lightworks/emulator/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/simulation/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/simulation/probability_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/simulation/quick_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18633 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/simulation/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/simulation/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.739483 lightworks-1.3.1/lightworks/emulator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/emulator/utils/state_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.739483 lightworks-1.3.1/lightworks/qubit/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/qubit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.739483 lightworks-1.3.1/lightworks/qubit/gates/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/qubit/gates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/qubit/gates/single_qubit_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/qubit/gates/two_qubit_gates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.739483 lightworks-1.3.1/lightworks/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.739483 lightworks-1.3.1/lightworks/sdk/circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29541 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/circuit/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/circuit/circuit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/circuit/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/circuit/unitary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.739483 lightworks-1.3.1/lightworks/sdk/optimisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/optimisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/optimisation/optimisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.739483 lightworks-1.3.1/lightworks/sdk/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/state/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.743483 lightworks-1.3.1/lightworks/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/utils/circuit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/utils/heralding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/utils/matrix_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/utils/permutation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/utils/state_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.743483 lightworks-1.3.1/lightworks/sdk/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/visualisation/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15875 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/visualisation/display_components_mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17005 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/visualisation/display_components_svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/visualisation/draw_circuit_mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-05-23 12:54:27.000000 lightworks-1.3.1/lightworks/sdk/visualisation/draw_circuit_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.747483 lightworks-1.3.1/lightworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-23 12:54:31.000000 lightworks-1.3.1/lightworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-23 12:54:31.000000 lightworks-1.3.1/lightworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:54:31.000000 lightworks-1.3.1/lightworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-23 12:54:31.000000 lightworks-1.3.1/lightworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 12:54:31.000000 lightworks-1.3.1/lightworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-23 12:54:27.000000 lightworks-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 12:54:31.747483 lightworks-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-23 12:54:27.000000 lightworks-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.735483 lightworks-1.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.743483 lightworks-1.3.1/tests/emulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/emulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/emulator/analyzer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/emulator/annotatedstate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/emulator/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/emulator/cnot_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/emulator/detector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/emulator/quicksampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15837 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/emulator/result_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23566 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/emulator/sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/emulator/simulator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/emulator/source_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:54:31.747483 lightworks-1.3.1/tests/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29106 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/sdk/circuit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/sdk/compiledcircuit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/sdk/display_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/sdk/parameter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/sdk/qubit_gate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/sdk/state_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-23 12:54:27.000000 lightworks-1.3.1/tests/sdk/util_test.py
```

### Comparing `lightworks-1.3.0/LICENSE` & `lightworks-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/PKG-INFO` & `lightworks-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightworks
-Version: 1.3.0
+Version: 1.3.1
 Summary: Open-source Python SDK for photonic quantum computation.
 Home-page: https://github.com/Aegiq/lightworks
 Author: Aegiq Ltd.
 License: Apache 2.0
 Project-URL: Source, https://github.com/Aegiq/lightworks
 Project-URL: Documentation, https://aegiq.github.io/lightworks/
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lightworks-1.3.0/README.md` & `lightworks-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/__init__.py` & `lightworks-1.3.1/lightworks/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/__version.py` & `lightworks-1.3.1/lightworks/__version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
```

### Comparing `lightworks-1.3.0/lightworks/emulator/__init__.py` & `lightworks-1.3.1/lightworks/emulator/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/annotated_state/__init__.py` & `lightworks-1.3.1/lightworks/emulator/annotated_state/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/annotated_state/annotated_state.py` & `lightworks-1.3.1/lightworks/emulator/annotated_state/annotated_state.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/backend/__init__.py` & `lightworks-1.3.1/lightworks/emulator/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/backend/backend.py` & `lightworks-1.3.1/lightworks/emulator/backend/backend.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/backend/permanent.py` & `lightworks-1.3.1/lightworks/emulator/backend/permanent.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/backend/slos.py` & `lightworks-1.3.1/lightworks/emulator/backend/slos.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/components/__init__.py` & `lightworks-1.3.1/lightworks/emulator/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/components/detector.py` & `lightworks-1.3.1/lightworks/emulator/components/detector.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/components/source.py` & `lightworks-1.3.1/lightworks/emulator/components/source.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/results/__init__.py` & `lightworks-1.3.1/lightworks/emulator/results/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/results/sampling_result.py` & `lightworks-1.3.1/lightworks/emulator/results/sampling_result.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/results/simulation_result.py` & `lightworks-1.3.1/lightworks/emulator/results/simulation_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,17 +140,14 @@
             if ostate is None:
                 return sub_r
             # Else return requested value
             elif ostate in sub_r:
                 return sub_r[ostate]
             else:
                 raise KeyError("Requested output state not in data.")
-        elif isinstance(item, slice):
-            raise DeprecationWarning(
-                "Retrieval of data through slicing is no longer supported.")
         else:
             raise ValueError(
                 "Get item value must be either one or two States.")
         
     def __str__(self) -> str:
         return str(self.dictionary)
     
@@ -223,15 +220,16 @@
                     new_s = State([s%2 for s in out_state])
                 if new_s in mapped_result[in_state]:
                     mapped_result[in_state][new_s] += val
                 else:
                     mapped_result[in_state][new_s] = val
         return self._recombine_mapped_result(mapped_result)
     
-    def _recombine_mapped_result(self, mapped_result: dict):
+    def _recombine_mapped_result(self, mapped_result: dict
+                                 ) -> "SimulationResult":
         """Creates a new Result object from mapped data."""
         unique_outputs = set()
         for in_state, pdist in mapped_result.items():
             for out_state in pdist:
                 unique_outputs.add(out_state)
         array = np.zeros((len(self.inputs), len(unique_outputs)))
         for i, in_state in enumerate(self.inputs):
@@ -418,16 +416,14 @@
         in_strings = [str(s) for s in self.inputs]
         out_strings = [str(s) for s in self.outputs]
         # Switch to probability if required
         data = self.array.copy()
         if conv_to_probability:
             if self.result_type == "probability_amplitude":
                 data = abs(data)**2
-            elif self.result_type == "counts":
-                data = data/np.sum(data)
         # Apply thresholding to values
         for i in range(data.shape[0]):
             for j in range(data.shape[1]):
                 val = data[i,j]
                 re = np.real(val) if abs(np.real(val)) > threshold else 0
                 im = np.imag(val) if abs(np.imag(val)) > threshold else 0
                 data[i,j] = re if abs(im) == 0 else re + 1j*im
```

### Comparing `lightworks-1.3.0/lightworks/emulator/simulation/__init__.py` & `lightworks-1.3.1/lightworks/emulator/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/simulation/analyzer.py` & `lightworks-1.3.1/lightworks/emulator/simulation/analyzer.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/simulation/probability_distribution.py` & `lightworks-1.3.1/lightworks/emulator/simulation/probability_distribution.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/simulation/quick_sampler.py` & `lightworks-1.3.1/lightworks/emulator/simulation/quick_sampler.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/simulation/sampler.py` & `lightworks-1.3.1/lightworks/emulator/simulation/sampler.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/simulation/simulator.py` & `lightworks-1.3.1/lightworks/emulator/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/utils/__init__.py` & `lightworks-1.3.1/lightworks/emulator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/utils/exceptions.py` & `lightworks-1.3.1/lightworks/emulator/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/emulator/utils/state_utils.py` & `lightworks-1.3.1/lightworks/emulator/utils/state_utils.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/qubit/__init__.py` & `lightworks-1.3.1/lightworks/qubit/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/qubit/gates/__init__.py` & `lightworks-1.3.1/lightworks/qubit/gates/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/__init__.py` & `lightworks-1.3.1/lightworks/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/circuit/__init__.py` & `lightworks-1.3.1/lightworks/sdk/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/circuit/circuit.py` & `lightworks-1.3.1/lightworks/sdk/circuit/circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,15 @@
         return
     
     def get_all_params(self) -> list:
         """
         Returns all the Parameter objects used as part of creating the circuit.
         """
         all_params = []
-        for _, params in unpack_circuit_spec(deepcopy(self.__circuit_spec)):
+        for _, params in unpack_circuit_spec(self.__circuit_spec):
             for p in params:
                 if isinstance(p, Parameter) and p not in all_params:
                     all_params.append(p)
         return all_params    
     
     def copy(self, freeze_parameters: bool =  False) -> "Circuit":
         """
```

### Comparing `lightworks-1.3.0/lightworks/sdk/circuit/circuit_compiler.py` & `lightworks-1.3.1/lightworks/sdk/circuit/circuit_compiler.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/circuit/parameters.py` & `lightworks-1.3.1/lightworks/sdk/circuit/parameters.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/circuit/unitary.py` & `lightworks-1.3.1/lightworks/sdk/circuit/unitary.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/optimisation/__init__.py` & `lightworks-1.3.1/lightworks/sdk/optimisation/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/optimisation/optimisation.py` & `lightworks-1.3.1/lightworks/sdk/optimisation/optimisation.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/state/__init__.py` & `lightworks-1.3.1/lightworks/sdk/state/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/state/state.py` & `lightworks-1.3.1/lightworks/sdk/state/state.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/utils/__init__.py` & `lightworks-1.3.1/lightworks/sdk/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .matrix_utils import (check_unitary, random_unitary, random_permutation,
                            add_mode_to_unitary)
-from .state_utils import fock_basis, state_to_string
+from .state_utils import state_to_string
 from .exceptions import *
 from .conversion import db_loss_to_transmission, transmission_to_db_loss
 from .permutation_conversion import permutation_mat_from_swaps_dict
 from .circuit_utils import unpack_circuit_spec
 from .circuit_utils import convert_non_adj_beamsplitters
 from .circuit_utils import compress_mode_swaps, add_empty_mode_to_circuit_spec
 from .circuit_utils import add_modes_to_circuit_spec
```

### Comparing `lightworks-1.3.0/lightworks/sdk/utils/circuit_utils.py` & `lightworks-1.3.1/lightworks/sdk/utils/circuit_utils.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/utils/conversion.py` & `lightworks-1.3.1/lightworks/sdk/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/utils/exceptions.py` & `lightworks-1.3.1/lightworks/sdk/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/utils/heralding_utils.py` & `lightworks-1.3.1/lightworks/sdk/utils/heralding_utils.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/utils/matrix_utils.py` & `lightworks-1.3.1/lightworks/sdk/utils/matrix_utils.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/utils/permutation_conversion.py` & `lightworks-1.3.1/lightworks/sdk/utils/permutation_conversion.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/visualisation/__init__.py` & `lightworks-1.3.1/lightworks/sdk/visualisation/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/visualisation/display.py` & `lightworks-1.3.1/lightworks/sdk/visualisation/display.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/visualisation/display_components_mpl.py` & `lightworks-1.3.1/lightworks/sdk/visualisation/display_components_mpl.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/visualisation/display_components_svg.py` & `lightworks-1.3.1/lightworks/sdk/visualisation/display_components_svg.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/visualisation/draw_circuit_mpl.py` & `lightworks-1.3.1/lightworks/sdk/visualisation/draw_circuit_mpl.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks/sdk/visualisation/draw_circuit_svg.py` & `lightworks-1.3.1/lightworks/sdk/visualisation/draw_circuit_svg.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/lightworks.egg-info/PKG-INFO` & `lightworks-1.3.1/lightworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightworks
-Version: 1.3.0
+Version: 1.3.1
 Summary: Open-source Python SDK for photonic quantum computation.
 Home-page: https://github.com/Aegiq/lightworks
 Author: Aegiq Ltd.
 License: Apache 2.0
 Project-URL: Source, https://github.com/Aegiq/lightworks
 Project-URL: Documentation, https://aegiq.github.io/lightworks/
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lightworks-1.3.0/lightworks.egg-info/SOURCES.txt` & `lightworks-1.3.1/lightworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/setup.py` & `lightworks-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/emulator/__init__.py` & `lightworks-1.3.1/tests/emulator/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/emulator/analyzer_test.py` & `lightworks-1.3.1/tests/emulator/analyzer_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/emulator/backend_test.py` & `lightworks-1.3.1/tests/emulator/backend_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,14 +126,38 @@
         p2 = backend_s.full_probability_distribution(circuit._build(),
                                                      input_state)
         # Check equivalence
         for s in p1:
             if round(p1[s], 8) != round(p2[s], 8):
                 pytest.fail("Methods do not produce equivalent distributions.")
                 
+    def test_clifford_not_implemented(self):
+        """
+        Confirms that clifford backend produces not-implemented error when 
+        trying to use it.
+        """
+        with pytest.raises(NotImplementedError):
+            Backend("clifford")
+            
+    def test_backend_str_return(self):
+        """
+        Check that backend value is stored and returned correctly when using
+        the str operator.
+        """
+        backend = Backend("permanent")
+        assert str(backend) == "permanent"
+        
+    def test_backend_repr_return(self):
+        """
+        Checks that backend value is correctly included in __repr__ for 
+        backend.
+        """
+        backend = Backend("permanent")
+        assert "permanent" in repr(backend)  
+                
 class TestPermanent:
     """
     Specific functions for testing Permanent calculation remains functional
     and consistent.
     """
     
     def test_single_photon_return(self):
```

### Comparing `lightworks-1.3.0/tests/emulator/cnot_test.py` & `lightworks-1.3.1/tests/emulator/cnot_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/emulator/detector_test.py` & `lightworks-1.3.1/tests/emulator/detector_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/emulator/quicksampler_test.py` & `lightworks-1.3.1/tests/emulator/quicksampler_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/emulator/sampler_test.py` & `lightworks-1.3.1/tests/emulator/sampler_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/emulator/simulator_test.py` & `lightworks-1.3.1/tests/emulator/simulator_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/emulator/source_test.py` & `lightworks-1.3.1/tests/emulator/source_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/sdk/__init__.py` & `lightworks-1.3.1/tests/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/sdk/circuit_test.py` & `lightworks-1.3.1/tests/sdk/circuit_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from lightworks import Parameter, ParameterDict, Circuit
 from lightworks import Unitary, random_unitary
 from lightworks.sdk.circuit.circuit_compiler import CompiledCircuit
 from lightworks.sdk.circuit.circuit_compiler import CompiledUnitary
+from lightworks import CircuitCompilationError
 
 import pytest
 from random import random, seed, randint
 from numpy import round
 
 class TestCircuit:
     """
@@ -638,14 +639,72 @@
         circuit._Circuit__internal_modes = [1, 3, 4]
         # Add bs on modes
         circuit.add_bs(*initial_modes)
         # Then check modes are converted to correct values
         assert circuit._Circuit__circuit_spec[0][1][0] == final_modes[0]
         assert circuit._Circuit__circuit_spec[0][1][1] == final_modes[1]
         
+    def test_add_bs_invalid_convention(self):
+        """
+        Checks a ValueError is raised if an invalid beam splitter convention is
+        set in add_bs.
+        """
+        circuit = Circuit(3)
+        with pytest.raises(ValueError):
+            circuit.add_bs(0, convention = "Not valid")
+            
+    def test_get_all_params(self):
+        """
+        Tests get_all_params method correctly identifies all parameters added
+        within a circuit.
+        """
+        p1 = Parameter(0.5)
+        p2 = Parameter(2)
+        p3 = Parameter(3)
+        # Create circuit with parameters
+        circuit = Circuit(4)
+        circuit.add_bs(0, reflectivity = p1)
+        circuit.add_ps(2, p2)
+        circuit.add_loss(3, p3)
+        # Recover all params and then check
+        all_params = circuit.get_all_params()
+        for param in [p1, p2, p3]:
+            assert param in all_params
+            
+    def test_get_all_params_grouped_circ(self):
+        """
+        Tests get_all_params method correctly identifies all parameters added
+        within a grouped circuit.
+        """
+        p1 = Parameter(0.5)
+        p2 = Parameter(2)
+        p3 = Parameter(3)
+        # Create sub-circuit with parameters
+        sub_circuit = Circuit(4)
+        sub_circuit.add_bs(0, reflectivity = p1)
+        sub_circuit.add_ps(2, p2)
+        sub_circuit.add_loss(3, p3)
+        # Then add to larger circuit
+        circuit = Circuit(5)
+        circuit.add(sub_circuit, 1, group = True)
+        # Recover all params and then check
+        all_params = circuit.get_all_params()
+        for param in [p1, p2, p3]:
+            assert param in all_params
+        
+    def test_edit_circuit_spec(self):
+        """
+        Checks an exception is raised if a circuit spec is modified with an 
+        invalid value.
+        """
+        circuit = Circuit(4)
+        circuit._Circuit__circuit_spec = [["test", None]]
+        with pytest.raises(CircuitCompilationError):
+            circuit._build()
+        
 class TestUnitary:
     """
     Unit tests to confirm correct functioning of the Unitary class when various 
     operations are performed.
     """
     
     def test_unitary_assignment(self):
```

### Comparing `lightworks-1.3.0/tests/sdk/compiledcircuit_test.py` & `lightworks-1.3.1/tests/sdk/compiledcircuit_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/sdk/display_test.py` & `lightworks-1.3.1/tests/sdk/display_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/sdk/parameter_test.py` & `lightworks-1.3.1/tests/sdk/parameter_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 from lightworks import Parameter, ParameterDict
 from lightworks import ParameterValueError, ParameterBoundsError
 from lightworks import ParameterDictError
 
 import pytest
 
+from math import inf
+
 class TestParameter:
     """Unit tests to test functionality of Parameter objects."""
     
     def test_parameter_creation(self):
         """
         Checks that a Parameter can be created as it's value can retrieved as 
         expected.
@@ -120,14 +122,34 @@
     def test_str_return(self):
         """
         Confirms that Parameter value is returned when str function is used on 
         Parameter.
         """
         p = Parameter(1.2)
         assert str(p) == "1.2"
+    
+    @pytest.mark.parametrize("value", [1, 2.1, "test"])
+    def test_repr_return(self, value):
+        """
+        Checks Parameter value is contained within the value returned when repr
+        is used.
+        """
+        p = Parameter(value)
+        assert str(value) in repr(p)
+    
+    def test_label_in_repr_return(self):
+        """Checks label included in repr return."""
+        p = Parameter(1, label = "label")
+        assert "label" in repr(p)
+        
+    def test_bounds_in_repr_return(self):
+        """Checks bounds in repr return."""
+        p = Parameter(1, bounds = [0, 3])
+        assert str(p.min_bound) in repr(p)
+        assert str(p.max_bound) in repr(p)
         
 class TestParameterDict:
     """Unit tests to test functionality of ParameterDict objects."""
     
     def test_dict_creation(self):
         """Checks dictionary can be created and is empty after creation."""
         pd = ParameterDict()
@@ -140,14 +162,23 @@
         assert pd["a"].get() == 1
             
     def test_dict_return(self):
         """Confirms that the return when using [] is a Parameter object."""
         pd = ParameterDict()
         pd["a"] = Parameter(1)
         assert isinstance(pd["a"], Parameter)
+        
+    def test_dict_invalid_param(self):
+        """
+        Confirms that a KeyError is raised when a parameter key does not exist.
+        """
+        pd = ParameterDict()
+        pd["a"] = Parameter(1)
+        with pytest.raises(KeyError):
+            pd["b"]
     
     def test_parameter_update(self):
         """Test updating of parameter through assigning new value to dict."""
         pd = ParameterDict()
         pd["a"] = Parameter(1)
         pd["a"] = 2
         assert pd["a"].get() == 2
@@ -229,8 +260,24 @@
         pd["b"] = Parameter(2)
         pd["c"] = Parameter(2)
         # Loop over dictionary and store returned values
         params = []
         for p in pd:
             params.append(p)
         # Check lists is equivalent to params attribute
-        assert params == pd.params
+        assert params == pd.params
+        
+    def test_get_bounds(self):
+        """
+        Confirms that get bounds is able to identify bounds for parameter.
+        """
+        pd = ParameterDict()
+        pd["a"] = Parameter(1, bounds = [0, 2])
+        assert pd.get_bounds()["a"] == (0, 2)
+        
+    def test_get_bounds_no_bounds(self):
+        """
+        Confirms that get bounds replaces None bounds with +/- inf.
+        """
+        pd = ParameterDict()
+        pd["a"] = Parameter(1)
+        assert pd.get_bounds()["a"] == (-inf, inf)
```

### Comparing `lightworks-1.3.0/tests/sdk/qubit_gate_test.py` & `lightworks-1.3.1/tests/sdk/qubit_gate_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/sdk/state_test.py` & `lightworks-1.3.1/tests/sdk/state_test.py`

 * *Files identical despite different names*

### Comparing `lightworks-1.3.0/tests/sdk/util_test.py` & `lightworks-1.3.1/tests/sdk/util_test.py`

 * *Files identical despite different names*

