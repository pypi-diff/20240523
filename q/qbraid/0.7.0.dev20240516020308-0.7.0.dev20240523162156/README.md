# Comparing `tmp/qbraid-0.7.0.dev20240516020308.tar.gz` & `tmp/qbraid-0.7.0.dev20240523162156.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-0.7.0.dev20240516020308.tar", last modified: Thu May 16 02:03:11 2024, max compression
+gzip compressed data, was "qbraid-0.7.0.dev20240523162156.tar", last modified: Thu May 23 16:21:59 2024, max compression
```

## Comparing `qbraid-0.7.0.dev20240516020308.tar` & `qbraid-0.7.0.dev20240523162156.tar`

### file list

```diff
@@ -1,221 +1,222 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.527386 qbraid-0.7.0.dev20240516020308/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15828 2024-05-16 02:03:11.527386 qbraid-0.7.0.dev20240516020308/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13159 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.495386 qbraid-0.7.0.dev20240516020308/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.495386 qbraid-0.7.0.dev20240516020308/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.495386 qbraid-0.7.0.dev20240516020308/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/cards/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.499386 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/
--rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/braket.png
--rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/cirq.png
--rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/pennylane.png
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/pyquil.png
--rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/qasm.png
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/qir.png
--rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/qiskit.png
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/quantinuum.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.499386 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/batch_counts.png
--rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/conversion_graph.png
--rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/get_devices.png
--rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/hub_spokes.png
--rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/lab_jobs.png
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/plot_counts.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.499386 qbraid-0.7.0.dev20240516020308/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.runtime.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.transforms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/api/qbraid.visualization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.503386 qbraid-0.7.0.dev20240516020308/docs/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/programs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/providers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/docs/sdk/transpiler.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.503386 qbraid-0.7.0.dev20240516020308/qbraid/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/_about.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 02:03:08.000000 qbraid-0.7.0.dev20240516020308/qbraid/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.503386 qbraid-0.7.0.dev20240516020308/qbraid/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/circuit_equality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.507386 qbraid-0.7.0.dev20240516020308/qbraid/interface/random/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/random/cirq_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/random/qasm3_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/random/qiskit_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/interface/random/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.507386 qbraid-0.7.0.dev20240516020308/qbraid/programs/
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/alias_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.507386 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/pennylane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/pyquil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/pytket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/qasm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15083 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/qiskit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/programs/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.511386 qbraid-0.7.0.dev20240516020308/qbraid/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/_display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.511386 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.511386 qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.511386 qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.511386 qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/runtime/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/braket/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/cirq/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/cirq/passes.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/pytket/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/pytket/ionq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/qasm_qelib1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm3/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm3/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transforms/qiskit/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.515386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/braket_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/braket_to_cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/braket_to_qasm3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/braket_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    21821 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_quil_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_to_pyquil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_to_qasm2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/openqasm3/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/openqasm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/openqasm3/openqasm3_to_qasm3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pennylane/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pennylane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pennylane/pennylane_to_qasm2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/pyquil_to_cirq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/pytket_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/pytket_to_qasm2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.519386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/cirq_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    23075 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/cirq_qasm_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/qasm2_to_cirq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/qasm2_to_pytket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/qasm2_to_qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/qasm2_to_qiskit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.523386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_to_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_to_openqasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_to_qiskit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.523386 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/qiskit_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/qiskit_to_qasm2.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/qiskit_to_qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/transpiler/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.523386 qbraid-0.7.0.dev20240516020308/qbraid/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/visualization/draw_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/visualization/draw_qasm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/visualization/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/visualization/plot_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/qbraid/visualization/plot_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.523386 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15828 2024-05-16 02:03:11.000000 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-05-16 02:03:11.000000 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:03:11.000000 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-16 02:03:11.000000 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-16 02:03:11.000000 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 02:03:11.000000 qbraid-0.7.0.dev20240516020308/qbraid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 02:03:11.527386 qbraid-0.7.0.dev20240516020308/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:03:11.523386 qbraid-0.7.0.dev20240516020308/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/tools/set_provider_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-16 02:03:04.000000 qbraid-0.7.0.dev20240516020308/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.149571 qbraid-0.7.0.dev20240523162156/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15844 2024-05-23 16:21:59.149571 qbraid-0.7.0.dev20240523162156/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13174 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.117571 qbraid-0.7.0.dev20240523162156/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.117571 qbraid-0.7.0.dev20240523162156/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.117571 qbraid-0.7.0.dev20240523162156/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/cards/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.121571 qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/braket.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53519 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/cirq.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/pennylane.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/pyquil.png
+-rw-r--r--   0 runner    (1001) docker     (127)   125852 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/qasm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/qir.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/qiskit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/quantinuum.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.125571 qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/batch_counts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/conversion_graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)   447304 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/get_devices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   180765 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/hub_spokes.png
+-rw-r--r--   0 runner    (1001) docker     (127)   707295 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/lab_jobs.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/plot_counts.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.125571 qbraid-0.7.0.dev20240523162156/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/api/qbraid.interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/api/qbraid.programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/api/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/api/qbraid.runtime.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/api/qbraid.transforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/api/qbraid.transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/api/qbraid.visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.125571 qbraid-0.7.0.dev20240523162156/docs/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/sdk/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/sdk/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/sdk/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/sdk/programs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/sdk/providers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/sdk/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/docs/sdk/transpiler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.125571 qbraid-0.7.0.dev20240523162156/qbraid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 16:21:56.000000 qbraid-0.7.0.dev20240523162156/qbraid/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.129571 qbraid-0.7.0.dev20240523162156/qbraid/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/interface/circuit_equality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.129571 qbraid-0.7.0.dev20240523162156/qbraid/interface/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/interface/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/interface/random/cirq_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/interface/random/qasm3_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/interface/random/qiskit_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/interface/random/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.129571 qbraid-0.7.0.dev20240523162156/qbraid/programs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/alias_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.133571 qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/pennylane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/pytket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/qasm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15083 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/programs/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.133571 qbraid-0.7.0.dev20240523162156/qbraid/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/_display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.133571 qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.133571 qbraid-0.7.0.dev20240523162156/qbraid/runtime/ionq/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/ionq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/ionq/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/ionq/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/ionq/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/ionq/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.137571 qbraid-0.7.0.dev20240523162156/qbraid/runtime/native/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/native/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/native/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/native/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/native/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.137571 qbraid-0.7.0.dev20240523162156/qbraid/runtime/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/qiskit/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/qiskit/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/qiskit/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/runtime/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.137571 qbraid-0.7.0.dev20240523162156/qbraid/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.137571 qbraid-0.7.0.dev20240523162156/qbraid/transforms/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/braket/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.137571 qbraid-0.7.0.dev20240523162156/qbraid/transforms/cirq/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/cirq/passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.137571 qbraid-0.7.0.dev20240523162156/qbraid/transforms/pytket/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/pytket/ionq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.137571 qbraid-0.7.0.dev20240523162156/qbraid/transforms/qasm2/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/qasm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/qasm2/passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/qasm2/qasm_qelib1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.137571 qbraid-0.7.0.dev20240523162156/qbraid/transforms/qasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/qasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/qasm3/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.137571 qbraid-0.7.0.dev20240523162156/qbraid/transforms/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transforms/qiskit/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.141571 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.141571 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.141571 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/braket/braket_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/braket/braket_to_cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/braket/braket_to_qasm3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.141571 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/braket_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/cirq_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21821 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/cirq_quil_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/cirq_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/cirq_to_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/cirq_to_qasm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.141571 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/openqasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/openqasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/openqasm3/openqasm3_to_qasm3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.141571 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pennylane/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pennylane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pennylane/pennylane_to_qasm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.141571 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pyquil/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pyquil/pyquil_to_cirq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.145571 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pytket/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pytket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pytket/pytket_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pytket/pytket_to_qasm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.145571 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/cirq_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23075 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/cirq_qasm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/qasm2_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/qasm2_to_cirq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/qasm2_to_pytket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/qasm2_to_qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/qasm2_to_qiskit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.145571 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm3/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm3/qasm3_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm3/qasm3_to_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm3/qasm3_to_openqasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm3/qasm3_to_qiskit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.145571 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qiskit/qiskit_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qiskit/qiskit_to_qasm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qiskit/qiskit_to_qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/transpiler/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.145571 qbraid-0.7.0.dev20240523162156/qbraid/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/visualization/draw_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/visualization/draw_qasm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/visualization/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/visualization/plot_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/qbraid/visualization/plot_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.149571 qbraid-0.7.0.dev20240523162156/qbraid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15844 2024-05-23 16:21:59.000000 qbraid-0.7.0.dev20240523162156/qbraid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-23 16:21:59.000000 qbraid-0.7.0.dev20240523162156/qbraid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:21:59.000000 qbraid-0.7.0.dev20240523162156/qbraid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-23 16:21:59.000000 qbraid-0.7.0.dev20240523162156/qbraid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-23 16:21:59.000000 qbraid-0.7.0.dev20240523162156/qbraid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 16:21:59.000000 qbraid-0.7.0.dev20240523162156/qbraid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 16:21:59.149571 qbraid-0.7.0.dev20240523162156/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:21:59.149571 qbraid-0.7.0.dev20240523162156/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/tools/set_provider_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-23 16:21:54.000000 qbraid-0.7.0.dev20240523162156/tox.ini
```

### Comparing `qbraid-0.7.0.dev20240516020308/CODE_OF_CONDUCT.md` & `qbraid-0.7.0.dev20240523162156/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/CONTRIBUTING.md` & `qbraid-0.7.0.dev20240523162156/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/LICENSE` & `qbraid-0.7.0.dev20240523162156/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/PKG-INFO` & `qbraid-0.7.0.dev20240523162156/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.7.0.dev20240516020308
+Version: 0.7.0.dev20240523162156
 Summary: Platform-agnostic quantum runtime framework.
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/en/stable/
 Project-URL: Source Code, https://github.com/qBraid/qBraid
