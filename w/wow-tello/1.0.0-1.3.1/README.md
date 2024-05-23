# Comparing `tmp/wow_tello-1.0.0.tar.gz` & `tmp/wow_tello-1.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wow_tello-1.0.0.tar", last modified: Mon May 20 09:26:49 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

