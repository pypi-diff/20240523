# Comparing `tmp/torch_model_manager-0.4.0.dev9.tar.gz` & `tmp/torch_model_manager-0.4.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.0.dev9.tar", last modified: Thu May 23 07:07:21 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.1.dev1.tar", last modified: Thu May 23 12:37:15 2024, max compression
```

## Comparing `torch_model_manager-0.4.0.dev9.tar` & `torch_model_manager-0.4.1.dev1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.106859 torch_model_manager-0.4.0.dev9/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-23 07:07:21.106859 torch_model_manager-0.4.0.dev9/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev9/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-23 07:07:21.106859 torch_model_manager-0.4.0.dev9/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2219 2024-05-23 07:07:19.000000 torch_model_manager-0.4.0.dev9/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.098859 torch_model_manager-0.4.0.dev9/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.102859 torch_model_manager-0.4.0.dev9/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev9/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.102859 torch_model_manager-0.4.0.dev9/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev9/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev9/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.102859 torch_model_manager-0.4.0.dev9/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev9/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev9/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev9/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    14009 2024-05-23 07:06:52.000000 torch_model_manager-0.4.0.dev9/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev9/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev9/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.106859 torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-23 07:07:21.000000 torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-23 07:07:21.000000 torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-23 07:07:21.000000 torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      228 2024-05-23 07:07:21.000000 torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-23 07:07:21.000000 torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.106859 torch_model_manager-0.4.0.dev9/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev9/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.0.dev9/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.538599 torch_model_manager-0.4.1.dev1/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-23 12:37:15.538599 torch_model_manager-0.4.1.dev1/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev1/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-23 12:37:15.538599 torch_model_manager-0.4.1.dev1/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2219 2024-05-23 12:37:13.000000 torch_model_manager-0.4.1.dev1/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.534599 torch_model_manager-0.4.1.dev1/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.534599 torch_model_manager-0.4.1.dev1/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev1/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.534599 torch_model_manager-0.4.1.dev1/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev1/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev1/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.538599 torch_model_manager-0.4.1.dev1/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.1.dev1/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32763 2024-05-23 09:59:17.000000 torch_model_manager-0.4.1.dev1/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.1.dev1/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    20684 2024-05-23 12:34:10.000000 torch_model_manager-0.4.1.dev1/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.1.dev1/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.1.dev1/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.538599 torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-23 12:37:15.000000 torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-23 12:37:15.000000 torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-23 12:37:15.000000 torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      228 2024-05-23 12:37:15.000000 torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-23 12:37:15.000000 torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.538599 torch_model_manager-0.4.1.dev1/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev1/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.1.dev1/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.0.dev9/PKG-INFO` & `torch_model_manager-0.4.1.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev9
+Version: 0.4.1.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.0.dev9/README.md` & `torch_model_manager-0.4.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev9/setup.py` & `torch_model_manager-0.4.1.dev1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.0.dev9',
+    version='0.4.1.dev1',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.1.dev1/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev9/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.1.dev1/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev9/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.1.dev1/torch_model_manager/neptune_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         struct = NeptuneManager.project.get_structure()
         for elem in ns :
             struct = struct[elem]
         
         return list(struct.keys())
 
     def log_tensors(self, 
-                    tensors, 
+                    tensors: torch.Tensor, 
                     descriptions: List[str] = None, 
                     names: List[str] = None, 
                     paths: List[str] = None, 
                     namespace: str = None, 
                     on_series: bool = False):
         """
         Log tensors to Neptune.
```

### Comparing `torch_model_manager-0.4.0.dev9/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.1.dev1/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev9/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.1.dev1/torch_model_manager/segmentation_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,238 +10,32 @@
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 from groundingdino.util.inference import Model
 from utils import helpers
 from segment_anything import sam_model_registry, SamPredictor
 from scipy.stats import hmean
 import pandas as pd
 from tqdm import tqdm
+from PIL import Image
+from lang_sam import LangSAM
 
-DEVICE = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
+DEVICE = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
 class SegmentationManager:
-    def __init__(self, sam_backbone="sam_vit_h", g_dino_backbone="swin_t", device=DEVICE):
+    def __init__(self, sam_type='vit_h', checkpoint_path=None, return_prompts=False, device=DEVICE):
         self.device = device
-        
-        # Paths for checkpoints and configs
-        g_dino_model_config_path = "GroundingDINO/groundingdino/config"
-        g_dino_checkpoint_path = "weights/GroundingDINO"
-        sam_checkpoint_path = "weights/SAM"
-        sam_type = None
-
-
-        helpers.create_hierarchy(g_dino_checkpoint_path)
-        helpers.create_hierarchy(sam_checkpoint_path)
-
-        if sam_backbone == "sam_vit_h":
-            sam_checkpoint_path = os.path.join(sam_checkpoint_path, "sam_vit_h_4b8939.pth")
-            sam_type = "vit_h"
-            if not os.path.exists(sam_checkpoint_path):
-                os.system(f"wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth")
-                os.system(f"mv sam_vit_h_4b8939.pth {sam_checkpoint_path}")
-                
-        elif sam_backbone == "sam_vit_b":
-            sam_checkpoint_path = os.path.join(sam_checkpoint_path, "sam_vit_b_01ec64.pth")
-            sam_type = "vit_b"
-
-            if not os.path.exists(sam_checkpoint_path):
-                os.system(f"wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth")
-                os.system(f"mv sam_vit_b_01ec64.pth {sam_checkpoint_path}")
-                
-        elif sam_backbone == "sam_vit_l":
-            sam_checkpoint_path = os.path.join(sam_checkpoint_path, "sam_vit_l_0b3195.pth")
-            sam_type = "vit_l"
-
-            if not os.path.exists(sam_checkpoint_path):
-                os.system(f"wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth")
-                os.system(f"mv sam_vit_l_0b3195.pth {sam_checkpoint_path}")
-
-        if g_dino_backbone == "swin_t":
-            g_dino_checkpoint_path = os.path.join(g_dino_checkpoint_path, "groundingdino_swint_ogc.pth")
-            g_dino_model_config_path = os.path.join(g_dino_model_config_path, "GroundingDINO_SwinT_OGC.py")
-            
-            if not os.path.exists(g_dino_checkpoint_path):
-                os.system(f"wget https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha/groundingdino_swint_ogc.pth")
-                os.system(f"mv groundingdino_swint_ogc.pth {g_dino_checkpoint_path}")
-
-        # Initialize models
-        self.grounding_dino_model = Model(model_config_path=g_dino_model_config_path, 
-                                          model_checkpoint_path=g_dino_checkpoint_path,
-                                          device = self.device)
-
-        sam = sam_model_registry[sam_type](checkpoint=sam_checkpoint_path)
-        sam.to(device=self.device)
-        self.sam_predictor = SamPredictor(sam)
-
-    def load_image(self, image_path):
-        return cv2.imread(image_path)
-
-
-
-    def detect_objects(self, image, classes, box_threshold=0.25, text_threshold=0.25):
-        detections = self.grounding_dino_model.predict_with_classes(
-            image=image,
-            classes=classes,
-            box_threshold=box_threshold,
-            text_threshold=text_threshold
-        )
-        return detections
-    
-    def iou(self, box1, box2):
-        """
-        Compute the Intersection over Union (IoU) of two bounding boxes.
-
-        Parameters:
-        - box1, box2 (list or np.array): Bounding boxes in the format [x1, y1, x2, y2].
-
-        Returns:
-        - float: IoU of the two bounding boxes.
-        """
-        # Coordinates of the intersection rectangle
-        x1_inter = max(box1[0], box2[0])
-        y1_inter = max(box1[1], box2[1])
-        x2_inter = min(box1[2], box2[2])
-        y2_inter = min(box1[3], box2[3])
-
-        # Compute the area of the intersection rectangle
-        inter_width = max(0, x2_inter - x1_inter + 1)
-        inter_height = max(0, y2_inter - y1_inter + 1)
-        inter_area = inter_width * inter_height
-
-        # Compute the area of both bounding boxes
-        box1_area = (box1[2] - box1[0] + 1) * (box1[3] - box1[1] + 1)
-        box2_area = (box2[2] - box2[0] + 1) * (box2[3] - box2[1] + 1)
-
-        # Compute the IoU by taking the intersection area and dividing it by the union area
-        union_area = box1_area + box2_area - inter_area
-        iou_value = inter_area / union_area
-
-        return iou_value
-
-    def nms(self, detections, nms_threshold=0.5):
-        bboxes = detections.xyxy
-        confidences = detections.confidence
-        class_ids = detections.class_id
-
-        to_drop = []
-        for i, bbox_i in enumerate(bboxes):
-            for j, bbox_j in enumerate(bboxes):
-                if i != j and class_ids[i]==class_ids[j] and self.iou(bbox_i, bbox_j) > nms_threshold:
-                    if confidences[i] > confidences[j]:
-                        to_drop.append(j)
-                    else:
-                        to_drop.append(i)
-
-        to_keep = [i for i in range(len(bboxes)) if i not in to_drop]
-        detections.xyxy = detections.xyxy[to_keep]
-        detections.confidence = detections.confidence[to_keep]
-        detections.class_id = detections.class_id[to_keep]
-
-        return detections
 
-    
-    def apply_nms(self, detections, nms_threshold=0.8):
-        
-        def first_occurrences_indices(lst):
-            seen = {}
-            indices = []
-            
-            for i, value in enumerate(lst):
-                if value not in seen:
-                    seen[value] = i
-                    indices.append(i)
-            
-            return indices
-        
-        nms_idx = torchvision.ops.nms(
-            torch.from_numpy(detections.xyxy),
-            torch.from_numpy(detections.confidence),
-            nms_threshold
-        ).numpy().tolist()
-  
-        detections.xyxy = detections.xyxy[nms_idx]
-        detections.confidence = detections.confidence[nms_idx]
-        detections.class_id = detections.class_id[nms_idx]
-        # idx = first_occurrences_indices(detections.class_id)
-
-        # detections.xyxy = detections.xyxy[idx]
-        # detections.confidence = detections.confidence[idx]
-        # detections.class_id = detections.class_id[idx]
+        self.lang_sam = LangSAM(sam_type=sam_type, ckpt_path=checkpoint_path, return_prompts=return_prompts)
+    def lang_segment(self, image_path, text_prompt, box_threshold, text_threshold):
+        image_pil = Image.open(image_path).convert("RGB")
+        masks, boxes, phrases, logits = self.lang_sam.predict(image_pil, text_prompt=text_prompt, text_threshold=text_threshold, box_threshold=box_threshold)
 
-        return detections
+        return sv.Detections(xyxy=boxes, confidence=logits, class_id=phrases, mask=masks)
     
-    def segment(self, image, xyxy):
-        self.sam_predictor.set_image(image)
-        result_masks = []
-        for box in xyxy:
-            masks, scores, logits = self.sam_predictor.predict(
-                box=box,
-                multimask_output=True
-            )
-            index = np.argmax(scores)
-            result_masks.append(masks[index])
-        return np.array(result_masks)
-
-    def annotate_image(self, image, detections, classes):
-        box_annotator = sv.BoxAnnotator()
-        mask_annotator = sv.MaskAnnotator()
-
-        confidences = detections.confidence
-        class_ids = detections.class_id
-        labels = [f"{classes[class_id]} {confidence:0.2f}" for class_id, confidence in zip(class_ids, confidences)]
-
-        annotated_image = mask_annotator.annotate(scene=image.copy(), detections=detections)
-        annotated_image = box_annotator.annotate(scene=annotated_image, detections=detections, labels=labels)
-        return annotated_image
-
-    def grounding_sam(self, source_image_path, classes, box_threshold=0.25, text_threshold=0.25, nms_threshold=0.8, output_path=None):
-        # Load image
-        image = self.load_image(source_image_path)
-
-        # Detect objects
-        detections = self.detect_objects(image, classes, box_threshold, text_threshold)
-        # Apply NMS
-        detections = self.nms(detections, nms_threshold)
-
-        # Convert detections to masks
-        detections.mask = self.segment(cv2.cvtColor(image, cv2.COLOR_BGR2RGB), detections.xyxy)
-  
-
-        # Annotate image with segmented masks
-        annotated_image = self.annotate_image(image, detections, classes)
-
-        if output_path is not None:
-            self.save_image(annotated_image, output_path)
-
-        return detections
-    
-    def aggregator(self, classes, confidences, agg=hmean):
-        """
-        Calculate the harmonic mean of confidences for each class.
-
-        Parameters:
-        - classes (np.ndarray): 1D array containing class IDs.
-        - confidences (np.ndarray): 1D array containing confidences.
-
-        Returns:
-        - np.ndarray: 2D array with class_id and their corresponding harmonic means of confidences.
-        """
-        classes = np.array(classes)
-        confidences = np.array(confidences)
-        unique_classes = np.unique(classes)
-        result = []
-
-        for cls in unique_classes:
-            class_confidences = confidences[classes == cls]
-            harmonic_mean_value = agg(class_confidences)
-            result.append([cls, harmonic_mean_value])
-
-        return np.array(result)
-
-    def create_annotation_matrix(self, dataset_path, classes, box_threshold, text_threshold, nms_threshold, agg=hmean):
+    def create_annotation_matrix(self, dataset_path, classes, box_threshold, text_threshold, agg=hmean, run=None, output_namespaces=None):
         """
         Create an annotation matrix for a dataset.
 
         Parameters:
         - dataset_path (str): Path to the dataset.
         - classes (list): List of classes.
 
