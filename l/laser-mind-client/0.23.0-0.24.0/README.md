# Comparing `tmp/laser_mind_client-0.23.0.tar.gz` & `tmp/laser_mind_client-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laser_mind_client-0.23.0.tar", last modified: Thu May 23 11:27:02 2024, max compression
+gzip compressed data, was "laser_mind_client-0.24.0.tar", last modified: Thu May 23 14:01:58 2024, max compression
```

## Comparing `laser_mind_client-0.23.0.tar` & `laser_mind_client-0.24.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:27:02.305035 laser_mind_client-0.23.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8914 2024-05-23 11:27:02.305035 laser_mind_client-0.23.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8294 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:27:02.301035 laser_mind_client-0.23.0/laser_mind_client/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/laser_mind_client/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8587 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/laser_mind_client/laser_mind_client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:27:02.305035 laser_mind_client-0.23.0/laser_mind_client.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8914 2024-05-23 11:27:02.000000 laser_mind_client-0.23.0/laser_mind_client.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      415 2024-05-23 11:27:02.000000 laser_mind_client-0.23.0/laser_mind_client.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 11:27:02.000000 laser_mind_client-0.23.0/laser_mind_client.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-05-23 11:27:02.000000 laser_mind_client-0.23.0/laser_mind_client.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-23 11:27:02.000000 laser_mind_client-0.23.0/laser_mind_client.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      722 2024-05-23 11:26:53.000000 laser_mind_client-0.23.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 11:27:02.305035 laser_mind_client-0.23.0/setup.cfg
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:27:02.305035 laser_mind_client-0.23.0/tests/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      453 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/tests/test_solve_qubo_adjacency_list.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      529 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/tests/test_solve_qubo_matrix.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      992 2024-05-23 10:46:36.000000 laser_mind_client-0.23.0/tests/test_solve_qubo_matrix_async.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 14:01:58.486000 laser_mind_client-0.24.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 13:10:36.000000 laser_mind_client-0.24.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8440 2024-05-23 14:01:58.486000 laser_mind_client-0.24.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7819 2024-05-23 13:48:50.000000 laser_mind_client-0.24.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 14:01:58.486000 laser_mind_client-0.24.0/laser_mind_client/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-23 13:10:36.000000 laser_mind_client-0.24.0/laser_mind_client/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8127 2024-05-23 13:48:50.000000 laser_mind_client-0.24.0/laser_mind_client/laser_mind_client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 14:01:58.486000 laser_mind_client-0.24.0/laser_mind_client.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8440 2024-05-23 14:01:58.000000 laser_mind_client-0.24.0/laser_mind_client.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      415 2024-05-23 14:01:58.000000 laser_mind_client-0.24.0/laser_mind_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 14:01:58.000000 laser_mind_client-0.24.0/laser_mind_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       85 2024-05-23 14:01:58.000000 laser_mind_client-0.24.0/laser_mind_client.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-23 14:01:58.000000 laser_mind_client-0.24.0/laser_mind_client.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      723 2024-05-23 14:01:50.000000 laser_mind_client-0.24.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 14:01:58.486000 laser_mind_client-0.24.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 14:01:58.486000 laser_mind_client-0.24.0/tests/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      522 2024-05-23 13:48:50.000000 laser_mind_client-0.24.0/tests/test_solve_qubo_adjacency_list.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      598 2024-05-23 13:48:50.000000 laser_mind_client-0.24.0/tests/test_solve_qubo_matrix.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2024-05-23 13:48:50.000000 laser_mind_client-0.24.0/tests/test_solve_qubo_matrix_async.py
```

### Comparing `laser_mind_client-0.23.0/LICENSE` & `laser_mind_client-0.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laser_mind_client-0.23.0/PKG-INFO` & `laser_mind_client-0.24.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: laser-mind-client
-Version: 0.23.0
-Summary: A client python API for accessing LightSolver's capabilities
-Author-email: Assaf Kalinski <assaf@lightsolver.com>
-Project-URL: Homepage, https://lightsolver.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.21.5
-Requires-Dist: laser-mind-client-meta>=0.0.9
-Requires-Dist: ls_api_clients>=0.4.6
-Requires-Dist: ls-packers>=0.2.0
-
 
 ## LightSolver Platform Client
 The LightSolver Platform Client is a Python package designed to interface with the LightSolver Cloud to facilitate solving Quadratic Unconstrained Binary Optimization (QUBO) problems.
 
 This package is designated for internal access to features during the development process, as well as serves as a prototype for future versions of the production LightSolver Platform Client.
 
 ## Features
