# Comparing `tmp/wrapper_pika-0.0.2.tar.gz` & `tmp/wrapper_pika-0.0.3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapper_pika-0.0.2.tar", last modified: Mon Apr  1 10:19:53 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

