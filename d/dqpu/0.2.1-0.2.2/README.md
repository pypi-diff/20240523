# Comparing `tmp/dqpu-0.2.1.tar.gz` & `tmp/dqpu-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqpu-0.2.1.tar", last modified: Sun May 19 10:24:23 2024, max compression
+gzip compressed data, was "dqpu-0.2.2.tar", last modified: Thu May 23 09:50:06 2024, max compression
```

## Comparing `dqpu-0.2.1.tar` & `dqpu-0.2.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-19 10:24:23.098284 dqpu-0.2.1/
--rw-r--r--   0 dakk      (1000) dakk      (1000)    10255 2024-04-30 07:00:05.000000 dqpu-0.2.1/LICENSE
--rw-r--r--   0 dakk      (1000) dakk      (1000)     8948 2024-05-19 10:24:23.098284 dqpu-0.2.1/PKG-INFO
--rw-r--r--   0 dakk      (1000) dakk      (1000)     8120 2024-05-19 09:35:04.000000 dqpu-0.2.1/README.md
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-19 10:24:23.088283 dqpu-0.2.1/dqpu/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      593 2024-05-19 10:20:38.000000 dqpu-0.2.1/dqpu/__init__.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-19 10:24:23.091617 dqpu-0.2.1/dqpu/backends/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      569 2024-05-17 14:08:15.000000 dqpu-0.2.1/dqpu/backends/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1234 2024-05-19 08:07:22.000000 dqpu-0.2.1/dqpu/backends/base.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-19 10:24:23.091617 dqpu-0.2.1/dqpu/backends/qiskit/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      717 2024-05-17 11:37:05.000000 dqpu-0.2.1/dqpu/backends/qiskit/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3984 2024-05-19 08:10:05.000000 dqpu-0.2.1/dqpu/backends/qiskit/dqpubackend.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3265 2024-05-19 08:07:22.000000 dqpu-0.2.1/dqpu/backends/qiskit/dqpujob.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1198 2024-05-19 08:07:22.000000 dqpu-0.2.1/dqpu/backends/qiskit/dqpuprovider.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-19 10:24:23.094950 dqpu-0.2.1/dqpu/blockchain/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      726 2024-05-15 08:24:53.000000 dqpu-0.2.1/dqpu/blockchain/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)      862 2024-05-15 09:15:07.000000 dqpu-0.2.1/dqpu/blockchain/blockchain.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2495 2024-05-17 14:02:38.000000 dqpu-0.2.1/dqpu/blockchain/ipfs_gateway.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6065 2024-05-19 08:09:28.000000 dqpu-0.2.1/dqpu/blockchain/near.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6980 2024-05-19 08:10:05.000000 dqpu-0.2.1/dqpu/cli.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-19 10:24:23.094950 dqpu-0.2.1/dqpu/q/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      801 2024-05-07 07:05:38.000000 dqpu-0.2.1/dqpu/q/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     6282 2024-05-15 10:01:00.000000 dqpu-0.2.1/dqpu/q/circuit.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1260 2024-05-06 15:31:42.000000 dqpu-0.2.1/dqpu/q/gate.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2013 2024-05-15 08:42:29.000000 dqpu-0.2.1/dqpu/q/gates.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2262 2024-05-14 10:21:28.000000 dqpu-0.2.1/dqpu/q/utils.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-19 10:24:23.094950 dqpu-0.2.1/dqpu/sampler/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      852 2024-05-19 08:10:05.000000 dqpu-0.2.1/dqpu/sampler/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1012 2024-05-15 09:32:39.000000 dqpu-0.2.1/dqpu/sampler/aersimulatorsampler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     5943 2024-05-15 10:21:58.000000 dqpu-0.2.1/dqpu/sampler/dasksimulatorsampler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)      836 2024-05-15 09:31:36.000000 dqpu-0.2.1/dqpu/sampler/sampler.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4155 2024-05-17 15:26:58.000000 dqpu-0.2.1/dqpu/samplernode.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     1310 2024-05-15 09:31:36.000000 dqpu-0.2.1/dqpu/utils.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-19 10:24:23.098284 dqpu-0.2.1/dqpu/verifier/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      691 2024-05-07 08:01:59.000000 dqpu-0.2.1/dqpu/verifier/__init__.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     4146 2024-05-19 07:59:30.000000 dqpu-0.2.1/dqpu/verifier/basictrapper.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     2322 2024-05-19 07:59:25.000000 dqpu-0.2.1/dqpu/verifier/trapper.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)      652 2024-05-07 05:50:44.000000 dqpu-0.2.1/dqpu/verifier/verifier.py
--rw-r--r--   0 dakk      (1000) dakk      (1000)     5879 2024-05-17 13:35:39.000000 dqpu-0.2.1/dqpu/verifiernode.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-19 10:24:23.091617 dqpu-0.2.1/dqpu.egg-info/
--rw-r--r--   0 dakk      (1000) dakk      (1000)     8948 2024-05-19 10:24:22.000000 dqpu-0.2.1/dqpu.egg-info/PKG-INFO
--rw-r--r--   0 dakk      (1000) dakk      (1000)      949 2024-05-19 10:24:23.000000 dqpu-0.2.1/dqpu.egg-info/SOURCES.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2024-05-19 10:24:22.000000 dqpu-0.2.1/dqpu.egg-info/dependency_links.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)      190 2024-05-19 10:24:22.000000 dqpu-0.2.1/dqpu.egg-info/entry_points.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2024-05-19 10:24:21.000000 dqpu-0.2.1/dqpu.egg-info/not-zip-safe
--rw-r--r--   0 dakk      (1000) dakk      (1000)      156 2024-05-19 10:24:22.000000 dqpu-0.2.1/dqpu.egg-info/requires.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)        5 2024-05-19 10:24:22.000000 dqpu-0.2.1/dqpu.egg-info/top_level.txt
--rw-r--r--   0 dakk      (1000) dakk      (1000)      382 2024-05-19 10:24:23.098284 dqpu-0.2.1/setup.cfg
--rw-r--r--   0 dakk      (1000) dakk      (1000)     3198 2024-05-17 11:37:01.000000 dqpu-0.2.1/setup.py
-drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-19 10:24:23.098284 dqpu-0.2.1/test/
--rw-r--r--   0 dakk      (1000) dakk      (1000)      741 2024-05-07 08:37:08.000000 dqpu-0.2.1/test/test_empty.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.379837 dqpu-0.2.2/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)    10255 2024-04-30 07:00:05.000000 dqpu-0.2.2/LICENSE
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     9223 2024-05-23 09:50:06.379837 dqpu-0.2.2/PKG-INFO
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     8395 2024-05-22 10:59:29.000000 dqpu-0.2.2/README.md
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.369836 dqpu-0.2.2/dqpu/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      593 2024-05-23 09:47:45.000000 dqpu-0.2.2/dqpu/__init__.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.373170 dqpu-0.2.2/dqpu/backends/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      569 2024-05-17 14:08:15.000000 dqpu-0.2.2/dqpu/backends/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1234 2024-05-19 08:07:22.000000 dqpu-0.2.2/dqpu/backends/base.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.373170 dqpu-0.2.2/dqpu/backends/qiskit/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      717 2024-05-17 11:37:05.000000 dqpu-0.2.2/dqpu/backends/qiskit/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4026 2024-05-23 09:22:47.000000 dqpu-0.2.2/dqpu/backends/qiskit/dqpubackend.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3288 2024-05-20 10:03:30.000000 dqpu-0.2.2/dqpu/backends/qiskit/dqpujob.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1198 2024-05-19 08:07:22.000000 dqpu-0.2.2/dqpu/backends/qiskit/dqpuprovider.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.373170 dqpu-0.2.2/dqpu/blockchain/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      726 2024-05-15 08:24:53.000000 dqpu-0.2.2/dqpu/blockchain/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1531 2024-05-22 06:01:25.000000 dqpu-0.2.2/dqpu/blockchain/blockchain.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2495 2024-05-22 14:41:31.000000 dqpu-0.2.2/dqpu/blockchain/ipfs_gateway.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6404 2024-05-23 09:41:09.000000 dqpu-0.2.2/dqpu/blockchain/near.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     7006 2024-05-23 09:41:33.000000 dqpu-0.2.2/dqpu/cli.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.376503 dqpu-0.2.2/dqpu/q/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      801 2024-05-07 07:05:38.000000 dqpu-0.2.2/dqpu/q/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6613 2024-05-23 09:41:41.000000 dqpu-0.2.2/dqpu/q/circuit.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1260 2024-05-23 08:49:53.000000 dqpu-0.2.2/dqpu/q/gate.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2322 2024-05-23 09:22:47.000000 dqpu-0.2.2/dqpu/q/gates.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2262 2024-05-14 10:21:28.000000 dqpu-0.2.2/dqpu/q/utils.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.376503 dqpu-0.2.2/dqpu/sampler/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      969 2024-05-23 09:41:33.000000 dqpu-0.2.2/dqpu/sampler/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1072 2024-05-23 09:22:47.000000 dqpu-0.2.2/dqpu/sampler/aersimulatorsampler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     5943 2024-05-15 10:21:58.000000 dqpu-0.2.2/dqpu/sampler/dasksimulatorsampler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1185 2024-05-23 09:22:47.000000 dqpu-0.2.2/dqpu/sampler/qracksimulatorsampler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1484 2024-05-22 06:06:47.000000 dqpu-0.2.2/dqpu/sampler/sampler.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6025 2024-05-23 09:22:47.000000 dqpu-0.2.2/dqpu/samplernode.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     1636 2024-05-23 09:22:47.000000 dqpu-0.2.2/dqpu/utils.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.376503 dqpu-0.2.2/dqpu/verifier/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      691 2024-05-07 08:01:59.000000 dqpu-0.2.2/dqpu/verifier/__init__.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     4158 2024-05-23 09:33:18.000000 dqpu-0.2.2/dqpu/verifier/basictrapper.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     2322 2024-05-19 07:59:25.000000 dqpu-0.2.2/dqpu/verifier/trapper.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      652 2024-05-07 05:50:44.000000 dqpu-0.2.2/dqpu/verifier/verifier.py
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     6374 2024-05-23 09:41:33.000000 dqpu-0.2.2/dqpu/verifiernode.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.373170 dqpu-0.2.2/dqpu.egg-info/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     9223 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/PKG-INFO
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      987 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/SOURCES.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/dependency_links.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      190 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/entry_points.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)        1 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/not-zip-safe
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      194 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/requires.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)        5 2024-05-23 09:50:06.000000 dqpu-0.2.2/dqpu.egg-info/top_level.txt
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      382 2024-05-23 09:50:06.379837 dqpu-0.2.2/setup.cfg
+-rw-r--r--   0 dakk      (1000) dakk      (1000)     3198 2024-05-22 05:34:05.000000 dqpu-0.2.2/setup.py
+drwxr-xr-x   0 dakk      (1000) dakk      (1000)        0 2024-05-23 09:50:06.379837 dqpu-0.2.2/test/
+-rw-r--r--   0 dakk      (1000) dakk      (1000)      741 2024-05-07 08:37:08.000000 dqpu-0.2.2/test/test_empty.py
```

### Comparing `dqpu-0.2.1/LICENSE` & `dqpu-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/PKG-INFO` & `dqpu-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqpu
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/dakk/dqpu
 Author: Davide Gessa
 Author-email: gessadavide@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dakk/dqpu/issues/
 Project-URL: Documentation, https://dakk.github.io/dqpu
 Project-URL: Source, https://github.com/dakk/dqpu
