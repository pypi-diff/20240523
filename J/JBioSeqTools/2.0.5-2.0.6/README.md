# Comparing `tmp/JBioSeqTools-2.0.5.tar.gz` & `tmp/JBioSeqTools-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBioSeqTools-2.0.5.tar", last modified: Wed May 22 22:02:40 2024, max compression
+gzip compressed data, was "JBioSeqTools-2.0.6.tar", last modified: Thu May 23 08:44:54 2024, max compression
```

## Comparing `JBioSeqTools-2.0.5.tar` & `JBioSeqTools-2.0.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 22:02:40.352687 JBioSeqTools-2.0.5/
-drwxrwxrwx   0        0        0        0 2024-05-22 22:02:40.283285 JBioSeqTools-2.0.5/JBioSeqTools.egg-info/
--rw-rw-rw-   0        0        0     1027 2024-05-22 22:02:37.000000 JBioSeqTools-2.0.5/JBioSeqTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      733 2024-05-22 22:02:39.000000 JBioSeqTools-2.0.5/JBioSeqTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 22:02:38.000000 JBioSeqTools-2.0.5/JBioSeqTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2024-05-22 22:02:39.000000 JBioSeqTools-2.0.5/JBioSeqTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 22:02:39.000000 JBioSeqTools-2.0.5/JBioSeqTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-2.0.5/LICENSE
--rw-rw-rw-   0        0        0       93 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1027 2024-05-22 22:02:40.352178 JBioSeqTools-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0   136379 2024-03-08 13:18:31.000000 JBioSeqTools-2.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 22:02:40.291374 JBioSeqTools-2.0.5/jbst/
--rw-rw-rw-   0        0        0     1489 2024-05-22 22:00:34.000000 JBioSeqTools-2.0.5/jbst/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:02:40.339281 JBioSeqTools-2.0.5/jbst/data/
--rw-rw-rw-   0        0        0    11970 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/backbone.xlsx
--rw-rw-rw-   0        0        0    18801 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/codons.xlsx
--rw-rw-rw-   0        0        0    24612 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/enzymes.xlsx
--rw-rw-rw-   0        0        0    10901 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/fluorescent_tag.xlsx
--rw-rw-rw-   0        0        0     9685 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/linkers.xlsx
--rw-rw-rw-   0        0        0    11897 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/polya.xlsx
--rw-rw-rw-   0        0        0    65342 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/promoters.xlsx
--rw-rw-rw-   0        0        0    11212 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/regulators.xlsx
--rw-rw-rw-   0        0        0   228812 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/restriction_enzymes.xlsx
--rw-rw-rw-   0        0        0     8571 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/rnai_scoring.xlsx
--rw-rw-rw-   0        0        0    11916 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/selectors.xlsx
--rw-rw-rw-   0        0        0    12038 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/sh_loops.xlsx
--rw-rw-rw-   0        0        0    10119 2024-05-22 12:14:29.000000 JBioSeqTools-2.0.5/jbst/data/vector_capacity.xlsx
--rw-rw-rw-   0        0        0    16543 2024-05-22 12:14:07.000000 JBioSeqTools-2.0.5/jbst/data/vectors.xlsx
--rw-rw-rw-   0        0        0    14686 2024-05-22 22:01:35.000000 JBioSeqTools-2.0.5/jbst/install.py
--rw-rw-rw-   0        0        0    99588 2024-05-22 10:14:39.000000 JBioSeqTools-2.0.5/jbst/seq_tools.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:02:40.347590 JBioSeqTools-2.0.5/jbst/tests/
--rw-rw-rw-   0        0        0        2 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/tests/__init__.py
--rw-rw-rw-   0        0        0    10100 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/tests/fasta_vector_test.fasta
--rw-rw-rw-   0        0        0   770959 2024-05-22 21:27:37.000000 JBioSeqTools-2.0.5/jbst/tests/jseq_tests.py
--rw-rw-rw-   0        0        0   126569 2024-05-22 10:16:21.000000 JBioSeqTools-2.0.5/jbst/vector_build.py
--rw-rw-rw-   0        0        0       42 2024-05-22 22:02:40.352687 JBioSeqTools-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1600 2024-05-22 22:00:48.000000 JBioSeqTools-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 08:44:54.386712 JBioSeqTools-2.0.6/
+drwxrwxrwx   0        0        0        0 2024-05-23 08:44:54.321811 JBioSeqTools-2.0.6/JBioSeqTools.egg-info/
+-rw-rw-rw-   0        0        0     1027 2024-05-23 08:44:52.000000 JBioSeqTools-2.0.6/JBioSeqTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      733 2024-05-23 08:44:53.000000 JBioSeqTools-2.0.6/JBioSeqTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 08:44:52.000000 JBioSeqTools-2.0.6/JBioSeqTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2024-05-23 08:44:52.000000 JBioSeqTools-2.0.6/JBioSeqTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-23 08:44:53.000000 JBioSeqTools-2.0.6/JBioSeqTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-2.0.6/LICENSE
+-rw-rw-rw-   0        0        0       93 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1027 2024-05-23 08:44:54.386712 JBioSeqTools-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0   136379 2024-03-08 13:18:31.000000 JBioSeqTools-2.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 08:44:54.331920 JBioSeqTools-2.0.6/jbst/
+-rw-rw-rw-   0        0        0     1489 2024-05-23 08:44:07.000000 JBioSeqTools-2.0.6/jbst/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 08:44:54.373246 JBioSeqTools-2.0.6/jbst/data/
+-rw-rw-rw-   0        0        0    11970 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/backbone.xlsx
+-rw-rw-rw-   0        0        0    18801 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/codons.xlsx
+-rw-rw-rw-   0        0        0    24612 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/enzymes.xlsx
+-rw-rw-rw-   0        0        0    10901 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/fluorescent_tag.xlsx
+-rw-rw-rw-   0        0        0     9685 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/linkers.xlsx
+-rw-rw-rw-   0        0        0    11897 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/polya.xlsx
+-rw-rw-rw-   0        0        0    65342 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/promoters.xlsx
+-rw-rw-rw-   0        0        0    11212 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/regulators.xlsx
+-rw-rw-rw-   0        0        0   228812 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/restriction_enzymes.xlsx
+-rw-rw-rw-   0        0        0     8571 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/rnai_scoring.xlsx
+-rw-rw-rw-   0        0        0    11916 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/selectors.xlsx
+-rw-rw-rw-   0        0        0    12038 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/sh_loops.xlsx
+-rw-rw-rw-   0        0        0    10119 2024-05-22 12:14:29.000000 JBioSeqTools-2.0.6/jbst/data/vector_capacity.xlsx
+-rw-rw-rw-   0        0        0    16543 2024-05-22 12:14:07.000000 JBioSeqTools-2.0.6/jbst/data/vectors.xlsx
+-rw-rw-rw-   0        0        0    14686 2024-05-22 22:01:35.000000 JBioSeqTools-2.0.6/jbst/install.py
+-rw-rw-rw-   0        0        0    99326 2024-05-23 08:39:50.000000 JBioSeqTools-2.0.6/jbst/seq_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-23 08:44:54.380195 JBioSeqTools-2.0.6/jbst/tests/
+-rw-rw-rw-   0        0        0        2 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/tests/__init__.py
+-rw-rw-rw-   0        0        0    10100 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/tests/fasta_vector_test.fasta
+-rw-rw-rw-   0        0        0   770959 2024-05-22 21:27:37.000000 JBioSeqTools-2.0.6/jbst/tests/jseq_tests.py
+-rw-rw-rw-   0        0        0   126514 2024-05-23 08:40:47.000000 JBioSeqTools-2.0.6/jbst/vector_build.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 08:44:54.386712 JBioSeqTools-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2024-05-23 08:43:45.000000 JBioSeqTools-2.0.6/setup.py
```

### Comparing `JBioSeqTools-2.0.5/JBioSeqTools.egg-info/PKG-INFO` & `JBioSeqTools-2.0.6/JBioSeqTools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 2.0.5
+Version: 2.0.6
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-2.0.5/JBioSeqTools.egg-info/SOURCES.txt` & `JBioSeqTools-2.0.6/JBioSeqTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/LICENSE` & `JBioSeqTools-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/PKG-INFO` & `JBioSeqTools-2.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 2.0.5
+Version: 2.0.6
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-2.0.5/README.md` & `JBioSeqTools-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/__init__.py` & `JBioSeqTools-2.0.6/jbst/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                                     __/ |                                   
                                    |___/                                   
 """
 
 print(pattern)
 
 print('')
-print('Welcome in JBioSeqTools v.2.0.5 library')
+print('Welcome in JBioSeqTools v.2.0.6 library')
 print('')
 print('Loading required packages...')
 
 
 
 
 import os
```

### Comparing `JBioSeqTools-2.0.5/jbst/data/backbone.xlsx` & `JBioSeqTools-2.0.6/jbst/data/backbone.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/codons.xlsx` & `JBioSeqTools-2.0.6/jbst/data/codons.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/enzymes.xlsx` & `JBioSeqTools-2.0.6/jbst/data/enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/fluorescent_tag.xlsx` & `JBioSeqTools-2.0.6/jbst/data/fluorescent_tag.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/linkers.xlsx` & `JBioSeqTools-2.0.6/jbst/data/linkers.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/polya.xlsx` & `JBioSeqTools-2.0.6/jbst/data/polya.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/promoters.xlsx` & `JBioSeqTools-2.0.6/jbst/data/promoters.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/regulators.xlsx` & `JBioSeqTools-2.0.6/jbst/data/regulators.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/restriction_enzymes.xlsx` & `JBioSeqTools-2.0.6/jbst/data/restriction_enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/rnai_scoring.xlsx` & `JBioSeqTools-2.0.6/jbst/data/rnai_scoring.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/selectors.xlsx` & `JBioSeqTools-2.0.6/jbst/data/selectors.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/sh_loops.xlsx` & `JBioSeqTools-2.0.6/jbst/data/sh_loops.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/vector_capacity.xlsx` & `JBioSeqTools-2.0.6/jbst/data/vector_capacity.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/data/vectors.xlsx` & `JBioSeqTools-2.0.6/jbst/data/vectors.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/install.py` & `JBioSeqTools-2.0.6/jbst/install.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/seq_tools.py` & `JBioSeqTools-2.0.6/jbst/seq_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -729,15 +729,15 @@
                     
         con_tmp = ""
         consesnuses = []
         for j, i in enumerate(seq_list[0]):
             nuc = []
             for c in range(len(seq_list)):
                 nuc.append(seq_list[c][j])
-                #poprawić na fascie bo popsulem
+                
             if len(set(nuc)) == 1 and '-' not in nuc and j != len(seq_list[0]) - 1:
                 con_tmp = con_tmp + str(seq_list[c][j]) 
             else:
                 if len(con_tmp) > 30:
                      consesnuses.append(con_tmp)
                      con_tmp = ""
                 else:
@@ -2161,14 +2161,18 @@
         print('\nLack of restriction places to choose')
         
     return np.asarray(enzyme_list)       
 
 
 
 
+sequence = project['transcripts']['sequences']['vector_sequence'][trans]
+restriction_df = project['transcripts']['sequences']['full_restriction'][trans]
+enzyme_list = project['transcripts']['sequences']['enzymes'][trans] 
+
 
 def repair_sequences(sequence, metadata, restriction_df, enzyme_list, species):
     
     if species.lower() in ['both', 'both2', 'multi']:
         species = 'human'
         
     codons = metadata['codons']
@@ -2262,44 +2266,37 @@
                 
             print('\nwere unable to optimize:')
             print('\nRest of chosen restriction places in the sequence has repaired...')
     
             
         print('\nChecking the new restriction places...')
         
-        enzyme_restriction = check_restriction(final_sequence, metadata)
+        enzyme_restriction, restriction_df2  = check_restriction(final_sequence, metadata)
                                    
         enzyme_restriction = pd.DataFrame.from_dict(enzyme_restriction)
         enzyme_restriction = enzyme_restriction.drop_duplicates()
         enzyme_restriction = enzyme_restriction.reset_index(drop=True)
         enzyme_restriction = enzyme_restriction[~enzyme_restriction['name'].isin(restriction_df['name'])]
         
-        if len(enzyme_restriction['name']) > 0:
-            restriction_df = enzyme_restriction.copy()
-            restriction_df['index'] = restriction_df.index
-            restriction_df = restriction_df[['name', 'index']]
-            restriction_df['index'] = [[x] for x in restriction_df['index']]
-            restriction_df = restriction_df.groupby('name').agg({'index': 'sum'})
-            restriction_df = restriction_df.reset_index()
-    
-        elif len(enzyme_restriction['name']) == 0:
-            restriction_df = enzyme_restriction
+        
+        if len(enzyme_restriction['name']) == 0:
             print('\nAny new restriction places were not created')
         else:
             print('\nNew restriction places were created:')
             for name in enzyme_restriction['name']:
                 print(name)
     
+    
     else:
         enzyme_restriction = {'name':[], 'restriction_place':[], 'restriction_sequence':[], 'start':[], 'stop':[]}
         enzyme_restriction = pd.DataFrame.from_dict(enzyme_restriction)
         not_repaired = []
         final_sequence = sequence
 
-    return final_sequence, not_repaired, enzyme_restriction, restriction_df
+    return final_sequence, not_repaired, enzyme_restriction, pd.DataFrame(restriction_df2)
 
 
 
 def sequence_restriction_removal(sequence:str, metadata, restriction_places:list = [], species:str = 'human'):
     
     """
     This function finds and removes restriction places inside the sequence.
