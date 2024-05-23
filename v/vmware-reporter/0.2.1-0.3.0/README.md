# Comparing `tmp/vmware_reporter-0.2.1-py3-none-any.whl.zip` & `tmp/vmware_reporter-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 30911 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat    17494 b- defN 24-May-20 09:08 vmware_reporter/__init__.py
--rw-rw-rw-  2.0 fat     3302 b- defN 24-May-20 09:08 vmware_reporter/__main__.py
--rw-rw-rw-  2.0 fat      427 b- defN 24-May-20 15:39 vmware_reporter/_version.py
--rw-rw-rw-  2.0 fat    17592 b- defN 24-May-20 09:08 vmware_reporter/datastore.py
--rw-rw-rw-  2.0 fat     2482 b- defN 24-May-20 09:08 vmware_reporter/dump.py
--rw-rw-rw-  2.0 fat     5265 b- defN 24-May-20 09:08 vmware_reporter/extract.py
--rw-rw-rw-  2.0 fat     8916 b- defN 24-May-20 09:08 vmware_reporter/inspect.py
--rw-rw-rw-  2.0 fat     7900 b- defN 24-May-20 09:08 vmware_reporter/inventory.py
--rw-rw-rw-  2.0 fat     5129 b- defN 24-May-20 09:08 vmware_reporter/networking.py
--rw-rw-rw-  2.0 fat    31721 b- defN 24-May-20 09:08 vmware_reporter/vm.py
--rw-rw-rw-  2.0 fat      705 b- defN 24-Mar-22 23:30 vmware_reporter/config/extractions/host.yml
--rw-rw-rw-  2.0 fat     1467 b- defN 24-Mar-22 23:30 vmware_reporter/config/extractions/vm.yml
--rw-rw-rw-  2.0 fat     1098 b- defN 24-May-20 15:39 vmware_reporter-0.2.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2602 b- defN 24-May-20 15:39 vmware_reporter-0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-20 15:39 vmware_reporter-0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       66 b- defN 24-May-20 15:39 vmware_reporter-0.2.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       16 b- defN 24-May-20 15:39 vmware_reporter-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1564 b- defN 24-May-20 15:39 vmware_reporter-0.2.1.dist-info/RECORD
-18 files, 107838 bytes uncompressed, 28327 bytes compressed:  73.7%
+Zip file size: 36666 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat    31153 b- defN 24-May-23 17:26 vmware_reporter/__init__.py
+-rw-rw-rw-  2.0 fat     3466 b- defN 24-May-23 10:33 vmware_reporter/__main__.py
+-rw-rw-rw-  2.0 fat      427 b- defN 24-May-23 17:27 vmware_reporter/_version.py
+-rw-rw-rw-  2.0 fat     1447 b- defN 24-May-23 15:52 vmware_reporter/autoreport.py
+-rw-rw-rw-  2.0 fat      844 b- defN 24-May-23 12:13 vmware_reporter/customfield.py
+-rw-rw-rw-  2.0 fat    18826 b- defN 24-May-23 17:23 vmware_reporter/datastore.py
+-rw-rw-rw-  2.0 fat     2547 b- defN 24-May-23 17:25 vmware_reporter/dump.py
+-rw-rw-rw-  2.0 fat     4034 b- defN 24-May-23 16:52 vmware_reporter/host.py
+-rw-rw-rw-  2.0 fat     7968 b- defN 24-May-23 17:24 vmware_reporter/inventory.py
+-rw-rw-rw-  2.0 fat     5971 b- defN 24-May-23 12:16 vmware_reporter/net.py
+-rw-rw-rw-  2.0 fat      235 b- defN 24-May-23 11:12 vmware_reporter/settings.py
+-rw-rw-rw-  2.0 fat    54717 b- defN 24-May-23 12:24 vmware_reporter/vm.py
+-rw-rw-rw-  2.0 fat     1098 b- defN 24-May-23 17:27 vmware_reporter-0.3.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     3435 b- defN 24-May-23 17:27 vmware_reporter-0.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 17:27 vmware_reporter-0.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       66 b- defN 24-May-23 17:27 vmware_reporter-0.3.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       16 b- defN 24-May-23 17:27 vmware_reporter-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1529 b- defN 24-May-23 17:27 vmware_reporter-0.3.0.dist-info/RECORD
+18 files, 137871 bytes uncompressed, 34150 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -3,53 +3,53 @@
 
 Filename: vmware_reporter/__main__.py
 Comment: 
 
 Filename: vmware_reporter/_version.py
 Comment: 
 
-Filename: vmware_reporter/datastore.py
+Filename: vmware_reporter/autoreport.py
 Comment: 
 
-Filename: vmware_reporter/dump.py
+Filename: vmware_reporter/customfield.py
 Comment: 
 
-Filename: vmware_reporter/extract.py
+Filename: vmware_reporter/datastore.py
 Comment: 
 
-Filename: vmware_reporter/inspect.py
+Filename: vmware_reporter/dump.py
 Comment: 
 
-Filename: vmware_reporter/inventory.py
+Filename: vmware_reporter/host.py
 Comment: 
 
-Filename: vmware_reporter/networking.py
+Filename: vmware_reporter/inventory.py
 Comment: 
 
-Filename: vmware_reporter/vm.py
+Filename: vmware_reporter/net.py
 Comment: 
 
-Filename: vmware_reporter/config/extractions/host.yml
+Filename: vmware_reporter/settings.py
 Comment: 
 
-Filename: vmware_reporter/config/extractions/vm.yml
+Filename: vmware_reporter/vm.py
 Comment: 
 
-Filename: vmware_reporter-0.2.1.dist-info/LICENSE.txt
+Filename: vmware_reporter-0.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vmware_reporter-0.2.1.dist-info/METADATA
+Filename: vmware_reporter-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: vmware_reporter-0.2.1.dist-info/WHEEL
+Filename: vmware_reporter-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: vmware_reporter-0.2.1.dist-info/entry_points.txt
+Filename: vmware_reporter-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: vmware_reporter-0.2.1.dist-info/top_level.txt
+Filename: vmware_reporter-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: vmware_reporter-0.2.1.dist-info/RECORD
+Filename: vmware_reporter-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vmware_reporter/__init__.py

