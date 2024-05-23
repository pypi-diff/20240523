# Comparing `tmp/molpipeline-0.8.1.tar.gz` & `tmp/molpipeline-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molpipeline-0.8.1.tar", last modified: Wed May 15 12:19:02 2024, max compression
+gzip compressed data, was "molpipeline-0.8.2.tar", last modified: Thu May 23 10:16:51 2024, max compression
```

## Comparing `molpipeline-0.8.1.tar` & `molpipeline-0.8.2.tar`

### file list

```diff
@@ -1,141 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.928191 molpipeline-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-15 12:18:56.000000 molpipeline-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-15 12:19:02.928191 molpipeline-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-15 12:18:56.000000 molpipeline-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.908191 molpipeline-0.8.1/molpipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.908191 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.912191 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/any2mol/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/any2mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/any2mol/string2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)    23644 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.912191 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/mol2bitvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/mol2floatvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/mol2string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.912191 molpipeline-0.8.1/molpipeline/any2mol/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/any2mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/any2mol/auto2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/any2mol/bin2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/any2mol/sdf2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/any2mol/smiles2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)    23790 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/error_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.912191 molpipeline-0.8.1/molpipeline/estimators/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.912191 molpipeline-0.8.1/molpipeline/estimators/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/algorithm/connected_component_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/algorithm/union_find.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.916191 molpipeline-0.8.1/molpipeline/estimators/chemprop/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/chemprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/chemprop/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/chemprop/component_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/chemprop/lightning_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/chemprop/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/chemprop/neural_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/connected_component_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/leader_picker_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/murcko_scaffold_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/nearest_neighbor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/estimators/similarity_transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.916191 molpipeline-0.8.1/molpipeline/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/metrics/ignore_error_scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.916191 molpipeline-0.8.1/molpipeline/mol2any/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2bin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2chemprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2concatinated_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2inchi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2morgan_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2net_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2rdkit_phys_chem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2any/mol2smiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.916191 molpipeline-0.8.1/molpipeline/mol2mol/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2mol/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2mol/reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2mol/scaffolds.py
--rw-r--r--   0 runner    (1001) docker     (127)    21043 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/mol2mol/standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.916191 molpipeline-0.8.1/molpipeline/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/pipeline/_molpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/pipeline/_skl_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/post_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.920191 molpipeline-0.8.1/molpipeline/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/json_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/molpipeline_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/substructure_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-15 12:18:56.000000 molpipeline-0.8.1/molpipeline/utils/value_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.928191 molpipeline-0.8.1/molpipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-15 12:19:02.000000 molpipeline-0.8.1/molpipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-15 12:19:02.000000 molpipeline-0.8.1/molpipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:19:02.000000 molpipeline-0.8.1/molpipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 12:19:02.000000 molpipeline-0.8.1/molpipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 12:19:02.000000 molpipeline-0.8.1/molpipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-15 12:18:56.000000 molpipeline-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 12:18:56.000000 molpipeline-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 12:18:56.000000 molpipeline-0.8.1/requirements_chemprop.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 12:18:56.000000 molpipeline-0.8.1/requirements_notebooks.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 12:19:02.928191 molpipeline-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.920191 molpipeline-0.8.1/test_extras/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.920191 molpipeline-0.8.1/test_extras/test_chemprop/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_chemprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_chemprop/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_chemprop/test_chemprop_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_chemprop/test_component_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_chemprop/test_lightning_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12424 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_chemprop/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.920191 molpipeline-0.8.1/test_extras/test_notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-15 12:18:56.000000 molpipeline-0.8.1/test_extras/test_notebooks/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.920191 molpipeline-0.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.920191 molpipeline-0.8.1/tests/test_elements/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.924191 molpipeline-0.8.1/tests/test_elements/test_any2mol/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_any2mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_any2mol/test_auto2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_any2mol/test_bin2mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_error_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.924191 molpipeline-0.8.1/tests/test_elements/test_mol2any/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2bin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2concatenated.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2inchi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2morgan_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2net_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2rdkit_phys_chem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.924191 molpipeline-0.8.1/tests/test_elements/test_mol2mol/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2mol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2mol/test_mol2mol_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_elements/test_mol2mol/test_mol2mol_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.924191 molpipeline-0.8.1/tests/test_estimators/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.924191 molpipeline-0.8.1/tests/test_estimators/test_algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_algorithm/test_connected_component_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_algorithm/test_union_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_connected_component_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_leader_picker_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_murcko_scaffold_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_nearest_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_estimators/test_similarity_transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.924191 molpipeline-0.8.1/tests/test_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_metrics/test_ignore_error_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.928191 molpipeline-0.8.1/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/test_utils/test_json_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:19:02.928191 molpipeline-0.8.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/utils/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-15 12:18:56.000000 molpipeline-0.8.1/tests/utils/mock_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.480758 molpipeline-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-23 10:16:43.000000 molpipeline-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-23 10:16:51.480758 molpipeline-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-23 10:16:43.000000 molpipeline-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.464758 molpipeline-0.8.2/molpipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.464758 molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.464758 molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/any2mol/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/any2mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/any2mol/string2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.464758 molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/mol2any/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/mol2any/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/mol2any/mol2bitvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/mol2any/mol2floatvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/mol2any/mol2string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.468758 molpipeline-0.8.2/molpipeline/any2mol/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/any2mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/any2mol/auto2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/any2mol/bin2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/any2mol/sdf2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/any2mol/smiles2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23671 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/error_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.468758 molpipeline-0.8.2/molpipeline/estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.468758 molpipeline-0.8.2/molpipeline/estimators/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/algorithm/connected_component_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/algorithm/union_find.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.468758 molpipeline-0.8.2/molpipeline/estimators/chemprop/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/chemprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/chemprop/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14752 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/chemprop/component_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/chemprop/lightning_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/chemprop/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/chemprop/neural_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/connected_component_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/leader_picker_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/murcko_scaffold_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/nearest_neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/estimators/similarity_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.468758 molpipeline-0.8.2/molpipeline/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/metrics/ignore_error_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.472758 molpipeline-0.8.2/molpipeline/mol2any/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2any/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2any/mol2bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2any/mol2chemprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2any/mol2concatinated_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2any/mol2inchi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2any/mol2morgan_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2any/mol2net_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2any/mol2rdkit_phys_chem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2any/mol2smiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.472758 molpipeline-0.8.2/molpipeline/mol2mol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2mol/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2mol/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2mol/scaffolds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20819 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/mol2mol/standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.472758 molpipeline-0.8.2/molpipeline/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15554 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/pipeline/_molpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32990 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/pipeline/_skl_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/post_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.472758 molpipeline-0.8.2/molpipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/utils/json_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/utils/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/utils/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/utils/molpipeline_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/utils/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/utils/substructure_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-23 10:16:43.000000 molpipeline-0.8.2/molpipeline/utils/value_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.480758 molpipeline-0.8.2/molpipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-23 10:16:51.000000 molpipeline-0.8.2/molpipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-23 10:16:51.000000 molpipeline-0.8.2/molpipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:16:51.000000 molpipeline-0.8.2/molpipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-23 10:16:51.000000 molpipeline-0.8.2/molpipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 10:16:51.000000 molpipeline-0.8.2/molpipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-23 10:16:43.000000 molpipeline-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-23 10:16:43.000000 molpipeline-0.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 10:16:43.000000 molpipeline-0.8.2/requirements_chemprop.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 10:16:43.000000 molpipeline-0.8.2/requirements_notebooks.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 10:16:51.480758 molpipeline-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.472758 molpipeline-0.8.2/test_extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 10:16:43.000000 molpipeline-0.8.2/test_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.476758 molpipeline-0.8.2/test_extras/test_chemprop/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 10:16:43.000000 molpipeline-0.8.2/test_extras/test_chemprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-23 10:16:43.000000 molpipeline-0.8.2/test_extras/test_chemprop/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-23 10:16:43.000000 molpipeline-0.8.2/test_extras/test_chemprop/test_chemprop_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-23 10:16:43.000000 molpipeline-0.8.2/test_extras/test_chemprop/test_component_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-23 10:16:43.000000 molpipeline-0.8.2/test_extras/test_chemprop/test_lightning_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12424 2024-05-23 10:16:43.000000 molpipeline-0.8.2/test_extras/test_chemprop/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.476758 molpipeline-0.8.2/test_extras/test_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 10:16:43.000000 molpipeline-0.8.2/test_extras/test_notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-23 10:16:43.000000 molpipeline-0.8.2/test_extras/test_notebooks/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.476758 molpipeline-0.8.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.476758 molpipeline-0.8.2/tests/test_elements/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.476758 molpipeline-0.8.2/tests/test_elements/test_any2mol/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_any2mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_any2mol/test_auto2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_any2mol/test_bin2mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_error_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.476758 molpipeline-0.8.2/tests/test_elements/test_mol2any/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_mol2any/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_mol2any/test_mol2bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_mol2any/test_mol2concatenated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_mol2any/test_mol2inchi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_mol2any/test_mol2morgan_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_mol2any/test_mol2net_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_mol2any/test_mol2rdkit_phys_chem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.476758 molpipeline-0.8.2/tests/test_elements/test_mol2mol/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_mol2mol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_mol2mol/test_mol2mol_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_elements/test_mol2mol/test_mol2mol_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.480758 molpipeline-0.8.2/tests/test_estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_estimators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.480758 molpipeline-0.8.2/tests/test_estimators/test_algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_estimators/test_algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_estimators/test_algorithm/test_connected_component_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_estimators/test_algorithm/test_union_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_estimators/test_connected_component_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_estimators/test_leader_picker_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_estimators/test_murcko_scaffold_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_estimators/test_nearest_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_estimators/test_similarity_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.480758 molpipeline-0.8.2/tests/test_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_metrics/test_ignore_error_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.480758 molpipeline-0.8.2/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_utils/test_json_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/test_utils/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:16:51.480758 molpipeline-0.8.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/utils/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-23 10:16:43.000000 molpipeline-0.8.2/tests/utils/mock_element.py
```

### Comparing `molpipeline-0.8.1/LICENSE` & `molpipeline-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/PKG-INFO` & `molpipeline-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molpipeline
-Version: 0.8.1
+Version: 0.8.2
 Summary: Integration of rdkit functionality into sklearn pipelines.
 Author: Christian W. Feldmann, Jennifer Hemmerich, Jochen Sieg
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib>=1.3.0
 Requires-Dist: loguru
 Requires-Dist: numpy
