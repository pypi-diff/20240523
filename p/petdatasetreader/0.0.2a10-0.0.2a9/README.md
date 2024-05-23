# Comparing `tmp/petdatasetreader-0.0.2a10.tar.gz` & `tmp/petdatasetreader-0.0.2a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petdatasetreader-0.0.2a10.tar", last modified: Wed Nov  9 15:11:37 2022, max compression
+gzip compressed data, was "petdatasetreader-0.0.2a9.tar", last modified: Thu Oct 27 13:48:56 2022, max compression
```

## Comparing `petdatasetreader-0.0.2a10.tar` & `petdatasetreader-0.0.2a9.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2022-11-09 15:11:37.240635 petdatasetreader-0.0.2a10/
--rw-r--r--   0 patrizio   (501) staff       (20)        0 2022-05-10 20:52:11.000000 petdatasetreader-0.0.2a10/LICENSE.txt
--rw-r--r--   0 patrizio   (501) staff       (20)     1874 2022-11-09 15:11:37.240480 petdatasetreader-0.0.2a10/PKG-INFO
--rw-r--r--   0 patrizio   (501) staff       (20)      410 2022-10-27 13:48:55.000000 petdatasetreader-0.0.2a10/README.rst
-drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2022-11-09 15:11:37.238496 petdatasetreader-0.0.2a10/petdatasetreader.egg-info/
--rw-r--r--   0 patrizio   (501) staff       (20)     1874 2022-11-09 15:11:36.000000 petdatasetreader-0.0.2a10/petdatasetreader.egg-info/PKG-INFO
--rw-r--r--   0 patrizio   (501) staff       (20)      461 2022-11-09 15:11:37.000000 petdatasetreader-0.0.2a10/petdatasetreader.egg-info/SOURCES.txt
--rw-r--r--   0 patrizio   (501) staff       (20)        1 2022-11-09 15:11:36.000000 petdatasetreader-0.0.2a10/petdatasetreader.egg-info/dependency_links.txt
--rw-r--r--   0 patrizio   (501) staff       (20)        9 2022-11-09 15:11:37.000000 petdatasetreader-0.0.2a10/petdatasetreader.egg-info/requires.txt
--rw-r--r--   0 patrizio   (501) staff       (20)       10 2022-11-09 15:11:37.000000 petdatasetreader-0.0.2a10/petdatasetreader.egg-info/top_level.txt
-drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2022-11-09 15:11:37.240250 petdatasetreader-0.0.2a10/petreader/
--rw-r--r--   0 patrizio   (501) staff       (20)    10899 2022-11-09 15:11:17.000000 petdatasetreader-0.0.2a10/petreader/ProcessInformation.py
--rw-r--r--   0 patrizio   (501) staff       (20)    12299 2022-06-27 08:39:36.000000 petdatasetreader-0.0.2a10/petreader/RelationsExtraction.py
--rw-r--r--   0 patrizio   (501) staff       (20)    20893 2022-06-27 10:46:21.000000 petdatasetreader-0.0.2a10/petreader/TokenClassification.py
--rw-r--r--   0 patrizio   (501) staff       (20)        0 2022-06-13 09:21:17.000000 petdatasetreader-0.0.2a10/petreader/__init__.py
--rw-r--r--   0 patrizio   (501) staff       (20)     1972 2022-10-27 15:16:38.000000 petdatasetreader-0.0.2a10/petreader/_gold_labels.py
--rw-r--r--   0 patrizio   (501) staff       (20)      327 2022-10-25 21:48:57.000000 petdatasetreader-0.0.2a10/petreader/colors.py
--rw-r--r--   0 patrizio   (501) staff       (20)     4675 2022-11-09 14:30:39.000000 petdatasetreader-0.0.2a10/petreader/labels.py
--rw-r--r--   0 patrizio   (501) staff       (20)     2966 2022-10-25 21:11:58.000000 petdatasetreader-0.0.2a10/petreader/petdataset.py
--rw-r--r--   0 patrizio   (501) staff       (20)     5651 2022-11-09 15:11:17.000000 petdatasetreader-0.0.2a10/petreader/utility.py
--rw-r--r--   0 patrizio   (501) staff       (20)       38 2022-11-09 15:11:37.240680 petdatasetreader-0.0.2a10/setup.cfg
--rw-r--r--   0 patrizio   (501) staff       (20)     2148 2022-11-09 15:11:30.000000 petdatasetreader-0.0.2a10/setup.py
+drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2022-10-27 13:48:56.354571 petdatasetreader-0.0.2a9/
+-rw-r--r--   0 patrizio   (501) staff       (20)        0 2022-05-10 20:52:11.000000 petdatasetreader-0.0.2a9/LICENSE.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)     1873 2022-10-27 13:48:56.354398 petdatasetreader-0.0.2a9/PKG-INFO
+-rw-r--r--   0 patrizio   (501) staff       (20)      410 2022-10-27 13:48:55.000000 petdatasetreader-0.0.2a9/README.rst
+drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2022-10-27 13:48:56.350598 petdatasetreader-0.0.2a9/petdatasetreader.egg-info/
+-rw-r--r--   0 patrizio   (501) staff       (20)     1873 2022-10-27 13:48:55.000000 petdatasetreader-0.0.2a9/petdatasetreader.egg-info/PKG-INFO
+-rw-r--r--   0 patrizio   (501) staff       (20)      414 2022-10-27 13:48:56.000000 petdatasetreader-0.0.2a9/petdatasetreader.egg-info/SOURCES.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)        1 2022-10-27 13:48:56.000000 petdatasetreader-0.0.2a9/petdatasetreader.egg-info/dependency_links.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)        9 2022-10-27 13:48:56.000000 petdatasetreader-0.0.2a9/petdatasetreader.egg-info/requires.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)       10 2022-10-27 13:48:56.000000 petdatasetreader-0.0.2a9/petdatasetreader.egg-info/top_level.txt
+drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2022-10-27 13:48:56.354141 petdatasetreader-0.0.2a9/petreader/
+-rw-r--r--   0 patrizio   (501) staff       (20)    13884 2022-10-18 20:37:38.000000 petdatasetreader-0.0.2a9/petreader/ProcessInformation.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    12299 2022-06-27 08:39:36.000000 petdatasetreader-0.0.2a9/petreader/RelationsExtraction.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    20893 2022-06-27 10:46:21.000000 petdatasetreader-0.0.2a9/petreader/TokenClassification.py
+-rw-r--r--   0 patrizio   (501) staff       (20)        0 2022-06-13 09:21:17.000000 petdatasetreader-0.0.2a9/petreader/__init__.py
+-rw-r--r--   0 patrizio   (501) staff       (20)      327 2022-10-25 21:48:57.000000 petdatasetreader-0.0.2a9/petreader/colors.py
+-rw-r--r--   0 patrizio   (501) staff       (20)     4630 2022-10-25 21:50:17.000000 petdatasetreader-0.0.2a9/petreader/labels.py
+-rw-r--r--   0 patrizio   (501) staff       (20)     2966 2022-10-25 21:11:58.000000 petdatasetreader-0.0.2a9/petreader/petdataset.py
+-rw-r--r--   0 patrizio   (501) staff       (20)       38 2022-10-27 13:48:56.354618 petdatasetreader-0.0.2a9/setup.cfg
+-rw-r--r--   0 patrizio   (501) staff       (20)     2147 2022-10-25 20:40:59.000000 petdatasetreader-0.0.2a9/setup.py
```

### Comparing `petdatasetreader-0.0.2a10/PKG-INFO` & `petdatasetreader-0.0.2a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petdatasetreader
-Version: 0.0.2a10
+Version: 0.0.2a9
 Summary: Convenient interface that provides structured representations of the PET dataset hosted on Huggingface
 Home-page: https://pdi.fbk.eu/pet-dataset
 Author: Patrizio Bellan
 Author-email: patrizio.bellan@gmail.com
 Maintainer: Patrizio Bellan
 Maintainer-email: patrizio.bellan@gmail.com
 License: MIT
