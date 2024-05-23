# Comparing `tmp/logyca_postgres-0.1.2rc1.tar.gz` & `tmp/logyca_postgres-0.1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logyca_postgres-0.1.2rc1.tar", last modified: Thu May 23 16:44:17 2024, max compression
+gzip compressed data, was "logyca_postgres-0.1.2rc2.tar", last modified: Thu May 23 17:43:05 2024, max compression
```

## Comparing `logyca_postgres-0.1.2rc1.tar` & `logyca_postgres-0.1.2rc2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 16:44:17.806637 logyca_postgres-0.1.2rc1/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc1/LICENSE.txt
--rw-rw-rw-   0        0        0    15699 2024-05-23 16:44:17.806637 logyca_postgres-0.1.2rc1/PKG-INFO
--rw-rw-rw-   0        0        0    12802 2024-05-23 15:32:49.000000 logyca_postgres-0.1.2rc1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 16:44:17.729698 logyca_postgres-0.1.2rc1/logyca_postgres/
--rw-rw-rw-   0        0        0      813 2024-04-26 23:15:08.000000 logyca_postgres-0.1.2rc1/logyca_postgres/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:44:17.775214 logyca_postgres-0.1.2rc1/logyca_postgres/dependencies/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc1/logyca_postgres/dependencies/__init__.py
--rw-rw-rw-   0        0        0     9945 2024-04-26 23:13:21.000000 logyca_postgres-0.1.2rc1/logyca_postgres/dependencies/conn_postgres_async.py
--rw-rw-rw-   0        0        0     9988 2024-05-20 21:52:10.000000 logyca_postgres-0.1.2rc1/logyca_postgres/dependencies/conn_postgres_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:44:17.793060 logyca_postgres-0.1.2rc1/logyca_postgres/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc1/logyca_postgres/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:44:17.806637 logyca_postgres-0.1.2rc1/logyca_postgres/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc1/logyca_postgres/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0      228 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc1/logyca_postgres/utils/helpers/functions.py
--rw-rw-rw-   0        0        0      331 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc1/logyca_postgres/utils/helpers/singleton.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:44:17.806637 logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/
--rw-rw-rw-   0        0        0    15699 2024-05-23 16:44:17.000000 logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2024-05-23 16:44:17.000000 logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:44:17.000000 logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      445 2024-05-23 16:44:17.000000 logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 16:44:17.000000 logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 16:44:17.823099 logyca_postgres-0.1.2rc1/setup.cfg
--rw-rw-rw-   0        0        0     2580 2024-05-23 15:30:06.000000 logyca_postgres-0.1.2rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:43:05.471806 logyca_postgres-0.1.2rc2/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc2/LICENSE.txt
+-rw-rw-rw-   0        0        0    15852 2024-05-23 17:43:05.469702 logyca_postgres-0.1.2rc2/PKG-INFO
+-rw-rw-rw-   0        0        0    12919 2024-05-23 17:41:42.000000 logyca_postgres-0.1.2rc2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 17:43:05.409554 logyca_postgres-0.1.2rc2/logyca_postgres/
+-rw-rw-rw-   0        0        0      813 2024-04-26 23:15:08.000000 logyca_postgres-0.1.2rc2/logyca_postgres/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:43:05.440745 logyca_postgres-0.1.2rc2/logyca_postgres/dependencies/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc2/logyca_postgres/dependencies/__init__.py
+-rw-rw-rw-   0        0        0     9945 2024-04-26 23:13:21.000000 logyca_postgres-0.1.2rc2/logyca_postgres/dependencies/conn_postgres_async.py
+-rw-rw-rw-   0        0        0     9988 2024-05-20 21:52:10.000000 logyca_postgres-0.1.2rc2/logyca_postgres/dependencies/conn_postgres_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:43:05.440745 logyca_postgres-0.1.2rc2/logyca_postgres/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc2/logyca_postgres/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:43:05.459690 logyca_postgres-0.1.2rc2/logyca_postgres/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc2/logyca_postgres/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0      228 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc2/logyca_postgres/utils/helpers/functions.py
+-rw-rw-rw-   0        0        0      331 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc2/logyca_postgres/utils/helpers/singleton.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:43:05.462472 logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/
+-rw-rw-rw-   0        0        0    15852 2024-05-23 17:43:05.000000 logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2024-05-23 17:43:05.000000 logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:43:05.000000 logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      445 2024-05-23 17:43:05.000000 logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 17:43:05.000000 logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 17:43:05.473644 logyca_postgres-0.1.2rc2/setup.cfg
+-rw-rw-rw-   0        0        0     2616 2024-05-23 17:42:19.000000 logyca_postgres-0.1.2rc2/setup.py
```

### Comparing `logyca_postgres-0.1.2rc1/LICENSE.txt` & `logyca_postgres-0.1.2rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.2rc1/PKG-INFO` & `logyca_postgres-0.1.2rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: logyca-postgres
-Version: 0.1.2rc1
+Version: 0.1.2rc2
 Summary: An integration package created by the company LOGYCA that connects Postgres and is used to standardize connections and dependency injection in synchronous or asynchronous mode. Tested in fastapi and in console/worker scripts.
