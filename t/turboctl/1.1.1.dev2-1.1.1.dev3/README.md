# Comparing `tmp/turboctl-1.1.1.dev2.tar.gz` & `tmp/turboctl-1.1.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turboctl-1.1.1.dev2.tar", last modified: Thu May 23 12:47:19 2024, max compression
+gzip compressed data, was "turboctl-1.1.1.dev3.tar", last modified: Thu May 23 12:51:53 2024, max compression
```

## Comparing `turboctl-1.1.1.dev2.tar` & `turboctl-1.1.1.dev3.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      104 2024-05-23 12:25:42.000000 turboctl-1.1.1.dev2/.gitignore
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.200790 turboctl-1.1.1.dev2/.hypothesis/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.200790 turboctl-1.1.1.dev2/.hypothesis/examples/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/.hypothesis/examples/098af05827140584/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/098af05827140584/236d65b6820cb9eb
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/098af05827140584/8f344065c6e31a55
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/098af05827140584/ebec0feb4a7296ef
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/.hypothesis/examples/3ef5c497a7146f5f/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/3ef5c497a7146f5f/37b7d6a6935710cc
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/.hypothesis/examples/6c152343fd7da806/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/6c152343fd7da806/37b7d6a6935710cc
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/6c152343fd7da806/bf2177f7c1c50efa
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/6c152343fd7da806/ebec0feb4a7296ef
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/.hypothesis/examples/719feafe55d6092a/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        5 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/719feafe55d6092a/008e1630a9922afd
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/719feafe55d6092a/27ed25acd9ac2252
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       12 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/719feafe55d6092a/88e1a36747cf7ba7
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/719feafe55d6092a/ecd6acb5382280fa
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        5 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/719feafe55d6092a/f8a0b55de165f0f7
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/.hypothesis/examples/79a409375dd4d4e2/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/79a409375dd4d4e2/0e3c5a512caa470e
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       27 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/79a409375dd4d4e2/1532c3657cb335c2
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/79a409375dd4d4e2/37b7d6a6935710cc
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       35 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/79a409375dd4d4e2/4b332aaacb70845a
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/79a409375dd4d4e2/8f344065c6e31a55
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/79a409375dd4d4e2/a92d75b981cc1d16
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/.hypothesis/examples/7ae13c50088acc79/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        8 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/7ae13c50088acc79/1157f47c0c21cc58
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        9 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/7ae13c50088acc79/5d9857cd134a7d76
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        6 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/7ae13c50088acc79/7f584f87e4c8748c
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/7ae13c50088acc79/bf2177f7c1c50efa
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        6 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/7ae13c50088acc79/bf9e0341c6723c0c
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/0b64596632c348d1
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        9 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/2a7de3a2e977d1bf
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        8 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/3159c3254a05fa28
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/563c99e486a45858
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/5be7ff32ddb1da60
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/658062a505f9a78d
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/71ebd30c888b37de
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/868d8d368a4a202b
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        8 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/91bd8eded23b9c4f
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/93e42aab04fa7201
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/9b6919dfe6d4ee68
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/a7ab860d9dd19a4f
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/d20a55593bc9dcb6
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/dd2d6fdd18636fda
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/e02700d5d11c71d4
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       26 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/e2d9c31bc45f7328
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/f62638bcbdd30c0d
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/examples/991880036e4bf226/f95b844e14efffe0
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.200790 turboctl-1.1.1.dev2/.hypothesis/unicode_data/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/.hypothesis/unicode_data/11.0.0/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    20358 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/.hypothesis/unicode_data/11.0.0/charmap.json.gz
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      326 2024-05-23 10:27:59.000000 turboctl-1.1.1.dev2/.readthedocs.yaml
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1964 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/PKG-INFO
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1448 2024-05-23 12:47:13.000000 turboctl-1.1.1.dev2/README.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1740 2024-05-23 12:45:14.000000 turboctl-1.1.1.dev2/TODO
--rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)      845 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/add-to-path
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.200790 turboctl-1.1.1.dev2/doc/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/doc/sphinx/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      634 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/Makefile
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/doc/sphinx/_static/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      509 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/_static/custom.css
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    40547 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/advanced_UI.png
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      753 2024-05-23 12:43:53.000000 turboctl-1.1.1.dev2/doc/sphinx/changelog.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     3498 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/conf.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     8337 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/errata.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1436 2024-05-23 12:47:13.000000 turboctl-1.1.1.dev2/doc/sphinx/index.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1449 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/installation.rst
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/doc/sphinx/modules/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       78 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/hacks.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      388 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/index.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      163 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/main.rst
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/doc/sphinx/modules/telegram/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       99 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/telegram/api.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      128 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/telegram/codes.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      140 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/telegram/datatypes.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      227 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/telegram/index.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      108 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/telegram/parser.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      115 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/telegram/telegram.rst
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/doc/sphinx/modules/ui/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      108 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/ui/advanced_tui.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      117 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/ui/command_line_ui.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      123 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/ui/control_interface.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       84 2024-05-23 12:15:41.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/ui/docs.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      251 2024-05-23 12:16:35.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/ui/index.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       99 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/ui/queuefile.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      111 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/ui/status_format.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       87 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/ui/table.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       93 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/ui/widgets.rst
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/doc/sphinx/modules/virtualpump/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      153 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/virtualpump/hardware_component.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      292 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/virtualpump/index.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      545 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/virtualpump/parameter_component.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      150 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/virtualpump/virtualconnection.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      132 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules/virtualpump/virtualpump.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      557 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/modules.rst
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      276 2024-05-23 10:52:05.000000 turboctl-1.1.1.dev2/doc/sphinx/requirements.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    40532 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/doc/sphinx/simple_UI.png
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     8290 2024-05-23 11:35:23.000000 turboctl-1.1.1.dev2/doc/sphinx/usage.rst
--rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)      617 2024-05-23 12:21:02.000000 turboctl-1.1.1.dev2/make-docs
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     2588 2024-05-23 12:21:38.000000 turboctl-1.1.1.dev2/make_readme.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      286 2024-05-23 12:04:43.000000 turboctl-1.1.1.dev2/makefile
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      748 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/pyproject.toml
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       38 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/setup.cfg
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/test_turboctl/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/__init__.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/test_turboctl/run_tests/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5303 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/run_tests/run_tests.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1590 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/run_tests/test_run_tests.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/test_turboctl/telegram/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/test_turboctl/telegram/.hypothesis/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.204790 turboctl-1.1.1.dev2/test_turboctl/telegram/.hypothesis/unicode_data/
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/test_turboctl/telegram/.hypothesis/unicode_data/11.0.0/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    20358 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/telegram/.hypothesis/unicode_data/11.0.0/charmap.json.gz
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/telegram/__init__.py
--rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)     3923 2020-07-24 18:46:53.000000 turboctl-1.1.1.dev2/test_turboctl/telegram/test_api.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     6031 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/telegram/test_codes.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    16462 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/test_turboctl/telegram/test_datatypes.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    13853 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/telegram/test_parser.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    17431 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev2/test_turboctl/telegram/test_telegram.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/test_turboctl/ui/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/ui/__init.py__
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     6682 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/ui/test_abstractui.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     3594 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/ui/test_command_parser.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     2359 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/ui/test_correct_error_message.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    10038 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/ui/test_output.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4136 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/ui/test_table.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5049 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/ui/test_tui.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/test_turboctl/virtualpump/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/virtualpump/__init__.py
--rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)    15397 2020-07-24 14:54:13.000000 turboctl-1.1.1.dev2/test_turboctl/virtualpump/test_hardware_component.py
--rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)    18089 2020-07-22 11:34:05.000000 turboctl-1.1.1.dev2/test_turboctl/virtualpump/test_parameter_component.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4253 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/virtualpump/test_virtualconnection.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5580 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/test_turboctl/virtualpump/test_virtualpump.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/turboctl/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      234 2024-05-23 12:47:06.000000 turboctl-1.1.1.dev2/turboctl/__init__.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5512 2024-05-23 11:34:07.000000 turboctl-1.1.1.dev2/turboctl/__main__.py
--rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     2631 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/turboctl/hacks.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/turboctl/telegram/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       78 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/turboctl/telegram/__init__.py
--rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     3972 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/turboctl/telegram/api.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    21340 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev2/turboctl/telegram/codes.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    17240 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/turboctl/telegram/datatypes.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     8444 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/turboctl/telegram/errors.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    22442 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev2/turboctl/telegram/parameters.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    18964 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/turboctl/telegram/parser.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    25563 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev2/turboctl/telegram/telegram.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     2972 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/turboctl/telegram/warnings.txt
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/turboctl/ui/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       70 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/turboctl/ui/__init__.py
--rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)     4670 2021-01-12 12:53:24.000000 turboctl-1.1.1.dev2/turboctl/ui/advanced_tui.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    19889 2024-05-23 11:35:55.000000 turboctl-1.1.1.dev2/turboctl/ui/command_line_ui.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     9720 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/turboctl/ui/control_interface.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      293 2024-05-23 12:17:25.000000 turboctl-1.1.1.dev2/turboctl/ui/docs.py
--rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)     3385 2020-07-03 12:38:41.000000 turboctl-1.1.1.dev2/turboctl/ui/queuefile.py
--rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     2862 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/turboctl/ui/status_format.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     6331 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev2/turboctl/ui/table.py
--rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)    21497 2021-01-12 12:53:13.000000 turboctl-1.1.1.dev2/turboctl/ui/widgets.py
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/turboctl/virtualpump/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       97 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/turboctl/virtualpump/__init__.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    18730 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev2/turboctl/virtualpump/hardware_component.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    15479 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/turboctl/virtualpump/parameter_component.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     7900 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/turboctl/virtualpump/virtualconnection.py
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4241 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev2/turboctl/virtualpump/virtualpump.py
--rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     1051 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev2/turboctl-run
-drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:47:19.208790 turboctl-1.1.1.dev2/turboctl.egg-info/
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1964 2024-05-23 12:47:19.000000 turboctl-1.1.1.dev2/turboctl.egg-info/PKG-INFO
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5449 2024-05-23 12:47:19.000000 turboctl-1.1.1.dev2/turboctl.egg-info/SOURCES.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        1 2024-05-23 12:47:19.000000 turboctl-1.1.1.dev2/turboctl.egg-info/dependency_links.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       52 2024-05-23 12:47:19.000000 turboctl-1.1.1.dev2/turboctl.egg-info/entry_points.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       52 2024-05-23 12:47:19.000000 turboctl-1.1.1.dev2/turboctl.egg-info/requires.txt
--rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       32 2024-05-23 12:47:19.000000 turboctl-1.1.1.dev2/turboctl.egg-info/top_level.txt
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.275288 turboctl-1.1.1.dev3/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      104 2024-05-23 12:25:42.000000 turboctl-1.1.1.dev3/.gitignore
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.255288 turboctl-1.1.1.dev3/.hypothesis/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.255288 turboctl-1.1.1.dev3/.hypothesis/examples/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.259288 turboctl-1.1.1.dev3/.hypothesis/examples/098af05827140584/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/098af05827140584/236d65b6820cb9eb
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/098af05827140584/8f344065c6e31a55
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/098af05827140584/ebec0feb4a7296ef
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.259288 turboctl-1.1.1.dev3/.hypothesis/examples/3ef5c497a7146f5f/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/3ef5c497a7146f5f/37b7d6a6935710cc
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.259288 turboctl-1.1.1.dev3/.hypothesis/examples/6c152343fd7da806/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/6c152343fd7da806/37b7d6a6935710cc
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/6c152343fd7da806/bf2177f7c1c50efa
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/6c152343fd7da806/ebec0feb4a7296ef
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.259288 turboctl-1.1.1.dev3/.hypothesis/examples/719feafe55d6092a/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        5 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/719feafe55d6092a/008e1630a9922afd
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/719feafe55d6092a/27ed25acd9ac2252
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       12 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/719feafe55d6092a/88e1a36747cf7ba7
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/719feafe55d6092a/ecd6acb5382280fa
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        5 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/719feafe55d6092a/f8a0b55de165f0f7
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.259288 turboctl-1.1.1.dev3/.hypothesis/examples/79a409375dd4d4e2/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/79a409375dd4d4e2/0e3c5a512caa470e
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       27 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/79a409375dd4d4e2/1532c3657cb335c2
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/79a409375dd4d4e2/37b7d6a6935710cc
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       35 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/79a409375dd4d4e2/4b332aaacb70845a
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/79a409375dd4d4e2/8f344065c6e31a55
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        3 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/79a409375dd4d4e2/a92d75b981cc1d16
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.259288 turboctl-1.1.1.dev3/.hypothesis/examples/7ae13c50088acc79/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        8 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/7ae13c50088acc79/1157f47c0c21cc58
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        9 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/7ae13c50088acc79/5d9857cd134a7d76
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        6 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/7ae13c50088acc79/7f584f87e4c8748c
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/7ae13c50088acc79/bf2177f7c1c50efa
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        6 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/7ae13c50088acc79/bf9e0341c6723c0c
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.259288 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/0b64596632c348d1
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        9 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/2a7de3a2e977d1bf
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        8 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/3159c3254a05fa28
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/563c99e486a45858
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/5be7ff32ddb1da60
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/658062a505f9a78d
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/71ebd30c888b37de
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/868d8d368a4a202b
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        8 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/91bd8eded23b9c4f
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/93e42aab04fa7201
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/9b6919dfe6d4ee68
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/a7ab860d9dd19a4f
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/d20a55593bc9dcb6
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/dd2d6fdd18636fda
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        4 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/e02700d5d11c71d4
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       26 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/e2d9c31bc45f7328
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        7 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/f62638bcbdd30c0d
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       25 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/examples/991880036e4bf226/f95b844e14efffe0
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.255288 turboctl-1.1.1.dev3/.hypothesis/unicode_data/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.259288 turboctl-1.1.1.dev3/.hypothesis/unicode_data/11.0.0/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    20358 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/.hypothesis/unicode_data/11.0.0/charmap.json.gz
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      317 2024-05-23 12:49:59.000000 turboctl-1.1.1.dev3/.readthedocs.yaml
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1964 2024-05-23 12:51:53.275288 turboctl-1.1.1.dev3/PKG-INFO
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1448 2024-05-23 12:51:46.000000 turboctl-1.1.1.dev3/README.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1740 2024-05-23 12:45:14.000000 turboctl-1.1.1.dev3/TODO
+-rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)      845 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/add-to-path
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.255288 turboctl-1.1.1.dev3/doc/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.263288 turboctl-1.1.1.dev3/doc/sphinx/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      634 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/Makefile
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.263288 turboctl-1.1.1.dev3/doc/sphinx/_static/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      509 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/_static/custom.css
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    40547 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/advanced_UI.png
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      753 2024-05-23 12:43:53.000000 turboctl-1.1.1.dev3/doc/sphinx/changelog.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     3498 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/conf.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     8337 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/errata.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1436 2024-05-23 12:51:46.000000 turboctl-1.1.1.dev3/doc/sphinx/index.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1449 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/installation.rst
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.263288 turboctl-1.1.1.dev3/doc/sphinx/modules/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       78 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/hacks.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      388 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/index.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      163 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/main.rst
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.263288 turboctl-1.1.1.dev3/doc/sphinx/modules/telegram/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       99 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/telegram/api.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      128 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/telegram/codes.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      140 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/telegram/datatypes.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      227 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/telegram/index.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      108 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/telegram/parser.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      115 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/telegram/telegram.rst
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.263288 turboctl-1.1.1.dev3/doc/sphinx/modules/ui/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      108 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/ui/advanced_tui.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      117 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/ui/command_line_ui.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      123 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/ui/control_interface.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       84 2024-05-23 12:15:41.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/ui/docs.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      251 2024-05-23 12:16:35.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/ui/index.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       99 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/ui/queuefile.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      111 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/ui/status_format.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       87 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/ui/table.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       93 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/ui/widgets.rst
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.263288 turboctl-1.1.1.dev3/doc/sphinx/modules/virtualpump/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      153 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/virtualpump/hardware_component.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      292 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/virtualpump/index.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      545 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/virtualpump/parameter_component.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      150 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/virtualpump/virtualconnection.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      132 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules/virtualpump/virtualpump.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      557 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/modules.rst
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      276 2024-05-23 10:52:05.000000 turboctl-1.1.1.dev3/doc/sphinx/requirements.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    40532 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/doc/sphinx/simple_UI.png
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     8290 2024-05-23 11:35:23.000000 turboctl-1.1.1.dev3/doc/sphinx/usage.rst
+-rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)      617 2024-05-23 12:21:02.000000 turboctl-1.1.1.dev3/make-docs
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     2588 2024-05-23 12:21:38.000000 turboctl-1.1.1.dev3/make_readme.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      286 2024-05-23 12:04:43.000000 turboctl-1.1.1.dev3/makefile
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      748 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/pyproject.toml
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       38 2024-05-23 12:51:53.275288 turboctl-1.1.1.dev3/setup.cfg
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.263288 turboctl-1.1.1.dev3/test_turboctl/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/__init__.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.263288 turboctl-1.1.1.dev3/test_turboctl/run_tests/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5303 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/run_tests/run_tests.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1590 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/run_tests/test_run_tests.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.263288 turboctl-1.1.1.dev3/test_turboctl/telegram/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.259288 turboctl-1.1.1.dev3/test_turboctl/telegram/.hypothesis/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.259288 turboctl-1.1.1.dev3/test_turboctl/telegram/.hypothesis/unicode_data/
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.267288 turboctl-1.1.1.dev3/test_turboctl/telegram/.hypothesis/unicode_data/11.0.0/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    20358 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/telegram/.hypothesis/unicode_data/11.0.0/charmap.json.gz
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/telegram/__init__.py
+-rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)     3923 2020-07-24 18:46:53.000000 turboctl-1.1.1.dev3/test_turboctl/telegram/test_api.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     6031 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/telegram/test_codes.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    16462 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/test_turboctl/telegram/test_datatypes.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    13853 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/telegram/test_parser.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    17431 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev3/test_turboctl/telegram/test_telegram.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.267288 turboctl-1.1.1.dev3/test_turboctl/ui/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/ui/__init.py__
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     6682 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/ui/test_abstractui.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     3594 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/ui/test_command_parser.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     2359 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/ui/test_correct_error_message.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    10038 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/ui/test_output.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4136 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/ui/test_table.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5049 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/ui/test_tui.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.267288 turboctl-1.1.1.dev3/test_turboctl/virtualpump/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        0 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/virtualpump/__init__.py
+-rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)    15397 2020-07-24 14:54:13.000000 turboctl-1.1.1.dev3/test_turboctl/virtualpump/test_hardware_component.py
+-rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)    18089 2020-07-22 11:34:05.000000 turboctl-1.1.1.dev3/test_turboctl/virtualpump/test_parameter_component.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4253 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/virtualpump/test_virtualconnection.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5580 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/test_turboctl/virtualpump/test_virtualpump.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.267288 turboctl-1.1.1.dev3/turboctl/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      234 2024-05-23 12:50:16.000000 turboctl-1.1.1.dev3/turboctl/__init__.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5512 2024-05-23 11:34:07.000000 turboctl-1.1.1.dev3/turboctl/__main__.py
+-rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     2631 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/turboctl/hacks.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.271288 turboctl-1.1.1.dev3/turboctl/telegram/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       78 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/turboctl/telegram/__init__.py
+-rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     3972 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/turboctl/telegram/api.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    21340 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev3/turboctl/telegram/codes.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    17240 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/turboctl/telegram/datatypes.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     8444 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/turboctl/telegram/errors.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    22442 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev3/turboctl/telegram/parameters.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    18964 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/turboctl/telegram/parser.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    25563 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev3/turboctl/telegram/telegram.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     2972 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/turboctl/telegram/warnings.txt
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.271288 turboctl-1.1.1.dev3/turboctl/ui/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       70 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/turboctl/ui/__init__.py
+-rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)     4670 2021-01-12 12:53:24.000000 turboctl-1.1.1.dev3/turboctl/ui/advanced_tui.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    19889 2024-05-23 11:35:55.000000 turboctl-1.1.1.dev3/turboctl/ui/command_line_ui.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     9720 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/turboctl/ui/control_interface.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)      293 2024-05-23 12:17:25.000000 turboctl-1.1.1.dev3/turboctl/ui/docs.py
+-rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)     3385 2020-07-03 12:38:41.000000 turboctl-1.1.1.dev3/turboctl/ui/queuefile.py
+-rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     2862 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/turboctl/ui/status_format.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     6331 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev3/turboctl/ui/table.py
+-rwxrwxrwx   0 kivelaf1 (3280510) domain users (70000)    21497 2021-01-12 12:53:13.000000 turboctl-1.1.1.dev3/turboctl/ui/widgets.py
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.271288 turboctl-1.1.1.dev3/turboctl/virtualpump/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       97 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/turboctl/virtualpump/__init__.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    18730 2024-05-22 14:25:33.000000 turboctl-1.1.1.dev3/turboctl/virtualpump/hardware_component.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)    15479 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/turboctl/virtualpump/parameter_component.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     7900 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/turboctl/virtualpump/virtualconnection.py
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     4241 2024-03-01 14:40:46.000000 turboctl-1.1.1.dev3/turboctl/virtualpump/virtualpump.py
+-rwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)     1051 2024-03-27 19:32:36.000000 turboctl-1.1.1.dev3/turboctl-run
+drwxr-xr-x   0 kivelaf1 (3280510) domain users (70000)        0 2024-05-23 12:51:53.275288 turboctl-1.1.1.dev3/turboctl.egg-info/
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     1964 2024-05-23 12:51:53.000000 turboctl-1.1.1.dev3/turboctl.egg-info/PKG-INFO
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)     5449 2024-05-23 12:51:53.000000 turboctl-1.1.1.dev3/turboctl.egg-info/SOURCES.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)        1 2024-05-23 12:51:53.000000 turboctl-1.1.1.dev3/turboctl.egg-info/dependency_links.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       52 2024-05-23 12:51:53.000000 turboctl-1.1.1.dev3/turboctl.egg-info/entry_points.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       52 2024-05-23 12:51:53.000000 turboctl-1.1.1.dev3/turboctl.egg-info/requires.txt
+-rw-r--r--   0 kivelaf1 (3280510) domain users (70000)       32 2024-05-23 12:51:53.000000 turboctl-1.1.1.dev3/turboctl.egg-info/top_level.txt
```

### Comparing `turboctl-1.1.1.dev2/.hypothesis/unicode_data/11.0.0/charmap.json.gz` & `turboctl-1.1.1.dev3/.hypothesis/unicode_data/11.0.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/PKG-INFO` & `turboctl-1.1.1.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turboctl
-Version: 1.1.1.dev2
+Version: 1.1.1.dev3
 Summary: TurboCtl is a RS-232 controller for a Leybold TURBOVAC i or iX turbovacuum pump.
 Author: Feliks Kivelä
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/fkivela/TurboCtl
 Keywords: RS-232,Turbovac
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
@@ -43,15 +43,15 @@
 
 The GitHub home page of the TurboCtl project can be found
 `here <https://github.com/fkivela/TurboCtl>`__.
 
 Version
 -------
 