```

### Comparing `petdatasetreader-0.0.2a10/petdatasetreader.egg-info/PKG-INFO` & `petdatasetreader-0.0.2a9/petdatasetreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petdatasetreader
-Version: 0.0.2a10
+Version: 0.0.2a9
 Summary: Convenient interface that provides structured representations of the PET dataset hosted on Huggingface
 Home-page: https://pdi.fbk.eu/pet-dataset
 Author: Patrizio Bellan
 Author-email: patrizio.bellan@gmail.com
 Maintainer: Patrizio Bellan
 Maintainer-email: patrizio.bellan@gmail.com
 License: MIT
```

### Comparing `petdatasetreader-0.0.2a10/petreader/ProcessInformation.py` & `petdatasetreader-0.0.2a9/petreader/ProcessInformation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,127 @@
 from petreader.labels import *
 from petreader.TokenClassification import TokenClassification
 from petreader.RelationsExtraction import RelationsExtraction
 import networkx as nx
+import matplotlib.pyplot as plt
+# from pydata.graphs.savegraphs import SaveGraph
+import os
+from collections import defaultdict
 
 BEHAVIORAL = 'b'
+TYPE = 'type'
+LABEL = 'label'
 
+colors = {ACTIVITY: "skyblue",
+          ACTIVITY_DATA: "yellow",
+          ACTOR:    'red',
+          AND_GATEWAY: 'black',
+          XOR_GATEWAY: 'black',
+          CONDITION_SPECIFICATION: 'black',
+
+          FLOW:     'green',
+          SAME_GATEWAY: 'red',
+          USES: "yellow",
+          ACTOR_PERFORMER: 'orange'}
+
+
+def SaveGraph(graph: nx.Graph,
+              outputfolder='./') -> None:
+    """Save a graph into .dot and create .png and .pdf images of the graph
+
+        graph is the nx graph
+        outputfolder is the folder where results are saved
+    """
+    name = graph.name
+    #  save graph in .dot
+    nx.nx_agraph.write_dot(graph,  os.path.join(outputfolder, name) + '.dot')
+
+    node_labels = dict()
+    node_color_map = list()
+    #  node attrs
+    for node in graph.nodes:
+        node_labels[node] = graph.nodes[node]['attrs'][LABEL]
+        node_color_map.append(colors[graph.nodes[node]['attrs'][TYPE]])
+
+    edge_labels = dict()
+    edge_color_map = list()
+    for edge in graph.edges:
+        edge_labels[edge] = graph.edges[edge]['attrs'][TYPE]
+        edge_color_map.append(colors[graph.edges[edge]['attrs'][TYPE]])
+
+
+    pos = nx.nx_agraph.graphviz_layout(graph, prog='dot')
+
+    plt.figure(figsize=(8, 8))
+    # draw labels
+    nx.draw_networkx_nodes(graph,
+                           pos,
+                           node_color=node_color_map,
+                           node_size=500, #23,
+                           alpha=0.35,
+                           )
+    # shifty = 1.50
+    # shiftx = 0  # -70.0
+    # pos_node_labels = {k: (p[0] + shiftx, p[1] + shifty) for k, p in pos.items()}
+    nx.draw_networkx_labels(graph,
+                            pos,  # _node_labels,
+                            labels=node_labels,
+                            horizontalalignment='center',
+                            verticalalignment='center',  # 'bottom',
+                            font_size=11,
+                            font_weight='bold',
+                            font_color='black')
+    nx.draw_networkx_edges(graph,
+                           pos,
+                           edge_color=edge_color_map,
+                           arrows=True,
+                           arrowsize=13,
+                           arrowstyle='->',
+                           )
+    nx.draw_networkx_edge_labels(graph,
+                                 pos,
+                                 edge_labels=edge_labels,
+                                 font_size=8, #10,
+                                 font_color='black')
+
+    ax = plt.gca()
+    ax.margins(0.05)
+    plt.axis("off")
+    plt.tight_layout()
+
+    #   save fig before show it
+    plt.savefig(os.path.join(outputfolder, name) + '.png',
+                format='png', dpi=1000)
+    plt.savefig(os.path.join(outputfolder, name) + '.pdf',
+                format='pdf', dpi=1000)
+
+    # warnings.warn('Show plot mode')
+    plt.show()
+    # plt.close('all')
 
