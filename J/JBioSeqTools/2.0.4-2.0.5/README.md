# Comparing `tmp/JBioSeqTools-2.0.4.tar.gz` & `tmp/JBioSeqTools-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBioSeqTools-2.0.4.tar", last modified: Wed May 22 12:48:14 2024, max compression
+gzip compressed data, was "JBioSeqTools-2.0.5.tar", last modified: Wed May 22 22:02:40 2024, max compression
```

## Comparing `JBioSeqTools-2.0.4.tar` & `JBioSeqTools-2.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 12:48:14.579867 JBioSeqTools-2.0.4/
-drwxrwxrwx   0        0        0        0 2024-05-22 12:48:14.544746 JBioSeqTools-2.0.4/JBioSeqTools.egg-info/
--rw-rw-rw-   0        0        0     1027 2024-05-22 12:48:13.000000 JBioSeqTools-2.0.4/JBioSeqTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      733 2024-05-22 12:48:14.000000 JBioSeqTools-2.0.4/JBioSeqTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 12:48:13.000000 JBioSeqTools-2.0.4/JBioSeqTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2024-05-22 12:48:14.000000 JBioSeqTools-2.0.4/JBioSeqTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 12:48:14.000000 JBioSeqTools-2.0.4/JBioSeqTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-2.0.4/LICENSE
--rw-rw-rw-   0        0        0       93 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1027 2024-05-22 12:48:14.579867 JBioSeqTools-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0   136379 2024-03-08 13:18:31.000000 JBioSeqTools-2.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 12:48:14.550181 JBioSeqTools-2.0.4/jbst/
--rw-rw-rw-   0        0        0     1489 2024-05-22 12:46:26.000000 JBioSeqTools-2.0.4/jbst/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 12:48:14.571658 JBioSeqTools-2.0.4/jbst/data/
--rw-rw-rw-   0        0        0    11970 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/backbone.xlsx
--rw-rw-rw-   0        0        0    18801 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/codons.xlsx
--rw-rw-rw-   0        0        0    24612 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/enzymes.xlsx
--rw-rw-rw-   0        0        0    10901 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/fluorescent_tag.xlsx
--rw-rw-rw-   0        0        0     9685 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/linkers.xlsx
--rw-rw-rw-   0        0        0    11897 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/polya.xlsx
--rw-rw-rw-   0        0        0    65342 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/promoters.xlsx
--rw-rw-rw-   0        0        0    11212 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/regulators.xlsx
--rw-rw-rw-   0        0        0   228812 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/restriction_enzymes.xlsx
--rw-rw-rw-   0        0        0     8571 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/rnai_scoring.xlsx
--rw-rw-rw-   0        0        0    11916 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/selectors.xlsx
--rw-rw-rw-   0        0        0    12038 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/sh_loops.xlsx
--rw-rw-rw-   0        0        0    10119 2024-05-22 12:14:29.000000 JBioSeqTools-2.0.4/jbst/data/vector_capacity.xlsx
--rw-rw-rw-   0        0        0    16543 2024-05-22 12:14:07.000000 JBioSeqTools-2.0.4/jbst/data/vectors.xlsx
--rw-rw-rw-   0        0        0    15427 2024-05-22 12:45:35.000000 JBioSeqTools-2.0.4/jbst/install.py
--rw-rw-rw-   0        0        0    99588 2024-05-22 10:14:39.000000 JBioSeqTools-2.0.4/jbst/seq_tools.py
-drwxrwxrwx   0        0        0        0 2024-05-22 12:48:14.576856 JBioSeqTools-2.0.4/jbst/tests/
--rw-rw-rw-   0        0        0        2 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/tests/__init__.py
--rw-rw-rw-   0        0        0    10100 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/tests/fasta_vector_test.fasta
--rw-rw-rw-   0        0        0   770959 2024-05-22 11:09:36.000000 JBioSeqTools-2.0.4/jbst/tests/jseq_tests.py
--rw-rw-rw-   0        0        0   126569 2024-05-22 10:16:21.000000 JBioSeqTools-2.0.4/jbst/vector_build.py
--rw-rw-rw-   0        0        0       42 2024-05-22 12:48:14.579867 JBioSeqTools-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1600 2024-05-22 12:46:08.000000 JBioSeqTools-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:02:40.352687 JBioSeqTools-2.0.5/
+drwxrwxrwx   0        0        0        0 2024-05-22 22:02:40.283285 JBioSeqTools-2.0.5/JBioSeqTools.egg-info/
+-rw-rw-rw-   0        0        0     1027 2024-05-22 22:02:37.000000 JBioSeqTools-2.0.5/JBioSeqTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      733 2024-05-22 22:02:39.000000 JBioSeqTools-2.0.5/JBioSeqTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 22:02:38.000000 JBioSeqTools-2.0.5/JBioSeqTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2024-05-22 22:02:39.000000 JBioSeqTools-2.0.5/JBioSeqTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 22:02:39.000000 JBioSeqTools-2.0.5/JBioSeqTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0       93 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1027 2024-05-22 22:02:40.352178 JBioSeqTools-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0   136379 2024-03-08 13:18:31.000000 JBioSeqTools-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 22:02:40.291374 JBioSeqTools-2.0.5/jbst/
+-rw-rw-rw-   0        0        0     1489 2024-05-22 22:00:34.000000 JBioSeqTools-2.0.5/jbst/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:02:40.339281 JBioSeqTools-2.0.5/jbst/data/
+-rw-rw-rw-   0        0        0    11970 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/backbone.xlsx
+-rw-rw-rw-   0        0        0    18801 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/codons.xlsx
+-rw-rw-rw-   0        0        0    24612 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/enzymes.xlsx
+-rw-rw-rw-   0        0        0    10901 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/fluorescent_tag.xlsx
+-rw-rw-rw-   0        0        0     9685 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/linkers.xlsx
+-rw-rw-rw-   0        0        0    11897 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/polya.xlsx
+-rw-rw-rw-   0        0        0    65342 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/promoters.xlsx
+-rw-rw-rw-   0        0        0    11212 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/regulators.xlsx
+-rw-rw-rw-   0        0        0   228812 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/restriction_enzymes.xlsx
+-rw-rw-rw-   0        0        0     8571 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/rnai_scoring.xlsx
+-rw-rw-rw-   0        0        0    11916 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/selectors.xlsx
+-rw-rw-rw-   0        0        0    12038 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/data/sh_loops.xlsx
+-rw-rw-rw-   0        0        0    10119 2024-05-22 12:14:29.000000 JBioSeqTools-2.0.5/jbst/data/vector_capacity.xlsx
+-rw-rw-rw-   0        0        0    16543 2024-05-22 12:14:07.000000 JBioSeqTools-2.0.5/jbst/data/vectors.xlsx
+-rw-rw-rw-   0        0        0    14686 2024-05-22 22:01:35.000000 JBioSeqTools-2.0.5/jbst/install.py
+-rw-rw-rw-   0        0        0    99588 2024-05-22 10:14:39.000000 JBioSeqTools-2.0.5/jbst/seq_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:02:40.347590 JBioSeqTools-2.0.5/jbst/tests/
+-rw-rw-rw-   0        0        0        2 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/tests/__init__.py
+-rw-rw-rw-   0        0        0    10100 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.5/jbst/tests/fasta_vector_test.fasta
+-rw-rw-rw-   0        0        0   770959 2024-05-22 21:27:37.000000 JBioSeqTools-2.0.5/jbst/tests/jseq_tests.py
+-rw-rw-rw-   0        0        0   126569 2024-05-22 10:16:21.000000 JBioSeqTools-2.0.5/jbst/vector_build.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 22:02:40.352687 JBioSeqTools-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2024-05-22 22:00:48.000000 JBioSeqTools-2.0.5/setup.py
```

### Comparing `JBioSeqTools-2.0.4/JBioSeqTools.egg-info/PKG-INFO` & `JBioSeqTools-2.0.5/JBioSeqTools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 2.0.4
+Version: 2.0.5
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-2.0.4/JBioSeqTools.egg-info/SOURCES.txt` & `JBioSeqTools-2.0.5/JBioSeqTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/LICENSE` & `JBioSeqTools-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/PKG-INFO` & `JBioSeqTools-2.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 2.0.4
+Version: 2.0.5
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-2.0.4/README.md` & `JBioSeqTools-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/__init__.py` & `JBioSeqTools-2.0.5/jbst/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                                     __/ |                                   
                                    |___/                                   
 """
 
 print(pattern)
 
 print('')
-print('Welcome in JBioSeqTools v.2.0.4 library')
+print('Welcome in JBioSeqTools v.2.0.5 library')
 print('')
 print('Loading required packages...')
 
 
 
 
 import os
```

### Comparing `JBioSeqTools-2.0.4/jbst/data/backbone.xlsx` & `JBioSeqTools-2.0.5/jbst/data/backbone.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/codons.xlsx` & `JBioSeqTools-2.0.5/jbst/data/codons.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/enzymes.xlsx` & `JBioSeqTools-2.0.5/jbst/data/enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/fluorescent_tag.xlsx` & `JBioSeqTools-2.0.5/jbst/data/fluorescent_tag.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/linkers.xlsx` & `JBioSeqTools-2.0.5/jbst/data/linkers.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/polya.xlsx` & `JBioSeqTools-2.0.5/jbst/data/polya.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/promoters.xlsx` & `JBioSeqTools-2.0.5/jbst/data/promoters.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/regulators.xlsx` & `JBioSeqTools-2.0.5/jbst/data/regulators.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/restriction_enzymes.xlsx` & `JBioSeqTools-2.0.5/jbst/data/restriction_enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/rnai_scoring.xlsx` & `JBioSeqTools-2.0.5/jbst/data/rnai_scoring.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/selectors.xlsx` & `JBioSeqTools-2.0.5/jbst/data/selectors.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/sh_loops.xlsx` & `JBioSeqTools-2.0.5/jbst/data/sh_loops.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/vector_capacity.xlsx` & `JBioSeqTools-2.0.5/jbst/data/vector_capacity.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/data/vectors.xlsx` & `JBioSeqTools-2.0.5/jbst/data/vectors.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/install.py` & `JBioSeqTools-2.0.5/jbst/install.py`

 * *Files 10% similar despite different names*

```diff
@@ -408,15 +408,15 @@
 
         # Clean up: remove the downloaded archive file
         os.remove(blast)
  
         
  
 
-def download_refseq_db(path_to_save = None, db = 'refseq_select_rna'):    
+def download_refseq_db(path_to_save = None):    
 
     if path_to_save == None:
         path_to_save = os.getcwd() 
         
     
     system = platform.system()
     
@@ -426,58 +426,37 @@
         path_to_save = os.path.join(path_to_save, 'blast/windows/ncbi-blast-2.14.1+/bin')
     
     
     elif system == "Linux":
         print("\nLinux operating system")        
         path_to_save = os.path.join(path_to_save, 'blast/linux/ncbi-blast-2.14.1+/bin')
 
+    file = 'refseq_select_rna.tar.gz'
+
+    local_file_path = os.path.join(path_to_save, file)
     
     
-    # Define the FTP URL and directory
-    ftp_url = "ftp.ncbi.nlm.nih.gov"
-    ftp_directory = "/blast/db/"
-    
-    # Connect to the FTP server
-    ftp = FTP(ftp_url)
-    ftp.login()
-    
-    # Change to the directory containing RefSeq RNA databases
-    ftp.cwd(ftp_directory)
-    
-    # List the available files in the directory
-    file_list = ftp.nlst()
-    
-    # Define the name of the RefSeq RNA database you want to download    
-    
-    file_list = [x for x in file_list if db in x and x.endswith('tar.gz') and not x.endswith('md5')]
-    
-    for file in tqdm(file_list):
-        local_file_path = os.path.join(path_to_save, file)
-    
-        # Download the database file
-        with open(local_file_path, 'wb') as local_file:
-            ftp.retrbinary('RETR ' + file, local_file.write)
-            
-        with tarfile.open(local_file_path, 'r:gz') as tar:
-            tar.extractall(path=path_to_save)
-            
+    ref_seq = 'https://drive.google.com/uc?id=1e6Gi1OWlvFPeVOCEGaoZ85Fi470MXy0z'
 
-        
-        try:
-            os.remove(local_file_path)
-            print(f'{local_file_path} successfully deleted.')
-        except OSError as e:
-            print(f'Error: {local_file_path} - {e.strerror}')
+    gdown.download(ref_seq, local_file_path, quiet=False)
+
+
+
+    with tarfile.open(local_file_path, 'r:gz') as tar:
+        tar.extractall(path=path_to_save)
+
+    
+    try:
+        os.remove(local_file_path)
+        print(f'{local_file_path} successfully deleted.')
+    except OSError as e:
+        print(f'Error: {local_file_path} - {e.strerror}')
         
             
-        
-        print(f"\n{db} has been downloaded to {local_file_path}")
-    
-    # Close the FTP connection
-    ftp.quit()
+    print(f"\nThe refseq_select_rna has been downloaded to {local_file_path}")
     
   
     
   
     
 #full instalation
 
@@ -494,15 +473,15 @@
        
     """
 
     try:
         create_temporary_directory(source = source)
         install_muscle(source = source)
         install_blast(source = source)
