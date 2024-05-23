# Comparing `tmp/types-requests-2.31.0.9.tar.gz` & `tmp/types-requests-2.32.0.20240521.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-requests-2.31.0.9.tar", last modified: Fri Oct 13 18:19:28 2023, max compression
+gzip compressed data, was "types-requests-2.32.0.20240521.tar", last modified: Tue May 21 02:21:30 2024, max compression
```

## Comparing `types-requests-2.31.0.9.tar` & `types-requests-2.32.0.20240521.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 18:19:28.737563 types-requests-2.31.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    13218 2023-10-13 18:19:26.000000 types-requests-2.31.0.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-13 18:19:26.000000 types-requests-2.31.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-10-13 18:19:28.737563 types-requests-2.31.0.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 18:19:28.737563 types-requests-2.31.0.9/requests-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-10-13 18:19:26.000000 types-requests-2.31.0.9/requests-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/__version__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/adapters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/certs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/help.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/hooks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/packages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/sessions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/status_codes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/structures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-13 18:19:28.737563 types-requests-2.31.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2023-10-13 18:19:26.000000 types-requests-2.31.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 18:19:28.737563 types-requests-2.31.0.9/types_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-10-13 18:19:28.000000 types-requests-2.31.0.9/types_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-10-13 18:19:28.000000 types-requests-2.31.0.9/types_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 18:19:28.000000 types-requests-2.31.0.9/types_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-13 18:19:28.000000 types-requests-2.31.0.9/types_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-13 18:19:28.000000 types-requests-2.31.0.9/types_requests.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:21:30.511952 types-requests-2.32.0.20240521/
+-rw-r--r--   0 runner    (1001) docker     (127)    15650 2024-05-21 02:21:27.000000 types-requests-2.32.0.20240521/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 02:21:27.000000 types-requests-2.32.0.20240521/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-21 02:21:30.511952 types-requests-2.32.0.20240521/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:21:30.511952 types-requests-2.32.0.20240521/requests-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-21 02:21:27.000000 types-requests-2.32.0.20240521/requests-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/__version__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/adapters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/certs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/help.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/hooks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/packages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:21:27.000000 types-requests-2.32.0.20240521/requests-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/sessions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/status_codes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/structures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-21 02:21:15.000000 types-requests-2.32.0.20240521/requests-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 02:21:30.511952 types-requests-2.32.0.20240521/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-21 02:21:27.000000 types-requests-2.32.0.20240521/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:21:30.511952 types-requests-2.32.0.20240521/types_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-21 02:21:30.000000 types-requests-2.32.0.20240521/types_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-21 02:21:30.000000 types-requests-2.32.0.20240521/types_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 02:21:30.000000 types-requests-2.32.0.20240521/types_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 02:21:30.000000 types-requests-2.32.0.20240521/types_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 02:21:30.000000 types-requests-2.32.0.20240521/types_requests.egg-info/top_level.txt
```

### Comparing `types-requests-2.31.0.9/CHANGELOG.md` & `types-requests-2.32.0.20240521/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,82 @@
+## 2.32.0.20240521 (2024-05-21)
+
+[stubsabot] Bump requests to 2.32.* (#11991)
+
+Release: https://pypi.org/pypi/requests/2.32.1
+Homepage: https://requests.readthedocs.io
+Repository: https://github.com/psf/requests
+Typeshed stubs: https://github.com/python/typeshed/tree/main/stubs/requests
+Diff: https://github.com/psf/requests/compare/v2.31.0...v2.32.1
+
+Stubsabot analysis of the diff between the two releases:
+ - Total lines of Python code added: 486.
+ - Total lines of Python code deleted: 131.
+
+## 2.31.0.20240406 (2024-04-06)
+
+requests: export `packages` and `utils` (#11723)
+
+## 2.31.0.20240403 (2024-04-03)
+
+requests: remove a `type: ignore` (#11704)
+
+## 2.31.0.20240402 (2024-04-02)
+
+requests: annotate RequestsCookieJar (#11656)
+
+## 2.31.0.20240311 (2024-03-11)
+
+Use PEP 570 syntax in third party stubs (#11554)
+
+## 2.31.0.20240310 (2024-03-10)
+
+Bump mypy to 1.9, add to json.encoder, small fixups (#11549)
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
+## 2.31.0.20240218 (2024-02-18)
+
+requests: Allow passing None header values (#11370)
+
+https://github.com/python/typeshed/pull/7773 changed
+`requests.session.Session` methods to accept None for header values, but
+didn't do quite the same for the functions in `requests.api`.  I think
+this was a mistake.  The functions in `requests.api` just pass through
+the `headers` argument without doing anything in particular to it.
+
+Furthermore, it's useful to be able to pass None as a header value:
+because `requests.utils.default_headers` sets an `Accept-Encoding`
+header by default, the easiest way to send a request with no
+`Accept-Encoding` header is something like `requests.get(url,
+headers={"Accept-Encoding": None})`.  It's annoying to have to construct
+a `Session` just to pass type-checking.
+
+It's a little confusing for the type alias to be called
+`_HeadersUpdateMapping` in `requests.sessions` but `_HeadersMapping` in
+`requests.api`; this is because the latter name was already used in
+other type stubs (`tensorflow.keras.callbacks`), so it seemed best to
+avoid breaking API.
+
+## 2.31.0.20240125 (2024-01-25)
+
+Add parameter type to PreparedRequest.prepare_content_length (#11304)
+
+## 2.31.0.20240106 (2024-01-06)
+
+Update typing_extensions imports in third-party stubs (#11245)
+
+## 2.31.0.20231231 (2023-12-31)
+
+requests: Use the `Any` trick in `HTTPError` (#11207)
+
+## 2.31.0.10 (2023-10-18)
+
+requests: annotate `utils.get_encoding_from_headers()` (#10901)
+
 ## 2.31.0.9 (2023-10-13)
 
 [requests] Allow HTTPError.response to be None (#10875)
 
 This aligns with the definition in requests, but means that user code might
 need additional assertions to ensure that `HTTPError.response` is not `None`.
```

### Comparing `types-requests-2.31.0.9/PKG-INFO` & `types-requests-2.32.0.20240521/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: types-requests
-Version: 2.31.0.9
+Version: 2.32.0.20240521
 Summary: Typing stubs for requests
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for requests
 
 This is a [PEP 561](https://peps.python.org/pep-0561/)
 type stub package for the [`requests`](https://github.com/psf/requests) package.
 It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `requests`.
 
 This version of `types-requests` aims to provide accurate annotations
-for `requests==2.31.*`.
+for `requests==2.32.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e92bfcbab2d15c407acc6ebaeceda5688e65e280` and was tested
-with mypy 1.5.1, pyright 1.1.330, and
-pytype 2023.10.5.
+This package was generated from typeshed commit `6816cf47f7f8c98f7214ee8187b7c697539907ee` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
+pytype 2024.4.11.
```

### Comparing `types-requests-2.31.0.9/requests-stubs/__init__.pyi` & `types-requests-2.32.0.20240521/requests-stubs/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from . import packages as packages, utils as utils
 from .__version__ import (
     __author__ as __author__,
     __author_email__ as __author_email__,
     __build__ as __build__,
     __cake__ as __cake__,
     __copyright__ as __copyright__,
     __description__ as __description__,
```

### Comparing `types-requests-2.31.0.9/requests-stubs/adapters.pyi` & `types-requests-2.32.0.20240521/requests-stubs/adapters.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.9/requests-stubs/api.pyi` & `types-requests-2.32.0.20240521/requests-stubs/api.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from _typeshed import Incomplete
 from collections.abc import Mapping
 from typing_extensions import TypeAlias
 
 from .models import Response
 from .sessions import RequestsCookieJar, _Auth, _Cert, _Data, _Files, _HooksInput, _Params, _TextMapping, _Timeout, _Verify
 
-_HeadersMapping: TypeAlias = Mapping[str, str | bytes]
+_HeadersMapping: TypeAlias = Mapping[str, str | bytes | None]
 
 def request(
     method: str | bytes,
     url: str | bytes,
     *,
     params: _Params | None = ...,
     data: _Data | None = ...,
```

### Comparing `types-requests-2.31.0.9/requests-stubs/auth.pyi` & `types-requests-2.32.0.20240521/requests-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.9/requests-stubs/compat.pyi` & `types-requests-2.32.0.20240521/requests-stubs/compat.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from builtins import bytes as bytes, str as str
 from collections import OrderedDict as OrderedDict
-from typing_extensions import Literal, TypeAlias
+from typing import Literal
+from typing_extensions import TypeAlias
 from urllib.parse import (
     quote as quote,
     quote_plus as quote_plus,
     unquote as unquote,
     unquote_plus as unquote_plus,
     urldefrag as urldefrag,
     urlencode as urlencode,
```

### Comparing `types-requests-2.31.0.9/requests-stubs/exceptions.pyi` & `types-requests-2.32.0.20240521/requests-stubs/exceptions.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+from typing import Any
+
 from urllib3.exceptions import HTTPError as BaseHTTPError
 
 from .models import Request, Response
 from .sessions import PreparedRequest
 
 class RequestException(OSError):
     response: Response | None
     request: Request | PreparedRequest | None
     def __init__(
         self, *args: object, request: Request | PreparedRequest | None = ..., response: Response | None = ...
     ) -> None: ...
 
 class InvalidJSONError(RequestException): ...
 class JSONDecodeError(InvalidJSONError): ...
-class HTTPError(RequestException): ...
+
+class HTTPError(RequestException):
+    request: Request | PreparedRequest | Any
+    response: Response | Any
+
 class ConnectionError(RequestException): ...
 class ProxyError(ConnectionError): ...
 class SSLError(ConnectionError): ...
 class Timeout(RequestException): ...
 class ConnectTimeout(ConnectionError, Timeout): ...
 class ReadTimeout(Timeout): ...
 class URLRequired(RequestException): ...
```

### Comparing `types-requests-2.31.0.9/requests-stubs/help.pyi` & `types-requests-2.32.0.20240521/requests-stubs/help.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing_extensions import TypedDict
+from typing import TypedDict
 
 class _VersionDict(TypedDict):
     version: str
 
 class _OptionalVersionDict(TypedDict):
     version: str | None
```

### Comparing `types-requests-2.31.0.9/requests-stubs/models.pyi` & `types-requests-2.32.0.20240521/requests-stubs/models.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         json=None,
     ) -> None: ...
     def copy(self) -> PreparedRequest: ...
     def prepare_method(self, method) -> None: ...
     def prepare_url(self, url, params) -> None: ...
     def prepare_headers(self, headers) -> None: ...
     def prepare_body(self, data, files, json=None) -> None: ...
-    def prepare_content_length(self, body) -> None: ...
+    def prepare_content_length(self, body: bytes | str | None) -> None: ...
     def prepare_auth(self, auth, url="") -> None: ...
     def prepare_cookies(self, cookies) -> None: ...
     def prepare_hooks(self, hooks) -> None: ...
 
 class Response:
     __attrs__: Any
     _content: bytes | None  # undocumented
```

### Comparing `types-requests-2.31.0.9/requests-stubs/sessions.pyi` & `types-requests-2.32.0.20240521/requests-stubs/sessions.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from _typeshed import Incomplete, SupportsItems, SupportsRead, Unused
 from collections.abc import Callable, Iterable, Mapping, MutableMapping
-from typing import Any
-from typing_extensions import Self, TypeAlias, TypedDict
+from typing import Any, TypedDict
+from typing_extensions import Self, TypeAlias
 
 from urllib3._collections import RecentlyUsedContainer
 
 from . import adapters, auth as _auth, compat, cookies, exceptions, hooks, models, status_codes, utils
 from .models import Response
 from .structures import CaseInsensitiveDict as CaseInsensitiveDict
 
@@ -32,14 +32,15 @@
 get_environ_proxies = utils.get_environ_proxies
 get_netrc_auth = utils.get_netrc_auth
 should_bypass_proxies = utils.should_bypass_proxies
 get_auth_from_url = utils.get_auth_from_url
 codes = status_codes.codes
 REDIRECT_STATI = models.REDIRECT_STATI
 
+def preferred_clock() -> float: ...
 def merge_setting(request_setting, session_setting, dict_class=...): ...
 def merge_hooks(request_hooks, session_hooks, dict_class=...): ...
 
 class SessionRedirectMixin:
     def resolve_redirects(
         self,
         resp,
```

### Comparing `types-requests-2.31.0.9/requests-stubs/structures.pyi` & `types-requests-2.32.0.20240521/requests-stubs/structures.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,12 +14,12 @@
     def __len__(self) -> int: ...
     def copy(self) -> CaseInsensitiveDict[_VT]: ...
 
 class LookupDict(dict[str, _VT]):
     name: Any
     def __init__(self, name: Any = None) -> None: ...
     def __getitem__(self, key: str) -> _VT | None: ...  # type: ignore[override]
-    def __setattr__(self, __attr: str, __value: _VT) -> None: ...
+    def __setattr__(self, attr: str, value: _VT, /) -> None: ...
     @overload
     def get(self, key: str, default: None = None) -> _VT | None: ...
     @overload
     def get(self, key: str, default: _D | _VT) -> _D | _VT: ...
```

### Comparing `types-requests-2.31.0.9/requests-stubs/utils.pyi` & `types-requests-2.32.0.20240521/requests-stubs/utils.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 def to_key_val_list(value): ...
 def parse_list_header(value): ...
 def parse_dict_header(value): ...
 def unquote_header_value(value, is_filename: bool = False): ...
 def dict_from_cookiejar(cj): ...
 def add_dict_to_cookiejar(cj, cookie_dict): ...
 def get_encodings_from_content(content): ...
-def get_encoding_from_headers(headers): ...
+def get_encoding_from_headers(headers: Mapping[str, str]) -> str | None: ...
 def stream_decode_response_unicode(iterator, r): ...
 def iter_slices(string: str, slice_length: int | None) -> Generator[str, None, None]: ...
 def get_unicode_from_response(r): ...
 
 UNRESERVED_SET: frozenset[str]
 
 def unquote_unreserved(uri: str) -> str: ...
```

### Comparing `types-requests-2.31.0.9/setup.py` & `types-requests-2.32.0.20240521/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,43 +11,43 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `requests`.
 
 This version of `types-requests` aims to provide accurate annotations
-for `requests==2.31.*`.
+for `requests==2.32.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e92bfcbab2d15c407acc6ebaeceda5688e65e280` and was tested
-with mypy 1.5.1, pyright 1.1.330, and
-pytype 2023.10.5.
+This package was generated from typeshed commit `6816cf47f7f8c98f7214ee8187b7c697539907ee` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.31.0.9",
+      version="2.32.0.20240521",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['urllib3>=2'],
       packages=['requests-stubs'],
-      package_data={'requests-stubs': ['__init__.pyi', '__version__.pyi', 'adapters.pyi', 'api.pyi', 'auth.pyi', 'certs.pyi', 'compat.pyi', 'cookies.pyi', 'exceptions.pyi', 'help.pyi', 'hooks.pyi', 'models.pyi', 'packages.pyi', 'sessions.pyi', 'status_codes.pyi', 'structures.pyi', 'utils.pyi', 'METADATA.toml']},
+      package_data={'requests-stubs': ['__init__.pyi', '__version__.pyi', 'adapters.pyi', 'api.pyi', 'auth.pyi', 'certs.pyi', 'compat.pyi', 'cookies.pyi', 'exceptions.pyi', 'help.pyi', 'hooks.pyi', 'models.pyi', 'packages.pyi', 'sessions.pyi', 'status_codes.pyi', 'structures.pyi', 'utils.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
-      python_requires=">=3.7",
+      python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-requests-2.31.0.9/types_requests.egg-info/PKG-INFO` & `types-requests-2.32.0.20240521/types_requests.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: types-requests
-Version: 2.31.0.9
+Version: 2.32.0.20240521
 Summary: Typing stubs for requests
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for requests
 
 This is a [PEP 561](https://peps.python.org/pep-0561/)
 type stub package for the [`requests`](https://github.com/psf/requests) package.
 It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `requests`.
 
 This version of `types-requests` aims to provide accurate annotations
-for `requests==2.31.*`.
+for `requests==2.32.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e92bfcbab2d15c407acc6ebaeceda5688e65e280` and was tested
-with mypy 1.5.1, pyright 1.1.330, and
-pytype 2023.10.5.
+This package was generated from typeshed commit `6816cf47f7f8c98f7214ee8187b7c697539907ee` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
+pytype 2024.4.11.
```

### Comparing `types-requests-2.31.0.9/types_requests.egg-info/SOURCES.txt` & `types-requests-2.32.0.20240521/types_requests.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 requests-stubs/compat.pyi
 requests-stubs/cookies.pyi
 requests-stubs/exceptions.pyi
 requests-stubs/help.pyi
 requests-stubs/hooks.pyi
 requests-stubs/models.pyi
 requests-stubs/packages.pyi
+requests-stubs/py.typed
 requests-stubs/sessions.pyi
 requests-stubs/status_codes.pyi
 requests-stubs/structures.pyi
 requests-stubs/utils.pyi
 types_requests.egg-info/PKG-INFO
 types_requests.egg-info/SOURCES.txt
 types_requests.egg-info/dependency_links.txt
```

