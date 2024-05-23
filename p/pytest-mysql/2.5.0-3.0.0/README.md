# Comparing `tmp/pytest-mysql-2.5.0.tar.gz` & `tmp/pytest_mysql-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-mysql-2.5.0.tar", last modified: Mon Oct 30 16:52:30 2023, max compression
+gzip compressed data, was "pytest_mysql-3.0.0.tar", last modified: Thu May 23 15:58:32 2024, max compression
```

## Comparing `pytest-mysql-2.5.0.tar` & `pytest_mysql-3.0.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:52:30.735259 pytest-mysql-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35146 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18981 2023-10-30 16:52:30.735259 pytest-mysql-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:52:30.735259 pytest-mysql-2.5.0/pytest_mysql/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/pytest_mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/pytest_mysql/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/pytest_mysql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/pytest_mysql/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/pytest_mysql/executor_noop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:52:30.735259 pytest-mysql-2.5.0/pytest_mysql/factories/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/pytest_mysql/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/pytest_mysql/factories/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/pytest_mysql/factories/noprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/pytest_mysql/factories/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/pytest_mysql/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:52:30.735259 pytest-mysql-2.5.0/pytest_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18981 2023-10-30 16:52:30.000000 pytest-mysql-2.5.0/pytest_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-10-30 16:52:30.000000 pytest-mysql-2.5.0/pytest_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 16:52:30.000000 pytest-mysql-2.5.0/pytest_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-30 16:52:30.000000 pytest-mysql-2.5.0/pytest_mysql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-30 16:52:30.000000 pytest-mysql-2.5.0/pytest_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-30 16:52:30.000000 pytest-mysql-2.5.0/pytest_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 16:52:30.000000 pytest-mysql-2.5.0/pytest_mysql.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 16:52:30.735259 pytest-mysql-2.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 16:52:30.735259 pytest-mysql-2.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/tests/test_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-10-30 16:52:18.000000 pytest-mysql-2.5.0/tests/test_mysqlnoproc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:58:32.324561 pytest_mysql-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-05-23 15:58:32.324561 pytest_mysql-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:58:32.320561 pytest_mysql-3.0.0/pytest_mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/pytest_mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/pytest_mysql/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/pytest_mysql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/pytest_mysql/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/pytest_mysql/executor_noop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:58:32.324561 pytest_mysql-3.0.0/pytest_mysql/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/pytest_mysql/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/pytest_mysql/factories/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/pytest_mysql/factories/noprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/pytest_mysql/factories/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/pytest_mysql/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/pytest_mysql/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:58:32.324561 pytest_mysql-3.0.0/pytest_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-05-23 15:58:32.000000 pytest_mysql-3.0.0/pytest_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 15:58:32.000000 pytest_mysql-3.0.0/pytest_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:58:32.000000 pytest_mysql-3.0.0/pytest_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 15:58:32.000000 pytest_mysql-3.0.0/pytest_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 15:58:32.000000 pytest_mysql-3.0.0/pytest_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 15:58:32.000000 pytest_mysql-3.0.0/pytest_mysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:58:32.000000 pytest_mysql-3.0.0/pytest_mysql.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:58:32.324561 pytest_mysql-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:58:32.324561 pytest_mysql-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/tests/test_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-23 15:58:28.000000 pytest_mysql-3.0.0/tests/test_mysqlnoproc.py
```

### Comparing `pytest-mysql-2.5.0/CHANGES.rst` & `pytest_mysql-3.0.0/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,31 @@
 CHANGELOG
 =========
 
 .. towncrier release notes start
 