@@ -35,15 +35,15 @@
 Requires-Dist: amazon-braket-sdk<1.80.0,>=1.42.1; extra == "braket"
 Requires-Dist: pytket-braket<0.37.0,>=0.30.0; extra == "braket"
 Provides-Extra: qiskit
 Requires-Dist: qiskit<1.1.0,>=0.44.0; extra == "qiskit"
 Requires-Dist: qiskit-ibm-runtime<0.21.0,>=0.18.0; extra == "qiskit"
 Provides-Extra: runtime
 Requires-Dist: qbraid-qir>=0.2.0; extra == "runtime"
-Requires-Dist: qbraid-core>=0.1.6; extra == "runtime"
+Requires-Dist: qbraid-core>=0.1.10; extra == "runtime"
 Provides-Extra: visualization
 Requires-Dist: ipython; extra == "visualization"
 Requires-Dist: matplotlib; extra == "visualization"
 Requires-Dist: pylatexenc; extra == "visualization"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -77,15 +77,15 @@
   <a href="https://pepy.tech/project/qbraid">
     <img src="https://static.pepy.tech/badge/qbraid" alt="Downloads"/>
   </a>
   <a href="https://www.gnu.org/licenses/gpl-3.0.html">
     <img src="https://img.shields.io/github/license/qBraid/qbraid.svg" alt="License"/>
   </a>
   <a href="https://discord.gg/TPBU2sa8Et">
