# Comparing `tmp/autograph-utils-0.2.0.tar.gz` & `tmp/autograph_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autograph-utils-0.2.0.tar", last modified: Fri Apr  5 14:01:01 2024, max compression
+gzip compressed data, was "autograph_utils-0.3.0.tar", last modified: Thu May 23 13:07:38 2024, max compression
```

## Comparing `autograph-utils-0.2.0.tar` & `autograph_utils-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.160618 autograph-utils-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.156618 autograph-utils-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.156618 autograph-utils-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/workflows/labels.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-05 14:01:01.156618 autograph-utils-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)    36127 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:01:01.160618 autograph-utils-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.152618 autograph-utils-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.156618 autograph-utils-0.2.0/src/autograph_utils/
--rw-r--r--   0 runner    (1001) docker     (127)    16361 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/src/autograph_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/src/autograph_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/src/autograph_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.156618 autograph-utils-0.2.0/src/autograph_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-05 14:01:01.000000 autograph-utils-0.2.0/src/autograph_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-05 14:01:01.000000 autograph-utils-0.2.0/src/autograph_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:01:01.000000 autograph-utils-0.2.0/src/autograph_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 14:01:01.000000 autograph-utils-0.2.0/src/autograph_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-05 14:01:01.000000 autograph-utils-0.2.0/src/autograph_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 14:01:01.000000 autograph-utils-0.2.0/src/autograph_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.156618 autograph-utils-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/tests/normandy.content-signature.mozilla.org-2019-12-04-18-15-23.chain
--rw-r--r--   0 runner    (1001) docker     (127)     7695 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/tests/normandy.content-signature.mozilla.org-20210705.dev.chain
--rwxr-xr-x   0 runner    (1001) docker     (127)    17282 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/tests/test_autograph_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:38.751088 autograph_utils-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:38.747088 autograph_utils-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:38.747088 autograph_utils-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/.github/workflows/labels.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-23 13:07:38.751088 autograph_utils-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)    37503 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:07:38.751088 autograph_utils-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:38.743088 autograph_utils-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:38.747088 autograph_utils-0.3.0/src/autograph_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/src/autograph_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/src/autograph_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/src/autograph_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:38.747088 autograph_utils-0.3.0/src/autograph_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-23 13:07:38.000000 autograph_utils-0.3.0/src/autograph_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-23 13:07:38.000000 autograph_utils-0.3.0/src/autograph_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:07:38.000000 autograph_utils-0.3.0/src/autograph_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 13:07:38.000000 autograph_utils-0.3.0/src/autograph_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-23 13:07:38.000000 autograph_utils-0.3.0/src/autograph_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 13:07:38.000000 autograph_utils-0.3.0/src/autograph_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:07:38.747088 autograph_utils-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/tests/normandy.content-signature.mozilla.org-2019-12-04-18-15-23.chain
+-rw-r--r--   0 runner    (1001) docker     (127)     7695 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/tests/normandy.content-signature.mozilla.org-20210705.dev.chain
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17546 2024-05-23 13:07:34.000000 autograph_utils-0.3.0/tests/test_autograph_utils.py
```

### Comparing `autograph-utils-0.2.0/.github/CONTRIBUTING.md` & `autograph_utils-0.3.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autograph-utils-0.2.0/.github/SECURITY.md` & `autograph_utils-0.3.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `autograph-utils-0.2.0/.github/workflows/publish.yml` & `autograph_utils-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `autograph-utils-0.2.0/.github/workflows/test.yml` & `autograph_utils-0.3.0/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,17 @@
     name: Lint
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
 
       - uses: actions/setup-python@v5
+        with:
+            python-version: "3.12"
+            cache: pip
 
       - name: Run linting and formatting checks
         run: make lint
 
   unit-tests:
     name: Unit tests
     runs-on: ubuntu-latest
```

### Comparing `autograph-utils-0.2.0/.gitignore` & `autograph_utils-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autograph-utils-0.2.0/.pre-commit-config.yaml` & `autograph_utils-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autograph-utils-0.2.0/LICENSE` & `autograph_utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autograph-utils-0.2.0/Makefile` & `autograph_utils-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `autograph-utils-0.2.0/PKG-INFO` & `autograph_utils-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autograph-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: autograph-utils is a tool to configure a kinto server from an YAML file.
 Author-email: Mozilla Services <dev-webdev@lists.mozilla.org>
 License: Apache Software License 2.0
         
         Copyright (c) 2019, Ethan Glasser-Camp
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `autograph-utils-0.2.0/README.rst` & `autograph_utils-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `autograph-utils-0.2.0/pyproject.toml` & `autograph_utils-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 
 [project.scripts]
 autograph_utils = "autograph_utils.cli:main"
 
 [tool.pip-tools]
 generate-hashes = true
 
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+
 [tool.coverage.run]
 relative_files = true
 
 [tool.ruff]
 line-length = 99
 extend-exclude = [
     "__pycache__",
```

### Comparing `autograph-utils-0.2.0/requirements.txt` & `autograph_utils-0.3.0/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
-#    pip-compile --generate-hashes
+#    pip-compile --generate-hashes --strip-extras
 #
