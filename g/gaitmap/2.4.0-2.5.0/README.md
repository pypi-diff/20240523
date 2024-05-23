# Comparing `tmp/gaitmap-2.4.0.tar.gz` & `tmp/gaitmap-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitmap-2.4.0.tar", max compression
+gzip compressed data, was "gaitmap-2.5.0.tar", max compression
```

## Comparing `gaitmap-2.4.0.tar` & `gaitmap-2.5.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     2032 2024-04-19 10:35:17.873916 gaitmap-2.4.0/LICENSE
--rw-r--r--   0        0        0    11674 2024-04-19 10:35:17.873916 gaitmap-2.4.0/README.md
--rw-r--r--   0        0        0       69 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/__init__.py
--rw-r--r--   0        0        0      164 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/_event_detection_common/__init__.py
--rw-r--r--   0        0        0     7495 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/_event_detection_common/_event_detection_mixin.py
--rw-r--r--   0        0        0    12515 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/base.py
--rw-r--r--   0        0        0     1317 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/data_transform/__init__.py
--rw-r--r--   0        0        0    15973 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/data_transform/_base.py
--rw-r--r--   0        0        0    12043 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/data_transform/_feature_transform.py
--rw-r--r--   0        0        0     3943 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/data_transform/_filter.py
--rw-r--r--   0        0        0    15601 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/data_transform/_scaler.py
--rw-r--r--   0        0        0      765 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/evaluation_utils/__init__.py
--rw-r--r--   0        0        0     6235 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/evaluation_utils/event_detection.py
--rw-r--r--   0        0        0    28906 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/evaluation_utils/parameter_errors.py
--rw-r--r--   0        0        0    11472 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/evaluation_utils/scores.py
--rw-r--r--   0        0        0    22318 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/evaluation_utils/stride_segmentation.py
--rw-r--r--   0        0        0      703 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/event_detection/__init__.py
--rw-r--r--   0        0        0    19365 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/event_detection/_herzer_event_detection.py
--rw-r--r--   0        0        0     8001 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/example_data.py
--rw-r--r--   0        0        0      543 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/gait_detection/__init__.py
--rw-r--r--   0        0        0      351 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/parameters/__init__.py
--rw-r--r--   0        0        0    22578 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/parameters/_spatial_parameters.py
--rw-r--r--   0        0        0     7833 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/parameters/_temporal_parameters.py
--rw-r--r--   0        0        0      288 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/preprocessing/__init__.py
--rw-r--r--   0        0        0      785 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/__init__.py
--rw-r--r--   0        0        0     5089 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py
--rw-r--r--   0        0        0     3940 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py
--rw-r--r--   0        0        0     6665 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py
--rw-r--r--   0        0        0     1732 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/stride_segmentation/__init__.py
--rw-r--r--   0        0        0    14886 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py
--rw-r--r--   0        0        0     2707 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/stride_segmentation/_utils.py
--rw-r--r--   0        0        0     1181 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/stride_segmentation/hmm.py
--rw-r--r--   0        0        0     1355 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/__init__.py
--rw-r--r--   0        0        0    21027 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py
--rw-r--r--   0        0        0     9356 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py
--rw-r--r--   0        0        0    10514 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py
--rw-r--r--   0        0        0      317 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/orientation_methods/__init__.py
--rw-r--r--   0        0        0     8223 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py
--rw-r--r--   0        0        0     4957 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py
--rw-r--r--   0        0        0      618 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py
--rw-r--r--   0        0        0     7849 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py
--rw-r--r--   0        0        0      243 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/trajectory_methods/__init__.py
--rw-r--r--   0        0        0    13674 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py
--rw-r--r--   0        0        0    16858 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py
--rw-r--r--   0        0        0       41 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/__init__.py
--rw-r--r--   0        0        0     1867 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/_algo_helper.py
--rw-r--r--   0        0        0     4609 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/_datatype_validation_helper.py
--rw-r--r--   0        0        0     1241 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/_gaitmap_mad.py
--rw-r--r--   0        0        0      409 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/_types.py
--rw-r--r--   0        0        0    18375 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/array_handling.py
--rw-r--r--   0        0        0     2556 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/consts.py
--rw-r--r--   0        0        0     6272 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/coordinate_conversion.py
--rw-r--r--   0        0        0    48470 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/datatype_helper.py
--rw-r--r--   0        0        0     1193 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/exceptions.py
--rw-r--r--   0        0        0     1866 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/fast_quaternion_math.py
--rw-r--r--   0        0        0    18902 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/rotations.py
--rw-r--r--   0        0        0     2367 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/signal_processing.py
--rw-r--r--   0        0        0    14394 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/static_moment_detection.py
--rw-r--r--   0        0        0     8481 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/stride_list_conversion.py
--rw-r--r--   0        0        0     4124 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/vector_math.py
--rw-r--r--   0        0        0      671 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/zupt_detection/__init__.py
--rw-r--r--   0        0        0     1582 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/zupt_detection/_base.py
--rw-r--r--   0        0        0     3063 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/zupt_detection/_combo_zupt_detector.py
--rw-r--r--   0        0        0    21982 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py
--rw-r--r--   0        0        0     4905 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py
--rw-r--r--   0        0        0     3586 2024-04-19 10:35:17.941916 gaitmap-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    13054 1970-01-01 00:00:00.000000 gaitmap-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2032 2024-05-23 14:22:55.463001 gaitmap-2.5.0/LICENSE
+-rw-r--r--   0        0        0    11674 2024-05-23 14:22:55.463001 gaitmap-2.5.0/README.md
+-rw-r--r--   0        0        0       69 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/_event_detection_common/__init__.py
+-rw-r--r--   0        0        0     7495 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/_event_detection_common/_event_detection_mixin.py
+-rw-r--r--   0        0        0    12515 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/base.py
+-rw-r--r--   0        0        0     1317 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/data_transform/__init__.py
+-rw-r--r--   0        0        0    15973 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/data_transform/_base.py
+-rw-r--r--   0        0        0    12043 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/data_transform/_feature_transform.py
+-rw-r--r--   0        0        0     3943 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/data_transform/_filter.py
+-rw-r--r--   0        0        0    15601 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/data_transform/_scaler.py
+-rw-r--r--   0        0        0      765 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/evaluation_utils/__init__.py
+-rw-r--r--   0        0        0     6235 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/evaluation_utils/event_detection.py
+-rw-r--r--   0        0        0    28906 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/evaluation_utils/parameter_errors.py
+-rw-r--r--   0        0        0    11472 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/evaluation_utils/scores.py
+-rw-r--r--   0        0        0    22318 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/evaluation_utils/stride_segmentation.py
+-rw-r--r--   0        0        0      703 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/event_detection/__init__.py
+-rw-r--r--   0        0        0    19365 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/event_detection/_herzer_event_detection.py
+-rw-r--r--   0        0        0     8001 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/example_data.py
+-rw-r--r--   0        0        0      543 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/gait_detection/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/parameters/__init__.py
+-rw-r--r--   0        0        0    22578 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/parameters/_spatial_parameters.py
+-rw-r--r--   0        0        0     7833 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/parameters/_temporal_parameters.py
+-rw-r--r--   0        0        0      288 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/preprocessing/__init__.py
+-rw-r--r--   0        0        0      785 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/__init__.py
+-rw-r--r--   0        0        0     5089 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py
+-rw-r--r--   0        0        0     3940 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py
+-rw-r--r--   0        0        0     6665 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py
+-rw-r--r--   0        0        0     1732 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/stride_segmentation/__init__.py
+-rw-r--r--   0        0        0    14886 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py
+-rw-r--r--   0        0        0     2707 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/stride_segmentation/_utils.py
+-rw-r--r--   0        0        0     1181 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/stride_segmentation/hmm.py
+-rw-r--r--   0        0        0     1355 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/__init__.py
+-rw-r--r--   0        0        0    21027 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py
+-rw-r--r--   0        0        0     9356 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py
+-rw-r--r--   0        0        0    10514 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py
+-rw-r--r--   0        0        0      317 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/orientation_methods/__init__.py
+-rw-r--r--   0        0        0     8223 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py
+-rw-r--r--   0        0        0     4957 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py
+-rw-r--r--   0        0        0      618 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py
+-rw-r--r--   0        0        0     7849 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py
+-rw-r--r--   0        0        0      243 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/trajectory_methods/__init__.py
+-rw-r--r--   0        0        0    13674 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py
+-rw-r--r--   0        0        0    16858 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py
+-rw-r--r--   0        0        0       41 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/__init__.py
+-rw-r--r--   0        0        0     1867 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/_algo_helper.py
+-rw-r--r--   0        0        0     4609 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/_datatype_validation_helper.py
+-rw-r--r--   0        0        0     1241 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/_gaitmap_mad.py
+-rw-r--r--   0        0        0      409 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/_types.py
+-rw-r--r--   0        0        0    18375 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/array_handling.py
+-rw-r--r--   0        0        0     2556 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/consts.py
+-rw-r--r--   0        0        0     6272 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/coordinate_conversion.py
+-rw-r--r--   0        0        0    48470 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/datatype_helper.py
+-rw-r--r--   0        0        0     1193 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/exceptions.py
+-rw-r--r--   0        0        0     1866 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/fast_quaternion_math.py
+-rw-r--r--   0        0        0    18902 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/utils/rotations.py
+-rw-r--r--   0        0        0     2367 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/utils/signal_processing.py
+-rw-r--r--   0        0        0    14394 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/utils/static_moment_detection.py
+-rw-r--r--   0        0        0     8481 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/utils/stride_list_conversion.py
+-rw-r--r--   0        0        0     4124 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/utils/vector_math.py
+-rw-r--r--   0        0        0      671 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/zupt_detection/__init__.py
+-rw-r--r--   0        0        0     1582 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/zupt_detection/_base.py
+-rw-r--r--   0        0        0     3063 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/zupt_detection/_combo_zupt_detector.py
+-rw-r--r--   0        0        0    21982 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py
+-rw-r--r--   0        0        0     4905 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py
+-rw-r--r--   0        0        0     3589 2024-05-23 14:22:55.531000 gaitmap-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0    13032 1970-01-01 00:00:00.000000 gaitmap-2.5.0/PKG-INFO
```

### Comparing `gaitmap-2.4.0/LICENSE` & `gaitmap-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/README.md` & `gaitmap-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/_event_detection_common/_event_detection_mixin.py` & `gaitmap-2.5.0/gaitmap/_event_detection_common/_event_detection_mixin.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/base.py` & `gaitmap-2.5.0/gaitmap/base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/data_transform/__init__.py` & `gaitmap-2.5.0/gaitmap/data_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/data_transform/_base.py` & `gaitmap-2.5.0/gaitmap/data_transform/_base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/data_transform/_feature_transform.py` & `gaitmap-2.5.0/gaitmap/data_transform/_feature_transform.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/data_transform/_filter.py` & `gaitmap-2.5.0/gaitmap/data_transform/_filter.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/data_transform/_scaler.py` & `gaitmap-2.5.0/gaitmap/data_transform/_scaler.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/evaluation_utils/__init__.py` & `gaitmap-2.5.0/gaitmap/evaluation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/evaluation_utils/event_detection.py` & `gaitmap-2.5.0/gaitmap/evaluation_utils/event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/evaluation_utils/parameter_errors.py` & `gaitmap-2.5.0/gaitmap/evaluation_utils/parameter_errors.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/evaluation_utils/scores.py` & `gaitmap-2.5.0/gaitmap/evaluation_utils/scores.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/evaluation_utils/stride_segmentation.py` & `gaitmap-2.5.0/gaitmap/evaluation_utils/stride_segmentation.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/event_detection/__init__.py` & `gaitmap-2.5.0/gaitmap/event_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/event_detection/_herzer_event_detection.py` & `gaitmap-2.5.0/gaitmap/event_detection/_herzer_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/example_data.py` & `gaitmap-2.5.0/gaitmap/example_data.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/gait_detection/__init__.py` & `gaitmap-2.5.0/gaitmap/gait_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/parameters/_spatial_parameters.py` & `gaitmap-2.5.0/gaitmap/parameters/_spatial_parameters.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/parameters/_temporal_parameters.py` & `gaitmap-2.5.0/gaitmap/parameters/_temporal_parameters.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/__init__.py` & `gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py` & `gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py` & `gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py` & `gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/stride_segmentation/__init__.py` & `gaitmap-2.5.0/gaitmap/stride_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py` & `gaitmap-2.5.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/stride_segmentation/_utils.py` & `gaitmap-2.5.0/gaitmap/stride_segmentation/_utils.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/stride_segmentation/hmm.py` & `gaitmap-2.5.0/gaitmap/stride_segmentation/hmm.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/__init__.py` & `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py` & `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py` & `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py` & `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py` & `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py` & `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py` & `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py` & `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py` & `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py` & `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/_algo_helper.py` & `gaitmap-2.5.0/gaitmap/utils/_algo_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/_datatype_validation_helper.py` & `gaitmap-2.5.0/gaitmap/utils/_datatype_validation_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/_gaitmap_mad.py` & `gaitmap-2.5.0/gaitmap/utils/_gaitmap_mad.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/array_handling.py` & `gaitmap-2.5.0/gaitmap/utils/array_handling.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/consts.py` & `gaitmap-2.5.0/gaitmap/utils/consts.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/coordinate_conversion.py` & `gaitmap-2.5.0/gaitmap/utils/coordinate_conversion.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/datatype_helper.py` & `gaitmap-2.5.0/gaitmap/utils/datatype_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/exceptions.py` & `gaitmap-2.5.0/gaitmap/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/fast_quaternion_math.py` & `gaitmap-2.5.0/gaitmap/utils/fast_quaternion_math.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/rotations.py` & `gaitmap-2.5.0/gaitmap/utils/rotations.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/signal_processing.py` & `gaitmap-2.5.0/gaitmap/utils/signal_processing.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/static_moment_detection.py` & `gaitmap-2.5.0/gaitmap/utils/static_moment_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/stride_list_conversion.py` & `gaitmap-2.5.0/gaitmap/utils/stride_list_conversion.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/utils/vector_math.py` & `gaitmap-2.5.0/gaitmap/utils/vector_math.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/zupt_detection/__init__.py` & `gaitmap-2.5.0/gaitmap/zupt_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/zupt_detection/_base.py` & `gaitmap-2.5.0/gaitmap/zupt_detection/_base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/zupt_detection/_combo_zupt_detector.py` & `gaitmap-2.5.0/gaitmap/zupt_detection/_combo_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py` & `gaitmap-2.5.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py` & `gaitmap-2.5.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.4.0/pyproject.toml` & `gaitmap-2.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gaitmap"
-version = "2.4.0"
+version = "2.5.0"
 description = "The Gait and Movement Analysis Package - Your definite guide to reliable IMU based human movement analysis."
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/gaitmap"
 repository = "https://github.com/mad-lab-fau/gaitmap"
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
@@ -33,17 +33,17 @@
 ]
 numpy = ">=1.20"
 joblib = ">=1.2.0"
 scikit-learn = ">=1.0.1"
 # We restrict it to 0.14.6 for now, as later versions don't seem to work on Linux
 # This version of pomegranate does not support Python 3.10, unfortunately
 pomegranate = {version = ">=0.14.2,<=0.14.6", python = "<3.10", optional = true}
