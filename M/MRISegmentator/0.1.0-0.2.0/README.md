# Comparing `tmp/mrisegmentator-0.1.0.tar.gz` & `tmp/mrisegmentator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrisegmentator-0.1.0.tar", last modified: Mon May 20 21:14:07 2024, max compression
+gzip compressed data, was "mrisegmentator-0.2.0.tar", last modified: Wed May 22 22:03:08 2024, max compression
```

## Comparing `mrisegmentator-0.1.0.tar` & `mrisegmentator-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-sr-x   0 suria2   (60730) drdcad   (10355)        0 2024-05-20 21:14:07.011121 mrisegmentator-0.1.0/
-drwxr-sr-x   0 suria2   (60730) drdcad   (10355)        0 2024-05-20 21:14:07.000338 mrisegmentator-0.1.0/MRISegmentator.egg-info/
--rw-r--r--   0 suria2   (60730) drdcad   (10355)      592 2024-05-20 21:14:06.000000 mrisegmentator-0.1.0/MRISegmentator.egg-info/PKG-INFO
--rw-r--r--   0 suria2   (60730) drdcad   (10355)      356 2024-05-20 21:14:06.000000 mrisegmentator-0.1.0/MRISegmentator.egg-info/SOURCES.txt
--rw-r--r--   0 suria2   (60730) drdcad   (10355)        1 2024-05-20 21:14:06.000000 mrisegmentator-0.1.0/MRISegmentator.egg-info/dependency_links.txt
--rw-r--r--   0 suria2   (60730) drdcad   (10355)       63 2024-05-20 21:14:06.000000 mrisegmentator-0.1.0/MRISegmentator.egg-info/entry_points.txt
--rw-r--r--   0 suria2   (60730) drdcad   (10355)        1 2024-05-20 20:46:47.000000 mrisegmentator-0.1.0/MRISegmentator.egg-info/not-zip-safe
--rw-r--r--   0 suria2   (60730) drdcad   (10355)       49 2024-05-20 21:14:06.000000 mrisegmentator-0.1.0/MRISegmentator.egg-info/requires.txt
--rw-r--r--   0 suria2   (60730) drdcad   (10355)       15 2024-05-20 21:14:06.000000 mrisegmentator-0.1.0/MRISegmentator.egg-info/top_level.txt
--rw-r--r--   0 suria2   (60730) drdcad   (10355)      592 2024-05-20 21:14:07.006344 mrisegmentator-0.1.0/PKG-INFO
-drwxr-sr-x   0 suria2   (60730) drdcad   (10355)        0 2024-05-20 21:14:06.994044 mrisegmentator-0.1.0/mrisegmentator/
--rw-r--r--   0 suria2   (60730) drdcad   (10355)        0 2024-05-20 20:13:31.000000 mrisegmentator-0.1.0/mrisegmentator/__init__.py
--rw-r--r--   0 suria2   (60730) drdcad   (10355)     1136 2024-05-20 21:01:11.000000 mrisegmentator-0.1.0/mrisegmentator/cmdline.py
--rw-r--r--   0 suria2   (60730) drdcad   (10355)     1772 2024-05-20 20:40:39.000000 mrisegmentator-0.1.0/mrisegmentator/inference.py
--rw-r--r--   0 suria2   (60730) drdcad   (10355)       38 2024-05-20 21:14:07.012574 mrisegmentator-0.1.0/setup.cfg
--rw-r--r--   0 suria2   (60730) drdcad   (10355)     1006 2024-05-20 20:32:13.000000 mrisegmentator-0.1.0/setup.py
+drwxr-s---   0 suria2   (60730) drdcad   (10355)        0 2024-05-22 22:03:08.406207 mrisegmentator-0.2.0/
+drwxr-s---   0 suria2   (60730) drdcad   (10355)        0 2024-05-22 22:03:08.384039 mrisegmentator-0.2.0/MRISegmentator.egg-info/
+-rw-r--r--   0 suria2   (60730) drdcad   (10355)     5374 2024-05-22 22:03:08.000000 mrisegmentator-0.2.0/MRISegmentator.egg-info/PKG-INFO
+-rw-r--r--   0 suria2   (60730) drdcad   (10355)      366 2024-05-22 22:03:08.000000 mrisegmentator-0.2.0/MRISegmentator.egg-info/SOURCES.txt
+-rw-r--r--   0 suria2   (60730) drdcad   (10355)        1 2024-05-22 22:03:08.000000 mrisegmentator-0.2.0/MRISegmentator.egg-info/dependency_links.txt
+-rw-r--r--   0 suria2   (60730) drdcad   (10355)       63 2024-05-22 22:03:08.000000 mrisegmentator-0.2.0/MRISegmentator.egg-info/entry_points.txt
+-rw-r--r--   0 suria2   (60730) drdcad   (10355)        1 2024-05-20 20:46:47.000000 mrisegmentator-0.2.0/MRISegmentator.egg-info/not-zip-safe
+-rw-r--r--   0 suria2   (60730) drdcad   (10355)       49 2024-05-22 22:03:08.000000 mrisegmentator-0.2.0/MRISegmentator.egg-info/requires.txt
+-rw-r--r--   0 suria2   (60730) drdcad   (10355)       15 2024-05-22 22:03:08.000000 mrisegmentator-0.2.0/MRISegmentator.egg-info/top_level.txt
+-rw-r--r--   0 suria2   (60730) drdcad   (10355)     5374 2024-05-22 22:03:08.397441 mrisegmentator-0.2.0/PKG-INFO
+-rw-r-----   0 suria2   (60730) drdcad   (10355)     4805 2024-05-22 19:28:19.000000 mrisegmentator-0.2.0/README.md
+drwxr-s---   0 suria2   (60730) drdcad   (10355)        0 2024-05-22 22:03:08.374055 mrisegmentator-0.2.0/mrisegmentator/
+-rw-r--r--   0 suria2   (60730) drdcad   (10355)        0 2024-05-20 20:13:31.000000 mrisegmentator-0.2.0/mrisegmentator/__init__.py
+-rw-r--r--   0 suria2   (60730) drdcad   (10355)     1106 2024-05-22 16:52:56.000000 mrisegmentator-0.2.0/mrisegmentator/cmdline.py
+-rw-r--r--   0 suria2   (60730) drdcad   (10355)     3103 2024-05-22 21:56:20.000000 mrisegmentator-0.2.0/mrisegmentator/inference.py
+-rw-r-----   0 suria2   (60730) drdcad   (10355)       38 2024-05-22 22:03:08.411928 mrisegmentator-0.2.0/setup.cfg
+-rw-r--r--   0 suria2   (60730) drdcad   (10355)     1057 2024-05-22 22:02:56.000000 mrisegmentator-0.2.0/setup.py
```

### Comparing `mrisegmentator-0.1.0/mrisegmentator/cmdline.py` & `mrisegmentator-0.2.0/mrisegmentator/cmdline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import argparse
 