-    <img src="https://img.shields.io/discord/771898982564626445.svg?color=pink" alt="Discord"/>
+    <img src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white" alt="Discord"/>
   </a>
 </p>
 
 The qBraid-SDK is a platform-agnostic quantum runtime framework designed for both quantum software and hardware providers.
 
 This Python-based tool streamlines the full lifecycle management of quantum jobs&mdash;from defining program specifications to job submission, and through to the post-processing and visualization of results. Distinguishing itself through a streamlined and highly-configurable approach to cross-platform integration, the qBraid-SDK *does not assume a fixed target software framework*. Instead, it allows providers to dynamically register any desired run input program type as the target, depending on their specific needs. These program types are interconnected via a graph-based transpiler, where each program type is represented as a node and supported conversions as edges. The breadth, depth, and connectivity of this `ConversionGraph` can be customized by the provider.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qbraid Version: 0.7.0.dev20240516020308 Summary:
+Metadata-Version: 2.1 Name: qbraid Version: 0.7.0.dev20240523162156 Summary:
 Platform-agnostic quantum runtime framework. Author: qBraid Development Team
 Author-email: contact@qbraid.com License: GNU General Public License v3.0
 Project-URL: Homepage, https://www.qbraid.com/ Project-URL: Documentation,
 https://docs.qbraid.com/en/stable/ Project-URL: Source Code, https://
 github.com/qBraid/qBraid Project-URL: Bug Tracker, https://github.com/qBraid/
 qBraid/issues Project-URL: Discord, https://discord.gg/TPBU2sa8Et Project-URL:
 Launch on Lab, https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/
