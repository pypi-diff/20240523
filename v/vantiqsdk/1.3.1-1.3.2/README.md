# Comparing `tmp/vantiqsdk-1.3.1.tar.gz` & `tmp/vantiqsdk-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantiqsdk-1.3.1.tar", last modified: Wed May 15 23:43:42 2024, max compression
+gzip compressed data, was "vantiqsdk-1.3.2.tar", last modified: Thu May 23 00:46:59 2024, max compression
```

## Comparing `vantiqsdk-1.3.1.tar` & `vantiqsdk-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-05-15 23:43:42.267874 vantiqsdk-1.3.1/
--rw-r--r--   0 fcarter    (501) staff       (20)     1079 2022-05-09 21:51:11.000000 vantiqsdk-1.3.1/LICENSE.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       31 2022-05-09 21:51:11.000000 vantiqsdk-1.3.1/MANIFEST.in
--rw-r--r--   0 fcarter    (501) staff       (20)     4758 2024-05-15 23:43:42.266605 vantiqsdk-1.3.1/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)     4135 2023-11-30 21:22:15.000000 vantiqsdk-1.3.1/README.md
--rw-r--r--   0 fcarter    (501) staff       (20)      961 2024-05-15 23:43:30.000000 vantiqsdk-1.3.1/pyproject.toml
--rw-r--r--   0 fcarter    (501) staff       (20)       38 2024-05-15 23:43:42.267951 vantiqsdk-1.3.1/setup.cfg
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-05-15 23:43:42.260899 vantiqsdk-1.3.1/src/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-05-15 23:43:42.261058 vantiqsdk-1.3.1/src/main/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-05-15 23:43:42.263538 vantiqsdk-1.3.1/src/main/python/
-drwxr-xr-x   0 fcarter    (501) staff       (20)        0 2024-05-15 23:43:42.266163 vantiqsdk-1.3.1/src/main/python/vantiqsdk.egg-info/
--rw-r--r--   0 fcarter    (501) staff       (20)     4758 2024-05-15 23:43:42.000000 vantiqsdk-1.3.1/src/main/python/vantiqsdk.egg-info/PKG-INFO
--rw-r--r--   0 fcarter    (501) staff       (20)      321 2024-05-15 23:43:42.000000 vantiqsdk-1.3.1/src/main/python/vantiqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 fcarter    (501) staff       (20)        1 2024-05-15 23:43:42.000000 vantiqsdk-1.3.1/src/main/python/vantiqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       19 2024-05-15 23:43:42.000000 vantiqsdk-1.3.1/src/main/python/vantiqsdk.egg-info/requires.txt
--rw-r--r--   0 fcarter    (501) staff       (20)       10 2024-05-15 23:43:42.000000 vantiqsdk-1.3.1/src/main/python/vantiqsdk.egg-info/top_level.txt
--rw-r--r--   0 fcarter    (501) staff       (20)    67035 2024-05-15 18:58:43.000000 vantiqsdk-1.3.1/src/main/python/vantiqsdk.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:46:59.191064 vantiqsdk-1.3.2/
+-rw-rw-rw-   0        0        0     1100 2023-07-25 15:39:50.000000 vantiqsdk-1.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       31 2023-07-25 15:39:50.000000 vantiqsdk-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4904 2024-05-23 00:46:59.190065 vantiqsdk-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4263 2024-01-03 19:08:16.000000 vantiqsdk-1.3.2/README.md
+-rw-rw-rw-   0        0        0      961 2024-05-23 00:46:41.000000 vantiqsdk-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 00:46:59.191064 vantiqsdk-1.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 00:46:59.170065 vantiqsdk-1.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 00:46:59.171065 vantiqsdk-1.3.2/src/main/
+drwxrwxrwx   0        0        0        0 2024-05-23 00:46:59.182064 vantiqsdk-1.3.2/src/main/python/
+drwxrwxrwx   0        0        0        0 2024-05-23 00:46:59.189064 vantiqsdk-1.3.2/src/main/python/vantiqsdk.egg-info/
+-rw-rw-rw-   0        0        0     4904 2024-05-23 00:46:59.000000 vantiqsdk-1.3.2/src/main/python/vantiqsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2024-05-23 00:46:59.000000 vantiqsdk-1.3.2/src/main/python/vantiqsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 00:46:59.000000 vantiqsdk-1.3.2/src/main/python/vantiqsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-23 00:46:59.000000 vantiqsdk-1.3.2/src/main/python/vantiqsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 00:46:59.000000 vantiqsdk-1.3.2/src/main/python/vantiqsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    69112 2024-05-23 00:34:11.000000 vantiqsdk-1.3.2/src/main/python/vantiqsdk.py
```

### Comparing `vantiqsdk-1.3.1/LICENSE.txt` & `vantiqsdk-1.3.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2022 Vantiq, Inc.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2022 Vantiq, Inc.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `vantiqsdk-1.3.1/PKG-INFO` & `vantiqsdk-1.3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-Metadata-Version: 2.1
-Name: vantiqsdk
-Version: 1.3.1
-Summary: SDK for working with the Vantiq system
-Author-email: Vantiq <fcarter@vantiq.com>
-License: MIT
-Project-URL: Homepage, https://github.com/vantiq/vantiq-python-sdk
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: websockets
-Requires-Dist: aiohttp
-
-
-# Vantiq SDK for Python
-
-The [Vantiq](http://www.vantiq.com) Python SDK is a Python package that provides an 
-API into a Vantiq system from Python applications.  The SDK connects to a
-Vantiq system using the 
-[Vantiq REST API](https://dev.vantiq.com/docs/system/api/index.html).
-
-## Installation
-
-The SDK is installed from the PyPI repo.  To install this into your system,
-use
-```commandline
-    pip install vantiqsdk
-```
-
-Note: depending on your local environment, you may need to use `pip3`
-instead of `pip`, or whatever is appropriate to install into your
-virtual environment.
-
-The Vantiq SDK for Python requires Python version 3.10 or better.
-It is built using `asyncio`, `aiohttp`, and `websockets`. In the documentation
-that follows, methods marked as _Async_ must be awaited. For more information
-about `asyncio` and `await`, please see the 
-[Python `asyncio` documentation](https://docs.python.org/3/library/asyncio.html)).
-
-## Quick Start
-
-You will need valid credentials on a Vantiq server in the form of a
-username and password or access token.  If you have a private Vantiq server,
-contact your administrator for credentials.  If you wish to use the
-Vantiq public cloud, contact [support@vantiq.com](mailto:support@vantiq.com).
-
-The first step is to create an instance of the Vantiq SDK providing the URL of the Vantiq server to connect:
-
-```python
-from vantiqsdk import Vantiq, VantiqResources, VantiqResponse
-import vantiqsdk
-
-server: str = "https://dev.vantiq.com"
-
-vantiq: Vantiq = Vantiq(server)
-```
-
-where `server` is the full URL for the Vantiq server to connect to, such as *https://dev.vantiq.com/*. 
-An optional second argument is the version of the API to connect to. 
-If not specified, this defaults to the latest version, currently *1*. 
-At this point, the *Vantiq* instance has not yet connected to the server.  
-To establish a connection to the server, use the `authenticate` method, e.g.,
-
-```python
-username = "joe@user"
-password = "my-secr3t-passw0rd!#!"
-
-await vantiq.authenticate(username, password)
-```
-
-The `username` and `password` are the same credentials used to log into the system.
-Note the username and password are not stored either in-memory or persistently after
-this authentication call.  After successfully authenticating with the system,
-the *Vantiq* instance stores an in-memory access token that subsequent API calls
-will use.
-
-Now, you are able to perform any SDK calls to the Vantiq server.  The async methods
-on the SDK classes can be immediately awaited to run in, effectively, a synchronous
-fashion, or they can return an `Awaitable` that can be _awaited_ later.
-
-```python
-vr: VantiqResponse = await vantiq.select(VantiqResources.TYPES)
-
-```
-
-Alternatively,
-
-```python
-to_await = vantiq.select(VantiqResources.TYPES)
-...
-vr: VantiqResponse = await to_await
-```
-
-In either case, the response to the operation is available
-in the VantiqResponse instance.
-
-## Documentation
-
-For the full documentation on the SDK, see the
-[SDK API Reference](https://github.com/Vantiq/vantiq-python-sdk/blob/master/docs/api.md).
-
-## Developers
-
-The project is set up as a `gradle` project.  To run the tests, use
-
-```commandline
-./gradlew test
-```
-
-or
-
-```commandline
-./gradlew.bat test
-```
-
-in a windows environment.
-
-The tests run will run a mocked version. To execute tests against a _live_ server,
-define the following gradle properties in your ~/.gradle/gradle.properties file:
-
-```properties
-# Python project values
-TestVantiqServer=<Vantiq server url> # Only do the base URL. Ex http://localhost:8080/
-TestAccessToken=<access token from that Vantiq system>
-TestVantiqUsername=<Vantiq user name>
-TestVantiqPassword=<Password for that Vantiq user>
-```
-
-Alternatively, when running directly, use the following environment variables:
-
-```commandline
-VANTIQ_URL <Vantiq erver url>
-VANTIQ_ACCESS_TOKEN <Access token from that Vantiq system>
-VANTIQ_USERNAME <Vantiq user name>
-VANTIQ_PASSWORD <Password for that Vantiq user>
-```
-
-## Copyright and License
-
-Copyright &copy; 2022 Vantiq, Inc.  Code released under the
-[MIT license](https://github.com/Vantiq/vantiq-python-sdk/blob/master/LICENSE.txt).
+Metadata-Version: 2.1
+Name: vantiqsdk
+Version: 1.3.2
+Summary: SDK for working with the Vantiq system
+Author-email: Vantiq <fcarter@vantiq.com>
+License: MIT
+Project-URL: Homepage, https://github.com/vantiq/vantiq-python-sdk
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: websockets
+Requires-Dist: aiohttp
+
+
+# Vantiq SDK for Python
+
+The [Vantiq](http://www.vantiq.com) Python SDK is a Python package that provides an 
+API into a Vantiq system from Python applications.  The SDK connects to a
+Vantiq system using the 
+[Vantiq REST API](https://dev.vantiq.com/docs/system/api/index.html).
+
+## Installation
+
+The SDK is installed from the PyPI repo.  To install this into your system,
+use
+```commandline
+    pip install vantiqsdk
+```
+
+Note: depending on your local environment, you may need to use `pip3`
+instead of `pip`, or whatever is appropriate to install into your
+virtual environment.
+
+The Vantiq SDK for Python requires Python version 3.10 or better.
+It is built using `asyncio`, `aiohttp`, and `websockets`. In the documentation
+that follows, methods marked as _Async_ must be awaited. For more information
+about `asyncio` and `await`, please see the 
+[Python `asyncio` documentation](https://docs.python.org/3/library/asyncio.html)).
+
+## Quick Start
+
+You will need valid credentials on a Vantiq server in the form of a
+username and password or access token.  If you have a private Vantiq server,
+contact your administrator for credentials.  If you wish to use the
+Vantiq public cloud, contact [support@vantiq.com](mailto:support@vantiq.com).
+
+The first step is to create an instance of the Vantiq SDK providing the URL of the Vantiq server to connect:
+
+```python
+from vantiqsdk import Vantiq, VantiqResources, VantiqResponse
+import vantiqsdk
+
+server: str = "https://dev.vantiq.com"
+
+vantiq: Vantiq = Vantiq(server)
+```
+
+where `server` is the full URL for the Vantiq server to connect to, such as *https://dev.vantiq.com/*. 
+An optional second argument is the version of the API to connect to. 
+If not specified, this defaults to the latest version, currently *1*. 
+At this point, the *Vantiq* instance has not yet connected to the server.  
+To establish a connection to the server, use the `authenticate` method, e.g.,
+
+```python
+username = "joe@user"
+password = "my-secr3t-passw0rd!#!"
+
+await vantiq.authenticate(username, password)
+```
+
+The `username` and `password` are the same credentials used to log into the system.
+Note the username and password are not stored either in-memory or persistently after
+this authentication call.  After successfully authenticating with the system,
+the *Vantiq* instance stores an in-memory access token that subsequent API calls
+will use.
+
+Now, you are able to perform any SDK calls to the Vantiq server.  The async methods
+on the SDK classes can be immediately awaited to run in, effectively, a synchronous
+fashion, or they can return an `Awaitable` that can be _awaited_ later.
+
+```python
+vr: VantiqResponse = await vantiq.select(VantiqResources.TYPES)
+
+```
+
+Alternatively,
+
+```python
+to_await = vantiq.select(VantiqResources.TYPES)
+...
+vr: VantiqResponse = await to_await
+```
+
+In either case, the response to the operation is available
+in the VantiqResponse instance.
+
+## Documentation
+
+For the full documentation on the SDK, see the
+[SDK API Reference](https://github.com/Vantiq/vantiq-python-sdk/blob/master/docs/api.md).
+
+## Developers
+
+The project is set up as a `gradle` project.  To run the tests, use
+
+```commandline
+./gradlew test
+```
+
+or
+
+```commandline
+./gradlew.bat test
+```
+
+in a windows environment.
+
+The tests run will run a mocked version. To execute tests against a _live_ server,
+define the following gradle properties in your ~/.gradle/gradle.properties file:
+
+```properties
+# Python project values
+TestVantiqServer=<Vantiq server url> # Only do the base URL. Ex http://localhost:8080/
+TestAccessToken=<access token from that Vantiq system>
+TestVantiqUsername=<Vantiq user name>
+TestVantiqPassword=<Password for that Vantiq user>
+```
+
+Alternatively, when running directly, use the following environment variables:
+
+```commandline
+VANTIQ_URL <Vantiq erver url>
+VANTIQ_ACCESS_TOKEN <Access token from that Vantiq system>
+VANTIQ_USERNAME <Vantiq user name>
+VANTIQ_PASSWORD <Password for that Vantiq user>
+```
+
+## Copyright and License
+
+Copyright &copy; 2022 Vantiq, Inc.  Code released under the
+[MIT license](https://github.com/Vantiq/vantiq-python-sdk/blob/master/LICENSE.txt).
```

