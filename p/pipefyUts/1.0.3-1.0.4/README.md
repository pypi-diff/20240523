# Comparing `tmp/pipefyUts-1.0.3.tar.gz` & `tmp/pipefyUts-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipefyUts-1.0.3.tar", last modified: Thu May 23 14:31:24 2024, max compression
+gzip compressed data, was "pipefyUts-1.0.4.tar", last modified: Thu May 23 20:18:46 2024, max compression
```

## Comparing `pipefyUts-1.0.3.tar` & `pipefyUts-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:31:24.892071 pipefyUts-1.0.3/
--rw-rw-rw-   0        0        0      465 2023-04-28 18:31:34.000000 pipefyUts-1.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-04-26 17:09:25.000000 pipefyUts-1.0.3/LICENCE.txt
--rw-rw-rw-   0        0        0       55 2024-05-23 13:46:23.000000 pipefyUts-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3813 2024-05-23 14:31:24.889071 pipefyUts-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2785 2024-05-23 01:31:27.000000 pipefyUts-1.0.3/README.md
--rw-rw-rw-   0        0        0      212 2024-04-16 22:37:47.000000 pipefyUts-1.0.3/commands.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 14:31:24.827071 pipefyUts-1.0.3/pipefyUts/
--rw-rw-rw-   0        0        0     4396 2024-05-23 14:31:13.000000 pipefyUts-1.0.3/pipefyUts/__init__.py
--rw-rw-rw-   0        0        0     3286 2024-05-22 23:05:12.000000 pipefyUts-1.0.3/pipefyUts/card.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:31:24.880080 pipefyUts-1.0.3/pipefyUts/graphql/
--rw-rw-rw-   0        0        0      181 2024-05-22 22:11:18.000000 pipefyUts-1.0.3/pipefyUts/graphql/createCard.gql
--rw-rw-rw-   0        0        0      336 2024-05-22 19:41:50.000000 pipefyUts-1.0.3/pipefyUts/graphql/listCardsFromPhase.gql
--rw-rw-rw-   0        0        0      137 2024-05-23 00:58:59.000000 pipefyUts-1.0.3/pipefyUts/graphql/listMembers.gql
--rw-rw-rw-   0        0        0      109 2024-05-22 19:34:03.000000 pipefyUts-1.0.3/pipefyUts/graphql/listStartFormFields.gql
--rw-rw-rw-   0        0        0      146 2024-05-22 19:24:55.000000 pipefyUts-1.0.3/pipefyUts/graphql/presignedUrl.gql
-drwxrwxrwx   0        0        0        0 2024-05-23 14:31:24.861072 pipefyUts-1.0.3/pipefyUts.egg-info/
--rw-rw-rw-   0        0        0     3813 2024-05-23 14:31:24.000000 pipefyUts-1.0.3/pipefyUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-05-23 14:31:24.000000 pipefyUts-1.0.3/pipefyUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:31:24.000000 pipefyUts-1.0.3/pipefyUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 14:31:24.000000 pipefyUts-1.0.3/pipefyUts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 14:31:24.000000 pipefyUts-1.0.3/pipefyUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1371 2024-05-23 01:30:25.000000 pipefyUts-1.0.3/run.py
--rw-rw-rw-   0        0        0       42 2024-05-23 14:31:24.893070 pipefyUts-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      819 2024-05-23 14:31:20.000000 pipefyUts-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:18:46.669977 pipefyUts-1.0.4/
+-rw-rw-rw-   0        0        0      465 2023-04-28 18:31:34.000000 pipefyUts-1.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-04-26 17:09:25.000000 pipefyUts-1.0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       55 2024-05-23 13:46:23.000000 pipefyUts-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3813 2024-05-23 20:18:46.663978 pipefyUts-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2785 2024-05-23 01:31:27.000000 pipefyUts-1.0.4/README.md
+-rw-rw-rw-   0        0        0      212 2024-04-16 22:37:47.000000 pipefyUts-1.0.4/commands.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 20:18:46.602464 pipefyUts-1.0.4/pipefyUts/
+-rw-rw-rw-   0        0        0     4396 2024-05-23 14:31:13.000000 pipefyUts-1.0.4/pipefyUts/__init__.py
+-rw-rw-rw-   0        0        0     5268 2024-05-23 20:17:00.000000 pipefyUts-1.0.4/pipefyUts/card.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:18:46.659981 pipefyUts-1.0.4/pipefyUts/graphql/
+-rw-rw-rw-   0        0        0      181 2024-05-22 22:11:18.000000 pipefyUts-1.0.4/pipefyUts/graphql/createCard.gql
+-rw-rw-rw-   0        0        0      336 2024-05-22 19:41:50.000000 pipefyUts-1.0.4/pipefyUts/graphql/listCardsFromPhase.gql
+-rw-rw-rw-   0        0        0      137 2024-05-23 00:58:59.000000 pipefyUts-1.0.4/pipefyUts/graphql/listMembers.gql
+-rw-rw-rw-   0        0        0      109 2024-05-22 19:34:03.000000 pipefyUts-1.0.4/pipefyUts/graphql/listStartFormFields.gql
+-rw-rw-rw-   0        0        0      146 2024-05-22 19:24:55.000000 pipefyUts-1.0.4/pipefyUts/graphql/presignedUrl.gql
+drwxrwxrwx   0        0        0        0 2024-05-23 20:18:46.648977 pipefyUts-1.0.4/pipefyUts.egg-info/
+-rw-rw-rw-   0        0        0     3813 2024-05-23 20:18:46.000000 pipefyUts-1.0.4/pipefyUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2024-05-23 20:18:46.000000 pipefyUts-1.0.4/pipefyUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 20:18:46.000000 pipefyUts-1.0.4/pipefyUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 20:18:46.000000 pipefyUts-1.0.4/pipefyUts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 20:18:46.000000 pipefyUts-1.0.4/pipefyUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1393 2024-05-23 20:11:27.000000 pipefyUts-1.0.4/run.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 20:18:46.670979 pipefyUts-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      819 2024-05-23 20:18:40.000000 pipefyUts-1.0.4/setup.py
```

### Comparing `pipefyUts-1.0.3/LICENCE.txt` & `pipefyUts-1.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pipefyUts-1.0.3/PKG-INFO` & `pipefyUts-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefyUts
-Version: 1.0.3
+Version: 1.0.4
 Summary: Pipefy manipulator
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: pipefyUts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pipefyUts-1.0.3/README.md` & `pipefyUts-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pipefyUts-1.0.3/pipefyUts/__init__.py` & `pipefyUts-1.0.4/pipefyUts/__init__.py`

 * *Files identical despite different names*

### Comparing `pipefyUts-1.0.3/pipefyUts.egg-info/PKG-INFO` & `pipefyUts-1.0.4/pipefyUts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefyUts
-Version: 1.0.3
+Version: 1.0.4
 Summary: Pipefy manipulator
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: pipefyUts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pipefyUts-1.0.3/run.py` & `pipefyUts-1.0.4/run.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 
 class MyCard(NewCard):
     #DEFAULT
     __title__                = "MyCardTitle"
     __pipeid__               = "304282374"
 
     #PIPEFY FIELDS
-    descricao                = CardField(str)
+    descricao                = CardField(str,default="Teste")
     valor_total              = CardField(float)
     respons_vel_pela_an_lise = CardField(list)
     arquivos                 = CardField(list,is_file_path=True)
 
     def __init__(self,**kwargs): NewCard.__init__(self,**kwargs)
 
 
 myNewCard = MyCard(
-    descricao                = "AdtPro",
-    valor_total              = 10000,
+    # descricao                = "Teste",
+    valor_total              = 1234567.89,
     respons_vel_pela_an_lise = ["301975616"],
     arquivos                 = [r"C:\Users\melque\Documents\Doc1.pdf"]
 )
 
 pfy.createCard(card=myNewCard)
```

### Comparing `pipefyUts-1.0.3/setup.py` & `pipefyUts-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='pipefyUts',
-  version='1.0.3',
+  version='1.0.4',
   description='Pipefy manipulator',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

