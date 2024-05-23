# Comparing `tmp/dbt_meshify-0.5.3.tar.gz` & `tmp/dbt_meshify-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_meshify-0.5.3.tar", max compression
+gzip compressed data, was "dbt_meshify-0.5.4.tar", max compression
```

## Comparing `dbt_meshify-0.5.3.tar` & `dbt_meshify-0.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11356 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/LICENSE
--rw-r--r--   0        0        0     1451 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/README.md
--rw-r--r--   0        0        0       11 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/dbt_meshify/.gitignore
--rw-r--r--   0        0        0        0 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/dbt_meshify/__init__.py
--rw-r--r--   0        0        0     3710 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/dbt_meshify/change.py
--rw-r--r--   0        0        0     1941 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/dbt_meshify/change_set_processor.py
--rw-r--r--   0        0        0     3811 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/dbt_meshify/cli.py
--rw-r--r--   0        0        0     2364 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/dbt_meshify/dbt.py
--rw-r--r--   0        0        0    20303 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/dbt_meshify/dbt_projects.py
--rw-r--r--   0        0        0      623 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/dbt_meshify/exceptions.py
--rw-r--r--   0        0        0    21287 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/dbt_meshify/main.py
--rw-r--r--   0        0        0        0 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/dbt_meshify/storage/__init__.py
--rw-r--r--   0        0        0    13603 2024-03-27 20:05:25.504645 dbt_meshify-0.5.3/dbt_meshify/storage/dbt_project_editors.py
--rw-r--r--   0        0        0     8109 2024-03-27 20:05:25.508645 dbt_meshify-0.5.3/dbt_meshify/storage/file_content_editors.py
--rw-r--r--   0        0        0     4060 2024-03-27 20:05:25.508645 dbt_meshify-0.5.3/dbt_meshify/storage/file_manager.py
--rw-r--r--   0        0        0     2561 2024-03-27 20:05:25.508645 dbt_meshify-0.5.3/dbt_meshify/storage/jinja_blocks.py
--rw-r--r--   0        0        0        0 2024-03-27 20:05:25.508645 dbt_meshify-0.5.3/dbt_meshify/utilities/__init__.py
--rw-r--r--   0        0        0     1699 2024-03-27 20:05:25.508645 dbt_meshify-0.5.3/dbt_meshify/utilities/contractor.py
--rw-r--r--   0        0        0     1182 2024-03-27 20:05:25.508645 dbt_meshify-0.5.3/dbt_meshify/utilities/dependencies.py
--rw-r--r--   0        0        0     6180 2024-03-27 20:05:25.508645 dbt_meshify-0.5.3/dbt_meshify/utilities/grouper.py
--rw-r--r--   0        0        0    13544 2024-03-27 20:05:25.508645 dbt_meshify-0.5.3/dbt_meshify/utilities/linker.py
--rw-r--r--   0        0        0    14052 2024-03-27 20:05:25.508645 dbt_meshify-0.5.3/dbt_meshify/utilities/references.py
--rw-r--r--   0        0        0     6849 2024-03-27 20:05:25.508645 dbt_meshify-0.5.3/dbt_meshify/utilities/versioner.py
--rw-r--r--   0        0        0     1377 2024-03-27 20:05:25.508645 dbt_meshify-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2292 1970-01-01 00:00:00.000000 dbt_meshify-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/LICENSE
+-rw-r--r--   0        0        0     1451 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/README.md
+-rw-r--r--   0        0        0       11 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/.gitignore
+-rw-r--r--   0        0        0        0 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/__init__.py
+-rw-r--r--   0        0        0     4002 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/change.py
+-rw-r--r--   0        0        0     2051 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/change_set_processor.py
+-rw-r--r--   0        0        0     3968 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/cli.py
+-rw-r--r--   0        0        0     2364 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/dbt.py
+-rw-r--r--   0        0        0    20303 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/dbt_projects.py
+-rw-r--r--   0        0        0      623 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/exceptions.py
+-rw-r--r--   0        0        0    22289 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/main.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/storage/__init__.py
+-rw-r--r--   0        0        0    14950 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/storage/dbt_project_editors.py
+-rw-r--r--   0        0        0     8592 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/storage/file_content_editors.py
+-rw-r--r--   0        0        0     4638 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/storage/file_manager.py
+-rw-r--r--   0        0        0     2569 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/storage/jinja_blocks.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/utilities/__init__.py
+-rw-r--r--   0        0        0     1699 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/utilities/contractor.py
+-rw-r--r--   0        0        0     1182 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/utilities/dependencies.py
+-rw-r--r--   0        0        0     6180 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/utilities/grouper.py
+-rw-r--r--   0        0        0    13544 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/utilities/linker.py
+-rw-r--r--   0        0        0    14052 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/utilities/references.py
+-rw-r--r--   0        0        0     7596 2024-05-23 15:34:44.948398 dbt_meshify-0.5.4/dbt_meshify/utilities/versioner.py
+-rw-r--r--   0        0        0     1377 2024-05-23 15:34:44.952398 dbt_meshify-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2292 1970-01-01 00:00:00.000000 dbt_meshify-0.5.4/PKG-INFO
```

### Comparing `dbt_meshify-0.5.3/LICENSE` & `dbt_meshify-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_meshify-0.5.3/README.md` & `dbt_meshify-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt_meshify-0.5.3/dbt_meshify/change.py` & `dbt_meshify-0.5.4/dbt_meshify/change.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import dataclasses
 import os
 from enum import Enum
 from pathlib import Path