@@ -18,15 +18,15 @@
 text/markdown License-File: LICENSE Requires-Dist: networkx<4.0,>=2.5 Requires-
 Dist: numpy<1.27,>=1.17 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0
 Requires-Dist: ply>=3.6 Provides-Extra: braket Requires-Dist: amazon-braket-
 sdk<1.80.0,>=1.42.1; extra == "braket" Requires-Dist: pytket-
 braket<0.37.0,>=0.30.0; extra == "braket" Provides-Extra: qiskit Requires-Dist:
 qiskit<1.1.0,>=0.44.0; extra == "qiskit" Requires-Dist: qiskit-ibm-
 runtime<0.21.0,>=0.18.0; extra == "qiskit" Provides-Extra: runtime Requires-
-Dist: qbraid-qir>=0.2.0; extra == "runtime" Requires-Dist: qbraid-core>=0.1.6;
+Dist: qbraid-qir>=0.2.0; extra == "runtime" Requires-Dist: qbraid-core>=0.1.10;
 extra == "runtime" Provides-Extra: visualization Requires-Dist: ipython; extra
 == "visualization" Requires-Dist: matplotlib; extra == "visualization"
 Requires-Dist: pylatexenc; extra == "visualization" Provides-Extra: test
 Requires-Dist: pytest; extra == "test" Requires-Dist: pytest-cov; extra ==
 "test" Provides-Extra: lint Requires-Dist: black; extra == "lint" Requires-
 Dist: isort; extra == "lint" Requires-Dist: pylint; extra == "lint" Requires-
 Dist: qbraid-cli; extra == "lint" Provides-Extra: docs Requires-Dist:
```

### Comparing `qbraid-0.7.0.dev20240516020308/README.md` & `qbraid-0.7.0.dev20240523162156/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   <a href="https://pepy.tech/project/qbraid">
     <img src="https://static.pepy.tech/badge/qbraid" alt="Downloads"/>
   </a>
   <a href="https://www.gnu.org/licenses/gpl-3.0.html">
     <img src="https://img.shields.io/github/license/qBraid/qbraid.svg" alt="License"/>
   </a>
   <a href="https://discord.gg/TPBU2sa8Et">
-    <img src="https://img.shields.io/discord/771898982564626445.svg?color=pink" alt="Discord"/>
+    <img src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white" alt="Discord"/>
   </a>
 </p>
 
 The qBraid-SDK is a platform-agnostic quantum runtime framework designed for both quantum software and hardware providers.
 
 This Python-based tool streamlines the full lifecycle management of quantum jobs&mdash;from defining program specifications to job submission, and through to the post-processing and visualization of results. Distinguishing itself through a streamlined and highly-configurable approach to cross-platform integration, the qBraid-SDK *does not assume a fixed target software framework*. Instead, it allows providers to dynamically register any desired run input program type as the target, depending on their specific needs. These program types are interconnected via a graph-based transpiler, where each program type is represented as a node and supported conversions as edges. The breadth, depth, and connectivity of this `ConversionGraph` can be customized by the provider.