@@ -254,24 +48,28 @@
         # Create a DataFrame full of zeros
         annotation_matrix = pd.DataFrame(data=np.zeros((len(image_ids), len(classes))), index=image_ids, columns=classes)
 
         for image_name in tqdm(image_ids, desc="Creating annotation matrix", unit="image"):
             image_path = os.path.join(dataset_path, image_name)
 
             # Apply the grounding SAM pipeline
-            detections = self.grounding_sam(image_path, classes, box_threshold=box_threshold, text_threshold=text_threshold, nms_threshold=nms_threshold)
+            detections = self.lang_segment(image_path, ". ".join(classes), box_threshold=box_threshold, text_threshold=text_threshold)
+            if run is not None and output_namespaces["detections"] is not None:
+                run.log_files(data = detections, namespace=os.path.join(output_namespaces["detections"], image_name), extension="pkl", wait=True)
             # Calculate the harmonic mean of confidences
             confidences = detections.confidence
             class_ids = [classes[id] for id in detections.class_id]
             harmonic_means = self.aggregator(class_ids, confidences, agg=agg)
             annotation_matrix.loc[image_name, harmonic_means[:, 0]] = harmonic_means[:, 1]
+        if run is not None and output_namespaces["annotation_matrix"] is not None:
+            run.log_dataframe(dataframe=annotation_matrix, namespace=output_namespaces["annotation_matrix"], csv_format=True, index=True, wait=True)
 
         return annotation_matrix
