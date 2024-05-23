# Comparing `tmp/new_pykube-24.5.1-py3-none-any.whl.zip` & `tmp/new_pykube-24.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 25478 bytes, number of entries: 14
+Zip file size: 25528 bytes, number of entries: 14
 -rw-r--r--  2.0 unx      862 b- defN 80-Jan-01 00:00 pykube/__init__.py
 -rw-r--r--  2.0 unx       34 b- defN 80-Jan-01 00:00 pykube/__main__.py
--rw-r--r--  2.0 unx    11033 b- defN 80-Jan-01 00:00 pykube/config.py
+-rw-r--r--  2.0 unx    11034 b- defN 80-Jan-01 00:00 pykube/config.py
 -rw-r--r--  2.0 unx     1720 b- defN 80-Jan-01 00:00 pykube/console.py
 -rw-r--r--  2.0 unx      415 b- defN 80-Jan-01 00:00 pykube/exceptions.py
--rw-r--r--  2.0 unx    18563 b- defN 80-Jan-01 00:00 pykube/http.py
+-rw-r--r--  2.0 unx    18566 b- defN 80-Jan-01 00:00 pykube/http.py
 -rw-r--r--  2.0 unx      843 b- defN 80-Jan-01 00:00 pykube/mixins.py
 -rw-r--r--  2.0 unx    19583 b- defN 80-Jan-01 00:00 pykube/objects.py
 -rw-r--r--  2.0 unx     8819 b- defN 80-Jan-01 00:00 pykube/query.py
 -rw-r--r--  2.0 unx     2430 b- defN 80-Jan-01 00:00 pykube/utils.py
--rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 new_pykube-24.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5488 b- defN 80-Jan-01 00:00 new_pykube-24.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 new_pykube-24.5.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1045 b- defN 16-Jan-01 00:00 new_pykube-24.5.1.dist-info/RECORD
-14 files, 82281 bytes uncompressed, 23784 bytes compressed:  71.1%
+-rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 new_pykube-24.5.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5637 b- defN 80-Jan-01 00:00 new_pykube-24.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 new_pykube-24.5.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1045 b- defN 16-Jan-01 00:00 new_pykube-24.5.2.dist-info/RECORD
+14 files, 82434 bytes uncompressed, 23834 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pykube/query.py
 Comment: 
 
 Filename: pykube/utils.py
 Comment: 
 
-Filename: new_pykube-24.5.1.dist-info/LICENSE
+Filename: new_pykube-24.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: new_pykube-24.5.1.dist-info/METADATA
+Filename: new_pykube-24.5.2.dist-info/METADATA
 Comment: 
 
-Filename: new_pykube-24.5.1.dist-info/WHEEL
+Filename: new_pykube-24.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: new_pykube-24.5.1.dist-info/RECORD
+Filename: new_pykube-24.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pykube/config.py

```diff
@@ -331,15 +331,15 @@
         """
         Returns the provided data as a file location.
         """
         if not self._path:
             m = hashlib.md5()
             m.update(self._bytes)
 
-            path = Path(f"{tempfile.gettempdir()}/pykube-ng.{m.hexdigest()}.crt")
+            path = Path(f"{tempfile.gettempdir()}/new-pykube.{m.hexdigest()}.crt")
             if not path.exists() or path.stat().st_size == 0:
                 with open(path, "wb") as f:
                     f.write(self._bytes)
 
             self._path = path
 
         return str(self._path)
```

## pykube/http.py

```diff
@@ -129,15 +129,15 @@
             - EXPIRY_SKEW_PREVENTION_DELAY
         ) > datetime.datetime.utcnow().replace(tzinfo=UTC)
 
     def _refresh_oidc_token(self, config):
         if not oidc_auth_installed:
             raise ImportError(
                 "missing dependencies for OIDC token refresh support "
-                "(try pip install pykube-ng[oidc]"
+                "(try pip install new-pykube[oidc]"
             )
         auth_config = config.user["auth-provider"]["config"]
         if "idp-certificate-authority" in auth_config:
             verify = auth_config["idp-certificate-authority"].filename()
         else:
             verify = None
         oauth = OAuth2Session()
@@ -253,15 +253,15 @@
 
         if "auth-provider" in config.user:
             auth_provider = config.user["auth-provider"]
             if auth_provider.get("name") == "gcp":
                 dependencies = [google_auth_installed, jsonpath_installed]
                 if not all(dependencies):
                     raise ImportError(
-                        "missing dependencies for GCP support (try pip install pykube-ng[gcp]"
+                        "missing dependencies for GCP support (try pip install new-pykube[gcp]"
                     )
                 auth_config = auth_provider.get("config", {})
                 if "cmd-path" in auth_config:
                     output = subprocess.check_output(
                         [auth_config["cmd-path"]] + shlex.split(auth_config["cmd-args"])
                     )
                     parsed = json.loads(output)
@@ -348,15 +348,15 @@
         """
         self.config = config
         self.timeout = timeout
         self.url = self.config.cluster["server"]
         self.dry_run = dry_run
 
         session = requests.Session()
-        session.headers["User-Agent"] = f"pykube-ng/{__version__}"
+        session.headers["User-Agent"] = f"new-pykube/{__version__}"
         if not http_adapter:
             http_adapter = self.http_adapter_cls(self.config)
         session.mount("https://", http_adapter)
         session.mount("http://", http_adapter)
         self.session = session
         self.session.verify = verify
```