+3.0.0 (2024-05-23)
+==================
+
+Breaking changes
+----------------
+
+- Replace mysqlclient with pymysql library.
+
+  Installation of mysqlclient became more and more problematic on macosx which in turn proved to be hard to maintain on github-actions.
+
+  PyMySQL is mostly API compatible so pytest-mysql usage is just changing import location with one exception for poorly documented client fixture closeup. (`#491 <https://github.com/ClearcodeHQ/pytest-mysql/issues/491>`_)
+
+
+Miscellaneus
+------------
+
+- `#481 <https://github.com/ClearcodeHQ/pytest-mysql/issues/481>`_, `#527 <https://github.com/ClearcodeHQ/pytest-mysql/issues/527>`_, `#530 <https://github.com/ClearcodeHQ/pytest-mysql/issues/530>`_
+
+
 2.5.0 (2023-10-30)
 ==================
 
 Features
 --------
 
 - Add missing user param (`#474 <https://github.com/ClearcodeHQ/pytest-mysql/issues/474>`_)
```

### Comparing `pytest-mysql-2.5.0/CONTRIBUTING.rst` & `pytest_mysql-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-mysql-2.5.0/COPYING` & `pytest_mysql-3.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `pytest-mysql-2.5.0/COPYING.lesser` & `pytest_mysql-3.0.0/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pytest-mysql-2.5.0/PKG-INFO` & `pytest_mysql-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mysql
-Version: 2.5.0
+Version: 3.0.0
 Summary: MySQL process and client fixtures for pytest
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,15 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-mysql
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-mysql/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-mysql/blob/v2.5.0/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-mysql/blob/v3.0.0/CHANGES.rst
 Keywords: tests,pytest,fixture,mysql
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -193,15 +193,15 @@
 Description-Content-Type: text/x-rst
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: AUTHORS.rst
 Requires-Dist: pytest>=6.2
 Requires-Dist: port-for>=0.6.0
 Requires-Dist: mirakuru
-Requires-Dist: mysqlclient
+Requires-Dist: pymysql
 Requires-Dist: packaging>=23
 
 .. image:: https://raw.githubusercontent.com/ClearcodeHQ/pytest-mysql/master/logo.png
     :width: 100px
     :height: 100px
     
 pytest-mysql
```

### Comparing `pytest-mysql-2.5.0/README.rst` & `pytest_mysql-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-mysql-2.5.0/pyproject.toml` & `pytest_mysql-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-mysql"
-version = "2.5.0"
+version = "3.0.0"
 description = "MySQL process and client fixtures for pytest"
 readme = "README.rst"
 keywords = ["tests", "pytest", "fixture", "mysql"]
 license = {file = "COPYING.lesser"}
 authors = [
     {name = "Grzegorz Śliwiński", email = "fizyk+pypi@fizyk.dev"}
 ]
@@ -27,23 +27,23 @@
     "Topic :: Software Development :: Testing",
     "Framework :: Pytest",
 ]
 dependencies = [
     "pytest >= 6.2",
     "port-for >= 0.6.0",
     "mirakuru",
-    "mysqlclient",
+    "pymysql",
     "packaging >= 23"
 ]
 requires-python = ">= 3.8"
 
 [project.urls]
 "Source" = "https://github.com/ClearcodeHQ/pytest-mysql"
 "Bug Tracker" = "https://github.com/ClearcodeHQ/pytest-mysql/issues"
-"Changelog" = "https://github.com/ClearcodeHQ/pytest-mysql/blob/v2.5.0/CHANGES.rst"
+"Changelog" = "https://github.com/ClearcodeHQ/pytest-mysql/blob/v3.0.0/CHANGES.rst"
 
 [project.entry-points."pytest11"]
 pytest_mysql = "pytest_mysql.plugin"
 
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
@@ -60,15 +60,15 @@
 xfail_strict=true
 addopts = "--max-worker-restart=0 --showlocals --verbose --cov"
 testpaths = "tests"
 mysql_dbname = "pytestmysql"
 
 [tool.black]
 line-length = 100
