# Comparing `tmp/python-swiftclient-4.5.0.tar.gz` & `tmp/python-swiftclient-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-swiftclient-4.5.0.tar", last modified: Thu Feb 29 13:13:51 2024, max compression
+gzip compressed data, was "python-swiftclient-4.6.0.tar", last modified: Thu May 23 08:01:55 2024, max compression
```

## Comparing `python-swiftclient-4.5.0.tar` & `python-swiftclient-4.6.0.tar`

### file list

```diff
@@ -1,126 +1,127 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.965757 python-swiftclient-4.5.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/.coveragerc
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      279 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/.functests
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5894 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/.mailmap
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      357 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/.manpages
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/.stestr.conf
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      131 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/.unittests
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7167 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26833 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3674 2024-02-29 13:13:51.965757 python-swiftclient-4.5.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1754 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.949756 python-swiftclient-4.5.0/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      736 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/bin/swift
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.949756 python-swiftclient-4.5.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3186 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/Makefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.949756 python-swiftclient-4.5.0/doc/manpages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9073 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/manpages/swift.1
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.949756 python-swiftclient-4.5.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.949756 python-swiftclient-4.5.0/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/source/_static/.gitignore
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.949756 python-swiftclient-4.5.0/doc/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/source/_templates/.empty
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.949756 python-swiftclient-4.5.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29202 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4604 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/source/client-api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6613 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.949756 python-swiftclient-4.5.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/source/introduction.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31626 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/source/service-api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/doc/source/swiftclient.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.953756 python-swiftclient-4.5.0/examples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/examples/capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1130 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/examples/copy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/examples/delete.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1242 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/examples/download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/examples/list.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/examples/post.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/examples/stat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2570 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/examples/upload.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/pyproject.toml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.953756 python-swiftclient-4.5.0/python_swiftclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3674 2024-02-29 13:13:51.000000 python-swiftclient-4.5.0/python_swiftclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2895 2024-02-29 13:13:51.000000 python-swiftclient-4.5.0/python_swiftclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-29 13:13:51.000000 python-swiftclient-4.5.0/python_swiftclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-02-29 13:13:51.000000 python-swiftclient-4.5.0/python_swiftclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-29 13:13:51.000000 python-swiftclient-4.5.0/python_swiftclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-29 13:13:51.000000 python-swiftclient-4.5.0/python_swiftclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-02-29 13:13:51.000000 python-swiftclient-4.5.0/python_swiftclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2024-02-29 13:13:51.000000 python-swiftclient-4.5.0/python_swiftclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.941755 python-swiftclient-4.5.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.957756 python-swiftclient-4.5.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/notes/310-notes-03040158a8683dd8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/notes/320_notes-bb367dba1053d34c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/notes/340_notes-1777780bbfdb4d96.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/notes/350_notes-ad0ae19704b2eb88.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1368 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/notes/360_notes-1ec385df13a3a735.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/notes/361_notes-59e020e68bcdd709.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/notes/3_8_0_release-bd867fbdb8c895d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/notes/3_8_1_release-cb5648c3ae69bde1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/notes/3_9_0_release-3c293d277f14ec22.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1229 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/notes/4_3_0_release.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/notes/4_4_0_release-d731bab5982c160b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/notes/4_5_0_release-b315d25b889293f2.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.957756 python-swiftclient-4.5.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/2023.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10152 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/current.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1095 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1647 2024-02-29 13:13:51.965757 python-swiftclient-4.5.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.961756 python-swiftclient-4.5.0/swiftclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/swiftclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12680 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/swiftclient/authv1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    82165 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/swiftclient/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7762 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/swiftclient/command_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3453 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/swiftclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7848 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/swiftclient/multithreading.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2155 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/swiftclient/requests_compat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   120483 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/swiftclient/service.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    92789 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/swiftclient/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15761 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/swiftclient/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1608 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/swiftclient/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.961756 python-swiftclient-4.5.0/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.961756 python-swiftclient-4.5.0/test/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3821 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3661 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/functional/test_openstacksdk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21340 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/functional/test_swiftclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1177 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/sample.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.965757 python-swiftclient-4.5.0/test/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10744 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/unit/test_authv1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8474 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/unit/test_command_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8387 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/unit/test_multithreading.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   132508 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/unit/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   176701 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   150150 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/unit/test_swiftclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29719 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20954 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test/unit/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-29 13:13:51.965757 python-swiftclient-4.5.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/tools/swift.bash_completion
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3207 2024-02-29 13:12:56.000000 python-swiftclient-4.5.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.497597 python-swiftclient-4.6.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/.coveragerc
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      279 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/.functests
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5894 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/.mailmap
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      357 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/.manpages
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/.stestr.conf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      131 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/.unittests
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2398 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7167 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26833 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3725 2024-05-23 08:01:55.497597 python-swiftclient-4.6.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1754 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.477598 python-swiftclient-4.6.0/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      736 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/bin/swift
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.477598 python-swiftclient-4.6.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3186 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/Makefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.477598 python-swiftclient-4.6.0/doc/manpages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9073 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/manpages/swift.1
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.477598 python-swiftclient-4.6.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.477598 python-swiftclient-4.6.0/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/source/_static/.gitignore
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.477598 python-swiftclient-4.6.0/doc/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/source/_templates/.empty
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.477598 python-swiftclient-4.6.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29202 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4604 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/source/client-api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6613 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.477598 python-swiftclient-4.6.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/source/introduction.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31626 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/source/service-api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/doc/source/swiftclient.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.481598 python-swiftclient-4.6.0/examples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/examples/capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1130 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/examples/copy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/examples/delete.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1242 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/examples/download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/examples/list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/examples/post.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/examples/stat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2570 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/examples/upload.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/pyproject.toml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.481598 python-swiftclient-4.6.0/python_swiftclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3725 2024-05-23 08:01:55.000000 python-swiftclient-4.6.0/python_swiftclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2926 2024-05-23 08:01:55.000000 python-swiftclient-4.6.0/python_swiftclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:01:55.000000 python-swiftclient-4.6.0/python_swiftclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-05-23 08:01:55.000000 python-swiftclient-4.6.0/python_swiftclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:01:55.000000 python-swiftclient-4.6.0/python_swiftclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 08:01:55.000000 python-swiftclient-4.6.0/python_swiftclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-05-23 08:01:55.000000 python-swiftclient-4.6.0/python_swiftclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2024-05-23 08:01:55.000000 python-swiftclient-4.6.0/python_swiftclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.473598 python-swiftclient-4.6.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.485597 python-swiftclient-4.6.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/notes/310-notes-03040158a8683dd8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/notes/320_notes-bb367dba1053d34c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/notes/340_notes-1777780bbfdb4d96.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/notes/350_notes-ad0ae19704b2eb88.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1368 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/notes/360_notes-1ec385df13a3a735.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/notes/361_notes-59e020e68bcdd709.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/notes/3_8_0_release-bd867fbdb8c895d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/notes/3_8_1_release-cb5648c3ae69bde1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/notes/3_9_0_release-3c293d277f14ec22.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1229 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/notes/4_3_0_release.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/notes/4_4_0_release-d731bab5982c160b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/notes/4_5_0_release-b315d25b889293f2.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.489597 python-swiftclient-4.6.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/2024.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10152 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/current.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1095 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1687 2024-05-23 08:01:55.497597 python-swiftclient-4.6.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.489597 python-swiftclient-4.6.0/swiftclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/swiftclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12680 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/swiftclient/authv1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    82520 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/swiftclient/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7762 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/swiftclient/command_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3453 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/swiftclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8021 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/swiftclient/multithreading.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2155 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/swiftclient/requests_compat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   121167 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/swiftclient/service.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    92968 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/swiftclient/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15761 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/swiftclient/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1608 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/swiftclient/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.493597 python-swiftclient-4.6.0/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.493597 python-swiftclient-4.6.0/test/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3821 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3661 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/functional/test_openstacksdk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21340 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/functional/test_swiftclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1177 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/sample.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.497597 python-swiftclient-4.6.0/test/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10744 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/unit/test_authv1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9492 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/unit/test_command_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8387 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/unit/test_multithreading.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   134325 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/unit/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   183753 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   150969 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/unit/test_swiftclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29719 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20954 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test/unit/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:55.497597 python-swiftclient-4.6.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/tools/swift.bash_completion
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3207 2024-05-23 08:01:23.000000 python-swiftclient-4.6.0/tox.ini
```

### Comparing `python-swiftclient-4.5.0/.mailmap` & `python-swiftclient-4.6.0/.mailmap`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/.zuul.yaml` & `python-swiftclient-4.6.0/.zuul.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -38,31 +38,33 @@
       - release-notes-jobs-python3
     experimental:
       # on-demand pipeline used to test older (but still supported) versions of python,
       # as well as intermediate releases that the openstack-python3-jobs might skip
       jobs:
         - openstack-tox-py36
         - openstack-tox-py37
-        - openstack-tox-py39
+        - openstack-tox-py38
         - openstack-tox-py310
     check:
       jobs:
         - swiftclient-functional:
             irrelevant-files: &functest-irrelevant-files
               - ^(doc|releasenotes)/.*$
               - ^test/unit/.*$
               - ^(.gitreview|.mailmap|AUTHORS|ChangeLog|.*\.rst)$
         - swiftclient-swift-functional:
             irrelevant-files: *functest-irrelevant-files
         - tempest-full-py3:
             irrelevant-files: *functest-irrelevant-files
-        - openstack-tox-py311:
+        - openstack-tox-py311
+        - openstack-tox-py312:
             voting: true
     gate:
       jobs:
         - swiftclient-swift-functional
         - swiftclient-functional
-        - openstack-tox-py311:
+        - openstack-tox-py311
+        - openstack-tox-py312:
             voting: true
     post:
       jobs:
         - openstack-tox-cover
```

