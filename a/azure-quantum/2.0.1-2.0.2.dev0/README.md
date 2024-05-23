# Comparing `tmp/azure-quantum-2.0.1.tar.gz` & `tmp/azure-quantum-2.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-quantum-2.0.1.tar", last modified: Fri May  3 23:30:57 2024, max compression
+gzip compressed data, was "azure-quantum-2.0.2.dev0.tar", last modified: Thu May 23 02:17:16 2024, max compression
```

## Comparing `azure-quantum-2.0.1.tar` & `azure-quantum-2.0.2.dev0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.667572 azure-quantum-2.0.1/
--rw-rw-rw-   0        0        0     5605 2024-05-03 23:30:57.667572 azure-quantum-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5050 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.601638 azure-quantum-2.0.1/azure/
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/
--rw-rw-rw-   0        0        0      508 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/_authentication/
--rw-rw-rw-   0        0        0      236 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_authentication/__init__.py
--rw-rw-rw-   0        0        0     4848 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_authentication/_chained.py
--rw-rw-rw-   0        0        0     6625 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_authentication/_default.py
--rw-rw-rw-   0        0        0     3616 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_authentication/_token.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/_client/
--rw-rw-rw-   0        0        0      896 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/__init__.py
--rw-rw-rw-   0        0        0     7143 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/_client.py
--rw-rw-rw-   0        0        0     4440 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/_configuration.py
--rw-rw-rw-   0        0        0      694 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/_patch.py
--rw-rw-rw-   0        0        0    81097 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/_serialization.py
--rw-rw-rw-   0        0        0      996 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/_vendor.py
--rw-rw-rw-   0        0        0      495 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure/quantum/_client/_version.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/_client/models/
--rw-rw-rw-   0        0        0     2100 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/models/__init__.py
--rw-rw-rw-   0        0        0     2977 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/models/_enums.py
--rw-rw-rw-   0        0        0    41810 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/models/_models.py
--rw-rw-rw-   0        0        0      694 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/models/_patch.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/_client/operations/
--rw-rw-rw-   0        0        0     1154 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/operations/__init__.py
--rw-rw-rw-   0        0        0    81928 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/operations/_operations.py
--rw-rw-rw-   0        0        0      694 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/operations/_patch.py
--rw-rw-rw-   0        0        0     3219 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_constants.py
--rw-rw-rw-   0        0        0    21685 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_workspace_connection_params.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/argument_types/
--rw-rw-rw-   0        0        0      271 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/argument_types/__init__.py
--rw-rw-rw-   0        0        0     1041 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/argument_types/types.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/chemistry/
--rw-rw-rw-   0        0        0      351 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/chemistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.632892 azure-quantum-2.0.1/azure/quantum/cirq/
--rw-rw-rw-   0        0        0      227 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/__init__.py
--rw-rw-rw-   0        0        0     3031 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/job.py
--rw-rw-rw-   0        0        0     8880 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/service.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.632892 azure-quantum-2.0.1/azure/quantum/cirq/targets/
--rw-rw-rw-   0        0        0      574 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/targets/__init__.py
--rw-rw-rw-   0        0        0     6804 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/targets/ionq.py
--rw-rw-rw-   0        0        0     4537 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/targets/quantinuum.py
--rw-rw-rw-   0        0        0     2184 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/targets/target.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.632892 azure-quantum-2.0.1/azure/quantum/job/
--rw-rw-rw-   0        0        0      829 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/__init__.py
--rw-rw-rw-   0        0        0    13876 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/base_job.py
--rw-rw-rw-   0        0        0     1877 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/filtered_job.py
--rw-rw-rw-   0        0        0     6390 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/job.py
--rw-rw-rw-   0        0        0     1597 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/job_failed_with_results_error.py
--rw-rw-rw-   0        0        0    11961 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/session.py
--rw-rw-rw-   0        0        0     1380 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/workspace_item.py
--rw-rw-rw-   0        0        0     1200 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/workspace_item_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.632892 azure-quantum-2.0.1/azure/quantum/qiskit/
--rw-rw-rw-   0        0        0      314 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.632892 azure-quantum-2.0.1/azure/quantum/qiskit/backends/
--rw-rw-rw-   0        0        0     1163 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/__init__.py
--rw-rw-rw-   0        0        0    20467 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/backend.py
--rw-rw-rw-   0        0        0    18024 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/ionq.py
--rw-rw-rw-   0        0        0     3478 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/microsoft.py
--rw-rw-rw-   0        0        0     4893 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/qci.py
--rw-rw-rw-   0        0        0    13437 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/quantinuum.py
--rw-rw-rw-   0        0        0     4322 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/rigetti.py
--rw-rw-rw-   0        0        0    14370 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/job.py
--rw-rw-rw-   0        0        0    10946 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/provider.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.648513 azure-quantum-2.0.1/azure/quantum/qiskit/results/
--rw-rw-rw-   0        0        0        0 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/results/__init__.py
--rw-rw-rw-   0        0        0      814 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/results/resource_estimator.py
--rw-rw-rw-   0        0        0    12556 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/storage.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.648513 azure-quantum-2.0.1/azure/quantum/target/
--rw-rw-rw-   0        0        0      689 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/__init__.py
--rw-rw-rw-   0        0        0     8130 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/ionq.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.648513 azure-quantum-2.0.1/azure/quantum/target/microsoft/
--rw-rw-rw-   0        0        0      570 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.648513 azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/
--rw-rw-rw-   0        0        0       70 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.648513 azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/dft/
--rw-rw-rw-   0        0        0      224 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/dft/__init__.py
--rw-rw-rw-   0        0        0     2936 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/dft/job.py
--rw-rw-rw-   0        0        0     2556 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/dft/target.py
--rw-rw-rw-   0        0        0     1249 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/job.py
--rw-rw-rw-   0        0        0    18784 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/result.py
--rw-rw-rw-   0        0        0    17879 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/target.py
--rw-rw-rw-   0        0        0     9130 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/params.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.648513 azure-quantum-2.0.1/azure/quantum/target/pasqal/
--rw-rw-rw-   0        0        0      348 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/pasqal/__init__.py
--rw-rw-rw-   0        0        0     1463 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/pasqal/result.py
--rw-rw-rw-   0        0        0     4833 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/pasqal/target.py
--rw-rw-rw-   0        0        0     7612 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/quantinuum.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.664138 azure-quantum-2.0.1/azure/quantum/target/rigetti/
--rw-rw-rw-   0        0        0      378 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/rigetti/__init__.py
--rw-rw-rw-   0        0        0     2334 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/rigetti/result.py
--rw-rw-rw-   0        0        0     7048 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/rigetti/target.py
--rw-rw-rw-   0        0        0    13868 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/target.py
--rw-rw-rw-   0        0        0     5266 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/target_factory.py
--rw-rw-rw-   0        0        0      235 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure/quantum/version.py
--rw-rw-rw-   0        0        0    23438 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/workspace.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.667572 azure-quantum-2.0.1/azure_quantum.egg-info/
--rw-rw-rw-   0        0        0     5605 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure_quantum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3130 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure_quantum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure_quantum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      744 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure_quantum.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure_quantum.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       52 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/requirements-cirq.txt
--rw-rw-rw-   0        0        0      112 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/requirements-dev.txt
--rw-rw-rw-   0        0        0      117 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/requirements-qiskit.txt
--rw-rw-rw-   0        0        0       19 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/requirements-qsharp.txt
--rw-rw-rw-   0        0        0      275 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/requirements-quil.txt
--rw-rw-rw-   0        0        0      192 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 23:30:57.667572 azure-quantum-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3838 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:16.962972 azure-quantum-2.0.2.dev0/
+-rw-rw-rw-   0        0        0     5610 2024-05-23 02:17:16.962972 azure-quantum-2.0.2.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     5050 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.133335 azure-quantum-2.0.2.dev0/azure/
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.148950 azure-quantum-2.0.2.dev0/azure/quantum/
+-rw-rw-rw-   0        0        0      508 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.148950 azure-quantum-2.0.2.dev0/azure/quantum/_authentication/
+-rw-rw-rw-   0        0        0      236 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_authentication/__init__.py
+-rw-rw-rw-   0        0        0     4848 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_authentication/_chained.py
+-rw-rw-rw-   0        0        0     6625 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_authentication/_default.py
+-rw-rw-rw-   0        0        0     3616 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_authentication/_token.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.148950 azure-quantum-2.0.2.dev0/azure/quantum/_client/
+-rw-rw-rw-   0        0        0      896 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/__init__.py
+-rw-rw-rw-   0        0        0     7143 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/_client.py
+-rw-rw-rw-   0        0        0     4440 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/_configuration.py
+-rw-rw-rw-   0        0        0      694 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/_patch.py
+-rw-rw-rw-   0        0        0    81097 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/_serialization.py
+-rw-rw-rw-   0        0        0      996 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/_vendor.py
+-rw-rw-rw-   0        0        0      500 2024-05-23 02:17:14.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.164576 azure-quantum-2.0.2.dev0/azure/quantum/_client/models/
+-rw-rw-rw-   0        0        0     2100 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/models/__init__.py
+-rw-rw-rw-   0        0        0     2977 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/models/_enums.py
+-rw-rw-rw-   0        0        0    41810 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/models/_models.py
+-rw-rw-rw-   0        0        0      694 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/models/_patch.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.946199 azure-quantum-2.0.2.dev0/azure/quantum/_client/operations/
+-rw-rw-rw-   0        0        0     1154 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/operations/__init__.py
+-rw-rw-rw-   0        0        0    81928 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/operations/_operations.py
+-rw-rw-rw-   0        0        0      694 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_client/operations/_patch.py
+-rw-rw-rw-   0        0        0     3350 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_constants.py
+-rw-rw-rw-   0        0        0    21685 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/_workspace_connection_params.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.946199 azure-quantum-2.0.2.dev0/azure/quantum/argument_types/
+-rw-rw-rw-   0        0        0      271 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/argument_types/__init__.py
+-rw-rw-rw-   0        0        0     1041 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/argument_types/types.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.946199 azure-quantum-2.0.2.dev0/azure/quantum/chemistry/
+-rw-rw-rw-   0        0        0      351 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/chemistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.946199 azure-quantum-2.0.2.dev0/azure/quantum/cirq/
+-rw-rw-rw-   0        0        0      227 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/cirq/__init__.py
+-rw-rw-rw-   0        0        0     3031 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/cirq/job.py
+-rw-rw-rw-   0        0        0     8880 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/cirq/service.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.946199 azure-quantum-2.0.2.dev0/azure/quantum/cirq/targets/
+-rw-rw-rw-   0        0        0      574 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/cirq/targets/__init__.py
+-rw-rw-rw-   0        0        0     6804 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/cirq/targets/ionq.py
+-rw-rw-rw-   0        0        0     4537 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/cirq/targets/quantinuum.py
+-rw-rw-rw-   0        0        0     2184 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/cirq/targets/target.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.961764 azure-quantum-2.0.2.dev0/azure/quantum/job/
+-rw-rw-rw-   0        0        0      829 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/job/__init__.py
+-rw-rw-rw-   0        0        0    13876 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/job/base_job.py
+-rw-rw-rw-   0        0        0     1877 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/job/filtered_job.py
+-rw-rw-rw-   0        0        0     6390 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/job/job.py
+-rw-rw-rw-   0        0        0     1597 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/job/job_failed_with_results_error.py
+-rw-rw-rw-   0        0        0    11961 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/job/session.py
+-rw-rw-rw-   0        0        0     1380 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/job/workspace_item.py
+-rw-rw-rw-   0        0        0     1200 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/job/workspace_item_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.961764 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/
+-rw-rw-rw-   0        0        0      314 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.961764 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/
+-rw-rw-rw-   0        0        0     1163 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/__init__.py
+-rw-rw-rw-   0        0        0    20467 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/backend.py
+-rw-rw-rw-   0        0        0    18024 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/ionq.py
+-rw-rw-rw-   0        0        0     3478 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/microsoft.py
+-rw-rw-rw-   0        0        0     4893 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/qci.py
+-rw-rw-rw-   0        0        0    13437 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/quantinuum.py
+-rw-rw-rw-   0        0        0     4322 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/rigetti.py
+-rw-rw-rw-   0        0        0    14370 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/job.py
+-rw-rw-rw-   0        0        0    10946 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/provider.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.961764 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/results/
+-rw-rw-rw-   0        0        0        0 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/results/__init__.py
+-rw-rw-rw-   0        0        0      814 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/qiskit/results/resource_estimator.py
+-rw-rw-rw-   0        0        0    12556 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.977386 azure-quantum-2.0.2.dev0/azure/quantum/target/
+-rw-rw-rw-   0        0        0      689 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/__init__.py
+-rw-rw-rw-   0        0        0     8130 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/ionq.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.977386 azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/
+-rw-rw-rw-   0        0        0      570 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:15.977386 azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/elements/
+-rw-rw-rw-   0        0        0       70 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/elements/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:16.947371 azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/elements/dft/
+-rw-rw-rw-   0        0        0      224 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/elements/dft/__init__.py
+-rw-rw-rw-   0        0        0     2936 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/elements/dft/job.py
+-rw-rw-rw-   0        0        0     2556 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/elements/dft/target.py
+-rw-rw-rw-   0        0        0     1249 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/job.py
+-rw-rw-rw-   0        0        0    18784 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/result.py
+-rw-rw-rw-   0        0        0    17879 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/target.py
+-rw-rw-rw-   0        0        0     9130 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/params.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:16.947371 azure-quantum-2.0.2.dev0/azure/quantum/target/pasqal/
+-rw-rw-rw-   0        0        0      348 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/pasqal/__init__.py
+-rw-rw-rw-   0        0        0     1463 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/pasqal/result.py
+-rw-rw-rw-   0        0        0     4833 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/pasqal/target.py
+-rw-rw-rw-   0        0        0     7612 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/quantinuum.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:16.947371 azure-quantum-2.0.2.dev0/azure/quantum/target/rigetti/
+-rw-rw-rw-   0        0        0      378 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/rigetti/__init__.py
+-rw-rw-rw-   0        0        0     2334 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/rigetti/result.py
+-rw-rw-rw-   0        0        0     7048 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/rigetti/target.py
+-rw-rw-rw-   0        0        0    13868 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/target.py
+-rw-rw-rw-   0        0        0     5266 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/target/target_factory.py
+-rw-rw-rw-   0        0        0      240 2024-05-23 02:17:14.000000 azure-quantum-2.0.2.dev0/azure/quantum/version.py
+-rw-rw-rw-   0        0        0    23438 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/azure/quantum/workspace.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:17:16.962972 azure-quantum-2.0.2.dev0/azure_quantum.egg-info/
+-rw-rw-rw-   0        0        0     5610 2024-05-23 02:17:15.000000 azure-quantum-2.0.2.dev0/azure_quantum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3130 2024-05-23 02:17:15.000000 azure-quantum-2.0.2.dev0/azure_quantum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 02:17:15.000000 azure-quantum-2.0.2.dev0/azure_quantum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      744 2024-05-23 02:17:15.000000 azure-quantum-2.0.2.dev0/azure_quantum.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-23 02:17:15.000000 azure-quantum-2.0.2.dev0/azure_quantum.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       52 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/requirements-cirq.txt
+-rw-rw-rw-   0        0        0      112 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/requirements-dev.txt
+-rw-rw-rw-   0        0        0      117 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/requirements-qiskit.txt
+-rw-rw-rw-   0        0        0       19 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/requirements-qsharp.txt
+-rw-rw-rw-   0        0        0      275 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/requirements-quil.txt
+-rw-rw-rw-   0        0        0      192 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 02:17:16.962972 azure-quantum-2.0.2.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     3838 2024-05-23 02:16:27.000000 azure-quantum-2.0.2.dev0/setup.py
```

### Comparing `azure-quantum-2.0.1/PKG-INFO` & `azure-quantum-2.0.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-quantum
-Version: 2.0.1
+Version: 2.0.2.dev0
 Summary: Python client for Azure Quantum
 Home-page: https://github.com/microsoft/azure-quantum-python
 Author: Microsoft
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `azure-quantum-2.0.1/README.md` & `azure-quantum-2.0.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_authentication/_chained.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_authentication/_chained.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_authentication/_default.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_authentication/_default.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_authentication/_token.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_authentication/_token.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/__init__.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/_client.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/_client.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/_configuration.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/_patch.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/_serialization.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/_vendor.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/models/__init__.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/models/_enums.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/models/_enums.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/models/_models.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/models/_models.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/models/_patch.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/operations/__init__.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/operations/_operations.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_client/operations/_patch.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_client/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/_constants.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     RESOURCE_GROUP = "RESOURCE_GROUP"
     QUANTUM_SUBSCRIPTION_ID = "AZURE_QUANTUM_SUBSCRIPTION_ID"
     SUBSCRIPTION_ID = "SUBSCRIPTION_ID"
     WORKSPACE_NAME = "AZURE_QUANTUM_WORKSPACE_NAME"
     QUANTUM_ENV = "AZURE_QUANTUM_ENV"
     AZURE_CLIENT_ID = SdkEnvironmentVariables.AZURE_CLIENT_ID
     AZURE_CLIENT_SECRET = SdkEnvironmentVariables.AZURE_CLIENT_SECRET
+    AZURE_CLIENT_CERTIFICATE_PATH = SdkEnvironmentVariables.AZURE_CLIENT_CERTIFICATE_PATH
     AZURE_TENANT_ID = SdkEnvironmentVariables.AZURE_TENANT_ID
     QUANTUM_TOKEN_FILE = "AZURE_QUANTUM_TOKEN_FILE"
     CONNECTION_STRING = "AZURE_QUANTUM_CONNECTION_STRING"
     ALL = [
         USER_AGENT_APPID,
         QUANTUM_LOCATION,
         LOCATION,
@@ -31,14 +32,15 @@
         RESOURCE_GROUP,
         QUANTUM_SUBSCRIPTION_ID,
         SUBSCRIPTION_ID,
         WORKSPACE_NAME,
         QUANTUM_ENV,
         AZURE_CLIENT_ID,
         AZURE_CLIENT_SECRET,
+        AZURE_CLIENT_CERTIFICATE_PATH,
         AZURE_TENANT_ID,
         QUANTUM_TOKEN_FILE,
         CONNECTION_STRING,
     ]
 
 
 class EnvironmentKind(Enum):
```

