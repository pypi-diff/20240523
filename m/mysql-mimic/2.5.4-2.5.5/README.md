# Comparing `tmp/mysql-mimic-2.5.4.tar.gz` & `tmp/mysql-mimic-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-mimic-2.5.4.tar", last modified: Tue Mar 19 21:40:24 2024, max compression
+gzip compressed data, was "mysql-mimic-2.5.5.tar", last modified: Thu May 23 19:42:14 2024, max compression
```

## Comparing `mysql-mimic-2.5.4.tar` & `mysql-mimic-2.5.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 21:40:24.347860 mysql-mimic-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-03-19 21:40:24.347860 mysql-mimic-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 21:40:24.347860 mysql-mimic-2.5.4/mysql_mimic/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/charset.py
--rw-r--r--   0 runner    (1001) docker     (127)    24575 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/intercept.py
--rw-r--r--   0 runner    (1001) docker     (127)    19310 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/packets.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/prepared.py
--rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    20500 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/mysql_mimic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 21:40:24.347860 mysql-mimic-2.5.4/mysql_mimic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-03-19 21:40:24.000000 mysql-mimic-2.5.4/mysql_mimic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-19 21:40:24.000000 mysql-mimic-2.5.4/mysql_mimic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 21:40:24.000000 mysql-mimic-2.5.4/mysql_mimic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-19 21:40:24.000000 mysql-mimic-2.5.4/mysql_mimic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-19 21:40:24.000000 mysql-mimic-2.5.4/mysql_mimic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 21:40:24.347860 mysql-mimic-2.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 21:40:24.347860 mysql-mimic-2.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    30562 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/tests/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-19 21:40:03.000000 mysql-mimic-2.5.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:42:14.670972 mysql-mimic-2.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-23 19:42:14.670972 mysql-mimic-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:42:14.666972 mysql-mimic-2.5.5/mysql_mimic/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/charset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24575 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/intercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19430 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/packets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/prepared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20500 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/mysql_mimic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:42:14.666972 mysql-mimic-2.5.5/mysql_mimic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-23 19:42:14.000000 mysql-mimic-2.5.5/mysql_mimic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-23 19:42:14.000000 mysql-mimic-2.5.5/mysql_mimic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:42:14.000000 mysql-mimic-2.5.5/mysql_mimic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-23 19:42:14.000000 mysql-mimic-2.5.5/mysql_mimic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 19:42:14.000000 mysql-mimic-2.5.5/mysql_mimic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:42:14.670972 mysql-mimic-2.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:42:14.670972 mysql-mimic-2.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30562 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/tests/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-23 19:41:52.000000 mysql-mimic-2.5.5/tests/test_version.py
```

### Comparing `mysql-mimic-2.5.4/LICENSE` & `mysql-mimic-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/PKG-INFO` & `mysql-mimic-2.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.5.4
+Version: 2.5.5
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.5.4/README.md` & `mysql-mimic-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/auth.py` & `mysql-mimic-2.5.5/mysql_mimic/auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/charset.py` & `mysql-mimic-2.5.5/mysql_mimic/charset.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/connection.py` & `mysql-mimic-2.5.5/mysql_mimic/connection.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/constants.py` & `mysql-mimic-2.5.5/mysql_mimic/constants.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/control.py` & `mysql-mimic-2.5.5/mysql_mimic/control.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/errors.py` & `mysql-mimic-2.5.5/mysql_mimic/errors.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/intercept.py` & `mysql-mimic-2.5.5/mysql_mimic/intercept.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/packets.py` & `mysql-mimic-2.5.5/mysql_mimic/packets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import io
 from dataclasses import dataclass, field
 from typing import Optional, Dict, Any, Sequence, Callable, Tuple, List, Union
 
 from mysql_mimic.charset import Collation, CharacterSet
