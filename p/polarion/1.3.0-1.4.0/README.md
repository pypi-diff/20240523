# Comparing `tmp/polarion-1.3.0.tar.gz` & `tmp/polarion-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polarion-1.3.0.tar", last modified: Sun Oct  8 18:10:57 2023, max compression
+gzip compressed data, was "polarion-1.4.0.tar", last modified: Wed May 22 21:02:36 2024, max compression
```

## Comparing `polarion-1.3.0.tar` & `polarion-1.4.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 agent     (1000) agent     (1000)        0 2023-10-08 18:10:57.026349 polarion-1.3.0/
--rw-r--r--   0 agent     (1000) agent     (1000)     1073 2023-10-08 18:10:41.000000 polarion-1.3.0/LICENSE
--rw-r--r--   0 agent     (1000) agent     (1000)     4059 2023-10-08 18:10:57.026349 polarion-1.3.0/PKG-INFO
--rw-r--r--   0 agent     (1000) agent     (1000)     3350 2023-10-08 18:10:41.000000 polarion-1.3.0/README.md
-drwxr-xr-x   0 agent     (1000) agent     (1000)        0 2023-10-08 18:10:57.022349 polarion-1.3.0/polarion/
--rw-r--r--   0 agent     (1000) agent     (1000)      323 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/__init__.py
-drwxr-xr-x   0 agent     (1000) agent     (1000)        0 2023-10-08 18:10:57.026349 polarion-1.3.0/polarion/base/
--rw-r--r--   0 agent     (1000) agent     (1000)        0 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/base/__init__.py
--rw-r--r--   0 agent     (1000) agent     (1000)     1291 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/base/comments.py
--rw-r--r--   0 agent     (1000) agent     (1000)     1938 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/base/custom_fields.py
--rw-r--r--   0 agent     (1000) agent     (1000)      329 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/base/polarion_object.py
--rw-r--r--   0 agent     (1000) agent     (1000)     8611 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/document.py
--rw-r--r--   0 agent     (1000) agent     (1000)      873 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/factory.py
--rw-r--r--   0 agent     (1000) agent     (1000)     7469 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/plan.py
--rw-r--r--   0 agent     (1000) agent     (1000)    12609 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/polarion.py
--rw-r--r--   0 agent     (1000) agent     (1000)    13017 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/project.py
--rw-r--r--   0 agent     (1000) agent     (1000)    10626 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/record.py
--rw-r--r--   0 agent     (1000) agent     (1000)     7027 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/testrun.py
--rw-r--r--   0 agent     (1000) agent     (1000)     1253 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/user.py
--rw-r--r--   0 agent     (1000) agent     (1000)     4810 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/utils.py
--rw-r--r--   0 agent     (1000) agent     (1000)    31181 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/workitem.py
--rw-r--r--   0 agent     (1000) agent     (1000)    14057 2023-10-08 18:10:41.000000 polarion-1.3.0/polarion/xml.py
-drwxr-xr-x   0 agent     (1000) agent     (1000)        0 2023-10-08 18:10:57.022349 polarion-1.3.0/polarion.egg-info/
--rw-r--r--   0 agent     (1000) agent     (1000)     4059 2023-10-08 18:10:57.000000 polarion-1.3.0/polarion.egg-info/PKG-INFO
--rw-r--r--   0 agent     (1000) agent     (1000)      874 2023-10-08 18:10:57.000000 polarion-1.3.0/polarion.egg-info/SOURCES.txt
--rw-r--r--   0 agent     (1000) agent     (1000)        1 2023-10-08 18:10:57.000000 polarion-1.3.0/polarion.egg-info/dependency_links.txt
--rw-r--r--   0 agent     (1000) agent     (1000)       20 2023-10-08 18:10:57.000000 polarion-1.3.0/polarion.egg-info/requires.txt
--rw-r--r--   0 agent     (1000) agent     (1000)       15 2023-10-08 18:10:57.000000 polarion-1.3.0/polarion.egg-info/top_level.txt
--rw-r--r--   0 agent     (1000) agent     (1000)      103 2023-10-08 18:10:41.000000 polarion-1.3.0/pyproject.toml
--rw-r--r--   0 agent     (1000) agent     (1000)      688 2023-10-08 18:10:57.026349 polarion-1.3.0/setup.cfg
--rw-r--r--   0 agent     (1000) agent     (1000)      954 2023-10-08 18:10:41.000000 polarion-1.3.0/setup.py
-drwxr-xr-x   0 agent     (1000) agent     (1000)        0 2023-10-08 18:10:57.026349 polarion-1.3.0/tests/
--rw-r--r--   0 agent     (1000) agent     (1000)        0 2023-10-08 18:10:41.000000 polarion-1.3.0/tests/__init__.py
--rw-r--r--   0 agent     (1000) agent     (1000)      134 2023-10-08 18:10:41.000000 polarion-1.3.0/tests/keys_template.py
--rw-r--r--   0 agent     (1000) agent     (1000)     4586 2023-10-08 18:10:41.000000 polarion-1.3.0/tests/test_polarion_client.py
--rw-r--r--   0 agent     (1000) agent     (1000)     6059 2023-10-08 18:10:41.000000 polarion-1.3.0/tests/test_polarion_document.py
--rw-r--r--   0 agent     (1000) agent     (1000)     5669 2023-10-08 18:10:41.000000 polarion-1.3.0/tests/test_polarion_plan.py
--rw-r--r--   0 agent     (1000) agent     (1000)     3150 2023-10-08 18:10:41.000000 polarion-1.3.0/tests/test_polarion_project.py
--rw-r--r--   0 agent     (1000) agent     (1000)     7733 2023-10-08 18:10:41.000000 polarion-1.3.0/tests/test_polarion_test_record.py
--rw-r--r--   0 agent     (1000) agent     (1000)     5134 2023-10-08 18:10:41.000000 polarion-1.3.0/tests/test_polarion_testrun.py
--rw-r--r--   0 agent     (1000) agent     (1000)      757 2023-10-08 18:10:41.000000 polarion-1.3.0/tests/test_polarion_user.py
--rw-r--r--   0 agent     (1000) agent     (1000)     3768 2023-10-08 18:10:41.000000 polarion-1.3.0/tests/test_polarion_utils.py
--rw-r--r--   0 agent     (1000) agent     (1000)    33496 2023-10-08 18:10:41.000000 polarion-1.3.0/tests/test_polarion_workitem.py
+drwxr-xr-x   0 agent     (1000) agent     (1000)        0 2024-05-22 21:02:35.998044 polarion-1.4.0/
+-rw-r--r--   0 agent     (1000) agent     (1000)     1073 2024-05-22 21:02:24.000000 polarion-1.4.0/LICENSE
+-rw-r--r--   0 agent     (1000) agent     (1000)     4059 2024-05-22 21:02:35.998044 polarion-1.4.0/PKG-INFO
+-rw-r--r--   0 agent     (1000) agent     (1000)     3350 2024-05-22 21:02:24.000000 polarion-1.4.0/README.md
+drwxr-xr-x   0 agent     (1000) agent     (1000)        0 2024-05-22 21:02:35.994044 polarion-1.4.0/polarion/
+-rw-r--r--   0 agent     (1000) agent     (1000)      323 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/__init__.py
+drwxr-xr-x   0 agent     (1000) agent     (1000)        0 2024-05-22 21:02:35.994044 polarion-1.4.0/polarion/base/
+-rw-r--r--   0 agent     (1000) agent     (1000)        0 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/base/__init__.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     1291 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/base/comments.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     1938 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/base/custom_fields.py
+-rw-r--r--   0 agent     (1000) agent     (1000)      329 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/base/polarion_object.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     8617 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/document.py
+-rw-r--r--   0 agent     (1000) agent     (1000)      873 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/factory.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     7469 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/plan.py
+-rw-r--r--   0 agent     (1000) agent     (1000)    12686 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/polarion.py
+-rw-r--r--   0 agent     (1000) agent     (1000)    13017 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/project.py
+-rw-r--r--   0 agent     (1000) agent     (1000)    10626 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/record.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     7027 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/testrun.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     1253 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/user.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     4810 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/utils.py
+-rw-r--r--   0 agent     (1000) agent     (1000)    31244 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/workitem.py
+-rw-r--r--   0 agent     (1000) agent     (1000)    17736 2024-05-22 21:02:24.000000 polarion-1.4.0/polarion/xml.py
+drwxr-xr-x   0 agent     (1000) agent     (1000)        0 2024-05-22 21:02:35.998044 polarion-1.4.0/polarion.egg-info/
+-rw-r--r--   0 agent     (1000) agent     (1000)     4059 2024-05-22 21:02:35.000000 polarion-1.4.0/polarion.egg-info/PKG-INFO
+-rw-r--r--   0 agent     (1000) agent     (1000)      894 2024-05-22 21:02:35.000000 polarion-1.4.0/polarion.egg-info/SOURCES.txt
+-rw-r--r--   0 agent     (1000) agent     (1000)        1 2024-05-22 21:02:35.000000 polarion-1.4.0/polarion.egg-info/dependency_links.txt
+-rw-r--r--   0 agent     (1000) agent     (1000)       20 2024-05-22 21:02:35.000000 polarion-1.4.0/polarion.egg-info/requires.txt
+-rw-r--r--   0 agent     (1000) agent     (1000)       15 2024-05-22 21:02:35.000000 polarion-1.4.0/polarion.egg-info/top_level.txt
+-rw-r--r--   0 agent     (1000) agent     (1000)      103 2024-05-22 21:02:24.000000 polarion-1.4.0/pyproject.toml
+-rw-r--r--   0 agent     (1000) agent     (1000)      688 2024-05-22 21:02:35.998044 polarion-1.4.0/setup.cfg
+-rw-r--r--   0 agent     (1000) agent     (1000)      954 2024-05-22 21:02:24.000000 polarion-1.4.0/setup.py
+drwxr-xr-x   0 agent     (1000) agent     (1000)        0 2024-05-22 21:02:35.998044 polarion-1.4.0/tests/
+-rw-r--r--   0 agent     (1000) agent     (1000)        0 2024-05-22 21:02:24.000000 polarion-1.4.0/tests/__init__.py
+-rw-r--r--   0 agent     (1000) agent     (1000)      134 2024-05-22 21:02:24.000000 polarion-1.4.0/tests/keys_template.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     9353 2024-05-22 21:02:24.000000 polarion-1.4.0/tests/test_junit.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     4586 2024-05-22 21:02:24.000000 polarion-1.4.0/tests/test_polarion_client.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     6059 2024-05-22 21:02:24.000000 polarion-1.4.0/tests/test_polarion_document.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     5669 2024-05-22 21:02:24.000000 polarion-1.4.0/tests/test_polarion_plan.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     3150 2024-05-22 21:02:24.000000 polarion-1.4.0/tests/test_polarion_project.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     7733 2024-05-22 21:02:24.000000 polarion-1.4.0/tests/test_polarion_test_record.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     5134 2024-05-22 21:02:24.000000 polarion-1.4.0/tests/test_polarion_testrun.py
+-rw-r--r--   0 agent     (1000) agent     (1000)      757 2024-05-22 21:02:24.000000 polarion-1.4.0/tests/test_polarion_user.py
+-rw-r--r--   0 agent     (1000) agent     (1000)     3768 2024-05-22 21:02:24.000000 polarion-1.4.0/tests/test_polarion_utils.py
+-rw-r--r--   0 agent     (1000) agent     (1000)    33496 2024-05-22 21:02:24.000000 polarion-1.4.0/tests/test_polarion_workitem.py
```

### Comparing `polarion-1.3.0/LICENSE` & `polarion-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/PKG-INFO` & `polarion-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarion
-Version: 1.3.0
+Version: 1.4.0
 Summary: Polarion client for Python
 Home-page: https://github.com/jesper-raemaekers/python-polarion
 Author: Jesper Raemaekers
 Author-email: j.raemaekers@relek.nl
 Project-URL: Bug Tracker, https://github.com/jesper-raemaekers/python-polarion/issues
 Project-URL: Documentation, https://python-polarion.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `polarion-1.3.0/README.md` & `polarion-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/polarion/base/comments.py` & `polarion-1.4.0/polarion/base/comments.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/polarion/base/custom_fields.py` & `polarion-1.4.0/polarion/base/custom_fields.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/polarion/document.py` & `polarion-1.4.0/polarion/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     def exportDocumentToPDF(self):
         """
         Download a PDF export of the document.
         :return: bytes
         """
         service = self._polarion.getService('Tracker')
