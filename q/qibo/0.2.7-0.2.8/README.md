# Comparing `tmp/qibo-0.2.7.tar.gz` & `tmp/qibo-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibo-0.2.7.tar", max compression
+gzip compressed data, was "qibo-0.2.8.tar", max compression
```

## Comparing `qibo-0.2.7.tar` & `qibo-0.2.8.tar`

### file list

```diff
@@ -1,79 +1,78 @@
--rw-r--r--   0        0        0    11342 2024-04-05 12:05:25.084715 qibo-0.2.7/LICENSE
--rw-r--r--   0        0        0     3277 2024-04-05 12:05:25.084715 qibo-0.2.7/README.md
--rw-r--r--   0        0        0     3119 2024-04-05 12:05:25.264717 qibo-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      569 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/__init__.py
--rw-r--r--   0        0        0     6346 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/__init__.py
--rw-r--r--   0        0        0    17580 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/_clifford_operations.py
--rw-r--r--   0        0        0    14561 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/abstract.py
--rw-r--r--   0        0        0    12600 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/clifford.py
--rw-r--r--   0        0        0     2780 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/einsum_utils.py
--rw-r--r--   0        0        0    14381 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/npmatrices.py
--rw-r--r--   0        0        0    34067 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/numpy.py
--rw-r--r--   0        0        0     6453 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/pytorch.py
--rw-r--r--   0        0        0     8588 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/backends/tensorflow.py
--rw-r--r--   0        0        0    11718 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/callbacks.py
--rw-r--r--   0        0        0     3097 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/config.py
--rw-r--r--   0        0        0     8794 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/derivative.py
--rw-r--r--   0        0        0      136 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/gates/__init__.py
--rw-r--r--   0        0        0    16946 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/gates/abstract.py
--rw-r--r--   0        0        0    30848 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/gates/channels.py
--rw-r--r--   0        0        0    70885 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/gates/gates.py
--rw-r--r--   0        0        0     9713 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/gates/measurements.py
--rw-r--r--   0        0        0     6004 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/gates/special.py
--rw-r--r--   0        0        0      109 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/hamiltonians/__init__.py
--rw-r--r--   0        0        0     4384 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/hamiltonians/abstract.py
--rw-r--r--   0        0        0     5941 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/hamiltonians/adiabatic.py
--rw-r--r--   0        0        0    32100 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/hamiltonians/hamiltonians.py
--rw-r--r--   0        0        0     6695 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/hamiltonians/models.py
--rw-r--r--   0        0        0    13024 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/hamiltonians/terms.py
--rw-r--r--   0        0        0     6875 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/measurements.py
--rw-r--r--   0        0        0      531 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/__init__.py
--rw-r--r--   0        0        0    12344 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/_openqasm.py
--rw-r--r--   0        0        0    52843 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/circuit.py
--rw-r--r--   0        0        0        0 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/dbi/__init__.py
--rw-r--r--   0        0        0     6182 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/dbi/double_bracket.py
--rw-r--r--   0        0        0     6023 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/dbi/utils.py
--rw-r--r--   0        0        0    13651 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/distcircuit.py
--rw-r--r--   0        0        0    15947 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/encodings.py
--rw-r--r--   0        0        0    39662 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/error_mitigation.py
--rw-r--r--   0        0        0    13481 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/evolution.py
--rw-r--r--   0        0        0    11600 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/grover.py
--rw-r--r--   0        0        0     9065 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/hep.py
--rw-r--r--   0        0        0    14786 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/iqae.py
--rw-r--r--   0        0        0    16497 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/qcnn.py
--rw-r--r--   0        0        0     2842 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/qft.py
--rw-r--r--   0        0        0    16345 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/qgan.py
--rw-r--r--   0        0        0     6922 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/tsp.py
--rw-r--r--   0        0        0     8166 2024-04-05 12:05:25.264717 qibo-0.2.7/src/qibo/models/utils.py
--rw-r--r--   0        0        0    26669 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/models/variational.py
--rw-r--r--   0        0        0    21207 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/noise.py
--rw-r--r--   0        0        0    19616 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/noise_model.py
--rw-r--r--   0        0        0    13516 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/optimizers.py
--rw-r--r--   0        0        0     6786 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/parallel.py
--rw-r--r--   0        0        0     4652 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/parameter.py
--rw-r--r--   0        0        0      404 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/__init__.py
--rw-r--r--   0        0        0    18833 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/_clifford_utils.py
--rw-r--r--   0        0        0     9608 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/basis.py
--rw-r--r--   0        0        0    17742 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/clifford.py
--rw-r--r--   0        0        0    10188 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/entanglement.py
--rw-r--r--   0        0        0    32812 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/entropies.py
--rw-r--r--   0        0        0    29696 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/metrics.py
--rw-r--r--   0        0        0    27251 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/quantum_networks.py
--rw-r--r--   0        0        0    48165 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/random_ensembles.py
--rw-r--r--   0        0        0    88591 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/superoperator_transformations.py
--rw-r--r--   0        0        0    17674 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/quantum_info/utils.py
--rw-r--r--   0        0        0    21454 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/result.py
--rw-r--r--   0        0        0     5069 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/solvers.py
--rw-r--r--   0        0        0     4950 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/symbols.py
--rw-r--r--   0        0        0      376 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/__init__.py
--rw-r--r--   0        0        0      604 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/_exceptions.py
--rw-r--r--   0        0        0     1787 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/abstract.py
--rw-r--r--   0        0        0    12514 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/blocks.py
--rw-r--r--   0        0        0    13310 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/decompositions.py
--rw-r--r--   0        0        0     1874 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/optimizer.py
--rw-r--r--   0        0        0    10588 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/pipeline.py
--rw-r--r--   0        0        0    16809 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/placer.py
--rw-r--r--   0        0        0    35659 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/router.py
--rw-r--r--   0        0        0    11816 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/unitary_decompositions.py
--rw-r--r--   0        0        0     8127 2024-04-05 12:05:25.268717 qibo-0.2.7/src/qibo/transpiler/unroller.py
--rw-r--r--   0        0        0     4656 1970-01-01 00:00:00.000000 qibo-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11342 2024-05-23 05:11:09.222716 qibo-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3277 2024-05-23 05:11:09.222716 qibo-0.2.8/README.md
+-rw-r--r--   0        0        0     3247 2024-05-23 05:11:09.402718 qibo-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      621 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/__init__.py
+-rw-r--r--   0        0        0     7876 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/backends/__init__.py
+-rw-r--r--   0        0        0    19687 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/backends/_clifford_operations.py
+-rw-r--r--   0        0        0    14561 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/backends/abstract.py
+-rw-r--r--   0        0        0    12452 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/backends/clifford.py
+-rw-r--r--   0        0        0     2780 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/backends/einsum_utils.py
+-rw-r--r--   0        0        0    14388 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/backends/npmatrices.py
+-rw-r--r--   0        0        0    34348 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/backends/numpy.py
+-rw-r--r--   0        0        0     6453 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/backends/pytorch.py
+-rw-r--r--   0        0        0     8666 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/backends/tensorflow.py
+-rw-r--r--   0        0        0    11718 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/callbacks.py
+-rw-r--r--   0        0        0     3097 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/config.py
+-rw-r--r--   0        0        0     8794 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/derivative.py
+-rw-r--r--   0        0        0      136 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/gates/__init__.py
+-rw-r--r--   0        0        0    16941 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/gates/abstract.py
+-rw-r--r--   0        0        0    30848 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/gates/channels.py
+-rw-r--r--   0        0        0    70980 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/gates/gates.py
+-rw-r--r--   0        0        0     9713 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/gates/measurements.py
+-rw-r--r--   0        0        0     6004 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/gates/special.py
+-rw-r--r--   0        0        0      109 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/hamiltonians/__init__.py
+-rw-r--r--   0        0        0     4384 2024-05-23 05:11:09.402718 qibo-0.2.8/src/qibo/hamiltonians/abstract.py
+-rw-r--r--   0        0        0     5941 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/hamiltonians/adiabatic.py
+-rw-r--r--   0        0        0    32070 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/hamiltonians/hamiltonians.py
+-rw-r--r--   0        0        0     6695 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/hamiltonians/models.py
+-rw-r--r--   0        0        0    13024 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/hamiltonians/terms.py
+-rw-r--r--   0        0        0     6875 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/measurements.py
+-rw-r--r--   0        0        0      492 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/__init__.py
+-rw-r--r--   0        0        0    12344 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/_openqasm.py
+-rw-r--r--   0        0        0    52843 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/circuit.py
+-rw-r--r--   0        0        0        0 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/dbi/__init__.py
+-rw-r--r--   0        0        0     7628 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/dbi/double_bracket.py
+-rw-r--r--   0        0        0     6063 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/dbi/utils.py
+-rw-r--r--   0        0        0    13651 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/distcircuit.py
+-rw-r--r--   0        0        0    15947 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/encodings.py
+-rw-r--r--   0        0        0    43561 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/error_mitigation.py
+-rw-r--r--   0        0        0    13481 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/evolution.py
+-rw-r--r--   0        0        0    11600 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/grover.py
+-rw-r--r--   0        0        0     9065 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/hep.py
+-rw-r--r--   0        0        0    14786 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/iqae.py
+-rw-r--r--   0        0        0    16497 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/qcnn.py
+-rw-r--r--   0        0        0     2842 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/qft.py
+-rw-r--r--   0        0        0     6922 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/tsp.py
+-rw-r--r--   0        0        0     8386 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/utils.py
+-rw-r--r--   0        0        0    26582 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/models/variational.py
+-rw-r--r--   0        0        0    21207 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/noise.py
+-rw-r--r--   0        0        0    19616 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/noise_model.py
+-rw-r--r--   0        0        0    13516 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/optimizers.py
+-rw-r--r--   0        0        0     6786 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/parallel.py
+-rw-r--r--   0        0        0     4652 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/parameter.py
+-rw-r--r--   0        0        0      404 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/quantum_info/__init__.py
+-rw-r--r--   0        0        0    18833 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/quantum_info/_clifford_utils.py
+-rw-r--r--   0        0        0     9608 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/quantum_info/basis.py
+-rw-r--r--   0        0        0    17742 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/quantum_info/clifford.py
+-rw-r--r--   0        0        0    10188 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/quantum_info/entanglement.py
+-rw-r--r--   0        0        0    32812 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/quantum_info/entropies.py
+-rw-r--r--   0        0        0    29631 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/quantum_info/metrics.py
+-rw-r--r--   0        0        0    27251 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/quantum_info/quantum_networks.py
+-rw-r--r--   0        0        0    47470 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/quantum_info/random_ensembles.py
+-rw-r--r--   0        0        0    88591 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/quantum_info/superoperator_transformations.py
+-rw-r--r--   0        0        0    17674 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/quantum_info/utils.py
+-rw-r--r--   0        0        0    21454 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/result.py
+-rw-r--r--   0        0        0     5069 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/solvers.py
+-rw-r--r--   0        0        0     4950 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/symbols.py
+-rw-r--r--   0        0        0      376 2024-05-23 05:11:09.406718 qibo-0.2.8/src/qibo/transpiler/__init__.py
+-rw-r--r--   0        0        0      604 2024-05-23 05:11:09.410718 qibo-0.2.8/src/qibo/transpiler/_exceptions.py
+-rw-r--r--   0        0        0     1787 2024-05-23 05:11:09.410718 qibo-0.2.8/src/qibo/transpiler/abstract.py
+-rw-r--r--   0        0        0    12514 2024-05-23 05:11:09.410718 qibo-0.2.8/src/qibo/transpiler/blocks.py
+-rw-r--r--   0        0        0    13310 2024-05-23 05:11:09.410718 qibo-0.2.8/src/qibo/transpiler/decompositions.py
+-rw-r--r--   0        0        0     1874 2024-05-23 05:11:09.410718 qibo-0.2.8/src/qibo/transpiler/optimizer.py
+-rw-r--r--   0        0        0    11211 2024-05-23 05:11:09.410718 qibo-0.2.8/src/qibo/transpiler/pipeline.py
+-rw-r--r--   0        0        0    16809 2024-05-23 05:11:09.410718 qibo-0.2.8/src/qibo/transpiler/placer.py
+-rw-r--r--   0        0        0    35659 2024-05-23 05:11:09.410718 qibo-0.2.8/src/qibo/transpiler/router.py
+-rw-r--r--   0        0        0    11816 2024-05-23 05:11:09.410718 qibo-0.2.8/src/qibo/transpiler/unitary_decompositions.py
+-rw-r--r--   0        0        0     8127 2024-05-23 05:11:09.410718 qibo-0.2.8/src/qibo/transpiler/unroller.py
+-rw-r--r--   0        0        0     4696 1970-01-01 00:00:00.000000 qibo-0.2.8/PKG-INFO
```

### Comparing `qibo-0.2.7/LICENSE` & `qibo-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/README.md` & `qibo-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/pyproject.toml` & `qibo-0.2.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qibo"
-version = "0.2.7"
+version = "0.2.8"
 description = "A framework for quantum computing with hardware acceleration."
 authors = ["The Qibo team"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://qibo.science/"
 repository = "https://github.com/qiboteam/qibo/"
 documentation = "https://qibo.science/docs/qibo/stable"
@@ -17,26 +17,27 @@
   "Programming Language :: Python :: 3",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 packages = [{ include = "qibo", from = "src" }]
 include = ["*.out", "*.yml"]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.9,<3.13"
 scipy = "^1.10.1"
 sympy = "^1.11.1"
 cma = "^3.3.0"
 joblib = "^1.2.0"
 hyperopt = "^0.2.7"
+# `setuptools` is only required because undeclared by `hyperopt`
+setuptools = "^69.1.1"
 tabulate = "^0.9.0"
 openqasm3 = { version = ">=0.5.0", extras = ["parser"] }
 numpy = "^1.26.4"
 networkx = "^3.2.1"
-cvxpy = { version = "^1.4.2", optional = true }
-tensorflow = { version = "^2.14.1,<2.16", markers = "sys_platform == 'linux' or sys_platform == 'darwin'", optional = true }
+tensorflow = { version = "^2.16.1", markers = "sys_platform == 'linux' or sys_platform == 'darwin'", optional = true }
 torch = { version = "^2.1.1", optional = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pdbpp = "^0.10.3"
@@ -57,56 +58,59 @@
 
 [tool.poetry.group.tests]
 optional = true
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.2.1"
 cirq = "^1.1.0"
-cvxpy = "^1.3.1"
 ply = "^3.11"
 scikit-learn = "^1.2.1"
 pytest-cov = "^4.0.0"
-pylint = "^3.0.3"
+pylint = "3.1.0"
 matplotlib = "^3.7.0"
-tensorflow = { version = "^2.14.1,<2.16", markers = "sys_platform == 'linux'" }
+tensorflow = { version = "^2.16.1", markers = "sys_platform == 'linux'" }
 torch = "^2.1.1"
 qibojit = { git = "https://github.com/qiboteam/qibojit.git" }
-qibotn = { git = "https://github.com/qiboteam/qibotn.git" }
+qibotn = { git = "https://github.com/qiboteam/qibotn.git", branch = "list_backends" }
 stim = "^1.12.0"
 
 [tool.poe.tasks]
 test = "pytest"
 lint = "pylint src --errors-only"
 lint-warnings = "pylint src --exit-zero"
 docs = "make -C doc html"
 docs-clean = "make -C doc clean"
 test-docs = "make -C doc doctest"
 
+
 [tool.poetry.group.cuda11]
 optional = true
 
 [tool.poetry.group.cuda11.dependencies]
 cupy-cuda11x = "^12.0.0"
 cuquantum-python-cu11 = "^23.3.0"
 qibojit = { git = "https://github.com/qiboteam/qibojit.git" }
-qibotn = { git = "https://github.com/qiboteam/qibotn.git" }
+qibotn = { git = "https://github.com/qiboteam/qibotn.git", branch = "list_backends" }
 
 [tool.poetry.group.cuda12]
 optional = true
 
 [tool.poetry.group.cuda12.dependencies]
 cupy-cuda12x = "^12.0.0"
 cuquantum-python-cu12 = "^23.3.0"
 qibojit = { git = "https://github.com/qiboteam/qibojit.git" }
-qibotn = { git = "https://github.com/qiboteam/qibotn.git" }
+qibotn = { git = "https://github.com/qiboteam/qibotn.git", branch = "list_backends" }
 
 [tool.poetry.extras]
 tensorflow = ["tensorflow"]
 torch = ["torch"]
-qinfo = ["cvxpy", "stim"]
+qinfo = ["stim"]
+
+[tool.pylint.main]
+ignored-modules = ["cvxpy"]
 
 [tool.pylint.reports]
 output-format = "colorized"
 
 [tool.coverage.run]
 omit = ["src/qibo/noise_model.py"]
```

### Comparing `qibo-0.2.7/src/qibo/__init__.py` & `qibo-0.2.8/src/qibo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,20 @@
     optimizers,
     parallel,
     parameter,
     result,
     solvers,
 )
 from qibo.backends import (
+    construct_backend,
     get_backend,
     get_device,
     get_precision,
     get_threads,
+    list_available_backends,
     matrices,
     set_backend,
     set_device,
     set_precision,
     set_threads,
 )
 from qibo.config import (
```

### Comparing `qibo-0.2.7/src/qibo/backends/_clifford_operations.py` & `qibo-0.2.8/src/qibo/backends/_clifford_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from functools import reduce
+from functools import cache, reduce
 
 import numpy as np
 from scipy import sparse
 
 name = "numpy"
 
 
@@ -325,57 +325,53 @@
 def ECR(symplectic_matrix, control_q, target_q, nqubits):
     symplectic_matrix = S(symplectic_matrix, control_q, nqubits)
     symplectic_matrix = SX(symplectic_matrix, target_q, nqubits)
     symplectic_matrix = CNOT(symplectic_matrix, control_q, target_q, nqubits)
     return X(symplectic_matrix, control_q, nqubits)
 
 
-def _exponent(x1, z1, x2, z2):
+def _exponent(
+    x1: np.ndarray, z1: np.ndarray, x2: np.ndarray, z2: np.ndarray
+) -> np.ndarray:
     """Helper function that computes the exponent to which i is raised for the product of the x and z paulis encoded in the symplectic matrix. This is used in _rowsum. The computation is performed parallely over the separated paulis x1[i], z1[i], x2[i] and z2[i].
 
     Args:
         x1 (np.array): Bits of the first x paulis.
         z1 (np.array): Bits of the first z paulis.
         x2 (np.array): Bits of the second x paulis.
         z2 (np.array): Bits of the second z paulis.
 
     Returns:
         (np.array): The calculated exponents.
     """
-    x1_ = x1.astype(np.int8)
-    x2_ = x2.astype(np.int8)
-    z1_ = z1.astype(np.int8)
-    z2_ = z2.astype(np.int8)
-    return (
-        2 * (x1_ * x2_ * (z2_ - z1_) + z1_ * z2_ * (x1_ - x2_)) - x1_ * z2_ + x2_ * z1_
-    )
+    return 2 * (x1 * x2 * (z2 - z1) + z1 * z2 * (x1 - x2)) - x1 * z2 + x2 * z1
 
 
 def _rowsum(symplectic_matrix, h, i, nqubits, determined=False):
     """Helper function that updates the symplectic matrix by setting the h-th generator equal to the (i+h)-th one. This is done to keep track of the phase of the h-th row of the symplectic matrix (r[h]). The function is applied parallely over all the rows h and i passed.
 
     Args:
         symplectic_matrix (np.array): Input symplectic matrix.
         h (np.array): Indices of the rows encoding the generators to update.
         i (np.array): Indices of the rows encoding the generators to use.
         nqubits (int): Total number of qubits.
 
     Returns:
         (np.array): The updated symplectic matrix.
     """
-    xi, xh = symplectic_matrix[i, :nqubits], symplectic_matrix[h, :nqubits]
-    zi, zh = symplectic_matrix[i, nqubits:-1], symplectic_matrix[h, nqubits:-1]
+    xi, zi = symplectic_matrix[i, :nqubits], symplectic_matrix[i, nqubits:-1]
+    xh, zh = symplectic_matrix[h, :nqubits], symplectic_matrix[h, nqubits:-1]
     exponents = _exponent(xi, zi, xh, zh)
     ind = (
         2 * symplectic_matrix[h, -1]
         + 2 * symplectic_matrix[i, -1]
         + np.sum(exponents, axis=-1)
     ) % 4 == 0
-    r = np.ones(h.shape[0], dtype=bool)
-    r[ind] = False
+    r = np.ones(h.shape[0], dtype=np.uint8)
+    r[ind] = 0
 
     xi_xh = xi ^ xh
     zi_zh = zi ^ zh
     if determined:
         r = reduce(np.logical_xor, r)
         xi_xh = reduce(np.logical_xor, xi_xh)
         zi_zh = reduce(np.logical_xor, zi_zh)
@@ -386,83 +382,152 @@
         symplectic_matrix[h, -1] = r
         symplectic_matrix[h, :nqubits] = xi_xh
         symplectic_matrix[h, nqubits:-1] = zi_zh
     return symplectic_matrix
 
 
 def _determined_outcome(state, q, nqubits):
-    state[-1, :] = False
+    state[-1, :] = 0
     idx = (state[:nqubits, q].nonzero()[0] + nqubits).astype(np.uint)
+    state = _pack_for_measurements(state, nqubits)
     state = _rowsum(
         state,
         2 * nqubits * np.ones(idx.shape, dtype=np.uint),
-        idx.astype(np.uint),
-        nqubits,
+        idx,
+        _packed_size(nqubits),
         True,
     )
-    return state, np.uint(state[-1, -1])
+    state = _unpack_for_measurements(state, nqubits)
+    return state, state[-1, -1]
 
 
 def _random_outcome(state, p, q, nqubits):
     p = p[0] + nqubits
     tmp = state[p, q].copy()
-    state[p, q] = False
+    state[p, q] = 0
     h = state[:-1, q].nonzero()[0]
     state[p, q] = tmp
     if h.shape[0] > 0:
+        state = _pack_for_measurements(state, nqubits)
         state = _rowsum(
             state,
             h.astype(np.uint),
             p * np.ones(h.shape[0], dtype=np.uint),
-            nqubits,
+            _packed_size(nqubits),
             False,
         )
+        state = _unpack_for_measurements(state, nqubits)
     state[p - nqubits, :] = state[p, :]
     outcome = np.random.randint(2, size=1).item()
-    state[p, :] = False
+    state[p, :] = 0
     state[p, -1] = outcome
-    state[p, nqubits + q] = True
+    state[p, nqubits + q] = 1
     return state, outcome
 
 
-def _get_p(state, q, nqubits):
-    return state[nqubits:-1, q].nonzero()[0]
+@cache
+def _dim(nqubits):
+    """Returns the dimension of the symplectic matrix for a given number of qubits."""
+    return 2 * nqubits + 1
+
+
+@cache
+def _packed_size(n):
+    """Returns the size of an array of `n` booleans after packing."""
+    return np.ceil(n / 8).astype(int)
+
+
+def _packbits(array, axis):
+    return np.packbits(array, axis=axis)
+
+
+def _unpackbits(array, axis):
+    return np.unpackbits(array, axis=axis)
+
+
+def _pack_for_measurements(state, nqubits):
+    """Prepares the state for measurements by packing the rows of the X and Z sections of the symplectic matrix."""
+    r, x, z = _get_rxz(state, nqubits)
+    x = _packbits(x, axis=1)
+    z = _packbits(z, axis=1)
+    return np.hstack((x, z, r[:, None]))
+
+
+@cache
+def _pad_size(n):
+    """Returns the size of the pad added to an array of original dimension `n` after unpacking."""
+    return 8 - (n % 8)
+
+
+def _unpack_for_measurements(state, nqubits):
+    """Unpacks the symplectc matrix that was packed for measurements."""
+    xz = _unpackbits(state[:, :-1], axis=1)
+    padding_size = _pad_size(nqubits)
+    x, z = xz[:, :nqubits], xz[:, nqubits + padding_size : -padding_size]
+    return np.hstack((x, z, state[:, -1][:, None]))
+
+
+def _init_state_for_measurements(state, nqubits, collapse):
+    if collapse:
+        return _unpackbits(state, axis=0)[: _dim(nqubits)]
+    else:
+        return state.copy()
 
 
 # valid for a standard basis measurement only
 def M(state, qubits, nqubits, collapse=False):
     sample = []
-    state_copy = state if collapse else state.copy()
+    state = _init_state_for_measurements(state, nqubits, collapse)
     for q in qubits:
-        p = _get_p(state_copy, q, nqubits)
+        p = state[nqubits:-1, q].nonzero()[0]
         # random outcome, affects the state
         if len(p) > 0:
-            state_copy, outcome = _random_outcome(state_copy, p, q, nqubits)
+            state, outcome = _random_outcome(state, p, q, nqubits)
         # determined outcome, state unchanged
         else:
-            state_copy, outcome = _determined_outcome(state_copy, q, nqubits)
+            state, outcome = _determined_outcome(state, q, nqubits)
         sample.append(outcome)
+    if collapse:
+        state = _packbits(state, axis=0)
     return sample
 
 
 def cast(x, dtype=None, copy=False):
     if dtype is None:
         dtype = "complex128"
     if isinstance(x, np.ndarray):
         return x.astype(dtype, copy=copy)
     elif sparse.issparse(x):  # pragma: no cover
         return x.astype(dtype, copy=copy)
     return np.array(x, dtype=dtype, copy=copy)
 
 
 def _clifford_pre_execution_reshape(state):
-    return state
+    """Reshape and packing applied to the symplectic matrix before execution to prepare the state in the form needed by each engine.
+
+    Args:
+        state (np.array): Input state.
+
+    Returns:
+        (np.array) The packed and reshaped state.
+    """
+    return _packbits(state, axis=0)
 
 
-def _clifford_post_execution_reshape(state, nqubits):
+def _clifford_post_execution_reshape(state, nqubits: int):
+    """Reshape and unpacking applied to the state after execution to retrieve the standard symplectic matrix form.
+
+    Args:
+        state (np.array): Input state.
+        nqubits (int): Number of qubits.
+
+    Returns:
+        (np.array) The unpacked and reshaped state.
+    """
+    state = _unpackbits(state, axis=0)[: _dim(nqubits)]
     return state
 
 
 def identity_density_matrix(nqubits, normalize: bool = True):
     state = np.eye(2**nqubits, dtype="complex128")
     if normalize is True:  # pragma: no cover
         state /= 2**nqubits
```

### Comparing `qibo-0.2.7/src/qibo/backends/abstract.py` & `qibo-0.2.8/src/qibo/backends/abstract.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/backends/clifford.py` & `qibo-0.2.8/src/qibo/backends/clifford.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         Returns:
             ndarray: Reshaped state.
         """
         return self.engine._clifford_pre_execution_reshape(  # pylint: disable=protected-access
             state
         )
 
-    def _clifford_post_execution_reshape(self, state, nqubits):
+    def _clifford_post_execution_reshape(self, state, nqubits: int):
         """Reshape the symplectic matrix to the shape needed by the engine after circuit execution.
 
         Args:
             state (ndarray): Input state.
             nqubits (int): Number of qubits.
 
         Returns:
@@ -290,25 +290,19 @@
 
         Returns:
             (ndarray): Samples shots.
         """
         if isinstance(qubits, list):
             qubits = tuple(qubits)
 
-        state = self._clifford_pre_execution_reshape(state)
-
         if collapse:
-            samples = [
-                self.engine.M(state, qubits, nqubits) for _ in range(nshots - 1)
-            ]  # parallelize?
+            samples = [self.engine.M(state, qubits, nqubits) for _ in range(nshots - 1)]
             samples.append(self.engine.M(state, qubits, nqubits, collapse))
         else:
-            samples = [
-                self.engine.M(state, qubits, nqubits) for _ in range(nshots)
-            ]  # parallelize?
+            samples = [self.engine.M(state, qubits, nqubits) for _ in range(nshots)]
 
         return self.engine.cast(samples, dtype=int)
 
     def symplectic_matrix_to_generators(
         self, symplectic_matrix, return_array: bool = False
     ):
         """Extract the stabilizers and destabilizers generators from symplectic matrix.
```

### Comparing `qibo-0.2.7/src/qibo/backends/einsum_utils.py` & `qibo-0.2.8/src/qibo/backends/einsum_utils.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/backends/npmatrices.py` & `qibo-0.2.8/src/qibo/backends/npmatrices.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         )
 
     def I(self, n=2):
         # dtype=complex is necessary for pytorch backend,
         # _cast will take care of casting in the right dtype for all the backends
         return self._cast(self.np.eye(n, dtype=complex), dtype=self.dtype)
 
-    def Align(self, n=2):
+    def Align(self, delay, n=2):
         return self._cast(self.I(n), dtype=self.dtype)
 
     def M(self):  # pragma: no cover
         raise_error(NotImplementedError)
 
     def RX(self, theta):
         cos = self.np.cos(theta / 2.0) + 0j
```

### Comparing `qibo-0.2.7/src/qibo/backends/numpy.py` & `qibo-0.2.8/src/qibo/backends/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -637,27 +637,31 @@
             range(len(probabilities)), size=nshots, p=probabilities
         )
 
     def aggregate_shots(self, shots):
         return self.cast(shots, dtype=shots[0].dtype)
 
     def samples_to_binary(self, samples, nqubits):
