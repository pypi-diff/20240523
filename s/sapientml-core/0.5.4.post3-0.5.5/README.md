# Comparing `tmp/sapientml_core-0.5.4.post3.tar.gz` & `tmp/sapientml_core-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapientml_core-0.5.4.post3.tar", max compression
+gzip compressed data, was "sapientml_core-0.5.5.tar", max compression
```

## Comparing `sapientml_core-0.5.4.post3.tar` & `sapientml_core-0.5.5.tar`

### file list

```diff
@@ -1,108 +1,110 @@
--rw-r--r--   0        0        0    11356 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/LICENSE
--rw-r--r--   0        0        0     1653 2024-01-19 02:01:57.359460 sapientml_core-0.5.4.post3/pyproject.toml
--rw-r--r--   0        0        0      717 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/__init__.py
--rw-r--r--   0        0        0      585 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/adaptation/__init__.py
--rw-r--r--   0        0        0     2513 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/adaptation/artifacts/label_order.json
--rw-r--r--   0        0        0      585 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/adaptation/generation/__init__.py
--rw-r--r--   0        0        0    30849 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/adaptation/generation/pipeline_template.py
--rw-r--r--   0        0        0     2626 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/adaptation/generation/predicate.py
--rw-r--r--   0        0        0     4438 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/adaptation/generation/preprocessing_label.py
--rw-r--r--   0        0        0    17361 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/adaptation/generation/template_based_adaptation.py
--rw-r--r--   0        0        0        0 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/design/__init__.py
--rw-r--r--   0        0        0     2993 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/design/label_util.py
--rw-r--r--   0        0        0     2762 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/design/pp_component_groups.py
--rw-r--r--   0        0        0     2177 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/design/search_space.py
--rw-r--r--   0        0        0      899 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/enums.py
--rw-r--r--   0        0        0    17237 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/explain/AutoEDA.py
--rw-r--r--   0        0        0    17606 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/explain/AutoVisualization.py
--rw-r--r--   0        0        0    40509 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/explain/code_miner.py
--rw-r--r--   0        0        0     1268 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/explain/code_template.py
--rw-r--r--   0        0        0     3779 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/explain/main.py
--rw-r--r--   0        0        0    20803 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/explain/pipeline_explanation.py
--rw-r--r--   0        0        0      493 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/explain/templates/jupyter_content.json
--rw-r--r--   0        0        0    16791 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/generator.py
--rw-r--r--   0        0        0     1242 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/internal_path.py
--rw-r--r--   0        0        0    40076 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/meta_features.py
--rw-r--r--   0        0        0    23893 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/models/feature_importance.json
--rw-r--r--   0        0        0    59630 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/models/model_metafeatures_test.csv
--rw-r--r--   0        0        0     5658 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/models/mp_model_1.pkl
--rw-r--r--   0        0        0   223570 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/models/mp_model_2.pkl
--rw-r--r--   0        0        0    12634 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/models/pp_models.pkl
--rw-r--r--   0        0        0    17670 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/params.py
--rw-r--r--   0        0        0     1923 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/ps_macros.py
--rw-r--r--   0        0        0      585 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/seeding/__init__.py
--rw-r--r--   0        0        0     9551 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/seeding/predictor.py
--rw-r--r--   0        0        0     7667 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/templates/explainability_templates/component_description.json
--rw-r--r--   0        0        0      172 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/templates/explainability_templates/model_explanation.py.jinja
--rw-r--r--   0        0        0      683 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/templates/explainability_templates/preprocessing_explanation.py.jinja
--rw-r--r--   0        0        0      281 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/classification_post_process.jinja
--rw-r--r--   0        0        0     4986 2024-01-19 02:01:43.091522 sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/hyperparameter_tuning.py.jinja
--rw-r--r--   0        0        0    12287 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/hyperparameters.py.jinja
--rw-r--r--   0        0        0     3934 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/hyperparameters_default_value.py.jinja
--rw-r--r--   0        0        0     2028 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/model.py.jinja
--rw-r--r--   0        0        0      811 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/model_predict.py.jinja
--rw-r--r--   0        0        0     1686 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/model_test.py.jinja
--rw-r--r--   0        0        0     1433 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/model_train.py.jinja
--rw-r--r--   0        0        0      352 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/confusion_matrix.py.jinja
--rw-r--r--   0        0        0      285 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/drop_columns.py.jinja
--rw-r--r--   0        0        0     4795 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/evaluation.py.jinja
--rw-r--r--   0        0        0     3929 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/hyperparameter_tuning_evaluation.py.jinja
--rw-r--r--   0        0        0      662 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/inverse_target.py.jinja
--rw-r--r--   0        0        0     1169 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/permutation_importance.py.jinja
--rw-r--r--   0        0        0     2373 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/prediction_result.py.jinja
--rw-r--r--   0        0        0      728 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/shap.py.jinja
--rw-r--r--   0        0        0      285 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/target_separation_predict.py.jinja
--rw-r--r--   0        0        0      396 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/target_separation_test.py.jinja
--rw-r--r--   0        0        0      178 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/target_separation_train.py.jinja
--rw-r--r--   0        0        0      287 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/target_separation_validation.py.jinja
--rw-r--r--   0        0        0     1682 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/pipeline_predict.py.jinja
--rw-r--r--   0        0        0     2356 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/pipeline_test.py.jinja
--rw-r--r--   0        0        0     1426 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/pipeline_train.py.jinja
--rw-r--r--   0        0        0     1561 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/pipeline_validation.py.jinja
--rw-r--r--   0        0        0      953 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/DATE.py.jinja
--rw-r--r--   0        0        0      495 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/DATE_predict.jinja
--rw-r--r--   0        0        0      507 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/DATE_train.jinja
--rw-r--r--   0        0        0      381 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/LabelEncoder.py.jinja
--rw-r--r--   0        0        0      217 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/LabelEncoder_predict.py.jinja
--rw-r--r--   0        0        0      360 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/LabelEncoder_train.py.jinja
--rw-r--r--   0        0        0      633 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/Processing.py.jinja
--rw-r--r--   0        0        0      577 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/Processing_predict.py.jinja
--rw-r--r--   0        0        0      579 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/Processing_train.py.jinja
--rw-r--r--   0        0        0      460 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/SMOTE.py.jinja
--rw-r--r--   0        0        0      562 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/STANDARD.py.jinja
--rw-r--r--   0        0        0      384 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/STANDARD_predict.py.jinja
--rw-r--r--   0        0        0      491 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/STANDARD_train.py.jinja
--rw-r--r--   0        0        0     3280 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/TfidfVectorizer.py.jinja
--rw-r--r--   0        0        0      763 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_predict.py.jinja
--rw-r--r--   0        0        0     2561 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_train.py.jinja
--rw-r--r--   0        0        0      814 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/fillna-type-numeric.py.jinja
--rw-r--r--   0        0        0      520 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_predict.py.jinja
--rw-r--r--   0        0        0      659 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_train.py.jinja
--rw-r--r--   0        0        0     1031 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/fillna-type-string.py.jinja
--rw-r--r--   0        0        0      620 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/fillna-type-string_predict.py.jinja
--rw-r--r--   0        0        0      770 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/fillna-type-string_train.py.jinja
--rw-r--r--   0        0        0      794 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/get_dummies.py.jinja
--rw-r--r--   0        0        0      425 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/get_dummies_predict.py.jinja
--rw-r--r--   0        0        0      561 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/get_dummies_train.py.jinja
--rw-r--r--   0        0        0      365 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/log.py.jinja
--rw-r--r--   0        0        0      266 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/log_predict.py.jinja
--rw-r--r--   0        0        0      156 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/log_train.py.jinja
--rw-r--r--   0        0        0     4623 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/augmentation/mutation_results.py
--rw-r--r--   0        0        0     8573 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/augmentation/mutation_runner.py
--rw-r--r--   0        0        0    32944 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/augmentation/mutator.py
--rw-r--r--   0        0        0     5241 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/dataflowmodel/ast_operation.py
--rw-r--r--   0        0        0    12596 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/dataflowmodel/dependent_api_extractor.py
--rw-r--r--   0        0        0     2762 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/dataflowmodel/determine_label_order.py
--rw-r--r--   0        0        0     7850 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/denoising/ast_info_collector.py
--rw-r--r--   0        0        0     8533 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/denoising/dataset_snapshot_extractor.py
--rw-r--r--   0        0        0     7987 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/denoising/determine_used_features.py
--rw-r--r--   0        0        0     1474 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/denoising/df_collector.py
--rw-r--r--   0        0        0     4791 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/denoising/static_analysis_of_columns.py
--rw-r--r--   0        0        0     7965 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/meta_feature_extractor.py
--rw-r--r--   0        0        0     6219 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/meta_feature_selector.py
--rw-r--r--   0        0        0    10682 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/meta_model_trainer.py
--rw-r--r--   0        0        0     5210 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/pp_model_trainer.py
--rw-r--r--   0        0        0      923 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/project.py
--rw-r--r--   0        0        0     4533 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/training/project_corpus.py
--rw-r--r--   0        0        0     5313 2024-01-19 02:01:43.095522 sapientml_core-0.5.4.post3/sapientml_core/util/file_util.py
--rw-r--r--   0        0        0     1356 1970-01-01 00:00:00.000000 sapientml_core-0.5.4.post3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/LICENSE
+-rw-r--r--   0        0        0     1669 2024-05-23 05:03:54.793486 sapientml_core-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      717 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/__init__.py
+-rw-r--r--   0        0        0      585 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/__init__.py
+-rw-r--r--   0        0        0     2513 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/artifacts/label_order.json
+-rw-r--r--   0        0        0      585 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/generation/__init__.py
+-rw-r--r--   0        0        0    31184 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/generation/pipeline_template.py
+-rw-r--r--   0        0        0     2626 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/generation/predicate.py
+-rw-r--r--   0        0        0     4438 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/generation/preprocessing_label.py
+-rw-r--r--   0        0        0    17616 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/adaptation/generation/template_based_adaptation.py
+-rw-r--r--   0        0        0        0 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/design/__init__.py
+-rw-r--r--   0        0        0     2993 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/design/label_util.py
+-rw-r--r--   0        0        0     2762 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/design/pp_component_groups.py
+-rw-r--r--   0        0        0     2177 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/design/search_space.py
+-rw-r--r--   0        0        0      899 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/enums.py
+-rw-r--r--   0        0        0    17237 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/explain/AutoEDA.py
+-rw-r--r--   0        0        0    17606 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/explain/AutoVisualization.py
+-rw-r--r--   0        0        0    40509 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/explain/code_miner.py
+-rw-r--r--   0        0        0     1268 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/explain/code_template.py
+-rw-r--r--   0        0        0     3779 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/explain/main.py
+-rw-r--r--   0        0        0    20803 2024-05-23 05:03:41.533297 sapientml_core-0.5.5/sapientml_core/explain/pipeline_explanation.py
+-rw-r--r--   0        0        0      493 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/explain/templates/jupyter_content.json
+-rw-r--r--   0        0        0    16874 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/generator.py
+-rw-r--r--   0        0        0     1242 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/internal_path.py
+-rw-r--r--   0        0        0    40076 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/meta_features.py
+-rw-r--r--   0        0        0    23893 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/models/feature_importance.json
+-rw-r--r--   0        0        0    59630 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/models/model_metafeatures_test.csv
+-rw-r--r--   0        0        0     5658 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/models/mp_model_1.pkl
+-rw-r--r--   0        0        0   223570 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/models/mp_model_2.pkl
+-rw-r--r--   0        0        0    12634 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/models/pp_models.pkl
+-rw-r--r--   0        0        0    17835 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/params.py
+-rw-r--r--   0        0        0     1923 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/ps_macros.py
+-rw-r--r--   0        0        0      585 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/seeding/__init__.py
+-rw-r--r--   0        0        0     9591 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/seeding/predictor.py
+-rw-r--r--   0        0        0     7667 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/explainability_templates/component_description.json
+-rw-r--r--   0        0        0      172 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/explainability_templates/model_explanation.py.jinja
+-rw-r--r--   0        0        0      683 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/explainability_templates/preprocessing_explanation.py.jinja
+-rw-r--r--   0        0        0      281 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/classification_post_process.jinja
+-rw-r--r--   0        0        0     4986 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/hyperparameter_tuning.py.jinja
+-rw-r--r--   0        0        0    12287 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/hyperparameters.py.jinja
+-rw-r--r--   0        0        0     3934 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/hyperparameters_default_value.py.jinja
+-rw-r--r--   0        0        0     2551 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/model.py.jinja
+-rw-r--r--   0        0        0     1086 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/model_predict.py.jinja
+-rw-r--r--   0        0        0     2540 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/model_test.py.jinja
+-rw-r--r--   0        0        0     1797 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/model_templates/model_train.py.jinja
+-rw-r--r--   0        0        0      563 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/confusion_matrix.py.jinja
+-rw-r--r--   0        0        0      285 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/drop_columns.py.jinja
+-rw-r--r--   0        0        0     5098 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/evaluation.py.jinja
+-rw-r--r--   0        0        0     4718 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/evaluation_test.py.jinja
+-rw-r--r--   0        0        0     3848 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/hyperparameter_tuning_evaluation.py.jinja
+-rw-r--r--   0        0        0      662 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/inverse_target.py.jinja
+-rw-r--r--   0        0        0     1082 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/permutation_importance.py.jinja
+-rw-r--r--   0        0        0     2641 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/prediction_result.py.jinja
+-rw-r--r--   0        0        0      398 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/preprocess_dataset.py.jinja
+-rw-r--r--   0        0        0      728 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/shap.py.jinja
+-rw-r--r--   0        0        0      285 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/target_separation_predict.py.jinja
+-rw-r--r--   0        0        0      396 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/target_separation_test.py.jinja
+-rw-r--r--   0        0        0      178 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/target_separation_train.py.jinja
+-rw-r--r--   0        0        0      287 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/other_templates/target_separation_validation.py.jinja
+-rw-r--r--   0        0        0     1685 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/pipeline_predict.py.jinja
+-rw-r--r--   0        0        0     2472 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/pipeline_test.py.jinja
+-rw-r--r--   0        0        0     1426 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/pipeline_train.py.jinja
+-rw-r--r--   0        0        0     1676 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/pipeline_validation.py.jinja
+-rw-r--r--   0        0        0      953 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/DATE.py.jinja
+-rw-r--r--   0        0        0      495 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/DATE_predict.jinja
+-rw-r--r--   0        0        0      507 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/DATE_train.jinja
+-rw-r--r--   0        0        0      381 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/LabelEncoder.py.jinja
+-rw-r--r--   0        0        0      217 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/LabelEncoder_predict.py.jinja
+-rw-r--r--   0        0        0      360 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/LabelEncoder_train.py.jinja
+-rw-r--r--   0        0        0      633 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/Processing.py.jinja
+-rw-r--r--   0        0        0      577 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/Processing_predict.py.jinja
+-rw-r--r--   0        0        0      579 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/Processing_train.py.jinja
+-rw-r--r--   0        0        0      460 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/SMOTE.py.jinja
+-rw-r--r--   0        0        0      562 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/STANDARD.py.jinja
+-rw-r--r--   0        0        0      384 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/STANDARD_predict.py.jinja
+-rw-r--r--   0        0        0      491 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/STANDARD_train.py.jinja
+-rw-r--r--   0        0        0     3280 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/TfidfVectorizer.py.jinja
+-rw-r--r--   0        0        0      763 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_predict.py.jinja
+-rw-r--r--   0        0        0     2561 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_train.py.jinja
+-rw-r--r--   0        0        0      814 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-numeric.py.jinja
+-rw-r--r--   0        0        0      520 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_predict.py.jinja
+-rw-r--r--   0        0        0      659 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_train.py.jinja
+-rw-r--r--   0        0        0     1031 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-string.py.jinja
+-rw-r--r--   0        0        0      620 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-string_predict.py.jinja
+-rw-r--r--   0        0        0      770 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-string_train.py.jinja
+-rw-r--r--   0        0        0      794 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/get_dummies.py.jinja
+-rw-r--r--   0        0        0      425 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/get_dummies_predict.py.jinja
+-rw-r--r--   0        0        0      561 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/get_dummies_train.py.jinja
+-rw-r--r--   0        0        0      365 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/log.py.jinja
+-rw-r--r--   0        0        0      266 2024-05-23 05:03:41.537297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/log_predict.py.jinja
+-rw-r--r--   0        0        0      156 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/log_train.py.jinja
+-rw-r--r--   0        0        0     4623 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/augmentation/mutation_results.py
+-rw-r--r--   0        0        0     8573 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/augmentation/mutation_runner.py
+-rw-r--r--   0        0        0    32944 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/augmentation/mutator.py
+-rw-r--r--   0        0        0     5241 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/dataflowmodel/ast_operation.py
+-rw-r--r--   0        0        0    12596 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/dataflowmodel/dependent_api_extractor.py
+-rw-r--r--   0        0        0     2762 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/dataflowmodel/determine_label_order.py
+-rw-r--r--   0        0        0     7850 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/denoising/ast_info_collector.py
+-rw-r--r--   0        0        0     8533 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/denoising/dataset_snapshot_extractor.py
+-rw-r--r--   0        0        0     7987 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/denoising/determine_used_features.py
+-rw-r--r--   0        0        0     1474 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/denoising/df_collector.py
+-rw-r--r--   0        0        0     4791 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/denoising/static_analysis_of_columns.py
+-rw-r--r--   0        0        0     7965 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/meta_feature_extractor.py
+-rw-r--r--   0        0        0     6219 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/meta_feature_selector.py
+-rw-r--r--   0        0        0    10682 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/meta_model_trainer.py
+-rw-r--r--   0        0        0     5210 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/pp_model_trainer.py
+-rw-r--r--   0        0        0      923 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/project.py
+-rw-r--r--   0        0        0     4533 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/training/project_corpus.py
+-rw-r--r--   0        0        0     5313 2024-05-23 05:03:41.541297 sapientml_core-0.5.5/sapientml_core/util/file_util.py
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 sapientml_core-0.5.5/PKG-INFO
```

### Comparing `sapientml_core-0.5.4.post3/LICENSE` & `sapientml_core-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/pyproject.toml` & `sapientml_core-0.5.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,73 +3,73 @@
 description = "A SapientML plugin of SapientMLGenerator"
 license = "Apache-2.0"
 maintainers = [
   "Kosaku Kimura <kimura.kosaku@fujitsu.com>",
   "Akira Ura <ura.akira@fujitsu.com>",
 ]
 name = "sapientml-core"
