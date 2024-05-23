# Comparing `tmp/gmspython-0.1.1.tar.gz` & `tmp/gmspython-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmspython-0.1.1.tar", last modified: Thu May  9 12:27:11 2024, max compression
+gzip compressed data, was "gmspython-0.1.2.tar", last modified: Thu May 23 05:40:29 2024, max compression
```

## Comparing `gmspython-0.1.1.tar` & `gmspython-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.929472 gmspython-0.1.1/
--rw-rw-rw-   0        0        0     1089 2022-11-24 13:42:30.000000 gmspython-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      726 2024-05-09 12:27:11.929472 gmspython-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      165 2024-05-09 09:22:27.000000 gmspython-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.782232 gmspython-0.1.1/gmsPython/
--rw-rw-rw-   0        0        0      201 2024-05-08 09:08:49.000000 gmspython-0.1.1/gmsPython/__init__.py
--rw-rw-rw-   0        0        0      609 2024-05-06 08:19:01.000000 gmspython-0.1.1/gmsPython/auxfuncs.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.851294 gmspython-0.1.1/gmsPython/gamY/
--rw-rw-rw-   0        0        0       29 2024-04-24 17:03:44.000000 gmspython-0.1.1/gmsPython/gamY/__init__.py
--rw-rw-rw-   0        0        0     3865 2024-05-06 12:20:51.000000 gmspython-0.1.1/gmsPython/gamY/classes.py
--rw-rw-rw-   0        0        0    51981 2024-05-09 11:27:58.000000 gmspython-0.1.1/gmsPython/gamY/gamY.py
--rw-rw-rw-   0        0        0     4532 2024-04-24 16:52:32.000000 gmspython-0.1.1/gmsPython/gamY/patterns.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.866959 gmspython-0.1.1/gmsPython/gmsPy/
--rw-rw-rw-   0        0        0       32 2024-05-07 08:59:34.000000 gmspython-0.1.1/gmsPython/gmsPy/__init__.py
--rw-rw-rw-   0        0        0     9492 2024-05-09 11:27:59.000000 gmspython-0.1.1/gmsPython/gmsPy/gmsPy.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.882601 gmspython-0.1.1/gmsPython/gmsPyModels/
--rw-rw-rw-   0        0        0       38 2024-05-07 11:48:39.000000 gmspython-0.1.1/gmsPython/gmsPyModels/__init__.py
--rw-rw-rw-   0        0        0     1898 2024-05-09 11:28:00.000000 gmspython-0.1.1/gmsPython/gmsPyModels/gmsPyModels.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.913846 gmspython-0.1.1/gmsPython/gmsWrite/
--rw-rw-rw-   0        0        0       89 2024-04-26 07:40:14.000000 gmspython-0.1.1/gmsPython/gmsWrite/__init__.py
--rw-rw-rw-   0        0        0     5973 2024-05-09 09:25:04.000000 gmspython-0.1.1/gmsPython/gmsWrite/gmsWrite.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.929472 gmspython-0.1.1/gmsPython/nestingTree/
--rw-rw-rw-   0        0        0       91 2024-05-02 08:44:45.000000 gmspython-0.1.1/gmsPython/nestingTree/__init__.py
--rw-rw-rw-   0        0        0    10078 2024-05-08 08:58:29.000000 gmspython-0.1.1/gmsPython/nestingTree/nestingTree.py
-drwxrwxrwx   0        0        0        0 2024-05-09 12:27:11.929472 gmspython-0.1.1/gmsPython.egg-info/
--rw-rw-rw-   0        0        0      726 2024-05-09 12:27:11.000000 gmspython-0.1.1/gmsPython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      594 2024-05-09 12:27:11.000000 gmspython-0.1.1/gmsPython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 12:27:11.000000 gmspython-0.1.1/gmsPython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 12:27:11.000000 gmspython-0.1.1/gmsPython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-09 12:27:11.000000 gmspython-0.1.1/gmsPython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 12:27:11.929472 gmspython-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      706 2024-05-09 12:26:58.000000 gmspython-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:40:29.964114 gmspython-0.1.2/
+-rw-rw-rw-   0        0        0     1089 2022-11-24 13:42:30.000000 gmspython-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      726 2024-05-23 05:40:29.961114 gmspython-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2024-05-09 09:22:27.000000 gmspython-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 05:40:29.806172 gmspython-0.1.2/gmsPython/
+-rw-rw-rw-   0        0        0      201 2024-05-08 09:08:49.000000 gmspython-0.1.2/gmsPython/__init__.py
+-rw-rw-rw-   0        0        0      609 2024-05-21 08:50:25.000000 gmspython-0.1.2/gmsPython/auxfuncs.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:40:29.879321 gmspython-0.1.2/gmsPython/gamY/
+-rw-rw-rw-   0        0        0       29 2024-04-24 17:03:44.000000 gmspython-0.1.2/gmsPython/gamY/__init__.py
+-rw-rw-rw-   0        0        0     3865 2024-05-06 12:20:51.000000 gmspython-0.1.2/gmsPython/gamY/classes.py
+-rw-rw-rw-   0        0        0    51981 2024-05-09 11:27:58.000000 gmspython-0.1.2/gmsPython/gamY/gamY.py
+-rw-rw-rw-   0        0        0     4532 2024-04-24 16:52:32.000000 gmspython-0.1.2/gmsPython/gamY/patterns.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:40:29.904662 gmspython-0.1.2/gmsPython/gmsPy/
+-rw-rw-rw-   0        0        0       32 2024-05-07 08:59:34.000000 gmspython-0.1.2/gmsPython/gmsPy/__init__.py
+-rw-rw-rw-   0        0        0     9494 2024-05-17 12:01:14.000000 gmspython-0.1.2/gmsPython/gmsPy/gmsPy.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:40:29.912213 gmspython-0.1.2/gmsPython/gmsPyModels/
+-rw-rw-rw-   0        0        0       38 2024-05-07 11:48:39.000000 gmspython-0.1.2/gmsPython/gmsPyModels/__init__.py
+-rw-rw-rw-   0        0        0     2976 2024-05-21 08:59:03.000000 gmspython-0.1.2/gmsPython/gmsPyModels/gmsPyModels.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:40:29.924201 gmspython-0.1.2/gmsPython/gmsWrite/
+-rw-rw-rw-   0        0        0       89 2024-04-26 07:40:14.000000 gmspython-0.1.2/gmsPython/gmsWrite/__init__.py
+-rw-rw-rw-   0        0        0     5973 2024-05-09 09:25:04.000000 gmspython-0.1.2/gmsPython/gmsWrite/gmsWrite.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:40:29.949591 gmspython-0.1.2/gmsPython/nestingTree/
+-rw-rw-rw-   0        0        0       91 2024-05-02 08:44:45.000000 gmspython-0.1.2/gmsPython/nestingTree/__init__.py
+-rw-rw-rw-   0        0        0    10078 2024-05-08 08:58:29.000000 gmspython-0.1.2/gmsPython/nestingTree/nestingTree.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:40:29.955489 gmspython-0.1.2/gmsPython.egg-info/
+-rw-rw-rw-   0        0        0      726 2024-05-23 05:40:29.000000 gmspython-0.1.2/gmsPython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2024-05-23 05:40:29.000000 gmspython-0.1.2/gmsPython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 05:40:29.000000 gmspython-0.1.2/gmsPython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 05:40:29.000000 gmspython-0.1.2/gmsPython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 05:40:29.000000 gmspython-0.1.2/gmsPython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 05:40:29.964114 gmspython-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      706 2024-05-23 05:39:47.000000 gmspython-0.1.2/setup.py
```

### Comparing `gmspython-0.1.1/LICENSE` & `gmspython-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gmspython-0.1.1/PKG-INFO` & `gmspython-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmsPython
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automating GAMS models and execution from Python
 Home-page: https://github.com/ChampionApe/gmsPython
 Author: Rasmus K. Skjødt Berg
 Author-email: rasmus.kehlet.berg@econ.ku.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `gmspython-0.1.1/gmsPython/auxfuncs.py` & `gmspython-0.1.2/gmsPython/auxfuncs.py`

 * *Files identical despite different names*

