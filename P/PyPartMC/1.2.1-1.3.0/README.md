# Comparing `tmp/pypartmc-1.2.1.tar.gz` & `tmp/PyPartMC-1.3.0-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypartmc-1.2.1.tar", last modified: Tue May 21 11:59:53 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

