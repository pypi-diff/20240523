# Comparing `tmp/tricore_cli-1.5.tar.gz` & `tmp/tricore_cli-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tricore_cli-1.5.tar", last modified: Thu May 16 19:55:16 2024, max compression
+gzip compressed data, was "tricore_cli-1.7.tar", last modified: Thu May 23 13:15:53 2024, max compression
```

## Comparing `tricore_cli-1.5.tar` & `tricore_cli-1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 francesco   (501) staff       (20)        0 2024-05-16 19:55:16.643534 tricore_cli-1.5/
--rw-r--r--   0 francesco   (501) staff       (20)     1068 2024-03-21 09:45:08.000000 tricore_cli-1.5/LICENSE
--rw-r--r--   0 francesco   (501) staff       (20)     1126 2024-05-16 19:55:16.643319 tricore_cli-1.5/PKG-INFO
--rw-r--r--   0 francesco   (501) staff       (20)      695 2024-05-16 19:54:32.000000 tricore_cli-1.5/README.md
--rw-r--r--   0 francesco   (501) staff       (20)      560 2024-05-16 19:54:38.000000 tricore_cli-1.5/pyproject.toml
--rw-r--r--   0 francesco   (501) staff       (20)       38 2024-05-16 19:55:16.643581 tricore_cli-1.5/setup.cfg
-drwxr-xr-x   0 francesco   (501) staff       (20)        0 2024-05-16 19:55:16.641737 tricore_cli-1.5/src/
--rw-r--r--   0 francesco   (501) staff       (20)      178 2024-05-16 19:53:47.000000 tricore_cli-1.5/src/args.py
--rw-r--r--   0 francesco   (501) staff       (20)     1764 2024-05-16 19:53:47.000000 tricore_cli-1.5/src/containers.py
-drwxr-xr-x   0 francesco   (501) staff       (20)        0 2024-05-16 19:55:16.643064 tricore_cli-1.5/src/tricore_cli.egg-info/
--rw-r--r--   0 francesco   (501) staff       (20)     1126 2024-05-16 19:55:16.000000 tricore_cli-1.5/src/tricore_cli.egg-info/PKG-INFO
--rw-r--r--   0 francesco   (501) staff       (20)      329 2024-05-16 19:55:16.000000 tricore_cli-1.5/src/tricore_cli.egg-info/SOURCES.txt
--rw-r--r--   0 francesco   (501) staff       (20)        1 2024-05-16 19:55:16.000000 tricore_cli-1.5/src/tricore_cli.egg-info/dependency_links.txt
--rw-r--r--   0 francesco   (501) staff       (20)       47 2024-05-16 19:55:16.000000 tricore_cli-1.5/src/tricore_cli.egg-info/entry_points.txt
--rw-r--r--   0 francesco   (501) staff       (20)       14 2024-05-16 19:55:16.000000 tricore_cli-1.5/src/tricore_cli.egg-info/requires.txt
--rw-r--r--   0 francesco   (501) staff       (20)       33 2024-05-16 19:55:16.000000 tricore_cli-1.5/src/tricore_cli.egg-info/top_level.txt
--rw-r--r--   0 francesco   (501) staff       (20)     2513 2024-05-16 19:53:47.000000 tricore_cli-1.5/src/tricorecli.py
--rw-r--r--   0 francesco   (501) staff       (20)     1605 2024-05-16 19:53:47.000000 tricore_cli-1.5/src/utils.py
+drwxr-xr-x   0 francesco   (501) staff       (20)        0 2024-05-23 13:15:53.199890 tricore_cli-1.7/
+-rw-r--r--   0 francesco   (501) staff       (20)     1068 2024-03-21 09:45:08.000000 tricore_cli-1.7/LICENSE
+-rw-r--r--   0 francesco   (501) staff       (20)     1153 2024-05-23 13:15:53.199661 tricore_cli-1.7/PKG-INFO
+-rw-r--r--   0 francesco   (501) staff       (20)      695 2024-05-16 19:54:32.000000 tricore_cli-1.7/README.md
+-rw-r--r--   0 francesco   (501) staff       (20)      562 2024-05-23 13:09:27.000000 tricore_cli-1.7/pyproject.toml
+-rw-r--r--   0 francesco   (501) staff       (20)       38 2024-05-23 13:15:53.199934 tricore_cli-1.7/setup.cfg
+drwxr-xr-x   0 francesco   (501) staff       (20)        0 2024-05-23 13:15:53.198151 tricore_cli-1.7/src/
+-rw-r--r--   0 francesco   (501) staff       (20)      178 2024-05-16 19:53:47.000000 tricore_cli-1.7/src/args.py
+-rw-r--r--   0 francesco   (501) staff       (20)     2176 2024-05-23 13:05:21.000000 tricore_cli-1.7/src/containers.py
+drwxr-xr-x   0 francesco   (501) staff       (20)        0 2024-05-23 13:15:53.199407 tricore_cli-1.7/src/tricore_cli.egg-info/
+-rw-r--r--   0 francesco   (501) staff       (20)     1153 2024-05-23 13:15:53.000000 tricore_cli-1.7/src/tricore_cli.egg-info/PKG-INFO
+-rw-r--r--   0 francesco   (501) staff       (20)      329 2024-05-23 13:15:53.000000 tricore_cli-1.7/src/tricore_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 francesco   (501) staff       (20)        1 2024-05-23 13:15:53.000000 tricore_cli-1.7/src/tricore_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 francesco   (501) staff       (20)       47 2024-05-23 13:15:53.000000 tricore_cli-1.7/src/tricore_cli.egg-info/entry_points.txt
+-rw-r--r--   0 francesco   (501) staff       (20)       25 2024-05-23 13:15:53.000000 tricore_cli-1.7/src/tricore_cli.egg-info/requires.txt
+-rw-r--r--   0 francesco   (501) staff       (20)       33 2024-05-23 13:15:53.000000 tricore_cli-1.7/src/tricore_cli.egg-info/top_level.txt
+-rw-r--r--   0 francesco   (501) staff       (20)     2578 2024-05-23 13:05:21.000000 tricore_cli-1.7/src/tricorecli.py
+-rw-r--r--   0 francesco   (501) staff       (20)     1737 2024-05-23 13:05:21.000000 tricore_cli-1.7/src/utils.py
```

### Comparing `tricore_cli-1.5/LICENSE` & `tricore_cli-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tricore_cli-1.5/PKG-INFO` & `tricore_cli-1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: tricore-cli
-Version: 1.5
+Version: 1.7
 Summary: A utility script for interacting with containerized TriCore development environment
 Author: Francesco Mecatti
 Project-URL: Homepage, https://github.com/mc-cat-tty/tricore-dev-env
 Project-URL: Issues, https://github.com/mc-cat-tty/tricore-dev-env/issues
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docker>=7.0.0
+Requires-Dist: rich>=13.7
 
 # TriCore CLI
 A utility script for interacting with containerized TriCore development environment.
 
 ## Usage
 ### Build