-tpcp = "^0.32.0"
-pingouin = {version = "^0.5.3", optional = true}
-pooch = "^1.7.0"
+tpcp = ">=0.32.0"
+pingouin = {version = ">=0.5.3", optional = true}
+pooch = ">=1.7.0"
 
 [tool.poetry.extras]
 hmm = ["pomegranate"]
 stats = ["pingouin"]
 all = ["pomegranate", "pingouin"]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `gaitmap-2.4.0/PKG-INFO` & `gaitmap-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitmap
-Version: 2.4.0
+Version: 2.5.0
 Summary: The Gait and Movement Analysis Package - Your definite guide to reliable IMU based human movement analysis.
 Home-page: https://github.com/mad-lab-fau/gaitmap
 License: MIT
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.9.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,20 +17,20 @@
 Provides-Extra: hmm
 Provides-Extra: stats
 Requires-Dist: joblib (>=1.2.0)
 Requires-Dist: numba (>=0.55)
 Requires-Dist: numba (>=0.55.2) ; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: numpy (>=1.20)
 Requires-Dist: pandas (>=2)
-Requires-Dist: pingouin (>=0.5.3,<0.6.0) ; extra == "stats" or extra == "all"
+Requires-Dist: pingouin (>=0.5.3) ; extra == "stats" or extra == "all"
 Requires-Dist: pomegranate (>=0.14.2,<=0.14.6) ; (python_version < "3.10") and (extra == "hmm" or extra == "all")
-Requires-Dist: pooch (>=1.7.0,<2.0.0)
+Requires-Dist: pooch (>=1.7.0)
 Requires-Dist: scikit-learn (>=1.0.1)
 Requires-Dist: scipy (>=1.6.1)
-Requires-Dist: tpcp (>=0.32.0,<0.33.0)
+Requires-Dist: tpcp (>=0.32.0)
 Requires-Dist: typing_extensions (>=4.1.1)
 Project-URL: Repository, https://github.com/mad-lab-fau/gaitmap
 Description-Content-Type: text/markdown
 
 <img src="./docs/_static/logo/gaitmap_logo_with_text.png" height="200">
 
 [![PyPI](https://img.shields.io/pypi/v/gaitmap)](https://pypi.org/project/gaitmap/)
```