@@ -20,15 +20,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dqpu
 
 ![CI Status](https://github.com/dakk/dqpu/actions/workflows/ci.yaml/badge.svg)
 ![Contract CI Status](https://github.com/dakk/dqpu/actions/workflows/ci-contract.yaml/badge.svg)
+![PyPI - Version](https://img.shields.io/pypi/v/dqpu)
 ![License: Apache 2.0](https://img.shields.io/badge/license-Apache_2.0-blue)
+[![Downloads](https://static.pepy.tech/badge/dqpu)](https://pepy.tech/project/dqpu)
 
 A Web3-Powered (Near), Decentralized Quantum Simulator with Verifiable Computation. 
 
 DQPU (Decentralized Quantum Processing Unit) introduces a novel, decentralized approach to quantum computing that leverages the power of blockchain and smart contracts. It addresses the challenges of securely and reliably executing quantum computations in a trustless and transparent manner, while fostering a competitive ecosystem for quantum resource providers.
 
 
 ## Workflow
@@ -42,18 +44,18 @@
 
 The following process outlines how clients can submit quantum circuits for sampling using the DQPU contract:
 
 1. **Client Submits Job**: A *Client* sends a quantum circuit along with a reward to the DQPU smart contract. The circuit data is uploaded to a distributed file storage system like IPFS. The smart contract adds the job to a queue in a 'pending-validation' state with the associated reward.
 
 2. **Verifier Validates Circuit**: A *Verifier*[^1] validates the submitted circuit. This might involve checks for syntax errors or ensuring the circuit is within allowed parameters. The verifier also adds special verification elements (traps) into the circuit and add the new circuit to the contract[^2]. Once validated, the job moves to a 'waiting' state, becomes 'invalid' otherwise.
 
-3. **Simulation or Hardware Execution**: A *Sampler* retrieves a job from the waiting list. It then either simulates the circuit on a software program or executes it on real quantum hardware, depending on the job requirements and available resources. The simulation or execution result is submitted back to the smart contract with a cautional deposit (a percentage of the reward). The job status changes to 'validating'.
+3. **Simulation or Hardware Execution**: A *Sampler* retrieves a job from the waiting list. It then either simulates the circuit on a software program or executes it on real quantum hardware, depending on the job requirements and available resources. The simulation or execution result is submitted back to the smart contract with a security deposit (a percentage of the reward). The job status changes to 'validating'.
 
 4. **Verifier Checks Result**: The same *Verifier* from step 2 examines the returned result. The *Verifier* specifically checks the traps inserted earlier to ensure the result hasn't been tampered with. If the trap verification succeeds, the job status is updated to 'executed' and the trap is disclosed by the *Verifier*. The *Sampler* account receives the reward, while the *Verifier* receives a percentage of this reward.
-If the trap verification fails, the job returns in 'waiting' state (and the *Verifier* receives the cautional deposit of the *Sampler*).
+If the trap verification fails, the job returns in 'waiting' state (and the *Verifier* receives the security deposit of the *Sampler*).
 
 5. **Client Receives Result**: Once the job is marked as 'executed', the *Client* can retrieve the final result from the smart contract.
 
 [^1]: In this first version of the contract, *Verifiers* are trusted entities designated by the smart contract creator.
 [^2]: This step will become private in future versions of the protocol.
 [^3]: In the next version of the protocol, the client will also add its trap in order to check *verifier*'s loyalty.
 
@@ -61,20 +63,28 @@
 ## Smart Contract Web UI
 
 A web interface showing the smart contract status is available here: [https://dakk.github.io/dqpu/app/](https://dakk.github.io/dqpu/app/)
 
 
 ## Installation
 
-```python setup.py install```
+```pip install dqpu```
+
+Or install the latest development version:
+
+```bash
+git clone https://github.com/dakk/dqpu
+cd dqpu
+python setup.py install
+```
 
 Install IPFS:
 - https://docs.ipfs.tech/install/command-line/#install-official-binary-distributions
 
-## Usage: running a sampling job
+## Usage: simulating a quantum circuit
 
 The workflow described before is hidden to the final user: DQPU can be used seamleassy as any other quantum backend as any other quantum sampler. Currently DQPU implements a **qiskit** wrapper, a low level library for accessing the system primitives and a cli tool.
 
 ### Qiskit example
 
 ```python
 import time
@@ -104,14 +114,15 @@
 counts = job.result().get_counts(circ)
 print(counts)
 ```
 
 ### Low-level example
 
 ```python
+import time
 from dqpu.blockchain import NearBlockchain, IPFSGateway
 from dqpu.backends.base import submit_job, job_status, job_result
 
 # Load account and initialize ipfs
 nb = NearBlockchain('dqpu_alice.testnet')
 ipfs = IPFSGateway()  # noqa: F841
```

### Comparing `dqpu-0.2.1/README.md` & `dqpu-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # dqpu
 
 ![CI Status](https://github.com/dakk/dqpu/actions/workflows/ci.yaml/badge.svg)
 ![Contract CI Status](https://github.com/dakk/dqpu/actions/workflows/ci-contract.yaml/badge.svg)
+![PyPI - Version](https://img.shields.io/pypi/v/dqpu)
 ![License: Apache 2.0](https://img.shields.io/badge/license-Apache_2.0-blue)
+[![Downloads](https://static.pepy.tech/badge/dqpu)](https://pepy.tech/project/dqpu)
 
 A Web3-Powered (Near), Decentralized Quantum Simulator with Verifiable Computation. 
 
 DQPU (Decentralized Quantum Processing Unit) introduces a novel, decentralized approach to quantum computing that leverages the power of blockchain and smart contracts. It addresses the challenges of securely and reliably executing quantum computations in a trustless and transparent manner, while fostering a competitive ecosystem for quantum resource providers.
 
 
 ## Workflow
@@ -20,18 +22,18 @@
 
 The following process outlines how clients can submit quantum circuits for sampling using the DQPU contract:
 
 1. **Client Submits Job**: A *Client* sends a quantum circuit along with a reward to the DQPU smart contract. The circuit data is uploaded to a distributed file storage system like IPFS. The smart contract adds the job to a queue in a 'pending-validation' state with the associated reward.
 
 2. **Verifier Validates Circuit**: A *Verifier*[^1] validates the submitted circuit. This might involve checks for syntax errors or ensuring the circuit is within allowed parameters. The verifier also adds special verification elements (traps) into the circuit and add the new circuit to the contract[^2]. Once validated, the job moves to a 'waiting' state, becomes 'invalid' otherwise.
 
-3. **Simulation or Hardware Execution**: A *Sampler* retrieves a job from the waiting list. It then either simulates the circuit on a software program or executes it on real quantum hardware, depending on the job requirements and available resources. The simulation or execution result is submitted back to the smart contract with a cautional deposit (a percentage of the reward). The job status changes to 'validating'.
+3. **Simulation or Hardware Execution**: A *Sampler* retrieves a job from the waiting list. It then either simulates the circuit on a software program or executes it on real quantum hardware, depending on the job requirements and available resources. The simulation or execution result is submitted back to the smart contract with a security deposit (a percentage of the reward). The job status changes to 'validating'.
 
 4. **Verifier Checks Result**: The same *Verifier* from step 2 examines the returned result. The *Verifier* specifically checks the traps inserted earlier to ensure the result hasn't been tampered with. If the trap verification succeeds, the job status is updated to 'executed' and the trap is disclosed by the *Verifier*. The *Sampler* account receives the reward, while the *Verifier* receives a percentage of this reward.
-If the trap verification fails, the job returns in 'waiting' state (and the *Verifier* receives the cautional deposit of the *Sampler*).
+If the trap verification fails, the job returns in 'waiting' state (and the *Verifier* receives the security deposit of the *Sampler*).
 
 5. **Client Receives Result**: Once the job is marked as 'executed', the *Client* can retrieve the final result from the smart contract.
 
 [^1]: In this first version of the contract, *Verifiers* are trusted entities designated by the smart contract creator.
 [^2]: This step will become private in future versions of the protocol.
 [^3]: In the next version of the protocol, the client will also add its trap in order to check *verifier*'s loyalty.
 
@@ -39,20 +41,28 @@
 ## Smart Contract Web UI
 
 A web interface showing the smart contract status is available here: [https://dakk.github.io/dqpu/app/](https://dakk.github.io/dqpu/app/)
 
 
 ## Installation
 
-```python setup.py install```
+```pip install dqpu```
+
+Or install the latest development version:
+
+```bash
+git clone https://github.com/dakk/dqpu
+cd dqpu
+python setup.py install
+```
 
 Install IPFS:
 - https://docs.ipfs.tech/install/command-line/#install-official-binary-distributions
 
-## Usage: running a sampling job
+## Usage: simulating a quantum circuit
 
 The workflow described before is hidden to the final user: DQPU can be used seamleassy as any other quantum backend as any other quantum sampler. Currently DQPU implements a **qiskit** wrapper, a low level library for accessing the system primitives and a cli tool.
 
 ### Qiskit example
 
 ```python
 import time
@@ -82,14 +92,15 @@
 counts = job.result().get_counts(circ)
 print(counts)
 ```
 
 ### Low-level example
 
 ```python
+import time
 from dqpu.blockchain import NearBlockchain, IPFSGateway
 from dqpu.backends.base import submit_job, job_status, job_result
 
 # Load account and initialize ipfs
 nb = NearBlockchain('dqpu_alice.testnet')
 ipfs = IPFSGateway()  # noqa: F841
```

### Comparing `dqpu-0.2.1/dqpu/__init__.py` & `dqpu-0.2.2/dqpu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `dqpu-0.2.1/dqpu/backends/__init__.py` & `dqpu-0.2.2/dqpu/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/dqpu/backends/base.py` & `dqpu-0.2.2/dqpu/backends/base.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/dqpu/backends/qiskit/__init__.py` & `dqpu-0.2.2/dqpu/backends/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/dqpu/backends/qiskit/dqpubackend.py` & `dqpu-0.2.2/dqpu/backends/qiskit/dqpubackend.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 BASIS_GATES = sorted(
     [
         "x",
         "y",
         "z",
         "h",
         "cx",
+        "cy",
+        "cz",
+        "p",
         # "swap",
         # "cswap",
         # "rx",
         # "ry",
         # "rz",
         # "id",
         # "ccx",
@@ -120,14 +123,15 @@
                 )
         options = {
             "shots": kwargs.get("shots", self.options.shots),
             "reward": kwargs.get("reward", self.options.reward),
         }
 
         qasm_data = qasm2.dumps(circuit)
+
         job_id = submit_job(
             self.near_blockchain,
             self.ipfs_gateway,
             qasm_data,
             circuit.num_qubits,
             circuit.depth(),
             options,
```

### Comparing `dqpu-0.2.1/dqpu/backends/qiskit/dqpujob.py` & `dqpu-0.2.2/dqpu/backends/qiskit/dqpujob.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def _wait_for_result(self, timeout=None, wait=5):
         start_time = time.time()
 
         while True:
             elapsed = time.time() - start_time
             if timeout and elapsed >= timeout:
                 raise JobTimeoutError("Timed out waiting for result")
-            status = job_status(self._backend.near_blockchain, self.job_id)
+            status = self.raw_status()
             if status == "executed":
                 break
             if status == "invalid":
                 raise JobError("Job has been marked as invalid")
             time.sleep(wait)
 
         if self._results is None:
@@ -80,16 +80,19 @@
                 "success": True,
             }
         )
 
     def remove(self):
         return job_remove(self._backend.near_blockchain, self.job_id)
 
+    def raw_status(self):
+        return job_status(self._backend.near_blockchain, self.job_id)
+
     def status(self):
-        status = job_status(self._backend.near_blockchain, self.job_id)
+        status = self.raw_status()
         if status == "executed":
             status = JobStatus.DONE
         elif status == "invalid":
             status = JobStatus.ERROR
         else:
             status = JobStatus.RUNNING
         return status
```

### Comparing `dqpu-0.2.1/dqpu/backends/qiskit/dqpuprovider.py` & `dqpu-0.2.2/dqpu/backends/qiskit/dqpuprovider.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/dqpu/blockchain/__init__.py` & `dqpu-0.2.2/dqpu/blockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/dqpu/blockchain/blockchain.py` & `dqpu-0.2.2/dqpu/blockchain/blockchain.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,7 +20,27 @@
         pass
 
     def connect(self):
         raise Exception("Abstract: blockchain.connect")
 
     def contract_call(self, call_name, params):
         raise Exception("Abstract: blockchain.contract_call")
+
+    def get_number_of_jobs(self) -> int:
+        raise Exception("Abstract: blockchain.get_number_of_jobs")
+
+    def get_jobs(self, from_index, limit):
+        raise Exception("Abstract: blockchain.get_number_of_jobs")
+
+    def get_jobs_paginated(self, from_index=0, to_index=None, limit=50, reverse=False):
+        n = self.get_number_of_jobs() if to_index is None else to_index
+        i = from_index
+        js = []
+
+        while i < n:
+            js += self.get_jobs(from_index=i, limit=50)
+            i += limit
+
+        return js if not reverse else js[::-1]
+
+    def get_all_jobs(self, reverse=False):
+        return self.get_jobs_paginated(reverse=reverse)
```

### Comparing `dqpu-0.2.1/dqpu/blockchain/ipfs_gateway.py` & `dqpu-0.2.2/dqpu/blockchain/ipfs_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
         if response.status_code == 200:
             ipfs_hash = response.text
             return json.loads(ipfs_hash)["Hash"]
         else:
             print(f"Error adding file to IPFS: {response.text}")
 
-    def get(self, ipfs_hash, destination_file=None, timeout=60):
+    def get(self, ipfs_hash, destination_file=None, timeout=10):
         # Set the URL for the IPFS daemon
         url = self.gateway + "/ipfs/"
 
         # Send a GET request to the IPFS daemon with the IPFS hash
         response = requests.get(f"{url}/{ipfs_hash}", timeout=timeout)
 
         # Check if the request was successful
```

### Comparing `dqpu-0.2.1/dqpu/blockchain/near.py` & `dqpu-0.2.2/dqpu/blockchain/near.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import asyncio
 import json
 import os
 from typing import Optional
 
 from py_near.account import Account
+from py_near.exceptions.exceptions import RpcEmptyResponse
 
 from .blockchain import Blockchain
 
 # export type JobStatus = 'pending-validation' | 'waiting' | 'validating-result'
 # | 'executed' | 'invalid';
 
 # class Job:
@@ -46,18 +47,22 @@
     return int(v * 1000000000000000000000000)
 
 
 def from_near(v):
     return int(v) / 1000000000000000000000000.0
 
 
-def asyncio_run_nested(v):
+def asyncio_run_nested(v, n_repeat=5):
     try:
         return asyncio.run(v())
-    except:
+    except RpcEmptyResponse as e:
+        print(e)
+        raise RpcEmptyResponse()
+    except Exception as e:
+        print(e)
         import nest_asyncio
 
         get_ipython()  # type: ignore # noqa: F821
         nest_asyncio.apply()
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(v())
 
@@ -76,35 +81,39 @@
 
     def balance(self):
         async def v():
             return await self.account.get_balance()
 
         return from_near(asyncio.run(v()))
 
+    def create_account(self, name: str, useFaucet: bool = True):
+        pass
+
     def load_account(self, account: str):
         fn = account
         if "/" not in account:
             fn = os.path.expanduser(
                 os.path.join("~", ".near-credentials", self.network, account + ".json")
             )
 
+        if not os.path.exists(fn):
+            raise Exception(f"Unable to load wallet file: {fn}")
+
         with open(fn, "r") as wf:
             w = json.loads(wf.read())
 
             acc = Account(w["account_id"], w["private_key"], self.rpc_addr)
 
             async def v():
                 await acc.startup()
 
             asyncio_run_nested(v)
 
             return acc
 
-        raise Exception("No wallet")
-
     def view(self, view_name: str, params):
         async def v():
             return await self.account.view_function(self.contract, view_name, params)
 
         return asyncio_run_nested(v).result
 
     def call(self, function_name: str, params, amount=0):
@@ -154,16 +163,16 @@
             "set_result_validity", {"id": id, "valid": valid, "trap_file": trap_file}
         )
 
     # Get latest quantum job list
     def get_latest_jobs(self, limit=50):
         return self.view("get_latest_jobs", {"limit": limit})
 
-    def get_jobs(self, index=0, limit=50):
-        return self.view("get_jobs", {"from_index": index, "limit": limit})
+    def get_jobs(self, from_index=0, limit=50):
+        return self.view("get_jobs", {"from_index": from_index, "limit": limit})
 
     # Get a single quantum job by its id
     def get_job(self, id: str):
         return self.view("get_job", {"id": id})
 
     # Get a quantum job status by its id
     def get_job_status(self, id: str):
```

### Comparing `dqpu-0.2.1/dqpu/cli.py` & `dqpu-0.2.2/dqpu/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,16 +163,17 @@
         print("Submitting...")
 
         # Upload job_file
         job_file = ipfs.upload(circuit_file)
         print(f"Circuit file is {job_file}")
 
         shots = random.choice([256, 512, 1024, 2048, 4096, 8192, 16384])
-        sh_fact = int(round((shots + 1024) / 1024))
-        reward = random.randint(1 * nq * sh_fact, 10 * nq * sh_fact) / 30000.0
+        sh_fact = (shots / 16384) * nq
+        reward = random.randint(int(0.5 * sh_fact), int(1.1 * sh_fact)) / 1000.0
+        reward = max(reward, 0.0001)
 
         print(f"Submitting with a reward of {reward:.6f} for {shots} shots")
 
         print(nb.submit_job(nq, dpt, shots, job_file, reward))
         print(f"Account balance is {nb.balance():0.5f} N")
         print(nb.get_latest_jobs()[-1]["id"])
```

### Comparing `dqpu-0.2.1/dqpu/q/__init__.py` & `dqpu-0.2.2/dqpu/q/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/dqpu/q/circuit.py` & `dqpu-0.2.2/dqpu/q/circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import random
 
 import openqasm3
 from openqasm3 import ast as oast
+from openqasm3 import printer
 
 from .gate import Gate
 from .gates import Gates
 
 
 # Abstract class representing a circuit; it doesn't hold a quantum state
 class Measure:
@@ -140,21 +141,23 @@
                     raise Exception("Only one qubit register is allowed")
                 n_q = s.size.value
             elif isinstance(s, oast.ClassicalDeclaration):
                 if n_c is not None:
                     raise Exception("Only one classical register is allowed")
                 n_c = s.type.size.value
             elif isinstance(s, oast.QuantumGate):
+                args = list(map(printer.dumps, s.arguments))
+
                 p = list(map(qubit_to_i, s.qubits))
                 gn = s.name.name.upper()
                 if not hasattr(Gates, gn):
                     raise Exception(f"Unknown gate {gn}")
 
                 g = getattr(Gates, gn)
-                gates.append((g, p))
+                gates.append((g, p, args))
             elif isinstance(s, oast.QuantumMeasurementStatement):
                 end = True
             elif isinstance(s, oast.Include):
                 pass
             else:
                 raise Exception(f"Unhandled {s}")
 
@@ -165,19 +168,25 @@
     def toQasmCircuit(self):
         qasm = "OPENQASM 2.0;\n"
         qasm += 'include "qelib1.inc";\n'
         qasm += "qreg q[" + str(self.n_qbits) + "];\n"
         qasm += "creg c[" + str(self.n_qbits) + "];\n"
 
         for x in self.gates:
-            # TODO: handle parameters
-            a, p = x
+            args = ""
+
+            if len(x) == 2:
+                x = (x[0], x[1], [])
+
+            a, p, ar = x
+            if len(ar) > 0:
+                args = ("(" + (",".join(ar)) + ")").replace(" ", "")
 
             qbs = ", ".join(map(lambda g: "q[" + str(g) + "]", p))
-            qasm += f"{a.iden.lower()} {qbs};\n"
+            qasm += f"{a.iden.lower()}{args} {qbs};\n"
 
         qasm += "measure q -> c;"
 
         return qasm
 
     def toQiskitCircuit(self):  # noqa: C901
         from qiskit import QuantumCircuit
@@ -188,14 +197,16 @@
             a, p = x
 
             if isinstance(a, Gate):
                 if a.iden == "CX":
                     qc.cx(p[0], p[1])
                 elif a.iden == "CZ":
                     qc.cz(p[0], p[1])
+                elif a.iden == "CY":
+                    qc.cy(p[0], p[1])
                 elif a.iden == "SWAP":
                     qc.swap(p[0], p[1])
                 elif a.iden == "X":
                     qc.x(p)
                 elif a.iden == "I":
                     qc.i(p)
                 elif a.iden == "Z":
```

### Comparing `dqpu-0.2.1/dqpu/q/gate.py` & `dqpu-0.2.2/dqpu/q/gate.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/dqpu/q/gates.py` & `dqpu-0.2.2/dqpu/q/gates.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,36 +26,45 @@
 ket_one = np.array([c_zero, c_one])
 
 
 # Standard gates
 
 
 class Gates:
+    P = Gate(
+        "P",
+        lambda k: np.array([[1, 0], [1, math.e ** (complex(0, 1) * k)]]),
+    )
     R = Gate(
         "R",
         lambda k: np.array(
             [[1, 0], [1, math.e ** ((2 * math.pi * complex(0, 1)) / 2**k)]]
         ),
     )
     I = Gate("I", np.array([[1, 0], [0, 1]]))  # noqa: E741
     X = Gate("X", np.array([[0, 1], [1, 0]]))
     Y = Gate("Y", np.array([[0, -1.0j], [+1.0j, 0]]))
     Z = Gate("Z", np.array([[1, 0], [0, -1]]))
     S = Gate("S", np.array([[1, 0], [0, +1.0j]]))
     T = Gate("T", np.array([[1, 0], [0, math.e ** (+1.0j * math.pi / 4)]]))
     H = Gate("H", 1 / np.sqrt(2) * np.array([[1, 1], [1, -1]]))
+    SDG = Gate("SDG", np.array([[1, 0], [0, complex(0, -1)]]))
 
     CR = Gate(
         "CR", lambda k: np.kron(Gates.I.matrix, Gates.R.parametrized(k).matrix), 2
     )
 
     CX = Gate(
         "CX", np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]]), 2
     )
 
+    CY = Gate(
+        "CY", np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, -1], [0, 0, +1.0j, 0]]), 2
+    )
+
     CZ = Gate(
         "CZ", np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, -1]]), 2
     )
 
     SWAP = Gate(
         "SWAP", np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]]), 2
     )
