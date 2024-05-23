# Comparing `tmp/pyllsm5dtools-1.1.2.tar.gz` & `tmp/pyllsm5dtools-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllsm5dtools-1.1.2.tar", last modified: Fri May 17 21:49:10 2024, max compression
+gzip compressed data, was "pyllsm5dtools-1.1.3.tar", last modified: Thu May 23 01:18:35 2024, max compression
```

## Comparing `pyllsm5dtools-1.1.2.tar` & `pyllsm5dtools-1.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-17 21:49:10.980253 pyllsm5dtools-1.1.2/
--rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 pyllsm5dtools-1.1.2/LICENSE.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-17 21:49:10.980253 pyllsm5dtools-1.1.2/PKG-INFO
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-17 21:49:10.976253 pyllsm5dtools-1.1.2/PyLLSM5DTools/
--rw-rw-r--   0 matt      (1000) matt      (1000)     3645 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3038 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_MIP_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3199 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_crop_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5155 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_decon_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5055 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3155 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6203 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6089 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3340 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_psf_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3144 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3351 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_resample_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3463 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2143 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2772 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-05-17 21:45:37.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     9176 2024-05-15 21:32:51.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/generatePythonWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools/generate_config_file.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-17 21:49:10.980253 pyllsm5dtools-1.1.2/PyLLSM5DTools.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-17 21:49:10.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-05-17 21:49:10.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-17 21:49:10.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-05-17 21:49:10.000000 pyllsm5dtools-1.1.2/PyLLSM5DTools.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 pyllsm5dtools-1.1.2/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-05-17 21:49:10.980253 pyllsm5dtools-1.1.2/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     3635 2024-05-17 21:46:11.000000 pyllsm5dtools-1.1.2/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-23 01:18:35.234588 pyllsm5dtools-1.1.3/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 pyllsm5dtools-1.1.3/LICENSE.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-23 01:18:35.234588 pyllsm5dtools-1.1.3/PKG-INFO
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-23 01:18:35.234588 pyllsm5dtools-1.1.3/PyLLSM5DTools/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3646 2024-05-23 01:14:40.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3038 2024-05-23 01:14:40.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_MIP_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3199 2024-05-23 01:14:40.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_crop_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5155 2024-05-23 01:14:40.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_decon_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5055 2024-05-23 01:14:40.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3155 2024-05-23 01:14:40.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6203 2024-05-23 01:14:40.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6089 2024-05-23 01:14:40.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3340 2024-05-23 01:14:40.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_psf_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3144 2024-05-23 01:14:40.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3351 2024-05-23 01:14:41.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_resample_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3463 2024-05-23 01:14:41.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2218 2024-05-23 01:14:41.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2772 2024-05-23 01:14:41.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-05-23 01:14:41.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     9176 2024-05-21 01:53:34.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/generatePythonWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools/generate_config_file.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-23 01:18:35.234588 pyllsm5dtools-1.1.3/PyLLSM5DTools.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-23 01:18:35.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-05-23 01:18:35.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-23 01:18:35.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-05-23 01:18:35.000000 pyllsm5dtools-1.1.3/PyLLSM5DTools.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 pyllsm5dtools-1.1.3/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-05-23 01:18:35.234588 pyllsm5dtools-1.1.3/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3635 2024-05-23 01:15:58.000000 pyllsm5dtools-1.1.3/setup.py
```

### Comparing `pyllsm5dtools-1.1.2/LICENSE.txt` & `pyllsm5dtools-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_FSC_analysis_wrapper.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_FSC_analysis_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def XR_FSC_analysis_wrapper(dataPaths, **kwargs):
     function_name = "XR_FSC_analysis_wrapper"
     XR_FSC_analysis_wrapper_dict = {
         "resultDirName": [kwargs.get("resultDirName", "FSCs"), "char"],
         "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericScalar"],
         "dz": [kwargs.get("dz", 0.1), "numericScalar"],