```

### Comparing `JBioSeqTools-2.0.5/jbst/tests/fasta_vector_test.fasta` & `JBioSeqTools-2.0.6/jbst/tests/fasta_vector_test.fasta`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/tests/jseq_tests.py` & `JBioSeqTools-2.0.6/jbst/tests/jseq_tests.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.5/jbst/vector_build.py` & `JBioSeqTools-2.0.6/jbst/vector_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,14 +422,15 @@
 
 
 def repair_restriction_vector(project, metadata, species):
     codons = metadata['codons']
     project['transcripts']['sequences']['not_repaired'] = []
     if len(project['transcripts']['sequences']['enzymes']) != 0:
         for trans in range(0,len(project['transcripts']['sequences']['name'])):
+            break
             final_sequence, not_repaired, enzyme_restriction, restriction_df =  repair_sequences(project['transcripts']['sequences']['vector_sequence'][trans], metadata, project['transcripts']['sequences']['full_restriction'][trans], project['transcripts']['sequences']['enzymes'][trans] , species)
             project['transcripts']['sequences']['vector_sequence'][trans] = final_sequence
             project['transcripts']['sequences']['not_repaired'].append(not_repaired)
             project['transcripts']['sequences']['full_restriction'][trans] = enzyme_restriction.to_dict()
             project['transcripts']['sequences']['enzymes_df'][trans] =  restriction_df.to_dict()
             
     
@@ -1176,15 +1177,14 @@
     
                 
                 #restriction
                 project['elements']['vector']['selection_marker'] = input_dict['selection_marker_sequence']
                 project['elements']['vector']['selection_marker_name'] = input_dict['selection_marker_name']
                 
                 
-                #poprawic stop check
                 promoter_dec = 'single'
         
                     
                 project = check_stop(project, metadata['codons'], promoter_dec)
                          
                 
                 run1 = input_dict['optimize']
@@ -1705,15 +1705,15 @@
                                 en = list(tmp['index'][tmp['name'].isin(user_defined_enzymes)])
                                 list_tmp = [item for sublist in en for item in sublist]
                                 list_of_list.append(list_tmp)
                             else:
                                 list_of_list.append([])
                 
                         project = add_chosen_restriction(project, list_of_list)
-                        # project = repair_restriction_vector(project, metadata, input_dict['species'])
+                        project = repair_restriction_vector(project, metadata, input_dict['species'])
                         
                     
                 project = vector_string(project, metadata['backbone'], input_dict['vector_type'], input_dict['vector_function'], promoter_dec)
                 project = eval_vector(project, metadata['vectors'], input_dict['vector_type'], input_dict['vector_function'])
             
                 project, pl = vector_plot_project(project, metadata, show_plot = show_plot),
                 
@@ -2098,15 +2098,14 @@
                 project['elements']['fluorescence']['polya_seq_name'] = ''
                 project['elements']['fluorescence']['promoter_name'] = ''
                 project['elements']['fluorescence']['promoter_seq'] = ''
            
     
         
             
-            #poprawic stop check
             if len(project['elements']['fluorescence']['sequence']) > 0 and len(project['elements']['fluorescence']['polya_seq']) > 0 and len(project['elements']['fluorescence']['promoter_seq']) > 0:
                 promoter_dec = 'multi'
             else:
                 promoter_dec = 'single'
                 
                 
             if len(project['transcripts']['sequences']['sequence']) > 0:
```

### Comparing `JBioSeqTools-2.0.5/setup.py` & `JBioSeqTools-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.0.5' 
+VERSION = '2.0.6' 
 DESCRIPTION = 'JBioSeqTools'
 LONG_DESCRIPTION = 'JBioSeqTools is the Python library for biological sequence optimization (GC % content & codon frequency), restriction places removal, DNA/RNA structure prediction, and RNAi selection. It also allows the building of many plasmid vectors with the possibility of choosing sequences such as transcript, promoter, enhancer, molecular fluorescent tag, etc. Finally, the user obtains a ready-for-order construct with a whole sequence and visualization. Package description  on https://github.com/jkubis96/JBioSeqTools'
 
 # Setting up
 setup(
         name="JBioSeqTools", 
         version=VERSION,
```