-aiohttp==3.9.3 \
-    --hash=sha256:017a21b0df49039c8f46ca0971b3a7fdc1f56741ab1240cb90ca408049766168 \
-    --hash=sha256:039df344b45ae0b34ac885ab5b53940b174530d4dd8a14ed8b0e2155b9dddccb \
-    --hash=sha256:055ce4f74b82551678291473f66dc9fb9048a50d8324278751926ff0ae7715e5 \
-    --hash=sha256:06a9b2c8837d9a94fae16c6223acc14b4dfdff216ab9b7202e07a9a09541168f \
-    --hash=sha256:07b837ef0d2f252f96009e9b8435ec1fef68ef8b1461933253d318748ec1acdc \
-    --hash=sha256:0ed621426d961df79aa3b963ac7af0d40392956ffa9be022024cd16297b30c8c \
-    --hash=sha256:0fa43c32d1643f518491d9d3a730f85f5bbaedcbd7fbcae27435bb8b7a061b29 \
-    --hash=sha256:1f5a71d25cd8106eab05f8704cd9167b6e5187bcdf8f090a66c6d88b634802b4 \
-    --hash=sha256:1f5cd333fcf7590a18334c90f8c9147c837a6ec8a178e88d90a9b96ea03194cc \
-    --hash=sha256:27468897f628c627230dba07ec65dc8d0db566923c48f29e084ce382119802bc \
-    --hash=sha256:298abd678033b8571995650ccee753d9458dfa0377be4dba91e4491da3f2be63 \
-    --hash=sha256:2c895a656dd7e061b2fd6bb77d971cc38f2afc277229ce7dd3552de8313a483e \
-    --hash=sha256:361a1026c9dd4aba0109e4040e2aecf9884f5cfe1b1b1bd3d09419c205e2e53d \
-    --hash=sha256:363afe77cfcbe3a36353d8ea133e904b108feea505aa4792dad6585a8192c55a \
-    --hash=sha256:38a19bc3b686ad55804ae931012f78f7a534cce165d089a2059f658f6c91fa60 \
-    --hash=sha256:38f307b41e0bea3294a9a2a87833191e4bcf89bb0365e83a8be3a58b31fb7f38 \
-    --hash=sha256:3e59c23c52765951b69ec45ddbbc9403a8761ee6f57253250c6e1536cacc758b \
-    --hash=sha256:4b4af9f25b49a7be47c0972139e59ec0e8285c371049df1a63b6ca81fdd216a2 \
-    --hash=sha256:504b6981675ace64c28bf4a05a508af5cde526e36492c98916127f5a02354d53 \
-    --hash=sha256:50fca156d718f8ced687a373f9e140c1bb765ca16e3d6f4fe116e3df7c05b2c5 \
-    --hash=sha256:522a11c934ea660ff8953eda090dcd2154d367dec1ae3c540aff9f8a5c109ab4 \
-    --hash=sha256:52df73f14ed99cee84865b95a3d9e044f226320a87af208f068ecc33e0c35b96 \
-    --hash=sha256:595f105710293e76b9dc09f52e0dd896bd064a79346234b521f6b968ffdd8e58 \
-    --hash=sha256:59c26c95975f26e662ca78fdf543d4eeaef70e533a672b4113dd888bd2423caa \
-    --hash=sha256:5bce0dc147ca85caa5d33debc4f4d65e8e8b5c97c7f9f660f215fa74fc49a321 \
-    --hash=sha256:5eafe2c065df5401ba06821b9a054d9cb2848867f3c59801b5d07a0be3a380ae \
-    --hash=sha256:5ed3e046ea7b14938112ccd53d91c1539af3e6679b222f9469981e3dac7ba1ce \
-    --hash=sha256:5fe9ce6c09668063b8447f85d43b8d1c4e5d3d7e92c63173e6180b2ac5d46dd8 \
-    --hash=sha256:648056db9a9fa565d3fa851880f99f45e3f9a771dd3ff3bb0c048ea83fb28194 \
-    --hash=sha256:69361bfdca5468c0488d7017b9b1e5ce769d40b46a9f4a2eed26b78619e9396c \
-    --hash=sha256:6b0e029353361f1746bac2e4cc19b32f972ec03f0f943b390c4ab3371840aabf \
-    --hash=sha256:6b88f9386ff1ad91ace19d2a1c0225896e28815ee09fc6a8932fded8cda97c3d \
-    --hash=sha256:770d015888c2a598b377bd2f663adfd947d78c0124cfe7b959e1ef39f5b13869 \
-    --hash=sha256:7943c414d3a8d9235f5f15c22ace69787c140c80b718dcd57caaade95f7cd93b \
-    --hash=sha256:7cf5c9458e1e90e3c390c2639f1017a0379a99a94fdfad3a1fd966a2874bba52 \
-    --hash=sha256:7f46acd6a194287b7e41e87957bfe2ad1ad88318d447caf5b090012f2c5bb528 \
-    --hash=sha256:82e6aa28dd46374f72093eda8bcd142f7771ee1eb9d1e223ff0fa7177a96b4a5 \
-    --hash=sha256:835a55b7ca49468aaaac0b217092dfdff370e6c215c9224c52f30daaa735c1c1 \
-    --hash=sha256:84871a243359bb42c12728f04d181a389718710129b36b6aad0fc4655a7647d4 \
-    --hash=sha256:8aacb477dc26797ee089721536a292a664846489c49d3ef9725f992449eda5a8 \
-    --hash=sha256:8e2c45c208c62e955e8256949eb225bd8b66a4c9b6865729a786f2aa79b72e9d \
-    --hash=sha256:90842933e5d1ff760fae6caca4b2b3edba53ba8f4b71e95dacf2818a2aca06f7 \
-    --hash=sha256:938a9653e1e0c592053f815f7028e41a3062e902095e5a7dc84617c87267ebd5 \
-    --hash=sha256:939677b61f9d72a4fa2a042a5eee2a99a24001a67c13da113b2e30396567db54 \
-    --hash=sha256:9d3c9b50f19704552f23b4eaea1fc082fdd82c63429a6506446cbd8737823da3 \
-    --hash=sha256:a6fe5571784af92b6bc2fda8d1925cccdf24642d49546d3144948a6a1ed58ca5 \
-    --hash=sha256:a78ed8a53a1221393d9637c01870248a6f4ea5b214a59a92a36f18151739452c \
-    --hash=sha256:ab40e6251c3873d86ea9b30a1ac6d7478c09277b32e14745d0d3c6e76e3c7e29 \
-    --hash=sha256:abf151955990d23f84205286938796c55ff11bbfb4ccfada8c9c83ae6b3c89a3 \
-    --hash=sha256:acef0899fea7492145d2bbaaaec7b345c87753168589cc7faf0afec9afe9b747 \
-    --hash=sha256:b40670ec7e2156d8e57f70aec34a7216407848dfe6c693ef131ddf6e76feb672 \
-    --hash=sha256:b791a3143681a520c0a17e26ae7465f1b6f99461a28019d1a2f425236e6eedb5 \
-    --hash=sha256:b955ed993491f1a5da7f92e98d5dad3c1e14dc175f74517c4e610b1f2456fb11 \
-    --hash=sha256:ba39e9c8627edc56544c8628cc180d88605df3892beeb2b94c9bc857774848ca \
-    --hash=sha256:bca77a198bb6e69795ef2f09a5f4c12758487f83f33d63acde5f0d4919815768 \
-    --hash=sha256:c3452ea726c76e92f3b9fae4b34a151981a9ec0a4847a627c43d71a15ac32aa6 \
-    --hash=sha256:c46956ed82961e31557b6857a5ca153c67e5476972e5f7190015018760938da2 \
-    --hash=sha256:c7c8b816c2b5af5c8a436df44ca08258fc1a13b449393a91484225fcb7545533 \
-    --hash=sha256:cd73265a9e5ea618014802ab01babf1940cecb90c9762d8b9e7d2cc1e1969ec6 \
-    --hash=sha256:dad46e6f620574b3b4801c68255492e0159d1712271cc99d8bdf35f2043ec266 \
-    --hash=sha256:dc9b311743a78043b26ffaeeb9715dc360335e5517832f5a8e339f8a43581e4d \
-    --hash=sha256:df822ee7feaaeffb99c1a9e5e608800bd8eda6e5f18f5cfb0dc7eeb2eaa6bbec \
-    --hash=sha256:e083c285857b78ee21a96ba1eb1b5339733c3563f72980728ca2b08b53826ca5 \
-    --hash=sha256:e5e46b578c0e9db71d04c4b506a2121c0cb371dd89af17a0586ff6769d4c58c1 \
-    --hash=sha256:e99abf0bba688259a496f966211c49a514e65afa9b3073a1fcee08856e04425b \
-    --hash=sha256:ee43080e75fc92bf36219926c8e6de497f9b247301bbf88c5c7593d931426679 \
-    --hash=sha256:f033d80bc6283092613882dfe40419c6a6a1527e04fc69350e87a9df02bbc283 \
-    --hash=sha256:f1088fa100bf46e7b398ffd9904f4808a0612e1d966b4aa43baa535d1b6341eb \
-    --hash=sha256:f56455b0c2c7cc3b0c584815264461d07b177f903a04481dfc33e08a89f0c26b \
-    --hash=sha256:f59dfe57bb1ec82ac0698ebfcdb7bcd0e99c255bd637ff613760d5f33e7c81b3 \
-    --hash=sha256:f7217af2e14da0856e082e96ff637f14ae45c10a5714b63c77f26d8884cf1051 \
-    --hash=sha256:f734e38fd8666f53da904c52a23ce517f1b07722118d750405af7e4123933511 \
-    --hash=sha256:f95511dd5d0e05fd9728bac4096319f80615aaef4acbecb35a990afebe953b0e \
-    --hash=sha256:fdd215b7b7fd4a53994f238d0f46b7ba4ac4c0adb12452beee724ddd0743ae5d \
-    --hash=sha256:feeb18a801aacb098220e2c3eea59a512362eb408d4afd0c242044c33ad6d542 \
-    --hash=sha256:ff30218887e62209942f91ac1be902cc80cddb86bf00fbc6783b7a43b2bea26f
+aiohttp==3.9.5 \
+    --hash=sha256:0605cc2c0088fcaae79f01c913a38611ad09ba68ff482402d3410bf59039bfb8 \
+    --hash=sha256:0a158704edf0abcac8ac371fbb54044f3270bdbc93e254a82b6c82be1ef08f3c \
+    --hash=sha256:0cbf56238f4bbf49dab8c2dc2e6b1b68502b1e88d335bea59b3f5b9f4c001475 \
+    --hash=sha256:1732102949ff6087589408d76cd6dea656b93c896b011ecafff418c9661dc4ed \
+    --hash=sha256:18f634d540dd099c262e9f887c8bbacc959847cfe5da7a0e2e1cf3f14dbf2daf \
+    --hash=sha256:239f975589a944eeb1bad26b8b140a59a3a320067fb3cd10b75c3092405a1372 \
+    --hash=sha256:2faa61a904b83142747fc6a6d7ad8fccff898c849123030f8e75d5d967fd4a81 \
+    --hash=sha256:320e8618eda64e19d11bdb3bd04ccc0a816c17eaecb7e4945d01deee2a22f95f \
+    --hash=sha256:38d80498e2e169bc61418ff36170e0aad0cd268da8b38a17c4cf29d254a8b3f1 \
+    --hash=sha256:3916c8692dbd9d55c523374a3b8213e628424d19116ac4308e434dbf6d95bbdd \
+    --hash=sha256:393c7aba2b55559ef7ab791c94b44f7482a07bf7640d17b341b79081f5e5cd1a \
+    --hash=sha256:3b7b30258348082826d274504fbc7c849959f1989d86c29bc355107accec6cfb \
+    --hash=sha256:3fcb4046d2904378e3aeea1df51f697b0467f2aac55d232c87ba162709478c46 \
+    --hash=sha256:4109adee842b90671f1b689901b948f347325045c15f46b39797ae1bf17019de \
+    --hash=sha256:4558e5012ee03d2638c681e156461d37b7a113fe13970d438d95d10173d25f78 \
+    --hash=sha256:45731330e754f5811c314901cebdf19dd776a44b31927fa4b4dbecab9e457b0c \
+    --hash=sha256:4715a9b778f4293b9f8ae7a0a7cef9829f02ff8d6277a39d7f40565c737d3771 \
+    --hash=sha256:471f0ef53ccedec9995287f02caf0c068732f026455f07db3f01a46e49d76bbb \
+    --hash=sha256:4d3ebb9e1316ec74277d19c5f482f98cc65a73ccd5430540d6d11682cd857430 \
+    --hash=sha256:4ff550491f5492ab5ed3533e76b8567f4b37bd2995e780a1f46bca2024223233 \
+    --hash=sha256:52c27110f3862a1afbcb2af4281fc9fdc40327fa286c4625dfee247c3ba90156 \
+    --hash=sha256:55b39c8684a46e56ef8c8d24faf02de4a2b2ac60d26cee93bc595651ff545de9 \
+    --hash=sha256:5a7ee16aab26e76add4afc45e8f8206c95d1d75540f1039b84a03c3b3800dd59 \
+    --hash=sha256:5ca51eadbd67045396bc92a4345d1790b7301c14d1848feaac1d6a6c9289e888 \
+    --hash=sha256:5d6b3f1fabe465e819aed2c421a6743d8debbde79b6a8600739300630a01bf2c \
+    --hash=sha256:60cdbd56f4cad9f69c35eaac0fbbdf1f77b0ff9456cebd4902f3dd1cf096464c \
+    --hash=sha256:6380c039ec52866c06d69b5c7aad5478b24ed11696f0e72f6b807cfb261453da \
+    --hash=sha256:639d0042b7670222f33b0028de6b4e2fad6451462ce7df2af8aee37dcac55424 \
+    --hash=sha256:66331d00fb28dc90aa606d9a54304af76b335ae204d1836f65797d6fe27f1ca2 \
+    --hash=sha256:67c3119f5ddc7261d47163ed86d760ddf0e625cd6246b4ed852e82159617b5fb \
+    --hash=sha256:694d828b5c41255e54bc2dddb51a9f5150b4eefa9886e38b52605a05d96566e8 \
+    --hash=sha256:6ae79c1bc12c34082d92bf9422764f799aee4746fd7a392db46b7fd357d4a17a \
+    --hash=sha256:702e2c7c187c1a498a4e2b03155d52658fdd6fda882d3d7fbb891a5cf108bb10 \
+    --hash=sha256:714d4e5231fed4ba2762ed489b4aec07b2b9953cf4ee31e9871caac895a839c0 \
+    --hash=sha256:7b179eea70833c8dee51ec42f3b4097bd6370892fa93f510f76762105568cf09 \
+    --hash=sha256:7f64cbd44443e80094309875d4f9c71d0401e966d191c3d469cde4642bc2e031 \
+    --hash=sha256:82a6a97d9771cb48ae16979c3a3a9a18b600a8505b1115cfe354dfb2054468b4 \
+    --hash=sha256:84dabd95154f43a2ea80deffec9cb44d2e301e38a0c9d331cc4aa0166fe28ae3 \
+    --hash=sha256:8676e8fd73141ded15ea586de0b7cda1542960a7b9ad89b2b06428e97125d4fa \
+    --hash=sha256:88e311d98cc0bf45b62fc46c66753a83445f5ab20038bcc1b8a1cc05666f428a \
+    --hash=sha256:8b4f72fbb66279624bfe83fd5eb6aea0022dad8eec62b71e7bf63ee1caadeafe \
+    --hash=sha256:8c64a6dc3fe5db7b1b4d2b5cb84c4f677768bdc340611eca673afb7cf416ef5a \
+    --hash=sha256:8cf142aa6c1a751fcb364158fd710b8a9be874b81889c2bd13aa8893197455e2 \
+    --hash=sha256:8d1964eb7617907c792ca00b341b5ec3e01ae8c280825deadbbd678447b127e1 \
+    --hash=sha256:93e22add827447d2e26d67c9ac0161756007f152fdc5210277d00a85f6c92323 \
+    --hash=sha256:9c69e77370cce2d6df5d12b4e12bdcca60c47ba13d1cbbc8645dd005a20b738b \
+    --hash=sha256:9dbc053ac75ccc63dc3a3cc547b98c7258ec35a215a92bd9f983e0aac95d3d5b \
+    --hash=sha256:9e3a1ae66e3d0c17cf65c08968a5ee3180c5a95920ec2731f53343fac9bad106 \
+    --hash=sha256:a6ea1a5b409a85477fd8e5ee6ad8f0e40bf2844c270955e09360418cfd09abac \
+    --hash=sha256:a81b1143d42b66ffc40a441379387076243ef7b51019204fd3ec36b9f69e77d6 \
+    --hash=sha256:ad7f2919d7dac062f24d6f5fe95d401597fbb015a25771f85e692d043c9d7832 \
+    --hash=sha256:afc52b8d969eff14e069a710057d15ab9ac17cd4b6753042c407dcea0e40bf75 \
+    --hash=sha256:b3df71da99c98534be076196791adca8819761f0bf6e08e07fd7da25127150d6 \
+    --hash=sha256:c088c4d70d21f8ca5c0b8b5403fe84a7bc8e024161febdd4ef04575ef35d474d \
+    --hash=sha256:c26959ca7b75ff768e2776d8055bf9582a6267e24556bb7f7bd29e677932be72 \
+    --hash=sha256:c413016880e03e69d166efb5a1a95d40f83d5a3a648d16486592c49ffb76d0db \
+    --hash=sha256:c6021d296318cb6f9414b48e6a439a7f5d1f665464da507e8ff640848ee2a58a \
+    --hash=sha256:c671dc117c2c21a1ca10c116cfcd6e3e44da7fcde37bf83b2be485ab377b25da \
+    --hash=sha256:c7a4b7a6cf5b6eb11e109a9755fd4fda7d57395f8c575e166d363b9fc3ec4678 \
+    --hash=sha256:c8a02fbeca6f63cb1f0475c799679057fc9268b77075ab7cf3f1c600e81dd46b \
+    --hash=sha256:cd2adf5c87ff6d8b277814a28a535b59e20bfea40a101db6b3bdca7e9926bc24 \
+    --hash=sha256:d1469f228cd9ffddd396d9948b8c9cd8022b6d1bf1e40c6f25b0fb90b4f893ed \
+    --hash=sha256:d153f652a687a8e95ad367a86a61e8d53d528b0530ef382ec5aaf533140ed00f \
+    --hash=sha256:d5ab8e1f6bee051a4bf6195e38a5c13e5e161cb7bad83d8854524798bd9fcd6e \
+    --hash=sha256:da00da442a0e31f1c69d26d224e1efd3a1ca5bcbf210978a2ca7426dfcae9f58 \
+    --hash=sha256:da22dab31d7180f8c3ac7c7635f3bcd53808f374f6aa333fe0b0b9e14b01f91a \
+    --hash=sha256:e0ae53e33ee7476dd3d1132f932eeb39bf6125083820049d06edcdca4381f342 \
+    --hash=sha256:e7a6a8354f1b62e15d48e04350f13e726fa08b62c3d7b8401c0a1314f02e3558 \
+    --hash=sha256:e9a3d838441bebcf5cf442700e3963f58b5c33f015341f9ea86dcd7d503c07e2 \
+    --hash=sha256:edea7d15772ceeb29db4aff55e482d4bcfb6ae160ce144f2682de02f6d693551 \
+    --hash=sha256:f22eb3a6c1080d862befa0a89c380b4dafce29dc6cd56083f630073d102eb595 \
+    --hash=sha256:f26383adb94da5e7fb388d441bf09c61e5e35f455a3217bfd790c6b6bc64b2ee \
+    --hash=sha256:f3c2890ca8c59ee683fd09adf32321a40fe1cf164e3387799efb2acebf090c11 \
+    --hash=sha256:f64fd07515dad67f24b6ea4a66ae2876c01031de91c93075b8093f07c0a2d93d \
+    --hash=sha256:fcde4c397f673fdec23e6b05ebf8d4751314fa7c24f93334bf1f1364c1c69ac7 \
+    --hash=sha256:ff84aeb864e0fac81f676be9f4685f0527b660f1efdc40dcede3c251ef1e867f
     # via -r requirements.in
 aiosignal==1.3.1 \
     --hash=sha256:54cd96e15e1649b75d6c87526a6ff0b6c1b0dd3459f43d9ca11d48c339b68cfc \
     --hash=sha256:f8376fb07dd1e86a584e4fcdec80b36b7f81aac666ebc724e2c090300dd83b17
     # via aiohttp
 async-timeout==4.0.3 \
     --hash=sha256:4640d96be84d82d02ed59ea2b7105a0f7b33abe8703703cd0ab0bf87c427522f \