-This is version 1.1.1.dev2 of TurboCtl.
+This is version 1.1.1.dev3 of TurboCtl.
 
 License
 -------
 
 TurboCtl is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `turboctl-1.1.1.dev2/README.rst` & `turboctl-1.1.1.dev3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 The GitHub home page of the TurboCtl project can be found
 `here <https://github.com/fkivela/TurboCtl>`__.
 
 Version
 -------
 
-This is version 1.1.1.dev2 of TurboCtl.
+This is version 1.1.1.dev3 of TurboCtl.
 
 License
 -------
 
 TurboCtl is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `turboctl-1.1.1.dev2/TODO` & `turboctl-1.1.1.dev3/TODO`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/add-to-path` & `turboctl-1.1.1.dev3/add-to-path`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/doc/sphinx/Makefile` & `turboctl-1.1.1.dev3/doc/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/doc/sphinx/advanced_UI.png` & `turboctl-1.1.1.dev3/doc/sphinx/advanced_UI.png`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/doc/sphinx/changelog.rst` & `turboctl-1.1.1.dev3/doc/sphinx/changelog.rst`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/doc/sphinx/conf.py` & `turboctl-1.1.1.dev3/doc/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/doc/sphinx/errata.rst` & `turboctl-1.1.1.dev3/doc/sphinx/errata.rst`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/doc/sphinx/index.rst` & `turboctl-1.1.1.dev3/doc/sphinx/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 The GitHub home page of the TurboCtl project can be found
 `here <https://github.com/fkivela/TurboCtl>`__.
 
 Version
 -------
 
