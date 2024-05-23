# Comparing `tmp/calculator_cli_builtincmds-0.1.1.tar.gz` & `tmp/calculator_cli_builtincmds-0.1.2-pp310-pypy310_pp73-manylinux_2_17_s390x.manylinux2014_s390x.whl.zip`

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