-        pdf_props_obj = self._polarion.PdfProperties('A4', 'Portrait', True, True, True)
+        pdf_props_obj = self._polarion.PdfProperties('A4', 'Portrait', True, True, True, True)
         serialized_pdf_props = serialize_object(pdf_props_obj)
         pdf = service.exportDocumentToPDF(self._uri, serialized_pdf_props)
         return pdf
 
     def getWorkitemUris(self):
         """
         Get the uris of all workitems in the document.
```

### Comparing `polarion-1.3.0/polarion/factory.py` & `polarion-1.4.0/polarion/factory.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/polarion/plan.py` & `polarion-1.4.0/polarion/plan.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/polarion/polarion.py` & `polarion-1.4.0/polarion/polarion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import atexit
 import re
 from urllib.parse import urljoin, urlparse
 import requests
-from zeep import Client, Transport
+import tempfile
+import os
+from zeep import Client, CachingClient
 from zeep.plugins import HistoryPlugin
 
 from .project import Project
 import logging
 logger = logging.getLogger(__name__)
 
 _baseServiceUrl = 'ws/services'
@@ -23,23 +25,25 @@
     :param static_service_list: Set to True when this class may not use a request to get the services list
     :param verify_certificate: Set to True/False to activate certification validation for TLS connection or provide string with link to certification chain (PEM & x264 encoded)
     :param svn_repo_url: Set to the correct url when the SVN repo is not accessible via <host>/repo. For example http://example/repo_extern
     :param proxy: Set to a proxy address to use a proxy, use the format: proxy='ip:port'
     """
 
     def __init__(self, polarion_url, user, password=None, token=None, static_service_list=False, verify_certificate=True,
-                 svn_repo_url=None, proxy=None, request_session=None):
+                 svn_repo_url=None, proxy=None, request_session=None, cache=False):
         self.user = user
         self.password = password
         self.token = token
         self.url = polarion_url
         self.verify_certificate = verify_certificate
         self.svn_repo_url = svn_repo_url
         self.proxy = None
         self.request_session = request_session
