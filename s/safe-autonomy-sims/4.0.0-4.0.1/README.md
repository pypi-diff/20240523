# Comparing `tmp/safe_autonomy_sims-4.0.0.tar.gz` & `tmp/safe_autonomy_sims-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_autonomy_sims-4.0.0.tar", max compression
+gzip compressed data, was "safe_autonomy_sims-4.0.1.tar", max compression
```

## Comparing `safe_autonomy_sims-4.0.0.tar` & `safe_autonomy_sims-4.0.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0       34 2024-04-25 14:19:43.956817 safe_autonomy_sims-4.0.0/LICENSE
--rw-r--r--   0        0        0     6533 2024-04-25 14:19:43.956817 safe_autonomy_sims-4.0.0/README.md
--rw-r--r--   0        0        0    11104 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/configuration.md
--rw-r--r--   0        0        0      282 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/css/images.css
--rw-r--r--   0        0        0       90 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/css/material.css
--rw-r--r--   0        0        0      263 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0      895 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/css/style.css
--rw-r--r--   0        0        0    36430 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/experiments.md
--rw-r--r--   0        0        0     1005 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/gen_ref_nav.py
--rw-r--r--   0        0        0   129349 2024-04-25 14:19:44.732819 safe_autonomy_sims-4.0.0/docs/images/HillsFrame2.png
--rw-r--r--   0        0        0   130401 2024-04-25 14:19:44.736819 safe_autonomy_sims-4.0.0/docs/images/HillsFrame3.png
--rw-r--r--   0        0        0    50311 2024-04-25 14:19:44.736819 safe_autonomy_sims-4.0.0/docs/images/inspection_problem.png
--rw-r--r--   0        0        0    41425 2024-04-25 14:19:44.736819 safe_autonomy_sims-4.0.0/docs/images/linear.png
--rw-r--r--   0        0        0    31143 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/images/relu.png
--rw-r--r--   0        0        0    33502 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/images/tanh.png
--rw-r--r--   0        0        0     6407 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/index.md
--rw-r--r--   0        0        0     1393 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/install.md
--rw-r--r--   0        0        0      392 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0    22587 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/docking.md
--rw-r--r--   0        0        0     2650 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/index.md
--rw-r--r--   0        0        0    23806 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_docking.md
--rw-r--r--   0        0        0    27267 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_translational_inspection.md
--rw-r--r--   0        0        0    34877 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_weighted_six_dof_inspection.md
--rw-r--r--   0        0        0    28120 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_weighted_translational_inspection.md
--rw-r--r--   0        0        0    26682 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/translational_inspection.md
--rw-r--r--   0        0        0    30735 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/weighted_six_dof_inspection.md
--rw-r--r--   0        0        0    27367 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/weighted_translational_inspection.md
--rw-r--r--   0        0        0     1207 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/index.md
--rw-r--r--   0        0        0     2322 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/pyproject.toml
--rw-r--r--   0        0        0      827 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/__init__.py
--rw-r--r--   0        0        0      839 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/agents/__init__.py
--rw-r--r--   0        0        0     2828 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/agents/rta_agent.py
--rw-r--r--   0        0        0      936 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/__init__.py
--rw-r--r--   0        0        0    12173 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/common_dones.py
--rw-r--r--   0        0        0      628 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/__init__.py
--rw-r--r--   0        0        0    11159 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/common.py
--rw-r--r--   0        0        0    13464 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/docking_dones.py
--rw-r--r--   0        0        0    12330 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/inspection_dones.py
--rw-r--r--   0        0        0      674 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/__init__.py
--rw-r--r--   0        0        0      643 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/__init__.py
--rw-r--r--   0        0        0     8202 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/base_animation.py
--rw-r--r--   0        0        0    19448 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/inspection_animation.py
--rw-r--r--   0        0        0    10705 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/six_dof_animation.py
--rw-r--r--   0        0        0    18823 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/evaluation_api.py
--rw-r--r--   0        0        0     4992 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/general_metrics.py
--rw-r--r--   0        0        0     6725 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/inspection_metrics.py
--rw-r--r--   0        0        0      661 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/launch/__init__.py
--rw-r--r--   0        0        0     1824 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/launch/serialize_cwh3d.py
--rw-r--r--   0        0        0      787 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/experiments/__init__.py
--rw-r--r--   0        0        0     7087 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/experiments/rllib_api_experiment.py
--rw-r--r--   0        0        0    20658 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/experiments/safe_autonomy_rllib_api_experiment.py
--rw-r--r--   0        0        0     1266 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/__init__.py
--rw-r--r--   0        0        0     3174 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/coordinate_axis_glue.py
--rw-r--r--   0        0        0     3348 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/dot_product_glue.py
--rw-r--r--   0        0        0      984 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/magnitude_glue.py
--rw-r--r--   0        0        0    10361 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/rta_glue.py
--rw-r--r--   0        0        0     7716 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/six_dof_glues.py
--rw-r--r--   0        0        0     3902 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/vel_limit_glue.py
--rw-r--r--   0        0        0     1064 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/__init__.py
--rw-r--r--   0        0        0      615 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/__init__.py
--rw-r--r--   0        0        0     3895 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/controllers.py
--rw-r--r--   0        0        0     1757 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/platform.py
--rw-r--r--   0        0        0     2085 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/sensors.py
--rw-r--r--   0        0        0      613 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/__init__.py
--rw-r--r--   0        0        0     1499 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_available_platforms.py
--rw-r--r--   0        0        0     7656 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_platform.py
--rw-r--r--   0        0        0    15755 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_properties.py
--rw-r--r--   0        0        0    21104 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_sensors.py
--rw-r--r--   0        0        0     5449 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/rotation_sensors.py
--rw-r--r--   0        0        0      971 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/__init__.py
--rw-r--r--   0        0        0      598 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/__init__.py
--rw-r--r--   0        0        0    21566 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/docking_rewards.py
--rw-r--r--   0        0        0     3971 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/done_state_rewards.py
--rw-r--r--   0        0        0     4319 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/gaussian_decay_from_target_value.py
--rw-r--r--   0        0        0    15621 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/inspection_rewards.py
--rw-r--r--   0        0        0     2097 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/live_timestep_reward.py
--rw-r--r--   0        0        0     1820 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/rta_rewards.py
--rw-r--r--   0        0        0     1017 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/__init__.py
--rw-r--r--   0        0        0      603 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/cwh/__init__.py
--rw-r--r--   0        0        0     9407 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/cwh/cwh_rta.py
--rw-r--r--   0        0        0     5785 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/cwh/inspection_rta_1v1.py
--rw-r--r--   0        0        0     8226 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/rta_rejection_sampler.py
--rw-r--r--   0        0        0     1123 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/__init__.py
--rw-r--r--   0        0        0     1262 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/cwh_simulator.py
--rw-r--r--   0        0        0    22988 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/illumination_functions.py
--rw-r--r--   0        0        0      831 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/initializers/__init__.py
--rw-r--r--   0        0        0    15277 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/initializers/cwh.py
--rw-r--r--   0        0        0     7033 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/initializers/initializer.py
--rw-r--r--   0        0        0    31944 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/inspection_simulator.py
--rw-r--r--   0        0        0    16947 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/saferl_simulator.py
--rw-r--r--   0        0        0     9010 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/utils.py
--rw-r--r--   0        0        0     7695 1970-01-01 00:00:00.000000 safe_autonomy_sims-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-05-23 15:26:57.545907 safe_autonomy_sims-4.0.1/LICENSE
+-rw-r--r--   0        0        0     6533 2024-05-23 15:26:57.545907 safe_autonomy_sims-4.0.1/README.md
+-rw-r--r--   0        0        0    11104 2024-05-23 15:26:57.549907 safe_autonomy_sims-4.0.1/docs/configuration.md
+-rw-r--r--   0        0        0      282 2024-05-23 15:26:57.549907 safe_autonomy_sims-4.0.1/docs/css/images.css
+-rw-r--r--   0        0        0       90 2024-05-23 15:26:57.549907 safe_autonomy_sims-4.0.1/docs/css/material.css
+-rw-r--r--   0        0        0      263 2024-05-23 15:26:57.549907 safe_autonomy_sims-4.0.1/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0      895 2024-05-23 15:26:57.549907 safe_autonomy_sims-4.0.1/docs/css/style.css
+-rw-r--r--   0        0        0    36430 2024-05-23 15:26:57.549907 safe_autonomy_sims-4.0.1/docs/experiments.md
+-rw-r--r--   0        0        0     1005 2024-05-23 15:26:57.549907 safe_autonomy_sims-4.0.1/docs/gen_ref_nav.py
+-rw-r--r--   0        0        0   129349 2024-05-23 15:26:58.481903 safe_autonomy_sims-4.0.1/docs/images/HillsFrame2.png
+-rw-r--r--   0        0        0   130401 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/images/HillsFrame3.png
+-rw-r--r--   0        0        0    50311 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/images/inspection_problem.png
+-rw-r--r--   0        0        0    41425 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/images/linear.png
+-rw-r--r--   0        0        0    31143 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/images/relu.png
+-rw-r--r--   0        0        0    33502 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/images/tanh.png
+-rw-r--r--   0        0        0     6407 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/index.md
+-rw-r--r--   0        0        0     1393 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/install.md
+-rw-r--r--   0        0        0      392 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0    22587 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/tasks/CWH/docking.md
+-rw-r--r--   0        0        0     2650 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/tasks/CWH/index.md
+-rw-r--r--   0        0        0    23806 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/tasks/CWH/multiagent_docking.md
+-rw-r--r--   0        0        0    27267 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/tasks/CWH/multiagent_translational_inspection.md
+-rw-r--r--   0        0        0    34877 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/tasks/CWH/multiagent_weighted_six_dof_inspection.md
+-rw-r--r--   0        0        0    28120 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/tasks/CWH/multiagent_weighted_translational_inspection.md
+-rw-r--r--   0        0        0    26682 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/tasks/CWH/translational_inspection.md
+-rw-r--r--   0        0        0    30735 2024-05-23 15:26:58.485903 safe_autonomy_sims-4.0.1/docs/tasks/CWH/weighted_six_dof_inspection.md
+-rw-r--r--   0        0        0    27367 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/docs/tasks/CWH/weighted_translational_inspection.md
+-rw-r--r--   0        0        0     1207 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/docs/tasks/index.md
+-rw-r--r--   0        0        0     2322 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0      827 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/__init__.py
+-rw-r--r--   0        0        0      839 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/agents/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/agents/rta_agent.py
+-rw-r--r--   0        0        0      936 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/dones/__init__.py
+-rw-r--r--   0        0        0    12173 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/dones/common_dones.py
+-rw-r--r--   0        0        0      628 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/dones/cwh/__init__.py
+-rw-r--r--   0        0        0    11159 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/dones/cwh/common.py
+-rw-r--r--   0        0        0    13464 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/dones/cwh/docking_dones.py
+-rw-r--r--   0        0        0    12330 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/dones/cwh/inspection_dones.py
+-rw-r--r--   0        0        0      674 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/__init__.py
+-rw-r--r--   0        0        0      643 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/animation/__init__.py
+-rw-r--r--   0        0        0     8202 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/animation/base_animation.py
+-rw-r--r--   0        0        0    19448 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/animation/inspection_animation.py
+-rw-r--r--   0        0        0    10705 2024-05-23 15:26:58.489904 safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/animation/six_dof_animation.py
+-rw-r--r--   0        0        0    18823 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/evaluation_api.py
+-rw-r--r--   0        0        0     4992 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/general_metrics.py
+-rw-r--r--   0        0        0     6725 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/inspection_metrics.py
+-rw-r--r--   0        0        0      661 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/launch/__init__.py
+-rw-r--r--   0        0        0     1824 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/launch/serialize_cwh3d.py
+-rw-r--r--   0        0        0      787 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/experiments/__init__.py
+-rw-r--r--   0        0        0     7087 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/experiments/rllib_api_experiment.py
+-rw-r--r--   0        0        0    20658 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/experiments/safe_autonomy_rllib_api_experiment.py
+-rw-r--r--   0        0        0     1266 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/__init__.py
+-rw-r--r--   0        0        0     3174 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/coordinate_axis_glue.py
+-rw-r--r--   0        0        0     3348 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/dot_product_glue.py
+-rw-r--r--   0        0        0      984 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/magnitude_glue.py
+-rw-r--r--   0        0        0    10361 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/rta_glue.py
+-rw-r--r--   0        0        0     7716 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/six_dof_glues.py
+-rw-r--r--   0        0        0     3902 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/vel_limit_glue.py
+-rw-r--r--   0        0        0     1064 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/__init__.py
+-rw-r--r--   0        0        0      615 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/common/__init__.py
+-rw-r--r--   0        0        0     3895 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/common/controllers.py
+-rw-r--r--   0        0        0     1757 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/common/platform.py
+-rw-r--r--   0        0        0     2085 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/common/sensors.py
+-rw-r--r--   0        0        0      613 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/cwh/__init__.py
+-rw-r--r--   0        0        0     1499 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/cwh/cwh_available_platforms.py
+-rw-r--r--   0        0        0     7656 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/cwh/cwh_platform.py
+-rw-r--r--   0        0        0    15755 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/cwh/cwh_properties.py
+-rw-r--r--   0        0        0    21104 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/cwh/cwh_sensors.py
+-rw-r--r--   0        0        0     5449 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/cwh/rotation_sensors.py
+-rw-r--r--   0        0        0      971 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/__init__.py
+-rw-r--r--   0        0        0      598 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/cwh/__init__.py
+-rw-r--r--   0        0        0    21566 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/cwh/docking_rewards.py
+-rw-r--r--   0        0        0     3971 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/cwh/done_state_rewards.py
+-rw-r--r--   0        0        0     4319 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/cwh/gaussian_decay_from_target_value.py
+-rw-r--r--   0        0        0    15621 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/cwh/inspection_rewards.py
+-rw-r--r--   0        0        0     2097 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/cwh/live_timestep_reward.py
+-rw-r--r--   0        0        0     1820 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/rta_rewards.py
+-rw-r--r--   0        0        0     1017 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rta/__init__.py
+-rw-r--r--   0        0        0      603 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rta/cwh/__init__.py
+-rw-r--r--   0        0        0     9407 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rta/cwh/cwh_rta.py
+-rw-r--r--   0        0        0     5785 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rta/cwh/inspection_rta_1v1.py
+-rw-r--r--   0        0        0     8226 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/rta/rta_rejection_sampler.py
+-rw-r--r--   0        0        0     1123 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/__init__.py
+-rw-r--r--   0        0        0     1262 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/cwh_simulator.py
+-rw-r--r--   0        0        0    22988 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/illumination_functions.py
+-rw-r--r--   0        0        0      831 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/initializers/__init__.py
+-rw-r--r--   0        0        0    15277 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/initializers/cwh.py
+-rw-r--r--   0        0        0     7033 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/initializers/initializer.py
+-rw-r--r--   0        0        0    32071 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/inspection_simulator.py
+-rw-r--r--   0        0        0    16947 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/saferl_simulator.py
+-rw-r--r--   0        0        0     9010 2024-05-23 15:26:58.493903 safe_autonomy_sims-4.0.1/safe_autonomy_sims/utils.py
+-rw-r--r--   0        0        0     7695 1970-01-01 00:00:00.000000 safe_autonomy_sims-4.0.1/PKG-INFO
```

### Comparing `safe_autonomy_sims-4.0.0/README.md` & `safe_autonomy_sims-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/configuration.md` & `safe_autonomy_sims-4.0.1/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/css/style.css` & `safe_autonomy_sims-4.0.1/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/experiments.md` & `safe_autonomy_sims-4.0.1/docs/experiments.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/gen_ref_nav.py` & `safe_autonomy_sims-4.0.1/docs/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/images/HillsFrame2.png` & `safe_autonomy_sims-4.0.1/docs/images/HillsFrame2.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/images/HillsFrame3.png` & `safe_autonomy_sims-4.0.1/docs/images/HillsFrame3.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/images/inspection_problem.png` & `safe_autonomy_sims-4.0.1/docs/images/inspection_problem.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/images/linear.png` & `safe_autonomy_sims-4.0.1/docs/images/linear.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/images/relu.png` & `safe_autonomy_sims-4.0.1/docs/images/relu.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/images/tanh.png` & `safe_autonomy_sims-4.0.1/docs/images/tanh.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/index.md` & `safe_autonomy_sims-4.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/install.md` & `safe_autonomy_sims-4.0.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/tasks/CWH/docking.md` & `safe_autonomy_sims-4.0.1/docs/tasks/CWH/docking.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/tasks/CWH/index.md` & `safe_autonomy_sims-4.0.1/docs/tasks/CWH/index.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_docking.md` & `safe_autonomy_sims-4.0.1/docs/tasks/CWH/multiagent_docking.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_translational_inspection.md` & `safe_autonomy_sims-4.0.1/docs/tasks/CWH/multiagent_translational_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_weighted_six_dof_inspection.md` & `safe_autonomy_sims-4.0.1/docs/tasks/CWH/multiagent_weighted_six_dof_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_weighted_translational_inspection.md` & `safe_autonomy_sims-4.0.1/docs/tasks/CWH/multiagent_weighted_translational_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/tasks/CWH/translational_inspection.md` & `safe_autonomy_sims-4.0.1/docs/tasks/CWH/translational_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/tasks/CWH/weighted_six_dof_inspection.md` & `safe_autonomy_sims-4.0.1/docs/tasks/CWH/weighted_six_dof_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/tasks/CWH/weighted_translational_inspection.md` & `safe_autonomy_sims-4.0.1/docs/tasks/CWH/weighted_translational_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/docs/tasks/index.md` & `safe_autonomy_sims-4.0.1/docs/tasks/index.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/pyproject.toml` & `safe_autonomy_sims-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "safe-autonomy-sims"
-version = "4.0.0"
+version = "4.0.1"
 description = "The Safe-Autonomy-Sims library provides the components and tools to build modular, integration-focused Reinforcement Learning environments with Run Time Assurance (RTA)"
 authors = [
     "Charles Keating <Charles.Keating@udri.udayton.edu>",
 ]
 license = ""
 readme = "README.md"
 homepage = "https://github.com/act3-ace/safe-autonomy-sims.git"