-target-version = ['py39']
+target-version = ['py38']
 include = '.*\.pyi?$'
 
 [tool.ruff]
 line-length = 100
 select = [
     "E",   # pycodestyle
     "F",   # pyflakes
@@ -99,15 +99,15 @@
 showcontent = false
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/ClearcodeHQ/pytest-dynamodb/"
 
 [tool.tbump.version]
-current = "2.5.0"
+current = "3.0.0"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `pytest-mysql-2.5.0/pytest_mysql/__init__.py` & `pytest_mysql-3.0.0/pytest_mysql/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-mysql. If not, see <http://www.gnu.org/licenses/>.
 """Main module for pytest-mysql."""
-__version__ = "2.5.0"
+__version__ = "3.0.0"
```

### Comparing `pytest-mysql-2.5.0/pytest_mysql/config.py` & `pytest_mysql-3.0.0/pytest_mysql/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Config module."""
+
 from pathlib import Path
 from typing import Any, TypedDict
 
 from pytest import FixtureRequest
 
 
 class MySQLConfigType(TypedDict):
```

### Comparing `pytest-mysql-2.5.0/pytest_mysql/exceptions.py` & `pytest_mysql-3.0.0/pytest_mysql/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest-mysql-2.5.0/pytest_mysql/executor.py` & `pytest_mysql-3.0.0/pytest_mysql/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Specified MySQL Executor."""
+
 import platform
 import re
 import subprocess
 from pathlib import Path
 from typing import Any, Literal, Optional, Union
 
 from mirakuru import TCPExecutor
```

### Comparing `pytest-mysql-2.5.0/pytest_mysql/executor_noop.py` & `pytest_mysql-3.0.0/pytest_mysql/executor_noop.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing Noop executor."""
+
 from typing import Any, Literal
 
 
 class NoopMySQLExecutor:
     """Noop Executor.
 
     Used to mimic in necessary scope the MySQL executor inside fixtures.
```

### Comparing `pytest-mysql-2.5.0/pytest_mysql/factories/client.py` & `pytest_mysql-3.0.0/pytest_mysql/factories/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,17 @@
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-mysql.  If not, see <http://www.gnu.org/licenses/>.
 """Client fixture factory for MySQL database."""
 from typing import Any, Callable, Dict, Generator, Optional, Union
 
-import MySQLdb
 import pytest
 from _pytest.fixtures import FixtureRequest
-from MySQLdb import Connection, OperationalError, ProgrammingError
+from pymysql import Connection, OperationalError, ProgrammingError
 
 from pytest_mysql.config import get_config
 from pytest_mysql.exceptions import DatabaseExists
 from pytest_mysql.executor import MySQLExecutor
 from pytest_mysql.executor_noop import NoopMySQLExecutor
 
 
@@ -53,17 +52,17 @@
     :param str collation: MySQL collation to use by default
         for *tests* database
 
     :returns: function ``mysql_fixture`` with suit scope
     :rtype: func
     """
 
-    def _connect(connect_kwargs: dict, query_str: str, mysql_db: str) -> MySQLdb.Connection:
+    def _connect(connect_kwargs: Dict[str, Any], query_str: str, mysql_db: str) -> Connection:
         """Apply given query to a  given MySQLdb connection."""
-        mysql_conn: MySQLdb.Connection = Connection(**connect_kwargs)
+        mysql_conn = Connection(**connect_kwargs)
         try:
             mysql_conn.query(query_str)
         except ProgrammingError as e:
             if "database exists" in str(e):
                 raise DatabaseExists(
                     f"Database {mysql_db} already exists. There's some test "
                     f"configuration error. Either you start your own server "
@@ -73,15 +72,15 @@
                 ) from e
             raise
         return mysql_conn
 
     @pytest.fixture
     def mysql_fixture(
         request: FixtureRequest,
-    ) -> Generator[MySQLdb.Connection, None, None]:
+    ) -> Generator[Connection, None, None]:
         """Client fixture for MySQL server.
 
         #. Get config.
         #. Try to import MySQLdb package.
         #. Connect to mysql server.
         #. Create database.
         #. Use proper database.
@@ -98,15 +97,15 @@
         if not process.running():
             process.start()
 
         mysql_user = process.user
         mysql_passwd = passwd or config["passwd"]
         mysql_db = dbname or config["dbname"]
 
-        connection_kwargs: Dict[str, Union[str, int]] = {
+        connection_kwargs: Dict[str, Any] = {
             "host": process.host,
             "user": mysql_user,
             "passwd": mysql_passwd,
         }
         if process.unixsocket:
             connection_kwargs["unix_socket"] = process.unixsocket
         else:
@@ -114,27 +113,28 @@
 
         query_str = (
             f"CREATE DATABASE `{mysql_db}` "
             f"DEFAULT CHARACTER SET {charset} "
             f"DEFAULT COLLATE {collation}"
         )
         try:
-            mysql_conn: MySQLdb.Connection = _connect(connection_kwargs, query_str, mysql_db)
+            mysql_conn: Connection = _connect(connection_kwargs, query_str, mysql_db)
         except OperationalError:
             # Fallback to mysql connection with root user
             connection_kwargs["user"] = "root"
             mysql_conn = _connect(connection_kwargs, query_str, mysql_db)
         mysql_conn.query(f"USE `{mysql_db}`")
         yield mysql_conn
 
         # clean up after test that forgot to fetch selected data
         if not mysql_conn.open:
             mysql_conn = Connection(**connection_kwargs)
         try:
-            mysql_conn.store_result()  # type: ignore
+            with mysql_conn.cursor() as cursor:
+                cursor.fetchall()
         except Exception as e:
             print(str(e))
         query_drop_database = f"DROP DATABASE IF EXISTS `{mysql_db}`"
         mysql_conn.query(query_drop_database)
-        mysql_conn.close()  # type: ignore
+        mysql_conn.close()
 
     return mysql_fixture
```

### Comparing `pytest-mysql-2.5.0/pytest_mysql/factories/noprocess.py` & `pytest_mysql-3.0.0/pytest_mysql/factories/noprocess.py`

 * *Files identical despite different names*

### Comparing `pytest-mysql-2.5.0/pytest_mysql/factories/process.py` & `pytest_mysql-3.0.0/pytest_mysql/factories/process.py`

 * *Files identical despite different names*

### Comparing `pytest-mysql-2.5.0/pytest_mysql/plugin.py` & `pytest_mysql-3.0.0/pytest_mysql/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-mysql-2.5.0/pytest_mysql.egg-info/PKG-INFO` & `pytest_mysql-3.0.0/pytest_mysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mysql
-Version: 2.5.0
+Version: 3.0.0
 Summary: MySQL process and client fixtures for pytest
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,15 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-mysql
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-mysql/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-mysql/blob/v2.5.0/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-mysql/blob/v3.0.0/CHANGES.rst
 Keywords: tests,pytest,fixture,mysql
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -193,15 +193,15 @@
 Description-Content-Type: text/x-rst
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: AUTHORS.rst
 Requires-Dist: pytest>=6.2
 Requires-Dist: port-for>=0.6.0
 Requires-Dist: mirakuru
-Requires-Dist: mysqlclient
+Requires-Dist: pymysql
 Requires-Dist: packaging>=23
 
 .. image:: https://raw.githubusercontent.com/ClearcodeHQ/pytest-mysql/master/logo.png
     :width: 100px
     :height: 100px
     
 pytest-mysql
```

### Comparing `pytest-mysql-2.5.0/pytest_mysql.egg-info/SOURCES.txt` & `pytest_mysql-3.0.0/pytest_mysql.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 pyproject.toml
 pytest_mysql/__init__.py
 pytest_mysql/config.py
 pytest_mysql/exceptions.py
 pytest_mysql/executor.py
 pytest_mysql/executor_noop.py
 pytest_mysql/plugin.py
+pytest_mysql/py.typed
 pytest_mysql.egg-info/PKG-INFO
 pytest_mysql.egg-info/SOURCES.txt
 pytest_mysql.egg-info/dependency_links.txt
 pytest_mysql.egg-info/entry_points.txt
 pytest_mysql.egg-info/requires.txt
 pytest_mysql.egg-info/top_level.txt
 pytest_mysql.egg-info/zip-safe
```

### Comparing `pytest-mysql-2.5.0/tests/test_executor.py` & `pytest_mysql-3.0.0/tests/test_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Executor tests."""
+
 from pathlib import Path
 from unittest.mock import patch
 
 import pytest
 from pytest import TempPathFactory
 
 from pytest_mysql.exceptions import MySQLUnsupported