## Comparing `new_pykube-24.5.1.dist-info/LICENSE` & `new_pykube-24.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `new_pykube-24.5.1.dist-info/METADATA` & `new_pykube-24.5.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: new-pykube
-Version: 24.5.1
+Version: 24.5.2
 Summary: Python client library for Kubernetes
 Home-page: https://github.com/caas-team/new-pykube
 License: Apache
 Author: Jonathan Mayer
 Author-email: jonathan.mayer@telekom.de
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
@@ -217,7 +217,12 @@
 Create an issue and we will take a look. PRs are welcome.
 
 
 ## Code of Conduct
 
 In order to foster a kind, inclusive, and harassment-free community, this project follows the [Contributor Covenant Code of Conduct](http://contributor-covenant.org/version/1/4/).
 
+## Acknowledgments
+
+Thanks to [pykube-ng](https://codeberg.org/hjacobs/pykube-ng) project authored
+by [Henning Jacobs](https://github.com/hjacobs).
+
```

## Comparing `new_pykube-24.5.1.dist-info/RECORD` & `new_pykube-24.5.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pykube/__init__.py,sha256=_kVjVVRKkgXs-jlhNCysMCOpK8pW-F-P65paQDPWOGs,862
 pykube/__main__.py,sha256=q8wRYHD0YaMGQW-CN73tdERxPm_TOwfFi41yxkvK6og,34
-pykube/config.py,sha256=5jQC6roG0Kns1sjyVs0CYCpQexDKvYFi7O9aw1Htvz0,11033
+pykube/config.py,sha256=sMLxLRMNG-_JIoI-DsmCjoNSTXF5mW-IVTHhVrwK1S0,11034
 pykube/console.py,sha256=wlzlAFZdxzLylzU_Lc0jSqVD5aEpO-Z1ytmqJijPr1s,1720
 pykube/exceptions.py,sha256=lPeqCy7ETGgJjVqQb8FKDjgrJp8NGMbLgiJNwUwg7O8,415
-pykube/http.py,sha256=snN5-vq3sg3Di1InlcwGxrdh6xCp7FNILzm95C8iOG8,18563
+pykube/http.py,sha256=M6dZe05tmTfv-J3Co-6WgBerEDIkkAb1ogTuY9gLEag,18566
 pykube/mixins.py,sha256=K4MFq5Ba8G4Fb_aLeNNvrsMzcuJRG1Z7ljDtWfJwizo,843
 pykube/objects.py,sha256=q67Hu99DeMNJRejINyagfZjZ0KffyHEmXF2GwO0qVjw,19583
 pykube/query.py,sha256=IAhNfhMnBt9DxOenxTXgx_jjqK7Zh2djN-QrEo2e5wU,8819
 pykube/utils.py,sha256=OOwppqj62RGeLKKWdTvAo9l4uk1fC86592gI9oXHArM,2430
-new_pykube-24.5.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-new_pykube-24.5.1.dist-info/METADATA,sha256=hSfWNiUVtvC9JfmGe5WC9-S3-0r5BEKHlUoRt4I9LNI,5488
-new_pykube-24.5.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-new_pykube-24.5.1.dist-info/RECORD,,
+new_pykube-24.5.2.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+new_pykube-24.5.2.dist-info/METADATA,sha256=BqpFwQa2ozgrlH_8Kn3Sgefxxh1DqMf8APopFyVUKu4,5637
+new_pykube-24.5.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+new_pykube-24.5.2.dist-info/RECORD,,
```

