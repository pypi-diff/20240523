# Comparing `tmp/oslo.versionedobjects-3.3.0.tar.gz` & `tmp/oslo.versionedobjects-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslo.versionedobjects-3.3.0.tar", last modified: Thu Feb 22 15:10:16 2024, max compression
+gzip compressed data, was "oslo.versionedobjects-3.4.0.tar", last modified: Thu May 23 08:26:38 2024, max compression
```

## Comparing `oslo.versionedobjects-3.3.0.tar` & `oslo.versionedobjects-3.4.0.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.318356 oslo.versionedobjects-3.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16279 2024-02-22 15:10:16.000000 oslo.versionedobjects-3.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      738 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   187397 2024-02-22 15:10:15.000000 oslo.versionedobjects-3.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2554 2024-02-22 15:10:16.318356 oslo.versionedobjects-3.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.298356 oslo.versionedobjects-3.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.302356 oslo.versionedobjects-3.3.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2805 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.302356 oslo.versionedobjects-3.3.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.302356 oslo.versionedobjects-3.3.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.302356 oslo.versionedobjects-3.3.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.302356 oslo.versionedobjects-3.3.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/reference/base.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/reference/exception.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/reference/fields.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/reference/fixture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.302356 oslo.versionedobjects-3.3.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      977 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/user/examples.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4638 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/doc/source/user/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.306356 oslo.versionedobjects-3.3.0/oslo.versionedobjects.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2554 2024-02-22 15:10:16.000000 oslo.versionedobjects-3.3.0/oslo.versionedobjects.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2542 2024-02-22 15:10:16.000000 oslo.versionedobjects-3.3.0/oslo.versionedobjects.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:10:16.000000 oslo.versionedobjects-3.3.0/oslo.versionedobjects.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-02-22 15:10:16.000000 oslo.versionedobjects-3.3.0/oslo.versionedobjects.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:10:16.000000 oslo.versionedobjects-3.3.0/oslo.versionedobjects.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-22 15:10:16.000000 oslo.versionedobjects-3.3.0/oslo.versionedobjects.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-02-22 15:10:16.000000 oslo.versionedobjects-3.3.0/oslo.versionedobjects.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       22 2024-02-22 15:10:16.000000 oslo.versionedobjects-3.3.0/oslo.versionedobjects.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.306356 oslo.versionedobjects-3.3.0/oslo_versionedobjects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/_options.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1193 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51253 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.306356 oslo.versionedobjects-3.3.0/oslo_versionedobjects/examples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/examples/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/examples/iot_bulb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6528 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44489 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20417 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/fixture.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.294356 oslo.versionedobjects-3.3.0/oslo_versionedobjects/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.294356 oslo.versionedobjects-3.3.0/oslo_versionedobjects/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.310356 oslo.versionedobjects-3.3.0/oslo_versionedobjects/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5726 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/locale/en_GB/LC_MESSAGES/oslo_versionedobjects.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7372 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/test.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.310356 oslo.versionedobjects-3.3.0/oslo_versionedobjects/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6473 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/tests/obj_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2822 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/tests/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50079 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/tests/test_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33118 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/tests/test_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   101210 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/oslo_versionedobjects/tests/test_objects.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.294356 oslo.versionedobjects-3.3.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.310356 oslo.versionedobjects-3.3.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/notes/drop-python27-support-b3e377b0dcfa4f5c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/notes/update_md5_for_fips-e5a8f8f438ac81fb.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.314356 oslo.versionedobjects-3.3.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.314356 oslo.versionedobjects-3.3.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.318356 oslo.versionedobjects-3.3.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9062 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.294356 oslo.versionedobjects-3.3.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.294356 oslo.versionedobjects-3.3.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:10:16.318356 oslo.versionedobjects-3.3.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2024-02-22 15:10:16.318356 oslo.versionedobjects-3.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2024-02-22 15:09:48.000000 oslo.versionedobjects-3.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.866407 oslo.versionedobjects-3.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16279 2024-05-23 08:26:38.000000 oslo.versionedobjects-3.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      738 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   187673 2024-05-23 08:26:38.000000 oslo.versionedobjects-3.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2554 2024-05-23 08:26:38.866407 oslo.versionedobjects-3.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.854406 oslo.versionedobjects-3.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.854406 oslo.versionedobjects-3.4.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2805 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.854406 oslo.versionedobjects-3.4.0/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.854406 oslo.versionedobjects-3.4.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.854406 oslo.versionedobjects-3.4.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.858407 oslo.versionedobjects-3.4.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/reference/base.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/reference/exception.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/reference/fields.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/reference/fixture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.858407 oslo.versionedobjects-3.4.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      977 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/user/examples.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4638 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.858407 oslo.versionedobjects-3.4.0/oslo.versionedobjects.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2554 2024-05-23 08:26:38.000000 oslo.versionedobjects-3.4.0/oslo.versionedobjects.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2573 2024-05-23 08:26:38.000000 oslo.versionedobjects-3.4.0/oslo.versionedobjects.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:26:38.000000 oslo.versionedobjects-3.4.0/oslo.versionedobjects.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-05-23 08:26:38.000000 oslo.versionedobjects-3.4.0/oslo.versionedobjects.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:26:38.000000 oslo.versionedobjects-3.4.0/oslo.versionedobjects.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 08:26:38.000000 oslo.versionedobjects-3.4.0/oslo.versionedobjects.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2024-05-23 08:26:38.000000 oslo.versionedobjects-3.4.0/oslo.versionedobjects.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       22 2024-05-23 08:26:38.000000 oslo.versionedobjects-3.4.0/oslo.versionedobjects.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.858407 oslo.versionedobjects-3.4.0/oslo_versionedobjects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1193 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51253 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.862407 oslo.versionedobjects-3.4.0/oslo_versionedobjects/examples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/examples/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/examples/iot_bulb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6528 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44489 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20417 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/fixture.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.846407 oslo.versionedobjects-3.4.0/oslo_versionedobjects/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.846407 oslo.versionedobjects-3.4.0/oslo_versionedobjects/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.862407 oslo.versionedobjects-3.4.0/oslo_versionedobjects/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5726 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/locale/en_GB/LC_MESSAGES/oslo_versionedobjects.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7372 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/test.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.862407 oslo.versionedobjects-3.4.0/oslo_versionedobjects/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6473 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/tests/obj_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2822 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/tests/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50079 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/tests/test_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33118 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/tests/test_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   101211 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/oslo_versionedobjects/tests/test_objects.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.850407 oslo.versionedobjects-3.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.862407 oslo.versionedobjects-3.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/notes/drop-python27-support-b3e377b0dcfa4f5c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/notes/update_md5_for_fips-e5a8f8f438ac81fb.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.866407 oslo.versionedobjects-3.4.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.866407 oslo.versionedobjects-3.4.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.866407 oslo.versionedobjects-3.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9062 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.850407 oslo.versionedobjects-3.4.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.850407 oslo.versionedobjects-3.4.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:26:38.866407 oslo.versionedobjects-3.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2024-05-23 08:26:38.866407 oslo.versionedobjects-3.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2024-05-23 08:25:52.000000 oslo.versionedobjects-3.4.0/tox.ini
```

### Comparing `oslo.versionedobjects-3.3.0/.pre-commit-config.yaml` & `oslo.versionedobjects-3.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/.zuul.yaml` & `oslo.versionedobjects-3.4.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/AUTHORS` & `oslo.versionedobjects-3.4.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/CONTRIBUTING.rst` & `oslo.versionedobjects-3.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/ChangeLog` & `oslo.versionedobjects-3.4.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGES
 =======
 