```

### Comparing `molpipeline-0.8.1/README.md` & `molpipeline-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/__init__.py` & `molpipeline-0.8.2/molpipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/any2mol/string2mol.py` & `molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/any2mol/string2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/core.py` & `molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,32 +201,20 @@
                     f"Cannot set attribute {att_name} on {self.__class__.__name__}"
                 )
             setattr(self, att_name, att_value)
         return self
 
     @property
     def additional_attributes(self) -> dict[str, Any]:
-        """Any attribute relevant for recreating and exact copy, which is not a parameter.
-
-        Returns
-        -------
-        dict[str, Any]
-            Additional attributes.
-        """
+        """Any attribute relevant for recreating and exact copy, which is not a parameter."""
         return {}
 
     @property
     def n_jobs(self) -> int:
-        """Get the number of cores.
-
-        Returns
-        -------
-        int
-            Number of cores used for processing.
-        """
+        """Get the number of cores."""
         return self._n_jobs
 
     @n_jobs.setter
     def n_jobs(self, n_jobs: int) -> None:
         """Set the number of cores.
 
         Parameters
@@ -238,21 +226,15 @@
         -------
         None
         """
         self._n_jobs = check_available_cores(n_jobs)
 
     @property
     def requires_fitting(self) -> bool:
-        """Return whether the object requires fitting or not.
-
-        Returns
-        -------
-        bool
-            True if object requires fitting, else False.
-        """
+        """Return whether the object requires fitting or not."""
         return self._requires_fitting
 
     def finish(self) -> None:
         """Inform object that iteration has been finished. Does in most cases nothing.
 
         Called after all transform singles have been processed. From MolPipeline
         """
@@ -372,54 +354,30 @@
             Unique identifier of the PipelineElement.
         """
         super().__init__(name=name, n_jobs=n_jobs, uuid=uuid)
         self._is_fitted = False
 
     @property
     def input_type(self) -> str:
-        """Return the input type.
-
-        Returns
-        -------
-        str
-            Input type of the object.
-        """
+        """Return the input type."""
         return self._input_type
 
     @property
     def is_fitted(self) -> bool:
-        """Return whether the object is fitted or not.
-
-        Returns
-        -------
-        bool
-            True if object is fitted, else False.
-        """
+        """Return whether the object is fitted or not."""
         return self._is_fitted
 
     @property
     def output_type(self) -> str:
-        """Return the output type.
-
-        Returns
-        -------
-        str
-            Output type of the object.
-        """
+        """Return the output type."""
         return self._output_type
 
     @property
     def parameters(self) -> dict[str, Any]:
-        """Return the parameters of the object.
-
-        Returns
-        -------
-        dict[str, Any]
-            Object parameters as a dictionary.
-        """
+        """Return the parameters of the object."""
         return self.get_params()
 
     @parameters.setter
     def parameters(self, **parameters: dict[str, Any]) -> None:
         """Set the parameters of the object.
 
         Parameters