```

### Comparing `qbraid-0.7.0.dev20240516020308/SECURITY.md` & `qbraid-0.7.0.dev20240523162156/SECURITY.md`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/cards/jupyter.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/cards/python.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/cards/terminal.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/favicon.ico` & `qbraid-0.7.0.dev20240523162156/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/logo.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/braket.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/braket.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/cirq.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/cirq.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/pennylane.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/pennylane.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/pyquil.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/pyquil.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/qasm.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/qasm.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/qir.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/qir.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/qiskit.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/qiskit.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/pkg-logos/quantinuum.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/pkg-logos/quantinuum.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/batch_counts.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/batch_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/conversion_graph.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/conversion_graph.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/get_devices.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/get_devices.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/hub_spokes.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/hub_spokes.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/lab_jobs.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/lab_jobs.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/_static/sdk-files/plot_counts.png` & `qbraid-0.7.0.dev20240523162156/docs/_static/sdk-files/plot_counts.png`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/conf.py` & `qbraid-0.7.0.dev20240523162156/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/index.rst` & `qbraid-0.7.0.dev20240523162156/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/sdk/devices.rst` & `qbraid-0.7.0.dev20240523162156/docs/sdk/devices.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/sdk/jobs.rst` & `qbraid-0.7.0.dev20240523162156/docs/sdk/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/sdk/overview.rst` & `qbraid-0.7.0.dev20240523162156/docs/sdk/overview.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/sdk/programs.rst` & `qbraid-0.7.0.dev20240523162156/docs/sdk/programs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/sdk/results.rst` & `qbraid-0.7.0.dev20240523162156/docs/sdk/results.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/docs/sdk/transpiler.rst` & `qbraid-0.7.0.dev20240523162156/docs/sdk/transpiler.rst`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/pyproject.toml` & `qbraid-0.7.0.dev20240523162156/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 "Bug Tracker" = "https://github.com/qBraid/qBraid/issues"
 Discord = "https://discord.gg/TPBU2sa8Et"
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid.git"
 
 [project.optional-dependencies]
 braket = ["amazon-braket-sdk>=1.42.1,<1.80.0", "pytket-braket>=0.30.0,<0.37.0"]
 qiskit = ["qiskit>=0.44.0,<1.1.0", "qiskit-ibm-runtime>=0.18.0,<0.21.0"]
-runtime = ["qbraid-qir>=0.2.0", "qbraid-core>=0.1.6"]
+runtime = ["qbraid-qir>=0.2.0", "qbraid-core>=0.1.10"]
 visualization = ["ipython", "matplotlib", "pylatexenc"]
 test = ["pytest", "pytest-cov"]
 lint = ["black", "isort", "pylint", "qbraid-cli"]
 docs = ["sphinx>=7.2.6,<7.4.0", "sphinx-autodoc-typehints>=1.24,<2.2", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.22", "sphinx-copybutton"]
 
 [project.entry-points."qbraid.programs"]
 braket = "qbraid.programs.libs.braket:BraketCircuit"
@@ -84,14 +84,15 @@
 [tool.coverage.run]
 parallel = true
 source = ["qbraid"]
 omit = [
   "**/qbraid/visualization/plot_conversions.py",
   "**/qbraid/visualization/draw_circuit.py.py",
   "**/qbraid/_compat.py",
+  "**/qbraid/transpiler/conversions/qasm2/qasm2_extras.py"
 ]
 
 [tool.coverage.paths]
 source = ["qbraid", ".tox/*/lib/python*/site-packages/qbraid"]
 
 [tool.coverage.report]
 show_missing = true
@@ -110,15 +111,15 @@
 directory = "build/coverage"
 
 [tool.coverage.xml]
 output = "build/coverage/coverage.xml"
 
 [tool.black]
 line-length = 100
-target-version = ['py39', 'py310', 'py311']
+target-version = ['py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
   | \.__pycache__
   | \.tox
   | \.venv
```

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/_about.py` & `qbraid-0.7.0.dev20240523162156/qbraid/_about.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/_compat.py` & `qbraid-0.7.0.dev20240523162156/qbraid/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/_display.py` & `qbraid-0.7.0.dev20240523162156/qbraid/_display.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/_import.py` & `qbraid-0.7.0.dev20240523162156/qbraid/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/exceptions.py` & `qbraid-0.7.0.dev20240523162156/qbraid/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/interface/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/interface/circuit_equality.py` & `qbraid-0.7.0.dev20240523162156/qbraid/interface/circuit_equality.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/interface/random/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/interface/random/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/interface/random/cirq_random.py` & `qbraid-0.7.0.dev20240523162156/qbraid/interface/random/cirq_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/interface/random/qasm3_random.py` & `qbraid-0.7.0.dev20240523162156/qbraid/interface/random/qasm3_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/interface/random/qiskit_random.py` & `qbraid-0.7.0.dev20240523162156/qbraid/interface/random/qiskit_random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/interface/random/random.py` & `qbraid-0.7.0.dev20240523162156/qbraid/interface/random/random.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/_import.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/_import.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/alias_manager.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/alias_manager.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/exceptions.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/braket.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/cirq.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/pennylane.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/pennylane.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/pyquil.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/pyquil.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/pytket.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/pytket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/qasm2.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/qasm2.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/qasm3.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/libs/qiskit.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/libs/qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/loader.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/loader.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/program.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/program.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/registry.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/programs/spec.py` & `qbraid-0.7.0.dev20240523162156/qbraid/programs/spec.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/_display.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/_display.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/device.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/job.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/provider.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/result.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/braket/tracker.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/braket/tracker.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/device.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/enums.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/enums.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/exceptions.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/ionq/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/device.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/ionq/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/job.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/ionq/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/provider.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/ionq/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/ionq/result.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/ionq/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/job.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/native/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/device.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/native/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/job.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/native/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/provider.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/native/provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,32 +106,38 @@
             device_data = self.client.get_device(qbraid_id=device_id)
         except (ValueError, QuantumServiceRequestError) as err:
             raise ResourceNotFoundError(f"Device '{device_id}' not found.") from err
 
         profile = self._build_runtime_profile(device_data)
         return QbraidDevice(profile, client=self.client)
 