```

### Comparing `tricore_cli-1.5/README.md` & `tricore_cli-1.7/README.md`

 * *Files identical despite different names*

### Comparing `tricore_cli-1.5/pyproject.toml` & `tricore_cli-1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "tricore-cli"
-version = "1.5"
+version = "1.7"
 authors = [{ name = "Francesco Mecatti" }]
 description = "A utility script for interacting with containerized TriCore development environment"
 readme = "README.md"
-requires-python = ">=3.9"
-dependencies = ["docker>=7.0.0"]
+requires-python = ">=3.10"
+dependencies = ["docker>=7.0.0", "rich>=13.7"]
 
 [project.urls]
 Homepage = "https://github.com/mc-cat-tty/tricore-dev-env"
 Issues = "https://github.com/mc-cat-tty/tricore-dev-env/issues"
 
 [project.scripts]
 tricorecli = "tricorecli:main"
 
 [build-system]
-requires = ["setuptools>=61.0", "rich>=13.7"]
-build-backend = "setuptools.build_meta"
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
```

### Comparing `tricore_cli-1.5/src/tricore_cli.egg-info/PKG-INFO` & `tricore_cli-1.7/src/tricore_cli.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: tricore-cli
-Version: 1.5
+Version: 1.7
 Summary: A utility script for interacting with containerized TriCore development environment
 Author: Francesco Mecatti
 Project-URL: Homepage, https://github.com/mc-cat-tty/tricore-dev-env
 Project-URL: Issues, https://github.com/mc-cat-tty/tricore-dev-env/issues
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docker>=7.0.0
+Requires-Dist: rich>=13.7
 
 # TriCore CLI
 A utility script for interacting with containerized TriCore development environment.
 
 ## Usage
 ### Build
```

### Comparing `tricore_cli-1.5/src/tricorecli.py` & `tricore_cli-1.7/src/tricorecli.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,25 +26,29 @@
     os.makedirs(build_path)
 
   CPUS: int = int(os.cpu_count()*1.5) if os.cpu_count() else 2
 
   with BuildDisposableContainer(abs_path) as build_container:
     print(f'Building source with {CPUS} jobs from {abs_path}')
 
-    res = build_container.exec_run('cmake -B build --toolchain tricore_toolchain.cmake', stream=True)
-    print_stream(res)
+    exit_if_error(
+      build_container.run_async('cmake -B build --toolchain tricore_toolchain.cmake', print_stream),
+      "Failed makefiles generation."
+    )
     
-    res = build_container.exec_run(f'cmake --build build --parallel {CPUS}', stream=True)
-    print_stream(res)
+    exit_if_error(
+      build_container.run_async(f'cmake --build build --parallel {CPUS}', print_stream),
+      "Build failed."
+    )
   
-  print(f"Successfully built artifacts in {build_path}")
+  print(f"Successfully built artifacts in {build_path}.")
     
 
 def flash(args: FlashHandlerArgs) -> None:
-  raise NotImplementedError('Feature not implemented yet')
+  raise NotImplementedError('Feature not implemented yet.')
 
 
 def main() -> None:
   parser = argparse.ArgumentParser(
     description='Utility script for managing the build of TriCore applications with ease.'
   )
   subparsers = parser.add_subparsers(title='action', required=True)
```

### Comparing `tricore_cli-1.5/src/utils.py` & `tricore_cli-1.7/src/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,18 +31,24 @@
 
 def check_file_or_exit(file_path: str, error_msg: str = "", exit_code: int = 1):
   if os.path.isfile(file_path): return
   
   print(error_msg)
   exit(exit_code)
 
-def print_stream(exec_result):
-  if GlobalConfiguration().verbosity_level < 1: return
-  
-  for line in exec_result.output:
+def exit_if_error(exit_code: int, msg: str):
+  if exit_code == 0: return
+  print(msg)
+  exit(exit_code)
+
+def print_stream(exec_stream):
+  skip_print: bool = GlobalConfiguration().verbosity_level < 1
+
+  for line in exec_stream:
+    if skip_print: continue
     print(line.decode('utf-8'), end='')
 
 def print_pull_progress(stream: Generator):
   tasks: dict = {}
 
   with Progress() as progress_bar:
     for line_dict in stream:
```

