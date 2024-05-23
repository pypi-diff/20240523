# Comparing `tmp/Leonardo-Ai-SDK-5.4.2.tar.gz` & `tmp/Leonardo-Ai-SDK-5.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Leonardo-Ai-SDK-5.4.2.tar", last modified: Tue May 21 03:12:40 2024, max compression
+gzip compressed data, was "Leonardo-Ai-SDK-5.4.3.tar", last modified: Thu May 23 00:02:23 2024, max compression
```

## Comparing `Leonardo-Ai-SDK-5.4.2.tar` & `Leonardo-Ai-SDK-5.4.3.tar`

### file list

```diff
@@ -1,96 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.922219 Leonardo-Ai-SDK-5.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    16049 2024-05-21 03:12:40.922219 Leonardo-Ai-SDK-5.4.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    10092 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 03:12:40.922219 Leonardo-Ai-SDK-5.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.910219 Leonardo-Ai-SDK-5.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.910219 Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16049 2024-05-21 03:12:40.000000 Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-21 03:12:40.000000 Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 03:12:40.000000 Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 03:12:40.000000 Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 03:12:40.000000 Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.914219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.914219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/element.py
--rw-r--r--   0 runner    (1001) docker     (127)    45413 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/initimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    27431 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.914219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.914219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.922219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/creategeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createlcmgeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createtexturegeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createvariationnobg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createvariationunzoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createvariationupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletedatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletemodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/get3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getdatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getgenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getuserself.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getvariationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/listelements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/listplatformmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/performinpaintinglcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/performinstantrefine.py
--rw-r--r--   0 runner    (1001) docker     (127)    13322 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/pricingcalculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/promptimprove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/promptrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploaddatasetimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploadinitimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploadmodelasset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.922219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/controlnet_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/custom_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/lcm_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/model_asset_texture_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/pricingcalculatorservices.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/sd_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/sd_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/strength.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/universal_upscaler_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/variation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/pricing_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.922219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32647 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:02:23.331349 Leonardo-Ai-SDK-5.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-05-23 00:02:23.331349 Leonardo-Ai-SDK-5.4.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10340 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 00:02:23.331349 Leonardo-Ai-SDK-5.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:02:23.319349 Leonardo-Ai-SDK-5.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:02:23.319349 Leonardo-Ai-SDK-5.4.3/src/Leonardo_Ai_SDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-05-23 00:02:23.000000 Leonardo-Ai-SDK-5.4.3/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-23 00:02:23.000000 Leonardo-Ai-SDK-5.4.3/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 00:02:23.000000 Leonardo-Ai-SDK-5.4.3/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 00:02:23.000000 Leonardo-Ai-SDK-5.4.3/src/Leonardo_Ai_SDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 00:02:23.000000 Leonardo-Ai-SDK-5.4.3/src/Leonardo_Ai_SDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:02:23.323349 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:02:23.323349 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/init_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:02:23.323349 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:02:23.323349 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:02:23.331349 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/creategeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createlcmgeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createtexturegeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createvariationnobg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createvariationunzoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createvariationupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/deletedatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/deletegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/deletemodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/get3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getdatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getgenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getuserself.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getvariationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/listelements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/listplatformmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/performinpaintinglcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/performinstantrefine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13322 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/pricingcalculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/promptimprove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/promptrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/uploaddatasetimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/uploadinitimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/uploadmodelasset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:02:23.331349 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/controlnet_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/custom_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/lcm_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/model_asset_texture_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/pricingcalculatorservices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/sd_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/sd_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/strength.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/universal_upscaler_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/variation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13058 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/pricing_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14219 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/realtime_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15328 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/texture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/threed_model_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:02:23.331349 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32647 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-05-23 00:02:14.000000 Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/variation.py
```

### Comparing `Leonardo-Ai-SDK-5.4.2/LICENSE.md` & `Leonardo-Ai-SDK-5.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/PKG-INFO` & `Leonardo-Ai-SDK-5.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.4.2
+Version: 5.4.3
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
@@ -48,54 +48,66 @@
         
         * [create_dataset](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/dataset/README.md#create_dataset) - Create a Dataset
         * [delete_dataset_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/dataset/README.md#delete_dataset_by_id) - Delete a Single Dataset by ID
         * [get_dataset_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/dataset/README.md#get_dataset_by_id) - Get a Single Dataset by ID
         * [upload_dataset_image](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/dataset/README.md#upload_dataset_image) - Upload dataset image
         * [upload_dataset_image_from_gen](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/dataset/README.md#upload_dataset_image_from_gen) - Upload a Single Generated Image to a Dataset
         
-        ### [element](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/element/README.md)
+        ### [elements](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/elements/README.md)
         
-        * [list_elements](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/element/README.md#list_elements) - List Elements
+        * [list_elements](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/elements/README.md#list_elements) - List Elements
         
-        ### [generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md)
+        ### [image](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/README.md)
         
-        * [create_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#create_generation) - Create a Generation of Images
-        * [create_lcm_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#create_lcm_generation) - Create LCM Generation
-        * [create_svd_motion_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#create_svd_motion_generation) - Create SVD Motion Generation
-        * [create_texture_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#create_texture_generation) - Create Texture Generation
-        * [delete_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#delete_generation_by_id) - Delete a Single Generation
-        * [delete_texture_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#delete_texture_generation_by_id) - Delete Texture Generation by ID
-        * [get_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#get_generation_by_id) - Get a Single Generation
-        * [get_generations_by_user_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#get_generations_by_user_id) - Get generations by user ID
-        * [get_texture_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#get_texture_generation_by_id) - Get Texture Generation by ID
-        * [get_texture_generations_by_model_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#get_texture_generations_by_model_id) - Get texture generations by 3D Model ID
-        * [perform_alchemy_upscale_lcm](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
-        * [perform_inpainting_lcm](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#perform_inpainting_lcm) - Perform inpainting on a LCM image
-        * [perform_instant_refine](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#perform_instant_refine) - Perform instant refine on a LCM image
-        
-        ### [init_image](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimage/README.md)
-        
-        * [delete_init_image_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimage/README.md#delete_init_image_by_id) - Delete init image
-        * [get_init_image_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimage/README.md#get_init_image_by_id) - Get single init image
-        * [upload_init_image](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimage/README.md#upload_init_image) - Upload init image
+        * [create_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/README.md#create_generation) - Create a Generation of Images
+        * [delete_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/README.md#delete_generation_by_id) - Delete a Single Generation
+        * [get_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/README.md#get_generation_by_id) - Get a Single Generation
+        * [get_generations_by_user_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/README.md#get_generations_by_user_id) - Get generations by user ID
+        
+        ### [realtime_canvas](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/realtimecanvas/README.md)
+        
+        * [create_lcm_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/realtimecanvas/README.md#create_lcm_generation) - Create LCM Generation
+        * [perform_alchemy_upscale_lcm](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/realtimecanvas/README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
+        * [perform_inpainting_lcm](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/realtimecanvas/README.md#perform_inpainting_lcm) - Perform inpainting on a LCM image
+        * [perform_instant_refine](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/realtimecanvas/README.md#perform_instant_refine) - Perform instant refine on a LCM image
+        
+        ### [motion](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/motion/README.md)
+        
+        * [create_svd_motion_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/motion/README.md#create_svd_motion_generation) - Create SVD Motion Generation
+        
+        ### [texture](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/texture/README.md)
+        
+        * [create_texture_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/texture/README.md#create_texture_generation) - Create Texture Generation
+        * [delete_texture_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/texture/README.md#delete_texture_generation_by_id) - Delete Texture Generation by ID
+        * [get_texture_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/texture/README.md#get_texture_generation_by_id) - Get Texture Generation by ID
+        * [get_texture_generations_by_model_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/texture/README.md#get_texture_generations_by_model_id) - Get texture generations by 3D Model ID
+        
+        ### [init_images](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimages/README.md)
+        
+        * [delete_init_image_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimages/README.md#delete_init_image_by_id) - Delete init image
+        * [get_init_image_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimages/README.md#get_init_image_by_id) - Get single init image
+        * [upload_init_image](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimages/README.md#upload_init_image) - Upload init image
         
         ### [user](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/user/README.md)
         
         * [get_user_self](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/user/README.md#get_user_self) - Get user information
         
-        ### [model](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md)
+        ### [models](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/models/README.md)
         
-        * [create_model](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#create_model) - Train a Custom Model
-        * [delete3_d_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#delete3_d_model_by_id) - Delete 3D Model by ID
-        * [delete_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
-        * [get3_d_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#get3_d_model_by_id) - Get 3D Model by ID
-        * [get3_d_models_by_user_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#get3_d_models_by_user_id) - Get 3D models by user ID
-        * [get_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#get_model_by_id) - Get a Single Custom Model by ID
-        * [list_platform_models](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#list_platform_models) - List Platform Models
-        * [upload_model_asset](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#upload_model_asset) - Upload 3D Model
+        * [create_model](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/models/README.md#create_model) - Train a Custom Model
+        * [delete_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/models/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
+        * [get_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/models/README.md#get_model_by_id) - Get a Single Custom Model by ID
+        * [list_platform_models](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/models/README.md#list_platform_models) - List Platform Models
+        
+        ### [three_d_model_assets](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/threedmodelassets/README.md)
+        
+        * [delete3_d_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/threedmodelassets/README.md#delete3_d_model_by_id) - Delete 3D Model by ID
+        * [get3_d_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/threedmodelassets/README.md#get3_d_model_by_id) - Get 3D Model by ID
+        * [get3_d_models_by_user_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/threedmodelassets/README.md#get3_d_models_by_user_id) - Get 3D models by user ID
+        * [upload_model_asset](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/threedmodelassets/README.md#upload_model_asset) - Upload 3D Model
         
         ### [pricing_calculator](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/pricingcalculator/README.md)
         
         * [pricing_calculator](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/pricingcalculator/README.md#pricing_calculator) - Calculating API Cost
         
         ### [prompt](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.4.2 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.4.3 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) res = s.dataset.create_dataset
 (request=operations.CreateDatasetRequestBody( name='', )) if res.object is not
@@ -17,100 +17,108 @@
 sdk/blob/master/docs/sdks/dataset/README.md#get_dataset_by_id) - Get a Single
 Dataset by ID * [upload_dataset_image](https://github.com/Leonardo-Interactive/
 leonardo-python-sdk/blob/master/docs/sdks/dataset/
 README.md#upload_dataset_image) - Upload dataset image *
 [upload_dataset_image_from_gen](https://github.com/Leonardo-Interactive/
 leonardo-python-sdk/blob/master/docs/sdks/dataset/
 README.md#upload_dataset_image_from_gen) - Upload a Single Generated Image to a
-Dataset ### [element](https://github.com/Leonardo-Interactive/leonardo-python-
-sdk/blob/master/docs/sdks/element/README.md) * [list_elements](https://
+Dataset ### [elements](https://github.com/Leonardo-Interactive/leonardo-python-
+sdk/blob/master/docs/sdks/elements/README.md) * [list_elements](https://
 github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-element/README.md#list_elements) - List Elements ### [generation](https://
+elements/README.md#list_elements) - List Elements ### [image](https://
 github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-generation/README.md) * [create_generation](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/
-README.md#create_generation) - Create a Generation of Images *
-[create_lcm_generation](https://github.com/Leonardo-Interactive/leonardo-
-python-sdk/blob/master/docs/sdks/generation/README.md#create_lcm_generation) -
-Create LCM Generation * [create_svd_motion_generation](https://github.com/
-Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/
-README.md#create_svd_motion_generation) - Create SVD Motion Generation *
-[create_texture_generation](https://github.com/Leonardo-Interactive/leonardo-
-python-sdk/blob/master/docs/sdks/generation/
-README.md#create_texture_generation) - Create Texture Generation *
-[delete_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-
-python-sdk/blob/master/docs/sdks/generation/README.md#delete_generation_by_id)
-- Delete a Single Generation * [delete_texture_generation_by_id](https://
-github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-generation/README.md#delete_texture_generation_by_id) - Delete Texture
-Generation by ID * [get_generation_by_id](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/
-README.md#get_generation_by_id) - Get a Single Generation *
-[get_generations_by_user_id](https://github.com/Leonardo-Interactive/leonardo-
-python-sdk/blob/master/docs/sdks/generation/
-README.md#get_generations_by_user_id) - Get generations by user ID *
+image/README.md) * [create_generation](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/image/README.md#create_generation) -
+Create a Generation of Images * [delete_generation_by_id](https://github.com/
+Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/
+README.md#delete_generation_by_id) - Delete a Single Generation *
+[get_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-
+sdk/blob/master/docs/sdks/image/README.md#get_generation_by_id) - Get a Single
+Generation * [get_generations_by_user_id](https://github.com/Leonardo-
+Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/
+README.md#get_generations_by_user_id) - Get generations by user ID ###
+[realtime_canvas](https://github.com/Leonardo-Interactive/leonardo-python-sdk/
+blob/master/docs/sdks/realtimecanvas/README.md) * [create_lcm_generation]
+(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
+sdks/realtimecanvas/README.md#create_lcm_generation) - Create LCM Generation *
+[perform_alchemy_upscale_lcm](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/realtimecanvas/
+README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
+* [perform_inpainting_lcm](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/realtimecanvas/
+README.md#perform_inpainting_lcm) - Perform inpainting on a LCM image *
+[perform_instant_refine](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/realtimecanvas/
+README.md#perform_instant_refine) - Perform instant refine on a LCM image ###
+[motion](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/
+master/docs/sdks/motion/README.md) * [create_svd_motion_generation](https://
+github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
+motion/README.md#create_svd_motion_generation) - Create SVD Motion Generation
+### [texture](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/
+master/docs/sdks/texture/README.md) * [create_texture_generation](https://
+github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
+texture/README.md#create_texture_generation) - Create Texture Generation *
+[delete_texture_generation_by_id](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/texture/
+README.md#delete_texture_generation_by_id) - Delete Texture Generation by ID *
 [get_texture_generation_by_id](https://github.com/Leonardo-Interactive/
-leonardo-python-sdk/blob/master/docs/sdks/generation/
+leonardo-python-sdk/blob/master/docs/sdks/texture/
 README.md#get_texture_generation_by_id) - Get Texture Generation by ID *
 [get_texture_generations_by_model_id](https://github.com/Leonardo-Interactive/
-leonardo-python-sdk/blob/master/docs/sdks/generation/
+leonardo-python-sdk/blob/master/docs/sdks/texture/
 README.md#get_texture_generations_by_model_id) - Get texture generations by 3D
-Model ID * [perform_alchemy_upscale_lcm](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/
-README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
-* [perform_inpainting_lcm](https://github.com/Leonardo-Interactive/leonardo-
-python-sdk/blob/master/docs/sdks/generation/README.md#perform_inpainting_lcm) -
-Perform inpainting on a LCM image * [perform_instant_refine](https://
-github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-generation/README.md#perform_instant_refine) - Perform instant refine on a LCM
-image ### [init_image](https://github.com/Leonardo-Interactive/leonardo-python-
-sdk/blob/master/docs/sdks/initimage/README.md) * [delete_init_image_by_id]
-(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
-sdks/initimage/README.md#delete_init_image_by_id) - Delete init image *
-[get_init_image_by_id](https://github.com/Leonardo-Interactive/leonardo-python-
-sdk/blob/master/docs/sdks/initimage/README.md#get_init_image_by_id) - Get
-single init image * [upload_init_image](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimage/
-README.md#upload_init_image) - Upload init image ### [user](https://github.com/
-Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/user/README.md)
-* [get_user_self](https://github.com/Leonardo-Interactive/leonardo-python-sdk/
-blob/master/docs/sdks/user/README.md#get_user_self) - Get user information ###
-[model](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/
-master/docs/sdks/model/README.md) * [create_model](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/
-README.md#create_model) - Train a Custom Model * [delete3_d_model_by_id](https:
-//github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-model/README.md#delete3_d_model_by_id) - Delete 3D Model by ID *
-[delete_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-
-sdk/blob/master/docs/sdks/model/README.md#delete_model_by_id) - Delete a Single
-Custom Model by ID * [get3_d_model_by_id](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/
-README.md#get3_d_model_by_id) - Get 3D Model by ID * [get3_d_models_by_user_id]
-(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
-sdks/model/README.md#get3_d_models_by_user_id) - Get 3D models by user ID *
-[get_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/
-blob/master/docs/sdks/model/README.md#get_model_by_id) - Get a Single Custom
-Model by ID * [list_platform_models](https://github.com/Leonardo-Interactive/
-leonardo-python-sdk/blob/master/docs/sdks/model/README.md#list_platform_models)
-- List Platform Models * [upload_model_asset](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/
-README.md#upload_model_asset) - Upload 3D Model ### [pricing_calculator](https:
-//github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-pricingcalculator/README.md) * [pricing_calculator](https://github.com/
-Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-pricingcalculator/README.md#pricing_calculator) - Calculating API Cost ###
-[prompt](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/
-master/docs/sdks/prompt/README.md) * [prompt_improve](https://github.com/
-Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/
-README.md#prompt_improve) - Improve a Prompt * [prompt_random](https://
+Model ID ### [init_images](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/initimages/README.md) *
+[delete_init_image_by_id](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/initimages/README.md#delete_init_image_by_id)
+- Delete init image * [get_init_image_by_id](https://github.com/Leonardo-
+Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimages/
+README.md#get_init_image_by_id) - Get single init image * [upload_init_image]
+(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
+sdks/initimages/README.md#upload_init_image) - Upload init image ### [user]
+(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
+sdks/user/README.md) * [get_user_self](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/user/README.md#get_user_self) - Get
+user information ### [models](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/models/README.md) * [create_model](https://
 github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-prompt/README.md#prompt_random) - Generate a Random prompt ### [variation]
+models/README.md#create_model) - Train a Custom Model * [delete_model_by_id]
+(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
+sdks/models/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
+* [get_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-
+sdk/blob/master/docs/sdks/models/README.md#get_model_by_id) - Get a Single
+Custom Model by ID * [list_platform_models](https://github.com/Leonardo-
+Interactive/leonardo-python-sdk/blob/master/docs/sdks/models/
+README.md#list_platform_models) - List Platform Models ###
+[three_d_model_assets](https://github.com/Leonardo-Interactive/leonardo-python-
+sdk/blob/master/docs/sdks/threedmodelassets/README.md) *
+[delete3_d_model_by_id](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/threedmodelassets/
+README.md#delete3_d_model_by_id) - Delete 3D Model by ID * [get3_d_model_by_id]
 (https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
-sdks/variation/README.md) * [create_universal_upscaler_job](https://github.com/
-Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/
+sdks/threedmodelassets/README.md#get3_d_model_by_id) - Get 3D Model by ID *
+[get3_d_models_by_user_id](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/threedmodelassets/
+README.md#get3_d_models_by_user_id) - Get 3D models by user ID *
+[upload_model_asset](https://github.com/Leonardo-Interactive/leonardo-python-
+sdk/blob/master/docs/sdks/threedmodelassets/README.md#upload_model_asset) -
+Upload 3D Model ### [pricing_calculator](https://github.com/Leonardo-
+Interactive/leonardo-python-sdk/blob/master/docs/sdks/pricingcalculator/
+README.md) * [pricing_calculator](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/pricingcalculator/
+README.md#pricing_calculator) - Calculating API Cost ### [prompt](https://
+github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
+prompt/README.md) * [prompt_improve](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_improve) -
+Improve a Prompt * [prompt_random](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_random) -
+Generate a Random prompt ### [variation](https://github.com/Leonardo-
+Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md) *
+[create_universal_upscaler_job](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/variation/
 README.md#create_universal_upscaler_job) - Create using Universal Upscaler *
 [create_variation_no_bg](https://github.com/Leonardo-Interactive/leonardo-
 python-sdk/blob/master/docs/sdks/variation/README.md#create_variation_no_bg) -
 Create no background * [create_variation_unzoom](https://github.com/Leonardo-
 Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/
 README.md#create_variation_unzoom) - Create unzoom * [create_variation_upscale]
 (https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
```

### Comparing `Leonardo-Ai-SDK-5.4.2/README.md` & `Leonardo-Ai-SDK-5.4.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,54 +41,66 @@
 
 * [create_dataset](docs/sdks/dataset/README.md#create_dataset) - Create a Dataset
 * [delete_dataset_by_id](docs/sdks/dataset/README.md#delete_dataset_by_id) - Delete a Single Dataset by ID
 * [get_dataset_by_id](docs/sdks/dataset/README.md#get_dataset_by_id) - Get a Single Dataset by ID
 * [upload_dataset_image](docs/sdks/dataset/README.md#upload_dataset_image) - Upload dataset image
 * [upload_dataset_image_from_gen](docs/sdks/dataset/README.md#upload_dataset_image_from_gen) - Upload a Single Generated Image to a Dataset
 
-### [element](docs/sdks/element/README.md)
+### [elements](docs/sdks/elements/README.md)
 
-* [list_elements](docs/sdks/element/README.md#list_elements) - List Elements
+* [list_elements](docs/sdks/elements/README.md#list_elements) - List Elements
 
-### [generation](docs/sdks/generation/README.md)
+### [image](docs/sdks/image/README.md)
 
-* [create_generation](docs/sdks/generation/README.md#create_generation) - Create a Generation of Images
-* [create_lcm_generation](docs/sdks/generation/README.md#create_lcm_generation) - Create LCM Generation
-* [create_svd_motion_generation](docs/sdks/generation/README.md#create_svd_motion_generation) - Create SVD Motion Generation
-* [create_texture_generation](docs/sdks/generation/README.md#create_texture_generation) - Create Texture Generation
-* [delete_generation_by_id](docs/sdks/generation/README.md#delete_generation_by_id) - Delete a Single Generation
-* [delete_texture_generation_by_id](docs/sdks/generation/README.md#delete_texture_generation_by_id) - Delete Texture Generation by ID
-* [get_generation_by_id](docs/sdks/generation/README.md#get_generation_by_id) - Get a Single Generation
-* [get_generations_by_user_id](docs/sdks/generation/README.md#get_generations_by_user_id) - Get generations by user ID
-* [get_texture_generation_by_id](docs/sdks/generation/README.md#get_texture_generation_by_id) - Get Texture Generation by ID
-* [get_texture_generations_by_model_id](docs/sdks/generation/README.md#get_texture_generations_by_model_id) - Get texture generations by 3D Model ID
-* [perform_alchemy_upscale_lcm](docs/sdks/generation/README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
-* [perform_inpainting_lcm](docs/sdks/generation/README.md#perform_inpainting_lcm) - Perform inpainting on a LCM image
-* [perform_instant_refine](docs/sdks/generation/README.md#perform_instant_refine) - Perform instant refine on a LCM image
-
-### [init_image](docs/sdks/initimage/README.md)
-
-* [delete_init_image_by_id](docs/sdks/initimage/README.md#delete_init_image_by_id) - Delete init image
-* [get_init_image_by_id](docs/sdks/initimage/README.md#get_init_image_by_id) - Get single init image
-* [upload_init_image](docs/sdks/initimage/README.md#upload_init_image) - Upload init image
+* [create_generation](docs/sdks/image/README.md#create_generation) - Create a Generation of Images
+* [delete_generation_by_id](docs/sdks/image/README.md#delete_generation_by_id) - Delete a Single Generation
+* [get_generation_by_id](docs/sdks/image/README.md#get_generation_by_id) - Get a Single Generation
+* [get_generations_by_user_id](docs/sdks/image/README.md#get_generations_by_user_id) - Get generations by user ID
+
+### [realtime_canvas](docs/sdks/realtimecanvas/README.md)
+
+* [create_lcm_generation](docs/sdks/realtimecanvas/README.md#create_lcm_generation) - Create LCM Generation
+* [perform_alchemy_upscale_lcm](docs/sdks/realtimecanvas/README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
+* [perform_inpainting_lcm](docs/sdks/realtimecanvas/README.md#perform_inpainting_lcm) - Perform inpainting on a LCM image
+* [perform_instant_refine](docs/sdks/realtimecanvas/README.md#perform_instant_refine) - Perform instant refine on a LCM image
+
+### [motion](docs/sdks/motion/README.md)
+
+* [create_svd_motion_generation](docs/sdks/motion/README.md#create_svd_motion_generation) - Create SVD Motion Generation
+
+### [texture](docs/sdks/texture/README.md)
+
+* [create_texture_generation](docs/sdks/texture/README.md#create_texture_generation) - Create Texture Generation
+* [delete_texture_generation_by_id](docs/sdks/texture/README.md#delete_texture_generation_by_id) - Delete Texture Generation by ID
+* [get_texture_generation_by_id](docs/sdks/texture/README.md#get_texture_generation_by_id) - Get Texture Generation by ID
+* [get_texture_generations_by_model_id](docs/sdks/texture/README.md#get_texture_generations_by_model_id) - Get texture generations by 3D Model ID
+
+### [init_images](docs/sdks/initimages/README.md)
+
+* [delete_init_image_by_id](docs/sdks/initimages/README.md#delete_init_image_by_id) - Delete init image
+* [get_init_image_by_id](docs/sdks/initimages/README.md#get_init_image_by_id) - Get single init image
+* [upload_init_image](docs/sdks/initimages/README.md#upload_init_image) - Upload init image
 
 ### [user](docs/sdks/user/README.md)
 
 * [get_user_self](docs/sdks/user/README.md#get_user_self) - Get user information
 
-### [model](docs/sdks/model/README.md)
+### [models](docs/sdks/models/README.md)
 
-* [create_model](docs/sdks/model/README.md#create_model) - Train a Custom Model
-* [delete3_d_model_by_id](docs/sdks/model/README.md#delete3_d_model_by_id) - Delete 3D Model by ID
-* [delete_model_by_id](docs/sdks/model/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
-* [get3_d_model_by_id](docs/sdks/model/README.md#get3_d_model_by_id) - Get 3D Model by ID
-* [get3_d_models_by_user_id](docs/sdks/model/README.md#get3_d_models_by_user_id) - Get 3D models by user ID
-* [get_model_by_id](docs/sdks/model/README.md#get_model_by_id) - Get a Single Custom Model by ID
-* [list_platform_models](docs/sdks/model/README.md#list_platform_models) - List Platform Models
-* [upload_model_asset](docs/sdks/model/README.md#upload_model_asset) - Upload 3D Model
+* [create_model](docs/sdks/models/README.md#create_model) - Train a Custom Model
+* [delete_model_by_id](docs/sdks/models/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
+* [get_model_by_id](docs/sdks/models/README.md#get_model_by_id) - Get a Single Custom Model by ID
+* [list_platform_models](docs/sdks/models/README.md#list_platform_models) - List Platform Models
+
+### [three_d_model_assets](docs/sdks/threedmodelassets/README.md)
+
+* [delete3_d_model_by_id](docs/sdks/threedmodelassets/README.md#delete3_d_model_by_id) - Delete 3D Model by ID
+* [get3_d_model_by_id](docs/sdks/threedmodelassets/README.md#get3_d_model_by_id) - Get 3D Model by ID
+* [get3_d_models_by_user_id](docs/sdks/threedmodelassets/README.md#get3_d_models_by_user_id) - Get 3D models by user ID
+* [upload_model_asset](docs/sdks/threedmodelassets/README.md#upload_model_asset) - Upload 3D Model
 
 ### [pricing_calculator](docs/sdks/pricingcalculator/README.md)
 
 * [pricing_calculator](docs/sdks/pricingcalculator/README.md#pricing_calculator) - Calculating API Cost
 
 ### [prompt](docs/sdks/prompt/README.md)
```

#### html2text {}

```diff
@@ -8,63 +8,68 @@
 README.md#create_dataset) - Create a Dataset * [delete_dataset_by_id](docs/
 sdks/dataset/README.md#delete_dataset_by_id) - Delete a Single Dataset by ID *
 [get_dataset_by_id](docs/sdks/dataset/README.md#get_dataset_by_id) - Get a
 Single Dataset by ID * [upload_dataset_image](docs/sdks/dataset/
 README.md#upload_dataset_image) - Upload dataset image *
 [upload_dataset_image_from_gen](docs/sdks/dataset/
 README.md#upload_dataset_image_from_gen) - Upload a Single Generated Image to a
-Dataset ### [element](docs/sdks/element/README.md) * [list_elements](docs/sdks/
-element/README.md#list_elements) - List Elements ### [generation](docs/sdks/
-generation/README.md) * [create_generation](docs/sdks/generation/
+Dataset ### [elements](docs/sdks/elements/README.md) * [list_elements](docs/
+sdks/elements/README.md#list_elements) - List Elements ### [image](docs/sdks/
+image/README.md) * [create_generation](docs/sdks/image/
 README.md#create_generation) - Create a Generation of Images *
-[create_lcm_generation](docs/sdks/generation/README.md#create_lcm_generation) -
-Create LCM Generation * [create_svd_motion_generation](docs/sdks/generation/
-README.md#create_svd_motion_generation) - Create SVD Motion Generation *
-[create_texture_generation](docs/sdks/generation/
+[delete_generation_by_id](docs/sdks/image/README.md#delete_generation_by_id) -
+Delete a Single Generation * [get_generation_by_id](docs/sdks/image/
+README.md#get_generation_by_id) - Get a Single Generation *
+[get_generations_by_user_id](docs/sdks/image/
+README.md#get_generations_by_user_id) - Get generations by user ID ###
+[realtime_canvas](docs/sdks/realtimecanvas/README.md) * [create_lcm_generation]
+(docs/sdks/realtimecanvas/README.md#create_lcm_generation) - Create LCM
+Generation * [perform_alchemy_upscale_lcm](docs/sdks/realtimecanvas/
+README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
+* [perform_inpainting_lcm](docs/sdks/realtimecanvas/
+README.md#perform_inpainting_lcm) - Perform inpainting on a LCM image *
+[perform_instant_refine](docs/sdks/realtimecanvas/
+README.md#perform_instant_refine) - Perform instant refine on a LCM image ###
+[motion](docs/sdks/motion/README.md) * [create_svd_motion_generation](docs/
+sdks/motion/README.md#create_svd_motion_generation) - Create SVD Motion
+Generation ### [texture](docs/sdks/texture/README.md) *
+[create_texture_generation](docs/sdks/texture/
 README.md#create_texture_generation) - Create Texture Generation *
-[delete_generation_by_id](docs/sdks/generation/
-README.md#delete_generation_by_id) - Delete a Single Generation *
-[delete_texture_generation_by_id](docs/sdks/generation/
+[delete_texture_generation_by_id](docs/sdks/texture/
 README.md#delete_texture_generation_by_id) - Delete Texture Generation by ID *
-[get_generation_by_id](docs/sdks/generation/README.md#get_generation_by_id) -
-Get a Single Generation * [get_generations_by_user_id](docs/sdks/generation/
-README.md#get_generations_by_user_id) - Get generations by user ID *
-[get_texture_generation_by_id](docs/sdks/generation/
+[get_texture_generation_by_id](docs/sdks/texture/
 README.md#get_texture_generation_by_id) - Get Texture Generation by ID *
-[get_texture_generations_by_model_id](docs/sdks/generation/
+[get_texture_generations_by_model_id](docs/sdks/texture/
 README.md#get_texture_generations_by_model_id) - Get texture generations by 3D
-Model ID * [perform_alchemy_upscale_lcm](docs/sdks/generation/
-README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
-* [perform_inpainting_lcm](docs/sdks/generation/
-README.md#perform_inpainting_lcm) - Perform inpainting on a LCM image *
-[perform_instant_refine](docs/sdks/generation/README.md#perform_instant_refine)
-- Perform instant refine on a LCM image ### [init_image](docs/sdks/initimage/
-README.md) * [delete_init_image_by_id](docs/sdks/initimage/
+Model ID ### [init_images](docs/sdks/initimages/README.md) *
+[delete_init_image_by_id](docs/sdks/initimages/
 README.md#delete_init_image_by_id) - Delete init image * [get_init_image_by_id]
-(docs/sdks/initimage/README.md#get_init_image_by_id) - Get single init image *
-[upload_init_image](docs/sdks/initimage/README.md#upload_init_image) - Upload
+(docs/sdks/initimages/README.md#get_init_image_by_id) - Get single init image *
+[upload_init_image](docs/sdks/initimages/README.md#upload_init_image) - Upload
 init image ### [user](docs/sdks/user/README.md) * [get_user_self](docs/sdks/
-user/README.md#get_user_self) - Get user information ### [model](docs/sdks/
-model/README.md) * [create_model](docs/sdks/model/README.md#create_model) -
-Train a Custom Model * [delete3_d_model_by_id](docs/sdks/model/
-README.md#delete3_d_model_by_id) - Delete 3D Model by ID * [delete_model_by_id]
-(docs/sdks/model/README.md#delete_model_by_id) - Delete a Single Custom Model
-by ID * [get3_d_model_by_id](docs/sdks/model/README.md#get3_d_model_by_id) -
-Get 3D Model by ID * [get3_d_models_by_user_id](docs/sdks/model/
+user/README.md#get_user_self) - Get user information ### [models](docs/sdks/
+models/README.md) * [create_model](docs/sdks/models/README.md#create_model) -
+Train a Custom Model * [delete_model_by_id](docs/sdks/models/
+README.md#delete_model_by_id) - Delete a Single Custom Model by ID *
+[get_model_by_id](docs/sdks/models/README.md#get_model_by_id) - Get a Single
+Custom Model by ID * [list_platform_models](docs/sdks/models/
+README.md#list_platform_models) - List Platform Models ###
+[three_d_model_assets](docs/sdks/threedmodelassets/README.md) *
+[delete3_d_model_by_id](docs/sdks/threedmodelassets/
+README.md#delete3_d_model_by_id) - Delete 3D Model by ID * [get3_d_model_by_id]
+(docs/sdks/threedmodelassets/README.md#get3_d_model_by_id) - Get 3D Model by ID
+* [get3_d_models_by_user_id](docs/sdks/threedmodelassets/
 README.md#get3_d_models_by_user_id) - Get 3D models by user ID *
-[get_model_by_id](docs/sdks/model/README.md#get_model_by_id) - Get a Single
-Custom Model by ID * [list_platform_models](docs/sdks/model/
-README.md#list_platform_models) - List Platform Models * [upload_model_asset]
-(docs/sdks/model/README.md#upload_model_asset) - Upload 3D Model ###
-[pricing_calculator](docs/sdks/pricingcalculator/README.md) *
-[pricing_calculator](docs/sdks/pricingcalculator/README.md#pricing_calculator)
-- Calculating API Cost ### [prompt](docs/sdks/prompt/README.md) *
-[prompt_improve](docs/sdks/prompt/README.md#prompt_improve) - Improve a Prompt
-* [prompt_random](docs/sdks/prompt/README.md#prompt_random) - Generate a Random
-prompt ### [variation](docs/sdks/variation/README.md) *
+[upload_model_asset](docs/sdks/threedmodelassets/README.md#upload_model_asset)
+- Upload 3D Model ### [pricing_calculator](docs/sdks/pricingcalculator/
+README.md) * [pricing_calculator](docs/sdks/pricingcalculator/
+README.md#pricing_calculator) - Calculating API Cost ### [prompt](docs/sdks/
+prompt/README.md) * [prompt_improve](docs/sdks/prompt/README.md#prompt_improve)
+- Improve a Prompt * [prompt_random](docs/sdks/prompt/README.md#prompt_random)
+- Generate a Random prompt ### [variation](docs/sdks/variation/README.md) *
 [create_universal_upscaler_job](docs/sdks/variation/
 README.md#create_universal_upscaler_job) - Create using Universal Upscaler *
 [create_variation_no_bg](docs/sdks/variation/README.md#create_variation_no_bg)
 - Create no background * [create_variation_unzoom](docs/sdks/variation/
 README.md#create_variation_unzoom) - Create unzoom * [create_variation_upscale]
 (docs/sdks/variation/README.md#create_variation_upscale) - Create upscale *
 [get_variation_by_id](docs/sdks/variation/README.md#get_variation_by_id) - Get
```

### Comparing `Leonardo-Ai-SDK-5.4.2/setup.py` & `Leonardo-Ai-SDK-5.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='Leonardo-Ai-SDK',
-    version='5.4.2',
+    version='5.4.3',
     author='Leonardo-Ai',
     description='Leonardo AI Python Client SDK',
     url='https://github.com/Leonardo-Interactive/leonardo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/PKG-INFO` & `Leonardo-Ai-SDK-5.4.3/src/Leonardo_Ai_SDK.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.4.2
+Version: 5.4.3
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
@@ -48,54 +48,66 @@
         
         * [create_dataset](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/dataset/README.md#create_dataset) - Create a Dataset
         * [delete_dataset_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/dataset/README.md#delete_dataset_by_id) - Delete a Single Dataset by ID
         * [get_dataset_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/dataset/README.md#get_dataset_by_id) - Get a Single Dataset by ID
         * [upload_dataset_image](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/dataset/README.md#upload_dataset_image) - Upload dataset image
         * [upload_dataset_image_from_gen](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/dataset/README.md#upload_dataset_image_from_gen) - Upload a Single Generated Image to a Dataset
         
-        ### [element](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/element/README.md)
+        ### [elements](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/elements/README.md)
         
-        * [list_elements](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/element/README.md#list_elements) - List Elements
+        * [list_elements](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/elements/README.md#list_elements) - List Elements
         
-        ### [generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md)
+        ### [image](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/README.md)
         
-        * [create_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#create_generation) - Create a Generation of Images
-        * [create_lcm_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#create_lcm_generation) - Create LCM Generation
-        * [create_svd_motion_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#create_svd_motion_generation) - Create SVD Motion Generation
-        * [create_texture_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#create_texture_generation) - Create Texture Generation
-        * [delete_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#delete_generation_by_id) - Delete a Single Generation
-        * [delete_texture_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#delete_texture_generation_by_id) - Delete Texture Generation by ID
-        * [get_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#get_generation_by_id) - Get a Single Generation
-        * [get_generations_by_user_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#get_generations_by_user_id) - Get generations by user ID
-        * [get_texture_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#get_texture_generation_by_id) - Get Texture Generation by ID
-        * [get_texture_generations_by_model_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#get_texture_generations_by_model_id) - Get texture generations by 3D Model ID
-        * [perform_alchemy_upscale_lcm](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
-        * [perform_inpainting_lcm](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#perform_inpainting_lcm) - Perform inpainting on a LCM image
-        * [perform_instant_refine](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/README.md#perform_instant_refine) - Perform instant refine on a LCM image
-        
-        ### [init_image](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimage/README.md)
-        
-        * [delete_init_image_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimage/README.md#delete_init_image_by_id) - Delete init image
-        * [get_init_image_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimage/README.md#get_init_image_by_id) - Get single init image
-        * [upload_init_image](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimage/README.md#upload_init_image) - Upload init image
+        * [create_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/README.md#create_generation) - Create a Generation of Images
+        * [delete_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/README.md#delete_generation_by_id) - Delete a Single Generation
+        * [get_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/README.md#get_generation_by_id) - Get a Single Generation
+        * [get_generations_by_user_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/README.md#get_generations_by_user_id) - Get generations by user ID
+        
+        ### [realtime_canvas](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/realtimecanvas/README.md)
+        
+        * [create_lcm_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/realtimecanvas/README.md#create_lcm_generation) - Create LCM Generation
+        * [perform_alchemy_upscale_lcm](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/realtimecanvas/README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
+        * [perform_inpainting_lcm](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/realtimecanvas/README.md#perform_inpainting_lcm) - Perform inpainting on a LCM image
+        * [perform_instant_refine](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/realtimecanvas/README.md#perform_instant_refine) - Perform instant refine on a LCM image
+        
+        ### [motion](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/motion/README.md)
+        
+        * [create_svd_motion_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/motion/README.md#create_svd_motion_generation) - Create SVD Motion Generation
+        
+        ### [texture](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/texture/README.md)
+        
+        * [create_texture_generation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/texture/README.md#create_texture_generation) - Create Texture Generation
+        * [delete_texture_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/texture/README.md#delete_texture_generation_by_id) - Delete Texture Generation by ID
+        * [get_texture_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/texture/README.md#get_texture_generation_by_id) - Get Texture Generation by ID
+        * [get_texture_generations_by_model_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/texture/README.md#get_texture_generations_by_model_id) - Get texture generations by 3D Model ID
+        
+        ### [init_images](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimages/README.md)
+        
+        * [delete_init_image_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimages/README.md#delete_init_image_by_id) - Delete init image
+        * [get_init_image_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimages/README.md#get_init_image_by_id) - Get single init image
+        * [upload_init_image](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimages/README.md#upload_init_image) - Upload init image
         
         ### [user](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/user/README.md)
         
         * [get_user_self](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/user/README.md#get_user_self) - Get user information
         
-        ### [model](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md)
+        ### [models](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/models/README.md)
         
-        * [create_model](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#create_model) - Train a Custom Model
-        * [delete3_d_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#delete3_d_model_by_id) - Delete 3D Model by ID
-        * [delete_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
-        * [get3_d_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#get3_d_model_by_id) - Get 3D Model by ID
-        * [get3_d_models_by_user_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#get3_d_models_by_user_id) - Get 3D models by user ID
-        * [get_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#get_model_by_id) - Get a Single Custom Model by ID
-        * [list_platform_models](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#list_platform_models) - List Platform Models
-        * [upload_model_asset](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#upload_model_asset) - Upload 3D Model
+        * [create_model](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/models/README.md#create_model) - Train a Custom Model
+        * [delete_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/models/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
+        * [get_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/models/README.md#get_model_by_id) - Get a Single Custom Model by ID
+        * [list_platform_models](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/models/README.md#list_platform_models) - List Platform Models
+        
+        ### [three_d_model_assets](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/threedmodelassets/README.md)
+        
+        * [delete3_d_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/threedmodelassets/README.md#delete3_d_model_by_id) - Delete 3D Model by ID
+        * [get3_d_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/threedmodelassets/README.md#get3_d_model_by_id) - Get 3D Model by ID
+        * [get3_d_models_by_user_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/threedmodelassets/README.md#get3_d_models_by_user_id) - Get 3D models by user ID
+        * [upload_model_asset](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/threedmodelassets/README.md#upload_model_asset) - Upload 3D Model
         
         ### [pricing_calculator](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/pricingcalculator/README.md)
         
         * [pricing_calculator](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/pricingcalculator/README.md#pricing_calculator) - Calculating API Cost
         
         ### [prompt](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.4.2 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.4.3 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) res = s.dataset.create_dataset
 (request=operations.CreateDatasetRequestBody( name='', )) if res.object is not
@@ -17,100 +17,108 @@
 sdk/blob/master/docs/sdks/dataset/README.md#get_dataset_by_id) - Get a Single
 Dataset by ID * [upload_dataset_image](https://github.com/Leonardo-Interactive/
 leonardo-python-sdk/blob/master/docs/sdks/dataset/
 README.md#upload_dataset_image) - Upload dataset image *
 [upload_dataset_image_from_gen](https://github.com/Leonardo-Interactive/
 leonardo-python-sdk/blob/master/docs/sdks/dataset/
 README.md#upload_dataset_image_from_gen) - Upload a Single Generated Image to a
-Dataset ### [element](https://github.com/Leonardo-Interactive/leonardo-python-
-sdk/blob/master/docs/sdks/element/README.md) * [list_elements](https://
+Dataset ### [elements](https://github.com/Leonardo-Interactive/leonardo-python-
+sdk/blob/master/docs/sdks/elements/README.md) * [list_elements](https://
 github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-element/README.md#list_elements) - List Elements ### [generation](https://
+elements/README.md#list_elements) - List Elements ### [image](https://
 github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-generation/README.md) * [create_generation](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/
-README.md#create_generation) - Create a Generation of Images *
-[create_lcm_generation](https://github.com/Leonardo-Interactive/leonardo-
-python-sdk/blob/master/docs/sdks/generation/README.md#create_lcm_generation) -
-Create LCM Generation * [create_svd_motion_generation](https://github.com/
-Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/
-README.md#create_svd_motion_generation) - Create SVD Motion Generation *
-[create_texture_generation](https://github.com/Leonardo-Interactive/leonardo-
-python-sdk/blob/master/docs/sdks/generation/
-README.md#create_texture_generation) - Create Texture Generation *
-[delete_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-
-python-sdk/blob/master/docs/sdks/generation/README.md#delete_generation_by_id)
-- Delete a Single Generation * [delete_texture_generation_by_id](https://
-github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-generation/README.md#delete_texture_generation_by_id) - Delete Texture
-Generation by ID * [get_generation_by_id](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/
-README.md#get_generation_by_id) - Get a Single Generation *
-[get_generations_by_user_id](https://github.com/Leonardo-Interactive/leonardo-
-python-sdk/blob/master/docs/sdks/generation/
-README.md#get_generations_by_user_id) - Get generations by user ID *
+image/README.md) * [create_generation](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/image/README.md#create_generation) -
+Create a Generation of Images * [delete_generation_by_id](https://github.com/
+Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/
+README.md#delete_generation_by_id) - Delete a Single Generation *
+[get_generation_by_id](https://github.com/Leonardo-Interactive/leonardo-python-
+sdk/blob/master/docs/sdks/image/README.md#get_generation_by_id) - Get a Single
+Generation * [get_generations_by_user_id](https://github.com/Leonardo-
+Interactive/leonardo-python-sdk/blob/master/docs/sdks/image/
+README.md#get_generations_by_user_id) - Get generations by user ID ###
+[realtime_canvas](https://github.com/Leonardo-Interactive/leonardo-python-sdk/
+blob/master/docs/sdks/realtimecanvas/README.md) * [create_lcm_generation]
+(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
+sdks/realtimecanvas/README.md#create_lcm_generation) - Create LCM Generation *
+[perform_alchemy_upscale_lcm](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/realtimecanvas/
+README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
+* [perform_inpainting_lcm](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/realtimecanvas/
+README.md#perform_inpainting_lcm) - Perform inpainting on a LCM image *
+[perform_instant_refine](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/realtimecanvas/
+README.md#perform_instant_refine) - Perform instant refine on a LCM image ###
+[motion](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/
+master/docs/sdks/motion/README.md) * [create_svd_motion_generation](https://
+github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
+motion/README.md#create_svd_motion_generation) - Create SVD Motion Generation
+### [texture](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/
+master/docs/sdks/texture/README.md) * [create_texture_generation](https://
+github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
+texture/README.md#create_texture_generation) - Create Texture Generation *
+[delete_texture_generation_by_id](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/texture/
+README.md#delete_texture_generation_by_id) - Delete Texture Generation by ID *
 [get_texture_generation_by_id](https://github.com/Leonardo-Interactive/
-leonardo-python-sdk/blob/master/docs/sdks/generation/
+leonardo-python-sdk/blob/master/docs/sdks/texture/
 README.md#get_texture_generation_by_id) - Get Texture Generation by ID *
 [get_texture_generations_by_model_id](https://github.com/Leonardo-Interactive/
-leonardo-python-sdk/blob/master/docs/sdks/generation/
+leonardo-python-sdk/blob/master/docs/sdks/texture/
 README.md#get_texture_generations_by_model_id) - Get texture generations by 3D
-Model ID * [perform_alchemy_upscale_lcm](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/generation/
-README.md#perform_alchemy_upscale_lcm) - Perform Alchemy Upscale on a LCM image
-* [perform_inpainting_lcm](https://github.com/Leonardo-Interactive/leonardo-
-python-sdk/blob/master/docs/sdks/generation/README.md#perform_inpainting_lcm) -
-Perform inpainting on a LCM image * [perform_instant_refine](https://
-github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-generation/README.md#perform_instant_refine) - Perform instant refine on a LCM
-image ### [init_image](https://github.com/Leonardo-Interactive/leonardo-python-
-sdk/blob/master/docs/sdks/initimage/README.md) * [delete_init_image_by_id]
-(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
-sdks/initimage/README.md#delete_init_image_by_id) - Delete init image *
-[get_init_image_by_id](https://github.com/Leonardo-Interactive/leonardo-python-
-sdk/blob/master/docs/sdks/initimage/README.md#get_init_image_by_id) - Get
-single init image * [upload_init_image](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimage/
-README.md#upload_init_image) - Upload init image ### [user](https://github.com/
-Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/user/README.md)
-* [get_user_self](https://github.com/Leonardo-Interactive/leonardo-python-sdk/
-blob/master/docs/sdks/user/README.md#get_user_self) - Get user information ###
-[model](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/
-master/docs/sdks/model/README.md) * [create_model](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/
-README.md#create_model) - Train a Custom Model * [delete3_d_model_by_id](https:
-//github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-model/README.md#delete3_d_model_by_id) - Delete 3D Model by ID *
-[delete_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-
-sdk/blob/master/docs/sdks/model/README.md#delete_model_by_id) - Delete a Single
-Custom Model by ID * [get3_d_model_by_id](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/
-README.md#get3_d_model_by_id) - Get 3D Model by ID * [get3_d_models_by_user_id]
-(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
-sdks/model/README.md#get3_d_models_by_user_id) - Get 3D models by user ID *
-[get_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/
-blob/master/docs/sdks/model/README.md#get_model_by_id) - Get a Single Custom
-Model by ID * [list_platform_models](https://github.com/Leonardo-Interactive/
-leonardo-python-sdk/blob/master/docs/sdks/model/README.md#list_platform_models)
-- List Platform Models * [upload_model_asset](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/
-README.md#upload_model_asset) - Upload 3D Model ### [pricing_calculator](https:
-//github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-pricingcalculator/README.md) * [pricing_calculator](https://github.com/
-Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-pricingcalculator/README.md#pricing_calculator) - Calculating API Cost ###
-[prompt](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/
-master/docs/sdks/prompt/README.md) * [prompt_improve](https://github.com/
-Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/
-README.md#prompt_improve) - Improve a Prompt * [prompt_random](https://
+Model ID ### [init_images](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/initimages/README.md) *
+[delete_init_image_by_id](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/initimages/README.md#delete_init_image_by_id)
+- Delete init image * [get_init_image_by_id](https://github.com/Leonardo-
+Interactive/leonardo-python-sdk/blob/master/docs/sdks/initimages/
+README.md#get_init_image_by_id) - Get single init image * [upload_init_image]
+(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
+sdks/initimages/README.md#upload_init_image) - Upload init image ### [user]
+(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
+sdks/user/README.md) * [get_user_self](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/user/README.md#get_user_self) - Get
+user information ### [models](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/models/README.md) * [create_model](https://
 github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-prompt/README.md#prompt_random) - Generate a Random prompt ### [variation]
+models/README.md#create_model) - Train a Custom Model * [delete_model_by_id]
+(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
+sdks/models/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
+* [get_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-
+sdk/blob/master/docs/sdks/models/README.md#get_model_by_id) - Get a Single
+Custom Model by ID * [list_platform_models](https://github.com/Leonardo-
+Interactive/leonardo-python-sdk/blob/master/docs/sdks/models/
+README.md#list_platform_models) - List Platform Models ###
+[three_d_model_assets](https://github.com/Leonardo-Interactive/leonardo-python-
+sdk/blob/master/docs/sdks/threedmodelassets/README.md) *
+[delete3_d_model_by_id](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/threedmodelassets/
+README.md#delete3_d_model_by_id) - Delete 3D Model by ID * [get3_d_model_by_id]
 (https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
-sdks/variation/README.md) * [create_universal_upscaler_job](https://github.com/
-Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/
+sdks/threedmodelassets/README.md#get3_d_model_by_id) - Get 3D Model by ID *
+[get3_d_models_by_user_id](https://github.com/Leonardo-Interactive/leonardo-
+python-sdk/blob/master/docs/sdks/threedmodelassets/
+README.md#get3_d_models_by_user_id) - Get 3D models by user ID *
+[upload_model_asset](https://github.com/Leonardo-Interactive/leonardo-python-
+sdk/blob/master/docs/sdks/threedmodelassets/README.md#upload_model_asset) -
+Upload 3D Model ### [pricing_calculator](https://github.com/Leonardo-
+Interactive/leonardo-python-sdk/blob/master/docs/sdks/pricingcalculator/
+README.md) * [pricing_calculator](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/pricingcalculator/
+README.md#pricing_calculator) - Calculating API Cost ### [prompt](https://
+github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
+prompt/README.md) * [prompt_improve](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_improve) -
+Improve a Prompt * [prompt_random](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_random) -
+Generate a Random prompt ### [variation](https://github.com/Leonardo-
+Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md) *
+[create_universal_upscaler_job](https://github.com/Leonardo-Interactive/
+leonardo-python-sdk/blob/master/docs/sdks/variation/
 README.md#create_universal_upscaler_job) - Create using Universal Upscaler *
 [create_variation_no_bg](https://github.com/Leonardo-Interactive/leonardo-
 python-sdk/blob/master/docs/sdks/variation/README.md#create_variation_no_bg) -
 Create no background * [create_variation_unzoom](https://github.com/Leonardo-
 Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/
 README.md#create_variation_unzoom) - Create unzoom * [create_variation_upscale]
 (https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
```

### Comparing `Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt` & `Leonardo-Ai-SDK-5.4.3/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 src/Leonardo_Ai_SDK.egg-info/PKG-INFO
 src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
 src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
 src/Leonardo_Ai_SDK.egg-info/requires.txt
 src/Leonardo_Ai_SDK.egg-info/top_level.txt
 src/leonardoaisdk/__init__.py
 src/leonardoaisdk/dataset.py
-src/leonardoaisdk/element.py
-src/leonardoaisdk/generation.py
-src/leonardoaisdk/initimage.py
-src/leonardoaisdk/model.py
+src/leonardoaisdk/elements.py
+src/leonardoaisdk/image.py
+src/leonardoaisdk/init_images.py
+src/leonardoaisdk/models_.py
+src/leonardoaisdk/motion.py
 src/leonardoaisdk/pricing_calculator.py
 src/leonardoaisdk/prompt.py
+src/leonardoaisdk/realtime_canvas.py
 src/leonardoaisdk/sdk.py
 src/leonardoaisdk/sdkconfiguration.py
+src/leonardoaisdk/texture.py
+src/leonardoaisdk/threed_model_assets.py
 src/leonardoaisdk/user.py
 src/leonardoaisdk/variation.py
 src/leonardoaisdk/_hooks/__init__.py
 src/leonardoaisdk/_hooks/sdkhooks.py
 src/leonardoaisdk/_hooks/types.py
 src/leonardoaisdk/models/__init__.py
 src/leonardoaisdk/models/errors/__init__.py
```

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/_hooks/sdkhooks.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/_hooks/types.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/dataset.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/dataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/element.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
 from leonardoaisdk._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from leonardoaisdk.models import errors, operations
 from typing import Optional
 
-class Element:
+class Elements:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
```

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/initimage.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/init_images.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
 from leonardoaisdk._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from leonardoaisdk.models import errors, operations
 from typing import Optional
 
-class InitImage:
+class InitImages:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
```

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/model.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/threed_model_assets.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,84 +3,22 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
 from leonardoaisdk._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from leonardoaisdk.models import errors, operations
 from typing import Optional
 
-class Model:
+class ThreeDModelAssets:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create_model(self, request: operations.CreateModelRequestBody) -> operations.CreateModelResponse:
-        r"""Train a Custom Model
-        This endpoint will train a new custom model
-        """
-        hook_ctx = HookContext(operation_id='createModel', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = base_url + '/models'
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateModelRequestBody, "request", False, False, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        if data is None and form is None:
-            raise Exception('request body is required')
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        res = operations.CreateModelResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[operations.CreateModelResponseBody])
-                res.object = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
     def delete3_d_model_by_id(self, id: str, request_body: Optional[operations.Delete3DModelByIDRequestBody] = None) -> operations.Delete3DModelByIDResponse:
         r"""Delete 3D Model by ID
         This endpoint deletes the specific 3D Model
         """
         hook_ctx = HookContext(operation_id='delete3DModelById', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.Delete3DModelByIDRequest(
             id=id,
@@ -138,75 +76,14 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def delete_model_by_id(self, id: str) -> operations.DeleteModelByIDResponse:
-        r"""Delete a Single Custom Model by ID
-        This endpoint will delete a specific custom model
-        """
-        hook_ctx = HookContext(operation_id='deleteModelById', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.DeleteModelByIDRequest(
-            id=id,
-        )
-        
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(base_url, '/models/{id}', request)
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        res = operations.DeleteModelByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteModelByIDResponseBody])
-                res.object = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
     def get3_d_model_by_id(self, id: str, request_body: Optional[operations.Get3DModelByIDRequestBody] = None, limit: Optional[int] = None, offset: Optional[int] = None) -> operations.Get3DModelByIDResponse:
         r"""Get 3D Model by ID
         This endpoint gets the specific 3D model
         """
         hook_ctx = HookContext(operation_id='get3DModelById', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.Get3DModelByIDRequest(
             id=id,
@@ -329,132 +206,14 @@
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
-    def get_model_by_id(self, id: str) -> operations.GetModelByIDResponse:
-        r"""Get a Single Custom Model by ID
-        This endpoint gets the specific custom model
-        """
-        hook_ctx = HookContext(operation_id='getModelById', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetModelByIDRequest(
-            id=id,
-        )
-        
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(base_url, '/models/{id}', request)
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        res = operations.GetModelByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetModelByIDResponseBody])
-                res.object = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
-    def list_platform_models(self) -> operations.ListPlatformModelsResponse:
-        r"""List Platform Models
-        Get a list of public Platform Models available for use with generations.
-        """
-        hook_ctx = HookContext(operation_id='listPlatformModels', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = base_url + '/platformModels'
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        res = operations.ListPlatformModelsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListPlatformModelsResponseBody])
-                res.object = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def upload_model_asset(self, request: Optional[operations.UploadModelAssetRequestBody] = None) -> operations.UploadModelAssetResponse:
```

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/errors/sdkerror.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/__init__.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createdataset.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createdataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/creategeneration.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/creategeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createlcmgeneration.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createlcmgeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createmodel.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createmodel.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createtexturegeneration.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createtexturegeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createvariationnobg.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createvariationnobg.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createvariationunzoom.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createvariationunzoom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createvariationupscale.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/createvariationupscale.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/delete3dmodelbyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/delete3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletedatasetbyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/deletedatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletegenerationbyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/deletegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deleteinitimagebyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/deleteinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletemodelbyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/deletemodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/get3dmodelbyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/get3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getdatasetbyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getdatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getgenerationbyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getgenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getinitimagebyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getmodelbyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getuserself.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getuserself.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getvariationbyid.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/getvariationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/listelements.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/listelements.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/listplatformmodels.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/listplatformmodels.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/performinpaintinglcm.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/performinpaintinglcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/performinstantrefine.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/performinstantrefine.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/pricingcalculator.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/pricingcalculator.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/promptimprove.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/promptimprove.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/promptrandom.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/promptrandom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploaddatasetimage.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/uploaddatasetimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploadinitimage.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/uploadinitimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploadmodelasset.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/operations/uploadmodelasset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/__init__.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/custom_model_type.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/custom_model_type.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/element_input.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/element_input.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/lcm_generation_style.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/lcm_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/pricingcalculatorservices.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/pricingcalculatorservices.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/sd_generation_style.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/sd_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/sd_versions.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/models/shared/sd_versions.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/pricing_calculator.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/pricing_calculator.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/prompt.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/prompt.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/sdk.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/sdk.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .dataset import Dataset
-from .element import Element
-from .generation import Generation
-from .initimage import InitImage
-from .model import Model
+from .elements import Elements
+from .image import Image
+from .init_images import InitImages
+from .models_ import Models
+from .motion import Motion
 from .pricing_calculator import PricingCalculator
 from .prompt import Prompt
+from .realtime_canvas import RealtimeCanvas
 from .sdkconfiguration import SDKConfiguration
+from .texture import Texture
+from .threed_model_assets import ThreeDModelAssets
 from .user import User
 from .utils.retries import RetryConfig
 from .variation import Variation
 from leonardoaisdk import utils
 from leonardoaisdk._hooks import SDKHooks
 from leonardoaisdk.models import shared
 from typing import Callable, Dict, Optional, Union
 
 class LeonardoAiSDK:
     r"""Rest Endpoints: Leonardo.Ai API OpenAPI specification."""
     dataset: Dataset
-    element: Element
-    generation: Generation
-    init_image: InitImage
+    elements: Elements
+    image: Image
+    realtime_canvas: RealtimeCanvas
+    motion: Motion
+    texture: Texture
+    init_images: InitImages
     user: User
-    model: Model
+    models: Models
+    three_d_model_assets: ThreeDModelAssets
     pricing_calculator: PricingCalculator
     prompt: Prompt
     variation: Variation
 
     sdk_configuration: SDKConfiguration
 
     def __init__(self,
@@ -87,15 +95,19 @@
         self.sdk_configuration.__dict__['_hooks'] = hooks
 
         self._init_sdks()
 
 
     def _init_sdks(self):
         self.dataset = Dataset(self.sdk_configuration)
-        self.element = Element(self.sdk_configuration)
-        self.generation = Generation(self.sdk_configuration)
-        self.init_image = InitImage(self.sdk_configuration)
+        self.elements = Elements(self.sdk_configuration)
+        self.image = Image(self.sdk_configuration)
+        self.realtime_canvas = RealtimeCanvas(self.sdk_configuration)
+        self.motion = Motion(self.sdk_configuration)
+        self.texture = Texture(self.sdk_configuration)
+        self.init_images = InitImages(self.sdk_configuration)
         self.user = User(self.sdk_configuration)
-        self.model = Model(self.sdk_configuration)
+        self.models = Models(self.sdk_configuration)
+        self.three_d_model_assets = ThreeDModelAssets(self.sdk_configuration)
         self.pricing_calculator = PricingCalculator(self.sdk_configuration)
         self.prompt = Prompt(self.sdk_configuration)
         self.variation = Variation(self.sdk_configuration)
```

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/sdkconfiguration.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/sdkconfiguration.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.0'
-    sdk_version: str = '5.4.2'
-    gen_version: str = '2.332.4'
-    user_agent: str = 'speakeasy-sdk/python 5.4.2 2.332.4 v1.0.0 Leonardo-Ai-SDK'
+    sdk_version: str = '5.4.3'
+    gen_version: str = '2.333.3'
+    user_agent: str = 'speakeasy-sdk/python 5.4.3 2.333.3 v1.0.0 Leonardo-Ai-SDK'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/user.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/user.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/utils/retries.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/utils/utils.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/variation.py` & `Leonardo-Ai-SDK-5.4.3/src/leonardoaisdk/variation.py`

 * *Files identical despite different names*

