# Comparing `tmp/dkist-spectral-lines-2.0.0rc1.tar.gz` & `tmp/dkist_spectral_lines-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-spectral-lines-2.0.0rc1.tar", last modified: Wed Jun 28 20:59:19 2023, max compression
+gzip compressed data, was "dkist_spectral_lines-3.0.0.tar", last modified: Thu May 23 21:08:35 2024, max compression
```

## Comparing `dkist-spectral-lines-2.0.0rc1.tar` & `dkist_spectral_lines-3.0.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 20:59:19.947974 dkist-spectral-lines-2.0.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2448 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4198 2023-06-28 20:59:19.947974 dkist-spectral-lines-2.0.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3640 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2066 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 20:59:19.943974 dkist-spectral-lines-2.0.0rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/changelog/2.misc.rst
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/changelog/3.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      643 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 20:59:19.943974 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6232 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/lines.py
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1475 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/search.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 20:59:19.947974 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1416 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/tests/test_lines.py
--rw-rw-rw-   0 root         (0) root         (0)     1964 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     6114 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/tests/test_search.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 20:59:19.947974 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4198 2023-06-28 20:59:19.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-06-28 20:59:19.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-28 20:59:19.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-06-28 20:59:19.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-28 20:59:19.000000 dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 20:59:19.947974 dkist-spectral-lines-2.0.0rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/docs/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 20:59:19.947974 dkist-spectral-lines-2.0.0rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-06-28 20:59:19.947974 dkist-spectral-lines-2.0.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-28 20:59:14.000000 dkist-spectral-lines-2.0.0rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 21:08:35.223024 dkist_spectral_lines-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2448 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)      663 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4917 2024-05-23 21:08:35.223024 dkist_spectral_lines-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2495 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 21:08:35.219024 dkist_spectral_lines-3.0.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      643 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 21:08:35.219024 dkist_spectral_lines-3.0.0/dkist_spectral_lines/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-23 21:08:35.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6232 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines/lines.py
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines/search.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 21:08:35.219024 dkist_spectral_lines-3.0.0/dkist_spectral_lines/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1416 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines/tests/test_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6114 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines/tests/test_search.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 21:08:35.219024 dkist_spectral_lines-3.0.0/dkist_spectral_lines.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4917 2024-05-23 21:08:35.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-23 21:08:35.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-23 21:08:35.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-23 21:08:34.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-23 21:08:35.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-23 21:08:35.000000 dkist_spectral_lines-3.0.0/dkist_spectral_lines.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 21:08:35.219024 dkist_spectral_lines-3.0.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/docs/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 21:08:35.219024 dkist_spectral_lines-3.0.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3257 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-23 21:08:35.223024 dkist_spectral_lines-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2024-05-23 21:08:21.000000 dkist_spectral_lines-3.0.0/tox.ini
```

### Comparing `dkist-spectral-lines-2.0.0rc1/.gitignore` & `dkist_spectral_lines-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-2.0.0rc1/.pre-commit-config.yaml` & `dkist_spectral_lines-3.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-2.0.0rc1/PKG-INFO` & `dkist_spectral_lines-3.0.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: dkist-spectral-lines
-Version: 2.0.0rc1
-Summary: Spectral line metadata for the DKIST suite of instruments
-Home-page: https://bitbucket.org/dkistdc/dkist-spectral-lines/src/main/
-Author: NSO / AURA
-Author-email: "dkistdc@nso.edu"
-License: MIT
-Project-URL: Documentation, https://docs.dkist.nso.edu/projects/spectral-lines
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.11
-Provides-Extra: test
-Provides-Extra: docs
-
 dkist-spectral-lines
 =====================
 
 Overview
 --------
 The dkist-spectral-lines package consolidates the definition of metadata associated with spectral lines observed by the
 DKIST instruments.
```

### Comparing `dkist-spectral-lines-2.0.0rc1/bitbucket-pipelines.yml` & `dkist_spectral_lines-3.0.0/bitbucket-pipelines.yml`

 * *Files 15% similar despite different names*

```diff
@@ -5,73 +5,86 @@
         caches:
           - pip
         name: Lint
         script:
           - pip install pre-commit
           - pre-commit install
           - pre-commit run --all-files
-    - step: &changelog
+    - step: &changelog_fragments
         caches:
           - pip
-        name: Changelog
+        name: Check for added fragments
         script:
           - pip install towncrier
           # We need to fetch the main branch to compare against
           - git remote set-branches --add origin main
           - git fetch origin main
           - towncrier check --compare-with origin/main
     - step: &scan
         caches:
           - pip
         name: Scan
         script:
-          - pip install -e .
+          - pip install .
           - pip freeze | grep -v @ > requirements.txt
           - cat requirements.txt
           - echo $SNYK_VERSION
           - curl -L -o snyk https://github.com/snyk/snyk/releases/download/$SNYK_VERSION/snyk-linux
           - chmod 755 snyk
           - ./snyk -d auth $SNYK_TOKEN
           - echo $SNYK_IGNORE
           - for id in $SNYK_IGNORE; do echo Ignoring $id; ./snyk ignore $id; done
           - cat .snyk || echo "No .snyk found. Probably because there was nothing to ignore."
           - echo $SNYK_CLI_COMMAND
           - $SNYK_CLI_COMMAND
-    - step: &test
+    - step: &test-311
         caches:
           - pip
-        name: Test
+        name: Test Python 3.11
         script:
-          - pip install .[test]
-          - pytest -m "not development" --cov dkist_spectral_lines
-    - step: &push
+          - pip install -U pip
+          - pip install tox
+          - tox run -e py311
+    - step: &test311-min
+        image: python:3.11
         caches:
           - pip
