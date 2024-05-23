# Comparing `tmp/git-versiointi-1.6rc4.tar.gz` & `tmp/git_versiointi-1.6rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-versiointi-1.6rc4.tar", last modified: Wed Nov 29 12:00:27 2023, max compression
+gzip compressed data, was "git_versiointi-1.6rc5.tar", last modified: Thu May 23 10:56:38 2024, max compression
```

## Comparing `git-versiointi-1.6rc4.tar` & `git_versiointi-1.6rc5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-11-29 12:00:27.880557 git-versiointi-1.6rc4/
--rw-r--r--   0 aha        (501) staff       (20)     6711 2023-11-29 12:00:27.880333 git-versiointi-1.6rc4/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)     6306 2023-11-29 12:00:08.000000 git-versiointi-1.6rc4/README.md
--rw-r--r--   0 aha        (501) staff       (20)      100 2023-11-29 12:00:08.000000 git-versiointi-1.6rc4/_versiointi_setuptools_build_meta.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-11-29 12:00:27.880111 git-versiointi-1.6rc4/git_versiointi.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)     6711 2023-11-29 12:00:27.000000 git-versiointi-1.6rc4/git_versiointi.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      547 2023-11-29 12:00:27.000000 git-versiointi-1.6rc4/git_versiointi.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-11-29 12:00:27.000000 git-versiointi-1.6rc4/git_versiointi.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)      247 2023-11-29 12:00:27.000000 git-versiointi-1.6rc4/git_versiointi.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)    11440 2023-11-29 11:57:08.000000 git-versiointi-1.6rc4/git_versiointi.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)       25 2023-11-29 12:00:27.000000 git-versiointi-1.6rc4/git_versiointi.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)       45 2023-11-29 12:00:27.000000 git-versiointi-1.6rc4/git_versiointi.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)      140 2023-11-29 12:00:08.000000 git-versiointi-1.6rc4/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-11-29 12:00:27.880605 git-versiointi-1.6rc4/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)     1143 2023-11-29 12:00:08.000000 git-versiointi-1.6rc4/setup.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-11-29 12:00:27.879931 git-versiointi-1.6rc4/versiointi/
--rw-r--r--   0 aha        (501) staff       (20)     5456 2023-11-29 12:00:08.000000 git-versiointi-1.6rc4/versiointi/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      566 2022-06-08 07:34:13.000000 git-versiointi-1.6rc4/versiointi/egg_info.py
--rw-r--r--   0 aha        (501) staff       (20)     5174 2023-11-29 12:00:08.000000 git-versiointi-1.6rc4/versiointi/kaytanto.py
--rw-r--r--   0 aha        (501) staff       (20)     1010 2023-11-29 12:00:08.000000 git-versiointi-1.6rc4/versiointi/oletus.py
--rw-r--r--   0 aha        (501) staff       (20)     1815 2022-06-08 07:34:13.000000 git-versiointi-1.6rc4/versiointi/parametrit.py
--rw-r--r--   0 aha        (501) staff       (20)     5491 2023-11-29 12:00:08.000000 git-versiointi-1.6rc4/versiointi/repo.py
--rw-r--r--   0 aha        (501) staff       (20)     2530 2022-06-08 07:51:15.000000 git-versiointi-1.6rc4/versiointi/tiedostot.py
--rw-r--r--   0 aha        (501) staff       (20)      654 2022-06-08 07:34:13.000000 git-versiointi-1.6rc4/versiointi/vaatimukset.py
--rw-r--r--   0 aha        (501) staff       (20)     3325 2023-11-29 12:00:08.000000 git-versiointi-1.6rc4/versiointi/versiointi.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-05-23 10:56:38.126889 git_versiointi-1.6rc5/
+-rw-r--r--   0 aha        (501) staff       (20)     6736 2024-05-23 10:56:38.126683 git_versiointi-1.6rc5/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)     6306 2023-11-29 12:00:08.000000 git_versiointi-1.6rc5/README.md
+-rw-r--r--   0 aha        (501) staff       (20)      100 2023-11-29 12:00:08.000000 git_versiointi-1.6rc5/_versiointi_setuptools_build_meta.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-05-23 10:56:38.126440 git_versiointi-1.6rc5/git_versiointi.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)     6736 2024-05-23 10:56:38.000000 git_versiointi-1.6rc5/git_versiointi.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      547 2024-05-23 10:56:38.000000 git_versiointi-1.6rc5/git_versiointi.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2024-05-23 10:56:38.000000 git_versiointi-1.6rc5/git_versiointi.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)      247 2024-05-23 10:56:38.000000 git_versiointi-1.6rc5/git_versiointi.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)    11440 2023-11-29 11:57:08.000000 git_versiointi-1.6rc5/git_versiointi.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)       35 2024-05-23 10:56:38.000000 git_versiointi-1.6rc5/git_versiointi.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)       45 2024-05-23 10:56:38.000000 git_versiointi-1.6rc5/git_versiointi.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)      153 2024-01-21 09:23:50.000000 git_versiointi-1.6rc5/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2024-05-23 10:56:38.126933 git_versiointi-1.6rc5/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)     1173 2024-01-21 09:21:45.000000 git_versiointi-1.6rc5/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-05-23 10:56:38.126119 git_versiointi-1.6rc5/versiointi/
+-rw-r--r--   0 aha        (501) staff       (20)     5456 2023-11-29 12:00:08.000000 git_versiointi-1.6rc5/versiointi/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      566 2022-06-08 07:34:13.000000 git_versiointi-1.6rc5/versiointi/egg_info.py
+-rw-r--r--   0 aha        (501) staff       (20)     5139 2024-01-21 09:21:21.000000 git_versiointi-1.6rc5/versiointi/kaytanto.py
+-rw-r--r--   0 aha        (501) staff       (20)     1010 2023-11-29 12:00:08.000000 git_versiointi-1.6rc5/versiointi/oletus.py
+-rw-r--r--   0 aha        (501) staff       (20)     1815 2022-06-08 07:34:13.000000 git_versiointi-1.6rc5/versiointi/parametrit.py
+-rw-r--r--   0 aha        (501) staff       (20)     5429 2024-01-21 09:20:11.000000 git_versiointi-1.6rc5/versiointi/repo.py
+-rw-r--r--   0 aha        (501) staff       (20)     2530 2022-06-08 07:51:15.000000 git_versiointi-1.6rc5/versiointi/tiedostot.py
+-rw-r--r--   0 aha        (501) staff       (20)      654 2022-06-08 07:34:13.000000 git_versiointi-1.6rc5/versiointi/vaatimukset.py
+-rw-r--r--   0 aha        (501) staff       (20)     3313 2024-01-21 09:19:22.000000 git_versiointi-1.6rc5/versiointi/versiointi.py
```

### Comparing `git-versiointi-1.6rc4/PKG-INFO` & `git_versiointi-1.6rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: git-versiointi
-Version: 1.6rc4
+Version: 1.6rc5
 Summary: Asennettavan pakettiversion haku git-leimojen mukaan
 Home-page: https://github.com/an7oine/git-versiointi.git
 Author: Antti Hautaniemi
 Author-email: antti.hautaniemi@pispalanit.fi
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: GitPython
+Requires-Dist: packaging
 Requires-Dist: setuptools>=63
 
 git-versiointi
 ==============
 
 Työkalupaketti pakettiversion ja -historian sekä vaadittavien riippuvuuksien
 automaattiseen määrittämiseen.
