# Comparing `tmp/aiida_workgraph-0.2.5.tar.gz` & `tmp/aiida_workgraph-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_workgraph-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_workgraph-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_workgraph-0.2.5.tar` & `aiida_workgraph-0.2.6.tar`

### file list

```diff
@@ -1,123 +1,126 @@
--rw-r--r--   0        0        0     1066 2023-12-11 16:36:18.395013 aiida_workgraph-0.2.5/LICENSE
--rw-r--r--   0        0        0     5318 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.5/README.md
--rw-r--r--   0        0        0      175 2024-05-20 19:34:02.324876 aiida_workgraph-0.2.5/aiida_workgraph/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/calculations/__init__.py
--rw-r--r--   0        0        0     2468 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/calculations/general_data.py
--rw-r--r--   0        0        0     7811 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/calculations/python.py
--rw-r--r--   0        0        0     1391 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/calculations/python_parser.py
--rw-r--r--   0        0        0      279 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/cli/__init__.py
--rw-r--r--   0        0        0    12112 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/cli/cmd_graph.py
--rw-r--r--   0        0        0     1937 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/cli/cmd_web.py
--rw-r--r--   0        0        0      714 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/cli/cmd_workgraph.py
--rw-r--r--   0        0        0     6599 2024-05-18 09:24:02.309034 aiida_workgraph-0.2.5/aiida_workgraph/cli/query_workgraph.py
--rw-r--r--   0        0        0     2679 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/collection.py
--rw-r--r--   0        0        0    18544 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/decorator.py
--rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/engine/__init__.py
--rw-r--r--   0        0        0    49863 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/engine/workgraph.py
--rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/executors/__init__.py
--rw-r--r--   0        0        0      897 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.5/aiida_workgraph/executors/builtin.py
--rw-r--r--   0        0        0      740 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.5/aiida_workgraph/executors/qe.py
--rw-r--r--   0        0        0      768 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.5/aiida_workgraph/executors/test.py
--rw-r--r--   0        0        0     4151 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.5/aiida_workgraph/node.py
--rw-r--r--   0        0        0      847 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.5/aiida_workgraph/nodes/__init__.py
--rw-r--r--   0        0        0     3957 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.5/aiida_workgraph/nodes/builtin.py
--rw-r--r--   0        0        0     2168 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.5/aiida_workgraph/nodes/qe.py
--rw-r--r--   0        0        0     7233 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.5/aiida_workgraph/nodes/test.py
--rw-r--r--   0        0        0     1214 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/orm/worktree.py
--rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/properties/__init__.py
--rw-r--r--   0        0        0    10647 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.5/aiida_workgraph/properties/built_in.py
--rw-r--r--   0        0        0     2131 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/property.py
--rw-r--r--   0        0        0     1386 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/socket.py
--rw-r--r--   0        0        0      111 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/sockets/__init__.py
--rw-r--r--   0        0        0     3760 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.5/aiida_workgraph/sockets/built_in.py
--rw-r--r--   0        0        0     7824 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/utils/__init__.py
--rw-r--r--   0        0        0     6132 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/utils/analysis.py
--rw-r--r--   0        0        0     1754 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.5/aiida_workgraph/utils/graph.py
--rw-r--r--   0        0        0      763 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/README.md
--rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/__init__.py
--rw-r--r--   0        0        0     2395 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/api.py
--rw-r--r--   0        0        0     3638 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/daemon.py
--rw-r--r--   0        0        0     2208 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/datanode.py
--rw-r--r--   0        0        0     6618 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/utils.py
--rw-r--r--   0        0        0     5130 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/workgraph.py
--rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/backend/main.py
--rw-r--r--   0        0        0      310 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/.gitignore
--rw-r--r--   0        0        0       62 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/.rete-patch
--rw-r--r--   0        0        0     2136 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/README.md
--rw-r--r--   0        0        0      517 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/favicon.ico
--rw-r--r--   0        0        0      654 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/index.html
--rw-r--r--   0        0        0      306 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/manifest.json
--rw-r--r--   0        0        0       67 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/robots.txt
--rw-r--r--   0        0        0    18033 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css
--rw-r--r--   0        0        0    46655 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map
--rw-r--r--   0        0        0     4518 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js
--rw-r--r--   0        0        0    10597 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map
--rw-r--r--   0        0        0  3614868 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js
--rw-r--r--   0        0        0     3456 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt
--rw-r--r--   0        0        0 13934230 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map
--rw-r--r--   0        0        0  1408324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/package-lock.json
--rw-r--r--   0        0        0     2249 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/package.json
--rw-r--r--   0        0        0     3870 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/public/favicon.ico
--rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/public/index.html
--rw-r--r--   0        0        0      306 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/public/manifest.json
--rw-r--r--   0        0        0       67 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/public/robots.txt
--rw-r--r--   0        0        0     2443 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/App.css
--rw-r--r--   0        0        0     1143 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/App.js
--rw-r--r--   0        0        0      273 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/App.test.tsx
--rw-r--r--   0        0        0     1675 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/AtomsItem.js
--rw-r--r--   0        0        0       94 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Data.js
--rw-r--r--   0        0        0      106 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/DataNode.js
--rw-r--r--   0        0        0      505 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/DataNodeItem.css
--rw-r--r--   0        0        0     1458 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx
--rw-r--r--   0        0        0     5593 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/DataNodeTable.js
--rw-r--r--   0        0        0      116 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Home.js
--rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Layout.css
--rw-r--r--   0        0        0     1067 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Layout.js
--rw-r--r--   0        0        0     5792 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/NodeDetails.js
--rw-r--r--   0        0        0     2784 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Settings.js
--rw-r--r--   0        0        0     1025 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js
--rw-r--r--   0        0        0     2631 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js
--rw-r--r--   0        0        0     1129 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js
--rw-r--r--   0        0        0     8796 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx
--rw-r--r--   0        0        0     1064 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts
--rw-r--r--   0        0        0      837 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js
--rw-r--r--   0        0        0     3434 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js
--rw-r--r--   0        0        0      990 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css
--rw-r--r--   0        0        0     7518 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js
--rw-r--r--   0        0        0      366 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/index.css
--rw-r--r--   0        0        0      554 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/index.tsx
--rw-r--r--   0        0        0     6007 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/logo.svg
--rw-r--r--   0        0        0       40 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      425 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/reportWebVitals.ts
--rw-r--r--   0        0        0      160 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete.css
--rw-r--r--   0        0        0     2787 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization.ts
--rw-r--r--   0        0        0      813 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx
--rw-r--r--   0        0        0     4981 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx
--rw-r--r--   0        0        0      566 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx
--rw-r--r--   0        0        0      540 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx
--rw-r--r--   0        0        0      602 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/background.css
--rw-r--r--   0        0        0      378 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/custom-background.ts
--rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/vars.ts
--rw-r--r--   0        0        0     4864 2024-05-04 20:38:47.853168 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/default.ts
--rw-r--r--   0        0        0      603 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/index.ts
--rw-r--r--   0        0        0      241 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/setupTests.ts
--rw-r--r--   0        0        0      535 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/tsconfig.json
--rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/widget/.gitignore
--rw-r--r--   0        0        0      488 2024-04-13 07:05:41.907170 aiida_workgraph-0.2.5/aiida_workgraph/widget/.ipynb_checkpoints/example-checkpoint.ipynb
--rw-r--r--   0        0        0      552 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/widget/README.md
--rw-r--r--   0        0        0       71 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/widget/__init__.py
--rw-r--r--   0        0        0     7122 2024-05-03 14:17:12.929117 aiida_workgraph-0.2.5/aiida_workgraph/widget/js/default_rete.ts
--rw-r--r--   0        0        0      565 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.5/aiida_workgraph/widget/js/widget.css
--rw-r--r--   0        0        0     5905 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.5/aiida_workgraph/widget/js/widget.tsx
--rw-r--r--   0        0        0   148687 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.5/aiida_workgraph/widget/package-lock.json
--rw-r--r--   0        0        0      851 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.5/aiida_workgraph/widget/package.json
--rw-r--r--   0        0        0      765 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/widget/pyproject.toml
--rw-r--r--   0        0        0     1981 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/__init__.py
--rw-r--r--   0        0        0      429 2024-05-20 19:36:16.932122 aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/static/widget.css
--rw-r--r--   0        0        0  1796776 2024-05-20 19:36:16.932122 aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/static/widget.js
--rw-r--r--   0        0        0      897 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/utils.py
--rw-r--r--   0        0        0      453 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.5/aiida_workgraph/widget/tsconfig.json
--rw-r--r--   0        0        0    14913 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/aiida_workgraph/workgraph.py
--rw-r--r--   0        0        0     2853 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     7358 1970-01-01 00:00:00.000000 aiida_workgraph-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-12-11 16:36:18.395013 aiida_workgraph-0.2.6/LICENSE
+-rw-r--r--   0        0        0     5318 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.6/README.md
+-rw-r--r--   0        0        0      175 2024-05-23 10:18:29.324006 aiida_workgraph-0.2.6/aiida_workgraph/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.6/aiida_workgraph/calculations/__init__.py
+-rw-r--r--   0        0        0     8238 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/calculations/python.py
+-rw-r--r--   0        0        0     2114 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/calculations/python_parser.py
+-rw-r--r--   0        0        0      279 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/cli/__init__.py
+-rw-r--r--   0        0        0    12112 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/cli/cmd_graph.py
+-rw-r--r--   0        0        0     1937 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/cli/cmd_web.py
+-rw-r--r--   0        0        0      714 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/cli/cmd_workgraph.py
+-rw-r--r--   0        0        0     6599 2024-05-18 09:24:02.309034 aiida_workgraph-0.2.6/aiida_workgraph/cli/query_workgraph.py
+-rw-r--r--   0        0        0     2829 2024-05-22 09:59:58.253538 aiida_workgraph-0.2.6/aiida_workgraph/collection.py
+-rw-r--r--   0        0        0    18855 2024-05-22 09:59:58.253538 aiida_workgraph-0.2.6/aiida_workgraph/decorator.py
+-rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/engine/__init__.py
+-rw-r--r--   0        0        0    50042 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/engine/workgraph.py
+-rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/executors/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.6/aiida_workgraph/executors/builtin.py
+-rw-r--r--   0        0        0      740 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.6/aiida_workgraph/executors/qe.py
+-rw-r--r--   0        0        0      768 2024-05-07 20:56:57.572283 aiida_workgraph-0.2.6/aiida_workgraph/executors/test.py
+-rw-r--r--   0        0        0     4151 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.6/aiida_workgraph/node.py
+-rw-r--r--   0        0        0      847 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.6/aiida_workgraph/nodes/__init__.py
+-rw-r--r--   0        0        0     3957 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.6/aiida_workgraph/nodes/builtin.py
+-rw-r--r--   0        0        0     2168 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.6/aiida_workgraph/nodes/qe.py
+-rw-r--r--   0        0        0     7233 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.6/aiida_workgraph/nodes/test.py
+-rw-r--r--   0        0        0      141 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/orm/__init__.py
+-rw-r--r--   0        0        0     4353 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/orm/atoms.py
+-rw-r--r--   0        0        0     2619 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/orm/general_data.py
+-rw-r--r--   0        0        0     1715 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/aiida_workgraph/orm/serializer.py
+-rw-r--r--   0        0        0     1214 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/orm/worktree.py
+-rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/properties/__init__.py
+-rw-r--r--   0        0        0    10647 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.6/aiida_workgraph/properties/built_in.py
+-rw-r--r--   0        0        0     2131 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/property.py
+-rw-r--r--   0        0        0     1386 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/socket.py
+-rw-r--r--   0        0        0      111 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/sockets/__init__.py
+-rw-r--r--   0        0        0     3760 2024-05-15 13:45:10.407702 aiida_workgraph-0.2.6/aiida_workgraph/sockets/built_in.py
+-rw-r--r--   0        0        0     8697 2024-05-22 09:59:58.253538 aiida_workgraph-0.2.6/aiida_workgraph/utils/__init__.py
+-rw-r--r--   0        0        0     6132 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/utils/analysis.py
+-rw-r--r--   0        0        0     1754 2024-05-14 07:23:38.731767 aiida_workgraph-0.2.6/aiida_workgraph/utils/graph.py
+-rw-r--r--   0        0        0      763 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/__init__.py
+-rw-r--r--   0        0        0     2395 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/api.py
+-rw-r--r--   0        0        0     3638 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/daemon.py
+-rw-r--r--   0        0        0     2208 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/datanode.py
+-rw-r--r--   0        0        0     6618 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/utils.py
+-rw-r--r--   0        0        0     5130 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/workgraph.py
+-rw-r--r--   0        0        0      115 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/backend/main.py
+-rw-r--r--   0        0        0      310 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/.gitignore
+-rw-r--r--   0        0        0       62 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/.rete-patch
+-rw-r--r--   0        0        0     2136 2024-04-22 15:35:28.433776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/README.md
+-rw-r--r--   0        0        0      517 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/favicon.ico
+-rw-r--r--   0        0        0      654 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/index.html
+-rw-r--r--   0        0        0      306 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-20 19:34:56.150973 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/robots.txt
+-rw-r--r--   0        0        0    18033 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css
+-rw-r--r--   0        0        0    46655 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map
+-rw-r--r--   0        0        0     4518 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js
+-rw-r--r--   0        0        0    10597 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map
+-rw-r--r--   0        0        0  3614868 2024-05-20 19:35:26.142370 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js
+-rw-r--r--   0        0        0     3456 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt
+-rw-r--r--   0        0        0 13934230 2024-05-20 19:35:26.170373 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map
+-rw-r--r--   0        0        0  1408324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/package-lock.json
+-rw-r--r--   0        0        0     2249 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/package.json
+-rw-r--r--   0        0        0     3870 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/public/favicon.ico
+-rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/public/index.html
+-rw-r--r--   0        0        0      306 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/public/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/public/robots.txt
+-rw-r--r--   0        0        0     2443 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/App.css
+-rw-r--r--   0        0        0     1143 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/App.js
+-rw-r--r--   0        0        0      273 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/App.test.tsx
+-rw-r--r--   0        0        0     1675 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/AtomsItem.js
+-rw-r--r--   0        0        0       94 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Data.js
+-rw-r--r--   0        0        0      106 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/DataNode.js
+-rw-r--r--   0        0        0      505 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/DataNodeItem.css
+-rw-r--r--   0        0        0     1458 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx
+-rw-r--r--   0        0        0     5593 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/DataNodeTable.js
+-rw-r--r--   0        0        0      116 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Home.js
+-rw-r--r--   0        0        0     1324 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Layout.css
+-rw-r--r--   0        0        0     1067 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Layout.js
+-rw-r--r--   0        0        0     5792 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/NodeDetails.js
+-rw-r--r--   0        0        0     2784 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Settings.js
+-rw-r--r--   0        0        0     1025 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js
+-rw-r--r--   0        0        0     2631 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js
+-rw-r--r--   0        0        0     1129 2024-04-22 15:35:28.437776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js
+-rw-r--r--   0        0        0     8796 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx
+-rw-r--r--   0        0        0     1064 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts
+-rw-r--r--   0        0        0      837 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js
+-rw-r--r--   0        0        0     3434 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js
+-rw-r--r--   0        0        0      990 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css
+-rw-r--r--   0        0        0     7518 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js
+-rw-r--r--   0        0        0      366 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/index.css
+-rw-r--r--   0        0        0      554 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/index.tsx
+-rw-r--r--   0        0        0     6007 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/logo.svg
+-rw-r--r--   0        0        0       40 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      425 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/reportWebVitals.ts
+-rw-r--r--   0        0        0      160 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete.css
+-rw-r--r--   0        0        0     2787 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization.ts
+-rw-r--r--   0        0        0      813 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx
+-rw-r--r--   0        0        0     4981 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx
+-rw-r--r--   0        0        0      566 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx
+-rw-r--r--   0        0        0      540 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx
+-rw-r--r--   0        0        0      602 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/background.css
+-rw-r--r--   0        0        0      378 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/custom-background.ts
+-rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/vars.ts
+-rw-r--r--   0        0        0     4864 2024-05-04 20:38:47.853168 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/default.ts
+-rw-r--r--   0        0        0      603 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/index.ts
+-rw-r--r--   0        0        0      241 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/setupTests.ts
+-rw-r--r--   0        0        0      535 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/tsconfig.json
+-rw-r--r--   0        0        0       94 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/widget/.gitignore
+-rw-r--r--   0        0        0      488 2024-04-13 07:05:41.907170 aiida_workgraph-0.2.6/aiida_workgraph/widget/.ipynb_checkpoints/example-checkpoint.ipynb
+-rw-r--r--   0        0        0      552 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/widget/README.md
+-rw-r--r--   0        0        0       71 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/widget/__init__.py
+-rw-r--r--   0        0        0     7122 2024-05-03 14:17:12.929117 aiida_workgraph-0.2.6/aiida_workgraph/widget/js/default_rete.ts
+-rw-r--r--   0        0        0      565 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.6/aiida_workgraph/widget/js/widget.css
+-rw-r--r--   0        0        0     5905 2024-04-22 20:35:00.919099 aiida_workgraph-0.2.6/aiida_workgraph/widget/js/widget.tsx
+-rw-r--r--   0        0        0   148687 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.6/aiida_workgraph/widget/package-lock.json
+-rw-r--r--   0        0        0      851 2024-04-22 20:35:00.923099 aiida_workgraph-0.2.6/aiida_workgraph/widget/package.json
+-rw-r--r--   0        0        0      765 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/widget/pyproject.toml
+-rw-r--r--   0        0        0     1981 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-20 19:36:16.932122 aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/static/widget.css
+-rw-r--r--   0        0        0  1796776 2024-05-20 19:36:16.932122 aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/static/widget.js
+-rw-r--r--   0        0        0      897 2024-05-07 20:56:57.576283 aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/utils.py
+-rw-r--r--   0        0        0      453 2024-04-22 15:35:28.441776 aiida_workgraph-0.2.6/aiida_workgraph/widget/tsconfig.json
+-rw-r--r--   0        0        0    14913 2024-05-20 19:33:14.095414 aiida_workgraph-0.2.6/aiida_workgraph/workgraph.py
+-rw-r--r--   0        0        0     3216 2024-05-23 10:17:58.548150 aiida_workgraph-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     7358 1970-01-01 00:00:00.000000 aiida_workgraph-0.2.6/PKG-INFO
```

