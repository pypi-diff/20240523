# Comparing `tmp/portpy-1.0.3.1.tar.gz` & `tmp/portpy-1.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\portpy-1.0.3.1.tar", last modified: Sun May 19 12:57:34 2024, max compression
+gzip compressed data, was "dist\portpy-1.0.3.2.tar", last modified: Thu May 23 19:29:09 2024, max compression
```

## Comparing `portpy-1.0.3.1.tar` & `portpy-1.0.3.2.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:34.000000 portpy-1.0.3.1/
--rw-rw-rw-   0        0        0      142 2023-06-13 16:08:24.000000 portpy-1.0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0    21230 2024-05-19 12:57:34.000000 portpy-1.0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    18430 2024-02-28 22:15:21.000000 portpy-1.0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:27.000000 portpy-1.0.3.1/images/
--rw-rw-rw-   0        0        0    94149 2024-02-28 21:30:18.000000 portpy-1.0.3.1/images/PortPy-full-pipeline.jpg
--rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-1.0.3.1/images/PortPy_logo.jpg
--rw-rw-rw-   0        0        0   179242 2023-07-20 15:30:39.000000 portpy-1.0.3.1/images/dose_comp.JPG
--rw-rw-rw-   0        0        0   161858 2023-07-20 15:59:20.000000 portpy-1.0.3.1/images/planner_vs_portpy_dvh.JPG
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:27.000000 portpy-1.0.3.1/portpy/
--rw-rw-rw-   0        0        0       54 2024-05-19 12:47:45.000000 portpy-1.0.3.1/portpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:28.000000 portpy-1.0.3.1/portpy/ai/
--rw-rw-rw-   0        0        0        2 2023-07-21 17:36:30.000000 portpy-1.0.3.1/portpy/ai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:29.000000 portpy-1.0.3.1/portpy/ai/data/
--rw-rw-rw-   0        0        0     3724 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/data/__init__.py
--rw-rw-rw-   0        0        0     9475 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/data/base_dataset.py
--rw-rw-rw-   0        0        0     3675 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/data/dosepred3d_dataset.py
--rw-rw-rw-   0        0        0     2005 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/data/image_folder.py
--rw-rw-rw-   0        0        0     2353 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/data/single_dataset.py
--rw-rw-rw-   0        0        0     3583 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/data/template_dataset.py
--rw-rw-rw-   0        0        0     4811 2023-07-17 14:00:42.000000 portpy-1.0.3.1/portpy/ai/example.py
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:29.000000 portpy-1.0.3.1/portpy/ai/models/
--rw-rw-rw-   0        0        0     3139 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/models/__init__.py
--rw-rw-rw-   0        0        0    11391 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/models/base_model.py
--rw-rw-rw-   0        0        0     7125 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/models/doseprediction3d_model.py
--rw-rw-rw-   0        0        0    22899 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/models/networks3d.py
--rw-rw-rw-   0        0        0     3490 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/models/test_model.py
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:30.000000 portpy-1.0.3.1/portpy/ai/options/
--rw-rw-rw-   0        0        0     1838 2023-07-21 19:16:51.000000 portpy-1.0.3.1/portpy/ai/options/PyesapiTutorial.py
--rw-rw-rw-   0        0        0      137 2023-07-21 19:16:51.000000 portpy-1.0.3.1/portpy/ai/options/__init__.py
--rw-rw-rw-   0        0        0     8196 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/options/base_options.py
--rw-rw-rw-   0        0        0     1181 2023-07-21 19:16:51.000000 portpy-1.0.3.1/portpy/ai/options/test_options.py
--rw-rw-rw-   0        0        0     3489 2023-07-21 19:16:51.000000 portpy-1.0.3.1/portpy/ai/options/train_options.py
--rw-rw-rw-   0        0        0     5048 2023-07-21 15:27:18.000000 portpy-1.0.3.1/portpy/ai/predict.py
--rw-rw-rw-   0        0        0     2238 2023-07-07 04:18:05.000000 portpy-1.0.3.1/portpy/ai/runRandomTrain.py
--rw-rw-rw-   0        0        0     4596 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/test.py
--rw-rw-rw-   0        0        0     9041 2023-07-21 19:16:53.000000 portpy-1.0.3.1/portpy/ai/train.py
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:31.000000 portpy-1.0.3.1/portpy/ai/util/
--rw-rw-rw-   0        0        0       84 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/util/__init__.py
--rw-rw-rw-   0        0        0     3633 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/util/html.py
--rw-rw-rw-   0        0        0     2280 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/util/image_pool.py
--rw-rw-rw-   0        0        0     4683 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/util/util.py
--rw-rw-rw-   0        0        0    10211 2023-07-21 19:16:52.000000 portpy-1.0.3.1/portpy/ai/util/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:31.000000 portpy-1.0.3.1/portpy/config_files/
--rw-rw-rw-   0        0        0        0 2023-06-13 16:25:21.000000 portpy-1.0.3.1/portpy/config_files/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:26.000000 portpy-1.0.3.1/portpy/config_files/clinical_criteria/
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:31.000000 portpy-1.0.3.1/portpy/config_files/clinical_criteria/Default/
--rw-rw-rw-   0        0        0     3922 2024-05-19 12:27:55.000000 portpy-1.0.3.1/portpy/config_files/clinical_criteria/Default/HN_1Gy_1Fx.json
--rw-rw-rw-   0        0        0     3372 2024-03-25 18:12:20.000000 portpy-1.0.3.1/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:26.000000 portpy-1.0.3.1/portpy/config_files/optimization_params/
--rw-rw-rw-   0        0        0     2815 2023-11-24 11:52:14.000000 portpy-1.0.3.1/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:33.000000 portpy-1.0.3.1/portpy/photon/
--rw-rw-rw-   0        0        0      395 2024-05-19 12:18:24.000000 portpy-1.0.3.1/portpy/photon/__init__.py
--rw-rw-rw-   0        0        0     8347 2024-05-19 12:18:24.000000 portpy-1.0.3.1/portpy/photon/beam.py
--rw-rw-rw-   0        0        0     5417 2024-05-19 12:18:25.000000 portpy-1.0.3.1/portpy/photon/clinical_criteria.py
--rw-rw-rw-   0        0        0      702 2023-06-13 15:15:28.000000 portpy-1.0.3.1/portpy/photon/ct.py
--rw-rw-rw-   0        0        0    25077 2023-07-20 03:11:35.000000 portpy-1.0.3.1/portpy/photon/data_explorer.py
--rw-rw-rw-   0        0        0    20413 2024-05-19 12:18:25.000000 portpy-1.0.3.1/portpy/photon/evaluation.py
--rw-rw-rw-   0        0        0    50525 2024-05-19 12:23:26.000000 portpy-1.0.3.1/portpy/photon/influence_matrix.py
--rw-rw-rw-   0        0        0    29430 2024-05-19 12:18:25.000000 portpy-1.0.3.1/portpy/photon/optimization.py
--rw-rw-rw-   0        0        0     5806 2024-05-19 12:18:25.000000 portpy-1.0.3.1/portpy/photon/plan.py
--rw-rw-rw-   0        0        0    23395 2024-05-19 12:36:34.000000 portpy-1.0.3.1/portpy/photon/structures.py
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:34.000000 portpy-1.0.3.1/portpy/photon/utils/
--rw-rw-rw-   0        0        0      454 2023-08-30 02:17:56.000000 portpy-1.0.3.1/portpy/photon/utils/__init__.py
--rw-rw-rw-   0        0        0     2926 2023-09-29 19:20:32.000000 portpy-1.0.3.1/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py
--rw-rw-rw-   0        0        0     2543 2024-05-19 12:18:26.000000 portpy-1.0.3.1/portpy/photon/utils/get_eclipse_fluence.py
--rw-rw-rw-   0        0        0     8852 2023-08-30 02:17:55.000000 portpy-1.0.3.1/portpy/photon/utils/leaf_sequencing_siochi.py
--rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-1.0.3.1/portpy/photon/utils/save_nrrd.py
--rw-rw-rw-   0        0        0     4887 2024-05-19 12:18:26.000000 portpy-1.0.3.1/portpy/photon/utils/save_or_load_pickle.py
--rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-1.0.3.1/portpy/photon/utils/slicer_script.py
--rw-rw-rw-   0        0        0     4188 2023-06-12 16:42:02.000000 portpy-1.0.3.1/portpy/photon/utils/view_in_slicer_jupyter.py
--rw-rw-rw-   0        0        0     3604 2023-08-30 02:17:55.000000 portpy-1.0.3.1/portpy/photon/utils/write_rt_plan_imrt.py
--rw-rw-rw-   0        0        0    24680 2023-11-24 11:51:19.000000 portpy-1.0.3.1/portpy/photon/visualization.py
-drwxrwxrwx   0        0        0        0 2024-05-19 12:57:27.000000 portpy-1.0.3.1/portpy.egg-info/
--rw-rw-rw-   0        0        0    21230 2024-05-19 12:57:09.000000 portpy-1.0.3.1/portpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2024-05-19 12:57:10.000000 portpy-1.0.3.1/portpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 12:57:09.000000 portpy-1.0.3.1/portpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      367 2024-05-19 12:57:10.000000 portpy-1.0.3.1/portpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-19 12:57:10.000000 portpy-1.0.3.1/portpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 12:57:34.000000 portpy-1.0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2547 2024-05-19 12:54:10.000000 portpy-1.0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:09.000000 portpy-1.0.3.2/
+-rw-rw-rw-   0        0        0      142 2023-06-13 16:08:24.000000 portpy-1.0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    21232 2024-05-23 19:29:09.000000 portpy-1.0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    18432 2024-05-23 19:24:12.000000 portpy-1.0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:01.000000 portpy-1.0.3.2/images/
+-rw-rw-rw-   0        0        0    94149 2024-02-28 21:30:18.000000 portpy-1.0.3.2/images/PortPy-full-pipeline.jpg
+-rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-1.0.3.2/images/PortPy_logo.jpg
+-rw-rw-rw-   0        0        0   179242 2023-07-20 15:30:39.000000 portpy-1.0.3.2/images/dose_comp.JPG
+-rw-rw-rw-   0        0        0   161858 2023-07-20 15:59:20.000000 portpy-1.0.3.2/images/planner_vs_portpy_dvh.JPG
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:01.000000 portpy-1.0.3.2/portpy/
+-rw-rw-rw-   0        0        0       54 2024-05-23 19:24:12.000000 portpy-1.0.3.2/portpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:02.000000 portpy-1.0.3.2/portpy/ai/
+-rw-rw-rw-   0        0        0        2 2023-07-21 17:36:30.000000 portpy-1.0.3.2/portpy/ai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:03.000000 portpy-1.0.3.2/portpy/ai/data/
+-rw-rw-rw-   0        0        0     3724 2023-07-21 19:16:53.000000 portpy-1.0.3.2/portpy/ai/data/__init__.py
+-rw-rw-rw-   0        0        0     9475 2023-07-21 19:16:53.000000 portpy-1.0.3.2/portpy/ai/data/base_dataset.py
+-rw-rw-rw-   0        0        0     3675 2023-07-21 19:16:53.000000 portpy-1.0.3.2/portpy/ai/data/dosepred3d_dataset.py
+-rw-rw-rw-   0        0        0     2005 2023-07-21 19:16:53.000000 portpy-1.0.3.2/portpy/ai/data/image_folder.py
+-rw-rw-rw-   0        0        0     2353 2023-07-21 19:16:53.000000 portpy-1.0.3.2/portpy/ai/data/single_dataset.py
+-rw-rw-rw-   0        0        0     3583 2023-07-21 19:16:53.000000 portpy-1.0.3.2/portpy/ai/data/template_dataset.py
+-rw-rw-rw-   0        0        0     4811 2023-07-17 14:00:42.000000 portpy-1.0.3.2/portpy/ai/example.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:04.000000 portpy-1.0.3.2/portpy/ai/models/
+-rw-rw-rw-   0        0        0     3139 2023-07-21 19:16:52.000000 portpy-1.0.3.2/portpy/ai/models/__init__.py
+-rw-rw-rw-   0        0        0    11391 2023-07-21 19:16:52.000000 portpy-1.0.3.2/portpy/ai/models/base_model.py
+-rw-rw-rw-   0        0        0     7125 2023-07-21 19:16:52.000000 portpy-1.0.3.2/portpy/ai/models/doseprediction3d_model.py
+-rw-rw-rw-   0        0        0    22899 2023-07-21 19:16:52.000000 portpy-1.0.3.2/portpy/ai/models/networks3d.py
+-rw-rw-rw-   0        0        0     3490 2023-07-21 19:16:52.000000 portpy-1.0.3.2/portpy/ai/models/test_model.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:05.000000 portpy-1.0.3.2/portpy/ai/options/
+-rw-rw-rw-   0        0        0     1838 2023-07-21 19:16:51.000000 portpy-1.0.3.2/portpy/ai/options/PyesapiTutorial.py
+-rw-rw-rw-   0        0        0      137 2023-07-21 19:16:51.000000 portpy-1.0.3.2/portpy/ai/options/__init__.py
+-rw-rw-rw-   0        0        0     8196 2023-07-21 19:16:52.000000 portpy-1.0.3.2/portpy/ai/options/base_options.py
+-rw-rw-rw-   0        0        0     1181 2023-07-21 19:16:51.000000 portpy-1.0.3.2/portpy/ai/options/test_options.py
+-rw-rw-rw-   0        0        0     3489 2023-07-21 19:16:51.000000 portpy-1.0.3.2/portpy/ai/options/train_options.py
+-rw-rw-rw-   0        0        0     5048 2023-07-21 15:27:18.000000 portpy-1.0.3.2/portpy/ai/predict.py
+-rw-rw-rw-   0        0        0     2238 2023-07-07 04:18:05.000000 portpy-1.0.3.2/portpy/ai/runRandomTrain.py
+-rw-rw-rw-   0        0        0     4596 2023-07-21 19:16:53.000000 portpy-1.0.3.2/portpy/ai/test.py
+-rw-rw-rw-   0        0        0     9041 2023-07-21 19:16:53.000000 portpy-1.0.3.2/portpy/ai/train.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:05.000000 portpy-1.0.3.2/portpy/ai/util/
+-rw-rw-rw-   0        0        0       84 2023-07-21 19:16:52.000000 portpy-1.0.3.2/portpy/ai/util/__init__.py
+-rw-rw-rw-   0        0        0     3633 2023-07-21 19:16:52.000000 portpy-1.0.3.2/portpy/ai/util/html.py
+-rw-rw-rw-   0        0        0     2280 2023-07-21 19:16:52.000000 portpy-1.0.3.2/portpy/ai/util/image_pool.py
+-rw-rw-rw-   0        0        0     4683 2023-07-21 19:16:52.000000 portpy-1.0.3.2/portpy/ai/util/util.py
+-rw-rw-rw-   0        0        0    10211 2023-07-21 19:16:52.000000 portpy-1.0.3.2/portpy/ai/util/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:05.000000 portpy-1.0.3.2/portpy/config_files/
+-rw-rw-rw-   0        0        0        0 2023-06-13 16:25:21.000000 portpy-1.0.3.2/portpy/config_files/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:00.000000 portpy-1.0.3.2/portpy/config_files/clinical_criteria/
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:06.000000 portpy-1.0.3.2/portpy/config_files/clinical_criteria/Default/
+-rw-rw-rw-   0        0        0     4127 2024-05-23 19:02:16.000000 portpy-1.0.3.2/portpy/config_files/clinical_criteria/Default/HN_1Gy_1Fx.json
+-rw-rw-rw-   0        0        0     3372 2024-03-25 18:12:20.000000 portpy-1.0.3.2/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:06.000000 portpy-1.0.3.2/portpy/config_files/optimization_params/
+-rw-rw-rw-   0        0        0     2714 2024-05-23 19:02:16.000000 portpy-1.0.3.2/portpy/config_files/optimization_params/optimization_params_HN_1Gy_1Fx.json
+-rw-rw-rw-   0        0        0     2815 2023-11-24 11:52:14.000000 portpy-1.0.3.2/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:07.000000 portpy-1.0.3.2/portpy/photon/
+-rw-rw-rw-   0        0        0      395 2024-05-23 19:05:37.000000 portpy-1.0.3.2/portpy/photon/__init__.py
+-rw-rw-rw-   0        0        0     8347 2024-05-23 19:05:37.000000 portpy-1.0.3.2/portpy/photon/beam.py
+-rw-rw-rw-   0        0        0     5417 2024-05-23 19:05:37.000000 portpy-1.0.3.2/portpy/photon/clinical_criteria.py
+-rw-rw-rw-   0        0        0      702 2023-06-13 15:15:28.000000 portpy-1.0.3.2/portpy/photon/ct.py
+-rw-rw-rw-   0        0        0    25077 2023-07-20 03:11:35.000000 portpy-1.0.3.2/portpy/photon/data_explorer.py
+-rw-rw-rw-   0        0        0    26037 2024-05-23 19:19:49.000000 portpy-1.0.3.2/portpy/photon/evaluation.py
+-rw-rw-rw-   0        0        0    50525 2024-05-23 19:05:38.000000 portpy-1.0.3.2/portpy/photon/influence_matrix.py
+-rw-rw-rw-   0        0        0    29430 2024-05-23 19:05:38.000000 portpy-1.0.3.2/portpy/photon/optimization.py
+-rw-rw-rw-   0        0        0     5806 2024-05-23 19:05:38.000000 portpy-1.0.3.2/portpy/photon/plan.py
+-rw-rw-rw-   0        0        0    23395 2024-05-19 12:36:34.000000 portpy-1.0.3.2/portpy/photon/structures.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:09.000000 portpy-1.0.3.2/portpy/photon/utils/
+-rw-rw-rw-   0        0        0      454 2024-05-23 19:05:38.000000 portpy-1.0.3.2/portpy/photon/utils/__init__.py
+-rw-rw-rw-   0        0        0     2926 2023-09-29 19:20:32.000000 portpy-1.0.3.2/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py
+-rw-rw-rw-   0        0        0     2543 2024-05-23 19:05:38.000000 portpy-1.0.3.2/portpy/photon/utils/get_eclipse_fluence.py
+-rw-rw-rw-   0        0        0     8852 2023-08-30 02:17:55.000000 portpy-1.0.3.2/portpy/photon/utils/leaf_sequencing_siochi.py
+-rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-1.0.3.2/portpy/photon/utils/save_nrrd.py
+-rw-rw-rw-   0        0        0     4887 2024-05-23 19:05:38.000000 portpy-1.0.3.2/portpy/photon/utils/save_or_load_pickle.py
+-rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-1.0.3.2/portpy/photon/utils/slicer_script.py
+-rw-rw-rw-   0        0        0     4188 2023-06-12 16:42:02.000000 portpy-1.0.3.2/portpy/photon/utils/view_in_slicer_jupyter.py
+-rw-rw-rw-   0        0        0     3604 2023-08-30 02:17:55.000000 portpy-1.0.3.2/portpy/photon/utils/write_rt_plan_imrt.py
+-rw-rw-rw-   0        0        0    24680 2023-11-24 11:51:19.000000 portpy-1.0.3.2/portpy/photon/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:29:02.000000 portpy-1.0.3.2/portpy.egg-info/
+-rw-rw-rw-   0        0        0    21232 2024-05-23 19:28:42.000000 portpy-1.0.3.2/portpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2094 2024-05-23 19:28:43.000000 portpy-1.0.3.2/portpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:28:42.000000 portpy-1.0.3.2/portpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      367 2024-05-23 19:28:43.000000 portpy-1.0.3.2/portpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 19:28:43.000000 portpy-1.0.3.2/portpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:29:09.000000 portpy-1.0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2547 2024-05-19 12:54:10.000000 portpy-1.0.3.2/setup.py
```

### Comparing `portpy-1.0.3.1/PKG-INFO` & `portpy-1.0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 1.0.3.1
+Version: 1.0.3.2
 Summary: First open-source radiation treatment planning system in Python
 Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.png" width="40%" height="40%">
         </p>
         
