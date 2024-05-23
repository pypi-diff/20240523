# Comparing `tmp/deepfusion-0.0.1-py3-none-any.whl.zip` & `tmp/deepfusion-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5865 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1090 b- defN 24-May-23 08:30 deepfusion-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    10857 b- defN 24-May-23 08:30 deepfusion-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 08:30 deepfusion-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-May-23 08:30 deepfusion-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      401 b- defN 24-May-23 08:30 deepfusion-0.0.1.dist-info/RECORD
-5 files, 12441 bytes uncompressed, 5115 bytes compressed:  58.9%
+Zip file size: 5867 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-May-23 08:45 deepfusion-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    10864 b- defN 24-May-23 08:45 deepfusion-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 08:45 deepfusion-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-May-23 08:45 deepfusion-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      401 b- defN 24-May-23 08:45 deepfusion-0.0.2.dist-info/RECORD
+5 files, 12448 bytes uncompressed, 5117 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: deepfusion-0.0.1.dist-info/LICENSE
+Filename: deepfusion-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: deepfusion-0.0.1.dist-info/METADATA
+Filename: deepfusion-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: deepfusion-0.0.1.dist-info/WHEEL
+Filename: deepfusion-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: deepfusion-0.0.1.dist-info/top_level.txt
+Filename: deepfusion-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: deepfusion-0.0.1.dist-info/RECORD
+Filename: deepfusion-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `deepfusion-0.0.1.dist-info/LICENSE` & `deepfusion-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `deepfusion-0.0.1.dist-info/METADATA` & `deepfusion-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfusion
-Version: 0.0.1
+Version: 0.0.2
 Summary: DeepFusion is a highly modular and customizable deep learning framework!
 Home-page: https://github.com/atharvaaalok/deepfusion
 Author: Atharva Aalok
 Author-email: atharvaaalok@gmail.com
 License: MIT
 Keywords: deepfusion,deep learning,neural networks,artificial intelligence,machine learning,model,optimization,backpropagation
 Description-Content-Type: text/markdown
@@ -62,14 +62,15 @@
 
 `Data` objects hold the network activations and `Module` objects perform operations on them. The
 `Net` object forms a thin wrapper around the `Data` and `Module` objects and is used to perform
 the forward and backward passes.
 
 A simple neural network is shown below, where, ellipses represent `Data` objects and rectangles
 represent `Module`.
+
 ![Basic Neural Network](https://raw.githubusercontent.com/atharvaaalok/deepfusion/main/assets/readme_assets/Basic_NeuralNetwork.svg)
 
 > Note the alternating sequence of `Data` and `Module`. The scheme is `Data` -> `Module` -> `Data`.
 > Red represents nodes with updatable parameters.
 
 Every node (`Data` or `Module`) has a unique *ID* (for eg: z1 or MatMul1) using which it can be
 accessed and modified thus providing explicit access and control over all data and parameters.
@@ -153,27 +154,29 @@
 directory or in other [resources](#resources).
 
 To have a look at the codebase tree have a look at [Codebase Tree](./assets/codebase_tree.txt).
 
 
 ## Highlights
 ### 1. Customizable training
-Let's say we make the simple neural network as before
+Let's say we make the simple neural network as before:
+
 ![Basic Neural Network](https://raw.githubusercontent.com/atharvaaalok/deepfusion/main/assets/readme_assets/Basic_NeuralNetwork.svg)
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
+
 ![Basic Neural Network](https://raw.githubusercontent.com/atharvaaalok/deepfusion/main/assets/readme_assets/Basic_NN_unfrozen_input.svg)
 Now when we train the network only the input node value will get updates and be trained!
 
 ### 2. Gradient Checking
 When developing new modules, the implementation of the backward pass can often be tricky and have
 subtle bugs. Deepfusion provides a gradient checking utility that can find the derivatives of the
 loss function(s) w.r.t. any specified data object (data node or module parameter). Eg:
```

