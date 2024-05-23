# Comparing `tmp/easykube-0.3.1.tar.gz` & `tmp/easykube-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easykube-0.3.1.tar", last modified: Tue Apr 30 15:13:14 2024, max compression
+gzip compressed data, was "easykube-0.3.2.tar", last modified: Thu May 23 16:53:43 2024, max compression
```

## Comparing `easykube-0.3.1.tar` & `easykube-0.3.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.774824 easykube-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.766824 easykube-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.770824 easykube-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-30 15:13:10.000000 easykube-0.3.1/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 15:13:10.000000 easykube-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 15:13:10.000000 easykube-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-30 15:13:14.774824 easykube-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 15:13:10.000000 easykube-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.770824 easykube-0.3.1/easykube/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/flow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.770824 easykube-0.3.1/easykube/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.770824 easykube-0.3.1/easykube/kubernetes/client/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.770824 easykube-0.3.1/easykube/rest/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/rest/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/rest/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/rest/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/rest/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.770824 easykube-0.3.1/easykube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-30 15:13:14.000000 easykube-0.3.1/easykube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-30 15:13:14.000000 easykube-0.3.1/easykube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:13:14.000000 easykube-0.3.1/easykube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:13:14.000000 easykube-0.3.1/easykube.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 15:13:14.000000 easykube-0.3.1/easykube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 15:13:14.000000 easykube-0.3.1/easykube.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-30 15:13:10.000000 easykube-0.3.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-30 15:13:14.774824 easykube-0.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-04-30 15:13:10.000000 easykube-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:43.138375 easykube-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:43.134375 easykube-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:43.134375 easykube-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-23 16:53:39.000000 easykube-0.3.2/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 16:53:39.000000 easykube-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 16:53:39.000000 easykube-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-23 16:53:43.138375 easykube-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 16:53:39.000000 easykube-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:43.134375 easykube-0.3.2/easykube/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:43.134375 easykube-0.3.2/easykube/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:43.138375 easykube-0.3.2/easykube/kubernetes/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/kubernetes/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/kubernetes/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/kubernetes/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/kubernetes/client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/kubernetes/client/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/kubernetes/client/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/kubernetes/client/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/kubernetes/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:43.138375 easykube-0.3.2/easykube/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/rest/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/rest/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/rest/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-23 16:53:39.000000 easykube-0.3.2/easykube/rest/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:53:43.138375 easykube-0.3.2/easykube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-23 16:53:43.000000 easykube-0.3.2/easykube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-23 16:53:43.000000 easykube-0.3.2/easykube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:53:43.000000 easykube-0.3.2/easykube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:53:42.000000 easykube-0.3.2/easykube.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 16:53:43.000000 easykube-0.3.2/easykube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 16:53:43.000000 easykube-0.3.2/easykube.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-23 16:53:39.000000 easykube-0.3.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-05-23 16:53:43.138375 easykube-0.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-23 16:53:39.000000 easykube-0.3.2/setup.py
```

### Comparing `easykube-0.3.1/.github/workflows/pypi-publish.yaml` & `easykube-0.3.2/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/LICENSE` & `easykube-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/easykube/flow.py` & `easykube-0.3.2/easykube/flow.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/easykube/kubernetes/client/api.py` & `easykube-0.3.2/easykube/kubernetes/client/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,22 @@
         if self._resources is None:
             prefix = "/apis" if "/" in self._api_version else "/api"
             response = yield self._client.get(f"{prefix}/{self._api_version}")
             self._resources = { r["name"]: r for r in response.json()["resources"] }
         return self._resources
 
     @flow
+    def resources(self):
+        """
+        Returns the resources for the API.
+        """
+        resources = yield self._ensure_resources()
+        return resources.values()
+
+    @flow
     def resource(self, name):
         """
         Returns a resource for the given name.
 
         The given name can be either the plural name, the singular name or the kind.
         Lookups by plural name will be faster as that is the key that is indexed.
         """
```

### Comparing `easykube-0.3.1/easykube/kubernetes/client/client.py` & `easykube-0.3.2/easykube/kubernetes/client/client.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/easykube/kubernetes/client/errors.py` & `easykube-0.3.2/easykube/kubernetes/client/errors.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/easykube/kubernetes/client/iterators.py` & `easykube-0.3.2/easykube/kubernetes/client/iterators.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/easykube/kubernetes/client/resource.py` & `easykube-0.3.2/easykube/kubernetes/client/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,26 @@
         data.setdefault("apiVersion", self._api_version)
         data.setdefault("kind", self._kind)
         # Set the name in metadata to the given id
         if id:
             data.setdefault("metadata", {}).update(name = id)
         return data
 
+    @property
+    def api_version(self):
+        return self._api_version
+
+    @property
+    def kind(self):
+        return self._kind
+
+    @property
+    def namespaced(self):
+        return self._namespaced
+
     def create(self, data, /, namespace = None):
         namespace = namespace or data.get("metadata", {}).get("namespace")
         return super().create(data, namespace = namespace)
 
     def fetch(self, id, /, namespace = None, **params):
         return super().fetch(id, namespace = namespace, **params)
```

### Comparing `easykube-0.3.1/easykube/kubernetes/client/spec.py` & `easykube-0.3.2/easykube/kubernetes/client/spec.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/easykube/kubernetes/config.py` & `easykube-0.3.2/easykube/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/easykube/kubernetes/resources.py` & `easykube-0.3.2/easykube/kubernetes/resources.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/easykube/rest/client.py` & `easykube-0.3.2/easykube/rest/client.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/easykube/rest/iterators.py` & `easykube-0.3.2/easykube/rest/iterators.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/easykube/rest/resource.py` & `easykube-0.3.2/easykube/rest/resource.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/easykube/rest/util.py` & `easykube-0.3.2/easykube/rest/util.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.1/easykube.egg-info/SOURCES.txt` & `easykube-0.3.2/easykube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

