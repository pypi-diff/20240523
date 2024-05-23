# Comparing `tmp/pdfconduit-2.0.2.tar.gz` & `tmp/pdfconduit-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfconduit-2.0.2.tar", last modified: Thu Jun 17 17:14:59 2021, max compression
+gzip compressed data, was "pdfconduit-2.1.0.tar", last modified: Thu May 23 20:15:57 2024, max compression
```

## Comparing `pdfconduit-2.0.2.tar` & `pdfconduit-2.1.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.397011 pdfconduit-2.0.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       36 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      865 2021-06-17 17:14:59.397011 pdfconduit-2.0.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    15396 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.389011 pdfconduit-2.0.2/pdfconduit/
--rw-rw-r--   0 travis    (2000) travis    (2000)      362 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.389011 pdfconduit-2.0.2/pdfconduit/conduit/
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3807 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/encrypt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1720 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/extract.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.389011 pdfconduit-2.0.2/pdfconduit/conduit/lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)      608 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/lib/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.389011 pdfconduit-2.0.2/pdfconduit/conduit/lib/img/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21694 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/lib/img/Standard (no blocks).png
--rw-rw-r--   0 travis    (2000) travis    (2000)    27224 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/lib/img/Standard.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    37495 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/lib/img/Wide (no blocks).png
--rw-rw-r--   0 travis    (2000) travis    (2000)    43888 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/lib/img/Wide.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     5130 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/samples.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.393011 pdfconduit-2.0.2/pdfconduit/conduit/watermark/
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/watermark/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10863 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/watermark/add.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1737 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/watermark/label.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9171 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/conduit/watermark/watermark.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.393011 pdfconduit-2.0.2/pdfconduit/convert/
--rw-rw-r--   0 travis    (2000) travis    (2000)      309 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/convert/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1861 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/convert/flatten.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2818 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/convert/img2pdf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/convert/pdf2img.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.393011 pdfconduit-2.0.2/pdfconduit/modify/
--rw-rw-r--   0 travis    (2000) travis    (2000)       96 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/modify/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.393011 pdfconduit-2.0.2/pdfconduit/modify/canvas/
--rw-rw-r--   0 travis    (2000) travis    (2000)      224 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/modify/canvas/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4745 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/modify/canvas/constructor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1586 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/modify/canvas/objects.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.393011 pdfconduit-2.0.2/pdfconduit/modify/draw/
--rw-rw-r--   0 travis    (2000) travis    (2000)      180 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/modify/draw/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5819 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/modify/draw/pdf.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.393011 pdfconduit-2.0.2/pdfconduit/transform/
--rw-rw-r--   0 travis    (2000) travis    (2000)      277 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/transform/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2377 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/transform/merge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2197 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/transform/rotate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1387 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/transform/slice.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2911 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/transform/upscale.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.397011 pdfconduit-2.0.2/pdfconduit/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)      430 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2475 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/utils/info.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2248 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/utils/path.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      449 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/utils/read.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1054 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/utils/receipt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      485 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/utils/view.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1451 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/pdfconduit/utils/write.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.389011 pdfconduit-2.0.2/pdfconduit.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      865 2021-06-17 17:14:59.000000 pdfconduit-2.0.2/pdfconduit.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1706 2021-06-17 17:14:59.000000 pdfconduit-2.0.2/pdfconduit.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-17 17:14:59.000000 pdfconduit-2.0.2/pdfconduit.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       95 2021-06-17 17:14:59.000000 pdfconduit-2.0.2/pdfconduit.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2021-06-17 17:14:59.000000 pdfconduit-2.0.2/pdfconduit.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-06-17 17:14:59.397011 pdfconduit-2.0.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1540 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-17 17:14:59.397011 pdfconduit-2.0.2/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      388 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3814 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/tests/test_conduit_encrypt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5049 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/tests/test_conduit_watermark.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1078 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/tests/test_convert_flatten.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1297 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/tests/test_convert_img2pdf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      798 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/tests/test_convert_pdf2img.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1620 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/tests/test_transform_merge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3657 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/tests/test_transform_rotate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1404 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/tests/test_transform_slice.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2550 2021-06-17 17:14:22.000000 pdfconduit-2.0.2/tests/test_transform_upscale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.722363 pdfconduit-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 20:15:57.722363 pdfconduit-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.710363 pdfconduit-2.1.0/pdfconduit/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.714363 pdfconduit-2.1.0/pdfconduit/conduit/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.714363 pdfconduit-2.1.0/pdfconduit/conduit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.714363 pdfconduit-2.1.0/pdfconduit/conduit/lib/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    21694 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/lib/img/Standard (no blocks).png
+-rw-r--r--   0 runner    (1001) docker     (127)    27224 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/lib/img/Standard.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37495 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/lib/img/Wide (no blocks).png
+-rw-r--r--   0 runner    (1001) docker     (127)    43888 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/lib/img/Wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.714363 pdfconduit-2.1.0/pdfconduit/conduit/watermark/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/watermark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/watermark/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/watermark/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/conduit/watermark/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.714363 pdfconduit-2.1.0/pdfconduit/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/convert/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/convert/img2pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/convert/pdf2img.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.714363 pdfconduit-2.1.0/pdfconduit/modify/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/modify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.714363 pdfconduit-2.1.0/pdfconduit/modify/canvas/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/modify/canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/modify/canvas/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/modify/canvas/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.718363 pdfconduit-2.1.0/pdfconduit/modify/draw/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/modify/draw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/modify/draw/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.718363 pdfconduit-2.1.0/pdfconduit/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/transform/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/transform/rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/transform/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/transform/upscale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.718363 pdfconduit-2.1.0/pdfconduit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/utils/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/utils/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/utils/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/utils/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/pdfconduit/utils/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.710363 pdfconduit-2.1.0/pdfconduit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 20:15:57.000000 pdfconduit-2.1.0/pdfconduit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-23 20:15:57.000000 pdfconduit-2.1.0/pdfconduit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:15:57.000000 pdfconduit-2.1.0/pdfconduit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 20:15:57.000000 pdfconduit-2.1.0/pdfconduit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 20:15:57.000000 pdfconduit-2.1.0/pdfconduit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:15:57.722363 pdfconduit-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:15:57.718363 pdfconduit-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/tests/test_conduit_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/tests/test_conduit_watermark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/tests/test_convert_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/tests/test_convert_img2pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/tests/test_convert_pdf2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/tests/test_transform_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/tests/test_transform_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/tests/test_transform_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-23 20:15:50.000000 pdfconduit-2.1.0/tests/test_transform_upscale.py
```

### Comparing `pdfconduit-2.0.2/LICENSE.md` & `pdfconduit-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/PKG-INFO` & `pdfconduit-2.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pdfconduit
-Version: 2.0.2
+Version: 2.1.0
 Summary: PDF toolkit for preparing documents for distribution.
 Home-page: https://github.com/sfneal/pdfconduit
 Author: Stephen Neal
 Author-email: stephen@stephenneal.net
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >3.6.8
 License-File: LICENSE.md
 
 
 A Pure-Python library built as a PDF toolkit.  Prepare documents for distribution.
 
 Features:
@@ -19,9 +17,7 @@
 - Encrypt: Password protect and restrict permissions to print only
 - Rotate: Rotate by increments of 90 degrees
 - Upscale: Scale PDF size
 - Merge: Concatenate multiple documents into one file
 - Slice: Extract page ranges from documents
 - Extract Text and Images
 - Retrieve document metadata and information
-
-
```

### Comparing `pdfconduit-2.0.2/README.md` & `pdfconduit-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/conduit/encrypt.py` & `pdfconduit-2.1.0/pdfconduit/conduit/encrypt.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/conduit/extract.py` & `pdfconduit-2.1.0/pdfconduit/conduit/extract.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/conduit/lib/__init__.py` & `pdfconduit-2.1.0/pdfconduit/conduit/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/conduit/lib/img/Standard (no blocks).png` & `pdfconduit-2.1.0/pdfconduit/conduit/lib/img/Standard (no blocks).png`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/conduit/lib/img/Standard.png` & `pdfconduit-2.1.0/pdfconduit/conduit/lib/img/Standard.png`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/conduit/lib/img/Wide (no blocks).png` & `pdfconduit-2.1.0/pdfconduit/conduit/lib/img/Wide (no blocks).png`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/conduit/lib/img/Wide.png` & `pdfconduit-2.1.0/pdfconduit/conduit/lib/img/Wide.png`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/conduit/samples.py` & `pdfconduit-2.1.0/pdfconduit/conduit/samples.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/conduit/watermark/add.py` & `pdfconduit-2.1.0/pdfconduit/conduit/watermark/add.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/conduit/watermark/label.py` & `pdfconduit-2.1.0/pdfconduit/conduit/watermark/label.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/conduit/watermark/watermark.py` & `pdfconduit-2.1.0/pdfconduit/conduit/watermark/watermark.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/convert/flatten.py` & `pdfconduit-2.1.0/pdfconduit/convert/flatten.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/convert/img2pdf.py` & `pdfconduit-2.1.0/pdfconduit/convert/img2pdf.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/convert/pdf2img.py` & `pdfconduit-2.1.0/pdfconduit/convert/pdf2img.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def _get_page_data(self, pno, zoom=0):
         """
         Return a PNG image for a document page number. If zoom is other than 0, one of
         the 4 page quadrants are zoomed-in instead and the corresponding clip returned.
         """
         dlist = self.dlist_tab[pno]    # get display list
         if not dlist:    # create if not yet there
-            self.dlist_tab[pno] = self.doc[pno].getDisplayList()
+            self.dlist_tab[pno] = self.doc[pno].get_displaylist()
             dlist = self.dlist_tab[pno]
         r = dlist.rect    # page rectangle
         mp = r.tl + (r.br - r.tl) * 0.5    # rect middle point
         mt = r.tl + (r.tr - r.tl) * 0.5    # middle of top edge
         ml = r.tl + (r.bl - r.tl) * 0.5    # middle of left edge
         mr = r.tr + (r.br - r.tr) * 0.5    # middle of right egde
         mb = r.bl + (r.br - r.bl) * 0.5    # middle of bottom edge