@@ -148,51 +148,51 @@
     --hash=sha256:fa3a0128b152627161ce47201262d3140edb5a5c3da88d73a1b790a959126956 \
     --hash=sha256:fcc8eb6d5902bb1cf6dc4f187ee3ea80a1eba0a89aba40a5cb20a5087d961357
     # via cryptography
 click==8.1.7 \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
     # via -r requirements.in
-cryptography==42.0.5 \
-    --hash=sha256:0270572b8bd2c833c3981724b8ee9747b3ec96f699a9665470018594301439ee \
-    --hash=sha256:111a0d8553afcf8eb02a4fea6ca4f59d48ddb34497aa8706a6cf536f1a5ec576 \
-    --hash=sha256:16a48c23a62a2f4a285699dba2e4ff2d1cff3115b9df052cdd976a18856d8e3d \
-    --hash=sha256:1b95b98b0d2af784078fa69f637135e3c317091b615cd0905f8b8a087e86fa30 \
-    --hash=sha256:1f71c10d1e88467126f0efd484bd44bca5e14c664ec2ede64c32f20875c0d413 \
-    --hash=sha256:2424ff4c4ac7f6b8177b53c17ed5d8fa74ae5955656867f5a8affaca36a27abb \
-    --hash=sha256:2bce03af1ce5a5567ab89bd90d11e7bbdff56b8af3acbbec1faded8f44cb06da \
-    --hash=sha256:329906dcc7b20ff3cad13c069a78124ed8247adcac44b10bea1130e36caae0b4 \
-    --hash=sha256:37dd623507659e08be98eec89323469e8c7b4c1407c85112634ae3dbdb926fdd \
-    --hash=sha256:3eaafe47ec0d0ffcc9349e1708be2aaea4c6dd4978d76bf6eb0cb2c13636c6fc \
-    --hash=sha256:5e6275c09d2badf57aea3afa80d975444f4be8d3bc58f7f80d2a484c6f9485c8 \
-    --hash=sha256:6fe07eec95dfd477eb9530aef5bead34fec819b3aaf6c5bd6d20565da607bfe1 \
-    --hash=sha256:7367d7b2eca6513681127ebad53b2582911d1736dc2ffc19f2c3ae49997496bc \
-    --hash=sha256:7cde5f38e614f55e28d831754e8a3bacf9ace5d1566235e39d91b35502d6936e \
-    --hash=sha256:9481ffe3cf013b71b2428b905c4f7a9a4f76ec03065b05ff499bb5682a8d9ad8 \
-    --hash=sha256:98d8dc6d012b82287f2c3d26ce1d2dd130ec200c8679b6213b3c73c08b2b7940 \
-    --hash=sha256:a011a644f6d7d03736214d38832e030d8268bcff4a41f728e6030325fea3e400 \
-    --hash=sha256:a2913c5375154b6ef2e91c10b5720ea6e21007412f6437504ffea2109b5a33d7 \
-    --hash=sha256:a30596bae9403a342c978fb47d9b0ee277699fa53bbafad14706af51fe543d16 \
-    --hash=sha256:b03c2ae5d2f0fc05f9a2c0c997e1bc18c8229f392234e8a0194f202169ccd278 \
-    --hash=sha256:b6cd2203306b63e41acdf39aa93b86fb566049aeb6dc489b70e34bcd07adca74 \
-    --hash=sha256:b7ffe927ee6531c78f81aa17e684e2ff617daeba7f189f911065b2ea2d526dec \
-    --hash=sha256:b8cac287fafc4ad485b8a9b67d0ee80c66bf3574f655d3b97ef2e1082360faf1 \
-    --hash=sha256:ba334e6e4b1d92442b75ddacc615c5476d4ad55cc29b15d590cc6b86efa487e2 \
-    --hash=sha256:ba3e4a42397c25b7ff88cdec6e2a16c2be18720f317506ee25210f6d31925f9c \
-    --hash=sha256:c41fb5e6a5fe9ebcd58ca3abfeb51dffb5d83d6775405305bfa8715b76521922 \
-    --hash=sha256:cd2030f6650c089aeb304cf093f3244d34745ce0cfcc39f20c6fbfe030102e2a \
-    --hash=sha256:cd65d75953847815962c84a4654a84850b2bb4aed3f26fadcc1c13892e1e29f6 \
-    --hash=sha256:e4985a790f921508f36f81831817cbc03b102d643b5fcb81cd33df3fa291a1a1 \
-    --hash=sha256:e807b3188f9eb0eaa7bbb579b462c5ace579f1cedb28107ce8b48a9f7ad3679e \
-    --hash=sha256:f12764b8fffc7a123f641d7d049d382b73f96a34117e0b637b80643169cec8ac \
-    --hash=sha256:f8837fe1d6ac4a8052a9a8ddab256bc006242696f03368a4009be7ee3075cdb7
+cryptography==42.0.7 \
+    --hash=sha256:02c0eee2d7133bdbbc5e24441258d5d2244beb31da5ed19fbb80315f4bbbff55 \
+    --hash=sha256:0d563795db98b4cd57742a78a288cdbdc9daedac29f2239793071fe114f13785 \
+    --hash=sha256:16268d46086bb8ad5bf0a2b5544d8a9ed87a0e33f5e77dd3c3301e63d941a83b \
+    --hash=sha256:1a58839984d9cb34c855197043eaae2c187d930ca6d644612843b4fe8513c886 \
+    --hash=sha256:2954fccea107026512b15afb4aa664a5640cd0af630e2ee3962f2602693f0c82 \
+    --hash=sha256:2e47577f9b18723fa294b0ea9a17d5e53a227867a0a4904a1a076d1646d45ca1 \
+    --hash=sha256:31adb7d06fe4383226c3e963471f6837742889b3c4caa55aac20ad951bc8ffda \
+    --hash=sha256:3577d029bc3f4827dd5bf8bf7710cac13527b470bbf1820a3f394adb38ed7d5f \
+    --hash=sha256:36017400817987670037fbb0324d71489b6ead6231c9604f8fc1f7d008087c68 \
+    --hash=sha256:362e7197754c231797ec45ee081f3088a27a47c6c01eff2ac83f60f85a50fe60 \
+    --hash=sha256:3de9a45d3b2b7d8088c3fbf1ed4395dfeff79d07842217b38df14ef09ce1d8d7 \
+    --hash=sha256:4f698edacf9c9e0371112792558d2f705b5645076cc0aaae02f816a0171770fd \
+    --hash=sha256:5482e789294854c28237bba77c4c83be698be740e31a3ae5e879ee5444166582 \
+    --hash=sha256:5e44507bf8d14b36b8389b226665d597bc0f18ea035d75b4e53c7b1ea84583cc \
+    --hash=sha256:779245e13b9a6638df14641d029add5dc17edbef6ec915688f3acb9e720a5858 \
+    --hash=sha256:789caea816c6704f63f6241a519bfa347f72fbd67ba28d04636b7c6b7da94b0b \
+    --hash=sha256:7f8b25fa616d8b846aef64b15c606bb0828dbc35faf90566eb139aa9cff67af2 \
+    --hash=sha256:8cb8ce7c3347fcf9446f201dc30e2d5a3c898d009126010cbd1f443f28b52678 \
+    --hash=sha256:93a3209f6bb2b33e725ed08ee0991b92976dfdcf4e8b38646540674fc7508e13 \
+    --hash=sha256:a3a5ac8b56fe37f3125e5b72b61dcde43283e5370827f5233893d461b7360cd4 \
+    --hash=sha256:a47787a5e3649008a1102d3df55424e86606c9bae6fb77ac59afe06d234605f8 \
+    --hash=sha256:a79165431551042cc9d1d90e6145d5d0d3ab0f2d66326c201d9b0e7f5bf43604 \
+    --hash=sha256:a987f840718078212fdf4504d0fd4c6effe34a7e4740378e59d47696e8dfb477 \
+    --hash=sha256:a9bc127cdc4ecf87a5ea22a2556cab6c7eda2923f84e4f3cc588e8470ce4e42e \
+    --hash=sha256:bd13b5e9b543532453de08bcdc3cc7cebec6f9883e886fd20a92f26940fd3e7a \
+    --hash=sha256:c65f96dad14f8528a447414125e1fc8feb2ad5a272b8f68477abbcc1ea7d94b9 \
+    --hash=sha256:d8e3098721b84392ee45af2dd554c947c32cc52f862b6a3ae982dbb90f577f14 \
+    --hash=sha256:e6b79d0adb01aae87e8a44c2b64bc3f3fe59515280e00fb6d57a7267a2583cda \
+    --hash=sha256:e6b8f1881dac458c34778d0a424ae5769de30544fc678eac51c1c8bb2183e9da \
+    --hash=sha256:e9b2a6309f14c0497f348d08a065d52f3020656f675819fc405fb63bbcd26562 \
+    --hash=sha256:ecbfbc00bf55888edda9868a4cf927205de8499e7fabe6c050322298382953f2 \
+    --hash=sha256:efd0bf5205240182e0f13bcaea41be4fdf5c22c5129fc7ced4a0282ac86998c9
     # via -r requirements.in
