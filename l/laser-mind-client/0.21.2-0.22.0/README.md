# Comparing `tmp/laser_mind_client-0.21.2.tar.gz` & `tmp/laser_mind_client-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laser_mind_client-0.21.2.tar", last modified: Thu May 23 09:42:19 2024, max compression
+gzip compressed data, was "laser_mind_client-0.22.0.tar", last modified: Thu May 23 10:47:47 2024, max compression
```

## Comparing `laser_mind_client-0.21.2.tar` & `laser_mind_client-0.22.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 09:42:19.912034 laser_mind_client-0.21.2/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 09:36:06.000000 laser_mind_client-0.21.2/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2024-05-23 09:42:19.908034 laser_mind_client-0.21.2/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8152 2024-05-23 09:36:06.000000 laser_mind_client-0.21.2/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 09:42:19.908034 laser_mind_client-0.21.2/laser_mind_client/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-23 09:36:06.000000 laser_mind_client-0.21.2/laser_mind_client/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7918 2024-05-23 09:36:06.000000 laser_mind_client-0.21.2/laser_mind_client/laser_mind_client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 09:42:19.908034 laser_mind_client-0.21.2/laser_mind_client.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2024-05-23 09:42:19.000000 laser_mind_client-0.21.2/laser_mind_client.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      305 2024-05-23 09:42:19.000000 laser_mind_client-0.21.2/laser_mind_client.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 09:42:19.000000 laser_mind_client-0.21.2/laser_mind_client.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-05-23 09:42:19.000000 laser_mind_client-0.21.2/laser_mind_client.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-23 09:42:19.000000 laser_mind_client-0.21.2/laser_mind_client.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      722 2024-05-23 09:42:13.000000 laser_mind_client-0.21.2/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 09:42:19.912034 laser_mind_client-0.21.2/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:47:47.107981 laser_mind_client-0.22.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8914 2024-05-23 10:47:47.103981 laser_mind_client-0.22.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8294 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:47:47.103981 laser_mind_client-0.22.0/laser_mind_client/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/laser_mind_client/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8587 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/laser_mind_client/laser_mind_client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:47:47.103981 laser_mind_client-0.22.0/laser_mind_client.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8914 2024-05-23 10:47:47.000000 laser_mind_client-0.22.0/laser_mind_client.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      415 2024-05-23 10:47:47.000000 laser_mind_client-0.22.0/laser_mind_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 10:47:47.000000 laser_mind_client-0.22.0/laser_mind_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-05-23 10:47:47.000000 laser_mind_client-0.22.0/laser_mind_client.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-23 10:47:47.000000 laser_mind_client-0.22.0/laser_mind_client.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      722 2024-05-23 10:47:40.000000 laser_mind_client-0.22.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 10:47:47.107981 laser_mind_client-0.22.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 10:47:47.103981 laser_mind_client-0.22.0/tests/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      453 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/tests/test_solve_qubo_adjacency_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      529 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/tests/test_solve_qubo_matrix.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      992 2024-05-23 10:46:36.000000 laser_mind_client-0.22.0/tests/test_solve_qubo_matrix_async.py
```

### Comparing `laser_mind_client-0.21.2/LICENSE` & `laser_mind_client-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laser_mind_client-0.21.2/PKG-INFO` & `laser_mind_client-0.22.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laser-mind-client
-Version: 0.21.2
+Version: 0.22.0
 Summary: A client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -20,15 +20,15 @@
 The LightSolver Platform Client is a Python package designed to interface with the LightSolver Cloud to facilitate solving Quadratic Unconstrained Binary Optimization (QUBO) problems.
 
 This package is designated for internal access to features during the development process, as well as serves as a prototype for future versions of the production LightSolver Platform Client.
 
 ## Features
 - **QUBO Problem Solving:** The `solve_qubo` function accepts a QUBO problem, represented either as a 2D array (matrix) or an adjacency list, and returns the solution.
 - **Synchronous and Asynchronous Operation:** Users can choose between blocking (synchronous) and non-blocking (asynchronous) modes for QUBO problem solving.
