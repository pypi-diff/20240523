# Comparing `tmp/didcomm_messaging-0.1.1a2.tar.gz` & `tmp/didcomm_messaging-0.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "didcomm_messaging-0.1.1a2.tar", last modified: Mon May 13 15:10:00 2024, max compression
+gzip compressed data, was "didcomm_messaging-0.1.1a3.tar", last modified: Thu May 23 16:31:21 2024, max compression
```

## Comparing `didcomm_messaging-0.1.1a2.tar` & `didcomm_messaging-0.1.1a3.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0    11357 2024-05-13 15:09:42.311867 didcomm_messaging-0.1.1a2/LICENSE
--rw-r--r--   0        0        0     3592 2024-05-13 15:09:42.311867 didcomm_messaging-0.1.1a2/README.md
--rw-r--r--   0        0        0     4855 2024-05-13 15:09:42.311867 didcomm_messaging-0.1.1a2/didcomm_messaging/__init__.py
--rw-r--r--   0        0        0      221 2024-05-13 15:09:42.311867 didcomm_messaging-0.1.1a2/didcomm_messaging/crypto/__init__.py
--rw-r--r--   0        0        0       52 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/crypto/backend/__init__.py
--rw-r--r--   0        0        0    13927 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/crypto/backend/askar.py
--rw-r--r--   0        0        0     7510 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/crypto/backend/authlib.py
--rw-r--r--   0        0        0      646 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/crypto/backend/basic.py
--rw-r--r--   0        0        0     4084 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/crypto/base.py
--rw-r--r--   0        0        0    15121 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/crypto/jwe.py
--rw-r--r--   0        0        0       42 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/multiformats/__init__.py
--rw-r--r--   0        0        0     3880 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/multiformats/multibase.py
--rw-r--r--   0        0        0     2264 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/multiformats/multicodec.py
--rw-r--r--   0        0        0     6742 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/packaging.py
--rw-r--r--   0        0        0    18352 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/quickstart.py
--rw-r--r--   0        0        0     2487 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/resolver/__init__.py
--rw-r--r--   0        0        0     1227 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/resolver/peer.py
--rw-r--r--   0        0        0     3811 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/resolver/web.py
--rw-r--r--   0        0        0     5947 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/didcomm_messaging/routing.py
--rw-r--r--   0        0        0     1590 2024-05-13 15:10:00.804160 didcomm_messaging-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/tests/__init__.py
--rw-r--r--   0        0        0      678 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/tests/crypto/__init__.py
--rw-r--r--   0        0        0     6607 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/tests/crypto/test_askar.py
--rw-r--r--   0        0        0     3166 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/tests/crypto/test_askar_x_authlib.py
--rw-r--r--   0        0        0     2124 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/tests/crypto/test_authlib.py
--rw-r--r--   0        0        0      740 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/tests/test_didresolver.py
--rw-r--r--   0        0        0     2787 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/tests/test_didweb.py
--rw-r--r--   0        0        0     2197 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/tests/test_packaging.py
--rw-r--r--   0        0        0      771 2024-05-13 15:09:42.315867 didcomm_messaging-0.1.1a2/tests/test_secrets.py
--rw-r--r--   0        0        0     4314 1970-01-01 00:00:00.000000 didcomm_messaging-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 16:31:01.585173 didcomm_messaging-0.1.1a3/LICENSE
+-rw-r--r--   0        0        0     3592 2024-05-23 16:31:01.585173 didcomm_messaging-0.1.1a3/README.md
+-rw-r--r--   0        0        0     4855 2024-05-23 16:31:01.585173 didcomm_messaging-0.1.1a3/didcomm_messaging/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-23 16:31:01.585173 didcomm_messaging-0.1.1a3/didcomm_messaging/crypto/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-23 16:31:01.585173 didcomm_messaging-0.1.1a3/didcomm_messaging/crypto/backend/__init__.py
+-rw-r--r--   0        0        0    13927 2024-05-23 16:31:01.585173 didcomm_messaging-0.1.1a3/didcomm_messaging/crypto/backend/askar.py
+-rw-r--r--   0        0        0     7510 2024-05-23 16:31:01.585173 didcomm_messaging-0.1.1a3/didcomm_messaging/crypto/backend/authlib.py
+-rw-r--r--   0        0        0      646 2024-05-23 16:31:01.585173 didcomm_messaging-0.1.1a3/didcomm_messaging/crypto/backend/basic.py
+-rw-r--r--   0        0        0     4084 2024-05-23 16:31:01.585173 didcomm_messaging-0.1.1a3/didcomm_messaging/crypto/base.py
+-rw-r--r--   0        0        0    15121 2024-05-23 16:31:01.585173 didcomm_messaging-0.1.1a3/didcomm_messaging/crypto/jwe.py
+-rw-r--r--   0        0        0    17909 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/didcomm_messaging/legacy/crypto.py
+-rw-r--r--   0        0        0       42 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/didcomm_messaging/multiformats/__init__.py
+-rw-r--r--   0        0        0     3880 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/didcomm_messaging/multiformats/multibase.py
+-rw-r--r--   0        0        0     2264 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/didcomm_messaging/multiformats/multicodec.py
+-rw-r--r--   0        0        0     6742 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/didcomm_messaging/packaging.py
+-rw-r--r--   0        0        0    18352 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/didcomm_messaging/quickstart.py
+-rw-r--r--   0        0        0     2487 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/didcomm_messaging/resolver/__init__.py
+-rw-r--r--   0        0        0     1227 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/didcomm_messaging/resolver/peer.py
+-rw-r--r--   0        0        0     3811 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/didcomm_messaging/resolver/web.py
+-rw-r--r--   0        0        0     5947 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/didcomm_messaging/routing.py
+-rw-r--r--   0        0        0     1646 2024-05-23 16:31:21.981185 didcomm_messaging-0.1.1a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/tests/__init__.py
+-rw-r--r--   0        0        0      678 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/tests/crypto/__init__.py
+-rw-r--r--   0        0        0     6607 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/tests/crypto/test_askar.py
+-rw-r--r--   0        0        0     3166 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/tests/crypto/test_askar_x_authlib.py
+-rw-r--r--   0        0        0     2124 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/tests/crypto/test_authlib.py
+-rw-r--r--   0        0        0      740 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/tests/test_didresolver.py
+-rw-r--r--   0        0        0     2787 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/tests/test_didweb.py
+-rw-r--r--   0        0        0     1324 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/tests/test_legacy.py
+-rw-r--r--   0        0        0     2197 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/tests/test_packaging.py
+-rw-r--r--   0        0        0      771 2024-05-23 16:31:01.589173 didcomm_messaging-0.1.1a3/tests/test_secrets.py
+-rw-r--r--   0        0        0     4434 1970-01-01 00:00:00.000000 didcomm_messaging-0.1.1a3/PKG-INFO
```

### Comparing `didcomm_messaging-0.1.1a2/LICENSE` & `didcomm_messaging-0.1.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/README.md` & `didcomm_messaging-0.1.1a3/README.md`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/__init__.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/crypto/backend/askar.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/crypto/backend/askar.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/crypto/backend/authlib.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/crypto/backend/authlib.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/crypto/backend/basic.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/crypto/backend/basic.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/crypto/base.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/crypto/base.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/crypto/jwe.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/crypto/jwe.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/multiformats/multibase.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/multiformats/multibase.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/multiformats/multicodec.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/multiformats/multicodec.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/packaging.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/packaging.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/quickstart.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/quickstart.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/resolver/__init__.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/resolver/peer.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/resolver/peer.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/resolver/web.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/resolver/web.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/didcomm_messaging/routing.py` & `didcomm_messaging-0.1.1a3/didcomm_messaging/routing.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/pyproject.toml` & `didcomm_messaging-0.1.1a3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "didcomm-messaging"
-version = "0.1.1a2"
+version = "0.1.1a3"
 description = "DIDComm Messaging implemented with swappable backends."
 authors = [
     { name = "Daniel Bluhm", email = "dbluhm@pm.me" },
     { name = "Colton Wolkins", email = "colton@indicio.tech" },
     { name = "Micah Peltier", email = "micah@indicio.tech" },
 ]
 dependencies = [
@@ -25,14 +25,18 @@
     "did-peer-2>=0.1.2",
     "did-peer-4>=0.1.2",
 ]
 authlib = [
     "authlib>=1.2.1",
     "pycryptodomex>=3.19.0",
 ]
+legacy = [
+    "msgpack>=1.0.8",
+    "PyNaCl>=1.5.0",
+]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `didcomm_messaging-0.1.1a2/tests/conftest.py` & `didcomm_messaging-0.1.1a3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/tests/crypto/test_askar.py` & `didcomm_messaging-0.1.1a3/tests/crypto/test_askar.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/tests/crypto/test_askar_x_authlib.py` & `didcomm_messaging-0.1.1a3/tests/crypto/test_askar_x_authlib.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/tests/crypto/test_authlib.py` & `didcomm_messaging-0.1.1a3/tests/crypto/test_authlib.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/tests/test_didresolver.py` & `didcomm_messaging-0.1.1a3/tests/test_didresolver.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/tests/test_didweb.py` & `didcomm_messaging-0.1.1a3/tests/test_didweb.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/tests/test_packaging.py` & `didcomm_messaging-0.1.1a3/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/tests/test_secrets.py` & `didcomm_messaging-0.1.1a3/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `didcomm_messaging-0.1.1a2/PKG-INFO` & `didcomm_messaging-0.1.1a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: didcomm-messaging
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: DIDComm Messaging implemented with swappable backends.
 Author-Email: Daniel Bluhm <dbluhm@pm.me>, Colton Wolkins <colton@indicio.tech>, Micah Peltier <micah@indicio.tech>
 License: Apache-2.0
 Requires-Python: >=3.9
 Requires-Dist: base58>=2.1.1
 Requires-Dist: pydid>=0.4.2
 Requires-Dist: aries-askar>=0.2.9; extra == "askar"
 Requires-Dist: did-peer-2>=0.1.2; extra == "did-peer"
 Requires-Dist: did-peer-4>=0.1.2; extra == "did-peer"
 Requires-Dist: authlib>=1.2.1; extra == "authlib"
 Requires-Dist: pycryptodomex>=3.19.0; extra == "authlib"
+Requires-Dist: msgpack>=1.0.8; extra == "legacy"
+Requires-Dist: PyNaCl>=1.5.0; extra == "legacy"
 Provides-Extra: askar
 Provides-Extra: did-peer
 Provides-Extra: authlib
+Provides-Extra: legacy
 Description-Content-Type: text/markdown
 
 # didcomm-messaging-python
 
 This is a minimal but flexible implementation of [DIDComm Messaging](https://identity.foundation/didcomm-messaging/spec/v2.1/). To learn more about DIDComm Messaging, check out the spec or visit [didcomm.org](https://didcomm.org) to learn about DIDComm Messaging protocols defined by the community.
 
 ## Usage
```