-from typing import Dict, Iterable, List, Optional, Protocol
+from typing import Callable, Dict, Iterable, List, Optional, Protocol
 
 
 class Operation(str, Enum):
     """An operation describes the type of work being performed."""
 
     Add = "add"
     Append = "append"
@@ -42,14 +42,15 @@
     Macro = "macro"
     Exposure = "exposure"
     Metric = "metric"
     Group = "group"
     SemanticModel = "semantic_model"
     Project = "project"
     Code = "code"
+    Directory = "directory"
 
     def pluralize(self) -> str:
         if self is self.Analysis:
             return "analyses"
         return f"{self.value}s"
 
 
@@ -94,14 +95,22 @@
             f"{self.operation.value.capitalize()} {self.entity_type.value} "
             f"`{self.source_name + '.' if self.source_name else ''}{self.identifier}` "
             f"{prepositions[self.operation]} {self.path.relative_to(os.getcwd())}"
         )
 
 
 @dataclasses.dataclass
+class DirectoryChange(BaseChange):
+    """A DirectoryChange represents a unit of work that should be performed on a Directory in a dbt project."""
+
+    source: Optional[Path] = None
+    ignore_function: Optional[Callable] = None
+
+
+@dataclasses.dataclass
 class FileChange(BaseChange):
     """A FileChange represents a unit of work that should be performed on a File in a dbt project."""
 
     data: Optional[str] = None
     source: Optional[Path] = None
```

### Comparing `dbt_meshify-0.5.3/dbt_meshify/change_set_processor.py` & `dbt_meshify-0.5.4/dbt_meshify/change_set_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from itertools import chain
 from typing import Iterable
 
 from loguru import logger
 
 from dbt_meshify.change import Change, ChangeSet, EntityType
-from dbt_meshify.storage.file_content_editors import RawFileEditor, ResourceFileEditor
+from dbt_meshify.storage.file_content_editors import (
+    DirectoryEditor,
+    RawFileEditor,
+    ResourceFileEditor,
+)
+
+# Enumeration of valid File Editors
+FILE_EDITORS = {EntityType.Code: RawFileEditor, EntityType.Directory: DirectoryEditor}
 
 
 class ChangeSetProcessorException(BaseException):
     def __init__(self, change: Change, exception: BaseException) -> None:
         self.change = change
         self.exception = exception
         super().__init__(f"Error processing change {self.change}")
@@ -20,17 +27,15 @@
     """
 
     def __init__(self, dry_run: bool = False) -> None:
         self.__dry_run = dry_run
 
     def write(self, change: Change) -> None:
         """Commit a Change to the file system."""
-        file_editor = (
-            RawFileEditor() if change.entity_type == EntityType.Code else ResourceFileEditor()
-        )
+        file_editor = FILE_EDITORS.get(change.entity_type, ResourceFileEditor)()
 
         file_editor.__getattribute__(change.operation)(change)
 
     def process(self, change_sets: Iterable[ChangeSet]) -> None:
         """
         Process an iterable of ChangeSets. This is the mechanism by which file modifications
         are orchestrated.
