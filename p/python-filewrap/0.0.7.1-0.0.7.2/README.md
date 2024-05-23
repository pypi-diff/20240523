# Comparing `tmp/python_filewrap-0.0.7.1.tar.gz` & `tmp/python_filewrap-0.0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_filewrap-0.0.7.1.tar", max compression
+gzip compressed data, was "python_filewrap-0.0.7.2.tar", max compression
```

## Comparing `python_filewrap-0.0.7.1.tar` & `python_filewrap-0.0.7.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.7.1/LICENSE
--rwxr-xr-x   0        0        0    16632 2024-05-22 17:10:33.789304 python_filewrap-0.0.7.1/filewrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.7.1/filewrap/py.typed
--rw-r--r--   0        0        0     1173 2024-05-22 17:11:00.216885 python_filewrap-0.0.7.1/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.7.1/readme.md
--rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 python_filewrap-0.0.7.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.7.2/LICENSE
+-rwxr-xr-x   0        0        0    16773 2024-05-23 07:26:16.047046 python_filewrap-0.0.7.2/filewrap/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.7.2/filewrap/py.typed
+-rw-r--r--   0        0        0     1173 2024-05-23 07:26:34.070148 python_filewrap-0.0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.7.2/readme.md
+-rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 python_filewrap-0.0.7.2/PKG-INFO
```

### Comparing `python_filewrap-0.0.7.1/LICENSE` & `python_filewrap-0.0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_filewrap-0.0.7.1/filewrap/__init__.py` & `python_filewrap-0.0.7.2/filewrap/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __version__ = (0, 0, 7)
 __all__ = [
-    "SupportsRead", "SupportsWrite", 
+    "SupportsRead", "SupportsWrite", "SupportsSeek", 
     "bio_chunk_iter", "bio_chunk_async_iter", 
     "bio_skip_iter", "bio_skip_async_iter", 
     "bytes_iter_skip", "bytes_async_iter_skip", 
     "bytes_iter_to_reader", "bytes_iter_to_async_reader", 
     "bytes_to_chunk_iter", "bytes_to_chunk_async_iter", 
     "bytes_ensure_part_iter", "bytes_ensure_part_async_iter", 
 ]
 
 from asyncio import to_thread, Lock as AsyncLock
-from collections.abc import Awaitable, AsyncIterable, Iterable
+from collections.abc import Awaitable, AsyncIterable, AsyncIterator, Callable, Iterable, Iterator
 from functools import update_wrapper
 from inspect import isawaitable, iscoroutinefunction
 from itertools import chain
-from collections.abc import AsyncIterator, Callable, Iterator
 from shutil import COPY_BUFSIZE # type: ignore
 from threading import Lock
 from typing import runtime_checkable, Any, Protocol, TypeVar
 
 try:
     from collections.abc import Buffer # type: ignore
 except ImportError:
@@ -33,20 +32,25 @@
 
 _T_co = TypeVar("_T_co", covariant=True)
 _T_contra = TypeVar("_T_contra", contravariant=True)
 
 
 @runtime_checkable
 class SupportsRead(Protocol[_T_co]):
-    def read(self, __length: int = ...) -> _T_co: ...
+    def read(self, /, __length: int = ...) -> _T_co: ...
 
 
 @runtime_checkable
 class SupportsWrite(Protocol[_T_contra]):
-    def write(self, __s: _T_contra) -> object: ...
+    def write(self, /, __s: _T_contra) -> object: ...
+
+
+@runtime_checkable
+class SupportsSeek(Protocol[_T_contra]):
+    def seek(self, /, __offset: int, __whence: int = 0) -> int: ...
 
 
 def bio_chunk_iter(
     bio: SupportsRead[Buffer] | Callable[[int], Buffer], 
     /, 
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
@@ -183,14 +187,15 @@
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
     callback: None | Callable[[int], Any] = None, 
 ) -> AsyncIterator[int]:
     if size == 0:
         return
     callback = ensure_async(callback) if callable(callback) else None
+    length: int
     try:
         seek = ensure_async(getattr(bio, "seek"))
         curpos = await seek(0, 1)
         if size > 0:
             length = (await seek(size, 1)) - curpos
         else:
             length = (await seek(0, 2)) - curpos
@@ -267,15 +272,15 @@
             return chain((m[size:],), it)
         else:
             size -= l
     return iter(())
 
 
 async def bytes_async_iter_skip(
-    it: Iterable[Buffer] | AsyncIterator[Buffer], 
+    it: Iterable[Buffer] | AsyncIterable[Buffer], 
     /, 
     size: int = -1, 
     callback: None | Callable[[int], Any] = None, 
 ) -> AsyncIterator[memoryview | Buffer]:
     it = aiter(ensure_aiter(it))
     if size == 0:
         return it
```

### Comparing `python_filewrap-0.0.7.1/pyproject.toml` & `python_filewrap-0.0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-filewrap"
-version = "0.0.7.1"
+version = "0.0.7.2"
 description = "Python file wrappers."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 keywords = ["file", "wrapper"]
```

### Comparing `python_filewrap-0.0.7.1/PKG-INFO` & `python_filewrap-0.0.7.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-filewrap
-Version: 0.0.7.1
+Version: 0.0.7.2
 Summary: Python file wrappers.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 License: MIT
 Keywords: file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