+        self.cache = cache
+        self.transport = None
         if proxy is not None:
             self.proxy = {
                 'http': proxy,
                 'https': proxy}
 
         self.services = {}
 
@@ -86,18 +90,17 @@
 
     def _createSession(self):
         """
         Starts a session with the specified user/password
         """
         if 'Session' in self.services:
             self.history = HistoryPlugin()
-            self.services['Session']['client'] = Client(
-                self.services['Session']['url'] + '?wsdl', plugins=[self.history], transport=self._getTransport())
+            self.services['Session']['client'] = self.get_client('Session',[self.history])
             if self.proxy is not None:
-                self.services['Session']['client'] .transport.session.proxies = self.proxy
+                self.services['Session']['client'].transport.session.proxies = self.proxy
             try:
                 self.sessionHeaderElement = None
                 self.sessionCookieJar = None
                 if self.token is not None:
                     self.services['Session']['client'].service.logInWithToken(
                         "AccessToken", "", self.token)
                 else:
@@ -112,26 +115,34 @@
                 raise Exception(
                     f'Could not log in to Polarion for user {self.user}')
             if self.sessionHeaderElement is not None:
                 self._updateServices()
         else:
             raise Exception(
                 'Cannot login because WSDL has no SessionWebService')
+    
+    def get_client(self,service,plugins=[]):
+        client = None
+        if self.cache:
+            client = CachingClient(self.services[service]['url'] + '?wsdl', plugins=plugins)
+        else:
+            client = Client(self.services[service]['url'] + '?wsdl', plugins=plugins)
+        client.transport.session.verify = self.verify_certificate
+        return client
 
     def _updateServices(self):
         """
         Updates all services with the correct session ID
         """
         if self.sessionHeaderElement is None:
             raise Exception('Cannot update services when not logged in')
         for service in self.services:
             if service != 'Session':
                 if 'client' not in service:
-                    self.services[service]['client'] = Client(
-                        self.services[service]['url'] + '?wsdl', transport=self._getTransport())
+                    self.services[service]['client'] = self.get_client(service)
                 self.services[service]['client'].set_default_soapheaders(
                     [self.sessionHeaderElement])
                 if self.proxy is not None:
                     self.services[service]['client'].transport.session.proxies = self.proxy
                 self.services[service]['client'].transport.session.cookies = self.sessionCookieJar
             if service == 'Tracker':
                 if hasattr(self.services[service]['client'].service, 'addComment'):
@@ -185,33 +196,25 @@
         If is was not able to get it from Polarion, fail with a exception only when using this feature
         @return: PdfProperties
         """
         if self._PdfProperties is None:
             raise Exception(f'PDF not supported in this Polarion version')
         return self._PdfProperties
 
-    def _getTransport(self):
-        """
-        Gets the zeep transport object
-        """
-        transport = Transport(session=self.request_session)
-        transport.session.verify = self.verify_certificate
-        return transport
-
     def hasService(self, name: str):
         """
         Checks if a WSDL service is available
         """
         if name in self.services:
             return True
         return False
 
     def getService(self, name: str):
         """
-        Get a WSDL service client. The name can be 'Trakcer' or 'Session'
+        Get a WSDL service client. The name can be 'Tracker' or 'Session'
         """
         # request user info to see if we're still logged in
         try:
             _user = self.services['Project']['client'].service.getUser(self.user)
         except Exception:
             # if not, create a new session
             self._createSession()
```

### Comparing `polarion-1.3.0/polarion/project.py` & `polarion-1.4.0/polarion/project.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/polarion/record.py` & `polarion-1.4.0/polarion/record.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/polarion/testrun.py` & `polarion-1.4.0/polarion/testrun.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/polarion/user.py` & `polarion-1.4.0/polarion/user.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/polarion/utils.py` & `polarion-1.4.0/polarion/utils.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/polarion/workitem.py` & `polarion-1.4.0/polarion/workitem.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,17 +120,18 @@
                     columns = []
                     self._parsed_test_steps = []
                     for col in self._polarion_test_steps.keys.EnumOptionId:
                         columns.append(col.id)
                     # now parse the rows
                     for row in self._polarion_test_steps.steps.TestStep:
                         current_row = {}
-                        for col_id in range(len(row.values.Text)):
-                            current_row[columns[col_id]] = row.values.Text[col_id].content
-                        self._parsed_test_steps.append(current_row)
+                        if row.values is not None:
+                            for col_id in range(len(row.values.Text)):
+                                current_row[columns[col_id]] = row.values.Text[col_id].content
+                            self._parsed_test_steps.append(current_row)
         else:
             raise Exception(f'Workitem not retrieved from Polarion')
 
     def getAuthor(self):
         """
         Get the author of the workitem