```

### Comparing `dbt_meshify-0.5.3/dbt_meshify/cli.py` & `dbt_meshify-0.5.4/dbt_meshify/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,15 +103,22 @@
     help="Skips the dbt docs generate step and reads the local catalog.json file.",
 )
 
 latest = click.option(
     "--latest",
     "-l",
     is_flag=True,
-    help="Makes the newest version the latest version when incrementing model versions",
+    help="Makes the newest version the latest version when creating model versions",
+)
+
+increment = click.option(
+    "--increment",
+    "--i",
+    is_flag=True,
+    help="Increments the latest_version setting by 1 when creating model versions",
 )
 
 
 def owner(func):
     """Add click options and argument validation for creating Owner objects."""
 
     @functools.wraps(func)
```

### Comparing `dbt_meshify-0.5.3/dbt_meshify/dbt.py` & `dbt_meshify-0.5.4/dbt_meshify/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_meshify-0.5.3/dbt_meshify/dbt_projects.py` & `dbt_meshify-0.5.4/dbt_meshify/dbt_projects.py`

 * *Files identical despite different names*

### Comparing `dbt_meshify-0.5.3/dbt_meshify/exceptions.py` & `dbt_meshify-0.5.4/dbt_meshify/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_meshify-0.5.3/dbt_meshify/main.py` & `dbt_meshify-0.5.4/dbt_meshify/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 from dbt_meshify.change_set_processor import (
     ChangeSetProcessor,
     ChangeSetProcessorException,
 )
 from dbt_meshify.storage.dbt_project_editors import DbtSubprojectCreator
 from dbt_meshify.utilities.contractor import Contractor
 from dbt_meshify.utilities.linker import Linker