### Comparing `python-swiftclient-4.5.0/AUTHORS` & `python-swiftclient-4.6.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/CONTRIBUTING.rst` & `python-swiftclient-4.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/ChangeLog` & `python-swiftclient-4.6.0/ChangeLog`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/LICENSE` & `python-swiftclient-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/PKG-INFO` & `python-swiftclient-4.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-swiftclient
-Version: 4.5.0
+Version: 4.6.0
 Summary: OpenStack Object Storage API Client Library
 Home-page: https://docs.openstack.org/python-swiftclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Project-URL: Bug Tracker, https://bugs.launchpad.net/python-swiftclient
 Project-URL: Documentation, https://docs.openstack.org/python-swiftclient/latest/
@@ -72,12 +72,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: keystone
 Provides-Extra: test
```

### Comparing `python-swiftclient-4.5.0/README.rst` & `python-swiftclient-4.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/bin/swift` & `python-swiftclient-4.6.0/bin/swift`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/doc/Makefile` & `python-swiftclient-4.6.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/doc/manpages/swift.1` & `python-swiftclient-4.6.0/doc/manpages/swift.1`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/doc/source/cli/index.rst` & `python-swiftclient-4.6.0/doc/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/doc/source/client-api.rst` & `python-swiftclient-4.6.0/doc/source/client-api.rst`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/doc/source/conf.py` & `python-swiftclient-4.6.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/doc/source/contributor/contributing.rst` & `python-swiftclient-4.6.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/doc/source/index.rst` & `python-swiftclient-4.6.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/doc/source/introduction.rst` & `python-swiftclient-4.6.0/doc/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/doc/source/service-api.rst` & `python-swiftclient-4.6.0/doc/source/service-api.rst`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/doc/source/swiftclient.rst` & `python-swiftclient-4.6.0/doc/source/swiftclient.rst`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/examples/capabilities.py` & `python-swiftclient-4.6.0/examples/capabilities.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/examples/copy.py` & `python-swiftclient-4.6.0/examples/copy.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/examples/delete.py` & `python-swiftclient-4.6.0/examples/delete.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/examples/download.py` & `python-swiftclient-4.6.0/examples/download.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/examples/list.py` & `python-swiftclient-4.6.0/examples/list.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/examples/post.py` & `python-swiftclient-4.6.0/examples/post.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/examples/stat.py` & `python-swiftclient-4.6.0/examples/stat.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/examples/upload.py` & `python-swiftclient-4.6.0/examples/upload.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/python_swiftclient.egg-info/PKG-INFO` & `python-swiftclient-4.6.0/python_swiftclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-swiftclient
-Version: 4.5.0
+Version: 4.6.0
 Summary: OpenStack Object Storage API Client Library
 Home-page: https://docs.openstack.org/python-swiftclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Project-URL: Bug Tracker, https://bugs.launchpad.net/python-swiftclient
 Project-URL: Documentation, https://docs.openstack.org/python-swiftclient/latest/
@@ -72,12 +72,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: keystone
 Provides-Extra: test
```