-        name: Push
+        name: Test Python 3.11 - Minimum
         script:
-          - python setup.py sdist
-          - pip install twine
-          - twine upload dist/*
+          - pip install -U pip
+          - pip install tox
+          - tox run -e py311-min
+    - step: &publish
+        caches:
+          - pip
+        name: Publish
+        script:
+          - pip install -U pip
+          - pip install twine build
+          - python -m build --outdir wheelhouse .
+          - python -m twine upload --skip-existing wheelhouse/*
     - step: &check_changelog
         name: Check for updated CHANGELOG
         script:
           - ./check_changelog_updated.sh
 
 options:
   max-time: 25
 pipelines:
   default:
     - parallel:
       - step: *lint
-      - step: *changelog
+      - step: *changelog_fragments
     - parallel:
       - step: *scan
-      - step: *test
+      - step: *test-311
+      - step: *test311-min
   tags:
     'v*':
       - parallel:
         - step: *check_changelog
         - step: *lint
       - parallel:
         - step: *scan
-        - step: *test
-      - step: *push
+        - step: *test-311
+        - step: *test311-min
+      - step: *publish
```

### Comparing `dkist-spectral-lines-2.0.0rc1/check_changelog_updated.sh` & `dkist_spectral_lines-3.0.0/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/lines.py` & `dkist_spectral_lines-3.0.0/dkist_spectral_lines/lines.py`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/models.py` & `dkist_spectral_lines-3.0.0/dkist_spectral_lines/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Spectral Line and Filter data structures."""
 from enum import StrEnum
 from enum import unique
+from typing import Type
 
 import astropy.units as u
 from pydantic import BaseModel
-from pydantic import validator
+from pydantic import BeforeValidator
+from pydantic import ConfigDict
+from typing_extensions import Annotated
 
 
 @unique
 class DiagnosticSpecies(StrEnum):
     """Controlled list of values for the prefix of a spectral line.  Diagnostic species values should NOT be changed after they have been released lest they produce duplicates in the set of processed dkist data."""
 
     H_GAMMA = "H gamma"
@@ -37,29 +40,29 @@
     FE_XI = "Fe XI"
     H_ALPHA = "H alpha"
     CA_II_K = "Ca II K"
     NA_I = "Na I"
     MG_I_B1 = "Mg I b1"
 
 
-class SpectralLine(BaseModel):
-    """Spectral line data model."""
+def validate_rest_wavelength_in_air(rest_wavelength_in_air: u.Quantity) -> u.Quantity:
+    """Ensure that the rest wavelength is and astropy unit in nanometers."""
+    try:
+        return rest_wavelength_in_air.to(u.nm)
+    except AttributeError as e:
+        raise ValueError("rest_wavelength_in_air must be an astropy.unit") from e
 
-    diagnostic_species: DiagnosticSpecies
-    rest_wavelength_in_air: u.Quantity
 
-    @validator("rest_wavelength_in_air")
-    def convert_to_nanometers(cls, v):
-        """Validate wavelength unit is for distance and convert to nanometers."""
-        return v.to(u.nm)
+class SpectralLine(BaseModel):
+    """Spectral line data model."""
 
-    class Config:
-        """pydantic.BaseModel configuration."""
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
-        arbitrary_types_allowed = True
+    diagnostic_species: DiagnosticSpecies
+    rest_wavelength_in_air: Annotated[u.Quantity, BeforeValidator(validate_rest_wavelength_in_air)]
 
     @property
     def name(self) -> str:
         """Return the name in a display friendly format."""
         return f"{self.diagnostic_species} ({self.rest_wavelength_in_air.value} {self.rest_wavelength_in_air.unit})"
 
     def __lt__(self, other):
```

### Comparing `dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/search.py` & `dkist_spectral_lines-3.0.0/dkist_spectral_lines/search.py`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/tests/test_lines.py` & `dkist_spectral_lines-3.0.0/dkist_spectral_lines/tests/test_lines.py`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/tests/test_models.py` & `dkist_spectral_lines-3.0.0/dkist_spectral_lines/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines/tests/test_search.py` & `dkist_spectral_lines-3.0.0/dkist_spectral_lines/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-2.0.0rc1/dkist_spectral_lines.egg-info/SOURCES.txt` & `dkist_spectral_lines-3.0.0/dkist_spectral_lines.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 CHANGELOG.rst
+LICENSE
+MANIFEST.in
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
-setup.cfg
-setup.py
+tox.ini
 changelog/.gitempty
-changelog/2.misc.rst
-changelog/3.misc.rst
 dkist_spectral_lines/__init__.py
+dkist_spectral_lines/_version.py
 dkist_spectral_lines/lines.py
 dkist_spectral_lines/models.py
 dkist_spectral_lines/search.py
 dkist_spectral_lines.egg-info/PKG-INFO
 dkist_spectral_lines.egg-info/SOURCES.txt
 dkist_spectral_lines.egg-info/dependency_links.txt
+dkist_spectral_lines.egg-info/not-zip-safe
 dkist_spectral_lines.egg-info/requires.txt
 dkist_spectral_lines.egg-info/top_level.txt
 dkist_spectral_lines/tests/__init__.py
 dkist_spectral_lines/tests/test_lines.py
 dkist_spectral_lines/tests/test_models.py
 dkist_spectral_lines/tests/test_search.py
 docs/Makefile
```

### Comparing `dkist-spectral-lines-2.0.0rc1/docs/Makefile` & `dkist_spectral_lines-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-2.0.0rc1/docs/conf.py` & `dkist_spectral_lines-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-2.0.0rc1/docs/make.bat` & `dkist_spectral_lines-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-spectral-lines-2.0.0rc1/licenses/LICENSE.rst` & `dkist_spectral_lines-3.0.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

