# Comparing `tmp/multi_repo_automation-1.2.0.tar.gz` & `tmp/multi_repo_automation-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_repo_automation-1.2.0.tar", max compression
+gzip compressed data, was "multi_repo_automation-1.3.0.tar", max compression
```

## Comparing `multi_repo_automation-1.2.0.tar` & `multi_repo_automation-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1284 2024-03-06 13:47:42.257515 multi_repo_automation-1.2.0/LICENSE
--rw-r--r--   0        0        0     2516 2024-03-06 13:47:42.257515 multi_repo_automation-1.2.0/README.md
--rw-r--r--   0        0        0    28854 2024-03-06 13:47:42.257515 multi_repo_automation-1.2.0/multi_repo_automation/__init__.py
--rw-r--r--   0        0        0     6415 2024-03-06 13:47:42.257515 multi_repo_automation-1.2.0/multi_repo_automation/commented_yaml.py
--rw-r--r--   0        0        0    44954 2024-03-06 13:47:42.257515 multi_repo_automation-1.2.0/multi_repo_automation/editor.py
--rw-r--r--   0        0        0     4933 2024-03-06 13:47:42.257515 multi_repo_automation-1.2.0/multi_repo_automation/tools.py
--rw-r--r--   0        0        0     2248 2024-03-06 13:48:10.845588 multi_repo_automation-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3787 1970-01-01 00:00:00.000000 multi_repo_automation-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1284 2024-05-23 12:16:55.491874 multi_repo_automation-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2516 2024-05-23 12:16:55.491874 multi_repo_automation-1.3.0/README.md
+-rw-r--r--   0        0        0    29391 2024-05-23 12:16:55.491874 multi_repo_automation-1.3.0/multi_repo_automation/__init__.py
+-rw-r--r--   0        0        0     6415 2024-05-23 12:16:55.491874 multi_repo_automation-1.3.0/multi_repo_automation/commented_yaml.py
+-rw-r--r--   0        0        0    44969 2024-05-23 12:16:55.491874 multi_repo_automation-1.3.0/multi_repo_automation/editor.py
+-rw-r--r--   0        0        0     4933 2024-05-23 12:16:55.491874 multi_repo_automation-1.3.0/multi_repo_automation/tools.py
+-rw-r--r--   0        0        0     2268 2024-05-23 12:18:19.159460 multi_repo_automation-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3807 1970-01-01 00:00:00.000000 multi_repo_automation-1.3.0/PKG-INFO
```

### Comparing `multi_repo_automation-1.2.0/LICENSE` & `multi_repo_automation-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multi_repo_automation-1.2.0/README.md` & `multi_repo_automation-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `multi_repo_automation-1.2.0/multi_repo_automation/__init__.py` & `multi_repo_automation-1.3.0/multi_repo_automation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -528,21 +528,35 @@
     From the `SECURITY.md` file.
     """
     versions: list[VersionSupport] = []
     security = get_security(repo)
     if security is not None:
         if "Version" not in security.headers:
             return versions
+
+        alternate_tags = []
+        if "Alternate Tag" in security.headers:
+            alternate_tag_index = security.headers.index("Alternate Tag")
+            for data in security.data:
+                current_alternate_tags = data[alternate_tag_index].split(", ")
+                current_alternate_tags = [tag.strip() for tag in current_alternate_tags]
+                alternate_tags.extend(current_alternate_tags)
+
         version_index = security.headers.index("Version")
         support_index = security.headers.index("Supported Until")
         for data in security.data:
-            if data[support_index] != "Unsupported" and data[version_index] != get_default_branch():
+            version = data[version_index]
+            if (
+                data[support_index] != "Unsupported"
+                and version != get_default_branch()
+                and version not in alternate_tags
+            ):
                 versions.append(
                     {
-                        "version": data[version_index],
+                        "version": version,
                         "supported_until": data[support_index],
                     }
                 )
     return versions
 
 
 def get_stabilization_versions(repo: Repo) -> list[str]:
```

### Comparing `multi_repo_automation-1.2.0/multi_repo_automation/commented_yaml.py` & `multi_repo_automation-1.3.0/multi_repo_automation/commented_yaml.py`

 * *Files identical despite different names*