-        qrange = self.np.arange(nqubits - 1, -1, -1, dtype=self.np.int32)
-        return self.np.mod(
-            self.np.right_shift(self.cast(samples[:, None], dtype="int32"), qrange), 2
-        )
+        ### This is faster just staying @ NumPy.
+        qrange = np.arange(nqubits - 1, -1, -1, dtype=np.int32)
+        samples = self.to_numpy(samples)
+        return np.mod(np.right_shift(samples[:, None], qrange), 2)
 
     def samples_to_decimal(self, samples, nqubits):
-        qrange = self.np.arange(nqubits - 1, -1, -1, dtype=self.np.int32)
+        ### This is faster just staying @ NumPy.
+        qrange = np.arange(nqubits - 1, -1, -1, dtype=np.int32)
         qrange = (2**qrange)[:, None]
-        return self.np.matmul(samples, qrange)[:, 0]
+        samples = np.asarray(samples.tolist())
+        return np.matmul(samples, qrange)[:, 0]
 
     def calculate_frequencies(self, samples):
         # Samples are a list of strings so there is no advantage in using other backends
         res, counts = np.unique(samples, return_counts=True)
+        res = self.to_numpy(res).tolist()
+        counts = self.to_numpy(counts).tolist()
         return collections.Counter(dict(zip(res, counts)))
 
     def update_frequencies(self, frequencies, probabilities, nsamples):
         samples = self.sample_shots(probabilities, nsamples)
         res, counts = self.np.unique(samples, return_counts=True)
         frequencies[res] += counts
         return frequencies
