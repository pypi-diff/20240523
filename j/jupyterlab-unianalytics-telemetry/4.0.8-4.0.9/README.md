# Comparing `tmp/jupyterlab_unianalytics_telemetry-4.0.8.tar.gz` & `tmp/jupyterlab_unianalytics_telemetry-4.0.9.tar.gz`

## Comparing `jupyterlab_unianalytics_telemetry-4.0.8.tar` & `jupyterlab_unianalytics_telemetry-4.0.9.tar`

### file list

```diff
@@ -1,65 +1,68 @@
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/.copier-answers.yml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/.yarnrc.yml
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/CHANGELOG.md
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/babel.config.js
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/jest.config.js
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/junit.xml
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/setup.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/tsconfig.test.json
--rw-r--r--   0        0        0   364880 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/yarn.lock
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/_version.py
--rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/package.json
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/schemas/jupyterlab_unianalytics_telemetry/dialogShownSettings.json
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/schemas/jupyterlab_unianalytics_telemetry/package.json.orig
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/schemas/jupyterlab_unianalytics_telemetry/settings.json
--rw-r--r--   0        0        0    19993 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/static/622.dfcc6f863c81bf0a5841.js
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/static/747.1caae4588978ba0392e1.js
--rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/static/remoteEntry.4c8f2b8808a7717691b7.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/schema/dialogShownSettings.json
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/schema/settings.json
--rw-r--r--   0        0        0     7593 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/PanelManager.ts
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/api.ts
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/dataCollectionPlugin.ts
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/index.ts
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/__tests__/jupyterlab_unianalytics_telemetry.spec.ts
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/icons/index.ts
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/icons/svg.d.ts
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/trackers/AlterationDisposable.ts
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/trackers/CellMappingDisposable.ts
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/trackers/ExecutionDisposable.ts
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/trackers/FocusDisposable.ts
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/trackers/InstanceInitializerDisposable.ts
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/utils/compatibility.ts
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/utils/constants.ts
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/utils/types.d.ts
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/utils/utils.ts
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/websocket/ChatExtension.ts
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/src/websocket/WebsocketManager.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/style/index.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/style/icons/chat.svg
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/style/icons/chat2.svg
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/style/icons/chat3.svg
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/style/icons/dataCollection_cropped.svg
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   152326 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/ui-tests/yarn.lock
--rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/ui-tests/tests/jupyterlab_unianalytics_telemetry.spec.ts
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/ui-tests/tests/types.ts
--rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/ui-tests/tests/utils.ts
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/LICENSE
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/README.md
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/pyproject.toml
--rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.8/PKG-INFO
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/.copier-answers.yml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/.yarnrc.yml
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/babel.config.js
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/conftest.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jest.config.js
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/junit.xml
+-rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/setup.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/tsconfig.test.json
+-rw-r--r--   0        0        0   367569 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/yarn.lock
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyter-config/server-config/jupyterlab_unianalytics_telemetry.json
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/_version.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/handlers.py
+-rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/package.json
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/schemas/jupyterlab_unianalytics_telemetry/dialogShownSettings.json
+-rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/schemas/jupyterlab_unianalytics_telemetry/package.json.orig
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/schemas/jupyterlab_unianalytics_telemetry/settings.json
+-rw-r--r--   0        0        0    19201 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/static/333.fc339a7b12932252a9bf.js
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/static/747.af77df2dd0efb547d5ac.js
+-rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/static/remoteEntry.aa29f5d9f0a6f487df86.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/tests/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/tests/test_handlers.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/schema/dialogShownSettings.json
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/schema/settings.json
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/PanelManager.ts
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/api.ts
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/dataCollectionPlugin.ts
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/handler.ts
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/index.ts
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/__tests__/jupyterlab_unianalytics_telemetry.spec.ts
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/icons/index.ts
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/icons/svg.d.ts
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/trackers/AlterationDisposable.ts
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/trackers/CellMappingDisposable.ts
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/trackers/ExecutionDisposable.ts
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/trackers/FocusDisposable.ts
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/utils/compatibility.ts
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/utils/constants.ts
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/utils/types.d.ts
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/utils/utils.ts
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/websocket/ChatExtension.ts
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/src/websocket/WebsocketManager.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/style/index.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/style/icons/chat.svg
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/style/icons/chat2.svg
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/style/icons/chat3.svg
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/style/icons/dataCollection_cropped.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   144130 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/ui-tests/tests/jupyterlab_unianalytics_telemetry.spec.ts
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/LICENSE
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/README.md
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 jupyterlab_unianalytics_telemetry-4.0.9/PKG-INFO
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/.copier-answers.yml` & `jupyterlab_unianalytics_telemetry-4.0.9/.copier-answers.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Changes here will be overwritten by Copier; NEVER EDIT MANUALLY
-_commit: v4.0.5
+_commit: v4.2.5
 _src_path: https://github.com/jupyterlab/extension-template
-author_email: me@test.com
+author_email: raphael.marietan@hotmail.com
 author_name: Raphael Marietan
 data_format: string
 file_extension: ''
 has_binder: true
 has_settings: true
-kind: frontend
+kind: server
 labextension_name: jupyterlab_unianalytics_telemetry
 mimetype: ''
 mimetype_name: ''
-project_short_description:
-  A JupyterLab extension to send notebook execution and activity
-  to a self-hosted backend.
+project_short_description: A JupyterLab extension to send notebook interaction data
+    to a backend.
 python_name: jupyterlab_unianalytics_telemetry
 repository: https://github.com/chili-epfl/jupyter-dashboard-send-extension
 test: true
 viewer_name: ''
+
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/CHANGELOG.md` & `jupyterlab_unianalytics_telemetry-4.0.9/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
-## 4.0.8
+## 4.0.9
 
-Removing redundant encryption
+- Adding server extension component
+- Generating or retrieving persistent user identifier
+- Small bug fixes
 
 <!-- <END NEW CHANGELOG ENTRY> -->
 
+## 4.0.8
+
+Removing redundant encryption
+
 ## 4.0.7
 
 Changes since last release:
 
 - Major refactor using PanelManager.
 - Disabling sending of data when user is also using the dashboard extension and is authorized to view that notebook's dashboard.
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/jest.config.js` & `jupyterlab_unianalytics_telemetry-4.0.9/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/package.json` & `jupyterlab_unianalytics_telemetry-4.0.9/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.907142857142857%*

 * *Differences: {"'author'": "{'email': 'raphael.marietan@hotmail.com'}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/settingregistry': '^4.0.0', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.0', '@jupyterlab/services': '^7.0.0'}",*

 * * "'description'": "'A JupyterLab extension to send notebook interaction data to a backend.'",*

 * * "'devDependencies'": "{'@typescript-eslint/eslint-plugin': '^6.1.0', '@typescript-eslint/parser': "*

 * *                      "'^6.1.0', 'eslint-config-prettier': '^8.8.0' […]*

```diff
@@ -1,44 +1,47 @@
 {
     "author": {
-        "email": "me@test.com",
+        "email": "raphael.marietan@hotmail.com",
         "name": "Raphael Marietan"
     },
     "bugs": {
         "url": "https://github.com/chili-epfl/jupyter-dashboard-send-extension/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0 || ^4.0.0",
-        "@jupyterlab/settingregistry": "^3.1.0 || ^4.0.0"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0"
     },
-    "description": "A JupyterLab extension to send notebook execution and activity to a self-hosted backend.",
+    "description": "A JupyterLab extension to send notebook interaction data to a backend.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
-        "@types/crypto-js": "^4.1.2",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
-        "@typescript-eslint/eslint-plugin": "^5.55.0",
-        "@typescript-eslint/parser": "^5.55.0",
+        "@types/react-addons-linked-state-mixin": "^0.14.22",
+        "@typescript-eslint/eslint-plugin": "^6.1.0",
+        "@typescript-eslint/parser": "^6.1.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
-        "eslint-config-prettier": "^8.7.0",
-        "eslint-plugin-prettier": "^4.2.1",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^5.0.0",
         "jest": "^29.2.0",
+        "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.8.7",
-        "rimraf": "^4.4.1",
+        "prettier": "^3.0.0",
+        "rimraf": "^5.0.1",
         "source-map-loader": "^1.0.2",
         "style-loader": "^3.3.1",
-        "stylelint": "^14.9.1",
-        "stylelint-config-prettier": "^9.0.4",
-        "stylelint-config-recommended": "^8.0.0",
-        "stylelint-config-standard": "^26.0.0",
-        "stylelint-prettier": "^2.0.0",
+        "stylelint": "^15.10.1",
+        "stylelint-config-recommended": "^13.0.0",
+        "stylelint-config-standard": "^34.0.0",
+        "stylelint-csstree-validator": "^3.0.0",
+        "stylelint-prettier": "^4.0.0",
         "typescript": "~5.0.2",
         "yjs": "^13.5.0"
     },
     "eslintConfig": {
         "extends": [
             "eslint:recommended",
             "plugin:@typescript-eslint/eslint-recommended",
@@ -100,18 +103,29 @@
         "tests",
         "**/__tests__",
         "ui-tests"
     ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/chili-epfl/jupyter-dashboard-send-extension",
     "jupyterlab": {
+        "discovery": {
+            "server": {
+                "base": {
+                    "name": "jupyterlab_unianalytics_telemetry"
+                },
+                "managers": [
+                    "pip"
+                ]
+            }
+        },
         "extension": true,
         "outputDir": "jupyterlab_unianalytics_telemetry/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -119,14 +133,22 @@
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "jupyterlab_unianalytics_telemetry",
     "prettier": {
         "arrowParens": "avoid",
         "endOfLine": "auto",
+        "overrides": [
+            {
+                "files": "package.json",
+                "options": {
+                    "tabWidth": 4
+                }
+            }
+        ],
         "singleQuote": true,
         "trailingComma": "none"
     },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
@@ -168,16 +190,21 @@
     "styleModule": "style/index.js",
     "stylelint": {
         "extends": [
             "stylelint-config-recommended",
             "stylelint-config-standard",
             "stylelint-prettier/recommended"
         ],
+        "plugins": [
+            "stylelint-csstree-validator"
+        ],
         "rules": {
+            "csstree/validator": true,
             "property-no-vendor-prefix": null,
+            "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.8"
+    "version": "4.0.9"
 }
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/tsconfig.json` & `jupyterlab_unianalytics_telemetry-4.0.9/tsconfig.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868421052631579%*

 * *Differences: {"'compilerOptions'": "{delete: ['types']}"}*

```diff
@@ -13,18 +13,15 @@
         "noUnusedLocals": false,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "ES2018",
-        "types": [
-            "jest"
-        ]
+        "target": "ES2018"
     },
     "include": [
         "src/*",
         "src/utils/*",
         "src/icons/*",
         "src/websocket/*",
         "src/trackers/*"
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/yarn.lock` & `jupyterlab_unianalytics_telemetry-4.0.9/yarn.lock`

 * *Files 2% similar despite different names*

```diff
@@ -18,145 +18,145 @@
   dependencies:
     "@jridgewell/gen-mapping": ^0.3.0
     "@jridgewell/trace-mapping": ^0.3.9
   checksum: 03c04fd526acc64a1f4df22651186f3e5ef0a9d6d6530ce4482ec9841269cf7a11dbb8af79237c282d721c5312024ff17529cd72cc4768c11e999b58e2302079
   languageName: node
   linkType: hard
 
-"@babel/code-frame@npm:^7.0.0, @babel/code-frame@npm:^7.12.13, @babel/code-frame@npm:^7.22.13":
-  version: 7.22.13
-  resolution: "@babel/code-frame@npm:7.22.13"
+"@babel/code-frame@npm:^7.0.0, @babel/code-frame@npm:^7.12.13, @babel/code-frame@npm:^7.23.5":
+  version: 7.23.5
+  resolution: "@babel/code-frame@npm:7.23.5"
   dependencies:
-    "@babel/highlight": ^7.22.13
+    "@babel/highlight": ^7.23.4
     chalk: ^2.4.2
-  checksum: 22e342c8077c8b77eeb11f554ecca2ba14153f707b85294fcf6070b6f6150aae88a7b7436dd88d8c9289970585f3fe5b9b941c5aa3aa26a6d5a8ef3f292da058
+  checksum: d90981fdf56a2824a9b14d19a4c0e8db93633fd488c772624b4e83e0ceac6039a27cd298a247c3214faa952bf803ba23696172ae7e7235f3b97f43ba278c569a
   languageName: node
   linkType: hard
 
-"@babel/compat-data@npm:^7.22.6, @babel/compat-data@npm:^7.22.9, @babel/compat-data@npm:^7.23.2":
-  version: 7.23.2
-  resolution: "@babel/compat-data@npm:7.23.2"
-  checksum: d8dc27437d40907b271161d4c88ffe72ccecb034c730deb1960a417b59a14d7c5ebca8cd80dd458a01cd396a7a329eb48cddcc3791b5a84da33d7f278f7bec6a
+"@babel/compat-data@npm:^7.22.6, @babel/compat-data@npm:^7.23.3, @babel/compat-data@npm:^7.23.5":
+  version: 7.23.5
+  resolution: "@babel/compat-data@npm:7.23.5"
+  checksum: 06ce244cda5763295a0ea924728c09bae57d35713b675175227278896946f922a63edf803c322f855a3878323d48d0255a2a3023409d2a123483c8a69ebb4744
   languageName: node
   linkType: hard
 
 "@babel/core@npm:^7.10.2, @babel/core@npm:^7.11.6, @babel/core@npm:^7.12.3":
-  version: 7.23.2
-  resolution: "@babel/core@npm:7.23.2"
+  version: 7.23.9
+  resolution: "@babel/core@npm:7.23.9"
   dependencies:
     "@ampproject/remapping": ^2.2.0
-    "@babel/code-frame": ^7.22.13
-    "@babel/generator": ^7.23.0
-    "@babel/helper-compilation-targets": ^7.22.15
-    "@babel/helper-module-transforms": ^7.23.0
-    "@babel/helpers": ^7.23.2
-    "@babel/parser": ^7.23.0
-    "@babel/template": ^7.22.15
-    "@babel/traverse": ^7.23.2
-    "@babel/types": ^7.23.0
+    "@babel/code-frame": ^7.23.5
+    "@babel/generator": ^7.23.6
+    "@babel/helper-compilation-targets": ^7.23.6
+    "@babel/helper-module-transforms": ^7.23.3
+    "@babel/helpers": ^7.23.9
+    "@babel/parser": ^7.23.9
+    "@babel/template": ^7.23.9
+    "@babel/traverse": ^7.23.9
+    "@babel/types": ^7.23.9
     convert-source-map: ^2.0.0
     debug: ^4.1.0
     gensync: ^1.0.0-beta.2
     json5: ^2.2.3
     semver: ^6.3.1
-  checksum: 003897718ded16f3b75632d63cd49486bf67ff206cc7ebd1a10d49e2456f8d45740910d5ec7e42e3faf0deec7a2e96b1a02e766d19a67a8309053f0d4e57c0fe
+  checksum: 634a511f74db52a5f5a283c1121f25e2227b006c095b84a02a40a9213842489cd82dc7d61cdc74e10b5bcd9bb0a4e28bab47635b54c7e2256d47ab57356e2a76
   languageName: node
   linkType: hard
 
-"@babel/generator@npm:^7.23.0, @babel/generator@npm:^7.7.2":
-  version: 7.23.0
-  resolution: "@babel/generator@npm:7.23.0"
+"@babel/generator@npm:^7.23.6, @babel/generator@npm:^7.7.2":
+  version: 7.23.6
+  resolution: "@babel/generator@npm:7.23.6"
   dependencies:
-    "@babel/types": ^7.23.0
+    "@babel/types": ^7.23.6
     "@jridgewell/gen-mapping": ^0.3.2
     "@jridgewell/trace-mapping": ^0.3.17
     jsesc: ^2.5.1
-  checksum: 8efe24adad34300f1f8ea2add420b28171a646edc70f2a1b3e1683842f23b8b7ffa7e35ef0119294e1901f45bfea5b3dc70abe1f10a1917ccdfb41bed69be5f1
+  checksum: 1a1a1c4eac210f174cd108d479464d053930a812798e09fee069377de39a893422df5b5b146199ead7239ae6d3a04697b45fc9ac6e38e0f6b76374390f91fc6c
   languageName: node
   linkType: hard
 
 "@babel/helper-annotate-as-pure@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-annotate-as-pure@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: 53da330f1835c46f26b7bf4da31f7a496dee9fd8696cca12366b94ba19d97421ce519a74a837f687749318f94d1a37f8d1abcbf35e8ed22c32d16373b2f6198d
   languageName: node
   linkType: hard
 
-"@babel/helper-builder-binary-assignment-operator-visitor@npm:^7.22.5":
+"@babel/helper-builder-binary-assignment-operator-visitor@npm:^7.22.15":
   version: 7.22.15
   resolution: "@babel/helper-builder-binary-assignment-operator-visitor@npm:7.22.15"
   dependencies:
     "@babel/types": ^7.22.15
   checksum: 639c697a1c729f9fafa2dd4c9af2e18568190299b5907bd4c2d0bc818fcbd1e83ffeecc2af24327a7faa7ac4c34edd9d7940510a5e66296c19bad17001cf5c7a
   languageName: node
   linkType: hard
 
-"@babel/helper-compilation-targets@npm:^7.22.15, @babel/helper-compilation-targets@npm:^7.22.5, @babel/helper-compilation-targets@npm:^7.22.6":
-  version: 7.22.15
-  resolution: "@babel/helper-compilation-targets@npm:7.22.15"
-  dependencies:
-    "@babel/compat-data": ^7.22.9
-    "@babel/helper-validator-option": ^7.22.15
-    browserslist: ^4.21.9
+"@babel/helper-compilation-targets@npm:^7.22.15, @babel/helper-compilation-targets@npm:^7.22.6, @babel/helper-compilation-targets@npm:^7.23.6":
+  version: 7.23.6
+  resolution: "@babel/helper-compilation-targets@npm:7.23.6"
+  dependencies:
+    "@babel/compat-data": ^7.23.5
+    "@babel/helper-validator-option": ^7.23.5
+    browserslist: ^4.22.2
     lru-cache: ^5.1.1
     semver: ^6.3.1
-  checksum: ce85196769e091ae54dd39e4a80c2a9df1793da8588e335c383d536d54f06baf648d0a08fc873044f226398c4ded15c4ae9120ee18e7dfd7c639a68e3cdc9980
+  checksum: c630b98d4527ac8fe2c58d9a06e785dfb2b73ec71b7c4f2ddf90f814b5f75b547f3c015f110a010fd31f76e3864daaf09f3adcd2f6acdbfb18a8de3a48717590
   languageName: node
   linkType: hard
 
-"@babel/helper-create-class-features-plugin@npm:^7.22.11, @babel/helper-create-class-features-plugin@npm:^7.22.5":
-  version: 7.22.15
-  resolution: "@babel/helper-create-class-features-plugin@npm:7.22.15"
+"@babel/helper-create-class-features-plugin@npm:^7.22.15":
+  version: 7.23.9
+  resolution: "@babel/helper-create-class-features-plugin@npm:7.23.9"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
-    "@babel/helper-environment-visitor": ^7.22.5
-    "@babel/helper-function-name": ^7.22.5
-    "@babel/helper-member-expression-to-functions": ^7.22.15
+    "@babel/helper-environment-visitor": ^7.22.20
+    "@babel/helper-function-name": ^7.23.0
+    "@babel/helper-member-expression-to-functions": ^7.23.0
     "@babel/helper-optimise-call-expression": ^7.22.5
-    "@babel/helper-replace-supers": ^7.22.9
+    "@babel/helper-replace-supers": ^7.22.20
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
     "@babel/helper-split-export-declaration": ^7.22.6
     semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: 52c500d8d164abb3a360b1b7c4b8fff77bc4a5920d3a2b41ae6e1d30617b0dc0b972c1f5db35b1752007e04a748908b4a99bc872b73549ae837e87dcdde005a3
+  checksum: 0f0c8592ec8833c0fd1d131655de929af07942fd626049d1e8fae5d85c1fe33fad97f7e9457a14b10258bc926a0cb39debc54a553abe8b4f7575c446d1c16d80
   languageName: node
   linkType: hard
 
-"@babel/helper-create-regexp-features-plugin@npm:^7.18.6, @babel/helper-create-regexp-features-plugin@npm:^7.22.5":
+"@babel/helper-create-regexp-features-plugin@npm:^7.18.6, @babel/helper-create-regexp-features-plugin@npm:^7.22.15, @babel/helper-create-regexp-features-plugin@npm:^7.22.5":
   version: 7.22.15
   resolution: "@babel/helper-create-regexp-features-plugin@npm:7.22.15"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
     regexpu-core: ^5.3.1
     semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: 0243b8d4854f1dc8861b1029a46d3f6393ad72f366a5a08e36a4648aa682044f06da4c6e87a456260e1e1b33c999f898ba591a0760842c1387bcc93fbf2151a6
   languageName: node
   linkType: hard
 
-"@babel/helper-define-polyfill-provider@npm:^0.4.3":
-  version: 0.4.3
-  resolution: "@babel/helper-define-polyfill-provider@npm:0.4.3"
+"@babel/helper-define-polyfill-provider@npm:^0.5.0":
+  version: 0.5.0
+  resolution: "@babel/helper-define-polyfill-provider@npm:0.5.0"
   dependencies:
     "@babel/helper-compilation-targets": ^7.22.6
     "@babel/helper-plugin-utils": ^7.22.5
     debug: ^4.1.1
     lodash.debounce: ^4.0.8
     resolve: ^1.14.2
   peerDependencies:
     "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
-  checksum: 5d21e3f47b320e4b5b644195ec405e7ebc3739e48e65899efc808c5fa9c3bf5b06ce0d8ff5246ca99d1411e368f4557bc66730196c5781a5c4e986ee703bee79
+  checksum: d24626b819d3875cb65189d761004e9230f2b3fb60542525c4785616f4b2366741369235a864b744f54beb26d625ae4b0af0c9bb3306b61bf4fccb61e0620020
   languageName: node
   linkType: hard
 
-"@babel/helper-environment-visitor@npm:^7.22.20, @babel/helper-environment-visitor@npm:^7.22.5":
+"@babel/helper-environment-visitor@npm:^7.22.20":
   version: 7.22.20
   resolution: "@babel/helper-environment-visitor@npm:7.22.20"
   checksum: d80ee98ff66f41e233f36ca1921774c37e88a803b2f7dca3db7c057a5fea0473804db9fb6729e5dbfd07f4bed722d60f7852035c2c739382e84c335661590b69
   languageName: node
   linkType: hard
 
 "@babel/helper-function-name@npm:^7.22.5, @babel/helper-function-name@npm:^7.23.0":
@@ -174,44 +174,44 @@
   resolution: "@babel/helper-hoist-variables@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: 394ca191b4ac908a76e7c50ab52102669efe3a1c277033e49467913c7ed6f7c64d7eacbeabf3bed39ea1f41731e22993f763b1edce0f74ff8563fd1f380d92cc
   languageName: node
   linkType: hard
 
-"@babel/helper-member-expression-to-functions@npm:^7.22.15":
+"@babel/helper-member-expression-to-functions@npm:^7.22.15, @babel/helper-member-expression-to-functions@npm:^7.23.0":
   version: 7.23.0
   resolution: "@babel/helper-member-expression-to-functions@npm:7.23.0"
   dependencies:
     "@babel/types": ^7.23.0
   checksum: 494659361370c979ada711ca685e2efe9460683c36db1b283b446122596602c901e291e09f2f980ecedfe6e0f2bd5386cb59768285446530df10c14df1024e75
   languageName: node
   linkType: hard
 
-"@babel/helper-module-imports@npm:^7.22.15, @babel/helper-module-imports@npm:^7.22.5":
+"@babel/helper-module-imports@npm:^7.22.15":
   version: 7.22.15
   resolution: "@babel/helper-module-imports@npm:7.22.15"
   dependencies:
     "@babel/types": ^7.22.15
   checksum: ecd7e457df0a46f889228f943ef9b4a47d485d82e030676767e6a2fdcbdaa63594d8124d4b55fd160b41c201025aec01fc27580352b1c87a37c9c6f33d116702
   languageName: node
   linkType: hard
 
-"@babel/helper-module-transforms@npm:^7.22.5, @babel/helper-module-transforms@npm:^7.23.0":
-  version: 7.23.0
-  resolution: "@babel/helper-module-transforms@npm:7.23.0"
+"@babel/helper-module-transforms@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/helper-module-transforms@npm:7.23.3"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.20
     "@babel/helper-module-imports": ^7.22.15
     "@babel/helper-simple-access": ^7.22.5
     "@babel/helper-split-export-declaration": ^7.22.6
     "@babel/helper-validator-identifier": ^7.22.20
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: 6e2afffb058cf3f8ce92f5116f710dda4341c81cfcd872f9a0197ea594f7ce0ab3cb940b0590af2fe99e60d2e5448bfba6bca8156ed70a2ed4be2adc8586c891
+  checksum: 5d0895cfba0e16ae16f3aa92fee108517023ad89a855289c4eb1d46f7aef4519adf8e6f971e1d55ac20c5461610e17213f1144097a8f932e768a9132e2278d71
   languageName: node
   linkType: hard
 
 "@babel/helper-optimise-call-expression@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-optimise-call-expression@npm:7.22.5"
   dependencies:
@@ -223,28 +223,28 @@
 "@babel/helper-plugin-utils@npm:^7.0.0, @babel/helper-plugin-utils@npm:^7.10.4, @babel/helper-plugin-utils@npm:^7.12.13, @babel/helper-plugin-utils@npm:^7.14.5, @babel/helper-plugin-utils@npm:^7.18.6, @babel/helper-plugin-utils@npm:^7.22.5, @babel/helper-plugin-utils@npm:^7.8.0, @babel/helper-plugin-utils@npm:^7.8.3":
   version: 7.22.5
   resolution: "@babel/helper-plugin-utils@npm:7.22.5"
   checksum: c0fc7227076b6041acd2f0e818145d2e8c41968cc52fb5ca70eed48e21b8fe6dd88a0a91cbddf4951e33647336eb5ae184747ca706817ca3bef5e9e905151ff5
   languageName: node
   linkType: hard
 
-"@babel/helper-remap-async-to-generator@npm:^7.22.20, @babel/helper-remap-async-to-generator@npm:^7.22.5":
+"@babel/helper-remap-async-to-generator@npm:^7.22.20":
   version: 7.22.20
   resolution: "@babel/helper-remap-async-to-generator@npm:7.22.20"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
     "@babel/helper-environment-visitor": ^7.22.20
     "@babel/helper-wrap-function": ^7.22.20
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: 2fe6300a6f1b58211dffa0aed1b45d4958506d096543663dba83bd9251fe8d670fa909143a65b45e72acb49e7e20fbdb73eae315d9ddaced467948c3329986e7
   languageName: node
   linkType: hard
 
-"@babel/helper-replace-supers@npm:^7.22.5, @babel/helper-replace-supers@npm:^7.22.9":
+"@babel/helper-replace-supers@npm:^7.22.20":
   version: 7.22.20
   resolution: "@babel/helper-replace-supers@npm:7.22.20"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.20
     "@babel/helper-member-expression-to-functions": ^7.22.15
     "@babel/helper-optimise-call-expression": ^7.22.5
   peerDependencies:
@@ -276,98 +276,110 @@
   resolution: "@babel/helper-split-export-declaration@npm:7.22.6"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: e141cace583b19d9195f9c2b8e17a3ae913b7ee9b8120246d0f9ca349ca6f03cb2c001fd5ec57488c544347c0bb584afec66c936511e447fd20a360e591ac921
   languageName: node
   linkType: hard
 
-"@babel/helper-string-parser@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/helper-string-parser@npm:7.22.5"
-  checksum: 836851ca5ec813077bbb303acc992d75a360267aa3b5de7134d220411c852a6f17de7c0d0b8c8dcc0f567f67874c00f4528672b2a4f1bc978a3ada64c8c78467
+"@babel/helper-string-parser@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/helper-string-parser@npm:7.23.4"
+  checksum: c0641144cf1a7e7dc93f3d5f16d5327465b6cf5d036b48be61ecba41e1eece161b48f46b7f960951b67f8c3533ce506b16dece576baef4d8b3b49f8c65410f90
   languageName: node
   linkType: hard
 
 "@babel/helper-validator-identifier@npm:^7.22.20":
   version: 7.22.20
   resolution: "@babel/helper-validator-identifier@npm:7.22.20"
   checksum: 136412784d9428266bcdd4d91c32bcf9ff0e8d25534a9d94b044f77fe76bc50f941a90319b05aafd1ec04f7d127cd57a179a3716009ff7f3412ef835ada95bdc
   languageName: node
   linkType: hard
 
-"@babel/helper-validator-option@npm:^7.22.15":
-  version: 7.22.15
-  resolution: "@babel/helper-validator-option@npm:7.22.15"
-  checksum: 68da52b1e10002a543161494c4bc0f4d0398c8fdf361d5f7f4272e95c45d5b32d974896d44f6a0ea7378c9204988879d73613ca683e13bd1304e46d25ff67a8d
+"@babel/helper-validator-option@npm:^7.23.5":
+  version: 7.23.5
+  resolution: "@babel/helper-validator-option@npm:7.23.5"
+  checksum: 537cde2330a8aede223552510e8a13e9c1c8798afee3757995a7d4acae564124fe2bf7e7c3d90d62d3657434a74340a274b3b3b1c6f17e9a2be1f48af29cb09e
   languageName: node
   linkType: hard
 
 "@babel/helper-wrap-function@npm:^7.22.20":
   version: 7.22.20
   resolution: "@babel/helper-wrap-function@npm:7.22.20"
   dependencies:
     "@babel/helper-function-name": ^7.22.5
     "@babel/template": ^7.22.15
     "@babel/types": ^7.22.19
   checksum: 221ed9b5572612aeb571e4ce6a256f2dee85b3c9536f1dd5e611b0255e5f59a3d0ec392d8d46d4152149156a8109f92f20379b1d6d36abb613176e0e33f05fca
   languageName: node
   linkType: hard
 
-"@babel/helpers@npm:^7.23.2":
-  version: 7.23.2
-  resolution: "@babel/helpers@npm:7.23.2"
+"@babel/helpers@npm:^7.23.9":
+  version: 7.23.9
+  resolution: "@babel/helpers@npm:7.23.9"
   dependencies:
-    "@babel/template": ^7.22.15
-    "@babel/traverse": ^7.23.2
-    "@babel/types": ^7.23.0
-  checksum: aaf4828df75ec460eaa70e5c9f66e6dadc28dae3728ddb7f6c13187dbf38030e142194b83d81aa8a31bbc35a5529a5d7d3f3cf59d5d0b595f5dd7f9d8f1ced8e
+    "@babel/template": ^7.23.9
+    "@babel/traverse": ^7.23.9
+    "@babel/types": ^7.23.9
+  checksum: 2678231192c0471dbc2fc403fb19456cc46b1afefcfebf6bc0f48b2e938fdb0fef2e0fe90c8c8ae1f021dae5012b700372e4b5d15867f1d7764616532e4a6324
   languageName: node
   linkType: hard
 
-"@babel/highlight@npm:^7.22.13":
-  version: 7.22.20
-  resolution: "@babel/highlight@npm:7.22.20"
+"@babel/highlight@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/highlight@npm:7.23.4"
   dependencies:
     "@babel/helper-validator-identifier": ^7.22.20
     chalk: ^2.4.2
     js-tokens: ^4.0.0
-  checksum: 84bd034dca309a5e680083cd827a766780ca63cef37308404f17653d32366ea76262bd2364b2d38776232f2d01b649f26721417d507e8b4b6da3e4e739f6d134
+  checksum: 643acecdc235f87d925979a979b539a5d7d1f31ae7db8d89047269082694122d11aa85351304c9c978ceeb6d250591ccadb06c366f358ccee08bb9c122476b89
   languageName: node
   linkType: hard
 
-"@babel/parser@npm:^7.1.0, @babel/parser@npm:^7.14.7, @babel/parser@npm:^7.20.7, @babel/parser@npm:^7.22.15, @babel/parser@npm:^7.23.0":
-  version: 7.23.0
-  resolution: "@babel/parser@npm:7.23.0"
+"@babel/parser@npm:^7.1.0, @babel/parser@npm:^7.14.7, @babel/parser@npm:^7.20.7, @babel/parser@npm:^7.23.9":
+  version: 7.23.9
+  resolution: "@babel/parser@npm:7.23.9"
   bin:
     parser: ./bin/babel-parser.js
-  checksum: 453fdf8b9e2c2b7d7b02139e0ce003d1af21947bbc03eb350fb248ee335c9b85e4ab41697ddbdd97079698de825a265e45a0846bb2ed47a2c7c1df833f42a354
+  checksum: e7cd4960ac8671774e13803349da88d512f9292d7baa952173260d3e8f15620a28a3701f14f709d769209022f9e7b79965256b8be204fc550cfe783cdcabe7c7
   languageName: node
   linkType: hard
 
-"@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:^7.22.15":
-  version: 7.22.15
-  resolution: "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:7.22.15"
+"@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: 8910ca21a7ec7c06f7b247d4b86c97c5aa15ef321518f44f6f490c5912fdf82c605aaa02b90892e375d82ccbedeadfdeadd922c1b836c9dd4c596871bf654753
+  checksum: ddbaf2c396b7780f15e80ee01d6dd790db076985f3dfeb6527d1a8d4cacf370e49250396a3aa005b2c40233cac214a106232f83703d5e8491848bde273938232
   languageName: node
   linkType: hard
 
-"@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:^7.22.15":
-  version: 7.22.15
-  resolution: "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:7.22.15"
+"@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
-    "@babel/plugin-transform-optional-chaining": ^7.22.15
+    "@babel/plugin-transform-optional-chaining": ^7.23.3
   peerDependencies:
     "@babel/core": ^7.13.0
-  checksum: fbefedc0da014c37f1a50a8094ce7dbbf2181ae93243f23d6ecba2499b5b20196c2124d6a4dfe3e9e0125798e80593103e456352a4beb4e5c6f7c75efb80fdac
+  checksum: 434b9d710ae856fa1a456678cc304fbc93915af86d581ee316e077af746a709a741ea39d7e1d4f5b98861b629cc7e87f002d3138f5e836775632466d4c74aef2
+  languageName: node
+  linkType: hard
+
+"@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly@npm:^7.23.7":
+  version: 7.23.7
+  resolution: "@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly@npm:7.23.7"
+  dependencies:
+    "@babel/helper-environment-visitor": ^7.22.20
+    "@babel/helper-plugin-utils": ^7.22.5
+  peerDependencies:
+    "@babel/core": ^7.0.0
+  checksum: f88e400b548202a6f8c5dfd25bc4949a13ea1ccb64a170d7dea4deaa655a0fcb001d3fd61c35e1ad9c09a3d5f0d43f783400425471fe6d660ccaf33dabea9aba
   languageName: node
   linkType: hard
 
 "@babel/plugin-proposal-private-property-in-object@npm:7.21.0-placeholder-for-preset-env.2":
   version: 7.21.0-placeholder-for-preset-env.2
   resolution: "@babel/plugin-proposal-private-property-in-object@npm:7.21.0-placeholder-for-preset-env.2"
   peerDependencies:
@@ -438,33 +450,33 @@
     "@babel/helper-plugin-utils": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: 85740478be5b0de185228e7814451d74ab8ce0a26fcca7613955262a26e99e8e15e9da58f60c754b84515d4c679b590dbd3f2148f0f58025f4ae706f1c5a5d4a
   languageName: node
   linkType: hard
 
-"@babel/plugin-syntax-import-assertions@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-syntax-import-assertions@npm:7.22.5"
+"@babel/plugin-syntax-import-assertions@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-syntax-import-assertions@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 2b8b5572db04a7bef1e6cd20debf447e4eef7cb012616f5eceb8fa3e23ce469b8f76ee74fd6d1e158ba17a8f58b0aec579d092fb67c5a30e83ccfbc5754916c1
+  checksum: 883e6b35b2da205138caab832d54505271a3fee3fc1e8dc0894502434fc2b5d517cbe93bbfbfef8068a0fb6ec48ebc9eef3f605200a489065ba43d8cddc1c9a7
   languageName: node
   linkType: hard
 
-"@babel/plugin-syntax-import-attributes@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-syntax-import-attributes@npm:7.22.5"
+"@babel/plugin-syntax-import-attributes@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-syntax-import-attributes@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 197b3c5ea2a9649347f033342cb222ab47f4645633695205c0250c6bf2af29e643753b8bb24a2db39948bef08e7c540babfd365591eb57fc110cb30b425ffc47
+  checksum: 9aed7661ffb920ca75df9f494757466ca92744e43072e0848d87fa4aa61a3f2ee5a22198ac1959856c036434b5614a8f46f1fb70298835dbe28220cdd1d4c11e
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-import-meta@npm:^7.10.4, @babel/plugin-syntax-import-meta@npm:^7.8.3":
   version: 7.10.4
   resolution: "@babel/plugin-syntax-import-meta@npm:7.10.4"
   dependencies:
@@ -483,21 +495,21 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: bf5aea1f3188c9a507e16efe030efb996853ca3cadd6512c51db7233cc58f3ac89ff8c6bdfb01d30843b161cfe7d321e1bf28da82f7ab8d7e6bc5464666f354a
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-jsx@npm:^7.7.2":
-  version: 7.22.5
-  resolution: "@babel/plugin-syntax-jsx@npm:7.22.5"
+  version: 7.23.3
+  resolution: "@babel/plugin-syntax-jsx@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 8829d30c2617ab31393d99cec2978e41f014f4ac6f01a1cecf4c4dd8320c3ec12fdc3ce121126b2d8d32f6887e99ca1a0bad53dedb1e6ad165640b92b24980ce
+  checksum: 89037694314a74e7f0e7a9c8d3793af5bf6b23d80950c29b360db1c66859d67f60711ea437e70ad6b5b4b29affe17eababda841b6c01107c2b638e0493bafb4e
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-logical-assignment-operators@npm:^7.10.4, @babel/plugin-syntax-logical-assignment-operators@npm:^7.8.3":
   version: 7.10.4
   resolution: "@babel/plugin-syntax-logical-assignment-operators@npm:7.10.4"
   dependencies:
@@ -582,21 +594,21 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: bbd1a56b095be7820029b209677b194db9b1d26691fe999856462e66b25b281f031f3dfd91b1619e9dcf95bebe336211833b854d0fb8780d618e35667c2d0d7e
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-typescript@npm:^7.7.2":
-  version: 7.22.5
-  resolution: "@babel/plugin-syntax-typescript@npm:7.22.5"
+  version: 7.23.3
+  resolution: "@babel/plugin-syntax-typescript@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 8ab7718fbb026d64da93681a57797d60326097fd7cb930380c8bffd9eb101689e90142c760a14b51e8e69c88a73ba3da956cb4520a3b0c65743aee5c71ef360a
+  checksum: abfad3a19290d258b028e285a1f34c9b8a0cbe46ef79eafed4ed7ffce11b5d0720b5e536c82f91cbd8442cde35a3dd8e861fa70366d87ff06fdc0d4756e30876
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-unicode-sets-regex@npm:^7.18.6":
   version: 7.18.6
   resolution: "@babel/plugin-syntax-unicode-sets-regex@npm:7.18.6"
   dependencies:
@@ -604,318 +616,318 @@
     "@babel/helper-plugin-utils": ^7.18.6
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: a651d700fe63ff0ddfd7186f4ebc24447ca734f114433139e3c027bc94a900d013cf1ef2e2db8430425ba542e39ae160c3b05f06b59fd4656273a3df97679e9c
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-arrow-functions@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-arrow-functions@npm:7.22.5"
+"@babel/plugin-transform-arrow-functions@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-arrow-functions@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 35abb6c57062802c7ce8bd96b2ef2883e3124370c688bbd67609f7d2453802fb73944df8808f893b6c67de978eb2bcf87bbfe325e46d6f39b5fcb09ece11d01a
+  checksum: 1e99118176e5366c2636064d09477016ab5272b2a92e78b8edb571d20bc3eaa881789a905b20042942c3c2d04efc530726cf703f937226db5ebc495f5d067e66
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-async-generator-functions@npm:^7.23.2":
-  version: 7.23.2
-  resolution: "@babel/plugin-transform-async-generator-functions@npm:7.23.2"
+"@babel/plugin-transform-async-generator-functions@npm:^7.23.9":
+  version: 7.23.9
+  resolution: "@babel/plugin-transform-async-generator-functions@npm:7.23.9"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.20
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/helper-remap-async-to-generator": ^7.22.20
     "@babel/plugin-syntax-async-generators": ^7.8.4
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: e1abae0edcda7304d7c17702ac25a127578791b89c4f767d60589249fa3e50ec33f8c9ff39d3d8d41f00b29947654eaddd4fd586e04c4d598122db745fab2868
+  checksum: d402494087a6b803803eb5ab46b837aab100a04c4c5148e38bfa943ea1bbfc1ecfb340f1ced68972564312d3580f550c125f452372e77607a558fbbaf98c31c0
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-async-to-generator@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-async-to-generator@npm:7.22.5"
+"@babel/plugin-transform-async-to-generator@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-async-to-generator@npm:7.23.3"
   dependencies:
-    "@babel/helper-module-imports": ^7.22.5
+    "@babel/helper-module-imports": ^7.22.15
     "@babel/helper-plugin-utils": ^7.22.5
-    "@babel/helper-remap-async-to-generator": ^7.22.5
+    "@babel/helper-remap-async-to-generator": ^7.22.20
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: b95f23f99dcb379a9f0a1c2a3bbea3f8dc0e1b16dc1ac8b484fe378370169290a7a63d520959a9ba1232837cf74a80e23f6facbe14fd42a3cda6d3c2d7168e62
+  checksum: 2e9d9795d4b3b3d8090332104e37061c677f29a1ce65bcbda4099a32d243e5d9520270a44bbabf0fb1fb40d463bd937685b1a1042e646979086c546d55319c3c
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-block-scoped-functions@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-block-scoped-functions@npm:7.22.5"
+"@babel/plugin-transform-block-scoped-functions@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-block-scoped-functions@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 416b1341858e8ca4e524dee66044735956ced5f478b2c3b9bc11ec2285b0c25d7dbb96d79887169eb938084c95d0a89338c8b2fe70d473bd9dc92e5d9db1732c
+  checksum: e63b16d94ee5f4d917e669da3db5ea53d1e7e79141a2ec873c1e644678cdafe98daa556d0d359963c827863d6b3665d23d4938a94a4c5053a1619c4ebd01d020
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-block-scoping@npm:^7.23.0":
-  version: 7.23.0
-  resolution: "@babel/plugin-transform-block-scoping@npm:7.23.0"
+"@babel/plugin-transform-block-scoping@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/plugin-transform-block-scoping@npm:7.23.4"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 0cfe925cc3b5a3ad407e2253fab3ceeaa117a4b291c9cb245578880872999bca91bd83ffa0128ae9ca356330702e1ef1dcb26804f28d2cef678239caf629f73e
+  checksum: fc4b2100dd9f2c47d694b4b35ae8153214ccb4e24ef545c259a9db17211b18b6a430f22799b56db8f6844deaeaa201af45a03331d0c80cc28b0c4e3c814570e4
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-class-properties@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-class-properties@npm:7.22.5"
+"@babel/plugin-transform-class-properties@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-class-properties@npm:7.23.3"
   dependencies:
-    "@babel/helper-create-class-features-plugin": ^7.22.5
+    "@babel/helper-create-class-features-plugin": ^7.22.15
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: b830152dfc2ff2f647f0abe76e6251babdfbef54d18c4b2c73a6bf76b1a00050a5d998dac80dc901a48514e95604324943a9dd39317073fe0928b559e0e0c579
+  checksum: 9c6f8366f667897541d360246de176dd29efc7a13d80a5b48361882f7173d9173be4646c3b7d9b003ccc0e01e25df122330308f33db921fa553aa17ad544b3fc
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-class-static-block@npm:^7.22.11":
-  version: 7.22.11
-  resolution: "@babel/plugin-transform-class-static-block@npm:7.22.11"
+"@babel/plugin-transform-class-static-block@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/plugin-transform-class-static-block@npm:7.23.4"
   dependencies:
-    "@babel/helper-create-class-features-plugin": ^7.22.11
+    "@babel/helper-create-class-features-plugin": ^7.22.15
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/plugin-syntax-class-static-block": ^7.14.5
   peerDependencies:
     "@babel/core": ^7.12.0
-  checksum: 69f040506fad66f1c6918d288d0e0edbc5c8a07c8b4462c1184ad2f9f08995d68b057126c213871c0853ae0c72afc60ec87492049dfacb20902e32346a448bcb
+  checksum: c8bfaba19a674fc2eb54edad71e958647360474e3163e8226f1acd63e4e2dbec32a171a0af596c1dc5359aee402cc120fea7abd1fb0e0354b6527f0fc9e8aa1e
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-classes@npm:^7.22.15":
-  version: 7.22.15
-  resolution: "@babel/plugin-transform-classes@npm:7.22.15"
+"@babel/plugin-transform-classes@npm:^7.23.8":
+  version: 7.23.8
+  resolution: "@babel/plugin-transform-classes@npm:7.23.8"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
-    "@babel/helper-compilation-targets": ^7.22.15
-    "@babel/helper-environment-visitor": ^7.22.5
-    "@babel/helper-function-name": ^7.22.5
-    "@babel/helper-optimise-call-expression": ^7.22.5
+    "@babel/helper-compilation-targets": ^7.23.6
+    "@babel/helper-environment-visitor": ^7.22.20
+    "@babel/helper-function-name": ^7.23.0
     "@babel/helper-plugin-utils": ^7.22.5
-    "@babel/helper-replace-supers": ^7.22.9
+    "@babel/helper-replace-supers": ^7.22.20
     "@babel/helper-split-export-declaration": ^7.22.6
     globals: ^11.1.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: d3f4d0c107dd8a3557ea3575cc777fab27efa92958b41e4a9822f7499725c1f554beae58855de16ddec0a7b694e45f59a26cea8fbde4275563f72f09c6e039a0
+  checksum: 7dee6cebe52131d2d16944f36e1fdb9d4b24f44d0e7e450f93a44435d001f17cc0789a4cb6b15ec67c8e484581b8a730b5c3ec374470f29ff0133086955b8c58
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-computed-properties@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-computed-properties@npm:7.22.5"
+"@babel/plugin-transform-computed-properties@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-computed-properties@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
-    "@babel/template": ^7.22.5
+    "@babel/template": ^7.22.15
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: c2a77a0f94ec71efbc569109ec14ea2aa925b333289272ced8b33c6108bdbb02caf01830ffc7e49486b62dec51911924d13f3a76f1149f40daace1898009e131
+  checksum: 80452661dc25a0956f89fe98cb562e8637a9556fb6c00d312c57653ce7df8798f58d138603c7e1aad96614ee9ccd10c47e50ab9ded6b6eded5adeb230d2a982e
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-destructuring@npm:^7.23.0":
-  version: 7.23.0
-  resolution: "@babel/plugin-transform-destructuring@npm:7.23.0"
+"@babel/plugin-transform-destructuring@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-destructuring@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: cd6dd454ccc2766be551e4f8a04b1acc2aa539fa19e5c7501c56cc2f8cc921dd41a7ffb78455b4c4b2f954fcab8ca4561ba7c9c7bd5af9f19465243603d18cc3
+  checksum: 9e015099877272501162419bfe781689aec5c462cd2aec752ee22288f209eec65969ff11b8fdadca2eaddea71d705d3bba5b9c60752fcc1be67874fcec687105
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-dotall-regex@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-dotall-regex@npm:7.22.5"
+"@babel/plugin-transform-dotall-regex@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-dotall-regex@npm:7.23.3"
   dependencies:
-    "@babel/helper-create-regexp-features-plugin": ^7.22.5
+    "@babel/helper-create-regexp-features-plugin": ^7.22.15
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 409b658d11e3082c8f69e9cdef2d96e4d6d11256f005772425fb230cc48fd05945edbfbcb709dab293a1a2f01f9c8a5bb7b4131e632b23264039d9f95864b453
+  checksum: a2dbbf7f1ea16a97948c37df925cb364337668c41a3948b8d91453f140507bd8a3429030c7ce66d09c299987b27746c19a2dd18b6f17dcb474854b14fd9159a3
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-duplicate-keys@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-duplicate-keys@npm:7.22.5"
+"@babel/plugin-transform-duplicate-keys@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-duplicate-keys@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: bb1280fbabaab6fab2ede585df34900712698210a3bd413f4df5bae6d8c24be36b496c92722ae676a7a67d060a4624f4d6c23b923485f906bfba8773c69f55b4
+  checksum: c2a21c34dc0839590cd945192cbc46fde541a27e140c48fe1808315934664cdbf18db64889e23c4eeb6bad9d3e049482efdca91d29de5734ffc887c4fbabaa16
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-dynamic-import@npm:^7.22.11":
-  version: 7.22.11
-  resolution: "@babel/plugin-transform-dynamic-import@npm:7.22.11"
+"@babel/plugin-transform-dynamic-import@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/plugin-transform-dynamic-import@npm:7.23.4"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/plugin-syntax-dynamic-import": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 78fc9c532210bf9e8f231747f542318568ac360ee6c27e80853962c984283c73da3f8f8aebe83c2096090a435b356b092ed85de617a156cbe0729d847632be45
+  checksum: 57a722604c430d9f3dacff22001a5f31250e34785d4969527a2ae9160fa86858d0892c5b9ff7a06a04076f8c76c9e6862e0541aadca9c057849961343aab0845
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-exponentiation-operator@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-exponentiation-operator@npm:7.22.5"
+"@babel/plugin-transform-exponentiation-operator@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-exponentiation-operator@npm:7.23.3"
   dependencies:
-    "@babel/helper-builder-binary-assignment-operator-visitor": ^7.22.5
+    "@babel/helper-builder-binary-assignment-operator-visitor": ^7.22.15
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: f2d660c1b1d51ad5fec1cd5ad426a52187204068c4158f8c4aa977b31535c61b66898d532603eef21c15756827be8277f724c869b888d560f26d7fe848bb5eae
+  checksum: 00d05ab14ad0f299160fcf9d8f55a1cc1b740e012ab0b5ce30207d2365f091665115557af7d989cd6260d075a252d9e4283de5f2b247dfbbe0e42ae586e6bf66
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-export-namespace-from@npm:^7.22.11":
-  version: 7.22.11
-  resolution: "@babel/plugin-transform-export-namespace-from@npm:7.22.11"
+"@babel/plugin-transform-export-namespace-from@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/plugin-transform-export-namespace-from@npm:7.23.4"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/plugin-syntax-export-namespace-from": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 73af5883a321ed56a4bfd43c8a7de0164faebe619287706896fc6ee2f7a4e69042adaa1338c0b8b4bdb9f7e5fdceb016fb1d40694cb43ca3b8827429e8aac4bf
+  checksum: 9f770a81bfd03b48d6ba155d452946fd56d6ffe5b7d871e9ec2a0b15e0f424273b632f3ed61838b90015b25bbda988896b7a46c7d964fbf8f6feb5820b309f93
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-for-of@npm:^7.22.15":
-  version: 7.22.15
-  resolution: "@babel/plugin-transform-for-of@npm:7.22.15"
+"@babel/plugin-transform-for-of@npm:^7.23.6":
+  version: 7.23.6
+  resolution: "@babel/plugin-transform-for-of@npm:7.23.6"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: f395ae7bce31e14961460f56cf751b5d6e37dd27d7df5b1f4e49fec1c11b6f9cf71991c7ffbe6549878591e87df0d66af798cf26edfa4bfa6b4c3dba1fb2f73a
+  checksum: 228c060aa61f6aa89dc447170075f8214863b94f830624e74ade99c1a09316897c12d76e848460b0b506593e58dbc42739af6dc4cb0fe9b84dffe4a596050a36
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-function-name@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-function-name@npm:7.22.5"
+"@babel/plugin-transform-function-name@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-function-name@npm:7.23.3"
   dependencies:
-    "@babel/helper-compilation-targets": ^7.22.5
-    "@babel/helper-function-name": ^7.22.5
+    "@babel/helper-compilation-targets": ^7.22.15
+    "@babel/helper-function-name": ^7.23.0
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: cff3b876357999cb8ae30e439c3ec6b0491a53b0aa6f722920a4675a6dd5b53af97a833051df4b34791fe5b3dd326ccf769d5c8e45b322aa50ee11a660b17845
+  checksum: 355c6dbe07c919575ad42b2f7e020f320866d72f8b79181a16f8e0cd424a2c761d979f03f47d583d9471b55dcd68a8a9d829b58e1eebcd572145b934b48975a6
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-json-strings@npm:^7.22.11":
-  version: 7.22.11
-  resolution: "@babel/plugin-transform-json-strings@npm:7.22.11"
+"@babel/plugin-transform-json-strings@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/plugin-transform-json-strings@npm:7.23.4"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/plugin-syntax-json-strings": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 50665e5979e66358c50e90a26db53c55917f78175127ac2fa05c7888d156d418ffb930ec0a109353db0a7c5f57c756ce01bfc9825d24cbfd2b3ec453f2ed8cba
+  checksum: f9019820233cf8955d8ba346df709a0683c120fe86a24ed1c9f003f2db51197b979efc88f010d558a12e1491210fc195a43cd1c7fee5e23b92da38f793a875de
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-literals@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-literals@npm:7.22.5"
+"@babel/plugin-transform-literals@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-literals@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: ec37cc2ffb32667af935ab32fe28f00920ec8a1eb999aa6dc6602f2bebd8ba205a558aeedcdccdebf334381d5c57106c61f52332045730393e73410892a9735b
+  checksum: 519a544cd58586b9001c4c9b18da25a62f17d23c48600ff7a685d75ca9eb18d2c5e8f5476f067f0a8f1fea2a31107eff950b9864833061e6076dcc4bdc3e71ed
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-logical-assignment-operators@npm:^7.22.11":
-  version: 7.22.11
-  resolution: "@babel/plugin-transform-logical-assignment-operators@npm:7.22.11"
+"@babel/plugin-transform-logical-assignment-operators@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/plugin-transform-logical-assignment-operators@npm:7.23.4"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/plugin-syntax-logical-assignment-operators": ^7.10.4
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: c664e9798e85afa7f92f07b867682dee7392046181d82f5d21bae6f2ca26dfe9c8375cdc52b7483c3fc09a983c1989f60eff9fbc4f373b0c0a74090553d05739
+  checksum: 2ae1dc9b4ff3bf61a990ff3accdecb2afe3a0ca649b3e74c010078d1cdf29ea490f50ac0a905306a2bcf9ac177889a39ac79bdcc3a0fdf220b3b75fac18d39b5
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-member-expression-literals@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-member-expression-literals@npm:7.22.5"
+"@babel/plugin-transform-member-expression-literals@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-member-expression-literals@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: ec4b0e07915ddd4fda0142fd104ee61015c208608a84cfa13643a95d18760b1dc1ceb6c6e0548898b8c49e5959a994e46367260176dbabc4467f729b21868504
+  checksum: 95cec13c36d447c5aa6b8e4c778b897eeba66dcb675edef01e0d2afcec9e8cb9726baf4f81b4bbae7a782595aed72e6a0d44ffb773272c3ca180fada99bf92db
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-modules-amd@npm:^7.23.0":
-  version: 7.23.0
-  resolution: "@babel/plugin-transform-modules-amd@npm:7.23.0"
+"@babel/plugin-transform-modules-amd@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-modules-amd@npm:7.23.3"
   dependencies:
-    "@babel/helper-module-transforms": ^7.23.0
+    "@babel/helper-module-transforms": ^7.23.3
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 5d92875170a37b8282d4bcd805f55829b8fab0f9c8d08b53d32a7a0bfdc62b868e489b52d329ae768ecafc0c993eed0ad7a387baa673ac33211390a9f833ab5d
+  checksum: d163737b6a3d67ea579c9aa3b83d4df4b5c34d9dcdf25f415f027c0aa8cded7bac2750d2de5464081f67a042ad9e1c03930c2fab42acd79f9e57c00cf969ddff
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-modules-commonjs@npm:^7.23.0":
-  version: 7.23.0
-  resolution: "@babel/plugin-transform-modules-commonjs@npm:7.23.0"
+"@babel/plugin-transform-modules-commonjs@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-modules-commonjs@npm:7.23.3"
   dependencies:
-    "@babel/helper-module-transforms": ^7.23.0
+    "@babel/helper-module-transforms": ^7.23.3
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/helper-simple-access": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 7fb25997194053e167c4207c319ff05362392da841bd9f42ddb3caf9c8798a5d203bd926d23ddf5830fdf05eddc82c2810f40d1287e3a4f80b07eff13d1024b5
+  checksum: 720a231ceade4ae4d2632478db4e7fecf21987d444942b72d523487ac8d715ca97de6c8f415c71e939595e1a4776403e7dc24ed68fe9125ad4acf57753c9bff7
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-modules-systemjs@npm:^7.23.0":
-  version: 7.23.0
-  resolution: "@babel/plugin-transform-modules-systemjs@npm:7.23.0"
+"@babel/plugin-transform-modules-systemjs@npm:^7.23.9":
+  version: 7.23.9
+  resolution: "@babel/plugin-transform-modules-systemjs@npm:7.23.9"
   dependencies:
     "@babel/helper-hoist-variables": ^7.22.5
-    "@babel/helper-module-transforms": ^7.23.0
+    "@babel/helper-module-transforms": ^7.23.3
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/helper-validator-identifier": ^7.22.20
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 2d481458b22605046badea2317d5cc5c94ac3031c2293e34c96f02063f5b02af0979c4da6a8fbc67cc249541575dc9c6d710db6b919ede70b7337a22d9fd57a7
+  checksum: cec6abeae6be66fd1a5940c482fe9ff94b689c71fcf4147e179119e4accd09d17d476e36528bc9cb4ab0ec6728fedf48b1c49d0551ea707fb192575d8eac9167
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-modules-umd@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-modules-umd@npm:7.22.5"
+"@babel/plugin-transform-modules-umd@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-modules-umd@npm:7.23.3"
   dependencies:
-    "@babel/helper-module-transforms": ^7.22.5
+    "@babel/helper-module-transforms": ^7.23.3
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 46622834c54c551b231963b867adbc80854881b3e516ff29984a8da989bd81665bd70e8cba6710345248e97166689310f544aee1a5773e262845a8f1b3e5b8b4
+  checksum: 586a7a2241e8b4e753a37af9466a9ffa8a67b4ba9aa756ad7500712c05d8fa9a8c1ed4f7bd25fae2a8265e6cf8fe781ec85a8ee885dd34cf50d8955ee65f12dc
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-named-capturing-groups-regex@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/plugin-transform-named-capturing-groups-regex@npm:7.22.5"
   dependencies:
@@ -923,362 +935,362 @@
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: 3ee564ddee620c035b928fdc942c5d17e9c4b98329b76f9cefac65c111135d925eb94ed324064cd7556d4f5123beec79abea1d4b97d1c8a2a5c748887a2eb623
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-new-target@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-new-target@npm:7.22.5"
+"@babel/plugin-transform-new-target@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-new-target@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 6b72112773487a881a1d6ffa680afde08bad699252020e86122180ee7a88854d5da3f15d9bca3331cf2e025df045604494a8208a2e63b486266b07c14e2ffbf3
+  checksum: e5053389316fce73ad5201b7777437164f333e24787fbcda4ae489cd2580dbbbdfb5694a7237bad91fabb46b591d771975d69beb1c740b82cb4761625379f00b
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-nullish-coalescing-operator@npm:^7.22.11":
-  version: 7.22.11
-  resolution: "@babel/plugin-transform-nullish-coalescing-operator@npm:7.22.11"
+"@babel/plugin-transform-nullish-coalescing-operator@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/plugin-transform-nullish-coalescing-operator@npm:7.23.4"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/plugin-syntax-nullish-coalescing-operator": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 167babecc8b8fe70796a7b7d34af667ebbf43da166c21689502e5e8cc93180b7a85979c77c9f64b7cce431b36718bd0a6df9e5e0ffea4ae22afb22cfef886372
+  checksum: a27d73ea134d3d9560a6b2e26ab60012fba15f1db95865aa0153c18f5ec82cfef6a7b3d8df74e3c2fca81534fa5efeb6cacaf7b08bdb7d123e3dafdd079886a3
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-numeric-separator@npm:^7.22.11":
-  version: 7.22.11
-  resolution: "@babel/plugin-transform-numeric-separator@npm:7.22.11"
+"@babel/plugin-transform-numeric-separator@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/plugin-transform-numeric-separator@npm:7.23.4"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/plugin-syntax-numeric-separator": ^7.10.4
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: af064d06a4a041767ec396a5f258103f64785df290e038bba9f0ef454e6c914f2ac45d862bbdad8fac2c7ad47fa4e95356f29053c60c100a0160b02a995fe2a3
+  checksum: 6ba0e5db3c620a3ec81f9e94507c821f483c15f196868df13fa454cbac719a5449baf73840f5b6eb7d77311b24a2cf8e45db53700d41727f693d46f7caf3eec3
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-object-rest-spread@npm:^7.22.15":
-  version: 7.22.15
-  resolution: "@babel/plugin-transform-object-rest-spread@npm:7.22.15"
+"@babel/plugin-transform-object-rest-spread@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/plugin-transform-object-rest-spread@npm:7.23.4"
   dependencies:
-    "@babel/compat-data": ^7.22.9
+    "@babel/compat-data": ^7.23.3
     "@babel/helper-compilation-targets": ^7.22.15
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/plugin-syntax-object-rest-spread": ^7.8.3
-    "@babel/plugin-transform-parameters": ^7.22.15
+    "@babel/plugin-transform-parameters": ^7.23.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 62197a6f12289c1c1bd57f3bed9f0f765ca32390bfe91e0b5561dd94dd9770f4480c4162dec98da094bc0ba99d2c2ebba68de47c019454041b0b7a68ba2ec66d
+  checksum: 73fec495e327ca3959c1c03d07a621be09df00036c69fff0455af9a008291677ee9d368eec48adacdc6feac703269a649747568b4af4c4e9f134aa71cc5b378d
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-object-super@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-object-super@npm:7.22.5"
+"@babel/plugin-transform-object-super@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-object-super@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
-    "@babel/helper-replace-supers": ^7.22.5
+    "@babel/helper-replace-supers": ^7.22.20
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: b71887877d74cb64dbccb5c0324fa67e31171e6a5311991f626650e44a4083e5436a1eaa89da78c0474fb095d4ec322d63ee778b202d33aa2e4194e1ed8e62d7
+  checksum: e495497186f621fa79026e183b4f1fbb172fd9df812cbd2d7f02c05b08adbe58012b1a6eb6dd58d11a30343f6ec80d0f4074f9b501d70aa1c94df76d59164c53
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-optional-catch-binding@npm:^7.22.11":
-  version: 7.22.11
-  resolution: "@babel/plugin-transform-optional-catch-binding@npm:7.22.11"
+"@babel/plugin-transform-optional-catch-binding@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/plugin-transform-optional-catch-binding@npm:7.23.4"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/plugin-syntax-optional-catch-binding": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: f17abd90e1de67c84d63afea29c8021c74abb2794d3a6eeafb0bbe7372d3db32aefca386e392116ec63884537a4a2815d090d26264d259bacc08f6e3ed05294c
+  checksum: d50b5ee142cdb088d8b5de1ccf7cea85b18b85d85b52f86618f6e45226372f01ad4cdb29abd4fd35ea99a71fefb37009e0107db7a787dcc21d4d402f97470faf
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-optional-chaining@npm:^7.22.15, @babel/plugin-transform-optional-chaining@npm:^7.23.0":
-  version: 7.23.0
-  resolution: "@babel/plugin-transform-optional-chaining@npm:7.23.0"
+"@babel/plugin-transform-optional-chaining@npm:^7.23.3, @babel/plugin-transform-optional-chaining@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/plugin-transform-optional-chaining@npm:7.23.4"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
     "@babel/plugin-syntax-optional-chaining": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: f702634f2b97e5260dbec0d4bde05ccb6f4d96d7bfa946481aeacfa205ca846cb6e096a38312f9d51fdbdac1f258f211138c5f7075952e46a5bf8574de6a1329
+  checksum: e7a4c08038288057b7a08d68c4d55396ada9278095509ca51ed8dfb72a7f13f26bdd7c5185de21079fe0a9d60d22c227cb32e300d266c1bda40f70eee9f4bc1e
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-parameters@npm:^7.22.15":
-  version: 7.22.15
-  resolution: "@babel/plugin-transform-parameters@npm:7.22.15"
+"@babel/plugin-transform-parameters@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-parameters@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 541188bb7d1876cad87687b5c7daf90f63d8208ae83df24acb1e2b05020ad1c78786b2723ca4054a83fcb74fb6509f30c4cacc5b538ee684224261ad5fb047c1
+  checksum: a735b3e85316d17ec102e3d3d1b6993b429bdb3b494651c9d754e3b7d270462ee1f1a126ccd5e3d871af5e683727e9ef98c9d34d4a42204fffaabff91052ed16
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-private-methods@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-private-methods@npm:7.22.5"
+"@babel/plugin-transform-private-methods@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-private-methods@npm:7.23.3"
   dependencies:
-    "@babel/helper-create-class-features-plugin": ^7.22.5
+    "@babel/helper-create-class-features-plugin": ^7.22.15
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 321479b4fcb6d3b3ef622ab22fd24001e43d46e680e8e41324c033d5810c84646e470f81b44cbcbef5c22e99030784f7cac92f1829974da7a47a60a7139082c3
+  checksum: cedc1285c49b5a6d9a3d0e5e413b756ac40b3ac2f8f68bdfc3ae268bc8d27b00abd8bb0861c72756ff5dd8bf1eb77211b7feb5baf4fdae2ebbaabe49b9adc1d0
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-private-property-in-object@npm:^7.22.11":
-  version: 7.22.11
-  resolution: "@babel/plugin-transform-private-property-in-object@npm:7.22.11"
+"@babel/plugin-transform-private-property-in-object@npm:^7.23.4":
+  version: 7.23.4
+  resolution: "@babel/plugin-transform-private-property-in-object@npm:7.23.4"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
-    "@babel/helper-create-class-features-plugin": ^7.22.11
+    "@babel/helper-create-class-features-plugin": ^7.22.15
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/plugin-syntax-private-property-in-object": ^7.14.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 4d029d84901e53c46dead7a46e2990a7bc62470f4e4ca58a0d063394f86652fd58fe4eea1eb941da3669cd536b559b9d058b342b59300026346b7a2a51badac8
+  checksum: fb7adfe94ea97542f250a70de32bddbc3e0b802381c92be947fec83ebffda57e68533c4d0697152719a3496fdd3ebf3798d451c024cd4ac848fc15ac26b70aa7
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-property-literals@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-property-literals@npm:7.22.5"
+"@babel/plugin-transform-property-literals@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-property-literals@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 796176a3176106f77fcb8cd04eb34a8475ce82d6d03a88db089531b8f0453a2fb8b0c6ec9a52c27948bc0ea478becec449893741fc546dfc3930ab927e3f9f2e
+  checksum: 16b048c8e87f25095f6d53634ab7912992f78e6997a6ff549edc3cf519db4fca01c7b4e0798530d7f6a05228ceee479251245cdd850a5531c6e6f404104d6cc9
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-regenerator@npm:^7.22.10":
-  version: 7.22.10
-  resolution: "@babel/plugin-transform-regenerator@npm:7.22.10"
+"@babel/plugin-transform-regenerator@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-regenerator@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
     regenerator-transform: ^0.15.2
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: e13678d62d6fa96f11cb8b863f00e8693491e7adc88bfca3f2820f80cbac8336e7dec3a596eee6a1c4663b7ececc3564f2cd7fb44ed6d4ce84ac2bb7f39ecc6e
+  checksum: 7fdacc7b40008883871b519c9e5cdea493f75495118ccc56ac104b874983569a24edd024f0f5894ba1875c54ee2b442f295d6241c3280e61c725d0dd3317c8e6
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-reserved-words@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-reserved-words@npm:7.22.5"
+"@babel/plugin-transform-reserved-words@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-reserved-words@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 3ffd7dbc425fe8132bfec118b9817572799cab1473113a635d25ab606c1f5a2341a636c04cf6b22df3813320365ed5a965b5eeb3192320a10e4cc2c137bd8bfc
+  checksum: 298c4440ddc136784ff920127cea137168e068404e635dc946ddb5d7b2a27b66f1dd4c4acb01f7184478ff7d5c3e7177a127279479926519042948fb7fa0fa48
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-shorthand-properties@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-shorthand-properties@npm:7.22.5"
+"@babel/plugin-transform-shorthand-properties@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-shorthand-properties@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: a5ac902c56ea8effa99f681340ee61bac21094588f7aef0bc01dff98246651702e677552fa6d10e548c4ac22a3ffad047dd2f8c8f0540b68316c2c203e56818b
+  checksum: 5d677a03676f9fff969b0246c423d64d77502e90a832665dc872a5a5e05e5708161ce1effd56bb3c0f2c20a1112fca874be57c8a759d8b08152755519281f326
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-spread@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-spread@npm:7.22.5"
+"@babel/plugin-transform-spread@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-spread@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 5587f0deb60b3dfc9b274e269031cc45ec75facccf1933ea2ea71ced9fd3ce98ed91bb36d6cd26817c14474b90ed998c5078415f0eab531caf301496ce24c95c
+  checksum: 8fd5cac201e77a0b4825745f4e07a25f923842f282f006b3a79223c00f61075c8868d12eafec86b2642cd0b32077cdd32314e27bcb75ee5e6a68c0144140dcf2
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-sticky-regex@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-sticky-regex@npm:7.22.5"
+"@babel/plugin-transform-sticky-regex@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-sticky-regex@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 63b2c575e3e7f96c32d52ed45ee098fb7d354b35c2223b8c8e76840b32cc529ee0c0ceb5742fd082e56e91e3d82842a367ce177e82b05039af3d602c9627a729
+  checksum: 53e55eb2575b7abfdb4af7e503a2bf7ef5faf8bf6b92d2cd2de0700bdd19e934e5517b23e6dfed94ba50ae516b62f3f916773ef7d9bc81f01503f585051e2949
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-template-literals@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-template-literals@npm:7.22.5"
+"@babel/plugin-transform-template-literals@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-template-literals@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 27e9bb030654cb425381c69754be4abe6a7c75b45cd7f962cd8d604b841b2f0fb7b024f2efc1c25cc53f5b16d79d5e8cfc47cacbdaa983895b3aeefa3e7e24ff
+  checksum: b16c5cb0b8796be0118e9c144d15bdc0d20a7f3f59009c6303a6e9a8b74c146eceb3f05186f5b97afcba7cfa87e34c1585a22186e3d5b22f2fd3d27d959d92b2
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-typeof-symbol@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-typeof-symbol@npm:7.22.5"
+"@babel/plugin-transform-typeof-symbol@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-typeof-symbol@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 82a53a63ffc3010b689ca9a54e5f53b2718b9f4b4a9818f36f9b7dba234f38a01876680553d2716a645a61920b5e6e4aaf8d4a0064add379b27ca0b403049512
+  checksum: 0af7184379d43afac7614fc89b1bdecce4e174d52f4efaeee8ec1a4f2c764356c6dba3525c0685231f1cbf435b6dd4ee9e738d7417f3b10ce8bbe869c32f4384
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-unicode-escapes@npm:^7.22.10":
-  version: 7.22.10
-  resolution: "@babel/plugin-transform-unicode-escapes@npm:7.22.10"
+"@babel/plugin-transform-unicode-escapes@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-unicode-escapes@npm:7.23.3"
   dependencies:
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 807f40ed1324c8cb107c45358f1903384ca3f0ef1d01c5a3c5c9b271c8d8eec66936a3dcc8d75ddfceea9421420368c2e77ae3adef0a50557e778dfe296bf382
+  checksum: 561c429183a54b9e4751519a3dfba6014431e9cdc1484fad03bdaf96582dfc72c76a4f8661df2aeeae7c34efd0fa4d02d3b83a2f63763ecf71ecc925f9cc1f60
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-unicode-property-regex@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-unicode-property-regex@npm:7.22.5"
+"@babel/plugin-transform-unicode-property-regex@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-unicode-property-regex@npm:7.23.3"
   dependencies:
-    "@babel/helper-create-regexp-features-plugin": ^7.22.5
+    "@babel/helper-create-regexp-features-plugin": ^7.22.15
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 2495e5f663cb388e3d888b4ba3df419ac436a5012144ac170b622ddfc221f9ea9bdba839fa2bc0185cb776b578030666406452ec7791cbf0e7a3d4c88ae9574c
+  checksum: 2298461a194758086d17c23c26c7de37aa533af910f9ebf31ebd0893d4aa317468043d23f73edc782ec21151d3c46cf0ff8098a83b725c49a59de28a1d4d6225
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-unicode-regex@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-unicode-regex@npm:7.22.5"
+"@babel/plugin-transform-unicode-regex@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-unicode-regex@npm:7.23.3"
   dependencies:
-    "@babel/helper-create-regexp-features-plugin": ^7.22.5
+    "@babel/helper-create-regexp-features-plugin": ^7.22.15
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 6b5d1404c8c623b0ec9bd436c00d885a17d6a34f3f2597996343ddb9d94f6379705b21582dfd4cec2c47fd34068872e74ab6b9580116c0566b3f9447e2a7fa06
+  checksum: c5f835d17483ba899787f92e313dfa5b0055e3deab332f1d254078a2bba27ede47574b6599fcf34d3763f0c048ae0779dc21d2d8db09295edb4057478dc80a9a
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-unicode-sets-regex@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/plugin-transform-unicode-sets-regex@npm:7.22.5"
+"@babel/plugin-transform-unicode-sets-regex@npm:^7.23.3":
+  version: 7.23.3
+  resolution: "@babel/plugin-transform-unicode-sets-regex@npm:7.23.3"
   dependencies:
-    "@babel/helper-create-regexp-features-plugin": ^7.22.5
+    "@babel/helper-create-regexp-features-plugin": ^7.22.15
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: c042070f980b139547f8b0179efbc049ac5930abec7fc26ed7a41d89a048d8ab17d362200e204b6f71c3c20d6991a0e74415e1a412a49adc8131c2a40c04822e
+  checksum: 79d0b4c951955ca68235c87b91ab2b393c96285f8aeaa34d6db416d2ddac90000c9bd6e8c4d82b60a2b484da69930507245035f28ba63c6cae341cf3ba68fdef
   languageName: node
   linkType: hard
 
 "@babel/preset-env@npm:^7.10.2":
-  version: 7.23.2
-  resolution: "@babel/preset-env@npm:7.23.2"
+  version: 7.23.9
+  resolution: "@babel/preset-env@npm:7.23.9"
   dependencies:
-    "@babel/compat-data": ^7.23.2
-    "@babel/helper-compilation-targets": ^7.22.15
+    "@babel/compat-data": ^7.23.5
+    "@babel/helper-compilation-targets": ^7.23.6
     "@babel/helper-plugin-utils": ^7.22.5
-    "@babel/helper-validator-option": ^7.22.15
-    "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression": ^7.22.15
-    "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining": ^7.22.15
+    "@babel/helper-validator-option": ^7.23.5
+    "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression": ^7.23.3
+    "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining": ^7.23.3
+    "@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly": ^7.23.7
     "@babel/plugin-proposal-private-property-in-object": 7.21.0-placeholder-for-preset-env.2
     "@babel/plugin-syntax-async-generators": ^7.8.4
     "@babel/plugin-syntax-class-properties": ^7.12.13
     "@babel/plugin-syntax-class-static-block": ^7.14.5
     "@babel/plugin-syntax-dynamic-import": ^7.8.3
     "@babel/plugin-syntax-export-namespace-from": ^7.8.3
-    "@babel/plugin-syntax-import-assertions": ^7.22.5
-    "@babel/plugin-syntax-import-attributes": ^7.22.5
+    "@babel/plugin-syntax-import-assertions": ^7.23.3
+    "@babel/plugin-syntax-import-attributes": ^7.23.3
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
-    "@babel/plugin-transform-arrow-functions": ^7.22.5
-    "@babel/plugin-transform-async-generator-functions": ^7.23.2
-    "@babel/plugin-transform-async-to-generator": ^7.22.5
-    "@babel/plugin-transform-block-scoped-functions": ^7.22.5
-    "@babel/plugin-transform-block-scoping": ^7.23.0
-    "@babel/plugin-transform-class-properties": ^7.22.5
-    "@babel/plugin-transform-class-static-block": ^7.22.11
-    "@babel/plugin-transform-classes": ^7.22.15
-    "@babel/plugin-transform-computed-properties": ^7.22.5
-    "@babel/plugin-transform-destructuring": ^7.23.0
-    "@babel/plugin-transform-dotall-regex": ^7.22.5
-    "@babel/plugin-transform-duplicate-keys": ^7.22.5
-    "@babel/plugin-transform-dynamic-import": ^7.22.11
-    "@babel/plugin-transform-exponentiation-operator": ^7.22.5
-    "@babel/plugin-transform-export-namespace-from": ^7.22.11
-    "@babel/plugin-transform-for-of": ^7.22.15
-    "@babel/plugin-transform-function-name": ^7.22.5
-    "@babel/plugin-transform-json-strings": ^7.22.11
-    "@babel/plugin-transform-literals": ^7.22.5
-    "@babel/plugin-transform-logical-assignment-operators": ^7.22.11
-    "@babel/plugin-transform-member-expression-literals": ^7.22.5
-    "@babel/plugin-transform-modules-amd": ^7.23.0
-    "@babel/plugin-transform-modules-commonjs": ^7.23.0
-    "@babel/plugin-transform-modules-systemjs": ^7.23.0
-    "@babel/plugin-transform-modules-umd": ^7.22.5
+    "@babel/plugin-transform-arrow-functions": ^7.23.3
+    "@babel/plugin-transform-async-generator-functions": ^7.23.9
+    "@babel/plugin-transform-async-to-generator": ^7.23.3
+    "@babel/plugin-transform-block-scoped-functions": ^7.23.3
+    "@babel/plugin-transform-block-scoping": ^7.23.4
+    "@babel/plugin-transform-class-properties": ^7.23.3
+    "@babel/plugin-transform-class-static-block": ^7.23.4
+    "@babel/plugin-transform-classes": ^7.23.8
+    "@babel/plugin-transform-computed-properties": ^7.23.3
+    "@babel/plugin-transform-destructuring": ^7.23.3
+    "@babel/plugin-transform-dotall-regex": ^7.23.3
+    "@babel/plugin-transform-duplicate-keys": ^7.23.3
+    "@babel/plugin-transform-dynamic-import": ^7.23.4
+    "@babel/plugin-transform-exponentiation-operator": ^7.23.3
+    "@babel/plugin-transform-export-namespace-from": ^7.23.4
+    "@babel/plugin-transform-for-of": ^7.23.6
+    "@babel/plugin-transform-function-name": ^7.23.3
+    "@babel/plugin-transform-json-strings": ^7.23.4
+    "@babel/plugin-transform-literals": ^7.23.3
+    "@babel/plugin-transform-logical-assignment-operators": ^7.23.4
+    "@babel/plugin-transform-member-expression-literals": ^7.23.3
+    "@babel/plugin-transform-modules-amd": ^7.23.3
+    "@babel/plugin-transform-modules-commonjs": ^7.23.3
+    "@babel/plugin-transform-modules-systemjs": ^7.23.9
+    "@babel/plugin-transform-modules-umd": ^7.23.3
     "@babel/plugin-transform-named-capturing-groups-regex": ^7.22.5
-    "@babel/plugin-transform-new-target": ^7.22.5
-    "@babel/plugin-transform-nullish-coalescing-operator": ^7.22.11
-    "@babel/plugin-transform-numeric-separator": ^7.22.11
-    "@babel/plugin-transform-object-rest-spread": ^7.22.15
-    "@babel/plugin-transform-object-super": ^7.22.5
-    "@babel/plugin-transform-optional-catch-binding": ^7.22.11
-    "@babel/plugin-transform-optional-chaining": ^7.23.0
-    "@babel/plugin-transform-parameters": ^7.22.15
-    "@babel/plugin-transform-private-methods": ^7.22.5
-    "@babel/plugin-transform-private-property-in-object": ^7.22.11
-    "@babel/plugin-transform-property-literals": ^7.22.5
-    "@babel/plugin-transform-regenerator": ^7.22.10
-    "@babel/plugin-transform-reserved-words": ^7.22.5
-    "@babel/plugin-transform-shorthand-properties": ^7.22.5
-    "@babel/plugin-transform-spread": ^7.22.5
-    "@babel/plugin-transform-sticky-regex": ^7.22.5
-    "@babel/plugin-transform-template-literals": ^7.22.5
-    "@babel/plugin-transform-typeof-symbol": ^7.22.5
-    "@babel/plugin-transform-unicode-escapes": ^7.22.10
-    "@babel/plugin-transform-unicode-property-regex": ^7.22.5
-    "@babel/plugin-transform-unicode-regex": ^7.22.5
-    "@babel/plugin-transform-unicode-sets-regex": ^7.22.5
+    "@babel/plugin-transform-new-target": ^7.23.3
+    "@babel/plugin-transform-nullish-coalescing-operator": ^7.23.4
+    "@babel/plugin-transform-numeric-separator": ^7.23.4
+    "@babel/plugin-transform-object-rest-spread": ^7.23.4
+    "@babel/plugin-transform-object-super": ^7.23.3
+    "@babel/plugin-transform-optional-catch-binding": ^7.23.4
+    "@babel/plugin-transform-optional-chaining": ^7.23.4
+    "@babel/plugin-transform-parameters": ^7.23.3
+    "@babel/plugin-transform-private-methods": ^7.23.3
+    "@babel/plugin-transform-private-property-in-object": ^7.23.4
+    "@babel/plugin-transform-property-literals": ^7.23.3
+    "@babel/plugin-transform-regenerator": ^7.23.3
+    "@babel/plugin-transform-reserved-words": ^7.23.3
+    "@babel/plugin-transform-shorthand-properties": ^7.23.3
+    "@babel/plugin-transform-spread": ^7.23.3
+    "@babel/plugin-transform-sticky-regex": ^7.23.3
+    "@babel/plugin-transform-template-literals": ^7.23.3
+    "@babel/plugin-transform-typeof-symbol": ^7.23.3
+    "@babel/plugin-transform-unicode-escapes": ^7.23.3
+    "@babel/plugin-transform-unicode-property-regex": ^7.23.3
+    "@babel/plugin-transform-unicode-regex": ^7.23.3
+    "@babel/plugin-transform-unicode-sets-regex": ^7.23.3
     "@babel/preset-modules": 0.1.6-no-external-plugins
-    "@babel/types": ^7.23.0
-    babel-plugin-polyfill-corejs2: ^0.4.6
-    babel-plugin-polyfill-corejs3: ^0.8.5
-    babel-plugin-polyfill-regenerator: ^0.5.3
+    babel-plugin-polyfill-corejs2: ^0.4.8
+    babel-plugin-polyfill-corejs3: ^0.9.0
+    babel-plugin-polyfill-regenerator: ^0.5.5
     core-js-compat: ^3.31.0
     semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 49327ef584b529b56aedd6577937b80c0d89603c68b23795495a13af04b5aa008db9ad04cd280423600cdc0d3cce13ae9d0d9a977db5c8193697b20ced8a10b2
+  checksum: 23a48468ba820c68ba34ea2c1dbc62fd2ff9cf858cfb69e159cabb0c85c72dc4c2266ce20ca84318d8742de050cb061e7c66902fbfddbcb09246afd248847933
   languageName: node
   linkType: hard
 
 "@babel/preset-modules@npm:0.1.6-no-external-plugins":
   version: 0.1.6-no-external-plugins
   resolution: "@babel/preset-modules@npm:0.1.6-no-external-plugins"
   dependencies:
@@ -1295,95 +1307,95 @@
   version: 0.8.0
   resolution: "@babel/regjsgen@npm:0.8.0"
   checksum: 89c338fee774770e5a487382170711014d49a68eb281e74f2b5eac88f38300a4ad545516a7786a8dd5702e9cf009c94c2f582d200f077ac5decd74c56b973730
   languageName: node
   linkType: hard
 
 "@babel/runtime@npm:^7.8.4":
-  version: 7.23.2
-  resolution: "@babel/runtime@npm:7.23.2"
+  version: 7.23.9
+  resolution: "@babel/runtime@npm:7.23.9"
   dependencies:
     regenerator-runtime: ^0.14.0
-  checksum: 6c4df4839ec75ca10175f636d6362f91df8a3137f86b38f6cd3a4c90668a0fe8e9281d320958f4fbd43b394988958585a17c3aab2a4ea6bf7316b22916a371fb
+  checksum: 6bbebe8d27c0c2dd275d1ac197fc1a6c00e18dab68cc7aaff0adc3195b45862bae9c4cc58975629004b0213955b2ed91e99eccb3d9b39cabea246c657323d667
   languageName: node
   linkType: hard
 
-"@babel/template@npm:^7.22.15, @babel/template@npm:^7.22.5, @babel/template@npm:^7.3.3":
-  version: 7.22.15
-  resolution: "@babel/template@npm:7.22.15"
+"@babel/template@npm:^7.22.15, @babel/template@npm:^7.23.9, @babel/template@npm:^7.3.3":
+  version: 7.23.9
+  resolution: "@babel/template@npm:7.23.9"
   dependencies:
-    "@babel/code-frame": ^7.22.13
-    "@babel/parser": ^7.22.15
-    "@babel/types": ^7.22.15
-  checksum: 1f3e7dcd6c44f5904c184b3f7fe280394b191f2fed819919ffa1e529c259d5b197da8981b6ca491c235aee8dbad4a50b7e31304aa531271cb823a4a24a0dd8fd
+    "@babel/code-frame": ^7.23.5
+    "@babel/parser": ^7.23.9
+    "@babel/types": ^7.23.9
+  checksum: 6e67414c0f7125d7ecaf20c11fab88085fa98a96c3ef10da0a61e962e04fdf3a18a496a66047005ddd1bb682a7cc7842d556d1db2f3f3f6ccfca97d5e445d342
   languageName: node
   linkType: hard
 
-"@babel/traverse@npm:^7.23.2":
-  version: 7.23.2
-  resolution: "@babel/traverse@npm:7.23.2"
+"@babel/traverse@npm:^7.23.9":
+  version: 7.23.9
+  resolution: "@babel/traverse@npm:7.23.9"
   dependencies:
-    "@babel/code-frame": ^7.22.13
-    "@babel/generator": ^7.23.0
+    "@babel/code-frame": ^7.23.5
+    "@babel/generator": ^7.23.6
     "@babel/helper-environment-visitor": ^7.22.20
     "@babel/helper-function-name": ^7.23.0
     "@babel/helper-hoist-variables": ^7.22.5
     "@babel/helper-split-export-declaration": ^7.22.6
-    "@babel/parser": ^7.23.0
-    "@babel/types": ^7.23.0
-    debug: ^4.1.0
+    "@babel/parser": ^7.23.9
+    "@babel/types": ^7.23.9
+    debug: ^4.3.1
     globals: ^11.1.0
-  checksum: 26a1eea0dde41ab99dde8b9773a013a0dc50324e5110a049f5d634e721ff08afffd54940b3974a20308d7952085ac769689369e9127dea655f868c0f6e1ab35d
+  checksum: a932f7aa850e158c00c97aad22f639d48c72805c687290f6a73e30c5c4957c07f5d28310c9bf59648e2980fe6c9d16adeb2ff92a9ca0f97fa75739c1328fc6c3
   languageName: node
   linkType: hard
 
-"@babel/types@npm:^7.0.0, @babel/types@npm:^7.20.7, @babel/types@npm:^7.22.15, @babel/types@npm:^7.22.19, @babel/types@npm:^7.22.5, @babel/types@npm:^7.23.0, @babel/types@npm:^7.3.3, @babel/types@npm:^7.4.4, @babel/types@npm:^7.8.3":
-  version: 7.23.0
-  resolution: "@babel/types@npm:7.23.0"
+"@babel/types@npm:^7.0.0, @babel/types@npm:^7.20.7, @babel/types@npm:^7.22.15, @babel/types@npm:^7.22.19, @babel/types@npm:^7.22.5, @babel/types@npm:^7.23.0, @babel/types@npm:^7.23.6, @babel/types@npm:^7.23.9, @babel/types@npm:^7.3.3, @babel/types@npm:^7.4.4, @babel/types@npm:^7.8.3":
+  version: 7.23.9
+  resolution: "@babel/types@npm:7.23.9"
   dependencies:
-    "@babel/helper-string-parser": ^7.22.5
+    "@babel/helper-string-parser": ^7.23.4
     "@babel/helper-validator-identifier": ^7.22.20
     to-fast-properties: ^2.0.0
-  checksum: 215fe04bd7feef79eeb4d33374b39909ce9cad1611c4135a4f7fdf41fe3280594105af6d7094354751514625ea92d0875aba355f53e86a92600f290e77b0e604
+  checksum: 0a9b008e9bfc89beb8c185e620fa0f8ed6c771f1e1b2e01e1596870969096fec7793898a1d64a035176abf1dd13e2668ee30bf699f2d92c210a8128f4b151e65
   languageName: node
   linkType: hard
 
 "@bcoe/v8-coverage@npm:^0.2.3":
   version: 0.2.3
   resolution: "@bcoe/v8-coverage@npm:0.2.3"
   checksum: 850f9305536d0f2bd13e9e0881cb5f02e4f93fad1189f7b2d4bebf694e3206924eadee1068130d43c11b750efcc9405f88a8e42ef098b6d75239c0f047de1a27
   languageName: node
   linkType: hard
 
 "@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.5.1, @codemirror/autocomplete@npm:^6.7.1":
-  version: 6.10.2
-  resolution: "@codemirror/autocomplete@npm:6.10.2"
+  version: 6.12.0
+  resolution: "@codemirror/autocomplete@npm:6.12.0"
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
-  checksum: 360cea6a87ae9c4e3c996903f636a8f47f8ea6cd44504181e69dd8ccf666bad3e8cc6d8935e0eedd8aa118fdfe86ea78f41bc15288f3a7517dbb87115e057563
+  checksum: 1d4da6ccc12f5a67053a76b361f2683b5af031dd405a0bd2a261a265eb8cb7dfb115343a3291260d1ba31ce7ccb5427208ebe50f50f6747fcf27a50b62c87f7e
   languageName: node
   linkType: hard
 
 "@codemirror/commands@npm:^6.2.3":
-  version: 6.3.0
-  resolution: "@codemirror/commands@npm:6.3.0"
+  version: 6.3.3
+  resolution: "@codemirror/commands@npm:6.3.3"
   dependencies:
     "@codemirror/language": ^6.0.0
-    "@codemirror/state": ^6.2.0
+    "@codemirror/state": ^6.4.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.1.0
-  checksum: d6ade0ba7d4f80c2e44163935783d2f2f35c8b641a4b4f62452c0630211670abe5093786cf5a4af14147102d4284dae660a26f3ae58fd840e838685a81107d11
+  checksum: 7d23aecc973823969434b839aefa9a98bb47212d2ce0e6869ae903adbb5233aad22a760788fb7bb6eb45b00b01a4932fb93ad43bacdcbc0215e7500cf54b17bb
   languageName: node
   linkType: hard
 
 "@codemirror/lang-cpp@npm:^6.0.2":
   version: 6.0.2
   resolution: "@codemirror/lang-cpp@npm:6.0.2"
   dependencies:
@@ -1403,27 +1415,27 @@
     "@lezer/common": ^1.0.2
     "@lezer/css": ^1.0.0
   checksum: 5a8457ee8a4310030a969f2d3128429f549c4dc9b7907ee8888b42119c80b65af99093801432efdf659b8ec36a147d2a947bc1ecbbf69a759395214e3f4834a8
   languageName: node
   linkType: hard
 
 "@codemirror/lang-html@npm:^6.0.0, @codemirror/lang-html@npm:^6.4.3":
-  version: 6.4.6
-  resolution: "@codemirror/lang-html@npm:6.4.6"
+  version: 6.4.8
+  resolution: "@codemirror/lang-html@npm:6.4.8"
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
-  checksum: 8f884f4423ffc783181ee933f7212ad4ece204695cf8af9535a593f95e901d36515a8561fc336a0fbcf5782369b9484eeb0d2cec2167622868238177c5e6eb36
+  checksum: 9aec56c333cc06f9e4bb6d09806ae83e4a7f235a26b3244010e2dcea83a923cfcd7bec84904b8a59bc81256b0bb579a52bf5614962dad031d7577db1c49a216a
   languageName: node
   linkType: hard
 
 "@codemirror/lang-java@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-java@npm:6.0.1"
   dependencies:
@@ -1455,25 +1467,25 @@
     "@codemirror/language": ^6.0.0
     "@lezer/json": ^1.0.0
   checksum: e9e87d50ff7b81bd56a6ab50740b1dd54e9a93f1be585e1d59d0642e2148842ea1528ac7b7221eb4ddc7fe84bbc28065144cc3ab86f6e06c6aeb2d4b4e62acf1
   languageName: node
   linkType: hard
 
 "@codemirror/lang-markdown@npm:^6.1.1":
-  version: 6.2.2
-  resolution: "@codemirror/lang-markdown@npm:6.2.2"
+  version: 6.2.4
+  resolution: "@codemirror/lang-markdown@npm:6.2.4"
   dependencies:
     "@codemirror/autocomplete": ^6.7.1
     "@codemirror/lang-html": ^6.0.0
     "@codemirror/language": ^6.3.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
-    "@lezer/common": ^1.0.0
+    "@lezer/common": ^1.2.1
     "@lezer/markdown": ^1.0.0
-  checksum: 36aa82a4fc07e5761e0e04108b54f112f0049ed210b3d4e81b7429a99be4677a1f9ef0e004c5243265dca3bac36525792cb1558999f6a224c689475e958d4aa8
+  checksum: fbdf1388a9fd08b4e6fc9950ac57fc59ef02bb0bd3e76654158ce1494b101356ded049b65dcf6da457e7e302cb178bf30852fd152680f3a8679be3c3884c0bc2
   languageName: node
   linkType: hard
 
 "@codemirror/lang-php@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-php@npm:6.0.1"
   dependencies:
@@ -1504,34 +1516,36 @@
     "@codemirror/language": ^6.0.0
     "@lezer/rust": ^1.0.0
   checksum: 8a439944cb22159b0b3465ca4fa4294c69843219d5d30e278ae6df8e48f30a7a9256129723c025ec9b5e694d31a3560fb004300b125ffcd81c22d13825845170
   languageName: node
   linkType: hard
 
 "@codemirror/lang-sql@npm:^6.4.1":
-  version: 6.5.4
-  resolution: "@codemirror/lang-sql@npm:6.5.4"
+  version: 6.5.5
+  resolution: "@codemirror/lang-sql@npm:6.5.5"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: face21b0231ac5a7981949b5bf6a99ed092d0d6f7eb83f35dcd31d56ecf07dafa19d21623e0bad36cec7a12e3149df7b45c3588aeee31eae41e9b05942c4fdd7
+  checksum: 404003ae73b986bd7a00f6924db78b7ffb28fdc38d689fdc11416aaafe2d5c6dc37cc18972530f82e940acb61e18ac74a1cf7712beef448c145344ff93970dc3
   languageName: node
   linkType: hard
 
 "@codemirror/lang-wast@npm:^6.0.1":
-  version: 6.0.1
-  resolution: "@codemirror/lang-wast@npm:6.0.1"
+  version: 6.0.2
+  resolution: "@codemirror/lang-wast@npm:6.0.2"
   dependencies:
     "@codemirror/language": ^6.0.0
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 600d98d3ea6a4e99292244ed707e39a2abd9f3abf62cfeff5c819a0cc0c7e86b8c5b91e91c1b7ea21233d9ea09c41abe61d8a40b2547bb5db74239c6df857934
+  checksum: 72119d4a7d726c54167aa227c982ae9fa785c8ad97a158d8350ae95eecfbd8028a803eef939f7e6c5c6e626fcecda1dc37e9dffc6d5d6ec105f686aeda6b2c24
   languageName: node
   linkType: hard
 
 "@codemirror/lang-xml@npm:^6.0.2":
   version: 6.0.2
   resolution: "@codemirror/lang-xml@npm:6.0.2"
   dependencies:
@@ -1541,24 +1555,24 @@
     "@lezer/common": ^1.0.0
     "@lezer/xml": ^1.0.0
   checksum: e156ecafaa87e9b6ef4ab6812ccd00d8f3c6cb81f232837636b36336d80513b61936dfee6f4f6800574f236208b61e95a2abcb997cdcd7366585a6b796e0e13b
   languageName: node
   linkType: hard
 
 "@codemirror/language@npm:^6.0.0, @codemirror/language@npm:^6.3.0, @codemirror/language@npm:^6.4.0, @codemirror/language@npm:^6.6.0, @codemirror/language@npm:^6.8.0":
-  version: 6.9.2
-  resolution: "@codemirror/language@npm:6.9.2"
+  version: 6.10.0
+  resolution: "@codemirror/language@npm:6.10.0"
   dependencies:
     "@codemirror/state": ^6.0.0
-    "@codemirror/view": ^6.0.0
+    "@codemirror/view": ^6.23.0
     "@lezer/common": ^1.1.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
     style-mod: ^4.0.0
-  checksum: eee7b861b5591114cac7502cd532d5b923639740081a4cd7e28696c252af8d759b14686aaf6d5eee7e0969ff647b7aaf03a5eea7235fb6d9858ee19433f1c74d
+  checksum: 3bfd9968f5a34ce22434489a5b226db5f3bc454a1ae7c4381587ff4270ac6af61b10f93df560cb73e9a77cc13d4843722a7a7b94dbed02a3ab1971dd329b9e81
   languageName: node
   linkType: hard
 
 "@codemirror/legacy-modes@npm:^6.3.2":
   version: 6.3.3
   resolution: "@codemirror/legacy-modes@npm:6.3.3"
   dependencies:
@@ -1575,129 +1589,155 @@
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
   checksum: 5e699960c1b28dbaa584fe091a3201978907bf4b9e52810fb15d3ceaf310e38053435e0b594da0985266ae812039a5cd6c36023284a6f8568664bdca04db137f
   languageName: node
   linkType: hard
 
 "@codemirror/search@npm:^6.3.0":
-  version: 6.5.4
-  resolution: "@codemirror/search@npm:6.5.4"
+  version: 6.5.5
+  resolution: "@codemirror/search@npm:6.5.5"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
-  checksum: 32a68e40486730949ee79f54b9fcc6c744559aef188d3c5bf82881f62e5fc9468fa21cf227507638160043c797eb054205802a649cf4a2350928fc161d5aac40
+  checksum: 825196ef63273494ba9a6153b01eda385edb65e77a1e49980dd3a28d4a692af1e9575e03e4b6c84f6fa2afe72217113ff4c50f58b20d13fe0d277cda5dd7dc81
   languageName: node
   linkType: hard
 
-"@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.1.4, @codemirror/state@npm:^6.2.0":
-  version: 6.3.1
-  resolution: "@codemirror/state@npm:6.3.1"
-  checksum: 8e7e55b3824653936606b31f146737459cb6654c935d668e7f36113ad523e1951966640f647c1286ae4ef22e3f0c7e37a6dfcbbcdb7bbeacca43c17c80fcc918
+"@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.2.0, @codemirror/state@npm:^6.4.0":
+  version: 6.4.0
+  resolution: "@codemirror/state@npm:6.4.0"
+  checksum: c5236fe5786f1b85d17273a5c17fa8aeb063658c1404ab18caeb6e7591663ec96b65d453ab8162f75839c3801b04cd55ba4bc48f44cb61ebfeeee383f89553c7
   languageName: node
   linkType: hard
 
-"@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.17.0, @codemirror/view@npm:^6.9.6":
-  version: 6.21.4
-  resolution: "@codemirror/view@npm:6.21.4"
+"@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.17.0, @codemirror/view@npm:^6.23.0, @codemirror/view@npm:^6.9.6":
+  version: 6.23.1
+  resolution: "@codemirror/view@npm:6.23.1"
   dependencies:
-    "@codemirror/state": ^6.1.4
+    "@codemirror/state": ^6.4.0
     style-mod: ^4.1.0
     w3c-keyname: ^2.2.4
-  checksum: e320eb46a6556984081c97e0bf5a9f5d45de2a4db5d632e6ee689a32dc081b10bda87aa989c4563981e28bf25bb651d1be57158fc2e753b587e3c6f7e2e486b2
+  checksum: 5ea3ba5761c574e1f6e1f1058cb452189c890982a77991606d0ae40da3c6fff77f7c7fc3c43fa78d62677ccdfa65dbc56175706b793e34ad4ec7a63b21e8c18e
   languageName: node
   linkType: hard
 
-"@csstools/selector-specificity@npm:^2.0.2":
-  version: 2.2.0
-  resolution: "@csstools/selector-specificity@npm:2.2.0"
+"@csstools/css-parser-algorithms@npm:^2.3.1":
+  version: 2.5.0
+  resolution: "@csstools/css-parser-algorithms@npm:2.5.0"
   peerDependencies:
-    postcss-selector-parser: ^6.0.10
-  checksum: 97c89f23b3b527d7bd51ed299969ed2b9fbb219a367948b44aefec228b8eda6ae0ad74fe8a82f9aac8ff32cfd00bb6d0c98d1daeab2e8fc6d5c4af25e5be5673
+    "@csstools/css-tokenizer": ^2.2.3
+  checksum: 6bfbdb4052acca48de9db0806a1b18458709103390656634ebe3cf0390048a6e9b304b78173fbcd524e03669dacb5cc3bedbe8008c354ff9511aed4935dcfc6f
+  languageName: node
+  linkType: hard
+
+"@csstools/css-tokenizer@npm:^2.2.0":
+  version: 2.2.3
+  resolution: "@csstools/css-tokenizer@npm:2.2.3"
+  checksum: a2a69f0de516046f85b8f47916879780f9712bdda8166ab01dd47613515ff5a0771555c78badd220686bc1dae3cb0eea5de6896e1e326247a276cc8965520aa6
+  languageName: node
+  linkType: hard
+
+"@csstools/media-query-list-parser@npm:^2.1.4":
+  version: 2.1.7
+  resolution: "@csstools/media-query-list-parser@npm:2.1.7"
+  peerDependencies:
+    "@csstools/css-parser-algorithms": ^2.5.0
+    "@csstools/css-tokenizer": ^2.2.3
+  checksum: f910d9c29c84e828d121f451607fe9c275297041f317075ede935ffacdd7fd53fcbc0dd4993585e405b5337b7f991b864d101dff3cb8fc400e8c32a9aedbfe69
+  languageName: node
+  linkType: hard
+
+"@csstools/selector-specificity@npm:^3.0.0":
+  version: 3.0.1
+  resolution: "@csstools/selector-specificity@npm:3.0.1"
+  peerDependencies:
+    postcss-selector-parser: ^6.0.13
+  checksum: e4b5aac3bd3ca1f824cb9578f52b16046a519aa8050ce291da37e611976a83cd3b2b2f908d2678dd4cbbe00bbde8ec28c34fffc40dbbf9a13608dfcaf382ee80
   languageName: node
   linkType: hard
 
 "@discoveryjs/json-ext@npm:^0.5.0":
   version: 0.5.7
   resolution: "@discoveryjs/json-ext@npm:0.5.7"
   checksum: 2176d301cc258ea5c2324402997cf8134ebb212469c0d397591636cea8d3c02f2b3cf9fd58dcb748c7a0dade77ebdc1b10284fa63e608c033a1db52fddc69918
   languageName: node
   linkType: hard
 
-"@eslint-community/eslint-utils@npm:^4.2.0":
+"@eslint-community/eslint-utils@npm:^4.2.0, @eslint-community/eslint-utils@npm:^4.4.0":
   version: 4.4.0
   resolution: "@eslint-community/eslint-utils@npm:4.4.0"
   dependencies:
     eslint-visitor-keys: ^3.3.0
   peerDependencies:
     eslint: ^6.0.0 || ^7.0.0 || >=8.0.0
   checksum: cdfe3ae42b4f572cbfb46d20edafe6f36fc5fb52bf2d90875c58aefe226892b9677fef60820e2832caf864a326fe4fc225714c46e8389ccca04d5f9288aabd22
   languageName: node
   linkType: hard
 
-"@eslint-community/regexpp@npm:^4.4.0, @eslint-community/regexpp@npm:^4.6.1":
+"@eslint-community/regexpp@npm:^4.5.1, @eslint-community/regexpp@npm:^4.6.1":
   version: 4.10.0
   resolution: "@eslint-community/regexpp@npm:4.10.0"
   checksum: 2a6e345429ea8382aaaf3a61f865cae16ed44d31ca917910033c02dc00d505d939f10b81e079fa14d43b51499c640138e153b7e40743c4c094d9df97d4e56f7b
   languageName: node
   linkType: hard
 
-"@eslint/eslintrc@npm:^2.1.2":
-  version: 2.1.2
-  resolution: "@eslint/eslintrc@npm:2.1.2"
+"@eslint/eslintrc@npm:^2.1.4":
+  version: 2.1.4
+  resolution: "@eslint/eslintrc@npm:2.1.4"
   dependencies:
     ajv: ^6.12.4
     debug: ^4.3.2
     espree: ^9.6.0
     globals: ^13.19.0
     ignore: ^5.2.0
     import-fresh: ^3.2.1
     js-yaml: ^4.1.0
     minimatch: ^3.1.2
     strip-json-comments: ^3.1.1
-  checksum: bc742a1e3b361f06fedb4afb6bf32cbd27171292ef7924f61c62f2aed73048367bcc7ac68f98c06d4245cd3fabc43270f844e3c1699936d4734b3ac5398814a7
+  checksum: 10957c7592b20ca0089262d8c2a8accbad14b4f6507e35416c32ee6b4dbf9cad67dfb77096bbd405405e9ada2b107f3797fe94362e1c55e0b09d6e90dd149127
   languageName: node
   linkType: hard
 
-"@eslint/js@npm:8.52.0":
-  version: 8.52.0
-  resolution: "@eslint/js@npm:8.52.0"
-  checksum: 490893b8091a66415f4ac98b963d23eb287264ea3bd6af7ec788f0570705cf64fd6ab84b717785980f55e39d08ff5c7fde6d8e4391ccb507169370ce3a6d091a
+"@eslint/js@npm:8.56.0":
+  version: 8.56.0
+  resolution: "@eslint/js@npm:8.56.0"
+  checksum: 5804130574ef810207bdf321c265437814e7a26f4e6fac9b496de3206afd52f533e09ec002a3be06cd9adcc9da63e727f1883938e663c4e4751c007d5b58e539
   languageName: node
   linkType: hard
 
 "@fortawesome/fontawesome-free@npm:^5.12.0":
   version: 5.15.4
   resolution: "@fortawesome/fontawesome-free@npm:5.15.4"
   checksum: 32281c3df4075290d9a96dfc22f72fadb3da7055d4117e48d34046b8c98032a55fa260ae351b0af5d6f6fb57a2f5d79a4abe52af456da35195f7cb7dda27b4a2
   languageName: node
   linkType: hard
 
 "@humanwhocodes/config-array@npm:^0.11.13":
-  version: 0.11.13
-  resolution: "@humanwhocodes/config-array@npm:0.11.13"
+  version: 0.11.14
+  resolution: "@humanwhocodes/config-array@npm:0.11.14"
   dependencies:
-    "@humanwhocodes/object-schema": ^2.0.1
-    debug: ^4.1.1
+    "@humanwhocodes/object-schema": ^2.0.2
+    debug: ^4.3.1
     minimatch: ^3.0.5
-  checksum: f8ea57b0d7ed7f2d64cd3944654976829d9da91c04d9c860e18804729a33f7681f78166ef4c761850b8c324d362f7d53f14c5c44907a6b38b32c703ff85e4805
+  checksum: 861ccce9eaea5de19546653bccf75bf09fe878bc39c3aab00aeee2d2a0e654516adad38dd1098aab5e3af0145bbcbf3f309bdf4d964f8dab9dcd5834ae4c02f2
   languageName: node
   linkType: hard
 
 "@humanwhocodes/module-importer@npm:^1.0.1":
   version: 1.0.1
   resolution: "@humanwhocodes/module-importer@npm:1.0.1"
   checksum: 0fd22007db8034a2cdf2c764b140d37d9020bbfce8a49d3ec5c05290e77d4b0263b1b972b752df8c89e5eaa94073408f2b7d977aed131faf6cf396ebb5d7fb61
   languageName: node
   linkType: hard
 
-"@humanwhocodes/object-schema@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@humanwhocodes/object-schema@npm:2.0.1"
-  checksum: 24929487b1ed48795d2f08346a0116cc5ee4634848bce64161fb947109352c562310fd159fc64dda0e8b853307f5794605191a9547f7341158559ca3c8262a45
+"@humanwhocodes/object-schema@npm:^2.0.2":
+  version: 2.0.2
+  resolution: "@humanwhocodes/object-schema@npm:2.0.2"
+  checksum: 2fc11503361b5fb4f14714c700c02a3f4c7c93e9acd6b87a29f62c522d90470f364d6161b03d1cc618b979f2ae02aed1106fd29d302695d8927e2fc8165ba8ee
   languageName: node
   linkType: hard
 
 "@isaacs/cliui@npm:^8.0.2":
   version: 8.0.2
   resolution: "@isaacs/cliui@npm:8.0.2"
   dependencies:
@@ -1999,120 +2039,120 @@
 "@jridgewell/sourcemap-codec@npm:^1.4.10, @jridgewell/sourcemap-codec@npm:^1.4.14":
   version: 1.4.15
   resolution: "@jridgewell/sourcemap-codec@npm:1.4.15"
   checksum: b881c7e503db3fc7f3c1f35a1dd2655a188cc51a3612d76efc8a6eb74728bef5606e6758ee77423e564092b4a518aba569bbb21c9bac5ab7a35b0c6ae7e344c8
   languageName: node
   linkType: hard
 
-"@jridgewell/trace-mapping@npm:^0.3.12, @jridgewell/trace-mapping@npm:^0.3.17, @jridgewell/trace-mapping@npm:^0.3.18, @jridgewell/trace-mapping@npm:^0.3.9":
-  version: 0.3.20
-  resolution: "@jridgewell/trace-mapping@npm:0.3.20"
+"@jridgewell/trace-mapping@npm:^0.3.12, @jridgewell/trace-mapping@npm:^0.3.17, @jridgewell/trace-mapping@npm:^0.3.18, @jridgewell/trace-mapping@npm:^0.3.20, @jridgewell/trace-mapping@npm:^0.3.9":
+  version: 0.3.22
+  resolution: "@jridgewell/trace-mapping@npm:0.3.22"
   dependencies:
     "@jridgewell/resolve-uri": ^3.1.0
     "@jridgewell/sourcemap-codec": ^1.4.14
-  checksum: cd1a7353135f385909468ff0cf20bdd37e59f2ee49a13a966dedf921943e222082c583ade2b579ff6cd0d8faafcb5461f253e1bf2a9f48fec439211fdbe788f5
+  checksum: ac7dd2cfe0b479aa1b81776d40d789243131cc792dc8b6b6a028c70fcd6171958ae1a71bf67b618ffe3c0c3feead9870c095ee46a5e30319410d92976b28f498
   languageName: node
   linkType: hard
 
-"@jupyter/ydoc@npm:^1.0.2":
+"@jupyter/ydoc@npm:^1.1.1":
   version: 1.1.1
   resolution: "@jupyter/ydoc@npm:1.1.1"
   dependencies:
     "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0
     "@lumino/coreutils": ^1.11.0 || ^2.0.0
     "@lumino/disposable": ^1.10.0 || ^2.0.0
     "@lumino/signaling": ^1.10.0 || ^2.0.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   checksum: a239b1dd57cfc9ba36c06ac5032a1b6388849ae01a1d0db0d45094f71fdadf4d473b4bf8becbef0cfcdc85cae505361fbec0822b02da5aa48e06b66f742dd7a0
   languageName: node
   linkType: hard
 
-"@jupyterlab/application@npm:^3.1.0 || ^4.0.0, @jupyterlab/application@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/application@npm:4.0.8"
+"@jupyterlab/application@npm:^4.0.0, @jupyterlab/application@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/application@npm:4.0.11"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/docregistry": ^4.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/statedb": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/statedb": ^4.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
     "@lumino/algorithm": ^2.0.1
     "@lumino/application": ^2.2.1
     "@lumino/commands": ^2.1.3
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.0
-  checksum: e6c50720992d50f8d6151752a31bf8dda2a21e912e896bbe9037f72086bddb515836fb9554603df8773313b27f45a39e01bda7e7b75cb2aca70ef15bcae1bc5e
+  checksum: 9df885a5369cd43bc6636ef24afaa4bb371f3fff8940e3487bdb5e0de4b6a70bb33b43c6a50da69590c563b4d3e04f5219de0239a7aa859ffac7d3d1e017d23f
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/apputils@npm:4.1.8"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/settingregistry": ^4.0.8
-    "@jupyterlab/statedb": ^4.0.8
-    "@jupyterlab/statusbar": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+"@jupyterlab/apputils@npm:^4.1.11":
+  version: 4.1.11
+  resolution: "@jupyterlab/apputils@npm:4.1.11"
+  dependencies:
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/settingregistry": ^4.0.11
+    "@jupyterlab/statedb": ^4.0.11
+    "@jupyterlab/statusbar": ^4.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
     "@lumino/algorithm": ^2.0.1
     "@lumino/commands": ^2.1.3
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.0
     "@types/react": ^18.0.26
     react: ^18.2.0
     sanitize-html: ~2.7.3
-  checksum: 1b028893ac0358d9f90585edd5fbb89a4fe251c31789cf6d809fb316b91c958c6ba33884d463dbe78dfdd864b579535e1e1849bcb9b16853002271a71418d31e
+  checksum: ab1bfa8e95de86464c35a2460e9cc4f89594a2cb69b38c19fd6d17a1c3d89e5c9fb368a1ac5425b5190c407e64c305c428e076a701117fc9007d0176bfe98501
   languageName: node
   linkType: hard
 
-"@jupyterlab/attachments@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/attachments@npm:4.0.8"
+"@jupyterlab/attachments@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/attachments@npm:4.0.11"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
-  checksum: 17e14257fb28006144bd7824e9f78e5c4c792c9dfa60e67efdd0bb6e6e33109b52e1e10b18d8a76f4d8e5e8d4ab9a22254e92f13d8c8f9ed0803961f5de8ece0
+  checksum: 13792a1a69280e48fcdaa5405042dad9135a1696197f40527a0c7c250285eab4330436df8cfa4e84b10f60ab07f4674c7abc89f98c50576061ca02c609458a84
   languageName: node
   linkType: hard
 
 "@jupyterlab/builder@npm:^4.0.0":
-  version: 4.0.8
-  resolution: "@jupyterlab/builder@npm:4.0.8"
+  version: 4.0.11
+  resolution: "@jupyterlab/builder@npm:4.0.11"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/application": ^2.2.1
     "@lumino/commands": ^2.1.3
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
-    "@lumino/dragdrop": ^2.1.3
+    "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.0
     ajv: ^8.12.0
     commander: ^9.4.1
@@ -2131,80 +2171,80 @@
     terser-webpack-plugin: ^5.3.7
     webpack: ^5.76.1
     webpack-cli: ^5.0.1
     webpack-merge: ^5.8.0
     worker-loader: ^3.0.2
   bin:
     build-labextension: lib/build-labextension.js
-  checksum: 9a1feeba36ba85ac0f1538f8df1b5a2140e5d1786530b7351880b8fb45b2902e961a48c2625d619c0b5c09b68299d9fea045adf139e439fd0f7f3cce41794662
+  checksum: 25f25098887572bb508759317b5a7e11716d3e45e554d3858dd16a70117a098281f2664ab8e89ea868298d279ae13840eda51924c39832aa43a3b994598058fe
   languageName: node
   linkType: hard
 
-"@jupyterlab/cells@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/cells@npm:4.0.8"
+"@jupyterlab/cells@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/cells@npm:4.0.11"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/attachments": ^4.0.8
-    "@jupyterlab/codeeditor": ^4.0.8
-    "@jupyterlab/codemirror": ^4.0.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/documentsearch": ^4.0.8
-    "@jupyterlab/filebrowser": ^4.0.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/outputarea": ^4.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/toc": ^6.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/attachments": ^4.0.11
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/codemirror": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/documentsearch": ^4.0.11
+    "@jupyterlab/filebrowser": ^4.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/outputarea": ^4.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/toc": ^6.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/domutils": ^2.0.1
-    "@lumino/dragdrop": ^2.1.3
+    "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: 42e4464574a603f48df299ccf2d84bf5f90f0aa39b0a9c680c9db5d254b416ee784ec3b5a1475ed72a10e6dcf1075715d66bf3afeee55e365c42656daea3f002
+  checksum: c0d554269b0ab598f6ee197e76e3d3aaadf2a17bee778b899f00d2446ca51b1846b03771fb69fbce6009f50c62e8c2d7cfb6f1bcb763d7bd70a6e4f809c7a4d7
   languageName: node
   linkType: hard
 
-"@jupyterlab/codeeditor@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/codeeditor@npm:4.0.8"
+"@jupyterlab/codeeditor@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/codeeditor@npm:4.0.11"
   dependencies:
     "@codemirror/state": ^6.2.0
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/statusbar": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/statusbar": ^4.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
-    "@lumino/dragdrop": ^2.1.3
+    "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: 151be40c60bcedf463d01b9c53466afc4b4747dd341fb4d5c2b9fc8b3c181af2ba391f867e10e78bb948848cdd300139b4b112634dec9f8aac9c36c5a13e1654
+  checksum: 65e3a5ad115fd288d4389b90e0d475051192f361d9ac119d3b75d150db973c735638051474dae18a3fca9ba8e986ea33b57ed424f1c444bafcd60b3e47e548f3
   languageName: node
   linkType: hard
 
-"@jupyterlab/codemirror@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/codemirror@npm:4.0.8"
+"@jupyterlab/codemirror@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/codemirror@npm:4.0.11"
   dependencies:
     "@codemirror/autocomplete": ^6.5.1
     "@codemirror/commands": ^6.2.3
     "@codemirror/lang-cpp": ^6.0.2
     "@codemirror/lang-css": ^6.1.1
     "@codemirror/lang-html": ^6.4.3
     "@codemirror/lang-java": ^6.0.1
@@ -2218,418 +2258,419 @@
     "@codemirror/lang-wast": ^6.0.1
     "@codemirror/lang-xml": ^6.0.2
     "@codemirror/language": ^6.6.0
     "@codemirror/legacy-modes": ^6.3.2
     "@codemirror/search": ^6.3.0
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/codeeditor": ^4.0.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/documentsearch": ^4.0.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/documentsearch": ^4.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/translation": ^4.0.11
     "@lezer/common": ^1.0.2
     "@lezer/generator": ^1.2.2
     "@lezer/highlight": ^1.1.4
     "@lezer/markdown": ^1.0.2
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     yjs: ^13.5.40
-  checksum: 2edd2ac9d695f8107d444379289b4cecf3603c118d748608738abe2a1af9d311d0407c5709ccbe016dd0a16c3a52d7f0132446173678246841c8ddf8ade371c7
+  checksum: e4d16faad69575a6d3c4e41ab3cc268475c92f0783ca14013dc701cc2f12ee4eb7b37c1a650d9e60f17fe4daf0fba303e7cb984e06e9fde587c8075bbee7f1c8
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^6.0.8":
-  version: 6.0.8
-  resolution: "@jupyterlab/coreutils@npm:6.0.8"
+"@jupyterlab/coreutils@npm:^6.0.0, @jupyterlab/coreutils@npm:^6.0.11":
+  version: 6.0.11
+  resolution: "@jupyterlab/coreutils@npm:6.0.11"
   dependencies:
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
-  checksum: b56e3b95c0ce52745b79549ef5b18a27e620086b87cf997b3a743b59d18dc529e403c812751b7e294a4abc60ac957381301e14327e1a4b9c1afb232f181f3a4d
+  checksum: 2a3ab30865439d486ad180c0779bf086992d5999727e1fb4cbadad6ecd4c53fbcfcde4fc611d9819dc28aedc6b36e7b48d267ff2bcdd8f35de5b4f3d7145f2cc
   languageName: node
   linkType: hard
 
-"@jupyterlab/docmanager@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/docmanager@npm:4.0.8"
+"@jupyterlab/docmanager@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/docmanager@npm:4.0.11"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/docregistry": ^4.0.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/statusbar": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/statusbar": ^4.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: 70eea965bb9edd6a4042c92d2cb98f8b1b145b6727a354e12e3f5ab84ff2ab7207c5d9433c43c03d01f4377f9dc901359d789d0f47d2c725e56f41c487295550
+  checksum: 964f85cceb54866bb3c603d5d7b3d3f064cb481917ae1e1f6aaf16fe2fb2a0863a9ab8427b82e72eed171e3ae80043b0de72e514dce0a4a0feb46e39c2faf9a0
   languageName: node
   linkType: hard
 
-"@jupyterlab/docregistry@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/docregistry@npm:4.0.8"
-  dependencies:
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/codeeditor": ^4.0.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+"@jupyterlab/docregistry@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/docregistry@npm:4.0.11"
+  dependencies:
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.0
-  checksum: 280697f97ca146cc711c5dafa1b27eaa89d96bc53fc92ade7d4b78c44c997feb9d2495b392c31e75ed3c836797865e2f3fa6ea8f3207f46a4ab2d26061dc9498
+  checksum: 0c08ec3660f17b6d45aae030215a008278e82068b94bdd1bb77ec4e2995b5ef974830e90a78f5b46e7863204bab1ac397306c5d65901fed4f6bca5e57b4cbe05
   languageName: node
   linkType: hard
 
-"@jupyterlab/documentsearch@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/documentsearch@npm:4.0.8"
+"@jupyterlab/documentsearch@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/documentsearch@npm:4.0.11"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: 5ee4c4b910af158b4ca488c617b12b2a84d391cfb6be94a38136a1eb80f639ec4b446fd862748a76732bc3eccd290750c0e9f6b6211d3c15d0776073173a5343
+  checksum: 1fa0087c6a0bc40e653a8e67f362b8765558ff9e1c6cf4dedb2e010cdd5112d863d9f10804f36dc22d79f41ad0757c54446af923337ad27e922f972881141bd4
   languageName: node
   linkType: hard
 
-"@jupyterlab/filebrowser@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/filebrowser@npm:4.0.8"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/docmanager": ^4.0.8
-    "@jupyterlab/docregistry": ^4.0.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/statedb": ^4.0.8
-    "@jupyterlab/statusbar": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+"@jupyterlab/filebrowser@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/filebrowser@npm:4.0.11"
+  dependencies:
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docmanager": ^4.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/statedb": ^4.0.11
+    "@jupyterlab/statusbar": ^4.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
-    "@lumino/dragdrop": ^2.1.3
+    "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: 907dade3b9ab6bde667cdf2acc76c0fb2d631c06d794115a456cb6b1995a3b89b2a9f5c53a75824b337833cd05967c55fd919ca1311f24279aa5f067f948378a
+  checksum: d4a452fd6e0772a79d662537a8abf10f83c1a66739813e73bf9218ef8c94b388bdfdb2919d97e135b914c40abfed551cb43b7bcc92b3bb896f99f3e5584d257f
   languageName: node
   linkType: hard
 
-"@jupyterlab/lsp@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/lsp@npm:4.0.8"
+"@jupyterlab/lsp@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/lsp@npm:4.0.11"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/codeeditor": ^4.0.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/docregistry": ^4.0.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/translation": ^4.0.8
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/translation": ^4.0.11
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     lodash.mergewith: ^4.6.1
     vscode-jsonrpc: ^6.0.0
     vscode-languageserver-protocol: ^3.17.0
     vscode-ws-jsonrpc: ~1.0.2
-  checksum: baf2d42800a617a9d06d8cbb9c755e0cc40994c25c7c5d31bca1b7ac4fc4ad67d77fadb53de020e52d499a46e41dea1d84abb388b9bc20d468a5e888c687f301
+  checksum: e2ca0286320c1c7855cf5c2eecf301037202de4df1e53ac109affd73b41c686a27e6205591f7a0ca85376d595db3e4779a423599c18745df24df93ad124be1a0
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/nbformat@npm:4.0.8"
+"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/nbformat@npm:4.0.11"
   dependencies:
     "@lumino/coreutils": ^2.1.2
-  checksum: 2d8255ac7c7c20dbfa8497ce4d8d2f5840568adefb2feaec8eb8ddbb4892f50706ce60e8c4719113485c5523f720802f7e4e7b63ed43fac90f870ff1134bed7a
+  checksum: 7bb488e94f09d66d858ce2a001e208beca9f1e87fc674332c4630cfb5039a6bd1579d9071019782aba546a9b43e2a7de5b125f7a0a7a7caa0b190a2b8d1266b6
   languageName: node
   linkType: hard
 
-"@jupyterlab/notebook@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/notebook@npm:4.0.8"
-  dependencies:
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/cells": ^4.0.8
-    "@jupyterlab/codeeditor": ^4.0.8
-    "@jupyterlab/codemirror": ^4.0.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/docregistry": ^4.0.8
-    "@jupyterlab/documentsearch": ^4.0.8
-    "@jupyterlab/lsp": ^4.0.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/settingregistry": ^4.0.8
-    "@jupyterlab/statusbar": ^4.0.8
-    "@jupyterlab/toc": ^6.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+"@jupyterlab/notebook@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/notebook@npm:4.0.11"
+  dependencies:
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/cells": ^4.0.11
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/codemirror": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/documentsearch": ^4.0.11
+    "@jupyterlab/lsp": ^4.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/settingregistry": ^4.0.11
+    "@jupyterlab/statusbar": ^4.0.11
+    "@jupyterlab/toc": ^6.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/domutils": ^2.0.1
-    "@lumino/dragdrop": ^2.1.3
+    "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: 64ea11e1923fcae46d263c732cfa6a69a51099bdd637f40599da5359fb884600179a3c5b6f3c176c6ffa725f425b33f435be6391f8d087b443e5fc6d6d11ced2
+  checksum: e8bbfca1cba7b78427fcca1211266ba989e4950da2361a3606a6ab8485ab4618c6f1a321463a8974b96c7a77d4d00ed9b293abf68f9ce84731bd0e9687ec8be7
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^5.0.8":
-  version: 5.0.8
-  resolution: "@jupyterlab/observables@npm:5.0.8"
+"@jupyterlab/observables@npm:^5.0.11":
+  version: 5.0.11
+  resolution: "@jupyterlab/observables@npm:5.0.11"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: 833c6af7f66a338d53e4ebfae2c10c57a55b8a1710730eed89e7a0103a4dd27b7b5634d0e7cf9c7db47d891fd4c8e72235de9816833482ef68356846200613be
+  checksum: b47cc8e73db9cc856454c0db530b774a4d11f6ade066b52fe521b0cec2b7a8f5eebfe2c0f0f7ada976474698dab9a77bdef3feea2960ea75bcf7052404ebec16
   languageName: node
   linkType: hard
 
-"@jupyterlab/outputarea@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/outputarea@npm:4.0.8"
+"@jupyterlab/outputarea@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/outputarea@npm:4.0.11"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/translation": ^4.0.8
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/translation": ^4.0.11
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.0
-  checksum: 4e97a367d6d06b05838056ef6da48891484fe84e5c06a08f0928f7359fa8362f48903434d033e8ddabdc193ef4b61859855fecbebda3949703583275fd099339
+  checksum: f9c69319d0bd144f35840d72784b606153fe62d44b51a22f11ab4ee7088a262955dff4ea86de8b1bd929841294c8c5a3fadff37fa46b15ca53586868bb498cad
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime-interfaces@npm:^3.8.8":
-  version: 3.8.8
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.8"
+"@jupyterlab/rendermime-interfaces@npm:^3.8.11":
+  version: 3.8.11
+  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.11"
   dependencies:
     "@lumino/coreutils": ^1.11.0 || ^2.1.2
     "@lumino/widgets": ^1.37.2 || ^2.3.0
-  checksum: b356cc18acedd7eebbf9e6f03329ad58f0aadb676ef7ef6b64dec610857a53593662df54752bb58780d34f39938ec35c6940918513e3a3cef7c5893bd0909684
+  checksum: 277373ca5e05bfbcd6e88c38cdf5c1bdfc052beaf1cac120cb3a458d96cce949b17c9b47cfd16cfcf2e2241530fa9f3062343512084b79a549f6bde84a846c84
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/rendermime@npm:4.0.8"
+"@jupyterlab/rendermime@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/rendermime@npm:4.0.11"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/translation": ^4.0.8
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/translation": ^4.0.11
     "@lumino/coreutils": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.0
     lodash.escape: ^4.0.1
-  checksum: c1f9ebffc746fdc13c1b14a148fd2ae10132b5ca4e1eab27d18ac5bf3d3ae70cf2850b06f6c05a799f2c769792d81dab1447885d0cda7206c7cf63af10bbe4f2
+  checksum: cb76d6824caac3b50e4e38c171f7db7239deb4499b0be237d51c68b3195c4d2edb1e4fa42253183949459ae0b78a1acbdc936b1eba51c8472bcf89586d267975
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^7.0.8":
-  version: 7.0.8
-  resolution: "@jupyterlab/services@npm:7.0.8"
+"@jupyterlab/services@npm:^7.0.0, @jupyterlab/services@npm:^7.0.11":
+  version: 7.0.11
+  resolution: "@jupyterlab/services@npm:7.0.11"
   dependencies:
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/settingregistry": ^4.0.8
-    "@jupyterlab/statedb": ^4.0.8
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/settingregistry": ^4.0.11
+    "@jupyterlab/statedb": ^4.0.11
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     ws: ^8.11.0
-  checksum: b0112854d3014eff9d9855a6840d1efd0d866d4c011e7a9c4c1c5fba404dd13107b62de6ce845902d12cc6404aafdfee95127a2af43560ade53a00fc7b73378a
+  checksum: 6539cc1b34f29feaab094a570576890984fe9cc3f0140dc3b17cca1ead878197bd3d2ca01b4f6fe6808ee5dca8f720769e0db10a27f1fcad1759b6ead9631b24
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:^3.1.0 || ^4.0.0, @jupyterlab/settingregistry@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/settingregistry@npm:4.0.8"
+"@jupyterlab/settingregistry@npm:^4.0.0, @jupyterlab/settingregistry@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/settingregistry@npm:4.0.11"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/statedb": ^4.0.8
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/statedb": ^4.0.11
     "@lumino/commands": ^2.1.3
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@rjsf/utils": ^5.1.0
     ajv: ^8.12.0
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
-  checksum: e9661539357edae60e4b300dff68b369e95e96acb343aeb25e23bdbcd6964c59dd40118ce3a856afaf969833958f3872c480e75cc488a5e882546cb88587c461
+  checksum: 97d06a08eff0589e83c40611f50e765dc8c75b33f821bee86defdb856c7747276174cc3370374159a37ae1393779cf18634fbca69072db447c053ccb872f3117
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/statedb@npm:4.0.8"
+"@jupyterlab/statedb@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/statedb@npm:4.0.11"
   dependencies:
     "@lumino/commands": ^2.1.3
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: bfd016e91158daf47e07e760126c0c2c3f6d01ecc8e9cad3e17241e5873decbc5fdfce82bf039fa83633b8760245af8003008f38272dafba56b73ac24768a99f
+  checksum: b0637af63185b71db698ce572d2fcdaee94e6fe93659ead1e2301cb6ee1ec2b16164a61275cb44af3cac679d40b1a2c3492f20b44d9eb07a75440706627cd733
   languageName: node
   linkType: hard
 
-"@jupyterlab/statusbar@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/statusbar@npm:4.0.8"
+"@jupyterlab/statusbar@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/statusbar@npm:4.0.11"
   dependencies:
-    "@jupyterlab/ui-components": ^4.0.8
+    "@jupyterlab/ui-components": ^4.0.11
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: a07345a173e1c4500e5ce9aca6c8d619e5fecd928de0f6e88fd29241b39c09b85b26722279cc8119031d3015f2b32a0d3b9d85fd3cf9370c7605ebcd37d0d31a
+  checksum: cb9d8e51533d1b0dd13f0459b3f33bab23c23dffdfb58467e58d47d0cb09f61fce320b67c50e3e5a2328fba9f7a815d4f483f460b6bea8b34cf7fcd02144fe10
   languageName: node
   linkType: hard
 
-"@jupyterlab/testing@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/testing@npm:4.0.8"
+"@jupyterlab/testing@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/testing@npm:4.0.11"
   dependencies:
     "@babel/core": ^7.10.2
     "@babel/preset-env": ^7.10.2
-    "@jupyterlab/coreutils": ^6.0.8
+    "@jupyterlab/coreutils": ^6.0.11
     "@lumino/coreutils": ^2.1.2
     "@lumino/signaling": ^2.1.2
     child_process: ~1.0.2
     deepmerge: ^4.2.2
     fs-extra: ^10.1.0
     identity-obj-proxy: ^3.0.0
     jest: ^29.2.0
     jest-environment-jsdom: ^29.3.0
     jest-junit: ^15.0.0
     node-fetch: ^2.6.0
     simulate-event: ~1.4.0
     ts-jest: ^29.1.0
   peerDependencies:
     typescript: ">=4.3"
-  checksum: 79ee06da8052564d5ae877480e9a12fa0fce6b4c880543853e62d0a0db847aae5221308fb53b97909f22d7d6ce0223352a13e8246ae0b70b589dcaa7cc315ae2
+  checksum: 089bdc24bb4376e8eec4129aa36640925d0f5e68388be41ed292f6c1c9be350495caa854bab9779d1431ab17ad272288bb5659a1d555335c2638c57a518cf116
   languageName: node
   linkType: hard
 
 "@jupyterlab/testutils@npm:^4.0.0":
-  version: 4.0.8
-  resolution: "@jupyterlab/testutils@npm:4.0.8"
+  version: 4.0.11
+  resolution: "@jupyterlab/testutils@npm:4.0.11"
   dependencies:
-    "@jupyterlab/application": ^4.0.8
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/notebook": ^4.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/testing": ^4.0.8
-  checksum: 70ee9e782847018cc0a18e304a9b3a8e0316bc1d811d8da815ba82f9c15ff7d54bb254ec41b9313b84f8f0c801f08793845a30241bf1c585ee11c16d6585a907
+    "@jupyterlab/application": ^4.0.11
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/notebook": ^4.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/testing": ^4.0.11
+  checksum: fbd17fe208d7cf8a1a80cfbe3aa0e08f9ac15436960729da9a870ce4a77c562b3dd9ac585f393faae25ebe23e7ee35a399b247284aa11d7856248a48f036e218
   languageName: node
   linkType: hard
 
-"@jupyterlab/toc@npm:^6.0.8":
-  version: 6.0.8
-  resolution: "@jupyterlab/toc@npm:6.0.8"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/docregistry": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+"@jupyterlab/toc@npm:^6.0.11":
+  version: 6.0.11
+  resolution: "@jupyterlab/toc@npm:6.0.11"
+  dependencies:
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: 5d4373c5e0b3ea302275cdf117e17a201a6ab8337288cbdb7e6048b87de2ed8e293e3dd203fb23f7d25db080e06e8271559b1d5aa5e33202130cc95d0972b95f
+  checksum: d93d003e65b36d648407c20d19d232c0c232e9c92757b7910a170a5bfc721ec2b229a97efb553726bfa940f570b54ec3dabf8d1bae07ab84a577903d1fd039e1
   languageName: node
   linkType: hard
 
-"@jupyterlab/translation@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/translation@npm:4.0.8"
+"@jupyterlab/translation@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/translation@npm:4.0.11"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/statedb": ^4.0.8
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/statedb": ^4.0.11
     "@lumino/coreutils": ^2.1.2
-  checksum: 998d42d85ccd779237ac69abfaf2e341d865374ed5a1a4d234470337f498636511eec0562c741ad44a6a75fae930a510a0a76e176f72665499be2b7edb0dc5f8
+  checksum: 1e65d0a162d56724a99dcb7eec874b80e78f8113e14d9cc1461f56cebef9a21604baf1fffd43cd62f186942b63fd49effec2b1960e4e3aca0a6cbe03df46bd51
   languageName: node
   linkType: hard
 
-"@jupyterlab/ui-components@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/ui-components@npm:4.0.8"
+"@jupyterlab/ui-components@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/ui-components@npm:4.0.11"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/translation": ^4.0.8
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/translation": ^4.0.11
     "@lumino/algorithm": ^2.0.1
     "@lumino/commands": ^2.1.3
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
@@ -2639,205 +2680,214 @@
     "@rjsf/core": ^5.1.0
     "@rjsf/utils": ^5.1.0
     react: ^18.2.0
     react-dom: ^18.2.0
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
-  checksum: 7bf11f5ee3c1f88656175c0d3b290be0670d7787076a1eba944875e4780bc2b34c0b9a3af038806ff925620b3056cee36daff08f3ff91acc6c46fd1438bf004d
+  checksum: 0ad2fcdcb531ffc4da4f475c24520007d65190c70bfe07888f4284256754e15ffb77d23f02a6ce44688bad0103484cba22327db49796abb13f8dfc335ea2373d
   languageName: node
   linkType: hard
 
-"@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2, @lezer/common@npm:^1.1.0":
-  version: 1.1.0
-  resolution: "@lezer/common@npm:1.1.0"
-  checksum: 93c208a44d1c0bdf7407853ba7c4ddcedf1c52d1b82170813d83b9bd6301aa23587405ac54332fe39ce8bc37f706936ab237ceb4d3d535d1dead650153b6474c
+"@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2, @lezer/common@npm:^1.1.0, @lezer/common@npm:^1.2.0, @lezer/common@npm:^1.2.1":
+  version: 1.2.1
+  resolution: "@lezer/common@npm:1.2.1"
+  checksum: 0bd092e293a509ce334f4aaf9a4d4a25528f743cd9d7e7948c697e34ac703b805b288b62ad01563488fb206fc34ff05084f7fc5d864be775924b3d0d53ea5dd2
   languageName: node
   linkType: hard
 
 "@lezer/cpp@npm:^1.0.0":
-  version: 1.1.1
-  resolution: "@lezer/cpp@npm:1.1.1"
+  version: 1.1.2
+  resolution: "@lezer/cpp@npm:1.1.2"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: c9e1db19776eafbfe0c3b8448d46c94d9a1d30f7fef630292e63bab82e6d5d6903a043ee8cf341bcbf84c00ee0d79b8c255bab8fd8e0a91355ae912b53c78935
+  checksum: a319cd46fd32affc07c9432e9b2b9954becf7766be0361176c525d03474bb794cc051aad9932f48c9df33833eee1d6bfdccab12e571f2b137b4ca765c60c75de
   languageName: node
   linkType: hard
 
 "@lezer/css@npm:^1.0.0, @lezer/css@npm:^1.1.0":
-  version: 1.1.3
-  resolution: "@lezer/css@npm:1.1.3"
+  version: 1.1.7
+  resolution: "@lezer/css@npm:1.1.7"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: c8069ef0a6751441d2dc9180f7ebfd7aeb35df0ca2f1a748a2f26203a9ef6cc30f17f3074e2b49520453eb39329dadfdbbb901c6d9d067dc955ceb58c1f8cc6a
+  checksum: 7760d294fd0b1ac6db319c4990517c1ed9027d6757de537553624238056df6e1ef1b6a571a023a4bce3d7a2b891036d9f85f76f2109f503bea94837f90c64bc2
   languageName: node
   linkType: hard
 
 "@lezer/generator@npm:^1.2.2":
-  version: 1.5.1
-  resolution: "@lezer/generator@npm:1.5.1"
+  version: 1.6.0
+  resolution: "@lezer/generator@npm:1.6.0"
   dependencies:
-    "@lezer/common": ^1.0.2
+    "@lezer/common": ^1.1.0
     "@lezer/lr": ^1.3.0
   bin:
     lezer-generator: src/lezer-generator.cjs
-  checksum: 4d8267e6d356e48ca5214a234679b2b3b1d3706cb9dffecee4495b7a16c8a02502d6a078f8afdf5d8c79f94af34f2c1b5c08556aead8376d7b23795612b651d0
+  checksum: dfbf19d0533922272ac00c4b7884e1df88e2a35dd758e4544ceb5d784aa38d5751add03ca87f35d14cc39416e0dbc06ccaf2a211a6ae982e00daaaffe9c9320c
   languageName: node
   linkType: hard
 
 "@lezer/highlight@npm:^1.0.0, @lezer/highlight@npm:^1.1.3, @lezer/highlight@npm:^1.1.4":
-  version: 1.1.6
-  resolution: "@lezer/highlight@npm:1.1.6"
+  version: 1.2.0
+  resolution: "@lezer/highlight@npm:1.2.0"
   dependencies:
     "@lezer/common": ^1.0.0
-  checksum: 411a702394c4c996b7d7f145a38f3a85a8cc698b3918acc7121c629255bb76d4ab383753f69009e011dc415210c6acbbb5b27bde613259ab67e600b29397b03b
+  checksum: 5b9dfe741f95db13f6124cb9556a43011cb8041ecf490be98d44a86b04d926a66e912bcd3a766f6a3d79e064410f1a2f60ab240b50b645a12c56987bf4870086
   languageName: node
   linkType: hard
 
 "@lezer/html@npm:^1.3.0":
-  version: 1.3.6
-  resolution: "@lezer/html@npm:1.3.6"
+  version: 1.3.8
+  resolution: "@lezer/html@npm:1.3.8"
   dependencies:
-    "@lezer/common": ^1.0.0
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 1d3af781660968505e5083a34f31ea3549fd5f3949227fa93cc318bca61bce76ffe977bd875624ba938a2039834ec1a33df5d365e94c48131c85dd26f980d92c
+  checksum: 06bce804487435ea6ccb39595176bb65d68691f082b0b68fb7d22d90d4de9798a8202f16e9aefe22865db15257a37f6fca93275d660715eea98f7578579e7135
   languageName: node
   linkType: hard
 
 "@lezer/java@npm:^1.0.0":
-  version: 1.0.4
-  resolution: "@lezer/java@npm:1.0.4"
+  version: 1.1.1
+  resolution: "@lezer/java@npm:1.1.1"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 97f5a2c2d733afba5dc57a0da9a97515b19b5e63bb5937717dac4e8c9baed74d15c0cb5c1580858b678931f11d517c56d89f903968fa48931f9c62e2ea67a107
+  checksum: 8a071aca6b5e1ed1d22bffed22bbd29f21b102b7337a7ea5c956eb259e6ff20eee2d6e85b7dadff69859cb6615d6b1a3f0ba109673e87ce5a1f6cabdeee626fd
   languageName: node
   linkType: hard
 
 "@lezer/javascript@npm:^1.0.0":
-  version: 1.4.9
-  resolution: "@lezer/javascript@npm:1.4.9"
+  version: 1.4.13
+  resolution: "@lezer/javascript@npm:1.4.13"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.1.3
     "@lezer/lr": ^1.3.0
-  checksum: adac0048e4ab33dc48db42014f02d53a2eab81d12c990b23f237a3e83b125bda271607442aaa50dc0ac870a803e678135111366235f7c29a5052a288c1003960
+  checksum: a5e4607fec7671dff66d1f3bfee5a5da7395982f1867e17ac4d8f2d8f223451fb18516ef2699340b148af112176a07e1fcba9e63c5f8397c12895dd0509113d6
   languageName: node
   linkType: hard
 
 "@lezer/json@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@lezer/json@npm:1.0.1"
+  version: 1.0.2
+  resolution: "@lezer/json@npm:1.0.2"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: fcd17178f6a58e71c83e08fdc047e3708528b28591ba8f08ed35268f370d1ec9b63af0afa9d82a77fec26e9eb477ab3cfdc31c951e080d118ef607f9f9bb52e3
+  checksum: f899d13765d95599c9199fc3404cb57969031dc40ce07de30f4e648979153966581f0bee02e2f8f70463b0a5322206a97c2fe8d5d14f218888c72a6dcedf90ef
   languageName: node
   linkType: hard
 
 "@lezer/lr@npm:^1.0.0, @lezer/lr@npm:^1.1.0, @lezer/lr@npm:^1.3.0":
-  version: 1.3.14
-  resolution: "@lezer/lr@npm:1.3.14"
+  version: 1.4.0
+  resolution: "@lezer/lr@npm:1.4.0"
   dependencies:
     "@lezer/common": ^1.0.0
-  checksum: 07be41edcb6c332a3567436d2c626131544181c4d680811baf23f6157db3dce4ebfef325cbd0b88dc8b128b83fbe6363c5dcf3e0a4ff369ddfae05d9f207daee
+  checksum: 4c8517017e9803415c6c5cb8230d8764107eafd7d0b847676cd1023abb863a4b268d0d01c7ce3cf1702c4749527c68f0a26b07c329cb7b68c36ed88362d7b193
   languageName: node
   linkType: hard
 
 "@lezer/markdown@npm:^1.0.0, @lezer/markdown@npm:^1.0.2":
-  version: 1.1.0
-  resolution: "@lezer/markdown@npm:1.1.0"
+  version: 1.2.0
+  resolution: "@lezer/markdown@npm:1.2.0"
   dependencies:
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
-  checksum: b3699c0724dd41e3e6e3078a0e1bcd272ccaebf17b20e5160de3ecf26200cdaa59aa19c9542aac5ab8c7e3aecce1003544b016bb5c32e458bbd5982add8ca0bf
+  checksum: e6355272ad98c97b339dd42d8d9b78fa4f48fdcc5c9c408720936cacb7d2bcd47b0cedf8e0997ef93539c2b03a65326fc59372e54f0b24acd98630e06869a350
   languageName: node
   linkType: hard
 
 "@lezer/php@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@lezer/php@npm:1.0.1"
+  version: 1.0.2
+  resolution: "@lezer/php@npm:1.0.2"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.1.0
-  checksum: a847c255c030b4d38913ddf1d5bd7324d83be7ef8d1d244542870be03b9bf7dc71283afeb2415c40dfd188cb99f0cc44bad760b5f3b7c35c3b8e5e00253848fc
+  checksum: c85ef18571d37826b687dd141a0fe110f5814adaf9d1a391e7e482020d7f81df189ca89ec0dd141c1433d48eff4c6e53648b46f008dea8ad2dc574f35f1d4d79
   languageName: node
   linkType: hard
 
 "@lezer/python@npm:^1.1.4":
-  version: 1.1.9
-  resolution: "@lezer/python@npm:1.1.9"
+  version: 1.1.11
+  resolution: "@lezer/python@npm:1.1.11"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: cc7e712665f0b7990fd00ba798c2e377f8393d0034a85da33b370e256322d92f668f51b70aa91585ed165718bad60fba6e86203f877d537819874be2549ec31f
+  checksum: ed0e58317716967644f57bf29eb902c0c205b909bc035c0960520222a79bd6525468c8adfb7d824787a8a29ec7a1c7d2da5fd59f912cdeff2830c71958b9576d
   languageName: node
   linkType: hard
 
 "@lezer/rust@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@lezer/rust@npm:1.0.1"
+  version: 1.0.2
+  resolution: "@lezer/rust@npm:1.0.2"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 1e02fdf09206979e7d4f87b020589f410c4c5e452a7b7b0296f6772ce3571c1bd7ed37495fbeeecf3d4423000f2efdabd462ba8a949c2b351fd35550327a7613
+  checksum: fc5e97852b42beeb44a0ebe316dc64e3cc49ff481c22e3e67d6003fc4a5c257fcd94959cfcc76cd154fa172db9b3b4b28de5c09f10550d6e5f14869ddc274e5b
   languageName: node
   linkType: hard
 
 "@lezer/xml@npm:^1.0.0":
-  version: 1.0.3
-  resolution: "@lezer/xml@npm:1.0.3"
+  version: 1.0.4
+  resolution: "@lezer/xml@npm:1.0.4"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: a4758859abcab3bc3f8680f79f7fb7dbbb6842c7d552888f95cc85a845450342a18731fbf49cbaec5f39970b9e5b96a66c8381eda036d3ebf7c952da5ddd7666
+  checksum: 68a82085bff6c1525f4ef03cd9f9dac0132b3e03fe574e0289700dd4475056e40e8744cde15cf5ad6d3760d0d584ff85ce707e26a7c938d0c5fe2e325c1c336e
   languageName: node
   linkType: hard
 
 "@lumino/algorithm@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/algorithm@npm:2.0.1"
   checksum: cbf7fcf6ee6b785ea502cdfddc53d61f9d353dcb9659343511d5cd4b4030be2ff2ca4c08daec42f84417ab0318a3d9972a17319fa5231693e109ab112dcf8000
   languageName: node
   linkType: hard
 
 "@lumino/application@npm:^2.2.1":
-  version: 2.2.1
-  resolution: "@lumino/application@npm:2.2.1"
+  version: 2.3.0
+  resolution: "@lumino/application@npm:2.3.0"
   dependencies:
-    "@lumino/commands": ^2.1.3
+    "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
-    "@lumino/widgets": ^2.3.0
-  checksum: a33e661703728440bc7d2ddb4674261f4de0d20eb8c9846646cbd6debac03b5c65e78d739a500903550fd83b8f47b47fa82ec178c97bc9967ca3ac4014075cde
+    "@lumino/widgets": ^2.3.1
+  checksum: 9d1eb5bc972ed158bf219604a53bbac1262059bc5b0123d3e041974486b9cbb8288abeeec916f3b62f62d7c32e716cccf8b73e4832ae927e4f9dd4e4b0cd37ed
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
 
-"@lumino/commands@npm:^2.1.3":
-  version: 2.1.3
-  resolution: "@lumino/commands@npm:2.1.3"
+"@lumino/commands@npm:^2.1.3, @lumino/commands@npm:^2.2.0":
+  version: 2.2.0
+  resolution: "@lumino/commands@npm:2.2.0"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/keyboard": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-  checksum: e4e3ee279f2a5e8d68e4ce142c880333f5542f90c684972402356936ecb5cf5e07163800b59e7cb8c911cbdb4e5089edcc5dd2990bc8db10c87517268de1fc5d
+  checksum: 093e9715491e5cef24bc80665d64841417b400f2fa595f9b60832a3b6340c405c94a6aa276911944a2c46d79a6229f3cc087b73f50852bba25ece805abd0fae9
   languageName: node
   linkType: hard
 
 "@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.1.2, @lumino/coreutils@npm:^2.1.2":
   version: 2.1.2
   resolution: "@lumino/coreutils@npm:2.1.2"
   checksum: 7865317ac0676b448d108eb57ab5d8b2a17c101995c0f7a7106662d9fe6c859570104525f83ee3cda12ae2e326803372206d6f4c1f415a5b59e4158a7b81066f
@@ -2856,21 +2906,21 @@
 "@lumino/domutils@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/domutils@npm:2.0.1"
   checksum: 61fa0ab226869dfbb763fc426790cf5a43b7d6f4cea1364c6dd56d61c44bff05eea188d33ff847449608ef58ed343161bee15c19b96f35410e4ee35815dc611a
   languageName: node
   linkType: hard
 
-"@lumino/dragdrop@npm:^2.1.3":
-  version: 2.1.3
-  resolution: "@lumino/dragdrop@npm:2.1.3"
+"@lumino/dragdrop@npm:^2.1.4":
+  version: 2.1.4
+  resolution: "@lumino/dragdrop@npm:2.1.4"
   dependencies:
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
-  checksum: d5f7eb4cc9f9a084cb9af10f02d6741b25d683350878ecbc324e24ba9d4b5246451a410e2ca5fff227aab1c191d1e73a2faf431f93e13111d67a4e426e126258
+  checksum: 43d82484b13b38b612e7dfb424a840ed6a38d0db778af10655c4ba235c67b5b12db1683929b35a36ab2845f77466066dfd1ee25c1c273e8e175677eba9dc560d
   languageName: node
   linkType: hard
 
 "@lumino/keyboard@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/keyboard@npm:2.0.1"
   checksum: cf33f13427a418efd7cc91061233321e860d5404f3d86397781028309bef86c8ad2d88276ffe335c1db0fe619bd9d1e60641c81f881696957a58703ee4652c3e
@@ -2920,30 +2970,30 @@
   resolution: "@lumino/virtualdom@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
   checksum: cf59b6f15b430e13e9e657b7a0619b9056cd9ea7b2a87f407391d071c501b77403c302b6a66dca510382045e75b2e3fe551630bb391f1c6b33678057d4bec164
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^1.37.2 || ^2.3.0, @lumino/widgets@npm:^2.3.0":
-  version: 2.3.0
-  resolution: "@lumino/widgets@npm:2.3.0"
+"@lumino/widgets@npm:^1.37.2 || ^2.3.0, @lumino/widgets@npm:^2.3.0, @lumino/widgets@npm:^2.3.1":
+  version: 2.3.1
+  resolution: "@lumino/widgets@npm:2.3.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.1.3
+    "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
-    "@lumino/dragdrop": ^2.1.3
+    "@lumino/dragdrop": ^2.1.4
     "@lumino/keyboard": ^2.0.1
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-  checksum: a8559bd3574b7fc16e7679e05994c515b0d3e78dada35786d161f67c639941d134e92ce31d95c2e4ac06709cdf83b0e7fb4b6414a3f7779579222a2fb525d025
+  checksum: ba7b8f8839c1cd2a41dbda13281094eb6981a270cccf4f25a0cf83686dcc526a2d8044a20204317630bb7dd4a04d65361408c7623a921549c781afca84b91c67
   languageName: node
   linkType: hard
 
 "@nodelib/fs.scandir@npm:2.1.5":
   version: 2.1.5
   resolution: "@nodelib/fs.scandir@npm:2.1.5"
   dependencies:
@@ -2995,58 +3045,65 @@
 "@pkgjs/parseargs@npm:^0.11.0":
   version: 0.11.0
   resolution: "@pkgjs/parseargs@npm:0.11.0"
   checksum: 6ad6a00fc4f2f2cfc6bff76fb1d88b8ee20bc0601e18ebb01b6d4be583733a860239a521a7fbca73b612e66705078809483549d2b18f370eb346c5155c8e4a0f
   languageName: node
   linkType: hard
 
+"@pkgr/core@npm:^0.1.0":
+  version: 0.1.1
+  resolution: "@pkgr/core@npm:0.1.1"
+  checksum: 6f25fd2e3008f259c77207ac9915b02f1628420403b2630c92a07ff963129238c9262afc9e84344c7a23b5cc1f3965e2cd17e3798219f5fd78a63d144d3cceba
+  languageName: node
+  linkType: hard
+
 "@rjsf/core@npm:^5.1.0":
-  version: 5.13.3
-  resolution: "@rjsf/core@npm:5.13.3"
+  version: 5.16.1
+  resolution: "@rjsf/core@npm:5.16.1"
   dependencies:
     lodash: ^4.17.21
     lodash-es: ^4.17.21
-    markdown-to-jsx: ^7.3.2
-    nanoid: ^3.3.6
+    markdown-to-jsx: ^7.4.0
+    nanoid: ^3.3.7
     prop-types: ^15.8.1
   peerDependencies:
-    "@rjsf/utils": ^5.12.x
+    "@rjsf/utils": ^5.16.x
     react: ^16.14.0 || >=17
-  checksum: ba7c855d2985bad845e75aadd1d5f227dde8715f14f9d1f2111cc502717eead93bc3430662fd9b04489a130e4100dc43eeb73a9c7d1c028655436dd7ca67eb4f
+  checksum: 2f88dc6af9dda8ec5c8cbac63f3f9e776a11fe363ce938aa7b5c7a3baaa84a7a2f3796ebf55b361a8cb65267a1715ab880a4743636fb88e06b0240d07f0e4c7b
   languageName: node
   linkType: hard
 
 "@rjsf/utils@npm:^5.1.0":
-  version: 5.13.3
-  resolution: "@rjsf/utils@npm:5.13.3"
+  version: 5.16.1
+  resolution: "@rjsf/utils@npm:5.16.1"
   dependencies:
     json-schema-merge-allof: ^0.8.1
     jsonpointer: ^5.0.1
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
-  checksum: 7b2d3c7791a6f10b620f5cec9820994f6a2a728604848423c8d7534d762ff4f6ae64132077a7c9c99c7ec3c8166667fa911d3012c4971eea8387758233070ab1
+  checksum: 0c69527de4ab6f9d6ec4d1a5e05a31a0a38062d40abe2a2da7bc2324b20b08b0e90c188977ac4408f3b004c758c28097444746f3215e21e184c11cad7e9278c1
   languageName: node
   linkType: hard
 
 "@sinclair/typebox@npm:^0.27.8":
   version: 0.27.8
   resolution: "@sinclair/typebox@npm:0.27.8"
   checksum: 00bd7362a3439021aa1ea51b0e0d0a0e8ca1351a3d54c606b115fdcc49b51b16db6e5f43b4fe7a28c38688523e22a94d49dd31168868b655f0d4d50f032d07a1
   languageName: node
   linkType: hard
 
 "@sinonjs/commons@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "@sinonjs/commons@npm:3.0.0"
+  version: 3.0.1
+  resolution: "@sinonjs/commons@npm:3.0.1"
   dependencies:
     type-detect: 4.0.8
-  checksum: b4b5b73d4df4560fb8c0c7b38c7ad4aeabedd362f3373859d804c988c725889cde33550e4bcc7cd316a30f5152a2d1d43db71b6d0c38f5feef71fd8d016763f8
+  checksum: a7c3e7cc612352f4004873747d9d8b2d4d90b13a6d483f685598c945a70e734e255f1ca5dc49702515533c403b32725defff148177453b3f3915bcb60e9d4601
   languageName: node
   linkType: hard
 
 "@sinonjs/fake-timers@npm:^10.0.2":
   version: 10.3.0
   resolution: "@sinonjs/fake-timers@npm:10.3.0"
   dependencies:
@@ -3059,378 +3116,385 @@
   version: 2.0.0
   resolution: "@tootallnate/once@npm:2.0.0"
   checksum: ad87447820dd3f24825d2d947ebc03072b20a42bfc96cbafec16bff8bbda6c1a81fcb0be56d5b21968560c5359a0af4038a68ba150c3e1694fe4c109a063bed8
   languageName: node
   linkType: hard
 
 "@types/babel__core@npm:^7.1.14":
-  version: 7.20.3
-  resolution: "@types/babel__core@npm:7.20.3"
+  version: 7.20.5
+  resolution: "@types/babel__core@npm:7.20.5"
   dependencies:
     "@babel/parser": ^7.20.7
     "@babel/types": ^7.20.7
     "@types/babel__generator": "*"
     "@types/babel__template": "*"
     "@types/babel__traverse": "*"
-  checksum: 8d14acc14d99b4b8bf36c00da368f6d597bd9ae3344aa7048f83f0f701b0463fa7c7bf2e50c3e4382fdbcfd1e4187b3452a0f0888b0f3ae8fad975591f7bdb94
+  checksum: a3226f7930b635ee7a5e72c8d51a357e799d19cbf9d445710fa39ab13804f79ab1a54b72ea7d8e504659c7dfc50675db974b526142c754398d7413aa4bc30845
   languageName: node
   linkType: hard
 
 "@types/babel__generator@npm:*":
-  version: 7.6.6
-  resolution: "@types/babel__generator@npm:7.6.6"
+  version: 7.6.8
+  resolution: "@types/babel__generator@npm:7.6.8"
   dependencies:
     "@babel/types": ^7.0.0
-  checksum: 36e8838c7e16eff611447579e840526946a8b14c794c82486cee2a5ad2257aa6cad746d8ecff3144e3721178837d2c25d0a435d384391eb67846b933c062b075
+  checksum: 5b332ea336a2efffbdeedb92b6781949b73498606ddd4205462f7d96dafd45ff3618770b41de04c4881e333dd84388bfb8afbdf6f2764cbd98be550d85c6bb48
   languageName: node
   linkType: hard
 
 "@types/babel__template@npm:*":
-  version: 7.4.3
-  resolution: "@types/babel__template@npm:7.4.3"
+  version: 7.4.4
+  resolution: "@types/babel__template@npm:7.4.4"
   dependencies:
     "@babel/parser": ^7.1.0
     "@babel/types": ^7.0.0
-  checksum: 55deb814c94d1bfb78c4d1de1de1b73eb17c79374602f3bd8aa14e356a77fca64d01646cebe25ec9b307f53a047acc6d53ad6e931019d0726422f5f911e945aa
+  checksum: d7a02d2a9b67e822694d8e6a7ddb8f2b71a1d6962dfd266554d2513eefbb205b33ca71a0d163b1caea3981ccf849211f9964d8bd0727124d18ace45aa6c9ae29
   languageName: node
   linkType: hard
 
 "@types/babel__traverse@npm:*, @types/babel__traverse@npm:^7.0.6":
-  version: 7.20.3
-  resolution: "@types/babel__traverse@npm:7.20.3"
+  version: 7.20.5
+  resolution: "@types/babel__traverse@npm:7.20.5"
   dependencies:
     "@babel/types": ^7.20.7
-  checksum: 6d0f70d8972647c9b78b51a54f0b6481c4f23f0bb2699ad276e6070678bd121fede99e8e2c8c3e409d2f31a0bf83ae511abc6fefb91f0630c8d728a3a9136790
+  checksum: 608e0ab4fc31cd47011d98942e6241b34d461608c0c0e153377c5fd822c436c475f1ded76a56bfa76a1adf8d9266b727bbf9bfac90c4cb152c97f30dadc5b7e8
   languageName: node
   linkType: hard
 
-"@types/crypto-js@npm:^4.1.2":
-  version: 4.1.3
-  resolution: "@types/crypto-js@npm:4.1.3"
-  checksum: 4489854579c1b90b77da881fc980e3f05ab1e9c68b18ae580fedbb7b0fb40d531fda7bdc05f1b3bd5d4218c1d97c2f821bbac57eb3d7d9e505ce5a2c5b034166
+"@types/create-react-class@npm:*":
+  version: 15.6.7
+  resolution: "@types/create-react-class@npm:15.6.7"
+  dependencies:
+    "@types/react": "*"
+  checksum: 072c1fe0472217fe80b94965a8c23dd2f53b701c56bcf1e16da4d422aeb3fcba65972768f4b8ac90a5ca1ef8721730fb78fb8da080b9a8b004b6df667acc7ec7
   languageName: node
   linkType: hard
 
 "@types/eslint-scope@npm:^3.7.3":
-  version: 3.7.6
-  resolution: "@types/eslint-scope@npm:3.7.6"
+  version: 3.7.7
+  resolution: "@types/eslint-scope@npm:3.7.7"
   dependencies:
     "@types/eslint": "*"
     "@types/estree": "*"
-  checksum: a2339e312949ae7f96bca52cde89a3d2218d4505746a78a0ba1aa56573e43b3d52ce9662b86ab785663a62fa8f2bd2fb61b990398785b40f2efc91be3fd246f8
+  checksum: e2889a124aaab0b89af1bab5959847c5bec09809209255de0e63b9f54c629a94781daa04adb66bffcdd742f5e25a17614fb933965093c0eea64aacda4309380e
   languageName: node
   linkType: hard
 
 "@types/eslint@npm:*":
-  version: 8.44.6
-  resolution: "@types/eslint@npm:8.44.6"
+  version: 8.56.2
+  resolution: "@types/eslint@npm:8.56.2"
   dependencies:
     "@types/estree": "*"
     "@types/json-schema": "*"
-  checksum: ed8de582ab3dbd7ec0bf97d41f4f3de28dd8a37fc48bc423e1c406bbb70d1fd8c4175ba17ad6495ef9ef99a43df71421277b7a2a0355097489c4c4cf6bb266ff
+  checksum: 38e054971596f5c0413f66a62dc26b10e0a21ac46ceacb06fbf8cfb838d20820787209b17218b3916e4c23d990ff77cfdb482d655cac0e0d2b837d430fcc5db8
   languageName: node
   linkType: hard
 
-"@types/estree@npm:*, @types/estree@npm:^1.0.0":
-  version: 1.0.4
-  resolution: "@types/estree@npm:1.0.4"
-  checksum: dcd08e6e967def3afff745774b6b9b912d6394ddacbb3e8be05bb291c1803f5f03f1ab0eeb852bf8a85ca14842663f461f3dac82179dcdccbf45fbc067673bbc
+"@types/estree@npm:*, @types/estree@npm:^1.0.5":
+  version: 1.0.5
+  resolution: "@types/estree@npm:1.0.5"
+  checksum: dd8b5bed28e6213b7acd0fb665a84e693554d850b0df423ac8076cc3ad5823a6bc26b0251d080bdc545af83179ede51dd3f6fa78cad2c46ed1f29624ddf3e41a
   languageName: node
   linkType: hard
 
 "@types/graceful-fs@npm:^4.1.3":
-  version: 4.1.8
-  resolution: "@types/graceful-fs@npm:4.1.8"
+  version: 4.1.9
+  resolution: "@types/graceful-fs@npm:4.1.9"
   dependencies:
     "@types/node": "*"
-  checksum: 6e1ee9c119e075134696171b680fee7b627f3e077ec5e5ad9ba9359f1688a84fa35ea6804f96922c43ca30ab8d4ca9531a526b64f57fa13e1d721bf741884829
+  checksum: 79d746a8f053954bba36bd3d94a90c78de995d126289d656fb3271dd9f1229d33f678da04d10bce6be440494a5a73438e2e363e92802d16b8315b051036c5256
   languageName: node
   linkType: hard
 
 "@types/istanbul-lib-coverage@npm:*, @types/istanbul-lib-coverage@npm:^2.0.0, @types/istanbul-lib-coverage@npm:^2.0.1":
-  version: 2.0.5
-  resolution: "@types/istanbul-lib-coverage@npm:2.0.5"
-  checksum: 978eaf327f9a238eb1e2828b93b4b48e288ffb88c4be81330c74477ab8b93fac41a8784260d72bdd9995535d70608f738199b6364fd3344842e924a3ec3301e7
+  version: 2.0.6
+  resolution: "@types/istanbul-lib-coverage@npm:2.0.6"
+  checksum: 3feac423fd3e5449485afac999dcfcb3d44a37c830af898b689fadc65d26526460bedb889db278e0d4d815a670331796494d073a10ee6e3a6526301fe7415778
   languageName: node
   linkType: hard
 
 "@types/istanbul-lib-report@npm:*":
-  version: 3.0.2
-  resolution: "@types/istanbul-lib-report@npm:3.0.2"
+  version: 3.0.3
+  resolution: "@types/istanbul-lib-report@npm:3.0.3"
   dependencies:
     "@types/istanbul-lib-coverage": "*"
-  checksum: 549e44e14a4dc98164ce477ca8650d33898e5c74a6bb8079cbec7f811567dcb805a3bfdbf83ce53222eaecc37ae53aa7f25bda1a7d8347449155c8f0b4f30232
+  checksum: b91e9b60f865ff08cb35667a427b70f6c2c63e88105eadd29a112582942af47ed99c60610180aa8dcc22382fa405033f141c119c69b95db78c4c709fbadfeeb4
   languageName: node
   linkType: hard
 
 "@types/istanbul-reports@npm:^3.0.0":
-  version: 3.0.3
-  resolution: "@types/istanbul-reports@npm:3.0.3"
+  version: 3.0.4
+  resolution: "@types/istanbul-reports@npm:3.0.4"
   dependencies:
     "@types/istanbul-lib-report": "*"
-  checksum: 21d007be7dd09165ed24f5cc9947319ad435fc3b3e568f3eec0a42ee80fd2adccdeb929bc1311efb2cf7597835638cde865d3630d8b4c15d1390c9527bcad1a9
+  checksum: 93eb18835770b3431f68ae9ac1ca91741ab85f7606f310a34b3586b5a34450ec038c3eed7ab19266635499594de52ff73723a54a72a75b9f7d6a956f01edee95
   languageName: node
   linkType: hard
 
 "@types/jest@npm:^29.2.0":
-  version: 29.5.7
-  resolution: "@types/jest@npm:29.5.7"
+  version: 29.5.11
+  resolution: "@types/jest@npm:29.5.11"
   dependencies:
     expect: ^29.0.0
     pretty-format: ^29.0.0
-  checksum: e28624ccb0ef1255a03fbbb4b5bc3e5cbcdc450d39e0739985ff679b124198f808c38c8c3e67859c6efc0e848196deeb8cfed028e12a821c511dfc1112a2d6e9
+  checksum: f892a06ec9f0afa9a61cd7fa316ec614e21d4df1ad301b5a837787e046fcb40dfdf7f264a55e813ac6b9b633cb9d366bd5b8d1cea725e84102477b366df23fdd
   languageName: node
   linkType: hard
 
 "@types/jsdom@npm:^20.0.0":
   version: 20.0.1
   resolution: "@types/jsdom@npm:20.0.1"
   dependencies:
     "@types/node": "*"
     "@types/tough-cookie": "*"
     parse5: ^7.0.0
   checksum: d55402c5256ef451f93a6e3d3881f98339fe73a5ac2030588df056d6835df8367b5a857b48d27528289057e26dcdd3f502edc00cb877c79174cb3a4c7f2198c1
   languageName: node
   linkType: hard
 
-"@types/json-schema@npm:*, @types/json-schema@npm:^7.0.11, @types/json-schema@npm:^7.0.5, @types/json-schema@npm:^7.0.8, @types/json-schema@npm:^7.0.9":
-  version: 7.0.14
-  resolution: "@types/json-schema@npm:7.0.14"
-  checksum: 4b3dd99616c7c808201c56f6c7f6552eb67b5c0c753ab3fa03a6cb549aae950da537e9558e53fa65fba23d1be624a1e4e8d20c15027efbe41e03ca56f2b04fb0
+"@types/json-schema@npm:*, @types/json-schema@npm:^7.0.11, @types/json-schema@npm:^7.0.12, @types/json-schema@npm:^7.0.5, @types/json-schema@npm:^7.0.8, @types/json-schema@npm:^7.0.9":
+  version: 7.0.15
+  resolution: "@types/json-schema@npm:7.0.15"
+  checksum: 97ed0cb44d4070aecea772b7b2e2ed971e10c81ec87dd4ecc160322ffa55ff330dace1793489540e3e318d90942064bb697cc0f8989391797792d919737b3b98
   languageName: node
   linkType: hard
 
-"@types/minimist@npm:^1.2.0":
-  version: 1.2.4
-  resolution: "@types/minimist@npm:1.2.4"
-  checksum: d7912f9a466312cbc1333800272b9208178140ef4da2ccec3fa82231c8e67f57f84275b3c19109c4f68f1b7b057baeacc6b80af1de14b58b46e6b54233e44c6a
+"@types/minimist@npm:^1.2.2":
+  version: 1.2.5
+  resolution: "@types/minimist@npm:1.2.5"
+  checksum: 477047b606005058ab0263c4f58097136268007f320003c348794f74adedc3166ffc47c80ec3e94687787f2ab7f4e72c468223946e79892cf0fd9e25e9970a90
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 20.8.10
-  resolution: "@types/node@npm:20.8.10"
+  version: 20.11.7
+  resolution: "@types/node@npm:20.11.7"
   dependencies:
     undici-types: ~5.26.4
-  checksum: 7c61190e43e8074a1b571e52ff14c880bc67a0447f2fe5ed0e1a023eb8a23d5f815658edb98890f7578afe0f090433c4a635c7c87311762544e20dd78723e515
+  checksum: 61ea0718bccda31110c643190518407b7c50d26698a20e3522871608db5fa3d2d43d1ae57c609068eae6996d563db43326045a90f22a9aacc825e8d6c7aea2ce
   languageName: node
   linkType: hard
 
 "@types/normalize-package-data@npm:^2.4.0":
-  version: 2.4.3
-  resolution: "@types/normalize-package-data@npm:2.4.3"
-  checksum: 6f60e157c0fc39b80d80eb9043cdd78e4090f25c5264ef0317f5701648a5712fd453d364569675a19aef44a18c6f14f6e4809bdc0b97a46a0ed9ce4a320bbe42
+  version: 2.4.4
+  resolution: "@types/normalize-package-data@npm:2.4.4"
+  checksum: 65dff72b543997b7be8b0265eca7ace0e34b75c3e5fee31de11179d08fa7124a7a5587265d53d0409532ecb7f7fba662c2012807963e1f9b059653ec2c83ee05
   languageName: node
   linkType: hard
 
-"@types/parse-json@npm:^4.0.0":
-  version: 4.0.1
-  resolution: "@types/parse-json@npm:4.0.1"
-  checksum: 467c5fb95f4b03ea10fac007b4de7c9db103e8fce87b039ba5b37f17b374911833724624c311f3591435e4c42e376cab219400af1aef1dc314d5bd495d22fde7
+"@types/prop-types@npm:*":
+  version: 15.7.11
+  resolution: "@types/prop-types@npm:15.7.11"
+  checksum: 7519ff11d06fbf6b275029fe03fff9ec377b4cb6e864cac34d87d7146c7f5a7560fd164bdc1d2dbe00b60c43713631251af1fd3d34d46c69cd354602bc0c7c54
   languageName: node
   linkType: hard
 
-"@types/prop-types@npm:*":
-  version: 15.7.9
-  resolution: "@types/prop-types@npm:15.7.9"
-  checksum: c7591d3ff7593e243908a07e1d3e2bb6e8879008af5800d8378115a90d0fdf669a1cae72a6d7f69e59c4fa7bb4c8ed61f6ebc1c520fe110c6f2b03ac02414072
+"@types/react-addons-linked-state-mixin@npm:^0.14.22":
+  version: 0.14.27
+  resolution: "@types/react-addons-linked-state-mixin@npm:0.14.27"
+  dependencies:
+    "@types/create-react-class": "*"
+    "@types/react": "*"
+  checksum: a78007698a236335a50c74ddd27669028213ff363219f97a6ea1f000ddb8714c83838002ea07c33024f964112a229e447127b457fa3f9b3db352dd41d6b8d328
   languageName: node
   linkType: hard
 
-"@types/react@npm:^18.0.26":
-  version: 18.2.34
-  resolution: "@types/react@npm:18.2.34"
+"@types/react@npm:*, @types/react@npm:^18.0.26":
+  version: 18.2.48
+  resolution: "@types/react@npm:18.2.48"
   dependencies:
     "@types/prop-types": "*"
     "@types/scheduler": "*"
     csstype: ^3.0.2
-  checksum: 16446542228cba827143caf0ecb4718cbf02ae5befd4a6bc6d67ed144fe1c0cb4b06b20facf3d2b972d86c67a17cc82f5ec8a03fce42d50e12b2dcd0592fc66e
+  checksum: c9ca43ed2995389b7e09492c24e6f911a8439bb8276dd17cc66a2fbebbf0b42daf7b2ad177043256533607c2ca644d7d928fdfce37a67af1f8646d2bac988900
   languageName: node
   linkType: hard
 
 "@types/scheduler@npm:*":
-  version: 0.16.5
-  resolution: "@types/scheduler@npm:0.16.5"
-  checksum: 5aae67331bb7877edc65f77f205fb03c3808d9e51c186afe26945ce69f4072886629580a751e9ce8573e4a7538d0dfa1e4ce388c7c451fa689a4c592fdf1ea45
+  version: 0.16.8
+  resolution: "@types/scheduler@npm:0.16.8"
+  checksum: 6c091b096daa490093bf30dd7947cd28e5b2cd612ec93448432b33f724b162587fed9309a0acc104d97b69b1d49a0f3fc755a62282054d62975d53d7fd13472d
   languageName: node
   linkType: hard
 
-"@types/semver@npm:^7.3.12":
-  version: 7.5.4
-  resolution: "@types/semver@npm:7.5.4"
-  checksum: 120c0189f6fec5f2d12d0d71ac8a4cfa952dc17fa3d842e8afddb82bba8828a4052f8799c1653e2b47ae1977435f38e8985658fde971905ce5afb8e23ee97ecf
+"@types/semver@npm:^7.5.0":
+  version: 7.5.6
+  resolution: "@types/semver@npm:7.5.6"
+  checksum: 563a0120ec0efcc326567db2ed920d5d98346f3638b6324ea6b50222b96f02a8add3c51a916b6897b51523aad8ac227d21d3dcf8913559f1bfc6c15b14d23037
   languageName: node
   linkType: hard
 
 "@types/source-list-map@npm:*":
-  version: 0.1.4
-  resolution: "@types/source-list-map@npm:0.1.4"
-  checksum: c18896ead356c77aa7a5bb6bd0ad72a5e8dea4c7ec1e5162c3f4d7e5afa6f547ace66ce506c47d1726adb34aee9758f9367b35ddd03126f3c9d4bde4700cddf4
+  version: 0.1.6
+  resolution: "@types/source-list-map@npm:0.1.6"
+  checksum: 9cd294c121f1562062de5d241fe4d10780b1131b01c57434845fe50968e9dcf67ede444591c2b1ad6d3f9b6bc646ac02cc8f51a3577c795f9c64cf4573dcc6b1
   languageName: node
   linkType: hard
 
 "@types/stack-utils@npm:^2.0.0":
-  version: 2.0.2
-  resolution: "@types/stack-utils@npm:2.0.2"
-  checksum: 777cc7ac0c1000c5a07561013bcf7bd8477a3d55f55f376ee2f0c586331f7b999f57788140cfbdb65f6d7d97c0c41fe8fe6c778fd3ed71859c9b681ea76fc621
+  version: 2.0.3
+  resolution: "@types/stack-utils@npm:2.0.3"
+  checksum: 72576cc1522090fe497337c2b99d9838e320659ac57fa5560fcbdcbafcf5d0216c6b3a0a8a4ee4fdb3b1f5e3420aa4f6223ab57b82fef3578bec3206425c6cf5
   languageName: node
   linkType: hard
 
 "@types/tough-cookie@npm:*":
-  version: 4.0.4
-  resolution: "@types/tough-cookie@npm:4.0.4"
-  checksum: 6be275b09f5fbf33f359fd6d5372c69357cf96dea5d7ba7a6563c76c6cce8b0c7f81caa4805810b0e67427cad381aeef00d8c060d614fee79ca245c2b9887c3a
+  version: 4.0.5
+  resolution: "@types/tough-cookie@npm:4.0.5"
+  checksum: f19409d0190b179331586365912920d192733112a195e870c7f18d20ac8adb7ad0b0ff69dad430dba8bc2be09593453a719cfea92dc3bda19748fd158fe1498d
   languageName: node
   linkType: hard
 
 "@types/webpack-sources@npm:^0.1.5":
-  version: 0.1.11
-  resolution: "@types/webpack-sources@npm:0.1.11"
+  version: 0.1.12
+  resolution: "@types/webpack-sources@npm:0.1.12"
   dependencies:
     "@types/node": "*"
     "@types/source-list-map": "*"
     source-map: ^0.6.1
-  checksum: da64fc4b7d774dca57a0b40c20641fd387bc6c02ed3245dfd62af75a9ab0c3bb752773e6c2a023e35ce151563302af4d427ee4e81698ec3f3a7ed9f81f3390f4
+  checksum: 75342659a9889478969f7bb7360b998aa084ba11ab523c172ded6a807dac43ab2a9e1212078ef8bbf0f33e4fadd2c8a91b75d38184d8030d96a32fe819c9bb57
   languageName: node
   linkType: hard
 
 "@types/yargs-parser@npm:*":
-  version: 21.0.2
-  resolution: "@types/yargs-parser@npm:21.0.2"
-  checksum: e979051aac91d778fdb3953aced8cf039d954c3936b910b57735b7b52a413d065e6b2aea1cb2c583f6c23296a6f8543d2541879d798f0afedd7409a562b7bdeb
+  version: 21.0.3
+  resolution: "@types/yargs-parser@npm:21.0.3"
+  checksum: ef236c27f9432983e91432d974243e6c4cdae227cb673740320eff32d04d853eed59c92ca6f1142a335cfdc0e17cccafa62e95886a8154ca8891cc2dec4ee6fc
   languageName: node
   linkType: hard
 
 "@types/yargs@npm:^17.0.8":
-  version: 17.0.29
-  resolution: "@types/yargs@npm:17.0.29"
+  version: 17.0.32
+  resolution: "@types/yargs@npm:17.0.32"
   dependencies:
     "@types/yargs-parser": "*"
-  checksum: 8bbc0edd573a5a084cb13a9985c124490fd74e73b1ed8a3058861c13124e103b00a19770dc55c53215653a7845d7033e0695917b75153cfe9618d5b2fd3cf86e
+  checksum: 4505bdebe8716ff383640c6e928f855b5d337cb3c68c81f7249fc6b983d0aa48de3eee26062b84f37e0d75a5797bc745e0c6e76f42f81771252a758c638f36ba
   languageName: node
   linkType: hard
 
-"@typescript-eslint/eslint-plugin@npm:^5.55.0":
-  version: 5.62.0
-  resolution: "@typescript-eslint/eslint-plugin@npm:5.62.0"
+"@typescript-eslint/eslint-plugin@npm:^6.1.0":
+  version: 6.19.1
+  resolution: "@typescript-eslint/eslint-plugin@npm:6.19.1"
   dependencies:
-    "@eslint-community/regexpp": ^4.4.0
-    "@typescript-eslint/scope-manager": 5.62.0
-    "@typescript-eslint/type-utils": 5.62.0
-    "@typescript-eslint/utils": 5.62.0
+    "@eslint-community/regexpp": ^4.5.1
+    "@typescript-eslint/scope-manager": 6.19.1
+    "@typescript-eslint/type-utils": 6.19.1
+    "@typescript-eslint/utils": 6.19.1
+    "@typescript-eslint/visitor-keys": 6.19.1
     debug: ^4.3.4
     graphemer: ^1.4.0
-    ignore: ^5.2.0
-    natural-compare-lite: ^1.4.0
-    semver: ^7.3.7
-    tsutils: ^3.21.0
+    ignore: ^5.2.4
+    natural-compare: ^1.4.0
+    semver: ^7.5.4
+    ts-api-utils: ^1.0.1
   peerDependencies:
-    "@typescript-eslint/parser": ^5.0.0
-    eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
+    "@typescript-eslint/parser": ^6.0.0 || ^6.0.0-alpha
+    eslint: ^7.0.0 || ^8.0.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: fc104b389c768f9fa7d45a48c86d5c1ad522c1d0512943e782a56b1e3096b2cbcc1eea3fcc590647bf0658eef61aac35120a9c6daf979bf629ad2956deb516a1
+  checksum: ad04000cd6c15d864ff92655baa3aec99bb0ccf4714fedd145fedde60a27590a5feafe480beb2f0f3864b416098bde1e9431bada7480eb7ca4efad891e1d2f6f
   languageName: node
   linkType: hard
 
-"@typescript-eslint/parser@npm:^5.55.0":
-  version: 5.62.0
-  resolution: "@typescript-eslint/parser@npm:5.62.0"
+"@typescript-eslint/parser@npm:^6.1.0":
+  version: 6.19.1
+  resolution: "@typescript-eslint/parser@npm:6.19.1"
   dependencies:
-    "@typescript-eslint/scope-manager": 5.62.0
-    "@typescript-eslint/types": 5.62.0
-    "@typescript-eslint/typescript-estree": 5.62.0
+    "@typescript-eslint/scope-manager": 6.19.1
+    "@typescript-eslint/types": 6.19.1
+    "@typescript-eslint/typescript-estree": 6.19.1
+    "@typescript-eslint/visitor-keys": 6.19.1
     debug: ^4.3.4
   peerDependencies:
-    eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
+    eslint: ^7.0.0 || ^8.0.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: d168f4c7f21a7a63f47002e2d319bcbb6173597af5c60c1cf2de046b46c76b4930a093619e69faf2d30214c29ab27b54dcf1efc7046a6a6bd6f37f59a990e752
+  checksum: cd29619da08a2d9b7123ba4d8240989c747f8e0d5672179d8b147e413ee1334d1fa48570b0c37cf0ae4e26a275fd2d268cbe702c6fed639d3331abbb3292570a
   languageName: node
   linkType: hard
 
-"@typescript-eslint/scope-manager@npm:5.62.0":
-  version: 5.62.0
-  resolution: "@typescript-eslint/scope-manager@npm:5.62.0"
+"@typescript-eslint/scope-manager@npm:6.19.1":
+  version: 6.19.1
+  resolution: "@typescript-eslint/scope-manager@npm:6.19.1"
   dependencies:
-    "@typescript-eslint/types": 5.62.0
-    "@typescript-eslint/visitor-keys": 5.62.0
-  checksum: 6062d6b797fe1ce4d275bb0d17204c827494af59b5eaf09d8a78cdd39dadddb31074dded4297aaf5d0f839016d601032857698b0e4516c86a41207de606e9573
+    "@typescript-eslint/types": 6.19.1
+    "@typescript-eslint/visitor-keys": 6.19.1
+  checksum: 848cdebc16a3803e8a6d6035a7067605309a652bb2425f475f755b5ace4d80d2c17c8c8901f0f4759556da8d0a5b71024d472b85c3f3c70d0e6dcfe2a972ef35
   languageName: node
   linkType: hard
 
-"@typescript-eslint/type-utils@npm:5.62.0":
-  version: 5.62.0
-  resolution: "@typescript-eslint/type-utils@npm:5.62.0"
+"@typescript-eslint/type-utils@npm:6.19.1":
+  version: 6.19.1
+  resolution: "@typescript-eslint/type-utils@npm:6.19.1"
   dependencies:
-    "@typescript-eslint/typescript-estree": 5.62.0
-    "@typescript-eslint/utils": 5.62.0
+    "@typescript-eslint/typescript-estree": 6.19.1
+    "@typescript-eslint/utils": 6.19.1
     debug: ^4.3.4
-    tsutils: ^3.21.0
+    ts-api-utils: ^1.0.1
   peerDependencies:
-    eslint: "*"
+    eslint: ^7.0.0 || ^8.0.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: fc41eece5f315dfda14320be0da78d3a971d650ea41300be7196934b9715f3fe1120a80207551eb71d39568275dbbcf359bde540d1ca1439d8be15e9885d2739
+  checksum: eab1a30f8d85f7c6e2545de5963fbec2f3bb91913d59623069b4b0db372a671ab048c7018376fc853c3af06ea39417f3e7b27dd665027dd812347a5e64cecd77
   languageName: node
   linkType: hard
 
-"@typescript-eslint/types@npm:5.62.0":
-  version: 5.62.0
-  resolution: "@typescript-eslint/types@npm:5.62.0"
-  checksum: 48c87117383d1864766486f24de34086155532b070f6264e09d0e6139449270f8a9559cfef3c56d16e3bcfb52d83d42105d61b36743626399c7c2b5e0ac3b670
+"@typescript-eslint/types@npm:6.19.1":
+  version: 6.19.1
+  resolution: "@typescript-eslint/types@npm:6.19.1"
+  checksum: 598ce222b59c20432d06f60703d0c2dd16d9b2151569c192852136c57b8188e3ef6ef9fddaa2c136c9a756fcc7d873c0e29ec41cfd340564842287ef7b4571cd
   languageName: node
   linkType: hard
 
-"@typescript-eslint/typescript-estree@npm:5.62.0":
-  version: 5.62.0
-  resolution: "@typescript-eslint/typescript-estree@npm:5.62.0"
+"@typescript-eslint/typescript-estree@npm:6.19.1":
+  version: 6.19.1
+  resolution: "@typescript-eslint/typescript-estree@npm:6.19.1"
   dependencies:
-    "@typescript-eslint/types": 5.62.0
-    "@typescript-eslint/visitor-keys": 5.62.0
+    "@typescript-eslint/types": 6.19.1
+    "@typescript-eslint/visitor-keys": 6.19.1
     debug: ^4.3.4
     globby: ^11.1.0
     is-glob: ^4.0.3
-    semver: ^7.3.7
-    tsutils: ^3.21.0
+    minimatch: 9.0.3
+    semver: ^7.5.4
+    ts-api-utils: ^1.0.1
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: 3624520abb5807ed8f57b1197e61c7b1ed770c56dfcaca66372d584ff50175225798bccb701f7ef129d62c5989070e1ee3a0aa2d84e56d9524dcf011a2bb1a52
+  checksum: fb71a14aeee0468780219c5b8d39075f85d360b04ccd0ee88f4f0a615d2c232a6d3016e36d8c6eda2d9dfda86b4f4cc2c3d7582940fb29d33c7cf305e124d4e2
   languageName: node
   linkType: hard
 
-"@typescript-eslint/utils@npm:5.62.0":
-  version: 5.62.0
-  resolution: "@typescript-eslint/utils@npm:5.62.0"
+"@typescript-eslint/utils@npm:6.19.1":
+  version: 6.19.1
+  resolution: "@typescript-eslint/utils@npm:6.19.1"
   dependencies:
-    "@eslint-community/eslint-utils": ^4.2.0
-    "@types/json-schema": ^7.0.9
-    "@types/semver": ^7.3.12
-    "@typescript-eslint/scope-manager": 5.62.0
-    "@typescript-eslint/types": 5.62.0
-    "@typescript-eslint/typescript-estree": 5.62.0
-    eslint-scope: ^5.1.1
-    semver: ^7.3.7
+    "@eslint-community/eslint-utils": ^4.4.0
+    "@types/json-schema": ^7.0.12
+    "@types/semver": ^7.5.0
+    "@typescript-eslint/scope-manager": 6.19.1
+    "@typescript-eslint/types": 6.19.1
+    "@typescript-eslint/typescript-estree": 6.19.1
+    semver: ^7.5.4
   peerDependencies:
-    eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
-  checksum: ee9398c8c5db6d1da09463ca7bf36ed134361e20131ea354b2da16a5fdb6df9ba70c62a388d19f6eebb421af1786dbbd79ba95ddd6ab287324fc171c3e28d931
+    eslint: ^7.0.0 || ^8.0.0
+  checksum: fe72e75c3ea17a85772b83f148555ea94ff5d55d13586f3fc038833197a74f8071e14c2bbf1781c40eec20005f052f4be2513a725eea82a15da3cb9af3046c70
   languageName: node
   linkType: hard
 
-"@typescript-eslint/visitor-keys@npm:5.62.0":
-  version: 5.62.0
-  resolution: "@typescript-eslint/visitor-keys@npm:5.62.0"
+"@typescript-eslint/visitor-keys@npm:6.19.1":
+  version: 6.19.1
+  resolution: "@typescript-eslint/visitor-keys@npm:6.19.1"
   dependencies:
-    "@typescript-eslint/types": 5.62.0
-    eslint-visitor-keys: ^3.3.0
-  checksum: 976b05d103fe8335bef5c93ad3f76d781e3ce50329c0243ee0f00c0fcfb186c81df50e64bfdd34970148113f8ade90887f53e3c4938183afba830b4ba8e30a35
+    "@typescript-eslint/types": 6.19.1
+    eslint-visitor-keys: ^3.4.1
+  checksum: bdf057a42e776970a89cdd568e493e3ea7ec085544d8f318d33084da63c3395ad2c0fb9cef9f61ceeca41f5dab54ab064b7078fe596889005e412ec74d2d1ae4
   languageName: node
   linkType: hard
 
 "@ungap/structured-clone@npm:^1.2.0":
   version: 1.2.0
   resolution: "@ungap/structured-clone@npm:1.2.0"
   checksum: 4f656b7b4672f2ce6e272f2427d8b0824ed11546a601d8d5412b9d7704e83db38a8d9f402ecdf2b9063fc164af842ad0ec4a55819f621ed7e7ea4d1efcc74524
@@ -3674,26 +3738,26 @@
   peerDependencies:
     acorn: ^6.0.0 || ^7.0.0 || ^8.0.0
   checksum: c3d3b2a89c9a056b205b69530a37b972b404ee46ec8e5b341666f9513d3163e2a4f214a71f4dfc7370f5a9c07472d2fd1c11c91c3f03d093e37637d95da98950
   languageName: node
   linkType: hard
 
 "acorn-walk@npm:^8.0.2":
-  version: 8.3.0
-  resolution: "acorn-walk@npm:8.3.0"
-  checksum: 15ea56ab6529135be05e7d018f935ca80a572355dd3f6d3cd717e36df3346e0f635a93ae781b1c7942607693e2e5f3ef81af5c6fc697bbadcc377ebda7b7f5f6
+  version: 8.3.2
+  resolution: "acorn-walk@npm:8.3.2"
+  checksum: 3626b9d26a37b1b427796feaa5261faf712307a8920392c8dce9a5739fb31077667f4ad2ec71c7ac6aaf9f61f04a9d3d67ff56f459587206fc04aa31c27ef392
   languageName: node
   linkType: hard
 
 "acorn@npm:^8.1.0, acorn@npm:^8.7.1, acorn@npm:^8.8.1, acorn@npm:^8.8.2, acorn@npm:^8.9.0":
-  version: 8.11.2
-  resolution: "acorn@npm:8.11.2"
+  version: 8.11.3
+  resolution: "acorn@npm:8.11.3"
   bin:
     acorn: bin/acorn
-  checksum: 818450408684da89423e3daae24e4dc9b68692db8ab49ea4569c7c5abb7a3f23669438bf129cc81dfdada95e1c9b944ee1bfca2c57a05a4dc73834a612fbf6a7
+  checksum: 76d8e7d559512566b43ab4aadc374f11f563f0a9e21626dd59cb2888444e9445923ae9f3699972767f18af61df89cd89f5eaaf772d1327b055b45cb829b4a88c
   languageName: node
   linkType: hard
 
 "agent-base@npm:6":
   version: 6.0.2
   resolution: "agent-base@npm:6.0.2"
   dependencies:
@@ -3958,47 +4022,47 @@
     "@babel/types": ^7.3.3
     "@types/babel__core": ^7.1.14
     "@types/babel__traverse": ^7.0.6
   checksum: 51250f22815a7318f17214a9d44650ba89551e6d4f47a2dc259128428324b52f5a73979d010cefd921fd5a720d8c1d55ad74ff601cd94c7bd44d5f6292fde2d1
   languageName: node
   linkType: hard
 
-"babel-plugin-polyfill-corejs2@npm:^0.4.6":
-  version: 0.4.6
-  resolution: "babel-plugin-polyfill-corejs2@npm:0.4.6"
+"babel-plugin-polyfill-corejs2@npm:^0.4.8":
+  version: 0.4.8
+  resolution: "babel-plugin-polyfill-corejs2@npm:0.4.8"
   dependencies:
     "@babel/compat-data": ^7.22.6
-    "@babel/helper-define-polyfill-provider": ^0.4.3
+    "@babel/helper-define-polyfill-provider": ^0.5.0
     semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
-  checksum: 08896811df31530be6a9bcdd630cb9fd4b5ae5181039d18db3796efbc54e38d57a42af460845c10a04434e1bc45c0d47743c7e6c860383cc6b141083cde22030
+  checksum: 22857b87268b354e095452199464accba5fd8f690558a2f24b0954807ca2494b96da8d5c13507955802427582015160bce26a66893acf6da5dafbed8b336cf79
   languageName: node
   linkType: hard
 
-"babel-plugin-polyfill-corejs3@npm:^0.8.5":
-  version: 0.8.6
-  resolution: "babel-plugin-polyfill-corejs3@npm:0.8.6"
+"babel-plugin-polyfill-corejs3@npm:^0.9.0":
+  version: 0.9.0
+  resolution: "babel-plugin-polyfill-corejs3@npm:0.9.0"
   dependencies:
-    "@babel/helper-define-polyfill-provider": ^0.4.3
-    core-js-compat: ^3.33.1
+    "@babel/helper-define-polyfill-provider": ^0.5.0
+    core-js-compat: ^3.34.0
   peerDependencies:
     "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
-  checksum: 36951c2edac42ac0f05b200502e90d77bf66ccee5b52e2937d23496c6ef2372cce31b8c64144da374b77bd3eb65e2721703a52eac56cad16a152326c092cbf77
+  checksum: 65bbf59fc0145c7a264822777403632008dce00015b4b5c7ec359125ef4faf9e8f494ae5123d2992104feb6f19a3cff85631992862e48b6d7bd64eb7e755ee1f
   languageName: node
   linkType: hard
 
-"babel-plugin-polyfill-regenerator@npm:^0.5.3":
-  version: 0.5.3
-  resolution: "babel-plugin-polyfill-regenerator@npm:0.5.3"
+"babel-plugin-polyfill-regenerator@npm:^0.5.5":
+  version: 0.5.5
+  resolution: "babel-plugin-polyfill-regenerator@npm:0.5.5"
   dependencies:
-    "@babel/helper-define-polyfill-provider": ^0.4.3
+    "@babel/helper-define-polyfill-provider": ^0.5.0
   peerDependencies:
     "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
-  checksum: 2bb546582cda1870d19e646a7183baeb2cccd56e0ef3e4eaeabd28e120daf17cb87399194a9ccdcf32506bcaa68d23e73440fc8ab990a7a0f8c5a77c12d5d4bc
+  checksum: 3a9b4828673b23cd648dcfb571eadcd9d3fadfca0361d0a7c6feeb5a30474e92faaa49f067a6e1c05e49b6a09812879992028ff3ef3446229ff132d6e1de7eb6
   languageName: node
   linkType: hard
 
 "babel-preset-current-node-syntax@npm:^1.0.0":
   version: 1.0.1
   resolution: "babel-preset-current-node-syntax@npm:1.0.1"
   dependencies:
@@ -4077,25 +4141,25 @@
   resolution: "braces@npm:3.0.2"
   dependencies:
     fill-range: ^7.0.1
   checksum: e2a8e769a863f3d4ee887b5fe21f63193a891c68b612ddb4b68d82d1b5f3ff9073af066c343e9867a393fe4c2555dcb33e89b937195feb9c1613d259edfcd459
   languageName: node
   linkType: hard
 
-"browserslist@npm:^4.14.5, browserslist@npm:^4.21.9, browserslist@npm:^4.22.1":
-  version: 4.22.1
-  resolution: "browserslist@npm:4.22.1"
-  dependencies:
-    caniuse-lite: ^1.0.30001541
-    electron-to-chromium: ^1.4.535
-    node-releases: ^2.0.13
+"browserslist@npm:^4.21.10, browserslist@npm:^4.22.2":
+  version: 4.22.2
+  resolution: "browserslist@npm:4.22.2"
+  dependencies:
+    caniuse-lite: ^1.0.30001565
+    electron-to-chromium: ^1.4.601
+    node-releases: ^2.0.14
     update-browserslist-db: ^1.0.13
   bin:
     browserslist: cli.js
-  checksum: 7e6b10c53f7dd5d83fd2b95b00518889096382539fed6403829d447e05df4744088de46a571071afb447046abc3c66ad06fbc790e70234ec2517452e32ffd862
+  checksum: 33ddfcd9145220099a7a1ac533cecfe5b7548ffeb29b313e1b57be6459000a1f8fa67e781cf4abee97268ac594d44134fcc4a6b2b4750ceddc9796e3a22076d9
   languageName: node
   linkType: hard
 
 "bs-logger@npm:0.x":
   version: 0.2.6
   resolution: "bs-logger@npm:0.2.6"
   dependencies:
@@ -4117,30 +4181,30 @@
   version: 1.1.2
   resolution: "buffer-from@npm:1.1.2"
   checksum: 0448524a562b37d4d7ed9efd91685a5b77a50672c556ea254ac9a6d30e3403a517d8981f10e565db24e8339413b43c97ca2951f10e399c6125a0d8911f5679bb
   languageName: node
   linkType: hard
 
 "cacache@npm:^18.0.0":
-  version: 18.0.0
-  resolution: "cacache@npm:18.0.0"
+  version: 18.0.2
+  resolution: "cacache@npm:18.0.2"
   dependencies:
     "@npmcli/fs": ^3.1.0
     fs-minipass: ^3.0.0
     glob: ^10.2.2
     lru-cache: ^10.0.1
     minipass: ^7.0.3
-    minipass-collect: ^1.0.2
+    minipass-collect: ^2.0.1
     minipass-flush: ^1.0.5
     minipass-pipeline: ^1.2.4
     p-map: ^4.0.0
     ssri: ^10.0.0
     tar: ^6.1.11
     unique-filename: ^3.0.0
-  checksum: 2cd6bf15551abd4165acb3a4d1ef0593b3aa2fd6853ae16b5bb62199c2faecf27d36555a9545c0e07dd03347ec052e782923bdcece724a24611986aafb53e152
+  checksum: 0250df80e1ad0c828c956744850c5f742c24244e9deb5b7dc81bca90f8c10e011e132ecc58b64497cc1cad9a98968676147fb6575f4f94722f7619757b17a11b
   languageName: node
   linkType: hard
 
 "call-bind@npm:^1.0.0, call-bind@npm:^1.0.2, call-bind@npm:^1.0.4, call-bind@npm:^1.0.5":
   version: 1.0.5
   resolution: "call-bind@npm:1.0.5"
   dependencies:
@@ -4154,43 +4218,44 @@
 "callsites@npm:^3.0.0":
   version: 3.1.0
   resolution: "callsites@npm:3.1.0"
   checksum: 072d17b6abb459c2ba96598918b55868af677154bec7e73d222ef95a8fdb9bbf7dae96a8421085cdad8cd190d86653b5b6dc55a4484f2e5b2e27d5e0c3fc15b3
   languageName: node
   linkType: hard
 
-"camelcase-keys@npm:^6.2.2":
-  version: 6.2.2
-  resolution: "camelcase-keys@npm:6.2.2"
+"camelcase-keys@npm:^7.0.0":
+  version: 7.0.2
+  resolution: "camelcase-keys@npm:7.0.2"
   dependencies:
-    camelcase: ^5.3.1
-    map-obj: ^4.0.0
-    quick-lru: ^4.0.1
-  checksum: 43c9af1adf840471e54c68ab3e5fe8a62719a6b7dbf4e2e86886b7b0ff96112c945736342b837bd2529ec9d1c7d1934e5653318478d98e0cf22c475c04658e2a
+    camelcase: ^6.3.0
+    map-obj: ^4.1.0
+    quick-lru: ^5.1.1
+    type-fest: ^1.2.1
+  checksum: b5821cc48dd00e8398a30c5d6547f06837ab44de123f1b3a603d0a03399722b2fc67a485a7e47106eb02ef543c3b50c5ebaabc1242cde4b63a267c3258d2365b
   languageName: node
   linkType: hard
 
 "camelcase@npm:^5.3.1":
   version: 5.3.1
   resolution: "camelcase@npm:5.3.1"
   checksum: e6effce26b9404e3c0f301498184f243811c30dfe6d0b9051863bd8e4034d09c8c2923794f280d6827e5aa055f6c434115ff97864a16a963366fb35fd673024b
   languageName: node
   linkType: hard
 
-"camelcase@npm:^6.2.0":
+"camelcase@npm:^6.2.0, camelcase@npm:^6.3.0":
   version: 6.3.0
   resolution: "camelcase@npm:6.3.0"
   checksum: 8c96818a9076434998511251dcb2761a94817ea17dbdc37f47ac080bd088fc62c7369429a19e2178b993497132c8cbcf5cc1f44ba963e76782ba469c0474938d
   languageName: node
   linkType: hard
 
-"caniuse-lite@npm:^1.0.30001541":
-  version: 1.0.30001559
-  resolution: "caniuse-lite@npm:1.0.30001559"
-  checksum: 17c7af10244dca2c7ca41c884df19fc4c7313b9b03ed1f9b1f352bffbc871701f35431f766838f669ebe1f9d20627c0c6f2d760a0837538bd1d21de5833020f4
+"caniuse-lite@npm:^1.0.30001565":
+  version: 1.0.30001580
+  resolution: "caniuse-lite@npm:1.0.30001580"
+  checksum: 8d287d1e2a64348365f55562457b52afc8c5e0e8ddf040e18e53395ca165241a697205611dc209dace5c7f7d1d3ee8d566672cce6f9668d658d7930b7a200875
   languageName: node
   linkType: hard
 
 "chalk@npm:^2.3.0, chalk@npm:^2.4.1, chalk@npm:^2.4.2":
   version: 2.4.2
   resolution: "chalk@npm:2.4.2"
   dependencies:
@@ -4405,33 +4470,37 @@
 "convert-source-map@npm:^2.0.0":
   version: 2.0.0
   resolution: "convert-source-map@npm:2.0.0"
   checksum: 63ae9933be5a2b8d4509daca5124e20c14d023c820258e484e32dc324d34c2754e71297c94a05784064ad27615037ef677e3f0c00469fb55f409d2bb21261035
   languageName: node
   linkType: hard
 
-"core-js-compat@npm:^3.31.0, core-js-compat@npm:^3.33.1":
-  version: 3.33.2
-  resolution: "core-js-compat@npm:3.33.2"
+"core-js-compat@npm:^3.31.0, core-js-compat@npm:^3.34.0":
+  version: 3.35.1
+  resolution: "core-js-compat@npm:3.35.1"
   dependencies:
-    browserslist: ^4.22.1
-  checksum: 4206d3ff282a9188399e9003301fa4b96844152afcea7b9c9accc653542f40f581f77bf079b8be67f614e305da1f29e868a49ceebb6dbe3f5fb4a28bd2dbf431
+    browserslist: ^4.22.2
+  checksum: 4c1a7076d31fa489eec5c46eb11c7127703f9756b5fed1eab9bf27b7f0f151247886d3fa488911078bd2801a5dfa12a9ea2ecb7a4e61dfa460b2c291805f503b
   languageName: node
   linkType: hard
 
-"cosmiconfig@npm:^7.1.0":
-  version: 7.1.0
-  resolution: "cosmiconfig@npm:7.1.0"
+"cosmiconfig@npm:^8.2.0":
+  version: 8.3.6
+  resolution: "cosmiconfig@npm:8.3.6"
   dependencies:
-    "@types/parse-json": ^4.0.0
-    import-fresh: ^3.2.1
-    parse-json: ^5.0.0
+    import-fresh: ^3.3.0
+    js-yaml: ^4.1.0
+    parse-json: ^5.2.0
     path-type: ^4.0.0
-    yaml: ^1.10.0
-  checksum: c53bf7befc1591b2651a22414a5e786cd5f2eeaa87f3678a3d49d6069835a9d8d1aef223728e98aa8fec9a95bf831120d245096db12abe019fecb51f5696c96f
+  peerDependencies:
+    typescript: ">=4.9.5"
+  peerDependenciesMeta:
+    typescript:
+      optional: true
+  checksum: dc339ebea427898c9e03bf01b56ba7afbac07fc7d2a2d5a15d6e9c14de98275a9565da949375aee1809591c152c0a3877bb86dbeaf74d5bd5aaa79955ad9e7a0
   languageName: node
   linkType: hard
 
 "create-jest@npm:^29.7.0":
   version: 29.7.0
   resolution: "create-jest@npm:29.7.0"
   dependencies:
@@ -4475,36 +4544,46 @@
     path-key: ^3.1.0
     shebang-command: ^2.0.0
     which: ^2.0.1
   checksum: 671cc7c7288c3a8406f3c69a3ae2fc85555c04169e9d611def9a675635472614f1c0ed0ef80955d5b6d4e724f6ced67f0ad1bb006c2ea643488fcfef994d7f52
   languageName: node
   linkType: hard
 
-"css-functions-list@npm:^3.1.0":
+"css-functions-list@npm:^3.2.1":
   version: 3.2.1
   resolution: "css-functions-list@npm:3.2.1"
   checksum: 57d7deb3b05e84d95b88ba9b3244cf60d33b40652b3357f084c805b24a9febda5987ade44ef25a56be41e73249a7dcc157abd704d8a0e998b2c1c2e2d5de6461
   languageName: node
   linkType: hard
 
 "css-loader@npm:^6.7.1":
-  version: 6.8.1
-  resolution: "css-loader@npm:6.8.1"
+  version: 6.9.1
+  resolution: "css-loader@npm:6.9.1"
   dependencies:
     icss-utils: ^5.1.0
-    postcss: ^8.4.21
+    postcss: ^8.4.33
     postcss-modules-extract-imports: ^3.0.0
-    postcss-modules-local-by-default: ^4.0.3
-    postcss-modules-scope: ^3.0.0
+    postcss-modules-local-by-default: ^4.0.4
+    postcss-modules-scope: ^3.1.1
     postcss-modules-values: ^4.0.0
     postcss-value-parser: ^4.2.0
-    semver: ^7.3.8
+    semver: ^7.5.4
   peerDependencies:
     webpack: ^5.0.0
-  checksum: 7c1784247bdbe76dc5c55fb1ac84f1d4177a74c47259942c9cfdb7a8e6baef11967a0bc85ac285f26bd26d5059decb848af8154a03fdb4f4894f41212f45eef3
+  checksum: b0c1776f9c46474219eb471eeb8f4c8986a7735dc8356e578a63303cf292a7c8cb868fa74bf94a1a174e948fcb6523c63fca081cac6bbf246be8275b3cc384f0
+  languageName: node
+  linkType: hard
+
+"css-tree@npm:^2.3.1":
+  version: 2.3.1
+  resolution: "css-tree@npm:2.3.1"
+  dependencies:
+    mdn-data: 2.0.30
+    source-map-js: ^1.0.1
+  checksum: 493cc24b5c22b05ee5314b8a0d72d8a5869491c1458017ae5ed75aeb6c3596637dbe1b11dac2548974624adec9f7a1f3a6cf40593dc1f9185eb0e8279543fbc0
   languageName: node
   linkType: hard
 
 "cssesc@npm:^3.0.0":
   version: 3.0.0
   resolution: "cssesc@npm:3.0.0"
   bin:
@@ -4540,17 +4619,17 @@
   version: 3.0.10
   resolution: "csstype@npm:3.0.10"
   checksum: 20a8fa324f2b33ddf94aa7507d1b6ab3daa6f3cc308888dc50126585d7952f2471de69b2dbe0635d1fdc31223fef8e070842691877e725caf456e2378685a631
   languageName: node
   linkType: hard
 
 "csstype@npm:^3.0.2":
-  version: 3.1.2
-  resolution: "csstype@npm:3.1.2"
-  checksum: e1a52e6c25c1314d6beef5168da704ab29c5186b877c07d822bd0806717d9a265e8493a2e35ca7e68d0f5d472d43fac1cdce70fd79fd0853dff81f3028d857b5
+  version: 3.1.3
+  resolution: "csstype@npm:3.1.3"
+  checksum: 8db785cc92d259102725b3c694ec0c823f5619a84741b5c7991b8ad135dfaa66093038a1cc63e03361a6cd28d122be48f2106ae72334e067dd619a51f49eddf7
   languageName: node
   linkType: hard
 
 "data-urls@npm:^2.0.0":
   version: 2.0.0
   resolution: "data-urls@npm:2.0.0"
   dependencies:
@@ -4568,15 +4647,15 @@
     abab: ^2.0.6
     whatwg-mimetype: ^3.0.0
     whatwg-url: ^11.0.0
   checksum: 033fc3dd0fba6d24bc9a024ddcf9923691dd24f90a3d26f6545d6a2f71ec6956f93462f2cdf2183cc46f10dc01ed3bcb36731a8208456eb1a08147e571fe2a76
   languageName: node
   linkType: hard
 
-"debug@npm:4, debug@npm:^4.1.0, debug@npm:^4.1.1, debug@npm:^4.3.2, debug@npm:^4.3.4":
+"debug@npm:4, debug@npm:^4.1.0, debug@npm:^4.1.1, debug@npm:^4.3.1, debug@npm:^4.3.2, debug@npm:^4.3.4":
   version: 4.3.4
   resolution: "debug@npm:4.3.4"
   dependencies:
     ms: 2.1.2
   peerDependenciesMeta:
     supports-color:
       optional: true
@@ -4590,21 +4669,28 @@
   dependencies:
     decamelize: ^1.1.0
     map-obj: ^1.0.0
   checksum: fc645fe20b7bda2680bbf9481a3477257a7f9304b1691036092b97ab04c0ab53e3bf9fcc2d2ae382536568e402ec41fb11e1d4c3836a9abe2d813dd9ef4311e0
   languageName: node
   linkType: hard
 
-"decamelize@npm:^1.1.0, decamelize@npm:^1.2.0":
+"decamelize@npm:^1.1.0":
   version: 1.2.0
   resolution: "decamelize@npm:1.2.0"
   checksum: ad8c51a7e7e0720c70ec2eeb1163b66da03e7616d7b98c9ef43cce2416395e84c1e9548dd94f5f6ffecfee9f8b94251fc57121a8b021f2ff2469b2bae247b8aa
   languageName: node
   linkType: hard
 
+"decamelize@npm:^5.0.0":
+  version: 5.0.1
+  resolution: "decamelize@npm:5.0.1"
+  checksum: 7c3b1ed4b3e60e7fbc00a35fb248298527c1cdfe603e41dfcf05e6c4a8cb9efbee60630deb677ed428908fb4e74e322966c687a094d1478ddc9c3a74e9dc7140
+  languageName: node
+  linkType: hard
+
 "decimal.js@npm:^10.4.2":
   version: 10.4.3
   resolution: "decimal.js@npm:10.4.3"
   checksum: 796404dcfa9d1dbfdc48870229d57f788b48c21c603c3f6554a1c17c10195fc1024de338b0cf9e1efe0c7c167eeb18f04548979bcc5fdfabebb7cc0ae3287bae
   languageName: node
   linkType: hard
 
@@ -4641,15 +4727,15 @@
     get-intrinsic: ^1.2.1
     gopd: ^1.0.1
     has-property-descriptors: ^1.0.0
   checksum: a29855ad3f0630ea82e3c5012c812efa6ca3078d5c2aa8df06b5f597c1cde6f7254692df41945851d903e05a1668607b6d34e778f402b9ff9ffb38111f1a3f0d
   languageName: node
   linkType: hard
 
-"define-properties@npm:^1.1.3, define-properties@npm:^1.1.4, define-properties@npm:^1.2.0":
+"define-properties@npm:^1.1.3, define-properties@npm:^1.2.0, define-properties@npm:^1.2.1":
   version: 1.2.1
   resolution: "define-properties@npm:1.2.1"
   dependencies:
     define-data-property: ^1.0.1
     has-property-descriptors: ^1.0.0
     object-keys: ^1.1.1
   checksum: b4ccd00597dd46cb2d4a379398f5b19fca84a16f3374e2249201992f36b30f6835949a9429669ee6b41b6e837205a163eadd745e472069e70dfc10f03e5fcc12
@@ -4757,18 +4843,18 @@
 "eastasianwidth@npm:^0.2.0":
   version: 0.2.0
   resolution: "eastasianwidth@npm:0.2.0"
   checksum: 7d00d7cd8e49b9afa762a813faac332dee781932d6f2c848dc348939c4253f1d4564341b7af1d041853bc3f32c2ef141b58e0a4d9862c17a7f08f68df1e0f1ed
   languageName: node
   linkType: hard
 
-"electron-to-chromium@npm:^1.4.535":
-  version: 1.4.575
-  resolution: "electron-to-chromium@npm:1.4.575"
-  checksum: 57ddf102e6b38d107ec72bb2e481f55dbcff58bfcc4f99be5f12baa69d1e6661e1f3b1b6324bbbbff3b35972a6061fb09381fc84f98110540c395a5987f8f067
+"electron-to-chromium@npm:^1.4.601":
+  version: 1.4.647
+  resolution: "electron-to-chromium@npm:1.4.647"
+  checksum: fd79098e08a03025fb64a0608dd20942a7004bb38a8c7fd6d18d8b1767712866a3dae2df7e69ddbc7c627352278cbd07ce1a7368b6c037129e68a042802e108c
   languageName: node
   linkType: hard
 
 "emittery@npm:^0.13.1":
   version: 0.13.1
   resolution: "emittery@npm:0.13.1"
   checksum: 2b089ab6306f38feaabf4f6f02792f9ec85fc054fda79f44f6790e61bbf6bc4e1616afb9b232e0c5ec5289a8a452f79bfa6d905a6fd64e94b49981f0934001c6
@@ -4905,17 +4991,17 @@
     unbox-primitive: ^1.0.2
     which-typed-array: ^1.1.13
   checksum: b1bdc962856836f6e72be10b58dc128282bdf33771c7a38ae90419d920fc3b36cc5d2b70a222ad8016e3fc322c367bf4e9e89fc2bc79b7e933c05b218e83d79a
   languageName: node
   linkType: hard
 
 "es-module-lexer@npm:^1.2.1":
-  version: 1.3.1
-  resolution: "es-module-lexer@npm:1.3.1"
-  checksum: 3beafa7e171eb1e8cc45695edf8d51638488dddf65294d7911f8d6a96249da6a9838c87529262cc6ea53988d8272cec0f4bff93f476ed031a54ba3afb51a0ed3
+  version: 1.4.1
+  resolution: "es-module-lexer@npm:1.4.1"
+  checksum: a11b5a256d4e8e9c7d94c2fd87415ccd1591617b6edd847e064503f8eaece2d25e2e9078a02c5ce3ed5e83bb748f5b4820efbe78072c8beb07ac619c2edec35d
   languageName: node
   linkType: hard
 
 "es-set-tostringtag@npm:^2.0.1":
   version: 2.0.2
   resolution: "es-set-tostringtag@npm:2.0.2"
   dependencies:
@@ -4979,41 +5065,46 @@
   bin:
     escodegen: bin/escodegen.js
     esgenerate: bin/esgenerate.js
   checksum: 096696407e161305cd05aebb95134ad176708bc5cb13d0dcc89a5fcbb959b8ed757e7f2591a5f8036f8f4952d4a724de0df14cd419e29212729fa6df5ce16bf6
   languageName: node
   linkType: hard
 
-"eslint-config-prettier@npm:^8.7.0":
+"eslint-config-prettier@npm:^8.8.0":
   version: 8.10.0
   resolution: "eslint-config-prettier@npm:8.10.0"
   peerDependencies:
     eslint: ">=7.0.0"
   bin:
     eslint-config-prettier: bin/cli.js
   checksum: 153266badd477e49b0759816246b2132f1dbdb6c7f313ca60a9af5822fd1071c2bc5684a3720d78b725452bbac04bb130878b2513aea5e72b1b792de5a69fec8
   languageName: node
   linkType: hard
 
-"eslint-plugin-prettier@npm:^4.2.1":
-  version: 4.2.1
-  resolution: "eslint-plugin-prettier@npm:4.2.1"
+"eslint-plugin-prettier@npm:^5.0.0":
+  version: 5.1.3
+  resolution: "eslint-plugin-prettier@npm:5.1.3"
   dependencies:
     prettier-linter-helpers: ^1.0.0
+    synckit: ^0.8.6
   peerDependencies:
-    eslint: ">=7.28.0"
-    prettier: ">=2.0.0"
+    "@types/eslint": ">=8.0.0"
+    eslint: ">=8.0.0"
+    eslint-config-prettier: "*"
+    prettier: ">=3.0.0"
   peerDependenciesMeta:
+    "@types/eslint":
+      optional: true
     eslint-config-prettier:
       optional: true
-  checksum: b9e839d2334ad8ec7a5589c5cb0f219bded260839a857d7a486997f9870e95106aa59b8756ff3f37202085ebab658de382b0267cae44c3a7f0eb0bcc03a4f6d6
+  checksum: eb2a7d46a1887e1b93788ee8f8eb81e0b6b2a6f5a66a62bc6f375b033fc4e7ca16448da99380be800042786e76cf5c0df9c87a51a2c9b960ed47acbd7c0b9381
   languageName: node
   linkType: hard
 
-"eslint-scope@npm:5.1.1, eslint-scope@npm:^5.1.1":
+"eslint-scope@npm:5.1.1":
   version: 5.1.1
   resolution: "eslint-scope@npm:5.1.1"
   dependencies:
     esrecurse: ^4.3.0
     estraverse: ^4.1.1
   checksum: 47e4b6a3f0cc29c7feedee6c67b225a2da7e155802c6ea13bbef4ac6b9e10c66cd2dcb987867ef176292bf4e64eccc680a49e35e9e9c669f4a02bac17e86abdb
   languageName: node
@@ -5033,21 +5124,21 @@
   version: 3.4.3
   resolution: "eslint-visitor-keys@npm:3.4.3"
   checksum: 36e9ef87fca698b6fd7ca5ca35d7b2b6eeaaf106572e2f7fd31c12d3bfdaccdb587bba6d3621067e5aece31c8c3a348b93922ab8f7b2cbc6aaab5e1d89040c60
   languageName: node
   linkType: hard
 
 "eslint@npm:^8.36.0":
-  version: 8.52.0
-  resolution: "eslint@npm:8.52.0"
+  version: 8.56.0
+  resolution: "eslint@npm:8.56.0"
   dependencies:
     "@eslint-community/eslint-utils": ^4.2.0
     "@eslint-community/regexpp": ^4.6.1
-    "@eslint/eslintrc": ^2.1.2
-    "@eslint/js": 8.52.0
+    "@eslint/eslintrc": ^2.1.4
+    "@eslint/js": 8.56.0
     "@humanwhocodes/config-array": ^0.11.13
     "@humanwhocodes/module-importer": ^1.0.1
     "@nodelib/fs.walk": ^1.2.8
     "@ungap/structured-clone": ^1.2.0
     ajv: ^6.12.4
     chalk: ^4.0.0
     cross-spawn: ^7.0.2
@@ -5076,15 +5167,15 @@
     minimatch: ^3.1.2
     natural-compare: ^1.4.0
     optionator: ^0.9.3
     strip-ansi: ^6.0.1
     text-table: ^0.2.0
   bin:
     eslint: bin/eslint.js
-  checksum: fd22d1e9bd7090e31b00cbc7a3b98f3b76020a4c4641f987ae7d0c8f52e1b88c3b268bdfdabac2e1a93513e5d11339b718ff45cbff48a44c35d7e52feba510ed
+  checksum: 883436d1e809b4a25d9eb03d42f584b84c408dbac28b0019f6ea07b5177940bf3cca86208f749a6a1e0039b63e085ee47aca1236c30721e91f0deef5cc5a5136
   languageName: node
   linkType: hard
 
 "espree@npm:^9.6.0, espree@npm:^9.6.1":
   version: 9.6.1
   resolution: "espree@npm:9.6.1"
   dependencies:
@@ -5205,24 +5296,24 @@
 "fast-diff@npm:^1.1.2":
   version: 1.3.0
   resolution: "fast-diff@npm:1.3.0"
   checksum: d22d371b994fdc8cce9ff510d7b8dc4da70ac327bcba20df607dd5b9cae9f908f4d1028f5fe467650f058d1e7270235ae0b8230809a262b4df587a3b3aa216c3
   languageName: node
   linkType: hard
 
-"fast-glob@npm:^3.2.12, fast-glob@npm:^3.2.9":
-  version: 3.3.1
-  resolution: "fast-glob@npm:3.3.1"
+"fast-glob@npm:^3.2.9, fast-glob@npm:^3.3.1":
+  version: 3.3.2
+  resolution: "fast-glob@npm:3.3.2"
   dependencies:
     "@nodelib/fs.stat": ^2.0.2
     "@nodelib/fs.walk": ^1.2.3
     glob-parent: ^5.1.2
     merge2: ^1.3.0
     micromatch: ^4.0.4
-  checksum: b6f3add6403e02cf3a798bfbb1183d0f6da2afd368f27456010c0bc1f9640aea308243d4cb2c0ab142f618276e65ecb8be1661d7c62a7b4e5ba774b9ce5432e5
+  checksum: 900e4979f4dbc3313840078419245621259f349950411ca2fa445a2f9a1a6d98c3b5e7e0660c5ccd563aa61abe133a21765c6c0dec8e57da1ba71d8000b05ec1
   languageName: node
   linkType: hard
 
 "fast-json-stable-stringify@npm:2.x, fast-json-stable-stringify@npm:^2.0.0, fast-json-stable-stringify@npm:^2.1.0":
   version: 2.1.0
   resolution: "fast-json-stable-stringify@npm:2.1.0"
   checksum: b191531e36c607977e5b1c47811158733c34ccb3bfde92c44798929e9b4154884378536d26ad90dfecd32e1ffc09c545d23535ad91b3161a27ddbb8ebe0cbecb
@@ -5240,19 +5331,19 @@
   version: 1.0.16
   resolution: "fastest-levenshtein@npm:1.0.16"
   checksum: a78d44285c9e2ae2c25f3ef0f8a73f332c1247b7ea7fb4a191e6bb51aa6ee1ef0dfb3ed113616dcdc7023e18e35a8db41f61c8d88988e877cf510df8edafbc71
   languageName: node
   linkType: hard
 
 "fastq@npm:^1.6.0":
-  version: 1.15.0
-  resolution: "fastq@npm:1.15.0"
+  version: 1.16.0
+  resolution: "fastq@npm:1.16.0"
   dependencies:
     reusify: ^1.0.4
-  checksum: 0170e6bfcd5d57a70412440b8ef600da6de3b2a6c5966aeaf0a852d542daff506a0ee92d6de7679d1de82e644bce69d7a574a6c93f0b03964b5337eed75ada1a
+  checksum: 1d40ed1f100ae625e5720484e8602b7ad07649370f1cbc3e34a6b9630a0bfed6946bab0322d8a368a1e3cde87bb9bbb8d3bc2ae01a0c1f022fac1d07c04e4feb
   languageName: node
   linkType: hard
 
 "fb-watchman@npm:^2.0.0":
   version: 2.0.2
   resolution: "fb-watchman@npm:2.0.2"
   dependencies:
@@ -5266,14 +5357,23 @@
   resolution: "file-entry-cache@npm:6.0.1"
   dependencies:
     flat-cache: ^3.0.4
   checksum: f49701feaa6314c8127c3c2f6173cfefff17612f5ed2daaafc6da13b5c91fd43e3b2a58fd0d63f9f94478a501b167615931e7200e31485e320f74a33885a9c74
   languageName: node
   linkType: hard
 
+"file-entry-cache@npm:^7.0.0":
+  version: 7.0.2
+  resolution: "file-entry-cache@npm:7.0.2"
+  dependencies:
+    flat-cache: ^3.2.0
+  checksum: 283c674fc26bed1c44e74cf25c2640c813e222ea30a2536404b53511ca311d4a2502ee8145a01aecd12b9a910eb4162364776be27a9683e8447332054e9d712f
+  languageName: node
+  linkType: hard
+
 "fill-range@npm:^7.0.1":
   version: 7.0.1
   resolution: "fill-range@npm:7.0.1"
   dependencies:
     to-regex-range: ^5.0.1
   checksum: cc283f4e65b504259e64fd969bcf4def4eb08d85565e906b7d36516e87819db52029a76b6363d0f02d0d532f0033c9603b9e2d943d56ee3b0d4f7ad3328ff917
   languageName: node
@@ -5302,22 +5402,22 @@
   dependencies:
     locate-path: ^6.0.0
     path-exists: ^4.0.0
   checksum: 07955e357348f34660bde7920783204ff5a26ac2cafcaa28bace494027158a97b9f56faaf2d89a6106211a8174db650dd9f503f9c0d526b1202d5554a00b9095
   languageName: node
   linkType: hard
 
-"flat-cache@npm:^3.0.4":
-  version: 3.1.1
-  resolution: "flat-cache@npm:3.1.1"
+"flat-cache@npm:^3.0.4, flat-cache@npm:^3.2.0":
+  version: 3.2.0
+  resolution: "flat-cache@npm:3.2.0"
   dependencies:
     flatted: ^3.2.9
     keyv: ^4.5.3
     rimraf: ^3.0.2
-  checksum: 4958cfe0f46acf84953d4e16676ef5f0d38eab3a92d532a1e8d5f88f11eea8b36d5d598070ff2aeae15f1fde18f8d7d089eefaf9db10b5a587cc1c9072325c7a
+  checksum: e7e0f59801e288b54bee5cb9681e9ee21ee28ef309f886b312c9d08415b79fc0f24ac842f84356ce80f47d6a53de62197ce0e6e148dc42d5db005992e2a756ec
   languageName: node
   linkType: hard
 
 "flat@npm:^5.0.2":
   version: 5.0.2
   resolution: "flat@npm:5.0.2"
   bin:
@@ -5522,15 +5622,15 @@
 "glob-to-regexp@npm:^0.4.1":
   version: 0.4.1
   resolution: "glob-to-regexp@npm:0.4.1"
   checksum: e795f4e8f06d2a15e86f76e4d92751cf8bbfcf0157cea5c2f0f35678a8195a750b34096b1256e436f0cebc1883b5ff0888c47348443e69546a5a87f9e1eb1167
   languageName: node
   linkType: hard
 
-"glob@npm:^10.2.2, glob@npm:^10.3.10":
+"glob@npm:^10.2.2, glob@npm:^10.3.10, glob@npm:^10.3.7":
   version: 10.3.10
   resolution: "glob@npm:10.3.10"
   dependencies:
     foreground-child: ^3.1.0
     jackspeak: ^2.3.5
     minimatch: ^9.0.1
     minipass: ^5.0.0 || ^6.0.2 || ^7.0.0
@@ -5551,26 +5651,14 @@
     minimatch: ^3.1.1
     once: ^1.3.0
     path-is-absolute: ^1.0.0
   checksum: 29452e97b38fa704dabb1d1045350fb2467cf0277e155aa9ff7077e90ad81d1ea9d53d3ee63bd37c05b09a065e90f16aec4a65f5b8de401d1dac40bc5605d133
   languageName: node
   linkType: hard
 
-"glob@npm:^9.2.0":
-  version: 9.3.5
-  resolution: "glob@npm:9.3.5"
-  dependencies:
-    fs.realpath: ^1.0.0
-    minimatch: ^8.0.2
-    minipass: ^4.2.4
-    path-scurry: ^1.6.1
-  checksum: 94b093adbc591bc36b582f77927d1fb0dbf3ccc231828512b017601408be98d1fe798fc8c0b19c6f2d1a7660339c3502ce698de475e9d938ccbb69b47b647c84
-  languageName: node
-  linkType: hard
-
 "glob@npm:~7.1.6":
   version: 7.1.7
   resolution: "glob@npm:7.1.7"
   dependencies:
     fs.realpath: ^1.0.0
     inflight: ^1.0.4
     inherits: 2
@@ -5605,19 +5693,19 @@
   version: 11.12.0
   resolution: "globals@npm:11.12.0"
   checksum: 67051a45eca3db904aee189dfc7cd53c20c7d881679c93f6146ddd4c9f4ab2268e68a919df740d39c71f4445d2b38ee360fc234428baea1dbdfe68bbcb46979e
   languageName: node
   linkType: hard
 
 "globals@npm:^13.19.0":
-  version: 13.23.0
-  resolution: "globals@npm:13.23.0"
+  version: 13.24.0
+  resolution: "globals@npm:13.24.0"
   dependencies:
     type-fest: ^0.20.2
-  checksum: 194c97cf8d1ef6ba59417234c2386549c4103b6e5f24b1ff1952de61a4753e5d2069435ba629de711a6480b1b1d114a98e2ab27f85e966d5a10c319c3bbd3dc3
+  checksum: 56066ef058f6867c04ff203b8a44c15b038346a62efbc3060052a1016be9f56f4cf0b2cd45b74b22b81e521a889fc7786c73691b0549c2f3a6e825b3d394f43c
   languageName: node
   linkType: hard
 
 "globalthis@npm:^1.0.3":
   version: 1.0.3
   resolution: "globalthis@npm:1.0.3"
   dependencies:
@@ -5701,15 +5789,15 @@
 "has-flag@npm:^4.0.0":
   version: 4.0.0
   resolution: "has-flag@npm:4.0.0"
   checksum: 261a1357037ead75e338156b1f9452c016a37dcd3283a972a30d9e4a87441ba372c8b81f818cd0fbcd9c0354b4ae7e18b9e1afa1971164aef6d18c2b6095a8ad
   languageName: node
   linkType: hard
 
-"has-property-descriptors@npm:^1.0.0":
+"has-property-descriptors@npm:^1.0.0, has-property-descriptors@npm:^1.0.1":
   version: 1.0.1
   resolution: "has-property-descriptors@npm:1.0.1"
   dependencies:
     get-intrinsic: ^1.2.2
   checksum: 2bcc6bf6ec6af375add4e4b4ef586e43674850a91ad4d46666d0b28ba8e1fd69e424c7677d24d60f69470ad0afaa2f3197f508b20b0bb7dd99a8ab77ffc4b7c4
   languageName: node
   linkType: hard
@@ -5774,15 +5862,15 @@
 "html-escaper@npm:^2.0.0":
   version: 2.0.2
   resolution: "html-escaper@npm:2.0.2"
   checksum: d2df2da3ad40ca9ee3a39c5cc6475ef67c8f83c234475f24d8e9ce0dc80a2c82df8e1d6fa78ddd1e9022a586ea1bd247a615e80a5cd9273d90111ddda7d9e974
   languageName: node
   linkType: hard
 
-"html-tags@npm:^3.2.0":
+"html-tags@npm:^3.3.1":
   version: 3.3.1
   resolution: "html-tags@npm:3.3.1"
   checksum: b4ef1d5a76b678e43cce46e3783d563607b1d550cab30b4f511211564574770aa8c658a400b100e588bc60b8234e59b35ff72c7851cc28f3b5403b13a2c6cbce
   languageName: node
   linkType: hard
 
 "htmlparser2@npm:^6.0.0":
@@ -5875,22 +5963,22 @@
   resolution: "identity-obj-proxy@npm:3.0.0"
   dependencies:
     harmony-reflect: ^1.4.6
   checksum: 97559f8ea2aeaa1a880d279d8c49550dce01148321e00a2102cda5ddf9ce622fa1d7f3efc7bed63458af78889de888fdaebaf31c816312298bb3fdd0ef8aaf2c
   languageName: node
   linkType: hard
 
-"ignore@npm:^5.2.0, ignore@npm:^5.2.1":
-  version: 5.2.4
-  resolution: "ignore@npm:5.2.4"
-  checksum: 3d4c309c6006e2621659311783eaea7ebcd41fe4ca1d78c91c473157ad6666a57a2df790fe0d07a12300d9aac2888204d7be8d59f9aaf665b1c7fcdb432517ef
+"ignore@npm:^5.2.0, ignore@npm:^5.2.4":
+  version: 5.3.0
+  resolution: "ignore@npm:5.3.0"
+  checksum: 2736da6621f14ced652785cb05d86301a66d70248597537176612bd0c8630893564bd5f6421f8806b09e8472e75c591ef01672ab8059c07c6eb2c09cefe04bf9
   languageName: node
   linkType: hard
 
-"import-fresh@npm:^3.2.1":
+"import-fresh@npm:^3.2.1, import-fresh@npm:^3.3.0":
   version: 3.3.0
   resolution: "import-fresh@npm:3.3.0"
   dependencies:
     parent-module: ^1.0.0
     resolve-from: ^4.0.0
   checksum: 2cacfad06e652b1edc50be650f7ec3be08c5e5a6f6d12d035c440a42a8cc028e60a5b99ca08a77ab4d6b1346da7d971915828f33cdab730d3d42f08242d09baa
   languageName: node
@@ -5925,14 +6013,21 @@
 "indent-string@npm:^4.0.0":
   version: 4.0.0
   resolution: "indent-string@npm:4.0.0"
   checksum: 824cfb9929d031dabf059bebfe08cf3137365e112019086ed3dcff6a0a7b698cb80cf67ccccde0e25b9e2d7527aa6cc1fed1ac490c752162496caba3e6699612
   languageName: node
   linkType: hard
 
+"indent-string@npm:^5.0.0":
+  version: 5.0.0
+  resolution: "indent-string@npm:5.0.0"
+  checksum: e466c27b6373440e6d84fbc19e750219ce25865cb82d578e41a6053d727e5520dc5725217d6eb1cc76005a1bb1696a0f106d84ce7ebda3033b963a38583fb3b3
+  languageName: node
+  linkType: hard
+
 "inflight@npm:^1.0.4":
   version: 1.0.6
   resolution: "inflight@npm:1.0.6"
   dependencies:
     once: ^1.3.0
     wrappy: 1
   checksum: f4f76aa072ce19fae87ce1ef7d221e709afb59d445e05d47fba710e85470923a75de35bfae47da6de1b18afc3ce83d70facf44cfb0aff89f0a3f45c0a0244dfd
@@ -6231,17 +6326,17 @@
   version: 0.2.5
   resolution: "isomorphic.js@npm:0.2.5"
   checksum: d8d1b083f05f3c337a06628b982ac3ce6db953bbef14a9de8ad49131250c3592f864b73c12030fdc9ef138ce97b76ef55c7d96a849561ac215b1b4b9d301c8e9
   languageName: node
   linkType: hard
 
 "istanbul-lib-coverage@npm:^3.0.0, istanbul-lib-coverage@npm:^3.2.0":
-  version: 3.2.0
-  resolution: "istanbul-lib-coverage@npm:3.2.0"
-  checksum: a2a545033b9d56da04a8571ed05c8120bf10e9bce01cf8633a3a2b0d1d83dff4ac4fe78d6d5673c27fc29b7f21a41d75f83a36be09f82a61c367b56aa73c1ff9
+  version: 3.2.2
+  resolution: "istanbul-lib-coverage@npm:3.2.2"
+  checksum: 2367407a8d13982d8f7a859a35e7f8dd5d8f75aae4bb5484ede3a9ea1b426dc245aff28b976a2af48ee759fdd9be374ce2bd2669b644f31e76c5f46a2e29a831
   languageName: node
   linkType: hard
 
 "istanbul-lib-instrument@npm:^5.0.4":
   version: 5.2.1
   resolution: "istanbul-lib-instrument@npm:5.2.1"
   dependencies:
@@ -6973,39 +7068,42 @@
   languageName: node
   linkType: hard
 
 "jupyterlab_unianalytics_telemetry@workspace:.":
   version: 0.0.0-use.local
   resolution: "jupyterlab_unianalytics_telemetry@workspace:."
   dependencies:
-    "@jupyterlab/application": ^3.1.0 || ^4.0.0
+    "@jupyterlab/application": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
-    "@jupyterlab/settingregistry": ^3.1.0 || ^4.0.0
+    "@jupyterlab/coreutils": ^6.0.0
+    "@jupyterlab/services": ^7.0.0
+    "@jupyterlab/settingregistry": ^4.0.0
     "@jupyterlab/testutils": ^4.0.0
-    "@types/crypto-js": ^4.1.2
     "@types/jest": ^29.2.0
     "@types/json-schema": ^7.0.11
     "@types/react": ^18.0.26
-    "@typescript-eslint/eslint-plugin": ^5.55.0
-    "@typescript-eslint/parser": ^5.55.0
+    "@types/react-addons-linked-state-mixin": ^0.14.22
+    "@typescript-eslint/eslint-plugin": ^6.1.0
+    "@typescript-eslint/parser": ^6.1.0
     css-loader: ^6.7.1
     eslint: ^8.36.0
-    eslint-config-prettier: ^8.7.0
-    eslint-plugin-prettier: ^4.2.1
+    eslint-config-prettier: ^8.8.0
+    eslint-plugin-prettier: ^5.0.0
     jest: ^29.2.0
+    mkdirp: ^1.0.3
     npm-run-all: ^4.1.5
-    prettier: ^2.8.7
-    rimraf: ^4.4.1
+    prettier: ^3.0.0
+    rimraf: ^5.0.1
     source-map-loader: ^1.0.2
     style-loader: ^3.3.1
-    stylelint: ^14.9.1
-    stylelint-config-prettier: ^9.0.4
-    stylelint-config-recommended: ^8.0.0
-    stylelint-config-standard: ^26.0.0
-    stylelint-prettier: ^2.0.0
+    stylelint: ^15.10.1
+    stylelint-config-recommended: ^13.0.0
+    stylelint-config-standard: ^34.0.0
+    stylelint-csstree-validator: ^3.0.0
+    stylelint-prettier: ^4.0.0
     typescript: ~5.0.2
     yjs: ^13.5.0
   languageName: unknown
   linkType: soft
 
 "keyv@npm:^4.5.3":
   version: 4.5.4
@@ -7026,18 +7124,18 @@
 "kleur@npm:^3.0.3":
   version: 3.0.3
   resolution: "kleur@npm:3.0.3"
   checksum: df82cd1e172f957bae9c536286265a5cdbd5eeca487cb0a3b2a7b41ef959fc61f8e7c0e9aeea9c114ccf2c166b6a8dd45a46fd619c1c569d210ecd2765ad5169
   languageName: node
   linkType: hard
 
-"known-css-properties@npm:^0.26.0":
-  version: 0.26.0
-  resolution: "known-css-properties@npm:0.26.0"
-  checksum: e706f4af9d2683202df9f717e7d713f0f8c3330f155842c40d8f3b2a5837956c34aeb7ba08760977ccde1afce8b5377e29b40eb3e5c0b42bef28ddd108543cfb
+"known-css-properties@npm:^0.29.0":
+  version: 0.29.0
+  resolution: "known-css-properties@npm:0.29.0"
+  checksum: daa6562e907f856cbfd58a00c42f532c9bba283388984da6a3bffb494e56612e5f23c52f30b0d9885f0ea07ad5d88bfa0470ee65017a6ce6c565289a1afd78af
   languageName: node
   linkType: hard
 
 "leven@npm:^3.1.0":
   version: 3.1.0
   resolution: "leven@npm:3.1.0"
   checksum: 638401d534585261b6003db9d99afd244dfe82d75ddb6db5c0df412842d5ab30b2ef18de471aaec70fe69a46f17b4ae3c7f01d8a4e6580ef7adb9f4273ad1e55
@@ -7050,23 +7148,23 @@
   dependencies:
     prelude-ls: ^1.2.1
     type-check: ~0.4.0
   checksum: 12c5021c859bd0f5248561bf139121f0358285ec545ebf48bb3d346820d5c61a4309535c7f387ed7d84361cf821e124ce346c6b7cef8ee09a67c1473b46d0fc4
   languageName: node
   linkType: hard
 
-"lib0@npm:^0.2.74, lib0@npm:^0.2.85":
-  version: 0.2.87
-  resolution: "lib0@npm:0.2.87"
+"lib0@npm:^0.2.85, lib0@npm:^0.2.86":
+  version: 0.2.88
+  resolution: "lib0@npm:0.2.88"
   dependencies:
     isomorphic.js: ^0.2.4
   bin:
     0gentesthtml: bin/gentesthtml.js
     0serve: bin/0serve.js
-  checksum: c50f4ed27e4df1a8fe8846251740e3757ac37146087a3b14f23240aa654174ccaf62f4f516cfa162fae019f82cdc0483b78310dd8410ac5fc8b5092b4d2e0b5d
+  checksum: 1ac13d6781f4d29aa317ad9fb9b6c41e8bed52b096a369f54d10d9b8651ceb4a0a63b06c01c2e1c7319d3bb74668afb6cac3735161b32031f185cec024bbba37
   languageName: node
   linkType: hard
 
 "license-webpack-plugin@npm:^2.3.14":
   version: 2.3.21
   resolution: "license-webpack-plugin@npm:2.3.21"
   dependencies:
@@ -7198,17 +7296,17 @@
   bin:
     loose-envify: cli.js
   checksum: 6517e24e0cad87ec9888f500c5b5947032cdfe6ef65e1c1936a0c48a524b81e65542c9c3edc91c97d5bddc806ee2a985dbc79be89215d613b1de5db6d1cfe6f4
   languageName: node
   linkType: hard
 
 "lru-cache@npm:^10.0.1, lru-cache@npm:^9.1.1 || ^10.0.0":
-  version: 10.0.1
-  resolution: "lru-cache@npm:10.0.1"
-  checksum: 06f8d0e1ceabd76bb6f644a26dbb0b4c471b79c7b514c13c6856113879b3bf369eb7b497dad4ff2b7e2636db202412394865b33c332100876d838ad1372f0181
+  version: 10.2.0
+  resolution: "lru-cache@npm:10.2.0"
+  checksum: eee7ddda4a7475deac51ac81d7dd78709095c6fa46e8350dc2d22462559a1faa3b81ed931d5464b13d48cbd7e08b46100b6f768c76833912bc444b99c37e25db
   languageName: node
   linkType: hard
 
 "lru-cache@npm:^5.1.1":
   version: 5.1.1
   resolution: "lru-cache@npm:5.1.1"
   dependencies:
@@ -7273,61 +7371,68 @@
 "map-obj@npm:^1.0.0":
   version: 1.0.1
   resolution: "map-obj@npm:1.0.1"
   checksum: 9949e7baec2a336e63b8d4dc71018c117c3ce6e39d2451ccbfd3b8350c547c4f6af331a4cbe1c83193d7c6b786082b6256bde843db90cb7da2a21e8fcc28afed
   languageName: node
   linkType: hard
 
-"map-obj@npm:^4.0.0":
+"map-obj@npm:^4.1.0":
   version: 4.3.0
   resolution: "map-obj@npm:4.3.0"
   checksum: fbc554934d1a27a1910e842bc87b177b1a556609dd803747c85ece420692380827c6ae94a95cce4407c054fa0964be3bf8226f7f2cb2e9eeee432c7c1985684e
   languageName: node
   linkType: hard
 
-"markdown-to-jsx@npm:^7.3.2":
-  version: 7.3.2
-  resolution: "markdown-to-jsx@npm:7.3.2"
+"markdown-to-jsx@npm:^7.4.0":
+  version: 7.4.0
+  resolution: "markdown-to-jsx@npm:7.4.0"
   peerDependencies:
     react: ">= 0.14.0"
-  checksum: 8885c6343b71570b0a7ec16cd85a49b853a830234790ee7430e2517ea5d8d361ff138bd52147f650790f3e7b3a28a15c755fc16f8856dd01ddf09a6161782e06
+  checksum: 59959d14d7927ed8a97e42d39771e2b445b90fa098477fb6ab040f044d230517dc4a95ba38a4f924cfc965a96b32211d93def150a6184f0e51d2cefdc8cb415d
   languageName: node
   linkType: hard
 
 "mathml-tag-names@npm:^2.1.3":
   version: 2.1.3
   resolution: "mathml-tag-names@npm:2.1.3"
   checksum: 1201a25a137d6b9e328facd67912058b8b45b19a6c4cc62641c9476195da28a275ca6e0eca070af5378b905c2b11abc1114676ba703411db0b9ce007de921ad0
   languageName: node
   linkType: hard
 
+"mdn-data@npm:2.0.30":
+  version: 2.0.30
+  resolution: "mdn-data@npm:2.0.30"
+  checksum: d6ac5ac7439a1607df44b22738ecf83f48e66a0874e4482d6424a61c52da5cde5750f1d1229b6f5fa1b80a492be89465390da685b11f97d62b8adcc6e88189aa
+  languageName: node
+  linkType: hard
+
 "memorystream@npm:^0.3.1":
   version: 0.3.1
   resolution: "memorystream@npm:0.3.1"
   checksum: f18b42440d24d09516d01466c06adf797df7873f0d40aa7db02e5fb9ed83074e5e65412d0720901d7069363465f82dc4f8bcb44f0cde271567a61426ce6ca2e9
   languageName: node
   linkType: hard
 
-"meow@npm:^9.0.0":
-  version: 9.0.0
-  resolution: "meow@npm:9.0.0"
-  dependencies:
-    "@types/minimist": ^1.2.0
-    camelcase-keys: ^6.2.2
-    decamelize: ^1.2.0
+"meow@npm:^10.1.5":
+  version: 10.1.5
+  resolution: "meow@npm:10.1.5"
+  dependencies:
+    "@types/minimist": ^1.2.2
+    camelcase-keys: ^7.0.0
+    decamelize: ^5.0.0
     decamelize-keys: ^1.1.0
     hard-rejection: ^2.1.0
     minimist-options: 4.1.0
-    normalize-package-data: ^3.0.0
-    read-pkg-up: ^7.0.1
-    redent: ^3.0.0
-    trim-newlines: ^3.0.0
-    type-fest: ^0.18.0
-    yargs-parser: ^20.2.3
-  checksum: 99799c47247f4daeee178e3124f6ef6f84bde2ba3f37652865d5d8f8b8adcf9eedfc551dd043e2455cd8206545fd848e269c0c5ab6b594680a0ad4d3617c9639
+    normalize-package-data: ^3.0.2
+    read-pkg-up: ^8.0.0
+    redent: ^4.0.0
+    trim-newlines: ^4.0.2
+    type-fest: ^1.2.2
+    yargs-parser: ^20.2.9
+  checksum: dd5f0caa4af18517813547dc66741dcbf52c4c23def5062578d39b11189fd9457aee5c1f2263a5cd6592a465023df8357e8ac876b685b64dbcf545e3f66c23a7
   languageName: node
   linkType: hard
 
 "merge-stream@npm:^2.0.0":
   version: 2.0.0
   resolution: "merge-stream@npm:2.0.0"
   checksum: 6fa4dcc8d86629705cea944a4b88ef4cb0e07656ebf223fa287443256414283dd25d91c1cd84c77987f2aec5927af1a9db6085757cb43d90eb170ebf4b47f4f4
@@ -7370,65 +7475,56 @@
 "mimic-fn@npm:^2.1.0":
   version: 2.1.0
   resolution: "mimic-fn@npm:2.1.0"
   checksum: d2421a3444848ce7f84bd49115ddacff29c15745db73f54041edc906c14b131a38d05298dae3081667627a59b2eb1ca4b436ff2e1b80f69679522410418b478a
   languageName: node
   linkType: hard
 
-"min-indent@npm:^1.0.0":
+"min-indent@npm:^1.0.1":
   version: 1.0.1
   resolution: "min-indent@npm:1.0.1"
   checksum: bfc6dd03c5eaf623a4963ebd94d087f6f4bbbfd8c41329a7f09706b0cb66969c4ddd336abeb587bc44bc6f08e13bf90f0b374f9d71f9f01e04adc2cd6f083ef1
   languageName: node
   linkType: hard
 
 "mini-css-extract-plugin@npm:^2.7.0":
-  version: 2.7.6
-  resolution: "mini-css-extract-plugin@npm:2.7.6"
+  version: 2.7.7
+  resolution: "mini-css-extract-plugin@npm:2.7.7"
   dependencies:
     schema-utils: ^4.0.0
   peerDependencies:
     webpack: ^5.0.0
-  checksum: be6f7cefc6275168eb0a6b8fe977083a18c743c9612c9f00e6c1a62c3393ca7960e93fba1a7ebb09b75f36a0204ad087d772c1ef574bc29c90c0e8175a3c0b83
+  checksum: 04af0e7d8c1a4ff31c70ac2d0895837dae3d51cce3bfd90e3c1d90d50eef7de21778361a3064531df046d775d80b3bf056324dddea93831c7def2047c5aa8718
   languageName: node
   linkType: hard
 
 "mini-svg-data-uri@npm:^1.4.4":
   version: 1.4.4
   resolution: "mini-svg-data-uri@npm:1.4.4"
   bin:
     mini-svg-data-uri: cli.js
   checksum: 997f1fbd8d59a70f03761e18626d335197a3479cb9d1ff75678e4b64b864d32a0b8fc18115eabde035e5299b8b4a354a78e57dd6ac10f9d604162a6170898d09
   languageName: node
   linkType: hard
 
-"minimatch@npm:^3.0.4, minimatch@npm:^3.0.5, minimatch@npm:^3.1.1, minimatch@npm:^3.1.2":
-  version: 3.1.2
-  resolution: "minimatch@npm:3.1.2"
-  dependencies:
-    brace-expansion: ^1.1.7
-  checksum: c154e566406683e7bcb746e000b84d74465b3a832c45d59912b9b55cd50dee66e5c4b1e5566dba26154040e51672f9aa450a9aef0c97cfc7336b78b7afb9540a
-  languageName: node
-  linkType: hard
-
-"minimatch@npm:^8.0.2":
-  version: 8.0.4
-  resolution: "minimatch@npm:8.0.4"
+"minimatch@npm:9.0.3, minimatch@npm:^9.0.1":
+  version: 9.0.3
+  resolution: "minimatch@npm:9.0.3"
   dependencies:
     brace-expansion: ^2.0.1
-  checksum: 2e46cffb86bacbc524ad45a6426f338920c529dd13f3a732cc2cf7618988ee1aae88df4ca28983285aca9e0f45222019ac2d14ebd17c1edadd2ee12221ab801a
+  checksum: 253487976bf485b612f16bf57463520a14f512662e592e95c571afdab1442a6a6864b6c88f248ce6fc4ff0b6de04ac7aa6c8bb51e868e99d1d65eb0658a708b5
   languageName: node
   linkType: hard
 
-"minimatch@npm:^9.0.1":
-  version: 9.0.3
-  resolution: "minimatch@npm:9.0.3"
+"minimatch@npm:^3.0.4, minimatch@npm:^3.0.5, minimatch@npm:^3.1.1, minimatch@npm:^3.1.2":
+  version: 3.1.2
+  resolution: "minimatch@npm:3.1.2"
   dependencies:
-    brace-expansion: ^2.0.1
-  checksum: 253487976bf485b612f16bf57463520a14f512662e592e95c571afdab1442a6a6864b6c88f248ce6fc4ff0b6de04ac7aa6c8bb51e868e99d1d65eb0658a708b5
+    brace-expansion: ^1.1.7
+  checksum: c154e566406683e7bcb746e000b84d74465b3a832c45d59912b9b55cd50dee66e5c4b1e5566dba26154040e51672f9aa450a9aef0c97cfc7336b78b7afb9540a
   languageName: node
   linkType: hard
 
 "minimist-options@npm:4.1.0":
   version: 4.1.0
   resolution: "minimist-options@npm:4.1.0"
   dependencies:
@@ -7442,20 +7538,20 @@
 "minimist@npm:~1.2.0":
   version: 1.2.8
   resolution: "minimist@npm:1.2.8"
   checksum: 75a6d645fb122dad29c06a7597bddea977258957ed88d7a6df59b5cd3fe4a527e253e9bbf2e783e4b73657f9098b96a5fe96ab8a113655d4109108577ecf85b0
   languageName: node
   linkType: hard
 
-"minipass-collect@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "minipass-collect@npm:1.0.2"
+"minipass-collect@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "minipass-collect@npm:2.0.1"
   dependencies:
-    minipass: ^3.0.0
-  checksum: 14df761028f3e47293aee72888f2657695ec66bd7d09cae7ad558da30415fdc4752bbfee66287dcc6fd5e6a2fa3466d6c484dc1cbd986525d9393b9523d97f10
+    minipass: ^7.0.3
+  checksum: b251bceea62090f67a6cced7a446a36f4cd61ee2d5cea9aee7fff79ba8030e416327a1c5aa2908dc22629d06214b46d88fdab8c51ac76bacbf5703851b5ad342
   languageName: node
   linkType: hard
 
 "minipass-fetch@npm:^3.0.0":
   version: 3.0.4
   resolution: "minipass-fetch@npm:3.0.4"
   dependencies:
@@ -7502,21 +7598,14 @@
   resolution: "minipass@npm:3.3.6"
   dependencies:
     yallist: ^4.0.0
   checksum: a30d083c8054cee83cdcdc97f97e4641a3f58ae743970457b1489ce38ee1167b3aaf7d815cd39ec7a99b9c40397fd4f686e83750e73e652b21cb516f6d845e48
   languageName: node
   linkType: hard
 
-"minipass@npm:^4.2.4":
-  version: 4.2.8
-  resolution: "minipass@npm:4.2.8"
-  checksum: 7f4914d5295a9a30807cae5227a37a926e6d910c03f315930fde52332cf0575dfbc20295318f91f0baf0e6bb11a6f668e30cde8027dea7a11b9d159867a3c830
-  languageName: node
-  linkType: hard
-
 "minipass@npm:^5.0.0":
   version: 5.0.0
   resolution: "minipass@npm:5.0.0"
   checksum: 425dab288738853fded43da3314a0b5c035844d6f3097a8e3b5b29b328da8f3c1af6fc70618b32c29ff906284cf6406b6841376f21caaadd0793c1d5a6a620ea
   languageName: node
   linkType: hard
 
@@ -7549,27 +7638,20 @@
 "ms@npm:2.1.2":
   version: 2.1.2
   resolution: "ms@npm:2.1.2"
   checksum: 673cdb2c3133eb050c745908d8ce632ed2c02d85640e2edb3ace856a2266a813b30c613569bf3354fdf4ea7d1a1494add3bfa95e2713baa27d0c2c71fc44f58f
   languageName: node
   linkType: hard
 
-"nanoid@npm:^3.3.6":
-  version: 3.3.6
-  resolution: "nanoid@npm:3.3.6"
+"nanoid@npm:^3.3.7":
+  version: 3.3.7
+  resolution: "nanoid@npm:3.3.7"
   bin:
     nanoid: bin/nanoid.cjs
-  checksum: 7d0eda657002738aa5206107bd0580aead6c95c460ef1bdd0b1a87a9c7ae6277ac2e9b945306aaa5b32c6dcb7feaf462d0f552e7f8b5718abfc6ead5c94a71b3
-  languageName: node
-  linkType: hard
-
-"natural-compare-lite@npm:^1.4.0":
-  version: 1.4.0
-  resolution: "natural-compare-lite@npm:1.4.0"
-  checksum: 5222ac3986a2b78dd6069ac62cbb52a7bf8ffc90d972ab76dfe7b01892485d229530ed20d0c62e79a6b363a663b273db3bde195a1358ce9e5f779d4453887225
+  checksum: d36c427e530713e4ac6567d488b489a36582ef89da1d6d4e3b87eded11eb10d7042a877958c6f104929809b2ab0bafa17652b076cdf84324aa75b30b722204f2
   languageName: node
   linkType: hard
 
 "natural-compare@npm:^1.4.0":
   version: 1.4.0
   resolution: "natural-compare@npm:1.4.0"
   checksum: 23ad088b08f898fc9b53011d7bb78ec48e79de7627e01ab5518e806033861bef68d5b0cd0e2205c2f36690ac9571ff6bcb05eb777ced2eeda8d4ac5b44592c3d
@@ -7634,45 +7716,45 @@
 "node-int64@npm:^0.4.0":
   version: 0.4.0
   resolution: "node-int64@npm:0.4.0"
   checksum: d0b30b1ee6d961851c60d5eaa745d30b5c95d94bc0e74b81e5292f7c42a49e3af87f1eb9e89f59456f80645d679202537de751b7d72e9e40ceea40c5e449057e
   languageName: node
   linkType: hard
 
-"node-releases@npm:^2.0.13":
-  version: 2.0.13
-  resolution: "node-releases@npm:2.0.13"
-  checksum: 17ec8f315dba62710cae71a8dad3cd0288ba943d2ece43504b3b1aa8625bf138637798ab470b1d9035b0545996f63000a8a926e0f6d35d0996424f8b6d36dda3
+"node-releases@npm:^2.0.14":
+  version: 2.0.14
+  resolution: "node-releases@npm:2.0.14"
+  checksum: 59443a2f77acac854c42d321bf1b43dea0aef55cd544c6a686e9816a697300458d4e82239e2d794ea05f7bbbc8a94500332e2d3ac3f11f52e4b16cbe638b3c41
   languageName: node
   linkType: hard
 
 "nopt@npm:^7.0.0":
   version: 7.2.0
   resolution: "nopt@npm:7.2.0"
   dependencies:
     abbrev: ^2.0.0
   bin:
     nopt: bin/nopt.js
   checksum: a9c0f57fb8cb9cc82ae47192ca2b7ef00e199b9480eed202482c962d61b59a7fbe7541920b2a5839a97b42ee39e288c0aed770e38057a608d7f579389dfde410
   languageName: node
   linkType: hard
 
-"normalize-package-data@npm:^2.3.2, normalize-package-data@npm:^2.5.0":
+"normalize-package-data@npm:^2.3.2":
   version: 2.5.0
   resolution: "normalize-package-data@npm:2.5.0"
   dependencies:
     hosted-git-info: ^2.1.4
     resolve: ^1.10.0
     semver: 2 || 3 || 4 || 5
     validate-npm-package-license: ^3.0.1
   checksum: 7999112efc35a6259bc22db460540cae06564aa65d0271e3bdfa86876d08b0e578b7b5b0028ee61b23f1cae9fc0e7847e4edc0948d3068a39a2a82853efc8499
   languageName: node
   linkType: hard
 
-"normalize-package-data@npm:^3.0.0":
+"normalize-package-data@npm:^3.0.2":
   version: 3.0.3
   resolution: "normalize-package-data@npm:3.0.3"
   dependencies:
     hosted-git-info: ^4.0.1
     is-core-module: ^2.5.0
     semver: ^7.3.4
     validate-npm-package-license: ^3.0.1
@@ -7742,22 +7824,22 @@
   version: 1.1.1
   resolution: "object-keys@npm:1.1.1"
   checksum: b363c5e7644b1e1b04aa507e88dcb8e3a2f52b6ffd0ea801e4c7a62d5aa559affe21c55a07fd4b1fd55fc03a33c610d73426664b20032405d7b92a1414c34d6a
   languageName: node
   linkType: hard
 
 "object.assign@npm:^4.1.4":
-  version: 4.1.4
-  resolution: "object.assign@npm:4.1.4"
+  version: 4.1.5
+  resolution: "object.assign@npm:4.1.5"
   dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.1.4
+    call-bind: ^1.0.5
+    define-properties: ^1.2.1
     has-symbols: ^1.0.3
     object-keys: ^1.1.1
-  checksum: 76cab513a5999acbfe0ff355f15a6a125e71805fcf53de4e9d4e082e1989bdb81d1e329291e1e4e0ae7719f0e4ef80e88fb2d367ae60500d79d25a6224ac8864
+  checksum: f9aeac0541661370a1fc86e6a8065eb1668d3e771f7dbb33ee54578201336c057b21ee61207a186dd42db0c62201d91aac703d20d12a79fc79c353eed44d4e25
   languageName: node
   linkType: hard
 
 "once@npm:^1.3.0":
   version: 1.4.0
   resolution: "once@npm:1.4.0"
   dependencies:
@@ -7856,15 +7938,15 @@
   dependencies:
     error-ex: ^1.3.1
     json-parse-better-errors: ^1.0.1
   checksum: 0fe227d410a61090c247e34fa210552b834613c006c2c64d9a05cfe9e89cf8b4246d1246b1a99524b53b313e9ac024438d0680f67e33eaed7e6f38db64cfe7b5
   languageName: node
   linkType: hard
 
-"parse-json@npm:^5.0.0, parse-json@npm:^5.2.0":
+"parse-json@npm:^5.2.0":
   version: 5.2.0
   resolution: "parse-json@npm:5.2.0"
   dependencies:
     "@babel/code-frame": ^7.0.0
     error-ex: ^1.3.1
     json-parse-even-better-errors: ^2.3.0
     lines-and-columns: ^1.1.6
@@ -7926,15 +8008,15 @@
 "path-parse@npm:^1.0.7":
   version: 1.0.7
   resolution: "path-parse@npm:1.0.7"
   checksum: 49abf3d81115642938a8700ec580da6e830dde670be21893c62f4e10bd7dd4c3742ddc603fe24f898cba7eb0c6bc1777f8d9ac14185d34540c6d4d80cd9cae8a
   languageName: node
   linkType: hard
 
-"path-scurry@npm:^1.10.1, path-scurry@npm:^1.6.1":
+"path-scurry@npm:^1.10.1":
   version: 1.10.1
   resolution: "path-scurry@npm:1.10.1"
   dependencies:
     lru-cache: ^9.1.1 || ^10.0.0
     minipass: ^5.0.0 || ^6.0.2 || ^7.0.0
   checksum: e2557cff3a8fb8bc07afdd6ab163a92587884f9969b05bbbaf6fe7379348bfb09af9ed292af12ed32398b15fb443e81692047b786d1eeb6d898a51eb17ed7d90
   languageName: node
@@ -7998,51 +8080,44 @@
   resolution: "pkg-dir@npm:4.2.0"
   dependencies:
     find-up: ^4.0.0
   checksum: 9863e3f35132bf99ae1636d31ff1e1e3501251d480336edb1c211133c8d58906bed80f154a1d723652df1fda91e01c7442c2eeaf9dc83157c7ae89087e43c8d6
   languageName: node
   linkType: hard
 
-"postcss-media-query-parser@npm:^0.2.3":
-  version: 0.2.3
-  resolution: "postcss-media-query-parser@npm:0.2.3"
-  checksum: 8000d4d95b912994928ff86137f5ab0ed4c4ee1498af2336e93d708ae8827a690cd7acbaed55d14684cf44d82c8d44b031c1c69ae6bcd2f9620ea67573888090
-  languageName: node
-  linkType: hard
-
 "postcss-modules-extract-imports@npm:^3.0.0":
   version: 3.0.0
   resolution: "postcss-modules-extract-imports@npm:3.0.0"
   peerDependencies:
     postcss: ^8.1.0
   checksum: 4b65f2f1382d89c4bc3c0a1bdc5942f52f3cb19c110c57bd591ffab3a5fee03fcf831604168205b0c1b631a3dce2255c70b61aaae3ef39d69cd7eb450c2552d2
   languageName: node
   linkType: hard
 
-"postcss-modules-local-by-default@npm:^4.0.3":
-  version: 4.0.3
-  resolution: "postcss-modules-local-by-default@npm:4.0.3"
+"postcss-modules-local-by-default@npm:^4.0.4":
+  version: 4.0.4
+  resolution: "postcss-modules-local-by-default@npm:4.0.4"
   dependencies:
     icss-utils: ^5.0.0
     postcss-selector-parser: ^6.0.2
     postcss-value-parser: ^4.1.0
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 2f8083687f3d6067885f8863dd32dbbb4f779cfcc7e52c17abede9311d84faf6d3ed8760e7c54c6380281732ae1f78e5e56a28baf3c271b33f450a11c9e30485
+  checksum: 578b955b0773147890caa88c30b10dfc849c5b1412a47ad51751890dba16fca9528c3ab00a19b186a8c2c150c2d08e2ce64d3d907800afee1f37c6d38252e365
   languageName: node
   linkType: hard
 
-"postcss-modules-scope@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "postcss-modules-scope@npm:3.0.0"
+"postcss-modules-scope@npm:^3.1.1":
+  version: 3.1.1
+  resolution: "postcss-modules-scope@npm:3.1.1"
   dependencies:
     postcss-selector-parser: ^6.0.4
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 330b9398dbd44c992c92b0dc612c0626135e2cc840fee41841eb61247a6cfed95af2bd6f67ead9dd9d0bb41f5b0367129d93c6e434fa3e9c58ade391d9a5a138
+  checksum: 9e9d23abb0babc7fa243be65704d72a5a9ceb2bded4dbaef96a88210d468b03c8c3158c197f4e22300c851f08c6fdddd6ebe65f44e4c34448b45b8a2e063a16d
   languageName: node
   linkType: hard
 
 "postcss-modules-values@npm:^4.0.0":
   version: 4.0.0
   resolution: "postcss-modules-values@npm:4.0.0"
   dependencies:
@@ -8065,39 +8140,39 @@
   resolution: "postcss-safe-parser@npm:6.0.0"
   peerDependencies:
     postcss: ^8.3.3
   checksum: 06c733eaad83a3954367e7ee02ddfe3796e7a44d4299ccf9239f40964a4daac153c7d77613f32964b5a86c0c6c2f6167738f31d578b73b17cb69d0c4446f0ebe
   languageName: node
   linkType: hard
 
-"postcss-selector-parser@npm:^6.0.11, postcss-selector-parser@npm:^6.0.2, postcss-selector-parser@npm:^6.0.4":
-  version: 6.0.13
-  resolution: "postcss-selector-parser@npm:6.0.13"
+"postcss-selector-parser@npm:^6.0.13, postcss-selector-parser@npm:^6.0.2, postcss-selector-parser@npm:^6.0.4":
+  version: 6.0.15
+  resolution: "postcss-selector-parser@npm:6.0.15"
   dependencies:
     cssesc: ^3.0.0
     util-deprecate: ^1.0.2
-  checksum: f89163338a1ce3b8ece8e9055cd5a3165e79a15e1c408e18de5ad8f87796b61ec2d48a2902d179ae0c4b5de10fccd3a325a4e660596549b040bc5ad1b465f096
+  checksum: 57decb94152111004f15e27b9c61131eb50ee10a3288e7fcf424cebbb4aba82c2817517ae718f8b5d704ee9e02a638d4a2acff8f47685c295a33ecee4fd31055
   languageName: node
   linkType: hard
 
 "postcss-value-parser@npm:^4.1.0, postcss-value-parser@npm:^4.2.0":
   version: 4.2.0
   resolution: "postcss-value-parser@npm:4.2.0"
   checksum: 819ffab0c9d51cf0acbabf8996dffbfafbafa57afc0e4c98db88b67f2094cb44488758f06e5da95d7036f19556a4a732525e84289a425f4f6fd8e412a9d7442f
   languageName: node
   linkType: hard
 
-"postcss@npm:^8.3.11, postcss@npm:^8.4.19, postcss@npm:^8.4.21":
-  version: 8.4.31
-  resolution: "postcss@npm:8.4.31"
+"postcss@npm:^8.3.11, postcss@npm:^8.4.28, postcss@npm:^8.4.33":
+  version: 8.4.33
+  resolution: "postcss@npm:8.4.33"
   dependencies:
-    nanoid: ^3.3.6
+    nanoid: ^3.3.7
     picocolors: ^1.0.0
     source-map-js: ^1.0.2
-  checksum: 1d8611341b073143ad90486fcdfeab49edd243377b1f51834dc4f6d028e82ce5190e4f11bb2633276864503654fb7cab28e67abdc0fbf9d1f88cad4a0ff0beea
+  checksum: 6f98b2af4b76632a3de20c4f47bf0e984a1ce1a531cf11adcb0b1d63a6cbda0aae4165e578b66c32ca4879038e3eaad386a6be725a8fb4429c78e3c1ab858fe9
   languageName: node
   linkType: hard
 
 "prelude-ls@npm:^1.2.1":
   version: 1.2.1
   resolution: "prelude-ls@npm:1.2.1"
   checksum: cd192ec0d0a8e4c6da3bb80e4f62afe336df3f76271ac6deb0e6a36187133b6073a19e9727a1ff108cd8b9982e4768850d413baa71214dd80c7979617dca827a
@@ -8109,20 +8184,20 @@
   resolution: "prettier-linter-helpers@npm:1.0.0"
   dependencies:
     fast-diff: ^1.1.2
   checksum: 00ce8011cf6430158d27f9c92cfea0a7699405633f7f1d4a45f07e21bf78e99895911cbcdc3853db3a824201a7c745bd49bfea8abd5fb9883e765a90f74f8392
   languageName: node
   linkType: hard
 
-"prettier@npm:^2.8.7":
-  version: 2.8.8
-  resolution: "prettier@npm:2.8.8"
+"prettier@npm:^3.0.0":
+  version: 3.2.4
+  resolution: "prettier@npm:3.2.4"
   bin:
-    prettier: bin-prettier.js
-  checksum: b49e409431bf129dd89238d64299ba80717b57ff5a6d1c1a8b1a28b590d998a34e083fa13573bc732bb8d2305becb4c9a4407f8486c81fa7d55100eb08263cf8
+    prettier: bin/prettier.cjs
+  checksum: 6ec9385a836e0b9bac549e585101c086d1521c31d7b882d5c8bb7d7646da0693da5f31f4fff6dc080710e5e2d34c85e6fb2f8766876b3645c8be2f33b9c3d1a3
   languageName: node
   linkType: hard
 
 "pretty-format@npm:^29.0.0, pretty-format@npm:^29.7.0":
   version: 29.7.0
   resolution: "pretty-format@npm:29.7.0"
   dependencies:
@@ -8209,18 +8284,18 @@
 "queue-microtask@npm:^1.2.2":
   version: 1.2.3
   resolution: "queue-microtask@npm:1.2.3"
   checksum: b676f8c040cdc5b12723ad2f91414d267605b26419d5c821ff03befa817ddd10e238d22b25d604920340fd73efd8ba795465a0377c4adf45a4a41e4234e42dc4
   languageName: node
   linkType: hard
 
-"quick-lru@npm:^4.0.1":
-  version: 4.0.1
-  resolution: "quick-lru@npm:4.0.1"
-  checksum: bea46e1abfaa07023e047d3cf1716a06172c4947886c053ede5c50321893711577cb6119360f810cc3ffcd70c4d7db4069c3cee876b358ceff8596e062bd1154
+"quick-lru@npm:^5.1.1":
+  version: 5.1.1
+  resolution: "quick-lru@npm:5.1.1"
+  checksum: a516faa25574be7947969883e6068dbe4aa19e8ef8e8e0fd96cddd6d36485e9106d85c0041a27153286b0770b381328f4072aa40d3b18a19f5f7d2b78b94b5ed
   languageName: node
   linkType: hard
 
 "randombytes@npm:^2.1.0":
   version: 2.1.0
   resolution: "randombytes@npm:2.1.0"
   dependencies:
@@ -8260,64 +8335,64 @@
   resolution: "react@npm:18.2.0"
   dependencies:
     loose-envify: ^1.1.0
   checksum: 88e38092da8839b830cda6feef2e8505dec8ace60579e46aa5490fc3dc9bba0bd50336507dc166f43e3afc1c42939c09fe33b25fae889d6f402721dcd78fca1b
   languageName: node
   linkType: hard
 
-"read-pkg-up@npm:^7.0.1":
-  version: 7.0.1
-  resolution: "read-pkg-up@npm:7.0.1"
+"read-pkg-up@npm:^8.0.0":
+  version: 8.0.0
+  resolution: "read-pkg-up@npm:8.0.0"
   dependencies:
-    find-up: ^4.1.0
-    read-pkg: ^5.2.0
-    type-fest: ^0.8.1
-  checksum: e4e93ce70e5905b490ca8f883eb9e48b5d3cebc6cd4527c25a0d8f3ae2903bd4121c5ab9c5a3e217ada0141098eeb661313c86fa008524b089b8ed0b7f165e44
+    find-up: ^5.0.0
+    read-pkg: ^6.0.0
+    type-fest: ^1.0.1
+  checksum: fe4c80401656b40b408884457fffb5a8015c03b1018cfd8e48f8d82a5e9023e24963603aeb2755608d964593e046c15b34d29b07d35af9c7aa478be81805209c
   languageName: node
   linkType: hard
 
 "read-pkg@npm:^3.0.0":
   version: 3.0.0
   resolution: "read-pkg@npm:3.0.0"
   dependencies:
     load-json-file: ^4.0.0
     normalize-package-data: ^2.3.2
     path-type: ^3.0.0
   checksum: 398903ebae6c7e9965419a1062924436cc0b6f516c42c4679a90290d2f87448ed8f977e7aa2dbba4aa1ac09248628c43e493ac25b2bc76640e946035200e34c6
   languageName: node
   linkType: hard
 
-"read-pkg@npm:^5.2.0":
-  version: 5.2.0
-  resolution: "read-pkg@npm:5.2.0"
+"read-pkg@npm:^6.0.0":
+  version: 6.0.0
+  resolution: "read-pkg@npm:6.0.0"
   dependencies:
     "@types/normalize-package-data": ^2.4.0
-    normalize-package-data: ^2.5.0
-    parse-json: ^5.0.0
-    type-fest: ^0.6.0
-  checksum: eb696e60528b29aebe10e499ba93f44991908c57d70f2d26f369e46b8b9afc208ef11b4ba64f67630f31df8b6872129e0a8933c8c53b7b4daf0eace536901222
+    normalize-package-data: ^3.0.2
+    parse-json: ^5.2.0
+    type-fest: ^1.0.1
+  checksum: 0cebdff381128e923815c643074a87011070e5fc352bee575d327d6485da3317fab6d802a7b03deeb0be7be8d3ad1640397b3d5d2f044452caf4e8d1736bf94f
   languageName: node
   linkType: hard
 
 "rechoir@npm:^0.8.0":
   version: 0.8.0
   resolution: "rechoir@npm:0.8.0"
   dependencies:
     resolve: ^1.20.0
   checksum: ad3caed8afdefbc33fbc30e6d22b86c35b3d51c2005546f4e79bcc03c074df804b3640ad18945e6bef9ed12caedc035655ec1082f64a5e94c849ff939dc0a788
   languageName: node
   linkType: hard
 
-"redent@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "redent@npm:3.0.0"
+"redent@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "redent@npm:4.0.0"
   dependencies:
-    indent-string: ^4.0.0
-    strip-indent: ^3.0.0
-  checksum: fa1ef20404a2d399235e83cc80bd55a956642e37dd197b4b612ba7327bf87fa32745aeb4a1634b2bab25467164ab4ed9c15be2c307923dd08b0fe7c52431ae6b
+    indent-string: ^5.0.0
+    strip-indent: ^4.0.0
+  checksum: 6944e7b1d8f3fd28c2515f5c605b9f7f0ea0f4edddf41890bbbdd4d9ee35abb7540c3b278f03ff827bd278bb6ff4a5bd8692ca406b748c5c1c3ce7355e9fbf8f
   languageName: node
   linkType: hard
 
 "regenerate-unicode-properties@npm:^10.1.0":
   version: 10.1.1
   resolution: "regenerate-unicode-properties@npm:10.1.1"
   dependencies:
@@ -8330,17 +8405,17 @@
   version: 1.4.2
   resolution: "regenerate@npm:1.4.2"
   checksum: 3317a09b2f802da8db09aa276e469b57a6c0dd818347e05b8862959c6193408242f150db5de83c12c3fa99091ad95fb42a6db2c3329bfaa12a0ea4cbbeb30cb0
   languageName: node
   linkType: hard
 
 "regenerator-runtime@npm:^0.14.0":
-  version: 0.14.0
-  resolution: "regenerator-runtime@npm:0.14.0"
-  checksum: 1c977ad82a82a4412e4f639d65d22be376d3ebdd30da2c003eeafdaaacd03fc00c2320f18120007ee700900979284fc78a9f00da7fb593f6e6eeebc673fba9a3
+  version: 0.14.1
+  resolution: "regenerator-runtime@npm:0.14.1"
+  checksum: 9f57c93277b5585d3c83b0cf76be47b473ae8c6d9142a46ce8b0291a04bb2cf902059f0f8445dcabb3fb7378e5fe4bb4ea1e008876343d42e46d3b484534ce38
   languageName: node
   linkType: hard
 
 "regenerator-transform@npm:^0.15.2":
   version: 0.15.2
   resolution: "regenerator-transform@npm:0.15.2"
   dependencies:
@@ -8483,61 +8558,61 @@
     glob: ^7.1.3
   bin:
     rimraf: bin.js
   checksum: 87f4164e396f0171b0a3386cc1877a817f572148ee13a7e113b238e48e8a9f2f31d009a92ec38a591ff1567d9662c6b67fd8818a2dbbaed74bc26a87a2a4a9a0
   languageName: node
   linkType: hard
 
-"rimraf@npm:^4.4.1":
-  version: 4.4.1
-  resolution: "rimraf@npm:4.4.1"
+"rimraf@npm:^5.0.1":
+  version: 5.0.5
+  resolution: "rimraf@npm:5.0.5"
   dependencies:
-    glob: ^9.2.0
+    glob: ^10.3.7
   bin:
-    rimraf: dist/cjs/src/bin.js
-  checksum: b786adc02651e2e24bbedb04bbdea80652fc9612632931ff2d9f898c5e4708fe30956186597373c568bd5230a4dc2fadfc816ccacba8a1daded3a006a6b74f1a
+    rimraf: dist/esm/bin.mjs
+  checksum: d66eef829b2e23b16445f34e73d75c7b7cf4cbc8834b04720def1c8f298eb0753c3d76df77325fad79d0a2c60470525d95f89c2475283ad985fd7441c32732d1
   languageName: node
   linkType: hard
 
 "run-parallel@npm:^1.1.9":
   version: 1.2.0
   resolution: "run-parallel@npm:1.2.0"
   dependencies:
     queue-microtask: ^1.2.2
   checksum: cb4f97ad25a75ebc11a8ef4e33bb962f8af8516bb2001082ceabd8902e15b98f4b84b4f8a9b222e5d57fc3bd1379c483886ed4619367a7680dad65316993021d
   languageName: node
   linkType: hard
 
 "safe-array-concat@npm:^1.0.1":
-  version: 1.0.1
-  resolution: "safe-array-concat@npm:1.0.1"
+  version: 1.1.0
+  resolution: "safe-array-concat@npm:1.1.0"
   dependencies:
-    call-bind: ^1.0.2
-    get-intrinsic: ^1.2.1
+    call-bind: ^1.0.5
+    get-intrinsic: ^1.2.2
     has-symbols: ^1.0.3
     isarray: ^2.0.5
-  checksum: 001ecf1d8af398251cbfabaf30ed66e3855127fbceee178179524b24160b49d15442f94ed6c0db0b2e796da76bb05b73bf3cc241490ec9c2b741b41d33058581
+  checksum: 5c71eaa999168ee7474929f1cd3aae80f486353a651a094d9968936692cf90aa065224929a6486dcda66334a27dce4250a83612f9e0fef6dced1a925d3ac7296
   languageName: node
   linkType: hard
 
 "safe-buffer@npm:^5.1.0":
   version: 5.2.1
   resolution: "safe-buffer@npm:5.2.1"
   checksum: b99c4b41fdd67a6aaf280fcd05e9ffb0813654894223afb78a31f14a19ad220bba8aba1cb14eddce1fcfb037155fe6de4e861784eb434f7d11ed58d1e70dd491
   languageName: node
   linkType: hard
 
 "safe-regex-test@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "safe-regex-test@npm:1.0.0"
+  version: 1.0.2
+  resolution: "safe-regex-test@npm:1.0.2"
   dependencies:
-    call-bind: ^1.0.2
-    get-intrinsic: ^1.1.3
+    call-bind: ^1.0.5
+    get-intrinsic: ^1.2.2
     is-regex: ^1.1.4
-  checksum: bc566d8beb8b43c01b94e67de3f070fd2781685e835959bbbaaec91cc53381145ca91f69bd837ce6ec244817afa0a5e974fc4e40a2957f0aca68ac3add1ddd34
+  checksum: 4af5ce05a2daa4f6d4bfd5a3c64fc33d6b886f6592122e93c0efad52f7147b9b605e5ffc03c269a1e3d1f8db2a23bc636628a961c9fd65bafdc09503330673fd
   languageName: node
   linkType: hard
 
 "safer-buffer@npm:>= 2.1.2 < 3.0.0":
   version: 2.1.2
   resolution: "safer-buffer@npm:2.1.2"
   checksum: cab8f25ae6f1434abee8d80023d7e72b598cf1327164ddab31003c51215526801e40b66c5e65d658a0af1e9d6478cadcb4c745f4bd6751f97d8644786c0978b0
@@ -8624,43 +8699,44 @@
   resolution: "semver@npm:6.3.1"
   bin:
     semver: bin/semver.js
   checksum: ae47d06de28836adb9d3e25f22a92943477371292d9b665fb023fae278d345d508ca1958232af086d85e0155aee22e313e100971898bbb8d5d89b8b1d4054ca2
   languageName: node
   linkType: hard
 
-"semver@npm:^7.3.4, semver@npm:^7.3.5, semver@npm:^7.3.7, semver@npm:^7.3.8, semver@npm:^7.5.3, semver@npm:^7.5.4":
+"semver@npm:^7.3.4, semver@npm:^7.3.5, semver@npm:^7.5.3, semver@npm:^7.5.4":
   version: 7.5.4
   resolution: "semver@npm:7.5.4"
   dependencies:
     lru-cache: ^6.0.0
   bin:
     semver: bin/semver.js
   checksum: 12d8ad952fa353b0995bf180cdac205a4068b759a140e5d3c608317098b3575ac2f1e09182206bf2eb26120e1c0ed8fb92c48c592f6099680de56bb071423ca3
   languageName: node
   linkType: hard
 
 "serialize-javascript@npm:^6.0.1":
-  version: 6.0.1
-  resolution: "serialize-javascript@npm:6.0.1"
+  version: 6.0.2
+  resolution: "serialize-javascript@npm:6.0.2"
   dependencies:
     randombytes: ^2.1.0
-  checksum: 3c4f4cb61d0893b988415bdb67243637333f3f574e9e9cc9a006a2ced0b390b0b3b44aef8d51c951272a9002ec50885eefdc0298891bc27eb2fe7510ea87dc4f
+  checksum: c4839c6206c1d143c0f80763997a361310305751171dd95e4b57efee69b8f6edd8960a0b7fbfc45042aadff98b206d55428aee0dc276efe54f100899c7fa8ab7
   languageName: node
   linkType: hard
 
 "set-function-length@npm:^1.1.1":
-  version: 1.1.1
-  resolution: "set-function-length@npm:1.1.1"
+  version: 1.2.0
+  resolution: "set-function-length@npm:1.2.0"
   dependencies:
     define-data-property: ^1.1.1
-    get-intrinsic: ^1.2.1
+    function-bind: ^1.1.2
+    get-intrinsic: ^1.2.2
     gopd: ^1.0.1
-    has-property-descriptors: ^1.0.0
-  checksum: c131d7569cd7e110cafdfbfbb0557249b538477624dfac4fc18c376d879672fa52563b74029ca01f8f4583a8acb35bb1e873d573a24edb80d978a7ee607c6e06
+    has-property-descriptors: ^1.0.1
+  checksum: 63e34b45a2ff9abb419f52583481bf8ba597d33c0c85e56999085eb6078a0f7fbb4222051981c287feceeb358aa7789e7803cea2c82ac94c0ab37059596aff79
   languageName: node
   linkType: hard
 
 "set-function-name@npm:^2.0.0":
   version: 2.0.1
   resolution: "set-function-name@npm:2.0.1"
   dependencies:
@@ -8809,15 +8885,15 @@
 "source-list-map@npm:^2.0.0":
   version: 2.0.1
   resolution: "source-list-map@npm:2.0.1"
   checksum: 806efc6f75e7cd31e4815e7a3aaf75a45c704871ea4075cb2eb49882c6fca28998f44fc5ac91adb6de03b2882ee6fb02f951fdc85e6a22b338c32bfe19557938
   languageName: node
   linkType: hard
 
-"source-map-js@npm:^1.0.2":
+"source-map-js@npm:^1.0.1, source-map-js@npm:^1.0.2":
   version: 1.0.2
   resolution: "source-map-js@npm:1.0.2"
   checksum: c049a7fc4deb9a7e9b481ae3d424cc793cb4845daa690bc5a05d428bf41bf231ced49b4cf0c9e77f9d42fdb3d20d6187619fc586605f5eabe995a316da8d377c
   languageName: node
   linkType: hard
 
 "source-map-loader@npm:^1.0.2":
@@ -8885,17 +8961,17 @@
     spdx-expression-parse: ^3.0.0
     spdx-license-ids: ^3.0.0
   checksum: e9ae98d22f69c88e7aff5b8778dc01c361ef635580e82d29e5c60a6533cc8f4d820803e67d7432581af0cc4fb49973125076ee3b90df191d153e223c004193b2
   languageName: node
   linkType: hard
 
 "spdx-exceptions@npm:^2.1.0":
-  version: 2.3.0
-  resolution: "spdx-exceptions@npm:2.3.0"
-  checksum: cb69a26fa3b46305637123cd37c85f75610e8c477b6476fa7354eb67c08128d159f1d36715f19be6f9daf4b680337deb8c65acdcae7f2608ba51931540687ac0
+  version: 2.4.0
+  resolution: "spdx-exceptions@npm:2.4.0"
+  checksum: b1b650a8d94424473bf9629cf972c86a91c03cccc260f5c901bce0e4b92d831627fec28c9e0a1e9c34c5ebad0a12cf2eab887bec088e0a862abb9d720c2fd0a1
   languageName: node
   linkType: hard
 
 "spdx-expression-parse@npm:^3.0.0":
   version: 3.0.1
   resolution: "spdx-expression-parse@npm:3.0.1"
   dependencies:
@@ -9048,36 +9124,36 @@
 "strip-final-newline@npm:^2.0.0":
   version: 2.0.0
   resolution: "strip-final-newline@npm:2.0.0"
   checksum: 69412b5e25731e1938184b5d489c32e340605bb611d6140344abc3421b7f3c6f9984b21dff296dfcf056681b82caa3bb4cc996a965ce37bcfad663e92eae9c64
   languageName: node
   linkType: hard
 
-"strip-indent@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "strip-indent@npm:3.0.0"
+"strip-indent@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "strip-indent@npm:4.0.0"
   dependencies:
-    min-indent: ^1.0.0
-  checksum: 18f045d57d9d0d90cd16f72b2313d6364fd2cb4bf85b9f593523ad431c8720011a4d5f08b6591c9d580f446e78855c5334a30fb91aa1560f5d9f95ed1b4a0530
+    min-indent: ^1.0.1
+  checksum: 06cbcd93da721c46bc13caeb1c00af93a9b18146a1c95927672d2decab6a25ad83662772417cea9317a2507fb143253ecc23c4415b64f5828cef9b638a744598
   languageName: node
   linkType: hard
 
 "strip-json-comments@npm:^3.1.1":
   version: 3.1.1
   resolution: "strip-json-comments@npm:3.1.1"
   checksum: 492f73e27268f9b1c122733f28ecb0e7e8d8a531a6662efbd08e22cccb3f9475e90a1b82cab06a392f6afae6d2de636f977e231296400d0ec5304ba70f166443
   languageName: node
   linkType: hard
 
 "style-loader@npm:^3.3.1, style-loader@npm:~3.3.1":
-  version: 3.3.3
-  resolution: "style-loader@npm:3.3.3"
+  version: 3.3.4
+  resolution: "style-loader@npm:3.3.4"
   peerDependencies:
     webpack: ^5.0.0
-  checksum: f59c953f56f6a935bd6a1dfa409f1128fed2b66b48ce4a7a75b85862a7156e5e90ab163878962762f528ec4d510903d828da645e143fbffd26f055dc1c094078
+  checksum: caac3f2fe2c3c89e49b7a2a9329e1cfa515ecf5f36b9c4885f9b218019fda207a9029939b2c35821dec177a264a007e7c391ccdd3ff7401881ce6287b9c8f38b
   languageName: node
   linkType: hard
 
 "style-mod@npm:^4.0.0, style-mod@npm:^4.1.0":
   version: 4.1.0
   resolution: "style-mod@npm:4.1.0"
   checksum: 8402b14ca11113a3640d46b3cf7ba49f05452df7846bc5185a3535d9b6a64a3019e7fb636b59ccbb7816aeb0725b24723e77a85b05612a9360e419958e13b4e6
@@ -9087,103 +9163,104 @@
 "style-search@npm:^0.1.0":
   version: 0.1.0
   resolution: "style-search@npm:0.1.0"
   checksum: 3cfefe335033aad6d47da0725cb48f5db91a73935954c77eab77d9e415e6668cdb406da4a4f7ef9f1aca77853cf5ba7952c45e869caa5bd6439691d88098d468
   languageName: node
   linkType: hard
 
-"stylelint-config-prettier@npm:^9.0.4":
-  version: 9.0.5
-  resolution: "stylelint-config-prettier@npm:9.0.5"
+"stylelint-config-recommended@npm:^13.0.0":
+  version: 13.0.0
+  resolution: "stylelint-config-recommended@npm:13.0.0"
   peerDependencies:
-    stylelint: ">= 11.x < 15"
-  bin:
-    stylelint-config-prettier: bin/check.js
-    stylelint-config-prettier-check: bin/check.js
-  checksum: 3d04e463e0bb7e42a5ddec49eea6ef4ea07705d887e8a3ff1fcb82278a5e2bec1a36b8498ea7ed2d24878de29d7c94ac75b1d3ac4f8b19c3a84970595b29261f
+    stylelint: ^15.10.0
+  checksum: a56eb6d1a7c7f3a7a172b54bc34218859ba22a5a06816fb4d0964f66cb83cf372062f2c97830e994ad68243548e15fc49abf28887c3261ab1b471b3aa69f8e82
   languageName: node
   linkType: hard
 
-"stylelint-config-recommended@npm:^8.0.0":
-  version: 8.0.0
-  resolution: "stylelint-config-recommended@npm:8.0.0"
+"stylelint-config-standard@npm:^34.0.0":
+  version: 34.0.0
+  resolution: "stylelint-config-standard@npm:34.0.0"
+  dependencies:
+    stylelint-config-recommended: ^13.0.0
   peerDependencies:
-    stylelint: ^14.8.0
-  checksum: 0c5ca94625e5308a7afb8315bb350a2b48f46fdd8d8922dd9a8c2e37b3407f2294794d930726ad6bf2007abcde1abd34084808cf83adf150efe3a643e0eb5ac4
+    stylelint: ^15.10.0
+  checksum: 536249800c04b48a9c354067765f042713982e8222be17bb897a27d26546e50adfb87e6f1e4541807d720de3554345da99ab470e13e8d7ab0ab326c73ae3df61
   languageName: node
   linkType: hard
 
-"stylelint-config-standard@npm:^26.0.0":
-  version: 26.0.0
-  resolution: "stylelint-config-standard@npm:26.0.0"
+"stylelint-csstree-validator@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "stylelint-csstree-validator@npm:3.0.0"
   dependencies:
-    stylelint-config-recommended: ^8.0.0
+    css-tree: ^2.3.1
   peerDependencies:
-    stylelint: ^14.9.0
-  checksum: c1fe44df1755bcccc740b385a24acffa922d331d9f9ba39dafad81cc9643e6c1f870abd1ee73b2737d6903e06efb83b2a1ee26d786faef0123fc22e1f09c13fe
+    stylelint: ">=7.0.0 <16.0.0"
+  checksum: e518c8c17714022946b7637c23a6816fd2ccdd6052a19c5a138b3f7ce9b913ead9c612ac4401e102f14800a19967dbfd4b588b44cbf3f3c6a5984bef7bda4017
   languageName: node
   linkType: hard
 
-"stylelint-prettier@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "stylelint-prettier@npm:2.0.0"
+"stylelint-prettier@npm:^4.0.0":
+  version: 4.1.0
+  resolution: "stylelint-prettier@npm:4.1.0"
   dependencies:
     prettier-linter-helpers: ^1.0.0
   peerDependencies:
-    prettier: ">=2.0.0"
-    stylelint: ">=14.0.0"
-  checksum: 6ce7628517a492e0c2e6104f654c9bc710f1aaf035c8b5274e187b68e8d510e70bae5ded2cb65df76aa01096460b9dfe02f844fea13bfba7e3dcca13baec2ff4
+    prettier: ">=3.0.0"
+    stylelint: ">=15.8.0"
+  checksum: bbeb7e0dd49099c43297e88a61385b39f4b5810c8bfcc972d5b2706b6a7e14a8eefd5f9e623841cf3127111a8859eb624a3e7cc1bc5197c83c55c6c9a616a4d2
   languageName: node
   linkType: hard
 
-"stylelint@npm:^14.9.1":
-  version: 14.16.1
-  resolution: "stylelint@npm:14.16.1"
+"stylelint@npm:^15.10.1":
+  version: 15.11.0
+  resolution: "stylelint@npm:15.11.0"
   dependencies:
-    "@csstools/selector-specificity": ^2.0.2
+    "@csstools/css-parser-algorithms": ^2.3.1
+    "@csstools/css-tokenizer": ^2.2.0
+    "@csstools/media-query-list-parser": ^2.1.4
+    "@csstools/selector-specificity": ^3.0.0
     balanced-match: ^2.0.0
     colord: ^2.9.3
-    cosmiconfig: ^7.1.0
-    css-functions-list: ^3.1.0
+    cosmiconfig: ^8.2.0
+    css-functions-list: ^3.2.1
+    css-tree: ^2.3.1
     debug: ^4.3.4
-    fast-glob: ^3.2.12
+    fast-glob: ^3.3.1
     fastest-levenshtein: ^1.0.16
-    file-entry-cache: ^6.0.1
+    file-entry-cache: ^7.0.0
     global-modules: ^2.0.0
     globby: ^11.1.0
     globjoin: ^0.1.4
-    html-tags: ^3.2.0
-    ignore: ^5.2.1
+    html-tags: ^3.3.1
+    ignore: ^5.2.4
     import-lazy: ^4.0.0
     imurmurhash: ^0.1.4
     is-plain-object: ^5.0.0
-    known-css-properties: ^0.26.0
+    known-css-properties: ^0.29.0
     mathml-tag-names: ^2.1.3
-    meow: ^9.0.0
+    meow: ^10.1.5
     micromatch: ^4.0.5
     normalize-path: ^3.0.0
     picocolors: ^1.0.0
-    postcss: ^8.4.19
-    postcss-media-query-parser: ^0.2.3
+    postcss: ^8.4.28
     postcss-resolve-nested-selector: ^0.1.1
     postcss-safe-parser: ^6.0.0
-    postcss-selector-parser: ^6.0.11
+    postcss-selector-parser: ^6.0.13
     postcss-value-parser: ^4.2.0
     resolve-from: ^5.0.0
     string-width: ^4.2.3
     strip-ansi: ^6.0.1
     style-search: ^0.1.0
-    supports-hyperlinks: ^2.3.0
+    supports-hyperlinks: ^3.0.0
     svg-tags: ^1.0.0
     table: ^6.8.1
-    v8-compile-cache: ^2.3.0
-    write-file-atomic: ^4.0.2
+    write-file-atomic: ^5.0.1
   bin:
-    stylelint: bin/stylelint.js
-  checksum: bc24050415e3c357a76d8ca2799e74ce31f33c9158b4086462512b0191db5d6a161b81ef35b064039c6eacf98a5553e45fca4c5f21eb4d45e7f1d44b2d226e9b
+    stylelint: bin/stylelint.mjs
+  checksum: 9835f8a3e3976a3b81a35569d08f5f4a9c3b5cff415f1345a505870afc0c3231acff27f119d937c5bb11fdbc98d554af564c2a648a52604280a59a11974fcbfc
   languageName: node
   linkType: hard
 
 "supports-color@npm:^5.3.0":
   version: 5.5.0
   resolution: "supports-color@npm:5.5.0"
   dependencies:
@@ -9206,21 +9283,21 @@
   resolution: "supports-color@npm:8.1.1"
   dependencies:
     has-flag: ^4.0.0
   checksum: c052193a7e43c6cdc741eb7f378df605636e01ad434badf7324f17fb60c69a880d8d8fcdcb562cf94c2350e57b937d7425ab5b8326c67c2adc48f7c87c1db406
   languageName: node
   linkType: hard
 
-"supports-hyperlinks@npm:^2.3.0":
-  version: 2.3.0
-  resolution: "supports-hyperlinks@npm:2.3.0"
+"supports-hyperlinks@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "supports-hyperlinks@npm:3.0.0"
   dependencies:
     has-flag: ^4.0.0
     supports-color: ^7.0.0
-  checksum: 9ee0de3c8ce919d453511b2b1588a8205bd429d98af94a01df87411391010fe22ca463f268c84b2ce2abad019dfff8452aa02806eeb5c905a8d7ad5c4f4c52b8
+  checksum: 41021305de5255b10d821bf93c7a781f783e1693d0faec293d7fc7ccf17011b90bde84b0295fa92ba75c6c390351fe84fdd18848cad4bf656e464a958243c3e7
   languageName: node
   linkType: hard
 
 "supports-preserve-symlinks-flag@npm:^1.0.0":
   version: 1.0.0
   resolution: "supports-preserve-symlinks-flag@npm:1.0.0"
   checksum: 53b1e247e68e05db7b3808b99b892bd36fb096e6fba213a06da7fab22045e97597db425c724f2bbd6c99a3c295e1e73f3e4de78592289f38431049e1277ca0ae
@@ -9237,14 +9314,24 @@
 "symbol-tree@npm:^3.2.4":
   version: 3.2.4
   resolution: "symbol-tree@npm:3.2.4"
   checksum: 6e8fc7e1486b8b54bea91199d9535bb72f10842e40c79e882fc94fb7b14b89866adf2fd79efa5ebb5b658bc07fb459ccce5ac0e99ef3d72f474e74aaf284029d
   languageName: node
   linkType: hard
 
+"synckit@npm:^0.8.6":
+  version: 0.8.8
+  resolution: "synckit@npm:0.8.8"
+  dependencies:
+    "@pkgr/core": ^0.1.0
+    tslib: ^2.6.2
+  checksum: 9ed5d33abb785f5f24e2531efd53b2782ca77abf7912f734d170134552b99001915531be5a50297aa45c5701b5c9041e8762e6cd7a38e41e2461c1e7fccdedf8
+  languageName: node
+  linkType: hard
+
 "table@npm:^6.8.1":
   version: 6.8.1
   resolution: "table@npm:6.8.1"
   dependencies:
     ajv: ^8.0.1
     lodash.truncate: ^4.4.2
     slice-ansi: ^4.0.0
@@ -9271,47 +9358,47 @@
     minizlib: ^2.1.1
     mkdirp: ^1.0.3
     yallist: ^4.0.0
   checksum: db4d9fe74a2082c3a5016630092c54c8375ff3b280186938cfd104f2e089c4fd9bad58688ef6be9cf186a889671bf355c7cda38f09bbf60604b281715ca57f5c
   languageName: node
   linkType: hard
 
-"terser-webpack-plugin@npm:^5.3.7":
-  version: 5.3.9
-  resolution: "terser-webpack-plugin@npm:5.3.9"
+"terser-webpack-plugin@npm:^5.3.10, terser-webpack-plugin@npm:^5.3.7":
+  version: 5.3.10
+  resolution: "terser-webpack-plugin@npm:5.3.10"
   dependencies:
-    "@jridgewell/trace-mapping": ^0.3.17
+    "@jridgewell/trace-mapping": ^0.3.20
     jest-worker: ^27.4.5
     schema-utils: ^3.1.1
     serialize-javascript: ^6.0.1
-    terser: ^5.16.8
+    terser: ^5.26.0
   peerDependencies:
     webpack: ^5.1.0
   peerDependenciesMeta:
     "@swc/core":
       optional: true
     esbuild:
       optional: true
     uglify-js:
       optional: true
-  checksum: 41705713d6f9cb83287936b21e27c658891c78c4392159f5148b5623f0e8c48559869779619b058382a4c9758e7820ea034695e57dc7c474b4962b79f553bc5f
+  checksum: bd6e7596cf815f3353e2a53e79cbdec959a1b0276f5e5d4e63e9d7c3c5bb5306df567729da287d1c7b39d79093e56863c569c42c6c24cc34c76aa313bd2cbcea
   languageName: node
   linkType: hard
 
-"terser@npm:^5.16.8":
-  version: 5.24.0
-  resolution: "terser@npm:5.24.0"
+"terser@npm:^5.26.0":
+  version: 5.27.0
+  resolution: "terser@npm:5.27.0"
   dependencies:
     "@jridgewell/source-map": ^0.3.3
     acorn: ^8.8.2
     commander: ^2.20.0
     source-map-support: ~0.5.20
   bin:
     terser: bin/terser
-  checksum: d88f774b6fa711a234fcecefd7657f99189c367e17dbe95a51c2776d426ad0e4d98d1ffe6edfdf299877c7602e495bdd711d21b2caaec188410795e5447d0f6c
+  checksum: c165052cfea061e8512e9b9ba42a098c2ff6382886ae122b040fd5b6153443070cc2dcb4862269f1669c09c716763e856125a355ff984aa72be525d6fffd8729
   languageName: node
   linkType: hard
 
 "test-exclude@npm:^6.0.0":
   version: 6.0.0
   resolution: "test-exclude@npm:6.0.0"
   dependencies:
@@ -9385,24 +9472,33 @@
 "tr46@npm:~0.0.3":
   version: 0.0.3
   resolution: "tr46@npm:0.0.3"
   checksum: 726321c5eaf41b5002e17ffbd1fb7245999a073e8979085dacd47c4b4e8068ff5777142fc6726d6ca1fd2ff16921b48788b87225cbc57c72636f6efa8efbffe3
   languageName: node
   linkType: hard
 
-"trim-newlines@npm:^3.0.0":
-  version: 3.0.1
-  resolution: "trim-newlines@npm:3.0.1"
-  checksum: b530f3fadf78e570cf3c761fb74fef655beff6b0f84b29209bac6c9622db75ad1417f4a7b5d54c96605dcd72734ad44526fef9f396807b90839449eb543c6206
+"trim-newlines@npm:^4.0.2":
+  version: 4.1.1
+  resolution: "trim-newlines@npm:4.1.1"
+  checksum: 5b09f8e329e8f33c1111ef26906332ba7ba7248cde3e26fc054bb3d69f2858bf5feedca9559c572ff91f33e52977c28e0d41c387df6a02a633cbb8c2d8238627
+  languageName: node
+  linkType: hard
+
+"ts-api-utils@npm:^1.0.1":
+  version: 1.0.3
+  resolution: "ts-api-utils@npm:1.0.3"
+  peerDependencies:
+    typescript: ">=4.2.0"
+  checksum: 441cc4489d65fd515ae6b0f4eb8690057add6f3b6a63a36073753547fb6ce0c9ea0e0530220a0b282b0eec535f52c4dfc315d35f8a4c9a91c0def0707a714ca6
   languageName: node
   linkType: hard
 
 "ts-jest@npm:^29.1.0":
-  version: 29.1.1
-  resolution: "ts-jest@npm:29.1.1"
+  version: 29.1.2
+  resolution: "ts-jest@npm:29.1.2"
   dependencies:
     bs-logger: 0.x
     fast-json-stable-stringify: 2.x
     jest-util: ^29.0.0
     json5: ^2.2.3
     lodash.memoize: 4.x
     make-error: 1.x
@@ -9421,33 +9517,22 @@
       optional: true
     babel-jest:
       optional: true
     esbuild:
       optional: true
   bin:
     ts-jest: cli.js
-  checksum: a8c9e284ed4f819526749f6e4dc6421ec666f20ab44d31b0f02b4ed979975f7580b18aea4813172d43e39b29464a71899f8893dd29b06b4a351a3af8ba47b402
-  languageName: node
-  linkType: hard
-
-"tslib@npm:^1.8.1":
-  version: 1.14.1
-  resolution: "tslib@npm:1.14.1"
-  checksum: dbe628ef87f66691d5d2959b3e41b9ca0045c3ee3c7c7b906cc1e328b39f199bb1ad9e671c39025bd56122ac57dfbf7385a94843b1cc07c60a4db74795829acd
+  checksum: a0ce0affc1b716c78c9ab55837829c42cb04b753d174a5c796bb1ddf9f0379fc20647b76fbe30edb30d9b23181908138d6b4c51ef2ae5e187b66635c295cefd5
   languageName: node
   linkType: hard
 
-"tsutils@npm:^3.21.0":
-  version: 3.21.0
-  resolution: "tsutils@npm:3.21.0"
-  dependencies:
-    tslib: ^1.8.1
-  peerDependencies:
-    typescript: ">=2.8.0 || >= 3.2.0-dev || >= 3.3.0-dev || >= 3.4.0-dev || >= 3.5.0-dev || >= 3.6.0-dev || >= 3.6.0-beta || >= 3.7.0-dev || >= 3.7.0-beta"
-  checksum: 1843f4c1b2e0f975e08c4c21caa4af4f7f65a12ac1b81b3b8489366826259323feb3fc7a243123453d2d1a02314205a7634e048d4a8009921da19f99755cdc48
+"tslib@npm:^2.6.2":
+  version: 2.6.2
+  resolution: "tslib@npm:2.6.2"
+  checksum: 329ea56123005922f39642318e3d1f0f8265d1e7fcb92c633e0809521da75eeaca28d2cf96d7248229deb40e5c19adf408259f4b9640afd20d13aecc1430f3ad
   languageName: node
   linkType: hard
 
 "type-check@npm:^0.4.0, type-check@npm:~0.4.0":
   version: 0.4.0
   resolution: "type-check@npm:0.4.0"
   dependencies:
@@ -9459,46 +9544,32 @@
 "type-detect@npm:4.0.8":
   version: 4.0.8
   resolution: "type-detect@npm:4.0.8"
   checksum: 62b5628bff67c0eb0b66afa371bd73e230399a8d2ad30d852716efcc4656a7516904570cd8631a49a3ce57c10225adf5d0cbdcb47f6b0255fe6557c453925a15
   languageName: node
   linkType: hard
 
-"type-fest@npm:^0.18.0":
-  version: 0.18.1
-  resolution: "type-fest@npm:0.18.1"
-  checksum: e96dcee18abe50ec82dab6cbc4751b3a82046da54c52e3b2d035b3c519732c0b3dd7a2fa9df24efd1a38d953d8d4813c50985f215f1957ee5e4f26b0fe0da395
-  languageName: node
-  linkType: hard
-
 "type-fest@npm:^0.20.2":
   version: 0.20.2
   resolution: "type-fest@npm:0.20.2"
   checksum: 4fb3272df21ad1c552486f8a2f8e115c09a521ad7a8db3d56d53718d0c907b62c6e9141ba5f584af3f6830d0872c521357e512381f24f7c44acae583ad517d73
   languageName: node
   linkType: hard
 
 "type-fest@npm:^0.21.3":
   version: 0.21.3
   resolution: "type-fest@npm:0.21.3"
   checksum: e6b32a3b3877f04339bae01c193b273c62ba7bfc9e325b8703c4ee1b32dc8fe4ef5dfa54bf78265e069f7667d058e360ae0f37be5af9f153b22382cd55a9afe0
   languageName: node
   linkType: hard
 
-"type-fest@npm:^0.6.0":
-  version: 0.6.0
-  resolution: "type-fest@npm:0.6.0"
-  checksum: b2188e6e4b21557f6e92960ec496d28a51d68658018cba8b597bd3ef757721d1db309f120ae987abeeda874511d14b776157ff809f23c6d1ce8f83b9b2b7d60f
-  languageName: node
-  linkType: hard
-
-"type-fest@npm:^0.8.1":
-  version: 0.8.1
-  resolution: "type-fest@npm:0.8.1"
-  checksum: d61c4b2eba24009033ae4500d7d818a94fd6d1b481a8111612ee141400d5f1db46f199c014766b9fa9b31a6a7374d96fc748c6d688a78a3ce5a33123839becb7
+"type-fest@npm:^1.0.1, type-fest@npm:^1.2.1, type-fest@npm:^1.2.2":
+  version: 1.4.0
+  resolution: "type-fest@npm:1.4.0"
+  checksum: b011c3388665b097ae6a109a437a04d6f61d81b7357f74cbcb02246f2f5bd72b888ae33631b99871388122ba0a87f4ff1c94078e7119ff22c70e52c0ff828201
   languageName: node
   linkType: hard
 
 "typed-array-buffer@npm:^1.0.0":
   version: 1.0.0
   resolution: "typed-array-buffer@npm:1.0.0"
   dependencies:
@@ -9702,29 +9773,22 @@
   resolution: "uuid@npm:8.3.2"
   bin:
     uuid: dist/bin/uuid
   checksum: 5575a8a75c13120e2f10e6ddc801b2c7ed7d8f3c8ac22c7ed0c7b2ba6383ec0abda88c905085d630e251719e0777045ae3236f04c812184b7c765f63a70e58df
   languageName: node
   linkType: hard
 
-"v8-compile-cache@npm:^2.3.0":
-  version: 2.4.0
-  resolution: "v8-compile-cache@npm:2.4.0"
-  checksum: 8eb6ddb59d86f24566503f1e6ca98f3e6f43599f05359bd3ab737eaaf1585b338091478a4d3d5c2646632cf8030288d7888684ea62238cdce15a65ae2416718f
-  languageName: node
-  linkType: hard
-
 "v8-to-istanbul@npm:^9.0.1":
-  version: 9.1.3
-  resolution: "v8-to-istanbul@npm:9.1.3"
+  version: 9.2.0
+  resolution: "v8-to-istanbul@npm:9.2.0"
   dependencies:
     "@jridgewell/trace-mapping": ^0.3.12
     "@types/istanbul-lib-coverage": ^2.0.1
     convert-source-map: ^2.0.0
-  checksum: 5d592ab3d186b386065dace8e01c543a922a904b3cfac39667de172455a6b3d0e8e1401574fecb8a12092ad0809b5a8fd15f1cc14d0666139a1bb77cd6ac2cf8
+  checksum: 31ef98c6a31b1dab6be024cf914f235408cd4c0dc56a5c744a5eea1a9e019ba279e1b6f90d695b78c3186feed391ed492380ccf095009e2eb91f3d058f0b4491
   languageName: node
   linkType: hard
 
 "validate-npm-package-license@npm:^3.0.1":
   version: 3.0.4
   resolution: "validate-npm-package-license@npm:3.0.4"
   dependencies:
@@ -9927,47 +9991,47 @@
   version: 3.2.3
   resolution: "webpack-sources@npm:3.2.3"
   checksum: 989e401b9fe3536529e2a99dac8c1bdc50e3a0a2c8669cbafad31271eadd994bc9405f88a3039cd2e29db5e6d9d0926ceb7a1a4e7409ece021fe79c37d9c4607
   languageName: node
   linkType: hard
 
 "webpack@npm:^5.76.1":
-  version: 5.89.0
-  resolution: "webpack@npm:5.89.0"
+  version: 5.90.0
+  resolution: "webpack@npm:5.90.0"
   dependencies:
     "@types/eslint-scope": ^3.7.3
-    "@types/estree": ^1.0.0
+    "@types/estree": ^1.0.5
     "@webassemblyjs/ast": ^1.11.5
     "@webassemblyjs/wasm-edit": ^1.11.5
     "@webassemblyjs/wasm-parser": ^1.11.5
     acorn: ^8.7.1
     acorn-import-assertions: ^1.9.0
-    browserslist: ^4.14.5
+    browserslist: ^4.21.10
     chrome-trace-event: ^1.0.2
     enhanced-resolve: ^5.15.0
     es-module-lexer: ^1.2.1
     eslint-scope: 5.1.1
     events: ^3.2.0
     glob-to-regexp: ^0.4.1
     graceful-fs: ^4.2.9
     json-parse-even-better-errors: ^2.3.1
     loader-runner: ^4.2.0
     mime-types: ^2.1.27
     neo-async: ^2.6.2
     schema-utils: ^3.2.0
     tapable: ^2.1.1
-    terser-webpack-plugin: ^5.3.7
+    terser-webpack-plugin: ^5.3.10
     watchpack: ^2.4.0
     webpack-sources: ^3.2.3
   peerDependenciesMeta:
     webpack-cli:
       optional: true
   bin:
     webpack: bin/webpack.js
-  checksum: 43fe0dbc30e168a685ef5a86759d5016a705f6563b39a240aa00826a80637d4a3deeb8062e709d6a4b05c63e796278244c84b04174704dc4a37bedb0f565c5ed
+  checksum: 178a0e7e9e5b26264a19dd5fe554a3508a8afafc9cce972bfd4452b5128d0db1b37832f5e615be1cff1934f24da0de967929f199be2b3fe283ca1951f98ea3fe
   languageName: node
   linkType: hard
 
 "whatwg-encoding@npm:^2.0.0":
   version: 2.0.0
   resolution: "whatwg-encoding@npm:2.0.0"
   dependencies:
@@ -10134,26 +10198,36 @@
   dependencies:
     imurmurhash: ^0.1.4
     signal-exit: ^3.0.7
   checksum: 5da60bd4eeeb935eec97ead3df6e28e5917a6bd317478e4a85a5285e8480b8ed96032bbcc6ecd07b236142a24f3ca871c924ec4a6575e623ec1b11bf8c1c253c
   languageName: node
   linkType: hard
 
+"write-file-atomic@npm:^5.0.1":
+  version: 5.0.1
+  resolution: "write-file-atomic@npm:5.0.1"
+  dependencies:
+    imurmurhash: ^0.1.4
+    signal-exit: ^4.0.1
+  checksum: 8dbb0e2512c2f72ccc20ccedab9986c7d02d04039ed6e8780c987dc4940b793339c50172a1008eed7747001bfacc0ca47562668a069a7506c46c77d7ba3926a9
+  languageName: node
+  linkType: hard
+
 "ws@npm:^8.11.0":
-  version: 8.14.2
-  resolution: "ws@npm:8.14.2"
+  version: 8.16.0
+  resolution: "ws@npm:8.16.0"
   peerDependencies:
     bufferutil: ^4.0.1
     utf-8-validate: ">=5.0.2"
   peerDependenciesMeta:
     bufferutil:
       optional: true
     utf-8-validate:
       optional: true
-  checksum: 3ca0dad26e8cc6515ff392b622a1467430814c463b3368b0258e33696b1d4bed7510bc7030f7b72838b9fdeb8dbd8839cbf808367d6aae2e1d668ce741d4308b
+  checksum: feb3eecd2bae82fa8a8beef800290ce437d8b8063bdc69712725f21aef77c49cb2ff45c6e5e7fce622248f9c7abaee506bae0a9064067ffd6935460c7357321b
   languageName: node
   linkType: hard
 
 "xml-name-validator@npm:^4.0.0":
   version: 4.0.0
   resolution: "xml-name-validator@npm:4.0.0"
   checksum: af100b79c29804f05fa35aa3683e29a321db9b9685d5e5febda3fa1e40f13f85abc40f45a6b2bf7bee33f68a1dc5e8eaef4cec100a304a9db565e6061d4cb5ad
@@ -10209,22 +10283,15 @@
 "yallist@npm:^4.0.0":
   version: 4.0.0
   resolution: "yallist@npm:4.0.0"
   checksum: 343617202af32df2a15a3be36a5a8c0c8545208f3d3dfbc6bb7c3e3b7e8c6f8e7485432e4f3b88da3031a6e20afa7c711eded32ddfb122896ac5d914e75848d5
   languageName: node
   linkType: hard
 
-"yaml@npm:^1.10.0":
-  version: 1.10.2
-  resolution: "yaml@npm:1.10.2"
-  checksum: ce4ada136e8a78a0b08dc10b4b900936912d15de59905b2bf415b4d33c63df1d555d23acb2a41b23cf9fb5da41c256441afca3d6509de7247daa062fd2c5ea5f
-  languageName: node
-  linkType: hard
-
-"yargs-parser@npm:^20.2.3":
+"yargs-parser@npm:^20.2.9":
   version: 20.2.9
   resolution: "yargs-parser@npm:20.2.9"
   checksum: 8bb69015f2b0ff9e17b2c8e6bfe224ab463dd00ca211eece72a4cd8a906224d2703fb8a326d36fdd0e68701e201b2a60ed7cf81ce0fd9b3799f9fe7745977ae3
   languageName: node
   linkType: hard
 
 "yargs-parser@npm:^21.0.1, yargs-parser@npm:^21.1.1":
@@ -10246,19 +10313,19 @@
     y18n: ^5.0.5
     yargs-parser: ^21.1.1
   checksum: 73b572e863aa4a8cbef323dd911d79d193b772defd5a51aab0aca2d446655216f5002c42c5306033968193bdbf892a7a4c110b0d77954a7fdf563e653967b56a
   languageName: node
   linkType: hard
 
 "yjs@npm:^13.5.0, yjs@npm:^13.5.40":
-  version: 13.6.8
-  resolution: "yjs@npm:13.6.8"
+  version: 13.6.11
+  resolution: "yjs@npm:13.6.11"
   dependencies:
-    lib0: ^0.2.74
-  checksum: a2a6fd17a2cce6461b64bedd69f66845b9dfd4702e285be0b5e382840337232e54ba5cf5d48f871263074de625d3902d17ab8a1766695af3fc05a0b4da8d95e0
+    lib0: ^0.2.86
+  checksum: fb2993b12c6d13caf52d41af747991fa0be0a7e560ad2de84a736b4b7fa085d8327ff7254238840c407fa0671ca8c8e5917baea32f6d6686923c602134045b94
   languageName: node
   linkType: hard
 
 "yocto-queue@npm:^0.1.0":
   version: 0.1.0
   resolution: "yocto-queue@npm:0.1.0"
   checksum: f77b3d8d00310def622123df93d4ee654fc6a0096182af8bd60679ddcdfb3474c56c6c7190817c84a2785648cdee9d721c0154eb45698c62176c322fb46fc700
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/package.json` & `jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9078373015873015%*

 * *Differences: {"'author'": "{'email': 'raphael.marietan@hotmail.com'}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/settingregistry': '^4.0.0', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.0', '@jupyterlab/services': '^7.0.0'}",*

 * * "'description'": "'A JupyterLab extension to send notebook interaction data to a backend.'",*

 * * "'devDependencies'": "{'@typescript-eslint/eslint-plugin': '^6.1.0', '@typescript-eslint/parser': "*

 * *                      "'^6.1.0', 'eslint-config-prettier': '^8.8.0' […]*

```diff
@@ -1,44 +1,47 @@
 {
     "author": {
-        "email": "me@test.com",
+        "email": "raphael.marietan@hotmail.com",
         "name": "Raphael Marietan"
     },
     "bugs": {
         "url": "https://github.com/chili-epfl/jupyter-dashboard-send-extension/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0 || ^4.0.0",
-        "@jupyterlab/settingregistry": "^3.1.0 || ^4.0.0"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0"
     },
-    "description": "A JupyterLab extension to send notebook execution and activity to a self-hosted backend.",
+    "description": "A JupyterLab extension to send notebook interaction data to a backend.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
-        "@types/crypto-js": "^4.1.2",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
-        "@typescript-eslint/eslint-plugin": "^5.55.0",
-        "@typescript-eslint/parser": "^5.55.0",
+        "@types/react-addons-linked-state-mixin": "^0.14.22",
+        "@typescript-eslint/eslint-plugin": "^6.1.0",
+        "@typescript-eslint/parser": "^6.1.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
-        "eslint-config-prettier": "^8.7.0",
-        "eslint-plugin-prettier": "^4.2.1",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^5.0.0",
         "jest": "^29.2.0",
+        "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.8.7",
-        "rimraf": "^4.4.1",
+        "prettier": "^3.0.0",
+        "rimraf": "^5.0.1",
         "source-map-loader": "^1.0.2",
         "style-loader": "^3.3.1",
-        "stylelint": "^14.9.1",
-        "stylelint-config-prettier": "^9.0.4",
-        "stylelint-config-recommended": "^8.0.0",
-        "stylelint-config-standard": "^26.0.0",
-        "stylelint-prettier": "^2.0.0",
+        "stylelint": "^15.10.1",
+        "stylelint-config-recommended": "^13.0.0",
+        "stylelint-config-standard": "^34.0.0",
+        "stylelint-csstree-validator": "^3.0.0",
+        "stylelint-prettier": "^4.0.0",
         "typescript": "~5.0.2",
         "yjs": "^13.5.0"
     },
     "eslintConfig": {
         "extends": [
             "eslint:recommended",
             "plugin:@typescript-eslint/eslint-recommended",
@@ -100,23 +103,34 @@
         "tests",
         "**/__tests__",
         "ui-tests"
     ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/chili-epfl/jupyter-dashboard-send-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.4c8f2b8808a7717691b7.js",
+            "load": "static/remoteEntry.aa29f5d9f0a6f487df86.js",
             "style": "./style"
         },
+        "discovery": {
+            "server": {
+                "base": {
+                    "name": "jupyterlab_unianalytics_telemetry"
+                },
+                "managers": [
+                    "pip"
+                ]
+            }
+        },
         "extension": true,
         "outputDir": "jupyterlab_unianalytics_telemetry/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -124,14 +138,22 @@
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "jupyterlab_unianalytics_telemetry",
     "prettier": {
         "arrowParens": "avoid",
         "endOfLine": "auto",
+        "overrides": [
+            {
+                "files": "package.json",
+                "options": {
+                    "tabWidth": 4
+                }
+            }
+        ],
         "singleQuote": true,
         "trailingComma": "none"
     },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
@@ -173,16 +195,21 @@
     "styleModule": "style/index.js",
     "stylelint": {
         "extends": [
             "stylelint-config-recommended",
             "stylelint-config-standard",
             "stylelint-prettier/recommended"
         ],
+        "plugins": [
+            "stylelint-csstree-validator"
+        ],
         "rules": {
+            "csstree/validator": true,
             "property-no-vendor-prefix": null,
+            "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.8"
+    "version": "4.0.9"
 }
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/schemas/jupyterlab_unianalytics_telemetry/package.json.orig` & `jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/schemas/jupyterlab_unianalytics_telemetry/package.json.orig`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.907142857142857%*

 * *Differences: {"'author'": "{'email': 'raphael.marietan@hotmail.com'}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/settingregistry': '^4.0.0', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.0', '@jupyterlab/services': '^7.0.0'}",*

 * * "'description'": "'A JupyterLab extension to send notebook interaction data to a backend.'",*

 * * "'devDependencies'": "{'@typescript-eslint/eslint-plugin': '^6.1.0', '@typescript-eslint/parser': "*

 * *                      "'^6.1.0', 'eslint-config-prettier': '^8.8.0' […]*

```diff
@@ -1,44 +1,47 @@
 {
     "author": {
-        "email": "me@test.com",
+        "email": "raphael.marietan@hotmail.com",
         "name": "Raphael Marietan"
     },
     "bugs": {
         "url": "https://github.com/chili-epfl/jupyter-dashboard-send-extension/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0 || ^4.0.0",
-        "@jupyterlab/settingregistry": "^3.1.0 || ^4.0.0"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0"
     },
-    "description": "A JupyterLab extension to send notebook execution and activity to a self-hosted backend.",
+    "description": "A JupyterLab extension to send notebook interaction data to a backend.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
-        "@types/crypto-js": "^4.1.2",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
-        "@typescript-eslint/eslint-plugin": "^5.55.0",
-        "@typescript-eslint/parser": "^5.55.0",
+        "@types/react-addons-linked-state-mixin": "^0.14.22",
+        "@typescript-eslint/eslint-plugin": "^6.1.0",
+        "@typescript-eslint/parser": "^6.1.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
-        "eslint-config-prettier": "^8.7.0",
-        "eslint-plugin-prettier": "^4.2.1",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^5.0.0",
         "jest": "^29.2.0",
+        "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.8.7",
-        "rimraf": "^4.4.1",
+        "prettier": "^3.0.0",
+        "rimraf": "^5.0.1",
         "source-map-loader": "^1.0.2",
         "style-loader": "^3.3.1",
-        "stylelint": "^14.9.1",
-        "stylelint-config-prettier": "^9.0.4",
-        "stylelint-config-recommended": "^8.0.0",
-        "stylelint-config-standard": "^26.0.0",
-        "stylelint-prettier": "^2.0.0",
+        "stylelint": "^15.10.1",
+        "stylelint-config-recommended": "^13.0.0",
+        "stylelint-config-standard": "^34.0.0",
+        "stylelint-csstree-validator": "^3.0.0",
+        "stylelint-prettier": "^4.0.0",
         "typescript": "~5.0.2",
         "yjs": "^13.5.0"
     },
     "eslintConfig": {
         "extends": [
             "eslint:recommended",
             "plugin:@typescript-eslint/eslint-recommended",
@@ -100,18 +103,29 @@
         "tests",
         "**/__tests__",
         "ui-tests"
     ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/chili-epfl/jupyter-dashboard-send-extension",
     "jupyterlab": {
+        "discovery": {
+            "server": {
+                "base": {
+                    "name": "jupyterlab_unianalytics_telemetry"
+                },
+                "managers": [
+                    "pip"
+                ]
+            }
+        },
         "extension": true,
         "outputDir": "jupyterlab_unianalytics_telemetry/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -119,14 +133,22 @@
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "jupyterlab_unianalytics_telemetry",
     "prettier": {
         "arrowParens": "avoid",
         "endOfLine": "auto",
+        "overrides": [
+            {
+                "files": "package.json",
+                "options": {
+                    "tabWidth": 4
+                }
+            }
+        ],
         "singleQuote": true,
         "trailingComma": "none"
     },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
@@ -168,16 +190,21 @@
     "styleModule": "style/index.js",
     "stylelint": {
         "extends": [
             "stylelint-config-recommended",
             "stylelint-config-standard",
             "stylelint-prettier/recommended"
         ],
+        "plugins": [
+            "stylelint-csstree-validator"
+        ],
         "rules": {
+            "csstree/validator": true,
             "property-no-vendor-prefix": null,
+            "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.8"
+    "version": "4.0.9"
 }
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/schemas/jupyterlab_unianalytics_telemetry/settings.json` & `jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/schemas/jupyterlab_unianalytics_telemetry/settings.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/static/622.dfcc6f863c81bf0a5841.js` & `jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/static/333.fc339a7b12932252a9bf.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,466 +1,451 @@
 "use strict";
 (self.webpackChunkjupyterlab_unianalytics_telemetry = self.webpackChunkjupyterlab_unianalytics_telemetry || []).push([
-    [622], {
-        622: (e, t, s) => {
-            let i, n;
+    [333], {
+        333: (e, t, s) => {
+            let n, i;
             s.r(t), s.d(t, {
-                default: () => E,
-                disabledNotebooksSignaler: () => A,
-                isDashboardExtensionInstalled: () => N,
-                schemaIcon: () => j
-            }), i = "https://api.unianalytics.ch/send/", n = "wss://ax5pzl8bwk.execute-api.eu-north-1.amazonaws.com/production/";
+                PERSISTENT_USER_ID: () => j,
+                default: () => N,
+                disabledNotebooksSignaler: () => E,
+                isDashboardExtensionInstalled: () => A,
+                schemaIcon: () => T
+            }), n = "https://api.unianalytics.ch/send/", i = "wss://ax5pzl8bwk.execute-api.eu-north-1.amazonaws.com/production/";
             const o = "jupyterlab_unianalytics_telemetry",
                 l = "SendExtension",
-                a = "unianalytics-notebook-user-ids",
-                c = "unianalytics";
-            var d, r;
+                a = "unianalytics";
+            var c, d;
             ! function(e) {
-                e.notebookId = `${c}_notebook_id`, e.instanceId = `${c}_instance_id`, e.cellMapping = `${c}_cell_mapping`
-            }(d || (d = {})),
+                e.notebookId = `${a}_notebook_id`, e.cellMapping = `${a}_cell_mapping`
+            }(c || (c = {})),
             function(e) {
                 e.dashboardOpenChat = `${o}:unianalytics-open-chat`
-            }(r || (r = {}));
-            var h = s(539),
-                p = s(83),
-                _ = s(901);
-            class u {
+            }(d || (d = {}));
+            var r = s(372),
+                h = s(553),
+                p = s(901);
+            class _ {
                 static setJupyterVersion(e) {
-                    u._jupyterVersion = e
+                    _._jupyterVersion = e
                 }
                 static checkJupyterVersionSet() {
-                    if (null === u._jupyterVersion) throw new Error("JupyterLab version is not set in CompatibilityManager before trying to access it.")
+                    if (null === _._jupyterVersion) throw new Error("JupyterLab version is not set in CompatibilityManager before trying to access it.")
                 }
             }
-            u._jupyterVersion = null, u.getMetadataComp = (e, t) => {
+            _._jupyterVersion = null, _.getMetadataComp = (e, t) => {
                 var s;
-                return u.checkJupyterVersionSet(), 4 === u._jupyterVersion ? null == e ? void 0 : e.getMetadata(t) : null === (s = null == e ? void 0 : e.metadata) || void 0 === s ? void 0 : s.get(t)
-            }, u.setMetadataComp = (e, t, s) => {
-                var i;
-                u.checkJupyterVersionSet(), 4 === u._jupyterVersion ? null == e || e.setMetadata(t, s) : null === (i = null == e ? void 0 : e.metadata) || void 0 === i || i.set(t, s)
-            }, u.getCellIdsComp = e => (u.checkJupyterVersionSet(), Array.from({
+                return _.checkJupyterVersionSet(), 4 === _._jupyterVersion ? null == e ? void 0 : e.getMetadata(t) : null === (s = null == e ? void 0 : e.metadata) || void 0 === s ? void 0 : s.get(t)
+            }, _.setMetadataComp = (e, t, s) => {
+                var n;
+                _.checkJupyterVersionSet(), 4 === _._jupyterVersion ? null == e || e.setMetadata(t, s) : null === (n = null == e ? void 0 : e.metadata) || void 0 === n || n.set(t, s)
+            }, _.getCellIdsComp = e => (_.checkJupyterVersionSet(), Array.from({
                 length: e.length
             }, ((t, s) => e.get(s).id)));
-            const g = () => {
-                    const e = document.cookie.split(";");
-                    for (const t of e) {
-                        const [e, s] = t.split("=").map((e => e.trim()));
-                        if (e === a) return s
-                    }
-                    return null
-                },
-                m = e => {
-                    let t = 0;
-                    if ("string" == typeof e) t = e.length;
-                    else if (Array.isArray(e))
-                        for (const s of e) t += s.length;
-                    else
-                        for (const s in e) t += JSON.stringify(e[s]).length;
-                    return t
-                };
-            class C {
+            const u = e => {
+                let t = 0;
+                if ("string" == typeof e) t = e.length;
+                else if (Array.isArray(e))
+                    for (const s of e) t += s.length;
+                else
+                    for (const s in e) t += JSON.stringify(e[s]).length;
+                return t
+            };
+            class g {
                 constructor() {
-                    this._socket = null, this._ongoingConnectionInfo = null, this._pingInterval = 54e4, this._pingTimer = null
+                    this._socket = null, this._pingInterval = 54e4, this._pingTimer = null
                 }
-                _createSocket(e) {
-                    this._socket = new WebSocket(`wss://ax5pzl8bwk.execute-api.eu-north-1.amazonaws.com/production/?conType=STUDENT&nbId=${e.notebookId}&usrId=${e.instanceId}`), this._socket.addEventListener("open", (() => {
-                        console.log("WebSocket connection opened for", e), this._startPingTimer()
+                _createSocket(e, t) {
+                    this._socket = new WebSocket(`wss://ax5pzl8bwk.execute-api.eu-north-1.amazonaws.com/production/?conType=STUDENT&nbId=${e}&usrId=${t}`), this._socket.addEventListener("open", (() => {
+                        console.log(`${o}: WebSocket connection opened for`, {
+                            notebookId: e,
+                            userId: t
+                        }), this._startPingTimer()
                     })), this._socket.addEventListener("message", (e => {
                         const t = JSON.parse(e.data);
-                        t.action, console.log("Received message from server:", t)
-                    })), this._socket.addEventListener("close", (t => {
-                        console.log("WebSocket connection closed for ", e, t), this._stopPingTimer()
+                        t.action, console.log(`${o}: Received message from server:`, t)
+                    })), this._socket.addEventListener("close", (s => {
+                        console.log(`${o}: WebSocket connection closed for `, {
+                            notebookId: e,
+                            userId: t
+                        }, s), this._stopPingTimer()
                     })), this._socket.addEventListener("error", (e => {
-                        console.error("WebSocket error", e)
+                        console.error(`${o}: WebSocket error`, e)
                     }))
                 }
                 establishSocketConnection(e) {
-                    this._closeSocketConnection(), this._ongoingConnectionInfo = e, e && this._createSocket(e)
+                    this._closeSocketConnection(), e && j && this._createSocket(e, j)
                 }
                 _closeSocketConnection() {
                     this._socket && this._socket.close(), this._socket = null
                 }
                 terminateSocketConnection() {
-                    this._closeSocketConnection(), this._ongoingConnectionInfo = null
+                    this._closeSocketConnection()
                 }
                 _startPingTimer() {
                     this._pingTimer = window.setInterval((() => {
                         this._socket && this._socket.readyState === WebSocket.OPEN && this._socket.send('{ "action":"ping" }')
                     }), this._pingInterval)
                 }
                 _stopPingTimer() {
                     this._pingTimer && (clearInterval(this._pingTimer), this._pingTimer = null)
                 }
             }
-            class b {
-                constructor(e) {
-                    this._isDisposed = !1;
-                    const t = e.context.model,
-                        s = u.getMetadataComp(t, d.notebookId);
-                    if (s) {
-                        const e = g(),
-                            t = e ? JSON.parse(e) : {};
-                        if (!t[s]) {
-                            const e = crypto.randomUUID();
-                            t[s] = e, i = JSON.stringify(t), document.cookie = `${a}=${i}; expires=Fri, 31 Dec 9999 23:59:59 GMT; path=/`
-                        }
-                    }
-                    var i
-                }
-                get isDisposed() {
-                    return this._isDisposed
-                }
-                dispose() {
-                    this.isDisposed || (this._isDisposed = !0, _.Signal.clearData(this))
-                }
-            }
-            class k {
+            class m {
                 constructor(e) {
                     this._onPanelDisposed = e => {
                         e.context.model.cells.changed.disconnect(this._onCellsAltered, this)
                     }, this._hasCellListChanged = (e, t) => {
                         if (e.length !== t.length) return !0;
                         for (let s = 0; s < e.length; s++)
                             if (e[s] !== t[s]) return !0;
                         return !1
                     }, this._updateCellMapping = e => {
                         var t, s;
-                        const i = u.getMetadataComp(null === (t = this._panel) || void 0 === t ? void 0 : t.model, d.cellMapping);
-                        if (!i) return;
-                        const n = [];
+                        const n = _.getMetadataComp(null === (t = this._panel) || void 0 === t ? void 0 : t.model, c.cellMapping);
+                        if (!n) return;
+                        const i = [];
                         for (const [t, s] of e.entries()) {
-                            const e = i.find((([e, t]) => e === s));
-                            if (e) n.push(e);
+                            const e = n.find((([e, t]) => e === s));
+                            if (e) i.push(e);
                             else if (t > 0) {
-                                const e = n[t - 1];
-                                n.push([s, e[1]])
+                                const e = i[t - 1];
+                                i.push([s, e[1]])
                             } else {
-                                const e = i[0];
-                                n.push([s, e[1]])
+                                const e = n[0];
+                                i.push([s, e[1]])
                             }
                         }
-                        u.setMetadataComp(null === (s = this._panel) || void 0 === s ? void 0 : s.model, d.cellMapping, n)
+                        _.setMetadataComp(null === (s = this._panel) || void 0 === s ? void 0 : s.model, c.cellMapping, i)
                     }, this._onCellsAltered = e => {
                         var t;
-                        const s = u.getCellIdsComp(e);
+                        const s = _.getCellIdsComp(e);
                         (null === (t = this._panel) || void 0 === t ? void 0 : t.context.isReady) && this._hasCellListChanged(s, this._cellIdList) && this._updateCellMapping(s), this._cellIdList = s
-                    }, this._isDisposed = !1, this._cellIdList = [], this._panel = e, e && !e.isDisposed && u.getMetadataComp(e.context.model, d.notebookId) && u.getMetadataComp(e.context.model, d.cellMapping) && (this._cellIdList = u.getCellIdsComp(e.context.model.cells), e.context.model.cells.changed.connect(this._onCellsAltered, this), e.disposed.connect(this._onPanelDisposed, this))
+                    }, this._isDisposed = !1, this._cellIdList = [], this._panel = e, e && !e.isDisposed && _.getMetadataComp(e.context.model, c.notebookId) && _.getMetadataComp(e.context.model, c.cellMapping) && (this._cellIdList = _.getCellIdsComp(e.context.model.cells), e.context.model.cells.changed.connect(this._onCellsAltered, this), e.disposed.connect(this._onPanelDisposed, this))
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 dispose() {
-                    this.isDisposed || (this._isDisposed = !0, this._panel = null, this._cellIdList = [], _.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, this._panel = null, this._cellIdList = [], p.Signal.clearData(this))
                 }
             }
-            var D = s(576),
-                v = s(930),
-                I = s(956);
-            const f = (e, t) => {
-                    const s = JSON.stringify(e),
-                        i = "https://api.unianalytics.ch/send/" + t;
-                    s.length > 1048576 ? console.log("Payload size exceeds limit of 1 Mb") : (console.log("Posting to " + t + " :\n", e), fetch(i, {
-                        method: "POST",
-                        headers: {
-                            "Content-Type": "application/json",
-                            "X-Nonce": crypto.randomUUID()
-                        },
-                        body: s
-                    }).then((e => {
-                        e.json().then((e => console.log(e)))
-                    })))
+            var C = s(392),
+                b = s(930),
+                k = s(774);
+            const v = (e, t) => {
+                    if (j) {
+                        const s = {
+                                ...e,
+                                user_id: j
+                            },
+                            n = JSON.stringify(s),
+                            i = "https://api.unianalytics.ch/send/" + t;
+                        if (n.length > 1048576) return void console.log(`${o}: Payload size exceeds limit of 1 Mb`);
+                        console.log(`${o}: Posting to ` + t + " :\n", s), fetch(i, {
+                            method: "POST",
+                            headers: {
+                                "Content-Type": "application/json",
+                                "X-Nonce": crypto.randomUUID()
+                            },
+                            body: n
+                        }).then((e => {
+                            e.json().then((e => console.log(`${o}: ` + e)))
+                        }))
+                    } else console.log(`${o}: No user id`)
                 },
-                y = e => {
-                    f(e, "alter")
+                D = e => {
+                    v(e, "alter")
                 };
-            class S {
+            class f {
                 constructor(e, t) {
-                    this._isDisposed = !1, this._panel = e, this._notebookId = t.notebookId, this._instanceId = t.instanceId, D.NotebookActions.executed.connect(this._onCellExecuted, this), e.disposed.connect((() => D.NotebookActions.executed.disconnect(this._onCellExecuted, this)))
+                    this._isDisposed = !1, this._panel = e, this._notebookId = t, C.NotebookActions.executed.connect(this._onCellExecuted, this), e.disposed.connect((() => C.NotebookActions.executed.disconnect(this._onCellExecuted, this)))
                 }
                 _onCellExecuted(e, t) {
-                    var s, i, n, o;
+                    var s, n, i, o;
                     const {
                         notebook: l,
                         cell: a
                     } = t;
-                    var c, r;
+                    var d, r;
                     if (l === this._panel.content)
-                        if (a instanceof I.CodeCell) {
-                            const e = u.getMetadataComp(a.model, "execution");
-                            if (e && v.JSONExt.isObject(e)) {
+                        if (a instanceof k.CodeCell) {
+                            const e = _.getMetadataComp(a.model, "execution");
+                            if (e && b.JSONExt.isObject(e)) {
                                 const t = e["shell.execute_reply.started"] || e["iopub.execute_input"],
-                                    n = e["shell.execute_reply"];
-                                if ((!n || e["iopub.execute_input"]) && n && t) {
+                                    i = e["shell.execute_reply"];
+                                if ((!i || e["iopub.execute_input"]) && i && t) {
                                     const e = a.model.outputs.toJSON(),
                                         o = this._panel.model,
                                         {
                                             status: l,
-                                            cell_output_length: c
+                                            cell_output_length: d
                                         } = (e => {
                                             let t = 0,
                                                 s = "ok";
-                                            for (const i of e) {
-                                                const e = i.output_type;
+                                            for (const n of e) {
+                                                const e = n.output_type;
                                                 if ("stream" === e) {
-                                                    const e = i.text;
-                                                    t += m(e)
-                                                } else "error" === e ? (s = "error", t += i.evalue.length) : t += "execute_result" === e || "display_data" === e ? m(i.data) : 0
+                                                    const e = n.text;
+                                                    t += u(e)
+                                                } else "error" === e ? (s = "error", t += n.evalue.length) : t += "execute_result" === e || "display_data" === e ? u(n.data) : 0
                                             }
                                             return {
                                                 status: s,
                                                 cell_output_length: t
                                             }
                                         })(e),
-                                        h = null === (i = null === (s = u.getMetadataComp(o, d.cellMapping)) || void 0 === s ? void 0 : s.find((([e]) => e === a.model.id))) || void 0 === i ? void 0 : i[1];
+                                        h = null === (n = null === (s = _.getMetadataComp(o, c.cellMapping)) || void 0 === s ? void 0 : s.find((([e]) => e === a.model.id))) || void 0 === n ? void 0 : n[1];
                                     h && (r = {
                                         notebook_id: this._notebookId,
-                                        instance_id: this._instanceId,
-                                        language_mimetype: u.getMetadataComp(o, "language_info").mimetype || "text/plain",
+                                        language_mimetype: _.getMetadataComp(o, "language_info").mimetype || "text/plain",
                                         cell_id: a.model.id,
                                         orig_cell_id: h,
                                         t_start: t,
-                                        t_finish: n,
+                                        t_finish: i,
                                         status: l,
                                         cell_input: a.model.sharedModel.getSource(),
                                         cell_output_model: e,
-                                        cell_output_length: c
-                                    }, f(r, "exec/code"))
+                                        cell_output_length: d
+                                    }, v(r, "exec/code"))
                                 }
                             }
-                        } else if (a instanceof I.MarkdownCell) {
-                        const e = null === (o = null === (n = u.getMetadataComp(this._panel.model, d.cellMapping)) || void 0 === n ? void 0 : n.find((([e]) => e === a.model.id))) || void 0 === o ? void 0 : o[1];
-                        e && (c = {
+                        } else if (a instanceof k.MarkdownCell) {
+                        const e = null === (o = null === (i = _.getMetadataComp(this._panel.model, c.cellMapping)) || void 0 === i ? void 0 : i.find((([e]) => e === a.model.id))) || void 0 === o ? void 0 : o[1];
+                        e && (d = {
                             notebook_id: this._notebookId,
-                            instance_id: this._instanceId,
                             cell_id: a.model.id,
                             orig_cell_id: e,
                             time: (new Date).toISOString(),
                             cell_content: a.model.sharedModel.getSource()
-                        }, f(c, "exec/markdown"))
+                        }, v(d, "exec/markdown"))
                     }
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 dispose() {
-                    this.isDisposed || (this._isDisposed = !0, _.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, p.Signal.clearData(this))
                 }
             }
-            class w {
+            class y {
                 constructor(e, t) {
                     this._onCellsAltered = e => {
-                        const t = u.getCellIdsComp(e),
+                        const t = _.getCellIdsComp(e),
                             s = t.filter((e => !this._cellIdList.includes(e))),
-                            i = this._cellIdList.filter((e => !t.includes(e)));
-                        for (const e of s) y({
+                            n = this._cellIdList.filter((e => !t.includes(e)));
+                        for (const e of s) D({
                             notebook_id: this._notebookId,
-                            instance_id: this._instanceId,
                             cell_id: e,
                             alteration_type: "ADD",
                             time: (new Date).toISOString()
                         });
-                        for (const e of i) y({
+                        for (const e of n) D({
                             notebook_id: this._notebookId,
-                            instance_id: this._instanceId,
                             cell_id: e,
                             alteration_type: "REMOVE",
                             time: (new Date).toISOString()
                         });
                         this._cellIdList = t
                     }, this._onPanelDisposed = e => {
                         e.context.model.cells.changed.disconnect(this._onCellsAltered, this)
-                    }, this._isDisposed = !1, this._cellIdList = [], this._notebookId = t.notebookId, this._instanceId = t.instanceId, this._cellIdList = u.getCellIdsComp(e.context.model.cells), e.context.model.cells.changed.connect(this._onCellsAltered, this), e.disposed.connect(this._onPanelDisposed, this)
+                    }, this._isDisposed = !1, this._cellIdList = [], this._notebookId = t, this._cellIdList = _.getCellIdsComp(e.context.model.cells), e.context.model.cells.changed.connect(this._onCellsAltered, this), e.disposed.connect(this._onPanelDisposed, this)
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 dispose() {
-                    this.isDisposed || (this._isDisposed = !0, this._cellIdList = [], _.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, this._cellIdList = [], p.Signal.clearData(this))
                 }
             }
-            class x {
+            class S {
                 constructor(e, t) {
                     this._onContentDisposed = e => {
                         e.activeCellChanged.disconnect(this._onCellChanged, this), e.disposed.disconnect(this._onContentDisposed, this)
                     }, this._onCellChanged = (e, t) => {
                         this._sendCellClick("OFF"), this._setActiveCellAndOrigCellId(t), this._sendCellClick("ON")
                     }, this._setActiveCellAndOrigCellId = e => {
-                        var t, s, i;
-                        this._lastActiveCellId = null == e ? void 0 : e.model.sharedModel.getId(), this._lastActiveCellId ? this._lastOrigCellId = null === (i = null === (s = u.getMetadataComp(null === (t = this._panel) || void 0 === t ? void 0 : t.model, d.cellMapping)) || void 0 === s ? void 0 : s.find((([e]) => e === this._lastActiveCellId))) || void 0 === i ? void 0 : i[1] : this._lastOrigCellId = null
+                        var t, s, n;
+                        this._lastActiveCellId = null == e ? void 0 : e.model.sharedModel.getId(), this._lastActiveCellId ? this._lastOrigCellId = null === (n = null === (s = _.getMetadataComp(null === (t = this._panel) || void 0 === t ? void 0 : t.model, c.cellMapping)) || void 0 === s ? void 0 : s.find((([e]) => e === this._lastActiveCellId))) || void 0 === n ? void 0 : n[1] : this._lastOrigCellId = null
                     }, this._sendCellClick = e => {
                         if (this._lastActiveCellId) {
                             let s = null;
                             "ON" === e ? (this._cellStart = new Date, s = null) : s = ((new Date).getTime() - this._cellStart.getTime()) / 1e3, this._lastOrigCellId && (t = {
                                 notebook_id: this._notebookId,
-                                instance_id: this._instanceId,
                                 cell_id: this._lastActiveCellId,
                                 orig_cell_id: this._lastOrigCellId,
                                 click_type: e,
                                 time: (new Date).toISOString(),
                                 click_duration: s
-                            }, f(t, "clickevent/cell"))
+                            }, v(t, "clickevent/cell"))
                         }
                         var t
                     }, this._sendNotebookClick = e => {
                         let t = null;
                         var s;
                         "ON" === e ? (this._notebookStart = new Date, t = null) : t = ((new Date).getTime() - this._notebookStart.getTime()) / 1e3, s = {
                             notebook_id: this._notebookId,
-                            instance_id: this._instanceId,
                             click_type: e,
                             time: (new Date).toISOString(),
                             click_duration: t
-                        }, f(s, "clickevent/notebook")
-                    }, this._isDisposed = !1, this._lastActiveCellId = null, this._lastOrigCellId = null, this._notebookStart = new Date, this._cellStart = new Date, this._panel = e, this._notebookId = t.notebookId, this._instanceId = t.instanceId, this._sendNotebookClick("ON"), this._onCellChanged(e.content, e.content.activeCell), e.content.activeCellChanged.connect(this._onCellChanged, this), e.content.disposed.connect(this._onContentDisposed, this)
+                        }, v(s, "clickevent/notebook")
+                    }, this._isDisposed = !1, this._lastActiveCellId = null, this._lastOrigCellId = null, this._notebookStart = new Date, this._cellStart = new Date, this._panel = e, this._notebookId = t, this._sendNotebookClick("ON"), this._onCellChanged(e.content, e.content.activeCell), e.content.activeCellChanged.connect(this._onCellChanged, this), e.content.disposed.connect(this._onContentDisposed, this)
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 dispose() {
-                    this.isDisposed || (this._sendNotebookClick("OFF"), this._sendCellClick("OFF"), this._isDisposed = !0, this._lastActiveCellId = null, _.Signal.clearData(this))
+                    this.isDisposed || (this._sendNotebookClick("OFF"), this._sendCellClick("OFF"), this._isDisposed = !0, this._lastActiveCellId = null, p.Signal.clearData(this))
                 }
             }
-            var M = s(178);
-            class O {
+            var w = s(678);
+            class I {
                 constructor(e, t) {
-                    this._ongoingContextId = "", this._instanceInitializerDisposable = null, this._cellMappingDisposable = null, this._executionDisposable = null, this._alterationDisposable = null, this._focusDisposable = null, this._panel = null, this._isDataCollectionEnabled = e.get(l).composite, e.changed.connect(this._onSettingsChanged.bind(this)), A.valueChanged.connect(this._addOptionalTrackers.bind(this)), this._settings = e, this._dialogShownSettings = t, this._websocketManager = new C
+                    this._ongoingContextId = "", this._cellMappingDisposable = null, this._executionDisposable = null, this._alterationDisposable = null, this._focusDisposable = null, this._panel = null, this._isDataCollectionEnabled = e.get(l).composite, e.changed.connect(this._onSettingsChanged.bind(this)), E.valueChanged.connect(this._addOptionalTrackers.bind(this)), this._settings = e, this._dialogShownSettings = t, this._websocketManager = new g
                 }
                 _onSettingsChanged(e) {
-                    const t = this._isDataCollectionEnabled;
-                    this._isDataCollectionEnabled = e.get(l).composite, this._isDataCollectionEnabled !== t && this._addOptionalTrackers()
+                    this._isDataCollectionEnabled = e.get(l).composite
                 }
                 get panel() {
                     return this._panel
                 }
                 set panel(e) {
                     if (this._panel === e) return;
                     if (this._panel && this._panel.disposed.disconnect(this._onPanelDisposed, this), this._disposeFromAllTrackers(), this._panel = e, this._panel && this._panel.disposed.connect(this._onPanelDisposed, this), !this._panel) return;
                     const t = crypto.randomUUID();
                     this._ongoingContextId = t, this._panel.sessionContext.ready.then((() => {
                         this._ongoingContextId === t && this._panel && !this._panel.isDisposed && this._addAllTrackers()
                     }))
                 }
                 _addAllTrackers() {
-                    this._panel && this._panel.sessionContext.isReady && (this._instanceInitializerDisposable = new b(this._panel), this._cellMappingDisposable = new k(this._panel), this._addOptionalTrackers())
+                    this._panel && this._panel.sessionContext.isReady && (this._cellMappingDisposable = new m(this._panel), this._addOptionalTrackers())
                 }
                 _addOptionalTrackers() {
                     if (this._disposeFromOptionalTrackers(), this._panel && this._panel.sessionContext.isReady) {
                         const e = (e => {
                             if (e && !e.isDisposed) {
-                                const t = u.getMetadataComp(e.context.model, d.notebookId),
-                                    s = u.getMetadataComp(e.context.model, d.cellMapping);
-                                if (t && s) {
-                                    if (N && (null === A.value || A.value.includes(t))) return null;
-                                    const e = (e => {
-                                        const t = g();
-                                        return t ? JSON.parse(t)[e] : null
-                                    })(t);
-                                    if (e) return {
-                                        notebookId: t,
-                                        instanceId: e
-                                    }
-                                }
+                                const t = _.getMetadataComp(e.context.model, c.notebookId),
+                                    s = _.getMetadataComp(e.context.model, c.cellMapping);
+                                if (t && s) return A && (null === E.value || E.value.includes(t)) ? null : t
                             }
                             return null
                         })(this._panel);
                         e && this._showConsentDialogPromise().then((() => {
-                            this._panel && !this._panel.isDisposed && this._isDataCollectionEnabled && (this._focusDisposable = new x(this._panel, e), this._executionDisposable = new S(this._panel, e), this._alterationDisposable = new w(this._panel, e), this._websocketManager.establishSocketConnection(e))
+                            this._panel && !this._panel.isDisposed && this._isDataCollectionEnabled && (this._focusDisposable = new S(this._panel, e), this._executionDisposable = new f(this._panel, e), this._alterationDisposable = new y(this._panel, e), this._websocketManager.establishSocketConnection(e))
                         }))
                     }
                 }
                 async _showConsentDialogPromise() {
                     if (!this._dialogShownSettings.get("DialogShown").composite) {
-                        const e = await (0, M.showDialog)({
+                        const e = await (0, w.showDialog)({
                             title: "Unianalytics Data",
                             hasClose: !1,
                             body: "Enable anonymous collection of interaction data in specific notebooks to make it easier for your teacher(s) to support your learning?",
-                            buttons: [M.Dialog.okButton({
+                            buttons: [w.Dialog.okButton({
                                 label: "Yes"
-                            }), M.Dialog.cancelButton({
+                            }), w.Dialog.cancelButton({
                                 label: "No"
                             })]
                         });
                         await this._dialogShownSettings.set("DialogShown", !0);
                         let t = !1;
                         e.button.accept ? (await this._settings.set(l, !0), t = !0) : (await this._settings.set(l, !1), t = !1), this._isDataCollectionEnabled = t
                     }
                 }
                 _disposeFromAllTrackers() {
-                    this._instanceInitializerDisposable && (this._instanceInitializerDisposable.dispose(), this._instanceInitializerDisposable = null), this._cellMappingDisposable && (this._cellMappingDisposable.dispose(), this._cellMappingDisposable = null), this._disposeFromOptionalTrackers()
+                    this._cellMappingDisposable && (this._cellMappingDisposable.dispose(), this._cellMappingDisposable = null), this._disposeFromOptionalTrackers()
                 }
                 _disposeFromOptionalTrackers() {
                     this._websocketManager.terminateSocketConnection(), this._executionDisposable && (this._executionDisposable.dispose(), this._executionDisposable = null), this._alterationDisposable && (this._alterationDisposable.dispose(), this._alterationDisposable = null), this._focusDisposable && (this._focusDisposable.dispose(), this._focusDisposable = null)
                 }
                 _onPanelDisposed(e) {
                     this._disposeFromAllTrackers(), this.panel = null
                 }
             }
 
-            function T(e, t) {
+            function x(e, t) {
                 const s = e.currentWidget;
                 if (s)
-                    if (s instanceof D.NotebookPanel) {
+                    if (s instanceof C.NotebookPanel) {
                         const e = s;
                         t.panel = e
                     } else t.panel = null
             }
-            const j = new p.LabIcon({
-                    name: `${o}:schema-icon`,
-                    svgstr: '<?xml version="1.0" standalone="no"?>\n<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 20010904//EN"\n "http://www.w3.org/TR/2001/REC-SVG-20010904/DTD/svg10.dtd">\n<svg version="1.0" xmlns="http://www.w3.org/2000/svg"\n width="1763.000000pt" height="1611.000000pt" viewBox="0 0 1763.000000 1611.000000"\n preserveAspectRatio="xMidYMid meet">\n\n<g transform="translate(0.000000,1611.000000) scale(0.100000,-0.100000)"\nfill="#000000" stroke="none">\n<path fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M8220 15781 c-122 -18 -249 -116 -311 -239 l-34 -67 -5 -1265 -5\n-1265 -455 -5 c-452 -5 -455 -5 -498 -28 -110 -59 -172 -164 -172 -290 0 -121\n-76 -25 1105 -1398 812 -943 748 -872 819 -914 32 -19 58 -25 128 -28 79 -4\n93 -2 140 22 29 14 67 39 85 55 25 23 1067 1232 1298 1506 33 39 161 189 285\n333 124 144 236 283 249 309 36 70 35 160 -3 237 -35 72 -75 111 -146 145\nl-55 26 -437 3 -438 3 0 1233 c0 785 -4 1253 -10 1286 -16 82 -57 159 -119\n220 -67 67 -146 108 -232 120 -71 11 -1118 11 -1189 1z"/>\n<path fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M1264 12910 c-103 -21 -130 -44 -573 -489 -396 -399 -425 -431 -459\n-500 -33 -68 -36 -81 -36 -167 0 -84 3 -98 34 -161 30 -63 92 -128 921 -958\n489 -490 889 -897 889 -905 0 -8 -139 -154 -309 -324 -284 -286 -310 -316\n-330 -369 -54 -147 7 -310 141 -376 71 -36 81 -38 258 -51 74 -6 214 -17 310\n-25 96 -8 238 -19 315 -25 77 -5 158 -12 180 -15 22 -4 101 -10 175 -15 74 -5\n182 -14 240 -19 58 -6 195 -17 305 -26 110 -9 247 -20 305 -26 58 -5 164 -14\n235 -19 72 -5 180 -14 240 -20 61 -6 164 -12 230 -13 105 -1 125 2 161 21 66\n34 101 69 142 140 l37 67 -2 160 c-1 143 -9 270 -44 695 -5 69 -14 193 -19\n275 -6 83 -16 242 -25 355 -36 505 -46 645 -55 790 -6 85 -15 196 -20 247 -6\n51 -10 125 -10 165 0 88 -21 191 -50 247 -33 66 -100 123 -168 145 -79 25\n-170 19 -234 -15 -30 -16 -153 -129 -353 -326 -209 -206 -311 -301 -320 -295\n-7 4 -409 400 -892 881 -569 564 -899 885 -934 907 -78 49 -180 64 -285 44z"/>\n<path fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M16170 12906 c-121 -25 -117 -21 -1051 -959 -711 -715 -879 -878\n-895 -873 -10 3 -149 137 -309 297 -159 160 -303 300 -318 311 -15 11 -51 26\n-80 34 -118 31 -214 7 -298 -76 -79 -79 -93 -125 -113 -380 -9 -113 -21 -252\n-27 -310 -5 -58 -14 -163 -19 -235 -5 -71 -16 -215 -25 -320 -24 -291 -45\n-547 -55 -685 -5 -69 -14 -177 -20 -240 -30 -328 -54 -647 -54 -735 0 -88 27\n-153 90 -212 77 -74 118 -86 274 -84 74 0 167 5 205 11 39 5 138 14 220 20 83\n6 231 17 330 25 427 34 568 45 695 55 74 5 187 14 250 20 198 18 360 31 511\n40 80 5 177 14 215 20 38 5 103 10 145 10 124 0 222 37 297 111 101 100 125\n244 61 370 -10 20 -120 135 -245 255 -126 120 -259 249 -297 286 l-69 67 20\n28 c11 15 406 413 878 883 490 489 870 876 889 905 47 75 65 132 65 211 0 133\n-45 217 -192 359 -51 50 -232 227 -403 394 -345 337 -404 382 -515 400 -76 13\n-87 12 -160 -3z"/>\n<path fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M8375 8590 c-228 -8 -598 -37 -830 -65 -1245 -146 -2171 -506 -2432\n-945 -39 -64 -65 -161 -65 -235 1 -380 502 -732 1383 -973 624 -171 1379 -266\n2209 -278 699 -11 1303 31 1885 131 1018 174 1727 479 1977 850 249 371 -45\n775 -780 1069 -578 231 -1365 383 -2258 436 -234 14 -834 19 -1089 10z"/>\n<path fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M5050 5241 c0 -569 3 -836 11 -873 28 -130 117 -250 289 -389 111\n-90 274 -183 470 -270 415 -183 1027 -333 1690 -414 213 -26 415 -43 786 -65\n221 -13 833 -13 1039 0 372 24 467 31 600 45 263 27 377 42 635 85 333 55 788\n173 1055 273 548 205 879 460 950 732 13 51 15 175 15 877 0 450 -2 818 -5\n818 -2 0 -47 -25 -100 -55 -229 -132 -644 -302 -955 -390 -503 -142 -1099\n-250 -1630 -295 -69 -6 -172 -15 -230 -20 -258 -24 -782 -33 -1210 -21 -501\n13 -706 28 -1180 87 -163 21 -461 71 -590 99 -41 10 -95 21 -120 26 -65 13\n-368 89 -415 104 -22 7 -94 29 -160 50 -291 89 -672 250 -825 347 -30 19 -70\n43 -87 52 l-33 17 0 -820z m6030 -458 c119 -53 200 -155 220 -276 20 -127 -12\n-231 -98 -315 -121 -117 -298 -136 -443 -46 -189 117 -225 380 -75 542 43 46\n79 71 145 99 47 20 69 23 131 20 45 -3 93 -12 120 -24z"/>\n<path fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M12505 3167 c-94 -59 -379 -198 -515 -252 -656 -259 -1552 -428\n-2515 -476 -276 -13 -1032 -13 -1310 0 -520 26 -1033 88 -1450 175 -38 8 -104\n21 -145 30 -90 18 -365 88 -435 109 -320 100 -453 148 -615 219 -153 68 -315\n149 -395 198 -36 22 -68 40 -70 40 -3 0 -4 -381 -3 -847 l3 -848 23 -57 c153\n-379 846 -735 1802 -928 146 -30 192 -38 430 -74 900 -138 2028 -141 2950 -10\n276 39 585 97 742 138 51 14 127 34 168 44 233 61 561 182 760 281 301 151\n509 321 598 490 64 120 63 112 60 1007 l-3 811 -80 -50z m-1408 -1268 c69 -33\n144 -101 173 -158 46 -91 44 -239 -5 -329 -74 -137 -229 -218 -367 -192 -260\n50 -391 334 -251 547 102 155 287 209 450 132z"/>\n</g>\n</svg>\n'
-                }),
-                A = new class {
-                    constructor() {
-                        this._value = null, this._valueChanged = new _.Signal(this)
-                    }
-                    set value(e) {
-                        e !== this._value && (this._value = e, this._valueChanged.emit(e))
-                    }
-                    get value() {
-                        return this._value
-                    }
-                    get valueChanged() {
-                        return this._valueChanged
-                    }
-                };
-            let N = !1;
-            const E = {
+            var M = s(170),
+                O = s(387);
+            const T = new h.LabIcon({
+                name: `${o}:schema-icon`,
+                svgstr: '<?xml version="1.0" standalone="no"?>\n<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 20010904//EN"\n "http://www.w3.org/TR/2001/REC-SVG-20010904/DTD/svg10.dtd">\n<svg version="1.0" xmlns="http://www.w3.org/2000/svg"\n width="1763.000000pt" height="1611.000000pt" viewBox="0 0 1763.000000 1611.000000"\n preserveAspectRatio="xMidYMid meet">\n\n<g transform="translate(0.000000,1611.000000) scale(0.100000,-0.100000)"\nfill="#000000" stroke="none">\n<path fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M8220 15781 c-122 -18 -249 -116 -311 -239 l-34 -67 -5 -1265 -5\n-1265 -455 -5 c-452 -5 -455 -5 -498 -28 -110 -59 -172 -164 -172 -290 0 -121\n-76 -25 1105 -1398 812 -943 748 -872 819 -914 32 -19 58 -25 128 -28 79 -4\n93 -2 140 22 29 14 67 39 85 55 25 23 1067 1232 1298 1506 33 39 161 189 285\n333 124 144 236 283 249 309 36 70 35 160 -3 237 -35 72 -75 111 -146 145\nl-55 26 -437 3 -438 3 0 1233 c0 785 -4 1253 -10 1286 -16 82 -57 159 -119\n220 -67 67 -146 108 -232 120 -71 11 -1118 11 -1189 1z"/>\n<path fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M1264 12910 c-103 -21 -130 -44 -573 -489 -396 -399 -425 -431 -459\n-500 -33 -68 -36 -81 -36 -167 0 -84 3 -98 34 -161 30 -63 92 -128 921 -958\n489 -490 889 -897 889 -905 0 -8 -139 -154 -309 -324 -284 -286 -310 -316\n-330 -369 -54 -147 7 -310 141 -376 71 -36 81 -38 258 -51 74 -6 214 -17 310\n-25 96 -8 238 -19 315 -25 77 -5 158 -12 180 -15 22 -4 101 -10 175 -15 74 -5\n182 -14 240 -19 58 -6 195 -17 305 -26 110 -9 247 -20 305 -26 58 -5 164 -14\n235 -19 72 -5 180 -14 240 -20 61 -6 164 -12 230 -13 105 -1 125 2 161 21 66\n34 101 69 142 140 l37 67 -2 160 c-1 143 -9 270 -44 695 -5 69 -14 193 -19\n275 -6 83 -16 242 -25 355 -36 505 -46 645 -55 790 -6 85 -15 196 -20 247 -6\n51 -10 125 -10 165 0 88 -21 191 -50 247 -33 66 -100 123 -168 145 -79 25\n-170 19 -234 -15 -30 -16 -153 -129 -353 -326 -209 -206 -311 -301 -320 -295\n-7 4 -409 400 -892 881 -569 564 -899 885 -934 907 -78 49 -180 64 -285 44z"/>\n<path fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M16170 12906 c-121 -25 -117 -21 -1051 -959 -711 -715 -879 -878\n-895 -873 -10 3 -149 137 -309 297 -159 160 -303 300 -318 311 -15 11 -51 26\n-80 34 -118 31 -214 7 -298 -76 -79 -79 -93 -125 -113 -380 -9 -113 -21 -252\n-27 -310 -5 -58 -14 -163 -19 -235 -5 -71 -16 -215 -25 -320 -24 -291 -45\n-547 -55 -685 -5 -69 -14 -177 -20 -240 -30 -328 -54 -647 -54 -735 0 -88 27\n-153 90 -212 77 -74 118 -86 274 -84 74 0 167 5 205 11 39 5 138 14 220 20 83\n6 231 17 330 25 427 34 568 45 695 55 74 5 187 14 250 20 198 18 360 31 511\n40 80 5 177 14 215 20 38 5 103 10 145 10 124 0 222 37 297 111 101 100 125\n244 61 370 -10 20 -120 135 -245 255 -126 120 -259 249 -297 286 l-69 67 20\n28 c11 15 406 413 878 883 490 489 870 876 889 905 47 75 65 132 65 211 0 133\n-45 217 -192 359 -51 50 -232 227 -403 394 -345 337 -404 382 -515 400 -76 13\n-87 12 -160 -3z"/>\n<path fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M8375 8590 c-228 -8 -598 -37 -830 -65 -1245 -146 -2171 -506 -2432\n-945 -39 -64 -65 -161 -65 -235 1 -380 502 -732 1383 -973 624 -171 1379 -266\n2209 -278 699 -11 1303 31 1885 131 1018 174 1727 479 1977 850 249 371 -45\n775 -780 1069 -578 231 -1365 383 -2258 436 -234 14 -834 19 -1089 10z"/>\n<path fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M5050 5241 c0 -569 3 -836 11 -873 28 -130 117 -250 289 -389 111\n-90 274 -183 470 -270 415 -183 1027 -333 1690 -414 213 -26 415 -43 786 -65\n221 -13 833 -13 1039 0 372 24 467 31 600 45 263 27 377 42 635 85 333 55 788\n173 1055 273 548 205 879 460 950 732 13 51 15 175 15 877 0 450 -2 818 -5\n818 -2 0 -47 -25 -100 -55 -229 -132 -644 -302 -955 -390 -503 -142 -1099\n-250 -1630 -295 -69 -6 -172 -15 -230 -20 -258 -24 -782 -33 -1210 -21 -501\n13 -706 28 -1180 87 -163 21 -461 71 -590 99 -41 10 -95 21 -120 26 -65 13\n-368 89 -415 104 -22 7 -94 29 -160 50 -291 89 -672 250 -825 347 -30 19 -70\n43 -87 52 l-33 17 0 -820z m6030 -458 c119 -53 200 -155 220 -276 20 -127 -12\n-231 -98 -315 -121 -117 -298 -136 -443 -46 -189 117 -225 380 -75 542 43 46\n79 71 145 99 47 20 69 23 131 20 45 -3 93 -12 120 -24z"/>\n<path fill="#616161" class="jp-custom-icon jp-icon3 jp-icon-selectable" d="M12505 3167 c-94 -59 -379 -198 -515 -252 -656 -259 -1552 -428\n-2515 -476 -276 -13 -1032 -13 -1310 0 -520 26 -1033 88 -1450 175 -38 8 -104\n21 -145 30 -90 18 -365 88 -435 109 -320 100 -453 148 -615 219 -153 68 -315\n149 -395 198 -36 22 -68 40 -70 40 -3 0 -4 -381 -3 -847 l3 -848 23 -57 c153\n-379 846 -735 1802 -928 146 -30 192 -38 430 -74 900 -138 2028 -141 2950 -10\n276 39 585 97 742 138 51 14 127 34 168 44 233 61 561 182 760 281 301 151\n509 321 598 490 64 120 63 112 60 1007 l-3 811 -80 -50z m-1408 -1268 c69 -33\n144 -101 173 -158 46 -91 44 -239 -5 -329 -74 -137 -229 -218 -367 -192 -260\n50 -391 334 -251 547 102 155 287 209 450 132z"/>\n</g>\n</svg>\n'
+            });
+            let j = null;
+            const E = new class {
+                constructor() {
+                    this._value = null, this._valueChanged = new p.Signal(this)
+                }
+                set value(e) {
+                    e !== this._value && (this._value = e, this._valueChanged.emit(e))
+                }
+                get value() {
+                    return this._value
+                }
+                get valueChanged() {
+                    return this._valueChanged
+                }
+            };
+            let A = !1;
+            const N = {
                 id: `${o}:plugin`,
                 autoStart: !0,
-                requires: [h.ISettingRegistry],
+                requires: [r.ISettingRegistry],
                 activate: (e, t) => {
-                    console.log(`JupyterLab extension ${o} is activated!`), N = e.listPlugins().some((e => e.includes("jupyterlab_unianalytics_dashboard"))), console.log("Is dashboard extension also installed ?", N), N && window.addEventListener("message", (e => {
-                        e.origin === window.origin && e.data && "unianalytics" === e.data.identifier && (A.value = e.data.authNotebooks)
+                    console.log(`JupyterLab extension ${o} is activated!`), async function(e = "", t = {}) {
+                        const s = O.ServerConnection.makeSettings(),
+                            n = M.URLExt.join(s.baseUrl, "jupyterlab-unianalytics-telemetry", e);
+                        let i;
+                        try {
+                            i = await O.ServerConnection.makeRequest(n, t, s)
+                        } catch (e) {
+                            throw new O.ServerConnection.NetworkError(e)
+                        }
+                        const o = await i.text();
+                        if (!i.ok) throw new O.ServerConnection.ResponseError(i, o.message || o);
+                        return o
+                    }("get_anonymized_user_id").then((e => {
+                        j = e
+                    })).catch((e => {
+                        console.error(`${o}: server extension appears to be missing.\n${e}`)
+                    })), A = e.listPlugins().some((e => e.includes("jupyterlab_unianalytics_dashboard"))), A && window.addEventListener("message", (e => {
+                        e.origin === window.origin && e.data && "unianalytics" === e.data.identifier && (E.value = e.data.authNotebooks)
                     }));
                     const s = "3.1.0",
-                        i = e.version.match(/[0-9]+/g);
-                    if (i && ((e, t) => {
+                        n = e.version.match(/[0-9]+/g);
+                    if (n && ((e, t) => {
                             const s = e.split(/[^0-9]+/).map(Number),
-                                i = t.split(/[^0-9]+/).map(Number);
-                            for (let e = 0; e < Math.min(s.length, i.length); e++) {
+                                n = t.split(/[^0-9]+/).map(Number);
+                            for (let e = 0; e < Math.min(s.length, n.length); e++) {
                                 const t = s[e],
-                                    n = i[e];
-                                if (t !== n) return t - n
+                                    i = n[e];
+                                if (t !== i) return t - i
                             }
-                            const n = e.replace(/[0-9]+/g, ""),
+                            const i = e.replace(/[0-9]+/g, ""),
                                 o = t.replace(/[0-9]+/g, "");
-                            return n.localeCompare(o)
+                            return i.localeCompare(o)
                         })(e.version, s) >= 0) {
-                        const s = parseInt(i[0]);
-                        u.setJupyterVersion(s), (async (e, t) => {
+                        const s = parseInt(n[0]);
+                        _.setJupyterVersion(s), (async (e, t) => {
                             t.load("@jupyterlab/notebook-extension:tracker").then((e => {
                                 e.set("recordTiming", !0)
                             })).catch((e => console.log(`${o}: Could not force cell execution metadata recording: ${e}`)));
                             try {
-                                const [s, i] = await Promise.all([t.load(`${o}:settings`), t.load(`${o}:dialogShownSettings`)]), n = new O(s, i), l = e.shell;
-                                l && l.currentChanged.connect((() => T(l, n))), e.restored.then((() => {
-                                    T(l, n)
+                                const [s, n] = await Promise.all([t.load(`${o}:settings`), t.load(`${o}:dialogShownSettings`)]), i = new I(s, n), l = e.shell;
+                                l && l.currentChanged.connect((() => x(l, i))), e.restored.then((() => {
+                                    x(l, i)
                                 }))
                             } catch (e) {
                                 console.log(`${o}: Could not load settings, error: ${e}`)
                             }
                         })(e, t)
-                    } else console.log(`Use a more recent version of JupyterLab (>=${s})`)
+                    } else console.log(`${o}: Use a more recent version of JupyterLab (>=${s})`)
                 }
             }
         }
     }
 ]);
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/static/747.1caae4588978ba0392e1.js` & `jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/static/747.af77df2dd0efb547d5ac.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -172,15 +172,15 @@
                 if (t.styleSheet) t.styleSheet.cssText = e;
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
-        747: (e, t, n) => {
+        394: (e, t, n) => {
             n.r(t);
             var r = n(379),
                 a = n.n(r),
                 o = n(795),
                 i = n.n(o),
                 s = n(569),
                 c = n.n(s),
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/static/remoteEntry.4c8f2b8808a7717691b7.js` & `jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/static/remoteEntry.aa29f5d9f0a6f487df86.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, f, d, p, c, h, v, y, m, b, g, j, w, _ = {
+    var e, r, t, n, a, o, i, u, l, s, f, d, c, p, h, v, y, b, m, g, j, w, _, S = {
             142: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(622).then((() => () => t(622))),
-                        "./extension": () => t.e(622).then((() => () => t(622))),
-                        "./style": () => t.e(747).then((() => () => t(747)))
+                        "./index": () => t.e(333).then((() => () => t(333))),
+                        "./extension": () => t.e(333).then((() => () => t(333))),
+                        "./style": () => t.e(747).then((() => () => t(394)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -21,113 +21,113 @@
                     };
                 t.d(r, {
                     get: () => a,
                     init: () => o
                 })
             }
         },
-        S = {};
+        k = {};
 
-    function k(e) {
-        var r = S[e];
+    function E(e) {
+        var r = k[e];
         if (void 0 !== r) return r.exports;
-        var t = S[e] = {
+        var t = k[e] = {
             id: e,
             exports: {}
         };
-        return _[e](t, t.exports, k), t.exports
+        return S[e](t, t.exports, E), t.exports
     }
-    k.m = _, k.c = S, k.n = e => {
+    E.m = S, E.c = k, E.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return k.d(r, {
+        return E.d(r, {
             a: r
         }), r
-    }, k.d = (e, r) => {
-        for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
+    }, E.d = (e, r) => {
+        for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
-        622: "dfcc6f863c81bf0a5841",
-        747: "1caae4588978ba0392e1"
+    }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
+        333: "fc339a7b12932252a9bf",
+        747: "af77df2dd0efb547d5ac"
     } [e] + ".js?v=" + {
-        622: "dfcc6f863c81bf0a5841",
-        747: "1caae4588978ba0392e1"
-    } [e], k.g = function() {
+        333: "fc339a7b12932252a9bf",
+        747: "af77df2dd0efb547d5ac"
+    } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab_unianalytics_telemetry:", k.l = (t, n, a, o) => {
+    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab_unianalytics_telemetry:", E.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== a)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
                     var f = l[s];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
                         i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, k.nc && i.setAttribute("nonce", k.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, k.r = e => {
+    }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        k.S = {};
+        E.S = {};
         var e = {},
             r = {};
-        k.I = (t, n) => {
+        E.I = (t, n) => {
             n || (n = []);
             var a = r[t];
             if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
                 if (n.push(a), e[t]) return e[t];
-                k.o(k.S, t) || (k.S[t] = {});
-                var o = k.S[t],
+                E.o(E.S, t) || (E.S[t] = {});
+                var o = E.S[t],
                     i = "jupyterlab_unianalytics_telemetry",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
-                        get: () => k.e(622).then((() => () => k(622))),
+                        get: () => E.e(333).then((() => () => E(333))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab_unianalytics_telemetry", "4.0.8"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab_unianalytics_telemetry", "4.0.9"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        k.g.importScripts && (e = k.g.location + "");
-        var r = k.g.document;
+        E.g.importScripts && (e = E.g.location + "");
+        var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
                 for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), k.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), E.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -185,107 +185,112 @@
                     l = !1, u--
                 } else {
                     if (u <= n || f < d != a) return !1;
                     l = !1
                 } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
-        var t = k.S[e];
-        if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = E.S[e];
+        if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
         var a = l(e, t);
-        return o(n, a) || c(s(e, t, a, n)), v(e[t][a])
+        return o(n, a) || p(s(e, t, a, n)), v(e[t][a])
     }, d = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, p = (e, r, t, n) => {
+    }, c = (e, r, t, n) => {
         var o = e[t];
         return "No satisfying version (" + a(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
-    }, c = e => {
+    }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, h = (e, r, t, n) => {
-        c(p(e, r, t, n))
-    }, v = e => (e.loaded = 1, e.get()), m = (y = e => function(r, t, n, a) {
-        var o = k.I(r);
-        return o && o.then ? o.then(e.bind(e, r, k.S[r], t, n, a)) : e(r, k.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), v(d(r, t, n) || h(r, e, t, n) || u(r, t))))), b = y(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), g = {}, j = {
-        83: () => b("default", "@jupyterlab/ui-components", [1, 4, 0, 10]),
-        178: () => b("default", "@jupyterlab/apputils", [1, 4, 1, 10]),
-        539: () => b("default", "@jupyterlab/settingregistry", [1, 4, 0, 10]),
-        576: () => b("default", "@jupyterlab/notebook", [1, 4, 0, 10]),
-        901: () => b("default", "@lumino/signaling", [1, 2, 0, 0]),
-        930: () => b("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        956: () => m("default", "@jupyterlab/cells", [1, 4, 0, 10])
+        p(c(e, r, t, n))
+    }, v = e => (e.loaded = 1, e.get()), b = (y = e => function(r, t, n, a) {
+        var o = E.I(r);
+        return o && o.then ? o.then(e.bind(e, r, E.S[r], t, n, a)) : e(r, E.S[r], t, n, a)
+    })(((e, r, t, n) => (i(e, t), v(d(r, t, n) || h(r, e, t, n) || u(r, t))))), m = y(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), g = {}, j = {
+        170: () => m("default", "@jupyterlab/coreutils", [1, 6, 0, 12]),
+        372: () => m("default", "@jupyterlab/settingregistry", [1, 4, 0, 12]),
+        387: () => m("default", "@jupyterlab/services", [1, 7, 0, 12]),
+        392: () => m("default", "@jupyterlab/notebook", [1, 4, 0, 12]),
+        553: () => m("default", "@jupyterlab/ui-components", [1, 4, 0, 12]),
+        678: () => m("default", "@jupyterlab/apputils", [1, 4, 1, 12]),
+        774: () => b("default", "@jupyterlab/cells", [1, 4, 0, 12]),
+        901: () => m("default", "@lumino/signaling", [1, 2, 0, 0]),
+        930: () => m("default", "@lumino/coreutils", [1, 2, 0, 0])
     }, w = {
-        622: [83, 178, 539, 576, 901, 930, 956]
-    }, k.f.consumes = (e, r) => {
-        k.o(w, e) && w[e].forEach((e => {
-            if (k.o(g, e)) return r.push(g[e]);
-            var t = r => {
-                    g[e] = 0, k.m[e] = t => {
-                        delete k.c[e], t.exports = r()
+        333: [170, 372, 387, 392, 553, 678, 774, 901, 930]
+    }, _ = {}, E.f.consumes = (e, r) => {
+        E.o(w, e) && w[e].forEach((e => {
+            if (E.o(g, e)) return r.push(g[e]);
+            if (!_[e]) {
+                var t = r => {
+                    g[e] = 0, E.m[e] = t => {
+                        delete E.c[e], t.exports = r()
                     }
-                },
-                n = r => {
-                    delete g[e], k.m[e] = t => {
-                        throw delete k.c[e], r
+                };
+                _[e] = !0;
+                var n = r => {
+                    delete g[e], E.m[e] = t => {
+                        throw delete E.c[e], r
                     }
                 };
-            try {
-                var a = j[e]();
-                a.then ? r.push(g[e] = a.then(t).catch(n)) : t(a)
-            } catch (e) {
-                n(e)
+                try {
+                    var a = j[e]();
+                    a.then ? r.push(g[e] = a.then(t).catch(n)) : t(a)
+                } catch (e) {
+                    n(e)
+                }
             }
         }))
     }, (() => {
         var e = {
             166: 0
         };
-        k.f.j = (r, t) => {
-            var n = k.o(e, r) ? e[r] : void 0;
+        E.f.j = (r, t) => {
+            var n = E.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var a = new Promise(((t, a) => n = e[r] = [t, a]));
                     t.push(n[2] = a);
-                    var o = k.p + k.u(r),
+                    var o = E.p + E.u(r),
                         i = new Error;
-                    k.l(o, (t => {
-                        if (k.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    E.l(o, (t => {
+                        if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var a = t && ("load" === t.type ? "missing" : t.type),
                                 o = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, a, [o, i, u] = t,
                     l = 0;
                 if (o.some((r => 0 !== e[r]))) {
-                    for (n in i) k.o(i, n) && (k.m[n] = i[n]);
-                    u && u(k)
+                    for (n in i) E.o(i, n) && (E.m[n] = i[n]);
+                    u && u(E)
                 }
-                for (r && r(t); l < o.length; l++) a = o[l], k.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); l < o.length; l++) a = o[l], E.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunkjupyterlab_unianalytics_telemetry = self.webpackChunkjupyterlab_unianalytics_telemetry || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), k.nc = void 0;
-    var E = k(142);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).jupyterlab_unianalytics_telemetry = E
+    })(), E.nc = void 0;
+    var P = E(142);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).jupyterlab_unianalytics_telemetry = P
 })();
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/jupyterlab_unianalytics_telemetry/labextension/static/third-party-licenses.json` & `jupyterlab_unianalytics_telemetry-4.0.9/jupyterlab_unianalytics_telemetry/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '6.9.1'}, 1: {'versionInfo': '3.3.4'}}"}*

```diff
@@ -1,16 +1,16 @@
 {
     "packages": [
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "6.8.1"
+            "versionInfo": "6.9.1"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
-            "versionInfo": "3.3.3"
+            "versionInfo": "3.3.4"
         }
     ]
 }
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/schema/settings.json` & `jupyterlab_unianalytics_telemetry-4.0.9/schema/settings.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/PanelManager.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/PanelManager.ts`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import { NotebookPanel } from '@jupyterlab/notebook';
 import { isNotebookValid } from './utils/utils';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { WebsocketManager } from './websocket/WebsocketManager';
 import { EXTENSION_SETTING_NAME } from './utils/constants';
-import { InstanceInitializerDisposable } from './trackers/InstanceInitializerDisposable';
 import { CellMappingDisposable } from './trackers/CellMappingDisposable';
 import { ExecutionDisposable } from './trackers/ExecutionDisposable';
 import { AlterationDisposable } from './trackers/AlterationDisposable';
 import { FocusDisposable } from './trackers/FocusDisposable';
 import { Dialog, showDialog } from '@jupyterlab/apputils';
 import { disabledNotebooksSignaler } from '.';
 
@@ -29,23 +28,16 @@
     this._settings = settings;
     this._dialogShownSettings = dialogShownSettings;
 
     this._websocketManager = new WebsocketManager();
   }
 
   private _onSettingsChanged(settings: ISettingRegistry.ISettings) {
-    const prevSettingValue = this._isDataCollectionEnabled;
     this._isDataCollectionEnabled = settings.get(EXTENSION_SETTING_NAME)
       .composite as boolean;
-
-    // only act on trackers/websocket if the target setting value actually changed
-    if (this._isDataCollectionEnabled !== prevSettingValue) {
-      // removes the previous trackers and adds new ones if the setting is enabled
-      this._addOptionalTrackers();
-    }
   }
 
   get panel(): NotebookPanel | null {
     return this._panel;
   }
 
   set panel(value: NotebookPanel | null) {
@@ -84,55 +76,49 @@
         this._addAllTrackers();
       }
     });
   }
 
   private _addAllTrackers() {
     if (this._panel && this._panel.sessionContext.isReady) {
-      this._instanceInitializerDisposable = new InstanceInitializerDisposable(
-        this._panel
-      );
-
       this._cellMappingDisposable = new CellMappingDisposable(this._panel);
 
       this._addOptionalTrackers();
     }
   }
 
   private _addOptionalTrackers() {
     this._disposeFromOptionalTrackers();
     if (this._panel && this._panel.sessionContext.isReady) {
       // check if notebook is tagged
-      const notebookTags = isNotebookValid(this._panel);
-      if (notebookTags) {
-        // notebookTags is { notebookId, instanceId }
-
+      const notebookId = isNotebookValid(this._panel);
+      if (notebookId) {
         // prompt the user with a dialog box to enable/disable the extension (opt-in) the first time they see a tagged notebook
         this._showConsentDialogPromise().then(() => {
           if (
             this._panel &&
             !this._panel.isDisposed &&
             this._isDataCollectionEnabled
           ) {
             this._focusDisposable = new FocusDisposable(
               this._panel,
-              notebookTags
+              notebookId
             );
 
             this._executionDisposable = new ExecutionDisposable(
               this._panel,
-              notebookTags
+              notebookId
             );
 
             this._alterationDisposable = new AlterationDisposable(
               this._panel,
-              notebookTags
+              notebookId
             );
 
-            this._websocketManager.establishSocketConnection(notebookTags);
+            this._websocketManager.establishSocketConnection(notebookId);
           }
         });
       }
     }
   }
 
   private async _showConsentDialogPromise() {
@@ -170,18 +156,14 @@
       }
       // setting update might happen after the first cell and notebook clicks are sent, so call the update directly
       this._isDataCollectionEnabled = isEnabled;
     }
   }
 
   private _disposeFromAllTrackers() {
-    if (this._instanceInitializerDisposable) {
-      this._instanceInitializerDisposable.dispose();
-      this._instanceInitializerDisposable = null;
-    }
     if (this._cellMappingDisposable) {
       this._cellMappingDisposable.dispose();
       this._cellMappingDisposable = null;
     }
     this._disposeFromOptionalTrackers();
   }
 
@@ -211,14 +193,12 @@
   private _panel: NotebookPanel | null;
   private _ongoingContextId = '';
   private _websocketManager: WebsocketManager;
   private _isDataCollectionEnabled: boolean;
   private _settings: ISettingRegistry.ISettings;
   private _dialogShownSettings: ISettingRegistry.ISettings;
 
-  private _instanceInitializerDisposable: InstanceInitializerDisposable | null =
-    null;
   private _cellMappingDisposable: CellMappingDisposable | null = null;
   private _executionDisposable: ExecutionDisposable | null = null;
   private _alterationDisposable: AlterationDisposable | null = null;
   private _focusDisposable: FocusDisposable | null = null;
 }
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/api.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/api.ts`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,53 @@
-import { BACKEND_API_URL, MAX_PAYLOAD_SIZE } from './utils/constants';
+import { PERSISTENT_USER_ID } from '.';
+import { APP_ID, BACKEND_API_URL, MAX_PAYLOAD_SIZE } from './utils/constants';
 import {
   ICellAlterationObject,
   ICellClickObject,
   ICodeExecObject,
   INotebookClickObject,
   IMarkdownExecObject,
   PostDataObject
 } from './utils/types';
 
 const postRequest = (data: PostDataObject, endpoint: string): void => {
-  const payload = JSON.stringify(data);
-  const url = BACKEND_API_URL + endpoint;
-
-  if (payload.length > MAX_PAYLOAD_SIZE) {
-    console.log(
-      `Payload size exceeds limit of ${MAX_PAYLOAD_SIZE / 1024 / 1024} Mb`
-    );
+  if (!PERSISTENT_USER_ID) {
+    console.log(`${APP_ID}: No user id`);
     return;
   } else {
-    console.log('Posting to ' + endpoint + ' :\n', data);
-    fetch(url, {
-      method: 'POST',
-      headers: {
-        'Content-Type': 'application/json',
-        // add a nonce to avoid poluting the DB with MITM attacks
-        'X-Nonce': crypto.randomUUID()
-      },
-      body: payload
-    }).then(response => {
-      response.json().then(responseData => console.log(responseData));
-    });
+    // add the user_id to the payload
+    const dataWithUser = {
+      ...data,
+      user_id: PERSISTENT_USER_ID
+    };
+
+    const payload = JSON.stringify(dataWithUser);
+    const url = BACKEND_API_URL + endpoint;
+
+    if (payload.length > MAX_PAYLOAD_SIZE) {
+      console.log(
+        `${APP_ID}: Payload size exceeds limit of ${MAX_PAYLOAD_SIZE / 1024 / 1024} Mb`
+      );
+      return;
+    } else {
+      console.log(`${APP_ID}: Posting to ` + endpoint + ' :\n', dataWithUser);
+      fetch(url, {
+        method: 'POST',
+        headers: {
+          'Content-Type': 'application/json',
+          // add a nonce to avoid poluting the DB with MITM attacks
+          'X-Nonce': crypto.randomUUID()
+        },
+        body: payload
+      }).then(response => {
+        response
+          .json()
+          .then(responseData => console.log(`${APP_ID}: ` + responseData));
+      });
+    }
   }
 };
 
 export const postCodeExec = (cellExec: ICodeExecObject): void => {
   postRequest(cellExec, 'exec/code');
 };
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/dataCollectionPlugin.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/dataCollectionPlugin.ts`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import { JupyterFrontEnd, LabShell } from '@jupyterlab/application';
-import { PLUGIN_ID } from './utils/constants';
+import { APP_ID } from './utils/constants';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { PanelManager } from './PanelManager';
 import { NotebookPanel } from '@jupyterlab/notebook';
 
 export const dataCollectionPlugin = async (
   app: JupyterFrontEnd,
   settingRegistry: ISettingRegistry
@@ -12,23 +12,23 @@
   settingRegistry
     .load('@jupyterlab/notebook-extension:tracker')
     .then((nbTrackerSettings: ISettingRegistry.ISettings) => {
       nbTrackerSettings.set('recordTiming', true);
     })
     .catch(error =>
       console.log(
-        `${PLUGIN_ID}: Could not force cell execution metadata recording: ${error}`
+        `${APP_ID}: Could not force cell execution metadata recording: ${error}`
       )
     );
 
   try {
     // wait for this extension's settings to load
     const [settings, dialogShownSettings] = await Promise.all([
-      settingRegistry.load(`${PLUGIN_ID}:settings`),
-      settingRegistry.load(`${PLUGIN_ID}:dialogShownSettings`)
+      settingRegistry.load(`${APP_ID}:settings`),
+      settingRegistry.load(`${APP_ID}:dialogShownSettings`)
     ]);
 
     const panelManager = new PanelManager(settings, dialogShownSettings);
 
     const labShell = app.shell as LabShell;
 
     // update the panel when the active widget changes
@@ -37,15 +37,15 @@
     }
 
     // connect to current widget
     void app.restored.then(() => {
       onConnect(labShell, panelManager);
     });
   } catch (error) {
-    console.log(`${PLUGIN_ID}: Could not load settings, error: ${error}`);
+    console.log(`${APP_ID}: Could not load settings, error: ${error}`);
   }
 };
 
 function onConnect(labShell: LabShell, panelManager: PanelManager) {
   const widget = labShell.currentWidget;
   if (!widget) {
     return;
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/index.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/index.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
-import { PLUGIN_ID } from './utils/constants';
+import { APP_ID } from './utils/constants';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { LabIcon } from '@jupyterlab/ui-components';
 import { ISignal, Signal } from '@lumino/signaling';
 import { CompatibilityManager } from './utils/compatibility';
 import { compareVersions } from './utils/utils';
 import { dataCollectionPlugin } from './dataCollectionPlugin';
+import { requestAPI } from './handler';
 
 // to register the svg icon to reuse it in the settings (through schema/settings.json > jupyter.lab.setting-icon)
 import schemaStr from '../style/icons/dataCollection_cropped.svg';
 export const schemaIcon = new LabIcon({
-  name: `${PLUGIN_ID}:schema-icon`,
+  name: `${APP_ID}:schema-icon`,
   svgstr: schemaStr
 });
 
+// persistent user id retrieved from the server-side extension
+export let PERSISTENT_USER_ID: string | null = null;
+
 // class that holds the value of the disabledNotebooks list and emits a signal when the value changes
 class DisabledNotebooksSignaler {
   set value(newValue: string[] | null) {
     if (newValue === this._value) {
       return;
     }
     this._value = newValue;
@@ -42,25 +46,30 @@
 export const disabledNotebooksSignaler = new DisabledNotebooksSignaler();
 export let isDashboardExtensionInstalled = false;
 
 const activate = (
   app: JupyterFrontEnd,
   settingRegistry: ISettingRegistry
 ): void => {
-  console.log(`JupyterLab extension ${PLUGIN_ID} is activated!`);
+  console.log(`JupyterLab extension ${APP_ID} is activated!`);
+
+  requestAPI<string>('get_anonymized_user_id')
+    .then(data => {
+      PERSISTENT_USER_ID = data;
+    })
+    .catch(reason => {
+      console.error(
+        `${APP_ID}: server extension appears to be missing.\n${reason}`
+      );
+    });
 
   isDashboardExtensionInstalled = app
     .listPlugins()
     .some(item => item.includes('jupyterlab_unianalytics_dashboard'));
 
-  console.log(
-    'Is dashboard extension also installed ?',
-    isDashboardExtensionInstalled
-  );
-
   if (isDashboardExtensionInstalled) {
     // do something
     window.addEventListener('message', (event: any) => {
       // check that the message was emitted from the same origin
       if (
         event.origin === window.origin &&
         event.data &&
@@ -77,19 +86,21 @@
   if (appNumbers && compareVersions(app.version, targetVersion) >= 0) {
     const jupyterVersion = parseInt(appNumbers[0]);
 
     CompatibilityManager.setJupyterVersion(jupyterVersion);
 
     dataCollectionPlugin(app, settingRegistry);
   } else {
-    console.log(`Use a more recent version of JupyterLab (>=${targetVersion})`);
+    console.log(
+      `${APP_ID}: Use a more recent version of JupyterLab (>=${targetVersion})`
+    );
   }
 };
 
 const plugin: JupyterFrontEndPlugin<void> = {
-  id: `${PLUGIN_ID}:plugin`,
+  id: `${APP_ID}:plugin`,
   autoStart: true,
   requires: [ISettingRegistry],
   activate: activate
 };
 
 export default plugin;
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/trackers/AlterationDisposable.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/trackers/AlterationDisposable.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import { Signal } from '@lumino/signaling';
 import { IDisposable } from '@lumino/disposable';
 import { NotebookPanel } from '@jupyterlab/notebook';
 import { postCellAlteration } from '../api';
 import { CompatibilityManager } from '../utils/compatibility';
-import { NotebookTags } from '../utils/types';
 
 export class AlterationDisposable implements IDisposable {
-  constructor(panel: NotebookPanel, notebookTags: NotebookTags) {
-    this._notebookId = notebookTags.notebookId;
-    this._instanceId = notebookTags.instanceId;
+  constructor(panel: NotebookPanel, notebookId: string) {
+    this._notebookId = notebookId;
     this._cellIdList = CompatibilityManager.getCellIdsComp(
       panel.context.model.cells
     );
 
     // connect to notebook cell insertion/deletion/move/set
     panel.context.model.cells.changed.connect(this._onCellsAltered, this);
 
@@ -28,25 +26,23 @@
     );
     const removedIds: string[] = this._cellIdList.filter(
       item => !newCellIdList.includes(item)
     );
 
     for (const added_id of addedIds) {
       postCellAlteration({
-        notebook_id: this._notebookId as string,
-        instance_id: this._instanceId as string,
+        notebook_id: this._notebookId,
         cell_id: added_id,
         alteration_type: 'ADD',
         time: new Date().toISOString()
       });
     }
     for (const removed_id of removedIds) {
       postCellAlteration({
-        notebook_id: this._notebookId as string,
-        instance_id: this._instanceId as string,
+        notebook_id: this._notebookId,
         cell_id: removed_id,
         alteration_type: 'REMOVE',
         time: new Date().toISOString()
       });
     }
 
     this._cellIdList = newCellIdList;
@@ -69,10 +65,9 @@
     this._cellIdList = [];
 
     Signal.clearData(this);
   }
 
   private _isDisposed = false;
   private _notebookId: string;
-  private _instanceId: string;
   private _cellIdList: string[] = [];
 }
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/trackers/CellMappingDisposable.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/trackers/CellMappingDisposable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/trackers/ExecutionDisposable.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/trackers/ExecutionDisposable.ts`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 import { IDisposable } from '@lumino/disposable';
 import { Signal } from '@lumino/signaling';
 import { Cell, CodeCell, MarkdownCell } from '@jupyterlab/cells';
 import { processCellOutput } from '../utils/utils';
 import { postCodeExec, postMarkdownExec } from '../api';
 import { Selectors } from '../utils/constants';
 import { CompatibilityManager } from '../utils/compatibility';
-import { NotebookTags } from '../utils/types';
 
 export class ExecutionDisposable implements IDisposable {
-  constructor(panel: NotebookPanel, notebookTags: NotebookTags) {
+  constructor(panel: NotebookPanel, notebookId: string) {
     this._panel = panel;
 
-    this._notebookId = notebookTags.notebookId;
-    this._instanceId = notebookTags.instanceId;
+    this._notebookId = notebookId;
 
     // connect to cell execution
     NotebookActions.executed.connect(this._onCellExecuted, this);
 
     panel.disposed.connect(() =>
       NotebookActions.executed.disconnect(this._onCellExecuted, this)
     );
@@ -59,15 +57,14 @@
                 notebookModel,
                 Selectors.cellMapping
               )?.find(([key]: [key: string]) => key === cell.model.id)?.[1];
 
             if (orig_cell_id) {
               postCodeExec({
                 notebook_id: this._notebookId,
-                instance_id: this._instanceId,
                 language_mimetype:
                   CompatibilityManager.getMetadataComp(
                     notebookModel,
                     'language_info'
                   )['mimetype'] || 'text/plain',
                 cell_id: cell.model.id,
                 orig_cell_id: orig_cell_id,
@@ -88,15 +85,14 @@
           this._panel.model,
           Selectors.cellMapping
         )?.find(([key]: [key: string]) => key === cell.model.id)?.[1];
 
       if (orig_cell_id) {
         postMarkdownExec({
           notebook_id: this._notebookId,
-          instance_id: this._instanceId,
           cell_id: cell.model.id,
           orig_cell_id: orig_cell_id,
           time: new Date().toISOString(),
           cell_content: cell.model.sharedModel.getSource()
         });
       }
     }
@@ -115,9 +111,8 @@
 
     Signal.clearData(this);
   }
 
   private _panel: NotebookPanel;
   private _isDisposed = false;
   private _notebookId: string;
-  private _instanceId: string;
 }
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/trackers/FocusDisposable.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/trackers/FocusDisposable.ts`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import { Signal } from '@lumino/signaling';
 import { IDisposable } from '@lumino/disposable';
 import { Cell, ICellModel } from '@jupyterlab/cells';
 import { Notebook, NotebookPanel } from '@jupyterlab/notebook';
 import { postNotebookClick, postCellClick } from '../api';
 import { Selectors } from '../utils/constants';
 import { CompatibilityManager } from '../utils/compatibility';
-import { NotebookTags } from '../utils/types';
 
 type ClickType = 'OFF' | 'ON';
 
 export class FocusDisposable implements IDisposable {
-  constructor(panel: NotebookPanel, notebookTags: NotebookTags) {
+  constructor(panel: NotebookPanel, notebookId: string) {
     this._panel = panel;
 
-    this._notebookId = notebookTags.notebookId;
-    this._instanceId = notebookTags.instanceId;
+    this._notebookId = notebookId;
 
     this._sendNotebookClick('ON');
 
     // call it a first time after the panel is ready to send missed start-up signals
     this._onCellChanged(panel.content, panel.content.activeCell);
 
     // connect to active cell changes
@@ -70,16 +68,15 @@
         const cellEnd = new Date();
         cellDurationSec =
           (cellEnd.getTime() - this._cellStart.getTime()) / 1000;
       }
 
       if (this._lastOrigCellId) {
         postCellClick({
-          notebook_id: this._notebookId as string,
-          instance_id: this._instanceId as string,
+          notebook_id: this._notebookId,
           cell_id: this._lastActiveCellId,
           orig_cell_id: this._lastOrigCellId,
           click_type: clickType,
           time: new Date().toISOString(),
           click_duration: cellDurationSec
         });
       }
@@ -94,16 +91,15 @@
     } else {
       const notebookEnd = new Date();
       notebookDurationSec =
         (notebookEnd.getTime() - this._notebookStart.getTime()) / 1000;
     }
 
     postNotebookClick({
-      notebook_id: this._notebookId as string,
-      instance_id: this._instanceId as string,
+      notebook_id: this._notebookId,
       click_type: clickType,
       time: new Date().toISOString(),
       click_duration: notebookDurationSec
     });
   };
 
   get isDisposed(): boolean {
@@ -123,14 +119,13 @@
 
     Signal.clearData(this);
   }
 
   private _isDisposed = false;
   private _panel: NotebookPanel;
   private _notebookId: string;
-  private _instanceId: string;
   private _lastActiveCellId: string | null | undefined = null;
   private _lastOrigCellId: string | null | undefined = null;
 
   private _notebookStart: Date = new Date();
   private _cellStart: Date = new Date();
 }
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/utils/compatibility.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/utils/compatibility.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/utils/constants.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/utils/constants.ts`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 const LOCAL_DEV = false;
 
 export let BACKEND_API_URL: string, WEBSOCKET_API_URL: string;
 if (LOCAL_DEV) {
-  BACKEND_API_URL = 'http://localhost:5000/send/';
+  // LOCAL
+  BACKEND_API_URL = 'http://localhost:80/send/';
   WEBSOCKET_API_URL = 'ws://localhost:1337/ws';
+
+  // LOCAL W/ GATEWAY
+  // BACKEND_API_URL = 'http://localhost:1015/send/';
+  // WEBSOCKET_API_URL = 'ws://localhost:1015/ws';
+
+  // TEST NOTO
+  // BACKEND_API_URL = 'https://test-noto.epfl.ch/api/unilytics/send/';
+  // WEBSOCKET_API_URL = 'ws://test-noto.epfl.ch/api/unilytics/ws';
 } else {
   BACKEND_API_URL = 'https://api.unianalytics.ch/send/';
   WEBSOCKET_API_URL =
     'wss://ax5pzl8bwk.execute-api.eu-north-1.amazonaws.com/production/';
 }
 
-export const PLUGIN_ID = 'jupyterlab_unianalytics_telemetry';
+export const APP_ID = 'jupyterlab_unianalytics_telemetry';
 
 export const MAX_PAYLOAD_SIZE = 1048576; // 1*1024*1024 => 1Mb
 
 export const EXTENSION_SETTING_NAME = 'SendExtension';
 
-export const UNIANALYTICS_COOKIE_NAME = 'unianalytics-notebook-user-ids';
-
 // notebook metadata field names
 const SELECTOR_ID = 'unianalytics';
 export namespace Selectors {
   export const notebookId = `${SELECTOR_ID}_notebook_id`;
 
-  export const instanceId = `${SELECTOR_ID}_instance_id`;
-
   export const cellMapping = `${SELECTOR_ID}_cell_mapping`;
 }
 
 export namespace CommandIDs {
-  export const dashboardOpenChat = `${PLUGIN_ID}:unianalytics-open-chat`;
+  export const dashboardOpenChat = `${APP_ID}:unianalytics-open-chat`;
 }
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/utils/types.d.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/utils/types.d.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import { IOutput } from '@jupyterlab/nbformat';
 
 type StringId = string | null | undefined;
 
 interface IBaseEvent {
   notebook_id: string;
-  instance_id: string;
 }
 
 export interface ICodeExecObject extends IBaseEvent {
   cell_id: string;
   orig_cell_id: StringId;
   t_start: string;
   t_finish: string;
@@ -47,12 +46,7 @@
 
 export type PostDataObject =
   | ICodeExecObject
   | IMarkdownExecObject
   | INotebookClickObject
   | ICellClickObject
   | ICellAlterationObject;
-
-export type NotebookTags = {
-  notebookId: string;
-  instanceId: string;
-};
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/utils/utils.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/utils/utils.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import { IOutput, MultilineString, IMimeBundle } from '@jupyterlab/nbformat';
 import { PartialJSONObject } from '@lumino/coreutils';
 import { NotebookPanel } from '@jupyterlab/notebook';
-import { Selectors, UNIANALYTICS_COOKIE_NAME } from './constants';
+import { Selectors } from './constants';
 import { CompatibilityManager } from './compatibility';
-import { NotebookTags } from './types';
 import { disabledNotebooksSignaler, isDashboardExtensionInstalled } from '..';
 
-// returns the notebookId and instanceId if they are defined, null otherwise
-export const isNotebookValid = (panel: NotebookPanel): NotebookTags | null => {
+// returns the notebookId if defined, null otherwise
+export const isNotebookValid = (panel: NotebookPanel): string | null => {
   if (panel && !panel.isDisposed) {
     const notebookId = CompatibilityManager.getMetadataComp(
       panel.context.model,
       Selectors.notebookId
     );
     const cellMapping = CompatibilityManager.getMetadataComp(
       panel.context.model,
@@ -25,53 +24,21 @@
         if (
           disabledNotebooksSignaler.value === null ||
           disabledNotebooksSignaler.value.includes(notebookId)
         ) {
           return null;
         }
       }
-      const instanceId = getInstanceIdCookie(notebookId);
-      if (instanceId) {
-        return {
-          notebookId: notebookId,
-          instanceId: instanceId
-        };
-      }
-    }
-  }
-  return null;
-};
-
-const getInstanceIdCookie = (notebookId: string): string | null => {
-  const notebookIdCookieMap = getUnianalyticsCookie();
-  if (notebookIdCookieMap) {
-    return JSON.parse(notebookIdCookieMap)[notebookId];
-  } else {
-    return null;
-  }
-};
-
-export const getUnianalyticsCookie = (): string | null => {
-  const cookieString = document.cookie;
-  const cookies = cookieString.split(';');
 
-  for (const cookie of cookies) {
-    const [cookieName, cookieValue] = cookie.split('=').map(c => c.trim());
-    if (cookieName === UNIANALYTICS_COOKIE_NAME) {
-      return cookieValue;
+      return notebookId;
     }
   }
-
   return null;
 };
 
-export const setUnianalyticsCookie = (value: string): void => {
-  document.cookie = `${UNIANALYTICS_COOKIE_NAME}=${value}; expires=Fri, 31 Dec 9999 23:59:59 GMT; path=/`;
-};
-
 export const compareVersions = (version1: string, version2: string): number => {
   // extract numeric parts by splitting at non-digit characters
   const parts1 = version1.split(/[^0-9]+/).map(Number);
   const parts2 = version2.split(/[^0-9]+/).map(Number);
 
   for (let i = 0; i < Math.min(parts1.length, parts2.length); i++) {
     const num1 = parts1[i];
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/websocket/ChatExtension.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/websocket/ChatExtension.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/src/websocket/WebsocketManager.ts` & `jupyterlab_unianalytics_telemetry-4.0.9/src/websocket/WebsocketManager.ts`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,77 @@
-import { WEBSOCKET_API_URL } from '../utils/constants';
-import { NotebookTags } from '../utils/types';
+import { PERSISTENT_USER_ID } from '..';
+import { APP_ID, WEBSOCKET_API_URL } from '../utils/constants';
 
 export class WebsocketManager {
   constructor() {
     this._socket = null;
-    this._ongoingConnectionInfo = null;
 
     this._pingInterval = 540000; // 9min (AWS disconnects after 10min idle)
     this._pingTimer = null;
   }
 
-  private _createSocket(connectionInfo: NotebookTags) {
+  private _createSocket(notebookId: string, userId: string) {
     this._socket = new WebSocket(
-      `${WEBSOCKET_API_URL}?conType=STUDENT&nbId=${connectionInfo.notebookId}&usrId=${connectionInfo.instanceId}`
+      `${WEBSOCKET_API_URL}?conType=STUDENT&nbId=${notebookId}&usrId=${userId}`
     );
 
     this._socket.addEventListener('open', () => {
-      console.log('WebSocket connection opened for', connectionInfo);
+      console.log(`${APP_ID}: WebSocket connection opened for`, {
+        notebookId,
+        userId
+      });
 
       this._startPingTimer();
     });
 
     this._socket.addEventListener('message', event => {
       const message = JSON.parse(event.data);
       if (message.action === 'BLA BLA BLA') {
         // process the message
       }
-      console.log('Received message from server:', message);
+      console.log(`${APP_ID}: Received message from server:`, message);
       // Handle messages from the server
     });
 
     this._socket.addEventListener('close', event => {
-      console.log('WebSocket connection closed for ', connectionInfo, event);
+      console.log(
+        `${APP_ID}: WebSocket connection closed for `,
+        { notebookId, userId },
+        event
+      );
 
       this._stopPingTimer();
     });
 
     this._socket.addEventListener('error', event => {
-      console.error('WebSocket error', event);
+      console.error(`${APP_ID}: WebSocket error`, event);
     });
   }
 
-  public establishSocketConnection(connectionInfo: NotebookTags | null) {
+  public establishSocketConnection(notebookId: string | null) {
     // if there is already a connection, close it and set the socket to null
     this._closeSocketConnection();
 
-    this._ongoingConnectionInfo = connectionInfo;
-
-    if (!connectionInfo) {
+    if (!notebookId || !PERSISTENT_USER_ID) {
       return;
     }
-    this._createSocket(connectionInfo);
+    this._createSocket(notebookId, PERSISTENT_USER_ID);
   }
 
   // close the connection without resetting connection info in case the connection is closed with setting change
   private _closeSocketConnection() {
     if (this._socket) {
       this._socket.close();
     }
     this._socket = null;
   }
 
   // terminate connection when a panel is disposed/switched, reset connection info
   public terminateSocketConnection() {
     this._closeSocketConnection();
-    this._ongoingConnectionInfo = null;
   }
 
   private _startPingTimer() {
     this._pingTimer = window.setInterval(() => {
       if (this._socket && this._socket.readyState === WebSocket.OPEN) {
         this._socket.send('{ "action":"ping" }');
       }
@@ -79,11 +82,10 @@
     if (this._pingTimer) {
       clearInterval(this._pingTimer);
       this._pingTimer = null;
     }
   }
 
   private _socket: WebSocket | null;
-  private _ongoingConnectionInfo: NotebookTags | null;
   private _pingInterval: number;
   private _pingTimer: number | null;
 }
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/style/icons/chat3.svg` & `jupyterlab_unianalytics_telemetry-4.0.9/style/icons/chat3.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/style/icons/dataCollection_cropped.svg` & `jupyterlab_unianalytics_telemetry-4.0.9/style/icons/dataCollection_cropped.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/ui-tests/README.md` & `jupyterlab_unianalytics_telemetry-4.0.9/ui-tests/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Integration Testing
 
 This folder contains the integration tests of the extension.
 
 They are defined using [Playwright](https://playwright.dev/docs/intro) test runner
-and [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) helper.
+and [Galata](https://github.com/jupyterlab/jupyterlab/tree/main/galata) helper.
 
 The Playwright configuration is defined in [playwright.config.js](./playwright.config.js).
 
 The JupyterLab server configuration to use for the integration test is defined
 in [jupyter_server_test_config.py](./jupyter_server_test_config.py).
 
 The default configuration will produce video for failing tests and an HTML report.
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/ui-tests/yarn.lock` & `jupyterlab_unianalytics_telemetry-4.0.9/ui-tests/yarn.lock`

 * *Files 5% similar despite different names*

```diff
@@ -2,129 +2,129 @@
 # Manual changes might be lost - proceed with caution!
 
 __metadata:
   version: 6
   cacheKey: 8
 
 "@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.5.1, @codemirror/autocomplete@npm:^6.7.1":
-  version: 6.8.1
-  resolution: "@codemirror/autocomplete@npm:6.8.1"
+  version: 6.12.0
+  resolution: "@codemirror/autocomplete@npm:6.12.0"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
-    "@codemirror/view": ^6.6.0
+    "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
   peerDependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
-  checksum: 8599cd91defa3fea5276a7f9aff43ced323d9c4401dfb867e43608ba72ded48cb458256c5c784949a6332c0c20ba2fedac16a5708335cd809d269e4ea5076957
+  checksum: 1d4da6ccc12f5a67053a76b361f2683b5af031dd405a0bd2a261a265eb8cb7dfb115343a3291260d1ba31ce7ccb5427208ebe50f50f6747fcf27a50b62c87f7e
   languageName: node
   linkType: hard
 
 "@codemirror/commands@npm:^6.2.3":
-  version: 6.2.4
-  resolution: "@codemirror/commands@npm:6.2.4"
+  version: 6.3.3
+  resolution: "@codemirror/commands@npm:6.3.3"
   dependencies:
     "@codemirror/language": ^6.0.0
-    "@codemirror/state": ^6.2.0
+    "@codemirror/state": ^6.4.0
     "@codemirror/view": ^6.0.0
-    "@lezer/common": ^1.0.0
-  checksum: 468895fa19ff0554181b698c81f850820de5c0289cab92c44392fb127286f09ca72b921d6ea4353b70b616a4fd0c3667d86b6f917202a3ad2e196eb7b581f7b6
+    "@lezer/common": ^1.1.0
+  checksum: 7d23aecc973823969434b839aefa9a98bb47212d2ce0e6869ae903adbb5233aad22a760788fb7bb6eb45b00b01a4932fb93ad43bacdcbc0215e7500cf54b17bb
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
 
 "@codemirror/lang-css@npm:^6.0.0, @codemirror/lang-css@npm:^6.1.1":
-  version: 6.2.0
-  resolution: "@codemirror/lang-css@npm:6.2.0"
+  version: 6.2.1
+  resolution: "@codemirror/lang-css@npm:6.2.1"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.0.2
     "@lezer/css": ^1.0.0
-  checksum: d824f169083613b63f04992c24d3fecd45c718cd3deb9da3f332dd3a889a762d05ea812e31ddf7ee4b661722f8c8b49676515cb98609067c53e25ac8b469a5e4
+  checksum: 5a8457ee8a4310030a969f2d3128429f549c4dc9b7907ee8888b42119c80b65af99093801432efdf659b8ec36a147d2a947bc1ecbbf69a759395214e3f4834a8
   languageName: node
   linkType: hard
 
 "@codemirror/lang-html@npm:^6.0.0, @codemirror/lang-html@npm:^6.4.3":
-  version: 6.4.5
-  resolution: "@codemirror/lang-html@npm:6.4.5"
+  version: 6.4.8
+  resolution: "@codemirror/lang-html@npm:6.4.8"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/lang-css": ^6.0.0
     "@codemirror/lang-javascript": ^6.0.0
     "@codemirror/language": ^6.4.0
     "@codemirror/state": ^6.0.0
-    "@codemirror/view": ^6.2.2
+    "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
     "@lezer/css": ^1.1.0
     "@lezer/html": ^1.3.0
-  checksum: 08c6a55557f5491059f1b20d7788e64dcc37c488d4c97c00fa1c21af599ab48cdd7f839f3ffc6814480b9756c7a96845a36b578427b3c8d5efbfe123bf4553b9
+  checksum: 9aec56c333cc06f9e4bb6d09806ae83e4a7f235a26b3244010e2dcea83a923cfcd7bec84904b8a59bc81256b0bb579a52bf5614962dad031d7577db1c49a216a
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
 
 "@codemirror/lang-javascript@npm:^6.0.0, @codemirror/lang-javascript@npm:^6.1.7":
-  version: 6.1.9
-  resolution: "@codemirror/lang-javascript@npm:6.1.9"
+  version: 6.2.1
+  resolution: "@codemirror/lang-javascript@npm:6.2.1"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.6.0
     "@codemirror/lint": ^6.0.0
     "@codemirror/state": ^6.0.0
-    "@codemirror/view": ^6.0.0
+    "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
     "@lezer/javascript": ^1.0.0
-  checksum: 6c79b51c61d37b3f4dde6312df02183045c31f055e5cf8550b497f39798b823b4e380a641a2cfc97f3f26fd4e89194258d8ef741c42acd72b3f2e18257b427a5
+  checksum: 3df38c4cced06195283a9a2a9365aaa7c8c1b157852b331bc3a118403f774bbba57d2a392de52f5e28d2b344a323bc0146bcf7c8ef8be2473f167d815e4a37cd
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
 
 "@codemirror/lang-markdown@npm:^6.1.1":
-  version: 6.2.0
-  resolution: "@codemirror/lang-markdown@npm:6.2.0"
+  version: 6.2.4
+  resolution: "@codemirror/lang-markdown@npm:6.2.4"
   dependencies:
     "@codemirror/autocomplete": ^6.7.1
     "@codemirror/lang-html": ^6.0.0
     "@codemirror/language": ^6.3.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
-    "@lezer/common": ^1.0.0
+    "@lezer/common": ^1.2.1
     "@lezer/markdown": ^1.0.0
-  checksum: 0b2b5334abc8bb46fdaf0723fcddb9565b89c58d245ee0cced2c62c9c5de8430ad8bd73ab92d8a6bd67130173b59006bec2922e614e0277aa2b2d62f308113cf
+  checksum: fbdf1388a9fd08b4e6fc9950ac57fc59ef02bb0bd3e76654158ce1494b101356ded049b65dcf6da457e7e302cb178bf30852fd152680f3a8679be3c3884c0bc2
   languageName: node
   linkType: hard
 
 "@codemirror/lang-php@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-php@npm:6.0.1"
   dependencies:
@@ -133,15 +133,15 @@
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/php": ^1.0.0
   checksum: c003a29a426486453fdfddbf7302982fa2aa7f059bf6f1ce4cbf08341b0162eee5e2f50e0d71c418dcd358491631780156d846fe352754d042576172c5d86721
   languageName: node
   linkType: hard
 
-"@codemirror/lang-python@npm:^6.1.2":
+"@codemirror/lang-python@npm:^6.1.3":
   version: 6.1.3
   resolution: "@codemirror/lang-python@npm:6.1.3"
   dependencies:
     "@codemirror/autocomplete": ^6.3.2
     "@codemirror/language": ^6.8.0
     "@lezer/python": ^1.1.4
   checksum: 65a0276a4503e4e3b70dd28d1c93ef472632b6d2c4bf3ae92d305d14ee8cf60b0bbbf62d5ceb51294de9598d9e2d42eafcde26f317ee7b90d0a11dfa863c1d1a
@@ -155,34 +155,36 @@
     "@codemirror/language": ^6.0.0
     "@lezer/rust": ^1.0.0
   checksum: 8a439944cb22159b0b3465ca4fa4294c69843219d5d30e278ae6df8e48f30a7a9256129723c025ec9b5e694d31a3560fb004300b125ffcd81c22d13825845170
   languageName: node
   linkType: hard
 
 "@codemirror/lang-sql@npm:^6.4.1":
-  version: 6.5.2
-  resolution: "@codemirror/lang-sql@npm:6.5.2"
+  version: 6.5.5
+  resolution: "@codemirror/lang-sql@npm:6.5.5"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 29c7f3245271e50707939946e0aa3bae36d2fc392281c5a44bed38c886a5709611a8c68494d1f21c854dd70771ddb2cff2f0f26221b031653278ba2d5678a2b8
+  checksum: 404003ae73b986bd7a00f6924db78b7ffb28fdc38d689fdc11416aaafe2d5c6dc37cc18972530f82e940acb61e18ac74a1cf7712beef448c145344ff93970dc3
   languageName: node
   linkType: hard
 
 "@codemirror/lang-wast@npm:^6.0.1":
-  version: 6.0.1
-  resolution: "@codemirror/lang-wast@npm:6.0.1"
+  version: 6.0.2
+  resolution: "@codemirror/lang-wast@npm:6.0.2"
   dependencies:
     "@codemirror/language": ^6.0.0
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 600d98d3ea6a4e99292244ed707e39a2abd9f3abf62cfeff5c819a0cc0c7e86b8c5b91e91c1b7ea21233d9ea09c41abe61d8a40b2547bb5db74239c6df857934
+  checksum: 72119d4a7d726c54167aa227c982ae9fa785c8ad97a158d8350ae95eecfbd8028a803eef939f7e6c5c6e626fcecda1dc37e9dffc6d5d6ec105f686aeda6b2c24
   languageName: node
   linkType: hard
 
 "@codemirror/lang-xml@npm:^6.0.2":
   version: 6.0.2
   resolution: "@codemirror/lang-xml@npm:6.0.2"
   dependencies:
@@ -192,73 +194,73 @@
     "@lezer/common": ^1.0.0
     "@lezer/xml": ^1.0.0
   checksum: e156ecafaa87e9b6ef4ab6812ccd00d8f3c6cb81f232837636b36336d80513b61936dfee6f4f6800574f236208b61e95a2abcb997cdcd7366585a6b796e0e13b
   languageName: node
   linkType: hard
 
 "@codemirror/language@npm:^6.0.0, @codemirror/language@npm:^6.3.0, @codemirror/language@npm:^6.4.0, @codemirror/language@npm:^6.6.0, @codemirror/language@npm:^6.8.0":
-  version: 6.8.0
-  resolution: "@codemirror/language@npm:6.8.0"
+  version: 6.10.0
+  resolution: "@codemirror/language@npm:6.10.0"
   dependencies:
     "@codemirror/state": ^6.0.0
-    "@codemirror/view": ^6.0.0
-    "@lezer/common": ^1.0.0
+    "@codemirror/view": ^6.23.0
+    "@lezer/common": ^1.1.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
     style-mod: ^4.0.0
-  checksum: 64408d996641931fa4c6b892e17ee1fdaee0f63d3d84c019a6ea7b1e6d1c774f92357b95c2ebaed60545062b795b72d0a058c03578b2bf4023c87726e97b5d2f
+  checksum: 3bfd9968f5a34ce22434489a5b226db5f3bc454a1ae7c4381587ff4270ac6af61b10f93df560cb73e9a77cc13d4843722a7a7b94dbed02a3ab1971dd329b9e81
   languageName: node
   linkType: hard
 
 "@codemirror/legacy-modes@npm:^6.3.2":
-  version: 6.3.2
-  resolution: "@codemirror/legacy-modes@npm:6.3.2"
+  version: 6.3.3
+  resolution: "@codemirror/legacy-modes@npm:6.3.3"
   dependencies:
     "@codemirror/language": ^6.0.0
-  checksum: fa5f5477fb9e19267251e2ecd3de8c1a4c2512813555bb60111dce3951f2c3f6080a2985a573b7542534ba1d2c34115f7e39ee23fdf8f6f81db6f8ce447c1efc
+  checksum: 3cd32b0f011b0a193e0948e5901b625f38aa6d9a8b24344531d6e142eb6fbb3e6cb5969429102044f3d04fbe53c4deaebd9f659c05067a0b18d17766290c9e05
   languageName: node
   linkType: hard
 
 "@codemirror/lint@npm:^6.0.0":
-  version: 6.4.0
-  resolution: "@codemirror/lint@npm:6.4.0"
+  version: 6.4.2
+  resolution: "@codemirror/lint@npm:6.4.2"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
-  checksum: ba15f7dd87afbceafaa0b68f94b0d53727e4aacca7a81a4ed3278706df5787fdf18cd3f0d807a136f902b2fc2296bf3490462fd543d1d4ced17a0d8c171820fd
+  checksum: 5e699960c1b28dbaa584fe091a3201978907bf4b9e52810fb15d3ceaf310e38053435e0b594da0985266ae812039a5cd6c36023284a6f8568664bdca04db137f
   languageName: node
   linkType: hard
 
 "@codemirror/search@npm:^6.3.0":
-  version: 6.5.0
-  resolution: "@codemirror/search@npm:6.5.0"
+  version: 6.5.5
+  resolution: "@codemirror/search@npm:6.5.5"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
-  checksum: 2e9f2344b7dbd4bad79058c105d8cbd02b2bf94c27495310f0e3b6e999010aa080dceea47ef46e35439cc9e131b47c46f7d2eda700ef491b5f2f34bbc8e145ab
+  checksum: 825196ef63273494ba9a6153b01eda385edb65e77a1e49980dd3a28d4a692af1e9575e03e4b6c84f6fa2afe72217113ff4c50f58b20d13fe0d277cda5dd7dc81
   languageName: node
   linkType: hard
 
-"@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.1.4, @codemirror/state@npm:^6.2.0":
-  version: 6.2.1
-  resolution: "@codemirror/state@npm:6.2.1"
-  checksum: d12a321d0471b264b9d3259042bff913a8b939e8d28d408ff452004538a71ca9d5329df3f8a1d8a9183f5b42a7ef5b200737bcab1065714f5ae8e0a5ba9d59d3
+"@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.2.0, @codemirror/state@npm:^6.4.0":
+  version: 6.4.0
+  resolution: "@codemirror/state@npm:6.4.0"
+  checksum: c5236fe5786f1b85d17273a5c17fa8aeb063658c1404ab18caeb6e7591663ec96b65d453ab8162f75839c3801b04cd55ba4bc48f44cb61ebfeeee383f89553c7
   languageName: node
   linkType: hard
 
-"@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.2.2, @codemirror/view@npm:^6.6.0, @codemirror/view@npm:^6.9.6":
-  version: 6.14.1
-  resolution: "@codemirror/view@npm:6.14.1"
+"@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.17.0, @codemirror/view@npm:^6.23.0, @codemirror/view@npm:^6.9.6":
+  version: 6.23.1
+  resolution: "@codemirror/view@npm:6.23.1"
   dependencies:
-    "@codemirror/state": ^6.1.4
-    style-mod: ^4.0.0
+    "@codemirror/state": ^6.4.0
+    style-mod: ^4.1.0
     w3c-keyname: ^2.2.4
-  checksum: 19114ee05b3795ebe07a69cf00c36e8351b3500ce105b8412d90e757d459f71370ead3de852f0fda069041803276e6c38e6f1f943f77e85c9b5c279ab7fa1c4a
+  checksum: 5ea3ba5761c574e1f6e1f1058cb452189c890982a77991606d0ae40da3c6fff77f7c7fc3c43fa78d62677ccdfa65dbc56175706b793e34ad4ec7a63b21e8c18e
   languageName: node
   linkType: hard
 
 "@fortawesome/fontawesome-free@npm:^5.12.0":
   version: 5.15.4
   resolution: "@fortawesome/fontawesome-free@npm:5.15.4"
   checksum: 32281c3df4075290d9a96dfc22f72fadb3da7055d4117e48d34046b8c98032a55fa260ae351b0af5d6f6fb57a2f5d79a4abe52af456da35195f7cb7dda27b4a2
@@ -275,995 +277,1019 @@
     strip-ansi-cjs: "npm:strip-ansi@^6.0.1"
     wrap-ansi: ^8.1.0
     wrap-ansi-cjs: "npm:wrap-ansi@^7.0.0"
   checksum: 4a473b9b32a7d4d3cfb7a614226e555091ff0c5a29a1734c28c72a182c2f6699b26fc6b5c2131dfd841e86b185aea714c72201d7c98c2fba5f17709333a67aeb
   languageName: node
   linkType: hard
 
-"@jupyter/ydoc@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "@jupyter/ydoc@npm:1.0.2"
+"@jupyter/ydoc@npm:^1.1.1":
+  version: 1.1.1
+  resolution: "@jupyter/ydoc@npm:1.1.1"
   dependencies:
     "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0
     "@lumino/coreutils": ^1.11.0 || ^2.0.0
     "@lumino/disposable": ^1.10.0 || ^2.0.0
     "@lumino/signaling": ^1.10.0 || ^2.0.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
-  checksum: 739f9630940466b3cfcd7b742dd06479f81772ca13f863d057af0bbb5e318829506969066ab72977e7c721644982b5c8f88cf44e1ae81955ed1c27e87632d1f2
+  checksum: a239b1dd57cfc9ba36c06ac5032a1b6388849ae01a1d0db0d45094f71fdadf4d473b4bf8becbef0cfcdc85cae505361fbec0822b02da5aa48e06b66f742dd7a0
   languageName: node
   linkType: hard
 
-"@jupyterlab/application@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/application@npm:4.0.2"
+"@jupyterlab/application@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/application@npm:4.0.11"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/statedb": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/application": ^2.1.1
-    "@lumino/commands": ^2.1.1
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/polling": ^2.1.1
-    "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/widgets": ^2.1.1
-  checksum: 5709b59c794e481d6e9b6c5575042c569f38058b6fc2a2c1d2831bdd0d1b0ff4df60c17132753ed8d9be1e2a28e4a0a18310d2b80e8ff5812fdaccbb1ee18bce
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/statedb": ^4.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/application": ^2.2.1
+    "@lumino/commands": ^2.1.3
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/polling": ^2.1.2
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.0
+  checksum: 9df885a5369cd43bc6636ef24afaa4bb371f3fff8940e3487bdb5e0de4b6a70bb33b43c6a50da69590c563b4d3e04f5219de0239a7aa859ffac7d3d1e017d23f
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:^4.1.2":
-  version: 4.1.2
-  resolution: "@jupyterlab/apputils@npm:4.1.2"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/settingregistry": ^4.0.2
-    "@jupyterlab/statedb": ^4.0.2
-    "@jupyterlab/statusbar": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/commands": ^2.1.1
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/domutils": ^2.0.0
-    "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/virtualdom": ^2.0.0
-    "@lumino/widgets": ^2.1.1
+"@jupyterlab/apputils@npm:^4.1.11":
+  version: 4.1.11
+  resolution: "@jupyterlab/apputils@npm:4.1.11"
+  dependencies:
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/settingregistry": ^4.0.11
+    "@jupyterlab/statedb": ^4.0.11
+    "@jupyterlab/statusbar": ^4.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/commands": ^2.1.3
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/domutils": ^2.0.1
+    "@lumino/messaging": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/virtualdom": ^2.0.1
+    "@lumino/widgets": ^2.3.0
     "@types/react": ^18.0.26
     react: ^18.2.0
     sanitize-html: ~2.7.3
-  checksum: 89a445478b54d1132e753022a81393dd3e53f7f36de2d9e905ece3bae911382ddff6afc16c4b649646b1a125c774ccc83fa4d92e29a48a423d4410a4a5554bb4
+  checksum: ab1bfa8e95de86464c35a2460e9cc4f89594a2cb69b38c19fd6d17a1c3d89e5c9fb368a1ac5425b5190c407e64c305c428e076a701117fc9007d0176bfe98501
   languageName: node
   linkType: hard
 
-"@jupyterlab/attachments@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/attachments@npm:4.0.2"
+"@jupyterlab/attachments@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/attachments@npm:4.0.11"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@lumino/disposable": ^2.1.1
-    "@lumino/signaling": ^2.1.1
-  checksum: 178d6abf3ff0767d87f78a79470760cf0025c3171e65dfd9a07916f3f6322f1080a21985ccdfdfeeec6fb73fb9aac9179cc413c43e4e33a45bcbcefa6cb97714
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@lumino/disposable": ^2.1.2
+    "@lumino/signaling": ^2.1.2
+  checksum: 13792a1a69280e48fcdaa5405042dad9135a1696197f40527a0c7c250285eab4330436df8cfa4e84b10f60ab07f4674c7abc89f98c50576061ca02c609458a84
   languageName: node
   linkType: hard
 
-"@jupyterlab/cells@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/cells@npm:4.0.2"
+"@jupyterlab/cells@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/cells@npm:4.0.11"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/attachments": ^4.0.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/codemirror": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/documentsearch": ^4.0.2
-    "@jupyterlab/filebrowser": ^4.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/outputarea": ^4.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/toc": ^6.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/domutils": ^2.0.0
-    "@lumino/dragdrop": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/polling": ^2.1.1
-    "@lumino/signaling": ^2.1.1
-    "@lumino/virtualdom": ^2.0.0
-    "@lumino/widgets": ^2.1.1
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/attachments": ^4.0.11
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/codemirror": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/documentsearch": ^4.0.11
+    "@jupyterlab/filebrowser": ^4.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/outputarea": ^4.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/toc": ^6.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/domutils": ^2.0.1
+    "@lumino/dragdrop": ^2.1.4
+    "@lumino/messaging": ^2.0.1
+    "@lumino/polling": ^2.1.2
+    "@lumino/signaling": ^2.1.2
+    "@lumino/virtualdom": ^2.0.1
+    "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: 92aa9ced743b41fbe5c0d3700762e3f825c9b01fb9b5684c909de330a62561a7b05af27390ca5993f905ec7141fa01072446b51232a8616181dd4eaed178b77f
+  checksum: c0d554269b0ab598f6ee197e76e3d3aaadf2a17bee778b899f00d2446ca51b1846b03771fb69fbce6009f50c62e8c2d7cfb6f1bcb763d7bd70a6e4f809c7a4d7
   languageName: node
   linkType: hard
 
-"@jupyterlab/codeeditor@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/codeeditor@npm:4.0.2"
+"@jupyterlab/codeeditor@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/codeeditor@npm:4.0.11"
   dependencies:
     "@codemirror/state": ^6.2.0
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/statusbar": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/dragdrop": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/widgets": ^2.1.1
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/statusbar": ^4.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/dragdrop": ^2.1.4
+    "@lumino/messaging": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: 61b638011acd21195fcd53b3b1f1df54abef0e0db85937f41f3a323cc6df75bcd63261739518bfd82b6bf45f638a090687cb43c2b66880546cff3e962d2e5994
+  checksum: 65e3a5ad115fd288d4389b90e0d475051192f361d9ac119d3b75d150db973c735638051474dae18a3fca9ba8e986ea33b57ed424f1c444bafcd60b3e47e548f3
   languageName: node
   linkType: hard
 
-"@jupyterlab/codemirror@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/codemirror@npm:4.0.2"
+"@jupyterlab/codemirror@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/codemirror@npm:4.0.11"
   dependencies:
     "@codemirror/autocomplete": ^6.5.1
     "@codemirror/commands": ^6.2.3
     "@codemirror/lang-cpp": ^6.0.2
     "@codemirror/lang-css": ^6.1.1
     "@codemirror/lang-html": ^6.4.3
     "@codemirror/lang-java": ^6.0.1
     "@codemirror/lang-javascript": ^6.1.7
     "@codemirror/lang-json": ^6.0.1
     "@codemirror/lang-markdown": ^6.1.1
     "@codemirror/lang-php": ^6.0.1
-    "@codemirror/lang-python": ^6.1.2
+    "@codemirror/lang-python": ^6.1.3
     "@codemirror/lang-rust": ^6.0.1
     "@codemirror/lang-sql": ^6.4.1
     "@codemirror/lang-wast": ^6.0.1
     "@codemirror/lang-xml": ^6.0.2
     "@codemirror/language": ^6.6.0
     "@codemirror/legacy-modes": ^6.3.2
     "@codemirror/search": ^6.3.0
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/documentsearch": ^4.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/documentsearch": ^4.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/translation": ^4.0.11
     "@lezer/common": ^1.0.2
     "@lezer/generator": ^1.2.2
     "@lezer/highlight": ^1.1.4
     "@lezer/markdown": ^1.0.2
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/signaling": ^2.1.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/signaling": ^2.1.2
     yjs: ^13.5.40
-  checksum: 1ddf08979874fc522eb88de6a743129640c5721410a8c6feb58d2e37b35ebcdeee5c217890e7f9561a595ca8b1c9b4a222b07da5e2e95c1e2dcd8c467378c50d
+  checksum: e4d16faad69575a6d3c4e41ab3cc268475c92f0783ca14013dc701cc2f12ee4eb7b37c1a650d9e60f17fe4daf0fba303e7cb984e06e9fde587c8075bbee7f1c8
   languageName: node
   linkType: hard
 
-"@jupyterlab/console@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/console@npm:4.0.2"
+"@jupyterlab/console@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/console@npm:4.0.11"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/cells": ^4.0.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/dragdrop": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/widgets": ^2.1.1
-  checksum: 4a7a4a8a06663902840c4216b257e380105366c7808f5f4ba891d45fb60b4f7605c455d2d0290dcc576dcc4c833a00d140c71604ecbeab3f2054c460fd6bbc79
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/cells": ^4.0.11
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/dragdrop": ^2.1.4
+    "@lumino/messaging": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.0
+  checksum: a7818d11d49acb7c3f44b8e8b984075548fe70b1c34aa1a8ad6dc3edf2b1514e4740773fc5869bf61cad0684bcba471b740dbf5ff1fd1b4f6d9428bdc81d31c3
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^6.0.2":
-  version: 6.0.2
-  resolution: "@jupyterlab/coreutils@npm:6.0.2"
-  dependencies:
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/signaling": ^2.1.1
+"@jupyterlab/coreutils@npm:^6.0.11":
+  version: 6.0.11
+  resolution: "@jupyterlab/coreutils@npm:6.0.11"
+  dependencies:
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/signaling": ^2.1.2
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
-  checksum: c2e9b9bf7227f68bb6b91044d2ac3808a872ac967e22f6aee10241d5dbc78a19deee65f91dd87c080f63170a760c96c99cb31e0e0b6f32c6341e432d781355ce
+  checksum: 2a3ab30865439d486ad180c0779bf086992d5999727e1fb4cbadad6ecd4c53fbcfcde4fc611d9819dc28aedc6b36e7b48d267ff2bcdd8f35de5b4f3d7145f2cc
   languageName: node
   linkType: hard
 
-"@jupyterlab/debugger@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/debugger@npm:4.0.2"
+"@jupyterlab/debugger@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/debugger@npm:4.0.11"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/application": ^4.0.2
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/cells": ^4.0.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/codemirror": ^4.0.2
-    "@jupyterlab/console": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/fileeditor": ^4.0.2
-    "@jupyterlab/notebook": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/commands": ^2.1.1
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/datagrid": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/polling": ^2.1.1
-    "@lumino/signaling": ^2.1.1
-    "@lumino/widgets": ^2.1.1
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/application": ^4.0.11
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/cells": ^4.0.11
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/codemirror": ^4.0.11
+    "@jupyterlab/console": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/fileeditor": ^4.0.11
+    "@jupyterlab/notebook": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/commands": ^2.1.3
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/datagrid": ^2.2.0
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/polling": ^2.1.2
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.0
     "@vscode/debugprotocol": ^1.51.0
     react: ^18.2.0
-  checksum: 5217fdca41a58397d97c6ca634f0e51f1f102e713c685748aaf04ab01b3e386d26d03881e27c5df66b422d7288a3b276008c59e056c1c068bf2629395887c251
+  checksum: 7bd03de7ba4ebe1df628eb903e950527ef624d30aabe3624d91138d4f3aa44ec72f6b93b8219f3eda32775c289a41f48fdef71909f741afb7078d9735ad547d4
   languageName: node
   linkType: hard
 
-"@jupyterlab/docmanager@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/docmanager@npm:4.0.2"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/statusbar": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/widgets": ^2.1.1
+"@jupyterlab/docmanager@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/docmanager@npm:4.0.11"
+  dependencies:
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/statusbar": ^4.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: dca1f56209608a82eebb0a365657f955bc8c546d66e00ec7747e753e3c76c8c0a5ed24b51736d157d2ed9d8264dc69545221e8fc2aa6af3eb6ec7eb4fd537a69
+  checksum: 964f85cceb54866bb3c603d5d7b3d3f064cb481917ae1e1f6aaf16fe2fb2a0863a9ab8427b82e72eed171e3ae80043b0de72e514dce0a4a0feb46e39c2faf9a0
   languageName: node
   linkType: hard
 
-"@jupyterlab/docregistry@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/docregistry@npm:4.0.2"
-  dependencies:
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/widgets": ^2.1.1
-  checksum: b88c6a6ab7825aff95541c8a9f4381ccee4533e8c5bda588538c8a110dd8c6cb413e73345bc8fbf74aebe9fed4f9d298de6efa08378212869510e81ccb9f10ca
+"@jupyterlab/docregistry@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/docregistry@npm:4.0.11"
+  dependencies:
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.0
+  checksum: 0c08ec3660f17b6d45aae030215a008278e82068b94bdd1bb77ec4e2995b5ef974830e90a78f5b46e7863204bab1ac397306c5d65901fed4f6bca5e57b4cbe05
   languageName: node
   linkType: hard
 
-"@jupyterlab/documentsearch@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/documentsearch@npm:4.0.2"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/polling": ^2.1.1
-    "@lumino/signaling": ^2.1.1
-    "@lumino/widgets": ^2.1.1
+"@jupyterlab/documentsearch@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/documentsearch@npm:4.0.11"
+  dependencies:
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/polling": ^2.1.2
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: d621722648f8d0e9c17c4df093bf02de0b3c5c1e8cb4b4b46482114700c4ca47dbb35831d2f046b0a28c950c6cd7442cdd791357af87d6e4df5da3b347d463e0
+  checksum: 1fa0087c6a0bc40e653a8e67f362b8765558ff9e1c6cf4dedb2e010cdd5112d863d9f10804f36dc22d79f41ad0757c54446af923337ad27e922f972881141bd4
   languageName: node
   linkType: hard
 
-"@jupyterlab/filebrowser@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/filebrowser@npm:4.0.2"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docmanager": ^4.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/statedb": ^4.0.2
-    "@jupyterlab/statusbar": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/domutils": ^2.0.0
-    "@lumino/dragdrop": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/polling": ^2.1.1
-    "@lumino/signaling": ^2.1.1
-    "@lumino/virtualdom": ^2.0.0
-    "@lumino/widgets": ^2.1.1
+"@jupyterlab/filebrowser@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/filebrowser@npm:4.0.11"
+  dependencies:
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docmanager": ^4.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/statedb": ^4.0.11
+    "@jupyterlab/statusbar": ^4.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/domutils": ^2.0.1
+    "@lumino/dragdrop": ^2.1.4
+    "@lumino/messaging": ^2.0.1
+    "@lumino/polling": ^2.1.2
+    "@lumino/signaling": ^2.1.2
+    "@lumino/virtualdom": ^2.0.1
+    "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: ae5426f6811488cb90538f8ec74fa87d4ead847a2727ba64d35b4b2d81e6058bc6340853affedb2e4e7362627453b8dd1e108142a425bc039745714058ce5d73
+  checksum: d4a452fd6e0772a79d662537a8abf10f83c1a66739813e73bf9218ef8c94b388bdfdb2919d97e135b914c40abfed551cb43b7bcc92b3bb896f99f3e5584d257f
   languageName: node
   linkType: hard
 
-"@jupyterlab/fileeditor@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/fileeditor@npm:4.0.2"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/codemirror": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/documentsearch": ^4.0.2
-    "@jupyterlab/lsp": ^4.0.2
-    "@jupyterlab/statusbar": ^4.0.2
-    "@jupyterlab/toc": ^6.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/commands": ^2.1.1
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/widgets": ^2.1.1
+"@jupyterlab/fileeditor@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/fileeditor@npm:4.0.11"
+  dependencies:
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/codemirror": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/documentsearch": ^4.0.11
+    "@jupyterlab/lsp": ^4.0.11
+    "@jupyterlab/statusbar": ^4.0.11
+    "@jupyterlab/toc": ^6.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/commands": ^2.1.3
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/widgets": ^2.3.0
     react: ^18.2.0
     regexp-match-indices: ^1.0.2
-  checksum: a83615c1094a143eb58701ba1f90f180d0e373d36db6d4aabebb73b26da7efaa47fd1946541cc529672b9042c66df1b2f23894267fe4afb5712a97cad42e471e
+  checksum: 27b812a55ac1f91fe149d71ea0e1b93b19f725d270292bb2351d60707d5a293e922cec8b5a7b90c33601ef4fbbe64f8f408d0208b260a62da4bad7028f81cd2e
   languageName: node
   linkType: hard
 
-"@jupyterlab/galata@npm:^5.0.0":
-  version: 5.0.2
-  resolution: "@jupyterlab/galata@npm:5.0.2"
-  dependencies:
-    "@jupyterlab/application": ^4.0.2
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/debugger": ^4.0.2
-    "@jupyterlab/docmanager": ^4.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/notebook": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/settingregistry": ^4.0.2
-    "@lumino/coreutils": ^2.1.1
+"@jupyterlab/galata@npm:^5.0.5":
+  version: 5.0.11
+  resolution: "@jupyterlab/galata@npm:5.0.11"
+  dependencies:
+    "@jupyterlab/application": ^4.0.11
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/debugger": ^4.0.11
+    "@jupyterlab/docmanager": ^4.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/notebook": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/settingregistry": ^4.0.11
+    "@lumino/coreutils": ^2.1.2
     "@playwright/test": ^1.32.2
     "@stdlib/stats": ~0.0.13
     fs-extra: ^10.1.0
     json5: ^2.2.3
     path: ~0.12.7
     systeminformation: ^5.8.6
     vega: ^5.20.0
     vega-lite: ^5.6.1
     vega-statistics: ^1.7.9
-  checksum: 175538962b02780fb3ce9ac0dc8ccb3f977f936ad18af1129272ddab0594eac0e8b1d911b3b902f18b0ab832dae689dea0eda51a202403507fef72df4d6fdaa8
+  checksum: d237be587b538297f77375ea4e20cf97acedcbcc47ce0a1d38f69e9787017b9dabe7badf56c091f6ae62758b29658e13787aaab7c6937a66ba0067995a44f70b
   languageName: node
   linkType: hard
 
-"@jupyterlab/lsp@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/lsp@npm:4.0.2"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/signaling": ^2.1.1
+"@jupyterlab/lsp@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/lsp@npm:4.0.11"
+  dependencies:
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/signaling": ^2.1.2
     lodash.mergewith: ^4.6.1
     vscode-jsonrpc: ^6.0.0
     vscode-languageserver-protocol: ^3.17.0
     vscode-ws-jsonrpc: ~1.0.2
-  checksum: 476517f4cd9ce7758638f96c1037f26d758ec8e102d87b9472cbaa6208d94bcfc1da0ec853202761f6542404a034932657b14f82e2355d312b3f0c5c140cfbfd
+  checksum: e2ca0286320c1c7855cf5c2eecf301037202de4df1e53ac109affd73b41c686a27e6205591f7a0ca85376d595db3e4779a423599c18745df24df93ad124be1a0
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/nbformat@npm:4.0.2"
-  dependencies:
-    "@lumino/coreutils": ^2.1.1
-  checksum: cccd1c7fd8717ccece1f7642f3f7218103c3baa479fce85666770719b3359116e5279cdd97e2b584122a793b437fc9ece7055d1da27ad35a090f90398a76d59f
+"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/nbformat@npm:4.0.11"
+  dependencies:
+    "@lumino/coreutils": ^2.1.2
+  checksum: 7bb488e94f09d66d858ce2a001e208beca9f1e87fc674332c4630cfb5039a6bd1579d9071019782aba546a9b43e2a7de5b125f7a0a7a7caa0b190a2b8d1266b6
   languageName: node
   linkType: hard
 
-"@jupyterlab/notebook@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/notebook@npm:4.0.2"
-  dependencies:
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/cells": ^4.0.2
-    "@jupyterlab/codeeditor": ^4.0.2
-    "@jupyterlab/codemirror": ^4.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/documentsearch": ^4.0.2
-    "@jupyterlab/lsp": ^4.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/settingregistry": ^4.0.2
-    "@jupyterlab/statusbar": ^4.0.2
-    "@jupyterlab/toc": ^6.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/domutils": ^2.0.0
-    "@lumino/dragdrop": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/virtualdom": ^2.0.0
-    "@lumino/widgets": ^2.1.1
+"@jupyterlab/notebook@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/notebook@npm:4.0.11"
+  dependencies:
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/cells": ^4.0.11
+    "@jupyterlab/codeeditor": ^4.0.11
+    "@jupyterlab/codemirror": ^4.0.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/documentsearch": ^4.0.11
+    "@jupyterlab/lsp": ^4.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/settingregistry": ^4.0.11
+    "@jupyterlab/statusbar": ^4.0.11
+    "@jupyterlab/toc": ^6.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/domutils": ^2.0.1
+    "@lumino/dragdrop": ^2.1.4
+    "@lumino/messaging": ^2.0.1
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/virtualdom": ^2.0.1
+    "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: 053cde5377aceac7ff6fe30e734354df1839cbf84bfd19f7d3992a1aaddcd66f5c8470bb2537c94b28dfdb194dfdacfaa38207fd2d4989b0575b27c20396bbfe
+  checksum: e8bbfca1cba7b78427fcca1211266ba989e4950da2361a3606a6ab8485ab4618c6f1a321463a8974b96c7a77d4d00ed9b293abf68f9ce84731bd0e9687ec8be7
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^5.0.2":
-  version: 5.0.2
-  resolution: "@jupyterlab/observables@npm:5.0.2"
-  dependencies:
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-  checksum: 6d206873f3e2bfd95267fde6fae565eef5c1f7df93dc0a27091ea3eceea5cbded6c8b90eb5d4311e3b6158385455ed358602cb4b3daee717f6cc195b259cfb24
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/outputarea@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/outputarea@npm:4.0.2"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/widgets": ^2.1.1
-  checksum: 8387b93e7b6bf1a63495eef8a7746870e4210818ff26af5c8ecdf4b9e78433ec47b58ddaa5ab11fbf5cf143802b23a186c90589974cd408cae95330fa3960f32
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/rendermime-interfaces@npm:^3.8.2":
-  version: 3.8.2
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.2"
-  dependencies:
-    "@lumino/coreutils": ^1.11.0 || ^2.1.1
-    "@lumino/widgets": ^1.37.2 || ^2.1.1
-  checksum: e1164a4ad7654e5e8af0c1c2f1c8938f01a4bd07e04ff788e8b3adfaa9cb7ef07118c44513648c69263929e1658f02dcbab7aac776c6071228b0b80c8ca4e65a
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/rendermime@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/rendermime@npm:4.0.2"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/widgets": ^2.1.1
+"@jupyterlab/observables@npm:^5.0.11":
+  version: 5.0.11
+  resolution: "@jupyterlab/observables@npm:5.0.11"
+  dependencies:
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+  checksum: b47cc8e73db9cc856454c0db530b774a4d11f6ade066b52fe521b0cec2b7a8f5eebfe2c0f0f7ada976474698dab9a77bdef3feea2960ea75bcf7052404ebec16
+  languageName: node
+  linkType: hard
+
+"@jupyterlab/outputarea@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/outputarea@npm:4.0.11"
+  dependencies:
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.0
+  checksum: f9c69319d0bd144f35840d72784b606153fe62d44b51a22f11ab4ee7088a262955dff4ea86de8b1bd929841294c8c5a3fadff37fa46b15ca53586868bb498cad
+  languageName: node
+  linkType: hard
+
+"@jupyterlab/rendermime-interfaces@npm:^3.8.11":
+  version: 3.8.11
+  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.11"
+  dependencies:
+    "@lumino/coreutils": ^1.11.0 || ^2.1.2
+    "@lumino/widgets": ^1.37.2 || ^2.3.0
+  checksum: 277373ca5e05bfbcd6e88c38cdf5c1bdfc052beaf1cac120cb3a458d96cce949b17c9b47cfd16cfcf2e2241530fa9f3062343512084b79a549f6bde84a846c84
+  languageName: node
+  linkType: hard
+
+"@jupyterlab/rendermime@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/rendermime@npm:4.0.11"
+  dependencies:
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/translation": ^4.0.11
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.0
     lodash.escape: ^4.0.1
-  checksum: 6118adf39cfe3c5918c9b677ff5d8dbe97ce469427f9969e1d16fba944b53d6e6c9d2c1e2deaaf928cdb94222a8941c7bb7cfc81693683fd07c08e92bc3d6cea
+  checksum: cb76d6824caac3b50e4e38c171f7db7239deb4499b0be237d51c68b3195c4d2edb1e4fa42253183949459ae0b78a1acbdc936b1eba51c8472bcf89586d267975
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^7.0.2":
-  version: 7.0.2
-  resolution: "@jupyterlab/services@npm:7.0.2"
-  dependencies:
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/settingregistry": ^4.0.2
-    "@jupyterlab/statedb": ^4.0.2
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/polling": ^2.1.1
-    "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.1.1
+"@jupyterlab/services@npm:^7.0.11":
+  version: 7.0.11
+  resolution: "@jupyterlab/services@npm:7.0.11"
+  dependencies:
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/settingregistry": ^4.0.11
+    "@jupyterlab/statedb": ^4.0.11
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/polling": ^2.1.2
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
     ws: ^8.11.0
-  checksum: 4a4b5328f2f50ec1d501f67d63fbfb329f37a6c090227e0aecdbbb7316d9df0e5891af47cb948958e9307a0afc52f0ddf05c2be7acb9e2f44e54cf568dc3b90c
+  checksum: 6539cc1b34f29feaab094a570576890984fe9cc3f0140dc3b17cca1ead878197bd3d2ca01b4f6fe6808ee5dca8f720769e0db10a27f1fcad1759b6ead9631b24
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/settingregistry@npm:4.0.2"
+"@jupyterlab/settingregistry@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/settingregistry@npm:4.0.11"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.2
-    "@jupyterlab/statedb": ^4.0.2
-    "@lumino/commands": ^2.1.1
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/signaling": ^2.1.1
+    "@jupyterlab/nbformat": ^4.0.11
+    "@jupyterlab/statedb": ^4.0.11
+    "@lumino/commands": ^2.1.3
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/signaling": ^2.1.2
     "@rjsf/utils": ^5.1.0
     ajv: ^8.12.0
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
-  checksum: c2e019f70a4f19cf99bc2029c136197f2a750f319e16f8605a6f8d690b6930ac32e24678b090a09f9e949e540cf6b4214d3d3597ec119bd6896db3b456ac6299
+  checksum: 97d06a08eff0589e83c40611f50e765dc8c75b33f821bee86defdb856c7747276174cc3370374159a37ae1393779cf18634fbca69072db447c053ccb872f3117
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/statedb@npm:4.0.2"
+"@jupyterlab/statedb@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/statedb@npm:4.0.11"
   dependencies:
-    "@lumino/commands": ^2.1.1
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-  checksum: 88fc80914f4c128ae6b0630ffe97111cc95a8edc4f34e749615aa8396262d74efcc82e02d0c7c2dcd0268b7cc35a0bfbd7455a4b6cb9203bcad488e1cbad5c25
+    "@lumino/commands": ^2.1.3
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+  checksum: b0637af63185b71db698ce572d2fcdaee94e6fe93659ead1e2301cb6ee1ec2b16164a61275cb44af3cac679d40b1a2c3492f20b44d9eb07a75440706627cd733
   languageName: node
   linkType: hard
 
-"@jupyterlab/statusbar@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/statusbar@npm:4.0.2"
+"@jupyterlab/statusbar@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/statusbar@npm:4.0.11"
   dependencies:
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/widgets": ^2.1.1
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: d792eb8fca00ac5ec7d5abcb3694db5c80706ec468aa4a9bef543f02a788d80ca2a9b81def0a846da14aed22dbd4ceffe0c95c0047c5025c2e5d69fc55f739b9
+  checksum: cb9d8e51533d1b0dd13f0459b3f33bab23c23dffdfb58467e58d47d0cb09f61fce320b67c50e3e5a2328fba9f7a815d4f483f460b6bea8b34cf7fcd02144fe10
   languageName: node
   linkType: hard
 
-"@jupyterlab/toc@npm:^6.0.2":
-  version: 6.0.2
-  resolution: "@jupyterlab/toc@npm:6.0.2"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.2
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/docregistry": ^4.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime": ^4.0.2
-    "@jupyterlab/translation": ^4.0.2
-    "@jupyterlab/ui-components": ^4.0.2
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/widgets": ^2.1.1
+"@jupyterlab/toc@npm:^6.0.11":
+  version: 6.0.11
+  resolution: "@jupyterlab/toc@npm:6.0.11"
+  dependencies:
+    "@jupyterlab/apputils": ^4.1.11
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/docregistry": ^4.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime": ^4.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/translation": ^4.0.11
+    "@jupyterlab/ui-components": ^4.0.11
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.0
     react: ^18.2.0
-  checksum: de36885b17d7fa067a89f84cbdeb48ecc7c90acd6b7596745c8c96b652f6853e5d744d04dab82746f94eeea65b090c32a6153191d182c2b4d969a4834c6ec8c3
+  checksum: d93d003e65b36d648407c20d19d232c0c232e9c92757b7910a170a5bfc721ec2b229a97efb553726bfa940f570b54ec3dabf8d1bae07ab84a577903d1fd039e1
   languageName: node
   linkType: hard
 
-"@jupyterlab/translation@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/translation@npm:4.0.2"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/services": ^7.0.2
-    "@jupyterlab/statedb": ^4.0.2
-    "@lumino/coreutils": ^2.1.1
-  checksum: 8f229be773607988509d059097c30bf8fbc8191d5b027221658436b2f539f6904ea48e7998276da7c52cdacd0821ea4cbdfd12ad0650ce0213525217d8735bf4
+"@jupyterlab/translation@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/translation@npm:4.0.11"
+  dependencies:
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/services": ^7.0.11
+    "@jupyterlab/statedb": ^4.0.11
+    "@lumino/coreutils": ^2.1.2
+  checksum: 1e65d0a162d56724a99dcb7eec874b80e78f8113e14d9cc1461f56cebef9a21604baf1fffd43cd62f186942b63fd49effec2b1960e4e3aca0a6cbe03df46bd51
   languageName: node
   linkType: hard
 
-"@jupyterlab/ui-components@npm:^4.0.2":
-  version: 4.0.2
-  resolution: "@jupyterlab/ui-components@npm:4.0.2"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.0.2
-    "@jupyterlab/observables": ^5.0.2
-    "@jupyterlab/rendermime-interfaces": ^3.8.2
-    "@jupyterlab/translation": ^4.0.2
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/commands": ^2.1.1
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/polling": ^2.1.1
-    "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/virtualdom": ^2.0.0
-    "@lumino/widgets": ^2.1.1
+"@jupyterlab/ui-components@npm:^4.0.11":
+  version: 4.0.11
+  resolution: "@jupyterlab/ui-components@npm:4.0.11"
+  dependencies:
+    "@jupyterlab/coreutils": ^6.0.11
+    "@jupyterlab/observables": ^5.0.11
+    "@jupyterlab/rendermime-interfaces": ^3.8.11
+    "@jupyterlab/translation": ^4.0.11
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/commands": ^2.1.3
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/messaging": ^2.0.1
+    "@lumino/polling": ^2.1.2
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/virtualdom": ^2.0.1
+    "@lumino/widgets": ^2.3.0
     "@rjsf/core": ^5.1.0
     "@rjsf/utils": ^5.1.0
     react: ^18.2.0
     react-dom: ^18.2.0
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
-  checksum: 5e941c557609e2cec3df3cb42de358c13f73f3cd0a3b0ce6c5d473dc8d7d09772d8dc35f843f9ef1b6619700fa4a403979a93aae047517efa5d9385a8f90eac7
+  checksum: 0ad2fcdcb531ffc4da4f475c24520007d65190c70bfe07888f4284256754e15ffb77d23f02a6ce44688bad0103484cba22327db49796abb13f8dfc335ea2373d
   languageName: node
   linkType: hard
 
-"@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2":
-  version: 1.0.3
-  resolution: "@lezer/common@npm:1.0.3"
-  checksum: cc90dc2f0aeaebeb3fe886cbd27f8b1e8bee817d8c2efff178604807debd68c5db820fd23afb830962780063d21891afbdf564420221faca2822e77bc6327184
+"@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2, @lezer/common@npm:^1.1.0, @lezer/common@npm:^1.2.0, @lezer/common@npm:^1.2.1":
+  version: 1.2.1
+  resolution: "@lezer/common@npm:1.2.1"
+  checksum: 0bd092e293a509ce334f4aaf9a4d4a25528f743cd9d7e7948c697e34ac703b805b288b62ad01563488fb206fc34ff05084f7fc5d864be775924b3d0d53ea5dd2
   languageName: node
   linkType: hard
 
 "@lezer/cpp@npm:^1.0.0":
-  version: 1.1.1
-  resolution: "@lezer/cpp@npm:1.1.1"
+  version: 1.1.2
+  resolution: "@lezer/cpp@npm:1.1.2"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: c9e1db19776eafbfe0c3b8448d46c94d9a1d30f7fef630292e63bab82e6d5d6903a043ee8cf341bcbf84c00ee0d79b8c255bab8fd8e0a91355ae912b53c78935
+  checksum: a319cd46fd32affc07c9432e9b2b9954becf7766be0361176c525d03474bb794cc051aad9932f48c9df33833eee1d6bfdccab12e571f2b137b4ca765c60c75de
   languageName: node
   linkType: hard
 
 "@lezer/css@npm:^1.0.0, @lezer/css@npm:^1.1.0":
-  version: 1.1.3
-  resolution: "@lezer/css@npm:1.1.3"
+  version: 1.1.7
+  resolution: "@lezer/css@npm:1.1.7"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: c8069ef0a6751441d2dc9180f7ebfd7aeb35df0ca2f1a748a2f26203a9ef6cc30f17f3074e2b49520453eb39329dadfdbbb901c6d9d067dc955ceb58c1f8cc6a
+  checksum: 7760d294fd0b1ac6db319c4990517c1ed9027d6757de537553624238056df6e1ef1b6a571a023a4bce3d7a2b891036d9f85f76f2109f503bea94837f90c64bc2
   languageName: node
   linkType: hard
 
 "@lezer/generator@npm:^1.2.2":
-  version: 1.3.0
-  resolution: "@lezer/generator@npm:1.3.0"
+  version: 1.6.0
+  resolution: "@lezer/generator@npm:1.6.0"
   dependencies:
-    "@lezer/common": ^1.0.2
+    "@lezer/common": ^1.1.0
     "@lezer/lr": ^1.3.0
   bin:
-    lezer-generator: dist/lezer-generator.cjs
-  checksum: 114df33679b44e86d0801473088bd1d52c208e3b3beb16cc923efac88280fc897bc2b79fd1a7bf2c04579a315898f4029127e5f15dc9557ff3c0ba0e710987eb
+    lezer-generator: src/lezer-generator.cjs
+  checksum: dfbf19d0533922272ac00c4b7884e1df88e2a35dd758e4544ceb5d784aa38d5751add03ca87f35d14cc39416e0dbc06ccaf2a211a6ae982e00daaaffe9c9320c
   languageName: node
   linkType: hard
 
 "@lezer/highlight@npm:^1.0.0, @lezer/highlight@npm:^1.1.3, @lezer/highlight@npm:^1.1.4":
-  version: 1.1.6
-  resolution: "@lezer/highlight@npm:1.1.6"
+  version: 1.2.0
+  resolution: "@lezer/highlight@npm:1.2.0"
   dependencies:
     "@lezer/common": ^1.0.0
-  checksum: 411a702394c4c996b7d7f145a38f3a85a8cc698b3918acc7121c629255bb76d4ab383753f69009e011dc415210c6acbbb5b27bde613259ab67e600b29397b03b
+  checksum: 5b9dfe741f95db13f6124cb9556a43011cb8041ecf490be98d44a86b04d926a66e912bcd3a766f6a3d79e064410f1a2f60ab240b50b645a12c56987bf4870086
   languageName: node
   linkType: hard
 
 "@lezer/html@npm:^1.3.0":
-  version: 1.3.5
-  resolution: "@lezer/html@npm:1.3.5"
+  version: 1.3.8
+  resolution: "@lezer/html@npm:1.3.8"
   dependencies:
-    "@lezer/common": ^1.0.0
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 19fcf262d06a89d8a1d3c6c825585f4b555dbdeaf60179fbe00164f72c0dbdf8cde8057172fd3660b13be63f0dcf1380cea9196ade7c1a9bc58a2aecd2b03125
+  checksum: 06bce804487435ea6ccb39595176bb65d68691f082b0b68fb7d22d90d4de9798a8202f16e9aefe22865db15257a37f6fca93275d660715eea98f7578579e7135
   languageName: node
   linkType: hard
 
 "@lezer/java@npm:^1.0.0":
-  version: 1.0.4
-  resolution: "@lezer/java@npm:1.0.4"
+  version: 1.1.1
+  resolution: "@lezer/java@npm:1.1.1"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 97f5a2c2d733afba5dc57a0da9a97515b19b5e63bb5937717dac4e8c9baed74d15c0cb5c1580858b678931f11d517c56d89f903968fa48931f9c62e2ea67a107
+  checksum: 8a071aca6b5e1ed1d22bffed22bbd29f21b102b7337a7ea5c956eb259e6ff20eee2d6e85b7dadff69859cb6615d6b1a3f0ba109673e87ce5a1f6cabdeee626fd
   languageName: node
   linkType: hard
 
 "@lezer/javascript@npm:^1.0.0":
-  version: 1.4.4
-  resolution: "@lezer/javascript@npm:1.4.4"
+  version: 1.4.13
+  resolution: "@lezer/javascript@npm:1.4.13"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.1.3
     "@lezer/lr": ^1.3.0
-  checksum: 29797dbb4c0632718cc5a3d0c6baeefe4240562f8b1ef1f60c58d0481c53ac4bbbac354369aa95e4131dfe0bbc4464bc025620f58f01739bd896974bb08dbad5
+  checksum: a5e4607fec7671dff66d1f3bfee5a5da7395982f1867e17ac4d8f2d8f223451fb18516ef2699340b148af112176a07e1fcba9e63c5f8397c12895dd0509113d6
   languageName: node
   linkType: hard
 
 "@lezer/json@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@lezer/json@npm:1.0.1"
+  version: 1.0.2
+  resolution: "@lezer/json@npm:1.0.2"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: fcd17178f6a58e71c83e08fdc047e3708528b28591ba8f08ed35268f370d1ec9b63af0afa9d82a77fec26e9eb477ab3cfdc31c951e080d118ef607f9f9bb52e3
+  checksum: f899d13765d95599c9199fc3404cb57969031dc40ce07de30f4e648979153966581f0bee02e2f8f70463b0a5322206a97c2fe8d5d14f218888c72a6dcedf90ef
   languageName: node
   linkType: hard
 
 "@lezer/lr@npm:^1.0.0, @lezer/lr@npm:^1.1.0, @lezer/lr@npm:^1.3.0":
-  version: 1.3.9
-  resolution: "@lezer/lr@npm:1.3.9"
+  version: 1.4.0
+  resolution: "@lezer/lr@npm:1.4.0"
   dependencies:
     "@lezer/common": ^1.0.0
-  checksum: d10982bae6c0b2f5a3ab8710a41dc689a4f9e81afafd3d2de4f0bec169f5c3fc9a321c0e90010a51682d41a6755ae90e1f3199134ff194b3ff4058ea5bcdf353
+  checksum: 4c8517017e9803415c6c5cb8230d8764107eafd7d0b847676cd1023abb863a4b268d0d01c7ce3cf1702c4749527c68f0a26b07c329cb7b68c36ed88362d7b193
   languageName: node
   linkType: hard
 
 "@lezer/markdown@npm:^1.0.0, @lezer/markdown@npm:^1.0.2":
-  version: 1.0.5
-  resolution: "@lezer/markdown@npm:1.0.5"
+  version: 1.2.0
+  resolution: "@lezer/markdown@npm:1.2.0"
   dependencies:
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
-  checksum: e862d7362faab54a4536c9913171580d0062ae5ffa9d46d6dcb4850b2b8f2fb6f2f28f98a30232640bfcd980682673ccb051230b06422814db89abea5f07d99e
+  checksum: e6355272ad98c97b339dd42d8d9b78fa4f48fdcc5c9c408720936cacb7d2bcd47b0cedf8e0997ef93539c2b03a65326fc59372e54f0b24acd98630e06869a350
   languageName: node
   linkType: hard
 
 "@lezer/php@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@lezer/php@npm:1.0.1"
+  version: 1.0.2
+  resolution: "@lezer/php@npm:1.0.2"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.1.0
-  checksum: a847c255c030b4d38913ddf1d5bd7324d83be7ef8d1d244542870be03b9bf7dc71283afeb2415c40dfd188cb99f0cc44bad760b5f3b7c35c3b8e5e00253848fc
+  checksum: c85ef18571d37826b687dd141a0fe110f5814adaf9d1a391e7e482020d7f81df189ca89ec0dd141c1433d48eff4c6e53648b46f008dea8ad2dc574f35f1d4d79
   languageName: node
   linkType: hard
 
 "@lezer/python@npm:^1.1.4":
-  version: 1.1.8
-  resolution: "@lezer/python@npm:1.1.8"
+  version: 1.1.11
+  resolution: "@lezer/python@npm:1.1.11"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: e4a4e0b0fd871acff25111d4f767944b5015479776504b85c4431859c8a2859fdfa6362f204f3027cf9858c7ea907fd57244852a18b67da9eba3b2fe38d31b03
+  checksum: ed0e58317716967644f57bf29eb902c0c205b909bc035c0960520222a79bd6525468c8adfb7d824787a8a29ec7a1c7d2da5fd59f912cdeff2830c71958b9576d
   languageName: node
   linkType: hard
 
 "@lezer/rust@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@lezer/rust@npm:1.0.1"
+  version: 1.0.2
+  resolution: "@lezer/rust@npm:1.0.2"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 1e02fdf09206979e7d4f87b020589f410c4c5e452a7b7b0296f6772ce3571c1bd7ed37495fbeeecf3d4423000f2efdabd462ba8a949c2b351fd35550327a7613
+  checksum: fc5e97852b42beeb44a0ebe316dc64e3cc49ff481c22e3e67d6003fc4a5c257fcd94959cfcc76cd154fa172db9b3b4b28de5c09f10550d6e5f14869ddc274e5b
   languageName: node
   linkType: hard
 
 "@lezer/xml@npm:^1.0.0":
-  version: 1.0.2
-  resolution: "@lezer/xml@npm:1.0.2"
+  version: 1.0.4
+  resolution: "@lezer/xml@npm:1.0.4"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: e834bcc5c0dee3eecb5362b3f10187e80908b6a293ebacf5750547a64b57ec710a068497334f109ecf4e5ea05e09e7e9c00e48ebbd30050673ea67b0929e5398
+  checksum: 68a82085bff6c1525f4ef03cd9f9dac0132b3e03fe574e0289700dd4475056e40e8744cde15cf5ad6d3760d0d584ff85ce707e26a7c938d0c5fe2e325c1c336e
   languageName: node
   linkType: hard
 
-"@lumino/algorithm@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/algorithm@npm:2.0.0"
-  checksum: 663edf536e94397b449c6a2643a735e602fbb396dec86b56ad1193a768dce27c6e7da5ad0384aa90086ea44cbb64dde3f9d565e9fd81858f1eb0c6b4253f3b94
+"@lumino/algorithm@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "@lumino/algorithm@npm:2.0.1"
+  checksum: cbf7fcf6ee6b785ea502cdfddc53d61f9d353dcb9659343511d5cd4b4030be2ff2ca4c08daec42f84417ab0318a3d9972a17319fa5231693e109ab112dcf8000
   languageName: node
   linkType: hard
 
-"@lumino/application@npm:^2.1.1":
-  version: 2.2.0
-  resolution: "@lumino/application@npm:2.2.0"
+"@lumino/application@npm:^2.2.1":
+  version: 2.3.0
+  resolution: "@lumino/application@npm:2.3.0"
   dependencies:
-    "@lumino/commands": ^2.1.2
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/widgets": ^2.2.0
-  checksum: b62da44b21d110c5d3478a49549326974b59325b8c60a58905d8e5ef08210273cd013cb60387d1f082fb79377a230278e2cf63e345491b0a54c75fdcc6164a68
+    "@lumino/commands": ^2.2.0
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/widgets": ^2.3.1
+  checksum: 9d1eb5bc972ed158bf219604a53bbac1262059bc5b0123d3e041974486b9cbb8288abeeec916f3b62f62d7c32e716cccf8b73e4832ae927e4f9dd4e4b0cd37ed
   languageName: node
   linkType: hard
 
-"@lumino/collections@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/collections@npm:2.0.0"
+"@lumino/collections@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "@lumino/collections@npm:2.0.1"
   dependencies:
-    "@lumino/algorithm": ^2.0.0
-  checksum: 4a7fc3571e92a1368a1ef01300ad7b6e0d4ff13cb78b89533d5962eea66d4a7550e15d8b80fa3ab1816b1a89382f35015f9dddf72ab04654c17e5b516b845d8f
+    "@lumino/algorithm": ^2.0.1
+  checksum: 8a29b7973a388a33c5beda0819dcd2dc2aad51a8406dcfd4581b055a9f77a39dc5800f7a8b4ae3c0bb97ae7b56a7a869e2560ffb7a920a28e93b477ba05907d6
   languageName: node
   linkType: hard
 
-"@lumino/commands@npm:^2.1.1, @lumino/commands@npm:^2.1.2":
-  version: 2.1.2
-  resolution: "@lumino/commands@npm:2.1.2"
+"@lumino/commands@npm:^2.1.3, @lumino/commands@npm:^2.2.0":
+  version: 2.2.0
+  resolution: "@lumino/commands@npm:2.2.0"
   dependencies:
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/domutils": ^2.0.0
-    "@lumino/keyboard": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/virtualdom": ^2.0.0
-  checksum: c0b5ce8c5e1a86a98a90f54bb07b74742748110cf3362b86ff8328c1b5475c4dc05f1c4c9f50bf79e51c4e2ddc5cd69d6194f3d39dd5b58f357b0f30758bf35b
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/domutils": ^2.0.1
+    "@lumino/keyboard": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/virtualdom": ^2.0.1
+  checksum: 093e9715491e5cef24bc80665d64841417b400f2fa595f9b60832a3b6340c405c94a6aa276911944a2c46d79a6229f3cc087b73f50852bba25ece805abd0fae9
   languageName: node
   linkType: hard
 
-"@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.1.1, @lumino/coreutils@npm:^2.1.1":
-  version: 2.1.1
-  resolution: "@lumino/coreutils@npm:2.1.1"
-  checksum: dfdeb2b0282caae17b6c3edfebadf4ce7c75fc879fa60cacfef9b154412f4b35e4ffd95b1833b99d8dacb99aaaa04513570129ae2024c3f33e2677a01f0576ce
+"@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.1.2, @lumino/coreutils@npm:^2.1.2":
+  version: 2.1.2
+  resolution: "@lumino/coreutils@npm:2.1.2"
+  checksum: 7865317ac0676b448d108eb57ab5d8b2a17c101995c0f7a7106662d9fe6c859570104525f83ee3cda12ae2e326803372206d6f4c1f415a5b59e4158a7b81066f
   languageName: node
   linkType: hard
 
-"@lumino/datagrid@npm:^2.1.1":
-  version: 2.1.2
-  resolution: "@lumino/datagrid@npm:2.1.2"
+"@lumino/datagrid@npm:^2.2.0":
+  version: 2.3.0
+  resolution: "@lumino/datagrid@npm:2.3.0"
   dependencies:
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/domutils": ^2.0.0
-    "@lumino/dragdrop": ^2.1.2
-    "@lumino/keyboard": ^2.0.0
-    "@lumino/messaging": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/widgets": ^2.2.0
-  checksum: b121cfff8295aa600c2ad9de0ef4c7a3b9c8bbbc202d89b853f6c64d70e13058c62f898cc52d092a3f11b6158fde55cb24b764326ef2b4333db182a4e6cd3cc5
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/domutils": ^2.0.1
+    "@lumino/dragdrop": ^2.1.4
+    "@lumino/keyboard": ^2.0.1
+    "@lumino/messaging": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.1
+  checksum: 906ecd8d02a4ccbd6d09384e181f809ef4c165ca7bbc2388b43276f28d0a7d2949093f8b1782f8e11c988640ffaaeca9fe889722a51ee424cad3314674658695
   languageName: node
   linkType: hard
 
-"@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^2.1.1":
-  version: 2.1.1
-  resolution: "@lumino/disposable@npm:2.1.1"
+"@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^2.1.2":
+  version: 2.1.2
+  resolution: "@lumino/disposable@npm:2.1.2"
   dependencies:
-    "@lumino/signaling": ^2.1.1
-  checksum: ed6cdfe13f3346178a087690d4e7baeccaed7e73ca23cb239765202409f5c01b4729a4058b4717f963462ee9ef2e5cb14ad1974e3163741267290edc3715c85c
+    "@lumino/signaling": ^2.1.2
+  checksum: ac2fb2bf18d0b2939fda454f3db248a0ff6e8a77b401e586d1caa9293b3318f808b93a117c9c3ac27cd17aab545aea83b49108d099b9b2f5503ae2a012fbc6e2
   languageName: node
   linkType: hard
 
-"@lumino/domutils@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/domutils@npm:2.0.0"
-  checksum: 4a146bfc1006d5fd00ccecc61d9803965d269c15c48c892fd87216336ce967f0db91f31203c5616c83d260224cddf25af4abb6704a6770757d19e44068f690bf
+"@lumino/domutils@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "@lumino/domutils@npm:2.0.1"
+  checksum: 61fa0ab226869dfbb763fc426790cf5a43b7d6f4cea1364c6dd56d61c44bff05eea188d33ff847449608ef58ed343161bee15c19b96f35410e4ee35815dc611a
   languageName: node
   linkType: hard
 
-"@lumino/dragdrop@npm:^2.1.1, @lumino/dragdrop@npm:^2.1.2":
-  version: 2.1.2
-  resolution: "@lumino/dragdrop@npm:2.1.2"
+"@lumino/dragdrop@npm:^2.1.4":
+  version: 2.1.4
+  resolution: "@lumino/dragdrop@npm:2.1.4"
   dependencies:
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-  checksum: 7ac64ec11423ec89fea937aa6c9ca818933ee98e775e500018a0a948f32171932033a1e302a48395cbe9bfeaa635acde2393fd935db14d7b1d569ca6a1daaa77
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+  checksum: 43d82484b13b38b612e7dfb424a840ed6a38d0db778af10655c4ba235c67b5b12db1683929b35a36ab2845f77466066dfd1ee25c1c273e8e175677eba9dc560d
   languageName: node
   linkType: hard
 
-"@lumino/keyboard@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/keyboard@npm:2.0.0"
-  checksum: 3852ba51f437b1c1d7e552a0f844592a05e04dd5012070dc6e4384c58965d1ebf536c6875c1b7bae03cde3c715ddc36cd290992fcefc1a8c39094194f4689fdd
+"@lumino/keyboard@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "@lumino/keyboard@npm:2.0.1"
+  checksum: cf33f13427a418efd7cc91061233321e860d5404f3d86397781028309bef86c8ad2d88276ffe335c1db0fe619bd9d1e60641c81f881696957a58703ee4652c3e
   languageName: node
   linkType: hard
 
-"@lumino/messaging@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/messaging@npm:2.0.0"
+"@lumino/messaging@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "@lumino/messaging@npm:2.0.1"
   dependencies:
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/collections": ^2.0.0
-  checksum: 1e82dcf9b110834d4342dc63dfeac0ee780880fb99051bd82d00a1f83afd91b276c1cea5af85a414d92c527adc365d54f20ec780123b562f89c5a2cd3e96bf81
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/collections": ^2.0.1
+  checksum: 964c4651c374b17452b4252b7d71500b32d2ecd87c192fc5bcf5d3bd1070661d78d07edcac8eca7d1d6fd50aa25992505485e1296d6dd995691b8e349b652045
   languageName: node
   linkType: hard
 
-"@lumino/polling@npm:^2.1.1":
-  version: 2.1.1
-  resolution: "@lumino/polling@npm:2.1.1"
+"@lumino/polling@npm:^2.1.2":
+  version: 2.1.2
+  resolution: "@lumino/polling@npm:2.1.2"
   dependencies:
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/signaling": ^2.1.1
-  checksum: 69177b26d5fc541e72533cbe7d7f7999eea541d392f1082d20dbd9e1797e7d46fba47bae9c65c06f9ccb2780cbae636e9354d9bf4423b5e1020754d4b07d4f6b
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/signaling": ^2.1.2
+  checksum: fa9b401e6dbeb8f31d7e3ba485e8ef1e0c92b3f2da086239c0ed49931026f5d3528709193c93e031e35ac624fb4bbbfcdcbaa0e25eb797f36e2952e5cd91e9e3
   languageName: node
   linkType: hard
 
-"@lumino/properties@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/properties@npm:2.0.0"
-  checksum: 81187a11a779eed4e20ff0035e77dee99bd271b0cf649096c4e8809dd6bdd06955b1a974bc1a115e536f8d2840b30183bb78a362b2c6991824477df6d17e6c59
+"@lumino/properties@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "@lumino/properties@npm:2.0.1"
+  checksum: c50173a935148cc4148fdaea119df1d323ee004ae16ab666800388d27e9730345629662d85f25591683329b39f0cdae60ee8c94e8943b4d0ef7d7370a38128d6
   languageName: node
   linkType: hard
 
-"@lumino/signaling@npm:^1.10.0 || ^2.0.0, @lumino/signaling@npm:^2.1.1":
-  version: 2.1.1
-  resolution: "@lumino/signaling@npm:2.1.1"
+"@lumino/signaling@npm:^1.10.0 || ^2.0.0, @lumino/signaling@npm:^2.1.2":
+  version: 2.1.2
+  resolution: "@lumino/signaling@npm:2.1.2"
   dependencies:
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-  checksum: 283ad4239b8577f68aca3d0b2606f73cc1c775f84cab25cf49aa6cd195f0d87949ef43fdff03b38b5a49ebbf2468581c6786d5f8b6159a04b2051260be5eab86
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/coreutils": ^2.1.2
+  checksum: ad7d7153db57980da899c43e412e6130316ef30b231a70250e7af49058db16cadb018c1417a2ea8083d83c48623cfe6b705fa82bf10216b1a8949aed9f4aca4e
   languageName: node
   linkType: hard
 
-"@lumino/virtualdom@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/virtualdom@npm:2.0.0"
+"@lumino/virtualdom@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "@lumino/virtualdom@npm:2.0.1"
+  dependencies:
+    "@lumino/algorithm": ^2.0.1
+  checksum: cf59b6f15b430e13e9e657b7a0619b9056cd9ea7b2a87f407391d071c501b77403c302b6a66dca510382045e75b2e3fe551630bb391f1c6b33678057d4bec164
+  languageName: node
+  linkType: hard
+
+"@lumino/widgets@npm:^1.37.2 || ^2.3.0, @lumino/widgets@npm:^2.3.0, @lumino/widgets@npm:^2.3.1":
+  version: 2.3.1
+  resolution: "@lumino/widgets@npm:2.3.1"
   dependencies:
-    "@lumino/algorithm": ^2.0.0
-  checksum: 6fc1d88e7d4a656be7664ccfc5745eb1d4e3d2034db0b11ad6abefcc642f22d265003eef0e1d02bca2e42b6da127123118c631369006f78e88a08885a6f36c25
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/commands": ^2.2.0
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/domutils": ^2.0.1
+    "@lumino/dragdrop": ^2.1.4
+    "@lumino/keyboard": ^2.0.1
+    "@lumino/messaging": ^2.0.1
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/virtualdom": ^2.0.1
+  checksum: ba7b8f8839c1cd2a41dbda13281094eb6981a270cccf4f25a0cf83686dcc526a2d8044a20204317630bb7dd4a04d65361408c7623a921549c781afca84b91c67
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^1.37.2 || ^2.1.1, @lumino/widgets@npm:^2.1.1, @lumino/widgets@npm:^2.2.0":
+"@npmcli/agent@npm:^2.0.0":
   version: 2.2.0
-  resolution: "@lumino/widgets@npm:2.2.0"
+  resolution: "@npmcli/agent@npm:2.2.0"
   dependencies:
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/commands": ^2.1.2
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/domutils": ^2.0.0
-    "@lumino/dragdrop": ^2.1.2
-    "@lumino/keyboard": ^2.0.0
-    "@lumino/messaging": ^2.0.0
-    "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/virtualdom": ^2.0.0
-  checksum: 963c0e54102b786a9cbf3467041c9f6f5c275af751afc311ebeba30d56516767c463c425e321bb389eaa66726dfc4420119a9a58573dcbf3110aba9515c80606
+    agent-base: ^7.1.0
+    http-proxy-agent: ^7.0.0
+    https-proxy-agent: ^7.0.1
+    lru-cache: ^10.0.1
+    socks-proxy-agent: ^8.0.1
+  checksum: 3b25312edbdfaa4089af28e2d423b6f19838b945e47765b0c8174c1395c79d43c3ad6d23cb364b43f59fd3acb02c93e3b493f72ddbe3dfea04c86843a7311fc4
   languageName: node
   linkType: hard
 
 "@npmcli/fs@npm:^3.1.0":
   version: 3.1.0
   resolution: "@npmcli/fs@npm:3.1.0"
   dependencies:
@@ -1275,58 +1301,53 @@
 "@pkgjs/parseargs@npm:^0.11.0":
   version: 0.11.0
   resolution: "@pkgjs/parseargs@npm:0.11.0"
   checksum: 6ad6a00fc4f2f2cfc6bff76fb1d88b8ee20bc0601e18ebb01b6d4be583733a860239a521a7fbca73b612e66705078809483549d2b18f370eb346c5155c8e4a0f
   languageName: node
   linkType: hard
 
-"@playwright/test@npm:^1.32.0, @playwright/test@npm:^1.32.2":
-  version: 1.35.1
-  resolution: "@playwright/test@npm:1.35.1"
+"@playwright/test@npm:^1.32.2, @playwright/test@npm:^1.37.0":
+  version: 1.41.1
+  resolution: "@playwright/test@npm:1.41.1"
   dependencies:
-    "@types/node": "*"
-    fsevents: 2.3.2
-    playwright-core: 1.35.1
-  dependenciesMeta:
-    fsevents:
-      optional: true
+    playwright: 1.41.1
   bin:
     playwright: cli.js
-  checksum: 3509d2f2c7397f9b0d4f49088cab8625f17d186f7e9b3389ddebf7c52ee8aae6407eab48f66b300b7bf6a33f6e3533fd5951e72bfdb001b68838af98596d5a53
+  checksum: d9877e777a1a7f60f097df57b6abc2478e2ae342930a409c8546c8aa40d6e206cbc16bf1c71b23414ac3fbad36dcae1ad79635d7f4eb705ab54d3c705e82ea04
   languageName: node
   linkType: hard
 
 "@rjsf/core@npm:^5.1.0":
-  version: 5.9.0
-  resolution: "@rjsf/core@npm:5.9.0"
+  version: 5.16.1
+  resolution: "@rjsf/core@npm:5.16.1"
   dependencies:
     lodash: ^4.17.21
     lodash-es: ^4.17.21
-    markdown-to-jsx: ^7.2.1
-    nanoid: ^3.3.6
+    markdown-to-jsx: ^7.4.0
+    nanoid: ^3.3.7
     prop-types: ^15.8.1
   peerDependencies:
-    "@rjsf/utils": ^5.8.x
+    "@rjsf/utils": ^5.16.x
     react: ^16.14.0 || >=17
-  checksum: 52406fcf560af51cb5b45ce95eb826ff1ad4ed1366c70b16b16137455f6b252cef507f76f139524228e12ccf2d49816b3538747431886476574ac2911f29aac1
+  checksum: 2f88dc6af9dda8ec5c8cbac63f3f9e776a11fe363ce938aa7b5c7a3baaa84a7a2f3796ebf55b361a8cb65267a1715ab880a4743636fb88e06b0240d07f0e4c7b
   languageName: node
   linkType: hard
 
 "@rjsf/utils@npm:^5.1.0":
-  version: 5.9.0
-  resolution: "@rjsf/utils@npm:5.9.0"
+  version: 5.16.1
+  resolution: "@rjsf/utils@npm:5.16.1"
   dependencies:
     json-schema-merge-allof: ^0.8.1
     jsonpointer: ^5.0.1
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
-  checksum: f1a1070539b24763b64631bb8d0d16a504fa46f029775a34e57c47e58b913b07e2869b45de6c993745a6320df3b6571f101abc2d07be59054a971e43facae6ea
+  checksum: 0c69527de4ab6f9d6ec4d1a5e05a31a0a38062d40abe2a2da7bc2324b20b08b0e90c188977ac4408f3b004c758c28097444746f3215e21e184c11cad7e9278c1
   languageName: node
   linkType: hard
 
 "@stdlib/array@npm:^0.0.x":
   version: 0.0.12
   resolution: "@stdlib/array@npm:0.0.12"
   dependencies:
@@ -1726,105 +1747,73 @@
     "@stdlib/types": ^0.0.x
     debug: ^2.6.9
   checksum: e0c3671c5f62c11bb3abd721f2958c41641b00a75d449bd25fbb62bcb8689cfe9c1f600c0688e7b6819ae870d6e5974d0fc7b2ec86081c45d9194b316b2a2ec2
   conditions: (os=aix | os=darwin | os=freebsd | os=linux | os=macos | os=openbsd | os=sunos | os=win32 | os=windows)
   languageName: node
   linkType: hard
 
-"@tootallnate/once@npm:2":
-  version: 2.0.0
-  resolution: "@tootallnate/once@npm:2.0.0"
-  checksum: ad87447820dd3f24825d2d947ebc03072b20a42bfc96cbafec16bff8bbda6c1a81fcb0be56d5b21968560c5359a0af4038a68ba150c3e1694fe4c109a063bed8
-  languageName: node
-  linkType: hard
-
-"@types/clone@npm:~2.1.1":
-  version: 2.1.1
-  resolution: "@types/clone@npm:2.1.1"
-  checksum: bda9668b9d6e0875d64bbe00763676f566e8647bc224333a03ac7fd66655dfed56a98a9f8304d0145c4411b964649c84c4d1a03adbdb6547eafb9ab8f303d254
-  languageName: node
-  linkType: hard
-
 "@types/estree@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@types/estree@npm:1.0.1"
-  checksum: e9aa175eacb797216fafce4d41e8202c7a75555bc55232dee0f9903d7171f8f19f0ae7d5191bb1a88cb90e65468be508c0df850a9fb81b4433b293a5a749899d
+  version: 1.0.5
+  resolution: "@types/estree@npm:1.0.5"
+  checksum: dd8b5bed28e6213b7acd0fb665a84e693554d850b0df423ac8076cc3ad5823a6bc26b0251d080bdc545af83179ede51dd3f6fa78cad2c46ed1f29624ddf3e41a
   languageName: node
   linkType: hard
 
 "@types/geojson@npm:7946.0.4":
   version: 7946.0.4
   resolution: "@types/geojson@npm:7946.0.4"
   checksum: 541aea46540c918b9fe21ab73f497fe17b1eaf4d0d3baeb5f5614029b7f488c37f63843b644c024a8178dc2fb66d3d6623c25d9cf61d7b553aa19c8dc7f99047
   languageName: node
   linkType: hard
 
-"@types/node@npm:*":
-  version: 20.4.1
-  resolution: "@types/node@npm:20.4.1"
-  checksum: 22cbcc792f2eb636fe4188778ed0f32658ab872aa7fcb9847b3fa289a42b14b9f5e30c6faec50ef3c7adbc6c2a246926e5858136bb8b10c035a3fcaa6afbeed2
-  languageName: node
-  linkType: hard
-
 "@types/prop-types@npm:*":
-  version: 15.7.5
-  resolution: "@types/prop-types@npm:15.7.5"
-  checksum: 5b43b8b15415e1f298243165f1d44390403bb2bd42e662bca3b5b5633fdd39c938e91b7fce3a9483699db0f7a715d08cef220c121f723a634972fdf596aec980
+  version: 15.7.11
+  resolution: "@types/prop-types@npm:15.7.11"
+  checksum: 7519ff11d06fbf6b275029fe03fff9ec377b4cb6e864cac34d87d7146c7f5a7560fd164bdc1d2dbe00b60c43713631251af1fd3d34d46c69cd354602bc0c7c54
   languageName: node
   linkType: hard
 
 "@types/react@npm:^18.0.26":
-  version: 18.2.14
-  resolution: "@types/react@npm:18.2.14"
+  version: 18.2.48
+  resolution: "@types/react@npm:18.2.48"
   dependencies:
     "@types/prop-types": "*"
     "@types/scheduler": "*"
     csstype: ^3.0.2
-  checksum: a6a5e8cc78f486b9020d1ad009aa6c56943c68c7c6376e0f8399e9cbcd950b7b8f5d73f00200f5379f5e58d31d57d8aed24357f301d8e86108cd438ce6c8b3dd
+  checksum: c9ca43ed2995389b7e09492c24e6f911a8439bb8276dd17cc66a2fbebbf0b42daf7b2ad177043256533607c2ca644d7d928fdfce37a67af1f8646d2bac988900
   languageName: node
   linkType: hard
 
 "@types/scheduler@npm:*":
-  version: 0.16.3
-  resolution: "@types/scheduler@npm:0.16.3"
-  checksum: 2b0aec39c24268e3ce938c5db2f2e77f5c3dd280e05c262d9c2fe7d890929e4632a6b8e94334017b66b45e4f92a5aa42ba3356640c2a1175fa37bef2f5200767
+  version: 0.16.8
+  resolution: "@types/scheduler@npm:0.16.8"
+  checksum: 6c091b096daa490093bf30dd7947cd28e5b2cd612ec93448432b33f724b162587fed9309a0acc104d97b69b1d49a0f3fc755a62282054d62975d53d7fd13472d
   languageName: node
   linkType: hard
 
 "@vscode/debugprotocol@npm:^1.51.0":
-  version: 1.61.0
-  resolution: "@vscode/debugprotocol@npm:1.61.0"
-  checksum: 14d4f6d2f385e15a39ba7aa506c25d3e2a2d6a22ebb6ee9d354062634f292b1ce3b0d9b5ac1c098052e3f6e572a1571bf0db647d13d85157b9a50645a0f1c69f
-  languageName: node
-  linkType: hard
-
-"abbrev@npm:^1.0.0":
-  version: 1.1.1
-  resolution: "abbrev@npm:1.1.1"
-  checksum: a4a97ec07d7ea112c517036882b2ac22f3109b7b19077dc656316d07d308438aac28e4d9746dc4d84bf6b1e75b4a7b0a5f3cb30592419f128ca9a8cee3bcfa17
+  version: 1.64.0
+  resolution: "@vscode/debugprotocol@npm:1.64.0"
+  checksum: 1c8a3d6dba035674a9b4ec1b2f5e98d75170fe86cd98cf3d05cdced40d0ee0c3371f3d291516a1903f70cc5a9beadb70048d1ffc71a778bca6767bbeecb716ab
   languageName: node
   linkType: hard
 
-"agent-base@npm:6, agent-base@npm:^6.0.2":
-  version: 6.0.2
-  resolution: "agent-base@npm:6.0.2"
-  dependencies:
-    debug: 4
-  checksum: f52b6872cc96fd5f622071b71ef200e01c7c4c454ee68bc9accca90c98cfb39f2810e3e9aa330435835eedc8c23f4f8a15267f67c6e245d2b33757575bdac49d
+"abbrev@npm:^2.0.0":
+  version: 2.0.0
+  resolution: "abbrev@npm:2.0.0"
+  checksum: 0e994ad2aa6575f94670d8a2149afe94465de9cedaaaac364e7fb43a40c3691c980ff74899f682f4ca58fa96b4cbd7421a015d3a6defe43a442117d7821a2f36
   languageName: node
   linkType: hard
 
-"agentkeepalive@npm:^4.2.1":
-  version: 4.3.0
-  resolution: "agentkeepalive@npm:4.3.0"
+"agent-base@npm:^7.0.2, agent-base@npm:^7.1.0":
+  version: 7.1.0
+  resolution: "agent-base@npm:7.1.0"
   dependencies:
-    debug: ^4.1.0
-    depd: ^2.0.0
-    humanize-ms: ^1.2.1
-  checksum: 982453aa44c11a06826c836025e5162c846e1200adb56f2d075400da7d32d87021b3b0a58768d949d824811f5654223d5a8a3dad120921a2439625eb847c6260
+    debug: ^4.3.4
+  checksum: f7828f991470a0cc22cb579c86a18cbae83d8a3cbed39992ab34fc7217c4d126017f1c74d0ab66be87f71455318a8ea3e757d6a37881b8d0f2a2c6aa55e5418f
   languageName: node
   linkType: hard
 
 "aggregate-error@npm:^3.0.0":
   version: 3.1.0
   resolution: "aggregate-error@npm:3.1.0"
   dependencies:
@@ -1872,74 +1861,47 @@
 "ansi-styles@npm:^6.1.0":
   version: 6.2.1
   resolution: "ansi-styles@npm:6.2.1"
   checksum: ef940f2f0ced1a6347398da88a91da7930c33ecac3c77b72c5905f8b8fe402c52e6fde304ff5347f616e27a742da3f1dc76de98f6866c69251ad0b07a66776d9
   languageName: node
   linkType: hard
 
-"aproba@npm:^1.0.3 || ^2.0.0":
-  version: 2.0.0
-  resolution: "aproba@npm:2.0.0"
-  checksum: 5615cadcfb45289eea63f8afd064ab656006361020e1735112e346593856f87435e02d8dcc7ff0d11928bc7d425f27bc7c2a84f6c0b35ab0ff659c814c138a24
-  languageName: node
-  linkType: hard
-
-"are-we-there-yet@npm:^3.0.0":
-  version: 3.0.1
-  resolution: "are-we-there-yet@npm:3.0.1"
-  dependencies:
-    delegates: ^1.0.0
-    readable-stream: ^3.6.0
-  checksum: 52590c24860fa7173bedeb69a4c05fb573473e860197f618b9a28432ee4379049336727ae3a1f9c4cb083114601c1140cee578376164d0e651217a9843f9fe83
-  languageName: node
-  linkType: hard
-
 "balanced-match@npm:^1.0.0":
   version: 1.0.2
   resolution: "balanced-match@npm:1.0.2"
   checksum: 9706c088a283058a8a99e0bf91b0a2f75497f185980d9ffa8b304de1d9e58ebda7c72c07ebf01dadedaac5b2907b2c6f566f660d62bd336c3468e960403b9d65
   languageName: node
   linkType: hard
 
-"brace-expansion@npm:^1.1.7":
-  version: 1.1.11
-  resolution: "brace-expansion@npm:1.1.11"
-  dependencies:
-    balanced-match: ^1.0.0
-    concat-map: 0.0.1
-  checksum: faf34a7bb0c3fcf4b59c7808bc5d2a96a40988addf2e7e09dfbb67a2251800e0d14cd2bfc1aa79174f2f5095c54ff27f46fb1289fe2d77dac755b5eb3434cc07
-  languageName: node
-  linkType: hard
-
 "brace-expansion@npm:^2.0.1":
   version: 2.0.1
   resolution: "brace-expansion@npm:2.0.1"
   dependencies:
     balanced-match: ^1.0.0
   checksum: a61e7cd2e8a8505e9f0036b3b6108ba5e926b4b55089eeb5550cd04a471fe216c96d4fe7e4c7f995c728c554ae20ddfc4244cad10aef255e72b62930afd233d1
   languageName: node
   linkType: hard
 
-"cacache@npm:^17.0.0":
-  version: 17.1.3
-  resolution: "cacache@npm:17.1.3"
+"cacache@npm:^18.0.0":
+  version: 18.0.2
+  resolution: "cacache@npm:18.0.2"
   dependencies:
     "@npmcli/fs": ^3.1.0
     fs-minipass: ^3.0.0
     glob: ^10.2.2
-    lru-cache: ^7.7.1
-    minipass: ^5.0.0
-    minipass-collect: ^1.0.2
+    lru-cache: ^10.0.1
+    minipass: ^7.0.3
+    minipass-collect: ^2.0.1
     minipass-flush: ^1.0.5
     minipass-pipeline: ^1.2.4
     p-map: ^4.0.0
     ssri: ^10.0.0
     tar: ^6.1.11
     unique-filename: ^3.0.0
-  checksum: 385756781e1e21af089160d89d7462b7ed9883c978e848c7075b90b73cb823680e66092d61513050164588387d2ca87dd6d910e28d64bc13a9ac82cd8580c796
+  checksum: 0250df80e1ad0c828c956744850c5f742c24244e9deb5b7dc81bca90f8c10e011e132ecc58b64497cc1cad9a98968676147fb6575f4f94722f7619757b17a11b
   languageName: node
   linkType: hard
 
 "chownr@npm:^2.0.0":
   version: 2.0.0
   resolution: "chownr@npm:2.0.0"
   checksum: c57cf9dd0791e2f18a5ee9c1a299ae6e801ff58fee96dc8bfd0dcb4738a6ce58dd252a3605b1c93c6418fe4f9d5093b28ffbf4d66648cb2a9c67eaef9679be2f
@@ -1960,21 +1922,14 @@
     string-width: ^4.2.0
     strip-ansi: ^6.0.1
     wrap-ansi: ^7.0.0
   checksum: 79648b3b0045f2e285b76fb2e24e207c6db44323581e421c3acbd0e86454cba1b37aea976ab50195a49e7384b871e6dfb2247ad7dec53c02454ac6497394cb56
   languageName: node
   linkType: hard
 
-"clone@npm:~2.1.2":
-  version: 2.1.2
-  resolution: "clone@npm:2.1.2"
-  checksum: aaf106e9bc025b21333e2f4c12da539b568db4925c0501a1bf4070836c9e848c892fa22c35548ce0d1132b08bbbfa17a00144fe58fccdab6fa900fec4250f67d
-  languageName: node
-  linkType: hard
-
 "color-convert@npm:^2.0.1":
   version: 2.0.1
   resolution: "color-convert@npm:2.0.1"
   dependencies:
     color-name: ~1.1.4
   checksum: 79e6bdb9fd479a205c71d89574fccfb22bd9053bd98c6c4d870d65c132e5e904e6034978e55b43d69fcaa7433af2016ee203ce76eeba9cfa554b373e7f7db336
   languageName: node
@@ -1983,23 +1938,14 @@
 "color-name@npm:~1.1.4":
   version: 1.1.4
   resolution: "color-name@npm:1.1.4"
   checksum: b0445859521eb4021cd0fb0cc1a75cecf67fceecae89b63f62b201cca8d345baf8b952c966862a9d9a2632987d4f6581f0ec8d957dfacece86f0a7919316f610
   languageName: node
   linkType: hard
 
-"color-support@npm:^1.1.3":
-  version: 1.1.3
-  resolution: "color-support@npm:1.1.3"
-  bin:
-    color-support: bin.js
-  checksum: 9b7356817670b9a13a26ca5af1c21615463b500783b739b7634a0c2047c16cef4b2865d7576875c31c3cddf9dd621fa19285e628f20198b233a5cfdda6d0793b
-  languageName: node
-  linkType: hard
-
 "commander@npm:2":
   version: 2.20.3
   resolution: "commander@npm:2.20.3"
   checksum: ab8c07884e42c3a8dbc5dd9592c606176c7eb5c1ca5ff274bcf907039b2c41de3626f684ea75ccf4d361ba004bbaff1f577d5384c155f3871e456bdf27becf9e
   languageName: node
   linkType: hard
 
@@ -2029,28 +1975,14 @@
     validate.io-array: ^1.0.3
     validate.io-function: ^1.0.2
     validate.io-integer-array: ^1.0.0
   checksum: d499ab57dcb48e8d0fd233b99844a06d1cc56115602c920c586e998ebba60293731f5b6976e8a1e83ae6cbfe86716f62d9432e8d94913fed8bd8352f447dc917
   languageName: node
   linkType: hard
 
-"concat-map@npm:0.0.1":
-  version: 0.0.1
-  resolution: "concat-map@npm:0.0.1"
-  checksum: 902a9f5d8967a3e2faf138d5cb784b9979bad2e6db5357c5b21c568df4ebe62bcb15108af1b2253744844eb964fc023fbd9afbbbb6ddd0bcc204c6fb5b7bf3af
-  languageName: node
-  linkType: hard
-
-"console-control-strings@npm:^1.1.0":
-  version: 1.1.0
-  resolution: "console-control-strings@npm:1.1.0"
-  checksum: 8755d76787f94e6cf79ce4666f0c5519906d7f5b02d4b884cf41e11dcd759ed69c57da0670afd9236d229a46e0f9cf519db0cd829c6dca820bb5a5c3def584ed
-  languageName: node
-  linkType: hard
-
 "core-util-is@npm:~1.0.0":
   version: 1.0.3
   resolution: "core-util-is@npm:1.0.3"
   checksum: 9de8597363a8e9b9952491ebe18167e3b36e7707569eed0ebf14f8bba773611376466ae34575bca8cfe3c767890c859c74056084738f09d4e4a6f902b2ad7d99
   languageName: node
   linkType: hard
 
@@ -2076,38 +2008,29 @@
   version: 3.0.10
   resolution: "csstype@npm:3.0.10"
   checksum: 20a8fa324f2b33ddf94aa7507d1b6ab3daa6f3cc308888dc50126585d7952f2471de69b2dbe0635d1fdc31223fef8e070842691877e725caf456e2378685a631
   languageName: node
   linkType: hard
 
 "csstype@npm:^3.0.2":
-  version: 3.1.2
-  resolution: "csstype@npm:3.1.2"
-  checksum: e1a52e6c25c1314d6beef5168da704ab29c5186b877c07d822bd0806717d9a265e8493a2e35ca7e68d0f5d472d43fac1cdce70fd79fd0853dff81f3028d857b5
+  version: 3.1.3
+  resolution: "csstype@npm:3.1.3"
+  checksum: 8db785cc92d259102725b3c694ec0c823f5619a84741b5c7991b8ad135dfaa66093038a1cc63e03361a6cd28d122be48f2106ae72334e067dd619a51f49eddf7
   languageName: node
   linkType: hard
 
-"d3-array@npm:1 - 3, d3-array@npm:2 - 3, d3-array@npm:2.10.0 - 3, d3-array@npm:2.5.0 - 3, d3-array@npm:^3.2.2":
+"d3-array@npm:1 - 3, d3-array@npm:2 - 3, d3-array@npm:2.10.0 - 3, d3-array@npm:2.5.0 - 3, d3-array@npm:3.2.4, d3-array@npm:^3.2.2":
   version: 3.2.4
   resolution: "d3-array@npm:3.2.4"
   dependencies:
     internmap: 1 - 2
   checksum: a5976a6d6205f69208478bb44920dd7ce3e788c9dceb86b304dbe401a4bfb42ecc8b04c20facde486e9adcb488b5d1800d49393a3f81a23902b68158e12cddd0
   languageName: node
   linkType: hard
 
-"d3-array@npm:3.2.2":
-  version: 3.2.2
-  resolution: "d3-array@npm:3.2.2"
-  dependencies:
-    internmap: 1 - 2
-  checksum: 98af3db792685ceca5d9c3721efba0c567520da5532b2c7a590fd83627a598ea225d11c2cecbad404dc154120feb5ea6df0ded38f82ddf342c714cfd0c6143d1
-  languageName: node
-  linkType: hard
-
 "d3-color@npm:1 - 3, d3-color@npm:^3.1.0":
   version: 3.1.0
   resolution: "d3-color@npm:3.1.0"
   checksum: 4931fbfda5d7c4b5cfa283a13c91a954f86e3b69d75ce588d06cde6c3628cebfc3af2069ccf225e982e8987c612aa7948b3932163ce15eb3c11cd7c003f3ee3b
   languageName: node
   linkType: hard
 
@@ -2265,15 +2188,15 @@
 "d3-timer@npm:1 - 3, d3-timer@npm:^3.0.1":
   version: 3.0.1
   resolution: "d3-timer@npm:3.0.1"
   checksum: 1cfddf86d7bca22f73f2c427f52dfa35c49f50d64e187eb788dcad6e927625c636aa18ae4edd44d084eb9d1f81d8ca4ec305dae7f733c15846a824575b789d73
   languageName: node
   linkType: hard
 
-"debug@npm:4, debug@npm:^4.1.0, debug@npm:^4.3.3":
+"debug@npm:4, debug@npm:^4.3.4":
   version: 4.3.4
   resolution: "debug@npm:4.3.4"
   dependencies:
     ms: 2.1.2
   peerDependenciesMeta:
     supports-color:
       optional: true
@@ -2294,33 +2217,19 @@
   version: 4.3.1
   resolution: "deepmerge@npm:4.3.1"
   checksum: 2024c6a980a1b7128084170c4cf56b0fd58a63f2da1660dcfe977415f27b17dbe5888668b59d0b063753f3220719d5e400b7f113609489c90160bb9a5518d052
   languageName: node
   linkType: hard
 
 "delaunator@npm:5":
-  version: 5.0.0
-  resolution: "delaunator@npm:5.0.0"
+  version: 5.0.1
+  resolution: "delaunator@npm:5.0.1"
   dependencies:
-    robust-predicates: ^3.0.0
-  checksum: d6764188442b7f7c6bcacebd96edc00e35f542a96f1af3ef600e586bfb9849a3682c489c0ab423440c90bc4c7cac77f28761babff76fa29e193e1cf50a95b860
-  languageName: node
-  linkType: hard
-
-"delegates@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "delegates@npm:1.0.0"
-  checksum: a51744d9b53c164ba9c0492471a1a2ffa0b6727451bdc89e31627fdf4adda9d51277cfcbfb20f0a6f08ccb3c436f341df3e92631a3440226d93a8971724771fd
-  languageName: node
-  linkType: hard
-
-"depd@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "depd@npm:2.0.0"
-  checksum: abbe19c768c97ee2eed6282d8ce3031126662252c58d711f646921c9623f9052e3e1906443066beec1095832f534e57c523b7333f8e7e0d93051ab6baef5ab3a
+    robust-predicates: ^3.0.2
+  checksum: 69ee43ec649b4a13b7f33c8a027fb3e8dfcb09266af324286118da757e04d3d39df619b905dca41421405c311317ccf632ecfa93db44519bacec3303c57c5a0b
   languageName: node
   linkType: hard
 
 "dom-serializer@npm:^1.0.1":
   version: 1.4.1
   resolution: "dom-serializer@npm:1.4.1"
   dependencies:
@@ -2426,28 +2335,21 @@
 "exponential-backoff@npm:^3.1.1":
   version: 3.1.1
   resolution: "exponential-backoff@npm:3.1.1"
   checksum: 3d21519a4f8207c99f7457287291316306255a328770d320b401114ec8481986e4e467e854cb9914dd965e0a1ca810a23ccb559c642c88f4c7f55c55778a9b48
   languageName: node
   linkType: hard
 
-"fast-deep-equal@npm:^3.1.1, fast-deep-equal@npm:~3.1.3":
+"fast-deep-equal@npm:^3.1.1":
   version: 3.1.3
   resolution: "fast-deep-equal@npm:3.1.3"
   checksum: e21a9d8d84f53493b6aa15efc9cfd53dd5b714a1f23f67fb5dc8f574af80df889b3bce25dc081887c6d25457cce704e636395333abad896ccdec03abaf1f3f9d
   languageName: node
   linkType: hard
 
-"fast-json-stable-stringify@npm:~2.1.0":
-  version: 2.1.0
-  resolution: "fast-json-stable-stringify@npm:2.1.0"
-  checksum: b191531e36c607977e5b1c47811158733c34ccb3bfde92c44798929e9b4154884378536d26ad90dfecd32e1ffc09c545d23535ad91b3161a27ddbb8ebe0cbecb
-  languageName: node
-  linkType: hard
-
 "foreground-child@npm:^3.1.0":
   version: 3.1.1
   resolution: "foreground-child@npm:3.1.1"
   dependencies:
     cross-spawn: ^7.0.0
     signal-exit: ^4.0.1
   checksum: 139d270bc82dc9e6f8bc045fe2aae4001dc2472157044fdfad376d0a3457f77857fa883c1c8b21b491c6caade9a926a4bed3d3d2e8d3c9202b151a4cbbd0bcd5
@@ -2478,26 +2380,19 @@
   dependencies:
     minipass: ^3.0.0
   checksum: 1b8d128dae2ac6cc94230cc5ead341ba3e0efaef82dab46a33d171c044caaa6ca001364178d42069b2809c35a1c3c35079a32107c770e9ffab3901b59af8c8b1
   languageName: node
   linkType: hard
 
 "fs-minipass@npm:^3.0.0":
-  version: 3.0.2
-  resolution: "fs-minipass@npm:3.0.2"
+  version: 3.0.3
+  resolution: "fs-minipass@npm:3.0.3"
   dependencies:
-    minipass: ^5.0.0
-  checksum: e9cc0e1f2d01c6f6f62f567aee59530aba65c6c7b2ae88c5027bc34c711ebcfcfaefd0caf254afa6adfe7d1fba16bc2537508a6235196bac7276747d078aef0a
-  languageName: node
-  linkType: hard
-
-"fs.realpath@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "fs.realpath@npm:1.0.0"
-  checksum: 99ddea01a7e75aa276c250a04eedeffe5662bce66c65c07164ad6264f9de18fb21be9433ead460e54cff20e31721c811f4fb5d70591799df5f85dce6d6746fd0
+    minipass: ^7.0.3
+  checksum: 8722a41109130851d979222d3ec88aabaceeaaf8f57b2a8f744ef8bd2d1ce95453b04a61daa0078822bc5cd21e008814f06fe6586f56fef511e71b8d2394d802
   languageName: node
   linkType: hard
 
 "fsevents@npm:2.3.2":
   version: 2.3.2
   resolution: "fsevents@npm:2.3.2"
   dependencies:
@@ -2512,80 +2407,43 @@
   resolution: "fsevents@patch:fsevents@npm%3A2.3.2#~builtin<compat/fsevents>::version=2.3.2&hash=df0bf1"
   dependencies:
     node-gyp: latest
   conditions: os=darwin
   languageName: node
   linkType: hard
 
-"gauge@npm:^4.0.3":
-  version: 4.0.4
-  resolution: "gauge@npm:4.0.4"
-  dependencies:
-    aproba: ^1.0.3 || ^2.0.0
-    color-support: ^1.1.3
-    console-control-strings: ^1.1.0
-    has-unicode: ^2.0.1
-    signal-exit: ^3.0.7
-    string-width: ^4.2.3
-    strip-ansi: ^6.0.1
-    wide-align: ^1.1.5
-  checksum: 788b6bfe52f1dd8e263cda800c26ac0ca2ff6de0b6eee2fe0d9e3abf15e149b651bd27bf5226be10e6e3edb5c4e5d5985a5a1a98137e7a892f75eff76467ad2d
-  languageName: node
-  linkType: hard
-
 "get-caller-file@npm:^2.0.5":
   version: 2.0.5
   resolution: "get-caller-file@npm:2.0.5"
   checksum: b9769a836d2a98c3ee734a88ba712e62703f1df31b94b784762c433c27a386dd6029ff55c2a920c392e33657d80191edbf18c61487e198844844516f843496b9
   languageName: node
   linkType: hard
 
-"glob@npm:^10.2.2":
-  version: 10.3.3
-  resolution: "glob@npm:10.3.3"
+"glob@npm:^10.2.2, glob@npm:^10.3.10":
+  version: 10.3.10
+  resolution: "glob@npm:10.3.10"
   dependencies:
     foreground-child: ^3.1.0
-    jackspeak: ^2.0.3
+    jackspeak: ^2.3.5
     minimatch: ^9.0.1
     minipass: ^5.0.0 || ^6.0.2 || ^7.0.0
     path-scurry: ^1.10.1
   bin:
-    glob: dist/cjs/src/bin.js
-  checksum: 29190d3291f422da0cb40b77a72fc8d2c51a36524e99b8bf412548b7676a6627489528b57250429612b6eec2e6fe7826d328451d3e694a9d15e575389308ec53
-  languageName: node
-  linkType: hard
-
-"glob@npm:^7.1.3, glob@npm:^7.1.4":
-  version: 7.2.3
-  resolution: "glob@npm:7.2.3"
-  dependencies:
-    fs.realpath: ^1.0.0
-    inflight: ^1.0.4
-    inherits: 2
-    minimatch: ^3.1.1
-    once: ^1.3.0
-    path-is-absolute: ^1.0.0
-  checksum: 29452e97b38fa704dabb1d1045350fb2467cf0277e155aa9ff7077e90ad81d1ea9d53d3ee63bd37c05b09a065e90f16aec4a65f5b8de401d1dac40bc5605d133
+    glob: dist/esm/bin.mjs
+  checksum: 4f2fe2511e157b5a3f525a54092169a5f92405f24d2aed3142f4411df328baca13059f4182f1db1bf933e2c69c0bd89e57ae87edd8950cba8c7ccbe84f721cf3
   languageName: node
   linkType: hard
 
 "graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.6":
   version: 4.2.11
   resolution: "graceful-fs@npm:4.2.11"
   checksum: ac85f94da92d8eb6b7f5a8b20ce65e43d66761c55ce85ac96df6865308390da45a8d3f0296dd3a663de65d30ba497bd46c696cc1e248c72b13d6d567138a4fc7
   languageName: node
   linkType: hard
 
-"has-unicode@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "has-unicode@npm:2.0.1"
-  checksum: 1eab07a7436512db0be40a710b29b5dc21fa04880b7f63c9980b706683127e3c1b57cb80ea96d47991bdae2dfe479604f6a1ba410106ee1046a41d1bd0814400
-  languageName: node
-  linkType: hard
-
 "htmlparser2@npm:^6.0.0":
   version: 6.1.0
   resolution: "htmlparser2@npm:6.1.0"
   dependencies:
     domelementtype: ^2.0.1
     domhandler: ^4.0.0
     domutils: ^2.5.2
@@ -2597,41 +2455,31 @@
 "http-cache-semantics@npm:^4.1.1":
   version: 4.1.1
   resolution: "http-cache-semantics@npm:4.1.1"
   checksum: 83ac0bc60b17a3a36f9953e7be55e5c8f41acc61b22583060e8dedc9dd5e3607c823a88d0926f9150e571f90946835c7fe150732801010845c72cd8bbff1a236
   languageName: node
   linkType: hard
 
-"http-proxy-agent@npm:^5.0.0":
-  version: 5.0.0
-  resolution: "http-proxy-agent@npm:5.0.0"
+"http-proxy-agent@npm:^7.0.0":
+  version: 7.0.0
+  resolution: "http-proxy-agent@npm:7.0.0"
   dependencies:
-    "@tootallnate/once": 2
-    agent-base: 6
-    debug: 4
-  checksum: e2ee1ff1656a131953839b2a19cd1f3a52d97c25ba87bd2559af6ae87114abf60971e498021f9b73f9fd78aea8876d1fb0d4656aac8a03c6caa9fc175f22b786
+    agent-base: ^7.1.0
+    debug: ^4.3.4
+  checksum: 48d4fac997917e15f45094852b63b62a46d0c8a4f0b9c6c23ca26d27b8df8d178bed88389e604745e748bd9a01f5023e25093722777f0593c3f052009ff438b6
   languageName: node
   linkType: hard
 
-"https-proxy-agent@npm:^5.0.0":
-  version: 5.0.1
-  resolution: "https-proxy-agent@npm:5.0.1"
+"https-proxy-agent@npm:^7.0.1":
+  version: 7.0.2
+  resolution: "https-proxy-agent@npm:7.0.2"
   dependencies:
-    agent-base: 6
+    agent-base: ^7.0.2
     debug: 4
-  checksum: 571fccdf38184f05943e12d37d6ce38197becdd69e58d03f43637f7fa1269cf303a7d228aa27e5b27bbd3af8f09fd938e1c91dcfefff2df7ba77c20ed8dfc765
-  languageName: node
-  linkType: hard
-
-"humanize-ms@npm:^1.2.1":
-  version: 1.2.1
-  resolution: "humanize-ms@npm:1.2.1"
-  dependencies:
-    ms: ^2.0.0
-  checksum: 9c7a74a2827f9294c009266c82031030eae811ca87b0da3dceb8d6071b9bde22c9f3daef0469c3c533cc67a97d8a167cd9fc0389350e5f415f61a79b171ded16
+  checksum: 088969a0dd476ea7a0ed0a2cf1283013682b08f874c3bc6696c83fa061d2c157d29ef0ad3eb70a2046010bb7665573b2388d10fdcb3e410a66995e5248444292
   languageName: node
   linkType: hard
 
 "iconv-lite@npm:0.6, iconv-lite@npm:^0.6.2":
   version: 0.6.3
   resolution: "iconv-lite@npm:0.6.3"
   dependencies:
@@ -2650,38 +2498,28 @@
 "indent-string@npm:^4.0.0":
   version: 4.0.0
   resolution: "indent-string@npm:4.0.0"
   checksum: 824cfb9929d031dabf059bebfe08cf3137365e112019086ed3dcff6a0a7b698cb80cf67ccccde0e25b9e2d7527aa6cc1fed1ac490c752162496caba3e6699612
   languageName: node
   linkType: hard
 
-"inflight@npm:^1.0.4":
-  version: 1.0.6
-  resolution: "inflight@npm:1.0.6"
-  dependencies:
-    once: ^1.3.0
-    wrappy: 1
-  checksum: f4f76aa072ce19fae87ce1ef7d221e709afb59d445e05d47fba710e85470923a75de35bfae47da6de1b18afc3ce83d70facf44cfb0aff89f0a3f45c0a0244dfd
+"inherits@npm:2.0.3":
+  version: 2.0.3
+  resolution: "inherits@npm:2.0.3"
+  checksum: 78cb8d7d850d20a5e9a7f3620db31483aa00ad5f722ce03a55b110e5a723539b3716a3b463e2b96ce3fe286f33afc7c131fa2f91407528ba80cea98a7545d4c0
   languageName: node
   linkType: hard
 
-"inherits@npm:2, inherits@npm:^2.0.3, inherits@npm:~2.0.3":
+"inherits@npm:~2.0.3":
   version: 2.0.4
   resolution: "inherits@npm:2.0.4"
   checksum: 4a48a733847879d6cf6691860a6b1e3f0f4754176e4d71494c41f3475553768b10f84b5ce1d40fbd0e34e6bfbb864ee35858ad4dd2cf31e02fc4a154b724d7f1
   languageName: node
   linkType: hard
 
-"inherits@npm:2.0.3":
-  version: 2.0.3
-  resolution: "inherits@npm:2.0.3"
-  checksum: 78cb8d7d850d20a5e9a7f3620db31483aa00ad5f722ce03a55b110e5a723539b3716a3b463e2b96ce3fe286f33afc7c131fa2f91407528ba80cea98a7545d4c0
-  languageName: node
-  linkType: hard
-
 "internmap@npm:1 - 2":
   version: 2.0.3
   resolution: "internmap@npm:2.0.3"
   checksum: 7ca41ec6aba8f0072fc32fa8a023450a9f44503e2d8e403583c55714b25efd6390c38a87161ec456bf42d7bc83aab62eb28f5aef34876b1ac4e60693d5e1d241
   languageName: node
   linkType: hard
 
@@ -2723,31 +2561,38 @@
 "isexe@npm:^2.0.0":
   version: 2.0.0
   resolution: "isexe@npm:2.0.0"
   checksum: 26bf6c5480dda5161c820c5b5c751ae1e766c587b1f951ea3fcfc973bafb7831ae5b54a31a69bd670220e42e99ec154475025a468eae58ea262f813fdc8d1c62
   languageName: node
   linkType: hard
 
+"isexe@npm:^3.1.1":
+  version: 3.1.1
+  resolution: "isexe@npm:3.1.1"
+  checksum: 7fe1931ee4e88eb5aa524cd3ceb8c882537bc3a81b02e438b240e47012eef49c86904d0f0e593ea7c3a9996d18d0f1f3be8d3eaa92333977b0c3a9d353d5563e
+  languageName: node
+  linkType: hard
+
 "isomorphic.js@npm:^0.2.4":
   version: 0.2.5
   resolution: "isomorphic.js@npm:0.2.5"
   checksum: d8d1b083f05f3c337a06628b982ac3ce6db953bbef14a9de8ad49131250c3592f864b73c12030fdc9ef138ce97b76ef55c7d96a849561ac215b1b4b9d301c8e9
   languageName: node
   linkType: hard
 
-"jackspeak@npm:^2.0.3":
-  version: 2.2.1
-  resolution: "jackspeak@npm:2.2.1"
+"jackspeak@npm:^2.3.5":
+  version: 2.3.6
+  resolution: "jackspeak@npm:2.3.6"
   dependencies:
     "@isaacs/cliui": ^8.0.2
     "@pkgjs/parseargs": ^0.11.0
   dependenciesMeta:
     "@pkgjs/parseargs":
       optional: true
-  checksum: e29291c0d0f280a063fa18fbd1e891ab8c2d7519fd34052c0ebde38538a15c603140d60c2c7f432375ff7ee4c5f1c10daa8b2ae19a97c3d4affe308c8360c1df
+  checksum: 57d43ad11eadc98cdfe7496612f6bbb5255ea69fe51ea431162db302c2a11011642f50cfad57288bd0aea78384a0612b16e131944ad8ecd09d619041c8531b54
   languageName: node
   linkType: hard
 
 "js-tokens@npm:^3.0.0 || ^4.0.0":
   version: 4.0.0
   resolution: "js-tokens@npm:4.0.0"
   checksum: 8a95213a5a77deb6cbe94d86340e8d9ace2b93bc367790b260101d2f36a2eaf4e4e22d9fa9cf459b38af3a32fb4190e638024cf82ec95ef708680e405ea7cc78
@@ -2813,23 +2658,32 @@
 "jsonpointer@npm:^5.0.1":
   version: 5.0.1
   resolution: "jsonpointer@npm:5.0.1"
   checksum: 0b40f712900ad0c846681ea2db23b6684b9d5eedf55807b4708c656f5894b63507d0e28ae10aa1bddbea551241035afe62b6df0800fc94c2e2806a7f3adecd7c
   languageName: node
   linkType: hard
 
-"lib0@npm:^0.2.42, lib0@npm:^0.2.74":
-  version: 0.2.78
-  resolution: "lib0@npm:0.2.78"
+"jupyterlab_unianalytics_telemetry-ui-tests@workspace:.":
+  version: 0.0.0-use.local
+  resolution: "jupyterlab_unianalytics_telemetry-ui-tests@workspace:."
+  dependencies:
+    "@jupyterlab/galata": ^5.0.5
+    "@playwright/test": ^1.37.0
+  languageName: unknown
+  linkType: soft
+
+"lib0@npm:^0.2.85, lib0@npm:^0.2.86":
+  version: 0.2.88
+  resolution: "lib0@npm:0.2.88"
   dependencies:
     isomorphic.js: ^0.2.4
   bin:
     0gentesthtml: bin/gentesthtml.js
     0serve: bin/0serve.js
-  checksum: a9c90a9228e10e581bf416f4ecade967687d67e6ea3e822ef69e2628a77a2a0254ef7e2eb7e555d412f9e9467049b7fb760c079878f9a934dd85d2646a53d172
+  checksum: 1ac13d6781f4d29aa317ad9fb9b6c41e8bed52b096a369f54d10d9b8651ceb4a0a63b06c01c2e1c7319d3bb74668afb6cac3735161b32031f185cec024bbba37
   languageName: node
   linkType: hard
 
 "lodash-es@npm:^4.17.21":
   version: 4.17.21
   resolution: "lodash-es@npm:4.17.21"
   checksum: 05cbffad6e2adbb331a4e16fbd826e7faee403a1a04873b82b42c0f22090f280839f85b95393f487c1303c8a3d2a010048bf06151a6cbe03eee4d388fb0a12d2
@@ -2864,75 +2718,55 @@
     js-tokens: ^3.0.0 || ^4.0.0
   bin:
     loose-envify: cli.js
   checksum: 6517e24e0cad87ec9888f500c5b5947032cdfe6ef65e1c1936a0c48a524b81e65542c9c3edc91c97d5bddc806ee2a985dbc79be89215d613b1de5db6d1cfe6f4
   languageName: node
   linkType: hard
 
+"lru-cache@npm:^10.0.1, lru-cache@npm:^9.1.1 || ^10.0.0":
+  version: 10.2.0
+  resolution: "lru-cache@npm:10.2.0"
+  checksum: eee7ddda4a7475deac51ac81d7dd78709095c6fa46e8350dc2d22462559a1faa3b81ed931d5464b13d48cbd7e08b46100b6f768c76833912bc444b99c37e25db
+  languageName: node
+  linkType: hard
+
 "lru-cache@npm:^6.0.0":
   version: 6.0.0
   resolution: "lru-cache@npm:6.0.0"
   dependencies:
     yallist: ^4.0.0
   checksum: f97f499f898f23e4585742138a22f22526254fdba6d75d41a1c2526b3b6cc5747ef59c5612ba7375f42aca4f8461950e925ba08c991ead0651b4918b7c978297
   languageName: node
   linkType: hard
 
-"lru-cache@npm:^7.7.1":
-  version: 7.18.3
-  resolution: "lru-cache@npm:7.18.3"
-  checksum: e550d772384709deea3f141af34b6d4fa392e2e418c1498c078de0ee63670f1f46f5eee746e8ef7e69e1c895af0d4224e62ee33e66a543a14763b0f2e74c1356
-  languageName: node
-  linkType: hard
-
-"lru-cache@npm:^9.1.1 || ^10.0.0":
-  version: 10.0.0
-  resolution: "lru-cache@npm:10.0.0"
-  checksum: 18f101675fe283bc09cda0ef1e3cc83781aeb8373b439f086f758d1d91b28730950db785999cd060d3c825a8571c03073e8c14512b6655af2188d623031baf50
-  languageName: node
-  linkType: hard
-
-"make-fetch-happen@npm:^11.0.3":
-  version: 11.1.1
-  resolution: "make-fetch-happen@npm:11.1.1"
+"make-fetch-happen@npm:^13.0.0":
+  version: 13.0.0
+  resolution: "make-fetch-happen@npm:13.0.0"
   dependencies:
-    agentkeepalive: ^4.2.1
-    cacache: ^17.0.0
+    "@npmcli/agent": ^2.0.0
+    cacache: ^18.0.0
     http-cache-semantics: ^4.1.1
-    http-proxy-agent: ^5.0.0
-    https-proxy-agent: ^5.0.0
     is-lambda: ^1.0.1
-    lru-cache: ^7.7.1
-    minipass: ^5.0.0
+    minipass: ^7.0.2
     minipass-fetch: ^3.0.0
     minipass-flush: ^1.0.5
     minipass-pipeline: ^1.2.4
     negotiator: ^0.6.3
     promise-retry: ^2.0.1
-    socks-proxy-agent: ^7.0.0
     ssri: ^10.0.0
-  checksum: 7268bf274a0f6dcf0343829489a4506603ff34bd0649c12058753900b0eb29191dce5dba12680719a5d0a983d3e57810f594a12f3c18494e93a1fbc6348a4540
+  checksum: 7c7a6d381ce919dd83af398b66459a10e2fe8f4504f340d1d090d3fa3d1b0c93750220e1d898114c64467223504bd258612ba83efbc16f31b075cd56de24b4af
   languageName: node
   linkType: hard
 
-"markdown-to-jsx@npm:^7.2.1":
-  version: 7.2.1
-  resolution: "markdown-to-jsx@npm:7.2.1"
+"markdown-to-jsx@npm:^7.4.0":
+  version: 7.4.0
+  resolution: "markdown-to-jsx@npm:7.4.0"
   peerDependencies:
     react: ">= 0.14.0"
-  checksum: 0c8c715229044401ea48c2fc26c2554464100074959dafacdd9e4a0e849f0a190b02f39edb373bbdd95e38b8f910074b83b63d08752b8ae6be6ddcfb40ea50a0
-  languageName: node
-  linkType: hard
-
-"minimatch@npm:^3.1.1":
-  version: 3.1.2
-  resolution: "minimatch@npm:3.1.2"
-  dependencies:
-    brace-expansion: ^1.1.7
-  checksum: c154e566406683e7bcb746e000b84d74465b3a832c45d59912b9b55cd50dee66e5c4b1e5566dba26154040e51672f9aa450a9aef0c97cfc7336b78b7afb9540a
+  checksum: 59959d14d7927ed8a97e42d39771e2b445b90fa098477fb6ab040f044d230517dc4a95ba38a4f924cfc965a96b32211d93def150a6184f0e51d2cefdc8cb415d
   languageName: node
   linkType: hard
 
 "minimatch@npm:^9.0.1":
   version: 9.0.3
   resolution: "minimatch@npm:9.0.3"
   dependencies:
@@ -2944,35 +2778,35 @@
 "minimist@npm:^1.2.0, minimist@npm:~1.2.0":
   version: 1.2.8
   resolution: "minimist@npm:1.2.8"
   checksum: 75a6d645fb122dad29c06a7597bddea977258957ed88d7a6df59b5cd3fe4a527e253e9bbf2e783e4b73657f9098b96a5fe96ab8a113655d4109108577ecf85b0
   languageName: node
   linkType: hard
 
-"minipass-collect@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "minipass-collect@npm:1.0.2"
+"minipass-collect@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "minipass-collect@npm:2.0.1"
   dependencies:
-    minipass: ^3.0.0
-  checksum: 14df761028f3e47293aee72888f2657695ec66bd7d09cae7ad558da30415fdc4752bbfee66287dcc6fd5e6a2fa3466d6c484dc1cbd986525d9393b9523d97f10
+    minipass: ^7.0.3
+  checksum: b251bceea62090f67a6cced7a446a36f4cd61ee2d5cea9aee7fff79ba8030e416327a1c5aa2908dc22629d06214b46d88fdab8c51ac76bacbf5703851b5ad342
   languageName: node
   linkType: hard
 
 "minipass-fetch@npm:^3.0.0":
-  version: 3.0.3
-  resolution: "minipass-fetch@npm:3.0.3"
+  version: 3.0.4
+  resolution: "minipass-fetch@npm:3.0.4"
   dependencies:
     encoding: ^0.1.13
-    minipass: ^5.0.0
+    minipass: ^7.0.3
     minipass-sized: ^1.0.3
     minizlib: ^2.1.2
   dependenciesMeta:
     encoding:
       optional: true
-  checksum: af5ab2552a16fcf505d35fd7ffb84b57f4a0eeb269e6e1d9a2a75824dda48b36e527083250b7cca4a4def21d9544e2ade441e4730e233c0bc2133f6abda31e18
+  checksum: af7aad15d5c128ab1ebe52e043bdf7d62c3c6f0cecb9285b40d7b395e1375b45dcdfd40e63e93d26a0e8249c9efd5c325c65575aceee192883970ff8cb11364a
   languageName: node
   linkType: hard
 
 "minipass-flush@npm:^1.0.5":
   version: 1.0.5
   resolution: "minipass-flush@npm:1.0.5"
   dependencies:
@@ -3011,18 +2845,18 @@
 "minipass@npm:^5.0.0":
   version: 5.0.0
   resolution: "minipass@npm:5.0.0"
   checksum: 425dab288738853fded43da3314a0b5c035844d6f3097a8e3b5b29b328da8f3c1af6fc70618b32c29ff906284cf6406b6841376f21caaadd0793c1d5a6a620ea
   languageName: node
   linkType: hard
 
-"minipass@npm:^5.0.0 || ^6.0.2 || ^7.0.0":
-  version: 7.0.1
-  resolution: "minipass@npm:7.0.1"
-  checksum: fedd1293f6a1b4e406c242a1cecfb75d0a81422bb2c365d999e33a88642fb68d70a89d95b550e08c640b3c0d9162829310e0c58b9b846b9218de25779818c709
+"minipass@npm:^5.0.0 || ^6.0.2 || ^7.0.0, minipass@npm:^7.0.2, minipass@npm:^7.0.3":
+  version: 7.0.4
+  resolution: "minipass@npm:7.0.4"
+  checksum: 87585e258b9488caf2e7acea242fd7856bbe9a2c84a7807643513a338d66f368c7d518200ad7b70a508664d408aa000517647b2930c259a8b1f9f0984f344a21
   languageName: node
   linkType: hard
 
 "minizlib@npm:^2.1.1, minizlib@npm:^2.1.2":
   version: 2.1.2
   resolution: "minizlib@npm:2.1.2"
   dependencies:
@@ -3051,120 +2885,82 @@
 "ms@npm:2.1.2":
   version: 2.1.2
   resolution: "ms@npm:2.1.2"
   checksum: 673cdb2c3133eb050c745908d8ce632ed2c02d85640e2edb3ace856a2266a813b30c613569bf3354fdf4ea7d1a1494add3bfa95e2713baa27d0c2c71fc44f58f
   languageName: node
   linkType: hard
 
-"ms@npm:^2.0.0":
-  version: 2.1.3
-  resolution: "ms@npm:2.1.3"
-  checksum: aa92de608021b242401676e35cfa5aa42dd70cbdc082b916da7fb925c542173e36bce97ea3e804923fe92c0ad991434e4a38327e15a1b5b5f945d66df615ae6d
-  languageName: node
-  linkType: hard
-
-"nanoid@npm:^3.3.6":
-  version: 3.3.6
-  resolution: "nanoid@npm:3.3.6"
+"nanoid@npm:^3.3.7":
+  version: 3.3.7
+  resolution: "nanoid@npm:3.3.7"
   bin:
     nanoid: bin/nanoid.cjs
-  checksum: 7d0eda657002738aa5206107bd0580aead6c95c460ef1bdd0b1a87a9c7ae6277ac2e9b945306aaa5b32c6dcb7feaf462d0f552e7f8b5718abfc6ead5c94a71b3
+  checksum: d36c427e530713e4ac6567d488b489a36582ef89da1d6d4e3b87eded11eb10d7042a877958c6f104929809b2ab0bafa17652b076cdf84324aa75b30b722204f2
   languageName: node
   linkType: hard
 
 "negotiator@npm:^0.6.3":
   version: 0.6.3
   resolution: "negotiator@npm:0.6.3"
   checksum: b8ffeb1e262eff7968fc90a2b6767b04cfd9842582a9d0ece0af7049537266e7b2506dfb1d107a32f06dd849ab2aea834d5830f7f4d0e5cb7d36e1ae55d021d9
   languageName: node
   linkType: hard
 
 "node-fetch@npm:^2.6.7":
-  version: 2.6.12
-  resolution: "node-fetch@npm:2.6.12"
+  version: 2.7.0
+  resolution: "node-fetch@npm:2.7.0"
   dependencies:
     whatwg-url: ^5.0.0
   peerDependencies:
     encoding: ^0.1.0
   peerDependenciesMeta:
     encoding:
       optional: true
-  checksum: 3bc1655203d47ee8e313c0d96664b9673a3d4dd8002740318e9d27d14ef306693a4b2ef8d6525775056fd912a19e23f3ac0d7111ad8925877b7567b29a625592
+  checksum: d76d2f5edb451a3f05b15115ec89fc6be39de37c6089f1b6368df03b91e1633fd379a7e01b7ab05089a25034b2023d959b47e59759cb38d88341b2459e89d6e5
   languageName: node
   linkType: hard
 
 "node-gyp@npm:latest":
-  version: 9.4.0
-  resolution: "node-gyp@npm:9.4.0"
+  version: 10.0.1
+  resolution: "node-gyp@npm:10.0.1"
   dependencies:
     env-paths: ^2.2.0
     exponential-backoff: ^3.1.1
-    glob: ^7.1.4
+    glob: ^10.3.10
     graceful-fs: ^4.2.6
-    make-fetch-happen: ^11.0.3
-    nopt: ^6.0.0
-    npmlog: ^6.0.0
-    rimraf: ^3.0.2
+    make-fetch-happen: ^13.0.0
+    nopt: ^7.0.0
+    proc-log: ^3.0.0
     semver: ^7.3.5
     tar: ^6.1.2
-    which: ^2.0.2
+    which: ^4.0.0
   bin:
     node-gyp: bin/node-gyp.js
-  checksum: 78b404e2e0639d64e145845f7f5a3cb20c0520cdaf6dda2f6e025e9b644077202ea7de1232396ba5bde3fee84cdc79604feebe6ba3ec84d464c85d407bb5da99
+  checksum: 60a74e66d364903ce02049966303a57f898521d139860ac82744a5fdd9f7b7b3b61f75f284f3bfe6e6add3b8f1871ce305a1d41f775c7482de837b50c792223f
   languageName: node
   linkType: hard
 
-"nopt@npm:^6.0.0":
-  version: 6.0.0
-  resolution: "nopt@npm:6.0.0"
+"nopt@npm:^7.0.0":
+  version: 7.2.0
+  resolution: "nopt@npm:7.2.0"
   dependencies:
-    abbrev: ^1.0.0
+    abbrev: ^2.0.0
   bin:
     nopt: bin/nopt.js
-  checksum: 82149371f8be0c4b9ec2f863cc6509a7fd0fa729929c009f3a58e4eb0c9e4cae9920e8f1f8eb46e7d032fec8fb01bede7f0f41a67eb3553b7b8e14fa53de1dac
-  languageName: node
-  linkType: hard
-
-"jupyterlab_unianalytics_telemetry-ui-tests@workspace:.":
-  version: 0.0.0-use.local
-  resolution: "jupyterlab_unianalytics_telemetry-ui-tests@workspace:."
-  dependencies:
-    "@jupyterlab/galata": ^5.0.0
-    "@playwright/test": ^1.32.0
-  languageName: unknown
-  linkType: soft
-
-"npmlog@npm:^6.0.0":
-  version: 6.0.2
-  resolution: "npmlog@npm:6.0.2"
-  dependencies:
-    are-we-there-yet: ^3.0.0
-    console-control-strings: ^1.1.0
-    gauge: ^4.0.3
-    set-blocking: ^2.0.0
-  checksum: ae238cd264a1c3f22091cdd9e2b106f684297d3c184f1146984ecbe18aaa86343953f26b9520dedd1b1372bc0316905b736c1932d778dbeb1fcf5a1001390e2a
+  checksum: a9c0f57fb8cb9cc82ae47192ca2b7ef00e199b9480eed202482c962d61b59a7fbe7541920b2a5839a97b42ee39e288c0aed770e38057a608d7f579389dfde410
   languageName: node
   linkType: hard
 
 "object-assign@npm:^4.1.1":
   version: 4.1.1
   resolution: "object-assign@npm:4.1.1"
   checksum: fcc6e4ea8c7fe48abfbb552578b1c53e0d194086e2e6bbbf59e0a536381a292f39943c6e9628af05b5528aa5e3318bb30d6b2e53cadaf5b8fe9e12c4b69af23f
   languageName: node
   linkType: hard
 
-"once@npm:^1.3.0":
-  version: 1.4.0
-  resolution: "once@npm:1.4.0"
-  dependencies:
-    wrappy: 1
-  checksum: cd0a88501333edd640d95f0d2700fbde6bff20b3d4d9bdc521bdd31af0656b5706570d6c6afe532045a20bb8dc0849f8332d6f2a416e0ba6d3d3b98806c7db68
-  languageName: node
-  linkType: hard
-
 "p-map@npm:^4.0.0":
   version: 4.0.0
   resolution: "p-map@npm:4.0.0"
   dependencies:
     aggregate-error: ^3.0.0
   checksum: cb0ab21ec0f32ddffd31dfc250e3afa61e103ef43d957cc45497afe37513634589316de4eb88abdfd969fe6410c22c0b93ab24328833b8eb1ccc087fc0442a1c
   languageName: node
@@ -3180,21 +2976,14 @@
 "path-browserify@npm:^1.0.0":
   version: 1.0.1
   resolution: "path-browserify@npm:1.0.1"
   checksum: c6d7fa376423fe35b95b2d67990060c3ee304fc815ff0a2dc1c6c3cfaff2bd0d572ee67e18f19d0ea3bbe32e8add2a05021132ac40509416459fffee35200699
   languageName: node
   linkType: hard
 
-"path-is-absolute@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "path-is-absolute@npm:1.0.1"
-  checksum: 060840f92cf8effa293bcc1bea81281bd7d363731d214cbe5c227df207c34cd727430f70c6037b5159c8a870b9157cba65e775446b0ab06fd5ecc7e54615a3b8
-  languageName: node
-  linkType: hard
-
 "path-key@npm:^3.1.0":
   version: 3.1.1
   resolution: "path-key@npm:3.1.1"
   checksum: 55cd7a9dd4b343412a8386a743f9c746ef196e57c823d90ca3ab917f90ab9f13dd0ded27252ba49dbdfcab2b091d998bc446f6220cd3cea65db407502a740020
   languageName: node
   linkType: hard
 
@@ -3221,31 +3010,53 @@
 "picocolors@npm:^1.0.0":
   version: 1.0.0
   resolution: "picocolors@npm:1.0.0"
   checksum: a2e8092dd86c8396bdba9f2b5481032848525b3dc295ce9b57896f931e63fc16f79805144321f72976383fc249584672a75cc18d6777c6b757603f372f745981
   languageName: node
   linkType: hard
 
-"playwright-core@npm:1.35.1":
-  version: 1.35.1
-  resolution: "playwright-core@npm:1.35.1"
+"playwright-core@npm:1.41.1":
+  version: 1.41.1
+  resolution: "playwright-core@npm:1.41.1"
   bin:
     playwright-core: cli.js
-  checksum: 179abc0051f00474e528935b507fa8cedc986b2803b020d7679878ba28cdd7036ad5a779792aad2ad281f8dc625eb1d2fb77663cb8de0d20c7ffbda7c18febdd
+  checksum: c83446a560c6bd85f6f0cd586ff8c643b77e2005567386e12f85890936cc370673114b94cd883246018797cc1580e93b0296ade7d07275bb611b8962f5bb9693
+  languageName: node
+  linkType: hard
+
+"playwright@npm:1.41.1":
+  version: 1.41.1
+  resolution: "playwright@npm:1.41.1"
+  dependencies:
+    fsevents: 2.3.2
+    playwright-core: 1.41.1
+  dependenciesMeta:
+    fsevents:
+      optional: true
+  bin:
+    playwright: cli.js
+  checksum: 3da7fb929abdec6adbdd8829f840580f5f210713214a8d230b130127f2270403eb2113c6c1418012221149707250fff896794c7c22c260dd09a92bf800227f31
   languageName: node
   linkType: hard
 
 "postcss@npm:^8.3.11":
-  version: 8.4.25
-  resolution: "postcss@npm:8.4.25"
+  version: 8.4.33
+  resolution: "postcss@npm:8.4.33"
   dependencies:
-    nanoid: ^3.3.6
+    nanoid: ^3.3.7
     picocolors: ^1.0.0
     source-map-js: ^1.0.2
-  checksum: 9ed3ab8af43ad5210c28f56f916fd9b8c9f94fbeaebbf645dcf579bc28bdd8056c2a7ecc934668d399b81fedb6128f0c4b299f931e50454964bc911c25a3a0a2
+  checksum: 6f98b2af4b76632a3de20c4f47bf0e984a1ce1a531cf11adcb0b1d63a6cbda0aae4165e578b66c32ca4879038e3eaad386a6be725a8fb4429c78e3c1ab858fe9
+  languageName: node
+  linkType: hard
+
+"proc-log@npm:^3.0.0":
+  version: 3.0.0
+  resolution: "proc-log@npm:3.0.0"
+  checksum: 02b64e1b3919e63df06f836b98d3af002b5cd92655cab18b5746e37374bfb73e03b84fe305454614b34c25b485cc687a9eebdccf0242cda8fda2475dd2c97e02
   languageName: node
   linkType: hard
 
 "process-nextick-args@npm:~2.0.0":
   version: 2.0.1
   resolution: "process-nextick-args@npm:2.0.1"
   checksum: 1d38588e520dab7cea67cbbe2efdd86a10cc7a074c09657635e34f035277b59fbb57d09d8638346bf7090f8e8ebc070c96fa5fd183b777fff4f5edff5e9466cf
@@ -3277,17 +3088,17 @@
     object-assign: ^4.1.1
     react-is: ^16.13.1
   checksum: c056d3f1c057cb7ff8344c645450e14f088a915d078dcda795041765047fa080d38e5d626560ccaac94a4e16e3aa15f3557c1a9a8d1174530955e992c675e459
   languageName: node
   linkType: hard
 
 "punycode@npm:^2.1.0":
-  version: 2.3.0
-  resolution: "punycode@npm:2.3.0"
-  checksum: 39f760e09a2a3bbfe8f5287cf733ecdad69d6af2fe6f97ca95f24b8921858b91e9ea3c9eeec6e08cede96181b3bb33f95c6ffd8c77e63986508aa2e8159fa200
+  version: 2.3.1
+  resolution: "punycode@npm:2.3.1"
+  checksum: bb0a0ceedca4c3c57a9b981b90601579058903c62be23c5e8e843d2c2d4148a3ecf029d5133486fb0e1822b098ba8bba09e89d6b21742d02fa26bda6441a6fb2
   languageName: node
   linkType: hard
 
 "querystringify@npm:^2.1.1":
   version: 2.2.0
   resolution: "querystringify@npm:2.2.0"
   checksum: 5641ea231bad7ef6d64d9998faca95611ed4b11c2591a8cae741e178a974f6a8e0ebde008475259abe1621cb15e692404e6b6626e927f7b849d5c09392604b15
@@ -3340,25 +3151,14 @@
     safe-buffer: ~5.1.1
     string_decoder: ~1.1.1
     util-deprecate: ~1.0.1
   checksum: 65645467038704f0c8aaf026a72fbb588a9e2ef7a75cd57a01702ee9db1c4a1e4b03aaad36861a6a0926546a74d174149c8c207527963e0c2d3eee2f37678a42
   languageName: node
   linkType: hard
 
-"readable-stream@npm:^3.6.0":
-  version: 3.6.2
-  resolution: "readable-stream@npm:3.6.2"
-  dependencies:
-    inherits: ^2.0.3
-    string_decoder: ^1.1.1
-    util-deprecate: ^1.0.1
-  checksum: bdcbe6c22e846b6af075e32cf8f4751c2576238c5043169a1c221c92ee2878458a816a4ea33f4c67623c0b6827c8a400409bfb3cf0bf3381392d0b1dfb52ac8d
-  languageName: node
-  linkType: hard
-
 "regexp-match-indices@npm:^1.0.2":
   version: 1.0.2
   resolution: "regexp-match-indices@npm:1.0.2"
   dependencies:
     regexp-tree: ^0.1.11
   checksum: 8cc779f6cf8f404ead828d09970a7d4bd66bd78d43ab9eb2b5e65f2ef2ba1ed53536f5b5fa839fb90b350365fb44b6a851c7f16289afc3f37789c113ab2a7916
   languageName: node
@@ -3397,26 +3197,15 @@
 "retry@npm:^0.12.0":
   version: 0.12.0
   resolution: "retry@npm:0.12.0"
   checksum: 623bd7d2e5119467ba66202d733ec3c2e2e26568074923bc0585b6b99db14f357e79bdedb63cab56cec47491c4a0da7e6021a7465ca6dc4f481d3898fdd3158c
   languageName: node
   linkType: hard
 
-"rimraf@npm:^3.0.2":
-  version: 3.0.2
-  resolution: "rimraf@npm:3.0.2"
-  dependencies:
-    glob: ^7.1.3
-  bin:
-    rimraf: bin.js
-  checksum: 87f4164e396f0171b0a3386cc1877a817f572148ee13a7e113b238e48e8a9f2f31d009a92ec38a591ff1567d9662c6b67fd8818a2dbbaed74bc26a87a2a4a9a0
-  languageName: node
-  linkType: hard
-
-"robust-predicates@npm:^3.0.0":
+"robust-predicates@npm:^3.0.2":
   version: 3.0.2
   resolution: "robust-predicates@npm:3.0.2"
   checksum: 36854c1321548ceca96d36ad9d6e0a5a512986029ec6929ad6ed3ec1612c22cc8b46cc72d2c5674af42e8074a119d793f6f0ea3a5b51373e3ab926c64b172d7a
   languageName: node
   linkType: hard
 
 "rw@npm:1":
@@ -3429,21 +3218,14 @@
 "safe-buffer@npm:~5.1.0, safe-buffer@npm:~5.1.1":
   version: 5.1.2
   resolution: "safe-buffer@npm:5.1.2"
   checksum: f2f1f7943ca44a594893a852894055cf619c1fbcb611237fc39e461ae751187e7baf4dc391a72125e0ac4fb2d8c5c0b3c71529622e6a58f46b960211e704903c
   languageName: node
   linkType: hard
 
-"safe-buffer@npm:~5.2.0":
-  version: 5.2.1
-  resolution: "safe-buffer@npm:5.2.1"
-  checksum: b99c4b41fdd67a6aaf280fcd05e9ffb0813654894223afb78a31f14a19ad220bba8aba1cb14eddce1fcfb037155fe6de4e861784eb434f7d11ed58d1e70dd491
-  languageName: node
-  linkType: hard
-
 "safer-buffer@npm:>= 2.1.2 < 3.0.0":
   version: 2.1.2
   resolution: "safer-buffer@npm:2.1.2"
   checksum: cab8f25ae6f1434abee8d80023d7e72b598cf1327164ddab31003c51215526801e40b66c5e65d658a0af1e9d6478cadcb4c745f4bd6751f97d8644786c0978b0
   languageName: node
   linkType: hard
 
@@ -3477,21 +3259,14 @@
     lru-cache: ^6.0.0
   bin:
     semver: bin/semver.js
   checksum: 12d8ad952fa353b0995bf180cdac205a4068b759a140e5d3c608317098b3575ac2f1e09182206bf2eb26120e1c0ed8fb92c48c592f6099680de56bb071423ca3
   languageName: node
   linkType: hard
 
-"set-blocking@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "set-blocking@npm:2.0.0"
-  checksum: 6e65a05f7cf7ebdf8b7c75b101e18c0b7e3dff4940d480efed8aad3a36a4005140b660fa1d804cb8bce911cac290441dc728084a30504d3516ac2ff7ad607b02
-  languageName: node
-  linkType: hard
-
 "shebang-command@npm:^2.0.0":
   version: 2.0.0
   resolution: "shebang-command@npm:2.0.0"
   dependencies:
     shebang-regex: ^3.0.0
   checksum: 6b52fe87271c12968f6a054e60f6bde5f0f3d2db483a1e5c3e12d657c488a15474121a1d55cd958f6df026a54374ec38a4a963988c213b7570e1d51575cea7fa
   languageName: node
@@ -3500,47 +3275,40 @@
 "shebang-regex@npm:^3.0.0":
   version: 3.0.0
   resolution: "shebang-regex@npm:3.0.0"
   checksum: 1a2bcae50de99034fcd92ad4212d8e01eedf52c7ec7830eedcf886622804fe36884278f2be8be0ea5fde3fd1c23911643a4e0f726c8685b61871c8908af01222
   languageName: node
   linkType: hard
 
-"signal-exit@npm:^3.0.7":
-  version: 3.0.7
-  resolution: "signal-exit@npm:3.0.7"
-  checksum: a2f098f247adc367dffc27845853e9959b9e88b01cb301658cfe4194352d8d2bb32e18467c786a7fe15f1d44b233ea35633d076d5e737870b7139949d1ab6318
-  languageName: node
-  linkType: hard
-
 "signal-exit@npm:^4.0.1":
-  version: 4.0.2
-  resolution: "signal-exit@npm:4.0.2"
-  checksum: 41f5928431cc6e91087bf0343db786a6313dd7c6fd7e551dbc141c95bb5fb26663444fd9df8ea47c5d7fc202f60aa7468c3162a9365cbb0615fc5e1b1328fe31
+  version: 4.1.0
+  resolution: "signal-exit@npm:4.1.0"
+  checksum: 64c757b498cb8629ffa5f75485340594d2f8189e9b08700e69199069c8e3070fb3e255f7ab873c05dc0b3cec412aea7402e10a5990cb6a050bd33ba062a6c549
   languageName: node
   linkType: hard
 
 "smart-buffer@npm:^4.2.0":
   version: 4.2.0
   resolution: "smart-buffer@npm:4.2.0"
   checksum: b5167a7142c1da704c0e3af85c402002b597081dd9575031a90b4f229ca5678e9a36e8a374f1814c8156a725d17008ae3bde63b92f9cfd132526379e580bec8b
   languageName: node
   linkType: hard
 
-"socks-proxy-agent@npm:^7.0.0":
-  version: 7.0.0
-  resolution: "socks-proxy-agent@npm:7.0.0"
+"socks-proxy-agent@npm:^8.0.1":
+  version: 8.0.2
+  resolution: "socks-proxy-agent@npm:8.0.2"
   dependencies:
-    agent-base: ^6.0.2
-    debug: ^4.3.3
-    socks: ^2.6.2
-  checksum: 720554370154cbc979e2e9ce6a6ec6ced205d02757d8f5d93fe95adae454fc187a5cbfc6b022afab850a5ce9b4c7d73e0f98e381879cf45f66317a4895953846
+    agent-base: ^7.0.2
+    debug: ^4.3.4
+    socks: ^2.7.1
+  checksum: 4fb165df08f1f380881dcd887b3cdfdc1aba3797c76c1e9f51d29048be6e494c5b06d68e7aea2e23df4572428f27a3ec22b3d7c75c570c5346507433899a4b6d
   languageName: node
   linkType: hard
 
-"socks@npm:^2.6.2":
+"socks@npm:^2.7.1":
   version: 2.7.1
   resolution: "socks@npm:2.7.1"
   dependencies:
     ip: ^2.0.0
     smart-buffer: ^4.2.0
   checksum: 259d9e3e8e1c9809a7f5c32238c3d4d2a36b39b83851d0f573bfde5f21c4b1288417ce1af06af1452569cd1eb0841169afd4998f0e04ba04656f6b7f0e46d748
   languageName: node
@@ -3550,23 +3318,23 @@
   version: 1.0.2
   resolution: "source-map-js@npm:1.0.2"
   checksum: c049a7fc4deb9a7e9b481ae3d424cc793cb4845daa690bc5a05d428bf41bf231ced49b4cf0c9e77f9d42fdb3d20d6187619fc586605f5eabe995a316da8d377c
   languageName: node
   linkType: hard
 
 "ssri@npm:^10.0.0":
-  version: 10.0.4
-  resolution: "ssri@npm:10.0.4"
+  version: 10.0.5
+  resolution: "ssri@npm:10.0.5"
   dependencies:
-    minipass: ^5.0.0
-  checksum: fb14da9f8a72b04eab163eb13a9dda11d5962cd2317f85457c4e0b575e9a6e0e3a6a87b5bf122c75cb36565830cd5f263fb457571bf6f1587eb5f95d095d6165
+    minipass: ^7.0.3
+  checksum: 0a31b65f21872dea1ed3f7c200d7bc1c1b91c15e419deca14f282508ba917cbb342c08a6814c7f68ca4ca4116dd1a85da2bbf39227480e50125a1ceffeecb750
   languageName: node
   linkType: hard
 
-"string-width-cjs@npm:string-width@^4.2.0, string-width@npm:^1.0.2 || 2 || 3 || 4, string-width@npm:^4.1.0, string-width@npm:^4.2.0, string-width@npm:^4.2.3":
+"string-width-cjs@npm:string-width@^4.2.0, string-width@npm:^4.1.0, string-width@npm:^4.2.0, string-width@npm:^4.2.3":
   version: 4.2.3
   resolution: "string-width@npm:4.2.3"
   dependencies:
     emoji-regex: ^8.0.0
     is-fullwidth-code-point: ^3.0.0
     strip-ansi: ^6.0.1
   checksum: e52c10dc3fbfcd6c3a15f159f54a90024241d0f149cf8aed2982a2d801d2e64df0bf1dc351cf8e95c3319323f9f220c16e740b06faecd53e2462df1d2b5443fb
@@ -3580,23 +3348,14 @@
     eastasianwidth: ^0.2.0
     emoji-regex: ^9.2.2
     strip-ansi: ^7.0.1
   checksum: 7369deaa29f21dda9a438686154b62c2c5f661f8dda60449088f9f980196f7908fc39fdd1803e3e01541970287cf5deae336798337e9319a7055af89dafa7193
   languageName: node
   linkType: hard
 
-"string_decoder@npm:^1.1.1":
-  version: 1.3.0
-  resolution: "string_decoder@npm:1.3.0"
-  dependencies:
-    safe-buffer: ~5.2.0
-  checksum: 8417646695a66e73aefc4420eb3b84cc9ffd89572861fe004e6aeb13c7bc00e2f616247505d2dbbef24247c372f70268f594af7126f43548565c68c117bdeb56
-  languageName: node
-  linkType: hard
-
 "string_decoder@npm:~1.1.1":
   version: 1.1.1
   resolution: "string_decoder@npm:1.1.1"
   dependencies:
     safe-buffer: ~5.1.0
   checksum: 9ab7e56f9d60a28f2be697419917c50cac19f3e8e6c28ef26ed5f4852289fe0de5d6997d29becf59028556f2c62983790c1d9ba1e2a3cc401768ca12d5183a5b
   languageName: node
@@ -3616,42 +3375,42 @@
   resolution: "strip-ansi@npm:7.1.0"
   dependencies:
     ansi-regex: ^6.0.1
   checksum: 859c73fcf27869c22a4e4d8c6acfe690064659e84bef9458aa6d13719d09ca88dcfd40cbf31fd0be63518ea1a643fe070b4827d353e09533a5b0b9fd4553d64d
   languageName: node
   linkType: hard
 
-"style-mod@npm:^4.0.0":
-  version: 4.0.3
-  resolution: "style-mod@npm:4.0.3"
-  checksum: 934556e720bd29026ff8fef43a1a35b58957813025b91f996d886e9405acf934ddb1934def4400b174bd7784c9263eb9c71f07ae83925af9271b7d921d546854
+"style-mod@npm:^4.0.0, style-mod@npm:^4.1.0":
+  version: 4.1.0
+  resolution: "style-mod@npm:4.1.0"
+  checksum: 8402b14ca11113a3640d46b3cf7ba49f05452df7846bc5185a3535d9b6a64a3019e7fb636b59ccbb7816aeb0725b24723e77a85b05612a9360e419958e13b4e6
   languageName: node
   linkType: hard
 
 "systeminformation@npm:^5.8.6":
-  version: 5.18.6
-  resolution: "systeminformation@npm:5.18.6"
+  version: 5.21.24
+  resolution: "systeminformation@npm:5.21.24"
   bin:
     systeminformation: lib/cli.js
-  checksum: c7bd43bd55c8cb8f95e4d209f6bcf1979c86e0a5a26d4dda2cb439bfdbfd11e8d48b64a5d519198cacf43446e1489f2b6252ff49885ccc8846eeee0f2cdc3543
+  checksum: d3cfe6a1b1e58494ca0a149e5fcf39f0fa09cda2813a1b9cdf7b0265a2cfd1fb98f331e78c4a7a92c74e87c4c1d83c10ef5f8f8db6e134f8223d7aa41b5137a6
   conditions: (os=darwin | os=linux | os=win32 | os=freebsd | os=openbsd | os=netbsd | os=sunos | os=android)
   languageName: node
   linkType: hard
 
 "tar@npm:^6.1.11, tar@npm:^6.1.2":
-  version: 6.1.15
-  resolution: "tar@npm:6.1.15"
+  version: 6.2.0
+  resolution: "tar@npm:6.2.0"
   dependencies:
     chownr: ^2.0.0
     fs-minipass: ^2.0.0
     minipass: ^5.0.0
     minizlib: ^2.1.1
     mkdirp: ^1.0.3
     yallist: ^4.0.0
-  checksum: f23832fceeba7578bf31907aac744ae21e74a66f4a17a9e94507acf460e48f6db598c7023882db33bab75b80e027c21f276d405e4a0322d58f51c7088d428268
+  checksum: db4d9fe74a2082c3a5016630092c54c8375ff3b280186938cfd104f2e089c4fd9bad58688ef6be9cf186a889671bf355c7cda38f09bbf60604b281715ca57f5c
   languageName: node
   linkType: hard
 
 "topojson-client@npm:^3.1.0":
   version: 3.1.0
   resolution: "topojson-client@npm:3.1.0"
   dependencies:
@@ -3667,18 +3426,18 @@
 "tr46@npm:~0.0.3":
   version: 0.0.3
   resolution: "tr46@npm:0.0.3"
   checksum: 726321c5eaf41b5002e17ffbd1fb7245999a073e8979085dacd47c4b4e8068ff5777142fc6726d6ca1fd2ff16921b48788b87225cbc57c72636f6efa8efbffe3
   languageName: node
   linkType: hard
 
-"tslib@npm:~2.5.0":
-  version: 2.5.3
-  resolution: "tslib@npm:2.5.3"
-  checksum: 88902b309afaf83259131c1e13da1dceb0ad1682a213143a1346a649143924d78cf3760c448b84d796938fd76127183894f8d85cbb3bf9c4fddbfcc140c0003c
+"tslib@npm:~2.6.2":
+  version: 2.6.2
+  resolution: "tslib@npm:2.6.2"
+  checksum: 329ea56123005922f39642318e3d1f0f8265d1e7fcb92c633e0809521da75eeaca28d2cf96d7248229deb40e5c19adf408259f4b9640afd20d13aecc1430f3ad
   languageName: node
   linkType: hard
 
 "typestyle@npm:^2.0.4":
   version: 2.4.0
   resolution: "typestyle@npm:2.4.0"
   dependencies:
@@ -3703,17 +3462,17 @@
   dependencies:
     imurmurhash: ^0.1.4
   checksum: 0884b58365af59f89739e6f71e3feacb5b1b41f2df2d842d0757933620e6de08eff347d27e9d499b43c40476cbaf7988638d3acb2ffbcb9d35fd035591adfd15
   languageName: node
   linkType: hard
 
 "universalify@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "universalify@npm:2.0.0"
-  checksum: 2406a4edf4a8830aa6813278bab1f953a8e40f2f63a37873ffa9a3bc8f9745d06cc8e88f3572cb899b7e509013f7f6fcc3e37e8a6d914167a5381d8440518c44
+  version: 2.0.1
+  resolution: "universalify@npm:2.0.1"
+  checksum: ecd8469fe0db28e7de9e5289d32bd1b6ba8f7183db34f3bfc4ca53c49891c2d6aa05f3fb3936a81285a905cc509fb641a0c3fc131ec786167eff41236ae32e60
   languageName: node
   linkType: hard
 
 "uri-js@npm:^4.2.2":
   version: 4.4.1
   resolution: "uri-js@npm:4.4.1"
   dependencies:
@@ -3728,15 +3487,15 @@
   dependencies:
     querystringify: ^2.1.1
     requires-port: ^1.0.0
   checksum: fbdba6b1d83336aca2216bbdc38ba658d9cfb8fc7f665eb8b17852de638ff7d1a162c198a8e4ed66001ddbf6c9888d41e4798912c62b4fd777a31657989f7bdf
   languageName: node
   linkType: hard
 
-"util-deprecate@npm:^1.0.1, util-deprecate@npm:~1.0.1":
+"util-deprecate@npm:~1.0.1":
   version: 1.0.2
   resolution: "util-deprecate@npm:1.0.2"
   checksum: 474acf1146cb2701fe3b074892217553dfcf9a031280919ba1b8d651a068c9b15d863b7303cb15bd00a862b498e6cf4ad7b4a08fb134edd5a6f7641681cb54a2
   languageName: node
   linkType: hard
 
 "util@npm:^0.10.3":
@@ -3867,30 +3626,30 @@
     d3-time-format: ^4.1.0
     vega-time: ^2.1.1
     vega-util: ^1.17.1
   checksum: d506acb8611a6340ff419ebf308a758a54aaf3cf141863553df83980dcf8dc7bf806bee257d11a52d43682d159d7be03ab8a92bdd4d018d8c9f39a70c45cb197
   languageName: node
   linkType: hard
 
-"vega-functions@npm:^5.13.1, vega-functions@npm:~5.13.2":
-  version: 5.13.2
-  resolution: "vega-functions@npm:5.13.2"
+"vega-functions@npm:^5.13.1, vega-functions@npm:^5.14.0, vega-functions@npm:~5.14.0":
+  version: 5.14.0
+  resolution: "vega-functions@npm:5.14.0"
   dependencies:
     d3-array: ^3.2.2
     d3-color: ^3.1.0
     d3-geo: ^3.1.0
     vega-dataflow: ^5.7.5
     vega-expression: ^5.1.0
     vega-scale: ^7.3.0
     vega-scenegraph: ^4.10.2
-    vega-selections: ^5.4.1
+    vega-selections: ^5.4.2
     vega-statistics: ^1.8.1
     vega-time: ^2.1.1
     vega-util: ^1.17.1
-  checksum: 178498cf93c3d9ef392fb57a5c7992dbb9118c546a6acb4cff9783f911fb30dbf50634cbfd6e3a9bc358c4aec9a571bd55f9cf3de551213cd386f152ac882986
+  checksum: 24857fade62d122ce95ddae87637ade069cac36018e53814cf0ef52055af574641e221199e9baaa8a648cba4fd607c469de7a5e5a0d630e2a676018bfa894673
   languageName: node
   linkType: hard
 
 "vega-geo@npm:~4.4.1":
   version: 4.4.1
   resolution: "vega-geo@npm:4.4.1"
   dependencies:
@@ -3926,35 +3685,31 @@
     vega-scenegraph: ^4.9.2
     vega-util: ^1.15.2
   checksum: 2704c99328ead677441e746acd8f4529301437d08b2758933fc13353d2eab9af353e4ebcc4ff1f09f41d600401b097e2df3c9e8e56d4861e5216222dd9e29185
   languageName: node
   linkType: hard
 
 "vega-lite@npm:^5.6.1":
-  version: 5.13.0
-  resolution: "vega-lite@npm:5.13.0"
+  version: 5.16.3
+  resolution: "vega-lite@npm:5.16.3"
   dependencies:
-    "@types/clone": ~2.1.1
-    clone: ~2.1.2
-    fast-deep-equal: ~3.1.3
-    fast-json-stable-stringify: ~2.1.0
     json-stringify-pretty-compact: ~3.0.0
-    tslib: ~2.5.0
+    tslib: ~2.6.2
     vega-event-selector: ~3.0.1
     vega-expression: ~5.1.0
     vega-util: ~1.17.2
     yargs: ~17.7.2
   peerDependencies:
     vega: ^5.24.0
   bin:
     vl2pdf: bin/vl2pdf
     vl2png: bin/vl2png
     vl2svg: bin/vl2svg
     vl2vg: bin/vl2vg
-  checksum: e177a649d8984770b1531985a1d7f68b533395c3a4ec23018650f8991ad2b83081ededadfbbfbe475c01e40112c1314e29c2c1be32623d47b4a411a640a14082
+  checksum: 9614bfe62de8ca82ea270f0ae05ef8798a0c1b83521eaede4c8c78be66892ca516ea8800b079916529102337e3cc295e404144420c4463145ee5551db7f52dfd
   languageName: node
   linkType: hard
 
 "vega-loader@npm:^4.5.1, vega-loader@npm:~4.5.1":
   version: 4.5.1
   resolution: "vega-loader@npm:4.5.1"
   dependencies:
@@ -3963,24 +3718,24 @@
     topojson-client: ^3.1.0
     vega-format: ^1.1.1
     vega-util: ^1.17.1
   checksum: 95f6eebc75a97665cf34faaea431934047e1b2e9d7532f48f62dab4884d606a7d9da53962e1631a5790a7a867f720581852a3db9be1a7f667882062f6c102ee0
   languageName: node
   linkType: hard
 
-"vega-parser@npm:~6.2.0":
-  version: 6.2.0
-  resolution: "vega-parser@npm:6.2.0"
+"vega-parser@npm:~6.2.1":
+  version: 6.2.1
+  resolution: "vega-parser@npm:6.2.1"
   dependencies:
     vega-dataflow: ^5.7.5
     vega-event-selector: ^3.0.1
-    vega-functions: ^5.13.1
-    vega-scale: ^7.3.0
-    vega-util: ^1.17.1
-  checksum: 19872153c16aab30c4df338e0df7bd331e0bf74c7c6afce5428df555b9bdb0c4acf76b54092cacd4726a1349912ea803c90e1b30d53f4a02044e0559873969a7
+    vega-functions: ^5.14.0
+    vega-scale: ^7.3.1
+    vega-util: ^1.17.2
+  checksum: d30161f84e6b6de1b74b7cb0b9435f281c0f1db91a9d968ab975bae250d36598f24e3fab2063390ad6445614f1f16f85fd99af55d7b65e3d73ce8ffca153ba47
   languageName: node
   linkType: hard
 
 "vega-projection@npm:^1.6.0, vega-projection@npm:~1.6.0":
   version: 1.6.0
   resolution: "vega-projection@npm:1.6.0"
   dependencies:
@@ -4009,49 +3764,49 @@
   dependencies:
     vega-dataflow: ^5.7.5
     vega-util: ^1.17.1
   checksum: a1da40ddb3109f1ced8e61d2e7b52784fbb29936ee4c47cb5630dbbeb12ef6e0c3cd3cd189c34377f82402bf19c61dd148d90330fec743b8667635ac48e4ba29
   languageName: node
   linkType: hard
 
-"vega-scale@npm:^7.3.0, vega-scale@npm:~7.3.0":
-  version: 7.3.0
-  resolution: "vega-scale@npm:7.3.0"
+"vega-scale@npm:^7.3.0, vega-scale@npm:^7.3.1, vega-scale@npm:~7.3.1":
+  version: 7.3.1
+  resolution: "vega-scale@npm:7.3.1"
   dependencies:
     d3-array: ^3.2.2
     d3-interpolate: ^3.0.1
     d3-scale: ^4.0.2
     vega-time: ^2.1.1
     vega-util: ^1.17.1
-  checksum: 8e434f27a51a913dd18374ec0d2bc33758eda7db1ee6342721644f977e705268b8df6b3e89813774d776d03a0cd24f91d4d59f9e80951f67dfbbf8637f5a69ad
+  checksum: c1f6a97b26bbf7b4d1d907e8851d8ac6b58200aa331a1b6c0f67f11aa1ce0ced6d121ac4b2036dbca5779429f41eae4013fe7dd55e09802feda8666b5a0a7ece
   languageName: node
   linkType: hard
 
-"vega-scenegraph@npm:^4.10.2, vega-scenegraph@npm:^4.9.2, vega-scenegraph@npm:~4.10.2":
-  version: 4.10.2
-  resolution: "vega-scenegraph@npm:4.10.2"
+"vega-scenegraph@npm:^4.10.2, vega-scenegraph@npm:^4.9.2, vega-scenegraph@npm:~4.11.2":
+  version: 4.11.2
+  resolution: "vega-scenegraph@npm:4.11.2"
   dependencies:
     d3-path: ^3.1.0
     d3-shape: ^3.2.0
     vega-canvas: ^1.2.7
     vega-loader: ^4.5.1
     vega-scale: ^7.3.0
     vega-util: ^1.17.1
-  checksum: 6caf3e298297b918c8b6a72f019e51e2bfbaecd316e4d1c37d855ac9366d177cdbf16e9c8857c5ccde128bcd9645af7ee7dc81111bcd743d192e1a3b9a9d7185
+  checksum: fefe12c1b0393184abf0cfcae6bfcff7894a1782fe545c6c048275674359e8ec2525280aba1ddbfe6f77e710e45480fdcd9293f849a2409cde87695b04065c5b
   languageName: node
   linkType: hard
 
-"vega-selections@npm:^5.4.1":
-  version: 5.4.1
-  resolution: "vega-selections@npm:5.4.1"
+"vega-selections@npm:^5.4.2":
+  version: 5.4.2
+  resolution: "vega-selections@npm:5.4.2"
   dependencies:
-    d3-array: 3.2.2
+    d3-array: 3.2.4
     vega-expression: ^5.0.1
     vega-util: ^1.17.1
-  checksum: c594d41ec3886af94976e4dc4e152bea9b3975a22d435aa38dac2aab105851cb83fd4aa0f1e81a47f8bc0bea1677af93816331e3ed084ab3ec2e51b3544c109f
+  checksum: 4e78053ab1f8ba4338005ed424043e7d0e91c857b58ab03600a07292e3777a4244d34caa7f8c85e72b2fdd9916882dfdda2fa93c730120ce790ec9883738f2be
   languageName: node
   linkType: hard
 
 "vega-statistics@npm:^1.7.9, vega-statistics@npm:^1.8.1, vega-statistics@npm:^1.9.0, vega-statistics@npm:~1.9.0":
   version: 1.9.0
   resolution: "vega-statistics@npm:1.9.0"
   dependencies:
@@ -4067,40 +3822,40 @@
     d3-array: ^3.2.2
     d3-time: ^3.1.0
     vega-util: ^1.17.1
   checksum: 3d6a50f779be4b5e7f27bd2aae766035c29e59e03e62d2e96b94a2f759ed3104c1102c1006dd416e7b819ee501880ae7a722c2fa9aabf9efac86503c1aada14a
   languageName: node
   linkType: hard
 
-"vega-transforms@npm:~4.10.2":
-  version: 4.10.2
-  resolution: "vega-transforms@npm:4.10.2"
+"vega-transforms@npm:~4.11.1":
+  version: 4.11.1
+  resolution: "vega-transforms@npm:4.11.1"
   dependencies:
     d3-array: ^3.2.2
     vega-dataflow: ^5.7.5
     vega-statistics: ^1.8.1
     vega-time: ^2.1.1
     vega-util: ^1.17.1
-  checksum: 2dbe4c767542a5dc4dbb453fd1317b00912e47dbdb3de637259b2552497dd8039c20c795318ad57341eb0d30b69712c55a2da16dc9ad2329a68c35fb75b4fee6
+  checksum: 88ae468613a768f2a6324ad66fb4db3712228a17984316080767bcaafbd5c3c1d198bed5844a9b184d9068284a1ad7bf42f93b7b7568e2e37f98bfd43c3c6bd7
   languageName: node
   linkType: hard
 
-"vega-typings@npm:~0.24.0":
-  version: 0.24.1
-  resolution: "vega-typings@npm:0.24.1"
+"vega-typings@npm:~1.1.0":
+  version: 1.1.0
+  resolution: "vega-typings@npm:1.1.0"
   dependencies:
     "@types/geojson": 7946.0.4
     vega-event-selector: ^3.0.1
-    vega-expression: ^5.0.1
-    vega-util: ^1.17.1
-  checksum: e6b7bf88d6e505ba472c8e5e734d1914515db0e4e23ca36c5b81f7bd2bf4df6ebf519ecc1f089dcef3caae48e196d29946dc5c9fa8ee454ea31d12f111f857ae
+    vega-expression: ^5.1.0
+    vega-util: ^1.17.2
+  checksum: 59c76d1b48087b36c4386cd1bccc242afa4e1008a147d0e9966912716522c231c1d8ad35b7bc72bb3d7ccab467b786e7ba43280c75ccb54e0381c7f3aed75721
   languageName: node
   linkType: hard
 
-"vega-util@npm:^1.15.2, vega-util@npm:^1.17.1, vega-util@npm:~1.17.2":
+"vega-util@npm:^1.15.2, vega-util@npm:^1.17.1, vega-util@npm:^1.17.2, vega-util@npm:~1.17.2":
   version: 1.17.2
   resolution: "vega-util@npm:1.17.2"
   checksum: 5d681cb1a6ffda7af1b74df7c1c46a32f1d874daef54f9c9c65c7d7c7bfc4271dc6d9b1c1c7a853b14eb6e4cc8ec811b0132cd3ea25fa85259eac92e1b4f07fa
   languageName: node
   linkType: hard
 
 "vega-view-transforms@npm:~4.5.9":
@@ -4110,38 +3865,38 @@
     vega-dataflow: ^5.7.5
     vega-scenegraph: ^4.10.2
     vega-util: ^1.17.1
   checksum: aeeaf3c2f1a02b1303c16a586dbcb20f208c101d06d7e988e18ab71fb67d87be5d8ff228ebf25971535d6e41dc816168cfa68b8676e7250df07a40aefdea32a7
   languageName: node
   linkType: hard
 
-"vega-view@npm:~5.11.1":
-  version: 5.11.1
-  resolution: "vega-view@npm:5.11.1"
+"vega-view@npm:~5.12.0":
+  version: 5.12.0
+  resolution: "vega-view@npm:5.12.0"
   dependencies:
     d3-array: ^3.2.2
     d3-timer: ^3.0.1
     vega-dataflow: ^5.7.5
     vega-format: ^1.1.1
     vega-functions: ^5.13.1
     vega-runtime: ^6.1.4
     vega-scenegraph: ^4.10.2
     vega-util: ^1.17.1
-  checksum: 82ddc74593b3a359d0b3458bc06573673ff9bf13f84020cb36fb4676c5d7f547e9650eb6faaa76799fbcedd27bcd266603dbd08c420e2d2229cc6b9f48a4a66d
+  checksum: 8ccbff58ad132dc51647afe1ca31759c8f2782e00124e9f3cb5c16a17c27daca10e354e7aa8517f275182ee36ec3e5be8913ab4eb91f66d2f5a17a385400e7ab
   languageName: node
   linkType: hard
 
-"vega-voronoi@npm:~4.2.1":
-  version: 4.2.1
-  resolution: "vega-voronoi@npm:4.2.1"
+"vega-voronoi@npm:~4.2.2":
+  version: 4.2.2
+  resolution: "vega-voronoi@npm:4.2.2"
   dependencies:
     d3-delaunay: ^6.0.2
     vega-dataflow: ^5.7.5
     vega-util: ^1.17.1
-  checksum: f618174ad5f451c507a80e373288bb2c0da7a8a908d62f885bc77b354c4334504ae2d1042742f68ad419ade7b548aeca9ca1042ae5541bebd7f5297afc23bb35
+  checksum: 719121a675ae021a30854e6c0fce39adc2a59478d7a1088b554140bf5a4a8e382186ad0762a21a969fa49e5e58ff757a4ec398fb77a834fcd2863d6862a1b92d
   languageName: node
   linkType: hard
 
 "vega-wordcloud@npm:~4.1.4":
   version: 4.1.4
   resolution: "vega-wordcloud@npm:4.1.4"
   dependencies:
@@ -4151,76 +3906,76 @@
     vega-statistics: ^1.8.1
     vega-util: ^1.17.1
   checksum: 34d1882651d3a2f34ce40a6eaeed700de126f627cdf041ec2bcc7ada46d7b4b68a38a2974236eec87ee876d9abd095af7ab17e7698b0e2fbc831460767969d7a
   languageName: node
   linkType: hard
 
 "vega@npm:^5.20.0":
-  version: 5.25.0
-  resolution: "vega@npm:5.25.0"
+  version: 5.27.0
+  resolution: "vega@npm:5.27.0"
   dependencies:
     vega-crossfilter: ~4.1.1
     vega-dataflow: ~5.7.5
     vega-encode: ~4.9.2
     vega-event-selector: ~3.0.1
     vega-expression: ~5.1.0
     vega-force: ~4.2.0
     vega-format: ~1.1.1
-    vega-functions: ~5.13.2
+    vega-functions: ~5.14.0
     vega-geo: ~4.4.1
     vega-hierarchy: ~4.1.1
     vega-label: ~1.2.1
     vega-loader: ~4.5.1
-    vega-parser: ~6.2.0
+    vega-parser: ~6.2.1
     vega-projection: ~1.6.0
     vega-regression: ~1.2.0
     vega-runtime: ~6.1.4
-    vega-scale: ~7.3.0
-    vega-scenegraph: ~4.10.2
+    vega-scale: ~7.3.1
+    vega-scenegraph: ~4.11.2
     vega-statistics: ~1.9.0
     vega-time: ~2.1.1
-    vega-transforms: ~4.10.2
-    vega-typings: ~0.24.0
+    vega-transforms: ~4.11.1
+    vega-typings: ~1.1.0
     vega-util: ~1.17.2
-    vega-view: ~5.11.1
+    vega-view: ~5.12.0
     vega-view-transforms: ~4.5.9
-    vega-voronoi: ~4.2.1
+    vega-voronoi: ~4.2.2
     vega-wordcloud: ~4.1.4
-  checksum: ddc7b1f2a70c72b842e111d32bdd8ff050992a50e385e8ddc6e35c02e7c481a652383c81c547b7ebfd31cda04ab9f9acf0a8cc47c6bd19b91765b254aac30d24
+  checksum: aafecd6fc30db8f254b534084e293fbf93b309ae6a8cdae56afe2ccf87ecd03ecab332e59f14aa02748ded23d5ee3eb93bea463e6473f0f7d8a469659d22ddf9
   languageName: node
   linkType: hard
 
-"vscode-jsonrpc@npm:8.1.0, vscode-jsonrpc@npm:^8.0.2":
-  version: 8.1.0
-  resolution: "vscode-jsonrpc@npm:8.1.0"
-  checksum: 8980037cc0014802e6ac1e5dfcff9a65e8292727096dfd23c92d2039c0c45de74a00d6ee06938cf1a671286dd8258a5f418cf048c26ad0fcb0c44f96c9e0f278
+"vscode-jsonrpc@npm:8.2.0, vscode-jsonrpc@npm:^8.0.2":
+  version: 8.2.0
+  resolution: "vscode-jsonrpc@npm:8.2.0"
+  checksum: f302a01e59272adc1ae6494581fa31c15499f9278df76366e3b97b2236c7c53ebfc71efbace9041cfd2caa7f91675b9e56f2407871a1b3c7f760a2e2ee61484a
   languageName: node
   linkType: hard
 
 "vscode-jsonrpc@npm:^6.0.0":
   version: 6.0.0
   resolution: "vscode-jsonrpc@npm:6.0.0"
   checksum: 3a67a56f287e8c449f2d9752eedf91e704dc7b9a326f47fb56ac07667631deb45ca52192e9bccb2ab108764e48409d70fa64b930d46fc3822f75270b111c5f53
   languageName: node
   linkType: hard
 
 "vscode-languageserver-protocol@npm:^3.17.0":
-  version: 3.17.3
-  resolution: "vscode-languageserver-protocol@npm:3.17.3"
+  version: 3.17.5
+  resolution: "vscode-languageserver-protocol@npm:3.17.5"
   dependencies:
-    vscode-jsonrpc: 8.1.0
-    vscode-languageserver-types: 3.17.3
-  checksum: ffea508b2efd7f4853f1cef5e5eac58672f0ae71a9ec275ad37a4a2a24cdc3ff023f941e759951aee01c79da3f3279f10e034f19d875f081eb387181241bd836
+    vscode-jsonrpc: 8.2.0
+    vscode-languageserver-types: 3.17.5
+  checksum: dfb42d276df5dfea728267885b99872ecff62f6c20448b8539fae71bb196b420f5351c5aca7c1047bf8fb1f89fa94a961dce2bc5bf7e726198f4be0bb86a1e71
   languageName: node
   linkType: hard
 
-"vscode-languageserver-types@npm:3.17.3":
-  version: 3.17.3
-  resolution: "vscode-languageserver-types@npm:3.17.3"
-  checksum: fbc8221297261f659a6482875ff2a419dc9d55965dc53745797da569ff9f819cd832e6f2699017baadd946548bbfe212e3f6971f3d960f12dc0ee9c629dacc07
+"vscode-languageserver-types@npm:3.17.5":
+  version: 3.17.5
+  resolution: "vscode-languageserver-types@npm:3.17.5"
+  checksum: 79b420e7576398d396579ca3a461c9ed70e78db4403cd28bbdf4d3ed2b66a2b4114031172e51fad49f0baa60a2180132d7cb2ea35aa3157d7af3c325528210ac
   languageName: node
   linkType: hard
 
 "vscode-ws-jsonrpc@npm:~1.0.2":
   version: 1.0.2
   resolution: "vscode-ws-jsonrpc@npm:1.0.2"
   dependencies:
@@ -4249,31 +4004,33 @@
   dependencies:
     tr46: ~0.0.3
     webidl-conversions: ^3.0.0
   checksum: b8daed4ad3356cc4899048a15b2c143a9aed0dfae1f611ebd55073310c7b910f522ad75d727346ad64203d7e6c79ef25eafd465f4d12775ca44b90fa82ed9e2c
   languageName: node
   linkType: hard
 
-"which@npm:^2.0.1, which@npm:^2.0.2":
+"which@npm:^2.0.1":
   version: 2.0.2
   resolution: "which@npm:2.0.2"
   dependencies:
     isexe: ^2.0.0
   bin:
     node-which: ./bin/node-which
   checksum: 1a5c563d3c1b52d5f893c8b61afe11abc3bab4afac492e8da5bde69d550de701cf9806235f20a47b5c8fa8a1d6a9135841de2596535e998027a54589000e66d1
   languageName: node
   linkType: hard
 
-"wide-align@npm:^1.1.5":
-  version: 1.1.5
-  resolution: "wide-align@npm:1.1.5"
+"which@npm:^4.0.0":
+  version: 4.0.0
+  resolution: "which@npm:4.0.0"
   dependencies:
-    string-width: ^1.0.2 || 2 || 3 || 4
-  checksum: d5fc37cd561f9daee3c80e03b92ed3e84d80dde3365a8767263d03dacfc8fa06b065ffe1df00d8c2a09f731482fcacae745abfbb478d4af36d0a891fad4834d3
+    isexe: ^3.1.1
+  bin:
+    node-which: bin/which.js
+  checksum: f17e84c042592c21e23c8195108cff18c64050b9efb8459589116999ea9da6dd1509e6a1bac3aeebefd137be00fabbb61b5c2bc0aa0f8526f32b58ee2f545651
   languageName: node
   linkType: hard
 
 "wrap-ansi-cjs@npm:wrap-ansi@^7.0.0, wrap-ansi@npm:^7.0.0":
   version: 7.0.0
   resolution: "wrap-ansi@npm:7.0.0"
   dependencies:
@@ -4291,42 +4048,37 @@
     ansi-styles: ^6.1.0
     string-width: ^5.0.1
     strip-ansi: ^7.0.1
   checksum: 371733296dc2d616900ce15a0049dca0ef67597d6394c57347ba334393599e800bab03c41d4d45221b6bc967b8c453ec3ae4749eff3894202d16800fdfe0e238
   languageName: node
   linkType: hard
 
-"wrappy@npm:1":
-  version: 1.0.2
-  resolution: "wrappy@npm:1.0.2"
-  checksum: 159da4805f7e84a3d003d8841557196034155008f817172d4e986bd591f74aa82aa7db55929a54222309e01079a65a92a9e6414da5a6aa4b01ee44a511ac3ee5
-  languageName: node
-  linkType: hard
-
 "ws@npm:^8.11.0":
-  version: 8.13.0
-  resolution: "ws@npm:8.13.0"
+  version: 8.16.0
+  resolution: "ws@npm:8.16.0"
   peerDependencies:
     bufferutil: ^4.0.1
     utf-8-validate: ">=5.0.2"
   peerDependenciesMeta:
     bufferutil:
       optional: true
     utf-8-validate:
       optional: true
-  checksum: 53e991bbf928faf5dc6efac9b8eb9ab6497c69feeb94f963d648b7a3530a720b19ec2e0ec037344257e05a4f35bd9ad04d9de6f289615ffb133282031b18c61c
+  checksum: feb3eecd2bae82fa8a8beef800290ce437d8b8063bdc69712725f21aef77c49cb2ff45c6e5e7fce622248f9c7abaee506bae0a9064067ffd6935460c7357321b
   languageName: node
   linkType: hard
 
 "y-protocols@npm:^1.0.5":
-  version: 1.0.5
-  resolution: "y-protocols@npm:1.0.5"
+  version: 1.0.6
+  resolution: "y-protocols@npm:1.0.6"
   dependencies:
-    lib0: ^0.2.42
-  checksum: d19404a4ebafcf3761c28b881abe8c32ab6e457db0e5ffc7dbb749cbc2c3bb98e003a43f3e8eba7f245b2698c76f2c4cdd1c2db869f8ec0c6ef94736d9a88652
+    lib0: ^0.2.85
+  peerDependencies:
+    yjs: ^13.0.0
+  checksum: 4b57c8811befcf2e45c3d47830005f8a33e626c734f78a42fe8a4fa3caad2233ba85a7c8bceefbd52ffc40130d3f3faee664fd0d1c324ff1fa8817a056ccdc1c
   languageName: node
   linkType: hard
 
 "y18n@npm:^5.0.5":
   version: 5.0.8
   resolution: "y18n@npm:5.0.8"
   checksum: 54f0fb95621ee60898a38c572c515659e51cc9d9f787fb109cef6fde4befbe1c4602dc999d30110feee37456ad0f1660fa2edcfde6a9a740f86a290999550d30
@@ -4359,14 +4111,14 @@
     y18n: ^5.0.5
     yargs-parser: ^21.1.1
   checksum: 73b572e863aa4a8cbef323dd911d79d193b772defd5a51aab0aca2d446655216f5002c42c5306033968193bdbf892a7a4c110b0d77954a7fdf563e653967b56a
   languageName: node
   linkType: hard
 
 "yjs@npm:^13.5.40":
-  version: 13.6.6
-  resolution: "yjs@npm:13.6.6"
+  version: 13.6.11
+  resolution: "yjs@npm:13.6.11"
   dependencies:
-    lib0: ^0.2.74
-  checksum: c69cb9a084aa433e813f6d0a191ebad5800a9a7098f7c6715952e4f8e5fc23270e3b8d7d747e1b0d0f1adca5f6efe01019654389eddb3977006814c4e2ff7ce6
+    lib0: ^0.2.86
+  checksum: fb2993b12c6d13caf52d41af747991fa0be0a7e560ad2de84a736b4b7fa085d8327ff7254238840c407fa0671ca8c8e5917baea32f6d6686923c602134045b94
   languageName: node
   linkType: hard
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/.gitignore` & `jupyterlab_unianalytics_telemetry-4.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/LICENSE` & `jupyterlab_unianalytics_telemetry-4.0.9/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Raphael Marietan
+Copyright (c) 2024, Raphael Marietan
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/README.md` & `jupyterlab_unianalytics_telemetry-4.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -22,31 +22,49 @@
 
 To remove the extension, execute:
 
 ```bash
 pip uninstall jupyterlab-unianalytics-telemetry
 ```
 
+## Troubleshoot
+
+If you are seeing the frontend extension, but it is not working, check
+that the server extension is enabled:
+
+```bash
+jupyter server extension list
+```
+
+If the server extension is installed and enabled, but you are not seeing
+the frontend extension, check the frontend extension is installed:
+
+```bash
+jupyter labextension list
+```
+
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
-# Change directory to the extension directory
+# Change directory to the jupyterlab_unianalytics_telemetry directory
 # Install package in development mode
-pip install -e "."
+pip install -e ".[test]"
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
+# Server extension must be manually installed in develop mode
+jupyter server extension enable jupyterlab_unianalytics_telemetry
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
@@ -63,37 +81,57 @@
 ```bash
 jupyter lab build --minimize=False
 ```
 
 ### Development uninstall
 
 ```bash
+# Server extension must be manually disabled in develop mode
+jupyter server extension disable jupyterlab_unianalytics_telemetry
 pip uninstall jupyterlab_unianalytics_telemetry
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `jupyterlab_unianalytics_telemetry` within that folder.
 
 ### Testing the extension
 
+#### Server tests
+
+This extension is using [Pytest](https://docs.pytest.org/) for Python code testing.
+
+Install test dependencies (needed only once):
+
+```sh
+pip install -e ".[test]"
+# Each time you install the Python package, you need to restore the front-end extension link
+jupyter labextension develop . --overwrite
+```
+
+To execute them, run:
+
+```sh
+pytest -vv -r ap --cov jupyterlab_unianalytics_telemetry
+```
+
 #### Frontend tests
 
 This extension is using [Jest](https://jestjs.io/) for JavaScript code testing.
 
 To execute them, execute:
 
 ```sh
 jlpm
 jlpm test
 ```
 
 #### Integration tests
 
-This extension uses [Playwright](https://playwright.dev/docs/intro/) for the integration tests (aka user level tests).
+This extension uses [Playwright](https://playwright.dev/docs/intro) for the integration tests (aka user level tests).
 More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
 
 More information are provided within the [ui-tests](./ui-tests/README.md) README.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/pyproject.toml` & `jupyterlab_unianalytics_telemetry-4.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling>=1.5.0", "jupyterlab>=3.5.3,<5.0.0a0", "hatch-nodejs-version"]
+requires = ["hatchling>=1.5.0", "jupyterlab>=3.5,<5", "hatch-nodejs-version>=0.3.2"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyterlab_unianalytics_telemetry"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
@@ -16,32 +16,44 @@
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
+    "jupyter_server>=1.12,<3"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
+[project.optional-dependencies]
+test = [
+    "coverage",
+    "pytest",
+    "pytest-asyncio",
+    "pytest-cov",
+    "pytest-jupyter[server]>=0.6.0"
+]
+
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
 fields = ["description", "authors", "urls"]
 
 [tool.hatch.build.targets.sdist]
 artifacts = ["jupyterlab_unianalytics_telemetry/labextension"]
 exclude = [".github", "binder"]
 
 [tool.hatch.build.targets.wheel.shared-data]
 "jupyterlab_unianalytics_telemetry/labextension" = "share/jupyter/labextensions/jupyterlab_unianalytics_telemetry"
 "install.json" = "share/jupyter/labextensions/jupyterlab_unianalytics_telemetry/install.json"
+"jupyter-config/server-config" = "etc/jupyter/jupyter_server_config.d"
 
 [tool.hatch.build.hooks.version]
 path = "jupyterlab_unianalytics_telemetry/_version.py"
 
 [tool.hatch.build.hooks.jupyter-builder]
 dependencies = ["hatch-jupyter-builder>=0.5"]
 build-function = "hatch_jupyter_builder.npm_builder"
```

### Comparing `jupyterlab_unianalytics_telemetry-4.0.8/PKG-INFO` & `jupyterlab_unianalytics_telemetry-4.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: jupyterlab_unianalytics_telemetry
-Version: 4.0.8
-Summary: A JupyterLab extension to send notebook execution and activity to a self-hosted backend.
+Version: 4.0.9
+Summary: A JupyterLab extension to send notebook interaction data to a backend.
 Project-URL: Homepage, https://github.com/chili-epfl/jupyter-dashboard-send-extension
 Project-URL: Bug Tracker, https://github.com/chili-epfl/jupyter-dashboard-send-extension/issues
 Project-URL: Repository, https://github.com/chili-epfl/jupyter-dashboard-send-extension.git
-Author-email: Raphael Marietan <me@test.com>
+Author-email: Raphael Marietan <raphael.marietan@hotmail.com>
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Raphael Marietan
+        Copyright (c) 2024, Raphael Marietan
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -44,15 +44,23 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
+Requires-Dist: jupyter-server<3,>=1.12
+Provides-Extra: test
+Requires-Dist: coverage; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-asyncio; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-jupyter[server]>=0.6.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Unianalytics Telemetry JupyterLab Extension
 
 [![Binder Badge](https://github.com/chili-epfl/jupyter-dashboard-send-extension/actions/workflows/binder-on-pr.yml/badge.svg)](https://github.com/chili-epfl/jupyter-dashboard-send-extension/actions/workflows/binder-on-pr.yml)
 [![Build](https://github.com/chili-epfl/jupyter-dashboard-send-extension/actions/workflows/build.yml/badge.svg)](https://github.com/chili-epfl/jupyter-dashboard-send-extension/actions/workflows/build.yml)
 [![Check Release](https://github.com/chili-epfl/jupyter-dashboard-send-extension/actions/workflows/check-release.yml/badge.svg)](https://github.com/chili-epfl/jupyter-dashboard-send-extension/actions/workflows/check-release.yml)
@@ -75,31 +83,49 @@
 
 To remove the extension, execute:
 
 ```bash
 pip uninstall jupyterlab-unianalytics-telemetry
 ```
 
+## Troubleshoot
+
+If you are seeing the frontend extension, but it is not working, check
+that the server extension is enabled:
+
+```bash
+jupyter server extension list
+```
+
+If the server extension is installed and enabled, but you are not seeing
+the frontend extension, check the frontend extension is installed:
+
+```bash
+jupyter labextension list
+```
+
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
-# Change directory to the extension directory
+# Change directory to the jupyterlab_unianalytics_telemetry directory
 # Install package in development mode
-pip install -e "."
+pip install -e ".[test]"
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
+# Server extension must be manually installed in develop mode
+jupyter server extension enable jupyterlab_unianalytics_telemetry
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
@@ -116,37 +142,57 @@
 ```bash
 jupyter lab build --minimize=False
 ```
 
 ### Development uninstall
 
 ```bash
+# Server extension must be manually disabled in develop mode
+jupyter server extension disable jupyterlab_unianalytics_telemetry
 pip uninstall jupyterlab_unianalytics_telemetry
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `jupyterlab_unianalytics_telemetry` within that folder.
 
 ### Testing the extension
 
+#### Server tests
+
+This extension is using [Pytest](https://docs.pytest.org/) for Python code testing.
+
+Install test dependencies (needed only once):
+
+```sh
+pip install -e ".[test]"
+# Each time you install the Python package, you need to restore the front-end extension link
+jupyter labextension develop . --overwrite
+```
+
+To execute them, run:
+
+```sh
+pytest -vv -r ap --cov jupyterlab_unianalytics_telemetry
+```
+
 #### Frontend tests
 
 This extension is using [Jest](https://jestjs.io/) for JavaScript code testing.
 
 To execute them, execute:
 
 ```sh
 jlpm
 jlpm test
 ```
 
 #### Integration tests
 
-This extension uses [Playwright](https://playwright.dev/docs/intro/) for the integration tests (aka user level tests).
+This extension uses [Playwright](https://playwright.dev/docs/intro) for the integration tests (aka user level tests).
 More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
 
 More information are provided within the [ui-tests](./ui-tests/README.md) README.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
```

