# Comparing `tmp/simple_acme_dns-3.0.0.tar.gz` & `tmp/simple_acme_dns-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_acme_dns-3.0.0.tar", last modified: Sat Oct 14 02:25:45 2023, max compression
+gzip compressed data, was "simple_acme_dns-3.1.0.tar", last modified: Thu May 23 17:51:40 2024, max compression
```

## Comparing `simple_acme_dns-3.0.0.tar` & `simple_acme_dns-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 02:25:45.876936 simple_acme_dns-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2023-10-14 02:25:34.000000 simple_acme_dns-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-14 02:25:34.000000 simple_acme_dns-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2023-10-14 02:25:45.876936 simple_acme_dns-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-10-14 02:25:34.000000 simple_acme_dns-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-14 02:25:34.000000 simple_acme_dns-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-14 02:25:45.876936 simple_acme_dns-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-10-14 02:25:34.000000 simple_acme_dns-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 02:25:45.872936 simple_acme_dns-3.0.0/simple_acme_dns/
--rw-r--r--   0 runner    (1001) docker     (127)    34772 2023-10-14 02:25:34.000000 simple_acme_dns-3.0.0/simple_acme_dns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 02:25:45.876936 simple_acme_dns-3.0.0/simple_acme_dns/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2023-10-14 02:25:34.000000 simple_acme_dns-3.0.0/simple_acme_dns/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 02:25:45.876936 simple_acme_dns-3.0.0/simple_acme_dns/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2023-10-14 02:25:34.000000 simple_acme_dns-3.0.0/simple_acme_dns/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 02:25:45.876936 simple_acme_dns-3.0.0/simple_acme_dns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2023-10-14 02:25:45.000000 simple_acme_dns-3.0.0/simple_acme_dns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-10-14 02:25:45.000000 simple_acme_dns-3.0.0/simple_acme_dns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-14 02:25:45.000000 simple_acme_dns-3.0.0/simple_acme_dns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-14 02:25:45.000000 simple_acme_dns-3.0.0/simple_acme_dns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-14 02:25:45.000000 simple_acme_dns-3.0.0/simple_acme_dns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:51:40.679349 simple_acme_dns-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-23 17:51:36.000000 simple_acme_dns-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-23 17:51:36.000000 simple_acme_dns-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-23 17:51:40.675349 simple_acme_dns-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-23 17:51:36.000000 simple_acme_dns-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 17:51:36.000000 simple_acme_dns-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:51:40.679349 simple_acme_dns-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-23 17:51:36.000000 simple_acme_dns-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:51:40.675349 simple_acme_dns-3.1.0/simple_acme_dns/
+-rw-r--r--   0 runner    (1001) docker     (127)    34830 2024-05-23 17:51:36.000000 simple_acme_dns-3.1.0/simple_acme_dns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:51:40.675349 simple_acme_dns-3.1.0/simple_acme_dns/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-23 17:51:36.000000 simple_acme_dns-3.1.0/simple_acme_dns/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:51:40.675349 simple_acme_dns-3.1.0/simple_acme_dns/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-23 17:51:36.000000 simple_acme_dns-3.1.0/simple_acme_dns/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:51:40.675349 simple_acme_dns-3.1.0/simple_acme_dns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-23 17:51:40.000000 simple_acme_dns-3.1.0/simple_acme_dns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-23 17:51:40.000000 simple_acme_dns-3.1.0/simple_acme_dns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:51:40.000000 simple_acme_dns-3.1.0/simple_acme_dns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 17:51:40.000000 simple_acme_dns-3.1.0/simple_acme_dns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 17:51:40.000000 simple_acme_dns-3.1.0/simple_acme_dns.egg-info/top_level.txt
```

### Comparing `simple_acme_dns-3.0.0/LICENSE` & `simple_acme_dns-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_acme_dns-3.0.0/PKG-INFO` & `simple_acme_dns-3.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: simple_acme_dns
-Version: 3.0.0
+Version: 3.1.0
 Summary: A Python ACME client for the DNS-01 challenge
 Home-page: https://github.com/jaredhendrickson13/simple_acme_dns
 Author: Jared Hendrickson
-Author-email: jaredhendrickson13@gmail.com
+Author-email: github@jaredhendrickson.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: acme~=2.6.0
-Requires-Dist: validators~=0.22.0
-Requires-Dist: dnspython~=2.4.2
+Requires-Dist: acme~=2.10.0
+Requires-Dist: validators~=0.28.1
+Requires-Dist: dnspython~=2.6.1
 
 simple_acme_dns
 ================
