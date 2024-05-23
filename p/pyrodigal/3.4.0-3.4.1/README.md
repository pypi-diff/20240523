# Comparing `tmp/pyrodigal-3.4.0.tar.gz` & `tmp/pyrodigal-3.4.1-cp38-cp38-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrodigal-3.4.0.tar", last modified: Sun May 19 09:13:10 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

