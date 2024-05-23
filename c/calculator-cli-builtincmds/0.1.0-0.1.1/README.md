# Comparing `tmp/calculator_cli_builtincmds-0.1.0.tar.gz` & `tmp/calculator_cli_builtincmds-0.1.1.tar.gz`

## Comparing `calculator_cli_builtincmds-0.1.0.tar` & `calculator_cli_builtincmds-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 calculator_cli_builtincmds-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     3422 2024-05-23 06:55:08.000000 calculator_cli_builtincmds-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-05-23 06:55:08.000000 calculator_cli_builtincmds-0.1.0/.gitignore
--rw-r--r--   0     1001      127        0 2024-05-23 06:55:08.000000 calculator_cli_builtincmds-0.1.0/README.md
--rw-r--r--   0     1001      127     3115 2024-05-23 06:55:08.000000 calculator_cli_builtincmds-0.1.0/poetry.lock
--rw-r--r--   0     1001      127      142 2024-05-23 06:55:08.000000 calculator_cli_builtincmds-0.1.0/python/builtincmds/__init__.py
--rw-r--r--   0     1001      127      123 2024-05-23 06:55:08.000000 calculator_cli_builtincmds-0.1.0/python/builtincmds/__init__.pyi
--rw-r--r--   0     1001      127     1481 2024-05-23 06:55:08.000000 calculator_cli_builtincmds-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127    15768 2024-05-23 06:55:08.000000 calculator_cli_builtincmds-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      524 2024-05-23 06:55:08.000000 calculator_cli_builtincmds-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      177 1970-01-01 00:00:00.000000 calculator_cli_builtincmds-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 calculator_cli_builtincmds-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     3422 2024-05-23 08:17:04.000000 calculator_cli_builtincmds-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-05-23 08:17:04.000000 calculator_cli_builtincmds-0.1.1/.gitignore
+-rw-r--r--   0     1001      127        0 2024-05-23 08:17:04.000000 calculator_cli_builtincmds-0.1.1/README.md
+-rw-r--r--   0     1001      127     6212 2024-05-23 08:17:04.000000 calculator_cli_builtincmds-0.1.1/poetry.lock
+-rw-r--r--   0     1001      127      202 2024-05-23 08:17:04.000000 calculator_cli_builtincmds-0.1.1/python/calculator_cli_builtincmds/__init__.py
+-rw-r--r--   0     1001      127      123 2024-05-23 08:17:04.000000 calculator_cli_builtincmds-0.1.1/python/calculator_cli_builtincmds/__init__.pyi
+-rw-r--r--   0     1001      127      128 2024-05-23 08:17:04.000000 calculator_cli_builtincmds-0.1.1/python/tests/test_import.py
+-rw-r--r--   0     1001      127     1496 2024-05-23 08:17:04.000000 calculator_cli_builtincmds-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127    15768 2024-05-23 08:17:04.000000 calculator_cli_builtincmds-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127      542 2024-05-23 08:17:04.000000 calculator_cli_builtincmds-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      177 1970-01-01 00:00:00.000000 calculator_cli_builtincmds-0.1.1/PKG-INFO
```

### Comparing `calculator_cli_builtincmds-0.1.0/.github/workflows/CI.yml` & `calculator_cli_builtincmds-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `calculator_cli_builtincmds-0.1.0/.gitignore` & `calculator_cli_builtincmds-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `calculator_cli_builtincmds-0.1.0/src/lib.rs` & `calculator_cli_builtincmds-0.1.1/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -36,12 +36,12 @@
     catch_err(pager.set_prompt(prompt))?;
     catch_err(pager.set_exit_strategy(ExitStrategy::PagerQuit))?;
     pager_thread.join().unwrap().unwrap();
     Ok(())
 }
 
 #[pymodule]
-pub fn builtincmds(m: &Bound<'_, PyModule>) -> PyResult<()> {
+pub fn calculator_cli_builtincmds(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(show_file, m)?)?;
     m.add_function(wrap_pyfunction!(show_text, m)?)?;
     Ok(())
 }
```

### Comparing `calculator_cli_builtincmds-0.1.0/Cargo.lock` & `calculator_cli_builtincmds-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "calculator_cli_builtincmds"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "minus",
  "pyo3",
 ]
 
 [[package]]
 name = "cfg-if"
```

### Comparing `calculator_cli_builtincmds-0.1.0/pyproject.toml` & `calculator_cli_builtincmds-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [project]
 name = "calculator_cli_builtincmds"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.10"
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry]
 name = "calculator_cli_builtincmds"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["salam99823 <salamatbekboev2008@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 maturin = "^1.5.1"
+pytest = "^8.2.1"
 
 [tool.maturin]
 python-source = "python"
 features = ["pyo3/extension-module"]
 
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
```

