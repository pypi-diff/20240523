# Comparing `tmp/sqla_async_orm_queries-1.1.2.tar.gz` & `tmp/sqla_async_orm_queries-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqla_async_orm_queries-1.1.2.tar", max compression
+gzip compressed data, was "sqla_async_orm_queries-1.1.3.tar", max compression
```

## Comparing `sqla_async_orm_queries-1.1.2.tar` & `sqla_async_orm_queries-1.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2024-03-15 13:29:12.038827 sqla_async_orm_queries-1.1.2/LICENCE.md
--rw-r--r--   0        0        0     2610 2024-03-15 13:29:12.038827 sqla_async_orm_queries-1.1.2/README.md
--rw-r--r--   0        0        0      889 2024-03-15 13:29:23.078837 sqla_async_orm_queries-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       72 2024-03-15 13:29:12.038827 sqla_async_orm_queries-1.1.2/sqla_async_orm_queries/__init__.py
--rw-r--r--   0        0        0     5379 2024-03-15 13:29:12.038827 sqla_async_orm_queries-1.1.2/sqla_async_orm_queries/models.py
--rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 sqla_async_orm_queries-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-23 06:58:20.502152 sqla_async_orm_queries-1.1.3/LICENCE.md
+-rw-r--r--   0        0        0     2610 2024-05-23 06:58:20.502152 sqla_async_orm_queries-1.1.3/README.md
+-rw-r--r--   0        0        0      909 2024-05-23 06:58:31.326200 sqla_async_orm_queries-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-05-23 06:58:20.506152 sqla_async_orm_queries-1.1.3/sqla_async_orm_queries/__init__.py
+-rw-r--r--   0        0        0     6892 2024-05-23 06:58:20.506152 sqla_async_orm_queries-1.1.3/sqla_async_orm_queries/models.py
+-rw-r--r--   0        0        0     3709 1970-01-01 00:00:00.000000 sqla_async_orm_queries-1.1.3/PKG-INFO
```

### Comparing `sqla_async_orm_queries-1.1.2/LICENCE.md` & `sqla_async_orm_queries-1.1.3/LICENCE.md`

 * *Files identical despite different names*

### Comparing `sqla_async_orm_queries-1.1.2/README.md` & `sqla_async_orm_queries-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sqla_async_orm_queries-1.1.2/pyproject.toml` & `sqla_async_orm_queries-1.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqla-async-orm-queries"
-version = "v1.1.2"
+version = "v1.1.3"
 description = "Base model for SqlAlchemy async orm queries"
 authors = ["Amrah <bagirovemrah97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/amrahhh/sqla_async_orm_queries"
 repository = "https://github.com/amrahhh/sqla_async_orm_queries"
 classifiers = [
@@ -20,7 +20,8 @@
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.2"
 sqlalchemy = ">=2.0.21"
 asyncpg = ">=0.28.0"
+greenlet = "^3.0.3"
```

### Comparing `sqla_async_orm_queries-1.1.2/PKG-INFO` & `sqla_async_orm_queries-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqla-async-orm-queries
-Version: 1.1.2
+Version: 1.1.3
 Summary: Base model for SqlAlchemy async orm queries
 Home-page: https://github.com/amrahhh/sqla_async_orm_queries
 License: MIT
 Author: Amrah
 Author-email: bagirovemrah97@gmail.com
 Requires-Python: >=3.8.2,<4.0.0
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: asyncpg (>=0.28.0)
+Requires-Dist: greenlet (>=3.0.3,<4.0.0)
 Requires-Dist: sqlalchemy (>=2.0.21)
 Project-URL: Repository, https://github.com/amrahhh/sqla_async_orm_queries
 Description-Content-Type: text/markdown
 
 # SQLAlchemy Async ORM Queries
 This is a simple implementation of an asynchronous ORM (Object-Relational Mapping) with SQLAlchemy, designed to work with asynchronous operations in Python. The code provided here demonstrates basic CRUD (Create, Read, Update, Delete) operations using SQLAlchemy's async features.
```