```

### Comparing `polarion-1.3.0/polarion/xml.py` & `polarion-1.4.0/polarion/xml.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import xml.etree.ElementTree as ET
 from .polarion import Polarion
 from .record import Record
 from datetime import datetime
 import logging, json
+import re
 logger = logging.getLogger(__name__)
 
 class Config:
     """
     Config structure for xml importer.
     """
     XML_FILE='xml_file'                                 # Xml file to import
@@ -17,19 +18,22 @@
     PROJECT_ID='project_id'                             # id of the project
     TESTRUN_ID='testrun_id'                             # id of the test run (if you want to use and existing one)
     TESTRUN_ID_GENERATOR='testrun_id_generator'         # function that generate the testrun_id (config as parameter) if testrun_id is not provided. If not set: f'unit-{datetime.now}'
     TESTRUN_TITLE='testrun_title'                       # title of the test run if testrun is created. If not set 'New unit test run'
     TESTRUN_TYPE='testrun_type'                         # type of the test run if testrun is created. If not set 'xUnit Test Manual Upload'
     TESTRUN_COMMENT='testrun_comment'                   # test run comment to add if set.
     SKIP_MISSING_TESTCASE='skip_missing_testcase'       # if set to True, skip result on unknown test cases
+    VERIFY_CERT ='verify_cert'                          # verify or not the cert
+    USE_CACHE ='use_cache'                              # verify or not the cert
     ATTRIBUTES = [
         XML_FILE, URL, USERNAME, PASSWORD, TOKEN, 
         PROJECT_ID, TESTRUN_ID, TESTRUN_ID_GENERATOR,
-        TESTRUN_TITLE, TESTRUN_TYPE, TESTRUN_COMMENT, SKIP_MISSING_TESTCASE]
+        TESTRUN_TITLE, TESTRUN_TYPE, TESTRUN_COMMENT, SKIP_MISSING_TESTCASE, VERIFY_CERT, USE_CACHE]
     MANDATORY = [XML_FILE, URL, PROJECT_ID]  # and also either user/password or token
+    
     _classinitialised = False
 
     def __new__(cls, *args, **kwargs):
         if not Config._classinitialised:
             # Add properties dynamicaly
             for attr in Config.ATTRIBUTES:
                 eval(f'setattr(Config, "{attr}", property(lambda self: self._data["{attr}"] if "{attr}" in self._data.keys() else Config._default_value("{attr}")))')
@@ -40,14 +44,18 @@
     def _default_value(cls, attribute_name):
         if attribute_name==Config.TESTRUN_TITLE:
             return 'New unit test run'
         elif attribute_name==Config.TESTRUN_TYPE:
             return 'xUnit Test Manual Upload'
         elif attribute_name==Config.SKIP_MISSING_TESTCASE:
             return False
+        elif attribute_name==Config.VERIFY_CERT:
+            return True
+        elif attribute_name==Config.USE_CACHE:
+            return False
         return None
 
     @classmethod
     def from_json(cls, json):
         """
         Create config from a json file
         """