-from .inference import mri_segmentator
-from pathlib import Path
-import os
 
 def main():
     parser = argparse.ArgumentParser(description="Segment 68 anatomical structures on T1 weighted MRI. Model by Yan Zhuang. Package by Abhinav Suri. If you use this tool cite https://arxiv.org/abs/2405.05944")
 
     parser.add_argument("-i", metavar="filepath", dest="input",
                         help="Path to MR nifti image", required=True)
 
-    parser.add_argument("-o", metavar="directory", dest="output",
+    parser.add_argument("-o", metavar="filepath", dest="output",
                         help="Output filepath for segmentation masks",
                         required=False)
     
     parser.add_argument("-d", "--device", choices=["gpu", "cpu", "mps"],
                         help="Device to run on (default: gpu).",
                         default="gpu")
     
     parser.add_argument("-m", metavar="directory", dest="path_to_model",
                         help="Path to trained nnunet model",
                         required=True)
 
     args = parser.parse_args()
 
+    from .inference import mri_segmentator
+
     mri_segmentator(args.input, args.output, args.device, args.path_to_model)
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `mrisegmentator-0.1.0/mrisegmentator/inference.py` & `mrisegmentator-0.2.0/mrisegmentator/inference.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,96 @@
-import torch
 from batchgenerators.utilities.file_and_folder_operations import join
-from nnunetv2.inference.predict_from_raw_data import nnUNetPredictor
 import os
+import contextlib
+import sys
+import warnings
+
+
+class DummyFile:
+    def write(self, x): pass
+    def flush(self): pass
+
+@contextlib.contextmanager
+def nostdout(verbose=False):
+    if not verbose:
+        save_stdout = sys.stdout
+        sys.stdout = DummyFile()
+        yield
+        sys.stdout = save_stdout
+    else:
+        yield
 
 
 def mri_segmentator(input_file, output_file, device='gpu', path_to_model='nnUNetTrainer__nnUNetPlans__3d_fullres'):
-    if input_file.find('.nii.gz') == -1:
-        raise ValueError("invalid file type: must have .nii.gz in filename")
+    print("Checking inputs")
+    if input_file.find('.nii') == -1:
+        raise ValueError("invalid file type: must have .nii in filename")
     if os.path.exists(input_file) == False:
         raise ValueError("path to input file must exist")
-        
-    if device == 'gpu':
-        device = torch.device('cuda')
-    elif device == 'cpu':
-        device = torch.device('cpu')
-    elif device == 'mps':
-        device = torch.device('mps')
-    else:
+    if device not in ['gpu', 'cpu', 'mps']:
         raise ValueError("invalid device: must be one of 'gpu', 'cpu', or 'mps'")
 
     if not os.path.isdir(path_to_model):
         raise ValueError("invalid path to trained model folder")
-     
+    print("setup devices") 
+
+    import torch
+
+    if device == 'gpu':
+        devicet = torch.device('cuda')
+    elif device == 'cpu':
+        devicet = torch.device('cpu')
+    elif device == 'mps':
+        devicet = torch.device('mps')
+
+    if device == 'cpu':
+        import multiprocessing
+        torch.set_num_threads(multiprocessing.cpu_count())
+
+    os.environ['nnUNet_raw'] = output_file
+    os.environ['nnUNet_preprocessed'] = output_file
+    os.environ['nnUNet_results'] = output_file
+    # os.environ['nnUNet_preprocessed'] = str(path_to_model)
+    # os.environ['nnUNet_results'] = str(path_to_model)
+
+    warnings.filterwarnings("ignore", category=UserWarning, module="nnunetv2")
+    with nostdout():
+        from nnunetv2.inference.predict_from_raw_data import nnUNetPredictor
+
     print("Instantiating nnunet predictor...")
-    predictor = nnUNetPredictor(
-        tile_step_size=0.5,
-        use_gaussian=True,
-        use_mirroring=True,
-        perform_everything_on_device=True,
-        device=device,
-        verbose=False,
-        verbose_preprocessing=False,
-        allow_tqdm=True
-    )
+    with nostdout():
+        predictor = nnUNetPredictor(
+            tile_step_size=0.5,
+            use_gaussian=True,
+            use_mirroring=False,
+            perform_everything_on_device=True,
+            device=devicet,
+            verbose=False,
+            verbose_preprocessing=False,
+            allow_tqdm=True
+        )
 
    
     print("Instantiating trained model...")
-    predictor.initialize_from_trained_model_folder(
-        path_to_model,
-        use_folds=(0,1,2,3,4),
-        checkpoint_name='checkpoint_final.pth',
-    )
+    with nostdout():
+        predictor.initialize_from_trained_model_folder(
+            path_to_model,
+            use_folds=(0,1,2,3,4) if device != 'cpu' else (0,),
+            checkpoint_name='checkpoint_final.pth',
+        )
 
     print("Starting prediction...")
-    return predictor.predict_from_files([[input_file]],
-         [output_file],
-         save_probabilities=False, overwrite=False,
-         num_processes_preprocessing=1, num_processes_segmentation_export=1,
-         folder_with_segs_from_prev_stage=None, num_parts=1, part_id=0)
+    with nostdout():
+        predictor.predict_from_files([[input_file]],
+             [output_file],
+             save_probabilities=False, overwrite=True,
+             num_processes_preprocessing=1, num_processes_segmentation_export=1,
+             folder_with_segs_from_prev_stage=None, num_parts=1, part_id=0)
+    print("Cleaning up...")
+    for i in ['dataset.json', 'plans.json', 'predict_from_raw_data_args.json']:
+        try:
+            os.remove(os.path.dirname(os.path.abspath(output_file)) + '/' + i)
+        except Exception as e:
+            print(i, e)
+            pass
     print("DONE!")
 
-
-
-
-
```