### Comparing `gmspython-0.1.1/gmsPython/gamY/classes.py` & `gmspython-0.1.2/gmsPython/gamY/classes.py`

 * *Files identical despite different names*

### Comparing `gmspython-0.1.1/gmsPython/gamY/gamY.py` & `gmspython-0.1.2/gmsPython/gamY/gamY.py`

 * *Files identical despite different names*

### Comparing `gmspython-0.1.1/gmsPython/gamY/patterns.py` & `gmspython-0.1.2/gmsPython/gamY/patterns.py`

 * *Files identical despite different names*

### Comparing `gmspython-0.1.1/gmsPython/gmsPy/gmsPy.py` & `gmspython-0.1.2/gmsPython/gmsPy/gmsPy.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 def vFromGroup(v, add = 'par_', level = 0):
     return addToLevel(pd.MultiIndex.from_tuples(v), add = add, level = level).to_list()
 def polGridText(n, i, ϕ):
 	return f'(1-({i}/{n})**({ϕ}))'
 
 class jTerms:
 	""" Use comiled block of equations from gamY to define Groups of j-terms, adjusted blocks etc. """	
-
 	def __init__(self, compiler):
 		self.compiler = compiler
 
 	def jModel(self, name, groups, db = None, solve = None, has_read_file = True):
 		self.group = jTerms.group(name, self.compiler.blocks[name])()
 		jDecl  = self.group.declare()
 		jBlock = jTerms.adjBlock(name, self.compiler.blocks[name])
