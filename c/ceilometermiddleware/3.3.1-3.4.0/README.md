# Comparing `tmp/ceilometermiddleware-3.3.1.tar.gz` & `tmp/ceilometermiddleware-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ceilometermiddleware-3.3.1.tar", last modified: Fri Feb 23 08:58:32 2024, max compression
+gzip compressed data, was "ceilometermiddleware-3.4.0.tar", last modified: Thu May 23 08:02:09 2024, max compression
```

## Comparing `ceilometermiddleware-3.3.1.tar` & `ceilometermiddleware-3.4.0.tar`

### file list

```diff
@@ -1,72 +1,75 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:32.418164 ceilometermiddleware-3.3.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2024-02-23 08:58:32.000000 ceilometermiddleware-3.3.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5644 2024-02-23 08:58:32.000000 ceilometermiddleware-3.3.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2024-02-23 08:58:32.418164 ceilometermiddleware-3.3.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      671 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:32.410164 ceilometermiddleware-3.3.1/ceilometermiddleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/ceilometermiddleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15058 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/ceilometermiddleware/swift.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:32.414164 ceilometermiddleware-3.3.1/ceilometermiddleware/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/ceilometermiddleware/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/ceilometermiddleware/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:32.414164 ceilometermiddleware-3.3.1/ceilometermiddleware/tests/data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14661 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/ceilometermiddleware/tests/data/list_projects.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22710 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/ceilometermiddleware/tests/test_swift.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:32.410164 ceilometermiddleware-3.3.1/ceilometermiddleware.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2024-02-23 08:58:32.000000 ceilometermiddleware-3.3.1/ceilometermiddleware.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1788 2024-02-23 08:58:32.000000 ceilometermiddleware-3.3.1/ceilometermiddleware.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-23 08:58:32.000000 ceilometermiddleware-3.3.1/ceilometermiddleware.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-02-23 08:58:32.000000 ceilometermiddleware-3.3.1/ceilometermiddleware.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-23 08:58:32.000000 ceilometermiddleware-3.3.1/ceilometermiddleware.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-23 08:58:32.000000 ceilometermiddleware-3.3.1/ceilometermiddleware.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-02-23 08:58:32.000000 ceilometermiddleware-3.3.1/ceilometermiddleware.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2024-02-23 08:58:32.000000 ceilometermiddleware-3.3.1/ceilometermiddleware.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:32.406164 ceilometermiddleware-3.3.1/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:32.414164 ceilometermiddleware-3.3.1/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2659 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/doc/source/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:32.406164 ceilometermiddleware-3.3.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:32.414164 ceilometermiddleware-3.3.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/notes/background-thread-notifier-21b36a5f5c8dec0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/notes/bug-1679196-ab9d6bb2134120e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/notes/drop-py-2-7-21178ddd27b28806.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/notes/drop-python-3-6-and-3-7-a7bb45e8a4be299a.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:32.418164 ceilometermiddleware-3.3.1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:32.418164 ceilometermiddleware-3.3.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:32.418164 ceilometermiddleware-3.3.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8866 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2024-02-23 08:58:32.418164 ceilometermiddleware-3.3.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2024-02-23 08:58:08.000000 ceilometermiddleware-3.3.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:09.057905 ceilometermiddleware-3.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1750 2024-05-23 08:02:08.000000 ceilometermiddleware-3.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5912 2024-05-23 08:02:08.000000 ceilometermiddleware-3.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2024-05-23 08:02:09.057905 ceilometermiddleware-3.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      671 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:09.053905 ceilometermiddleware-3.4.0/ceilometermiddleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/ceilometermiddleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15637 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/ceilometermiddleware/swift.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:09.053905 ceilometermiddleware-3.4.0/ceilometermiddleware/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/ceilometermiddleware/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/ceilometermiddleware/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:09.053905 ceilometermiddleware-3.4.0/ceilometermiddleware/tests/data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14661 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/ceilometermiddleware/tests/data/list_projects.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22710 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/ceilometermiddleware/tests/test_swift.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:09.053905 ceilometermiddleware-3.4.0/ceilometermiddleware.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2024-05-23 08:02:08.000000 ceilometermiddleware-3.4.0/ceilometermiddleware.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2024-05-23 08:02:09.000000 ceilometermiddleware-3.4.0/ceilometermiddleware.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:02:08.000000 ceilometermiddleware-3.4.0/ceilometermiddleware.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-05-23 08:02:08.000000 ceilometermiddleware-3.4.0/ceilometermiddleware.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:02:08.000000 ceilometermiddleware-3.4.0/ceilometermiddleware.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 08:02:08.000000 ceilometermiddleware-3.4.0/ceilometermiddleware.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-05-23 08:02:08.000000 ceilometermiddleware-3.4.0/ceilometermiddleware.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2024-05-23 08:02:08.000000 ceilometermiddleware-3.4.0/ceilometermiddleware.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:09.053905 ceilometermiddleware-3.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:09.053905 ceilometermiddleware-3.4.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2659 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/doc/source/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:09.049905 ceilometermiddleware-3.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:09.057905 ceilometermiddleware-3.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/notes/background-thread-notifier-21b36a5f5c8dec0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/notes/bug-1673738-ec8f7dd8ac43ad54.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/notes/bug-1679196-ab9d6bb2134120e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/notes/drop-py-2-7-21178ddd27b28806.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/notes/drop-python-3-6-and-3-7-a7bb45e8a4be299a.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:09.057905 ceilometermiddleware-3.4.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:09.057905 ceilometermiddleware-3.4.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:02:09.057905 ceilometermiddleware-3.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8866 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2024-05-23 08:02:09.057905 ceilometermiddleware-3.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2024-05-23 08:01:28.000000 ceilometermiddleware-3.4.0/tox.ini
```

### Comparing `ceilometermiddleware-3.3.1/AUTHORS` & `ceilometermiddleware-3.4.0/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Corey Bryant <corey.bryant@canonical.com>
 Darren Hague <d.hague@sap.com>
 Doug Hellmann <doug@doughellmann.com>
 Erno Kuvaja <jokke@usr.fi>
 Flavio Percoco <flaper87@gmail.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Hanxi Liu <hanxi.liu@easystack.cn>