@@ -673,14 +677,15 @@
             frequencies, nprobs, nshots % SHOT_BATCH_SIZE
         )
         return collections.Counter(
             {i: int(f) for i, f in enumerate(frequencies) if f > 0}
         )
 
     def apply_bitflips(self, noiseless_samples, bitflip_probabilities):
+        noiseless_samples = self.cast(noiseless_samples, dtype=noiseless_samples.dtype)
         fprobs = self.cast(bitflip_probabilities, dtype="float64")
         sprobs = self.cast(np.random.random(noiseless_samples.shape), dtype="float64")
         flip_0 = self.cast(sprobs < fprobs[0], dtype=noiseless_samples.dtype)
         flip_1 = self.cast(sprobs < fprobs[1], dtype=noiseless_samples.dtype)
         noisy_samples = noiseless_samples + (1 - noiseless_samples) * flip_0
         noisy_samples = noisy_samples - noiseless_samples * flip_1
         return noisy_samples
```

### Comparing `qibo-0.2.7/src/qibo/backends/pytorch.py` & `qibo-0.2.8/src/qibo/backends/pytorch.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/backends/tensorflow.py` & `qibo-0.2.8/src/qibo/backends/tensorflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,21 @@
 
 
 class TensorflowBackend(NumpyBackend):
     def __init__(self):
         super().__init__()
         self.name = "tensorflow"
         os.environ["TF_CPP_MIN_LOG_LEVEL"] = str(TF_LOG_LEVEL)
+
         import tensorflow as tf  # pylint: disable=import-error
         import tensorflow.experimental.numpy as tnp  # pylint: disable=import-error
 
+        if TF_LOG_LEVEL >= 2:
+            tf.get_logger().setLevel("ERROR")
+
         tnp.experimental_enable_numpy_behavior()
         self.tf = tf
         self.np = tnp
 
         self.versions = {
             "qibo": __version__,
             "numpy": np.__version__,
```

### Comparing `qibo-0.2.7/src/qibo/callbacks.py` & `qibo-0.2.8/src/qibo/callbacks.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/config.py` & `qibo-0.2.8/src/qibo/config.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/derivative.py` & `qibo-0.2.8/src/qibo/derivative.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/gates/abstract.py` & `qibo-0.2.8/src/qibo/gates/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
     def apply(self, backend, state, nqubits):
         return backend.apply_gate(self, state, nqubits)
 
     def apply_density_matrix(self, backend, state, nqubits):
         return backend.apply_gate_density_matrix(self, state, nqubits)
 
     def apply_clifford(self, backend, state, nqubits):
-        return backend.apply_gate_clifford(self, state[:-1], nqubits)
+        return backend.apply_gate_clifford(self, state, nqubits)
 
 
 class SpecialGate(Gate):
     """Abstract class for special gates."""
 
     def commutes(self, gate):
         return False
```

### Comparing `qibo-0.2.7/src/qibo/gates/channels.py` & `qibo-0.2.8/src/qibo/gates/channels.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/gates/gates.py` & `qibo-0.2.8/src/qibo/gates/gates.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,38 +499,39 @@
         return True
 
     @property
     def qasm_label(self):
         return "id"
 
 
-class Align(Gate):
+class Align(ParametrizedGate):
     """Aligns proceeding qubit operations and (optionally) waits ``delay`` amount of time.
 
     Args:
-        *q (int): The qubit ID numbers.
+        q (int): The qubit ID.
         delay (int, optional): The time (in ns) for which to delay circuit execution on the specified qubits.
             Defaults to ``0`` (zero).
     """
 
-    def __init__(self, *q, delay: int = 0):
+    def __init__(self, q, delay=0, trainable=True):
         if not isinstance(delay, int):
             raise_error(
                 TypeError, f"delay must be type int, but it is type {type(delay)}."
             )
         if delay < 0.0:
             raise_error(ValueError, "Delay must not be negative.")
 
-        super().__init__()
+        super().__init__(trainable)
         self.name = "align"
-        self.delay = delay
         self.draw_label = f"A({delay})"
-        self.init_args = q
-        self.init_kwargs = {"delay": delay}
-        self.target_qubits = tuple(q)
+        self.init_args = [q]
+        self.init_kwargs = {"name": self.name, "delay": delay, "trainable": trainable}
+        self.target_qubits = (q,)
+        self._parameters = (delay,)
+        self.nparams = 1
 
 
 def _is_clifford_given_angle(angle):
     """Helper function to update Clifford boolean condition according to the given angle ``angle``."""
     return isinstance(angle, (float, int)) and (angle % (np.pi / 2)).is_integer()
```

### Comparing `qibo-0.2.7/src/qibo/gates/measurements.py` & `qibo-0.2.8/src/qibo/gates/measurements.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/gates/special.py` & `qibo-0.2.8/src/qibo/gates/special.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/hamiltonians/abstract.py` & `qibo-0.2.8/src/qibo/hamiltonians/abstract.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/hamiltonians/adiabatic.py` & `qibo-0.2.8/src/qibo/hamiltonians/adiabatic.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/hamiltonians/hamiltonians.py` & `qibo-0.2.8/src/qibo/hamiltonians/hamiltonians.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         Return:
             Energy fluctuation value (float).
         """
         state = self.backend.cast(state)
         energy = self.expectation(state)
         h = self.matrix
         h2 = Hamiltonian(nqubits=self.nqubits, matrix=h @ h, backend=self.backend)
-        average_h2 = self.backend.calculate_expectation_state(h2, state, normalize=True)
+        average_h2 = h2.expectation(state, normalize=True)
         return np.sqrt(np.abs(average_h2 - energy**2))
 
     def __add__(self, o):
         if isinstance(o, self.__class__):
             if self.nqubits != o.nqubits:
                 raise_error(
                     RuntimeError,
```

### Comparing `qibo-0.2.7/src/qibo/hamiltonians/models.py` & `qibo-0.2.8/src/qibo/hamiltonians/models.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/hamiltonians/terms.py` & `qibo-0.2.8/src/qibo/hamiltonians/terms.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/measurements.py` & `qibo-0.2.8/src/qibo/measurements.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/models/_openqasm.py` & `qibo-0.2.8/src/qibo/models/_openqasm.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/models/circuit.py` & `qibo-0.2.8/src/qibo/models/circuit.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/models/dbi/double_bracket.py` & `qibo-0.2.8/src/qibo/models/dbi/double_bracket.py`

 * *Files 24% similar despite different names*

```diff
@@ -52,42 +52,63 @@
         self.h = hamiltonian
         self.h0 = deepcopy(self.h)
         self.mode = mode
 
     def __call__(
         self, step: float, mode: DoubleBracketGeneratorType = None, d: np.array = None
     ):
+        r"""We use convention that $H' = U^\dagger H U$ where $U=e^{-sW}$ with $W=[D,H]$ (or depending on `mode` an approximation, see `eval_dbr_unitary`). If $s>0$ then for $D = \Delta(H)$ the GWW DBR will give a $\sigma$-decrease, see https://arxiv.org/abs/2206.11772."""
+
+        operator = self.eval_dbr_unitary(step, mode, d)
+        operator_dagger = self.backend.cast(
+            np.matrix(self.backend.to_numpy(operator)).getH()
+        )
+        self.h.matrix = operator_dagger @ self.h.matrix @ operator
+        return operator
+
+    def eval_dbr_unitary(
+        self, step: float, mode: DoubleBracketGeneratorType = None, d: np.array = None
+    ):
+        """In call we will are working in the convention that $H' = U^\\dagger H U$ where $U=e^{-sW}$ with $W=[D,H]$ or an approximation of that by a group commutator. That is handy because if we switch from the DBI in the Heisenberg picture for the Hamiltonian, we get that the transformation of the state is $|\\psi'\rangle = U |\\psi\rangle$ so that $\\langle H\rangle_{\\psi'} = \\langle H' \rangle_\\psi$ (i.e. when writing the unitary acting on the state dagger notation is avoided).
+
+        The group commutator must approximate $U=e^{-s[D,H]}$. This is achieved by setting $r = \\sqrt{s}$ so that
+        $$V = e^{-irH}e^{irD}e^{irH}e^{-irD}$$
+        because
+        $$e^{-irH}De^{irH} = D+ir[D,H]+O(r^2)$$
+        so
+        $$V\approx e^{irD +i^2 r^2[D,H] + O(r^2) -irD} \approx U\\ .$$
+        See the app in https://arxiv.org/abs/2206.11772 for a derivation.
+        """
         if mode is None:
             mode = self.mode
 
         if mode is DoubleBracketGeneratorType.canonical:
             operator = self.backend.calculate_matrix_exp(
-                1.0j * step,
+                -1.0j * step,
                 self.commutator(self.diagonal_h_matrix, self.h.matrix),
             )
         elif mode is DoubleBracketGeneratorType.single_commutator:
             if d is None:
                 d = self.diagonal_h_matrix
             operator = self.backend.calculate_matrix_exp(
-                1.0j * step,
+                -1.0j * step,
                 self.commutator(d, self.h.matrix),
             )
         elif mode is DoubleBracketGeneratorType.group_commutator:
             if d is None:
                 d = self.diagonal_h_matrix
+
+            sqrt_step = np.sqrt(step)
             operator = (
-                self.h.exp(-step)
-                @ self.backend.calculate_matrix_exp(-step, d)
-                @ self.h.exp(step)
-                @ self.backend.calculate_matrix_exp(step, d)
+                self.h.exp(sqrt_step)
+                @ self.backend.calculate_matrix_exp(-sqrt_step, d)
+                @ self.h.exp(-sqrt_step)
+                @ self.backend.calculate_matrix_exp(sqrt_step, d)
             )
-        operator_dagger = self.backend.cast(
-            np.matrix(self.backend.to_numpy(operator)).getH()
-        )
-        self.h.matrix = operator @ self.h.matrix @ operator_dagger
+        return operator
 
     @staticmethod
     def commutator(a, b):
         """Compute commutator between two arrays."""
         return a @ b - b @ a
 
     @property
```

### Comparing `qibo-0.2.7/src/qibo/models/dbi/utils.py` & `qibo-0.2.8/src/qibo/models/dbi/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,19 +129,21 @@
                 step_max=step_max,
                 space=hp.uniform,
                 optimizer=tpe,
                 max_evals=max_evals,
             )
         else:
             step_best = step
