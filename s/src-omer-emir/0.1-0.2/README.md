# Comparing `tmp/src_omer_emir-0.1.tar.gz` & `tmp/src_omer_emir-0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "src_omer_emir-0.1.tar", last modified: Thu May 23 11:05:15 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