-ecdsa==0.18.0 \
-    --hash=sha256:190348041559e21b22a1d65cee485282ca11a6f81d503fddb84d5017e9ed1e49 \
-    --hash=sha256:80600258e7ed2f16b9aa1d7c295bd70194109ad5a30fdee0eaeefef1d4c559dd
+ecdsa==0.19.0 \
+    --hash=sha256:2cea9b88407fdac7bbeca0833b189e4c9c53f2ef1e1eaa29f6224dbc809b707a \
+    --hash=sha256:60eaad1199659900dd0af521ed462b793bbdf867432b3948e87416ae4caf6bf8
     # via -r requirements.in
 frozenlist==1.4.1 \
     --hash=sha256:04ced3e6a46b4cfffe20f9ae482818e34eba9b5fb0ce4056e4cc9b6e212d09b7 \
     --hash=sha256:0633c8d5337cb5c77acbccc6357ac49a1770b8c487e5b3505c57b949b4b82e98 \
     --hash=sha256:068b63f23b17df8569b7fdca5517edef76171cf3897eb68beb01341131fbd2ad \
     --hash=sha256:0c250a29735d4f15321007fb02865f0e6b6a41a6b88f1f523ca1596ab5f50bd5 \
     --hash=sha256:1979bc0aeb89b33b588c51c54ab0161791149f2461ea7c7c946d95d5f93b56ae \