-version = "0.5.4.post3"
+version = "0.5.5"
 
 [tool.poetry.dependencies]
-catboost = "^1.2"
-imbalanced-learn = "^0.11.0"
+catboost = ">=1.2.3"
+imbalanced-learn = ">=0.11,<0.13"
 ipykernel = "^6.25.1"
 japanize-matplotlib = "^1.1.3"
 jinja2 = "^3.1.2"
 libcst = "^1.0.1"
 lightgbm = "^4.0.0"
 nbconvert = "^7.7.4"
 nbformat = "^5.9.2"
 nltk = "^3.8.1"
-numba = ">=0.57.1,<0.59.0"
+numba = ">=0.57.1,<0.60.0"
 optuna = "^3.2.0"
 python = ">=3.10,<3.13"
 sapientml = "*"
 sapientml-loaddata = "*"
 sapientml-preprocess = "*"
 scikit-learn = "1.3.2"
 scipy = "^1.11.1"
 seaborn = ">=0.12.2,<0.14.0"
 shap = ">=0.43,<0.45"
 tqdm = "^4.66.1"
 xgboost = ">=1.7.6,<3.0.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.7.0"
-flake8 = "^6.1.0"
+black = ">=23.7,<25.0"
+flake8 = ">=6.1,<8.0"
 isort = "^5.12.0"
 pre-commit = "^3.3.3"