-# TYPE = 'type'
-# LABEL = 'label'
 
 class ProcessInformation:
     def __init__(self):
         self.tc = TokenClassification()
         self.rc = RelationsExtraction()
 
     def GetGateways(self,
                     doc_name: str):
         #  return the list of gateways and condition specification
-        gateway_list = list()
+        gateway_list =list()
         gateway_entities = list()
 
         doc_id = self.rc.GetDocumentNumber(doc_name)
         relations = self.rc.GetRelations(doc_id)[SAME_GATEWAY]
         print('here')
         assert False
 
+
     def GetActivityData(self,
                         doc_name: str):
-
         activity_data = list()
         activity_data_entities = list()
         doc_id = self.rc.GetDocumentNumber(doc_name)
         relations = self.rc.GetRelations(doc_id)[USES]
 
         for use_rel in relations:
             activity_node = (use_rel[SOURCE_SENTENCE_ID], use_rel[SOURCE_HEAD_TOKEN_ID])
@@ -41,15 +131,14 @@
 
             activity_data.append((activity_node, ad_node))
             activity_data_entities.append((activity_label, ad_label))
         return activity_data, activity_data_entities
 
     def GetPerformsActors(self,
                           doc_name: str):
-
         performs = list()
         performs_entities = list()
         doc_id = self.rc.GetDocumentNumber(doc_name)
         activities = self.tc.GetActivities(doc_name)
         relations = self.rc.GetRelations(doc_id)[ACTOR_PERFORMER]
 
         for performs_rel in relations:
@@ -58,14 +147,15 @@
             actor_node = (performs_rel[TARGET_SENTENCE_ID], performs_rel[TARGET_HEAD_TOKEN_ID])
             actor_label = ' '.join(performs_rel[TARGET_ENTITY])
 
             performs.append((activity_node, actor_node))
             performs_entities.append((activity_label, actor_label))
         return performs, performs_entities
 
+
     def GetKnowledgeGraph(self,
                           doc_name,
                           outputdir='./'):
         actors = self.GetKG_DFGPerformsActors(doc_name)
         act_data = self.GetKG_DFGActivityData(doc_name)
 
         combined = nx.DiGraph()
@@ -74,26 +164,26 @@
         combined.add_edges_from(act_data.edges(data=True))
         combined.add_nodes_from(actors.nodes(data=True))
         combined.add_nodes_from(act_data.nodes(data=True))  # deals with isolated nodes
 
         return combined
 
     def GetKG_DFGActivityData(self,
-                              doc_name: str,
-                              outputdir='./'):
+                                doc_name: str,
+                                outputdir='./'):
         #  return a a graph
         graph = self.GetDFG(doc_name, outputdir=outputdir)
 
         doc_id = self.rc.GetDocumentNumber(doc_name)
         # activities = self.tc.GetActivities(doc_name)
         relations = self.rc.GetRelations(doc_id)[USES]
 
         for use_rel in relations:
             activity_node = (use_rel[SOURCE_SENTENCE_ID], use_rel[SOURCE_HEAD_TOKEN_ID])
-            ad_node = (use_rel[TARGET_SENTENCE_ID], use_rel[TARGET_HEAD_TOKEN_ID])
+            ad_node =  (use_rel[TARGET_SENTENCE_ID], use_rel[TARGET_HEAD_TOKEN_ID])
             graph.add_node(ad_node, attrs={TYPE: ACTIVITY_DATA, LABEL: ' '.join(use_rel[TARGET_ENTITY])})
 
             graph.add_edge(activity_node, ad_node, attrs={TYPE: USES, LABEL: USES})
 
         return graph
 
     def GetKG_DFGPerformsActors(self,
@@ -104,27 +194,29 @@
 
         doc_id = self.rc.GetDocumentNumber(doc_name)
         # activities = self.tc.GetActivities(doc_name)
         relations = self.rc.GetRelations(doc_id)[ACTOR_PERFORMER]
 
         for performs_rel in relations:
             activity_node = (performs_rel[SOURCE_SENTENCE_ID], performs_rel[SOURCE_HEAD_TOKEN_ID])
-            actor_node = (performs_rel[TARGET_SENTENCE_ID], performs_rel[TARGET_HEAD_TOKEN_ID])
+            actor_node =  (performs_rel[TARGET_SENTENCE_ID], performs_rel[TARGET_HEAD_TOKEN_ID])
             graph.add_node(actor_node, attrs={TYPE: ACTOR, LABEL: ' '.join(performs_rel[TARGET_ENTITY])})
 
             graph.add_edge(activity_node, actor_node, attrs={TYPE: ACTOR_PERFORMER, LABEL: ACTOR_PERFORMER})
 
         return graph
 
+
     def GetRawActivityLabels(self,
                              doc_name: str):
         #  store activity information (sentence, head word index, text)
         # activity_info = list()
         activity_info2 = dict()
 
+
         doc_id = self.rc.GetDocumentNumber(doc_name)
         # token classification sentence indexes
         tc_indexes = self.tc.get_n_sample_of_a_document(doc_name)
         process_description = self.tc.GetDocumentText(doc_name)
         #  get activities from TC
         activities = self.tc.GetActivities(doc_name)
         activities_indexes = self.tc.GetActivities(doc_name, True)
@@ -137,16 +229,16 @@
                 #                       TEXT: [self.tc.GetTokens(tc_indexes[n_sent])],
                 #                       RAW_LABEL: [act_],
                 #                       ACTIVITY_DATA: list(),
                 #                       FURTHER_SPECIFICATION: list()})
 
                 key = (n_sent, act_head[0])
                 activity_info2[key] = {PROCESS_DESCRIPTION: process_description,
-                                       TEXT:                ' '.join(self.tc.GetTokens(tc_indexes[n_sent])),
-                                       RAW_LABEL:           [act_], }
+                                       TEXT: ' '.join(self.tc.GetTokens(tc_indexes[n_sent])),
+                                       RAW_LABEL: [act_],}
         #  get activities from RC
         # Get Activity + Activity Data for each activity in texts
         r = self.rc.GetRelations(doc_id)
 
         #  uses relation
         uses = r[USES]
         for use_rel in uses:
@@ -177,21 +269,22 @@
         # print()
         return activity_info2
 
     def GetDFG(self,
                doc_name: str,
                outputdir='./'):
         graph = self.construct_behavioral_graph(doc_name)
-        # SaveGraph(graph, outputfolder=outputdir)
+        SaveGraph(graph, outputfolder=outputdir)
 
         graph = self.construct_dfg(graph)
-        # SaveGraph(graph, outputfolder=outputdir)
+        SaveGraph(graph, outputfolder=outputdir)
 
         return graph
 
+
     def construct_behavioral_graph(self, doc_name):
         #  returns:
         #       a nx graph representing behavioral elements (ACTIVITY, GATEWAY, CONDITION SPECIFICATION)
         #       a dict(node code)= {type: Act/Gate/CondSpec, label: str}
         #       a dict(edge) = edge type: str
 
         graph = nx.DiGraph()
@@ -240,19 +333,17 @@
         [graph.remove_node(n) for n in nodes_to_be_removed]
 
         return graph
 
 
 if __name__ == '__main__':
     from pprint import pprint
-    from petreader.utility import ShowGraph
-
     pi = ProcessInformation()
     doc_name = 'doc-1.3'
-    ShowGraph(pi.GetKnowledgeGraph(doc_name))
+    SaveGraph(pi.GetKnowledgeGraph(doc_name))
     print()
     # SaveGraph(pi.GetKG_DFGActivityData(doc_name))
     # pprint(pi.GetActivityData(doc_name))
     # pprint(pi.GetRawActivityLabels(doc_name))
     # print()
     # pi.GetDFG(doc_name)
     # print()
```

### Comparing `petdatasetreader-0.0.2a10/petreader/RelationsExtraction.py` & `petdatasetreader-0.0.2a9/petreader/RelationsExtraction.py`

 * *Files identical despite different names*

### Comparing `petdatasetreader-0.0.2a10/petreader/TokenClassification.py` & `petdatasetreader-0.0.2a9/petreader/TokenClassification.py`

 * *Files identical despite different names*

### Comparing `petdatasetreader-0.0.2a10/petreader/labels.py` & `petdatasetreader-0.0.2a9/petreader/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-#  Attributes
-TYPE = 'type'
-LABEL = 'label'
-
 #  Process Information
 TEXT = 'text'
 PROCESS_DESCRIPTION = 'process-description'
 RAW_LABEL = 'raw-label'
 
 #  Matching strategy
 WORD_BASED_STRATEGY = 'word-based'
```

### Comparing `petdatasetreader-0.0.2a10/petreader/petdataset.py` & `petdatasetreader-0.0.2a9/petreader/petdataset.py`

 * *Files identical despite different names*

### Comparing `petdatasetreader-0.0.2a10/setup.py` & `petdatasetreader-0.0.2a9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 _REQUIRED = ['datasets']
 _EXTRAS = []
 
 setup(
     name='petdatasetreader',
-    version='0.0.2a10',
+    version='0.0.2a9',
     packages=find_packages(exclude=("tests", "docs", "dist", "build")),
     install_requires=_REQUIRED,
     # extras_require=_EXTRAS,
     include_package_data=False,
     platforms="Any",
 
     python_requires='!=2.7, >=3.5.*',
```