+3.4.0
+-----
+
+* reno: Update master for unmaintained/zed
+* Remove old excludes
+* Replace usage of pytz
+* Update master for stable/2024.1
+* reno: Update master for unmaintained/xena
+* reno: Update master for unmaintained/wallaby
+* reno: Update master for unmaintained/victoria
+
 3.3.0
 -----
 
 * reno: Update master for unmaintained/yoga
 * Bump hacking
 * Update python classifier in setup.cfg
 * coveragerc: Remove non-existent path
```

### Comparing `oslo.versionedobjects-3.3.0/LICENSE` & `oslo.versionedobjects-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/PKG-INFO` & `oslo.versionedobjects-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: oslo.versionedobjects
-Version: 3.3.0
+Version: 3.4.0
 Summary: Oslo Versioned Objects library
 Home-page: https://docs.openstack.org/oslo.versionedobjects/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `oslo.versionedobjects-3.3.0/README.rst` & `oslo.versionedobjects-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/doc/source/conf.py` & `oslo.versionedobjects-3.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/doc/source/index.rst` & `oslo.versionedobjects-3.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/doc/source/reference/fixture.rst` & `oslo.versionedobjects-3.4.0/doc/source/reference/fixture.rst`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/doc/source/user/examples.rst` & `oslo.versionedobjects-3.4.0/doc/source/user/examples.rst`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/doc/source/user/usage.rst` & `oslo.versionedobjects-3.4.0/doc/source/user/usage.rst`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo.versionedobjects.egg-info/PKG-INFO` & `oslo.versionedobjects-3.4.0/oslo.versionedobjects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: oslo.versionedobjects
