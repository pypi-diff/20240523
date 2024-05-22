# Comparing `tmp/parallax_app-0.37.6.tar.gz` & `tmp/parallax_app-0.37.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallax_app-0.37.6.tar", last modified: Thu May  9 18:18:04 2024, max compression
+gzip compressed data, was "parallax_app-0.37.7.tar", last modified: Wed May 22 22:21:46 2024, max compression
```

## Comparing `parallax_app-0.37.6.tar` & `parallax_app-0.37.7.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.679052 parallax_app-0.37.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.663052 parallax_app-0.37.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.667052 parallax_app-0.37.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-09 18:17:27.000000 parallax_app-0.37.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-09 18:17:27.000000 parallax_app-0.37.6/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 18:17:27.000000 parallax_app-0.37.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-09 18:17:27.000000 parallax_app-0.37.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-09 18:17:27.000000 parallax_app-0.37.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-09 18:18:04.679052 parallax_app-0.37.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-09 18:17:27.000000 parallax_app-0.37.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.667052 parallax_app-0.37.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/ReadMe.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/parallax.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 18:17:27.000000 parallax_app-0.37.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.667052 parallax_app-0.37.6/img/
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/arrow-right.png
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/gear.png
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/recordingButton.png
--rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/sextant.png
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/snapshotButton_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/stop-sign.png
--rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-09 18:17:27.000000 parallax_app-0.37.6/img/target.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.675052 parallax_app-0.37.6/parallax/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/axis_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20382 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/calibration_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27694 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/curr_bg_cmp_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/curr_prev_cmp_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    32369 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/main_window_wip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/mask_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5664 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/no_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13398 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/probe_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/probe_detect_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18237 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/probe_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/probe_fine_tip_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/recording_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11958 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/reticle_detect_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    23325 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/reticle_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/reticle_detection_coords_interests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13394 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/screen_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    18064 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/stage_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/stage_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    34101 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/stage_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/user_setting_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-09 18:17:27.000000 parallax_app-0.37.6/parallax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.679052 parallax_app-0.37.6/parallax_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-09 18:18:04.000000 parallax_app-0.37.6/parallax_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-09 18:18:04.000000 parallax_app-0.37.6/parallax_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:18:04.000000 parallax_app-0.37.6/parallax_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-09 18:18:04.000000 parallax_app-0.37.6/parallax_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 18:18:04.000000 parallax_app-0.37.6/parallax_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-09 18:17:27.000000 parallax_app-0.37.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:18:04.679052 parallax_app-0.37.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-09 18:17:27.000000 parallax_app-0.37.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.675052 parallax_app-0.37.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 18:17:27.000000 parallax_app-0.37.6/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-09 18:17:27.000000 parallax_app-0.37.6/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-09 18:17:27.000000 parallax_app-0.37.6/tests/test_screen_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.675052 parallax_app-0.37.6/ui/
--rw-r--r--   0 runner    (1001) docker     (127)   192973 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/ParallaxReadME.JPG
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.675052 parallax_app-0.37.6/ui/font/
--rw-r--r--   0 runner    (1001) docker     (127)   259308 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/font/FiraCode-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/mainWindow.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/probe_calib.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:18:04.679052 parallax_app-0.37.6/ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/arrow-right.png
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/check.png
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/gear.png
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/recordingButton.png
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/recordingButton_disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/sextant.png
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/snapshotButton_disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/snapshotButton_green.png
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/snapshotButton_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/stop-sign.png
--rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/target.png
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/resources/x.png
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/reticle_calib.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/settingPopUpMenu.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-09 18:17:27.000000 parallax_app-0.37.6/ui/stage_info.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.794746 parallax_app-0.37.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.778746 parallax_app-0.37.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.778746 parallax_app-0.37.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-22 22:21:06.000000 parallax_app-0.37.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-22 22:21:06.000000 parallax_app-0.37.7/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 22:21:06.000000 parallax_app-0.37.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-22 22:21:06.000000 parallax_app-0.37.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 22:21:06.000000 parallax_app-0.37.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-22 22:21:46.794746 parallax_app-0.37.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-22 22:21:06.000000 parallax_app-0.37.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.782746 parallax_app-0.37.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/ReadMe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/parallax.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 22:21:06.000000 parallax_app-0.37.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.782746 parallax_app-0.37.7/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/gear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/recordingButton.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/sextant.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/snapshotButton_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/stop-sign.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-22 22:21:06.000000 parallax_app-0.37.7/img/target.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.786746 parallax_app-0.37.7/parallax/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/axis_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20382 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/calibration_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27905 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/curr_bg_cmp_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/curr_prev_cmp_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32369 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/main_window_wip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/mask_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6058 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/no_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15573 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/probe_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13433 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/probe_detect_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18237 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/probe_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/probe_fine_tip_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/recording_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11958 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/reticle_detect_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23325 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/reticle_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/reticle_detection_coords_interests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13577 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/screen_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18248 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/stage_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/stage_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39667 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/stage_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/user_setting_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-22 22:21:06.000000 parallax_app-0.37.7/parallax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.790746 parallax_app-0.37.7/parallax_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-22 22:21:46.000000 parallax_app-0.37.7/parallax_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-22 22:21:46.000000 parallax_app-0.37.7/parallax_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:21:46.000000 parallax_app-0.37.7/parallax_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-22 22:21:46.000000 parallax_app-0.37.7/parallax_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 22:21:46.000000 parallax_app-0.37.7/parallax_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 22:21:06.000000 parallax_app-0.37.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:21:46.794746 parallax_app-0.37.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-22 22:21:06.000000 parallax_app-0.37.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.786746 parallax_app-0.37.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-22 22:21:06.000000 parallax_app-0.37.7/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-22 22:21:06.000000 parallax_app-0.37.7/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-22 22:21:06.000000 parallax_app-0.37.7/tests/test_screen_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.790746 parallax_app-0.37.7/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)   192973 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/ParallaxReadME.JPG
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.790746 parallax_app-0.37.7/ui/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   259308 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/font/FiraCode-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/mainWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/probe_calib.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:21:46.790746 parallax_app-0.37.7/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/check.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/gear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/recordingButton.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/recordingButton_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/sextant.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/snapshotButton_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/snapshotButton_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/snapshotButton_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/stop-sign.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/target.png
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/resources/x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/reticle_calib.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/settingPopUpMenu.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-22 22:21:06.000000 parallax_app-0.37.7/ui/stage_info.ui
```

### Comparing `parallax_app-0.37.6/.github/workflows/ci.yml` & `parallax_app-0.37.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/.github/workflows/tag_and_publish.yml` & `parallax_app-0.37.7/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/LICENSE` & `parallax_app-0.37.7/LICENSE`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/PKG-INFO` & `parallax_app-0.37.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallax-app
-Version: 0.37.6
+Version: 0.37.7
 Summary: GUI software for photogrammetry-assisted probe targeting in electrophysiology
 Author-email: Hanna Lee <hanna.lee@alleninstitute.org>
 License: MIT
 Keywords: parallax
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
@@ -36,18 +36,19 @@
 
 # Parallax
 
 ![Parallax](ui/ParallaxReadME.JPG)
 
 Parallax is a graphical user interface designed to streamline the process of setting up and performing acute *in vivo* electrophysiology experiments.
 
-User documentation available on [here](https://parallax.readthedocs.io/en/latest/).
+User documentation available on [here](https://parallax.readthedocs.io/en/stable/).
 
 ### Prerequisites
 - **Python~=3.8** (Recommended to install via [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
+  -  Python 3.8 is required for the Spinnaker library.
 - PySpin (for Linux or Mac OS users)
 
 
 ### Installation
 1. Create virtual environment using **Python version 3.8** and activate it:
 - On Windows:
 ```bash
```

### Comparing `parallax_app-0.37.6/README.md` & `parallax_app-0.37.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Parallax
 
 ![Parallax](ui/ParallaxReadME.JPG)
 
 Parallax is a graphical user interface designed to streamline the process of setting up and performing acute *in vivo* electrophysiology experiments.
 
