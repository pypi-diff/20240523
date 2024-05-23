# Comparing `tmp/nlpx-0.2.1.tar.gz` & `tmp/nlpx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-0.2.1.tar", last modified: Thu May 23 00:31:58 2024, max compression
+gzip compressed data, was "nlpx-0.3.0.tar", last modified: Thu May 23 00:45:35 2024, max compression
```

## Comparing `nlpx-0.2.1.tar` & `nlpx-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 00:31:58.669281 nlpx-0.2.1/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-23 00:31:58.668810 nlpx-0.2.1/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.2.1/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 00:31:58.662931 nlpx-0.2.1/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.2.1/nlpx/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2091 2024-05-21 12:03:46.000000 nlpx-0.2.1/nlpx/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)       30 2024-05-23 00:31:50.000000 nlpx-0.2.1/nlpx/models.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.2.1/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 00:31:58.668084 nlpx-0.2.1/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-23 00:31:58.000000 nlpx-0.2.1/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      227 2024-05-23 00:31:58.000000 nlpx-0.2.1/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-23 00:31:58.000000 nlpx-0.2.1/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-23 00:31:58.000000 nlpx-0.2.1/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-23 00:31:58.000000 nlpx-0.2.1/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-23 00:31:58.669492 nlpx-0.2.1/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      998 2024-05-23 00:31:50.000000 nlpx-0.2.1/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 00:45:35.503932 nlpx-0.3.0/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-23 00:45:35.501892 nlpx-0.3.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.3.0/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 00:45:35.494891 nlpx-0.3.0/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.3.0/nlpx/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2095 2024-05-23 00:44:38.000000 nlpx-0.3.0/nlpx/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)       30 2024-05-23 00:31:50.000000 nlpx-0.3.0/nlpx/models.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.3.0/nlpx/text_token.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 00:45:35.500772 nlpx-0.3.0/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-23 00:45:35.000000 nlpx-0.3.0/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      227 2024-05-23 00:45:35.000000 nlpx-0.3.0/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-23 00:45:35.000000 nlpx-0.3.0/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-23 00:45:35.000000 nlpx-0.3.0/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-23 00:45:35.000000 nlpx-0.3.0/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-23 00:45:35.504456 nlpx-0.3.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      998 2024-05-23 00:45:30.000000 nlpx-0.3.0/setup.py
```

### Comparing `nlpx-0.2.1/PKG-INFO` & `nlpx-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.2.1
+Version: 0.3.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-0.2.1/nlpx/_text_cnn.py` & `nlpx-0.3.0/nlpx/_text_cnn.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 from typing import Collection
 from torch import nn
 from torch.nn import functional as F
 
 
 class TextCNN(nn.Module):
 
-    def __init__(self, word_dim: int, cnn_out_channels: int, cnn_kernel_sizes: Collection[int], num_classes: int,
+    def __init__(self, word_dim: int, cnn_out_channels: int, cnn_kernel_sizes: Collection[int], out_features: int,
                  drop_out=None):
         """ TextCNN model
         Parameters
         ----------
         word_dim:
         cnn_out_channels:
         cnn_kernel_sizes:
-        num_classes:
+        out_features:
         drop_out:
 
         Examples
         --------
         >>> import torch
         >>> from nlpx.models import TextCNN
         >>> X = torch.randn(batch_size, 10, word_dim)
         >>> targets = torch.randint(0, num_classes, (batch_size,))
-        >>> model = TextCNN(word_dim, cnn_out_channels=64, cnn_kernel_sizes=(2, 3, 4), num_classes=num_classes)
+        >>> model = TextCNN(word_dim, cnn_out_channels=64, cnn_kernel_sizes=(2, 3, 4), out_features=num_classes)
         >>> output = model(X)
         >>> loss, output = model(X, targets)
         """
         super().__init__()
         self.convs = nn.ModuleList([
             nn.Sequential(
                 nn.Conv1d(in_channels=word_dim, out_channels=cnn_out_channels, kernel_size=kernel_size, bias=False),
                 nn.ReLU(inplace=True),  # inplace为True，将会改变输入的数据 ，否则不会改变原输入，只会产生新的输出
                 nn.AdaptiveMaxPool1d(1)
             ) for kernel_size in cnn_kernel_sizes
         ])
-        self.fc = nn.Linear(in_features=cnn_out_channels * len(cnn_kernel_sizes), out_features=num_classes)
+        self.fc = nn.Linear(in_features=cnn_out_channels * len(cnn_kernel_sizes), out_features=out_features)
         self.dropout = nn.Dropout(drop_out) if drop_out else None
 
     def forward(self, inputs, labels=None):
         """
         :param inputs: [(batch, sentence, word_dim)]
         :param labels: [long]
         """
```

### Comparing `nlpx-0.2.1/nlpx/text_token.py` & `nlpx-0.3.0/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-0.2.1/nlpx.egg-info/PKG-INFO` & `nlpx-0.3.0/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.2.1
+Version: 0.3.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-0.2.1/setup.py` & `nlpx-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.2.1',
+    version='0.3.0',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