@@ -57,14 +65,15 @@
     @classmethod
     def from_dict(cls, data):
         """
         Create config from a dict
         """
         return Config(data)
 
+
     def __init__(self, data):
         """
         Init from existing data
 
         param data: dict to initialise.
         """
         self._data=data
@@ -80,22 +89,26 @@
     def generate_test_run_id(self):
         if getattr(self, Config.TESTRUN_ID) is None:
             if getattr(self, Config.TESTRUN_ID_GENERATOR) is not None:
                 self._data[Config.TESTRUN_ID]=getattr(self, Config.TESTRUN_ID_GENERATOR)(self)
             else:
                 self._data[Config.TESTRUN_ID]=f'unit-{datetime.now().strftime("%Y-%m-%d-%H-%M-%S-%f")}'
         return getattr(self, Config.TESTRUN_ID)
+    
 
 class XmlParser:
     """
     Xml parser for xml_junit.xsd format
     """
     TEST_SUITES='testsuites'
     TEST_SUITE='testsuite'
     TEST_CASE='testcase'
+    PROPERTIES='properties'
+    PROPERTY='property'
+    SYSOUT='system-out'
 
     @classmethod
     def parse_root(cls, xml_file):
         """
         Parse Xml file
         :return: List of cases for the file
         """
@@ -127,14 +140,29 @@
                 if child.tag == XmlParser.TEST_SUITE:
                     XmlParser._parse_suite(child, suite, returned_cases)
                 if child.tag == XmlParser.TEST_CASE:
                     XmlParser._parse_case(child, suite, returned_cases)
         else:
             raise Exception(f'Unmanaged {XmlParser.TEST_SUITE} {test_suite.tag} in {parent["path"]}')
 
+    # matches expressions like [[PROPERTY|verifies=REQ-001]]
+    RE_PATTTERN = re.compile("\\[\\[PROPERTY\\|(.*)\\=(.*)\\]\\]")
+
+    @classmethod
+    def tranform_string_properties(cls, value):
+        result = [] 
+        tmp =  XmlParser.RE_PATTTERN.findall(value)
+        for res in tmp:
+            if len(res) == 2:
+                result.append({
+                    "name":res[0],
+                    "value":res[1]
+                }) 
+        return result
+
     @classmethod
     def _parse_case(cls, test_case, parent, returned_cases):
         if test_case.tag == XmlParser.TEST_CASE:
             case=parent.copy()
             case.update({ 'path': f'{parent["path"]}/{XmlParser.TEST_CASE}{XmlParser._xmlnode_name(test_case)}' })
             # id
             if 'name' not in test_case.attrib.keys() or 'classname' not in test_case.attrib.keys():
@@ -142,64 +170,77 @@
                 return
             case.update({ 'id': test_case.attrib['classname']+'.'+test_case.attrib['name'] })
             
             # time
             if 'time' in test_case.attrib.keys():
                 case.update({ 'time': test_case.attrib['time'] })
             
-            # error & failure
+            # error & failure & properties
             for elem in test_case:
-                if elem.tag in ['error', 'failure']:
+                if elem.tag in ['error', 'failure','skipped']:
                     text = []
                     for attrib in ['type', 'message']:
                         if attrib in elem.attrib.keys(): text.append(elem.attrib[attrib])
-                    text.append(elem.text)
+                    if elem.text is not None:
+                        text.append(elem.text)
                     case.update({ elem.tag: '\n'.join(text)})
+                elif elem.tag == XmlParser.PROPERTIES:
+                    if "properties" not in case:
+                        case.update({'properties':[]})
+                    for property in elem:
+                        if XmlParser.PROPERTY == property.tag and 'name' in property.attrib.keys() and 'value' in property.attrib.keys():
+                            case['properties'].append({property.get('name') : property.get('value')})
+                elif elem.tag == XmlParser.SYSOUT:
+                    if "properties" not in case:
+                        case.update({'properties':[]})
+                    for property in XmlParser.tranform_string_properties(elem.text):
+                        case['properties'].append({property['name'] : property['value']})
             returned_cases.append(case)
         else:
             raise Exception(f'Unmanaged {XmlParser.TEST_CASE} {test_case.tag} in {parent["path"]}')
 
     @classmethod
     def _xmlnode_name(cls, node):
         """
         Build name of the xmlnode
         """
         if 'name' in node.attrib.keys():
             return f'{node.tag}[name={node.attrib["name"]}]'
         return node.tag
-
+    
 class Importer:
     """
     Import xml file to polarion using a config
     """
