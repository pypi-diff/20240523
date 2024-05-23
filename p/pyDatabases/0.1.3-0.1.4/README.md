# Comparing `tmp/pydatabases-0.1.3.tar.gz` & `tmp/pydatabases-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydatabases-0.1.3.tar", last modified: Thu May  9 12:13:49 2024, max compression
+gzip compressed data, was "pydatabases-0.1.4.tar", last modified: Thu May 23 05:35:22 2024, max compression
```

## Comparing `pydatabases-0.1.3.tar` & `pydatabases-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 12:13:49.077406 pydatabases-0.1.3/
--rw-rw-rw-   0        0        0     1089 2022-11-24 10:36:30.000000 pydatabases-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      761 2024-05-09 12:13:49.069348 pydatabases-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-16 22:31:17.000000 pydatabases-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 12:13:49.018670 pydatabases-0.1.3/pyDatabases/
--rw-rw-rw-   0        0        0       67 2024-05-08 09:08:36.000000 pydatabases-0.1.3/pyDatabases/__init__.py
--rw-rw-rw-   0        0        0    12976 2024-05-07 13:38:36.000000 pydatabases-0.1.3/pyDatabases/auxfuncs.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:13:49.057126 pydatabases-0.1.3/pyDatabases/gpyDB/
--rw-rw-rw-   0        0        0      101 2024-05-08 09:08:38.000000 pydatabases-0.1.3/pyDatabases/gpyDB/__init__.py
--rw-rw-rw-   0        0        0    20468 2024-05-09 11:27:53.000000 pydatabases-0.1.3/pyDatabases/gpyDB/database.py
--rw-rw-rw-   0        0        0    24932 2024-05-09 11:14:06.000000 pydatabases-0.1.3/pyDatabases/gpyDB/gpyDB.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:13:49.069348 pydatabases-0.1.3/pyDatabases/simpleDB/
--rw-rw-rw-   0        0        0       23 2024-04-05 12:13:25.000000 pydatabases-0.1.3/pyDatabases/simpleDB/__init__.py
--rw-rw-rw-   0        0        0     6339 2024-04-15 19:40:03.000000 pydatabases-0.1.3/pyDatabases/simpleDB/simpleDB.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:13:49.069348 pydatabases-0.1.3/pyDatabases.egg-info/
--rw-rw-rw-   0        0        0      761 2024-05-09 12:13:48.000000 pydatabases-0.1.3/pyDatabases.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-05-09 12:13:48.000000 pydatabases-0.1.3/pyDatabases.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 12:13:48.000000 pydatabases-0.1.3/pyDatabases.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-09 12:13:48.000000 pydatabases-0.1.3/pyDatabases.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-09 12:13:48.000000 pydatabases-0.1.3/pyDatabases.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 12:13:49.077406 pydatabases-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      734 2024-05-09 12:11:41.000000 pydatabases-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:35:22.836967 pydatabases-0.1.4/
+-rw-rw-rw-   0        0        0     1089 2022-11-24 10:36:30.000000 pydatabases-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      761 2024-05-23 05:35:22.833014 pydatabases-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-16 22:31:17.000000 pydatabases-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 05:35:22.612788 pydatabases-0.1.4/pyDatabases/
+-rw-rw-rw-   0        0        0       67 2024-05-08 09:08:36.000000 pydatabases-0.1.4/pyDatabases/__init__.py
+-rw-rw-rw-   0        0        0    12976 2024-05-16 07:21:53.000000 pydatabases-0.1.4/pyDatabases/auxfuncs.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:35:22.773328 pydatabases-0.1.4/pyDatabases/gpyDB/
+-rw-rw-rw-   0        0        0      101 2024-05-08 09:08:38.000000 pydatabases-0.1.4/pyDatabases/gpyDB/__init__.py
+-rw-rw-rw-   0        0        0    20496 2024-05-21 07:39:44.000000 pydatabases-0.1.4/pyDatabases/gpyDB/database.py
+-rw-rw-rw-   0        0        0    24944 2024-05-22 11:54:33.000000 pydatabases-0.1.4/pyDatabases/gpyDB/gpyDB.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:35:22.824965 pydatabases-0.1.4/pyDatabases/simpleDB/
+-rw-rw-rw-   0        0        0       23 2024-04-05 12:13:25.000000 pydatabases-0.1.4/pyDatabases/simpleDB/__init__.py
+-rw-rw-rw-   0        0        0     6339 2024-04-15 19:40:03.000000 pydatabases-0.1.4/pyDatabases/simpleDB/simpleDB.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:35:22.828971 pydatabases-0.1.4/pyDatabases.egg-info/
+-rw-rw-rw-   0        0        0      761 2024-05-23 05:35:22.000000 pydatabases-0.1.4/pyDatabases.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-05-23 05:35:22.000000 pydatabases-0.1.4/pyDatabases.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 05:35:22.000000 pydatabases-0.1.4/pyDatabases.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-23 05:35:22.000000 pydatabases-0.1.4/pyDatabases.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-23 05:35:22.000000 pydatabases-0.1.4/pyDatabases.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 05:35:22.836967 pydatabases-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-05-23 05:34:51.000000 pydatabases-0.1.4/setup.py
```

### Comparing `pydatabases-0.1.3/LICENSE` & `pydatabases-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatabases-0.1.3/PKG-INFO` & `pydatabases-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDatabases
-Version: 0.1.3
+Version: 0.1.4
 Summary: Small collection of database classes based primarily pandas, secondarily scipy and GAMS.
 Home-page: https://github.com/ChampionApe/pyDatabases
 Author: Rasmus K. Skjødt Berg
 Author-email: rasmus.kehlet.berg@econ.ku.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `pydatabases-0.1.3/pyDatabases/auxfuncs.py` & `pydatabases-0.1.4/pyDatabases/auxfuncs.py`

 * *Files identical despite different names*