@@ -47,105 +30,73 @@
 - **Synchronous Mode (Default):** The `waitForSolution` flag is set to **True** by default. The function blocks operations until a result is received.
 - **Asynchronous Mode:** Set `waitForSolution` to **False**. The function returns immediately with a token object, allowing the script to continue while the server processes the QUBO problem.
 
 ## Setting Up
 
 ### Prerequisites
 - Operating System: MacOS or Windows 11.
-- Valid credentials for connecting to the LightSolver Cloud ([Registration](https://id.lightsolver.com/signin/register)).
-- LightSolver Client code project (provided separately).
-    - Verify installation of software for unzipping the LightSolver Client.
+- Valid token for connecting to the LightSolver Cloud (provided separately).
 - Python 3.10 or higher ([Download Here](https://www.python.org/downloads/release/python-31011/)).
     - Select the appropriate MacOS/Windows version at the bottom.
     - Note: for Windows installation, switch on the "Add to Path" option in the wizard.
 - Highly Recommended: Use a virtual environment before installing laser-mind-client (Please see detailed action further below under the relevant OS).
 
 ### Installation
 Complete the installation on Windows or MacOS as described below.
 For further assistance with setup or connection issues, contact support@lightsolver.com.
 
 #### Windows
-1. Press the windows key, type "cmd", right click on the result and select "Run as administrator".
-2. Navigate to the root folder where you unzipped and plan to use the LightSolver Client:
-    ```
-    cd <your project folder>
-    ```
+1. Press the windows key, type "cmd", and select "Command Prompt".
 
-3. (Recommended) Set the LightSolver credentials using environment variables (will remove the need to provide credentials for every usage).
-    Run the following command:
+2. Navigate to the root folder of the project where you plan to use the LightSolver Client:
 ```sh
-    python setup_env.py
+    cd <your project folder>
 ```
 
-4. (Recommended) Create a virtual environment:
+3. (Recommended) Create and activate the virtual environment:
 ```sh
     python -m venv .venv
-```
-
-5. (Recommended) Activate the new virtual environment:
-```sh
     .venv\Scripts\activate
 ```
 
-6. Install the laser-mind-client package. This command instructs pip to install the package from a local folder instead of searching online:
+4. Install the laser-mind-client package:
 ```sh
-    pip install --no-cache-dir --find-links=.\packages laser-mind-client
+    pip install laser-mind-client
 ```
 
-7. (Recommended) Test LightSolver credentials
-    Run the following command:
-```sh
-    python test_env.py
-```
-8. (Recommended) Test - using the inline project test examples
-   Run the following command:
+5. (Recommended) Test using one of the provided test examples. Unzip "lightsolver_onboarding.zip."
 ```sh
+    cd lightsolver_onboarding
     python ./tests/test_solve_qubo_matrix.py
 ```
 
 
 #### MacOS
-1. Open new terminal window
-2. Navigate to the root folder where you unzipped and plan to use the LightSolver Client:
-    ```
-    cd <your project folder>
-    ```
+1. Open new terminal window.
 
-3. (Recommended) Set the LightSolver credentials using environment variables (will remove the need to provide credentials for every usage).
-    Run the following command:
+2. Navigate to the root folder of the project where you plan to use the LightSolver Client:
 ```sh
-    python3 setup_env.py
-    source ~/.bash_profile
+    cd <your project folder>
 ```
 
-4. (Recommended) Create a virtual environment:
+4. (Recommended) Create and activate the virtual environment:
 ```sh
     python3 -m venv .venv
-```
-
-5. (Recommended) Activate the new virtual environment:
-```sh
     chmod 755  .venv/bin/activate
     source .venv/bin/activate
 ```
 
-6. Install the laser-mind-client package. This command instructs pip to install the package from a local folder instead of searching online:
-```sh
-    pip install --no-cache-dir --find-links=./packages laser-mind-client
-```
-
-7. (Recommended) Test LightSolver credentials
-    Run the following command:
+5. Install the laser-mind-client package.
 ```sh
-    python3 test_env.py
+    pip install laser-mind-client
 ```
 
-8. (Recommended) Test - using the inline project test examples
-   Run the following command:
+8. (Recommended) Test using one of the provided test examples. Unzip "lightsolver_onboarding.zip."
 ```sh
+    cd lightsolver_onboarding
     python3 ./tests/test_solve_qubo_matrix.py
 ```
 
 ***
 ## Authentication
 Initialization of the `LaserMind` class automatically forms a secure and authenticated connection with the LightSolver Cloud.
 Subsequent calls by the same user are similarly secure and authenticated.
@@ -160,82 +111,100 @@
 This example creates a matrix representing a QUBO problem and solves it using the LightSolver Platform Client.
 The `solve_qubo` function is used with the following parameters:
 - ```matrixData```: A 2D array representing the QUBO problem.
 - ```timeout```: The required time limit for the calculation in seconds.
 
 ```python
 import numpy
+from laser_mind_client_meta import MessageKeys
 from laser_mind_client import LaserMind
 
+# Enter your TOKEN here
+userToken = "<my_token>"
+
 # Create a mock QUBO problem
 quboProblemData = numpy.random.randint(-1, 2, (10,10))
 
 # Symmetrize the matrix
 quboProblemData = (quboProblemData + quboProblemData.T) // 2
 
 # Connect to the LightSolver Cloud
-lsClient = LaserMind()
+lsClient = LaserMind(userToken=userToken)
 
 res = lsClient.solve_qubo(matrixData = quboProblemData, timeout=1)
 
-print(res)
+assert MessageKeys.SOLUTION in res, "Test FAILED, response is not in expected format"
+
+print(f"Test PASSED, response is: \n{res}")
 ```
 
 ### Solve QUBO Adjacency List Example
 This example describes a QUBO problem using an adjacency list. This is useful for sparse matrices.
 The `solve_qubo` function is used with the following parameters:
 - ```edgeList```: The adjacency list representing the QUBO problem.
 - ```timeout```: The required time limit for the calculation in seconds.
 
 
 ```python
+from laser_mind_client_meta import MessageKeys
 from laser_mind_client import LaserMind
 
+# Enter your TOKEN here
+userToken = "<my_token>"
+
 # Create a mock QUBO problem
 quboListData = [
     [1,1,5],
     [1,2,-6],
     [2,2,3],
     [2,3,-1],
     [3,10,1]]
 
 # Connect to the LightSolver Cloud
-lsClient = LaserMind()
+lsClient = LaserMind(userToken=userToken)
 
 res = lsClient.solve_qubo(edgeList=quboListData, timeout=1)
 
-print(res)
+assert MessageKeys.SOLUTION in res, "Test FAILED, response is not in expected format"
+
+print(f"Test PASSED, response is: \n{res}")
 ```
 
 ### Solve QUBO Matrix using Asynchronous Flow
 This example demonstrates how to solve a QUBO problem asynchronously using the LightSolver Platform Client.
 Begin by creating a matrix to represent your QUBO problem.
 The `solve_qubo` function is used with the following parameters:
    - `matrixData`: A 2D array representing the QUBO problem.
    - `timeout`: The desired time limit for the calculation in seconds.
    - `waitForSolution`: A boolean flag set to `False` to indicate non-blocking mode.
 
 ```python
 import numpy
+from laser_mind_client_meta import MessageKeys
 from laser_mind_client import LaserMind
 
+# Enter your TOKEN here
+userToken = "<my_token>"
+
 # Create a mock QUBO problem
 quboProblemData = numpy.random.randint(-1, 2, (10,10))
 
 # Symmetrize our matrix
 quboProblemData = (quboProblemData + quboProblemData.T) // 2
 
 # Connect to the LightSolver Cloud
-lsClient = LaserMind()
+lsClient = LaserMind(userToken=userToken)
 
 # Request a solution to the QUBO problem and get the request token for future retrieval.
 # This call does not block operations until the problem is solved.
 requestToken = lsClient.solve_qubo(matrixData = quboProblemData, timeout=1, waitForSolution=False)
 
 # You can run other code here that is not dependant on the request, while the server processes your request.
 
 # Retrieve the solution using the get_solution_sync method.
 # This blocks operations until the solution is acquired.
 res = lsClient.get_solution_sync(requestToken)
 
-print(res)
+assert MessageKeys.SOLUTION in res, "Test FAILED, response is not in expected format"
+
+print(f"Test PASSED, response is: \n{res}")
 ```
```

### Comparing `laser_mind_client-0.23.0/README.md` & `laser_mind_client-0.24.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: laser-mind-client
+Version: 0.24.0
+Summary: A client python API for accessing LightSolver's capabilities
+Author-email: Assaf Kalinski <assaf@lightsolver.com>
+Project-URL: Homepage, https://lightsolver.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.21.5
+Requires-Dist: laser-mind-client-meta>=0.0.9
+Requires-Dist: ls_api_clients>=0.16.0
+Requires-Dist: ls-packers>=0.2.0
+
 
 ## LightSolver Platform Client
 The LightSolver Platform Client is a Python package designed to interface with the LightSolver Cloud to facilitate solving Quadratic Unconstrained Binary Optimization (QUBO) problems.
 
 This package is designated for internal access to features during the development process, as well as serves as a prototype for future versions of the production LightSolver Platform Client.
 
 ## Features
@@ -30,105 +47,73 @@
 - **Synchronous Mode (Default):** The `waitForSolution` flag is set to **True** by default. The function blocks operations until a result is received.
 - **Asynchronous Mode:** Set `waitForSolution` to **False**. The function returns immediately with a token object, allowing the script to continue while the server processes the QUBO problem.
 
 ## Setting Up
 
 ### Prerequisites
 - Operating System: MacOS or Windows 11.
-- Valid credentials for connecting to the LightSolver Cloud ([Registration](https://id.lightsolver.com/signin/register)).
-- LightSolver Client code project (provided separately).
-    - Verify installation of software for unzipping the LightSolver Client.
+- Valid token for connecting to the LightSolver Cloud (provided separately).
 - Python 3.10 or higher ([Download Here](https://www.python.org/downloads/release/python-31011/)).
     - Select the appropriate MacOS/Windows version at the bottom.
     - Note: for Windows installation, switch on the "Add to Path" option in the wizard.
 - Highly Recommended: Use a virtual environment before installing laser-mind-client (Please see detailed action further below under the relevant OS).
 
 ### Installation
 Complete the installation on Windows or MacOS as described below.
 For further assistance with setup or connection issues, contact support@lightsolver.com.
 
 #### Windows
-1. Press the windows key, type "cmd", right click on the result and select "Run as administrator".
-2. Navigate to the root folder where you unzipped and plan to use the LightSolver Client:
-    ```
-    cd <your project folder>
-    ```
+1. Press the windows key, type "cmd", and select "Command Prompt".
 
-3. (Recommended) Set the LightSolver credentials using environment variables (will remove the need to provide credentials for every usage).
-    Run the following command:
+2. Navigate to the root folder of the project where you plan to use the LightSolver Client:
 ```sh
-    python setup_env.py
+    cd <your project folder>
 ```
 
-4. (Recommended) Create a virtual environment:
+3. (Recommended) Create and activate the virtual environment:
 ```sh
     python -m venv .venv
-```
-
-5. (Recommended) Activate the new virtual environment:
-```sh
     .venv\Scripts\activate
 ```
 
-6. Install the laser-mind-client package. This command instructs pip to install the package from a local folder instead of searching online:
+4. Install the laser-mind-client package:
 ```sh
-    pip install --no-cache-dir --find-links=.\packages laser-mind-client
+    pip install laser-mind-client
 ```
 
-7. (Recommended) Test LightSolver credentials
-    Run the following command:
-```sh
-    python test_env.py
-```
-8. (Recommended) Test - using the inline project test examples
-   Run the following command:
+5. (Recommended) Test using one of the provided test examples. Unzip "lightsolver_onboarding.zip."
 ```sh
+    cd lightsolver_onboarding
     python ./tests/test_solve_qubo_matrix.py
 ```
 
 
 #### MacOS
-1. Open new terminal window
-2. Navigate to the root folder where you unzipped and plan to use the LightSolver Client:
-    ```
-    cd <your project folder>
-    ```
+1. Open new terminal window.
 
-3. (Recommended) Set the LightSolver credentials using environment variables (will remove the need to provide credentials for every usage).
-    Run the following command:
+2. Navigate to the root folder of the project where you plan to use the LightSolver Client:
 ```sh
-    python3 setup_env.py
-    source ~/.bash_profile
+    cd <your project folder>
 ```
 
-4. (Recommended) Create a virtual environment:
+4. (Recommended) Create and activate the virtual environment:
 ```sh
     python3 -m venv .venv
-```
-
-5. (Recommended) Activate the new virtual environment:
-```sh
     chmod 755  .venv/bin/activate
     source .venv/bin/activate
 ```
 
-6. Install the laser-mind-client package. This command instructs pip to install the package from a local folder instead of searching online:
-```sh
-    pip install --no-cache-dir --find-links=./packages laser-mind-client
-```
-
-7. (Recommended) Test LightSolver credentials
-    Run the following command:
+5. Install the laser-mind-client package.
 ```sh
-    python3 test_env.py
+    pip install laser-mind-client
 ```
 
-8. (Recommended) Test - using the inline project test examples
-   Run the following command:
+8. (Recommended) Test using one of the provided test examples. Unzip "lightsolver_onboarding.zip."
 ```sh
+    cd lightsolver_onboarding
     python3 ./tests/test_solve_qubo_matrix.py
 ```
 
 ***
 ## Authentication
 Initialization of the `LaserMind` class automatically forms a secure and authenticated connection with the LightSolver Cloud.
 Subsequent calls by the same user are similarly secure and authenticated.
@@ -143,82 +128,100 @@
 This example creates a matrix representing a QUBO problem and solves it using the LightSolver Platform Client.
 The `solve_qubo` function is used with the following parameters:
 - ```matrixData```: A 2D array representing the QUBO problem.
 - ```timeout```: The required time limit for the calculation in seconds.
 
 ```python
 import numpy
+from laser_mind_client_meta import MessageKeys
 from laser_mind_client import LaserMind
 
+# Enter your TOKEN here
+userToken = "<my_token>"
+
 # Create a mock QUBO problem
 quboProblemData = numpy.random.randint(-1, 2, (10,10))
 
 # Symmetrize the matrix
 quboProblemData = (quboProblemData + quboProblemData.T) // 2
 
 # Connect to the LightSolver Cloud
-lsClient = LaserMind()
+lsClient = LaserMind(userToken=userToken)
 
 res = lsClient.solve_qubo(matrixData = quboProblemData, timeout=1)
 
-print(res)
+assert MessageKeys.SOLUTION in res, "Test FAILED, response is not in expected format"
+
+print(f"Test PASSED, response is: \n{res}")
 ```
 
 ### Solve QUBO Adjacency List Example
 This example describes a QUBO problem using an adjacency list. This is useful for sparse matrices.
 The `solve_qubo` function is used with the following parameters:
 - ```edgeList```: The adjacency list representing the QUBO problem.
 - ```timeout```: The required time limit for the calculation in seconds.
 
 
 ```python
+from laser_mind_client_meta import MessageKeys
 from laser_mind_client import LaserMind
 
+# Enter your TOKEN here
+userToken = "<my_token>"
+
 # Create a mock QUBO problem
 quboListData = [
     [1,1,5],
     [1,2,-6],
     [2,2,3],
     [2,3,-1],
     [3,10,1]]
 
 # Connect to the LightSolver Cloud
-lsClient = LaserMind()
+lsClient = LaserMind(userToken=userToken)
 
 res = lsClient.solve_qubo(edgeList=quboListData, timeout=1)
 
-print(res)
+assert MessageKeys.SOLUTION in res, "Test FAILED, response is not in expected format"
+
+print(f"Test PASSED, response is: \n{res}")
 ```
 
 ### Solve QUBO Matrix using Asynchronous Flow
 This example demonstrates how to solve a QUBO problem asynchronously using the LightSolver Platform Client.
 Begin by creating a matrix to represent your QUBO problem.
 The `solve_qubo` function is used with the following parameters:
    - `matrixData`: A 2D array representing the QUBO problem.
    - `timeout`: The desired time limit for the calculation in seconds.
    - `waitForSolution`: A boolean flag set to `False` to indicate non-blocking mode.
 
 ```python
 import numpy
+from laser_mind_client_meta import MessageKeys
 from laser_mind_client import LaserMind
 
+# Enter your TOKEN here
+userToken = "<my_token>"
+
 # Create a mock QUBO problem
 quboProblemData = numpy.random.randint(-1, 2, (10,10))
 
 # Symmetrize our matrix
 quboProblemData = (quboProblemData + quboProblemData.T) // 2
 
 # Connect to the LightSolver Cloud
-lsClient = LaserMind()
+lsClient = LaserMind(userToken=userToken)
 
 # Request a solution to the QUBO problem and get the request token for future retrieval.
 # This call does not block operations until the problem is solved.
 requestToken = lsClient.solve_qubo(matrixData = quboProblemData, timeout=1, waitForSolution=False)
 
 # You can run other code here that is not dependant on the request, while the server processes your request.
 
 # Retrieve the solution using the get_solution_sync method.
 # This blocks operations until the solution is acquired.
 res = lsClient.get_solution_sync(requestToken)
 
-print(res)
+assert MessageKeys.SOLUTION in res, "Test FAILED, response is not in expected format"
+
+print(f"Test PASSED, response is: \n{res}")
 ```
```

### Comparing `laser_mind_client-0.23.0/laser_mind_client/laser_mind_client.py` & `laser_mind_client-0.24.0/laser_mind_client/laser_mind_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,31 +28,23 @@
     """
     ## A client for accessing LightSolver's computaion capabilities via web services.
     """
     POLL_MAX_RETRIES = 100000
     POLL_DELAY_SECS = 0.5
 
     def __init__(self,
-                 username = None,
-                 password = None,
+                 userToken = None,
                  states_per_call=3):
-        if username == None:
-            if 'LS_USER' in os.environ:
-                username = os.environ['LS_USER']
-            else:
-                raise Exception("the 'username' parameter cannot be None if the LS_USER environment variable is not set.")
-        if password == None:
-            if 'LS_PASS' in os.environ:
-                password = os.environ['LS_PASS']
-            else:
-                raise Exception("the 'password' parameter cannot be None if the LS_PASS environment variable is not set.")
+        if userToken is None:
+            raise Exception("the 'token' parameter cannot be None ")
+
         try:
             self.states_per_call = states_per_call
             logging.info('LightSolver connection init started')
-            self.apiClient = LSAPIClient(username, password)
+            self.apiClient = LSAPIClient(userToken)
             logging.info('LightSolver connection init finished')
         except requests.exceptions.ConnectionError as e:
             raise Exception("!!!!! No access to LightSolver Cloud. !!!!!")
         except Exception as e:
                 raise  e
 
     def get_solution_by_id(self, solutionId, timestamp):
```

### Comparing `laser_mind_client-0.23.0/laser_mind_client.egg-info/PKG-INFO` & `laser_mind_client-0.24.0/laser_mind_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: laser-mind-client
-Version: 0.23.0
+Version: 0.24.0
 Summary: A client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.5
 Requires-Dist: laser-mind-client-meta>=0.0.9
-Requires-Dist: ls_api_clients>=0.4.6
+Requires-Dist: ls_api_clients>=0.16.0
 Requires-Dist: ls-packers>=0.2.0
 
 
 ## LightSolver Platform Client
 The LightSolver Platform Client is a Python package designed to interface with the LightSolver Cloud to facilitate solving Quadratic Unconstrained Binary Optimization (QUBO) problems.
 
 This package is designated for internal access to features during the development process, as well as serves as a prototype for future versions of the production LightSolver Platform Client.
@@ -47,105 +47,73 @@
 - **Synchronous Mode (Default):** The `waitForSolution` flag is set to **True** by default. The function blocks operations until a result is received.
 - **Asynchronous Mode:** Set `waitForSolution` to **False**. The function returns immediately with a token object, allowing the script to continue while the server processes the QUBO problem.
 
 ## Setting Up
 
 ### Prerequisites
 - Operating System: MacOS or Windows 11.
-- Valid credentials for connecting to the LightSolver Cloud ([Registration](https://id.lightsolver.com/signin/register)).
-- LightSolver Client code project (provided separately).
-    - Verify installation of software for unzipping the LightSolver Client.
+- Valid token for connecting to the LightSolver Cloud (provided separately).
 - Python 3.10 or higher ([Download Here](https://www.python.org/downloads/release/python-31011/)).
     - Select the appropriate MacOS/Windows version at the bottom.
     - Note: for Windows installation, switch on the "Add to Path" option in the wizard.
 - Highly Recommended: Use a virtual environment before installing laser-mind-client (Please see detailed action further below under the relevant OS).
 
 ### Installation
 Complete the installation on Windows or MacOS as described below.
 For further assistance with setup or connection issues, contact support@lightsolver.com.
 
 #### Windows
-1. Press the windows key, type "cmd", right click on the result and select "Run as administrator".
-2. Navigate to the root folder where you unzipped and plan to use the LightSolver Client:
-    ```
-    cd <your project folder>
-    ```
+1. Press the windows key, type "cmd", and select "Command Prompt".
 
-3. (Recommended) Set the LightSolver credentials using environment variables (will remove the need to provide credentials for every usage).
-    Run the following command:
+2. Navigate to the root folder of the project where you plan to use the LightSolver Client:
 ```sh
-    python setup_env.py
+    cd <your project folder>
 ```
 
-4. (Recommended) Create a virtual environment:
+3. (Recommended) Create and activate the virtual environment:
 ```sh
     python -m venv .venv
-```
-
-5. (Recommended) Activate the new virtual environment:
-```sh
     .venv\Scripts\activate
 ```
 
-6. Install the laser-mind-client package. This command instructs pip to install the package from a local folder instead of searching online:
+4. Install the laser-mind-client package:
 ```sh
-    pip install --no-cache-dir --find-links=.\packages laser-mind-client
+    pip install laser-mind-client
 ```
 
-7. (Recommended) Test LightSolver credentials
-    Run the following command:
-```sh
-    python test_env.py
-```
-8. (Recommended) Test - using the inline project test examples
-   Run the following command:
+5. (Recommended) Test using one of the provided test examples. Unzip "lightsolver_onboarding.zip."
 ```sh
+    cd lightsolver_onboarding
     python ./tests/test_solve_qubo_matrix.py
 ```
 
 
 #### MacOS
-1. Open new terminal window
-2. Navigate to the root folder where you unzipped and plan to use the LightSolver Client:
-    ```
-    cd <your project folder>
-    ```
+1. Open new terminal window.
 
-3. (Recommended) Set the LightSolver credentials using environment variables (will remove the need to provide credentials for every usage).
-    Run the following command:
+2. Navigate to the root folder of the project where you plan to use the LightSolver Client:
 ```sh
-    python3 setup_env.py
-    source ~/.bash_profile
+    cd <your project folder>
 ```
 
-4. (Recommended) Create a virtual environment:
+4. (Recommended) Create and activate the virtual environment:
 ```sh
     python3 -m venv .venv
-```
-
-5. (Recommended) Activate the new virtual environment:
-```sh
     chmod 755  .venv/bin/activate
     source .venv/bin/activate
 ```
 
-6. Install the laser-mind-client package. This command instructs pip to install the package from a local folder instead of searching online:
+5. Install the laser-mind-client package.
 ```sh
-    pip install --no-cache-dir --find-links=./packages laser-mind-client
+    pip install laser-mind-client
 ```
 
-7. (Recommended) Test LightSolver credentials
-    Run the following command:
-```sh
-    python3 test_env.py
-```
-
-8. (Recommended) Test - using the inline project test examples
-   Run the following command:
+8. (Recommended) Test using one of the provided test examples. Unzip "lightsolver_onboarding.zip."
 ```sh
+    cd lightsolver_onboarding
     python3 ./tests/test_solve_qubo_matrix.py
 ```
 
 ***
 ## Authentication
 Initialization of the `LaserMind` class automatically forms a secure and authenticated connection with the LightSolver Cloud.
 Subsequent calls by the same user are similarly secure and authenticated.
@@ -160,82 +128,100 @@
 This example creates a matrix representing a QUBO problem and solves it using the LightSolver Platform Client.
 The `solve_qubo` function is used with the following parameters:
 - ```matrixData```: A 2D array representing the QUBO problem.
 - ```timeout```: The required time limit for the calculation in seconds.
 
 ```python
 import numpy
+from laser_mind_client_meta import MessageKeys
 from laser_mind_client import LaserMind
 
+# Enter your TOKEN here
+userToken = "<my_token>"
+
 # Create a mock QUBO problem
 quboProblemData = numpy.random.randint(-1, 2, (10,10))
 
 # Symmetrize the matrix
 quboProblemData = (quboProblemData + quboProblemData.T) // 2
 
 # Connect to the LightSolver Cloud
-lsClient = LaserMind()
+lsClient = LaserMind(userToken=userToken)
 
 res = lsClient.solve_qubo(matrixData = quboProblemData, timeout=1)
 
-print(res)
+assert MessageKeys.SOLUTION in res, "Test FAILED, response is not in expected format"
+
+print(f"Test PASSED, response is: \n{res}")
 ```
 
 ### Solve QUBO Adjacency List Example
 This example describes a QUBO problem using an adjacency list. This is useful for sparse matrices.
 The `solve_qubo` function is used with the following parameters:
 - ```edgeList```: The adjacency list representing the QUBO problem.
 - ```timeout```: The required time limit for the calculation in seconds.
 
 
 ```python
+from laser_mind_client_meta import MessageKeys
 from laser_mind_client import LaserMind
 
+# Enter your TOKEN here
+userToken = "<my_token>"
+
 # Create a mock QUBO problem
 quboListData = [
     [1,1,5],
     [1,2,-6],
     [2,2,3],
     [2,3,-1],
     [3,10,1]]
 
 # Connect to the LightSolver Cloud
-lsClient = LaserMind()
+lsClient = LaserMind(userToken=userToken)
 
 res = lsClient.solve_qubo(edgeList=quboListData, timeout=1)
 
-print(res)
+assert MessageKeys.SOLUTION in res, "Test FAILED, response is not in expected format"
+
+print(f"Test PASSED, response is: \n{res}")
 ```
 
 ### Solve QUBO Matrix using Asynchronous Flow
 This example demonstrates how to solve a QUBO problem asynchronously using the LightSolver Platform Client.
 Begin by creating a matrix to represent your QUBO problem.
 The `solve_qubo` function is used with the following parameters:
    - `matrixData`: A 2D array representing the QUBO problem.
    - `timeout`: The desired time limit for the calculation in seconds.
    - `waitForSolution`: A boolean flag set to `False` to indicate non-blocking mode.
 
 ```python
 import numpy
+from laser_mind_client_meta import MessageKeys
 from laser_mind_client import LaserMind
 
+# Enter your TOKEN here
+userToken = "<my_token>"
+
 # Create a mock QUBO problem
 quboProblemData = numpy.random.randint(-1, 2, (10,10))
 
 # Symmetrize our matrix
 quboProblemData = (quboProblemData + quboProblemData.T) // 2
 
 # Connect to the LightSolver Cloud
-lsClient = LaserMind()
+lsClient = LaserMind(userToken=userToken)
 
 # Request a solution to the QUBO problem and get the request token for future retrieval.
 # This call does not block operations until the problem is solved.
 requestToken = lsClient.solve_qubo(matrixData = quboProblemData, timeout=1, waitForSolution=False)
 
 # You can run other code here that is not dependant on the request, while the server processes your request.
 
 # Retrieve the solution using the get_solution_sync method.
 # This blocks operations until the solution is acquired.
 res = lsClient.get_solution_sync(requestToken)
 
-print(res)
+assert MessageKeys.SOLUTION in res, "Test FAILED, response is not in expected format"
+
+print(f"Test PASSED, response is: \n{res}")
 ```
```

### Comparing `laser_mind_client-0.23.0/pyproject.toml` & `laser_mind_client-0.24.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "laser-mind-client"
-version = "0.23.0"
+version = "0.24.0"
 description = "A client python API for accessing LightSolver's capabilities"
 readme = "README.md"
 requires-python = ">=3.8"
-dependencies = [ "numpy>=1.21.5", "laser-mind-client-meta>=0.0.9", "ls_api_clients>=0.4.6", "ls-packers>=0.2.0",]
+dependencies = [ "numpy>=1.21.5", "laser-mind-client-meta>=0.0.9", "ls_api_clients>=0.16.0", "ls-packers>=0.2.0",]
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
 email = "assaf@lightsolver.com"
 
 [project.urls]
 Homepage = "https://lightsolver.com"
```

### Comparing `laser_mind_client-0.23.0/tests/test_solve_qubo_matrix_async.py` & `laser_mind_client-0.24.0/tests/test_solve_qubo_matrix_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import numpy
 from laser_mind_client_meta import MessageKeys
 from laser_mind_client import LaserMind
 
+# Enter your TOKEN here
+userToken = "<my_token>"
+
 # Create a mock QUBO problem
 quboProblemData = numpy.random.randint(-1, 2, (10,10))
 
 # Symmetrize our matrix
 quboProblemData = (quboProblemData + quboProblemData.T) // 2
 
 # Connect to the LightSolver Cloud
-lsClient = LaserMind()
+lsClient = LaserMind(userToken=userToken)
 
 # Request a solution to the QUBO problem and get the request token for future retrieval.
 # This call does not block operations until the problem is solved.
 requestToken = lsClient.solve_qubo(matrixData = quboProblemData, timeout=1, waitForSolution=False)
 
 # You can run other code here that is not dependant on the request, while the server processes your request.
```

