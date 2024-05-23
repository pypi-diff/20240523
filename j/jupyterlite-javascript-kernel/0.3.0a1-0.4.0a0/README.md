# Comparing `tmp/jupyterlite_javascript_kernel-0.3.0a1.tar.gz` & `tmp/jupyterlite_javascript_kernel-0.4.0a0.tar.gz`

## Comparing `jupyterlite_javascript_kernel-0.3.0a1.tar` & `jupyterlite_javascript_kernel-0.4.0a0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/.copier-answers.yml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/.yarnrc.yml
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/CHANGELOG.md
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/RELEASE.md
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/install.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/lerna.json
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/setup.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/tsconfig.eslint.json
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/tsconfig.json
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/tsconfigbase.json
--rw-r--r--   0        0        0   467205 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/yarn.lock
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/_version.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/package.json
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/312.4028241b320224658118.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/312.4028241b320224658118.js.LICENSE.txt
--rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/584.7e49152bd31ca0f8291b.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/584.7e49152bd31ca0f8291b.js.LICENSE.txt
--rw-r--r--   0        0        0    16598 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/5e8d6f34d83488f083fd.png
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/692.d7dd851ce6b7f32bbac2.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/692.d7dd851ce6b7f32bbac2.js.LICENSE.txt
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/804.1ac186e1afa78c8a2770.js
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/b1c098fa349a030dacbe.png
--rw-r--r--   0        0        0     7370 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/remoteEntry.9db3df3efa1ab7d5af05.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/style.js
--rw-r--r--   0        0        0    13115 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/scripts/bump-version.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/.gitignore
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/LICENSE
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/README.md
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/pyproject.toml
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.3.0a1/PKG-INFO
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/.copier-answers.yml
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/.yarnrc.yml
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/CHANGELOG.md
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/RELEASE.md
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/install.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/lerna.json
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/tsconfig.eslint.json
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/tsconfig.json
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/tsconfigbase.json
+-rw-r--r--   0        0        0   469338 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/yarn.lock
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/_version.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/package.json
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/238.453d2599405730ec7a31.js
+-rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/535.46e2f879361140e66596.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/535.46e2f879361140e66596.js.LICENSE.txt
+-rw-r--r--   0        0        0    16598 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/5e8d6f34d83488f083fd.png
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/851.f06be08f4dbb05785c82.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/851.f06be08f4dbb05785c82.js.LICENSE.txt
+-rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/916.6c2158a1e7981a0b119d.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/916.6c2158a1e7981a0b119d.js.LICENSE.txt
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/b1c098fa349a030dacbe.png
+-rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/remoteEntry.bcb6e0c823f3bdb2c1ce.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/style.js
+-rw-r--r--   0        0        0    13115 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/scripts/bump-version.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/.gitignore
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/LICENSE
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/README.md
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     5862 2020-02-02 00:00:00.000000 jupyterlite_javascript_kernel-0.4.0a0/PKG-INFO
```

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/.copier-answers.yml` & `jupyterlite_javascript_kernel-0.4.0a0/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/CHANGELOG.md` & `jupyterlite_javascript_kernel-0.4.0a0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,57 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.4.0a0
+
+([Full Changelog](https://github.com/jupyterlite/javascript-kernel/compare/@jupyterlite/javascript-kernel-extension@0.3.0...d557adf3cd01c6007b64e5a9be185d091c6531c3))
+
+### Maintenance and upkeep improvements
+
+- Update to JupyterLite 0.4.0 [#14](https://github.com/jupyterlite/javascript-kernel/pull/14) ([@jtpio](https://github.com/jtpio))
+- Fix CI [#13](https://github.com/jupyterlite/javascript-kernel/pull/13) ([@jtpio](https://github.com/jtpio))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlite/javascript-kernel/graphs/contributors?from=2024-03-26&to=2024-05-23&type=c))
+
+[@jtpio](https://github.com/search?q=repo%3Ajupyterlite%2Fjavascript-kernel+involves%3Ajtpio+updated%3A2024-03-26..2024-05-23&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
+## 0.3.0
+
+([Full Changelog](https://github.com/jupyterlite/javascript-kernel/compare/@jupyterlite/javascript-kernel-extension@0.3.0-alpha.1...0ec2e58c1ec85fefbb35109e8414f5a2ba97de80))
+
+### Maintenance and upkeep improvements
+
+- Update releaser workflows [#11](https://github.com/jupyterlite/javascript-kernel/pull/11) ([@jtpio](https://github.com/jtpio))
+- Update `@jupyterlite` packages [#10](https://github.com/jupyterlite/javascript-kernel/pull/10) ([@jtpio](https://github.com/jtpio))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlite/javascript-kernel/graphs/contributors?from=2024-02-16&to=2024-03-26&type=c))
+
+[@jtpio](https://github.com/search?q=repo%3Ajupyterlite%2Fjavascript-kernel+involves%3Ajtpio+updated%3A2024-02-16..2024-03-26&type=Issues)
+
 ## 0.3.0a1
 
 ([Full Changelog](https://github.com/jupyterlite/javascript-kernel/compare/v0.3.0a0...24e8d7abb6bd51633233c5bbeac9d54a70e98047))
 
 ### Maintenance and upkeep improvements
 
 - Fix shared packages [#8](https://github.com/jupyterlite/javascript-kernel/pull/8) ([@jtpio](https://github.com/jtpio))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlite/javascript-kernel/graphs/contributors?from=2024-02-15&to=2024-02-16&type=c))
 
 [@jtpio](https://github.com/search?q=repo%3Ajupyterlite%2Fjavascript-kernel+involves%3Ajtpio+updated%3A2024-02-15..2024-02-16&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.3.0a0
 
 ([Full Changelog](https://github.com/jupyterlite/javascript-kernel/compare/123a40c18f04b8aa22a86f2352366153e8ed1706...535e97b683a0fa127a936fbe07e05345794a3674))
 
 ### Maintenance and upkeep improvements
 
 - Update pre-release replace logic [#7](https://github.com/jupyterlite/javascript-kernel/pull/7) ([@jtpio](https://github.com/jtpio))
```

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/RELEASE.md` & `jupyterlite_javascript_kernel-0.4.0a0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/package.json` & `jupyterlite_javascript_kernel-0.4.0a0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.4.0-a0'"}*

```diff
@@ -116,14 +116,14 @@
         "lint:check": "yarn run eslint:check && yarn run prettier:check",
         "prettier": "prettier --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "prettier --list-different \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "publish": "yarn run clean && yarn run build && lerna publish",
         "test": "lerna run test",
         "watch": "lerna run watch"
     },
-    "version": "0.3.0-a1",
+    "version": "0.4.0-a0",
     "workspaces": {
         "packages": [
             "packages/*"
         ]
     }
 }
```

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/tsconfig.json` & `jupyterlite_javascript_kernel-0.4.0a0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/yarn.lock` & `jupyterlite_javascript_kernel-0.4.0a0/yarn.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,80 +1,73 @@
 # This file is generated by running "yarn install" inside your project.
 # Manual changes might be lost - proceed with caution!
 
 __metadata:
   version: 6
   cacheKey: 8
 
-"@aashutoshrathi/word-wrap@npm:^1.2.3":
-  version: 1.2.6
-  resolution: "@aashutoshrathi/word-wrap@npm:1.2.6"
-  checksum: ada901b9e7c680d190f1d012c84217ce0063d8f5c5a7725bb91ec3c5ed99bb7572680eb2d2938a531ccbaec39a95422fcd8a6b4a13110c7d98dd75402f66a0cd
-  languageName: node
-  linkType: hard
-
 "@ampproject/remapping@npm:^2.2.0":
-  version: 2.2.1
-  resolution: "@ampproject/remapping@npm:2.2.1"
+  version: 2.3.0
+  resolution: "@ampproject/remapping@npm:2.3.0"
   dependencies:
-    "@jridgewell/gen-mapping": ^0.3.0
-    "@jridgewell/trace-mapping": ^0.3.9
-  checksum: 03c04fd526acc64a1f4df22651186f3e5ef0a9d6d6530ce4482ec9841269cf7a11dbb8af79237c282d721c5312024ff17529cd72cc4768c11e999b58e2302079
+    "@jridgewell/gen-mapping": ^0.3.5
+    "@jridgewell/trace-mapping": ^0.3.24
+  checksum: d3ad7b89d973df059c4e8e6d7c972cbeb1bb2f18f002a3bd04ae0707da214cb06cc06929b65aa2313b9347463df2914772298bae8b1d7973f246bb3f2ab3e8f0
   languageName: node
   linkType: hard
 
-"@babel/code-frame@npm:^7.0.0, @babel/code-frame@npm:^7.12.13, @babel/code-frame@npm:^7.23.5":
-  version: 7.23.5
-  resolution: "@babel/code-frame@npm:7.23.5"
+"@babel/code-frame@npm:^7.0.0, @babel/code-frame@npm:^7.12.13, @babel/code-frame@npm:^7.23.5, @babel/code-frame@npm:^7.24.2":
+  version: 7.24.2
+  resolution: "@babel/code-frame@npm:7.24.2"
   dependencies:
-    "@babel/highlight": ^7.23.4
-    chalk: ^2.4.2
-  checksum: d90981fdf56a2824a9b14d19a4c0e8db93633fd488c772624b4e83e0ceac6039a27cd298a247c3214faa952bf803ba23696172ae7e7235f3b97f43ba278c569a
+    "@babel/highlight": ^7.24.2
+    picocolors: ^1.0.0
+  checksum: 70e867340cfe09ca5488b2f36372c45cabf43c79a5b6426e6df5ef0611ff5dfa75a57dda841895693de6008f32c21a7c97027a8c7bcabd63a7d17416cbead6f8
   languageName: node
   linkType: hard
 
-"@babel/compat-data@npm:^7.22.6, @babel/compat-data@npm:^7.23.3, @babel/compat-data@npm:^7.23.5":
-  version: 7.23.5
-  resolution: "@babel/compat-data@npm:7.23.5"
-  checksum: 06ce244cda5763295a0ea924728c09bae57d35713b675175227278896946f922a63edf803c322f855a3878323d48d0255a2a3023409d2a123483c8a69ebb4744
+"@babel/compat-data@npm:^7.22.6, @babel/compat-data@npm:^7.23.5, @babel/compat-data@npm:^7.24.4":
+  version: 7.24.4
+  resolution: "@babel/compat-data@npm:7.24.4"
+  checksum: 52ce371658dc7796c9447c9cb3b9c0659370d141b76997f21c5e0028cca4d026ca546b84bc8d157ce7ca30bd353d89f9238504eb8b7aefa9b1f178b4c100c2d4
   languageName: node
   linkType: hard
 
-"@babel/core@npm:^7.10.2, @babel/core@npm:^7.11.6, @babel/core@npm:^7.12.3":
-  version: 7.23.9
-  resolution: "@babel/core@npm:7.23.9"
+"@babel/core@npm:^7.10.2, @babel/core@npm:^7.11.6, @babel/core@npm:^7.12.3, @babel/core@npm:^7.23.9":
+  version: 7.24.5
+  resolution: "@babel/core@npm:7.24.5"
   dependencies:
     "@ampproject/remapping": ^2.2.0
-    "@babel/code-frame": ^7.23.5
-    "@babel/generator": ^7.23.6
+    "@babel/code-frame": ^7.24.2
+    "@babel/generator": ^7.24.5
     "@babel/helper-compilation-targets": ^7.23.6
-    "@babel/helper-module-transforms": ^7.23.3
-    "@babel/helpers": ^7.23.9
-    "@babel/parser": ^7.23.9
-    "@babel/template": ^7.23.9
-    "@babel/traverse": ^7.23.9
-    "@babel/types": ^7.23.9
+    "@babel/helper-module-transforms": ^7.24.5
+    "@babel/helpers": ^7.24.5
+    "@babel/parser": ^7.24.5
+    "@babel/template": ^7.24.0
+    "@babel/traverse": ^7.24.5
+    "@babel/types": ^7.24.5
     convert-source-map: ^2.0.0
     debug: ^4.1.0
     gensync: ^1.0.0-beta.2
     json5: ^2.2.3
     semver: ^6.3.1
-  checksum: 634a511f74db52a5f5a283c1121f25e2227b006c095b84a02a40a9213842489cd82dc7d61cdc74e10b5bcd9bb0a4e28bab47635b54c7e2256d47ab57356e2a76
+  checksum: f4f0eafde12b145f2cb9cc893085e5f1436e1ef265bb3b7d8aa6282515c9b4e740bbd5e2cbc32114adb9afed2dd62c2336758b9fabb7e46e8ba542f76d4f3f80
   languageName: node
   linkType: hard
 
-"@babel/generator@npm:^7.23.6, @babel/generator@npm:^7.7.2":
-  version: 7.23.6
-  resolution: "@babel/generator@npm:7.23.6"
+"@babel/generator@npm:^7.24.5, @babel/generator@npm:^7.7.2":
+  version: 7.24.5
+  resolution: "@babel/generator@npm:7.24.5"
   dependencies:
-    "@babel/types": ^7.23.6
-    "@jridgewell/gen-mapping": ^0.3.2
-    "@jridgewell/trace-mapping": ^0.3.17
+    "@babel/types": ^7.24.5
+    "@jridgewell/gen-mapping": ^0.3.5
+    "@jridgewell/trace-mapping": ^0.3.25
     jsesc: ^2.5.1
-  checksum: 1a1a1c4eac210f174cd108d479464d053930a812798e09fee069377de39a893422df5b5b146199ead7239ae6d3a04697b45fc9ac6e38e0f6b76374390f91fc6c
+  checksum: a08c0ab900b36e1a17863e18e3216153322ea993246fd7a358ba38a31cfb15bab2af1dc178b2adafe4cb8a9f3ab0e0ceafd3fe6e8ca870dffb435b53b2b2a803
   languageName: node
   linkType: hard
 
 "@babel/helper-annotate-as-pure@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-annotate-as-pure@npm:7.22.5"
   dependencies:
@@ -88,43 +81,43 @@
   resolution: "@babel/helper-builder-binary-assignment-operator-visitor@npm:7.22.15"
   dependencies:
     "@babel/types": ^7.22.15
   checksum: 639c697a1c729f9fafa2dd4c9af2e18568190299b5907bd4c2d0bc818fcbd1e83ffeecc2af24327a7faa7ac4c34edd9d7940510a5e66296c19bad17001cf5c7a
   languageName: node
   linkType: hard
 
-"@babel/helper-compilation-targets@npm:^7.22.15, @babel/helper-compilation-targets@npm:^7.22.6, @babel/helper-compilation-targets@npm:^7.23.6":
+"@babel/helper-compilation-targets@npm:^7.22.6, @babel/helper-compilation-targets@npm:^7.23.6":
   version: 7.23.6
   resolution: "@babel/helper-compilation-targets@npm:7.23.6"
   dependencies:
     "@babel/compat-data": ^7.23.5
     "@babel/helper-validator-option": ^7.23.5
     browserslist: ^4.22.2
     lru-cache: ^5.1.1
     semver: ^6.3.1
   checksum: c630b98d4527ac8fe2c58d9a06e785dfb2b73ec71b7c4f2ddf90f814b5f75b547f3c015f110a010fd31f76e3864daaf09f3adcd2f6acdbfb18a8de3a48717590
   languageName: node
   linkType: hard
 
-"@babel/helper-create-class-features-plugin@npm:^7.22.15":
-  version: 7.23.10
-  resolution: "@babel/helper-create-class-features-plugin@npm:7.23.10"
+"@babel/helper-create-class-features-plugin@npm:^7.24.1, @babel/helper-create-class-features-plugin@npm:^7.24.4, @babel/helper-create-class-features-plugin@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helper-create-class-features-plugin@npm:7.24.5"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
     "@babel/helper-environment-visitor": ^7.22.20
     "@babel/helper-function-name": ^7.23.0
-    "@babel/helper-member-expression-to-functions": ^7.23.0
+    "@babel/helper-member-expression-to-functions": ^7.24.5
     "@babel/helper-optimise-call-expression": ^7.22.5
-    "@babel/helper-replace-supers": ^7.22.20
+    "@babel/helper-replace-supers": ^7.24.1
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
-    "@babel/helper-split-export-declaration": ^7.22.6
+    "@babel/helper-split-export-declaration": ^7.24.5
     semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: ff0730c21f0e73b9e314701bca6568bb5885dff2aa3c32b1e2e3d18ed2818f56851b9ffdbe2e8008c9bb94b265a1443883ae4c1ca5dde278ce71ac4218006d68
+  checksum: ea761c1155442620ee02920ec7c3190f869ff4d4fcab48a021a11fd8a46c046ed1facb070e5c76539c2b7efc2c8338f50f08a5e49d0ebf12e48743570e92247b
   languageName: node
   linkType: hard
 
 "@babel/helper-create-regexp-features-plugin@npm:^7.18.6, @babel/helper-create-regexp-features-plugin@npm:^7.22.15, @babel/helper-create-regexp-features-plugin@npm:^7.22.5":
   version: 7.22.15
   resolution: "@babel/helper-create-regexp-features-plugin@npm:7.22.15"
   dependencies:
@@ -133,37 +126,37 @@
     semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: 0243b8d4854f1dc8861b1029a46d3f6393ad72f366a5a08e36a4648aa682044f06da4c6e87a456260e1e1b33c999f898ba591a0760842c1387bcc93fbf2151a6
   languageName: node
   linkType: hard
 
-"@babel/helper-define-polyfill-provider@npm:^0.5.0":
-  version: 0.5.0
-  resolution: "@babel/helper-define-polyfill-provider@npm:0.5.0"
+"@babel/helper-define-polyfill-provider@npm:^0.6.1, @babel/helper-define-polyfill-provider@npm:^0.6.2":
+  version: 0.6.2
+  resolution: "@babel/helper-define-polyfill-provider@npm:0.6.2"
   dependencies:
     "@babel/helper-compilation-targets": ^7.22.6
     "@babel/helper-plugin-utils": ^7.22.5
     debug: ^4.1.1
     lodash.debounce: ^4.0.8
     resolve: ^1.14.2
   peerDependencies:
     "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
-  checksum: d24626b819d3875cb65189d761004e9230f2b3fb60542525c4785616f4b2366741369235a864b744f54beb26d625ae4b0af0c9bb3306b61bf4fccb61e0620020
+  checksum: 2bba965ea9a4887ddf9c11d51d740ab473bd7597b787d042c325f6a45912dfe908c2d6bb1d837bf82f7e9fa51e6ad5150563c58131d2bb85515e63d971414a9c
   languageName: node
   linkType: hard
 
 "@babel/helper-environment-visitor@npm:^7.22.20":
   version: 7.22.20
   resolution: "@babel/helper-environment-visitor@npm:7.22.20"
   checksum: d80ee98ff66f41e233f36ca1921774c37e88a803b2f7dca3db7c057a5fea0473804db9fb6729e5dbfd07f4bed722d60f7852035c2c739382e84c335661590b69
   languageName: node
   linkType: hard
 
-"@babel/helper-function-name@npm:^7.22.5, @babel/helper-function-name@npm:^7.23.0":
+"@babel/helper-function-name@npm:^7.23.0":
   version: 7.23.0
   resolution: "@babel/helper-function-name@npm:7.23.0"
   dependencies:
     "@babel/template": ^7.22.15
     "@babel/types": ^7.23.0
   checksum: e44542257b2d4634a1f979244eb2a4ad8e6d75eb6761b4cfceb56b562f7db150d134bc538c8e6adca3783e3bc31be949071527aa8e3aab7867d1ad2d84a26e10
   languageName: node
@@ -174,60 +167,60 @@
   resolution: "@babel/helper-hoist-variables@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: 394ca191b4ac908a76e7c50ab52102669efe3a1c277033e49467913c7ed6f7c64d7eacbeabf3bed39ea1f41731e22993f763b1edce0f74ff8563fd1f380d92cc
   languageName: node
   linkType: hard
 
-"@babel/helper-member-expression-to-functions@npm:^7.22.15, @babel/helper-member-expression-to-functions@npm:^7.23.0":
-  version: 7.23.0
-  resolution: "@babel/helper-member-expression-to-functions@npm:7.23.0"
+"@babel/helper-member-expression-to-functions@npm:^7.23.0, @babel/helper-member-expression-to-functions@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helper-member-expression-to-functions@npm:7.24.5"
   dependencies:
-    "@babel/types": ^7.23.0
-  checksum: 494659361370c979ada711ca685e2efe9460683c36db1b283b446122596602c901e291e09f2f980ecedfe6e0f2bd5386cb59768285446530df10c14df1024e75
+    "@babel/types": ^7.24.5
+  checksum: d3ad681655128463aa5c2a239345687345f044542563506ee53c9636d147e97f93a470be320950a8ba5f497ade6b27a8136a3a681794867ff94b90060a6e427c
   languageName: node
   linkType: hard
 
-"@babel/helper-module-imports@npm:^7.22.15":
-  version: 7.22.15
-  resolution: "@babel/helper-module-imports@npm:7.22.15"
+"@babel/helper-module-imports@npm:^7.24.1, @babel/helper-module-imports@npm:^7.24.3":
+  version: 7.24.3
+  resolution: "@babel/helper-module-imports@npm:7.24.3"
   dependencies:
-    "@babel/types": ^7.22.15
-  checksum: ecd7e457df0a46f889228f943ef9b4a47d485d82e030676767e6a2fdcbdaa63594d8124d4b55fd160b41c201025aec01fc27580352b1c87a37c9c6f33d116702
+    "@babel/types": ^7.24.0
+  checksum: c23492189ba97a1ec7d37012336a5661174e8b88194836b6bbf90d13c3b72c1db4626263c654454986f924c6da8be7ba7f9447876d709cd00bd6ffde6ec00796
   languageName: node
   linkType: hard
 
-"@babel/helper-module-transforms@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/helper-module-transforms@npm:7.23.3"
+"@babel/helper-module-transforms@npm:^7.23.3, @babel/helper-module-transforms@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helper-module-transforms@npm:7.24.5"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.20
-    "@babel/helper-module-imports": ^7.22.15
-    "@babel/helper-simple-access": ^7.22.5
-    "@babel/helper-split-export-declaration": ^7.22.6
-    "@babel/helper-validator-identifier": ^7.22.20
+    "@babel/helper-module-imports": ^7.24.3
+    "@babel/helper-simple-access": ^7.24.5
+    "@babel/helper-split-export-declaration": ^7.24.5
+    "@babel/helper-validator-identifier": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: 5d0895cfba0e16ae16f3aa92fee108517023ad89a855289c4eb1d46f7aef4519adf8e6f971e1d55ac20c5461610e17213f1144097a8f932e768a9132e2278d71
+  checksum: 208c2e3877536c367ae3f39345bb5c5954ad481fdb2204d4d1906063e53ae564e5b7b846951b1aa96ee716ec24ec3b6db01b41d128884c27315b415f62db9fd2
   languageName: node
   linkType: hard
 
 "@babel/helper-optimise-call-expression@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-optimise-call-expression@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: c70ef6cc6b6ed32eeeec4482127e8be5451d0e5282d5495d5d569d39eb04d7f1d66ec99b327f45d1d5842a9ad8c22d48567e93fc502003a47de78d122e355f7c
   languageName: node
   linkType: hard
 
-"@babel/helper-plugin-utils@npm:^7.0.0, @babel/helper-plugin-utils@npm:^7.10.4, @babel/helper-plugin-utils@npm:^7.12.13, @babel/helper-plugin-utils@npm:^7.14.5, @babel/helper-plugin-utils@npm:^7.18.6, @babel/helper-plugin-utils@npm:^7.22.5, @babel/helper-plugin-utils@npm:^7.8.0, @babel/helper-plugin-utils@npm:^7.8.3":
-  version: 7.22.5
-  resolution: "@babel/helper-plugin-utils@npm:7.22.5"
-  checksum: c0fc7227076b6041acd2f0e818145d2e8c41968cc52fb5ca70eed48e21b8fe6dd88a0a91cbddf4951e33647336eb5ae184747ca706817ca3bef5e9e905151ff5
+"@babel/helper-plugin-utils@npm:^7.0.0, @babel/helper-plugin-utils@npm:^7.10.4, @babel/helper-plugin-utils@npm:^7.12.13, @babel/helper-plugin-utils@npm:^7.14.5, @babel/helper-plugin-utils@npm:^7.18.6, @babel/helper-plugin-utils@npm:^7.22.5, @babel/helper-plugin-utils@npm:^7.24.0, @babel/helper-plugin-utils@npm:^7.24.5, @babel/helper-plugin-utils@npm:^7.8.0, @babel/helper-plugin-utils@npm:^7.8.3":
+  version: 7.24.5
+  resolution: "@babel/helper-plugin-utils@npm:7.24.5"
+  checksum: fa1450c92541b32fe18a6ae85e5c989296a284838fa0a282a2138732cae6f173f36d39dc724890c1740ae72d6d6fbca0b009916b168d4bc874bacc7e5c2fdce0
   languageName: node
   linkType: hard
 
 "@babel/helper-remap-async-to-generator@npm:^7.22.20":
   version: 7.22.20
   resolution: "@babel/helper-remap-async-to-generator@npm:7.22.20"
   dependencies:
@@ -236,150 +229,163 @@
     "@babel/helper-wrap-function": ^7.22.20
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: 2fe6300a6f1b58211dffa0aed1b45d4958506d096543663dba83bd9251fe8d670fa909143a65b45e72acb49e7e20fbdb73eae315d9ddaced467948c3329986e7
   languageName: node
   linkType: hard
 
-"@babel/helper-replace-supers@npm:^7.22.20":
-  version: 7.22.20
-  resolution: "@babel/helper-replace-supers@npm:7.22.20"
+"@babel/helper-replace-supers@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/helper-replace-supers@npm:7.24.1"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.20
-    "@babel/helper-member-expression-to-functions": ^7.22.15
+    "@babel/helper-member-expression-to-functions": ^7.23.0
     "@babel/helper-optimise-call-expression": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: a0008332e24daedea2e9498733e3c39b389d6d4512637e000f96f62b797e702ee24a407ccbcd7a236a551590a38f31282829a8ef35c50a3c0457d88218cae639
+  checksum: c04182c34a3195c6396de2f2945f86cb60daa94ca7392db09bd8b0d4e7a15b02fbe1947c70f6062c87eadaea6d7135207129efa35cf458ea0987bab8c0f02d5a
   languageName: node
   linkType: hard
 
-"@babel/helper-simple-access@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/helper-simple-access@npm:7.22.5"
+"@babel/helper-simple-access@npm:^7.22.5, @babel/helper-simple-access@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helper-simple-access@npm:7.24.5"
   dependencies:
-    "@babel/types": ^7.22.5
-  checksum: fe9686714caf7d70aedb46c3cce090f8b915b206e09225f1e4dbc416786c2fdbbee40b38b23c268b7ccef749dd2db35f255338fb4f2444429874d900dede5ad2
+    "@babel/types": ^7.24.5
+  checksum: 5616044603c98434342f09b056c869394acdeba7cd9ec29e6a9abb0dae1922f779d364aaba74dc2ae4facf85945c6156295adbe0511a8aaecaa8a1559d14757a
   languageName: node
   linkType: hard
 
 "@babel/helper-skip-transparent-expression-wrappers@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-skip-transparent-expression-wrappers@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: 1012ef2295eb12dc073f2b9edf3425661e9b8432a3387e62a8bc27c42963f1f216ab3124228015c748770b2257b4f1fda882ca8fa34c0bf485e929ae5bc45244
   languageName: node
   linkType: hard
 
-"@babel/helper-split-export-declaration@npm:^7.22.6":
-  version: 7.22.6
-  resolution: "@babel/helper-split-export-declaration@npm:7.22.6"
+"@babel/helper-split-export-declaration@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helper-split-export-declaration@npm:7.24.5"
   dependencies:
-    "@babel/types": ^7.22.5
-  checksum: e141cace583b19d9195f9c2b8e17a3ae913b7ee9b8120246d0f9ca349ca6f03cb2c001fd5ec57488c544347c0bb584afec66c936511e447fd20a360e591ac921
+    "@babel/types": ^7.24.5
+  checksum: f23ab6942568084a57789462ce55dc9631aef1d2142ffa2ee28fc411ab55ed3ca65adf109e48655aa349bf8df7ca6dd81fd91c8c229fee1dc77e283189dc83c2
   languageName: node
   linkType: hard
 
-"@babel/helper-string-parser@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/helper-string-parser@npm:7.23.4"
-  checksum: c0641144cf1a7e7dc93f3d5f16d5327465b6cf5d036b48be61ecba41e1eece161b48f46b7f960951b67f8c3533ce506b16dece576baef4d8b3b49f8c65410f90
+"@babel/helper-string-parser@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/helper-string-parser@npm:7.24.1"
+  checksum: 8404e865b06013979a12406aab4c0e8d2e377199deec09dfe9f57b833b0c9ce7b6e8c1c553f2da8d0bcd240c5005bd7a269f4fef0d628aeb7d5fe035c436fb67
   languageName: node
   linkType: hard
 
-"@babel/helper-validator-identifier@npm:^7.22.20":
-  version: 7.22.20
-  resolution: "@babel/helper-validator-identifier@npm:7.22.20"
-  checksum: 136412784d9428266bcdd4d91c32bcf9ff0e8d25534a9d94b044f77fe76bc50f941a90319b05aafd1ec04f7d127cd57a179a3716009ff7f3412ef835ada95bdc
+"@babel/helper-validator-identifier@npm:^7.22.20, @babel/helper-validator-identifier@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helper-validator-identifier@npm:7.24.5"
+  checksum: 75d6f9f475c08f3be87bae4953e9b8d8c72983e16ed2860870b328d048cb20dccb4fcbf85eacbdd817ea1efbb38552a6db9046e2e37bfe13bdec44ac8939024c
   languageName: node
   linkType: hard
 
 "@babel/helper-validator-option@npm:^7.23.5":
   version: 7.23.5
   resolution: "@babel/helper-validator-option@npm:7.23.5"
   checksum: 537cde2330a8aede223552510e8a13e9c1c8798afee3757995a7d4acae564124fe2bf7e7c3d90d62d3657434a74340a274b3b3b1c6f17e9a2be1f48af29cb09e
   languageName: node
   linkType: hard
 
 "@babel/helper-wrap-function@npm:^7.22.20":
-  version: 7.22.20
-  resolution: "@babel/helper-wrap-function@npm:7.22.20"
+  version: 7.24.5
+  resolution: "@babel/helper-wrap-function@npm:7.24.5"
   dependencies:
-    "@babel/helper-function-name": ^7.22.5
-    "@babel/template": ^7.22.15
-    "@babel/types": ^7.22.19
-  checksum: 221ed9b5572612aeb571e4ce6a256f2dee85b3c9536f1dd5e611b0255e5f59a3d0ec392d8d46d4152149156a8109f92f20379b1d6d36abb613176e0e33f05fca
+    "@babel/helper-function-name": ^7.23.0
+    "@babel/template": ^7.24.0
+    "@babel/types": ^7.24.5
+  checksum: c895b95f0fd5e070ced93f315f85e3b63a7236dc9c302bbdce87c699e599d3fd6ad6e44cc820ec7df2d60fadbc922b3b59a0318b708fe69e3d01e5ed15687876
   languageName: node
   linkType: hard
 
-"@babel/helpers@npm:^7.23.9":
-  version: 7.23.9
-  resolution: "@babel/helpers@npm:7.23.9"
+"@babel/helpers@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helpers@npm:7.24.5"
   dependencies:
-    "@babel/template": ^7.23.9
-    "@babel/traverse": ^7.23.9
-    "@babel/types": ^7.23.9
-  checksum: 2678231192c0471dbc2fc403fb19456cc46b1afefcfebf6bc0f48b2e938fdb0fef2e0fe90c8c8ae1f021dae5012b700372e4b5d15867f1d7764616532e4a6324
+    "@babel/template": ^7.24.0
+    "@babel/traverse": ^7.24.5
+    "@babel/types": ^7.24.5
+  checksum: 941937456ca50ef44dbc5cdcb9a74c6ce18ce38971663acd80b622e7ecf1cc4fa034597de3ccccc37939d324139f159709f493fd8e7c385adbc162cb0888cfee
   languageName: node
   linkType: hard
 
-"@babel/highlight@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/highlight@npm:7.23.4"
+"@babel/highlight@npm:^7.24.2":
+  version: 7.24.5
+  resolution: "@babel/highlight@npm:7.24.5"
   dependencies:
-    "@babel/helper-validator-identifier": ^7.22.20
+    "@babel/helper-validator-identifier": ^7.24.5
     chalk: ^2.4.2
     js-tokens: ^4.0.0
-  checksum: 643acecdc235f87d925979a979b539a5d7d1f31ae7db8d89047269082694122d11aa85351304c9c978ceeb6d250591ccadb06c366f358ccee08bb9c122476b89
+    picocolors: ^1.0.0
+  checksum: eece0e63e9210e902f1ee88f15cabfa31d2693bd2e56806eb849478b859d274c24477081c649cee6a241c4aed7da6f3e05c7afa5c3cd70094006ed095292b0d0
   languageName: node
   linkType: hard
 
-"@babel/parser@npm:^7.1.0, @babel/parser@npm:^7.14.7, @babel/parser@npm:^7.20.7, @babel/parser@npm:^7.23.9":
-  version: 7.23.9
-  resolution: "@babel/parser@npm:7.23.9"
+"@babel/parser@npm:^7.1.0, @babel/parser@npm:^7.14.7, @babel/parser@npm:^7.20.7, @babel/parser@npm:^7.23.9, @babel/parser@npm:^7.24.0, @babel/parser@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/parser@npm:7.24.5"
   bin:
     parser: ./bin/babel-parser.js
-  checksum: e7cd4960ac8671774e13803349da88d512f9292d7baa952173260d3e8f15620a28a3701f14f709d769209022f9e7b79965256b8be204fc550cfe783cdcabe7c7
+  checksum: a251ea41bf8b5f61048beb320d43017aff68af5a3506bd2ef392180f5fa32c1061513171d582bb3d46ea48e3659dece8b3ba52511a2566066e58abee300ce2a0
   languageName: node
   linkType: hard
 
-"@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:7.23.3"
+"@babel/plugin-bugfix-firefox-class-in-computed-class-key@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-bugfix-firefox-class-in-computed-class-key@npm:7.24.5"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-environment-visitor": ^7.22.20
+    "@babel/helper-plugin-utils": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: ddbaf2c396b7780f15e80ee01d6dd790db076985f3dfeb6527d1a8d4cacf370e49250396a3aa005b2c40233cac214a106232f83703d5e8491848bde273938232
+  checksum: d9921b3561762b8c7227cfbf1591436d2a12b99472993a7ce382123e88d98cb359952fbc64d66b1a492187d283d02f51e707f524b708c91b9ab82fb2659eae13
   languageName: node
   linkType: hard
 
-"@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:7.23.3"
+"@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
+  peerDependencies:
+    "@babel/core": ^7.0.0
+  checksum: ec5fddc8db6de0e0082a883f21141d6f4f9f9f0bc190d662a732b5e9a506aae5d7d2337049a1bf055d7cb7add6f128036db6d4f47de5e9ac1be29e043c8b7ca8
+  languageName: node
+  linkType: hard
+
+"@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:7.24.1"
+  dependencies:
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
-    "@babel/plugin-transform-optional-chaining": ^7.23.3
+    "@babel/plugin-transform-optional-chaining": ^7.24.1
   peerDependencies:
     "@babel/core": ^7.13.0
-  checksum: 434b9d710ae856fa1a456678cc304fbc93915af86d581ee316e077af746a709a741ea39d7e1d4f5b98861b629cc7e87f002d3138f5e836775632466d4c74aef2
+  checksum: e18235463e716ac2443938aaec3c18b40c417a1746fba0fa4c26cf4d71326b76ef26c002081ab1b445abfae98e063d561519aa55672dddc1ef80b3940211ffbb
   languageName: node
   linkType: hard
 
-"@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly@npm:^7.23.7":
-  version: 7.23.7
-  resolution: "@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly@npm:7.23.7"
+"@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly@npm:7.24.1"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.20
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: f88e400b548202a6f8c5dfd25bc4949a13ea1ccb64a170d7dea4deaa655a0fcb001d3fd61c35e1ad9c09a3d5f0d43f783400425471fe6d660ccaf33dabea9aba
+  checksum: b5e5889ce5ef51e813e3063cd548f55eb3c88e925c3c08913f334e15d62496861e538ae52a3974e0c56a3044ed8fd5033faea67a64814324af56edc9865b7359
   languageName: node
   linkType: hard
 
 "@babel/plugin-proposal-private-property-in-object@npm:7.21.0-placeholder-for-preset-env.2":
   version: 7.21.0-placeholder-for-preset-env.2
   resolution: "@babel/plugin-proposal-private-property-in-object@npm:7.21.0-placeholder-for-preset-env.2"
   peerDependencies:
@@ -450,33 +456,33 @@
     "@babel/helper-plugin-utils": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: 85740478be5b0de185228e7814451d74ab8ce0a26fcca7613955262a26e99e8e15e9da58f60c754b84515d4c679b590dbd3f2148f0f58025f4ae706f1c5a5d4a
   languageName: node
   linkType: hard
 
-"@babel/plugin-syntax-import-assertions@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-syntax-import-assertions@npm:7.23.3"
+"@babel/plugin-syntax-import-assertions@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-syntax-import-assertions@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 883e6b35b2da205138caab832d54505271a3fee3fc1e8dc0894502434fc2b5d517cbe93bbfbfef8068a0fb6ec48ebc9eef3f605200a489065ba43d8cddc1c9a7
+  checksum: 2a463928a63b62052e9fb8f8b0018aa11a926e94f32c168260ae012afe864875c6176c6eb361e13f300542c31316dad791b08a5b8ed92436a3095c7a0e4fce65
   languageName: node
   linkType: hard
 
-"@babel/plugin-syntax-import-attributes@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-syntax-import-attributes@npm:7.23.3"
+"@babel/plugin-syntax-import-attributes@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-syntax-import-attributes@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 9aed7661ffb920ca75df9f494757466ca92744e43072e0848d87fa4aa61a3f2ee5a22198ac1959856c036434b5614a8f46f1fb70298835dbe28220cdd1d4c11e
+  checksum: 87c8aa4a5ef931313f956871b27f2c051556f627b97ed21e9a5890ca4906b222d89062a956cde459816f5e0dec185ff128d7243d3fdc389504522acb88f0464e
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-import-meta@npm:^7.10.4, @babel/plugin-syntax-import-meta@npm:^7.8.3":
   version: 7.10.4
   resolution: "@babel/plugin-syntax-import-meta@npm:7.10.4"
   dependencies:
@@ -495,21 +501,21 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: bf5aea1f3188c9a507e16efe030efb996853ca3cadd6512c51db7233cc58f3ac89ff8c6bdfb01d30843b161cfe7d321e1bf28da82f7ab8d7e6bc5464666f354a
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-jsx@npm:^7.7.2":
-  version: 7.23.3
-  resolution: "@babel/plugin-syntax-jsx@npm:7.23.3"
+  version: 7.24.1
+  resolution: "@babel/plugin-syntax-jsx@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 89037694314a74e7f0e7a9c8d3793af5bf6b23d80950c29b360db1c66859d67f60711ea437e70ad6b5b4b29affe17eababda841b6c01107c2b638e0493bafb4e
+  checksum: 712f7e7918cb679f106769f57cfab0bc99b311032665c428b98f4c3e2e6d567601d45386a4f246df6a80d741e1f94192b3f008800d66c4f1daae3ad825c243f0
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-logical-assignment-operators@npm:^7.10.4, @babel/plugin-syntax-logical-assignment-operators@npm:^7.8.3":
   version: 7.10.4
   resolution: "@babel/plugin-syntax-logical-assignment-operators@npm:7.10.4"
   dependencies:
@@ -594,21 +600,21 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: bbd1a56b095be7820029b209677b194db9b1d26691fe999856462e66b25b281f031f3dfd91b1619e9dcf95bebe336211833b854d0fb8780d618e35667c2d0d7e
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-typescript@npm:^7.7.2":
-  version: 7.23.3
-  resolution: "@babel/plugin-syntax-typescript@npm:7.23.3"
+  version: 7.24.1
+  resolution: "@babel/plugin-syntax-typescript@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: abfad3a19290d258b028e285a1f34c9b8a0cbe46ef79eafed4ed7ffce11b5d0720b5e536c82f91cbd8442cde35a3dd8e861fa70366d87ff06fdc0d4756e30876
+  checksum: bf4bd70788d5456b5f75572e47a2e31435c7c4e43609bd4dffd2cc0c7a6cf90aabcf6cd389e351854de9a64412a07d30effef5373251fe8f6a4c9db0c0163bda
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-unicode-sets-regex@npm:^7.18.6":
   version: 7.18.6
   resolution: "@babel/plugin-syntax-unicode-sets-regex@npm:7.18.6"
   dependencies:
@@ -616,318 +622,318 @@
     "@babel/helper-plugin-utils": ^7.18.6
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: a651d700fe63ff0ddfd7186f4ebc24447ca734f114433139e3c027bc94a900d013cf1ef2e2db8430425ba542e39ae160c3b05f06b59fd4656273a3df97679e9c
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-arrow-functions@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-arrow-functions@npm:7.23.3"
+"@babel/plugin-transform-arrow-functions@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-arrow-functions@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 1e99118176e5366c2636064d09477016ab5272b2a92e78b8edb571d20bc3eaa881789a905b20042942c3c2d04efc530726cf703f937226db5ebc495f5d067e66
+  checksum: 58f9aa9b0de8382f8cfa3f1f1d40b69d98cd2f52340e2391733d0af745fdddda650ba392e509bc056157c880a2f52834a38ab2c5aa5569af8c61bb6ecbf45f34
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-async-generator-functions@npm:^7.23.9":
-  version: 7.23.9
-  resolution: "@babel/plugin-transform-async-generator-functions@npm:7.23.9"
+"@babel/plugin-transform-async-generator-functions@npm:^7.24.3":
+  version: 7.24.3
+  resolution: "@babel/plugin-transform-async-generator-functions@npm:7.24.3"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.20
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-remap-async-to-generator": ^7.22.20
     "@babel/plugin-syntax-async-generators": ^7.8.4
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: d402494087a6b803803eb5ab46b837aab100a04c4c5148e38bfa943ea1bbfc1ecfb340f1ced68972564312d3580f550c125f452372e77607a558fbbaf98c31c0
+  checksum: 309af02610be65d937664435adb432a32d9b6eb42bb3d3232c377d27fbc57014774d931665a5bfdaff3d1841b72659e0ad7adcef84b709f251cb0b8444f19214
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-async-to-generator@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-async-to-generator@npm:7.23.3"
+"@babel/plugin-transform-async-to-generator@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-async-to-generator@npm:7.24.1"
   dependencies:
-    "@babel/helper-module-imports": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-module-imports": ^7.24.1
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-remap-async-to-generator": ^7.22.20
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 2e9d9795d4b3b3d8090332104e37061c677f29a1ce65bcbda4099a32d243e5d9520270a44bbabf0fb1fb40d463bd937685b1a1042e646979086c546d55319c3c
+  checksum: 429004a6596aa5c9e707b604156f49a146f8d029e31a3152b1649c0b56425264fda5fd38e5db1ddaeb33c3fe45c97dc8078d7abfafe3542a979b49f229801135
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-block-scoped-functions@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-block-scoped-functions@npm:7.23.3"
+"@babel/plugin-transform-block-scoped-functions@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-block-scoped-functions@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: e63b16d94ee5f4d917e669da3db5ea53d1e7e79141a2ec873c1e644678cdafe98daa556d0d359963c827863d6b3665d23d4938a94a4c5053a1619c4ebd01d020
+  checksum: d8e18bd57b156da1cd4d3c1780ab9ea03afed56c6824ca8e6e74f67959d7989a0e953ec370fe9b417759314f2eef30c8c437395ce63ada2e26c2f469e4704f82
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-block-scoping@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-block-scoping@npm:7.23.4"
+"@babel/plugin-transform-block-scoping@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-block-scoping@npm:7.24.5"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: fc4b2100dd9f2c47d694b4b35ae8153214ccb4e24ef545c259a9db17211b18b6a430f22799b56db8f6844deaeaa201af45a03331d0c80cc28b0c4e3c814570e4
+  checksum: 898c91efc0f8ac8e2a8d3ece36edf0001963bcf5bbeefe9bf798ac36318a33f366e88a24a90bf7c39a7aeb1593846b720ed9a9ba56709d27279f7ba61c5e43c4
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-class-properties@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-class-properties@npm:7.23.3"
+"@babel/plugin-transform-class-properties@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-class-properties@npm:7.24.1"
   dependencies:
-    "@babel/helper-create-class-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-create-class-features-plugin": ^7.24.1
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 9c6f8366f667897541d360246de176dd29efc7a13d80a5b48361882f7173d9173be4646c3b7d9b003ccc0e01e25df122330308f33db921fa553aa17ad544b3fc
+  checksum: 95779e9eef0c0638b9631c297d48aee53ffdbb2b1b5221bf40d7eccd566a8e34f859ff3571f8f20b9159b67f1bff7d7dc81da191c15d69fbae5a645197eae7e0
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-class-static-block@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-class-static-block@npm:7.23.4"
+"@babel/plugin-transform-class-static-block@npm:^7.24.4":
+  version: 7.24.4
+  resolution: "@babel/plugin-transform-class-static-block@npm:7.24.4"
   dependencies:
-    "@babel/helper-create-class-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-create-class-features-plugin": ^7.24.4
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-class-static-block": ^7.14.5
   peerDependencies:
     "@babel/core": ^7.12.0
-  checksum: c8bfaba19a674fc2eb54edad71e958647360474e3163e8226f1acd63e4e2dbec32a171a0af596c1dc5359aee402cc120fea7abd1fb0e0354b6527f0fc9e8aa1e
+  checksum: 3b1db3308b57ba21d47772a9f183804234c23fd64c9ca40915d2d65c5dc7a48b49a6de16b8b90b7a354eacbb51232a862f0fca3dbd23e27d34641f511decddab
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-classes@npm:^7.23.8":
-  version: 7.23.8
-  resolution: "@babel/plugin-transform-classes@npm:7.23.8"
+"@babel/plugin-transform-classes@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-classes@npm:7.24.5"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
     "@babel/helper-compilation-targets": ^7.23.6
     "@babel/helper-environment-visitor": ^7.22.20
     "@babel/helper-function-name": ^7.23.0
-    "@babel/helper-plugin-utils": ^7.22.5
-    "@babel/helper-replace-supers": ^7.22.20
-    "@babel/helper-split-export-declaration": ^7.22.6
+    "@babel/helper-plugin-utils": ^7.24.5
+    "@babel/helper-replace-supers": ^7.24.1
+    "@babel/helper-split-export-declaration": ^7.24.5
     globals: ^11.1.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 7dee6cebe52131d2d16944f36e1fdb9d4b24f44d0e7e450f93a44435d001f17cc0789a4cb6b15ec67c8e484581b8a730b5c3ec374470f29ff0133086955b8c58
+  checksum: 797bf2bda770148d3ee43e305e1aea26fa16ca78eb81eaaeb95b441428f52e0d12dd98e93f00bda3b65bbfde3001006995725ce911587efdef0465c41bd0a3f3
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-computed-properties@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-computed-properties@npm:7.23.3"
+"@babel/plugin-transform-computed-properties@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-computed-properties@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
-    "@babel/template": ^7.22.15
+    "@babel/helper-plugin-utils": ^7.24.0
+    "@babel/template": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 80452661dc25a0956f89fe98cb562e8637a9556fb6c00d312c57653ce7df8798f58d138603c7e1aad96614ee9ccd10c47e50ab9ded6b6eded5adeb230d2a982e
+  checksum: f2832bcf100a70f348facbb395873318ef5b9ee4b0fb4104a420d9daaeb6003cc2ecc12fd8083dd2e4a7c2da873272ad73ff94de4497125a0cf473294ef9664e
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-destructuring@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-destructuring@npm:7.23.3"
+"@babel/plugin-transform-destructuring@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-destructuring@npm:7.24.5"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 9e015099877272501162419bfe781689aec5c462cd2aec752ee22288f209eec65969ff11b8fdadca2eaddea71d705d3bba5b9c60752fcc1be67874fcec687105
+  checksum: c5def67de09315cd38895c021ee7d02fd53fed596924512c33196ceed143b88f1ea76e4ac777a55bbb9db49be8b63aafb22b12e7d5c7f3051f14caa07e8d4023
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-dotall-regex@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-dotall-regex@npm:7.23.3"
+"@babel/plugin-transform-dotall-regex@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-dotall-regex@npm:7.24.1"
   dependencies:
     "@babel/helper-create-regexp-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: a2dbbf7f1ea16a97948c37df925cb364337668c41a3948b8d91453f140507bd8a3429030c7ce66d09c299987b27746c19a2dd18b6f17dcb474854b14fd9159a3
+  checksum: 7f623d25b6f213b94ebc1754e9e31c1077c8e288626d8b7bfa76a97b067ce80ddcd0ede402a546706c65002c0ccf45cd5ec621511c2668eed31ebcabe8391d35
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-duplicate-keys@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-duplicate-keys@npm:7.23.3"
+"@babel/plugin-transform-duplicate-keys@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-duplicate-keys@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: c2a21c34dc0839590cd945192cbc46fde541a27e140c48fe1808315934664cdbf18db64889e23c4eeb6bad9d3e049482efdca91d29de5734ffc887c4fbabaa16
+  checksum: a3b07c07cee441e185858a9bb9739bb72643173c18bf5f9f949dd2d4784ca124e56b01d0a270790fb1ff0cf75d436075db0a2b643fb4285ff9a21df9e8dc6284
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-dynamic-import@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-dynamic-import@npm:7.23.4"
+"@babel/plugin-transform-dynamic-import@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-dynamic-import@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-dynamic-import": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 57a722604c430d9f3dacff22001a5f31250e34785d4969527a2ae9160fa86858d0892c5b9ff7a06a04076f8c76c9e6862e0541aadca9c057849961343aab0845
+  checksum: 59fc561ee40b1a69f969c12c6c5fac206226d6642213985a569dd0f99f8e41c0f4eaedebd36936c255444a8335079842274c42a975a433beadb436d4c5abb79b
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-exponentiation-operator@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-exponentiation-operator@npm:7.23.3"
+"@babel/plugin-transform-exponentiation-operator@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-exponentiation-operator@npm:7.24.1"
   dependencies:
     "@babel/helper-builder-binary-assignment-operator-visitor": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 00d05ab14ad0f299160fcf9d8f55a1cc1b740e012ab0b5ce30207d2365f091665115557af7d989cd6260d075a252d9e4283de5f2b247dfbbe0e42ae586e6bf66
+  checksum: f90841fe1a1e9f680b4209121d3e2992f923e85efcd322b26e5901c180ef44ff727fb89790803a23fac49af34c1ce2e480018027c22b4573b615512ac5b6fc50
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-export-namespace-from@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-export-namespace-from@npm:7.23.4"
+"@babel/plugin-transform-export-namespace-from@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-export-namespace-from@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-export-namespace-from": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 9f770a81bfd03b48d6ba155d452946fd56d6ffe5b7d871e9ec2a0b15e0f424273b632f3ed61838b90015b25bbda988896b7a46c7d964fbf8f6feb5820b309f93
+  checksum: bc710ac231919df9555331885748385c11c5e695d7271824fe56fba51dd637d48d3e5cd52e1c69f2b1a384fbbb41552572bc1ca3a2285ee29571f002e9bb2421
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-for-of@npm:^7.23.6":
-  version: 7.23.6
-  resolution: "@babel/plugin-transform-for-of@npm:7.23.6"
+"@babel/plugin-transform-for-of@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-for-of@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 228c060aa61f6aa89dc447170075f8214863b94f830624e74ade99c1a09316897c12d76e848460b0b506593e58dbc42739af6dc4cb0fe9b84dffe4a596050a36
+  checksum: 990adde96ea1766ed6008c006c7040127bef59066533bb2977b246ea4a596fe450a528d1881a0db5f894deaf1b81654dfb494b19ad405b369be942738aa9c364
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-function-name@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-function-name@npm:7.23.3"
+"@babel/plugin-transform-function-name@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-function-name@npm:7.24.1"
   dependencies:
-    "@babel/helper-compilation-targets": ^7.22.15
+    "@babel/helper-compilation-targets": ^7.23.6
     "@babel/helper-function-name": ^7.23.0
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 355c6dbe07c919575ad42b2f7e020f320866d72f8b79181a16f8e0cd424a2c761d979f03f47d583d9471b55dcd68a8a9d829b58e1eebcd572145b934b48975a6
+  checksum: 31eb3c75297dda7265f78eba627c446f2324e30ec0124a645ccc3e9f341254aaa40d6787bd62b2280d77c0a5c9fbfce1da2c200ef7c7f8e0a1b16a8eb3644c6f
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-json-strings@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-json-strings@npm:7.23.4"
+"@babel/plugin-transform-json-strings@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-json-strings@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-json-strings": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: f9019820233cf8955d8ba346df709a0683c120fe86a24ed1c9f003f2db51197b979efc88f010d558a12e1491210fc195a43cd1c7fee5e23b92da38f793a875de
+  checksum: f42302d42fc81ac00d14e9e5d80405eb80477d7f9039d7208e712d6bcd486a4e3b32fdfa07b5f027d6c773723d8168193ee880f93b0e430c828e45f104fb82a4
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-literals@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-literals@npm:7.23.3"
+"@babel/plugin-transform-literals@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-literals@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 519a544cd58586b9001c4c9b18da25a62f17d23c48600ff7a685d75ca9eb18d2c5e8f5476f067f0a8f1fea2a31107eff950b9864833061e6076dcc4bdc3e71ed
+  checksum: 2df94e9478571852483aca7588419e574d76bde97583e78551c286f498e01321e7dbb1d0ef67bee16e8f950688f79688809cfde370c5c4b84c14d841a3ef217a
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-logical-assignment-operators@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-logical-assignment-operators@npm:7.23.4"
+"@babel/plugin-transform-logical-assignment-operators@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-logical-assignment-operators@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-logical-assignment-operators": ^7.10.4
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 2ae1dc9b4ff3bf61a990ff3accdecb2afe3a0ca649b3e74c010078d1cdf29ea490f50ac0a905306a2bcf9ac177889a39ac79bdcc3a0fdf220b3b75fac18d39b5
+  checksum: 895f2290adf457cbf327428bdb4fb90882a38a22f729bcf0629e8ad66b9b616d2721fbef488ac00411b647489d1dda1d20171bb3772d0796bb7ef5ecf057808a
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-member-expression-literals@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-member-expression-literals@npm:7.23.3"
+"@babel/plugin-transform-member-expression-literals@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-member-expression-literals@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 95cec13c36d447c5aa6b8e4c778b897eeba66dcb675edef01e0d2afcec9e8cb9726baf4f81b4bbae7a782595aed72e6a0d44ffb773272c3ca180fada99bf92db
+  checksum: 4ea641cc14a615f9084e45ad2319f95e2fee01c77ec9789685e7e11a6c286238a426a98f9c1ed91568a047d8ac834393e06e8c82d1ff01764b7aa61bee8e9023
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-modules-amd@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-modules-amd@npm:7.23.3"
+"@babel/plugin-transform-modules-amd@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-modules-amd@npm:7.24.1"
   dependencies:
     "@babel/helper-module-transforms": ^7.23.3
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: d163737b6a3d67ea579c9aa3b83d4df4b5c34d9dcdf25f415f027c0aa8cded7bac2750d2de5464081f67a042ad9e1c03930c2fab42acd79f9e57c00cf969ddff
+  checksum: 3d777c262f257e93f0405b13e178f9c4a0f31855b409f0191a76bb562a28c541326a027bfe6467fcb74752f3488c0333b5ff2de64feec1b3c4c6ace1747afa03
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-modules-commonjs@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-modules-commonjs@npm:7.23.3"
+"@babel/plugin-transform-modules-commonjs@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-modules-commonjs@npm:7.24.1"
   dependencies:
     "@babel/helper-module-transforms": ^7.23.3
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-simple-access": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 720a231ceade4ae4d2632478db4e7fecf21987d444942b72d523487ac8d715ca97de6c8f415c71e939595e1a4776403e7dc24ed68fe9125ad4acf57753c9bff7
+  checksum: 11402b34c49f76aa921b43c2d76f3f129a32544a1dc4f0d1e48b310f9036ab75269a6d8684ed0198b7a0b07bd7898b12f0cacceb26fbb167999fd2a819aa0802
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-modules-systemjs@npm:^7.23.9":
-  version: 7.23.9
-  resolution: "@babel/plugin-transform-modules-systemjs@npm:7.23.9"
+"@babel/plugin-transform-modules-systemjs@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-modules-systemjs@npm:7.24.1"
   dependencies:
     "@babel/helper-hoist-variables": ^7.22.5
     "@babel/helper-module-transforms": ^7.23.3
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-validator-identifier": ^7.22.20
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: cec6abeae6be66fd1a5940c482fe9ff94b689c71fcf4147e179119e4accd09d17d476e36528bc9cb4ab0ec6728fedf48b1c49d0551ea707fb192575d8eac9167
+  checksum: 903766f6808f04278e887e4adec9b1efa741726279652dad255eaad0f5701df8f8ff0af25eb8541a00eb3c9eae2dccf337b085cfa011426ca33ed1f95d70bf75
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-modules-umd@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-modules-umd@npm:7.23.3"
+"@babel/plugin-transform-modules-umd@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-modules-umd@npm:7.24.1"
   dependencies:
     "@babel/helper-module-transforms": ^7.23.3
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 586a7a2241e8b4e753a37af9466a9ffa8a67b4ba9aa756ad7500712c05d8fa9a8c1ed4f7bd25fae2a8265e6cf8fe781ec85a8ee885dd34cf50d8955ee65f12dc
+  checksum: 4922f5056d34de6fd59a1ab1c85bc3472afa706c776aceeb886289c9ac9117e6eb8e22d06c537eb5bc0ede6c30f6bd85210bdcc150dc0ae2d2373f8252df9364
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-named-capturing-groups-regex@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/plugin-transform-named-capturing-groups-regex@npm:7.22.5"
   dependencies:
@@ -935,362 +941,362 @@
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: 3ee564ddee620c035b928fdc942c5d17e9c4b98329b76f9cefac65c111135d925eb94ed324064cd7556d4f5123beec79abea1d4b97d1c8a2a5c748887a2eb623
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-new-target@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-new-target@npm:7.23.3"
+"@babel/plugin-transform-new-target@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-new-target@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: e5053389316fce73ad5201b7777437164f333e24787fbcda4ae489cd2580dbbbdfb5694a7237bad91fabb46b591d771975d69beb1c740b82cb4761625379f00b
+  checksum: f56159ba56e8824840b8073f65073434e4bc4ef20e366bc03aa6cae9a4389365574fa72390e48aed76049edbc6eba1181eb810e58fae22c25946c62f9da13db4
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-nullish-coalescing-operator@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-nullish-coalescing-operator@npm:7.23.4"
+"@babel/plugin-transform-nullish-coalescing-operator@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-nullish-coalescing-operator@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-nullish-coalescing-operator": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: a27d73ea134d3d9560a6b2e26ab60012fba15f1db95865aa0153c18f5ec82cfef6a7b3d8df74e3c2fca81534fa5efeb6cacaf7b08bdb7d123e3dafdd079886a3
+  checksum: 74025e191ceb7cefc619c15d33753aab81300a03d81b96ae249d9b599bc65878f962d608f452462d3aad5d6e334b7ab2b09a6bdcfe8d101fe77ac7aacca4261e
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-numeric-separator@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-numeric-separator@npm:7.23.4"
+"@babel/plugin-transform-numeric-separator@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-numeric-separator@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-numeric-separator": ^7.10.4
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 6ba0e5db3c620a3ec81f9e94507c821f483c15f196868df13fa454cbac719a5449baf73840f5b6eb7d77311b24a2cf8e45db53700d41727f693d46f7caf3eec3
+  checksum: 3247bd7d409574fc06c59e0eb573ae7470d6d61ecf780df40b550102bb4406747d8f39dcbec57eb59406df6c565a86edd3b429e396ad02e4ce201ad92050832e
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-object-rest-spread@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-object-rest-spread@npm:7.23.4"
+"@babel/plugin-transform-object-rest-spread@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-object-rest-spread@npm:7.24.5"
   dependencies:
-    "@babel/compat-data": ^7.23.3
-    "@babel/helper-compilation-targets": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-compilation-targets": ^7.23.6
+    "@babel/helper-plugin-utils": ^7.24.5
     "@babel/plugin-syntax-object-rest-spread": ^7.8.3
-    "@babel/plugin-transform-parameters": ^7.23.3
+    "@babel/plugin-transform-parameters": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 73fec495e327ca3959c1c03d07a621be09df00036c69fff0455af9a008291677ee9d368eec48adacdc6feac703269a649747568b4af4c4e9f134aa71cc5b378d
+  checksum: 427705fe1358ca4862e6cfbfc174dc0fbfdd640b786cfe759dd4881cfb2fd51723e8432ecd89f07a60444e555a9c19e0e7bf4c657b91844994b39a53a602eb16
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-object-super@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-object-super@npm:7.23.3"
+"@babel/plugin-transform-object-super@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-object-super@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
-    "@babel/helper-replace-supers": ^7.22.20
+    "@babel/helper-plugin-utils": ^7.24.0
+    "@babel/helper-replace-supers": ^7.24.1
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: e495497186f621fa79026e183b4f1fbb172fd9df812cbd2d7f02c05b08adbe58012b1a6eb6dd58d11a30343f6ec80d0f4074f9b501d70aa1c94df76d59164c53
+  checksum: d34d437456a54e2a5dcb26e9cf09ed4c55528f2a327c5edca92c93e9483c37176e228d00d6e0cf767f3d6fdbef45ae3a5d034a7c59337a009e20ae541c8220fa
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-optional-catch-binding@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-optional-catch-binding@npm:7.23.4"
+"@babel/plugin-transform-optional-catch-binding@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-optional-catch-binding@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-optional-catch-binding": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: d50b5ee142cdb088d8b5de1ccf7cea85b18b85d85b52f86618f6e45226372f01ad4cdb29abd4fd35ea99a71fefb37009e0107db7a787dcc21d4d402f97470faf
+  checksum: ff7c02449d32a6de41e003abb38537b4a1ad90b1eaa4c0b578cb1b55548201a677588a8c47f3e161c72738400ae811a6673ea7b8a734344755016ca0ac445dac
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-optional-chaining@npm:^7.23.3, @babel/plugin-transform-optional-chaining@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-optional-chaining@npm:7.23.4"
+"@babel/plugin-transform-optional-chaining@npm:^7.24.1, @babel/plugin-transform-optional-chaining@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-optional-chaining@npm:7.24.5"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.5
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
     "@babel/plugin-syntax-optional-chaining": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: e7a4c08038288057b7a08d68c4d55396ada9278095509ca51ed8dfb72a7f13f26bdd7c5185de21079fe0a9d60d22c227cb32e300d266c1bda40f70eee9f4bc1e
+  checksum: 233934463ef1f9a02a9fda96c722e9c162477fd94816a58413f0d4165cc536c7af0482b46fe066e754748a20bbabec255b4bbde194a7fd20b32280e526e1bfec
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-parameters@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-parameters@npm:7.23.3"
+"@babel/plugin-transform-parameters@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-parameters@npm:7.24.5"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: a735b3e85316d17ec102e3d3d1b6993b429bdb3b494651c9d754e3b7d270462ee1f1a126ccd5e3d871af5e683727e9ef98c9d34d4a42204fffaabff91052ed16
+  checksum: b052e1cf43b1ea571fc0867baa01041ce32f46576b711c6331f03263ae479a582f81a6039287535cd90ee46d2977e2f3c66f5bdbf454a9f8cdc7c5c6c67b50be
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-private-methods@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-private-methods@npm:7.23.3"
+"@babel/plugin-transform-private-methods@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-private-methods@npm:7.24.1"
   dependencies:
-    "@babel/helper-create-class-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-create-class-features-plugin": ^7.24.1
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: cedc1285c49b5a6d9a3d0e5e413b756ac40b3ac2f8f68bdfc3ae268bc8d27b00abd8bb0861c72756ff5dd8bf1eb77211b7feb5baf4fdae2ebbaabe49b9adc1d0
+  checksum: 7208c30bb3f3fbc73fb3a88bdcb78cd5cddaf6d523eb9d67c0c04e78f6fc6319ece89f4a5abc41777ceab16df55b3a13a4120e0efc9275ca6d2d89beaba80aa0
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-private-property-in-object@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-private-property-in-object@npm:7.23.4"
+"@babel/plugin-transform-private-property-in-object@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-private-property-in-object@npm:7.24.5"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
-    "@babel/helper-create-class-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-create-class-features-plugin": ^7.24.5
+    "@babel/helper-plugin-utils": ^7.24.5
     "@babel/plugin-syntax-private-property-in-object": ^7.14.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: fb7adfe94ea97542f250a70de32bddbc3e0b802381c92be947fec83ebffda57e68533c4d0697152719a3496fdd3ebf3798d451c024cd4ac848fc15ac26b70aa7
+  checksum: 59f9007671f50ef8f9eff33bb2dc3de22a2849612d4b64fc9e4ba502466ddbaf3f94774011695dde5128c4ca2009e241babe928ac63f71a29f27c1cc7ce01e5f
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-property-literals@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-property-literals@npm:7.23.3"
+"@babel/plugin-transform-property-literals@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-property-literals@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 16b048c8e87f25095f6d53634ab7912992f78e6997a6ff549edc3cf519db4fca01c7b4e0798530d7f6a05228ceee479251245cdd850a5531c6e6f404104d6cc9
+  checksum: a73646d7ecd95b3931a3ead82c7d5efeb46e68ba362de63eb437d33531f294ec18bd31b6d24238cd3b6a3b919a6310c4a0ba4a2629927721d4d10b0518eb7715
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-regenerator@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-regenerator@npm:7.23.3"
+"@babel/plugin-transform-regenerator@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-regenerator@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     regenerator-transform: ^0.15.2
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 7fdacc7b40008883871b519c9e5cdea493f75495118ccc56ac104b874983569a24edd024f0f5894ba1875c54ee2b442f295d6241c3280e61c725d0dd3317c8e6
+  checksum: a04319388a0a7931c3f8e15715d01444c32519692178b70deccc86d53304e74c0f589a4268f6c68578d86f75e934dd1fe6e6ed9071f54ee8379f356f88ef6e42
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-reserved-words@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-reserved-words@npm:7.23.3"
+"@babel/plugin-transform-reserved-words@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-reserved-words@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 298c4440ddc136784ff920127cea137168e068404e635dc946ddb5d7b2a27b66f1dd4c4acb01f7184478ff7d5c3e7177a127279479926519042948fb7fa0fa48
+  checksum: 132c6040c65aabae2d98a39289efb5c51a8632546dc50d2ad032c8660aec307fbed74ef499856ea4f881fc8505905f49b48e0270585da2ea3d50b75e962afd89
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-shorthand-properties@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-shorthand-properties@npm:7.23.3"
+"@babel/plugin-transform-shorthand-properties@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-shorthand-properties@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 5d677a03676f9fff969b0246c423d64d77502e90a832665dc872a5a5e05e5708161ce1effd56bb3c0f2c20a1112fca874be57c8a759d8b08152755519281f326
+  checksum: 006a2032d1c57dca76579ce6598c679c2f20525afef0a36e9d42affe3c8cf33c1427581ad696b519cc75dfee46c5e8ecdf0c6a29ffb14250caa3e16dd68cb424
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-spread@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-spread@npm:7.23.3"
+"@babel/plugin-transform-spread@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-spread@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 8fd5cac201e77a0b4825745f4e07a25f923842f282f006b3a79223c00f61075c8868d12eafec86b2642cd0b32077cdd32314e27bcb75ee5e6a68c0144140dcf2
+  checksum: 622ef507e2b5120a9010b25d3df5186c06102ecad8751724a38ec924df8d3527688198fa490c47064eabba14ef2f961b3069855bd22a8c0a1e51a23eed348d02
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-sticky-regex@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-sticky-regex@npm:7.23.3"
+"@babel/plugin-transform-sticky-regex@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-sticky-regex@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 53e55eb2575b7abfdb4af7e503a2bf7ef5faf8bf6b92d2cd2de0700bdd19e934e5517b23e6dfed94ba50ae516b62f3f916773ef7d9bc81f01503f585051e2949
+  checksum: e326e96a9eeb6bb01dbc4d3362f989411490671b97f62edf378b8fb102c463a018b777f28da65344d41b22aa6efcdfa01ed43d2b11fdcf202046d3174be137c5
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-template-literals@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-template-literals@npm:7.23.3"
+"@babel/plugin-transform-template-literals@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-template-literals@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: b16c5cb0b8796be0118e9c144d15bdc0d20a7f3f59009c6303a6e9a8b74c146eceb3f05186f5b97afcba7cfa87e34c1585a22186e3d5b22f2fd3d27d959d92b2
+  checksum: 4c9009c72321caf20e3b6328bbe9d7057006c5ae57b794cf247a37ca34d87dfec5e27284169a16df5a6235a083bf0f3ab9e1bfcb005d1c8b75b04aed75652621
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-typeof-symbol@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-typeof-symbol@npm:7.23.3"
+"@babel/plugin-transform-typeof-symbol@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-typeof-symbol@npm:7.24.5"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 0af7184379d43afac7614fc89b1bdecce4e174d52f4efaeee8ec1a4f2c764356c6dba3525c0685231f1cbf435b6dd4ee9e738d7417f3b10ce8bbe869c32f4384
+  checksum: 35504219e4e8b361dbd285400c846f154754e591e931cd30dbe1426a619e41ed0c410b26dd173824ed3a2ff0371d64213ae2304b6f169b32e78b004114f5acd5
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-unicode-escapes@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-unicode-escapes@npm:7.23.3"
+"@babel/plugin-transform-unicode-escapes@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-unicode-escapes@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 561c429183a54b9e4751519a3dfba6014431e9cdc1484fad03bdaf96582dfc72c76a4f8661df2aeeae7c34efd0fa4d02d3b83a2f63763ecf71ecc925f9cc1f60
+  checksum: d4d7cfea91af7be2768fb6bed902e00d6e3190bda738b5149c3a788d570e6cf48b974ec9548442850308ecd8fc9a67681f4ea8403129e7867bcb85adaf6ec238
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-unicode-property-regex@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-unicode-property-regex@npm:7.23.3"
+"@babel/plugin-transform-unicode-property-regex@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-unicode-property-regex@npm:7.24.1"
   dependencies:
     "@babel/helper-create-regexp-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 2298461a194758086d17c23c26c7de37aa533af910f9ebf31ebd0893d4aa317468043d23f73edc782ec21151d3c46cf0ff8098a83b725c49a59de28a1d4d6225
+  checksum: 276099b4483e707f80b054e2d29bc519158bfe52461ef5ff76f70727d592df17e30b1597ef4d8a0f04d810f6cb5a8dd887bdc1d0540af3744751710ef280090f
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-unicode-regex@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-unicode-regex@npm:7.23.3"
+"@babel/plugin-transform-unicode-regex@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-unicode-regex@npm:7.24.1"
   dependencies:
     "@babel/helper-create-regexp-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: c5f835d17483ba899787f92e313dfa5b0055e3deab332f1d254078a2bba27ede47574b6599fcf34d3763f0c048ae0779dc21d2d8db09295edb4057478dc80a9a
+  checksum: 400a0927bdb1425b4c0dc68a61b5b2d7d17c7d9f0e07317a1a6a373c080ef94be1dd65fdc4ac9a78fcdb58f89fd128450c7bc0d5b8ca0ae7eca3fbd98e50acba
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-unicode-sets-regex@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-unicode-sets-regex@npm:7.23.3"
+"@babel/plugin-transform-unicode-sets-regex@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-unicode-sets-regex@npm:7.24.1"
   dependencies:
     "@babel/helper-create-regexp-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: 79d0b4c951955ca68235c87b91ab2b393c96285f8aeaa34d6db416d2ddac90000c9bd6e8c4d82b60a2b484da69930507245035f28ba63c6cae341cf3ba68fdef
+  checksum: 364342fb8e382dfaa23628b88e6484dc1097e53fb7199f4d338f1e2cd71d839bb0a35a9b1380074f6a10adb2e98b79d53ca3ec78c0b8c557ca895ffff42180df
   languageName: node
   linkType: hard
 
 "@babel/preset-env@npm:^7.10.2, @babel/preset-env@npm:^7.12.1":
-  version: 7.23.9
-  resolution: "@babel/preset-env@npm:7.23.9"
+  version: 7.24.5
+  resolution: "@babel/preset-env@npm:7.24.5"
   dependencies:
-    "@babel/compat-data": ^7.23.5
+    "@babel/compat-data": ^7.24.4
     "@babel/helper-compilation-targets": ^7.23.6
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.5
     "@babel/helper-validator-option": ^7.23.5
-    "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression": ^7.23.3
-    "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining": ^7.23.3
-    "@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly": ^7.23.7
+    "@babel/plugin-bugfix-firefox-class-in-computed-class-key": ^7.24.5
+    "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression": ^7.24.1
+    "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining": ^7.24.1
+    "@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly": ^7.24.1
     "@babel/plugin-proposal-private-property-in-object": 7.21.0-placeholder-for-preset-env.2
     "@babel/plugin-syntax-async-generators": ^7.8.4
     "@babel/plugin-syntax-class-properties": ^7.12.13
     "@babel/plugin-syntax-class-static-block": ^7.14.5
     "@babel/plugin-syntax-dynamic-import": ^7.8.3
     "@babel/plugin-syntax-export-namespace-from": ^7.8.3
-    "@babel/plugin-syntax-import-assertions": ^7.23.3
-    "@babel/plugin-syntax-import-attributes": ^7.23.3
+    "@babel/plugin-syntax-import-assertions": ^7.24.1
+    "@babel/plugin-syntax-import-attributes": ^7.24.1
     "@babel/plugin-syntax-import-meta": ^7.10.4
     "@babel/plugin-syntax-json-strings": ^7.8.3
     "@babel/plugin-syntax-logical-assignment-operators": ^7.10.4
     "@babel/plugin-syntax-nullish-coalescing-operator": ^7.8.3
     "@babel/plugin-syntax-numeric-separator": ^7.10.4
     "@babel/plugin-syntax-object-rest-spread": ^7.8.3
     "@babel/plugin-syntax-optional-catch-binding": ^7.8.3
     "@babel/plugin-syntax-optional-chaining": ^7.8.3
     "@babel/plugin-syntax-private-property-in-object": ^7.14.5
     "@babel/plugin-syntax-top-level-await": ^7.14.5
     "@babel/plugin-syntax-unicode-sets-regex": ^7.18.6
-    "@babel/plugin-transform-arrow-functions": ^7.23.3
-    "@babel/plugin-transform-async-generator-functions": ^7.23.9
-    "@babel/plugin-transform-async-to-generator": ^7.23.3
-    "@babel/plugin-transform-block-scoped-functions": ^7.23.3
-    "@babel/plugin-transform-block-scoping": ^7.23.4
-    "@babel/plugin-transform-class-properties": ^7.23.3
-    "@babel/plugin-transform-class-static-block": ^7.23.4
-    "@babel/plugin-transform-classes": ^7.23.8
-    "@babel/plugin-transform-computed-properties": ^7.23.3
-    "@babel/plugin-transform-destructuring": ^7.23.3
-    "@babel/plugin-transform-dotall-regex": ^7.23.3
-    "@babel/plugin-transform-duplicate-keys": ^7.23.3
-    "@babel/plugin-transform-dynamic-import": ^7.23.4
-    "@babel/plugin-transform-exponentiation-operator": ^7.23.3
-    "@babel/plugin-transform-export-namespace-from": ^7.23.4
-    "@babel/plugin-transform-for-of": ^7.23.6
-    "@babel/plugin-transform-function-name": ^7.23.3
-    "@babel/plugin-transform-json-strings": ^7.23.4
-    "@babel/plugin-transform-literals": ^7.23.3
-    "@babel/plugin-transform-logical-assignment-operators": ^7.23.4
-    "@babel/plugin-transform-member-expression-literals": ^7.23.3
-    "@babel/plugin-transform-modules-amd": ^7.23.3
-    "@babel/plugin-transform-modules-commonjs": ^7.23.3
-    "@babel/plugin-transform-modules-systemjs": ^7.23.9
-    "@babel/plugin-transform-modules-umd": ^7.23.3
+    "@babel/plugin-transform-arrow-functions": ^7.24.1
+    "@babel/plugin-transform-async-generator-functions": ^7.24.3
+    "@babel/plugin-transform-async-to-generator": ^7.24.1
+    "@babel/plugin-transform-block-scoped-functions": ^7.24.1
+    "@babel/plugin-transform-block-scoping": ^7.24.5
+    "@babel/plugin-transform-class-properties": ^7.24.1
+    "@babel/plugin-transform-class-static-block": ^7.24.4
+    "@babel/plugin-transform-classes": ^7.24.5
+    "@babel/plugin-transform-computed-properties": ^7.24.1
+    "@babel/plugin-transform-destructuring": ^7.24.5
+    "@babel/plugin-transform-dotall-regex": ^7.24.1
+    "@babel/plugin-transform-duplicate-keys": ^7.24.1
+    "@babel/plugin-transform-dynamic-import": ^7.24.1
+    "@babel/plugin-transform-exponentiation-operator": ^7.24.1
+    "@babel/plugin-transform-export-namespace-from": ^7.24.1
+    "@babel/plugin-transform-for-of": ^7.24.1
+    "@babel/plugin-transform-function-name": ^7.24.1
+    "@babel/plugin-transform-json-strings": ^7.24.1
+    "@babel/plugin-transform-literals": ^7.24.1
+    "@babel/plugin-transform-logical-assignment-operators": ^7.24.1
+    "@babel/plugin-transform-member-expression-literals": ^7.24.1
+    "@babel/plugin-transform-modules-amd": ^7.24.1
+    "@babel/plugin-transform-modules-commonjs": ^7.24.1
+    "@babel/plugin-transform-modules-systemjs": ^7.24.1
+    "@babel/plugin-transform-modules-umd": ^7.24.1
     "@babel/plugin-transform-named-capturing-groups-regex": ^7.22.5
-    "@babel/plugin-transform-new-target": ^7.23.3
-    "@babel/plugin-transform-nullish-coalescing-operator": ^7.23.4
-    "@babel/plugin-transform-numeric-separator": ^7.23.4
-    "@babel/plugin-transform-object-rest-spread": ^7.23.4
-    "@babel/plugin-transform-object-super": ^7.23.3
-    "@babel/plugin-transform-optional-catch-binding": ^7.23.4
-    "@babel/plugin-transform-optional-chaining": ^7.23.4
-    "@babel/plugin-transform-parameters": ^7.23.3
-    "@babel/plugin-transform-private-methods": ^7.23.3
-    "@babel/plugin-transform-private-property-in-object": ^7.23.4
-    "@babel/plugin-transform-property-literals": ^7.23.3
-    "@babel/plugin-transform-regenerator": ^7.23.3
-    "@babel/plugin-transform-reserved-words": ^7.23.3
-    "@babel/plugin-transform-shorthand-properties": ^7.23.3
-    "@babel/plugin-transform-spread": ^7.23.3
-    "@babel/plugin-transform-sticky-regex": ^7.23.3
-    "@babel/plugin-transform-template-literals": ^7.23.3
-    "@babel/plugin-transform-typeof-symbol": ^7.23.3
-    "@babel/plugin-transform-unicode-escapes": ^7.23.3
-    "@babel/plugin-transform-unicode-property-regex": ^7.23.3
-    "@babel/plugin-transform-unicode-regex": ^7.23.3
-    "@babel/plugin-transform-unicode-sets-regex": ^7.23.3
+    "@babel/plugin-transform-new-target": ^7.24.1
+    "@babel/plugin-transform-nullish-coalescing-operator": ^7.24.1
+    "@babel/plugin-transform-numeric-separator": ^7.24.1
+    "@babel/plugin-transform-object-rest-spread": ^7.24.5
+    "@babel/plugin-transform-object-super": ^7.24.1
+    "@babel/plugin-transform-optional-catch-binding": ^7.24.1
+    "@babel/plugin-transform-optional-chaining": ^7.24.5
+    "@babel/plugin-transform-parameters": ^7.24.5
+    "@babel/plugin-transform-private-methods": ^7.24.1
+    "@babel/plugin-transform-private-property-in-object": ^7.24.5
+    "@babel/plugin-transform-property-literals": ^7.24.1
+    "@babel/plugin-transform-regenerator": ^7.24.1
+    "@babel/plugin-transform-reserved-words": ^7.24.1
+    "@babel/plugin-transform-shorthand-properties": ^7.24.1
+    "@babel/plugin-transform-spread": ^7.24.1
+    "@babel/plugin-transform-sticky-regex": ^7.24.1
+    "@babel/plugin-transform-template-literals": ^7.24.1
+    "@babel/plugin-transform-typeof-symbol": ^7.24.5
+    "@babel/plugin-transform-unicode-escapes": ^7.24.1
+    "@babel/plugin-transform-unicode-property-regex": ^7.24.1
+    "@babel/plugin-transform-unicode-regex": ^7.24.1
+    "@babel/plugin-transform-unicode-sets-regex": ^7.24.1
     "@babel/preset-modules": 0.1.6-no-external-plugins
-    babel-plugin-polyfill-corejs2: ^0.4.8
-    babel-plugin-polyfill-corejs3: ^0.9.0
-    babel-plugin-polyfill-regenerator: ^0.5.5
+    babel-plugin-polyfill-corejs2: ^0.4.10
+    babel-plugin-polyfill-corejs3: ^0.10.4
+    babel-plugin-polyfill-regenerator: ^0.6.1
     core-js-compat: ^3.31.0
     semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 23a48468ba820c68ba34ea2c1dbc62fd2ff9cf858cfb69e159cabb0c85c72dc4c2266ce20ca84318d8742de050cb061e7c66902fbfddbcb09246afd248847933
+  checksum: cced4e5331231158e02ba5903c4de12ef0aa2d2266ebb07fa80a85045b1fe2c63410d7558b702f1916d9d038531f3d79ab31007762188de5f712b16f7a66bb74
   languageName: node
   linkType: hard
 
 "@babel/preset-modules@npm:0.1.6-no-external-plugins":
   version: 0.1.6-no-external-plugins
   resolution: "@babel/preset-modules@npm:0.1.6-no-external-plugins"
   dependencies:
@@ -1307,185 +1313,185 @@
   version: 0.8.0
   resolution: "@babel/regjsgen@npm:0.8.0"
   checksum: 89c338fee774770e5a487382170711014d49a68eb281e74f2b5eac88f38300a4ad545516a7786a8dd5702e9cf009c94c2f582d200f077ac5decd74c56b973730
   languageName: node
   linkType: hard
 
 "@babel/runtime@npm:^7.8.4":
-  version: 7.23.9
-  resolution: "@babel/runtime@npm:7.23.9"
+  version: 7.24.5
+  resolution: "@babel/runtime@npm:7.24.5"
   dependencies:
     regenerator-runtime: ^0.14.0
-  checksum: 6bbebe8d27c0c2dd275d1ac197fc1a6c00e18dab68cc7aaff0adc3195b45862bae9c4cc58975629004b0213955b2ed91e99eccb3d9b39cabea246c657323d667
+  checksum: 755383192f3ac32ba4c62bd4f1ae92aed5b82d2c6665f39eb28fa94546777cf5c63493ea92dd03f1c2e621b17e860f190c056684b7f234270fdc91e29beda063
   languageName: node
   linkType: hard
 
-"@babel/template@npm:^7.22.15, @babel/template@npm:^7.23.9, @babel/template@npm:^7.3.3":
-  version: 7.23.9
-  resolution: "@babel/template@npm:7.23.9"
+"@babel/template@npm:^7.22.15, @babel/template@npm:^7.24.0, @babel/template@npm:^7.3.3":
+  version: 7.24.0
+  resolution: "@babel/template@npm:7.24.0"
   dependencies:
     "@babel/code-frame": ^7.23.5
-    "@babel/parser": ^7.23.9
-    "@babel/types": ^7.23.9
-  checksum: 6e67414c0f7125d7ecaf20c11fab88085fa98a96c3ef10da0a61e962e04fdf3a18a496a66047005ddd1bb682a7cc7842d556d1db2f3f3f6ccfca97d5e445d342
+    "@babel/parser": ^7.24.0
+    "@babel/types": ^7.24.0
+  checksum: f257b003c071a0cecdbfceca74185f18fe62c055469ab5c1d481aab12abeebed328e67e0a19fd978a2a8de97b28953fa4bc3da6d038a7345fdf37923b9fcdec8
   languageName: node
   linkType: hard
 
-"@babel/traverse@npm:^7.23.9":
-  version: 7.23.9
-  resolution: "@babel/traverse@npm:7.23.9"
+"@babel/traverse@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/traverse@npm:7.24.5"
   dependencies:
-    "@babel/code-frame": ^7.23.5
-    "@babel/generator": ^7.23.6
+    "@babel/code-frame": ^7.24.2
+    "@babel/generator": ^7.24.5
     "@babel/helper-environment-visitor": ^7.22.20
     "@babel/helper-function-name": ^7.23.0
     "@babel/helper-hoist-variables": ^7.22.5
-    "@babel/helper-split-export-declaration": ^7.22.6
-    "@babel/parser": ^7.23.9
-    "@babel/types": ^7.23.9
+    "@babel/helper-split-export-declaration": ^7.24.5
+    "@babel/parser": ^7.24.5
+    "@babel/types": ^7.24.5
     debug: ^4.3.1
     globals: ^11.1.0
-  checksum: a932f7aa850e158c00c97aad22f639d48c72805c687290f6a73e30c5c4957c07f5d28310c9bf59648e2980fe6c9d16adeb2ff92a9ca0f97fa75739c1328fc6c3
+  checksum: a313fbf4a06946cc4b74b06e9846d7393a9ca1e8b6df6da60c669cff0a9426d6198c21a478041c60807b62b48f980473d4afbd3768764b0d9741ac80f5dfa04f
   languageName: node
   linkType: hard
 
-"@babel/types@npm:^7.0.0, @babel/types@npm:^7.20.7, @babel/types@npm:^7.22.15, @babel/types@npm:^7.22.19, @babel/types@npm:^7.22.5, @babel/types@npm:^7.23.0, @babel/types@npm:^7.23.6, @babel/types@npm:^7.23.9, @babel/types@npm:^7.3.3, @babel/types@npm:^7.4.4, @babel/types@npm:^7.8.3":
-  version: 7.23.9
-  resolution: "@babel/types@npm:7.23.9"
+"@babel/types@npm:^7.0.0, @babel/types@npm:^7.20.7, @babel/types@npm:^7.22.15, @babel/types@npm:^7.22.5, @babel/types@npm:^7.23.0, @babel/types@npm:^7.24.0, @babel/types@npm:^7.24.5, @babel/types@npm:^7.3.3, @babel/types@npm:^7.4.4, @babel/types@npm:^7.8.3":
+  version: 7.24.5
+  resolution: "@babel/types@npm:7.24.5"
   dependencies:
-    "@babel/helper-string-parser": ^7.23.4
-    "@babel/helper-validator-identifier": ^7.22.20
+    "@babel/helper-string-parser": ^7.24.1
+    "@babel/helper-validator-identifier": ^7.24.5
     to-fast-properties: ^2.0.0
-  checksum: 0a9b008e9bfc89beb8c185e620fa0f8ed6c771f1e1b2e01e1596870969096fec7793898a1d64a035176abf1dd13e2668ee30bf699f2d92c210a8128f4b151e65
+  checksum: 8eeeacd996593b176e649ee49d8dc3f26f9bb6aa1e3b592030e61a0e58ea010fb018dccc51e5314c8139409ea6cbab02e29b33e674e1f6962d8e24c52da6375b
   languageName: node
   linkType: hard
 
 "@bcoe/v8-coverage@npm:^0.2.3":
   version: 0.2.3
   resolution: "@bcoe/v8-coverage@npm:0.2.3"
   checksum: 850f9305536d0f2bd13e9e0881cb5f02e4f93fad1189f7b2d4bebf694e3206924eadee1068130d43c11b750efcc9405f88a8e42ef098b6d75239c0f047de1a27
   languageName: node
   linkType: hard
 
-"@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.5.1, @codemirror/autocomplete@npm:^6.7.1":
-  version: 6.12.0
-  resolution: "@codemirror/autocomplete@npm:6.12.0"
+"@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.15.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.7.1":
+  version: 6.16.0
+  resolution: "@codemirror/autocomplete@npm:6.16.0"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
   peerDependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
-  checksum: 1d4da6ccc12f5a67053a76b361f2683b5af031dd405a0bd2a261a265eb8cb7dfb115343a3291260d1ba31ce7ccb5427208ebe50f50f6747fcf27a50b62c87f7e
+  checksum: e33d3d8c961c03dc4a70d1ac6f01aee5362d778da9d873a8335aed47f7de9430eab083589736e7922464b941d5da23c51ab6af05400413a8d1a07604ffcb99f7
   languageName: node
   linkType: hard
 
-"@codemirror/commands@npm:^6.2.3":
-  version: 6.3.3
-  resolution: "@codemirror/commands@npm:6.3.3"
+"@codemirror/commands@npm:^6.3.3":
+  version: 6.5.0
+  resolution: "@codemirror/commands@npm:6.5.0"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.4.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.1.0
-  checksum: 7d23aecc973823969434b839aefa9a98bb47212d2ce0e6869ae903adbb5233aad22a760788fb7bb6eb45b00b01a4932fb93ad43bacdcbc0215e7500cf54b17bb
+  checksum: 27e49c5e0cb918b95d6a9f741bcc0e72cb76f963b0c829308edfb4491a37d8b12ae6fb96f9f1886b3189a22c82fec4434fbe65547dc3cd3e8dfb5222dfead2e7
   languageName: node
   linkType: hard
 
 "@codemirror/lang-cpp@npm:^6.0.2":
   version: 6.0.2
   resolution: "@codemirror/lang-cpp@npm:6.0.2"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/cpp": ^1.0.0
   checksum: bb9eba482cca80037ce30c7b193cf45eff19ccbb773764fddf2071756468ecc25aa53c777c943635054f89095b0247b9b50c339e107e41e68d34d12a7295f9a9
   languageName: node
   linkType: hard
 
-"@codemirror/lang-css@npm:^6.0.0, @codemirror/lang-css@npm:^6.1.1":
+"@codemirror/lang-css@npm:^6.0.0, @codemirror/lang-css@npm:^6.2.1":
   version: 6.2.1
   resolution: "@codemirror/lang-css@npm:6.2.1"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.0.2
     "@lezer/css": ^1.0.0
   checksum: 5a8457ee8a4310030a969f2d3128429f549c4dc9b7907ee8888b42119c80b65af99093801432efdf659b8ec36a147d2a947bc1ecbbf69a759395214e3f4834a8
   languageName: node
   linkType: hard
 
-"@codemirror/lang-html@npm:^6.0.0, @codemirror/lang-html@npm:^6.4.3":
-  version: 6.4.8
-  resolution: "@codemirror/lang-html@npm:6.4.8"
+"@codemirror/lang-html@npm:^6.0.0, @codemirror/lang-html@npm:^6.4.8":
+  version: 6.4.9
+  resolution: "@codemirror/lang-html@npm:6.4.9"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/lang-css": ^6.0.0
     "@codemirror/lang-javascript": ^6.0.0
     "@codemirror/language": ^6.4.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
     "@lezer/css": ^1.1.0
     "@lezer/html": ^1.3.0
-  checksum: 9aec56c333cc06f9e4bb6d09806ae83e4a7f235a26b3244010e2dcea83a923cfcd7bec84904b8a59bc81256b0bb579a52bf5614962dad031d7577db1c49a216a
+  checksum: ac8c3ceb0396f2e032752c5079bd950124dca708bc64e96fc147dc5fe7133e5cee0814fe951abdb953ec1d11fa540e4b30a712b5149d9a36016a197a28de45d7
   languageName: node
   linkType: hard
 
 "@codemirror/lang-java@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-java@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/java": ^1.0.0
   checksum: 4679104683cbffcd224ac04c7e5d144b787494697b26470b07017259035b7bb3fa62609d9a61bfbc566f1756d9f972f9f26d96a3c1362dd48881c1172f9a914d
   languageName: node
   linkType: hard
 
-"@codemirror/lang-javascript@npm:^6.0.0, @codemirror/lang-javascript@npm:^6.1.7":
-  version: 6.2.1
-  resolution: "@codemirror/lang-javascript@npm:6.2.1"
+"@codemirror/lang-javascript@npm:^6.0.0, @codemirror/lang-javascript@npm:^6.2.2":
+  version: 6.2.2
+  resolution: "@codemirror/lang-javascript@npm:6.2.2"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.6.0
     "@codemirror/lint": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
     "@lezer/javascript": ^1.0.0
-  checksum: 3df38c4cced06195283a9a2a9365aaa7c8c1b157852b331bc3a118403f774bbba57d2a392de52f5e28d2b344a323bc0146bcf7c8ef8be2473f167d815e4a37cd
+  checksum: 66379942a8347dff2bd76d10ed7cf313bca83872f8336fdd3e14accfef23e7b690cd913c9d11a3854fba2b32299da07fc3275995327642c9ee43c2a8e538c19d
   languageName: node
   linkType: hard
 
 "@codemirror/lang-json@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-json@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/json": ^1.0.0
   checksum: e9e87d50ff7b81bd56a6ab50740b1dd54e9a93f1be585e1d59d0642e2148842ea1528ac7b7221eb4ddc7fe84bbc28065144cc3ab86f6e06c6aeb2d4b4e62acf1
   languageName: node
   linkType: hard
 
-"@codemirror/lang-markdown@npm:^6.1.1":
-  version: 6.2.4
-  resolution: "@codemirror/lang-markdown@npm:6.2.4"
+"@codemirror/lang-markdown@npm:^6.2.4":
+  version: 6.2.5
+  resolution: "@codemirror/lang-markdown@npm:6.2.5"
   dependencies:
     "@codemirror/autocomplete": ^6.7.1
     "@codemirror/lang-html": ^6.0.0
     "@codemirror/language": ^6.3.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.2.1
     "@lezer/markdown": ^1.0.0
-  checksum: fbdf1388a9fd08b4e6fc9950ac57fc59ef02bb0bd3e76654158ce1494b101356ded049b65dcf6da457e7e302cb178bf30852fd152680f3a8679be3c3884c0bc2
+  checksum: 3d9e0817f888eddcb6d05ec8f0d8dacbde7b9ef7650303bc4ab8b08a550a986c60c65b1565212e06af389c31590330f1f5ed65e619a9446dc2979ff3dac0e874
   languageName: node
   linkType: hard
 
 "@codemirror/lang-php@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-php@npm:6.0.1"
   dependencies:
@@ -1494,136 +1500,137 @@
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/php": ^1.0.0
   checksum: c003a29a426486453fdfddbf7302982fa2aa7f059bf6f1ce4cbf08341b0162eee5e2f50e0d71c418dcd358491631780156d846fe352754d042576172c5d86721
   languageName: node
   linkType: hard
 
-"@codemirror/lang-python@npm:^6.1.3":
-  version: 6.1.4
-  resolution: "@codemirror/lang-python@npm:6.1.4"
+"@codemirror/lang-python@npm:^6.1.4":
+  version: 6.1.6
+  resolution: "@codemirror/lang-python@npm:6.1.6"
   dependencies:
     "@codemirror/autocomplete": ^6.3.2
     "@codemirror/language": ^6.8.0
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.2.1
     "@lezer/python": ^1.1.4
-  checksum: 94d0126bc5da4878eb3cc4da5afae4dc2ca7bb1c4c1f483e786ec0fed439490bb6ed8cad0a6090e2638e6b3453a6f4225bfaa3b49aac5cfb3e466556d0aaae1e
+  checksum: eb1faabd332bb95d0f3e227eb19ac5a31140cf238905bbe73e061040999f5680a012f9145fb3688bc2fcbb1908c957511edc8eeb8a9aa88d27d4fa55ad451e95
   languageName: node
   linkType: hard
 
 "@codemirror/lang-rust@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-rust@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/rust": ^1.0.0
   checksum: 8a439944cb22159b0b3465ca4fa4294c69843219d5d30e278ae6df8e48f30a7a9256129723c025ec9b5e694d31a3560fb004300b125ffcd81c22d13825845170
   languageName: node
   linkType: hard
 
-"@codemirror/lang-sql@npm:^6.4.1":
-  version: 6.5.5
-  resolution: "@codemirror/lang-sql@npm:6.5.5"
+"@codemirror/lang-sql@npm:^6.6.1":
+  version: 6.6.4
+  resolution: "@codemirror/lang-sql@npm:6.6.4"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 404003ae73b986bd7a00f6924db78b7ffb28fdc38d689fdc11416aaafe2d5c6dc37cc18972530f82e940acb61e18ac74a1cf7712beef448c145344ff93970dc3
+  checksum: ae7c498d08c118d8f1751c28d12c54f45cacd589f6adb56216d44eb14abc0e436dcefe675d50bd02a242426327384cbcafa8c35098aa63384570a33c4cf27038
   languageName: node
   linkType: hard
 
-"@codemirror/lang-wast@npm:^6.0.1":
+"@codemirror/lang-wast@npm:^6.0.2":
   version: 6.0.2
   resolution: "@codemirror/lang-wast@npm:6.0.2"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: 72119d4a7d726c54167aa227c982ae9fa785c8ad97a158d8350ae95eecfbd8028a803eef939f7e6c5c6e626fcecda1dc37e9dffc6d5d6ec105f686aeda6b2c24
   languageName: node
   linkType: hard
 
-"@codemirror/lang-xml@npm:^6.0.2":
-  version: 6.0.2
-  resolution: "@codemirror/lang-xml@npm:6.0.2"
+"@codemirror/lang-xml@npm:^6.1.0":
+  version: 6.1.0
+  resolution: "@codemirror/lang-xml@npm:6.1.0"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.4.0
     "@codemirror/state": ^6.0.0
+    "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/xml": ^1.0.0
-  checksum: e156ecafaa87e9b6ef4ab6812ccd00d8f3c6cb81f232837636b36336d80513b61936dfee6f4f6800574f236208b61e95a2abcb997cdcd7366585a6b796e0e13b
+  checksum: 3a1b7af07b29ad7e53b77bf584245580b613bc92256059f175f2b1d7c28c4e39b75654fe169b9a8a330a60164b53ff5254bdb5b8ee8c6e6766427ee115c4e229
   languageName: node
   linkType: hard
 
-"@codemirror/language@npm:^6.0.0, @codemirror/language@npm:^6.3.0, @codemirror/language@npm:^6.4.0, @codemirror/language@npm:^6.6.0, @codemirror/language@npm:^6.8.0":
+"@codemirror/language@npm:^6.0.0, @codemirror/language@npm:^6.10.1, @codemirror/language@npm:^6.3.0, @codemirror/language@npm:^6.4.0, @codemirror/language@npm:^6.6.0, @codemirror/language@npm:^6.8.0":
   version: 6.10.1
   resolution: "@codemirror/language@npm:6.10.1"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.23.0
     "@lezer/common": ^1.1.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
     style-mod: ^4.0.0
   checksum: 453bbe122a84795752f29261412b69a8dcfdd7e4369eb7e112bffba36b9e527ad21adff1d3845e0dc44c9ab44eb0c6f823eb6ba790ddd00cc749847574eda779
   languageName: node
   linkType: hard
 
-"@codemirror/legacy-modes@npm:^6.3.2":
-  version: 6.3.3
-  resolution: "@codemirror/legacy-modes@npm:6.3.3"
+"@codemirror/legacy-modes@npm:^6.3.3":
+  version: 6.4.0
+  resolution: "@codemirror/legacy-modes@npm:6.4.0"
   dependencies:
     "@codemirror/language": ^6.0.0
-  checksum: 3cd32b0f011b0a193e0948e5901b625f38aa6d9a8b24344531d6e142eb6fbb3e6cb5969429102044f3d04fbe53c4deaebd9f659c05067a0b18d17766290c9e05
+  checksum: d382aa6f640a67418bd209e1e4b395340f96aac1b0cf185927fc2c7f98b62cfd0c59ef0f7048148ce8771622003ca844c78c2d18548235ecc57d0bcbfbbfe091
   languageName: node
   linkType: hard
 
 "@codemirror/lint@npm:^6.0.0":
-  version: 6.5.0
-  resolution: "@codemirror/lint@npm:6.5.0"
+  version: 6.7.1
+  resolution: "@codemirror/lint@npm:6.7.1"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
-  checksum: b4f3899d0f73e5a2b5e9bc1df8e13ecb9324b94c7d384e7c8dde794109dee051461fc86658338f41652b44879b2ccc12cdd51a8ac0bb16a5b18aafa8e57a843c
+  checksum: b3f52b16367abe150c734b75fd9224132a06c83ebc8148724acd1352fa27d4565a3b29dbdf31d5e27a9232d595fc32c23d68321391e7345d13937ad88b48a87f
   languageName: node
   linkType: hard
 
-"@codemirror/search@npm:^6.3.0":
+"@codemirror/search@npm:^6.5.6":
   version: 6.5.6
   resolution: "@codemirror/search@npm:6.5.6"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
   checksum: 19dc88d09fc750563347001e83c6194bbb2a25c874bd919d2d81809e1f98d6330222ddbd284aa9758a09eeb41fd153ec7c2cf810b2ee51452c25963d7f5833d5
   languageName: node
   linkType: hard
 
-"@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.2.0, @codemirror/state@npm:^6.4.0":
-  version: 6.4.0
-  resolution: "@codemirror/state@npm:6.4.0"
-  checksum: c5236fe5786f1b85d17273a5c17fa8aeb063658c1404ab18caeb6e7591663ec96b65d453ab8162f75839c3801b04cd55ba4bc48f44cb61ebfeeee383f89553c7
+"@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.4.0, @codemirror/state@npm:^6.4.1":
+  version: 6.4.1
+  resolution: "@codemirror/state@npm:6.4.1"
+  checksum: b81b55574091349eed4d32fc0eadb0c9688f1f7c98b681318f59138ee0f527cb4c4a97831b70547c0640f02f3127647838ae6730782de4a3dd2cc58836125d01
   languageName: node
   linkType: hard
 
-"@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.17.0, @codemirror/view@npm:^6.23.0, @codemirror/view@npm:^6.9.6":
-  version: 6.24.0
-  resolution: "@codemirror/view@npm:6.24.0"
+"@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.17.0, @codemirror/view@npm:^6.23.0, @codemirror/view@npm:^6.26.0":
+  version: 6.26.3
+  resolution: "@codemirror/view@npm:6.26.3"
   dependencies:
     "@codemirror/state": ^6.4.0
     style-mod: ^4.1.0
     w3c-keyname: ^2.2.4
-  checksum: c594f7628074d6f1a87636bb1281d1a1b579d0d73df4f8e04972eb7aca53de9c98f45e585d059f682920a89fa68dcad85a1418df90c28a746ae52aa06cdd0b8f
+  checksum: fdee35fb5e0bbba7b6f1a9b43a865880911bbfafd30360da5dda21b35f81ba2d080ff66b6c3d94dbe946b6b7ec98a76208786360b8f030ef10bcb054b816de05
   languageName: node
   linkType: hard
 
 "@discoveryjs/json-ext@npm:^0.5.0":
   version: 0.5.7
   resolution: "@discoveryjs/json-ext@npm:0.5.7"
   checksum: 2176d301cc258ea5c2324402997cf8134ebb212469c0d397591636cea8d3c02f2b3cf9fd58dcb748c7a0dade77ebdc1b10284fa63e608c033a1db52fddc69918
@@ -1661,18 +1668,18 @@
     js-yaml: ^4.1.0
     minimatch: ^3.1.2
     strip-json-comments: ^3.1.1
   checksum: 10957c7592b20ca0089262d8c2a8accbad14b4f6507e35416c32ee6b4dbf9cad67dfb77096bbd405405e9ada2b107f3797fe94362e1c55e0b09d6e90dd149127
   languageName: node
   linkType: hard
 
-"@eslint/js@npm:8.56.0":
-  version: 8.56.0
-  resolution: "@eslint/js@npm:8.56.0"
-  checksum: 5804130574ef810207bdf321c265437814e7a26f4e6fac9b496de3206afd52f533e09ec002a3be06cd9adcc9da63e727f1883938e663c4e4751c007d5b58e539
+"@eslint/js@npm:8.57.0":
+  version: 8.57.0
+  resolution: "@eslint/js@npm:8.57.0"
+  checksum: 315dc65b0e9893e2bff139bddace7ea601ad77ed47b4550e73da8c9c2d2766c7a575c3cddf17ef85b8fd6a36ff34f91729d0dcca56e73ca887c10df91a41b0bb
   languageName: node
   linkType: hard
 
 "@fortawesome/fontawesome-free@npm:^5.12.0":
   version: 5.15.4
   resolution: "@fortawesome/fontawesome-free@npm:5.15.4"
   checksum: 32281c3df4075290d9a96dfc22f72fadb3da7055d4117e48d34046b8c98032a55fa260ae351b0af5d6f6fb57a2f5d79a4abe52af456da35195f7cb7dda27b4a2
@@ -1682,15 +1689,15 @@
 "@gar/promisify@npm:^1.1.3":
   version: 1.1.3
   resolution: "@gar/promisify@npm:1.1.3"
   checksum: 4059f790e2d07bf3c3ff3e0fec0daa8144fe35c1f6e0111c9921bd32106adaa97a4ab096ad7dab1e28ee6a9060083c4d1a4ada42a7f5f3f7a96b8812e2b757c1
   languageName: node
   linkType: hard
 
-"@humanwhocodes/config-array@npm:^0.11.13":
+"@humanwhocodes/config-array@npm:^0.11.14":
   version: 0.11.14
   resolution: "@humanwhocodes/config-array@npm:0.11.14"
   dependencies:
     "@humanwhocodes/object-schema": ^2.0.2
     debug: ^4.3.1
     minimatch: ^3.0.5
   checksum: 861ccce9eaea5de19546653bccf75bf09fe878bc39c3aab00aeee2d2a0e654516adad38dd1098aab5e3af0145bbcbf3f309bdf4d964f8dab9dcd5834ae4c02f2
@@ -1701,17 +1708,17 @@
   version: 1.0.1
   resolution: "@humanwhocodes/module-importer@npm:1.0.1"
   checksum: 0fd22007db8034a2cdf2c764b140d37d9020bbfce8a49d3ec5c05290e77d4b0263b1b972b752df8c89e5eaa94073408f2b7d977aed131faf6cf396ebb5d7fb61
   languageName: node
   linkType: hard
 
 "@humanwhocodes/object-schema@npm:^2.0.2":
-  version: 2.0.2
-  resolution: "@humanwhocodes/object-schema@npm:2.0.2"
-  checksum: 2fc11503361b5fb4f14714c700c02a3f4c7c93e9acd6b87a29f62c522d90470f364d6161b03d1cc618b979f2ae02aed1106fd29d302695d8927e2fc8165ba8ee
+  version: 2.0.3
+  resolution: "@humanwhocodes/object-schema@npm:2.0.3"
+  checksum: d3b78f6c5831888c6ecc899df0d03bcc25d46f3ad26a11d7ea52944dc36a35ef543fad965322174238d677a43d5c694434f6607532cff7077062513ad7022631
   languageName: node
   linkType: hard
 
 "@hutson/parse-repository-url@npm:^3.0.0":
   version: 3.0.2
   resolution: "@hutson/parse-repository-url@npm:3.0.2"
   checksum: 39992c5f183c5ca3d761d6ed9dfabcb79b5f3750bf1b7f3532e1dc439ca370138bbd426ee250fdaba460bc948e6761fbefd484b8f4f36885d71ded96138340d1
@@ -1748,15 +1755,15 @@
     get-package-type: ^0.1.0
     js-yaml: ^3.13.1
     resolve-from: ^5.0.0
   checksum: d578da5e2e804d5c93228450a1380e1a3c691de4953acc162f387b717258512a3e07b83510a936d9fab03eac90817473917e24f5d16297af3867f59328d58568
   languageName: node
   linkType: hard
 
-"@istanbuljs/schema@npm:^0.1.2":
+"@istanbuljs/schema@npm:^0.1.2, @istanbuljs/schema@npm:^0.1.3":
   version: 0.1.3
   resolution: "@istanbuljs/schema@npm:0.1.3"
   checksum: 5282759d961d61350f33d9118d16bcaed914ebf8061a52f4fa474b2cb08720c9c81d165e13b82f2e5a8a212cc5af482f0c6fc1ac27b9e067e5394c9a6ed186c9
   languageName: node
   linkType: hard
 
 "@jest/console@npm:^29.7.0":
@@ -1985,86 +1992,86 @@
     "@types/node": "*"
     "@types/yargs": ^17.0.8
     chalk: ^4.0.0
   checksum: a0bcf15dbb0eca6bdd8ce61a3fb055349d40268622a7670a3b2eb3c3dbafe9eb26af59938366d520b86907b9505b0f9b29b85cec11579a9e580694b87cd90fcc
   languageName: node
   linkType: hard
 
-"@jridgewell/gen-mapping@npm:^0.3.0, @jridgewell/gen-mapping@npm:^0.3.2":
-  version: 0.3.3
-  resolution: "@jridgewell/gen-mapping@npm:0.3.3"
+"@jridgewell/gen-mapping@npm:^0.3.5":
+  version: 0.3.5
+  resolution: "@jridgewell/gen-mapping@npm:0.3.5"
   dependencies:
-    "@jridgewell/set-array": ^1.0.1
+    "@jridgewell/set-array": ^1.2.1
     "@jridgewell/sourcemap-codec": ^1.4.10
-    "@jridgewell/trace-mapping": ^0.3.9
-  checksum: 4a74944bd31f22354fc01c3da32e83c19e519e3bbadafa114f6da4522ea77dd0c2842607e923a591d60a76699d819a2fbb6f3552e277efdb9b58b081390b60ab
+    "@jridgewell/trace-mapping": ^0.3.24
+  checksum: ff7a1764ebd76a5e129c8890aa3e2f46045109dabde62b0b6c6a250152227647178ff2069ea234753a690d8f3c4ac8b5e7b267bbee272bffb7f3b0a370ab6e52
   languageName: node
   linkType: hard
 
 "@jridgewell/resolve-uri@npm:^3.1.0":
   version: 3.1.2
   resolution: "@jridgewell/resolve-uri@npm:3.1.2"
   checksum: 83b85f72c59d1c080b4cbec0fef84528963a1b5db34e4370fa4bd1e3ff64a0d80e0cee7369d11d73c704e0286fb2865b530acac7a871088fbe92b5edf1000870
   languageName: node
   linkType: hard
 
-"@jridgewell/set-array@npm:^1.0.1":
-  version: 1.1.2
-  resolution: "@jridgewell/set-array@npm:1.1.2"
-  checksum: 69a84d5980385f396ff60a175f7177af0b8da4ddb81824cb7016a9ef914eee9806c72b6b65942003c63f7983d4f39a5c6c27185bbca88eb4690b62075602e28e
+"@jridgewell/set-array@npm:^1.2.1":
+  version: 1.2.1
+  resolution: "@jridgewell/set-array@npm:1.2.1"
+  checksum: 832e513a85a588f8ed4f27d1279420d8547743cc37fcad5a5a76fc74bb895b013dfe614d0eed9cb860048e6546b798f8f2652020b4b2ba0561b05caa8c654b10
   languageName: node
   linkType: hard
 
 "@jridgewell/source-map@npm:^0.3.3":
-  version: 0.3.5
-  resolution: "@jridgewell/source-map@npm:0.3.5"
+  version: 0.3.6
+  resolution: "@jridgewell/source-map@npm:0.3.6"
   dependencies:
-    "@jridgewell/gen-mapping": ^0.3.0
-    "@jridgewell/trace-mapping": ^0.3.9
-  checksum: 1ad4dec0bdafbade57920a50acec6634f88a0eb735851e0dda906fa9894e7f0549c492678aad1a10f8e144bfe87f238307bf2a914a1bc85b7781d345417e9f6f
+    "@jridgewell/gen-mapping": ^0.3.5
+    "@jridgewell/trace-mapping": ^0.3.25
+  checksum: c9dc7d899397df95e3c9ec287b93c0b56f8e4453cd20743e2b9c8e779b1949bc3cccf6c01bb302779e46560eb45f62ea38d19fedd25370d814734268450a9f30
   languageName: node
   linkType: hard
 
 "@jridgewell/sourcemap-codec@npm:^1.4.10, @jridgewell/sourcemap-codec@npm:^1.4.14":
   version: 1.4.15
   resolution: "@jridgewell/sourcemap-codec@npm:1.4.15"
   checksum: b881c7e503db3fc7f3c1f35a1dd2655a188cc51a3612d76efc8a6eb74728bef5606e6758ee77423e564092b4a518aba569bbb21c9bac5ab7a35b0c6ae7e344c8
   languageName: node
   linkType: hard
 
-"@jridgewell/trace-mapping@npm:^0.3.12, @jridgewell/trace-mapping@npm:^0.3.17, @jridgewell/trace-mapping@npm:^0.3.18, @jridgewell/trace-mapping@npm:^0.3.20, @jridgewell/trace-mapping@npm:^0.3.9":
-  version: 0.3.22
-  resolution: "@jridgewell/trace-mapping@npm:0.3.22"
+"@jridgewell/trace-mapping@npm:^0.3.12, @jridgewell/trace-mapping@npm:^0.3.18, @jridgewell/trace-mapping@npm:^0.3.20, @jridgewell/trace-mapping@npm:^0.3.24, @jridgewell/trace-mapping@npm:^0.3.25":
+  version: 0.3.25
+  resolution: "@jridgewell/trace-mapping@npm:0.3.25"
   dependencies:
     "@jridgewell/resolve-uri": ^3.1.0
     "@jridgewell/sourcemap-codec": ^1.4.14
-  checksum: ac7dd2cfe0b479aa1b81776d40d789243131cc792dc8b6b6a028c70fcd6171958ae1a71bf67b618ffe3c0c3feead9870c095ee46a5e30319410d92976b28f498
+  checksum: 9d3c40d225e139987b50c48988f8717a54a8c994d8a948ee42e1412e08988761d0754d7d10b803061cc3aebf35f92a5dbbab493bd0e1a9ef9e89a2130e83ba34
   languageName: node
   linkType: hard
 
-"@jupyter/react-components@npm:^0.15.2":
-  version: 0.15.2
-  resolution: "@jupyter/react-components@npm:0.15.2"
+"@jupyter/react-components@npm:^0.15.3":
+  version: 0.15.3
+  resolution: "@jupyter/react-components@npm:0.15.3"
   dependencies:
-    "@jupyter/web-components": ^0.15.2
+    "@jupyter/web-components": ^0.15.3
     "@microsoft/fast-react-wrapper": ^0.3.22
     react: ">=17.0.0 <19.0.0"
-  checksum: d6d339ff9c2fed1fd5afda612be500d73c4a83eee5470d50e94020dadd1e389a3bf745c7240b0a48edbc6d3fdacec93367b7b5e40588f2df588419caada705be
+  checksum: 1a6b256314259c6465c4b6d958575710536b82234a7bf0fba3e889a07e1f19ff8ab321450be354359876f92c45dbcc9d21a840237ff4a619806d9de696f55496
   languageName: node
   linkType: hard
 
-"@jupyter/web-components@npm:^0.15.2":
-  version: 0.15.2
-  resolution: "@jupyter/web-components@npm:0.15.2"
+"@jupyter/web-components@npm:^0.15.3":
+  version: 0.15.3
+  resolution: "@jupyter/web-components@npm:0.15.3"
   dependencies:
     "@microsoft/fast-colors": ^5.3.1
     "@microsoft/fast-element": ^1.12.0
     "@microsoft/fast-foundation": ^2.49.4
     "@microsoft/fast-web-utilities": ^5.4.1
-  checksum: f272ef91de08e28f9414a26dbd2388e1a8985c90f4ab00231978cee49bd5212f812411397a9038d298c8c0c4b41eb28cc86f1127bc7ace309bda8df60c4a87c8
+  checksum: a0980af934157bfdbdb6cc169c0816c1b2e57602d524c56bdcef746a4c25dfeb8f505150d83207c8695ed89b5486cf53d35a3382584d25ef64db666e4e16e45b
   languageName: node
   linkType: hard
 
 "@jupyter/ydoc@npm:^1.1.1":
   version: 1.1.1
   resolution: "@jupyter/ydoc@npm:1.1.1"
   dependencies:
@@ -2074,88 +2081,102 @@
     "@lumino/signaling": ^1.10.0 || ^2.0.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   checksum: a239b1dd57cfc9ba36c06ac5032a1b6388849ae01a1d0db0d45094f71fdadf4d473b4bf8becbef0cfcdc85cae505361fbec0822b02da5aa48e06b66f742dd7a0
   languageName: node
   linkType: hard
 
-"@jupyterlab/application@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/application@npm:4.1.1"
+"@jupyter/ydoc@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "@jupyter/ydoc@npm:2.0.1"
+  dependencies:
+    "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0
+    "@lumino/coreutils": ^1.11.0 || ^2.0.0
+    "@lumino/disposable": ^1.10.0 || ^2.0.0
+    "@lumino/signaling": ^1.10.0 || ^2.0.0
+    y-protocols: ^1.0.5
+    yjs: ^13.5.40
+  checksum: f5f29e1ff3327ebc1cf326f53634e03c4c7bf7733d235087fe26975c16eebd404f23c2f3ba88b6e04b1927846be7162b09b8b8719a4b29e51d0299c745018cbb
+  languageName: node
+  linkType: hard
+
+"@jupyterlab/application@npm:^4.1.8":
+  version: 4.2.0
+  resolution: "@jupyterlab/application@npm:4.2.0"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/docregistry": ^4.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/statedb": ^4.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/docregistry": ^4.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/statedb": ^4.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
-    "@lumino/application": ^2.3.0
-    "@lumino/commands": ^2.2.0
+    "@lumino/application": ^2.3.1
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
-  checksum: d8b1254c6eb5db30133703926d82e75d8655001af863007bf69e73e4e3e98cc0159ffd55a32f03121b602215b354e7e467fed0cabd7b109b9928c81f45166375
+    "@lumino/widgets": ^2.3.2
+  checksum: 74811d63ddf4e6628c2467659ca1b0c39bba271689cff05925efbd3529bf4c771d41f42b04a458d1acdb0ced87b5fee5fb31d315a5b45e3449bd5f581f3be377
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:^4.2.1":
-  version: 4.2.1
-  resolution: "@jupyterlab/apputils@npm:4.2.1"
+"@jupyterlab/apputils@npm:^4.2.8, @jupyterlab/apputils@npm:^4.3.0":
+  version: 4.3.0
+  resolution: "@jupyterlab/apputils@npm:4.3.0"
   dependencies:
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/settingregistry": ^4.1.1
-    "@jupyterlab/statedb": ^4.1.1
-    "@jupyterlab/statusbar": ^4.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/settingregistry": ^4.2.0
+    "@jupyterlab/statedb": ^4.2.0
+    "@jupyterlab/statusbar": ^4.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     "@types/react": ^18.0.26
     react: ^18.2.0
-    sanitize-html: ~2.7.3
-  checksum: e64f4d342c97a32ec74ef7045fd4793d998fea0f9bb296835a597b4a0e0739904dd8dd3ff5531fbcd8fc53bae40f6c796143a0b06dd7851c78afd1d4ffaa7ccd
+    sanitize-html: ~2.12.1
+  checksum: 96f4f9055c464fb6f0e2545d21623b9500936da44cd7bafa9c1154164f6fc1846a518bc637ef46d6a082d208d12acf737d8aa679ce5546427ac04f068cf10cd5
   languageName: node
   linkType: hard
 
-"@jupyterlab/attachments@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/attachments@npm:4.1.1"
+"@jupyterlab/attachments@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/attachments@npm:4.2.0"
   dependencies:
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
-  checksum: a0dfbcf9b74743574ecbb917f8193ad443e360471c911c946b5f810f06259e80b54c530133badd6fef7042ab13c1f3f57fb3a8d3bbc9462df3541bd5d0ea0017
+  checksum: 1224fe573aadeaf09f803d7619d3ecadc5b8f8d85ae76abb1cbd09a12be7a55f1f84ce29f576eb4bb8f806e28a412edce26fbae7fb841e9cb7fbcce1f5cf4bf4
   languageName: node
   linkType: hard
 
 "@jupyterlab/builder@npm:~4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/builder@npm:4.1.1"
+  version: 4.1.8
+  resolution: "@jupyterlab/builder@npm:4.1.8"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/application": ^2.3.0
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
@@ -2182,645 +2203,646 @@
     terser-webpack-plugin: ^5.3.7
     webpack: ^5.76.1
     webpack-cli: ^5.0.1
     webpack-merge: ^5.8.0
     worker-loader: ^3.0.2
   bin:
     build-labextension: lib/build-labextension.js
-  checksum: 4bc1c00a29effe964f44b0277dbd14f97735a886e31945d77eb1c119396f2cad8783090571e357f2f2628732bcaf067224e2b11b6daba137490a85b86d5da4ab
+  checksum: e727e4fddbfd4e8f7d4c83e5c5aaf9be41b67771f6a4ef10b44bbc0e51bb21966b2fa1ad33eacf58420ca3a2cda2ab410331a1543e6f945b9ca0a59e109f240b
   languageName: node
   linkType: hard
 
-"@jupyterlab/cells@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/cells@npm:4.1.1"
+"@jupyterlab/cells@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/cells@npm:4.2.0"
   dependencies:
-    "@codemirror/state": ^6.2.0
-    "@codemirror/view": ^6.9.6
-    "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/attachments": ^4.1.1
-    "@jupyterlab/codeeditor": ^4.1.1
-    "@jupyterlab/codemirror": ^4.1.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/documentsearch": ^4.1.1
-    "@jupyterlab/filebrowser": ^4.1.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/outputarea": ^4.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/toc": ^6.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@codemirror/state": ^6.4.1
+    "@codemirror/view": ^6.26.0
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/attachments": ^4.2.0
+    "@jupyterlab/codeeditor": ^4.2.0
+    "@jupyterlab/codemirror": ^4.2.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/documentsearch": ^4.2.0
+    "@jupyterlab/filebrowser": ^4.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/outputarea": ^4.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/toc": ^6.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: 5590da50acdd1f25255ce28e4f50d6c5425d872c241723074ed8ab050dc650362cac1f74b355eb01066654eb9fa532b993f002bcce01ab3768fac7552498492b
+  checksum: 444ddf33c9ecda1880af67cd163a6b0416f761e5e454b4fe6dc36dc9b7f39f0deaca063bfd17de6312a2627f38a44645599d9a42501e2e2790d45a395e149a9a
   languageName: node
   linkType: hard
 
-"@jupyterlab/codeeditor@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/codeeditor@npm:4.1.1"
+"@jupyterlab/codeeditor@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/codeeditor@npm:4.2.0"
   dependencies:
-    "@codemirror/state": ^6.2.0
-    "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/statusbar": ^4.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@codemirror/state": ^6.4.1
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/statusbar": ^4.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: d29817772368d30352da4631592f3bacf73dba12031f06247c16e2e3122a65ab7d5feca254f69fb61e3f4dad83cc1f148310b3474a00be60b8fc25cc15846dda
+  checksum: a6e2b1cf7e46ae86154b20bd4a3c29c7c4bb0feb7b0cf6461470db99f2d6f4df13084f861fad7de9409a040191f075dcb3f148328eff419a2494cd84326749b2
   languageName: node
   linkType: hard
 
-"@jupyterlab/codemirror@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/codemirror@npm:4.1.1"
+"@jupyterlab/codemirror@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/codemirror@npm:4.2.0"
   dependencies:
-    "@codemirror/autocomplete": ^6.5.1
-    "@codemirror/commands": ^6.2.3
+    "@codemirror/autocomplete": ^6.15.0
+    "@codemirror/commands": ^6.3.3
     "@codemirror/lang-cpp": ^6.0.2
-    "@codemirror/lang-css": ^6.1.1
-    "@codemirror/lang-html": ^6.4.3
+    "@codemirror/lang-css": ^6.2.1
+    "@codemirror/lang-html": ^6.4.8
     "@codemirror/lang-java": ^6.0.1
-    "@codemirror/lang-javascript": ^6.1.7
+    "@codemirror/lang-javascript": ^6.2.2
     "@codemirror/lang-json": ^6.0.1
-    "@codemirror/lang-markdown": ^6.1.1
+    "@codemirror/lang-markdown": ^6.2.4
     "@codemirror/lang-php": ^6.0.1
-    "@codemirror/lang-python": ^6.1.3
+    "@codemirror/lang-python": ^6.1.4
     "@codemirror/lang-rust": ^6.0.1
-    "@codemirror/lang-sql": ^6.4.1
-    "@codemirror/lang-wast": ^6.0.1
-    "@codemirror/lang-xml": ^6.0.2
-    "@codemirror/language": ^6.6.0
-    "@codemirror/legacy-modes": ^6.3.2
-    "@codemirror/search": ^6.3.0
-    "@codemirror/state": ^6.2.0
-    "@codemirror/view": ^6.9.6
-    "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/codeeditor": ^4.1.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/documentsearch": ^4.1.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@lezer/common": ^1.0.2
-    "@lezer/generator": ^1.2.2
-    "@lezer/highlight": ^1.1.4
-    "@lezer/markdown": ^1.0.2
+    "@codemirror/lang-sql": ^6.6.1
+    "@codemirror/lang-wast": ^6.0.2
+    "@codemirror/lang-xml": ^6.1.0
+    "@codemirror/language": ^6.10.1
+    "@codemirror/legacy-modes": ^6.3.3
+    "@codemirror/search": ^6.5.6
+    "@codemirror/state": ^6.4.1
+    "@codemirror/view": ^6.26.0
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/codeeditor": ^4.2.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/documentsearch": ^4.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@lezer/common": ^1.2.1
+    "@lezer/generator": ^1.7.0
+    "@lezer/highlight": ^1.2.0
+    "@lezer/markdown": ^1.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     yjs: ^13.5.40
-  checksum: 453a09bab7a443c014fb84843f052f1186be5ed153415b56ecd4d1cae7c41122e7e37eeaa62348ab0c4a29711e169b3e1fbb953514b0e0fe0624eb8f3609bb0b
+  checksum: 5fa46acd267dbd2e555250256a7e7820ccf9f931dfcf6a41bf15f71ed220ac317d386d81fe7ca55eb7c6136bc4e715fe086421296eb6e8fbe992b12e4b7d1be6
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^6.0.12, @jupyterlab/coreutils@npm:^6.1.1, @jupyterlab/coreutils@npm:~6.1.1":
-  version: 6.1.1
-  resolution: "@jupyterlab/coreutils@npm:6.1.1"
+"@jupyterlab/coreutils@npm:^6.1.8, @jupyterlab/coreutils@npm:^6.2.0":
+  version: 6.2.0
+  resolution: "@jupyterlab/coreutils@npm:6.2.0"
   dependencies:
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
-  checksum: bdcd5135a1f13a7c8df1e22ad081d3da81bb7d9f802d1339baa3aaa6238099d8066ce10a3452f879069c737e471a2a55409a855398c5c211bc044c17056c9e7c
+  checksum: 1975f19f567b63484055b0d1d10757b2bf66274814083e50702bb6017af22341cc3f5924d0ec7da408feacd652120b476aaaf50286a5401f798f257e899aed91
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:~6.0.11":
-  version: 6.0.12
-  resolution: "@jupyterlab/coreutils@npm:6.0.12"
+"@jupyterlab/coreutils@npm:~6.1.1, @jupyterlab/coreutils@npm:~6.1.5":
+  version: 6.1.8
+  resolution: "@jupyterlab/coreutils@npm:6.1.8"
   dependencies:
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
-  checksum: 4a225e5e05cefe5f1cfbbfc25222553f89e866b6dca61bc3cba7ecbd759b1b0738ea2798489f41329dceedf3f5de63250554a6b2d5100cbf1c56c153e6d49672
+  checksum: 1049c78bdbffb247fe7e7be4e082fe15711ca0d8da997d6da7042e0299d7ebbf1d0341d830ae0ab451bf8dfbfc30027bf3f063fc7e35210409a7aa56fe94cee9
   languageName: node
   linkType: hard
 
-"@jupyterlab/docmanager@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/docmanager@npm:4.1.1"
+"@jupyterlab/docmanager@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/docmanager@npm:4.2.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/docregistry": ^4.1.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/statusbar": ^4.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/docregistry": ^4.2.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/statedb": ^4.2.0
+    "@jupyterlab/statusbar": ^4.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
+    "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: 835e8ce43145fb9700ea4df8e433eb7f2c24e81003d34e8085b9118d0b769bad612ccd2d2d7fb209f4baf2bccda9d2dd36063776742a810c9d81220f3a50a356
+  checksum: 63e461bf75ce4b12ada41cf727b11f956c62312b2e017fdaf9979ba16a86cb5078e7eed4f508e122afc3718d1ee18548c8ec6a1bb50f4a95a2217a77a8e0b1c3
   languageName: node
   linkType: hard
 
-"@jupyterlab/docregistry@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/docregistry@npm:4.1.1"
+"@jupyterlab/docregistry@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/docregistry@npm:4.2.0"
   dependencies:
-    "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/codeeditor": ^4.1.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/codeeditor": ^4.2.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: 8ad2e4deb280b6e95dc5f3e917d362462b018f65f4d438ad46994bef5ee9ba4350e7264455e68fb329286ac3e83aebbc63e80ca4ded0feab05974e83b73ba410
+  checksum: ef616ca11a07a5a2d8865d909499662e8c37b19e9487081682c47808becb5d87fe09a4d1c0175ea8afd3c96a255a437b8d762e990c81d71cf9cc13cf99fe3c3b
   languageName: node
   linkType: hard
 
-"@jupyterlab/documentsearch@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/documentsearch@npm:4.1.1"
+"@jupyterlab/documentsearch@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/documentsearch@npm:4.2.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
-    "@lumino/commands": ^2.2.0
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: d54976b192154dd32bc7d1794c76013d74e54ee63ffbeba51e3334d8153435d5412649a313cb5d16dced3cca749ea7bf04354f243f2c4c5f0f453e036a848f8f
+  checksum: c49919b3094390c6cefdf66c2d13baf6e7a387e087a75090cd04e65bda593bf3e9afc91307b80b851e41544ba22eae766bcacfa63480738f3f54b43f6f111c8e
   languageName: node
   linkType: hard
 
-"@jupyterlab/filebrowser@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/filebrowser@npm:4.1.1"
+"@jupyterlab/filebrowser@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/filebrowser@npm:4.2.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/docmanager": ^4.1.1
-    "@jupyterlab/docregistry": ^4.1.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/statedb": ^4.1.1
-    "@jupyterlab/statusbar": ^4.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/docmanager": ^4.2.0
+    "@jupyterlab/docregistry": ^4.2.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/statedb": ^4.2.0
+    "@jupyterlab/statusbar": ^4.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: 38a1b2650334047958eba3d51735069dc5791259e62ed34bb6cae598f6e8a300a918aa638776380e9d066b1455dd9fdeabcbeebe4d9ddd8661d10a6f824805ce
+  checksum: d80fdb55c25472cae56852c6ce8633a9899430e784ff60fbac956c17db60bc3eb92fdc5cf4e7b1c06e1fd5b7e37c3c4f9992e4ed7d4d800cd5c65eac43d5ac08
   languageName: node
   linkType: hard
 
-"@jupyterlab/lsp@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/lsp@npm:4.1.1"
+"@jupyterlab/lsp@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/lsp@npm:4.2.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/codeeditor": ^4.1.1
-    "@jupyterlab/codemirror": ^4.1.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/docregistry": ^4.1.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/translation": ^4.1.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/codeeditor": ^4.2.0
+    "@jupyterlab/codemirror": ^4.2.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/docregistry": ^4.2.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/translation": ^4.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     lodash.mergewith: ^4.6.1
     vscode-jsonrpc: ^6.0.0
     vscode-languageserver-protocol: ^3.17.0
     vscode-ws-jsonrpc: ~1.0.2
-  checksum: 55a96a0cf03b49a156bd14e9df776289be7bbd26ced685f23613c71f4a5d8d34a510c1a52956ab893e393dfb209c4c9f35df71dc0aca2b19d148e568bccb3700
+  checksum: e016ed7efb6c664eb386d6036e601fd603ad34232cb11c40c5c35fe32710cdfa55346ae33759fc1006428f6e7dcadb0a371e0907a872519cedc123779770dc67
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.12, @jupyterlab/nbformat@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/nbformat@npm:4.1.1"
+"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.1.8, @jupyterlab/nbformat@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/nbformat@npm:4.2.0"
   dependencies:
     "@lumino/coreutils": ^2.1.2
-  checksum: 8c952760e077d4b5b7c54a12e7b5a50880bdc6d4a13c4a9a5901763eaa04077b00c9a81a4c91c4a7eaafef72fb4d7a3ac1230e3fc9b91914bef27b7a8933e756
+  checksum: adecadcb63de48f09aeb54eebfed8b77ab322c478fd903001e09780a01e7cf68f93716a2598631d4426d8ad9d3dc6349e8892db12575f74c8daea33f63b9c111
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:~4.0.11":
-  version: 4.0.12
-  resolution: "@jupyterlab/nbformat@npm:4.0.12"
+"@jupyterlab/nbformat@npm:~4.1.5":
+  version: 4.1.8
+  resolution: "@jupyterlab/nbformat@npm:4.1.8"
   dependencies:
     "@lumino/coreutils": ^2.1.2
-  checksum: e9bd3385e9b7020f27577dc790462cebab3fada9571b64e57c19d9246b944726a1b3d866fec79b4be67153e2b19a1caa08d15d066274b975bfd07cd8211de605
+  checksum: 11d89ae6fb2385a00e60ab84defc61e3cf28510b029ffbe9ffe27a75bc84f85e64a0d0d16b6deb7b57256fdd651d842a0626128def511e7755121a5a0a71f078
   languageName: node
   linkType: hard
 
-"@jupyterlab/notebook@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/notebook@npm:4.1.1"
+"@jupyterlab/notebook@npm:^4.1.8":
+  version: 4.2.0
+  resolution: "@jupyterlab/notebook@npm:4.2.0"
   dependencies:
-    "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/cells": ^4.1.1
-    "@jupyterlab/codeeditor": ^4.1.1
-    "@jupyterlab/codemirror": ^4.1.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/docregistry": ^4.1.1
-    "@jupyterlab/documentsearch": ^4.1.1
-    "@jupyterlab/lsp": ^4.1.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/settingregistry": ^4.1.1
-    "@jupyterlab/statusbar": ^4.1.1
-    "@jupyterlab/toc": ^6.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/cells": ^4.2.0
+    "@jupyterlab/codeeditor": ^4.2.0
+    "@jupyterlab/codemirror": ^4.2.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/docregistry": ^4.2.0
+    "@jupyterlab/documentsearch": ^4.2.0
+    "@jupyterlab/lsp": ^4.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/settingregistry": ^4.2.0
+    "@jupyterlab/statusbar": ^4.2.0
+    "@jupyterlab/toc": ^6.2.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
+    "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: ffc0a95a794266129a341ae779d380b30abe70819ce60002e2b3bbef8a47dba8f4e55d32754f6350a715d4fa7790cece4da31b4e45714d35af84d9b3fa75244b
+  checksum: 2f4bcc4edde849a77b3a257c1920ca03dc666ec442acdf56e4e5acb4d4ff81231fc065cc753f07f91010e08f1c888f49d4813eaef6bc5b444f5d4d85dfb93f98
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^5.1.1":
-  version: 5.1.1
-  resolution: "@jupyterlab/observables@npm:5.1.1"
+"@jupyterlab/observables@npm:^5.2.0":
+  version: 5.2.0
+  resolution: "@jupyterlab/observables@npm:5.2.0"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: 611b70e274043ef86b268e406725c9f31141f6c6ce62df76e5be2ca76eee883e0b045859a8ee5541547d5e4f79941f606c9e11b4d2be5caf1156ac16a4853c32
+  checksum: 98460d55d8ac559c79be87fe5e105cc200556e87276daed739fd89e8393c74ba9b03f67c8ecf7a02e8d8ee1fd8a60031ced6c1b7884ab5f10c8bdb876f150c5f
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:~5.0.11":
-  version: 5.0.12
-  resolution: "@jupyterlab/observables@npm:5.0.12"
+"@jupyterlab/observables@npm:~5.1.5":
+  version: 5.1.8
+  resolution: "@jupyterlab/observables@npm:5.1.8"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: 49eddcdf16283977879117b99117cbdfcbd25a3f4d9e4f174a0c2d78996b9ec686e5939854f22be1e5ae4d74175f9c4d44b5bdd180993270a42acecaee6553e7
+  checksum: c349b4fea92ef28019c0b3f5a100abdd4384554188d6741234e90e03f3f18b343a22ea8560f9d2eea1a00d4cd9514074d195ec850e930785f28a2f8a624a0f4d
   languageName: node
   linkType: hard
 
-"@jupyterlab/outputarea@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/outputarea@npm:4.1.1"
+"@jupyterlab/outputarea@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/outputarea@npm:4.2.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/translation": ^4.1.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/translation": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
-  checksum: 0bcc11058a9b33e5c8f3edf1eb383f1a641410388df389aa39d11a396d390cd7ff5bcb998982a96aa149cdf32c64666268d471c73ec48c439336c66b11938e2c
+    "@lumino/widgets": ^2.3.2
+  checksum: 79403a2a27bf608a453f907c270afd0df822b398460cf5e435fcf938111201f35a1fc298a93be7e5386d5d38f9431a90a9c451f8f1255c8169d6aea7c3391163
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime-interfaces@npm:^3.9.1":
-  version: 3.9.1
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.9.1"
+"@jupyterlab/rendermime-interfaces@npm:^3.10.0":
+  version: 3.10.0
+  resolution: "@jupyterlab/rendermime-interfaces@npm:3.10.0"
   dependencies:
     "@lumino/coreutils": ^1.11.0 || ^2.1.2
-    "@lumino/widgets": ^1.37.2 || ^2.3.1
-  checksum: 5a746134a1f9f073213002bd8336327907d871599d879806994816b5fe4875c5ace3af919f1d9125e6a12f3d93f0df15b52c2fbe778b977463b621b1eb93c502
+    "@lumino/widgets": ^1.37.2 || ^2.3.2
+  checksum: 08999b64a6896a4d58869ec00ca64a1b3931e01b438d471a0ad1404407f6231667f686b823a9cb482349f3d774693368320d2d4463c23fdd1de81cb4ddf34f20
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/rendermime@npm:4.1.1"
+"@jupyterlab/rendermime@npm:^4.1.8, @jupyterlab/rendermime@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/rendermime@npm:4.2.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/translation": ^4.1.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/translation": ^4.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     lodash.escape: ^4.0.1
-  checksum: 9c23fa5714ba38956e9e94164777b3494591cd8a25e46fad4c6acef52fad30b36ab77b06bf078cc8b229fb577108561c3871a07c7ceebc35cb8ec87c12048f0f
+  checksum: 296eba0721a2900cb960fbdb99e98f82999e982f4332f6be8af7ccbb7055b9bcb1517a2b24e5c3b6759c722d5f06f9a68d6a61c8cb59c40855b7852a45aca2bd
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^7.1.1":
-  version: 7.1.1
-  resolution: "@jupyterlab/services@npm:7.1.1"
+"@jupyterlab/services@npm:^7.2.0":
+  version: 7.2.0
+  resolution: "@jupyterlab/services@npm:7.2.0"
   dependencies:
-    "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/settingregistry": ^4.1.1
-    "@jupyterlab/statedb": ^4.1.1
+    "@jupyter/ydoc": ^2.0.1
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/settingregistry": ^4.2.0
+    "@jupyterlab/statedb": ^4.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     ws: ^8.11.0
-  checksum: d2dbd3af7944f551653f2771e2c8ff87b84f42ce9bd3bf0b71bb0e6dbb422410719b8e4edeb668710211a939340f6e20cd49a137128cc4efa07ecc3fa32a66b9
+  checksum: edc93389913d792841b615cd0a317e16c77621cd5cb35e67c40f7a58bcf0e31c77718ae7abcf643621ba86ce78c795d6008a9413d84ecad2b42e39bd52db1447
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:~7.0.11":
-  version: 7.0.12
-  resolution: "@jupyterlab/services@npm:7.0.12"
+"@jupyterlab/services@npm:~7.1.5":
+  version: 7.1.8
+  resolution: "@jupyterlab/services@npm:7.1.8"
   dependencies:
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/coreutils": ^6.0.12
-    "@jupyterlab/nbformat": ^4.0.12
-    "@jupyterlab/settingregistry": ^4.0.12
-    "@jupyterlab/statedb": ^4.0.12
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/nbformat": ^4.1.8
+    "@jupyterlab/settingregistry": ^4.1.8
+    "@jupyterlab/statedb": ^4.1.8
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     ws: ^8.11.0
-  checksum: 0f50969443db19f39985524202b110bf38c4c4554d06d287d5f04758823446b879b7ed541f179c4db5f1a73184ee2790a29ebdff49820f00e1254729c223f15a
+  checksum: 56143631829ee1081f6ad2f03343a47d83549d2463f9c4bfddb34e4770c74cf78cbcc5f54aca5338a0d5ce4d28e9b8d8301e6e04b4fb7f66570c49d1ceaf19e5
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:^4.0.12, @jupyterlab/settingregistry@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/settingregistry@npm:4.1.1"
+"@jupyterlab/settingregistry@npm:^4.1.8, @jupyterlab/settingregistry@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/settingregistry@npm:4.2.0"
   dependencies:
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/statedb": ^4.1.1
-    "@lumino/commands": ^2.2.0
+    "@jupyterlab/nbformat": ^4.2.0
+    "@jupyterlab/statedb": ^4.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@rjsf/utils": ^5.13.4
     ajv: ^8.12.0
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
-  checksum: 1beddc68e8a5f01062ea856286d2e4ae2bb1993a89f71adb3a0725a191cbf2fdf927f95235b69cdfd73f848452ba40d9e7dd35ed985dd9e382c70cfbaf54cf67
+  checksum: fc60490e9e977e38b14b27a9e3896b47a28930a76a84888dd86180105b9ab6d1e68544f1184bdba72b4c5aa003cb13f10c8e5ca60685827fe6f893302483a109
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:~4.0.11":
-  version: 4.0.12
-  resolution: "@jupyterlab/settingregistry@npm:4.0.12"
+"@jupyterlab/settingregistry@npm:~4.1.5":
+  version: 4.1.8
+  resolution: "@jupyterlab/settingregistry@npm:4.1.8"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.12
-    "@jupyterlab/statedb": ^4.0.12
-    "@lumino/commands": ^2.1.3
+    "@jupyterlab/nbformat": ^4.1.8
+    "@jupyterlab/statedb": ^4.1.8
+    "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
-    "@rjsf/utils": ^5.1.0
+    "@rjsf/utils": ^5.13.4
     ajv: ^8.12.0
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
-  checksum: 1d3b425effb33333b3c89b0f4bac08ffba5fd97602ce92fb3c3037c15573c853609ec04b0e7e2d4c74f67a75360063e1fd00ba19862abc992f867a3d31e8b440
+  checksum: 90067142211fdaf6e9a6e0029fe1bc4c9ae05fa8e88e37f912373a0365bc8d507ef44e0bf83deb1e0bd0855a2cf05b0f541db38fafe3bc37d83422df8671e56a
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^4.0.12, @jupyterlab/statedb@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/statedb@npm:4.1.1"
+"@jupyterlab/statedb@npm:^4.1.8, @jupyterlab/statedb@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/statedb@npm:4.2.0"
   dependencies:
-    "@lumino/commands": ^2.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: 3291a9f10557c545b41730e657890557dbfa2b7893679ee8d406562bc62b7da3906f3691f099c9aae1bfc490cd3642552f0cbfbaed58cf58e6877e7f8ca8fd9a
+  checksum: 69620478aa7bf452d7440b9433b6411edef537cd7d9f72f87f70bd6fc0c8fc50003d02ab8d9d4b0746383f98cb7035b093ce5e596e6560e3c35c5a0fe434dce4
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:~4.0.11":
-  version: 4.0.12
-  resolution: "@jupyterlab/statedb@npm:4.0.12"
+"@jupyterlab/statedb@npm:~4.1.5":
+  version: 4.1.8
+  resolution: "@jupyterlab/statedb@npm:4.1.8"
   dependencies:
-    "@lumino/commands": ^2.1.3
+    "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: a0bc781a2c16067890ad1a7f7a774ea9b47a9db052cde756416f953aef6cb9451e057a18230b0bb91dad0c3000dbeb6d349121561050e8dc4a91478aa0d40e61
+  checksum: 28983e98affec8b8d6bb8e0cbacfe2c74d1ae48af8e69fddc7f457dcd87210adf5e39dafd21bcad24cfe572f45758c7531cd8d991e9eda894e63392b544bf09d
   languageName: node
   linkType: hard
 
-"@jupyterlab/statusbar@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/statusbar@npm:4.1.1"
+"@jupyterlab/statusbar@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/statusbar@npm:4.2.0"
   dependencies:
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: c060b1ce5c87f8277407e1fcdc0cf03bfdba496a6288c8821e19a785b5d656b454ae72fb5103cf7361a167f4eef07432c2b143883de67a54baab66444b371258
+  checksum: 1ab4bfab3d6b37f0ff93ffd8b747b90ec7e532c554c8203716931923bcd97c61ad1b34c07b9973517022f022879014b57614a27f7417996697a5c97cad814c3b
   languageName: node
   linkType: hard
 
-"@jupyterlab/testing@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/testing@npm:4.1.1"
+"@jupyterlab/testing@npm:^4.1.8":
+  version: 4.2.0
+  resolution: "@jupyterlab/testing@npm:4.2.0"
   dependencies:
     "@babel/core": ^7.10.2
     "@babel/preset-env": ^7.10.2
-    "@jupyterlab/coreutils": ^6.1.1
+    "@jupyterlab/coreutils": ^6.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/signaling": ^2.1.2
-    child_process: ~1.0.2
     deepmerge: ^4.2.2
     fs-extra: ^10.1.0
     identity-obj-proxy: ^3.0.0
     jest: ^29.2.0
     jest-environment-jsdom: ^29.3.0
     jest-junit: ^15.0.0
-    node-fetch: ^2.6.0
     simulate-event: ~1.4.0
     ts-jest: ^29.1.0
   peerDependencies:
     typescript: ">=4.3"
-  checksum: dbff63820c3a12e31163213d8b324bbc5f7a7c7f222f26f00c805384ae4ddfcd7941b459d072d3a5ab21433fe1d6c2bb7d81d35f8e15a2dd7c949abcdb3132df
+  checksum: 65ef38d488ba6cab82602d733f72e5492ba0ec9e67f8cb91d68a012e455a9abd0538962f6bfe422c4ec44954005c7da90f13851866366f45833a11107b27fb80
   languageName: node
   linkType: hard
 
 "@jupyterlab/testutils@npm:~4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/testutils@npm:4.1.1"
+  version: 4.1.8
+  resolution: "@jupyterlab/testutils@npm:4.1.8"
   dependencies:
-    "@jupyterlab/application": ^4.1.1
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/notebook": ^4.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/testing": ^4.1.1
-  checksum: 0a87fbb3f7a0901dadf151bff96f9470f7167f223b999d74c6b7e2fd4adafa40762f005db6fb61e727991e5f750d493aab6576dd6ddac1538034955a8bc81f33
+    "@jupyterlab/application": ^4.1.8
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/notebook": ^4.1.8
+    "@jupyterlab/rendermime": ^4.1.8
+    "@jupyterlab/testing": ^4.1.8
+  checksum: efabbdd60565a76cf7c17ef05ae73956f5955bbe943430c64ff9985677cadbfdc35eb79f20ea5e4ae5227fdcb397e8920a71e8b0f9b60a5c31dc6a9a4815fa11
   languageName: node
   linkType: hard
 
-"@jupyterlab/toc@npm:^6.1.1":
-  version: 6.1.1
-  resolution: "@jupyterlab/toc@npm:6.1.1"
+"@jupyterlab/toc@npm:^6.2.0":
+  version: 6.2.0
+  resolution: "@jupyterlab/toc@npm:6.2.0"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/docregistry": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/apputils": ^4.3.0
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/docregistry": ^4.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime": ^4.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/translation": ^4.2.0
+    "@jupyterlab/ui-components": ^4.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     react: ^18.2.0
-  checksum: 4affcdc2015f363e3f57da3e8613b4cff2f6e8477f308e97ce055f8ceafcab117dbb72780d2eba8dbcbba90b77affac7b8c7dd3dbc8f65db4dbc4b22629fdd4e
+  checksum: 68906012ba858d33587ce28e7a9785af4ff61cf119ed34bdfaceb48201ba56a941e2df0d722cb48f5ae2b541397fc7cea79509c388c762dccff20916d5dfdc2b
   languageName: node
   linkType: hard
 
-"@jupyterlab/translation@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/translation@npm:4.1.1"
+"@jupyterlab/translation@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/translation@npm:4.2.0"
   dependencies:
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/statedb": ^4.1.1
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/services": ^7.2.0
+    "@jupyterlab/statedb": ^4.2.0
     "@lumino/coreutils": ^2.1.2
-  checksum: adb9840f8e98af6d06d986120d542469ee349c4337e3a7f84f449535f88cc84839fe169a562447abf7bf31254bf28d1d4627684b5c521b6cb2bd21fab73e0234
+  checksum: 0b2d4d3827946bf5b12db5e98356d15dc7721279bb791a46f2927b20b49b597fd717b0d24b84ae4c7b96540f99a0eed82ba0609c186675daf80b343df9792a21
   languageName: node
   linkType: hard
 
-"@jupyterlab/ui-components@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/ui-components@npm:4.1.1"
+"@jupyterlab/ui-components@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "@jupyterlab/ui-components@npm:4.2.0"
   dependencies:
-    "@jupyter/react-components": ^0.15.2
-    "@jupyter/web-components": ^0.15.2
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/translation": ^4.1.1
+    "@jupyter/react-components": ^0.15.3
+    "@jupyter/web-components": ^0.15.3
+    "@jupyterlab/coreutils": ^6.2.0
+    "@jupyterlab/observables": ^5.2.0
+    "@jupyterlab/rendermime-interfaces": ^3.10.0
+    "@jupyterlab/translation": ^4.2.0
     "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.1
+    "@lumino/widgets": ^2.3.2
     "@rjsf/core": ^5.13.4
     "@rjsf/utils": ^5.13.4
     react: ^18.2.0
     react-dom: ^18.2.0
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
-  checksum: ac0762493671fdb146b9655b260d09de95163030a7adcbaedb41a74c67b21b72916b3a6b51e3fb54a9f1785364f5e413edd2667a9615a5d98922bdaaeb5142e4
+  checksum: 9352c9d5d4df2671999a79bcc0434c50731bc78e89b5d94cfcf1e91f55fb14dbe4670576f49b8c53f9c7bb3995e72455c9062ad6953411c188c8bb85edee0a00
   languageName: node
   linkType: hard
 
-"@jupyterlite/contents@npm:^0.2.3":
-  version: 0.2.3
-  resolution: "@jupyterlite/contents@npm:0.2.3"
+"@jupyterlite/contents@npm:^0.3.0":
+  version: 0.3.0
+  resolution: "@jupyterlite/contents@npm:0.3.0"
   dependencies:
-    "@jupyterlab/nbformat": ~4.0.11
-    "@jupyterlab/services": ~7.0.11
-    "@jupyterlite/localforage": ^0.2.3
+    "@jupyterlab/nbformat": ~4.1.5
+    "@jupyterlab/services": ~7.1.5
+    "@jupyterlite/localforage": ^0.3.0
     "@lumino/coreutils": ^2.1.2
     "@types/emscripten": ^1.39.6
     localforage: ^1.9.0
     mime: ^3.0.0
-  checksum: 7bdf110a56dc06eb5d2cd8202055c707ad49b6bd0b23e4f70bca5e160e70aa21a1e9e7b35de9729784b617b1c9df07a60e2cd2d060dbbcb1872aefb9028f9885
+  checksum: b0ca5e9b377c1a312cc04cbc9fce01355a3c956e5760f0ca5db42a520b7285e86cd386703183f3bee997a77ee7a26921b50bfed6e511a9f7f703c375863b1bd9
   languageName: node
   linkType: hard
 
 "@jupyterlite/javascript-kernel-extension@workspace:packages/javascript-kernel-extension":
   version: 0.0.0-use.local
   resolution: "@jupyterlite/javascript-kernel-extension@workspace:packages/javascript-kernel-extension"
   dependencies:
     "@jupyterlab/builder": ~4.1.1
-    "@jupyterlite/javascript-kernel": ^0.3.0-alpha.0
-    "@jupyterlite/kernel": ^0.2.1
-    "@jupyterlite/server": ^0.2.1
+    "@jupyterlite/javascript-kernel": ^0.3.0
+    "@jupyterlite/kernel": ^0.2.1  || ^0.3.0 || ^0.4.0-alpha.0
+    "@jupyterlite/server": ^0.2.1 || ^0.3.0 || ^0.4.0-alpha.0
     rimraf: ~5.0.1
     typescript: ~5.1.6
   languageName: unknown
   linkType: soft
 
 "@jupyterlite/javascript-kernel-root@workspace:.":
   version: 0.0.0-use.local
@@ -2833,120 +2855,120 @@
     eslint-plugin-prettier: ^5
     lerna: ^6.4.1
     prettier: ^3
     rimraf: ^3.0.2
   languageName: unknown
   linkType: soft
 
-"@jupyterlite/javascript-kernel@^0.3.0-alpha.0, @jupyterlite/javascript-kernel@workspace:packages/javascript-kernel":
+"@jupyterlite/javascript-kernel@^0.3.0, @jupyterlite/javascript-kernel@workspace:packages/javascript-kernel":
   version: 0.0.0-use.local
   resolution: "@jupyterlite/javascript-kernel@workspace:packages/javascript-kernel"
   dependencies:
     "@babel/core": ^7.11.6
     "@babel/preset-env": ^7.12.1
     "@jupyterlab/coreutils": ~6.1.1
     "@jupyterlab/testutils": ~4.1.1
-    "@jupyterlite/kernel": ^0.2.1
+    "@jupyterlite/kernel": ^0.2.1 || ^0.3.0 || ^0.4.0-alpha.0
     "@types/jest": ^29.5.3
     "@types/object-inspect": ^1.8.4
     comlink: ^4.3.1
     jest: ^29.6.2
     object-inspect: ^1.13.1
     rimraf: ~5.0.1
     ts-jest: ^29.1.1
     typescript: ~5.1.6
   languageName: unknown
   linkType: soft
 
-"@jupyterlite/kernel@npm:^0.2.1, @jupyterlite/kernel@npm:^0.2.3":
-  version: 0.2.3
-  resolution: "@jupyterlite/kernel@npm:0.2.3"
+"@jupyterlite/kernel@npm:^0.2.1  || ^0.3.0 || ^0.4.0-alpha.0, @jupyterlite/kernel@npm:^0.2.1 || ^0.3.0 || ^0.4.0-alpha.0, @jupyterlite/kernel@npm:^0.3.0":
+  version: 0.3.0
+  resolution: "@jupyterlite/kernel@npm:0.3.0"
   dependencies:
-    "@jupyterlab/coreutils": ~6.0.11
-    "@jupyterlab/observables": ~5.0.11
-    "@jupyterlab/services": ~7.0.11
+    "@jupyterlab/coreutils": ~6.1.5
+    "@jupyterlab/observables": ~5.1.5
+    "@jupyterlab/services": ~7.1.5
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     async-mutex: ^0.3.1
     comlink: ^4.3.1
     mock-socket: ^9.1.0
-  checksum: 206bd9e657a1ee0f2414478e3292ee803ae9dda67b1526581f992ee10e472ba13082e8dd64930fa3111ae102dd4f446944687dbd1c946e78491c56c2661c5728
+  checksum: 0c1c4e19077c910f9808b1c14bee98ae0f5af1ed86bd4b8768942fc2717a9834618693686892b3efa455e77014540522dc491d74b6dd9a2d41ad8148d275d802
   languageName: node
   linkType: hard
 
-"@jupyterlite/localforage@npm:^0.2.3":
-  version: 0.2.3
-  resolution: "@jupyterlite/localforage@npm:0.2.3"
+"@jupyterlite/localforage@npm:^0.3.0":
+  version: 0.3.0
+  resolution: "@jupyterlite/localforage@npm:0.3.0"
   dependencies:
-    "@jupyterlab/coreutils": ~6.0.11
+    "@jupyterlab/coreutils": ~6.1.5
     "@lumino/coreutils": ^2.1.2
     localforage: ^1.9.0
     localforage-memoryStorageDriver: ^0.9.2
-  checksum: 2e5f57c3a56a3c7f03244847216380aa3bf3ef540253b63268a1a24e7ac8d5df59d6038f86958da2e37641e89d2fe1ea52ecb9962efd4fde6dd7add9bd5a09ba
+  checksum: e090fe2b0ff18d230ef14e9f69c788b92432c30efeca0222d33378d8282399d86fe8ec446f7cdd29ae13ee31de8b7f2f73c1d03a5504b58c8297c17d8db8bb12
   languageName: node
   linkType: hard
 
-"@jupyterlite/server@npm:^0.2.1":
-  version: 0.2.3
-  resolution: "@jupyterlite/server@npm:0.2.3"
+"@jupyterlite/server@npm:^0.2.1 || ^0.3.0 || ^0.4.0-alpha.0":
+  version: 0.3.0
+  resolution: "@jupyterlite/server@npm:0.3.0"
   dependencies:
-    "@jupyterlab/coreutils": ~6.0.11
-    "@jupyterlab/nbformat": ~4.0.11
-    "@jupyterlab/observables": ~5.0.11
-    "@jupyterlab/services": ~7.0.11
-    "@jupyterlab/settingregistry": ~4.0.11
-    "@jupyterlab/statedb": ~4.0.11
-    "@jupyterlite/contents": ^0.2.3
-    "@jupyterlite/kernel": ^0.2.3
-    "@jupyterlite/session": ^0.2.3
-    "@jupyterlite/settings": ^0.2.3
-    "@jupyterlite/translation": ^0.2.3
+    "@jupyterlab/coreutils": ~6.1.5
+    "@jupyterlab/nbformat": ~4.1.5
+    "@jupyterlab/observables": ~5.1.5
+    "@jupyterlab/services": ~7.1.5
+    "@jupyterlab/settingregistry": ~4.1.5
+    "@jupyterlab/statedb": ~4.1.5
+    "@jupyterlite/contents": ^0.3.0
+    "@jupyterlite/kernel": ^0.3.0
+    "@jupyterlite/session": ^0.3.0
+    "@jupyterlite/settings": ^0.3.0
+    "@jupyterlite/translation": ^0.3.0
     "@lumino/application": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/signaling": ^2.1.2
     mock-socket: ^9.1.0
-  checksum: a9f2454162f42c08aa513c0e5f0d4b5f306ccc72d1402ca1d5015bcc92f56506763a345986e5f6bbe9ed724473bfef491aea2c9b518307cdc3b901b61e48a222
+  checksum: d7b738dd5eb4cfd75539241d4d8ebe279e095eea675d142a30181f4f84b381c8aab8400a986bc97d3be4c33793da715211660357782af47d4d4f9f3e10d0416a
   languageName: node
   linkType: hard
 
-"@jupyterlite/session@npm:^0.2.3":
-  version: 0.2.3
-  resolution: "@jupyterlite/session@npm:0.2.3"
+"@jupyterlite/session@npm:^0.3.0":
+  version: 0.3.0
+  resolution: "@jupyterlite/session@npm:0.3.0"
   dependencies:
-    "@jupyterlab/coreutils": ~6.0.11
-    "@jupyterlab/services": ~7.0.11
-    "@jupyterlite/kernel": ^0.2.3
+    "@jupyterlab/coreutils": ~6.1.5
+    "@jupyterlab/services": ~7.1.5
+    "@jupyterlite/kernel": ^0.3.0
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
-  checksum: c0f3e36c25f40c6cea0f861315e39795868d6e66f2f383e14f707b243af7e8ca1188e00df46f36c7f395793222d357520024f4ed357a0a56abf83d7cec807e59
+  checksum: 80e62c15b77d54f20a904aec741d602f14c87de8e6a67b54fe7d76615dfc7dbe747c79b48863441b89c7a20dc933444609d2ee21387d7b85b041bddb2eb86036
   languageName: node
   linkType: hard
 
-"@jupyterlite/settings@npm:^0.2.3":
-  version: 0.2.3
-  resolution: "@jupyterlite/settings@npm:0.2.3"
+"@jupyterlite/settings@npm:^0.3.0":
+  version: 0.3.0
+  resolution: "@jupyterlite/settings@npm:0.3.0"
   dependencies:
-    "@jupyterlab/coreutils": ~6.0.11
-    "@jupyterlab/settingregistry": ~4.0.11
-    "@jupyterlite/localforage": ^0.2.3
+    "@jupyterlab/coreutils": ~6.1.5
+    "@jupyterlab/settingregistry": ~4.1.5
+    "@jupyterlite/localforage": ^0.3.0
     "@lumino/coreutils": ^2.1.2
     json5: ^2.2.0
     localforage: ^1.9.0
-  checksum: 74ed7694318bfba1d9c2ccae7d7a1ce244a8d114eb69405effb0f07e36ccf236ccb1dbedc84470e25236ccec9bcc72d6d731a73837817acca6b90c044f2bfc9c
+  checksum: 343f88fe19cf9b24c1f518bf99d288204e922cddf584bff7424ee5ec52c2824a45b7958c3642a53126bedcc8b400289297b21f02dba5326d801f71c6b30a790e
   languageName: node
   linkType: hard
 
-"@jupyterlite/translation@npm:^0.2.3":
-  version: 0.2.3
-  resolution: "@jupyterlite/translation@npm:0.2.3"
+"@jupyterlite/translation@npm:^0.3.0":
+  version: 0.3.0
+  resolution: "@jupyterlite/translation@npm:0.3.0"
   dependencies:
-    "@jupyterlab/coreutils": ~6.0.11
+    "@jupyterlab/coreutils": ~6.1.5
     "@lumino/coreutils": ^2.1.2
-  checksum: 0c2a515512da329ff1cfcc8437e69c221f439208f3a1026ae125d8442407e08b7332594ceb26e3378b0cee6bba550d57b793d8ae6bccc4d22489ec9f3fad4ad8
+  checksum: 4ad7301f66cea0d1f82ea6a9d748321b0b3be8d238383b9aeb160427695a71a941042fddfd3d9052f19508219a250d8c59affaf76c260f5e8db095a11d5b66dc
   languageName: node
   linkType: hard
 
 "@lerna/child-process@npm:6.6.2":
   version: 6.6.2
   resolution: "@lerna/child-process@npm:6.6.2"
   dependencies:
@@ -3063,75 +3085,75 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: a319cd46fd32affc07c9432e9b2b9954becf7766be0361176c525d03474bb794cc051aad9932f48c9df33833eee1d6bfdccab12e571f2b137b4ca765c60c75de
   languageName: node
   linkType: hard
 
 "@lezer/css@npm:^1.0.0, @lezer/css@npm:^1.1.0":
-  version: 1.1.7
-  resolution: "@lezer/css@npm:1.1.7"
+  version: 1.1.8
+  resolution: "@lezer/css@npm:1.1.8"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 7760d294fd0b1ac6db319c4990517c1ed9027d6757de537553624238056df6e1ef1b6a571a023a4bce3d7a2b891036d9f85f76f2109f503bea94837f90c64bc2
+  checksum: 1f5968360dbac7ba27f0c2a194143769f7b01824715274dd8507dacf13cc790bb8c48ce95de355e9c58be93bb3e271bf98b9fc51213f79e4ce918e7c7ebbef04
   languageName: node
   linkType: hard
 
-"@lezer/generator@npm:^1.2.2":
-  version: 1.6.0
-  resolution: "@lezer/generator@npm:1.6.0"
+"@lezer/generator@npm:^1.7.0":
+  version: 1.7.0
+  resolution: "@lezer/generator@npm:1.7.0"
   dependencies:
     "@lezer/common": ^1.1.0
     "@lezer/lr": ^1.3.0
   bin:
     lezer-generator: src/lezer-generator.cjs
-  checksum: dfbf19d0533922272ac00c4b7884e1df88e2a35dd758e4544ceb5d784aa38d5751add03ca87f35d14cc39416e0dbc06ccaf2a211a6ae982e00daaaffe9c9320c
+  checksum: 69f4c6625446cb65adaa509480ec67502f27651707a8e45e99373e682d7f66f8842205669f174bcb138eade72c64ded0b54d6de6aa5af995ac1f1e805ef021fd
   languageName: node
   linkType: hard
 
-"@lezer/highlight@npm:^1.0.0, @lezer/highlight@npm:^1.1.3, @lezer/highlight@npm:^1.1.4":
+"@lezer/highlight@npm:^1.0.0, @lezer/highlight@npm:^1.1.3, @lezer/highlight@npm:^1.2.0":
   version: 1.2.0
   resolution: "@lezer/highlight@npm:1.2.0"
   dependencies:
     "@lezer/common": ^1.0.0
   checksum: 5b9dfe741f95db13f6124cb9556a43011cb8041ecf490be98d44a86b04d926a66e912bcd3a766f6a3d79e064410f1a2f60ab240b50b645a12c56987bf4870086
   languageName: node
   linkType: hard
 
 "@lezer/html@npm:^1.3.0":
-  version: 1.3.8
-  resolution: "@lezer/html@npm:1.3.8"
+  version: 1.3.9
+  resolution: "@lezer/html@npm:1.3.9"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 06bce804487435ea6ccb39595176bb65d68691f082b0b68fb7d22d90d4de9798a8202f16e9aefe22865db15257a37f6fca93275d660715eea98f7578579e7135
+  checksum: 40d89b0af4379768ce7d3e7162988e9ec73b42984e333e877c7451f7e2c10131e39e4b50150bc334093cbd84a3b34f9fc1a6ac62cbba51f503a495ad243e880b
   languageName: node
   linkType: hard
 
 "@lezer/java@npm:^1.0.0":
-  version: 1.1.1
-  resolution: "@lezer/java@npm:1.1.1"
+  version: 1.1.2
+  resolution: "@lezer/java@npm:1.1.2"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 8a071aca6b5e1ed1d22bffed22bbd29f21b102b7337a7ea5c956eb259e6ff20eee2d6e85b7dadff69859cb6615d6b1a3f0ba109673e87ce5a1f6cabdeee626fd
+  checksum: 752e8c9b99cccf022669a702016e0c3a793d8326e043b1d053159f5de4d222cd188e8e31e1427cbe6a8ed8e53de3977ab551c64cbd5a76a12eb3a1da5e18b6a5
   languageName: node
   linkType: hard
 
 "@lezer/javascript@npm:^1.0.0":
-  version: 1.4.13
-  resolution: "@lezer/javascript@npm:1.4.13"
+  version: 1.4.16
+  resolution: "@lezer/javascript@npm:1.4.16"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.1.3
     "@lezer/lr": ^1.3.0
-  checksum: a5e4607fec7671dff66d1f3bfee5a5da7395982f1867e17ac4d8f2d8f223451fb18516ef2699340b148af112176a07e1fcba9e63c5f8397c12895dd0509113d6
+  checksum: 20fcf5ad95d3cf0155af8a060045d1c14609e1178669e087f246854d1ef7e7326e512cc05f90db1bcbd58ce229fcc7aa8600c7f757580c5f980c420835a2cd3c
   languageName: node
   linkType: hard
 
 "@lezer/json@npm:^1.0.0":
   version: 1.0.2
   resolution: "@lezer/json@npm:1.0.2"
   dependencies:
@@ -3147,21 +3169,21 @@
   resolution: "@lezer/lr@npm:1.4.0"
   dependencies:
     "@lezer/common": ^1.0.0
   checksum: 4c8517017e9803415c6c5cb8230d8764107eafd7d0b847676cd1023abb863a4b268d0d01c7ce3cf1702c4749527c68f0a26b07c329cb7b68c36ed88362d7b193
   languageName: node
   linkType: hard
 
-"@lezer/markdown@npm:^1.0.0, @lezer/markdown@npm:^1.0.2":
-  version: 1.2.0
-  resolution: "@lezer/markdown@npm:1.2.0"
+"@lezer/markdown@npm:^1.0.0, @lezer/markdown@npm:^1.2.0":
+  version: 1.3.0
+  resolution: "@lezer/markdown@npm:1.3.0"
   dependencies:
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
-  checksum: e6355272ad98c97b339dd42d8d9b78fa4f48fdcc5c9c408720936cacb7d2bcd47b0cedf8e0997ef93539c2b03a65326fc59372e54f0b24acd98630e06869a350
+  checksum: 13eb2720e4cb84278349bad8af116f748813094f99fad02680010c3a8c5985e0358c344487990f87a31ef0d6c1a2be582301f914c0e4a6e9cfa22647b6cd6545
   languageName: node
   linkType: hard
 
 "@lezer/php@npm:^1.0.0":
   version: 1.0.2
   resolution: "@lezer/php@npm:1.0.2"
   dependencies:
@@ -3169,21 +3191,21 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.1.0
   checksum: c85ef18571d37826b687dd141a0fe110f5814adaf9d1a391e7e482020d7f81df189ca89ec0dd141c1433d48eff4c6e53648b46f008dea8ad2dc574f35f1d4d79
   languageName: node
   linkType: hard
 
 "@lezer/python@npm:^1.1.4":
-  version: 1.1.11
-  resolution: "@lezer/python@npm:1.1.11"
+  version: 1.1.13
+  resolution: "@lezer/python@npm:1.1.13"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: ed0e58317716967644f57bf29eb902c0c205b909bc035c0960520222a79bd6525468c8adfb7d824787a8a29ec7a1c7d2da5fd59f912cdeff2830c71958b9576d
+  checksum: 43465f3289063e16caac9a109f61b8f810dd6a0e1043874df1b4d0f1cee5fba39cfd8c78fa2e507c0aa8f50cee8c48fe36df549ac1f959dae8d51c06e8ec0d0b
   languageName: node
   linkType: hard
 
 "@lezer/rust@npm:^1.0.0":
   version: 1.0.2
   resolution: "@lezer/rust@npm:1.0.2"
   dependencies:
@@ -3191,63 +3213,63 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: fc5e97852b42beeb44a0ebe316dc64e3cc49ff481c22e3e67d6003fc4a5c257fcd94959cfcc76cd154fa172db9b3b4b28de5c09f10550d6e5f14869ddc274e5b
   languageName: node
   linkType: hard
 
 "@lezer/xml@npm:^1.0.0":
-  version: 1.0.4
-  resolution: "@lezer/xml@npm:1.0.4"
+  version: 1.0.5
+  resolution: "@lezer/xml@npm:1.0.5"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 68a82085bff6c1525f4ef03cd9f9dac0132b3e03fe574e0289700dd4475056e40e8744cde15cf5ad6d3760d0d584ff85ce707e26a7c938d0c5fe2e325c1c336e
+  checksum: a0a077b9e455b03593b93a7fdff2a4eab2cb7b230c8e1b878a8bebe80184632b9cc75ca018f1f9e2acb3a26e1386f4777385ab6e87aea70ccf479cde5ca268ee
   languageName: node
   linkType: hard
 
 "@lumino/algorithm@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/algorithm@npm:2.0.1"
   checksum: cbf7fcf6ee6b785ea502cdfddc53d61f9d353dcb9659343511d5cd4b4030be2ff2ca4c08daec42f84417ab0318a3d9972a17319fa5231693e109ab112dcf8000
   languageName: node
   linkType: hard
 
-"@lumino/application@npm:^2.3.0":
-  version: 2.3.0
-  resolution: "@lumino/application@npm:2.3.0"
+"@lumino/application@npm:^2.3.0, @lumino/application@npm:^2.3.1":
+  version: 2.3.1
+  resolution: "@lumino/application@npm:2.3.1"
   dependencies:
-    "@lumino/commands": ^2.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
-    "@lumino/widgets": ^2.3.1
-  checksum: 9d1eb5bc972ed158bf219604a53bbac1262059bc5b0123d3e041974486b9cbb8288abeeec916f3b62f62d7c32e716cccf8b73e4832ae927e4f9dd4e4b0cd37ed
+    "@lumino/widgets": ^2.3.2
+  checksum: c112789d99baf62e5c2cee98834bc3efb5027bbca1aac81f10ea8855c0cd2538ec0a7c56c3f5dd42dce244e6892ef5bf8ef356f97e1cd4c161b99eb2068c195c
   languageName: node
   linkType: hard
 
 "@lumino/collections@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/collections@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
   checksum: 8a29b7973a388a33c5beda0819dcd2dc2aad51a8406dcfd4581b055a9f77a39dc5800f7a8b4ae3c0bb97ae7b56a7a869e2560ffb7a920a28e93b477ba05907d6
   languageName: node
   linkType: hard
 
-"@lumino/commands@npm:^2.1.3, @lumino/commands@npm:^2.2.0":
-  version: 2.2.0
-  resolution: "@lumino/commands@npm:2.2.0"
+"@lumino/commands@npm:^2.2.0, @lumino/commands@npm:^2.3.0":
+  version: 2.3.0
+  resolution: "@lumino/commands@npm:2.3.0"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/keyboard": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-  checksum: 093e9715491e5cef24bc80665d64841417b400f2fa595f9b60832a3b6340c405c94a6aa276911944a2c46d79a6229f3cc087b73f50852bba25ece805abd0fae9
+  checksum: a9b83bbfcc0421ff501e818dd234c65db438a8abb450628db0dea9ee05e8077d10b2275e7e2289f6df9c20dc26d2af458b1db88ccf43ec69f185eb207dbad419
   languageName: node
   linkType: hard
 
 "@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.1.2, @lumino/coreutils@npm:^2.1.2":
   version: 2.1.2
   resolution: "@lumino/coreutils@npm:2.1.2"
   checksum: 7865317ac0676b448d108eb57ab5d8b2a17c101995c0f7a7106662d9fe6c859570104525f83ee3cda12ae2e326803372206d6f4c1f415a5b59e4158a7b81066f
@@ -3330,68 +3352,68 @@
   resolution: "@lumino/virtualdom@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
   checksum: cf59b6f15b430e13e9e657b7a0619b9056cd9ea7b2a87f407391d071c501b77403c302b6a66dca510382045e75b2e3fe551630bb391f1c6b33678057d4bec164
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^1.37.2 || ^2.3.1, @lumino/widgets@npm:^2.3.1":
-  version: 2.3.1
-  resolution: "@lumino/widgets@npm:2.3.1"
+"@lumino/widgets@npm:^1.37.2 || ^2.3.2, @lumino/widgets@npm:^2.3.1, @lumino/widgets@npm:^2.3.2":
+  version: 2.3.2
+  resolution: "@lumino/widgets@npm:2.3.2"
   dependencies:
     "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/keyboard": ^2.0.1
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-  checksum: ba7b8f8839c1cd2a41dbda13281094eb6981a270cccf4f25a0cf83686dcc526a2d8044a20204317630bb7dd4a04d65361408c7623a921549c781afca84b91c67
+  checksum: 954fe066b0826cf00c019731bb3f70e635c63be4a0ce27f7573dbe6bd59e2154f511594b50e8f58f44877cf514084128c1e894ecbbbfd6e20d937e5cfb69ca8b
   languageName: node
   linkType: hard
 
 "@microsoft/fast-colors@npm:^5.3.1":
   version: 5.3.1
   resolution: "@microsoft/fast-colors@npm:5.3.1"
   checksum: ff87f402faadb4b5aeee3d27762566c11807f927cd4012b8bbc7f073ca68de0e2197f95330ff5dfd7038f4b4f0e2f51b11feb64c5d570f5c598d37850a5daf60
   languageName: node
   linkType: hard
 
-"@microsoft/fast-element@npm:^1.12.0":
-  version: 1.12.0
-  resolution: "@microsoft/fast-element@npm:1.12.0"
-  checksum: bbff4e9c83106d1d74f3eeedc87bf84832429e78fee59c6a4ae8164ee4f42667503f586896bea72341b4d2c76c244a3cb0d4fd0d5d3732755f00357714dd609e
+"@microsoft/fast-element@npm:^1.12.0, @microsoft/fast-element@npm:^1.13.0":
+  version: 1.13.0
+  resolution: "@microsoft/fast-element@npm:1.13.0"
+  checksum: 1cb7b4cfb7531116a3542d3f59bf1dd35106194f5764205403590250aaff744de79e35a5a1f36b4941c4eda9edc088148d4d629fb80be15fdf25f6be01770f3a
   languageName: node
   linkType: hard
 
-"@microsoft/fast-foundation@npm:^2.49.4, @microsoft/fast-foundation@npm:^2.49.5":
-  version: 2.49.5
-  resolution: "@microsoft/fast-foundation@npm:2.49.5"
+"@microsoft/fast-foundation@npm:^2.49.4, @microsoft/fast-foundation@npm:^2.49.6":
+  version: 2.49.6
+  resolution: "@microsoft/fast-foundation@npm:2.49.6"
   dependencies:
-    "@microsoft/fast-element": ^1.12.0
+    "@microsoft/fast-element": ^1.13.0
     "@microsoft/fast-web-utilities": ^5.4.1
     tabbable: ^5.2.0
     tslib: ^1.13.0
-  checksum: 8a4729e8193ee93f780dc88fac26561b42f2636e3f0a8e89bb1dfe256f50a01a21ed1d8e4d31ce40678807dc833e25f31ba735cb5d3c247b65219aeb2560c82c
+  checksum: 15fdf9dd0b910a72a9cff140f765d522304df11f8a78d5a97a815e2bbae25027c2b336e94f89ca31e650d6aabe17b590b7453acc0d2cb7340c219eb76350a942
   languageName: node
   linkType: hard
 
 "@microsoft/fast-react-wrapper@npm:^0.3.22":
-  version: 0.3.23
-  resolution: "@microsoft/fast-react-wrapper@npm:0.3.23"
+  version: 0.3.24
+  resolution: "@microsoft/fast-react-wrapper@npm:0.3.24"
   dependencies:
-    "@microsoft/fast-element": ^1.12.0
-    "@microsoft/fast-foundation": ^2.49.5
+    "@microsoft/fast-element": ^1.13.0
+    "@microsoft/fast-foundation": ^2.49.6
   peerDependencies:
     react: ">=16.9.0"
-  checksum: 45885e1868916d2aa9059e99c341c97da434331d9340a57128d4218081df68b5e1107031c608db9a550d6d1c3b010d516ed4f8dc5a8a2470058da6750dcd204a
+  checksum: 1d7a87509c22872bafc9b5c64f66659e52ba0cfdff484d7204125e503dafdea143f5e1bd2a643e2f3fbba6cc7567d916393369433f19dab9f0adcbe7a88b7d98
   languageName: node
   linkType: hard
 
 "@microsoft/fast-web-utilities@npm:^5.4.1":
   version: 5.4.1
   resolution: "@microsoft/fast-web-utilities@npm:5.4.1"
   dependencies:
@@ -3424,23 +3446,23 @@
     "@nodelib/fs.scandir": 2.1.5
     fastq: ^1.6.0
   checksum: 190c643f156d8f8f277bf2a6078af1ffde1fd43f498f187c2db24d35b4b4b5785c02c7dc52e356497b9a1b65b13edc996de08de0b961c32844364da02986dc53
   languageName: node
   linkType: hard
 
 "@npmcli/agent@npm:^2.0.0":
-  version: 2.2.1
-  resolution: "@npmcli/agent@npm:2.2.1"
+  version: 2.2.2
+  resolution: "@npmcli/agent@npm:2.2.2"
   dependencies:
     agent-base: ^7.1.0
     http-proxy-agent: ^7.0.0
     https-proxy-agent: ^7.0.1
     lru-cache: ^10.0.1
-    socks-proxy-agent: ^8.0.1
-  checksum: c69aca42dbba393f517bc5777ee872d38dc98ea0e5e93c1f6d62b82b8fecdc177a57ea045f07dda1a770c592384b2dd92a5e79e21e2a7cf51c9159466a8f9c9b
+    socks-proxy-agent: ^8.0.3
+  checksum: 67de7b88cc627a79743c88bab35e023e23daf13831a8aa4e15f998b92f5507b644d8ffc3788afc8e64423c612e0785a6a92b74782ce368f49a6746084b50d874
   languageName: node
   linkType: hard
 
 "@npmcli/arborist@npm:6.2.3":
   version: 6.2.3
   resolution: "@npmcli/arborist@npm:6.2.3"
   dependencies:
@@ -3490,19 +3512,19 @@
     "@gar/promisify": ^1.1.3
     semver: ^7.3.5
   checksum: 405074965e72d4c9d728931b64d2d38e6ea12066d4fad651ac253d175e413c06fe4350970c783db0d749181da8fe49c42d3880bd1cbc12cd68e3a7964d820225
   languageName: node
   linkType: hard
 
 "@npmcli/fs@npm:^3.1.0":
-  version: 3.1.0
-  resolution: "@npmcli/fs@npm:3.1.0"
+  version: 3.1.1
+  resolution: "@npmcli/fs@npm:3.1.1"
   dependencies:
     semver: ^7.3.5
-  checksum: a50a6818de5fc557d0b0e6f50ec780a7a02ab8ad07e5ac8b16bf519e0ad60a144ac64f97d05c443c3367235d337182e1d012bbac0eb8dbae8dc7b40b193efd0e
+  checksum: d960cab4b93adcb31ce223bfb75c5714edbd55747342efb67dcc2f25e023d930a7af6ece3e75f2f459b6f38fc14d031c766f116cd124fdc937fd33112579e820
   languageName: node
   linkType: hard
 
 "@npmcli/git@npm:^4.0.0, @npmcli/git@npm:^4.1.0":
   version: 4.1.0
   resolution: "@npmcli/git@npm:4.1.0"
   dependencies:
@@ -3515,34 +3537,34 @@
     semver: ^7.3.5
     which: ^3.0.0
   checksum: 37efb926593f294eb263297cdfffec9141234f977b89a7a6b95ff7a72576c1d7f053f4961bc4b5e79dea6476fe08e0f3c1ed9e4aeb84169e357ff757a6a70073
   languageName: node
   linkType: hard
 
 "@npmcli/installed-package-contents@npm:^2.0.0, @npmcli/installed-package-contents@npm:^2.0.1":
-  version: 2.0.2
-  resolution: "@npmcli/installed-package-contents@npm:2.0.2"
+  version: 2.1.0
+  resolution: "@npmcli/installed-package-contents@npm:2.1.0"
   dependencies:
     npm-bundled: ^3.0.0
     npm-normalize-package-bin: ^3.0.0
   bin:
-    installed-package-contents: lib/index.js
-  checksum: 60789d5ed209ee5df479232f62d9d38ecec36e95701cae88320b828b8651351b32d7b47d16d4c36cc7ce5000db4bf1f3e6981bed6381bdc5687ff4bc0795682d
+    installed-package-contents: bin/index.js
+  checksum: d0f307e0c971a4ffaea44d4f38d53b57e19222413f338bab26d4321c4a7b9098318d74719dd1f8747a6de0575ac0ba29aeb388edf6599ac8299506947f53ffb6
   languageName: node
   linkType: hard
 
 "@npmcli/map-workspaces@npm:^3.0.2":
-  version: 3.0.4
-  resolution: "@npmcli/map-workspaces@npm:3.0.4"
+  version: 3.0.6
+  resolution: "@npmcli/map-workspaces@npm:3.0.6"
   dependencies:
     "@npmcli/name-from-folder": ^2.0.0
     glob: ^10.2.2
     minimatch: ^9.0.0
     read-package-json-fast: ^3.0.0
-  checksum: 99607dbc502b16d0ce7a47a81ccc496b3f5ed10df4e61e61a505929de12c356092996044174ae0cfd6d8cc177ef3b597eef4987b674fc0c5a306d3a8cc1fe91a
+  checksum: bdb09ee1d044bb9b2857d9e2d7ca82f40783a8549b5a7e150e25f874ee354cdbc8109ad7c3df42ec412f7057d95baa05920c4d361c868a93a42146b8e4390d3d
   languageName: node
   linkType: hard
 
 "@npmcli/metavuln-calculator@npm:^5.0.0":
   version: 5.0.1
   resolution: "@npmcli/metavuln-calculator@npm:5.0.1"
   dependencies:
@@ -3614,19 +3636,19 @@
   dependencies:
     which: ^3.0.0
   checksum: aa725780c13e1f97ab32ed7bcb5a207a3fb988e1d7ecdc3d22a549a22c8034740366b351c4dde4b011bcffcd8c4a7be6083d9cf7bc7e897b88837150de018528
   languageName: node
   linkType: hard
 
 "@npmcli/query@npm:^3.0.0":
-  version: 3.0.1
-  resolution: "@npmcli/query@npm:3.0.1"
+  version: 3.1.0
+  resolution: "@npmcli/query@npm:3.1.0"
   dependencies:
     postcss-selector-parser: ^6.0.10
-  checksum: b169b9c9a37c5a6e68d61604c7e3175ebdefbc3a77a8981326eaa8fa89cf4044fc6a87bd0fdbe5d096eda2f765aff1477924b55f4e23f64b3143dd1d9004eead
+  checksum: 33c018bfcc6d64593e7969847d0442beab4e8a42b6c9f932237c9fd135c95ab55de5c4b5d5d66302dd9fc3c748bc4ead780d3595e5d586fedf9859ed6b5f2744
   languageName: node
   linkType: hard
 
 "@npmcli/run-script@npm:4.1.7":
   version: 4.1.7
   resolution: "@npmcli/run-script@npm:4.1.7"
   dependencies:
@@ -3940,41 +3962,41 @@
   version: 0.1.1
   resolution: "@pkgr/core@npm:0.1.1"
   checksum: 6f25fd2e3008f259c77207ac9915b02f1628420403b2630c92a07ff963129238c9262afc9e84344c7a23b5cc1f3965e2cd17e3798219f5fd78a63d144d3cceba
   languageName: node
   linkType: hard
 
 "@rjsf/core@npm:^5.13.4":
-  version: 5.17.0
-  resolution: "@rjsf/core@npm:5.17.0"
+  version: 5.18.4
+  resolution: "@rjsf/core@npm:5.18.4"
   dependencies:
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     markdown-to-jsx: ^7.4.1
     nanoid: ^3.3.7
     prop-types: ^15.8.1
   peerDependencies:
-    "@rjsf/utils": ^5.16.x
+    "@rjsf/utils": ^5.18.x
     react: ^16.14.0 || >=17
-  checksum: adfcbd1d44cef5f9e5de2873096085abd03b146dcef2c9c226060341ce2c935b5399e4ad5f00ad5091394224f5859bd6ac9bac533537dc5c8e2edb16b52b67cf
+  checksum: 8c3f49914be396595ce67dc4c36ac25c5cb6673917ec82c47f79321f5bb78d02741e8dca39287d0435270e7c9ccb06f7d40e396bdf71a3e9eb1371ef16954817
   languageName: node
   linkType: hard
 
-"@rjsf/utils@npm:^5.1.0, @rjsf/utils@npm:^5.13.4":
-  version: 5.17.0
-  resolution: "@rjsf/utils@npm:5.17.0"
+"@rjsf/utils@npm:^5.13.4":
+  version: 5.18.4
+  resolution: "@rjsf/utils@npm:5.18.4"
   dependencies:
     json-schema-merge-allof: ^0.8.1
     jsonpointer: ^5.0.1
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
-  checksum: 01d0001f83083764a8552e009aa7df084621df9d1fc6ccdfad9d534513084421b1ad7494cab77b9b8205d680fd915f612d87800e20ab242e7066f33184c73d4f
+  checksum: d7cf514527ec50a94751c5ec1f9e5eafd89d0c56441a22ae28a4e667aaa7c60447e1e1ccf8355c5be5b97e9a1163853c116816b13307e3463433d50f6b89bb3e
   languageName: node
   linkType: hard
 
 "@sigstore/bundle@npm:^1.1.0":
   version: 1.1.0
   resolution: "@sigstore/bundle@npm:1.1.0"
   dependencies:
@@ -4098,37 +4120,37 @@
   dependencies:
     "@babel/types": ^7.20.7
   checksum: 608e0ab4fc31cd47011d98942e6241b34d461608c0c0e153377c5fd822c436c475f1ded76a56bfa76a1adf8d9266b727bbf9bfac90c4cb152c97f30dadc5b7e8
   languageName: node
   linkType: hard
 
 "@types/emscripten@npm:^1.39.6":
-  version: 1.39.10
-  resolution: "@types/emscripten@npm:1.39.10"
-  checksum: 1721da76593f9194e0b7c90a581e2d31c23bd4eb28f93030cd1dc58216cdf1e692c045274f2eedaed29c652c25c9a4dff2e503b11bd1258d07095c009a1956b1
+  version: 1.39.12
+  resolution: "@types/emscripten@npm:1.39.12"
+  checksum: 31fe4c20c0fa543f6f1d0a8218008eeeb167f9f817237a0e6c458a3e7ea4e12d7af128c3075e51ba231fe897fcd28fabec5773ac29597011de42767d69ecf757
   languageName: node
   linkType: hard
 
 "@types/eslint-scope@npm:^3.7.3":
   version: 3.7.7
   resolution: "@types/eslint-scope@npm:3.7.7"
   dependencies:
     "@types/eslint": "*"
     "@types/estree": "*"
   checksum: e2889a124aaab0b89af1bab5959847c5bec09809209255de0e63b9f54c629a94781daa04adb66bffcdd742f5e25a17614fb933965093c0eea64aacda4309380e
   languageName: node
   linkType: hard
 
 "@types/eslint@npm:*":
-  version: 8.56.2
-  resolution: "@types/eslint@npm:8.56.2"
+  version: 8.56.10
+  resolution: "@types/eslint@npm:8.56.10"
   dependencies:
     "@types/estree": "*"
     "@types/json-schema": "*"
-  checksum: 38e054971596f5c0413f66a62dc26b10e0a21ac46ceacb06fbf8cfb838d20820787209b17218b3916e4c23d990ff77cfdb482d655cac0e0d2b837d430fcc5db8
+  checksum: fb7137dd263ce1130b42d14452bdd0266ef81f52cb55ba1a5e9750e65da1f0596dc598c88bffc7e415458b6cb611a876dcc132bcf40ea48701c6d05b40c57be5
   languageName: node
   linkType: hard
 
 "@types/estree@npm:*, @types/estree@npm:^1.0.5":
   version: 1.0.5
   resolution: "@types/estree@npm:1.0.5"
   checksum: dd8b5bed28e6213b7acd0fb665a84e693554d850b0df423ac8076cc3ad5823a6bc26b0251d080bdc545af83179ede51dd3f6fa78cad2c46ed1f29624ddf3e41a
@@ -4208,72 +4230,64 @@
   version: 1.2.5
   resolution: "@types/minimist@npm:1.2.5"
   checksum: 477047b606005058ab0263c4f58097136268007f320003c348794f74adedc3166ffc47c80ec3e94687787f2ab7f4e72c468223946e79892cf0fd9e25e9970a90
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 20.11.18
-  resolution: "@types/node@npm:20.11.18"
+  version: 20.12.12
+  resolution: "@types/node@npm:20.12.12"
   dependencies:
     undici-types: ~5.26.4
-  checksum: b34fb342152b5a5b486e9d54d62003f6ca18e2f0f1682c8c4a3d6388e9456dab310775cbdc8302a7945fb72a42ff283b770f8fb6ca5120f77b9b3b7de40c9760
+  checksum: 5373983874b9af7c216e7ca5d26b32a8d9829c703a69f1e66f2113598b5be8582c0e009ca97369f1ec9a6282b3f92812208d06eb1e9fc3bd9b939b022303d042
   languageName: node
   linkType: hard
 
 "@types/normalize-package-data@npm:^2.4.0":
   version: 2.4.4
   resolution: "@types/normalize-package-data@npm:2.4.4"
   checksum: 65dff72b543997b7be8b0265eca7ace0e34b75c3e5fee31de11179d08fa7124a7a5587265d53d0409532ecb7f7fba662c2012807963e1f9b059653ec2c83ee05
   languageName: node
   linkType: hard
 
 "@types/object-inspect@npm:^1.8.4":
-  version: 1.8.4
-  resolution: "@types/object-inspect@npm:1.8.4"
-  checksum: 06e1993607285603c619e6f8402effb8d3a7a797fc857a96f9d8200eb31e0e2017d26efc82b0a5e40ae82f6da5caa824edc4dff798afb63dbfaa8a029cd3b4ad
+  version: 1.13.0
+  resolution: "@types/object-inspect@npm:1.13.0"
+  checksum: 8caf52c815947540b5246e0b5b2d455a2183791fe9427537eab8a40b465392400cee6ce50beaeb35465e167e9cb405ccfde90eb5317ee2c9df85af7508f0a320
   languageName: node
   linkType: hard
 
 "@types/parse-json@npm:^4.0.0":
   version: 4.0.2
   resolution: "@types/parse-json@npm:4.0.2"
   checksum: 5bf62eec37c332ad10059252fc0dab7e7da730764869c980b0714777ad3d065e490627be9f40fc52f238ffa3ac4199b19de4127196910576c2fe34dd47c7a470
   languageName: node
   linkType: hard
 
 "@types/prop-types@npm:*":
-  version: 15.7.11
-  resolution: "@types/prop-types@npm:15.7.11"
-  checksum: 7519ff11d06fbf6b275029fe03fff9ec377b4cb6e864cac34d87d7146c7f5a7560fd164bdc1d2dbe00b60c43713631251af1fd3d34d46c69cd354602bc0c7c54
+  version: 15.7.12
+  resolution: "@types/prop-types@npm:15.7.12"
+  checksum: ac16cc3d0a84431ffa5cfdf89579ad1e2269549f32ce0c769321fdd078f84db4fbe1b461ed5a1a496caf09e637c0e367d600c541435716a55b1d9713f5035dfe
   languageName: node
   linkType: hard
 
 "@types/react@npm:^18.0.26":
-  version: 18.2.55
-  resolution: "@types/react@npm:18.2.55"
+  version: 18.3.2
+  resolution: "@types/react@npm:18.3.2"
   dependencies:
     "@types/prop-types": "*"
-    "@types/scheduler": "*"
     csstype: ^3.0.2
-  checksum: a8eb4fa77f73831b9112d4f11a7006217dc0740361649b9b0da3fd441d151a9cd415d5d68b91c0af4e430e063424d301c77489e5edaddc9f711c4e46cf9818a5
-  languageName: node
-  linkType: hard
-
-"@types/scheduler@npm:*":
-  version: 0.16.8
-  resolution: "@types/scheduler@npm:0.16.8"
-  checksum: 6c091b096daa490093bf30dd7947cd28e5b2cd612ec93448432b33f724b162587fed9309a0acc104d97b69b1d49a0f3fc755a62282054d62975d53d7fd13472d
+  checksum: d0b8b9d0ede6cd28dbbe34106d914b5e3652d9d7aa9d0f32fe6171506b6fc7c826d9d6571642976a5422bd29c5022fd893a710ed59a1177a0c1df8e02cf17ffe
   languageName: node
   linkType: hard
 
 "@types/semver@npm:^7.5.0":
-  version: 7.5.7
-  resolution: "@types/semver@npm:7.5.7"
-  checksum: 5af9b13e3d74d86d4b618f6506ccbded801fb35dbc28608cd5a7bfb8bcac0021dd35ef305a72a0c2a8def0cff60acd706bfee16a9ed1c39a893d2a175e778ea7
+  version: 7.5.8
+  resolution: "@types/semver@npm:7.5.8"
+  checksum: ea6f5276f5b84c55921785a3a27a3cd37afee0111dfe2bcb3e03c31819c197c782598f17f0b150a69d453c9584cd14c4c4d7b9a55d2c5e6cacd4d66fdb3b3663
   languageName: node
   linkType: hard
 
 "@types/source-list-map@npm:*":
   version: 0.1.6
   resolution: "@types/source-list-map@npm:0.1.6"
   checksum: 9cd294c121f1562062de5d241fe4d10780b1131b01c57434845fe50968e9dcf67ede444591c2b1ad6d3f9b6bc646ac02cc8f51a3577c795f9c64cf4573dcc6b1
@@ -4447,21 +4461,21 @@
 "@ungap/structured-clone@npm:^1.2.0":
   version: 1.2.0
   resolution: "@ungap/structured-clone@npm:1.2.0"
   checksum: 4f656b7b4672f2ce6e272f2427d8b0824ed11546a601d8d5412b9d7704e83db38a8d9f402ecdf2b9063fc164af842ad0ec4a55819f621ed7e7ea4d1efcc74524
   languageName: node
   linkType: hard
 
-"@webassemblyjs/ast@npm:1.11.6, @webassemblyjs/ast@npm:^1.11.5":
-  version: 1.11.6
-  resolution: "@webassemblyjs/ast@npm:1.11.6"
+"@webassemblyjs/ast@npm:1.12.1, @webassemblyjs/ast@npm:^1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/ast@npm:1.12.1"
   dependencies:
     "@webassemblyjs/helper-numbers": 1.11.6
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
-  checksum: 38ef1b526ca47c210f30975b06df2faf1a8170b1636ce239fc5738fc231ce28389dd61ecedd1bacfc03cbe95b16d1af848c805652080cb60982836eb4ed2c6cf
+  checksum: 31bcc64147236bd7b1b6d29d1f419c1f5845c785e1e42dc9e3f8ca2e05a029e9393a271b84f3a5bff2a32d35f51ff59e2181a6e5f953fe88576acd6750506202
   languageName: node
   linkType: hard
 
 "@webassemblyjs/floating-point-hex-parser@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/floating-point-hex-parser@npm:1.11.6"
   checksum: 29b08758841fd8b299c7152eda36b9eb4921e9c584eb4594437b5cd90ed6b920523606eae7316175f89c20628da14326801090167cc7fbffc77af448ac84b7e2
@@ -4471,18 +4485,18 @@
 "@webassemblyjs/helper-api-error@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-api-error@npm:1.11.6"
   checksum: e8563df85161096343008f9161adb138a6e8f3c2cc338d6a36011aa55eabb32f2fd138ffe63bc278d009ada001cc41d263dadd1c0be01be6c2ed99076103689f
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-buffer@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/helper-buffer@npm:1.11.6"
-  checksum: b14d0573bf680d22b2522e8a341ec451fddd645d1f9c6bd9012ccb7e587a2973b86ab7b89fe91e1c79939ba96095f503af04369a3b356c8023c13a5893221644
+"@webassemblyjs/helper-buffer@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/helper-buffer@npm:1.12.1"
+  checksum: c3ffb723024130308db608e86e2bdccd4868bbb62dffb0a9a1530606496f79c87f8565bd8e02805ce64912b71f1a70ee5fb00307258b0c082c3abf961d097eca
   languageName: node
   linkType: hard
 
 "@webassemblyjs/helper-numbers@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-numbers@npm:1.11.6"
   dependencies:
@@ -4496,23 +4510,23 @@
 "@webassemblyjs/helper-wasm-bytecode@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-wasm-bytecode@npm:1.11.6"
   checksum: 3535ef4f1fba38de3475e383b3980f4bbf3de72bbb631c2b6584c7df45be4eccd62c6ff48b5edd3f1bcff275cfd605a37679ec199fc91fd0a7705d7f1e3972dc
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-wasm-section@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/helper-wasm-section@npm:1.11.6"
+"@webassemblyjs/helper-wasm-section@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/helper-wasm-section@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
-    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
+    "@webassemblyjs/helper-buffer": 1.12.1
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
-    "@webassemblyjs/wasm-gen": 1.11.6
-  checksum: b2cf751bf4552b5b9999d27bbb7692d0aca75260140195cb58ea6374d7b9c2dc69b61e10b211a0e773f66209c3ddd612137ed66097e3684d7816f854997682e9
+    "@webassemblyjs/wasm-gen": 1.12.1
+  checksum: c19810cdd2c90ff574139b6d8c0dda254d42d168a9e5b3d353d1bc085f1d7164ccd1b3c05592a45a939c47f7e403dc8d03572bb686642f06a3d02932f6f0bc8f
   languageName: node
   linkType: hard
 
 "@webassemblyjs/ieee754@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/ieee754@npm:1.11.6"
   dependencies:
@@ -4533,76 +4547,76 @@
 "@webassemblyjs/utf8@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/utf8@npm:1.11.6"
   checksum: 807fe5b5ce10c390cfdd93e0fb92abda8aebabb5199980681e7c3743ee3306a75729bcd1e56a3903980e96c885ee53ef901fcbaac8efdfa480f9c0dae1d08713
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-edit@npm:^1.11.5":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wasm-edit@npm:1.11.6"
+"@webassemblyjs/wasm-edit@npm:^1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wasm-edit@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
-    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
+    "@webassemblyjs/helper-buffer": 1.12.1
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
-    "@webassemblyjs/helper-wasm-section": 1.11.6
-    "@webassemblyjs/wasm-gen": 1.11.6
-    "@webassemblyjs/wasm-opt": 1.11.6
-    "@webassemblyjs/wasm-parser": 1.11.6
-    "@webassemblyjs/wast-printer": 1.11.6
-  checksum: 29ce75870496d6fad864d815ebb072395a8a3a04dc9c3f4e1ffdc63fc5fa58b1f34304a1117296d8240054cfdbc38aca88e71fb51483cf29ffab0a61ef27b481
+    "@webassemblyjs/helper-wasm-section": 1.12.1
+    "@webassemblyjs/wasm-gen": 1.12.1
+    "@webassemblyjs/wasm-opt": 1.12.1
+    "@webassemblyjs/wasm-parser": 1.12.1
+    "@webassemblyjs/wast-printer": 1.12.1
+  checksum: ae23642303f030af888d30c4ef37b08dfec7eab6851a9575a616e65d1219f880d9223913a39056dd654e49049d76e97555b285d1f7e56935047abf578cce0692
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-gen@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wasm-gen@npm:1.11.6"
+"@webassemblyjs/wasm-gen@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wasm-gen@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
     "@webassemblyjs/ieee754": 1.11.6
     "@webassemblyjs/leb128": 1.11.6
     "@webassemblyjs/utf8": 1.11.6
-  checksum: a645a2eecbea24833c3260a249704a7f554ef4a94c6000984728e94bb2bc9140a68dfd6fd21d5e0bbb09f6dfc98e083a45760a83ae0417b41a0196ff6d45a23a
+  checksum: 5787626bb7f0b033044471ddd00ce0c9fe1ee4584e8b73e232051e3a4c99ba1a102700d75337151c8b6055bae77eefa4548960c610a5e4a504e356bd872138ff
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-opt@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wasm-opt@npm:1.11.6"
+"@webassemblyjs/wasm-opt@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wasm-opt@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
-    "@webassemblyjs/helper-buffer": 1.11.6
-    "@webassemblyjs/wasm-gen": 1.11.6
-    "@webassemblyjs/wasm-parser": 1.11.6
-  checksum: b4557f195487f8e97336ddf79f7bef40d788239169aac707f6eaa2fa5fe243557c2d74e550a8e57f2788e70c7ae4e7d32f7be16101afe183d597b747a3bdd528
+    "@webassemblyjs/ast": 1.12.1
+    "@webassemblyjs/helper-buffer": 1.12.1
+    "@webassemblyjs/wasm-gen": 1.12.1
+    "@webassemblyjs/wasm-parser": 1.12.1
+  checksum: 0e8fa8a0645304a1e18ff40d3db5a2e9233ebaa169b19fcc651d6fc9fe2cac0ce092ddee927318015ae735d9cd9c5d97c0cafb6a51dcd2932ac73587b62df991
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-parser@npm:1.11.6, @webassemblyjs/wasm-parser@npm:^1.11.5":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wasm-parser@npm:1.11.6"
+"@webassemblyjs/wasm-parser@npm:1.12.1, @webassemblyjs/wasm-parser@npm:^1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wasm-parser@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
     "@webassemblyjs/helper-api-error": 1.11.6
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
     "@webassemblyjs/ieee754": 1.11.6
     "@webassemblyjs/leb128": 1.11.6
     "@webassemblyjs/utf8": 1.11.6
-  checksum: 8200a8d77c15621724a23fdabe58d5571415cda98a7058f542e670ea965dd75499f5e34a48675184947c66f3df23adf55df060312e6d72d57908e3f049620d8a
+  checksum: 176015de3551ac068cd4505d837414f258d9ade7442bd71efb1232fa26c9f6d7d4e11a5c816caeed389943f409af7ebff6899289a992d7a70343cb47009d21a8
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wast-printer@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wast-printer@npm:1.11.6"
+"@webassemblyjs/wast-printer@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wast-printer@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
     "@xtuc/long": 4.2.2
-  checksum: d2fa6a4c427325ec81463e9c809aa6572af6d47f619f3091bf4c4a6fc34f1da3df7caddaac50b8e7a457f8784c62cd58c6311b6cb69b0162ccd8d4c072f79cf8
+  checksum: 2974b5dda8d769145ba0efd886ea94a601e61fb37114c14f9a9a7606afc23456799af652ac3052f284909bd42edc3665a76bc9b50f95f0794c053a8a1757b713
   languageName: node
   linkType: hard
 
 "@webpack-cli/configtest@npm:^2.1.1":
   version: 2.1.1
   resolution: "@webpack-cli/configtest@npm:2.1.1"
   peerDependencies:
@@ -4766,20 +4780,20 @@
   resolution: "agent-base@npm:6.0.2"
   dependencies:
     debug: 4
   checksum: f52b6872cc96fd5f622071b71ef200e01c7c4c454ee68bc9accca90c98cfb39f2810e3e9aa330435835eedc8c23f4f8a15267f67c6e245d2b33757575bdac49d
   languageName: node
   linkType: hard
 
-"agent-base@npm:^7.0.2, agent-base@npm:^7.1.0":
-  version: 7.1.0
-  resolution: "agent-base@npm:7.1.0"
+"agent-base@npm:^7.0.2, agent-base@npm:^7.1.0, agent-base@npm:^7.1.1":
+  version: 7.1.1
+  resolution: "agent-base@npm:7.1.1"
   dependencies:
     debug: ^4.3.4
-  checksum: f7828f991470a0cc22cb579c86a18cbae83d8a3cbed39992ab34fc7217c4d126017f1c74d0ab66be87f71455318a8ea3e757d6a37881b8d0f2a2c6aa55e5418f
+  checksum: 51c158769c5c051482f9ca2e6e1ec085ac72b5a418a9b31b4e82fe6c0a6699adb94c1c42d246699a587b3335215037091c79e0de512c516f73b6ea844202f037
   languageName: node
   linkType: hard
 
 "agentkeepalive@npm:^4.2.1":
   version: 4.5.0
   resolution: "agentkeepalive@npm:4.5.0"
   dependencies:
@@ -4841,22 +4855,22 @@
     json-schema-traverse: ^0.4.1
     uri-js: ^4.2.2
   checksum: 874972efe5c4202ab0a68379481fbd3d1b5d0a7bd6d3cc21d40d3536ebff3352a2a1fabb632d4fd2cc7fe4cbdcd5ed6782084c9bbf7f32a1536d18f9da5007d4
   languageName: node
   linkType: hard
 
 "ajv@npm:^8.0.0, ajv@npm:^8.12.0, ajv@npm:^8.9.0":
-  version: 8.12.0
-  resolution: "ajv@npm:8.12.0"
+  version: 8.13.0
+  resolution: "ajv@npm:8.13.0"
   dependencies:
-    fast-deep-equal: ^3.1.1
+    fast-deep-equal: ^3.1.3
     json-schema-traverse: ^1.0.0
     require-from-string: ^2.0.2
-    uri-js: ^4.2.2
-  checksum: 4dc13714e316e67537c8b31bc063f99a1d9d9a497eb4bbd55191ac0dcd5e4985bbb71570352ad6f1e76684fb6d790928f96ba3b2d4fd6e10024be9612fe3f001
+    uri-js: ^4.4.1
+  checksum: 6de82d0b2073e645ca3300561356ddda0234f39b35d2125a8700b650509b296f41c00ab69f53178bbe25ad688bd6ac3747ab44101f2f4bd245952e8fd6ccc3c1
   languageName: node
   linkType: hard
 
 "ansi-colors@npm:^4.1.1":
   version: 4.1.3
   resolution: "ansi-colors@npm:4.1.3"
   checksum: a9c2ec842038a1fabc7db9ece7d3177e2fe1c5dc6f0c51ecfbf5f39911427b89c00b5dc6b8bd95f82a26e9b16aaae2e83d45f060e98070ce4d1333038edceb0e
@@ -5030,21 +5044,21 @@
   version: 1.0.0
   resolution: "at-least-node@npm:1.0.0"
   checksum: 463e2f8e43384f1afb54bc68485c436d7622acec08b6fad269b421cb1d29cebb5af751426793d0961ed243146fe4dc983402f6d5a51b720b277818dbf6f2e49e
   languageName: node
   linkType: hard
 
 "axios@npm:^1.0.0":
-  version: 1.6.7
-  resolution: "axios@npm:1.6.7"
+  version: 1.7.1
+  resolution: "axios@npm:1.7.1"
   dependencies:
-    follow-redirects: ^1.15.4
+    follow-redirects: ^1.15.6
     form-data: ^4.0.0
     proxy-from-env: ^1.1.0
-  checksum: 87d4d429927d09942771f3b3a6c13580c183e31d7be0ee12f09be6d5655304996bb033d85e54be81606f4e89684df43be7bf52d14becb73a12727bf33298a082
+  checksum: 77760d94b3812e07d4a5b02468a55eed5c8435ef4d605d159f2808775bdd15da60ab5b15b665a6f72800b5d261875d808b410cd3cb1d7571cdc6ec5e0108025a
   languageName: node
   linkType: hard
 
 "babel-jest@npm:^29.7.0":
   version: 29.7.0
   resolution: "babel-jest@npm:29.7.0"
   dependencies:
@@ -5082,47 +5096,47 @@
     "@babel/types": ^7.3.3
     "@types/babel__core": ^7.1.14
     "@types/babel__traverse": ^7.0.6
   checksum: 51250f22815a7318f17214a9d44650ba89551e6d4f47a2dc259128428324b52f5a73979d010cefd921fd5a720d8c1d55ad74ff601cd94c7bd44d5f6292fde2d1
   languageName: node
   linkType: hard
 
-"babel-plugin-polyfill-corejs2@npm:^0.4.8":
-  version: 0.4.8
-  resolution: "babel-plugin-polyfill-corejs2@npm:0.4.8"
+"babel-plugin-polyfill-corejs2@npm:^0.4.10":
+  version: 0.4.11
+  resolution: "babel-plugin-polyfill-corejs2@npm:0.4.11"
   dependencies:
     "@babel/compat-data": ^7.22.6
-    "@babel/helper-define-polyfill-provider": ^0.5.0
+    "@babel/helper-define-polyfill-provider": ^0.6.2
     semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
-  checksum: 22857b87268b354e095452199464accba5fd8f690558a2f24b0954807ca2494b96da8d5c13507955802427582015160bce26a66893acf6da5dafbed8b336cf79
+  checksum: f098353ce7c7dde1a1d2710858e01b471e85689110c9e37813e009072347eb8c55d5f84d20d3bf1cab31755f20078ba90f8855fdc4686a9daa826a95ff280bd7
   languageName: node
   linkType: hard
 
-"babel-plugin-polyfill-corejs3@npm:^0.9.0":
-  version: 0.9.0
-  resolution: "babel-plugin-polyfill-corejs3@npm:0.9.0"
+"babel-plugin-polyfill-corejs3@npm:^0.10.4":
+  version: 0.10.4
+  resolution: "babel-plugin-polyfill-corejs3@npm:0.10.4"
   dependencies:
-    "@babel/helper-define-polyfill-provider": ^0.5.0
-    core-js-compat: ^3.34.0
+    "@babel/helper-define-polyfill-provider": ^0.6.1
+    core-js-compat: ^3.36.1
   peerDependencies:
     "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
-  checksum: 65bbf59fc0145c7a264822777403632008dce00015b4b5c7ec359125ef4faf9e8f494ae5123d2992104feb6f19a3cff85631992862e48b6d7bd64eb7e755ee1f
+  checksum: b96a54495f7cc8b3797251c8c15f5ed015edddc3110fc122f6b32c94bec33af1e8bc56fa99091808f500bde0cccaaa266889cdc5935d9e6e9cf09898214f02dd
   languageName: node
   linkType: hard
 
-"babel-plugin-polyfill-regenerator@npm:^0.5.5":
-  version: 0.5.5
-  resolution: "babel-plugin-polyfill-regenerator@npm:0.5.5"
+"babel-plugin-polyfill-regenerator@npm:^0.6.1":
+  version: 0.6.2
+  resolution: "babel-plugin-polyfill-regenerator@npm:0.6.2"
   dependencies:
-    "@babel/helper-define-polyfill-provider": ^0.5.0
+    "@babel/helper-define-polyfill-provider": ^0.6.2
   peerDependencies:
     "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
-  checksum: 3a9b4828673b23cd648dcfb571eadcd9d3fadfca0361d0a7c6feeb5a30474e92faaa49f067a6e1c05e49b6a09812879992028ff3ef3446229ff132d6e1de7eb6
+  checksum: 150233571072b6b3dfe946242da39cba8587b7f908d1c006f7545fc88b0e3c3018d445739beb61e7a75835f0c2751dbe884a94ff9b245ec42369d9267e0e1b3f
   languageName: node
   linkType: hard
 
 "babel-preset-current-node-syntax@npm:^1.0.0":
   version: 1.0.1
   resolution: "babel-preset-current-node-syntax@npm:1.0.1"
   dependencies:
@@ -5181,22 +5195,22 @@
   version: 5.2.2
   resolution: "big.js@npm:5.2.2"
   checksum: b89b6e8419b097a8fb4ed2399a1931a68c612bce3cfd5ca8c214b2d017531191070f990598de2fc6f3f993d91c0f08aa82697717f6b3b8732c9731866d233c9e
   languageName: node
   linkType: hard
 
 "bin-links@npm:^4.0.1":
-  version: 4.0.3
-  resolution: "bin-links@npm:4.0.3"
+  version: 4.0.4
+  resolution: "bin-links@npm:4.0.4"
   dependencies:
     cmd-shim: ^6.0.0
     npm-normalize-package-bin: ^3.0.0
     read-cmd-shim: ^4.0.0
     write-file-atomic: ^5.0.0
-  checksum: 3b3ee22efc38d608479d51675c8958a841b8b55b8975342ce86f28ac4e0bb3aef46e9dbdde976c6dc1fe1bd2aa00d42e00869ad35b57ee6d868f39f662858911
+  checksum: 9fca1fddaa3c1c9f7efd6fd7a6d991e3d8f6aaa9de5d0b9355469c2c594d8d06c9b2e0519bb0304202c14ddbe832d27b6d419d55cea4340e2c26116f9190e5c9
   languageName: node
   linkType: hard
 
 "bl@npm:^4.0.3, bl@npm:^4.1.0":
   version: 4.1.0
   resolution: "bl@npm:4.1.0"
   dependencies:
@@ -5222,24 +5236,24 @@
   resolution: "brace-expansion@npm:2.0.1"
   dependencies:
     balanced-match: ^1.0.0
   checksum: a61e7cd2e8a8505e9f0036b3b6108ba5e926b4b55089eeb5550cd04a471fe216c96d4fe7e4c7f995c728c554ae20ddfc4244cad10aef255e72b62930afd233d1
   languageName: node
   linkType: hard
 
-"braces@npm:^3.0.2":
-  version: 3.0.2
-  resolution: "braces@npm:3.0.2"
+"braces@npm:^3.0.3":
+  version: 3.0.3
+  resolution: "braces@npm:3.0.3"
   dependencies:
-    fill-range: ^7.0.1
-  checksum: e2a8e769a863f3d4ee887b5fe21f63193a891c68b612ddb4b68d82d1b5f3ff9073af066c343e9867a393fe4c2555dcb33e89b937195feb9c1613d259edfcd459
+    fill-range: ^7.1.1
+  checksum: b95aa0b3bd909f6cd1720ffcf031aeaf46154dd88b4da01f9a1d3f7ea866a79eba76a6d01cbc3c422b2ee5cdc39a4f02491058d5df0d7bf6e6a162a832df1f69
   languageName: node
   linkType: hard
 
-"browserslist@npm:^4.21.10, browserslist@npm:^4.22.2, browserslist@npm:^4.22.3":
+"browserslist@npm:^4.21.10, browserslist@npm:^4.22.2, browserslist@npm:^4.23.0":
   version: 4.23.0
   resolution: "browserslist@npm:4.23.0"
   dependencies:
     caniuse-lite: ^1.0.30001587
     electron-to-chromium: ^1.4.668
     node-releases: ^2.0.14
     update-browserslist-db: ^1.0.13
@@ -5288,19 +5302,19 @@
   version: 1.0.3
   resolution: "builtins@npm:1.0.3"
   checksum: 47ce94f7eee0e644969da1f1a28e5f29bd2e48b25b2bbb61164c345881086e29464ccb1fb88dbc155ea26e8b1f5fc8a923b26c8c1ed0935b67b644d410674513
   languageName: node
   linkType: hard
 
 "builtins@npm:^5.0.0":
-  version: 5.0.1
-  resolution: "builtins@npm:5.0.1"
+  version: 5.1.0
+  resolution: "builtins@npm:5.1.0"
   dependencies:
     semver: ^7.0.0
-  checksum: 66d204657fe36522822a95b288943ad11b58f5eaede235b11d8c4edaa28ce4800087d44a2681524c340494aadb120a0068011acabe99d30e8f11a7d826d83515
+  checksum: 76327fa85b8e253b26e52f79988148013ea742691b4ab15f7228ebee47dd757832da308c9d4e4fc89763a1773e3f25a9836fff6315df85c7c6c72190436bf11d
   languageName: node
   linkType: hard
 
 "byte-size@npm:7.0.0":
   version: 7.0.0
   resolution: "byte-size@npm:7.0.0"
   checksum: 6cdd45fb64ac3f80d5cbbc01df7974a4613b3e64bd792b6b8211c8669ca3d1f7efd9379ba24cebfc371ce3e890817dcdaf0bd7ed99571fe2de4b946e6c31a138
@@ -5350,30 +5364,30 @@
     tar: ^6.1.11
     unique-filename: ^3.0.0
   checksum: b7751df756656954a51201335addced8f63fc53266fa56392c9f5ae83c8d27debffb4458ac2d168a744a4517ec3f2163af05c20097f93d17bdc2dc8a385e14a6
   languageName: node
   linkType: hard
 
 "cacache@npm:^18.0.0":
-  version: 18.0.2
-  resolution: "cacache@npm:18.0.2"
+  version: 18.0.3
+  resolution: "cacache@npm:18.0.3"
   dependencies:
     "@npmcli/fs": ^3.1.0
     fs-minipass: ^3.0.0
     glob: ^10.2.2
     lru-cache: ^10.0.1
     minipass: ^7.0.3
     minipass-collect: ^2.0.1
     minipass-flush: ^1.0.5
     minipass-pipeline: ^1.2.4
     p-map: ^4.0.0
     ssri: ^10.0.0
     tar: ^6.1.11
     unique-filename: ^3.0.0
-  checksum: 0250df80e1ad0c828c956744850c5f742c24244e9deb5b7dc81bca90f8c10e011e132ecc58b64497cc1cad9a98968676147fb6575f4f94722f7619757b17a11b
+  checksum: b717fd9b36e9c3279bfde4545c3a8f6d5a539b084ee26a9504d48f83694beb724057d26e090b97540f9cc62bea18b9f6cf671c50e18fb7dac60eda9db691714f
   languageName: node
   linkType: hard
 
 "callsites@npm:^3.0.0":
   version: 3.1.0
   resolution: "callsites@npm:3.1.0"
   checksum: 072d17b6abb459c2ba96598918b55868af677154bec7e73d222ef95a8fdb9bbf7dae96a8421085cdad8cd190d86653b5b6dc55a4484f2e5b2e27d5e0c3fc15b3
@@ -5402,17 +5416,17 @@
   version: 6.3.0
   resolution: "camelcase@npm:6.3.0"
   checksum: 8c96818a9076434998511251dcb2761a94817ea17dbdc37f47ac080bd088fc62c7369429a19e2178b993497132c8cbcf5cc1f44ba963e76782ba469c0474938d
   languageName: node
   linkType: hard
 
 "caniuse-lite@npm:^1.0.30001587":
-  version: 1.0.30001587
-  resolution: "caniuse-lite@npm:1.0.30001587"
-  checksum: fb50aa9beaaae42f9feae92ce038f6ff71e97510f024ef1bef2666f3adcfd36d6c59e5675442e5fe795575193f71bc826cb7721d4b0f6d763e82d193bea57863
+  version: 1.0.30001620
+  resolution: "caniuse-lite@npm:1.0.30001620"
+  checksum: 1831e519c29ce6971bc50d56bab196a307fcb4181e7deaa80df314b035b87b3912b8626b4e87adc301d0bfe6a90b99814101b1cb28114b96e720f996f19bdc0d
   languageName: node
   linkType: hard
 
 "chalk@npm:4.1.0":
   version: 4.1.0
   resolution: "chalk@npm:4.1.0"
   dependencies:
@@ -5453,21 +5467,14 @@
 "chardet@npm:^0.7.0":
   version: 0.7.0
   resolution: "chardet@npm:0.7.0"
   checksum: 6fd5da1f5d18ff5712c1e0aed41da200d7c51c28f11b36ee3c7b483f3696dabc08927fc6b227735eb8f0e1215c9a8abd8154637f3eff8cada5959df7f58b024d
   languageName: node
   linkType: hard
 
-"child_process@npm:~1.0.2":
-  version: 1.0.2
-  resolution: "child_process@npm:1.0.2"
-  checksum: bd814d82bc8c6e85ed6fb157878978121cd03b5296c09f6135fa3d081fd9a6a617a6d509c50397711df713af403331241a9c0397a7fad30672051485e156c2a1
-  languageName: node
-  linkType: hard
-
 "chownr@npm:^2.0.0":
   version: 2.0.0
   resolution: "chownr@npm:2.0.0"
   checksum: c57cf9dd0791e2f18a5ee9c1a299ae6e801ff58fee96dc8bfd0dcb4738a6ce58dd252a3605b1c93c6418fe4f9d5093b28ffbf4d66648cb2a9c67eaef9679be2f
   languageName: node
   linkType: hard
 
@@ -5489,17 +5496,17 @@
   version: 3.9.0
   resolution: "ci-info@npm:3.9.0"
   checksum: 6b19dc9b2966d1f8c2041a838217299718f15d6c4b63ae36e4674edd2bee48f780e94761286a56aa59eb305a85fbea4ddffb7630ec063e7ec7e7e5ad42549a87
   languageName: node
   linkType: hard
 
 "cjs-module-lexer@npm:^1.0.0":
-  version: 1.2.3
-  resolution: "cjs-module-lexer@npm:1.2.3"
-  checksum: 5ea3cb867a9bb609b6d476cd86590d105f3cfd6514db38ff71f63992ab40939c2feb68967faa15a6d2b1f90daa6416b79ea2de486e9e2485a6f8b66a21b4fb0a
+  version: 1.3.1
+  resolution: "cjs-module-lexer@npm:1.3.1"
+  checksum: 75f20ac264a397ea5c63f9c2343a51ab878043666468f275e94862f7180ec1d764a400ec0c09085dcf0db3193c74a8b571519abd2bf4be0d2be510d1377c8d4b
   languageName: node
   linkType: hard
 
 "clean-stack@npm:^2.0.0":
   version: 2.2.0
   resolution: "clean-stack@npm:2.2.0"
   checksum: 2ac8cd2b2f5ec986a3c743935ec85b07bc174d5421a5efc8017e1f146a1cf5f781ae962618f416352103b32c9cd7e203276e8c28241bbe946160cab16149fb68
@@ -5582,17 +5589,17 @@
   dependencies:
     mkdirp-infer-owner: ^2.0.0
   checksum: 83d2a46cdf4adbb38d3d3184364b2df0e4c001ac770f5ca94373825d7a48838b4cb8a59534ef48f02b0d556caa047728589ca65c640c17c0b417b3afb34acfbb
   languageName: node
   linkType: hard
 
 "cmd-shim@npm:^6.0.0":
-  version: 6.0.2
-  resolution: "cmd-shim@npm:6.0.2"
-  checksum: df3a01fc4d72a49b450985b991205e65774b28e7f74a2e4d2a11fd0df8732e3828f9e7b644050def3cd0be026cbd3ee46a1f50ce5f57d0b3fb5afe335bdfacde
+  version: 6.0.3
+  resolution: "cmd-shim@npm:6.0.3"
+  checksum: bd79ac1505fea77cba0caf271c16210ebfbe50f348a1907f4700740876ab2157e00882b9baa685a9fcf9bc92e08a87e21bd757f45a6938f00290422f80f7d27a
   languageName: node
   linkType: hard
 
 "co@npm:^4.6.0":
   version: 4.6.0
   resolution: "co@npm:4.6.0"
   checksum: 5210d9223010eb95b29df06a91116f2cf7c8e0748a9013ed853b53f362ea0e822f1e5bb054fb3cefc645239a4cf966af1f6133a3b43f40d591f3b68ed6cf0510
@@ -5882,20 +5889,20 @@
 "convert-source-map@npm:^2.0.0":
   version: 2.0.0
   resolution: "convert-source-map@npm:2.0.0"
   checksum: 63ae9933be5a2b8d4509daca5124e20c14d023c820258e484e32dc324d34c2754e71297c94a05784064ad27615037ef677e3f0c00469fb55f409d2bb21261035
   languageName: node
   linkType: hard
 
-"core-js-compat@npm:^3.31.0, core-js-compat@npm:^3.34.0":
-  version: 3.36.0
-  resolution: "core-js-compat@npm:3.36.0"
+"core-js-compat@npm:^3.31.0, core-js-compat@npm:^3.36.1":
+  version: 3.37.1
+  resolution: "core-js-compat@npm:3.37.1"
   dependencies:
-    browserslist: ^4.22.3
-  checksum: 89d9bdc91cc4085e81c7774427a02b42b494d569f62972658bf8b6ace1931ee60620691fbcd646fcb6a7ead3d874a46990491f345fc29e0d084ed2fcce335aa5
+    browserslist: ^4.23.0
+  checksum: 5e7430329358bced08c30950512d2081aea0a5652b4c5892cbb3c4a6db05b0d3893a191a955162a07fdb5f4fe74e61b6429fdb503f54e062336d76e43c9555d9
   languageName: node
   linkType: hard
 
 "core-util-is@npm:~1.0.0":
   version: 1.0.3
   resolution: "core-util-is@npm:1.0.3"
   checksum: 9de8597363a8e9b9952491ebe18167e3b36e7707569eed0ebf14f8bba773611376466ae34575bca8cfe3c767890c859c74056084738f09d4e4a6f902b2ad7d99
@@ -5954,34 +5961,34 @@
   version: 2.0.0
   resolution: "crypto-random-string@npm:2.0.0"
   checksum: 0283879f55e7c16fdceacc181f87a0a65c53bc16ffe1d58b9d19a6277adcd71900d02bb2c4843dd55e78c51e30e89b0fec618a7f170ebcc95b33182c28f05fd6
   languageName: node
   linkType: hard
 
 "css-loader@npm:^6.7.1":
-  version: 6.10.0
-  resolution: "css-loader@npm:6.10.0"
+  version: 6.11.0
+  resolution: "css-loader@npm:6.11.0"
   dependencies:
     icss-utils: ^5.1.0
     postcss: ^8.4.33
-    postcss-modules-extract-imports: ^3.0.0
-    postcss-modules-local-by-default: ^4.0.4
-    postcss-modules-scope: ^3.1.1
+    postcss-modules-extract-imports: ^3.1.0
+    postcss-modules-local-by-default: ^4.0.5
+    postcss-modules-scope: ^3.2.0
     postcss-modules-values: ^4.0.0
     postcss-value-parser: ^4.2.0
     semver: ^7.5.4
   peerDependencies:
     "@rspack/core": 0.x || 1.x
     webpack: ^5.0.0
   peerDependenciesMeta:
     "@rspack/core":
       optional: true
     webpack:
       optional: true
-  checksum: ee3d62b5f7e4eb24281a22506431e920d07a45bd6ea627731ce583f3c6a846ab8b8b703bace599b9b35256b9e762f9f326d969abb72b69c7e6055eacf39074fd
+  checksum: 5c8d35975a7121334905394e88e28f05df72f037dbed2fb8fec4be5f0b313ae73a13894ba791867d4a4190c35896da84a7fd0c54fb426db55d85ba5e714edbe3
   languageName: node
   linkType: hard
 
 "cssesc@npm:^3.0.0":
   version: 3.0.0
   resolution: "cssesc@npm:3.0.0"
   bin:
@@ -6103,22 +6110,22 @@
   version: 0.7.0
   resolution: "dedent@npm:0.7.0"
   checksum: 87de191050d9a40dd70cad01159a0bcf05ecb59750951242070b6abf9569088684880d00ba92a955b4058804f16eeaf91d604f283929b4f614d181cd7ae633d2
   languageName: node
   linkType: hard
 
 "dedent@npm:^1.0.0":
-  version: 1.5.1
-  resolution: "dedent@npm:1.5.1"
+  version: 1.5.3
+  resolution: "dedent@npm:1.5.3"
   peerDependencies:
     babel-plugin-macros: ^3.1.0
   peerDependenciesMeta:
     babel-plugin-macros:
       optional: true
-  checksum: c3c300a14edf1bdf5a873f9e4b22e839d62490bc5c8d6169c1f15858a1a76733d06a9a56930e963d677a2ceeca4b6b0894cc5ea2f501aa382ca5b92af3413c2a
+  checksum: 045b595557b2a8ea2eb9b0b4623d764e9a87326486fe2b61191b4342ed93dc01245644d8a09f3108a50c0ee7965f1eedd92e4a3a503ed89ea8e810566ea27f9a
   languageName: node
   linkType: hard
 
 "deep-is@npm:^0.1.3":
   version: 0.1.4
   resolution: "deep-is@npm:0.1.4"
   checksum: edb65dd0d7d1b9c40b2f50219aef30e116cedd6fc79290e740972c132c09106d2e80aa0bc8826673dd5a00222d4179c84b36a790eef63a4c4bca75a37ef90804
@@ -6220,26 +6227,26 @@
   resolution: "doctrine@npm:3.0.0"
   dependencies:
     esutils: ^2.0.2
   checksum: fd7673ca77fe26cd5cba38d816bc72d641f500f1f9b25b83e8ce28827fe2da7ad583a8da26ab6af85f834138cf8dae9f69b0cd6ab925f52ddab1754db44d99ce
   languageName: node
   linkType: hard
 
-"dom-serializer@npm:^1.0.1":
-  version: 1.4.1
-  resolution: "dom-serializer@npm:1.4.1"
+"dom-serializer@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "dom-serializer@npm:2.0.0"
   dependencies:
-    domelementtype: ^2.0.1
-    domhandler: ^4.2.0
-    entities: ^2.0.0
-  checksum: fbb0b01f87a8a2d18e6e5a388ad0f7ec4a5c05c06d219377da1abc7bb0f674d804f4a8a94e3f71ff15f6cb7dcfc75704a54b261db672b9b3ab03da6b758b0b22
+    domelementtype: ^2.3.0
+    domhandler: ^5.0.2
+    entities: ^4.2.0
+  checksum: cd1810544fd8cdfbd51fa2c0c1128ec3a13ba92f14e61b7650b5de421b88205fd2e3f0cc6ace82f13334114addb90ed1c2f23074a51770a8e9c1273acbc7f3e6
   languageName: node
   linkType: hard
 
-"domelementtype@npm:^2.0.1, domelementtype@npm:^2.2.0":
+"domelementtype@npm:^2.3.0":
   version: 2.3.0
   resolution: "domelementtype@npm:2.3.0"
   checksum: ee837a318ff702622f383409d1f5b25dd1024b692ef64d3096ff702e26339f8e345820f29a68bcdcea8cfee3531776b3382651232fbeae95612d6f0a75efb4f6
   languageName: node
   linkType: hard
 
 "domexception@npm:^4.0.0":
@@ -6247,31 +6254,31 @@
   resolution: "domexception@npm:4.0.0"
   dependencies:
     webidl-conversions: ^7.0.0
   checksum: ddbc1268edf33a8ba02ccc596735ede80375ee0cf124b30d2f05df5b464ba78ef4f49889b6391df4a04954e63d42d5631c7fcf8b1c4f12bc531252977a5f13d5
   languageName: node
   linkType: hard
 
-"domhandler@npm:^4.0.0, domhandler@npm:^4.2.0":
-  version: 4.3.1
-  resolution: "domhandler@npm:4.3.1"
+"domhandler@npm:^5.0.2, domhandler@npm:^5.0.3":
+  version: 5.0.3
+  resolution: "domhandler@npm:5.0.3"
   dependencies:
-    domelementtype: ^2.2.0
-  checksum: 4c665ceed016e1911bf7d1dadc09dc888090b64dee7851cccd2fcf5442747ec39c647bb1cb8c8919f8bbdd0f0c625a6bafeeed4b2d656bbecdbae893f43ffaaa
+    domelementtype: ^2.3.0
+  checksum: 0f58f4a6af63e6f3a4320aa446d28b5790a009018707bce2859dcb1d21144c7876482b5188395a188dfa974238c019e0a1e610d2fc269a12b2c192ea2b0b131c
   languageName: node
   linkType: hard
 
-"domutils@npm:^2.5.2":
-  version: 2.8.0
-  resolution: "domutils@npm:2.8.0"
+"domutils@npm:^3.0.1":
+  version: 3.1.0
+  resolution: "domutils@npm:3.1.0"
   dependencies:
-    dom-serializer: ^1.0.1
-    domelementtype: ^2.2.0
-    domhandler: ^4.2.0
-  checksum: abf7434315283e9aadc2a24bac0e00eab07ae4313b40cc239f89d84d7315ebdfd2fb1b5bf750a96bc1b4403d7237c7b2ebf60459be394d625ead4ca89b934391
+    dom-serializer: ^2.0.0
+    domelementtype: ^2.3.0
+    domhandler: ^5.0.3
+  checksum: e5757456ddd173caa411cfc02c2bb64133c65546d2c4081381a3bafc8a57411a41eed70494551aa58030be9e58574fcc489828bebd673863d39924fb4878f416
   languageName: node
   linkType: hard
 
 "dot-prop@npm:6.0.1":
   version: 6.0.1
   resolution: "dot-prop@npm:6.0.1"
   dependencies:
@@ -6319,28 +6326,28 @@
   version: 0.2.0
   resolution: "eastasianwidth@npm:0.2.0"
   checksum: 7d00d7cd8e49b9afa762a813faac332dee781932d6f2c848dc348939c4253f1d4564341b7af1d041853bc3f32c2ef141b58e0a4d9862c17a7f08f68df1e0f1ed
   languageName: node
   linkType: hard
 
 "ejs@npm:^3.1.7":
-  version: 3.1.9
-  resolution: "ejs@npm:3.1.9"
+  version: 3.1.10
+  resolution: "ejs@npm:3.1.10"
   dependencies:
     jake: ^10.8.5
   bin:
     ejs: bin/cli.js
-  checksum: af6f10eb815885ff8a8cfacc42c6b6cf87daf97a4884f87a30e0c3271fedd85d76a3a297d9c33a70e735b97ee632887f85e32854b9cdd3a2d97edf931519a35f
+  checksum: ce90637e9c7538663ae023b8a7a380b2ef7cc4096de70be85abf5a3b9641912dde65353211d05e24d56b1f242d71185c6d00e02cb8860701d571786d92c71f05
   languageName: node
   linkType: hard
 
 "electron-to-chromium@npm:^1.4.668":
-  version: 1.4.670
-  resolution: "electron-to-chromium@npm:1.4.670"
-  checksum: 862fb1ebb0ff58816cf2f70c973c1915d5c4b1f88c43dad040130e0fdf162b9477f9ff14d70cac8aa668e45c093dd5b0b3815728ec79a8118aa5e62d8c48ee6b
+  version: 1.4.776
+  resolution: "electron-to-chromium@npm:1.4.776"
+  checksum: 18c5a4da40296e9a27638ff479dd79d8496dd8848998a9a8b32bd85ab4c1431f65d88b0c3df8944fab7fda86b239da72017a4ae5c40c22f17704c4ff29f151d8
   languageName: node
   linkType: hard
 
 "emittery@npm:^0.13.1":
   version: 0.13.1
   resolution: "emittery@npm:0.13.1"
   checksum: 2b089ab6306f38feaabf4f6f02792f9ec85fc054fda79f44f6790e61bbf6bc4e1616afb9b232e0c5ec5289a8a452f79bfa6d905a6fd64e94b49981f0934001c6
@@ -6382,60 +6389,53 @@
   resolution: "end-of-stream@npm:1.4.4"
   dependencies:
     once: ^1.4.0
   checksum: 530a5a5a1e517e962854a31693dbb5c0b2fc40b46dad2a56a2deec656ca040631124f4795823acc68238147805f8b021abbe221f4afed5ef3c8e8efc2024908b
   languageName: node
   linkType: hard
 
-"enhanced-resolve@npm:^5.15.0":
-  version: 5.15.0
-  resolution: "enhanced-resolve@npm:5.15.0"
+"enhanced-resolve@npm:^5.16.0":
+  version: 5.16.1
+  resolution: "enhanced-resolve@npm:5.16.1"
   dependencies:
     graceful-fs: ^4.2.4
     tapable: ^2.2.0
-  checksum: fbd8cdc9263be71cc737aa8a7d6c57b43d6aa38f6cc75dde6fcd3598a130cc465f979d2f4d01bb3bf475acb43817749c79f8eef9be048683602ca91ab52e4f11
+  checksum: 6e4c166fef72ef231455f9119686d93ecccb11874f8256d73a42de5b293cb2536050849382468864b25973514ca4fa4cb13c37be2ff857a211e2aca3ff05bb6c
   languageName: node
   linkType: hard
 
 "enquirer@npm:~2.3.6":
   version: 2.3.6
   resolution: "enquirer@npm:2.3.6"
   dependencies:
     ansi-colors: ^4.1.1
   checksum: 1c0911e14a6f8d26721c91e01db06092a5f7675159f0261d69c403396a385afd13dd76825e7678f66daffa930cfaa8d45f506fb35f818a2788463d022af1b884
   languageName: node
   linkType: hard
 
-"entities@npm:^2.0.0":
-  version: 2.2.0
-  resolution: "entities@npm:2.2.0"
-  checksum: 19010dacaf0912c895ea262b4f6128574f9ccf8d4b3b65c7e8334ad0079b3706376360e28d8843ff50a78aabcb8f08f0a32dbfacdc77e47ed77ca08b713669b3
-  languageName: node
-  linkType: hard
-
-"entities@npm:^4.4.0":
+"entities@npm:^4.2.0, entities@npm:^4.4.0":
   version: 4.5.0
   resolution: "entities@npm:4.5.0"
   checksum: 853f8ebd5b425d350bffa97dd6958143179a5938352ccae092c62d1267c4e392a039be1bae7d51b6e4ffad25f51f9617531fedf5237f15df302ccfb452cbf2d7
   languageName: node
   linkType: hard
 
 "env-paths@npm:^2.2.0":
   version: 2.2.1
   resolution: "env-paths@npm:2.2.1"
   checksum: 65b5df55a8bab92229ab2b40dad3b387fad24613263d103a97f91c9fe43ceb21965cd3392b1ccb5d77088021e525c4e0481adb309625d0cb94ade1d1fb8dc17e
   languageName: node
   linkType: hard
 
 "envinfo@npm:^7.7.3, envinfo@npm:^7.7.4":
-  version: 7.11.1
-  resolution: "envinfo@npm:7.11.1"
+  version: 7.13.0
+  resolution: "envinfo@npm:7.13.0"
   bin:
     envinfo: dist/cli.js
-  checksum: f3d38ab6bc62388466e86e2f5665f90f238ca349c81bb36b311d908cb5ca96650569b43b308c9dcb6725a222693f6c43a704794e74a68fb445ec5575a90ca05e
+  checksum: 822fc30f53bd0be67f0e25be96eb6a2562b8062f3058846bbd7ec471bd4b7835fca6436ee72c4029c8ae4a3d8f8cddbe2ee725b22291f015232d20a682bee732
   languageName: node
   linkType: hard
 
 "err-code@npm:^2.0.2":
   version: 2.0.3
   resolution: "err-code@npm:2.0.3"
   checksum: 8b7b1be20d2de12d2255c0bc2ca638b7af5171142693299416e6a9339bd7d88fc8d7707d913d78e0993176005405a236b066b45666b27b797252c771156ace54
@@ -6448,21 +6448,21 @@
   dependencies:
     is-arrayish: ^0.2.1
   checksum: c1c2b8b65f9c91b0f9d75f0debaa7ec5b35c266c2cac5de412c1a6de86d4cbae04ae44e510378cb14d032d0645a36925d0186f8bb7367bcc629db256b743a001
   languageName: node
   linkType: hard
 
 "es-module-lexer@npm:^1.2.1":
-  version: 1.4.1
-  resolution: "es-module-lexer@npm:1.4.1"
-  checksum: a11b5a256d4e8e9c7d94c2fd87415ccd1591617b6edd847e064503f8eaece2d25e2e9078a02c5ce3ed5e83bb748f5b4820efbe78072c8beb07ac619c2edec35d
+  version: 1.5.3
+  resolution: "es-module-lexer@npm:1.5.3"
+  checksum: 2e0a0936fb49ca072d438128f588d5b46974035f7a1362bdb26447868016243cfd1c5ec8f12e80d273749e8c603f5aba5a828d5c2d95c07f61fbe77ab4fce4af
   languageName: node
   linkType: hard
 
-"escalade@npm:^3.1.1":
+"escalade@npm:^3.1.1, escalade@npm:^3.1.2":
   version: 3.1.2
   resolution: "escalade@npm:3.1.2"
   checksum: 1ec0977aa2772075493002bdbd549d595ff6e9393b1cb0d7d6fcaf78c750da0c158f180938365486f75cb69fba20294351caddfce1b46552a7b6c3cde52eaa02
   languageName: node
   linkType: hard
 
 "escape-string-regexp@npm:^1.0.5":
@@ -6559,22 +6559,22 @@
   version: 3.4.3
   resolution: "eslint-visitor-keys@npm:3.4.3"
   checksum: 36e9ef87fca698b6fd7ca5ca35d7b2b6eeaaf106572e2f7fd31c12d3bfdaccdb587bba6d3621067e5aece31c8c3a348b93922ab8f7b2cbc6aaab5e1d89040c60
   languageName: node
   linkType: hard
 
 "eslint@npm:^8":
-  version: 8.56.0
-  resolution: "eslint@npm:8.56.0"
+  version: 8.57.0
+  resolution: "eslint@npm:8.57.0"
   dependencies:
     "@eslint-community/eslint-utils": ^4.2.0
     "@eslint-community/regexpp": ^4.6.1
     "@eslint/eslintrc": ^2.1.4
-    "@eslint/js": 8.56.0
-    "@humanwhocodes/config-array": ^0.11.13
+    "@eslint/js": 8.57.0
+    "@humanwhocodes/config-array": ^0.11.14
     "@humanwhocodes/module-importer": ^1.0.1
     "@nodelib/fs.walk": ^1.2.8
     "@ungap/structured-clone": ^1.2.0
     ajv: ^6.12.4
     chalk: ^4.0.0
     cross-spawn: ^7.0.2
     debug: ^4.3.2
@@ -6602,15 +6602,15 @@
     minimatch: ^3.1.2
     natural-compare: ^1.4.0
     optionator: ^0.9.3
     strip-ansi: ^6.0.1
     text-table: ^0.2.0
   bin:
     eslint: bin/eslint.js
-  checksum: 883436d1e809b4a25d9eb03d42f584b84c408dbac28b0019f6ea07b5177940bf3cca86208f749a6a1e0039b63e085ee47aca1236c30721e91f0deef5cc5a5136
+  checksum: 3a48d7ff85ab420a8447e9810d8087aea5b1df9ef68c9151732b478de698389ee656fd895635b5f2871c89ee5a2652b3f343d11e9db6f8486880374ebc74a2d9
   languageName: node
   linkType: hard
 
 "espree@npm:^9.6.0, espree@npm:^9.6.1":
   version: 9.6.1
   resolution: "espree@npm:9.6.1"
   dependencies:
@@ -6872,20 +6872,20 @@
   resolution: "filelist@npm:1.0.4"
   dependencies:
     minimatch: ^5.0.1
   checksum: a303573b0821e17f2d5e9783688ab6fbfce5d52aaac842790ae85e704a6f5e4e3538660a63183d6453834dedf1e0f19a9dadcebfa3e926c72397694ea11f5160
   languageName: node
   linkType: hard
 
-"fill-range@npm:^7.0.1":
-  version: 7.0.1
-  resolution: "fill-range@npm:7.0.1"
+"fill-range@npm:^7.1.1":
+  version: 7.1.1
+  resolution: "fill-range@npm:7.1.1"
   dependencies:
     to-regex-range: ^5.0.1
-  checksum: cc283f4e65b504259e64fd969bcf4def4eb08d85565e906b7d36516e87819db52029a76b6363d0f02d0d532f0033c9603b9e2d943d56ee3b0d4f7ad3328ff917
+  checksum: b4abfbca3839a3d55e4ae5ec62e131e2e356bf4859ce8480c64c4876100f4df292a63e5bb1618e1d7460282ca2b305653064f01654474aa35c68000980f17798
   languageName: node
   linkType: hard
 
 "find-root@npm:^1.0.0":
   version: 1.1.0
   resolution: "find-root@npm:1.1.0"
   checksum: b2a59fe4b6c932eef36c45a048ae8f93c85640212ebe8363164814990ee20f154197505965f3f4f102efc33bfb1cbc26fd17c4a2fc739ebc51b886b137cbefaf
@@ -6938,27 +6938,27 @@
   bin:
     flat: cli.js
   checksum: 12a1536ac746db74881316a181499a78ef953632ddd28050b7a3a43c62ef5462e3357c8c29d76072bb635f147f7a9a1f0c02efef6b4be28f8db62ceb3d5c7f5d
   languageName: node
   linkType: hard
 
 "flatted@npm:^3.2.9":
-  version: 3.2.9
-  resolution: "flatted@npm:3.2.9"
-  checksum: f14167fbe26a9d20f6fca8d998e8f1f41df72c8e81f9f2c9d61ed2bea058248f5e1cbd05e7f88c0e5087a6a0b822a1e5e2b446e879f3cfbe0b07ba2d7f80b026
+  version: 3.3.1
+  resolution: "flatted@npm:3.3.1"
+  checksum: 85ae7181650bb728c221e7644cbc9f4bf28bc556f2fc89bb21266962bdf0ce1029cc7acc44bb646cd469d9baac7c317f64e841c4c4c00516afa97320cdac7f94
   languageName: node
   linkType: hard
 
-"follow-redirects@npm:^1.15.4":
-  version: 1.15.5
-  resolution: "follow-redirects@npm:1.15.5"
+"follow-redirects@npm:^1.15.6":
+  version: 1.15.6
+  resolution: "follow-redirects@npm:1.15.6"
   peerDependenciesMeta:
     debug:
       optional: true
-  checksum: 5ca49b5ce6f44338cbfc3546823357e7a70813cecc9b7b768158a1d32c1e62e7407c944402a918ea8c38ae2e78266312d617dc68783fac502cbb55e1047b34ec
+  checksum: a62c378dfc8c00f60b9c80cab158ba54e99ba0239a5dd7c81245e5a5b39d10f0c35e249c3379eae719ff0285fff88c365dd446fab19dee771f1d76252df1bbf5
   languageName: node
   linkType: hard
 
 "foreground-child@npm:^3.1.0":
   version: 3.1.1
   resolution: "foreground-child@npm:3.1.1"
   dependencies:
@@ -7091,26 +7091,26 @@
     strip-ansi: ^6.0.1
     wide-align: ^1.1.5
   checksum: 788b6bfe52f1dd8e263cda800c26ac0ca2ff6de0b6eee2fe0d9e3abf15e149b651bd27bf5226be10e6e3edb5c4e5d5985a5a1a98137e7a892f75eff76467ad2d
   languageName: node
   linkType: hard
 
 "gauge@npm:^5.0.0":
-  version: 5.0.1
-  resolution: "gauge@npm:5.0.1"
+  version: 5.0.2
+  resolution: "gauge@npm:5.0.2"
   dependencies:
     aproba: ^1.0.3 || ^2.0.0
     color-support: ^1.1.3
     console-control-strings: ^1.1.0
     has-unicode: ^2.0.1
     signal-exit: ^4.0.1
     string-width: ^4.2.3
     strip-ansi: ^6.0.1
     wide-align: ^1.1.5
-  checksum: 09b1eb8d8c850df7e4e2822feef27427afc845d4839fa13a08ddad74f882caf668dd1e77ac5e059d3e9a7b0cef59b706d28be40e1dc5fd326da32965e1f206a6
+  checksum: bc51e4f849bce385e51047d5f372fd15e04b8d41abf63b32cc29587678542570eab9694e4ebeb9afa9ff77440eeceb427296409a7c181ce502222a8856f225c6
   languageName: node
   linkType: hard
 
 "gensync@npm:^1.0.0-beta.2":
   version: 1.0.0-beta.2
   resolution: "gensync@npm:1.0.0-beta.2"
   checksum: a7437e58c6be12aa6c90f7730eac7fa9833dc78872b4ad2963d2031b00a3367a93f98aec75f9aaac7220848e4026d67a8655e870b24f20a543d103c0d65952ec
@@ -7267,25 +7267,25 @@
     once: ^1.3.0
     path-is-absolute: ^1.0.0
   checksum: f52480fc82b1e66e52990f0f2e7306447d12294c83fbbee0395e761ad1178172012a7cc0673dbf4810baac400fc09bf34484c08b5778c216403fd823db281716
   languageName: node
   linkType: hard
 
 "glob@npm:^10.2.2, glob@npm:^10.3.10, glob@npm:^10.3.7":
-  version: 10.3.10
-  resolution: "glob@npm:10.3.10"
+  version: 10.3.15
+  resolution: "glob@npm:10.3.15"
   dependencies:
     foreground-child: ^3.1.0
-    jackspeak: ^2.3.5
+    jackspeak: ^2.3.6
     minimatch: ^9.0.1
-    minipass: ^5.0.0 || ^6.0.2 || ^7.0.0
-    path-scurry: ^1.10.1
+    minipass: ^7.0.4
+    path-scurry: ^1.11.0
   bin:
     glob: dist/esm/bin.mjs
-  checksum: 4f2fe2511e157b5a3f525a54092169a5f92405f24d2aed3142f4411df328baca13059f4182f1db1bf933e2c69c0bd89e57ae87edd8950cba8c7ccbe84f721cf3
+  checksum: c7aeae0b4eea0dfedc6682b71a8ad4d1ea9dfec0f2440571f916e1918c046824c8d441bbe1965c06fede025a0726c6daab5ae8019afe667364f43776eaaf9044
   languageName: node
   linkType: hard
 
 "glob@npm:^7.1.3, glob@npm:^7.1.4":
   version: 7.2.3
   resolution: "glob@npm:7.2.3"
   dependencies:
@@ -7371,15 +7371,15 @@
 "graceful-fs@npm:4.2.10":
   version: 4.2.10
   resolution: "graceful-fs@npm:4.2.10"
   checksum: 3f109d70ae123951905d85032ebeae3c2a5a7a997430df00ea30df0e3a6c60cf6689b109654d6fdacd28810a053348c4d14642da1d075049e6be1ba5216218da
   languageName: node
   linkType: hard
 
-"graceful-fs@npm:^4.1.11, graceful-fs@npm:^4.1.15, graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.4, graceful-fs@npm:^4.2.6, graceful-fs@npm:^4.2.9":
+"graceful-fs@npm:^4.1.11, graceful-fs@npm:^4.1.15, graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.11, graceful-fs@npm:^4.2.4, graceful-fs@npm:^4.2.6, graceful-fs@npm:^4.2.9":
   version: 4.2.11
   resolution: "graceful-fs@npm:4.2.11"
   checksum: ac85f94da92d8eb6b7f5a8b20ce65e43d66761c55ce85ac96df6865308390da45a8d3f0296dd3a663de65d30ba497bd46c696cc1e248c72b13d6d567138a4fc7
   languageName: node
   linkType: hard
 
 "graphemer@npm:^1.4.0":
@@ -7439,19 +7439,19 @@
   version: 2.0.1
   resolution: "has-unicode@npm:2.0.1"
   checksum: 1eab07a7436512db0be40a710b29b5dc21fa04880b7f63c9980b706683127e3c1b57cb80ea96d47991bdae2dfe479604f6a1ba410106ee1046a41d1bd0814400
   languageName: node
   linkType: hard
 
 "hasown@npm:^2.0.0":
-  version: 2.0.1
-  resolution: "hasown@npm:2.0.1"
+  version: 2.0.2
+  resolution: "hasown@npm:2.0.2"
   dependencies:
     function-bind: ^1.1.2
-  checksum: 9081c382a4fe8a62639a8da5c7d3322b203c319147e48783763dd741863d9f2dcaa743574fe2a1283871c445d8ba99ea45d5fff384e5ad27ca9dd7a367d79de0
+  checksum: e8516f776a15149ca6c6ed2ae3110c417a00b62260e222590e54aa367cbcd6ed99122020b37b7fbdf05748df57b265e70095d7bf35a47660587619b15ffb93db
   languageName: node
   linkType: hard
 
 "hosted-git-info@npm:^2.1.4":
   version: 2.8.9
   resolution: "hosted-git-info@npm:2.8.9"
   checksum: c955394bdab888a1e9bb10eb33029e0f7ce5a2ac7b3f158099dc8c486c99e73809dca609f5694b223920ca2174db33d32b12f9a2a47141dc59607c29da5a62dd
@@ -7506,23 +7506,23 @@
 "html-escaper@npm:^2.0.0":
   version: 2.0.2
   resolution: "html-escaper@npm:2.0.2"
   checksum: d2df2da3ad40ca9ee3a39c5cc6475ef67c8f83c234475f24d8e9ce0dc80a2c82df8e1d6fa78ddd1e9022a586ea1bd247a615e80a5cd9273d90111ddda7d9e974
   languageName: node
   linkType: hard
 
-"htmlparser2@npm:^6.0.0":
-  version: 6.1.0
-  resolution: "htmlparser2@npm:6.1.0"
+"htmlparser2@npm:^8.0.0":
+  version: 8.0.2
+  resolution: "htmlparser2@npm:8.0.2"
   dependencies:
-    domelementtype: ^2.0.1
-    domhandler: ^4.0.0
-    domutils: ^2.5.2
-    entities: ^2.0.0
-  checksum: 81a7b3d9c3bb9acb568a02fc9b1b81ffbfa55eae7f1c41ae0bf840006d1dbf54cb3aa245b2553e2c94db674840a9f0fdad7027c9a9d01a062065314039058c4e
+    domelementtype: ^2.3.0
+    domhandler: ^5.0.3
+    domutils: ^3.0.1
+    entities: ^4.4.0
+  checksum: 29167a0f9282f181da8a6d0311b76820c8a59bc9e3c87009e21968264c2987d2723d6fde5a964d4b7b6cba663fca96ffb373c06d8223a85f52a6089ced942700
   languageName: node
   linkType: hard
 
 "http-cache-semantics@npm:^4.1.0, http-cache-semantics@npm:^4.1.1":
   version: 4.1.1
   resolution: "http-cache-semantics@npm:4.1.1"
   checksum: 83ac0bc60b17a3a36f9953e7be55e5c8f41acc61b22583060e8dedc9dd5e3607c823a88d0926f9150e571f90946835c7fe150732801010845c72cd8bbff1a236
@@ -7537,40 +7537,40 @@
     agent-base: 6
     debug: 4
   checksum: e2ee1ff1656a131953839b2a19cd1f3a52d97c25ba87bd2559af6ae87114abf60971e498021f9b73f9fd78aea8876d1fb0d4656aac8a03c6caa9fc175f22b786
   languageName: node
   linkType: hard
 
 "http-proxy-agent@npm:^7.0.0":
-  version: 7.0.1
-  resolution: "http-proxy-agent@npm:7.0.1"
+  version: 7.0.2
+  resolution: "http-proxy-agent@npm:7.0.2"
   dependencies:
     agent-base: ^7.1.0
     debug: ^4.3.4
-  checksum: e8e153dc9106c2a2a05f7a576ea2002ab4a24f2586eeab3947571962532829c0c7cf8a88e67c2cfe2fff9a81deb27e9b5d69452f4a8a1b5d7066a162763e6307
+  checksum: 670858c8f8f3146db5889e1fa117630910101db601fff7d5a8aa637da0abedf68c899f03d3451cac2f83bcc4c3d2dabf339b3aa00ff8080571cceb02c3ce02f3
   languageName: node
   linkType: hard
 
 "https-proxy-agent@npm:^5.0.0, https-proxy-agent@npm:^5.0.1":
   version: 5.0.1
   resolution: "https-proxy-agent@npm:5.0.1"
   dependencies:
     agent-base: 6
     debug: 4
   checksum: 571fccdf38184f05943e12d37d6ce38197becdd69e58d03f43637f7fa1269cf303a7d228aa27e5b27bbd3af8f09fd938e1c91dcfefff2df7ba77c20ed8dfc765
   languageName: node
   linkType: hard
 
 "https-proxy-agent@npm:^7.0.1":
-  version: 7.0.3
-  resolution: "https-proxy-agent@npm:7.0.3"
+  version: 7.0.4
+  resolution: "https-proxy-agent@npm:7.0.4"
   dependencies:
     agent-base: ^7.0.2
     debug: 4
-  checksum: 8aacdde7db31d57674e86e23ecb5f37d79baf54dfc674a44671cb33c1f6a302cc78b2bdf042f6ce37f7c0c61b9b556965cb34f5484880b1864171122dedbdd7d
+  checksum: daaab857a967a2519ddc724f91edbbd388d766ff141b9025b629f92b9408fc83cee8a27e11a907aede392938e9c398e240d643e178408a59e4073539cde8cfe9
   languageName: node
   linkType: hard
 
 "human-signals@npm:^2.1.0":
   version: 2.1.0
   resolution: "human-signals@npm:2.1.0"
   checksum: b87fd89fce72391625271454e70f67fe405277415b48bcc0117ca73d31fa23a4241787afdc8d67f5a116cf37258c052f59ea82daffa72364d61351423848e3b8
@@ -7635,19 +7635,19 @@
   dependencies:
     minimatch: ^5.0.1
   checksum: 1a4ef35174653a1aa6faab3d9f8781269166536aee36a04946f6e2b319b2475c1903a75ed42f04219274128242f49d0a10e20c4354ee60d9548e97031451150b
   languageName: node
   linkType: hard
 
 "ignore-walk@npm:^6.0.0":
-  version: 6.0.4
-  resolution: "ignore-walk@npm:6.0.4"
+  version: 6.0.5
+  resolution: "ignore-walk@npm:6.0.5"
   dependencies:
     minimatch: ^9.0.0
-  checksum: 8161bb3232eee92367049b186a02ad35e3a47edda2de0c0eb216aa89cf6183c33c46aef22b25e1bf5105c643bd2cc2bb722f474870a93a3c56ef8cca22eb64a1
+  checksum: 06f88a53c412385ca7333276149a7e9461b7fad977c44272d854522b0d456c2aa75d832bd3980a530e2c3881126aa9cc4782b3551ca270fffc0ce7c2b4a2e199
   languageName: node
   linkType: hard
 
 "ignore@npm:^5.0.4, ignore@npm:^5.2.0, ignore@npm:^5.2.4":
   version: 5.3.1
   resolution: "ignore@npm:5.3.1"
   checksum: 71d7bb4c1dbe020f915fd881108cbe85a0db3d636a0ea3ba911393c53946711d13a9b1143c7e70db06d571a5822c0a324a6bcde5c9904e7ca5047f01f1bf8cd3
@@ -8044,23 +8044,23 @@
     istanbul-lib-coverage: ^3.2.0
     semver: ^6.3.0
   checksum: bf16f1803ba5e51b28bbd49ed955a736488381e09375d830e42ddeb403855b2006f850711d95ad726f2ba3f1ae8e7366de7e51d2b9ac67dc4d80191ef7ddf272
   languageName: node
   linkType: hard
 
 "istanbul-lib-instrument@npm:^6.0.0":
-  version: 6.0.1
-  resolution: "istanbul-lib-instrument@npm:6.0.1"
+  version: 6.0.2
+  resolution: "istanbul-lib-instrument@npm:6.0.2"
   dependencies:
-    "@babel/core": ^7.12.3
-    "@babel/parser": ^7.14.7
-    "@istanbuljs/schema": ^0.1.2
+    "@babel/core": ^7.23.9
+    "@babel/parser": ^7.23.9
+    "@istanbuljs/schema": ^0.1.3
     istanbul-lib-coverage: ^3.2.0
     semver: ^7.5.4
-  checksum: fb23472e739cfc9b027cefcd7d551d5e7ca7ff2817ae5150fab99fe42786a7f7b56a29a2aa8309c37092e18297b8003f9c274f50ca4360949094d17fbac81472
+  checksum: c10aa1e93a022f9767d7f41e6c07d244cc0a5c090fbb5522d70a5f21fcb98c52b7038850276c6fd1a7a17d1868c14a9d4eb8a24efe58a0ebb9a06f3da68131fe
   languageName: node
   linkType: hard
 
 "istanbul-lib-report@npm:^3.0.0":
   version: 3.0.1
   resolution: "istanbul-lib-report@npm:3.0.1"
   dependencies:
@@ -8079,47 +8079,47 @@
     istanbul-lib-coverage: ^3.0.0
     source-map: ^0.6.1
   checksum: 21ad3df45db4b81852b662b8d4161f6446cd250c1ddc70ef96a585e2e85c26ed7cd9c2a396a71533cfb981d1a645508bc9618cae431e55d01a0628e7dec62ef2
   languageName: node
   linkType: hard
 
 "istanbul-reports@npm:^3.1.3":
-  version: 3.1.6
-  resolution: "istanbul-reports@npm:3.1.6"
+  version: 3.1.7
+  resolution: "istanbul-reports@npm:3.1.7"
   dependencies:
     html-escaper: ^2.0.0
     istanbul-lib-report: ^3.0.0
-  checksum: 44c4c0582f287f02341e9720997f9e82c071627e1e862895745d5f52ec72c9b9f38e1d12370015d2a71dcead794f34c7732aaef3fab80a24bc617a21c3d911d6
+  checksum: 2072db6e07bfbb4d0eb30e2700250636182398c1af811aea5032acb219d2080f7586923c09fa194029efd6b92361afb3dcbe1ebcc3ee6651d13340f7c6c4ed95
   languageName: node
   linkType: hard
 
-"jackspeak@npm:^2.3.5":
+"jackspeak@npm:^2.3.6":
   version: 2.3.6
   resolution: "jackspeak@npm:2.3.6"
   dependencies:
     "@isaacs/cliui": ^8.0.2
     "@pkgjs/parseargs": ^0.11.0
   dependenciesMeta:
     "@pkgjs/parseargs":
       optional: true
   checksum: 57d43ad11eadc98cdfe7496612f6bbb5255ea69fe51ea431162db302c2a11011642f50cfad57288bd0aea78384a0612b16e131944ad8ecd09d619041c8531b54
   languageName: node
   linkType: hard
 
 "jake@npm:^10.8.5":
-  version: 10.8.7
-  resolution: "jake@npm:10.8.7"
+  version: 10.9.1
+  resolution: "jake@npm:10.9.1"
   dependencies:
     async: ^3.2.3
     chalk: ^4.0.2
     filelist: ^1.0.4
     minimatch: ^3.1.2
   bin:
     jake: bin/cli.js
-  checksum: a23fd2273fb13f0d0d845502d02c791fd55ef5c6a2d207df72f72d8e1eac6d2b8ffa6caf660bc8006b3242e0daaa88a3ecc600194d72b5c6016ad56e9cd43553
+  checksum: 49659c156b8ad921af377fb782505ae3cc7e7dd8793695b782070d99b4b66d2688b4e3efb32e09252400bfe6e49a7fb393a3a0959e8e1a51dbda95bcacbb9c36
   languageName: node
   linkType: hard
 
 "jest-changed-files@npm:^29.7.0":
   version: 29.7.0
   resolution: "jest-changed-files@npm:29.7.0"
   dependencies:
@@ -8714,17 +8714,17 @@
   version: 2.3.1
   resolution: "json-parse-even-better-errors@npm:2.3.1"
   checksum: 798ed4cf3354a2d9ccd78e86d2169515a0097a5c133337807cdf7f1fc32e1391d207ccfc276518cc1d7d8d4db93288b8a50ba4293d212ad1336e52a8ec0a941f
   languageName: node
   linkType: hard
 
 "json-parse-even-better-errors@npm:^3.0.0":
-  version: 3.0.1
-  resolution: "json-parse-even-better-errors@npm:3.0.1"
-  checksum: bf74fa3f715e56699ccd68b80a7d20908de432a3fae2d5aa2ed530a148e9d9ccdf8e6983b93d9966a553aa70dcf003ce3a7ffec2c0ce74d2a6173e3691a426f0
+  version: 3.0.2
+  resolution: "json-parse-even-better-errors@npm:3.0.2"
+  checksum: 6f04ea6c9ccb783630a59297959247e921cc90b917b8351197ca7fd058fccc7079268fd9362be21ba876fc26aa5039369dd0a2280aae49aae425784794a94927
   languageName: node
   linkType: hard
 
 "json-schema-compare@npm:^0.2.2":
   version: 0.2.2
   resolution: "json-schema-compare@npm:0.2.2"
   dependencies:
@@ -8959,22 +8959,23 @@
     prelude-ls: ^1.2.1
     type-check: ~0.4.0
   checksum: 12c5021c859bd0f5248561bf139121f0358285ec545ebf48bb3d346820d5c61a4309535c7f387ed7d84361cf821e124ce346c6b7cef8ee09a67c1473b46d0fc4
   languageName: node
   linkType: hard
 
 "lib0@npm:^0.2.85, lib0@npm:^0.2.86":
-  version: 0.2.88
-  resolution: "lib0@npm:0.2.88"
+  version: 0.2.94
+  resolution: "lib0@npm:0.2.94"
   dependencies:
     isomorphic.js: ^0.2.4
   bin:
+    0ecdsa-generate-keypair: bin/0ecdsa-generate-keypair.js
     0gentesthtml: bin/gentesthtml.js
     0serve: bin/0serve.js
-  checksum: 1ac13d6781f4d29aa317ad9fb9b6c41e8bed52b096a369f54d10d9b8651ceb4a0a63b06c01c2e1c7319d3bb74668afb6cac3735161b32031f185cec024bbba37
+  checksum: b091c7b39875a58d92ae6dcb014a42b56caf1336e03d310403c47a2fcea079eba92ffb43da90eaff9d010f08bcd20de35fffed7c655c83312ff4e3477f5dc261
   languageName: node
   linkType: hard
 
 "libnpmaccess@npm:^6.0.3":
   version: 6.0.4
   resolution: "libnpmaccess@npm:6.0.4"
   dependencies:
@@ -9199,18 +9200,18 @@
     js-tokens: ^3.0.0 || ^4.0.0
   bin:
     loose-envify: cli.js
   checksum: 6517e24e0cad87ec9888f500c5b5947032cdfe6ef65e1c1936a0c48a524b81e65542c9c3edc91c97d5bddc806ee2a985dbc79be89215d613b1de5db6d1cfe6f4
   languageName: node
   linkType: hard
 
-"lru-cache@npm:^10.0.1, lru-cache@npm:^9.1.1 || ^10.0.0":
-  version: 10.2.0
-  resolution: "lru-cache@npm:10.2.0"
-  checksum: eee7ddda4a7475deac51ac81d7dd78709095c6fa46e8350dc2d22462559a1faa3b81ed931d5464b13d48cbd7e08b46100b6f768c76833912bc444b99c37e25db
+"lru-cache@npm:^10.0.1, lru-cache@npm:^10.2.0":
+  version: 10.2.2
+  resolution: "lru-cache@npm:10.2.2"
+  checksum: 98e8fc93691c546f719a76103ef2bee5a3ac823955c755a47641ec41f8c7fafa1baeaba466937cc1cbfa9cfd47e03536d10e2db3158a64ad91ff3a58a32c893e
   languageName: node
   linkType: hard
 
 "lru-cache@npm:^5.1.1":
   version: 5.1.1
   resolution: "lru-cache@npm:5.1.1"
   dependencies:
@@ -9314,29 +9315,30 @@
     socks-proxy-agent: ^7.0.0
     ssri: ^10.0.0
   checksum: 7268bf274a0f6dcf0343829489a4506603ff34bd0649c12058753900b0eb29191dce5dba12680719a5d0a983d3e57810f594a12f3c18494e93a1fbc6348a4540
   languageName: node
   linkType: hard
 
 "make-fetch-happen@npm:^13.0.0":
-  version: 13.0.0
-  resolution: "make-fetch-happen@npm:13.0.0"
+  version: 13.0.1
+  resolution: "make-fetch-happen@npm:13.0.1"
   dependencies:
     "@npmcli/agent": ^2.0.0
     cacache: ^18.0.0
     http-cache-semantics: ^4.1.1
     is-lambda: ^1.0.1
     minipass: ^7.0.2
     minipass-fetch: ^3.0.0
     minipass-flush: ^1.0.5
     minipass-pipeline: ^1.2.4
     negotiator: ^0.6.3
+    proc-log: ^4.2.0
     promise-retry: ^2.0.1
     ssri: ^10.0.0
-  checksum: 7c7a6d381ce919dd83af398b66459a10e2fe8f4504f340d1d090d3fa3d1b0c93750220e1d898114c64467223504bd258612ba83efbc16f31b075cd56de24b4af
+  checksum: 5c9fad695579b79488fa100da05777213dd9365222f85e4757630f8dd2a21a79ddd3206c78cfd6f9b37346819681782b67900ac847a57cf04190f52dda5343fd
   languageName: node
   linkType: hard
 
 "makeerror@npm:1.0.12":
   version: 1.0.12
   resolution: "makeerror@npm:1.0.12"
   dependencies:
@@ -9356,19 +9358,19 @@
   version: 4.3.0
   resolution: "map-obj@npm:4.3.0"
   checksum: fbc554934d1a27a1910e842bc87b177b1a556609dd803747c85ece420692380827c6ae94a95cce4407c054fa0964be3bf8226f7f2cb2e9eeee432c7c1985684e
   languageName: node
   linkType: hard
 
 "markdown-to-jsx@npm:^7.4.1":
-  version: 7.4.1
-  resolution: "markdown-to-jsx@npm:7.4.1"
+  version: 7.4.7
+  resolution: "markdown-to-jsx@npm:7.4.7"
   peerDependencies:
     react: ">= 0.14.0"
-  checksum: 2888cb2389cb810ab35454a59d0623474a60a78e28f281ae0081f87053f6c59b033232a2cd269cc383a5edcaa1eab8ca4b3cf639fe4e1aa3fb418648d14bcc7d
+  checksum: bb8a696c8a95dd67ac1eb44255f31cf17e60b6c2ff03bfcd51b5e28da17856c57d7a16da59fda7f3a4eedb01d7e92eeef57a10ff3abd5431e5c80059d4565016
   languageName: node
   linkType: hard
 
 "meow@npm:^8.0.0":
   version: 8.1.2
   resolution: "meow@npm:8.1.2"
   dependencies:
@@ -9398,20 +9400,20 @@
   version: 1.4.1
   resolution: "merge2@npm:1.4.1"
   checksum: 7268db63ed5169466540b6fb947aec313200bcf6d40c5ab722c22e242f651994619bcd85601602972d3c85bd2cc45a358a4c61937e9f11a061919a1da569b0c2
   languageName: node
   linkType: hard
 
 "micromatch@npm:^4.0.4":
-  version: 4.0.5
-  resolution: "micromatch@npm:4.0.5"
+  version: 4.0.6
+  resolution: "micromatch@npm:4.0.6"
   dependencies:
-    braces: ^3.0.2
-    picomatch: ^2.3.1
-  checksum: 02a17b671c06e8fefeeb6ef996119c1e597c942e632a21ef589154f23898c9c6a9858526246abb14f8bca6e77734aa9dcf65476fca47cedfb80d9577d52843fc
+    braces: ^3.0.3
+    picomatch: ^4.0.2
+  checksum: cd44a850c638d82232608e2a03677c5828b9faf35bacfd4817ae232208e2a56bac97bceb67da6a5d4d5a603c1cc88f65ecae3af6be11b5a8c10c995515231e78
   languageName: node
   linkType: hard
 
 "mime-db@npm:1.52.0":
   version: 1.52.0
   resolution: "mime-db@npm:1.52.0"
   checksum: 0d99a03585f8b39d68182803b12ac601d9c01abfa28ec56204fa330bc9f3d1c5e14beb049bafadb3dbdf646dfb94b87e24d4ec7b31b7279ef906a8ea9b6a513f
@@ -9447,22 +9449,22 @@
   version: 1.0.1
   resolution: "min-indent@npm:1.0.1"
   checksum: bfc6dd03c5eaf623a4963ebd94d087f6f4bbbfd8c41329a7f09706b0cb66969c4ddd336abeb587bc44bc6f08e13bf90f0b374f9d71f9f01e04adc2cd6f083ef1
   languageName: node
   linkType: hard
 
 "mini-css-extract-plugin@npm:^2.7.0":
-  version: 2.8.0
-  resolution: "mini-css-extract-plugin@npm:2.8.0"
+  version: 2.9.0
+  resolution: "mini-css-extract-plugin@npm:2.9.0"
   dependencies:
     schema-utils: ^4.0.0
     tapable: ^2.2.1
   peerDependencies:
     webpack: ^5.0.0
-  checksum: c1edc3ee0e1b3514c3323fa72ad38e993f357964e76737f1d7bb6cf50a0af1ac071080ec16b4e1a94688d23f78533944badad50cd0f00d2ae176f9c58c1f2029
+  checksum: ae192c67ba85ac8bffeab66774635bf90181f00d5dd6cf95412426192599ddf5506fb4b1550acbd7a5476476e39db53c770dd40f8378f7baf5de96e3fec4e6e9
   languageName: node
   linkType: hard
 
 "mini-svg-data-uri@npm:^1.4.4":
   version: 1.4.4
   resolution: "mini-svg-data-uri@npm:1.4.4"
   bin:
@@ -9476,15 +9478,15 @@
   resolution: "minimatch@npm:3.0.5"
   dependencies:
     brace-expansion: ^1.1.7
   checksum: a3b84b426eafca947741b864502cee02860c4e7b145de11ad98775cfcf3066fef422583bc0ffce0952ddf4750c1ccf4220b1556430d4ce10139f66247d87d69e
   languageName: node
   linkType: hard
 
-"minimatch@npm:9.0.3, minimatch@npm:^9.0.0, minimatch@npm:^9.0.1":
+"minimatch@npm:9.0.3":
   version: 9.0.3
   resolution: "minimatch@npm:9.0.3"
   dependencies:
     brace-expansion: ^2.0.1
   checksum: 253487976bf485b612f16bf57463520a14f512662e592e95c571afdab1442a6a6864b6c88f248ce6fc4ff0b6de04ac7aa6c8bb51e868e99d1d65eb0658a708b5
   languageName: node
   linkType: hard
@@ -9521,14 +9523,23 @@
   resolution: "minimatch@npm:8.0.4"
   dependencies:
     brace-expansion: ^2.0.1
   checksum: 2e46cffb86bacbc524ad45a6426f338920c529dd13f3a732cc2cf7618988ee1aae88df4ca28983285aca9e0f45222019ac2d14ebd17c1edadd2ee12221ab801a
   languageName: node
   linkType: hard
 
+"minimatch@npm:^9.0.0, minimatch@npm:^9.0.1":
+  version: 9.0.4
+  resolution: "minimatch@npm:9.0.4"
+  dependencies:
+    brace-expansion: ^2.0.1
+  checksum: cf717f597ec3eed7dabc33153482a2e8d49f4fd3c26e58fd9c71a94c5029a0838728841b93f46bf1263b65a8010e2ee800d0dc9b004ab8ba8b6d1ec07cc115b5
+  languageName: node
+  linkType: hard
+
 "minimist-options@npm:4.1.0":
   version: 4.1.0
   resolution: "minimist-options@npm:4.1.0"
   dependencies:
     arrify: ^1.0.1
     is-plain-obj: ^1.1.0
     kind-of: ^6.0.3
@@ -9573,25 +9584,25 @@
     encoding:
       optional: true
   checksum: 3f216be79164e915fc91210cea1850e488793c740534985da017a4cbc7a5ff50506956d0f73bb0cb60e4fe91be08b6b61ef35101706d3ef5da2c8709b5f08f91
   languageName: node
   linkType: hard
 
 "minipass-fetch@npm:^3.0.0":
-  version: 3.0.4
-  resolution: "minipass-fetch@npm:3.0.4"
+  version: 3.0.5
+  resolution: "minipass-fetch@npm:3.0.5"
   dependencies:
     encoding: ^0.1.13
     minipass: ^7.0.3
     minipass-sized: ^1.0.3
     minizlib: ^2.1.2
   dependenciesMeta:
     encoding:
       optional: true
-  checksum: af7aad15d5c128ab1ebe52e043bdf7d62c3c6f0cecb9285b40d7b395e1375b45dcdfd40e63e93d26a0e8249c9efd5c325c65575aceee192883970ff8cb11364a
+  checksum: 8047d273236157aab27ab7cd8eab7ea79e6ecd63e8f80c3366ec076cb9a0fed550a6935bab51764369027c414647fd8256c2a20c5445fb250c483de43350de83
   languageName: node
   linkType: hard
 
 "minipass-flush@npm:^1.0.5":
   version: 1.0.5
   resolution: "minipass-flush@npm:1.0.5"
   dependencies:
@@ -9647,18 +9658,18 @@
 "minipass@npm:^5.0.0":
   version: 5.0.0
   resolution: "minipass@npm:5.0.0"
   checksum: 425dab288738853fded43da3314a0b5c035844d6f3097a8e3b5b29b328da8f3c1af6fc70618b32c29ff906284cf6406b6841376f21caaadd0793c1d5a6a620ea
   languageName: node
   linkType: hard
 
-"minipass@npm:^5.0.0 || ^6.0.2 || ^7.0.0, minipass@npm:^7.0.2, minipass@npm:^7.0.3":
-  version: 7.0.4
-  resolution: "minipass@npm:7.0.4"
-  checksum: 87585e258b9488caf2e7acea242fd7856bbe9a2c84a7807643513a338d66f368c7d518200ad7b70a508664d408aa000517647b2930c259a8b1f9f0984f344a21
+"minipass@npm:^5.0.0 || ^6.0.2 || ^7.0.0, minipass@npm:^7.0.2, minipass@npm:^7.0.3, minipass@npm:^7.0.4":
+  version: 7.1.1
+  resolution: "minipass@npm:7.1.1"
+  checksum: d2c461947a7530f93de4162aa3ca0a1bed1f121626906f6ec63a5ba05fd7b1d9bee4fe89a37a43db7241c2416be98a799c1796abae583c7180be37be5c392ef6
   languageName: node
   linkType: hard
 
 "minizlib@npm:^2.1.1, minizlib@npm:^2.1.2":
   version: 2.1.2
   resolution: "minizlib@npm:2.1.2"
   dependencies:
@@ -9785,36 +9796,36 @@
   peerDependenciesMeta:
     encoding:
       optional: true
   checksum: 8d816ffd1ee22cab8301c7756ef04f3437f18dace86a1dae22cf81db8ef29c0bf6655f3215cb0cdb22b420b6fe141e64b26905e7f33f9377a7fa59135ea3e10b
   languageName: node
   linkType: hard
 
-"node-fetch@npm:^2.6.0, node-fetch@npm:^2.6.7":
+"node-fetch@npm:^2.6.7":
   version: 2.7.0
   resolution: "node-fetch@npm:2.7.0"
   dependencies:
     whatwg-url: ^5.0.0
   peerDependencies:
     encoding: ^0.1.0
   peerDependenciesMeta:
     encoding:
       optional: true
   checksum: d76d2f5edb451a3f05b15115ec89fc6be39de37c6089f1b6368df03b91e1633fd379a7e01b7ab05089a25034b2023d959b47e59759cb38d88341b2459e89d6e5
   languageName: node
   linkType: hard
 
 "node-gyp-build@npm:^4.3.0":
-  version: 4.8.0
-  resolution: "node-gyp-build@npm:4.8.0"
+  version: 4.8.1
+  resolution: "node-gyp-build@npm:4.8.1"
   bin:
     node-gyp-build: bin.js
     node-gyp-build-optional: optional.js
     node-gyp-build-test: build-test.js
-  checksum: b82a56f866034b559dd3ed1ad04f55b04ae381b22ec2affe74b488d1582473ca6e7f85fccf52da085812d3de2b0bf23109e752a57709ac7b9963951c710fea40
+  checksum: fe6e95da6f4608c1a98655f6bf2fe4e8dd9c877cd13256056a8acaf585cc7f98718823fe9366be11b78c2f332d5a184b00cf07a4af96c9d8fea45f640c019f98
   languageName: node
   linkType: hard
 
 "node-gyp@npm:^9.0.0":
   version: 9.4.1
   resolution: "node-gyp@npm:9.4.1"
   dependencies:
@@ -9832,30 +9843,30 @@
   bin:
     node-gyp: bin/node-gyp.js
   checksum: 8576c439e9e925ab50679f87b7dfa7aa6739e42822e2ad4e26c36341c0ba7163fdf5a946f0a67a476d2f24662bc40d6c97bd9e79ced4321506738e6b760a1577
   languageName: node
   linkType: hard
 
 "node-gyp@npm:latest":
-  version: 10.0.1
-  resolution: "node-gyp@npm:10.0.1"
+  version: 10.1.0
+  resolution: "node-gyp@npm:10.1.0"
   dependencies:
     env-paths: ^2.2.0
     exponential-backoff: ^3.1.1
     glob: ^10.3.10
     graceful-fs: ^4.2.6
     make-fetch-happen: ^13.0.0
     nopt: ^7.0.0
     proc-log: ^3.0.0
     semver: ^7.3.5
     tar: ^6.1.2
     which: ^4.0.0
   bin:
     node-gyp: bin/node-gyp.js
-  checksum: 60a74e66d364903ce02049966303a57f898521d139860ac82744a5fdd9f7b7b3b61f75f284f3bfe6e6add3b8f1871ce305a1d41f775c7482de837b50c792223f
+  checksum: 72e2ab4b23fc32007a763da94018f58069fc0694bf36115d49a2b195c8831e12cf5dd1e7a3718fa85c06969aedf8fc126722d3b672ec1cb27e06ed33caee3c60
   languageName: node
   linkType: hard
 
 "node-int64@npm:^0.4.0":
   version: 0.4.0
   resolution: "node-int64@npm:0.4.0"
   checksum: d0b30b1ee6d961851c60d5eaa745d30b5c95d94bc0e74b81e5292f7c42a49e3af87f1eb9e89f59456f80645d679202537de751b7d72e9e40ceea40c5e449057e
@@ -9877,21 +9888,21 @@
   bin:
     nopt: bin/nopt.js
   checksum: 82149371f8be0c4b9ec2f863cc6509a7fd0fa729929c009f3a58e4eb0c9e4cae9920e8f1f8eb46e7d032fec8fb01bede7f0f41a67eb3553b7b8e14fa53de1dac
   languageName: node
   linkType: hard
 
 "nopt@npm:^7.0.0":
-  version: 7.2.0
-  resolution: "nopt@npm:7.2.0"
+  version: 7.2.1
+  resolution: "nopt@npm:7.2.1"
   dependencies:
     abbrev: ^2.0.0
   bin:
     nopt: bin/nopt.js
-  checksum: a9c0f57fb8cb9cc82ae47192ca2b7ef00e199b9480eed202482c962d61b59a7fbe7541920b2a5839a97b42ee39e288c0aed770e38057a608d7f579389dfde410
+  checksum: 6fa729cc77ce4162cfad8abbc9ba31d4a0ff6850c3af61d59b505653bef4781ec059f8890ecfe93ee8aa0c511093369cca88bfc998101616a2904e715bbbb7c9
   languageName: node
   linkType: hard
 
 "normalize-package-data@npm:^2.3.2, normalize-package-data@npm:^2.5.0":
   version: 2.5.0
   resolution: "normalize-package-data@npm:2.5.0"
   dependencies:
@@ -9952,19 +9963,19 @@
   dependencies:
     npm-normalize-package-bin: ^1.0.1
   checksum: 6e599155ef28d0b498622f47f1ba189dfbae05095a1ed17cb3a5babf961e965dd5eab621f0ec6f0a98de774e5836b8f5a5ee639010d64f42850a74acec3d4d09
   languageName: node
   linkType: hard
 
 "npm-bundled@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "npm-bundled@npm:3.0.0"
+  version: 3.0.1
+  resolution: "npm-bundled@npm:3.0.1"
   dependencies:
     npm-normalize-package-bin: ^3.0.0
-  checksum: 110859c2d6dcd7941dac0932a29171cbde123060486a4b6e897aaf5e025abeb3d9ffcdfe9e9271992e6396b2986c2c534f1029a45a7c196f1257fa244305dbf8
+  checksum: 1f4f7307d0ff2fbd31638689490f1fd673a4540cd1d027c7c5d15e484c71d63c4b27979944b6f8738035260cf5a5477ebaae75b08818420508e7cf317d71416e
   languageName: node
   linkType: hard
 
 "npm-install-checks@npm:^6.0.0":
   version: 6.3.0
   resolution: "npm-install-checks@npm:6.3.0"
   dependencies:
@@ -10139,17 +10150,17 @@
     gauge: ^5.0.0
     set-blocking: ^2.0.0
   checksum: caabeb1f557c1094ad7ed3275b968b83ccbaefc133f17366ebb9fe8eb44e1aace28c31419d6244bfc0422aede1202875d555fe6661978bf04386f6cf617f43a4
   languageName: node
   linkType: hard
 
 "nwsapi@npm:^2.2.2":
-  version: 2.2.7
-  resolution: "nwsapi@npm:2.2.7"
-  checksum: cab25f7983acec7e23490fec3ef7be608041b460504229770e3bfcf9977c41d6fe58f518994d3bd9aa3a101f501089a3d4a63536f4ff8ae4b8c4ca23bdbfda4e
+  version: 2.2.10
+  resolution: "nwsapi@npm:2.2.10"
+  checksum: 5f1d361b38c47ab49727d5ea8bbfeb5867ae6de0e538eec9a8b77c88005ddde36d8b930e0730b50ee5e5dda949112c0f9ffed1bf15e7e1b3cd9cfa319f5a9b6f
   languageName: node
   linkType: hard
 
 "nx@npm:15.9.7, nx@npm:>=15.5.2 < 16":
   version: 15.9.7
   resolution: "nx@npm:15.9.7"
   dependencies:
@@ -10270,24 +10281,24 @@
     is-docker: ^2.1.1
     is-wsl: ^2.2.0
   checksum: 6388bfff21b40cb9bd8f913f9130d107f2ed4724ea81a8fd29798ee322b361ca31fa2cdfb491a5c31e43a3996cfe9566741238c7a741ada8d7af1cb78d85cf26
   languageName: node
   linkType: hard
 
 "optionator@npm:^0.9.3":
-  version: 0.9.3
-  resolution: "optionator@npm:0.9.3"
+  version: 0.9.4
+  resolution: "optionator@npm:0.9.4"
   dependencies:
-    "@aashutoshrathi/word-wrap": ^1.2.3
     deep-is: ^0.1.3
     fast-levenshtein: ^2.0.6
     levn: ^0.4.1
     prelude-ls: ^1.2.1
     type-check: ^0.4.0
-  checksum: 09281999441f2fe9c33a5eeab76700795365a061563d66b098923eb719251a42bdbe432790d35064d0816ead9296dbeb1ad51a733edf4167c96bd5d0882e428a
+    word-wrap: ^1.2.5
+  checksum: ecbd010e3dc73e05d239976422d9ef54a82a13f37c11ca5911dff41c98a6c7f0f163b27f922c37e7f8340af9d36febd3b6e9cef508f3339d4c393d7276d716bb
   languageName: node
   linkType: hard
 
 "ora@npm:^5.4.1":
   version: 5.4.1
   resolution: "ora@npm:5.4.1"
   dependencies:
@@ -10614,21 +10625,21 @@
 "path-parse@npm:^1.0.7":
   version: 1.0.7
   resolution: "path-parse@npm:1.0.7"
   checksum: 49abf3d81115642938a8700ec580da6e830dde670be21893c62f4e10bd7dd4c3742ddc603fe24f898cba7eb0c6bc1777f8d9ac14185d34540c6d4d80cd9cae8a
   languageName: node
   linkType: hard
 
-"path-scurry@npm:^1.10.1, path-scurry@npm:^1.6.1":
-  version: 1.10.1
-  resolution: "path-scurry@npm:1.10.1"
+"path-scurry@npm:^1.11.0, path-scurry@npm:^1.6.1":
+  version: 1.11.1
+  resolution: "path-scurry@npm:1.11.1"
   dependencies:
-    lru-cache: ^9.1.1 || ^10.0.0
+    lru-cache: ^10.2.0
     minipass: ^5.0.0 || ^6.0.2 || ^7.0.0
-  checksum: e2557cff3a8fb8bc07afdd6ab163a92587884f9969b05bbbaf6fe7379348bfb09af9ed292af12ed32398b15fb443e81692047b786d1eeb6d898a51eb17ed7d90
+  checksum: 890d5abcd593a7912dcce7cf7c6bf7a0b5648e3dee6caf0712c126ca0a65c7f3d7b9d769072a4d1baf370f61ce493ab5b038d59988688e0c5f3f646ee3c69023
   languageName: node
   linkType: hard
 
 "path-type@npm:^3.0.0":
   version: 3.0.0
   resolution: "path-type@npm:3.0.0"
   dependencies:
@@ -10640,28 +10651,35 @@
 "path-type@npm:^4.0.0":
   version: 4.0.0
   resolution: "path-type@npm:4.0.0"
   checksum: 5b1e2daa247062061325b8fdbfd1fb56dde0a448fb1455453276ea18c60685bdad23a445dc148cf87bc216be1573357509b7d4060494a6fd768c7efad833ee45
   languageName: node
   linkType: hard
 
-"picocolors@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "picocolors@npm:1.0.0"
-  checksum: a2e8092dd86c8396bdba9f2b5481032848525b3dc295ce9b57896f931e63fc16f79805144321f72976383fc249584672a75cc18d6777c6b757603f372f745981
+"picocolors@npm:^1.0.0, picocolors@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "picocolors@npm:1.0.1"
+  checksum: fa68166d1f56009fc02a34cdfd112b0dd3cf1ef57667ac57281f714065558c01828cdf4f18600ad6851cbe0093952ed0660b1e0156bddf2184b6aaf5817553a5
   languageName: node
   linkType: hard
 
-"picomatch@npm:^2.0.4, picomatch@npm:^2.2.3, picomatch@npm:^2.3.1":
+"picomatch@npm:^2.0.4, picomatch@npm:^2.2.3":
   version: 2.3.1
   resolution: "picomatch@npm:2.3.1"
   checksum: 050c865ce81119c4822c45d3c84f1ced46f93a0126febae20737bd05ca20589c564d6e9226977df859ed5e03dc73f02584a2b0faad36e896936238238b0446cf
   languageName: node
   linkType: hard
 
+"picomatch@npm:^4.0.2":
+  version: 4.0.2
+  resolution: "picomatch@npm:4.0.2"
+  checksum: a7a5188c954f82c6585720e9143297ccd0e35ad8072231608086ca950bee672d51b0ef676254af0788205e59bd4e4deb4e7708769226bed725bf13370a7d1464
+  languageName: node
+  linkType: hard
+
 "pify@npm:5.0.0, pify@npm:^5.0.0":
   version: 5.0.0
   resolution: "pify@npm:5.0.0"
   checksum: 443e3e198ad6bfa8c0c533764cf75c9d5bc976387a163792fb553ffe6ce923887cf14eebf5aea9b7caa8eab930da8c33612990ae85bd8c2bc18bedb9eae94ecb
   languageName: node
   linkType: hard
 
@@ -10698,44 +10716,44 @@
   resolution: "pkg-dir@npm:4.2.0"
   dependencies:
     find-up: ^4.0.0
   checksum: 9863e3f35132bf99ae1636d31ff1e1e3501251d480336edb1c211133c8d58906bed80f154a1d723652df1fda91e01c7442c2eeaf9dc83157c7ae89087e43c8d6
   languageName: node
   linkType: hard
 
-"postcss-modules-extract-imports@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "postcss-modules-extract-imports@npm:3.0.0"
+"postcss-modules-extract-imports@npm:^3.1.0":
+  version: 3.1.0
+  resolution: "postcss-modules-extract-imports@npm:3.1.0"
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 4b65f2f1382d89c4bc3c0a1bdc5942f52f3cb19c110c57bd591ffab3a5fee03fcf831604168205b0c1b631a3dce2255c70b61aaae3ef39d69cd7eb450c2552d2
+  checksum: b9192e0f4fb3d19431558be6f8af7ca45fc92baaad9b2778d1732a5880cd25c3df2074ce5484ae491e224f0d21345ffc2d419bd51c25b019af76d7a7af88c17f
   languageName: node
   linkType: hard
 
-"postcss-modules-local-by-default@npm:^4.0.4":
-  version: 4.0.4
-  resolution: "postcss-modules-local-by-default@npm:4.0.4"
+"postcss-modules-local-by-default@npm:^4.0.5":
+  version: 4.0.5
+  resolution: "postcss-modules-local-by-default@npm:4.0.5"
   dependencies:
     icss-utils: ^5.0.0
     postcss-selector-parser: ^6.0.2
     postcss-value-parser: ^4.1.0
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 578b955b0773147890caa88c30b10dfc849c5b1412a47ad51751890dba16fca9528c3ab00a19b186a8c2c150c2d08e2ce64d3d907800afee1f37c6d38252e365
+  checksum: ca9b01f4a0a3dfb33e016299e2dfb7e85c3123292f7aec2efc0c6771b9955648598bfb4c1561f7ee9732fb27fb073681233661b32eef98baab43743f96735452
   languageName: node
   linkType: hard
 
-"postcss-modules-scope@npm:^3.1.1":
-  version: 3.1.1
-  resolution: "postcss-modules-scope@npm:3.1.1"
+"postcss-modules-scope@npm:^3.2.0":
+  version: 3.2.0
+  resolution: "postcss-modules-scope@npm:3.2.0"
   dependencies:
     postcss-selector-parser: ^6.0.4
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 9e9d23abb0babc7fa243be65704d72a5a9ceb2bded4dbaef96a88210d468b03c8c3158c197f4e22300c851f08c6fdddd6ebe65f44e4c34448b45b8a2e063a16d
+  checksum: 2ffe7e98c1fa993192a39c8dd8ade93fc4f59fbd1336ce34fcedaee0ee3bafb29e2e23fb49189256895b30e4f21af661c6a6a16ef7b17ae2c859301e4a4459ae
   languageName: node
   linkType: hard
 
 "postcss-modules-values@npm:^4.0.0":
   version: 4.0.0
   resolution: "postcss-modules-values@npm:4.0.0"
   dependencies:
@@ -10743,38 +10761,38 @@
   peerDependencies:
     postcss: ^8.1.0
   checksum: f7f2cdf14a575b60e919ad5ea52fed48da46fe80db2733318d71d523fc87db66c835814940d7d05b5746b0426e44661c707f09bdb83592c16aea06e859409db6
   languageName: node
   linkType: hard
 
 "postcss-selector-parser@npm:^6.0.10, postcss-selector-parser@npm:^6.0.2, postcss-selector-parser@npm:^6.0.4":
-  version: 6.0.15
-  resolution: "postcss-selector-parser@npm:6.0.15"
+  version: 6.0.16
+  resolution: "postcss-selector-parser@npm:6.0.16"
   dependencies:
     cssesc: ^3.0.0
     util-deprecate: ^1.0.2
-  checksum: 57decb94152111004f15e27b9c61131eb50ee10a3288e7fcf424cebbb4aba82c2817517ae718f8b5d704ee9e02a638d4a2acff8f47685c295a33ecee4fd31055
+  checksum: e1cd68e33a39e3dc1e1e5bd8717be5bbe3cc23a4cecb466c3acb2f3a77daad7a47df4d6137a76f8db74cf160d2fb16b2cfdb4ccbebdfda844690f8d545fe281d
   languageName: node
   linkType: hard
 
 "postcss-value-parser@npm:^4.1.0, postcss-value-parser@npm:^4.2.0":
   version: 4.2.0
   resolution: "postcss-value-parser@npm:4.2.0"
   checksum: 819ffab0c9d51cf0acbabf8996dffbfafbafa57afc0e4c98db88b67f2094cb44488758f06e5da95d7036f19556a4a732525e84289a425f4f6fd8e412a9d7442f
   languageName: node
   linkType: hard
 
 "postcss@npm:^8.3.11, postcss@npm:^8.4.33":
-  version: 8.4.35
-  resolution: "postcss@npm:8.4.35"
+  version: 8.4.38
+  resolution: "postcss@npm:8.4.38"
   dependencies:
     nanoid: ^3.3.7
     picocolors: ^1.0.0
-    source-map-js: ^1.0.2
-  checksum: cf3c3124d3912a507603f6d9a49b3783f741075e9aa73eb592a6dd9194f9edab9d20a8875d16d137d4f779fe7b6fbd1f5727e39bfd1c3003724980ee4995e1da
+    source-map-js: ^1.2.0
+  checksum: 649f9e60a763ca4b5a7bbec446a069edf07f057f6d780a5a0070576b841538d1ecf7dd888f2fbfd1f76200e26c969e405aeeae66332e6927dbdc8bdcb90b9451
   languageName: node
   linkType: hard
 
 "prelude-ls@npm:^1.2.1":
   version: 1.2.1
   resolution: "prelude-ls@npm:1.2.1"
   checksum: cd192ec0d0a8e4c6da3bb80e4f62afe336df3f76271ac6deb0e6a36187133b6073a19e9727a1ff108cd8b9982e4768850d413baa71214dd80c7979617dca827a
@@ -10831,14 +10849,21 @@
 "proc-log@npm:^3.0.0":
   version: 3.0.0
   resolution: "proc-log@npm:3.0.0"
   checksum: 02b64e1b3919e63df06f836b98d3af002b5cd92655cab18b5746e37374bfb73e03b84fe305454614b34c25b485cc687a9eebdccf0242cda8fda2475dd2c97e02
   languageName: node
   linkType: hard
 
+"proc-log@npm:^4.2.0":
+  version: 4.2.0
+  resolution: "proc-log@npm:4.2.0"
+  checksum: 98f6cd012d54b5334144c5255ecb941ee171744f45fca8b43b58ae5a0c1af07352475f481cadd9848e7f0250376ee584f6aa0951a856ff8f021bdfbff4eb33fc
+  languageName: node
+  linkType: hard
+
 "process-nextick-args@npm:~2.0.0":
   version: 2.0.1
   resolution: "process-nextick-args@npm:2.0.1"
   checksum: 1d38588e520dab7cea67cbbe2efdd86a10cc7a074c09657635e34f035277b59fbb57d09d8638346bf7090f8e8ebc070c96fa5fd183b777fff4f5edff5e9466cf
   languageName: node
   linkType: hard
 
@@ -10942,17 +10967,17 @@
   version: 2.3.1
   resolution: "punycode@npm:2.3.1"
   checksum: bb0a0ceedca4c3c57a9b981b90601579058903c62be23c5e8e843d2c2d4148a3ecf029d5133486fb0e1822b098ba8bba09e89d6b21742d02fa26bda6441a6fb2
   languageName: node
   linkType: hard
 
 "pure-rand@npm:^6.0.0":
-  version: 6.0.4
-  resolution: "pure-rand@npm:6.0.4"
-  checksum: e1c4e69f8bf7303e5252756d67c3c7551385cd34d94a1f511fe099727ccbab74c898c03a06d4c4a24a89b51858781057b83ebbfe740d984240cdc04fead36068
+  version: 6.1.0
+  resolution: "pure-rand@npm:6.1.0"
+  checksum: 8d53bc02bed99eca0b65b505090152ee7e9bd67dd74f8ff32ba1c883b87234067c5bf68d2614759fb217d82594d7a92919e6df80f97885e7b12b42af4bd3316a
   languageName: node
   linkType: hard
 
 "q@npm:^1.5.1":
   version: 1.5.1
   resolution: "q@npm:1.5.1"
   checksum: 147baa93c805bc1200ed698bdf9c72e9e42c05f96d007e33a558b5fdfd63e5ea130e99313f28efc1783e90e6bdb4e48b67a36fcc026b7b09202437ae88a1fb12
@@ -10986,45 +11011,45 @@
   dependencies:
     safe-buffer: ^5.1.0
   checksum: d779499376bd4cbb435ef3ab9a957006c8682f343f14089ed5f27764e4645114196e75b7f6abf1cbd84fd247c0cb0651698444df8c9bf30e62120fbbc52269d6
   languageName: node
   linkType: hard
 
 "react-dom@npm:^18.2.0":
-  version: 18.2.0
-  resolution: "react-dom@npm:18.2.0"
+  version: 18.3.1
+  resolution: "react-dom@npm:18.3.1"
   dependencies:
     loose-envify: ^1.1.0
-    scheduler: ^0.23.0
+    scheduler: ^0.23.2
   peerDependencies:
-    react: ^18.2.0
-  checksum: 7d323310bea3a91be2965f9468d552f201b1c27891e45ddc2d6b8f717680c95a75ae0bc1e3f5cf41472446a2589a75aed4483aee8169287909fcd59ad149e8cc
+    react: ^18.3.1
+  checksum: 298954ecd8f78288dcaece05e88b570014d8f6dce5db6f66e6ee91448debeb59dcd31561dddb354eee47e6c1bb234669459060deb238ed0213497146e555a0b9
   languageName: node
   linkType: hard
 
 "react-is@npm:^16.13.1":
   version: 16.13.1
   resolution: "react-is@npm:16.13.1"
   checksum: f7a19ac3496de32ca9ae12aa030f00f14a3d45374f1ceca0af707c831b2a6098ef0d6bdae51bd437b0a306d7f01d4677fcc8de7c0d331eb47ad0f46130e53c5f
   languageName: node
   linkType: hard
 
 "react-is@npm:^18.0.0, react-is@npm:^18.2.0":
-  version: 18.2.0
-  resolution: "react-is@npm:18.2.0"
-  checksum: e72d0ba81b5922759e4aff17e0252bd29988f9642ed817f56b25a3e217e13eea8a7f2322af99a06edb779da12d5d636e9fda473d620df9a3da0df2a74141d53e
+  version: 18.3.1
+  resolution: "react-is@npm:18.3.1"
+  checksum: e20fe84c86ff172fc8d898251b7cc2c43645d108bf96d0b8edf39b98f9a2cae97b40520ee7ed8ee0085ccc94736c4886294456033304151c3f94978cec03df21
   languageName: node
   linkType: hard
 
 "react@npm:>=17.0.0 <19.0.0, react@npm:^18.2.0":
-  version: 18.2.0
-  resolution: "react@npm:18.2.0"
+  version: 18.3.1
+  resolution: "react@npm:18.3.1"
   dependencies:
     loose-envify: ^1.1.0
-  checksum: 88e38092da8839b830cda6feef2e8505dec8ace60579e46aa5490fc3dc9bba0bd50336507dc166f43e3afc1c42939c09fe33b25fae889d6f402721dcd78fca1b
+  checksum: a27bcfa8ff7c15a1e50244ad0d0c1cb2ad4375eeffefd266a64889beea6f6b64c4966c9b37d14ee32d6c9fcd5aa6ba183b6988167ab4d127d13e7cb5b386a376
   languageName: node
   linkType: hard
 
 "read-cmd-shim@npm:3.0.0":
   version: 3.0.0
   resolution: "read-cmd-shim@npm:3.0.0"
   checksum: b518c6026f3320e30b692044f6ff5c4dc80f9c71261296da8994101b569b26b12b8e5df397bba2d4691dd3a3a2f770a1eca7be18a69ec202fac6dcfadc5016fd
@@ -11346,15 +11371,15 @@
 "reusify@npm:^1.0.4":
   version: 1.0.4
   resolution: "reusify@npm:1.0.4"
   checksum: c3076ebcc22a6bc252cb0b9c77561795256c22b757f40c0d8110b1300723f15ec0fc8685e8d4ea6d7666f36c79ccc793b1939c748bf36f18f542744a4e379fcc
   languageName: node
   linkType: hard
 
-"rimraf@npm:^3.0.0, rimraf@npm:^3.0.2":
+"rimraf@npm:^3.0.2":
   version: 3.0.2
   resolution: "rimraf@npm:3.0.2"
   dependencies:
     glob: ^7.1.3
   bin:
     rimraf: bin.js
   checksum: 87f4164e396f0171b0a3386cc1877a817f572148ee13a7e113b238e48e8a9f2f31d009a92ec38a591ff1567d9662c6b67fd8818a2dbbaed74bc26a87a2a4a9a0
@@ -11369,21 +11394,21 @@
   bin:
     rimraf: dist/cjs/src/bin.js
   checksum: b786adc02651e2e24bbedb04bbdea80652fc9612632931ff2d9f898c5e4708fe30956186597373c568bd5230a4dc2fadfc816ccacba8a1daded3a006a6b74f1a
   languageName: node
   linkType: hard
 
 "rimraf@npm:~5.0.1":
-  version: 5.0.5
-  resolution: "rimraf@npm:5.0.5"
+  version: 5.0.7
+  resolution: "rimraf@npm:5.0.7"
   dependencies:
     glob: ^10.3.7
   bin:
     rimraf: dist/esm/bin.mjs
-  checksum: d66eef829b2e23b16445f34e73d75c7b7cf4cbc8834b04720def1c8f298eb0753c3d76df77325fad79d0a2c60470525d95f89c2475283ad985fd7441c32732d1
+  checksum: 884852abf8aefd4667448d87bdab04120a8641266c828cf382ac811713547eda18f81799d2146ffec3178f357d83d44ec01c10095949c82e23551660732bf14f
   languageName: node
   linkType: hard
 
 "run-async@npm:^2.4.0":
   version: 2.4.1
   resolution: "run-async@npm:2.4.1"
   checksum: a2c88aa15df176f091a2878eb840e68d0bdee319d8d97bbb89112223259cebecb94bc0defd735662b83c2f7a30bed8cddb7d1674eb48ae7322dc602b22d03797
@@ -11425,43 +11450,43 @@
 "safer-buffer@npm:>= 2.1.2 < 3, safer-buffer@npm:>= 2.1.2 < 3.0.0":
   version: 2.1.2
   resolution: "safer-buffer@npm:2.1.2"
   checksum: cab8f25ae6f1434abee8d80023d7e72b598cf1327164ddab31003c51215526801e40b66c5e65d658a0af1e9d6478cadcb4c745f4bd6751f97d8644786c0978b0
   languageName: node
   linkType: hard
 
-"sanitize-html@npm:~2.7.3":
-  version: 2.7.3
-  resolution: "sanitize-html@npm:2.7.3"
+"sanitize-html@npm:~2.12.1":
+  version: 2.12.1
+  resolution: "sanitize-html@npm:2.12.1"
   dependencies:
     deepmerge: ^4.2.2
     escape-string-regexp: ^4.0.0
-    htmlparser2: ^6.0.0
+    htmlparser2: ^8.0.0
     is-plain-object: ^5.0.0
     parse-srcset: ^1.0.2
     postcss: ^8.3.11
-  checksum: 2399d1fdbbc3a263fb413c1fe1971b3dc2b51abc6cc5cb49490624539d1c57a8fe31e2b21408c118e2a957f4e673e3169b1f9a5807654408f17b130a9d78aed7
+  checksum: fb96ea7170d51b5af2607f5cfd84464c78fc6f47e339407f55783e781c6a0288a8d40bbf97ea6a8758924ba9b2d33dcc4846bb94caacacd90d7f2de10ed8541a
   languageName: node
   linkType: hard
 
 "saxes@npm:^6.0.0":
   version: 6.0.0
   resolution: "saxes@npm:6.0.0"
   dependencies:
     xmlchars: ^2.2.0
   checksum: d3fa3e2aaf6c65ed52ee993aff1891fc47d5e47d515164b5449cbf5da2cbdc396137e55590472e64c5c436c14ae64a8a03c29b9e7389fc6f14035cf4e982ef3b
   languageName: node
   linkType: hard
 
-"scheduler@npm:^0.23.0":
-  version: 0.23.0
-  resolution: "scheduler@npm:0.23.0"
+"scheduler@npm:^0.23.2":
+  version: 0.23.2
+  resolution: "scheduler@npm:0.23.2"
   dependencies:
     loose-envify: ^1.1.0
-  checksum: d79192eeaa12abef860c195ea45d37cbf2bbf5f66e3c4dcd16f54a7da53b17788a70d109ee3d3dde1a0fd50e6a8fc171f4300356c5aee4fc0171de526bf35f8a
+  checksum: 3e82d1f419e240ef6219d794ff29c7ee415fbdc19e038f680a10c067108e06284f1847450a210b29bbaf97b9d8a97ced5f624c31c681248ac84c80d56ad5a2c4
   languageName: node
   linkType: hard
 
 "schema-utils@npm:^2.7.0":
   version: 2.7.1
   resolution: "schema-utils@npm:2.7.1"
   dependencies:
@@ -11532,21 +11557,19 @@
   bin:
     semver: bin/semver.js
   checksum: ae47d06de28836adb9d3e25f22a92943477371292d9b665fb023fae278d345d508ca1958232af086d85e0155aee22e313e100971898bbb8d5d89b8b1d4054ca2
   languageName: node
   linkType: hard
 
 "semver@npm:^7.0.0, semver@npm:^7.1.1, semver@npm:^7.3.4, semver@npm:^7.3.5, semver@npm:^7.3.7, semver@npm:^7.3.8, semver@npm:^7.5.3, semver@npm:^7.5.4":
-  version: 7.6.0
-  resolution: "semver@npm:7.6.0"
-  dependencies:
-    lru-cache: ^6.0.0
+  version: 7.6.2
+  resolution: "semver@npm:7.6.2"
   bin:
     semver: bin/semver.js
-  checksum: 7427f05b70786c696640edc29fdd4bc33b2acf3bbe1740b955029044f80575fc664e1a512e4113c3af21e767154a94b4aa214bf6cd6e42a1f6dba5914e0b208c
+  checksum: 40f6a95101e8d854357a644da1b8dd9d93ce786d5c6a77227bc69dbb17bea83d0d1d1d7c4cd5920a6df909f48e8bd8a5909869535007f90278289f2451d0292d
   languageName: node
   linkType: hard
 
 "serialize-javascript@npm:^6.0.1":
   version: 6.0.2
   resolution: "serialize-javascript@npm:6.0.2"
   dependencies:
@@ -11653,32 +11676,32 @@
     agent-base: ^6.0.2
     debug: ^4.3.3
     socks: ^2.6.2
   checksum: 720554370154cbc979e2e9ce6a6ec6ced205d02757d8f5d93fe95adae454fc187a5cbfc6b022afab850a5ce9b4c7d73e0f98e381879cf45f66317a4895953846
   languageName: node
   linkType: hard
 
-"socks-proxy-agent@npm:^8.0.1":
-  version: 8.0.2
-  resolution: "socks-proxy-agent@npm:8.0.2"
+"socks-proxy-agent@npm:^8.0.3":
+  version: 8.0.3
+  resolution: "socks-proxy-agent@npm:8.0.3"
   dependencies:
-    agent-base: ^7.0.2
+    agent-base: ^7.1.1
     debug: ^4.3.4
     socks: ^2.7.1
-  checksum: 4fb165df08f1f380881dcd887b3cdfdc1aba3797c76c1e9f51d29048be6e494c5b06d68e7aea2e23df4572428f27a3ec22b3d7c75c570c5346507433899a4b6d
+  checksum: 8fab38821c327c190c28f1658087bc520eb065d55bc07b4a0fdf8d1e0e7ad5d115abbb22a95f94f944723ea969dd771ad6416b1e3cde9060c4c71f705c8b85c5
   languageName: node
   linkType: hard
 
 "socks@npm:^2.6.2, socks@npm:^2.7.1":
-  version: 2.8.0
-  resolution: "socks@npm:2.8.0"
+  version: 2.8.3
+  resolution: "socks@npm:2.8.3"
   dependencies:
     ip-address: ^9.0.5
     smart-buffer: ^4.2.0
-  checksum: b245081650c5fc112f0e10d2ee3976f5665d2191b9f86b181edd3c875d53d84a94bc173752d5be2651a450e3ef799fe7ec405dba3165890c08d9ac0b4ec1a487
+  checksum: 7a6b7f6eedf7482b9e4597d9a20e09505824208006ea8f2c49b71657427f3c137ca2ae662089baa73e1971c62322d535d9d0cf1c9235cf6f55e315c18203eadd
   languageName: node
   linkType: hard
 
 "sort-keys@npm:^2.0.0":
   version: 2.0.0
   resolution: "sort-keys@npm:2.0.0"
   dependencies:
@@ -11690,18 +11713,18 @@
 "source-list-map@npm:^2.0.0":
   version: 2.0.1
   resolution: "source-list-map@npm:2.0.1"
   checksum: 806efc6f75e7cd31e4815e7a3aaf75a45c704871ea4075cb2eb49882c6fca28998f44fc5ac91adb6de03b2882ee6fb02f951fdc85e6a22b338c32bfe19557938
   languageName: node
   linkType: hard
 
-"source-map-js@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "source-map-js@npm:1.0.2"
-  checksum: c049a7fc4deb9a7e9b481ae3d424cc793cb4845daa690bc5a05d428bf41bf231ced49b4cf0c9e77f9d42fdb3d20d6187619fc586605f5eabe995a316da8d377c
+"source-map-js@npm:^1.2.0":
+  version: 1.2.0
+  resolution: "source-map-js@npm:1.2.0"
+  checksum: 791a43306d9223792e84293b00458bf102a8946e7188f3db0e4e22d8d530b5f80a4ce468eb5ec0bf585443ad55ebbd630bf379c98db0b1f317fd902500217f97
   languageName: node
   linkType: hard
 
 "source-map-loader@npm:~1.0.2":
   version: 1.0.2
   resolution: "source-map-loader@npm:1.0.2"
   dependencies:
@@ -11815,19 +11838,19 @@
   dependencies:
     minipass: ^3.1.1
   checksum: fb58f5e46b6923ae67b87ad5ef1c5ab6d427a17db0bead84570c2df3cd50b4ceb880ebdba2d60726588272890bae842a744e1ecce5bd2a2a582fccd5068309eb
   languageName: node
   linkType: hard
 
 "ssri@npm:^10.0.0, ssri@npm:^10.0.1":
-  version: 10.0.5
-  resolution: "ssri@npm:10.0.5"
+  version: 10.0.6
+  resolution: "ssri@npm:10.0.6"
   dependencies:
     minipass: ^7.0.3
-  checksum: 0a31b65f21872dea1ed3f7c200d7bc1c1b91c15e419deca14f282508ba917cbb342c08a6814c7f68ca4ca4116dd1a85da2bbf39227480e50125a1ceffeecb750
+  checksum: 4603d53a05bcd44188747d38f1cc43833b9951b5a1ee43ba50535bdfc5fe4a0897472dbe69837570a5417c3c073377ef4f8c1a272683b401857f72738ee57299
   languageName: node
   linkType: hard
 
 "stack-utils@npm:^2.0.3":
   version: 2.0.6
   resolution: "stack-utils@npm:2.0.6"
   dependencies:
@@ -11960,17 +11983,17 @@
   peerDependencies:
     webpack: ^5.0.0
   checksum: caac3f2fe2c3c89e49b7a2a9329e1cfa515ecf5f36b9c4885f9b218019fda207a9029939b2c35821dec177a264a007e7c391ccdd3ff7401881ce6287b9c8f38b
   languageName: node
   linkType: hard
 
 "style-mod@npm:^4.0.0, style-mod@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "style-mod@npm:4.1.0"
-  checksum: 8402b14ca11113a3640d46b3cf7ba49f05452df7846bc5185a3535d9b6a64a3019e7fb636b59ccbb7816aeb0725b24723e77a85b05612a9360e419958e13b4e6
+  version: 4.1.2
+  resolution: "style-mod@npm:4.1.2"
+  checksum: 7c5c3e82747f9bcf5f288d8d07f50848e4630fe5ff7bfe4d94cc87d6b6a2588227cbf21b4c792ac6406e5852293300a75e710714479a5c59a06af677f0825ef8
   languageName: node
   linkType: hard
 
 "supports-color@npm:^5.3.0":
   version: 5.5.0
   resolution: "supports-color@npm:5.5.0"
   dependencies:
@@ -12059,24 +12082,24 @@
     mkdirp: ^1.0.3
     yallist: ^4.0.0
   checksum: a04c07bb9e2d8f46776517d4618f2406fb977a74d914ad98b264fc3db0fe8224da5bec11e5f8902c5b9bcb8ace22d95fbe3c7b36b8593b7dfc8391a25898f32f
   languageName: node
   linkType: hard
 
 "tar@npm:^6.1.11, tar@npm:^6.1.2":
-  version: 6.2.0
-  resolution: "tar@npm:6.2.0"
+  version: 6.2.1
+  resolution: "tar@npm:6.2.1"
   dependencies:
     chownr: ^2.0.0
     fs-minipass: ^2.0.0
     minipass: ^5.0.0
     minizlib: ^2.1.1
     mkdirp: ^1.0.3
     yallist: ^4.0.0
-  checksum: db4d9fe74a2082c3a5016630092c54c8375ff3b280186938cfd104f2e089c4fd9bad58688ef6be9cf186a889671bf355c7cda38f09bbf60604b281715ca57f5c
+  checksum: f1322768c9741a25356c11373bce918483f40fa9a25c69c59410c8a1247632487edef5fe76c5f12ac51a6356d2f1829e96d2bc34098668a2fc34d76050ac2b6c
   languageName: node
   linkType: hard
 
 "temp-dir@npm:1.0.0":
   version: 1.0.0
   resolution: "temp-dir@npm:1.0.0"
   checksum: cb2b58ddfb12efa83e939091386ad73b425c9a8487ea0095fe4653192a40d49184a771a1beba99045fbd011e389fd563122d79f54f82be86a55620667e08a6b2
@@ -12122,24 +12145,24 @@
     uglify-js:
       optional: true
   checksum: bd6e7596cf815f3353e2a53e79cbdec959a1b0276f5e5d4e63e9d7c3c5bb5306df567729da287d1c7b39d79093e56863c569c42c6c24cc34c76aa313bd2cbcea
   languageName: node
   linkType: hard
 
 "terser@npm:^5.26.0":
-  version: 5.27.1
-  resolution: "terser@npm:5.27.1"
+  version: 5.31.0
+  resolution: "terser@npm:5.31.0"
   dependencies:
     "@jridgewell/source-map": ^0.3.3
     acorn: ^8.8.2
     commander: ^2.20.0
     source-map-support: ~0.5.20
   bin:
     terser: bin/terser
-  checksum: 6b917f9ddeff3264882988ed48a23652a2dbfce67df703ca92a35cedd7ef45a9ad3db2a68f383da745dde529053385048c7d347ab46837ac43d01ed9bbe09a40
+  checksum: 48f14229618866bba8a9464e9d0e7fdcb6b6488b3a6c4690fcf4d48df65bf45959d5ae8c02f1a0b3f3dd035a9ae340b715e1e547645b112dc3963daa3564699a
   languageName: node
   linkType: hard
 
 "test-exclude@npm:^6.0.0":
   version: 6.0.0
   resolution: "test-exclude@npm:6.0.0"
   dependencies:
@@ -12196,19 +12219,17 @@
   dependencies:
     os-tmpdir: ~1.0.2
   checksum: 902d7aceb74453ea02abbf58c203f4a8fc1cead89b60b31e354f74ed5b3fb09ea817f94fb310f884a5d16987dd9fa5a735412a7c2dd088dd3d415aa819ae3a28
   languageName: node
   linkType: hard
 
 "tmp@npm:~0.2.1":
-  version: 0.2.1
-  resolution: "tmp@npm:0.2.1"
-  dependencies:
-    rimraf: ^3.0.0
-  checksum: 8b1214654182575124498c87ca986ac53dc76ff36e8f0e0b67139a8d221eaecfdec108c0e6ec54d76f49f1f72ab9325500b246f562b926f85bcdfca8bf35df9e
+  version: 0.2.3
+  resolution: "tmp@npm:0.2.3"
+  checksum: 73b5c96b6e52da7e104d9d44afb5d106bb1e16d9fa7d00dbeb9e6522e61b571fbdb165c756c62164be9a3bbe192b9b268c236d370a2a0955c7689cd2ae377b95
   languageName: node
   linkType: hard
 
 "tmpl@npm:1.0.5":
   version: 1.0.5
   resolution: "tmpl@npm:1.0.5"
   checksum: cd922d9b853c00fe414c5a774817be65b058d54a2d01ebb415840960406c669a0fc632f66df885e24cb022ec812739199ccbdb8d1164c3e513f85bfca5ab2873
@@ -12228,22 +12249,22 @@
   dependencies:
     is-number: ^7.0.0
   checksum: f76fa01b3d5be85db6a2a143e24df9f60dd047d151062d0ba3df62953f2f697b16fe5dad9b0ac6191c7efc7b1d9dcaa4b768174b7b29da89d4428e64bc0a20ed
   languageName: node
   linkType: hard
 
 "tough-cookie@npm:^4.1.2":
-  version: 4.1.3
-  resolution: "tough-cookie@npm:4.1.3"
+  version: 4.1.4
+  resolution: "tough-cookie@npm:4.1.4"
   dependencies:
     psl: ^1.1.33
     punycode: ^2.1.1
     universalify: ^0.2.0
     url-parse: ^1.5.3
-  checksum: c9226afff36492a52118432611af083d1d8493a53ff41ec4ea48e5b583aec744b989e4280bcf476c910ec1525a89a4a0f1cae81c08b18fb2ec3a9b3a72b91dcc
+  checksum: 5815059f014c31179a303c673f753f7899a6fce94ac93712c88ea5f3c26e0c042b5f0c7a599a00f8e0feeca4615dba75c3dffc54f3c1a489978aa8205e09307c
   languageName: node
   linkType: hard
 
 "tr46@npm:^2.1.0":
   version: 2.1.0
   resolution: "tr46@npm:2.1.0"
   dependencies:
@@ -12279,52 +12300,55 @@
   version: 3.0.1
   resolution: "trim-newlines@npm:3.0.1"
   checksum: b530f3fadf78e570cf3c761fb74fef655beff6b0f84b29209bac6c9622db75ad1417f4a7b5d54c96605dcd72734ad44526fef9f396807b90839449eb543c6206
   languageName: node
   linkType: hard
 
 "ts-api-utils@npm:^1.0.1":
-  version: 1.2.1
-  resolution: "ts-api-utils@npm:1.2.1"
+  version: 1.3.0
+  resolution: "ts-api-utils@npm:1.3.0"
   peerDependencies:
     typescript: ">=4.2.0"
-  checksum: 17a2a4454d65a6765b9351304cfd516fcda3098f49d72bba90cb7f22b6a09a573b4a1993fd7de7d6b8046c408960c5f21a25e64ccb969d484b32ea3b3e19d6e4
+  checksum: c746ddabfdffbf16cb0b0db32bb287236a19e583057f8649ee7c49995bb776e1d3ef384685181c11a1a480369e022ca97512cb08c517b2d2bd82c83754c97012
   languageName: node
   linkType: hard
 
 "ts-jest@npm:^29.1.0, ts-jest@npm:^29.1.1":
-  version: 29.1.2
-  resolution: "ts-jest@npm:29.1.2"
+  version: 29.1.3
+  resolution: "ts-jest@npm:29.1.3"
   dependencies:
     bs-logger: 0.x
     fast-json-stable-stringify: 2.x
     jest-util: ^29.0.0
     json5: ^2.2.3
     lodash.memoize: 4.x
     make-error: 1.x
     semver: ^7.5.3
     yargs-parser: ^21.0.1
   peerDependencies:
     "@babel/core": ">=7.0.0-beta.0 <8"
+    "@jest/transform": ^29.0.0
     "@jest/types": ^29.0.0
     babel-jest: ^29.0.0
     jest: ^29.0.0
     typescript: ">=4.3 <6"
   peerDependenciesMeta:
     "@babel/core":
       optional: true
+    "@jest/transform":
+      optional: true
     "@jest/types":
       optional: true
     babel-jest:
       optional: true
     esbuild:
       optional: true
   bin:
     ts-jest: cli.js
-  checksum: a0ce0affc1b716c78c9ab55837829c42cb04b753d174a5c796bb1ddf9f0379fc20647b76fbe30edb30d9b23181908138d6b4c51ef2ae5e187b66635c295cefd5
+  checksum: c5b2c0501680a9056c50541a3315de7b3b85a611056b978062b4defc96fb0066d12bf1e15715021799a3779723343fb98a9a4ba01dc01709f274899b6c28453d
   languageName: node
   linkType: hard
 
 "tsconfig-paths@npm:^4.1.2":
   version: 4.2.0
   resolution: "tsconfig-paths@npm:4.2.0"
   dependencies:
@@ -12599,28 +12623,28 @@
   version: 2.0.1
   resolution: "upath@npm:2.0.1"
   checksum: 2db04f24a03ef72204c7b969d6991abec9e2cb06fb4c13a1fd1c59bc33b46526b16c3325e55930a11ff86a77a8cbbcda8f6399bf914087028c5beae21ecdb33c
   languageName: node
   linkType: hard
 
 "update-browserslist-db@npm:^1.0.13":
-  version: 1.0.13
-  resolution: "update-browserslist-db@npm:1.0.13"
+  version: 1.0.16
+  resolution: "update-browserslist-db@npm:1.0.16"
   dependencies:
-    escalade: ^3.1.1
-    picocolors: ^1.0.0
+    escalade: ^3.1.2
+    picocolors: ^1.0.1
   peerDependencies:
     browserslist: ">= 4.21.0"
   bin:
     update-browserslist-db: cli.js
-  checksum: 1e47d80182ab6e4ad35396ad8b61008ae2a1330221175d0abd37689658bdb61af9b705bfc41057fd16682474d79944fb2d86767c5ed5ae34b6276b9bed353322
+  checksum: 51b1f7189c9ea5925c80154b0a6fd3ec36106d07858d8f69826427d8edb4735d1801512c69eade38ba0814d7407d11f400d74440bbf3da0309f3d788017f35b2
   languageName: node
   linkType: hard
 
-"uri-js@npm:^4.2.2":
+"uri-js@npm:^4.2.2, uri-js@npm:^4.4.1":
   version: 4.4.1
   resolution: "uri-js@npm:4.4.1"
   dependencies:
     punycode: ^2.1.0
   checksum: 7167432de6817fe8e9e0c9684f1d2de2bb688c94388f7569f7dbdb1587c9f4ca2a77962f134ec90be0cc4d004c939ff0d05acc9f34a0db39a3c797dada262633
   languageName: node
   linkType: hard
@@ -12694,19 +12718,17 @@
   dependencies:
     builtins: ^1.0.3
   checksum: ce4c68207abfb22c05eedb09ff97adbcedc80304a235a0844f5344f1fd5086aa80e4dbec5684d6094e26e35065277b765c1caef68bcea66b9056761eddb22967
   languageName: node
   linkType: hard
 
 "validate-npm-package-name@npm:^5.0.0":
-  version: 5.0.0
-  resolution: "validate-npm-package-name@npm:5.0.0"
-  dependencies:
-    builtins: ^5.0.0
-  checksum: 5342a994986199b3c28e53a8452a14b2bb5085727691ea7aa0d284a6606b127c371e0925ae99b3f1ef7cc7d2c9de75f52eb61a3d1cc45e39bca1e3a9444cbb4e
+  version: 5.0.1
+  resolution: "validate-npm-package-name@npm:5.0.1"
+  checksum: 0d583a1af23aeffea7748742cf22b6802458736fb8b60323ba5949763824d46f796474b0e1b9206beb716f9d75269e19dbd7795d6b038b29d561be95dd827381
   languageName: node
   linkType: hard
 
 "validate.io-array@npm:^1.0.3":
   version: 1.0.6
   resolution: "validate.io-array@npm:1.0.6"
   checksum: 54eca83ebc702e3e46499f9d9e77287a95ae25c4e727cd2fafee29c7333b3a36cca0c5d8f090b9406262786de80750fba85e7e7ef41e20bf8cc67d5570de449b
@@ -12742,28 +12764,35 @@
 "validate.io-number@npm:^1.0.3":
   version: 1.0.3
   resolution: "validate.io-number@npm:1.0.3"
   checksum: 42418aeb6c969efa745475154fe576809b02eccd0961aad0421b090d6e7a12d23a3e28b0d5dddd2c6347c1a6bdccb82bba5048c716131cd20207244d50e07282
   languageName: node
   linkType: hard
 
-"vscode-jsonrpc@npm:8.2.0, vscode-jsonrpc@npm:^8.0.2":
+"vscode-jsonrpc@npm:8.2.0":
   version: 8.2.0
   resolution: "vscode-jsonrpc@npm:8.2.0"
   checksum: f302a01e59272adc1ae6494581fa31c15499f9278df76366e3b97b2236c7c53ebfc71efbace9041cfd2caa7f91675b9e56f2407871a1b3c7f760a2e2ee61484a
   languageName: node
   linkType: hard
 
 "vscode-jsonrpc@npm:^6.0.0":
   version: 6.0.0
   resolution: "vscode-jsonrpc@npm:6.0.0"
   checksum: 3a67a56f287e8c449f2d9752eedf91e704dc7b9a326f47fb56ac07667631deb45ca52192e9bccb2ab108764e48409d70fa64b930d46fc3822f75270b111c5f53
   languageName: node
   linkType: hard
 
+"vscode-jsonrpc@npm:^8.0.2":
+  version: 8.2.1
+  resolution: "vscode-jsonrpc@npm:8.2.1"
+  checksum: 2af2c333d73f6587896a7077978b8d4b430e55c674d5dbb90597a84a6647057c1655a3bff398a9b08f1f8ba57dbd2deabf05164315829c297b0debba3b8bc19e
+  languageName: node
+  linkType: hard
+
 "vscode-languageserver-protocol@npm:^3.17.0":
   version: 3.17.5
   resolution: "vscode-languageserver-protocol@npm:3.17.5"
   dependencies:
     vscode-jsonrpc: 8.2.0
     vscode-languageserver-types: 3.17.5
   checksum: dfb42d276df5dfea728267885b99872ecff62f6c20448b8539fae71bb196b420f5351c5aca7c1047bf8fb1f89fa94a961dce2bc5bf7e726198f4be0bb86a1e71
@@ -12814,21 +12843,21 @@
   resolution: "walker@npm:1.0.8"
   dependencies:
     makeerror: 1.0.12
   checksum: ad7a257ea1e662e57ef2e018f97b3c02a7240ad5093c392186ce0bcf1f1a60bbadd520d073b9beb921ed99f64f065efb63dfc8eec689a80e569f93c1c5d5e16c
   languageName: node
   linkType: hard
 
-"watchpack@npm:^2.4.0":
-  version: 2.4.0
-  resolution: "watchpack@npm:2.4.0"
+"watchpack@npm:^2.4.1":
+  version: 2.4.1
+  resolution: "watchpack@npm:2.4.1"
   dependencies:
     glob-to-regexp: ^0.4.1
     graceful-fs: ^4.1.2
-  checksum: 23d4bc58634dbe13b86093e01c6a68d8096028b664ab7139d58f0c37d962d549a940e98f2f201cecdabd6f9c340338dc73ef8bf094a2249ef582f35183d1a131
+  checksum: 5b0179348655dcdf19cac7cb4ff923fdc024d630650c0bf6bec8899cf47c60e19d4f810a88dba692ed0e7f684cf0fcffea86efdbf6c35d81f031e328043b7fab
   languageName: node
   linkType: hard
 
 "wcwidth@npm:^1.0.0, wcwidth@npm:^1.0.1":
   version: 1.0.1
   resolution: "wcwidth@npm:1.0.1"
   dependencies:
@@ -12915,47 +12944,47 @@
   version: 3.2.3
   resolution: "webpack-sources@npm:3.2.3"
   checksum: 989e401b9fe3536529e2a99dac8c1bdc50e3a0a2c8669cbafad31271eadd994bc9405f88a3039cd2e29db5e6d9d0926ceb7a1a4e7409ece021fe79c37d9c4607
   languageName: node
   linkType: hard
 
 "webpack@npm:^5.76.1":
-  version: 5.90.1
-  resolution: "webpack@npm:5.90.1"
+  version: 5.91.0
+  resolution: "webpack@npm:5.91.0"
   dependencies:
     "@types/eslint-scope": ^3.7.3
     "@types/estree": ^1.0.5
-    "@webassemblyjs/ast": ^1.11.5
-    "@webassemblyjs/wasm-edit": ^1.11.5
-    "@webassemblyjs/wasm-parser": ^1.11.5
+    "@webassemblyjs/ast": ^1.12.1
+    "@webassemblyjs/wasm-edit": ^1.12.1
+    "@webassemblyjs/wasm-parser": ^1.12.1
     acorn: ^8.7.1
     acorn-import-assertions: ^1.9.0
     browserslist: ^4.21.10
     chrome-trace-event: ^1.0.2
-    enhanced-resolve: ^5.15.0
+    enhanced-resolve: ^5.16.0
     es-module-lexer: ^1.2.1
     eslint-scope: 5.1.1
     events: ^3.2.0
     glob-to-regexp: ^0.4.1
-    graceful-fs: ^4.2.9
+    graceful-fs: ^4.2.11
     json-parse-even-better-errors: ^2.3.1
     loader-runner: ^4.2.0
     mime-types: ^2.1.27
     neo-async: ^2.6.2
     schema-utils: ^3.2.0
     tapable: ^2.1.1
     terser-webpack-plugin: ^5.3.10
-    watchpack: ^2.4.0
+    watchpack: ^2.4.1
     webpack-sources: ^3.2.3
   peerDependenciesMeta:
     webpack-cli:
       optional: true
   bin:
     webpack: bin/webpack.js
-  checksum: a7be844d5720a0c6282fec012e6fa34b1137dff953c5d48bf2ef066a6c27c1dbc92a9b9effc05ee61c9fe269499266db9782073f2d82a589d3c5c966ffc56584
+  checksum: f1073715dbb1ed5c070affef293d800a867708bcbc5aba4d8baee87660e0cf53c55966a6f36fab078d1d6c9567cdcd0a9086bdfb607cab87ea68c6449791b9a3
   languageName: node
   linkType: hard
 
 "whatwg-encoding@npm:^2.0.0":
   version: 2.0.0
   resolution: "whatwg-encoding@npm:2.0.0"
   dependencies:
@@ -13054,14 +13083,21 @@
 "wildcard@npm:^2.0.0":
   version: 2.0.1
   resolution: "wildcard@npm:2.0.1"
   checksum: e0c60a12a219e4b12065d1199802d81c27b841ed6ad6d9d28240980c73ceec6f856771d575af367cbec2982d9ae7838759168b551776577f155044f5a5ba843c
   languageName: node
   linkType: hard
 
+"word-wrap@npm:^1.2.5":
+  version: 1.2.5
+  resolution: "word-wrap@npm:1.2.5"
+  checksum: f93ba3586fc181f94afdaff3a6fef27920b4b6d9eaefed0f428f8e07adea2a7f54a5f2830ce59406c8416f033f86902b91eb824072354645eea687dff3691ccb
+  languageName: node
+  linkType: hard
+
 "wordwrap@npm:^1.0.0":
   version: 1.0.0
   resolution: "wordwrap@npm:1.0.0"
   checksum: 2a44b2788165d0a3de71fd517d4880a8e20ea3a82c080ce46e294f0b68b69a2e49cff5f99c600e275c698a90d12c5ea32aff06c311f0db2eb3f1201f3e7b2a04
   languageName: node
   linkType: hard
 
@@ -13180,25 +13216,25 @@
     type-fest: ^0.4.1
     write-json-file: ^3.2.0
   checksum: 7864d44370f42a6761f6898d07ee2818c7a2faad45116580cf779f3adaf94e4bea5557612533a6c421c32323253ecb63b50615094960a637aeaef5df0fd2d6cd
   languageName: node
   linkType: hard
 
 "ws@npm:^8.11.0":
-  version: 8.16.0
-  resolution: "ws@npm:8.16.0"
+  version: 8.17.0
+  resolution: "ws@npm:8.17.0"
   peerDependencies:
     bufferutil: ^4.0.1
     utf-8-validate: ">=5.0.2"
   peerDependenciesMeta:
     bufferutil:
       optional: true
     utf-8-validate:
       optional: true
-  checksum: feb3eecd2bae82fa8a8beef800290ce437d8b8063bdc69712725f21aef77c49cb2ff45c6e5e7fce622248f9c7abaee506bae0a9064067ffd6935460c7357321b
+  checksum: 147ef9eab0251364e1d2c55338ad0efb15e6913923ccbfdf20f7a8a6cb8f88432bcd7f4d8f66977135bfad35575644f9983201c1a361019594a4e53977bf6d4e
   languageName: node
   linkType: hard
 
 "xml-name-validator@npm:^4.0.0":
   version: 4.0.0
   resolution: "xml-name-validator@npm:4.0.0"
   checksum: af100b79c29804f05fa35aa3683e29a321db9b9685d5e5febda3fa1e40f13f85abc40f45a6b2bf7bee33f68a1dc5e8eaef4cec100a304a9db565e6061d4cb5ad
@@ -13313,19 +13349,19 @@
     y18n: ^5.0.5
     yargs-parser: ^21.1.1
   checksum: 73b572e863aa4a8cbef323dd911d79d193b772defd5a51aab0aca2d446655216f5002c42c5306033968193bdbf892a7a4c110b0d77954a7fdf563e653967b56a
   languageName: node
   linkType: hard
 
 "yjs@npm:^13.5.40":
-  version: 13.6.12
-  resolution: "yjs@npm:13.6.12"
+  version: 13.6.15
+  resolution: "yjs@npm:13.6.15"
   dependencies:
     lib0: ^0.2.86
-  checksum: 40e189e521b343eb979af43d811de90e82169539b5e50472467c86b6096b911a986a7f93fe5b07fe63e7a27b8086f8b256192d6bbc6f1045d14e21bb8b76eceb
+  checksum: a0cdb323f9cd40de37c9cd0a9a4613e35d8365488ed6078ec632f0ec1853de4d16e46d435dc97e4029c0e70666e24d02c7240a71e84f7b1f15ff18670d715483
   languageName: node
   linkType: hard
 
 "yocto-queue@npm:^0.1.0":
   version: 0.1.0
   resolution: "yocto-queue@npm:0.1.0"
   checksum: f77b3d8d00310def622123df93d4ee654fc6a0096182af8bd60679ddcdfb3474c56c6c7190817c84a2785648cdee9d721c0154eb45698c62176c322fb46fc700
```

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/__init__.py` & `jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/package.json` & `jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9574652777777778%*

 * *Differences: {"'dependencies'": "{'@jupyterlite/javascript-kernel': '^0.4.0-alpha.0', '@jupyterlite/kernel': "*

 * *                   "'^0.2.1  || ^0.3.0 || ^0.4.0-alpha.0', '@jupyterlite/server': '^0.2.1 || "*

 * *                   "^0.3.0 || ^0.4.0-alpha.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.bcb6e0c823f3bdb2c1ce.js'}}",*

 * * "'version'": "'0.4.0-alpha.0'"}*

```diff
@@ -1,16 +1,16 @@
 {
     "author": "JupyterLite Contributors",
     "bugs": {
         "url": "https://github.com/jupyterlite/javascript-kernel/issues"
     },
     "dependencies": {
-        "@jupyterlite/javascript-kernel": "^0.3.0-alpha.1",
-        "@jupyterlite/kernel": "^0.2.1",
-        "@jupyterlite/server": "^0.2.1"
+        "@jupyterlite/javascript-kernel": "^0.4.0-alpha.0",
+        "@jupyterlite/kernel": "^0.2.1  || ^0.3.0 || ^0.4.0-alpha.0",
+        "@jupyterlite/server": "^0.2.1 || ^0.3.0 || ^0.4.0-alpha.0"
     },
     "description": "JupyterLite - JavaScript Kernel Extension",
     "devDependencies": {
         "@jupyterlab/builder": "~4.1.1",
         "rimraf": "~5.0.1",
         "typescript": "~5.1.6"
     },
@@ -22,15 +22,15 @@
         "lib/*.js.map",
         "lib/*.js"
     ],
     "homepage": "https://github.com/jupyterlite/javascript-kernel",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9db3df3efa1ab7d5af05.js"
+            "load": "static/remoteEntry.bcb6e0c823f3bdb2c1ce.js"
         },
         "extension": true,
         "outputDir": "../../jupyterlite_javascript_kernel/labextension",
         "sharedPackages": {
             "@jupyterlite/contents": {
                 "bundled": false,
                 "singleton": true
@@ -71,9 +71,9 @@
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "install:extension": "jlpm build",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.0-alpha.1"
+    "version": "0.4.0-alpha.0"
 }
```

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/312.4028241b320224658118.js` & `jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/916.6c2158a1e7981a0b119d.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
-/*! For license information please see 312.4028241b320224658118.js.LICENSE.txt */
+/*! For license information please see 916.6c2158a1e7981a0b119d.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_jupyterlite_javascript_kernel_extension = self.webpackChunk_jupyterlite_javascript_kernel_extension || []).push([
-    [312, 692], {
-        692: (e, t, n) => {
+    [916, 535], {
+        916: (e, t, n) => {
             n.r(t), n.d(t, {
                 JavaScriptKernel: () => j
             });
-            var r = n(388),
-                a = n(960),
-                s = n(464);
+            var r = n(655),
+                a = n(197),
+                s = n(262);
             const o = Symbol("Comlink.proxy"),
                 i = Symbol("Comlink.endpoint"),
                 c = Symbol("Comlink.releaseProxy"),
                 u = Symbol("Comlink.finalizer"),
                 l = Symbol("Comlink.thrown"),
                 p = e => "object" == typeof e && null !== e || "function" == typeof e,
                 m = new Map([
@@ -319,15 +319,15 @@
                 async commMsg(e) {
                     throw new Error("Not implemented")
                 }
                 async commClose(e) {
                     throw new Error("Not implemented")
                 }
                 initWorker(e) {
-                    return new Worker(new URL(n.p + n.u(584), n.b), {
+                    return new Worker(new URL(n.p + n.u(851), n.b), {
                         type: void 0
                     })
                 }
                 initRemote(e) {
                     const t = g(this._worker);
                     return t.initialize({
                         baseUrl: r.PageConfig.getBaseUrl()
```

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/584.7e49152bd31ca0f8291b.js` & `jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/851.f06be08f4dbb05785c82.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
-/*! For license information please see 584.7e49152bd31ca0f8291b.js.LICENSE.txt */
+/*! For license information please see 851.f06be08f4dbb05785c82.js.LICENSE.txt */
 (() => {
     var t = {
-            544: (t, e, n) => {
+            660: (t, e, n) => {
                 var r = "function" == typeof Map && Map.prototype,
                     o = Object.getOwnPropertyDescriptor && r ? Object.getOwnPropertyDescriptor(Map.prototype, "size") : null,
                     a = r && o && "function" == typeof o.get ? o.get : null,
                     i = r && Map.prototype.forEach,
                     c = "function" == typeof Set && Set.prototype,
                     u = Object.getOwnPropertyDescriptor && c ? Object.getOwnPropertyDescriptor(Set.prototype, "size") : null,
                     l = c && u && "function" == typeof u.get ? u.get : null,
@@ -45,15 +45,15 @@
                             var o = String(r),
                                 a = d.call(e, o.length + 1);
                             return v.call(o, n, "$&_") + "." + v.call(v.call(a, /([0-9]{3})/g, "$&_"), /_$/, "")
                         }
                     }
                     return v.call(e, n, "$&_")
                 }
-                var N = n(308),
+                var N = n(973),
                     C = N.custom,
                     $ = H(C) ? C : null;
 
                 function z(t, e, n) {
                     var r = "double" === (n.quoteStyle || e) ? '"' : "'";
                     return r + t + r
                 }
@@ -336,15 +336,15 @@
                     }
                     for (var u in t) B(t, u) && (n && String(Number(u)) === u && u < t.length || L && a["$" + u] instanceof Symbol || (w.call(/[^\w$]/, u) ? r.push(e(u, t) + ": " + e(t[u], t)) : r.push(u + ": " + e(t[u], t))));
                     if ("function" == typeof _)
                         for (var l = 0; l < i.length; l++) A.call(t, i[l]) && r.push("[" + e(i[l]) + "]: " + e(t[i[l]], t));
                     return r
                 }
             },
-            584: (t, e, n) => {
+            851: (t, e, n) => {
                 "use strict";
                 const r = Symbol("Comlink.proxy"),
                     o = Symbol("Comlink.endpoint"),
                     a = Symbol("Comlink.releaseProxy"),
                     i = Symbol("Comlink.finalizer"),
                     c = Symbol("Comlink.thrown"),
                     u = t => "object" == typeof t && null !== t || "function" == typeof t,
@@ -585,15 +585,15 @@
                         t.addEventListener("message", (function e(n) {
                             n.data && n.data.id && n.data.id === o && (t.removeEventListener("message", e), r(n.data))
                         })), t.start && t.start(), t.postMessage(Object.assign({
                             id: o
                         }, e), n)
                     }))
                 }
-                var w = n(544),
+                var w = n(660),
                     O = n.n(w);
                 s(new class {
                     constructor() {
                         this._executionCount = 0
                     }
                     async initialize(t) {
                         console.log = function(...t) {
@@ -678,15 +678,15 @@
                         }
                     }
                     _inspect(t) {
                         return void 0 === t ? void 0 : O()(t)
                     }
                 })
             },
-            308: () => {}
+            973: () => {}
         },
         e = {};
 
     function n(r) {
         var o = e[r];
         if (void 0 !== o) return o.exports;
         var a = e[r] = {
@@ -721,9 +721,9 @@
             if (a || (a = e[r] = {}), !(o.indexOf(a) >= 0)) {
                 if (o.push(a), t[r]) return t[r];
                 n.o(n.S, r) || (n.S[r] = {}), n.S[r];
                 var i = [];
                 return t[r] = i.length ? Promise.all(i).then((() => t[r] = 1)) : 1
             }
         }
-    })(), n(584)
+    })(), n(851)
 })();
```

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/5e8d6f34d83488f083fd.png` & `jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/5e8d6f34d83488f083fd.png`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/692.d7dd851ce6b7f32bbac2.js` & `jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/535.46e2f879361140e66596.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
-/*! For license information please see 692.d7dd851ce6b7f32bbac2.js.LICENSE.txt */
+/*! For license information please see 535.46e2f879361140e66596.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_jupyterlite_javascript_kernel_extension = self.webpackChunk_jupyterlite_javascript_kernel_extension || []).push([
-    [692, 312], {
-        692: (e, t, n) => {
+    [535, 916], {
+        916: (e, t, n) => {
             n.r(t), n.d(t, {
                 JavaScriptKernel: () => j
             });
-            var r = n(388),
-                a = n(960),
-                s = n(464);
+            var r = n(655),
+                a = n(197),
+                s = n(262);
             const o = Symbol("Comlink.proxy"),
                 i = Symbol("Comlink.endpoint"),
                 c = Symbol("Comlink.releaseProxy"),
                 u = Symbol("Comlink.finalizer"),
                 l = Symbol("Comlink.thrown"),
                 p = e => "object" == typeof e && null !== e || "function" == typeof e,
                 m = new Map([
@@ -319,15 +319,15 @@
                 async commMsg(e) {
                     throw new Error("Not implemented")
                 }
                 async commClose(e) {
                     throw new Error("Not implemented")
                 }
                 initWorker(e) {
-                    return new Worker(new URL(n.p + n.u(584), n.b), {
+                    return new Worker(new URL(n.p + n.u(851), n.b), {
                         type: void 0
                     })
                 }
                 initRemote(e) {
                     const t = g(this._worker);
                     return t.initialize({
                         baseUrl: r.PageConfig.getBaseUrl()
```

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/b1c098fa349a030dacbe.png` & `jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/b1c098fa349a030dacbe.png`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/remoteEntry.9db3df3efa1ab7d5af05.js` & `jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/remoteEntry.bcb6e0c823f3bdb2c1ce.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, l, u, f, s, c, p, d, h, v, m, b, g, y, j = {
-            228: (e, r, t) => {
+    var e, r, t, n, a, o, i, l, u, s, f, c, p, d, h, v, b, m, g, y, j = {
+            291: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(960), t.e(804)]).then((() => () => t(372))),
-                        "./extension": () => Promise.all([t.e(960), t.e(804)]).then((() => () => t(372)))
+                        "./index": () => Promise.all([t.e(197), t.e(238)]).then((() => () => t(496))),
+                        "./extension": () => Promise.all([t.e(197), t.e(238)]).then((() => () => t(496)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -36,43 +36,43 @@
     }
     k.m = j, k.c = w, k.d = (e, r) => {
         for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
-        312: "4028241b320224658118",
-        500: "51d01a57f7d3f6775b14",
-        584: "7e49152bd31ca0f8291b",
-        692: "d7dd851ce6b7f32bbac2",
-        804: "1ac186e1afa78c8a2770",
-        960: "56f4824ee7a5568ce76f"
+        197: "1b6a94fd514f00c8afe2",
+        238: "453d2599405730ec7a31",
+        256: "2a7bc9db483fccd1c202",
+        535: "46e2f879361140e66596",
+        851: "f06be08f4dbb05785c82",
+        916: "6c2158a1e7981a0b119d"
     } [e] + ".js?v=" + {
-        312: "4028241b320224658118",
-        500: "51d01a57f7d3f6775b14",
-        584: "7e49152bd31ca0f8291b",
-        692: "d7dd851ce6b7f32bbac2",
-        804: "1ac186e1afa78c8a2770",
-        960: "56f4824ee7a5568ce76f"
+        197: "1b6a94fd514f00c8afe2",
+        238: "453d2599405730ec7a31",
+        256: "2a7bc9db483fccd1c202",
+        535: "46e2f879361140e66596",
+        851: "f06be08f4dbb05785c82",
+        916: "6c2158a1e7981a0b119d"
     } [e], k.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlite/javascript-kernel-extension:", k.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
             if (void 0 !== a)
-                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
-                        i = s;
+                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
+                    var f = u[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
+                        i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, k.nc && i.setAttribute("nonce", k.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var c = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var a = e[t];
@@ -108,25 +108,25 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyterlite/javascript-kernel-extension", "0.3.0-alpha.1", (() => Promise.all([k.e(960), k.e(804)]).then((() => () => k(372))))), l("@jupyterlite/javascript-kernel", "0.3.0-alpha.1", (() => Promise.all([k.e(500), k.e(960), k.e(692)]).then((() => () => k(692)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyterlite/javascript-kernel-extension", "0.4.0-alpha.0", (() => Promise.all([k.e(197), k.e(238)]).then((() => () => k(496))))), l("@jupyterlite/javascript-kernel", "0.4.0-alpha.0", (() => Promise.all([k.e(256), k.e(197), k.e(916)]).then((() => () => k(916)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
-                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
+                for (var n = t.length - 1; n > -1 && (!e || !/^http(s?):/.test(e));) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), k.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
@@ -166,31 +166,31 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, s, c = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == c ? l > n && !a : "" == c != a);
-                if ("u" == s) {
+                var s, f, c = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !u || ("u" == c ? l > n && !a : "" == c != a);
+                if ("u" == f) {
                     if (!u || "u" != c) return !1
                 } else if (u)
-                    if (c == s)
+                    if (c == f)
                         if (l <= n) {
-                            if (f != e[l]) return !1
+                            if (s != e[l]) return !1
                         } else {
-                            if (a ? f > e[l] : f < e[l]) return !1;
-                            f != e[l] && (u = !1)
+                            if (a ? s > e[l] : s < e[l]) return !1;
+                            s != e[l] && (u = !1)
                         }
                 else if ("s" != c && "n" != c) {
                     if (a || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || s < c != a) return !1;
+                    if (l <= n || f < c != a) return !1;
                     u = !1
                 } else "s" != c && "n" != c && (u = !1, l--)
             }
         }
         var p = [],
             d = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
@@ -201,70 +201,73 @@
     }, i = (e, r) => {
         var t = k.S[e];
         if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
         var a = l(e, t);
         return o(n, a) || c(u(e, t, a, n)), p(e[t][a])
-    }, s = (e, r, t) => {
+    }, f = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, p = e => (e.loaded = 1, e.get()), h = (d = e => function(r, t, n, a) {
         var o = k.I(r);
         return o && o.then ? o.then(e.bind(e, r, k.S[r], t, n, a)) : e(r, k.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), v = d(((e, r, t, n, a) => {
-        var o = r && k.o(r, t) && s(r, t, n);
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = d(((e, r, t, n, a) => {
+        var o = r && k.o(r, t) && f(r, t, n);
         return o ? p(o) : a()
-    })), m = {}, b = {
-        960: () => h("default", "@jupyterlite/kernel", [2, 0, 2, 1]),
-        788: () => v("default", "@jupyterlite/javascript-kernel", [2, 0, 3, 0, , "alpha", 1], (() => Promise.all([k.e(500), k.e(312)]).then((() => () => k(692))))),
-        388: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 1]),
-        464: () => h("default", "@lumino/coreutils", [1, 2, 0, 0])
+    })), b = {}, m = {
+        197: () => h("default", "@jupyterlite/kernel", [, [2, 0, 4, 0, , "alpha", 0],
+            [2, 0, 3, 0],
+            [2, 0, 2, 1], 1, 1
+        ]),
+        687: () => v("default", "@jupyterlite/javascript-kernel", [2, 0, 4, 0, , "alpha", 0], (() => Promise.all([k.e(256), k.e(535)]).then((() => () => k(916))))),
+        262: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
+        655: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 8])
     }, g = {
-        500: [388, 464],
-        804: [788],
-        960: [960]
+        197: [197],
+        238: [687],
+        256: [262, 655]
     }, y = {}, k.f.consumes = (e, r) => {
         k.o(g, e) && g[e].forEach((e => {
-            if (k.o(m, e)) return r.push(m[e]);
+            if (k.o(b, e)) return r.push(b[e]);
             if (!y[e]) {
                 var t = r => {
-                    m[e] = 0, k.m[e] = t => {
+                    b[e] = 0, k.m[e] = t => {
                         delete k.c[e], t.exports = r()
                     }
                 };
                 y[e] = !0;
                 var n = r => {
-                    delete m[e], k.m[e] = t => {
+                    delete b[e], k.m[e] = t => {
                         throw delete k.c[e], r
                     }
                 };
                 try {
-                    var a = b[e]();
-                    a.then ? r.push(m[e] = a.then(t).catch(n)) : t(a)
+                    var a = m[e]();
+                    a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         k.b = document.baseURI || self.location.href;
         var e = {
-            80: 0
+            960: 0
         };
         k.f.j = (r, t) => {
             var n = k.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (/^(50|96)0$/.test(r)) e[r] = 0;
+                else if (/^(197|256)$/.test(r)) e[r] = 0;
             else {
                 var a = new Promise(((t, a) => n = e[r] = [t, a]));
                 t.push(n[2] = a);
                 var o = k.p + k.u(r),
                     i = new Error;
                 k.l(o, (t => {
                     if (k.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
@@ -283,10 +286,10 @@
                     l && l(k)
                 }
                 for (r && r(t); u < o.length; u++) a = o[u], k.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_jupyterlite_javascript_kernel_extension = self.webpackChunk_jupyterlite_javascript_kernel_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var S = k(228);
+    var S = k(291);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlite/javascript-kernel-extension"] = S
 })();
```

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/jupyterlite_javascript_kernel/labextension/static/third-party-licenses.json` & `jupyterlite_javascript_kernel-0.4.0a0/jupyterlite_javascript_kernel/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '0.4.0-alpha.0'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlite/javascript-kernel",
-            "versionInfo": "0.3.0-alpha.1"
+            "versionInfo": "0.4.0-alpha.0"
         },
         {
             "extractedText": "\n                                 Apache License\n                           Version 2.0, January 2004\n                        http://www.apache.org/licenses/\n\n   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION\n\n   1. Definitions.\n\n      \"License\" shall mean the terms and conditions for use, reproduction,\n      and distribution as defined by Sections 1 through 9 of this document.\n\n      \"Licensor\" shall mean the copyright owner or entity authorized by\n      the copyright owner that is granting the License.\n\n      \"Legal Entity\" shall mean the union of the acting entity and all\n      other entities that control, are controlled by, or are under common\n      control with that entity. For the purposes of this definition,\n      \"control\" means (i) the power, direct or indirect, to cause the\n      direction or management of such entity, whether by contract or\n      otherwise, or (ii) ownership of fifty percent (50%) or more of the\n      outstanding shares, or (iii) beneficial ownership of such entity.\n\n      \"You\" (or \"Your\") shall mean an individual or Legal Entity\n      exercising permissions granted by this License.\n\n      \"Source\" form shall mean the preferred form for making modifications,\n      including but not limited to software source code, documentation\n      source, and configuration files.\n\n      \"Object\" form shall mean any form resulting from mechanical\n      transformation or translation of a Source form, including but\n      not limited to compiled object code, generated documentation,\n      and conversions to other media types.\n\n      \"Work\" shall mean the work of authorship, whether in Source or\n      Object form, made available under the License, as indicated by a\n      copyright notice that is included in or attached to the work\n      (an example is provided in the Appendix below).\n\n      \"Derivative Works\" shall mean any work, whether in Source or Object\n      form, that is based on (or derived from) the Work and for which the\n      editorial revisions, annotations, elaborations, or other modifications\n      represent, as a whole, an original work of authorship. For the purposes\n      of this License, Derivative Works shall not include works that remain\n      separable from, or merely link (or bind by name) to the interfaces of,\n      the Work and Derivative Works thereof.\n\n      \"Contribution\" shall mean any work of authorship, including\n      the original version of the Work and any modifications or additions\n      to that Work or Derivative Works thereof, that is intentionally\n      submitted to Licensor for inclusion in the Work by the copyright owner\n      or by an individual or Legal Entity authorized to submit on behalf of\n      the copyright owner. For the purposes of this definition, \"submitted\"\n      means any form of electronic, verbal, or written communication sent\n      to the Licensor or its representatives, including but not limited to\n      communication on electronic mailing lists, source code control systems,\n      and issue tracking systems that are managed by, or on behalf of, the\n      Licensor for the purpose of discussing and improving the Work, but\n      excluding communication that is conspicuously marked or otherwise\n      designated in writing by the copyright owner as \"Not a Contribution.\"\n\n      \"Contributor\" shall mean Licensor and any individual or Legal Entity\n      on behalf of whom a Contribution has been received by Licensor and\n      subsequently incorporated within the Work.\n\n   2. Grant of Copyright License. Subject to the terms and conditions of\n      this License, each Contributor hereby grants to You a perpetual,\n      worldwide, non-exclusive, no-charge, royalty-free, irrevocable\n      copyright license to reproduce, prepare Derivative Works of,\n      publicly display, publicly perform, sublicense, and distribute the\n      Work and such Derivative Works in Source or Object form.\n\n   3. Grant of Patent License. Subject to the terms and conditions of\n      this License, each Contributor hereby grants to You a perpetual,\n      worldwide, non-exclusive, no-charge, royalty-free, irrevocable\n      (except as stated in this section) patent license to make, have made,\n      use, offer to sell, sell, import, and otherwise transfer the Work,\n      where such license applies only to those patent claims licensable\n      by such Contributor that are necessarily infringed by their\n      Contribution(s) alone or by combination of their Contribution(s)\n      with the Work to which such Contribution(s) was submitted. If You\n      institute patent litigation against any entity (including a\n      cross-claim or counterclaim in a lawsuit) alleging that the Work\n      or a Contribution incorporated within the Work constitutes direct\n      or contributory patent infringement, then any patent licenses\n      granted to You under this License for that Work shall terminate\n      as of the date such litigation is filed.\n\n   4. Redistribution. You may reproduce and distribute copies of the\n      Work or Derivative Works thereof in any medium, with or without\n      modifications, and in Source or Object form, provided that You\n      meet the following conditions:\n\n      (a) You must give any other recipients of the Work or\n          Derivative Works a copy of this License; and\n\n      (b) You must cause any modified files to carry prominent notices\n          stating that You changed the files; and\n\n      (c) You must retain, in the Source form of any Derivative Works\n          that You distribute, all copyright, patent, trademark, and\n          attribution notices from the Source form of the Work,\n          excluding those notices that do not pertain to any part of\n          the Derivative Works; and\n\n      (d) If the Work includes a \"NOTICE\" text file as part of its\n          distribution, then any Derivative Works that You distribute must\n          include a readable copy of the attribution notices contained\n          within such NOTICE file, excluding those notices that do not\n          pertain to any part of the Derivative Works, in at least one\n          of the following places: within a NOTICE text file distributed\n          as part of the Derivative Works; within the Source form or\n          documentation, if provided along with the Derivative Works; or,\n          within a display generated by the Derivative Works, if and\n          wherever such third-party notices normally appear. The contents\n          of the NOTICE file are for informational purposes only and\n          do not modify the License. You may add Your own attribution\n          notices within Derivative Works that You distribute, alongside\n          or as an addendum to the NOTICE text from the Work, provided\n          that such additional attribution notices cannot be construed\n          as modifying the License.\n\n      You may add Your own copyright statement to Your modifications and\n      may provide additional or different license terms and conditions\n      for use, reproduction, or distribution of Your modifications, or\n      for any such Derivative Works as a whole, provided Your use,\n      reproduction, and distribution of the Work otherwise complies with\n      the conditions stated in this License.\n\n   5. Submission of Contributions. Unless You explicitly state otherwise,\n      any Contribution intentionally submitted for inclusion in the Work\n      by You to the Licensor shall be under the terms and conditions of\n      this License, without any additional terms or conditions.\n      Notwithstanding the above, nothing herein shall supersede or modify\n      the terms of any separate license agreement you may have executed\n      with Licensor regarding such Contributions.\n\n   6. Trademarks. This License does not grant permission to use the trade\n      names, trademarks, service marks, or product names of the Licensor,\n      except as required for reasonable and customary use in describing the\n      origin of the Work and reproducing the content of the NOTICE file.\n\n   7. Disclaimer of Warranty. Unless required by applicable law or\n      agreed to in writing, Licensor provides the Work (and each\n      Contributor provides its Contributions) on an \"AS IS\" BASIS,\n      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or\n      implied, including, without limitation, any warranties or conditions\n      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A\n      PARTICULAR PURPOSE. You are solely responsible for determining the\n      appropriateness of using or redistributing the Work and assume any\n      risks associated with Your exercise of permissions under this License.\n\n   8. Limitation of Liability. In no event and under no legal theory,\n      whether in tort (including negligence), contract, or otherwise,\n      unless required by applicable law (such as deliberate and grossly\n      negligent acts) or agreed to in writing, shall any Contributor be\n      liable to You for damages, including any direct, indirect, special,\n      incidental, or consequential damages of any character arising as a\n      result of this License or out of the use or inability to use the\n      Work (including but not limited to damages for loss of goodwill,\n      work stoppage, computer failure or malfunction, or any and all\n      other commercial damages or losses), even if such Contributor\n      has been advised of the possibility of such damages.\n\n   9. Accepting Warranty or Additional Liability. While redistributing\n      the Work or Derivative Works thereof, You may choose to offer,\n      and charge a fee for, acceptance of support, warranty, indemnity,\n      or other liability obligations and/or rights consistent with this\n      License. However, in accepting such obligations, You may act only\n      on Your own behalf and on Your sole responsibility, not on behalf\n      of any other Contributor, and only if You agree to indemnify,\n      defend, and hold each Contributor harmless for any liability\n      incurred by, or claims asserted against, such Contributor by reason\n      of your accepting any such warranty or additional liability.\n\n   END OF TERMS AND CONDITIONS\n\n   APPENDIX: How to apply the Apache License to your work.\n\n      To apply the Apache License to your work, attach the following\n      boilerplate notice, with the fields enclosed by brackets \"[]\"\n      replaced with your own identifying information. (Don't include\n      the brackets!)  The text should be enclosed in the appropriate\n      comment syntax for the file format. We also recommend that a\n      file or class name and description of purpose be included on the\n      same \"printed page\" as the copyright notice for easier\n      identification within third-party archives.\n\n   Copyright 2017 Google Inc.\n\n   Licensed under the Apache License, Version 2.0 (the \"License\");\n   you may not use this file except in compliance with the License.\n   You may obtain a copy of the License at\n\n       http://www.apache.org/licenses/LICENSE-2.0\n\n   Unless required by applicable law or agreed to in writing, software\n   distributed under the License is distributed on an \"AS IS\" BASIS,\n   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n   See the License for the specific language governing permissions and\n   limitations under the License.",
             "licenseId": "Apache-2.0",
             "name": "comlink",
             "versionInfo": "4.4.1"
         },
```

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/scripts/bump-version.py` & `jupyterlite_javascript_kernel-0.4.0a0/scripts/bump-version.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/.gitignore` & `jupyterlite_javascript_kernel-0.4.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/LICENSE` & `jupyterlite_javascript_kernel-0.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/README.md` & `jupyterlite_javascript_kernel-0.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/pyproject.toml` & `jupyterlite_javascript_kernel-0.4.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlite_javascript_kernel-0.3.0a1/PKG-INFO` & `jupyterlite_javascript_kernel-0.4.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlite_javascript_kernel
-Version: 0.3.0a1
+Version: 0.4.0a0
+Dynamic: Keywords
 Summary: A JavaScript kernel for JupyterLite
 Project-URL: Homepage, https://github.com/jupyterlite/javascript-kernel
 Project-URL: Bug Tracker, https://github.com/jupyterlite/javascript-kernel/issues
 Project-URL: Repository, https://github.com/jupyterlite/javascript-kernel.git
 Author: JupyterLite Contributors
 License: BSD 3-Clause License
```