### Comparing `aiida_workgraph-0.2.5/LICENSE` & `aiida_workgraph-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/README.md` & `aiida_workgraph-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/calculations/general_data.py` & `aiida_workgraph-0.2.6/aiida_workgraph/orm/general_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 """`Data` sub class to represent any data using pickle."""
 
-from aiida.orm import Data
+from aiida import orm
 
-__all__ = ("GeneralData",)
 
+class Dict(orm.Dict):
+    @property
+    def value(self):
+        return self.get_dict()
 
-class GeneralData(Data):
+
+class List(orm.List):
+    @property
+    def value(self):
+        return self.get_list()
+
+
+class GeneralData(orm.Data):
     """`Data to represent a pickled value."""
 
     def __init__(self, value=None, **kwargs):
         """Initialise a ``General`` node instance.
 
         :param value: list to initialise the ``List`` node from
         """
```

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/calculations/python.py` & `aiida_workgraph-0.2.6/aiida_workgraph/calculations/python.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 from aiida.orm import (
     Data,
     SinglefileData,
     Str,
     List,
     FolderData,
     RemoteData,
+    to_aiida_type,
 )
 
 
-from .general_data import GeneralData
-
 __all__ = ("PythonJob",)
 
 
 class PythonJob(CalcJob):
     """Calcjob to run a Python function on a remote computer."""
 
     # Default name of the subfolder that you want to create in the working directory,
@@ -41,41 +40,53 @@
     @classmethod
     def define(cls, spec: CalcJobProcessSpec) -> None:  # type: ignore[override]
         """Define the process specification, including its inputs, outputs and known exit codes.
 
         :param spec: the calculation job process spec to define.
         """
         super().define(spec)
-        spec.input("function_source_code", required=False)
-        spec.input("function_name", required=False)
-        spec.input_namespace("kwargs", valid_type=Data, required=False)
+        spec.input(
+            "function_source_code",
+            valid_type=Str,
+            serializer=to_aiida_type,
+            required=False,
+        )
+        spec.input(
+            "function_name", valid_type=Str, serializer=to_aiida_type, required=False
+        )
+        spec.input_namespace(
+            "kwargs", valid_type=Data, required=False
+        )  # , serializer=general_serializer)
         spec.input(
             "output_name_list",
             valid_type=List,
             required=False,
+            serializer=to_aiida_type,
             help="The names of the output ports",
         )
         spec.input(
             "parent_folder",
             valid_type=(RemoteData, FolderData, SinglefileData),
             required=False,
             help="Use a local or remote folder as parent folder (for restarts and similar)",
         )
         spec.input(
             "parent_output_folder",
-            valid_type=(Str),
+            valid_type=Str,
             default=None,
             required=False,
+            serializer=to_aiida_type,
             help="Name of the subfolder inside 'parent_folder' from which you want to copy the files",
         )
         spec.input(
             "additional_retrieve_list",
             valid_type=List,
             default=None,
             required=False,
+            serializer=to_aiida_type,
             help="The names of the files to retrieve",
         )
         spec.outputs.dynamic = True
         # set default options (optional)
         spec.inputs["metadata"]["options"]["parser_name"].default = "workgraph.python"
         spec.inputs["metadata"]["options"]["input_filename"].default = "script.py"
         spec.inputs["metadata"]["options"]["output_filename"].default = "aiida.out"
@@ -173,20 +184,22 @@
                 )
                 local_copy_list.append((source.uuid, dirname, self._PARENT_SUBFOLDER))
             elif isinstance(source, SinglefileData):
                 local_copy_list.append((source.uuid, source.filename, source.filename))
         # create pickle file for the inputs
         input_values = {}
         for key, value in inputs.items():
-            if isinstance(value, GeneralData):
+            if isinstance(value, Data) and hasattr(value, "value"):
                 # get the value of the pickled data
                 input_values[key] = value.value
             else:
-                raise ValueError(f"Unsupported data type: {type(value)}")
-            # save the value as a pickle file, the path is absolute
+                raise ValueError(
+                    f"Input data {value} is not supported. Only AiiDA data Node with a value attribute is allowed. "
+                )
+        # save the value as a pickle file, the path is absolute
         filename = "inputs.pickle"
         with folder.open(filename, "wb") as handle:
             pickle.dump(input_values, handle)
             # create a singlefiledata object for the pickled data
             file_data = SinglefileData(file=f"{dirpath}/{filename}")
             local_copy_list.append((file_data.uuid, file_data.filename, filename))
```

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/cli/cmd_graph.py` & `aiida_workgraph-0.2.6/aiida_workgraph/cli/cmd_graph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/cli/cmd_web.py` & `aiida_workgraph-0.2.6/aiida_workgraph/cli/cmd_web.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/cli/cmd_workgraph.py` & `aiida_workgraph-0.2.6/aiida_workgraph/cli/cmd_workgraph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/cli/query_workgraph.py` & `aiida_workgraph-0.2.6/aiida_workgraph/cli/query_workgraph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/collection.py` & `aiida_workgraph-0.2.6/aiida_workgraph/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
             build_node_from_callable,
             build_PythonJob_node,
         )
 
         # build the node on the fly if the identifier is a callable
         if callable(identifier):
             identifier = build_node_from_callable(identifier)
