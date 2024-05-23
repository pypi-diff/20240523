# Comparing `tmp/loadupch-0.0.0-py3-none-any.whl.zip` & `tmp/loadupch-0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,10 @@
-Zip file size: 20695 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat       26 b- defN 24-May-23 18:29 loaderch/__init__.py
--rw-rw-rw-  2.0 fat       97 b- defN 24-May-23 18:29 loaderch/__main__.py
--rw-rw-rw-  2.0 fat    13642 b- defN 24-May-23 17:38 loaderch/loaderch.py
+Zip file size: 17252 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       38 b- defN 24-May-23 18:29 loadupch/__init__.py
--rw-rw-rw-  2.0 fat      111 b- defN 24-May-23 18:33 loadupch/__main__.py
+-rw-rw-rw-  2.0 fat      116 b- defN 24-May-23 18:37 loadupch/__main__.py
 -rw-rw-rw-  2.0 fat    13518 b- defN 24-May-23 18:24 loadupch/app.py
--rw-rw-rw-  2.0 fat    35821 b- defN 24-May-23 18:35 loadupch-0.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      684 b- defN 24-May-23 18:35 loadupch-0.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 18:35 loadupch-0.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-23 18:35 loadupch-0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      842 b- defN 24-May-23 18:35 loadupch-0.0.0.dist-info/RECORD
-11 files, 64880 bytes uncompressed, 19279 bytes compressed:  70.3%
+-rw-rw-rw-  2.0 fat    35821 b- defN 24-May-23 18:38 loadupch-0.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      684 b- defN 24-May-23 18:38 loadupch-0.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 18:38 loadupch-0.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-23 18:38 loadupch-0.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      614 b- defN 24-May-23 18:38 loadupch-0.0.1.dist-info/RECORD
+8 files, 50892 bytes uncompressed, 16184 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,34 +1,25 @@
-Filename: loaderch/__init__.py
-Comment: 
-
-Filename: loaderch/__main__.py
-Comment: 
-
-Filename: loaderch/loaderch.py
-Comment: 
-
 Filename: loadupch/__init__.py
 Comment: 
 
 Filename: loadupch/__main__.py
 Comment: 
 
 Filename: loadupch/app.py
 Comment: 
 
-Filename: loadupch-0.0.0.dist-info/LICENSE
+Filename: loadupch-0.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: loadupch-0.0.0.dist-info/METADATA
+Filename: loadupch-0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: loadupch-0.0.0.dist-info/WHEEL
+Filename: loadupch-0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: loadupch-0.0.0.dist-info/top_level.txt
+Filename: loadupch-0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: loadupch-0.0.0.dist-info/RECORD
+Filename: loadupch-0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## loadupch/__main__.py

```diff
@@ -1,6 +1,6 @@
 from loadupch import Interfacetk
 
 if __name__ == "__main__":
-    app = Interfacetk()
-    app.mainloop()
+    gui = Interfacetk()
+    gui.root.mainloop()
```

## Comparing `loadupch-0.0.0.dist-info/LICENSE` & `loadupch-0.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

