# Comparing `tmp/k8-29.0.8.tar.gz` & `tmp/k8-29.0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8-29.0.8.tar", last modified: Fri May  3 23:47:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