+            if kwargs.pop("run_remotely", False):
+                # this is a PythonJob
+                identifier = build_PythonJob_node(identifier)
         if isinstance(identifier, str) and identifier.upper() == "PYTHONJOB":
             # copy the inputs and outputs from the function node to the PythonJob node
             identifier = build_PythonJob_node(kwargs.pop("function"))
         # Call the original new method
         return super().new(identifier, name, uuid, **kwargs)
```

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/decorator.py` & `aiida_workgraph-0.2.6/aiida_workgraph/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,30 +232,40 @@
     node = create_node(ndata)
     return node, ndata
 
 
 def build_PythonJob_node(func: Callable) -> Node:
     """Build PythonJob node from function."""
     from aiida_workgraph.calculations.python import PythonJob
+    from copy import deepcopy
 
     ndata = {"executor": PythonJob, "node_type": "CALCJOB"}
     _, ndata_py = build_node_from_AiiDA(ndata)
-    ndata = func.ndata
+    ndata = deepcopy(func.ndata)
     # merge the inputs and outputs from the PythonJob node to the function node
     # skip the already existed inputs and outputs
     inputs = ndata["inputs"]
+    inputs.extend(
+        [
+            ["String", "computer"],
+            ["String", "code_label"],
+            ["String", "code_path"],
+            ["String", "prepend_text"],
+        ]
+    )
     outputs = ndata["outputs"]
     for input in ndata_py["inputs"]:
         if input not in inputs:
             inputs.append(input)
     for output in ndata_py["outputs"]:
         if output not in outputs:
             outputs.append(output)
     # append the kwargs of the PythonJob node to the function node
     kwargs = ndata["kwargs"]
+    kwargs.extend(["computer", "code_label", "code_path", "prepend_text"])
     kwargs.extend(ndata_py["kwargs"])
     ndata["inputs"] = inputs
     ndata["outputs"] = outputs
     ndata["kwargs"] = kwargs
     ndata["node_type"] = "PYTHONJOB"
     return create_node(ndata)
```

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/engine/workgraph.py` & `aiida_workgraph-0.2.6/aiida_workgraph/engine/workgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -821,40 +821,42 @@
                 print("submit workgraph: ")
                 process = self.submit(process_inited)
                 node["process"] = process
                 self.ctx.nodes[name]["state"] = "RUNNING"
                 self.to_context(**{name: process})
             elif node["metadata"]["node_type"].upper() in ["PYTHONJOB"]:
                 from aiida_workgraph.calculations.python import PythonJob