-    TEST_CASE_ID_CUSTOM_FILED='testCaseID'
+    TEST_CASE_ID_CUSTOM_FIELD='testCaseID'
     TEST_CASE_TYPE='type:testcase'
     TEST_CASE_WI_TYPE='testcase'
     TEST_CASE_WI_TITLE='title'
     TEST_RUN_COMMENT_CUSTOM_FIELD='environmentDescription'
 
     @classmethod
     def from_xml(cls, config):
         """
         Import xml file having junit.xsd structure (see documentation)
         """
         logger.info(f'Parsing test file {config.xml_file}')
         cases=XmlParser.parse_root(config.xml_file)
 
         logger.info(f'Connection to polarion {config.url} on project {config.project_id}')
-        polarion=Polarion(polarion_url=config.url, user=config.username, password=config.password, token=config.token)
+
+        polarion=Polarion(polarion_url=config.url, user=config.username, password=config.password, token=config.token, verify_certificate=config.verify_cert, cache=config.use_cache)
         project=polarion.getProject(config.project_id)
 
         # Indexing existing cases with custom field '
-        test_cases=project.searchWorkitem(Importer.TEST_CASE_TYPE, field_list=['id', f'customFields.{Importer.TEST_CASE_ID_CUSTOM_FILED}'])
+        test_cases=project.searchWorkitem(Importer.TEST_CASE_TYPE, field_list=['id', f'customFields.{Importer.TEST_CASE_ID_CUSTOM_FIELD}'])
         test_cases_from_id={}
         for test_case in test_cases:
             if hasattr(test_case,'customFields') and hasattr(test_case.customFields,'Custom'):
                 for custom in test_case.customFields.Custom:
-                    if getattr(custom, 'key', None) == Importer.TEST_CASE_ID_CUSTOM_FILED and hasattr(custom,'value'):
+                    if getattr(custom, 'key', None) == Importer.TEST_CASE_ID_CUSTOM_FIELD and hasattr(custom,'value'):
                         test_cases_from_id[custom.value]=test_case.id
 
         # Getting or creating test run
         if config.testrun_id is None:
             config.generate_test_run_id()
             logger.info(f'Creating testrun {config.testrun_id}')
             test_run=project.createTestRun(config.testrun_id, config.testrun_title, config.testrun_type)
@@ -218,40 +259,72 @@
                     if len(split)==2:
                         comment=split[0]+'<br>'+config.testrun_comment+'</body></html>'
                     else:
                         logger.warn(f'unable to parse properly {Importer.TEST_RUN_COMMENT_CUSTOM_FIELD} of testrun: {comment}. So it is not updated')
             test_run.setCustomField(Importer.TEST_RUN_COMMENT_CUSTOM_FIELD, test_run._polarion.TextType(
                     content=comment, type='text/html', contentLossy=False))
 
+        # cache for work items traced
+        cache_for_workitems = {}
+
         # Filling
         logger.info('Saving results')
         for case in cases:
             if case['id'] not in test_cases_from_id.keys():
                 if config.skip_missing_testcase:
-                    logger.warn(f'Skipping case with {Importer.TEST_CASE_ID_CUSTOM_FILED} {case["id"]}')
+                    logger.warn(f'Skipping case with {Importer.TEST_CASE_ID_CUSTOM_FIELD} {case["id"]}')
                     continue
-                print(f'Creating case with {Importer.TEST_CASE_ID_CUSTOM_FILED} {case["id"]}')
+                print(f'Creating case with {Importer.TEST_CASE_ID_CUSTOM_FIELD} {case["id"]}')
                 wi_case=project.createWorkitem(workitem_type=Importer.TEST_CASE_WI_TYPE, new_workitem_fields={Importer.TEST_CASE_WI_TITLE: case['id']})
-                wi_case.setCustomField(key=Importer.TEST_CASE_ID_CUSTOM_FILED, value=case['id'])
+                wi_case.setCustomField(key=Importer.TEST_CASE_ID_CUSTOM_FIELD, value=case['id'])
             else:
                 wi_case=project.getWorkitem(test_cases_from_id[case['id']])
             test_run.addTestcase(wi_case)
             
             if 'time' in case.keys():
                 test_run.records[-1].duration=case['time']
 
             if 'timestamp' in case.keys():
                 test_run.records[-1].executed=case['timestamp']
 
             if 'failure' in case.keys():
                 test_run.records[-1].setResult(Record.ResultType.FAILED, case['failure'])
             elif 'error' in case.keys():
                 test_run.records[-1].setResult(Record.ResultType.BLOCKED, case['error'])
