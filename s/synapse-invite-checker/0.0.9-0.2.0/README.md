# Comparing `tmp/synapse_invite_checker-0.0.9.tar.gz` & `tmp/synapse_invite_checker-0.2.0.tar.gz`

## Comparing `synapse_invite_checker-0.0.9.tar` & `synapse_invite_checker-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/CHANGELOG.md
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/cliff.toml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/.github/CODEOWNERS
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/.github/workflows/main.yml
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/.github/workflows/python.yml
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/synapse_invite_checker/__init__.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/synapse_invite_checker/config.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/synapse_invite_checker/handlers.py
--rw-r--r--   0        0        0    16019 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/synapse_invite_checker/invite_checker.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/synapse_invite_checker/store.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/synapse_invite_checker/types.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/tests/__init__.py
--rw-r--r--   0        0        0    30670 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/tests/rest.py
--rw-r--r--   0        0        0    34243 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/tests/server.py
--rw-r--r--   0        0        0    60887 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/tests/test_simple.py
--rw-r--r--   0        0        0    34967 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/tests/unittest.py
--rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/tests/utils.py
--rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/tests/certs/client.pem
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/tests/test_utils/event_injection.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/tests/test_utils/html_parsers.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/tests/test_utils/logging_setup.py
--rw-r--r--   0        0        0    12094 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/tests/test_utils/oidc.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/.gitignore
--rw-r--r--   0        0        0    34468 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/LICENSE
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/README.md
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 synapse_invite_checker-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/cliff.toml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/.github/workflows/python.yml
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/synapse_invite_checker/__init__.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/synapse_invite_checker/config.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/synapse_invite_checker/handlers.py
+-rw-r--r--   0        0        0    16055 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/synapse_invite_checker/invite_checker.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/synapse_invite_checker/store.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/synapse_invite_checker/types.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    30654 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/tests/rest.py
+-rw-r--r--   0        0        0    34243 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/tests/server.py
+-rw-r--r--   0        0        0    60887 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/tests/test_simple.py
+-rw-r--r--   0        0        0    34959 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/tests/unittest.py
+-rw-r--r--   0        0        0    10068 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/tests/certs/client.pem
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/tests/test_utils/event_injection.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/tests/test_utils/html_parsers.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/tests/test_utils/logging_setup.py
+-rw-r--r--   0        0        0    12094 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/tests/test_utils/oidc.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/.gitignore
+-rw-r--r--   0        0        0    34468 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/README.md
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 synapse_invite_checker-0.2.0/PKG-INFO
```

### Comparing `synapse_invite_checker-0.0.9/CHANGELOG.md` & `synapse_invite_checker-0.2.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.2.0] - 2024-05-22
+
+- Use SimpleHttpClient with proxy enabled to fetch CA roots
+
 ## [0.0.9] - 2023-02-10
 
 BREAKING: rename user column to avoid issues with SQL statements on postgres (that aren't handled by the synapse DB
 API). This also renames the table to simplify migration. You may want to delete the old (and probably empty table).
 
 ## [0.0.8] - 2023-02-09
```

### Comparing `synapse_invite_checker-0.0.9/cliff.toml` & `synapse_invite_checker-0.2.0/cliff.toml`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/.github/workflows/python.yml` & `synapse_invite_checker-0.2.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/synapse_invite_checker/config.py` & `synapse_invite_checker-0.2.0/synapse_invite_checker/config.py`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/synapse_invite_checker/handlers.py` & `synapse_invite_checker-0.2.0/synapse_invite_checker/handlers.py`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/synapse_invite_checker/invite_checker.py` & `synapse_invite_checker-0.2.0/synapse_invite_checker/invite_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             connectTimeout=15,
             contextFactory=MtlsPolicy(config),
             pool=pool,
         )
 
 
 class InviteChecker:
-    __version__ = "0.0.9"
+    __version__ = "0.2.0"
 
     def __init__(self, config: InviteCheckerConfig, api: ModuleApi):
         self.api = api
 
         self.config = config
 
         self.federation_list_client = FederationAllowListClient(api._hs, self.config)
@@ -271,20 +271,20 @@
     async def _raw_federation_list_fetch(self) -> str:
         resp = await self.federation_list_client.get_raw(
             self.config.federation_list_url
         )
         return resp.decode()
 
     async def _raw_gematik_root_ca_fetch(self) -> dict:
-        return await self.api.http_client.get_json(
+        return await self.api._hs.get_proxied_http_client().get_json(
             f"{self.config.gematik_ca_baseurl}/ECC/ROOT-CA/roots.json"
         )
 
     async def _raw_gematik_intermediate_cert_fetch(self, cn: str) -> bytes:
-        return await self.api.http_client.get_raw(
+        return await self.api._hs.get_proxied_http_client().get_raw(
             f"{self.config.gematik_ca_baseurl}/ECC/SUB-CA/{quote(cn.replace(' ', '_'), safe='')}.der"
         )
 
     def _load_cert_b64(self, cert: str) -> X509:
         return load_certificate(FILETYPE_ASN1, base64.b64decode(cert))
 
     @cached(cache=TTLCache(maxsize=1, ttl=60 * 60))
```

