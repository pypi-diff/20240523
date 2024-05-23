# Comparing `tmp/pyobas-1.0.2.tar.gz` & `tmp/pyobas-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobas-1.0.2.tar", last modified: Fri May 17 19:51:49 2024, max compression
+gzip compressed data, was "pyobas-1.0.3.tar", last modified: Thu May 23 14:27:25 2024, max compression
```

## Comparing `pyobas-1.0.2.tar` & `pyobas-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-17 19:51:49.866795 pyobas-1.0.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-17 19:51:41.000000 pyobas-1.0.2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2024-05-17 19:51:49.866795 pyobas-1.0.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-05-17 19:51:41.000000 pyobas-1.0.2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-17 19:51:49.862795 pyobas-1.0.2/pyobas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-17 19:51:49.866795 pyobas-1.0.2/pyobas/apis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      497 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/apis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/apis/attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/apis/collector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/apis/document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/apis/inject.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/apis/injector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/apis/kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/apis/me.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/apis/organization.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/apis/team.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/apis/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-17 19:51:49.866795 pyobas-1.0.2/pyobas/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/backends/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/backends/backend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/backends/protocol.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16141 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-17 19:51:49.866795 pyobas-1.0.2/pyobas/contracts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/contracts/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/contracts/contract_builder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5582 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/contracts/contract_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/contracts/contract_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/contracts/variable_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14284 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3865 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyobas/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-17 19:51:49.866795 pyobas-1.0.2/pyobas.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2024-05-17 19:51:49.000000 pyobas-1.0.2/pyobas.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2024-05-17 19:51:49.000000 pyobas-1.0.2/pyobas.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-17 19:51:49.000000 pyobas-1.0.2/pyobas.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2024-05-17 19:51:49.000000 pyobas-1.0.2/pyobas.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-17 19:51:49.000000 pyobas-1.0.2/pyobas.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-17 19:51:41.000000 pyobas-1.0.2/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1386 2024-05-17 19:51:49.866795 pyobas-1.0.2/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 14:27:25.912378 pyobas-1.0.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-23 14:27:16.000000 pyobas-1.0.3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2024-05-23 14:27:25.912378 pyobas-1.0.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-05-23 14:27:16.000000 pyobas-1.0.3/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 14:27:25.904378 pyobas-1.0.3/pyobas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 14:27:25.908378 pyobas-1.0.3/pyobas/apis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      497 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/collector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/inject.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/injector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/me.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/organization.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/team.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 14:27:25.908378 pyobas-1.0.3/pyobas/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/backends/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/backends/backend.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/backends/protocol.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16141 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 14:27:25.908378 pyobas-1.0.3/pyobas/contracts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/contracts/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/contracts/contract_builder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/contracts/contract_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/contracts/contract_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/contracts/variable_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14284 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3865 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 14:27:25.908378 pyobas-1.0.3/pyobas.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2024-05-23 14:27:25.000000 pyobas-1.0.3/pyobas.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2024-05-23 14:27:25.000000 pyobas-1.0.3/pyobas.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-23 14:27:25.000000 pyobas-1.0.3/pyobas.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2024-05-23 14:27:25.000000 pyobas-1.0.3/pyobas.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-23 14:27:25.000000 pyobas-1.0.3/pyobas.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1386 2024-05-23 14:27:25.912378 pyobas-1.0.3/setup.cfg
```

### Comparing `pyobas-1.0.2/LICENSE` & `pyobas-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/PKG-INFO` & `pyobas-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobas
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python API client for OpenBAS.
 Home-page: https://github.com/OpenBAS-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,17 +22,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dataclasses-json~=0.6.4
 Requires-Dist: pika~=1.3.1
 Requires-Dist: prometheus-client~=0.20.0
 Requires-Dist: python_json_logger~=2.0.4
 Requires-Dist: pyyaml~=6.0
-Requires-Dist: requests~=2.31.0
+Requires-Dist: requests~=2.32.2
 Requires-Dist: requests-toolbelt~=1.0.0
-Requires-Dist: setuptools~=69.5.1
+Requires-Dist: setuptools~=70.0.0
 Provides-Extra: dev
 Requires-Dist: black~=24.4.0; extra == "dev"
 Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
 Requires-Dist: pre-commit~=3.7.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9.0; extra == "dev"