### Comparing `python-swiftclient-4.5.0/python_swiftclient.egg-info/SOURCES.txt` & `python-swiftclient-4.6.0/python_swiftclient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 releasenotes/notes/3_8_1_release-cb5648c3ae69bde1.yaml
 releasenotes/notes/3_9_0_release-3c293d277f14ec22.yaml
 releasenotes/notes/4_3_0_release.yaml
 releasenotes/notes/4_4_0_release-d731bab5982c160b.yaml
 releasenotes/notes/4_5_0_release-b315d25b889293f2.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/current.rst
 releasenotes/source/index.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
```

### Comparing `python-swiftclient-4.5.0/releasenotes/notes/310-notes-03040158a8683dd8.yaml` & `python-swiftclient-4.6.0/releasenotes/notes/310-notes-03040158a8683dd8.yaml`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/releasenotes/notes/340_notes-1777780bbfdb4d96.yaml` & `python-swiftclient-4.6.0/releasenotes/notes/340_notes-1777780bbfdb4d96.yaml`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/releasenotes/notes/350_notes-ad0ae19704b2eb88.yaml` & `python-swiftclient-4.6.0/releasenotes/notes/350_notes-ad0ae19704b2eb88.yaml`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/releasenotes/notes/360_notes-1ec385df13a3a735.yaml` & `python-swiftclient-4.6.0/releasenotes/notes/360_notes-1ec385df13a3a735.yaml`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/releasenotes/notes/4_3_0_release.yaml` & `python-swiftclient-4.6.0/releasenotes/notes/4_3_0_release.yaml`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/releasenotes/source/conf.py` & `python-swiftclient-4.6.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/run_tests.sh` & `python-swiftclient-4.6.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/setup.cfg` & `python-swiftclient-4.6.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: 3 :: Only
 
 [files]
 packages = 
 	swiftclient
 data_files = 
 	share/man/man1 = doc/manpages/swift.1
```

### Comparing `python-swiftclient-4.5.0/setup.py` & `python-swiftclient-4.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/swiftclient/__init__.py` & `python-swiftclient-4.6.0/swiftclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/swiftclient/authv1.py` & `python-swiftclient-4.6.0/swiftclient/authv1.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/swiftclient/client.py` & `python-swiftclient-4.6.0/swiftclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,21 @@
 
 """
 OpenStack Swift client library used internally
 """
 import socket
 import re
 import logging
+from urllib3.exceptions import HTTPError as urllib_http_error
+
 import warnings
 
 from requests.exceptions import RequestException, SSLError
 import http.client as http_client
+from requests.structures import CaseInsensitiveDict
 from urllib.parse import quote, unquote
 from urllib.parse import urljoin, urlparse, urlunparse
 from time import sleep, time
 
 from swiftclient import version as swiftclient_version
 from swiftclient.exceptions import ClientException
 from swiftclient.requests_compat import SwiftClientRequestsSession
@@ -205,14 +208,23 @@
                 header.startswith(USER_METADATA_TYPE)):
             header = encode_utf8(header)
 
         ret[header] = value
     return ret
 
 
+class LowerKeyCaseInsensitiveDict(CaseInsensitiveDict):
+    """
+    CaseInsensitiveDict returning lower case keys for items()
+    """
+
+    def __iter__(self):
+        return iter(self._store.keys())
+
+
 class _ObjectBody:
     """
     Readable and iterable object body response wrapper.
     """
 
     def __init__(self, resp, chunk_size, conn_to_close):
         """
@@ -283,15 +295,15 @@
         self.bytes_read = 0
 
     def read(self, length=None):
         buf = None
         try:
             buf = self.resp.read(length)
             self.bytes_read += len(buf)
-        except (socket.error, RequestException):
+        except (socket.error, urllib_http_error, RequestException):
             if self.conn.attempts > self.conn.retries:
                 raise
         if (not buf and self.bytes_read < self.expected_length and
                 self.conn.attempts <= self.conn.retries):
             self.headers['Range'] = 'bytes=%d-' % self.bytes_read
             self.headers['If-Match'] = self.resp.getheader('ETag')
             hdrs, body = self.conn._retry(None, get_object,
@@ -731,17 +743,17 @@
     if os_options.get('object_storage_url'):
         return os_options['object_storage_url'], token
     else:
         return storage_url, token
 
 
 def resp_header_dict(resp):
-    resp_headers = {}
+    resp_headers = LowerKeyCaseInsensitiveDict()
     for header, value in resp.getheaders():
-        header = parse_header_string(header).lower()
+        header = parse_header_string(header)
         resp_headers[header] = parse_header_string(value)
     return resp_headers
 
 
 def store_response(resp, response_dict):
     """
     store information about an operation into a dict
