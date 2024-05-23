# Comparing `tmp/manteia_qa_pylinac-1.2.3.tar.gz` & `tmp/manteia_qa_pylinac-1.2.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manteia_qa_pylinac-1.2.3.tar", last modified: Mon May 13 03:03:19 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

