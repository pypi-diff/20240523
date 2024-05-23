# Comparing `tmp/deepfusion-0.0.0-py3-none-any.whl.zip` & `tmp/deepfusion-0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5859 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1090 b- defN 24-May-23 07:00 deepfusion-0.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    10592 b- defN 24-May-23 07:00 deepfusion-0.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 07:00 deepfusion-0.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-May-23 07:00 deepfusion-0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      401 b- defN 24-May-23 07:00 deepfusion-0.0.0.dist-info/RECORD
-5 files, 12176 bytes uncompressed, 5109 bytes compressed:  58.0%
+Zip file size: 5865 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-May-23 08:30 deepfusion-0.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    10857 b- defN 24-May-23 08:30 deepfusion-0.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 08:30 deepfusion-0.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-May-23 08:30 deepfusion-0.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      401 b- defN 24-May-23 08:30 deepfusion-0.0.1.dist-info/RECORD
+5 files, 12441 bytes uncompressed, 5115 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: deepfusion-0.0.0.dist-info/LICENSE
+Filename: deepfusion-0.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: deepfusion-0.0.0.dist-info/METADATA
+Filename: deepfusion-0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: deepfusion-0.0.0.dist-info/WHEEL
+Filename: deepfusion-0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: deepfusion-0.0.0.dist-info/top_level.txt
+Filename: deepfusion-0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: deepfusion-0.0.0.dist-info/RECORD
+Filename: deepfusion-0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `deepfusion-0.0.0.dist-info/LICENSE` & `deepfusion-0.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `deepfusion-0.0.0.dist-info/METADATA` & `deepfusion-0.0.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfusion
-Version: 0.0.0
+Version: 0.0.1
 Summary: DeepFusion is a highly modular and customizable deep learning framework!
 Home-page: https://github.com/atharvaaalok/deepfusion
 Author: Atharva Aalok
 Author-email: atharvaaalok@gmail.com
 License: MIT
 Keywords: deepfusion,deep learning,neural networks,artificial intelligence,machine learning,model,optimization,backpropagation
 Description-Content-Type: text/markdown
@@ -16,18 +16,18 @@
 Provides-Extra: gpu
 Requires-Dist: cupy-cuda12x ==13.1.0 ; extra == 'gpu'
 Provides-Extra: visualization
 Requires-Dist: graphviz ==0.20.3 ; extra == 'visualization'
 
 <div align="center">
     <picture>
-        <source media="(prefers-color-scheme: light)" srcset="./assets/logos/Light_TextRight.svg">
-        <source media="(prefers-color-scheme: dark)" srcset="./assets/logos/Dark_TextBelow.svg">
+        <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/atharvaaalok/deepfusion/main/assets/logos/Light_TextRight.svg">
+        <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/atharvaaalok/deepfusion/main/assets/logos/Dark_TextRight.svg">
         <img alt="DeepFusion Logo with text below it. Displays the light version in light mode and
-        the dark version logo in dark mode." src="./assets/logos/Light_TextBelow.svg" width="100%">
+        the dark version logo in dark mode." src="https://raw.githubusercontent.com/atharvaaalok/deepfusion/main/assets/logos/Light_TextRight.svg" width="100%">
     </picture>
 </div>
 
 <br>
 
 DeepFusion is a highly modular and customizable deep learning framework.
 
@@ -62,15 +62,15 @@
 
 `Data` objects hold the network activations and `Module` objects perform operations on them. The
 `Net` object forms a thin wrapper around the `Data` and `Module` objects and is used to perform
 the forward and backward passes.
 
 A simple neural network is shown below, where, ellipses represent `Data` objects and rectangles
 represent `Module`.
-![Basic Neural Network](./assets/readme_assets/Basic_NeuralNetwork.svg)
+![Basic Neural Network](https://raw.githubusercontent.com/atharvaaalok/deepfusion/main/assets/readme_assets/Basic_NeuralNetwork.svg)
 
 > Note the alternating sequence of `Data` and `Module`. The scheme is `Data` -> `Module` -> `Data`.
 > Red represents nodes with updatable parameters.
 
 Every node (`Data` or `Module`) has a unique *ID* (for eg: z1 or MatMul1) using which it can be
 accessed and modified thus providing explicit access and control over all data and parameters.
 
@@ -87,21 +87,21 @@
 - `Data`
 - `Module`
 - `Net`
 
 The codebase follows the same intuitive structure:
 ```
 deepfusion
-â””â”€â”€ components
-    â”œâ”€â”€ net
-    â”œâ”€â”€ data
-    â””â”€â”€ modules
-        â”œâ”€â”€ activation_functions
-        â”œâ”€â”€ loss_functions
-        â””â”€â”€ matmul.py
+└── components
+    ├── net
+    ├── data
+    └── modules
+        ├── activation_functions
+        ├── loss_functions
+        └── matmul.py
 ```
 
 To construct a neural network we need to import the `Net`, `Data` and required `Module` objects.
 ```python
 # Import Net, Data and necessary Modules
 from deepfusion.components.net import Net
 from deepfusion.components.data import Data
@@ -154,27 +154,27 @@
 
 To have a look at the codebase tree have a look at [Codebase Tree](./assets/codebase_tree.txt).
 
 
 ## Highlights
 ### 1. Customizable training
 Let's say we make the simple neural network as before
-![Basic Neural Network](./assets/readme_assets/Basic_NeuralNetwork.svg)
+![Basic Neural Network](https://raw.githubusercontent.com/atharvaaalok/deepfusion/main/assets/readme_assets/Basic_NeuralNetwork.svg)
 And train it. During training only the *red* portions of the network receive updates and are
 trained. Therefore, the matrix multiplication modules will be trained.
 
 Let's say we have trained the network and now we want to find the input that optimizes the function
 that we have learnt. This also falls under the same forward-backward-update procedure with the
 following simple twist:
 ```python
 net.freeze() # Freezes all modules
 x.unfreeze() # Unfreezes the input node
 ```
 After this we obtain the following network:
-![Basic Neural Network](./assets/readme_assets/Basic_NN_unfrozen_input.svg)
+![Basic Neural Network](https://raw.githubusercontent.com/atharvaaalok/deepfusion/main/assets/readme_assets/Basic_NN_unfrozen_input.svg)
 Now when we train the network only the input node value will get updates and be trained!
 
 ### 2. Gradient Checking
 When developing new modules, the implementation of the backward pass can often be tricky and have
 subtle bugs. Deepfusion provides a gradient checking utility that can find the derivatives of the
 loss function(s) w.r.t. any specified data object (data node or module parameter). Eg:
 ```python
```