-Home-page: https://github.com/logyca/<soon>
+Home-page: https://github.com/logyca/python-libraries/tree/main/logyca-postgres
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: postgres,driver database
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -84,16 +84,17 @@
 
 ---
 
 # LOGYCA public libraries: Standard methods to connect to postgres
 
 * **Traversal libraries**: Standard methods to connect to postgres with dependency injection using yield to be used by microservices such as API(s), Workers or scripts.
 
-[Source code](https://github.com/logyca/python-libraries)
+[Source code](https://github.com/logyca/python-libraries/tree/main/logyca-postgres)
 | [Package (PyPI)](https://pypi.org/project/logyca-postgres/)
+| [Samples](https://github.com/logyca/python-libraries/tree/main/logyca-postgres/samples)
 
 ---
 
 # "pip install" dependency check
 The user must select the required libraries and versions for the project that uses this library, which validates that they are pre-installed in order to be installed.
 
 To install the libraries of the logyca postgres package verifying the SQLAlchemy prerequisite without validating connection drivers to postgres, use the following command:
```

#### html2text {}

```diff
@@ -1,81 +1,83 @@
-Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.2rc1 Summary: An
+Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.2rc2 Summary: An
 integration package created by the company LOGYCA that connects Postgres and is
 used to standardize connections and dependency injection in synchronous or
 asynchronous mode. Tested in fastapi and in console/worker scripts. Home-page:
-https://github.com/logyca/ Author: Jaime Andres Cardona Carrillo Author-email:
-jacardona@outlook.com License: MIT License Keywords: postgres,driver database
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Information Technology Classifier:
-Intended Audience :: System Administrators Classifier: License :: OSI Approved
-:: MIT License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-Classifier: Topic :: Database Classifier: Topic :: Database :: Front-Ends
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development Classifier: Typing :: Typed Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
-Dist: SQLAlchemy>=2.0.6 Requires-Dist: starlette>=0.24.0 Provides-Extra: async
-Requires-Dist: SQLAlchemy>=2.0.6; extra == "async" Requires-Dist:
-starlette>=0.24.0; extra == "async" Requires-Dist: asyncpg>=0.27.0; extra ==
-"async" Provides-Extra: sync-psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra
-== "sync-psycopg2" Requires-Dist: starlette>=0.24.0; extra == "sync-psycopg2"
-Requires-Dist: psycopg2>=2.9.6; extra == "sync-psycopg2" Provides-Extra: sync-
-psycopg2-binary Requires-Dist: SQLAlchemy>=2.0.6; extra == "sync-psycopg2-
-binary" Requires-Dist: starlette>=0.24.0; extra == "sync-psycopg2-binary"
-Requires-Dist: psycopg2-binary>=2.9.6; extra == "sync-psycopg2-binary"
-Provides-Extra: async-sync-psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra ==
-"async-sync-psycopg2" Requires-Dist: starlette>=0.24.0; extra == "async-sync-
-psycopg2" Requires-Dist: asyncpg>=0.27.0; extra == "async-sync-psycopg2"
-Requires-Dist: psycopg2>=2.9.6; extra == "async-sync-psycopg2" Provides-Extra:
-async-sync-psycopg2-binary Requires-Dist: SQLAlchemy>=2.0.6; extra == "async-
-sync-psycopg2-binary" Requires-Dist: starlette>=0.24.0; extra == "async-sync-
-psycopg2-binary" Requires-Dist: asyncpg>=0.27.0; extra == "async-sync-psycopg2-
-binary" Requires-Dist: psycopg2-binary>=2.9.6; extra == "async-sync-psycopg2-
-binary"
+https://github.com/logyca/python-libraries/tree/main/logyca-postgres Author:
+Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com License: MIT
+License Keywords: postgres,driver database Classifier: Development Status :: 4
+- Beta Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Information Technology Classifier: Intended Audience :: System
+Administrators Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python Classifier: Topic ::
+Database Classifier: Topic :: Database :: Front-Ends Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development
+Classifier: Typing :: Typed Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE.txt Requires-Dist: SQLAlchemy>=2.0.6
+Requires-Dist: starlette>=0.24.0 Provides-Extra: async Requires-Dist:
+SQLAlchemy>=2.0.6; extra == "async" Requires-Dist: starlette>=0.24.0; extra ==
+"async" Requires-Dist: asyncpg>=0.27.0; extra == "async" Provides-Extra: sync-
+psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra == "sync-psycopg2" Requires-
+Dist: starlette>=0.24.0; extra == "sync-psycopg2" Requires-Dist:
+psycopg2>=2.9.6; extra == "sync-psycopg2" Provides-Extra: sync-psycopg2-binary
+Requires-Dist: SQLAlchemy>=2.0.6; extra == "sync-psycopg2-binary" Requires-
+Dist: starlette>=0.24.0; extra == "sync-psycopg2-binary" Requires-Dist:
+psycopg2-binary>=2.9.6; extra == "sync-psycopg2-binary" Provides-Extra: async-
+sync-psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra == "async-sync-psycopg2"
+Requires-Dist: starlette>=0.24.0; extra == "async-sync-psycopg2" Requires-Dist:
+asyncpg>=0.27.0; extra == "async-sync-psycopg2" Requires-Dist: psycopg2>=2.9.6;
+extra == "async-sync-psycopg2" Provides-Extra: async-sync-psycopg2-binary
+Requires-Dist: SQLAlchemy>=2.0.6; extra == "async-sync-psycopg2-binary"
+Requires-Dist: starlette>=0.24.0; extra == "async-sync-psycopg2-binary"
+Requires-Dist: asyncpg>=0.27.0; extra == "async-sync-psycopg2-binary" Requires-
+Dist: psycopg2-binary>=2.9.6; extra == "async-sync-psycopg2-binary"
                                    _[_L_o_g_y_c_a_]
                             LLOOGGYYCCAA ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # About us * _L_O_G_Y_C_A_ _C_o_m_p_a_n_y * _L_O_G_Y_C_A_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l * _[_L_i_n_k_e_d_i_n_]*
 _[_T_w_i_t_t_e_r_]* _[_F_a_c_e_b_o_o_k_]--- # LOGYCA public libraries: Standard methods to connect
 to postgres * **Traversal libraries**: Standard methods to connect to postgres
 with dependency injection using yield to be used by microservices such as API
 (s), Workers or scripts. [Source code](https://github.com/logyca/python-
-libraries) | [Package (PyPI)](https://pypi.org/project/logyca-postgres/) --- #
-"pip install" dependency check The user must select the required libraries and
-versions for the project that uses this library, which validates that they are
-pre-installed in order to be installed. To install the libraries of the logyca
-postgres package verifying the SQLAlchemy prerequisite without validating
-connection drivers to postgres, use the following command: ```Python # Check
-SQLAlchemy dependency that is installed pip install logyca_postgres ``` To
-install the logyca postgres package libraries and validate the postgres
-asynchronous or synchronous connection driver, use the following command:
-```Python # Check asyncpg driver dependency that is installed pip install
-logyca_postgres[async] # Check psycopg2 driver dependency that is installed pip
-install logyca_postgres[sync-psycopg2] # Check psycopg2-binary driver
-dependency that is installed pip install logyca_postgres[sync-psycopg2-binary]
-# Check asyncpg+psycopg2-binary driver dependency that is installed pip install
-logyca_postgres[async-sync-psycopg2] ``` --- # Semantic Versioning logyca <
-MAJOR >.< MINOR >.< PATCH > * **MAJOR**: version when you make incompatible API
-changes * **MINOR**: version when you add functionality in a backwards
-compatible manner * **PATCH**: version when you make backwards compatible bug
-fixes ## Definitions for releasing versions * https://peps.python.org/pep-0440/
-- X.YaN (Alpha release): Identify and fix early-stage bugs. Not suitable for
-production use. - X.YbN (Beta release): Stabilize and refine features. Address
-reported bugs. Prepare for official release. - X.YrcN (Release candidate):
-Final version before official release. Assumes all major features are complete
-and stable. Recommended for testing in non-critical environments. - X.Y (Final
-release/Stable/Production): Completed, stable version ready for use in
-production. Full release for public use. --- # Example of concepts that use a
-library with a singleton pattern and connection to multiple engines with yield
-dependency injection The library uses a singleton pattern "class SyncConnEngine
+libraries/tree/main/logyca-postgres) | [Package (PyPI)](https://pypi.org/
+project/logyca-postgres/) | [Samples](https://github.com/logyca/python-
+libraries/tree/main/logyca-postgres/samples) --- # "pip install" dependency
+check The user must select the required libraries and versions for the project
+that uses this library, which validates that they are pre-installed in order to
+be installed. To install the libraries of the logyca postgres package verifying
+the SQLAlchemy prerequisite without validating connection drivers to postgres,
+use the following command: ```Python # Check SQLAlchemy dependency that is
+installed pip install logyca_postgres ``` To install the logyca postgres
+package libraries and validate the postgres asynchronous or synchronous
+connection driver, use the following command: ```Python # Check asyncpg driver
+dependency that is installed pip install logyca_postgres[async] # Check
+psycopg2 driver dependency that is installed pip install logyca_postgres[sync-
+psycopg2] # Check psycopg2-binary driver dependency that is installed pip
+install logyca_postgres[sync-psycopg2-binary] # Check asyncpg+psycopg2-binary
+driver dependency that is installed pip install logyca_postgres[async-sync-
+psycopg2] ``` --- # Semantic Versioning logyca < MAJOR >.< MINOR >.< PATCH > *
+**MAJOR**: version when you make incompatible API changes * **MINOR**: version
+when you add functionality in a backwards compatible manner * **PATCH**:
+version when you make backwards compatible bug fixes ## Definitions for
+releasing versions * https://peps.python.org/pep-0440/ - X.YaN (Alpha release):
+Identify and fix early-stage bugs. Not suitable for production use. - X.YbN
+(Beta release): Stabilize and refine features. Address reported bugs. Prepare
+for official release. - X.YrcN (Release candidate): Final version before
+official release. Assumes all major features are complete and stable.
+Recommended for testing in non-critical environments. - X.Y (Final release/
+Stable/Production): Completed, stable version ready for use in production. Full
+release for public use. --- # Example of concepts that use a library with a
+singleton pattern and connection to multiple engines with yield dependency
+injection The library uses a singleton pattern "class SyncConnEngine
 (metaclass=Singleton):", where the class is allowed to be instantiated only
 once. You can create another connection to another engine but you must create
 an inherited class in order to create a new configuration instance. Example:
 class SyncConnEngineX(SyncConnEngine): def __init__(self,
 url_connection,server_settings): super().__init__
 (url_connection,server_settings) sync_session_x=SyncConnEngineX
 ( url_connection=SyncConnEngine.build_url_connection
```

### Comparing `logyca_postgres-0.1.2rc1/README.md` & `logyca_postgres-0.1.2rc2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 
 ---
 
 # LOGYCA public libraries: Standard methods to connect to postgres
 
 * **Traversal libraries**: Standard methods to connect to postgres with dependency injection using yield to be used by microservices such as API(s), Workers or scripts.
 
-[Source code](https://github.com/logyca/python-libraries)
+[Source code](https://github.com/logyca/python-libraries/tree/main/logyca-postgres)
 | [Package (PyPI)](https://pypi.org/project/logyca-postgres/)
+| [Samples](https://github.com/logyca/python-libraries/tree/main/logyca-postgres/samples)
 
 ---
 
 # "pip install" dependency check
 The user must select the required libraries and versions for the project that uses this library, which validates that they are pre-installed in order to be installed.
 
 To install the libraries of the logyca postgres package verifying the SQLAlchemy prerequisite without validating connection drivers to postgres, use the following command:
```

#### html2text {}

```diff
@@ -2,42 +2,44 @@
                             LLOOGGYYCCAA ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # About us * _L_O_G_Y_C_A_ _C_o_m_p_a_n_y * _L_O_G_Y_C_A_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l * _[_L_i_n_k_e_d_i_n_]*
 _[_T_w_i_t_t_e_r_]* _[_F_a_c_e_b_o_o_k_]--- # LOGYCA public libraries: Standard methods to connect
 to postgres * **Traversal libraries**: Standard methods to connect to postgres
 with dependency injection using yield to be used by microservices such as API
 (s), Workers or scripts. [Source code](https://github.com/logyca/python-
-libraries) | [Package (PyPI)](https://pypi.org/project/logyca-postgres/) --- #
-"pip install" dependency check The user must select the required libraries and
-versions for the project that uses this library, which validates that they are
-pre-installed in order to be installed. To install the libraries of the logyca
-postgres package verifying the SQLAlchemy prerequisite without validating
-connection drivers to postgres, use the following command: ```Python # Check
-SQLAlchemy dependency that is installed pip install logyca_postgres ``` To
-install the logyca postgres package libraries and validate the postgres
-asynchronous or synchronous connection driver, use the following command:
-```Python # Check asyncpg driver dependency that is installed pip install
-logyca_postgres[async] # Check psycopg2 driver dependency that is installed pip
-install logyca_postgres[sync-psycopg2] # Check psycopg2-binary driver
-dependency that is installed pip install logyca_postgres[sync-psycopg2-binary]
-# Check asyncpg+psycopg2-binary driver dependency that is installed pip install
-logyca_postgres[async-sync-psycopg2] ``` --- # Semantic Versioning logyca <
-MAJOR >.< MINOR >.< PATCH > * **MAJOR**: version when you make incompatible API
-changes * **MINOR**: version when you add functionality in a backwards
-compatible manner * **PATCH**: version when you make backwards compatible bug
-fixes ## Definitions for releasing versions * https://peps.python.org/pep-0440/
-- X.YaN (Alpha release): Identify and fix early-stage bugs. Not suitable for
-production use. - X.YbN (Beta release): Stabilize and refine features. Address
-reported bugs. Prepare for official release. - X.YrcN (Release candidate):
-Final version before official release. Assumes all major features are complete
-and stable. Recommended for testing in non-critical environments. - X.Y (Final
-release/Stable/Production): Completed, stable version ready for use in
-production. Full release for public use. --- # Example of concepts that use a
-library with a singleton pattern and connection to multiple engines with yield
-dependency injection The library uses a singleton pattern "class SyncConnEngine
+libraries/tree/main/logyca-postgres) | [Package (PyPI)](https://pypi.org/
+project/logyca-postgres/) | [Samples](https://github.com/logyca/python-
+libraries/tree/main/logyca-postgres/samples) --- # "pip install" dependency
+check The user must select the required libraries and versions for the project
+that uses this library, which validates that they are pre-installed in order to
+be installed. To install the libraries of the logyca postgres package verifying
+the SQLAlchemy prerequisite without validating connection drivers to postgres,
+use the following command: ```Python # Check SQLAlchemy dependency that is
+installed pip install logyca_postgres ``` To install the logyca postgres
+package libraries and validate the postgres asynchronous or synchronous
+connection driver, use the following command: ```Python # Check asyncpg driver
+dependency that is installed pip install logyca_postgres[async] # Check
+psycopg2 driver dependency that is installed pip install logyca_postgres[sync-
+psycopg2] # Check psycopg2-binary driver dependency that is installed pip
+install logyca_postgres[sync-psycopg2-binary] # Check asyncpg+psycopg2-binary
+driver dependency that is installed pip install logyca_postgres[async-sync-
+psycopg2] ``` --- # Semantic Versioning logyca < MAJOR >.< MINOR >.< PATCH > *
+**MAJOR**: version when you make incompatible API changes * **MINOR**: version
+when you add functionality in a backwards compatible manner * **PATCH**:
+version when you make backwards compatible bug fixes ## Definitions for
+releasing versions * https://peps.python.org/pep-0440/ - X.YaN (Alpha release):
+Identify and fix early-stage bugs. Not suitable for production use. - X.YbN
+(Beta release): Stabilize and refine features. Address reported bugs. Prepare
+for official release. - X.YrcN (Release candidate): Final version before
+official release. Assumes all major features are complete and stable.
+Recommended for testing in non-critical environments. - X.Y (Final release/
+Stable/Production): Completed, stable version ready for use in production. Full
+release for public use. --- # Example of concepts that use a library with a
+singleton pattern and connection to multiple engines with yield dependency
+injection The library uses a singleton pattern "class SyncConnEngine
 (metaclass=Singleton):", where the class is allowed to be instantiated only
 once. You can create another connection to another engine but you must create
 an inherited class in order to create a new configuration instance. Example:
 class SyncConnEngineX(SyncConnEngine): def __init__(self,
 url_connection,server_settings): super().__init__
 (url_connection,server_settings) sync_session_x=SyncConnEngineX
 ( url_connection=SyncConnEngine.build_url_connection
```

### Comparing `logyca_postgres-0.1.2rc1/logyca_postgres/__init__.py` & `logyca_postgres-0.1.2rc2/logyca_postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.2rc1/logyca_postgres/dependencies/conn_postgres_async.py` & `logyca_postgres-0.1.2rc2/logyca_postgres/dependencies/conn_postgres_async.py`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.2rc1/logyca_postgres/dependencies/conn_postgres_sync.py` & `logyca_postgres-0.1.2rc2/logyca_postgres/dependencies/conn_postgres_sync.py`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/PKG-INFO` & `logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: logyca-postgres
-Version: 0.1.2rc1
+Version: 0.1.2rc2
 Summary: An integration package created by the company LOGYCA that connects Postgres and is used to standardize connections and dependency injection in synchronous or asynchronous mode. Tested in fastapi and in console/worker scripts.
-Home-page: https://github.com/logyca/<soon>
+Home-page: https://github.com/logyca/python-libraries/tree/main/logyca-postgres
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: postgres,driver database
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -84,16 +84,17 @@
 
 ---
 
 # LOGYCA public libraries: Standard methods to connect to postgres
 
 * **Traversal libraries**: Standard methods to connect to postgres with dependency injection using yield to be used by microservices such as API(s), Workers or scripts.
 
-[Source code](https://github.com/logyca/python-libraries)
+[Source code](https://github.com/logyca/python-libraries/tree/main/logyca-postgres)
 | [Package (PyPI)](https://pypi.org/project/logyca-postgres/)
+| [Samples](https://github.com/logyca/python-libraries/tree/main/logyca-postgres/samples)
 
 ---
 
 # "pip install" dependency check
 The user must select the required libraries and versions for the project that uses this library, which validates that they are pre-installed in order to be installed.
 
 To install the libraries of the logyca postgres package verifying the SQLAlchemy prerequisite without validating connection drivers to postgres, use the following command:
```

#### html2text {}

```diff
@@ -1,81 +1,83 @@
-Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.2rc1 Summary: An
+Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.2rc2 Summary: An
 integration package created by the company LOGYCA that connects Postgres and is
 used to standardize connections and dependency injection in synchronous or
 asynchronous mode. Tested in fastapi and in console/worker scripts. Home-page:
-https://github.com/logyca/ Author: Jaime Andres Cardona Carrillo Author-email:
-jacardona@outlook.com License: MIT License Keywords: postgres,driver database
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Information Technology Classifier:
-Intended Audience :: System Administrators Classifier: License :: OSI Approved
-:: MIT License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-Classifier: Topic :: Database Classifier: Topic :: Database :: Front-Ends
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development Classifier: Typing :: Typed Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
-Dist: SQLAlchemy>=2.0.6 Requires-Dist: starlette>=0.24.0 Provides-Extra: async
-Requires-Dist: SQLAlchemy>=2.0.6; extra == "async" Requires-Dist:
-starlette>=0.24.0; extra == "async" Requires-Dist: asyncpg>=0.27.0; extra ==
-"async" Provides-Extra: sync-psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra
-== "sync-psycopg2" Requires-Dist: starlette>=0.24.0; extra == "sync-psycopg2"
-Requires-Dist: psycopg2>=2.9.6; extra == "sync-psycopg2" Provides-Extra: sync-
-psycopg2-binary Requires-Dist: SQLAlchemy>=2.0.6; extra == "sync-psycopg2-
-binary" Requires-Dist: starlette>=0.24.0; extra == "sync-psycopg2-binary"
-Requires-Dist: psycopg2-binary>=2.9.6; extra == "sync-psycopg2-binary"
-Provides-Extra: async-sync-psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra ==
-"async-sync-psycopg2" Requires-Dist: starlette>=0.24.0; extra == "async-sync-
-psycopg2" Requires-Dist: asyncpg>=0.27.0; extra == "async-sync-psycopg2"
-Requires-Dist: psycopg2>=2.9.6; extra == "async-sync-psycopg2" Provides-Extra:
-async-sync-psycopg2-binary Requires-Dist: SQLAlchemy>=2.0.6; extra == "async-
-sync-psycopg2-binary" Requires-Dist: starlette>=0.24.0; extra == "async-sync-
-psycopg2-binary" Requires-Dist: asyncpg>=0.27.0; extra == "async-sync-psycopg2-
-binary" Requires-Dist: psycopg2-binary>=2.9.6; extra == "async-sync-psycopg2-
-binary"
+https://github.com/logyca/python-libraries/tree/main/logyca-postgres Author:
+Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com License: MIT
+License Keywords: postgres,driver database Classifier: Development Status :: 4
+- Beta Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Information Technology Classifier: Intended Audience :: System
+Administrators Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python Classifier: Topic ::
+Database Classifier: Topic :: Database :: Front-Ends Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development
+Classifier: Typing :: Typed Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE.txt Requires-Dist: SQLAlchemy>=2.0.6
+Requires-Dist: starlette>=0.24.0 Provides-Extra: async Requires-Dist:
+SQLAlchemy>=2.0.6; extra == "async" Requires-Dist: starlette>=0.24.0; extra ==
+"async" Requires-Dist: asyncpg>=0.27.0; extra == "async" Provides-Extra: sync-
+psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra == "sync-psycopg2" Requires-
+Dist: starlette>=0.24.0; extra == "sync-psycopg2" Requires-Dist:
+psycopg2>=2.9.6; extra == "sync-psycopg2" Provides-Extra: sync-psycopg2-binary
+Requires-Dist: SQLAlchemy>=2.0.6; extra == "sync-psycopg2-binary" Requires-
+Dist: starlette>=0.24.0; extra == "sync-psycopg2-binary" Requires-Dist:
+psycopg2-binary>=2.9.6; extra == "sync-psycopg2-binary" Provides-Extra: async-
+sync-psycopg2 Requires-Dist: SQLAlchemy>=2.0.6; extra == "async-sync-psycopg2"
+Requires-Dist: starlette>=0.24.0; extra == "async-sync-psycopg2" Requires-Dist:
+asyncpg>=0.27.0; extra == "async-sync-psycopg2" Requires-Dist: psycopg2>=2.9.6;
+extra == "async-sync-psycopg2" Provides-Extra: async-sync-psycopg2-binary
+Requires-Dist: SQLAlchemy>=2.0.6; extra == "async-sync-psycopg2-binary"
+Requires-Dist: starlette>=0.24.0; extra == "async-sync-psycopg2-binary"
+Requires-Dist: asyncpg>=0.27.0; extra == "async-sync-psycopg2-binary" Requires-
+Dist: psycopg2-binary>=2.9.6; extra == "async-sync-psycopg2-binary"
                                    _[_L_o_g_y_c_a_]
                             LLOOGGYYCCAA ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # About us * _L_O_G_Y_C_A_ _C_o_m_p_a_n_y * _L_O_G_Y_C_A_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l * _[_L_i_n_k_e_d_i_n_]*
 _[_T_w_i_t_t_e_r_]* _[_F_a_c_e_b_o_o_k_]--- # LOGYCA public libraries: Standard methods to connect
 to postgres * **Traversal libraries**: Standard methods to connect to postgres
 with dependency injection using yield to be used by microservices such as API
 (s), Workers or scripts. [Source code](https://github.com/logyca/python-
-libraries) | [Package (PyPI)](https://pypi.org/project/logyca-postgres/) --- #
-"pip install" dependency check The user must select the required libraries and
-versions for the project that uses this library, which validates that they are
-pre-installed in order to be installed. To install the libraries of the logyca
-postgres package verifying the SQLAlchemy prerequisite without validating
-connection drivers to postgres, use the following command: ```Python # Check
-SQLAlchemy dependency that is installed pip install logyca_postgres ``` To
-install the logyca postgres package libraries and validate the postgres
-asynchronous or synchronous connection driver, use the following command:
-```Python # Check asyncpg driver dependency that is installed pip install
-logyca_postgres[async] # Check psycopg2 driver dependency that is installed pip
-install logyca_postgres[sync-psycopg2] # Check psycopg2-binary driver
-dependency that is installed pip install logyca_postgres[sync-psycopg2-binary]
-# Check asyncpg+psycopg2-binary driver dependency that is installed pip install
-logyca_postgres[async-sync-psycopg2] ``` --- # Semantic Versioning logyca <
-MAJOR >.< MINOR >.< PATCH > * **MAJOR**: version when you make incompatible API
-changes * **MINOR**: version when you add functionality in a backwards
-compatible manner * **PATCH**: version when you make backwards compatible bug
-fixes ## Definitions for releasing versions * https://peps.python.org/pep-0440/
-- X.YaN (Alpha release): Identify and fix early-stage bugs. Not suitable for
-production use. - X.YbN (Beta release): Stabilize and refine features. Address
-reported bugs. Prepare for official release. - X.YrcN (Release candidate):
-Final version before official release. Assumes all major features are complete
-and stable. Recommended for testing in non-critical environments. - X.Y (Final
-release/Stable/Production): Completed, stable version ready for use in
-production. Full release for public use. --- # Example of concepts that use a
-library with a singleton pattern and connection to multiple engines with yield
-dependency injection The library uses a singleton pattern "class SyncConnEngine
+libraries/tree/main/logyca-postgres) | [Package (PyPI)](https://pypi.org/
+project/logyca-postgres/) | [Samples](https://github.com/logyca/python-
+libraries/tree/main/logyca-postgres/samples) --- # "pip install" dependency
+check The user must select the required libraries and versions for the project
+that uses this library, which validates that they are pre-installed in order to
+be installed. To install the libraries of the logyca postgres package verifying
+the SQLAlchemy prerequisite without validating connection drivers to postgres,
+use the following command: ```Python # Check SQLAlchemy dependency that is
+installed pip install logyca_postgres ``` To install the logyca postgres
+package libraries and validate the postgres asynchronous or synchronous
+connection driver, use the following command: ```Python # Check asyncpg driver
+dependency that is installed pip install logyca_postgres[async] # Check
+psycopg2 driver dependency that is installed pip install logyca_postgres[sync-
+psycopg2] # Check psycopg2-binary driver dependency that is installed pip
+install logyca_postgres[sync-psycopg2-binary] # Check asyncpg+psycopg2-binary
+driver dependency that is installed pip install logyca_postgres[async-sync-
+psycopg2] ``` --- # Semantic Versioning logyca < MAJOR >.< MINOR >.< PATCH > *
+**MAJOR**: version when you make incompatible API changes * **MINOR**: version
+when you add functionality in a backwards compatible manner * **PATCH**:
+version when you make backwards compatible bug fixes ## Definitions for
+releasing versions * https://peps.python.org/pep-0440/ - X.YaN (Alpha release):
+Identify and fix early-stage bugs. Not suitable for production use. - X.YbN
+(Beta release): Stabilize and refine features. Address reported bugs. Prepare
+for official release. - X.YrcN (Release candidate): Final version before
+official release. Assumes all major features are complete and stable.
+Recommended for testing in non-critical environments. - X.Y (Final release/
+Stable/Production): Completed, stable version ready for use in production. Full
+release for public use. --- # Example of concepts that use a library with a
+singleton pattern and connection to multiple engines with yield dependency
+injection The library uses a singleton pattern "class SyncConnEngine
 (metaclass=Singleton):", where the class is allowed to be instantiated only
 once. You can create another connection to another engine but you must create
 an inherited class in order to create a new configuration instance. Example:
 class SyncConnEngineX(SyncConnEngine): def __init__(self,
 url_connection,server_settings): super().__init__
 (url_connection,server_settings) sync_session_x=SyncConnEngineX
 ( url_connection=SyncConnEngine.build_url_connection
```

### Comparing `logyca_postgres-0.1.2rc1/logyca_postgres.egg-info/SOURCES.txt` & `logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.2rc1/setup.py` & `logyca_postgres-0.1.2rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="LOGYCA"
 PACKAGE_NAME = "logyca-postgres"
-VERSION = "0.1.2rc1"
+VERSION = "0.1.2rc2"
 
 install_requires = ["SQLAlchemy>=2.0.6","starlette>=0.24.0"]
 install_requires_asyncpg = ["asyncpg >=0.27.0"]
 install_requires_psycopg2 = ["psycopg2 >=2.9.6"]
 install_requires_psycopg2_binary = ["psycopg2-binary >=2.9.6"]
 
 extras_require = {
@@ -23,15 +23,15 @@
     version=VERSION,
     description=f'An integration package created by the company {COMPANY_NAME} that connects Postgres and is used to standardize connections and dependency injection in synchronous or asynchronous mode. Tested in fastapi and in console/worker scripts.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     author='Jaime Andres Cardona Carrillo',
     author_email='jacardona@outlook.com',
-    url='https://github.com/logyca/<soon>',
+    url='https://github.com/logyca/python-libraries/tree/main/logyca-postgres',
     keywords="postgres, driver database",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
```

