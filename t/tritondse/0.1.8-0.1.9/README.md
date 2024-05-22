# Comparing `tmp/tritondse-0.1.8.tar.gz` & `tmp/tritondse-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritondse-0.1.8.tar", last modified: Fri Aug  4 21:30:40 2023, max compression
+gzip compressed data, was "tritondse-0.1.9.tar", last modified: Thu Dec 28 16:55:26 2023, max compression
```

## Comparing `tritondse-0.1.8.tar` & `tritondse-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:30:40.095861 tritondse-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 21:30:37.000000 tritondse-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-04 21:30:40.095861 tritondse-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-08-04 21:30:37.000000 tritondse-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:30:40.095861 tritondse-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-04 21:30:37.000000 tritondse-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:30:40.095861 tritondse-0.1.8/tritondse/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    36167 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29299 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/heap_allocator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:30:40.095861 tritondse-0.1.8/tritondse/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/loaders/cle_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/loaders/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/loaders/quokkaprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    22880 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:30:40.095861 tritondse-0.1.8/tritondse/probes/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/probes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/probes/basic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    52429 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/process_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/qbdi_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    75406 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/sanitizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)    18644 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/seeds_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/symbolic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/symbolic_explorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/thread_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/worklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-08-04 21:30:37.000000 tritondse-0.1.8/tritondse/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:30:40.095861 tritondse-0.1.8/tritondse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-04 21:30:40.000000 tritondse-0.1.8/tritondse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-04 21:30:40.000000 tritondse-0.1.8/tritondse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:30:40.000000 tritondse-0.1.8/tritondse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-04 21:30:40.000000 tritondse-0.1.8/tritondse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 21:30:40.000000 tritondse-0.1.8/tritondse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 16:55:26.920555 tritondse-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-28 16:55:25.000000 tritondse-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2023-12-28 16:55:26.920555 tritondse-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2023-12-28 16:55:25.000000 tritondse-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 16:55:26.920555 tritondse-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2023-12-28 16:55:25.000000 tritondse-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 16:55:26.920555 tritondse-0.1.9/tritondse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36200 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7705 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29444 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/heap_allocator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 16:55:26.920555 tritondse-0.1.9/tritondse/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/loaders/cle_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9137 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/loaders/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/loaders/quokkaprogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22880 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 16:55:26.920555 tritondse-0.1.9/tritondse/probes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/probes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2033 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/probes/basic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52429 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/process_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/qbdi_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75406 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/routines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/sanitizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9452 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19003 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/seeds_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37955 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/symbolic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10547 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/symbolic_explorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/thread_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11611 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/worklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2023-12-28 16:55:25.000000 tritondse-0.1.9/tritondse/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 16:55:26.920555 tritondse-0.1.9/tritondse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2023-12-28 16:55:26.000000 tritondse-0.1.9/tritondse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2023-12-28 16:55:26.000000 tritondse-0.1.9/tritondse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 16:55:26.000000 tritondse-0.1.9/tritondse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-28 16:55:26.000000 tritondse-0.1.9/tritondse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-28 16:55:26.000000 tritondse-0.1.9/tritondse.egg-info/top_level.txt
```

### Comparing `tritondse-0.1.8/LICENSE` & `tritondse-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/PKG-INFO` & `tritondse-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritondse
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library of Dynamic Symbolic Exploration based the Triton library
 Home-page: https://github.com/quarkslab/tritondse
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/tritondse/
 Project-URL: Bug Tracker, https://github.com/quarkslab/tritondse/issues
 Project-URL: Source, https://github.com/quarkslab/tritondse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tritondse Version: 0.1.8 Summary: A library of
+Metadata-Version: 2.1 Name: tritondse Version: 0.1.9 Summary: A library of
 Dynamic Symbolic Exploration based the Triton library Home-page: https://
 github.com/quarkslab/tritondse Author: Quarkslab License: AGPL-3.0 Project-URL:
 Documentation, https://quarkslab.github.io/tritondse/ Project-URL: Bug Tracker,
 https://github.com/quarkslab/tritondse/issues Project-URL: Source, https://
 github.com/quarkslab/tritondse Classifier: Topic :: Security Classifier:
 Environment :: Console Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # TritonDSE