+from mysql_mimic.constants import DEFAULT_SERVER_CAPABILITIES
 from mysql_mimic.errors import ErrorCode, get_sqlstate, MysqlError
 from mysql_mimic.prepared import PreparedStatement, REGEX_PARAM
 from mysql_mimic.results import NullBitmap, ResultColumn
 from mysql_mimic.types import (
     Capabilities,
     uint_2,
     uint_1,
@@ -149,17 +150,17 @@
         parts.append(uint_2(warnings))
         parts.append(uint_2(status_flags | flags))
 
     return _concat(*parts)
 
 
 def make_error(
-    capabilities: Capabilities,
-    server_charset: CharacterSet,
-    msg: Any,
+    capabilities: Capabilities = DEFAULT_SERVER_CAPABILITIES,
+    server_charset: CharacterSet = CharacterSet.utf8mb4,
+    msg: Any = "",
     code: ErrorCode = ErrorCode.UNKNOWN_ERROR,
 ) -> bytes:
     parts = [uint_1(0xFF), uint_2(code)]
 
     if Capabilities.CLIENT_PROTOCOL_41 in capabilities:
         parts.append(str_fixed(1, b"#"))
         parts.append(str_fixed(5, get_sqlstate(code)))
```

### Comparing `mysql-mimic-2.5.4/mysql_mimic/results.py` & `mysql-mimic-2.5.5/mysql_mimic/results.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/schema.py` & `mysql-mimic-2.5.5/mysql_mimic/schema.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/server.py` & `mysql-mimic-2.5.5/mysql_mimic/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from __future__ import annotations
 
 import asyncio
 import inspect
+import logging
 from ssl import SSLContext
 from socket import socket
 from typing import Callable, Any, Optional, Sequence, Awaitable
 
+from mysql_mimic import packets
 from mysql_mimic.auth import IdentityProvider, SimpleIdentityProvider
 from mysql_mimic.connection import Connection
 from mysql_mimic.control import Control, LocalControl, TooManyConnections
 from mysql_mimic.errors import ErrorCode
 from mysql_mimic.session import Session, BaseSession
 from mysql_mimic.constants import DEFAULT_SERVER_CAPABILITIES
 from mysql_mimic.stream import MysqlStream
 from mysql_mimic.types import Capabilities
 
 
+logger = logging.getLogger(__name__)
+
+
 class MaxConnectionsExceeded(Exception):
     pass
 
 
 class MysqlServer:
     """
     MySQL mimic server.
@@ -54,39 +59,53 @@
         self._server: Optional[asyncio.base_events.Server] = None
 
     async def _client_connected_cb(
         self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter
     ) -> None:
         stream = MysqlStream(reader, writer)
 
-        if inspect.iscoroutinefunction(self.session_factory):
-            session = await self.session_factory()
-        else:
-            session = self.session_factory()
-
-        connection = Connection(
-            stream=stream,
-            session=session,
-            control=self.control,
-            server_capabilities=self.capabilities,
-            identity_provider=self.identity_provider,
-            ssl=self.ssl,
-        )
+        try:
+            if inspect.iscoroutinefunction(self.session_factory):
+                session = await self.session_factory()
+            else:
+                session = self.session_factory()
+
+            connection = Connection(
+                stream=stream,
+                session=session,
+                control=self.control,
+                server_capabilities=self.capabilities,
+                identity_provider=self.identity_provider,
+                ssl=self.ssl,
+            )
+
+        except Exception:  # pylint: disable=broad-except
+            logger.exception("Failed to create connection")
+            await stream.write(
+                # Return an error so clients don't freeze
+                packets.make_error(capabilities=self.capabilities)
+            )
+            return
 
         try:
             connection_id = await self.control.add(connection)
+            connection.connection_id = connection_id
         except TooManyConnections:
             await stream.write(
                 connection.error(
                     msg="Too many connections",
                     code=ErrorCode.CON_COUNT_ERROR,
                 )
             )
             return
-        connection.connection_id = connection_id
+        except Exception:  # pylint: disable=broad-except
+            logger.exception("Failed to register connection")
+            await stream.write(connection.error(msg="Failed to register connection"))
+            return
+
         try:
             return await connection.start()
         finally:
             writer.close()
             await self.control.remove(connection_id)
 
     async def start_server(self, **kwargs: Any) -> None:
```

### Comparing `mysql-mimic-2.5.4/mysql_mimic/session.py` & `mysql-mimic-2.5.5/mysql_mimic/session.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/stream.py` & `mysql-mimic-2.5.5/mysql_mimic/stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/types.py` & `mysql-mimic-2.5.5/mysql_mimic/types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/utils.py` & `mysql-mimic-2.5.5/mysql_mimic/utils.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic/variables.py` & `mysql-mimic-2.5.5/mysql_mimic/variables.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/mysql_mimic.egg-info/PKG-INFO` & `mysql-mimic-2.5.5/mysql_mimic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.5.4
+Version: 2.5.5
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.5.4/mysql_mimic.egg-info/SOURCES.txt` & `mysql-mimic-2.5.5/mysql_mimic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/setup.py` & `mysql-mimic-2.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/tests/test_auth.py` & `mysql-mimic-2.5.5/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/tests/test_control.py` & `mysql-mimic-2.5.5/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/tests/test_query.py` & `mysql-mimic-2.5.5/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/tests/test_result.py` & `mysql-mimic-2.5.5/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/tests/test_ssl.py` & `mysql-mimic-2.5.5/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/tests/test_stream.py` & `mysql-mimic-2.5.5/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/tests/test_types.py` & `mysql-mimic-2.5.5/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.5.4/tests/test_variables.py` & `mysql-mimic-2.5.5/tests/test_variables.py`

 * *Files identical despite different names*