@@ -1922,14 +1934,15 @@
                                      headers=headers)
         is_not_range_request = (
             not headers or 'range' not in (k.lower() for k in headers))
         retry_is_possible = (
             is_not_range_request and resp_chunk_size and
             self.attempts <= self.retries and
             rheaders.get('transfer-encoding') is None)
+
         if retry_is_possible:
             body = _RetryBody(body.resp, self, container, obj,
                               resp_chunk_size=resp_chunk_size,
                               query_string=query_string,
                               response_dict=response_dict,
                               headers=headers)
         return rheaders, body
```

### Comparing `python-swiftclient-4.5.0/swiftclient/command_helpers.py` & `python-swiftclient-4.6.0/swiftclient/command_helpers.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/swiftclient/exceptions.py` & `python-swiftclient-4.6.0/swiftclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/swiftclient/multithreading.py` & `python-swiftclient-4.6.0/swiftclient/multithreading.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,18 @@
             self.print_msg((template % (k, v)).rstrip())
 
     def error(self, msg, *fmt_args):
         if fmt_args:
             msg = msg % fmt_args
         self.error_print_pool.submit(self._print_error, msg)
 
+    def error_with_txn_id(self, swift_err):
+        self.error("{}\nFailed Transaction ID: {}".format(
+            swift_err.value, swift_err.transaction_id or 'unknown'))
+
     def get_error_count(self):
         return self.error_count
 
     def _print(self, item, stream=None):
         if stream is None:
             stream = self.print_stream
         print(item, file=stream)
```

### Comparing `python-swiftclient-4.5.0/swiftclient/requests_compat.py` & `python-swiftclient-4.6.0/swiftclient/requests_compat.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/swiftclient/service.py` & `python-swiftclient-4.6.0/swiftclient/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 )
 from posixpath import join as urljoin
 from random import shuffle
 from time import time
 from threading import Thread
 from queue import Queue
 from queue import Empty as QueueEmpty
+from requests.exceptions import RequestException
+from socket import error as socket_error
+from urllib3.exceptions import HTTPError as urllib_http_error
 from urllib.parse import quote
 
 import json
 
 
 from swiftclient import Connection
 from swiftclient.command_helpers import (
@@ -64,20 +67,24 @@
     def __next__(self):
         next_completed_future = next(self.futures)
         return next_completed_future.result()
 
 
 class SwiftError(Exception):
     def __init__(self, value, container=None, obj=None,
-                 segment=None, exc=None):
+                 segment=None, exc=None, transaction_id=None):
         self.value = value
         self.container = container
         self.obj = obj
         self.segment = segment
         self.exception = exc
+        if transaction_id is None:
+            self.transaction_id = getattr(exc, 'transaction_id', None)
+        else:
+            self.transaction_id = transaction_id
 
     def __str__(self):
         value = repr(self.value)
         if self.container is not None:
             value += " container:%s" % self.container
         if self.obj is not None:
             value += " object:%s" % self.obj
@@ -455,15 +462,17 @@
         if self._expected_md5 and checksum:
             self._actual_md5 = md5()
 
         if 'content-length' in headers:
             try:
                 self._content_length = int(headers.get('content-length'))
             except ValueError:
-                raise SwiftError('content-length header must be an integer')
+                raise SwiftError(
+                    'content-length header must be an integer',
+                    transaction_id=self._txn_id)
 
     def __iter__(self):
         for chunk in self._body:
             if self._actual_md5:
                 self._actual_md5.update(chunk)
             self._actual_read += len(chunk)
             yield chunk
@@ -1302,17 +1311,23 @@
                             fp = open(out_file, 'wb', DISK_BUFFER)
                         else:
                             if basename(path):
                                 fp = open(path, 'wb', DISK_BUFFER)
                             else:
                                 pseudodir = True
 
-                for chunk in obj_body:
-                    if fp is not None:
-                        fp.write(chunk)
+                try:
+                    for chunk in obj_body:
+                        if fp is not None:
+                            fp.write(chunk)
+                except (socket_error,
+                        urllib_http_error,
+                        RequestException) as err:
+                    raise ClientException(
+                        str(err), http_response_headers=headers)
 
                 finish_time = time()
 
             finally:
                 bytes_read = obj_body.bytes_read()
                 if fp is not None:
                     fp.close()
```

### Comparing `python-swiftclient-4.5.0/swiftclient/shell.py` & `python-swiftclient-4.6.0/swiftclient/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 
                             output_manager.print_msg('{0}{1}'.format(p, a))
                     else:
                         p = '{0}/{1}'.format(c, o) if o else c
                         output_manager.error('Error Deleting: {0}: {1}'
                                              .format(p, r['error']))
         except SwiftError as err:
-            output_manager.error(err.value)
+            output_manager.error_with_txn_id(err)
 
 
 st_download_options = '''[--all] [--marker <marker>] [--prefix <prefix>]
                       [--output <out_file>] [--output-dir <out_directory>]
                       [--object-threads <threads>] [--ignore-checksum]
                       [--container-threads <threads>] [--no-download]
                       [--skip-identical] [--remove-prefix]
@@ -480,19 +480,21 @@
                                     "Skipped identical file '%s'", path)
                                 continue
                             if error.http_status == 404:
                                 output_manager.error(
                                     "Object '%s/%s' not found", container, obj)
                                 continue
                         output_manager.error(
-                            "Error downloading object '%s/%s': %s",
-                            container, obj, error)
+                            "Error downloading object '%s/%s': %s\n"
+                            "Failed Transaction ID: %s",
+                            container, obj, error,
+                            getattr(error, 'transaction_id', 'unknown'))
 
         except SwiftError as e:
-            output_manager.error(e.value)
+            output_manager.error_with_txn_id(e)
         except Exception as e:
             output_manager.error(e)
 
 
 st_list_options = '''[--long] [--lh] [--totals] [--prefix <prefix>]
                   [--delimiter <delimiter>] [--header <header:value>]
                   [--versions] [<container>]