```

### Comparing `tritondse-0.1.8/README.md` & `tritondse-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/setup.py` & `tritondse-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md") as f:
     README = f.read()
 
 
 setup(
     name="tritondse",
-    version="0.1.8",
+    version="0.1.9",
     description="A library of Dynamic Symbolic Exploration based the Triton library",
     packages=find_packages(),
     long_description=README,
     long_description_content_type='text/markdown',
     url="https://github.com/quarkslab/tritondse",
     project_urls={
         "Documentation": "https://quarkslab.github.io/tritondse/",
```

### Comparing `tritondse-0.1.8/tritondse/__init__.py` & `tritondse-0.1.9/tritondse/__init__.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/arch.py` & `tritondse-0.1.9/tritondse/arch.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/callbacks.py` & `tritondse-0.1.9/tritondse/callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Callable, Tuple, List, Optional, Union, Any
 import enum_tools.documentation
 # third-party imports
 from triton import CALLBACK, Instruction, MemoryAccess, OPCODE
 
 # local imports
 from tritondse.process_state import ProcessState
-from tritondse.types import Addr, Input, Register, Expression, Edge, SymExType
+from tritondse.types import Addr, Input, Register, Expression, Edge, SymExType, AstNode
 from tritondse.thread_context import ThreadContext
 from tritondse.seed import Seed
 from tritondse.memory import MemoryAccessViolation
 import tritondse.logging
 
 logger = tritondse.logging.get()  # get root tritondse logger
 
@@ -53,15 +53,15 @@
 
 AddrCallback            = Callable[['SymbolicExecutor', ProcessState, Addr], None]
 ExplorationStepCallback = Callable[['SymbolicExplorator'], None]
 InstrCallback           = Callable[['SymbolicExecutor', ProcessState, Instruction], None]
 MemReadCallback         = Callable[['SymbolicExecutor', ProcessState, MemoryAccess], None]
 MemWriteCallback        = Callable[['SymbolicExecutor', ProcessState, MemoryAccess, int], None]
 MnemonicCallback        = Callable[['SymbolicExecutor', ProcessState, OPCODE], None]
-SymExSolvingCallback    = Callable[['SymbolicExecutor', ProcessState, Edge, SymExType], bool]
+SymExSolvingCallback    = Callable[['SymbolicExecutor', ProcessState, Edge, SymExType, AstNode, List[AstNode]], bool]
 BranchCoveredCallback   = Callable[['SymbolicExecutor', ProcessState, Edge], bool]
 NewInputCallback        = Callable[['SymbolicExecutor', ProcessState, Seed], Optional[Seed]]
 OpcodeCallback          = Callable[['SymbolicExecutor', ProcessState, bytes], None]
 RegReadCallback         = Callable[['SymbolicExecutor', ProcessState, Register], None]
 RegWriteCallback        = Callable[['SymbolicExecutor', ProcessState, Register, int], None]
 RtnCallback             = Callable[['SymbolicExecutor', ProcessState, str, Addr], Optional[Union[int, Expression]]]
 SymExCallback           = Callable[['SymbolicExecutor', ProcessState], None]
```

### Comparing `tritondse-0.1.8/tritondse/config.py` & `tritondse-0.1.9/tritondse/config.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/coverage.py` & `tritondse-0.1.9/tritondse/coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,18 +400,20 @@
                                 res = yield typ, pending_csts, p1, (addr, p2.evaluate()), i
                                 self.covered_symbolic_pointers.add(addr)  # add the pointer in covered regardless of result
                             else:
                                 logger.warning(f"memory constraint unexpected pattern: {pred}")
                         else:
                             logger.warning(f"memory constraint unexpected pattern: {pred}")
 
-                if BranchSolvingStrategy.SOUND_MEM_ACCESS in self.branch_strategy:
-                    pending_csts.append(pc)  # if sound add the mem dereference as a constraint in path predicate
-                    # NOTE: in both case the branch is not taken in account in the current_path_hash
+                    if BranchSolvingStrategy.SOUND_MEM_ACCESS in self.branch_strategy:
+                        pending_csts.append(pc)  # if sound add the mem dereference as a constraint in path predicate
+                        # NOTE: in both case the branch is not taken in account in the current_path_hash
 
+                else:  # Routines, or user-defined constraints thus add it all the time.
+                    pending_csts.append(pc)
 
     def _get_covitem(self, path_hash, branch: PathBranch) -> CovItem:
         src, dst = branch['srcAddr'], branch['dstAddr']
 
         # Check if the target is new with regards to the strategy
         if self.strategy == CoverageStrategy.BLOCK:
             return dst
```

### Comparing `tritondse-0.1.8/tritondse/exception.py` & `tritondse-0.1.9/tritondse/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,7 +32,16 @@
 
     * trying to allocate data which overflow heap size
     * trying to free a pointer already freed
     * trying to free a non-allocated pointer
     """
     def __init__(self, message):
         super(Exception, self).__init__(message)
+
+
+class ProbeException(Exception):
+    """
+    Exception to raise in a probe to stop the current exception.
+    It is caught by SymbolicExplorator.
+    """
+    def __init__(self, message):
+        super(Exception, self).__init__(message)
```

### Comparing `tritondse-0.1.8/tritondse/heap_allocator.py` & `tritondse-0.1.9/tritondse/heap_allocator.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/loaders/cle_loader.py` & `tritondse-0.1.9/tritondse/loaders/cle_loader.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/loaders/loader.py` & `tritondse-0.1.9/tritondse/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/loaders/program.py` & `tritondse-0.1.9/tritondse/loaders/program.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/loaders/quokkaprogram.py` & `tritondse-0.1.9/tritondse/loaders/quokkaprogram.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/logging.py` & `tritondse-0.1.9/tritondse/logging.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/memory.py` & `tritondse-0.1.9/tritondse/memory.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/probes/basic_trace.py` & `tritondse-0.1.9/tritondse/probes/basic_trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/process_state.py` & `tritondse-0.1.9/tritondse/process_state.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/qbdi_trace.py` & `tritondse-0.1.9/tritondse/qbdi_trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/routines.py` & `tritondse-0.1.9/tritondse/routines.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/sanitizers.py` & `tritondse-0.1.9/tritondse/sanitizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from triton import Instruction
 from tritondse.callbacks import CbType, ProbeInterface
 from tritondse.seed import Seed, SeedStatus
 from tritondse.types import Architecture, Addr, Tuple, SolverStatus
 from tritondse import SymbolicExecutor, ProcessState
+from tritondse.exception import ProbeException
 import tritondse.logging
 
 logger = tritondse.logging.get("sanitizers")
 
 
 
 def mk_new_crashing_seed(se, model) -> Seed:
@@ -125,16 +126,19 @@
         # page on déclenche ce sanitizer...
 
         # FIXME: Why do we call is_valid_memory_mapping ? It is not a "Null Deref vulnerability", it is more a segmentation error
         if ptr == 0 or (pstate.memory.segmentation_enabled and not pstate.memory.is_mapped(ptr)):
             if description:
                 logger.critical(description)
             se.seed.status = SeedStatus.CRASH
-            pstate.stop = True
-            return True
+
+            # An exception is needed here to break execution on the first
+            # invalid memory access. Otherwise, the memory access callback
+            # will report on all bytes.
+            raise ProbeException(description)
 
         return False
 
     @staticmethod
     def _memory_read(se, pstate, mem):
         return NullDerefSanitizer.check(se, pstate, mem.getAddress(), f'Invalid memory access when reading at {mem} from {pstate.current_instruction}')
```

### Comparing `tritondse-0.1.8/tritondse/seed.py` & `tritondse-0.1.9/tritondse/seed.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     At the end of a :py:obj:`SymbolicExecutor` run one of these
     status must have set to the seed.
     """
     NEW = 0      # doc: The input seed is new (has not been executed yet)
     OK_DONE = 1  # doc: The input seed has been executed and terminated correctly
     CRASH = 2    # doc: The input seed crashed in some ways
     HANG = 3     # doc: The input seed made the program to hang
+    FAIL = 4     # doc: The input seed made the symbolic executor to raise an exception
 
 
 @enum_tools.documentation.document_enum
 class SeedFormat(Enum):
     """
     Seed format enum
     Raw seeds are just bytes Seed(b"AAAAA\x00BBBBB")
```

### Comparing `tritondse-0.1.8/tritondse/seeds_manager.py` & `tritondse-0.1.9/tritondse/seeds_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         else:
             self.worklist = seed_scheduler_class(self)
         self.cbm = callback_manager
 
         self.corpus = set()
         self.crash = set()
         self.hangs = set()
+        self.fails = set()
 
         self.__load_seed_workspace()
 
         self._solv_count = 0
         self._solv_time_sum = 0
         self._solv_status = {SolverStatus.SAT: 0, SolverStatus.UNSAT: 0, SolverStatus.UNKNOWN: 0, SolverStatus.TIMEOUT: 0}
         self._stat_branch_reverted = Counter()
@@ -78,27 +79,30 @@
             self.hangs.add(seed)
         # Load crashes
         for seed in self.workspace.iter_crashes():
             self.crash.add(seed)
         # Load worklist
         for seed in self.workspace.iter_worklist():
             self.worklist.add(seed)
+        # Load fails
+        for seed in self.workspace.iter_fails():
+            self.fails.add(seed)
 
     def is_new_seed(self, seed: Seed) -> bool:
         """
-        Check if a seed is a new one (not into corpus, crash and hangs)
+        Check if a seed is a new one (not into corpus, crash, hangs and fails)
 
         :param seed: The seed to test
         :type seed: Seed
         :return: True if the seed is a new one
 
         .. warning:: That function does not check that the seed
                      is not in the pending seeds queue
         """
-        return sum(seed in x for x in [self.corpus, self.crash, self.hangs]) == 0
+        return sum(seed in x for x in [self.corpus, self.crash, self.hangs, self.fails]) == 0
 
     def add_seed_queue(self, seed: Seed) -> None:
         """
         Add a seed to to appropriate internal queue depending
         on its status. If it is new it is added in pending seed,
         if OK, HANG or CRASH it the appropriate set.
         **Note that the seed is not written in the workspace**
@@ -111,14 +115,16 @@
             self.worklist.add(seed)
         elif seed.status == SeedStatus.OK_DONE:
             self.corpus.add(seed)
         elif seed.status == SeedStatus.HANG:
             self.hangs.add(seed)
         elif seed.status == SeedStatus.CRASH:
             self.crash.add(seed)
+        elif seed.status == SeedStatus.FAIL:
+            self.fails.add(seed)
         else:
             assert False
 
     def post_execution(self, execution: SymbolicExecutor, seed: Seed, solve_new_path: int = True) -> float:
         """
         Function called after each execution. It updates the global
         code coverage object, and tries to generate new paths through
@@ -155,15 +161,15 @@
                 logger.warning(f"dropping enqueued seed: {s.hash} (already seen)")
 
         # Update the current seed queue
         if seed.status == SeedStatus.NEW:
             logger.error(f"seed not meant to be NEW at the end of execution ({seed.hash}) (dropped)")
             self.drop_seed(seed)
 
-        elif seed.status in [SeedStatus.HANG, SeedStatus.CRASH]:
+        elif seed.status in [SeedStatus.HANG, SeedStatus.CRASH, SeedStatus.FAIL]:
             self.archive_seed(seed)
             # NOTE: Do not perform further processing on the seed (like generating inputs from it)
 
         elif seed.status == SeedStatus.OK_DONE:
             if self.coverage.can_improve_coverage(execution.coverage) or self.coverage.can_cover_symbolic_pointers(execution):
                 items = self.coverage.new_items_to_cover(execution.coverage)
                 seed.coverage_objectives = items  # Set its new objectives
@@ -224,23 +230,25 @@
                     break
 
                 typ, p_prefix, branch, covitem, ith = path_generator.send(status)
 
                 # Create edge in case of conditional branch, for all the other the edge shall be already set
                 edge = (branch['srcAddr'], branch['dstAddr']) if typ == SymExType.CONDITIONAL_JMP else covitem
 
+                # Add path_prefix in path predicate (regardless on whether we solve the item or not)
+                path_predicate.extend(x.getTakenPredicate() for x in p_prefix)
+
+                expr = branch['constraint'] if typ == SymExType.CONDITIONAL_JMP else branch
+
                 # Call on_branch_solving, if one replies False does not solve the branch
                 if self.cbm is not None:
-                    cb_result = all(cb(execution, execution.pstate, edge, typ) for cb in self.cbm.get_on_solving_callback())
+                    cb_result = all(cb(execution, execution.pstate, edge, typ, expr, path_predicate) for cb in self.cbm.get_on_solving_callback())
                 else:
                     cb_result = True
 
-                # Add path_prefix in path predicate (regardless on whether we solve the item or not)
-                path_predicate.extend(x.getTakenPredicate() for x in p_prefix)
-
                 # Skip processing the current path in case the result of the
                 # callbacks return False.
                 if not cb_result:
                     status = None
                     continue
 
                 # Create the constraint
```

### Comparing `tritondse-0.1.8/tritondse/symbolic_executor.py` & `tritondse-0.1.9/tritondse/symbolic_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # built-in imports
 import io
 import time
 import os
-import resource
+
+if os.name == 'posix':
+    import resource
+
 from typing import Optional, Union, List, NoReturn, Dict, Type
 
 # third party imports
 from triton import MODE, Instruction, CPUSIZE, MemoryAccess, CALLBACK
 
 # local imports
 from tritondse.config import Config
@@ -16,15 +19,15 @@
 from tritondse.seed import Seed, SeedStatus, SeedFormat, CompositeData
 from tritondse.types import Expression, Architecture, Addr, Model, SymbolicVariable, Register
 from tritondse.routines import SUPPORTED_ROUTINES, SUPORTED_GVARIABLES
 from tritondse.callbacks import CallbackManager
 from tritondse.workspace import Workspace
 from tritondse.heap_allocator import AllocatorException
 from tritondse.thread_context import ThreadContext
-from tritondse.exception import AbortExecutionException, SkipInstructionException, StopExplorationException
+from tritondse.exception import AbortExecutionException, SkipInstructionException, StopExplorationException, ProbeException
 from tritondse.memory import MemoryAccessViolation, Perm
 import tritondse.logging
 
 logger = tritondse.logging.get("executor")
 
 
 class SymbolicExecutor(object):
@@ -59,15 +62,15 @@
         self.seed: Seed = seed  #: The current seed used for the execution
 
         # Override config if there is a mismatch between seed format and config file
         if seed.format != self.config.seed_format:
             logger.warning(f"seed format {seed.format} mismatch config {config.seed_format} (override config)")
             self.config.seed_format = seed.format
 
-        self._symbolic_seed = self._init_symbolic_seed(seed)
+        self.symbolic_seed = self._init_symbolic_seed(seed) #: symbolic seed (same structure than Seed but with symbols)
 
         self.coverage: CoverageSingleRun = CoverageSingleRun(self.config.coverage_strategy)  #: Coverage of the execution
         self.rtn_table = dict()   # Addr -> Tuple[fname, routine]
         self.uid: int = uid       #: Unique identifier meant to unique accross Exploration instances
         self.start_time: int = 0  #: start time of the process
         self.end_time: int = 0    #: end time of the process
 
@@ -183,18 +186,18 @@
     def is_seed_injected(self) -> bool:
         """
         Get whether or not the seed has been injected.
 
         :return: True if the seed has already been inserted
         """
         if self.config.is_format_raw():
-            return bool(self._symbolic_seed)
+            return bool(self.symbolic_seed)
         elif self.config.is_format_composite():
             # Namely has one of the various input been injected or not
-            return bool(self._symbolic_seed.content.files) or bool(self._symbolic_seed.content.variables)
+            return bool(self.symbolic_seed.content.files) or bool(self.symbolic_seed.content.variables)
         else:
             assert False
 
     def _configure_pstate(self) -> None:
         #for mode in [MODE.ALIGNED_MEMORY, MODE.AST_OPTIMIZATIONS, MODE.CONSTANT_FOLDING, MODE.ONLY_ON_SYMBOLIZED]:
         for mode in [MODE.ONLY_ON_SYMBOLIZED]:
             self.pstate.set_triton_mode(mode, True)
@@ -325,21 +328,22 @@
 
             # Process
             prev_pc = self.current_pc
             self._in_processing = True
             if not self.pstate.process_instruction(instruction):
                 if self.pstate.is_halt_instruction():
                     logger.info(f"hit {str(instruction)} instruction stop.")
+                    return False
                 else:
                     logger.error('Instruction not supported: %s' % (str(instruction)))
+                    if self.config.skip_unsupported_instruction:
+                        self.pstate.cpu.program_counter += instruction.getSize() # try to jump over the instruction
+                    else:
+                        return False  # stop emulation
 
-                if self.config.skip_unsupported_instruction:
-                    self.pstate.cpu.program_counter += instruction.getSize() # try to jump over the instruction
-                else:
-                    return False  # stop emulation
             self._in_processing = False
             # increment trace offset
             self.trace_offset += 1
 
             # update previous program counters
             self.previous_pc = prev_pc
             self.current_pc = self.pstate.cpu.program_counter  # current_pc becomes new instruction pointer
@@ -400,22 +404,28 @@
 
             # Check timeout of the execution
             if self.config.execution_timeout and (time.time() - self.start_time) >= self.config.execution_timeout:
                 logger.info('Timeout of an execution reached')
                 self.seed.status = SeedStatus.HANG
                 return False
             return True
-        except AbortExecutionException as e:
-            return False
-        except MemoryAccessViolation as e:
-            logger.warning(f"Memory violation: {str(e)}")
 
             # Call all the callbacks on the memory violations
             for cb in self.callback_manager.get_memory_violation_callbacks():
                 cb(self, self.pstate, e)
+        except AbortExecutionException as e:
+            return False
+        except MemoryAccessViolation as e:
+            logger.warning(f"Memory violation: {str(e)}")
+        except ProbeException:
+            return False
+        except Exception as e:
+            logger.warning(f"Execution interrupted: {e}")
+            self.seed.status = SeedStatus.FAIL
+            return False
 
             # Assign the seed the status of crash
             if not self.seed.is_status_set():
                 self.seed.status = SeedStatus.CRASH
             return False
 
 
@@ -667,65 +677,72 @@
         is simply the concrete value of the register
         marked as return_register (rax, on x86, r0 on ARM..)
         """
         return self.pstate.read_register(self.pstate.return_register) & 0xFF
 
     @staticmethod
     def mem_usage_str() -> str:
-        """ debug function to track memory consumption of an execution """
-        size, resident, shared, _, _, _, _ = (int(x) for x in open(f"/proc/{os.getpid()}/statm").read().split(" "))
-        resident = resident * resource.getpagesize()
-        units = [(float(1024), "Kb"), (float(1024 **2), "Mb"), (float(1024 **3), "Gb")]
-        for unit, s in units[::-1]:
-            if resident / unit < 1:
-                continue
-            else:  # We are on the right unit
-                return "%.2f%s" % (resident/unit, s)
-        return "%dB" % resident
+        """
+        Debug function to track memory consumption of an execution (not
+        implemented on Windows).
+        """
+        if os.name == "posix":
+            size, resident, shared, _, _, _, _ = (int(x) for x in open(f"/proc/{os.getpid()}/statm").read().split(" "))
+            resident = resident * resource.getpagesize()
+            units = [(float(1024), "Kb"), (float(1024 **2), "Mb"), (float(1024 **3), "Gb")]
+            for unit, s in units[::-1]:
+                if resident / unit < 1:
+                    continue
+                else:  # We are on the right unit
+                    return "%.2f%s" % (resident/unit, s)
+            return "%dB" % resident
+        else:
+          return "N/A"
 
     def mk_new_seed_from_model(self, model: Model) -> Seed:
         """
         Creates a new seed from the given SMT model.
 
         :param model: SMT model
         :return: new seed object
         """
         def repl_bytearray(concrete, symbolic):
             for i, sv in enumerate(symbolic):  # Enumerate symvars associated with each bytes
                 if sv is not None:
                     if sv.getId() in model:  # If solver provided a new value for the symvar
-                        concrete[i] = model[sv.getId()].getValue()  # Replace it in the bytearray
+                        value = model[sv.getId()].getValue()
+                        concrete[i] = value # Replace it in the bytearray
             return concrete
 
         if self.config.is_format_raw(): # RAW seed. => symbolize_stdin
-            content = bytes(repl_bytearray(bytearray(self.seed.content), self._symbolic_seed))
+            content = bytes(repl_bytearray(bytearray(self.seed.content), self.symbolic_seed))
 
         elif self.config.is_format_composite():
             # NOTE will have to update this if more things are added to CompositeData
             new_files, new_vars = {}, {}
 
             # Handle argv (its meant to be here)
             args = [bytearray(x) for x in self.seed.content.argv]
-            new_argv = [bytes(repl_bytearray(c, s)) for c, s in zip(args, self._symbolic_seed.argv)]
+            new_argv = [bytes(repl_bytearray(c, s)) for c, s in zip(args, self.symbolic_seed.argv)]
 
             # Handle stdin and files
             # If the seed provides the content of files (#NOTE stdin is treated as a file)
             new_files = {}
             for k, c in self.seed.content.files.items():
-                if k in self._symbolic_seed.files:
-                    new_files[k] = bytes(repl_bytearray(bytearray(c), self._symbolic_seed.files[k]))
+                if k in self.symbolic_seed.files:
+                    new_files[k] = bytes(repl_bytearray(bytearray(c), self.symbolic_seed.files[k]))
                 else:
                     new_files[k] = c  # keep the current value in the seed
 
             # Handle variables, if the seed provides some
             new_variables = {}
             for k, c in self.seed.content.variables.items():
-                if k in self._symbolic_seed.variables:
+                if k in self.symbolic_seed.variables:
                     conc = bytearray(c) if isinstance(c, bytes) else [c]
-                    new_vals = repl_bytearray(conc, self._symbolic_seed.variables[k])
+                    new_vals = repl_bytearray(conc, self.symbolic_seed.variables[k])
                     new_variables[k] = bytes(new_vals) if isinstance(c, bytes) else new_vals[0]  # new variables are either bytes or int
                 else:
                     new_variables[k] = c  # If it has not been injected keep the current concrete value
 
             content = CompositeData(new_argv, new_files, new_variables)
         else:
             assert False
@@ -747,44 +764,44 @@
 
         :param addr: address where to inject the argv[ith]
         :param index: ith argv item
         :param value: value of the item
         """
         self.pstate.memory.write(addr, value)  # Write concrete bytes in memory
         sym_vars = self.pstate.symbolize_memory_bytes(addr, len(value), f"argv[{index}]") # Symbolize bytes
-        self._symbolic_seed.argv[index] = sym_vars # Add symbolic variables to symbolic seed
+        self.symbolic_seed.argv[index] = sym_vars # Add symbolic variables to symbolic seed
 
     def inject_symbolic_file_memory(self, addr: Addr, name: str, value: bytes, offset: int = 0) -> None:
         """
         Inject a symbolic file (or part of it) in memory.
 
         :param addr: address where to inject the file bytes
         :param name: name of the file in the composite seed
         :param value: bytes content of the file
         :param offset: offset within the file (for partial file injection)
         """
         self.pstate.memory.write(addr, value)  # Write concrete bytes in memory
         sym_vars = self.pstate.symbolize_memory_bytes(addr, len(value), name, offset) # Symbolize bytes
-        sym_seed = self._symbolic_seed.files[name] if self.seed.is_composite() else self._symbolic_seed
-        sym_seed[offset:offset+len(value)-1] = sym_vars # Add symbolic variables to symbolic seed
+        sym_seed = self.symbolic_seed.files[name] if self.seed.is_composite() else self.symbolic_seed
+        sym_seed[offset:offset+len(value)] = sym_vars # Add symbolic variables to symbolic seed
         # FIXME: Handle if reading twice same input bytes !
 
     def inject_symbolic_variable_memory(self, addr: Addr, name: str, value: bytes, offset: int = 0) -> None:
         """
         Inject a symbolic variable in memory.
 
         :param addr: address where to inject the variable
         :param name: name of the variable in the composite seed
         :param value: value of the variable
         :param offset: offset within the variable (for partial variable injection)
         :return:
         """
         self.pstate.memory.write(addr, value)  # Write concrete bytes in memory
         sym_vars = self.pstate.symbolize_memory_bytes(addr, len(value), name, offset)  # Symbolize bytes
-        self._symbolic_seed.variables[name][offset:offset+len(value)-1] = sym_vars # Add symbolic variables to symbolic seed
+        self.symbolic_seed.variables[name][offset:offset+len(value)-1] = sym_vars # Add symbolic variables to symbolic seed
         # FIXME: Handle if reading twice same input bytes !
 
     def inject_symbolic_file_register(self, reg: Union[str, Register], name: str, value: int, offset: int = 0) -> None:
         """
         Inject a symbolic file (or part of it) into a register.
         The value has to be an integer.
 
@@ -794,15 +811,15 @@
         :param offset: offset within the file
         """
         if reg.getSize != 1:
             logger.error("can't call inject_symbolic_file_register with regsiter larger than 1!")
             return
         self.pstate.write_register(reg, value)  # Write concrete value in register
         sym_vars = self.pstate.symbolize_register(reg, f"{name}[{offset}]")  # Symbolize bytes
-        sym_seed = self._symbolic_seed.files[name] if self.seed.is_composite() else self._symbolic_seed
+        sym_seed = self.symbolic_seed.files[name] if self.seed.is_composite() else self.symbolic_seed
         sym_seed[offset] = sym_vars  # Add symbolic variables to symbolic seed
 
     def inject_symbolic_variable_register(self, reg: Union[str, Register], name: str, value: int) -> None:
         """
         Inject a symbolic variable (or part of it) in a register.
         The value has to be an integer.
 
@@ -813,15 +830,15 @@
         if not self.seed.is_composite():
             logger.warning("cannot use inject_symbolic_variable_register on raw seeds!")
             return
 
         if isinstance(value, int):
             self.pstate.write_register(reg, value)                         # write concrete value in register
             sym_var = self.pstate.symbolize_register(reg, f"{name}[{0}]")  # symbolize value
-            self._symbolic_seed.variables[name][0] = sym_var               # add the symbolic variables to symbolic seed
+            self.symbolic_seed.variables[name][0] = sym_var               # add the symbolic variables to symbolic seed
         else:  # meant to be bytes
             logger.warning("variable injected in registers have to be integer values")
 
     def inject_symbolic_raw_input(self, addr: Addr, data: bytes, offset: int = 0) -> None:
         """
         Inject the input in memory. This injection method should
         be used for RAW seed type.
```

### Comparing `tritondse-0.1.8/tritondse/symbolic_explorator.py` & `tritondse-0.1.9/tritondse/symbolic_explorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import stat
 import enum_tools.documentation
 
 from tritondse.config            import Config
 from tritondse.process_state     import ProcessState
 from tritondse.loaders           import Loader
 from tritondse.seed              import Seed
+from tritondse.seed              import SeedStatus
 from tritondse.symbolic_executor import SymbolicExecutor
 from tritondse.workspace         import Workspace
 from tritondse.coverage          import GlobalCoverage
 from tritondse.types             import Addr
 from tritondse.exception         import StopExplorationException
 from tritondse.seeds_manager import SeedManager
 from tritondse.worklist import SeedScheduler
```

### Comparing `tritondse-0.1.8/tritondse/thread_context.py` & `tritondse-0.1.9/tritondse/thread_context.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/trace.py` & `tritondse-0.1.9/tritondse/trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             raise FileNotFoundError()
 
         args = [] if not args else args
 
         cmdlne = f'timeout {timeout} python -m pyqbdipreload {QBDITrace.QBDI_SCRIPT_FILEPATH}'.split(' ') + [binary_path] + args
         cmdlne = " ".join(cmdlne)
 
-        logger.debug(f'Command line: {" ".join(cmdlne)}')
+        logger.debug(f'Command line: {cmdlne}')
 
         # Set environment variables.
         environ = {
             'PYQBDIPRELOAD_COVERAGE_STRATEGY': strategy.name,
             'PYQBDIPRELOAD_OUTPUT_FILEPATH': output_path,
             'PYQBDIPRELOAD_DUMP_TRACE': str(dump_trace),
             'LD_BIND_NOW': '1',
```

### Comparing `tritondse-0.1.8/tritondse/types.py` & `tritondse-0.1.9/tritondse/types.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/worklist.py` & `tritondse-0.1.9/tritondse/worklist.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.8/tritondse/workspace.py` & `tritondse-0.1.9/tritondse/workspace.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     location of it.
     """
 
     DEFAULT_WORKSPACE = "/tmp/triton_workspace"
     CORPUS_DIR = "corpus"
     CRASH_DIR = "crashes"
     HANG_DIR = "hangs"
+    FAIL_DIR = "fails"
     WORKLIST_DIR = "worklist"
     METADATA_DIR = "metadata"
     BIN_DIR = "bin"
     LOG_FILE = "tritondse.log"
 
     def __init__(self, root_dir: PathLike):
         """
@@ -50,15 +51,15 @@
         Initialize the workspace by creating all required subfolders
         if not already existing.
 
         :param flush: if True deletes all files contained in the workspace
         :type flush: bool
         """
 
-        for dir in (self.root_dir / x for x in [self.CORPUS_DIR, self.CRASH_DIR, self.HANG_DIR, self.WORKLIST_DIR, self.METADATA_DIR, self.BIN_DIR]):
+        for dir in (self.root_dir / x for x in [self.CORPUS_DIR, self.CRASH_DIR, self.HANG_DIR, self.WORKLIST_DIR, self.METADATA_DIR, self.BIN_DIR, self.FAIL_DIR]):
             if not dir.exists():
                 logger.debug(f"Creating the {dir} directory")
                 dir.mkdir(parents=True)
             else:
                 if flush:
                     shutil.rmtree(dir)
                     dir.mkdir()
@@ -157,25 +158,35 @@
         Worklist are all the pending seeds
 
         :returns: generator of Seed object
         :rtype: Generator[Seed, None, None]
         """
         yield from self._iter_seeds(self.WORKLIST_DIR, SeedStatus.NEW)
 
+    def iter_fails(self) -> Generator[Seed, None, None]:
+        """
+        Iterate over the fail files as Seed object.
+
+        :returns: generator of Seed object
+        :rtype: Generator[Seed, None, None]
+        """
+        yield from self._iter_seeds(self.FAIL_DIR, SeedStatus.FAIL)
+
     def save_seed(self, seed: Seed) -> None:
         """
         Save the current seed in the workspace directory matching its status.
 
         :param seed: Seed to save
         :type seed: Seed
         """
         mapper = {SeedStatus.NEW: self.WORKLIST_DIR,
                   SeedStatus.OK_DONE: self.CORPUS_DIR,
                   SeedStatus.HANG: self.HANG_DIR,
-                  SeedStatus.CRASH: self.CRASH_DIR}
+                  SeedStatus.CRASH: self.CRASH_DIR,
+                  SeedStatus.FAIL: self.FAIL_DIR}
         p = (self.root_dir / mapper[seed.status]) / seed.filename
         p.write_bytes(bytes(seed))
 
     def update_seed_location(self, seed: Seed) -> None:
         """
         Move a worklist seed to its final location according to its (new) status.
         Typically used to move a seed from pending ones to corpus or crash once it
```

### Comparing `tritondse-0.1.8/tritondse.egg-info/PKG-INFO` & `tritondse-0.1.9/tritondse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritondse
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library of Dynamic Symbolic Exploration based the Triton library
 Home-page: https://github.com/quarkslab/tritondse
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/tritondse/
 Project-URL: Bug Tracker, https://github.com/quarkslab/tritondse/issues
 Project-URL: Source, https://github.com/quarkslab/tritondse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tritondse Version: 0.1.8 Summary: A library of
+Metadata-Version: 2.1 Name: tritondse Version: 0.1.9 Summary: A library of
 Dynamic Symbolic Exploration based the Triton library Home-page: https://
 github.com/quarkslab/tritondse Author: Quarkslab License: AGPL-3.0 Project-URL:
 Documentation, https://quarkslab.github.io/tritondse/ Project-URL: Bug Tracker,
 https://github.com/quarkslab/tritondse/issues Project-URL: Source, https://
 github.com/quarkslab/tritondse Classifier: Topic :: Security Classifier:
 Environment :: Console Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # TritonDSE
```

### Comparing `tritondse-0.1.8/tritondse.egg-info/SOURCES.txt` & `tritondse-0.1.9/tritondse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

