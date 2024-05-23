# Comparing `tmp/nelsie-0.8.0.tar.gz` & `tmp/nelsie-0.9.0-cp39-abi3-macosx_10_12_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