-User documentation available on [here](https://parallax.readthedocs.io/en/latest/).
+User documentation available on [here](https://parallax.readthedocs.io/en/stable/).
 
 ### Prerequisites
 - **Python~=3.8** (Recommended to install via [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
+  -  Python 3.8 is required for the Spinnaker library.
 - PySpin (for Linux or Mac OS users)
 
 
 ### Installation
 1. Create virtual environment using **Python version 3.8** and activate it:
 - On Windows:
 ```bash
```

### Comparing `parallax_app-0.37.6/docs/Makefile` & `parallax_app-0.37.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/docs/ReadMe.rst` & `parallax_app-0.37.7/docs/ReadMe.rst`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/docs/conf.py` & `parallax_app-0.37.7/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 import os
 import sys
+from parallax import __version__ as version
 
 sys.path.insert(0, os.path.abspath(".."))
 
 project = 'Parallax'
 copyright = '2024, Hanna Lee'
 author = 'Hanna Lee'
-release = '0.37.1'
+release = version # Automatically set version from parallax package
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.todo", "sphinx.ext.viewcode", "sphinx.ext.autodoc"]
 
 templates_path = ['_templates']
```

### Comparing `parallax_app-0.37.6/docs/make.bat` & `parallax_app-0.37.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/docs/parallax.rst` & `parallax_app-0.37.7/docs/parallax.rst`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/img/arrow-right.png` & `parallax_app-0.37.7/img/arrow-right.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/img/gear.png` & `parallax_app-0.37.7/img/gear.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/img/recordingButton.png` & `parallax_app-0.37.7/img/recordingButton.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/img/sextant.png` & `parallax_app-0.37.7/img/sextant.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/img/snapshotButton_white.png` & `parallax_app-0.37.7/img/snapshotButton_white.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/img/stop-sign.png` & `parallax_app-0.37.7/img/stop-sign.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/img/target.png` & `parallax_app-0.37.7/img/target.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/__main__.py` & `parallax_app-0.37.7/parallax/__main__.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/axis_filter.py` & `parallax_app-0.37.7/parallax/axis_filter.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/calibration_camera.py` & `parallax_app-0.37.7/parallax/calibration_camera.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/camera.py` & `parallax_app-0.37.7/parallax/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,14 +377,23 @@
         sn = self.camera.DeviceSerialNumber()
         device_model = self.camera.DeviceModelName()
         if sn_only:
             return sn
         else:
             return "%s (Serial # %s)" % (device_model, sn)
 
+    def get_device_color_type(self):
+        """
+        Retrieves the color type of the camera.
+
+        Returns:
+        - str: The color type of the camera.
+        """
+        return self.device_color_type
+
     def begin_singleframe_acquisition(self):
         """
         Begings a single Frame image acquisition.
         """
         # set acquisition mode to singleFrame
         node_acquisition_mode = PySpin.CEnumerationPtr(
             self.node_map.GetNode("AcquisitionMode")
```

### Comparing `parallax_app-0.37.6/parallax/curr_bg_cmp_processor.py` & `parallax_app-0.37.7/parallax/curr_bg_cmp_processor.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/curr_prev_cmp_processor.py` & `parallax_app-0.37.7/parallax/curr_prev_cmp_processor.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/main_window_wip.py` & `parallax_app-0.37.7/parallax/main_window_wip.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
             newNameMicroscope = f"Microscope_{screen_index+1}"
         microscopeGrp = QGroupBox(self.scrollAreaWidgetContents)
 
         # Construct and configure the Microscope widget
         microscopeGrp.setObjectName(newNameMicroscope)
         microscopeGrp.setStyleSheet("background-color: rgb(58, 58, 58);")
         font_grpbox = QFont()
-        font_grpbox.setPointSize(9)  # Setting font size to 9
+        font_grpbox.setPointSize(8)  # Setting font size to 9
         microscopeGrp.setFont(font_grpbox)
         verticalLayout = QVBoxLayout(microscopeGrp)
         verticalLayout.setObjectName("verticalLayout")
 
         # Add screens
         if mock:
             screen = ScreenWidget(
```

### Comparing `parallax_app-0.37.6/parallax/mask_generator.py` & `parallax_app-0.37.7/parallax/mask_generator.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/model.py` & `parallax_app-0.37.7/parallax/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         self.cameras_sn = []
         self.nPySpinCameras = 0
         self.nMockCameras = 0
         self.focos = []
 
         # stage
         self.nStages = 0
-        self.init_stages()
-        self.elevators = {}
+        self.stages = {}
+        self.stages_calib = {}
         self.stage_listener_url = "http://localhost:8080/"
 
         # probe detector
         self.probeDetectors = []
 
         # coords axis
         self.coords_axis = {}
@@ -77,14 +77,15 @@
     def clear_rcorr(self):
         """Clear right coordinates."""
         self.rcorr = False
 
     def init_stages(self):
         """Initialize stages."""
         self.stages = {}
+        self.stages_calib = {}
 
     def add_video_source(self, video_source):
         """Add a video source."""
         self.cameras.append(video_source)
 
     def add_mock_cameras(self, n=1):
         """Add mock cameras."""
@@ -124,14 +125,26 @@
         """Add a stage."""
         self.stages[stage.sn] = stage
 
     def get_stage(self, stage_sn):
         """Get a stage."""
         return self.stages.get(stage_sn)
 
+    def add_stage_calib_info(self, stage_sn, info):
+        """Add a stage."""
+        self.stages_calib[stage_sn] = info
+
+    def get_stage_calib_info(self, stage_sn):
+        """Get a stage."""
+        return self.stages_calib.get(stage_sn)
+    
+    def reset_stage_calib_info(self):
+        """Reset stage calibration info."""
+        self.stages_calib = {}
+
     def add_probe_detector(self, probeDetector):
         """Add a probe detector."""
         self.probeDetectors.append(probeDetector)
 
     def reset_coords_intrinsic_extrinsic(self):
         """Reset coordinates intrinsic extrinsic."""
         self.coords_axis = {}
```

### Comparing `parallax_app-0.37.6/parallax/no_filter.py` & `parallax_app-0.37.7/parallax/no_filter.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/probe_calibration.py` & `parallax_app-0.37.7/parallax/probe_calibration.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,84 +8,92 @@
 import logging
 import os
 
 import numpy as np
 import pandas as pd
 from PyQt5.QtCore import QObject, pyqtSignal
 from sklearn.linear_model import LinearRegression
+from sklearn.linear_model import Ridge
 
 # Set logger name
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
 
-
 class ProbeCalibration(QObject):
     """
     Handles the transformation of probe coordinates from local (stage) to global (reticle) space.
 
     Attributes:
         calib_complete_x (pyqtSignal): Signal emitted when calibration in the X direction is complete.
         calib_complete_y (pyqtSignal): Signal emitted when calibration in the Y direction is complete.
         calib_complete_z (pyqtSignal): Signal emitted when calibration in the Z direction is complete.
         calib_complete (pyqtSignal): General signal emitted when calibration is fully complete.
 
     Args:
         stage_listener (QObject): The stage listener object that emits signals related to stage movements.
     """
 
-    calib_complete_x = pyqtSignal()
-    calib_complete_y = pyqtSignal()
-    calib_complete_z = pyqtSignal()
+    calib_complete_x = pyqtSignal(str)
+    calib_complete_y = pyqtSignal(str)
+    calib_complete_z = pyqtSignal(str)
     calib_complete = pyqtSignal(str, object)
-    transM_info = pyqtSignal(object, float, object)
+    transM_info = pyqtSignal(str, object, float, object)
 
     """Class for probe calibration."""
 
     def __init__(self, stage_listener):
         """
         Initializes the ProbeCalibration object with a given stage listener.
         """
         super().__init__()
         self.stage_listener = stage_listener
         self.stage_listener.probeCalibRequest.connect(self.update)
         self.stages = {}
         self.df = None
         self.inliers = []
         self.stage = None
-        self.threshold_min_max = 2000  # TODO
-        self.model_LR, self.transM_LR, self.transM_LR_prev = None, None, None
+        self.threshold_min_max = 2500 
+        self.threshold_min_max_z = 2000
+        self.LR_err_L2_threshold = 20
         self.threshold_matrix = np.array(
             [
                 [0.00002, 0.00002, 0.00002, 50.0],  # TODO
                 [0.00002, 0.00002, 0.00002, 50.0],
                 [0.00002, 0.00002, 0.00002, 50.0],
                 [0.0, 0.0, 0.0, 0.0],
             ]
         )
-        self.LR_err_L2_threshold = 20  # TODO
+        self.model_LR, self.transM_LR, self.transM_LR_prev = None, None, None
         self._create_file()
 
-        # Test signal
-        self.reset_calib()
-
-    def reset_calib(self):
+    def reset_calib(self, sn=None):
         """
         Resets calibration to its initial state, clearing any stored min and max values.
+        Called from StageWidget.
         """
-        self.min_x, self.max_x = float("inf"), float("-inf")
-        self.min_y, self.max_y = float("inf"), float("-inf")
-        self.min_z, self.max_z = float("inf"), float("-inf")
-        self.transM_LR_prev = np.zeros((4, 4), dtype=np.float64)
-        self.signal_emitted_x = False
-        self.signal_emitted_y = False
-        self.signal_emitted_z = False
+        if sn is not None:
+             self.stages[sn] = {
+            'min_x': float("inf"),
+            'max_x': float("-inf"),
+            'min_y': float("inf"),
+            'max_y': float("-inf"),
+            'min_z': float("inf"),
+            'max_z': float("-inf"),
+            'signal_emitted_x': False,
+            'signal_emitted_y': False,
+            'signal_emitted_z': False
+        }
+        else:
+            self.stages = {}
 
+        self.transM_LR_prev = np.zeros((4, 4), dtype=np.float64)
+        
     def _create_file(self):
         """
         Creates or clears the CSV file used to store local and global points during calibration.
         """
         package_dir = os.path.dirname(os.path.abspath(__file__))
         debug_dir = os.path.join(os.path.dirname(package_dir), "debug")
         os.makedirs(debug_dir, exist_ok=True)
@@ -96,14 +104,15 @@
             os.remove(self.csv_file)
 
         # Create a new file and write column names
         with open(self.csv_file, "w", newline="") as file:
             writer = csv.writer(file)
             # Define column names
             column_names = [
+                "sn",
                 "local_x",
                 "local_y",
                 "local_z",
                 "global_x",
                 "global_y",
                 "global_z",
                 "ts_local_coords",
@@ -111,32 +120,40 @@
                 "cam0",
                 "pt0",
                 "cam1",
                 "pt1"
             ]
             writer.writerow(column_names)
 
-    def clear(self):
+    def clear(self, sn = None):
         """
         Clears all stored data and resets the transformation matrix to its default state.
         """
-        self._create_file()
+        if sn is None:
+            self._create_file()
+        else:
+            self.df = pd.read_csv(self.csv_file)
+            self.df = self.df[self.df["sn"] != sn]
+            self.df.to_csv(self.csv_file, index=False)
         self.model_LR, self.transM_LR, self.transM_LR_prev = None, None, None
 
     def _get_local_global_points(self):
         """
         Retrieves local and global points from the CSV file as numpy arrays.
 
         Returns:
             tuple: A tuple containing arrays of local points and global points.
         """
         self.df = pd.read_csv(self.csv_file)
+        # Filter the DataFrame based on self.stage.sn
+        filtered_df = self.df[self.df["sn"] == self.stage.sn]
         # Extract local and global points
-        local_points = self.df[["local_x", "local_y", "local_z"]].values
-        global_points = self.df[["global_x", "global_y", "global_z"]].values
+        local_points = filtered_df[["local_x", "local_y", "local_z"]].values
+        global_points = filtered_df[["global_x", "global_y", "global_z"]].values
+        
         return local_points, global_points
 
     def _get_transM_LR(self, local_points, global_points):
         """
         Computes the transformation matrix from local to global coordinates.
 
         Args:
@@ -147,15 +164,16 @@
             tuple: Linear regression model and transformation matrix.
         """
         local_points_with_bias = np.hstack(
             [local_points, np.ones((local_points.shape[0], 1))]
         )
 
         # Train the linear regression model
-        model = LinearRegression(fit_intercept=False)
+        model = LinearRegression(fit_intercept=False) 
+        #model = Ridge(alpha=1.0, fit_intercept=False) # TODO
         model.fit(local_points_with_bias, global_points)
 
         # Weights and Bias
         # All but last column, which are the weights
         weights = model.coef_[:, :-1]
         bias = model.coef_[:, -1] # Last column, which is the bias
 
@@ -169,14 +187,15 @@
     def _update_local_global_point(self, debug_info=None):
         """
         Updates the CSV file with a new set of local and global points from the current stage position.
         """
         with open(self.csv_file, "a", newline='') as file:
             writer = csv.writer(file)
             row_data = [
+                self.stage.sn,
                 self.stage.stage_x,
                 self.stage.stage_y,
                 self.stage.stage_z,
                 self.stage.stage_x_global,
                 self.stage.stage_y_global,
                 self.stage.stage_z_global,
             ]
@@ -206,43 +225,44 @@
         diff_matrix = np.abs(self.transM_LR - self.transM_LR_prev)
         if np.all(diff_matrix <= self.threshold_matrix):
             return True
         else:
             return False
 
     def _update_min_max_x_y_z(self):
-        self.min_x, self.max_x = min(self.min_x, self.stage.stage_x), max(
-            self.max_x, self.stage.stage_x
-        )
-        self.min_y, self.max_y = min(self.min_y, self.stage.stage_y), max(
-            self.max_y, self.stage.stage_y
-        )
-        self.min_z, self.max_z = min(self.min_z, self.stage.stage_z), max(
-            self.max_z, self.stage.stage_z
-        )
-
+        sn = self.stage.sn
+        if sn not in self.stages:
+            self.stages[sn] = {
+                'min_x': float("inf"), 'max_x': float("-inf"),
+                'min_y': float("inf"), 'max_y': float("-inf"),
+                'min_z': float("inf"), 'max_z': float("-inf")
+            }
+
+        self.stages[sn]['min_x'] = min(self.stages[sn]['min_x'], self.stage.stage_x)
+        self.stages[sn]['max_x'] = max(self.stages[sn]['max_x'], self.stage.stage_x)
+        self.stages[sn]['min_y'] = min(self.stages[sn]['min_y'], self.stage.stage_y)
+        self.stages[sn]['max_y'] = max(self.stages[sn]['max_y'], self.stage.stage_y)
+        self.stages[sn]['min_z'] = min(self.stages[sn]['min_z'], self.stage.stage_z)
+        self.stages[sn]['max_z'] = max(self.stages[sn]['max_z'], self.stage.stage_z)
+       
     def _is_criteria_met_points_min_max(self):
-        """
-        Checks if the range of collected points in each direction exceeds minimum thresholds.
-
-        Returns:
-            bool: True if sufficient range is achieved, otherwise False.
-        """
+        sn = self.stage.sn
+        if sn is not None and sn in self.stages:
+            stage_data = self.stages[sn]
         
-        if self.max_x - self.min_x > self.threshold_min_max \
-            or self.max_y - self.min_y > self.threshold_min_max \
-            or self.max_z - self.min_z > self.threshold_min_max:
-            self._enough_points_emit_signal()
-
-        if self.max_x - self.min_x > self.threshold_min_max \
-            and self.max_y - self.min_y > self.threshold_min_max \
-            and self.max_z - self.min_z > self.threshold_min_max:
-            return True
-        else:
-            return False
+            if (stage_data['max_x'] - stage_data['min_x'] > self.threshold_min_max or
+                stage_data['max_y'] - stage_data['min_y'] > self.threshold_min_max or
+                stage_data['max_z'] - stage_data['min_z'] > self.threshold_min_max_z):
+                self._enough_points_emit_signal()
+
+            if (stage_data['max_x'] - stage_data['min_x'] > self.threshold_min_max and
+                stage_data['max_y'] - stage_data['min_y'] > self.threshold_min_max and
+                stage_data['max_z'] - stage_data['min_z'] > self.threshold_min_max_z):
+                return True
+        return False
 
     def _apply_transformation(self):
         """
         Applies the calculated transformation matrix to convert a local point to global coordinates.
 
         Returns:
             np.array: The transformed global point.
@@ -278,32 +298,39 @@
         else:
             return False
 
     def _enough_points_emit_signal(self):
         """
         Emits calibration complete signals based on the sufficiency of point ranges in each direction.
         """
-        if (
-            not self.signal_emitted_x
-            and self.max_x - self.min_x > self.threshold_min_max
-        ):
-            self.calib_complete_x.emit()
-            self.signal_emitted_x = True
-        if (
-            not self.signal_emitted_y
-            and self.max_y - self.min_y > self.threshold_min_max
-        ):
-            self.calib_complete_y.emit()
-            self.signal_emitted_y = True
-        if (
-            not self.signal_emitted_z
-            and self.max_z - self.min_z > self.threshold_min_max
-        ):
-            self.calib_complete_z.emit()
-            self.signal_emitted_z = True
+        sn = self.stage.sn
+        if sn is not None and sn in self.stages:
+            stage_data = self.stages[sn]
+
+            if (
+                not stage_data.get('signal_emitted_x', False)
+                and stage_data['max_x'] - stage_data['min_x'] > self.threshold_min_max
+            ):
+                self.calib_complete_x.emit(sn)
+                stage_data['signal_emitted_x'] = True
+            if (
+                not stage_data.get('signal_emitted_y', False)
+                and stage_data['max_y'] - stage_data['min_y'] > self.threshold_min_max
+            ):
+                self.calib_complete_y.emit(sn)
+                stage_data['signal_emitted_y'] = True
+            if (
+                not stage_data.get('signal_emitted_z', False)
+                and stage_data['max_z'] - stage_data['min_z'] > self.threshold_min_max_z
+            ):
+                self.calib_complete_z.emit(sn)
+                stage_data['signal_emitted_z'] = True
+            
+            # Update self.stages with the new signal emitted status
+            self.stages[sn] = stage_data
 
     def _is_enough_points(self):
         """Check if there are enough points for calibration.
 
         Returns:
             bool: True if there are enough points, False otherwise.
         """
@@ -317,22 +344,39 @@
                     logger.debug("Enough points gathered.")
                     return True
 
         self.transM_LR_prev = self.transM_LR
         return False
 
     def _update_info_ui(self):
+        """
         x_diff = self.max_x - self.min_x
         y_diff = self.max_y - self.min_y
         z_diff = self.max_z - self.min_z
         self.transM_info.emit(
+            self.stage.sn,
             self.transM_LR,
             self.LR_err_L2_current,
             np.array([x_diff, y_diff, z_diff]),
         )
+        """
+        sn = self.stage.sn
+        if sn is not None and sn in self.stages:
+            stage_data = self.stages[sn]
+            
+            x_diff = stage_data['max_x'] - stage_data['min_x']
+            y_diff = stage_data['max_y'] - stage_data['min_y']
+            z_diff = stage_data['max_z'] - stage_data['min_z']
+            
+            self.transM_info.emit(
+                sn,
+                self.transM_LR,
+                self.LR_err_L2_current,
+                np.array([x_diff, y_diff, z_diff]),
+            )
 
     def update(self, stage, debug_info=None):
         """
         Main method to update calibration with a new stage position and check if calibration is complete.
 
         Args:
             stage (Stage): The current stage object with new position data.
```

### Comparing `parallax_app-0.37.6/parallax/probe_detect_manager.py` & `parallax_app-0.37.7/parallax/probe_detect_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,26 +213,26 @@
                     for point_idx, (x, y) in enumerate(coords):
                         color = colormap[point_idx][0].tolist()
                         cv2.circle(frame, (x, y), 2, color, -1)
             return frame
 
         def run(self):
             """Run the worker thread."""
-            print("probe_detect_manager running ")
+            logger.debug("probe_detect_manager running ")
             while self.running:
                 if self.new:
                     if self.is_detection_on:
                         self.frame, self.timestamp = self.process(
                             self.frame, self.timestamp
                         )
                     self.frame = self.process_draw_reticle(self.frame)
                     self.frame_processed.emit(self.frame)
                     self.new = False
                 time.sleep(0.001)
-            print("probe_detect_manager running done")
+            logger.debug("probe_detect_manager running done")
             self.finished.emit()
 
         def set_name(self, name):
             """Set name as camera serial number."""
             self.name = name
             self.reticle_coords = self.model.get_coords_axis(self.name)
```

### Comparing `parallax_app-0.37.6/parallax/probe_detector.py` & `parallax_app-0.37.7/parallax/probe_detector.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/probe_fine_tip_detector.py` & `parallax_app-0.37.7/parallax/probe_fine_tip_detector.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/recording_manager.py` & `parallax_app-0.37.7/parallax/recording_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/reticle_detect_manager.py` & `parallax_app-0.37.7/parallax/reticle_detect_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/reticle_detection.py` & `parallax_app-0.37.7/parallax/reticle_detection.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/reticle_detection_coords_interests.py` & `parallax_app-0.37.7/parallax/reticle_detection_coords_interests.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/screen_widget.py` & `parallax_app-0.37.7/parallax/screen_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,14 +165,20 @@
 
     def get_camera_name(self):
         """
         Return the name of the camera.
         """
         return self.camera.name(sn_only=True) if self.camera else None
 
+    def get_camera_color_type(self):
+        """
+        Return the color type of the camera.
+        """
+        return self.camera.get_device_color_type() if self.camera else None
+
     def clear_selected(self):
         """
         Clear the selected target.
         """
         self.click_target.setVisible(False)
         self.cleared.emit()
```

### Comparing `parallax_app-0.37.6/parallax/stage_listener.py` & `parallax_app-0.37.7/parallax/stage_listener.py`

 * *Files 3% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         # Format the current timestamp
         self.timestamp_local = self.get_last_moved_time(millisecond=True)
 
         id = probe["Id"]
         sn = probe["SerialNumber"]
         local_coords_x = round(probe["Stage_X"] * 1000, 1)
         local_coords_y = round(probe["Stage_Y"] * 1000, 1)
-        local_coords_z = round(probe["Stage_Z"] * 1000, 1)
+        local_coords_z = 15000 - round(probe["Stage_Z"] * 1000, 1)
 
         # update into model
         moving_stage = self.model.stages.get(sn)
 
         if moving_stage is not None:
             moving_stage.stage_x = local_coords_x
             moving_stage.stage_y = local_coords_y
@@ -279,15 +279,16 @@
 
         # Update to buffer
         self.append_to_buffer(self.timestamp_local, moving_stage)
 
         # Update into UI
         if self.stage_ui.get_selected_stage_sn() == sn:
             self.stage_ui.updateStageLocalCoords()
-        # logger.debug(sn, moving_stage.stage_x, self.stage_ui.get_selected_stage_sn())
+        else:
+            logger.warning(f"moving_probe: {sn}, selected_probe: {self.stage_ui.get_selected_stage_sn()}")
 
         if sn in self.transM_dict:
             transM = self.transM_dict[sn]
             if transM is not None:
                 self._updateGlobalDataTransformM(sn, moving_stage, transM)
 
     def _updateGlobalDataTransformM(self, sn, moving_stage, transM):
@@ -312,16 +313,15 @@
                 moving_stage.stage_y,
                 moving_stage.stage_z,
                 1,
             ]
         )
         global_point = np.dot(transM, local_point)
         global_point = np.around(global_point[:3], decimals=1)
-        logger.debug(f"_updateGlobalDataTransformM: {sn}, {global_point}")
-
+        
         # Update into UI
         moving_stage.stage_x_global = global_point[0]
         moving_stage.stage_y_global = global_point[1]
         moving_stage.stage_z_global = global_point[2]
         if self.stage_ui.get_selected_stage_sn() == sn:
             self.stage_ui.updateStageGlobalCoords()
 
@@ -334,23 +334,27 @@
         Args:
             sn (str): The serial number of the stage.
             transM (np.ndarray): A 4x4 numpy array representing the transformation matrix for the specified stage.
         """
         self.transM_dict[sn] = transM
         logger.debug(f"requestUpdateGlobalDataTransformM {sn} {transM}")
 
-    def requestClearGlobalDataTransformM(self):
+    def requestClearGlobalDataTransformM(self, sn = None):
         """
         Clears all stored transformation matrices and resets the UI to default global coordinates.
 
         Effects:
             - Clears `transM_dict`, removing all stored transformation matrices.
             - Triggers a UI update to reset the display of global coordinates to default values.
         """
-        self.transM_dict = {}
+        if sn is None: # Not specified, clear all (Use case: reticle Dection is reset)
+            self.transM_dict = {}
+        else:
+            if self.transM_dict.get(sn) is not None:
+                self.transM_dict.pop(sn)
         self.stage_ui.updateStageGlobalCoords_default()
         logger.debug(f"requestClearGlobalDataTransformM {self.transM_dict}")
 
     def _change_time_format(self, str_time):
         """Change the time format from string to datetime."""
         fmt = "%Y%m%d-%H%M%S.%f"
         date_time = datetime.strptime(str_time, fmt)
```

### Comparing `parallax_app-0.37.6/parallax/stage_ui.py` & `parallax_app-0.37.7/parallax/stage_ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 """
 Defines StageUI, a PyQt5 QWidget for showing and updating stage information in the UI, 
 including serial numbers and coordinates. It interacts with the model to reflect 
 real-time data changes.
 """
 
 from PyQt5.QtWidgets import QWidget
-
+from PyQt5.QtCore import pyqtSignal
 
 class StageUI(QWidget):
     """User interface for stage control and display."""
+    prev_curr_stages = pyqtSignal(str, str)
 
     def __init__(self, model, parent=None):
         """Initialize StageUI object"""
         QWidget.__init__(self, parent)
         self.selected_stage = None
         self.model = model
         self.ui = parent
+    
         self.update_stage_selector()
         self.updateStageSN()
         self.updateStageLocalCoords()
         self.updateStageGlobalCoords()
+        self.previous_stage_id = self.get_current_stage_id()
 
         self.ui.stage_selector.currentIndexChanged.connect(self.updateStageSN)
         self.ui.stage_selector.currentIndexChanged.connect(
             self.updateStageLocalCoords
         )
         self.ui.stage_selector.currentIndexChanged.connect(
             self.updateStageGlobalCoords
         )
+        self.ui.stage_selector.currentIndexChanged.connect(self.sendInfoToStageWidget)
 
     def get_selected_stage_sn(self):
         """Get the serial number of the selected stage.
 
         Returns:
             str or None: The serial number of the selected stage, or None if no stage is selected.
         """
@@ -41,47 +45,58 @@
 
     def update_stage_selector(self):
         """Update the stage selector with available stages."""
         self.ui.stage_selector.clear()
         for stage in self.model.stages.keys():
             self.ui.stage_selector.addItem("Probe " + stage, stage)
 
-    def _get_current_stage_id(self):
+    def get_current_stage_id(self):
         """Get the ID of the currently selected stage.
 
         Returns:
             str or None: The ID of the currently selected stage, or None if no stage is selected.
         """
         currentIndex = self.ui.stage_selector.currentIndex()
         stage_id = self.ui.stage_selector.itemData(currentIndex)
         return stage_id
 
+    def update_stage_widget(self, prev_stage_id, curr_stage_id):
+        # signal
+        self.prev_curr_stages.emit(prev_stage_id, curr_stage_id)
+        
+    def sendInfoToStageWidget(self):
+        """Send the selected stage information to the stage widget."""    
+        # Get updated stage_id
+        stage_id = self.get_current_stage_id()
+        self.update_stage_widget(self.previous_stage_id, stage_id)
+        self.previous_stage_id = stage_id
+
     def updateStageSN(self):
         """Update the displayed stage serial number."""
-        stage_id = self._get_current_stage_id()
+        stage_id = self.get_current_stage_id()
         if stage_id:
             self.selected_stage = self.model.stages.get(stage_id)
             if self.selected_stage:
                 self.ui.stage_sn.setText(" " + self.selected_stage.sn)
 
     def updateStageLocalCoords(self):
         """Update the displayed local coordinates of the selected stage."""
-        stage_id = self._get_current_stage_id()
+        stage_id = self.get_current_stage_id()
         if stage_id:
             self.selected_stage = self.model.stages.get(stage_id)
             if self.selected_stage:
                 self.ui.local_coords_x.setText(str(self.selected_stage.stage_x))
                 self.ui.local_coords_y.setText(str(self.selected_stage.stage_y))
                 self.ui.local_coords_z.setText(str(self.selected_stage.stage_z))
 
     def updateStageGlobalCoords(self):
         """Update the displayed global coordinates of the selected stage."""
-        stage_id = self._get_current_stage_id()
+        stage_id = self.get_current_stage_id()
         if stage_id:
-            self.selected_stage = self.model.stages.get(stage_id)
+            self.selected_stage = self.model.get_stage(stage_id)
             if self.selected_stage:
                 if self.selected_stage.stage_x_global is not None \
                 and self.selected_stage.stage_y_global is not None \
                 and self.selected_stage.stage_z_global is not None:
                     self.ui.global_coords_x.setText(
                         str(self.selected_stage.stage_x_global)
                     )
```

### Comparing `parallax_app-0.37.6/parallax/stage_widget.py` & `parallax_app-0.37.7/parallax/stage_widget.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import logging
 import os
 import math
 import time
 
 import numpy as np
-from PyQt5.QtCore import QTimer
+from PyQt5.QtCore import QTimer, Qt
 from PyQt5.QtWidgets import (QLabel, QMessageBox, QPushButton, QSizePolicy,
                              QSpacerItem, QWidget)
 from PyQt5.uic import loadUi
 
 from .calibration_camera import CalibrationStereo
 from .probe_calibration import ProbeCalibration
 from .stage_listener import StageListener
@@ -36,29 +36,29 @@
             ui_dir (str): The directory path where UI files are located.
             screen_widgets (list): A list of ScreenWidget instances for reticle and probe detection.
         """
         super().__init__()
         self.model = model
         self.screen_widgets = screen_widgets
         loadUi(os.path.join(ui_dir, "stage_info.ui"), self)
-        self.setMaximumWidth(380)
+        self.setMaximumWidth(350)
 
         # Load reticle_calib.ui into its placeholder
         self.reticle_calib_widget = QWidget()  # Create a new widget
         loadUi(os.path.join(ui_dir, "reticle_calib.ui"), self.reticle_calib_widget)
         # Assuming reticleCalibPlaceholder is the name of an empty widget designated as a placeholder in your stage_info.ui
         self.stage_status_ui.layout().addWidget(self.reticle_calib_widget)  # Add it to the placeholder's layout
-        self.reticle_calib_widget.setMinimumSize(0, 160)
+        self.reticle_calib_widget.setMinimumSize(0, 120)
 
         # Load probe_calib.ui into its placeholder
         self.probe_calib_widget = QWidget()  # Create a new widget
         loadUi(os.path.join(ui_dir, "probe_calib.ui"), self.probe_calib_widget)
         # Assuming probeCalibPlaceholder is the name of an empty widget designated as a placeholder in your stage_info.ui
         self.stage_status_ui.layout().addWidget(self.probe_calib_widget)  # Add it to the placeholder's layout
-        self.probe_calib_widget.setMinimumSize(0, 450) 
+        self.probe_calib_widget.setMinimumSize(0, 420)
         
         # Create a vertical spacer with expanding policy
         spacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
         # Add the spacer to the layout
         self.stage_status_ui.addItem(spacer)
 
         # Access probe_calibration_btn
@@ -79,14 +79,15 @@
         )
         self.calib_x = self.probe_calib_widget.findChild(QPushButton, "calib_x")
         self.calib_y = self.probe_calib_widget.findChild(QPushButton, "calib_y")
         self.calib_z = self.probe_calib_widget.findChild(QPushButton, "calib_z")
         self.probeCalibrationLabel = self.probe_calib_widget.findChild(
             QLabel, "probeCalibrationLabel"
         )
+        self.probeCalibrationLabel.setTextInteractionFlags(Qt.TextSelectableByMouse)
 
         # Reticle Widget
         self.reticle_detection_status = (
             "default"  # options: default, process, detected, accepted, request_axis
         )
         self.reticle_calibration_btn.clicked.connect(
             self.reticle_detection_button_handler
@@ -105,14 +106,17 @@
             self.reticle_detect_default_status
         )
         self.get_pos_x_from_user_timer = QTimer()
         self.get_pos_x_from_user_timer.timeout.connect(self.check_positive_x_axis)
 
         # Stage widget
         self.stageUI = StageUI(self.model, self)
+        self.stageUI.prev_curr_stages.connect(self.update_stages)
+        self.selected_stage_id = self.stageUI.get_current_stage_id()
+
         self.probe_calibration_btn.setEnabled(False)
         self.probe_calibration_btn.clicked.connect(
             self.probe_detection_button_handler
         )
         # Start refreshing stage info
         self.stageListener = StageListener(self.model, self.stageUI)
         self.stageListener.start()
@@ -126,28 +130,33 @@
         self.probeCalibration.calib_complete_z.connect(self.calib_z_complete)
         self.probeCalibration.calib_complete.connect(
             self.probe_detect_accepted_status
         )
         self.probeCalibration.transM_info.connect(
             self.update_probe_calib_status
         )
+        self.probe_detection_status = "default"    # options: default, process, accepted
         self.calib_status_x, self.calib_status_y, self.calib_status_z = False, False, False
-        self.probe_detection_status = None    # options: default, process, x_y_z_detected, accepted
+        self.transM, self.L2_err, self.dist_travled = None, None, None
+        self.moving_stage_id = None
 
+        # Set current filter
         self.filter = "no_filter"
         logger.debug(f"filter: {self.filter}")
 
     def reticle_detection_button_handler(self):
         """
         Handles clicks on the reticle detection button, initiating or canceling reticle detection.
         """
         logger.debug(f"\n reticle_detection_button_handler {self.reticle_detection_status}")
         if self.reticle_calibration_btn.isChecked():
             # Run reticle detectoin
             self.reticle_detect_process_status()
+            # Init probe calibration property 
+            # self.probeCalibration.reset_calib(sn = self.selected_stage_id)
         else:
             if self.reticle_detection_status == "accepted":
                 response = self.reticle_overwrite_popup_window()
                 if response:
                     # Overwrite the result
                     self.reticle_detect_default_status()
                 else:
@@ -193,14 +202,16 @@
             }
         """)
         self.reticle_detection_status = "default"
         self.reticleCalibrationLabel.setText("")
         if self.probe_calibration_btn.isEnabled():
             # Disable probe calibration
             self.probe_detect_default_status()
+        self.model.reset_stage_calib_info()
+        self.probeCalibration.clear()
 
     def reticle_overwrite_popup_window(self):
         """
         Displays a confirmation dialog to decide whether to overwrite the current reticle position.
 
         Returns:
             bool: True if the user chooses to overwrite, False otherwise.
@@ -259,15 +270,17 @@
         self.model.reset_coords_intrinsic_extrinsic()
 
         for screen in self.screen_widgets:
             screen.reset_reticle_coords()
             screen.reticle_coords_detected.connect(
                 self.reticle_detect_two_screens
             )
-            screen.run_reticle_detection()
+            #TODO implement camera calib for mono camera
+            if screen.get_camera_color_type() == "Color": 
+                screen.run_reticle_detection()
         self.filter = "reticle_detection"
         logger.debug(f"filter: {self.filter}")
 
         # Hide Accept and Reject Button
         self.acceptButton.hide()
         self.rejectButton.hide()
 
@@ -635,199 +648,232 @@
     def probe_detection_button_handler(self):
         """Handle the probe detection button click."""
         if self.probe_calibration_btn.isChecked():
             self.probe_detect_process_status()
         else:
             response = self.probe_overwrite_popup_window()
             if response:
-                self.probe_detect_default_status()
+                self.probe_detect_default_status(sn = self.selected_stage_id)
             else:
                 # Keep the last calibration result
                 self.probe_calibration_btn.setChecked(True)
 
-    def probe_detect_default_status(self):
-        """
-        Resets the probe detection status to its default state and updates the UI to reflect this change.
-        This method is called after completing or aborting the probe detection process.
-        """
-        self.probe_detection_status = "default"
+    def probe_detect_default_status_ui(self, sn = None):
         self.probe_calibration_btn.setStyleSheet("""
             QPushButton {
                 color: white;
                 background-color: black;
             }
             QPushButton:hover {
                 background-color: #641e1e;
             }
         """)
         self.hide_x_y_z()
+    
         self.probeCalibrationLabel.setText("")
-        self.probeCalibration.reset_calib()
-        # self.reset_calib_status()
-
         self.probe_calibration_btn.setChecked(False)
         if self.reticle_detection_status == "default":
             self.probe_calibration_btn.setEnabled(False)
 
         if self.filter == "probe_detection":
             for screen in self.screen_widgets:
                 camera_name = screen.get_camera_name()
                 if camera_name == self.camA_best or camera_name == self.camB_best:
-                    print(f"Disconnect probe_detection: {camera_name}")
+                    logger.debug(f"Disconnect probe_detection: {camera_name}")
                     screen.probe_coords_detected.disconnect(
                         self.probe_detect_two_screens
                     )
                     screen.run_no_filter()
  
             self.filter = "no_filter"
             logger.debug(f"filter: {self.filter}")
-            self.probeCalibration.clear()
+            self.probeCalibration.clear(self.selected_stage_id)
 
-        # update global coords
-        self.stageListener.requestClearGlobalDataTransformM()
+        # update global coords. Set  to '-' on UI
+        self.stageListener.requestClearGlobalDataTransformM(sn = sn)  # TODO
+
+    def probe_detect_default_status(self, sn = None):
+        """
+        Resets the probe detection status to its default state and updates the UI to reflect this change.
+        This method is called after completing or aborting the probe detection process.
+        """
+        self.probe_detection_status = "default"
+        self.calib_status_x, self.calib_status_y, self.calib_status_z = False, False, False
+        self.transM, self.L2_err, self.dist_travled = None, None, None
+        self.probeCalibration.reset_calib(sn = sn)
+        self.probe_detect_default_status_ui(sn = sn)
 
     def probe_detect_process_status(self):
         """
         Updates the UI and internal state to reflect that the probe detection process is underway.
         """
-        self.probe_detection_status = "                                                                                                                                         "
+        if self.probe_detection_status == "process":
+            return
+        
+        self.probe_detection_status = "process"
         self.probe_calibration_btn.setStyleSheet(
             "color: white;"
             "background-color: #bc9e44;"
         )
+        if not self.probe_calibration_btn.isChecked():
+            self.probe_calibration_btn.setChecked(True)
+        
         self.calib_x.show()
         self.calib_y.show()
         self.calib_z.show()
 
         # Connect with only reticle detected screens
         for screen in self.screen_widgets:
             camera_name = screen.get_camera_name()
             if camera_name == self.camA_best or camera_name == self.camB_best:
-                print(f"Connect probe_detection: {camera_name}")
+                logger.debug(f"Connect `probe_detection`: {camera_name}")
                 screen.probe_coords_detected.connect(self.probe_detect_two_screens)
                 screen.run_probe_detection()
             else:
                 screen.run_no_filter()
         self.filter = "probe_detection"
         logger.debug(f"filter: {self.filter}")
 
         # message
         message = f"Move probe at least 2mm along X, Y, and Z axes"
         QMessageBox.information(self, "Probe calibration info", message)
 
-    def probe_detect_accepted_status(self, stage_sn, transformation_matrix):
+    def probe_detect_accepted_status(self, stage_sn, transformation_matrix, switch_probe = False):
         """
         Finalizes the probe detection process, accepting the detected probe position and updating the UI accordingly.
         Additionally, it updates the model with the transformation matrix obtained from the calibration.
 
         Parameters:
             stage_sn (str): The serial number of the stage for which the probe position is accepted.
             transformation_matrix (np.ndarray): The transformation matrix obtained from the probe calibration process.
         """
+        if self.probe_detection_status == "accepted":
+            return
+        if not switch_probe and self.moving_stage_id != self.selected_stage_id:
+            return
+
         self.probe_detection_status = "accepted"
         self.probe_calibration_btn.setStyleSheet(
             "color: white;"
             "background-color: #84c083;"
         )
+        if not self.probe_calibration_btn.isChecked():
+            self.probe_calibration_btn.setChecked(True)
+
         self.hide_x_y_z()
         if self.filter == "probe_detection":
             for screen in self.screen_widgets:
                 camera_name = screen.get_camera_name()
                 if camera_name == self.camA_best or camera_name == self.camB_best:
-                    print(f"Disconnect probe_detection: {camera_name}")
+                    logger.debug(f"Disconnect probe_detection: {camera_name}")
                     screen.probe_coords_detected.disconnect(
                         self.probe_detect_two_screens
                     )
                     screen.run_no_filter()
 
             self.filter = "no_filter"
             logger.debug(f"filter: {self.filter}")
 
         # update global coords
         self.stageListener.requestUpdateGlobalDataTransformM(
             stage_sn, transformation_matrix
         )
 
+    def set_default_x_y_z_style(self):
+        self.calib_x.setStyleSheet(
+            "color: white;"
+            "background-color: black;"
+        )
+        self.calib_y.setStyleSheet(
+            "color: white;"
+            "background-color: black;"
+        )
+
+        self.calib_z.setStyleSheet(
+            "color: white;"
+            "background-color: black;"
+        )
+
     def hide_x_y_z(self):
         """
         Hides the X, Y, and Z calibration buttons and updates their styles to indicate that the calibration for
         each axis has been completed.
         """
         if self.calib_x.isVisible():
             self.calib_x.hide()
-            # Change the button to green.
-            self.calib_x.setStyleSheet(
-            "color: white;"
-            "background-color: black;"
-        )
+            
         if self.calib_y.isVisible():
             self.calib_y.hide()
-            # Change the button to green.
-            self.calib_y.setStyleSheet(
-            "color: white;"
-            "background-color: black;"
-        )
+             
         if self.calib_z.isVisible():
             self.calib_z.hide()
-            # Change the button to green.
-            self.calib_z.setStyleSheet(
-            "color: white;"
-            "background-color: black;"
-        )
+            
+        self.set_default_x_y_z_style()
 
-    def calib_x_complete(self):
+    def calib_x_complete(self, switch_probe = False):
         """
         Updates the UI to indicate that the calibration for the X-axis is complete.
         """
+        if not switch_probe and self.moving_stage_id != self.selected_stage_id:
+            return
+
         if self.calib_x.isVisible():
             # Change the button to green.
             self.calib_x.setStyleSheet(
             "color: white;"
             "background-color: #84c083;"
         )
+        self.calib_status_x = True
     
-    def calib_y_complete(self):
+    def calib_y_complete(self, switch_probe = False):
         """
         Updates the UI to indicate that the calibration for the Y-axis is complete.
         """
+        if not switch_probe and self.moving_stage_id != self.selected_stage_id:
+            return
+
         if self.calib_y.isVisible():
             # Change the button to green.
             self.calib_y.setStyleSheet(
             "color: white;"
             "background-color: #84c083;"
         )
+        self.calib_status_y = True
 
-
-    def calib_z_complete(self):
+    def calib_z_complete(self, switch_probe = False):
         """
         Updates the UI to indicate that the calibration for the Z-axis is complete.
         """
+        if not switch_probe and self.moving_stage_id != self.selected_stage_id:
+            return
+
         if self.calib_z.isVisible():
             # Change the button to green.
             self.calib_z.setStyleSheet(
             "color: white;"
             "background-color: #84c083;"
         )
+        self.calib_status_z = True
 
     def update_probe_calib_status_transM(self, transformation_matrix):
         # Extract the rotation matrix (top-left 3x3)
         R = transformation_matrix[:3, :3]
         # Extract the translation vector (top 3 elements of the last column)
         T = transformation_matrix[:3, 3]
 
         # Set the formatted string as the label's text
         content = (
             f"<span style='color:yellow;'><small>"
             f"[Transformation Matrix]<br></small></span>"
             f"<span style='color:green;'><small><b>R:</b><br>"
-            f" {R[0][0]:.5f}, {R[0][1]:.5f}, {R[0][2]:.5f},<br>"
-            f" {R[1][0]:.5f}, {R[1][1]:.5f}, {R[1][2]:.5f},<br>"
-            f" {R[2][0]:.5f}, {R[2][1]:.5f}, {R[2][2]:.5f},<br>"
-            f"<b>T:</b><br>"
-            f" {T[0]:.0f}, {T[1]:.0f}, {T[2]:.0f}<br>"
+            f" [[{R[0][0]:.5f}, {R[0][1]:.5f}, {R[0][2]:.5f}],<br>"
+            f" [{R[1][0]:.5f}, {R[1][1]:.5f}, {R[1][2]:.5f}],<br>"
+            f" [{R[2][0]:.5f}, {R[2][1]:.5f}, {R[2][2]:.5f}]]<br>"
+            f"<b>T: </b>"
+            f" [{T[0]:.1f}, {T[1]:.1f}, {T[2]:.1f}]<br>"
             f"</small></span>"
         )
         return content
 
     def update_probe_calib_status_L2(self, L2_err):
         content = (
             f"<span style='color:yellow;'><small>[L2 distance]<br></small></span>"
@@ -837,20 +883,98 @@
         return content
 
     def update_probe_calib_status_distance_traveled(self, dist_traveled):
         x, y, z = dist_traveled[0], dist_traveled[1], dist_traveled[2]
         content = (
             f"<span style='color:yellow;'><small>[Distance traveled (µm)]<br></small></span>"
             f"<span style='color:green;'><small>"
-            f"x: {x} y: {y} z: {z}<br>"
+            f"x: {int(x)} y: {int(y)} z: {int(z)}<br>"
             f"</small></span>"
         )
         return content
 
-    def update_probe_calib_status(self, transformation_matrix, L2_err, dist_traveled):
-        content_transM = self.update_probe_calib_status_transM(transformation_matrix)
+    def display_probe_calib_status(self, transM, L2_err, dist_traveled):
+        content_transM = self.update_probe_calib_status_transM(transM)
         content_L2 = self.update_probe_calib_status_L2(L2_err)
         content_L2_travel = self.update_probe_calib_status_distance_traveled(dist_traveled)
-        # Ensure HTML content is properly combined
+        # Display the transformation matrix, L2 error, and distance traveled
         full_content = content_transM + content_L2 + content_L2_travel
-
         self.probeCalibrationLabel.setText(full_content)
+
+    def update_probe_calib_status(self, moving_stage_id, transM, L2_err, dist_traveled):
+        self.transM, self.L2_err, self.dist_travled = transM, L2_err, dist_traveled
+        self.moving_stage_id = moving_stage_id
+
+        if self.moving_stage_id == self.selected_stage_id:
+            # If moving stage is the selected stage, update the probe calibration status on UI
+            self.display_probe_calib_status(transM, L2_err, dist_traveled)
+        else:
+            # If moving stage is not the selected stage, save the calibration info
+            content = (
+                f"<span style='color:yellow;'><small>Moving probe not selected.<br></small></span>"
+            )
+            self.probeCalibrationLabel.setText(content)
+
+    def get_stage_info(self):
+        info = {}
+        info['detection_status'] = self.probe_detection_status
+        info['transM'] = self.transM
+        info['L2_err'] = self.L2_err
+        info['dist_traveled'] = self.dist_travled
+        info['status_x'] = self.calib_status_x
+        info['status_y'] = self.calib_status_y
+        info['status_z'] = self.calib_status_z
+        return info
+
+    def update_stage_info(self, info):
+        #self.probe_detection_status = info['detection_status']
+        self.transM = info['transM']
+        self.L2_err = info['L2_err']
+        self.dist_travled = info['dist_traveled']
+        self.calib_status_x = info['status_x']
+        self.calib_status_y = info['status_y']
+        self.calib_status_z = info['status_z']
+
+    def update_stages(self, prev_stage_id, curr_stage_id):
+        logger.debug(f"update_stages, prev:{prev_stage_id}, curr:{curr_stage_id}")
+        self.selected_stage_id = curr_stage_id
+        if prev_stage_id is None or curr_stage_id is None:
+            return
+
+        # Save the previous stage's calibration info
+        #if self.moving_stage_id == prev_stage_id: # TODO
+        info = self.get_stage_info()
+        self.model.add_stage_calib_info(prev_stage_id, info)
+        logger.debug(f"Saved stage {prev_stage_id} info: {info}")
+
+        # Load the current stage's calibration info
+        info = self.model.get_stage_calib_info(curr_stage_id)
+        logger.debug(f"Loaded stage {curr_stage_id} info: {info}")
+        if info is not None:
+            self.update_stage_info(info)
+            probe_detection_status = info['detection_status']
+        else:
+            probe_detection_status = "default"
+
+        # Go to the appropriate status based on the info
+        if probe_detection_status == "default":
+            self.probe_detect_default_status(sn = self.selected_stage_id)  # Reset the probe detection status
+        elif probe_detection_status == "process":
+            self.probe_detect_process_status()
+            # Update calib status of x, y, z, calib status info
+            self.set_default_x_y_z_style()
+            if self.calib_status_x:
+                self.calib_x_complete(switch_probe = True)
+            if self.calib_status_y:
+                self.calib_y_complete(switch_probe = True)
+            if self.calib_status_z:
+                self.calib_z_complete(switch_probe = True)
+            if self.transM is not None:
+                self.display_probe_calib_status(self.transM, self.L2_err, self.dist_travled)
+            else:
+                self.probeCalibrationLabel.setText("")
+        elif probe_detection_status == "accepted":
+            self.probe_detect_accepted_status(curr_stage_id, self.transM, switch_probe = True)
+            if self.transM is not None:
+                self.display_probe_calib_status(self.transM, self.L2_err, self.dist_travled)
+
+        self.probe_detection_status = probe_detection_status
```

### Comparing `parallax_app-0.37.6/parallax/user_setting_manager.py` & `parallax_app-0.37.7/parallax/user_setting_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax/utils.py` & `parallax_app-0.37.7/parallax/utils.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/parallax_app.egg-info/PKG-INFO` & `parallax_app-0.37.7/parallax_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallax-app
-Version: 0.37.6
+Version: 0.37.7
 Summary: GUI software for photogrammetry-assisted probe targeting in electrophysiology
 Author-email: Hanna Lee <hanna.lee@alleninstitute.org>
 License: MIT
 Keywords: parallax
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
@@ -36,18 +36,19 @@
 
 # Parallax
 
 ![Parallax](ui/ParallaxReadME.JPG)
 
 Parallax is a graphical user interface designed to streamline the process of setting up and performing acute *in vivo* electrophysiology experiments.
 
-User documentation available on [here](https://parallax.readthedocs.io/en/latest/).
+User documentation available on [here](https://parallax.readthedocs.io/en/stable/).
 
 ### Prerequisites
 - **Python~=3.8** (Recommended to install via [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html))
+  -  Python 3.8 is required for the Spinnaker library.
 - PySpin (for Linux or Mac OS users)
 
 
 ### Installation
 1. Create virtual environment using **Python version 3.8** and activate it:
 - On Windows:
 ```bash
```

### Comparing `parallax_app-0.37.6/parallax_app.egg-info/SOURCES.txt` & `parallax_app-0.37.7/parallax_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/pyproject.toml` & `parallax_app-0.37.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/tests/test_screen_widget.py` & `parallax_app-0.37.7/tests/test_screen_widget.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/ParallaxReadME.JPG` & `parallax_app-0.37.7/ui/ParallaxReadME.JPG`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/font/FiraCode-VariableFont_wght.ttf` & `parallax_app-0.37.7/ui/font/FiraCode-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/mainWindow.ui` & `parallax_app-0.37.7/ui/mainWindow.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/probe_calib.ui` & `parallax_app-0.37.7/ui/probe_calib.ui`

 * *Files 15% similar despite different names*

#### Comparing `parallax_app-0.37.6/ui/probe_calib.ui` & `parallax_app-0.37.7/ui/probe_calib.ui`

```diff
@@ -14,157 +14,157 @@
       <string>Form</string>
     </property>
     <widget class="QWidget" name="gridLayoutWidget">
       <property name="geometry">
         <rect>
           <x>10</x>
           <y>10</y>
-          <width>361</width>
-          <height>694</height>
+          <width>286</width>
+          <height>705</height>
         </rect>
       </property>
       <layout class="QGridLayout" name="gridLayout">
         <property name="verticalSpacing">
           <number>1</number>
         </property>
-        <item row="1" column="4">
+        <item row="2" column="4">
           <spacer name="horizontalSpacer_2">
             <property name="orientation">
               <enum>Qt::Horizontal</enum>
             </property>
             <property name="sizeHint" stdset="0">
               <size>
                 <width>40</width>
                 <height>20</height>
               </size>
             </property>
           </spacer>
         </item>
-        <item row="0" column="0" colspan="5" alignment="Qt::AlignHCenter|Qt::AlignTop">
+        <item row="2" column="0">
+          <spacer name="horizontalSpacer">
+            <property name="orientation">
+              <enum>Qt::Horizontal</enum>
+            </property>
+            <property name="sizeHint" stdset="0">
+              <size>
+                <width>40</width>
+                <height>20</height>
+              </size>
+            </property>
+          </spacer>
+        </item>
+        <item row="1" column="0" colspan="5">
           <widget class="QPushButton" name="probe_calibration_btn">
             <property name="sizePolicy">
               <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
             </property>
             <property name="minimumSize">
               <size>
-                <width>330</width>
-                <height>50</height>
+                <width>200</width>
+                <height>40</height>
               </size>
             </property>
             <property name="maximumSize">
               <size>
-                <width>350</width>
-                <height>16777215</height>
+                <width>300</width>
+                <height>40</height>
               </size>
             </property>
             <property name="text">
               <string>Probe Calibration</string>
             </property>
             <property name="checkable">
               <bool>true</bool>
             </property>
           </widget>
         </item>
-        <item row="1" column="0">
-          <spacer name="horizontalSpacer">
-            <property name="orientation">
-              <enum>Qt::Horizontal</enum>
-            </property>
-            <property name="sizeHint" stdset="0">
-              <size>
-                <width>40</width>
-                <height>20</height>
-              </size>
-            </property>
-          </spacer>
-        </item>
-        <item row="1" column="1" alignment="Qt::AlignTop">
+        <item row="2" column="1">
           <widget class="QPushButton" name="calib_x">
             <property name="enabled">
               <bool>false</bool>
             </property>
             <property name="minimumSize">
               <size>
                 <width>0</width>
-                <height>40</height>
+                <height>30</height>
               </size>
             </property>
             <property name="maximumSize">
               <size>
                 <width>30</width>
-                <height>16777215</height>
+                <height>30</height>
               </size>
             </property>
             <property name="text">
               <string>X</string>
             </property>
           </widget>
         </item>
-        <item row="1" column="2" alignment="Qt::AlignTop">
+        <item row="4" column="0" rowspan="2" colspan="5">
+          <widget class="QLabel" name="probeCalibrationLabel">
+            <property name="minimumSize">
+              <size>
+                <width>0</width>
+                <height>600</height>
+              </size>
+            </property>
+            <property name="text">
+              <string/>
+            </property>
+            <property name="alignment">
+              <set>Qt::AlignLeading|Qt::AlignLeft|Qt::AlignTop</set>
+            </property>
+          </widget>
+        </item>
+        <item row="2" column="2">
           <widget class="QPushButton" name="calib_y">
             <property name="enabled">
               <bool>false</bool>
             </property>
             <property name="minimumSize">
               <size>
                 <width>0</width>
-                <height>40</height>
+                <height>30</height>
               </size>
             </property>
             <property name="maximumSize">
               <size>
                 <width>30</width>
-                <height>16777215</height>
+                <height>30</height>
               </size>
             </property>
             <property name="text">
               <string>Y</string>
             </property>
           </widget>
         </item>
-        <item row="1" column="3" alignment="Qt::AlignTop">
+        <item row="2" column="3">
           <widget class="QPushButton" name="calib_z">
             <property name="enabled">
               <bool>false</bool>
             </property>
             <property name="minimumSize">
               <size>
                 <width>0</width>
-                <height>40</height>
+                <height>30</height>
               </size>
             </property>
             <property name="maximumSize">
               <size>
                 <width>30</width>
-                <height>16777215</height>
+                <height>30</height>
               </size>
             </property>
             <property name="text">
               <string>Z</string>
             </property>
           </widget>
         </item>
-        <item row="2" column="0" colspan="5">
-          <widget class="QLabel" name="probeCalibrationLabel">
-            <property name="minimumSize">
-              <size>
-                <width>0</width>
-                <height>600</height>
-              </size>
-            </property>
-            <property name="text">
-              <string/>
-            </property>
-            <property name="alignment">
-              <set>Qt::AlignLeading|Qt::AlignLeft|Qt::AlignTop</set>
-            </property>
-          </widget>
-        </item>
       </layout>
     </widget>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `parallax_app-0.37.6/ui/resources/arrow-right.png` & `parallax_app-0.37.7/ui/resources/arrow-right.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/resources/check.png` & `parallax_app-0.37.7/ui/resources/check.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/resources/gear.png` & `parallax_app-0.37.7/ui/resources/gear.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/resources/recordingButton.png` & `parallax_app-0.37.7/ui/resources/recordingButton.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/resources/recordingButton_disabled.png` & `parallax_app-0.37.7/ui/resources/recordingButton_disabled.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/resources/sextant.png` & `parallax_app-0.37.7/ui/resources/sextant.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/resources/snapshotButton_disabled.png` & `parallax_app-0.37.7/ui/resources/snapshotButton_disabled.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/resources/snapshotButton_green.png` & `parallax_app-0.37.7/ui/resources/snapshotButton_green.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/resources/snapshotButton_white.png` & `parallax_app-0.37.7/ui/resources/snapshotButton_white.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/resources/stop-sign.png` & `parallax_app-0.37.7/ui/resources/stop-sign.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/resources/target.png` & `parallax_app-0.37.7/ui/resources/target.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/reticle_calib.ui` & `parallax_app-0.37.7/ui/reticle_calib.ui`

 * *Files 8% similar despite different names*

#### Comparing `parallax_app-0.37.6/ui/reticle_calib.ui` & `parallax_app-0.37.7/ui/reticle_calib.ui`

```diff
@@ -18,135 +18,144 @@
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <widget class="QWidget" name="gridLayoutWidget">
       <property name="geometry">
         <rect>
-          <x>30</x>
+          <x>10</x>
           <y>10</y>
-          <width>332</width>
-          <height>494</height>
+          <width>289</width>
+          <height>502</height>
         </rect>
       </property>
       <layout class="QGridLayout" name="gridLayout">
+        <property name="horizontalSpacing">
+          <number>4</number>
+        </property>
         <property name="verticalSpacing">
-          <number>1</number>
+          <number>0</number>
         </property>
-        <item row="1" column="1" alignment="Qt::AlignVCenter">
+        <item row="2" column="0" colspan="4">
+          <widget class="QLabel" name="reticleCalibResultLabel">
+            <property name="minimumSize">
+              <size>
+                <width>0</width>
+                <height>400</height>
+              </size>
+            </property>
+            <property name="text">
+              <string/>
+            </property>
+            <property name="alignment">
+              <set>Qt::AlignHCenter|Qt::AlignTop</set>
+            </property>
+          </widget>
+        </item>
+        <item row="1" column="3">
+          <spacer name="horizontalSpacer_2">
+            <property name="orientation">
+              <enum>Qt::Horizontal</enum>
+            </property>
+            <property name="sizeHint" stdset="0">
+              <size>
+                <width>20</width>
+                <height>10</height>
+              </size>
+            </property>
+          </spacer>
+        </item>
+        <item row="1" column="1">
           <widget class="QPushButton" name="acceptButton">
             <property name="minimumSize">
               <size>
                 <width>0</width>
-                <height>40</height>
+                <height>30</height>
+              </size>
+            </property>
+            <property name="maximumSize">
+              <size>
+                <width>125</width>
+                <height>30</height>
               </size>
             </property>
             <property name="text">
               <string>Accept</string>
             </property>
             <property name="icon">
               <iconset>
                 <normalon>resources/check.png</normalon>
               </iconset>
             </property>
           </widget>
         </item>
-        <item row="1" column="3">
-          <spacer name="horizontalSpacer_2">
+        <item row="1" column="0">
+          <spacer name="horizontalSpacer_4">
             <property name="orientation">
               <enum>Qt::Horizontal</enum>
             </property>
             <property name="sizeHint" stdset="0">
               <size>
-                <width>40</width>
-                <height>20</height>
+                <width>20</width>
+                <height>10</height>
               </size>
             </property>
           </spacer>
         </item>
         <item row="1" column="2" alignment="Qt::AlignVCenter">
           <widget class="QPushButton" name="rejectButton">
             <property name="minimumSize">
               <size>
                 <width>0</width>
-                <height>40</height>
+                <height>30</height>
               </size>
             </property>
             <property name="maximumSize">
               <size>
-                <width>16777215</width>
-                <height>50</height>
+                <width>125</width>
+                <height>30</height>
               </size>
             </property>
             <property name="text">
               <string>Reject</string>
             </property>
             <property name="icon">
               <iconset>
                 <normalon>resources/x.png</normalon>
               </iconset>
             </property>
           </widget>
         </item>
-        <item row="0" column="0" colspan="4" alignment="Qt::AlignHCenter|Qt::AlignTop">
+        <item row="0" column="0" colspan="4">
           <widget class="QPushButton" name="reticle_calibration_btn">
             <property name="sizePolicy">
               <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
             </property>
             <property name="minimumSize">
               <size>
-                <width>330</width>
-                <height>50</height>
+                <width>200</width>
+                <height>40</height>
               </size>
             </property>
             <property name="maximumSize">
               <size>
-                <width>350</width>
-                <height>16777215</height>
+                <width>300</width>
+                <height>40</height>
               </size>
             </property>
             <property name="text">
               <string>Reticle Detection</string>
             </property>
             <property name="checkable">
               <bool>true</bool>
             </property>
           </widget>
         </item>
-        <item row="1" column="0">
-          <spacer name="horizontalSpacer_4">
-            <property name="orientation">
-              <enum>Qt::Horizontal</enum>
-            </property>
-            <property name="sizeHint" stdset="0">
-              <size>
-                <width>40</width>
-                <height>20</height>
-              </size>
-            </property>
-          </spacer>
-        </item>
-        <item row="2" column="0" colspan="4">
-          <widget class="QLabel" name="reticleCalibResultLabel">
-            <property name="minimumSize">
-              <size>
-                <width>0</width>
-                <height>400</height>
-              </size>
-            </property>
-            <property name="text">
-              <string/>
-            </property>
-            <property name="alignment">
-              <set>Qt::AlignHCenter|Qt::AlignTop</set>
-            </property>
-          </widget>
-        </item>
       </layout>
     </widget>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `parallax_app-0.37.6/ui/settingPopUpMenu.ui` & `parallax_app-0.37.7/ui/settingPopUpMenu.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.6/ui/stage_info.ui` & `parallax_app-0.37.7/ui/stage_info.ui`

 * *Files 2% similar despite different names*

#### Comparing `parallax_app-0.37.6/ui/stage_info.ui` & `parallax_app-0.37.7/ui/stage_info.ui`

```diff
@@ -2,16 +2,16 @@
 <ui version="4.0">
   <class>Form</class>
   <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>525</width>
-        <height>754</height>
+        <width>266</width>
+        <height>338</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
       <item row="0" column="0">
@@ -41,323 +41,346 @@
               </property>
               <property name="horizontalSpacing">
                 <number>1</number>
               </property>
               <property name="verticalSpacing">
                 <number>2</number>
               </property>
-              <item row="2" column="2">
-                <widget class="QPushButton" name="pushButton">
-                  <property name="maximumSize">
-                    <size>
-                      <width>40</width>
-                      <height>39</height>
-                    </size>
-                  </property>
-                  <property name="styleSheet">
-                    <string notr="true">background-color : yellow</string>
-                  </property>
-                  <property name="text">
-                    <string/>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="0" colspan="2">
-                <widget class="QLabel" name="stage_sn">
+              <item row="5" column="0">
+                <widget class="QLabel" name="label_11">
                   <property name="minimumSize">
                     <size>
                       <width>0</width>
-                      <height>50</height>
+                      <height>25</height>
                     </size>
                   </property>
                   <property name="maximumSize">
                     <size>
                       <width>16777215</width>
-                      <height>70</height>
+                      <height>25</height>
                     </size>
                   </property>
                   <property name="text">
-                    <string>SN</string>
+                    <string>Z:</string>
                   </property>
                 </widget>
               </item>
-              <item row="0" column="0" colspan="3">
-                <widget class="QLabel" name="label">
+              <item row="3" column="2">
+                <widget class="QLabel" name="label_13">
                   <property name="minimumSize">
                     <size>
-                      <width>0</width>
-                      <height>30</height>
+                      <width>50</width>
+                      <height>0</height>
                     </size>
                   </property>
                   <property name="maximumSize">
                     <size>
-                      <width>16777215</width>
-                      <height>30</height>
+                      <width>50</width>
+                      <height>16777215</height>
                     </size>
                   </property>
                   <property name="text">
-                    <string/>
+                    <string>μm</string>
                   </property>
                 </widget>
               </item>
-              <item row="7" column="0" colspan="3">
-                <widget class="QLabel" name="label_3">
+              <item row="5" column="2">
+                <widget class="QLabel" name="label_15">
                   <property name="maximumSize">
                     <size>
-                      <width>150</width>
-                      <height>30</height>
+                      <width>40</width>
+                      <height>16777215</height>
                     </size>
                   </property>
                   <property name="text">
-                    <string/>
+                    <string>μm</string>
                   </property>
                 </widget>
               </item>
-              <item row="4" column="1" alignment="Qt::AlignRight">
+              <item row="9" column="2">
+                <widget class="QLabel" name="label_17">
+                  <property name="text">
+                    <string>μm</string>
+                  </property>
+                </widget>
+              </item>
+              <item row="5" column="1" alignment="Qt::AlignRight">
+                <widget class="QLabel" name="local_coords_z">
+                  <property name="text">
+                    <string>-</string>
+                  </property>
+                </widget>
+              </item>
+              <item row="3" column="1" alignment="Qt::AlignRight">
                 <widget class="QLabel" name="local_coords_x">
                   <property name="maximumSize">
                     <size>
                       <width>16777215</width>
                       <height>16777215</height>
                     </size>
                   </property>
                   <property name="text">
                     <string>-</string>
                   </property>
                 </widget>
               </item>
-              <item row="11" column="2">
-                <widget class="QLabel" name="label_18">
+              <item row="11" column="0" colspan="3">
+                <widget class="QLabel" name="label_4">
+                  <property name="maximumSize">
+                    <size>
+                      <width>16777215</width>
+                      <height>5</height>
+                    </size>
+                  </property>
                   <property name="text">
-                    <string>μm</string>
+                    <string/>
                   </property>
                 </widget>
               </item>
-              <item row="3" column="0" colspan="3">
-                <widget class="QLabel" name="local_coords">
+              <item row="8" column="0">
+                <widget class="QLabel" name="label_5">
                   <property name="minimumSize">
                     <size>
                       <width>0</width>
-                      <height>70</height>
+                      <height>25</height>
                     </size>
                   </property>
                   <property name="maximumSize">
                     <size>
                       <width>16777215</width>
-                      <height>70</height>
+                      <height>25</height>
                     </size>
                   </property>
                   <property name="text">
-                    <string>Local coords</string>
+                    <string>X:</string>
                   </property>
                 </widget>
               </item>
-              <item row="4" column="0">
-                <widget class="QLabel" name="label_2">
+              <item row="1" column="2">
+                <widget class="QPushButton" name="pushButton">
                   <property name="maximumSize">
                     <size>
-                      <width>16777215</width>
-                      <height>50</height>
+                      <width>25</width>
+                      <height>25</height>
                     </size>
                   </property>
+                  <property name="styleSheet">
+                    <string notr="true">background-color : yellow</string>
+                  </property>
                   <property name="text">
-                    <string>X:</string>
+                    <string/>
                   </property>
                 </widget>
               </item>
-              <item row="9" column="2">
-                <widget class="QLabel" name="label_16">
+              <item row="10" column="2">
+                <widget class="QLabel" name="label_18">
                   <property name="text">
                     <string>μm</string>
                   </property>
                 </widget>
               </item>
-              <item row="6" column="0">
-                <widget class="QLabel" name="label_11">
+              <item row="10" column="0">
+                <widget class="QLabel" name="label_7">
+                  <property name="minimumSize">
+                    <size>
+                      <width>0</width>
+                      <height>25</height>
+                    </size>
+                  </property>
                   <property name="maximumSize">
                     <size>
                       <width>16777215</width>
-                      <height>50</height>
+                      <height>25</height>
                     </size>
                   </property>
                   <property name="text">
                     <string>Z:</string>
                   </property>
                 </widget>
               </item>
-              <item row="11" column="0">
-                <widget class="QLabel" name="label_7">
+              <item row="10" column="1" alignment="Qt::AlignRight">
+                <widget class="QLabel" name="global_coords_z">
+                  <property name="text">
+                    <string>-</string>
+                  </property>
+                </widget>
+              </item>
+              <item row="7" column="0" colspan="3">
+                <widget class="QLabel" name="global_coords">
+                  <property name="minimumSize">
+                    <size>
+                      <width>0</width>
+                      <height>30</height>
+                    </size>
+                  </property>
                   <property name="maximumSize">
                     <size>
                       <width>16777215</width>
-                      <height>50</height>
+                      <height>30</height>
                     </size>
                   </property>
                   <property name="text">
-                    <string>Z:</string>
+                    <string>Global coords</string>
                   </property>
                 </widget>
               </item>
-              <item row="9" column="0">
-                <widget class="QLabel" name="label_5">
+              <item row="3" column="0">
+                <widget class="QLabel" name="label_2">
+                  <property name="minimumSize">
+                    <size>
+                      <width>0</width>
+                      <height>25</height>
+                    </size>
+                  </property>
                   <property name="maximumSize">
                     <size>
                       <width>16777215</width>
-                      <height>50</height>
+                      <height>25</height>
                     </size>
                   </property>
                   <property name="text">
                     <string>X:</string>
                   </property>
                 </widget>
               </item>
-              <item row="10" column="2">
-                <widget class="QLabel" name="label_17">
-                  <property name="text">
-                    <string>μm</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="4" column="2">
-                <widget class="QLabel" name="label_13">
+              <item row="1" column="0" colspan="2">
+                <widget class="QLabel" name="stage_sn">
                   <property name="minimumSize">
                     <size>
-                      <width>50</width>
-                      <height>0</height>
+                      <width>0</width>
+                      <height>30</height>
                     </size>
                   </property>
                   <property name="maximumSize">
                     <size>
-                      <width>50</width>
-                      <height>16777215</height>
+                      <width>16777215</width>
+                      <height>30</height>
                     </size>
                   </property>
                   <property name="text">
-                    <string>μm</string>
+                    <string>SN</string>
                   </property>
                 </widget>
               </item>
-              <item row="6" column="1" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="local_coords_z">
+              <item row="8" column="1" alignment="Qt::AlignRight">
+                <widget class="QLabel" name="global_coords_x">
                   <property name="text">
                     <string>-</string>
                   </property>
                 </widget>
               </item>
-              <item row="10" column="1" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="global_coords_y">
-                  <property name="text">
-                    <string>-</string>
+              <item row="2" column="0" colspan="3">
+                <widget class="QLabel" name="local_coords">
+                  <property name="minimumSize">
+                    <size>
+                      <width>0</width>
+                      <height>30</height>
+                    </size>
                   </property>
-                </widget>
-              </item>
-              <item row="5" column="1" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="local_coords_y">
-                  <property name="text">
-                    <string>-</string>
+                  <property name="maximumSize">
+                    <size>
+                      <width>16777215</width>
+                      <height>30</height>
+                    </size>
                   </property>
-                </widget>
-              </item>
-              <item row="9" column="1" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="global_coords_x">
                   <property name="text">
-                    <string>-</string>
+                    <string>Local coords</string>
                   </property>
                 </widget>
               </item>
-              <item row="8" column="0" colspan="3">
-                <widget class="QLabel" name="global_coords">
+              <item row="0" column="0" colspan="3">
+                <widget class="QComboBox" name="stage_selector">
                   <property name="minimumSize">
                     <size>
                       <width>0</width>
-                      <height>70</height>
+                      <height>40</height>
                     </size>
                   </property>
                   <property name="maximumSize">
                     <size>
                       <width>16777215</width>
-                      <height>70</height>
+                      <height>40</height>
                     </size>
                   </property>
-                  <property name="text">
-                    <string>Global coords</string>
-                  </property>
                 </widget>
               </item>
-              <item row="5" column="0">
-                <widget class="QLabel" name="label_10">
+              <item row="6" column="0" colspan="3">
+                <widget class="QLabel" name="label_3">
                   <property name="maximumSize">
                     <size>
-                      <width>16777215</width>
-                      <height>50</height>
+                      <width>150</width>
+                      <height>5</height>
                     </size>
                   </property>
                   <property name="text">
-                    <string>Y:</string>
+                    <string/>
                   </property>
                 </widget>
               </item>
-              <item row="11" column="1" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="global_coords_z">
+              <item row="4" column="2">
+                <widget class="QLabel" name="label_14">
+                  <property name="text">
+                    <string>μm</string>
+                  </property>
+                </widget>
+              </item>
+              <item row="4" column="1" alignment="Qt::AlignRight">
+                <widget class="QLabel" name="local_coords_y">
                   <property name="text">
                     <string>-</string>
                   </property>
                 </widget>
               </item>
-              <item row="1" column="0" colspan="3">
-                <widget class="QComboBox" name="stage_selector">
-                  <property name="maximumSize">
+              <item row="4" column="0">
+                <widget class="QLabel" name="label_10">
+                  <property name="minimumSize">
                     <size>
-                      <width>16777215</width>
-                      <height>70</height>
+                      <width>0</width>
+                      <height>25</height>
                     </size>
                   </property>
-                </widget>
-              </item>
-              <item row="10" column="0">
-                <widget class="QLabel" name="label_6">
                   <property name="maximumSize">
                     <size>
                       <width>16777215</width>
-                      <height>50</height>
+                      <height>25</height>
                     </size>
                   </property>
                   <property name="text">
                     <string>Y:</string>
                   </property>
                 </widget>
               </item>
-              <item row="5" column="2">
-                <widget class="QLabel" name="label_14">
-                  <property name="text">
-                    <string>μm</string>
+              <item row="9" column="0">
+                <widget class="QLabel" name="label_6">
+                  <property name="minimumSize">
+                    <size>
+                      <width>0</width>
+                      <height>25</height>
+                    </size>
                   </property>
-                </widget>
-              </item>
-              <item row="12" column="0" colspan="3">
-                <widget class="QLabel" name="label_4">
                   <property name="maximumSize">
                     <size>
                       <width>16777215</width>
-                      <height>10</height>
+                      <height>25</height>
                     </size>
                   </property>
                   <property name="text">
-                    <string/>
+                    <string>Y:</string>
                   </property>
                 </widget>
               </item>
-              <item row="6" column="2">
-                <widget class="QLabel" name="label_15">
-                  <property name="maximumSize">
-                    <size>
-                      <width>40</width>
-                      <height>16777215</height>
-                    </size>
+              <item row="9" column="1" alignment="Qt::AlignRight">
+                <widget class="QLabel" name="global_coords_y">
+                  <property name="text">
+                    <string>-</string>
                   </property>
+                </widget>
+              </item>
+              <item row="8" column="2">
+                <widget class="QLabel" name="label_16">
                   <property name="text">
                     <string>μm</string>
                   </property>
                 </widget>
               </item>
             </layout>
           </item>
```