-Version: 3.3.0
+Version: 3.4.0
 Summary: Oslo Versioned Objects library
 Home-page: https://docs.openstack.org/oslo.versionedobjects/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `oslo.versionedobjects-3.3.0/oslo.versionedobjects.egg-info/SOURCES.txt` & `oslo.versionedobjects-3.4.0/oslo.versionedobjects.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 oslo_versionedobjects/tests/test_fixture.py
 oslo_versionedobjects/tests/test_objects.py
 releasenotes/notes/add-reno-996dd44974d53238.yaml
 releasenotes/notes/drop-python27-support-b3e377b0dcfa4f5c.yaml
 releasenotes/notes/update_md5_for_fips-e5a8f8f438ac81fb.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
```

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/_i18n.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/_i18n.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/_options.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/_options.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/_utils.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/_utils.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/base.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/base.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/examples/iot_bulb.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/examples/iot_bulb.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/exception.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/exception.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/fields.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/fields.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/fixture.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/locale/en_GB/LC_MESSAGES/oslo_versionedobjects.po` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/locale/en_GB/LC_MESSAGES/oslo_versionedobjects.po`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/test.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/test.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/tests/obj_fixtures.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/tests/obj_fixtures.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/tests/test_exception.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/tests/test_fields.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/tests/test_fixture.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/oslo_versionedobjects/tests/test_objects.py` & `oslo.versionedobjects-3.4.0/oslo_versionedobjects/tests/test_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import copy
 import datetime
 import jsonschema
 import logging
-import pytz
 from unittest import mock
 
 from oslo_context import context
 from oslo_serialization import jsonutils
 from oslo_utils import timeutils
 import testtools
 from testtools import matchers
@@ -1093,15 +1092,15 @@
         obj.foo = 123
         self.assertEqual({'foo': 123}, obj.obj_get_changes())
         obj.bar = 'test'
         self.assertEqual({'foo': 123, 'bar': 'test'}, obj.obj_get_changes())
         obj.obj_reset_changes()
         self.assertEqual({}, obj.obj_get_changes())
 
-        timestamp = datetime.datetime(2001, 1, 1, tzinfo=pytz.utc)
+        timestamp = datetime.datetime(2001, 1, 1, tzinfo=datetime.timezone.utc)
         with mock.patch.object(timeutils, 'utcnow') as mock_utcnow:
             mock_utcnow.return_value = timestamp
             obj.timestamp = timeutils.utcnow()
             self.assertEqual({'timestamp': timestamp}, obj.obj_get_changes())
 
         obj.obj_reset_changes()
         self.assertEqual({}, obj.obj_get_changes())
```

### Comparing `oslo.versionedobjects-3.3.0/releasenotes/source/conf.py` & `oslo.versionedobjects-3.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `oslo.versionedobjects-3.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/setup.cfg` & `oslo.versionedobjects-3.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/setup.py` & `oslo.versionedobjects-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `oslo.versionedobjects-3.3.0/tox.ini` & `oslo.versionedobjects-3.4.0/tox.ini`

 * *Files identical despite different names*

