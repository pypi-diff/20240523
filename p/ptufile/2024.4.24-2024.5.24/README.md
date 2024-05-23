# Comparing `tmp/ptufile-2024.4.24.tar.gz` & `tmp/ptufile-2024.5.24-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptufile-2024.4.24.tar", last modified: Thu Apr 25 18:36:25 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