-    
-    def occ_proba_disjoint_tensor(self, matrix: pd.DataFrame = None, apply_on_annotation_matrix = True, **kwargs):
+
+    def occ_proba_disjoint_tensor(self, matrix: pd.DataFrame = None, apply_on_annotation_matrix = True, run=None, output_namespaces=None, **kwargs):
         """
         Calculate the occurrence probability disjoint matrix.
 
         Parameters:
         - matrix (np.ndarray): Annotation matrix with shape (num_images, num_classes).
 
         Returns:
@@ -288,36 +86,345 @@
         if apply_on_annotation_matrix:
             assert matrix is None, "Annotation matrix should not be provided."
             matrix = self.create_annotation_matrix(dataset_path=dataset_path, 
                                                    classes=classes, 
                                                    box_threshold=box_threshold, 
                                                    text_threshold=text_threshold,
                                                    nms_threshold=nms_threshold, 
-                                                   agg=agg)
+                                                   agg=agg,
+                                                   run=run,
+                                                   output_namespaces=output_namespaces)
         if annotation_matrix_processing is not None:
             matrix = annotation_matrix_processing(matrix, **annotation_matrix_processing_args)
 
         classes = matrix.columns
         num_rows, num_cols = matrix.shape
 
         tensor = np.zeros(shape=(num_cols, num_rows, num_rows))
         for i, c in enumerate(classes):
             column = matrix.loc[:, c].values
             column = np.array([float(val) for val in column]).reshape(len(column), 1)
 
             # The result is square rooted to normalize the values
-            mat = np.sqrt(column * column.T)
-            
+            mat = np.sqrt(column * column.T)       
             tensor[i] = mat
+        if run is not None and output_namespaces["adjacency_tensor"] is not None:
+            run.log_files(data=tensor, namespace=output_namespaces["adjacency_tensor"], extension="pkl", wait=True)
+
+        return {"adjacency_tensor" : tensor, "index": matrix.index, "columns": classes, "annotation_matrix": matrix}
+
+
+# seg = SegmentationManager()
+# class SegmentationManager:
+#     def __init__(self, sam_backbone="sam_vit_h", g_dino_backbone="swin_t", device=DEVICE):
+#         self.device = device
+        
+#         # Paths for checkpoints and configs
+#         g_dino_model_config_path = "GroundingDINO/groundingdino/config"
+#         g_dino_checkpoint_path = "weights/GroundingDINO"
+#         sam_checkpoint_path = "weights/SAM"
+#         sam_type = None
+
+
+#         helpers.create_hierarchy(g_dino_checkpoint_path)
+#         helpers.create_hierarchy(sam_checkpoint_path)
+
+#         if sam_backbone == "sam_vit_h":
+#             sam_checkpoint_path = os.path.join(sam_checkpoint_path, "sam_vit_h_4b8939.pth")
+#             sam_type = "vit_h"
+#             if not os.path.exists(sam_checkpoint_path):
+#                 os.system(f"wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth")
+#                 os.system(f"mv sam_vit_h_4b8939.pth {sam_checkpoint_path}")
+                
+#         elif sam_backbone == "sam_vit_b":
+#             sam_checkpoint_path = os.path.join(sam_checkpoint_path, "sam_vit_b_01ec64.pth")
+#             sam_type = "vit_b"
+
+#             if not os.path.exists(sam_checkpoint_path):
+#                 os.system(f"wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth")
+#                 os.system(f"mv sam_vit_b_01ec64.pth {sam_checkpoint_path}")
+                
+#         elif sam_backbone == "sam_vit_l":
+#             sam_checkpoint_path = os.path.join(sam_checkpoint_path, "sam_vit_l_0b3195.pth")
+#             sam_type = "vit_l"
+
+#             if not os.path.exists(sam_checkpoint_path):
+#                 os.system(f"wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth")
+#                 os.system(f"mv sam_vit_l_0b3195.pth {sam_checkpoint_path}")
+
+#         if g_dino_backbone == "swin_t":
+#             config_name = "GroundingDINO_SwinT_OGC.py"
+#             g_dino_checkpoint_path = os.path.join(g_dino_checkpoint_path, "groundingdino_swint_ogc.pth")
+#             g_dino_model_config_path = os.path.join(g_dino_model_config_path, config_name)
+
+
+#             if not os.path.exists(g_dino_checkpoint_path):
+#                 os.system(f"wget https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha/groundingdino_swint_ogc.pth")
+#                 os.system(f"mv groundingdino_swint_ogc.pth {g_dino_checkpoint_path}")
+
+#         # Initialize models
+#         self.grounding_dino_model = Model(model_config_path=g_dino_model_config_path, 
+#                                           model_checkpoint_path=g_dino_checkpoint_path,
+#                                           device = self.device)
+
+#         sam = sam_model_registry[sam_type](checkpoint=sam_checkpoint_path)
+#         sam.to(device=self.device)
+#         self.sam_predictor = SamPredictor(sam)
+
+#     def load_image(self, image_path):
+#         return cv2.imread(image_path)
+
+
+
+#     def detect_objects(self, image, classes, box_threshold=0.25, text_threshold=0.25):
+#         detections = self.grounding_dino_model.predict_with_classes(
+#             image=image,
+#             classes=classes,
+#             box_threshold=box_threshold,
+#             text_threshold=text_threshold
+#         )
+#         return detections
+    
+#     def iou(self, box1, box2):
+#         """
+#         Compute the Intersection over Union (IoU) of two bounding boxes.
+
+#         Parameters:
+#         - box1, box2 (list or np.array): Bounding boxes in the format [x1, y1, x2, y2].
+
+#         Returns:
+#         - float: IoU of the two bounding boxes.
+#         """
+#         # Coordinates of the intersection rectangle
+#         x1_inter = max(box1[0], box2[0])
+#         y1_inter = max(box1[1], box2[1])
+#         x2_inter = min(box1[2], box2[2])
+#         y2_inter = min(box1[3], box2[3])
+
+#         # Compute the area of the intersection rectangle
+#         inter_width = max(0, x2_inter - x1_inter + 1)
+#         inter_height = max(0, y2_inter - y1_inter + 1)
+#         inter_area = inter_width * inter_height
+
+#         # Compute the area of both bounding boxes
+#         box1_area = (box1[2] - box1[0] + 1) * (box1[3] - box1[1] + 1)
+#         box2_area = (box2[2] - box2[0] + 1) * (box2[3] - box2[1] + 1)
+
+#         # Compute the IoU by taking the intersection area and dividing it by the union area
+#         union_area = box1_area + box2_area - inter_area
+#         iou_value = inter_area / union_area
+
+#         return iou_value
+
+#     def nms(self, detections, nms_threshold=0.5):
+#         bboxes = detections.xyxy
+#         confidences = detections.confidence
+#         class_ids = detections.class_id
+
+#         to_drop = []
+#         for i, bbox_i in enumerate(bboxes):
+#             for j, bbox_j in enumerate(bboxes):
+#                 if i != j and class_ids[i]==class_ids[j] and self.iou(bbox_i, bbox_j) > nms_threshold:
+#                     if confidences[i] > confidences[j]:
+#                         to_drop.append(j)
+#                     else:
+#                         to_drop.append(i)
+
+#         to_keep = [i for i in range(len(bboxes)) if i not in to_drop]
+#         detections.xyxy = detections.xyxy[to_keep]
+#         detections.confidence = detections.confidence[to_keep]
+#         detections.class_id = detections.class_id[to_keep]
+
+#         return detections
 