-        "dr": [kwargs.get("dr", 1), "numericScalar"],
+        "dr": [kwargs.get("dr", 10), "numericScalar"],
         "dtheta": [kwargs.get("dtheta", math.pi/12), "numericScalar"],
         "resThreshMethod": [kwargs.get("resThreshMethod", "fixed"), "char"],
         "resThresh": [kwargs.get("resThresh", 0.2), "numericScalar"],
         "halfSize": [kwargs.get("halfSize", [251,251,251]), "numericArr"],
         "inputBbox": [kwargs.get("inputBbox", []), "numericArr"],
         "resAxis": [kwargs.get("resAxis", "xz"), "char"],
         "skipConeRegion": [kwargs.get("skipConeRegion", True), "logical"],
```

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_MIP_wrapper.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_MIP_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_crop_dataset.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_crop_dataset.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_decon_data_wrapper.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_decon_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_matlab_stitching_wrapper.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_matlab_stitching_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_psf_analysis_wrapper.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_psf_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_resample_dataset.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_resample_dataset.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_tiffToZarr_wrapper.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_tiffToZarr_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import subprocess
 
 
 def XR_visualize_OTF_mask_segmentation(psfFn, OTFCumThresh, skewed, **kwargs):
     function_name = "XR_visualize_OTF_mask_segmentation"
     XR_visualize_OTF_mask_segmentation_dict = {
-
+        "minIntThrsh": [kwargs.get("minIntThrsh", 2.5e-3), "numericScalar"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux_with_jvm/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
     OTFCumThreshString = "[" + ",".join(str(item) for item in OTFCumThresh) + "]"
     skewedString = "{" + ",".join(f"'{item}'" for item in skewed) + "}"
     cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{psfFn}\" \"{OTFCumThreshString}\" \"{skewedString}\" "
```

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/XR_zarrToTiff_wrapper.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/XR_zarrToTiff_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/__init__.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/generatePythonWrapper.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/generatePythonWrapper.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,22 @@
     if not match:
         raise ValueError(f"Invalid MATLAB function format for file: {matlab_file_path}")
 
     function_name = match.group(1)
 
     # Extract inputParser parameters
     input_parser_params_addRequired = re.findall(r"ip\.addRequired\((.*?)(?:\s*,(.*))?\);", matlab_function)
-    input_parser_params_addParameter = re.findall(r"ip\.addParameter\((.*)\s*,(.*)\s*,(.*)\);", matlab_function)
     input_parser_params_addOptional = re.findall(r"ip\.addOptional\((.*)\s*,(.*)\s*,(.*)\);", matlab_function)
+    input_parser_params_addParameter = re.findall(r"ip\.addParameter\((.*)\s*,(.*)\s*,(.*)\);", matlab_function)
     num_optional = len(input_parser_params_addOptional)
 
     # Concatenate the capture groups and remove spaces
     input_parser_params = [",".join(param).replace(" ", "") for param in input_parser_params_addRequired]
-    input_parser_params += [",".join(param).replace(" ", "") for param in input_parser_params_addParameter]
     input_parser_params += [",".join(param).replace(" ", "") for param in input_parser_params_addOptional]
+    input_parser_params += [",".join(param).replace(" ", "") for param in input_parser_params_addParameter]
 
     return function_name, input_parser_params, num_optional
 
 
 def generate_function(matlab_file_path):
     function_name, input_parser_params, num_optional = parse_matlab_file(matlab_file_path)
```

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools/generate_config_file.py` & `pyllsm5dtools-1.1.3/PyLLSM5DTools/generate_config_file.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/PyLLSM5DTools.egg-info/SOURCES.txt` & `pyllsm5dtools-1.1.3/PyLLSM5DTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/README.md` & `pyllsm5dtools-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.1.2/setup.py` & `pyllsm5dtools-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 matlab_runtime_url = ("https://ssd.mathworks.com/supportfiles/downloads/R2023a/Release/6/deployment_files"
                       "/installer/complete/glnxa64/MATLAB_Runtime_R2023a_Update_6_glnxa64.zip")
 name = 'PyLLSM5DTools'
-version = '1.1.2'
+version = '1.1.3'
 
 
 class CustomInstall(install):
     def download_and_extract_matlab_runtime(self, install_dir):
         llsm5dtools_url = "https://github.com/abcucberkeley/LLSM5DTools/archive/refs/heads/main.zip"
         llsm5dtools_github_dir = os.path.join(install_dir, "LLSM5DTools-main")
         llsm5dtools_dir = os.path.join(install_dir, "LLSM5DTools")
```