```diff
@@ -1,36 +1,47 @@
+"""
+Top-level API of vmware-reporter library.
+"""
 from __future__ import annotations
 
+import json
 import logging
+import os
 import re
 from collections.abc import Callable, Iterator
 from configparser import ConfigParser
+from contextlib import nullcontext
+from datetime import date
 from inspect import signature
+from io import IOBase
 from pathlib import Path
-from typing import Literal, TypeVar, overload
+from types import (BuiltinFunctionType, BuiltinMethodType, FunctionType,
+                   MethodType)
+from typing import Any, Literal, TypeVar, overload
 from uuid import UUID
 
 from pyVim.connect import Disconnect, SmartConnect
 from pyVmomi import vim, vmodl
 from pyVmomi.VmomiSupport import _managedDefMap
-from zut import Filters, MessageError, get_config, resolve_host
+from zut import (ExtendedJSONEncoder, Filters, MessageError,
+                 iter_dicts_from_csv, resolve_host)
+from zut.excel import ExcelWorkbook, is_excel_path, split_excel_path
 
-import vmware_reporter
-
-from .inspect import get_obj_ref
+from .settings import CONFIG, CONFIG_SECTION
 
 __prog__ = 'vmware-reporter'
 
 try:
     # Version generated by setuptools_scm during build
     from ._version import __version__, __version_tuple__
 except ImportError:
     __version__ = None
     __version_tuple__ = None
 
+_logger = logging.getLogger(__name__)
 
 T_Obj = TypeVar('T_Obj', bound=vim.ManagedEntity)
 
 
 class VCenterClient:
     """
     Main entry point of the library to retrieve VMWare managed objects and interact with them. 
@@ -44,17 +55,17 @@
 
         :param env: An optional name to distinguish between several vCenters.
         :param host: Host name of the vCenter.
         :param user: Name of the vCenter user having access to the API.
         :param password: Password of the vCenter user having access to the API.
         """        
         if not config:
-            config = get_config(vmware_reporter)
+            config = CONFIG
         if not section:
-            section = __prog__
+            section = CONFIG_SECTION
         
         if not env:
             envs = VCenterClient.get_configured_envs(config=config, section=section)
             if len(envs) > 1:
                 raise MessageError(f"Name of the environment / VCenter to use must be provided. Available: {', '.join(envs) if envs else 'none'}.")
             elif len(envs) == 1:
                 env = envs[0]
@@ -206,18 +217,18 @@
         for datacenter in self.iter_objs(vim.Datacenter):
             obj = self.service_content.searchIndex.FindByUuid(datacenter, uuid, vmSearch=for_vm, instanceUuid=instance_uuid)
             if obj:
                 return obj
 
 
     @overload
-    def get_objs(self, types: type[T_Obj], search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name', sort_key: str|list[str]|Callable = None) -> list[T_Obj]:
+    def get_objs(self, types: type[T_Obj], search: list[str|Path|re.Pattern]|str|Path|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name', sort_key: str|list[str]|Callable = None) -> list[T_Obj]:
         ...
 
-    def get_objs(self, types: list[type|str]|type|str = None, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name', sort_key: str|list[str]|Callable = None):        
+    def get_objs(self, types: list[type|str]|type|str = None, search: list[str|Path|re.Pattern]|str|Path|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name', sort_key: str|list[str]|Callable = None):        
         """
         List VMWare managed objects matching the given search.
         """
         objs = [obj for obj in self.iter_objs(types, search, normalize=normalize, key=key)]
 
         if sort_key:
             if isinstance(sort_key, str):
@@ -230,21 +241,23 @@
 
             objs.sort(key=sort_func)
 
         return objs
 
 
     @overload
-    def iter_objs(self, types: type[T_Obj], search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name') -> Iterator[T_Obj]:
+    def iter_objs(self, types: type[T_Obj], search: list[str|Path|re.Pattern]|str|Path|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name') -> Iterator[T_Obj]:
         ...
 
-    def iter_objs(self, types: list[type|str]|type|str = None, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name'):
+    def iter_objs(self, types: list[type|str]|type|str = None, search: list[str|Path|re.Pattern]|str|Path|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name'):
         """
         Iterate over VMWare managed objects matching the given search.
         """
+        # Expand search from CSV or Excel files if search ends with '.csv' or '.xlsx'
+        search = _expand_search_from_files(search, key=key)
 
         # Prepare value filter
         filters = Filters(search, normalize=normalize)
 
         # Prepare types
         if not types:
             types = []
@@ -308,72 +321,103 @@
 
         # Make a cookie
         self._cookie = dict()
         self._cookie[cookie_name] = cookie_text
         return self._cookie
 
 
-    def wait_for_task(self, *tasks: vim.Task):
+    def wait_for_task(self, tasks: vim.Task|list[vim.Task]|dict[vim.Task,Any]):
         """
         Given a service instance and tasks, return after all the tasks are complete.
+        - `tasks`: a task, a list of tasks, or a dict associating task to log prefixes.
         """
-        property_collector = self.service_instance.content.propertyCollector
-        task_list = [str(task) for task in tasks]
+        task_list: list[vim.Task] = []
+        log_prefixes: dict[vim.Task,Any] = {}
+        if isinstance(tasks, dict):
+            log_prefixes = tasks
+            for task in tasks.keys():
+                if not isinstance(task, vim.Task):
+                    raise TypeError(f"Invalid dict key: {task} (type {type(task).__name__}, expected vim.Task)")
+                task_list.append(task)
+        elif isinstance(tasks, list):
+            for task in tasks:
+                if not isinstance(task, vim.Task):
+                    raise TypeError(f"Invalid list element: {task} (type {type(task).__name__}, expected vim.Task)")
+                task_list.append(task)
+        elif isinstance(tasks, vim.Task):
+            task_list.append(tasks)
+        else:
+            raise TypeError(f"Invalid argument: {task} (type {type(task).__name__}, expected vim.Task)")
+        
         # Create filter
-        obj_specs = [vmodl.query.PropertyCollector.ObjectSpec(obj=task) for task in tasks]
+        obj_specs = [vmodl.query.PropertyCollector.ObjectSpec(obj=task) for task in task_list]   
         property_spec = vmodl.query.PropertyCollector.PropertySpec(type=vim.Task, pathSet=[], all=True)
-        filter_spec = vmodl.query.PropertyCollector.FilterSpec()
-        filter_spec.objectSet = obj_specs
-        filter_spec.propSet = [property_spec]
-        pc_filter = property_collector.CreateFilter(filter_spec, True)
+        filter_spec = vmodl.query.PropertyCollector.FilterSpec(objectSet=obj_specs, propSet=[property_spec])
+        pc = self.service_instance.content.propertyCollector
+        pc_filter = pc.CreateFilter(filter_spec, True)
+
+        task_failures = 0
         try:
-            version, state = None, None
+            remaining_task_strs = [str(task) for task in task_list]
+            version = None
+            state = None
             # Loop looking for updates till the state moves to a completed state.
-            while task_list:
-                update = property_collector.WaitForUpdates(version)
+            # (tasks are removed from task_list one by one when they reach a completed)
+            while remaining_task_strs:
+                update = pc.WaitForUpdates(version)
                 for filter_set in update.filterSet:
                     for obj_set in filter_set.objectSet:
-                        task = obj_set.obj
+                        task: vim.Task = obj_set.obj
                         for change in obj_set.changeSet:
                             if change.name == 'info':
                                 state = change.val.state
                             elif change.name == 'info.state':
                                 state = change.val
                             else:
                                 continue
 
-                            if not str(task) in task_list:
+                            if not str(task) in remaining_task_strs:
                                 continue
 
                             if state == vim.TaskInfo.State.success:
-                                # Remove task from taskList
-                                task_list.remove(str(task))
+                                remaining_task_strs.remove(str(task))
+                                if log_prefix := log_prefixes.get(task):
+                                    self.logger.info(f"{log_prefix}: success")
                             elif state == vim.TaskInfo.State.error:
-                                raise task.info.error
+                                if len(task_list) > 1:
+                                    remaining_task_strs.remove(str(task))
+                                    log_prefix = log_prefixes.get(task)
+                                    self.logger.error(f"{f'{log_prefix}: ' if log_prefix else ''}{task.info.error}", exc_info=task.info.error)
+                                    task_failures += 1
+                                else:
+                                    raise task.info.error
                 # Move to next version
                 version = update.version
         finally:
             if pc_filter:
                 pc_filter.Destroy()
 
+        if task_failures > 0:
+            raise MessageError(f"{task_failures} task{'s' if task_failures > 1 else ''} failed (see previous logs)")
 
+ 
     def get_out_dir(self):
         return Path('data' if self.env == 'default' else f'data/{self.env}')
 
     #endregion
 
 
     #region Class helpers
     
     @classmethod
     def get_configured_envs(cls, *, config: ConfigParser = None, section: str = None):
         if not config:
-            config = get_config(vmware_reporter)
+            config = CONFIG
         if not section:
-            section = __prog__
+            section = CONFIG_SECTION
         
         envs: list[str] = []
         for _section in config.sections():
             if m := re.match(r'^' + re.escape(section) + r'(?:\:(.+))?', _section):
                 env = m[1]
                 if env == 'default':
                     raise ValueError(f"Invalid configuration section \"{_section}\": name \"default\" is reserved")
@@ -478,12 +522,337 @@
             for obj in self.iter_objs(vim.DistributedVirtualSwitch):
                 by_uuid[obj.uuid] = obj
             self._switchs_by_uuid = by_uuid
 
         return by_uuid.get(uuid)
 
     #endregion
+    
+
+def _expand_search_from_files(search: list[str|Path|re.Pattern]|str|Path|re.Pattern|None, *, key: Literal['name', 'ref'] = 'name') -> list[str|re.Pattern]|None:
+    """
+    Expand search from CSV or Excel files if search ends with '.csv' or '.xlsx'.
+    """
+    if search is None:
+        return None
+    elif isinstance(search, (str,Path,re.Pattern)):
+        search = [search]
+    
+    def expand_from_xlsx_file(path: Path, table_name: str = None):
+        workbook = ExcelWorkbook(path)
+        table = workbook.get_table(table_name)
+        if not key in table.column_names:
+            raise ValueError(f"Column \"{key}\" not found in {path}")
+        for row in table:
+            if row[key]:
+                yield row[key]
+
+    def expand_from_csv_file(path: Path):
+        for row in iter_dicts_from_csv(path):
+            if not key in row:
+                raise ValueError(f"Column \"{key}\" not found in {path}")
+            if row[key]:
+                yield row[key]
+    
+    result = []
+    for elem in search:
+        if isinstance(elem, Path):
+            if elem.suffix.lower() == '.xlsx':
+                for file_elem in expand_from_xlsx_file(elem):
+                    result.append(file_elem)
+            elif elem.suffix.lower() == '.csv':
+                for file_elem in expand_from_csv_file(elem):
+                    result.append(file_elem)
+            else:
+                raise ValueError(f"Invalid search path extension: {elem}")
+        elif isinstance(elem, str):
+            if is_excel_path(elem, accept_table_suffix=True):
+                path, table_name = split_excel_path(elem)
+                for file_elem in expand_from_xlsx_file(path, table_name):
+                    result.append(file_elem)
+            elif elem.lower().endswith('.csv'):
+                for file_elem in expand_from_csv_file(Path(elem)):
+                    result.append(file_elem)
+            else:
+                result.append(elem)
+        else:
+            result.append(elem)
+
+    return result
+
+
+def get_obj_ref(obj: vim.ManagedObject) -> str:
+    """
+    Get the value of the Managed Object Reference (MOR) of the given object.
+
+    See: https://vdc-repo.vmware.com/vmwb-repository/dcr-public/1ef6c336-7bef-477d-b9bb-caa1767d7e30/82521f49-9d9a-42b7-b19b-9e6cd9b30db1/mo-types-landing.html
+    """
+    text = str(obj)
+    m = re.match(r"^'(.*)\:(.*)'$", text)
+    if not m:
+        raise ValueError(f'Invalid object identifier: {text}')
+    
+    expected_type = type(obj).__name__
+    if m.group(1) != expected_type:
+        raise ValueError(f'Invalid type for object identifier: {text}, expected: {expected_type}')
+    return m.group(2)
+
+
+def get_obj_path(obj: vim.ManagedEntity, full: bool = False) -> str:
+    """ Return the path of the given vim managed entity. """
+    if not obj:
+        return None
+    if isinstance(obj, vim.Datacenter):
+        return obj.name
+    if not full:
+        if obj.parent:
+            if isinstance(obj.parent, vim.Datacenter):
+                return None            
+            super_parent = obj.parent.parent
+            if isinstance(super_parent, vim.Datacenter):
+                return obj.name
+                
+    if not obj.parent:
+        return obj.name
+    elif not full and isinstance(obj, vim.ResourcePool) and obj.name == 'Resources':
+        return get_obj_path(obj.parent, full=full)
+    else:        
+        return get_obj_path(obj.parent, full=full) + "/" + obj.name
+
+
+def identify_obj(obj: vim.ManagedObject) -> dict:
+    if obj is None:
+        return None
+
+    if not isinstance(obj, vim.ManagedObject):
+        raise ValueError(f'invalid type: {type(obj)}')
+
+    data = {
+        "_type": type(obj).__name__, # managed object type
+        "ref": get_obj_ref(obj),
+    }
+
+    try:
+        if name := getattr(obj, 'name', None):
+            data["name"] = name            
+    except vim.fault.NoPermission:
+        data["name"] = '!error:no_permission'
+
+    if 'name' in data and data["name"] == "Resources" and isinstance(obj, vim.ResourcePool) and hasattr(obj, 'parent') and isinstance(obj.parent, vim.ClusterComputeResource):
+        # root resource pool of a cluster (named 'Resources'): let's prepend cluster name
+        data["name"] = obj.parent.name + "/" + data["name"]
+
+    return data
+    
+
+def dictify_value(data: list|str):
+    """
+    Return a dict if data is a list of OptionValue, StringValue or SystemIdentificationInfo objects, or if it is a string like guestOS.detailed.data.
+    Otherwise leave as is.
+    """
+    def allinstance(enumerable_instance, element_type):
+        any = False
+        for element in enumerable_instance:
+            any = True
+            if not isinstance(element, element_type):
+                return False
+        return any
+        
+    if isinstance(data, list):
+        if allinstance(data, vim.option.OptionValue) or allinstance(data, vim.CustomFieldsManager.StringValue): #example for vm: config.extraConfig, summary.config.customValue
+            result = {}
+            for ov in data:
+                key = ov.key
+                value = ov.value
+                if key == "guestOS.detailed.data":
+                    value = dictify_value(value)
+                result[key] = value
+            return result
+
+        elif allinstance(data, vim.host.SystemIdentificationInfo): #example for host: summary.hardware.otherIdentifyingInfo
+            result = {}
+            for ov in data:
+                key = ov.identifierType.key
+                value = ov.identifierValue
+                result[key] = value
+            return result
+
+        else:
+            return data
+    
+    if isinstance(data, str):
+        if matches := re.findall(r"([a-zA-Z0-9]+)='([^']+)'", data): # example: guestOS.detailed.data
+            result = {}
+            for m in matches:
+                key = m[0]
+                value = m[1]
+                if key == 'bitness' and re.match(r'^\d+$', value):
+                    value = int(value)
+                result[key] = value
+            return result
+
+        else:
+            return data       
+        
+    else:
+        return data
+
+
+def dictify_obj(obj: vim.ManagedEntity, *, object_types=False, exclude_keys=[], max_depth=None) -> dict:
+    """
+    Export all available information about the given VMWare managed object to a dictionnary.
+    """    
+    for key in ['dynamicProperty', 'recentTask']:
+        if not key in exclude_keys:
+            exclude_keys.append(key)
+    exclude_keys_containing = ['capability', 'alarm']
+    keypath = []
+
+    def keypath_str():
+        s = ''
+        for key in keypath:
+            s += ('.' if s and not isinstance(key, int) else '') + (f"[{key}]" if isinstance(key, int) else key)
+        return s
+
+    def forward(key: str):
+        keypath.append(key)
+
+    def backward():
+        del keypath[-1]
+
+    def handle_object(obj: object):
+        if method := getattr(obj.__class__, 'to_dict', None):
+            value = method(obj)
+            if value and object_types:
+                    return { '_type': type(obj).__name__, **value }
+            return value
+
+        result = { '_type': type(obj).__name__ } if object_types else {}
+        any = False
+        for key in dir(obj):
+            ignore = False
+            if key.startswith('_') or key in exclude_keys:
+                ignore = True
+            else:
+                for containing in exclude_keys_containing:
+                    if containing in key.lower():
+                        ignore = True
+                        break
+
+            if ignore:
+                continue
+
+            forward(key)
+            
+            try:
+                value = getattr(obj, key)
+            except: # problem getting the data (e.g. invalid/not-supported accessor)
+                _key = keypath_str()
+                if _key not in ['configManagerEnabled', 'environmentBrowser']:
+                    _logger.error('Cannot read attribute: %s', _key)
+                value = "!error:cannot_read"
+            
+            value = handle_any(value)
+
+            if value is not None:
+                result[key] = value
+                any = True
+
+            backward()
+
+        if any:
+            return result
+
+    def handle_dict(data: dict):
+        result = {}
+        any = False
+        for key in data:
+            forward(key)
+            value = handle_any(data[key])
+            if value is not None:
+                result[key] = value
+                any = True
+            backward()
+
+        if any:
+            return result
+
+    def handle_list(data: list):
+        result = dictify_value(data)
+        if isinstance(result, dict):
+            return result
+
+        # general case
+        result = []
+        any = False
+        for i, value in enumerate(data):
+            forward(i)
+            extracted = handle_any(value)
+            if extracted is not None:
+                result.append(extracted)
+                any = True
+            backward()
+
+        if any:
+            return result
+
+    def handle_any(data):
+        if data is None or isinstance(data, (type, FunctionType, MethodType, BuiltinMethodType, BuiltinFunctionType)):
+            return None
+        
+        elif isinstance(data, (str, int, float, complex)):
+            return data
+
+        elif isinstance(data, date):
+            if data.year == 1970 and data.month == 1 and data.day == 1:
+                return None
+            return data
+
+        elif isinstance(data, vim.ManagedObject):
+            if not keypath: # depth == 0
+                result = identify_obj(data)
+                for key, value in handle_object(data).items():
+                    result[key] = value
+                return result
+            else:
+                return identify_obj(data)
+
+        elif max_depth and len(keypath) >= max_depth:
+            _logger.error('Reached max depth: %s', type(data).__name__)
+            return f"!error:max_depth({type(data).__name__})"
+
+        elif isinstance(data, dict):
+            return handle_dict(data)
+
+        elif isinstance(data, list):
+            return handle_list(data)
+            
+        else:
+            return handle_object(data)
+
+    return handle_any(obj)
+
+
+def dump_obj(obj: vim.ManagedObject, obj_out: os.PathLike|IOBase, *, title: str = None):
+    if not title:
+        title = getattr(obj, 'name', None)
+        if not title:
+            title = type(obj).__name__
+
+    if isinstance(obj_out, IOBase):
+        out_name = getattr(obj_out, 'name', '<io>')
+    else:
+        out_name = str(obj_out)
+
+    data = dictify_obj(obj)
+
+    _logger.info(f"Export {title} to {out_name}")
+    with nullcontext(obj_out) if isinstance(obj_out, IOBase) else open(obj_out, 'w', encoding='utf-8') as fp:
+        json.dump(data, fp=fp, indent=4, cls=ExtendedJSONEncoder, ensure_ascii=False)
 
 
+# For docs
 __all__ = (
     '__prog__', '__version__', '__version_tuple__',
+    'VCenterClient',
+    'get_obj_ref', 'get_obj_path', 'identify_obj', 'dictify_value', 'dictify_obj', 'dump_obj',
 )
```

