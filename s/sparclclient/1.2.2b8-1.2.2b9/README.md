# Comparing `tmp/sparclclient-1.2.2b8.tar.gz` & `tmp/sparclclient-1.2.2b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparclclient-1.2.2b8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sparclclient-1.2.2b9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sparclclient-1.2.2b8.tar` & `sparclclient-1.2.2b9.tar`

### file list

```diff
@@ -1,39 +1,37 @@
--rw-r--r--   0        0        0      624 2024-02-28 13:14:23.075817 sparclclient-1.2.2b8/.github/workflows/django.yml
--rw-r--r--   0        0        0     1812 2024-02-28 18:44:20.870945 sparclclient-1.2.2b8/.gitignore
--rw-r--r--   0        0        0      520 2024-03-01 22:14:39.145923 sparclclient-1.2.2b8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1065 2023-02-08 18:38:30.463459 sparclclient-1.2.2b8/.readthedocs.yaml
--rw-r--r--   0        0        0     1576 2023-02-08 18:38:30.463459 sparclclient-1.2.2b8/LICENSE
--rw-r--r--   0        0        0      638 2023-02-08 18:38:30.463459 sparclclient-1.2.2b8/Makefile
--rw-r--r--   0        0        0       87 2024-02-28 13:14:23.075817 sparclclient-1.2.2b8/README.md
--rw-r--r--   0        0        0      799 2023-02-08 18:38:30.507459 sparclclient-1.2.2b8/make.bat
--rw-r--r--   0        0        0     1365 2024-03-01 21:49:16.432474 sparclclient-1.2.2b8/pyproject.toml
--rw-r--r--   0        0        0       41 2024-02-28 13:14:23.075817 sparclclient-1.2.2b8/requirements-client.txt
--rw-r--r--   0        0        0      323 2024-02-28 16:18:05.019893 sparclclient-1.2.2b8/requirements-internal.txt
--rw-r--r--   0        0        0       56 2023-02-08 18:38:30.507459 sparclclient-1.2.2b8/requirements.txt
--rw-r--r--   0        0        0     3198 2024-02-28 13:14:23.075817 sparclclient-1.2.2b8/source/conf.py
--rw-r--r--   0        0        0      415 2023-02-08 18:38:30.507459 sparclclient-1.2.2b8/source/index.rst
--rw-r--r--   0        0        0      397 2023-02-08 18:38:30.507459 sparclclient-1.2.2b8/source/sparcl.rst
--rw-r--r--   0        0        0     8477 2024-02-28 13:14:23.075817 sparclclient-1.2.2b8/sparcl/Results.py
--rw-r--r--   0        0        0     1032 2024-03-06 14:15:41.383430 sparclclient-1.2.2b8/sparcl/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 18:38:30.507459 sparclclient-1.2.2b8/sparcl/benchmarks/__init__.py
--rwxr-xr-x   0        0        0     9424 2024-02-28 13:14:23.075817 sparclclient-1.2.2b8/sparcl/benchmarks/benchmarks.py
--rw-r--r--   0        0        0    35877 2024-03-06 14:02:40.648089 sparclclient-1.2.2b8/sparcl/client.py
--rw-r--r--   0        0        0      928 2024-02-28 13:14:23.075817 sparclclient-1.2.2b8/sparcl/conf.py
--rw-r--r--   0        0        0     3855 2024-02-28 13:14:23.075817 sparclclient-1.2.2b8/sparcl/exceptions.py
--rw-r--r--   0        0        0     5127 2024-03-01 22:17:05.364764 sparclclient-1.2.2b8/sparcl/fields.py
--rw-r--r--   0        0        0     8686 2024-03-01 22:17:05.364764 sparclclient-1.2.2b8/sparcl/gather_2d.py
--rw-r--r--   0        0        0    60801 2024-02-28 13:14:23.079817 sparclclient-1.2.2b8/sparcl/notebooks/UNPUBLISHED/SPARCL_client_method_tests.ipynb
--rw-r--r--   0        0        0    24728 2024-02-28 17:28:08.882246 sparclclient-1.2.2b8/sparcl/notebooks/UNPUBLISHED/sparcl_auth_cases.ipynb
--rw-r--r--   0        0        0   134582 2024-03-06 14:15:21.539041 sparclclient-1.2.2b8/sparcl/notebooks/sparcl-examples.ipynb
--rw-r--r--   0        0        0     1282 2024-02-28 13:14:23.079817 sparclclient-1.2.2b8/sparcl/resample_spectra.py
--rw-r--r--   0        0        0      329 2023-02-08 18:38:30.507459 sparclclient-1.2.2b8/sparcl/sparc.ini
--rw-r--r--   0        0        0    12965 2024-02-28 13:14:23.079817 sparclclient-1.2.2b8/sparcl/type_conversion.py
--rw-r--r--   0        0        0     1848 2024-02-28 13:14:23.079817 sparclclient-1.2.2b8/sparcl/unsupported.py
--rw-r--r--   0        0        0     6259 2024-02-28 13:14:23.079817 sparclclient-1.2.2b8/sparcl/utils.py
--rw-r--r--   0        0        0     3136 2024-02-28 13:14:23.079817 sparclclient-1.2.2b8/tests/expected_dev1.py
--rw-r--r--   0        0        0     4433 2024-02-28 13:14:23.079817 sparclclient-1.2.2b8/tests/expected_pat.py
--rw-r--r--   0        0        0    44333 2024-02-28 13:14:23.079817 sparclclient-1.2.2b8/tests/methods_tests.py
--rwxr-xr-x   0        0        0    23063 2024-02-28 13:14:23.079817 sparclclient-1.2.2b8/tests/tests_api.py
--rw-r--r--   0        0        0      944 2024-02-28 13:14:23.079817 sparclclient-1.2.2b8/tests/utils.py
--rw-r--r--   0        0        0      683 2024-02-28 13:14:23.079817 sparclclient-1.2.2b8/tox.ini
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 sparclclient-1.2.2b8/PKG-INFO
+-rw-r--r--   0        0        0      624 2024-02-28 13:14:23.075817 sparclclient-1.2.2b9/.github/workflows/django.yml
+-rw-r--r--   0        0        0     1812 2024-02-28 18:44:20.870945 sparclclient-1.2.2b9/.gitignore
+-rw-r--r--   0        0        0      520 2024-04-29 23:03:38.089790 sparclclient-1.2.2b9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1065 2023-02-08 18:38:30.463459 sparclclient-1.2.2b9/.readthedocs.yaml
+-rw-r--r--   0        0        0     1576 2023-02-08 18:38:30.463459 sparclclient-1.2.2b9/LICENSE
+-rw-r--r--   0        0        0      638 2023-02-08 18:38:30.463459 sparclclient-1.2.2b9/Makefile
+-rw-r--r--   0        0        0       87 2024-02-28 13:14:23.075817 sparclclient-1.2.2b9/README.md
+-rw-r--r--   0        0        0      799 2023-02-08 18:38:30.507459 sparclclient-1.2.2b9/make.bat
+-rw-r--r--   0        0        0     1430 2024-05-23 12:13:15.396191 sparclclient-1.2.2b9/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-02-28 13:14:23.075817 sparclclient-1.2.2b9/requirements-client.txt
+-rw-r--r--   0        0        0      323 2024-04-29 23:03:38.089790 sparclclient-1.2.2b9/requirements-internal.txt
+-rw-r--r--   0        0        0       56 2023-02-08 18:38:30.507459 sparclclient-1.2.2b9/requirements.txt
+-rw-r--r--   0        0        0     3198 2024-02-28 13:14:23.075817 sparclclient-1.2.2b9/source/conf.py
+-rw-r--r--   0        0        0      415 2023-02-08 18:38:30.507459 sparclclient-1.2.2b9/source/index.rst
+-rw-r--r--   0        0        0      397 2023-02-08 18:38:30.507459 sparclclient-1.2.2b9/source/sparcl.rst
+-rw-r--r--   0        0        0     8477 2024-02-28 13:14:23.075817 sparclclient-1.2.2b9/sparcl/Results.py
+-rw-r--r--   0        0        0     1032 2024-05-23 12:14:12.389295 sparclclient-1.2.2b9/sparcl/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-08 18:38:30.507459 sparclclient-1.2.2b9/sparcl/benchmarks/__init__.py
+-rwxr-xr-x   0        0        0     9424 2024-02-28 13:14:23.075817 sparclclient-1.2.2b9/sparcl/benchmarks/benchmarks.py
+-rw-r--r--   0        0        0    36177 2024-05-14 16:38:29.585010 sparclclient-1.2.2b9/sparcl/client.py
+-rw-r--r--   0        0        0      928 2024-02-28 13:14:23.075817 sparclclient-1.2.2b9/sparcl/conf.py
+-rw-r--r--   0        0        0     4040 2024-05-02 20:49:37.311262 sparclclient-1.2.2b9/sparcl/exceptions.py
+-rw-r--r--   0        0        0     5127 2024-04-29 23:03:38.089790 sparclclient-1.2.2b9/sparcl/fields.py
+-rw-r--r--   0        0        0     8686 2024-04-29 23:03:38.089790 sparclclient-1.2.2b9/sparcl/gather_2d.py
+-rw-r--r--   0        0        0   169268 2024-05-02 19:49:14.555035 sparclclient-1.2.2b9/sparcl/notebooks/sparcl-examples.ipynb
+-rw-r--r--   0        0        0     1282 2024-02-28 13:14:23.079817 sparclclient-1.2.2b9/sparcl/resample_spectra.py
+-rw-r--r--   0        0        0      329 2023-02-08 18:38:30.507459 sparclclient-1.2.2b9/sparcl/sparc.ini
+-rw-r--r--   0        0        0    12965 2024-02-28 13:14:23.079817 sparclclient-1.2.2b9/sparcl/type_conversion.py
+-rw-r--r--   0        0        0     1848 2024-02-28 13:14:23.079817 sparclclient-1.2.2b9/sparcl/unsupported.py
+-rw-r--r--   0        0        0     6259 2024-04-29 23:03:38.093790 sparclclient-1.2.2b9/sparcl/utils.py
+-rw-r--r--   0        0        0     3136 2024-04-29 23:48:03.383714 sparclclient-1.2.2b9/tests/expected_dev1.py
+-rw-r--r--   0        0        0     7381 2024-05-13 23:31:58.035417 sparclclient-1.2.2b9/tests/expected_pat.py
+-rw-r--r--   0        0        0    44333 2024-02-28 13:14:23.079817 sparclclient-1.2.2b9/tests/methods_tests.py
+-rwxr-xr-x   0        0        0    37043 2024-05-23 00:00:29.651537 sparclclient-1.2.2b9/tests/tests_api.py
+-rw-r--r--   0        0        0      944 2024-02-28 13:14:23.079817 sparclclient-1.2.2b9/tests/utils.py
+-rw-r--r--   0        0        0      683 2024-02-28 13:14:23.079817 sparclclient-1.2.2b9/tox.ini
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 sparclclient-1.2.2b9/PKG-INFO
```

### Comparing `sparclclient-1.2.2b8/.github/workflows/django.yml` & `sparclclient-1.2.2b9/.github/workflows/django.yml`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/.gitignore` & `sparclclient-1.2.2b9/.gitignore`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/.pre-commit-config.yaml` & `sparclclient-1.2.2b9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/.readthedocs.yaml` & `sparclclient-1.2.2b9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/LICENSE` & `sparclclient-1.2.2b9/LICENSE`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/Makefile` & `sparclclient-1.2.2b9/Makefile`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/make.bat` & `sparclclient-1.2.2b9/make.bat`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/pyproject.toml` & `sparclclient-1.2.2b9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 "Homepage" = "https://github.com/pypa/sparclclient"
 "Bug Tracker" = "https://github.com/pypa/sparclclient/issues"
 "Documentation" = "https://sparclclient.readthedocs.io/en/latest/"
 
 [tool.flit.module]
 name = "sparcl"
 
