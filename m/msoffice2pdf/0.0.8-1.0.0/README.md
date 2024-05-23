# Comparing `tmp/msoffice2pdf-0.0.8.tar.gz` & `tmp/msoffice2pdf-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msoffice2pdf-0.0.8.tar", last modified: Mon Sep 13 12:14:41 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

