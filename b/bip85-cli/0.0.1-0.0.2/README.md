# Comparing `tmp/bip85-cli-0.0.1.tar.gz` & `tmp/bip85_cli-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bip85-cli-0.0.1.tar", last modified: Tue Sep 13 19:35:47 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