```

### Comparing `molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/mol2bitvector.py` & `molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/mol2any/mol2bitvector.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,21 +63,15 @@
             n_jobs=n_jobs,
             uuid=uuid,
         )
         self._return_as = return_as
 
     @property
     def n_bits(self) -> int:
-        """Get number of bits in (or size of) fingerprint.
-
-        Returns
-        -------
-        int
-            Number of bits in fingerprint.
-        """
+        """Get number of bits in (or size of) fingerprint."""
         return self._n_bits
 
     @overload
     def assemble_output(  # type: ignore
         self, value_list: Iterable[npt.NDArray[np.int_]]
     ) -> npt.NDArray[np.int_]: ...
 
@@ -299,32 +293,20 @@
         if use_features is not None:
             self._use_features = bool(use_features)
         super().set_params(**parameter_copy)
         return self
 
     @property
     def radius(self) -> int:
-        """Get radius of Morgan fingerprint.
-
-        Returns
-        -------
-        int
-            Radius of Morgan fingerprint.
-        """
+        """Get radius of Morgan fingerprint."""
         return self._radius
 
     @property
     def use_features(self) -> bool:
-        """Get whether to encode atoms by features or not.
-
-        Returns
-        -------
-        bool
-            Whether to encode atoms by features or not.
-        """
+        """Get whether to encode atoms by features or not."""
         return self._use_features
 
     @abc.abstractmethod
     def _explain_rdmol(self, mol_obj: RDKitMol) -> dict[int, list[tuple[int, int]]]:
         """Get central atom and radius of all features in molecule.
 
         Parameters
```

### Comparing `molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/mol2floatvector.py` & `molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/mol2any/mol2floatvector.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,21 +60,15 @@
             self._requires_fitting = True
         self._mean = None
         self._std = None
 
     @property
     @abc.abstractmethod
     def n_features(self) -> int:
-        """Return the number of features.
-
-        Returns
-        -------
-        int
-            Number of features.
-        """
+        """Return the number of features."""
 
     def assemble_output(
         self,
         value_list: Iterable[npt.NDArray[np.float_]],
     ) -> npt.NDArray[np.float_]:
         """Transform output of all transform_single operations to matrix.
```

### Comparing `molpipeline-0.8.1/molpipeline/abstract_pipeline_elements/mol2any/mol2string.py` & `molpipeline-0.8.2/molpipeline/abstract_pipeline_elements/mol2any/mol2string.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/any2mol/auto2mol.py` & `molpipeline-0.8.2/molpipeline/any2mol/auto2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/any2mol/bin2mol.py` & `molpipeline-0.8.2/molpipeline/any2mol/bin2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/any2mol/sdf2mol.py` & `molpipeline-0.8.2/molpipeline/any2mol/sdf2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/any2mol/smiles2mol.py` & `molpipeline-0.8.2/molpipeline/any2mol/smiles2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/error_handling.py` & `molpipeline-0.8.2/molpipeline/error_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -527,21 +527,15 @@
         if "fill_value" in parameter_copy:
             self.fill_value = parameter_copy.pop("fill_value")
         super().set_params(**parameter_copy)
         return self
 
     @property
     def error_filter(self) -> ErrorFilter:
-        """Get the ErrorFilter connected to this FilterReinserter.
-
-        Returns
-        -------
-        ErrorFilter
-            ErrorFilter used for filling removed values.
-        """
+        """Get the ErrorFilter connected to this FilterReinserter."""
         if self._error_filter is None:
             raise ValueError("ErrorFilter not set")
         return self._error_filter
 
     @error_filter.setter
     def error_filter(self, error_filter: ErrorFilter) -> None:
         """Set the ErrorFilter.
```

### Comparing `molpipeline-0.8.1/molpipeline/estimators/__init__.py` & `molpipeline-0.8.2/molpipeline/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/estimators/algorithm/connected_component_clustering.py` & `molpipeline-0.8.2/molpipeline/estimators/algorithm/connected_component_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/estimators/algorithm/union_find.py` & `molpipeline-0.8.2/molpipeline/estimators/algorithm/union_find.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/estimators/chemprop/abstract.py` & `molpipeline-0.8.2/molpipeline/estimators/chemprop/abstract.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/estimators/chemprop/component_wrapper.py` & `molpipeline-0.8.2/molpipeline/estimators/chemprop/component_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,21 +207,15 @@
         self.dropout = dropout
         self.activation = activation
         self.task_weights = task_weights
         self.threshold = threshold
 
     @property
     def input_dim(self) -> int:
-        """Get the dimension of input.
-
-        Returns
-        -------
-        int
-            The dimension of input.
-        """
+        """Get the dimension of input."""
         return self._input_dim
 
     @input_dim.setter
     def input_dim(self, value: int) -> None:
         """Set the dimension of input.
 
         Parameters
@@ -229,21 +223,15 @@
         value : int
             The dimension of input.
         """
         self._input_dim = value
 
     @property
     def n_tasks(self) -> int:
-        """Get the number of tasks.
-
-        Returns
-        -------
-        int
-            The number of tasks.
-        """
+        """Get the number of tasks."""
         return self._n_tasks
 
     @n_tasks.setter
     def n_tasks(self, value: int) -> None:
         """Set the number of tasks.
 
         Parameters
```

### Comparing `molpipeline-0.8.1/molpipeline/estimators/chemprop/lightning_wrapper.py` & `molpipeline-0.8.2/molpipeline/estimators/chemprop/lightning_wrapper.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/estimators/chemprop/models.py` & `molpipeline-0.8.2/molpipeline/estimators/chemprop/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,36 +74,24 @@
             n_jobs=n_jobs,
             **kwargs,
         )
         self._classes_ = None
 
     @property
     def classes_(self) -> npt.NDArray[np.int_]:
-        """Return the classes.
-
-        Returns
-        -------
-        npt.NDArray[np.int_]
-            The classes.
-        """
+        """Return the classes."""
         if not self._is_classifier():
             raise ValueError("Model is not a classifier.")
         if self._classes_ is None:
             raise ValueError("Classes are not set.")
         return self._classes_
 
     @property
     def _estimator_type(self) -> str:
-        """Return the estimator type.
-
-        Returns
-        -------
-        str
-            The estimator type.
-        """
+        """Return the estimator type."""
         if self._is_classifier():
             return "classifier"
         return "regressor"
 
     def _is_binary_classifier(self) -> bool:
         """Check if the model is a binary classifier.
```

### Comparing `molpipeline-0.8.1/molpipeline/estimators/chemprop/neural_fingerprint.py` & `molpipeline-0.8.2/molpipeline/estimators/chemprop/neural_fingerprint.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/estimators/connected_component_clustering.py` & `molpipeline-0.8.2/molpipeline/estimators/connected_component_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/estimators/leader_picker_clustering.py` & `molpipeline-0.8.2/molpipeline/estimators/leader_picker_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/estimators/murcko_scaffold_clustering.py` & `molpipeline-0.8.2/molpipeline/estimators/murcko_scaffold_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/estimators/nearest_neighbor.py` & `molpipeline-0.8.2/molpipeline/estimators/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/estimators/similarity_transformation.py` & `molpipeline-0.8.2/molpipeline/estimators/similarity_transformation.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/metrics/ignore_error_scorer.py` & `molpipeline-0.8.2/molpipeline/metrics/ignore_error_scorer.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/mol2any/__init__.py` & `molpipeline-0.8.2/molpipeline/mol2any/__init__.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/mol2any/mol2bin.py` & `molpipeline-0.8.2/molpipeline/mol2any/mol2bin.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/mol2any/mol2chemprop.py` & `molpipeline-0.8.2/molpipeline/mol2any/mol2chemprop.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/mol2any/mol2concatinated_vector.py` & `molpipeline-0.8.2/molpipeline/mol2any/mol2concatinated_vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,21 +65,15 @@
         self._requires_fitting = any(
             element[1]._requires_fitting for element in element_list
         )
         self.set_params(**kwargs)
 
     @property
     def element_list(self) -> list[tuple[str, MolToAnyPipelineElement]]:
-        """Get pipeline elements.
-
-        Returns
-        -------
-        list[tuple[str, MolToAnyPipelineElement]]
-            List of pipeline elements.
-        """
+        """Get pipeline elements."""
         return self._element_list
 
     def get_params(self, deep: bool = True) -> dict[str, Any]:
         """Return all parameters defining the object.
 
         Parameters
         ----------
```

### Comparing `molpipeline-0.8.1/molpipeline/mol2any/mol2inchi.py` & `molpipeline-0.8.2/molpipeline/mol2any/mol2inchi.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/mol2any/mol2morgan_fingerprint.py` & `molpipeline-0.8.2/molpipeline/mol2any/mol2morgan_fingerprint.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/mol2any/mol2net_charge.py` & `molpipeline-0.8.2/molpipeline/mol2any/mol2net_charge.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,32 +63,20 @@
             name=name,
             n_jobs=n_jobs,
             uuid=uuid,
         )
 
     @property
     def n_features(self) -> int:
-        """Return the number of features.
-
-        Returns
-        -------
-        int
-            Number of features.
-        """
+        """Return the number of features."""
         return len(self._descriptor_list)
 
     @property
     def descriptor_list(self) -> list[str]:
-        """Return a copy of the descriptor list.
-
-        Returns
-        -------
-        list[str]
-            List of descriptor names.
-        """
+        """Return a copy of the descriptor list."""
         return self._descriptor_list[:]
 
     def _get_net_charge_gasteiger(
         self, value: RDKitMol
     ) -> npt.NDArray[np.float_] | InvalidInstance:
         """Transform a single molecule to it's net charge using Gasteiger charges.
```

### Comparing `molpipeline-0.8.1/molpipeline/mol2any/mol2rdkit_phys_chem.py` & `molpipeline-0.8.2/molpipeline/mol2any/mol2rdkit_phys_chem.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 except ImportError:
     from typing_extensions import Self
 
 import copy
 
 import numpy as np
 import numpy.typing as npt
+from loguru import logger
 from rdkit import Chem
 from rdkit.Chem import Descriptors
 from sklearn.preprocessing import StandardScaler
 
 from molpipeline.abstract_pipeline_elements.core import InvalidInstance
 from molpipeline.abstract_pipeline_elements.mol2any.mol2floatvector import (
     MolToDescriptorPipelineElement,
@@ -39,64 +40,87 @@
     """PipelineElement for creating a Descriptor vector based on RDKit phys-chem properties."""
 
     _descriptor_list: list[str]
 
     def __init__(
         self,
         descriptor_list: Optional[list[str]] = None,
+        return_with_errors: bool = False,
         standardizer: Optional[AnyTransformer] = StandardScaler(),
+        log_exceptions: bool = True,
         name: str = "Mol2RDKitPhysChem",
         n_jobs: int = 1,
         uuid: Optional[str] = None,
     ) -> None:
         """Initialize MolToRDKitPhysChem.
 
         Parameters
         ----------
         descriptor_list: Optional[list[str]], optional (default=None)
             List of descriptor names to calculate. If None, DEFAULT_DESCRIPTORS are used.
+        return_with_errors: bool, optional (default = False)
+            If False, the pipeline element will return an InvalidInstance if any error occurs during calculations.
+            If True, the pipeline element will return a vector with NaN values for failed descriptor calculations.
         standardizer: Optional[AnyTransformer], optional (default=StandardScaler())
             Standardizer to use.
