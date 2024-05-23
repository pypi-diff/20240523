# Comparing `tmp/aizynthfinder-4.0.0.tar.gz` & `tmp/aizynthfinder-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aizynthfinder-4.0.0.tar", max compression
+gzip compressed data, was "aizynthfinder-4.3.0.tar", max compression
```

## Comparing `aizynthfinder-4.0.0.tar` & `aizynthfinder-4.3.0.tar`

### file list

```diff
@@ -1,70 +1,74 @@
--rw-r--r--   0        0        0     1072 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/LICENSE
--rw-r--r--   0        0        0     5563 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/README.md
--rw-r--r--   0        0        0        0 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/__init__.py
--rw-r--r--   0        0        0    12532 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/aizynthfinder.py
--rw-r--r--   0        0        0      249 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/analysis/__init__.py
--rw-r--r--   0        0        0    14215 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/analysis/routes.py
--rw-r--r--   0        0        0     9445 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/analysis/tree_analysis.py
--rw-r--r--   0        0        0     4985 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/analysis/utils.py
--rw-r--r--   0        0        0      493 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/chem/__init__.py
--rw-r--r--   0        0        0    12921 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/chem/mol.py
--rw-r--r--   0        0        0    21975 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/chem/reaction.py
--rw-r--r--   0        0        0     4772 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/chem/serialization.py
--rw-r--r--   0        0        0        0 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/__init__.py
--rw-r--r--   0        0        0     4585 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/collection.py
--rw-r--r--   0        0        0     6323 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/config.py
--rw-r--r--   0        0        0      470 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/policy/__init__.py
--rw-r--r--   0        0        0    12104 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/policy/expansion_strategies.py
--rw-r--r--   0        0        0     5680 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/policy/filter_strategies.py
--rw-r--r--   0        0        0     7663 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/policy/policies.py
--rw-r--r--   0        0        0      572 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/policy/utils.py
--rw-r--r--   0        0        0      571 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/scoring/__init__.py
--rw-r--r--   0        0        0     5888 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/scoring/collection.py
--rw-r--r--   0        0        0    19909 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/scoring/scorers.py
--rw-r--r--   0        0        0      282 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/stock/__init__.py
--rw-r--r--   0        0        0     8367 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/stock/queries.py
--rw-r--r--   0        0        0    10654 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/context/stock/stock.py
--rw-r--r--   0        0        0     1446 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/data/default_training.yml
--rw-r--r--   0        0        0      487 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/data/logging.yml
--rw-r--r--   0        0        0      782 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/data/templates/reaction_tree.dot
--rw-r--r--   0        0        0     1265 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/data/templates/reaction_tree.thtml
--rw-r--r--   0        0        0      176 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/interfaces/__init__.py
--rw-r--r--   0        0        0    13604 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/interfaces/aizynthapp.py
--rw-r--r--   0        0        0    11961 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/interfaces/aizynthcli.py
--rw-r--r--   0        0        0       81 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/interfaces/gui/__init__.py
--rw-r--r--   0        0        0     4248 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/interfaces/gui/clustering.py
--rw-r--r--   0        0        0    14317 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/reactiontree.py
--rw-r--r--   0        0        0        0 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/search/__init__.py
--rw-r--r--   0        0        0     8221 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/search/andor_trees.py
--rw-r--r--   0        0        0      124 2023-12-05 15:36:35.386745 aizynthfinder-4.0.0/aizynthfinder/search/breadth_first/__init__.py
--rw-r--r--   0        0        0     7760 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/breadth_first/nodes.py
--rw-r--r--   0        0        0     5603 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/breadth_first/search_tree.py
--rw-r--r--   0        0        0      106 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/dfpn/__init__.py
--rw-r--r--   0        0        0    11087 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/dfpn/nodes.py
--rw-r--r--   0        0        0     4758 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/dfpn/search_tree.py
--rw-r--r--   0        0        0      211 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/mcts/__init__.py
--rw-r--r--   0        0        0    19629 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/mcts/node.py
--rw-r--r--   0        0        0     5710 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/mcts/search.py
--rw-r--r--   0        0        0     5027 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/mcts/state.py
--rw-r--r--   0        0        0     2583 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/mcts/utils.py
--rw-r--r--   0        0        0        0 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/retrostar/__init__.py
--rw-r--r--   0        0        0     4450 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/retrostar/cost.py
--rw-r--r--   0        0        0    12266 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/retrostar/nodes.py
--rw-r--r--   0        0        0     6719 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/search/retrostar/search_tree.py
--rw-r--r--   0        0        0        0 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/tools/__init__.py
--rw-r--r--   0        0        0      815 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/tools/cat_output.py
--rw-r--r--   0        0        0     3680 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/tools/download_public_data.py
--rw-r--r--   0        0        0     7209 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/tools/make_stock.py
--rw-r--r--   0        0        0        0 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/utils/__init__.py
--rw-r--r--   0        0        0      914 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/utils/exceptions.py
--rw-r--r--   0        0        0     5322 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/utils/files.py
--rw-r--r--   0        0        0    14081 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/utils/image.py
--rw-r--r--   0        0        0     1532 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/utils/loading.py
--rw-r--r--   0        0        0     1694 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/utils/logging.py
--rw-r--r--   0        0        0      299 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/utils/math.py
--rw-r--r--   0        0        0    12001 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/utils/models.py
--rw-r--r--   0        0        0     1559 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/utils/mongo.py
--rw-r--r--   0        0        0      355 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/utils/paths.py
--rw-r--r--   0        0        0      729 2023-12-05 15:36:35.390745 aizynthfinder-4.0.0/aizynthfinder/utils/type_utils.py
--rw-r--r--   0        0        0     2367 2023-12-05 15:36:35.394745 aizynthfinder-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     7366 1970-01-01 00:00:00.000000 aizynthfinder-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/LICENSE
+-rw-r--r--   0        0        0     5549 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/__init__.py
+-rw-r--r--   0        0        0    15755 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/aizynthfinder.py
+-rw-r--r--   0        0        0      249 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/analysis/__init__.py
+-rw-r--r--   0        0        0    14316 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/analysis/routes.py
+-rw-r--r--   0        0        0    16442 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/analysis/tree_analysis.py
+-rw-r--r--   0        0        0     4985 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/analysis/utils.py
+-rw-r--r--   0        0        0      493 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/chem/__init__.py
+-rw-r--r--   0        0        0    13936 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/chem/mol.py
+-rw-r--r--   0        0        0    22347 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/chem/reaction.py
+-rw-r--r--   0        0        0     4772 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/chem/serialization.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/context/__init__.py
+-rw-r--r--   0        0        0     4585 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/context/collection.py
+-rw-r--r--   0        0        0     6476 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/context/config.py
+-rw-r--r--   0        0        0      529 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/context/policy/__init__.py
+-rw-r--r--   0        0        0    18512 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/context/policy/expansion_strategies.py
+-rw-r--r--   0        0        0     6716 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/context/policy/filter_strategies.py
+-rw-r--r--   0        0        0     7915 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/context/policy/policies.py
+-rw-r--r--   0        0        0      572 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/context/policy/utils.py
+-rw-r--r--   0        0        0      681 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/context/scoring/__init__.py
+-rw-r--r--   0        0        0     6360 2024-05-23 11:25:07.883640 aizynthfinder-4.3.0/aizynthfinder/context/scoring/collection.py
+-rw-r--r--   0        0        0    30271 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/context/scoring/scorers.py
+-rw-r--r--   0        0        0      282 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/context/stock/__init__.py
+-rw-r--r--   0        0        0     8284 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/context/stock/queries.py
+-rw-r--r--   0        0        0    10684 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/context/stock/stock.py
+-rw-r--r--   0        0        0     1446 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/data/default_training.yml
+-rw-r--r--   0        0        0      487 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/data/logging.yml
+-rw-r--r--   0        0        0      782 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/data/templates/reaction_tree.dot
+-rw-r--r--   0        0        0     1265 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/data/templates/reaction_tree.thtml
+-rw-r--r--   0        0        0      176 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/interfaces/__init__.py
+-rw-r--r--   0        0        0    14411 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/interfaces/aizynthapp.py
+-rw-r--r--   0        0        0    12643 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/interfaces/aizynthcli.py
+-rw-r--r--   0        0        0       81 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/interfaces/gui/__init__.py
+-rw-r--r--   0        0        0     4248 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/interfaces/gui/clustering.py
+-rw-r--r--   0        0        0     5865 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/interfaces/gui/pareto_fronts.py
+-rw-r--r--   0        0        0     4083 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/interfaces/gui/utils.py
+-rw-r--r--   0        0        0    14827 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/reactiontree.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/__init__.py
+-rw-r--r--   0        0        0     8159 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/andor_trees.py
+-rw-r--r--   0        0        0      124 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/breadth_first/__init__.py
+-rw-r--r--   0        0        0     7760 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/breadth_first/nodes.py
+-rw-r--r--   0        0        0     5603 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/breadth_first/search_tree.py
+-rw-r--r--   0        0        0      106 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/dfpn/__init__.py
+-rw-r--r--   0        0        0    11087 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/dfpn/nodes.py
+-rw-r--r--   0        0        0     4758 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/dfpn/search_tree.py
+-rw-r--r--   0        0        0      211 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/mcts/__init__.py
+-rw-r--r--   0        0        0    28273 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/mcts/node.py
+-rw-r--r--   0        0        0     8259 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/mcts/search.py
+-rw-r--r--   0        0        0     5022 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/mcts/state.py
+-rw-r--r--   0        0        0     2582 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/mcts/utils.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/retrostar/__init__.py
+-rw-r--r--   0        0        0     4486 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/retrostar/cost.py
+-rw-r--r--   0        0        0    12266 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/retrostar/nodes.py
+-rw-r--r--   0        0        0     6719 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/search/retrostar/search_tree.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/tools/__init__.py
+-rw-r--r--   0        0        0      815 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/tools/cat_output.py
+-rw-r--r--   0        0        0     3680 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/tools/download_public_data.py
+-rw-r--r--   0        0        0     7259 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/tools/make_stock.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/__init__.py
+-rw-r--r--   0        0        0     2515 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/bonds.py
+-rw-r--r--   0        0        0      914 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/exceptions.py
+-rw-r--r--   0        0        0     5322 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/files.py
+-rw-r--r--   0        0        0    14141 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/image.py
+-rw-r--r--   0        0        0     1532 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/loading.py
+-rw-r--r--   0        0        0     1694 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/logging.py
+-rw-r--r--   0        0        0     1104 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/math.py
+-rw-r--r--   0        0        0    12070 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/models.py
+-rw-r--r--   0        0        0     1584 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/mongo.py
+-rw-r--r--   0        0        0      355 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/paths.py
+-rw-r--r--   0        0        0     3059 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/sc_score.py
+-rw-r--r--   0        0        0      729 2024-05-23 11:25:07.887640 aizynthfinder-4.3.0/aizynthfinder/utils/type_utils.py
+-rw-r--r--   0        0        0     2487 2024-05-23 11:25:07.895640 aizynthfinder-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7535 1970-01-01 00:00:00.000000 aizynthfinder-4.3.0/PKG-INFO
```

### Comparing `aizynthfinder-4.0.0/LICENSE` & `aizynthfinder-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/README.md` & `aizynthfinder-4.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AiZynthFinder
 
 [![License](https://img.shields.io/github/license/MolecularAI/aizynthfinder)](https://github.com/MolecularAI/aizynthfinder/blob/master/LICENSE)
 [![Tests](https://github.com/MolecularAI/aizynthfinder/workflows/tests/badge.svg)](https://github.com/MolecularAI/aizynthfinder/actions?workflow=tests)
 [![codecov](https://codecov.io/gh/MolecularAI/aizynthfinder/branch/master/graph/badge.svg)](https://codecov.io/gh/MolecularAI/aizynthfinder)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black) 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![version](https://img.shields.io/github/v/release/MolecularAI/aizynthfinder)](https://github.com/MolecularAI/aizynthfinder/releases)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MolecularAI/aizynthfinder/blob/master/contrib/notebook.ipynb)
 
 AiZynthFinder is a tool for retrosynthetic planning. The default algorithm is based on a Monte Carlo tree search that recursively breaks down a molecule to purchasable precursors. The tree search is guided by a policy that suggests possible precursors by utilizing a neural network trained on a library of known reaction templates. This setup is completely customizable as the tool
 supports multiple search algorithms and expansion policies.
 
 An introduction video can be found here: [https://youtu.be/r9Dsxm-mcgA](https://youtu.be/r9Dsxm-mcgA)
@@ -24,35 +24,35 @@
 
 ## Installation
 
 ### For end-users
 
 First time, execute the following command in a console or an Anaconda prompt
 
-    conda create "python>=3.8,<3.10" -n aizynth-env
+    conda create "python>=3.9,<3.11" -n aizynth-env
 
 To install, activate the environment and install the package using pypi
 
     conda activate aizynth-env
     python -m pip install aizynthfinder[all]
 
 for a smaller package, without all the functionality, you can also type
 
     python -m pip install aizynthfinder
 
 ### For developers
 
 First clone the repository using Git.
 
-Then execute the following commands in the root of the repository 
+Then execute the following commands in the root of the repository
 
     conda env create -f env-dev.yml
     conda activate aizynth-dev
     poetry install --all-extras
-    
+
 the `aizynthfinder` package is now installed in editable mode.
 
 
 ## Usage
 
 The tool will install the `aizynthcli` and `aizynthapp` tools
 as interfaces to the algorithm:
@@ -64,15 +64,15 @@
 Consult the documentation [here](https://molecularai.github.io/aizynthfinder/) for more information.
 
 To use the tool you need
 
     1. A stock file
     2. A trained expansion policy network
     3. A trained filter policy network (optional)
-    
+
 Such files can be downloaded from [figshare](https://figshare.com/articles/AiZynthFinder_a_fast_robust_and_flexible_open-source_software_for_retrosynthetic_planning/12334577) and [here](https://figshare.com/articles/dataset/A_quick_policy_to_filter_reactions_based_on_feasibility_in_AI-guided_retrosynthetic_planning/13280507) or they can be downloaded automatically using
 
 ```
 download_public_data my_folder
 ```
 
 where ``my_folder`` is the folder that you want download to.
@@ -87,15 +87,15 @@
 Run the tests using:
 
     pytest -v
 
 The full command run on the CI server is available through an `invoke` command
 
     invoke full-tests
-    
+
  ### Documentation generation
 
 The documentation is generated by Sphinx from hand-written tutorials and docstrings
 
 The HTML documentation can be generated by
 
     invoke build-docs
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/aizynthfinder.py` & `aizynthfinder-4.3.0/aizynthfinder/aizynthfinder.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from aizynthfinder.analysis import (
     RouteCollection,
     RouteSelectionArguments,
     TreeAnalysis,
 )
 from aizynthfinder.chem import FixedRetroReaction, Molecule, TreeMolecule
 from aizynthfinder.context.config import Configuration
-from aizynthfinder.context.scoring import CombinedScorer
+from aizynthfinder.context.policy import BondFilter
+from aizynthfinder.context.scoring import BrokenBondsScorer, CombinedScorer
 from aizynthfinder.reactiontree import ReactionTreeFromExpansion
 from aizynthfinder.search.andor_trees import AndOrSearchTreeBase
 from aizynthfinder.search.mcts import MctsSearchTree
 from aizynthfinder.utils.exceptions import MoleculeException
 from aizynthfinder.utils.loading import load_dynamic_class
 
 # This must be imported first to setup logging for rdkit, tensorflow etc
@@ -78,14 +79,17 @@
         self.stock = self.config.stock
         self.scorers = self.config.scorers
         self.tree: Optional[Union[MctsSearchTree, AndOrSearchTreeBase]] = None
         self._target_mol: Optional[Molecule] = None
         self.search_stats: StrDict = dict()
         self.routes = RouteCollection([])
         self.analysis: Optional[TreeAnalysis] = None
+        self._num_objectives = len(
+            self.config.search.algorithm_config.get("search_rewards", [])
+        )
 
     @property
     def target_smiles(self) -> str:
         """The SMILES representation of the molecule to predict routes on."""
         if not self._target_mol:
             return ""
         return self._target_mol.smiles
@@ -103,35 +107,27 @@
     def target_mol(self, mol: Molecule) -> None:
         self.tree = None
         self._target_mol = mol
 
     def build_routes(
         self,
         selection: Optional[RouteSelectionArguments] = None,
-        scorer: Optional[str] = None,
+        scorer: Optional[Union[str, List[str]]] = None,
     ) -> None:
         """
         Build reaction routes
 
         This is necessary to call after the tree search has completed in order
         to extract results from the tree search.
 
         :param selection: the selection criteria for the routes
-        :param scorer: a reference to the object used to score the nodes
+        :param scorer: a reference to the object used to score the nodes, can be a list
         :raises ValueError: if the search tree not initialized
         """
-
-        scorer = scorer or self.config.post_processing.route_scorer
-
-        if not self.tree:
-            raise ValueError("Search tree not initialized")
-
-        _scorer = self.scorers[scorer]
-
-        self.analysis = TreeAnalysis(self.tree, scorer=_scorer)
+        self.analysis = self._setup_analysis(scorer=scorer)
         config_selection = RouteSelectionArguments(
             nmin=self.config.post_processing.min_routes,
             nmax=self.config.post_processing.max_routes,
             return_all=self.config.post_processing.all_routes,
         )
         self.routes = RouteCollection.from_analysis(
             self.analysis, selection or config_selection
@@ -170,17 +166,21 @@
         if (
             self.config.search.exclude_target_from_stock
             and self.target_mol in self.stock
         ):
             self.stock.exclude(self.target_mol)
             self._logger.debug("Excluding the target compound from the stock")
 
+        if self.config.search.break_bonds or self.config.search.freeze_bonds:
+            self._setup_focussed_bonds(self.target_mol)
+
         self._setup_search_tree()
         self.analysis = None
         self.routes = RouteCollection([])
+        self.filter_policy.reset_cache()
         self.expansion_policy.reset_cache()
 
     def stock_info(self) -> StrDict:
         """
         Return the stock availability for all leaf nodes in all collected reaction trees
 
         The key of the return dictionary will be the SMILES string of the leaves,
@@ -245,24 +245,100 @@
         if show_progress:
             pbar.close()
         time_past = time.time() - time0
         self._logger.debug("Search completed")
         self.search_stats["time"] = time_past
         return time_past
 
+    def _setup_focussed_bonds(self, target_mol: Molecule) -> None:
+        """
+        Setup multi-objective scoring function with 'broken bonds'-scorer and
+        add 'frozen bonds'-filter to filter policy.
+
+        :param target_mol: the target molecule.
+        """
+        target_mol = TreeMolecule(smiles=target_mol.smiles, parent=None)
+
+        bond_filter_key = "__finder_bond_filter"
+        if self.config.search.freeze_bonds:
+            if not target_mol.has_all_focussed_bonds(self.config.search.freeze_bonds):
+                raise ValueError("Bonds in 'freeze_bond' must exist in target molecule")
+            bond_filter = BondFilter(bond_filter_key, self.config)
+            self.filter_policy.load(bond_filter)
+            self.filter_policy.select(bond_filter_key, append=True)
+        elif (
+            self.filter_policy.selection
+            and bond_filter_key in self.filter_policy.selection
+        ):
+            self.filter_policy.deselect(bond_filter_key)
+
+        search_rewards = self.config.search.algorithm_config.get("search_rewards")
+        if not search_rewards:
+            return
+
+        if self.config.search.break_bonds and "broken bonds" in search_rewards:
+            if not target_mol.has_all_focussed_bonds(self.config.search.break_bonds):
+                raise ValueError("Bonds in 'break_bonds' must exist in target molecule")
+            self.scorers.load(BrokenBondsScorer(self.config))
+            self._num_objectives = len(search_rewards)
+
     def _setup_search_tree(self) -> None:
-        self._logger.debug("Defining tree root: %s" % self.target_smiles)
+        self._logger.debug(f"Defining tree root:  {self.target_smiles}")
         if self.config.search.algorithm.lower() == "mcts":
             self.tree = MctsSearchTree(
                 root_smiles=self.target_smiles, config=self.config
             )
         else:
             cls = load_dynamic_class(self.config.search.algorithm)
             self.tree = cls(root_smiles=self.target_smiles, config=self.config)
 
+    def _setup_analysis(
+        self,
+        scorer: Optional[Union[str, List[str]]],
+    ) -> TreeAnalysis:
+        """Configure TreeAnalysis
+
+        :param scorer: a reference to the object used to score the nodes, can be a list
+        :returns: the configured TreeAnalysis
+        :raises ValueError: if the search tree not initialized
+        """
+        if not self.tree:
+            raise ValueError("Search tree not initialized")
+
+        if scorer is None:
+            scorer_names = self.config.post_processing.route_scorers
+            # If not defined, use the same scorer as the search rewards
+            if not scorer_names:
+                search_rewards = self.config.search.algorithm_config.get(
+                    "search_rewards"
+                )
+                scorer_names = search_rewards if search_rewards else ["state score"]
+
+        elif isinstance(scorer, str):
+            scorer_names = [scorer]
+        else:
+            scorer_names = list(scorer)
+
+        if "broken bonds" in scorer_names:
+            # Add broken bonds scorer if required
+            self.scorers.load(BrokenBondsScorer(self.config))
+
+        scorers = [self.scorers[name] for name in scorer_names]
+
+        if self.config.post_processing.scorer_weights:
+            scorers = [
+                CombinedScorer(
+                    self.config,
+                    scorer_names,
+                    self.config.post_processing.scorer_weights,
+                )
+            ]
+
+        return TreeAnalysis(self.tree, scorers)
+
 
 class AiZynthExpander:
     """
     Public API to the AiZynthFinder expansion and filter policies
 
     If instantiated with the path to a yaml file or dictionary of settings
     the stocks and policy networks are loaded directly.
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/analysis/routes.py` & `aizynthfinder-4.3.0/aizynthfinder/analysis/routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """ Module containing classes to store and manipulate collections of synthetic routes.
 """
 from __future__ import annotations
 
+import copy
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 try:
     from route_distances.clustering import ClusteringHelper
     from route_distances.route_distances import route_distances_calculator
 except ImportError:
     pass
 
-from aizynthfinder.analysis import TreeAnalysis
 from aizynthfinder.analysis.utils import CombinedReactionTrees, RouteSelectionArguments
 from aizynthfinder.reactiontree import SUPPORT_DISTANCES, ReactionTree
 from aizynthfinder.search.mcts import MctsNode, MctsSearchTree
 
 if TYPE_CHECKING:
+    from aizynthfinder.analysis import TreeAnalysis
     from aizynthfinder.context.scoring import Scorer
     from aizynthfinder.utils.type_utils import (
         Any,
         Dict,
         Optional,
         PilImage,
         Sequence,
         StrDict,
+        Union,
     )
 
 
 class RouteCollection:
     """
     Holds a collections of reaction routes.
 
@@ -60,42 +62,44 @@
         self._routes: Sequence[StrDict] = [{} for _ in range(len(reaction_trees))]
         self.reaction_trees = reaction_trees
         self._update_route_dict(reaction_trees, "reaction_tree")
         self.route_metadata = [rt.metadata for rt in reaction_trees]
         self._update_route_dict(self.route_metadata, "route_metadata")
 
         self.nodes = self._unpack_kwarg_with_default("nodes", None, **kwargs)
-        self.scores = self._unpack_kwarg_with_default("scores", np.nan, **kwargs)
+        self.scores = self._unpack_kwarg_with_default("scores", dict, **kwargs)
         self.all_scores = self._unpack_kwarg_with_default("all_scores", dict, **kwargs)
 
         self._dicts: Optional[Sequence[StrDict]] = self._unpack_kwarg("dicts", **kwargs)
-        self._images: Optional[Sequence[PilImage]] = self._unpack_kwarg(
+        self._images: Optional[Sequence[Optional[PilImage]]] = self._unpack_kwarg(
             "images", **kwargs
         )
         self._jsons: Optional[Sequence[str]] = self._unpack_kwarg("jsons", **kwargs)
         self.clusters: Optional[Sequence[RouteCollection]] = self._unpack_kwarg(
             "clusters", **kwargs
         )
         self._distance_matrix: Dict[str, np.ndarray] = {}
         self._combined_reaction_trees: Optional[CombinedReactionTrees] = None
 
     @classmethod
     def from_analysis(
-        cls, analysis: TreeAnalysis, selection: RouteSelectionArguments = None
+        cls,
+        analysis: TreeAnalysis,
+        selection: Optional[RouteSelectionArguments] = None,
     ) -> "RouteCollection":
         """
         Create a collection from a tree analysis.
 
         :param analysis: the tree analysis to use
         :param selection: selection criteria for the routes
         :return: the created collection
         """
         items, scores = analysis.sort(selection)
-        all_scores = [{repr(analysis.scorer): score} for score in scores]
-        kwargs = {"scores": scores, "all_scores": all_scores}
+        all_scores = copy.deepcopy(scores)
+        kwargs: Dict[str, Any] = {"scores": scores, "all_scores": all_scores}
         if isinstance(analysis.search_tree, MctsSearchTree):
             kwargs["nodes"] = items
             reaction_trees = [
                 from_node.to_reaction_tree()
                 for from_node in items
                 if isinstance(from_node, MctsNode)
             ]
@@ -116,18 +120,19 @@
     def dicts(self) -> Sequence[StrDict]:
         """Returns a list of dictionary representation of the routes"""
         if self._dicts is None:
             self._dicts = self.make_dicts()
         return self._dicts
 
     @property
-    def images(self) -> Sequence[PilImage]:
+    def images(self) -> Sequence[Optional[PilImage]]:
         """Returns a list of pictoral representation of the routes"""
         if self._images is None:
             self._images = self.make_images()
+        assert self._images is not None
         return self._images
 
     @property
     def jsons(self) -> Sequence[str]:
         """Returns a list of JSON string representation of the routes"""
         if self._jsons is None:
             self._jsons = self.make_jsons()
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/analysis/tree_analysis.py` & `aizynthfinder-4.3.0/aizynthfinder/context/stock/stock.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,245 +1,328 @@
-""" Module containing classes to perform analysis of the tree search results.
+""" Module containing classes that interfaces different stock classes
 """
 from __future__ import annotations
 
+import copy
 from collections import defaultdict
 from typing import TYPE_CHECKING
 
-from aizynthfinder.analysis.utils import RouteSelectionArguments
-from aizynthfinder.chem import FixedRetroReaction, hash_reactions
-from aizynthfinder.context.scoring import StateScorer
-from aizynthfinder.reactiontree import ReactionTree
-from aizynthfinder.search.andor_trees import AndOrSearchTreeBase
-from aizynthfinder.search.mcts import MctsNode, MctsSearchTree
+from aizynthfinder.chem import Molecule
+from aizynthfinder.context.collection import ContextCollection
+from aizynthfinder.context.stock.queries import (
+    InMemoryInchiKeyQuery,
+    MolbloomFilterQuery,
+    STOCK_QUERY_ALIAS,
+    StockQueryMixin,
+)
+from aizynthfinder.context.stock.queries import __name__ as queries_module
+from aizynthfinder.utils.exceptions import StockException
+from aizynthfinder.utils.loading import load_dynamic_class
 
 if TYPE_CHECKING:
-    from aizynthfinder.chem import RetroReaction
-    from aizynthfinder.context.scoring import Scorer
     from aizynthfinder.utils.type_utils import (
         Any,
-        Iterable,
+        Dict,
         List,
         Optional,
-        Sequence,
+        Set,
         StrDict,
-        Tuple,
         Union,
     )
 
 
-class TreeAnalysis:
+class Stock(ContextCollection):
     """
-    Class that encapsulate various analysis that can be
-    performed on a search tree.
+    A collection of molecules that are in stock
 
-    :ivar scorer: the object used to score the nodes
-    :ivar search_tree: the search tree
+    A molecule can be queried on the stock with:
+
+    .. code-block::
+
+        my_mol = Molecule(smiles="CCO")
+        my_mol in stock
+
+    One can obtain individual stocks with:
+
+    .. code-block::
+
+        sub_stock = stock["key"]
+
+    One can obtain the number of molecules in the selected stock with:
+
+    .. code-block::
+
+        number_of_molecules = len(stock)
 
-    :param search_tree: the search tree to do the analysis on
-    :param scorer: the object used to score the nodes, defaults to StateScorer
     """
 
-    def __init__(
-        self,
-        search_tree: Union[MctsSearchTree, AndOrSearchTreeBase],
-        scorer: Optional[Scorer] = None,
-    ) -> None:
-        self.search_tree = search_tree
-        if scorer is None:
-            self.scorer: Scorer = StateScorer(search_tree.config)
-        else:
-            self.scorer = scorer
-
-    def best(self) -> Union[MctsNode, ReactionTree]:
-        """
-        Returns the route or MCTS-like node with the highest score.
-        If several routes have the same score, it will return the first
-
-        :return: the top scoring node or route
-        """
-        if isinstance(self.search_tree, MctsSearchTree):
-            nodes = self._all_nodes()
-            sorted_nodes, _, _ = self.scorer.sort(nodes)
-            return sorted_nodes[0]
-
-        sorted_routes, _, _ = self.scorer.sort(self.search_tree.routes())
-        return sorted_routes[0]
-
-    def sort(
-        self, selection: Optional[RouteSelectionArguments] = None
-    ) -> Tuple[Union[Sequence[MctsNode], Sequence[ReactionTree]], Sequence[float]]:
-        """
-        Sort and select the nodes or routes in the search tree.
-
-        :param selection: selection criteria for the routes
-        :return: the items
-        :return: the score
-        """
-        selection = selection or RouteSelectionArguments()
-
-        if isinstance(self.search_tree, MctsSearchTree):
-            nodes = self._all_nodes()
-            sorted_items, sorted_scores, _ = self.scorer.sort(nodes)
-            actions = [node.actions_to() for node in sorted_items]
-
-        else:
-            sorted_items, sorted_scores, _ = self.scorer.sort(self.search_tree.routes())
-            actions = [route.reactions() for route in sorted_items]
-
-        return self._collect_top_items(sorted_items, sorted_scores, actions, selection)
-
-    def tree_statistics(self) -> StrDict:
-        """
-        Returns statistics of the tree
-
-        Currently it returns the number of nodes, the maximum number of transforms,
-        maximum number of children, top score, if the top score route is solved,
-        the number of molecule in the top score node, and information on pre-cursors
-
-        :return: the statistics
-        """
-        if isinstance(self.search_tree, MctsSearchTree):
-            return self._tree_statistics_mcts()
-        return self._tree_statistics_andor()
-
-    def _all_nodes(self) -> Sequence[MctsNode]:
-        assert isinstance(self.search_tree, MctsSearchTree)
-        # This is to keep backwards compatibility, this should be investigate further
-        if repr(self.scorer) == "state score":
-            return list(self.search_tree.graph())
-        return [node for node in self.search_tree.graph() if not node.children]
-
-    def _tree_statistics_andor(self) -> StrDict:
-        assert isinstance(self.search_tree, AndOrSearchTreeBase)
-        top_route = self.best()
-        assert isinstance(top_route, ReactionTree)
-        mols_in_stock = ", ".join(
-            mol.smiles for mol in top_route.leafs() if top_route.in_stock(mol)
-        )
-        mols_not_in_stock = ", ".join(
-            mol.smiles for mol in top_route.leafs() if not top_route.in_stock(mol)
-        )
-        all_routes = self.search_tree.routes()
-        policy_used_counts = self._policy_used_statistics(
-            [reaction for route in all_routes for reaction in route.reactions()]
-        )
-        availability = ";".join(
-            self.search_tree.config.stock.availability_string(mol)
-            for mol in top_route.leafs()
-        )
-
-        return {
-            "number_of_nodes": len(self.search_tree.mol_nodes),
-            "max_transforms": max(
-                node.prop["mol"].transform for node in self.search_tree.mol_nodes
-            ),
-            "max_children": max(
-                len(node.children) for node in self.search_tree.mol_nodes
-            ),
-            "number_of_routes": len(all_routes),
-            "number_of_solved_routes": sum(route.is_solved for route in all_routes),
-            "top_score": self.scorer(top_route),
-            "is_solved": top_route.is_solved,
-            "number_of_steps": len(list(top_route.reactions())),
-            "number_of_precursors": len(list(top_route.leafs())),
-            "number_of_precursors_in_stock": sum(
-                top_route.in_stock(leaf) for leaf in top_route.leafs()
-            ),
-            "precursors_in_stock": mols_in_stock,
-            "precursors_not_in_stock": mols_not_in_stock,
-            "precursors_availability": availability,
-            "policy_used_counts": policy_used_counts,
-            "profiling": getattr(self.search_tree, "profiling", {}),
-        }
+    _collection_name = "stock"
 
-    def _tree_statistics_mcts(self) -> StrDict:
-        assert isinstance(self.search_tree, MctsSearchTree)
-        top_node = self.best()
-        assert isinstance(top_node, MctsNode)
-        top_state = top_node.state
-        nodes = list(self.search_tree.graph())
-        mols_in_stock = ", ".join(
-            mol.smiles
-            for mol, instock in zip(top_state.mols, top_state.in_stock_list)
-            if instock
-        )
-        mols_not_in_stock = ", ".join(
-            mol.smiles
-            for mol, instock in zip(top_state.mols, top_state.in_stock_list)
-            if not instock
-        )
-
-        policy_used_counts = self._policy_used_statistics(
-            [node[child]["action"] for node in nodes for child in node.children]
-        )
-
-        return {
-            "number_of_nodes": len(nodes),
-            "max_transforms": max(node.state.max_transforms for node in nodes),
-            "max_children": max(len(node.children) for node in nodes),
-            "number_of_routes": sum(1 for node in nodes if not node.children),
-            "number_of_solved_routes": sum(
-                1 for node in nodes if not node.children and node.state.is_solved
-            ),
-            "top_score": self.scorer(top_node),
-            "is_solved": top_state.is_solved,
-            "number_of_steps": top_state.max_transforms,
-            "number_of_precursors": len(top_state.mols),
-            "number_of_precursors_in_stock": sum(top_state.in_stock_list),
-            "precursors_in_stock": mols_in_stock,
-            "precursors_not_in_stock": mols_not_in_stock,
-            "precursors_availability": ";".join(top_state.stock_availability),
-            "policy_used_counts": policy_used_counts,
-            "profiling": getattr(self.search_tree, "profiling", {}),
-        }
+    def __init__(self) -> None:
+        super().__init__()
+        self._exclude: Set[str] = set()
+        self._stop_criteria: StrDict = {"amount": None, "price": None, "counts": {}}
+        self._use_stop_criteria: bool = False
+
+    def __contains__(self, mol: Molecule) -> bool:
+        if not self.selection or mol.inchi_key in self._exclude:
+            return False
+
+        if self._use_stop_criteria:
+            return self._apply_stop_criteria(mol)
+
+        for key in self.selection:
+            if mol in self[key]:
+                return True
+        return False
+
+    def __len__(self) -> int:
+        return sum(len(self[key]) for key in self.selection or [])
+
+    @property
+    def stop_criteria(self) -> dict:
+        """Return a copy of the stop criteria used by the stock"""
+        return copy.deepcopy(self._stop_criteria)
+
+    def amount(self, mol: Molecule) -> float:
+        """
+        Calculate the maximum amount of a molecule in stock
+
+        :param mol: the molecule to query
+        :raises StockException: if the amount could not be computed
+        :return: the maximum amount
+        """
+        amounts = self._mol_property(mol, "amount")
+        if not amounts:
+            raise StockException("Could not obtain amount of molecule")
+        return max(amounts)
+
+    def availability_list(self, mol: Molecule) -> List[str]:
+        """
+        Return a list of what stocks a given mol is available
 
-    @staticmethod
-    def _collect_top_items(
-        items: Union[Sequence[MctsNode], Sequence[ReactionTree]],
-        scores: Sequence[float],
-        reactions: Sequence[
-            Union[Iterable[RetroReaction], Iterable[FixedRetroReaction]]
-        ],
-        selection,
-    ) -> Tuple[Union[Sequence[MctsNode], Sequence[ReactionTree]], Sequence[float]]:
-        if len(items) <= selection.nmin:
-            return items, scores
-
-        max_return, min_return = selection.nmax, selection.nmin
-        if selection.return_all:
-            nsolved = sum(int(item.is_solved) for item in items)
-            if nsolved:
-                max_return = nsolved
-                min_return = nsolved
-
-        seen_hashes = set()
-        best_items: List[Any] = []
-        best_scores = []
-        last_score = 1e16
-        for score, item, actions in zip(scores, items, reactions):
-            if len(best_items) >= min_return and score < last_score:
-                break
-            route_hash = hash_reactions(actions)
+        If the molecule is not in stock it will return any empty list
 
-            if route_hash in seen_hashes:
+        :param mol: The molecule to query
+        :returns: string with a list of stocks that mol was found in
+        """
+        availability = []
+        for key in self.selection or []:
+            if mol not in self[key]:
                 continue
-            seen_hashes.add(route_hash)
-            best_items.append(item)
-            best_scores.append(score)
-            last_score = score
-
-            if max_return and len(best_items) == max_return:
-                break
-
-        return best_items, best_scores
-
-    @staticmethod
-    def _policy_used_statistics(
-        reactions: Iterable[Union[RetroReaction, FixedRetroReaction]]
-    ) -> StrDict:
-        policy_used_counts: StrDict = defaultdict(lambda: 0)
-        for reaction in reactions:
-            policy_used = reaction.metadata.get("policy_name")
-            if policy_used:
-                policy_used_counts[policy_used] += 1
-        return dict(policy_used_counts)
+            try:
+                availability.extend(self[key].availability_string(mol).split(","))
+            except (StockException, AttributeError):
+                availability.append(key)
+        return sorted(list(set(availability)))
+
+    def availability_string(self, mol: Molecule) -> str:
+        """
+        Return a string of what stocks a given mol is available
+
+        If the molecule is not in stock it will return "Not in stock"
+
+        :param mol: The molecule to query
+        :returns: string with a list of stocks that mol was found in
+        """
+        availability = self.availability_list(mol)
+        if availability:
+            return ",".join(availability)
+        return "Not in stock"
+
+    def exclude(self, mol: Molecule) -> None:
+        """
+        Exclude a molecule from the stock.
+        When this molecule is queried it will return False,
+        regardless if the molecule is in the stock.
+
+        :param mol: the molecule to exclude
+        """
+        self._exclude.add(mol.inchi_key)
+
+    def load(self, source: StockQueryMixin, key: str) -> None:  # type: ignore
+        """
+        Add a pre-initialized stock query object to the stock
+
+        :param source: the item to add
+        :param key: The key that will be used to select the stock
+        """
+        if not isinstance(source, StockQueryMixin):
+            raise StockException(
+                "Only objects of classes inherited from StockQueryMixin can be added"
+            )
+
+        self._logger.info(f"Loading stock from {source.__class__.__name__} to {key}")
+        self._items[key] = source
+
+    def load_from_config(self, **config: Any) -> None:
+        """
+        Load one or more stock queries from a configuration
+
+        The key can be "stop_criteria" in case the config is given to the
+        `set_stop_criteria` method
+
+        The format should be
+        key:
+            type: name of the stock class or custom_package.custom_model.CustomClass
+            path: path to the stock file
+            other settings or params
+        or
+        key: path_to_model
+
+        :param config: the configuration
+        """
+        if "stop_criteria" in config:
+            self.set_stop_criteria(config["stop_criteria"])
+
+        for key, stock_config in config.items():
+            if key == "stop_criteria":
+                continue
+
+            if not isinstance(stock_config, dict):
+                kwargs = {"path": stock_config}
+                if stock_config.endswith(".bloom"):
+                    cls: Any = MolbloomFilterQuery
+                else:
+                    cls = InMemoryInchiKeyQuery
+            else:
+                if "type" not in stock_config or stock_config["type"] == "inchiset":
+                    cls = InMemoryInchiKeyQuery
+                else:
+                    stock_query = STOCK_QUERY_ALIAS.get(
+                        stock_config["type"], stock_config["type"]
+                    )
+                    cls = load_dynamic_class(
+                        stock_query, queries_module, StockException
+                    )
+                kwargs = dict(stock_config)
+
+            if "type" in kwargs:
+                del kwargs["type"]
+            obj = cls(**kwargs)
+            self.load(obj, key)
+
+    def price(self, mol: Molecule) -> float:
+        """
+        Calculate the minimum price of a molecule in stock
+
+        :param mol: the molecule to query
+        :raises StockException: if the price could not be computed
+        :return: the minimum price
+        """
+        prices = self._mol_property(mol, "price")
+        if not prices:
+            raise StockException("Could not obtain price of molecule")
+        return min(prices)
+
+    def reset_exclusion_list(self) -> None:
+        """Remove all molecules in the exclusion list"""
+        self._exclude = set()
+
+    def select(self, value: Union[str, List[str]], append: bool = False) -> None:
+        """
+        Select one or more stock queries
+
+        :param value: the key of the stocks to select
+        :param append: if True and ``value`` is a single key append it to the current selection
+        """
+        super().select(value, append)
+        try:
+            self._logger.info(f"Compounds in stock: {len(self)}")
+        except (TypeError, ValueError):  # In case len is not possible to compute
+            pass
+
+    def set_stop_criteria(self, criteria: Optional[Dict] = None) -> None:
+        """
+        Set criteria that stop the search
+
+        The keys of the criteria can be "price" or "amount" which accepts numerical settings,
+        or "counts" that should be dictionary of maximum allowed count for each atomic symbol.
+
+        Example:
+
+        .. code-block::
+
+            criteria = {
+                "price": 5,
+                "amount": 100,
+                "counts": {
+                    "C": 6,
+                    "O": 4
+                }
+            }
+
+        :param criteria: the criteria settings
+        """
+        criteria = criteria or {}
+        self._stop_criteria = {
+            "price": criteria.get("price"),
+            "amount": criteria.get("amount"),
+            "counts": copy.deepcopy(criteria.get("size", criteria.get("counts"))),
+        }
+        self._use_stop_criteria = any(self._stop_criteria.values())
+        reduced_criteria = {
+            key: value for key, value in self._stop_criteria.items() if value
+        }
+        self._logger.info(f"Stop criteria for stock updated to: {reduced_criteria}")
+
+    def smiles_in_stock(self, smiles: str) -> bool:
+        """
+        Check if the SMILES is in the currently selected stocks
+
+        :param smiles: SMILES string (must be RDKit sanitizable)
+        :returns: if the SMILES was on stock
+        """
+        return Molecule(smiles=smiles) in self
+
+    def _apply_amount_criteria(self, mol: Molecule) -> bool:
+        if not self._stop_criteria["amount"]:
+            return True
+        try:
+            amount = self.amount(mol)
+        except StockException:
+            return True
+        return amount >= self._stop_criteria.get("amount", amount)
+
+    def _apply_counts_criteria(self, mol: Molecule) -> bool:
+        if not self._stop_criteria["counts"]:
+            return True
+        atom_counts: dict = defaultdict(int)
+        for atom in mol.rd_mol.GetAtoms():
+            atom_counts[atom.GetSymbol()] += 1
+        for symbol, threshold in self._stop_criteria["counts"].items():
+            if atom_counts[symbol] > threshold:
+                return False
+        return True
+
+    def _apply_price_criteria(self, mol: Molecule) -> bool:
+        if not self._stop_criteria["price"]:
+            return True
+        try:
+            price = self.price(mol)
+        except StockException:
+            return True
+        return price <= self._stop_criteria.get("price", price)
+
+    def _apply_stop_criteria(self, mol: Molecule) -> bool:
+        if not self._apply_counts_criteria(mol):
+            return False
+
+        passes = False
+        for key in self.selection or []:
+            passes = passes or self[key].cached_search(mol)
+        passes = passes and self._apply_amount_criteria(mol)
+        passes = passes and self._apply_price_criteria(mol)
+
+        for key in self.selection or []:
+            self[key].clear_cache()
+        return passes
+
+    def _mol_property(self, mol, property_name):
+        values = []
+        for key in self.selection:
+            try:
+                func = getattr(self[key], property_name)
+                values.append(func(mol))
+            except StockException:
+                pass
+        return values
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/analysis/utils.py` & `aizynthfinder-4.3.0/aizynthfinder/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/chem/mol.py` & `aizynthfinder-4.3.0/aizynthfinder/chem/mol.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 from rdkit import Chem, DataStructs
 from rdkit.Chem import AllChem, Descriptors
 
+from aizynthfinder.utils.bonds import sort_bonds
 from aizynthfinder.utils.exceptions import MoleculeException
 
 if TYPE_CHECKING:
     from aizynthfinder.utils.type_utils import (
         Callable,
         Dict,
         List,
@@ -316,14 +317,38 @@
 
         self._atom_bonds = [
             (self.index_to_mapping[atom_index1], self.index_to_mapping[atom_index2])
             for atom_index1, atom_index2 in bonds
         ]
         return self._atom_bonds
 
+    def get_bonds_in_molecule(
+        self, query_bonds: Sequence[Sequence[int]]
+    ) -> Sequence[Sequence[int]]:
+        """
+        Get bonds (from a list of bonds) that are present in the molecule.
+        :param bonds: List of bond (atom pairs)
+        :return: A list of bonds
+        """
+        molecule_bonds = sort_bonds(self.mapped_atom_bonds)
+        query_bonds = sort_bonds(query_bonds)
+        bonds_in_mol = [bond for bond in query_bonds if bond in molecule_bonds]
+        return bonds_in_mol
+
+    def has_all_focussed_bonds(self, bonds: Sequence[Sequence[int]]) -> bool:
+        """Checks that the focussed bonds exist in the target molecule's atom bonds.
+
+        :param bonds: Focussed bonds.
+        :param target_mol: The target molecule.
+
+        :return: A boolean indicating if the input bonds exist in the target molecule.
+        """
+        bonds_in_mol = self.get_bonds_in_molecule(bonds)
+        return len(bonds_in_mol) == len(bonds)
+
     def _set_atom_mappings(self) -> None:
         atom_mappings = [
             atom.GetAtomMapNum()
             for atom in self.mapped_mol.GetAtoms()
             if atom.GetAtomMapNum() != 0
         ]
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/chem/reaction.py` & `aizynthfinder-4.3.0/aizynthfinder/chem/reaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,22 @@
 import abc
 import hashlib
 from functools import partial
 from typing import TYPE_CHECKING
 
 import numpy as np
 from rdchiral import main as rdc
-from rdchiral.bonds import get_atoms_across_double_bonds
-from rdchiral.initialization import BondDirOpposite
+
+try:
+    from rdchiral.bonds import get_atoms_across_double_bonds
+    from rdchiral.initialization import BondDirOpposite
+except ImportError:
+    RDCHIRAL_CPP = True
+else:
+    RDCHIRAL_CPP = False
 from rdkit import Chem
 from rdkit.Chem import AllChem
 from rdkit.Chem.rdchem import BondDir, BondStereo, ChiralType
 
 from aizynthfinder.chem.mol import (
     Molecule,
     MoleculeException,
@@ -32,14 +38,19 @@
         RdReaction,
         Set,
         StrDict,
         Tuple,
         Union,
     )
 
+if RDCHIRAL_CPP:
+    logger().warning(
+        "WARNING: C++ version of RDChiral is supported, but with limited functionality"
+    )
+
 
 class _ReactionInterfaceMixin:
     """
     Mixin class to define a common interface for all reaction class
 
     The methods `_products_getter` and `_reactants_getter` needs to be implemented by subclasses
     """
@@ -98,15 +109,15 @@
         """
         Get the reaction SMILES, i.e. the SMILES of the reactants and products joined together
 
         :return: the SMILES
         """
         reactants = ".".join(mol.smiles for mol in self._reactants_getter())  # type: ignore
         products = ".".join(mol.smiles for mol in self._products_getter())  # type: ignore
-        return "%s>>%s" % (reactants, products)
+        return f"{reactants}>>{products}"
 
 
 class RetroReaction(abc.ABC, _ReactionInterfaceMixin):
     """
     A retrosynthesis reaction. Only a single molecule is the reactant.
 
     This is an abstract class and child classes needs to implement the `_apply` and `_make_smiles` functions
@@ -627,7 +638,15 @@
         for i, j, b in self.bonds_by_mapnum:
             if b.GetBondDir() != BondDir.NONE:
                 self.bond_dirs_by_mapnum[(i, j)] = b.GetBondDir()
                 self.bond_dirs_by_mapnum[(j, i)] = BondDirOpposite[b.GetBondDir()]
 
         # Get atoms across double bonds defined by mapnum
         self.atoms_across_double_bonds = get_atoms_across_double_bonds(self.reactants)
+
+
+if RDCHIRAL_CPP:
+
+    def _wrapper(mol):
+        return rdc.rdchiralReactants(mol.mapped_smiles)
+
+    _RdChiralProductWrapper = _wrapper  # type: ignore
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/chem/serialization.py` & `aizynthfinder-4.3.0/aizynthfinder/chem/serialization.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/context/collection.py` & `aizynthfinder-4.3.0/aizynthfinder/context/collection.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/context/config.py` & `aizynthfinder-4.3.0/aizynthfinder/context/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import os
 import re
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING
 
 import yaml
+
 from aizynthfinder.context.policy import ExpansionPolicy, FilterPolicy
 from aizynthfinder.context.scoring import ScorerCollection
 from aizynthfinder.context.stock import Stock
 from aizynthfinder.utils.logging import logger
 
 if TYPE_CHECKING:
     from aizynthfinder.utils.type_utils import Any, Dict, List, Optional, StrDict, Union
@@ -19,29 +20,31 @@
 
 @dataclass
 class _PostprocessingConfiguration:
     min_routes: int = 5
     max_routes: int = 25
     all_routes: bool = False
     route_distance_model: Optional[str] = None
-    route_scorer: str = "state score"
+    route_scorers: List[str] = field(default_factory=lambda: [])
+    scorer_weights: Optional[List[float]] = field(default_factory=lambda: None)
 
 
 @dataclass
 class _SearchConfiguration:
     algorithm: str = "mcts"
     algorithm_config: Dict[str, Any] = field(
         default_factory=lambda: {
             "C": 1.4,
             "default_prior": 0.5,
             "use_prior": True,
             "prune_cycles_in_search": True,
-            "search_reward": "state score",
+            "search_rewards": ["state score"],
             "immediate_instantiation": (),
             "mcts_grouping": None,
+            "search_rewards_weights": [],
         }
     )
     max_transforms: int = 6
     iteration_limit: int = 100
     time_limit: int = 120
     return_first: bool = False
     exclude_target_from_stock: bool = True
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/context/policy/expansion_strategies.py` & `aizynthfinder-4.3.0/aizynthfinder/context/policy/expansion_strategies.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 """ Module containing classes that implements different expansion policy strategies
 """
+
 from __future__ import annotations
 
 import abc
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 
-from aizynthfinder.chem import TemplatedRetroReaction
+from aizynthfinder.chem import SmilesBasedRetroReaction, TemplatedRetroReaction
 from aizynthfinder.context.policy.utils import _make_fingerprint
 from aizynthfinder.utils.exceptions import PolicyException
 from aizynthfinder.utils.logging import logger
 from aizynthfinder.utils.models import load_model
-from aizynthfinder.utils.math import softmax
 
 if TYPE_CHECKING:
     from aizynthfinder.chem import TreeMolecule
     from aizynthfinder.chem.reaction import RetroReaction
     from aizynthfinder.context.config import Configuration
-    from aizynthfinder.utils.type_utils import Any, Dict, List, Sequence, Tuple
+    from aizynthfinder.utils.type_utils import (
+        Any,
+        Dict,
+        List,
+        Optional,
+        Sequence,
+        StrDict,
+        Tuple,
+    )
 
 
 class ExpansionStrategy(abc.ABC):
     """
     A base class for all expansion strategies.
 
     The strategy can be used by either calling the `get_actions` method
@@ -50,23 +58,23 @@
         self._config = config
         self._logger = logger()
         self.key = key
 
     def __call__(
         self,
         molecules: Sequence[TreeMolecule],
-        cache_molecules: Sequence[TreeMolecule] = None,
+        cache_molecules: Optional[Sequence[TreeMolecule]] = None,
     ) -> Tuple[List[RetroReaction], List[float]]:
         return self.get_actions(molecules, cache_molecules)
 
     @abc.abstractmethod
     def get_actions(
         self,
         molecules: Sequence[TreeMolecule],
-        cache_molecules: Sequence[TreeMolecule] = None,
+        cache_molecules: Optional[Sequence[TreeMolecule]] = None,
     ) -> Tuple[List[RetroReaction], List[float]]:
         """
         Get all the probable actions of a set of molecules
 
         :param molecules: the molecules to consider
         :param cache_molecules: additional molecules to submit to the expansion
                                   policy but that only will be cached for later use
@@ -84,91 +92,177 @@
     The strategy can be used by either calling the `get_actions` method
     or by calling the instantiated class with a list of molecules.
 
     :ivar expansion_strategy_keys: the keys of the selected expansion strategies
     :ivar additive_expansion: a conditional setting to specify whether all the actions
         and priors of the selected expansion strategies should be combined or not.
         Defaults to False.
+    :ivar expansion_strategy_weights: a list of weights for each expansion strategy.
+        The weights should sum to one. Exception is the default, where unity weight
+        is associated to each strategy.
 
     :param key: the key or label
     :param config: the configuration of the tree search
     :param expansion_strategies: the keys of the selected expansion strategies. All keys
         of the selected expansion strategies must exist in the expansion policies listed
         in config
     """
 
     _required_kwargs = ["expansion_strategies"]
 
     def __init__(
         self,
         key: str,
         config: Configuration,
-        **kwargs: str,
+        **kwargs: Any,
     ) -> None:
         super().__init__(key, config, **kwargs)
         self._config = config
+        self._expansion_strategies: List[ExpansionStrategy] = []
         self.expansion_strategy_keys = kwargs["expansion_strategies"]
+
+        self.cutoff_number = kwargs.get("cutoff_number")
+        if self.cutoff_number:
+            print(f"Setting multi-expansion cutoff_number: {self.cutoff_number}")
+
+        self.expansion_strategy_weights = self._set_expansion_strategy_weights(kwargs)
         self.additive_expansion: bool = bool(kwargs.get("additive_expansion", False))
+        self._logger.info(
+            f"Multi-expansion strategy with policies: {self.expansion_strategy_keys}"
+            f", and corresponding weights: {self.expansion_strategy_weights}"
+        )
 
     def get_actions(
         self,
         molecules: Sequence[TreeMolecule],
-        cache_molecules: Sequence[TreeMolecule] = None,
+        cache_molecules: Optional[Sequence[TreeMolecule]] = None,
     ) -> Tuple[List[RetroReaction], List[float]]:
         """
         Get all the probable actions of a set of molecules, using the selected policies.
 
         The default implementation combines all the actions and priors of the
         selected expansion strategies into two lists respectively if the
         'additive_expansion' setting is set to True. This function can be overridden by
         a sub class to combine different expansion strategies in different ways.
 
         :param molecules: the molecules to consider
+        :param cache_molecules: additional molecules to submit to the expansion
+            policy but that only will be cached for later use
         :return: the actions and the priors of those actions
         :raises: PolicyException: if the policy isn't selected
         """
         expansion_strategies = self._get_expansion_strategies_from_config()
 
         all_possible_actions = []
         all_priors = []
-        for expansion_strategy in expansion_strategies:
+        for expansion_strategy, expansion_strategy_weight in zip(
+            expansion_strategies, self.expansion_strategy_weights
+        ):
             possible_actions, priors = expansion_strategy.get_actions(
                 molecules, cache_molecules
             )
+
             all_possible_actions.extend(possible_actions)
-            all_priors.extend(priors)
             if not self.additive_expansion and all_possible_actions:
+                all_priors.extend(priors)
                 break
+
+            weighted_prior = [expansion_strategy_weight * p for p in priors]
+
+            all_priors.extend(weighted_prior)
+
+        all_possible_actions, all_priors = self._prune_actions(
+            all_possible_actions, all_priors
+        )
         return all_possible_actions, all_priors
 
     def _get_expansion_strategies_from_config(self) -> List[ExpansionStrategy]:
+        if self._expansion_strategies:
+            return self._expansion_strategies
+
         if not all(
             key in self._config.expansion_policy.items
             for key in self.expansion_strategy_keys
         ):
             raise ValueError(
                 "The input expansion strategy keys must exist in the "
                 "expansion policies listed in config"
             )
-        return [
+        self._expansion_strategies = [
             self._config.expansion_policy[key] for key in self.expansion_strategy_keys
         ]
 
+        for expansion_strategy, weight in zip(
+            self._expansion_strategies, self.expansion_strategy_weights
+        ):
+            if not getattr(expansion_strategy, "rescale_prior", True) and weight < 1:
+                setattr(expansion_strategy, "rescale_prior", True)
+                self._logger.info(
+                    f"Enforcing {expansion_strategy.key}.rescale_prior=True"
+                )
+        return self._expansion_strategies
+
+    def _prune_actions(
+        self, actions: List[RetroReaction], priors: List[float]
+    ) -> Tuple[List[RetroReaction], List[float]]:
+        """
+        Prune the actions if a maximum number of actions is specified.
+
+        :param actions: list of predicted actions
+        :param priors: list of prediction probabilities
+        :return: the top 'self.cutoff_number' actions and corresponding priors.
+        """
+        if not self.cutoff_number:
+            return actions, priors
+
+        sortidx = np.argsort(np.array(priors))[::-1].astype(int)
+        priors = [priors[idx] for idx in sortidx[0 : self.cutoff_number]]
+        actions = [actions[idx] for idx in sortidx[0 : self.cutoff_number]]
+        return actions, priors
+
+    def _set_expansion_strategy_weights(self, kwargs: StrDict) -> List[float]:
+        """
+        Set the weights of each expansion strategy using the input kwargs from config.
+        The weights in the config should sum to one.
+        If not set in the config file, the weights default to one for each strategy
+        (for backwards compatibility).
+
+        :param kwargs: input arguments to the MultiExpansionStrategy
+        :raises: ValueError if weights from the config file do not sum to one.
+        :return: a list of expansion strategy weights
+        """
+        if not "expansion_strategy_weights" in kwargs:
+            return [1.0 for _ in self.expansion_strategy_keys]
+
+        expansion_strategy_weights = kwargs["expansion_strategy_weights"]
+        sum_weights = sum(expansion_strategy_weights)
+
+        if sum_weights != 1:
+            raise ValueError(
+                "The expansion strategy weights in MultiExpansion should "
+                "sum to one. -> "
+                f"sum({expansion_strategy_weights})={sum_weights}."
+            )
+
+        return expansion_strategy_weights
+
 
 class TemplateBasedExpansionStrategy(ExpansionStrategy):
     """
     A template-based expansion strategy that will return `TemplatedRetroReaction` objects upon expansion.
 
     :ivar template_column: the column in the template file that contains the templates
     :ivar cutoff_cumulative: the accumulative probability of the suggested templates
     :ivar cutoff_number: the maximum number of templates to returned
     :ivar use_rdchiral: a boolean to apply templates with RDChiral
     :ivar use_remote_models: a boolean to connect to remote TensorFlow servers
     :ivar rescale_prior: a boolean to apply softmax to the priors
     :ivar chiral_fingerprints: if True will base expansion on chiral fingerprint
+    :ivar mask: a boolean vector of masks for the reaction templates. The length of the vector should be equal to the
+        number of templates. It is set to None if no mask file is provided as input.
 
     :param key: the key or label
     :param config: the configuration of the tree search
     :param model: the source of the policy model
     :param template: the path to a HDF5 file with the templates
     :raises PolicyException: if the length of the model output vector is not same as the
         number of templates
@@ -180,14 +274,15 @@
     ]
 
     def __init__(self, key: str, config: Configuration, **kwargs: str) -> None:
         super().__init__(key, config, **kwargs)
 
         source = kwargs["model"]
         templatefile = kwargs["template"]
+        maskfile: str = kwargs.get("mask", "")
         self.template_column: str = kwargs.get("template_column", "retro_template")
         self.cutoff_cumulative: float = float(kwargs.get("cutoff_cumulative", 0.995))
         self.cutoff_number: int = int(kwargs.get("cutoff_number", 50))
         self.use_rdchiral: bool = bool(kwargs.get("use_rdchiral", True))
         self.use_remote_models: bool = bool(kwargs.get("use_remote_models", False))
         self.rescale_prior: bool = bool(kwargs.get("rescale_prior", False))
         self.chiral_fingerprints = bool(kwargs.get("chiral_fingerprints", False))
@@ -201,26 +296,29 @@
         if templatefile.endswith(".csv.gz") or templatefile.endswith(".csv"):
             self.templates: pd.DataFrame = pd.read_csv(
                 templatefile, index_col=0, sep="\t"
             )
         else:
             self.templates = pd.read_hdf(templatefile, "table")
 
+        self.mask: Optional[np.ndarray] = (
+            self._load_mask_file(maskfile) if maskfile else None
+        )
+
         if hasattr(self.model, "output_size") and len(self.templates) != self.model.output_size:  # type: ignore
             raise PolicyException(
                 f"The number of templates ({len(self.templates)}) does not agree with the "  # type: ignore
                 f"output dimensions of the model ({self.model.output_size})"
             )
         self._cache: Dict[str, Tuple[np.ndarray, np.ndarray]] = {}
 
-    # pylint: disable=R0914
     def get_actions(
         self,
         molecules: Sequence[TreeMolecule],
-        cache_molecules: Sequence[TreeMolecule] = None,
+        cache_molecules: Optional[Sequence[TreeMolecule]] = None,
     ) -> Tuple[List[RetroReaction], List[float]]:
         """
         Get all the probable actions of a set of molecules, using the selected policies and given cutoffs
 
         :param molecules: the molecules to consider
         :param cache_molecules: additional molecules to submit to the expansion
                                   policy but that only will be cached for later use
@@ -232,15 +330,15 @@
         cache_molecules = cache_molecules or []
         self._update_cache(list(molecules) + list(cache_molecules))
 
         for mol in molecules:
             probable_transforms_idx, probs = self._cache[mol.inchi_key]
             possible_moves = self.templates.iloc[probable_transforms_idx]
             if self.rescale_prior:
-                probs = softmax(probs)
+                probs /= probs.sum()
             priors.extend(probs)
             for idx, (move_index, move) in enumerate(possible_moves.iterrows()):
                 metadata = dict(move)
                 del metadata[self.template_column]
                 metadata["policy_probability"] = float(probs[idx].round(4))
                 metadata["policy_probability_rank"] = idx
                 metadata["policy_name"] = self.key
@@ -262,23 +360,34 @@
 
     def _cutoff_predictions(self, predictions: np.ndarray) -> np.ndarray:
         """
         Get the top transformations, by selecting those that have:
             * cumulative probability less than a threshold (cutoff_cumulative)
             * or at most N (cutoff_number)
         """
+        if self.mask is not None:
+            predictions[~self.mask] = 0
         sortidx = np.argsort(predictions)[::-1]
         cumsum: np.ndarray = np.cumsum(predictions[sortidx])
         if any(cumsum >= self.cutoff_cumulative):
             maxidx = int(np.argmin(cumsum < self.cutoff_cumulative))
         else:
             maxidx = len(cumsum)
         maxidx = min(maxidx, self.cutoff_number) or 1
         return sortidx[:maxidx]
 
+    def _load_mask_file(self, maskfile: str) -> np.ndarray:
+        self._logger.info(f"Loading masking of templates from {maskfile} to {self.key}")
+        mask = np.load(maskfile)["arr_0"]
+        if len(mask) != len(self.templates):
+            raise PolicyException(
+                f"The number of masks {len(mask)} does not match the number of templates {len(self.templates)}"
+            )
+        return mask
+
     def _update_cache(self, molecules: Sequence[TreeMolecule]) -> None:
         pred_inchis = []
         fp_list = []
         for molecule in molecules:
             if molecule.inchi_key in self._cache or molecule.inchi_key in pred_inchis:
                 continue
             fp_list.append(
@@ -292,7 +401,50 @@
         pred_list = np.asarray(self.model.predict(np.vstack(fp_list)))
         for pred, inchi in zip(pred_list, pred_inchis):
             probable_transforms_idx = self._cutoff_predictions(pred)
             self._cache[inchi] = (
                 probable_transforms_idx,
                 pred[probable_transforms_idx],
             )
+
+
+class TemplateBasedDirectExpansionStrategy(TemplateBasedExpansionStrategy):
+    """
+    A template-based expansion strategy that will return `SmilesBasedRetroReaction` objects upon expansion
+    by directly applying the template
+
+    :param key: the key or label
+    :param config: the configuration of the tree search
+    :param source: the source of the policy model
+    :param templatefile: the path to a HDF5 file with the templates
+    :raises PolicyException: if the length of the model output vector is not same as the number of templates
+    """
+
+    def get_actions(
+        self,
+        molecules: Sequence[TreeMolecule],
+        cache_molecules: Optional[Sequence[TreeMolecule]] = None,
+    ) -> Tuple[List[RetroReaction], List[float]]:
+        """
+        Get all the probable actions of a set of molecules, using the selected policies and given cutoffs
+
+        :param molecules: the molecules to consider
+        :param cache_molecules: additional molecules to submit to the expansion
+            policy but that only will be cached for later use
+        :return: the actions and the priors of those actions
+        """
+        possible_actions = []
+        priors = []
+
+        super_actions, super_priors = super().get_actions(molecules, cache_molecules)
+        for templated_action, prior in zip(super_actions, super_priors):
+            for reactants in templated_action.reactants:
+                reactants_str = ".".join(mol.smiles for mol in reactants)
+                new_action = SmilesBasedRetroReaction(
+                    templated_action.mol,
+                    metadata=templated_action.metadata,
+                    reactants_str=reactants_str,
+                )
+                possible_actions.append(new_action)
+                priors.append(prior)
+
+        return possible_actions, priors  # type: ignore
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/context/policy/filter_strategies.py` & `aizynthfinder-4.3.0/aizynthfinder/context/policy/filter_strategies.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,22 +5,26 @@
 import abc
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from aizynthfinder.chem import TemplatedRetroReaction
 from aizynthfinder.context.policy.utils import _make_fingerprint
-from aizynthfinder.utils.exceptions import PolicyException, RejectionException
+from aizynthfinder.utils.bonds import BrokenBonds
+from aizynthfinder.utils.exceptions import (
+    PolicyException,
+    RejectionException,
+)
 from aizynthfinder.utils.logging import logger
 from aizynthfinder.utils.models import load_model
 
 if TYPE_CHECKING:
     from aizynthfinder.chem.reaction import RetroReaction
     from aizynthfinder.context.config import Configuration
-    from aizynthfinder.utils.type_utils import Any, List, Tuple
+    from aizynthfinder.utils.type_utils import Any, Dict, List, Optional, Tuple
 
 
 class FilterStrategy(abc.ABC):
     """
     A base class for all filter strategies.
 
     The filter can be applied by either calling the `apply` method
@@ -58,14 +62,41 @@
         should be rejected a `RejectionException` is raised
 
         :param reaction: the reaction to filter
         :raises: if the reaction should be rejected.
         """
 
 
+class BondFilter(FilterStrategy):
+    """
+    Check if focussed bonds to freeze stay frozen in a reaction.
+
+    :param key: the key or label
+    :param config: the configuration of the tree search
+    """
+
+    def __init__(self, key: str, config: Configuration, **kwargs: Any) -> None:
+        super().__init__(key, config, **kwargs)
+
+        self._freeze_bonds = config.search.freeze_bonds
+        self._broken_bonds = BrokenBonds(self._freeze_bonds)
+        self._logger.info(
+            f"Loading bond filter to {key} with {len(self._freeze_bonds)} "
+            "bonds to freeze"
+        )
+
+    def apply(self, reaction: RetroReaction) -> None:
+        broken_frozen_bonds = self._broken_bonds(reaction)
+        if len(broken_frozen_bonds) > 0:
+            raise RejectionException(
+                f"{reaction} was filtered out as the focussed bonds "
+                f"'{broken_frozen_bonds}' were found to be broken in the reaction"
+            )
+
+
 class QuickKerasFilter(FilterStrategy):
     """
     Filter quick-filter trained on artificial negative data
 
     :ivar use_remote_models: a boolean to connect to remote TensorFlow servers. Defaults
         to False.
     :ivar filter_cutoff: the cut-off value
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/context/policy/policies.py` & `aizynthfinder-4.3.0/aizynthfinder/context/policy/policies.py`

 * *Files 5% similar despite different names*

```diff
@@ -218,7 +218,16 @@
                     )
                 kwargs = dict(strategy_config)
 
             if "type" in kwargs:
                 del kwargs["type"]
             obj = cls(key, self._config, **kwargs)
             self.load(obj)
+
+    def reset_cache(self) -> None:
+        """Reset filtering cache."""
+        if not self.selection:
+            return
+
+        for name in self.selection:
+            if hasattr(self[name], "reset_cache"):
+                self[name].reset_cache()
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/context/policy/utils.py` & `aizynthfinder-4.3.0/aizynthfinder/context/policy/utils.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/context/scoring/collection.py` & `aizynthfinder-4.3.0/aizynthfinder/context/scoring/collection.py`

 * *Files 23% similar despite different names*

```diff
@@ -57,32 +57,41 @@
     _collection_name = "scorer"
 
     def __init__(self, config: Configuration) -> None:
         super().__init__()
         self._config = config
         self.create_default_scorers()
 
+    def __repr__(self) -> str:
+        if self.selection:
+            return f"{self._collection_name} ({', '.join(self.selection)})"
+
+        return f"{self._collection_name} ({', '.join(self.items)})"
+
     def create_default_scorers(self) -> None:
         """
         Setup the scores that only need the config as their input.
         """
         for cls in _SIMPLE_SCORERS:
-            self.load(cls(self._config))
+            self.load(cls(self._config), silent=True)
 
-    def load(self, scorer: Scorer) -> None:  # type: ignore
+    def load(self, scorer: Scorer, silent: bool = False) -> None:  # type: ignore
         """
         Add a pre-initialized scorer object to the collection
 
         :param scorer: the item to add
+        :param silent: if True will not write out the name of the loaded scorer
         """
         if not isinstance(scorer, Scorer):
             raise ScorerException(
                 "Only objects of classes inherited from Scorer can be added"
             )
         self._items[repr(scorer)] = scorer
+        if not silent:
+            self._logger.info(f"Loaded scorer: {repr(scorer)}")
 
     def load_from_config(self, **scorers_config: Any) -> None:
         """
         Load one or several scorers from a configuration dictionary
 
         The keys are the name of scorer class. If a scorer is not
         defined in the ``aizynthfinder.context.scoring`` module, the module
@@ -115,15 +124,16 @@
         for name in new_collection.names():
             del new_collection[name]
         for name in subset_names:
             try:
                 scorer = self._items[name]
             except KeyError:
                 raise ScorerException(f"Unable to find '{name}' in parent collection")
-            new_collection.load(scorer)
+            new_collection.load(scorer, silent=True)
+            new_collection.select(name, append=True)
         return new_collection
 
     def names(self) -> List[str]:
         """Return a list of the names of all the loaded scorers"""
         return self.items
 
     def objects(self) -> List[Scorer]:
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/context/scoring/scorers.py` & `aizynthfinder-4.3.0/aizynthfinder/context/scoring/scorers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,56 @@
 """ Module containing classes used to score the reaction routes.
 """
+
 from __future__ import annotations
 
 import abc
+import json
 from collections import defaultdict
 from collections.abc import Sequence as SequenceAbc
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 import numpy as np
 
+try:
+    from route_distances.route_distances import route_distances_calculator
+except ImportError:
+    SUPPORT_DISTANCES = False
+else:
+    SUPPORT_DISTANCES = True
+
 from aizynthfinder.chem import TreeMolecule
 from aizynthfinder.context.stock import StockException
 from aizynthfinder.reactiontree import ReactionTree
 from aizynthfinder.search.mcts import MctsNode
+from aizynthfinder.utils.bonds import BrokenBonds
 from aizynthfinder.utils.exceptions import ScorerException
+from aizynthfinder.utils.logging import logger
+from aizynthfinder.utils.sc_score import SCScore
 
 if TYPE_CHECKING:
-    from aizynthfinder.chem import FixedRetroReaction, Molecule, RetroReaction
+    from aizynthfinder.chem import (
+        FixedRetroReaction,
+        Molecule,
+        RetroReaction,
+        UniqueMolecule,
+    )
     from aizynthfinder.context.config import Configuration
     from aizynthfinder.utils.type_utils import (
         Iterable,
         Optional,
         Sequence,
         StrDict,
         Tuple,
         TypeVar,
         Union,
     )
 
+    _Molecules = Sequence[Molecule]
     _Scoreable = TypeVar("_Scoreable", MctsNode, ReactionTree)
     _Scoreables = Sequence[_Scoreable]
     _ScorerItemType = Union[_Scoreables, _Scoreable]
 
 
 @dataclass
 class SquashScaler:
@@ -511,27 +529,30 @@
 
 class StockAvailabilityScorer(Scorer):
     """
     Scorer that computes score based on the stock availability of the starting material
 
     The score is calculated as a product of a stock score per starting material. The stock
     score for each molecule is based on the source of the stock, or a default value if the
-    molecule is not in stock.
+    molecule is not in stock. The `other_source_score` parameter can be used to
+    distinguish between "not in stock" and "not in the specificed sources" cases.
     """
 
     def __init__(
         self,
         config: Configuration,
         source_score: StrDict,
         default_score: float = 0.1,
+        other_source_score: Optional[float] = None,
     ) -> None:
         super().__init__(config)
         assert self._config is not None
         self.source_score = source_score
         self.default_score = default_score
+        self.other_source_score = other_source_score
 
     def __repr__(self) -> str:
         return "stock availability"
 
     def _calculate_leaf_costs(
         self, leafs: Union[Sequence[Molecule], Iterable[Molecule]]
     ) -> float:
@@ -540,24 +561,292 @@
         for mol in leafs:
             availability = self._config.stock.availability_list(mol)
             scores = [
                 self.source_score[source]
                 for source in availability
                 if source in self.source_score
             ]
-            prod *= max(scores) if scores else self.default_score
+            if scores:
+                prod *= max(scores)
+            elif self.other_source_score and mol in self._config.stock:
+                prod *= self.other_source_score
+            else:
+                prod *= self.default_score
         return prod
 
     def _score_node(self, node: MctsNode) -> float:
         return self._calculate_leaf_costs(node.state.mols)
 
     def _score_reaction_tree(self, tree: ReactionTree) -> float:
         return self._calculate_leaf_costs(tree.leafs())
 
 
+class BrokenBondsScorer(Scorer):
+    """Class for scoring nodes and reaction trees based on the breaking of atom bonds
+
+    The score is a summation of the depths in the tree where the focussed bonds
+    are found to break in the reaction. If a focussed bond is found to be unbroken
+    in the entire tree, the total length of the tree will be added to the score.
+    """
+
+    scorer_name = "broken bonds"
+
+    def __init__(self, config: Configuration) -> None:
+        super().__init__(config)
+        self._break_bonds = [tuple(bond) for bond in config.search.break_bonds]
+        self._break_bonds_operator = config.search.break_bonds_operator.lower()
+        self._reverse_order = False
+
+    def __repr__(self) -> str:
+        return self.scorer_name
+
+    def _calculate_broken_bonds_score(
+        self, reactions: Sequence[RetroReaction], depths: Sequence[int]
+    ) -> float:
+
+        if not reactions:
+            return 0
+
+        max_score = len(set(depths)) * len(self._break_bonds)
+        broken_focussed_bonds = []
+        scores = []
+
+        # The score should be 0 when no transformations were reported
+        if not depths:
+            return 0
+
+        for reaction, depth in zip(reactions, depths):
+            broken_bonds = BrokenBonds(self._break_bonds)(reaction)
+            broken_untracked_bonds = [
+                bond for bond in broken_bonds if bond not in broken_focussed_bonds
+            ]
+            if len(broken_untracked_bonds) > 0:
+                broken_focussed_bonds += broken_untracked_bonds
+                scores.append(1 - (depth / max_score))
+                if self._break_bonds_operator == "or":
+                    break
+
+        if self._break_bonds_operator != "or" or (
+            self._break_bonds_operator == "or" and len(broken_focussed_bonds) == 0
+        ):
+            # type: ignore
+            if unbroken_bonds := set(self._break_bonds) - set(broken_focussed_bonds):
+                scores.append(1 - (len(set(depths)) * len(unbroken_bonds)) / max_score)
+        return sum(scores) / len(scores)
+
+    def _score_node(self, node: MctsNode) -> float:
+        reactions = node.actions_to()
+        depths = []
+        for reaction in reactions:
+            depth = (
+                max(
+                    reactant.transform
+                    for reactant in reaction.reactants[reaction.index]
+                )
+                - 1
+            )
+            depths.append(depth)
+        return self._calculate_broken_bonds_score(reactions, depths)
+
+    def _score_reaction_tree(self, tree: ReactionTree) -> float:
+        reactions = [
+            reaction.to_smiles_based_retroreaction() for reaction in tree.reactions()
+        ]
+        depths = [tree.depth(reaction) // 2 for reaction in tree.reactions()]
+        return self._calculate_broken_bonds_score(reactions, depths)
+
+
+class RouteSimilarityScorer(Scorer):
+    """
+    Class for scoring based on an LSTM model for computing Tree Edit Distance to
+    a set of reference routes.
+
+    :param config: the configuration of the tree search
+    :param routes_path: the filename of a JSON file with reference routes
+    :param model_path: the filename of a checkpoint file with the LSTM model
+    :param scaler_params: the parameter settings of the scaler
+    :param agg_func: the name of numpy function used to aggregate the distances
+                     to the reference routes
+    :param similarity: if True, will compute similarity score else distance scores
+    """
+
+    scorer_name = "route similarity"
+
+    def __init__(
+        self,
+        config: Configuration,
+        routes_path: str,
+        model_path: str,
+        scaler_params: Optional[StrDict] = None,
+        agg_func: str = "min",
+        similarity: bool = False,
+    ) -> None:
+        if not SUPPORT_DISTANCES:
+            raise ValueError(
+                "Distance calculations are not supported by this installation."
+                " Please install aizynthfinder with extras dependencies."
+            )
+
+        # Default scaler from benchmarking
+        if scaler_params is None:
+            scaler_params = {
+                "name": "squash",
+                "slope": 0.5,
+                "xoffset": 10,
+                "yoffset": 0,
+            }
+
+        super().__init__(config, scaler_params)
+        self._reverse_order = similarity
+        self.calculator = route_distances_calculator("lstm", model_path=model_path)
+
+        # Scalar needs to be applied before taking into account of `similarity` parameter,
+        # hence we are reassigning the global scaler and then disabling it.
+        self._local_scaler = self._scaler
+        self._scaler = None
+
+        if not hasattr(np, agg_func):
+            raise ValueError(f"Cannot identify aggregate function {agg_func} in numpy")
+        self.agg_func = getattr(np, agg_func)
+        self.similarity = similarity
+
+        try:
+            with open(routes_path or "") as file:
+                self.routes = json.load(file)
+        except FileNotFoundError:
+            logger().info(
+                f"Could not load reference routes from {routes_path}. Assuming they will be set later"
+            )
+            self.routes = []
+        self.n_routes = len(self.routes)
+
+    def _score_node(self, node: MctsNode) -> float:
+        # We don't have any short-cut to score a node,
+        # so we need to convert it to a reaction tree
+        return self._score_reaction_tree(node.to_reaction_tree())
+
+    def _score_reaction_tree(self, tree: ReactionTree) -> float:
+        if not self.routes:
+            return 0.0 if self.similarity else 1.0
+
+        dist_matrix = self.calculator(self.routes + [tree.to_dict()])
+        distances = dist_matrix[self.n_routes, : self.n_routes]
+        score = self.agg_func(distances)
+        norm_score = self._local_scaler(score)
+        if self.similarity:
+            return 1.0 - float(norm_score)
+        return float(norm_score)
+
+
+class DeltaSyntheticComplexityScorer(Scorer):
+    """
+    Class for scoring nodes based on the delta-synthetic-complexity of the node
+    and its parent 'horizon' steps up in the tree.
+
+    :param config: the configuration the tree search
+    :param sc_score_model: the path to the SCScore model
+    :param scaler_params: the parameter settings of the scaler, defaults to max-min between -1.5 and 4
+    :param horizon: the number of steps backwards to look for parent molecule
+    """
+
+    scorer_name: str = "delta-SC score"
+
+    def __init__(
+        self,
+        config: Configuration,
+        sc_score_model: str,
+        scaler_params: Optional[StrDict] = None,
+        horizon: int = 3,
+    ) -> None:
+        if scaler_params is None:
+            scaler_params = {
+                "name": "min_max",
+                "min_val": -1.5,
+                "max_val": 4,
+                "reverse": False,
+            }
+        super().__init__(config, scaler_params)
+        ## This is necessary because config should not be optional for this scorer
+        self._config: Configuration = config
+
+        self.horizon = horizon
+        self._model = SCScore(sc_score_model)
+
+    def sc_deltas(self, mols: _Molecules, parents: _Molecules) -> Sequence[float]:
+        """
+        Calculate delta SC-score among the list of mol-parent pairs.
+
+        :params mols: the leaves of the tree
+        :param parents: the parent of the leaves
+        :returns: the pair-wise difference in SCScore
+        """
+        delta_sc_scores = []
+        for mol, parent in zip(mols, parents):
+            mol.sanitize()
+            parent.sanitize()
+
+            sc_score_mol = self._model(mol.rd_mol)
+            sc_score_parent = self._model(parent.rd_mol)
+
+            delta_sc_score = sc_score_parent - sc_score_mol
+            delta_sc_scores.append(delta_sc_score)
+        return delta_sc_scores
+
+    def _get_parent_from_reaction_tree(
+        self, tree: ReactionTree, mol: UniqueMolecule, horizon: int
+    ) -> UniqueMolecule:
+        horizon = min(horizon, tree.depth(mol) // 2)
+
+        parent = mol
+        # Step up in the tree, first a reaction, then a molecule
+        for _ in range(horizon):
+            parent = tree.parent_molecule(parent)
+
+        return parent
+
+    def _get_parent_from_tree_molecule(
+        self, mol: TreeMolecule, horizon: int
+    ) -> TreeMolecule:
+        horizon = min(horizon, mol.transform)
+
+        parent = mol
+        # Step up in the tree via parent nodes
+        for _ in range(horizon):
+            grandparent = parent.parent
+            if not grandparent:
+                break
+            parent = grandparent
+
+        return parent
+
+    def _score_node(self, node: MctsNode) -> float:
+        expandable_mols = node.state.expandable_mols
+        if not expandable_mols:
+            expandable_mols = list(node.state.mols)
+
+        parent_mols = [
+            self._get_parent_from_tree_molecule(mol, self.horizon)
+            for mol in expandable_mols
+        ]
+        delta_sc_scores = self.sc_deltas(expandable_mols, parent_mols)
+        return min(delta_sc_scores)
+
+    def _score_reaction_tree(self, tree: ReactionTree) -> float:
+        expandable_mols = [node for node in tree.leafs() if not tree.in_stock(node)]
+        if not expandable_mols:
+            expandable_mols = list(tree.leafs())
+
+        parent_mols = [
+            self._get_parent_from_reaction_tree(tree, node, self.horizon)
+            for node in expandable_mols
+        ]
+        delta_sc_scores = self.sc_deltas(expandable_mols, parent_mols)
+        return min(delta_sc_scores)
+
+
 class CombinedScorer(Scorer):
     """Class for scoring nodes and reaction trees by combining weighted scores from a list of scorers
 
     If no weights are provided as input, the scorer provides default weights that are
     equal for all input scorers.
 
     The CombinedScorer cannot be instantiated from the config file as it requires the
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/context/stock/queries.py` & `aizynthfinder-4.3.0/aizynthfinder/context/stock/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Module containing classes that interfaces different stocks query classes
 """
+
 from __future__ import annotations
 
 import os
 from typing import TYPE_CHECKING
 
 import pandas as pd
 
@@ -18,19 +19,17 @@
 from aizynthfinder.utils.exceptions import StockException
 from aizynthfinder.utils.mongo import get_mongo_client
 
 if TYPE_CHECKING:
     from pymongo.collection import Collection as MongoCollection
     from pymongo.database import Database as MongoDatabase
 
-    # pylint: disable=ungrouped-imports
     from aizynthfinder.utils.type_utils import Optional, Set, StrDict
 
 
-# pylint: disable=no-self-use
 class StockQueryMixin:
     """
     Mixin class for all query classes, providing a default interface
     to some methods that might not be possible to implement for each
     query class.
     """
 
@@ -116,15 +115,15 @@
                 inchis = fileobj.read().splitlines()
             self._stock_inchikeys = set(inchis)
             self._price_dict: StrDict = {}
             return
 
         if ext in [".h5", ".hdf5"]:
             stock_df: pd.DataFrame = pd.read_hdf(path, key="table")
-        elif ext == ".csv":
+        else:
             stock_df = pd.read_csv(
                 path,
                 usecols=[inchi_key_col, price_col] if price_col else [inchi_key_col],
             )
         inchis = stock_df[inchi_key_col].values
         self._stock_inchikeys = set(inchis)
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/data/default_training.yml` & `aizynthfinder-4.3.0/aizynthfinder/data/default_training.yml`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/data/templates/reaction_tree.dot` & `aizynthfinder-4.3.0/aizynthfinder/data/templates/reaction_tree.dot`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/data/templates/reaction_tree.thtml` & `aizynthfinder-4.3.0/aizynthfinder/data/templates/reaction_tree.thtml`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/interfaces/aizynthapp.py` & `aizynthfinder-4.3.0/aizynthfinder/interfaces/aizynthapp.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     SelectMultiple,
     Text,
     VBox,
 )
 from rdkit import Chem
 
 from aizynthfinder.aizynthfinder import AiZynthFinder
+from aizynthfinder.interfaces.gui.utils import pareto_fronts_plot, route_display
 from aizynthfinder.utils.logging import setup_logger
 
 if TYPE_CHECKING:
     from aizynthfinder.utils.type_utils import StrDict
 
 
 class AiZynthApp:
@@ -49,15 +50,14 @@
     :ivar finder: the finder instance
 
     :param configfile: the path to yaml file with configuration
     :param setup: if True will create and display the GUI on instantiation, defaults to True
     """
 
     def __init__(self, configfile: str, setup: bool = True) -> None:
-        # pylint: disable=used-before-assignment
         setup_logger(logging.INFO)
         self.finder = AiZynthFinder(configfile=configfile)
         self._input: StrDict = dict()
         self._output: StrDict = dict()
         self._buttons: StrDict = dict()
         if setup:
             self.setup()
@@ -148,56 +148,77 @@
         self._input["max_transforms"] = BoundedIntText(
             description="Max tree depth",
             min=1,
             max=20,
             value=self.finder.config.search.max_transforms,
             style={"description_width": "initial"},
         )
-        self._input["exclude_target_from_stock"] = widgets.Checkbox(
-            value=self.finder.config.search.exclude_target_from_stock,
-            description="Exclude target from stock",
+
+        rewards = self.finder.config.search.algorithm_config.get("search_rewards", [])
+        objective1 = rewards[0] if len(rewards) > 0 else "state score"
+        objective2 = rewards[1] if len(rewards) > 1 else "None"
+        self._input["reward1"] = widgets.Dropdown(
+            options=self.finder.scorers.names(),
+            description="MCTS reward 1:",
+            value=objective1,
+            style={"description_width": "initial"},
+        )
+
+        self._input["reward2"] = widgets.Dropdown(
+            options=["None"] + self.finder.scorers.names(),
+            description="MCTS reward 2:",
+            value=objective2,
+            style={"description_width": "initial"},
         )
+
         vbox = VBox(
             [
                 self._input["policy"],
                 self._input["filter"],
                 max_time_box,
                 max_iter_box,
                 self._input["return_first"],
                 self._input["max_transforms"],
-                self._input["exclude_target_from_stock"],
+                self._input["reward1"],
+                self._input["reward2"],
             ]
         )
         box_options = HBox([box_stocks, vbox])
         display(box_options)
 
     def _create_route_widgets(self) -> None:
         self._input["scorer"] = widgets.Dropdown(
             options=self.finder.scorers.names(),
             description="Reorder by:",
             style={"description_width": "initial"},
         )
+        self._input["scorer"].disabled = True
         self._input["scorer"].observe(self._on_change_scorer)
-        self._buttons["show_routes"] = Button(description="Show Reactions")
+        self._buttons["show_routes"] = Button(description="Show Routes")
         self._buttons["show_routes"].on_click(self._on_display_button_clicked)
         self._input["route"] = Dropdown(
             options=[],
             description="Routes: ",
         )
+        self._input["route"].disabled = True
         self._input["route"].observe(self._on_change_route_option)
         display(
             HBox(
                 [
                     self._buttons["show_routes"],
                     self._input["route"],
                     self._input["scorer"],
                 ]
             )
         )
 
+        self._output["pareto_fronts"] = widgets.Output(
+            layout={"border": "1px solid silver", "width": "99%", "overflow": "auto"}
+        )
+        display(self._output["pareto_fronts"])
         self._output["routes"] = widgets.Output(
             layout={"border": "1px solid silver", "width": "99%"}
         )
         display(self._output["routes"])
 
     def _create_search_widgets(self) -> None:
         self._buttons["execute"] = Button(description="Run Search")
@@ -247,21 +268,30 @@
     def _on_extend_button_clicked(self, _) -> None:
         self._toggle_button(False)
         self._tree_search()
         self._toggle_button(True)
 
     def _on_display_button_clicked(self, _) -> None:
         self._toggle_button(False)
-        self.finder.build_routes()
+        rewards = self.finder.config.search.algorithm_config["search_rewards"]
+        self.finder.build_routes(scorer=rewards)
         self.finder.routes.make_images()
         self.finder.routes.compute_scores(*self.finder.scorers.objects())
         self._input["route"].options = [
             f"Option {i}" for i, _ in enumerate(self.finder.routes, 1)  # type: ignore
         ]
+
+        self._output["pareto_fronts"].clear_output()
+        if len(rewards) > 1:
+            with self._output["pareto_fronts"]:
+                pareto_fronts_plot(self.finder.routes)
+
         self._show_route(0)
+        self._input["scorer"].disabled = len(rewards) > 1
+        self._input["route"].disabled = False
         self._toggle_button(True)
 
     def _prepare_search(self) -> None:
         self._output["tree_search"].clear_output()
         with self._output["tree_search"]:
             selected_stocks = [
                 cb.description for cb in self._input["stocks"] if cb.value
@@ -284,53 +314,38 @@
                 "max_transforms"
             ].value
             self.finder.config.search.return_first = self._input["return_first"].value
             self.finder.config.search.time_limit = self._input["time_limit"].value * 60
             self.finder.config.search.iteration_limit = self._input[
                 "iteration_limit"
             ].value
-            self.finder.config.search.exclude_target_from_stock = self._input[
-                "exclude_target_from_stock"
-            ].value
+
+            rewards = [self._input["reward1"].value]
+            if self._input["reward2"].value != "None":
+                rewards.append(self._input["reward2"].value)
+            self.finder.config.search.algorithm_config["search_rewards"] = rewards
+            if self.finder.config.search.algorithm != "mcts":
+                print(
+                    "Only MCTS algorithm is supported in GUI interface. Resetting to MCTS"
+                )
+                self.finder.config.search.algorithm = "mcts"
 
             smiles = self._input["smiles"].value
-            print("Setting target molecule with smiles: %s" % smiles)
+            print(f"Setting target molecule with smiles: {smiles}")
             self.finder.target_smiles = smiles
             self.finder.prepare_tree()
 
     def _show_mol(self, change) -> None:
         self._output["smiles"].clear_output()
         with self._output["smiles"]:
             mol = Chem.MolFromSmiles(change["new"])
             display(mol)
 
     def _show_route(self, index) -> None:
-        if (
-            index is None
-            or self.finder.routes is None
-            or index >= len(self.finder.routes)
-        ):
-            return
-
-        route = self.finder.routes[index]
-        state = route["node"].state
-        status = "Solved" if state.is_solved else "Not Solved"
-
-        self._output["routes"].clear_output()
-        with self._output["routes"]:
-            display(HTML("<H2>%s" % status))
-            table_content = "".join(
-                f"<tr><td>{name}</td><td>{score:.4f}</td></tr>"
-                for name, score in route["all_score"].items()
-            )
-            display(HTML(f"<table>{table_content}</table>"))
-            display(HTML("<H2>Compounds to Procure"))
-            display(state.to_image())
-            display(HTML("<H2>Steps"))
-            display(self.finder.routes[index]["image"])
+        route_display(index, self.finder.routes, self._output["routes"])
 
     def _toggle_button(self, on_) -> None:
         for button in self._buttons.values():
             button.disabled = not on_
 
     def _tree_search(self) -> None:
         with self._output["tree_search"]:
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/interfaces/aizynthcli.py` & `aizynthfinder-4.3.0/aizynthfinder/interfaces/aizynthcli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Module containing classes and routines for the CLI
 """
+
 from __future__ import annotations
 
 import argparse
 import importlib
 import json
 import logging
 import os
@@ -32,14 +33,15 @@
         List,
         Optional,
         StrDict,
         Union,
     )
 
     _PostProcessingJob = Callable[[AiZynthFinder], StrDict]
+    _PreProcessingJob = Callable[[AiZynthFinder, int], None]
 
 
 def _do_clustering(
     finder: AiZynthFinder,
     results: StrDict,
     detailed_results: bool,
     model_path: Optional[str] = None,
@@ -112,14 +114,17 @@
     )
     parser.add_argument(
         "--post_processing",
         nargs="+",
         help="a number of modules that performs post-processing tasks",
     )
     parser.add_argument(
+        "--pre_processing", help="a module that perform pre-processing tasks"
+    )
+    parser.add_argument(
         "--checkpoint",
         required=False,
         help="the path to the checkpoint file",
     )
     return parser.parse_args()
 
 
@@ -133,14 +138,29 @@
         else:
             if hasattr(module, "post_processing"):
                 print(f"Adding post-processing job from {module_name}")
                 jobs.append(getattr(module, "post_processing"))
     return jobs
 
 
+def _load_preprocessing_job(module_name: Optional[str]) -> Optional[_PreProcessingJob]:
+    if not module_name:
+        return None
+
+    try:
+        module = importlib.import_module(module_name)
+    except ModuleNotFoundError:
+        pass
+    else:
+        if hasattr(module, "pre_processing"):
+            print(f"Adding pre-processing job from {module_name}")
+            return getattr(module, "pre_processing")
+    return None
+
+
 def _select_stocks(finder: AiZynthFinder, args: argparse.Namespace) -> None:
     stocks = list(args.stocks)
     try:
         module = importlib.import_module("custom_stock")
     except ModuleNotFoundError:
         pass
     else:
@@ -172,17 +192,20 @@
 def _process_single_smiles(
     smiles: str,
     finder: AiZynthFinder,
     output_name: str,
     do_clustering: bool,
     route_distance_model: Optional[str],
     post_processing: List[_PostProcessingJob],
+    pre_processing: Optional[_PreProcessingJob],
 ) -> None:
     output_name = output_name or "trees.json"
     finder.target_smiles = smiles
+    if pre_processing:
+        pre_processing(finder, -1)
     try:
         finder.prepare_tree()
     except ValueError as err:
         print(f"Failed to setup search due to: '{str(err).lower()}'")
         return
     finder.tree_search(show_progress=True)
     finder.build_routes()
@@ -192,17 +215,14 @@
         json.dump(
             finder.routes.dict_with_extra(include_metadata=True, include_scores=True),
             fileobj,
             indent=2,
         )
     logger().info(f"Trees saved to {output_name}")
 
-    scores = ", ".join("%.4f" % score for score in finder.routes.scores)
-    logger().info(f"Scores for best routes: {scores}")
-
     stats = finder.extract_statistics()
     if do_clustering:
         _do_clustering(
             finder, stats, detailed_results=False, model_path=route_distance_model
         )
     _do_post_processing(finder, stats, post_processing)
     stats_str = "\n".join(
@@ -214,14 +234,15 @@
 def _process_multi_smiles(
     filename: str,
     finder: AiZynthFinder,
     output_name: str,
     do_clustering: bool,
     route_distance_model: Optional[str],
     post_processing: List[_PostProcessingJob],
+    pre_processing: Optional[_PreProcessingJob],
     checkpoint: Optional[str],
 ) -> None:
     output_name = output_name or "output.json.gz"
     with open(filename, "r") as fileobj:
         smiles = [line.strip() for line in fileobj.readlines()]
 
     checkpoint_data: StrDict = defaultdict(list)
@@ -233,15 +254,17 @@
     results: StrDict = defaultdict(list)
     if checkpoint_data:
         results = {
             key: value
             for key, value in checkpoint_data.items()
             if key != "processed_smiles"
         }
-    for smi in smiles:
+    for idx, smi in enumerate(smiles):
+        if pre_processing:
+            pre_processing(finder, idx)
         processed_results = {}
         finder.target_smiles = smi
         try:
             finder.prepare_tree()
         except ValueError as err:
             print(f"Failed to setup search for {smi} due to: '{str(err).lower()}'")
             continue
@@ -257,17 +280,14 @@
                 finder, stats, detailed_results=True, model_path=route_distance_model
             )
         _do_post_processing(finder, stats, post_processing)
 
         for key, value in stats.items():
             processed_results[key] = value
         processed_results["stock_info"] = finder.stock_info()
-        processed_results["top_scores"] = ", ".join(
-            "%.4f" % score for score in finder.routes.scores
-        )
         processed_results["trees"] = finder.routes.dict_with_extra(
             include_metadata=True, include_scores=True
         )
 
         if checkpoint:
             with open(checkpoint, "a") as checkpoint_file:
                 checkpoint_file.write(
@@ -351,27 +371,29 @@
         return
 
     multi_smiles = os.path.exists(args.smiles)
 
     finder = AiZynthFinder(configfile=args.config)
     _select_stocks(finder, args)
     post_processing = _load_postprocessing_jobs(args.post_processing)
+    pre_processing = _load_preprocessing_job(args.pre_processing)
     finder.expansion_policy.select(args.policy or finder.expansion_policy.items[0])
     if args.filter:
         finder.filter_policy.select(args.filter)
     else:
         finder.filter_policy.select_all()
 
     params = [
         args.smiles,
         finder,
         args.output,
         args.cluster,
         args.route_distance_model,
         post_processing,
+        pre_processing,
         args.checkpoint,
     ]
     if multi_smiles:
         _process_multi_smiles(*params)
     else:
         params = params[:-1]
         _process_single_smiles(*params)
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/interfaces/gui/clustering.py` & `aizynthfinder-4.3.0/aizynthfinder/interfaces/gui/clustering.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/reactiontree.py` & `aizynthfinder-4.3.0/aizynthfinder/reactiontree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ Module containing the implementation of a reaction tree or route and factory classes to make such trees """
+
 from __future__ import annotations
 
 import abc
 import hashlib
 import json
 import operator
 from typing import TYPE_CHECKING
@@ -160,14 +161,26 @@
 
         :yield: the next molecule in the tree
         """
         for node in self.graph:
             if isinstance(node, UniqueMolecule):
                 yield node
 
+    def parent_molecule(self, mol: UniqueMolecule) -> UniqueMolecule:
+        """Returns the parent molecule within the reaction tree.
+        :param mol: the query node (molecule)
+        :return: the parent molecule
+        """
+        if mol is self.root:
+            raise ValueError("Root molecule does not have any parent node.")
+
+        parent_reaction = list(self.graph.predecessors(mol))[0]
+        parent_molecule = list(self.graph.predecessors(parent_reaction))[0]
+        return parent_molecule
+
     def reactions(self) -> Iterable[FixedRetroReaction]:
         """
         Generates the reaction nodes of the reaction tree
 
         :yield: the next reaction in the tree
         """
         for node in self.graph:
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/search/andor_trees.py` & `aizynthfinder-4.3.0/aizynthfinder/search/andor_trees.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,20 @@
 
     @property
     def mol_nodes(self) -> List[TreeNodeMixin]:
         """Return the molecule nodes of the tree"""
         return []
 
     @abc.abstractmethod
-    def one_iteration(self) -> bool:  # pylint: disable=no-self-use
+    def one_iteration(self) -> bool:
         """Perform one iteration of the search"""
         return False
 
     @abc.abstractmethod
-    def routes(self) -> List[ReactionTree]:  # pylint: disable=no-self-use
+    def routes(self) -> List[ReactionTree]:
         """Return the routes of the tree"""
         return []
 
 
 class SplitAndOrTree:
     """
     Encapsulation of an algorithm to split an AND/OR tree into separate routes
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/search/breadth_first/nodes.py` & `aizynthfinder-4.3.0/aizynthfinder/search/breadth_first/nodes.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/search/breadth_first/search_tree.py` & `aizynthfinder-4.3.0/aizynthfinder/search/breadth_first/search_tree.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/search/dfpn/nodes.py` & `aizynthfinder-4.3.0/aizynthfinder/search/dfpn/nodes.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/search/dfpn/search_tree.py` & `aizynthfinder-4.3.0/aizynthfinder/search/dfpn/search_tree.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/search/mcts/node.py` & `aizynthfinder-4.3.0/aizynthfinder/search/mcts/node.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 from __future__ import annotations
 
 import random
 from typing import TYPE_CHECKING
 
 import numpy as np
+from paretoset import paretoset
 
 from aizynthfinder.chem import TreeMolecule, deserialize_action, serialize_action
 from aizynthfinder.search.mcts.state import MctsState
 from aizynthfinder.search.mcts.utils import ReactionTreeFromSuperNode, route_to_node
 from aizynthfinder.utils.exceptions import (
     NodeUnexpectedBehaviourException,
     RejectionException,
@@ -110,82 +111,82 @@
         :param smiles: the SMILES representation of the root state
         :param tree: the search tree
         :param config: settings of the tree search algorithm
         :return: the created node
         """
         mol = TreeMolecule(parent=None, transform=0, smiles=smiles)
         state = MctsState(mols=[mol], config=config)
-        return MctsNode(state=state, owner=tree, config=config)
+        return cls(state=state, owner=tree, config=config)
 
     @classmethod
     def from_dict(
         cls,
         dict_: StrDict,
         tree: MctsSearchTree,
         config: Configuration,
         molecules: MoleculeDeserializer,
         parent: Optional["MctsNode"] = None,
     ) -> "MctsNode":
         """
-        Create a new node from a dictionary, i.e. deserialization
+        Create a new node from a dictionary, i.e. deserialization.
 
         :param dict_: the serialized node
         :param tree: the search tree
         :param config: settings of the tree search algorithm
         :param molecules: the deserialized molecules
         :param parent: the parent node
         :return: a deserialized node
         """
         # pylint: disable=protected-access
         state = MctsState.from_dict(dict_["state"], config, molecules)
-        node = MctsNode(state=state, owner=tree, config=config, parent=parent)
+        node = cls(state=state, owner=tree, config=config, parent=parent)
         node.is_expanded = dict_["is_expanded"]
         node.is_expandable = dict_["is_expandable"]
         node._children_values = dict_["children_values"]
         node._children_priors = dict_["children_priors"]
         node._children_visitations = dict_["children_visitations"]
         node._children_actions = [
             deserialize_action(action_dict, molecules)
             for action_dict in dict_["children_actions"]
         ]
         node._children = [
-            MctsNode.from_dict(child, tree, config, molecules, parent=node)
+            cls.from_dict(child, tree, config, molecules, parent=node)
             if child
             else None
             for child in dict_["children"]
         ]
         return node
 
     @property
     def children(self) -> List["MctsNode"]:
         """
-        Returns all of the instantiated children
+        Returns all of the instantiated children.
 
         :return: the children
         """
         return [child for child in self._children if child]
 
     @property
     def is_solved(self) -> bool:
-        """Return if the state is solved"""
+        """Return if the state is solved."""
         return self.state.is_solved
 
     @property
     def parent(self) -> Optional["MctsNode"]:
-        """Return the parent of the node"""
+        """Return the parent of the node."""
         return self._parent
 
     @property
     def state(self) -> MctsState:
-        """Return the underlying state of the node"""
+        """Return the underlying state of the node."""
         return self._state
 
     @property
     def _algo_config(self) -> StrDict:
-        """Just a convinient, shorter name of this"""
+        """Just a convinient, shorter name of this."""
         return self._config.search.algorithm_config
 
     def actions_to(self) -> List[RetroReaction]:
         """
         Returns the actions leading to this node
 
         :return: the list of actions
@@ -247,105 +248,97 @@
         if self.parent:
             for child in self.parent.children:
                 if child is not self:
                     cache_molecules.extend(child.state.expandable_mols)
 
         # Calculate the possible actions, fill the child_info lists
         # Actions by default only assumes 1 set of reactants
-        (
-            self._children_actions,
-            self._children_priors,
-        ) = self._expansion_policy(self.state.expandable_mols, cache_molecules)
-        nactions = len(self._children_actions)
-        self._children_visitations = [1] * nactions
-        self._children = [None] * nactions
-        if self._algo_config["use_prior"]:
-            self._children_values = list(self._children_priors)
-        else:
-            self._children_values = [self._algo_config["default_prior"]] * nactions
+        actions, priors = self._expansion_policy(
+            self.state.expandable_mols, cache_molecules
+        )
+        self._fill_children_lists(actions, priors)
 
-        if nactions == 0:  # Reverse the expansion if it did not produce any children
+        # Reverse the expansion if it did not produce any children
+        if len(actions) == 0:
             self.is_expandable = False
             self.is_expanded = False
 
         if self.tree:
             self.tree.profiling["expansion_calls"] += 1
 
         if not self._algo_config["immediate_instantiation"]:
             return
         # Instantiate all children actions created by the marked policy,
         # a new list of actions will be iterated over, because it can grow due
         # to instantiation
+        nactions = len(actions)
         for child_idx, action in enumerate(self._children_actions[:nactions]):
             policy_name = action.metadata.get("policy_name")
             if (
                 policy_name
                 and policy_name in self._algo_config["immediate_instantiation"]
             ):
                 self._instantiate_child(child_idx)
 
     def is_terminal(self) -> bool:
         """
-        Node is terminal if its unexpandable, or the internal state is terminal (solved)
+        Node is terminal if its unexpandable, or the internal state is terminal (solved).
 
         :return: the terminal attribute of the node
         """
         return not self.is_expandable or self.state.is_terminal
 
     def path_to(self) -> Tuple[List[RetroReaction], List[MctsNode]]:
         """
-        Return the path to this node, which is a list of actions and a list of node
+        Return the path to this node, which is a list of actions and a list of node.
 
         :return: the actions and nodes
         """
         return route_to_node(self)
 
     def promising_child(self) -> Optional["MctsNode"]:
         """
-        Return the child with the currently highest Q+U
+        Return the child with the currently highest Q+U.
 
         The selected child will be instantiated if it has not been already.
 
         If no actions could be found that were applicable, the method will
         return None.
 
         :return: the child
         """
-
-        def _score_and_select():
-            scores = self._children_q() + self._children_u()
-            indices = np.where(scores == scores.max())[0]
-            index = np.random.choice(indices)
-
-            return self._select_child(index)
-
         child = None
-        while child is None and max(self._children_values) > 0:
-            child = _score_and_select()
+        while child is None:
+            try:
+                child = self._score_and_select()
+            # _score_and_select raises exception if no children can be selected
+            except ValueError:
+                child = None
+                break
 
         if not child:
             self._logger.debug(
                 "Returning None from promising_child() because there were no applicable action"
             )
             self.is_expanded = False
             self.is_expandable = False
 
         return child
 
     def serialize(self, molecule_store: MoleculeSerializer) -> StrDict:
         """
-        Serialize the node object to a dictionary
+        Serialize the node object to a dictionary.
 
         :param molecule_store: the serialized molecules
         :return: the serialized node
         """
         return {
             "state": self.state.serialize(molecule_store),
-            "children_values": [float(value) for value in self._children_values],
-            "children_priors": [float(value) for value in self._children_priors],
+            "children_values": self._serialize_stats_list("_children_values"),
+            "children_priors": self._serialize_stats_list("_children_priors"),
             "children_visitations": self._children_visitations,
             "children_actions": [
                 serialize_action(action, molecule_store)
                 for action in self._children_actions
             ],
             "children": [
                 child.serialize(molecule_store) if child else None
@@ -353,15 +346,15 @@
             ],
             "is_expanded": self.is_expanded,
             "is_expandable": self.is_expandable,
         }
 
     def to_reaction_tree(self) -> ReactionTree:
         """
-        Return reaction tree from the path of actions and nodes leading to this node
+        Return reaction tree from the path of actions and nodes leading to this node.
 
         :return: the constructed tree
         """
         return ReactionTreeFromSuperNode(self).tree
 
     def _check_child_reaction(self, reaction: RetroReaction) -> bool:
         if not reaction.reactants:
@@ -391,40 +384,56 @@
         first_child_idx = child_idx
         for state_index, state in enumerate(states):
             if self._generated_degeneracy(state, first_child_idx):
                 # Only need to disable first new child,
                 # if the action generated more states, we will just not generate
                 # a child for that state
                 if state_index == 0:
-                    self._children_values[child_idx] = -1e6
+                    self._disable_child(child_idx)
                 continue
 
             # If there's more than one outcome, the lists need be expanded
             if state_index > 0:
                 child_idx = self._expand_children_lists(first_child_idx, state_index)
 
             if self._filter_child_reaction(self._children_actions[child_idx]):
-                self._children_values[child_idx] = -1e6
+                self._disable_child(child_idx)
             else:
-                new_node = MctsNode(
+                new_node = self.__class__(
                     state=state, owner=self.tree, config=self._config, parent=self
                 )
                 self._children[child_idx] = new_node
                 new_nodes.append(new_node)
         return new_nodes
 
+    def _disable_child(self, child_idx: int) -> None:
+        self._children_values[child_idx] = -1e6
+
     def _expand_children_lists(self, old_index: int, action_index: int) -> int:
         new_action = self._children_actions[old_index].copy(index=action_index)
         self._children_actions.append(new_action)
         self._children_priors.append(self._children_priors[old_index])
         self._children_values.append(self._children_values[old_index])
         self._children_visitations.append(self._children_visitations[old_index])
         self._children.append(None)
         return len(self._children) - 1
 
+    def _fill_children_lists(
+        self, actions: List[RetroReaction], priors: List[float]
+    ) -> None:
+        self._children_actions = actions
+        self._children_priors = priors
+        nactions = len(actions)
+        self._children_visitations = [1] * nactions
+        self._children = [None] * nactions
+        if self._algo_config["use_prior"]:
+            self._children_values = list(self._children_priors)
+        else:
+            self._children_values = [self._algo_config["default_prior"]] * nactions
+
     def _filter_child_reaction(self, reaction: RetroReaction) -> bool:
         if self._regenerated_blacklisted(reaction):
             self._logger.debug(
                 f"Reaction {reaction.reaction_smiles()} "
                 f"was rejected because it re-generated molecule not in stock"
             )
             return True
@@ -436,16 +445,15 @@
         except RejectionException as err:
             self._logger.debug(str(err))
             return True
         return False
 
     def _generated_degeneracy(self, new_state: MctsState, child_idx: int) -> bool:
         """
-        Check if a new MCTS state is equal to another MCTS state of a children
-        node.
+        Check if a new MCTS state is equal to another MCTS state of a children node.
 
         The check can be "partial" in which the equality is based only on the expandable molecules,
         or "full" in which the equality is based on all molecules in the state.
 
         The comparison will not be made on unexpanded children nodes
         or terminal children nodes.
 
@@ -481,15 +489,15 @@
         if "additional_actions" not in previous_action.metadata:
             previous_action.metadata["additional_actions"] = []
         previous_action.metadata["additional_actions"].append(metadata_copy)
         return True
 
     def _instantiate_child(self, child_idx: int) -> List["MctsNode"]:
         """
-        Instantiate the children node
+        Instantiate the children node.
 
         The algorithm is:
         * Apply the reaction associated with the child
         * If the application of the action failed, set value to -1e6 and return None
         * Create a new state array, one new state for each of the reaction outcomes
         * Create new child nodes
             - If a filter policy is available and the reaction outcome is unlikely
@@ -502,15 +510,15 @@
         reaction = self._children_actions[child_idx]
         if reaction.unqueried:
             if self.tree:
                 self.tree.profiling["reactants_generations"] += 1
             _ = reaction.reactants
 
         if not self._check_child_reaction(reaction):
-            self._children_values[child_idx] = -1e6
+            self._disable_child(child_idx)
             return []
 
         keep_mols = [mol for mol in self.state.mols if mol is not reaction.mol]
         new_states = [
             MctsState(keep_mols + list(reactants), self._config)
             for reactants in reaction.reactants
         ]
@@ -521,21 +529,220 @@
             return False
         for reactants in reaction.reactants:
             for mol in reactants:
                 if mol.inchi_key in self.blacklist:
                     return True
         return False
 
+    def _score_and_select(self) -> Optional["MctsNode"]:
+        if not max(self._children_values) > 0:
+            raise ValueError("Has no selectable children")
+        scores = self._children_q() + self._children_u()
+        indices = np.where(scores == scores.max())[0]
+        index = np.random.choice(indices)
+        return self._select_child(index)
+
     def _select_child(self, child_idx: int) -> Optional["MctsNode"]:
         """
-        Selecting a child node implies instantiating the children nodes
+        Selecting a child node implies instantiating the children nodes.
 
         If the child has already been instantiated, return immediately
         Otherwise, select a random node of the feasible ones to return
         """
         if self._children[child_idx]:
             return self._children[child_idx]
 
         new_nodes = self._instantiate_child(child_idx)
         if new_nodes:
             return random.choice(new_nodes)
         return None
+
+    def _serialize_stats_list(self, name: str) -> List[float]:
+        return [float(value) for value in getattr(self, name)]
+
+
+class ParetoMctsNode(MctsNode):
+    """
+    A node in a multi-objective tree search.
+
+    This implements the algorithm from:
+        Chen W., Liu L. Pareto Monte Carlo Tree Search for Multi-Objective Informative Planning
+        Robotics: Science and Systems 2019, 2012 arXiv:2111.01825
+
+
+    The main difference compared to the standard MCTS algorithm is:
+        - Children stats: the values, cumulative reward and priors are nested
+                     list, with one value per objective
+        - Selection: children on Pareto front are computed, and
+                     a child from this set is taken randomly
+
+    This implementation disregards the prior of the children when it has been
+    visited once.
+
+    It is assumed that all objectives are to be maximised.
+    """
+
+    def __init__(
+        self,
+        state: MctsState,
+        owner: MctsSearchTree,
+        config: Configuration,
+        parent: Optional[ParetoMctsNode] = None,
+    ):
+        super().__init__(state, owner, config, parent)
+        self._num_objectives = len(self._algo_config["search_rewards"])
+        self._prior_weight = 1
+        self._direction = "max"  # current implementation assumes maximisation
+        self._children_rewards_cummulative: List[List[float]]
+        self._children_values: List[List[float]]  # type: ignore
+        self._children_priors: List[List[float]]  # type: ignore
+
+    def backpropagate(self, child: "MctsNode", value_estimate: List[float]) -> None:  # type: ignore
+        """
+        Update the number of visitations of a particular child and its value.
+
+        :param child: the child node
+        :param value_estimate: the value to add to the child value
+        """
+        idx = self._children.index(child)
+        self._children_visitations[idx] += 1
+        # here we only update the cummulative rewards,
+        #  _children_values are updated at selection time
+        new_value_estimate = [
+            cum_reward + new_reward
+            for cum_reward, new_reward in zip(
+                self._children_rewards_cummulative[idx], value_estimate
+            )
+        ]
+        self._children_rewards_cummulative[idx] = new_value_estimate
+
+    def children_view(self) -> StrDict:
+        """
+        Creates a view of the children attributes. Each of the
+        list returned is a new list, although the actual children
+        are not copied.
+
+        The return dictionary will have keys "actions", "values",
+        "priors", "visitations", "rewards_cum", and "objects".
+
+        :return: the view
+        """
+        dict_ = super().children_view()
+        dict_["rewards_cum"] = list(self._children_rewards_cummulative)
+        return dict_
+
+    def serialize(self, molecule_store: MoleculeSerializer) -> StrDict:
+        """
+        Serialize the node object to a dictionary.
+
+        :param molecule_store: the serialized molecules
+        :return: the serialized node
+        """
+        dict_ = super().serialize(molecule_store)
+        dict_["children_cumulative_reward"] = self._serialize_stats_list(
+            "_children_rewards_cummulative"
+        )
+        return dict_
+
+    def _disable_child(self, child_idx: int) -> None:
+        self._children_rewards_cummulative[child_idx] = [-1e6] * self._num_objectives
+
+    def _expand_children_lists(self, old_index: int, action_index: int) -> int:
+        ret = super()._expand_children_lists(old_index, action_index)
+        # These lists are nested lists, so need to make sure that the inner lists are also new
+        self._children_values[-1] = list(self._children_values[-1])
+        self._children_priors[-1] = list(self._children_priors[-1])
+        self._children_rewards_cummulative.append(
+            list(self._children_rewards_cummulative[old_index])
+        )
+        return ret
+
+    def _fill_children_lists(
+        self, actions: List[RetroReaction], priors: List[float]
+    ) -> None:
+        self._children_actions = actions
+        nactions = len(actions)
+        # shape: num_actions x 1
+        self._children_visitations = [1] * nactions
+        self._children = [None] * nactions
+        # shape: num_actions x num_objectives
+        self._children_rewards_cummulative = [[0.0] * self._num_objectives] * nactions
+        if self._algo_config["use_prior"]:
+            # shape: num_actions x num_objectives
+            # for children i, 3 objectives -> [prior i, prior i, prior i]
+            self._children_priors = [[prior] * self._num_objectives for prior in priors]
+
+        else:
+            self._children_priors = [
+                [self._algo_config["default_prior"]] * self._num_objectives
+            ] * nactions
+
+        # at initialisation, values = prior as cummulative rewards are zero
+        self._children_values = [
+            [prior * self._prior_weight for prior in priors]
+            for priors in self._children_priors
+        ]
+
+    def _children_q(self, children_values_arr):
+        children_visitations_expanded = np.repeat(
+            np.array(self._children_visitations).reshape(-1, 1),
+            axis=1,
+            repeats=self._num_objectives,
+        )
+        return children_values_arr / children_visitations_expanded
+
+    def _compute_children_scores(self) -> np.ndarray:
+        """Compute the modified ucb scores: alpha * prior + average reward + exploration."""
+        # update prior to zero once the node has been visited
+        children_priors_arr = self._prior_schedule_oneoff()
+        # compute prior_weight * prior + cummulative rewards
+        children_values_arr = self._prior_weight * children_priors_arr + np.array(
+            self._children_rewards_cummulative
+        )
+        expanded_u = np.repeat(
+            self._children_u().reshape(-1, 1), axis=1, repeats=self._num_objectives
+        )
+        # _children_scores shape: num_childrens x num_objectives
+        children_scores = self._children_q(children_values_arr) + expanded_u
+        if children_scores.shape[1] != self._num_objectives:
+            raise ValueError(
+                f"expected second dimension to have {self._num_objectives},"
+                f"currently has {children_scores.shape[1]}"
+            )
+        self._children_values = children_values_arr.tolist()
+        self._children_priors = children_priors_arr.tolist()
+        return children_scores
+
+    def _prior_schedule_oneoff(self) -> np.ndarray:
+        # shape: num_children x 1
+        visted_mask = (np.array(self._children_visitations) > 1).reshape(-1, 1)
+        # shape: num_children x num_objectives
+        visted_mask = np.repeat(visted_mask, axis=1, repeats=self._num_objectives)
+        # set the prior weights for visited children to be zero
+        children_priors_arr = np.array(self._children_priors)
+        children_priors_arr[visted_mask] = 0
+        return children_priors_arr
+
+    def _score_and_select(self) -> Optional["MctsNode"]:
+        if not max(max(value_list) for value_list in self._children_values) > 0:
+            raise ValueError("Has no selectable children")
+        children_scores = self._compute_children_scores()
+        pareto_idxs = self._update_pareto_front(children_scores)
+        index = np.random.choice(pareto_idxs)
+        return self._select_child(index)
+
+    def _serialize_stats_list(self, name: str):
+        return [
+            [float(value) for value in value_list] for value_list in getattr(self, name)
+        ]
+
+    def _update_pareto_front(self, children_scores: np.ndarray) -> np.ndarray:
+        """
+        Update the pareto front of a node, this step normally happens
+        after its values for the best child have been updated.
+
+        :param children_scores: Children scores
+        :returns: Pareto front children indexes
+        """
+        direction_arr = np.repeat(self._direction, self._num_objectives)
+        mask = paretoset(children_scores, sense=direction_arr, distinct=False)
+        return np.arange(len(self._children))[mask]
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/search/mcts/search.py` & `aizynthfinder-4.3.0/aizynthfinder/search/retrostar/search_tree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,168 +1,205 @@
 """ Module containing a class that holds the tree search
 """
 from __future__ import annotations
 
 import json
 from typing import TYPE_CHECKING
 
-import networkx as nx
+import numpy as np
 
-from aizynthfinder.chem import MoleculeDeserializer, MoleculeSerializer
-from aizynthfinder.search.mcts.node import MctsNode
+from aizynthfinder.chem.serialization import MoleculeDeserializer, MoleculeSerializer
+from aizynthfinder.search.andor_trees import AndOrSearchTreeBase, SplitAndOrTree
+from aizynthfinder.search.retrostar.cost import MoleculeCost
+from aizynthfinder.search.retrostar.nodes import MoleculeNode
+from aizynthfinder.utils.exceptions import RejectionException
+from aizynthfinder.utils.logging import logger
 
 if TYPE_CHECKING:
+    from aizynthfinder.chem import RetroReaction
     from aizynthfinder.context.config import Configuration
-    from aizynthfinder.utils.type_utils import List, Optional
+    from aizynthfinder.reactiontree import ReactionTree
+    from aizynthfinder.utils.type_utils import List, Optional, Sequence
 
 
-class MctsSearchTree:
+class SearchTree(AndOrSearchTreeBase):
     """
-    Encapsulation of the search tree.
+    Encapsulation of the Retro* search tree (an AND/OR tree).
 
+    :ivar config: settings of the tree search algorithm
     :ivar root: the root node
-    :ivar config: the configuration of the search tree
 
     :param config: settings of the tree search algorithm
     :param root_smiles: the root will be set to a node representing this molecule, defaults to None
     """
 
     def __init__(
         self, config: Configuration, root_smiles: Optional[str] = None
     ) -> None:
-        self.profiling = {
-            "expansion_calls": 0,
-            "reactants_generations": 0,
-            "iterations": 0,
-        }
+        super().__init__(config, root_smiles)
+        self._mol_nodes: List[MoleculeNode] = []
+        self._logger = logger()
+        self.molecule_cost = MoleculeCost(config)
 
         if root_smiles:
-            self.root: Optional[MctsNode] = MctsNode.create_root(
-                smiles=root_smiles, tree=self, config=config
+            self.root: Optional[MoleculeNode] = MoleculeNode.create_root(
+                root_smiles, config, self.molecule_cost
             )
+            self._mol_nodes.append(self.root)
         else:
             self.root = None
-        self.config = config
-        self._graph: Optional[nx.DiGraph] = None
-        self.reward_scorer_name = config.search.algorithm_config["search_reward"]
-        self.reward_scorer = config.scorers[self.reward_scorer_name]
+
+        self._routes: List[ReactionTree] = []
+
+        self.profiling = {
+            "expansion_calls": 0,
+            "reactants_generations": 0,
+        }
 
     @classmethod
-    def from_json(cls, filename: str, config: Configuration) -> "MctsSearchTree":
+    def from_json(cls, filename: str, config: Configuration) -> SearchTree:
         """
         Create a new search tree by deserialization from a JSON file
 
         :param filename: the path to the JSON node
-        :param config: the configuration of the search
+        :param config: the configuration of the search tree
         :return: a deserialized tree
         """
-        tree = MctsSearchTree(config)
+
+        def _find_mol_nodes(node):
+            for child_ in node.children:
+                tree._mol_nodes.append(child_)  # pylint: disable=protected-access
+                for grandchild in child_.children:
+                    _find_mol_nodes(grandchild)
+
+        tree = cls(config)
         with open(filename, "r") as fileobj:
             dict_ = json.load(fileobj)
         mol_deser = MoleculeDeserializer(dict_["molecules"])
-        tree.root = MctsNode.from_dict(dict_["tree"], tree, config, mol_deser)
+        tree.root = MoleculeNode.from_dict(
+            dict_["tree"], config, mol_deser, tree.molecule_cost
+        )
+        tree._mol_nodes.append(tree.root)  # pylint: disable=protected-access
+        for child in tree.root.children:
+            _find_mol_nodes(child)
         return tree
 
-    def backpropagate(self, from_node: MctsNode, value_estimate: float) -> None:
-        """
-        Backpropagate the value estimate and update all nodes from a
-        given node all the way to the root.
-
-        :param from_node: the end node of the route to update
-        :param value_estimate: The score value to backpropagate
-        """
-        current = from_node
-        while current is not self.root:
-            parent = current.parent
-            # For mypy, parent should never by None unless current is the root
-            assert parent is not None
-            parent.backpropagate(current, value_estimate)
-            current = parent
-
-    def graph(self, recreate: bool = False) -> nx.DiGraph:
-        """
-        Construct a directed graph object with the nodes as
-        vertices and the actions as edges attribute "action".
-
-        :param recreate: if True will construct the graph even though it is cached, defaults to False
-        :return: the graph object
-        :raises ValueError: if the tree is not defined
-        """
-        if not self.root:
-            raise ValueError("Root of search tree is not defined ")
-
-        if not recreate and self._graph:
-            return self._graph
-
-        def add_node(node):
-            self._graph.add_edge(node.parent, node, action=node.parent[node]["action"])
-            for grandchild in node.children:
-                add_node(grandchild)
-
-        self._graph = nx.DiGraph()
-        # Always add the root
-        self._graph.add_node(self.root)
-        for child in self.root.children:
-            add_node(child)
-        return self._graph
-
-    def nodes(self) -> List[MctsNode]:
-        """Return all the nodes in the search tree"""
-        return list(self.graph())
+    @property
+    def mol_nodes(self) -> Sequence[MoleculeNode]:  # type: ignore
+        """Return the molecule nodes of the tree"""
+        return self._mol_nodes
 
     def one_iteration(self) -> bool:
         """
         Perform one iteration of
             1. Selection
             2. Expansion
-            3. Rollout
-            4. Backpropagation
+            3. Update
 
+        :raises StopIteration: if the search should be pre-maturely terminated
         :return: if a solution was found
+        :rtype: bool
         """
-        self.profiling["iterations"] += 1
-        leaf = self.select_leaf()
-        leaf.expand()
-        while not leaf.is_terminal():
-            child = leaf.promising_child()
-            if child:
-                child.expand()
-                leaf = child
-
-        state_score = self.reward_scorer(leaf)
-        self.backpropagate(leaf, state_score)
-        return leaf.state.is_solved
-
-    def select_leaf(self) -> MctsNode:
-        """
-        Traverse the tree selecting the most promising child at
-        each step until leaf node returned.
-
-        :return: the leaf node
-        :raises ValueError: if the tree is not defined
-        """
-        if not self.root:
-            raise ValueError("Root of search tree is not defined ")
-
-        current = self.root
-        while current.is_expanded and not current.state.is_solved:
-            promising_child = current.promising_child()
-            # If promising_child returns None it means that the node
-            # is unexpandable, and hence we should break the loop
-            if promising_child:
-                current = promising_child
-        return current
+        if self.root is None:
+            raise ValueError("Root is undefined. Cannot make an iteration")
+
+        self._routes = []
+
+        next_node = self._select()
+
+        if not next_node:
+            self._logger.debug("No expandable nodes in Retro* iteration")
+            raise StopIteration
+
+        self._expand(next_node)
+
+        if not next_node.children:
+            next_node.expandable = False
+
+        self._update(next_node)
+
+        return self.root.solved
+
+    def routes(self) -> List[ReactionTree]:
+        """
+        Extracts and returns routes from the AND/OR tree
+
+        :return: the routes
+        """
+        if self.root is None:
+            return []
+        if not self._routes:
+            self._routes = SplitAndOrTree(self.root, self.config.stock).routes
+        return self._routes
 
     def serialize(self, filename: str) -> None:
         """
-        Serialize the search tree to a JSON file
+        Seralize the search tree to a JSON file
 
         :param filename: the path to the JSON file
-        :raises ValueError: if the tree is not defined
+        :type filename: str
         """
-        if not self.root:
-            raise ValueError("Root of search tree is not defined ")
+        if self.root is None:
+            raise ValueError("Cannot serialize tree as root is not defined")
 
         mol_ser = MoleculeSerializer()
         dict_ = {"tree": self.root.serialize(mol_ser), "molecules": mol_ser.store}
         with open(filename, "w") as fileobj:
             json.dump(dict_, fileobj, indent=2)
+
+    def _expand(self, node: MoleculeNode) -> None:
+        reactions, priors = self.config.expansion_policy([node.mol])
+        self.profiling["expansion_calls"] += 1
+
+        if not reactions:
+            return
+
+        costs = -np.log(np.clip(priors, 1e-3, 1.0))
+        reactions_to_expand = []
+        reaction_costs = []
+        for reaction, cost in zip(reactions, costs):
+            try:
+                self.profiling["reactants_generations"] += 1
+                _ = reaction.reactants
+            except:  # pylint: disable=bare-except
+                continue
+            if not reaction.reactants:
+                continue
+            for idx, _ in enumerate(reaction.reactants):
+                rxn_copy = reaction.copy(idx)
+                if self._filter_reaction(rxn_copy):
+                    continue
+                reactions_to_expand.append(rxn_copy)
+                reaction_costs.append(cost)
+
+        for cost, rxn in zip(reaction_costs, reactions_to_expand):
+            new_nodes = node.add_stub(cost, rxn)
+            self._mol_nodes.extend(new_nodes)
+
+    def _filter_reaction(self, reaction: RetroReaction) -> bool:
+        if not self.config.filter_policy.selection:
+            return False
+        try:
+            self.config.filter_policy(reaction)
+        except RejectionException as err:
+            self._logger.debug(str(err))
+            return True
+        return False
+
+    def _select(self) -> Optional[MoleculeNode]:
+        scores = np.asarray(
+            [
+                node.target_value if node.expandable else np.inf
+                for node in self._mol_nodes
+            ]
+        )
+
+        if scores.min() == np.inf:
+            return None
+
+        return self._mol_nodes[int(np.argmin(scores))]
+
+    @staticmethod
+    def _update(node: MoleculeNode) -> None:
+        v_delta = node.close()
+        if node.parent and np.isfinite(v_delta):
+            node.parent.update(v_delta, from_mol=node.mol)
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/search/mcts/state.py` & `aizynthfinder-4.3.0/aizynthfinder/search/mcts/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,20 +66,19 @@
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, MctsState):
             return False
         return self.__hash__() == other.__hash__()
 
     def __str__(self) -> str:
         """A string representation of the state (for print(state))"""
-        string = "%s\n%s\n%s\n%s\n Solved: %s" % (
-            str([mol.smiles for mol in self.mols]),
-            str([mol.transform for mol in self.mols]),
-            str([mol.parent.smiles if mol.parent else "-" for mol in self.mols]),
-            str(self.in_stock_list),
-            self.is_solved,
+        string = (
+            f"{str([mol.smiles for mol in self.mols])}\n"
+            + f"{str([mol.transform for mol in self.mols])}\n"
+            + f"{str([mol.parent.smiles if mol.parent else '-' for mol in self.mols])}\n"
+            + f"{str(self.in_stock_list)}\n Solved: {self.is_solved}"
         )
         return string
 
     @classmethod
     def from_dict(
         cls, dict_: StrDict, config: Configuration, molecules: MoleculeDeserializer
     ) -> "MctsState":
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/search/mcts/utils.py` & `aizynthfinder-4.3.0/aizynthfinder/search/mcts/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
             in_stock=nodes[0].state.is_solved,
         )
 
         for child, action in zip(nodes[1:], actions):
             self._add_bipartite(child, action)
 
     def _add_bipartite(self, child: MctsNode, action: RetroReaction) -> None:
-
         reaction_obj = self._unique_reaction(action)
         self._add_node(reaction_obj, depth=2 * action.mol.transform + 1)
         self.tree.graph.add_edge(self._unique_mol(action.mol), reaction_obj)
         reactant_nodes = []
         for mol in child.state.mols:
             if mol.parent is action.mol:
                 self._add_node(
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/search/retrostar/cost.py` & `aizynthfinder-4.3.0/aizynthfinder/search/retrostar/cost.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,9 +125,9 @@
 
 class ZeroMoleculeCost:
     """Encapsulation of a Zero cost model"""
 
     def __repr__(self) -> str:
         return "zero"
 
-    def calculate(self, mol: Molecule) -> float:
+    def calculate(self, _mol: Molecule) -> float:  # pytest: disable=unused-argument
         return 0.0
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/search/retrostar/nodes.py` & `aizynthfinder-4.3.0/aizynthfinder/search/retrostar/nodes.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/tools/cat_output.py` & `aizynthfinder-4.3.0/aizynthfinder/tools/cat_output.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/tools/download_public_data.py` & `aizynthfinder-4.3.0/aizynthfinder/tools/download_public_data.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/tools/make_stock.py` & `aizynthfinder-4.3.0/aizynthfinder/tools/make_stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,20 +93,20 @@
     The other elements are taken as input to the ``extract_smiles`` method
 
     The SMILES are yielded to save memory.
     """
     module_name = files.pop(0)
     module = importlib.import_module(module_name)
     if not files:
-        for smiles in module.extract_smiles():  # type: ignore
+        for smiles in module.extract_smiles():  # type: ignore  # pylint: disable=R1737
             yield smiles
     else:
         for filename in files:
             print(f"Processing {filename}", flush=True)
-            for smiles in module.extract_smiles(filename):  # type: ignore
+            for smiles in module.extract_smiles(filename):  # type: ignore  # pylint: disable=R1737
                 yield smiles
 
 
 def make_hdf5_stock(inchi_keys: _StrIterator, filename: str) -> None:
     """
     Put all the inchi keys from the given iterable in a pandas
     dataframe and save it as an HDF5 file. Only unique inchi keys
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/utils/exceptions.py` & `aizynthfinder-4.3.0/aizynthfinder/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/utils/files.py` & `aizynthfinder-4.3.0/aizynthfinder/utils/files.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/utils/image.py` & `aizynthfinder-4.3.0/aizynthfinder/utils/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from aizynthfinder.utils.paths import data_path
 
 if TYPE_CHECKING:
     import networkx as nx
 
     from aizynthfinder.chem import FixedRetroReaction, RetroReaction, UniqueMolecule
 
-    # pylint: disable=ungrouped-imports
     from aizynthfinder.utils.type_utils import (
         Any,
         Dict,
         FrameColors,
         List,
         PilColor,
         PilImage,
@@ -117,21 +116,21 @@
     x0_lim = img.width
     y0_lim = img.height
     x1_lim = 0
     y1_lim = 0
     for x in range(0, img.width):
         for y in range(0, img.height):
             if img.getpixel((x, y)) != (255, 255, 255):
-                if x < x0_lim:
+                if x < x0_lim:  # pylint: disable=R1730
                     x0_lim = x
-                if x > x1_lim:
+                if x > x1_lim:  # pylint: disable=R1731
                     x1_lim = x
-                if y < y0_lim:
+                if y < y0_lim:  # pylint: disable=R1730
                     y0_lim = y
-                if y > y1_lim:
+                if y > y1_lim:  # pylint: disable=R1731
                     y1_lim = y
     x0_lim = max(x0_lim, 0)
     y0_lim = max(y0_lim, 0)
     x1_lim = min(x1_lim + 1, img.width)
     y1_lim = min(y1_lim + 1, img.height)
     # Then crop to this area
     cropped = img.crop((x0_lim, y0_lim, x1_lim, y1_lim))
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/utils/loading.py` & `aizynthfinder-4.3.0/aizynthfinder/utils/loading.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/utils/logging.py` & `aizynthfinder-4.3.0/aizynthfinder/utils/logging.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/aizynthfinder/utils/models.py` & `aizynthfinder-4.3.0/aizynthfinder/utils/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,16 @@
             inputs = kwargs
         else:
             inputs = dict(zip(self._sig_def["inputs"].keys(), args))
 
         tensors = {}
         for name, vec in inputs.items():
             size = int(self._sig_def["inputs"][name]["tensorShape"]["dim"][1]["size"])
-            tensors[name] = tf.make_tensor_proto(vec, dtype=np.float32, shape=(1, size))
+            assert size == vec.shape[1], "Incorrect shape for input"
+            tensors[name] = tf.make_tensor_proto(vec, dtype=np.float32, shape=vec.shape)
         return tensors
 
     @staticmethod
     def _get_server(name: str) -> str:
         warning = f"Failed to get gRPC server for external model {name}"
         if not TF_SERVING_HOST:
             _logger.warning(warning)
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/utils/mongo.py` & `aizynthfinder-4.3.0/aizynthfinder/utils/mongo.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,9 +44,9 @@
     if _CLIENT is None:
         params = {}
         if tls_certs_path:
             params.update({"ssl": "true", "ssl_ca_certs": tls_certs_path})
         cred_str = f"{user}:{password}@" if password else ""
         uri = f"mongodb://{cred_str}{host}:{port}/?{urlencode(params)}"
         logger().debug(f"Connecting to MongoDB on {host}:{port}")
-        _CLIENT = MongoClient(uri)
+        _CLIENT = MongoClient(uri)  # pylint: disable=C0103
     return _CLIENT
```

### Comparing `aizynthfinder-4.0.0/aizynthfinder/utils/type_utils.py` & `aizynthfinder-4.3.0/aizynthfinder/utils/type_utils.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-4.0.0/pyproject.toml` & `aizynthfinder-4.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aizynthfinder"
-version = "4.0.0"
+version = "4.3.0"
 description = "Retrosynthetic route finding using neural network guided Monte-Carlo tree search"
 authors = ["Molecular AI group <samuel.genheden@astrazeneca.com>"]
 license = "MIT"
 include = ["aizynthfinder/data/*.yml", "aizynthfinder/data/templates/*"]
 readme = "README.md"
 homepage = "https://github.com/MolecularAI/aizynthfinder/"
 repository = "https://github.com/MolecularAI/aizynthfinder/"
@@ -22,32 +22,36 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 ipywidgets = "^7.5.1"
 jinja2 = "^3.0.0"
 jupyter = "^1.0.0"
 jupytext = "^1.3.3"
+notebook = "^6.5.3"
 networkx = "^2.4"
 deprecated = "^1.2.10"
 pandas = "^1.0.0"
 pillow = "^9.0.0"
 requests = "^2.23.0"
 rdchiral = "^1.0.0"
 rdkit = "^2022.3.3"
 tables = "^3.6.1"
 tqdm = "^4.42.1"
 onnxruntime = "^1.14.0"
 tensorflow = {version = "^2.8.0", optional=true}
 grpcio = {version = "^1.24.0", optional=true}
 tensorflow-serving-api = {version = "^2.1.0", optional=true}
 pymongo = {version = "^3.10.1", optional=true}
-route-distances = {version = "^1.1.0", optional=true}
+route-distances = {version = "^1.1.1", optional=true}
 scipy = {version = "^1.0", optional=true}
 matplotlib = {version = "^3.0.0", optional=true}
 timeout-decorator = {version = "^0.5.0", optional=true}
+molbloom = {version = "^2.1.0", optional=true}
+paretoset = "^1.2.3"
+seaborn = "^0.13.2"
 
 [tool.poetry.dev-dependencies]
 black = "^22.0.0"
 invoke = "^1.5.0"
 pytest = "^6.2.2"
 pytest-black = "^0.3.12"
 pytest-cov = "^2.11.0"
@@ -55,15 +59,15 @@
 pytest-mock = "^3.5.0"
 pytest-mccabe = "^2.0.0"
 sphinx = "^4.0.0"
 mypy = "^1.0.0"
 pylint = "^2.16.0"
 
 [tool.poetry.extras]
-all = ["pymongo", "route-distances", "scipy", "matplotlib", "timeout-decorator"]
+all = ["pymongo", "route-distances", "scipy", "matplotlib", "timeout-decorator", "molbloom"]
 tf = ["tensorflow", "grpcio", "tensorflow-serving-api"]
 
 [tool.poetry.scripts]
 aizynthapp = "aizynthfinder.interfaces.aizynthapp:main"
 aizynthcli = "aizynthfinder.interfaces.aizynthcli:main"
 cat_aizynth_output = "aizynthfinder.tools.cat_output:main"
 download_public_data = "aizynthfinder.tools.download_public_data:main"
```

### Comparing `aizynthfinder-4.0.0/PKG-INFO` & `aizynthfinder-4.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aizynthfinder
-Version: 4.0.0
+Version: 4.3.0
 Summary: Retrosynthetic route finding using neural network guided Monte-Carlo tree search
 Home-page: https://github.com/MolecularAI/aizynthfinder/
 License: MIT
 Author: Molecular AI group
 Author-email: samuel.genheden@astrazeneca.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -16,39 +16,43 @@
 Requires-Dist: deprecated (>=1.2.10,<2.0.0)
 Requires-Dist: grpcio (>=1.24.0,<2.0.0) ; extra == "tf"
 Requires-Dist: ipywidgets (>=7.5.1,<8.0.0)
 Requires-Dist: jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: jupytext (>=1.3.3,<2.0.0)
 Requires-Dist: matplotlib (>=3.0.0,<4.0.0) ; extra == "all"
+Requires-Dist: molbloom (>=2.1.0,<3.0.0) ; extra == "all"
 Requires-Dist: networkx (>=2.4,<3.0)
+Requires-Dist: notebook (>=6.5.3,<7.0.0)
 Requires-Dist: onnxruntime (>=1.14.0,<2.0.0)
 Requires-Dist: pandas (>=1.0.0,<2.0.0)
+Requires-Dist: paretoset (>=1.2.3,<2.0.0)
 Requires-Dist: pillow (>=9.0.0,<10.0.0)
 Requires-Dist: pymongo (>=3.10.1,<4.0.0) ; extra == "all"
 Requires-Dist: rdchiral (>=1.0.0,<2.0.0)
 Requires-Dist: rdkit (>=2022.3.3,<2023.0.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
-Requires-Dist: route-distances (>=1.1.0,<2.0.0) ; extra == "all"
+Requires-Dist: route-distances (>=1.1.1,<2.0.0) ; extra == "all"
 Requires-Dist: scipy (>=1.0,<2.0) ; extra == "all"
+Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: tables (>=3.6.1,<4.0.0)
 Requires-Dist: tensorflow (>=2.8.0,<3.0.0) ; extra == "tf"
 Requires-Dist: tensorflow-serving-api (>=2.1.0,<3.0.0) ; extra == "tf"
 Requires-Dist: timeout-decorator (>=0.5.0,<0.6.0) ; extra == "all"
 Requires-Dist: tqdm (>=4.42.1,<5.0.0)
 Project-URL: Documentation, https://molecularai.github.io/aizynthfinder/
 Project-URL: Repository, https://github.com/MolecularAI/aizynthfinder/
 Description-Content-Type: text/markdown
 
 # AiZynthFinder
 
 [![License](https://img.shields.io/github/license/MolecularAI/aizynthfinder)](https://github.com/MolecularAI/aizynthfinder/blob/master/LICENSE)
 [![Tests](https://github.com/MolecularAI/aizynthfinder/workflows/tests/badge.svg)](https://github.com/MolecularAI/aizynthfinder/actions?workflow=tests)
 [![codecov](https://codecov.io/gh/MolecularAI/aizynthfinder/branch/master/graph/badge.svg)](https://codecov.io/gh/MolecularAI/aizynthfinder)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black) 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![version](https://img.shields.io/github/v/release/MolecularAI/aizynthfinder)](https://github.com/MolecularAI/aizynthfinder/releases)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MolecularAI/aizynthfinder/blob/master/contrib/notebook.ipynb)
 
 AiZynthFinder is a tool for retrosynthetic planning. The default algorithm is based on a Monte Carlo tree search that recursively breaks down a molecule to purchasable precursors. The tree search is guided by a policy that suggests possible precursors by utilizing a neural network trained on a library of known reaction templates. This setup is completely customizable as the tool
 supports multiple search algorithms and expansion policies.
 
 An introduction video can be found here: [https://youtu.be/r9Dsxm-mcgA](https://youtu.be/r9Dsxm-mcgA)
@@ -65,35 +69,35 @@
 
 ## Installation
 
 ### For end-users
 
 First time, execute the following command in a console or an Anaconda prompt
 
-    conda create "python>=3.8,<3.10" -n aizynth-env
+    conda create "python>=3.9,<3.11" -n aizynth-env
 
 To install, activate the environment and install the package using pypi
 
     conda activate aizynth-env
     python -m pip install aizynthfinder[all]
 
 for a smaller package, without all the functionality, you can also type
 
     python -m pip install aizynthfinder
 
 ### For developers
 
 First clone the repository using Git.
 
-Then execute the following commands in the root of the repository 
+Then execute the following commands in the root of the repository
 
     conda env create -f env-dev.yml
     conda activate aizynth-dev
     poetry install --all-extras
-    
+
 the `aizynthfinder` package is now installed in editable mode.
 
 
 ## Usage
 
 The tool will install the `aizynthcli` and `aizynthapp` tools
 as interfaces to the algorithm:
@@ -105,15 +109,15 @@
 Consult the documentation [here](https://molecularai.github.io/aizynthfinder/) for more information.
 
 To use the tool you need
 
     1. A stock file
     2. A trained expansion policy network
     3. A trained filter policy network (optional)
-    
+
 Such files can be downloaded from [figshare](https://figshare.com/articles/AiZynthFinder_a_fast_robust_and_flexible_open-source_software_for_retrosynthetic_planning/12334577) and [here](https://figshare.com/articles/dataset/A_quick_policy_to_filter_reactions_based_on_feasibility_in_AI-guided_retrosynthetic_planning/13280507) or they can be downloaded automatically using
 
 ```
 download_public_data my_folder
 ```
 
 where ``my_folder`` is the folder that you want download to.
@@ -128,15 +132,15 @@
 Run the tests using:
 
     pytest -v
 
 The full command run on the CI server is available through an `invoke` command
 
     invoke full-tests
-    
+
  ### Documentation generation
 
 The documentation is generated by Sphinx from hand-written tutorials and docstrings
 
 The HTML documentation can be generated by
 
     invoke build-docs
```

