# Comparing `tmp/pychomp2-1.0.3.tar.gz` & `tmp/pychomp2-1.0.4-cp37-cp37m-musllinux_1_2_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychomp2-1.0.3.tar", last modified: Fri May  3 20:59:22 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