+        log_exceptions: bool, optional (default=True)
+            If True, traceback of exceptions occurring during descriptor calculation are logged.
         name: str, optional (default="Mol2RDKitPhysChem")
             Name of the PipelineElement.
         n_jobs: int, optional (default=1)
             Number of jobs to use for parallelization.
         uuid: Optional[str], optional (default=None)
             UUID of the PipelineElement. If None, a new UUID is generated.
         """
-        self._descriptor_list = descriptor_list or DEFAULT_DESCRIPTORS
+        self.descriptor_list = descriptor_list  # type: ignore
+        self._return_with_errors = return_with_errors
+        self._log_exceptions = log_exceptions
         super().__init__(
             standardizer=standardizer,
             name=name,
             n_jobs=n_jobs,
             uuid=uuid,
         )
 
     @property
     def n_features(self) -> int:
-        """Return the number of features.
-
-        Returns
-        -------
-        int
-            Number of features.
-        """
+        """Return the number of features."""
         return len(self._descriptor_list)
 
     @property
     def descriptor_list(self) -> list[str]:
-        """Return a copy of the descriptor list.
-
-        Returns
-        -------
-        list[str]
-            List of descriptor names.
-        """
+        """Return a copy of the descriptor list."""
         return self._descriptor_list[:]
 
+    @descriptor_list.setter
+    def descriptor_list(self, descriptor_list: list[str] | None) -> None:
+        """Set the descriptor list.
+
+        Parameters
+        ----------
+        descriptor_list: list[str] | None
+            List of descriptor names to calculate. If None, DEFAULT_DESCRIPTORS are used.
+
+        Raises
+        ------
+        ValueError
+            If an unknown descriptor name is used.
+        """
+        if descriptor_list is None or descriptor_list is DEFAULT_DESCRIPTORS:
+            # if None or DEFAULT_DESCRIPTORS are used, set the default descriptors
+            self._descriptor_list = DEFAULT_DESCRIPTORS
+        else:
+            # check all user defined descriptors are valid
+            for descriptor_name in descriptor_list:
+                if descriptor_name not in RDKIT_DESCRIPTOR_DICT:
+                    raise ValueError(
+                        f"Unknown descriptor function with name: {descriptor_name}"
+                    )
+            self._descriptor_list = descriptor_list
+
     def pretransform_single(
         self, value: RDKitMol
     ) -> Union[npt.NDArray[np.float_], InvalidInstance]:
         """Transform a single molecule to a descriptor vector.
 
         Parameters
         ----------
@@ -104,18 +128,23 @@
             RDKit molecule to transform.
 
         Returns
         -------
         Optional[npt.NDArray[np.float_]]
             Descriptor vector for given molecule. None if calculation failed.
         """
-        vec = np.array(
-            [RDKIT_DESCRIPTOR_DICT[name](value) for name in self._descriptor_list]
-        )
-        if np.any(np.isnan(vec)):
+        vec = np.full((len(self._descriptor_list),), np.nan)
+        for i, name in enumerate(self._descriptor_list):
+            descriptor_func = RDKIT_DESCRIPTOR_DICT[name]
+            try:
+                vec[i] = descriptor_func(value)
+            except Exception:  # pylint: disable=broad-except
+                if self._log_exceptions:
+                    logger.exception(f"Failed calculating descriptor: {name}")
+        if not self._return_with_errors and np.any(np.isnan(vec)):
             return InvalidInstance(self.uuid, "NaN in descriptor vector", self.name)
         return vec
 
     def get_params(self, deep: bool = True) -> dict[str, Any]:
         """Get the parameters of the pipeline element.
 
         Parameters
@@ -127,16 +156,20 @@
         -------
         dict[str, Any]
             Parameter of the pipeline element.
         """
         parent_dict = dict(super().get_params(deep=deep))
         if deep:
             parent_dict["descriptor_list"] = copy.deepcopy(self._descriptor_list)
+            parent_dict["return_with_errors"] = copy.deepcopy(self._return_with_errors)
+            parent_dict["log_exceptions"] = copy.deepcopy(self._log_exceptions)
         else:
             parent_dict["descriptor_list"] = self._descriptor_list
+            parent_dict["return_with_errors"] = self._return_with_errors
+            parent_dict["log_exceptions"] = self._log_exceptions
         return parent_dict
 
     def set_params(self, **parameters: dict[str, Any]) -> Self:
         """Set parameters.
 
         Parameters
         ----------
@@ -145,12 +178,14 @@
 
         Returns
         -------
         Self
             Self
         """
         parameters_shallow_copy = dict(parameters)
-        descriptor_list = parameters_shallow_copy.pop("descriptor_list", None)
-        if descriptor_list is not None:
-            self._descriptor_list = descriptor_list  # type: ignore
+        params_list = ["descriptor_list", "return_with_errors", "log_exceptions"]
+        for param_name in params_list:
+            if param_name in parameters:
+                setattr(self, f"_{param_name}", parameters[param_name])
+                parameters_shallow_copy.pop(param_name)
         super().set_params(**parameters_shallow_copy)
         return self
```

### Comparing `molpipeline-0.8.1/molpipeline/mol2any/mol2smiles.py` & `molpipeline-0.8.2/molpipeline/mol2any/mol2smiles.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/mol2mol/__init__.py` & `molpipeline-0.8.2/molpipeline/mol2mol/__init__.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/mol2mol/filter.py` & `molpipeline-0.8.2/molpipeline/mol2mol/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,15 @@
         return value
 
 
 class InorganicsFilter(_MolToMolPipelineElement):
     """Filters Molecules which do not contain any organic (i.e. Carbon) atoms."""
 
     CARBON_INORGANICS = ["O=C=O", "[C-]#[O+]"]  # CO2 and CO are not organic
+    CARBON_INORGANICS_MAX_ATOMS = 3
 
     def __init__(
         self,
         name: str = "InorganicsFilter",
         n_jobs: int = 1,
         uuid: Optional[str] = None,
     ) -> None:
@@ -254,12 +255,14 @@
         OptionalMol
             Molecule if it contains carbon, else InvalidInstance.
         """
         if not any(atom.GetAtomicNum() == 6 for atom in value.GetAtoms()):
             return InvalidInstance(
                 self.uuid, "Molecule contains no organic atoms.", self.name
             )
-        smiles = Chem.MolToSmiles(value)
-        print(smiles)
-        if smiles in self.CARBON_INORGANICS:
-            return InvalidInstance(self.uuid, "Molecule is not organic.", self.name)
+
+        # Only check for inorganic molecules if the molecule is small enough
+        if value.GetNumAtoms() <= self.CARBON_INORGANICS_MAX_ATOMS:
+            smiles = Chem.MolToSmiles(value)
+            if smiles in self.CARBON_INORGANICS:
+                return InvalidInstance(self.uuid, "Molecule is not organic.", self.name)
         return value
```

### Comparing `molpipeline-0.8.1/molpipeline/mol2mol/reaction.py` & `molpipeline-0.8.2/molpipeline/mol2mol/reaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,21 +111,15 @@
             self.additive_list = parameters["additive_list"]  # type: ignore
         if "handle_multi" in parameters:
             self.handle_multi = parameters["handle_multi"]  # type: ignore
         return self
 
     @property
     def reaction(self) -> AllChem.ChemicalReaction:
-        """Get the reaction which is applied to the input molecule.
-
-        Returns
-        -------
-        AllChem.ChemicalReaction
-            Reaction which is applied to molecules.
-        """
+        """Get the reaction which is applied to the input molecule."""
         return self._reaction
 
     @reaction.setter
     def reaction(self, reaction: AllChem.ChemicalReaction) -> None:
         """Set the reaction which is applied to the input molecule.
 
         Parameters
```

### Comparing `molpipeline-0.8.1/molpipeline/mol2mol/scaffolds.py` & `molpipeline-0.8.2/molpipeline/mol2mol/scaffolds.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/mol2mol/standardization.py` & `molpipeline-0.8.2/molpipeline/mol2mol/standardization.py`

 * *Files 1% similar despite different names*

```diff
@@ -490,32 +490,20 @@
         super().__init__(name=name, n_jobs=n_jobs, uuid=uuid)
         if solvent_smiles_list is None:
             solvent_smiles_list = self.standard_solvent_smiles_list
         self.solvent_smiles_list = solvent_smiles_list
 
     @property
     def solvent_mol_list(self) -> list[RDKitMol]:
-        """Return molecule representation of smiles list.
-
-        Returns
-        -------
-        list[RDKitMol]
-            List of molecule objects to remove.
-        """
+        """Return molecule representation of smiles list."""
         return self._solvent_mol_list
 
     @property
     def solvent_smiles_list(self) -> list[str]:
-        """Return the smiles list.
-
-        Returns
-        -------
-        list[str]
-            List of SMILES of fragments to remove.
-        """
+        """Return the smiles list."""
         return self._solvent_smiles_list
 
     @solvent_smiles_list.setter
     def solvent_smiles_list(self, solvent_smiles_list: list[str]) -> None:
         """Set the smiles list.
 
         Parameters
```

### Comparing `molpipeline-0.8.1/molpipeline/pipeline/_molpipeline.py` & `molpipeline-0.8.2/molpipeline/pipeline/_molpipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,64 +66,40 @@
         self._requires_fitting = any(
             element.requires_fitting for element in self._element_list
         )
         self.raise_nones = raise_nones
 
     @property
     def _filter_elements(self) -> list[ErrorFilter]:
-        """Get the elements which filter the input.
-
-        Returns
-        -------
-        list[ErrorFilter]
-            List of elements which filter the input.
-        """
+        """Get the elements which filter the input."""
         return [
             element
             for element in self._element_list
             if isinstance(element, ErrorFilter)
         ]
 
     @property
     def _filter_elements_agg(self) -> _MultipleErrorFilter:
-        """Get the aggregated filter element.
-
-        Returns
-        -------
-        _MultipleErrorFilter
-            Aggregated filter element.
-        """
+        """Get the aggregated filter element."""
         return _MultipleErrorFilter(self._filter_elements)
 
     @property
     def _transforming_elements(
         self,
     ) -> list[Union[TransformingPipelineElement, _MolPipeline]]:
-        """Get the elements which transform the input.
-
-        Returns
-        -------
-        list[Union[TransformingPipelineElement, _MolPipeline]]
-            List of elements which transform the input.
-        """
+        """Get the elements which transform the input."""
         return [
             element
             for element in self._element_list
             if isinstance(element, (TransformingPipelineElement, _MolPipeline))
         ]
 
     @property
     def n_jobs(self) -> int:
-        """Return the number of cores to use in transformation step.
-
-        Returns
-        -------
-        int
-            Number of cores used in transformation steps.
-        """
+        """Return the number of cores to use in transformation step."""
         return self._n_jobs
 
     @n_jobs.setter
     def n_jobs(self, requested_jobs: int) -> None:
         """Set the number of cores to use in transformation step.
 
         Parameters
@@ -136,21 +112,15 @@
         -------
         None
         """
         self._n_jobs = check_available_cores(requested_jobs)
 
     @property
     def parameters(self) -> dict[str, Any]:
-        """Get all parameters defining the object.
-
-        Returns
-        -------
-        dict[str, Any]
-            Dictionary containing the parameter names and corresponding values.
-        """
+        """Get all parameters defining the object."""
         return self.get_params()
 
     @parameters.setter
     def parameters(self, parameter_dict: dict[str, Any]) -> None:
         """Set parameters of the pipeline and pipeline elements.
 
         Parameters
@@ -162,21 +132,15 @@
         -------
         None
         """
         self.set_params(**parameter_dict)
 
     @property
     def requires_fitting(self) -> bool:
-        """Return whether the pipeline requires fitting.
-
-        Returns
-        -------
-        bool
-            True if the pipeline requires fitting, False otherwise.
-        """
+        """Return whether the pipeline requires fitting."""
         return self._requires_fitting
 
     def get_params(self, deep: bool = True) -> dict[str, Any]:
         """Get all parameters defining the object.
 
         Parameters
         ----------
@@ -223,21 +187,15 @@
             self.name = str(parameter_dict["name"])
         if "raise_nones" in parameter_dict:
             self.raise_nones = bool(parameter_dict["raise_nones"])
         return self
 
     @property
     def element_list(self) -> list[ABCPipelineElement]:
-        """Get a shallow copy from the list of pipeline elements.
-
-        Returns
-        -------
-        list[ABCPipelineElement]
-            List of pipeline elements.
-        """
+        """Get a shallow copy from the list of pipeline elements."""
         return self._element_list[:]  # [:] to create shallow copy.
 
     def _get_meta_element_list(
         self,
     ) -> list[Union[ABCPipelineElement, _MolPipeline]]:
         """Merge elements which do not require fitting to a meta element which improves parallelization.
```

### Comparing `molpipeline-0.8.1/molpipeline/pipeline/_skl_pipeline.py` & `molpipeline-0.8.2/molpipeline/pipeline/_skl_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 """Defines a pipeline is exposed to the user, accessible via pipeline."""
 
 from __future__ import annotations
 
 from typing import Any, Iterable, List, Literal, Optional, Tuple, TypeVar, Union
 
+
 try:
     from typing import Self  # type: ignore[attr-defined]
 except ImportError:
     from typing_extensions import Self
 
 import joblib
 import numpy as np
 import numpy.typing as npt
 from loguru import logger
 from sklearn.base import _fit_context  # pylint: disable=protected-access
 from sklearn.base import clone
 from sklearn.pipeline import Pipeline as _Pipeline
 from sklearn.pipeline import _final_estimator_has, _fit_transform_one
