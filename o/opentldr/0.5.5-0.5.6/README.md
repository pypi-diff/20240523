# Comparing `tmp/opentldr-0.5.5.tar.gz` & `tmp/opentldr-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentldr-0.5.5.tar", last modified: Wed May 22 14:58:40 2024, max compression
+gzip compressed data, was "opentldr-0.5.6.tar", last modified: Thu May 23 14:30:30 2024, max compression
```

## Comparing `opentldr-0.5.5.tar` & `opentldr-0.5.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:40.726451 opentldr-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 14:58:36.000000 opentldr-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:36.000000 opentldr-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-22 14:58:40.726451 opentldr-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-05-22 14:58:36.000000 opentldr-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-22 14:58:36.000000 opentldr-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:58:40.726451 opentldr-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:40.718450 opentldr-0.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:40.722450 opentldr-0.5.5/src/opentldr/
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/AbstractDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/DataRepoJson.py
--rw-r--r--   0 runner    (1001) docker     (127)    28557 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/Domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/FileSystemDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)    37495 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/KnowledgeGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/S3DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/Workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:40.726451 opentldr-0.5.5/src/opentldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-22 14:58:40.000000 opentldr-0.5.5/src/opentldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-22 14:58:40.000000 opentldr-0.5.5/src/opentldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:58:40.000000 opentldr-0.5.5/src/opentldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-22 14:58:40.000000 opentldr-0.5.5/src/opentldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 14:58:40.000000 opentldr-0.5.5/src/opentldr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:40.726451 opentldr-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 14:58:36.000000 opentldr-0.5.5/tests/test_contentrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 14:58:36.000000 opentldr-0.5.5/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-22 14:58:36.000000 opentldr-0.5.5/tests/test_knowledgegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-22 14:58:36.000000 opentldr-0.5.5/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:30:30.093306 opentldr-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 14:30:25.000000 opentldr-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:30:25.000000 opentldr-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-23 14:30:30.093306 opentldr-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-05-23 14:30:25.000000 opentldr-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-23 14:30:25.000000 opentldr-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:30:30.093306 opentldr-0.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:30:30.085306 opentldr-0.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:30:30.089306 opentldr-0.5.6/src/opentldr/
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/AbstractDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/DataRepoJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28557 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/Domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/FileSystemDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38066 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/KnowledgeGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/S3DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/Workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-23 14:30:25.000000 opentldr-0.5.6/src/opentldr/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:30:30.093306 opentldr-0.5.6/src/opentldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-23 14:30:30.000000 opentldr-0.5.6/src/opentldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-23 14:30:30.000000 opentldr-0.5.6/src/opentldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:30:30.000000 opentldr-0.5.6/src/opentldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 14:30:30.000000 opentldr-0.5.6/src/opentldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 14:30:30.000000 opentldr-0.5.6/src/opentldr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:30:30.093306 opentldr-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 14:30:25.000000 opentldr-0.5.6/tests/test_contentrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 14:30:25.000000 opentldr-0.5.6/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-23 14:30:25.000000 opentldr-0.5.6/tests/test_knowledgegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-23 14:30:25.000000 opentldr-0.5.6/tests/test_workflow.py
```

### Comparing `opentldr-0.5.5/LICENSE` & `opentldr-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.5/PKG-INFO` & `opentldr-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.5.5
+Version: 0.5.6
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opentldr-0.5.5/README.md` & `opentldr-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.5/pyproject.toml` & `opentldr-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "opentldr"
-version = "0.5.5"
+version = "0.5.6"
 authors = [
   { name="Chris Argenta", email="cargenta@rockfishresearch.com" },
 ]
 description = "An open framework for creation of a Tailored Daily Report."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `opentldr-0.5.5/src/opentldr/AbstractDataRepo.py` & `opentldr-0.5.6/src/opentldr/AbstractDataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.5/src/opentldr/DataRepo.py` & `opentldr-0.5.6/src/opentldr/DataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.5/src/opentldr/DataRepoJson.py` & `opentldr-0.5.6/src/opentldr/DataRepoJson.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.5/src/opentldr/Domain.py` & `opentldr-0.5.6/src/opentldr/Domain.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.5/src/opentldr/FileSystemDataRepo.py` & `opentldr-0.5.6/src/opentldr/FileSystemDataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.5/src/opentldr/KnowledgeGraph.py` & `opentldr-0.5.6/src/opentldr/KnowledgeGraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     KnowledgeGraph is the API for OpenTLDR's interface to Neo4j graph database. It attempts to make the
     driver connection using OS, .env, and then default values for connections. This API maps neo4j
     nodes/edges to types specified in the Domain module (using Neomodel OGM and some custom cypher).
 
     In order to be successful, you will need to have a neo4j server running, reachable on the network,
     and with environment variables (either in OS or .env files) similar to these:
 
-        NEO4J_CONNECTION='bolt://localhost:7687'
+        NEO4J_CONNECTION='neo4j://localhost:7687'
         NEO4J_USERNAME=neo4jUser
         NEO4J_PASSWORD=neo4jPassword
         NEO4J_DATABASE=neo4j
 
     This class can be used in several different ways, including:
         (1) import opentldr.KnowledgeGraph ... kg=KnowledgeGraph() ... (use kg here) ... kg.close() 
         (2) with opentldr.KnowledgeGraph as kg: ... (use kg here, and then it will autoclose)
@@ -486,14 +486,16 @@
     def get_all_content(self) -> list[Content]:
         content = Content.nodes
         return content
 
     def delete_content(self, content:Content):
         for e in self.get_entities_by_content(content):
             self.delete_entity(e)
+        for k in self.get_evalkeys_by_content(content):
+            self.delete_evalkey(k)
         return self.delete_content_by_uid(content.uid)
 
     def delete_content_by_uid(self, uid:str):
         return self.cypher_query('''
             MATCH (c:Content) WHERE c.uid=$uid
             DETACH DELETE c ''',
             params={"uid": uid})
@@ -648,14 +650,18 @@
     def get_all_requests(self) -> list[Request]:
         requests = Request.nodes
         return requests
 
     def delete_request(self,request:Request):
         for e in self.get_entities_by_request(request):
             self.delete_entity(e)
+        for t in self.get_tldr_by_request(request):
+            self.delete_tldr(t)
+        for k in self.get_evalkeys_by_request(request):
+            self.delete_evalkey(k)   
         return self.delete_request_by_uid(request.uid)
     
     def delete_request_by_uid(self,uid:str):
         return self.cypher_query('''
             MATCH (r:Request) WHERE r.uid=$uid
             DETACH DELETE r ''',
             params={"uid": uid})
@@ -944,25 +950,32 @@
 
     def add_evalkey(self, content:Content, request:Request, score:float, text:str) -> EvalKey:
         key = EvalKey(text=text, score=score).save()
         key.key_for_content.connect(content)
         key.key_for_request.connect(request)
         return key
 
-    def get_evalkey_by_uid(self, uid: str) -> Content:
+    def get_evalkey_by_uid(self, uid: str) -> EvalKey:
         key = EvalKey.nodes.get_or_none(uid=uid)
         return key
 
-    def get_evalkeys_by_request(self, request: Request) -> list[Content]:
+    def get_evalkeys_by_request(self, request: Request) -> list[EvalKey]:
         return self.cypher_query("""
             MATCH (q:Request) WHERE q.uid=$request_id
             MATCH (e:EvalKey)-[eq:KEY_FOR_REQUEST]->(q)
             RETURN e """,
             "e", params={"request_id": request.uid})
 
+    def get_evalkeys_by_content(self, content: Content) -> list[EvalKey]:
+        return self.cypher_query("""
+            MATCH (c:Content) WHERE c.uid=$content_id
+            MATCH (c)<-[ec:KEY_FOR_CONTENT]-(e:EvalKey)
+            RETURN e """,
+            "e", params={"content_id": content.uid})
+
     def get_evalkey_by_content_and_request(self, content: Content, request: Request) -> EvalKey:
         return self.cypher_query_one("""
             MATCH (c:Content) WHERE c.uid=$content_id
             MATCH (q:Request) WHERE q.uid=$request_id
             MATCH (c)<-[ec:KEY_FOR_CONTENT]-(e:EvalKey)-[eq:KEY_FOR_REQUEST]->(q)
             RETURN e """,
             "e", params={
```

### Comparing `opentldr-0.5.5/src/opentldr/S3DataRepo.py` & `opentldr-0.5.6/src/opentldr/S3DataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.5/src/opentldr/Workflow.py` & `opentldr-0.5.6/src/opentldr/Workflow.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.5/src/opentldr.egg-info/PKG-INFO` & `opentldr-0.5.6/src/opentldr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.5.5
+Version: 0.5.6
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opentldr-0.5.5/src/opentldr.egg-info/SOURCES.txt` & `opentldr-0.5.6/src/opentldr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.5/tests/test_knowledgegraph.py` & `opentldr-0.5.6/tests/test_knowledgegraph.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.5/tests/test_workflow.py` & `opentldr-0.5.6/tests/test_workflow.py`

 * *Files identical despite different names*