-        ![Version](https://img.shields.io/static/v1?label=latest&message=v1.0.3&color=darkgreen)
+        ![Version](https://img.shields.io/static/v1?label=latest&message=v1.0.3.2&color=darkgreen)
         [![Total Downloads](https://static.pepy.tech/personalized-badge/portpy?period=total&units=international_system&left_color=grey&right_color=blue&left_text=total%20downloads)](https://pepy.tech/project/portpy?&left_text=totalusers)
         
         # What is PortPy?
         
         PortPy, short for **P**lanning and **O**ptimization for **R**adiation **T**herapy, represents a collective effort 
         to establish an open-source Python library dedicated to advancing the development and clinical implementation of 
         cancer radiotherapy treatment planning algorithms. This initiative encompasses planning methodologies for
```

### Comparing `portpy-1.0.3.1/README.md` & `portpy-1.0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <p align="center">
   <img src="./images/PortPy_logo.png" width="40%" height="40%">
 </p>
 
-![Version](https://img.shields.io/static/v1?label=latest&message=v1.0.3&color=darkgreen)
+![Version](https://img.shields.io/static/v1?label=latest&message=v1.0.3.2&color=darkgreen)
 [![Total Downloads](https://static.pepy.tech/personalized-badge/portpy?period=total&units=international_system&left_color=grey&right_color=blue&left_text=total%20downloads)](https://pepy.tech/project/portpy?&left_text=totalusers)
 
 # What is PortPy?
 
 PortPy, short for **P**lanning and **O**ptimization for **R**adiation **T**herapy, represents a collective effort 
 to establish an open-source Python library dedicated to advancing the development and clinical implementation of 
 cancer radiotherapy treatment planning algorithms. This initiative encompasses planning methodologies for
```

### Comparing `portpy-1.0.3.1/images/PortPy-full-pipeline.jpg` & `portpy-1.0.3.2/images/PortPy-full-pipeline.jpg`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/images/PortPy_logo.jpg` & `portpy-1.0.3.2/images/PortPy_logo.jpg`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/images/dose_comp.JPG` & `portpy-1.0.3.2/images/dose_comp.JPG`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/images/planner_vs_portpy_dvh.JPG` & `portpy-1.0.3.2/images/planner_vs_portpy_dvh.JPG`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/data/__init__.py` & `portpy-1.0.3.2/portpy/ai/data/__init__.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/data/base_dataset.py` & `portpy-1.0.3.2/portpy/ai/data/base_dataset.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/data/dosepred3d_dataset.py` & `portpy-1.0.3.2/portpy/ai/data/dosepred3d_dataset.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/data/image_folder.py` & `portpy-1.0.3.2/portpy/ai/data/image_folder.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/data/single_dataset.py` & `portpy-1.0.3.2/portpy/ai/data/single_dataset.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/data/template_dataset.py` & `portpy-1.0.3.2/portpy/ai/data/template_dataset.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/example.py` & `portpy-1.0.3.2/portpy/ai/example.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/models/__init__.py` & `portpy-1.0.3.2/portpy/ai/models/__init__.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/models/base_model.py` & `portpy-1.0.3.2/portpy/ai/models/base_model.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/models/doseprediction3d_model.py` & `portpy-1.0.3.2/portpy/ai/models/doseprediction3d_model.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/models/networks3d.py` & `portpy-1.0.3.2/portpy/ai/models/networks3d.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/models/test_model.py` & `portpy-1.0.3.2/portpy/ai/models/test_model.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/options/PyesapiTutorial.py` & `portpy-1.0.3.2/portpy/ai/options/PyesapiTutorial.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/options/base_options.py` & `portpy-1.0.3.2/portpy/ai/options/base_options.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/options/test_options.py` & `portpy-1.0.3.2/portpy/ai/options/test_options.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/options/train_options.py` & `portpy-1.0.3.2/portpy/ai/options/train_options.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/predict.py` & `portpy-1.0.3.2/portpy/ai/predict.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/runRandomTrain.py` & `portpy-1.0.3.2/portpy/ai/runRandomTrain.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/test.py` & `portpy-1.0.3.2/portpy/ai/test.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/train.py` & `portpy-1.0.3.2/portpy/ai/train.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/util/html.py` & `portpy-1.0.3.2/portpy/ai/util/html.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/util/image_pool.py` & `portpy-1.0.3.2/portpy/ai/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/util/util.py` & `portpy-1.0.3.2/portpy/ai/util/util.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/ai/util/visualizer.py` & `portpy-1.0.3.2/portpy/ai/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json` & `portpy-1.0.3.2/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json` & `portpy-1.0.3.2/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/beam.py` & `portpy-1.0.3.2/portpy/photon/beam.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/clinical_criteria.py` & `portpy-1.0.3.2/portpy/photon/clinical_criteria.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/ct.py` & `portpy-1.0.3.2/portpy/photon/ct.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/data_explorer.py` & `portpy-1.0.3.2/portpy/photon/data_explorer.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/influence_matrix.py` & `portpy-1.0.3.2/portpy/photon/influence_matrix.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/optimization.py` & `portpy-1.0.3.2/portpy/photon/optimization.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/plan.py` & `portpy-1.0.3.2/portpy/photon/plan.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/structures.py` & `portpy-1.0.3.2/portpy/photon/structures.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py` & `portpy-1.0.3.2/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/utils/get_eclipse_fluence.py` & `portpy-1.0.3.2/portpy/photon/utils/get_eclipse_fluence.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/utils/leaf_sequencing_siochi.py` & `portpy-1.0.3.2/portpy/photon/utils/leaf_sequencing_siochi.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/utils/save_nrrd.py` & `portpy-1.0.3.2/portpy/photon/utils/save_nrrd.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/utils/save_or_load_pickle.py` & `portpy-1.0.3.2/portpy/photon/utils/save_or_load_pickle.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/utils/slicer_script.py` & `portpy-1.0.3.2/portpy/photon/utils/slicer_script.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/utils/view_in_slicer_jupyter.py` & `portpy-1.0.3.2/portpy/photon/utils/view_in_slicer_jupyter.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/utils/write_rt_plan_imrt.py` & `portpy-1.0.3.2/portpy/photon/utils/write_rt_plan_imrt.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy/photon/visualization.py` & `portpy-1.0.3.2/portpy/photon/visualization.py`

 * *Files identical despite different names*

### Comparing `portpy-1.0.3.1/portpy.egg-info/PKG-INFO` & `portpy-1.0.3.2/portpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 1.0.3.1
+Version: 1.0.3.2
 Summary: First open-source radiation treatment planning system in Python
 Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.png" width="40%" height="40%">
         </p>
         
-        ![Version](https://img.shields.io/static/v1?label=latest&message=v1.0.3&color=darkgreen)
+        ![Version](https://img.shields.io/static/v1?label=latest&message=v1.0.3.2&color=darkgreen)
         [![Total Downloads](https://static.pepy.tech/personalized-badge/portpy?period=total&units=international_system&left_color=grey&right_color=blue&left_text=total%20downloads)](https://pepy.tech/project/portpy?&left_text=totalusers)
         
         # What is PortPy?
         
         PortPy, short for **P**lanning and **O**ptimization for **R**adiation **T**herapy, represents a collective effort 
         to establish an open-source Python library dedicated to advancing the development and clinical implementation of 
         cancer radiotherapy treatment planning algorithms. This initiative encompasses planning methodologies for
```

### Comparing `portpy-1.0.3.1/portpy.egg-info/SOURCES.txt` & `portpy-1.0.3.2/portpy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 portpy/ai/util/html.py
 portpy/ai/util/image_pool.py
 portpy/ai/util/util.py
 portpy/ai/util/visualizer.py
 portpy/config_files/__init__.py
 portpy/config_files/clinical_criteria/Default/HN_1Gy_1Fx.json
 portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
+portpy/config_files/optimization_params/optimization_params_HN_1Gy_1Fx.json
 portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
 portpy/photon/__init__.py
 portpy/photon/beam.py
 portpy/photon/clinical_criteria.py
 portpy/photon/ct.py
 portpy/photon/data_explorer.py
 portpy/photon/evaluation.py
```

### Comparing `portpy-1.0.3.1/setup.py` & `portpy-1.0.3.2/setup.py`

 * *Files identical despite different names*