-from dbt_meshify.utilities.versioner import ModelVersioner
+from dbt_meshify.utilities.versioner import LatestVersionBehavior, ModelVersioner
 
 from .cli import (
     TupleCompatibleCommand,
     create_path,
     exclude,
     exclude_projects,
     get_version,
     group_yml_path,
+    increment,
     latest,
     owner,
     owner_email,
     owner_name,
     owner_properties,
     project_path,
     project_paths,
@@ -369,27 +370,41 @@
 @operation.command(name="bump-version")
 @exclude
 @project_path
 @read_catalog
 @select
 @selector
 @latest
+@increment
 @click.option("--defined-in", default=None)
 def bump_version(
     select,
     exclude,
     project_path,
     selector,
     latest: bool,
+    increment: bool,
     defined_in: Optional[Path],
     read_catalog,
 ) -> List[ChangeSet]:
     """
     Create new model versions for all selected models.
     """
+
+    if latest and increment:
+        raise FatalMeshifyException(
+            "Cannot specify both --latest and --increment. Please choose one or the other."
+        )
+
+    latest_version_behavior = LatestVersionBehavior.Prerelease
+    if latest:
+        latest_version_behavior = LatestVersionBehavior.Latest
+    elif increment:
+        latest_version_behavior = LatestVersionBehavior.Increment
+
     path = Path(project_path).expanduser().resolve()
 
     logger.info(f"Reading dbt project at {path}")
     project = DbtProject.from_directory(path, read_catalog)
     resources = list(
         project.select_resources(
             select=select, exclude=exclude, selector=selector, output_key="unique_id"
@@ -408,15 +423,17 @@
             if not isinstance(model_node, ModelNode):
                 continue
 
             if model_node.version != model_node.latest_version:
                 continue
 
             changes: ChangeSet = versioner.bump_version(
-                model=model_node, prerelease=not (latest), defined_in=defined_in
+                model=model_node,
+                latest_version_behavior=latest_version_behavior,
+                defined_in=defined_in,
             )
             change_set.extend(changes)
 
         except Exception as e:
             raise FatalMeshifyException(f"Error adding version to model: {model_unique_id}. {e}")
 
     return [change_set]
@@ -425,27 +442,40 @@
 @cli.command(name="version")
 @exclude
 @project_path
 @read_catalog
 @select
 @selector
 @latest
+@increment
 @click.option("--defined-in", default=None)
 def version(
     select,
     exclude,
     project_path,
     selector,
     latest: bool,
+    increment: bool,
     defined_in: Optional[Path],
     read_catalog,
 ) -> List[ChangeSet]:
     """
     Increment the models to the next version, and create in the initial version if it has not yet been defined.
     """
+    if latest and increment:
+        raise FatalMeshifyException(
+            "Cannot specify both --latest and --increment. Please choose one or the other."
+        )
+
+    latest_version_behavior = LatestVersionBehavior.Prerelease
+    if latest:
+        latest_version_behavior = LatestVersionBehavior.Latest
+    elif increment:
+        latest_version_behavior = LatestVersionBehavior.Increment
+
     path = Path(project_path).expanduser().resolve()
 
     logger.info(f"Reading dbt project at {path}")
     project = DbtProject.from_directory(path, read_catalog)
     resources = list(
         project.select_resources(
             select=select, exclude=exclude, selector=selector, output_key="unique_id"
@@ -470,15 +500,15 @@
             if model_node.latest_version is not None:
                 # We already have a version. Simply bump
 
                 change_set.extend(
                     versioner.bump_version(
                         model=model_node,
                         defined_in=defined_in,
-                        prerelease=not (latest),
+                        latest_version_behavior=latest_version_behavior,
                     )
                 )
 
             else:
                 # We don't have a version! This means we have to both add versions to the model, and then bump it!
 
                 add_changes: ChangeSet = versioner.add_version(
@@ -494,15 +524,15 @@
                     raise FatalMeshifyException(
                         f"Fault in change calculations for model {model_unique_id}"
                     )
 
                 bump_change: ChangeSet = versioner.bump_version(
                     model=model_node,
                     defined_in=defined_in,
-                    prerelease=not (latest),
+                    latest_version_behavior=latest_version_behavior,
                     model_override=model_add_change.data,
                 )
 
                 # Update the bump change for the model copy to reference the new model path
                 file_bump_change = bump_change[1]
                 if not isinstance(file_bump_change, FileChange):
                     raise FatalMeshifyException(
```

### Comparing `dbt_meshify-0.5.3/dbt_meshify/storage/dbt_project_editors.py` & `dbt_meshify-0.5.4/dbt_meshify/storage/dbt_project_editors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+import shutil
 from pathlib import Path
+from tracemalloc import start
 from typing import Dict, Optional, Set
 
 from dbt.contracts.graph.nodes import (
     CompiledNode,
     GenericTestNode,
     Macro,
     ModelNode,
     NodeType,
     Resource,
     SnapshotNode,
 )
 from dbt.node_types import AccessType
 from loguru import logger
+from regex import D
 
 from dbt_meshify.change import (
     ChangeSet,
+    DirectoryChange,
     EntityType,
     FileChange,
     Operation,
     ResourceChange,
 )
 from dbt_meshify.dbt_projects import DbtSubProject
 from dbt_meshify.storage.file_content_editors import NamedList, filter_empty_dict_items
@@ -26,14 +30,28 @@
 from dbt_meshify.storage.jinja_blocks import JinjaBlock
 from dbt_meshify.utilities.contractor import Contractor
 from dbt_meshify.utilities.dependencies import DependenciesUpdater
 from dbt_meshify.utilities.grouper import ResourceGrouper
 from dbt_meshify.utilities.references import ReferenceUpdater
 
 
+def get_starter_project_path() -> Path:
+    """Obtain the path of a dbt starter project on the local filesystem."""
+
+    from importlib import resources
+
+    import dbt.include.starter_project
+
+    starter_path = Path(str(resources.files(dbt.include.starter_project)))
+    assert starter_path is not None
+    assert (starter_path / "dbt_project.yml").exists()
+
+    return starter_path
+
+
 class DbtSubprojectCreator:
     """
     Takes a `DbtSubProject` and creates the directory structure and files for it.
     """
 
     def __init__(
         self,
@@ -81,40 +99,65 @@
             filter(
                 lambda x: (x.startswith("model") and x.split(".")[1] == parent_project_name),
                 interface,
             )
         )
         return boundary_models
 
+    def create_starter_project(self) -> DirectoryChange:
+        """Create a new starter project using the default stored in dbt-core"""
+
+        return DirectoryChange(
+            operation=Operation.Copy,
+            entity_type=EntityType.Directory,
+            identifier=str(self.subproject.path),
+            path=self.subproject.path,
+            source=get_starter_project_path(),
+            ignore_function=shutil.ignore_patterns("__init__.py", "__pycache__", "**/*.pyc"),
+        )
+
     def write_project_file(self) -> FileChange:
         """
         Writes the dbt_project.yml file for the subproject in the specified subdirectory
         """
+
+        # Read a starter `dbt_project.yml` file as a baseline
+        starter_path: Path = get_starter_project_path() / "dbt_project.yml"
+        starter_dbt_project = YAMLFileManager.read_file(starter_path)
+
         contents = self.subproject.project.to_dict()
-        # was getting a weird serialization error from ruamel on this value
-        # it's been deprecated, so no reason to keep it
-        contents.pop("version")
+
         # this one appears in the project yml, but i don't think it should be written
         contents.pop("query-comment")
         contents = filter_empty_dict_items(contents)
 
         # Serialize the `require-dbt-version` field into a string. This happens because dbt is expecting a list of
         # strings, but also accepts a singular string value, too. We can handle the latter case by checking the length
         # of each item in the list. If they're all one character long, then we're really working with a single version
         # string.
         if "require-dbt-version" in contents:
             if max([len(version) for version in contents["require-dbt-version"]]) == 1:
                 contents["require-dbt-version"] = "".join(contents["require-dbt-version"])
 
+        for key, value in contents.items():
+            if value is None:
+                continue
+
+            if isinstance(value, (list, dict, tuple)):
+                if len(value) == 0:
+                    continue
+
+            starter_dbt_project[key] = value
+
         return FileChange(
             operation=Operation.Add,
             entity_type=EntityType.Code,
             identifier="dbt_project.yml",
             path=self.subproject.path / Path("dbt_project.yml"),
-            data=yaml.dump(contents),
+            data=yaml.dump(starter_dbt_project),
         )
 
     def copy_packages_yml_file(self) -> FileChange:
         """
         Writes the dbt_project.yml file for the subproject in the specified subdirectory
         """
         return FileChange(
@@ -139,14 +182,16 @@
         parent_contractor = Contractor(project=subproject.parent_project)
         parent_resource_grouper = ResourceGrouper(project=subproject.parent_project)
 
         logger.info(
             f"Identifying operations required to split {subproject.name} from {subproject.parent_project.name}."
         )
 
+        change_set.add(self.create_starter_project())
+
         for unique_id in (
             subproject.resources
             | subproject.custom_macros
             | subproject.groups
             | subproject.referenced_docs
         ):
             resource = subproject.get_manifest_node(unique_id)
```

### Comparing `dbt_meshify-0.5.3/dbt_meshify/storage/file_content_editors.py` & `dbt_meshify-0.5.4/dbt_meshify/storage/file_content_editors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import Any, Dict, List, Optional
 
 from loguru import logger
 
-from dbt_meshify.change import EntityType, FileChange, ResourceChange
+from dbt_meshify.change import DirectoryChange, EntityType, FileChange, ResourceChange
 from dbt_meshify.exceptions import FileEditorException
-from dbt_meshify.storage.file_manager import RawFileManager, YAMLFileManager
+from dbt_meshify.storage.file_manager import (
+    DirectoryManager,
+    RawFileManager,
+    YAMLFileManager,
+)
 
 
 class NamedList(dict):
     """An NamedList is a Dict generated from a list with an indexable value."""
 
     def __init__(self, source_list: Optional[List[Dict]] = None, index_field: str = "name"):
         self.index_field = index_field
@@ -85,14 +89,26 @@
         elif value is None and key in original:
             del original[key]
         elif value is not None:
             original[key] = value
     return original
 
 
+class DirectoryEditor:
+    """A helper class used to perform filesystem operations on Directories"""
+
+    @staticmethod
+    def copy(change: DirectoryChange):
+        """Copy a file from one location to another."""
+        if change.source is None:
+            raise FileEditorException("None source value provided in Copy operation.")
+
+        DirectoryManager.copy_directory(change.source, change.path, change.ignore_function)
+
+
 class RawFileEditor:
     """A class used to perform Raw operations on Files"""
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     @staticmethod
```

### Comparing `dbt_meshify-0.5.3/dbt_meshify/storage/file_manager.py` & `dbt_meshify-0.5.4/dbt_meshify/storage/file_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # classes that deal specifically with file manipulation
 # of dbt files to be used in the meshify dbt project
 
 import shutil
 from pathlib import Path
-from typing import Any, Dict, List, Protocol
+from typing import Any, Callable, Dict, List, Optional, Protocol
 
 from dbt.contracts.util import Identifier
 from ruamel.yaml import YAML
 from ruamel.yaml.compat import StringIO
 
 
 class DbtYAML(YAML):
     """dbt-compatible YAML class."""
 
     def __init__(self):
         super().__init__()
         self.preserve_quotes = True
         self.width = 4096
         self.indent(mapping=2, sequence=4, offset=2)
+        self.default_flow_style = False
 
     def dump(self, data, stream=None, **kw):
         inefficient = False
         if stream is None:
             inefficient = True
             stream = StringIO()
         super().dump(data, stream, **kw)
@@ -39,14 +40,29 @@
         pass
 
     def write_file(self, path: Path, content: Any) -> None:
         """Write content to a file."""
         pass
 
 
+class DirectoryManager:
+    """DirectoryManager is a FileManager for operating on directories in the filesystem"""
+
+    @staticmethod
+    def copy_directory(
+        source_path: Path, target_path: Path, ignore_function: Optional[Callable] = None
+    ) -> None:
+        """Copy a directory from source to target"""
+
+        if not target_path.parent.exists():
+            target_path.parent.mkdir(parents=True, exist_ok=True)
+
+        shutil.copytree(source_path, target_path, symlinks=True, ignore=ignore_function)
+
+
 class RawFileManager:
     """RawFileManager is a FileManager for operating on raw files in the filesystem."""
 
     @staticmethod
     def read_file(path: Path) -> str:
         """Read a file from the filesystem and return a string value."""
         return path.read_text()
```

### Comparing `dbt_meshify-0.5.3/dbt_meshify/storage/jinja_blocks.py` & `dbt_meshify-0.5.4/dbt_meshify/storage/jinja_blocks.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,27 +20,27 @@
     @staticmethod
     def find_block_range(file_content: str, block_type: str, name: str) -> Tuple[int, int]:
         """Find the line number that a block started."""
         start_line = None
         end_line = None
 
         for match in re.finditer(
-            r"{%-?\s+" + block_type + r"\s+" + name + r"([(a-zA-Z0-9=,_ )]*)\s-?%}",
+            r"{%-?\s*" + block_type + r"\s*" + name + r"\s*([(a-zA-Z0-9=,_ \'\")]*)\s*-?%}",
             file_content,
             re.MULTILINE,
         ):
             start = match.span()[0]  # .span() gives tuple (start, end)
             start_line = start  # file_content[:start].count("\n")
             break
 
         if start_line is None:
             raise Exception(f"Unable to find a {block_type} block with the name {name}.")
 
         for match in re.finditer(
-            r"{%-?\s+end" + block_type + r"\s+-?%}", file_content, re.MULTILINE
+            r"{%-?\s*end" + block_type + r"\s*-?%}", file_content, re.MULTILINE
         ):
             end = match.span()[1]  # .span() gives tuple (start, end)
             new_end_line = end  # file_content[:start].count("\n")
 
             if new_end_line >= start_line:
                 end_line = new_end_line
                 break
```

### Comparing `dbt_meshify-0.5.3/dbt_meshify/utilities/contractor.py` & `dbt_meshify-0.5.4/dbt_meshify/utilities/contractor.py`

 * *Files identical despite different names*

### Comparing `dbt_meshify-0.5.3/dbt_meshify/utilities/dependencies.py` & `dbt_meshify-0.5.4/dbt_meshify/utilities/dependencies.py`

 * *Files identical despite different names*

### Comparing `dbt_meshify-0.5.3/dbt_meshify/utilities/grouper.py` & `dbt_meshify-0.5.4/dbt_meshify/utilities/grouper.py`

 * *Files identical despite different names*

### Comparing `dbt_meshify-0.5.3/dbt_meshify/utilities/linker.py` & `dbt_meshify-0.5.4/dbt_meshify/utilities/linker.py`

 * *Files identical despite different names*

### Comparing `dbt_meshify-0.5.3/dbt_meshify/utilities/references.py` & `dbt_meshify-0.5.4/dbt_meshify/utilities/references.py`

 * *Files identical despite different names*

### Comparing `dbt_meshify-0.5.3/dbt_meshify/utilities/versioner.py` & `dbt_meshify-0.5.4/dbt_meshify/utilities/versioner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 from dbt.contracts.graph.nodes import ModelNode
 from loguru import logger
 
 from dbt_meshify.change import (
@@ -12,14 +13,22 @@
     ResourceChange,
 )
 from dbt_meshify.dbt_projects import DbtProject, DbtSubProject
 from dbt_meshify.storage.file_content_editors import NamedList, safe_update
 from dbt_meshify.storage.file_manager import FileManager, YAMLFileManager
 
 
+class LatestVersionBehavior(str, Enum):
+    """The type of behavior applied to `latest_version` when updating model versions"""
+
+    Prerelease = "prerelease"
+    Increment = "increment"
+    Latest = "latest"
+
+
 class ModelVersionerException(Exception):
     """Exceptions raised during versioning of a Model."""
 
 
 class ModelVersioner:
     """Class for creating and incrementing version Changes on Models."""
 
@@ -123,15 +132,15 @@
         )
 
         return change_set
 
     def bump_version(
         self,
         model: ModelNode,
-        prerelease: bool = False,
+        latest_version_behavior: LatestVersionBehavior = LatestVersionBehavior.Prerelease,
         defined_in: Optional[Path] = None,
         model_override: Optional[Dict] = None,
     ) -> ChangeSet:
         """Increment a model's version, and create a new version definition and model file for the new version number"""
 
         path = self.project.resolve_patch_path(model)
         model_path = self.project.path / model.original_file_path
@@ -145,20 +154,28 @@
 
         if len(model_versions) == 0:
             raise ModelVersionerException(
                 f"The model {model.name} does not have any versions defined. Please use add-version first."
             )
 
         # Within dbt-core, if unset `latest_version` defaults to the greatest version identifier.
-        latest_version = model_yml.get("latest_version", greatest_version)
-
-        # Bump versions
+        current_latest_version = model_yml.get("latest_version", greatest_version)
         new_greatest_version_number = greatest_version + 1
-        new_latest_version_number = latest_version if prerelease else latest_version + 1
 
+        # if prerelease, the latest version is unchanged
+        # if increment, the latest version is incremented by 1
+        # if latest, the latest version is set to the greatest version + 1 (newly created version)
+
+        latest_version_number_map = {
+            LatestVersionBehavior.Prerelease: current_latest_version,
+            LatestVersionBehavior.Increment: current_latest_version + 1,
+            LatestVersionBehavior.Latest: greatest_version + 1,
+        }
+
+        new_latest_version_number = latest_version_number_map[latest_version_behavior]
         # Setup the new version definitions
         new_version_data: Dict[str, Any] = {"v": new_greatest_version_number}
         if defined_in:
             new_version_data["defined_in"] = defined_in
         model_versions[new_version_data["v"]] = new_version_data
 
         # Determine the file name for the versioned model
```

### Comparing `dbt_meshify-0.5.3/pyproject.toml` & `dbt_meshify-0.5.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [tool.ruff]
 # Allow lines to be as long as 120 characters.
 line-length = 120
 
 [tool.poetry]
 name = "dbt-meshify"
-version = "0.5.3"
+version = "0.5.4"
 description = "a package to upgrade dbt packages to the dbt mesh framework"
 authors = [
     "Dave Connors <dave.connors@fishtownanalytics.com>",
     "Grace Goheen <grace.goheen@dbtlabs.com>",
     "Nicholas Yager <yager@nicholasyager.com>",
 ]
 license = "Apache 2.0"
```

### Comparing `dbt_meshify-0.5.3/PKG-INFO` & `dbt_meshify-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-meshify
-Version: 0.5.3
+Version: 0.5.4
 Summary: a package to upgrade dbt packages to the dbt mesh framework
 License: Apache 2.0
 Author: Dave Connors
 Author-email: dave.connors@fishtownanalytics.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