@@ -67,9 +76,11 @@
         I,
         X,
         # Y,
         Z,
         # S,
         # T,
         H,
+        P,
+        SDG,
     ]
-    Gates2 = [CX, CZ, SWAP]
+    Gates2 = [CX, CY, CZ, SWAP]
```

### Comparing `dqpu-0.2.1/dqpu/q/utils.py` & `dqpu-0.2.2/dqpu/q/utils.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/dqpu/sampler/__init__.py` & `dqpu-0.2.2/dqpu/sampler/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .aersimulatorsampler import AerSimulatorSampler  # noqa: F401
+from .qracksimulatorsampler import QrackSimulatorSampler  # noqa: F401
 
 # from .dasksimulatorsampler import DaskSimulatorSampler  # noqa: F401
 from .sampler import Sampler  # noqa: F401
 
 SAMPLERS = {
-    "aersimulator": AerSimulatorSampler
+    "aersimulator": AerSimulatorSampler,
+    "qracksimulator": QrackSimulatorSampler,
 }  # , "dasksimulator": DaskSimulatorSampler}
```

### Comparing `dqpu-0.2.1/dqpu/sampler/aersimulatorsampler.py` & `dqpu-0.2.2/dqpu/sampler/aersimulatorsampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,13 +16,15 @@
 from qiskit_aer import AerSimulator
 
 from .sampler import Sampler
 
 
 class AerSimulatorSampler(Sampler):
     def sample(self, shots):