-pysen = "^0.10.5"
-pytest = "^7.4.0"
-pytest-cov = "^4.1.0"
+pysen = ">=0.10.5,<0.12.0"
+pytest = ">=7.4,<9.0"
+pytest-cov = ">=4.1,<6.0"
 pytest-xdist = "^3.3.1"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.poetry.plugins."sapientml.pipeline_generator"]
 sapientml = "sapientml_core:SapientMLGenerator"
 
 [tool.poetry.plugins."sapientml.config"]
 sapientml = "sapientml_core:SapientMLConfig"
 
 [tool.pysen]
-version = "0.5.4.post3"
+version = "0.5.5"
 
 [tool.pysen-cli]
 settings_dir = ".pysen"
 
 [tool.pysen.lint]
 enable_black = true
 enable_flake8 = true
 enable_isort = true
 enable_mypy = false
 line_length = 120
-py_version = "0.5.4.post3"
+py_version = "0.5.5"
 
 [tool.pysen.lint.source]
 includes = ["sapientml_core/", "tests/"]
 
 [tool.pytest.ini_options]
 addopts = "-s -x --cov=sapientml_core"
 testpaths = ["tests"]
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/__init__.py` & `sapientml_core-0.5.5/sapientml_core/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/adaptation/__init__.py` & `sapientml_core-0.5.5/sapientml_core/adaptation/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/adaptation/artifacts/label_order.json` & `sapientml_core-0.5.5/sapientml_core/adaptation/artifacts/label_order.json`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/adaptation/generation/__init__.py` & `sapientml_core-0.5.5/sapientml_core/adaptation/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/adaptation/generation/pipeline_template.py` & `sapientml_core-0.5.5/sapientml_core/adaptation/generation/pipeline_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,21 +133,14 @@
     def generate(self):
         """generate pipeline."""
 
         pipeline = self.pipeline
         if pipeline.model is None:
             return
         model_name = pipeline.model.label_name.split(":")[2]
-        is_boolean_target = any(
-            [pipeline.dataset_summary.columns[col].dtype == "bool" for col in pipeline.task.target_columns]
-        )
-        if model_name == "CatBoostClassifier" and is_boolean_target:
-            target2string = True
-        else:
-            target2string = False
 
         # Use tpl.render but self._render because keep blank lines.
         if len(pipeline.dataset_summary.cols_str_other) > 0:
             irrelevant_columns = pipeline.dataset_summary.cols_str_other
             tpl = env.get_template("other_templates/drop_columns.py.jinja")
             pipeline.pipeline_json["discard_columns"]["code"] = self._render(
                 tpl, train=True, test=True, irrelevant_columns=irrelevant_columns
@@ -163,33 +156,52 @@
         pipeline.pipeline_json["target_separation"]["code_validation"] = self._render(tpl, pipeline=pipeline)
         tpl = env.get_template("other_templates/target_separation_test.py.jinja")
         pipeline.pipeline_json["target_separation"]["code_test"] = self._render(tpl, pipeline=pipeline)
         tpl = env.get_template("other_templates/target_separation_train.py.jinja")
         pipeline.pipeline_json["target_separation"]["code_train"] = self._render(tpl, pipeline=pipeline)
         tpl = env.get_template("other_templates/target_separation_predict.py.jinja")
         pipeline.pipeline_json["target_separation"]["code_predict"] = self._render(tpl, pipeline=pipeline)
+        if pipeline.config.export_preprocess_dataset:
+            tpl = env.get_template("other_templates/preprocess_dataset.py.jinja")
+            pipeline.pipeline_json["preprocess_dataset"]["code_test"] = self._render(tpl, pipeline=pipeline)
 
         flag_hyperparameter_tuning = (
             pipeline.config.hyperparameter_tuning and model_name not in NO_TUNABLE_PARAMS_MODELS
         )
         if pipeline.inverse_target:
             tpl = env.get_template("other_templates/inverse_target.py.jinja")
             pipeline.pipeline_json["inverse_target"]["code"] = self._render(tpl, pipeline=pipeline)
             pipeline.pipeline_json["inverse_target_hpo"]["code"] = self._render(
                 tpl, pipeline=pipeline, flag_hyperparameter_tuning=flag_hyperparameter_tuning
             )
 
+        _is_multioutput_classification = (
+            pipeline.task.task_type == macros.TASK_CLASSIFICATION and len(pipeline.task.target_columns) > 1
+        )
+
         tpl = env.get_template("other_templates/evaluation.py.jinja")
-        code = self._render(tpl, pipeline=pipeline, target2string=target2string, macros=macros)
+        code = self._render(
+            tpl, pipeline=pipeline, macros=macros, is_multioutput_classification=_is_multioutput_classification
+        )
         pipeline.pipeline_json["evaluation"]["code_validation"] = code
+        pipeline.pipeline_json["evaluation"]["code_predict"] = code
+        tpl = env.get_template("other_templates/evaluation_test.py.jinja")
+        code = self._render(
+            tpl,
+            pipeline=pipeline,
+            macros=macros,
+            is_multioutput_classification=_is_multioutput_classification,
+        )
         pipeline.pipeline_json["evaluation"]["code_test"] = code
 
         # Adding confusion_matrix
         tpl = env.get_template("other_templates/confusion_matrix.py.jinja")
-        pipeline.pipeline_json["confusion_matrix"]["code"] = self._render(tpl, pipeline=pipeline)
+        pipeline.pipeline_json["confusion_matrix"]["code"] = self._render(
+            tpl, pipeline=pipeline, is_multioutput_classification=_is_multioutput_classification
+        )
 
         # Adding Shap Visualization data
         tpl = env.get_template("other_templates/shap.py.jinja")
         pipeline.pipeline_json["shap"]["code"] = self._render(tpl, pipeline=pipeline, model_name=model_name)
 
         tpl = env.get_template("other_templates/prediction_result.py.jinja")
         pipeline.pipeline_json["output_prediction"]["code"] = self._render(
@@ -201,15 +213,15 @@
             pipeline.pipeline_json["hyperparameters"]["code"] = self._render(tpl, model_name=model_name)
 
             tpl = env.get_template("model_templates/hyperparameters_default_value.py.jinja")
             pipeline.pipeline_json["hyperparameters_default_value"]["code"] = self._render(tpl, model_name=model_name)
 
             tpl = env.get_template("other_templates/hyperparameter_tuning_evaluation.py.jinja")
             pipeline.pipeline_json["hyperparameter_tuning_evaluation"]["code"] = self._render(
-                tpl, pipeline=pipeline, target2string=target2string, macros=macros
+                tpl, pipeline=pipeline, macros=macros
             )
 
             self.populate_hyperparameter_tuning()
         elif pipeline.config.hyperparameter_tuning and model_name in NO_TUNABLE_PARAMS_MODELS:
             logger.debug(
                 "'hyperparameter_tuning' is set to True, but the candidate model("
                 + model_name
@@ -218,23 +230,21 @@
 
         self.populate_model()
 
         if pipeline.adaptation_metric and (
             pipeline.adaptation_metric in macros.metric_needing_predict_proba
             or pipeline.adaptation_metric.startswith(macros.Metric.MAP_K.value)
         ):
-            pipeline.pipeline_json["evaluation"]["code_test"] = pipeline.pipeline_json["evaluation"][
-                "code_test"
+            pipeline.pipeline_json["evaluation"]["code_predict"] = pipeline.pipeline_json["evaluation"][
+                "code_predict"
             ].replace("y_pred", "y_prob")
 
         if pipeline.config.permutation_importance:
             tpl = env.get_template("other_templates/permutation_importance.py.jinja")
-            pipeline.pipeline_json["permutation_importance"]["code"] = self._render(
-                tpl, pipeline=pipeline, target2string=target2string
-            )
+            pipeline.pipeline_json["permutation_importance"]["code"] = self._render(tpl, pipeline=pipeline)
 
         tpl_validation = env.get_template("pipeline_validation.py.jinja")
         pipeline.validation = tpl_validation.render(
             pipeline_json=pipeline.pipeline_json,
             pipeline=pipeline,
             flag_hyperparameter_tuning=flag_hyperparameter_tuning,
         )
@@ -427,17 +437,19 @@
             evaluation=pipeline.pipeline_json["hyperparameter_tuning_evaluation"]["code"],
             enqueue_default_hyperparameters=pipeline.pipeline_json["hyperparameters_default_value"]["code"],
             binary_classification_snippet=binary_classification_snippet,
             flag_no_random_seed_model=flag_no_random_seed_model,
             is_multioutput_regression=_is_multioutput_regression,
             is_multioutput_classification=_is_multioutput_classification,
             flag_predict_proba=flag_predict_proba,
-            timeout=pipeline.config.hyperparameter_tuning_timeout
-            if pipeline.config.hyperparameter_tuning_timeout > 0
-            else None,
+            timeout=(
+                pipeline.config.hyperparameter_tuning_timeout
+                if pipeline.config.hyperparameter_tuning_timeout > 0
+                else None
+            ),
         )
         pipeline.pipeline_json["hyperparameter_optimization"]["code"] = snippet
 
     def populate_model(self):
         """populate_model.
 
         Returns
@@ -538,17 +550,14 @@
             snippet = snippet.replace("predict", "predict_proba")
             tpl = env.get_template("model_templates/classification_post_process.jinja")
             snippet += "\n" + self._render(tpl, pipeline=pipeline)
 
             tpl_predict = env.get_template("model_templates/classification_post_process.jinja")
             snippet_predict += "\n" + self._render(tpl_predict, pipeline=pipeline).replace("y_pred", "y_prob")
 
-            tpl_test = env.get_template("model_templates/classification_post_process.jinja")
-            snippet_test += "\n" + self._render(tpl_test, pipeline=pipeline).replace("y_pred", "y_prob")
-
         model_component_json["code"] = snippet
         model_component_json["code_train"] = snippet_train
         model_component_json["code_predict"] = snippet_predict
         model_component_json["code_test"] = snippet_test
 
         with open(Path(os.path.dirname(__file__)) / "../../models/feature_importance.json", "r", encoding="utf-8") as f:
             model_feature_weights = json.load(f)
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/adaptation/generation/predicate.py` & `sapientml_core-0.5.5/sapientml_core/adaptation/generation/predicate.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/adaptation/generation/preprocessing_label.py` & `sapientml_core-0.5.5/sapientml_core/adaptation/generation/preprocessing_label.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/adaptation/generation/template_based_adaptation.py` & `sapientml_core-0.5.5/sapientml_core/adaptation/generation/template_based_adaptation.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,23 +118,27 @@
         preprocessing_labels = dict(
             filter(
                 lambda elem: elem[1]["probability"] > preprocessing_threshold,
                 all_preprocessing_labels.items(),
             )
         )
 
+        # resolve conflicting preprocessing labels by keeping the one with highest probability
+        conflicting_labels = dict()
+        preprocessing_labels, conflicting_labels = self._resolve_conflicting_labels(preprocessing_labels)
+
+        # remove GausianNB and SVC if TfidfVectorizer is contain
+        if "PREPROCESS:Text:TfidfVectorizer:sklearn" in preprocessing_labels:
+            model_labels = {k: v for k, v in model_labels.items() if "GaussianNB" not in k and "SVC" not in k}
+
         n_models = self.config.n_models
         if n_models < 1:
             raise ValueError("Please set 'n_models' to a number greater than or equal to 1.")
         model_labels = dict(list(model_labels.items())[0:n_models])
 
-        # resolve conflicting preprocessing labels by keeping the one with highest probability
-        conflicting_labels = dict()
-        preprocessing_labels, conflicting_labels = self._resolve_conflicting_labels(preprocessing_labels)
-
         # order preprocessing labels and model labels
         preprocessing_labels, model_labels = self._order_labels(preprocessing_labels, model_labels)
 
         # convert to preprocessing and model objects
         preprocessing_label_objects: list[PreprocessingLabel] = list()
         model_label_objects: list[ModelLabel] = list()
         for name, details in preprocessing_labels.items():
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/design/label_util.py` & `sapientml_core-0.5.5/sapientml_core/design/label_util.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/design/pp_component_groups.py` & `sapientml_core-0.5.5/sapientml_core/design/pp_component_groups.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/design/search_space.py` & `sapientml_core-0.5.5/sapientml_core/design/search_space.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/enums.py` & `sapientml_core-0.5.5/sapientml_core/enums.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/explain/AutoEDA.py` & `sapientml_core-0.5.5/sapientml_core/explain/AutoEDA.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/explain/AutoVisualization.py` & `sapientml_core-0.5.5/sapientml_core/explain/AutoVisualization.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/explain/code_miner.py` & `sapientml_core-0.5.5/sapientml_core/explain/code_miner.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/explain/code_template.py` & `sapientml_core-0.5.5/sapientml_core/explain/code_template.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/explain/main.py` & `sapientml_core-0.5.5/sapientml_core/explain/main.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/explain/pipeline_explanation.py` & `sapientml_core-0.5.5/sapientml_core/explain/pipeline_explanation.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/generator.py` & `sapientml_core-0.5.5/sapientml_core/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,16 +395,17 @@
 
             # copy libs
             lib_path = self.output_dir / "lib"
             lib_path.mkdir(exist_ok=True)
 
             eps = entry_points(group="sapientml.export_modules")
             for ep in eps:
-                for file in glob(f"{ep.load().__path__[0]}/*.py"):
-                    copyfile(file, lib_path / Path(file).name)
+                if ep.name in [self.__class__.__name__, "sample-dataset"]:
+                    for file in glob(f"{ep.load().__path__[0]}/*.py"):
+                        copyfile(file, lib_path / Path(file).name)
 
             for index, (script, detail) in enumerate(candidate_scripts, start=1):
                 script_body = script.validation
                 with open(self.output_dir / f"{index}_script.py", "w", encoding="utf-8") as f:
                     f.write(script_body)
 
         self.debug_info = {}
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/internal_path.py` & `sapientml_core-0.5.5/sapientml_core/internal_path.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/meta_features.py` & `sapientml_core-0.5.5/sapientml_core/meta_features.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/models/feature_importance.json` & `sapientml_core-0.5.5/sapientml_core/models/feature_importance.json`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/models/model_metafeatures_test.csv` & `sapientml_core-0.5.5/sapientml_core/models/model_metafeatures_test.csv`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/models/mp_model_1.pkl` & `sapientml_core-0.5.5/sapientml_core/models/mp_model_1.pkl`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/models/mp_model_2.pkl` & `sapientml_core-0.5.5/sapientml_core/models/mp_model_2.pkl`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/models/pp_models.pkl` & `sapientml_core-0.5.5/sapientml_core/models/pp_models.pkl`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/params.py` & `sapientml_core-0.5.5/sapientml_core/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,28 +69,32 @@
         Random seed for hyperparameter tuning.
     predict_option: Literal["default", "probability", None], default None
         Specify predict method (default: predict(), probability: predict_proba(), None: Comply with metric requirements.)
     permutation_importance: bool, default True
         On/Off of outputting permutation importance calculation code.
     add_explanation: bool, default False
         If True, outputs ipynb files including EDA and explanation.
