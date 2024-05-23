# Comparing `tmp/gemmapy-1.0.2.tar.gz` & `tmp/gemmapy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemmapy-1.0.2.tar", last modified: Wed May 22 00:24:19 2024, max compression
+gzip compressed data, was "gemmapy-1.0.3.tar", last modified: Thu May 23 02:40:05 2024, max compression
```

## Comparing `gemmapy-1.0.2.tar` & `gemmapy-1.0.3.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:19.016328 gemmapy-1.0.2/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    11357 2024-05-04 04:09:08.000000 gemmapy-1.0.2/LICENSE.md
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     1730 2024-05-22 00:24:19.016328 gemmapy-1.0.2/PKG-INFO
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     1306 2024-05-07 21:06:20.000000 gemmapy-1.0.2/README.rst
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:18.984327 gemmapy-1.0.2/gemmapy/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)       61 2024-05-04 04:09:08.000000 gemmapy-1.0.2/gemmapy/__init__.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    21984 2024-05-22 00:14:58.000000 gemmapy-1.0.2/gemmapy/_processors.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6768 2024-05-07 20:41:44.000000 gemmapy-1.0.2/gemmapy/_subprocessors.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)      936 2024-05-07 20:41:44.000000 gemmapy-1.0.2/gemmapy/_validators.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    89515 2024-05-17 06:20:47.000000 gemmapy-1.0.2/gemmapy/gemmapy_api.py
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:18.988327 gemmapy-1.0.2/gemmapy/sdk/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    13741 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/__init__.py
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:18.988327 gemmapy-1.0.2/gemmapy/sdk/api/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)      138 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/api/__init__.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)   268620 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/api/default_api.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    25975 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/api_client.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9213 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/configuration.py
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:19.016328 gemmapy-1.0.2/gemmapy/sdk/models/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    13544 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/__init__.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6156 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/annotation_search_result_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8608 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/annotation_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9891 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/annotation_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5987 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/api_info_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    24020 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/array_design_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    24987 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/array_design_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8819 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/audit_event_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7478 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/bibliographic_phenotypes_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    16799 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/bibliographic_reference_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    14982 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/bio_assay_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9742 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/bio_material_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10036 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/bio_sequence_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5992 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/category_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7293 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/characteristic_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6624 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/citation_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3104 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/composite_sequence_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6014 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/composite_sequence_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8528 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/contrast_result_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/database_entry_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5384 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/database_entry_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3052 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset1.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset10.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset2.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset3.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset4.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset5.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset6.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset7.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset8.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset9.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3064 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/dataset_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    15728 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/diff_ex_result_set_summary_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9056 2024-05-22 00:18:33.000000 gemmapy-1.0.2/gemmapy/sdk/models/differential_expression_analysis_result_set_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9659 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/differential_expression_analysis_result_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    14048 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/differential_expression_analysis_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5109 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/experiment_expression_levels_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9358 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/experimental_factor_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    15105 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/expression_experiment_set_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    28654 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/expression_experiment_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    31623 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/expression_experiment_with_search_result_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9207 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/external_database_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10910 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/factor_value_basic_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    16266 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/factor_value_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3104 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filter_arg_array_design.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3168 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filter_arg_expression_analysis_result_set.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3140 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filter_arg_expression_experiment.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10951 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_inferred_and_paginated_response_data_object_expression_experiment_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9152 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_array_design_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9362 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_composite_sequence_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10132 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_differential_expression_analysis_result_set_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9467 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_expression_experiment_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8907 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_gene_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    25633 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/geeq_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3040 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene1.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene2.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene3.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene4.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene5.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3052 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5754 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene_element_expressions_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7870 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene_ontology_term_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6956 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene_set_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9642 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/gene_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7056 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/measurement_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3208 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/one_of_search_result_value_object_object_result_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5194 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/ontology_term_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8221 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/paginated_response_data_object_composite_sequence_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8314 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/paginated_response_data_object_expression_experiment_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7818 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/paginated_response_data_object_gene_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9986 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/paginated_results_response_data_object_differential_expression_analysis_result_set_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8127 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/physical_location_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform1.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform2.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform3.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform4.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform5.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3068 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/platform_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/probe.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/quantitation_type.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3100 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/quantitation_type_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    17466 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/quantitation_type_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10454 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_annotation_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10489 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_array_design_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10384 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_category_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    12908 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_paginated_response_data_object_expression_experiment_with_search_result_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     9082 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_response_data_object_taxon_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10652 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_paginated_response_data_object_expression_experiment_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/query_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3884 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_api_info_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4099 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_annotation_search_result_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3978 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_array_design_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3945 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_bio_assay_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4187 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_differential_expression_analysis_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4143 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_experiment_expression_levels_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4033 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_gene_ontology_term_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3901 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_gene_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4033 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_physical_location_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3912 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_taxon_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3727 2024-05-22 00:18:34.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_long.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3959 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_set_annotation_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4025 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_set_quantitation_type_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3906 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_simple_svd_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4521 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/response_error_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/search_result_type.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7682 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/search_result_value_object_expression_experiment_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7127 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/search_result_value_object_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4833 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/search_results_response_data_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6838 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/search_settings_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5411 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/simple_svd_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3096 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/sort_arg_array_design.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3160 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/sort_arg_expression_analysis_result_set.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3132 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/sort_arg_expression_experiment.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     4439 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/sort_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    10286 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/statement_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3040 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxa.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon1.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon2.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon3.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon4.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon5.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon6.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon7.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon8.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon9.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon_arg.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     6759 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     8441 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/taxon_with_usage_statistics_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5162 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/vector_element_value_object.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     5078 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/models/well_composed_error_body.py
--rw-r--r--   0 omancarci (30067) pavlab   (30005)    13649 2024-05-22 00:18:35.000000 gemmapy-1.0.2/gemmapy/sdk/rest.py
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:19.016328 gemmapy-1.0.2/gemmapy.egg-info/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     1730 2024-05-22 00:24:18.000000 gemmapy-1.0.2/gemmapy.egg-info/PKG-INFO
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     7909 2024-05-22 00:24:18.000000 gemmapy-1.0.2/gemmapy.egg-info/SOURCES.txt
--rw-r--r--   0 omancarci (30067) pavlab   (30005)        1 2024-05-22 00:24:18.000000 gemmapy-1.0.2/gemmapy.egg-info/dependency_links.txt
--rw-r--r--   0 omancarci (30067) pavlab   (30005)      114 2024-05-22 00:24:18.000000 gemmapy-1.0.2/gemmapy.egg-info/requires.txt
--rw-r--r--   0 omancarci (30067) pavlab   (30005)        8 2024-05-22 00:24:18.000000 gemmapy-1.0.2/gemmapy.egg-info/top_level.txt
--rw-r--r--   0 omancarci (30067) pavlab   (30005)       81 2024-05-04 04:09:08.000000 gemmapy-1.0.2/pyproject.toml
--rw-r--r--   0 omancarci (30067) pavlab   (30005)      404 2024-05-22 00:24:19.016328 gemmapy-1.0.2/setup.cfg
-drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-22 00:24:19.016328 gemmapy-1.0.2/tests/
--rw-r--r--   0 omancarci (30067) pavlab   (30005)     3861 2024-05-17 23:46:21.000000 gemmapy-1.0.2/tests/test_basic.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-23 02:40:05.715144 gemmapy-1.0.3/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    11357 2024-05-04 04:09:08.000000 gemmapy-1.0.3/LICENSE.md
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     1730 2024-05-23 02:40:05.715144 gemmapy-1.0.3/PKG-INFO
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     1306 2024-05-07 21:06:20.000000 gemmapy-1.0.3/README.rst
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-23 02:40:05.691143 gemmapy-1.0.3/gemmapy/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)       61 2024-05-04 04:09:08.000000 gemmapy-1.0.3/gemmapy/__init__.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    22750 2024-05-23 02:28:38.000000 gemmapy-1.0.3/gemmapy/_processors.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6768 2024-05-07 20:41:44.000000 gemmapy-1.0.3/gemmapy/_subprocessors.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)      936 2024-05-07 20:41:44.000000 gemmapy-1.0.3/gemmapy/_validators.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    89515 2024-05-17 06:20:47.000000 gemmapy-1.0.3/gemmapy/gemmapy_api.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-23 02:40:05.691143 gemmapy-1.0.3/gemmapy/sdk/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    13741 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/__init__.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-23 02:40:05.691143 gemmapy-1.0.3/gemmapy/sdk/api/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)      138 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/api/__init__.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)   268620 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/api/default_api.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    25975 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/api_client.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9213 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/configuration.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-23 02:40:05.715144 gemmapy-1.0.3/gemmapy/sdk/models/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    13544 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/__init__.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6156 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/annotation_search_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8608 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/annotation_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9891 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/annotation_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5987 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/api_info_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    24020 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/array_design_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    24987 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/array_design_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8819 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/audit_event_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7478 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/bibliographic_phenotypes_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    16799 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/bibliographic_reference_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    14982 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/bio_assay_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9742 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/bio_material_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10036 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/bio_sequence_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5992 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/category_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7293 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/characteristic_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6624 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/citation_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3104 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/composite_sequence_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6014 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/composite_sequence_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8528 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/contrast_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/database_entry_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5384 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/database_entry_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3052 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/dataset.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/dataset1.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/dataset10.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/dataset2.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/dataset3.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-23 02:37:13.000000 gemmapy-1.0.3/gemmapy/sdk/models/dataset4.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/dataset5.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/dataset6.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/dataset7.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/dataset8.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/dataset9.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3064 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/dataset_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    15728 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/diff_ex_result_set_summary_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9056 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/differential_expression_analysis_result_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9659 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/differential_expression_analysis_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    14048 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/differential_expression_analysis_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5109 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/experiment_expression_levels_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9358 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/experimental_factor_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    15105 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/expression_experiment_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    28654 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    31623 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/expression_experiment_with_search_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9207 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/external_database_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10910 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/factor_value_basic_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    16266 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/factor_value_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3104 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/filter_arg_array_design.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3168 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/filter_arg_expression_analysis_result_set.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3140 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/filter_arg_expression_experiment.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10951 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/filtered_and_inferred_and_paginated_response_data_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9152 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/filtered_and_paginated_response_data_object_array_design_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9362 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/filtered_and_paginated_response_data_object_composite_sequence_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10132 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/filtered_and_paginated_response_data_object_differential_expression_analysis_result_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9467 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/filtered_and_paginated_response_data_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8907 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/filtered_and_paginated_response_data_object_gene_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    25633 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/geeq_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3040 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/gene.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/gene1.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/gene2.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/gene3.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/gene4.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/gene5.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3052 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/gene_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5754 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/gene_element_expressions_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7870 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/gene_ontology_term_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6956 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/gene_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9642 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/gene_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7056 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/measurement_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3208 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/one_of_search_result_value_object_object_result_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5194 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/ontology_term_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8221 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/paginated_response_data_object_composite_sequence_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8314 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/paginated_response_data_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7818 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/paginated_response_data_object_gene_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9986 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/paginated_results_response_data_object_differential_expression_analysis_result_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8127 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/physical_location_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/platform.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/platform1.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/platform2.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/platform3.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/platform4.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/platform5.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3068 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/platform_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/probe.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/quantitation_type.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3100 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/quantitation_type_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    17466 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/quantitation_type_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10454 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_annotation_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10489 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_array_design_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10384 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_category_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    12908 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_paginated_response_data_object_expression_experiment_with_search_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9082 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/queried_and_filtered_and_inferred_response_data_object_taxon_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10652 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/queried_and_filtered_and_paginated_response_data_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/query_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3884 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_api_info_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4099 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_annotation_search_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3978 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_array_design_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3945 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_bio_assay_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4187 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_differential_expression_analysis_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4143 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_experiment_expression_levels_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4033 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_gene_ontology_term_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3901 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_gene_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4033 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_physical_location_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3912 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_taxon_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3727 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_long.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3959 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_set_annotation_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4025 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_set_quantitation_type_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3906 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_simple_svd_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4521 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/response_error_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/search_result_type.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7682 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/search_result_value_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7127 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/search_result_value_object_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4833 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/search_results_response_data_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6838 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/search_settings_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5411 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/simple_svd_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3096 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/sort_arg_array_design.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3160 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/sort_arg_expression_analysis_result_set.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3132 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/sort_arg_expression_experiment.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4439 2024-05-23 02:37:14.000000 gemmapy-1.0.3/gemmapy/sdk/models/sort_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10286 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/statement_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3040 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxa.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon1.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon2.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon3.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon4.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon5.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon6.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon7.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon8.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon9.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6759 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8441 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/taxon_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5162 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/vector_element_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5078 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/models/well_composed_error_body.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    13649 2024-05-23 02:37:15.000000 gemmapy-1.0.3/gemmapy/sdk/rest.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-23 02:40:05.715144 gemmapy-1.0.3/gemmapy.egg-info/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     1730 2024-05-23 02:40:05.000000 gemmapy-1.0.3/gemmapy.egg-info/PKG-INFO
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7909 2024-05-23 02:40:05.000000 gemmapy-1.0.3/gemmapy.egg-info/SOURCES.txt
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)        1 2024-05-23 02:40:05.000000 gemmapy-1.0.3/gemmapy.egg-info/dependency_links.txt
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)      114 2024-05-23 02:40:05.000000 gemmapy-1.0.3/gemmapy.egg-info/requires.txt
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)        8 2024-05-23 02:40:05.000000 gemmapy-1.0.3/gemmapy.egg-info/top_level.txt
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)       81 2024-05-04 04:09:08.000000 gemmapy-1.0.3/pyproject.toml
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)      404 2024-05-23 02:40:05.715144 gemmapy-1.0.3/setup.cfg
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-23 02:40:05.715144 gemmapy-1.0.3/tests/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3857 2024-05-23 01:47:38.000000 gemmapy-1.0.3/tests/test_basic.py
```

### Comparing `gemmapy-1.0.2/LICENSE.md` & `gemmapy-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/PKG-INFO` & `gemmapy-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemmapy
-Version: 1.0.2
+Version: 1.0.3
 Summary: a Python Wrapper for the Gemma API
 Keywords: gemma,bioinformatics
 Requires-Python: >3.10
 License-File: LICENSE.md
 Requires-Dist: certifi>=14.05.14
 Requires-Dist: six>=1.10
 Requires-Dist: python_dateutil>=2.5.3