-        qc = qasm2.loads(self.circuit.decode("ascii"))  # .toQasmCircuit())
+        qc = qasm2.loads(
+            self.circuit, custom_instructions=qasm2.LEGACY_CUSTOM_INSTRUCTIONS
+        )  # .toQasmCircuit())
         simulator = AerSimulator()
         circ = transpile(qc, simulator)
         result = simulator.run(circ, shots=shots).result()
         counts = result.get_counts(circ)
         return counts
```

### Comparing `dqpu-0.2.1/dqpu/sampler/dasksimulatorsampler.py` & `dqpu-0.2.2/dqpu/sampler/dasksimulatorsampler.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/dqpu/verifier/__init__.py` & `dqpu-0.2.2/dqpu/verifier/__init__.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/dqpu/verifier/basictrapper.py` & `dqpu-0.2.2/dqpu/verifier/basictrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,17 +71,17 @@
             qc.n_qbits += 1
             i_r = random.randint(0, qc.n_qbits - 1)
 
             def remap_qbit(q_idx):
                 return q_idx + 1 if q_idx >= i_r else q_idx
 
             def remap_gate(gq):
-                a, p = gq
+                a, p, args = gq
                 p = list(map(remap_qbit, p))
-                return (a, p)
+                return (a, p, args)
 
             def remap_trap(t):
                 t.qubit = remap_qbit(t.qubit)
                 return t
 
             gates = list(map(remap_gate, gates))
             traps = list(map(remap_trap, traps))