+    # pylint: disable-next=too-many-arguments
     def display_jobs(
         self,
         device_id: Optional[str] = None,
+        provider: Optional[str] = None,
         status: Optional[str] = None,
         tags: Optional[dict] = None,
         max_results: int = 10,
     ):
         """Displays a list of quantum jobs submitted by user, tabulated by job ID,
         the date/time it was submitted, and status. You can specify filters to
         narrow the search by supplying a dictionary containing the desired criteria.
 
         Args:
             device_id (optional, str): The qBraid ID of the device used in the job.
+            provider (optional, str): The name of the provider.
             tags (optional, dict): A list of tags associated with the job.
             status (optional, str): The status of the job.
             max_results (optional, int): Maximum number of results to display. Defaults to 10.
         """
-        query = {"provider": "qbraid"}
+        query = {}
+
+        if provider:
+            query["provider"] = provider.lower()
 
         if device_id:
             query["qbraidDeviceId"] = device_id
 
         if status:
             query["status"] = status
```

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/native/result.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/native/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/profile.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/profile.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/provider.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/device.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/qiskit/device.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/job.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/qiskit/job.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/provider.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/qiskit/result.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/qiskit/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/runtime/result.py` & `qbraid-0.7.0.dev20240523162156/qbraid/runtime/result.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/braket/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/braket/transform.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/braket/transform.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/cirq/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/cirq/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/cirq/passes.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/cirq/passes.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/exceptions.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/pytket/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/pytket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/pytket/ionq.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/pytket/ionq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/qasm2/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/passes.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/qasm2/passes.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm2/qasm_qelib1.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/qasm2/qasm_qelib1.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm3/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/qasm3/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/qasm3/compat.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/qasm3/compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/qiskit/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transforms/qiskit/transform.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transforms/qiskit/transform.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/annotations.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/annotations.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/braket_extras.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/braket/braket_extras.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/braket_to_cirq.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/braket/braket_to_cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/braket/braket_to_qasm3.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/braket/braket_to_qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/braket_custom.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/braket_custom.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_extras.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/cirq_extras.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_quil_output.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/cirq_quil_output.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_to_braket.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/cirq_to_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_to_pyquil.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/cirq_to_pyquil.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/cirq/cirq_to_qasm2.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/cirq/cirq_to_qasm2.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/openqasm3/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/openqasm3/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/openqasm3/openqasm3_to_qasm3.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/openqasm3/openqasm3_to_qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pennylane/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pennylane/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pennylane/pennylane_to_qasm2.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pennylane/pennylane_to_qasm2.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pyquil/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pyquil/cirq_quil_input.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pyquil/pyquil_to_cirq.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pyquil/pyquil_to_cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pytket/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/pytket_extras.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pytket/pytket_extras.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/pytket/pytket_to_qasm2.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/pytket/pytket_to_qasm2.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/cirq_custom.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/cirq_custom.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/cirq_qasm_parser.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/cirq_qasm_parser.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/qasm2_to_cirq.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/qasm2_to_cirq.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/qasm2_to_pytket.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/qasm2_to_pytket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/qasm2_to_qasm3.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/qasm2_to_qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm2/qasm2_to_qiskit.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm2/qasm2_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm3/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_extras.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm3/qasm3_extras.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_to_braket.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm3/qasm3_to_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_to_openqasm3.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm3/qasm3_to_openqasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qasm3/qasm3_to_qiskit.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qasm3/qasm3_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/qiskit_extras.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qiskit/qiskit_extras.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/qiskit_to_qasm2.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qiskit/qiskit_to_qasm2.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/conversions/qiskit/qiskit_to_qasm3.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/conversions/qiskit/qiskit_to_qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/converter.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/converter.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/edge.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/edge.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/exceptions.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/graph.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/graph.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/transpiler/scheme.py` & `qbraid-0.7.0.dev20240523162156/qbraid/transpiler/scheme.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/visualization/__init__.py` & `qbraid-0.7.0.dev20240523162156/qbraid/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/visualization/draw_circuit.py` & `qbraid-0.7.0.dev20240523162156/qbraid/visualization/draw_circuit.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/visualization/draw_qasm3.py` & `qbraid-0.7.0.dev20240523162156/qbraid/visualization/draw_qasm3.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/visualization/exceptions.py` & `qbraid-0.7.0.dev20240523162156/qbraid/visualization/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/visualization/plot_conversions.py` & `qbraid-0.7.0.dev20240523162156/qbraid/visualization/plot_conversions.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid/visualization/plot_counts.py` & `qbraid-0.7.0.dev20240523162156/qbraid/visualization/plot_counts.py`

 * *Files identical despite different names*

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid.egg-info/PKG-INFO` & `qbraid-0.7.0.dev20240523162156/qbraid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid
-Version: 0.7.0.dev20240516020308
+Version: 0.7.0.dev20240523162156
 Summary: Platform-agnostic quantum runtime framework.
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/en/stable/
 Project-URL: Source Code, https://github.com/qBraid/qBraid