-- **Flexible Installation:** Compatible with both Windows and Ubuntu systems.
+- **Flexible Installation:** Compatible with both Windows and MacOS systems.
 
 ### Solve QUBO
 The `solve_qubo` function handles the computation of QUBO problems, either represented by a 2D array (matrix) or by an adjacency list. For code samples, see the **Usage** section.
 
 #### Input Matrix Validity
 - The matrix must be square.
 - The matrix supports int or float cell values.
@@ -46,23 +46,26 @@
 ### Synchronous and Asynchronous Usage
 - **Synchronous Mode (Default):** The `waitForSolution` flag is set to **True** by default. The function blocks operations until a result is received.
 - **Asynchronous Mode:** Set `waitForSolution` to **False**. The function returns immediately with a token object, allowing the script to continue while the server processes the QUBO problem.
 
 ## Setting Up
 
 ### Prerequisites
-- Valid credentials for connecting to the LightSolver Cloud.
-- LightSolver Client code project - please use this link to download.
-- Python 3.10.
-- Operating System: Linux or Windows. Tested on Ubuntu 20.04 and Windows 11.
+- Operating System: MacOS or Windows 11.
+- Valid credentials for connecting to the LightSolver Cloud ([Registration](https://id.lightsolver.com/signin/register)).
+- LightSolver Client code project (provided separately).
+    - Verify installation of software for unzipping the LightSolver Client.
+- Python 3.10 or higher ([Download Here](https://www.python.org/downloads/release/python-31011/)).
+    - Select the appropriate MacOS/Windows version at the bottom.
+    - Note: for Windows installation, switch on the "Add to Path" option in the wizard.
 - Highly Recommended: Use a virtual environment before installing laser-mind-client (Please see detailed action further below under the relevant OS).
 
 ### Installation
-Complete the installation on Windows or Ubuntu as described below.
-For further assistance  with setup or connection issues, contact support@lightsolver.com.
+Complete the installation on Windows or MacOS as described below.
+For further assistance with setup or connection issues, contact support@lightsolver.com.
 
 #### Windows
 1. Press the windows key, type "cmd", right click on the result and select "Run as administrator".
 2. Navigate to the root folder where you unzipped and plan to use the LightSolver Client:
     ```
     cd <your project folder>
     ```
@@ -89,26 +92,22 @@
 ```
 
 7. (Recommended) Test LightSolver credentials
     Run the following command:
 ```sh
     python test_env.py
 ```
-    if test credentials failed , please  reinstall credentials using following commands:
-    - Exit virtual environment , by running :
+8. (Recommended) Test - using the inline project test examples
+   Run the following command:
 ```sh
-    deactivate
-```
-    - Run the following command:
-```sh
-    python setup_env.py
+    python ./tests/test_solve_qubo_matrix.py
 ```
 
 
-#### Ubuntu
+#### MacOS
 1. Open new terminal window
 2. Navigate to the root folder where you unzipped and plan to use the LightSolver Client:
     ```
     cd <your project folder>
     ```
 
 3. (Recommended) Set the LightSolver credentials using environment variables (will remove the need to provide credentials for every usage).
@@ -135,25 +134,22 @@
 ```
 
 7. (Recommended) Test LightSolver credentials
     Run the following command:
 ```sh
     python3 test_env.py
 ```
-    if test credentials failed , please  reinstall credentials using following commands:
-    - Exit virtual environment , by running :
-```sh
-    deactivate
-```
-    - Run the following command:
+
+8. (Recommended) Test - using the inline project test examples
+   Run the following command:
 ```sh
-    python3 setup_env.py
-    source ~/.bash_profile
+    python3 ./tests/test_solve_qubo_matrix.py
 ```
 
+***
 ## Authentication
 Initialization of the `LaserMind` class automatically forms a secure and authenticated connection with the LightSolver Cloud.
 Subsequent calls by the same user are similarly secure and authenticated.
 
 ## Usage
 To begin solving any QUBO problem:
 1. Create an instance of the ```LaserMind``` class. This class represents the client that requests solutions from the LightSolver Cloud.
@@ -207,15 +203,15 @@
 
 res = lsClient.solve_qubo(edgeList=quboListData, timeout=1)
 
 print(res)
 ```
 
 ### Solve QUBO Matrix using Asynchronous Flow
-This example demonstratse how to solve a QUBO problem asynchronously using the LightSolver Platform Client.
+This example demonstrates how to solve a QUBO problem asynchronously using the LightSolver Platform Client.
 Begin by creating a matrix to represent your QUBO problem.
 The `solve_qubo` function is used with the following parameters:
    - `matrixData`: A 2D array representing the QUBO problem.
    - `timeout`: The desired time limit for the calculation in seconds.
    - `waitForSolution`: A boolean flag set to `False` to indicate non-blocking mode.
 
 ```python
```

### Comparing `laser_mind_client-0.21.2/README.md` & `laser_mind_client-0.22.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 The LightSolver Platform Client is a Python package designed to interface with the LightSolver Cloud to facilitate solving Quadratic Unconstrained Binary Optimization (QUBO) problems.
 
 This package is designated for internal access to features during the development process, as well as serves as a prototype for future versions of the production LightSolver Platform Client.
 
 ## Features
 - **QUBO Problem Solving:** The `solve_qubo` function accepts a QUBO problem, represented either as a 2D array (matrix) or an adjacency list, and returns the solution.
 - **Synchronous and Asynchronous Operation:** Users can choose between blocking (synchronous) and non-blocking (asynchronous) modes for QUBO problem solving.
-- **Flexible Installation:** Compatible with both Windows and Ubuntu systems.
+- **Flexible Installation:** Compatible with both Windows and MacOS systems.
 
 ### Solve QUBO
 The `solve_qubo` function handles the computation of QUBO problems, either represented by a 2D array (matrix) or by an adjacency list. For code samples, see the **Usage** section.
 
 #### Input Matrix Validity
 - The matrix must be square.
 - The matrix supports int or float cell values.
@@ -29,23 +29,26 @@
 ### Synchronous and Asynchronous Usage
 - **Synchronous Mode (Default):** The `waitForSolution` flag is set to **True** by default. The function blocks operations until a result is received.
 - **Asynchronous Mode:** Set `waitForSolution` to **False**. The function returns immediately with a token object, allowing the script to continue while the server processes the QUBO problem.
 
 ## Setting Up
 
 ### Prerequisites
-- Valid credentials for connecting to the LightSolver Cloud.
-- LightSolver Client code project - please use this link to download.
-- Python 3.10.
-- Operating System: Linux or Windows. Tested on Ubuntu 20.04 and Windows 11.
+- Operating System: MacOS or Windows 11.
+- Valid credentials for connecting to the LightSolver Cloud ([Registration](https://id.lightsolver.com/signin/register)).
+- LightSolver Client code project (provided separately).
+    - Verify installation of software for unzipping the LightSolver Client.
+- Python 3.10 or higher ([Download Here](https://www.python.org/downloads/release/python-31011/)).
+    - Select the appropriate MacOS/Windows version at the bottom.
+    - Note: for Windows installation, switch on the "Add to Path" option in the wizard.
 - Highly Recommended: Use a virtual environment before installing laser-mind-client (Please see detailed action further below under the relevant OS).
 
 ### Installation
-Complete the installation on Windows or Ubuntu as described below.
-For further assistance  with setup or connection issues, contact support@lightsolver.com.
+Complete the installation on Windows or MacOS as described below.
+For further assistance with setup or connection issues, contact support@lightsolver.com.
 
 #### Windows
 1. Press the windows key, type "cmd", right click on the result and select "Run as administrator".
 2. Navigate to the root folder where you unzipped and plan to use the LightSolver Client:
     ```
     cd <your project folder>
     ```
@@ -72,26 +75,22 @@
 ```
 
 7. (Recommended) Test LightSolver credentials
     Run the following command:
 ```sh
     python test_env.py
 ```
-    if test credentials failed , please  reinstall credentials using following commands:
-    - Exit virtual environment , by running :
+8. (Recommended) Test - using the inline project test examples
+   Run the following command:
 ```sh
-    deactivate
-```
-    - Run the following command:
-```sh
-    python setup_env.py
+    python ./tests/test_solve_qubo_matrix.py
 ```
 
 
-#### Ubuntu
+#### MacOS
 1. Open new terminal window
 2. Navigate to the root folder where you unzipped and plan to use the LightSolver Client:
     ```
     cd <your project folder>
     ```
 
 3. (Recommended) Set the LightSolver credentials using environment variables (will remove the need to provide credentials for every usage).
@@ -118,25 +117,22 @@
 ```
 
 7. (Recommended) Test LightSolver credentials
     Run the following command:
 ```sh
     python3 test_env.py
 ```
-    if test credentials failed , please  reinstall credentials using following commands:
-    - Exit virtual environment , by running :
-```sh
-    deactivate
-```
-    - Run the following command:
+
+8. (Recommended) Test - using the inline project test examples
+   Run the following command:
 ```sh
-    python3 setup_env.py
-    source ~/.bash_profile
+    python3 ./tests/test_solve_qubo_matrix.py
 ```
 
+***
 ## Authentication
 Initialization of the `LaserMind` class automatically forms a secure and authenticated connection with the LightSolver Cloud.
 Subsequent calls by the same user are similarly secure and authenticated.
 
 ## Usage
 To begin solving any QUBO problem:
 1. Create an instance of the ```LaserMind``` class. This class represents the client that requests solutions from the LightSolver Cloud.
@@ -190,15 +186,15 @@
 
 res = lsClient.solve_qubo(edgeList=quboListData, timeout=1)
 
 print(res)
 ```
 
 ### Solve QUBO Matrix using Asynchronous Flow
-This example demonstratse how to solve a QUBO problem asynchronously using the LightSolver Platform Client.
+This example demonstrates how to solve a QUBO problem asynchronously using the LightSolver Platform Client.
 Begin by creating a matrix to represent your QUBO problem.
 The `solve_qubo` function is used with the following parameters:
    - `matrixData`: A 2D array representing the QUBO problem.
    - `timeout`: The desired time limit for the calculation in seconds.
    - `waitForSolution`: A boolean flag set to `False` to indicate non-blocking mode.
 
 ```python
```

### Comparing `laser_mind_client-0.21.2/laser_mind_client/laser_mind_client.py` & `laser_mind_client-0.22.0/laser_mind_client/laser_mind_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import logging
 import time
 import numpy
+import requests
 
 from ls_api_clients import LSAPIClient
 from ls_packers import float_array_as_int
 from ls_packers import numpy_array_to_triu_flat
 from laser_mind_client_meta import MessageKeys
 
 logging.basicConfig(
@@ -40,19 +41,23 @@
             else:
                 raise Exception("the 'username' parameter cannot be None if the LS_USER environment variable is not set.")
         if password == None:
             if 'LS_PASS' in os.environ:
                 password = os.environ['LS_PASS']
             else:
                 raise Exception("the 'password' parameter cannot be None if the LS_PASS environment variable is not set.")
-
-        self.states_per_call = states_per_call
-        logging.info('LightSolver connection init started')
-        self.apiClient = LSAPIClient(username, password)
-        logging.info('LightSolver connection init finished')
+        try:
+            self.states_per_call = states_per_call
+            logging.info('LightSolver connection init started')
+            self.apiClient = LSAPIClient(username, password)
+            logging.info('LightSolver connection init finished')
+        except requests.exceptions.ConnectionError as e:
+            raise Exception("!!!!! No access to LightSolver Cloud. !!!!!")
+        except Exception as e:
+                raise  e
 
     def get_solution_by_id(self, solutionId, timestamp):
         """
         Retrieve a previously requested solution from the LightSolver cloud.
 
         - `solutionId` : the solution id received when requesting a solution.
         - `timestamp` : the timestamp received when requesting a solution.
@@ -125,18 +130,23 @@
         - `inputPath` : (optional) The the path to a pre-uploaded input file if not given a random string is used returned.
 
         Returns a dictionary with the 'data' key being a dictionary representing the solution using the following keys:
         - `iid` : The id of the uploaded file.
         - `varCount` : The amount number of variables of the problem.
 
         """
-        commandInput, varCount = self.make_command_input(matrixData, edgeList, timeout)
+        try:
+            commandInput, varCount = self.make_command_input(matrixData, edgeList, timeout)
 
-        iid = self.apiClient.upload_command_input(commandInput, inputPath)
-        return iid, varCount
+            iid = self.apiClient.upload_command_input(commandInput, inputPath)
+            return iid, varCount
+        except requests.exceptions.ConnectionError as e:
+            raise Exception("!!!!! No access to LightSolver Cloud. !!!!!")
+        except Exception as e:
+                raise  e
 
     def solve_qubo(self, matrixData = None, edgeList = None, inputPath = None, timeout = 10, waitForSolution = True):
         """
         Solves a qubo problem using the optimized algorithm.
 
         - `matrixData` : (optional) The matrix data of the target problem, must be a symmetric matrix. if given, the edge list in the vortex parameters is ignored.
         - `edgeList` : (optional) The edge list describing Ising matrix of the target problem. if the matrixData parameter is given, this parameter is ignored.
@@ -156,15 +166,19 @@
             varCount = 10000
 
         requestInput = {
             MessageKeys.QUBO_INPUT_PATH : iid,
             MessageKeys.ALGO_RUN_TIMEOUT : timeout,
             MessageKeys.VAR_COUNT_KEY : varCount
             }
-
-        response = self.apiClient.SendCommandRequest(command_name, requestInput)
-        logging.info(f"got response {response}")
-        if not waitForSolution:
-            return response
-        result = self.get_solution_sync(response)
-        return result
+        try:
+            response = self.apiClient.SendCommandRequest(command_name, requestInput)
+            logging.info(f"got response {response}")
+            if not waitForSolution:
+                return response
+            result = self.get_solution_sync(response)
+            return result
+        except requests.exceptions.ConnectionError as e:
+            raise Exception("!!!!! No access to LightSolver Cloud. !!!!!")
+        except Exception as e:
+                raise  e
```

### Comparing `laser_mind_client-0.21.2/laser_mind_client.egg-info/PKG-INFO` & `laser_mind_client-0.22.0/laser_mind_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laser-mind-client
-Version: 0.21.2
+Version: 0.22.0
 Summary: A client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -20,15 +20,15 @@
 The LightSolver Platform Client is a Python package designed to interface with the LightSolver Cloud to facilitate solving Quadratic Unconstrained Binary Optimization (QUBO) problems.
 
 This package is designated for internal access to features during the development process, as well as serves as a prototype for future versions of the production LightSolver Platform Client.
 
 ## Features
 - **QUBO Problem Solving:** The `solve_qubo` function accepts a QUBO problem, represented either as a 2D array (matrix) or an adjacency list, and returns the solution.
 - **Synchronous and Asynchronous Operation:** Users can choose between blocking (synchronous) and non-blocking (asynchronous) modes for QUBO problem solving.
-- **Flexible Installation:** Compatible with both Windows and Ubuntu systems.
+- **Flexible Installation:** Compatible with both Windows and MacOS systems.
 
 ### Solve QUBO
 The `solve_qubo` function handles the computation of QUBO problems, either represented by a 2D array (matrix) or by an adjacency list. For code samples, see the **Usage** section.
 
 #### Input Matrix Validity
 - The matrix must be square.
 - The matrix supports int or float cell values.
@@ -46,23 +46,26 @@
 ### Synchronous and Asynchronous Usage
 - **Synchronous Mode (Default):** The `waitForSolution` flag is set to **True** by default. The function blocks operations until a result is received.
 - **Asynchronous Mode:** Set `waitForSolution` to **False**. The function returns immediately with a token object, allowing the script to continue while the server processes the QUBO problem.
 
 ## Setting Up
 
 ### Prerequisites
-- Valid credentials for connecting to the LightSolver Cloud.
-- LightSolver Client code project - please use this link to download.
-- Python 3.10.
-- Operating System: Linux or Windows. Tested on Ubuntu 20.04 and Windows 11.
+- Operating System: MacOS or Windows 11.
+- Valid credentials for connecting to the LightSolver Cloud ([Registration](https://id.lightsolver.com/signin/register)).
+- LightSolver Client code project (provided separately).
+    - Verify installation of software for unzipping the LightSolver Client.
+- Python 3.10 or higher ([Download Here](https://www.python.org/downloads/release/python-31011/)).
+    - Select the appropriate MacOS/Windows version at the bottom.
+    - Note: for Windows installation, switch on the "Add to Path" option in the wizard.
 - Highly Recommended: Use a virtual environment before installing laser-mind-client (Please see detailed action further below under the relevant OS).
 
 ### Installation
-Complete the installation on Windows or Ubuntu as described below.
-For further assistance  with setup or connection issues, contact support@lightsolver.com.
+Complete the installation on Windows or MacOS as described below.
+For further assistance with setup or connection issues, contact support@lightsolver.com.
 
 #### Windows
 1. Press the windows key, type "cmd", right click on the result and select "Run as administrator".
 2. Navigate to the root folder where you unzipped and plan to use the LightSolver Client:
     ```
     cd <your project folder>
     ```
@@ -89,26 +92,22 @@
 ```
 
 7. (Recommended) Test LightSolver credentials
     Run the following command:
 ```sh
     python test_env.py
 ```
-    if test credentials failed , please  reinstall credentials using following commands:
-    - Exit virtual environment , by running :
+8. (Recommended) Test - using the inline project test examples
+   Run the following command:
 ```sh
-    deactivate
-```
-    - Run the following command:
-```sh
-    python setup_env.py
+    python ./tests/test_solve_qubo_matrix.py
 ```
 
 
-#### Ubuntu
+#### MacOS
 1. Open new terminal window
 2. Navigate to the root folder where you unzipped and plan to use the LightSolver Client:
     ```
     cd <your project folder>
     ```
 
 3. (Recommended) Set the LightSolver credentials using environment variables (will remove the need to provide credentials for every usage).
@@ -135,25 +134,22 @@
 ```
 
 7. (Recommended) Test LightSolver credentials
     Run the following command:
 ```sh
     python3 test_env.py
 ```
-    if test credentials failed , please  reinstall credentials using following commands:
-    - Exit virtual environment , by running :
-```sh
-    deactivate
-```
-    - Run the following command:
+
+8. (Recommended) Test - using the inline project test examples
+   Run the following command:
 ```sh
-    python3 setup_env.py
-    source ~/.bash_profile
+    python3 ./tests/test_solve_qubo_matrix.py
 ```
 
+***
 ## Authentication
 Initialization of the `LaserMind` class automatically forms a secure and authenticated connection with the LightSolver Cloud.
 Subsequent calls by the same user are similarly secure and authenticated.
 
 ## Usage
 To begin solving any QUBO problem:
 1. Create an instance of the ```LaserMind``` class. This class represents the client that requests solutions from the LightSolver Cloud.
@@ -207,15 +203,15 @@
 
 res = lsClient.solve_qubo(edgeList=quboListData, timeout=1)
 
 print(res)
 ```
 
 ### Solve QUBO Matrix using Asynchronous Flow
-This example demonstratse how to solve a QUBO problem asynchronously using the LightSolver Platform Client.
+This example demonstrates how to solve a QUBO problem asynchronously using the LightSolver Platform Client.
 Begin by creating a matrix to represent your QUBO problem.
 The `solve_qubo` function is used with the following parameters:
    - `matrixData`: A 2D array representing the QUBO problem.
    - `timeout`: The desired time limit for the calculation in seconds.
    - `waitForSolution`: A boolean flag set to `False` to indicate non-blocking mode.
 
 ```python
```

### Comparing `laser_mind_client-0.21.2/pyproject.toml` & `laser_mind_client-0.22.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "laser-mind-client"
-version = "0.21.2"
+version = "0.22.0"
 description = "A client python API for accessing LightSolver's capabilities"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [ "numpy>=1.21.5", "laser-mind-client-meta>=0.0.9", "ls_api_clients>=0.4.6", "ls-packers>=0.2.0",]
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
```