@@ -267,99 +267,115 @@
     --hash=sha256:fb3c2db03683b5767dedb5769b8a40ebb47d6f7f45b1b3e3b4b51ec8ad9d9825 \
     --hash=sha256:fbeb989b5cc29e8daf7f976b421c220f1b8c731cbf22b9130d8815418ea45887 \
     --hash=sha256:fde5bd59ab5357e3853313127f4d3565fc7dad314a74d7b5d43c22c6a5ed2ced \
     --hash=sha256:fe1a06da377e3a1062ae5fe0926e12b84eceb8a50b350ddca72dc85015873f74
     # via
     #   aiohttp
     #   aiosignal
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via yarl
-multidict==6.0.4 \
-    --hash=sha256:01a3a55bd90018c9c080fbb0b9f4891db37d148a0a18722b42f94694f8b6d4c9 \
-    --hash=sha256:0b1a97283e0c85772d613878028fec909f003993e1007eafa715b24b377cb9b8 \
-    --hash=sha256:0dfad7a5a1e39c53ed00d2dd0c2e36aed4650936dc18fd9a1826a5ae1cad6f03 \
-    --hash=sha256:11bdf3f5e1518b24530b8241529d2050014c884cf18b6fc69c0c2b30ca248710 \
-    --hash=sha256:1502e24330eb681bdaa3eb70d6358e818e8e8f908a22a1851dfd4e15bc2f8161 \
-    --hash=sha256:16ab77bbeb596e14212e7bab8429f24c1579234a3a462105cda4a66904998664 \
-    --hash=sha256:16d232d4e5396c2efbbf4f6d4df89bfa905eb0d4dc5b3549d872ab898451f569 \
-    --hash=sha256:21a12c4eb6ddc9952c415f24eef97e3e55ba3af61f67c7bc388dcdec1404a067 \
-    --hash=sha256:27c523fbfbdfd19c6867af7346332b62b586eed663887392cff78d614f9ec313 \
-    --hash=sha256:281af09f488903fde97923c7744bb001a9b23b039a909460d0f14edc7bf59706 \
-    --hash=sha256:33029f5734336aa0d4c0384525da0387ef89148dc7191aae00ca5fb23d7aafc2 \
-    --hash=sha256:3601a3cece3819534b11d4efc1eb76047488fddd0c85a3948099d5da4d504636 \
-    --hash=sha256:3666906492efb76453c0e7b97f2cf459b0682e7402c0489a95484965dbc1da49 \
-    --hash=sha256:36c63aaa167f6c6b04ef2c85704e93af16c11d20de1d133e39de6a0e84582a93 \
-    --hash=sha256:39ff62e7d0f26c248b15e364517a72932a611a9b75f35b45be078d81bdb86603 \
-    --hash=sha256:43644e38f42e3af682690876cff722d301ac585c5b9e1eacc013b7a3f7b696a0 \
-    --hash=sha256:4372381634485bec7e46718edc71528024fcdc6f835baefe517b34a33c731d60 \
-    --hash=sha256:458f37be2d9e4c95e2d8866a851663cbc76e865b78395090786f6cd9b3bbf4f4 \
-    --hash=sha256:45e1ecb0379bfaab5eef059f50115b54571acfbe422a14f668fc8c27ba410e7e \
-    --hash=sha256:4b9d9e4e2b37daddb5c23ea33a3417901fa7c7b3dee2d855f63ee67a0b21e5b1 \
-    --hash=sha256:4ceef517eca3e03c1cceb22030a3e39cb399ac86bff4e426d4fc6ae49052cc60 \
-    --hash=sha256:4d1a3d7ef5e96b1c9e92f973e43aa5e5b96c659c9bc3124acbbd81b0b9c8a951 \
-    --hash=sha256:4dcbb0906e38440fa3e325df2359ac6cb043df8e58c965bb45f4e406ecb162cc \
-    --hash=sha256:509eac6cf09c794aa27bcacfd4d62c885cce62bef7b2c3e8b2e49d365b5003fe \
-    --hash=sha256:52509b5be062d9eafc8170e53026fbc54cf3b32759a23d07fd935fb04fc22d95 \
-    --hash=sha256:52f2dffc8acaba9a2f27174c41c9e57f60b907bb9f096b36b1a1f3be71c6284d \
-    --hash=sha256:574b7eae1ab267e5f8285f0fe881f17efe4b98c39a40858247720935b893bba8 \
-    --hash=sha256:5979b5632c3e3534e42ca6ff856bb24b2e3071b37861c2c727ce220d80eee9ed \
-    --hash=sha256:59d43b61c59d82f2effb39a93c48b845efe23a3852d201ed2d24ba830d0b4cf2 \
-    --hash=sha256:5a4dcf02b908c3b8b17a45fb0f15b695bf117a67b76b7ad18b73cf8e92608775 \
-    --hash=sha256:5cad9430ab3e2e4fa4a2ef4450f548768400a2ac635841bc2a56a2052cdbeb87 \
-    --hash=sha256:5fc1b16f586f049820c5c5b17bb4ee7583092fa0d1c4e28b5239181ff9532e0c \
-    --hash=sha256:62501642008a8b9871ddfccbf83e4222cf8ac0d5aeedf73da36153ef2ec222d2 \
-    --hash=sha256:64bdf1086b6043bf519869678f5f2757f473dee970d7abf6da91ec00acb9cb98 \
-    --hash=sha256:64da238a09d6039e3bd39bb3aee9c21a5e34f28bfa5aa22518581f910ff94af3 \
-    --hash=sha256:666daae833559deb2d609afa4490b85830ab0dfca811a98b70a205621a6109fe \
-    --hash=sha256:67040058f37a2a51ed8ea8f6b0e6ee5bd78ca67f169ce6122f3e2ec80dfe9b78 \
-    --hash=sha256:6748717bb10339c4760c1e63da040f5f29f5ed6e59d76daee30305894069a660 \
-    --hash=sha256:6b181d8c23da913d4ff585afd1155a0e1194c0b50c54fcfe286f70cdaf2b7176 \
-    --hash=sha256:6ed5f161328b7df384d71b07317f4d8656434e34591f20552c7bcef27b0ab88e \
-    --hash=sha256:7582a1d1030e15422262de9f58711774e02fa80df0d1578995c76214f6954988 \
-    --hash=sha256:7d18748f2d30f94f498e852c67d61261c643b349b9d2a581131725595c45ec6c \
-    --hash=sha256:7d6ae9d593ef8641544d6263c7fa6408cc90370c8cb2bbb65f8d43e5b0351d9c \
-    --hash=sha256:81a4f0b34bd92df3da93315c6a59034df95866014ac08535fc819f043bfd51f0 \
-    --hash=sha256:8316a77808c501004802f9beebde51c9f857054a0c871bd6da8280e718444449 \
-    --hash=sha256:853888594621e6604c978ce2a0444a1e6e70c8d253ab65ba11657659dcc9100f \
-    --hash=sha256:99b76c052e9f1bc0721f7541e5e8c05db3941eb9ebe7b8553c625ef88d6eefde \
-    --hash=sha256:a2e4369eb3d47d2034032a26c7a80fcb21a2cb22e1173d761a162f11e562caa5 \
-    --hash=sha256:ab55edc2e84460694295f401215f4a58597f8f7c9466faec545093045476327d \
-    --hash=sha256:af048912e045a2dc732847d33821a9d84ba553f5c5f028adbd364dd4765092ac \
-    --hash=sha256:b1a2eeedcead3a41694130495593a559a668f382eee0727352b9a41e1c45759a \
-    --hash=sha256:b1e8b901e607795ec06c9e42530788c45ac21ef3aaa11dbd0c69de543bfb79a9 \
-    --hash=sha256:b41156839806aecb3641f3208c0dafd3ac7775b9c4c422d82ee2a45c34ba81ca \
-    --hash=sha256:b692f419760c0e65d060959df05f2a531945af31fda0c8a3b3195d4efd06de11 \
-    --hash=sha256:bc779e9e6f7fda81b3f9aa58e3a6091d49ad528b11ed19f6621408806204ad35 \
-    --hash=sha256:bf6774e60d67a9efe02b3616fee22441d86fab4c6d335f9d2051d19d90a40063 \
-    --hash=sha256:c048099e4c9e9d615545e2001d3d8a4380bd403e1a0578734e0d31703d1b0c0b \
-    --hash=sha256:c5cb09abb18c1ea940fb99360ea0396f34d46566f157122c92dfa069d3e0e982 \
-    --hash=sha256:cc8e1d0c705233c5dd0c5e6460fbad7827d5d36f310a0fadfd45cc3029762258 \
-    --hash=sha256:d5e3fc56f88cc98ef8139255cf8cd63eb2c586531e43310ff859d6bb3a6b51f1 \
-    --hash=sha256:d6aa0418fcc838522256761b3415822626f866758ee0bc6632c9486b179d0b52 \
-    --hash=sha256:d6c254ba6e45d8e72739281ebc46ea5eb5f101234f3ce171f0e9f5cc86991480 \
-    --hash=sha256:d6d635d5209b82a3492508cf5b365f3446afb65ae7ebd755e70e18f287b0adf7 \
-    --hash=sha256:dcfe792765fab89c365123c81046ad4103fcabbc4f56d1c1997e6715e8015461 \
-    --hash=sha256:ddd3915998d93fbcd2566ddf9cf62cdb35c9e093075f862935573d265cf8f65d \
-    --hash=sha256:ddff9c4e225a63a5afab9dd15590432c22e8057e1a9a13d28ed128ecf047bbdc \
-    --hash=sha256:e41b7e2b59679edfa309e8db64fdf22399eec4b0b24694e1b2104fb789207779 \
-    --hash=sha256:e69924bfcdda39b722ef4d9aa762b2dd38e4632b3641b1d9a57ca9cd18f2f83a \
-    --hash=sha256:ea20853c6dbbb53ed34cb4d080382169b6f4554d394015f1bef35e881bf83547 \
-    --hash=sha256:ee2a1ece51b9b9e7752e742cfb661d2a29e7bcdba2d27e66e28a99f1890e4fa0 \
-    --hash=sha256:eeb6dcc05e911516ae3d1f207d4b0520d07f54484c49dfc294d6e7d63b734171 \
-    --hash=sha256:f70b98cd94886b49d91170ef23ec5c0e8ebb6f242d734ed7ed677b24d50c82cf \
-    --hash=sha256:fc35cb4676846ef752816d5be2193a1e8367b4c1397b74a565a9d0389c433a1d \
-    --hash=sha256:ff959bee35038c4624250473988b24f846cbeb2c6639de3602c073f10410ceba
+multidict==6.0.5 \
+    --hash=sha256:01265f5e40f5a17f8241d52656ed27192be03bfa8764d88e8220141d1e4b3556 \
+    --hash=sha256:0275e35209c27a3f7951e1ce7aaf93ce0d163b28948444bec61dd7badc6d3f8c \
+    --hash=sha256:04bde7a7b3de05732a4eb39c94574db1ec99abb56162d6c520ad26f83267de29 \
+    --hash=sha256:04da1bb8c8dbadf2a18a452639771951c662c5ad03aefe4884775454be322c9b \
+    --hash=sha256:09a892e4a9fb47331da06948690ae38eaa2426de97b4ccbfafbdcbe5c8f37ff8 \
+    --hash=sha256:0d63c74e3d7ab26de115c49bffc92cc77ed23395303d496eae515d4204a625e7 \
+    --hash=sha256:107c0cdefe028703fb5dafe640a409cb146d44a6ae201e55b35a4af8e95457dd \
+    --hash=sha256:141b43360bfd3bdd75f15ed811850763555a251e38b2405967f8e25fb43f7d40 \
+    --hash=sha256:14c2976aa9038c2629efa2c148022ed5eb4cb939e15ec7aace7ca932f48f9ba6 \
+    --hash=sha256:19fe01cea168585ba0f678cad6f58133db2aa14eccaf22f88e4a6dccadfad8b3 \
+    --hash=sha256:1d147090048129ce3c453f0292e7697d333db95e52616b3793922945804a433c \
+    --hash=sha256:1d9ea7a7e779d7a3561aade7d596649fbecfa5c08a7674b11b423783217933f9 \
+    --hash=sha256:215ed703caf15f578dca76ee6f6b21b7603791ae090fbf1ef9d865571039ade5 \
+    --hash=sha256:21fd81c4ebdb4f214161be351eb5bcf385426bf023041da2fd9e60681f3cebae \
+    --hash=sha256:220dd781e3f7af2c2c1053da9fa96d9cf3072ca58f057f4c5adaaa1cab8fc442 \
+    --hash=sha256:228b644ae063c10e7f324ab1ab6b548bdf6f8b47f3ec234fef1093bc2735e5f9 \
+    --hash=sha256:29bfeb0dff5cb5fdab2023a7a9947b3b4af63e9c47cae2a10ad58394b517fddc \
+    --hash=sha256:2f4848aa3baa109e6ab81fe2006c77ed4d3cd1e0ac2c1fbddb7b1277c168788c \
+    --hash=sha256:2faa5ae9376faba05f630d7e5e6be05be22913782b927b19d12b8145968a85ea \
+    --hash=sha256:2ffc42c922dbfddb4a4c3b438eb056828719f07608af27d163191cb3e3aa6cc5 \
+    --hash=sha256:37b15024f864916b4951adb95d3a80c9431299080341ab9544ed148091b53f50 \
+    --hash=sha256:3cc2ad10255f903656017363cd59436f2111443a76f996584d1077e43ee51182 \
+    --hash=sha256:3d25f19500588cbc47dc19081d78131c32637c25804df8414463ec908631e453 \
+    --hash=sha256:403c0911cd5d5791605808b942c88a8155c2592e05332d2bf78f18697a5fa15e \
+    --hash=sha256:411bf8515f3be9813d06004cac41ccf7d1cd46dfe233705933dd163b60e37600 \
+    --hash=sha256:425bf820055005bfc8aa9a0b99ccb52cc2f4070153e34b701acc98d201693733 \
+    --hash=sha256:435a0984199d81ca178b9ae2c26ec3d49692d20ee29bc4c11a2a8d4514c67eda \
+    --hash=sha256:4a6a4f196f08c58c59e0b8ef8ec441d12aee4125a7d4f4fef000ccb22f8d7241 \
+    --hash=sha256:4cc0ef8b962ac7a5e62b9e826bd0cd5040e7d401bc45a6835910ed699037a461 \
+    --hash=sha256:51d035609b86722963404f711db441cf7134f1889107fb171a970c9701f92e1e \
+    --hash=sha256:53689bb4e102200a4fafa9de9c7c3c212ab40a7ab2c8e474491914d2305f187e \
+    --hash=sha256:55205d03e8a598cfc688c71ca8ea5f66447164efff8869517f175ea632c7cb7b \
+    --hash=sha256:5c0631926c4f58e9a5ccce555ad7747d9a9f8b10619621f22f9635f069f6233e \
+    --hash=sha256:5cb241881eefd96b46f89b1a056187ea8e9ba14ab88ba632e68d7a2ecb7aadf7 \
+    --hash=sha256:60d698e8179a42ec85172d12f50b1668254628425a6bd611aba022257cac1386 \
+    --hash=sha256:612d1156111ae11d14afaf3a0669ebf6c170dbb735e510a7438ffe2369a847fd \
+    --hash=sha256:6214c5a5571802c33f80e6c84713b2c79e024995b9c5897f794b43e714daeec9 \
+    --hash=sha256:6939c95381e003f54cd4c5516740faba40cf5ad3eeff460c3ad1d3e0ea2549bf \
+    --hash=sha256:69db76c09796b313331bb7048229e3bee7928eb62bab5e071e9f7fcc4879caee \
+    --hash=sha256:6bf7a982604375a8d49b6cc1b781c1747f243d91b81035a9b43a2126c04766f5 \
+    --hash=sha256:766c8f7511df26d9f11cd3a8be623e59cca73d44643abab3f8c8c07620524e4a \
+    --hash=sha256:76c0de87358b192de7ea9649beb392f107dcad9ad27276324c24c91774ca5271 \
+    --hash=sha256:76f067f5121dcecf0d63a67f29080b26c43c71a98b10c701b0677e4a065fbd54 \
+    --hash=sha256:7901c05ead4b3fb75113fb1dd33eb1253c6d3ee37ce93305acd9d38e0b5f21a4 \
+    --hash=sha256:79660376075cfd4b2c80f295528aa6beb2058fd289f4c9252f986751a4cd0496 \
+    --hash=sha256:79a6d2ba910adb2cbafc95dad936f8b9386e77c84c35bc0add315b856d7c3abb \
+    --hash=sha256:7afcdd1fc07befad18ec4523a782cde4e93e0a2bf71239894b8d61ee578c1319 \
+    --hash=sha256:7be7047bd08accdb7487737631d25735c9a04327911de89ff1b26b81745bd4e3 \
+    --hash=sha256:7c6390cf87ff6234643428991b7359b5f59cc15155695deb4eda5c777d2b880f \
+    --hash=sha256:7df704ca8cf4a073334e0427ae2345323613e4df18cc224f647f251e5e75a527 \
+    --hash=sha256:85f67aed7bb647f93e7520633d8f51d3cbc6ab96957c71272b286b2f30dc70ed \
+    --hash=sha256:896ebdcf62683551312c30e20614305f53125750803b614e9e6ce74a96232604 \
+    --hash=sha256:92d16a3e275e38293623ebf639c471d3e03bb20b8ebb845237e0d3664914caef \
+    --hash=sha256:99f60d34c048c5c2fabc766108c103612344c46e35d4ed9ae0673d33c8fb26e8 \
+    --hash=sha256:9fe7b0653ba3d9d65cbe7698cca585bf0f8c83dbbcc710db9c90f478e175f2d5 \
+    --hash=sha256:a3145cb08d8625b2d3fee1b2d596a8766352979c9bffe5d7833e0503d0f0b5e5 \
+    --hash=sha256:aeaf541ddbad8311a87dd695ed9642401131ea39ad7bc8cf3ef3967fd093b626 \
+    --hash=sha256:b55358304d7a73d7bdf5de62494aaf70bd33015831ffd98bc498b433dfe5b10c \
+    --hash=sha256:b82cc8ace10ab5bd93235dfaab2021c70637005e1ac787031f4d1da63d493c1d \
+    --hash=sha256:c0868d64af83169e4d4152ec612637a543f7a336e4a307b119e98042e852ad9c \
+    --hash=sha256:c1c1496e73051918fcd4f58ff2e0f2f3066d1c76a0c6aeffd9b45d53243702cc \
+    --hash=sha256:c9bf56195c6bbd293340ea82eafd0071cb3d450c703d2c93afb89f93b8386ccc \
+    --hash=sha256:cbebcd5bcaf1eaf302617c114aa67569dd3f090dd0ce8ba9e35e9985b41ac35b \
+    --hash=sha256:cd6c8fca38178e12c00418de737aef1261576bd1b6e8c6134d3e729a4e858b38 \
+    --hash=sha256:ceb3b7e6a0135e092de86110c5a74e46bda4bd4fbfeeb3a3bcec79c0f861e450 \
+    --hash=sha256:cf590b134eb70629e350691ecca88eac3e3b8b3c86992042fb82e3cb1830d5e1 \
+    --hash=sha256:d3eb1ceec286eba8220c26f3b0096cf189aea7057b6e7b7a2e60ed36b373b77f \
+    --hash=sha256:d65f25da8e248202bd47445cec78e0025c0fe7582b23ec69c3b27a640dd7a8e3 \
+    --hash=sha256:d6f6d4f185481c9669b9447bf9d9cf3b95a0e9df9d169bbc17e363b7d5487755 \
+    --hash=sha256:d84a5c3a5f7ce6db1f999fb9438f686bc2e09d38143f2d93d8406ed2dd6b9226 \
+    --hash=sha256:d946b0a9eb8aaa590df1fe082cee553ceab173e6cb5b03239716338629c50c7a \
+    --hash=sha256:dce1c6912ab9ff5f179eaf6efe7365c1f425ed690b03341911bf4939ef2f3046 \
+    --hash=sha256:de170c7b4fe6859beb8926e84f7d7d6c693dfe8e27372ce3b76f01c46e489fcf \
+    --hash=sha256:e02021f87a5b6932fa6ce916ca004c4d441509d33bbdbeca70d05dff5e9d2479 \
+    --hash=sha256:e030047e85cbcedbfc073f71836d62dd5dadfbe7531cae27789ff66bc551bd5e \
+    --hash=sha256:e0e79d91e71b9867c73323a3444724d496c037e578a0e1755ae159ba14f4f3d1 \
+    --hash=sha256:e4428b29611e989719874670fd152b6625500ad6c686d464e99f5aaeeaca175a \
+    --hash=sha256:e4972624066095e52b569e02b5ca97dbd7a7ddd4294bf4e7247d52635630dd83 \
+    --hash=sha256:e7be68734bd8c9a513f2b0cfd508802d6609da068f40dc57d4e3494cefc92929 \
+    --hash=sha256:e8e94e6912639a02ce173341ff62cc1201232ab86b8a8fcc05572741a5dc7d93 \
+    --hash=sha256:ea1456df2a27c73ce51120fa2f519f1bea2f4a03a917f4a43c8707cf4cbbae1a \
+    --hash=sha256:ebd8d160f91a764652d3e51ce0d2956b38efe37c9231cd82cfc0bed2e40b581c \
+    --hash=sha256:eca2e9d0cc5a889850e9bbd68e98314ada174ff6ccd1129500103df7a94a7a44 \
+    --hash=sha256:edd08e6f2f1a390bf137080507e44ccc086353c8e98c657e666c017718561b89 \
+    --hash=sha256:f285e862d2f153a70586579c15c44656f888806ed0e5b56b64489afe4a2dbfba \
+    --hash=sha256:f2a1dee728b52b33eebff5072817176c172050d44d67befd681609b4746e1c2e \
+    --hash=sha256:f7e301075edaf50500f0b341543c41194d8df3ae5caf4702f2095f3ca73dd8da \
+    --hash=sha256:fb616be3538599e797a2017cccca78e354c767165e8858ab5116813146041a24 \
+    --hash=sha256:fce28b3c8a81b6b36dfac9feb1de115bab619b3c13905b419ec71d03a3fc1423 \
+    --hash=sha256:fe5d7785250541f7f5019ab9cba2c71169dc7d74d0f45253f8313f436458a4ef
     # via
     #   aiohttp
     #   yarl
