# Comparing `tmp/logyca_postgres-0.1.1.tar.gz` & `tmp/logyca_postgres-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logyca_postgres-0.1.1.tar", last modified: Tue May 21 23:34:56 2024, max compression
+gzip compressed data, was "logyca_postgres-0.1.2rc1.tar", last modified: Thu May 23 16:44:17 2024, max compression
```

## Comparing `logyca_postgres-0.1.1.tar` & `logyca_postgres-0.1.2rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 23:34:56.050252 logyca_postgres-0.1.1/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_postgres-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0    15458 2024-05-21 23:34:56.048251 logyca_postgres-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    12554 2024-05-21 23:29:47.000000 logyca_postgres-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 23:34:56.006252 logyca_postgres-0.1.1/logyca_postgres/
--rw-rw-rw-   0        0        0      813 2024-04-26 23:15:08.000000 logyca_postgres-0.1.1/logyca_postgres/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 23:34:56.029252 logyca_postgres-0.1.1/logyca_postgres/dependencies/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.1/logyca_postgres/dependencies/__init__.py
--rw-rw-rw-   0        0        0     9945 2024-04-26 23:13:21.000000 logyca_postgres-0.1.1/logyca_postgres/dependencies/conn_postgres_async.py
--rw-rw-rw-   0        0        0     9988 2024-05-20 21:52:10.000000 logyca_postgres-0.1.1/logyca_postgres/dependencies/conn_postgres_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-21 23:34:56.032251 logyca_postgres-0.1.1/logyca_postgres/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.1/logyca_postgres/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 23:34:56.040251 logyca_postgres-0.1.1/logyca_postgres/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.1/logyca_postgres/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0      228 2024-04-23 14:32:08.000000 logyca_postgres-0.1.1/logyca_postgres/utils/helpers/functions.py
--rw-rw-rw-   0        0        0      331 2024-04-23 14:32:08.000000 logyca_postgres-0.1.1/logyca_postgres/utils/helpers/singleton.py
-drwxrwxrwx   0        0        0        0 2024-05-21 23:34:56.043251 logyca_postgres-0.1.1/logyca_postgres.egg-info/
--rw-rw-rw-   0        0        0    15458 2024-05-21 23:34:55.000000 logyca_postgres-0.1.1/logyca_postgres.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2024-05-21 23:34:55.000000 logyca_postgres-0.1.1/logyca_postgres.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 23:34:55.000000 logyca_postgres-0.1.1/logyca_postgres.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      445 2024-05-21 23:34:55.000000 logyca_postgres-0.1.1/logyca_postgres.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-21 23:34:55.000000 logyca_postgres-0.1.1/logyca_postgres.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 23:34:56.051250 logyca_postgres-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2589 2024-05-21 23:32:35.000000 logyca_postgres-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:44:17.806637 logyca_postgres-0.1.2rc1/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc1/LICENSE.txt
+-rw-rw-rw-   0        0        0    15699 2024-05-23 16:44:17.806637 logyca_postgres-0.1.2rc1/PKG-INFO
+-rw-rw-rw-   0        0        0    12802 2024-05-23 15:32:49.000000 logyca_postgres-0.1.2rc1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 16:44:17.729698 logyca_postgres-0.1.2rc1/logyca_postgres/
+-rw-rw-rw-   0        0        0      813 2024-04-26 23:15:08.000000 logyca_postgres-0.1.2rc1/logyca_postgres/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:44:17.775214 logyca_postgres-0.1.2rc1/logyca_postgres/dependencies/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc1/logyca_postgres/dependencies/__init__.py
+-rw-rw-rw-   0        0        0     9945 2024-04-26 23:13:21.000000 logyca_postgres-0.1.2rc1/logyca_postgres/dependencies/conn_postgres_async.py
+-rw-rw-rw-   0        0        0     9988 2024-05-20 21:52:10.000000 logyca_postgres-0.1.2rc1/logyca_postgres/dependencies/conn_postgres_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:44:17.793060 logyca_postgres-0.1.2rc1/logyca_postgres/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc1/logyca_postgres/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:44:17.806637 logyca_postgres-0.1.2rc1/logyca_postgres/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc1/logyca_postgres/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0      228 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc1/logyca_postgres/utils/helpers/functions.py
+-rw-rw-rw-   0        0        0      331 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc1/logyca_postgres/utils/helpers/singleton.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:44:17.806637 logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/
+-rw-rw-rw-   0        0        0    15699 2024-05-23 16:44:17.000000 logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2024-05-23 16:44:17.000000 logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:44:17.000000 logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      445 2024-05-23 16:44:17.000000 logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 16:44:17.000000 logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 16:44:17.823099 logyca_postgres-0.1.2rc1/setup.cfg
+-rw-rw-rw-   0        0        0     2580 2024-05-23 15:30:06.000000 logyca_postgres-0.1.2rc1/setup.py
```

### Comparing `logyca_postgres-0.1.1/LICENSE.txt` & `logyca_postgres-0.1.2rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.1/PKG-INFO` & `logyca_postgres-0.1.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: logyca-postgres
-Version: 0.1.1
+Version: 0.1.2rc1
 Summary: An integration package created by the company LOGYCA that connects Postgres and is used to standardize connections and dependency injection in synchronous or asynchronous mode. Tested in fastapi and in console/worker scripts.
 Home-page: https://github.com/logyca/<soon>
 Author: Jaime Andres Cardona Carrillo
-Author-email: tecnologiaeinformacion@logyca.com
+Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: postgres,driver database
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
@@ -63,15 +63,15 @@
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/logyca" target="_blank">
     <img src="https://img.shields.io/pypi/v/logyca?color=orange&label=PyPI%20Package" alt="Package version">
 </a>
 <a href="(https://www.python.org" target="_blank">
-    <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.7%2C%3C%3D3.11%5D-orange" alt="Python">
+    <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.8%2C%3C%3D3.11%5D-orange" alt="Python">
 </a>
 </p>
 
 
 ---
 
 # About us
@@ -80,18 +80,21 @@
 * <a href="https://www.youtube.com/channel/UCzcJtxfScoAtwFbxaLNnEtA" target="_blank">LOGYCA Youtube Channel</a>
 * <a href="https://www.linkedin.com/company/logyca" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="Linkedin"></a>
 * <a href="https://twitter.com/LOGYCA_Org" target="_blank"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter"></a>
 * <a href="https://www.facebook.com/OrganizacionLOGYCA/" target="_blank"><img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook"></a>
 
 ---
 
-# What's libraries
+# LOGYCA public libraries: Standard methods to connect to postgres
 
 * **Traversal libraries**: Standard methods to connect to postgres with dependency injection using yield to be used by microservices such as API(s), Workers or scripts.
 
