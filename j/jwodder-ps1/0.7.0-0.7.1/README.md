# Comparing `tmp/jwodder_ps1-0.7.0.tar.gz` & `tmp/jwodder_ps1-0.7.1.tar.gz`

## Comparing `jwodder_ps1-0.7.0.tar` & `jwodder_ps1-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/tox.ini
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/src/jwodder_ps1/__init__.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/src/jwodder_ps1/__main__.py
--rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/src/jwodder_ps1/git.py
--rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/src/jwodder_ps1/info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/src/jwodder_ps1/py.typed
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/src/jwodder_ps1/styles.py
--rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/test/test_git.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/test/test_info.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/test/test_util.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/LICENSE
--rw-r--r--   0        0        0     6393 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/README.rst
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7682 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/tox.ini
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/src/jwodder_ps1/__init__.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/src/jwodder_ps1/__main__.py
+-rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/src/jwodder_ps1/git.py
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/src/jwodder_ps1/info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/src/jwodder_ps1/py.typed
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/src/jwodder_ps1/styles.py
+-rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/test/test_git.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/test/test_info.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/test/test_util.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6393 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/README.rst
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7682 2020-02-02 00:00:00.000000 jwodder_ps1-0.7.1/PKG-INFO
```

### Comparing `jwodder_ps1-0.7.0/CHANGELOG.md` & `jwodder_ps1-0.7.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+v0.7.1 (2024-05-23)
+-------------------
+- Fixed support for custom venv prompt prefixes
+
 v0.7.0 (2024-05-13)
 -------------------
 - The branch name/`HEAD` description is now truncated if it gets too long.
 - Add `--theme` option for selecting between dark and light themes
 - Add `--no-hostname` option
 - Drop support for Python 3.8
```

### Comparing `jwodder_ps1-0.7.0/tox.ini` & `jwodder_ps1-0.7.1/tox.ini`

 * *Files identical despite different names*

### Comparing `jwodder_ps1-0.7.0/src/jwodder_ps1/__init__.py` & `jwodder_ps1-0.7.1/src/jwodder_ps1/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 - Supports both Bash and zsh
 - Can optionally output just the Git status, in case you want to combine it
   with your own prompt string
 
 Visit <https://github.com/jwodder/ps1.py> for more information.
 """
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 __author__ = "John Thorvald Wodder II"
 __author_email__ = "ps1@varonathe.org"
 __license__ = "MIT"
 __url__ = "https://github.com/jwodder/ps1.py"
```

### Comparing `jwodder_ps1-0.7.0/src/jwodder_ps1/__main__.py` & `jwodder_ps1-0.7.1/src/jwodder_ps1/__main__.py`

 * *Files identical despite different names*

### Comparing `jwodder_ps1-0.7.0/src/jwodder_ps1/git.py` & `jwodder_ps1-0.7.1/src/jwodder_ps1/git.py`

 * *Files identical despite different names*

### Comparing `jwodder_ps1-0.7.0/src/jwodder_ps1/info.py` & `jwodder_ps1-0.7.1/src/jwodder_ps1/info.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,19 +61,19 @@
             venv = Path(venv_str)
             venv_prompt = venv.name
             try:
                 with (venv / "pyvenv.cfg").open(encoding="utf-8") as fp:
                     for line in fp:
                         line = line.strip()
                         if m := re.match(r"^prompt\s*=\s*", line):
-                            prompt = line[m.end() :]
-                            if re.fullmatch(r'([\x27"]).*\1', prompt):
+                            venv_prompt = line[m.end() :]
+                            if re.fullmatch(r'([\x27"]).*\1', venv_prompt):
                                 # repr-ized prompt produced by venv
                                 try:
-                                    venv_prompt = literal_eval(prompt)
+                                    venv_prompt = literal_eval(venv_prompt)
                                 except Exception:
                                     pass
                             break
             except FileNotFoundError:
                 pass
         else:
             venv_prompt = None
```

### Comparing `jwodder_ps1-0.7.0/src/jwodder_ps1/styles.py` & `jwodder_ps1-0.7.1/src/jwodder_ps1/styles.py`

 * *Files identical despite different names*

### Comparing `jwodder_ps1-0.7.0/test/test_git.py` & `jwodder_ps1-0.7.1/test/test_git.py`

 * *Files identical despite different names*

### Comparing `jwodder_ps1-0.7.0/test/test_info.py` & `jwodder_ps1-0.7.1/test/test_info.py`

 * *Files identical despite different names*

### Comparing `jwodder_ps1-0.7.0/test/test_util.py` & `jwodder_ps1-0.7.1/test/test_util.py`

 * *Files identical despite different names*

### Comparing `jwodder_ps1-0.7.0/LICENSE` & `jwodder_ps1-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jwodder_ps1-0.7.0/README.rst` & `jwodder_ps1-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `jwodder_ps1-0.7.0/pyproject.toml` & `jwodder_ps1-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jwodder_ps1-0.7.0/PKG-INFO` & `jwodder_ps1-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jwodder-ps1
-Version: 0.7.0
+Version: 0.7.1
 Summary: Yet another bash/zsh custom prompt script
 Project-URL: Source Code, https://github.com/jwodder/ps1.py
 Project-URL: Bug Tracker, https://github.com/jwodder/ps1.py/issues
 Author-email: John Thorvald Wodder II <ps1@varonathe.org>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: bash,git,prompt,ps1,zsh
```