```

### Comparing `gemmapy-1.0.2/README.rst` & `gemmapy-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/_processors.py` & `gemmapy-1.0.3/gemmapy/_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,58 +380,69 @@
 
 def process_expression(d, dataset, api):
     # dataset 2 is an example why this more complex renaming is needed
     # check a non gsm study too since R's make names might be handling
     # more non-uniformities
     df = sub.read_tsv(d)
     m_cols = list(df.columns)
-    samples = api.raw.get_dataset_samples(dataset).data
-    sample_ids = sub.field_in_list(samples,"sample",'name')
-    sample_names = sub.field_in_list(samples,"name")
+    # we use the order returned by get_dataset_samples as authoritative which makes
+    # it a bit awkward when we need to access a property left out of the processed output
+    # this could be simplified by ordering by ids but I don't want to break
+    # get_dataseset_samples supremacy in case ordering changes later
+    # R package makes this easier by appending raw outputs to every processed
+    # results. we don't do that here so calling twice is necessary
+    samples = api.get_dataset_samples(dataset)
+    samples_raw = api.raw.get_dataset_samples(dataset).data
+    
+    raw_ids = sub.field_in_list(samples_raw,'sample','id')
+    sample_internal_names = sub.field_in_list(samples_raw,'sample','name')
+    sample_internal_names = sub.match_by(sample_internal_names, samples.sample_ID, raw_ids)
     
