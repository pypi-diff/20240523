# Comparing `tmp/deltachat-rpc-server-1.139.4.tar.gz` & `tmp/deltachat-rpc-server-1.139.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat-rpc-server-1.139.4.tar", last modified: Tue May 21 19:12:04 2024, max compression
+gzip compressed data, was "deltachat-rpc-server-1.139.5.tar", last modified: Thu May 23 14:26:00 2024, max compression
```

## Comparing `deltachat-rpc-server-1.139.4.tar` & `deltachat-rpc-server-1.139.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.4/PKG-INFO
--rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.4/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.4/setup.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.4/src/deltachat_rpc_server/__init__.py
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.5/PKG-INFO
+-rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.5/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.5/setup.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.5/src/deltachat_rpc_server/__init__.py
```

### Comparing `deltachat-rpc-server-1.139.4/PKG-INFO` & `deltachat-rpc-server-1.139.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-server
-Version: 1.139.4
+Version: 1.139.5
 Summary: Delta Chat JSON-RPC server
 Description-Content-Type: text/markdown
 
 # Delta Chat RPC server
 
 This program provides a [JSON-RPC 2.0](https://www.jsonrpc.org/specification) interface to DeltaChat
 over standard I/O.
```

### Comparing `deltachat-rpc-server-1.139.4/setup.py` & `deltachat-rpc-server-1.139.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 "download",
                 "--no-input",
                 "--timeout",
                 "1000",
                 "--platform",
                 "musllinux_1_1_" + platform.machine(),
                 "--only-binary=:all:",
-                "deltachat-rpc-server==1.139.4",
+                "deltachat-rpc-server==1.139.5",
             ],
             cwd=tmpdir,
         )
 
         wheel_path = next(Path(tmpdir).glob("*.whl"))
         with ZipFile(wheel_path, "r") as wheel:
             exe_path = wheel.extract("deltachat_rpc_server/deltachat-rpc-server", "src")
```