+            elif 'skipped' in case.keys():
+                test_run.records[-1].setResult(Record.ResultType.NOTTESTED, case['skipped'])
             else:
                 test_run.records[-1].setResult(Record.ResultType.PASSED)
+            
+            # handle traceability, because of API, traqceability must use default traceability role 
+            # and not the opposite one.
+            # traceability links are made using IDs or titles 
+            # this implementation does not allow traceability between test cases
+            if 'properties' in case.keys():
+                for property in case['properties']:
+                    for key in property.keys():
+                        linked_item = None
+                        title=property.get(key)
+                        if title in cache_for_workitems:
+                            linked_item = cache_for_workitems[title]
+                        else:
+                            try:
+                                linked_item=project.getWorkitem(property.get(key))
+                            except Exception:
+                                linked_items=project.searchWorkitem(query=f'title:{title}', field_list=['id','title'])
+                                if len(linked_items) > 0 and linked_items[0]['title']==title:
+                                    linked_item=linked_items[0]
+                                    # work item is reload to avoid isues of class not correctly loaded by search work item
+                                    linked_item=project.getWorkitem(linked_item['id'])
+                                else:
+                                    logger.error(f'impossible to link{wi_case.id} to {title}')
+                                cache_for_workitems[title] = linked_item
+                        if linked_item is not None:
+                            wi_case.addLinkedItem(linked_item, key)
+
         logger.info(f'Results saved in {config.url}/#/project/{config.project_id}/testrun?id={config.testrun_id}')
 
         return test_run
 
 class ResultExporter:
     """
     Export an object as a json (tested with a testrun)
```

### Comparing `polarion-1.3.0/polarion.egg-info/PKG-INFO` & `polarion-1.4.0/polarion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarion
-Version: 1.3.0
+Version: 1.4.0
 Summary: Polarion client for Python
 Home-page: https://github.com/jesper-raemaekers/python-polarion
 Author: Jesper Raemaekers
 Author-email: j.raemaekers@relek.nl
 Project-URL: Bug Tracker, https://github.com/jesper-raemaekers/python-polarion/issues
 Project-URL: Documentation, https://python-polarion.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `polarion-1.3.0/polarion.egg-info/SOURCES.txt` & `polarion-1.4.0/polarion.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 polarion.egg-info/top_level.txt
 polarion/base/__init__.py
 polarion/base/comments.py
 polarion/base/custom_fields.py
 polarion/base/polarion_object.py
 tests/__init__.py
 tests/keys_template.py
+tests/test_junit.py
 tests/test_polarion_client.py
 tests/test_polarion_document.py
 tests/test_polarion_plan.py
 tests/test_polarion_project.py
 tests/test_polarion_test_record.py
 tests/test_polarion_testrun.py
 tests/test_polarion_user.py
```

### Comparing `polarion-1.3.0/setup.cfg` & `polarion-1.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = polarion
-version = 1.3.0
+version = 1.4.0
 author = Jesper Raemaekers
 author_email = j.raemaekers@relek.nl
 description = Polarion client for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jesper-raemaekers/python-polarion
 project_urls =
```

### Comparing `polarion-1.3.0/setup.py` & `polarion-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="polarion",
-    version="1.3.0",
+    version="1.4.0",
     author="Jesper Raemaekers",
     author_email="j.raemaekers@relek.nl",
     description="Polarion client for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jesper-raemaekers/python-polarion",
     project_urls={
```

### Comparing `polarion-1.3.0/tests/test_polarion_client.py` & `polarion-1.4.0/tests/test_polarion_client.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/tests/test_polarion_document.py` & `polarion-1.4.0/tests/test_polarion_document.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/tests/test_polarion_plan.py` & `polarion-1.4.0/tests/test_polarion_plan.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/tests/test_polarion_project.py` & `polarion-1.4.0/tests/test_polarion_project.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/tests/test_polarion_test_record.py` & `polarion-1.4.0/tests/test_polarion_test_record.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/tests/test_polarion_testrun.py` & `polarion-1.4.0/tests/test_polarion_testrun.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/tests/test_polarion_user.py` & `polarion-1.4.0/tests/test_polarion_user.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/tests/test_polarion_utils.py` & `polarion-1.4.0/tests/test_polarion_utils.py`

 * *Files identical despite different names*

### Comparing `polarion-1.3.0/tests/test_polarion_workitem.py` & `polarion-1.4.0/tests/test_polarion_workitem.py`

 * *Files identical despite different names*