### Comparing `vantiqsdk-1.3.1/README.md` & `vantiqsdk-1.3.2/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-
-# Vantiq SDK for Python
-
-The [Vantiq](http://www.vantiq.com) Python SDK is a Python package that provides an 
-API into a Vantiq system from Python applications.  The SDK connects to a
-Vantiq system using the 
-[Vantiq REST API](https://dev.vantiq.com/docs/system/api/index.html).
-
-## Installation
-
-The SDK is installed from the PyPI repo.  To install this into your system,
-use
-```commandline
-    pip install vantiqsdk
-```
-
-Note: depending on your local environment, you may need to use `pip3`
-instead of `pip`, or whatever is appropriate to install into your
-virtual environment.
-
-The Vantiq SDK for Python requires Python version 3.10 or better.
-It is built using `asyncio`, `aiohttp`, and `websockets`. In the documentation
-that follows, methods marked as _Async_ must be awaited. For more information
-about `asyncio` and `await`, please see the 
-[Python `asyncio` documentation](https://docs.python.org/3/library/asyncio.html)).
-
-## Quick Start
-
-You will need valid credentials on a Vantiq server in the form of a
-username and password or access token.  If you have a private Vantiq server,
-contact your administrator for credentials.  If you wish to use the
-Vantiq public cloud, contact [support@vantiq.com](mailto:support@vantiq.com).
-
-The first step is to create an instance of the Vantiq SDK providing the URL of the Vantiq server to connect:
-
-```python
-from vantiqsdk import Vantiq, VantiqResources, VantiqResponse
-import vantiqsdk
-
-server: str = "https://dev.vantiq.com"
-
-vantiq: Vantiq = Vantiq(server)
-```
-
-where `server` is the full URL for the Vantiq server to connect to, such as *https://dev.vantiq.com/*. 
-An optional second argument is the version of the API to connect to. 
-If not specified, this defaults to the latest version, currently *1*. 
-At this point, the *Vantiq* instance has not yet connected to the server.  
-To establish a connection to the server, use the `authenticate` method, e.g.,
-
-```python
-username = "joe@user"
-password = "my-secr3t-passw0rd!#!"
-
-await vantiq.authenticate(username, password)
-```
-
-The `username` and `password` are the same credentials used to log into the system.
-Note the username and password are not stored either in-memory or persistently after
-this authentication call.  After successfully authenticating with the system,
-the *Vantiq* instance stores an in-memory access token that subsequent API calls
-will use.
-
-Now, you are able to perform any SDK calls to the Vantiq server.  The async methods
-on the SDK classes can be immediately awaited to run in, effectively, a synchronous
-fashion, or they can return an `Awaitable` that can be _awaited_ later.
-
-```python
-vr: VantiqResponse = await vantiq.select(VantiqResources.TYPES)
-
-```
-
-Alternatively,
-
-```python
-to_await = vantiq.select(VantiqResources.TYPES)
-...
-vr: VantiqResponse = await to_await
-```
-
-In either case, the response to the operation is available
-in the VantiqResponse instance.
-
-## Documentation
-
-For the full documentation on the SDK, see the
-[SDK API Reference](https://github.com/Vantiq/vantiq-python-sdk/blob/master/docs/api.md).
-
-## Developers
-
-The project is set up as a `gradle` project.  To run the tests, use
-
-```commandline
-./gradlew test
-```
-
-or
-
-```commandline
-./gradlew.bat test
-```
-
-in a windows environment.
-
-The tests run will run a mocked version. To execute tests against a _live_ server,
-define the following gradle properties in your ~/.gradle/gradle.properties file:
-
-```properties
-# Python project values
-TestVantiqServer=<Vantiq server url> # Only do the base URL. Ex http://localhost:8080/
-TestAccessToken=<access token from that Vantiq system>
-TestVantiqUsername=<Vantiq user name>
-TestVantiqPassword=<Password for that Vantiq user>
-```
-
-Alternatively, when running directly, use the following environment variables:
-
-```commandline
-VANTIQ_URL <Vantiq erver url>
-VANTIQ_ACCESS_TOKEN <Access token from that Vantiq system>
-VANTIQ_USERNAME <Vantiq user name>
-VANTIQ_PASSWORD <Password for that Vantiq user>
-```
-
-## Copyright and License
-
-Copyright &copy; 2022 Vantiq, Inc.  Code released under the
-[MIT license](https://github.com/Vantiq/vantiq-python-sdk/blob/master/LICENSE.txt).
+
+# Vantiq SDK for Python
+
+The [Vantiq](http://www.vantiq.com) Python SDK is a Python package that provides an 
+API into a Vantiq system from Python applications.  The SDK connects to a
+Vantiq system using the 
+[Vantiq REST API](https://dev.vantiq.com/docs/system/api/index.html).
+
+## Installation
+
+The SDK is installed from the PyPI repo.  To install this into your system,
+use
+```commandline
+    pip install vantiqsdk
+```
+
+Note: depending on your local environment, you may need to use `pip3`
+instead of `pip`, or whatever is appropriate to install into your
+virtual environment.
+
+The Vantiq SDK for Python requires Python version 3.10 or better.
+It is built using `asyncio`, `aiohttp`, and `websockets`. In the documentation
+that follows, methods marked as _Async_ must be awaited. For more information
+about `asyncio` and `await`, please see the 
+[Python `asyncio` documentation](https://docs.python.org/3/library/asyncio.html)).
+
+## Quick Start
+
+You will need valid credentials on a Vantiq server in the form of a
+username and password or access token.  If you have a private Vantiq server,
+contact your administrator for credentials.  If you wish to use the
+Vantiq public cloud, contact [support@vantiq.com](mailto:support@vantiq.com).
+
+The first step is to create an instance of the Vantiq SDK providing the URL of the Vantiq server to connect:
+
+```python
+from vantiqsdk import Vantiq, VantiqResources, VantiqResponse
+import vantiqsdk
+
+server: str = "https://dev.vantiq.com"
+
+vantiq: Vantiq = Vantiq(server)
+```
+
+where `server` is the full URL for the Vantiq server to connect to, such as *https://dev.vantiq.com/*. 
+An optional second argument is the version of the API to connect to. 
+If not specified, this defaults to the latest version, currently *1*. 
+At this point, the *Vantiq* instance has not yet connected to the server.  
+To establish a connection to the server, use the `authenticate` method, e.g.,
+
+```python
+username = "joe@user"
+password = "my-secr3t-passw0rd!#!"
+
+await vantiq.authenticate(username, password)
+```
+
+The `username` and `password` are the same credentials used to log into the system.
+Note the username and password are not stored either in-memory or persistently after
+this authentication call.  After successfully authenticating with the system,
+the *Vantiq* instance stores an in-memory access token that subsequent API calls
+will use.
+
+Now, you are able to perform any SDK calls to the Vantiq server.  The async methods
+on the SDK classes can be immediately awaited to run in, effectively, a synchronous
+fashion, or they can return an `Awaitable` that can be _awaited_ later.
+
+```python
+vr: VantiqResponse = await vantiq.select(VantiqResources.TYPES)
+
+```
+
+Alternatively,
+
+```python
+to_await = vantiq.select(VantiqResources.TYPES)
+...
+vr: VantiqResponse = await to_await
+```
+
+In either case, the response to the operation is available
+in the VantiqResponse instance.
+
+## Documentation
+
+For the full documentation on the SDK, see the
+[SDK API Reference](https://github.com/Vantiq/vantiq-python-sdk/blob/master/docs/api.md).
+
+## Developers
+
+The project is set up as a `gradle` project.  To run the tests, use
+
+```commandline
+./gradlew test
+```
+
+or
+
+```commandline
+./gradlew.bat test
+```
+
+in a windows environment.
+
+The tests run will run a mocked version. To execute tests against a _live_ server,
+define the following gradle properties in your ~/.gradle/gradle.properties file:
+
+```properties
+# Python project values
+TestVantiqServer=<Vantiq server url> # Only do the base URL. Ex http://localhost:8080/
+TestAccessToken=<access token from that Vantiq system>
+TestVantiqUsername=<Vantiq user name>
+TestVantiqPassword=<Password for that Vantiq user>
+```
+
+Alternatively, when running directly, use the following environment variables:
+
+```commandline
+VANTIQ_URL <Vantiq erver url>
+VANTIQ_ACCESS_TOKEN <Access token from that Vantiq system>
+VANTIQ_USERNAME <Vantiq user name>
+VANTIQ_PASSWORD <Password for that Vantiq user>
+```
+
+## Copyright and License
+
+Copyright &copy; 2022 Vantiq, Inc.  Code released under the
+[MIT license](https://github.com/Vantiq/vantiq-python-sdk/blob/master/LICENSE.txt).
```

### Comparing `vantiqsdk-1.3.1/pyproject.toml` & `vantiqsdk-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vantiqsdk"
-version = "1.3.1"
+version = "1.3.2"
 description = "SDK for working with the Vantiq system"
 authors = [
     { name = "Vantiq", email = "fcarter@vantiq.com" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
```

### Comparing `vantiqsdk-1.3.1/src/main/python/vantiqsdk.egg-info/PKG-INFO` & `vantiqsdk-1.3.2/src/main/python/vantiqsdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-Metadata-Version: 2.1
-Name: vantiqsdk
-Version: 1.3.1
-Summary: SDK for working with the Vantiq system
-Author-email: Vantiq <fcarter@vantiq.com>
-License: MIT
-Project-URL: Homepage, https://github.com/vantiq/vantiq-python-sdk
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: websockets
-Requires-Dist: aiohttp
-
-
-# Vantiq SDK for Python
-
-The [Vantiq](http://www.vantiq.com) Python SDK is a Python package that provides an 
-API into a Vantiq system from Python applications.  The SDK connects to a
-Vantiq system using the 
-[Vantiq REST API](https://dev.vantiq.com/docs/system/api/index.html).
-
-## Installation
-
-The SDK is installed from the PyPI repo.  To install this into your system,
-use
-```commandline
-    pip install vantiqsdk
-```
-
-Note: depending on your local environment, you may need to use `pip3`
-instead of `pip`, or whatever is appropriate to install into your
-virtual environment.
-
-The Vantiq SDK for Python requires Python version 3.10 or better.
-It is built using `asyncio`, `aiohttp`, and `websockets`. In the documentation
-that follows, methods marked as _Async_ must be awaited. For more information
-about `asyncio` and `await`, please see the 
-[Python `asyncio` documentation](https://docs.python.org/3/library/asyncio.html)).
-
-## Quick Start
-
-You will need valid credentials on a Vantiq server in the form of a
-username and password or access token.  If you have a private Vantiq server,
-contact your administrator for credentials.  If you wish to use the
-Vantiq public cloud, contact [support@vantiq.com](mailto:support@vantiq.com).
-
-The first step is to create an instance of the Vantiq SDK providing the URL of the Vantiq server to connect:
-
-```python
-from vantiqsdk import Vantiq, VantiqResources, VantiqResponse
-import vantiqsdk
-
-server: str = "https://dev.vantiq.com"
-
-vantiq: Vantiq = Vantiq(server)
-```
-
-where `server` is the full URL for the Vantiq server to connect to, such as *https://dev.vantiq.com/*. 
-An optional second argument is the version of the API to connect to. 
-If not specified, this defaults to the latest version, currently *1*. 
-At this point, the *Vantiq* instance has not yet connected to the server.  
-To establish a connection to the server, use the `authenticate` method, e.g.,
-
-```python
-username = "joe@user"
-password = "my-secr3t-passw0rd!#!"
-
-await vantiq.authenticate(username, password)
-```
-
-The `username` and `password` are the same credentials used to log into the system.
-Note the username and password are not stored either in-memory or persistently after
-this authentication call.  After successfully authenticating with the system,
-the *Vantiq* instance stores an in-memory access token that subsequent API calls
-will use.
-
-Now, you are able to perform any SDK calls to the Vantiq server.  The async methods
-on the SDK classes can be immediately awaited to run in, effectively, a synchronous
-fashion, or they can return an `Awaitable` that can be _awaited_ later.
-
-```python
-vr: VantiqResponse = await vantiq.select(VantiqResources.TYPES)
-
-```
-
-Alternatively,
-
-```python
-to_await = vantiq.select(VantiqResources.TYPES)
-...
-vr: VantiqResponse = await to_await
-```
-
-In either case, the response to the operation is available
-in the VantiqResponse instance.
-
-## Documentation
-
-For the full documentation on the SDK, see the
-[SDK API Reference](https://github.com/Vantiq/vantiq-python-sdk/blob/master/docs/api.md).
-
-## Developers
-
-The project is set up as a `gradle` project.  To run the tests, use
-
-```commandline
-./gradlew test
-```
-
-or
-
-```commandline
-./gradlew.bat test
-```
-
-in a windows environment.
-
-The tests run will run a mocked version. To execute tests against a _live_ server,
-define the following gradle properties in your ~/.gradle/gradle.properties file:
-
-```properties
-# Python project values
-TestVantiqServer=<Vantiq server url> # Only do the base URL. Ex http://localhost:8080/
-TestAccessToken=<access token from that Vantiq system>
-TestVantiqUsername=<Vantiq user name>
-TestVantiqPassword=<Password for that Vantiq user>
-```
-
-Alternatively, when running directly, use the following environment variables:
-
-```commandline
-VANTIQ_URL <Vantiq erver url>
-VANTIQ_ACCESS_TOKEN <Access token from that Vantiq system>
-VANTIQ_USERNAME <Vantiq user name>
-VANTIQ_PASSWORD <Password for that Vantiq user>
-```
-
-## Copyright and License
-
-Copyright &copy; 2022 Vantiq, Inc.  Code released under the
-[MIT license](https://github.com/Vantiq/vantiq-python-sdk/blob/master/LICENSE.txt).
+Metadata-Version: 2.1
+Name: vantiqsdk
+Version: 1.3.2
+Summary: SDK for working with the Vantiq system
+Author-email: Vantiq <fcarter@vantiq.com>
+License: MIT
+Project-URL: Homepage, https://github.com/vantiq/vantiq-python-sdk
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: websockets
+Requires-Dist: aiohttp
+
+
+# Vantiq SDK for Python
+
+The [Vantiq](http://www.vantiq.com) Python SDK is a Python package that provides an 
+API into a Vantiq system from Python applications.  The SDK connects to a
+Vantiq system using the 
+[Vantiq REST API](https://dev.vantiq.com/docs/system/api/index.html).
+
+## Installation
+
+The SDK is installed from the PyPI repo.  To install this into your system,
+use
+```commandline
+    pip install vantiqsdk
+```
+
+Note: depending on your local environment, you may need to use `pip3`
+instead of `pip`, or whatever is appropriate to install into your
+virtual environment.
+
+The Vantiq SDK for Python requires Python version 3.10 or better.
+It is built using `asyncio`, `aiohttp`, and `websockets`. In the documentation
+that follows, methods marked as _Async_ must be awaited. For more information
+about `asyncio` and `await`, please see the 
+[Python `asyncio` documentation](https://docs.python.org/3/library/asyncio.html)).
+
+## Quick Start
+
+You will need valid credentials on a Vantiq server in the form of a
+username and password or access token.  If you have a private Vantiq server,
+contact your administrator for credentials.  If you wish to use the
+Vantiq public cloud, contact [support@vantiq.com](mailto:support@vantiq.com).
+
+The first step is to create an instance of the Vantiq SDK providing the URL of the Vantiq server to connect:
+
+```python
+from vantiqsdk import Vantiq, VantiqResources, VantiqResponse
+import vantiqsdk
+
+server: str = "https://dev.vantiq.com"
+
+vantiq: Vantiq = Vantiq(server)
+```
+
+where `server` is the full URL for the Vantiq server to connect to, such as *https://dev.vantiq.com/*. 
+An optional second argument is the version of the API to connect to. 
+If not specified, this defaults to the latest version, currently *1*. 
+At this point, the *Vantiq* instance has not yet connected to the server.  
+To establish a connection to the server, use the `authenticate` method, e.g.,
+
+```python
+username = "joe@user"
+password = "my-secr3t-passw0rd!#!"
+
+await vantiq.authenticate(username, password)
+```
+
+The `username` and `password` are the same credentials used to log into the system.
+Note the username and password are not stored either in-memory or persistently after
+this authentication call.  After successfully authenticating with the system,
+the *Vantiq* instance stores an in-memory access token that subsequent API calls
+will use.
+
+Now, you are able to perform any SDK calls to the Vantiq server.  The async methods
+on the SDK classes can be immediately awaited to run in, effectively, a synchronous
+fashion, or they can return an `Awaitable` that can be _awaited_ later.
+
+```python
+vr: VantiqResponse = await vantiq.select(VantiqResources.TYPES)
+
+```
+
+Alternatively,
+
+```python
+to_await = vantiq.select(VantiqResources.TYPES)
+...
+vr: VantiqResponse = await to_await
+```
+
+In either case, the response to the operation is available
+in the VantiqResponse instance.
+
+## Documentation
+
+For the full documentation on the SDK, see the
+[SDK API Reference](https://github.com/Vantiq/vantiq-python-sdk/blob/master/docs/api.md).
+
+## Developers
+
+The project is set up as a `gradle` project.  To run the tests, use
+
+```commandline
+./gradlew test
+```
+
+or
+
+```commandline
+./gradlew.bat test
+```
+
+in a windows environment.
+
+The tests run will run a mocked version. To execute tests against a _live_ server,
+define the following gradle properties in your ~/.gradle/gradle.properties file:
+
+```properties
+# Python project values
+TestVantiqServer=<Vantiq server url> # Only do the base URL. Ex http://localhost:8080/
+TestAccessToken=<access token from that Vantiq system>
+TestVantiqUsername=<Vantiq user name>
+TestVantiqPassword=<Password for that Vantiq user>
+```
+
+Alternatively, when running directly, use the following environment variables:
+
+```commandline
+VANTIQ_URL <Vantiq erver url>
+VANTIQ_ACCESS_TOKEN <Access token from that Vantiq system>
+VANTIQ_USERNAME <Vantiq user name>
+VANTIQ_PASSWORD <Password for that Vantiq user>
+```
+
+## Copyright and License
+
+Copyright &copy; 2022 Vantiq, Inc.  Code released under the
+[MIT license](https://github.com/Vantiq/vantiq-python-sdk/blob/master/LICENSE.txt).
```

### Comparing `vantiqsdk-1.3.1/src/main/python/vantiqsdk.py` & `vantiqsdk-1.3.2/src/main/python/vantiqsdk.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1516 +1,1527 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-"""Vantiq SDK for Python
-
-This module contains the Vantiq  SDK for the Python language.
-
-The SDK consists of the following
-    Vantiq -- this is a class handling the client's interaction with the Vantiq system
-    VantiqError -- structured errors returned from Vantiq
-    VantiqException -- Exception raised from Vantiq when necessary
-    VantiqResponse -- Structured response from Vantiq operations
-    VantiqResources -- Names for Vantiq resources that may be used in for Vantiq operations
-
-The Vantiq SDK is built atop the asyncio-based aiohttp. Consequently, operations marked as async must be awaited.
-See https://docs.python.org/3/library/asyncio.html for more details.
-"""
-
-__author__ = 'fhcarter'
-__copyright__ = "Copyright 2022, Vantiq, Inc."
-__license__ = "MIT License"
-__email__ = "support@vantiq.com"
-__all__ = ['Vantiq',
-           'VantiqResources',
-           'VantiqResponse',
-           'VantiqError',
-           'VantiqException'
-           ]
-
-import asyncio
-import base64
-import json
-import logging
-from logging import Logger
-from typing import Awaitable, Callable, List, Union, Dict
-
-import aiohttp
-import websockets
-
-_MIMETYPE_JSON = 'application/json'
-_MIMETYPE_TEXT_PREFIX = 'text/'
-_SYSTEM_PREFIX = 'system.'
-
-
-class _RestClient:
-    """A generic HTTP Rest client."""
-
-    def __init__(self, url: str) -> None:
-        self._url = url
-        self._con = None
-
-    def __str__(self):
-        return f'_RestClient for {self._url}'
-
-    def __repr__(self):
-        return f'_RestClient({self._url})'
-
-    async def __aenter__(self):
-        self._con = self.connect()
-        return self
-
-    async def __aexit__(self, exc_type, exc, tb):
-        await self._con.close()
-
-    async def connect(self):
-        # set trust_env to True to enable env variable settings for network proxy support
-        self._con = aiohttp.ClientSession(base_url=self._url, trust_env=True)
-
-    async def close(self):
-        await self._con.close()
-
-    async def request(
-        self,
-        method: str,
-        url: str,
-        query_param: dict = None,
-        headers: dict = None,
-        body: json = None,
-        data: any = None
-    ) -> (bool, aiohttp.ClientResponse):
-        assert isinstance(method, str)
-        assert isinstance(url, str)
-
-        method = method.upper()
-        assert method in ('GET', 'POST', 'PUT', 'DELETE')
-
-        headers = headers or {}
-        if data is None:
-            data = body
-
-        try:
-            if method == 'GET':
-                return await self._con.get(url, params=query_param, headers=headers)
-            elif method == 'POST':
-                return await self._con.post(url, params=query_param, headers=headers, data=data)
-            elif method == 'DELETE':
-                return await self._con.delete(url, params=query_param, headers=headers)
-            elif method == 'PUT':
-                return await self._con.put(url, params=query_param, headers=headers, data=data)
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.exception',
-                                  'Unexpected exception performing {0} against server {1},',
-                                  [method, self._url]) from e
-
-    async def download(self, url: str, headers: Union[dict, None]) -> aiohttp.ClientResponse:
-        return await self._con.get(url, headers=headers)
-
-    async def upload(self, url: str, headers: Union[dict, None], content_type: str, filename: Union[str, None] = None,
-                     doc_name: Union[str, None] = None,
-                     inmem: Union[str, bytes, bytearray, None] = None) -> aiohttp.ClientResponse:
-
-        # Note:  Without the quote_fields parameter, this FormData object will url-encode all the fields.
-        # This plays havoc with the file names we're using as document names.
-        data = aiohttp.FormData(quote_fields=False)
-        if doc_name is None:
-            doc_name = filename
-        if inmem:
-            data.add_field(name=filename, value=inmem, content_type=content_type, filename=doc_name)
-        else:
-            data.add_field(name=filename, value=open(filename, 'rb'), content_type=content_type, filename=doc_name)
-        return await self._con.post(url, headers=headers, data=data)
-
-
-class VantiqResources:
-    """Defines the set of Vantiq Resources
-
-    More details about these resources can be found in the Vantiq Resource Reference Guide.
-    """
-
-    ANALYTICS_MODELS = 'system.analyticsmodels'
-    AUDITS = 'system.audits'
-    CATALOGS = 'system.catalogs'
-    COLLABORATIONS = 'system.collaborations'
-    COLLABORATION_TYPES = 'system.collaborationtypes'
-    DOCUMENTS = 'system.documents'
-    IMAGES = 'system.images'
-    K8S_CLUSTERS = 'system.k8sclusters'
-    K8S_INSTALLATIONS = 'system.k8sinstallations'
-    LLMS = 'system.llms'
-    NAMESPACES = 'system.namespaces'
-    ORGANIZATIONS = 'system.organizations'
-    PROFILES = 'system.profiles'
-    PROJECTS = 'system.projects'
-    RULES = 'system.rules'
-    SCHEDULED_EVENTS = 'system.scheduledevents'
-    SECRETS = 'system.secrets'
-    SEMANTIC_INDEXES = 'system.semanticindexes'
-    SERVICES = 'system.services'
-    SITUATIONS = 'system.situations'
-    SOURCES = 'system.sources'
-    SOURCE_IMPLS = 'system.sourceimpls'
-    SUBSCRIPTIONS = 'system.subscriptions'
-    SYSTEM_MODELS = 'system.systemmodels'
-    TENSORFLOW_MODELS = 'system.tensorflowmodels'
-    TESTS = 'system.tests'
-    TEST_REPORTS = 'system.testreports'
-    TEST_SUITE_REPORTS = 'system.testsuitereports'
-    TEST_SUITES = 'system.testsuites'
-    TOKENS = 'system.tokens'
-    TOPICS = 'system.topics'
-    TRACKING_REGIONS = 'system.trackingRegions'
-    TYPES = 'system.types'
-    USERS = 'system.users'
-    VIDEOS = 'system.videos'
-
-    @staticmethod
-    def unqualified_name(qualified_name: str) -> Union[str, None]:
-        if qualified_name:
-            if qualified_name.startswith(_SYSTEM_PREFIX):
-                return qualified_name[len(_SYSTEM_PREFIX):]
-            else:
-                return qualified_name
-        else:
-            return qualified_name
-        # return qualified_name.removeprefix(_SYSTEM_PREFIX) if qualified_name is not None else None
-
-
-class VantiqError:
-    """Contains an error from the Vantiq system.
-
-    A VantiqError contains three (3) properties:
-        code (str) The short string identifying the error
-        message (sr) The message template for the errors
-        params (list) The parameters for the message template.
-
-    Message templates look and behave like strings for which the Python format() can supply values.
-    """
-
-    def __init__(self, code: str, message: str, params: list):
-        self.code = code
-        self.message = message
-        self.params = params
-
-    def __str__(self):
-        return f'VantiqError: code: {self.code}, message: {self.message}'
-
-    def __repr__(self):
-        return f'VantiqError(code={self.code}, message={self.message}, params={self.params})'
-
-
-class VantiqException(RuntimeError):
-    """Contains an exception from the Vantiq system.
-
-       A VantiqException is a RuntimeError and contains three (3) properties:
-           code (str) The short string identifying the error
-           message (sr) The message template for the errors
-           params (list) The parameters for the message template.
-
-       Message templates look and behave like strings for which the Python format() can supply values.
-       """
-
-    def __init__(self, code: str, message: str, params: list):
-        self.code = code
-        self.message = message
-        self.params = params
-        super().__init__(message.format(*params))
-
-    def __str__(self):
-        return f'VantiqException: code: {self.code}, message={self.message.format(*self.params)}'
-
-    def __repr__(self):
-        return f'VantiqException(code={self.code}, message={self.message}, params={self.params})'
-
-
-class VantiqResponse:
-    """A response from a Vantiq operation
-
-    A Vantiq response contains information returned from a Vantiq operation. This information is represented by the
-    following properties:
-        is_success (bool) Did the operation succeed
-        content_type (str) The content type of the message returned.  Usually 'application/json'.
-        count (int) Where applicable, the number of items returned for a successful operation.  This is generally
-                    available after a count() or delete() operation.
-        errors (list) A list of VantiqError entries outlining a failed operation
-        body (list or dict) The results of the operation.
-    """
-
-    def __init__(self, successful: bool, status_code: int, content_type: Union[str, None]):
-        self.status_code = status_code
-        self.content_type = content_type
-        self.is_success = successful
-        self.body = None
-        self.count: Union[int, None] = None
-        self.errors = None
-
-    def __str__(self):
-        ret_val = f'VantiqResponse: successful: {self.is_success}, status_code: {self.status_code}, ' \
-                  f'content_type:{self.content_type}, count: {self.count})'
-        if self.is_success:
-            if isinstance(self.body, list):
-                if not self.body:
-                    ret_val += '\n\t body: empty'
-                else:
-                    for item in self.body:
-                        ret_val += '\n\t body: ' + str(item)
-            elif isinstance(self.body, aiohttp.StreamReader):
-                ret_val += '\n\t body: <<streaming body>>'
-            elif self.body is not None:
-                ret_val += '\n\t body: ' + str(self.body)
-            else:
-                ret_val += '\n\t body: None'
-        else:
-            if self.errors:
-                for err in self.errors:
-                    ret_val += '\n\t Error: ' + str(err)
-        return ret_val
-
-    def __repr__(self):
-        return f'VantiqResponse(successful={self.is_success}, status_code={self.status_code}, ' \
-               f'content_type={self.content_type}) # count={self.count}, errors={self.errors}, ' \
-               f'body={self.body}'
-
-    @classmethod
-    def from_error(cls, err: VantiqError):
-        vr = cls(False, 400, None)
-        vr.errors = [err]
-        return vr
-
-    def _populate_count(self, resp: aiohttp.ClientResponse) -> None:
-        cnt = resp.headers.get('X-Total-Count')
-        if cnt is not None:
-            self.count = int(cnt)
-
-    async def _populate_body(self, resp: aiohttp.ClientResponse) -> None:
-        if self.content_type == _MIMETYPE_JSON:
-            self.body = await resp.json()
-        elif self.content_type and self.content_type.startswith(_MIMETYPE_TEXT_PREFIX):
-            self.body = await resp.text()
-        else:
-            # If we don't recognize the type, just return all the bytes
-            self.body = await resp.read()
-
-    def _populate_streaming_body(self, resp: aiohttp.ClientResponse) -> None:
-        self.body = resp.content
-
-    async def _populate_errors(self, resp: aiohttp.ClientResponse) -> None:
-        # noinspection PyBroadException
-        try:
-            if self.content_type == _MIMETYPE_JSON:
-                errors = await resp.json()
-                err_list = []
-                if isinstance(errors, list):
-                    for err in errors:
-                        if 'code' in err.keys():
-                            err_list.append(VantiqError(err['code'], err['message'], err['params']))
-                        elif 'error' in err.keys():
-                            err_list.append(VantiqError(str(resp.status), err['error'], []))
-                        else:
-                            err_list.append(VantiqError('io.vantiq.python.unknownerrorprops',
-                                                        'Received error in an unknown format: {0}',
-                                                        [err]))
-                elif isinstance(errors, dict):
-                    if 'code' in errors.keys():
-                        err_list.append(VantiqError(errors['code'], errors['message'], errors['params']))
-                    elif 'error' in errors.keys():
-                        err_list.append(VantiqError(str(resp.status), errors['error'], []))
-                    else:
-                        err_list.append(VantiqError('io.vantiq.python.unknownerrorprops',
-                                                    'Received error in an unknown format: {0}',
-                                                    [errors]))
-                else:
-                    err_list.append(VantiqError('io.vantiq.python.unknownerrorformat',
-                                                'Received error in an unknown format: {0}',
-                                                [errors]))
-                self.errors = err_list
-            else:
-                code = "io.vantiq.python.nonjson.error"
-                msg = await resp.text()
-                message = 'Status: {0}, non-json error: {1}'
-                params = [self.status_code, msg]
-                ve = VantiqError(code, message, params)
-                self.errors = [ve]
-        except Exception:
-            # noinspection PyBroadException
-            try:
-                unparseable = await resp.text()
-            except Exception:
-                # noinspection PyBroadException
-                try:
-                    unparseable = await resp.read()
-                except Exception:
-                    unparseable = 'unable to extract error information'
-            ve = VantiqError('io.vantiq.python.parse.exception',
-                             'Error parsing error messages: {0}',
-                             [unparseable])
-            self.errors = [ve]
-
-
-class Vantiq:
-    """The interface for working with the Vantiq System.
-
-    This class consists of operations that can be performed using the Vantiq system. More information about
-    these operations can be found in the Vantiq Resource Reference Guide and the Vantiq API Reference Guide.
-
-    Logging for this class is done through a standard Python logger named "Vantiq".  It is assumed that the
-    client of this library will configure the logger as desired.
-
-    The Vantiq object instance can be used as a context manager.
-        async with Vantiq(<server url>) as client:
-            resp: VantiqResponse = client.select(VantiqResource, ...)
-    for example.
-
-    As noted, most of the operations in the Vantiq object are `async` and must be awaited for them to run. See
-    https://docs.python.org/3/library/asyncio.html for more details about working with async operations.
-
-    """
-
-    def __init__(self, server: str, api_version: Union[str, None] = None):
-        """Create a Vantiq client object.
-
-        Parameters:
-            server : str
-                URL String at which to find the Vantiq Server
-
-            api_version : str (optional)
-                Version of the API to use. Defaults to '1'
-
-        Returns:
-            Vantiq client object with which to interact with the Vantiq system.
-
-        Can be used as a context manager
-
-        Examples:
-            As a context manager::
-            ::
-
-                async with Vantiq('https://dev.vantiq.com') as client:
-                    ...
-
-            or, in a client object:
-            ::
-                client = Vantiq('https://dev.vantiq.com')
-                ...
-                await client.close()
-
-
-        """
-        self._vlog: Logger = logging.getLogger(self.__class__.__name__)
-
-        if server.endswith('/'):
-            self._server = server[:-len('/')]  # server.removesuffix('/')'
-        else:
-            self._server = server
-        self._api_version = api_version if api_version else '1'
-        self._is_authenticated = False
-        self._username = None
-        self._target_namespace = None
-        self._access_token = None
-        self._id_token = None
-        self._auth_header = None
-        self._connection = None
-        self._is_connected = False
-        self._connection = _RestClient(self._server)
-        self._base_path = '/api/v' + self._api_version + '/'
-        self._subscriber: Union[_VantiqSubscriber, None] = None
-
-    def __str__(self):
-        return f'Vantiq connection to {self._server}, is_connected: {self._is_connected}, ' \
-               f'is_authenticated: {self._is_authenticated}'
-
-    def __repr__(self):
-        return f'Vantiq({self._server}, {self._api_version}) n# is_connected: {self._is_connected}, ' \
-               f'is_authenticated: {self._is_authenticated}'
-
-    async def __aenter__(self):
-        await self.connect()
-        return self
-
-    async def __aexit__(self, exc_type, exc, tb):
-        await self.close()
-
-    async def connect(self) -> None:
-        """Make the connection to the Vantiq server
-
-        Returns:
-            None
-        Raises:
-            VantiqException for connection issues
-
-        Notes:
-            Should precede the .authenticate().  Must be done before other operations.
-        """
-
-        if not self._is_connected:
-            await self._connection.connect()
-            self._is_connected = True
-            self._vlog.debug('Connected to server: %s', self._server)
-
-    def get_server(self):
-        """Returns the server url used for this connection."""
-        return self._server
-
-    def get_api_version(self):
-        """Returns the API version used for this connection."""
-        return self._api_version
-
-    async def set_access_token(self, access_token: str) -> None:
-        """Set the access token for server access.
-
-        Access to the Vantiq server is controlled.  Access can be granted by using an access token (recommended) or
-        a username and password.
-
-        Parameters:
-            access_token : str
-                Access token to be used to gain access to the Vantiq system
-        """
-        if not self._is_connected:
-            await self.connect()
-        self._access_token = access_token
-        self._auth_header = 'Bearer ' + self._access_token
-        self._is_authenticated = True  # We have an access token, we'll figure we're OK til we're not
-
-    def get_access_token(self) -> str:
-        """Returns the access token currently in use."""
-        return self._access_token
-
-    def set_target_namespace(self, namespace: Union[str, None]) -> None:
-        """Set the target namespace to be used to access the Vantiq server"""
-        self._target_namespace = namespace
-
-    def get_target_namespace(self) -> Union[str, None]:
-        """Returns the target namespace currently in use."""
-        return self._target_namespace
-
-    def set_username(self, username: str) -> None:
-        """Set the username to be used to access the Vantiq server"""
-        self._username = username
-
-    def get_username(self) -> str:
-        """Returns the username currently in use."""
-        return self._username
-
-    def get_id_token(self) -> str:
-        return self._id_token
-
-    def is_authenticated(self) -> bool:
-        """Returns a boolean indicating whether this Vantiq instance is authenticated."""
-        return self._is_authenticated
-
-    async def authenticate(self, username: str, password: str) -> None:
-        """(Async) Use a username and password to connect to the Vantiq system.
-
-        Parameters:
-            username : str
-                The username to be used to authenticate to the Vantiq server.
-            password : str
-                The password to be used to authenticate to the Vantiq server.
-
-        Returns:
-            Raises a VantiqException in case of failure.
-
-        Example:
-        ::
-            await client.authenticate('vantiquser', 'secret')
-        """
-        if not self._is_connected:
-            await self.connect()
-        b64 = base64.b64encode((username + ':' + password).encode('utf=8')).decode('utf-8')
-        headers = {aiohttp.hdrs.AUTHORIZATION: 'Basic ' + b64}
-        resp = await self._connection.request('GET', '/authenticate', headers=headers)
-        ret_val = VantiqResponse(resp.ok, resp.status, resp.content_type)
-        if not resp.ok:
-            # noinspection PyProtectedMember
-            await ret_val._populate_errors(resp)
-            self._vlog.error('Authentication to server %s failed: %s', self._server, resp)
-            raise VantiqException(resp.errors[0].code, resp.errors[0].message, resp.errors[0].params)
-        # noinspection PyProtectedMember
-        await ret_val._populate_body(resp)
-        self._access_token = ret_val.body['accessToken']
-        self._username = username
-        self._id_token = ret_val.body['idToken']
-        self._is_authenticated = True
-        self._auth_header = 'Bearer ' + self._access_token
-
-    async def refresh(self) -> None:
-        """(Async) Refresh the access token with the Vantiq Server."""
-        if self._is_authenticated:
-            path = '/authenticate/refresh'
-            headers = {aiohttp.hdrs.CONTENT_TYPE: 'text/plain'}
-            resp = await self._connection.request('POST', path, headers=headers, data=self._access_token)
-            ret_val = VantiqResponse(resp.ok, resp.status, resp.content_type)
-            if not resp.ok:
-                self._vlog.error('Authentication/refresh to server %s failed: %s', self._server, resp)
-                # noinspection PyProtectedMember
-                await ret_val._populate_errors(resp)
-                raise VantiqException(resp.errors[0].code, resp.errors[0].message, resp.errors[0].params)
-            # noinspection PyProtectedMember
-            await ret_val._populate_body(resp)
-            self._access_token = ret_val.body['accessToken']
-            self._id_token = ret_val.body['idToken']
-            self._is_authenticated = True
-            self._auth_header = 'Bearer ' + self._access_token
-        else:
-            raise VantiqException('io.vantiq.python.refreshnotauthenticated',
-                                  'Cannot refresh access token as this session is not authenticated.',
-                                  [])
-
-    async def close(self):
-        """(Async) End the Vantiq session"""
-        self._is_authenticated = False
-        self._access_token = None
-        self._id_token = None
-        self._base_path = None
-        self._auth_header = None
-        self._target_namespace = None
-        self._username = None
-        if self._subscriber:
-            await self._subscriber.close()
-            self._subscriber = None
-        if self._connection:
-            await self._connection.close()
-            self._connection = None
-
-    def _build_path(self, qualified_name: str, resource_id: Union[str, None], ext: Union[str, None] = None) -> str:
-        if qualified_name.startswith('system.'):
-            path = self._base_path + 'resources/' + qualified_name[len('system.'):]  # removeprefix(_SYSTEM_PREFIX)
-        else:
-            path = self._base_path + 'resources/custom/' + qualified_name
-
-        if resource_id:
-            path += '/' + resource_id
-        if ext:
-            path += '/' + ext
-
-        return path
-
-    @staticmethod
-    def _check_error(response: Union[dict, List[dict], None]):
-        if response:
-            code = None
-            message = None
-            params = None
-            if isinstance(response, list):
-                response = response[0]
-            if 'code' in response.keys():
-                code = response['code']
-                if 'message' in response.keys():
-                    message = response['message']
-                if 'params' in response.keys():
-                    params = response['params']
-            elif 'error' in response.keys():
-                message = response['error']
-                code = 'io.vantiq.python.error'
-                params = []
-            raise VantiqException(code, message, params)
-
-    def _get_auth_headers(self) -> dict:
-        headers = {aiohttp.hdrs.AUTHORIZATION: self._auth_header}
-        if self._target_namespace is not None:
-            headers['X-Target-Namespace'] = self._target_namespace
-        return headers
-
-    async def _perform_operation(self, operation: str, method: str, path: str,
-                                 query_params: Union[dict, None], is_streaming: bool,
-                                 instance: Union[dict, None] = None) -> VantiqResponse:
-        if self._is_authenticated:
-            try:
-                headers = self._get_auth_headers()
-                if instance is None:
-                    # When no parameters are passed at all, we get 404's back.  So None as parameters == {}.
-                    instance = {}
-
-                body = json.dumps(instance)
-                headers[aiohttp.hdrs.CONTENT_TYPE] = 'application/json'
-                resp: aiohttp.ClientResponse = await self._connection.request(method, path, headers=headers,
-                                                                              query_param=query_params, body=body)
-                ret_val = VantiqResponse(resp.ok, resp.status, resp.content_type)
-                if resp.ok:
-                    # noinspection PyProtectedMember
-                    ret_val._populate_count(resp)
-                    if is_streaming:
-                        # noinspection PyProtectedMember
-                        ret_val._populate_streaming_body(resp)
-                    else:
-                        # noinspection PyProtectedMember
-                        await ret_val._populate_body(resp)
-                else:
-                    # noinspection PyProtectedMember
-                    await ret_val._populate_errors(resp)
-                return ret_val
-            except Exception as e:
-                raise VantiqException('io.vantiq.python.operationerror',
-                                      'Unexpected error during {0} operation.',
-                                      [operation]) from e
-
-        else:
-            raise VantiqException('io.vantiq.python.request.notauthenticated',
-                                  'A {0} request was made on a session that is not connected.',
-                                  [operation])
-
-    async def select(self, resource: str,
-                     properties: Union[list, None] = None,
-                     where: Union[dict, None] = None,
-                     sort_spec: Union[dict, None] = None,
-                     limit: Union[int, None] = None,
-                     options: Union[dict, None] = None) -> VantiqResponse:
-        """(Async) Return items from a Vantiq resource.
-
-        Select specific items from a Vantiq resource. Selection and details of the return are controlled
-        by the following parameters:
-
-        Parameters:
-            resource : str
-                The name of the resource to be returned.  System resource names are provided via the VantiqResource
-                class.
-            properties : list(str)
-                (optional) The list of properties for the resource to be returned. If missing, return all properties.
-            where : dict(str: *)
-                (optional) The "where clause" to be used to restrict the selection.  The contents are defined
-                in the API Reference Guide.
-            sort_spec : dict(str: int)
-                (optional) Defines the sort order of the returned values.  The key value defines the property on which
-                to sort, and the value determines the order (1 = ascending, -1 = descending).  See the API Reference
-                Guide for details.
-            limit : int
-                (optional) Limit the number of records returned
-            options : dict (str, *)
-                (optional) Additional query parameter options
-        Returns:
-            VantiqResponse
-
-        Examples:
-        ::
-            vr: VantiqResponse = await client.select('myType')
-            if vr.is_success:
-                ...
-        """
-        operation = 'select'
-        try:
-            query_params = {}
-            if properties:
-                query_params['props'] = json.dumps(properties)
-            if where is not None:
-                query_params['where'] = json.dumps(where)
-            if sort_spec:
-                query_params['sort'] = json.dumps(sort_spec)
-            if limit is not None and limit > 0:
-                query_params['limit'] = limit
-                query_params['count'] = 'true'
-            if options:
-                for key, value in options.items():
-                    if isinstance(key, str) and isinstance(value, str):
-                        query_params[key] = value
-                    else:
-                        raise VantiqException('io.vantiq.python.option.stringsrequired',
-                                              'Options to queries must be of type str. ' +
-                                              'Found key {0}:{1} and value {2}:{3}.',
-                                              [key, type(key).__name__, value, type(value).__name__])
-            method = 'GET'
-            path = self._build_path(resource, None)
-            resp = await self._perform_operation(operation, method, path, query_params, False)
-            return resp
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operation.unexpectederror',
-                                  'Unexpected error during {0} operation.',
-                                  [operation]) from e
-
-    async def select_one(self, resource: str, resource_id: str = None) -> VantiqResponse:
-        """(Async) Select a single item from a Vantiq resource
-
-        Parameters:
-            resource : str
-                The name of the resource from which to select.
-            resource_id : str
-                The identifier for the specific item within the resource.
-        Returns:
-            VantiqResponse object
-
-        Example:
-        ::
-            vr: VantiqResponse = await client.selectOne('myType', 'type name')
-            if vr.is_success:
-                ....
-        """
-        operation = 'selectOne'
-        try:
-            method = 'GET'
-            query_params = {}
-            path = self._build_path(resource, resource_id)
-            resp = await self._perform_operation(operation, method, path, query_params, False)
-            return resp
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operation.unexpectederror',
-                                  'Unexpected error during {0} operation.',
-                                  [operation]) from e
-
-    async def delete(self, resource: str, where: Union[dict, None]) -> VantiqResponse:
-        """(Async) Delete item(s) from a Vantiq resource.
-
-        Parameters:
-            resource : str
-                The name of the Vantiq resource from which to delete items
-            where : dict (str: *)
-                The "where clause" to be used to determine which items to delete. The contents are defined
-                in the API Reference Guide.
-                Note that if where is None, this may delete all objects in the resource type.
-        Returns:
-            VantiqResponse.  The count property of the VantiqResponse will provide the number of objects deleted.
-
-        Examples:
-        ::
-           vr: VantiqResponse = await client.delete('myType', {'name': 'some name'}
-           if vr.is_success:
-              print('Count of items deleted: ', vr.count)
-        """
-
-        operation = 'delete'
-        try:
-            query_params = {'count': 'true'}
-            if where is not None:
-                query_params['where'] = json.dumps(where)
-            method = 'DELETE'
-            path = self._build_path(resource, None)
-            resp = await self._perform_operation(operation, method, path, query_params, False)
-            return resp
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operation.unexpectederror',
-                                  'Unexpected error during {0} operation.',
-                                  [operation]) from e
-
-    async def delete_one(self, resource: str, resource_id: str) -> VantiqResponse:
-        """(Async) Delete a single item from a resource.
-
-        Parameters:
-            resource : str
-                The name of the Vantiq resource from which to delete.
-            resource_id : str
-                The key for the item to delete.
-
-        Returns:
-            VantiqResponse indicating success of the operation
-
-        """
-        operation = 'delete'
-        try:
-            method = 'DELETE'
-            path = self._build_path(resource, resource_id)
-            resp = await self._perform_operation(operation, method, path, None, False)
-            return resp
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operation.unexpectederror',
-                                  'Unexpected error during {0} operation.',
-                                  [operation]) from e
-
-    async def insert(self, resource: str, instance: dict) -> VantiqResponse:
-        """(Async) Insert an item into Vantiq Resource.
-
-        Parameters:
-            resource : str
-                Name of the Vantiq resource into which to insert.
-            instance : dict
-                The values to be inserted.  The key names in the _instance_ parameter
-                must match the property names in the Vantiq object.
-
-        Returns:
-            VantiqResponse indicating success/failure of the operation and the value inserted.
-        """
-
-        if instance is None:
-            raise VantiqException('io.vantiq.python.insert.none',
-                                  'The object to be inserted cannot be None.', [])
-        operation = 'insert'
-        try:
-            method = 'POST'
-            path = self._build_path(resource, None)
-            resp = await self._perform_operation(operation, method, path, None, False, instance)
-            return resp
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operation.unexpectederror',
-                                  'Unexpected error during {0} operation.',
-                                  [operation]) from e
-
-    async def upsert(self, resource: str, instance: dict) -> VantiqResponse:
-        """(Async) Upsert an item into Vantiq Resource.
-
-            Parameters:
-                resource : str
-                    Name of the Vantiq resource into which to upsert.
-                instance : dict
-                    The values to be upserted.   The key names in the _instance_ parameter
-                    must match the property names in the Vantiq object.
-
-            Returns:
-                VantiqResponse indicating success/failure of the operation and the value upserted.
-        """
-
-        if instance is None:
-            raise VantiqException('io.vantiq.python.upsert.none',
-                                  'The object to be upserted cannot be None.', [])
-        operation = 'upsert'
-        try:
-            instance.pop('_id', None)
-            query_params = {'upsert': 'true'}
-            method = 'POST'
-            path = self._build_path(resource, None)
-            resp = await self._perform_operation(operation, method, path, query_params, False, instance)
-            return resp
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operation.unexpectederror',
-                                  'Unexpected error during {0} operation.',
-                                  [operation]) from e
-
-    async def update(self, resource: str, resource_id: str, instance: dict) -> VantiqResponse:
-        """(Async) Update an item in a  Vantiq Resource.
-
-            Parameters:
-                resource : str
-                    Name of the Vantiq resource in which to update.
-                resource_id : str
-                    The key of the record to look up for replacement.  The _id property can be used/
-                instance : dict
-                    The values to be updated. The key names in the _instance_ parameter
-                    must match the property names being updated in the Vantiq object.
-
-            Returns:
-                VantiqResponse indicating success/failure of the operation and the value updated.
-        """
-
-        if instance is None:
-            raise VantiqException('io.vantiq.python.upsert.none',
-                                  'The object to be upserted cannot be None.', [])
-        operation = 'update'
-        try:
-            instance.pop('_id', None)
-            query_params = {}
-            method = 'PUT'
-            path = self._build_path(resource, resource_id)
-            resp = await self._perform_operation(operation, method, path, query_params, False, instance)
-            return resp
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operation.unexpectederror',
-                                  'Unexpected error during {0} operation.',
-                                  [operation]) from e
-
-    async def download(self, path: str) -> VantiqResponse:
-        """(Async) Download content from a Vantiq Document, Image, Video, or TensorflowModel.
-
-        Parameters:
-            path : str
-                The path from which to obtain the data. This is found in the `content` field of the base object.
-
-        Returns:
-            VantiqResponse. In this case, the response's `body` field is an `aiohttp.StreamReader` that can be used
-            to fetch the content returned.
-
-        Examples:
-        ::
-            vr: VantiqResponse = await client.selectOne(VantiqResources.DOCUMENTS, 'mydoc')
-            mydoc = vr.body
-            if vr.is_success:
-                download_vr: VantiqResponse = await client.download(mydoc.content)
-                if download_vr.is_success:
-                    reader = download_vr.body
-                    while True:
-                        data = await reader.read(100)  # Read our data 100 bytes at a time
-                        if len(data) == 0:
-                            break
-                        # Do something with the data
-                        ...
-        """
-        url = path
-        headers = self._get_auth_headers()
-        try:
-            resp = await self._connection.download(url, headers)
-            ret_val = VantiqResponse(resp.ok, resp.status, resp.content_type)
-            # noinspection PyProtectedMember
-            ret_val._populate_count(resp)
-            # noinspection PyProtectedMember
-            ret_val._populate_streaming_body(resp)
-            return ret_val
-        except aiohttp.ClientPayloadError as cpe:
-            raise VantiqException('io,vantiq.python.downloaderror',
-                                  'Error encountered during download of {0}',
-                                  [path]) from cpe
-
-    async def upload(self, resource: str, content_type: str, filename: str,
-                     doc_name: Union[str, None] = None,
-                     inmem: Union[str, bytes, bytearray, None] = None) -> VantiqResponse:
-        """(Async) Upload a file (or in-memory data), creating an object to hold that data.
-
-        This allows the upload of a file to create a document, inage, video, or tensorflow model.
-
-        Parameters:
-            resource : str
-                The Vantiq resource type to create.
-            content_type : str
-                The type of data contained in the file.  This will be set as the `contentType` of the resulting
-                object.
-            filename : str
-                The name of the file to upload.
-            doc_name : str
-                (optional) The name of the object to create. If this is missing, use the filename.
-            inmem : str | bytes | bytearray
-                (optional) Content to be uploaded.  Used when the content is not in a file.
-
-        Returns:
-            VantiqResponse containing the object created.
-
-        Examples:
-        ::
-            vr: VantiqResponse = await client.upload(VantiqResources.DOCUMENTS, 'iamge/png', 'path/name.png')
-            if vr.is_success:
-                # Here, we will have uploaded a file named `path/name.png`,
-                # and created a Document named `path/name.png`.
-
-            vr: VantiqResponse = await client.upload(VantiqResource.DOCUMENTS, 'text/plain', None,
-                                                     'my document', 'some content for my document')
-            if vr.is_success:
-                # Here, we will have created a document named 'my document' with the content
-                # 'some content for my document'
-
-        """
-        ve = None
-        if content_type is None:
-            ve = VantiqError('io.vantiq.python.upload.contenttype',
-                             'Missing content type specification for an upload call().',
-                             [])
-        elif resource is None:
-            ve = VantiqError('io.vantiq.python.upload.resource',
-                             'The resource type is missing for an upload() call.',
-                             [])
-        elif filename is None and inmem is None:
-            ve = VantiqError('io.vantiq.python.content',
-                             'The filename and inmem parameters for an upload() call are both missing.',
-                             [])
-        elif filename and doc_name and inmem:
-            ve = VantiqError('io.vantiq.python.duplicatename',
-                             'When uploading in memory object, only one of filename or doc_name is permitted.',
-                             [])
-        elif filename is None and doc_name is None:
-            ve = VantiqError('io.vantiq.python.noname',
-                             'Neither a file name nor a document name was provided for an upload() call.',
-                             [])
-
-        if ve:
-            return VantiqResponse.from_error(ve)
-
-        path = self._build_path(resource, None)
-        headers = self._get_auth_headers()
-
-        try:
-            resp = await self._connection.upload(path, headers, content_type, filename, doc_name, inmem)
-            ret_val = VantiqResponse(resp.ok, resp.status, resp.content_type)
-            # noinspection PyProtectedMember
-            ret_val._populate_count(resp)
-            # noinspection PyProtectedMember
-            await ret_val._populate_body(resp)
-            return ret_val
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operationerror',
-                                  'Unexpected error during {0} operation.',
-                                  ['upload']) from e
-
-    async def count(self, resource: str, where: Union[dict, None] = None) -> VantiqResponse:
-        """(Async) Return the number of items in a Vantiq resource that satisfy the where clause
-
-        Parameters:
-            resource : str
-                The name of the resource to be counted.  System resource names are provided via the VantiqResource
-                class.
-            where : dict(str: *)
-                (optional) The "where clause" to be used to restrict the counting.  The where clause is defined
-                in the API Reference Guide.
-        Returns:
-            VantiqResponse where the `count` field contains the count requested.
-        """
-
-        operation = 'count'
-        try:
-            # Here, specify that we want the count but don't really care about the data.  So we'll limit
-            # the return to a single row & limit the properties returned
-            query_params = {'count': 'true', 'limit': 1}
-            if where is not None:
-                query_params['where'] = json.dumps(where)
-            props = ['_id']  # Since we don't care about the data, return the least we can
-            query_params['props'] = json.dumps(props)
-            method = 'GET'
-            path = self._build_path(resource, None)
-            resp = await self._perform_operation(operation, method, path, query_params, False)
-            resp.body = {}  # After a count, we don't need to return the data fetched (since we decided it anyway)
-            return resp
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operation.unexpectederror',
-                                  'Unexpected error during {0} operation.',
-                                  [operation]) from e
-
-    async def query(self, source_id: str, query: dict) -> VantiqResponse:
-        """(Async) Send a query message to a Vantiq source
-
-        Parameters:
-            source_id : str
-                Name of the source to which to send the query
-            query : dict
-                The message describing the query to be sent.  These messages are source specific.
-
-        Returns:
-            VantiqResponse indicating the success or failure of the query.  The body field will contain the results
-            of the query (if applicable).
-        """
-
-        operation = 'query'
-        try:
-            query_params = {}
-            method = 'POST'
-            path = self._build_path(VantiqResources.SOURCES, source_id, 'query')
-            resp = await self._perform_operation(operation, method, path, query_params, False, query)
-            return resp
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operation.unexpectederror',
-                                  'Unexpected error during {0} operation.',
-                                  [operation]) from e
-
-    async def execute(self, procedure_id: str, params: dict) -> VantiqResponse:
-        """(Async) Execute a Vantiq procedure.
-
-        Parameters:
-            procedure_id : str
-                The name of the procedure to execute.
-            params : dict
-                The parameters provided for the procedure's execution.  The key names are the parameter names,
-                and the values their values.
-        Returns:
-            VantiqResponse where the body contains the results of the procedure execution, if any.
-
-        """
-
-        operation = 'execute'
-        try:
-            query_params = {}
-            method = 'POST'
-            path = self._build_path(_SYSTEM_PREFIX + 'procedures', procedure_id)
-            resp = await self._perform_operation(operation, method, path, query_params, False, params)
-            return resp
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operation.unexpectederror',
-                                  'Unexpected error during {0} operation.',
-                                  [operation]) from e
-
-    async def publish(self, resource: str, resource_id: str, msg: dict) -> VantiqResponse:
-        """(Async) Publish a message to a Vantiq Service (event), Source, or Topic.
-
-        Parameters:
-            resource : str
-                The resource to which to publish.  Must be either VantiqResources.SERVICES, VantiqResources.SOURCES,
-                or VantiqResources.TOPICS.
-            resource_id : str
-                The specific service, source, or topic to which to publish. If the resource is VantiqResources.SERVICES,
-                the resource_id will take the form 'service_name/event_name.  This event should be defined as one of
-                the inbound events for the service in question.
-            msg : dict
-                The message to publish
-        Returns:
-            VantiqResponse
-
-        """
-
-        operation = 'publish'
-        if resource not in [VantiqResources.SOURCES, VantiqResources.TOPICS, VantiqResources.SERVICES]:
-            err = VantiqError('io.vantiq.python.publish.invalidresource',
-                              'The publish operation can be performed only on the following resources: {0}',
-                              [[VantiqResources.SERVICES, VantiqResources.SOURCES, VantiqResources.TOPICS]])
-            return VantiqResponse.from_error(err)
-        try:
-            query_params = {}
-            method = 'POST'
-            path = self._build_path(resource, resource_id)
-            resp = await self._perform_operation(operation, method, path, query_params, False, msg)
-            return resp
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operation.unexpectederror',
-                                  'Unexpected error during {0} operation.',
-                                  [operation]) from e
-
-    async def get_namespace_users(self, namespace: str) -> VantiqResponse:
-        """(Async) Returns a JsonArray containing objects which map between "username" and "preferredUsername"
-
-        Parameters:
-            namespace : str
-                The name of the namespace from which to get the list of users.
-        Returns:
-            VantiqResponse
-     """
-        operation = 'getNamespaceUsers'
-        try:
-            query_params = {}
-            method = 'GET'
-            path = self._build_path(VantiqResources.NAMESPACES, namespace, 'authorizedUsers')
-            resp = await self._perform_operation(operation, method, path, query_params, False)
-            return resp
-        except VantiqException:
-            # If we've already handled or wrapped it, just pass it along
-            raise
-        except Exception as e:
-            raise VantiqException('io.vantiq.python.operation.unexpectederror',
-                                  'Unexpected error during {0} operation.',
-                                  [operation]) from e
-
-    async def start_subscriber_transport(self):
-        """(Async) Start a task to handle subscriptions.
-
-        To handle incoming messages from the Vantiq server that arise from subscriptions, you must start an
-        asyncio task to do this work.  This method does that work.
-
-        If the transport does not exist when subscribe() is called, subscribe() will start
-        the transport on your behalf.
-
-        Parameters:
-            (none)
-        Returns:
-            The task created. Can be used to wait or manage that task.
-            If the subscriber connection already exists, None is returned as there is no new task.
-
-        """
-
-        if self._subscriber is None:
-            self._subscriber = _VantiqSubscriber(self)
-            task = asyncio.create_task(self._subscriber.connect())
-            failure_reason = None
-            try:
-                if self._subscriber.connected_future:
-                    await self._subscriber.connected_future
-            except Exception as e:
-                failure_reason = e
-            if not failure_reason:
-                failure_reason = self._subscriber.connected_future.exception()
-            if not failure_reason:
-                failure_reason = self._subscriber.connected_future.result()
-            if failure_reason != 'OK':
-                await self._subscriber.close()
-                self._subscriber = None
-                await task
-                if isinstance(failure_reason, Exception):
-                    raise VantiqException('io.vantiq.python.subtransport.exception',
-                                          'Failed to start subscriber transport: {0}',
-                                          [failure_reason]) from failure_reason
-                else:
-                    raise VantiqException('io.vantiq.python.subtransport.failed',
-                                          'Failed to start subscriber transport: {0}',
-                                          [failure_reason])
-            return task
-        else:
-            return None
-
-    async def subscribe(self, resource: str, resource_id: str, operation: Union[str, None],
-                        callback: Callable[[str, dict], Awaitable[None]], params: Union[dict, None] = None,
-                        target_namespace: Union[str, None] = None) -> VantiqResponse:
-        """(Async) Subscribe to an event from the Vantiq server.
-
-        Subscribes to a specific topic, source, service, or type event.
-
-        For sources, this will subscribe to message arrival events.  The name of the
-        source is required (e.g. "MySource").
-
-        For topics, this will subscribe to any messages published on that topic.  The
-        name of the topic is required (e.g. "/some/topic").
-
-        For services, this will subscribe to any messages published to the named service event. The name of the
-        service and service event is required, and should be passed into the resource id as service_name/event_name.
-
-        For types, this will subscribe to the specified type event.  The name of the
-        type and the operation (i.e. "insert", "update", or "delete") are required.
-
-        Parameters:
-            resource : str
-                The resource type for which this subscription is being made
-            resource_id : str
-                The identifier of the specific instance of the `resource` in question.
-            operation : str
-                The operation to which to subscribe when subscribing to a VantiqResources.TYPES event. Should be None
-                for other resource types.
-            callback : Callable[[str, dict], Awaitable[None]]
-                A callback function to call when a subscribed event arrives. The callback will be called with the
-                type of the callback ('connect', 'message', 'error') and the message contents.
-
-                The callback message contains the following properties:
-                    status : int -- the status of the event
-                    contentType : str -- the content type of the message
-                    path : str -- the event specification
-                    value : dict -- the value of the event (type inserted, topic contents, etc.)
-
-            params : dict
-                (optional) Parameters for the subscription. May be subscription dependent, but can usually be ignored.
-        Returns:
-            VantiqResponse indicating the success of the operation.
-
-        For details, see the Vantiq API Reference Guide.
-        """
-
-        if VantiqResources.TOPICS == resource:
-            path = "/" + resource[len(_SYSTEM_PREFIX):] + resource_id  # .removeprefix(_SYSTEM_PREFIX) + resource_id
-        else:
-            path = "/" + resource[len(_SYSTEM_PREFIX):] + '/' + resource_id  # .removeprefix(_SYSTEM_PREFIX) ...
-        if resource in [VantiqResources.SERVICES, VantiqResources.SOURCES, VantiqResources.TOPICS]:
-            if operation:
-                raise VantiqException('io.vantiq.python.operationillegal',
-                                      "Operation only support for {0}",
-                                      [VantiqResources.TYPES])
-        elif VantiqResources.TYPES == resource:
-            if operation is None:
-                raise VantiqException('io.vantiq.python.operationrequired',
-                                      "Operation required for {0}",
-                                      [VantiqResources.TYPES])
-
-            path += "/" + operation.lower()
-        else:
-            raise VantiqException('io.vantiq.python.invalidsubscribetype',
-                                  "Only 'topics', 'sources', 'services', and 'types' support subscribe",
-                                  [])
-
-        if self._subscriber is None:
-            await self.start_subscriber_transport()
-
-        vr = await self._subscriber.subscribe(path, params, callback, target_namespace)
-        return vr
-
-    async def ack(self, request_id: str, subscription_id: str, msg: dict) -> None:
-        """ Acknowledge the receipt of a reliable message
-
-        Parameters:
-            request_id : str
-                id of the request -- this can be found in the 'X-Request_id' header of the callback for the subscription
-            subscription_id : str
-                id of the subscription that delivered the message -- this is found in the [body][name] field of the
-                callback for the subscription message.
-            msg : dict
-                message being acknowledged
-        Raises:
-            VantiqException
-        """
-        if 'partitionId' not in msg.keys():
-            raise VantiqException('io.vantiq.python.ack.nopartitionid',
-                                  'The message being acknowledged contains no partition_id.',
-                                  [])
-        elif 'sequenceId' not in msg.keys():
-            raise VantiqException('io.vantiq.python.ack.nosequenceid',
-                                  'The message being acknowledged contains no sequence_id.',
-                                  [])
-
-        sequence_id = msg['sequenceId']
-        partition_id = msg['partitionId']
-        await self._subscriber.ack(request_id, subscription_id, sequence_id, partition_id)
-        return
-
-    def register_subscriber_on_close(self, callback: Callable[[], Awaitable[None]]):
-        """ Register a callback to be called when the subscriber is closed.
-
-        Parameters:
-            callback : Callable[[], Awaitable[None]]
-                The callback to be called when the subscriber is closed.
-        """
-        self._subscriber.on_close_handler = callback
-
-
-class _VantiqSubscriber:
-    CONNECT = 'connect'
-    MESSAGE = 'message'
-    ERROR = 'error'
-
-    def __init__(self, parent: Vantiq):
-        self.parent: Vantiq = parent
-        self.connected = False
-        self.connected_future: asyncio.Future = asyncio.get_running_loop().create_future()
-        self.connection: websockets.ClientProtocol = None
-        self.url = None
-        self._vlog = logging.getLogger(self.__class__.__name__)
-        self.subscriptions: Dict[str, bool] = {}
-        self.callbacks: Dict[str, Callable[[str, dict], Awaitable[None]]] = {}
-        self.is_authenticated = False
-        self.on_close_handler: Callable[[], Awaitable[None]] = None
-
-    def __str__(self):
-        ret_val = f'VantiqSubscriber for {str(self.parent)}'
-        if self.subscriptions:
-            for key, value in self.subscriptions.items():
-                ret_val += '\n\t' + key + ': ' + str(value)
-        return ret_val
-
-    def __repr__(self):
-        return f'VantiqSubscriber(repr({self.parent}))'
-
-    async def connect(self, do_pings: bool = True):
-        if self.parent is None or not self.parent.is_authenticated():
-            ve = VantiqException('io.vantiq.python.subscriber.notauthenticated',
-                                 'Attempt to connect subscriber when parent was not authenticated.',
-                                 [])
-            self.connected_future.set_exception(ve)
-            raise ve
-
-        if not self.connected:
-            self.url = self.parent.get_server().replace("http", "ws") + "/api/v" + self.parent.get_api_version() + \
-                  "/wsock/websocket"
-            async with websockets.connect(uri=self.url,
-                                          ping_interval=20 if do_pings else None,
-                                          ping_timeout=20 if do_pings else None) as websocket:
-                if not self.connected:
-                    auth_msg = {
-                        'op': 'validate',
-                        'resourceName': 'system.credentials',
-                        'object': self.parent.get_access_token()
-                    }
-                    await websocket.send(json.dumps(auth_msg))
-
-                async for raw in websocket:
-
-                    resp = json.loads(raw)
-                    request_id = None
-                    if 'headers' in resp.keys():
-                        hdrs = resp['headers']
-                        if 'X-Request-Id' in hdrs.keys():
-                            request_id = hdrs['X-Request-Id']
-                    else:
-                        pass
-
-                    # Using request id, track back to request for which this is a response
-
-                    if 'status' in resp.keys():
-                        if resp['status'] == 200:
-                            if not self.is_authenticated:
-                                self.connection = websocket
-                                self.connected = True
-                                self.is_authenticated = True
-                                self.connected_future.set_result('OK')
-                                self._vlog.debug('Authentication completed.')
-                            else:
-                                if request_id:
-                                    if request_id in self.subscriptions.keys():
-                                        if not self.subscriptions[request_id]:
-                                            # Then this is our response for our subscription.
-                                            self.subscriptions[request_id] = True
-                                            self._vlog.debug('Subscription requested accepted.')
-                                            callback = self.callbacks[request_id]
-                                            await callback(self.CONNECT, resp)
-                                        elif request_id in self.callbacks.keys():
-                                            callback = self.callbacks[request_id]
-                                            body = resp.get('body', None)
-                                            if body is not None and body.get('op', None) == 'unsubscribe':
-                                                self.subscriptions.pop(request_id)
-                                                self.callbacks.pop(request_id)
-                                            await callback(self.MESSAGE, resp)
-                        elif resp['status'] >= 400:
-                            if not self.connected:
-                                self._vlog.error('Connect call failed: %s :: %s:%s', resp['status'],
-                                                 resp['body'][0]['code'], resp['body'][0]['message'])
-                                ve = VantiqException('io.vantiq.python.connect.failed',
-                                                     'Connect call failed: {0} :: {1}:{2}',
-                                                     [resp['status'], resp['body'][0]['code'],
-                                                      resp['body'][0]['message']])
-                                self.connected_future.set_exception(ve)
-                                raise ve
-                            else:
-                                if request_id and request_id in self.callbacks.keys():
-                                    callback = self.callbacks[request_id]
-                                    await callback(self.ERROR, resp)
-                        elif resp['status'] == 100:
-                            if request_id and request_id in self.callbacks.keys():
-                                self._vlog.debug('Message received via subscription.')
-                                callback = self.callbacks[request_id]
-                                await callback(self.MESSAGE, resp)
-
-            # Once we get here, any transient subscriptions will be gone, so we should reset our side as well
-            await self.unsubscribe_all()
-
-    async def subscribe(self, path: str, params: dict, callback: Callable[[str, dict], Awaitable[None]],
-                        target_namespace: Union[str, None] = None) -> VantiqResponse:
-        if self.connected:
-            if path in self.subscriptions.keys():
-                vr = VantiqResponse(False, 400, None)
-                ve = VantiqError('io.vantiq.python.subscribed',
-                                 'A subscription for path {0} already exists.',
-                                 [path])
-                vr.errors = [ve]
-                return vr
-            self.callbacks[path] = callback
-            self.subscriptions[path] = False  # Will be set to true when the server responds
-            if params is None:
-                params = {}
-            params['requestId'] = path
-            sub_msg = {'op': 'subscribe',
-                       'resourceName': 'events',
-                       'resourceId': path,
-                       'parameters': params}
-            target_namespace = target_namespace or self.parent.get_target_namespace()
-            if target_namespace is not None:
-                sub_msg['targetNamespace'] = target_namespace
-            await self.connection.send(json.dumps(sub_msg))
-            self._vlog.debug('Subscription request sent.')
-
-            vr = VantiqResponse(True, 204, None)
-            return vr
-        else:
-            self._vlog.error('No transport for subscriptions established.')
-            vr = VantiqResponse(False, 400, None)
-            ve = VantiqError('io.vantiq.python.notransport',
-                             'No transport for subscriptions has been established.',
-                             [])
-            vr.errors = [ve]
-            return vr
-
-    async def ack(self, request_id: str, subscription_id: str, sequence_id: float, partition_id: float):
-        params = {'requestId': request_id,
-                  'subscriptionName': subscription_id, 'sequenceId': sequence_id, 'partitionId': partition_id}
-        msg = {'op': 'acknowledge', 'resourceName': 'events', 'resourceId': request_id,
-               'parameters': params}
-        if self.parent.get_target_namespace() is not None:
-            msg['targetNamespace'] = self.parent.get_target_namespace()
-        raw = json.dumps(msg)
-        await self.connection.send(raw)
-
-    async def unsubscribe_all(self):
-        await self.close()
-        self.subscriptions = {}
-        self.callbacks = {}
-
-    async def close(self):
-        self.connected = False
-        await self.connection.close()
-        self.connection = None
-        self.is_authenticated = False
-        if self.on_close_handler is not None:
-            await self.on_close_handler()
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+"""Vantiq SDK for Python
+
+This module contains the Vantiq  SDK for the Python language.
+
+The SDK consists of the following
+    Vantiq -- this is a class handling the client's interaction with the Vantiq system
+    VantiqError -- structured errors returned from Vantiq
+    VantiqException -- Exception raised from Vantiq when necessary
+    VantiqResponse -- Structured response from Vantiq operations
+    VantiqResources -- Names for Vantiq resources that may be used in for Vantiq operations
+
+The Vantiq SDK is built atop the asyncio-based aiohttp. Consequently, operations marked as async must be awaited.
+See https://docs.python.org/3/library/asyncio.html for more details.
+"""
+
+__author__ = 'fhcarter'
+__copyright__ = "Copyright 2022, Vantiq, Inc."
+__license__ = "MIT License"
+__email__ = "support@vantiq.com"
+__all__ = ['Vantiq',
+           'VantiqResources',
+           'VantiqResponse',
+           'VantiqError',
+           'VantiqException'
+           ]
+
+import asyncio
+import base64
+import json
+import logging
+from logging import Logger
+from typing import Awaitable, Callable, List, Union, Dict
+
+import aiohttp
+import websockets
+
+_MIMETYPE_JSON = 'application/json'
+_MIMETYPE_TEXT_PREFIX = 'text/'
+_SYSTEM_PREFIX = 'system.'
+
+
+class _RestClient:
+    """A generic HTTP Rest client."""
+
+    def __init__(self, url: str) -> None:
+        self._url = url
+        self._con = None
+
+    def __str__(self):
+        return f'_RestClient for {self._url}'
+
+    def __repr__(self):
+        return f'_RestClient({self._url})'
+
+    async def __aenter__(self):
+        self._con = self.connect()
+        return self
+
+    async def __aexit__(self, exc_type, exc, tb):
+        await self._con.close()
+
+    async def connect(self):
+        # set trust_env to True to enable env variable settings for network proxy support
+        self._con = aiohttp.ClientSession(base_url=self._url, trust_env=True)
+
+    async def close(self):
+        await self._con.close()
+
+    async def request(
+        self,
+        method: str,
+        url: str,
+        query_param: dict = None,
+        headers: dict = None,
+        body: json = None,
+        data: any = None
+    ) -> (bool, aiohttp.ClientResponse):
+        assert isinstance(method, str)
+        assert isinstance(url, str)
+
+        method = method.upper()
+        assert method in ('GET', 'POST', 'PUT', 'DELETE')
+
+        headers = headers or {}
+        if data is None:
+            data = body
+
+        try:
+            if method == 'GET':
+                return await self._con.get(url, params=query_param, headers=headers)
+            elif method == 'POST':
+                return await self._con.post(url, params=query_param, headers=headers, data=data)
+            elif method == 'DELETE':
+                return await self._con.delete(url, params=query_param, headers=headers)
+            elif method == 'PUT':
+                return await self._con.put(url, params=query_param, headers=headers, data=data)
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.exception',
+                                  'Unexpected exception performing {0} against server {1},',
+                                  [method, self._url]) from e
+
+    async def download(self, url: str, headers: Union[dict, None]) -> aiohttp.ClientResponse:
+        return await self._con.get(url, headers=headers)
+
+    async def upload(self, url: str, headers: Union[dict, None], content_type: str, filename: Union[str, None] = None,
+                     doc_name: Union[str, None] = None,
+                     inmem: Union[str, bytes, bytearray, None] = None) -> aiohttp.ClientResponse:
+
+        # Note:  Without the quote_fields parameter, this FormData object will url-encode all the fields.
+        # This plays havoc with the file names we're using as document names.
+        data = aiohttp.FormData(quote_fields=False)
+        if doc_name is None:
+            doc_name = filename
+        if inmem:
+            data.add_field(name=filename, value=inmem, content_type=content_type, filename=doc_name)
+        else:
+            data.add_field(name=filename, value=open(filename, 'rb'), content_type=content_type, filename=doc_name)
+        return await self._con.post(url, headers=headers, data=data)
+
+
+class VantiqResources:
+    """Defines the set of Vantiq Resources
+
+    More details about these resources can be found in the Vantiq Resource Reference Guide.
+    """
+
+    ANALYTICS_MODELS = 'system.analyticsmodels'
+    AUDITS = 'system.audits'
+    CATALOGS = 'system.catalogs'
+    COLLABORATIONS = 'system.collaborations'
+    COLLABORATION_TYPES = 'system.collaborationtypes'
+    DOCUMENTS = 'system.documents'
+    IMAGES = 'system.images'
+    K8S_CLUSTERS = 'system.k8sclusters'
+    K8S_INSTALLATIONS = 'system.k8sinstallations'
+    LLMS = 'system.llms'
+    NAMESPACES = 'system.namespaces'
+    ORGANIZATIONS = 'system.organizations'
+    PROFILES = 'system.profiles'
+    PROJECTS = 'system.projects'
+    RULES = 'system.rules'
+    SCHEDULED_EVENTS = 'system.scheduledevents'
+    SECRETS = 'system.secrets'
+    SEMANTIC_INDEXES = 'system.semanticindexes'
+    SERVICES = 'system.services'
+    SITUATIONS = 'system.situations'
+    SOURCES = 'system.sources'
+    SOURCE_IMPLS = 'system.sourceimpls'
+    SUBSCRIPTIONS = 'system.subscriptions'
+    SYSTEM_MODELS = 'system.systemmodels'
+    TENSORFLOW_MODELS = 'system.tensorflowmodels'
+    TESTS = 'system.tests'
+    TEST_REPORTS = 'system.testreports'
+    TEST_SUITE_REPORTS = 'system.testsuitereports'
+    TEST_SUITES = 'system.testsuites'
+    TOKENS = 'system.tokens'
+    TOPICS = 'system.topics'
+    TRACKING_REGIONS = 'system.trackingRegions'
+    TYPES = 'system.types'
+    USERS = 'system.users'
+    VIDEOS = 'system.videos'
+
+    @staticmethod
+    def unqualified_name(qualified_name: str) -> Union[str, None]:
+        if qualified_name:
+            if qualified_name.startswith(_SYSTEM_PREFIX):
+                return qualified_name[len(_SYSTEM_PREFIX):]
+            else:
+                return qualified_name
+        else:
+            return qualified_name
+        # return qualified_name.removeprefix(_SYSTEM_PREFIX) if qualified_name is not None else None
+
+
+class VantiqError:
+    """Contains an error from the Vantiq system.
+
+    A VantiqError contains three (3) properties:
+        code (str) The short string identifying the error
+        message (sr) The message template for the errors
+        params (list) The parameters for the message template.
+
+    Message templates look and behave like strings for which the Python format() can supply values.
+    """
+
+    def __init__(self, code: str, message: str, params: list):
+        self.code = code
+        self.message = message
+        self.params = params
+
+    def __str__(self):
+        return f'VantiqError: code: {self.code}, message: {self.message}'
+
+    def __repr__(self):
+        return f'VantiqError(code={self.code}, message={self.message}, params={self.params})'
+
+
+class VantiqException(RuntimeError):
+    """Contains an exception from the Vantiq system.
+
+       A VantiqException is a RuntimeError and contains three (3) properties:
+           code (str) The short string identifying the error
+           message (sr) The message template for the errors
+           params (list) The parameters for the message template.
+
+       Message templates look and behave like strings for which the Python format() can supply values.
+       """
+
+    def __init__(self, code: str, message: str, params: list):
+        self.code = code
+        self.message = message
+        self.params = params
+        super().__init__(message.format(*params))
+
+    def __str__(self):
+        return f'VantiqException: code: {self.code}, message={self.message.format(*self.params)}'
+
+    def __repr__(self):
+        return f'VantiqException(code={self.code}, message={self.message}, params={self.params})'
+
+
+class VantiqResponse:
+    """A response from a Vantiq operation
+
+    A Vantiq response contains information returned from a Vantiq operation. This information is represented by the
+    following properties:
+        is_success (bool) Did the operation succeed
+        content_type (str) The content type of the message returned.  Usually 'application/json'.
+        count (int) Where applicable, the number of items returned for a successful operation.  This is generally
+                    available after a count() or delete() operation.
+        errors (list) A list of VantiqError entries outlining a failed operation
+        body (list or dict) The results of the operation.
+    """
+
+    def __init__(self, successful: bool, status_code: int, content_type: Union[str, None]):
+        self.status_code = status_code
+        self.content_type = content_type
+        self.is_success = successful
+        self.body = None
+        self.count: Union[int, None] = None
+        self.errors = None
+
+    def __str__(self):
+        ret_val = f'VantiqResponse: successful: {self.is_success}, status_code: {self.status_code}, ' \
+                  f'content_type:{self.content_type}, count: {self.count})'
+        if self.is_success:
+            if isinstance(self.body, list):
+                if not self.body:
+                    ret_val += '\n\t body: empty'
+                else:
+                    for item in self.body:
+                        ret_val += '\n\t body: ' + str(item)
+            elif isinstance(self.body, aiohttp.StreamReader):
+                ret_val += '\n\t body: <<streaming body>>'
+            elif self.body is not None:
+                ret_val += '\n\t body: ' + str(self.body)
+            else:
+                ret_val += '\n\t body: None'
+        else:
+            if self.errors:
+                for err in self.errors:
+                    ret_val += '\n\t Error: ' + str(err)
+        return ret_val
+
+    def __repr__(self):
+        return f'VantiqResponse(successful={self.is_success}, status_code={self.status_code}, ' \
+               f'content_type={self.content_type}) # count={self.count}, errors={self.errors}, ' \
+               f'body={self.body}'
+
+    @classmethod
+    def from_error(cls, err: VantiqError):
+        vr = cls(False, 400, None)
+        vr.errors = [err]
+        return vr
+
+    def _populate_count(self, resp: aiohttp.ClientResponse) -> None:
+        cnt = resp.headers.get('X-Total-Count')
+        if cnt is not None:
+            self.count = int(cnt)
+
+    async def _populate_body(self, resp: aiohttp.ClientResponse) -> None:
+        if self.content_type == _MIMETYPE_JSON:
+            self.body = await resp.json()
+        elif self.content_type and self.content_type.startswith(_MIMETYPE_TEXT_PREFIX):
+            self.body = await resp.text()
+        else:
+            # If we don't recognize the type, just return all the bytes
+            self.body = await resp.read()
+
+    def _populate_streaming_body(self, resp: aiohttp.ClientResponse) -> None:
+        self.body = resp.content
+
+    async def _populate_errors(self, resp: aiohttp.ClientResponse) -> None:
+        # noinspection PyBroadException
+        try:
+            if self.content_type == _MIMETYPE_JSON:
+                errors = await resp.json()
+                err_list = []
+                if isinstance(errors, list):
+                    for err in errors:
+                        if 'code' in err.keys():
+                            err_list.append(VantiqError(err['code'], err['message'], err['params']))
+                        elif 'error' in err.keys():
+                            err_list.append(VantiqError(str(resp.status), err['error'], []))
+                        else:
+                            err_list.append(VantiqError('io.vantiq.python.unknownerrorprops',
+                                                        'Received error in an unknown format: {0}',
+                                                        [err]))
+                elif isinstance(errors, dict):
+                    if 'code' in errors.keys():
+                        err_list.append(VantiqError(errors['code'], errors['message'], errors['params']))
+                    elif 'error' in errors.keys():
+                        err_list.append(VantiqError(str(resp.status), errors['error'], []))
+                    else:
+                        err_list.append(VantiqError('io.vantiq.python.unknownerrorprops',
+                                                    'Received error in an unknown format: {0}',
+                                                    [errors]))
+                else:
+                    err_list.append(VantiqError('io.vantiq.python.unknownerrorformat',
+                                                'Received error in an unknown format: {0}',
+                                                [errors]))
+                self.errors = err_list
+            else:
+                code = "io.vantiq.python.nonjson.error"
+                msg = await resp.text()
+                message = 'Status: {0}, non-json error: {1}'
+                params = [self.status_code, msg]
+                ve = VantiqError(code, message, params)
+                self.errors = [ve]
+        except Exception:
+            # noinspection PyBroadException
+            try:
+                unparseable = await resp.text()
+            except Exception:
+                # noinspection PyBroadException
+                try:
+                    unparseable = await resp.read()
+                except Exception:
+                    unparseable = 'unable to extract error information'
+            ve = VantiqError('io.vantiq.python.parse.exception',
+                             'Error parsing error messages: {0}',
+                             [unparseable])
+            self.errors = [ve]
+
+
+class Vantiq:
+    """The interface for working with the Vantiq System.
+
+    This class consists of operations that can be performed using the Vantiq system. More information about
+    these operations can be found in the Vantiq Resource Reference Guide and the Vantiq API Reference Guide.
+
+    Logging for this class is done through a standard Python logger named "Vantiq".  It is assumed that the
+    client of this library will configure the logger as desired.
+
+    The Vantiq object instance can be used as a context manager.
+        async with Vantiq(<server url>) as client:
+            resp: VantiqResponse = client.select(VantiqResource, ...)
+    for example.
+
+    As noted, most of the operations in the Vantiq object are `async` and must be awaited for them to run. See
+    https://docs.python.org/3/library/asyncio.html for more details about working with async operations.
+
+    """
+
+    def __init__(self, server: str, api_version: Union[str, None] = None):
+        """Create a Vantiq client object.
+
+        Parameters:
+            server : str
+                URL String at which to find the Vantiq Server
+
+            api_version : str (optional)
+                Version of the API to use. Defaults to '1'
+
+        Returns:
+            Vantiq client object with which to interact with the Vantiq system.
+
+        Can be used as a context manager
+
+        Examples:
+            As a context manager::
+            ::
+
+                async with Vantiq('https://dev.vantiq.com') as client:
+                    ...
+
+            or, in a client object:
+            ::
+                client = Vantiq('https://dev.vantiq.com')
+                ...
+                await client.close()
+
+
+        """
+        self._vlog: Logger = logging.getLogger(self.__class__.__name__)
+
+        if server.endswith('/'):
+            self._server = server[:-len('/')]  # server.removesuffix('/')'
+        else:
+            self._server = server
+        self._api_version = api_version if api_version else '1'
+        self._is_authenticated = False
+        self._username = None
+        self._target_namespace = None
+        self._access_token = None
+        self._id_token = None
+        self._auth_header = None
+        self._connection = None
+        self._is_connected = False
+        self._connection = _RestClient(self._server)
+        self._base_path = '/api/v' + self._api_version + '/'
+        self._subscriber: Union[_VantiqSubscriber, None] = None
+
+    def __str__(self):
+        return f'Vantiq connection to {self._server}, is_connected: {self._is_connected}, ' \
+               f'is_authenticated: {self._is_authenticated}'
+
+    def __repr__(self):
+        return f'Vantiq({self._server}, {self._api_version}) n# is_connected: {self._is_connected}, ' \
+               f'is_authenticated: {self._is_authenticated}'
+
+    async def __aenter__(self):
+        await self.connect()
+        return self
+
+    async def __aexit__(self, exc_type, exc, tb):
+        await self.close()
+
+    async def connect(self) -> None:
+        """Make the connection to the Vantiq server
+
+        Returns:
+            None
+        Raises:
+            VantiqException for connection issues
+
+        Notes:
+            Should precede the .authenticate().  Must be done before other operations.
+        """
+
+        if not self._is_connected:
+            await self._connection.connect()
+            self._is_connected = True
+            self._vlog.debug('Connected to server: %s', self._server)
+
+    def get_server(self):
+        """Returns the server url used for this connection."""
+        return self._server
+
+    def get_api_version(self):
+        """Returns the API version used for this connection."""
+        return self._api_version
+
+    async def set_access_token(self, access_token: str) -> None:
+        """Set the access token for server access.
+
+        Access to the Vantiq server is controlled.  Access can be granted by using an access token (recommended) or
+        a username and password.
+
+        Parameters:
+            access_token : str
+                Access token to be used to gain access to the Vantiq system
+        """
+        if not self._is_connected:
+            await self.connect()
+        self._access_token = access_token
+        self._auth_header = 'Bearer ' + self._access_token
+        self._is_authenticated = True  # We have an access token, we'll figure we're OK til we're not
+
+    def get_access_token(self) -> str:
+        """Returns the access token currently in use."""
+        return self._access_token
+
+    def set_target_namespace(self, namespace: Union[str, None]) -> None:
+        """Set the target namespace to be used to access the Vantiq server"""
+        self._target_namespace = namespace
+
+    def get_target_namespace(self) -> Union[str, None]:
+        """Returns the target namespace currently in use."""
+        return self._target_namespace
+
+    def set_username(self, username: str) -> None:
+        """Set the username to be used to access the Vantiq server"""
+        self._username = username
+
+    def get_username(self) -> str:
+        """Returns the username currently in use."""
+        return self._username
+
+    def get_id_token(self) -> str:
+        return self._id_token
+
+    def is_authenticated(self) -> bool:
+        """Returns a boolean indicating whether this Vantiq instance is authenticated."""
+        return self._is_authenticated
+
+    async def authenticate(self, username: str, password: str) -> None:
+        """(Async) Use a username and password to connect to the Vantiq system.
+
+        Parameters:
+            username : str
+                The username to be used to authenticate to the Vantiq server.
+            password : str
+                The password to be used to authenticate to the Vantiq server.
+
+        Returns:
+            Raises a VantiqException in case of failure.
+
+        Example:
+        ::
+            await client.authenticate('vantiquser', 'secret')
+        """
+        if not self._is_connected:
+            await self.connect()
+        b64 = base64.b64encode((username + ':' + password).encode('utf=8')).decode('utf-8')
+        headers = {aiohttp.hdrs.AUTHORIZATION: 'Basic ' + b64}
+        resp = await self._connection.request('GET', '/authenticate', headers=headers)
+        ret_val = VantiqResponse(resp.ok, resp.status, resp.content_type)
+        if not resp.ok:
+            # noinspection PyProtectedMember
+            await ret_val._populate_errors(resp)
+            self._vlog.error('Authentication to server %s failed: %s', self._server, resp)
+            raise VantiqException(resp.errors[0].code, resp.errors[0].message, resp.errors[0].params)
+        # noinspection PyProtectedMember
+        await ret_val._populate_body(resp)
+        self._access_token = ret_val.body['accessToken']
+        self._username = username
+        self._id_token = ret_val.body['idToken']
+        self._is_authenticated = True
+        self._auth_header = 'Bearer ' + self._access_token
+
+    async def refresh(self) -> None:
+        """(Async) Refresh the access token with the Vantiq Server."""
+        if self._is_authenticated:
+            path = '/authenticate/refresh'
+            headers = {aiohttp.hdrs.CONTENT_TYPE: 'text/plain'}
+            resp = await self._connection.request('POST', path, headers=headers, data=self._access_token)
+            ret_val = VantiqResponse(resp.ok, resp.status, resp.content_type)
+            if not resp.ok:
+                self._vlog.error('Authentication/refresh to server %s failed: %s', self._server, resp)
+                # noinspection PyProtectedMember
+                await ret_val._populate_errors(resp)
+                raise VantiqException(resp.errors[0].code, resp.errors[0].message, resp.errors[0].params)
+            # noinspection PyProtectedMember
+            await ret_val._populate_body(resp)
+            self._access_token = ret_val.body['accessToken']
+            self._id_token = ret_val.body['idToken']
+            self._is_authenticated = True
+            self._auth_header = 'Bearer ' + self._access_token
+        else:
+            raise VantiqException('io.vantiq.python.refreshnotauthenticated',
+                                  'Cannot refresh access token as this session is not authenticated.',
+                                  [])
+
+    async def close(self):
+        """(Async) End the Vantiq session"""
+        self._is_authenticated = False
+        self._access_token = None
+        self._id_token = None
+        self._base_path = None
+        self._auth_header = None
+        self._target_namespace = None
+        self._username = None
+        if self._subscriber:
+            await self._subscriber.close()
+            self._subscriber = None
+        if self._connection:
+            await self._connection.close()
+            self._connection = None
+
+    def _build_path(self, qualified_name: str, resource_id: Union[str, None], ext: Union[str, None] = None) -> str:
+        if qualified_name.startswith('system.'):
+            path = self._base_path + 'resources/' + qualified_name[len('system.'):]  # removeprefix(_SYSTEM_PREFIX)
+        else:
+            path = self._base_path + 'resources/custom/' + qualified_name
+
+        if resource_id:
+            path += '/' + resource_id
+        if ext:
+            path += '/' + ext
+
+        return path
+
+    @staticmethod
+    def _check_error(response: Union[dict, List[dict], None]):
+        if response:
+            code = None
+            message = None
+            params = None
+            if isinstance(response, list):
+                response = response[0]
+            if 'code' in response.keys():
+                code = response['code']
+                if 'message' in response.keys():
+                    message = response['message']
+                if 'params' in response.keys():
+                    params = response['params']
+            elif 'error' in response.keys():
+                message = response['error']
+                code = 'io.vantiq.python.error'
+                params = []
+            raise VantiqException(code, message, params)
+
+    def _get_auth_headers(self) -> dict:
+        headers = {aiohttp.hdrs.AUTHORIZATION: self._auth_header}
+        if self._target_namespace is not None:
+            headers['X-Target-Namespace'] = self._target_namespace
+        return headers
+
+    async def _perform_operation(self, operation: str, method: str, path: str,
+                                 query_params: Union[dict, None], is_streaming: bool,
+                                 instance: Union[dict, None] = None) -> VantiqResponse:
+        if self._is_authenticated:
+            try:
+                headers = self._get_auth_headers()
+                if instance is None:
+                    # When no parameters are passed at all, we get 404's back.  So None as parameters == {}.
+                    instance = {}
+
+                body = json.dumps(instance)
+                headers[aiohttp.hdrs.CONTENT_TYPE] = 'application/json'
+                resp: aiohttp.ClientResponse = await self._connection.request(method, path, headers=headers,
+                                                                              query_param=query_params, body=body)
+                ret_val = VantiqResponse(resp.ok, resp.status, resp.content_type)
+                if resp.ok:
+                    # noinspection PyProtectedMember
+                    ret_val._populate_count(resp)
+                    if is_streaming:
+                        # noinspection PyProtectedMember
+                        ret_val._populate_streaming_body(resp)
+                    else:
+                        # noinspection PyProtectedMember
+                        await ret_val._populate_body(resp)
+                else:
+                    # noinspection PyProtectedMember
+                    await ret_val._populate_errors(resp)
+                return ret_val
+            except Exception as e:
+                raise VantiqException('io.vantiq.python.operationerror',
+                                      'Unexpected error during {0} operation.',
+                                      [operation]) from e
+
+        else:
+            raise VantiqException('io.vantiq.python.request.notauthenticated',
+                                  'A {0} request was made on a session that is not connected.',
+                                  [operation])
+
+    async def select(self, resource: str,
+                     properties: Union[list, None] = None,
+                     where: Union[dict, None] = None,
+                     sort_spec: Union[dict, None] = None,
+                     limit: Union[int, None] = None,
+                     options: Union[dict, None] = None) -> VantiqResponse:
+        """(Async) Return items from a Vantiq resource.
+
+        Select specific items from a Vantiq resource. Selection and details of the return are controlled
+        by the following parameters:
+
+        Parameters:
+            resource : str
+                The name of the resource to be returned.  System resource names are provided via the VantiqResource
+                class.
+            properties : list(str)
+                (optional) The list of properties for the resource to be returned. If missing, return all properties.
+            where : dict(str: *)
+                (optional) The "where clause" to be used to restrict the selection.  The contents are defined
+                in the API Reference Guide.
+            sort_spec : dict(str: int)
+                (optional) Defines the sort order of the returned values.  The key value defines the property on which
+                to sort, and the value determines the order (1 = ascending, -1 = descending).  See the API Reference
+                Guide for details.
+            limit : int
+                (optional) Limit the number of records returned
+            options : dict (str, *)
+                (optional) Additional query parameter options
+        Returns:
+            VantiqResponse
+
+        Examples:
+        ::
+            vr: VantiqResponse = await client.select('myType')
+            if vr.is_success:
+                ...
+        """
+        operation = 'select'
+        try:
+            query_params = {}
+            if properties:
+                query_params['props'] = json.dumps(properties)
+            if where is not None:
+                query_params['where'] = json.dumps(where)
+            if sort_spec:
+                query_params['sort'] = json.dumps(sort_spec)
+            if limit is not None and limit > 0:
+                query_params['limit'] = limit
+                query_params['count'] = 'true'
+            if options:
+                for key, value in options.items():
+                    if isinstance(key, str) and isinstance(value, str):
+                        query_params[key] = value
+                    else:
+                        raise VantiqException('io.vantiq.python.option.stringsrequired',
+                                              'Options to queries must be of type str. ' +
+                                              'Found key {0}:{1} and value {2}:{3}.',
+                                              [key, type(key).__name__, value, type(value).__name__])
+            method = 'GET'
+            path = self._build_path(resource, None)
+            resp = await self._perform_operation(operation, method, path, query_params, False)
+            return resp
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operation.unexpectederror',
+                                  'Unexpected error during {0} operation.',
+                                  [operation]) from e
+
+    async def select_one(self, resource: str, resource_id: str = None) -> VantiqResponse:
+        """(Async) Select a single item from a Vantiq resource
+
+        Parameters:
+            resource : str
+                The name of the resource from which to select.
+            resource_id : str
+                The identifier for the specific item within the resource.
+        Returns:
+            VantiqResponse object
+
+        Example:
+        ::
+            vr: VantiqResponse = await client.selectOne('myType', 'type name')
+            if vr.is_success:
+                ....
+        """
+        operation = 'selectOne'
+        try:
+            method = 'GET'
+            query_params = {}
+            path = self._build_path(resource, resource_id)
+            resp = await self._perform_operation(operation, method, path, query_params, False)
+            return resp
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operation.unexpectederror',
+                                  'Unexpected error during {0} operation.',
+                                  [operation]) from e
+
+    async def delete(self, resource: str, where: Union[dict, None]) -> VantiqResponse:
+        """(Async) Delete item(s) from a Vantiq resource.
+
+        Parameters:
+            resource : str
+                The name of the Vantiq resource from which to delete items
+            where : dict (str: *)
+                The "where clause" to be used to determine which items to delete. The contents are defined
+                in the API Reference Guide.
+                Note that if where is None, this may delete all objects in the resource type.
+        Returns:
+            VantiqResponse.  The count property of the VantiqResponse will provide the number of objects deleted.
+
+        Examples:
+        ::
+           vr: VantiqResponse = await client.delete('myType', {'name': 'some name'}
+           if vr.is_success:
+              print('Count of items deleted: ', vr.count)
+        """
+
+        operation = 'delete'
+        try:
+            query_params = {'count': 'true'}
+            if where is not None:
+                query_params['where'] = json.dumps(where)
+            method = 'DELETE'
+            path = self._build_path(resource, None)
+            resp = await self._perform_operation(operation, method, path, query_params, False)
+            return resp
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operation.unexpectederror',
+                                  'Unexpected error during {0} operation.',
+                                  [operation]) from e
+
+    async def delete_one(self, resource: str, resource_id: str) -> VantiqResponse:
+        """(Async) Delete a single item from a resource.
+
+        Parameters:
+            resource : str
+                The name of the Vantiq resource from which to delete.
+            resource_id : str
+                The key for the item to delete.
+
+        Returns:
+            VantiqResponse indicating success of the operation
+
+        """
+        operation = 'delete'
+        try:
+            method = 'DELETE'
+            path = self._build_path(resource, resource_id)
+            resp = await self._perform_operation(operation, method, path, None, False)
+            return resp
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operation.unexpectederror',
+                                  'Unexpected error during {0} operation.',
+                                  [operation]) from e
+
+    async def insert(self, resource: str, instance: dict) -> VantiqResponse:
+        """(Async) Insert an item into Vantiq Resource.
+
+        Parameters:
+            resource : str
+                Name of the Vantiq resource into which to insert.
+            instance : dict
+                The values to be inserted.  The key names in the _instance_ parameter
+                must match the property names in the Vantiq object.
+
+        Returns:
+            VantiqResponse indicating success/failure of the operation and the value inserted.
+        """
+
+        if instance is None:
+            raise VantiqException('io.vantiq.python.insert.none',
+                                  'The object to be inserted cannot be None.', [])
+        operation = 'insert'
+        try:
+            method = 'POST'
+            path = self._build_path(resource, None)
+            resp = await self._perform_operation(operation, method, path, None, False, instance)
+            return resp
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operation.unexpectederror',
+                                  'Unexpected error during {0} operation.',
+                                  [operation]) from e
+
+    async def upsert(self, resource: str, instance: dict) -> VantiqResponse:
+        """(Async) Upsert an item into Vantiq Resource.
+
+            Parameters:
+                resource : str
+                    Name of the Vantiq resource into which to upsert.
+                instance : dict
+                    The values to be upserted.   The key names in the _instance_ parameter
+                    must match the property names in the Vantiq object.
+
+            Returns:
+                VantiqResponse indicating success/failure of the operation and the value upserted.
+        """
+
+        if instance is None:
+            raise VantiqException('io.vantiq.python.upsert.none',
+                                  'The object to be upserted cannot be None.', [])
+        operation = 'upsert'
+        try:
+            instance.pop('_id', None)
+            query_params = {'upsert': 'true'}
+            method = 'POST'
+            path = self._build_path(resource, None)
+            resp = await self._perform_operation(operation, method, path, query_params, False, instance)
+            return resp
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operation.unexpectederror',
+                                  'Unexpected error during {0} operation.',
+                                  [operation]) from e
+
+    async def update(self, resource: str, resource_id: str, instance: dict) -> VantiqResponse:
+        """(Async) Update an item in a  Vantiq Resource.
+
+            Parameters:
+                resource : str
+                    Name of the Vantiq resource in which to update.
+                resource_id : str
+                    The key of the record to look up for replacement.  The _id property can be used/
+                instance : dict
+                    The values to be updated. The key names in the _instance_ parameter
+                    must match the property names being updated in the Vantiq object.
+
+            Returns:
+                VantiqResponse indicating success/failure of the operation and the value updated.
+        """
+
+        if instance is None:
+            raise VantiqException('io.vantiq.python.upsert.none',
+                                  'The object to be upserted cannot be None.', [])
+        operation = 'update'
+        try:
+            instance.pop('_id', None)
+            query_params = {}
+            method = 'PUT'
+            path = self._build_path(resource, resource_id)
+            resp = await self._perform_operation(operation, method, path, query_params, False, instance)
+            return resp
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operation.unexpectederror',
+                                  'Unexpected error during {0} operation.',
+                                  [operation]) from e
+
+    async def download(self, path: str) -> VantiqResponse:
+        """(Async) Download content from a Vantiq Document, Image, Video, or TensorflowModel.
+
+        Parameters:
+            path : str
+                The path from which to obtain the data. This is found in the `content` field of the base object.
+
+        Returns:
+            VantiqResponse. In this case, the response's `body` field is an `aiohttp.StreamReader` that can be used
+            to fetch the content returned.
+
+        Examples:
+        ::
+            vr: VantiqResponse = await client.selectOne(VantiqResources.DOCUMENTS, 'mydoc')
+            mydoc = vr.body
+            if vr.is_success:
+                download_vr: VantiqResponse = await client.download(mydoc.content)
+                if download_vr.is_success:
+                    reader = download_vr.body
+                    while True:
+                        data = await reader.read(100)  # Read our data 100 bytes at a time
+                        if len(data) == 0:
+                            break
+                        # Do something with the data
+                        ...
+        """
+        url = path
+        headers = self._get_auth_headers()
+        try:
+            resp = await self._connection.download(url, headers)
+            ret_val = VantiqResponse(resp.ok, resp.status, resp.content_type)
+            # noinspection PyProtectedMember
+            ret_val._populate_count(resp)
+            # noinspection PyProtectedMember
+            ret_val._populate_streaming_body(resp)
+            return ret_val
+        except aiohttp.ClientPayloadError as cpe:
+            raise VantiqException('io,vantiq.python.downloaderror',
+                                  'Error encountered during download of {0}',
+                                  [path]) from cpe
+
+    async def upload(self, resource: str, content_type: str, filename: str,
+                     doc_name: Union[str, None] = None,
+                     inmem: Union[str, bytes, bytearray, None] = None) -> VantiqResponse:
+        """(Async) Upload a file (or in-memory data), creating an object to hold that data.
+
+        This allows the upload of a file to create a document, inage, video, or tensorflow model.
+
+        Parameters:
+            resource : str
+                The Vantiq resource type to create.
+            content_type : str
+                The type of data contained in the file.  This will be set as the `contentType` of the resulting
+                object.
+            filename : str
+                The name of the file to upload.
+            doc_name : str
+                (optional) The name of the object to create. If this is missing, use the filename.
+            inmem : str | bytes | bytearray
+                (optional) Content to be uploaded.  Used when the content is not in a file.
+
+        Returns:
+            VantiqResponse containing the object created.
+
+        Examples:
+        ::
+            vr: VantiqResponse = await client.upload(VantiqResources.DOCUMENTS, 'iamge/png', 'path/name.png')
+            if vr.is_success:
+                # Here, we will have uploaded a file named `path/name.png`,
+                # and created a Document named `path/name.png`.
+
+            vr: VantiqResponse = await client.upload(VantiqResource.DOCUMENTS, 'text/plain', None,
+                                                     'my document', 'some content for my document')
+            if vr.is_success:
+                # Here, we will have created a document named 'my document' with the content
+                # 'some content for my document'
+
+        """
+        ve = None
+        if content_type is None:
+            ve = VantiqError('io.vantiq.python.upload.contenttype',
+                             'Missing content type specification for an upload call().',
+                             [])
+        elif resource is None:
+            ve = VantiqError('io.vantiq.python.upload.resource',
+                             'The resource type is missing for an upload() call.',
+                             [])
+        elif filename is None and inmem is None:
+            ve = VantiqError('io.vantiq.python.content',
+                             'The filename and inmem parameters for an upload() call are both missing.',
+                             [])
+        elif filename and doc_name and inmem:
+            ve = VantiqError('io.vantiq.python.duplicatename',
+                             'When uploading in memory object, only one of filename or doc_name is permitted.',
+                             [])
+        elif filename is None and doc_name is None:
+            ve = VantiqError('io.vantiq.python.noname',
+                             'Neither a file name nor a document name was provided for an upload() call.',
+                             [])
+
+        if ve:
+            return VantiqResponse.from_error(ve)
+
+        path = self._build_path(resource, None)
+        headers = self._get_auth_headers()
+
+        try:
+            resp = await self._connection.upload(path, headers, content_type, filename, doc_name, inmem)
+            ret_val = VantiqResponse(resp.ok, resp.status, resp.content_type)
+            # noinspection PyProtectedMember
+            ret_val._populate_count(resp)
+            # noinspection PyProtectedMember
+            await ret_val._populate_body(resp)
+            return ret_val
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operationerror',
+                                  'Unexpected error during {0} operation.',
+                                  ['upload']) from e
+
+    async def count(self, resource: str, where: Union[dict, None] = None) -> VantiqResponse:
+        """(Async) Return the number of items in a Vantiq resource that satisfy the where clause
+
+        Parameters:
+            resource : str
+                The name of the resource to be counted.  System resource names are provided via the VantiqResource
+                class.
+            where : dict(str: *)
+                (optional) The "where clause" to be used to restrict the counting.  The where clause is defined
+                in the API Reference Guide.
+        Returns:
+            VantiqResponse where the `count` field contains the count requested.
+        """
+
+        operation = 'count'
+        try:
+            # Here, specify that we want the count but don't really care about the data.  So we'll limit
+            # the return to a single row & limit the properties returned
+            query_params = {'count': 'true', 'limit': 1}
+            if where is not None:
+                query_params['where'] = json.dumps(where)
+            props = ['_id']  # Since we don't care about the data, return the least we can
+            query_params['props'] = json.dumps(props)
+            method = 'GET'
+            path = self._build_path(resource, None)
+            resp = await self._perform_operation(operation, method, path, query_params, False)
+            resp.body = {}  # After a count, we don't need to return the data fetched (since we decided it anyway)
+            return resp
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operation.unexpectederror',
+                                  'Unexpected error during {0} operation.',
+                                  [operation]) from e
+
+    async def query(self, source_id: str, query: dict) -> VantiqResponse:
+        """(Async) Send a query message to a Vantiq source
+
+        Parameters:
+            source_id : str
+                Name of the source to which to send the query
+            query : dict
+                The message describing the query to be sent.  These messages are source specific.
+
+        Returns:
+            VantiqResponse indicating the success or failure of the query.  The body field will contain the results
+            of the query (if applicable).
+        """
+
+        operation = 'query'
+        try:
+            query_params = {}
+            method = 'POST'
+            path = self._build_path(VantiqResources.SOURCES, source_id, 'query')
+            resp = await self._perform_operation(operation, method, path, query_params, False, query)
+            return resp
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operation.unexpectederror',
+                                  'Unexpected error during {0} operation.',
+                                  [operation]) from e
+
+    async def execute(self, procedure_id: str, params: dict) -> VantiqResponse:
+        """(Async) Execute a Vantiq procedure.
+
+        Parameters:
+            procedure_id : str
+                The name of the procedure to execute.
+            params : dict
+                The parameters provided for the procedure's execution.  The key names are the parameter names,
+                and the values their values.
+        Returns:
+            VantiqResponse where the body contains the results of the procedure execution, if any.
+
+        """
+
+        operation = 'execute'
+        try:
+            query_params = {}
+            method = 'POST'
+            path = self._build_path(_SYSTEM_PREFIX + 'procedures', procedure_id)
+            resp = await self._perform_operation(operation, method, path, query_params, False, params)
+            return resp
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operation.unexpectederror',
+                                  'Unexpected error during {0} operation.',
+                                  [operation]) from e
+
+    async def publish(self, resource: str, resource_id: str, msg: dict) -> VantiqResponse:
+        """(Async) Publish a message to a Vantiq Service (event), Source, or Topic.
+
+        Parameters:
+            resource : str
+                The resource to which to publish.  Must be either VantiqResources.SERVICES, VantiqResources.SOURCES,
+                or VantiqResources.TOPICS.
+            resource_id : str
+                The specific service, source, or topic to which to publish. If the resource is VantiqResources.SERVICES,
+                the resource_id will take the form 'service_name/event_name.  This event should be defined as one of
+                the inbound events for the service in question.
+            msg : dict
+                The message to publish
+        Returns:
+            VantiqResponse
+
+        """
+
+        operation = 'publish'
+        if resource not in [VantiqResources.SOURCES, VantiqResources.TOPICS, VantiqResources.SERVICES]:
+            err = VantiqError('io.vantiq.python.publish.invalidresource',
+                              'The publish operation can be performed only on the following resources: {0}',
+                              [[VantiqResources.SERVICES, VantiqResources.SOURCES, VantiqResources.TOPICS]])
+            return VantiqResponse.from_error(err)
+        try:
+            query_params = {}
+            method = 'POST'
+            path = self._build_path(resource, resource_id)
+            resp = await self._perform_operation(operation, method, path, query_params, False, msg)
+            return resp
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operation.unexpectederror',
+                                  'Unexpected error during {0} operation.',
+                                  [operation]) from e
+
+    async def get_namespace_users(self, namespace: str) -> VantiqResponse:
+        """(Async) Returns a JsonArray containing objects which map between "username" and "preferredUsername"
+
+        Parameters:
+            namespace : str
+                The name of the namespace from which to get the list of users.
+        Returns:
+            VantiqResponse
+     """
+        operation = 'getNamespaceUsers'
+        try:
+            query_params = {}
+            method = 'GET'
+            path = self._build_path(VantiqResources.NAMESPACES, namespace, 'authorizedUsers')
+            resp = await self._perform_operation(operation, method, path, query_params, False)
+            return resp
+        except VantiqException:
+            # If we've already handled or wrapped it, just pass it along
+            raise
+        except Exception as e:
+            raise VantiqException('io.vantiq.python.operation.unexpectederror',
+                                  'Unexpected error during {0} operation.',
+                                  [operation]) from e
+
+    async def start_subscriber_transport(self):
+        """(Async) Start a task to handle subscriptions.
+
+        To handle incoming messages from the Vantiq server that arise from subscriptions, you must start an
+        asyncio task to do this work.  This method does that work.
+
+        If the transport does not exist when subscribe() is called, subscribe() will start
+        the transport on your behalf.
+
+        Parameters:
+            (none)
+        Returns:
+            The task created. Can be used to wait or manage that task.
+            If the subscriber connection already exists, None is returned as there is no new task.
+
+        """
+
+        if self._subscriber is None:
+            self._subscriber = _VantiqSubscriber(self)
+            task = asyncio.create_task(self._subscriber.connect())
+            failure_reason = None
+            try:
+                if self._subscriber.connected_future:
+                    await self._subscriber.connected_future
+            except Exception as e:
+                failure_reason = e
+            if not failure_reason:
+                failure_reason = self._subscriber.connected_future.exception()
+            if not failure_reason:
+                failure_reason = self._subscriber.connected_future.result()
+            if failure_reason != 'OK':
+                await self._subscriber.close()
+                self._subscriber = None
+                await task
+                if isinstance(failure_reason, Exception):
+                    raise VantiqException('io.vantiq.python.subtransport.exception',
+                                          'Failed to start subscriber transport: {0}',
+                                          [failure_reason]) from failure_reason
+                else:
+                    raise VantiqException('io.vantiq.python.subtransport.failed',
+                                          'Failed to start subscriber transport: {0}',
+                                          [failure_reason])
+            return task
+        else:
+            return None
+
+    async def subscribe(self, resource: str, resource_id: str, operation: Union[str, None],
+                        callback: Callable[[str, dict], Awaitable[None]], params: Union[dict, None] = None,
+                        target_namespace: Union[str, None] = None) -> VantiqResponse:
+        """(Async) Subscribe to an event from the Vantiq server.
+
+        Subscribes to a specific topic, source, service, or type event.
+
+        For sources, this will subscribe to message arrival events.  The name of the
+        source is required (e.g. "MySource").
+
+        For topics, this will subscribe to any messages published on that topic.  The
+        name of the topic is required (e.g. "/some/topic").
+
+        For services, this will subscribe to any messages published to the named service event. The name of the
+        service and service event is required, and should be passed into the resource id as service_name/event_name.
+
+        For types, this will subscribe to the specified type event.  The name of the
+        type and the operation (i.e. "insert", "update", or "delete") are required.
+
+        Parameters:
+            resource : str
+                The resource type for which this subscription is being made
+            resource_id : str
+                The identifier of the specific instance of the `resource` in question.
+            operation : str
+                The operation to which to subscribe when subscribing to a VantiqResources.TYPES event. Should be None
+                for other resource types.
+            callback : Callable[[str, dict], Awaitable[None]]
+                A callback function to call when a subscribed event arrives. The callback will be called with the
+                type of the callback ('connect', 'message', 'error') and the message contents.
+
+                The callback message contains the following properties:
+                    status : int -- the status of the event
+                    contentType : str -- the content type of the message
+                    path : str -- the event specification
+                    value : dict -- the value of the event (type inserted, topic contents, etc.)
+
+            params : dict
+                (optional) Parameters for the subscription. May be subscription dependent, but can usually be ignored.
+            target_namespace : str
+                (optional) The namespace in which to subscribe.  If not provided, the current namespace is used.
+        Returns:
+            VantiqResponse indicating the success of the operation.
+
+        For details, see the Vantiq API Reference Guide.
+        """
+
+        if VantiqResources.TOPICS == resource:
+            path = "/" + resource[len(_SYSTEM_PREFIX):] + resource_id  # .removeprefix(_SYSTEM_PREFIX) + resource_id
+        else:
+            path = "/" + resource[len(_SYSTEM_PREFIX):] + '/' + resource_id  # .removeprefix(_SYSTEM_PREFIX) ...
+        if resource in [VantiqResources.SERVICES, VantiqResources.SOURCES, VantiqResources.TOPICS]:
+            if operation:
+                raise VantiqException('io.vantiq.python.operationillegal',
+                                      "Operation only support for {0}",
+                                      [VantiqResources.TYPES])
+        elif VantiqResources.TYPES == resource:
+            if operation is None:
+                raise VantiqException('io.vantiq.python.operationrequired',
+                                      "Operation required for {0}",
+                                      [VantiqResources.TYPES])
+
+            path += "/" + operation.lower()
+        else:
+            raise VantiqException('io.vantiq.python.invalidsubscribetype',
+                                  "Only 'topics', 'sources', 'services', and 'types' support subscribe",
+                                  [])
+
+        if self._subscriber is None:
+            await self.start_subscriber_transport()
+
+        vr = await self._subscriber.subscribe(path, params, callback, target_namespace)
+        return vr
+
+    async def ack(self, request_id: str, subscription_id: str, msg: dict) -> None:
+        """ Acknowledge the receipt of a reliable message
+
+        Parameters:
+            request_id : str
+                id of the request -- this can be found in the 'X-Request_id' header of the callback for the subscription
+            subscription_id : str
+                id of the subscription that delivered the message -- this is found in the [body][name] field of the
+                callback for the subscription message.
+            msg : dict
+                message being acknowledged
+        Raises:
+            VantiqException
+        """
+        if 'partitionId' not in msg.keys():
+            raise VantiqException('io.vantiq.python.ack.nopartitionid',
+                                  'The message being acknowledged contains no partition_id.',
+                                  [])
+        elif 'sequenceId' not in msg.keys():
+            raise VantiqException('io.vantiq.python.ack.nosequenceid',
+                                  'The message being acknowledged contains no sequence_id.',
+                                  [])
+
+        sequence_id = msg['sequenceId']
+        partition_id = msg['partitionId']
+        await self._subscriber.ack(request_id, subscription_id, sequence_id, partition_id)
+        return
+
+    def register_subscriber_on_close(self, callback: Callable[[], Awaitable[None]]):
+        """ Register a callback to be called when the subscriber is closed.
+
+        Parameters:
+            callback : Callable[[], Awaitable[None]]
+                The callback to be called when the subscriber is closed.
+        """
+        self._subscriber.on_close_handler = callback
+
+
+class _VantiqSubscriber:
+    CONNECT = 'connect'
+    MESSAGE = 'message'
+    ERROR = 'error'
+
+    def __init__(self, parent: Vantiq):
+        self.parent: Vantiq = parent
+        self.connected = False
+        self.connected_future: asyncio.Future = asyncio.get_running_loop().create_future()
+        # noinspection PyTypeChecker
+        self.connection: websockets.ClientProtocol = None
+        self.url = None
+        self._vlog = logging.getLogger(self.__class__.__name__)
+        self.subscriptions: Dict[str, bool] = {}
+        self.callbacks: Dict[str, Callable[[str, dict], Awaitable[None]]] = {}
+        self.is_authenticated = False
+        # noinspection PyTypeChecker
+        self.on_close_handler: Callable[[], Awaitable[None]] = None
+
+    def __str__(self):
+        ret_val = f'VantiqSubscriber for {str(self.parent)}'
+        if self.subscriptions:
+            for key, value in self.subscriptions.items():
+                ret_val += '\n\t' + key + ': ' + str(value)
+        return ret_val
+
+    def __repr__(self):
+        return f'VantiqSubscriber(repr({self.parent}))'
+
+    async def connect(self, do_pings: bool = True):
+        if self.parent is None or not self.parent.is_authenticated():
+            ve = VantiqException('io.vantiq.python.subscriber.notauthenticated',
+                                 'Attempt to connect subscriber when parent was not authenticated.',
+                                 [])
+            self.connected_future.set_exception(ve)
+            raise ve
+
+        if not self.connected:
+            self.url = self.parent.get_server().replace("http", "ws") + "/api/v" + self.parent.get_api_version() + \
+                  "/wsock/websocket"
+            async with websockets.connect(uri=self.url,
+                                          ping_interval=20 if do_pings else None,
+                                          ping_timeout=20 if do_pings else None) as websocket:
+                if not self.connected:
+                    auth_msg = {
+                        'op': 'validate',
+                        'resourceName': 'system.credentials',
+                        'object': self.parent.get_access_token()
+                    }
+                    await websocket.send(json.dumps(auth_msg))
+
+                async for raw in websocket:
+
+                    resp = json.loads(raw)
+                    request_id = None
+                    if 'headers' in resp.keys():
+                        hdrs = resp['headers']
+                        if 'X-Request-Id' in hdrs.keys():
+                            request_id = hdrs['X-Request-Id']
+                    else:
+                        pass
+
+                    # Using request id, track back to request for which this is a response
+
+                    if 'status' in resp.keys():
+                        if resp['status'] == 200:
+                            if not self.is_authenticated:
+                                self.connection = websocket
+                                self.connected = True
+                                self.is_authenticated = True
+                                self.connected_future.set_result('OK')
+                                self._vlog.debug('Authentication completed.')
+                            else:
+                                if request_id:
+                                    if request_id in self.subscriptions.keys():
+                                        if not self.subscriptions[request_id]:
+                                            # Then this is our response for our subscription.
+                                            self.subscriptions[request_id] = True
+                                            self._vlog.debug('Subscription requested accepted.')
+                                            callback = self.callbacks[request_id]
+                                            await callback(self.CONNECT, resp)
+                                        elif request_id in self.callbacks.keys():
+                                            callback = self.callbacks[request_id]
+                                            body = resp.get('body', None)
+                                            if body is not None and body.get('op', None) == 'unsubscribe':
+                                                self.subscriptions.pop(request_id)
+                                                self.callbacks.pop(request_id)
+                                            await callback(self.MESSAGE, resp)
+                        elif resp['status'] >= 400:
+                            if not self.connected:
+                                self._vlog.error('Connect call failed: %s :: %s:%s', resp['status'],
+                                                 resp['body'][0]['code'], resp['body'][0]['message'])
+                                ve = VantiqException('io.vantiq.python.connect.failed',
+                                                     'Connect call failed: {0} :: {1}:{2}',
+                                                     [resp['status'], resp['body'][0]['code'],
+                                                      resp['body'][0]['message']])
+                                self.connected_future.set_exception(ve)
+                                raise ve
+                            else:
+                                if request_id and request_id in self.callbacks.keys():
+                                    callback = self.callbacks[request_id]
+                                    await callback(self.ERROR, resp)
+                        elif resp['status'] == 100:
+                            if request_id and request_id in self.callbacks.keys():
+                                self._vlog.debug('Message received via subscription.')
+                                callback = self.callbacks[request_id]
+                                await callback(self.MESSAGE, resp)
+
+            # Once we get here, any transient subscriptions will be gone, so we should reset our side as well
+            await self.unsubscribe_all()
+
+    async def subscribe(self, path: str, params: dict, callback: Callable[[str, dict], Awaitable[None]],
+                        target_namespace: Union[str, None] = None) -> VantiqResponse:
+        # If we aren't connected, complain
+        if not self.connected:
+            self._vlog.error('No transport for subscriptions established.')
+            vr = VantiqResponse(False, 400, None)
+            ve = VantiqError('io.vantiq.python.notransport',
+                             'No transport for subscriptions has been established.',
+                             [])
+            vr.errors = [ve]
+            return vr
+
+        # Construct the request id using the path and (optional) target namespace
+        target_namespace = target_namespace or self.parent.get_target_namespace()
+        request_id = path
+        if target_namespace is not None:
+            request_id += '@' + target_namespace
+
+        if request_id in self.subscriptions.keys():
+            vr = VantiqResponse(False, 400, None)
+            ve = VantiqError('io.vantiq.python.subscribed',
+                             'A subscription for path {0} already exists for ns {1}.',
+                             [path, target_namespace or "current"])
+            vr.errors = [ve]
+            return vr
+        self.callbacks[request_id] = callback
+        self.subscriptions[request_id] = False  # Will be set to true when the server responds
+        if params is None:
+            params = {}
+        params['requestId'] = request_id
+        sub_msg = {'op': 'subscribe',
+                   'resourceName': 'events',
+                   'resourceId': path,
+                   'parameters': params}
+        if target_namespace is not None:
+            sub_msg['targetNamespace'] = target_namespace
+        # noinspection PyUnresolvedReferences
+        await self.connection.send(json.dumps(sub_msg))
+        self._vlog.debug('Subscription request sent.')
+        return VantiqResponse(True, 204, None)
+
+    async def ack(self, request_id: str, subscription_id: str, sequence_id: float, partition_id: float):
+        params = {'requestId': request_id,
+                  'subscriptionName': subscription_id, 'sequenceId': sequence_id, 'partitionId': partition_id}
+        msg = {'op': 'acknowledge', 'resourceName': 'events', 'resourceId': request_id,
+               'parameters': params}
+        if self.parent.get_target_namespace() is not None:
+            msg['targetNamespace'] = self.parent.get_target_namespace()
+        raw = json.dumps(msg)
+        # noinspection PyUnresolvedReferences
+        await self.connection.send(raw)
+
+    async def unsubscribe_all(self):
+        await self.close()
+        self.subscriptions = {}
+        self.callbacks = {}
+
+    async def close(self):
+        self.connected = False
+        # noinspection PyUnresolvedReferences
+        await self.connection.close()
+        self.connection = None
+        self.is_authenticated = False
+        if self.on_close_handler is not None:
+            await self.on_close_handler()
```