-                from aiida_workgraph.calculations.general_data import GeneralData
+                from aiida_workgraph.orm.serializer import general_serializer
+                from aiida_workgraph.utils import get_or_create_code
 
                 print("node  type: Python.")
                 # normal function does not have a process
-                code = kwargs.pop("code")
+                code = kwargs.pop("code", None)
+                computer = kwargs.pop("computer", None)
+                code_label = kwargs.pop("code_label", None)
+                code_path = kwargs.pop("code_path", None)
+                prepend_text = kwargs.pop("prepend_text", None)
+                #
+                if code is None:
+                    code = get_or_create_code(
+                        computer=computer or "localhost",
+                        code_label=code_label or "python3",
+                        code_path=code_path,
+                        prepend_text=prepend_text,
+                    )
                 parent_folder = kwargs.pop("parent_folder", None)
                 metadata = kwargs.pop("metadata", {})
                 metadata.update({"call_link_label": name})
                 # get the source code of the function
                 function_name = executor.__name__
                 function_source_code = node["executor"]["function_source_code"]
-                inputs = {}
-                # save all kwargs to inputs port
-                for key, value in kwargs.items():
-                    if isinstance(value, orm.Node):
-                        if not hasattr(value, "value"):
-                            raise ValueError(
-                                "Only AiiDA data Node with a value attribute is allowed."
-                            )
-                        inputs[key] = value
-                    else:
-                        inputs[key] = GeneralData(value)
-                print("inputs: ", inputs)
                 # outputs
                 output_name_list = [output["name"] for output in node["outputs"]]