```

### Comparing `dqpu-0.2.1/dqpu/verifier/trapper.py` & `dqpu-0.2.2/dqpu/verifier/trapper.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/dqpu/verifier/verifier.py` & `dqpu-0.2.2/dqpu/verifier/verifier.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/dqpu/verifiernode.py` & `dqpu-0.2.2/dqpu/verifiernode.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,151 +12,185 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import pickle
 import random
 import time
+import traceback
 
 from requests.exceptions import ReadTimeout
 
 from .blockchain import IPFSGateway, NearBlockchain
 from .cli import default_parser
 from .q import Circuit
-from .utils import create_dqpu_dirs
+from .utils import create_dqpu_dirs, repeat_until_done
 from .verifier import BasicTrapper  # BasicTrapInfo,
 
 
+def handle_pending_validation_job(j, ipfs, nb, base_dir):
+    print(f"Processing pending-validation job {j['id']} from {j['owner_id']}")
+
+    try:
+        jf = ipfs.get(j["job_file"], timeout=10)
+    except ReadTimeout:  # TODO: move on ipfs.get raising a new exception
+        print(f"\tTimeout getting file {j['job_file']}, skipping for now")
+        return False
+
+    # Parse the file using q.Circuit.fromQasm
+    try:
+        qc = Circuit.fromQasmCircuit(jf.decode("ascii"))
+    except Exception as e:
+        print("\t", "Failed to parse", j["id"], e)
+        nb.set_job_validity(j["id"], False)
+        return True
+
+    # Add a trap
+    trapper = BasicTrapper()
+    (qc2, trap_list) = trapper.trap(qc)
+
+    # Save trap info to a file
+    with open(f"{base_dir}/{j['id']}_qc_traps.pickle", "wb") as outp:
+        pickle.dump(trap_list, outp, pickle.HIGHEST_PROTOCOL)
+
+    # Save qasm to file
+    trapped_qasm_file = f"{base_dir}/{j['id']}_qc_trapped.qasm"
+
+    with open(trapped_qasm_file, "w") as f:
+        f.write(qc2.toQasmCircuit())
+
+    # Upload the file
+    jf_trapped = ipfs.upload(trapped_qasm_file)
+    print("\tTrapped file uploaded", jf_trapped)
+
+    # Send the set_validity
+    print("\t", nb.set_job_validity(j["id"], True, jf_trapped))
+    return True
+
+
+def handle_validating_result_job(j, ipfs, nb, base_dir):  # noqa: C901
+    print(
+        f"Processing validating-result job {j['id']} from {j['owner_id']} "
+        + f"sampled by {j['sampler_id']}"
+    )
+
+    # Get the result data
+    try:
+        rf = ipfs.get(j["result_file"], timeout=10)
+    except ReadTimeout:  # TODO: move on ipfs.get raising a new exception
+        print(f"\tTimeout getting file {j['result_file']}, skipping for now")
+        return False
+
+    try:
+        counts = json.loads(rf)
+    except:
+        print("\tInvalid result data")
+        print(nb.set_result_validity(j["id"], False))
+        return True
+
+    # Check if shots match
+    ctot = sum(counts.values())
+    if j["shots"] > ctot:
+        print("\t", "Invalid number of shots")
+        print(nb.set_result_validity(j["id"], False))
+        return True
+
+    # Load the trap from file
+    trap_fp = f"{base_dir}/{j['id']}_qc_traps.pickle"
+    try:
+        with open(trap_fp, "rb") as inp:
+            trap_list = pickle.load(inp)
+    except:
+        print(f'Unable to load {trap_fp}, skipping job {j["id"]}')
+        return False
+
+    # Check trap validity
+    try:
+        trapper = BasicTrapper()
+        validity = trapper.verify(trap_list, counts)
+    except Exception as e:
+        print("Got exception while verifying, contact dakk")
+        print(e)
+        return False
+
+    # Send the set_result_validity
+    if validity:
+        trap_j = list(map(lambda t: t.dump(), trap_list))
+        trap_file = f"{base_dir}/{j['id']}_traps.json"
+
+        with open(trap_file, "w") as inp:
+            inp.write(json.dumps(trap_j))
+
+        trap_file_i = ipfs.upload(trap_file)
+
+        print("\t", nb.set_result_validity(j["id"], True, trap_file_i))
+    else:
+        print("\t", nb.set_result_validity(j["id"], False))
+
+    return True
+
+
 def verifier_node():  # noqa: C901
     parser = default_parser()
     args = parser.parse_args()  # noqa: F841
 
     base_dir = create_dqpu_dirs()
 
     nb = NearBlockchain(args.account, args.network)
     ipfs = IPFSGateway(gateway="http://" + args.ipfs_gateway)  # noqa: F841
 
     # Start contract polling for new jobs
     running = True