@@ -35,15 +35,15 @@
 Requires-Dist: amazon-braket-sdk<1.80.0,>=1.42.1; extra == "braket"
 Requires-Dist: pytket-braket<0.37.0,>=0.30.0; extra == "braket"
 Provides-Extra: qiskit
 Requires-Dist: qiskit<1.1.0,>=0.44.0; extra == "qiskit"
 Requires-Dist: qiskit-ibm-runtime<0.21.0,>=0.18.0; extra == "qiskit"
 Provides-Extra: runtime
 Requires-Dist: qbraid-qir>=0.2.0; extra == "runtime"
-Requires-Dist: qbraid-core>=0.1.6; extra == "runtime"
+Requires-Dist: qbraid-core>=0.1.10; extra == "runtime"
 Provides-Extra: visualization
 Requires-Dist: ipython; extra == "visualization"
 Requires-Dist: matplotlib; extra == "visualization"
 Requires-Dist: pylatexenc; extra == "visualization"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
@@ -77,15 +77,15 @@
   <a href="https://pepy.tech/project/qbraid">
     <img src="https://static.pepy.tech/badge/qbraid" alt="Downloads"/>
   </a>
   <a href="https://www.gnu.org/licenses/gpl-3.0.html">
     <img src="https://img.shields.io/github/license/qBraid/qbraid.svg" alt="License"/>
   </a>
   <a href="https://discord.gg/TPBU2sa8Et">
-    <img src="https://img.shields.io/discord/771898982564626445.svg?color=pink" alt="Discord"/>
+    <img src="https://img.shields.io/badge/Discord-%235865F2.svg?logo=discord&logoColor=white" alt="Discord"/>
   </a>
 </p>
 
 The qBraid-SDK is a platform-agnostic quantum runtime framework designed for both quantum software and hardware providers.
 
 This Python-based tool streamlines the full lifecycle management of quantum jobs&mdash;from defining program specifications to job submission, and through to the post-processing and visualization of results. Distinguishing itself through a streamlined and highly-configurable approach to cross-platform integration, the qBraid-SDK *does not assume a fixed target software framework*. Instead, it allows providers to dynamically register any desired run input program type as the target, depending on their specific needs. These program types are interconnected via a graph-based transpiler, where each program type is represented as a node and supported conversions as edges. The breadth, depth, and connectivity of this `ConversionGraph` can be customized by the provider.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qbraid Version: 0.7.0.dev20240516020308 Summary:
+Metadata-Version: 2.1 Name: qbraid Version: 0.7.0.dev20240523162156 Summary:
 Platform-agnostic quantum runtime framework. Author: qBraid Development Team
 Author-email: contact@qbraid.com License: GNU General Public License v3.0
 Project-URL: Homepage, https://www.qbraid.com/ Project-URL: Documentation,
 https://docs.qbraid.com/en/stable/ Project-URL: Source Code, https://
 github.com/qBraid/qBraid Project-URL: Bug Tracker, https://github.com/qBraid/
 qBraid/issues Project-URL: Discord, https://discord.gg/TPBU2sa8Et Project-URL:
 Launch on Lab, https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/
@@ -18,15 +18,15 @@
 text/markdown License-File: LICENSE Requires-Dist: networkx<4.0,>=2.5 Requires-
 Dist: numpy<1.27,>=1.17 Requires-Dist: openqasm3[parser]<0.6.0,>=0.4.0
 Requires-Dist: ply>=3.6 Provides-Extra: braket Requires-Dist: amazon-braket-
 sdk<1.80.0,>=1.42.1; extra == "braket" Requires-Dist: pytket-
 braket<0.37.0,>=0.30.0; extra == "braket" Provides-Extra: qiskit Requires-Dist:
 qiskit<1.1.0,>=0.44.0; extra == "qiskit" Requires-Dist: qiskit-ibm-
 runtime<0.21.0,>=0.18.0; extra == "qiskit" Provides-Extra: runtime Requires-