-        dbi_eval(step=step_best)
-        optimal_steps.append(step_best)
-        norms_off_diagonal_restriction.append(dbi_eval.off_diagonal_norm)
+        dbi_object(step=step)
+        optimal_steps.append(step)
+        norms_off_diagonal_restriction.append(dbi_object.off_diagonal_norm)
     # find best d
-    idx_max_loss = np.argmin(norms_off_diagonal_restriction)
+    idx_max_loss = norms_off_diagonal_restriction.index(
+        min(norms_off_diagonal_restriction)
+    )
     flip = flip_list[idx_max_loss]
     step_optimal = optimal_steps[idx_max_loss]
     dbi_eval = deepcopy(dbi_object)
     if idx_max_loss == len(d_list) and compare_canonical is True:
         # canonical
         dbi_eval(step=step_optimal, mode=DoubleBracketGeneratorType.canonical)
```

### Comparing `qibo-0.2.7/src/qibo/models/distcircuit.py` & `qibo-0.2.8/src/qibo/models/distcircuit.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/models/encodings.py` & `qibo-0.2.8/src/qibo/models/encodings.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/models/error_mitigation.py` & `qibo-0.2.8/src/qibo/models/error_mitigation.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from itertools import product
 
 import numpy as np
 from scipy.optimize import curve_fit
 
 from qibo import gates
-from qibo.backends import GlobalBackend, _check_backend
+from qibo.backends import GlobalBackend, _check_backend, _check_backend_and_local_state
 from qibo.config import raise_error
 
 
 def get_gammas(noise_levels, analytical: bool = True):
     """Standalone function to compute the ZNE coefficients given the noise levels.
 
     Args:
@@ -106,14 +106,15 @@
     noise_levels,
     noise_model=None,
     nshots=10000,
     solve_for_gammas=False,
     insertion_gate="CNOT",
     readout=None,
     qubit_map=None,
+    seed=None,
     backend=None,
 ):
     """Runs the Zero Noise Extrapolation method for error mitigation.
 
     The different noise levels are realized by the insertion of pairs of
     either ``CNOT`` or ``RX(pi/2)`` gates that resolve to the identiy in
     the noise-free case.
@@ -132,27 +133,31 @@
             Defaults to ``"CNOT"``.
         readout (dict, optional): a dictionary that may contain the following keys:
 
             *    ncircuits: int, specifies the number of random circuits to use for the randomized method of readout error mitigation.
             *    response_matrix: numpy.ndarray, used for applying a pre-computed response matrix for readout error mitigation.
             *    ibu_iters: int, specifies the number of iterations for the iterative Bayesian unfolding method of readout error mitigation. If provided, the corresponding readout error mitigation method is used. Defaults to {}.
 
-        qubit_map (list, optional): the qubit map. If None, a list of range of circuit's qubits is used. Defaults to ``None``.
+        qubit_map (list, optional): the qubit map. If None, a list of range of circuit's qubits is used.
+            Defaults to ``None``.
+        seed (int or :class:`numpy.random.Generator`, optional): Either a generator of random
+            numbers or a fixed seed to initialize a generator. If ``None``, initializes
+            a generator with a random seed. Default: ``None``.
         backend (:class:`qibo.backends.abstract.Backend`, optional): backend to be used
             in the execution. If ``None``, it uses :class:`qibo.backends.GlobalBackend`.
             Defaults to ``None``.
 
     Returns:
         numpy.ndarray: Estimate of the expected value of ``observable`` in the noise free condition.
 
     Reference:
         1. K. Temme, S. Bravyi et al, *Error mitigation for short-depth quantum circuits*.
            `arXiv:1612.02058 [quant-ph] <https://arxiv.org/abs/1612.02058>`_.
     """
-    backend = _check_backend(backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     if readout is None:
         readout = {}
 
     expected_values = []
     for num_insertions in noise_levels:
         noisy_circuit = get_noisy_circuit(
@@ -161,47 +166,52 @@
         val = get_expectation_val_with_readout_mitigation(
             noisy_circuit,
             observable,
             noise_model,
             nshots,
             readout,
             qubit_map,
+            seed=local_state,
             backend=backend,
         )
         expected_values.append(val)
 
     gamma = get_gammas(noise_levels, analytical=solve_for_gammas)
 
     return np.sum(gamma * expected_values)
 
 
 def sample_training_circuit_cdr(
     circuit,
     replacement_gates: list = None,
     sigma: float = 0.5,
+    seed=None,
     backend=None,
 ):
     """Samples a training circuit for CDR by susbtituting some of the non-Clifford gates.
 
     Args:
         circuit (:class:`qibo.models.Circuit`): circuit to sample from,
             decomposed in ``RX(pi/2)``, ``X``, ``CNOT`` and ``RZ`` gates.
         replacement_gates (list, optional): candidates for the substitution of the
             non-Clifford gates. The ``list`` should be composed by ``tuples`` of the
             form (``gates.XYZ``, ``kwargs``). For example, phase gates are used by default:
             ``list((RZ, {'theta':0}), (RZ, {'theta':pi/2}), (RZ, {'theta':pi}), (RZ, {'theta':3*pi/2}))``.
         sigma (float, optional): standard devation of the Gaussian distribution used for sampling.
+        seed (int or :class:`numpy.random.Generator`, optional): Either a generator of random
+            numbers or a fixed seed to initialize a generator. If ``None``, initializes
+            a generator with a random seed. Default: ``None``.
         backend (:class:`qibo.backends.abstract.Backend`, optional): backend to be used
             in the execution. If ``None``, it uses :class:`qibo.backends.GlobalBackend`.
             Defaults to ``None``.
 
     Returns:
         :class:`qibo.models.Circuit`: The sampled circuit.
     """
-    backend = _check_backend(backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     if replacement_gates is None:
         replacement_gates = [(gates.RZ, {"theta": n * np.pi / 2}) for n in range(4)]
 
     gates_to_replace = []
     for i, gate in enumerate(circuit.queue):
         if isinstance(gate, gates.RZ):
@@ -217,36 +227,39 @@
             [rg(*gate.init_args, **kwargs) for rg, kwargs in replacement_gates]
         )
 
         replacement.append(rep_gates)
         distance.append(
             np.linalg.norm(
                 gate.matrix(backend)
-                - [rep_gate.matrix(backend) for rep_gate in rep_gates],
+                - backend.cast([rep_gate.matrix(backend) for rep_gate in rep_gates]),
                 ord="fro",
                 axis=(1, 2),
             )
         )
 
     distance = np.vstack(distance)
     prob = np.exp(-(distance**2) / sigma**2)
+    prob = backend.cast(prob, dtype=prob.dtype)
 
-    index = np.random.choice(
+    index = local_state.choice(
         range(len(gates_to_replace)),
         size=min(int(len(gates_to_replace) / 2), 50),
         replace=False,
-        p=prob.sum(-1) / prob.sum(),
+        p=backend.to_numpy(backend.np.sum(prob, -1) / backend.np.sum(prob)),
     )
 
     gates_to_replace = np.array([gates_to_replace[i] for i in index])
     prob = [prob[i] for i in index]
+    prob = backend.cast(prob, dtype=prob[0].dtype)
+    prob = backend.to_numpy(prob)
 
     replacement = np.array([replacement[i] for i in index])
     replacement = [
-        replacement[i][np.random.choice(range(len(p)), size=1, p=p / p.sum())[0]]
+        replacement[i][local_state.choice(range(len(p)), size=1, p=p / np.sum(p))[0]]
         for i, p in enumerate(prob)
     ]
     replacement = {i[0]: g for i, g in zip(gates_to_replace, replacement)}
 
     sampled_circuit = circuit.__class__(**circuit.init_kwargs)
     for i, gate in enumerate(circuit.queue):
         sampled_circuit.add(replacement.get(i, gate))
@@ -260,14 +273,15 @@
     noise_model,
     nshots: int = 10000,
     model=lambda x, a, b: a * x + b,
     n_training_samples: int = 100,
     full_output: bool = False,
     readout=None,
     qubit_map=None,
+    seed=None,
     backend=None,
 ):
     """Runs the Clifford Data Regression error mitigation method.
 
     Args:
         circuit (:class:`qibo.models.Circuit`): input circuit decomposed in the
             primitive gates ``X``, ``CNOT``, ``RX(pi/2)``, ``RZ(theta)``.
@@ -283,56 +297,75 @@
             information: ``val``, ``optimal_params``, ``train_val``. Defaults to ``False``.
         readout (dict, optional): a dictionary that may contain the following keys:
 
             *    ncircuits: int, specifies the number of random circuits to use for the randomized method of readout error mitigation.
             *    response_matrix: numpy.ndarray, used for applying a pre-computed response matrix for readout error mitigation.
             *    ibu_iters: int, specifies the number of iterations for the iterative Bayesian unfolding method of readout error mitigation. If provided, the corresponding readout error mitigation method is used. Defaults to {}.
 
-        qubit_map (list, optional): the qubit map. If None, a list of range of circuit's qubits is used. Defaults to ``None``.
+        qubit_map (list, optional): the qubit map. If None, a list of range of circuit's qubits is used.
+            Defaults to ``None``.
+        seed (int or :class:`numpy.random.Generator`, optional): Either a generator of random
+            numbers or a fixed seed to initialize a generator. If ``None``, initializes
+            a generator with a random seed. Default: ``None``.
         backend (:class:`qibo.backends.abstract.Backend`, optional): backend to be used
             in the execution. If ``None``, it uses :class:`qibo.backends.GlobalBackend`.
             Defaults to ``None``.
 
     Returns:
         mit_val (float): Mitigated expectation value of `observable`.
         val (float): Noisy expectation value of `observable`.
         optimal_params (list): Optimal values for `params`.
         train_val (dict): Contains the noise-free and noisy expectation values obtained with the training circuits.
 
     Reference:
         1. P. Czarnik, A. Arrasmith et al, *Error mitigation with Clifford quantum-circuit data*.
            `arXiv:2005.10189 [quant-ph] <https://arxiv.org/abs/2005.10189>`_.
     """
-    backend = _check_backend(backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     if readout is None:
         readout = {}
 
     training_circuits = [
-        sample_training_circuit_cdr(circuit) for _ in range(n_training_samples)
+        sample_training_circuit_cdr(circuit, seed=local_state, backend=backend)
+        for _ in range(n_training_samples)
     ]
 
     train_val = {"noise-free": [], "noisy": []}
     for circ in training_circuits:
         result = backend.execute_circuit(circ, nshots=nshots)
         val = result.expectation_from_samples(observable)
         train_val["noise-free"].append(val)
         val = get_expectation_val_with_readout_mitigation(
-            circ, observable, noise_model, nshots, readout, qubit_map, backend=backend
+            circ,
+            observable,
+            noise_model,
+            nshots,
+            readout,
+            qubit_map,
+            seed=local_state,
+            backend=backend,
         )
         train_val["noisy"].append(val)
 
     optimal_params = curve_fit(model, train_val["noisy"], train_val["noise-free"])[0]
 
     val = get_expectation_val_with_readout_mitigation(
-        circuit, observable, noise_model, nshots, readout, qubit_map, backend=backend
+        circuit,
+        observable,
+        noise_model,
+        nshots,
+        readout,
+        qubit_map,
+        seed=local_state,
+        backend=backend,
     )
     mit_val = model(val, *optimal_params)
 
-    if full_output is True:
+    if full_output:
         return mit_val, val, optimal_params, train_val
 
     return mit_val
 
 
 def vnCDR(
     circuit,
@@ -342,14 +375,15 @@
     nshots: int = 10000,
     model=lambda x, *params: (x * np.array(params).reshape(-1, 1)).sum(0),
     n_training_samples: int = 100,
     insertion_gate: str = "CNOT",
     full_output: bool = False,
     readout=None,
     qubit_map=None,
+    seed=None,
     backend=None,
 ):
     """Runs the variable-noise Clifford Data Regression error mitigation method.
 
     Args:
         circuit (:class:`qibo.models.Circuit`): input circuit decomposed in the
             primitive gates ``X``, ``CNOT``, ``RX(pi/2)``, ``RZ(theta)``.
@@ -370,14 +404,17 @@
         readout (dict, optional): a dictionary that may contain the following keys:
 
             *    ncircuits: int, specifies the number of random circuits to use for the randomized method of readout error mitigation.
             *    response_matrix: numpy.ndarray, used for applying a pre-computed response matrix for readout error mitigation.
             *    ibu_iters: int, specifies the number of iterations for the iterative Bayesian unfolding method of readout error mitigation. If provided, the corresponding readout error mitigation method is used. Defaults to {}.
 
         qubit_map (list, optional): the qubit map. If None, a list of range of circuit's qubits is used. Defaults to ``None``.
+        seed (int or :class:`numpy.random.Generator`, optional): Either a generator of random
+            numbers or a fixed seed to initialize a generator. If ``None``, initializes
+            a generator with a random seed. Default: ``None``.
         backend (:class:`qibo.backends.abstract.Backend`, optional): backend to be used
             in the execution. If ``None``, it uses :class:`qibo.backends.GlobalBackend`.
             Defaults to ``None``.
 
     Returns:
         mit_val (float): Mitigated expectation value of `observable`.
         val (list): Expectation value of `observable` with increased noise levels.