## vmware_reporter/__main__.py

```diff
@@ -1,28 +1,30 @@
 """
 Interact easily with your VMWare clusters.
 """
 from __future__ import annotations
-from configparser import ConfigParser
-import inspect
+
 import logging
 import os
 from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
+from configparser import ConfigParser
 from contextlib import nullcontext
+from inspect import signature
 from types import FunctionType
 
-from zut import (OutTable, add_func_command, configure_logging, exec_command,
-                 get_help_text, register_locale)
+from zut import (OutTable, add_func_command, add_module_command,
+                 configure_logging, exec_command, get_help_text,
+                 register_locale)
 
-from . import VCenterClient, __prog__, __version__
+from . import VCenterClient, __prog__, __version__, customfield, autoreport
 from .datastore import add_datastore_commands
 from .dump import dump
-from .extract import handle as extract_handle
+from .host import add_host_commands
 from .inventory import export_inventory
-from .networking import add_networking_commands
+from .net import add_net_commands
 from .vm import add_vm_commands
 
 logger = logging.getLogger(__name__)
 
 def main():
     configure_logging()
     register_locale(use_excel_csv=(os.environ.get('USE_EXCEL_CSV') or '1').lower() in ['1', 'yes', 'true', 'on'])
@@ -33,38 +35,41 @@
     subparsers = parser.add_subparsers(title='Commands')
     add_commands(subparsers)
     
     parse_and_exec_command(parser)
     
 
 def init_parser(prog: str = None, version: str = None, doc: str = None, *, config: ConfigParser = None, section: str = None):
-    parser = ArgumentParser(prog=prog, description=get_help_text(doc), formatter_class=RawTextHelpFormatter, add_help=False, epilog='\n'.join(doc.splitlines()[2:]))
+    parser = ArgumentParser(prog=prog, description=get_help_text(doc), formatter_class=RawTextHelpFormatter, add_help=False, epilog='\n'.join(doc.splitlines()[2:]) if doc else None)
     
     envs = VCenterClient.get_configured_envs(config=config, section=section)
 
     group = parser.add_argument_group(title='General options')
     group.add_argument('-e', '--env', default=os.environ.get('VMWARE_DEFAULT_ENV'), help=f"Name of the vCenter to use. Available: {', '.join(envs) if envs else 'none'}.")
     group.add_argument('-h', '--help', action='help', help=f"Show this program help message and exit.")
     group.add_argument('--version', action='version', version=f"{prog} {version or '?'}", help="Show version information and exit.")
 
     return parser
 
 
 def add_commands(subparsers: _SubParsersAction[ArgumentParser]):
     add_func_command(subparsers, export_inventory, name='inventory')
     add_func_command(subparsers, dump, name='dump')
-    add_func_command(subparsers, extract_handle, name='extract')
-    
+
     add_datastore_commands(subparsers, name='datastore')
-    add_networking_commands(subparsers, name='networking')
+    add_net_commands(subparsers, name='net')
+    add_host_commands(subparsers, name='host')
     add_vm_commands(subparsers, name='vm')
+    add_func_command(subparsers, customfield.list_customfields, name='customfield')
+
+    add_module_command(subparsers, autoreport)
         
 
 def get_vcenter(handle: FunctionType, args: dict, *, config: ConfigParser = None, section: str = None):
-    if 'vcenter' in inspect.signature(handle).parameters:
+    if 'vcenter' in signature(handle).parameters:
         env = args.pop('env', None)
         vcenter = VCenterClient(env, config=config, section=section)
         args['vcenter'] = vcenter    
     else:
         vcenter = nullcontext()
 
     return vcenter
```

## vmware_reporter/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.2.1'
-__version_tuple__ = version_tuple = (0, 2, 1)
+__version__ = version = '0.3.0'
+__version_tuple__ = version_tuple = (0, 3, 0)
```

## vmware_reporter/datastore.py

```diff
@@ -1,9 +1,9 @@
 """
-Analyze datastore files or perform operations on datastores.
+Analyze datastores or perform operations on datastores.
 """
 from __future__ import annotations
 
 import logging
 import os
 import re
 from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
@@ -15,82 +15,112 @@
 from typing import BinaryIO
 from urllib.parse import urlencode
 
 import requests
 from pyVmomi import vim
 from zut import (Header, add_func_command, get_description_text, get_help_text,
                  out_table)
-from zut.excel import openpyxl
 
-from . import VCenterClient
-from .inspect import get_obj_path, get_obj_ref
+from . import VCenterClient, get_obj_path, get_obj_ref
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 def add_datastore_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
     parser = commands_subparsers.add_parser(name, help=get_help_text(__doc__), description=get_description_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False)
 
     group = parser.add_argument_group(title='Command options')
     group.add_argument('-h', '--help', action='help', help=f"Show this command help message and exit.")
 
     subparsers = parser.add_subparsers(title='Sub commands')
     add_func_command(subparsers, list_datastores, name='list')
-    add_func_command(subparsers, analyze_datastore_elements, name='elements')
-    add_func_command(subparsers, analyze_datastore_stats, name='stats')
+    add_func_command(subparsers, list_datastore_elements, name='elements')
+    add_func_command(subparsers, list_datastore_stats, name='stats')
     add_func_command(subparsers, download_from_datastore, name='download')
     add_func_command(subparsers, upload_to_datastore, name='upload')
     add_func_command(subparsers, delete_from_datastore, name='delete')
 
 
-DEFAULT_OUT = 'datastores.xlsx#{title}' if openpyxl else 'datastores-{title}.csv'
+_DEFAULT_OUT = '{title}.csv'
 
 
-def list_datastores(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: os.PathLike|IOBase = DEFAULT_OUT):
+def list_datastores(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: os.PathLike|IOBase = _DEFAULT_OUT):
     headers = [
         'name',
         'ref',
+        'overall_status',
+        'config_status',
         Header('capacity', fmt='gib'),
         Header('freespace', fmt='gib'),
+        'accessible',
+        'maintenance_mode',
+        'vmfs_version',
         'url',
         'extent',
+        'multiple_host_access',
+        'host_access',
     ]
 
-    with out_table(out, title='datastores', dir=vcenter.get_out_dir(), headers=headers) as t:
+    with out_table(out, title='datastores', dir=vcenter.get_out_dir(), env=vcenter.env, headers=headers) as t:
         for obj in vcenter.iter_objs(vim.Datastore, search, normalize=normalize, key=key):            
             try:
-                logger.info(f"Analyze {obj.name}")
+                _logger.info(f"Analyze datastore {obj.name}")
 
                 t.append([
                     obj.name,
                     get_obj_ref(obj),
+                    obj.overallStatus,
+                    obj.configStatus,
                     obj.info.vmfs.capacity,
                     obj.info.freeSpace,
+                    obj.summary.accessible,
+                    obj.summary.maintenanceMode,
+                    obj.info.vmfs.version,
                     obj.info.url,
-                    parse_extent(obj.info.vmfs.extent),
+                    parse_datacore_extent(obj.info.vmfs.extent),
+                    obj.summary.multipleHostAccess,
+                    get_datastore_host_summaries(obj),
                 ])
             
             except Exception as err:
-                logger.exception(f"Error while analyzing {str(obj)}")
+                _logger.exception(f"Error while analyzing {str(obj)}")
 
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('search', nargs='*', help="Search term(s).")
     parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
     parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
-    parser.add_argument('-o', '--out', default=DEFAULT_OUT, help="Output table (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output table (default: %(default)s).")
 
 list_datastores.add_arguments = _add_arguments
 
-def parse_extent(extent: list[vim.host.ScsiDisk.Partition]):
+
+def get_datastore_host_summaries(datastore: vim.Datastore):
+    summaries = []
+    for host_access in sorted(datastore.host, key=lambda ha: ha.key.name):
+        issue = ''
+
+        if not host_access.mountInfo.mounted:
+            issue = (', ' if issue else '') + f'notMounted'
+        elif not host_access.mountInfo.accessible:
+            issue = (', ' if issue else '') + f'notAccessible'
+
+        if host_access.mountInfo.accessMode != 'readWrite':
+            issue = (', ' if issue else '') + f'{host_access.mountInfo.accessMode}'
+
+        summaries.append(host_access.key.name + (f' [{issue}]' if issue else ''))
+
+    return summaries
+
+
+def parse_datacore_extent(extent: list[vim.host.ScsiDisk.Partition]):
     if extent is None:
         return None
     return [part.diskName + ('' if part.partition == 1 else f' (partition {part.partition})') for part in extent]
 
 
