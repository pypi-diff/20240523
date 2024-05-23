# Comparing `tmp/pycodata-0.9.0.tar.gz` & `tmp/pycodata-1.0.0-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodata-0.9.0.tar", last modified: Sun Dec 17 21:04:14 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

