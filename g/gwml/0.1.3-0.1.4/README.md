# Comparing `tmp/gwml-0.1.3-py3-none-any.whl.zip` & `tmp/gwml-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 98474 bytes, number of entries: 63
+Zip file size: 98478 bytes, number of entries: 63
 -rw-r--r--  2.0 unx        0 b- defN 24-May-14 09:40 gwml/__init__.py
 -rw-r--r--  2.0 unx     1521 b- defN 24-May-16 05:28 gwml/_command.py
 -rw-r--r--  2.0 unx      206 b- defN 24-May-16 05:31 gwml/_main.py
--rw-r--r--  2.0 unx     6090 b- defN 24-May-23 02:10 gwml/command.py
+-rw-r--r--  2.0 unx     6108 b- defN 24-May-23 02:12 gwml/command.py
 -rw-r--r--  2.0 unx      797 b- defN 24-May-22 09:19 gwml/main.py
 -rw-r--r--  2.0 unx      104 b- defN 24-May-16 05:28 gwml/mldump.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-22 09:12 gwml/cmdLib/__init__.py
 -rw-r--r--  2.0 unx     2437 b- defN 24-May-22 09:16 gwml/cmdLib/envCollector.py
 -rw-r--r--  2.0 unx     2233 b- defN 24-May-22 09:16 gwml/cmdLib/getHyperParam.py
 -rw-r--r--  2.0 unx     1818 b- defN 24-May-22 09:16 gwml/cmdLib/getLagacyFile.py
 -rw-r--r--  2.0 unx     3858 b- defN 24-May-23 02:02 gwml/cmdLib/organizeModel.py
@@ -53,13 +53,13 @@
 -rw-r--r--  2.0 unx       22 b- defN 24-May-16 05:48 gwml/lib/common/trainer/__init__.py
 -rw-r--r--  2.0 unx    11894 b- defN 24-May-16 06:40 gwml/lib/common/trainer/customTrainer.py
 -rw-r--r--  2.0 unx    10834 b- defN 24-May-16 05:48 gwml/lib/common/trainer/regTrainer.py
 -rw-r--r--  2.0 unx     2317 b- defN 24-May-16 05:48 gwml/lib/common/utils/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-16 06:46 gwml/lib/reg/__init__.py
 -rw-r--r--  2.0 unx     5131 b- defN 24-May-16 06:41 gwml/lib/reg/regDecorator.py
 -rw-r--r--  2.0 unx    24563 b- defN 24-May-16 06:42 gwml/lib/reg/regTrainer.py
--rw-r--r--  2.0 unx       49 b- defN 24-May-23 02:10 gwml-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-23 02:10 gwml-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 24-May-23 02:10 gwml-0.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-May-23 02:10 gwml-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     5519 b- defN 24-May-23 02:10 gwml-0.1.3.dist-info/RECORD
-63 files, 321701 bytes uncompressed, 89598 bytes compressed:  72.1%
+-rw-r--r--  2.0 unx       49 b- defN 24-May-23 02:12 gwml-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-23 02:12 gwml-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 24-May-23 02:12 gwml-0.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-May-23 02:12 gwml-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5519 b- defN 24-May-23 02:12 gwml-0.1.4.dist-info/RECORD
+63 files, 321719 bytes uncompressed, 89602 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -168,23 +168,23 @@
 
 Filename: gwml/lib/reg/regDecorator.py
 Comment: 
 
 Filename: gwml/lib/reg/regTrainer.py
 Comment: 
 
-Filename: gwml-0.1.3.dist-info/METADATA
+Filename: gwml-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: gwml-0.1.3.dist-info/WHEEL
+Filename: gwml-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: gwml-0.1.3.dist-info/entry_points.txt
+Filename: gwml-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: gwml-0.1.3.dist-info/top_level.txt
+Filename: gwml-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: gwml-0.1.3.dist-info/RECORD
+Filename: gwml-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gwml/command.py

```diff
@@ -152,15 +152,15 @@
     output_filename = "model.tar.gz"
 
     organizer = ModelOrganizer(base_directory)
     organizer.organize_and_compress(
         output_filename, opt["purposeType"] + ".py", modelInfo, opt["hpoOpt"]
     )
 
-    sendData = {"modelName": opt["environment"]}
+    sendData = {"modelName": opt["environment"], "trainTf": False}
     mhResult = send_post_request(
         response["systemInfo"]["mhUrl"],
         os.path.join("./", output_filename),
         sendData,
         response["jwt"],
     )
     print(mhResult)
```