+    export_preprocess_dataset : bool, default False
+        export pre-processed (feature engineered) the input dataset
+
 
     """
 
     n_models: int = 3
     seed_for_model: int = 42
     id_columns_for_prediction: Optional[list[str]] = None
     use_word_list: Optional[Union[list[str], dict[str, list[str]]]] = None
     hyperparameter_tuning: bool = False
     hyperparameter_tuning_n_trials: int = 10
     hyperparameter_tuning_timeout: int = 0
     hyperparameter_tuning_random_state: int = 1023
     predict_option: Optional[Literal["default", "probability"]] = None
     permutation_importance: bool = True
     add_explanation: bool = False
+    export_preprocess_dataset: bool = False
 
     def postinit(self):
         """Set initial_timeout and hyperparameter_tuning_timeout.
 
         If initial_timeout is set as None and hyperparameter_tuning is false, set initial_timeout as INITIAL_TIMEOUT.
 
         For hyperparameter_tuning_timeout,
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/ps_macros.py` & `sapientml_core-0.5.5/sapientml_core/ps_macros.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/seeding/__init__.py` & `sapientml_core-0.5.5/sapientml_core/seeding/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/seeding/predictor.py` & `sapientml_core-0.5.5/sapientml_core/seeding/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,17 +198,19 @@
     predict_proba = m_model[0].predict_proba(meta_features) + m_model[1].predict_proba(meta_features)
 
     index_ranking = predict_proba.argsort(axis=1)[:, ::-1]
     model_ranking = np.array(m_model[0].classes_)[index_ranking]
 
     model_ranking = [
         [
-            name_to_label_mapping[item][task_type]
-            if item in name_to_label_mapping and task_type in name_to_label_mapping[item]
-            else None
+            (
+                name_to_label_mapping[item][task_type]
+                if item in name_to_label_mapping and task_type in name_to_label_mapping[item]
+                else None
+            )
             for item in preds
         ]
         for preds, task_type in zip(model_ranking, task_type)
     ]
     columns = ["Pred " + str(i + 1) for i in range(len(model_ranking[0]))]
     predictions_df = pd.DataFrame(model_ranking, columns=columns)
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/explainability_templates/component_description.json` & `sapientml_core-0.5.5/sapientml_core/templates/explainability_templates/component_description.json`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/explainability_templates/preprocessing_explanation.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/explainability_templates/preprocessing_explanation.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/hyperparameter_tuning.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/model_templates/hyperparameter_tuning.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/hyperparameters.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/model_templates/hyperparameters.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/hyperparameters_default_value.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/model_templates/hyperparameters_default_value.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/model.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/model_templates/model.py.jinja`

 * *Files 13% similar despite different names*