-from sklearn.utils import Bunch, _print_elapsed_time
+from sklearn.utils import Bunch
 from sklearn.utils.metadata_routing import (
     _routing_enabled,  # pylint: disable=protected-access
 )
 from sklearn.utils.metadata_routing import process_routing
 from sklearn.utils.metaestimators import available_if
 from sklearn.utils.validation import check_memory
 
 from molpipeline.abstract_pipeline_elements.core import ABCPipelineElement
 from molpipeline.error_handling import ErrorFilter, FilterReinserter
 from molpipeline.pipeline._molpipeline import _MolPipeline
 from molpipeline.post_prediction import (
     PostPredictionTransformation,
     PostPredictionWrapper,
 )
+from molpipeline.utils.logging import print_elapsed_time
 from molpipeline.utils.molpipeline_types import (
     AnyElement,
     AnyPredictor,
     AnyStep,
     AnyTransformer,
 )
 from molpipeline.utils.value_checks import is_empty
@@ -177,21 +179,15 @@
 
         if with_final and last_element[2] is not None:
             if last_element[2] != "passthrough":
                 yield last_element
 
     @property
     def _estimator_type(self) -> Any:
-        """Return the estimator type.
-
-        Returns
-        -------
-        Any
-            The estimator type.
-        """
+        """Return the estimator type."""
         if self._final_estimator is None or self._final_estimator == "passthrough":
             return None
         if hasattr(self._final_estimator, "_estimator_type"):
             # pylint: disable=protected-access
             return self._final_estimator._estimator_type
         return None
 
@@ -201,21 +197,15 @@
     ) -> Union[
         Literal["passthrough"],
         AnyTransformer,
         AnyPredictor,
         _MolPipeline,
         ABCPipelineElement,
     ]:
-        """Return the lst estimator which is not a PostprocessingTransformer.
-
-        Returns
-        -------
-        Union[Literal["passthrough"], AnyTransformer, AnyPredictor, _MolPipeline, ABCPipelineElement]
-            The last estimator which is not a PostprocessingTransformer.
-        """
+        """Return the lst estimator which is not a PostprocessingTransformer."""
         element_list = list(self._agg_non_postpred_steps())
         last_element = element_list[-1]
         return last_element[2]
 
     # pylint: disable=too-many-locals,too-many-branches
     def _fit(
         self,
@@ -248,15 +238,15 @@
         # Set up the memory
         memory: joblib.Memory = check_memory(self.memory)
 
         fit_transform_one_cached = memory.cache(_fit_transform_one)
         for step in self._iter(with_final=False, filter_passthrough=False):
             step_idx, name, transformer = step
             if transformer is None or transformer == "passthrough":
-                with _print_elapsed_time("Pipeline", self._log_message(step_idx)):
+                with print_elapsed_time("Pipeline", self._log_message(step_idx)):
                     continue
 
             if hasattr(memory, "location") and memory.location is None:
                 # we do not clone when caching is disabled to
                 # preserve backward compatibility
                 cloned_transformer = transformer
             else:
@@ -465,15 +455,15 @@
         Returns
         -------
         self : object
             Pipeline with fitted steps.
         """
         routed_params = self._check_method_params(method="fit", props=fit_params)
         Xt, yt = self._fit(X, y, routed_params)  # pylint: disable=invalid-name
-        with _print_elapsed_time("Pipeline", self._log_message(len(self.steps) - 1)):
+        with print_elapsed_time("Pipeline", self._log_message(len(self.steps) - 1)):
             if self._final_estimator != "passthrough":
                 if is_empty(Xt):
                     logger.warning(
                         "All input rows were filtered out! Model is not fitted!"
                     )
                 else:
                     fit_params_last_step = routed_params[self.steps[-1][0]]
@@ -536,15 +526,15 @@
         -------
         Xt : ndarray of shape (n_samples, n_transformed_features)
             Transformed samples.
         """
         routed_params = self._check_method_params(method="fit_transform", props=params)
         iter_input, iter_label = self._fit(X, y, routed_params)
         last_step = self._final_estimator
-        with _print_elapsed_time("Pipeline", self._log_message(len(self.steps) - 1)):
+        with print_elapsed_time("Pipeline", self._log_message(len(self.steps) - 1)):
             if last_step == "passthrough":
                 pass
             elif is_empty(iter_input):
                 logger.warning("All input rows were filtered out! Model is not fitted!")
             else:
                 last_step_params = routed_params[self.steps[-1][0]]
                 if hasattr(last_step, "fit_transform"):
@@ -656,15 +646,15 @@
         """
         routed_params = self._check_method_params(method="fit_predict", props=params)
         iter_input, iter_label = self._fit(
             X, y, routed_params
         )  # pylint: disable=invalid-name
 
         params_last_step = routed_params[self.steps[-1][0]]
-        with _print_elapsed_time("Pipeline", self._log_message(len(self.steps) - 1)):
+        with print_elapsed_time("Pipeline", self._log_message(len(self.steps) - 1)):
             if self._final_estimator == "passthrough":
                 y_pred = iter_input
             elif is_empty(iter_input):
                 logger.warning("All input rows were filtered out! Model is not fitted!")
                 iter_input = []
                 y_pred = []
             elif hasattr(self._final_estimator, "fit_predict"):
@@ -832,21 +822,15 @@
             )
         for _, post_element in self._post_processing_steps():
             iter_input = post_element.transform(iter_input)
         return iter_input
 
     @property
     def classes_(self) -> list[Any] | npt.NDArray[Any]:
-        """Return the classes of the last element, which is not a PostPredictionTransformation.
-
-        Returns
-        -------
-        list[Any] | npt.NDArray[Any]
-            The classes of the last element.
-        """
+        """Return the classes of the last element, which is not a PostPredictionTransformation."""
         check_last = [
             step
             for step in self.steps
             if not isinstance(step[1], PostPredictionTransformation)
         ]
         last_step = check_last[-1][1]
         if last_step == "passthrough":
```

### Comparing `molpipeline-0.8.1/molpipeline/post_prediction.py` & `molpipeline-0.8.2/molpipeline/post_prediction.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/utils/json_operations.py` & `molpipeline-0.8.2/molpipeline/utils/json_operations.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/utils/kernel.py` & `molpipeline-0.8.2/molpipeline/utils/kernel.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/utils/matrices.py` & `molpipeline-0.8.2/molpipeline/utils/matrices.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/utils/molpipeline_types.py` & `molpipeline-0.8.2/molpipeline/utils/molpipeline_types.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/utils/multi_proc.py` & `molpipeline-0.8.2/molpipeline/utils/multi_proc.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/utils/substructure_handling.py` & `molpipeline-0.8.2/molpipeline/utils/substructure_handling.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline/utils/value_checks.py` & `molpipeline-0.8.2/molpipeline/utils/value_checks.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/molpipeline.egg-info/PKG-INFO` & `molpipeline-0.8.2/molpipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molpipeline
-Version: 0.8.1
+Version: 0.8.2
 Summary: Integration of rdkit functionality into sklearn pipelines.
 Author: Christian W. Feldmann, Jennifer Hemmerich, Jochen Sieg
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib>=1.3.0
 Requires-Dist: loguru
 Requires-Dist: numpy
```

### Comparing `molpipeline-0.8.1/molpipeline.egg-info/SOURCES.txt` & `molpipeline-0.8.2/molpipeline.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 molpipeline/mol2mol/standardization.py
 molpipeline/pipeline/__init__.py
 molpipeline/pipeline/_molpipeline.py
 molpipeline/pipeline/_skl_pipeline.py
 molpipeline/utils/__init__.py
 molpipeline/utils/json_operations.py
 molpipeline/utils/kernel.py
+molpipeline/utils/logging.py
 molpipeline/utils/matrices.py
 molpipeline/utils/molpipeline_types.py
 molpipeline/utils/multi_proc.py
 molpipeline/utils/substructure_handling.py
 molpipeline/utils/value_checks.py
 test_extras/__init__.py
 test_extras/test_chemprop/__init__.py
@@ -102,10 +103,11 @@
 tests/test_estimators/test_algorithm/__init__.py
 tests/test_estimators/test_algorithm/test_connected_component_clustering.py
 tests/test_estimators/test_algorithm/test_union_find.py
 tests/test_metrics/__init__.py
 tests/test_metrics/test_ignore_error_scorer.py
 tests/test_utils/__init__.py
 tests/test_utils/test_json_operations.py
+tests/test_utils/test_logging.py
 tests/utils/__init__.py
 tests/utils/fingerprints.py
 tests/utils/mock_element.py
```

### Comparing `molpipeline-0.8.1/pyproject.toml` & `molpipeline-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 name = "molpipeline"
 authors = [
     {name = "Christian W. Feldmann"},
     {name = "Jennifer Hemmerich"},
     {name = "Jochen Sieg"}
 ]
 description = "Integration of rdkit functionality into sklearn pipelines."
-version = "0.8.1"
+version = "0.8.2"
 readme = "README.md"
 
 [tool.setuptools.dynamic]
 dependencies = {file = "requirements.txt"}
 
 [tool.setuptools.dynamic.optional-dependencies]
 all = {file = ["requirements_chemprop.txt", "requirements_notebooks.txt"]}
```

### Comparing `molpipeline-0.8.1/test_extras/test_chemprop/test_abstract.py` & `molpipeline-0.8.2/test_extras/test_chemprop/test_abstract.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/test_extras/test_chemprop/test_chemprop_pipeline.py` & `molpipeline-0.8.2/test_extras/test_chemprop/test_chemprop_pipeline.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/test_extras/test_chemprop/test_component_wrapper.py` & `molpipeline-0.8.2/test_extras/test_chemprop/test_component_wrapper.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/test_extras/test_chemprop/test_lightning_wrapper.py` & `molpipeline-0.8.2/test_extras/test_chemprop/test_lightning_wrapper.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/test_extras/test_chemprop/test_models.py` & `molpipeline-0.8.2/test_extras/test_chemprop/test_models.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/test_extras/test_notebooks/test_notebooks.py` & `molpipeline-0.8.2/test_extras/test_notebooks/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_elements/test_any2mol/test_auto2mol.py` & `molpipeline-0.8.2/tests/test_elements/test_any2mol/test_auto2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_elements/test_any2mol/test_bin2mol.py` & `molpipeline-0.8.2/tests/test_elements/test_any2mol/test_bin2mol.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_elements/test_error_handling.py` & `molpipeline-0.8.2/tests/test_elements/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2bin.py` & `molpipeline-0.8.2/tests/test_elements/test_mol2any/test_mol2bin.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2concatenated.py` & `molpipeline-0.8.2/tests/test_elements/test_mol2any/test_mol2concatenated.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2inchi.py` & `molpipeline-0.8.2/tests/test_elements/test_mol2any/test_mol2inchi.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2morgan_fingerprint.py` & `molpipeline-0.8.2/tests/test_elements/test_mol2any/test_mol2morgan_fingerprint.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_elements/test_mol2any/test_mol2net_charge.py` & `molpipeline-0.8.2/tests/test_elements/test_mol2any/test_mol2net_charge.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_elements/test_mol2mol/test_mol2mol_filter.py` & `molpipeline-0.8.2/tests/test_elements/test_mol2mol/test_mol2mol_filter.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_elements/test_mol2mol/test_mol2mol_standardization.py` & `molpipeline-0.8.2/tests/test_elements/test_mol2mol/test_mol2mol_standardization.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_estimators/test_algorithm/test_connected_component_clustering.py` & `molpipeline-0.8.2/tests/test_estimators/test_algorithm/test_connected_component_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_estimators/test_algorithm/test_union_find.py` & `molpipeline-0.8.2/tests/test_estimators/test_algorithm/test_union_find.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_estimators/test_connected_component_clustering.py` & `molpipeline-0.8.2/tests/test_estimators/test_connected_component_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_estimators/test_leader_picker_clustering.py` & `molpipeline-0.8.2/tests/test_estimators/test_leader_picker_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_estimators/test_murcko_scaffold_clustering.py` & `molpipeline-0.8.2/tests/test_estimators/test_murcko_scaffold_clustering.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_estimators/test_nearest_neighbors.py` & `molpipeline-0.8.2/tests/test_estimators/test_nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_estimators/test_similarity_transformation.py` & `molpipeline-0.8.2/tests/test_estimators/test_similarity_transformation.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_metrics/test_ignore_error_scorer.py` & `molpipeline-0.8.2/tests/test_metrics/test_ignore_error_scorer.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_pipeline.py` & `molpipeline-0.8.2/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/test_utils/test_json_operations.py` & `molpipeline-0.8.2/tests/test_utils/test_json_operations.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/utils/fingerprints.py` & `molpipeline-0.8.2/tests/utils/fingerprints.py`

 * *Files identical despite different names*

### Comparing `molpipeline-0.8.1/tests/utils/mock_element.py` & `molpipeline-0.8.2/tests/utils/mock_element.py`

 * *Files identical despite different names*