-pycparser==2.21 \
-    --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
-    --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
+pycparser==2.22 \
+    --hash=sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6 \
+    --hash=sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc
     # via cffi
 six==1.16.0 \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via ecdsa
 yarl==1.9.4 \
     --hash=sha256:008d3e808d03ef28542372d01057fd09168419cdc8f848efe2804f894ae03e51 \
```

### Comparing `autograph-utils-0.2.0/src/autograph_utils/__init__.py` & `autograph_utils-0.3.0/src/autograph_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,15 +256,15 @@
     certificates that chains back up to some well-known root
     hash. Certificate chains are identified by x5u. x5us are assumed
     to be static and so can be cached to save network traffic.
 
     :params ClientSession session: An aiohttp session, used to retrieve x5us.
     :params Cache cache: A cache used to store results for x5u verification.
     :params bytes root_hash: The expected hash for the first
-        certificate in a chain.  This should not be encoded in any
+        certificate in a chain. Disabled if ``None``. This should not be encoded in any
         way. Hashes can be decoded using decode_mozilla_hash.
     :params SubjectNameCheck subject_name_check: Predicate to use to
         validate cert subject names. Defaults to
         EndsWith(".content-signature.mozilla.org").
 
     """
 
@@ -340,16 +340,17 @@
             if now < cert.not_valid_before:
                 raise CertificateNotYetValid(cert.not_valid_before)
             if now > cert.not_valid_after:
                 raise CertificateExpired(cert.not_valid_after)
 
         # Verify chain of trust.
         chain = certs[::-1]
-        root_hash = chain[0].fingerprint(SHA256())
-        if root_hash != self.root_hash:
+
+        # Check root certificate hash if specified
+        if self.root_hash and self.root_hash != (root_hash := chain[0].fingerprint(SHA256())):
             raise CertificateHasWrongRoot(expected=self.root_hash, actual=root_hash)
 
         current_cert = chain[0]
         for next_cert in chain[1:]:
             self._check_can_sign_other_certs(current_cert)
             self._verify_cert_link(current_cert, next_cert)
             self._check_name_constraints(current_cert, next_cert)
```

### Comparing `autograph-utils-0.2.0/src/autograph_utils.egg-info/PKG-INFO` & `autograph_utils-0.3.0/src/autograph_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autograph-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: autograph-utils is a tool to configure a kinto server from an YAML file.
 Author-email: Mozilla Services <dev-webdev@lists.mozilla.org>
 License: Apache Software License 2.0
         
         Copyright (c) 2019, Ethan Glasser-Camp
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `autograph-utils-0.2.0/src/autograph_utils.egg-info/SOURCES.txt` & `autograph_utils-0.3.0/src/autograph_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autograph-utils-0.2.0/tests/normandy.content-signature.mozilla.org-2019-12-04-18-15-23.chain` & `autograph_utils-0.3.0/tests/normandy.content-signature.mozilla.org-2019-12-04-18-15-23.chain`

 * *Files identical despite different names*

### Comparing `autograph-utils-0.2.0/tests/normandy.content-signature.mozilla.org-20210705.dev.chain` & `autograph_utils-0.3.0/tests/normandy.content-signature.mozilla.org-20210705.dev.chain`

 * *Files identical despite different names*

### Comparing `autograph-utils-0.2.0/tests/test_autograph_utils.py` & `autograph_utils-0.3.0/tests/test_autograph_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os.path
 from unittest import mock
 
 import aiohttp
 import autograph_utils
 import cryptography.x509
 import pytest
+import pytest_asyncio
 from aioresponses import aioresponses
 from autograph_utils import (
     ExactMatch,
     MemoryCache,
     SignatureVerifier,
     decode_mozilla_hash,
     main,
@@ -88,26 +89,27 @@
     with mock.patch("autograph_utils._now") as m:
         # A common static time used in a lot of tests.
         m.return_value = datetime.datetime(2019, 10, 23, 16, 16)
         # Yield the mock so someone can change the time if they want
         yield m
 
 
-@pytest.fixture
-async def aiohttp_session(loop):
+@pytest_asyncio.fixture
+async def aiohttp_session():
     async with aiohttp.ClientSession() as s:
         yield s
 
 
 def mock_cert(real_cert):
     """Utility function to create a mock of a cert that has all the same
     data but can have fields overridden.
 
     """
-    mock_cert = mock.create_autospec(spec=real_cert)
+
+    mock_cert = mock.MagicMock(wraps=real_cert)
     mock_cert.not_valid_before = real_cert.not_valid_before
     mock_cert.not_valid_after = real_cert.not_valid_after
     mock_cert.signature = real_cert.signature
     mock_cert.tbs_certificate_bytes = real_cert.tbs_certificate_bytes
     mock_cert.signature_hash_algorithm = real_cert.signature_hash_algorithm
     mock_cert.subject = real_cert.subject
     mock_cert.extensions = real_cert.extensions
@@ -196,15 +198,15 @@
 
 async def test_verify_x5u_screwy_dates(aiohttp_session, mock_with_x5u, cache, now_fixed):
     now_fixed.return_value = datetime.datetime(2010, 10, 23, 16, 16, 16)
     s = SignatureVerifier(aiohttp_session, cache, DEV_ROOT_HASH)
     leaf_cert = cryptography.x509.load_pem_x509_certificate(
         CERT_LIST[0], backend=default_backend()
     )
-    bad_cert = mock.Mock(spec=leaf_cert)
+    bad_cert = mock_cert(leaf_cert)
     bad_cert.not_valid_before = leaf_cert.not_valid_after
     bad_cert.not_valid_after = leaf_cert.not_valid_before
     with mock.patch("autograph_utils.x509.load_pem_x509_certificate") as x509:
         x509.return_value = bad_cert
         with pytest.raises(autograph_utils.BadCertificate) as excinfo:
             await s.verify(SIGNED_DATA, SAMPLE_SIGNATURE, FAKE_CERT_URL)
 
@@ -258,14 +260,23 @@
     expected = actual[:-1] + "3"
 
     assert excinfo.value.detail == (
         "Certificate is not based on expected root hash. " f"Got '{actual}' expected '{expected}'"
     )
 
 
+async def test_root_hash_is_ignored_if_none(aiohttp_session, mock_with_x5u, cache, now_fixed):
+    s = SignatureVerifier(
+        aiohttp_session,
+        cache,
+        root_hash=None,
+    )
+    await s.verify_x5u(FAKE_CERT_URL)  # not raising
+
+
 async def test_verify_broken_chain(aiohttp_session, mock_aioresponses, cache, now_fixed):
     # Drop next-to-last cert in cert list
     broken_chain = CERT_LIST[:1] + CERT_LIST[2:]
     mock_aioresponses.get(FAKE_CERT_URL, status=200, body=b"\n".join(broken_chain))
     s = SignatureVerifier(aiohttp_session, cache, DEV_ROOT_HASH)
     with pytest.raises(autograph_utils.CertificateChainBroken) as excinfo:
         await s.verify_x5u(FAKE_CERT_URL)
```