```diff
@@ -24,25 +24,37 @@
 model = MultiOutputRegressor(model)
 {% elif is_multioutput_classification %}
 from sklearn.multioutput import MultiOutputClassifier
 
 model = MultiOutputClassifier(model)
 {% endif %}
 {% set xgbclassifier = "XGBClassifier" %}
-{% if model_name == xgbclassifier %}
+{% if is_multioutput_classification %}
+from sklearn.preprocessing import LabelEncoder
+label_encoders = {}
+for i, column in enumerate(target_train.columns):
+    le = LabelEncoder()
+    target_train[column] = le.fit_transform(target_train[column])
+    label_encoders[column] = le
+{% elif model_name == xgbclassifier %}
 from sklearn.preprocessing import LabelEncoder
 
 label_encoder = LabelEncoder()
 target_train = pd.DataFrame(label_encoder.fit_transform(target_train), columns=TARGET_COLUMNS)
 {% endif %}
 {% if pipeline.task.target_columns|length == 1 %}
 model.fit(feature_train, target_train.values.ravel())
 {% else %}
 model.fit(feature_train, target_train)
 {% endif %}
 y_pred = model.predict(feature_test)
 {% if flag_predict_proba and (not pipeline.adaptation_metric.startswith("MAP_")) and (not pipeline.adaptation_metric == "LogLoss") and (pipeline.adaptation_metric not in metric_needing_predict_proba) %}
 y_pred = model.classes_[np.argmax(y_pred, axis=1)].reshape(-1, 1)
 {% endif %}
-{% if model_name == xgbclassifier and (not pipeline.adaptation_metric.startswith("MAP_")) and (not pipeline.adaptation_metric == "LogLoss") and (pipeline.adaptation_metric not in metric_needing_predict_proba) %}
+{% if is_multioutput_classification %}
+y_pred_df = pd.DataFrame(y_pred, columns=TARGET_COLUMNS)
+for column in TARGET_COLUMNS:
+    y_pred_df[column] = label_encoders[column].inverse_transform(y_pred_df[column].astype(int))
+y_pred = y_pred_df
+{% elif model_name == xgbclassifier and (not pipeline.adaptation_metric.startswith("MAP_")) and (not pipeline.adaptation_metric == "LogLoss") and (pipeline.adaptation_metric not in metric_needing_predict_proba) %}
 y_pred = label_encoder.inverse_transform(y_pred).reshape(-1, 1)
 {% endif %}
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/model_templates/model_train.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/model_templates/model_train.py.jinja`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,24 @@
 model = MultiOutputRegressor(model)
 {% elif is_multioutput_classification %}
 from sklearn.multioutput import MultiOutputClassifier
 
 model = MultiOutputClassifier(model)
 {% endif %}
 {% set xgbclassifier = "XGBClassifier" %}