### Comparing `pydatabases-0.1.3/pyDatabases/gpyDB/database.py` & `pydatabases-0.1.4/pyDatabases/gpyDB/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 	@property
 	def domains(self):
 		return [] if self.index is None else self.index.names
 
 	@property
 	def np(self):
-		return np.hstack([self.vals.values.reshape(len(self),1), 
+		return np.hstack([self.vals.values.astype(float).reshape(len(self),1), 
 				np.vstack([np.full(len(self), v) for k,v in self.defaultAttrs.items() if k != 'level']).T])
 
 	@property
 	def defaultAttrs(self):
 		return default_attributes_variables
 
 	@property
@@ -371,15 +371,15 @@
 		""" Explanatory text accompanying index symbols; for now, pass empty vector with suitable shape."""
 		return np.full((len(s),1), '', dtype = 'object')
 	@staticmethod
 	def gpyVar2np(s):
 		return gmdFromGpy.gpyIdx2np(s.vals.index), s.np
 	@staticmethod
 	def gpyPar2np(s):
-		return gmdFromGpy.gpyIdx2np(s.vals.index), s.vals.values.reshape(len(s),1)
+		return gmdFromGpy.gpyIdx2np(s.vals.index), s.vals.values.astype(float).reshape(len(s),1)
 	@staticmethod
 	def gpyScalarVar2np(s):
 		return np.empty((1,0), dtype =object), np.array([list((gt._internals.constants.VAR_DEFAULT_VALUES['free'] |{'level': s.vals}).values())])
 	@staticmethod
 	def gpyScalarPar2np(s):
 		return np.empty((1,0), dtype =object), np.array([[s.vals]])
```

### Comparing `pydatabases-0.1.3/pyDatabases/gpyDB/gpyDB.py` & `pydatabases-0.1.4/pyDatabases/gpyDB/gpyDB.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,15 +460,15 @@
 			AggDB.updateSubsetsFromSets(db)
 			AggDB.updateMapsFromSets(db)
 		return db
 
 	def readSets(db, types=None, ignore_alias=True):
 		""" read and define set elements from all symbols of type 'types'. """
 		if ignore_alias:
-			[db.aom(gpy(symbol.index.get_level_values(setName).unique())) for symbol in db.getTypes(noneInit(types,['var','par'])).values() for setName in (set(symbol.domains)-db.alias_notin_db)];
+			[db.aom(gpy(symbol.index.get_level_values(setName).unique().rename(db.aliasAll(setName)[0]))) for symbol in db.getTypes(noneInit(types,['var','par'])).values() for setName in set(symbol.domains)];
 		else:
 			[db.aom(gpy(symbol.index.get_level_values(setName).unique())) for symbol in db.getTypes(noneInit(types,['var','par'])).values() for setName in set(symbol.domains)];
 
 	def cleanSets(db):
 		""" create empty indices for all sets  """
 		[db.__setitem__(set_, pd.Index([], name = set_)) for set_ in set(db.getTypes(['set']))-set(['alias_set','alias_map2'])];
```

### Comparing `pydatabases-0.1.3/pyDatabases/simpleDB/simpleDB.py` & `pydatabases-0.1.4/pyDatabases/simpleDB/simpleDB.py`

 * *Files identical despite different names*

### Comparing `pydatabases-0.1.3/pyDatabases.egg-info/PKG-INFO` & `pydatabases-0.1.4/pyDatabases.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDatabases
-Version: 0.1.3
+Version: 0.1.4
 Summary: Small collection of database classes based primarily pandas, secondarily scipy and GAMS.
 Home-page: https://github.com/ChampionApe/pyDatabases
 Author: Rasmus K. Skjødt Berg
 Author-email: rasmus.kehlet.berg@econ.ku.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `pydatabases-0.1.3/setup.py` & `pydatabases-0.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
   long_description = file.read()
 
 setuptools.setup(
   name="pyDatabases",
-  version="0.1.3",
+  version="0.1.4",
   author="Rasmus K. Skjødt Berg",
   author_email="rasmus.kehlet.berg@econ.ku.dk",
   description="Small collection of database classes based primarily pandas, secondarily scipy and GAMS.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ChampionApe/pyDatabases",
   packages=setuptools.find_packages(),
```

