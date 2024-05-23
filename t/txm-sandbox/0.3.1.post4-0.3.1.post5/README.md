# Comparing `tmp/txm_sandbox-0.3.1.post4.tar.gz` & `tmp/txm_sandbox-0.3.1.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txm_sandbox-0.3.1.post4.tar", last modified: Tue May 21 05:52:14 2024, max compression
+gzip compressed data, was "txm_sandbox-0.3.1.post5.tar", last modified: Thu May 23 02:27:50 2024, max compression
```

## Comparing `txm_sandbox-0.3.1.post4.tar` & `txm_sandbox-0.3.1.post5.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.118980 txm_sandbox-0.3.1.post4/
--rw-rw-r--   0 xianghui   (501) staff       (20)     1070 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1.post4/LICENSE
--rw-rw-r--   0 xianghui   (501) staff       (20)      203 2024-05-09 00:28:45.000000 txm_sandbox-0.3.1.post4/MANIFEST.in
--rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-21 05:52:14.118776 txm_sandbox-0.3.1.post4/PKG-INFO
--rw-rw-r--   0 xianghui   (501) staff       (20)     1964 2024-05-09 00:35:34.000000 txm_sandbox-0.3.1.post4/README.md
--rwxrwxr-x   0 xianghui   (501) staff       (20)     2565 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1.post4/TXM_GUI2.ipynb
--rw-r--r--   0 xianghui   (501) staff       (20)       38 2024-05-21 05:52:14.119021 txm_sandbox-0.3.1.post4/setup.cfg
--rw-rw-r--   0 xianghui   (501) staff       (20)     1130 2024-05-21 05:51:43.000000 txm_sandbox-0.3.1.post4/setup.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.086325 txm_sandbox-0.3.1.post4/txm_sandbox/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/__init__.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.088834 txm_sandbox-0.3.1.post4/txm_sandbox/config/
--rw-rw-r--   0 xianghui   (501) staff       (20)     5092 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/config/XANES2D_GUI_config.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/config/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)       45 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/config/analysis_tool_gui_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      497 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/config/io_tomo_h5_data_structure.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/config/io_xanes2D_h5_data_structure.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      616 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/config/io_xanes3D_h5_data_structure.json
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.090321 txm_sandbox-0.3.1.post4/txm_sandbox/dicts/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/dicts/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     3848 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/dicts/config_dict.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    61110 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/dicts/customized_struct_dict.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      755 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/dicts/sklearn_opt_dict.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      583 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/dicts/xanes_analysis_dict.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.090781 txm_sandbox-0.3.1.post4/txm_sandbox/external/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/external/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      253 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/external/user_io.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.099102 txm_sandbox-0.3.1.post4/txm_sandbox/gui/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/gui/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    32500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/gui/conv_data_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    74137 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/gui/gen_algn_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    79148 2024-05-12 04:56:04.000000 txm_sandbox-0.3.1.post4/txm_sandbox/gui/gui_components.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    36752 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/gui/io_config_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    15709 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/gui/main_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      795 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/gui/misc_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   169879 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/gui/tomo_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   204783 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/gui/xanes2D_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   202060 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/gui/xanes3D_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    91679 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/gui/xanes_analysis_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)   203269 2024-05-18 14:45:10.000000 txm_sandbox-0.3.1.post4/txm_sandbox/gui/xanes_fitting_gui.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.101523 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/__init__.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.103268 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/configs/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/configs/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      979 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      957 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)      899 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)     2389 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
--rw-rw-r--   0 xianghui   (501) staff       (20)     1362 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.103629 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/dicts/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/dicts/__init__.py
--rw-r--r--   0 xianghui   (501) staff       (20)     8853 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/dicts/data_struct_dict.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.107842 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/
--rw-rw-r--   0 xianghui   (501) staff       (20)      106 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16170 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/appl_mask_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     9799 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/convert_data_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)     3929 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/extra_io_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)      196 2024-05-19 15:27:59.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/lcf_cfg_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)    29844 2024-05-19 22:28:29.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/tomo_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)    24249 2024-05-21 03:24:11.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
--rw-r--r--   0 xianghui   (501) staff       (20)    67248 2024-05-18 02:01:00.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16157 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.109964 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     4223 2024-05-14 05:10:46.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      650 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)      599 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    15251 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     2441 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16610 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     1197 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
--rw-r--r--   0 xianghui   (501) staff       (20)     2029 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
--rw-r--r--   0 xianghui   (501) staff       (20)     1533 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/txm_gui.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.111105 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/utils/
--rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/utils/__init__.py
--rw-r--r--   0 xianghui   (501) staff       (20)     6339 2024-05-19 22:44:39.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/utils/ext_io_lib.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     1264 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/utils/io.py
--rw-r--r--   0 xianghui   (501) staff       (20)    10709 2024-05-16 05:38:21.000000 txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/utils/misc.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.111613 txm_sandbox-0.3.1.post4/txm_sandbox/tmp/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/tmp/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)       69 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/tmp/readme.txt
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.118213 txm_sandbox-0.3.1.post4/txm_sandbox/utils/
--rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/__init__.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    16672 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/io.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    14410 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/lineshapes.py
--rwxrwxr-x   0 xianghui   (501) staff       (20)     4246 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/misc.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     1439 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/plotlib.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    61837 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/reg_algs.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    70498 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/tomo_recon_tools.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    42166 2024-05-18 14:44:34.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/xanes_analysis.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     2342 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/xanes_image_utils.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    27376 2024-05-18 14:19:49.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/xanes_math.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     6083 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/xanes_post_analysis.py
--rw-rw-r--   0 xianghui   (501) staff       (20)    84137 2024-05-19 13:48:34.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/xanes_regtools.py
--rw-rw-r--   0 xianghui   (501) staff       (20)     3266 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post4/txm_sandbox/utils/xanes_spectra_filters.py
-drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-21 05:52:14.118505 txm_sandbox-0.3.1.post4/txm_sandbox.egg-info/
--rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-21 05:52:14.000000 txm_sandbox-0.3.1.post4/txm_sandbox.egg-info/PKG-INFO
--rw-r--r--   0 xianghui   (501) staff       (20)     3239 2024-05-21 05:52:14.000000 txm_sandbox-0.3.1.post4/txm_sandbox.egg-info/SOURCES.txt
--rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-21 05:52:14.000000 txm_sandbox-0.3.1.post4/txm_sandbox.egg-info/dependency_links.txt
--rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-21 05:52:14.000000 txm_sandbox-0.3.1.post4/txm_sandbox.egg-info/not-zip-safe
--rw-r--r--   0 xianghui   (501) staff       (20)      170 2024-05-21 05:52:14.000000 txm_sandbox-0.3.1.post4/txm_sandbox.egg-info/requires.txt
--rw-r--r--   0 xianghui   (501) staff       (20)       12 2024-05-21 05:52:14.000000 txm_sandbox-0.3.1.post4/txm_sandbox.egg-info/top_level.txt
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.286214 txm_sandbox-0.3.1.post5/
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1070 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1.post5/LICENSE
+-rw-rw-r--   0 xianghui   (501) staff       (20)      203 2024-05-09 00:28:45.000000 txm_sandbox-0.3.1.post5/MANIFEST.in
+-rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-23 02:27:50.286001 txm_sandbox-0.3.1.post5/PKG-INFO
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1964 2024-05-09 00:35:34.000000 txm_sandbox-0.3.1.post5/README.md
+-rwxrwxr-x   0 xianghui   (501) staff       (20)     2565 2024-04-27 23:21:56.000000 txm_sandbox-0.3.1.post5/TXM_GUI2.ipynb
+-rw-r--r--   0 xianghui   (501) staff       (20)       38 2024-05-23 02:27:50.286251 txm_sandbox-0.3.1.post5/setup.cfg
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1130 2024-05-23 02:26:48.000000 txm_sandbox-0.3.1.post5/setup.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.250469 txm_sandbox-0.3.1.post5/txm_sandbox/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/__init__.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.253041 txm_sandbox-0.3.1.post5/txm_sandbox/config/
+-rw-rw-r--   0 xianghui   (501) staff       (20)     5092 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/config/XANES2D_GUI_config.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/config/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)       45 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/config/analysis_tool_gui_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      497 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/config/io_tomo_h5_data_structure.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/config/io_xanes2D_h5_data_structure.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      616 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/config/io_xanes3D_h5_data_structure.json
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.255118 txm_sandbox-0.3.1.post5/txm_sandbox/dicts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/dicts/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     3848 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/dicts/config_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    61110 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/dicts/customized_struct_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      755 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/dicts/sklearn_opt_dict.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      583 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/dicts/xanes_analysis_dict.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.255812 txm_sandbox-0.3.1.post5/txm_sandbox/external/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/external/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      253 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/external/user_io.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.268251 txm_sandbox-0.3.1.post5/txm_sandbox/gui/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/gui/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    32500 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/gui/conv_data_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    74137 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/gui/gen_algn_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    79148 2024-05-12 04:56:04.000000 txm_sandbox-0.3.1.post5/txm_sandbox/gui/gui_components.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    36752 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/gui/io_config_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    15709 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/gui/main_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      795 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/gui/misc_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   169879 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/gui/tomo_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   204783 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/gui/xanes2D_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   202060 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/gui/xanes3D_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    91679 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/gui/xanes_analysis_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)   203269 2024-05-18 14:45:10.000000 txm_sandbox-0.3.1.post5/txm_sandbox/gui/xanes_fitting_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.270403 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/__init__.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.272479 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/configs/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/configs/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      979 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      957 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)      899 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2389 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1362 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.272846 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/dicts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/dicts/__init__.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     8853 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/dicts/data_struct_dict.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.276193 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      106 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16170 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/appl_mask_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     9799 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/convert_data_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     3929 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/extra_io_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     1040 2024-05-23 02:20:05.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/lcf_cfg_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    29844 2024-05-19 22:28:29.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/tomo_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    24405 2024-05-23 02:25:29.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    67248 2024-05-18 02:01:00.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16157 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.278331 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     4223 2024-05-14 05:10:46.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      650 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)      599 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    15251 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2441 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16610 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1197 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     2029 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     1533 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/txm_gui.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.279523 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/utils/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      181 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/utils/__init__.py
+-rw-r--r--   0 xianghui   (501) staff       (20)     6339 2024-05-19 22:44:39.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/utils/ext_io_lib.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1264 2024-05-14 04:58:24.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/utils/io.py
+-rw-r--r--   0 xianghui   (501) staff       (20)    10709 2024-05-16 05:38:21.000000 txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/utils/misc.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.280028 txm_sandbox-0.3.1.post5/txm_sandbox/tmp/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/tmp/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)       69 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/tmp/readme.txt
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.285461 txm_sandbox-0.3.1.post5/txm_sandbox/utils/
+-rw-rw-r--   0 xianghui   (501) staff       (20)      107 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/__init__.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    16672 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/io.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    14410 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/lineshapes.py
+-rwxrwxr-x   0 xianghui   (501) staff       (20)     4246 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/misc.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     1439 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/plotlib.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    61837 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/reg_algs.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    70498 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/tomo_recon_tools.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    42166 2024-05-18 14:44:34.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/xanes_analysis.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     2342 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/xanes_image_utils.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    27376 2024-05-18 14:19:49.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/xanes_math.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     6083 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/xanes_post_analysis.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)    84137 2024-05-19 13:48:34.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/xanes_regtools.py
+-rw-rw-r--   0 xianghui   (501) staff       (20)     3266 2024-04-28 16:42:36.000000 txm_sandbox-0.3.1.post5/txm_sandbox/utils/xanes_spectra_filters.py
+drwxr-xr-x   0 xianghui   (501) staff       (20)        0 2024-05-23 02:27:50.285761 txm_sandbox-0.3.1.post5/txm_sandbox.egg-info/
+-rw-r--r--   0 xianghui   (501) staff       (20)      712 2024-05-23 02:27:50.000000 txm_sandbox-0.3.1.post5/txm_sandbox.egg-info/PKG-INFO
+-rw-r--r--   0 xianghui   (501) staff       (20)     3239 2024-05-23 02:27:50.000000 txm_sandbox-0.3.1.post5/txm_sandbox.egg-info/SOURCES.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-23 02:27:50.000000 txm_sandbox-0.3.1.post5/txm_sandbox.egg-info/dependency_links.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)        1 2024-05-23 02:27:50.000000 txm_sandbox-0.3.1.post5/txm_sandbox.egg-info/not-zip-safe
+-rw-r--r--   0 xianghui   (501) staff       (20)      170 2024-05-23 02:27:50.000000 txm_sandbox-0.3.1.post5/txm_sandbox.egg-info/requires.txt
+-rw-r--r--   0 xianghui   (501) staff       (20)       12 2024-05-23 02:27:50.000000 txm_sandbox-0.3.1.post5/txm_sandbox.egg-info/top_level.txt
```

### Comparing `txm_sandbox-0.3.1.post4/LICENSE` & `txm_sandbox-0.3.1.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/PKG-INFO` & `txm_sandbox-0.3.1.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txm_sandbox
-Version: 0.3.1.post4
+Version: 0.3.1.post5
 Summary: Integrated Spectro-Imaging Analysis Toolbox
 Home-page: https://github.com/xianghuix/TXM_Sandbox
 Author: Xianghui Xiao
 Author-email: xianghuix@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: python>=3.11
