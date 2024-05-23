# Comparing `tmp/isvirtual-1.0.0.tar.gz` & `tmp/isvirtual-1.1.0.tar.gz`

## Comparing `isvirtual-1.0.0.tar` & `isvirtual-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 isvirtual-1.0.0/VERSION.md
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 isvirtual-1.0.0/main.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 isvirtual-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 isvirtual-1.0.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 isvirtual-1.0.0/LICENSE
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 isvirtual-1.0.0/README.md
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 isvirtual-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 isvirtual-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 isvirtual-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 isvirtual-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 isvirtual-1.1.0/src/VERSION.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 isvirtual-1.1.0/src/__init__.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 isvirtual-1.1.0/src/main.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 isvirtual-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 isvirtual-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 isvirtual-1.1.0/README.md
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 isvirtual-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 isvirtual-1.1.0/PKG-INFO
```

### Comparing `isvirtual-1.0.0/.github/workflows/release.yml` & `isvirtual-1.1.0/.github/workflows/release.yml`

 * *Files 12% similar despite different names*

```diff
@@ -7,33 +7,39 @@
   contents: write
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
       - name: Github actions init
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           # To force fetching tags
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.8"
 
       - name: Install build dependencies
         run: pip install build
 
+      - name: Build
+        run: python -m build
+
       - name: Read VERSION file
         id: getversion
-        run: echo "::set-output name=version::$(cat pyittention2/VERSION.md)"
+        run: echo "version=$(cat src/VERSION.md)" >> $GITHUB_OUTPUT
 
       - name: Changelog
         run: git log $(git describe --tags --abbrev=0)..HEAD --format="%s %h" > LATEST-CHANGES.md
 
       - name: Release
-        uses: softprops/action-gh-release@v1
+        uses: softprops/action-gh-release@v2
         with:
-          files: dist/*.whl
+          files: |
+            dist/*.whl
+            dist/*.tar.gz
           tag_name: v${{ steps.getversion.outputs.version }}
           body_path: LATEST-CHANGES.md
+          token: ${{ secrets.PAT_ISVIRTUAL }}
```

### Comparing `isvirtual-1.0.0/LICENSE` & `isvirtual-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isvirtual-1.0.0/README.md` & `isvirtual-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,26 +10,53 @@
 
 ```bash
 pip install isvirtual
 ```
 
 # Usage
 
-Within a python script:
+This lib can be used within a python script or as a command line.
+
+## Python
+Simple check:
 ```python
 from isvirtual import is_virtual_env
 
 if __name__ == "__main__":
     if is_virtual_env() is True:
         print("You are within a virtual environment")
     else:
         print("You are not in a virtual env")
 ```
 
-CLI mode:
+You can also check if you are specifically in a `venv` or `virtualenv` environment:
+```python
+from isvirtual import is_venv, is_virtualenv
+
+if __name__ == "__main__":
+    if is_venv() is True:
+        print("You are in a venv")
+    elif is_virtualenv() is True:
+        print("You are in a virtualenv")
+    else:
+        print("You are not in a virtual env")
+```
+
+You can also get the info from the env coming from `pyvenv.cfg`. The `sys.prefix` data is added to the original config file:
+```python
+from isvirtual import is_virtual_env, pyvenv_cfg
+
+if __name__ == "__main__":
+    if is_virtual_env() is True:
+        data = pyvenv_cfg()
+        print(data["home"])
+```
+
+
+## CLI
 ```console
 $ isvirtual
 Yes
 ```
 
 # License
```

### Comparing `isvirtual-1.0.0/pyproject.toml` & `isvirtual-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "isvirtual"
-version = "1.0.0"
 description = "Detect if your script is running inside a virtual environment"
+dynamic = ["version"]
 readme = "README.md"
 authors = [{ name = "Alex Mili" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.3"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
@@ -35,8 +35,12 @@
 Repository = "https://github.com/AlexMili/isVirtual"
 Documentation = "https://github.com/AlexMili/isVirtual"
 
 [project.scripts]
 isvirtual = "main:is_virtual_env_cli"
 
 [tool.hatch.build.targets.wheel]
-packages = ["."]
+packages = ["./src"]
+
+[tool.hatch.version]
+path = "src/VERSION.md"
+pattern = "(?P<version>.*)"
```

### Comparing `isvirtual-1.0.0/PKG-INFO` & `isvirtual-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: isvirtual
-Version: 1.0.0
+Version: 1.1.0
 Summary: Detect if your script is running inside a virtual environment
 Project-URL: Homepage, https://github.com/AlexMili/isVirtual
 Project-URL: Issues, https://github.com/AlexMili/isVirtual/issues
 Project-URL: Repository, https://github.com/AlexMili/isVirtual
 Project-URL: Documentation, https://github.com/AlexMili/isVirtual
 Author: Alex Mili
 License: MIT License
@@ -59,26 +59,53 @@
 
 ```bash
 pip install isvirtual
 ```
 
 # Usage
 
-Within a python script:
+This lib can be used within a python script or as a command line.
+
+## Python
+Simple check:
 ```python
 from isvirtual import is_virtual_env
 
 if __name__ == "__main__":
     if is_virtual_env() is True:
         print("You are within a virtual environment")
     else:
         print("You are not in a virtual env")
 ```
 
-CLI mode:
+You can also check if you are specifically in a `venv` or `virtualenv` environment:
+```python
+from isvirtual import is_venv, is_virtualenv
+
+if __name__ == "__main__":
+    if is_venv() is True:
+        print("You are in a venv")
+    elif is_virtualenv() is True:
+        print("You are in a virtualenv")
+    else:
+        print("You are not in a virtual env")
+```
+
+You can also get the info from the env coming from `pyvenv.cfg`. The `sys.prefix` data is added to the original config file:
+```python
+from isvirtual import is_virtual_env, pyvenv_cfg
+
+if __name__ == "__main__":
+    if is_virtual_env() is True:
+        data = pyvenv_cfg()
+        print(data["home"])
+```
+
+
+## CLI
 ```console
 $ isvirtual
 Yes
 ```
 
 # License
```