-{% if model_name == xgbclassifier %}
+{% if is_multioutput_classification %}
+from sklearn.preprocessing import LabelEncoder
+label_encoders = {}
+for i, column in enumerate(target_train.columns):
+    le = LabelEncoder()
+    target_train[column] = le.fit_transform(target_train[column])
+    label_encoders[column] = le
+with open('target_LabelEncoder.pkl', 'wb') as f:
+    pickle.dump(label_encoders, f)
+{% elif model_name == xgbclassifier %}
 from sklearn.preprocessing import LabelEncoder
 
 label_encoder = LabelEncoder()
 target_train = pd.DataFrame(label_encoder.fit_transform(target_train), columns=TARGET_COLUMNS)
 with open('target_LabelEncoder.pkl', 'wb') as f:
     pickle.dump(label_encoder, f)
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/evaluation.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/other_templates/evaluation.py.jinja`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-{% if target2string %}
-target_test = target_test.astype(str)
-{% endif %}
 {% if pipeline.adaptation_metric == macros.Metric.AUC.value %}
 from sklearn.metrics import roc_auc_score
 {% if pipeline.task.is_multiclass == True %}
 auc = roc_auc_score(target_test.values.ravel(), y_pred, multi_class="ovr")
 {% else %}
 auc = roc_auc_score(target_test, y_pred)
 {% endif %}
@@ -15,22 +12,30 @@
 accuracy = accuracy_score(target_test, y_pred)
 print('RESULT: Accuracy: ' + str(accuracy))
 {% elif (pipeline.adaptation_metric == macros.Metric.Accuracy.value) and (pipeline.is_multi_class_multi_targets) %}
 from sklearn.metrics import accuracy_score
 
 __accs = []
 for i, col in enumerate(target_test.columns):
-    one_acc = accuracy_score(target_test[col], y_pred[:, i:i+1])
+    one_acc = accuracy_score(target_test[col], y_pred[col])
     __accs.append(one_acc)
 print(f"RESULT: Accuracy : {str(sum(__accs)/len(__accs))}")
-{% elif pipeline.adaptation_metric == macros.Metric.F1.value %}
+{% elif pipeline.adaptation_metric == macros.Metric.F1.value and not is_multioutput_classification%}
 from sklearn import metrics
 
 f1 = metrics.f1_score(target_test, y_pred, average='macro')
 print('RESULT: F1 Score: ' + str(f1))
+{% elif pipeline.adaptation_metric == macros.Metric.F1.value and is_multioutput_classification%}
+from sklearn import metrics
+
+__f1s = []
+for i, col in enumerate(target_test.columns):
+    one_f1 = metrics.f1_score(target_test[col], y_pred[col], average='macro')
+    __f1s.append(one_f1)
+print(f"RESULT: F1 Score : {str(sum(__f1s)/len(__f1s))}")
 {% elif pipeline.adaptation_metric == macros.Metric.R2.value %}
 from sklearn import metrics
 
 r2 = metrics.r2_score(target_test, y_pred)
 print('RESULT: R2 Score:', str(r2))
 {% elif pipeline.adaptation_metric == macros.Metric.RMSE.value %}
 from sklearn.metrics import mean_squared_error
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/hyperparameter_tuning_evaluation.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/other_templates/hyperparameter_tuning_evaluation.py.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-{% if target2string %}
-        target_test = target_test.astype(str)
-{% endif %}
 {% if pipeline.adaptation_metric == macros.Metric.AUC.value %}
         from sklearn.metrics import roc_auc_score
 {% if pipeline.task.is_multiclass == True %}
         score = roc_auc_score(target_test.values.ravel(), y_pred, multi_class="ovr")
 {% else %}
         score = roc_auc_score(target_test, y_pred)
 {% endif %}
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/inverse_target.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/other_templates/inverse_target.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/permutation_importance.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/other_templates/permutation_importance.py.jinja`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # PERMUTATION IMPORTANCE
 from sklearn.inspection import permutation_importance
 {% if pipeline.task.target_columns|length == 1 %}
 {% set TARGET_TRAIN = 'target_train[TARGET_COLUMNS[0]]' %}
 {% else %}
 {% set TARGET_TRAIN = 'target_train' %}
 {% endif %}