-
 def iterate_datastore_elements(vcenter: VCenterClient, obj: vim.Datastore, path: str = None, *, pattern: str = None, max_depth: int = None, with_size: bool = True, with_mtime: bool = True, with_owner: bool = True, case_sensitive: bool = False):
     """
     Iterate over datastore elements (files and directories).
     """
     if path:
         path = path.strip("/\\")
         dspath = f"[{obj.name}] {path}"
@@ -172,76 +202,76 @@
             stat.file_count += 1
         else:
             stat.other_count += 1
 
     return sorted(stats.values(), key=lambda stat: stat.path)
 
 
-def analyze_datastore_elements(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', path: str = None, max_depth: int = None, out: os.PathLike|IOBase = None, bytes: bool = False):
+def list_datastore_elements(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', path: str = None, max_depth: int = None, out: os.PathLike|IOBase = _DEFAULT_OUT, bytes: bool = False):
     """
-    Analyze datastore elements (files and directories).
+    List datastore elements (files and directories).
     """
-    with out_table(out, headers=DatastoreElement.get_headers(bytes=bytes), title="datastore elements", dir=vcenter.get_out_dir()) as t:
+    with out_table(out, headers=DatastoreElement.get_headers(bytes=bytes), title="datastore_elements", dir=vcenter.get_out_dir(), env=vcenter.env) as t:
         for obj in vcenter.get_objs(vim.Datastore, search, normalize=normalize, key=key, sort_key='name'):
-            logger.info(f'analyze datastore {obj.name}')
-
+            _logger.info(f'List datastore elements: {obj.name}')
+        
             try:
                 for info in sorted(iterate_datastore_elements(vcenter, obj, path=path, max_depth=max_depth), key=lambda info: info.path):
                     t.append(info.as_row())
             except:
-                logger.exception(f'cannot analyze datastore {obj.name}')
+                _logger.exception(f'Cannot analyze datastore {obj.name}')
 
 
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('search', nargs='*', help="Search term(s).")
     parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
     parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
     parser.add_argument("--path", help="Detail elements only for the given path.")
     parser.add_argument("--max-depth", type=int, help="Detail elements until the given depth (default: %(default)s).")
-    parser.add_argument('-o', '--out', help="Output file (default: stdout).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output file (default: %(default)s).")
     parser.add_argument('--bytes', action="store_true", help="Display size as bytes.")
 
-analyze_datastore_elements.add_arguments = _add_arguments
+list_datastore_elements.add_arguments = _add_arguments
 
 
-def analyze_datastore_stats(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', path: str = None, max_depth: int = None, out: os.PathLike|IOBase = None, bytes: bool = False):
+def list_datastore_stats(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', path: str = None, max_depth: int = 1, out: os.PathLike|IOBase = _DEFAULT_OUT, bytes: bool = False):
     """
     Analyze stats about datastore elements (files and directories).
     """
-    with out_table(out, headers=DatastoreStat.get_headers(bytes=bytes), title="datastore elements", dir=vcenter.get_out_dir()) as t:
+    with out_table(out, headers=DatastoreStat.get_headers(bytes=bytes), title="datastore_stats", dir=vcenter.get_out_dir(), env=vcenter.env) as t:
         for obj in vcenter.get_objs(vim.Datastore, search, normalize=normalize, key=key, sort_key='name'):
-            logger.info(f'analyze datastore {obj.name}')
+            _logger.info(f'Analyze datastore stats: {obj.name}')
 
             try:
                 for info in get_datastore_stats(vcenter, obj, path=path, max_depth=max_depth):
                     t.append(info.as_row())
             except:
-                logger.exception(f'cannot analyze datastore {obj.name}')
+                _logger.exception(f'Cannot analyze datastore {obj.name}')
 
 
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('search', nargs='*', help="Search term(s).")
     parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
     parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
     parser.add_argument("--path", help="Detail elements only for the given path.")
     parser.add_argument("--max-depth", type=int, default=1, help="Detail elements until the given depth (default: %(default)s).")
-    parser.add_argument('-o', '--out', help="Output file (default: stdout).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output file (default: %(default)s).")
     parser.add_argument('--bytes', action="store_true", help="Display size as bytes.")
 
-analyze_datastore_stats.add_arguments = _add_arguments
+list_datastore_stats.add_arguments = _add_arguments
 
 
 def request_datastore_resource(method: str, vcenter: VCenterClient, datastore: vim.Datastore|str, path: os.PathLike, data: BinaryIO = None):
     datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
 
     if not isinstance(path, Path):
         path = Path(path)
 
     path = "/folder/%s" % path.as_posix()
-    params = {"dsName": datastore_name, "dcPath": get_obj_path(vcenter.datacenter)}
+    params = {"dsName": datastore_name, "dcPath": get_obj_path(vcenter.datacenter, full=True)}
     url = f"https://{vcenter.host}" + path + '?' + urlencode(params)
     
     headers = {}
     if data:
         headers['Content-Type'] = 'application/octet-stream'
 
     response = requests.request(method, url, data=data, headers=headers, cookies=vcenter.cookie, verify=not vcenter.no_ssl_verify)
@@ -258,15 +288,15 @@
 
     response = request_datastore_resource('GET', vcenter, datastore, path)
     with open(target, 'wb') as fp:
         for chunck in response.iter_content():
             fp.write(chunck)
     
     datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
-    logger.info("%s %s from datastore %s to %s", 'downloaded' if response.status_code == HTTPStatus.OK else f'{response.status_code} {response.reason}', path, datastore_name, target)
+    _logger.info("%s %s from datastore %s to %s", 'downloaded' if response.status_code == HTTPStatus.OK else f'{response.status_code} {response.reason}', path, datastore_name, target)
 
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('datastore', help="Name of the datastore.")
     parser.add_argument('path', help="Path of the object to download on the datastore.")
     parser.add_argument('target', nargs='?', default='', help="Target path on the local file system.")
 
 download_from_datastore.add_arguments = _add_arguments
@@ -284,15 +314,15 @@
     if isinstance(source, IOBase) and hasattr(source, 'encoding'):
         raise ValueError("Cannot send files opened in text mode")
 
     with nullcontext(source) if isinstance(source, IOBase) else open(source, 'rb') as fp:
         response = request_datastore_resource('PUT', vcenter, datastore, target, data=fp)
     
     datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
-    logger.info("uploaded %s to datastore %s: %s %s", source, datastore_name, 'created' if response.status_code == HTTPStatus.CREATED else ('updated' if response.status_code == HTTPStatus.OK else f'{response.status_code} {response.reason}'), target)
+    _logger.info("uploaded %s to datastore %s: %s %s", source, datastore_name, 'created' if response.status_code == HTTPStatus.CREATED else ('updated' if response.status_code == HTTPStatus.OK else f'{response.status_code} {response.reason}'), target)
 
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('source', help="Path of the source data.")
     parser.add_argument('datastore', help="Name of the datastore.")
     parser.add_argument('target', nargs='?', default='', help="Target path on the datastore.")
 
 upload_to_datastore.add_arguments = _add_arguments
@@ -301,15 +331,15 @@
 def delete_from_datastore(vcenter: VCenterClient, datastore: vim.Datastore|str, path: os.PathLike):
     """
     Delete a file from a datastore.
     """
     response = request_datastore_resource('DELETE', vcenter, datastore, path)
     
     datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
-    logger.info("%s %s from datastore %s", 'deleted' if response.status_code == HTTPStatus.NO_CONTENT else f'{response.status_code} {response.reason}', path, datastore_name)
+    _logger.info("%s %s from datastore %s", 'deleted' if response.status_code == HTTPStatus.NO_CONTENT else f'{response.status_code} {response.reason}', path, datastore_name)
 
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('datastore', help="Name of the datastore.")
     parser.add_argument('path', help="Path of the object to delete on the datastore.")
 
 delete_from_datastore.add_arguments = _add_arguments
```

## vmware_reporter/dump.py

```diff
@@ -1,25 +1,27 @@
+"""
+Dump all available data about VMWare managed objects.
+"""
 from __future__ import annotations
 
 import logging
 import os
 import re
 import sys
 from argparse import ArgumentParser
 from io import IOBase
 
-from . import VCenterClient
-from .inspect import get_obj_ref, dump_obj
+from . import VCenterClient, get_obj_ref, dump_obj
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
-DEFAULT_OUT = os.path.join("dumps", "{type}", "{name} ({ref}).json")
+_DEFAULT_OUT = os.path.join("dumps", "{type}", "{name} ({ref}).json")
 
 
-def dump(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', first: bool = False, types: list[type|str]|type|str = None, out: os.PathLike|IOBase = DEFAULT_OUT):
+def dump(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', first: bool = False, types: list[type|str]|type|str = None, out: os.PathLike|IOBase = _DEFAULT_OUT):
     """
     Export all available data about VMWare managed objects to JSON files.
     """
     if not out or out == 'stdout':
         out = sys.stdout
     elif out == 'stderr':
         out = sys.stderr
@@ -38,15 +40,15 @@
 
         name = obj.name
         ref = get_obj_ref(obj)
         
         if isinstance(out, IOBase):
             obj_out = out
         else:
-            obj_out = os.path.join(vcenter.get_out_dir(), str(out).format(type=type(obj).__name__, name=name, ref=ref))
+            obj_out = os.path.join(vcenter.get_out_dir(), str(out).format(type=type(obj).__name__, name=name, ref=ref, env=vcenter.env))
             obj_out_dir = os.path.dirname(obj_out)
             if obj_out_dir:
                 os.makedirs(obj_out_dir, exist_ok=True)
         
         dump_obj(obj, obj_out, title=f'{name} ({ref})')
 
         if first:
@@ -54,10 +56,10 @@
 
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('search', nargs='*', help="Search term(s).")
     parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
     parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
     parser.add_argument('-t', '--type', dest='types', metavar='type', help="Managed object type name (example: datastore).")
     parser.add_argument('--first', action='store_true', help="Only handle the first object found for each type.")
-    parser.add_argument('-o', '--out', default=DEFAULT_OUT, help="Output JSON file (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output JSON file (default: %(default)s).")
 
 dump.add_arguments = _add_arguments
```

## vmware_reporter/inventory.py

```diff
@@ -1,75 +1,77 @@
+"""
+Inventory of VMWare managed objects.
+"""
 from __future__ import annotations
 
 import logging
 import os
 import sys
 from argparse import ArgumentParser
 from contextlib import nullcontext
 from io import IOBase
 
 from pyVmomi import vim
 
-from . import VCenterClient
-from .inspect import get_obj_ref
+from . import VCenterClient, get_obj_ref
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
-DEFAULT_OUT = "inventory.yml"
+_DEFAULT_OUT = "inventory.yml"
 
 
-def export_inventory(vcenter: VCenterClient, assets: list[str] = None, out: os.PathLike|IOBase = DEFAULT_OUT):
+def export_inventory(vcenter: VCenterClient, assets: list[str] = None, out: os.PathLike|IOBase = _DEFAULT_OUT):
     """
-    Export inventory of VMWare managed objects to a YAML file.
+    Export an inventory of VMWare managed objects to a YAML file.
     """
     inventory = build_inventory(vcenter, assets=assets)
     
     if not out or out == 'stdout':
         out = sys.stdout
     elif out == 'stderr':
         out = sys.stderr
 
     if isinstance(out, IOBase):
         out_name = getattr(out, 'name', '<io>')
     else:
-        out = os.path.join(vcenter.get_out_dir(), out)
+        out = os.path.join(vcenter.get_out_dir(), str(out).format(env=vcenter.env))
         out_name = str(out)
         
-    logger.info(f"export inventory to {out_name}")
+    _logger.info(f"export inventory to {out_name}")
     inventory.to_yaml(out)
 
 
 def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('-o', '--out', default=DEFAULT_OUT, help="Output YAML file (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output YAML file (default: %(default)s).")
     parser.add_argument('--asset', nargs='*', dest='assets')
 
 export_inventory.add_arguments = _add_arguments
 
 
 def build_inventory(vcenter: VCenterClient, assets: list[str] = None) -> InventoryNode:
     node = InventoryNode(vcenter.env, nature=VCenterClient)
 
     if not assets:
         assets = ['folder', 'license', 'authorization']
 
     for asset in assets:
         if asset == 'folder':
-            logger.info(f"build folder inventory")
+            _logger.info(f"build folder inventory")
             build_folder_inventory(vcenter, parent=node)
             
         elif asset == 'authorization':
-            logger.info(f"build authorization inventory")
+            _logger.info(f"build authorization inventory")
             build_authorization_inventory(vcenter, parent=node)
         
         elif asset == 'license':
-            logger.info(f"build license inventory")
+            _logger.info(f"build license inventory")
             build_license_inventory(vcenter, parent=node)
 
         else:
-            logger.error(f"Unknown asset: {asset}")
+            _logger.error(f"Unknown asset: {asset}")
 
     return node
 
 
 def build_folder_inventory(vcenter: VCenterClient, parent = None) -> InventoryNode:
     found_by_ref: dict[str,vim.ManagedEntity] = {}
```

## vmware_reporter/vm.py

```diff
@@ -1,55 +1,447 @@
 """
-Analyze VM disks or NICs.
+Manage virtual machines.
 """
 from __future__ import annotations
 
+import json
 import logging
+import os
 import re
 from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
+from datetime import datetime
+from io import IOBase
+from ipaddress import IPv4Address, IPv6Address, ip_address
 from pathlib import Path
-from typing import Literal
+from typing import Any, Callable, Literal
 
 from pyVmomi import vim
 from zut import (Header, add_func_command, get_description_text, get_help_text,
-                 gigi_bytes, out_table)
-from zut.excel import openpyxl
+                 gigi_bytes, out_table, slugify)
+from zut.excel import ExcelRow, ExcelWorkbook, split_excel_path
 
-from . import VCenterClient
-from .inspect import dictify_obj, dictify_value, get_obj_ref
+from . import (VCenterClient, dictify_obj, dictify_value, get_obj_path,
+               get_obj_ref)
 
 logger = logging.getLogger(__name__)
 
+_DEFAULT_OUT = '{title}.csv'
+
 def add_vm_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
     parser = commands_subparsers.add_parser(name, help=get_help_text(__doc__), description=get_description_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False)
 
     group = parser.add_argument_group(title='Command options')
     group.add_argument('-h', '--help', action='help', help=f"Show this command help message and exit.")
 
     subparsers = parser.add_subparsers(title='Sub commands')
-    #TODO add_func_command(subparsers, list_vms, name='list')
-    add_func_command(subparsers, analyze_disks, name='disks')
-    add_func_command(subparsers, analyze_nics, name='nics')
+    add_func_command(subparsers, list_vms, name='list')
+    add_func_command(subparsers, list_vm_disks, name='disks')
+    add_func_command(subparsers, list_vm_nics, name='nics')
+    
+    # Operations
+    add_func_command(subparsers, start_vms, name='start')
+    add_func_command(subparsers, stop_vms, name='stop')
+    add_func_command(subparsers, suspend_vms, name='suspend')    
+    add_func_command(subparsers, reconfigure_vms, name='reconfigure')
+
+
+#region List
+
+def list_vms(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: os.PathLike|IOBase = _DEFAULT_OUT):
+    headers = [
+        'name',
+        'ref',
+        'overall_status',
+        'config_status',
+        'template',
+        # Config
+        'vcpu',
+        'cores_per_socket',
+        Header('memory', fmt='gib'),
+        Header('disk_capacity', fmt='gib'),
+        Header('disk_freespace', fmt='gib'),
+        'disk_count',
+        'nic_count',
+        # Dossier / rangement
+        'folder',
+        'Appartenance',
+        'other_custom_values',
+        'annotation',
+        'create_date',
+        'change_date',
+        # Config details
+        'hostname',
+        'network',
+        'disk',
+        # ResourcePool / runtime
+        'resource_pool',
+        'host',
+        'power_state',
+        'paused',
+        'connection_state',
+        'boot_time',
+        'hw_version',
+        # Guest info
+        'os_family',
+        'os_version',
+        'os_distro_version',
+        'os_kernel_version',
+        'tools_status',
+        'tools_running_status',
+        'tools_version_number',
+        'tools_version',
+        'guestinfo_publish_time',
+    ]
+
+    with out_table(out, title='vms', dir=vcenter.get_out_dir(), env=vcenter.env, headers=headers, after1970=True) as t:
+        for obj in vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key):  
+            try:
+                logger.info(f"Analyze vm {obj.name}")
+
+                disks = extract_disks(obj)
+                nics = extract_nics(obj, vcenter=vcenter)
+
+                custom_values = get_custom_values(obj)
+                Appartenance = custom_values.pop('Appartenance', None)
+                other_custom_values = ' | '.join(f"{key}: {value}" for key, value in custom_values.items())
+
+                extra_config = dictify_value(obj.config.extraConfig)
+
+                t.append([
+                    obj.name,
+                    get_obj_ref(obj),
+                    obj.overallStatus,
+                    obj.configStatus,
+                    obj.config.template,
+                    # Config
+                    obj.config.hardware.numCPU,
+                    obj.config.hardware.numCoresPerSocket,
+                    obj.config.hardware.memoryMB * 1024 * 1024,
+                    disks.capacity,
+                    disks.freespace,
+                    obj.summary.config.numVirtualDisks,
+                    obj.summary.config.numEthernetCards,
+                    # Dossier / rangement
+                    get_obj_path(obj.parent),
+                    Appartenance,
+                    other_custom_values,
+                    obj.config.annotation,
+                    obj.config.createDate,
+                    datetime.fromisoformat(obj.config.changeVersion),
+                    # Config details
+                    obj.guest.hostName,
+                    nics.to_summary(ip_version=4),
+                    disks.to_summary(),
+                    # ResourcePool / runtime
+                    get_obj_path(obj.resourcePool),
+                    obj.runtime.host.name,
+                    obj.runtime.powerState,
+                    obj.runtime.paused,
+                    obj.runtime.connectionState,
+                    obj.runtime.bootTime,
+                    obj.config.version,
+                    # Guest info
+                    get_os_family(extra_config, obj.config.guestFullName),
+                    get_os_version(extra_config),
+                    get_os_distro_version(extra_config),
+                    get_os_kernel_version(extra_config),
+                    obj.guest.toolsStatus,  # nominal: toolsOk
+                    obj.guest.toolsRunningStatus,  # nominal: guestToolsRunning
+                    get_tools_version_number(obj.guest.toolsVersion),  # version number
+                    get_tools_version(extra_config, obj.guest.toolsVersion),      
+                    get_guestinfo_publish_time(extra_config),
+                ])
+            
+            except Exception as err:
+                logger.exception(f"Error while analyzing {str(obj)}")
+
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output table (default: %(default)s).")
+
+list_vms.add_arguments = _add_arguments
+
+#endregion
 
 
-DEFAULT_OUT = 'vms.xlsx#{title}' if openpyxl else 'vms-{title}.csv'
+#region Start, stop, suspend
+
+def start_vms(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', **options):
+    _invoke_and_track('PowerOn', vcenter, search, normalize=normalize, key=key)
+
+def stop_vms(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', force: bool = False):
+    if force:
+        _invoke_and_track('PowerOff', vcenter, search, normalize=normalize, key=key)
+    else:
+        _invoke_and_track('ShutdownGuest', vcenter, search, normalize=normalize, key=key)
+
+def suspend_vms(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', force: bool = False):
+    if force:
+        _invoke_and_track('Suspend', vcenter, search, normalize=normalize, key=key)
+    else:
+        _invoke_and_track('StandbyGuest', vcenter, search, normalize=normalize, key=key)
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument('-f', '--force', action='store_true', help="Force operation.")
+
+start_vms.add_arguments = _add_arguments
+stop_vms.add_arguments = _add_arguments
+suspend_vms.add_arguments = _add_arguments
+
+
+def _invoke_and_track(op: str, vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name'):
+    # Idea: https://github.com/reubenur-rahman/vmware-pyvmomi-examples/blob/master/vm_power_ops.py
+    tasks = {}
+    for vm in vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key):
+        log_prefix = f"{vm.name} ({get_obj_ref(vm)})"
+        logger.info(f"{op} {log_prefix}...")
+        func = getattr(vm, op)
+        try:
+            task = func()
+            if task is not None:
+                tasks[task] = log_prefix
+        except Exception as err:
+            logger.error(f"{log_prefix}: {str(err)}")
+
+    if tasks:
+        vcenter.wait_for_task(tasks)
+
+
+#endregion
+
+
+#region Reconfigure
+
+DEFAULT_RECONFIGURE_FILE = 'vms_reconfigure.xlsx'
+DEFAULT_RECONFIGURE_TABLE = 'vms'
+
+def reconfigure_vms(vcenter: VCenterClient, path: str|Path = DEFAULT_RECONFIGURE_FILE, top: int = None, ignore_invalid_current: bool = False):
+    """
+    Reconfigure VMs (vcpu, memory, annotation, custom fields) as a mass operation, using an Excel file.
+    """
+    class Helper:
+        def __init__(self, row: ExcelRow, found: bool = False):
+            self.row = row
+            self.found = found
+
+        def report_ok(self, details: str):
+            logger.info(f"OK: {details}")
+            self.row['status'] = 'OK'
+            self.row['details'] = details
+
+        def report_error(self, details: str):
+            logger.error(details)
+            self.row['status'] = 'ERROR'
+            self.row['details'] = details
+            
+    class FieldDef:
+        def __init__(self, name: str, type: type, getter: Callable[[vim.VirtualMachine],Any]|Literal['__customvalue__'], target_key:str|int, target_formatter: Callable[[vim.VirtualMachine],Any] = None):
+            """
+            - `key`: if str, this is the reconfigure ConfigSpec argument to use. If int, this is the customfield key to use.
+            """
+            self.name = name
+            self.type = type
+            self.getter = getter
+            self.target_key = target_key
+            self.target_formatter = target_formatter
+
+        def get_from_vm(self, vm: vim.VirtualMachine):
+            if self.getter == '__customvalue__':
+                for kv in vm.customValue:
+                    if kv.key == self.target_key:
+                        return kv.value
+            else:
+                return self.getter(vm)
+
+        def get_from_row(self, row: ExcelRow, suffix: str = None):
+            value = row.get(f"{self.name}_{suffix}" if suffix else self.name)
+            if value is None or value == '':
+                return None
+            if self.type == str and value == '-':
+                return ''
+            return self.type(value)
+        
+        def format_for_target(self, value):
+            if not self.target_formatter:
+                return value
+            return self.target_formatter(value)
+
+    fielddefs: list[FieldDef] = [
+        FieldDef('vcpu', int, lambda vm: vm.config.hardware.numCPU, 'numCPUs'),
+        FieldDef('memory', float, lambda vm: vm.config.hardware.memoryMB / 1024.0, 'memoryMB', lambda val: int(val * 1024.0)),
+        FieldDef('annotation', str, lambda vm: vm.config.annotation, 'annotation'),
+    ]
+
+    for customfield in vcenter.service_content.customFieldsManager.field:
+        if customfield.managedObjectType == vim.VirtualMachine:
+            fielddefs.append(FieldDef(customfield.name, str, '__customvalue__', customfield.key))
+    
+    path, tablename = split_excel_path(path, default_table_name=DEFAULT_RECONFIGURE_TABLE, dir=vcenter.get_out_dir(), env=vcenter.env)
+
+    workbook = ExcelWorkbook(path)
+    table = workbook.get_or_create_table(tablename)
+    
+    helpers: dict[str,Helper] = {}
+    search_by_ref = 'ref' in table.column_names
+    for row in table:
+        if search_by_ref:
+            if row['ref']:
+                helpers[row['ref']] = Helper(row)
+        else:
+            if row['name']:
+                helpers[slugify(row['name'])] = Helper(row)
+        row['status'] = None
+        row['details'] = None
+    
+    n = 0
+    for vm in vcenter.iter_objs(vim.VirtualMachine):
+        if top is not None and n == top:
+            logger.warning(f"Stop after {n} VMs")
+            break
+
+        key = get_obj_ref(vm) if search_by_ref else slugify(vm.name)
+        helper = helpers.get(key)
+        if not helper:
+            continue
+        
+        if helper.found:
+            logger.error(f"VM {vm.name}: ignore (several VMs with key \"{key}\")")
+            continue
+        helper.found = True
+
+        n += 1        
+        logger.info(f"Handle {vm.name} ({get_obj_ref(vm)})")
+        row = helper.row
+
+        try:
+            if search_by_ref and slugify(vm.name) != slugify(row['name']):
+                helper.report_error(f"Invalid VM name: expected {vm.name}")
+                continue
+
+            if vm.config.template:
+                helper.report_error(f"This is a template")
+                continue
+
+            if vm.runtime.powerState != 'poweredOff':
+                helper.report_error(f"Not powered off")
+                continue
+
+            config_previous: dict[str|int,Any] = {}
+            config_targets: dict[str|int,Any] = {}
+            invalid_current = ''
+
+            # Prepare reconfiguration
+            change_version = vm.config.changeVersion  # used to guard against updates that have happened between when configInfo is read and when it is applied
+
+            for fielddef in fielddefs:
+                target = fielddef.get_from_row(row, 'target')
+                if target is None:
+                    continue
+
+                current = fielddef.get_from_vm(vm)
+                current_expected = fielddef.get_from_row(row)
+                if current_expected is not None:
+                    if current_expected != current and not ignore_invalid_current:
+                        invalid_current += (', ' if invalid_current else '') + f"current {fielddef.name}: {'(empty)' if current == '' else current}"   
+                        continue
+
+                if target != current:
+                    config_previous[fielddef.target_key] = fielddef.format_for_target(current)
+                    config_targets[fielddef.target_key] = fielddef.format_for_target(target)
+
+            if invalid_current:
+                helper.report_error(f"Invalid {invalid_current}")
+                continue
+
+            if not config_targets:
+                helper.report_ok("Nothing to do")
+                continue
+
+            config_targets_reconfigure = {}
+            config_targets_customfields = {}
+            for key, value in config_targets.items():
+                if isinstance(key, str):
+                    config_targets_reconfigure[key] = value
+                else:
+                    config_targets_customfields[key] = value
+
+            # Perform the reconfiguration
+            if config_targets_reconfigure:
+                logger.debug("Reconfigure VM: %s", config_targets_reconfigure)
+                configspec = vim.vm.ConfigSpec(**config_targets_reconfigure, changeVersion=change_version)
+                task = vm.ReconfigVM_Task(configspec)
+                vcenter.wait_for_task(task)
+
+            for key, value in config_targets_customfields.items():
+                logger.debug("Set custom field %s: %s", key, value)
+                vcenter.service_content.customFieldsManager.SetField(vm, key, value)
+
+            # Verification
+            status_ok = True
+            details = ''
+
+            for fielddef in fielddefs:
+                if not fielddef.target_key in config_targets:
+                    continue # field not modified
+
+                previous_value = config_previous[fielddef.target_key]
+                target_value = config_targets[fielddef.target_key]
+                new_value = fielddef.format_for_target(fielddef.get_from_vm(vm))
+                details += (', ' if details else '') + f"{fielddef.target_key}: {previous_value} -> {'(empty)' if new_value == '' else new_value}"
+
+                if new_value != target_value:
+                    status_ok = False
+                    details += ' [ERROR]'
+
+            if status_ok:
+                helper.report_ok(details)
+            else:
+                helper.report_error(details)
+        
+        except Exception as err:
+            logger.exception(str(err))
+            row['status'] = type(err).__name__
+            row['details'] = str(err)
+
+    # Report not found
+    for key, helper in helpers.items():
+        if not helper.found:
+            helper.report_error(f"VM {key} not found")
+
+    workbook.close()
+
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('path', nargs='?', default=DEFAULT_RECONFIGURE_FILE, help="Path to Excel file describing VMs to reconfigure.")
+    parser.add_argument('--top', type=int)
+    parser.add_argument('--ignore-invalid-current', action='store_true')
+
+reconfigure_vms.add_arguments = _add_arguments
+
+
+#endregion
 
 
 #region Disks
 
-def analyze_disks(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: str = DEFAULT_OUT, top: int = None):
+def list_vm_disks(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: str = _DEFAULT_OUT, top: int = None):
     """
     Analyze VM disks.
     """
     disks_per_vm_headers = [
         'vm',
         'power_state',
-        'os_info',
         'os_family',
-        'os_name',
+        'os_version',
         'device_disks',
         'guest_disks',
         'with_mappings',
         'without_mappings',
         'mapped_guest',
         'unmapped_guest',
         Header('capacity', fmt='gib'),
@@ -62,17 +454,16 @@
         Header('unmapped_guests_freespace', fmt='gib'),
         'issues',
     ]
 
     disks_headers = [
         'vm',
         'power_state',
-        'os_info',
         'os_family',
-        'os_name',
+        'os_version',
         'key',
         'backing',
         'datastore',
         'filename',
         'diskmode',
         'sharing',
         'remaining_backing_info',
@@ -81,43 +472,40 @@
         'mapping',
         'guests',
         Header('guests_capacity', fmt='gib'),
         Header('guests_freespace', fmt='gib'),
         'capacity_loss_pct',
     ]
     
-    with (out_table(out, title='disks', headers=disks_headers, dir=vcenter.get_out_dir()) as t_disks,
-          out_table(out, title='disks_per_vm', headers=disks_per_vm_headers, dir=vcenter.get_out_dir()) as t_disks_per_vm):
+    with (out_table(out, title='vm_disks', headers=disks_headers, dir=vcenter.get_out_dir(), env=vcenter.env) as t_disks,
+          out_table(out, title='vm_disks_per_vm', headers=disks_per_vm_headers, dir=vcenter.get_out_dir(), env=vcenter.env) as t_disks_per_vm):
         
         for i, vm in enumerate(vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key)):
             if top is not None and i == top:
                 break
             
             try:
-                logger.info(f"Analyze {vm.name} disks")
+                logger.info(f"Analyze vm {vm.name} disks")
 
                 info = extract_disks(vm)
 
-                os = dictify_value(vm.config.extraConfig).get('guestOS.detailed.data')
-                if not os:
-                    os = {}
-                os_family = os.get('familyName')
-                os_name = os.get('prettyName')
+                extra_config = dictify_value(vm.config.extraConfig)
+                os_family = get_os_family(extra_config, vm.config.guestFullName)
+                os_version = get_os_version(extra_config)
 
                 mapped_guests: list[vim.vm.GuestInfo.DiskInfo] = []
                 for disk in info.disks:
                     for guest in disk.guests:
                         mapped_guests.append(guest)
 
                 t_disks_per_vm.append([
                     vm.name, # vm
                     vm.runtime.powerState, # power_state
-                    vm.config.guestFullName, # os_info
-                    os_family, # os_family
-                    os_name, # os_name
+                    os_family,
+                    os_version,
                     len(info.disks), # 'device_disks',
                     len(mapped_guests) + len(info.unmapped_guests), # 'guest_disks',
                     len(mapped_guests), # 'with_mappings',
                     len(info.unmapped_guests), # 'without_mappings',
                     sorted(f'{guest.diskPath} ({guest.filesystemType})' if guest.filesystemType else guest.diskPath for guest in mapped_guests), # 'mapped_guest',
                     sorted(f'{guest.diskPath} ({guest.filesystemType})' if guest.filesystemType else guest.diskPath for guest in info.unmapped_guests),# 'unmapped_guests',
                     info.capacity,
@@ -143,17 +531,16 @@
 
                     capacity_loss = disk.capacity - disk.guests_capacity if disk.guests else None
                     capacity_loss_pct = 100 * capacity_loss / disk.capacity if disk.guests else None
                     
                     t_disks.append([
                         vm.name, # vm
                         vm.runtime.powerState, # power_state
-                        vm.config.guestFullName, # os_info
-                        os_family, # os_family
-                        os_name, # os_name
+                        os_family,
+                        os_version,
                         disk.device.key, # key
                         backing_typename, # backing
                         datastore['name'] if datastore else None, # datastore
                         fileName,
                         diskMode,
                         sharing,
                         device_backing, # remaining_backing_info
@@ -166,17 +553,16 @@
                         capacity_loss_pct,
                     ])
 
                 for guest in [*info.unmapped_guests, *info.ignored_guests]:
                     t_disks.append([
                         vm.name, # vm
                         vm.runtime.powerState, # power_state
-                        vm.config.guestFullName, # os_info
-                        os_family, # os_family
-                        os_name, # os_name
+                        os_family,
+                        os_version,
                         None, # key
                         guest.mappings, # backing
                         None, # datastore
                         None, # filename
                         None, # diskMode
                         None, # sharing
                         None, # remaining_backing_info
@@ -194,17 +580,17 @@
 
 
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('search', nargs='*', help="Search term(s).")
     parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
     parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
     parser.add_argument('--top', type=int)
-    parser.add_argument('-o', '--out', default=DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
 
-analyze_disks.add_arguments = _add_arguments
+list_vm_disks.add_arguments = _add_arguments
 
 
 def extract_disks(vm: vim.VirtualMachine):
     info = VmDisks(vm)
 
     # Retrieve disk devices
     disks_per_key: dict[int,VmDisk] = {}
@@ -399,23 +785,44 @@
             guests_data = []
             data.append({'guests_mapping': 'ignored', 'guests':  guests_data})
             for guest in self.ignored_guests:
                 guests_data.append(self._get_guest_dict(guest))
 
         return data
     
+    def to_summary(self):
+        result = ''
+
+        for disk in self.disks:
+            result += (' | ' if result else '') + disk.to_summary()
+
+        if self.unmapped_guests:
+            result += (' | ' if result else '') + f"Unmapped guests ("
+            for i, guest in enumerate(self.unmapped_guests):
+                if i > 0:
+                    result += ', '
+                result += self._get_guest_summary(guest)
+            result += ')'
+
+        return result
+    
     @classmethod
     def _get_guest_dict(cls, guest: vim.vm.GuestInfo.DiskInfo):
         data = {}
         data['path'] = guest.diskPath
         data['capacity'] = gigi_bytes(guest.capacity)
         data['freespace'] = gigi_bytes(guest.freeSpace)
         if value := guest.filesystemType:
             data['filesystem'] = value
         return data
+    
+    @classmethod
+    def _get_guest_summary(cls, guest: vim.vm.GuestInfo.DiskInfo):
+        path = guest.diskPath.rstrip(':\\')
+        return f'{path}: {gigi_bytes(guest.freeSpace):.1f}/{gigi_bytes(guest.capacity):.1f} GiB'
 
 
 class VmDisk:
     def __init__(self, device: vim.vm.device.VirtualDisk):
         self.device = device
         self.guests: list[vim.vm.GuestInfo.DiskInfo] = []
         self.guests_mapping: Literal['key','capacity'] = None
@@ -458,83 +865,97 @@
         if self.guests:
             data['guests'] = []
 
             for guest in self.guests:
                 data['guests'].append(VmDisks._get_guest_dict(guest))
         
         return data
+    
+    def to_summary(self):
+
+        filename: str = getattr(self.device.backing, 'fileName', None)
+        if filename:
+            identifier = filename
+        else:
+            identifier = f'#{self.device.key}'
+
+        result = f'{identifier}: {gigi_bytes(self.freespace):.1f}/{gigi_bytes(self.capacity):.1f} GiB'
+
+        if self.guests:
+            result += f' ('
+            for i, guest in enumerate(self.guests):
+                if i > 0:
+                    result += ', '
+                result += VmDisks._get_guest_summary(guest)
+            result += ')'
+        return result
 
 #endregion
 
 
 #region NICs
 
-def analyze_nics(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: str = DEFAULT_OUT, top: int = None):
+def list_vm_nics(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: str = _DEFAULT_OUT, top: int = None):
     """
     Analyze VM network interfaces.
     """
     nics_per_vm_headers = [
         'vm',
         'power_state',
-        'os_info',
         'os_family',
-        'os_name',
+        'os_version',
         'device_networks',
         'guest_networks',
         'with_mappings',
         'without_mappings',
         'mapped_guest',
         'unmapped_guest',
         'issues',
     ]
 
     nics_headers = [
         'vm',
         'power_state',
-        'os_info',
         'os_family',
-        'os_name',
+        'os_version',
         'backing',
         'network',
         'address_type',
         'key',
         'mac',
         'guests_ips',
         'guests_network_name',
     ]
     
-    with (out_table(out, title='nics', headers=nics_headers, dir=vcenter.get_out_dir()) as t_nics,
-          out_table(out, title='nics_per_vm', headers=nics_per_vm_headers, dir=vcenter.get_out_dir()) as t_nics_per_vm):
+    with (out_table(out, title='vm_nics', headers=nics_headers, dir=vcenter.get_out_dir(), env=vcenter.env) as t_nics,
+          out_table(out, title='vm_nics_per_vm', headers=nics_per_vm_headers, dir=vcenter.get_out_dir(), env=vcenter.env) as t_nics_per_vm):
         
         for i, vm in enumerate(vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key)):
             if top is not None and i == top:
                 break
             
             try:
-                logger.info(f"Analyze {vm.name} nics")
+                logger.info(f"Analyze vm {vm.name} nics")
 
                 info = extract_nics(vm, vcenter=vcenter)
 
-                os = dictify_value(vm.config.extraConfig).get('guestOS.detailed.data')
-                if not os:
-                    os = {}
-                os_family = os.get('familyName')
-                os_name = os.get('prettyName')
+                extra_config = dictify_value(vm.config.extraConfig)
+                os_family = get_os_family(extra_config, vm.config.guestFullName)
+                os_version = get_os_version(extra_config)
 
                 mapped_guests: list[vim.vm.GuestInfo.NicInfo] = []
                 for nic in info.nics:
                     for guest in nic.guests:
                         mapped_guests.append(guest)
 
                 t_nics_per_vm.append([
                     vm.name, # vm
                     vm.runtime.powerState, # power_state
-                    vm.config.guestFullName, # os_info
-                    os_family, # os_family
-                    os_name, # os_name
+                    os_family,
+                    os_version,
                     len(info.nics), # 'device_networks',
                     len(mapped_guests) + len(info.unmapped_guests), # 'guest_networks',
                     len(mapped_guests), # 'with_mappings',
                     len(info.unmapped_guests), # 'without_mappings',
                     [guest.macAddress for guest in mapped_guests], # 'mapped_guest',
                     [guest.macAddress for guest in info.unmapped_guests], # 'unmapped_guests',
                     info.issues,
@@ -568,33 +989,31 @@
                         for ip in guest.ipAddress:
                             ip_addresses.append(ip)
                         networks.append(guest.network)
                     
                     t_nics.append([
                         vm.name, # vm
                         vm.runtime.powerState, # power_state
-                        vm.config.guestFullName, # os_info
-                        os_family, # os_family
-                        os_name, # os_name
+                        os_family,
+                        os_version,
                         backing_typename, # backing
                         network,
                         nic.device.addressType, # address_type
                         nic.device.key, # key
                         nic.device.macAddress.lower(), # mac
                         ip_addresses,
                         networks,
                     ])
 
                 for guest in info.unmapped_guests:
                     t_nics.append([
                         vm.name, # vm
                         vm.runtime.powerState, # power_state
-                        vm.config.guestFullName, # os_info
-                        os_family, # os_family
-                        os_name, # os_name
+                        os_family,
+                        os_version,
                         None, # backing
                         None, # network
                         None, # address_type
                         guest.deviceConfigId, # key
                         guest.macAddress.lower(), # mac
                         guest.ipAddress,
                         guest.network,
@@ -605,17 +1024,17 @@
 
 
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('search', nargs='*', help="Search term(s).")
     parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
     parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
     parser.add_argument('--top', type=int)
-    parser.add_argument('-o', '--out', default=DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
 
-analyze_nics.add_arguments = _add_arguments
+list_vm_nics.add_arguments = _add_arguments
 
 
 def extract_nics(vm: vim.VirtualMachine, *, vcenter: VCenterClient):
     info = VmNics(vm)
 
     # Retrieve nic devices
     nics_per_key: dict[int,VmNic] = {}
@@ -683,48 +1102,67 @@
             yield guest
 
     @property
     def network_names(self):
         names = set()
 
         for nic in self.nics:
-            network = nic.network
-            if isinstance(network, dict):
-                if 'switch' in network:
-                    network['switch'] = network['switch'].name
-                name = ', '.join(f'{key}: {value}' for key, value in network.items())
-            elif network:
-                name = network.name
-            else:
-                name = None
-
+            name = nic.network_name
             if name:
                 names.add(name)
 
         return sorted(names)      
     
     def to_dict(self):
         data = []
 
-        for disk in self.nics:
-            data.append(disk.to_dict())
+        for nic in self.nics:
+            data.append(nic.to_dict())
 
         if self.unmapped_guests:
             for guest in self.unmapped_guests:
                 data.append({'key': guest.deviceConfigId, 'mac': guest.macAddress.lower(), 'guest':  self._get_guest_dict(guest)})
 
         return data
     
+    def to_summary(self, ip_version: int = None):
+        result = ''
+        
+        for nic in self.nics:
+            result += (' | ' if result else '') + nic.to_summary(ip_version=ip_version)
+
+        if self.unmapped_guests:
+            for guest in self.unmapped_guests:
+                result += (' | ' if result else '') + f"unmapped {guest.macAddress.lower()}: {guest.network} (" + VmNics._get_guest_summary(guest, ip_version=ip_version) + ")"
+
+        return result
+    
     @classmethod
     def _get_guest_dict(cls, guest: vim.vm.GuestInfo.NicInfo):
         data = {}
-        data['connected'] = guest.connected
         data['ips'] = guest.ipAddress
+        data['connected'] = guest.connected
         data['network_name'] = guest.network
         return data
+    
+    @classmethod
+    def _get_guest_summary(cls, guest: vim.vm.GuestInfo.NicInfo, ip_version: int = None):        
+        ip_addresses: list[IPv4Address|IPv6Address] = []
+        for ip_str in guest.ipAddress:
+            ip = ip_address(ip_str)
+            if ip_version is None or ip.version == ip_version:
+                ip_addresses.append(ip)
+
+        ip_addresses.sort()
+                
+        result = ''
+        for ip in ip_addresses:
+            result += (', ' if result else '') + ip.compressed
+        result += (', ' if result else '') + ('connected' if guest.connected else 'notConnected')
+        return result
 
 
 class VmNic:
     def __init__(self, device: vim.vm.device.VirtualEthernetCard, *, vcenter: VCenterClient):
         self.vcenter = vcenter
         self.device = device
         self.guests: list[vim.vm.GuestInfo.NicInfo] = []
@@ -743,14 +1181,31 @@
                     return {'switch': switch_obj, 'port': port_key}
                 else:
                     return {'switch_uuid': connection_obj.switchUuid, 'port': port_key}
         elif isinstance(self.device.backing, vim.vm.device.VirtualEthernetCard.NetworkBackingInfo):
             return self.device.backing.network
         else:
             return None
+        
+    @property
+    def network_name(self):
+        network = self.network
+        if not network:
+            return None
+        elif isinstance(network, (vim.dvs.DistributedVirtualPortgroup, vim.Network)):
+            return network.name
+        elif isinstance(network, dict):
+            result = ''
+            for key, value in network.items():
+                if isinstance(value, vim.ManagedEntity):
+                    value = value.name
+                result += (', ' if result else '') + f"{key}: {value}"
+            return str(network)
+        else:
+            return str(network)
 
     def to_dict(self):
         data = {}
         data['key'] = self.device.key
         data['mac'] = self.device.macAddress.lower()
 
         # vim.vm.device.VirtualEthernetCard.NetworkBackingInfo, vim.vm.device.VirtualEthernetCard.DistributedVirtualPortBackingInfo, etc
@@ -768,9 +1223,142 @@
 
         data['address_type'] = self.device.addressType
 
         if self.guests:
             data['guests'] = [VmNics._get_guest_dict(guest) for guest in self.guests]
         
         return data
+    
+    def to_summary(self, ip_version: int = None):
+        result = f"{self.device.macAddress.lower()}: {self.network_name}"
+        if self.guests:
+            result += " ("
+            for i, guest in enumerate(self.guests):
+                if i > 0:
+                    result += ', '
+                result += VmNics._get_guest_summary(guest, ip_version=ip_version)
+            result += ")"
+        return result
 
 #endregion
+
+
+def get_tools_version_number(toolsversion: str):
+    if re.match(r'^\d+$', toolsversion):
+        toolsversion = int(toolsversion)
+        if toolsversion == 0 or toolsversion == 2147483647:
+            return None
+        return toolsversion    
+    elif toolsversion:
+        return str(toolsversion)
+    else:
+        return None
+
+
+def get_os_family(extra_config: dict, configured_fullname: str):
+    def get_family_from_configured(fullname: str):
+        if m := re.match(r'^(.+) \(\d\d\-bit\)$', fullname):
+            fullname = m[1]
+            
+        lower_fullname = fullname.lower()
+        if 'windows' in lower_fullname:
+            return "Windows"
+        elif 'linux' in lower_fullname or 'centos' in lower_fullname:
+            return "Linux"
+        elif lower_fullname == 'other':
+            return None
+        else:
+            return fullname
+      
+    if 'guestInfo.detailed.data' in extra_config:
+        line = extra_config['guestInfo.detailed.data']
+        if m := re.match(r".*familyName='([^']+)'.*", line):
+            return m[1]
+    elif 'guestOS.detailed.data' in extra_config:
+        data = extra_config.get("guestOS.detailed.data")
+        if isinstance(data, dict) and 'familyName' in data:
+            return data['familyName']
+
+    if configured_fullname:
+        return get_family_from_configured(configured_fullname)
+
+
+
+def get_os_version(extra_config: dict):
+    if 'guestInfo.detailed.data' in extra_config:
+        line = extra_config['guestInfo.detailed.data']
+        if m := re.match(r".*prettyName='([^']+)'.*", line):
+            return m[1]
+        else:
+            return line
+    elif 'guestOS.detailed.data' in extra_config:
+        data = extra_config.get("guestOS.detailed.data")
+        if isinstance(data, dict) and 'prettyName' in data:
+            return data['prettyName']
+        else:
+            return str(data)
+    else:
+        return None
+
+
+def get_os_distro_version(extra_config: dict):
+    if 'guestInfo.detailed.data' in extra_config:
+        line = extra_config['guestInfo.detailed.data']
+        if m := re.match(r".*distroVersion='([^']+)'.*", line):
+            return m[1]
+    if 'guestOS.detailed.data' in extra_config:
+        data = extra_config.get("guestOS.detailed.data")
+        if isinstance(data, dict) and 'distroVersion' in data:
+            return data['distroVersion']
+
+
+def get_os_kernel_version(extra_config: dict):
+    if 'guestInfo.detailed.data' in extra_config:
+        line = extra_config['guestInfo.detailed.data']
+        if m := re.match(r".*kernelVersion='([^']+)'.*", line):
+            return m[1]
+    if 'guestOS.detailed.data' in extra_config:
+        data = extra_config.get("guestOS.detailed.data")
+        if isinstance(data, dict) and 'kernelVersion' in data:
+            return data['kernelVersion']
+        
+
+def get_guestinfo_publish_time(extra_config: dict):
+    if not 'guestinfo.appInfo' in extra_config:
+        return
+    
+    appinfo_str = extra_config['guestinfo.appInfo']
+    if not isinstance(appinfo_str, str):
+        return str(appinfo_str)
+    
+    if appinfo_str == "":
+        return
+    
+    try:
+        appinfo = json.loads(appinfo_str)
+    except json.decoder.JSONDecodeError as err:
+        return f"Cannot parse \"{appinfo_str}\": {err}"
+
+    if 'publishTime' in appinfo:
+        return datetime.fromisoformat(appinfo['publishTime'])
+
+
+def get_tools_version(extra_config: dict, version_number: str):
+    if 'guestinfo.vmtools.versionNumber' in extra_config and 'guestinfo.vmtools.description' in extra_config:
+        if extra_config['guestinfo.vmtools.versionNumber'] == version_number:
+            return extra_config['guestinfo.vmtools.description']
+
+
+def get_custom_values(vm: vim.VirtualMachine):
+    available_fields = {}
+    custom_values = {}
+
+    for field in vm.availableField:
+        available_fields[field.key] = field.name
+
+    for value in vm.value:
+        custom_values[available_fields[value.key]] = value.value
+        
+    for value in vm.customValue:
+        custom_values[available_fields[value.key]] = value.value
+
+    return custom_values
```

## Comparing `vmware_reporter-0.2.1.dist-info/LICENSE.txt` & `vmware_reporter-0.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `vmware_reporter-0.2.1.dist-info/METADATA` & `vmware_reporter-0.3.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vmware-reporter
-Version: 0.2.1
+Version: 0.3.0
 Summary: Interact easily with your VMWare clusters.
 Author-email: Sébastien Hocquet <dev@ipamo.net>
 Project-URL: Homepage, https://github.com/ipamo/vmware-reporter
 Project-URL: Bug Tracker, https://github.com/ipamo/vmware-reporter/issues
 Keywords: vmware,vsphere,vm,reporter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: reporter-utils
+Requires-Dist: zut[commons] >=0.9.2
 Requires-Dist: pyvmomi
 Requires-Dist: requests
 
 VMWare-reporter
 ===============
 
 Interact easily with your VMWare clusters.
@@ -32,24 +32,42 @@
 ```sh
 pip install vmware-reporter
 ```
 
 
 ## Configuration
 
-Create file `C:\Users\$USER\AppData\Local\vmware-reporter\vmware-reporter.conf` (`/home/$USER/.config/vmware-reporter/vmware-reporter.conf` on Linux). Example:
+Create file `C:\Users\$USER\AppData\Local\vmware-reporter\vmware-reporter.conf` (`/home/$USER/.config/vmware-reporter/vmware-reporter.conf` on Linux).
+
+Example:
 
 ```ini
 [vmware-reporter]
 host = myvcenter.example.org
 user = reporter@vsphere.local
 password = ...
 no_ssl_verify = True
 ```
 
+Several environments may be distinguished. Example for two environments named `ENV1` and `ENV2`:
+
+```ini
+[vmware-reporter:ENV1]
+host = myvcenter.env1.example.org
+user = reporter@vsphere.local
+password = ...
+no_ssl_verify = True
+
+[vmware-reporter:ENV2]
+host = myvcenter.env2.example.org
+user = reporter@vsphere.local
+password = ...
+no_ssl_verify = True
+```
+
 
 ## Usage examples
 
 See also [full documentation](https://ipamo.net/vmware-reporter) (including [API reference](https://ipamo.net/vmware-reporter/latest/api-reference.html)).
 
 VMWare-reporter may be used as a library in your Python code:
 
@@ -70,14 +88,26 @@
 
 - Export all available information about VMWare managed objects to JSON files:
 
 ```sh
 vmware-reporter dump
 ```
 
+- Reconfigure VMs (mass operation): copy template [vms_reconfigure.xlsx](https://ipamo.net/vmware-reporter/latest/_static/templates/vms_reconfigure.xlsx) to `data/vms_reconfigure.xlsx`, fill-in this file, then:
+
+```sh
+vmware-reporter vm reconfigure
+```
+
+- If you use several environments, put files in `data/ENV1/` instead of `data/` and specify environment on the command line. Example:
+
+```sh
+vmware-reporter -e ENV1 vm reconfigure
+```
+
 Complete help about command-line usage may be displayed by typing:
 
 ```sh
 vmware-reporter --help
 ```
```

## Comparing `vmware_reporter-0.2.1.dist-info/RECORD` & `vmware_reporter-0.3.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-vmware_reporter/__init__.py,sha256=CRiHWqdhR6L0AVO9oiHHq1eK-J7J6KfCajHDEu4Hnkg,17494
-vmware_reporter/__main__.py,sha256=sa0IIK20o46T8AtiH6Hk3BIP6BQ0mn45DVjxAMox1c8,3302
-vmware_reporter/_version.py,sha256=ZX5om7Ovkz6dOhGLYm2Tr_wCABow6rirLhSHdYiHgpk,427
-vmware_reporter/datastore.py,sha256=gfNgh56wsPIP3YRU0wujN44pgYJwGpvjNMGrOYiSjIs,17592
-vmware_reporter/dump.py,sha256=jxLKRSNiYwt2Y4KDYLZ-E0Msdrxo5P49xmSI1UhtOe8,2482
-vmware_reporter/extract.py,sha256=8vQiYmdIOgAS0mosmQ3lv2kvdX_MJVjcBQsEH4gCpUY,5265
-vmware_reporter/inspect.py,sha256=zui_U7u9w0t3Jmf6SJSuqrNXOZDEEKNDhOvGiFaaZOI,8916
-vmware_reporter/inventory.py,sha256=6cF4StyNkqYPPJGeZAQ-x_8oSgo1SabXb2b8T9DP3qU,7900
-vmware_reporter/networking.py,sha256=uReP1HvWBKbKoEn5mX-Smtt-U9uVlxw6Nycvcubbz0M,5129
-vmware_reporter/vm.py,sha256=57R-gchEh5Axy0gm9oA2dlfwY_v1z_CBg4PMVPHwjdg,31721
-vmware_reporter/config/extractions/host.yml,sha256=yMXT4cJru1a84rqLYOTT6EpcreNmY_ukTKbtIv5xneo,705
-vmware_reporter/config/extractions/vm.yml,sha256=dUU89TGM3eEumVYtbYITMcQq-t_ZgojgOPnrrRLm3vM,1467
-vmware_reporter-0.2.1.dist-info/LICENSE.txt,sha256=GIOy7i81R9zaxGmerWRrvgsSukOj10VspxRwsEWtlCY,1098
-vmware_reporter-0.2.1.dist-info/METADATA,sha256=kaVLbZRTN5RB-p4HM4TtHC7CZX4wHStpsVkoebY0GX8,2602
-vmware_reporter-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-vmware_reporter-0.2.1.dist-info/entry_points.txt,sha256=Sd7R6PmUzLkJr4eez7nM8-z6yISX2pb3Dc8mnXDuguM,66
-vmware_reporter-0.2.1.dist-info/top_level.txt,sha256=uBrhSJjB5QxsyeQKqRdCv8l6JOmXKhnfPKnetEEAqso,16
-vmware_reporter-0.2.1.dist-info/RECORD,,
+vmware_reporter/__init__.py,sha256=qRQcQQxnfr6UjXYaTAvd_JIIxrMA7Q8Re4u9BzpyKXI,31153
+vmware_reporter/__main__.py,sha256=KjoRljGbAPbNyWcMA2BdVcOo8b9Ne5lHr7iNK1La874,3466
+vmware_reporter/_version.py,sha256=MQTeK44Cj4PxMB5VTeNSrMxwkURTN6SjVTQLlqfFFH8,427
+vmware_reporter/autoreport.py,sha256=3zkwSC6gPgoj0oAQ7b0pTFV-zELIqVzsQ2NF4NTBhMU,1447
+vmware_reporter/customfield.py,sha256=JLvG3El-IGihWHbS7Rtj-FAG7BLj962RZ11W8pIbCls,844
+vmware_reporter/datastore.py,sha256=xR_Xn0uE35ZaEolkCg5epLJGmG003NjWjsv7Ffx6sUc,18826
+vmware_reporter/dump.py,sha256=eS_aYOO-ac0uuePdbjWp2tOaCrXvDB073lVmK040VsM,2547
+vmware_reporter/host.py,sha256=sz5Bq7A5vIMk-7cC0QpHzMm-hUZf29z8-VHG7Rnb_50,4034
+vmware_reporter/inventory.py,sha256=hYV5xryl1bbfb84qLCw_OmwYePkEl4Gjsm8VceZCXK4,7968
+vmware_reporter/net.py,sha256=w0iTS3u6mpGTZseK1eOokz1gx47kKI4XthHnvFyxZVY,5971
+vmware_reporter/settings.py,sha256=TDs4bXPO7nGg46nZHvNFJHsavQgQyuG7NBRgeJAWVtQ,235
+vmware_reporter/vm.py,sha256=1XdOhGHOr105v-2wWOLJAiDFlF2MQ8OIweKE8a3VCF0,54717
+vmware_reporter-0.3.0.dist-info/LICENSE.txt,sha256=GIOy7i81R9zaxGmerWRrvgsSukOj10VspxRwsEWtlCY,1098
+vmware_reporter-0.3.0.dist-info/METADATA,sha256=j8qBGUO0Z2Xkg0wafvMtU9KHZOAdyIcaH30zOOPxJIo,3435
+vmware_reporter-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+vmware_reporter-0.3.0.dist-info/entry_points.txt,sha256=Sd7R6PmUzLkJr4eez7nM8-z6yISX2pb3Dc8mnXDuguM,66
+vmware_reporter-0.3.0.dist-info/top_level.txt,sha256=uBrhSJjB5QxsyeQKqRdCv8l6JOmXKhnfPKnetEEAqso,16
+vmware_reporter-0.3.0.dist-info/RECORD,,
```