+[tool.flit.sdist]
+exclude = ["**/UNPUBLISHED/", "**/OBSOLETE/"]
+
 [tool.black]
 # https://black.readthedocs.io/en/stable/usage_and_configuration/index.html
 line-length = 79
 target-version = ['py37']
 include = '\.pyi?$'
 # 'extend-exclude' excludes files or directories in addition to the defaults
 extend-exclude = '''
```

### Comparing `sparclclient-1.2.2b8/source/conf.py` & `sparclclient-1.2.2b9/source/conf.py`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/sparcl/Results.py` & `sparclclient-1.2.2b9/sparcl/Results.py`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/sparcl/__init__.py` & `sparclclient-1.2.2b9/sparcl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 # Example of a correct version string: '0.4.0a3.dev35'
 # __version__ = '1.1'
 # __version__ = '1.2.0b4'
 # __version__ = '1.2.0'  # Release
 # __version__ = "1.2.1b3"
 # __version__ = "1.2.1"
 # FIRST uncommented value will be used! (so only leave one uncommented)
-__version__ = "1.2.2b8"
+__version__ = "1.2.2b9"
```

### Comparing `sparclclient-1.2.2b8/sparcl/benchmarks/benchmarks.py` & `sparclclient-1.2.2b9/sparcl/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/sparcl/client.py` & `sparclclient-1.2.2b9/sparcl/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,25 +246,27 @@
     def login(self, email, password=None):
         """Login to the SPARCL service.
 
         Args:
             email (:obj:`str`): User login email.
 
             password (:obj:`str`, optional): User SSO password.
-                If not given, the output will
-                prompt the user to enter in their SSO password.
+                If not given, the output will prompt the user
+                to enter in their SSO password.
 
         Returns:
             None.
 
         Example:
-            >>> client = SparclClient()
-            >>> client.login('test_user@noirlab.edu', 'test123')
+            >>>
+            >> client = SparclClient()
+            >> client.login('test_user@noirlab.edu', 'testpw')
             Logged in successfully with email='test_user@noirlab.edu'
         """
+
         if email is None:  # "logout"
             old_email = self.session.auth[0] if self.session.auth else None
             self.session.auth = None
             self.token = None
             print(
                 f"Logged-out successfully. "
                 f" Previously logged-in with email {old_email}."
@@ -304,30 +306,30 @@
 
         Returns:
             None.
 
         Example:
             >>> client = SparclClient()
             >>> client.logout()
-            Logged-out successfully.
-            Previously logged-in with email test_user@noirlab.edu.
+            Logged-out successfully.  Previously logged-in with email None.
         """
+
         return self.login(None)
 
     @property
     def authorized(self):
         auth = TokenAuth(self.token) if self.token else None
         response = requests.get(
             f"{self.apiurl}/auth_status/", auth=auth, timeout=self.timeout
         )
         auth_status = response.json()
         #! print(f"DBG authorized: {auth_status=}")
 
-        username = auth_status.get('Loggedin_User')
-        all_private_drs = set(auth_status.get("All_Private_Datasets"))
+        username = auth_status.get("Loggedin_User")
+        #! all_private_drs = set(auth_status.get("All_Private_Datasets"))
         all_public_drs = set(auth_status.get("All_Public_Datasets"))
         auth_drs = set(auth_status.get("Authorized_Private_Datasets"))
         res = dict(
             Loggedin_As=username,  # email
             Authorized_Datasets=auth_drs | all_public_drs,
             #! Unauthorized_Datasets=all_private_drs - auth_drs,
             #! All_Private_Datasets=all_private_drs,
@@ -442,15 +444,16 @@
 
         Returns:
             Set of fields available from data sets in DATASET_LIST.
 
         Example:
             >>> client = SparclClient()
             >>> sorted(client.get_available_fields())
-            ['data_release', 'datasetgroup', 'dateobs', 'dateobs_center', 'dec', 'dirpath', 'exptime', 'extra_files', 'filename', 'filesize', 'flux', 'instrument', 'ivar', 'mask', 'model', 'ra', 'redshift', 'redshift_err', 'redshift_warning', 'site', 'sparcl_id', 'specid', 'specprimary', 'spectype', 'survey', 'targetid', 'telescope', 'updated', 'wave_sigma', 'wavelength', 'wavemax', 'wavemin']
+            ['data_release', 'datasetgroup', 'dateobs', 'dateobs_center', 'dec', 'exptime', 'extra_files', 'file', 'flux', 'instrument', 'ivar', 'mask', 'model', 'ra', 'redshift', 'redshift_err', 'redshift_warning', 'site', 'sparcl_id', 'specid', 'specprimary', 'spectype', 'survey', 'targetid', 'telescope', 'updated', 'wave_sigma', 'wavelength', 'wavemax', 'wavemin']
+
         """  # noqa: E501
 
         drs = self.fields.all_drs if dataset_list is None else dataset_list
         every = [set(self.fields.n2o[dr]) for dr in drs]
         return set.intersection(*every)
 
     @property
@@ -461,15 +464,15 @@
 
         Returns:
             API version (:obj:`float`).
 
         Example:
             >>> client = SparclClient()
             >>> client.version
-            9.0
+            11.0
         """
 
         if self.apiversion is None:
             response = requests.get(
                 f"{self.apiurl}/version", timeout=self.timeout, cache=True
             )
             self.apiversion = float(response.content)
@@ -651,16 +654,17 @@
                 statement. Defaults to False.
 
         Returns:
             A list of the subset of specids in the given specid_list that
             are NOT stored in the SPARCL database.
 
         Example:
-            >>> client = SparclClient(url=_PAT)
-            >>> specids = ['7972592460248666112', '3663710814482833408']
+            >>> client = SparclClient(url=_DEV)
+            >>> found = client.find(outfields=['specid'], limit=2)
+            >>> specids = [f.specid for f in found.records]
             >>> client.missing_specids(specids + ['bad_id'])
             ['bad_id']
         """
         if dataset_list is None:
             dataset_list = self.fields.all_drs
         assert isinstance(
             dataset_list, (list, set)
@@ -739,15 +743,15 @@
                 statement. Defaults to False.
 
         Returns:
             :class:`~sparcl.Results.Retrieved`: Contains header and records.
 
         Example:
             >>> client = SparclClient()
-            >>> ids = ['00000f0b-07db-4234-892a-6e347db79c89',]
+            >>> ids = client.find(limit=1).ids
             >>> inc = ['sparcl_id', 'flux', 'wavelength', 'model']
             >>> ret = client.retrieve(uuid_list=ids, include=inc)
             >>> type(ret.records[0].wavelength)
             <class 'numpy.ndarray'>
         """
 
         # Variants for async, etc.
@@ -762,14 +766,15 @@
         #        Defaults to 500.
         #
         # These were keyword params:
         svc = "spectras"  # retrieve, spectras
         format = "pkl"  # 'json',
         chunk = 500
 
+        orig_dataset_list = dataset_list
         if dataset_list is None:
             dataset_list = self.fields.all_drs
         assert isinstance(
             dataset_list, (list, set)
         ), f"DATASET_LIST must be a list. Found {dataset_list}"
 
         verbose = self.verbose if verbose is None else verbose
@@ -803,16 +808,21 @@
         )
         uparams = {
             "include": ",".join(com_include),
             # limit=limit,  # altered uuid_list to reflect limit
             #! "chunk_len": chunk,
             "format": format,
             #! "1thread": "yes",  # @@@ 7.3.2023
-            "dataset_list": ",".join(dataset_list),
+            #!"dataset_list": ",".join(dataset_list),
         }
+        # Do not put dataset_list in server call if it wasn't in client call.
+        # Else will interfer with defaulting behavior of AUTH (DLS-504).
+        if orig_dataset_list is not None:
+            uparams["dataset_list"] = ",".join(dataset_list)
+
         qstr = urlencode(uparams)
 
         #!url = f'{self.apiurl}/retrieve/?{qstr}'
         url = f"{self.apiurl}/{svc}/?{qstr}"
         if verbose:
             print(f'Using url="{url}"')
             ut.tic()
```

### Comparing `sparclclient-1.2.2b8/sparcl/conf.py` & `sparclclient-1.2.2b9/sparcl/conf.py`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/sparcl/exceptions.py` & `sparclclient-1.2.2b9/sparcl/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,28 +17,30 @@
         return BadPath(status.get("errorMessage"))
     elif status.get("errorCode") == "BADQUERY":
         return BadQuery(status.get("errorMessage"))
     elif status.get("errorCode") == "UNKFIELD":
         return UnknownField(status.get("errorMessage"))
     elif status.get("errorCode") == "BADCONST":
         return BadSearchConstraint(status.get("errorMessage"))
+    elif status.get("errorCode") == "NODRACCESS":
+        return AccessNotAllowed(status.get("errorMessage"))
     else:
         return UnknownServerError(
             f"{status.get('errorMessage')} "
             f"[{status.get('errorCode')}] "
             f"{status.get('traceback')}"
         )
 
 
 class BaseSparclException(Exception):
     """Base Class for all SPARCL exceptions."""
 
     error_code = "UNKNOWN"
     error_message = "<NA>"
-    traceback = None
+    traceback = True
 
     def get_subclass_name(self):
         return self.__class__.__name__
 
     def __init__(self, error_message, error_code=None):
         Exception.__init__(self)
         self.error_message = error_message
@@ -136,8 +138,12 @@
 class NoIDs(BaseSparclException):
     """The length of the list of original IDs passed to the reorder
     method was zero"""
 
     error_code = "NOIDS"
 
 
+class AccessNotAllowed(BaseSparclException):
+    error_code = "DSDENIED"
+
+
 # error_code values should be no bigger than 8 characters 12345678
```

### Comparing `sparclclient-1.2.2b8/sparcl/fields.py` & `sparclclient-1.2.2b9/sparcl/fields.py`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/sparcl/gather_2d.py` & `sparclclient-1.2.2b9/sparcl/gather_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         >>> client = sparcl.client.SparclClient()
         >>> specflds = ['wavelength', 'model']
         >>> cons = {"data_release": ['BOSS-DR16']}
         >>> found = client.find(constraints=cons, limit=21)
         >>> got = client.retrieve(found.ids, include=specflds)
         >>> ar_dict, grid = align_records(got.records, fields=specflds)
         >>> ar_dict['model'].shape
-        (21, 4666)
+        (21, 4669)
 
     """
     # Report Garbage In
     if "wavelength" not in fields:
         msg = (
             f'You must provide "wavelength" in the list provided'
             f' in the "fields" paramter.  Got: {fields}'
```

### Comparing `sparclclient-1.2.2b8/sparcl/notebooks/sparcl-examples.ipynb` & `sparclclient-1.2.2b9/sparcl/notebooks/sparcl-examples.ipynb`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9728316053732949%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(1, "__version__ = \'20240306\' # yyyymmdd; \\n")], '*

 * *            "delete: [1]}}, 5: {'metadata': {replace: OrderedDict([('tags', [])])}, 'source': "*

 * *            "{insert: [(12, 'from IPython.display import display, Markdown, Latex\\n')]}}, 8: "*

 * *            "{'metadata': {replace: OrderedDict([('tags', [])])}, 'outputs': {0: {'text': {insert: "*

 * *            "[(0, 'Processing /home/pothiers/sandbox/sparclclient\\n'), (1, '  Installing build "*

 * *            "dependencies . […]*

```diff
@@ -14,15 +14,15 @@
             "execution_count": 1,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "__author__ = 'Steve Pothier <steve.pothier@noirlab.edu>'\n",
-                "__version__ = '20240224' # yyyymmdd; \n",
+                "__version__ = '20240306' # yyyymmdd; \n",
                 "__keywords__ = ['HowTo', 'astronomy', 'tutorial', 'client', 'sparcl', 'NOIRlab']"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
@@ -59,92 +59,110 @@
                 "<a class=\"anchor\" id=\"imports\"></a>\n",
                 "## Imports and Setup"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "from pprint import pformat as pf\n",
                 "from pprint import pp\n",
                 "import os.path\n",
                 "from importlib import reload\n",
                 "from collections import defaultdict\n",
                 "from datetime import datetime\n",
                 "import warnings\n",
                 "from getpass import getpass\n",
                 "\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
+                "from IPython.display import display, Markdown, Latex\n",
                 "\n",
                 "class StopExecution(Exception):\n",
                 "    def _render_traceback_(self):\n",
                 "        pass\n",
                 "\n",
                 "# %matplotlib inline\n",
                 "# requires installing ipympl\n",
                 "%matplotlib widget\n",
                 "plt.rcParams['font.size'] = 14"
             ]
         },
         {
+            "cell_type": "raw",
+            "metadata": {},
+            "source": [
+                "### "
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "<a class=\"anchor\" id=\"install\"></a>\n",
                 "## Install most recent version of the SPARCLCLIENT\n",
                 "*NOTE: After installing the most recent version, please restart your kernel.*"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: sparclclient in /home/pothiers/sandbox/sparclclient/venv/lib/python3.10/site-packages (1.2.2b6)\n",
-                        "Collecting sparclclient\n",
-                        "  Downloading sparclclient-1.2.2b7-py2.py3-none-any.whl.metadata (566 bytes)\n",
-                        "Downloading sparclclient-1.2.2b7-py2.py3-none-any.whl (111 kB)\n",
-                        "\u001b[2K   \u001b[90m\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u001b[0m \u001b[32m111.9/111.9 kB\u001b[0m \u001b[31m2.1 MB/s\u001b[0m eta \u001b[36m0:00:00\u001b[0m \u001b[36m0:00:01\u001b[0m\n",
-                        "\u001b[?25hInstalling collected packages: sparclclient\n",
+                        "Processing /home/pothiers/sandbox/sparclclient\n",
+                        "  Installing build dependencies ... \u001b[?25ldone\n",
+                        "\u001b[?25h  Getting requirements to build wheel ... \u001b[?25ldone\n",
+                        "\u001b[?25h  Preparing metadata (pyproject.toml) ... \u001b[?25ldone\n",
+                        "\u001b[?25hBuilding wheels for collected packages: sparclclient\n",
+                        "  Building wheel for sparclclient (pyproject.toml) ... \u001b[?25ldone\n",
+                        "\u001b[?25h  Created wheel for sparclclient: filename=sparclclient-1.2.2b8-py2.py3-none-any.whl size=3533665 sha256=fc035800e3269eccc70d3658f293c93d2fe7f07850a17cbdb47c9b2ce0de36ad\n",
+                        "  Stored in directory: /tmp/pip-ephem-wheel-cache-lko1mvqq/wheels/9b/de/a2/3f7a82cf4ca7c9e775a1ed1daeea35010570464a1aaa8c370c\n",
+                        "Successfully built sparclclient\n",
+                        "Installing collected packages: sparclclient\n",
                         "  Attempting uninstall: sparclclient\n",
-                        "    Found existing installation: sparclclient 1.2.2b6\n",
-                        "    Uninstalling sparclclient-1.2.2b6:\n",
-                        "      Successfully uninstalled sparclclient-1.2.2b6\n",
-                        "Successfully installed sparclclient-1.2.2b7\n"
+                        "    Found existing installation: sparclclient 1.2.2b8\n",
+                        "    Uninstalling sparclclient-1.2.2b8:\n",
+                        "      Successfully uninstalled sparclclient-1.2.2b8\n",
+                        "Successfully installed sparclclient-1.2.2b8\n"
                     ]
                 }
             ],
             "source": [
                 "# !pip install --upgrade sparclclient         # Latest released version\n",
-                "!pip install --pre --upgrade sparclclient   # Lastest pre-released version\n",
+                "# !pip install --pre --upgrade sparclclient   # Lastest pre-released version\n",
                 "\n",
                 "# Uncomment next line to load SPARCLCLIENT from local current version of software.\n",
-                "#!pip install --pre --upgrade ../.."
+                "!pip install --pre --upgrade ../.."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Run started: 2024-03-06 07:12:12.121248\n"
+                        "Run started: 2024-05-02 10:22:12.795845\n"
                     ]
                 }
             ],
             "source": [
                 "import sparcl.client\n",
                 "print(f'Run started: {str(datetime.now())}')"
             ]
@@ -163,63 +181,68 @@
                 "# Configure SPARCLCLIENT"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
-                "scrolled": true
+                "scrolled": true,
+                "tags": []
             },
             "outputs": [
                 {
                     "name": "stdin",
                     "output_type": "stream",
                     "text": [
                         " \u00b7\u00b7\u00b7\u00b7\u00b7\u00b7\u00b7\u00b7\n"
                     ]
                 }
             ],
             "source": [
                 "# How much output to we want to show?\n",
                 "show_help = False   # HELP for client functions\n",
                 "show_curl = True   # Show the underlying SPARCL Server API call\n",
+                "verbose = True\n",
                 "\n",
                 "server = 'https://astrosparcl.datalab.noirlab.edu'  # Public Server\n",
                 "server = 'https://sparc1.datalab.noirlab.edu'       # internal TEST Server\n",
-                "#server = 'http://localhost:8050'                    # internal DEV Server\n",
+                "server = 'http://localhost:8050'                    # internal DEV Server\n",
                 "\n",
-                "priv_dr = 'SDSS-DR17'\n",
+                "priv_dr = 'SDSS-DR17-test'\n",
+                "pub_dr = 'BOSS-DR16'\n",
                 "\n",
                 "# Authenticated Users that are never authorized for anything important.\n",
                 "# These are authenticated on both Public and Test SSO servers.\n",
                 "auth_user   = 'test_user_1@noirlab.edu'\n",
                 "unauth_user = 'test_user_2@noirlab.edu'\n",
                 "non_user    = 'test_user_3@noirlab.edu'\n",
                 "usrpw = getpass()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
-                "scrolled": true
+                "scrolled": true,
+                "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "client=(sparclclient:1.2.2b7, api:11.0, http://localhost:8050/sparc, client_hash=1223070d1915675d0589eeb5844f9c3d535498d4, verbose=False, connect_timeout=1.1, read_timeout=5400.0)\n"
+                        "apiurl=http://localhost:8050/sparc\n",
+                        "client=(sparclclient:1.2.2b8, api:11.0, http://localhost:8050/sparc, client_hash=f7bd410278bee26a425387c598dd47e80a8fcdcb, verbose=True, connect_timeout=1.1, read_timeout=5400.0)\n"
                     ]
                 }
             ],
             "source": [
                 "if show_help:\n",
                 "    help(sparcl.client.SparclClient)\n",
-                "client = sparcl.client.SparclClient(url=server, show_curl=show_curl)\n",
+                "client = sparcl.client.SparclClient(url=server, show_curl=show_curl, verbose=verbose)\n",
                 "print(f'{client=}')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -235,20 +258,22 @@
                 "## Data sets available\n",
                 "List all currently available data sets from the server/url associated with client"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16', 'SDSS-DR17'}"
+                            "{'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16', 'SDSS-DR17-test'}"
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -265,26 +290,29 @@
                 "Gets fields tagged as 'default' that are common to all data sets in the `dataset_list` passed to the function. If `dataset_list` is None (the default), the function returns the intersection of 'default' fields across all datasets currently available in the SPARC database. The following example of this function produces the same output as it would with no `dataset_list` argument because we currently only have SDSS-DR16 and BOSS-DR16 records in the SPARC database."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {
-                "scrolled": true
+                "scrolled": true,
+                "tags": []
             },
             "outputs": [],
             "source": [
                 "if show_help:\n",
                 "    client.get_default_fields?"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "['dec', 'flux', 'ra', 'sparcl_id', 'specid', 'wavelength']"
                         ]
                     },
@@ -305,15 +333,17 @@
                 "## All field names\n",
                 "Gets fields tagged as 'all' that are common to all data sets in the `dataset_list` passed to the function. If `dataset_list` is None (the default), the function returns the intersection of 'all' fields across all datasets currently available in the SPARC database.  The following example of this function produces the same output as it would with no `dataset_list` argument because we currently only have SDSS-DR16 and BOSS-DR16 records in the SPARC database."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "\u001b[0;31mSignature:\u001b[0m \u001b[0mclient\u001b[0m\u001b[0;34m.\u001b[0m\u001b[0mget_all_fields\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;34m*\u001b[0m\u001b[0;34m,\u001b[0m \u001b[0mdataset_list\u001b[0m\u001b[0;34m=\u001b[0m\u001b[0;32mNone\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n",
                             "\u001b[0;31mDocstring:\u001b[0m\n",
                             "Get fields tagged as 'all' that are in DATASET_LIST.\n",
@@ -344,15 +374,17 @@
             "source": [
                 "client.get_all_fields?"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "['ancillary_target1', 'ancillary_target2', 'anyandmask', 'anyormask', 'bluefiber', 'boss_specobj_id', 'boss_target1', 'boss_target2', 'calibflux', 'calibflux_ivar', 'chi68p', 'chunk', 'class_noqso', 'class_person', 'comments_person', 'cx', 'cy', 'cz', 'data_release', 'datasetgroup', 'dateobs', 'dateobs_center', 'dec', 'deredsn2', 'designid', 'dof', 'eboss_target0', 'eboss_target1', 'eboss_target2', 'eboss_target_id', 'elodie_bv', 'elodie_dof', 'elodie_feh', 'elodie_filename', 'elodie_logg', 'elodie_object', 'elodie_rchi2', 'elodie_sptype', 'elodie_teff', 'elodie_z', 'elodie_z_err', 'elodie_z_modelerr', 'exptime', 'fiberid', 'firstrelease', 'flux', 'fluxobjid', 'fracnsighi', 'fracnsiglo', 'fracnsigma', 'instrument', 'ivar', 'lambda_eff', 'legacy_target1', 'legacy_target2', 'marvels_target1', 'marvels_target2', 'mask', 'mjd', 'model', 'npoly', 'nspecobs', 'nturnoff', 'objid', 'plate', 'plateid', 'platequality', 'platerun', 'platesn2', 'primtarget', 'programname', 'ra', 'rchi2', 'rchi2diff', 'rchi2diff_noqso', 'redshift', 'redshift_err', 'redshift_warning', 'run1d', 'run2d', 'sectarget', 'segue1_target1', 'segue1_target2', 'segue2_target1', 'segue2_target2', 'site', 'sky', 'sn_median', 'sn_median_all', 'snturnoff', 'sourcetype', 'sparcl_id', 'spec1_g', 'spec1_i', 'spec1_r', 'spec2_g', 'spec2_i', 'spec2_r', 'specboss', 'special_target1', 'special_target2', 'specid', 'speclegacy', 'specprimary', 'specsdss', 'specsegue', 'specsegue1', 'specsegue2', 'spectroflux', 'spectroflux_ivar', 'spectrographid', 'spectroskyflux', 'spectrosynflux', 'spectrosynflux_ivar', 'spectype', 'subclass', 'subclass_noqso', 'survey', 'targetid', 'targetobjid', 'targettype', 'tcolumn', 'telescope', 'tfile', 'theta', 'thing_id', 'thing_id_targeting', 'tile', 'vdisp', 'vdisp_err', 'vdispchi2', 'vdispdof', 'vdispnpix', 'vdispz', 'vdispz_err', 'wave_sigma', 'wavelength', 'wavemax', 'wavemin', 'wcoverage', 'xfocal', 'yfocal', 'z_conf_person', 'z_err_noqso', 'z_noqso', 'z_person', 'zoffset', 'zwarning_noqso']\n"
                     ]
@@ -369,15 +401,17 @@
                 "## Version of Server API used by this client\n",
                 "The SPARCL Client you use must match the version of the SPARCL Server you use. The server is specified with the client.SparclClient `url` parameter.  If Server and Client are incompatible, when you excecute SparclClient() you will instructed to upgrade your client."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "11.0"
                         ]
                     },
@@ -461,15 +495,17 @@
                 "#### Define fields and constraints for metadata FIND\n",
                 "Define the fields we want returned (`outfields`) and the constraints (`constraints`)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "out = ['sparcl_id','specid', 'ra', 'dec', 'redshift', 'spectype', 'data_release', 'redshift_err']\n",
                 "cons = {'spectype': ['GALAXY'],\n",
                 "        'redshift': [0.5, 0.9],\n",
                 "        'data_release': ['BOSS-DR16', 'SDSS-DR16']}"
             ]
@@ -483,22 +519,25 @@
                 "The `limit` argument here is being used for demonstration purposes only, and simply returns only the first 20 results here."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
             "metadata": {
-                "scrolled": true
+                "scrolled": true,
+                "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"specid\", \"ra\", \"dec\", \"redshift\", \"spectype\", \"data_release\", \"redshift_err\"], \"search\": [[\"spectype\", \"GALAXY\"], [\"redshift\", 0.5, 0.9], [\"data_release\", \"BOSS-DR16\", \"SDSS-DR16\"]]}' 'http://localhost:8050/sparc/find/?limit=20' | python3 -m json.tool\n"
+                        "url=http://localhost:8050/sparc/find/?limit=20 sspec={'outfields': ['sparcl_id', 'specid', 'ra', 'dec', 'redshift', 'spectype', 'data_release', 'redshift_err'], 'search': [['spectype', 'GALAXY'], ['redshift', 0.5, 0.9], ['data_release', 'BOSS-DR16', 'SDSS-DR16']]}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"specid\", \"ra\", \"dec\", \"redshift\", \"spectype\", \"data_release\", \"redshift_err\"], \"search\": [[\"spectype\", \"GALAXY\"], [\"redshift\", 0.5, 0.9], [\"data_release\", \"BOSS-DR16\", \"SDSS-DR16\"]]}' 'http://localhost:8050/sparc/find/?limit=20' | python3 -m json.tool\n",
+                        "Record key counts: {'spectype': 20, 'redshift': 20, 'sparcl_id': 20, 'ra': 20, 'dec': 20, 'specid': 20, '_dr': 20, 'data_release': 20, 'redshift_err': 20}\n"
                     ]
                 }
             ],
             "source": [
                 "found = client.find(outfields=out, constraints=cons, limit=20)"
             ]
         },
@@ -510,15 +549,17 @@
             },
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
             "execution_count": 16,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
@@ -533,48 +574,314 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>spectype</th>\n",
-                            "      <th>specid</th>\n",
-                            "      <th>sparcl_id</th>\n",
-                            "      <th>redshift_err</th>\n",
                             "      <th>redshift</th>\n",
-                            "      <th>data_release</th>\n",
-                            "      <th>dec</th>\n",
                             "      <th>ra</th>\n",
+                            "      <th>dec</th>\n",
+                            "      <th>data_release</th>\n",
+                            "      <th>specid</th>\n",
+                            "      <th>redshift_err</th>\n",
+                            "      <th>spectype</th>\n",
+                            "      <th>sparcl_id</th>\n",
                             "      <th>_dr</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
+                            "      <td>0.545929</td>\n",
+                            "      <td>246.74298</td>\n",
+                            "      <td>35.985258</td>\n",
+                            "      <td>SDSS-DR16</td>\n",
+                            "      <td>1506516519029336064</td>\n",
+                            "      <td>0.000422</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>2c6c82dc-fe87-11ee-838b-08002725f1ef</td>\n",
+                            "      <td>SDSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>0.667431</td>\n",
+                            "      <td>245.40676</td>\n",
+                            "      <td>36.438884</td>\n",
+                            "      <td>SDSS-DR16</td>\n",
+                            "      <td>1506548404866541568</td>\n",
+                            "      <td>0.000026</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>3063feb6-fe87-11ee-8aa0-08002725f1ef</td>\n",
+                            "      <td>SDSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>0.502511</td>\n",
+                            "      <td>246.45702</td>\n",
+                            "      <td>36.657405</td>\n",
+                            "      <td>SDSS-DR16</td>\n",
+                            "      <td>1506572869000259584</td>\n",
+                            "      <td>0.000172</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>336d71cf-fe87-11ee-9390-08002725f1ef</td>\n",
+                            "      <td>SDSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>0.724874</td>\n",
+                            "      <td>246.89323</td>\n",
+                            "      <td>37.209662</td>\n",
+                            "      <td>SDSS-DR16</td>\n",
+                            "      <td>1506578916314212352</td>\n",
+                            "      <td>11.831918</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>342e5eaa-fe87-11ee-9047-08002725f1ef</td>\n",
+                            "      <td>SDSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>4</th>\n",
+                            "      <td>0.741196</td>\n",
+                            "      <td>247.40873</td>\n",
+                            "      <td>36.381456</td>\n",
+                            "      <td>SDSS-DR16</td>\n",
+                            "      <td>1506596508500256768</td>\n",
+                            "      <td>0.614932</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>36565b1b-fe87-11ee-b857-08002725f1ef</td>\n",
+                            "      <td>SDSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>5</th>\n",
+                            "      <td>0.675723</td>\n",
+                            "      <td>134.10755</td>\n",
+                            "      <td>28.038851</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444647351317147648</td>\n",
+                            "      <td>0.000241</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>5182df54-fe87-11ee-a660-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>6</th>\n",
+                            "      <td>0.782685</td>\n",
+                            "      <td>134.23727</td>\n",
+                            "      <td>28.084685</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444646251805519872</td>\n",
+                            "      <td>0.000242</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>51ad9b94-fe87-11ee-af3e-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>7</th>\n",
+                            "      <td>0.797439</td>\n",
+                            "      <td>133.98095</td>\n",
+                            "      <td>28.226386</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444643503026450432</td>\n",
+                            "      <td>0.000424</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>521321c8-fe87-11ee-946d-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>8</th>\n",
+                            "      <td>0.647712</td>\n",
+                            "      <td>134.54531</td>\n",
+                            "      <td>28.429551</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444641304003194880</td>\n",
+                            "      <td>0.000238</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>52643970-fe87-11ee-abb3-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>9</th>\n",
+                            "      <td>0.886086</td>\n",
+                            "      <td>134.46525</td>\n",
+                            "      <td>28.452505</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444640754247380992</td>\n",
+                            "      <td>0.000274</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>5278859e-fe87-11ee-8427-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>10</th>\n",
+                            "      <td>0.898559</td>\n",
+                            "      <td>134.43695</td>\n",
+                            "      <td>28.450988</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444640204491567104</td>\n",
+                            "      <td>0.000311</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>52913c34-fe87-11ee-844b-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>11</th>\n",
+                            "      <td>0.566015</td>\n",
+                            "      <td>133.95386</td>\n",
+                            "      <td>27.305313</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444639654735753216</td>\n",
+                            "      <td>0.000315</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>52a796f0-fe87-11ee-b337-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>12</th>\n",
+                            "      <td>0.599517</td>\n",
+                            "      <td>134.05133</td>\n",
+                            "      <td>27.381025</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444639104979939328</td>\n",
+                            "      <td>0.000412</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>52bbb47f-fe87-11ee-b8d7-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>13</th>\n",
+                            "      <td>0.812179</td>\n",
+                            "      <td>133.95189</td>\n",
+                            "      <td>27.333753</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444638555224125440</td>\n",
+                            "      <td>0.000338</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>52cfb971-fe87-11ee-be51-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>14</th>\n",
+                            "      <td>0.795586</td>\n",
+                            "      <td>134.21014</td>\n",
+                            "      <td>27.571681</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444638005468311552</td>\n",
+                            "      <td>0.000337</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>52e3cf35-fe87-11ee-b89c-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>15</th>\n",
+                            "      <td>0.554642</td>\n",
+                            "      <td>134.11568</td>\n",
+                            "      <td>27.491442</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444636356200869888</td>\n",
+                            "      <td>0.000287</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>53203e47-fe87-11ee-b26f-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>16</th>\n",
+                            "      <td>0.688878</td>\n",
+                            "      <td>134.19652</td>\n",
+                            "      <td>27.657880</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444635256689242112</td>\n",
+                            "      <td>0.000177</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>534af931-fe87-11ee-8467-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>17</th>\n",
+                            "      <td>0.638226</td>\n",
+                            "      <td>133.85629</td>\n",
+                            "      <td>28.080178</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444633057665986560</td>\n",
+                            "      <td>0.000194</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>539b0add-fe87-11ee-b991-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>18</th>\n",
+                            "      <td>0.614235</td>\n",
+                            "      <td>133.79296</td>\n",
+                            "      <td>27.907149</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "      <td>-6444632233032265728</td>\n",
+                            "      <td>0.000294</td>\n",
                             "      <td>GALAXY</td>\n",
-                            "      <td>-6444532452352045056</td>\n",
-                            "      <td>bb3d4287-8a2f-479f-9c7f-1053051e4925</td>\n",
-                            "      <td>0.000332</td>\n",
-                            "      <td>0.761637</td>\n",
+                            "      <td>53b9cd41-fe87-11ee-8132-08002725f1ef</td>\n",
+                            "      <td>BOSS-DR16</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>19</th>\n",
+                            "      <td>0.804484</td>\n",
+                            "      <td>133.87033</td>\n",
+                            "      <td>28.192423</td>\n",
                             "      <td>BOSS-DR16</td>\n",
-                            "      <td>28.063643</td>\n",
-                            "      <td>132.14379</td>\n",
+                            "      <td>-6444631408398544896</td>\n",
+                            "      <td>0.000317</td>\n",
+                            "      <td>GALAXY</td>\n",
+                            "      <td>53d853da-fe87-11ee-9f77-08002725f1ef</td>\n",
                             "      <td>BOSS-DR16</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  spectype               specid                             sparcl_id  \\\n",
-                            "0   GALAXY -6444532452352045056  bb3d4287-8a2f-479f-9c7f-1053051e4925   \n",
+                            "    redshift         ra        dec data_release               specid  \\\n",
+                            "0   0.545929  246.74298  35.985258    SDSS-DR16  1506516519029336064   \n",
+                            "1   0.667431  245.40676  36.438884    SDSS-DR16  1506548404866541568   \n",
+                            "2   0.502511  246.45702  36.657405    SDSS-DR16  1506572869000259584   \n",
+                            "3   0.724874  246.89323  37.209662    SDSS-DR16  1506578916314212352   \n",
+                            "4   0.741196  247.40873  36.381456    SDSS-DR16  1506596508500256768   \n",
+                            "5   0.675723  134.10755  28.038851    BOSS-DR16 -6444647351317147648   \n",
+                            "6   0.782685  134.23727  28.084685    BOSS-DR16 -6444646251805519872   \n",
+                            "7   0.797439  133.98095  28.226386    BOSS-DR16 -6444643503026450432   \n",
+                            "8   0.647712  134.54531  28.429551    BOSS-DR16 -6444641304003194880   \n",
+                            "9   0.886086  134.46525  28.452505    BOSS-DR16 -6444640754247380992   \n",
+                            "10  0.898559  134.43695  28.450988    BOSS-DR16 -6444640204491567104   \n",
+                            "11  0.566015  133.95386  27.305313    BOSS-DR16 -6444639654735753216   \n",
+                            "12  0.599517  134.05133  27.381025    BOSS-DR16 -6444639104979939328   \n",
+                            "13  0.812179  133.95189  27.333753    BOSS-DR16 -6444638555224125440   \n",
+                            "14  0.795586  134.21014  27.571681    BOSS-DR16 -6444638005468311552   \n",
+                            "15  0.554642  134.11568  27.491442    BOSS-DR16 -6444636356200869888   \n",
+                            "16  0.688878  134.19652  27.657880    BOSS-DR16 -6444635256689242112   \n",
+                            "17  0.638226  133.85629  28.080178    BOSS-DR16 -6444633057665986560   \n",
+                            "18  0.614235  133.79296  27.907149    BOSS-DR16 -6444632233032265728   \n",
+                            "19  0.804484  133.87033  28.192423    BOSS-DR16 -6444631408398544896   \n",
                             "\n",
-                            "   redshift_err  redshift data_release        dec         ra        _dr  \n",
-                            "0      0.000332  0.761637    BOSS-DR16  28.063643  132.14379  BOSS-DR16  "
+                            "    redshift_err spectype                             sparcl_id        _dr  \n",
+                            "0       0.000422   GALAXY  2c6c82dc-fe87-11ee-838b-08002725f1ef  SDSS-DR16  \n",
+                            "1       0.000026   GALAXY  3063feb6-fe87-11ee-8aa0-08002725f1ef  SDSS-DR16  \n",
+                            "2       0.000172   GALAXY  336d71cf-fe87-11ee-9390-08002725f1ef  SDSS-DR16  \n",
+                            "3      11.831918   GALAXY  342e5eaa-fe87-11ee-9047-08002725f1ef  SDSS-DR16  \n",
+                            "4       0.614932   GALAXY  36565b1b-fe87-11ee-b857-08002725f1ef  SDSS-DR16  \n",
+                            "5       0.000241   GALAXY  5182df54-fe87-11ee-a660-08002725f1ef  BOSS-DR16  \n",
+                            "6       0.000242   GALAXY  51ad9b94-fe87-11ee-af3e-08002725f1ef  BOSS-DR16  \n",
+                            "7       0.000424   GALAXY  521321c8-fe87-11ee-946d-08002725f1ef  BOSS-DR16  \n",
+                            "8       0.000238   GALAXY  52643970-fe87-11ee-abb3-08002725f1ef  BOSS-DR16  \n",
+                            "9       0.000274   GALAXY  5278859e-fe87-11ee-8427-08002725f1ef  BOSS-DR16  \n",
+                            "10      0.000311   GALAXY  52913c34-fe87-11ee-844b-08002725f1ef  BOSS-DR16  \n",
+                            "11      0.000315   GALAXY  52a796f0-fe87-11ee-b337-08002725f1ef  BOSS-DR16  \n",
+                            "12      0.000412   GALAXY  52bbb47f-fe87-11ee-b8d7-08002725f1ef  BOSS-DR16  \n",
+                            "13      0.000338   GALAXY  52cfb971-fe87-11ee-be51-08002725f1ef  BOSS-DR16  \n",
+                            "14      0.000337   GALAXY  52e3cf35-fe87-11ee-b89c-08002725f1ef  BOSS-DR16  \n",
+                            "15      0.000287   GALAXY  53203e47-fe87-11ee-b26f-08002725f1ef  BOSS-DR16  \n",
+                            "16      0.000177   GALAXY  534af931-fe87-11ee-8467-08002725f1ef  BOSS-DR16  \n",
+                            "17      0.000194   GALAXY  539b0add-fe87-11ee-b991-08002725f1ef  BOSS-DR16  \n",
+                            "18      0.000294   GALAXY  53b9cd41-fe87-11ee-8132-08002725f1ef  BOSS-DR16  \n",
+                            "19      0.000317   GALAXY  53d853da-fe87-11ee-9f77-08002725f1ef  BOSS-DR16  "
                         ]
                     },
                     "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -604,15 +911,16 @@
                 "**NOTE: A reasonable amount of records to request retrieval of is about 10,000. Exceeding this value may cause the retrieval to timeout or fail.**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "metadata": {
-                "scrolled": true
+                "scrolled": true,
+                "tags": []
             },
             "outputs": [],
             "source": [
                 "if show_help:\n",
                 "    client.retrieve?"
             ]
         },
@@ -625,40 +933,48 @@
                 "\n",
                 "Note that `ids` in `found_I.ids` is a property name of the Found class. It is a list of records from all records, not a field name of a record."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "# Define the fields to include in the retrieve function\n",
                 "inc = ['specid', 'data_release', 'redshift', 'flux', 'wavelength', 'model', 'ivar', 'mask', 'spectype']"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 19,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '[\"bb3d4287-8a2f-479f-9c7f-1053051e4925\"]' 'http://localhost:8050/sparc/spectras/?include=spectype%2Cmodel%2Cspecid%2Cdata_release%2Civar%2Cflux%2Cwavelength%2Cmask%2Credshift&format=pkl&dataset_list=SDSS-DR16%2CBOSS-DR16' | python3 -m json.tool\n",
-                        "CPU times: user 916 \u00b5s, sys: 2.36 ms, total: 3.28 ms\n",
-                        "Wall time: 49.6 ms\n"
+                        "Using url=\"http://localhost:8050/sparc/spectras/?include=mask%2Cspectype%2Cmodel%2Credshift%2Cwavelength%2Cspecid%2Civar%2Cdata_release%2Cflux&format=pkl&dataset_list=SDSS-DR16%2CBOSS-DR16\"\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '[\"2c6c82dc-fe87-11ee-838b-08002725f1ef\", \"3063feb6-fe87-11ee-8aa0-08002725f1ef\", \"336d71cf-fe87-11ee-9390-08002725f1ef\", \"342e5eaa-fe87-11ee-9047-08002725f1ef\", \"36565b1b-fe87-11ee-b857-08002725f1ef\", \"5182df54-fe87-11ee-a660-08002725f1ef\", \"51ad9b94-fe87-11ee-af3e-08002725f1ef\", \"521321c8-fe87-11ee-946d-08002725f1ef\", \"52643970-fe87-11ee-abb3-08002725f1ef\", \"5278859e-fe87-11ee-8427-08002725f1ef\", \"52913c34-fe87-11ee-844b-08002725f1ef\", \"52a796f0-fe87-11ee-b337-08002725f1ef\", \"52bbb47f-fe87-11ee-b8d7-08002725f1ef\", \"52cfb971-fe87-11ee-be51-08002725f1ef\", \"52e3cf35-fe87-11ee-b89c-08002725f1ef\", \"53203e47-fe87-11ee-b26f-08002725f1ef\", \"534af931-fe87-11ee-8467-08002725f1ef\", \"539b0add-fe87-11ee-b991-08002725f1ef\", \"53b9cd41-fe87-11ee-8132-08002725f1ef\", \"53d853da-fe87-11ee-9f77-08002725f1ef\"]' 'http://localhost:8050/sparc/spectras/?include=mask%2Cspectype%2Cmodel%2Credshift%2Cwavelength%2Cspecid%2Civar%2Cdata_release%2Cflux&format=pkl&dataset_list=SDSS-DR16%2CBOSS-DR16' | python3 -m json.tool\n",
+                        "Got response to post in 0.264625997049734 seconds\n",
+                        "Got 20 spectra in 0.26 seconds (76 spectra/sec)\n",
+                        "{'success': True, 'info': [\"Successfully found 20 records in dr_list=['SDSS-DR16', 'BOSS-DR16']\"], 'warnings': []}\n",
+                        "CPU times: user 7.69 ms, sys: 10 ms, total: 17.7 ms\n",
+                        "Wall time: 269 ms\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "{'status': {'success': True,\n",
-                            "  'info': [\"Successfully found 1 records in dr_list=['SDSS-DR16', 'BOSS-DR16']\"],\n",
+                            "  'info': [\"Successfully found 20 records in dr_list=['SDSS-DR16', 'BOSS-DR16']\"],\n",
                             "  'warnings': []}}"
                         ]
                     },
                     "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -670,32 +986,34 @@
                 "                          dataset_list=['SDSS-DR16','BOSS-DR16'])\n",
                 "results.info"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'redshift': 0.761636912822723,\n",
+                            "{'redshift': 0.5459291338920593,\n",
+                            " 'specid': 1506516519029336064,\n",
                             " 'spectype': 'GALAXY',\n",
-                            " 'specid': -6444532452352045056,\n",
-                            " 'data_release': 'BOSS-DR16',\n",
-                            " 'model': array([-0.01559776, -0.01588696, -0.01609746, ...,  0.94615489,\n",
-                            "         0.92513317,  0.8983984 ]),\n",
-                            " 'mask': array([88080384, 88080384, 88080384, ..., 83886080, 83886080, 83886080]),\n",
+                            " 'data_release': 'SDSS-DR16',\n",
+                            " '_dr': 'SDSS-DR16',\n",
                             " 'ivar': array([0., 0., 0., ..., 0., 0., 0.]),\n",
-                            " 'flux': array([0.19426258, 0.19424935, 0.19423614, ..., 0.27637786, 0.2763944 ,\n",
-                            "        0.27641097]),\n",
-                            " 'wavelength': array([ 3580.13991843,  3580.96437103,  3581.78901348, ...,\n",
-                            "        10368.11964061, 10370.50726326, 10372.89543574]),\n",
-                            " '_dr': 'BOSS-DR16'}"
+                            " 'mask': array([16777216, 16777216, 16777216, ..., 16777216, 16777216, 16777216]),\n",
+                            " 'flux': array([1.23176956, 1.23148859, 1.23120809, ..., 4.00684404, 4.00690508,\n",
+                            "        4.00696611]),\n",
+                            " 'wavelength': array([3794.89706208, 3795.77097003, 3796.64507922, ..., 9217.22098659,\n",
+                            "        9219.34357452, 9221.46665124]),\n",
+                            " 'model': array([0.34971759, 0.35207507, 0.35443148, ..., 2.31373858, 2.30945611,\n",
+                            "        2.30356026])}"
                         ]
                     },
                     "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -709,41 +1027,43 @@
             "source": [
                 "## Plot spectra"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 21,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<matplotlib.legend.Legend at 0x7f47bfced810>"
+                            "<matplotlib.legend.Legend at 0x7fd1f96db7c0>"
                         ]
                     },
                     "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "a2854906526c42f49c1fc769732e5228",
+                            "model_id": "84c674d2919c4a9f804a778cb667076f",
                             "version_major": 2,
                             "version_minor": 0
                         },
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAyAAAAGQCAYAAABWJQQ0AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/SrBM8AAAACXBIWXMAAA9hAAAPYQGoP6dpAAByPUlEQVR4nO3dd3hTZcMG8PtkNN0ttIW20MEou5S9N8hQX1HBgYKAijh4RUEFXICIiOuT162oIAIuFBQRkC1lyt6UXVoKLaVNdzOe7480adKMrjTpuH/XhbYnJzlPetLT5z7PkoQQAkRERERERC4gc3cBiIiIiIio7mAAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil1G4uwBUTK/XIzk5GX5+fpAkyd3FISIiIqIShBDIyspCeHg4ZDLey68IBpBqJDk5GREREe4uBhERERGVIjExEY0bN3Z3MWokBpBqxM/PD4DhA+3v7+/m0hARERFRSWq1GhEREaZ6G5UfA0g1Yux25e/vzwBCREREVI2xu3zFseMaERERERG5DAMIERERERG5DAMIERERERG5DAMIERERERG5DAMIERERERG5DAMIERERERG5DKfhrQU0Gg10Op27i0EupFQqIZfL3V0MIiIionJjAKnB1Go10tLSUFBQ4O6ikItJkoSAgACEhoZyHnIiIiKqURhAaii1Wo2kpCT4+voiODgYSqWSFdE6QgiBnJwcpKamwsvLC4GBge4uEhEREVGZMYDUUGlpafD19UXjxo0ZPOogLy8vFBQU4MaNGwgICOBngIiI6gy9XkAm49+9moyD0GsgjUaDgoICVjzrOH9/f+h0Oo7/ISKiOiP+XBri3tiI348ku7soVAkMIDWQscKpVCrdXBJyJ4XC0ICp1WrdXBIiIiLXGPf1XmTla/HsykPuLgpVAgNIDcbWj7qN55+IiIhqIgYQIiIiIiJyGQYQqpE0Gg3mzJmDmJgYqFQqSJKEDz/8EJIkYcKECe4uHhERERHZwVmwqEZ6//33MXfuXPTr1w/3338/lEolhg8fjueff97dRSMiIqIqIkkSIIS7i0GVxABCNdLatWvh6+uLv//+Gx4eHgCAS5cuubdQRERERFQqdsGiGik5ORlBQUGm8EFERERENQMDCNUoc+bMgSRJuHjxIi5fvgxJkiBJEqKjo+0+Jzo62u7jAwYMsJhN6ubNm2jcuDH8/Pxw7tw5i30dPUZEREREZcMuWFSjDBgwAADw4YcfAgCee+45AEBgYKBTXj8oKAjfffcdbrvtNjz00EOIj483rbfy2GOPISkpCUuWLEHz5s2dcjwiIiKiuoYBhGqUAQMGYMCAAViyZAkAQ4uIkbPGgAwaNAgvvfQS3n77bbz66qtYuHAhPv30U6xZswZjxozB+PHjnXIcIiIiorqIAaSWEUIgT6NzdzEc8lLKq/0iem+88QY2b96M9957D40bN8aMGTMQHR2Nzz//3N1FIyIiqrOqd+2ByooBpJbJ0+jQ5vUN7i6GQyffGAZvj+r90VMqlVi5ciU6dOiAZ599FnK5HMuXL4e/v7+7i0ZERERUo3EQOpEdTZs2RVxcHACgc+fO6NWrl5tLRERERFTzVe/b0FRuXko5Tr4xzN3FcMhLKXfp8WQyGQoLC20+lpmZafd5H3zwAeLj4xEUFIR9+/bh008/xdNPP11VxSQiIqJSVPMe3FRGDCC1jCRJ1b57k6vVq1cPx44dg1arhUJR/LPJyclBQkKCzeccOnQIL7/8Mlq2bImtW7eid+/eeOGFF9C/f3+0bdvWVUUnIiIiqnXYBYtqva5du0Kj0WD58uWmbUIIzJo1Czk5OVb75+TkYMyYMQCAlStXIiwsDCtWrIBGo8GYMWOQn5/vsrITERER1TYMIFTrTZkyBR4eHnj88ccxduxYPP/88+jatSvWrVtnGuNhburUqThz5gzeeustdOzYEQDQo0cPzJ49G8eOHcOLL77o6rdAREREVGswgFCt165dO6xfvx6dO3fGL7/8gmXLlqFNmzbYtWuX1QKGq1atwtdff43bbrsN06ZNs3js5ZdfRr9+/fDxxx9j7dq1LnwHRERERLUHBwtQjWRr0cHo6GgIIWzuP3DgQOzZs8dq+7Zt2yy+HzVqlN3XkMlk2L59e7nLSkRERETF2AJCRERERDWCxKUIawUGECIiIiKqcfZdTHd3EaiCGECIiIiIqMa5/4vd7i4CVRADCBERERERuQwDCBERERERuQwDCBERERERuQwDCBERERHVDJwEq1ZgACEiIiIiIpdhACEiIiIiIpdhACEiIiKiGoE9sGoHBhAiIiIiInIZBhAiIiIiInIZBhAiIiIiInIZBhAiJ9m2bRskScKcOXMq9TrR0dGIjo52SpmIiIiIqhsGkBK+//57TJ48GV26dIFKpYIkSViyZInd/dVqNaZNm4aoqCioVCpER0fjxRdfRHZ2tusKTURERERUQyjcXYDq5tVXX8Xly5cRHByMsLAwXL582e6+OTk56N+/Pw4fPoyhQ4dizJgxOHToEN577z1s374dO3bsgKenpwtLT0RERFR7SZwGq1ZgC0gJixcvxqVLl5Camoonn3zS4b7vvPMODh8+jBkzZmDDhg14++23sWHDBsyYMQP79+/H//3f/7mo1ERERERENQMDSAlDhgxBVFRUqfsJIbB48WL4+vritddes3jstddeg6+vLxYvXlxVxazzzMdb7Nq1CwMHDoSfnx9CQkLw9NNPIy8vDwDw559/omfPnvDx8UHDhg3x0ksvQavVWryWVqvFBx98gLi4OHh5eSEgIAADBw7EH3/8YfPYeXl5mDlzJiIiIuDp6Yl27drhq6++cljeixcv4vHHH0dkZCRUKhXCwsIwYcIEhy1sRERERLURA0gFJSQkIDk5Gb1794aPj4/FYz4+PujduzcuXLiAxMREN5Wwbti7dy8GDx6MgIAATJ48GZGRkfjss88wadIk/Pjjjxg9ejSioqIwefJkBAYG4t1338Vbb71ler4QAqNHj8b06dORn5+PZ555Bg899BCOHDmCu+66y6oVS6/X46677sLChQtRr149TJ06FT169MDz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iIiIyAk4AqT24BgQJ8vJycGJEyfg4+OD4OBgdxeHiIiIiKhaYQCpgKysLJw9e9Zqe15eHiZNmoSsrCzcf//9UCjqdAMTERERkfOwCaTWYA25Am7evIlWrVqha9euaN26NUJDQ3H9+nVs2rQJV69eRWxsLN599113F5OIiIiIqNphAKmA+vXr4+mnn8a+ffuwbt063Lp1C15eXmjdujWeffZZTJkyBV5eXu4uJhEREVGtwQaQ2oMBpAL8/f3x8ccfu7sYREREREQ1DseAEBEREVG1x5XQaw8GECIiIiIichkGECIiIiKq9sIDOb62tmAAISIiIqJqa8Wk7hjapiEWjop1d1HISTgInYiIiIiqrV7NgtGrGRd3rk0YQKhM7u3YCC/f0drdxSAiIiKiGo4BhBx6/744bDubigWjYqFSyN1dHCIiIiKq4RhAyKFRnRtjVOfG7i4GEREREdUSHIROREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCVgK8lO4uAhERERHVUgwgZGXFpO7o3qQ+Vj3Vy91FISIiIqJaRuHuAlD10zY8AD9O7unuYhARERFRLcQWECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGkCKHDx/Gyy+/jGHDhiEkJASSJGHAgAGlPm/58uXo1q0bfHx8UK9ePdx55504ePBg1ReYiIiIiKgGYgApsnr1aixYsADbtm1DaGhomZ4zf/58jB07Fjdu3MCTTz6J++67Dzt27ECvXr0QHx9fxSUmIiIiIqp5FO4uQHVx33334a677kJsbCxu3ryJsLAwh/snJCRgzpw5aNGiBfbt24eAgAAAwNNPP40ePXpg0qRJOH78OGQyZjwiIiIiIiPWjou0bdsWnTp1glKpLNP+3377LbRaLV555RVT+ACADh06YMyYMTh1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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAyAAAAGQCAYAAABWJQQ0AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/SrBM8AAAACXBIWXMAAA9hAAAPYQGoP6dpAACFfklEQVR4nO3dd3gUVdsG8Hu2JqQCCRAgDQhI70gvUlUUFURREVB4bXwWVBAEaQKiKGIvqCCCDRQUUHoNvQSQGiDUAKEmJKRsOd8fyW62l2Szu0nu33VxkcycnTk7mZ2dZ845z5GEEAJEREREREReIPN1BYiIiIiIqPxgAEJERERERF7DAISIiIiIiLyGAQgREREREXkNAxAiIiIiIvIaBiBEREREROQ1DECIiIiIiMhrGIAQEREREZHXMAAhIiIiIiKvYQBCRERERERewwCEiIiIiIi8hgEIERERERF5DQMQIiIiIiLyGgYgRERERETkNQxAiIiIiIjIaxiAEBERERGR1zAAISIiIiIir2EAQkREREREXsMAhIiIiIiIvIYBCBEREREReQ0DECIiIiIi8hoGIERERERE5DUMQIiIiIiIyGsYgBARERERkdcwACEiIiIiIq9hAEJERERERF7DAISIiIiIiLyGAQgREREREXkNAxAiIiIiIvIaBiBEREREROQ1DECIiIiIiMhrGIAQEREREZHXMAAhIiIiIiKvYQBCRERERERewwCEiIiIiIi8hgEIERERERF5DQMQIiIiIiLyGgYgRERERETkNQxAiIiIiIjIaxiAEBERERGR1zAAISIiIiIir2EAQkREREREXsMAhIiIiIiIvIYBCBEREREReQ0DECIiIiIi8hoGIERERERE5DUKX1eACun1eqSmpiIkJASSJPm6OkRERERkQQiB27dvo3r16pDJ+Cy/KBiA+JHU1FRER0f7uhpERERE5MT58+dRs2ZNX1ejVGIA4kdCQkIA5J/QoaGhPq4NEREREVnKyMhAdHS08b6N3McAxI8Yul2FhoYyACEiIiLyY+wuX3TsuEZERERERF7DAISIiIiIiLyGAQgREREREXkNAxAiIiIiIvIaBiBEREREROQ1DECIiIiIiMhrmIaXiIiIqIBOp4NGo/F1NciL5HI5lEqlr6tRrjAAISIionJPCIHLly8jPT0dQghfV4e8TK1WIyIigvOweQkDECIiIir30tPTcevWLURGRiIoKIiTzJUTQghoNBqkp6fj4sWLAMAgxAsYgBARlRF6vYBMxpsmIncJIZCWlobQ0FBERET4ujrkZYGBgQgJCcGFCxdw7do1BiBewEHoRERlQI5Gh66zNuLVX/b7uipEpY5Op4NOp+ONZzkmSRLCwsKQm5vLMUBewACEiKgMWHPkCs7duIOlSam+rgpRqaPVagEACgU7hpRnhoHoOp3OxzUp+xiAEBEREQEc91HO8e/vPQxAiIiIiIjIaxiAEBGVAUwaSkTFodFoMGnSJCQkJECtVkOSJHz88ceQJAlDhw71dfWojGFnRyIiIqJy7sMPP8TkyZPRuXNnDBw4EEqlEn369MFrr73m66pRGcQAhIioDGDPZSIqjuXLlyM4OBhr1qyBSqUCAJw5c8a3laIyi12wiIiIiMq51NRUVK5c2Rh8EJUkBiBERGUAx4AQUVFMmjQJkiQhJSUFZ8+ehSRJkCQJcXFxdl8TFxdnd33Xrl3Nskldv34dNWvWREhICE6ePGlW1tE6KtvYBYuIiIionOratSsA4OOPPwYAvPrqqwCA8PBwj2y/cuXK+PHHH9GzZ0888cQTSExMNM638eyzz+LixYuYN28e6tSp45H9UenAAISIiIionOratSu6du2KefPmAchvETHw1BiQe+65B6NHj8Z7772H8ePHY+bMmfjiiy+wbNkyDBo0CEOGDPHIfqj0YABCRFQGcBA6kecJIZCt8f9ZsQOVcr+fRG/KlClYt24dZs2ahZo1a2LMmDGIi4vDV1995euqkQ8wACEiKgM4BoTI87I1OjR4Z5Wvq+HUkSm9UUHl37d0SqUSP//8M5o1a4aXX34ZcrkcCxcuRGhoqK+rRj7AQehEREREVOJq1aqFpk2bAgBatmyJ9u3b+7hG5Cv+HS4TERER+UigUo4jU3r7uhpOBSrlXt2fTCZDXl6ezXXp6el2X/fRRx8hMTERlStXxq5du/DFF1/gxRdfLKlqkh9jAEJERERkgyRJft+1yRcqVqyIQ4cOQavVQqEoPD5ZWVlITk62+Zr9+/dj3LhxqFevHjZs2IAOHTrgjTfeQJcuXdCwYUNvVZ38BLtgEREREZHLWrduDY1Gg4ULFxqXCSEwduxYZGVlWZXPysrCoEGDAAA///wzoqKisGjRImg0GgwaNAg5OTleqzv5BwYgREREROSykSNHQqVSYfjw4Xjqqafw2muvoXXr1li5cqVxjIepV155BcePH8f06dPRvHlzAEDbtm0xceJEHDp0CG+++aa33wL5GAMQExcvXsTHH3+MXr16ISYmBiqVCtWqVUP//v2xc+dOm6/JyMjAqFGjEBsbC7Vajbi4OLz55pvIzMz0cu2JiIiISl6jRo3w77//omXLlli8eDEWLFiABg0aYNu2bVYTGC5ZsgTfffcdevbsiVGjRpmtGzduHDp37ozPPvsMy5cv9+I7IF+ThBDM3ljgrbfewsyZM1G7dm107doVkZGRSE5OxtKlSyGEwKJFi/DYY48Zy2dlZaFjx45ISkpCr1690Lx5c+zfvx+rV69G69atsXnzZgQEBLi8/4yMDISFhSE9PZ1p6YjILX8dSMXLP+8HAJx5734f14aodMnJyUFKSgri4+Pd+t6mssXV84D3a8XHkVUm2rRpg40bN6JLly5my7ds2YLu3bvjhRdewEMPPQS1Wg0AeP/995GUlIQxY8bgvffeM5Y3BDKzZ8/G2LFjvfoeiIiIiIj8GbtgmXjkkUesgg8A6NSpE7p164abN2/i0KFDAPIHW82dOxfBwcGYMGGCWfkJEyYgODgYc+fO9Uq9iYiIiIhKCwYgLlIqlQBgTDeXnJyM1NRUdOjQAUFBQWZlg4KC0KFDB5w+fRrnz5/3el2JiIiIiPwVAxAXnDt3DmvXrkVUVBQaN24MAMY81wkJCTZfY1huLx82EREREVF5xDEgTmg0GgwePBi5ubmYOXMm5PL82UYNM32GhYXZfJ1hUJKjGUFzc3ORm5tr/D0jI8NT1SYiIiIi8ktsAXFAr9dj6NCh2Lx5M0aMGIHBgwd7dPszZsxAWFiY8V90dLRHt09ERERE5G8YgNih1+vxzDPPYNGiRXjqqafw1Vdfma03tHzYa+EwtGbYayEBgLFjxyI9Pd34j+NFiIiIiKisYxcsG/R6PYYNG4Yff/wRgwYNwrx58yCTmcdqzsZ4OBsjAgBqtdqY0peIqDg4pRMREZUWbAGxYBp8PPbYY1iwYIFx3IephIQEVK9eHYmJicjKyjJbl5WVhcTERMTHx7NbFRERERGRCQYgJgzdrn788Uc8+uij+Omnn2wGHwAgSRKGDx+OzMxMTJ061Wzd1KlTkZmZiREjRnij2kREkCTJ11UgIiJyCbtgmZgyZQrmz5+P4OBg1K1bF++++65VmYceegjNmjUDAIwePRrLli3DzJkzsX//frRo0QL79u3D6tWr0bp1a7z66qvefQNEVG6xCxYREZUWDEBMnDlzBgCQmZmJadOm2SwTFxdnDECCgoKwadMmTJo0CUuWLMGGDRsQFRWF119/HRMnTkRgYKCXak5EREREVDowADExb948zJs3z63XhIWFYfbs2Zg9e3bJVIqIiIiIqAzhGBAiojKAY0CIqKzZuHEjJEnCpEmTirWduLg4xMXFeaRO5BkMQIiIygCOASEiotKCAQgREREREXkNAxAiIiIiIvIaBiBERERE5ZzpeItt27ahW7duCAkJQWRkJF588UVkZ2cDAFasWIF27dohKCgIVatWxejRo6HVas22pdVq8dFHH6Fp06YIDAxEWFgYunXrhr///tvmvrOzs/HWW28hOjoaAQEBaNSoEb799luH9U1JScHw4cMRExMDtVqNqKgoDB06FGfPnvXMAaESxQCEiIiIiAAAO3fuRPfu3REWFobnnnsOMTEx+PLLLzFixAj8+uuvGDBgAGJjY/Hcc88hPDwcH3zwAaZPn258vRACAwYMwOuvv46cnBy89NJLeOKJJ3DgwAE8+OCDVllD9Xo9HnzwQcycORMVK1bEK6+8grZt2+K1117Dhx9+aLeOzZs3x/z589GyZUu88sor6NSpExYuXIg2bdrg9OnTJXqMqPiYhpeIiIjIFiEAzR1f18I5ZQXAQ5nw/v33XyxduhT9+vUDAGg0GrRq1QqLFi3CqlWrsHnzZrRu3RoAMHnyZNSpUwdz5szB2LFjoVQqsWDBAixbtgxdunTB6tWroVKpAABjx45Fy5YtMXr0aPTr1w+1atUCAPz4449Yu3Yt+vTpg+XLl0MulwMAXnnlFbRq1cqqfhqNBo8//jj0ej127dqF5s2bG9dt3boVXbt2xSuvvGK3tYX8AwMQIiIiIls0d4Dp1X1dC+fGpQKqII9sqlu3bsbgAwCUSiUGDBiAgwcP4oEHHjAGHwAQEhKCvn374vvvv8eFCxcQHx+P+fPnAwDef/99Y/ABADExMXjttdfw9ttvY+HChZgwYQKA/AAEAKZNm2YMPgCgcePGGDx4ML777juz+i1fvhxnzpzBlClTzIIPAOjYsSP69euHpUuXIiMjA6GhoR45JuR5DECIiIiICADQrFkzq2VRUVFO16WmpiI+Ph779+9HhQoV0KZNG6uy3bp1AwAkJSUZlx04cABBQUFo0aKFVflOnTpZBSA7duwAABw/ftzm/CCXL1+GXq/HiRMnbLagkH9gAEJERERki7JCfuuCv1NW8NimbLUaKBQKp+s0Gg0AICMjA9HR0Ta3bQhWMjIyjMvS09Ptlq9atarVshs3bgAAFi5caPc9AEBWVpbD9eRbDECIiIiIbJEkj3VtKi9CQ0ORlpZmc93ly5eNZQzCwsJw9epVm+WvXLlic/sA8Pfff6Nv377FrS75CLNgEREREZFHNG/eHHfu3MGuXbus1m3cuBGAeVeupk2bIisrC/v27bMqv2XLFqtld999NwBg+/btnqkw+QQDECIiIiLyiCFDhgDIz3pl6JYFAOfPn8dHH30EhUKBJ5980rh88ODBAIC3334bOp3OuPzQoUNYsGCB1fb79euHmJgYfPTRR9i8ebPVeo1Gg61bt3rs/VDJYBcsIiIiIvKIwYMH448//sCyZcvQpEkT9O3bF1lZWfj1119x48YNfPjhh8YUvEB+wLJo0SL8+++/aN68Oe69917cuHEDP//8M3r16oXly5ebbV+tVmPx4sW499570aVLF9xzzz1o3LgxJEnC2bNnsWXLFlSuXBnHjh3z9lsnNzAAISIiIiKPkCQJixcvxpw5czB//nx8+umnUKlUaNGiBUaNGoUHH3zQrLxMJsOyZcswefJkLFy4EHPmzEHt2rUxe/ZsJCQkWAUgANC6dWscOHAAH3zwAVauXInExESo1WrUqFEDDz30EAYNGuStt0tFJAkhhK8rQfkyMjIQFhaG9PR05q4mIrcsS7qIV35JAgCcee9+31aGqJTJyclBSkoK4uPjERAQ4OvqkI+4eh7wfq34OAaEiIiIiIi8hgEIERERERF5DQMQIiIiIiLyGgYgRERERETkNQxAiIiIiIjIaxiAEBERERGR1zAAISIiIiIir2EAQkRERASAU6OVb/z7ew8DECIiIirXFAoFAECr1fq4JuRLGo0GACCXy31ck7KPAQgRERGVa3K5HHK5HBkZGb6uCvmIEALp6elQq9VQKpW+rk6Zp/B1BYiIiIh8SZIkVKlSBZcuXYJarUZQUBAkSfJ1tcgLhBDQaDRIT09HZmYmatSo4esqlQsMQIiIiKjcCwsLQ3Z2Nq5du4arV6/6ujrkZWq1GjVq1EBoaKivq1IuMAAhIiKick+SJERFRaFKlSrGsQBUPsjlcna78jIGIEREREQFDONBiKjkcBA6ERERERF5DQMQIiIiIiLyGgYgRERERETkNQxAiIiIiIjIaxiAEBERERGR1zAAISIiIiIir2EAQkREREREXsMAhIiIiIiIvIYBCBFRGSCEr2tARETkGgYgRERERETkNQxAiIiIiIjIaxiAEBGVAZLk6xoQERG5hgEIEVEZwDEgRERUWjAAISIiIiIir2EAQkREREREXsMAhIioDOAYECIiKi0YgBARlQEcA0JERKUFAxAiIiIiIvIaBiBEREREROQ1DECIiIiIiMhrGIAQEREREZHXMAAhIiIiIiKvYQBCRERERERewwCEiIiIiIi8hgEIERERERF5DQMQIiIiIiLyGgYgRERERETkNQxAiIjKAAHh6yoQERG5hAEIERERERF5DQMQIqIyQILk6yoQERG5hAEIERERERF5DQMQIqIygGNAiIiotGAAQkREREREXsMAhIioDOAYECIiKi0YgBARERERkdcwACEiKgM4BoSIiEoLBiBEREREROQ1DECIiIiIiMhrGIAQEREREZHXMACx8NNPP+G5555Dq1atoFarIUkS5s2bZ7d8RkYGRo0ahdjYWKjVasTFxeHNN99EZmam9ypNRERERFRKKHxdAX8zfvx4nD17FhEREYiKisLZs2ftls3KykKXLl2QlJSEXr16YdCgQdi/fz9mzZqFTZs2YfPmzQgICPBi7YmIiIiI/BtbQCzMnTsXZ86cwdWrV/H88887LPv+++8jKSkJY8aMwapVq/Dee+9h1apVGDNmDHbv3o3Zs2d7qdZERIWEYEYsIiLyXwxALPTo0QOxsbFOywkhMHfuXAQHB2PChAlm6yZMmIDg4GDMnTu3pKpJRERERFQqMQApouTkZKSmpqJDhw4ICgoyWxcUFIQOHTrg9OnTOH/+vI9qSERERETkfxiAFFFycjIAICEhweZ6w3JDOSIiIiIi4iD0IktPTwcAhIWF2VwfGhpqVs6W3Nxc5ObmGn/PyMjwYA2JiIiIiPwPW0B8aMaMGQgLCzP+i46O9nWViKgM4Bh0IvJ3By/cwpu/H0BaRo6vq0I+wACkiAwtH/ZaOAytGfZaSABg7NixSE9PN/7jeBEiIiIqDx78LBG/772A138/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",
                         "text/html": [
                             "\n",
                             "            <div style=\"display: inline-block;\">\n",
                             "                <div class=\"jupyter-widgets widget-label\" style=\"text-align: center;\">\n",
                             "                    Figure\n",
                             "                </div>\n",
-                            "                <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAyAAAAGQCAYAAABWJQQ0AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/SrBM8AAAACXBIWXMAAA9hAAAPYQGoP6dpAAByPUlEQVR4nO3dd3hTZcMG8PtkNN0ttIW20MEou5S9N8hQX1HBgYKAijh4RUEFXICIiOuT162oIAIuFBQRkC1lyt6UXVoKLaVNdzOe7480adKMrjTpuH/XhbYnJzlPetLT5z7PkoQQAkRERERERC4gc3cBiIiIiIio7mAAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil2EAISIiIiIil1G4uwBUTK/XIzk5GX5+fpAkyd3FISIiIqIShBDIyspCeHg4ZDLey68IBpBqJDk5GREREe4uBhERERGVIjExEY0bN3Z3MWokBpBqxM/PD4DhA+3v7+/m0hARERFRSWq1GhEREaZ6G5UfA0g1Yux25e/vzwBCREREVI2xu3zFseMaERERERG5DAMIERERERG5DAMIERERERG5DAMIERERERG5DAMIERERERG5DAMIERERERG5DKfhrQU0Gg10Op27i0EupFQqIZfL3V0MIiIionJjAKnB1Go10tLSUFBQ4O6ikItJkoSAgACEhoZyHnIiIiKqURhAaii1Wo2kpCT4+voiODgYSqWSFdE6QgiBnJwcpKamwsvLC4GBge4uEhEREVGZMYDUUGlpafD19UXjxo0ZPOogLy8vFBQU4MaNGwgICOBngIiI6gy9XkAm49+9moyD0GsgjUaDgoICVjzrOH9/f+h0Oo7/ISKiOiP+XBri3tiI348ku7soVAkMIDWQscKpVCrdXBJyJ4XC0ICp1WrdXBIiIiLXGPf1XmTla/HsykPuLgpVAgNIDcbWj7qN55+IiIhqIgYQIiIiIiJyGQYQqpE0Gg3mzJmDmJgYqFQqSJKEDz/8EJIkYcKECe4uHhERERHZwVmwqEZ6//33MXfuXPTr1w/3338/lEolhg8fjueff97dRSMiIqIqIkkSIIS7i0GVxABCNdLatWvh6+uLv//+Gx4eHgCAS5cuubdQRERERFQqdsGiGik5ORlBQUGm8EFERERENQMDCNUoc+bMgSRJuHjxIi5fvgxJkiBJEqKjo+0+Jzo62u7jAwYMsJhN6ubNm2jcuDH8/Pxw7tw5i30dPUZEREREZcMuWFSjDBgwAADw4YcfAgCee+45AEBgYKBTXj8oKAjfffcdbrvtNjz00EOIj483rbfy2GOPISkpCUuWLEHz5s2dcjwiIiKiuoYBhGqUAQMGYMCAAViyZAkAQ4uIkbPGgAwaNAgvvfQS3n77bbz66qtYuHAhPv30U6xZswZjxozB+PHjnXIcIiIiorqIAaSWEUIgT6NzdzEc8lLKq/0iem+88QY2b96M9957D40bN8aMGTMQHR2Nzz//3N1FIyIiqrOqd+2ByooBpJbJ0+jQ5vUN7i6GQyffGAZvj+r90VMqlVi5ciU6dOiAZ599FnK5HMuXL4e/v7+7i0ZERERUo3EQOpEdTZs2RVxcHACgc+fO6NWrl5tLRERERFTzVe/b0FRuXko5Tr4xzN3FcMhLKXfp8WQyGQoLC20+lpmZafd5H3zwAeLj4xEUFIR9+/bh008/xdNPP11VxSQiIqJSVPMe3FRGDCC1jCRJ1b57k6vVq1cPx44dg1arhUJR/LPJyclBQkKCzeccOnQIL7/8Mlq2bImtW7eid+/eeOGFF9C/f3+0bdvWVUUnIiIiqnXYBYtqva5du0Kj0WD58uWmbUIIzJo1Czk5OVb75+TkYMyYMQCAlStXIiwsDCtWrIBGo8GYMWOQn5/vsrITERER1TYMIFTrTZkyBR4eHnj88ccxduxYPP/88+jatSvWrVtnGuNhburUqThz5gzeeustdOzYEQDQo0cPzJ49G8eOHcOLL77o6rdAREREVGswgFCt165dO6xfvx6dO3fGL7/8gmXLlqFNmzbYtWuX1QKGq1atwtdff43bbrsN06ZNs3js5ZdfRr9+/fDxxx9j7dq1LnwHRERERLUHBwtQjWRr0cHo6GgIIWzuP3DgQOzZs8dq+7Zt2yy+HzVqlN3XkMlk2L59e7nLSkRERETF2AJCRERERDWCxKUIawUGECIiIiKqcfZdTHd3EaiCGECIiIiIqMa5/4vd7i4CVRADCBERERERuQwDCBERERERuQwDCBERERERuQwDCBERERHVDJwEq1ZgACEiIiIiIpdhACEiIiIiIpdhACEiIiKiGoE9sGoHBhAiIiIiInIZBhAiIiIiInIZBhAiIiIiInIZBhAiJ9m2bRskScKcOXMq9TrR0dGIjo52SpmIiIiIqhsGkBK+//57TJ48GV26dIFKpYIkSViyZInd/dVqNaZNm4aoqCioVCpER0fjxRdfRHZ2tusKTURERERUQyjcXYDq5tVXX8Xly5cRHByMsLAwXL582e6+OTk56N+/Pw4fPoyhQ4dizJgxOHToEN577z1s374dO3bsgKenpwtLT0RERFR7SZwGq1ZgC0gJixcvxqVLl5Camoonn3zS4b7vvPMODh8+jBkzZmDDhg14++23sWHDBsyYMQP79+/H//3f/7mo1ERERERENQMDSAlDhgxBVFRUqfsJIbB48WL4+vritddes3jstddeg6+vLxYvXlxVxazzzMdb7Nq1CwMHDoSfnx9CQkLw9NNPIy8vDwDw559/omfPnvDx8UHDhg3x0ksvQavVWryWVqvFBx98gLi4OHh5eSEgIAADBw7EH3/8YfPYeXl5mDlzJiIiIuDp6Yl27drhq6++cljeixcv4vHHH0dkZCRUKhXCwsIwYcIEhy1sRERERLURA0gFJSQkIDk5Gb1794aPj4/FYz4+PujduzcuXLiAxMREN5Wwbti7dy8GDx6MgIAATJ48GZGRkfjss88wadIk/Pjjjxg9ejSioqIwefJkBAYG4t1338Vbb71ler4QAqNHj8b06dORn5+PZ555Bg899BCOHDmCu+66y6oVS6/X46677sLChQtRr149TJ06FT169MDz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iIiIyAk4AqT24BgQJ8vJycGJEyfg4+OD4OBgdxeHiIiIiKhaYQCpgKysLJw9e9Zqe15eHiZNmoSsrCzcf//9UCjqdAMTERERkfOwCaTWYA25Am7evIlWrVqha9euaN26NUJDQ3H9+nVs2rQJV69eRWxsLN599113F5OIiIiIqNphAKmA+vXr4+mnn8a+ffuwbt063Lp1C15eXmjdujWeffZZTJkyBV5eXu4uJhEREVGtwQaQ2oMBpAL8/f3x8ccfu7sYREREREQ1DseAEBEREVG1x5XQaw8GECIiIiIichkGECIiIiKq9sIDOb62tmAAISIiIqJqa8Wk7hjapiEWjop1d1HISTgInYiIiIiqrV7NgtGrGRd3rk0YQKhM7u3YCC/f0drdxSAiIiKiGo4BhBx6/744bDubigWjYqFSyN1dHCIiIiKq4RhAyKFRnRtjVOfG7i4GEREREdUSHIROREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCREREREQuwwBCVgK8lO4uAhERERHVUgwgZGXFpO7o3qQ+Vj3Vy91FISIiIqJaRuHuAlD10zY8AD9O7unuYhARERFRLcQWECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGECIiIiIichkGkCKHDx/Gyy+/jGHDhiEkJASSJGHAgAGlPm/58uXo1q0bfHx8UK9ePdx55504ePBg1ReYiIiIiKgGYgApsnr1aixYsADbtm1DaGhomZ4zf/58jB07Fjdu3MCTTz6J++67Dzt27ECvXr0QHx9fxSUmIiIiIqp5FO4uQHVx33334a677kJsbCxu3ryJsLAwh/snJCRgzpw5aNGiBfbt24eAgAAAwNNPP40ePXpg0qRJOH78OGQyZjwiIiIiIiPWjou0bdsWnTp1glKpLNP+3377LbRaLV555RVT+ACADh06YMyYMTh1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' width=800.0/>\n",
+                            "                <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAyAAAAGQCAYAAABWJQQ0AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/SrBM8AAAACXBIWXMAAA9hAAAPYQGoP6dpAACFfklEQVR4nO3dd3gUVdsG8Hu2JqQCCRAgDQhI70gvUlUUFURREVB4bXwWVBAEaQKiKGIvqCCCDRQUUHoNvQSQGiDUAKEmJKRsOd8fyW62l2Szu0nu33VxkcycnTk7mZ2dZ845z5GEEAJEREREREReIPN1BYiIiIiIqPxgAEJERERERF7DAISIiIiIiLyGAQgREREREXkNAxAiIiIiIvIaBiBEREREROQ1DECIiIiIiMhrGIAQEREREZHXMAAhIiIiIiKvYQBCRERERERewwCEiIiIiIi8hgEIERERERF5DQMQIiIiIiLyGgYgRERERETkNQxAiIiIiIjIaxiAEBERERGR1zAAISIiIiIir2EAQkREREREXsMAhIiIiIiIvIYBCBEREREReQ0DECIiIiIi8hoGIERERERE5DUMQIiIiIiIyGsYgBARERERkdcwACEiIiIiIq9hAEJERERERF7DAISIiIiIiLyGAQgREREREXkNAxAiIiIiIvIaBiBEREREROQ1DECIiIiIiMhrGIAQEREREZHXMAAhIiIiIiKvYQBCRERERERewwCEiIiIiIi8hgEIERERERF5DQMQIiIiIiLyGgYgRERERETkNQxAiIiIiIjIaxiAEBERERGR1zAAISIiIiIir2EAQkREREREXsMAhIiIiIiIvIYBCBEREREReQ0DECIiIiIi8hoGIERERERE5DUKX1eACun1eqSmpiIkJASSJPm6OkRERERkQQiB27dvo3r16pDJ+Cy/KBiA+JHU1FRER0f7uhpERERE5MT58+dRs2ZNX1ejVGIA4kdCQkIA5J/QoaGhPq4NEREREVnKyMhAdHS08b6N3McAxI8Yul2FhoYyACEiIiLyY+wuX3TsuEZERERERF7DAISIiIiIiLyGAQgREREREXkNAxAiIiIiIvIaBiBEREREROQ1DECIiIiIiMhrmIaXiIiIqIBOp4NGo/F1NciL5HI5lEqlr6tRrjAAISIionJPCIHLly8jPT0dQghfV4e8TK1WIyIigvOw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ujrkZWq1GjVq1EBoaKivq1IuMAAhIiKick+SJERFRaFKlSrGsQBUPsjlcna78jIGIEREREQFDONBiKjkcBA6ERERERF5DQMQIiIiIiLyGgYgRERERETkNQxAiIiIiIjIaxiAEBERERGR1zAAISIiIiIir2EAQkREREREXsMAhIiIiIiIvIYBCBFRGSCEr2tARETkGgYgRERERETkNQxAiIiIiIjIaxiAEBGVAZLk6xoQERG5hgEIEVEZwDEgRERUWjAAISIiIiIir2EAQkREREREXsMAhIioDOAYECIiKi0YgBARlQEcA0JERKUFAxAiIiIiIvIaBiBEREREROQ1DECIiIiIiMhrGIAQEREREZHXMAAhIiIiIiKvYQBCRERERERewwCEiIiIiIi8hgEIERERERF5DQMQIiIiIiLyGgYgRERERETkNQxAiIjKAAHh6yoQERG5hAEIERERERF5DQMQIqIyQILk6yoQERG5hAEIERERERF5DQMQIqIygGNAiIiotGAAQkREREREXsMAhIioDOAYECIiKi0YgBARERERkdcwACEiKgM4BoSIiEoLBiBEREREROQ1DECIiIiIiMhrGIAQEREREZHXMACx8NNPP+G5555Dq1atoFarIUkS5s2bZ7d8RkYGRo0ahdjYWKjVasTFxeHNN99EZmam9ypNRERERFRKKHxdAX8zfvx4nD17FhEREYiKisLZs2ftls3KykKXLl2QlJSEXr16YdCgQdi/fz9mzZqFTZs2YfPmzQgICPBi7YmIiIiI/BtbQCzMnTsXZ86cwdWrV/H88887LPv+++8jKSkJY8aMwapVq/Dee+9h1apVGDNmDHbv3o3Zs2d7qdZERIWEYEYsIiLyXwxALPTo0QOxsbFOywkhMHfuXAQHB2PChAlm6yZMmIDg4GDMnTu3pKpJRERERFQqMQApouTkZKSmpqJDhw4ICgoyWxcUFIQOHTrg9OnTOH/+vI9qSERERETkfxiAFFFycjIAICEhweZ6w3JDOSIiIiIi4iD0IktPTwcAhIWF2VwfGhpqVs6W3Nxc5ObmGn/PyMjwYA2JiIiIiPwPW0B8aMaMGQgLCzP+i46O9nWViKgM4Bh0IvJ3By/cwpu/H0BaRo6vq0I+wACkiAwtH/ZaOAytGfZaSABg7NixSE9PN/7jeBEiIiIqDx78LBG/772A138/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' width=800.0/>\n",
                             "            </div>\n",
                             "        "
                         ],
                         "text/plain": [
                             "Canvas(toolbar=Toolbar(toolitems=[('Home', 'Reset original view', 'home', 'home'), ('Back', 'Back to previous \u2026"
                         ]
                     },
@@ -768,15 +1088,17 @@
             "source": [
                 "## Plot FLUX for all records"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Ignoring unsupported feature: align_records\n"
                     ]
@@ -785,15 +1107,17 @@
             "source": [
                 "print('Ignoring unsupported feature: align_records')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 23,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "#import sparcl.gather_2d\n",
                 "#ar_dict, grid = sparcl.gather_2d.align_records(results.records)\n",
                 "#modeldf = pd.DataFrame(data=ar_dict['flux'],columns=grid)\n",
                 "#modeldf.transpose().plot(xlabel='Wavelength', ylabel='Flux', legend=False)"
             ]
@@ -819,26 +1143,30 @@
             "source": [
                 "## Logging in and logging out"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "if show_help:\n",
                 "    client.login?\n",
                 "    client.logout?"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 25,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Logged in successfully with email='test_user_1@noirlab.edu'\n"
                     ]
@@ -848,37 +1176,43 @@
                 "client.login(auth_user, usrpw)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 26,
             "metadata": {
-                "scrolled": true
+                "scrolled": true,
+                "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'Loggedin_As': 'test_user_1@noirlab.edu',\n",
-                            " 'Authorized_Datasets': {'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16', 'SDSS-DR17'}}"
+                            " 'Authorized_Datasets': {'BOSS-DR16',\n",
+                            "  'DESI-EDR',\n",
+                            "  'SDSS-DR16',\n",
+                            "  'SDSS-DR17-test'}}"
                         ]
                     },
                     "execution_count": 26,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "client.authorized"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 27,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Logged-out successfully.  Previously logged-in with email test_user_1@noirlab.edu.\n"
                     ]
@@ -887,15 +1221,17 @@
             "source": [
                 "client.logout()   # can also be done with client.login(None)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 28,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'Loggedin_As': 'Anonymous',\n",
                             " 'Authorized_Datasets': {'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'}}"
                         ]
@@ -913,729 +1249,785 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## FIND"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 29,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "out = ['sparcl_id', 'data_release']\n",
+                "\n",
+                "def pass_find(user, drs):\n",
+                "    client.login(user, usrpw)\n",
+                "    print(f'{client.authorized=}')\n",
+                "    try:\n",
+                "        if drs is None:\n",
+                "            found = client.find(outfields=out, limit=2)\n",
+                "        else:\n",
+                "            found = client.find(outfields=out, constraints=dict(data_release=drs), limit=2)\n",
+                "        print(f'\\nSUCCESS: {found.count=} records from FIND: {user=}; {drs=}')\n",
+                "    except Exception as err:\n",
+                "        raise Exception(f'\\nFAILED to get records from FIND: {user=}; {drs=}')\n",
+                "\n",
+                "def fail_find(user, drs):\n",
+                "    client.login(user, usrpw)\n",
+                "    print(f'{client.authorized=}')\n",
+                "\n",
+                "    try:\n",
+                "        found = client.find(outfields=out, constraints=dict(data_release=drs), limit=2)\n",
+                "        raise Exception(f'\\nFAILED: Auth wrongly got {found.count} records in FIND: {user=}; {drs=}')\n",
+                "    except Exception as err:\n",
+                "        print(f'\\nSUCCESS: Find did not get records. \\n{err}')"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Pass FIND with Public DRs as Anonymous"
+                "### Pass FIND as Authorized with Default DRs"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
-            "metadata": {},
+            "execution_count": 30,
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Logged-out successfully.  Previously logged-in with email None.\n"
+                        "Logged in successfully with email='test_user_1@noirlab.edu'\n",
+                        "client.authorized={'Loggedin_As': 'test_user_1@noirlab.edu', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16', 'SDSS-DR17-test'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id', 'data_release'], 'search': []}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"data_release\"], \"search\": []}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Record key counts: {'data_release': 2, 'sparcl_id': 2, '_dr': 2}\n",
+                        "\n",
+                        "SUCCESS: found.count=2 records from FIND: user='test_user_1@noirlab.edu'; drs=None\n"
                     ]
                 }
             ],
             "source": [
-                "client.logout()"
+                "pass_find(auth_user, None)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 30,
+            "cell_type": "markdown",
             "metadata": {},
+            "source": [
+                "### Pass FIND as Authorized with Priv&Pub DRs"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 31,
+            "metadata": {
+                "scrolled": true,
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"specid\", \"ra\", \"dec\", \"redshift\", \"spectype\", \"data_release\", \"redshift_err\"], \"search\": [[\"spectype\", \"GALAXY\"], [\"redshift\", 0.5, 0.9], [\"data_release\", \"BOSS-DR16\", \"SDSS-DR16\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
-                        "{'META': {'endpoint': 'sparc/find'},\n",
-                        " 'PARAMETERS': {'limit': 2,\n",
-                        "                'include': 'dec,ra,sparcl_id,specid',\n",
-                        "                'offset': 0,\n",
-                        "                'user': None,\n",
-                        "                'format': 'json',\n",
-                        "                'drs': ['BOSS-DR16', 'SDSS-DR16'],\n",
-                        "                'private_drs': ['SDSS-DR17'],\n",
-                        "                'username': 'Anonymous',\n",
-                        "                'json_payload': {'outfields': ['sparcl_id',\n",
-                        "                                               'specid',\n",
-                        "                                               'ra',\n",
-                        "                                               'dec',\n",
-                        "                                               'redshift',\n",
-                        "                                               'spectype',\n",
-                        "                                               'data_release',\n",
-                        "                                               'redshift_err'],\n",
-                        "                                 'search': [['spectype', 'GALAXY'],\n",
-                        "                                            ['redshift', 0.5, 0.9],\n",
-                        "                                            ['data_release',\n",
-                        "                                             'BOSS-DR16',\n",
-                        "                                             'SDSS-DR16']]}},\n",
-                        " 'HEADER': {'spectype': 'category',\n",
-                        "            'specid': 'np.int64',\n",
-                        "            'sparcl_id': 'str',\n",
-                        "            'redshift_err': 'np.float64',\n",
-                        "            'redshift': 'np.float64',\n",
-                        "            'data_release': 'category',\n",
-                        "            'dec': 'np.float64',\n",
-                        "            'ra': 'np.float64'},\n",
-                        " 'WARNINGS': ['OFFSET parameter needs SORT but it was not provided. Using '\n",
-                        "              \"default 'sparcl_id' for sorting\"]}\n",
-                        "{'spectype': 'GALAXY', 'specid': -6444532452352045056, 'sparcl_id': 'bb3d4287-8a2f-479f-9c7f-1053051e4925', 'redshift_err': 0.000331654009642079, 'redshift': 0.761636912822723, 'data_release': 'BOSS-DR16', 'dec': 28.063643, 'ra': 132.14379, '_dr': 'BOSS-DR16'}\n",
+                        "Logged in successfully with email='test_user_1@noirlab.edu'\n",
+                        "client.authorized={'Loggedin_As': 'test_user_1@noirlab.edu', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16', 'SDSS-DR17-test'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id', 'data_release'], 'search': [['data_release', 'BOSS-DR16', 'SDSS-DR17-test']]}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"data_release\"], \"search\": [[\"data_release\", \"BOSS-DR16\", \"SDSS-DR17-test\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Record key counts: {'data_release': 2, 'sparcl_id': 2, '_dr': 2}\n",
                         "\n",
-                        "SUCCESS: found.count=1 records from FIND\n"
+                        "SUCCESS: found.count=2 records from FIND: user='test_user_1@noirlab.edu'; drs=['BOSS-DR16', 'SDSS-DR17-test']\n"
                     ]
                 }
             ],
             "source": [
-                "out = ['sparcl_id','specid', 'ra', 'dec', 'redshift', 'spectype', 'data_release', 'redshift_err']\n",
-                "cons = {'spectype': ['GALAXY'],\n",
-                "        'redshift': [0.5, 0.9],\n",
-                "        'data_release': ['BOSS-DR16', 'SDSS-DR16']}\n",
-                "found = client.find(outfields=out, constraints=cons, limit=2)\n",
-                "pp(found.info)\n",
-                "print(found.records[0])\n",
-                "print(f'\\nSUCCESS: {found.count=} records from FIND')"
+                "pass_find(auth_user, [pub_dr,priv_dr])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Fail FIND with private DR as Anonymous"
+                "### Pass FIND as Unauthorized with Default DRs\n",
+                "DRs default to only what are authorized for authenticated user."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
-            "metadata": {},
+            "execution_count": 32,
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Logged-out successfully.  Previously logged-in with email None.\n"
+                        "Logged in successfully with email='test_user_2@noirlab.edu'\n",
+                        "client.authorized={'Loggedin_As': 'test_user_2@noirlab.edu', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id', 'data_release'], 'search': []}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"data_release\"], \"search\": []}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Record key counts: {'data_release': 2, 'sparcl_id': 2, '_dr': 2}\n",
+                        "\n",
+                        "SUCCESS: found.count=2 records from FIND: user='test_user_2@noirlab.edu'; drs=None\n"
                     ]
                 }
             ],
             "source": [
-                "client.logout()"
+                "pass_find(unauth_user, None)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 32,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "{'Loggedin_As': 'Anonymous',\n",
-                            " 'Authorized_Datasets': {'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'}}"
-                        ]
-                    },
-                    "execution_count": 32,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
             "source": [
-                "client.authorized"
+                "### Fail FIND as Unauthorized with Priv&Pub DRs"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 33,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"specid\", \"ra\", \"dec\", \"redshift\", \"spectype\", \"data_release\", \"redshift_err\"], \"search\": [[\"spectype\", \"GALAXY\"], [\"redshift\", 0.5, 0.9], [\"data_release\", \"BOSS-DR16\", \"SDSS-DR17\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
-                        "SUCCESS: Could not execute find: [UNKNOWN] uname='ANONYMOUS' is declined access to datasets:   SDSS-DR17.  drs_requested={'SDSS-DR17', 'BOSS-DR16'} my_auth={'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'} [NODRACCESS] None\n"
+                        "Logged in successfully with email='test_user_2@noirlab.edu'\n",
+                        "client.authorized={'Loggedin_As': 'test_user_2@noirlab.edu', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id', 'data_release'], 'search': [['data_release', 'BOSS-DR16', 'SDSS-DR17-test']]}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"data_release\"], \"search\": [[\"data_release\", \"BOSS-DR16\", \"SDSS-DR17-test\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Exception: response content=b'{\"errorMessage\": \"test_user_2@noirlab.edu is declined access to datasets [\\'SDSS-DR17-test\\']; drs_requested=[\\'BOSS-DR16\\', \\'SDSS-DR17-test\\'] my_auth=[\\'BOSS-DR16\\', \\'DESI-EDR\\', \\'SDSS-DR16\\']\", \"errorCode\": \"NODRACCESS\", \"statusCode\": 400, \"saved_tb\": \"NoneType: None\\\\n\"}'\n",
+                        "\n",
+                        "SUCCESS: Find did not get records. \n",
+                        "[UNKNOWN] test_user_2@noirlab.edu is declined access to datasets ['SDSS-DR17-test']; drs_requested=['BOSS-DR16', 'SDSS-DR17-test'] my_auth=['BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'] [NODRACCESS] None\n"
                     ]
                 }
             ],
             "source": [
-                "out = ['sparcl_id','specid', 'ra', 'dec', 'redshift', 'spectype', 'data_release', 'redshift_err']\n",
-                "cons = {'spectype': ['GALAXY'],\n",
-                "        'redshift': [0.5, 0.9],\n",
-                "        'data_release': ['BOSS-DR16',priv_dr]}\n",
-                "try:\n",
-                "    found = client.find(outfields=out, constraints=cons, limit=2)\n",
-                "    print('FOUND info:')\n",
-                "    pp(found.info)\n",
-                "    print(f'\\nFOUND records. {found.records[0]=}')\n",
-                "    gotrecord = True\n",
-                "except Exception as err:\n",
-                "    gotrecord = False\n",
-                "    print(f'SUCCESS: Could not execute find: {err}')\n",
-                "\n",
-                "if gotrecord:\n",
-                "    raise Exception('Wrongly got record from PRIVATE DR {priv_dr}')"
+                "fail_find(unauth_user, [pub_dr,priv_dr])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Pass FIND with default DR list as Anonymous"
+                "### Pass FIND as Unknown with Default DRs\n",
+                "DRs default to only what are authorized for authenticated user."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 34,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"specid\", \"ra\", \"dec\", \"redshift\", \"spectype\", \"data_release\", \"redshift_err\"], \"search\": [[\"spectype\", \"GALAXY\"], [\"redshift\", 0.5, 0.9]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
-                        "FOUND info:\n",
-                        "{'META': {'endpoint': 'sparc/find'},\n",
-                        " 'PARAMETERS': {'limit': 2,\n",
-                        "                'include': 'dec,ra,sparcl_id,specid',\n",
-                        "                'offset': 0,\n",
-                        "                'user': None,\n",
-                        "                'format': 'json',\n",
-                        "                'drs': ['BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'],\n",
-                        "                'private_drs': ['SDSS-DR17'],\n",
-                        "                'username': 'Anonymous',\n",
-                        "                'json_payload': {'outfields': ['sparcl_id',\n",
-                        "                                               'specid',\n",
-                        "                                               'ra',\n",
-                        "                                               'dec',\n",
-                        "                                               'redshift',\n",
-                        "                                               'spectype',\n",
-                        "                                               'data_release',\n",
-                        "                                               'redshift_err'],\n",
-                        "                                 'search': [['spectype', 'GALAXY'],\n",
-                        "                                            ['redshift', 0.5, 0.9]]}},\n",
-                        " 'HEADER': {'spectype': 'category',\n",
-                        "            'specid': 'np.int64',\n",
-                        "            'sparcl_id': 'str',\n",
-                        "            'redshift_err': 'np.float64',\n",
-                        "            'redshift': 'np.float64',\n",
-                        "            'data_release': 'category',\n",
-                        "            'dec': 'np.float64',\n",
-                        "            'ra': 'np.float64'},\n",
-                        " 'WARNINGS': ['OFFSET parameter needs SORT but it was not provided. Using '\n",
-                        "              \"default 'sparcl_id' for sorting\"]}\n",
+                        "Logged in successfully with email='test_user_3@noirlab.edu'\n",
+                        "client.authorized={'Loggedin_As': 'Anonymous', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id', 'data_release'], 'search': []}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"data_release\"], \"search\": []}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Record key counts: {'data_release': 2, 'sparcl_id': 2, '_dr': 2}\n",
                         "\n",
-                        "FOUND records. found.records[0]={'spectype': 'GALAXY', 'specid': 39627072179543889, 'sparcl_id': '2f79ffc2-71fa-11ee-b0da-08002725f1ef', 'redshift_err': 0.0001345702651861459, 'redshift': 0.6348533970651531, 'data_release': 'DESI-EDR', 'dec': -31.05971652239488, 'ra': 59.93519495098703, '_dr': 'DESI-EDR'}\n"
+                        "SUCCESS: found.count=2 records from FIND: user='test_user_3@noirlab.edu'; drs=None\n"
                     ]
                 }
             ],
             "source": [
-                "# Default Dataset list\n",
-                "out = ['sparcl_id','specid', 'ra', 'dec', 'redshift', 'spectype', 'data_release', 'redshift_err']\n",
-                "cons = {'spectype': ['GALAXY'],\n",
-                "        'redshift': [0.5, 0.9],\n",
-                "        #'data_release': ['BOSS-DR16',priv_dr]}\n",
-                "        }\n",
-                "try:\n",
-                "    found = client.find(outfields=out, constraints=cons, limit=2)\n",
-                "    print('FOUND info:')\n",
-                "    pp(found.info)\n",
-                "    print(f'\\nFOUND records. {found.records[0]=}')\n",
-                "    gotrecord = True\n",
-                "except Exception as err:\n",
-                "    gotrecord = False\n",
-                "    print(f'\\nSUCCESS: Could not execute find: {err}')\n",
-                "\n",
-                "if not gotrecord:\n",
-                "    raise Exception(f'\\nFailed to get record from default DR list as Anonymous.')"
+                "pass_find(non_user, None)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Fail FIND with prviate DR as Unauthorized"
+                "### Fail FIND as Unknown with Priv&Pub DRs"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 35,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Logged in successfully with email='test_user_2@noirlab.edu'\n"
+                        "Logged in successfully with email='test_user_3@noirlab.edu'\n",
+                        "client.authorized={'Loggedin_As': 'Anonymous', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id', 'data_release'], 'search': [['data_release', 'BOSS-DR16', 'SDSS-DR17-test']]}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"data_release\"], \"search\": [[\"data_release\", \"BOSS-DR16\", \"SDSS-DR17-test\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Exception: response content=b'{\"errorMessage\": \"ANONYMOUS is declined access to datasets [\\'SDSS-DR17-test\\']; drs_requested=[\\'BOSS-DR16\\', \\'SDSS-DR17-test\\'] my_auth=[\\'BOSS-DR16\\', \\'DESI-EDR\\', \\'SDSS-DR16\\']\", \"errorCode\": \"NODRACCESS\", \"statusCode\": 400, \"saved_tb\": \"NoneType: None\\\\n\"}'\n",
+                        "\n",
+                        "SUCCESS: Find did not get records. \n",
+                        "[UNKNOWN] ANONYMOUS is declined access to datasets ['SDSS-DR17-test']; drs_requested=['BOSS-DR16', 'SDSS-DR17-test'] my_auth=['BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'] [NODRACCESS] None\n"
                     ]
                 }
             ],
             "source": [
-                "client.login(unauth_user, usrpw)"
+                "fail_find(non_user, [pub_dr,priv_dr])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Pass FIND as Anonymous with Default DR list \n",
+                "DRs default to only what are authorized for authenticated user."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 36,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"specid\", \"ra\", \"dec\", \"redshift\", \"spectype\", \"data_release\", \"redshift_err\"], \"search\": [[\"spectype\", \"GALAXY\"], [\"redshift\", 0.5, 0.9], [\"data_release\", \"BOSS-DR16\", \"SDSS-DR17\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
-                        "SUCCESS: Could not execute find: [UNKNOWN] uname='test_user_2@noirlab.edu' is declined access to datasets:   SDSS-DR17.  drs_requested={'SDSS-DR17', 'BOSS-DR16'} my_auth={'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'} [NODRACCESS] None\n"
+                        "Logged-out successfully.  Previously logged-in with email test_user_3@noirlab.edu.\n",
+                        "client.authorized={'Loggedin_As': 'Anonymous', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id', 'data_release'], 'search': []}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"data_release\"], \"search\": []}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Record key counts: {'data_release': 2, 'sparcl_id': 2, '_dr': 2}\n",
+                        "\n",
+                        "SUCCESS: found.count=2 records from FIND: user=None; drs=None\n"
                     ]
                 }
             ],
             "source": [
-                "out = ['sparcl_id','specid', 'ra', 'dec', 'redshift', 'spectype', 'data_release', 'redshift_err']\n",
-                "cons = {'spectype': ['GALAXY'],\n",
-                "        'redshift': [0.5, 0.9],\n",
-                "        'data_release': ['BOSS-DR16',priv_dr]\n",
-                "        }\n",
-                "try:\n",
-                "    found = client.find(outfields=out, constraints=cons, limit=2)\n",
-                "    print('FOUND info:')\n",
-                "    pp(found.info)\n",
-                "    print(f'\\nFOUND records. {found.records[0]=}')\n",
-                "    gotrecord = True\n",
-                "except Exception as err:\n",
-                "    gotrecord = False\n",
-                "    print(f'SUCCESS: Could not execute find: {err}')\n",
-                "\n",
-                "if gotrecord:\n",
-                "    raise Exception('Wrongly got record from PRIVATE DR {priv_dr}')"
+                "pass_find(None, None)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Pass FIND with prviate DR as Authorized"
+                "### Pass FIND as Anonymous with Public DR"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 37,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Logged in successfully with email='test_user_1@noirlab.edu'\n"
+                        "Logged-out successfully.  Previously logged-in with email None.\n",
+                        "client.authorized={'Loggedin_As': 'Anonymous', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id', 'data_release'], 'search': [['data_release', 'BOSS-DR16']]}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"data_release\"], \"search\": [[\"data_release\", \"BOSS-DR16\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Record key counts: {'data_release': 2, 'sparcl_id': 2, '_dr': 2}\n",
+                        "\n",
+                        "SUCCESS: found.count=2 records from FIND: user=None; drs=['BOSS-DR16']\n"
                     ]
                 }
             ],
             "source": [
-                "client.login(auth_user, usrpw)"
+                "pass_find(None, [pub_dr])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Fail FIND as Anonymous with Priv&Pub DRs"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 38,
-            "metadata": {},
+            "metadata": {
+                "scrolled": true,
+                "tags": []
+            },
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "{'Loggedin_As': 'test_user_1@noirlab.edu',\n",
-                            " 'Authorized_Datasets': {'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16', 'SDSS-DR17'}}"
-                        ]
-                    },
-                    "execution_count": 38,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Logged-out successfully.  Previously logged-in with email None.\n",
+                        "client.authorized={'Loggedin_As': 'Anonymous', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id', 'data_release'], 'search': [['data_release', 'BOSS-DR16', 'SDSS-DR17-test']]}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"data_release\"], \"search\": [[\"data_release\", \"BOSS-DR16\", \"SDSS-DR17-test\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Exception: response content=b'{\"errorMessage\": \"ANONYMOUS is declined access to datasets [\\'SDSS-DR17-test\\']; drs_requested=[\\'BOSS-DR16\\', \\'SDSS-DR17-test\\'] my_auth=[\\'BOSS-DR16\\', \\'DESI-EDR\\', \\'SDSS-DR16\\']\", \"errorCode\": \"NODRACCESS\", \"statusCode\": 400, \"saved_tb\": \"NoneType: None\\\\n\"}'\n",
+                        "\n",
+                        "SUCCESS: Find did not get records. \n",
+                        "[UNKNOWN] ANONYMOUS is declined access to datasets ['SDSS-DR17-test']; drs_requested=['BOSS-DR16', 'SDSS-DR17-test'] my_auth=['BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'] [NODRACCESS] None\n"
+                    ]
                 }
             ],
             "source": [
-                "client.authorized"
+                "fail_find(None, [pub_dr, priv_dr])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## RETRIEVE"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 39,
-            "metadata": {},
+            "metadata": {
+                "scrolled": true
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"specid\", \"ra\", \"dec\", \"redshift\", \"spectype\", \"data_release\", \"redshift_err\"], \"search\": [[\"spectype\", \"GALAXY\"], [\"redshift\", 0.5, 0.9]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
-                        "FOUND info:\n",
-                        "{'META': {'endpoint': 'sparc/find'},\n",
-                        " 'PARAMETERS': {'limit': 2,\n",
-                        "                'include': 'dec,ra,sparcl_id,specid',\n",
-                        "                'offset': 0,\n",
-                        "                'format': 'json',\n",
-                        "                'drs': ['BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'],\n",
-                        "                'private_drs': ['SDSS-DR17'],\n",
-                        "                'username': 'test_user_1@noirlab.edu',\n",
-                        "                'json_payload': {'outfields': ['sparcl_id',\n",
-                        "                                               'specid',\n",
-                        "                                               'ra',\n",
-                        "                                               'dec',\n",
-                        "                                               'redshift',\n",
-                        "                                               'spectype',\n",
-                        "                                               'data_release',\n",
-                        "                                               'redshift_err'],\n",
-                        "                                 'search': [['spectype', 'GALAXY'],\n",
-                        "                                            ['redshift', 0.5, 0.9]]}},\n",
-                        " 'HEADER': {'spectype': 'category',\n",
-                        "            'specid': 'np.int64',\n",
-                        "            'sparcl_id': 'str',\n",
-                        "            'redshift_err': 'np.float64',\n",
-                        "            'redshift': 'np.float64',\n",
-                        "            'data_release': 'category',\n",
-                        "            'dec': 'np.float64',\n",
-                        "            'ra': 'np.float64'},\n",
-                        " 'WARNINGS': ['OFFSET parameter needs SORT but it was not provided. Using '\n",
-                        "              \"default 'sparcl_id' for sorting\"]}\n"
+                        "client=(sparclclient:1.2.2b8, api:11.0, http://localhost:8050/sparc, client_hash=f7bd410278bee26a425387c598dd47e80a8fcdcb, verbose=True, connect_timeout=1.1, read_timeout=5400.0)\n"
                     ]
                 }
             ],
             "source": [
-                "out = ['sparcl_id','specid', 'ra', 'dec', 'redshift', 'spectype', 'data_release', 'redshift_err']\n",
-                "cons = {'spectype': ['GALAXY'],\n",
-                "        'redshift': [0.5, 0.9],\n",
-                "        #'data_release': ['BOSS-DR16',priv_dr]}\n",
-                "        }\n",
-                "found = client.find(outfields=out, constraints=cons, limit=2)\n",
-                "print('FOUND info:')\n",
-                "pp(found.info)"
+                "print(f'{client=}')\n",
+                "inc = ['sparcl_id', 'data_release']\n",
+                "\n",
+                "#pub_ids = client.find(constraints=dict(data_release=[pub_dr]),limit=2).ids\n",
+                "#print(f'{pub_ids=}')\n",
+                "#priv_ids = client.find(constraints=dict(data_release=[priv_dr]),limit=2).ids\n",
+                "#print(f'{priv_ids=}')\n",
+                "\n",
+                "def pass_retrieve(user, drs):\n",
+                "    client.login(user, usrpw)\n",
+                "    print(f'{client.authorized=}')\n",
+                "\n",
+                "    if drs is None:\n",
+                "        ids = client.find(outfields=['sparcl_id'], limit=2).ids\n",
+                "    else:\n",
+                "        ids = client.find(outfields=['sparcl_id'], constraints=dict(data_release=drs), limit=2).ids\n",
+                "    try:\n",
+                "        if drs is None:\n",
+                "            got = client.retrieve(uuid_list=ids, include=inc, limit=2)\n",
+                "        else:\n",
+                "            got = client.retrieve(uuid_list=ids, include=inc, dataset_list=drs, limit=2)\n",
+                "        print(f'\\nSUCCESS: {got.count=} records from RETRIEVE: {user=}; {drs=}')\n",
+                "    except Exception as err:\n",
+                "        raise Exception(f'Auth wrongly refused records from RETRIEVE: {user=}; {drs=}')\n",
+                "\n",
+                "def fail_retrieve(user, drs):\n",
+                "    client.login(user, usrpw)\n",
+                "    print(f'{client.authorized=}')\n",
+                "\n",
+                "    try:\n",
+                "        found = client.find(outfields=out, constraints=dict(data_release=drs), limit=2)\n",
+                "        raise Exception(f'Auth wrongly got {found.count} records in RETRIEVE: {user=}; {drs=}')\n",
+                "    except Exception as err:\n",
+                "        print(f'\\nSUCCESS: RETRIEVE did not get records. \\n{err}')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Fail FIND with Unknown user\n",
-                "User is authenticated with SSO, but is unknown to SPARCL"
+                "### Pass RETRIEVE as Auth with Default DRs"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 40,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Logged in successfully with email='test_user_3@noirlab.edu'\n"
+                        "Logged in successfully with email='test_user_1@noirlab.edu'\n",
+                        "client.authorized={'Loggedin_As': 'test_user_1@noirlab.edu', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16', 'SDSS-DR17-test'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id'], 'search': []}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\"], \"search\": []}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Record key counts: {'_dr': 2, 'sparcl_id': 2}\n",
+                        "Using url=\"http://localhost:8050/sparc/spectras/?include=data_release%2Csparcl_id&format=pkl\"\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '[\"000923d5-fe87-11ee-acd2-08002725f1ef\", \"0016db04-fe87-11ee-a58b-08002725f1ef\"]' 'http://localhost:8050/sparc/spectras/?include=data_release%2Csparcl_id&format=pkl' | python3 -m json.tool\n",
+                        "Got response to post in 0.23809996293857694 seconds\n",
+                        "Got 2 spectra in 0.24 seconds (8 spectra/sec)\n",
+                        "{'success': True, 'info': [\"Successfully found 2 records in dr_list={'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'}\"], 'warnings': []}\n",
+                        "\n",
+                        "SUCCESS: found.count=20 records from RETRIEVE: user='test_user_1@noirlab.edu'; drs=None\n"
                     ]
                 }
             ],
             "source": [
-                "client.login(non_user, usrpw)"
+                "pass_retrieve(auth_user, None)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Pass RETRIEVE as Auth with Priv&Pub DRs"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 41,
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "{'Loggedin_As': 'Anonymous',\n",
-                            " 'Authorized_Datasets': {'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'}}"
-                        ]
-                    },
-                    "execution_count": 41,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Logged in successfully with email='test_user_1@noirlab.edu'\n",
+                        "client.authorized={'Loggedin_As': 'test_user_1@noirlab.edu', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16', 'SDSS-DR17-test'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id'], 'search': [['data_release', 'SDSS-DR17-test', 'BOSS-DR16']]}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\"], \"search\": [[\"data_release\", \"SDSS-DR17-test\", \"BOSS-DR16\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Record key counts: {'_dr': 2, 'sparcl_id': 2}\n",
+                        "Using url=\"http://localhost:8050/sparc/spectras/?include=data_release%2Csparcl_id&format=pkl&dataset_list=SDSS-DR17-test%2CBOSS-DR16\"\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '[\"510760cd-fe87-11ee-8470-08002725f1ef\", \"5111ce02-fe87-11ee-bea1-08002725f1ef\"]' 'http://localhost:8050/sparc/spectras/?include=data_release%2Csparcl_id&format=pkl&dataset_list=SDSS-DR17-test%2CBOSS-DR16' | python3 -m json.tool\n",
+                        "Got response to post in 0.27477827202528715 seconds\n",
+                        "Got 2 spectra in 0.27 seconds (7 spectra/sec)\n",
+                        "{'success': True, 'info': [\"Successfully found 2 records in dr_list=['SDSS-DR17-test', 'BOSS-DR16']\"], 'warnings': []}\n",
+                        "\n",
+                        "SUCCESS: found.count=20 records from RETRIEVE: user='test_user_1@noirlab.edu'; drs=['SDSS-DR17-test', 'BOSS-DR16']\n"
+                    ]
                 }
             ],
             "source": [
-                "client.authorized"
+                "pass_retrieve(auth_user, [priv_dr, pub_dr])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Pass RETRIEVE as Unauth with Default DRs\n",
+                "DRs default to only what are authorized for authenticated user."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 42,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"specid\", \"ra\", \"dec\", \"redshift\", \"spectype\", \"data_release\", \"redshift_err\"], \"search\": [[\"spectype\", \"GALAXY\"], [\"redshift\", 0.5, 0.9], [\"data_release\", \"BOSS-DR16\", \"SDSS-DR17\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
-                        "SUCCESS: Could not execute find: [UNKNOWN] uname='ANONYMOUS' is declined access to datasets:   SDSS-DR17.  drs_requested={'SDSS-DR17', 'BOSS-DR16'} my_auth={'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'} [NODRACCESS] None\n"
+                        "Logged in successfully with email='test_user_2@noirlab.edu'\n",
+                        "client.authorized={'Loggedin_As': 'test_user_2@noirlab.edu', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id'], 'search': []}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\"], \"search\": []}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Record key counts: {'_dr': 2, 'sparcl_id': 2}\n",
+                        "Using url=\"http://localhost:8050/sparc/spectras/?include=data_release%2Csparcl_id&format=pkl\"\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '[\"000923d5-fe87-11ee-acd2-08002725f1ef\", \"0016db04-fe87-11ee-a58b-08002725f1ef\"]' 'http://localhost:8050/sparc/spectras/?include=data_release%2Csparcl_id&format=pkl' | python3 -m json.tool\n",
+                        "Got response to post in 0.26971720601432025 seconds\n",
+                        "Got 2 spectra in 0.27 seconds (7 spectra/sec)\n",
+                        "{'success': True, 'info': [\"Successfully found 2 records in dr_list={'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'}\"], 'warnings': []}\n",
+                        "\n",
+                        "SUCCESS: found.count=20 records from RETRIEVE: user='test_user_2@noirlab.edu'; drs=None\n"
                     ]
                 }
             ],
             "source": [
-                "out = ['sparcl_id','specid', 'ra', 'dec', 'redshift', 'spectype', 'data_release', 'redshift_err']\n",
-                "cons = {'spectype': ['GALAXY'],\n",
-                "        'redshift': [0.5, 0.9],\n",
-                "        'data_release': ['BOSS-DR16',priv_dr]\n",
-                "        }\n",
                 "try:\n",
-                "    found = client.find(outfields=out, constraints=cons, limit=2)\n",
-                "    print('FOUND info:')\n",
-                "    pp(found.info)\n",
-                "    print(f'\\nFOUND records. {found.records[0]=}')\n",
-                "    gotrecord = True\n",
+                "    pass_retrieve(unauth_user, None)\n",
                 "except Exception as err:\n",
-                "    gotrecord = False\n",
-                "    print(f'SUCCESS: Could not execute find: {err}')\n",
-                "\n",
-                "if gotrecord:\n",
-                "    raise Exception(f'Wrongly got {found.count} records from {priv_dr=}')"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## RETRIEVE"
+                "    display(Markdown(f'#### BUG: {str(err)}'))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Pass RETRIEVE with public DRs as Anonymous"
+                "### Fail RETRIEVE as Unauth with Priv&Pub DRs"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 43,
-            "metadata": {},
+            "metadata": {
+                "scrolled": true
+            },
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "{'Loggedin_As': 'Anonymous',\n",
-                            " 'Authorized_Datasets': {'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'}}"
-                        ]
-                    },
-                    "execution_count": 43,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Logged in successfully with email='test_user_2@noirlab.edu'\n",
+                        "client.authorized={'Loggedin_As': 'test_user_2@noirlab.edu', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id', 'data_release'], 'search': [['data_release', 'SDSS-DR17-test', 'BOSS-DR16']]}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"data_release\"], \"search\": [[\"data_release\", \"SDSS-DR17-test\", \"BOSS-DR16\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Exception: response content=b'{\"errorMessage\": \"test_user_2@noirlab.edu is declined access to datasets [\\'SDSS-DR17-test\\']; drs_requested=[\\'BOSS-DR16\\', \\'SDSS-DR17-test\\'] my_auth=[\\'BOSS-DR16\\', \\'DESI-EDR\\', \\'SDSS-DR16\\']\", \"errorCode\": \"NODRACCESS\", \"statusCode\": 400, \"saved_tb\": \"NoneType: None\\\\n\"}'\n",
+                        "\n",
+                        "SUCCESS: RETRIEVE did not get records. \n",
+                        "[UNKNOWN] test_user_2@noirlab.edu is declined access to datasets ['SDSS-DR17-test']; drs_requested=['BOSS-DR16', 'SDSS-DR17-test'] my_auth=['BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'] [NODRACCESS] None\n"
+                    ]
                 }
             ],
             "source": [
-                "client.authorized"
+                "fail_retrieve(unauth_user, [priv_dr, pub_dr])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Pass RETRIEVE as Unknown with Default DRs\n",
+                "DRs default to only what are authorized for authenticated user."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 44,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\"], \"search\": [[\"data_release\", \"SDSS-DR16\", \"BOSS-DR16\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '[\"1ec5eb87-c678-4a17-9fec-2fe2982e24b0\", \"bb3d4287-8a2f-479f-9c7f-1053051e4925\"]' 'http://localhost:8050/sparc/spectras/?include=spectype%2Cspecid%2Cdata_release%2Cflux%2Credshift&format=pkl&dataset_list=SDSS-DR16%2CBOSS-DR16' | python3 -m json.tool\n",
-                        "Pass: got.records[0].spectype='GALAXY' len(got.records[0].flux)=4621\n"
+                        "Logged in successfully with email='test_user_3@noirlab.edu'\n",
+                        "client.authorized={'Loggedin_As': 'Anonymous', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id'], 'search': []}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\"], \"search\": []}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Record key counts: {'_dr': 2, 'sparcl_id': 2}\n",
+                        "Using url=\"http://localhost:8050/sparc/spectras/?include=data_release%2Csparcl_id&format=pkl\"\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '[\"000923d5-fe87-11ee-acd2-08002725f1ef\", \"0016db04-fe87-11ee-a58b-08002725f1ef\"]' 'http://localhost:8050/sparc/spectras/?include=data_release%2Csparcl_id&format=pkl' | python3 -m json.tool\n",
+                        "Got response to post in 0.3079184840898961 seconds\n",
+                        "Got 2 spectra in 0.31 seconds (6 spectra/sec)\n",
+                        "{'success': True, 'info': [\"Successfully found 2 records in dr_list={'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'}\"], 'warnings': []}\n",
+                        "\n",
+                        "SUCCESS: found.count=20 records from RETRIEVE: user='test_user_3@noirlab.edu'; drs=None\n"
                     ]
                 }
             ],
             "source": [
-                "inc = ['specid', 'data_release', 'redshift', 'flux', 'spectype']\n",
-                "drs = ['SDSS-DR16','BOSS-DR16']\n",
-                "found = client.find(outfields=['sparcl_id'], constraints=dict(data_release=drs),limit=2)\n",
-                "\n",
                 "try:\n",
-                "    got = client.retrieve(uuid_list=found.ids,\n",
-                "                          include=inc,\n",
-                "                          dataset_list=drs)\n",
-                "    gotrecord = True\n",
+                "    pass_retrieve(non_user, None)\n",
                 "except Exception as err:\n",
-                "    gotrecord = False\n",
-                "\n",
-                "if gotrecord:\n",
-                "   print(f'Pass: {got.records[0].spectype=} {len(got.records[0].flux)=}')\n",
-                "else:\n",
-                "    print(f'Failed: {err=}')"
+                "    display(Markdown(f'#### BUG: {str(err)}'))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Fail RETRIEVE with private DR as Anonymous"
+                "### Fail RETRIEVE as Unknown with Priv&Pub DRs"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 45,
-            "metadata": {},
+            "metadata": {
+                "scrolled": true
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Logged-out successfully.  Previously logged-in with email test_user_3@noirlab.edu.\n",
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '[\"1ec5eb87-c678-4a17-9fec-2fe2982e24b0\", \"bb3d4287-8a2f-479f-9c7f-1053051e4925\"]' 'http://localhost:8050/sparc/spectras/?include=spectype%2Cspecid%2Cdata_release%2Cflux%2Credshift&format=pkl&dataset_list=SDSS-DR16%2CSDSS-DR17%2CBOSS-DR16' | python3 -m json.tool\n",
-                        "Correctly could not retrieve: [UNKNOWN] uname='ANONYMOUS' is declined access to datasets:   SDSS-DR17.  drs_requested=['SDSS-DR16', 'SDSS-DR17', 'BOSS-DR16'] my_auth={'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'} [NODRACCESS] None\n"
+                        "Logged in successfully with email='test_user_3@noirlab.edu'\n",
+                        "client.authorized={'Loggedin_As': 'Anonymous', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id', 'data_release'], 'search': [['data_release', 'SDSS-DR17-test', 'BOSS-DR16']]}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"data_release\"], \"search\": [[\"data_release\", \"SDSS-DR17-test\", \"BOSS-DR16\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Exception: response content=b'{\"errorMessage\": \"ANONYMOUS is declined access to datasets [\\'SDSS-DR17-test\\']; drs_requested=[\\'BOSS-DR16\\', \\'SDSS-DR17-test\\'] my_auth=[\\'BOSS-DR16\\', \\'DESI-EDR\\', \\'SDSS-DR16\\']\", \"errorCode\": \"NODRACCESS\", \"statusCode\": 400, \"saved_tb\": \"NoneType: None\\\\n\"}'\n",
+                        "\n",
+                        "SUCCESS: RETRIEVE did not get records. \n",
+                        "[UNKNOWN] ANONYMOUS is declined access to datasets ['SDSS-DR17-test']; drs_requested=['BOSS-DR16', 'SDSS-DR17-test'] my_auth=['BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'] [NODRACCESS] None\n"
                     ]
                 }
             ],
             "source": [
-                "client.logout()\n",
-                "try:\n",
-                "    got = client.retrieve(uuid_list=found.ids,\n",
-                "                          include=inc,\n",
-                "                          dataset_list=['SDSS-DR16',priv_dr,'BOSS-DR16'])\n",
-                "    gotrecord = True\n",
-                "except Exception as err:\n",
-                "    gotrecord = False\n",
-                "    print(f'Correctly could not retrieve: {err}')\n",
-                "\n",
-                "if gotrecord:\n",
-                "    raise Exception('Wrongly got record from PRIVATE DR {priv_dr}')"
+                "fail_retrieve(non_user, [priv_dr, pub_dr])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Pass RETRIEVE with private DRs as Authorized"
+                "### Pass RETRIEVE as Anon with Default DRs\n",
+                "DRs default to only what are authorized for authenticated user."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 46,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Logged in successfully with email='test_user_1@noirlab.edu'\n"
+                        "Logged-out successfully.  Previously logged-in with email test_user_3@noirlab.edu.\n",
+                        "client.authorized={'Loggedin_As': 'Anonymous', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id'], 'search': []}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\"], \"search\": []}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Record key counts: {'_dr': 2, 'sparcl_id': 2}\n",
+                        "Using url=\"http://localhost:8050/sparc/spectras/?include=data_release%2Csparcl_id&format=pkl\"\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '[\"000923d5-fe87-11ee-acd2-08002725f1ef\", \"0016db04-fe87-11ee-a58b-08002725f1ef\"]' 'http://localhost:8050/sparc/spectras/?include=data_release%2Csparcl_id&format=pkl' | python3 -m json.tool\n",
+                        "Got response to post in 0.03403094399254769 seconds\n",
+                        "Got 2 spectra in 0.03 seconds (59 spectra/sec)\n",
+                        "{'success': True, 'info': [\"Successfully found 2 records in dr_list={'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'}\"], 'warnings': []}\n",
+                        "\n",
+                        "SUCCESS: found.count=20 records from RETRIEVE: user=None; drs=None\n"
                     ]
                 }
             ],
             "source": [
-                "client.login(auth_user, usrpw)"
+                "try:\n",
+                "    pass_retrieve(None, None)\n",
+                "except Exception as err:\n",
+                "    display(Markdown(f'#### BUG: {str(err)}'))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Fail RETRIEVE as Anon with Priv&Pub DR "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 47,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "{'Loggedin_As': 'test_user_1@noirlab.edu',\n",
-                            " 'Authorized_Datasets': {'BOSS-DR16', 'DESI-EDR', 'SDSS-DR16', 'SDSS-DR17'}}"
-                        ]
-                    },
-                    "execution_count": 47,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Logged-out successfully.  Previously logged-in with email None.\n",
+                        "client.authorized={'Loggedin_As': 'Anonymous', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id', 'data_release'], 'search': [['data_release', 'SDSS-DR17-test', 'BOSS-DR16']]}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\", \"data_release\"], \"search\": [[\"data_release\", \"SDSS-DR17-test\", \"BOSS-DR16\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Exception: response content=b'{\"errorMessage\": \"ANONYMOUS is declined access to datasets [\\'SDSS-DR17-test\\']; drs_requested=[\\'BOSS-DR16\\', \\'SDSS-DR17-test\\'] my_auth=[\\'BOSS-DR16\\', \\'DESI-EDR\\', \\'SDSS-DR16\\']\", \"errorCode\": \"NODRACCESS\", \"statusCode\": 400, \"saved_tb\": \"NoneType: None\\\\n\"}'\n",
+                        "\n",
+                        "SUCCESS: RETRIEVE did not get records. \n",
+                        "[UNKNOWN] ANONYMOUS is declined access to datasets ['SDSS-DR17-test']; drs_requested=['BOSS-DR16', 'SDSS-DR17-test'] my_auth=['BOSS-DR16', 'DESI-EDR', 'SDSS-DR16'] [NODRACCESS] None\n"
+                    ]
                 }
             ],
             "source": [
-                "client.authorized"
+                "fail_retrieve(None, [priv_dr, pub_dr])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Pass RETRIEVE as Anon with Public DR "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 48,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\"], \"search\": [[\"data_release\", \"SDSS-DR16\", \"BOSS-DR16\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
-                        "curl -X 'POST' -H 'Content-Type: application/json' -d '[\"1ec5eb87-c678-4a17-9fec-2fe2982e24b0\", \"bb3d4287-8a2f-479f-9c7f-1053051e4925\"]' 'http://localhost:8050/sparc/spectras/?include=spectype%2Cspecid%2Cdata_release%2Cflux%2Credshift&format=pkl&dataset_list=SDSS-DR16%2CSDSS-DR17%2CBOSS-DR16' | python3 -m json.tool\n",
-                        "got.count=2\n",
-                        "Pass: got.records[0].spectype='GALAXY' len(got.records[0].flux)=4621\n"
+                        "Logged-out successfully.  Previously logged-in with email None.\n",
+                        "client.authorized={'Loggedin_As': 'Anonymous', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n",
+                        "url=http://localhost:8050/sparc/find/?limit=2 sspec={'outfields': ['sparcl_id'], 'search': [['data_release', 'BOSS-DR16']]}\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '{\"outfields\": [\"sparcl_id\"], \"search\": [[\"data_release\", \"BOSS-DR16\"]]}' 'http://localhost:8050/sparc/find/?limit=2' | python3 -m json.tool\n",
+                        "Record key counts: {'_dr': 2, 'sparcl_id': 2}\n",
+                        "Using url=\"http://localhost:8050/sparc/spectras/?include=data_release%2Csparcl_id&format=pkl&dataset_list=BOSS-DR16\"\n",
+                        "curl -X 'POST' -H 'Content-Type: application/json' -d '[\"510760cd-fe87-11ee-8470-08002725f1ef\", \"5111ce02-fe87-11ee-bea1-08002725f1ef\"]' 'http://localhost:8050/sparc/spectras/?include=data_release%2Csparcl_id&format=pkl&dataset_list=BOSS-DR16' | python3 -m json.tool\n",
+                        "Got response to post in 0.0383652689633891 seconds\n",
+                        "Got 2 spectra in 0.04 seconds (52 spectra/sec)\n",
+                        "{'success': True, 'info': [\"Successfully found 2 records in dr_list=['BOSS-DR16']\"], 'warnings': []}\n",
+                        "\n",
+                        "SUCCESS: found.count=20 records from RETRIEVE: user=None; drs=['BOSS-DR16']\n"
                     ]
                 }
             ],
             "source": [
-                "inc = ['specid', 'data_release', 'redshift', 'flux', 'spectype']\n",
-                "drs = ['SDSS-DR16','BOSS-DR16']\n",
-                "found = client.find(outfields=['sparcl_id'], constraints=dict(data_release=drs),limit=2)\n",
-                "\n",
-                "try:\n",
-                "    got = client.retrieve(uuid_list=found.ids,\n",
-                "                          include=inc,\n",
-                "                          dataset_list=['SDSS-DR16',priv_dr,'BOSS-DR16'])\n",
-                "    gotrecord = True\n",
-                "    print(f'{got.count=}')\n",
-                "except Exception as err:\n",
-                "    gotrecord = False\n",
-                "    msg = err\n",
-                "    \n",
-                "if gotrecord:\n",
-                "   print(f'Pass: {got.records[0].spectype=} {len(got.records[0].flux)=}')\n",
-                "else:\n",
-                "    print(f'Failed: {msg}')"
+                "pass_retrieve(None, [pub_dr])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# All Done"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 49,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Run finished: 2024-03-06 07:12:30.513140\n"
+                        "Run finished: 2024-05-02 10:22:39.403970\n"
                     ]
                 }
             ],
             "source": [
                 "print(f'Run finished: {str(datetime.now())}')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 50,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Logged in successfully with email='test_user_1@noirlab.edu'\n",
                         "\n",
-                        "client.authorized={'Loggedin_As': 'test_user_1@noirlab.edu', 'Authorized_Datasets': {'SDSS-DR17', 'DESI-EDR', 'SDSS-DR16', 'BOSS-DR16'}}\n",
+                        "client.authorized={'Loggedin_As': 'test_user_1@noirlab.edu', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16', 'SDSS-DR17-test'}}\n",
                         "\n",
                         "\n",
                         "Logged-out successfully.  Previously logged-in with email test_user_1@noirlab.edu.\n",
                         "\n",
-                        "client.authorized={'Loggedin_As': 'Anonymous', 'Authorized_Datasets': {'DESI-EDR', 'BOSS-DR16', 'SDSS-DR16'}}\n"
+                        "client.authorized={'Loggedin_As': 'Anonymous', 'Authorized_Datasets': {'SDSS-DR16', 'DESI-EDR', 'BOSS-DR16'}}\n"
                     ]
                 }
             ],
             "source": [
                 "# DLS-496\n",
                 "client.login(auth_user, usrpw)\n",
                 "print(f'\\n{client.authorized=}\\n\\n')\n",
                 "client.logout()   # can also be done with client.login(None)\n",
                 "print(f'\\n{client.authorized=}')"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `sparclclient-1.2.2b8/sparcl/resample_spectra.py` & `sparclclient-1.2.2b9/sparcl/resample_spectra.py`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/sparcl/type_conversion.py` & `sparclclient-1.2.2b9/sparcl/type_conversion.py`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/sparcl/unsupported.py` & `sparclclient-1.2.2b9/sparcl/unsupported.py`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/sparcl/utils.py` & `sparclclient-1.2.2b9/sparcl/utils.py`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/tests/expected_dev1.py` & `sparclclient-1.2.2b9/tests/expected_dev1.py`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/tests/methods_tests.py` & `sparclclient-1.2.2b9/tests/methods_tests.py`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/tests/utils.py` & `sparclclient-1.2.2b9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/tox.ini` & `sparclclient-1.2.2b9/tox.ini`

 * *Files identical despite different names*

### Comparing `sparclclient-1.2.2b8/PKG-INFO` & `sparclclient-1.2.2b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparclclient
-Version: 1.2.2b8
+Version: 1.2.2b9
 Summary: A client for getting spectra and meta-data from NOIRLab.
 Author-email: "S. Pothier" <datalab-spectro@noirlab.edu>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Bug Tracker, https://github.com/pypa/sparclclient/issues
 Project-URL: Documentation, https://sparclclient.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/pypa/sparclclient
```