### Comparing `synapse_invite_checker-0.0.9/synapse_invite_checker/store.py` & `synapse_invite_checker-0.2.0/synapse_invite_checker/store.py`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/synapse_invite_checker/types.py` & `synapse_invite_checker-0.2.0/synapse_invite_checker/types.py`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/tests/__init__.py` & `synapse_invite_checker-0.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/tests/rest.py` & `synapse_invite_checker-0.2.0/tests/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,29 +70,27 @@
         room_creator: str | None = ...,
         is_public: bool | None = ...,
         room_version: str | None = ...,
         tok: str | None = ...,
         expect_code: Literal[200] = ...,
         extra_content: dict | None = ...,
         custom_headers: Iterable[tuple[AnyStr, AnyStr]] | None = ...,
-    ) -> str:
-        ...
+    ) -> str: ...
 
     @overload
     def create_room_as(
         self,
         room_creator: str | None = ...,
         is_public: bool | None = ...,
         room_version: str | None = ...,
         tok: str | None = ...,
         expect_code: int = ...,
         extra_content: dict | None = ...,
         custom_headers: Iterable[tuple[AnyStr, AnyStr]] | None = ...,
-    ) -> str | None:
-        ...
+    ) -> str | None: ...
 
     def create_room_as(
         self,
         room_creator: str | None = None,
         is_public: bool | None = True,
         room_version: str | None = None,
         tok: str | None = None,
```

### Comparing `synapse_invite_checker-0.0.9/tests/server.py` & `synapse_invite_checker-0.2.0/tests/server.py`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/tests/test_simple.py` & `synapse_invite_checker-0.2.0/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/tests/unittest.py` & `synapse_invite_checker-0.2.0/tests/unittest.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,15 @@
 S = TypeVar("S")
 
 
 class _TypedFailure(Generic[_ExcType_co], Protocol):
     """Extension to twisted.Failure, where the 'value' has a certain type."""
 
     @property
-    def value(self) -> _ExcType_co:
-        ...
+    def value(self) -> _ExcType_co: ...
 
 
 def around(target: TV) -> Callable[[Callable[Concatenate[S, P], R]], None]:
     """A CLOS-style 'around' modifier, which wraps the original method of the
     given instance with another piece of code.
 
     @around(self)
```

### Comparing `synapse_invite_checker-0.0.9/tests/utils.py` & `synapse_invite_checker-0.2.0/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,21 +28,19 @@
 
 # When debugging a specific test, it's occasionally useful to write the
 # DB to disk and query it with the sqlite CLI.
 SQLITE_PERSIST_DB = os.environ.get("SYNAPSE_TEST_PERSIST_SQLITE_DB") is not None
 
 
 @overload
-def default_config(name: str, parse: Literal[False] = ...) -> dict[str, object]:
-    ...
+def default_config(name: str, parse: Literal[False] = ...) -> dict[str, object]: ...
 
 
 @overload
-def default_config(name: str, parse: Literal[True]) -> HomeServerConfig:
-    ...
+def default_config(name: str, parse: Literal[True]) -> HomeServerConfig: ...
 
 
 def default_config(
     name: str, parse: bool = False
 ) -> dict[str, object] | HomeServerConfig:
     """
     Create a reasonable test config.
```

### Comparing `synapse_invite_checker-0.0.9/tests/certs/client.pem` & `synapse_invite_checker-0.2.0/tests/certs/client.pem`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/tests/test_utils/__init__.py` & `synapse_invite_checker-0.2.0/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/tests/test_utils/event_injection.py` & `synapse_invite_checker-0.2.0/tests/test_utils/event_injection.py`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/tests/test_utils/html_parsers.py` & `synapse_invite_checker-0.2.0/tests/test_utils/html_parsers.py`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/tests/test_utils/logging_setup.py` & `synapse_invite_checker-0.2.0/tests/test_utils/logging_setup.py`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/tests/test_utils/oidc.py` & `synapse_invite_checker-0.2.0/tests/test_utils/oidc.py`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/LICENSE` & `synapse_invite_checker-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/README.md` & `synapse_invite_checker-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `synapse_invite_checker-0.0.9/pyproject.toml` & `synapse_invite_checker-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 dependencies = [
   "twisted",
   "cachetools",
   "asyncache",
   "jwcrypto",
   "pyopenssl"
 ]
-version = "0.0.9"
+version = "0.2.0"
 
 [project.urls]
 Documentation = "https://github.com/famedly/synapse-invite-checker#synapse-invite-checker"
 Issues = "https://github.com/famedly/synapse-invite-checker/-/issues"
 Source = "https://github.com/famedly/synapse-invite-checker/"
 
 [tool.hatch.envs.default]
```

### Comparing `synapse_invite_checker-0.0.9/PKG-INFO` & `synapse_invite_checker-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: synapse-invite-checker
-Version: 0.0.9
+Version: 0.2.0
 Summary: Synapse module to handle TIM contact management and invite permissions
 Project-URL: Documentation, https://github.com/famedly/synapse-invite-checker#synapse-invite-checker
 Project-URL: Issues, https://github.com/famedly/synapse-invite-checker/-/issues
 Project-URL: Source, https://github.com/famedly/synapse-invite-checker/
 Author-email: Nicolas Werner <n.werner@famedly.com>
 License-Expression: AGPL-3.0-only
 License-File: LICENSE
```