@@ -385,21 +422,22 @@
         train_val (dict): Contains the noise-free and noisy expectation values obtained
         with the training circuits.
 
     Reference:
         1. A. Lowe, MH. Gordon et al, *Unified approach to data-driven quantum error mitigation*.
            `arXiv:2011.01157 [quant-ph] <https://arxiv.org/abs/2011.01157>`_.
     """
-    backend = _check_backend(backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     if readout is None:
         readout = {}
 
     training_circuits = [
-        sample_training_circuit_cdr(circuit) for _ in range(n_training_samples)
+        sample_training_circuit_cdr(circuit, seed=local_state, backend=backend)
+        for _ in range(n_training_samples)
     ]
     train_val = {"noise-free": [], "noisy": []}
 
     for circ in training_circuits:
         result = backend.execute_circuit(circ, nshots=nshots)
         val = result.expectation_from_samples(observable)
         train_val["noise-free"].append(val)
@@ -408,40 +446,42 @@
             val = get_expectation_val_with_readout_mitigation(
                 noisy_c,
                 observable,
                 noise_model,
                 nshots,
                 readout,
                 qubit_map,
+                seed=local_state,
                 backend=backend,
             )
             train_val["noisy"].append(val)
 
     noisy_array = np.array(train_val["noisy"]).reshape(-1, len(noise_levels))
 
-    params = np.random.rand(len(noise_levels))
+    params = local_state.random(len(noise_levels))
     optimal_params = curve_fit(model, noisy_array.T, train_val["noise-free"], p0=params)
 
     val = []
     for level in noise_levels:
         noisy_c = get_noisy_circuit(circuit, level, insertion_gate=insertion_gate)
         expval = get_expectation_val_with_readout_mitigation(
             noisy_c,
             observable,
             noise_model,
             nshots,
             readout,
             qubit_map,
+            seed=local_state,
             backend=backend,
         )
         val.append(expval)
 
     mit_val = model(np.array(val).reshape(-1, 1), *optimal_params[0])[0]
 
-    if full_output is True:
+    if full_output:
         return mit_val, val, optimal_params, train_val
 
     return mit_val
 
 
 def iterative_bayesian_unfolding(probabilities, response_matrix, iterations=10):
     """
@@ -563,55 +603,67 @@
 
 def apply_randomized_readout_mitigation(
     circuit,
     noise_model=None,
     nshots: int = 10000,
     ncircuits: int = 10,
     qubit_map=None,
+    seed=None,
     backend=None,
 ):
-    """Readout mitigation method that transforms the bias in an expectation value into a measurable multiplicative factor. This factor can be eliminated at the expense of increased sampling complexity for the observable.
+    """Readout mitigation method that transforms the bias in an expectation value into a
+    measurable multiplicative factor.
+
+    This factor can be eliminated at the expense of increased sampling complexity
+    for the observable.
 
     Args:
         circuit (:class:`qibo.models.Circuit`): input circuit.
         noise_model(:class:`qibo.noise.NoiseModel`, optional): noise model used for
             simulating noisy computation. Defaults to ``None``.
         nshots (int, optional): number of shots. Defaults to :math:`10000`.
         ncircuits (int, optional): number of randomized circuits. Each of them uses
             ``int(nshots / ncircuits)`` shots. Defaults to 10.
-        qubit_map (list, optional): the qubit map. If None, a list of range of circuit's qubits is used. Defaults to ``None``.
+        qubit_map (list, optional): the qubit map. If None, a list of range of circuit's qubits is used.
+            Defaults to ``None``.
+        seed (int or :class:`numpy.random.Generator`, optional): Either a generator of random
+            numbers or a fixed seed to initialize a generator. If ``None``, initializes
+            a generator with a random seed. Default: ``None``.
         backend (:class:`qibo.backends.abstract.Backend`, optional): backend to be used
             in the execution. If ``None``, it uses :class:`qibo.backends.GlobalBackend`.
             Defaults to ``None``.
 
     Return:
         :class:`qibo.measurements.CircuitResult`: the state of the input circuit with
             mitigated frequencies.
 
 
     Reference:
-        1. Ewout van den Berg, Zlatko K. Minev et al, *Model-free readout-error mitigation for quantum expectation values*.
+        1. Ewout van den Berg, Zlatko K. Minev et al,
+        *Model-free readout-error mitigation for quantum expectation values*.
            `arXiv:2012.09738 [quant-ph] <https://arxiv.org/abs/2012.09738>`_.
     """
     from qibo import Circuit  # pylint: disable=import-outside-toplevel
     from qibo.quantum_info import (  # pylint: disable=import-outside-toplevel
         random_pauli,
     )
 
-    backend = _check_backend(backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     meas_qubits = circuit.measurements[0].qubits
     nshots_r = int(nshots / ncircuits)
     freq = np.zeros((ncircuits, 2), object)
     for k in range(ncircuits):
         circuit_c = circuit.copy(True)
         circuit_c.queue.pop()
         cal_circuit = Circuit(circuit.nqubits, density_matrix=True)
 
-        x_gate = random_pauli(circuit.nqubits, 1, subset=["I", "X"]).queue
+        x_gate = random_pauli(
+            circuit.nqubits, 1, subset=["I", "X"], seed=local_state
+        ).queue
 
         error_map = {}
         for j, gate in enumerate(x_gate):
             if isinstance(gate, gates.X) and gate.qubits[0] in meas_qubits:
                 error_map[gate.qubits[0]] = 1
 
         circuits = [circuit_c, cal_circuit]
@@ -642,14 +694,15 @@
 def get_expectation_val_with_readout_mitigation(
     circuit,
     observable,
     noise_model=None,
     nshots: int = 10000,
     readout=None,
     qubit_map=None,
+    seed=None,
     backend=None,
 ):
     """
     Applies readout error mitigation to the given circuit and observable.
 
     Args:
         circuit (qibo.models.Circuit): input circuit.
@@ -658,29 +711,38 @@
         nshots (int, optional): the number of shots for the circuit execution. Defaults to :math:`10000`.
         readout (dict, optional): a dictionary that may contain the following keys:
 
             *    ncircuits: int, specifies the number of random circuits to use for the randomized method of readout error mitigation.
             *    response_matrix: numpy.ndarray, used for applying a pre-computed response matrix for readout error mitigation.
             *    ibu_iters: int, specifies the number of iterations for the iterative Bayesian unfolding method of readout error mitigation. If provided, the corresponding readout error mitigation method is used. Defaults to {}.
 
-        qubit_map (list, optional): the qubit map. If None, a list of range of circuit's qubits is used. Defaults to ``None``.
+        qubit_map (list, optional): the qubit map. If None, a list of range of circuit's qubits is used.
+            Defaults to ``None``.
+        seed (int or :class:`numpy.random.Generator`, optional): Either a generator of random
+            numbers or a fixed seed to initialize a generator. If ``None``, initializes
+            a generator with a random seed. Default: ``None``.
         backend (qibo.backends.abstract.Backend, optional): the backend to be used in the execution.
             If None, it uses the global backend. Defaults to ``None``.
 
     Returns:
         float: the mitigated expectation value of the observable.
     """
-    backend = _check_backend(backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     if readout is None:  # pragma: no cover
         readout = {}
 
     if "ncircuits" in readout:
         circuit_result, circuit_result_cal = apply_randomized_readout_mitigation(
-            circuit, noise_model, nshots, readout["ncircuits"], backend
+            circuit,
+            noise_model,
+            nshots,
+            readout["ncircuits"],
+            seed=local_state,
+            backend=backend,
         )
     else:
         circuit_result = _execute_circuit(
             circuit, qubit_map, noise_model, nshots, backend=backend
         )
         if "response_matrix" in readout:
             circuit_result = apply_resp_mat_readout_mitigation(
@@ -695,32 +757,36 @@
         exp_val /= circuit_result_cal.expectation_from_samples(observable)
 
     return exp_val
 
 
 def sample_clifford_training_circuit(
     circuit,
+    seed=None,
     backend=None,
 ):
     """Samples a training circuit for CDR by susbtituting all the non-Clifford gates.
 
     Args:
         circuit (:class:`qibo.models.Circuit`): circuit to sample from.
+        seed (int or :class:`numpy.random.Generator`, optional): Either a generator of random
+            numbers or a fixed seed to initialize a generator. If ``None``, initializes
+            a generator with a random seed. Default: ``None``.
         backend (:class:`qibo.backends.abstract.Backend`, optional): backend to be used
             in the execution. If ``None``, it uses :class:`qibo.backends.GlobalBackend`.
             Defaults to ``None``.
 
     Returns:
         :class:`qibo.models.Circuit`: the sampled circuit.
     """
     from qibo.quantum_info import (  # pylint: disable=import-outside-toplevel
         random_clifford,
     )
 
-    backend = _check_backend(backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     non_clifford_gates_indices = [
         i
         for i, gate in enumerate(circuit.queue)
         if not gate.clifford and not isinstance(gate, gates.M)
     ]
 
@@ -729,63 +795,75 @@
 
     sampled_circuit = circuit.__class__(**circuit.init_kwargs)
 
     for i, gate in enumerate(circuit.queue):
         if isinstance(gate, gates.M):
             for q in gate.qubits:
                 gate_rand = gates.Unitary(
-                    random_clifford(1, backend=backend, return_circuit=False),
+                    random_clifford(
+                        1, return_circuit=False, seed=local_state, backend=backend
+                    ),
                     q,
                 )
                 gate_rand.clifford = True
                 sampled_circuit.add(gate_rand)
             sampled_circuit.add(gate)
         else:
             if i in non_clifford_gates_indices:
                 gate = gates.Unitary(
                     random_clifford(
-                        len(gate.qubits), backend=backend, return_circuit=False
+                        len(gate.qubits),
+                        return_circuit=False,
+                        seed=local_state,
+                        backend=backend,
                     ),
                     *gate.qubits,
                 )
                 gate.clifford = True
             sampled_circuit.add(gate)
 
     return sampled_circuit
 
 
-def error_sensitive_circuit(circuit, observable, backend=None):
+def error_sensitive_circuit(circuit, observable, seed=None, backend=None):
     """
     Generates a Clifford circuit that preserves the same circuit frame as the input circuit, and stabilizes the specified Pauli observable.
 
     Args:
         circuit (:class:`qibo.models.Circuit`): input circuit.
