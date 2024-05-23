# Comparing `tmp/civis-2.0.0.tar.gz` & `tmp/civis-2.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civis-2.0.0.tar", last modified: Tue May 21 13:12:26 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