-
+                # serialize the kwargs into AiiDA Data
+                inputs = general_serializer(kwargs)
                 # transfer the args to kwargs
                 process = self.submit(
                     PythonJob,
                     inputs={
                         "function_source_code": orm.Str(function_source_code),
                         "function_name": orm.Str(function_name),
                         "code": code,
```

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/executors/builtin.py` & `aiida_workgraph-0.2.6/aiida_workgraph/executors/builtin.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/executors/qe.py` & `aiida_workgraph-0.2.6/aiida_workgraph/executors/qe.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/executors/test.py` & `aiida_workgraph-0.2.6/aiida_workgraph/executors/test.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/node.py` & `aiida_workgraph-0.2.6/aiida_workgraph/node.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/nodes/__init__.py` & `aiida_workgraph-0.2.6/aiida_workgraph/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/nodes/builtin.py` & `aiida_workgraph-0.2.6/aiida_workgraph/nodes/builtin.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/nodes/qe.py` & `aiida_workgraph-0.2.6/aiida_workgraph/nodes/qe.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/nodes/test.py` & `aiida_workgraph-0.2.6/aiida_workgraph/nodes/test.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/orm/worktree.py` & `aiida_workgraph-0.2.6/aiida_workgraph/orm/worktree.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/properties/built_in.py` & `aiida_workgraph-0.2.6/aiida_workgraph/properties/built_in.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/property.py` & `aiida_workgraph-0.2.6/aiida_workgraph/property.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/socket.py` & `aiida_workgraph-0.2.6/aiida_workgraph/socket.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/sockets/built_in.py` & `aiida_workgraph-0.2.6/aiida_workgraph/sockets/built_in.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/utils/__init__.py` & `aiida_workgraph-0.2.6/aiida_workgraph/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, Optional, Union
 from aiida.engine.processes import Process
 from aiida import orm
+from aiida.common.exceptions import NotExistent
 
 
 def get_executor(data: Dict[str, Any]) -> Union[Process, Any]:
     """Import executor from path and return the executor and type."""
     import importlib
     from aiida.plugins import CalculationFactory, WorkflowFactory, DataFactory
 
@@ -232,7 +233,35 @@
                     nodes[label] = {
                         "pk": node.pk,
                         "state": "Stored" if node.is_stored else "Unstored",
                         "ctime": nodes.ctime,
                         "mtime": nodes.mtime,
                     }
     return nodes
+
+
+def get_or_create_code(
+    computer: str = "localhost",
+    code_label: str = "python3",
+    code_path: str = None,
+    prepend_text: str = "",
+):
+    """Try to load code, create if not exit."""
+    from aiida.orm.nodes.data.code.installed import InstalledCode
+
+    try:
+        return orm.load_code(f"{code_label}@{computer}")
+    except NotExistent:
+        description = f"Python code on computer: {computer}"
+        computer = orm.load_computer(computer)
+        code_path = code_path or code_label
+        code = InstalledCode(
+            computer=computer,
+            label=code_label,
+            description=description,
+            filepath_executable=code_path,
+            default_calc_job_plugin="workgraph.python",
+            prepend_text=prepend_text,
+        )
+
+        code.store()
+        return code
```

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/utils/analysis.py` & `aiida_workgraph-0.2.6/aiida_workgraph/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/utils/graph.py` & `aiida_workgraph-0.2.6/aiida_workgraph/utils/graph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/README.md` & `aiida_workgraph-0.2.6/aiida_workgraph/web/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/api.py` & `aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/api.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/daemon.py` & `aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/daemon.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/datanode.py` & `aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/datanode.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/utils.py` & `aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/backend/app/workgraph.py` & `aiida_workgraph-0.2.6/aiida_workgraph/web/backend/app/workgraph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/README.md` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/asset-manifest.json` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/favicon.ico` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/index.html` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/css/main.8ddb8b68.css.map`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/787.095790c7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/build/static/js/main.1b3f61aa.js.map`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/package-lock.json` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/package.json` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/package.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/public/favicon.ico` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/public/index.html` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/App.css` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/App.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/App.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/App.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/AtomsItem.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/AtomsItem.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/DataNodeItem.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/DataNodeTable.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/DataNodeTable.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Layout.css` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Layout.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Layout.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Layout.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/NodeDetails.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/NodeDetails.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/Settings.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/Settings.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphDetail.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphDuration.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphIndicator.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphItem.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphItemStyles.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphLog.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphSummary.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphTable.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/components/WorkGraphTable.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/index.tsx` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/logo.svg` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/logo.svg`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization.ts` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/CustomConnection.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/CustomNode.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/CustomSocket.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/StyledNode.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/customization/background.css` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/customization/background.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/default.ts` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/default.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/src/rete/index.ts` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/src/rete/index.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/web/frontend/tsconfig.json` & `aiida_workgraph-0.2.6/aiida_workgraph/web/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/widget/README.md` & `aiida_workgraph-0.2.6/aiida_workgraph/widget/README.md`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/widget/js/default_rete.ts` & `aiida_workgraph-0.2.6/aiida_workgraph/widget/js/default_rete.ts`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/widget/js/widget.css` & `aiida_workgraph-0.2.6/aiida_workgraph/widget/js/widget.css`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/widget/js/widget.tsx` & `aiida_workgraph-0.2.6/aiida_workgraph/widget/js/widget.tsx`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/widget/package-lock.json` & `aiida_workgraph-0.2.6/aiida_workgraph/widget/package-lock.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/widget/package.json` & `aiida_workgraph-0.2.6/aiida_workgraph/widget/package.json`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/widget/pyproject.toml` & `aiida_workgraph-0.2.6/aiida_workgraph/widget/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/__init__.py` & `aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/static/widget.js` & `aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/static/widget.js`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/widget/src/widget/utils.py` & `aiida_workgraph-0.2.6/aiida_workgraph/widget/src/widget/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/aiida_workgraph/workgraph.py` & `aiida_workgraph-0.2.6/aiida_workgraph/workgraph.py`

 * *Files identical despite different names*

### Comparing `aiida_workgraph-0.2.5/pyproject.toml` & `aiida_workgraph-0.2.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -73,15 +73,23 @@
 [project.entry-points."aiida.calculations"]
 "workgraph.python" = "aiida_workgraph.calculations.python:PythonJob"
 
 [project.entry-points."aiida.parsers"]
 "workgraph.python" = "aiida_workgraph.calculations.python_parser:PythonParser"
 
 [project.entry-points."aiida.data"]
-"workgraph.general" = "aiida_workgraph.calculations.general_data:GeneralData"
+"workgraph.general" = "aiida_workgraph.orm.general_data:GeneralData"
+"ase.atoms.Atoms" = "aiida_workgraph.orm.atoms:AtomsData"
+"builtins.int" = "aiida.orm.nodes.data.int:Int"
+"builtins.float" = "aiida.orm.nodes.data.float:Float"
+"builtins.str" = "aiida.orm.nodes.data.str:Str"
+"builtins.bool" = "aiida.orm.nodes.data.bool:Bool"
+"builtins.list"="aiida_workgraph.orm.general_data:List"
+"builtins.dict"="aiida_workgraph.orm.general_data:Dict"
+
 
 [project.entry-points."aiida.node"]
 "process.workflow.workgraph" = "aiida_workgraph.orm.workgraph:WorkgraphNode"
 
 [project.entry-points."aiida_workgraph.node"]
 "aiida" = "aiida_workgraph.nodes:node_list"
```

### Comparing `aiida_workgraph-0.2.5/PKG-INFO` & `aiida_workgraph-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-workgraph
-Version: 0.2.5
+Version: 0.2.6
 Summary: Design flexible node-based workflow for AiiDA calculation.
 Keywords: aiida,workflows
 Author-email: Xing Wang <xingwang1991@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Framework :: AiiDA
```