-        observable (:class:`qibo.hamiltonians.Hamiltonian/:class:`qibo.hamiltonians.SymbolicHamiltonian`): Pauli observable to be measured.
+        observable (:class:`qibo.hamiltonians.Hamiltonian` or :class:`qibo.hamiltonians.SymbolicHamiltonian`):
+            Pauli observable to be measured.
+        seed (int or :class:`numpy.random.Generator`, optional): Either a generator of random
+            numbers or a fixed seed to initialize a generator. If ``None``, initializes
+            a generator with a random seed. Default: ``None``.
         backend (:class:`qibo.backends.abstract.Backend`, optional): backend to be used
             in the execution. if ``None``, it uses :class:`qibo.backends.GlobalBackend`.
             Defaults to ``None``.
 
     Returns:
         :class:`qibo.models.Circuit`: the error sensitive circuit.
         :class:`qibo.models.Circuit`: the sampled Clifford circuit.
         list: the list of adjustment gates.
 
     Reference:
         1. Dayue Qin, Yanzhu Chen et al, *Error statistics and scalability of quantum error mitigation formulas*.
            `arXiv:2112.06255 [quant-ph] <https://arxiv.org/abs/2112.06255>`_.
     """
+    from qibo import matrices  # pylint: disable=import-outside-toplevel
     from qibo.quantum_info import (  # pylint: disable=import-outside-toplevel
         comp_basis_to_pauli,
         random_clifford,
         vectorization,
     )
 
-    backend = _check_backend(backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
-    sampled_circuit = sample_clifford_training_circuit(circuit, backend=backend)
+    sampled_circuit = sample_clifford_training_circuit(
+        circuit, seed=local_state, backend=backend
+    )
     unitary_matrix = sampled_circuit.unitary(backend=backend)
     num_qubits = sampled_circuit.nqubits
 
     comp_to_pauli = comp_basis_to_pauli(num_qubits, backend=backend)
     observable.nqubits = num_qubits
     observable_liouville = vectorization(
         backend.np.transpose(backend.np.conj(unitary_matrix), (1, 0))
@@ -799,28 +877,30 @@
     index = int(
         backend.np.where(backend.np.abs(observable_pauli_liouville) >= 1e-5)[0][0]
     )
 
     observable_pauli = list(product(["I", "X", "Y", "Z"], repeat=num_qubits))[index]
 
     pauli_gates = {
-        "I": backend.cast(gates.I(0).matrix(backend=backend)),
-        "X": backend.cast(gates.X(0).matrix(backend=backend)),
-        "Y": backend.cast(gates.Y(0).matrix(backend=backend)),
-        "Z": backend.cast(gates.Z(0).matrix(backend=backend)),
+        "I": backend.cast(matrices.I, dtype=matrices.I.dtype),
+        "X": backend.cast(matrices.X, dtype=matrices.X.dtype),
+        "Y": backend.cast(matrices.Y, dtype=matrices.Y.dtype),
+        "Z": backend.cast(matrices.Z, dtype=matrices.Z.dtype),
     }
 
     adjustment_gates = []
     for i in range(num_qubits):
         observable_i = pauli_gates[observable_pauli[i]]
         random_init = pauli_gates["I"]
         while backend.np.any(
             backend.np.abs(observable_i - pauli_gates["Z"]) > 1e-5
         ) and backend.np.any(abs(observable_i - pauli_gates["I"]) > 1e-5):
-            random_init = random_clifford(1, backend=backend, return_circuit=False)
+            random_init = random_clifford(
+                1, return_circuit=False, seed=local_state, backend=backend
+            )
             observable_i = (
                 backend.np.conj(backend.np.transpose(random_init, (1, 0)))
                 @ pauli_gates[observable_pauli[i]]
                 @ random_init
             )
 
         adjustment_gate = gates.Unitary(random_init, i)
@@ -842,34 +922,39 @@
     observable,
     readout=None,
     qubit_map=None,
     noise_model=None,
     nshots=int(1e4),
     n_training_samples=10,
     full_output=False,
+    seed=None,
     backend=None,
 ):
     """
     Computes the Important Clifford Sampling method.
 
     Args:
         circuit (:class:`qibo.models.Circuit`): input circuit.
         observable (:class:`qibo.hamiltonians.Hamiltonian/:class:`qibo.hamiltonians.SymbolicHamiltonian`): the observable to be measured.
         readout (dict, optional): a dictionary that may contain the following keys:
 
             *    ncircuits: int, specifies the number of random circuits to use for the randomized method of readout error mitigation.
             *    response_matrix: numpy.ndarray, used for applying a pre-computed response matrix for readout error mitigation.
             *    ibu_iters: int, specifies the number of iterations for the iterative Bayesian unfolding method of readout error mitigation. If provided, the corresponding readout error mitigation method is used. Defaults to {}.
 
-        qubit_map (list, optional): the qubit map. If ``None``, a list of range of circuit's qubits is used. Defaults to ``None``.
+        qubit_map (list, optional): the qubit map. If ``None``, a list of range of circuit's qubits is used.
+            Defaults to ``None``.
         noise_model (qibo.models.noise.Noise, optional): the noise model to be applied. Defaults to ``None``.
         nshots (int, optional): the number of shots for the circuit execution. Defaults to :math:`10000`.
         n_training_samples (int, optional): the number of training samples. Defaults to 10.
         full_output (bool, optional): if ``True``, this function returns additional
             information: ``val``, ``optimal_params``, ``train_val``. Defaults to ``False``.
+        seed (int or :class:`numpy.random.Generator`, optional): Either a generator of random
+            numbers or a fixed seed to initialize a generator. If ``None``, initializes
+            a generator with a random seed. Default: ``None``.
         backend (qibo.backends.abstract.Backend, optional): the backend to be used in the execution.
             If None, it uses the global backend. Defaults to ``None``.
 
     Returns:
         mitigated_expectation (float): the mitigated expectated value.
         mitigated_expectation_std (float): the standard deviation of the mitigated expectated value.
         dep_param (float): the depolarizing parameter.
@@ -877,24 +962,26 @@
         lambda_list (list): the list of the depolarizing parameters.
         data (dict): the data dictionary containing the noise-free and noisy expectation values obtained with the training circuits.
 
     Reference:
         1. Dayue Qin, Yanzhu Chen et al, *Error statistics and scalability of quantum error mitigation formulas*.
            `arXiv:2112.06255 [quant-ph] <https://arxiv.org/abs/2112.06255>`_.
     """
-    backend = _check_backend(backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     if readout is None:
         readout = {}
 
     if qubit_map is None:
         qubit_map = list(range(circuit.nqubits))
 
     training_circuits = [
-        error_sensitive_circuit(circuit, observable, backend=backend)[0]
+        error_sensitive_circuit(circuit, observable, seed=local_state, backend=backend)[
+            0
+        ]
         for _ in range(n_training_samples)
     ]
 
     data = {"noise-free": [], "noisy": []}
     lambda_list = []
 
     for training_circuit in training_circuits:
@@ -904,26 +991,34 @@
         noisy_expectation = get_expectation_val_with_readout_mitigation(
             training_circuit,
             observable,
             noise_model,
             nshots,
             readout,
             qubit_map,
+            seed=local_state,
             backend=backend,
         )
 
         data["noise-free"].append(expectation)
         data["noisy"].append(noisy_expectation)
         lambda_list.append(1 - noisy_expectation / expectation)
 
     dep_param = np.mean(lambda_list)
     dep_param_std = np.std(lambda_list)
 
     noisy_expectation = get_expectation_val_with_readout_mitigation(
-        circuit, observable, noise_model, nshots, readout, qubit_map, backend=backend
+        circuit,
+        observable,
+        noise_model,
+        nshots,
+        readout,
+        qubit_map,
+        seed=local_state,
+        backend=backend,
     )
     one_dep_squared = (1 - dep_param) ** 2
     dep_std_squared = dep_param_std**2
 
     mitigated_expectation = (
         (1 - dep_param) * noisy_expectation / (one_dep_squared + dep_std_squared)
     )
```

### Comparing `qibo-0.2.7/src/qibo/models/evolution.py` & `qibo-0.2.8/src/qibo/models/evolution.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/models/grover.py` & `qibo-0.2.8/src/qibo/models/grover.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/models/hep.py` & `qibo-0.2.8/src/qibo/models/hep.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/models/iqae.py` & `qibo-0.2.8/src/qibo/models/iqae.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/models/qcnn.py` & `qibo-0.2.8/src/qibo/models/qcnn.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/models/qft.py` & `qibo-0.2.8/src/qibo/models/qft.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/models/tsp.py` & `qibo-0.2.8/src/qibo/models/tsp.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/models/utils.py` & `qibo-0.2.8/src/qibo/models/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,7 +203,14 @@
             np.arange(shifted_filtered_coeffs.shape[axis])[slice_object],
             axis=axis,
         )
 
     # Shift the filtered coefficients back
     filtered_coeffs = np.fft.ifftshift(shifted_filtered_coeffs)
     return filtered_coeffs
+
+
+def vqe_loss(params, circuit, hamiltonian):
+    circuit.set_parameters(params)
+    result = hamiltonian.backend.execute_circuit(circuit)
+    final_state = result.state()
+    return hamiltonian.expectation(final_state)
```

### Comparing `qibo-0.2.7/src/qibo/models/variational.py` & `qibo-0.2.8/src/qibo/models/variational.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from qibo.config import raise_error
-from qibo.hamiltonians import Hamiltonian
 from qibo.models.evolution import StateEvolution
+from qibo.models.utils import vqe_loss
 
 
 class VQE:
     """This class implements the variational quantum eigensolver algorithm.
 
     Args:
         circuit (:class:`qibo.models.circuit.Circuit`): Circuit that
@@ -38,14 +38,15 @@
         self.hamiltonian = hamiltonian
         self.backend = hamiltonian.backend
 
     def minimize(
         self,
         initial_state,
         method="Powell",
+        loss_func=None,
         jac=None,
         hess=None,
         hessp=None,
         bounds=None,
         constraints=(),
         tol=None,
         callback=None,
@@ -57,14 +58,15 @@
 
         Args:
             initial_state (array): a initial guess for the parameters of the
                 variational circuit.
             method (str): the desired minimization method.
                 See :meth:`qibo.optimizers.optimize` for available optimization
                 methods.
+            loss (callable): loss function, the default one is :func:`qibo.models.utils.vqe_loss`.
             jac (dict): Method for computing the gradient vector for scipy optimizers.
             hess (dict): Method for computing the hessian matrix for scipy optimizers.
             hessp (callable): Hessian of objective function times an arbitrary
                 vector for scipy optimizers.
             bounds (sequence or Bounds): Bounds on variables for scipy optimizers.
             constraints (dict): Constraints definition for scipy optimizers.
             tol (float): Tolerance of termination for scipy optimizers.
@@ -76,33 +78,28 @@
         Return:
             The final expectation value.
             The corresponding best parameters.
             The optimization result object. For scipy methods it returns
             the ``OptimizeResult``, for ``'cma'`` the ``CMAEvolutionStrategy.result``,
             and for ``'sgd'`` the options used during the optimization.
         """
-
-        def _loss(params, circuit, hamiltonian):
-            circuit.set_parameters(params)
-            result = hamiltonian.backend.execute_circuit(circuit)
-            final_state = result.state()
-            return hamiltonian.expectation(final_state)
-
+        if loss_func is None:
+            loss_func = vqe_loss
         if compile:
-            loss = self.hamiltonian.backend.compile(_loss)
+            loss = self.hamiltonian.backend.compile(loss_func)
         else:
-            loss = _loss
+            loss = loss_func
 
         if method == "cma":
             # TODO: check if we can use this shortcut
             # dtype = getattr(self.hamiltonian.backend.np, self.hamiltonian.backend._dtypes.get('DTYPE'))
             dtype = self.hamiltonian.backend.np.float64
-            loss = lambda p, c, h: dtype(_loss(p, c, h))
+            loss = lambda p, c, h: dtype(loss_func(p, c, h))
         elif method != "sgd":
-            loss = lambda p, c, h: self.hamiltonian.backend.to_numpy(_loss(p, c, h))
+            loss = lambda p, c, h: self.hamiltonian.backend.to_numpy(loss_func(p, c, h))
 
         result, parameters, extra = self.optimizers.optimize(
             loss,
             initial_state,
             args=(self.circuit, self.hamiltonian),
             method=method,
             jac=jac,
@@ -632,26 +629,24 @@
             options (dict): a dictionary with options for the different optimizers.
 
         Return:
             The final energy (expectation value of the ``hamiltonian``).
             The corresponding best parameters.
             extra: variable with historical data for the energy and callbacks.
         """
-        import numpy as np
-
         parameters = np.array([delta_t, 0])
 
         def _loss(params, falqon, hamiltonian):
             falqon.set_parameters(params)
             state = falqon(initial_state)
             return hamiltonian.expectation(state)
 
         energy = [np.inf]
         callback_result = []
-        for it in range(1, max_layers + 1):
+        for _ in range(1, max_layers + 1):
             beta = self.hamiltonian.backend.to_numpy(
                 _loss(parameters, self, self.evol_hamiltonian)
             )
 
             if tol is not None:
                 energy.append(
                     self.hamiltonian.backend.to_numpy(
```

### Comparing `qibo-0.2.7/src/qibo/noise.py` & `qibo-0.2.8/src/qibo/noise.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/noise_model.py` & `qibo-0.2.8/src/qibo/noise_model.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/optimizers.py` & `qibo-0.2.8/src/qibo/optimizers.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/parallel.py` & `qibo-0.2.8/src/qibo/parallel.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/parameter.py` & `qibo-0.2.8/src/qibo/parameter.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/quantum_info/_clifford_utils.py` & `qibo-0.2.8/src/qibo/quantum_info/_clifford_utils.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/quantum_info/basis.py` & `qibo-0.2.8/src/qibo/quantum_info/basis.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/quantum_info/clifford.py` & `qibo-0.2.8/src/qibo/quantum_info/clifford.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/quantum_info/entanglement.py` & `qibo-0.2.8/src/qibo/quantum_info/entanglement.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/quantum_info/entropies.py` & `qibo-0.2.8/src/qibo/quantum_info/entropies.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/quantum_info/metrics.py` & `qibo-0.2.8/src/qibo/quantum_info/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-"""Submodule with distances, metrics, and measures for quantum states and channels."""
+"""Distances, metrics, and measures for quantum states and channels."""
 
 from typing import Optional, Union
 
 import numpy as np
 from scipy import sparse
 
 from qibo.backends import _check_backend
 from qibo.config import PRECISION_TOL, raise_error
 
 
 def purity(state):
-    """Purity of a quantum state :math:`\\rho`, which is given by
+    """Purity of a quantum state :math:`\\rho`.
+
+    This is given by
 
     .. math::
         \\text{purity}(\\rho) = \\text{tr}(\\rho^{2}) \\, .
 
     Args:
         state (ndarray): statevector or density matrix.
     Returns:
@@ -40,29 +42,31 @@
     # a 0-dim ndarray
     pur = float(pur)
 
     return pur
 
 
 def impurity(state):
-    """Impurity of quantum state :math:`\\rho`, which is given by
-    :math:`1 - \\text{purity}(\\rho)`, where :math:`\\text{purity}`
+    """Impurity of quantum state :math:`\\rho`.
+
+    This is given by :math:`1 - \\text{purity}(\\rho)`, where :math:`\\text{purity}`
     is defined in :func:`qibo.quantum_info.purity`.
 
     Args:
         state (ndarray): statevector or density matrix.
 
     Returns:
         float: impurity of ``state`` :math:`\\rho`.
     """
     return 1 - purity(state)
 
 
 def trace_distance(state, target, check_hermitian: bool = False, backend=None):
-    """Trace distance between two quantum states, :math:`\\rho` and :math:`\\sigma`:
+    """Trace distance between two quantum states, :math:`\\rho` and
+    :math:`\\sigma`:
 
     .. math::
         T(\\rho, \\sigma) = \\frac{1}{2} \\, \\|\\rho - \\sigma\\|_{1} = \\frac{1}{2} \\,
             \\text{tr}\\left[ \\sqrt{(\\rho - \\sigma)^{\\dagger}(\\rho - \\sigma)}
             \\right] \\, ,
 
     where :math:`\\|\\cdot\\|_{1}` is the Schatten 1-norm.
@@ -174,16 +178,16 @@
     distance = np.real(np.trace((state - target) ** 2))
     distance = float(distance)
 
     return distance
 
 
 def fidelity(state, target, check_hermitian: bool = False, backend=None):
-    """Fidelity :math:`F(\\rho, \\sigma)` between ``state`` :math:`\\rho`
-    and ``target`` state :math:`\\sigma`. In general,
+    """Fidelity :math:`F(\\rho, \\sigma)` between ``state`` :math:`\\rho` and
+    ``target`` state :math:`\\sigma`. In general,
 
     .. math::
         F(\\rho, \\sigma) = \\text{tr}^{2}\\left( \\sqrt{\\sqrt{\\sigma} \\,
         \\rho^{\\dagger} \\, \\sqrt{\\sigma}} \\right) \\, .
 
     However, when at least one of the states is pure, then
 
@@ -279,16 +283,16 @@
 
     fid = float(fid)
 
     return fid
 
 
 def infidelity(state, target, check_hermitian: bool = False, backend=None):
-    """Infidelity between ``state`` :math:`\\rho` and ``target`` state :math:`\\sigma`,
-    which is given by
+    """Infidelity between ``state`` :math:`\\rho` and ``target`` state
+    :math:`\\sigma`, which is given by
 
     .. math::
         1 - F(\\rho, \\, \\sigma) \\, ,
 
     where :math:`F(\\rho, \\, \\sigma)` is the :func:`qibo.quantum_info.fidelity`
     between ``state`` and ``target``.
 
@@ -304,16 +308,16 @@
     Returns:
         float: Infidelity between ``state`` :math:`\\rho` and ``target`` :math:`\\sigma`.
     """
     return 1 - fidelity(state, target, check_hermitian=check_hermitian, backend=backend)
 
 
 def bures_angle(state, target, check_hermitian: bool = False, backend=None):
-    """Calculates the Bures angle :math:`D_{A}` between a ``state`` :math:`\\rho`
-    and a ``target`` state :math:`\\sigma`. This is given by
+    """Calculates the Bures angle :math:`D_{A}` between a ``state``
+    :math:`\\rho` and a ``target`` state :math:`\\sigma`. This is given by
 
     .. math::
         D_{A}(\\rho, \\, \\sigma) = \\text{arccos}\\left(\\sqrt{F(\\rho, \\, \\sigma)}\\right) \\, ,
 
     where :math:`F(\\rho, \\sigma)` is the :func:`qibo.quantum_info.fidelity`
     between `state` and `target`.
 
@@ -333,16 +337,16 @@
         np.sqrt(fidelity(state, target, check_hermitian, backend=backend))
     )
 
     return angle
 
 
 def bures_distance(state, target, check_hermitian: bool = False, backend=None):
-    """Calculates the Bures distance :math:`D_{B}` between a ``state`` :math:`\\rho`
-    and a ``target`` state :math:`\\sigma`. This is given by
+    """Calculates the Bures distance :math:`D_{B}` between a ``state``
+    :math:`\\rho` and a ``target`` state :math:`\\sigma`. This is given by
 
     .. math::
         D_{B}(\\rho, \\, \\sigma) = \\sqrt{2 \\, \\left(1 - \\sqrt{F(\\rho, \\, \\sigma)}\\right)}
 
     where :math:`F(\\rho, \\sigma)` is the :func:`qibo.quantum_info.fidelity`
     between `state` and `target`.
 
@@ -362,16 +366,16 @@
         2 * (1 - np.sqrt(fidelity(state, target, check_hermitian, backend=backend)))
     )
 
     return distance
 
 
 def process_fidelity(channel, target=None, check_unitary: bool = False, backend=None):
-    """Process fidelity between a quantum ``channel`` :math:`\\mathcal{E}` and a
-    ``target`` unitary channel :math:`U`. The process fidelity is defined as
+    """Process fidelity between a quantum ``channel`` :math:`\\mathcal{E}` and
+    a ``target`` unitary channel :math:`U`. The process fidelity is defined as
 
     .. math::
         F_{\\text{pro}}(\\mathcal{E}, \\mathcal{U}) = \\frac{1}{d^{2}} \\,
             \\text{tr}(\\mathcal{E}^{\\dagger} \\, \\mathcal{U})
 
     Args:
         channel: quantum channel :math:`\\mathcal{E}`.
@@ -425,16 +429,16 @@
     process_fid = np.real(np.trace(process_fid)) / dim**2
     process_fid = float(process_fid)
 
     return process_fid
 
 
 def process_infidelity(channel, target=None, check_unitary: bool = False, backend=None):
-    """Process infidelity between quantum channel :math:`\\mathcal{E}`
-    and a ``target`` unitary channel :math:`U`. The process infidelity is defined as
+    """Process infidelity between quantum channel :math:`\\mathcal{E}` and a
+    ``target`` unitary channel :math:`U`. The process infidelity is defined as
 
     .. math::
         1 - F_{\\text{pro}}(\\mathcal{E}, \\mathcal{U}) \\, ,
 
     where :math:`F_{\\text{pro}}` is the :func:`qibo.quantum_info.process_fidelity`.
 
     Args:
@@ -457,16 +461,16 @@
     )
 
 
 def average_gate_fidelity(
     channel, target=None, check_unitary: bool = False, backend=None
 ):
     """Average gate fidelity between a quantum ``channel`` :math:`\\mathcal{E}`
-    and a ``target`` unitary channel :math:`U`. The average gate fidelity
-    is defined as
+    and a ``target`` unitary channel :math:`U`. The average gate fidelity is
+    defined as
 
     .. math::
         F_{\\text{avg}}(\\mathcal{E}, \\mathcal{U}) = \\frac{d \\,
             F_{pro}(\\mathcal{E}, \\mathcal{U}) + 1}{d + 1}
 
     where :math:`d` is the dimension of the channels and
     :math:`F_{pro}(\\mathcal{E}, \\mathcal{U})` is the
@@ -496,16 +500,16 @@
     )
     process_fid = (dim * process_fid + 1) / (dim + 1)
 
     return process_fid
 
 
 def gate_error(channel, target=None, check_unitary: bool = False, backend=None):
-    """Gate error between a quantum ``channel`` :math:`\\mathcal{E}`
-    and a ``target`` unitary channel :math:`U`, which is defined as
+    """Gate error between a quantum ``channel`` :math:`\\mathcal{E}` and a
+    ``target`` unitary channel :math:`U`, which is defined as
 
     .. math::
         E(\\mathcal{E}, \\mathcal{U}) = 1 - F_{\\text{avg}}(\\mathcal{E}, \\mathcal{U}) \\, ,
 
     where :math:`F_{\\text{avg}}(\\mathcal{E}, \\mathcal{U})` is the
     :func:`qibo.quantum_info.average_gate_fidelity`.
 
@@ -526,61 +530,58 @@
     error = 1 - average_gate_fidelity(
         channel, target, check_unitary=check_unitary, backend=backend
     )
 
     return error
 
 
-def diamond_norm(channel, target=None, backend=None, **kwargs):
+def diamond_norm(channel, target=None, backend=None, **kwargs):  # pragma: no cover
     """Calculates the diamond norm :math:`\\|\\mathcal{E}\\|_{\\diamond}` of
     ``channel`` :math:`\\mathcal{E}`, which is given by
 
     .. math::
         \\|\\mathcal{E}\\|_{\\diamond} = \\max_{\\rho} \\, \\| \\left(\\mathcal{E} \\otimes I_{d^{2}}\\right)(\\rho) \\|_{1} \\, ,
 
     where :math:`I_{d^{2}}` is the :math:`d^{2} \\times d^{2}` Identity operator,
     :math:`d = 2^{n}`, :math:`n` is the number of qubits,
     and :math:`\\|\\cdot\\|_{1}` denotes the trace norm.
 
     If a ``target`` channel :math:`\\Lambda` is specified,
     then it calculates :math:`\\| \\mathcal{E} - \\Lambda\\|_{\\diamond}`.
 
-    Example:
-
-        .. testcode::
+    Example::
 
-            from qibo.quantum_info import diamond_norm, random_unitary, to_choi
+        from qibo.quantum_info import diamond_norm, random_unitary, to_choi
 
-            nqubits = 1
-            dim = 2**nqubits
+        nqubits = 1
+        dim = 2**nqubits
 
-            unitary = random_unitary(dim)
-            unitary = to_choi(unitary, order="row")
+        unitary = random_unitary(dim)
+        unitary = to_choi(unitary, order="row")
 
-            unitary_2 = random_unitary(dim)
-            unitary_2 = to_choi(unitary_2, order="row")
+        unitary_2 = random_unitary(dim)
+        unitary_2 = to_choi(unitary_2, order="row")
 
-            dnorm = diamond_norm(unitary, unitary_2)
+        dnorm = diamond_norm(unitary, unitary_2)
 
     Args:
         channel (ndarray): row-vectorized Choi representation of a quantum channel.
         target (ndarray, optional): row-vectorized Choi representation of a target
             quantum channel. Defaults to ``None``.
         kwargs: optional arguments to pass to CVXPY solver. For more information,
             please visit `CVXPY's API documentation
             <https://www.cvxpy.org/api_reference/cvxpy.problems.html#problem>`_.
 
     Returns:
         float: diamond norm of either ``channel`` or ``channel - target``.
 
     .. note::
         This function requires the optional CVXPY package to be installed.
-
     """
-    import cvxpy  # pylint: disable=C0415
+    import cvxpy
 
     if target is not None:
         if channel.shape != target.shape:
             raise_error(
                 TypeError,
                 f"Channels must have the same dims, but {channel.shape} != {target.shape}",
             )
@@ -663,16 +664,16 @@
 def expressibility(
     circuit,
     power_t: int,
     samples: int,
     order: Optional[Union[int, float, str]] = 2,
     backend=None,
 ):
-    """Returns the expressibility :math:`\\|A\\|` of a parametrized
-    circuit, where
+    """Returns the expressibility :math:`\\|A\\|` of a parametrized circuit,
+    where
 
     .. math::
         A = \\int_{\\text{Haar}} d\\psi \\, \\left(|\\psi\\rangle\\right.\\left.
             \\langle\\psi|\\right)^{\\otimes t} - \\int_{\\Theta} d\\psi \\,
             \\left(|\\psi_{\\theta}\\rangle\\right.\\left.
             \\langle\\psi_{\\theta}|\\right)^{\\otimes t}
 
@@ -719,15 +720,16 @@
 
 def frame_potential(
     circuit,
     power_t: int,
     samples: int = None,
     backend=None,
 ):
-    """Returns the frame potential of a parametrized circuit under uniform sampling of the parameters.
+    """Returns the frame potential of a parametrized circuit under uniform
+    sampling of the parameters.
 
     For :math:`n` qubits and moment :math:`t`, the frame potential
     :math:`\\mathcal{F}_{\\mathcal{U}}^{(t)}` if given by [1]
 
     .. math::
         \\mathcal{F}_{\\mathcal{U}}^{(t)} = \\int_{U,V \\in \\mathcal{U}} \\,
             \\text{d}U \\, \\text{d}V \\, \\bigl| \\, \\text{tr}(U^{\\dagger} \\, V)
@@ -752,15 +754,14 @@
 
     Returns:
         float: Frame potential of the parametrized circuit.
 
     References:
         1. M. Liu *et al.*, *Estimating the randomness of quantum circuit ensembles up to 50 qubits*.
         `arXiv:2205.09900 [quant-ph] <https://arxiv.org/abs/2205.09900>`_.
-
     """
     if not isinstance(power_t, int):
         raise_error(
             TypeError, f"power_t must be type int, but it is type {type(power_t)}."
         )
 
     if not isinstance(samples, int):
@@ -790,31 +791,30 @@
                 np.trace(np.transpose(np.conj(unitary_1)) @ unitary_2)
             ) ** (2 * power_t)
 
     return potential / samples**2
 
 
 def _check_hermitian_or_not_gpu(matrix, backend=None):
-    """Checks if a given matrix is Hermitian and whether
-    the backend is neither :class:`qibojit.backends.CupyBackend`
-    nor :class:`qibojit.backends.CuQuantumBackend`.
+    """Checks if a given matrix is Hermitian and whether the backend is neither
+    :class:`qibojit.backends.CupyBackend` nor
+    :class:`qibojit.backends.CuQuantumBackend`.
 
     Args:
         matrix: input array.
         backend (:class:`qibo.backends.abstract.Backend`, optional): backend to be used
             in the execution. If ``None``, it uses :class:`qibo.backends.GlobalBackend`.
             Defaults to ``None``.
 
     Returns:
         bool: whether the matrix is Hermitian.
 
     Raises:
         NotImplementedError: If `matrix` is not Hermitian and
         `backend` is not :class:`qibojit.backends.CupyBackend`
-
     """
     backend = _check_backend(backend)
 
     norm = backend.calculate_norm_density_matrix(
         np.transpose(np.conj(matrix)) - matrix, order=2
     )
```

### Comparing `qibo-0.2.7/src/qibo/quantum_info/quantum_networks.py` & `qibo-0.2.8/src/qibo/quantum_info/quantum_networks.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/quantum_info/random_ensembles.py` & `qibo-0.2.8/src/qibo/quantum_info/random_ensembles.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import warnings
 from functools import cache
 from typing import Optional, Union
 
 import numpy as np
 from scipy.stats import rv_continuous
 
-from qibo import Circuit, gates
-from qibo.backends import NumpyBackend, _check_backend
+from qibo import Circuit, gates, matrices
+from qibo.backends import NumpyBackend, _check_backend_and_local_state
 from qibo.config import MAX_ITERATIONS, PRECISION_TOL, raise_error
 from qibo.quantum_info.basis import comp_basis_to_pauli
 from qibo.quantum_info.superoperator_transformations import (
     choi_to_chi,
     choi_to_kraus,
     choi_to_liouville,
     choi_to_pauli,
@@ -63,15 +63,15 @@
     if not isinstance(ngates, int):
         raise_error(
             TypeError, f"ngates must be type int, but it is type {type(ngates)}."
         )
     elif ngates <= 0:
         raise_error(ValueError, f"ngates must be non-negative, but it is {ngates}.")
 
-    backend, local_state = _set_backend_and_local_state(seed, backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     sampler = _probability_distribution_sin(a=0, b=np.pi, seed=local_state)
     phases = local_state.random((ngates, 3))
     phases[:, 0] = sampler.rvs(size=len(phases[:, 0]))
     phases[:, 1] = phases[:, 1] * 2 * np.pi
     phases[:, 2] = phases[:, 2] * 2 * np.pi
 
@@ -129,15 +129,15 @@
             )
         elif rank <= 0:
             raise_error(ValueError, f"rank ({rank}) must be an int between 1 and dims.")
 
     if stddev is not None and stddev <= 0.0:
         raise_error(ValueError, "stddev must be a positive float.")
 
-    backend, local_state = _set_backend_and_local_state(seed, backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     dims = (dims, rank)
 
     matrix = 1.0j * local_state.normal(loc=mean, scale=stddev, size=dims)
     matrix += local_state.normal(loc=mean, scale=stddev, size=dims)
     matrix = backend.cast(matrix, dtype=matrix.dtype)
 
@@ -175,15 +175,15 @@
 
     if dims <= 0:
         raise_error(ValueError, f"dims ({dims}) must be type int and positive.")
 
     if not isinstance(semidefinite, bool) or not isinstance(normalize, bool):
         raise_error(TypeError, "semidefinite and normalize must be type bool.")
 
-    backend, local_state = _set_backend_and_local_state(seed, backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     matrix = random_gaussian_matrix(dims, dims, seed=local_state, backend=backend)
 
     if semidefinite:
         matrix = np.dot(np.transpose(np.conj(matrix)), matrix)
     else:
         matrix = (matrix + np.transpose(np.conj(matrix))) / 2
@@ -222,15 +222,15 @@
         if not isinstance(measure, str):
             raise_error(
                 TypeError, f"measure must be type str but it is type {type(measure)}."
             )
         if measure != "haar":
             raise_error(ValueError, f"measure {measure} not implemented.")
 
-    backend, local_state = _set_backend_and_local_state(seed, backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     if measure == "haar":
         unitary = random_gaussian_matrix(dims, dims, seed=local_state, backend=backend)
         Q, R = np.linalg.qr(unitary)
         D = np.diag(R)
         D = D / np.abs(D)
         R = np.diag(D)
@@ -338,15 +338,15 @@
             raise_error(ValueError, f"representation {representation} not implemented.")
 
     if measure == "bcsz" and order not in ["row", "column"]:
         raise_error(
             NotImplementedError, f"order {order} not implemented for measure {measure}."
         )
 
-    backend, local_state = _set_backend_and_local_state(seed, backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     if measure == "bcsz":
         super_op = _super_op_from_bcsz_measure(
             dims=dims, rank=rank, order=order, seed=local_state, backend=backend
         )
     else:
         super_op = random_unitary(dims, measure, local_state, backend)
@@ -430,15 +430,15 @@
         and not isinstance(seed, int)
         and not isinstance(seed, np.random.Generator)
     ):
         raise_error(
             TypeError, "seed must be either type int or numpy.random.Generator."
         )
 
-    backend, local_state = _set_backend_and_local_state(seed, backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     state = local_state.standard_normal(dims).astype(complex)
     state += 1.0j * local_state.standard_normal(dims)
     state /= np.linalg.norm(state)
     state = backend.cast(state, dtype=state.dtype)
 
     return state
@@ -535,15 +535,15 @@
     if not isinstance(normalize, bool):
         raise_error(
             TypeError, f"normalize must be type bool, but it is type {type(normalize)}."
         )
     elif normalize is True and basis is None:
         raise_error(ValueError, "normalize cannot be True when basis=None.")
 
-    backend, local_state = _set_backend_and_local_state(seed, backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     if metric == "hilbert-schmidt":
         rank = None
 
     if pure:
         state = random_statevector(dims, seed=local_state, backend=backend)
         state = np.outer(state, np.transpose(np.conj(state)))
@@ -624,15 +624,15 @@
 
     if not isinstance(return_circuit, bool):
         raise_error(
             TypeError,
             f"return_circuit must be type bool, but it is type {type(return_circuit)}.",
         )
 
-    backend, local_state = _set_backend_and_local_state(seed, backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     hadamards, permutations = _sample_from_quantum_mallows_distribution(
         nqubits, local_state=local_state
     )
 
     delta_matrix = np.eye(nqubits, dtype=int)
     delta_matrix_prime = np.copy(delta_matrix)
@@ -805,17 +805,21 @@
 
     if subset is not None and any(isinstance(item, str) is False for item in subset):
         raise_error(
             TypeError,
             "subset argument must be a subset of strings in the set ['I', 'X', 'Y', 'Z'].",
         )
 
-    backend, local_state = _set_backend_and_local_state(seed, backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
-    complete_set = {"I": gates.I, "X": gates.X, "Y": gates.Y, "Z": gates.Z}
+    complete_set = (
+        {"I": gates.I, "X": gates.X, "Y": gates.Y, "Z": gates.Z}
+        if return_circuit
+        else {"I": matrices.I, "X": matrices.X, "Y": matrices.Y, "Z": matrices.Z}
+    )
 
     if subset is None:
         subset = complete_set
     else:
         subset = {key: complete_set[key] for key in subset}
 
     keys = list(subset.keys())
@@ -836,21 +840,17 @@
     if return_circuit:
         gate_grid = Circuit(max_qubits, density_matrix=density_matrix)
         for qubit, row in zip(qubits, indexes):
             for column_item in row:
                 if subset[column_item] != gates.I:
                     gate_grid.add(subset[column_item](qubit))
     else:
-        gate_grid = np.array(
-            [
-                [subset[column_item](qubit).matrix(backend) for column_item in row]
-                for qubit, row in zip(qubits, indexes)
-            ]
+        gate_grid = backend.cast(
+            [[subset[column_item] for column_item in row] for row in indexes]
         )
-        gate_grid = backend.cast(gate_grid, dtype=gate_grid.dtype)
 
     return gate_grid
 
 
 def random_pauli_hamiltonian(
     nqubits: int,
     max_eigenvalue: Optional[Union[int, float]] = None,
@@ -908,15 +908,15 @@
         )
     elif normalize is True and max_eigenvalue <= 1.0:
         raise_error(
             ValueError,
             "when normalize=True, gap is = 1, thus max_eigenvalue must be > 1.",
         )
 
-    backend, local_state = _set_backend_and_local_state(seed, backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     d = 2**nqubits
 
     hamiltonian = random_hermitian(d, normalize=True, seed=local_state, backend=backend)
 
     eigenvalues, eigenvectors = np.linalg.eigh(hamiltonian)
 
@@ -1012,15 +1012,15 @@
             raise_error(
                 TypeError,
                 f"max_iterations must be type int, but it is type {type(precision_tol)}.",
             )
         if max_iterations <= 0.0:
             raise_error(ValueError, "max_iterations must be a positive int.")
 
-    backend, local_state = _set_backend_and_local_state(seed, backend)
+    backend, local_state = _check_backend_and_local_state(seed, backend)
 
     if precision_tol is None:
         precision_tol = PRECISION_TOL
     if max_iterations is None:
         max_iterations = MAX_ITERATIONS
 
     matrix = local_state.random(size=(dims, dims))
@@ -1215,33 +1215,7 @@
         operator = backend.np.kron(
             operator, backend.identity_density_matrix(nqubits, normalize=False)
         )
 
     super_op = operator @ super_op @ operator
 
     return super_op
-
-
-def _set_backend_and_local_state(seed, backend):
-    if (
-        seed is not None
-        and not isinstance(seed, int)
-        and not isinstance(seed, np.random.Generator)
-    ):
-        raise_error(
-            TypeError, "seed must be either type int or numpy.random.Generator."
-        )
-
-    backend = _check_backend(backend)
-
-    if seed is None or isinstance(seed, int):
-        if backend.__class__.__name__ in [
-            "CupyBackend",
-            "CuQuantumBackend",
-        ]:  # pragma: no cover
-            local_state = backend.np.random.default_rng(seed)
-        else:
-            local_state = np.random.default_rng(seed)
-    else:
-        local_state = seed
-
-    return backend, local_state
```

### Comparing `qibo-0.2.7/src/qibo/quantum_info/superoperator_transformations.py` & `qibo-0.2.8/src/qibo/quantum_info/superoperator_transformations.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/quantum_info/utils.py` & `qibo-0.2.8/src/qibo/quantum_info/utils.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/result.py` & `qibo-0.2.8/src/qibo/result.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/solvers.py` & `qibo-0.2.8/src/qibo/solvers.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/symbols.py` & `qibo-0.2.8/src/qibo/symbols.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/transpiler/_exceptions.py` & `qibo-0.2.8/src/qibo/transpiler/_exceptions.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/transpiler/abstract.py` & `qibo-0.2.8/src/qibo/transpiler/abstract.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/transpiler/blocks.py` & `qibo-0.2.8/src/qibo/transpiler/blocks.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/transpiler/decompositions.py` & `qibo-0.2.8/src/qibo/transpiler/decompositions.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/transpiler/optimizer.py` & `qibo-0.2.8/src/qibo/transpiler/optimizer.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/transpiler/pipeline.py` & `qibo-0.2.8/src/qibo/transpiler/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -176,28 +176,33 @@
         connectivity (:class:`networkx.Graph`, optional): physical qubits connectivity.
             If ``None``, :class:`` is used.
             Defaults to ``None``.
         native_gates (:class:`qibo.transpiler.unroller.NativeGates`, optional): native gates.
             Defaults to :math:`qibo.transpiler.unroller.NativeGates.default`.
         on_qubits (list, optional): list of physical qubits to be used.
             If "None" all qubits are used. Defaults to ``None``.
+        int_qubit_name (bool, optional): if `True` the `final_layout` keys are
+            cast to integers.
     """
 
     def __init__(
         self,
         passes: list = None,
         connectivity: nx.Graph = None,
         native_gates: NativeGates = NativeGates.default(),
         on_qubits: list = None,
+        int_qubit_names: bool = False,
     ):
         if on_qubits is not None:
             connectivity = restrict_connectivity_qubits(connectivity, on_qubits)
         self.connectivity = connectivity
         self.native_gates = native_gates
         self.passes = self.default() if passes is None else passes
+        self.initial_layout = None
+        self.int_qubit_names = int_qubit_names
 
     def default(self):
         """Return the default transpiler pipeline for the required hardware connectivity."""
         if not isinstance(self.connectivity, nx.Graph):
             raise_error(
                 TranspilerPipelineError,
                 "Define the hardware chip connectivity to use default transpiler",
@@ -211,16 +216,20 @@
         default_passes.append(StarConnectivityRouter())
         # default unroller pass
         default_passes.append(Unroller(native_gates=self.native_gates))
 
         return default_passes
 
     def __call__(self, circuit):
-        self.initial_layout = None
-        final_layout = None
+        """
+        This function returns the compiled circuits and the dictionary mapping
+        physical (keys) to logical (values) qubit. If `int_qubit_name` is `True`
+        each key `i` correspond to the `i-th` qubit in the graph.
+        """
+        final_layout = self.initial_layout
         for transpiler_pass in self.passes:
             if isinstance(transpiler_pass, Optimizer):
                 transpiler_pass.connectivity = self.connectivity
                 circuit = transpiler_pass(circuit)
             elif isinstance(transpiler_pass, Placer):
                 transpiler_pass.connectivity = self.connectivity
                 if self.initial_layout == None:
@@ -243,15 +252,17 @@
             elif isinstance(transpiler_pass, Unroller):
                 circuit = transpiler_pass(circuit)
             else:
                 raise_error(
                     TranspilerPipelineError,
                     f"Unrecognised transpiler pass: {transpiler_pass}",
                 )
-
+        # TODO: use directly integers keys
+        if self.int_qubit_names:
+            final_layout = {int(key[1:]): value for key, value in final_layout.items()}
         return circuit, final_layout
 
     def is_satisfied(self, circuit: Circuit):
         """Returns ``True`` if the circuit respects the hardware connectivity and native gates, ``False`` otherwise.
 
         Args:
             circuit (:class:`qibo.models.circuit.Circuit`): circuit to be checked.
```

### Comparing `qibo-0.2.7/src/qibo/transpiler/placer.py` & `qibo-0.2.8/src/qibo/transpiler/placer.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/transpiler/router.py` & `qibo-0.2.8/src/qibo/transpiler/router.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/transpiler/unitary_decompositions.py` & `qibo-0.2.8/src/qibo/transpiler/unitary_decompositions.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/src/qibo/transpiler/unroller.py` & `qibo-0.2.8/src/qibo/transpiler/unroller.py`

 * *Files identical despite different names*

### Comparing `qibo-0.2.7/PKG-INFO` & `qibo-0.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: qibo
-Version: 0.2.7
+Version: 0.2.8
 Summary: A framework for quantum computing with hardware acceleration.
 Home-page: https://qibo.science/
 License: Apache-2.0
 Author: The Qibo team
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: qinfo
 Provides-Extra: tensorflow
 Provides-Extra: torch
 Requires-Dist: cma (>=3.3.0,<4.0.0)
-Requires-Dist: cvxpy (>=1.4.2,<2.0.0) ; extra == "qinfo"
 Requires-Dist: hyperopt (>=0.2.7,<0.3.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: openqasm3[parser] (>=0.5.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Requires-Dist: setuptools (>=69.1.1,<70.0.0)
 Requires-Dist: sympy (>=1.11.1,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: tensorflow (>=2.14.1,<2.16) ; (sys_platform == "linux" or sys_platform == "darwin") and (extra == "tensorflow")
+Requires-Dist: tensorflow (>=2.16.1,<3.0.0) ; (sys_platform == "linux" or sys_platform == "darwin") and (extra == "tensorflow")
 Requires-Dist: torch (>=2.1.1,<3.0.0) ; extra == "torch"
 Project-URL: Documentation, https://qibo.science/docs/qibo/stable
 Project-URL: Repository, https://github.com/qiboteam/qibo/
 Description-Content-Type: text/markdown
 
 ![Logo](https://github.com/qiboteam/qibo/blob/master/doc/source/_static/qibo_logo_dark.svg)
```