-{% if target2string %}
-{{ TARGET_TRAIN }} = {{ TARGET_TRAIN }}.astype(str)
-{% endif %}
 {% if pipeline.sparse_matrix %}
 if len(feature_train.columns) <= 100:
     perm = permutation_importance(model, feature_train.sparse.to_dense(), {{ TARGET_TRAIN }},
                                     n_repeats=5,
                                     random_state=0)
     perm_df = pd.DataFrame({"feature": feature_train.columns, "importance": perm.importances_mean})
     perm_df.to_csv("./permutation_importance.csv", index=False)
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/prediction_result.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/other_templates/prediction_result.py.jinja`

 * *Files 13% similar despite different names*

```diff
@@ -10,12 +10,18 @@
 prediction = pd.DataFrame(y_prob, columns=label_encoder.inverse_transform(model.classes_), index=feature_test.index)
 {% elif pipeline.config.predict_option is none and pipeline.task.is_multiclass == True and (pipeline.adaptation_metric in macros.metric_needing_predict_proba) and (not pipeline.adaptation_metric.startswith("MAP_"))%}
 prediction = pd.DataFrame(y_prob, columns=model.classes_, index=feature_test.index)
 {% elif pipeline.config.predict_option is none and (pipeline.adaptation_metric in macros.metric_needing_predict_proba) and (not pipeline.adaptation_metric.startswith("MAP_"))%}
 prediction = pd.DataFrame(y_prob, columns=TARGET_COLUMNS, index=feature_test.index)
 {% elif pipeline.adaptation_metric.startswith("MAP_") %}
 {% set k = pipeline.adaptation_metric.split("_")[1] %}
+{% if y_prob_map_k is none %}
 prediction = pd.DataFrame(y_prob, columns=[TARGET_COLUMNS[0] + "_" +str(i) for i in range(1, y_prob.shape[1] + 1)], index=feature_test.index)
+{% elif is_multioutput_classification %}
+prediction = y_pred
+{% else %}
+prediction = pd.DataFrame(y_prob_map_k, columns=[TARGET_COLUMNS[0] + "_" +str(i) for i in range(1, y_prob_map_k.shape[1] + 1)], index=feature_test.index)
+{% endif %}
 {% else %}
 prediction = pd.DataFrame(y_pred, columns=TARGET_COLUMNS, index=feature_test.index)
 {% endif %}
 prediction.to_csv("./prediction_result.csv")
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/other_templates/shap.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/other_templates/shap.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/pipeline_predict.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/pipeline_predict.py.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,14 @@
 {{ pipeline_json['inverse_target']['code'] }}
 {% endif %}
 {% if 'evaluation' in pipeline_json %}
 
 #EVALUATION
 if set(TARGET_COLUMNS).issubset(test_dataset.columns.tolist()):
 {% filter indent(width=4, first=True) %}