```

### Comparing `pyobas-1.0.2/README.md` & `pyobas-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/__init__.py` & `pyobas-1.0.3/pyobas/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 from pyobas._version import (  # noqa: F401
     __author__,
     __copyright__,
     __email__,
     __license__,
     __title__,
```

### Comparing `pyobas-1.0.2/pyobas/apis/attack_pattern.py` & `pyobas-1.0.3/pyobas/apis/attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/apis/collector.py` & `pyobas-1.0.3/pyobas/apis/collector.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/apis/document.py` & `pyobas-1.0.3/pyobas/apis/document.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/apis/inject.py` & `pyobas-1.0.3/pyobas/apis/inject.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/apis/injector.py` & `pyobas-1.0.3/pyobas/apis/injector.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/apis/kill_chain_phase.py` & `pyobas-1.0.3/pyobas/apis/kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/apis/team.py` & `pyobas-1.0.3/pyobas/apis/team.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/apis/user.py` & `pyobas-1.0.3/pyobas/apis/user.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/backends/backend.py` & `pyobas-1.0.3/pyobas/backends/backend.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/backends/protocol.py` & `pyobas-1.0.3/pyobas/backends/protocol.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/base.py` & `pyobas-1.0.3/pyobas/base.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/client.py` & `pyobas-1.0.3/pyobas/client.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/contracts/contract_builder.py` & `pyobas-1.0.3/pyobas/contracts/contract_builder.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/contracts/contract_config.py` & `pyobas-1.0.3/pyobas/contracts/contract_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,20 +102,20 @@
         default_factory=lambda: [
             VariableHelper.user_variable(),
             VariableHelper.exercise_variable(),
             VariableHelper.team_variable(),
         ]
         + VariableHelper.uri_variables()
     )
-    attack_patterns_external_ids: List[str] = field(default_factory=list)
+    contract_attack_patterns_external_ids: List[str] = field(default_factory=list)
     is_atomic_testing: bool = True
     platforms: List[str] = field(default_factory=list)
 
     def add_attack_pattern(self, var: str):
-        self.attack_patterns_external_ids.append(var)
+        self.contract_attack_patterns_external_ids.append(var)
 
     def add_variable(self, var: ContractVariable):
         self.variables.append(var)
 
 
 @dataclass
 class ContractTeam(ContractCardinalityElement):
@@ -136,15 +136,15 @@
 
 def prepare_contracts(contracts):
     return list(
         map(
             lambda c: {
                 "contract_id": c.contract_id,
                 "contract_labels": c.label,
-                "contract_attack_patterns_external_ids": c.attack_patterns_external_ids,
+                "contract_attack_patterns_external_ids": c.contract_attack_patterns_external_ids,
                 "contract_content": json.dumps(c, cls=utils.EnhancedJSONEncoder),
                 "contract_platforms": c.platforms,
             },
             contracts,
         )
     )
```

### Comparing `pyobas-1.0.2/pyobas/contracts/variable_helper.py` & `pyobas-1.0.3/pyobas/contracts/variable_helper.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/exceptions.py` & `pyobas-1.0.3/pyobas/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/helpers.py` & `pyobas-1.0.3/pyobas/helpers.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/mixins.py` & `pyobas-1.0.3/pyobas/mixins.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas/utils.py` & `pyobas-1.0.3/pyobas/utils.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyobas.egg-info/PKG-INFO` & `pyobas-1.0.3/pyobas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobas
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python API client for OpenBAS.
 Home-page: https://github.com/OpenBAS-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,17 +22,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dataclasses-json~=0.6.4
 Requires-Dist: pika~=1.3.1
 Requires-Dist: prometheus-client~=0.20.0
 Requires-Dist: python_json_logger~=2.0.4
 Requires-Dist: pyyaml~=6.0
-Requires-Dist: requests~=2.31.0
+Requires-Dist: requests~=2.32.2
 Requires-Dist: requests-toolbelt~=1.0.0
-Requires-Dist: setuptools~=69.5.1
+Requires-Dist: setuptools~=70.0.0
 Provides-Extra: dev
 Requires-Dist: black~=24.4.0; extra == "dev"
 Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
 Requires-Dist: pre-commit~=3.7.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9.0; extra == "dev"
```

### Comparing `pyobas-1.0.2/pyobas.egg-info/SOURCES.txt` & `pyobas-1.0.3/pyobas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/pyproject.toml` & `pyobas-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.2/setup.cfg` & `pyobas-1.0.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 include_package_data = True
 install_requires = 
 	dataclasses-json~=0.6.4
 	pika~=1.3.1
 	prometheus-client~=0.20.0
 	python_json_logger~=2.0.4
 	pyyaml~=6.0
-	requests~=2.31.0
+	requests~=2.32.2
 	requests-toolbelt~=1.0.0
-	setuptools~=69.5.1
+	setuptools~=70.0.0
 
 [options.extras_require]
 dev = 
 	black~=24.4.0
 	build~=1.2.1
 	isort~=5.13.0
 	types-pytz~=2024.1.0.20240203
```