@@ -65,18 +65,18 @@
         elif zoom == 4:    # bot-right quadrant
             clip = fitz.Rect(mp, r.br)
         elif zoom == 2:    # top-right
             clip = fitz.Rect(mt, mr)
         elif zoom == 3:    # bot-left
             clip = fitz.Rect(ml, mb)
         if zoom == 0:    # total page
-            pix = dlist.getPixmap(alpha=self.alpha)
+            pix = dlist.get_pixmap(alpha=self.alpha)
         else:
-            pix = dlist.getPixmap(alpha=self.alpha, matrix=mat, clip=clip)
-        return pix.getPNGData()    # return the PNG image
+            pix = dlist.get_pixmap(alpha=self.alpha, matrix=mat, clip=clip)
+        return pix.tobytes()    # return the PNG image
 
     def _get_output(self, index):
         if self.output:
             return self.output
         elif not self.tempdir:
             output_file = add_suffix(self.file_name, str(index + 1), ext=self.ext)
             return os.path.join(self.output_dir, output_file)
```

### Comparing `pdfconduit-2.0.2/pdfconduit/modify/canvas/constructor.py` & `pdfconduit-2.1.0/pdfconduit/modify/canvas/constructor.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/modify/canvas/objects.py` & `pdfconduit-2.1.0/pdfconduit/modify/canvas/objects.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/modify/draw/pdf.py` & `pdfconduit-2.1.0/pdfconduit/modify/draw/pdf.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/transform/merge.py` & `pdfconduit-2.1.0/pdfconduit/transform/merge.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/transform/rotate.py` & `pdfconduit-2.1.0/pdfconduit/transform/rotate.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/transform/slice.py` & `pdfconduit-2.1.0/pdfconduit/transform/slice.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/transform/upscale.py` & `pdfconduit-2.1.0/pdfconduit/transform/upscale.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/utils/info.py` & `pdfconduit-2.1.0/pdfconduit/utils/info.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/utils/path.py` & `pdfconduit-2.1.0/pdfconduit/utils/path.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/utils/receipt.py` & `pdfconduit-2.1.0/pdfconduit/utils/receipt.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit/utils/write.py` & `pdfconduit-2.1.0/pdfconduit/utils/write.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/pdfconduit.egg-info/PKG-INFO` & `pdfconduit-2.1.0/pdfconduit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pdfconduit
-Version: 2.0.2
+Version: 2.1.0
 Summary: PDF toolkit for preparing documents for distribution.
 Home-page: https://github.com/sfneal/pdfconduit
 Author: Stephen Neal
 Author-email: stephen@stephenneal.net
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >3.6.8
 License-File: LICENSE.md
 
 
 A Pure-Python library built as a PDF toolkit.  Prepare documents for distribution.
 
 Features:
@@ -19,9 +17,7 @@
 - Encrypt: Password protect and restrict permissions to print only
 - Rotate: Rotate by increments of 90 degrees
 - Upscale: Scale PDF size
 - Merge: Concatenate multiple documents into one file
 - Slice: Extract page ranges from documents
 - Extract Text and Images
 - Retrieve document metadata and information
-
-
```

### Comparing `pdfconduit-2.0.2/pdfconduit.egg-info/SOURCES.txt` & `pdfconduit-2.1.0/pdfconduit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/setup.py` & `pdfconduit-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 setup(
     name='pdfconduit',
     version=get_version(),
     packages=find_packages(),
     install_requires=[
         'looptools',
         'pdfrw>=0.4',
-        'PyMuPDF>=1.17.7,<=1.18.8',
+        'PyMuPDF>=1.17.7,<=1.24.4',
         'PyPDF3>=1.0.1',
-        'PillowImage>=1.1.6',
+        'PillowImage>=1.2.0',
         'PyBundle>=1.0.6',
     ],
     python_requires='>3.6.8',
     include_package_data=True,
     url='https://github.com/sfneal/pdfconduit',
     license='',
     author='Stephen Neal',
```

### Comparing `pdfconduit-2.0.2/tests/test_conduit_encrypt.py` & `pdfconduit-2.1.0/tests/test_conduit_encrypt.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/tests/test_conduit_watermark.py` & `pdfconduit-2.1.0/tests/test_conduit_watermark.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/tests/test_convert_flatten.py` & `pdfconduit-2.1.0/tests/test_convert_flatten.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/tests/test_convert_img2pdf.py` & `pdfconduit-2.1.0/tests/test_convert_img2pdf.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/tests/test_convert_pdf2img.py` & `pdfconduit-2.1.0/tests/test_convert_pdf2img.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/tests/test_transform_merge.py` & `pdfconduit-2.1.0/tests/test_transform_merge.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/tests/test_transform_rotate.py` & `pdfconduit-2.1.0/tests/test_transform_rotate.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/tests/test_transform_slice.py` & `pdfconduit-2.1.0/tests/test_transform_slice.py`

 * *Files identical despite different names*

### Comparing `pdfconduit-2.0.2/tests/test_transform_upscale.py` & `pdfconduit-2.1.0/tests/test_transform_upscale.py`

 * *Files identical despite different names*