@@ -71,16 +70,18 @@
 		""" Initialize a parameter group that inherits values from the self.group. """
 		self.pGroup = Group(f'{self.group.name}0', v = vFromGroup(self.group.v))()
 		decl = self.pGroup.declareAsPar()
 		init = strBlock('# Initialize parameter group:', (self.pGroupFromGroup_v(v) for v in self.pGroup.out), end = '')
 		initScalar = f'Scalar {loopName};\n'
 		loop = strBlock(f'for ({loopName} = 1 to {n},', (self.adjustGroup_v(v, n, loopName, ϕ=ϕ) for v in self.pGroup.out), end = f"{self.solve});")
 		return decl+init+initScalar+loop
+
 	def adjustGroup_v(self, v, n, loopName, ϕ = 1):
 		return f"""{self.group.writeVar(v.lstrip('par_'), self.group.conditions, l = '.fx')} = {polGridText(n,loopName, ϕ)}*{self.pGroup.writeVar(v)};"""
+
 	def pGroupFromGroup_v(self, v):
 		return self.pGroup.writeVar(v, self.pGroup.conditions) +'='+self.group.writeVar(v.lstrip('par_'), l = '.l')+';'
 
 	@staticmethod
 	def group(name, block):
 		""" Return Group with j-terms corresponding to block of equations"""
 		return Group(f'j_{name}', v = [jTerms.eqToGroup(eq) for eq in block.values()])
```

### Comparing `gmspython-0.1.1/gmsPython/gmsPyModels/gmsPyModels.py` & `gmspython-0.1.2/gmsPython/gmsPyModels/gmsPyModels.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,62 @@
 from gmsPython.auxfuncs import *
+import os, pickle
 from pyDatabases import noneInit
 from pyDatabases.gpyDB import GpyDB
 from gmsPython.gamY.gamY import Precompiler
 from gmsPython.gmsPy.gmsPy import jTerms
 
 class Model:
 	""" Simple shell for models defined with namespaces, databases, compiler etc.."""