-        download_refseq_db(path_to_save = source, db = 'refseq_select_rna')
+        download_refseq_db(path_to_save = source)
         
         utr5, utr3 = download_and_prepare_UTRs(source = source, min_size = 50)
           
         utr5 = utr5.to_dict(orient = 'list')
         
         file_path = 'data/utr5.json'
         file_path = os.path.join(source, file_path)
```

### Comparing `JBioSeqTools-2.0.4/jbst/seq_tools.py` & `JBioSeqTools-2.0.5/jbst/seq_tools.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/tests/fasta_vector_test.fasta` & `JBioSeqTools-2.0.5/jbst/tests/fasta_vector_test.fasta`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/jbst/tests/jseq_tests.py` & `JBioSeqTools-2.0.5/jbst/tests/jseq_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -4956,15 +4956,15 @@
                            'input_dict_mrna_1', 'input_dict_mrna_2','input_dict_mrna_3', 'input_dict_mrna_4', 'input_dict_mrna_5',
                            'input_dict_mrna_6']
 
 
 
 tests_dictonaries = [test_rnai_list, test_transcription_list, test_expression_list]
 
-tests_dictonaries_names = [test_expression_list_names, test_rnai_list_names, test_transcription_list_names]
+tests_dictonaries_names = [test_rnai_list_names, test_transcription_list_names, test_expression_list_names]
 
 non = ['input_dict_expression_333', 'input_dict_rnai_7', 'input_dict_expression_4444444', 'input_dict_expression_44444441', 
        'input_dict_rnai_12', 'input_dict_rnai_777','input_dict_rnai_888', 'input_dict_rnai_1212',
        'input_dict_rnai_77777', 'input_dict_rnai_88888', 'input_dict_rnai_121212','input_dict_transcript_rnai_6']
 
 
  #       _  ____   _         _____              _                      __ _____  __
```

### Comparing `JBioSeqTools-2.0.4/jbst/vector_build.py` & `JBioSeqTools-2.0.5/jbst/vector_build.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.4/setup.py` & `JBioSeqTools-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.0.4' 
+VERSION = '2.0.5' 
 DESCRIPTION = 'JBioSeqTools'
 LONG_DESCRIPTION = 'JBioSeqTools is the Python library for biological sequence optimization (GC % content & codon frequency), restriction places removal, DNA/RNA structure prediction, and RNAi selection. It also allows the building of many plasmid vectors with the possibility of choosing sequences such as transcript, promoter, enhancer, molecular fluorescent tag, etc. Finally, the user obtains a ready-for-order construct with a whole sequence and visualization. Package description  on https://github.com/jkubis96/JBioSeqTools'
 
 # Setting up
 setup(
         name="JBioSeqTools", 
         version=VERSION,
```