## Comparing `gwml-0.1.3.dist-info/RECORD` & `gwml-0.1.4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 gwml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gwml/_command.py,sha256=TaBIi24kTzCexXpTyxsbaFYmT5rVavItqnMh1RZI-8A,1521
 gwml/_main.py,sha256=jTS67aubfEs7U4uCU7a7gWlOllWm0AUjfvVKiXSIQEs,206
-gwml/command.py,sha256=B1dWMIos5N7NwwCxVixEqqkOTcehY5Fzlv3GfhiRMeU,6090
+gwml/command.py,sha256=sWeNlI8dFVlveGCNBWPAG1i_2XXU05uSCThGEYtqHA4,6108
 gwml/main.py,sha256=pbAVfTZVkl5MQHcLA314CLwlAvNEjCwPm0uMobaRG8w,797
 gwml/mldump.py,sha256=BhfNWnOwFqjgwkH7CPDDwL4FfA1L-QKGvD4u5lKzhCA,104
 gwml/cmdLib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gwml/cmdLib/envCollector.py,sha256=QNRM6w69zpac7IHmn3SIVcn-5EKUfmaEtb_BUAbReR0,2437
 gwml/cmdLib/getHyperParam.py,sha256=3Yj28_WM759mx3jAzfHRpjWdYbYn-HYU3Q0eFyHq8qQ,2233
 gwml/cmdLib/getLagacyFile.py,sha256=LLzHq9j56jI6ZBC4_zxQ6iGiYfgiThDrguNytwOm00o,1818
 gwml/cmdLib/organizeModel.py,sha256=0eQxzAjUf8Rr0TAJyCUiUsFdwJFl3gD1Q43LvJHcnF4,3858
@@ -52,12 +52,12 @@
 gwml/lib/common/trainer/__init__.py,sha256=46Yjk3fz9o8aTN8E95McnzpJcjGzVJmHmQqUZ5mXzfc,22
 gwml/lib/common/trainer/customTrainer.py,sha256=05rWhPyD0xcbBV8FTkHBR2igBlEZPOfyyJhekcjuzUQ,11894
 gwml/lib/common/trainer/regTrainer.py,sha256=BXupe-vk72dLZ0Bp8NZq5O2bJ4sHVYQVeFg-SDQyOfw,10834
 gwml/lib/common/utils/utils.py,sha256=auXrdDqukRQnAOsRBAxioLvsocyniZeoh3eGjnZlrsA,2317
 gwml/lib/reg/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gwml/lib/reg/regDecorator.py,sha256=lkN5pxnutUvjWjk44Uz1w3QGCSVYuYZirSCrIL7VlSQ,5131
 gwml/lib/reg/regTrainer.py,sha256=6Qv1ploKZpGGCpEu4_7k4zLaEaAUOv8IrTuVMOoddvk,24563
-gwml-0.1.3.dist-info/METADATA,sha256=PliZLb4_2loegVGuiwTeGfyR-UafoX2gVmOtzp26qkc,49
-gwml-0.1.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-gwml-0.1.3.dist-info/entry_points.txt,sha256=imL6Gb7yRsNcKwqqUM7kpMULMW5smUSYZSX7i_BVdmo,40
-gwml-0.1.3.dist-info/top_level.txt,sha256=-Ib3RiOMqlhiZ_idfsP2Unxpw70_Lzk5xN0I7vWHuAQ,5
-gwml-0.1.3.dist-info/RECORD,,
+gwml-0.1.4.dist-info/METADATA,sha256=MYJLcQe51WabrFMyNAmAE9ay7xx_jHPge7lgFtR_KqE,49
+gwml-0.1.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+gwml-0.1.4.dist-info/entry_points.txt,sha256=imL6Gb7yRsNcKwqqUM7kpMULMW5smUSYZSX7i_BVdmo,40
+gwml-0.1.4.dist-info/top_level.txt,sha256=-Ib3RiOMqlhiZ_idfsP2Unxpw70_Lzk5xN0I7vWHuAQ,5
+gwml-0.1.4.dist-info/RECORD,,
```