+[Source code](https://github.com/logyca/python-libraries)
+| [Package (PyPI)](https://pypi.org/project/logyca-postgres/)
+
 ---
 
 # "pip install" dependency check
 The user must select the required libraries and versions for the project that uses this library, which validates that they are pre-installed in order to be installed.
 
 To install the libraries of the logyca postgres package verifying the SQLAlchemy prerequisite without validating connection drivers to postgres, use the following command:
 
@@ -340,7 +343,11 @@
 - Functionalities can be used in fastapi or workers like Azure Functions.
 - Examples of use are added to the documentation of the functions in docstring
 - In the samples folder of this library, there are complete working examples of using the code.
 
 ## [0.1.0] - 2024-05-21
 ### Added
 - Completion of testing and launch into production.
+
+## [0.1.2] - 2024-05-23
+### Added
+- Documentation integrated with github
```

#### html2text {}

```diff
@@ -1,65 +1,67 @@
-Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.1 Summary: An
+Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.2rc1 Summary: An
 integration package created by the company LOGYCA that connects Postgres and is
 used to standardize connections and dependency injection in synchronous or
 asynchronous mode. Tested in fastapi and in console/worker scripts. Home-page:
 https://github.com/logyca/ Author: Jaime Andres Cardona Carrillo Author-email:
-tecnologiaeinformacion@logyca.com License: MIT License Keywords:
-postgres,driver database Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Information
-Technology Classifier: Intended Audience :: System Administrators Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python Classifier: Topic :: Database Classifier: Topic
-:: Database :: Front-Ends Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Software Development Classifier: Typing :: Typed
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE.txt Requires-Dist: SQLAlchemy>=2.0.6 Requires-Dist: starlette>=0.24.0
-Provides-Extra: async Requires-Dist: SQLAlchemy>=2.0.6; extra == "async"
-Requires-Dist: starlette>=0.24.0; extra == "async" Requires-Dist:
-asyncpg>=0.27.0; extra == "async" Provides-Extra: sync-psycopg2 Requires-Dist:
-SQLAlchemy>=2.0.6; extra == "sync-psycopg2" Requires-Dist: starlette>=0.24.0;
-extra == "sync-psycopg2" Requires-Dist: psycopg2>=2.9.6; extra == "sync-
-psycopg2" Provides-Extra: sync-psycopg2-binary Requires-Dist:
-SQLAlchemy>=2.0.6; extra == "sync-psycopg2-binary" Requires-Dist:
-starlette>=0.24.0; extra == "sync-psycopg2-binary" Requires-Dist: psycopg2-
-binary>=2.9.6; extra == "sync-psycopg2-binary" Provides-Extra: async-sync-
-psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra == "async-sync-psycopg2"
-Requires-Dist: starlette>=0.24.0; extra == "async-sync-psycopg2" Requires-Dist:
-asyncpg>=0.27.0; extra == "async-sync-psycopg2" Requires-Dist: psycopg2>=2.9.6;
-extra == "async-sync-psycopg2" Provides-Extra: async-sync-psycopg2-binary
-Requires-Dist: SQLAlchemy>=2.0.6; extra == "async-sync-psycopg2-binary"
-Requires-Dist: starlette>=0.24.0; extra == "async-sync-psycopg2-binary"
-Requires-Dist: asyncpg>=0.27.0; extra == "async-sync-psycopg2-binary" Requires-
-Dist: psycopg2-binary>=2.9.6; extra == "async-sync-psycopg2-binary"
+jacardona@outlook.com License: MIT License Keywords: postgres,driver database
+Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Information Technology Classifier:
+Intended Audience :: System Administrators Classifier: License :: OSI Approved
+:: MIT License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+Classifier: Topic :: Database Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development Classifier: Typing :: Typed Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
+Dist: SQLAlchemy>=2.0.6 Requires-Dist: starlette>=0.24.0 Provides-Extra: async
+Requires-Dist: SQLAlchemy>=2.0.6; extra == "async" Requires-Dist:
+starlette>=0.24.0; extra == "async" Requires-Dist: asyncpg>=0.27.0; extra ==
+"async" Provides-Extra: sync-psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra
+== "sync-psycopg2" Requires-Dist: starlette>=0.24.0; extra == "sync-psycopg2"
+Requires-Dist: psycopg2>=2.9.6; extra == "sync-psycopg2" Provides-Extra: sync-
+psycopg2-binary Requires-Dist: SQLAlchemy>=2.0.6; extra == "sync-psycopg2-
+binary" Requires-Dist: starlette>=0.24.0; extra == "sync-psycopg2-binary"
+Requires-Dist: psycopg2-binary>=2.9.6; extra == "sync-psycopg2-binary"
+Provides-Extra: async-sync-psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra ==
+"async-sync-psycopg2" Requires-Dist: starlette>=0.24.0; extra == "async-sync-
+psycopg2" Requires-Dist: asyncpg>=0.27.0; extra == "async-sync-psycopg2"
+Requires-Dist: psycopg2>=2.9.6; extra == "async-sync-psycopg2" Provides-Extra:
+async-sync-psycopg2-binary Requires-Dist: SQLAlchemy>=2.0.6; extra == "async-
+sync-psycopg2-binary" Requires-Dist: starlette>=0.24.0; extra == "async-sync-
+psycopg2-binary" Requires-Dist: asyncpg>=0.27.0; extra == "async-sync-psycopg2-
+binary" Requires-Dist: psycopg2-binary>=2.9.6; extra == "async-sync-psycopg2-
+binary"
                                    _[_L_o_g_y_c_a_]
                             LLOOGGYYCCAA ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # About us * _L_O_G_Y_C_A_ _C_o_m_p_a_n_y * _L_O_G_Y_C_A_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l * _[_L_i_n_k_e_d_i_n_]*
-_[_T_w_i_t_t_e_r_]* _[_F_a_c_e_b_o_o_k_]--- # What's libraries * **Traversal libraries**: Standard
-methods to connect to postgres with dependency injection using yield to be used
-by microservices such as API(s), Workers or scripts. --- # "pip install"
-dependency check The user must select the required libraries and versions for
-the project that uses this library, which validates that they are pre-installed
-in order to be installed. To install the libraries of the logyca postgres
-package verifying the SQLAlchemy prerequisite without validating connection
-drivers to postgres, use the following command: ```Python # Check SQLAlchemy
-dependency that is installed pip install logyca_postgres ``` To install the
-logyca postgres package libraries and validate the postgres asynchronous or
-synchronous connection driver, use the following command: ```Python # Check
-asyncpg driver dependency that is installed pip install logyca_postgres[async]
-# Check psycopg2 driver dependency that is installed pip install
-logyca_postgres[sync-psycopg2] # Check psycopg2-binary driver dependency that
-is installed pip install logyca_postgres[sync-psycopg2-binary] # Check
-asyncpg+psycopg2-binary driver dependency that is installed pip install
+_[_T_w_i_t_t_e_r_]* _[_F_a_c_e_b_o_o_k_]--- # LOGYCA public libraries: Standard methods to connect
+to postgres * **Traversal libraries**: Standard methods to connect to postgres
+with dependency injection using yield to be used by microservices such as API
+(s), Workers or scripts. [Source code](https://github.com/logyca/python-
+libraries) | [Package (PyPI)](https://pypi.org/project/logyca-postgres/) --- #
+"pip install" dependency check The user must select the required libraries and
+versions for the project that uses this library, which validates that they are
+pre-installed in order to be installed. To install the libraries of the logyca
+postgres package verifying the SQLAlchemy prerequisite without validating
+connection drivers to postgres, use the following command: ```Python # Check
+SQLAlchemy dependency that is installed pip install logyca_postgres ``` To
+install the logyca postgres package libraries and validate the postgres
+asynchronous or synchronous connection driver, use the following command:
+```Python # Check asyncpg driver dependency that is installed pip install
+logyca_postgres[async] # Check psycopg2 driver dependency that is installed pip
+install logyca_postgres[sync-psycopg2] # Check psycopg2-binary driver
+dependency that is installed pip install logyca_postgres[sync-psycopg2-binary]
+# Check asyncpg+psycopg2-binary driver dependency that is installed pip install
 logyca_postgres[async-sync-psycopg2] ``` --- # Semantic Versioning logyca <
 MAJOR >.< MINOR >.< PATCH > * **MAJOR**: version when you make incompatible API
 changes * **MINOR**: version when you add functionality in a backwards
 compatible manner * **PATCH**: version when you make backwards compatible bug
 fixes ## Definitions for releasing versions * https://peps.python.org/pep-0440/
 - X.YaN (Alpha release): Identify and fix early-stage bugs. Not suitable for
 production use. - X.YbN (Beta release): Stabilize and refine features. Address
@@ -178,8 +180,9 @@
 Security in case of vulnerabilities. ## [0.0.1rc1] - 2024-04-22 ### Added -
 First tests using pypi.org in develop environment. - New functionality of
 asynchronous and synchronous connections to postgresql databases. -
 Functionalities can be used in fastapi or workers like Azure Functions. -
 Examples of use are added to the documentation of the functions in docstring -
 In the samples folder of this library, there are complete working examples of
 using the code. ## [0.1.0] - 2024-05-21 ### Added - Completion of testing and
-launch into production.
+launch into production. ## [0.1.2] - 2024-05-23 ### Added - Documentation
+integrated with github
```

### Comparing `logyca_postgres-0.1.1/README.md` & `logyca_postgres-0.1.2rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 00000190: 3c61 2068 7265 663d 2228 6874 7470 733a  <a href="(https:
 000001a0: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
 000001b0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
 000001c0: 223e 0d0a 2020 2020 3c69 6d67 2073 7263  ">..    <img src
 000001d0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
 000001e0: 6965 6c64 732e 696f 2f62 6164 6765 2f50  ields.io/badge/P
 000001f0: 7974 686f 6e2d 2535 4225 3345 2533 4433  ython-%5B%3E%3D3
-00000200: 2e37 2532 4325 3343 2533 4433 2e31 3125  .7%2C%3C%3D3.11%
+00000200: 2e38 2532 4325 3343 2533 4433 2e31 3125  .8%2C%3C%3D3.11%
 00000210: 3544 2d6f 7261 6e67 6522 2061 6c74 3d22  5D-orange" alt="
 00000220: 5079 7468 6f6e 223e 0d0a 3c2f 613e 0d0a  Python">..</a>..
 00000230: 3c2f 703e 0d0a 0d0a 0d0a 2d2d 2d0d 0a0d  </p>......---...
 00000240: 0a23 2041 626f 7574 2075 730d 0a0d 0a2a  .# About us....*
 00000250: 203c 6120 6872 6566 3d22 6874 7470 3a2f   <a href="http:/
 00000260: 2f6c 6f67 7963 612e 636f 6d22 2074 6172  /logyca.com" tar
 00000270: 6765 743d 225f 626c 616e 6b22 3e4c 4f47  get="_blank">LOG
@@ -78,708 +78,724 @@
 000004d0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
 000004e0: 6473 2e69 6f2f 6261 6467 652f 4661 6365  ds.io/badge/Face
 000004f0: 626f 6f6b 2d31 3837 3746 323f 7374 796c  book-1877F2?styl
 00000500: 653d 666f 722d 7468 652d 6261 6467 6526  e=for-the-badge&
 00000510: 6c6f 676f 3d66 6163 6562 6f6f 6b26 6c6f  logo=facebook&lo
 00000520: 676f 436f 6c6f 723d 7768 6974 6522 2061  goColor=white" a
 00000530: 6c74 3d22 4661 6365 626f 6f6b 223e 3c2f  lt="Facebook"></
-00000540: 613e 0d0a 0d0a 2d2d 2d0d 0a0d 0a23 2057  a>....---....# W
-00000550: 6861 7427 7320 6c69 6272 6172 6965 730d  hat's libraries.
-00000560: 0a0d 0a2a 202a 2a54 7261 7665 7273 616c  ...* **Traversal
-00000570: 206c 6962 7261 7269 6573 2a2a 3a20 5374   libraries**: St
-00000580: 616e 6461 7264 206d 6574 686f 6473 2074  andard methods t
-00000590: 6f20 636f 6e6e 6563 7420 746f 2070 6f73  o connect to pos
-000005a0: 7467 7265 7320 7769 7468 2064 6570 656e  tgres with depen
-000005b0: 6465 6e63 7920 696e 6a65 6374 696f 6e20  dency injection 
-000005c0: 7573 696e 6720 7969 656c 6420 746f 2062  using yield to b
-000005d0: 6520 7573 6564 2062 7920 6d69 6372 6f73  e used by micros
-000005e0: 6572 7669 6365 7320 7375 6368 2061 7320  ervices such as 
-000005f0: 4150 4928 7329 2c20 576f 726b 6572 7320  API(s), Workers 
-00000600: 6f72 2073 6372 6970 7473 2e0d 0a0d 0a2d  or scripts.....-
-00000610: 2d2d 0d0a 0d0a 2320 2270 6970 2069 6e73  --....# "pip ins
-00000620: 7461 6c6c 2220 6465 7065 6e64 656e 6379  tall" dependency
-00000630: 2063 6865 636b 0d0a 5468 6520 7573 6572   check..The user
-00000640: 206d 7573 7420 7365 6c65 6374 2074 6865   must select the
-00000650: 2072 6571 7569 7265 6420 6c69 6272 6172   required librar
-00000660: 6965 7320 616e 6420 7665 7273 696f 6e73  ies and versions
-00000670: 2066 6f72 2074 6865 2070 726f 6a65 6374   for the project
-00000680: 2074 6861 7420 7573 6573 2074 6869 7320   that uses this 
-00000690: 6c69 6272 6172 792c 2077 6869 6368 2076  library, which v
-000006a0: 616c 6964 6174 6573 2074 6861 7420 7468  alidates that th
-000006b0: 6579 2061 7265 2070 7265 2d69 6e73 7461  ey are pre-insta
-000006c0: 6c6c 6564 2069 6e20 6f72 6465 7220 746f  lled in order to
-000006d0: 2062 6520 696e 7374 616c 6c65 642e 0d0a   be installed...
-000006e0: 0d0a 546f 2069 6e73 7461 6c6c 2074 6865  ..To install the
-000006f0: 206c 6962 7261 7269 6573 206f 6620 7468   libraries of th
-00000700: 6520 6c6f 6779 6361 2070 6f73 7467 7265  e logyca postgre
-00000710: 7320 7061 636b 6167 6520 7665 7269 6679  s package verify
-00000720: 696e 6720 7468 6520 5351 4c41 6c63 6865  ing the SQLAlche
-00000730: 6d79 2070 7265 7265 7175 6973 6974 6520  my prerequisite 
-00000740: 7769 7468 6f75 7420 7661 6c69 6461 7469  without validati
-00000750: 6e67 2063 6f6e 6e65 6374 696f 6e20 6472  ng connection dr
-00000760: 6976 6572 7320 746f 2070 6f73 7467 7265  ivers to postgre
-00000770: 732c 2075 7365 2074 6865 2066 6f6c 6c6f  s, use the follo
-00000780: 7769 6e67 2063 6f6d 6d61 6e64 3a0d 0a0d  wing command:...
-00000790: 0a60 6060 5079 7468 6f6e 0d0a 2320 4368  .```Python..# Ch
-000007a0: 6563 6b20 5351 4c41 6c63 6865 6d79 2064  eck SQLAlchemy d
-000007b0: 6570 656e 6465 6e63 7920 7468 6174 2069  ependency that i
-000007c0: 7320 696e 7374 616c 6c65 640d 0a70 6970  s installed..pip
-000007d0: 2069 6e73 7461 6c6c 206c 6f67 7963 615f   install logyca_
-000007e0: 706f 7374 6772 6573 0d0a 6060 600d 0a0d  postgres..```...
-000007f0: 0a54 6f20 696e 7374 616c 6c20 7468 6520  .To install the 
-00000800: 6c6f 6779 6361 2070 6f73 7467 7265 7320  logyca postgres 
-00000810: 7061 636b 6167 6520 6c69 6272 6172 6965  package librarie
-00000820: 7320 616e 6420 7661 6c69 6461 7465 2074  s and validate t
-00000830: 6865 2070 6f73 7467 7265 7320 6173 796e  he postgres asyn
-00000840: 6368 726f 6e6f 7573 206f 7220 7379 6e63  chronous or sync
-00000850: 6872 6f6e 6f75 7320 636f 6e6e 6563 7469  hronous connecti
-00000860: 6f6e 2064 7269 7665 722c 2075 7365 2074  on driver, use t
-00000870: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00000880: 6d61 6e64 3a0d 0a0d 0a60 6060 5079 7468  mand:....```Pyth
-00000890: 6f6e 0d0a 2320 4368 6563 6b20 6173 796e  on..# Check asyn
-000008a0: 6370 6720 6472 6976 6572 2064 6570 656e  cpg driver depen
-000008b0: 6465 6e63 7920 7468 6174 2069 7320 696e  dency that is in
-000008c0: 7374 616c 6c65 640d 0a70 6970 2069 6e73  stalled..pip ins
-000008d0: 7461 6c6c 206c 6f67 7963 615f 706f 7374  tall logyca_post
-000008e0: 6772 6573 5b61 7379 6e63 5d0d 0a23 2043  gres[async]..# C
-000008f0: 6865 636b 2070 7379 636f 7067 3220 6472  heck psycopg2 dr
-00000900: 6976 6572 2064 6570 656e 6465 6e63 7920  iver dependency 
-00000910: 7468 6174 2069 7320 696e 7374 616c 6c65  that is installe
-00000920: 640d 0a70 6970 2069 6e73 7461 6c6c 206c  d..pip install l
-00000930: 6f67 7963 615f 706f 7374 6772 6573 5b73  ogyca_postgres[s
-00000940: 796e 632d 7073 7963 6f70 6732 5d0d 0a23  ync-psycopg2]..#
-00000950: 2043 6865 636b 2070 7379 636f 7067 322d   Check psycopg2-
-00000960: 6269 6e61 7279 2064 7269 7665 7220 6465  binary driver de
-00000970: 7065 6e64 656e 6379 2074 6861 7420 6973  pendency that is
-00000980: 2069 6e73 7461 6c6c 6564 0d0a 7069 7020   installed..pip 
-00000990: 696e 7374 616c 6c20 6c6f 6779 6361 5f70  install logyca_p
-000009a0: 6f73 7467 7265 735b 7379 6e63 2d70 7379  ostgres[sync-psy
-000009b0: 636f 7067 322d 6269 6e61 7279 5d0d 0a23  copg2-binary]..#
-000009c0: 2043 6865 636b 2061 7379 6e63 7067 2b70   Check asyncpg+p
-000009d0: 7379 636f 7067 322d 6269 6e61 7279 2064  sycopg2-binary d
-000009e0: 7269 7665 7220 6465 7065 6e64 656e 6379  river dependency
-000009f0: 2074 6861 7420 6973 2069 6e73 7461 6c6c   that is install
-00000a00: 6564 0d0a 7069 7020 696e 7374 616c 6c20  ed..pip install 
-00000a10: 6c6f 6779 6361 5f70 6f73 7467 7265 735b  logyca_postgres[
-00000a20: 6173 796e 632d 7379 6e63 2d70 7379 636f  async-sync-psyco
-00000a30: 7067 325d 0d0a 6060 600d 0a2d 2d2d 0d0a  pg2]..```..---..
-00000a40: 0d0a 2320 5365 6d61 6e74 6963 2056 6572  ..# Semantic Ver
-00000a50: 7369 6f6e 696e 670d 0a0d 0a6c 6f67 7963  sioning....logyc
-00000a60: 6120 3c20 4d41 4a4f 5220 3e2e 3c20 4d49  a < MAJOR >.< MI
-00000a70: 4e4f 5220 3e2e 3c20 5041 5443 4820 3e0d  NOR >.< PATCH >.
-00000a80: 0a0d 0a2a 202a 2a4d 414a 4f52 2a2a 3a20  ...* **MAJOR**: 
-00000a90: 7665 7273 696f 6e20 7768 656e 2079 6f75  version when you
-00000aa0: 206d 616b 6520 696e 636f 6d70 6174 6962   make incompatib
-00000ab0: 6c65 2041 5049 2063 6861 6e67 6573 0d0a  le API changes..
-00000ac0: 2a20 2a2a 4d49 4e4f 522a 2a3a 2076 6572  * **MINOR**: ver
-00000ad0: 7369 6f6e 2077 6865 6e20 796f 7520 6164  sion when you ad
-00000ae0: 6420 6675 6e63 7469 6f6e 616c 6974 7920  d functionality 
-00000af0: 696e 2061 2062 6163 6b77 6172 6473 2063  in a backwards c
-00000b00: 6f6d 7061 7469 626c 6520 6d61 6e6e 6572  ompatible manner
-00000b10: 0d0a 2a20 2a2a 5041 5443 482a 2a3a 2076  ..* **PATCH**: v
-00000b20: 6572 7369 6f6e 2077 6865 6e20 796f 7520  ersion when you 
-00000b30: 6d61 6b65 2062 6163 6b77 6172 6473 2063  make backwards c
-00000b40: 6f6d 7061 7469 626c 6520 6275 6720 6669  ompatible bug fi
-00000b50: 7865 730d 0a0d 0a23 2320 4465 6669 6e69  xes....## Defini
-00000b60: 7469 6f6e 7320 666f 7220 7265 6c65 6173  tions for releas
-00000b70: 696e 6720 7665 7273 696f 6e73 0d0a 2a20  ing versions..* 
-00000b80: 6874 7470 733a 2f2f 7065 7073 2e70 7974  https://peps.pyt
-00000b90: 686f 6e2e 6f72 672f 7065 702d 3034 3430  hon.org/pep-0440
-00000ba0: 2f0d 0a0d 0a20 2020 202d 2058 2e59 614e  /....    - X.YaN
-00000bb0: 2028 416c 7068 6120 7265 6c65 6173 6529   (Alpha release)
-00000bc0: 3a20 4964 656e 7469 6679 2061 6e64 2066  : Identify and f
-00000bd0: 6978 2065 6172 6c79 2d73 7461 6765 2062  ix early-stage b
-00000be0: 7567 732e 204e 6f74 2073 7569 7461 626c  ugs. Not suitabl
-00000bf0: 6520 666f 7220 7072 6f64 7563 7469 6f6e  e for production
-00000c00: 2075 7365 2e0d 0a20 2020 202d 2058 2e59   use...    - X.Y
-00000c10: 624e 2028 4265 7461 2072 656c 6561 7365  bN (Beta release
-00000c20: 293a 2053 7461 6269 6c69 7a65 2061 6e64  ): Stabilize and
-00000c30: 2072 6566 696e 6520 6665 6174 7572 6573   refine features
-00000c40: 2e20 4164 6472 6573 7320 7265 706f 7274  . Address report
-00000c50: 6564 2062 7567 732e 2050 7265 7061 7265  ed bugs. Prepare
-00000c60: 2066 6f72 206f 6666 6963 6961 6c20 7265   for official re
-00000c70: 6c65 6173 652e 0d0a 2020 2020 2d20 582e  lease...    - X.
-00000c80: 5972 634e 2028 5265 6c65 6173 6520 6361  YrcN (Release ca
-00000c90: 6e64 6964 6174 6529 3a20 4669 6e61 6c20  ndidate): Final 
-00000ca0: 7665 7273 696f 6e20 6265 666f 7265 206f  version before o
-00000cb0: 6666 6963 6961 6c20 7265 6c65 6173 652e  fficial release.
-00000cc0: 2041 7373 756d 6573 2061 6c6c 206d 616a   Assumes all maj
-00000cd0: 6f72 2066 6561 7475 7265 7320 6172 6520  or features are 
-00000ce0: 636f 6d70 6c65 7465 2061 6e64 2073 7461  complete and sta
-00000cf0: 626c 652e 2052 6563 6f6d 6d65 6e64 6564  ble. Recommended
-00000d00: 2066 6f72 2074 6573 7469 6e67 2069 6e20   for testing in 
-00000d10: 6e6f 6e2d 6372 6974 6963 616c 2065 6e76  non-critical env
-00000d20: 6972 6f6e 6d65 6e74 732e 0d0a 2020 2020  ironments...    
-00000d30: 2d20 582e 5920 2846 696e 616c 2072 656c  - X.Y (Final rel
-00000d40: 6561 7365 2f53 7461 626c 652f 5072 6f64  ease/Stable/Prod
-00000d50: 7563 7469 6f6e 293a 2043 6f6d 706c 6574  uction): Complet
-00000d60: 6564 2c20 7374 6162 6c65 2076 6572 7369  ed, stable versi
-00000d70: 6f6e 2072 6561 6479 2066 6f72 2075 7365  on ready for use
-00000d80: 2069 6e20 7072 6f64 7563 7469 6f6e 2e20   in production. 
-00000d90: 4675 6c6c 2072 656c 6561 7365 2066 6f72  Full release for
-00000da0: 2070 7562 6c69 6320 7573 652e 0d0a 0d0a   public use.....
-00000db0: 2d2d 2d0d 0a0d 0a23 2045 7861 6d70 6c65  ---....# Example
-00000dc0: 206f 6620 636f 6e63 6570 7473 2074 6861   of concepts tha
-00000dd0: 7420 7573 6520 6120 6c69 6272 6172 7920  t use a library 
-00000de0: 7769 7468 2061 2073 696e 676c 6574 6f6e  with a singleton
-00000df0: 2070 6174 7465 726e 2061 6e64 2063 6f6e   pattern and con
-00000e00: 6e65 6374 696f 6e20 746f 206d 756c 7469  nection to multi
-00000e10: 706c 6520 656e 6769 6e65 7320 7769 7468  ple engines with
-00000e20: 2079 6965 6c64 2064 6570 656e 6465 6e63   yield dependenc
-00000e30: 7920 696e 6a65 6374 696f 6e0d 0a0d 0a54  y injection....T
-00000e40: 6865 206c 6962 7261 7279 2075 7365 7320  he library uses 
-00000e50: 6120 7369 6e67 6c65 746f 6e20 7061 7474  a singleton patt
-00000e60: 6572 6e20 2263 6c61 7373 2053 796e 6343  ern "class SyncC
-00000e70: 6f6e 6e45 6e67 696e 6528 6d65 7461 636c  onnEngine(metacl
-00000e80: 6173 733d 5369 6e67 6c65 746f 6e29 3a22  ass=Singleton):"
-00000e90: 2c20 7768 6572 6520 7468 6520 636c 6173  , where the clas
-00000ea0: 7320 6973 2061 6c6c 6f77 6564 2074 6f20  s is allowed to 
-00000eb0: 6265 2069 6e73 7461 6e74 6961 7465 6420  be instantiated 
-00000ec0: 6f6e 6c79 206f 6e63 652e 2059 6f75 2063  only once. You c
-00000ed0: 616e 2063 7265 6174 6520 616e 6f74 6865  an create anothe
-00000ee0: 7220 636f 6e6e 6563 7469 6f6e 2074 6f20  r connection to 
-00000ef0: 616e 6f74 6865 7220 656e 6769 6e65 2062  another engine b
-00000f00: 7574 2079 6f75 206d 7573 7420 6372 6561  ut you must crea
-00000f10: 7465 2061 6e20 696e 6865 7269 7465 6420  te an inherited 
-00000f20: 636c 6173 7320 696e 206f 7264 6572 2074  class in order t
-00000f30: 6f20 6372 6561 7465 2061 206e 6577 2063  o create a new c
-00000f40: 6f6e 6669 6775 7261 7469 6f6e 2069 6e73  onfiguration ins
-00000f50: 7461 6e63 652e 0d0a 0d0a 4578 616d 706c  tance.....Exampl
-00000f60: 653a 0d0a 636c 6173 7320 5379 6e63 436f  e:..class SyncCo
-00000f70: 6e6e 456e 6769 6e65 5828 5379 6e63 436f  nnEngineX(SyncCo
-00000f80: 6e6e 456e 6769 6e65 293a 0d0a 2020 2020  nnEngine):..    
-00000f90: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00000fa0: 662c 2075 726c 5f63 6f6e 6e65 6374 696f  f, url_connectio
-00000fb0: 6e2c 7365 7276 6572 5f73 6574 7469 6e67  n,server_setting
-00000fc0: 7329 3a0d 0a20 2020 2020 2020 2073 7570  s):..        sup
-00000fd0: 6572 2829 2e5f 5f69 6e69 745f 5f28 7572  er().__init__(ur
-00000fe0: 6c5f 636f 6e6e 6563 7469 6f6e 2c73 6572  l_connection,ser
-00000ff0: 7665 725f 7365 7474 696e 6773 290d 0a73  ver_settings)..s
-00001000: 796e 635f 7365 7373 696f 6e5f 783d 5379  ync_session_x=Sy
-00001010: 6e63 436f 6e6e 456e 6769 6e65 5828 0d0a  ncConnEngineX(..
-00001020: 2020 2020 7572 6c5f 636f 6e6e 6563 7469      url_connecti
-00001030: 6f6e 3d53 796e 6343 6f6e 6e45 6e67 696e  on=SyncConnEngin
-00001040: 652e 6275 696c 645f 7572 6c5f 636f 6e6e  e.build_url_conn
-00001050: 6563 7469 6f6e 2875 7365 723d 7365 7474  ection(user=sett
-00001060: 696e 6773 2e44 425f 5553 4552 5f58 2c70  ings.DB_USER_X,p
-00001070: 6173 7377 6f72 643d 7365 7474 696e 6773  assword=settings
-00001080: 2e44 425f 5041 5353 5f58 2c68 6f73 743d  .DB_PASS_X,host=
-00001090: 7365 7474 696e 6773 2e44 425f 484f 5354  settings.DB_HOST
-000010a0: 5f58 2c70 6f72 743d 7365 7474 696e 6773  _X,port=settings
-000010b0: 2e44 425f 504f 5254 5f58 2c64 6174 6162  .DB_PORT_X,datab
-000010c0: 6173 653d 7365 7474 696e 6773 2e44 425f  ase=settings.DB_
-000010d0: 4e41 4d45 5f58 2c73 736c 5f65 6e61 626c  NAME_X,ssl_enabl
-000010e0: 653d 7365 7474 696e 6773 2e44 425f 5353  e=settings.DB_SS
-000010f0: 4c5f 5829 2c0d 0a20 2020 2073 6572 7665  L_X),..    serve
-00001100: 725f 7365 7474 696e 6773 3d53 796e 6343  r_settings=SyncC
-00001110: 6f6e 6e45 6e67 696e 652e 7365 7276 6572  onnEngine.server
-00001120: 5f73 6574 7469 6e67 7328 706f 6f6c 5f73  _settings(pool_s
-00001130: 697a 653d 352c 6d61 785f 6f76 6572 666c  ize=5,max_overfl
-00001140: 6f77 3d31 2c70 6f6f 6c5f 7265 6379 636c  ow=1,pool_recycl
-00001150: 653d 3130 3830 302c 6170 706c 6963 6174  e=10800,applicat
-00001160: 696f 6e5f 6e61 6d65 3d66 227b 4170 702e  ion_name=f"{App.
-00001170: 5365 7474 696e 6773 2e4e 414d 457d 202d  Settings.NAME} -
-00001180: 2053 796e 6343 6f6e 6e45 6e67 696e 6558   SyncConnEngineX
-00001190: 2229 0d0a 2020 2020 290d 0a0d 0a23 2320  ")..    )....## 
-000011a0: 4173 796e 6368 726f 6e6f 7573 206d 6f64  Asynchronous mod
-000011b0: 650d 0a46 6173 7441 5049 0d0a 6060 6070  e..FastAPI..```p
-000011c0: 7974 686f 6e0d 0a66 726f 6d20 6661 7374  ython..from fast
-000011d0: 6170 6920 696d 706f 7274 2046 6173 7441  api import FastA
-000011e0: 5049 2c20 4465 7065 6e64 732c 2048 5454  PI, Depends, HTT
-000011f0: 5045 7863 6570 7469 6f6e 0d0a 6672 6f6d  PException..from
-00001200: 206c 6f67 7963 615f 706f 7374 6772 6573   logyca_postgres
-00001210: 2069 6d70 6f72 7420 4173 796e 6343 6f6e   import AsyncCon
-00001220: 6e45 6e67 696e 652c 2063 6f6d 6d69 745f  nEngine, commit_
-00001230: 726f 6c6c 6261 636b 5f61 7379 6e63 2c20  rollback_async, 
-00001240: 6368 6563 6b5f 636f 6e6e 6563 7469 6f6e  check_connection
-00001250: 5f61 7379 6e63 0d0a 6672 6f6d 2073 716c  _async..from sql
-00001260: 616c 6368 656d 7920 696d 706f 7274 2074  alchemy import t
-00001270: 6578 7420 6173 2074 6578 745f 746f 5f73  ext as text_to_s
-00001280: 716c 0d0a 6672 6f6d 2073 716c 616c 6368  ql..from sqlalch
-00001290: 656d 792e 6578 742e 6173 796e 6369 6f20  emy.ext.asyncio 
-000012a0: 696d 706f 7274 2041 7379 6e63 5365 7373  import AsyncSess
-000012b0: 696f 6e0d 0a69 6d70 6f72 7420 6f73 0d0a  ion..import os..
-000012c0: 0d0a 4442 5f55 5345 523d 6f73 2e67 6574  ..DB_USER=os.get
-000012d0: 656e 7628 2744 425f 5553 4552 272c 2770  env('DB_USER','p
-000012e0: 6f73 7467 7265 7327 290d 0a44 425f 5041  ostgres')..DB_PA
-000012f0: 5353 3d6f 732e 6765 7465 6e76 2827 4442  SS=os.getenv('DB
-00001300: 5f50 4153 5327 2c27 7878 7827 290d 0a44  _PASS','xxx')..D
-00001310: 425f 484f 5354 3d6f 732e 6765 7465 6e76  B_HOST=os.getenv
-00001320: 2827 4442 5f48 4f53 5427 2c27 6c6f 6361  ('DB_HOST','loca
-00001330: 6c68 6f73 7427 290d 0a44 425f 504f 5254  lhost')..DB_PORT
-00001340: 3d6f 732e 6765 7465 6e76 2827 4442 5f50  =os.getenv('DB_P
-00001350: 4f52 5427 2c35 3433 3229 0d0a 4442 5f4e  ORT',5432)..DB_N
-00001360: 414d 453d 6f73 2e67 6574 656e 7628 2744  AME=os.getenv('D
-00001370: 425f 4e41 4d45 272c 2774 6573 7427 290d  B_NAME','test').
-00001380: 0a73 736c 5f65 6e61 626c 655f 6c69 6b65  .ssl_enable_like
-00001390: 5f6c 6f63 616c 5f64 6f63 6b65 725f 636f  _local_docker_co
-000013a0: 6e74 6169 6e65 723d 4661 6c73 650d 0a0d  ntainer=False...
-000013b0: 0a61 7070 203d 2046 6173 7441 5049 2829  .app = FastAPI()
-000013c0: 0d0a 0d0a 636f 6e6e 5f61 7379 6e63 5f73  ....conn_async_s
-000013d0: 6573 7369 6f6e 3d41 7379 6e63 436f 6e6e  ession=AsyncConn
-000013e0: 456e 6769 6e65 280d 0a20 2020 2075 726c  Engine(..    url
-000013f0: 5f63 6f6e 6e65 6374 696f 6e3d 4173 796e  _connection=Asyn
-00001400: 6343 6f6e 6e45 6e67 696e 652e 6275 696c  cConnEngine.buil
-00001410: 645f 7572 6c5f 636f 6e6e 6563 7469 6f6e  d_url_connection
-00001420: 2875 7365 723d 4442 5f55 5345 522c 7061  (user=DB_USER,pa
-00001430: 7373 776f 7264 3d44 425f 5041 5353 2c68  ssword=DB_PASS,h
-00001440: 6f73 743d 4442 5f48 4f53 542c 706f 7274  ost=DB_HOST,port
-00001450: 3d44 425f 504f 5254 2c64 6174 6162 6173  =DB_PORT,databas
-00001460: 653d 4442 5f4e 414d 452c 7373 6c5f 656e  e=DB_NAME,ssl_en
-00001470: 6162 6c65 3d73 736c 5f65 6e61 626c 655f  able=ssl_enable_
-00001480: 6c69 6b65 5f6c 6f63 616c 5f64 6f63 6b65  like_local_docke
-00001490: 725f 636f 6e74 6169 6e65 7229 2c0d 0a20  r_container),.. 
-000014a0: 2020 2073 6572 7665 725f 7365 7474 696e     server_settin
-000014b0: 6773 3d41 7379 6e63 436f 6e6e 456e 6769  gs=AsyncConnEngi
-000014c0: 6e65 2e73 6572 7665 725f 7365 7474 696e  ne.server_settin
-000014d0: 6773 2870 6f6f 6c5f 7369 7a65 3d35 2c6d  gs(pool_size=5,m
-000014e0: 6178 5f6f 7665 7266 6c6f 773d 312c 706f  ax_overflow=1,po
-000014f0: 6f6c 5f72 6563 7963 6c65 3d31 3038 3030  ol_recycle=10800
-00001500: 2c61 7070 6c69 6361 7469 6f6e 5f6e 616d  ,application_nam
-00001510: 653d 224d 7941 7070 202d 2041 7379 6e63  e="MyApp - Async
-00001520: 436f 6e6e 456e 6769 6e65 2229 0d0a 2020  ConnEngine")..  
-00001530: 2020 290d 0a0d 0a27 2727 0d0a 5468 6520    )....'''..The 
-00001540: 636f 6e6e 6563 7469 6f6e 2070 6f6f 6c20  connection pool 
-00001550: 2870 6f6f 6c5f 7369 7a65 2920 6166 7465  (pool_size) afte
-00001560: 7220 7468 6520 6669 7273 7420 7175 6572  r the first quer
-00001570: 7920 7769 6c6c 2072 656d 6169 6e20 6f70  y will remain op
-00001580: 656e 2075 6e74 696c 2074 6865 2061 7070  en until the app
-00001590: 6c69 6361 7469 6f6e 2069 7320 7374 6f70  lication is stop
-000015a0: 7065 642e 0d0a 2727 270d 0a0d 0a40 6170  ped...'''....@ap
-000015b0: 702e 6765 7428 222f 7369 6d75 6c61 7465  p.get("/simulate
-000015c0: 645f 7175 6572 795f 6173 796e 632f 2229  d_query_async/")
-000015d0: 0d0a 6173 796e 6320 6465 6620 7265 6164  ..async def read
-000015e0: 5f69 7465 6d28 6173 796e 635f 7365 7373  _item(async_sess
-000015f0: 696f 6e3a 4173 796e 6353 6573 7369 6f6e  ion:AsyncSession
-00001600: 203d 2044 6570 656e 6473 2863 6f6e 6e5f   = Depends(conn_
-00001610: 6173 796e 635f 7365 7373 696f 6e29 293a  async_session)):
-00001620: 0d0a 2020 2020 7472 793a 0d0a 2020 2020  ..    try:..    
-00001630: 2020 2020 7374 6174 7573 2c20 6461 7465      status, date
-00001640: 5f74 696d 655f 6368 6563 6b5f 636f 6e6e  _time_check_conn
-00001650: 203d 2061 7761 6974 2063 6865 636b 5f63   = await check_c
-00001660: 6f6e 6e65 6374 696f 6e5f 6173 796e 6328  onnection_async(
-00001670: 6173 796e 635f 7365 7373 696f 6e29 0d0a  async_session)..
-00001680: 2020 2020 2020 2020 6966 2873 7461 7475          if(statu
-00001690: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
-000016a0: 2071 7565 7279 203d 2074 6578 745f 746f   query = text_to
-000016b0: 5f73 716c 2822 5345 4c45 4354 206e 6f77  _sql("SELECT now
-000016c0: 2829 3b22 290d 0a20 2020 2020 2020 2020  ();")..         
-000016d0: 2020 2072 6573 756c 7420 3d20 6177 6169     result = awai
-000016e0: 7420 6173 796e 635f 7365 7373 696f 6e2e  t async_session.
-000016f0: 6578 6563 7574 6528 7175 6572 7929 0d0a  execute(query)..
-00001700: 2020 2020 2020 2020 2020 2020 7369 6d75              simu
-00001710: 6c61 7465 645f 7175 6572 7920 3d20 7265  lated_query = re
-00001720: 7375 6c74 2e73 6361 6c61 725f 6f6e 655f  sult.scalar_one_
-00001730: 6f72 5f6e 6f6e 6528 290d 0a20 2020 2020  or_none()..     
-00001740: 2020 2020 2020 2061 7761 6974 2063 6f6d         await com
-00001750: 6d69 745f 726f 6c6c 6261 636b 5f61 7379  mit_rollback_asy
-00001760: 6e63 2861 7379 6e63 5f73 6573 7369 6f6e  nc(async_session
+00000540: 613e 0d0a 0d0a 2d2d 2d0d 0a0d 0a23 204c  a>....---....# L
+00000550: 4f47 5943 4120 7075 626c 6963 206c 6962  OGYCA public lib
+00000560: 7261 7269 6573 3a20 5374 616e 6461 7264  raries: Standard
+00000570: 206d 6574 686f 6473 2074 6f20 636f 6e6e   methods to conn
+00000580: 6563 7420 746f 2070 6f73 7467 7265 730d  ect to postgres.
+00000590: 0a0d 0a2a 202a 2a54 7261 7665 7273 616c  ...* **Traversal
+000005a0: 206c 6962 7261 7269 6573 2a2a 3a20 5374   libraries**: St
+000005b0: 616e 6461 7264 206d 6574 686f 6473 2074  andard methods t
+000005c0: 6f20 636f 6e6e 6563 7420 746f 2070 6f73  o connect to pos
+000005d0: 7467 7265 7320 7769 7468 2064 6570 656e  tgres with depen
+000005e0: 6465 6e63 7920 696e 6a65 6374 696f 6e20  dency injection 
+000005f0: 7573 696e 6720 7969 656c 6420 746f 2062  using yield to b
+00000600: 6520 7573 6564 2062 7920 6d69 6372 6f73  e used by micros
+00000610: 6572 7669 6365 7320 7375 6368 2061 7320  ervices such as 
+00000620: 4150 4928 7329 2c20 576f 726b 6572 7320  API(s), Workers 
+00000630: 6f72 2073 6372 6970 7473 2e0d 0a0d 0a5b  or scripts.....[
+00000640: 536f 7572 6365 2063 6f64 655d 2868 7474  Source code](htt
+00000650: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000660: 6c6f 6779 6361 2f70 7974 686f 6e2d 6c69  logyca/python-li
+00000670: 6272 6172 6965 7329 0d0a 7c20 5b50 6163  braries)..| [Pac
+00000680: 6b61 6765 2028 5079 5049 295d 2868 7474  kage (PyPI)](htt
+00000690: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+000006a0: 6f6a 6563 742f 6c6f 6779 6361 2d70 6f73  oject/logyca-pos
+000006b0: 7467 7265 732f 290d 0a0d 0a2d 2d2d 0d0a  tgres/)....---..
+000006c0: 0d0a 2320 2270 6970 2069 6e73 7461 6c6c  ..# "pip install
+000006d0: 2220 6465 7065 6e64 656e 6379 2063 6865  " dependency che
+000006e0: 636b 0d0a 5468 6520 7573 6572 206d 7573  ck..The user mus
+000006f0: 7420 7365 6c65 6374 2074 6865 2072 6571  t select the req
+00000700: 7569 7265 6420 6c69 6272 6172 6965 7320  uired libraries 
+00000710: 616e 6420 7665 7273 696f 6e73 2066 6f72  and versions for
+00000720: 2074 6865 2070 726f 6a65 6374 2074 6861   the project tha
+00000730: 7420 7573 6573 2074 6869 7320 6c69 6272  t uses this libr
+00000740: 6172 792c 2077 6869 6368 2076 616c 6964  ary, which valid
+00000750: 6174 6573 2074 6861 7420 7468 6579 2061  ates that they a
+00000760: 7265 2070 7265 2d69 6e73 7461 6c6c 6564  re pre-installed
+00000770: 2069 6e20 6f72 6465 7220 746f 2062 6520   in order to be 
+00000780: 696e 7374 616c 6c65 642e 0d0a 0d0a 546f  installed.....To
+00000790: 2069 6e73 7461 6c6c 2074 6865 206c 6962   install the lib
+000007a0: 7261 7269 6573 206f 6620 7468 6520 6c6f  raries of the lo
+000007b0: 6779 6361 2070 6f73 7467 7265 7320 7061  gyca postgres pa
+000007c0: 636b 6167 6520 7665 7269 6679 696e 6720  ckage verifying 
+000007d0: 7468 6520 5351 4c41 6c63 6865 6d79 2070  the SQLAlchemy p
+000007e0: 7265 7265 7175 6973 6974 6520 7769 7468  rerequisite with
+000007f0: 6f75 7420 7661 6c69 6461 7469 6e67 2063  out validating c
+00000800: 6f6e 6e65 6374 696f 6e20 6472 6976 6572  onnection driver
+00000810: 7320 746f 2070 6f73 7467 7265 732c 2075  s to postgres, u
+00000820: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
+00000830: 2063 6f6d 6d61 6e64 3a0d 0a0d 0a60 6060   command:....```
+00000840: 5079 7468 6f6e 0d0a 2320 4368 6563 6b20  Python..# Check 
+00000850: 5351 4c41 6c63 6865 6d79 2064 6570 656e  SQLAlchemy depen
+00000860: 6465 6e63 7920 7468 6174 2069 7320 696e  dency that is in
+00000870: 7374 616c 6c65 640d 0a70 6970 2069 6e73  stalled..pip ins
+00000880: 7461 6c6c 206c 6f67 7963 615f 706f 7374  tall logyca_post
+00000890: 6772 6573 0d0a 6060 600d 0a0d 0a54 6f20  gres..```....To 
+000008a0: 696e 7374 616c 6c20 7468 6520 6c6f 6779  install the logy
+000008b0: 6361 2070 6f73 7467 7265 7320 7061 636b  ca postgres pack
+000008c0: 6167 6520 6c69 6272 6172 6965 7320 616e  age libraries an
+000008d0: 6420 7661 6c69 6461 7465 2074 6865 2070  d validate the p
+000008e0: 6f73 7467 7265 7320 6173 796e 6368 726f  ostgres asynchro
+000008f0: 6e6f 7573 206f 7220 7379 6e63 6872 6f6e  nous or synchron
+00000900: 6f75 7320 636f 6e6e 6563 7469 6f6e 2064  ous connection d
+00000910: 7269 7665 722c 2075 7365 2074 6865 2066  river, use the f
+00000920: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00000930: 3a0d 0a0d 0a60 6060 5079 7468 6f6e 0d0a  :....```Python..
+00000940: 2320 4368 6563 6b20 6173 796e 6370 6720  # Check asyncpg 
+00000950: 6472 6976 6572 2064 6570 656e 6465 6e63  driver dependenc
+00000960: 7920 7468 6174 2069 7320 696e 7374 616c  y that is instal
+00000970: 6c65 640d 0a70 6970 2069 6e73 7461 6c6c  led..pip install
+00000980: 206c 6f67 7963 615f 706f 7374 6772 6573   logyca_postgres
+00000990: 5b61 7379 6e63 5d0d 0a23 2043 6865 636b  [async]..# Check
+000009a0: 2070 7379 636f 7067 3220 6472 6976 6572   psycopg2 driver
+000009b0: 2064 6570 656e 6465 6e63 7920 7468 6174   dependency that
+000009c0: 2069 7320 696e 7374 616c 6c65 640d 0a70   is installed..p
+000009d0: 6970 2069 6e73 7461 6c6c 206c 6f67 7963  ip install logyc
+000009e0: 615f 706f 7374 6772 6573 5b73 796e 632d  a_postgres[sync-
+000009f0: 7073 7963 6f70 6732 5d0d 0a23 2043 6865  psycopg2]..# Che
+00000a00: 636b 2070 7379 636f 7067 322d 6269 6e61  ck psycopg2-bina
+00000a10: 7279 2064 7269 7665 7220 6465 7065 6e64  ry driver depend
+00000a20: 656e 6379 2074 6861 7420 6973 2069 6e73  ency that is ins
+00000a30: 7461 6c6c 6564 0d0a 7069 7020 696e 7374  talled..pip inst
+00000a40: 616c 6c20 6c6f 6779 6361 5f70 6f73 7467  all logyca_postg
+00000a50: 7265 735b 7379 6e63 2d70 7379 636f 7067  res[sync-psycopg
+00000a60: 322d 6269 6e61 7279 5d0d 0a23 2043 6865  2-binary]..# Che
+00000a70: 636b 2061 7379 6e63 7067 2b70 7379 636f  ck asyncpg+psyco
+00000a80: 7067 322d 6269 6e61 7279 2064 7269 7665  pg2-binary drive
+00000a90: 7220 6465 7065 6e64 656e 6379 2074 6861  r dependency tha
+00000aa0: 7420 6973 2069 6e73 7461 6c6c 6564 0d0a  t is installed..
+00000ab0: 7069 7020 696e 7374 616c 6c20 6c6f 6779  pip install logy
+00000ac0: 6361 5f70 6f73 7467 7265 735b 6173 796e  ca_postgres[asyn
+00000ad0: 632d 7379 6e63 2d70 7379 636f 7067 325d  c-sync-psycopg2]
+00000ae0: 0d0a 6060 600d 0a2d 2d2d 0d0a 0d0a 2320  ..```..---....# 
+00000af0: 5365 6d61 6e74 6963 2056 6572 7369 6f6e  Semantic Version
+00000b00: 696e 670d 0a0d 0a6c 6f67 7963 6120 3c20  ing....logyca < 
+00000b10: 4d41 4a4f 5220 3e2e 3c20 4d49 4e4f 5220  MAJOR >.< MINOR 
+00000b20: 3e2e 3c20 5041 5443 4820 3e0d 0a0d 0a2a  >.< PATCH >....*
+00000b30: 202a 2a4d 414a 4f52 2a2a 3a20 7665 7273   **MAJOR**: vers
+00000b40: 696f 6e20 7768 656e 2079 6f75 206d 616b  ion when you mak
+00000b50: 6520 696e 636f 6d70 6174 6962 6c65 2041  e incompatible A
+00000b60: 5049 2063 6861 6e67 6573 0d0a 2a20 2a2a  PI changes..* **
+00000b70: 4d49 4e4f 522a 2a3a 2076 6572 7369 6f6e  MINOR**: version
+00000b80: 2077 6865 6e20 796f 7520 6164 6420 6675   when you add fu
+00000b90: 6e63 7469 6f6e 616c 6974 7920 696e 2061  nctionality in a
+00000ba0: 2062 6163 6b77 6172 6473 2063 6f6d 7061   backwards compa
+00000bb0: 7469 626c 6520 6d61 6e6e 6572 0d0a 2a20  tible manner..* 
+00000bc0: 2a2a 5041 5443 482a 2a3a 2076 6572 7369  **PATCH**: versi
+00000bd0: 6f6e 2077 6865 6e20 796f 7520 6d61 6b65  on when you make
+00000be0: 2062 6163 6b77 6172 6473 2063 6f6d 7061   backwards compa
+00000bf0: 7469 626c 6520 6275 6720 6669 7865 730d  tible bug fixes.
+00000c00: 0a0d 0a23 2320 4465 6669 6e69 7469 6f6e  ...## Definition
+00000c10: 7320 666f 7220 7265 6c65 6173 696e 6720  s for releasing 
+00000c20: 7665 7273 696f 6e73 0d0a 2a20 6874 7470  versions..* http
+00000c30: 733a 2f2f 7065 7073 2e70 7974 686f 6e2e  s://peps.python.
+00000c40: 6f72 672f 7065 702d 3034 3430 2f0d 0a0d  org/pep-0440/...
+00000c50: 0a20 2020 202d 2058 2e59 614e 2028 416c  .    - X.YaN (Al
+00000c60: 7068 6120 7265 6c65 6173 6529 3a20 4964  pha release): Id
+00000c70: 656e 7469 6679 2061 6e64 2066 6978 2065  entify and fix e
+00000c80: 6172 6c79 2d73 7461 6765 2062 7567 732e  arly-stage bugs.
+00000c90: 204e 6f74 2073 7569 7461 626c 6520 666f   Not suitable fo
+00000ca0: 7220 7072 6f64 7563 7469 6f6e 2075 7365  r production use
+00000cb0: 2e0d 0a20 2020 202d 2058 2e59 624e 2028  ...    - X.YbN (
+00000cc0: 4265 7461 2072 656c 6561 7365 293a 2053  Beta release): S
+00000cd0: 7461 6269 6c69 7a65 2061 6e64 2072 6566  tabilize and ref
+00000ce0: 696e 6520 6665 6174 7572 6573 2e20 4164  ine features. Ad
+00000cf0: 6472 6573 7320 7265 706f 7274 6564 2062  dress reported b
+00000d00: 7567 732e 2050 7265 7061 7265 2066 6f72  ugs. Prepare for
+00000d10: 206f 6666 6963 6961 6c20 7265 6c65 6173   official releas
+00000d20: 652e 0d0a 2020 2020 2d20 582e 5972 634e  e...    - X.YrcN
+00000d30: 2028 5265 6c65 6173 6520 6361 6e64 6964   (Release candid
+00000d40: 6174 6529 3a20 4669 6e61 6c20 7665 7273  ate): Final vers
+00000d50: 696f 6e20 6265 666f 7265 206f 6666 6963  ion before offic
+00000d60: 6961 6c20 7265 6c65 6173 652e 2041 7373  ial release. Ass
+00000d70: 756d 6573 2061 6c6c 206d 616a 6f72 2066  umes all major f
+00000d80: 6561 7475 7265 7320 6172 6520 636f 6d70  eatures are comp
+00000d90: 6c65 7465 2061 6e64 2073 7461 626c 652e  lete and stable.
+00000da0: 2052 6563 6f6d 6d65 6e64 6564 2066 6f72   Recommended for
+00000db0: 2074 6573 7469 6e67 2069 6e20 6e6f 6e2d   testing in non-
+00000dc0: 6372 6974 6963 616c 2065 6e76 6972 6f6e  critical environ
+00000dd0: 6d65 6e74 732e 0d0a 2020 2020 2d20 582e  ments...    - X.
+00000de0: 5920 2846 696e 616c 2072 656c 6561 7365  Y (Final release
+00000df0: 2f53 7461 626c 652f 5072 6f64 7563 7469  /Stable/Producti
+00000e00: 6f6e 293a 2043 6f6d 706c 6574 6564 2c20  on): Completed, 
+00000e10: 7374 6162 6c65 2076 6572 7369 6f6e 2072  stable version r
+00000e20: 6561 6479 2066 6f72 2075 7365 2069 6e20  eady for use in 
+00000e30: 7072 6f64 7563 7469 6f6e 2e20 4675 6c6c  production. Full
+00000e40: 2072 656c 6561 7365 2066 6f72 2070 7562   release for pub
+00000e50: 6c69 6320 7573 652e 0d0a 0d0a 2d2d 2d0d  lic use.....---.
+00000e60: 0a0d 0a23 2045 7861 6d70 6c65 206f 6620  ...# Example of 
+00000e70: 636f 6e63 6570 7473 2074 6861 7420 7573  concepts that us
+00000e80: 6520 6120 6c69 6272 6172 7920 7769 7468  e a library with
+00000e90: 2061 2073 696e 676c 6574 6f6e 2070 6174   a singleton pat
+00000ea0: 7465 726e 2061 6e64 2063 6f6e 6e65 6374  tern and connect
+00000eb0: 696f 6e20 746f 206d 756c 7469 706c 6520  ion to multiple 
+00000ec0: 656e 6769 6e65 7320 7769 7468 2079 6965  engines with yie
+00000ed0: 6c64 2064 6570 656e 6465 6e63 7920 696e  ld dependency in
+00000ee0: 6a65 6374 696f 6e0d 0a0d 0a54 6865 206c  jection....The l
+00000ef0: 6962 7261 7279 2075 7365 7320 6120 7369  ibrary uses a si
+00000f00: 6e67 6c65 746f 6e20 7061 7474 6572 6e20  ngleton pattern 
+00000f10: 2263 6c61 7373 2053 796e 6343 6f6e 6e45  "class SyncConnE
+00000f20: 6e67 696e 6528 6d65 7461 636c 6173 733d  ngine(metaclass=
+00000f30: 5369 6e67 6c65 746f 6e29 3a22 2c20 7768  Singleton):", wh
+00000f40: 6572 6520 7468 6520 636c 6173 7320 6973  ere the class is
+00000f50: 2061 6c6c 6f77 6564 2074 6f20 6265 2069   allowed to be i
+00000f60: 6e73 7461 6e74 6961 7465 6420 6f6e 6c79  nstantiated only
+00000f70: 206f 6e63 652e 2059 6f75 2063 616e 2063   once. You can c
+00000f80: 7265 6174 6520 616e 6f74 6865 7220 636f  reate another co
+00000f90: 6e6e 6563 7469 6f6e 2074 6f20 616e 6f74  nnection to anot
+00000fa0: 6865 7220 656e 6769 6e65 2062 7574 2079  her engine but y
+00000fb0: 6f75 206d 7573 7420 6372 6561 7465 2061  ou must create a
+00000fc0: 6e20 696e 6865 7269 7465 6420 636c 6173  n inherited clas
+00000fd0: 7320 696e 206f 7264 6572 2074 6f20 6372  s in order to cr
+00000fe0: 6561 7465 2061 206e 6577 2063 6f6e 6669  eate a new confi
+00000ff0: 6775 7261 7469 6f6e 2069 6e73 7461 6e63  guration instanc
+00001000: 652e 0d0a 0d0a 4578 616d 706c 653a 0d0a  e.....Example:..
+00001010: 636c 6173 7320 5379 6e63 436f 6e6e 456e  class SyncConnEn
+00001020: 6769 6e65 5828 5379 6e63 436f 6e6e 456e  gineX(SyncConnEn
+00001030: 6769 6e65 293a 0d0a 2020 2020 6465 6620  gine):..    def 
+00001040: 5f5f 696e 6974 5f5f 2873 656c 662c 2075  __init__(self, u
+00001050: 726c 5f63 6f6e 6e65 6374 696f 6e2c 7365  rl_connection,se
+00001060: 7276 6572 5f73 6574 7469 6e67 7329 3a0d  rver_settings):.
+00001070: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00001080: 2e5f 5f69 6e69 745f 5f28 7572 6c5f 636f  .__init__(url_co
+00001090: 6e6e 6563 7469 6f6e 2c73 6572 7665 725f  nnection,server_
+000010a0: 7365 7474 696e 6773 290d 0a73 796e 635f  settings)..sync_
+000010b0: 7365 7373 696f 6e5f 783d 5379 6e63 436f  session_x=SyncCo
+000010c0: 6e6e 456e 6769 6e65 5828 0d0a 2020 2020  nnEngineX(..    
+000010d0: 7572 6c5f 636f 6e6e 6563 7469 6f6e 3d53  url_connection=S
+000010e0: 796e 6343 6f6e 6e45 6e67 696e 652e 6275  yncConnEngine.bu
+000010f0: 696c 645f 7572 6c5f 636f 6e6e 6563 7469  ild_url_connecti
+00001100: 6f6e 2875 7365 723d 7365 7474 696e 6773  on(user=settings
+00001110: 2e44 425f 5553 4552 5f58 2c70 6173 7377  .DB_USER_X,passw
+00001120: 6f72 643d 7365 7474 696e 6773 2e44 425f  ord=settings.DB_
+00001130: 5041 5353 5f58 2c68 6f73 743d 7365 7474  PASS_X,host=sett
+00001140: 696e 6773 2e44 425f 484f 5354 5f58 2c70  ings.DB_HOST_X,p
+00001150: 6f72 743d 7365 7474 696e 6773 2e44 425f  ort=settings.DB_
+00001160: 504f 5254 5f58 2c64 6174 6162 6173 653d  PORT_X,database=
+00001170: 7365 7474 696e 6773 2e44 425f 4e41 4d45  settings.DB_NAME
+00001180: 5f58 2c73 736c 5f65 6e61 626c 653d 7365  _X,ssl_enable=se
+00001190: 7474 696e 6773 2e44 425f 5353 4c5f 5829  ttings.DB_SSL_X)
+000011a0: 2c0d 0a20 2020 2073 6572 7665 725f 7365  ,..    server_se
+000011b0: 7474 696e 6773 3d53 796e 6343 6f6e 6e45  ttings=SyncConnE
+000011c0: 6e67 696e 652e 7365 7276 6572 5f73 6574  ngine.server_set
+000011d0: 7469 6e67 7328 706f 6f6c 5f73 697a 653d  tings(pool_size=
+000011e0: 352c 6d61 785f 6f76 6572 666c 6f77 3d31  5,max_overflow=1
+000011f0: 2c70 6f6f 6c5f 7265 6379 636c 653d 3130  ,pool_recycle=10
+00001200: 3830 302c 6170 706c 6963 6174 696f 6e5f  800,application_
+00001210: 6e61 6d65 3d66 227b 4170 702e 5365 7474  name=f"{App.Sett
+00001220: 696e 6773 2e4e 414d 457d 202d 2053 796e  ings.NAME} - Syn
+00001230: 6343 6f6e 6e45 6e67 696e 6558 2229 0d0a  cConnEngineX")..
+00001240: 2020 2020 290d 0a0d 0a23 2320 4173 796e      )....## Asyn
+00001250: 6368 726f 6e6f 7573 206d 6f64 650d 0a46  chronous mode..F
+00001260: 6173 7441 5049 0d0a 6060 6070 7974 686f  astAPI..```pytho
+00001270: 6e0d 0a66 726f 6d20 6661 7374 6170 6920  n..from fastapi 
+00001280: 696d 706f 7274 2046 6173 7441 5049 2c20  import FastAPI, 
+00001290: 4465 7065 6e64 732c 2048 5454 5045 7863  Depends, HTTPExc
+000012a0: 6570 7469 6f6e 0d0a 6672 6f6d 206c 6f67  eption..from log
+000012b0: 7963 615f 706f 7374 6772 6573 2069 6d70  yca_postgres imp
+000012c0: 6f72 7420 4173 796e 6343 6f6e 6e45 6e67  ort AsyncConnEng
+000012d0: 696e 652c 2063 6f6d 6d69 745f 726f 6c6c  ine, commit_roll
+000012e0: 6261 636b 5f61 7379 6e63 2c20 6368 6563  back_async, chec
+000012f0: 6b5f 636f 6e6e 6563 7469 6f6e 5f61 7379  k_connection_asy
+00001300: 6e63 0d0a 6672 6f6d 2073 716c 616c 6368  nc..from sqlalch
+00001310: 656d 7920 696d 706f 7274 2074 6578 7420  emy import text 
+00001320: 6173 2074 6578 745f 746f 5f73 716c 0d0a  as text_to_sql..
+00001330: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
+00001340: 6578 742e 6173 796e 6369 6f20 696d 706f  ext.asyncio impo
+00001350: 7274 2041 7379 6e63 5365 7373 696f 6e0d  rt AsyncSession.
+00001360: 0a69 6d70 6f72 7420 6f73 0d0a 0d0a 4442  .import os....DB
+00001370: 5f55 5345 523d 6f73 2e67 6574 656e 7628  _USER=os.getenv(
+00001380: 2744 425f 5553 4552 272c 2770 6f73 7467  'DB_USER','postg
+00001390: 7265 7327 290d 0a44 425f 5041 5353 3d6f  res')..DB_PASS=o
+000013a0: 732e 6765 7465 6e76 2827 4442 5f50 4153  s.getenv('DB_PAS
+000013b0: 5327 2c27 7878 7827 290d 0a44 425f 484f  S','xxx')..DB_HO
+000013c0: 5354 3d6f 732e 6765 7465 6e76 2827 4442  ST=os.getenv('DB
+000013d0: 5f48 4f53 5427 2c27 6c6f 6361 6c68 6f73  _HOST','localhos
+000013e0: 7427 290d 0a44 425f 504f 5254 3d6f 732e  t')..DB_PORT=os.
+000013f0: 6765 7465 6e76 2827 4442 5f50 4f52 5427  getenv('DB_PORT'
+00001400: 2c35 3433 3229 0d0a 4442 5f4e 414d 453d  ,5432)..DB_NAME=
+00001410: 6f73 2e67 6574 656e 7628 2744 425f 4e41  os.getenv('DB_NA
+00001420: 4d45 272c 2774 6573 7427 290d 0a73 736c  ME','test')..ssl
+00001430: 5f65 6e61 626c 655f 6c69 6b65 5f6c 6f63  _enable_like_loc
+00001440: 616c 5f64 6f63 6b65 725f 636f 6e74 6169  al_docker_contai
+00001450: 6e65 723d 4661 6c73 650d 0a0d 0a61 7070  ner=False....app
+00001460: 203d 2046 6173 7441 5049 2829 0d0a 0d0a   = FastAPI()....
+00001470: 636f 6e6e 5f61 7379 6e63 5f73 6573 7369  conn_async_sessi
+00001480: 6f6e 3d41 7379 6e63 436f 6e6e 456e 6769  on=AsyncConnEngi
+00001490: 6e65 280d 0a20 2020 2075 726c 5f63 6f6e  ne(..    url_con
+000014a0: 6e65 6374 696f 6e3d 4173 796e 6343 6f6e  nection=AsyncCon
+000014b0: 6e45 6e67 696e 652e 6275 696c 645f 7572  nEngine.build_ur
+000014c0: 6c5f 636f 6e6e 6563 7469 6f6e 2875 7365  l_connection(use
+000014d0: 723d 4442 5f55 5345 522c 7061 7373 776f  r=DB_USER,passwo
+000014e0: 7264 3d44 425f 5041 5353 2c68 6f73 743d  rd=DB_PASS,host=
+000014f0: 4442 5f48 4f53 542c 706f 7274 3d44 425f  DB_HOST,port=DB_
+00001500: 504f 5254 2c64 6174 6162 6173 653d 4442  PORT,database=DB
+00001510: 5f4e 414d 452c 7373 6c5f 656e 6162 6c65  _NAME,ssl_enable
+00001520: 3d73 736c 5f65 6e61 626c 655f 6c69 6b65  =ssl_enable_like
+00001530: 5f6c 6f63 616c 5f64 6f63 6b65 725f 636f  _local_docker_co
+00001540: 6e74 6169 6e65 7229 2c0d 0a20 2020 2073  ntainer),..    s
+00001550: 6572 7665 725f 7365 7474 696e 6773 3d41  erver_settings=A
+00001560: 7379 6e63 436f 6e6e 456e 6769 6e65 2e73  syncConnEngine.s
+00001570: 6572 7665 725f 7365 7474 696e 6773 2870  erver_settings(p
+00001580: 6f6f 6c5f 7369 7a65 3d35 2c6d 6178 5f6f  ool_size=5,max_o
+00001590: 7665 7266 6c6f 773d 312c 706f 6f6c 5f72  verflow=1,pool_r
+000015a0: 6563 7963 6c65 3d31 3038 3030 2c61 7070  ecycle=10800,app
+000015b0: 6c69 6361 7469 6f6e 5f6e 616d 653d 224d  lication_name="M
+000015c0: 7941 7070 202d 2041 7379 6e63 436f 6e6e  yApp - AsyncConn
+000015d0: 456e 6769 6e65 2229 0d0a 2020 2020 290d  Engine")..    ).
+000015e0: 0a0d 0a27 2727 0d0a 5468 6520 636f 6e6e  ...'''..The conn
+000015f0: 6563 7469 6f6e 2070 6f6f 6c20 2870 6f6f  ection pool (poo
+00001600: 6c5f 7369 7a65 2920 6166 7465 7220 7468  l_size) after th
+00001610: 6520 6669 7273 7420 7175 6572 7920 7769  e first query wi
+00001620: 6c6c 2072 656d 6169 6e20 6f70 656e 2075  ll remain open u
+00001630: 6e74 696c 2074 6865 2061 7070 6c69 6361  ntil the applica
+00001640: 7469 6f6e 2069 7320 7374 6f70 7065 642e  tion is stopped.
+00001650: 0d0a 2727 270d 0a0d 0a40 6170 702e 6765  ..'''....@app.ge
+00001660: 7428 222f 7369 6d75 6c61 7465 645f 7175  t("/simulated_qu
+00001670: 6572 795f 6173 796e 632f 2229 0d0a 6173  ery_async/")..as
+00001680: 796e 6320 6465 6620 7265 6164 5f69 7465  ync def read_ite
+00001690: 6d28 6173 796e 635f 7365 7373 696f 6e3a  m(async_session:
+000016a0: 4173 796e 6353 6573 7369 6f6e 203d 2044  AsyncSession = D
+000016b0: 6570 656e 6473 2863 6f6e 6e5f 6173 796e  epends(conn_asyn
+000016c0: 635f 7365 7373 696f 6e29 293a 0d0a 2020  c_session)):..  
+000016d0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+000016e0: 7374 6174 7573 2c20 6461 7465 5f74 696d  status, date_tim
+000016f0: 655f 6368 6563 6b5f 636f 6e6e 203d 2061  e_check_conn = a
+00001700: 7761 6974 2063 6865 636b 5f63 6f6e 6e65  wait check_conne
+00001710: 6374 696f 6e5f 6173 796e 6328 6173 796e  ction_async(asyn
+00001720: 635f 7365 7373 696f 6e29 0d0a 2020 2020  c_session)..    
+00001730: 2020 2020 6966 2873 7461 7475 7329 3a0d      if(status):.
+00001740: 0a20 2020 2020 2020 2020 2020 2071 7565  .            que
+00001750: 7279 203d 2074 6578 745f 746f 5f73 716c  ry = text_to_sql
+00001760: 2822 5345 4c45 4354 206e 6f77 2829 3b22  ("SELECT now();"
 00001770: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00001780: 6574 7572 6e20 7b22 6461 7465 5f74 696d  eturn {"date_tim
-00001790: 655f 6368 6563 6b5f 636f 6e6e 223a 2064  e_check_conn": d
-000017a0: 6174 655f 7469 6d65 5f63 6865 636b 5f63  ate_time_check_c
-000017b0: 6f6e 6e2c 2022 7369 6d75 6c61 7465 645f  onn, "simulated_
-000017c0: 7175 6572 7922 3a20 7369 6d75 6c61 7465  query": simulate
-000017d0: 645f 7175 6572 797d 0d0a 2020 2020 2020  d_query}..      
-000017e0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000017f0: 2020 2020 2072 6169 7365 2048 5454 5045       raise HTTPE
-00001800: 7863 6570 7469 6f6e 2873 7461 7475 735f  xception(status_
-00001810: 636f 6465 3d34 3034 2c20 6465 7461 696c  code=404, detail
-00001820: 3d22 6173 796e 635f 7365 7373 696f 6e20  ="async_session 
-00001830: 636f 6e6e 6563 7420 6462 2065 7272 6f72  connect db error
-00001840: 2e2e 2e22 290d 0a20 2020 2065 7863 6570  ...")..    excep
-00001850: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00001860: 3a0d 0a20 2020 2020 2020 2072 6169 7365  :..        raise
-00001870: 2048 5454 5045 7863 6570 7469 6f6e 2873   HTTPException(s
-00001880: 7461 7475 735f 636f 6465 3d34 3034 2c20  tatus_code=404, 
-00001890: 6465 7461 696c 3d66 2265 7272 6f72 3a20  detail=f"error: 
-000018a0: 7b65 7d22 290d 0a60 6060 0d0a 576f 726b  {e}")..```..Work
-000018b0: 6572 206f 7220 7363 7269 7074 0d0a 6060  er or script..``
-000018c0: 6070 7974 686f 6e0d 0a66 726f 6d20 6c6f  `python..from lo
-000018d0: 6779 6361 5f70 6f73 7467 7265 7320 696d  gyca_postgres im
-000018e0: 706f 7274 2041 7379 6e63 436f 6e6e 456e  port AsyncConnEn
-000018f0: 6769 6e65 2c20 636f 6d6d 6974 5f72 6f6c  gine, commit_rol
-00001900: 6c62 6163 6b5f 6173 796e 632c 2063 6865  lback_async, che
-00001910: 636b 5f63 6f6e 6e65 6374 696f 6e5f 6173  ck_connection_as
-00001920: 796e 630d 0a66 726f 6d20 7371 6c61 6c63  ync..from sqlalc
-00001930: 6865 6d79 2069 6d70 6f72 7420 7465 7874  hemy import text
-00001940: 2061 7320 7465 7874 5f74 6f5f 7371 6c0d   as text_to_sql.
-00001950: 0a66 726f 6d20 7371 6c61 6c63 6865 6d79  .from sqlalchemy
-00001960: 2e65 7874 2e61 7379 6e63 696f 2069 6d70  .ext.asyncio imp
-00001970: 6f72 7420 4173 796e 6353 6573 7369 6f6e  ort AsyncSession
-00001980: 0d0a 696d 706f 7274 2061 7379 6e63 696f  ..import asyncio
-00001990: 0d0a 696d 706f 7274 206f 730d 0a0d 0a44  ..import os....D
-000019a0: 425f 5553 4552 3d6f 732e 6765 7465 6e76  B_USER=os.getenv
-000019b0: 2827 4442 5f55 5345 5227 2c27 706f 7374  ('DB_USER','post
-000019c0: 6772 6573 2729 0d0a 4442 5f50 4153 533d  gres')..DB_PASS=
-000019d0: 6f73 2e67 6574 656e 7628 2744 425f 5041  os.getenv('DB_PA
-000019e0: 5353 272c 2778 7878 2729 0d0a 4442 5f48  SS','xxx')..DB_H
-000019f0: 4f53 543d 6f73 2e67 6574 656e 7628 2744  OST=os.getenv('D
-00001a00: 425f 484f 5354 272c 276c 6f63 616c 686f  B_HOST','localho
-00001a10: 7374 2729 0d0a 4442 5f50 4f52 543d 6f73  st')..DB_PORT=os
-00001a20: 2e67 6574 656e 7628 2744 425f 504f 5254  .getenv('DB_PORT
-00001a30: 272c 3534 3332 290d 0a44 425f 4e41 4d45  ',5432)..DB_NAME
-00001a40: 3d6f 732e 6765 7465 6e76 2827 4442 5f4e  =os.getenv('DB_N
-00001a50: 414d 4527 2c27 7465 7374 2729 0d0a 7373  AME','test')..ss
-00001a60: 6c5f 656e 6162 6c65 5f6c 696b 655f 6c6f  l_enable_like_lo
-00001a70: 6361 6c5f 646f 636b 6572 5f63 6f6e 7461  cal_docker_conta
-00001a80: 696e 6572 3d46 616c 7365 0d0a 0d0a 636f  iner=False....co
-00001a90: 6e6e 5f61 7379 6e63 5f73 6573 7369 6f6e  nn_async_session
-00001aa0: 3d41 7379 6e63 436f 6e6e 456e 6769 6e65  =AsyncConnEngine
-00001ab0: 280d 0a20 2020 2075 726c 5f63 6f6e 6e65  (..    url_conne
-00001ac0: 6374 696f 6e3d 4173 796e 6343 6f6e 6e45  ction=AsyncConnE
-00001ad0: 6e67 696e 652e 6275 696c 645f 7572 6c5f  ngine.build_url_
-00001ae0: 636f 6e6e 6563 7469 6f6e 2875 7365 723d  connection(user=
-00001af0: 4442 5f55 5345 522c 7061 7373 776f 7264  DB_USER,password
-00001b00: 3d44 425f 5041 5353 2c68 6f73 743d 4442  =DB_PASS,host=DB
-00001b10: 5f48 4f53 542c 706f 7274 3d44 425f 504f  _HOST,port=DB_PO
-00001b20: 5254 2c64 6174 6162 6173 653d 4442 5f4e  RT,database=DB_N
-00001b30: 414d 452c 7373 6c5f 656e 6162 6c65 3d73  AME,ssl_enable=s
-00001b40: 736c 5f65 6e61 626c 655f 6c69 6b65 5f6c  sl_enable_like_l
-00001b50: 6f63 616c 5f64 6f63 6b65 725f 636f 6e74  ocal_docker_cont
-00001b60: 6169 6e65 7229 2c0d 0a20 2020 2073 6572  ainer),..    ser
-00001b70: 7665 725f 7365 7474 696e 6773 3d41 7379  ver_settings=Asy
-00001b80: 6e63 436f 6e6e 456e 6769 6e65 2e73 6572  ncConnEngine.ser
-00001b90: 7665 725f 7365 7474 696e 6773 2870 6f6f  ver_settings(poo
-00001ba0: 6c5f 7369 7a65 3d35 2c6d 6178 5f6f 7665  l_size=5,max_ove
-00001bb0: 7266 6c6f 773d 312c 706f 6f6c 5f72 6563  rflow=1,pool_rec
-00001bc0: 7963 6c65 3d31 3038 3030 2c61 7070 6c69  ycle=10800,appli
-00001bd0: 6361 7469 6f6e 5f6e 616d 653d 224d 7941  cation_name="MyA
-00001be0: 7070 202d 2041 7379 6e63 436f 6e6e 456e  pp - AsyncConnEn
-00001bf0: 6769 6e65 2229 0d0a 2020 2020 2020 2020  gine")..        
-00001c00: 2020 2020 290d 0a0d 0a27 2727 0d0a 5468      )....'''..Th
-00001c10: 6520 636f 6e6e 6563 7469 6f6e 2070 6f6f  e connection poo
-00001c20: 6c20 2870 6f6f 6c5f 7369 7a65 2920 6166  l (pool_size) af
-00001c30: 7465 7220 7468 6520 6669 7273 7420 7175  ter the first qu
-00001c40: 6572 7920 7769 6c6c 2072 656d 6169 6e20  ery will remain 
-00001c50: 6f70 656e 2075 6e74 696c 2074 6865 2061  open until the a
-00001c60: 7070 6c69 6361 7469 6f6e 2069 7320 7374  pplication is st
-00001c70: 6f70 7065 6420 6f72 2074 6865 2065 6e67  opped or the eng
-00001c80: 696e 6520 6973 2074 6572 6d69 6e61 7465  ine is terminate
-00001c90: 643a 2063 6c6f 7365 5f65 6e67 696e 6528  d: close_engine(
-00001ca0: 292e 0d0a 2727 270d 0a0d 0a61 7379 6e63  )...'''....async
-00001cb0: 2064 6566 206d 6574 686f 6473 2861 7379   def methods(asy
-00001cc0: 6e63 5f73 6573 7369 6f6e 3a41 7379 6e63  nc_session:Async
-00001cd0: 5365 7373 696f 6e29 3a0d 0a20 2020 2073  Session):..    s
-00001ce0: 7461 7475 732c 2064 6174 655f 7469 6d65  tatus, date_time
-00001cf0: 5f63 6865 636b 5f63 6f6e 6e20 3d20 6177  _check_conn = aw
-00001d00: 6169 7420 6368 6563 6b5f 636f 6e6e 6563  ait check_connec
-00001d10: 7469 6f6e 5f61 7379 6e63 2861 7379 6e63  tion_async(async
-00001d20: 5f73 6573 7369 6f6e 290d 0a20 2020 2069  _session)..    i
-00001d30: 6628 7374 6174 7573 293a 0d0a 2020 2020  f(status):..    
-00001d40: 2020 2020 7175 6572 7920 3d20 7465 7874      query = text
-00001d50: 5f74 6f5f 7371 6c28 2253 454c 4543 5420  _to_sql("SELECT 
-00001d60: 6e6f 7728 293b 2229 0d0a 2020 2020 2020  now();")..      
-00001d70: 2020 7265 7375 6c74 203d 2061 7761 6974    result = await
-00001d80: 2061 7379 6e63 5f73 6573 7369 6f6e 2e65   async_session.e
-00001d90: 7865 6375 7465 2871 7565 7279 290d 0a20  xecute(query).. 
-00001da0: 2020 2020 2020 2073 696d 756c 6174 6564         simulated
-00001db0: 5f71 7565 7279 203d 2072 6573 756c 742e  _query = result.
-00001dc0: 7363 616c 6172 5f6f 6e65 5f6f 725f 6e6f  scalar_one_or_no
-00001dd0: 6e65 2829 0d0a 2020 2020 2020 2020 6177  ne()..        aw
-00001de0: 6169 7420 636f 6d6d 6974 5f72 6f6c 6c62  ait commit_rollb
-00001df0: 6163 6b5f 6173 796e 6328 6173 796e 635f  ack_async(async_
-00001e00: 7365 7373 696f 6e29 0d0a 2020 2020 2020  session)..      
-00001e10: 2020 7072 696e 7428 6622 6461 7465 5f74    print(f"date_t
-00001e20: 696d 655f 6368 6563 6b5f 636f 6e6e 3d7b  ime_check_conn={
-00001e30: 6461 7465 5f74 696d 655f 6368 6563 6b5f  date_time_check_
-00001e40: 636f 6e6e 7d2c 7369 6d75 6c61 7465 645f  conn},simulated_
-00001e50: 7175 6572 793d 7b73 696d 756c 6174 6564  query={simulated
-00001e60: 5f71 7565 7279 7d22 290d 0a20 2020 2065  _query}")..    e
-00001e70: 6c73 653a 0d0a 2020 2020 2020 2020 7072  lse:..        pr
-00001e80: 696e 7428 2261 7379 6e63 5f73 6573 7369  int("async_sessi
-00001e90: 6f6e 2063 6f6e 6e65 6374 2064 6220 6572  on connect db er
-00001ea0: 726f 722e 2e2e 2229 0d0a 6173 796e 6320  ror...")..async 
-00001eb0: 6465 6620 6d61 696e 2829 3a0d 0a20 2020  def main():..   
-00001ec0: 2061 7379 6e63 2066 6f72 2061 7379 6e63   async for async
-00001ed0: 5f73 6573 7369 6f6e 2069 6e20 636f 6e6e  _session in conn
-00001ee0: 5f61 7379 6e63 5f73 6573 7369 6f6e 2e67  _async_session.g
-00001ef0: 6574 5f61 7379 6e63 5f73 6573 7369 6f6e  et_async_session
-00001f00: 2829 3a0d 0a20 2020 2020 2020 2061 7761  ():..        awa
-00001f10: 6974 206d 6574 686f 6473 2861 7379 6e63  it methods(async
-00001f20: 5f73 6573 7369 6f6e 290d 0a20 2020 2061  _session)..    a
-00001f30: 7761 6974 2063 6f6e 6e5f 6173 796e 635f  wait conn_async_
-00001f40: 7365 7373 696f 6e2e 636c 6f73 655f 656e  session.close_en
-00001f50: 6769 6e65 2829 0d0a 0d0a 6966 205f 5f6e  gine()....if __n
-00001f60: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
-00001f70: 5f5f 223a 0d0a 2020 2020 6173 796e 6369  __":..    asynci
-00001f80: 6f2e 7275 6e28 6d61 696e 2829 290d 0a60  o.run(main())..`
-00001f90: 6060 0d0a 0d0a 2323 2073 796e 6368 726f  ``....## synchro
-00001fa0: 6e6f 7573 206d 6f64 650d 0a46 6173 7441  nous mode..FastA
-00001fb0: 5049 0d0a 6060 6070 7974 686f 6e0d 0a66  PI..```python..f
-00001fc0: 726f 6d20 6661 7374 6170 6920 696d 706f  rom fastapi impo
-00001fd0: 7274 2046 6173 7441 5049 2c20 4465 7065  rt FastAPI, Depe
-00001fe0: 6e64 732c 2048 5454 5045 7863 6570 7469  nds, HTTPExcepti
-00001ff0: 6f6e 0d0a 6672 6f6d 206c 6f67 7963 615f  on..from logyca_
-00002000: 706f 7374 6772 6573 2069 6d70 6f72 7420  postgres import 
-00002010: 5379 6e63 436f 6e6e 456e 6769 6e65 2c20  SyncConnEngine, 
-00002020: 636f 6d6d 6974 5f72 6f6c 6c62 6163 6b5f  commit_rollback_
-00002030: 7379 6e63 2c20 6368 6563 6b5f 636f 6e6e  sync, check_conn
-00002040: 6563 7469 6f6e 5f73 796e 630d 0a66 726f  ection_sync..fro
-00002050: 6d20 7371 6c61 6c63 6865 6d79 2e6f 726d  m sqlalchemy.orm
-00002060: 2e73 6573 7369 6f6e 2069 6d70 6f72 7420  .session import 
-00002070: 5365 7373 696f 6e0d 0a69 6d70 6f72 7420  Session..import 
-00002080: 6f73 0d0a 6672 6f6d 2073 716c 616c 6368  os..from sqlalch
-00002090: 656d 7920 696d 706f 7274 2074 6578 7420  emy import text 
-000020a0: 6173 2074 6578 745f 746f 5f73 716c 0d0a  as text_to_sql..
-000020b0: 0d0a 4442 5f55 5345 523d 6f73 2e67 6574  ..DB_USER=os.get
-000020c0: 656e 7628 2744 425f 5553 4552 272c 2770  env('DB_USER','p
-000020d0: 6f73 7467 7265 7327 290d 0a44 425f 5041  ostgres')..DB_PA
-000020e0: 5353 3d6f 732e 6765 7465 6e76 2827 4442  SS=os.getenv('DB
-000020f0: 5f50 4153 5327 2c27 7878 7827 290d 0a44  _PASS','xxx')..D
-00002100: 425f 484f 5354 3d6f 732e 6765 7465 6e76  B_HOST=os.getenv
-00002110: 2827 4442 5f48 4f53 5427 2c27 6c6f 6361  ('DB_HOST','loca
-00002120: 6c68 6f73 7427 290d 0a44 425f 504f 5254  lhost')..DB_PORT
-00002130: 3d6f 732e 6765 7465 6e76 2827 4442 5f50  =os.getenv('DB_P
-00002140: 4f52 5427 2c35 3433 3229 0d0a 4442 5f4e  ORT',5432)..DB_N
-00002150: 414d 453d 6f73 2e67 6574 656e 7628 2744  AME=os.getenv('D
-00002160: 425f 4e41 4d45 272c 2774 6573 7427 290d  B_NAME','test').
-00002170: 0a73 736c 5f65 6e61 626c 655f 6c69 6b65  .ssl_enable_like
-00002180: 5f6c 6f63 616c 5f64 6f63 6b65 725f 636f  _local_docker_co
-00002190: 6e74 6169 6e65 723d 4661 6c73 650d 0a0d  ntainer=False...
-000021a0: 0a61 7070 203d 2046 6173 7441 5049 2829  .app = FastAPI()
-000021b0: 0d0a 0d0a 636f 6e6e 5f73 796e 635f 7365  ....conn_sync_se
-000021c0: 7373 696f 6e3d 5379 6e63 436f 6e6e 456e  ssion=SyncConnEn
-000021d0: 6769 6e65 280d 0a20 2020 2075 726c 5f63  gine(..    url_c
-000021e0: 6f6e 6e65 6374 696f 6e3d 5379 6e63 436f  onnection=SyncCo
-000021f0: 6e6e 456e 6769 6e65 2e62 7569 6c64 5f75  nnEngine.build_u
-00002200: 726c 5f63 6f6e 6e65 6374 696f 6e28 7573  rl_connection(us
-00002210: 6572 3d44 425f 5553 4552 2c70 6173 7377  er=DB_USER,passw
-00002220: 6f72 643d 4442 5f50 4153 532c 686f 7374  ord=DB_PASS,host
-00002230: 3d44 425f 484f 5354 2c70 6f72 743d 4442  =DB_HOST,port=DB
-00002240: 5f50 4f52 542c 6461 7461 6261 7365 3d44  _PORT,database=D
-00002250: 425f 4e41 4d45 2c73 736c 5f65 6e61 626c  B_NAME,ssl_enabl
-00002260: 653d 7373 6c5f 656e 6162 6c65 5f6c 696b  e=ssl_enable_lik
-00002270: 655f 6c6f 6361 6c5f 646f 636b 6572 5f63  e_local_docker_c
-00002280: 6f6e 7461 696e 6572 292c 0d0a 2020 2020  ontainer),..    
-00002290: 7365 7276 6572 5f73 6574 7469 6e67 733d  server_settings=
-000022a0: 5379 6e63 436f 6e6e 456e 6769 6e65 2e73  SyncConnEngine.s
-000022b0: 6572 7665 725f 7365 7474 696e 6773 2870  erver_settings(p
-000022c0: 6f6f 6c5f 7369 7a65 3d35 2c6d 6178 5f6f  ool_size=5,max_o
-000022d0: 7665 7266 6c6f 773d 312c 706f 6f6c 5f72  verflow=1,pool_r
-000022e0: 6563 7963 6c65 3d31 3038 3030 2c61 7070  ecycle=10800,app
-000022f0: 6c69 6361 7469 6f6e 5f6e 616d 653d 224d  lication_name="M
-00002300: 7941 7070 202d 2041 7379 6e63 436f 6e6e  yApp - AsyncConn
-00002310: 456e 6769 6e65 2229 0d0a 2020 2020 290d  Engine")..    ).
-00002320: 0a0d 0a27 2727 0d0a 5468 6520 636f 6e6e  ...'''..The conn
-00002330: 6563 7469 6f6e 2070 6f6f 6c20 2870 6f6f  ection pool (poo
-00002340: 6c5f 7369 7a65 2920 6166 7465 7220 7468  l_size) after th
-00002350: 6520 6669 7273 7420 7175 6572 7920 7769  e first query wi
-00002360: 6c6c 2072 656d 6169 6e20 6f70 656e 2075  ll remain open u
-00002370: 6e74 696c 2074 6865 2061 7070 6c69 6361  ntil the applica
-00002380: 7469 6f6e 2069 7320 7374 6f70 7065 642e  tion is stopped.
-00002390: 0d0a 2727 270d 0a0d 0a40 6170 702e 6765  ..'''....@app.ge
-000023a0: 7428 222f 7369 6d75 6c61 7465 645f 7175  t("/simulated_qu
-000023b0: 6572 795f 7379 6e63 2f22 290d 0a64 6566  ery_sync/")..def
-000023c0: 2072 6561 645f 6974 656d 2873 796e 635f   read_item(sync_
-000023d0: 7365 7373 696f 6e3a 5365 7373 696f 6e20  session:Session 
-000023e0: 3d20 4465 7065 6e64 7328 636f 6e6e 5f73  = Depends(conn_s
-000023f0: 796e 635f 7365 7373 696f 6e29 293a 0d0a  ync_session)):..
-00002400: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00002410: 2020 7374 6174 7573 2c20 6461 7465 5f74    status, date_t
-00002420: 696d 655f 6368 6563 6b5f 636f 6e6e 203d  ime_check_conn =
-00002430: 2063 6865 636b 5f63 6f6e 6e65 6374 696f   check_connectio
-00002440: 6e5f 7379 6e63 2873 796e 635f 7365 7373  n_sync(sync_sess
-00002450: 696f 6e29 0d0a 2020 2020 2020 2020 6966  ion)..        if
-00002460: 2873 7461 7475 7329 3a0d 0a20 2020 2020  (status):..     
-00002470: 2020 2020 2020 2071 7565 7279 203d 2074         query = t
-00002480: 6578 745f 746f 5f73 716c 2822 5345 4c45  ext_to_sql("SELE
-00002490: 4354 206e 6f77 2829 3b22 290d 0a20 2020  CT now();")..   
-000024a0: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-000024b0: 3d20 7379 6e63 5f73 6573 7369 6f6e 2e65  = sync_session.e
-000024c0: 7865 6375 7465 2871 7565 7279 290d 0a20  xecute(query).. 
-000024d0: 2020 2020 2020 2020 2020 2073 696d 756c             simul
-000024e0: 6174 6564 5f71 7565 7279 203d 2072 6573  ated_query = res
-000024f0: 756c 742e 6665 7463 686f 6e65 2829 5b30  ult.fetchone()[0
-00002500: 5d0d 0a20 2020 2020 2020 2020 2020 2063  ]..            c
-00002510: 6f6d 6d69 745f 726f 6c6c 6261 636b 5f73  ommit_rollback_s
-00002520: 796e 6328 7379 6e63 5f73 6573 7369 6f6e  ync(sync_session
-00002530: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00002540: 6574 7572 6e20 7b22 6461 7465 5f74 696d  eturn {"date_tim
-00002550: 655f 6368 6563 6b5f 636f 6e6e 223a 2064  e_check_conn": d
-00002560: 6174 655f 7469 6d65 5f63 6865 636b 5f63  ate_time_check_c
-00002570: 6f6e 6e2c 2022 7369 6d75 6c61 7465 645f  onn, "simulated_
-00002580: 7175 6572 7922 3a20 7369 6d75 6c61 7465  query": simulate
-00002590: 645f 7175 6572 797d 0d0a 2020 2020 2020  d_query}..      
-000025a0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000025b0: 2020 2020 2072 6169 7365 2048 5454 5045       raise HTTPE
-000025c0: 7863 6570 7469 6f6e 2873 7461 7475 735f  xception(status_
-000025d0: 636f 6465 3d34 3034 2c20 6465 7461 696c  code=404, detail
-000025e0: 3d22 6173 796e 635f 7365 7373 696f 6e20  ="async_session 
-000025f0: 636f 6e6e 6563 7420 6462 2065 7272 6f72  connect db error
-00002600: 2e2e 2e22 290d 0a20 2020 2065 7863 6570  ...")..    excep
-00002610: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00002620: 3a0d 0a20 2020 2020 2020 2072 6169 7365  :..        raise
-00002630: 2048 5454 5045 7863 6570 7469 6f6e 2873   HTTPException(s
-00002640: 7461 7475 735f 636f 6465 3d34 3034 2c20  tatus_code=404, 
-00002650: 6465 7461 696c 3d66 2265 7272 6f72 3a20  detail=f"error: 
-00002660: 7b65 7d22 290d 0a60 6060 0d0a 576f 726b  {e}")..```..Work
-00002670: 6572 206f 7220 7363 7269 7074 0d0a 6060  er or script..``
-00002680: 6070 7974 686f 6e0d 0a66 726f 6d20 6c6f  `python..from lo
-00002690: 6779 6361 5f70 6f73 7467 7265 7320 696d  gyca_postgres im
-000026a0: 706f 7274 2053 796e 6343 6f6e 6e45 6e67  port SyncConnEng
-000026b0: 696e 652c 2063 6f6d 6d69 745f 726f 6c6c  ine, commit_roll
-000026c0: 6261 636b 5f73 796e 632c 2063 6865 636b  back_sync, check
-000026d0: 5f63 6f6e 6e65 6374 696f 6e5f 7379 6e63  _connection_sync
-000026e0: 0d0a 6672 6f6d 2073 716c 616c 6368 656d  ..from sqlalchem
-000026f0: 7920 696d 706f 7274 2074 6578 7420 6173  y import text as
-00002700: 2074 6578 745f 746f 5f73 716c 0d0a 6672   text_to_sql..fr
-00002710: 6f6d 2073 716c 616c 6368 656d 792e 6f72  om sqlalchemy.or
-00002720: 6d2e 7365 7373 696f 6e20 696d 706f 7274  m.session import
-00002730: 2053 6573 7369 6f6e 0d0a 696d 706f 7274   Session..import
-00002740: 206f 730d 0a0d 0a44 425f 5553 4552 3d6f   os....DB_USER=o
-00002750: 732e 6765 7465 6e76 2827 4442 5f55 5345  s.getenv('DB_USE
-00002760: 5227 2c27 706f 7374 6772 6573 2729 0d0a  R','postgres')..
-00002770: 4442 5f50 4153 533d 6f73 2e67 6574 656e  DB_PASS=os.geten
-00002780: 7628 2744 425f 5041 5353 272c 272a 2a2a  v('DB_PASS','***
-00002790: 2729 0d0a 4442 5f48 4f53 543d 6f73 2e67  ')..DB_HOST=os.g
-000027a0: 6574 656e 7628 2744 425f 484f 5354 272c  etenv('DB_HOST',
-000027b0: 276c 6f63 616c 686f 7374 2729 0d0a 4442  'localhost')..DB
-000027c0: 5f50 4f52 543d 6f73 2e67 6574 656e 7628  _PORT=os.getenv(
-000027d0: 2744 425f 504f 5254 272c 3534 3332 290d  'DB_PORT',5432).
-000027e0: 0a44 425f 4e41 4d45 3d6f 732e 6765 7465  .DB_NAME=os.gete
-000027f0: 6e76 2827 4442 5f4e 414d 4527 2c27 7465  nv('DB_NAME','te
-00002800: 7374 2729 0d0a 7373 6c5f 656e 6162 6c65  st')..ssl_enable
-00002810: 5f6c 696b 655f 6c6f 6361 6c5f 646f 636b  _like_local_dock
-00002820: 6572 5f63 6f6e 7461 696e 6572 3d46 616c  er_container=Fal
-00002830: 7365 0d0a 0d0a 636f 6e6e 5f73 796e 635f  se....conn_sync_
-00002840: 7365 7373 696f 6e3d 5379 6e63 436f 6e6e  session=SyncConn
-00002850: 456e 6769 6e65 280d 0a20 2020 2075 726c  Engine(..    url
-00002860: 5f63 6f6e 6e65 6374 696f 6e3d 5379 6e63  _connection=Sync
-00002870: 436f 6e6e 456e 6769 6e65 2e62 7569 6c64  ConnEngine.build
-00002880: 5f75 726c 5f63 6f6e 6e65 6374 696f 6e28  _url_connection(
-00002890: 7573 6572 3d44 425f 5553 4552 2c70 6173  user=DB_USER,pas
-000028a0: 7377 6f72 643d 4442 5f50 4153 532c 686f  sword=DB_PASS,ho
-000028b0: 7374 3d44 425f 484f 5354 2c70 6f72 743d  st=DB_HOST,port=
-000028c0: 4442 5f50 4f52 542c 6461 7461 6261 7365  DB_PORT,database
-000028d0: 3d44 425f 4e41 4d45 2c73 736c 5f65 6e61  =DB_NAME,ssl_ena
-000028e0: 626c 653d 7373 6c5f 656e 6162 6c65 5f6c  ble=ssl_enable_l
-000028f0: 696b 655f 6c6f 6361 6c5f 646f 636b 6572  ike_local_docker
-00002900: 5f63 6f6e 7461 696e 6572 292c 0d0a 2020  _container),..  
-00002910: 2020 7365 7276 6572 5f73 6574 7469 6e67    server_setting
-00002920: 733d 5379 6e63 436f 6e6e 456e 6769 6e65  s=SyncConnEngine
-00002930: 2e73 6572 7665 725f 7365 7474 696e 6773  .server_settings
-00002940: 2870 6f6f 6c5f 7369 7a65 3d35 2c6d 6178  (pool_size=5,max
-00002950: 5f6f 7665 7266 6c6f 773d 312c 706f 6f6c  _overflow=1,pool
-00002960: 5f72 6563 7963 6c65 3d31 3038 3030 2c61  _recycle=10800,a
-00002970: 7070 6c69 6361 7469 6f6e 5f6e 616d 653d  pplication_name=
-00002980: 224d 7941 7070 202d 2053 796e 6343 6f6e  "MyApp - SyncCon
-00002990: 6e45 6e67 696e 6522 290d 0a20 2020 2020  nEngine")..     
-000029a0: 2020 2020 2020 2029 0d0a 0d0a 2727 270d         )....'''.
-000029b0: 0a54 6865 2063 6f6e 6e65 6374 696f 6e20  .The connection 
-000029c0: 706f 6f6c 2028 706f 6f6c 5f73 697a 6529  pool (pool_size)
-000029d0: 2061 6674 6572 2074 6865 2066 6972 7374   after the first
-000029e0: 2071 7565 7279 2077 696c 6c20 7265 6d61   query will rema
-000029f0: 696e 206f 7065 6e20 756e 7469 6c20 7468  in open until th
-00002a00: 6520 6170 706c 6963 6174 696f 6e20 6973  e application is
-00002a10: 2073 746f 7070 6564 206f 7220 7468 6520   stopped or the 
-00002a20: 656e 6769 6e65 2069 7320 7465 726d 696e  engine is termin
-00002a30: 6174 6564 3a20 636c 6f73 655f 656e 6769  ated: close_engi
-00002a40: 6e65 2829 2e0d 0a27 2727 0d0a 0d0a 6465  ne()...'''....de
-00002a50: 6620 6d65 7468 6f64 7328 7379 6e63 5f73  f methods(sync_s
-00002a60: 6573 7369 6f6e 3a20 5365 7373 696f 6e29  ession: Session)
-00002a70: 3a0d 0a20 2020 2073 7461 7475 732c 2064  :..    status, d
-00002a80: 6174 655f 7469 6d65 5f63 6865 636b 5f63  ate_time_check_c
-00002a90: 6f6e 6e20 3d20 6368 6563 6b5f 636f 6e6e  onn = check_conn
-00002aa0: 6563 7469 6f6e 5f73 796e 6328 7379 6e63  ection_sync(sync
-00002ab0: 5f73 6573 7369 6f6e 290d 0a20 2020 2069  _session)..    i
-00002ac0: 6628 7374 6174 7573 293a 0d0a 2020 2020  f(status):..    
-00002ad0: 2020 2020 7175 6572 7920 3d20 7465 7874      query = text
-00002ae0: 5f74 6f5f 7371 6c28 2253 454c 4543 5420  _to_sql("SELECT 
-00002af0: 6e6f 7728 293b 2229 0d0a 2020 2020 2020  now();")..      
-00002b00: 2020 7265 7375 6c74 203d 2073 796e 635f    result = sync_
-00002b10: 7365 7373 696f 6e2e 6578 6563 7574 6528  session.execute(
-00002b20: 7175 6572 7929 0d0a 2020 2020 2020 2020  query)..        
-00002b30: 7369 6d75 6c61 7465 645f 7175 6572 7920  simulated_query 
-00002b40: 3d20 7265 7375 6c74 2e66 6574 6368 6f6e  = result.fetchon
-00002b50: 6528 295b 305d 0d0a 2020 2020 2020 2020  e()[0]..        
-00002b60: 636f 6d6d 6974 5f72 6f6c 6c62 6163 6b5f  commit_rollback_
-00002b70: 7379 6e63 2873 796e 635f 7365 7373 696f  sync(sync_sessio
-00002b80: 6e29 0d0a 2020 2020 2020 2020 7072 696e  n)..        prin
-00002b90: 7428 6622 6461 7465 5f74 696d 655f 6368  t(f"date_time_ch
-00002ba0: 6563 6b5f 636f 6e6e 3d7b 6461 7465 5f74  eck_conn={date_t
-00002bb0: 696d 655f 6368 6563 6b5f 636f 6e6e 7d2c  ime_check_conn},
-00002bc0: 7369 6d75 6c61 7465 645f 7175 6572 793d  simulated_query=
-00002bd0: 7b73 696d 756c 6174 6564 5f71 7565 7279  {simulated_query
-00002be0: 7d22 290d 0a20 2020 2065 6c73 653a 0d0a  }")..    else:..
-00002bf0: 2020 2020 2020 2020 7072 696e 7428 2273          print("s
-00002c00: 796e 635f 7365 7373 696f 6e20 636f 6e6e  ync_session conn
-00002c10: 6563 7420 6462 2065 7272 6f72 2e2e 2e22  ect db error..."
-00002c20: 290d 0a64 6566 206d 6169 6e28 293a 0d0a  )..def main():..
-00002c30: 2020 2020 666f 7220 7379 6e63 5f73 6573      for sync_ses
-00002c40: 7369 6f6e 2069 6e20 636f 6e6e 5f73 796e  sion in conn_syn
-00002c50: 635f 7365 7373 696f 6e2e 6765 745f 7379  c_session.get_sy
-00002c60: 6e63 5f73 6573 7369 6f6e 2829 3a0d 0a20  nc_session():.. 
-00002c70: 2020 2020 2020 206d 6574 686f 6473 2873         methods(s
-00002c80: 796e 635f 7365 7373 696f 6e29 0d0a 2020  ync_session)..  
-00002c90: 2020 636f 6e6e 5f73 796e 635f 7365 7373    conn_sync_sess
-00002ca0: 696f 6e2e 636c 6f73 655f 656e 6769 6e65  ion.close_engine
-00002cb0: 2829 2020 2020 2020 2020 2020 2020 0d0a  ()            ..
-00002cc0: 0d0a 0d0a 6966 205f 5f6e 616d 655f 5f20  ....if __name__ 
-00002cd0: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0d0a  == "__main__":..
-00002ce0: 2020 2020 6d61 696e 2829 0d0a 6060 600d      main()..```.
-00002cf0: 0a0d 0a2d 2d2d 0d0a 0d0a 2320 4368 616e  ...---....# Chan
-00002d00: 6765 6c6f 670d 0a0d 0a41 6c6c 206e 6f74  gelog....All not
-00002d10: 6162 6c65 2063 6861 6e67 6573 2074 6f20  able changes to 
-00002d20: 7468 6973 2070 726f 6a65 6374 2077 696c  this project wil
-00002d30: 6c20 6265 2064 6f63 756d 656e 7465 6420  l be documented 
-00002d40: 696e 2074 6869 7320 6669 6c65 2e0d 0a0d  in this file....
-00002d50: 0a54 6865 2066 6f72 6d61 7420 6973 2062  .The format is b
-00002d60: 6173 6564 206f 6e20 5b4b 6565 7020 6120  ased on [Keep a 
-00002d70: 4368 616e 6765 6c6f 675d 2868 7474 7073  Changelog](https
-00002d80: 3a2f 2f6b 6565 7061 6368 616e 6765 6c6f  ://keepachangelo
-00002d90: 672e 636f 6d2f 656e 2f31 2e30 2e30 2f29  g.com/en/1.0.0/)
-00002da0: 2c0d 0a61 6e64 2074 6869 7320 7072 6f6a  ,..and this proj
-00002db0: 6563 7420 6164 6865 7265 7320 746f 205b  ect adheres to [
-00002dc0: 5365 6d61 6e74 6963 2056 6572 7369 6f6e  Semantic Version
-00002dd0: 696e 675d 2868 7474 7073 3a2f 2f73 656d  ing](https://sem
-00002de0: 7665 722e 6f72 672f 7370 6563 2f76 322e  ver.org/spec/v2.
-00002df0: 302e 302e 6874 6d6c 292e 0d0a 0d0a 2323  0.0.html).....##
-00002e00: 2054 7970 6573 206f 6620 6368 616e 6765   Types of change
-00002e10: 730d 0a0d 0a2d 2041 6464 6564 2066 6f72  s....- Added for
-00002e20: 206e 6577 2066 6561 7475 7265 732e 0d0a   new features...
-00002e30: 2d20 4368 616e 6765 6420 666f 7220 6368  - Changed for ch
-00002e40: 616e 6765 7320 696e 2065 7869 7374 696e  anges in existin
-00002e50: 6720 6675 6e63 7469 6f6e 616c 6974 792e  g functionality.
-00002e60: 0d0a 2d20 4465 7072 6563 6174 6564 2066  ..- Deprecated f
-00002e70: 6f72 2073 6f6f 6e2d 746f 2d62 6520 7265  or soon-to-be re
-00002e80: 6d6f 7665 6420 6665 6174 7572 6573 2e0d  moved features..
-00002e90: 0a2d 2052 656d 6f76 6564 2066 6f72 206e  .- Removed for n
-00002ea0: 6f77 2072 656d 6f76 6564 2066 6561 7475  ow removed featu
-00002eb0: 7265 732e 0d0a 2d20 4669 7865 6420 666f  res...- Fixed fo
-00002ec0: 7220 616e 7920 6275 6720 6669 7865 732e  r any bug fixes.
-00002ed0: 0d0a 2d20 5365 6375 7269 7479 2069 6e20  ..- Security in 
-00002ee0: 6361 7365 206f 6620 7675 6c6e 6572 6162  case of vulnerab
-00002ef0: 696c 6974 6965 732e 0d0a 0d0a 2323 205b  ilities.....## [
-00002f00: 302e 302e 3172 6331 5d20 2d20 3230 3234  0.0.1rc1] - 2024
-00002f10: 2d30 342d 3232 0d0a 2323 2320 4164 6465  -04-22..### Adde
-00002f20: 640d 0a2d 2046 6972 7374 2074 6573 7473  d..- First tests
-00002f30: 2075 7369 6e67 2070 7970 692e 6f72 6720   using pypi.org 
-00002f40: 696e 2064 6576 656c 6f70 2065 6e76 6972  in develop envir
-00002f50: 6f6e 6d65 6e74 2e0d 0a2d 204e 6577 2066  onment...- New f
-00002f60: 756e 6374 696f 6e61 6c69 7479 206f 6620  unctionality of 
-00002f70: 6173 796e 6368 726f 6e6f 7573 2061 6e64  asynchronous and
-00002f80: 2073 796e 6368 726f 6e6f 7573 2063 6f6e   synchronous con
-00002f90: 6e65 6374 696f 6e73 2074 6f20 706f 7374  nections to post
-00002fa0: 6772 6573 716c 2064 6174 6162 6173 6573  gresql databases
-00002fb0: 2e0d 0a2d 2046 756e 6374 696f 6e61 6c69  ...- Functionali
-00002fc0: 7469 6573 2063 616e 2062 6520 7573 6564  ties can be used
-00002fd0: 2069 6e20 6661 7374 6170 6920 6f72 2077   in fastapi or w
-00002fe0: 6f72 6b65 7273 206c 696b 6520 417a 7572  orkers like Azur
-00002ff0: 6520 4675 6e63 7469 6f6e 732e 0d0a 2d20  e Functions...- 
-00003000: 4578 616d 706c 6573 206f 6620 7573 6520  Examples of use 
-00003010: 6172 6520 6164 6465 6420 746f 2074 6865  are added to the
-00003020: 2064 6f63 756d 656e 7461 7469 6f6e 206f   documentation o
-00003030: 6620 7468 6520 6675 6e63 7469 6f6e 7320  f the functions 
-00003040: 696e 2064 6f63 7374 7269 6e67 0d0a 2d20  in docstring..- 
-00003050: 496e 2074 6865 2073 616d 706c 6573 2066  In the samples f
-00003060: 6f6c 6465 7220 6f66 2074 6869 7320 6c69  older of this li
-00003070: 6272 6172 792c 2074 6865 7265 2061 7265  brary, there are
-00003080: 2063 6f6d 706c 6574 6520 776f 726b 696e   complete workin
-00003090: 6720 6578 616d 706c 6573 206f 6620 7573  g examples of us
-000030a0: 696e 6720 7468 6520 636f 6465 2e0d 0a0d  ing the code....
-000030b0: 0a23 2320 5b30 2e31 2e30 5d20 2d20 3230  .## [0.1.0] - 20
-000030c0: 3234 2d30 352d 3231 0d0a 2323 2320 4164  24-05-21..### Ad
-000030d0: 6465 640d 0a2d 2043 6f6d 706c 6574 696f  ded..- Completio
-000030e0: 6e20 6f66 2074 6573 7469 6e67 2061 6e64  n of testing and
-000030f0: 206c 6175 6e63 6820 696e 746f 2070 726f   launch into pro
-00003100: 6475 6374 696f 6e2e 0d0a                 duction...
+00001780: 6573 756c 7420 3d20 6177 6169 7420 6173  esult = await as
+00001790: 796e 635f 7365 7373 696f 6e2e 6578 6563  ync_session.exec
+000017a0: 7574 6528 7175 6572 7929 0d0a 2020 2020  ute(query)..    
+000017b0: 2020 2020 2020 2020 7369 6d75 6c61 7465          simulate
+000017c0: 645f 7175 6572 7920 3d20 7265 7375 6c74  d_query = result
+000017d0: 2e73 6361 6c61 725f 6f6e 655f 6f72 5f6e  .scalar_one_or_n
+000017e0: 6f6e 6528 290d 0a20 2020 2020 2020 2020  one()..         
+000017f0: 2020 2061 7761 6974 2063 6f6d 6d69 745f     await commit_
+00001800: 726f 6c6c 6261 636b 5f61 7379 6e63 2861  rollback_async(a
+00001810: 7379 6e63 5f73 6573 7369 6f6e 290d 0a20  sync_session).. 
+00001820: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001830: 6e20 7b22 6461 7465 5f74 696d 655f 6368  n {"date_time_ch
+00001840: 6563 6b5f 636f 6e6e 223a 2064 6174 655f  eck_conn": date_
+00001850: 7469 6d65 5f63 6865 636b 5f63 6f6e 6e2c  time_check_conn,
+00001860: 2022 7369 6d75 6c61 7465 645f 7175 6572   "simulated_quer
+00001870: 7922 3a20 7369 6d75 6c61 7465 645f 7175  y": simulated_qu
+00001880: 6572 797d 0d0a 2020 2020 2020 2020 656c  ery}..        el
+00001890: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+000018a0: 2072 6169 7365 2048 5454 5045 7863 6570   raise HTTPExcep
+000018b0: 7469 6f6e 2873 7461 7475 735f 636f 6465  tion(status_code
+000018c0: 3d34 3034 2c20 6465 7461 696c 3d22 6173  =404, detail="as
+000018d0: 796e 635f 7365 7373 696f 6e20 636f 6e6e  ync_session conn
+000018e0: 6563 7420 6462 2065 7272 6f72 2e2e 2e22  ect db error..."
+000018f0: 290d 0a20 2020 2065 7863 6570 7420 4578  )..    except Ex
+00001900: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
+00001910: 2020 2020 2020 2072 6169 7365 2048 5454         raise HTT
+00001920: 5045 7863 6570 7469 6f6e 2873 7461 7475  PException(statu
+00001930: 735f 636f 6465 3d34 3034 2c20 6465 7461  s_code=404, deta
+00001940: 696c 3d66 2265 7272 6f72 3a20 7b65 7d22  il=f"error: {e}"
+00001950: 290d 0a60 6060 0d0a 576f 726b 6572 206f  )..```..Worker o
+00001960: 7220 7363 7269 7074 0d0a 6060 6070 7974  r script..```pyt
+00001970: 686f 6e0d 0a66 726f 6d20 6c6f 6779 6361  hon..from logyca
+00001980: 5f70 6f73 7467 7265 7320 696d 706f 7274  _postgres import
+00001990: 2041 7379 6e63 436f 6e6e 456e 6769 6e65   AsyncConnEngine
+000019a0: 2c20 636f 6d6d 6974 5f72 6f6c 6c62 6163  , commit_rollbac
+000019b0: 6b5f 6173 796e 632c 2063 6865 636b 5f63  k_async, check_c
+000019c0: 6f6e 6e65 6374 696f 6e5f 6173 796e 630d  onnection_async.
+000019d0: 0a66 726f 6d20 7371 6c61 6c63 6865 6d79  .from sqlalchemy
+000019e0: 2069 6d70 6f72 7420 7465 7874 2061 7320   import text as 
+000019f0: 7465 7874 5f74 6f5f 7371 6c0d 0a66 726f  text_to_sql..fro
+00001a00: 6d20 7371 6c61 6c63 6865 6d79 2e65 7874  m sqlalchemy.ext
+00001a10: 2e61 7379 6e63 696f 2069 6d70 6f72 7420  .asyncio import 
+00001a20: 4173 796e 6353 6573 7369 6f6e 0d0a 696d  AsyncSession..im
+00001a30: 706f 7274 2061 7379 6e63 696f 0d0a 696d  port asyncio..im
+00001a40: 706f 7274 206f 730d 0a0d 0a44 425f 5553  port os....DB_US
+00001a50: 4552 3d6f 732e 6765 7465 6e76 2827 4442  ER=os.getenv('DB
+00001a60: 5f55 5345 5227 2c27 706f 7374 6772 6573  _USER','postgres
+00001a70: 2729 0d0a 4442 5f50 4153 533d 6f73 2e67  ')..DB_PASS=os.g
+00001a80: 6574 656e 7628 2744 425f 5041 5353 272c  etenv('DB_PASS',
+00001a90: 2778 7878 2729 0d0a 4442 5f48 4f53 543d  'xxx')..DB_HOST=
+00001aa0: 6f73 2e67 6574 656e 7628 2744 425f 484f  os.getenv('DB_HO
+00001ab0: 5354 272c 276c 6f63 616c 686f 7374 2729  ST','localhost')
+00001ac0: 0d0a 4442 5f50 4f52 543d 6f73 2e67 6574  ..DB_PORT=os.get
+00001ad0: 656e 7628 2744 425f 504f 5254 272c 3534  env('DB_PORT',54
+00001ae0: 3332 290d 0a44 425f 4e41 4d45 3d6f 732e  32)..DB_NAME=os.
+00001af0: 6765 7465 6e76 2827 4442 5f4e 414d 4527  getenv('DB_NAME'
+00001b00: 2c27 7465 7374 2729 0d0a 7373 6c5f 656e  ,'test')..ssl_en
+00001b10: 6162 6c65 5f6c 696b 655f 6c6f 6361 6c5f  able_like_local_
+00001b20: 646f 636b 6572 5f63 6f6e 7461 696e 6572  docker_container
+00001b30: 3d46 616c 7365 0d0a 0d0a 636f 6e6e 5f61  =False....conn_a
+00001b40: 7379 6e63 5f73 6573 7369 6f6e 3d41 7379  sync_session=Asy
+00001b50: 6e63 436f 6e6e 456e 6769 6e65 280d 0a20  ncConnEngine(.. 
+00001b60: 2020 2075 726c 5f63 6f6e 6e65 6374 696f     url_connectio
+00001b70: 6e3d 4173 796e 6343 6f6e 6e45 6e67 696e  n=AsyncConnEngin
+00001b80: 652e 6275 696c 645f 7572 6c5f 636f 6e6e  e.build_url_conn
+00001b90: 6563 7469 6f6e 2875 7365 723d 4442 5f55  ection(user=DB_U
+00001ba0: 5345 522c 7061 7373 776f 7264 3d44 425f  SER,password=DB_
+00001bb0: 5041 5353 2c68 6f73 743d 4442 5f48 4f53  PASS,host=DB_HOS
+00001bc0: 542c 706f 7274 3d44 425f 504f 5254 2c64  T,port=DB_PORT,d
+00001bd0: 6174 6162 6173 653d 4442 5f4e 414d 452c  atabase=DB_NAME,
+00001be0: 7373 6c5f 656e 6162 6c65 3d73 736c 5f65  ssl_enable=ssl_e
+00001bf0: 6e61 626c 655f 6c69 6b65 5f6c 6f63 616c  nable_like_local
+00001c00: 5f64 6f63 6b65 725f 636f 6e74 6169 6e65  _docker_containe
+00001c10: 7229 2c0d 0a20 2020 2073 6572 7665 725f  r),..    server_
+00001c20: 7365 7474 696e 6773 3d41 7379 6e63 436f  settings=AsyncCo
+00001c30: 6e6e 456e 6769 6e65 2e73 6572 7665 725f  nnEngine.server_
+00001c40: 7365 7474 696e 6773 2870 6f6f 6c5f 7369  settings(pool_si
+00001c50: 7a65 3d35 2c6d 6178 5f6f 7665 7266 6c6f  ze=5,max_overflo
+00001c60: 773d 312c 706f 6f6c 5f72 6563 7963 6c65  w=1,pool_recycle
+00001c70: 3d31 3038 3030 2c61 7070 6c69 6361 7469  =10800,applicati
+00001c80: 6f6e 5f6e 616d 653d 224d 7941 7070 202d  on_name="MyApp -
+00001c90: 2041 7379 6e63 436f 6e6e 456e 6769 6e65   AsyncConnEngine
+00001ca0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00001cb0: 290d 0a0d 0a27 2727 0d0a 5468 6520 636f  )....'''..The co
+00001cc0: 6e6e 6563 7469 6f6e 2070 6f6f 6c20 2870  nnection pool (p
+00001cd0: 6f6f 6c5f 7369 7a65 2920 6166 7465 7220  ool_size) after 
+00001ce0: 7468 6520 6669 7273 7420 7175 6572 7920  the first query 
+00001cf0: 7769 6c6c 2072 656d 6169 6e20 6f70 656e  will remain open
+00001d00: 2075 6e74 696c 2074 6865 2061 7070 6c69   until the appli
+00001d10: 6361 7469 6f6e 2069 7320 7374 6f70 7065  cation is stoppe
+00001d20: 6420 6f72 2074 6865 2065 6e67 696e 6520  d or the engine 
+00001d30: 6973 2074 6572 6d69 6e61 7465 643a 2063  is terminated: c
+00001d40: 6c6f 7365 5f65 6e67 696e 6528 292e 0d0a  lose_engine()...
+00001d50: 2727 270d 0a0d 0a61 7379 6e63 2064 6566  '''....async def
+00001d60: 206d 6574 686f 6473 2861 7379 6e63 5f73   methods(async_s
+00001d70: 6573 7369 6f6e 3a41 7379 6e63 5365 7373  ession:AsyncSess
+00001d80: 696f 6e29 3a0d 0a20 2020 2073 7461 7475  ion):..    statu
+00001d90: 732c 2064 6174 655f 7469 6d65 5f63 6865  s, date_time_che
+00001da0: 636b 5f63 6f6e 6e20 3d20 6177 6169 7420  ck_conn = await 
+00001db0: 6368 6563 6b5f 636f 6e6e 6563 7469 6f6e  check_connection
+00001dc0: 5f61 7379 6e63 2861 7379 6e63 5f73 6573  _async(async_ses
+00001dd0: 7369 6f6e 290d 0a20 2020 2069 6628 7374  sion)..    if(st
+00001de0: 6174 7573 293a 0d0a 2020 2020 2020 2020  atus):..        
+00001df0: 7175 6572 7920 3d20 7465 7874 5f74 6f5f  query = text_to_
+00001e00: 7371 6c28 2253 454c 4543 5420 6e6f 7728  sql("SELECT now(
+00001e10: 293b 2229 0d0a 2020 2020 2020 2020 7265  );")..        re
+00001e20: 7375 6c74 203d 2061 7761 6974 2061 7379  sult = await asy
+00001e30: 6e63 5f73 6573 7369 6f6e 2e65 7865 6375  nc_session.execu
+00001e40: 7465 2871 7565 7279 290d 0a20 2020 2020  te(query)..     
+00001e50: 2020 2073 696d 756c 6174 6564 5f71 7565     simulated_que
+00001e60: 7279 203d 2072 6573 756c 742e 7363 616c  ry = result.scal
+00001e70: 6172 5f6f 6e65 5f6f 725f 6e6f 6e65 2829  ar_one_or_none()
+00001e80: 0d0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
+00001e90: 636f 6d6d 6974 5f72 6f6c 6c62 6163 6b5f  commit_rollback_
+00001ea0: 6173 796e 6328 6173 796e 635f 7365 7373  async(async_sess
+00001eb0: 696f 6e29 0d0a 2020 2020 2020 2020 7072  ion)..        pr
+00001ec0: 696e 7428 6622 6461 7465 5f74 696d 655f  int(f"date_time_
+00001ed0: 6368 6563 6b5f 636f 6e6e 3d7b 6461 7465  check_conn={date
+00001ee0: 5f74 696d 655f 6368 6563 6b5f 636f 6e6e  _time_check_conn
+00001ef0: 7d2c 7369 6d75 6c61 7465 645f 7175 6572  },simulated_quer
+00001f00: 793d 7b73 696d 756c 6174 6564 5f71 7565  y={simulated_que
+00001f10: 7279 7d22 290d 0a20 2020 2065 6c73 653a  ry}")..    else:
+00001f20: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00001f30: 2261 7379 6e63 5f73 6573 7369 6f6e 2063  "async_session c
+00001f40: 6f6e 6e65 6374 2064 6220 6572 726f 722e  onnect db error.
+00001f50: 2e2e 2229 0d0a 6173 796e 6320 6465 6620  ..")..async def 
+00001f60: 6d61 696e 2829 3a0d 0a20 2020 2061 7379  main():..    asy
+00001f70: 6e63 2066 6f72 2061 7379 6e63 5f73 6573  nc for async_ses
+00001f80: 7369 6f6e 2069 6e20 636f 6e6e 5f61 7379  sion in conn_asy
+00001f90: 6e63 5f73 6573 7369 6f6e 2e67 6574 5f61  nc_session.get_a
+00001fa0: 7379 6e63 5f73 6573 7369 6f6e 2829 3a0d  sync_session():.
+00001fb0: 0a20 2020 2020 2020 2061 7761 6974 206d  .        await m
+00001fc0: 6574 686f 6473 2861 7379 6e63 5f73 6573  ethods(async_ses
+00001fd0: 7369 6f6e 290d 0a20 2020 2061 7761 6974  sion)..    await
+00001fe0: 2063 6f6e 6e5f 6173 796e 635f 7365 7373   conn_async_sess
+00001ff0: 696f 6e2e 636c 6f73 655f 656e 6769 6e65  ion.close_engine
+00002000: 2829 0d0a 0d0a 6966 205f 5f6e 616d 655f  ()....if __name_
+00002010: 5f20 3d3d 2022 5f5f 6d61 696e 5f5f 223a  _ == "__main__":
+00002020: 0d0a 2020 2020 6173 796e 6369 6f2e 7275  ..    asyncio.ru
+00002030: 6e28 6d61 696e 2829 290d 0a60 6060 0d0a  n(main())..```..
+00002040: 0d0a 2323 2073 796e 6368 726f 6e6f 7573  ..## synchronous
+00002050: 206d 6f64 650d 0a46 6173 7441 5049 0d0a   mode..FastAPI..
+00002060: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
+00002070: 6661 7374 6170 6920 696d 706f 7274 2046  fastapi import F
+00002080: 6173 7441 5049 2c20 4465 7065 6e64 732c  astAPI, Depends,
+00002090: 2048 5454 5045 7863 6570 7469 6f6e 0d0a   HTTPException..
+000020a0: 6672 6f6d 206c 6f67 7963 615f 706f 7374  from logyca_post
+000020b0: 6772 6573 2069 6d70 6f72 7420 5379 6e63  gres import Sync
+000020c0: 436f 6e6e 456e 6769 6e65 2c20 636f 6d6d  ConnEngine, comm
+000020d0: 6974 5f72 6f6c 6c62 6163 6b5f 7379 6e63  it_rollback_sync
+000020e0: 2c20 6368 6563 6b5f 636f 6e6e 6563 7469  , check_connecti
+000020f0: 6f6e 5f73 796e 630d 0a66 726f 6d20 7371  on_sync..from sq
+00002100: 6c61 6c63 6865 6d79 2e6f 726d 2e73 6573  lalchemy.orm.ses
+00002110: 7369 6f6e 2069 6d70 6f72 7420 5365 7373  sion import Sess
+00002120: 696f 6e0d 0a69 6d70 6f72 7420 6f73 0d0a  ion..import os..
+00002130: 6672 6f6d 2073 716c 616c 6368 656d 7920  from sqlalchemy 
+00002140: 696d 706f 7274 2074 6578 7420 6173 2074  import text as t
+00002150: 6578 745f 746f 5f73 716c 0d0a 0d0a 4442  ext_to_sql....DB
+00002160: 5f55 5345 523d 6f73 2e67 6574 656e 7628  _USER=os.getenv(
+00002170: 2744 425f 5553 4552 272c 2770 6f73 7467  'DB_USER','postg
+00002180: 7265 7327 290d 0a44 425f 5041 5353 3d6f  res')..DB_PASS=o
+00002190: 732e 6765 7465 6e76 2827 4442 5f50 4153  s.getenv('DB_PAS
+000021a0: 5327 2c27 7878 7827 290d 0a44 425f 484f  S','xxx')..DB_HO
+000021b0: 5354 3d6f 732e 6765 7465 6e76 2827 4442  ST=os.getenv('DB
+000021c0: 5f48 4f53 5427 2c27 6c6f 6361 6c68 6f73  _HOST','localhos
+000021d0: 7427 290d 0a44 425f 504f 5254 3d6f 732e  t')..DB_PORT=os.
+000021e0: 6765 7465 6e76 2827 4442 5f50 4f52 5427  getenv('DB_PORT'
+000021f0: 2c35 3433 3229 0d0a 4442 5f4e 414d 453d  ,5432)..DB_NAME=
+00002200: 6f73 2e67 6574 656e 7628 2744 425f 4e41  os.getenv('DB_NA
+00002210: 4d45 272c 2774 6573 7427 290d 0a73 736c  ME','test')..ssl
+00002220: 5f65 6e61 626c 655f 6c69 6b65 5f6c 6f63  _enable_like_loc
+00002230: 616c 5f64 6f63 6b65 725f 636f 6e74 6169  al_docker_contai
+00002240: 6e65 723d 4661 6c73 650d 0a0d 0a61 7070  ner=False....app
+00002250: 203d 2046 6173 7441 5049 2829 0d0a 0d0a   = FastAPI()....
+00002260: 636f 6e6e 5f73 796e 635f 7365 7373 696f  conn_sync_sessio
+00002270: 6e3d 5379 6e63 436f 6e6e 456e 6769 6e65  n=SyncConnEngine
+00002280: 280d 0a20 2020 2075 726c 5f63 6f6e 6e65  (..    url_conne
+00002290: 6374 696f 6e3d 5379 6e63 436f 6e6e 456e  ction=SyncConnEn
+000022a0: 6769 6e65 2e62 7569 6c64 5f75 726c 5f63  gine.build_url_c
+000022b0: 6f6e 6e65 6374 696f 6e28 7573 6572 3d44  onnection(user=D
+000022c0: 425f 5553 4552 2c70 6173 7377 6f72 643d  B_USER,password=
+000022d0: 4442 5f50 4153 532c 686f 7374 3d44 425f  DB_PASS,host=DB_
+000022e0: 484f 5354 2c70 6f72 743d 4442 5f50 4f52  HOST,port=DB_POR
+000022f0: 542c 6461 7461 6261 7365 3d44 425f 4e41  T,database=DB_NA
+00002300: 4d45 2c73 736c 5f65 6e61 626c 653d 7373  ME,ssl_enable=ss
+00002310: 6c5f 656e 6162 6c65 5f6c 696b 655f 6c6f  l_enable_like_lo
+00002320: 6361 6c5f 646f 636b 6572 5f63 6f6e 7461  cal_docker_conta
+00002330: 696e 6572 292c 0d0a 2020 2020 7365 7276  iner),..    serv
+00002340: 6572 5f73 6574 7469 6e67 733d 5379 6e63  er_settings=Sync
+00002350: 436f 6e6e 456e 6769 6e65 2e73 6572 7665  ConnEngine.serve
+00002360: 725f 7365 7474 696e 6773 2870 6f6f 6c5f  r_settings(pool_
+00002370: 7369 7a65 3d35 2c6d 6178 5f6f 7665 7266  size=5,max_overf
+00002380: 6c6f 773d 312c 706f 6f6c 5f72 6563 7963  low=1,pool_recyc
+00002390: 6c65 3d31 3038 3030 2c61 7070 6c69 6361  le=10800,applica
+000023a0: 7469 6f6e 5f6e 616d 653d 224d 7941 7070  tion_name="MyApp
+000023b0: 202d 2041 7379 6e63 436f 6e6e 456e 6769   - AsyncConnEngi
+000023c0: 6e65 2229 0d0a 2020 2020 290d 0a0d 0a27  ne")..    )....'
+000023d0: 2727 0d0a 5468 6520 636f 6e6e 6563 7469  ''..The connecti
+000023e0: 6f6e 2070 6f6f 6c20 2870 6f6f 6c5f 7369  on pool (pool_si
+000023f0: 7a65 2920 6166 7465 7220 7468 6520 6669  ze) after the fi
+00002400: 7273 7420 7175 6572 7920 7769 6c6c 2072  rst query will r
+00002410: 656d 6169 6e20 6f70 656e 2075 6e74 696c  emain open until
+00002420: 2074 6865 2061 7070 6c69 6361 7469 6f6e   the application
+00002430: 2069 7320 7374 6f70 7065 642e 0d0a 2727   is stopped...''
+00002440: 270d 0a0d 0a40 6170 702e 6765 7428 222f  '....@app.get("/
+00002450: 7369 6d75 6c61 7465 645f 7175 6572 795f  simulated_query_
+00002460: 7379 6e63 2f22 290d 0a64 6566 2072 6561  sync/")..def rea
+00002470: 645f 6974 656d 2873 796e 635f 7365 7373  d_item(sync_sess
+00002480: 696f 6e3a 5365 7373 696f 6e20 3d20 4465  ion:Session = De
+00002490: 7065 6e64 7328 636f 6e6e 5f73 796e 635f  pends(conn_sync_
+000024a0: 7365 7373 696f 6e29 293a 0d0a 2020 2020  session)):..    
+000024b0: 7472 793a 0d0a 2020 2020 2020 2020 7374  try:..        st
+000024c0: 6174 7573 2c20 6461 7465 5f74 696d 655f  atus, date_time_
+000024d0: 6368 6563 6b5f 636f 6e6e 203d 2063 6865  check_conn = che
+000024e0: 636b 5f63 6f6e 6e65 6374 696f 6e5f 7379  ck_connection_sy
+000024f0: 6e63 2873 796e 635f 7365 7373 696f 6e29  nc(sync_session)
+00002500: 0d0a 2020 2020 2020 2020 6966 2873 7461  ..        if(sta
+00002510: 7475 7329 3a0d 0a20 2020 2020 2020 2020  tus):..         
+00002520: 2020 2071 7565 7279 203d 2074 6578 745f     query = text_
+00002530: 746f 5f73 716c 2822 5345 4c45 4354 206e  to_sql("SELECT n
+00002540: 6f77 2829 3b22 290d 0a20 2020 2020 2020  ow();")..       
+00002550: 2020 2020 2072 6573 756c 7420 3d20 7379       result = sy
+00002560: 6e63 5f73 6573 7369 6f6e 2e65 7865 6375  nc_session.execu
+00002570: 7465 2871 7565 7279 290d 0a20 2020 2020  te(query)..     
+00002580: 2020 2020 2020 2073 696d 756c 6174 6564         simulated
+00002590: 5f71 7565 7279 203d 2072 6573 756c 742e  _query = result.
+000025a0: 6665 7463 686f 6e65 2829 5b30 5d0d 0a20  fetchone()[0].. 
+000025b0: 2020 2020 2020 2020 2020 2063 6f6d 6d69             commi
+000025c0: 745f 726f 6c6c 6261 636b 5f73 796e 6328  t_rollback_sync(
+000025d0: 7379 6e63 5f73 6573 7369 6f6e 290d 0a20  sync_session).. 
+000025e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000025f0: 6e20 7b22 6461 7465 5f74 696d 655f 6368  n {"date_time_ch
+00002600: 6563 6b5f 636f 6e6e 223a 2064 6174 655f  eck_conn": date_
+00002610: 7469 6d65 5f63 6865 636b 5f63 6f6e 6e2c  time_check_conn,
+00002620: 2022 7369 6d75 6c61 7465 645f 7175 6572   "simulated_quer
+00002630: 7922 3a20 7369 6d75 6c61 7465 645f 7175  y": simulated_qu
+00002640: 6572 797d 0d0a 2020 2020 2020 2020 656c  ery}..        el
+00002650: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00002660: 2072 6169 7365 2048 5454 5045 7863 6570   raise HTTPExcep
+00002670: 7469 6f6e 2873 7461 7475 735f 636f 6465  tion(status_code
+00002680: 3d34 3034 2c20 6465 7461 696c 3d22 6173  =404, detail="as
+00002690: 796e 635f 7365 7373 696f 6e20 636f 6e6e  ync_session conn
+000026a0: 6563 7420 6462 2065 7272 6f72 2e2e 2e22  ect db error..."
+000026b0: 290d 0a20 2020 2065 7863 6570 7420 4578  )..    except Ex
+000026c0: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
+000026d0: 2020 2020 2020 2072 6169 7365 2048 5454         raise HTT
+000026e0: 5045 7863 6570 7469 6f6e 2873 7461 7475  PException(statu
+000026f0: 735f 636f 6465 3d34 3034 2c20 6465 7461  s_code=404, deta
+00002700: 696c 3d66 2265 7272 6f72 3a20 7b65 7d22  il=f"error: {e}"
+00002710: 290d 0a60 6060 0d0a 576f 726b 6572 206f  )..```..Worker o
+00002720: 7220 7363 7269 7074 0d0a 6060 6070 7974  r script..```pyt
+00002730: 686f 6e0d 0a66 726f 6d20 6c6f 6779 6361  hon..from logyca
+00002740: 5f70 6f73 7467 7265 7320 696d 706f 7274  _postgres import
+00002750: 2053 796e 6343 6f6e 6e45 6e67 696e 652c   SyncConnEngine,
+00002760: 2063 6f6d 6d69 745f 726f 6c6c 6261 636b   commit_rollback
+00002770: 5f73 796e 632c 2063 6865 636b 5f63 6f6e  _sync, check_con
+00002780: 6e65 6374 696f 6e5f 7379 6e63 0d0a 6672  nection_sync..fr
+00002790: 6f6d 2073 716c 616c 6368 656d 7920 696d  om sqlalchemy im
+000027a0: 706f 7274 2074 6578 7420 6173 2074 6578  port text as tex
+000027b0: 745f 746f 5f73 716c 0d0a 6672 6f6d 2073  t_to_sql..from s
+000027c0: 716c 616c 6368 656d 792e 6f72 6d2e 7365  qlalchemy.orm.se
+000027d0: 7373 696f 6e20 696d 706f 7274 2053 6573  ssion import Ses
+000027e0: 7369 6f6e 0d0a 696d 706f 7274 206f 730d  sion..import os.
+000027f0: 0a0d 0a44 425f 5553 4552 3d6f 732e 6765  ...DB_USER=os.ge
+00002800: 7465 6e76 2827 4442 5f55 5345 5227 2c27  tenv('DB_USER','
+00002810: 706f 7374 6772 6573 2729 0d0a 4442 5f50  postgres')..DB_P
+00002820: 4153 533d 6f73 2e67 6574 656e 7628 2744  ASS=os.getenv('D
+00002830: 425f 5041 5353 272c 272a 2a2a 2729 0d0a  B_PASS','***')..
+00002840: 4442 5f48 4f53 543d 6f73 2e67 6574 656e  DB_HOST=os.geten
+00002850: 7628 2744 425f 484f 5354 272c 276c 6f63  v('DB_HOST','loc
+00002860: 616c 686f 7374 2729 0d0a 4442 5f50 4f52  alhost')..DB_POR
+00002870: 543d 6f73 2e67 6574 656e 7628 2744 425f  T=os.getenv('DB_
+00002880: 504f 5254 272c 3534 3332 290d 0a44 425f  PORT',5432)..DB_
+00002890: 4e41 4d45 3d6f 732e 6765 7465 6e76 2827  NAME=os.getenv('
+000028a0: 4442 5f4e 414d 4527 2c27 7465 7374 2729  DB_NAME','test')
+000028b0: 0d0a 7373 6c5f 656e 6162 6c65 5f6c 696b  ..ssl_enable_lik
+000028c0: 655f 6c6f 6361 6c5f 646f 636b 6572 5f63  e_local_docker_c
+000028d0: 6f6e 7461 696e 6572 3d46 616c 7365 0d0a  ontainer=False..
+000028e0: 0d0a 636f 6e6e 5f73 796e 635f 7365 7373  ..conn_sync_sess
+000028f0: 696f 6e3d 5379 6e63 436f 6e6e 456e 6769  ion=SyncConnEngi
+00002900: 6e65 280d 0a20 2020 2075 726c 5f63 6f6e  ne(..    url_con
+00002910: 6e65 6374 696f 6e3d 5379 6e63 436f 6e6e  nection=SyncConn
+00002920: 456e 6769 6e65 2e62 7569 6c64 5f75 726c  Engine.build_url
+00002930: 5f63 6f6e 6e65 6374 696f 6e28 7573 6572  _connection(user
+00002940: 3d44 425f 5553 4552 2c70 6173 7377 6f72  =DB_USER,passwor
+00002950: 643d 4442 5f50 4153 532c 686f 7374 3d44  d=DB_PASS,host=D
+00002960: 425f 484f 5354 2c70 6f72 743d 4442 5f50  B_HOST,port=DB_P
+00002970: 4f52 542c 6461 7461 6261 7365 3d44 425f  ORT,database=DB_
+00002980: 4e41 4d45 2c73 736c 5f65 6e61 626c 653d  NAME,ssl_enable=
+00002990: 7373 6c5f 656e 6162 6c65 5f6c 696b 655f  ssl_enable_like_
+000029a0: 6c6f 6361 6c5f 646f 636b 6572 5f63 6f6e  local_docker_con
+000029b0: 7461 696e 6572 292c 0d0a 2020 2020 7365  tainer),..    se
+000029c0: 7276 6572 5f73 6574 7469 6e67 733d 5379  rver_settings=Sy
+000029d0: 6e63 436f 6e6e 456e 6769 6e65 2e73 6572  ncConnEngine.ser
+000029e0: 7665 725f 7365 7474 696e 6773 2870 6f6f  ver_settings(poo
+000029f0: 6c5f 7369 7a65 3d35 2c6d 6178 5f6f 7665  l_size=5,max_ove
+00002a00: 7266 6c6f 773d 312c 706f 6f6c 5f72 6563  rflow=1,pool_rec
+00002a10: 7963 6c65 3d31 3038 3030 2c61 7070 6c69  ycle=10800,appli
+00002a20: 6361 7469 6f6e 5f6e 616d 653d 224d 7941  cation_name="MyA
+00002a30: 7070 202d 2053 796e 6343 6f6e 6e45 6e67  pp - SyncConnEng
+00002a40: 696e 6522 290d 0a20 2020 2020 2020 2020  ine")..         
+00002a50: 2020 2029 0d0a 0d0a 2727 270d 0a54 6865     )....'''..The
+00002a60: 2063 6f6e 6e65 6374 696f 6e20 706f 6f6c   connection pool
+00002a70: 2028 706f 6f6c 5f73 697a 6529 2061 6674   (pool_size) aft
+00002a80: 6572 2074 6865 2066 6972 7374 2071 7565  er the first que
+00002a90: 7279 2077 696c 6c20 7265 6d61 696e 206f  ry will remain o
+00002aa0: 7065 6e20 756e 7469 6c20 7468 6520 6170  pen until the ap
+00002ab0: 706c 6963 6174 696f 6e20 6973 2073 746f  plication is sto
+00002ac0: 7070 6564 206f 7220 7468 6520 656e 6769  pped or the engi
+00002ad0: 6e65 2069 7320 7465 726d 696e 6174 6564  ne is terminated
+00002ae0: 3a20 636c 6f73 655f 656e 6769 6e65 2829  : close_engine()
+00002af0: 2e0d 0a27 2727 0d0a 0d0a 6465 6620 6d65  ...'''....def me
+00002b00: 7468 6f64 7328 7379 6e63 5f73 6573 7369  thods(sync_sessi
+00002b10: 6f6e 3a20 5365 7373 696f 6e29 3a0d 0a20  on: Session):.. 
+00002b20: 2020 2073 7461 7475 732c 2064 6174 655f     status, date_
+00002b30: 7469 6d65 5f63 6865 636b 5f63 6f6e 6e20  time_check_conn 
+00002b40: 3d20 6368 6563 6b5f 636f 6e6e 6563 7469  = check_connecti
+00002b50: 6f6e 5f73 796e 6328 7379 6e63 5f73 6573  on_sync(sync_ses
+00002b60: 7369 6f6e 290d 0a20 2020 2069 6628 7374  sion)..    if(st
+00002b70: 6174 7573 293a 0d0a 2020 2020 2020 2020  atus):..        
+00002b80: 7175 6572 7920 3d20 7465 7874 5f74 6f5f  query = text_to_
+00002b90: 7371 6c28 2253 454c 4543 5420 6e6f 7728  sql("SELECT now(
+00002ba0: 293b 2229 0d0a 2020 2020 2020 2020 7265  );")..        re
+00002bb0: 7375 6c74 203d 2073 796e 635f 7365 7373  sult = sync_sess
+00002bc0: 696f 6e2e 6578 6563 7574 6528 7175 6572  ion.execute(quer
+00002bd0: 7929 0d0a 2020 2020 2020 2020 7369 6d75  y)..        simu
+00002be0: 6c61 7465 645f 7175 6572 7920 3d20 7265  lated_query = re
+00002bf0: 7375 6c74 2e66 6574 6368 6f6e 6528 295b  sult.fetchone()[
+00002c00: 305d 0d0a 2020 2020 2020 2020 636f 6d6d  0]..        comm
+00002c10: 6974 5f72 6f6c 6c62 6163 6b5f 7379 6e63  it_rollback_sync
+00002c20: 2873 796e 635f 7365 7373 696f 6e29 0d0a  (sync_session)..
+00002c30: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
+00002c40: 6461 7465 5f74 696d 655f 6368 6563 6b5f  date_time_check_
+00002c50: 636f 6e6e 3d7b 6461 7465 5f74 696d 655f  conn={date_time_
+00002c60: 6368 6563 6b5f 636f 6e6e 7d2c 7369 6d75  check_conn},simu
+00002c70: 6c61 7465 645f 7175 6572 793d 7b73 696d  lated_query={sim
+00002c80: 756c 6174 6564 5f71 7565 7279 7d22 290d  ulated_query}").
+00002c90: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
+00002ca0: 2020 2020 7072 696e 7428 2273 796e 635f      print("sync_
+00002cb0: 7365 7373 696f 6e20 636f 6e6e 6563 7420  session connect 
+00002cc0: 6462 2065 7272 6f72 2e2e 2e22 290d 0a64  db error...")..d
+00002cd0: 6566 206d 6169 6e28 293a 0d0a 2020 2020  ef main():..    
+00002ce0: 666f 7220 7379 6e63 5f73 6573 7369 6f6e  for sync_session
+00002cf0: 2069 6e20 636f 6e6e 5f73 796e 635f 7365   in conn_sync_se
+00002d00: 7373 696f 6e2e 6765 745f 7379 6e63 5f73  ssion.get_sync_s
+00002d10: 6573 7369 6f6e 2829 3a0d 0a20 2020 2020  ession():..     
+00002d20: 2020 206d 6574 686f 6473 2873 796e 635f     methods(sync_
+00002d30: 7365 7373 696f 6e29 0d0a 2020 2020 636f  session)..    co
+00002d40: 6e6e 5f73 796e 635f 7365 7373 696f 6e2e  nn_sync_session.
+00002d50: 636c 6f73 655f 656e 6769 6e65 2829 2020  close_engine()  
+00002d60: 2020 2020 2020 2020 2020 0d0a 0d0a 0d0a            ......
+00002d70: 6966 205f 5f6e 616d 655f 5f20 3d3d 2022  if __name__ == "
+00002d80: 5f5f 6d61 696e 5f5f 223a 0d0a 2020 2020  __main__":..    
+00002d90: 6d61 696e 2829 0d0a 6060 600d 0a0d 0a2d  main()..```....-
+00002da0: 2d2d 0d0a 0d0a 2320 4368 616e 6765 6c6f  --....# Changelo
+00002db0: 670d 0a0d 0a41 6c6c 206e 6f74 6162 6c65  g....All notable
+00002dc0: 2063 6861 6e67 6573 2074 6f20 7468 6973   changes to this
+00002dd0: 2070 726f 6a65 6374 2077 696c 6c20 6265   project will be
+00002de0: 2064 6f63 756d 656e 7465 6420 696e 2074   documented in t
+00002df0: 6869 7320 6669 6c65 2e0d 0a0d 0a54 6865  his file.....The
+00002e00: 2066 6f72 6d61 7420 6973 2062 6173 6564   format is based
+00002e10: 206f 6e20 5b4b 6565 7020 6120 4368 616e   on [Keep a Chan
+00002e20: 6765 6c6f 675d 2868 7474 7073 3a2f 2f6b  gelog](https://k
+00002e30: 6565 7061 6368 616e 6765 6c6f 672e 636f  eepachangelog.co
+00002e40: 6d2f 656e 2f31 2e30 2e30 2f29 2c0d 0a61  m/en/1.0.0/),..a
+00002e50: 6e64 2074 6869 7320 7072 6f6a 6563 7420  nd this project 
+00002e60: 6164 6865 7265 7320 746f 205b 5365 6d61  adheres to [Sema
+00002e70: 6e74 6963 2056 6572 7369 6f6e 696e 675d  ntic Versioning]
+00002e80: 2868 7474 7073 3a2f 2f73 656d 7665 722e  (https://semver.
+00002e90: 6f72 672f 7370 6563 2f76 322e 302e 302e  org/spec/v2.0.0.
+00002ea0: 6874 6d6c 292e 0d0a 0d0a 2323 2054 7970  html).....## Typ
+00002eb0: 6573 206f 6620 6368 616e 6765 730d 0a0d  es of changes...
+00002ec0: 0a2d 2041 6464 6564 2066 6f72 206e 6577  .- Added for new
+00002ed0: 2066 6561 7475 7265 732e 0d0a 2d20 4368   features...- Ch
+00002ee0: 616e 6765 6420 666f 7220 6368 616e 6765  anged for change
+00002ef0: 7320 696e 2065 7869 7374 696e 6720 6675  s in existing fu
+00002f00: 6e63 7469 6f6e 616c 6974 792e 0d0a 2d20  nctionality...- 
+00002f10: 4465 7072 6563 6174 6564 2066 6f72 2073  Deprecated for s
+00002f20: 6f6f 6e2d 746f 2d62 6520 7265 6d6f 7665  oon-to-be remove
+00002f30: 6420 6665 6174 7572 6573 2e0d 0a2d 2052  d features...- R
+00002f40: 656d 6f76 6564 2066 6f72 206e 6f77 2072  emoved for now r
+00002f50: 656d 6f76 6564 2066 6561 7475 7265 732e  emoved features.
+00002f60: 0d0a 2d20 4669 7865 6420 666f 7220 616e  ..- Fixed for an
+00002f70: 7920 6275 6720 6669 7865 732e 0d0a 2d20  y bug fixes...- 
+00002f80: 5365 6375 7269 7479 2069 6e20 6361 7365  Security in case
+00002f90: 206f 6620 7675 6c6e 6572 6162 696c 6974   of vulnerabilit
+00002fa0: 6965 732e 0d0a 0d0a 2323 205b 302e 302e  ies.....## [0.0.
+00002fb0: 3172 6331 5d20 2d20 3230 3234 2d30 342d  1rc1] - 2024-04-
+00002fc0: 3232 0d0a 2323 2320 4164 6465 640d 0a2d  22..### Added..-
+00002fd0: 2046 6972 7374 2074 6573 7473 2075 7369   First tests usi
+00002fe0: 6e67 2070 7970 692e 6f72 6720 696e 2064  ng pypi.org in d
+00002ff0: 6576 656c 6f70 2065 6e76 6972 6f6e 6d65  evelop environme
+00003000: 6e74 2e0d 0a2d 204e 6577 2066 756e 6374  nt...- New funct
+00003010: 696f 6e61 6c69 7479 206f 6620 6173 796e  ionality of asyn
+00003020: 6368 726f 6e6f 7573 2061 6e64 2073 796e  chronous and syn
+00003030: 6368 726f 6e6f 7573 2063 6f6e 6e65 6374  chronous connect
+00003040: 696f 6e73 2074 6f20 706f 7374 6772 6573  ions to postgres
+00003050: 716c 2064 6174 6162 6173 6573 2e0d 0a2d  ql databases...-
+00003060: 2046 756e 6374 696f 6e61 6c69 7469 6573   Functionalities
+00003070: 2063 616e 2062 6520 7573 6564 2069 6e20   can be used in 
+00003080: 6661 7374 6170 6920 6f72 2077 6f72 6b65  fastapi or worke
+00003090: 7273 206c 696b 6520 417a 7572 6520 4675  rs like Azure Fu
+000030a0: 6e63 7469 6f6e 732e 0d0a 2d20 4578 616d  nctions...- Exam
+000030b0: 706c 6573 206f 6620 7573 6520 6172 6520  ples of use are 
+000030c0: 6164 6465 6420 746f 2074 6865 2064 6f63  added to the doc
+000030d0: 756d 656e 7461 7469 6f6e 206f 6620 7468  umentation of th
+000030e0: 6520 6675 6e63 7469 6f6e 7320 696e 2064  e functions in d
+000030f0: 6f63 7374 7269 6e67 0d0a 2d20 496e 2074  ocstring..- In t
+00003100: 6865 2073 616d 706c 6573 2066 6f6c 6465  he samples folde
+00003110: 7220 6f66 2074 6869 7320 6c69 6272 6172  r of this librar
+00003120: 792c 2074 6865 7265 2061 7265 2063 6f6d  y, there are com
+00003130: 706c 6574 6520 776f 726b 696e 6720 6578  plete working ex
+00003140: 616d 706c 6573 206f 6620 7573 696e 6720  amples of using 
+00003150: 7468 6520 636f 6465 2e0d 0a0d 0a23 2320  the code.....## 
+00003160: 5b30 2e31 2e30 5d20 2d20 3230 3234 2d30  [0.1.0] - 2024-0
+00003170: 352d 3231 0d0a 2323 2320 4164 6465 640d  5-21..### Added.
+00003180: 0a2d 2043 6f6d 706c 6574 696f 6e20 6f66  .- Completion of
+00003190: 2074 6573 7469 6e67 2061 6e64 206c 6175   testing and lau
+000031a0: 6e63 6820 696e 746f 2070 726f 6475 6374  nch into product
+000031b0: 696f 6e2e 0d0a 0d0a 2323 205b 302e 312e  ion.....## [0.1.
+000031c0: 325d 202d 2032 3032 342d 3035 2d32 330d  2] - 2024-05-23.
+000031d0: 0a23 2323 2041 6464 6564 0d0a 2d20 446f  .### Added..- Do
+000031e0: 6375 6d65 6e74 6174 696f 6e20 696e 7465  cumentation inte
+000031f0: 6772 6174 6564 2077 6974 6820 6769 7468  grated with gith
+00003200: 7562                                     ub
```

### Comparing `logyca_postgres-0.1.1/logyca_postgres/__init__.py` & `logyca_postgres-0.1.2rc1/logyca_postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.1/logyca_postgres/dependencies/conn_postgres_async.py` & `logyca_postgres-0.1.2rc1/logyca_postgres/dependencies/conn_postgres_async.py`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.1/logyca_postgres/dependencies/conn_postgres_sync.py` & `logyca_postgres-0.1.2rc1/logyca_postgres/dependencies/conn_postgres_sync.py`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.1/logyca_postgres.egg-info/PKG-INFO` & `logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: logyca-postgres
-Version: 0.1.1
+Version: 0.1.2rc1
 Summary: An integration package created by the company LOGYCA that connects Postgres and is used to standardize connections and dependency injection in synchronous or asynchronous mode. Tested in fastapi and in console/worker scripts.
 Home-page: https://github.com/logyca/<soon>
 Author: Jaime Andres Cardona Carrillo
-Author-email: tecnologiaeinformacion@logyca.com
+Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: postgres,driver database
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
@@ -63,15 +63,15 @@
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/logyca" target="_blank">
     <img src="https://img.shields.io/pypi/v/logyca?color=orange&label=PyPI%20Package" alt="Package version">
 </a>
 <a href="(https://www.python.org" target="_blank">
-    <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.7%2C%3C%3D3.11%5D-orange" alt="Python">
+    <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.8%2C%3C%3D3.11%5D-orange" alt="Python">
 </a>
 </p>
 
 
 ---
 
 # About us
@@ -80,18 +80,21 @@
 * <a href="https://www.youtube.com/channel/UCzcJtxfScoAtwFbxaLNnEtA" target="_blank">LOGYCA Youtube Channel</a>
 * <a href="https://www.linkedin.com/company/logyca" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="Linkedin"></a>
 * <a href="https://twitter.com/LOGYCA_Org" target="_blank"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter"></a>
 * <a href="https://www.facebook.com/OrganizacionLOGYCA/" target="_blank"><img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook"></a>
 
 ---
 
-# What's libraries
+# LOGYCA public libraries: Standard methods to connect to postgres
 
 * **Traversal libraries**: Standard methods to connect to postgres with dependency injection using yield to be used by microservices such as API(s), Workers or scripts.
 
+[Source code](https://github.com/logyca/python-libraries)
+| [Package (PyPI)](https://pypi.org/project/logyca-postgres/)
+
 ---
 
 # "pip install" dependency check
 The user must select the required libraries and versions for the project that uses this library, which validates that they are pre-installed in order to be installed.
 
 To install the libraries of the logyca postgres package verifying the SQLAlchemy prerequisite without validating connection drivers to postgres, use the following command:
 
@@ -340,7 +343,11 @@
 - Functionalities can be used in fastapi or workers like Azure Functions.
 - Examples of use are added to the documentation of the functions in docstring
 - In the samples folder of this library, there are complete working examples of using the code.
 
 ## [0.1.0] - 2024-05-21
 ### Added
 - Completion of testing and launch into production.
+
+## [0.1.2] - 2024-05-23
+### Added
+- Documentation integrated with github
```

#### html2text {}

```diff
@@ -1,65 +1,67 @@
-Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.1 Summary: An
+Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.2rc1 Summary: An
 integration package created by the company LOGYCA that connects Postgres and is
 used to standardize connections and dependency injection in synchronous or
 asynchronous mode. Tested in fastapi and in console/worker scripts. Home-page:
 https://github.com/logyca/ Author: Jaime Andres Cardona Carrillo Author-email:
-tecnologiaeinformacion@logyca.com License: MIT License Keywords:
-postgres,driver database Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Information
-Technology Classifier: Intended Audience :: System Administrators Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python Classifier: Topic :: Database Classifier: Topic
-:: Database :: Front-Ends Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Software Development Classifier: Typing :: Typed
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE.txt Requires-Dist: SQLAlchemy>=2.0.6 Requires-Dist: starlette>=0.24.0
-Provides-Extra: async Requires-Dist: SQLAlchemy>=2.0.6; extra == "async"
-Requires-Dist: starlette>=0.24.0; extra == "async" Requires-Dist:
-asyncpg>=0.27.0; extra == "async" Provides-Extra: sync-psycopg2 Requires-Dist:
-SQLAlchemy>=2.0.6; extra == "sync-psycopg2" Requires-Dist: starlette>=0.24.0;
-extra == "sync-psycopg2" Requires-Dist: psycopg2>=2.9.6; extra == "sync-
-psycopg2" Provides-Extra: sync-psycopg2-binary Requires-Dist:
-SQLAlchemy>=2.0.6; extra == "sync-psycopg2-binary" Requires-Dist:
-starlette>=0.24.0; extra == "sync-psycopg2-binary" Requires-Dist: psycopg2-
-binary>=2.9.6; extra == "sync-psycopg2-binary" Provides-Extra: async-sync-
-psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra == "async-sync-psycopg2"
-Requires-Dist: starlette>=0.24.0; extra == "async-sync-psycopg2" Requires-Dist:
-asyncpg>=0.27.0; extra == "async-sync-psycopg2" Requires-Dist: psycopg2>=2.9.6;
-extra == "async-sync-psycopg2" Provides-Extra: async-sync-psycopg2-binary
-Requires-Dist: SQLAlchemy>=2.0.6; extra == "async-sync-psycopg2-binary"
-Requires-Dist: starlette>=0.24.0; extra == "async-sync-psycopg2-binary"
-Requires-Dist: asyncpg>=0.27.0; extra == "async-sync-psycopg2-binary" Requires-
-Dist: psycopg2-binary>=2.9.6; extra == "async-sync-psycopg2-binary"
+jacardona@outlook.com License: MIT License Keywords: postgres,driver database
+Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Information Technology Classifier:
+Intended Audience :: System Administrators Classifier: License :: OSI Approved
+:: MIT License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+Classifier: Topic :: Database Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development Classifier: Typing :: Typed Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
+Dist: SQLAlchemy>=2.0.6 Requires-Dist: starlette>=0.24.0 Provides-Extra: async
+Requires-Dist: SQLAlchemy>=2.0.6; extra == "async" Requires-Dist:
+starlette>=0.24.0; extra == "async" Requires-Dist: asyncpg>=0.27.0; extra ==
+"async" Provides-Extra: sync-psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra
+== "sync-psycopg2" Requires-Dist: starlette>=0.24.0; extra == "sync-psycopg2"
+Requires-Dist: psycopg2>=2.9.6; extra == "sync-psycopg2" Provides-Extra: sync-
+psycopg2-binary Requires-Dist: SQLAlchemy>=2.0.6; extra == "sync-psycopg2-
+binary" Requires-Dist: starlette>=0.24.0; extra == "sync-psycopg2-binary"
+Requires-Dist: psycopg2-binary>=2.9.6; extra == "sync-psycopg2-binary"
+Provides-Extra: async-sync-psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra ==
+"async-sync-psycopg2" Requires-Dist: starlette>=0.24.0; extra == "async-sync-
+psycopg2" Requires-Dist: asyncpg>=0.27.0; extra == "async-sync-psycopg2"
+Requires-Dist: psycopg2>=2.9.6; extra == "async-sync-psycopg2" Provides-Extra:
+async-sync-psycopg2-binary Requires-Dist: SQLAlchemy>=2.0.6; extra == "async-
+sync-psycopg2-binary" Requires-Dist: starlette>=0.24.0; extra == "async-sync-
+psycopg2-binary" Requires-Dist: asyncpg>=0.27.0; extra == "async-sync-psycopg2-
+binary" Requires-Dist: psycopg2-binary>=2.9.6; extra == "async-sync-psycopg2-
+binary"
                                    _[_L_o_g_y_c_a_]
                             LLOOGGYYCCAA ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # About us * _L_O_G_Y_C_A_ _C_o_m_p_a_n_y * _L_O_G_Y_C_A_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l * _[_L_i_n_k_e_d_i_n_]*
-_[_T_w_i_t_t_e_r_]* _[_F_a_c_e_b_o_o_k_]--- # What's libraries * **Traversal libraries**: Standard
-methods to connect to postgres with dependency injection using yield to be used
-by microservices such as API(s), Workers or scripts. --- # "pip install"
-dependency check The user must select the required libraries and versions for
-the project that uses this library, which validates that they are pre-installed
-in order to be installed. To install the libraries of the logyca postgres
-package verifying the SQLAlchemy prerequisite without validating connection
-drivers to postgres, use the following command: ```Python # Check SQLAlchemy
-dependency that is installed pip install logyca_postgres ``` To install the
-logyca postgres package libraries and validate the postgres asynchronous or
-synchronous connection driver, use the following command: ```Python # Check
-asyncpg driver dependency that is installed pip install logyca_postgres[async]
-# Check psycopg2 driver dependency that is installed pip install
-logyca_postgres[sync-psycopg2] # Check psycopg2-binary driver dependency that
-is installed pip install logyca_postgres[sync-psycopg2-binary] # Check
-asyncpg+psycopg2-binary driver dependency that is installed pip install
+_[_T_w_i_t_t_e_r_]* _[_F_a_c_e_b_o_o_k_]--- # LOGYCA public libraries: Standard methods to connect
+to postgres * **Traversal libraries**: Standard methods to connect to postgres
+with dependency injection using yield to be used by microservices such as API
+(s), Workers or scripts. [Source code](https://github.com/logyca/python-
+libraries) | [Package (PyPI)](https://pypi.org/project/logyca-postgres/) --- #
+"pip install" dependency check The user must select the required libraries and
+versions for the project that uses this library, which validates that they are
+pre-installed in order to be installed. To install the libraries of the logyca
+postgres package verifying the SQLAlchemy prerequisite without validating
+connection drivers to postgres, use the following command: ```Python # Check
+SQLAlchemy dependency that is installed pip install logyca_postgres ``` To
+install the logyca postgres package libraries and validate the postgres
+asynchronous or synchronous connection driver, use the following command:
+```Python # Check asyncpg driver dependency that is installed pip install
+logyca_postgres[async] # Check psycopg2 driver dependency that is installed pip
+install logyca_postgres[sync-psycopg2] # Check psycopg2-binary driver
+dependency that is installed pip install logyca_postgres[sync-psycopg2-binary]
+# Check asyncpg+psycopg2-binary driver dependency that is installed pip install
 logyca_postgres[async-sync-psycopg2] ``` --- # Semantic Versioning logyca <
 MAJOR >.< MINOR >.< PATCH > * **MAJOR**: version when you make incompatible API
 changes * **MINOR**: version when you add functionality in a backwards
 compatible manner * **PATCH**: version when you make backwards compatible bug
 fixes ## Definitions for releasing versions * https://peps.python.org/pep-0440/
 - X.YaN (Alpha release): Identify and fix early-stage bugs. Not suitable for
 production use. - X.YbN (Beta release): Stabilize and refine features. Address
@@ -178,8 +180,9 @@
 Security in case of vulnerabilities. ## [0.0.1rc1] - 2024-04-22 ### Added -
 First tests using pypi.org in develop environment. - New functionality of
 asynchronous and synchronous connections to postgresql databases. -
 Functionalities can be used in fastapi or workers like Azure Functions. -
 Examples of use are added to the documentation of the functions in docstring -
 In the samples folder of this library, there are complete working examples of
 using the code. ## [0.1.0] - 2024-05-21 ### Added - Completion of testing and
-launch into production.
+launch into production. ## [0.1.2] - 2024-05-23 ### Added - Documentation
+integrated with github
```

### Comparing `logyca_postgres-0.1.1/logyca_postgres.egg-info/SOURCES.txt` & `logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.1/setup.py` & `logyca_postgres-0.1.2rc1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="LOGYCA"
 PACKAGE_NAME = "logyca-postgres"
-VERSION = "0.1.1"
+VERSION = "0.1.2rc1"
 
 install_requires = ["SQLAlchemy>=2.0.6","starlette>=0.24.0"]
 install_requires_asyncpg = ["asyncpg >=0.27.0"]
 install_requires_psycopg2 = ["psycopg2 >=2.9.6"]
 install_requires_psycopg2_binary = ["psycopg2-binary >=2.9.6"]
 
 extras_require = {
@@ -22,15 +22,15 @@
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'An integration package created by the company {COMPANY_NAME} that connects Postgres and is used to standardize connections and dependency injection in synchronous or asynchronous mode. Tested in fastapi and in console/worker scripts.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     author='Jaime Andres Cardona Carrillo',
-    author_email='tecnologiaeinformacion@logyca.com',
+    author_email='jacardona@outlook.com',
     url='https://github.com/logyca/<soon>',
     keywords="postgres, driver database",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
```