```

### Comparing `txm_sandbox-0.3.1.post4/README.md` & `txm_sandbox-0.3.1.post5/README.md`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/TXM_GUI2.ipynb` & `txm_sandbox-0.3.1.post5/TXM_GUI2.ipynb`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/setup.py` & `txm_sandbox-0.3.1.post5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: xiao
 """
 
 from setuptools import setup, find_packages
 
 setup(name='txm_sandbox',
-      version='0.3.1.post4',
+      version='0.3.1.post5',
       description='Integrated Spectro-Imaging Analysis Toolbox',
       url='https://github.com/xianghuix/TXM_Sandbox',
       author='Xianghui Xiao',
       author_email='xianghuix@gmail.com',
       license='MIT',
       packages=find_packages(),
       install_requires=[
```

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/config/XANES2D_GUI_config.json` & `txm_sandbox-0.3.1.post5/txm_sandbox/config/XANES2D_GUI_config.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/config/io_xanes3D_h5_data_structure.json` & `txm_sandbox-0.3.1.post5/txm_sandbox/config/io_xanes3D_h5_data_structure.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/dicts/config_dict.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/dicts/config_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/dicts/customized_struct_dict.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/dicts/customized_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/dicts/sklearn_opt_dict.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/dicts/sklearn_opt_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/dicts/xanes_analysis_dict.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/dicts/xanes_analysis_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/gui/conv_data_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/gui/conv_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/gui/gen_algn_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/gui/gen_algn_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/gui/gui_components.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/gui/gui_components.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/gui/io_config_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/gui/io_config_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/gui/main_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/gui/main_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/gui/misc_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/gui/misc_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/gui/tomo_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/gui/tomo_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/gui/xanes2D_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/gui/xanes2D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/gui/xanes3D_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/gui/xanes3D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/gui/xanes_analysis_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/gui/xanes_analysis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/gui/xanes_fitting_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/gui/xanes_fitting_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/dicts/data_struct_dict.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/dicts/data_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/appl_mask_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/appl_mask_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/convert_data_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/convert_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/extra_io_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/extra_io_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/tomo_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/tomo_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/xanes_fit_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/xanes_fit_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     set_data_widget,
     overlap_roi,
     update_layer_in_viewer,
     show_layers_in_viewer,
     rm_gui_viewers,
     disp_progress_info,
 )
+from .lcf_cfg_gui import lcf_cfg_gui
 
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 xanes3d_fit_script_fn = Path(__file__).parents[1] / "scripts/xanes3D_fit_cmd.py"
 xanes2d_fit_script_fn = Path(__file__).parents[1] / "scripts/xanes2D_fit_cmd.py"
 
 with open(Path(__file__).parents[1] / "configs/xanes_proc_data_struct_cfg.json") as f:
@@ -308,15 +309,15 @@
         self.eng_eV.value = ""
         self.sli.value = 0
         self.E.value = 0
         self.spec_in_roi.value = False
         self.roi_cen_x.value = self.roi_cen_x.min
         self.roi_cen_y.value = self.roi_cen_y.min
         self.element.value = ""
-        self.analysis_type = "wl"
+        self.analysis_type.value = "wl"
         self.edge_eng.value = ""
         self.wl_s.value = ""
         self.wl_e.value = ""
         self.edge_s.value = ""
         self.edge_e.value = ""
         self.downsample_factor.value = 1
         global _XANES_FIT_SAVE_ITEMS_CHOICES
@@ -464,15 +465,15 @@
                 "wl_fit_err",
             ]
             self.save_items.reset_choices()
             self.save_items.value = [
                 "wl_pos_fit",
                 "weighted_attenuation",
             ]
-        else:
+        elif self.analysis_type.value == "full":
             self.edge_eng.enabled = True
             self.edge_s.enabled = True
             self.edge_e.enabled = True
             _XANES_FIT_SAVE_ITEMS_CHOICES = [
                 "wl_pos_fit",
                 "edge_pos_fit",
                 "edge50_pos_fit",
@@ -483,14 +484,16 @@
             self.save_items.reset_choices()
             self.save_items.value = [
                 "wl_pos_fit",
                 "edge_pos_fit",
                 "edge50_pos_fit",
                 "weighted_attenuation",
             ]
+        elif self.analysis_type.value == "lcf":
+            lcf_cfg_gui(self)
 
     @disp_progress_info("xanes data fitting")
     def _xanes_fit(self):
         self._close_file()
 
         with open(cfg_fn, "r") as f:
             tem = json.load(f)
```

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/xanes_reg_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/xanes_reg_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/guis/xanes_vis_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/guis/xanes_vis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/aps_xanes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/txm_gui.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/txm_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/utils/ext_io_lib.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/utils/ext_io_lib.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/utils/io.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/napari_gui/utils/misc.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/napari_gui/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/utils/io.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/utils/lineshapes.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/utils/lineshapes.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/utils/misc.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/utils/plotlib.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/utils/plotlib.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/utils/reg_algs.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/utils/reg_algs.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/utils/tomo_recon_tools.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/utils/tomo_recon_tools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/utils/xanes_analysis.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/utils/xanes_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/utils/xanes_image_utils.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/utils/xanes_image_utils.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/utils/xanes_math.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/utils/xanes_math.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/utils/xanes_post_analysis.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/utils/xanes_post_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/utils/xanes_regtools.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/utils/xanes_regtools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox/utils/xanes_spectra_filters.py` & `txm_sandbox-0.3.1.post5/txm_sandbox/utils/xanes_spectra_filters.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox.egg-info/PKG-INFO` & `txm_sandbox-0.3.1.post5/txm_sandbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txm_sandbox
-Version: 0.3.1.post4
+Version: 0.3.1.post5
 Summary: Integrated Spectro-Imaging Analysis Toolbox
 Home-page: https://github.com/xianghuix/TXM_Sandbox
 Author: Xianghui Xiao
 Author-email: xianghuix@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: python>=3.11
```

### Comparing `txm_sandbox-0.3.1.post4/txm_sandbox.egg-info/SOURCES.txt` & `txm_sandbox-0.3.1.post5/txm_sandbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