-{{ pipeline_json['evaluation']['code_test'] }}
+{{ pipeline_json['evaluation']['code_predict'] }}
 {% endfilter %}
 {% endif %}
 {% if 'output_prediction' in pipeline_json %}
 
 {{ pipeline_json['output_prediction']['code'] }}
 {% endif %}
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/pipeline_test.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/pipeline_test.py.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 {% endif %}
 {% if flag_hyperparameter_tuning %}
 
 # BEST PARAMETERS IN THE CANDIDATE SCRIPT
 # PLEASE SEE THE CANDIDATE SCRIPTS FOR THE HYPERPARAMTER OPTIMIZATION CODE
 best_params = study.best_params
 {% endif %}
+
+{% if 'preprocess_dataset' in pipeline_json %}
+{{ pipeline_json['preprocess_dataset']['code_test'] }}
+
+{% endif %}
 {% if 'model' in pipeline_json %}
 
 # MODEL
 {{ pipeline_json['model']['code_test'] }}
 {% endif %}
 {% if 'inverse_target' in pipeline_json %}
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/pipeline_train.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/pipeline_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/pipeline_validation.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/pipeline_validation.py.jinja`

 * *Files 12% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 {% endfor %}
 {% endif %}
 {% if flag_hyperparameter_tuning %}
 
 {{ pipeline_json['hyperparameter_optimization']['code'] }}
 {% else %}
 {% if 'model' in pipeline_json %}
+{% if 'preprocess_dataset' in pipeline_json %}
+{{ pipeline_json['preprocess_dataset']['code_test'] }}
+
+{% endif %}
 
 # MODEL
 {{ pipeline_json['model']['code'] }}
 {% endif %}
 {% if 'inverse_target' in pipeline_json %}
 
 {{ pipeline_json['inverse_target']['code'] }}
```

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/DATE.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/DATE.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/Processing.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/Processing.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/Processing_predict.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/Processing_predict.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/Processing_train.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/Processing_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/STANDARD.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/STANDARD.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/TfidfVectorizer.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/TfidfVectorizer.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_predict.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_predict.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_train.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/TfidfVectorizer_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/fillna-type-numeric.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-numeric.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_predict.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_predict.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_train.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-numeric_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/fillna-type-string.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-string.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/fillna-type-string_predict.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-string_predict.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/fillna-type-string_train.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/fillna-type-string_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/get_dummies.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/get_dummies.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/templates/preprocessing_templates/get_dummies_train.py.jinja` & `sapientml_core-0.5.5/sapientml_core/templates/preprocessing_templates/get_dummies_train.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/augmentation/mutation_results.py` & `sapientml_core-0.5.5/sapientml_core/training/augmentation/mutation_results.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/augmentation/mutation_runner.py` & `sapientml_core-0.5.5/sapientml_core/training/augmentation/mutation_runner.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/augmentation/mutator.py` & `sapientml_core-0.5.5/sapientml_core/training/augmentation/mutator.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/dataflowmodel/ast_operation.py` & `sapientml_core-0.5.5/sapientml_core/training/dataflowmodel/ast_operation.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/dataflowmodel/dependent_api_extractor.py` & `sapientml_core-0.5.5/sapientml_core/training/dataflowmodel/dependent_api_extractor.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/dataflowmodel/determine_label_order.py` & `sapientml_core-0.5.5/sapientml_core/training/dataflowmodel/determine_label_order.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/denoising/ast_info_collector.py` & `sapientml_core-0.5.5/sapientml_core/training/denoising/ast_info_collector.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/denoising/dataset_snapshot_extractor.py` & `sapientml_core-0.5.5/sapientml_core/training/denoising/dataset_snapshot_extractor.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/denoising/determine_used_features.py` & `sapientml_core-0.5.5/sapientml_core/training/denoising/determine_used_features.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/denoising/df_collector.py` & `sapientml_core-0.5.5/sapientml_core/training/denoising/df_collector.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/denoising/static_analysis_of_columns.py` & `sapientml_core-0.5.5/sapientml_core/training/denoising/static_analysis_of_columns.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/meta_feature_extractor.py` & `sapientml_core-0.5.5/sapientml_core/training/meta_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/meta_feature_selector.py` & `sapientml_core-0.5.5/sapientml_core/training/meta_feature_selector.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/meta_model_trainer.py` & `sapientml_core-0.5.5/sapientml_core/training/meta_model_trainer.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/pp_model_trainer.py` & `sapientml_core-0.5.5/sapientml_core/training/pp_model_trainer.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/project.py` & `sapientml_core-0.5.5/sapientml_core/training/project.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/training/project_corpus.py` & `sapientml_core-0.5.5/sapientml_core/training/project_corpus.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/sapientml_core/util/file_util.py` & `sapientml_core-0.5.5/sapientml_core/util/file_util.py`

 * *Files identical despite different names*

### Comparing `sapientml_core-0.5.4.post3/PKG-INFO` & `sapientml_core-0.5.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: sapientml-core
-Version: 0.5.4.post3
+Version: 0.5.5
 Summary: A SapientML plugin of SapientMLGenerator
 License: Apache-2.0
 Author: The SapientML Authors
 Maintainer: Kosaku Kimura
 Maintainer-email: kimura.kosaku@fujitsu.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: catboost (>=1.2,<2.0)
-Requires-Dist: imbalanced-learn (>=0.11.0,<0.12.0)
+Requires-Dist: catboost (>=1.2.3)
+Requires-Dist: imbalanced-learn (>=0.11,<0.13)
 Requires-Dist: ipykernel (>=6.25.1,<7.0.0)
 Requires-Dist: japanize-matplotlib (>=1.1.3,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: libcst (>=1.0.1,<2.0.0)
 Requires-Dist: lightgbm (>=4.0.0,<5.0.0)
 Requires-Dist: nbconvert (>=7.7.4,<8.0.0)
 Requires-Dist: nbformat (>=5.9.2,<6.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
-Requires-Dist: numba (>=0.57.1,<0.59.0)
+Requires-Dist: numba (>=0.57.1,<0.60.0)
 Requires-Dist: optuna (>=3.2.0,<4.0.0)
 Requires-Dist: sapientml
 Requires-Dist: sapientml-loaddata
 Requires-Dist: sapientml-preprocess
 Requires-Dist: scikit-learn (==1.3.2)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.14.0)
```