```

### Comparing `git-versiointi-1.6rc4/README.md` & `git_versiointi-1.6rc5/README.md`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc4/git_versiointi.egg-info/PKG-INFO` & `git_versiointi-1.6rc5/git_versiointi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: git-versiointi
-Version: 1.6rc4
+Version: 1.6rc5
 Summary: Asennettavan pakettiversion haku git-leimojen mukaan
 Home-page: https://github.com/an7oine/git-versiointi.git
 Author: Antti Hautaniemi
 Author-email: antti.hautaniemi@pispalanit.fi
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: GitPython
+Requires-Dist: packaging
 Requires-Dist: setuptools>=63
 
 git-versiointi
 ==============
 
 Työkalupaketti pakettiversion ja -historian sekä vaadittavien riippuvuuksien
 automaattiseen määrittämiseen.
```

### Comparing `git-versiointi-1.6rc4/git_versiointi.egg-info/SOURCES.txt` & `git_versiointi-1.6rc5/git_versiointi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc4/git_versiointi.egg-info/historia.json` & `git_versiointi-1.6rc5/git_versiointi.egg-info/historia.json`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc4/setup.py` & `git_versiointi-1.6rc5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,9 +30,13 @@
     'setuptools.finalize_distribution_options': [
       'versiointi = versiointi:finalize_distribution_options',
     ]
   },
   classifiers=[
     'Programming Language :: Python :: 3',
   ],