-Dist: qbraid-qir>=0.2.0; extra == "runtime" Requires-Dist: qbraid-core>=0.1.6;
+Dist: qbraid-qir>=0.2.0; extra == "runtime" Requires-Dist: qbraid-core>=0.1.10;
 extra == "runtime" Provides-Extra: visualization Requires-Dist: ipython; extra
 == "visualization" Requires-Dist: matplotlib; extra == "visualization"
 Requires-Dist: pylatexenc; extra == "visualization" Provides-Extra: test
 Requires-Dist: pytest; extra == "test" Requires-Dist: pytest-cov; extra ==
 "test" Provides-Extra: lint Requires-Dist: black; extra == "lint" Requires-
 Dist: isort; extra == "lint" Requires-Dist: pylint; extra == "lint" Requires-
 Dist: qbraid-cli; extra == "lint" Provides-Extra: docs Requires-Dist:
```

### Comparing `qbraid-0.7.0.dev20240516020308/qbraid.egg-info/SOURCES.txt` & `qbraid-0.7.0.dev20240523162156/qbraid.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
 qbraid/transpiler/conversions/pyquil/pyquil_to_cirq.py
 qbraid/transpiler/conversions/pytket/__init__.py
 qbraid/transpiler/conversions/pytket/pytket_extras.py
 qbraid/transpiler/conversions/pytket/pytket_to_qasm2.py
 qbraid/transpiler/conversions/qasm2/__init__.py
 qbraid/transpiler/conversions/qasm2/cirq_custom.py
 qbraid/transpiler/conversions/qasm2/cirq_qasm_parser.py
+qbraid/transpiler/conversions/qasm2/qasm2_extras.py
 qbraid/transpiler/conversions/qasm2/qasm2_to_cirq.py
 qbraid/transpiler/conversions/qasm2/qasm2_to_pytket.py
 qbraid/transpiler/conversions/qasm2/qasm2_to_qasm3.py
 qbraid/transpiler/conversions/qasm2/qasm2_to_qiskit.py
 qbraid/transpiler/conversions/qasm3/__init__.py
 qbraid/transpiler/conversions/qasm3/qasm3_extras.py
 qbraid/transpiler/conversions/qasm3/qasm3_to_braket.py
```

### Comparing `qbraid-0.7.0.dev20240516020308/tools/set_provider_configs.py` & `qbraid-0.7.0.dev20240523162156/tools/set_provider_configs.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,13 +46,8 @@
     token = token or os.getenv("QISKIT_IBM_TOKEN", "MY_IBM_QUANTUM_TOKEN")
     channel = channel or os.getenv("QISKIT_IBM_CHANNEL", "ibm_quantum")
     QiskitRuntimeService.save_account(token=token, channel=channel, overwrite=overwrite, **kwargs)
 
 
 if __name__ == "__main__":
     if not skip_remote_tests:
-        qbraid_configure()
         aws_configure()
-        try:
-            ibm_configure()
-        except ImportError:
-            logger.error("qiskit-ibm-runtime not installed, skipping IBM Quantum configuration")
```

### Comparing `qbraid-0.7.0.dev20240516020308/tox.ini` & `qbraid-0.7.0.dev20240523162156/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 [testenv]
 commands_pre = python -m pip install --editable .
 basepython = python3
 deps =
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/requirements-dev.txt
 pass_env =
-    QBRAID_API_KEY
     AWS_ACCESS_KEY_ID
     AWS_SECRET_ACCESS_KEY
-    QISKIT_IBM_TOKEN
     QBRAID_RUN_REMOTE_TESTS
 
 [testenv:unit-tests]
 description = Run pytests and generate coverage report.
 commands =
     python3 tools/set_provider_configs.py
     coverage run -m pytest -x tests/programs \
@@ -31,15 +29,15 @@
                               tests/visualization \
                               tests/top_level \
                            -W ignore::DeprecationWarning \
                            -W ignore::PendingDeprecationWarning \
                            -W ignore::urllib3.exceptions.InsecureRequestWarning \
                            -W ignore::RuntimeWarning
     coverage combine
-    coverage report --omit=qbraid/visualization/draw_circuit.py,qbraid/visualization/plot_conversions.py,qbraid/_compat.py
+    coverage report --omit=qbraid/visualization/draw_circuit.py,qbraid/visualization/plot_conversions.py,qbraid/_compat.py,qbraid/transpiler/conversions/qasm2/qasm2_extras.py,qbraid/runtime/ionq/*
     coverage html
     coverage xml
 
 [testenv:docs]
 description = Use sphinx to build the HTML docs.
 extras =
     docs
```