-    current_limit = 256
+    first_run = True
     n_vresult = 0
     n_verified = 0
 
     print("Verifier node started.")
+    stats = repeat_until_done(lambda: nb.get_jobs_stats())
 
     while running:
-        latest_jobs = nb.get_latest_jobs(limit=current_limit)
+        if first_run:
+            first_run = False
+            latest_jobs = repeat_until_done(lambda: nb.get_all_jobs())
+        else:
+            i = 0
+            while (
+                repeat_until_done(lambda: nb.get_jobs_stats())["validating-result"]
+                == stats["validating-result"]
+                and repeat_until_done(lambda: nb.get_jobs_stats())["pending-validation"]
+                == stats["pending-validation"]
+            ) and i < 5:
+                time.sleep(random.randint(0, 5))
+                i += 1
+
+            latest_jobs = repeat_until_done(lambda: nb.get_latest_jobs())
+
+        stats = repeat_until_done(lambda: nb.get_jobs_stats())
+        random.shuffle(latest_jobs)
 
         # If there is a new job that needs validation, process it
         for j in latest_jobs:
             if j["status"] == "pending-validation":
-                print(
-                    f"Processing pending-validation job {j['id']} from {j['owner_id']}"
-                )
-
-                try:
-                    jf = ipfs.get(j["job_file"], timeout=120)
-                except ReadTimeout:  # TODO: move on ipfs.get raising a new exception
-                    print(f"\tTimeout getting file {j['job_file']}, skipping for now")
-                    continue
-
-                # Parse the file using q.Circuit.fromQasm
-                try:
-                    qc = Circuit.fromQasmCircuit(jf.decode("ascii"))
-                except Exception as e:
-                    print("\t", "Failed to parse", j["id"], e)
-                    nb.set_job_validity(j["id"], False)
-                    continue
-
-                # Add a trap
-                trapper = BasicTrapper()
-                (qc2, trap_list) = trapper.trap(qc)
-
-                # Save trap info to a file
-                with open(f"{base_dir}/{j['id']}_qc_traps.pickle", "wb") as outp:
-                    pickle.dump(trap_list, outp, pickle.HIGHEST_PROTOCOL)
-
-                # Save qasm to file
-                trapped_qasm_file = f"{base_dir}/{j['id']}_qc_trapped.qasm"
-
-                with open(trapped_qasm_file, "w") as f:
-                    f.write(qc2.toQasmCircuit())
-
-                # Upload the file
-                jf_trapped = ipfs.upload(trapped_qasm_file)
-                print("\t", "Trapped file uploaded", jf_trapped)
-
-                # Send the set_validity
                 try:
-                    print("\t", nb.set_job_validity(j["id"], True, jf_trapped))
-                    n_verified += 1
+                    if handle_pending_validation_job(j, ipfs, nb, base_dir):
+                        n_verified += 1
+                        stats["pending-validation"] -= 1
                 except Exception as e:
-                    print("\tFailed to set", e)
+                    print("\tFailed to handle pending-validation job:", e)
+                    traceback.print_exc()
 
             elif (
                 j["status"] == "validating-result"
                 and j["verifier_id"] == nb.account.account_id
             ):
-                print(
-                    f"Processing validating-result job {j['id']} from {j['owner_id']} "
-                    + f"sampled by {j['sampler_id']}"
-                )
-
-                # Get the result data
-                try:
-                    rf = ipfs.get(j["result_file"], timeout=120)
-                except ReadTimeout:  # TODO: move on ipfs.get raising a new exception
-                    print(
-                        f"\tTimeout getting file {j['result_file']}, skipping for now"
-                    )
-                    continue
-
-                try:
-                    counts = json.loads(rf)
-                except:
-                    print("\t", "Invalid result data")
-                    continue
-
-                # Check if shots match
-                ctot = sum(counts.values())
-                if j["shots"] > ctot:
-                    print("\t", "Invalid number of shots")
-                    print(nb.set_result_validity(j["id"], False))
-                    continue
-
-                # Load the trap from file
-                trap_fp = f"{base_dir}/{j['id']}_qc_traps.pickle"
-                try:
-                    with open(trap_fp, "rb") as inp:
-                        trap_list = pickle.load(inp)
-                except:
-                    print(f'Unable to load {trap_fp}, skipping job {j["id"]}')
-                    continue
-
-                # Check trap validity
-                trapper = BasicTrapper()
-                validity = trapper.verify(trap_list, counts)
-
-                # Send the set_result_validity
                 try:
-                    if validity:
-                        trap_j = list(map(lambda t: t.dump(), trap_list))
-                        trap_file = f"{base_dir}/{j['id']}_traps.json"
-
-                        with open(trap_file, "w") as inp:
-                            inp.write(json.dumps(trap_j))
-
-                        trap_file_i = ipfs.upload(trap_file)
-
-                        print("\t", nb.set_result_validity(j["id"], True, trap_file_i))
-                    else:
-                        print("\t", nb.set_result_validity(j["id"], False))
-                    n_vresult += 1
+                    if handle_validating_result_job(j, ipfs, nb, base_dir):
+                        n_vresult += 1
+                        stats["validating-result"] -= 1
                 except Exception as e:
-                    print("\tFailed to set", e)
+                    print("\tFailed to handle validating-result job:", e)
+                    traceback.print_exc()
 
-        current_limit = 48
         print(
             f"Account balance is {nb.balance():0.5f} N, job verified {n_verified}, "
             + f"result verified {n_vresult}"
         )
-        time.sleep(random.randint(0, 60))
```

### Comparing `dqpu-0.2.1/dqpu.egg-info/PKG-INFO` & `dqpu-0.2.2/dqpu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqpu
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/dakk/dqpu
 Author: Davide Gessa
 Author-email: gessadavide@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dakk/dqpu/issues/
 Project-URL: Documentation, https://dakk.github.io/dqpu
 Project-URL: Source, https://github.com/dakk/dqpu
@@ -20,15 +20,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dqpu
 
 ![CI Status](https://github.com/dakk/dqpu/actions/workflows/ci.yaml/badge.svg)
 ![Contract CI Status](https://github.com/dakk/dqpu/actions/workflows/ci-contract.yaml/badge.svg)
+![PyPI - Version](https://img.shields.io/pypi/v/dqpu)
 ![License: Apache 2.0](https://img.shields.io/badge/license-Apache_2.0-blue)
+[![Downloads](https://static.pepy.tech/badge/dqpu)](https://pepy.tech/project/dqpu)
 
 A Web3-Powered (Near), Decentralized Quantum Simulator with Verifiable Computation. 
 
 DQPU (Decentralized Quantum Processing Unit) introduces a novel, decentralized approach to quantum computing that leverages the power of blockchain and smart contracts. It addresses the challenges of securely and reliably executing quantum computations in a trustless and transparent manner, while fostering a competitive ecosystem for quantum resource providers.
 
 
 ## Workflow
@@ -42,18 +44,18 @@
 
 The following process outlines how clients can submit quantum circuits for sampling using the DQPU contract:
 
 1. **Client Submits Job**: A *Client* sends a quantum circuit along with a reward to the DQPU smart contract. The circuit data is uploaded to a distributed file storage system like IPFS. The smart contract adds the job to a queue in a 'pending-validation' state with the associated reward.
 
 2. **Verifier Validates Circuit**: A *Verifier*[^1] validates the submitted circuit. This might involve checks for syntax errors or ensuring the circuit is within allowed parameters. The verifier also adds special verification elements (traps) into the circuit and add the new circuit to the contract[^2]. Once validated, the job moves to a 'waiting' state, becomes 'invalid' otherwise.
 
-3. **Simulation or Hardware Execution**: A *Sampler* retrieves a job from the waiting list. It then either simulates the circuit on a software program or executes it on real quantum hardware, depending on the job requirements and available resources. The simulation or execution result is submitted back to the smart contract with a cautional deposit (a percentage of the reward). The job status changes to 'validating'.
+3. **Simulation or Hardware Execution**: A *Sampler* retrieves a job from the waiting list. It then either simulates the circuit on a software program or executes it on real quantum hardware, depending on the job requirements and available resources. The simulation or execution result is submitted back to the smart contract with a security deposit (a percentage of the reward). The job status changes to 'validating'.
 
 4. **Verifier Checks Result**: The same *Verifier* from step 2 examines the returned result. The *Verifier* specifically checks the traps inserted earlier to ensure the result hasn't been tampered with. If the trap verification succeeds, the job status is updated to 'executed' and the trap is disclosed by the *Verifier*. The *Sampler* account receives the reward, while the *Verifier* receives a percentage of this reward.
-If the trap verification fails, the job returns in 'waiting' state (and the *Verifier* receives the cautional deposit of the *Sampler*).
+If the trap verification fails, the job returns in 'waiting' state (and the *Verifier* receives the security deposit of the *Sampler*).
 
 5. **Client Receives Result**: Once the job is marked as 'executed', the *Client* can retrieve the final result from the smart contract.
 
 [^1]: In this first version of the contract, *Verifiers* are trusted entities designated by the smart contract creator.
 [^2]: This step will become private in future versions of the protocol.
 [^3]: In the next version of the protocol, the client will also add its trap in order to check *verifier*'s loyalty.
 
@@ -61,20 +63,28 @@
 ## Smart Contract Web UI
 
 A web interface showing the smart contract status is available here: [https://dakk.github.io/dqpu/app/](https://dakk.github.io/dqpu/app/)
 
 
 ## Installation
 
-```python setup.py install```
+```pip install dqpu```
+
+Or install the latest development version:
+
+```bash
+git clone https://github.com/dakk/dqpu
+cd dqpu
+python setup.py install
+```
 
 Install IPFS:
 - https://docs.ipfs.tech/install/command-line/#install-official-binary-distributions
 
-## Usage: running a sampling job
+## Usage: simulating a quantum circuit
 
 The workflow described before is hidden to the final user: DQPU can be used seamleassy as any other quantum backend as any other quantum sampler. Currently DQPU implements a **qiskit** wrapper, a low level library for accessing the system primitives and a cli tool.
 
 ### Qiskit example
 
 ```python
 import time
@@ -104,14 +114,15 @@
 counts = job.result().get_counts(circ)
 print(counts)
 ```
 
 ### Low-level example
 
 ```python
+import time
 from dqpu.blockchain import NearBlockchain, IPFSGateway
 from dqpu.backends.base import submit_job, job_status, job_result
 
 # Load account and initialize ipfs
 nb = NearBlockchain('dqpu_alice.testnet')
 ipfs = IPFSGateway()  # noqa: F841
```

### Comparing `dqpu-0.2.1/dqpu.egg-info/SOURCES.txt` & `dqpu-0.2.2/dqpu.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -28,13 +28,14 @@
 dqpu/q/circuit.py
 dqpu/q/gate.py
 dqpu/q/gates.py
 dqpu/q/utils.py
 dqpu/sampler/__init__.py
 dqpu/sampler/aersimulatorsampler.py
 dqpu/sampler/dasksimulatorsampler.py
+dqpu/sampler/qracksimulatorsampler.py
 dqpu/sampler/sampler.py
 dqpu/verifier/__init__.py
 dqpu/verifier/basictrapper.py
 dqpu/verifier/trapper.py
 dqpu/verifier/verifier.py
 test/test_empty.py
```

### Comparing `dqpu-0.2.1/setup.py` & `dqpu-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `dqpu-0.2.1/test/test_empty.py` & `dqpu-0.2.2/test/test_empty.py`

 * *Files identical despite different names*