```

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/agents/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/agents/rta_agent.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/agents/rta_agent.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/dones/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/common_dones.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/dones/common_dones.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/dones/cwh/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/common.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/dones/cwh/common.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/docking_dones.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/dones/cwh/docking_dones.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/inspection_dones.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/dones/cwh/inspection_dones.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/base_animation.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/animation/base_animation.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/inspection_animation.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/animation/inspection_animation.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/six_dof_animation.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/animation/six_dof_animation.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/evaluation_api.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/evaluation_api.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/general_metrics.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/general_metrics.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/inspection_metrics.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/inspection_metrics.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/launch/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/launch/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/launch/serialize_cwh3d.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/evaluation/launch/serialize_cwh3d.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/experiments/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/experiments/rllib_api_experiment.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/experiments/rllib_api_experiment.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/experiments/safe_autonomy_rllib_api_experiment.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/experiments/safe_autonomy_rllib_api_experiment.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/coordinate_axis_glue.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/coordinate_axis_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/dot_product_glue.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/dot_product_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/magnitude_glue.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/magnitude_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/rta_glue.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/rta_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/six_dof_glues.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/six_dof_glues.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/vel_limit_glue.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/glues/vel_limit_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/common/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/controllers.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/common/controllers.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/platform.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/common/platform.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/sensors.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/common/sensors.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/cwh/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_available_platforms.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/cwh/cwh_available_platforms.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_platform.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/cwh/cwh_platform.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_properties.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/cwh/cwh_properties.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_sensors.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/cwh/cwh_sensors.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/rotation_sensors.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/platforms/cwh/rotation_sensors.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/cwh/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/docking_rewards.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/cwh/docking_rewards.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/done_state_rewards.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/cwh/done_state_rewards.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/gaussian_decay_from_target_value.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/cwh/gaussian_decay_from_target_value.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/inspection_rewards.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/cwh/inspection_rewards.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/live_timestep_reward.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/cwh/live_timestep_reward.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/rta_rewards.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rewards/rta_rewards.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rta/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/cwh/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rta/cwh/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/cwh/cwh_rta.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rta/cwh/cwh_rta.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/cwh/inspection_rta_1v1.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rta/cwh/inspection_rta_1v1.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/rta_rejection_sampler.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/rta/rta_rejection_sampler.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/cwh_simulator.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/cwh_simulator.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/illumination_functions.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/illumination_functions.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/initializers/__init__.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/initializers/cwh.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/initializers/cwh.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/initializers/initializer.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/inspection_simulator.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/inspection_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,23 +83,24 @@
         The number of inspectable points maintained.
     radius: float
         The radius of the sphere on which the points will be generated.
     points_algorithm: str
         The name of the algorithm used to generate initial point positions.
     sensor_fov: float
         The field of view of the inspector's camera sensor in radians.
+        Default is 2 * pi (everything is in view).
     initial_sensor_unit_vec: list
         The initial direction the inspector's camera sensor is pointing.
     illumination_params: typing.Union[IlluminationValidator, None]
         The parameters defining lighting of the environment.
     """
     num_points: int
     radius: float
     points_algorithm: str = "cmu"
-    sensor_fov: float = np.pi
+    sensor_fov: float = 2 * np.pi
     initial_sensor_unit_vec: list = [1., 0., 0.]
     illumination_params: typing.Union[IlluminationValidator, None] = None
 
     @validator("points_algorithm")
     def valid_algorithm(cls, v):
         """
         Check if provided algorithm is a valid choice.
@@ -199,18 +200,18 @@
 
         p_hat = position / np.linalg.norm(position)  # position unit vector (inspection zone cone axis)
 
         for point_id, point_position in self.points_position_dict.items():  # pylint: disable=too-many-nested-blocks
             # check that point hasn't already been inspected
             if not self.points_inspected_dict[point_id]:
                 p = point_position - position
-                p_rc = np.dot(p, r_c) * r_c
-                d = np.linalg.norm(p - p_rc)
-                c_r = np.linalg.norm(p_rc) * np.tan(self.config.sensor_fov / 2)
-                if c_r >= d:
+                cos_theta = np.dot(p / np.linalg.norm(p), r_c)
+                angle_to_point = np.arccos(cos_theta)
+                # If the point can be inspected (within FOV)
+                if angle_to_point <= self.config.sensor_fov / 2:
                     # if no illumination params detected
                     if not self.config.illumination_params:
                         # project point onto inspection zone axis and check if in inspection zone
                         if np.dot(point_position, p_hat) >= r - h:
                             self.points_inspected_dict[point_id] = inspector_entity.name
                     else:
                         mag = np.dot(point_position, p_hat)
@@ -497,29 +498,30 @@
     delta_v_scale_step: float
         The amount to advance/retract the delta_v_scale by at each update
     inspected_points_update_bounds: list
         bounds for when to update the delta_v_scale.
         if inspected_points_value >= inspected_points_update_bounds[1], delta_v_scale is advanced by delta_v_scale_step
         if inspected_points_value <= inspected_points_update_bounds[0], delta_v_scale is retracted by delta_v_scale_step
     sensor_fov: float
-        field of view of the sensor (radians). By default pi (180 degrees)
+        field of view of the sensor (radians).
+        Default is 2 * pi (everything is in view).
     initial_sensor_unit_vec: list
         If using the 6DOF spacecraft model, initial unit vector along sensor boresight.
         By default [1., 0., 0.]
     inspection_points_map: dict
         A map of entity name strings to InspectionPoints objects, which track the inspection progress of each entity.
     """
 
     illumination_params: typing.Union[IlluminationValidator, None] = None
     steps_until_update: int
     delta_v_updater_criteria: str = 'count'
     delta_v_scale_bounds: list
     delta_v_scale_step: float
     inspected_points_update_bounds: list
-    sensor_fov: float = np.pi
+    sensor_fov: float = 2 * np.pi
     initial_sensor_unit_vec: list = [1., 0., 0.]
     inspection_points_map: typing.Dict[str, InspectionPointsValidator]
 
     class Config:
         """Allow arbitrary types for Parameter"""
         arbitrary_types_allowed = True
```

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/saferl_simulator.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/simulators/saferl_simulator.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/safe_autonomy_sims/utils.py` & `safe_autonomy_sims-4.0.1/safe_autonomy_sims/utils.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-4.0.0/PKG-INFO` & `safe_autonomy_sims-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-autonomy-sims
-Version: 4.0.0
+Version: 4.0.1
 Summary: The Safe-Autonomy-Sims library provides the components and tools to build modular, integration-focused Reinforcement Learning environments with Run Time Assurance (RTA)
 Home-page: https://github.com/act3-ace/safe-autonomy-sims.git
 Author: Charles Keating
 Author-email: Charles.Keating@udri.udayton.edu
 Requires-Python: >=3.10,<3.11
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