-    sample_ids = [x.replace("|",".") for x in sample_ids]
+    sample_names = samples.sample_name
+    
+    sample_internal_names = [x.replace("|",".") for x in sample_internal_names]
     
     def find_match(x):
         match = None
         for i in range(len(m_cols)):
             if m_cols[i].find(x+"_") != -1:
                 match = i
         return match
     
-    sample_matches = [find_match(x) for x in sample_ids]
+    sample_matches = [find_match(x) for x in sample_internal_names]
     
     
     rename_dict = sub.make_dict([m_cols[i] for i in sample_matches],sample_names)
 
     df = df.rename(columns = rename_dict)
     
     assert all(sub.list_in_list(sample_names,list(df.columns)))
     
     df = df.drop(columns=['Sequence', 'GemmaId'], errors='ignore')
     
-    non_samples = [x for x in list(df.columns) if not x in sample_names]
-    df = df.reindex(columns = non_samples + sample_names)
+    non_samples = [x for x in list(df.columns) if not x in list(sample_names)]
+    df = df.reindex(columns = non_samples +list(sample_names))
     
     return df
 
 def process_samples(d:list):
-    
+
     df = pd.DataFrame({
         "sample_name": sub.field_in_list(d,"name"),
         "sample_ID": sub.field_in_list(d,"sample",'id'),
         "sample_description": sub.field_in_list(d,"description"),
         "sample_outlier": sub.field_in_list(d,"outlier"),
         "sample_accession": sub.field_in_list(d,"accession","accession"),
         "sample_database": sub.field_in_list(d,"accession","external_database",'name'),
         "sample_characteristics": [sub.process_CharacteristicValueObject(x).drop("value_ID",axis = 1) 
                                    for x in sub.field_in_list(d,"sample","characteristics")],
         "sample_factor_values": [sub.process_FactorValueValueObject_list(x)
                                 for x in sub.field_in_list(d,"sample","factor_value_objects")]
         
-        })
+        }).sort_values(by= ['sample_ID'],ignore_index=True)
     
     return df
 
 def process_datasets(d:list):
     df = pd.DataFrame({
         "experiment_short_name": sub.field_in_list(d,"short_name"),
         "experiment_name": sub.field_in_list(d,"name"),
```

### Comparing `gemmapy-1.0.2/gemmapy/_subprocessors.py` & `gemmapy-1.0.3/gemmapy/_subprocessors.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/_validators.py` & `gemmapy-1.0.3/gemmapy/_validators.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/gemmapy_api.py` & `gemmapy-1.0.3/gemmapy/gemmapy_api.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/__init__.py` & `gemmapy-1.0.3/gemmapy/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/api/default_api.py` & `gemmapy-1.0.3/gemmapy/sdk/api/default_api.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/api_client.py` & `gemmapy-1.0.3/gemmapy/sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'gemmapy/1.0.2'
+        self.user_agent = 'gemmapy/1.0.3'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `gemmapy-1.0.2/gemmapy/sdk/configuration.py` & `gemmapy-1.0.3/gemmapy/sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/__init__.py` & `gemmapy-1.0.3/gemmapy/sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/annotation_search_result_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/annotation_search_result_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/annotation_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/annotation_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/annotation_with_usage_statistics_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/annotation_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/api_info_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/api_info_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/array_design_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/array_design_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/array_design_with_usage_statistics_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/array_design_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/audit_event_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/audit_event_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/bibliographic_phenotypes_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/bibliographic_phenotypes_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/bibliographic_reference_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/bibliographic_reference_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/bio_assay_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/bio_assay_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/bio_material_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/bio_material_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/bio_sequence_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/bio_sequence_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/category_with_usage_statistics_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/category_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/characteristic_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/characteristic_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/citation_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/citation_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/composite_sequence_arg.py` & `gemmapy-1.0.3/gemmapy/sdk/models/composite_sequence_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/composite_sequence_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/composite_sequence_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/contrast_result_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/contrast_result_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/database_entry_arg.py` & `gemmapy-1.0.3/gemmapy/sdk/models/database_entry_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/database_entry_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/database_entry_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/dataset.py` & `gemmapy-1.0.3/gemmapy/sdk/models/dataset.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/dataset1.py` & `gemmapy-1.0.3/gemmapy/sdk/models/dataset1.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/dataset10.py` & `gemmapy-1.0.3/gemmapy/sdk/models/dataset10.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/dataset2.py` & `gemmapy-1.0.3/gemmapy/sdk/models/dataset2.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/dataset3.py` & `gemmapy-1.0.3/gemmapy/sdk/models/dataset3.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/dataset4.py` & `gemmapy-1.0.3/gemmapy/sdk/models/dataset4.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/dataset5.py` & `gemmapy-1.0.3/gemmapy/sdk/models/dataset5.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/dataset6.py` & `gemmapy-1.0.3/gemmapy/sdk/models/dataset6.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/dataset7.py` & `gemmapy-1.0.3/gemmapy/sdk/models/dataset7.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/dataset8.py` & `gemmapy-1.0.3/gemmapy/sdk/models/dataset8.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/dataset9.py` & `gemmapy-1.0.3/gemmapy/sdk/models/dataset9.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/dataset_arg.py` & `gemmapy-1.0.3/gemmapy/sdk/models/dataset_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/diff_ex_result_set_summary_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/diff_ex_result_set_summary_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/differential_expression_analysis_result_set_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/differential_expression_analysis_result_set_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/differential_expression_analysis_result_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/differential_expression_analysis_result_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/differential_expression_analysis_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/differential_expression_analysis_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/experiment_expression_levels_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/experiment_expression_levels_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/experimental_factor_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/experimental_factor_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/expression_experiment_set_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/expression_experiment_set_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/expression_experiment_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/expression_experiment_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/expression_experiment_with_search_result_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/expression_experiment_with_search_result_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/external_database_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/external_database_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/factor_value_basic_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/factor_value_basic_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/factor_value_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/factor_value_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/filter_arg_array_design.py` & `gemmapy-1.0.3/gemmapy/sdk/models/filter_arg_array_design.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/filter_arg_expression_analysis_result_set.py` & `gemmapy-1.0.3/gemmapy/sdk/models/filter_arg_expression_analysis_result_set.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/filter_arg_expression_experiment.py` & `gemmapy-1.0.3/gemmapy/sdk/models/filter_arg_expression_experiment.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_inferred_and_paginated_response_data_object_expression_experiment_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/filtered_and_inferred_and_paginated_response_data_object_expression_experiment_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_array_design_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/filtered_and_paginated_response_data_object_array_design_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_composite_sequence_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/filtered_and_paginated_response_data_object_composite_sequence_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_differential_expression_analysis_result_set_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/filtered_and_paginated_response_data_object_differential_expression_analysis_result_set_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_expression_experiment_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/filtered_and_paginated_response_data_object_expression_experiment_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/filtered_and_paginated_response_data_object_gene_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/filtered_and_paginated_response_data_object_gene_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/geeq_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/geeq_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/gene.py` & `gemmapy-1.0.3/gemmapy/sdk/models/gene.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/gene1.py` & `gemmapy-1.0.3/gemmapy/sdk/models/gene1.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/gene2.py` & `gemmapy-1.0.3/gemmapy/sdk/models/gene2.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/gene3.py` & `gemmapy-1.0.3/gemmapy/sdk/models/gene3.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/gene4.py` & `gemmapy-1.0.3/gemmapy/sdk/models/gene4.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/gene5.py` & `gemmapy-1.0.3/gemmapy/sdk/models/gene5.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/gene_arg.py` & `gemmapy-1.0.3/gemmapy/sdk/models/gene_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/gene_element_expressions_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/gene_element_expressions_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/gene_ontology_term_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/gene_ontology_term_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/gene_set_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/gene_set_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/gene_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/gene_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/measurement_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/measurement_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/one_of_search_result_value_object_object_result_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/one_of_search_result_value_object_object_result_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/ontology_term_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/ontology_term_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/paginated_response_data_object_composite_sequence_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/paginated_response_data_object_composite_sequence_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/paginated_response_data_object_expression_experiment_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/paginated_response_data_object_expression_experiment_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/paginated_response_data_object_gene_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/paginated_response_data_object_gene_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/paginated_results_response_data_object_differential_expression_analysis_result_set_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/paginated_results_response_data_object_differential_expression_analysis_result_set_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/physical_location_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/physical_location_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/platform.py` & `gemmapy-1.0.3/gemmapy/sdk/models/platform.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/platform1.py` & `gemmapy-1.0.3/gemmapy/sdk/models/platform1.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/platform2.py` & `gemmapy-1.0.3/gemmapy/sdk/models/platform2.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/platform3.py` & `gemmapy-1.0.3/gemmapy/sdk/models/platform3.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/platform4.py` & `gemmapy-1.0.3/gemmapy/sdk/models/platform4.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/platform5.py` & `gemmapy-1.0.3/gemmapy/sdk/models/platform5.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/platform_arg.py` & `gemmapy-1.0.3/gemmapy/sdk/models/platform_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/probe.py` & `gemmapy-1.0.3/gemmapy/sdk/models/probe.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/quantitation_type.py` & `gemmapy-1.0.3/gemmapy/sdk/models/quantitation_type.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/quantitation_type_arg.py` & `gemmapy-1.0.3/gemmapy/sdk/models/quantitation_type_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/quantitation_type_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/quantitation_type_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_annotation_with_usage_statistics_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_annotation_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_array_design_with_usage_statistics_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_array_design_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_category_with_usage_statistics_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_limited_response_data_object_category_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_paginated_response_data_object_expression_experiment_with_search_result_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/queried_and_filtered_and_inferred_and_paginated_response_data_object_expression_experiment_with_search_result_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_inferred_response_data_object_taxon_with_usage_statistics_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/queried_and_filtered_and_inferred_response_data_object_taxon_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/queried_and_filtered_and_paginated_response_data_object_expression_experiment_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/queried_and_filtered_and_paginated_response_data_object_expression_experiment_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/query_arg.py` & `gemmapy-1.0.3/gemmapy/sdk/models/query_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_api_info_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_api_info_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_annotation_search_result_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_annotation_search_result_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_array_design_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_array_design_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_bio_assay_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_bio_assay_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_differential_expression_analysis_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_differential_expression_analysis_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_experiment_expression_levels_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_experiment_expression_levels_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_gene_ontology_term_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_gene_ontology_term_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_gene_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_gene_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_physical_location_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_physical_location_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_list_taxon_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_list_taxon_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_long.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_long.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_set_annotation_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_set_annotation_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_set_quantitation_type_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_set_quantitation_type_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_data_object_simple_svd_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_data_object_simple_svd_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/response_error_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/response_error_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/search_result_type.py` & `gemmapy-1.0.3/gemmapy/sdk/models/search_result_type.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/search_result_value_object_expression_experiment_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/search_result_value_object_expression_experiment_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/search_result_value_object_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/search_result_value_object_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/search_results_response_data_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/search_results_response_data_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/search_settings_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/search_settings_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/simple_svd_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/simple_svd_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/sort_arg_array_design.py` & `gemmapy-1.0.3/gemmapy/sdk/models/sort_arg_array_design.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/sort_arg_expression_analysis_result_set.py` & `gemmapy-1.0.3/gemmapy/sdk/models/sort_arg_expression_analysis_result_set.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/sort_arg_expression_experiment.py` & `gemmapy-1.0.3/gemmapy/sdk/models/sort_arg_expression_experiment.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/sort_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/sort_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/statement_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/statement_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxa.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxa.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon1.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon1.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon2.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon2.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon3.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon3.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon4.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon4.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon5.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon5.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon6.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon6.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon7.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon7.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon8.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon8.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon9.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon9.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon_arg.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon_arg.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/taxon_with_usage_statistics_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/taxon_with_usage_statistics_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/vector_element_value_object.py` & `gemmapy-1.0.3/gemmapy/sdk/models/vector_element_value_object.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/models/well_composed_error_body.py` & `gemmapy-1.0.3/gemmapy/sdk/models/well_composed_error_body.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy/sdk/rest.py` & `gemmapy-1.0.3/gemmapy/sdk/rest.py`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/gemmapy.egg-info/PKG-INFO` & `gemmapy-1.0.3/gemmapy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemmapy
-Version: 1.0.2
+Version: 1.0.3
 Summary: a Python Wrapper for the Gemma API
 Keywords: gemma,bioinformatics
 Requires-Python: >3.10
 License-File: LICENSE.md
 Requires-Dist: certifi>=14.05.14
 Requires-Dist: six>=1.10
 Requires-Dist: python_dateutil>=2.5.3
```

### Comparing `gemmapy-1.0.2/gemmapy.egg-info/SOURCES.txt` & `gemmapy-1.0.3/gemmapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemmapy-1.0.2/tests/test_basic.py` & `gemmapy-1.0.3/tests/test_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     assert res[4].shape[0]>1
      
 def test_get_processed_expression_samples_compatibility():
     exp = api.get_dataset_processed_expression(2)
     samples = api.get_dataset_samples(2)
     
     exp_cols = [x for x in exp.columns if x in list(samples.sample_name)]    
-    
+
     assert all([exp_cols[i] == samples.sample_name[i] for i in range(len(exp_cols))])
 
 
 def test_get_dataset_qt_types_raw_expression():
     qtypes = api.get_dataset_quantitation_types(2)
     qtype_id = list(qtypes[qtypes.type=='raw'].ID)[0]
```