-  install_requires=['GitPython', 'setuptools>=63'],
+  install_requires=[
+    'GitPython',
+    'packaging',
+    'setuptools>=63',
+  ],
 )
```

### Comparing `git-versiointi-1.6rc4/versiointi/__init__.py` & `git_versiointi-1.6rc5/versiointi/__init__.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc4/versiointi/egg_info.py` & `git_versiointi-1.6rc5/versiointi/egg_info.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc4/versiointi/kaytanto.py` & `git_versiointi-1.6rc5/versiointi/kaytanto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import itertools
 import re
 
-import pkg_resources
+from packaging.version import parse, InvalidVersion
 
 
 class KaytantoMeta(type):
   '''
   Yksittäisen versiointikäytännön tyyppi.
   '''
   def __new__(mcs, name, bases, attrs, *, i=None, tyyppi=None, kaytanto=None):
@@ -147,16 +147,16 @@
       versio += indeksi
       versio = '+'.join((re.sub(
         # PEP 440: +haara.X -pääte voi sisältää
         # vain ASCII-kirjaimia, numeroita ja pisteitä.
         '[^a-zA-Z0-9.]', '', s
       ) for s in versio.split('+', 1)))
       try:
-        return str(pkg_resources.packaging.version.Version(versio))
-      except pkg_resources.packaging.version.InvalidVersion:
+        return str(parse(versio))
+      except InvalidVersion:
         return versio
       # def versio
     attrs['_versio'] = versio
 
     return super().__new__(mcs, name, tuple(bases), attrs)
     # def __new__
```

### Comparing `git-versiointi-1.6rc4/versiointi/oletus.py` & `git_versiointi-1.6rc5/versiointi/oletus.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc4/versiointi/parametrit.py` & `git_versiointi-1.6rc5/versiointi/parametrit.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc4/versiointi/repo.py` & `git_versiointi-1.6rc5/versiointi/repo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import itertools
 import re
 
-from pkg_resources import parse_version
-from pkg_resources.extern.packaging.version import InvalidVersion
+from packaging.version import parse, InvalidVersion
 
 from git.objects.commit import Commit
 from git.objects.tag import TagObject
 from git import Git, Repo
 
 
 class LiianVanha(Repo):
@@ -147,15 +146,15 @@
 
     # Mikäli yhtään symbolia ei löytynyt, palautetaan `None`.
     # Mikäli löytyi yksi, palautetaan se.
     # Mikäli löytyi useampia, palautetaan versiojärjestyksessä suurin.
     # Löytynyt, tyhjä symboli korvataan `Nonella`.
     def jarjestys(symboli):
       try:
-        return (True, parse_version(symboli), symboli)
+        return (True, parse(symboli), symboli)
       except InvalidVersion:
         return (False, None, symboli)
     try:
       symboli, *__ = sorted(
         symbolit,
         key=jarjestys,
         reverse=True,
```

### Comparing `git-versiointi-1.6rc4/versiointi/tiedostot.py` & `git_versiointi-1.6rc5/versiointi/tiedostot.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc4/versiointi/vaatimukset.py` & `git_versiointi-1.6rc5/versiointi/vaatimukset.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6rc4/versiointi/versiointi.py` & `git_versiointi-1.6rc5/versiointi/versiointi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import itertools
 import warnings
 
-from pkg_resources import parse_version
+from packaging.version import parse
 
 from .kaytanto import VersiointiMeta
 from .repo import Tietovarasto
 
 
 class Versiointi:
   '''Versiointikäytäntö.
@@ -112,15 +112,15 @@
     Args:
       haettu_versio (str / None): esim. '1.0.2' (oletus nykyinen)
       ref: git-revisio, josta haku aloitetaan (oletus HEAD)
 
     Returns:
       ref (str): git-viittaus
     '''
-    versio = str(parse_version(haettu_versio)) if haettu_versio else None
+    versio = str(parse(haettu_versio)) if haettu_versio else None
     for muutos in self.tietovarasto.muutokset(ref):
       if versio is None or self._versio(muutos) == versio:
         return muutos
     return None
     # def revisio
 
   # class Versiointi
```