```

### Comparing `pytest-mysql-2.5.0/tests/test_mysql.py` & `pytest_mysql-3.0.0/tests/test_mysql.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Actual tests for pytest-mysql."""
-from MySQLdb import Connection
+
+from pymysql import Connection
 
 from pytest_mysql.executor import MySQLExecutor
 
 QUERY = """CREATE TABLE pet (name VARCHAR(20), owner VARCHAR(20),
     species VARCHAR(20), sex CHAR(1), birth DATE, death DATE);"""
 
 
@@ -12,33 +13,33 @@
     assert mysql_proc.running()
 
 
 def test_mysql(mysql: Connection) -> None:
     """Check first, basic client fixture factory."""
     cursor = mysql.cursor()
     cursor.execute(QUERY)
-    mysql.commit()  # type: ignore
+    mysql.commit()
     cursor.close()
 
 
 def test_mysql_test_without_cursor(mysql: Connection) -> None:
     """Run test without cursor and without fetching the data."""
     mysql.query("SELECT VERSION();")
 
 
 def test_mysql_newfixture(mysql: Connection, mysql2: Connection) -> None:
     """More complext test with several mysql_processes."""
     cursor = mysql.cursor()
     cursor.execute(QUERY)
-    mysql.commit()  # type: ignore
+    mysql.commit()
     cursor.close()
 
     cursor = mysql2.cursor()
     cursor.execute(QUERY)
-    mysql2.commit()  # type: ignore
+    mysql2.commit()
     cursor.close()
 
 
 def test_random_port(mysql_rand: Connection) -> None:
     """Test if mysql fixture can be started on random port."""
     mysql = mysql_rand
     mysql.cursor()
```

### Comparing `pytest-mysql-2.5.0/tests/test_mysqlnoproc.py` & `pytest_mysql-3.0.0/tests/test_mysqlnoproc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """MySQL tests that do not start mysql server."""
-from MySQLdb import Connection
+
+from pymysql import Connection
 
 from pytest_mysql import factories
 from tests.test_mysql import QUERY
 
 mysql_noproc2 = factories.mysql_noproc()
 mysqlnoproc_client = factories.mysql("mysql_noproc2")
 
 
 def test_mysql_noproc(mysqlnoproc_client: Connection) -> None:
     """Check if noproc fixture connects to the running mysql instance."""
     cursor = mysqlnoproc_client.cursor()
     cursor.execute(QUERY)
-    mysqlnoproc_client.commit()  # type: ignore
+    mysqlnoproc_client.commit()
     cursor.close()
 
 
 def test_mysql_noproc_closing_connection_not_throwing_exception(
     mysqlnoproc_client: Connection,
 ) -> None:
     """Check if closing the connection doesn't throw an exception.
 
     When cleaning the fixture.
     """
     cursor = mysqlnoproc_client.cursor()
     cursor.execute(QUERY)
-    mysqlnoproc_client.commit()  # type: ignore
+    mysqlnoproc_client.commit()
     cursor.close()
-    mysqlnoproc_client.close()  # type: ignore
+    mysqlnoproc_client.close()
```