-        return tensor, matrix.index, classes
     
+#     def apply_nms(self, detections, nms_threshold=0.8):
+        
+#         def first_occurrences_indices(lst):
+#             seen = {}
+#             indices = []
+            
+#             for i, value in enumerate(lst):
+#                 if value not in seen:
+#                     seen[value] = i
+#                     indices.append(i)
+            
+#             return indices
+        
+#         nms_idx = torchvision.ops.nms(
+#             torch.from_numpy(detections.xyxy),
+#             torch.from_numpy(detections.confidence),
+#             nms_threshold
+#         ).numpy().tolist()
+  
+#         detections.xyxy = detections.xyxy[nms_idx]
+#         detections.confidence = detections.confidence[nms_idx]
+#         detections.class_id = detections.class_id[nms_idx]
+#         # idx = first_occurrences_indices(detections.class_id)
+
+#         # detections.xyxy = detections.xyxy[idx]
+#         # detections.confidence = detections.confidence[idx]
+#         # detections.class_id = detections.class_id[idx]
+
+#         return detections
     
-    def save_image(self, image, path):
-        cv2.imwrite(path, image)
+#     def segment(self, image, xyxy):
+#         self.sam_predictor.set_image(image)
+#         result_masks = []
+#         for box in xyxy:
+#             masks, scores, logits = self.sam_predictor.predict(
+#                 box=box,
+#                 multimask_output=True
+#             )
+#             index = np.argmax(scores)
+#             result_masks.append(masks[index])
+#         return np.array(result_masks)
+
+#     def annotate_image(self, image, detections, classes):
+#         box_annotator = sv.BoxAnnotator()
+#         mask_annotator = sv.MaskAnnotator()
+
+#         confidences = detections.confidence
+#         class_ids = detections.class_id
+#         labels = [f"{classes[class_id]} {confidence:0.2f}" for class_id, confidence in zip(class_ids, confidences)]
+
+#         annotated_image = mask_annotator.annotate(scene=image.copy(), detections=detections)
+#         annotated_image = box_annotator.annotate(scene=annotated_image, detections=detections, labels=labels)
+#         return annotated_image
+
+#     def grounding_sam(self, source_image_path, classes, box_threshold=0.25, text_threshold=0.25, nms_threshold=0.8, output_path=None):
+#         # Load image
+#         image = self.load_image(source_image_path)
+
+#         # Detect objects
+#         detections = self.detect_objects(image, classes, box_threshold, text_threshold)
+#         # Apply NMS
+#         detections = self.nms(detections, nms_threshold)
+
+#         # Convert detections to masks
+#         detections.mask = self.segment(cv2.cvtColor(image, cv2.COLOR_BGR2RGB), detections.xyxy)
+  
+
+#         # Annotate image with segmented masks
+#         annotated_image = self.annotate_image(image, detections, classes)
+
+#         if output_path is not None:
+#             self.save_image(annotated_image, output_path)
+
+#         return detections
+    
+#     def aggregator(self, classes, confidences, agg=hmean):
+#         """
+#         Calculate the harmonic mean of confidences for each class.
+
+#         Parameters:
+#         - classes (np.ndarray): 1D array containing class IDs.
+#         - confidences (np.ndarray): 1D array containing confidences.
+
+#         Returns:
+#         - np.ndarray: 2D array with class_id and their corresponding harmonic means of confidences.
+#         """
+#         classes = np.array(classes)
+#         confidences = np.array(confidences)
+#         unique_classes = np.unique(classes)
+#         result = []
+
+#         for cls in unique_classes:
+#             class_confidences = confidences[classes == cls]
+#             harmonic_mean_value = agg(class_confidences)
+#             result.append([cls, harmonic_mean_value])
+
+#         return np.array(result)
+
+#     def create_annotation_matrix(self, dataset_path, classes, box_threshold, text_threshold, nms_threshold, agg=hmean, run=None, output_namespaces=None):
+#         """
+#         Create an annotation matrix for a dataset.
+
+#         Parameters:
+#         - dataset_path (str): Path to the dataset.
+#         - classes (list): List of classes.
+
+#         Returns:
+#         - np.ndarray: Annotation matrix with shape (num_images, num_classes).
+#         """
+#         # Import image base paths
+#         image_ids = sorted(os.listdir(dataset_path))
+
+#         # Create a DataFrame full of zeros
+#         annotation_matrix = pd.DataFrame(data=np.zeros((len(image_ids), len(classes))), index=image_ids, columns=classes)
+
+#         for image_name in tqdm(image_ids, desc="Creating annotation matrix", unit="image"):
+#             image_path = os.path.join(dataset_path, image_name)
+
+#             # Apply the grounding SAM pipeline
+#             detections = self.grounding_sam(image_path, classes, box_threshold=box_threshold, text_threshold=text_threshold, nms_threshold=nms_threshold)
+#             if run is not None and output_namespaces["detections"] is not None:
+#                 run.log_files(data = detections, namespace=os.path.join(output_namespaces["detections"], image_name), extension="pkl", wait=True)
+#             # Calculate the harmonic mean of confidences
+#             confidences = detections.confidence
+#             class_ids = [classes[id] for id in detections.class_id]
+#             harmonic_means = self.aggregator(class_ids, confidences, agg=agg)
+#             annotation_matrix.loc[image_name, harmonic_means[:, 0]] = harmonic_means[:, 1]
+#         if run is not None and output_namespaces["annotation_matrix"] is not None:
+#             run.log_dataframe(dataframe=annotation_matrix, namespace=output_namespaces["annotation_matrix"], csv_format=True, index=True, wait=True)
+
+#         return annotation_matrix
+    
+#     def occ_proba_disjoint_tensor(self, matrix: pd.DataFrame = None, apply_on_annotation_matrix = True, run=None, output_namespaces=None, **kwargs):
+#         """
+#         Calculate the occurrence probability disjoint matrix.
+
+#         Parameters:
+#         - matrix (np.ndarray): Annotation matrix with shape (num_images, num_classes).
+
+#         Returns:
+#         - np.ndarray: Occurrence probability disjoint matrix with shape (num_classes, num_classes).
+#         """
+#         dataset_path = kwargs.get("dataset_path", None)
+#         classes = kwargs.get("classes", None)
+#         box_threshold = kwargs.get("box_threshold", 0.25)
+#         text_threshold = kwargs.get("text_threshold", 0.25)
+#         nms_threshold = kwargs.get("nms_threshold", 0.8)
+#         agg = kwargs.get("agg", hmean)
+#         annotation_matrix_processing = kwargs.get("annotation_matrix_processing", None)
+#         annotation_matrix_processing_args = kwargs.get("annotation_matrix_processing_args", {})
+#         if apply_on_annotation_matrix:
+#             assert matrix is None, "Annotation matrix should not be provided."
+#             matrix = self.create_annotation_matrix(dataset_path=dataset_path, 
+#                                                    classes=classes, 
+#                                                    box_threshold=box_threshold, 
+#                                                    text_threshold=text_threshold,
+#                                                    nms_threshold=nms_threshold, 
+#                                                    agg=agg,
+#                                                    run=run,
+#                                                    output_namespaces=output_namespaces)
+#         if annotation_matrix_processing is not None:
+#             matrix = annotation_matrix_processing(matrix, **annotation_matrix_processing_args)
+
+#         classes = matrix.columns
+#         num_rows, num_cols = matrix.shape
+
+#         tensor = np.zeros(shape=(num_cols, num_rows, num_rows))
+#         for i, c in enumerate(classes):
+#             column = matrix.loc[:, c].values
+#             column = np.array([float(val) for val in column]).reshape(len(column), 1)
+
+#             # The result is square rooted to normalize the values
+#             mat = np.sqrt(column * column.T)       
+#             tensor[i] = mat
+#         if run is not None and output_namespaces["adjacency_tensor"] is not None:
+#             run.log_files(data=tensor, namespace=output_namespaces["adjacency_tensor"], extension="pkl", wait=True)
+
+#         return {"adjacency_tensor" : tensor, "index": matrix.index, "columns": classes, "annotation_matrix": matrix}
+    
+#     def lang_sam(self):
+#         pass
+
+#     def save_image(self, image, path):
+#         cv2.imwrite(path, image)
         
 # # # Example usage
 # if __name__ == "__main__":
 #     SOURCE_IMAGE_PATH = "G0041951.JPG"
 #     CLASSES = ["person", "banner", "finger", "hand", "foot", "glasses", "desert", "sky", "clouds"]
 #     BOX_THRESHOLD = 0.3
 #     TEXT_THRESHOLD = 0.25
```

### Comparing `torch_model_manager-0.4.0.dev9/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.1.dev1/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev9/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.1.dev1/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev9
+Version: 0.4.1.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev9/utils/helpers.py` & `torch_model_manager-0.4.1.dev1/utils/helpers.py`

 * *Files identical despite different names*