+Hervé Beraud <hberaud@redhat.com>
 Julien Danjou <julien@danjou.info>
 Le Hou <houl7@chinaunicom.cn>
 Mehdi Abaakouk <sileht@sileht.net>
 Monty Taylor <mordred@inaugust.com>
 Nadya Privalova <nprivalova@mirantis.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Rohit Jaiswal <rohit.jaiswal@hp.com>
```

### Comparing `ceilometermiddleware-3.3.1/CONTRIBUTING.rst` & `ceilometermiddleware-3.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ceilometermiddleware-3.3.1/ChangeLog` & `ceilometermiddleware-3.4.0/ChangeLog`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 CHANGES
 =======
 
+3.4.0
+-----
+
+* Load additional config files for oslo.messaging options
+* reno: Update master for unmaintained/xena
+* reno: Update master for unmaintained/wallaby
+* reno: Update master for unmaintained/victoria
+* Update master for stable/2024.1
+
 3.3.1
 -----
 
 * Fix releasenotes build of yoga moved to unmaintained
 * Bump hacking
+* Add doc/requirements
 
 3.3.0
 -----
 
 * Update python classifier in setup.cfg
 * Remove unused six library
 * Ignore .eggs directory
```

### Comparing `ceilometermiddleware-3.3.1/LICENSE` & `ceilometermiddleware-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ceilometermiddleware-3.3.1/PKG-INFO` & `ceilometermiddleware-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ceilometermiddleware
-Version: 3.3.1
+Version: 3.4.0
 Summary: OpenStack Telemetry middleware for generating metrics
 Home-page: https://docs.openstack.org/ceilometermiddleware/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===============================================
         Middleware for OpenStack Telemetry (Ceilometer)
```

### Comparing `ceilometermiddleware-3.3.1/README.rst` & `ceilometermiddleware-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `ceilometermiddleware-3.3.1/ceilometermiddleware/__init__.py` & `ceilometermiddleware-3.4.0/ceilometermiddleware/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometermiddleware-3.3.1/ceilometermiddleware/swift.py` & `ceilometermiddleware-3.4.0/ceilometermiddleware/swift.py`

 * *Files 8% similar despite different names*

```diff
@@ -156,18 +156,32 @@
     DEFAULT_IGNORE_PROJECT_NAMES = ['service']
 
     def __init__(self, app, conf):
         self._app = app
 
         self.ignore_projects = self._get_ignore_projects(conf)
 
+        extra_config_files = conf.get('extra_config_files')
+        if extra_config_files is not None:
+            extra_config_files = list_from_csv(extra_config_files)
+
+        extra_config_dirs = conf.get('extra_config_dirs')
+        if extra_config_dirs is not None:
+            extra_config_dirs = list_from_csv(extra_config_dirs)
+
+        oslo_conf = cfg.ConfigOpts()
+        oslo_conf([], project='swift',
+                  default_config_files=extra_config_files,
+                  default_config_dirs=extra_config_dirs,
+                  validate_default_values=True)
+
         oslo_messaging.set_transport_defaults(conf.get('control_exchange',
                                                        'swift'))
         self._notifier = oslo_messaging.Notifier(
-            oslo_messaging.get_notification_transport(cfg.CONF,
+            oslo_messaging.get_notification_transport(oslo_conf,
                                                       url=conf.get('url')),
             publisher_id='ceilometermiddleware',
             driver=conf.get('driver', 'messagingv2'),
             topics=[conf.get('topic', 'notifications')])
 
         self.metadata_headers = [h.strip().replace('-', '_').lower()
                                  for h in conf.get(
```