-This is version 1.1.1.dev2 of TurboCtl.
+This is version 1.1.1.dev3 of TurboCtl.
 
 License
 -------
 
 TurboCtl is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `turboctl-1.1.1.dev2/doc/sphinx/installation.rst` & `turboctl-1.1.1.dev3/doc/sphinx/installation.rst`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/doc/sphinx/modules/virtualpump/parameter_component.rst` & `turboctl-1.1.1.dev3/doc/sphinx/modules/virtualpump/parameter_component.rst`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/doc/sphinx/modules.rst` & `turboctl-1.1.1.dev3/doc/sphinx/modules.rst`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/doc/sphinx/simple_UI.png` & `turboctl-1.1.1.dev3/doc/sphinx/simple_UI.png`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/doc/sphinx/usage.rst` & `turboctl-1.1.1.dev3/doc/sphinx/usage.rst`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/make-docs` & `turboctl-1.1.1.dev3/make-docs`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/make_readme.py` & `turboctl-1.1.1.dev3/make_readme.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/pyproject.toml` & `turboctl-1.1.1.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/run_tests/run_tests.py` & `turboctl-1.1.1.dev3/test_turboctl/run_tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/run_tests/test_run_tests.py` & `turboctl-1.1.1.dev3/test_turboctl/run_tests/test_run_tests.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/telegram/.hypothesis/unicode_data/11.0.0/charmap.json.gz` & `turboctl-1.1.1.dev3/test_turboctl/telegram/.hypothesis/unicode_data/11.0.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/telegram/test_api.py` & `turboctl-1.1.1.dev3/test_turboctl/telegram/test_api.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/telegram/test_codes.py` & `turboctl-1.1.1.dev3/test_turboctl/telegram/test_codes.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/telegram/test_datatypes.py` & `turboctl-1.1.1.dev3/test_turboctl/telegram/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/telegram/test_parser.py` & `turboctl-1.1.1.dev3/test_turboctl/telegram/test_parser.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/telegram/test_telegram.py` & `turboctl-1.1.1.dev3/test_turboctl/telegram/test_telegram.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/ui/test_abstractui.py` & `turboctl-1.1.1.dev3/test_turboctl/ui/test_abstractui.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/ui/test_command_parser.py` & `turboctl-1.1.1.dev3/test_turboctl/ui/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/ui/test_correct_error_message.py` & `turboctl-1.1.1.dev3/test_turboctl/ui/test_correct_error_message.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/ui/test_output.py` & `turboctl-1.1.1.dev3/test_turboctl/ui/test_output.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/ui/test_table.py` & `turboctl-1.1.1.dev3/test_turboctl/ui/test_table.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/ui/test_tui.py` & `turboctl-1.1.1.dev3/test_turboctl/ui/test_tui.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/virtualpump/test_hardware_component.py` & `turboctl-1.1.1.dev3/test_turboctl/virtualpump/test_hardware_component.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/virtualpump/test_parameter_component.py` & `turboctl-1.1.1.dev3/test_turboctl/virtualpump/test_parameter_component.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/virtualpump/test_virtualconnection.py` & `turboctl-1.1.1.dev3/test_turboctl/virtualpump/test_virtualconnection.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/test_turboctl/virtualpump/test_virtualpump.py` & `turboctl-1.1.1.dev3/test_turboctl/virtualpump/test_virtualpump.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/__main__.py` & `turboctl-1.1.1.dev3/turboctl/__main__.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/hacks.py` & `turboctl-1.1.1.dev3/turboctl/hacks.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/telegram/api.py` & `turboctl-1.1.1.dev3/turboctl/telegram/api.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/telegram/codes.py` & `turboctl-1.1.1.dev3/turboctl/telegram/codes.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/telegram/datatypes.py` & `turboctl-1.1.1.dev3/turboctl/telegram/datatypes.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/telegram/errors.txt` & `turboctl-1.1.1.dev3/turboctl/telegram/errors.txt`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/telegram/parameters.txt` & `turboctl-1.1.1.dev3/turboctl/telegram/parameters.txt`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/telegram/parser.py` & `turboctl-1.1.1.dev3/turboctl/telegram/parser.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/telegram/telegram.py` & `turboctl-1.1.1.dev3/turboctl/telegram/telegram.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/telegram/warnings.txt` & `turboctl-1.1.1.dev3/turboctl/telegram/warnings.txt`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/ui/advanced_tui.py` & `turboctl-1.1.1.dev3/turboctl/ui/advanced_tui.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/ui/command_line_ui.py` & `turboctl-1.1.1.dev3/turboctl/ui/command_line_ui.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/ui/control_interface.py` & `turboctl-1.1.1.dev3/turboctl/ui/control_interface.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/ui/queuefile.py` & `turboctl-1.1.1.dev3/turboctl/ui/queuefile.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/ui/status_format.py` & `turboctl-1.1.1.dev3/turboctl/ui/status_format.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/ui/table.py` & `turboctl-1.1.1.dev3/turboctl/ui/table.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/ui/widgets.py` & `turboctl-1.1.1.dev3/turboctl/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/virtualpump/hardware_component.py` & `turboctl-1.1.1.dev3/turboctl/virtualpump/hardware_component.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/virtualpump/parameter_component.py` & `turboctl-1.1.1.dev3/turboctl/virtualpump/parameter_component.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/virtualpump/virtualconnection.py` & `turboctl-1.1.1.dev3/turboctl/virtualpump/virtualconnection.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl/virtualpump/virtualpump.py` & `turboctl-1.1.1.dev3/turboctl/virtualpump/virtualpump.py`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl-run` & `turboctl-1.1.1.dev3/turboctl-run`

 * *Files identical despite different names*

### Comparing `turboctl-1.1.1.dev2/turboctl.egg-info/PKG-INFO` & `turboctl-1.1.1.dev3/turboctl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turboctl
-Version: 1.1.1.dev2
+Version: 1.1.1.dev3
 Summary: TurboCtl is a RS-232 controller for a Leybold TURBOVAC i or iX turbovacuum pump.
 Author: Feliks Kivelä
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/fkivela/TurboCtl
 Keywords: RS-232,Turbovac
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
@@ -43,15 +43,15 @@
 
 The GitHub home page of the TurboCtl project can be found
 `here <https://github.com/fkivela/TurboCtl>`__.
 
 Version
 -------
 
-This is version 1.1.1.dev2 of TurboCtl.
+This is version 1.1.1.dev3 of TurboCtl.
 
 License
 -------
 
 TurboCtl is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `turboctl-1.1.1.dev2/turboctl.egg-info/SOURCES.txt` & `turboctl-1.1.1.dev3/turboctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

