# Comparing `tmp/pydicomsorter-0.9.0.tar.gz` & `tmp/pydicomsorter-0.9.1.tar.gz`

## Comparing `pydicomsorter-0.9.0.tar` & `pydicomsorter-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0   237059 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/pixi.lock
--rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/config/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/config/coverage.toml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/config/hatch.toml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/config/mkdocs.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/config/releaserc.toml
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/config/ruff.toml
--rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/docs/about.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/docs/index.md
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/__init__.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/cli.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/dicomsort.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/io.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/options.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/parser.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/tags4format.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/sandbox/__init__.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/sandbox/dicomsort.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/sandbox/diffwork.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/tests/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/tests/test_say_hello.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/LICENSE
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/README.md
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   237059 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/pixi.lock
+-rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/config/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/config/coverage.toml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/config/hatch.toml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/config/releaserc.toml
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/config/ruff.toml
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/docs/index.md
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/__init__.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/cli.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/dicomsort.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/io.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/options.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/parser.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/tags4format.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/sandbox/__init__.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/sandbox/dicomsort.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/src/pydicomsorter/sandbox/diffwork.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/tests/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/README.md
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 pydicomsorter-0.9.1/PKG-INFO
```

### Comparing `pydicomsorter-0.9.0/.pre-commit-config.yaml` & `pydicomsorter-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/pixi.lock` & `pydicomsorter-0.9.1/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3974,40 +3974,40 @@
   purls:
   - pkg:pypi/pydantic?source=conda-forge-mapping
   size: 282275
   timestamp: 1713905769522
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/e4/49/f29028068b5cb364ad066a58490dd26fd1d4ba2943d829eb0f85dbc8ab06/pydantic_core-2.18.2-cp312-none-win_amd64.whl
-  sha256: b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438
+  url: https://files.pythonhosted.org/packages/15/b1/e6edfe46402a5b415fc3de86aa64fb10009b323907f8d513175bfb839aa9/pydantic_core-2.18.2-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/15/b1/e6edfe46402a5b415fc3de86aa64fb10009b323907f8d513175bfb839aa9/pydantic_core-2.18.2-cp312-cp312-macosx_10_12_x86_64.whl
-  sha256: fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
+  url: https://files.pythonhosted.org/packages/a1/c9/7d61469af6386e5846b5864bb93dc770979968c113863f923916c1a8bca2/pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/30/49/397da3f6910d62f092684a50bcaba2566825c6eee27a743846583a01fadf/pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: 6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043
+  url: https://files.pythonhosted.org/packages/e4/49/f29028068b5cb364ad066a58490dd26fd1d4ba2943d829eb0f85dbc8ab06/pydantic_core-2.18.2-cp312-none-win_amd64.whl
+  sha256: b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/a1/c9/7d61469af6386e5846b5864bb93dc770979968c113863f923916c1a8bca2/pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72
+  url: https://files.pythonhosted.org/packages/30/49/397da3f6910d62f092684a50bcaba2566825c6eee27a743846583a01fadf/pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: 6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: conda
   name: pydantic-core
   version: 2.18.2
   build: py312h2615798_0
@@ -4104,17 +4104,17 @@
   - sphinx-rtd-theme ; extra == 'docs'
   - sphinx-gallery ; extra == 'docs'
   - sphinxcontrib-napoleon ; extra == 'docs'
   - sphinx-copybutton ; extra == 'docs'
   requires_python: '>=3.7'
 - kind: pypi
   name: pydicomsorter
-  version: 0.9.0
+  version: 0.9.1
   path: .
-  sha256: dd3f41cc50e1ee2292b9acd5c46633dde72ffc007b02dd98da0918d011ad4926
+  sha256: 3ff057f04884da1a7268b9a059201795eec8ae7974486f37474e649f80299824
   requires_dist:
   - rich
   - rich-click
   - pydicom
   - pydantic
   requires_python: '>=3.12'
   editable: true
```

### Comparing `pydicomsorter-0.9.0/.github/workflows/main.yaml` & `pydicomsorter-0.9.1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/config/mkdocs.yaml` & `pydicomsorter-0.9.1/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/config/releaserc.toml` & `pydicomsorter-0.9.1/config/releaserc.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [semantic_release]
-version_variables = ["src/pydicomsorter/__init__.py:__version__"]
+version_variables = ["src/pydicomsorter/__init__.py:version"]
 version_toml = ["pyproject.toml:project.version"]
 commit_parser = "angular"
 logging_use_named_masks = false
 major_on_zero = true
 allow_zero_version = true
 tag_format = "v{version}"
```

### Comparing `pydicomsorter-0.9.0/config/ruff.toml` & `pydicomsorter-0.9.1/config/ruff.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/docs/CHANGELOG.md` & `pydicomsorter-0.9.1/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.9.1 (2024-05-22)
+
+### Fix
+
+* fix: version variable ([`23843a5`](https://github.com/jjjermiah/PyDicomSorter/commit/23843a5902fc7f88e1b69d3ada3ca4b2a2705c45))
+
+
 ## v0.9.0 (2024-05-22)
 
 ### Feature
 
 * feat: functioning cli ([`69e5d57`](https://github.com/jjjermiah/PyDicomSorter/commit/69e5d57da188b1161197a040d04477ebb278eeba))
 
 ### Fix
```

### Comparing `pydicomsorter-0.9.0/docs/about.md` & `pydicomsorter-0.9.1/docs/about.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/src/pydicomsorter/cli.py` & `pydicomsorter-0.9.1/src/pydicomsorter/cli.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/src/pydicomsorter/dicomsort.py` & `pydicomsorter-0.9.1/src/pydicomsorter/dicomsort.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/src/pydicomsorter/io.py` & `pydicomsorter-0.9.1/src/pydicomsorter/io.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/src/pydicomsorter/options.py` & `pydicomsorter-0.9.1/src/pydicomsorter/options.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/src/pydicomsorter/parser.py` & `pydicomsorter-0.9.1/src/pydicomsorter/parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/src/pydicomsorter/tags4format.py` & `pydicomsorter-0.9.1/src/pydicomsorter/tags4format.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/src/pydicomsorter/sandbox/dicomsort.py` & `pydicomsorter-0.9.1/src/pydicomsorter/sandbox/dicomsort.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/src/pydicomsorter/sandbox/diffwork.py` & `pydicomsorter-0.9.1/src/pydicomsorter/sandbox/diffwork.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/tests/test_parser.py` & `pydicomsorter-0.9.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/.gitignore` & `pydicomsorter-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/LICENSE` & `pydicomsorter-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.9.0/pyproject.toml` & `pydicomsorter-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "pydicomsorter"
-version = "0.9.0"
+version = "0.9.1"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["pydicomsorter", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
```