### Comparing `multi_repo_automation-1.2.0/multi_repo_automation/editor.py` & `multi_repo_automation-1.3.0/multi_repo_automation/editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1242,15 +1242,15 @@
             attribute[key] = value
 
         index = self.regex_manager_index(data, comment)
 
         if index is not None:
             self.data["regexManagers"][index] = attribute
         else:
-            self.data["regexManagers"].append(attribute)
+            self.data.setdefault("regexManagers", []).append(attribute)
 
     def remove_regex_manager(self, data: dict[str, Any], comment: Optional[list[str]] = None) -> None:
         """Remove a regex manager to the Renovate config."""
         index = self.regex_manager_index(data, comment)
 
         if "regexManagers" not in self.data:
             self.data["regexManagers"] = JSON5List()
```

### Comparing `multi_repo_automation-1.2.0/multi_repo_automation/tools.py` & `multi_repo_automation-1.3.0/multi_repo_automation/tools.py`

 * *Files identical despite different names*

### Comparing `multi_repo_automation-1.2.0/pyproject.toml` & `multi_repo_automation-1.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 strict = true
 
 [tool.poetry]
 name = "multi-repo-automation"
-version = "1.2.0"
+version = "1.3.0"
 description = "Library for automation updates on multiple repositories."
 readme = "README.md"
 keywords = ["pre-commit"]
 license = "BSD-2-Clause"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -32,31 +32,32 @@
 authors = ["Stéphane Brunner <stephane.brunner@gmail.com>"]
 repository = "https://github.com/sbrunner/multi-repo-automation"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 PyYAML = "6.0.1"
 requests = "2.31.0"
-"ruamel.yaml" = "0.18.5"
-identify = "2.5.33"
-c2cciutils = { version = "1.6.15", optional = true }
-tomlkit = "0.12.3"
-json5 = "0.9.14"
+"ruamel.yaml" = "0.18.6"
+identify = "2.5.35"
+c2cciutils = { version = "1.6.18", optional = true }
+tomlkit = "0.12.4"
+json5 = "0.9.24"
 configupdater = "3.2"
-typing_extensions = "4.9.0"
+typing_extensions = "4.10.0"
+idna = "3.7"
 
 [tool.poetry.extras]
 update_stabilization_branches = ["c2cciutils"]
 
 [tool.poetry.group.dev.dependencies]
 prospector = { extras = ["with_bandit", "with_mypy", "with_pyroma"], version = "1.10.3" }
-types-PyYAML = "6.0.12.12"
-types-requests = "2.31.0.20240125"
-prospector-profile-duplicated = "0.5.1"
-prospector-profile-utils = "1.6.0"
+types-PyYAML = "6.0.12.20240311"
+types-requests = "2.31.0.20240311"
+prospector-profile-duplicated = "1.2.0"
+prospector-profile-utils = "1.7.2"
 
 [tool.poetry.scripts]
 mra-yaml = "multi_repo_automation.commented_yaml:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "poetry-plugin-tweak-dependencies-version", "poetry-plugin-drop-python-upper-constraint"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `multi_repo_automation-1.2.0/PKG-INFO` & `multi_repo_automation-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-repo-automation
-Version: 1.2.0
+Version: 1.3.0
 Summary: Library for automation updates on multiple repositories.
 Home-page: https://github.com/sbrunner/multi-repo-automation
 License: BSD-2-Clause
 Keywords: pre-commit
 Author: Stéphane Brunner
 Author-email: stephane.brunner@gmail.com
 Requires-Python: >=3.9
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Provides-Extra: update-stabilization-branches
 Requires-Dist: PyYAML
 Requires-Dist: c2cciutils ; extra == "update-stabilization-branches"
 Requires-Dist: configupdater
 Requires-Dist: identify
+Requires-Dist: idna
 Requires-Dist: json5
 Requires-Dist: requests
 Requires-Dist: ruamel.yaml
 Requires-Dist: tomlkit
 Requires-Dist: typing_extensions
 Project-URL: Repository, https://github.com/sbrunner/multi-repo-automation
 Description-Content-Type: text/markdown
```