-[![Coverage](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/coverage.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/coverage.yml)
-[![PyPI](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/pypi.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/pypi.yml)
-[![PyLint](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/pylint.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/pylint.yml)
+[![Quality](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/quality.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/quality.yml)
+[![Release](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/release.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/release.yml)
 [![CodeQL](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/codeql.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/codeql.yml)
 
 **simple_acme_dns** is a Python ACME client wrapper specifically tailored to the DNS-01 challenge. This makes it easy to manage ACME 
 certificates and accounts without the need for an external tool like `certbot`. Although this module is intended for use
 with Let's Encrypt, it will support any CA utilizing the ACME v2 protocol.
 
 ### Installation
```

### Comparing `simple_acme_dns-3.0.0/README.md` & `simple_acme_dns-3.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 simple_acme_dns
 ================
-[![Coverage](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/coverage.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/coverage.yml)
-[![PyPI](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/pypi.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/pypi.yml)
-[![PyLint](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/pylint.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/pylint.yml)
+[![Quality](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/quality.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/quality.yml)
+[![Release](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/release.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/release.yml)
 [![CodeQL](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/codeql.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/codeql.yml)
 
 **simple_acme_dns** is a Python ACME client wrapper specifically tailored to the DNS-01 challenge. This makes it easy to manage ACME 
 certificates and accounts without the need for an external tool like `certbot`. Although this module is intended for use
 with Let's Encrypt, it will support any CA utilizing the ACME v2 protocol.
 
 ### Installation
```

### Comparing `simple_acme_dns-3.0.0/setup.py` & `simple_acme_dns-3.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,21 +29,21 @@
         return list(filter(None, requirements_file.read().split("\n")))
 
 
 # Set our setup parameters
 setup(
     name='simple_acme_dns',
     author='Jared Hendrickson',
-    author_email='jaredhendrickson13@gmail.com',
+    author_email='github@jaredhendrickson.com',
     url="https://github.com/jaredhendrickson13/simple_acme_dns",
     license="Apache-2.0",
     description="A Python ACME client for the DNS-01 challenge",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
-    version="3.0.0",
+    version="3.1.0",
     packages=["simple_acme_dns", "simple_acme_dns.tools", "simple_acme_dns.errors"],
     install_requires=read_requirements(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `simple_acme_dns-3.0.0/simple_acme_dns/__init__.py` & `simple_acme_dns-3.1.0/simple_acme_dns/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 
         # Initialize our ACME client object
         self.net = client.ClientNetwork(self.account_key, user_agent='simple_acme_dns/v2')
         self.directory_obj = messages.Directory.from_json(self.net.get(self.directory).json())
         self.acme_client = client.ClientV2(self.directory_obj, net=self.net)
 
         # Complete registration
-        registration = messages.NewRegistration.from_data(email=self.email, terms_of_service_agreed=True)
+        registration = messages.NewRegistration.from_data(email=self._email, terms_of_service_agreed=True)
         self.account = self.acme_client.new_account(registration)
 
     def deactivate_account(self, delete: bool = True) -> None:
         """
         Deactivates the current account registration. This action is irreversible.
 
         Args:
@@ -342,15 +342,15 @@
             '{"account": {"body": {"key": {"n": "vtByzpW..."}}}}'
         """
         # Format our object into a serializable format
         acct_data = {
             'account': self.account.to_json(),
             'account_key': self.account_key.json_dumps(),
             'directory': self.directory,
-            'domains': self.domains,
+            'domains': self._domains,
             'certificate': self.certificate.decode() if save_certificate else '',
             'private_key': self.private_key.decode() if save_private_key else ''
         }
 
         return json.dumps(acct_data)
 
     def export_account_to_file(
@@ -412,15 +412,16 @@
         obj = ACMEClient()
 
         # Format the serialized data back into the object
         obj.directory = acct_data.get('directory', None)
         obj.domains = acct_data.get('domains', [])
         obj.certificate = acct_data.get('certificate', '').encode()
         obj.private_key = acct_data.get('private_key', '').encode()
-        obj.email = acct_data['account']['body']['contact'][0].replace('mailto:', '')
+        if acct_data['account']['body']['contact']:
+            obj.email = acct_data['account']['body']['contact'][0].replace('mailto:', '')
         obj.account = messages.RegistrationResource.json_loads(json.dumps(acct_data['account']))
         obj.account_key = jose.JWKRSA.json_loads(acct_data['account_key'])
 
         # Re-initialize the ACME client and registration
         obj.net = client.ClientNetwork(obj.account_key, user_agent='simple_acme_dns/1.0.0')
         obj.directory_obj = messages.Directory.from_json(obj.net.get(obj.directory).json())
         obj.acme_client = client.ClientV2(obj.directory_obj, net=obj.net)
```

### Comparing `simple_acme_dns-3.0.0/simple_acme_dns/errors/__init__.py` & `simple_acme_dns-3.1.0/simple_acme_dns/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_acme_dns-3.0.0/simple_acme_dns/tools/__init__.py` & `simple_acme_dns-3.1.0/simple_acme_dns/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_acme_dns-3.0.0/simple_acme_dns.egg-info/PKG-INFO` & `simple_acme_dns-3.1.0/simple_acme_dns.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
-Name: simple-acme-dns
-Version: 3.0.0
+Name: simple_acme_dns
+Version: 3.1.0
 Summary: A Python ACME client for the DNS-01 challenge
 Home-page: https://github.com/jaredhendrickson13/simple_acme_dns
 Author: Jared Hendrickson
-Author-email: jaredhendrickson13@gmail.com
+Author-email: github@jaredhendrickson.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: acme~=2.6.0
-Requires-Dist: validators~=0.22.0
-Requires-Dist: dnspython~=2.4.2
+Requires-Dist: acme~=2.10.0
+Requires-Dist: validators~=0.28.1
+Requires-Dist: dnspython~=2.6.1
 
 simple_acme_dns
 ================
-[![Coverage](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/coverage.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/coverage.yml)
-[![PyPI](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/pypi.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/pypi.yml)
-[![PyLint](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/pylint.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/pylint.yml)
+[![Quality](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/quality.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/quality.yml)
+[![Release](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/release.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/release.yml)
 [![CodeQL](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/codeql.yml/badge.svg)](https://github.com/jaredhendrickson13/simple_acme_dns/actions/workflows/codeql.yml)
 
 **simple_acme_dns** is a Python ACME client wrapper specifically tailored to the DNS-01 challenge. This makes it easy to manage ACME 
 certificates and accounts without the need for an external tool like `certbot`. Although this module is intended for use
 with Let's Encrypt, it will support any CA utilizing the ACME v2 protocol.
 
 ### Installation
```