### Comparing `azure-quantum-2.0.1/azure/quantum/_workspace_connection_params.py` & `azure-quantum-2.0.2.dev0/azure/quantum/_workspace_connection_params.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/argument_types/types.py` & `azure-quantum-2.0.2.dev0/azure/quantum/argument_types/types.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/cirq/job.py` & `azure-quantum-2.0.2.dev0/azure/quantum/cirq/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/cirq/service.py` & `azure-quantum-2.0.2.dev0/azure/quantum/cirq/service.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/cirq/targets/__init__.py` & `azure-quantum-2.0.2.dev0/azure/quantum/cirq/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/cirq/targets/ionq.py` & `azure-quantum-2.0.2.dev0/azure/quantum/cirq/targets/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/cirq/targets/quantinuum.py` & `azure-quantum-2.0.2.dev0/azure/quantum/cirq/targets/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/cirq/targets/target.py` & `azure-quantum-2.0.2.dev0/azure/quantum/cirq/targets/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/job/__init__.py` & `azure-quantum-2.0.2.dev0/azure/quantum/job/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/job/base_job.py` & `azure-quantum-2.0.2.dev0/azure/quantum/job/base_job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/job/filtered_job.py` & `azure-quantum-2.0.2.dev0/azure/quantum/job/filtered_job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/job/job.py` & `azure-quantum-2.0.2.dev0/azure/quantum/job/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/job/job_failed_with_results_error.py` & `azure-quantum-2.0.2.dev0/azure/quantum/job/job_failed_with_results_error.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/job/session.py` & `azure-quantum-2.0.2.dev0/azure/quantum/job/session.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/job/workspace_item.py` & `azure-quantum-2.0.2.dev0/azure/quantum/job/workspace_item.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/job/workspace_item_factory.py` & `azure-quantum-2.0.2.dev0/azure/quantum/job/workspace_item_factory.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/qiskit/backends/__init__.py` & `azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/qiskit/backends/backend.py` & `azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/backend.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/qiskit/backends/ionq.py` & `azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/qiskit/backends/microsoft.py` & `azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/microsoft.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/qiskit/backends/qci.py` & `azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/qci.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/qiskit/backends/quantinuum.py` & `azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/qiskit/backends/rigetti.py` & `azure-quantum-2.0.2.dev0/azure/quantum/qiskit/backends/rigetti.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/qiskit/job.py` & `azure-quantum-2.0.2.dev0/azure/quantum/qiskit/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/qiskit/provider.py` & `azure-quantum-2.0.2.dev0/azure/quantum/qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/qiskit/results/resource_estimator.py` & `azure-quantum-2.0.2.dev0/azure/quantum/qiskit/results/resource_estimator.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/storage.py` & `azure-quantum-2.0.2.dev0/azure/quantum/storage.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/__init__.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/ionq.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/microsoft/__init__.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/dft/job.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/elements/dft/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/dft/target.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/elements/dft/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/microsoft/job.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/microsoft/result.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/result.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/microsoft/target.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/microsoft/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/params.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/params.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/pasqal/result.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/pasqal/result.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/pasqal/target.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/pasqal/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/quantinuum.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/rigetti/result.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/rigetti/result.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/rigetti/target.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/rigetti/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/target.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/target/target_factory.py` & `azure-quantum-2.0.2.dev0/azure/quantum/target/target_factory.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure/quantum/workspace.py` & `azure-quantum-2.0.2.dev0/azure/quantum/workspace.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure_quantum.egg-info/PKG-INFO` & `azure-quantum-2.0.2.dev0/azure_quantum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-quantum
-Version: 2.0.1
+Version: 2.0.2.dev0
 Summary: Python client for Azure Quantum
 Home-page: https://github.com/microsoft/azure-quantum-python
 Author: Microsoft
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `azure-quantum-2.0.1/azure_quantum.egg-info/SOURCES.txt` & `azure-quantum-2.0.2.dev0/azure_quantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/azure_quantum.egg-info/requires.txt` & `azure-quantum-2.0.2.dev0/azure_quantum.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.1/setup.py` & `azure-quantum-2.0.2.dev0/setup.py`

 * *Files identical despite different names*