-	def __init__(self, name = None, ns = None, database = None, **kwargs):
+	def __init__(self, name = None, ns = None, database = None, asModule = False, **kwargs):
 		self.db = noneInit(database, GpyDB(**kwargs))
 		self.name = name
 		self.compiler = Precompiler()
 		self.j = jTerms(self.compiler)
 		self.ns = noneInit(ns, {})
 		self.m = {}
 		self.cps = {} # checkpoints
+		self._asModule = asModule
+		self.dropattrs = ['cps','job','out_db'] # what attributes are dropped in exports
 
 	### 0: Properties/customized methods
+	@classmethod
+	def load(cls, filename):
+		with open(filename, "rb") as f:
+			return pickle.load(f)
 	@property
 	def ws(self):
 		return self.db.ws
 	@property
 	def work_folder(self):
 		return self.db.work_folder
+	@property
+	def data_folder(self):
+		return self.db.data_folder
+
+	def __getstate__(self):
+		if not self._asModule:
+			self._loadDbFrom = os.path.join(self.data_folder, self.db.name)
+			self.db.export()
+		return {key:value for key,value in self.__dict__.items() if key not in (self.dropattrs+['db'])}
+		
+	def __setstate__(self,dict_):
+		""" Don't include ws. Don't include db. """
+		self.__dict__ = dict_
+		if not self._asModule:
+			self.db = GpyDB(dict_['_loadDbFrom'])
+			for m in self.m.values():
+				if isinstance(m, Model):
+					m.db = self.db
+
+	def export(self, name = None, repo = None):
+		name = self.name if name is None else name
+		repo = self.data_folder if repo is None else repo
+		with open(os.path.join(repo,name), "wb") as file:
+			pickle.dump(self, file)
 
 	### 1. Navigate symbols
 	def n(self, item, m = None):
 		try:
 			return getattr(self, f'n_{m.__class__.__name__}')(item, m)
 		except KeyError:
 			return item
@@ -38,16 +69,17 @@
 	def g(self, item, m = None):
 		return self.db[self.n(item, m = m)]
 	def get(self, item, m = None):
 		return self.db(self.n(item, m = m))
 
 	### 2: Modules
 	def addModule(self, m, **kwargs):
-		if isinstance(m, type(self)):
+		if isinstance(m, Model):
 			self.m[m.name] = m
+			self.m[m.name]._asModule = True
 		else:
 			self.m[m.name] = Module(**kwargs)
 
 	def attrFromM(self, attr):
 		""" Get attributes from self.m modules """
 		return {k:v for d in (getattr(m,attr)(m=m.name) if hasattr(m,attr) else {} for m in self.m.values()) for k,v in d.items()}
```

### Comparing `gmspython-0.1.1/gmsPython/gmsWrite/gmsWrite.py` & `gmspython-0.1.2/gmsPython/gmsWrite/gmsWrite.py`

 * *Files identical despite different names*

### Comparing `gmspython-0.1.1/gmsPython/nestingTree/nestingTree.py` & `gmspython-0.1.2/gmsPython/nestingTree/nestingTree.py`

 * *Files identical despite different names*

### Comparing `gmspython-0.1.1/gmsPython.egg-info/PKG-INFO` & `gmspython-0.1.2/gmsPython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmsPython
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automating GAMS models and execution from Python
 Home-page: https://github.com/ChampionApe/gmsPython
 Author: Rasmus K. Skjødt Berg
 Author-email: rasmus.kehlet.berg@econ.ku.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `gmspython-0.1.1/gmsPython.egg-info/SOURCES.txt` & `gmspython-0.1.2/gmsPython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmspython-0.1.1/setup.py` & `gmspython-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
   long_description = file.read()
 
 setuptools.setup(
   name="gmsPython",
-  version="0.1.1",
+  version="0.1.2",
   author="Rasmus K. Skjødt Berg",
   author_email="rasmus.kehlet.berg@econ.ku.dk",
   description="Automating GAMS models and execution from Python",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ChampionApe/gmsPython",
   packages=setuptools.find_packages(),
```