### Comparing `ceilometermiddleware-3.3.1/ceilometermiddleware/tests/base.py` & `ceilometermiddleware-3.4.0/ceilometermiddleware/tests/base.py`

 * *Files identical despite different names*

### Comparing `ceilometermiddleware-3.3.1/ceilometermiddleware/tests/data/list_projects.yaml` & `ceilometermiddleware-3.4.0/ceilometermiddleware/tests/data/list_projects.yaml`

 * *Files identical despite different names*

### Comparing `ceilometermiddleware-3.3.1/ceilometermiddleware/tests/test_swift.py` & `ceilometermiddleware-3.4.0/ceilometermiddleware/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `ceilometermiddleware-3.3.1/ceilometermiddleware.egg-info/PKG-INFO` & `ceilometermiddleware-3.4.0/ceilometermiddleware.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ceilometermiddleware
-Version: 3.3.1
+Version: 3.4.0
 Summary: OpenStack Telemetry middleware for generating metrics
 Home-page: https://docs.openstack.org/ceilometermiddleware/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===============================================
         Middleware for OpenStack Telemetry (Ceilometer)
```

### Comparing `ceilometermiddleware-3.3.1/ceilometermiddleware.egg-info/SOURCES.txt` & `ceilometermiddleware-3.4.0/ceilometermiddleware.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,30 @@
 ceilometermiddleware.egg-info/pbr.json
 ceilometermiddleware.egg-info/requires.txt
 ceilometermiddleware.egg-info/top_level.txt
 ceilometermiddleware/tests/__init__.py
 ceilometermiddleware/tests/base.py
 ceilometermiddleware/tests/test_swift.py
 ceilometermiddleware/tests/data/list_projects.yaml
+doc/requirements.txt
 doc/source/conf.py
 doc/source/contributing.rst
 doc/source/index.rst
 doc/source/installation.rst
 doc/source/readme.rst
 doc/source/usage.rst
 releasenotes/notes/.placeholder
 releasenotes/notes/background-thread-notifier-21b36a5f5c8dec0e.yaml
+releasenotes/notes/bug-1673738-ec8f7dd8ac43ad54.yaml
 releasenotes/notes/bug-1679196-ab9d6bb2134120e0.yaml
 releasenotes/notes/drop-py-2-7-21178ddd27b28806.yaml
 releasenotes/notes/drop-python-3-6-and-3-7-a7bb45e8a4be299a.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
```

### Comparing `ceilometermiddleware-3.3.1/doc/source/conf.py` & `ceilometermiddleware-3.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ceilometermiddleware-3.3.1/releasenotes/notes/background-thread-notifier-21b36a5f5c8dec0e.yaml` & `ceilometermiddleware-3.4.0/releasenotes/notes/background-thread-notifier-21b36a5f5c8dec0e.yaml`

 * *Files identical despite different names*

### Comparing `ceilometermiddleware-3.3.1/releasenotes/source/conf.py` & `ceilometermiddleware-3.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ceilometermiddleware-3.3.1/setup.cfg` & `ceilometermiddleware-3.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ceilometermiddleware-3.3.1/setup.py` & `ceilometermiddleware-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `ceilometermiddleware-3.3.1/tox.ini` & `ceilometermiddleware-3.4.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -28,20 +28,23 @@
 commands =
     stestr run '{posargs}'
     coverage combine
     coverage html -d cover
     coverage xml -o cover/coverage.xml
 
 [testenv:docs]
+deps = -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+       -r{toxinidir}/doc/requirements.txt
 commands = sphinx-build -W -b html -d doc/build/doctrees doc/source doc/build/html
 
 [testenv:debug]
 commands = oslo_debug_helper {posargs}
 
 [testenv:releasenotes]
+deps = {[testenv:docs]deps}
 commands = sphinx-build -a -E -d releasenotes/build/doctrees -b html releasenotes/source releasenotes/build/html
 
 [flake8]
 show-source = True
 # W503 line break before binary operator
 ignore = W503
 exclude=.venv,.git,.tox,dist,doc,*lib/python*,*egg,build
```