@@ -666,15 +668,15 @@
                         "%12s %s", prt_bytes(totals['count'], True),
                         prt_bytes(totals['bytes'], human))
                 else:
                     output_manager.print_msg(
                         prt_bytes(totals['bytes'], human))
 
         except SwiftError as e:
-            output_manager.error(e.value)
+            output_manager.error_with_txn_id(e)
 
 
 st_stat_options = '''[--lh] [--header <header:value>]
                   [--version-id <version_id>]
                   [<container> [<object>]]
 '''
 
@@ -757,15 +759,15 @@
                                 raise stat_result["error"]
                     else:
                         output_manager.error(
                             'Usage: %s stat %s\n%s', BASENAME,
                             st_stat_options, st_stat_help)
 
         except SwiftError as e:
-            output_manager.error(e.value)
+            output_manager.error_with_txn_id(e)
 
 
 st_post_options = '''[--read-acl <acl>] [--write-acl <acl>] [--sync-to <sync-to>]
                   [--sync-key <sync-key>] [--meta <name:value>]
                   [--header <header>]
                   [<container> [<object>]]
 '''  # noqa
@@ -863,15 +865,15 @@
                         return
                 else:
                     result = swift.post(container=container)
             if not result["success"]:
                 raise result["error"]
 
         except SwiftError as e:
-            output_manager.error(e.value)
+            output_manager.error_with_txn_id(e)
 
 
 st_copy_options = '''[--destination </container/object>] [--fresh-metadata]
                   [--meta <name:value>] [--header <header>] <container>
                   <object> [<object>] [...]
 '''
 
@@ -968,15 +970,15 @@
             else:
                 output_manager.error(
                     'Usage: %s copy %s\n%s', BASENAME,
                     st_copy_options, st_copy_help)
                 return
 
         except SwiftError as e:
-            output_manager.error(e.value)
+            output_manager.error_with_txn_id(e)
 
 
 st_upload_options = '''[--changed] [--skip-identical] [--segment-size <size>]
                     [--segment-container <container>] [--leave-segments]
                     [--object-threads <thread>] [--segment-threads <threads>]
                     [--meta <name:value>] [--header <header>] [--use-slo]
                     [--use-dlo] [--ignore-checksum] [--skip-container-put]
@@ -1266,15 +1268,15 @@
                                      error.http_status == 413)
                         if too_large and options['verbose'] > 0:
                             output_manager.error(
                                 "Consider using the --segment-size option "
                                 "to chunk the object")
 
         except SwiftError as e:
-            output_manager.error(e.value)
+            output_manager.error_with_txn_id(e)
 
 
 st_capabilities_options = '''[--json] [<proxy_url>]
 '''
 st_info_options = st_capabilities_options
 st_capabilities_help = '''
 Retrieve capability of the proxy.
@@ -1328,15 +1330,15 @@
                     json.dumps(capabilities, sort_keys=True, indent=2))
             else:
                 capabilities = dict(capabilities)
                 _print_compo_cap('Core', {'swift': capabilities['swift']})
                 del capabilities['swift']
                 _print_compo_cap('Additional middleware', capabilities)
         except SwiftError as e:
-            output_manager.error(e.value)
+            output_manager.error_with_txn_id(e)
 
 
 st_info = st_capabilities
 
 st_auth_help = '''
 Display auth related authentication variables in shell friendly format.
```

### Comparing `python-swiftclient-4.5.0/swiftclient/utils.py` & `python-swiftclient-4.6.0/swiftclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/swiftclient/version.py` & `python-swiftclient-4.6.0/swiftclient/version.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/test/functional/__init__.py` & `python-swiftclient-4.6.0/test/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/test/functional/test_openstacksdk.py` & `python-swiftclient-4.6.0/test/functional/test_openstacksdk.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/test/functional/test_swiftclient.py` & `python-swiftclient-4.6.0/test/functional/test_swiftclient.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/test/sample.conf` & `python-swiftclient-4.6.0/test/sample.conf`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/test/unit/test_authv1.py` & `python-swiftclient-4.6.0/test/unit/test_authv1.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/test/unit/test_command_helpers.py` & `python-swiftclient-4.6.0/test/unit/test_command_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 
 from io import StringIO
 import unittest
 from unittest import mock
 
 from swiftclient import command_helpers as h
+from swiftclient.client import LowerKeyCaseInsensitiveDict
 from swiftclient.multithreading import OutputManager
 
 
 class TestStatHelpers(unittest.TestCase):
 
     def setUp(self):
         super(TestStatHelpers, self).setUp()
@@ -233,14 +234,41 @@
         self.conn.head_object.return_value = stub_headers
         args = ('c', 'o')
         with self.output_manager as output_manager:
             items, headers = h.stat_object(self.conn, self.options, *args)
             h.print_object_stats(items, headers, output_manager)
         expected = """
              URL: http://storage/v1/a/c/o
+      Auth Token: tk12345
+         Account: a
+       Container: c
+          Object: o
+  Content Length: 1048576
+            ETag: 68b329da9893e34099c7d8ad5cb9c940
+      Meta Color: blue
+Content-Encoding: gzip
+"""
+        self.assertOut(expected)
+
+    def test_stat_object_case_insensitive_headers(self):
+        self.options['verbose'] += 1
+        # stub head object request
+        stub_headers = LowerKeyCaseInsensitiveDict({
+            'content-length': 2 ** 20,
+            'x-object-meta-color': 'blue',
+            'ETag': '68b329da9893e34099c7d8ad5cb9c940',
+            'content-encoding': 'gzip',
+        })
+        self.conn.head_object.return_value = stub_headers
+        args = ('c', 'o')
+        with self.output_manager as output_manager:
+            items, headers = h.stat_object(self.conn, self.options, *args)
+            h.print_object_stats(items, headers, output_manager)
+        expected = """
+             URL: http://storage/v1/a/c/o
       Auth Token: tk12345
          Account: a
        Container: c
           Object: o
   Content Length: 1048576
             ETag: 68b329da9893e34099c7d8ad5cb9c940
       Meta Color: blue
```

### Comparing `python-swiftclient-4.5.0/test/unit/test_multithreading.py` & `python-swiftclient-4.6.0/test/unit/test_multithreading.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/test/unit/test_service.py` & `python-swiftclient-4.6.0/test/unit/test_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 from concurrent.futures import Future
 from hashlib import md5
 from queue import Queue, Empty as QueueEmptyError
 from time import sleep
 
 import swiftclient
 import swiftclient.utils as utils
-from swiftclient.client import Connection, ClientException
+from swiftclient.client import (
+    Connection, ClientException, LowerKeyCaseInsensitiveDict
+)
 from swiftclient.service import (
     SwiftService, SwiftError, SwiftUploadObject, SwiftDeleteObject
 )
 
 from test.unit import utils as test_utils
 
 
@@ -163,16 +165,18 @@
         self.assertEqual(sr._body, 'body')
         self.assertEqual(sr._content_length, 5)
         self.assertFalse(sr._expected_md5)
 
         self.assertIsNone(sr._actual_md5)
 
         # Check Contentlength raises error if it isn't an integer
-        self.assertRaises(SwiftError, self.sr, 'path', 'body',
-                          {'content-length': 'notanint'})
+        with self.assertRaises(SwiftError) as cm:
+            self.sr('path', 'body', {'content-length': 'notanint'})
+        self.assertEqual("'content-length header must be an integer'",
+                         str(cm.exception))
 
     def test_iterator_usage(self):
         def _consume(sr):
             for _ in sr:
                 pass
 
         sr = self.sr('path', BytesIO(b'body'), {})
@@ -235,14 +239,34 @@
                      {'content-length': 9,
                       'etag': md5('abc'.encode() * 3).hexdigest()})
         _consume(sr)
         self.assertEqual(sr._actual_read, 9)
         self.assertEqual(sr._actual_md5.hexdigest(),
                          md5('abc'.encode() * 3).hexdigest())
 
+    def test_swift_reader_knows_slo_etag_is_not_md5(self):
+        segment_bodies = [b'abc', b'def', b'ghi']
+        # slo etag is md5 of the sum of md5 of segments
+        slo_etag = md5(b''.join(
+            md5(b).hexdigest().encode()
+            for b in segment_bodies
+        )).hexdigest()
+        headers = LowerKeyCaseInsensitiveDict({
+            'Content-Length': len(b''.join(segment_bodies)),
+            'X-Static-Large-Object': 'true',
+            'ETag': '"%s"' % slo_etag
+        })
+        sr = self.sr('path', segment_bodies, headers)
+        # x-static-large-object; so no exception is raised!
+        actual_md5 = md5(b''.join(sr)).hexdigest()
+        self.assertEqual(sr._actual_read, 9)
+        self.assertIsNone(sr._actual_md5)
+        self.assertEqual(actual_md5,
+                         md5(b''.join(segment_bodies)).hexdigest())
+
 
 class _TestServiceBase(unittest.TestCase):
     def _get_mock_connection(self, attempts=2):
         m = mock.Mock(spec=Connection)
         type(m).attempts = mock.PropertyMock(return_value=attempts)
         type(m).auth_end_time = mock.PropertyMock(return_value=4)
         return m
@@ -649,26 +673,46 @@
         self.assertEqual(se.value, 5)
         self.assertIsNone(se.container)
         self.assertIsNone(se.obj)
         self.assertIsNone(se.segment)
         self.assertIsNone(se.exception)
 
         self.assertEqual(str(se), '5')
+        self.assertNotIn(str(se), 'Transaction ID')
 
     def test_swifterror_creation(self):
         test_exc = Exception('test exc')
         se = SwiftError(5, 'con', 'obj', 'seg', test_exc)
 
         self.assertEqual(se.value, 5)
         self.assertEqual(se.container, 'con')
         self.assertEqual(se.obj, 'obj')
         self.assertEqual(se.segment, 'seg')
         self.assertEqual(se.exception, test_exc)
 
         self.assertEqual(str(se), '5 container:con object:obj segment:seg')
+        self.assertNotIn(str(se), 'Transaction ID')
+
+    def test_swifterror_clientexception_creation(self):
+        test_exc = ClientException(
+            Exception('test exc'),
+            http_response_headers=LowerKeyCaseInsensitiveDict({
+                'x-trans-id': 'someTransId'})
+        )
+        se = SwiftError(5, 'con', 'obj', 'seg', test_exc)
+
+        self.assertEqual(se.value, 5)
+        self.assertEqual(se.container, 'con')
+        self.assertEqual(se.obj, 'obj')
+        self.assertEqual(se.segment, 'seg')
+        self.assertEqual(se.exception, test_exc)
+
+        self.assertEqual('someTransId', se.transaction_id)
+        self.assertNotIn('someTransId', str(se))
+        self.assertIn('5 container:con object:obj segment:seg', str(se))
 
 
 class TestServiceUtils(unittest.TestCase):
 
     def setUp(self):
         super(TestServiceUtils, self).setUp()
         with mock.patch.dict(swiftclient.service.environ, clean_os_environ):
```

### Comparing `python-swiftclient-4.5.0/test/unit/test_shell.py` & `python-swiftclient-4.6.0/test/unit/test_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,31 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 # implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 import contextlib
+import socket
 from genericpath import getmtime
 import getpass
 import hashlib
 import json
 import logging
 import os
 import tempfile
 import unittest
 from unittest import mock
 import textwrap
 from time import localtime, mktime, strftime, strptime
+from requests.exceptions import RequestException
+from urllib3.exceptions import HTTPError
 
 import swiftclient
+from swiftclient.client import LowerKeyCaseInsensitiveDict
 from swiftclient.service import SwiftError
 import swiftclient.shell
 import swiftclient.utils
 
 from os.path import basename, dirname
 from .utils import (
     CaptureOutput, fake_get_auth_keystone,
@@ -232,14 +236,36 @@
                              '    Bytes: 2\n'
                              ' Read ACL: test2:tester2\n'
                              'Write ACL: test3:tester3\n'
                              '  Sync To: other\n'
                              ' Sync Key: secret\n')
 
     @mock.patch('swiftclient.service.Connection')
+    def test_stat_container_not_found(self, connection):
+        connection.return_value.head_container.side_effect = \
+            swiftclient.ClientException(
+                'test',
+                http_status=404,
+                http_response_headers=LowerKeyCaseInsensitiveDict({
+                    'x-trans-id': 'someTransId'})
+            )
+        argv = ["", "stat", "container"]
+
+        with CaptureOutput() as output:
+            with self.assertRaises(SystemExit):
+                swiftclient.shell.main(argv)
+                connection.return_value.head_container.assert_called_with(
+                    'container', headers={}, resp_chunk_size=65536,
+                    response_dict={})
+
+            self.assertIn('Container \'container\' not found\n'
+                          'Failed Transaction ID: someTransId',
+                          output.err)
+
+    @mock.patch('swiftclient.service.Connection')
     def test_stat_container_with_headers(self, connection):
         return_headers = {
             'x-container-object-count': '1',
             'x-container-bytes-used': '2',
             'x-container-read': 'test2:tester2',
             'x-container-write': 'test3:tester3',
             'x-container-sync-to': 'other',
@@ -310,14 +336,35 @@
                              '  Content Type: text/plain\n'
                              'Content Length: 42\n'
                              ' Last Modified: yesterday\n'
                              '          ETag: md5\n'
                              '      Manifest: manifest\n')
 
     @mock.patch('swiftclient.service.Connection')
+    def test_stat_object_not_found(self, connection):
+        connection.return_value.head_object.side_effect = \
+            swiftclient.ClientException(
+                'test', http_status=404,
+                http_response_headers=LowerKeyCaseInsensitiveDict({
+                    'x-trans-id': 'someTransId'})
+            )
+        argv = ["", "stat", "container", "object"]
+
+        with CaptureOutput() as output:
+            with self.assertRaises(SystemExit):
+                swiftclient.shell.main(argv)
+                connection.return_value.head_object.assert_called_with(
+                    'container', 'object', headers={}, resp_chunk_size=65536,
+                    response_dict={})
+
+            self.assertIn('test: 404\n'
+                          'Failed Transaction ID: someTransId',
+                          output.err)
+
+    @mock.patch('swiftclient.service.Connection')
     def test_stat_object_with_headers(self, connection):
         return_headers = {
             'x-object-manifest': 'manifest',
             'etag': 'md5',
             'last-modified': 'yesterday',
             'content-type': 'text/plain',
             'content-length': 42,
@@ -731,14 +778,125 @@
              objcontent)
         ]
         with CaptureOutput() as output:
             argv = ["", "download", "--output", "-", "container", "object"]
             swiftclient.shell.main(argv)
             self.assertEqual('objcontent', output.out)
 
+    def _do_test_download_clientexception(self, exc):
+        retry_calls = []
+
+        def _fake_retry(conn, *args, **kwargs):
+            retry_calls.append((args, kwargs))
+            conn.attempts += 1
+
+            body = mock.MagicMock()
+            body.resp.read.side_effect = RequestException('test_exc')
+            return (LowerKeyCaseInsensitiveDict({
+                'content-type': 'text/plain',
+                'etag': '2cbbfe139a744d6abbe695e17f3c1991',
+                'x-trans-id': 'someTransId'}),
+                body)
+
+        argv = ["", "download", "container", "object", "--retries", "1"]
+        with CaptureOutput() as output:
+            with mock.patch(BUILTIN_OPEN) as mock_open:
+                with mock.patch("swiftclient.service.Connection._retry",
+                                _fake_retry):
+                    with self.assertRaises(SystemExit):
+                        swiftclient.shell.main(argv)
+                    mock_open.assert_called_with('object', 'wb', 65536)
+            self.assertEqual([
+                ((None, swiftclient.client.get_object, 'container', 'object'),
+                 {'headers': {},
+                  'query_string': None,
+                  'resp_chunk_size': 65536,
+                  'response_dict': {}}),
+                ((None, swiftclient.client.get_object, 'container', 'object'),
+                 {'attempts': 1,
+                  'headers': {'If-Match': mock.ANY, 'Range': 'bytes=0-'},
+                  'query_string': None,
+                  'resp_chunk_size': 65536,
+                  'response_dict': {}})],
+                retry_calls)
+            self.assertIn('Error downloading object \'container/object\': '
+                          'test_exc',
+                          str(output.err))
+            self.assertIn('someTransId', str(output.err))
+
+    def test_download_request_exception(self):
+        self._do_test_download_clientexception(RequestException('text_exc'))
+
+    def test_download_socket_error(self):
+        self._do_test_download_clientexception(socket.error())
+
+    def test_download_http_error(self):
+        self._do_test_download_clientexception(HTTPError)
+
+    def test_download_request_exception_retries_0(self):
+        retry_calls = []
+
+        def _fake_retry(conn, *args, **kwargs):
+            retry_calls.append((args, kwargs))
+            conn.attempts += 1
+
+            body = mock.MagicMock()
+            body.__iter__.side_effect = RequestException('test_exc')
+            return (LowerKeyCaseInsensitiveDict({
+                'content-type': 'text/plain',
+                'etag': '2cbbfe139a744d6abbe695e17f3c1991',
+                'x-trans-id': 'someTransId'}),
+                body)
+
+        argv = ["", "download", "container", "object", "--retries", "0"]
+        with CaptureOutput() as output:
+            with mock.patch(BUILTIN_OPEN) as mock_open:
+                with mock.patch("swiftclient.service.Connection._retry",
+                                _fake_retry):
+                    with self.assertRaises(SystemExit):
+                        swiftclient.shell.main(argv)
+                    mock_open.assert_called_with('object', 'wb', 65536)
+            self.assertEqual([
+                ((None, swiftclient.client.get_object, 'container', 'object'),
+                 {'headers': {},
+                  'query_string': None,
+                  'resp_chunk_size': 65536,
+                  'response_dict': {}}), ],
+                retry_calls)
+            self.assertIn('Error downloading object \'container/object\': '
+                          'test_exc',
+                          str(output.err))
+            self.assertIn('someTransId', str(output.err))
+
+    @mock.patch('swiftclient.service.Connection')
+    def test_download_bad_content_length(self, connection):
+        objcontent = io.BytesIO(b'objcontent')
+        connection.return_value.get_object.side_effect = [
+            (LowerKeyCaseInsensitiveDict({
+                'content-type': 'text/plain',
+                'content-length': 'BAD',
+                'etag': '2cbbfe139a744d6abbe695e17f3c1991',
+                'x-trans-id': 'someTransId'}),
+             objcontent)
+        ]
+        with CaptureOutput() as output:
+            with self.assertRaises(SystemExit):
+                with mock.patch(BUILTIN_OPEN) as mock_open:
+                    argv = ["", "download", "container", "object"]
+                    swiftclient.shell.main(argv)
+                connection.return_value.get_object.assert_called_with(
+                    'container', 'object', headers={}, resp_chunk_size=65536,
+                    response_dict={})
+                mock_open.assert_called_with('object', 'wb', 65536)
+
+            self.assertIn("Error downloading object \'container/object\': "
+                          "'content-length header must be an integer'"
+                          "\nFailed Transaction ID: someTransId",
+                          str(output.err))
+
     @mock.patch('swiftclient.service.shuffle')
     @mock.patch('swiftclient.service.Connection')
     def test_download_shuffle(self, connection, mock_shuffle):
         # Test that the container and object lists are shuffled
         mock_shuffle.side_effect = lambda to_shuffle: to_shuffle
         connection.return_value.get_object.return_value = [
             {'content-type': 'text/plain',
@@ -1926,15 +2084,17 @@
         connection.return_value.post_account.side_effect = \
             swiftclient.ClientException('test', http_status=404)
 
         with CaptureOutput() as output:
             with self.assertRaises(SystemExit):
                 swiftclient.shell.main(argv)
 
-            self.assertEqual(output.err, 'Account not found\n')
+            self.assertEqual(
+                output.err,
+                'Account not found\nFailed Transaction ID: unknown\n')
 
     @mock.patch('swiftclient.service.Connection')
     def test_post_container(self, connection):
         argv = ["", "post", "container"]
         swiftclient.shell.main(argv)
         connection.return_value.post_container.assert_called_with(
             'container', headers={}, response_dict={})
@@ -2118,15 +2278,16 @@
         with CaptureOutput() as output:
             with self.assertRaises(SystemExit):
                 swiftclient.shell.main(argv)
 
             self.assertEqual(
                 output.err,
                 'Combination of multiple objects and destination '
-                'including object is invalid\n')
+                'including object is invalid\n'
+                'Failed Transaction ID: unknown\n')
 
     @mock.patch('swiftclient.service.Connection')
     def test_copy_object_bad_auth(self, connection):
         argv = ["", "copy", "container", "object"]
         connection.return_value.copy_object.side_effect = \
             swiftclient.ClientException("bad auth")
```

### Comparing `python-swiftclient-4.5.0/test/unit/test_swiftclient.py` & `python-swiftclient-4.6.0/test/unit/test_swiftclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -1113,14 +1113,33 @@
                           'X-Binary-Header': b'\xff'})
         conn = c.http_connection('http://www.test.com')
         headers, data = c.get_object('url_is_irrelevant', 'TOKEN',
                                      'container', 'object', http_conn=conn)
         self.assertEqual('t\xe9st', headers.get('x-utf-8-header', ''))
         self.assertEqual('%ff', headers.get('x-non-utf-8-header', ''))
         self.assertEqual('%FF', headers.get('x-binary-header', ''))
+        for k, v in headers.items():
+            # N.B. k is always lower case!
+            self.assertTrue(k.islower())
+        for k in headers.keys():
+            # N.B. k is always lower case!
+            self.assertTrue(k.islower())
+        self.assertTrue(set([
+            'x-utf-8-header',
+            'x-non-utf-8-header',
+            'x-binary-header',
+        ]).intersection(headers))
+
+        self.assertEqual('t\xe9st', headers.get('X-Utf-8-Header', ''))
+        self.assertEqual('%ff', headers.get('X-Non-Utf-8-Header', ''))
+        self.assertEqual('%FF', headers.get('X-Binary-Header', ''))
+
+        self.assertEqual('t\xe9st', headers.get('X-UTF-8-HEADER', ''))
+        self.assertEqual('%ff', headers.get('X-NON-UTF-8-HEADER', ''))
+        self.assertEqual('%FF', headers.get('X-BINARY-HEADER', ''))
 
     def test_chunk_size_read_method(self):
         conn = c.Connection('http://auth.url/', 'some_user', 'some_key')
         with mock.patch('swiftclient.client.get_auth_1_0') as mock_get_auth:
             mock_get_auth.return_value = ('http://auth.url/', 'tToken')
             c.http_connection = self.fake_http_connection(200, body='abcde')
             __, resp = conn.get_object('asdf', 'asdf', resp_chunk_size=3)
```

### Comparing `python-swiftclient-4.5.0/test/unit/test_utils.py` & `python-swiftclient-4.6.0/test/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/test/unit/utils.py` & `python-swiftclient-4.6.0/test/unit/utils.py`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/tools/swift.bash_completion` & `python-swiftclient-4.6.0/tools/swift.bash_completion`

 * *Files identical despite different names*

### Comparing `python-swiftclient-4.5.0/tox.ini` & `python-swiftclient-4.6.0/tox.ini`

 * *Files identical despite different names*

