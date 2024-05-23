# Comparing `tmp/zope_interface-6.4.tar.gz` & `tmp/zope.interface-6.4.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope_interface-6.4.tar", last modified: Wed May 15 20:23:10 2024, max compression
+gzip compressed data, was "zope.interface-6.4.post0.tar", last modified: Wed May 22 06:43:23 2024, max compression
```

## Comparing `zope_interface-6.4.tar` & `zope.interface-6.4.post0.tar`

### file list

```diff
@@ -1,133 +1,109 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.738219 zope_interface-6.4/
--rw-r--r--   0 jens       (501) staff       (20)      588 2024-05-13 12:30:38.000000 zope_interface-6.4/.coveragerc
--rwxr-xr-x   0 jens       (501) staff       (20)     2259 2024-05-13 12:30:38.000000 zope_interface-6.4/.manylinux-install.sh
--rwxr-xr-x   0 jens       (501) staff       (20)      509 2024-05-13 12:30:38.000000 zope_interface-6.4/.manylinux.sh
--rw-r--r--   0 jens       (501) staff       (20)      664 2024-05-13 12:30:38.000000 zope_interface-6.4/.readthedocs.yaml
--rw-r--r--   0 jens       (501) staff       (20)    39159 2024-05-15 20:12:06.000000 zope_interface-6.4/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      799 2024-05-13 12:30:38.000000 zope_interface-6.4/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       32 2023-01-03 12:44:50.000000 zope_interface-6.4/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2023-01-03 12:44:50.000000 zope_interface-6.4/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      558 2024-05-13 12:30:38.000000 zope_interface-6.4/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)    42209 2024-05-15 20:23:10.738130 zope_interface-6.4/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     1353 2023-01-03 12:44:50.000000 zope_interface-6.4/README.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.713046 zope_interface-6.4/benchmarks/
--rw-r--r--   0 jens       (501) staff       (20)     8497 2023-01-03 12:44:50.000000 zope_interface-6.4/benchmarks/micro.py
--rw-r--r--   0 jens       (501) staff       (20)      838 2023-01-03 12:44:50.000000 zope_interface-6.4/build.cmd
--rw-r--r--   0 jens       (501) staff       (20)      215 2023-01-03 12:44:50.000000 zope_interface-6.4/buildout.cfg
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.717054 zope_interface-6.4/docs/
--rw-r--r--   0 jens       (501) staff       (20)     5592 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/Makefile
--rw-r--r--   0 jens       (501) staff       (20)    41051 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/README.rst
--rw-r--r--   0 jens       (501) staff       (20)    33998 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/README.ru.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.707262 zope_interface-6.4/docs/_build/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.717330 zope_interface-6.4/docs/_build/doctest/
--rw-r--r--   0 jens       (501) staff       (20)     1292 2024-05-14 09:54:19.000000 zope_interface-6.4/docs/_build/doctest/output.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.707308 zope_interface-6.4/docs/_build/html/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.721435 zope_interface-6.4/docs/_build/html/_sources/
--rw-r--r--   0 jens       (501) staff       (20)    41051 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/README.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    33998 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/README.ru.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    18817 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/adapter.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    21169 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/adapter.ru.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.722457 zope_interface-6.4/docs/_build/html/_sources/api/
--rw-r--r--   0 jens       (501) staff       (20)      691 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/adapters.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     1283 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/common.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     2465 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/components.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    21746 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/declarations.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      165 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      687 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/ro.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     9948 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/specifications.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       28 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/changes.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     1742 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/foodforthought.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     9509 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/hacking.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     6537 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/human.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    10681 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/human.ru.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      639 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    10222 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/verify.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    18817 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/adapter.rst
--rw-r--r--   0 jens       (501) staff       (20)    21169 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/adapter.ru.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.723830 zope_interface-6.4/docs/api/
--rw-r--r--   0 jens       (501) staff       (20)      691 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/adapters.rst
--rw-r--r--   0 jens       (501) staff       (20)     1283 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/common.rst
--rw-r--r--   0 jens       (501) staff       (20)     2465 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/components.rst
--rw-r--r--   0 jens       (501) staff       (20)    21746 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/declarations.rst
--rw-r--r--   0 jens       (501) staff       (20)      165 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/index.rst
--rw-r--r--   0 jens       (501) staff       (20)      687 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/ro.rst
--rw-r--r--   0 jens       (501) staff       (20)     9948 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/specifications.rst
--rw-r--r--   0 jens       (501) staff       (20)       28 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/changes.rst
--rw-r--r--   0 jens       (501) staff       (20)     9130 2024-04-12 14:41:20.000000 zope_interface-6.4/docs/conf.py
--rw-r--r--   0 jens       (501) staff       (20)     1742 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/foodforthought.rst
--rw-r--r--   0 jens       (501) staff       (20)     9509 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/hacking.rst
--rw-r--r--   0 jens       (501) staff       (20)     6537 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/human.rst
--rw-r--r--   0 jens       (501) staff       (20)    10681 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/human.ru.rst
--rw-r--r--   0 jens       (501) staff       (20)      639 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     5110 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/make.bat
--rw-r--r--   0 jens       (501) staff       (20)       68 2023-10-05 10:12:16.000000 zope_interface-6.4/docs/requirements.txt
--rw-r--r--   0 jens       (501) staff       (20)    10222 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/verify.rst
--rw-r--r--   0 jens       (501) staff       (20)      570 2024-05-15 20:23:10.738424 zope_interface-6.4/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     5014 2024-05-15 20:12:24.000000 zope_interface-6.4/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.707549 zope_interface-6.4/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.723986 zope_interface-6.4/src/zope/
--rw-r--r--   0 jens       (501) staff       (20)       56 2023-01-03 12:44:50.000000 zope_interface-6.4/src/zope/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.728593 zope_interface-6.4/src/zope/interface/
--rw-r--r--   0 jens       (501) staff       (20)     3460 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     4369 2024-05-15 13:08:06.000000 zope_interface-6.4/src/zope/interface/_compat.py
--rw-r--r--   0 jens       (501) staff       (20)     1057 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/_flatten.py
--rw-r--r--   0 jens       (501) staff       (20)    57205 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/_zope_interface_coptimizations.c
--rw-r--r--   0 jens       (501) staff       (20)    36218 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/adapter.py
--rw-r--r--   0 jens       (501) staff       (20)     3892 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/advice.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.730860 zope_interface-6.4/src/zope/interface/common/
--rw-r--r--   0 jens       (501) staff       (20)    10462 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     3027 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/builtins.py
--rw-r--r--   0 jens       (501) staff       (20)     6792 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/collections.py
--rw-r--r--   0 jens       (501) staff       (20)    20964 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/idatetime.py
--rw-r--r--   0 jens       (501) staff       (20)     5368 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)     1242 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/io.py
--rw-r--r--   0 jens       (501) staff       (20)     4678 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/mapping.py
--rw-r--r--   0 jens       (501) staff       (20)     1682 2023-01-03 12:44:50.000000 zope_interface-6.4/src/zope/interface/common/numbers.py
--rw-r--r--   0 jens       (501) staff       (20)     5526 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/sequence.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.732600 zope_interface-6.4/src/zope/interface/common/tests/
--rw-r--r--   0 jens       (501) staff       (20)     5476 2024-05-13 12:27:59.000000 zope_interface-6.4/src/zope/interface/common/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     3907 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/tests/basemapping.py
--rw-r--r--   0 jens       (501) staff       (20)     1345 2023-01-03 12:44:50.000000 zope_interface-6.4/src/zope/interface/common/tests/test_builtins.py
--rw-r--r--   0 jens       (501) staff       (20)     5718 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/tests/test_collections.py
--rw-r--r--   0 jens       (501) staff       (20)     1923 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/tests/test_idatetime.py
--rw-r--r--   0 jens       (501) staff       (20)      813 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/tests/test_import_interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)     1663 2024-05-13 12:27:59.000000 zope_interface-6.4/src/zope/interface/common/tests/test_io.py
--rw-r--r--   0 jens       (501) staff       (20)     1394 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/tests/test_numbers.py
--rw-r--r--   0 jens       (501) staff       (20)    43007 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/declarations.py
--rw-r--r--   0 jens       (501) staff       (20)     4068 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/document.py
--rw-r--r--   0 jens       (501) staff       (20)     8636 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/exceptions.py
--rw-r--r--   0 jens       (501) staff       (20)    39409 2024-05-15 20:11:48.000000 zope_interface-6.4/src/zope/interface/interface.py
--rw-r--r--   0 jens       (501) staff       (20)    50126 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)    25829 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/registry.py
--rw-r--r--   0 jens       (501) staff       (20)    24157 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/ro.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.737229 zope_interface-6.4/src/zope/interface/tests/
--rw-r--r--   0 jens       (501) staff       (20)     3961 2023-01-03 12:44:50.000000 zope_interface-6.4/src/zope/interface/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)      898 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/advisory_testing.py
--rw-r--r--   0 jens       (501) staff       (20)      912 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/dummy.py
--rw-r--r--   0 jens       (501) staff       (20)      890 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/idummy.py
--rw-r--r--   0 jens       (501) staff       (20)      839 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/m1.py
--rw-r--r--   0 jens       (501) staff       (20)     3015 2023-01-03 12:44:50.000000 zope_interface-6.4/src/zope/interface/tests/odd.py
--rw-r--r--   0 jens       (501) staff       (20)    79479 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_adapter.py
--rw-r--r--   0 jens       (501) staff       (20)     6040 2024-05-15 20:11:48.000000 zope_interface-6.4/src/zope/interface/tests/test_advice.py
--rw-r--r--   0 jens       (501) staff       (20)     1290 2023-01-03 12:44:50.000000 zope_interface-6.4/src/zope/interface/tests/test_compile_flags.py
--rw-r--r--   0 jens       (501) staff       (20)    82140 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_declarations.py
--rw-r--r--   0 jens       (501) staff       (20)    17164 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_document.py
--rw-r--r--   0 jens       (501) staff       (20)     1120 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_element.py
--rw-r--r--   0 jens       (501) staff       (20)     6412 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_exceptions.py
--rw-r--r--   0 jens       (501) staff       (20)    92312 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_interface.py
--rw-r--r--   0 jens       (501) staff       (20)     4377 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)     7566 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_odd_declarations.py
--rw-r--r--   0 jens       (501) staff       (20)   112910 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_registry.py
--rw-r--r--   0 jens       (501) staff       (20)    14124 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_ro.py
--rw-r--r--   0 jens       (501) staff       (20)     1934 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_sorting.py
--rw-r--r--   0 jens       (501) staff       (20)    19191 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_verify.py
--rw-r--r--   0 jens       (501) staff       (20)     7226 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/verify.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.737610 zope_interface-6.4/src/zope.interface.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)    42209 2024-05-15 20:23:10.000000 zope_interface-6.4/src/zope.interface.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     3770 2024-05-15 20:23:10.000000 zope_interface-6.4/src/zope.interface.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-15 20:23:10.000000 zope_interface-6.4/src/zope.interface.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)        5 2024-05-15 20:23:10.000000 zope_interface-6.4/src/zope.interface.egg-info/namespace_packages.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-01-03 13:57:16.000000 zope_interface-6.4/src/zope.interface.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)      170 2024-05-15 20:23:10.000000 zope_interface-6.4/src/zope.interface.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)        5 2024-05-15 20:23:10.000000 zope_interface-6.4/src/zope.interface.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     2132 2024-05-13 12:30:38.000000 zope_interface-6.4/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.410102 zope.interface-6.4.post0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      588 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/.coveragerc
+-rwxr-xr-x   0 m.howitz   (502) staff       (20)     2259 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/.manylinux-install.sh
+-rwxr-xr-x   0 m.howitz   (502) staff       (20)      509 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/.manylinux.sh
+-rw-r--r--   0 m.howitz   (502) staff       (20)      664 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/.readthedocs.yaml
+-rw-r--r--   0 m.howitz   (502) staff       (20)    39533 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      799 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      558 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    42589 2024-05-22 06:43:23.409971 zope.interface-6.4.post0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1353 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/README.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.394587 zope.interface-6.4.post0/benchmarks/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8497 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/benchmarks/micro.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      838 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/build.cmd
+-rw-r--r--   0 m.howitz   (502) staff       (20)      215 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.397470 zope.interface-6.4.post0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5592 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)    41051 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    33998 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/README.ru.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    18817 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/adapter.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21169 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/adapter.ru.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.398522 zope.interface-6.4.post0/docs/api/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      691 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/adapters.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1283 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/common.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2465 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/components.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21746 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/declarations.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      165 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      687 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/ro.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9948 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/api/specifications.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/changes.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9130 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1742 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/foodforthought.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9509 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/hacking.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6537 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/human.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10681 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/human.ru.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      639 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5110 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/make.bat
+-rw-r--r--   0 m.howitz   (502) staff       (20)       68 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/requirements.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10222 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/docs/verify.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      570 2024-05-22 06:43:23.410475 zope.interface-6.4.post0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5020 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.391102 zope.interface-6.4.post0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.398692 zope.interface-6.4.post0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.402369 zope.interface-6.4.post0/src/zope/interface/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3460 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4369 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/_compat.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1057 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/_flatten.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    57205 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/_zope_interface_coptimizations.c
+-rw-r--r--   0 m.howitz   (502) staff       (20)    36218 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/adapter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3892 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/advice.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.404089 zope.interface-6.4.post0/src/zope/interface/common/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10462 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3027 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/builtins.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6792 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/collections.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    20964 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/idatetime.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5368 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1242 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/io.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4678 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/mapping.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1682 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/numbers.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5526 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/sequence.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.405487 zope.interface-6.4.post0/src/zope/interface/common/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5476 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3907 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/basemapping.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1345 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/test_builtins.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5718 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/test_collections.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1923 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/test_idatetime.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      813 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/test_import_interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1663 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/test_io.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1394 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/common/tests/test_numbers.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    43007 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/declarations.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4068 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/document.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8636 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/exceptions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    39409 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/interface.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    50126 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    25829 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/registry.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    24157 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/ro.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.409061 zope.interface-6.4.post0/src/zope/interface/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3961 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      898 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/advisory_testing.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      912 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/dummy.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      890 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/idummy.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      839 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/m1.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3015 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/odd.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    79479 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_adapter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6040 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_advice.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1290 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_compile_flags.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    82140 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_declarations.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17164 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_document.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1120 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_element.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6412 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_exceptions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    92312 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_interface.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4377 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7566 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_odd_declarations.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)   112910 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_registry.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    14124 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_ro.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1934 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_sorting.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    19191 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/tests/test_verify.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7226 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/src/zope/interface/verify.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 06:43:23.409299 zope.interface-6.4.post0/src/zope.interface.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    42589 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2940 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      170 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2024-05-22 06:43:23.000000 zope.interface-6.4.post0/src/zope.interface.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2132 2024-05-22 06:43:22.000000 zope.interface-6.4.post0/tox.ini
```

### Comparing `zope_interface-6.4/.coveragerc` & `zope.interface-6.4.post0/.coveragerc`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/.manylinux-install.sh` & `zope.interface-6.4.post0/.manylinux-install.sh`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/.readthedocs.yaml` & `zope.interface-6.4.post0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/CHANGES.rst` & `zope.interface-6.4.post0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
  Changes
 =========
 
+6.4.post0 (2024-05-22)
+======================
+
+- The sdist of version 6.4 was uploaded to PyPI as
+  ``zope_interface-6.4.tar.gz`` instead of ``zope.interface-6.4-py2.tar.gz``
+  which cannot be installed by ``zc.buildout``.  This release is a re-release
+  of version 6.4 with the correct sdist name.
+  (`#298 <https://github.com/zopefoundation/zope.interface/issues/298>`)
+
+
 6.4 (2024-05-15)
 ================
 
 - Adjust for incompatible changes in Python 3.13b1.
   (`#292 <https://github.com/zopefoundation/zope.interface/issues/292>`)
 
 - Build windows wheels on GHA.
```

### Comparing `zope_interface-6.4/CONTRIBUTING.md` & `zope.interface-6.4.post0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/LICENSE.txt` & `zope.interface-6.4.post0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/MANIFEST.in` & `zope.interface-6.4.post0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/PKG-INFO` & `zope.interface-6.4.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.interface
-Version: 6.4
+Version: 6.4.post0
 Summary: Interfaces for Python
 Home-page: https://github.com/zopefoundation/zope.interface
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: interface,components,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,14 +71,24 @@
 
 For detailed documentation, please see https://zopeinterface.readthedocs.io/en/latest/
 
 =========
  Changes
 =========
 
+6.4.post0 (2024-05-22)
+======================
+
+- The sdist of version 6.4 was uploaded to PyPI as
+  ``zope_interface-6.4.tar.gz`` instead of ``zope.interface-6.4-py2.tar.gz``
+  which cannot be installed by ``zc.buildout``.  This release is a re-release
+  of version 6.4 with the correct sdist name.
+  (`#298 <https://github.com/zopefoundation/zope.interface/issues/298>`)
+
+
 6.4 (2024-05-15)
 ================
 
 - Adjust for incompatible changes in Python 3.13b1.
   (`#292 <https://github.com/zopefoundation/zope.interface/issues/292>`)
 
 - Build windows wheels on GHA.
```

### Comparing `zope_interface-6.4/README.rst` & `zope.interface-6.4.post0/README.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/benchmarks/micro.py` & `zope.interface-6.4.post0/benchmarks/micro.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/build.cmd` & `zope.interface-6.4.post0/build.cmd`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/Makefile` & `zope.interface-6.4.post0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/README.rst` & `zope.interface-6.4.post0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/README.ru.rst` & `zope.interface-6.4.post0/docs/README.ru.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/README.rst.txt` & `zope.interface-6.4.post0/src/zope/interface/declarations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1357 +1,1189 @@
-============
- Interfaces
-============
+##############################################################################
+# Copyright (c) 2003 Zope Foundation and Contributors.
+# All Rights Reserved.
+#
+# This software is subject to the provisions of the Zope Public License,
+# Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
+# THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
+# WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+# WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
+# FOR A PARTICULAR PURPOSE.
+##############################################################################
+"""Implementation of interface declarations
+
+There are three flavors of declarations:
+
+  - Declarations are used to simply name declared interfaces.
+
+  - ImplementsDeclarations are used to express the interfaces that a
+    class implements (that instances of the class provides).
+
+    Implements specifications support inheriting interfaces.
+
+  - ProvidesDeclarations are used to express interfaces directly
+    provided by objects.
+
+"""
+__docformat__ = 'restructuredtext'
+
+import sys
+import weakref
+from types import FunctionType
+from types import MethodType
+from types import ModuleType
+
+from zope.interface._compat import _use_c_impl
+from zope.interface.interface import Interface
+from zope.interface.interface import InterfaceClass
+from zope.interface.interface import NameAndModuleComparisonMixin
+from zope.interface.interface import Specification
+from zope.interface.interface import SpecificationBase
+
+
+__all__ = [
+    # None. The public APIs of this module are
+    # re-exported from zope.interface directly.
+]
+
+# pylint:disable=too-many-lines
+
+# Registry of class-implementation specifications
+BuiltinImplementationSpecifications = {}
+
+
+def _next_super_class(ob):
+    # When ``ob`` is an instance of ``super``, return
+    # the next class in the MRO that we should actually be
+    # looking at. Watch out for diamond inheritance!
+    self_class = ob.__self_class__
+    class_that_invoked_super = ob.__thisclass__
+    complete_mro = self_class.__mro__
+    next_class = complete_mro[complete_mro.index(class_that_invoked_super) + 1]
+    return next_class
+
+class named:
+
+    def __init__(self, name):
+        self.name = name
+
+    def __call__(self, ob):
+        ob.__component_name__ = self.name
+        return ob
+
+
+class Declaration(Specification):
+    """Interface declarations"""
+
+    __slots__ = ()
+
+    def __init__(self, *bases):
+        Specification.__init__(self, _normalizeargs(bases))
+
+    def __contains__(self, interface):
+        """Test whether an interface is in the specification
+        """
+
+        return self.extends(interface) and interface in self.interfaces()
+
+    def __iter__(self):
+        """Return an iterator for the interfaces in the specification
+        """
+        return self.interfaces()
+
+    def flattened(self):
+        """Return an iterator of all included and extended interfaces
+        """
+        return iter(self.__iro__)
+
+    def __sub__(self, other):
+        """Remove interfaces from a specification
+        """
+        return Declaration(*[
+            i for i in self.interfaces()
+            if not [
+                j
+                for j in other.interfaces()
+                if i.extends(j, 0) # non-strict extends
+            ]
+        ])
+
+    def __add__(self, other):
+        """
+        Add two specifications or a specification and an interface
+        and produce a new declaration.
+
+        .. versionchanged:: 5.4.0
+           Now tries to preserve a consistent resolution order. Interfaces
+           being added to this object are added to the front of the resulting resolution
+           order if they already extend an interface in this object. Previously,
+           they were always added to the end of the order, which easily resulted in
+           invalid orders.
+        """
+        before = []
+        result = list(self.interfaces())
+        seen = set(result)
+        for i in other.interfaces():
+            if i in seen:
+                continue
+            seen.add(i)
+            if any(i.extends(x) for x in result):
+                # It already extends us, e.g., is a subclass,
+                # so it needs to go at the front of the RO.
+                before.append(i)
+            else:
+                result.append(i)
+        return Declaration(*(before + result))
+
+    # XXX: Is __radd__ needed? No tests break if it's removed.
+    # If it is needed, does it need to handle the C3 ordering differently?
+    # I (JAM) don't *think* it does.
+    __radd__ = __add__
+
+    @staticmethod
+    def _add_interfaces_to_cls(interfaces, cls):
+        # Strip redundant interfaces already provided
+        # by the cls so we don't produce invalid
+        # resolution orders.
+        implemented_by_cls = implementedBy(cls)
+        interfaces = tuple([
+            iface
+            for iface in interfaces
+            if not implemented_by_cls.isOrExtends(iface)
+        ])
+        return interfaces + (implemented_by_cls,)
+
+    @staticmethod
+    def _argument_names_for_repr(interfaces):
+        # These don't actually have to be interfaces, they could be other
+        # Specification objects like Implements. Also, the first
+        # one is typically/nominally the cls.
+        ordered_names = []
+        names = set()
+        for iface in interfaces:
+            duplicate_transform = repr
+            if isinstance(iface, InterfaceClass):
+                # Special case to get 'foo.bar.IFace'
+                # instead of '<InterfaceClass foo.bar.IFace>'
+                this_name = iface.__name__
+                duplicate_transform = str
+            elif isinstance(iface, type):
+                # Likewise for types. (Ignoring legacy old-style
+                # classes.)
+                this_name = iface.__name__
+                duplicate_transform = _implements_name
+            elif (isinstance(iface, Implements)
+                  and not iface.declared
+                  and iface.inherit in interfaces):
+                # If nothing is declared, there's no need to even print this;
+                # it would just show as ``classImplements(Class)``, and the
+                # ``Class`` has typically already.
+                continue
+            else:
+                this_name = repr(iface)
+
+            already_seen = this_name in names
+            names.add(this_name)
+            if already_seen:
+                this_name = duplicate_transform(iface)
+
+            ordered_names.append(this_name)
+        return ', '.join(ordered_names)
+
+
+class _ImmutableDeclaration(Declaration):
+    # A Declaration that is immutable. Used as a singleton to
+    # return empty answers for things like ``implementedBy``.
+    # We have to define the actual singleton after normalizeargs
+    # is defined, and that in turn is defined after InterfaceClass and
+    # Implements.
+
+    __slots__ = ()
+
+    __instance = None
+
+    def __new__(cls):
+        if _ImmutableDeclaration.__instance is None:
+            _ImmutableDeclaration.__instance = object.__new__(cls)
+        return _ImmutableDeclaration.__instance
+
+    def __reduce__(self):
+        return "_empty"
+
+    @property
+    def __bases__(self):
+        return ()
+
+    @__bases__.setter
+    def __bases__(self, new_bases):
+        # We expect the superclass constructor to set ``self.__bases__ = ()``.
+        # Rather than attempt to special case that in the constructor and allow
+        # setting __bases__ only at that time, it's easier to just allow setting
+        # the empty tuple at any time. That makes ``x.__bases__ = x.__bases__`` a nice
+        # no-op too. (Skipping the superclass constructor altogether is a recipe
+        # for maintenance headaches.)
+        if new_bases != ():
+            raise TypeError("Cannot set non-empty bases on shared empty Declaration.")
+
+    # As the immutable empty declaration, we cannot be changed.
+    # This means there's no logical reason for us to have dependents
+    # or subscriptions: we'll never notify them. So there's no need for
+    # us to keep track of any of that.
+    @property
+    def dependents(self):
+        return {}
+
+    changed = subscribe = unsubscribe = lambda self, _ignored: None
+
+    def interfaces(self):
+        # An empty iterator
+        return iter(())
+
+    def extends(self, interface, strict=True):
+        return interface is self._ROOT
+
+    def get(self, name, default=None):
+        return default
+
+    def weakref(self, callback=None):
+        # We're a singleton, we never go away. So there's no need to return
+        # distinct weakref objects here; their callbacks will never
+        # be called. Instead, we only need to return a callable that
+        # returns ourself. The easiest one is to return _ImmutableDeclaration
+        # itself; testing on Python 3.8 shows that's faster than a function that
+        # returns _empty. (Remember, one goal is to avoid allocating any
+        # object, and that includes a method.)
+        return _ImmutableDeclaration
+
+    @property
+    def _v_attrs(self):
+        # _v_attrs is not a public, documented property, but some client code
+        # uses it anyway as a convenient place to cache things. To keep the
+        # empty declaration truly immutable, we must ignore that. That includes
+        # ignoring assignments as well.
+        return {}
+
+    @_v_attrs.setter
+    def _v_attrs(self, new_attrs):
+        pass
+
+
+##############################################################################
+#
+# Implementation specifications
+#
+# These specify interfaces implemented by instances of classes
+
+class Implements(NameAndModuleComparisonMixin,
+                 Declaration):
+    # Inherit from NameAndModuleComparisonMixin to be
+    # mutually comparable with InterfaceClass objects.
+    # (The two must be mutually comparable to be able to work in e.g., BTrees.)
+    # Instances of this class generally don't have a __module__ other than
+    # `zope.interface.declarations`, whereas they *do* have a __name__ that is the
+    # fully qualified name of the object they are representing.
+
+    # Note, though, that equality and hashing are still identity based. This
+    # accounts for things like nested objects that have the same name (typically
+    # only in tests) and is consistent with pickling. As far as comparisons to InterfaceClass
+    # goes, we'll never have equal name and module to those, so we're still consistent there.
+    # Instances of this class are essentially intended to be unique and are
+    # heavily cached (note how our __reduce__ handles this) so having identity
+    # based hash and eq should also work.
+
+    # We want equality and hashing to be based on identity. However, we can't actually
+    # implement __eq__/__ne__ to do this because sometimes we get wrapped in a proxy.
+    # We need to let the proxy types implement these methods so they can handle unwrapping
+    # and then rely on: (1) the interpreter automatically changing `implements == proxy` into
+    # `proxy == implements` (which will call proxy.__eq__ to do the unwrapping) and then
+    # (2) the default equality and hashing semantics being identity based.
+
+    # class whose specification should be used as additional base
+    inherit = None
+
+    # interfaces actually declared for a class
+    declared = ()
+
+    # Weak cache of {class: <implements>} for super objects.
+    # Created on demand. These are rare, as of 5.0 anyway. Using a class
+    # level default doesn't take space in instances. Using _v_attrs would be
+    # another place to store this without taking space unless needed.
+    _super_cache = None
+
+    __name__ = '?'
+
+    @classmethod
+    def named(cls, name, *bases):
+        # Implementation method: Produce an Implements interface with
+        # a fully fleshed out __name__ before calling the constructor, which
+        # sets bases to the given interfaces and which may pass this object to
+        # other objects (e.g., to adjust dependents). If they're sorting or comparing
+        # by name, this needs to be set.
+        inst = cls.__new__(cls)
+        inst.__name__ = name
+        inst.__init__(*bases)
+        return inst
+
+    def changed(self, originally_changed):
+        try:
+            del self._super_cache
+        except AttributeError:
+            pass
+        return super().changed(originally_changed)
+
+    def __repr__(self):
+        if self.inherit:
+            name = getattr(self.inherit, '__name__', None) or _implements_name(self.inherit)
+        else:
+            name = self.__name__
+        declared_names = self._argument_names_for_repr(self.declared)
+        if declared_names:
+            declared_names = ', ' + declared_names
+        return 'classImplements({}{})'.format(name, declared_names)
+
+    def __reduce__(self):
+        return implementedBy, (self.inherit, )
+
+
+def _implements_name(ob):
+    # Return the __name__ attribute to be used by its __implemented__
+    # property.
+    # This must be stable for the "same" object across processes
+    # because it is used for sorting. It needn't be unique, though, in cases
+    # like nested classes named Foo created by different functions, because
+    # equality and hashing is still based on identity.
+    # It might be nice to use __qualname__ on Python 3, but that would produce
+    # different values between Py2 and Py3.
+    return (getattr(ob, '__module__', '?') or '?') + \
+        '.' + (getattr(ob, '__name__', '?') or '?')
+
+
+def _implementedBy_super(sup):
+    # TODO: This is now simple enough we could probably implement
+    # in C if needed.
+
+    # If the class MRO is strictly linear, we could just
+    # follow the normal algorithm for the next class in the
+    # search order (e.g., just return
+    # ``implemented_by_next``). But when diamond inheritance
+    # or mixins + interface declarations are present, we have
+    # to consider the whole MRO and compute a new Implements
+    # that excludes the classes being skipped over but
+    # includes everything else.
+    implemented_by_self = implementedBy(sup.__self_class__)
+    cache = implemented_by_self._super_cache # pylint:disable=protected-access
+    if cache is None:
+        cache = implemented_by_self._super_cache = weakref.WeakKeyDictionary()
+
+    key = sup.__thisclass__
+    try:
+        return cache[key]
+    except KeyError:
+        pass
+
+    next_cls = _next_super_class(sup)
+    # For ``implementedBy(cls)``:
+    # .__bases__ is .declared + [implementedBy(b) for b in cls.__bases__]
+    # .inherit is cls
+
+    implemented_by_next = implementedBy(next_cls)
+    mro = sup.__self_class__.__mro__
+    ix_next_cls = mro.index(next_cls)
+    classes_to_keep = mro[ix_next_cls:]
+    new_bases = [implementedBy(c) for c in classes_to_keep]
+
+    new = Implements.named(
+        implemented_by_self.__name__ + ':' + implemented_by_next.__name__,
+        *new_bases
+    )
+    new.inherit = implemented_by_next.inherit
+    new.declared = implemented_by_next.declared
+    # I don't *think* that new needs to subscribe to ``implemented_by_self``;
+    # it auto-subscribed to its bases, and that should be good enough.
+    cache[key] = new
+
+    return new
+
+
+@_use_c_impl
+def implementedBy(cls): # pylint:disable=too-many-return-statements,too-many-branches
+    """Return the interfaces implemented for a class' instances
+
+      The value returned is an `~zope.interface.interfaces.IDeclaration`.
+    """
+    try:
+        if isinstance(cls, super):
+            # Yes, this needs to be inside the try: block. Some objects
+            # like security proxies even break isinstance.
+            return _implementedBy_super(cls)
+
+        spec = cls.__dict__.get('__implemented__')
+    except AttributeError:
+
+        # we can't get the class dict. This is probably due to a
+        # security proxy.  If this is the case, then probably no
+        # descriptor was installed for the class.
+
+        # We don't want to depend directly on zope.security in
+        # zope.interface, but we'll try to make reasonable
+        # accommodations in an indirect way.
+
+        # We'll check to see if there's an implements:
+
+        spec = getattr(cls, '__implemented__', None)
+        if spec is None:
+            # There's no spec stred in the class. Maybe its a builtin:
+            spec = BuiltinImplementationSpecifications.get(cls)
+            if spec is not None:
+                return spec
+            return _empty
+
+        if spec.__class__ == Implements:
+            # we defaulted to _empty or there was a spec. Good enough.
+            # Return it.
+            return spec
+
+        # TODO: need old style __implements__ compatibility?
+        # Hm, there's an __implemented__, but it's not a spec. Must be
+        # an old-style declaration. Just compute a spec for it
+        return Declaration(*_normalizeargs((spec, )))
+
+    if isinstance(spec, Implements):
+        return spec
+
+    if spec is None:
+        spec = BuiltinImplementationSpecifications.get(cls)
+        if spec is not None:
+            return spec
+
+    # TODO: need old style __implements__ compatibility?
+    spec_name = _implements_name(cls)
+    if spec is not None:
+        # old-style __implemented__ = foo declaration
+        spec = (spec, ) # tuplefy, as it might be just an int
+        spec = Implements.named(spec_name, *_normalizeargs(spec))
+        spec.inherit = None    # old-style implies no inherit
+        del cls.__implemented__ # get rid of the old-style declaration
+    else:
+        try:
+            bases = cls.__bases__
+        except AttributeError:
+            if not callable(cls):
+                raise TypeError("ImplementedBy called for non-factory", cls)
+            bases = ()
+
+        spec = Implements.named(spec_name, *[implementedBy(c) for c in bases])
+        spec.inherit = cls
+
+    try:
+        cls.__implemented__ = spec
+        if not hasattr(cls, '__providedBy__'):
+            cls.__providedBy__ = objectSpecificationDescriptor
+
+        if isinstance(cls, type) and '__provides__' not in cls.__dict__:
+            # Make sure we get a __provides__ descriptor
+            cls.__provides__ = ClassProvides(
+                cls,
+                getattr(cls, '__class__', type(cls)),
+                )
+
+    except TypeError:
+        if not isinstance(cls, type):
+            raise TypeError("ImplementedBy called for non-type", cls)
+        BuiltinImplementationSpecifications[cls] = spec
+
+    return spec
+
+
+def classImplementsOnly(cls, *interfaces):
+    """
+    Declare the only interfaces implemented by instances of a class
+
+    The arguments after the class are one or more interfaces or interface
+    specifications (`~zope.interface.interfaces.IDeclaration` objects).
+
+    The interfaces given (including the interfaces in the specifications)
+    replace any previous declarations, *including* inherited definitions. If you
+    wish to preserve inherited declarations, you can pass ``implementedBy(cls)``
+    in *interfaces*. This can be used to alter the interface resolution order.
+    """
+    spec = implementedBy(cls)
+    # Clear out everything inherited. It's important to
+    # also clear the bases right now so that we don't improperly discard
+    # interfaces that are already implemented by *old* bases that we're
+    # about to get rid of.
+    spec.declared = ()
+    spec.inherit = None
+    spec.__bases__ = ()
+    _classImplements_ordered(spec, interfaces, ())
+
+
+def classImplements(cls, *interfaces):
+    """
+    Declare additional interfaces implemented for instances of a class
+
+    The arguments after the class are one or more interfaces or
+    interface specifications (`~zope.interface.interfaces.IDeclaration` objects).
+
+    The interfaces given (including the interfaces in the specifications)
+    are added to any interfaces previously declared. An effort is made to
+    keep a consistent C3 resolution order, but this cannot be guaranteed.
+
+    .. versionchanged:: 5.0.0
+       Each individual interface in *interfaces* may be added to either the
+       beginning or end of the list of interfaces declared for *cls*,
+       based on inheritance, in order to try to maintain a consistent
+       resolution order. Previously, all interfaces were added to the end.
+    .. versionchanged:: 5.1.0
+       If *cls* is already declared to implement an interface (or derived interface)
+       in *interfaces* through inheritance, the interface is ignored. Previously, it
+       would redundantly be made direct base of *cls*, which often produced inconsistent
+       interface resolution orders. Now, the order will be consistent, but may change.
+       Also, if the ``__bases__`` of the *cls* are later changed, the *cls* will no
+       longer be considered to implement such an interface (changing the ``__bases__`` of *cls*
+       has never been supported).
+    """
+    spec = implementedBy(cls)
+    interfaces = tuple(_normalizeargs(interfaces))
+
+    before = []
+    after = []
+
+    # Take steps to try to avoid producing an invalid resolution
+    # order, while still allowing for BWC (in the past, we always
+    # appended)
+    for iface in interfaces:
+        for b in spec.declared:
+            if iface.extends(b):
+                before.append(iface)
+                break
+        else:
+            after.append(iface)
+    _classImplements_ordered(spec, tuple(before), tuple(after))
+
+
+def classImplementsFirst(cls, iface):
+    """
+    Declare that instances of *cls* additionally provide *iface*.
+
+    The second argument is an interface or interface specification.
+    It is added as the highest priority (first in the IRO) interface;
+    no attempt is made to keep a consistent resolution order.
+
+    .. versionadded:: 5.0.0
+    """
+    spec = implementedBy(cls)
+    _classImplements_ordered(spec, (iface,), ())
+
+
+def _classImplements_ordered(spec, before=(), after=()):
+    # Elide everything already inherited.
+    # Except, if it is the root, and we don't already declare anything else
+    # that would imply it, allow the root through. (TODO: When we disallow non-strict
+    # IRO, this part of the check can be removed because it's not possible to re-declare
+    # like that.)
+    before = [
+        x
+        for x in before
+        if not spec.isOrExtends(x) or (x is Interface and not spec.declared)
+    ]
+    after = [
+        x
+        for x in after
+        if not spec.isOrExtends(x) or (x is Interface and not spec.declared)
+    ]
+
+    # eliminate duplicates
+    new_declared = []
+    seen = set()
+    for l in before, spec.declared, after:
+        for b in l:
+            if b not in seen:
+                new_declared.append(b)
+                seen.add(b)
+
+    spec.declared = tuple(new_declared)
+
+    # compute the bases
+    bases = new_declared # guaranteed no dupes
+
+    if spec.inherit is not None:
+        for c in spec.inherit.__bases__:
+            b = implementedBy(c)
+            if b not in seen:
+                seen.add(b)
+                bases.append(b)
+
+    spec.__bases__ = tuple(bases)
+
+
+def _implements_advice(cls):
+    interfaces, do_classImplements = cls.__dict__['__implements_advice_data__']
+    del cls.__implements_advice_data__
+    do_classImplements(cls, *interfaces)
+    return cls
+
+
+class implementer:
+    """
+    Declare the interfaces implemented by instances of a class.
+
+    This function is called as a class decorator.
+
+    The arguments are one or more interfaces or interface
+    specifications (`~zope.interface.interfaces.IDeclaration`
+    objects).
+
+    The interfaces given (including the interfaces in the
+    specifications) are added to any interfaces previously declared,
+    unless the interface is already implemented.
+
+    Previous declarations include declarations for base classes unless
+    implementsOnly was used.
+
+    This function is provided for convenience. It provides a more
+    convenient way to call `classImplements`. For example::
+
+        @implementer(I1)
+        class C(object):
+            pass
+
+    is equivalent to calling::
+
+        classImplements(C, I1)
+
+    after the class has been created.
+
+    .. seealso:: `classImplements`
+       The change history provided there applies to this function too.
+    """
+    __slots__ = ('interfaces',)
+
+    def __init__(self, *interfaces):
+        self.interfaces = interfaces
+
+    def __call__(self, ob):
+        if isinstance(ob, type):
+            # This is the common branch for classes.
+            classImplements(ob, *self.interfaces)
+            return ob
+
+        spec_name = _implements_name(ob)
+        spec = Implements.named(spec_name, *self.interfaces)
+        try:
+            ob.__implemented__ = spec
+        except AttributeError:
+            raise TypeError("Can't declare implements", ob)
+        return ob
+
+class implementer_only:
+    """Declare the only interfaces implemented by instances of a class
+
+      This function is called as a class decorator.
+
+      The arguments are one or more interfaces or interface
+      specifications (`~zope.interface.interfaces.IDeclaration` objects).
+
+      Previous declarations including declarations for base classes
+      are overridden.
+
+      This function is provided for convenience. It provides a more
+      convenient way to call `classImplementsOnly`. For example::
+
+        @implementer_only(I1)
+        class C(object): pass
+
+      is equivalent to calling::
+
+        classImplementsOnly(I1)
+
+      after the class has been created.
+      """
+
+    def __init__(self, *interfaces):
+        self.interfaces = interfaces
+
+    def __call__(self, ob):
+        if isinstance(ob, (FunctionType, MethodType)):
+            # XXX Does this decorator make sense for anything but classes?
+            # I don't think so. There can be no inheritance of interfaces
+            # on a method or function....
+            raise ValueError('The implementer_only decorator is not '
+                             'supported for methods or functions.')
+
+        # Assume it's a class:
+        classImplementsOnly(ob, *self.interfaces)
+        return ob
+
+
+##############################################################################
+#
+# Instance declarations
+
+class Provides(Declaration):  # Really named ProvidesClass
+    """Implement ``__provides__``, the instance-specific specification
+
+    When an object is pickled, we pickle the interfaces that it implements.
+    """
+
+    def __init__(self, cls, *interfaces):
+        self.__args = (cls, ) + interfaces
+        self._cls = cls
+        Declaration.__init__(self, *self._add_interfaces_to_cls(interfaces, cls))
+
+    # Added to by ``moduleProvides``, et al
+    _v_module_names = ()
+
+    def __repr__(self):
+        # The typical way to create instances of this
+        # object is via calling ``directlyProvides(...)`` or ``alsoProvides()``,
+        # but that's not the only way. Proxies, for example,
+        # directly use the ``Provides(...)`` function (which is the
+        # more generic method, and what we pickle as). We're after the most
+        # readable, useful repr in the common case, so we use the most
+        # common name.
+        #
+        # We also cooperate with ``moduleProvides`` to attempt to do the
+        # right thing for that API. See it for details.
+        function_name = 'directlyProvides'
+        if self._cls is ModuleType and self._v_module_names:
+            # See notes in ``moduleProvides``/``directlyProvides``
+            providing_on_module = True
+            interfaces = self.__args[1:]
+        else:
+            providing_on_module = False
+            interfaces = (self._cls,) + self.__bases__
+        ordered_names = self._argument_names_for_repr(interfaces)
+        if providing_on_module:
+            mod_names = self._v_module_names
+            if len(mod_names) == 1:
+                mod_names = "sys.modules[%r]" % mod_names[0]
+            ordered_names = (
+                '{}, '.format(mod_names)
+            ) + ordered_names
+        return "{}({})".format(
+            function_name,
+            ordered_names,
+        )
+
+    def __reduce__(self):
+        # This reduces to the Provides *function*, not
+        # this class.
+        return Provides, self.__args
+
+    __module__ = 'zope.interface'
+
+    def __get__(self, inst, cls):
+        """Make sure that a class __provides__ doesn't leak to an instance
+        """
+        if inst is None and cls is self._cls:
+            # We were accessed through a class, so we are the class'
+            # provides spec. Just return this object, but only if we are
+            # being called on the same class that we were defined for:
+            return self
+
+        raise AttributeError('__provides__')
+
+ProvidesClass = Provides
+
+# Registry of instance declarations
+# This is a memory optimization to allow objects to share specifications.
+InstanceDeclarations = weakref.WeakValueDictionary()
+
+def Provides(*interfaces): # pylint:disable=function-redefined
+    """Declaration for an instance of *cls*.
+
+       The correct signature is ``cls, *interfaces``.
+       The *cls* is necessary to avoid the
+       construction of inconsistent resolution orders.
+
+      Instance declarations are shared among instances that have the same
+      declaration. The declarations are cached in a weak value dictionary.
+    """
+    spec = InstanceDeclarations.get(interfaces)
+    if spec is None:
+        spec = ProvidesClass(*interfaces)
+        InstanceDeclarations[interfaces] = spec
+
+    return spec
+
+Provides.__safe_for_unpickling__ = True
+
+
+def directlyProvides(object, *interfaces): # pylint:disable=redefined-builtin
+    """Declare interfaces declared directly for an object
+
+      The arguments after the object are one or more interfaces or interface
+      specifications (`~zope.interface.interfaces.IDeclaration` objects).
+
+      The interfaces given (including the interfaces in the specifications)
+      replace interfaces previously declared for the object.
+    """
+    cls = getattr(object, '__class__', None)
+    if cls is not None and getattr(cls, '__class__', None) is cls:
+        # It's a meta class (well, at least it it could be an extension class)
+        # Note that we can't get here from the tests:  there is no normal
+        # class which isn't descriptor aware.
+        if not isinstance(object, type):
+            raise TypeError("Attempt to make an interface declaration on a "
+                            "non-descriptor-aware class")
+
+    interfaces = _normalizeargs(interfaces)
+    if cls is None:
+        cls = type(object)
+
+    if issubclass(cls, type):
+        # we have a class or type.  We'll use a special descriptor
+        # that provides some extra caching
+        object.__provides__ = ClassProvides(object, cls, *interfaces)
+    else:
+        provides = object.__provides__ = Provides(cls, *interfaces)
+        # See notes in ``moduleProvides``.
+        if issubclass(cls, ModuleType) and hasattr(object, '__name__'):
+            provides._v_module_names += (object.__name__,)
+
+
+
+def alsoProvides(object, *interfaces): # pylint:disable=redefined-builtin
+    """Declare interfaces declared directly for an object
+
+    The arguments after the object are one or more interfaces or interface
+    specifications (`~zope.interface.interfaces.IDeclaration` objects).
+
+    The interfaces given (including the interfaces in the specifications) are
+    added to the interfaces previously declared for the object.
+    """
+    directlyProvides(object, directlyProvidedBy(object), *interfaces)
+
+
+def noLongerProvides(object, interface): # pylint:disable=redefined-builtin
+    """ Removes a directly provided interface from an object.
+    """
+    directlyProvides(object, directlyProvidedBy(object) - interface)
+    if interface.providedBy(object):
+        raise ValueError("Can only remove directly provided interfaces.")
+
+
+@_use_c_impl
+class ClassProvidesBase(SpecificationBase):
+
+    __slots__ = (
+        '_cls',
+        '_implements',
+    )
+
+    def __get__(self, inst, cls):
+        # member slots are set by subclass
+        # pylint:disable=no-member
+        if cls is self._cls:
+            # We only work if called on the class we were defined for
+
+            if inst is None:
+                # We were accessed through a class, so we are the class'
+                # provides spec. Just return this object as is:
+                return self
+
+            return self._implements
+
+        raise AttributeError('__provides__')
+
+
+class ClassProvides(Declaration, ClassProvidesBase):
+    """Special descriptor for class ``__provides__``
+
+    The descriptor caches the implementedBy info, so that
+    we can get declarations for objects without instance-specific
+    interfaces a bit quicker.
+    """
+
+    __slots__ = (
+        '__args',
+    )
+
+    def __init__(self, cls, metacls, *interfaces):
+        self._cls = cls
+        self._implements = implementedBy(cls)
+        self.__args = (cls, metacls, ) + interfaces
+        Declaration.__init__(self, *self._add_interfaces_to_cls(interfaces, metacls))
+
+    def __repr__(self):
+        # There are two common ways to get instances of this object:
+        # The most interesting way is calling ``@provider(..)`` as a decorator
+        # of a class; this is the same as calling ``directlyProvides(cls, ...)``.
+        #
+        # The other way is by default: anything that invokes ``implementedBy(x)``
+        # will wind up putting an instance in ``type(x).__provides__``; this includes
+        # the ``@implementer(...)`` decorator. Those instances won't have any
+        # interfaces.
+        #
+        # Thus, as our repr, we go with the ``directlyProvides()`` syntax.
+        interfaces = (self._cls, ) + self.__args[2:]
+        ordered_names = self._argument_names_for_repr(interfaces)
+        return "directlyProvides({})".format(ordered_names)
+
+    def __reduce__(self):
+        return self.__class__, self.__args
+
+    # Copy base-class method for speed
+    __get__ = ClassProvidesBase.__get__
+
+
+def directlyProvidedBy(object): # pylint:disable=redefined-builtin
+    """Return the interfaces directly provided by the given object
+
+    The value returned is an `~zope.interface.interfaces.IDeclaration`.
+    """
+    provides = getattr(object, "__provides__", None)
+    if (
+            provides is None # no spec
+            # We might have gotten the implements spec, as an
+            # optimization. If so, it's like having only one base, that we
+            # lop off to exclude class-supplied declarations:
+            or isinstance(provides, Implements)
+    ):
+        return _empty
+
+    # Strip off the class part of the spec:
+    return Declaration(provides.__bases__[:-1])
+
+
+class provider:
+    """Declare interfaces provided directly by a class
+
+      This function is called in a class definition.
+
+      The arguments are one or more interfaces or interface specifications
+      (`~zope.interface.interfaces.IDeclaration` objects).
+
+      The given interfaces (including the interfaces in the specifications)
+      are used to create the class's direct-object interface specification.
+      An error will be raised if the module class has an direct interface
+      specification. In other words, it is an error to call this function more
+      than once in a class definition.
+
+      Note that the given interfaces have nothing to do with the interfaces
+      implemented by instances of the class.
+
+      This function is provided for convenience. It provides a more convenient
+      way to call `directlyProvides` for a class. For example::
+
+        @provider(I1)
+        class C:
+            pass
+
+      is equivalent to calling::
+
+        directlyProvides(C, I1)
+
+      after the class has been created.
+    """
+
+    def __init__(self, *interfaces):
+        self.interfaces = interfaces
+
+    def __call__(self, ob):
+        directlyProvides(ob, *self.interfaces)
+        return ob
+
+
+def moduleProvides(*interfaces):
+    """Declare interfaces provided by a module
+
+    This function is used in a module definition.
+
+    The arguments are one or more interfaces or interface specifications
+    (`~zope.interface.interfaces.IDeclaration` objects).
+
+    The given interfaces (including the interfaces in the specifications) are
+    used to create the module's direct-object interface specification.  An
+    error will be raised if the module already has an interface specification.
+    In other words, it is an error to call this function more than once in a
+    module definition.
+
+    This function is provided for convenience. It provides a more convenient
+    way to call directlyProvides. For example::
+
+      moduleProvides(I1)
+
+    is equivalent to::
+
+      directlyProvides(sys.modules[__name__], I1)
+    """
+    frame = sys._getframe(1) # pylint:disable=protected-access
+    locals = frame.f_locals # pylint:disable=redefined-builtin
+
+    # Try to make sure we were called from a module body
+    if (locals is not frame.f_globals) or ('__name__' not in locals):
+        raise TypeError(
+            "moduleProvides can only be used from a module definition.")
+
+    if '__provides__' in locals:
+        raise TypeError(
+            "moduleProvides can only be used once in a module definition.")
+
+    # Note: This is cached based on the key ``(ModuleType, *interfaces)``;
+    # One consequence is that any module that provides the same interfaces
+    # gets the same ``__repr__``, meaning that you can't tell what module
+    # such a declaration came from. Adding the module name to ``_v_module_names``
+    # attempts to correct for this; it works in some common situations, but fails
+    # (1) after pickling (the data is lost) and (2) if declarations are
+    # actually shared and (3) if the alternate spelling of ``directlyProvides()``
+    # is used. Problem (3)  is fixed by cooperating with ``directlyProvides``
+    # to maintain this information, and problem (2) is worked around by
+    # printing all the names, but (1) is unsolvable without introducing
+    # new classes or changing the stored data...but it doesn't actually matter,
+    # because ``ModuleType`` can't be pickled!
+    p = locals["__provides__"] = Provides(ModuleType,
+                                          *_normalizeargs(interfaces))
+    p._v_module_names += (locals['__name__'],)
+
+
+##############################################################################
+#
+# Declaration querying support
+
+# XXX:  is this a fossil?  Nobody calls it, no unit tests exercise it, no
+#       doctests import it, and the package __init__ doesn't import it.
+#       (Answer: Versions of zope.container prior to 4.4.0 called this,
+#        and zope.proxy.decorator up through at least 4.3.5 called this.)
+def ObjectSpecification(direct, cls):
+    """Provide object specifications
+
+    These combine information for the object and for it's classes.
+    """
+    return Provides(cls, direct) # pragma: no cover fossil
+
+@_use_c_impl
+def getObjectSpecification(ob):
+    try:
+        provides = ob.__provides__
+    except AttributeError:
+        provides = None
+
+    if provides is not None:
+        if isinstance(provides, SpecificationBase):
+            return provides
+
+    try:
+        cls = ob.__class__
+    except AttributeError:
+        # We can't get the class, so just consider provides
+        return _empty
+    return implementedBy(cls)
+
+
+@_use_c_impl
+def providedBy(ob):
+    """
+    Return the interfaces provided by *ob*.
+
+    If *ob* is a :class:`super` object, then only interfaces implemented
+    by the remainder of the classes in the method resolution order are
+    considered. Interfaces directly provided by the object underlying *ob*
+    are not.
+    """
+    # Here we have either a special object, an old-style declaration
+    # or a descriptor
+
+    # Try to get __providedBy__
+    try:
+        if isinstance(ob, super): # Some objects raise errors on isinstance()
+            return implementedBy(ob)
+
+        r = ob.__providedBy__
+    except AttributeError:
+        # Not set yet. Fall back to lower-level thing that computes it
+        return getObjectSpecification(ob)
+
+    try:
+        # We might have gotten a descriptor from an instance of a
+        # class (like an ExtensionClass) that doesn't support
+        # descriptors.  We'll make sure we got one by trying to get
+        # the only attribute, which all specs have.
+        r.extends
+    except AttributeError:
+
+        # The object's class doesn't understand descriptors.
+        # Sigh. We need to get an object descriptor, but we have to be
+        # careful.  We want to use the instance's __provides__, if
+        # there is one, but only if it didn't come from the class.
+
+        try:
+            r = ob.__provides__
+        except AttributeError:
+            # No __provides__, so just fall back to implementedBy
+            return implementedBy(ob.__class__)
+
+        # We need to make sure we got the __provides__ from the
+        # instance. We'll do this by making sure we don't get the same
+        # thing from the class:
+
+        try:
+            cp = ob.__class__.__provides__
+        except AttributeError:
+            # The ob doesn't have a class or the class has no
+            # provides, assume we're done:
+            return r
+
+        if r is cp:
+            # Oops, we got the provides from the class. This means
+            # the object doesn't have it's own. We should use implementedBy
+            return implementedBy(ob.__class__)
+
+    return r
+
+
+@_use_c_impl
+class ObjectSpecificationDescriptor:
+    """Implement the ``__providedBy__`` attribute
+
+    The ``__providedBy__`` attribute computes the interfaces provided by
+    an object. If an object has an ``__provides__`` attribute, that is returned.
+    Otherwise, `implementedBy` the *cls* is returned.
+
+    .. versionchanged:: 5.4.0
+       Both the default (C) implementation and the Python implementation
+       now let exceptions raised by accessing ``__provides__`` propagate.
+       Previously, the C version ignored all exceptions.
+    .. versionchanged:: 5.4.0
+       The Python implementation now matches the C implementation and lets
+       a ``__provides__`` of ``None`` override what the class is declared to
+       implement.
+    """
+
+    def __get__(self, inst, cls):
+        """Get an object specification for an object
+        """
+        if inst is None:
+            return getObjectSpecification(cls)
+
+        try:
+            return inst.__provides__
+        except AttributeError:
+            return implementedBy(cls)
+
+
+##############################################################################
+
+def _normalizeargs(sequence, output=None):
+    """Normalize declaration arguments
+
+    Normalization arguments might contain Declarions, tuples, or single
+    interfaces.
+
+    Anything but individual interfaces or implements specs will be expanded.
+    """
+    if output is None:
+        output = []
+
+    cls = sequence.__class__
+    if InterfaceClass in cls.__mro__ or Implements in cls.__mro__:
+        output.append(sequence)
+    else:
+        for v in sequence:
+            _normalizeargs(v, output)
 
-.. currentmodule:: zope.interface
+    return output
 
-Interfaces are objects that specify (document) the external behavior
-of objects that "provide" them.  An interface specifies behavior
-through:
+_empty = _ImmutableDeclaration()
 
-- Informal documentation in a doc string
-
-- Attribute definitions
-
-- Invariants, which are conditions that must hold for objects that
-  provide the interface
-
-Attribute definitions specify specific attributes. They define the
-attribute name and provide documentation and constraints of attribute
-values.  Attribute definitions can take a number of forms, as we'll
-see below.
-
-Defining interfaces
-===================
-
-Interfaces are defined using Python ``class`` statements:
-
-.. doctest::
-
-  >>> import zope.interface
-  >>> class IFoo(zope.interface.Interface):
-  ...    """Foo blah blah"""
-  ...
-  ...    x = zope.interface.Attribute("""X blah blah""")
-  ...
-  ...    def bar(q, r=None):
-  ...        """bar blah blah"""
-
-In the example above, we've created an interface, :class:`IFoo`.  We
-subclassed :class:`zope.interface.Interface`, which is an ancestor interface for
-all interfaces, much as ``object`` is an ancestor of all new-style
-classes [#create]_.   The interface is not a class, it's an Interface,
-an instance of :class:`zope.interface.interface.InterfaceClass`:
-
-.. doctest::
-
-  >>> type(IFoo)
-  <class 'zope.interface.interface.InterfaceClass'>
-
-We can ask for the interface's documentation:
-
-.. doctest::
-
-  >>> IFoo.__doc__
-  'Foo blah blah'
-
-and its name:
-
-.. doctest::
-
-  >>> IFoo.__name__
-  'IFoo'
-
-and even its module:
-
-.. doctest::
-
-  >>> IFoo.__module__
-  'builtins'
-
-The interface defined two attributes:
-
-``x``
-  This is the simplest form of attribute definition.  It has a name
-  and a doc string.  It doesn't formally specify anything else.
-
-``bar``
-  This is a method.  A method is defined via a function definition.  A
-  method is simply an attribute constrained to be a callable with a
-  particular signature, as provided by the function definition.
-
-  Note that ``bar`` doesn't take a ``self`` argument.  Interfaces document
-  how an object is *used*.  When calling instance methods, you don't
-  pass a ``self`` argument, so a ``self`` argument isn't included in the
-  interface signature.  The ``self`` argument in instance methods is
-  really an implementation detail of Python instances. Other objects,
-  besides instances can provide interfaces and their methods might not
-  be instance methods. For example, modules can provide interfaces and
-  their methods are usually just functions.  Even instances can have
-  methods that are not instance methods.
-
-You can access the attributes defined by an interface using mapping
-syntax:
-
-.. doctest::
-
-  >>> x = IFoo['x']
-  >>> type(x)
-  <class 'zope.interface.interface.Attribute'>
-  >>> x.__name__
-  'x'
-  >>> x.__doc__
-  'X blah blah'
-
-  >>> IFoo.get('x').__name__
-  'x'
-
-  >>> IFoo.get('y')
-
-You can use ``in`` to determine if an interface defines a name:
-
-.. doctest::
-
-  >>> 'x' in IFoo
-  True
-
-You can iterate over interfaces to get the names they define:
-
-.. doctest::
-
-  >>> names = list(IFoo)
-  >>> names.sort()
-  >>> names
-  ['bar', 'x']
-
-Remember that interfaces aren't classes. You can't access attribute
-definitions as attributes of interfaces:
-
-.. doctest::
-
-  >>> IFoo.x
-  Traceback (most recent call last):
-    File "<stdin>", line 1, in ?
-  AttributeError: 'InterfaceClass' object has no attribute 'x'
-
-Methods provide access to the method signature:
-
-.. doctest::
-
-  >>> bar = IFoo['bar']
-  >>> bar.getSignatureString()
-  '(q, r=None)'
-
-TODO
-  Methods really should have a better API.  This is something that
-  needs to be improved.
-
-Declaring interfaces
-====================
-
-Having defined interfaces, we can *declare* that objects provide
-them.  Before we describe the details, lets define some terms:
-
-*provide*
-   We say that objects *provide* interfaces.  If an object provides an
-   interface, then the interface specifies the behavior of the
-   object. In other words, interfaces specify the behavior of the
-   objects that provide them.
-
-*implement*
-   We normally say that classes *implement* interfaces.  If a class
-   implements an interface, then the instances of the class provide
-   the interface.  Objects provide interfaces that their classes
-   implement [#factory]_.  (Objects can provide interfaces directly,
-   in addition to what their classes implement.)
-
-   It is important to note that classes don't usually provide the
-   interfaces that they implement.
-
-   We can generalize this to factories.  For any callable object we
-   can declare that it produces objects that provide some interfaces
-   by saying that the factory implements the interfaces.
-
-Now that we've defined these terms, we can talk about the API for
-declaring interfaces.
-
-Declaring implemented interfaces
---------------------------------
-
-The most common way to declare interfaces is using the `implementer`
-decorator on a class:
-
-.. doctest::
-
-  >>> @zope.interface.implementer(IFoo)
-  ... class Foo:
-  ...
-  ...     def __init__(self, x=None):
-  ...         self.x = x
-  ...
-  ...     def bar(self, q, r=None):
-  ...         return q, r, self.x
-  ...
-  ...     def __repr__(self):
-  ...         return "Foo(%s)" % self.x
-
-
-In this example, we declared that ``Foo`` implements ``IFoo``. This means
-that instances of ``Foo`` provide ``IFoo``.  Having made this declaration,
-there are several ways we can introspect the declarations.  First, we
-can ask an interface whether it is implemented by a class:
-
-.. doctest::
-
-  >>> IFoo.implementedBy(Foo)
-  True
-
-And we can ask whether an interface is provided by an object:
-
-.. doctest::
-
-  >>> foo = Foo()
-  >>> IFoo.providedBy(foo)
-  True
-
-Of course, ``Foo`` doesn't *provide* ``IFoo``, it *implements* it:
-
-.. doctest::
-
-  >>> IFoo.providedBy(Foo)
-  False
-
-We can also ask what interfaces are implemented by a class:
-
-.. doctest::
-
-  >>> list(zope.interface.implementedBy(Foo))
-  [<InterfaceClass builtins.IFoo>]
-
-It's an error to ask for interfaces implemented by a non-callable
-object:
-
-.. doctest::
-
-  >>> IFoo.implementedBy(foo)
-  Traceback (most recent call last):
-  ...
-  TypeError: ('ImplementedBy called for non-factory', Foo(None))
-
-  >>> list(zope.interface.implementedBy(foo))
-  Traceback (most recent call last):
-  ...
-  TypeError: ('ImplementedBy called for non-factory', Foo(None))
-
-Similarly, we can ask what interfaces are provided by an object:
-
-.. doctest::
-
-  >>> list(zope.interface.providedBy(foo))
-  [<InterfaceClass builtins.IFoo>]
-  >>> list(zope.interface.providedBy(Foo))
-  []
-
-We can declare interfaces implemented by other factories (besides
-classes).  We do this using the same `implementer` decorator.
-
-.. doctest::
-
-  >>> @zope.interface.implementer(IFoo)
-  ... def yfoo(y):
-  ...     foo = Foo()
-  ...     foo.y = y
-  ...     return foo
-
-  >>> list(zope.interface.implementedBy(yfoo))
-  [<InterfaceClass builtins.IFoo>]
-
-Note that the implementer decorator may modify its argument. Callers
-should not assume that a new object is created.
-
-Using implementer also works on callable objects. This is used by
-:py:mod:`zope.formlib`, as an example:
-
-.. doctest::
-
-  >>> class yfactory:
-  ...     def __call__(self, y):
-  ...         foo = Foo()
-  ...         foo.y = y
-  ...         return foo
-  >>> yfoo = yfactory()
-  >>> yfoo = zope.interface.implementer(IFoo)(yfoo)
-
-  >>> list(zope.interface.implementedBy(yfoo))
-  [<InterfaceClass builtins.IFoo>]
-
-XXX: Double check and update these version numbers:
-
-In :py:mod:`zope.interface` 3.5.2 and lower, the implementer decorator can not
-be used for classes, but in 3.6.0 and higher it can:
-
-.. doctest::
-
-  >>> Foo = zope.interface.implementer(IFoo)(Foo)
-  >>> list(zope.interface.providedBy(Foo()))
-  [<InterfaceClass builtins.IFoo>]
-
-Note that class decorators using the ``@implementer(IFoo)`` syntax are only
-supported in Python 2.6 and later.
-
-.. autofunction:: implementer
-   :noindex:
-
-   .. XXX: Duplicate description.
-
-Declaring provided interfaces
------------------------------
-
-We can declare interfaces directly provided by objects.  Suppose that
-we want to document what the ``__init__`` method of the ``Foo`` class
-does.  It's not *really* part of ``IFoo``.  You wouldn't normally call
-the ``__init__`` method on Foo instances.  Rather, the ``__init__`` method
-is part of ``Foo``'s ``__call__`` method:
-
-.. doctest::
-
-  >>> class IFooFactory(zope.interface.Interface):
-  ...     """Create foos"""
-  ...
-  ...     def __call__(x=None):
-  ...         """Create a foo
-  ...
-  ...         The argument provides the initial value for x ...
-  ...         """
-
-It's the class that provides this interface, so we declare the
-interface on the class:
-
-.. doctest::
-
-  >>> zope.interface.directlyProvides(Foo, IFooFactory)
-
-And then, we'll see that Foo provides some interfaces:
-
-.. doctest::
-
-  >>> list(zope.interface.providedBy(Foo))
-  [<InterfaceClass builtins.IFooFactory>]
-  >>> IFooFactory.providedBy(Foo)
-  True
-
-Declaring class interfaces is common enough that there's a special
-decorator for it, `provider`:
-
-.. doctest::
-
-  >>> @zope.interface.implementer(IFoo)
-  ... @zope.interface.provider(IFooFactory)
-  ... class Foo2:
-  ...
-  ...     def __init__(self, x=None):
-  ...         self.x = x
-  ...
-  ...     def bar(self, q, r=None):
-  ...         return q, r, self.x
-  ...
-  ...     def __repr__(self):
-  ...         return "Foo(%s)" % self.x
-
-  >>> list(zope.interface.providedBy(Foo2))
-  [<InterfaceClass builtins.IFooFactory>]
-  >>> IFooFactory.providedBy(Foo2)
-  True
-
-There's a similar function, ``moduleProvides``, that supports interface
-declarations from within module definitions.  For example, see the use
-of ``moduleProvides`` call in ``zope.interface.__init__``, which declares that
-the package ``zope.interface`` provides ``IInterfaceDeclaration``.
-
-Sometimes, we want to declare interfaces on instances, even though
-those instances get interfaces from their classes.  Suppose we create
-a new interface, ``ISpecial``:
-
-.. doctest::
-
-  >>> class ISpecial(zope.interface.Interface):
-  ...     reason = zope.interface.Attribute("Reason why we're special")
-  ...     def brag():
-  ...         "Brag about being special"
-
-We can make an existing foo instance special by providing ``reason``
-and ``brag`` attributes:
-
-.. doctest::
-
-  >>> foo.reason = 'I just am'
-  >>> def brag():
-  ...      return "I'm special!"
-  >>> foo.brag = brag
-  >>> foo.reason
-  'I just am'
-  >>> foo.brag()
-  "I'm special!"
-
-and by declaring the interface:
-
-.. doctest::
-
-  >>> zope.interface.directlyProvides(foo, ISpecial)
-
-then the new interface is included in the provided interfaces:
-
-.. doctest::
-
-  >>> ISpecial.providedBy(foo)
-  True
-  >>> list(zope.interface.providedBy(foo))
-  [<InterfaceClass builtins.ISpecial>, <InterfaceClass builtins.IFoo>]
-
-We can find out what interfaces are directly provided by an object:
-
-.. doctest::
-
-  >>> list(zope.interface.directlyProvidedBy(foo))
-  [<InterfaceClass builtins.ISpecial>]
-
-  >>> newfoo = Foo()
-  >>> list(zope.interface.directlyProvidedBy(newfoo))
-  []
-
-.. autofunction:: provider
-   :noindex:
-
-   .. XXX: Duplicate description.
-
-Inherited declarations
-----------------------
-
-Normally, declarations are inherited:
-
-.. doctest::
-
-  >>> @zope.interface.implementer(ISpecial)
-  ... class SpecialFoo(Foo):
-  ...     reason = 'I just am'
-  ...     def brag(self):
-  ...         return "I'm special because %s" % self.reason
-
-  >>> list(zope.interface.implementedBy(SpecialFoo))
-  [<InterfaceClass builtins.ISpecial>, <InterfaceClass builtins.IFoo>]
-
-  >>> list(zope.interface.providedBy(SpecialFoo()))
-  [<InterfaceClass builtins.ISpecial>, <InterfaceClass builtins.IFoo>]
-
-Sometimes, you don't want to inherit declarations.  In that case, you
-can use ``implementer_only``, instead of ``implementer``:
-
-.. doctest::
-
-  >>> @zope.interface.implementer_only(ISpecial)
-  ... class Special(Foo):
-  ...     reason = 'I just am'
-  ...     def brag(self):
-  ...         return "I'm special because %s" % self.reason
-
-  >>> list(zope.interface.implementedBy(Special))
-  [<InterfaceClass builtins.ISpecial>]
-
-  >>> list(zope.interface.providedBy(Special()))
-  [<InterfaceClass builtins.ISpecial>]
-
-External declarations
----------------------
-
-Normally, we make implementation declarations as part of a class
-definition. Sometimes, we may want to make declarations from outside
-the class definition. For example, we might want to declare interfaces
-for classes that we didn't write.  The function ``classImplements`` can
-be used for this purpose:
-
-.. doctest::
-
-  >>> class C:
-  ...     pass
-
-  >>> zope.interface.classImplements(C, IFoo)
-  >>> list(zope.interface.implementedBy(C))
-  [<InterfaceClass builtins.IFoo>]
-
-.. autofunction:: classImplements
-   :noindex:
-
-We can use ``classImplementsOnly`` to exclude inherited interfaces:
-
-.. doctest::
-
-  >>> class C(Foo):
-  ...     pass
-
-  >>> zope.interface.classImplementsOnly(C, ISpecial)
-  >>> list(zope.interface.implementedBy(C))
-  [<InterfaceClass builtins.ISpecial>]
-
-.. autofunction:: classImplementsOnly
-   :noindex:
-
-   .. XXX: Duplicate description.
-
-Declaration Objects
--------------------
-
-When we declare interfaces, we create *declaration* objects.  When we
-query declarations, declaration objects are returned:
-
-.. doctest::
-
-  >>> type(zope.interface.implementedBy(Special))
-  <class 'zope.interface.declarations.Implements'>
-
-Declaration objects and interface objects are similar in many ways. In
-fact, they share a common base class.  The important thing to realize
-about them is that they can be used where interfaces are expected in
-declarations. Here's a silly example:
-
-.. doctest::
-
-  >>> @zope.interface.implementer_only(
-  ...     zope.interface.implementedBy(Foo),
-  ...     ISpecial,
-  ... )
-  ... class Special2(object):
-  ...     reason = 'I just am'
-  ...     def brag(self):
-  ...         return "I'm special because %s" % self.reason
-
-The declaration here is almost the same as
-``zope.interface.implementer(ISpecial)``, except that the order of
-interfaces in the resulting declaration is different:
-
-.. doctest::
-
-  >>> list(zope.interface.implementedBy(Special2))
-  [<InterfaceClass builtins.IFoo>, <InterfaceClass builtins.ISpecial>]
-
-
-Interface Inheritance
-=====================
-
-Interfaces can extend other interfaces. They do this simply by listing
-the other interfaces as base interfaces:
-
-.. doctest::
-
-  >>> class IBlat(zope.interface.Interface):
-  ...     """Blat blah blah"""
-  ...
-  ...     y = zope.interface.Attribute("y blah blah")
-  ...     def eek():
-  ...         """eek blah blah"""
-
-  >>> IBlat.__bases__
-  (<InterfaceClass zope.interface.Interface>,)
-
-  >>> class IBaz(IFoo, IBlat):
-  ...     """Baz blah"""
-  ...     def eek(a=1):
-  ...         """eek in baz blah"""
-  ...
-
-  >>> IBaz.__bases__
-  (<InterfaceClass builtins.IFoo>, <InterfaceClass builtins.IBlat>)
-
-  >>> names = list(IBaz)
-  >>> names.sort()
-  >>> names
-  ['bar', 'eek', 'x', 'y']
-
-Note that ``IBaz`` overrides ``eek``:
-
-.. doctest::
-
-  >>> IBlat['eek'].__doc__
-  'eek blah blah'
-  >>> IBaz['eek'].__doc__
-  'eek in baz blah'
-
-We were careful to override ``eek`` in a compatible way.  When extending
-an interface, the extending interface should be compatible [#compat]_
-with the extended interfaces.
-
-We can ask whether one interface extends another:
-
-.. doctest::
-
-  >>> IBaz.extends(IFoo)
-  True
-  >>> IBlat.extends(IFoo)
-  False
-
-Note that interfaces don't extend themselves:
-
-.. doctest::
-
-  >>> IBaz.extends(IBaz)
-  False
-
-Sometimes we wish they did, but we can instead use ``isOrExtends``:
-
-.. doctest::
-
-  >>> IBaz.isOrExtends(IBaz)
-  True
-  >>> IBaz.isOrExtends(IFoo)
-  True
-  >>> IFoo.isOrExtends(IBaz)
-  False
-
-When we iterate over an interface, we get all of the names it defines,
-including names defined by base interfaces. Sometimes, we want *just*
-the names defined by the interface directly. We can use the ``names``
-method for that:
-
-.. doctest::
-
-  >>> list(IBaz.names())
-  ['eek']
-
-Inheritance of attribute specifications
----------------------------------------
-
-An interface may override attribute definitions from base interfaces.
-If two base interfaces define the same attribute, the attribute is
-inherited from the most specific interface. For example, with:
-
-.. doctest::
-
-  >>> class IBase(zope.interface.Interface):
-  ...
-  ...     def foo():
-  ...         "base foo doc"
-
-  >>> class IBase1(IBase):
-  ...     pass
-
-  >>> class IBase2(IBase):
-  ...
-  ...     def foo():
-  ...         "base2 foo doc"
-
-  >>> class ISub(IBase1, IBase2):
-  ...     pass
-
-``ISub``'s definition of ``foo`` is the one from ``IBase2``, since ``IBase2`` is more
-specific than ``IBase``:
-
-.. doctest::
-
-  >>> ISub['foo'].__doc__
-  'base2 foo doc'
-
-Note that this differs from a depth-first search.
-
-Sometimes, it's useful to ask whether an interface defines an
-attribute directly.  You can use the direct method to get a directly
-defined definitions:
-
-.. doctest::
-
-  >>> IBase.direct('foo').__doc__
-  'base foo doc'
-
-  >>> ISub.direct('foo')
-
-Specifications
---------------
-
-Interfaces and declarations are both special cases of specifications.
-What we described above for interface inheritance applies to both
-declarations and specifications.  Declarations actually extend the
-interfaces that they declare:
-
-.. doctest::
-
-  >>> @zope.interface.implementer(IBaz)
-  ... class Baz(object):
-  ...     pass
-
-  >>> baz_implements = zope.interface.implementedBy(Baz)
-  >>> baz_implements.__bases__
-  (<InterfaceClass builtins.IBaz>, classImplements(object))
-
-  >>> baz_implements.extends(IFoo)
-  True
-
-  >>> baz_implements.isOrExtends(IFoo)
-  True
-  >>> baz_implements.isOrExtends(baz_implements)
-  True
-
-Specifications (interfaces and declarations) provide an ``__sro__``
-that lists the specification and all of it's ancestors:
-
-.. doctest::
-
-  >>> from pprint import pprint
-  >>> pprint(baz_implements.__sro__)
-  (classImplements(Baz, IBaz),
-   <InterfaceClass builtins.IBaz>,
-   <InterfaceClass builtins.IFoo>,
-   <InterfaceClass builtins.IBlat>,
-   classImplements(object),
-   <InterfaceClass zope.interface.Interface>)
-  >>> class IBiz(zope.interface.Interface):
-  ...    pass
-  >>> @zope.interface.implementer(IBiz)
-  ... class Biz(Baz):
-  ...    pass
-  >>> pprint(zope.interface.implementedBy(Biz).__sro__)
-  (classImplements(Biz, IBiz),
-   <InterfaceClass builtins.IBiz>,
-   classImplements(Baz, IBaz),
-   <InterfaceClass builtins.IBaz>,
-   <InterfaceClass builtins.IFoo>,
-   <InterfaceClass builtins.IBlat>,
-   classImplements(object),
-   <InterfaceClass zope.interface.Interface>)
-
-Tagged Values
-=============
-
-.. autofunction:: taggedValue
-
-Interfaces and attribute descriptions support an extension mechanism,
-borrowed from UML, called "tagged values" that lets us store extra
-data:
-
-.. doctest::
-
-  >>> IFoo.setTaggedValue('date-modified', '2004-04-01')
-  >>> IFoo.setTaggedValue('author', 'Jim Fulton')
-  >>> IFoo.getTaggedValue('date-modified')
-  '2004-04-01'
-  >>> IFoo.queryTaggedValue('date-modified')
-  '2004-04-01'
-  >>> IFoo.queryTaggedValue('datemodified')
-  >>> tags = list(IFoo.getTaggedValueTags())
-  >>> tags.sort()
-  >>> tags
-  ['author', 'date-modified']
-
-Function attributes are converted to tagged values when method
-attribute definitions are created:
-
-.. doctest::
-
-  >>> class IBazFactory(zope.interface.Interface):
-  ...     def __call__():
-  ...         "create one"
-  ...     __call__.return_type = IBaz
-
-  >>> IBazFactory['__call__'].getTaggedValue('return_type')
-  <InterfaceClass builtins.IBaz>
-
-Tagged values can also be defined from within an interface definition:
-
-.. doctest::
-
-  >>> class IWithTaggedValues(zope.interface.Interface):
-  ...     zope.interface.taggedValue('squish', 'squash')
-  >>> IWithTaggedValues.getTaggedValue('squish')
-  'squash'
-
-Tagged values are inherited in the same way that attribute and method
-descriptions are. Inheritance can be ignored by using the "direct"
-versions of functions.
-
-.. doctest::
-
-   >>> class IExtendsIWithTaggedValues(IWithTaggedValues):
-   ...     zope.interface.taggedValue('child', True)
-   >>> IExtendsIWithTaggedValues.getTaggedValue('child')
-   True
-   >>> IExtendsIWithTaggedValues.getDirectTaggedValue('child')
-   True
-   >>> IExtendsIWithTaggedValues.getTaggedValue('squish')
-   'squash'
-   >>> print(IExtendsIWithTaggedValues.queryDirectTaggedValue('squish'))
-   None
-   >>> IExtendsIWithTaggedValues.setTaggedValue('squish', 'SQUASH')
-   >>> IExtendsIWithTaggedValues.getTaggedValue('squish')
-   'SQUASH'
-   >>> IExtendsIWithTaggedValues.getDirectTaggedValue('squish')
-   'SQUASH'
-
-
-Invariants
-==========
-
-.. autofunction:: invariant
-
-Interfaces can express conditions that must hold for objects that
-provide them. These conditions are expressed using one or more
-invariants.  Invariants are callable objects that will be called with
-an object that provides an interface. An invariant raises an ``Invalid``
-exception if the condition doesn't hold.  Here's an example:
-
-.. doctest::
-
-  >>> class RangeError(zope.interface.Invalid):
-  ...     """A range has invalid limits"""
-  ...     def __repr__(self):
-  ...         return "RangeError(%r)" % self.args
-
-  >>> def range_invariant(ob):
-  ...     if ob.max < ob.min:
-  ...         raise RangeError(ob)
-
-Given this invariant, we can use it in an interface definition:
-
-.. doctest::
-
-  >>> class IRange(zope.interface.Interface):
-  ...     min = zope.interface.Attribute("Lower bound")
-  ...     max = zope.interface.Attribute("Upper bound")
-  ...
-  ...     zope.interface.invariant(range_invariant)
-
-Interfaces have a method for checking their invariants:
-
-.. doctest::
-
-  >>> @zope.interface.implementer(IRange)
-  ... class Range(object):
-  ...     def __init__(self, min, max):
-  ...         self.min, self.max = min, max
-  ...
-  ...     def __repr__(self):
-  ...         return "Range(%s, %s)" % (self.min, self.max)
-
-  >>> IRange.validateInvariants(Range(1,2))
-  >>> IRange.validateInvariants(Range(1,1))
-  >>> IRange.validateInvariants(Range(2,1))
-  Traceback (most recent call last):
-  ...
-  RangeError: Range(2, 1)
-
-If you have multiple invariants, you may not want to stop checking
-after the first error.  If you pass a list to ``validateInvariants``,
-then a single ``Invalid`` exception will be raised with the list of
-exceptions as its argument:
-
-.. doctest::
-
-  >>> from zope.interface.exceptions import Invalid
-  >>> errors = []
-  >>> try:
-  ...     IRange.validateInvariants(Range(2,1), errors)
-  ... except Invalid as e:
-  ...     str(e)
-  '[RangeError(Range(2, 1))]'
-
-And the list will be filled with the individual exceptions:
-
-.. doctest::
-
-  >>> errors
-  [RangeError(Range(2, 1))]
-
-  >>> del errors[:]
-
-Adaptation
-==========
-
-Interfaces can be called to perform *adaptation*. Adaptation is the
-process of converting an object to an object implementing the
-interface. For example, in mathematics, to represent a point in space
-or on a graph there's the familiar Cartesian coordinate system using
-``CartesianPoint(x, y)``, and there's also the Polar coordinate system
-using ``PolarPoint(r, theta)``, plus several others (homogeneous,
-log-polar, etc). Polar points are most convenient for some types of
-operations, but cartesian points may make more intuitive sense to most
-people. Before printing an arbitrary point, we might want to *adapt* it
-to ``ICartesianPoint``, or before performing some mathematical
-operation you might want to adapt the arbitrary point to ``IPolarPoint``.
-
-The semantics are based on those of the  :pep:`246` ``adapt``
-function.
-
-If an object cannot be adapted, then a ``TypeError`` is raised:
-
-.. doctest::
-
-  >>> class ICartesianPoint(zope.interface.Interface):
-  ...     x = zope.interface.Attribute("Distance from origin along x axis")
-  ...     y = zope.interface.Attribute("Distance from origin along y axis")
-
-  >>> ICartesianPoint(0)
-  Traceback (most recent call last):
-  ...
-  TypeError: ('Could not adapt', 0, <InterfaceClass builtins.ICartesianPoint>)
-
-
-unless a default value is provided as a second positional argument;
-this value is not checked to see if it implements the interface:
-
-.. doctest::
-
-  >>> ICartesianPoint(0, 'bob')
-  'bob'
-
-If an object already implements the interface, then it will be returned:
-
-.. doctest::
-
-  >>> @zope.interface.implementer(ICartesianPoint)
-  ... class CartesianPoint(object):
-  ...     """The default cartesian point is the origin."""
-  ...     def __init__(self, x=0, y=0):
-  ...         self.x = x
-  ...         self.y = y
-  ...     def __repr__(self):
-  ...         return "CartesianPoint(%s, %s)" % (self.x, self.y)
-
-  >>> obj = CartesianPoint()
-  >>> ICartesianPoint(obj) is obj
-  True
-
-``__conform__``
----------------
-
-:pep:`246` outlines a requirement:
-
-    When the object knows about the [interface], and either considers
-    itself compliant, or knows how to wrap itself suitably.
-
-This is handled with ``__conform__``. If an object implements
-``__conform__``, then it will be used to give the object the chance to
-decide if it knows about the interface. This is true even if the class
-declares that it implements the interface.
-
-.. doctest::
-
-  >>> @zope.interface.implementer(ICartesianPoint)
-  ... class C(object):
-  ...     def __conform__(self, proto):
-  ...          return "This could be anything."
-
-  >>> ICartesianPoint(C())
-  'This could be anything.'
-
-If ``__conform__`` returns ``None`` (because the object is unaware of
-the interface), then the rest of the adaptation process will continue.
-Here, we demonstrate that if the object already provides the
-interface, it is returned.
-
-.. doctest::
-
-  >>> @zope.interface.implementer(ICartesianPoint)
-  ... class C(object):
-  ...     def __conform__(self, proto):
-  ...          return None
-
-  >>> c = C()
-  >>> ICartesianPoint(c) is c
-  True
-
-
-Adapter hooks (see :ref:`adapt_adapter_hooks`) will also be used, if present (after
-a ``__conform__`` method, if any, has been tried):
-
-.. doctest::
-
-  >>> from zope.interface.interface import adapter_hooks
-  >>> def adapt_tuple_to_point(iface, obj):
-  ...     if isinstance(obj, tuple) and len(obj) == 2:
-  ...         return CartesianPoint(*obj)
-
-  >>> adapter_hooks.append(adapt_tuple_to_point)
-  >>> ICartesianPoint((1, 1))
-  CartesianPoint(1, 1)
-
-  >>> adapter_hooks.remove(adapt_tuple_to_point)
-  >>> ICartesianPoint((1, 1))
-  Traceback (most recent call last):
-  ...
-  TypeError: ('Could not adapt', (1, 1), <InterfaceClass builtins.ICartesianPoint>)
-
-.. _adapt_adapter_hooks:
-
-``__adapt__`` and adapter hooks
--------------------------------
-
-Interfaces implement the :pep:`246` ``__adapt__`` method to satisfy
-the requirement:
-
-    When the [interface] knows about the object, and either the object
-    already complies or the [interface] knows how to suitably wrap the
-    object.
-
-This method is normally not called directly. It is called by the
-:pep:`246` adapt framework and by the interface ``__call__`` operator
-once ``__conform__`` (if any) has failed.
-
-The ``__adapt__`` method is responsible for adapting an object to the
-receiver.
-
-The default version returns ``None`` (because by default no interface
-"knows how to suitably wrap the object"):
-
-.. doctest::
-
-  >>> ICartesianPoint.__adapt__(0)
-
-unless the object given provides the interface ("the object already complies"):
-
-.. doctest::
-
-  >>> @zope.interface.implementer(ICartesianPoint)
-  ... class C(object):
-  ...     pass
-
-  >>> obj = C()
-  >>> ICartesianPoint.__adapt__(obj) is obj
-  True
-
-.. rubric:: Customizing ``__adapt__`` in an interface
-
-It is possible to replace or customize the ``__adapt___``
-functionality for particular interfaces, if that interface "knows how
-to suitably wrap [an] object". This method should return the adapted
-object if it knows how, or call the super class to continue with the
-default adaptation process.
-
-.. doctest::
-
-   >>> import math
-   >>> class IPolarPoint(zope.interface.Interface):
-   ...     r = zope.interface.Attribute("Distance from center.")
-   ...     theta = zope.interface.Attribute("Angle from horizontal.")
-   ...     @zope.interface.interfacemethod
-   ...     def __adapt__(self, obj):
-   ...          if ICartesianPoint.providedBy(obj):
-   ...              # Convert to polar coordinates.
-   ...              r = math.sqrt(obj.x ** 2 + obj.y ** 2)
-   ...              theta = math.acos(obj.x / r)
-   ...              theta = math.degrees(theta)
-   ...              return PolarPoint(r, theta)
-   ...          return super(type(IPolarPoint), self).__adapt__(obj)
-
-   >>> @zope.interface.implementer(IPolarPoint)
-   ... class PolarPoint(object):
-   ...     def __init__(self, r=0, theta=0):
-   ...        self.r = r; self.theta = theta
-   ...     def __repr__(self):
-   ...        return "PolarPoint(%s, %s)" % (self.r, self.theta)
-   >>> IPolarPoint(CartesianPoint(0, 1))
-   PolarPoint(1.0, 90.0)
-   >>> IPolarPoint(PolarPoint())
-   PolarPoint(0, 0)
-
-.. seealso:: :func:`zope.interface.interfacemethod`, which explains
-   how to override functions in interface definitions and why, prior
-   to Python 3.6, the zero-argument version of `super` cannot be used.
-
-.. rubric:: Using adapter hooks for loose coupling
-
-Commonly, the author of the interface doesn't know how to wrap all
-possible objects, and neither does the author of an object know how to
-``__conform__`` to all possible interfaces. To support decoupling
-interfaces and objects, interfaces support the concept of "adapter
-hooks." Adapter hooks are a global sequence of callables
-``hook(interface, object)`` that are called, in order, from the
-default ``__adapt__`` method until one returns a non-``None`` result.
-
-.. note::
-   In many applications, a :doc:`adapter` is installed as
-   the first or only adapter hook.
-
-We'll install a hook that adapts from a 2D ``(x, y)`` Cartesian point
-on a plane to a three-dimensional point ``(x, y, z)`` by assuming the
-``z`` coordinate is 0. First, we'll define this new interface and an
-implementation:
-
-.. doctest::
-
-  >>> class ICartesianPoint3D(ICartesianPoint):
-  ...      z = zope.interface.Attribute("Depth.")
-  >>> @zope.interface.implementer(ICartesianPoint3D)
-  ... class CartesianPoint3D(CartesianPoint):
-  ...     def __init__(self, x=0, y=0, z=0):
-  ...        CartesianPoint.__init__(self, x, y)
-  ...        self.z = 0
-  ...     def __repr__(self):
-  ...        return "CartesianPoint3D(%s, %s, %s)" % (self.x, self.y, self.z)
-
-
-We install a hook by simply adding it to the ``adapter_hooks`` list:
-
-.. doctest::
-
-  >>> from zope.interface.interface import adapter_hooks
-  >>> def returns_none(iface, obj):
-  ...     print("(First adapter hook returning None.)")
-  >>> def adapt_2d_to_3d(iface, obj):
-  ...     if iface == ICartesianPoint3D and ICartesianPoint.providedBy(obj):
-  ...         return CartesianPoint3D(obj.x, obj.y, 0)
-  >>> adapter_hooks.append(returns_none)
-  >>> adapter_hooks.append(adapt_2d_to_3d)
-  >>> ICartesianPoint3D.__adapt__(CartesianPoint())
-  (First adapter hook returning None.)
-  CartesianPoint3D(0, 0, 0)
-  >>> ICartesianPoint3D(CartesianPoint())
-  (First adapter hook returning None.)
-  CartesianPoint3D(0, 0, 0)
-
-Hooks can be uninstalled by removing them from the list:
-
-.. doctest::
-
-  >>> adapter_hooks.remove(returns_none)
-  >>> adapter_hooks.remove(adapt_2d_to_3d)
-  >>> ICartesianPoint3D.__adapt__(CartesianPoint())
-
-.. _global_persistence:
-
-Persistence, Sorting, Equality and Hashing
-==========================================
-
-.. tip:: For the practical implications of what's discussed below, and
-         some potential problems, see :ref:`spec_eq_hash`.
-
-Just like Python classes, interfaces are designed to inexpensively
-support persistence using Python's standard :mod:`pickle` module. This
-means that one process can send a *reference* to an interface to another
-process in the form of a byte string, and that other process can load
-that byte string and get the object that is that interface. The processes
-may be separated in time (one after the other), in space (running on
-different machines) or even be parts of the same process communicating
-with itself.
-
-We can demonstrate this. Observe how small the byte string needed to
-capture the reference is. Also note that since this is the same
-process, the identical object is found and returned:
-
-.. doctest::
-
-   >>> import sys
-   >>> import pickle
-   >>> class Foo(object):
-   ...    pass
-   >>> sys.modules[__name__].Foo = Foo # XXX, see below
-   >>> pickled_byte_string = pickle.dumps(Foo, 0)
-   >>> len(pickled_byte_string)
-   21
-   >>> imported = pickle.loads(pickled_byte_string)
-   >>> imported == Foo
-   True
-   >>> imported is Foo
-   True
-   >>> class IFoo(zope.interface.Interface):
-   ...     pass
-   >>> sys.modules[__name__].IFoo = IFoo # XXX, see below
-   >>> pickled_byte_string = pickle.dumps(IFoo, 0)
-   >>> len(pickled_byte_string)
-   22
-   >>> imported = pickle.loads(pickled_byte_string)
-   >>> imported is IFoo
-   True
-   >>> imported == IFoo
-   True
-
-.. rubric:: References to Global Objects
-
-The eagle-eyed reader will have noticed the two funny lines like
-``sys.modules[__name__].Foo = Foo``. What's that for? To understand,
-we must know a bit about how Python "pickles" (``pickle.dump`` or
-``pickle.dumps``) classes or interfaces.
-
-When Python pickles a class or an interface, it does so as a "global
-object" [#global_object]_. Global objects are expected to already
-exist (contrast this with pickling a string or an object instance,
-which creates a new object in the receiving process) with all their
-necessary state information (for classes and interfaces, the state
-information would be things like the list of methods and defined
-attributes) in the receiving process, so the pickled byte string needs
-only contain enough data to look up that existing object; this data is a
-*reference*. Not only does this minimize the amount of data required
-to persist such an object, it also facilitates changing the definition
-of the object over time: if a class or interface gains or loses
-methods or attributes, loading a previously pickled reference will use
-the *current definition* of the object.
-
-The *reference* to a global object that's stored in the byte string
-consists only of the object's ``__name__`` and ``__module__``. Before
-a global object *obj* is pickled, Python makes sure that the object being
-pickled is the same one that can be found at
-``getattr(sys.modules[obj.__module__], obj.__name__)``; if there is no
-such object, or it refers to a different object, pickling fails. The
-two funny lines make sure that holds, no matter how this example is
-run (using some doctest runners, it doesn't hold by default, unlike it
-normally would).
-
-We can show some examples of what happens when that condition doesn't
-hold. First, what if we change the global object and try to pickle the
-old one?
-
-.. doctest::
-
-   >>> sys.modules[__name__].Foo = 42
-   >>> pickle.dumps(Foo)
-   Traceback (most recent call last):
-   ...
-   _pickle.PicklingError: Can't pickle <class 'Foo'>: it's not the same object as builtins.Foo
-
-A consequence of this is that only one object of the given name can be
-defined and pickled at a time. If we were to try to define a new ``Foo``
-class (remembering that normally the ``sys.modules[__name__].Foo =``
-line is automatic), we still cannot pickle the old one:
-
-.. doctest::
-
-   >>> orig_Foo = Foo
-   >>> class Foo(object):
-   ...    pass
-   >>> sys.modules[__name__].Foo = Foo # XXX, usually automatic
-   >>> pickle.dumps(orig_Foo)
-   Traceback (most recent call last):
-   ...
-   _pickle.PicklingError: Can't pickle <class 'Foo'>: it's not the same object as builtins.Foo
-
-Or what if there simply is no global object?
-
-.. doctest::
-
-   >>> del sys.modules[__name__].Foo
-   >>> pickle.dumps(Foo)
-   Traceback (most recent call last):
-   ...
-   _pickle.PicklingError: Can't pickle <class 'Foo'>: attribute lookup Foo on builtins failed
-
-Interfaces and classes behave the same in all those ways.
-
-.. rubric:: What's This Have To Do With Sorting, Equality and Hashing?
-
-Another important design consideration for interfaces is that they
-should be sortable. This permits them to be used, for example, as keys
-in a (persistent) `BTree <https://btrees.readthedocs.io>`_. As such,
-they define a total ordering, meaning that any given interface can
-definitively said to be greater than, less than, or equal to, any
-other interface. This relationship must be *stable* and hold the same
-across any two processes.
-
-An object becomes sortable by overriding the equality method
-``__eq__`` and at least one of the comparison methods (such as
-``__lt__``).
-
-Classes, on the other hand, are not sortable [#class_sort]_.
-Classes can only be tested for equality, and they implement this using
-object identity: ``class_a == class_b`` is equivalent to ``class_a is class_b``.
-
-In addition to being sortable, it's important for interfaces to be
-hashable so they can be used as keys in dictionaries or members of
-sets. This is done by implementing the ``__hash__`` method [#hashable]_.
-
-Classes are hashable, and they also implement this based on object
-identity, with the equivalent of ``id(class_a)``.
-
-To be both hashable and sortable, the hash method and the equality and
-comparison methods **must** `be consistent with each other
-<https://docs.python.org/3/reference/datamodel.html#object.__hash__>`_.
-That is, they must all be based on the same principle.
-
-Classes use the principle of identity to implement equality and
-hashing, but they don't implement sorting because identity isn't a
-stable sorting method (it is different in every process).
-
-Interfaces need to be sortable. In order for all three of hashing,
-equality and sorting to be consistent, interfaces implement them using
-the same principle as persistence. Interfaces are treated like "global
-objects" and sort and hash using the same information a *reference* to
-them would: their ``__name__`` and ``__module__``.
-
-In this way, hashing, equality and sorting are consistent with each
-other, and consistent with pickling:
-
-.. doctest::
-
-   >>> class IFoo(zope.interface.Interface):
-   ...     pass
-   >>> sys.modules[__name__].IFoo = IFoo # XXX, usually automatic
-   >>> f1 = IFoo
-   >>> pickled_f1 = pickle.dumps(f1)
-   >>> class IFoo(zope.interface.Interface):
-   ...     pass
-   >>> sys.modules[__name__].IFoo = IFoo # XXX, usually automatic
-   >>> IFoo == f1
-   True
-   >>> unpickled_f1 = pickle.loads(pickled_f1)
-   >>> unpickled_f1 == IFoo == f1
-   True
-
-This isn't quite the case for classes; note how ``f1`` wasn't equal to
-``Foo`` before pickling, but the unpickled value is:
-
-.. doctest::
-
-   >>> class Foo(object):
-   ...     pass
-   >>> sys.modules[__name__].Foo = Foo # XXX, usually automatic
-   >>> f1 = Foo
-   >>> pickled_f1 = pickle.dumps(Foo)
-   >>> class Foo(object):
-   ...     pass
-   >>> sys.modules[__name__].Foo = Foo # XXX, usually automatic
-   >>> f1 == Foo
-   False
-   >>> unpickled_f1 = pickle.loads(pickled_f1)
-   >>> unpickled_f1 == Foo # Surprise!
-   True
-   >>> unpickled_f1 == f1
-   False
-
-For more information, and some rare potential pitfalls, see
-:ref:`spec_eq_hash`.
-
-.. rubric:: Footnotes
-
-.. [#create] The main reason we subclass ``Interface`` is to cause the
-             Python class statement to create an interface, rather
-             than a class.
-
-             It's possible to create interfaces by calling a special
-             interface class directly.  Doing this, it's possible
-             (and, on rare occasions, useful) to create interfaces
-             that don't descend from ``Interface``.  Using this
-             technique is beyond the scope of this document.
-
-.. [#factory] Classes are factories.  They can be called to create
-              their instances.  We expect that we will eventually
-              extend the concept of implementation to other kinds of
-              factories, so that we can declare the interfaces
-              provided by the objects created.
-
-.. [#compat] The goal is substitutability.  An object that provides an
-             extending interface should be substitutable for an object
-             that provides the extended interface.  In our example, an
-             object that provides ``IBaz`` should be usable wherever an
-             object that provides ``IBlat`` is expected.
-
-             The interface implementation doesn't enforce this,
-             but maybe it should do some checks.
-
-.. [#class_sort] In Python 2, classes could be sorted, but the sort
-                 was not stable (it also used the identity principle)
-                 and not useful for persistence; this was considered a
-                 bug that was fixed in Python 3.
-
-.. [#hashable] In order to be hashable, you must implement both
-               ``__eq__``  and ``__hash__``. If you only implement
-               ``__eq__``, Python makes sure the type cannot be
-               used in a dictionary, set, or with :func:`hash`. In
-               Python 2, this wasn't the case, and forgetting to
-               override ``__hash__`` was a constant source of bugs.
-
-.. [#global_object] From the name of the pickle bytecode operator; it
-                    varies depending on the protocol but always
-                    includes "GLOBAL".
+objectSpecificationDescriptor = ObjectSpecificationDescriptor()
```

### Comparing `zope_interface-6.4/docs/_build/html/_sources/adapter.rst.txt` & `zope.interface-6.4.post0/docs/adapter.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/adapter.ru.rst.txt` & `zope.interface-6.4.post0/docs/adapter.ru.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/api/adapters.rst.txt` & `zope.interface-6.4.post0/docs/api/adapters.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/api/common.rst.txt` & `zope.interface-6.4.post0/docs/api/common.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/api/components.rst.txt` & `zope.interface-6.4.post0/docs/api/components.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/api/declarations.rst.txt` & `zope.interface-6.4.post0/docs/api/declarations.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/api/ro.rst.txt` & `zope.interface-6.4.post0/docs/api/ro.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/api/specifications.rst.txt` & `zope.interface-6.4.post0/docs/api/specifications.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/foodforthought.rst.txt` & `zope.interface-6.4.post0/docs/foodforthought.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/hacking.rst.txt` & `zope.interface-6.4.post0/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/human.rst.txt` & `zope.interface-6.4.post0/docs/human.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/human.ru.rst.txt` & `zope.interface-6.4.post0/docs/human.ru.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/index.rst.txt` & `zope.interface-6.4.post0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/_build/html/_sources/verify.rst.txt` & `zope.interface-6.4.post0/docs/verify.rst`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/conf.py` & `zope.interface-6.4.post0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/docs/make.bat` & `zope.interface-6.4.post0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/setup.cfg` & `zope.interface-6.4.post0/setup.cfg`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/setup.py` & `zope.interface-6.4.post0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 long_description = (
         read('README.rst')
         + '\n' +
         read('CHANGES.rst')
         )
 
 setup(name='zope.interface',
-      version='6.4',
+      version='6.4.post0',
       url='https://github.com/zopefoundation/zope.interface',
       license='ZPL 2.1',
       description='Interfaces for Python',
       author='Zope Foundation and Contributors',
       author_email='zope-dev@zope.org',
       long_description=long_description,
       classifiers=[
```

### Comparing `zope_interface-6.4/src/zope/interface/__init__.py` & `zope.interface-6.4.post0/src/zope/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/_compat.py` & `zope.interface-6.4.post0/src/zope/interface/_compat.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/_flatten.py` & `zope.interface-6.4.post0/src/zope/interface/_flatten.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/_zope_interface_coptimizations.c` & `zope.interface-6.4.post0/src/zope/interface/_zope_interface_coptimizations.c`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/adapter.py` & `zope.interface-6.4.post0/src/zope/interface/adapter.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/advice.py` & `zope.interface-6.4.post0/src/zope/interface/advice.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/__init__.py` & `zope.interface-6.4.post0/src/zope/interface/common/__init__.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/builtins.py` & `zope.interface-6.4.post0/src/zope/interface/common/builtins.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/collections.py` & `zope.interface-6.4.post0/src/zope/interface/common/collections.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/idatetime.py` & `zope.interface-6.4.post0/src/zope/interface/common/idatetime.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/interfaces.py` & `zope.interface-6.4.post0/src/zope/interface/common/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/io.py` & `zope.interface-6.4.post0/src/zope/interface/common/io.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/mapping.py` & `zope.interface-6.4.post0/src/zope/interface/common/mapping.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/numbers.py` & `zope.interface-6.4.post0/src/zope/interface/common/numbers.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/sequence.py` & `zope.interface-6.4.post0/src/zope/interface/common/sequence.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/tests/__init__.py` & `zope.interface-6.4.post0/src/zope/interface/common/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/tests/basemapping.py` & `zope.interface-6.4.post0/src/zope/interface/common/tests/basemapping.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/tests/test_builtins.py` & `zope.interface-6.4.post0/src/zope/interface/common/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/tests/test_collections.py` & `zope.interface-6.4.post0/src/zope/interface/common/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/tests/test_idatetime.py` & `zope.interface-6.4.post0/src/zope/interface/common/tests/test_idatetime.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/tests/test_import_interfaces.py` & `zope.interface-6.4.post0/src/zope/interface/common/tests/test_import_interfaces.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/tests/test_io.py` & `zope.interface-6.4.post0/src/zope/interface/common/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/common/tests/test_numbers.py` & `zope.interface-6.4.post0/src/zope/interface/common/tests/test_numbers.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/declarations.py` & `zope.interface-6.4.post0/src/zope/interface/interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1189 +1,1148 @@
 ##############################################################################
-# Copyright (c) 2003 Zope Foundation and Contributors.
+#
+# Copyright (c) 2001, 2002 Zope Foundation and Contributors.
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
+#
 ##############################################################################
-"""Implementation of interface declarations
-
-There are three flavors of declarations:
-
-  - Declarations are used to simply name declared interfaces.
-
-  - ImplementsDeclarations are used to express the interfaces that a
-    class implements (that instances of the class provides).
-
-    Implements specifications support inheriting interfaces.
-
-  - ProvidesDeclarations are used to express interfaces directly
-    provided by objects.
-
+"""Interface object implementation
 """
-__docformat__ = 'restructuredtext'
-
+# pylint:disable=protected-access
 import sys
 import weakref
 from types import FunctionType
 from types import MethodType
-from types import ModuleType
+from typing import Union
 
+from zope.interface import ro
 from zope.interface._compat import _use_c_impl
-from zope.interface.interface import Interface
-from zope.interface.interface import InterfaceClass
-from zope.interface.interface import NameAndModuleComparisonMixin
-from zope.interface.interface import Specification
-from zope.interface.interface import SpecificationBase
+from zope.interface.exceptions import Invalid
+from zope.interface.ro import ro as calculate_ro
 
 
 __all__ = [
-    # None. The public APIs of this module are
-    # re-exported from zope.interface directly.
+    # Most of the public API from this module is directly exported
+    # from zope.interface. The only remaining public API intended to
+    # be imported from here should be those few things documented as
+    # such.
+    'InterfaceClass',
+    'Specification',
+    'adapter_hooks',
 ]
 
-# pylint:disable=too-many-lines
+CO_VARARGS = 4
+CO_VARKEYWORDS = 8
+# Put in the attrs dict of an interface by ``taggedValue`` and ``invariants``
+TAGGED_DATA = '__interface_tagged_values__'
+# Put in the attrs dict of an interface by ``interfacemethod``
+INTERFACE_METHODS = '__interface_methods__'
 
-# Registry of class-implementation specifications
-BuiltinImplementationSpecifications = {}
+_decorator_non_return = object()
+_marker = object()
 
 
-def _next_super_class(ob):
-    # When ``ob`` is an instance of ``super``, return
-    # the next class in the MRO that we should actually be
-    # looking at. Watch out for diamond inheritance!
-    self_class = ob.__self_class__
-    class_that_invoked_super = ob.__thisclass__
-    complete_mro = self_class.__mro__
-    next_class = complete_mro[complete_mro.index(class_that_invoked_super) + 1]
-    return next_class
 
-class named:
+def invariant(call):
+    f_locals = sys._getframe(1).f_locals
+    tags = f_locals.setdefault(TAGGED_DATA, {})
+    invariants = tags.setdefault('invariants', [])
+    invariants.append(call)
+    return _decorator_non_return
 
-    def __init__(self, name):
-        self.name = name
 
-    def __call__(self, ob):
-        ob.__component_name__ = self.name
-        return ob
+def taggedValue(key, value):
+    """Attaches a tagged value to an interface at definition time."""
+    f_locals = sys._getframe(1).f_locals
+    tagged_values = f_locals.setdefault(TAGGED_DATA, {})
+    tagged_values[key] = value
+    return _decorator_non_return
 
 
-class Declaration(Specification):
-    """Interface declarations"""
+class Element:
+    """
+    Default implementation of `zope.interface.interfaces.IElement`.
+    """
 
-    __slots__ = ()
+    # We can't say this yet because we don't have enough
+    # infrastructure in place.
+    #
+    #implements(IElement)
 
-    def __init__(self, *bases):
-        Specification.__init__(self, _normalizeargs(bases))
+    def __init__(self, __name__, __doc__=''): # pylint:disable=redefined-builtin
+        if not __doc__ and __name__.find(' ') >= 0:
+            __doc__ = __name__
+            __name__ = None
 
-    def __contains__(self, interface):
-        """Test whether an interface is in the specification
-        """
+        self.__name__ = __name__
+        self.__doc__ = __doc__
+        # Tagged values are rare, especially on methods or attributes.
+        # Deferring the allocation can save substantial memory.
+        self.__tagged_values = None
 
-        return self.extends(interface) and interface in self.interfaces()
+    def getName(self):
+        """ Returns the name of the object. """
+        return self.__name__
 
-    def __iter__(self):
-        """Return an iterator for the interfaces in the specification
-        """
-        return self.interfaces()
+    def getDoc(self):
+        """ Returns the documentation for the object. """
+        return self.__doc__
 
-    def flattened(self):
-        """Return an iterator of all included and extended interfaces
-        """
-        return iter(self.__iro__)
+    ###
+    # Tagged values.
+    #
+    # Direct tagged values are set only in this instance. Others
+    # may be inherited (for those subclasses that have that concept).
+    ###
 
-    def __sub__(self, other):
-        """Remove interfaces from a specification
-        """
-        return Declaration(*[
-            i for i in self.interfaces()
-            if not [
-                j
-                for j in other.interfaces()
-                if i.extends(j, 0) # non-strict extends
-            ]
-        ])
+    def getTaggedValue(self, tag):
+        """ Returns the value associated with 'tag'. """
+        if not self.__tagged_values:
+            raise KeyError(tag)
+        return self.__tagged_values[tag]
 
-    def __add__(self, other):
-        """
-        Add two specifications or a specification and an interface
-        and produce a new declaration.
+    def queryTaggedValue(self, tag, default=None):
+        """ Returns the value associated with 'tag'. """
+        return self.__tagged_values.get(tag, default) if self.__tagged_values else default
 
-        .. versionchanged:: 5.4.0
-           Now tries to preserve a consistent resolution order. Interfaces
-           being added to this object are added to the front of the resulting resolution
-           order if they already extend an interface in this object. Previously,
-           they were always added to the end of the order, which easily resulted in
-           invalid orders.
-        """
-        before = []
-        result = list(self.interfaces())
-        seen = set(result)
-        for i in other.interfaces():
-            if i in seen:
-                continue
-            seen.add(i)
-            if any(i.extends(x) for x in result):
-                # It already extends us, e.g., is a subclass,
-                # so it needs to go at the front of the RO.
-                before.append(i)
-            else:
-                result.append(i)
-        return Declaration(*(before + result))
+    def getTaggedValueTags(self):
+        """ Returns a collection of all tags. """
+        return self.__tagged_values.keys() if self.__tagged_values else ()
 
-    # XXX: Is __radd__ needed? No tests break if it's removed.
-    # If it is needed, does it need to handle the C3 ordering differently?
-    # I (JAM) don't *think* it does.
-    __radd__ = __add__
-
-    @staticmethod
-    def _add_interfaces_to_cls(interfaces, cls):
-        # Strip redundant interfaces already provided
-        # by the cls so we don't produce invalid
-        # resolution orders.
-        implemented_by_cls = implementedBy(cls)
-        interfaces = tuple([
-            iface
-            for iface in interfaces
-            if not implemented_by_cls.isOrExtends(iface)
-        ])
-        return interfaces + (implemented_by_cls,)
-
-    @staticmethod
-    def _argument_names_for_repr(interfaces):
-        # These don't actually have to be interfaces, they could be other
-        # Specification objects like Implements. Also, the first
-        # one is typically/nominally the cls.
-        ordered_names = []
-        names = set()
-        for iface in interfaces:
-            duplicate_transform = repr
-            if isinstance(iface, InterfaceClass):
-                # Special case to get 'foo.bar.IFace'
-                # instead of '<InterfaceClass foo.bar.IFace>'
-                this_name = iface.__name__
-                duplicate_transform = str
-            elif isinstance(iface, type):
-                # Likewise for types. (Ignoring legacy old-style
-                # classes.)
-                this_name = iface.__name__
-                duplicate_transform = _implements_name
-            elif (isinstance(iface, Implements)
-                  and not iface.declared
-                  and iface.inherit in interfaces):
-                # If nothing is declared, there's no need to even print this;
-                # it would just show as ``classImplements(Class)``, and the
-                # ``Class`` has typically already.
-                continue
-            else:
-                this_name = repr(iface)
+    def setTaggedValue(self, tag, value):
+        """ Associates 'value' with 'key'. """
+        if self.__tagged_values is None:
+            self.__tagged_values = {}
+        self.__tagged_values[tag] = value
 
-            already_seen = this_name in names
-            names.add(this_name)
-            if already_seen:
-                this_name = duplicate_transform(iface)
-
-            ordered_names.append(this_name)
-        return ', '.join(ordered_names)
-
-
-class _ImmutableDeclaration(Declaration):
-    # A Declaration that is immutable. Used as a singleton to
-    # return empty answers for things like ``implementedBy``.
-    # We have to define the actual singleton after normalizeargs
-    # is defined, and that in turn is defined after InterfaceClass and
-    # Implements.
+    queryDirectTaggedValue = queryTaggedValue
+    getDirectTaggedValue = getTaggedValue
+    getDirectTaggedValueTags = getTaggedValueTags
 
-    __slots__ = ()
 
-    __instance = None
+SpecificationBasePy = object # filled by _use_c_impl.
 
-    def __new__(cls):
-        if _ImmutableDeclaration.__instance is None:
-            _ImmutableDeclaration.__instance = object.__new__(cls)
-        return _ImmutableDeclaration.__instance
 
-    def __reduce__(self):
-        return "_empty"
+@_use_c_impl
+class SpecificationBase:
+    # This object is the base of the inheritance hierarchy for ClassProvides:
+    #
+    # ClassProvides < ClassProvidesBase, Declaration
+    # Declaration < Specification < SpecificationBase
+    # ClassProvidesBase < SpecificationBase
+    #
+    # In order to have compatible instance layouts, we need to declare
+    # the storage used by Specification and Declaration here (and
+    # those classes must have ``__slots__ = ()``); fortunately this is
+    # not a waste of space because those are the only two inheritance
+    # trees. These all translate into tp_members in C.
+    __slots__ = (
+        # Things used here.
+        '_implied',
+        # Things used in Specification.
+        '_dependents',
+        '_bases',
+        '_v_attrs',
+        '__iro__',
+        '__sro__',
+        '__weakref__',
+    )
 
-    @property
-    def __bases__(self):
-        return ()
+    def providedBy(self, ob):
+        """Is the interface implemented by an object
+        """
+        spec = providedBy(ob)
+        return self in spec._implied
 
-    @__bases__.setter
-    def __bases__(self, new_bases):
-        # We expect the superclass constructor to set ``self.__bases__ = ()``.
-        # Rather than attempt to special case that in the constructor and allow
-        # setting __bases__ only at that time, it's easier to just allow setting
-        # the empty tuple at any time. That makes ``x.__bases__ = x.__bases__`` a nice
-        # no-op too. (Skipping the superclass constructor altogether is a recipe
-        # for maintenance headaches.)
-        if new_bases != ():
-            raise TypeError("Cannot set non-empty bases on shared empty Declaration.")
-
-    # As the immutable empty declaration, we cannot be changed.
-    # This means there's no logical reason for us to have dependents
-    # or subscriptions: we'll never notify them. So there's no need for
-    # us to keep track of any of that.
-    @property
-    def dependents(self):
-        return {}
+    def implementedBy(self, cls):
+        """Test whether the specification is implemented by a class or factory.
 
-    changed = subscribe = unsubscribe = lambda self, _ignored: None
+        Raise TypeError if argument is neither a class nor a callable.
+        """
+        spec = implementedBy(cls)
+        return self in spec._implied
 
-    def interfaces(self):
-        # An empty iterator
-        return iter(())
+    def isOrExtends(self, interface):
+        """Is the interface the same as or extend the given interface
+        """
+        return interface in self._implied # pylint:disable=no-member
 
-    def extends(self, interface, strict=True):
-        return interface is self._ROOT
+    __call__ = isOrExtends
 
-    def get(self, name, default=None):
-        return default
 
-    def weakref(self, callback=None):
-        # We're a singleton, we never go away. So there's no need to return
-        # distinct weakref objects here; their callbacks will never
-        # be called. Instead, we only need to return a callable that
-        # returns ourself. The easiest one is to return _ImmutableDeclaration
-        # itself; testing on Python 3.8 shows that's faster than a function that
-        # returns _empty. (Remember, one goal is to avoid allocating any
-        # object, and that includes a method.)
-        return _ImmutableDeclaration
+class NameAndModuleComparisonMixin:
+    # Internal use. Implement the basic sorting operators (but not (in)equality
+    # or hashing). Subclasses must provide ``__name__`` and ``__module__``
+    # attributes. Subclasses will be mutually comparable; but because equality
+    # and hashing semantics are missing from this class, take care in how
+    # you define those two attributes: If you stick with the default equality
+    # and hashing (identity based) you should make sure that all possible ``__name__``
+    # and ``__module__`` pairs are unique ACROSS ALL SUBCLASSES. (Actually, pretty
+    # much the same thing goes if you define equality and hashing to be based on
+    # those two attributes: they must still be consistent ACROSS ALL SUBCLASSES.)
 
-    @property
-    def _v_attrs(self):
-        # _v_attrs is not a public, documented property, but some client code
-        # uses it anyway as a convenient place to cache things. To keep the
-        # empty declaration truly immutable, we must ignore that. That includes
-        # ignoring assignments as well.
-        return {}
-
-    @_v_attrs.setter
-    def _v_attrs(self, new_attrs):
-        pass
+    # pylint:disable=assigning-non-slot
+    __slots__ = ()
 
+    def _compare(self, other):
+        """
+        Compare *self* to *other* based on ``__name__`` and ``__module__``.
 
-##############################################################################
-#
-# Implementation specifications
-#
-# These specify interfaces implemented by instances of classes
+        Return 0 if they are equal, return 1 if *self* is
+        greater than *other*, and return -1 if *self* is less than
+        *other*.
+
+        If *other* does not have ``__name__`` or ``__module__``, then
+        return ``NotImplemented``.
+
+        .. caution::
+           This allows comparison to things well outside the type hierarchy,
+           perhaps not symmetrically.
+
+           For example, ``class Foo(object)`` and ``class Foo(Interface)``
+           in the same file would compare equal, depending on the order of
+           operands. Writing code like this by hand would be unusual, but it could
+           happen with dynamic creation of types and interfaces.
+
+        None is treated as a pseudo interface that implies the loosest
+        contact possible, no contract. For that reason, all interfaces
+        sort before None.
+        """
+        if other is self:
+            return 0
 
-class Implements(NameAndModuleComparisonMixin,
-                 Declaration):
-    # Inherit from NameAndModuleComparisonMixin to be
-    # mutually comparable with InterfaceClass objects.
-    # (The two must be mutually comparable to be able to work in e.g., BTrees.)
-    # Instances of this class generally don't have a __module__ other than
-    # `zope.interface.declarations`, whereas they *do* have a __name__ that is the
-    # fully qualified name of the object they are representing.
-
-    # Note, though, that equality and hashing are still identity based. This
-    # accounts for things like nested objects that have the same name (typically
-    # only in tests) and is consistent with pickling. As far as comparisons to InterfaceClass
-    # goes, we'll never have equal name and module to those, so we're still consistent there.
-    # Instances of this class are essentially intended to be unique and are
-    # heavily cached (note how our __reduce__ handles this) so having identity
-    # based hash and eq should also work.
-
-    # We want equality and hashing to be based on identity. However, we can't actually
-    # implement __eq__/__ne__ to do this because sometimes we get wrapped in a proxy.
-    # We need to let the proxy types implement these methods so they can handle unwrapping
-    # and then rely on: (1) the interpreter automatically changing `implements == proxy` into
-    # `proxy == implements` (which will call proxy.__eq__ to do the unwrapping) and then
-    # (2) the default equality and hashing semantics being identity based.
-
-    # class whose specification should be used as additional base
-    inherit = None
-
-    # interfaces actually declared for a class
-    declared = ()
-
-    # Weak cache of {class: <implements>} for super objects.
-    # Created on demand. These are rare, as of 5.0 anyway. Using a class
-    # level default doesn't take space in instances. Using _v_attrs would be
-    # another place to store this without taking space unless needed.
-    _super_cache = None
-
-    __name__ = '?'
-
-    @classmethod
-    def named(cls, name, *bases):
-        # Implementation method: Produce an Implements interface with
-        # a fully fleshed out __name__ before calling the constructor, which
-        # sets bases to the given interfaces and which may pass this object to
-        # other objects (e.g., to adjust dependents). If they're sorting or comparing
-        # by name, this needs to be set.
-        inst = cls.__new__(cls)
-        inst.__name__ = name
-        inst.__init__(*bases)
-        return inst
+        if other is None:
+            return -1
 
-    def changed(self, originally_changed):
+        n1 = (self.__name__, self.__module__)
         try:
-            del self._super_cache
+            n2 = (other.__name__, other.__module__)
         except AttributeError:
-            pass
-        return super().changed(originally_changed)
+            return NotImplemented
 
-    def __repr__(self):
-        if self.inherit:
-            name = getattr(self.inherit, '__name__', None) or _implements_name(self.inherit)
-        else:
-            name = self.__name__
-        declared_names = self._argument_names_for_repr(self.declared)
-        if declared_names:
-            declared_names = ', ' + declared_names
-        return 'classImplements({}{})'.format(name, declared_names)
+        # This spelling works under Python3, which doesn't have cmp().
+        return (n1 > n2) - (n1 < n2)
+
+    def __lt__(self, other):
+        c = self._compare(other)
+        if c is NotImplemented:
+            return c
+        return c < 0
+
+    def __le__(self, other):
+        c = self._compare(other)
+        if c is NotImplemented:
+            return c
+        return c <= 0
+
+    def __gt__(self, other):
+        c = self._compare(other)
+        if c is NotImplemented:
+            return c
+        return c > 0
+
+    def __ge__(self, other):
+        c = self._compare(other)
+        if c is NotImplemented:
+            return c
+        return c >= 0
 
-    def __reduce__(self):
-        return implementedBy, (self.inherit, )
 
+@_use_c_impl
+class InterfaceBase(NameAndModuleComparisonMixin, SpecificationBasePy):
+    """Base class that wants to be replaced with a C base :)
+    """
 
-def _implements_name(ob):
-    # Return the __name__ attribute to be used by its __implemented__
-    # property.
-    # This must be stable for the "same" object across processes
-    # because it is used for sorting. It needn't be unique, though, in cases
-    # like nested classes named Foo created by different functions, because
-    # equality and hashing is still based on identity.
-    # It might be nice to use __qualname__ on Python 3, but that would produce
-    # different values between Py2 and Py3.
-    return (getattr(ob, '__module__', '?') or '?') + \
-        '.' + (getattr(ob, '__name__', '?') or '?')
-
-
-def _implementedBy_super(sup):
-    # TODO: This is now simple enough we could probably implement
-    # in C if needed.
-
-    # If the class MRO is strictly linear, we could just
-    # follow the normal algorithm for the next class in the
-    # search order (e.g., just return
-    # ``implemented_by_next``). But when diamond inheritance
-    # or mixins + interface declarations are present, we have
-    # to consider the whole MRO and compute a new Implements
-    # that excludes the classes being skipped over but
-    # includes everything else.
-    implemented_by_self = implementedBy(sup.__self_class__)
-    cache = implemented_by_self._super_cache # pylint:disable=protected-access
-    if cache is None:
-        cache = implemented_by_self._super_cache = weakref.WeakKeyDictionary()
-
-    key = sup.__thisclass__
-    try:
-        return cache[key]
-    except KeyError:
-        pass
-
-    next_cls = _next_super_class(sup)
-    # For ``implementedBy(cls)``:
-    # .__bases__ is .declared + [implementedBy(b) for b in cls.__bases__]
-    # .inherit is cls
-
-    implemented_by_next = implementedBy(next_cls)
-    mro = sup.__self_class__.__mro__
-    ix_next_cls = mro.index(next_cls)
-    classes_to_keep = mro[ix_next_cls:]
-    new_bases = [implementedBy(c) for c in classes_to_keep]
-
-    new = Implements.named(
-        implemented_by_self.__name__ + ':' + implemented_by_next.__name__,
-        *new_bases
+    __slots__ = (
+        '__name__',
+        '__ibmodule__',
+        '_v_cached_hash',
     )
-    new.inherit = implemented_by_next.inherit
-    new.declared = implemented_by_next.declared
-    # I don't *think* that new needs to subscribe to ``implemented_by_self``;
-    # it auto-subscribed to its bases, and that should be good enough.
-    cache[key] = new
 
-    return new
+    def __init__(self, name=None, module=None):
+        self.__name__ = name
+        self.__ibmodule__ = module
 
+    def _call_conform(self, conform):
+        raise NotImplementedError
 
-@_use_c_impl
-def implementedBy(cls): # pylint:disable=too-many-return-statements,too-many-branches
-    """Return the interfaces implemented for a class' instances
+    @property
+    def __module_property__(self):
+        # This is for _InterfaceMetaClass
+        return self.__ibmodule__
 
-      The value returned is an `~zope.interface.interfaces.IDeclaration`.
-    """
-    try:
-        if isinstance(cls, super):
-            # Yes, this needs to be inside the try: block. Some objects
-            # like security proxies even break isinstance.
-            return _implementedBy_super(cls)
-
-        spec = cls.__dict__.get('__implemented__')
-    except AttributeError:
-
-        # we can't get the class dict. This is probably due to a
-        # security proxy.  If this is the case, then probably no
-        # descriptor was installed for the class.
-
-        # We don't want to depend directly on zope.security in
-        # zope.interface, but we'll try to make reasonable
-        # accommodations in an indirect way.
-
-        # We'll check to see if there's an implements:
-
-        spec = getattr(cls, '__implemented__', None)
-        if spec is None:
-            # There's no spec stred in the class. Maybe its a builtin:
-            spec = BuiltinImplementationSpecifications.get(cls)
-            if spec is not None:
-                return spec
-            return _empty
-
-        if spec.__class__ == Implements:
-            # we defaulted to _empty or there was a spec. Good enough.
-            # Return it.
-            return spec
-
-        # TODO: need old style __implements__ compatibility?
-        # Hm, there's an __implemented__, but it's not a spec. Must be
-        # an old-style declaration. Just compute a spec for it
-        return Declaration(*_normalizeargs((spec, )))
-
-    if isinstance(spec, Implements):
-        return spec
-
-    if spec is None:
-        spec = BuiltinImplementationSpecifications.get(cls)
-        if spec is not None:
-            return spec
-
-    # TODO: need old style __implements__ compatibility?
-    spec_name = _implements_name(cls)
-    if spec is not None:
-        # old-style __implemented__ = foo declaration
-        spec = (spec, ) # tuplefy, as it might be just an int
-        spec = Implements.named(spec_name, *_normalizeargs(spec))
-        spec.inherit = None    # old-style implies no inherit
-        del cls.__implemented__ # get rid of the old-style declaration
-    else:
+    def __call__(self, obj, alternate=_marker):
+        """Adapt an object to the interface
+        """
         try:
-            bases = cls.__bases__
+            conform = obj.__conform__
         except AttributeError:
-            if not callable(cls):
-                raise TypeError("ImplementedBy called for non-factory", cls)
-            bases = ()
-
-        spec = Implements.named(spec_name, *[implementedBy(c) for c in bases])
-        spec.inherit = cls
-
-    try:
-        cls.__implemented__ = spec
-        if not hasattr(cls, '__providedBy__'):
-            cls.__providedBy__ = objectSpecificationDescriptor
-
-        if isinstance(cls, type) and '__provides__' not in cls.__dict__:
-            # Make sure we get a __provides__ descriptor
-            cls.__provides__ = ClassProvides(
-                cls,
-                getattr(cls, '__class__', type(cls)),
-                )
-
-    except TypeError:
-        if not isinstance(cls, type):
-            raise TypeError("ImplementedBy called for non-type", cls)
-        BuiltinImplementationSpecifications[cls] = spec
+            conform = None
 
-    return spec
+        if conform is not None:
+            adapter = self._call_conform(conform)
+            if adapter is not None:
+                return adapter
+
+        adapter = self.__adapt__(obj)
+
+        if adapter is not None:
+            return adapter
+        if alternate is not _marker:
+            return alternate
+        raise TypeError("Could not adapt", obj, self)
 
+    def __adapt__(self, obj):
+        """Adapt an object to the receiver
+        """
+        if self.providedBy(obj):
+            return obj
 
-def classImplementsOnly(cls, *interfaces):
-    """
-    Declare the only interfaces implemented by instances of a class
-
-    The arguments after the class are one or more interfaces or interface
-    specifications (`~zope.interface.interfaces.IDeclaration` objects).
+        for hook in adapter_hooks:
+            adapter = hook(self, obj)
+            if adapter is not None:
+                return adapter
 
-    The interfaces given (including the interfaces in the specifications)
-    replace any previous declarations, *including* inherited definitions. If you
-    wish to preserve inherited declarations, you can pass ``implementedBy(cls)``
-    in *interfaces*. This can be used to alter the interface resolution order.
-    """
-    spec = implementedBy(cls)
-    # Clear out everything inherited. It's important to
-    # also clear the bases right now so that we don't improperly discard
-    # interfaces that are already implemented by *old* bases that we're
-    # about to get rid of.
-    spec.declared = ()
-    spec.inherit = None
-    spec.__bases__ = ()
-    _classImplements_ordered(spec, interfaces, ())
+        return None
 
+    def __hash__(self):
+        # pylint:disable=assigning-non-slot,attribute-defined-outside-init
+        try:
+            return self._v_cached_hash
+        except AttributeError:
+            self._v_cached_hash = hash((self.__name__, self.__module__))
+        return self._v_cached_hash
 
-def classImplements(cls, *interfaces):
-    """
-    Declare additional interfaces implemented for instances of a class
+    def __eq__(self, other):
+        c = self._compare(other)
+        if c is NotImplemented:
+            return c
+        return c == 0
 
-    The arguments after the class are one or more interfaces or
-    interface specifications (`~zope.interface.interfaces.IDeclaration` objects).
+    def __ne__(self, other):
+        if other is self:
+            return False
 
-    The interfaces given (including the interfaces in the specifications)
-    are added to any interfaces previously declared. An effort is made to
-    keep a consistent C3 resolution order, but this cannot be guaranteed.
-
-    .. versionchanged:: 5.0.0
-       Each individual interface in *interfaces* may be added to either the
-       beginning or end of the list of interfaces declared for *cls*,
-       based on inheritance, in order to try to maintain a consistent
-       resolution order. Previously, all interfaces were added to the end.
-    .. versionchanged:: 5.1.0
-       If *cls* is already declared to implement an interface (or derived interface)
-       in *interfaces* through inheritance, the interface is ignored. Previously, it
-       would redundantly be made direct base of *cls*, which often produced inconsistent
-       interface resolution orders. Now, the order will be consistent, but may change.
-       Also, if the ``__bases__`` of the *cls* are later changed, the *cls* will no
-       longer be considered to implement such an interface (changing the ``__bases__`` of *cls*
-       has never been supported).
-    """
-    spec = implementedBy(cls)
-    interfaces = tuple(_normalizeargs(interfaces))
+        c = self._compare(other)
+        if c is NotImplemented:
+            return c
+        return c != 0
 
-    before = []
-    after = []
+adapter_hooks = _use_c_impl([], 'adapter_hooks')
 
-    # Take steps to try to avoid producing an invalid resolution
-    # order, while still allowing for BWC (in the past, we always
-    # appended)
-    for iface in interfaces:
-        for b in spec.declared:
-            if iface.extends(b):
-                before.append(iface)
-                break
-        else:
-            after.append(iface)
-    _classImplements_ordered(spec, tuple(before), tuple(after))
 
+class Specification(SpecificationBase):
+    """Specifications
 
-def classImplementsFirst(cls, iface):
-    """
-    Declare that instances of *cls* additionally provide *iface*.
+    An interface specification is used to track interface declarations
+    and component registrations.
 
-    The second argument is an interface or interface specification.
-    It is added as the highest priority (first in the IRO) interface;
-    no attempt is made to keep a consistent resolution order.
+    This class is a base class for both interfaces themselves and for
+    interface specifications (declarations).
 
-    .. versionadded:: 5.0.0
+    Specifications are mutable.  If you reassign their bases, their
+    relations with other specifications are adjusted accordingly.
     """
-    spec = implementedBy(cls)
-    _classImplements_ordered(spec, (iface,), ())
-
-
-def _classImplements_ordered(spec, before=(), after=()):
-    # Elide everything already inherited.
-    # Except, if it is the root, and we don't already declare anything else
-    # that would imply it, allow the root through. (TODO: When we disallow non-strict
-    # IRO, this part of the check can be removed because it's not possible to re-declare
-    # like that.)
-    before = [
-        x
-        for x in before
-        if not spec.isOrExtends(x) or (x is Interface and not spec.declared)
-    ]
-    after = [
-        x
-        for x in after
-        if not spec.isOrExtends(x) or (x is Interface and not spec.declared)
-    ]
-
-    # eliminate duplicates
-    new_declared = []
-    seen = set()
-    for l in before, spec.declared, after:
-        for b in l:
-            if b not in seen:
-                new_declared.append(b)
-                seen.add(b)
-
-    spec.declared = tuple(new_declared)
-
-    # compute the bases
-    bases = new_declared # guaranteed no dupes
-
-    if spec.inherit is not None:
-        for c in spec.inherit.__bases__:
-            b = implementedBy(c)
-            if b not in seen:
-                seen.add(b)
-                bases.append(b)
-
-    spec.__bases__ = tuple(bases)
-
-
-def _implements_advice(cls):
-    interfaces, do_classImplements = cls.__dict__['__implements_advice_data__']
-    del cls.__implements_advice_data__
-    do_classImplements(cls, *interfaces)
-    return cls
-
-
-class implementer:
-    """
-    Declare the interfaces implemented by instances of a class.
-
-    This function is called as a class decorator.
-
-    The arguments are one or more interfaces or interface
-    specifications (`~zope.interface.interfaces.IDeclaration`
-    objects).
-
-    The interfaces given (including the interfaces in the
-    specifications) are added to any interfaces previously declared,
-    unless the interface is already implemented.
-
-    Previous declarations include declarations for base classes unless
-    implementsOnly was used.
-
-    This function is provided for convenience. It provides a more
-    convenient way to call `classImplements`. For example::
-
-        @implementer(I1)
-        class C(object):
-            pass
-
-    is equivalent to calling::
+    __slots__ = ()
 
-        classImplements(C, I1)
+    # The root of all Specifications. This will be assigned `Interface`,
+    # once it is defined.
+    _ROOT = None
+
+    # Copy some base class methods for speed
+    isOrExtends = SpecificationBase.isOrExtends
+    providedBy = SpecificationBase.providedBy
+
+    def __init__(self, bases=()):
+        # There are many leaf interfaces with no dependents,
+        # and a few with very many. It's a heavily left-skewed
+        # distribution. In a survey of Plone and Zope related packages
+        # that loaded 2245 InterfaceClass objects and 2235 ClassProvides
+        # instances, there were a total of 7000 Specification objects created.
+        # 4700 had 0 dependents, 1400 had 1, 382 had 2 and so on. Only one
+        # for <type> had 1664. So there's savings to be had deferring
+        # the creation of dependents.
+        self._dependents = None # type: weakref.WeakKeyDictionary
+        self._bases = ()
+        self._implied = {}
+        self._v_attrs = None
+        self.__iro__ = ()
+        self.__sro__ = ()
 
-    after the class has been created.
+        self.__bases__ = tuple(bases)
 
-    .. seealso:: `classImplements`
-       The change history provided there applies to this function too.
-    """
-    __slots__ = ('interfaces',)
-
-    def __init__(self, *interfaces):
-        self.interfaces = interfaces
+    @property
+    def dependents(self):
+        if self._dependents is None:
+            self._dependents = weakref.WeakKeyDictionary()
+        return self._dependents
 
-    def __call__(self, ob):
-        if isinstance(ob, type):
-            # This is the common branch for classes.
-            classImplements(ob, *self.interfaces)
-            return ob
+    def subscribe(self, dependent):
+        self._dependents[dependent] = self.dependents.get(dependent, 0) + 1
 
-        spec_name = _implements_name(ob)
-        spec = Implements.named(spec_name, *self.interfaces)
+    def unsubscribe(self, dependent):
         try:
-            ob.__implemented__ = spec
-        except AttributeError:
-            raise TypeError("Can't declare implements", ob)
-        return ob
+            n = self._dependents[dependent]
+        except TypeError:
+            raise KeyError(dependent)
+        n -= 1
+        if not n:
+            del self.dependents[dependent]
+        else:
+            assert n > 0
+            self.dependents[dependent] = n
 
-class implementer_only:
-    """Declare the only interfaces implemented by instances of a class
+    def __setBases(self, bases):
+        # Remove ourselves as a dependent of our old bases
+        for b in self.__bases__:
+            b.unsubscribe(self)
+
+        # Register ourselves as a dependent of our new bases
+        self._bases = bases
+        for b in bases:
+            b.subscribe(self)
+
+        self.changed(self)
+
+    __bases__ = property(
+        lambda self: self._bases,
+        __setBases,
+        )
 
-      This function is called as a class decorator.
+    # This method exists for tests to override the way we call
+    # ro.calculate_ro(), usually by adding extra kwargs. We don't
+    # want to have a mutable dictionary as a class member that we pass
+    # ourself because mutability is bad, and passing **kw is slower than
+    # calling the bound function.
+    _do_calculate_ro = calculate_ro
 
-      The arguments are one or more interfaces or interface
-      specifications (`~zope.interface.interfaces.IDeclaration` objects).
+    def _calculate_sro(self):
+        """
+        Calculate and return the resolution order for this object, using its ``__bases__``.
 
-      Previous declarations including declarations for base classes
-      are overridden.
+        Ensures that ``Interface`` is always the last (lowest priority) element.
+        """
+        # We'd like to make Interface the lowest priority as a
+        # property of the resolution order algorithm. That almost
+        # works out naturally, but it fails when class inheritance has
+        # some bases that DO implement an interface, and some that DO
+        # NOT. In such a mixed scenario, you wind up with a set of
+        # bases to consider that look like this: [[..., Interface],
+        # [..., object], ...]. Depending on the order of inheritance,
+        # Interface can wind up before or after object, and that can
+        # happen at any point in the tree, meaning Interface can wind
+        # up somewhere in the middle of the order. Since Interface is
+        # treated as something that everything winds up implementing
+        # anyway (a catch-all for things like adapters), having it high up
+        # the order is bad. It's also bad to have it at the end, just before
+        # some concrete class: concrete classes should be HIGHER priority than
+        # interfaces (because there's only one class, but many implementations).
+        #
+        # One technically nice way to fix this would be to have
+        # ``implementedBy(object).__bases__ = (Interface,)``
+        #
+        # But: (1) That fails for old-style classes and (2) that causes
+        # everything to appear to *explicitly* implement Interface, when up
+        # to this point it's been an implicit virtual sort of relationship.
+        #
+        # So we force the issue by mutating the resolution order.
 
-      This function is provided for convenience. It provides a more
-      convenient way to call `classImplementsOnly`. For example::
+        # Note that we let C3 use pre-computed __sro__ for our bases.
+        # This requires that by the time this method is invoked, our bases
+        # have settled their SROs. Thus, ``changed()`` must first
+        # update itself before telling its descendents of changes.
+        sro = self._do_calculate_ro(base_mros={
+            b: b.__sro__
+            for b in self.__bases__
+        })
+        root = self._ROOT
+        if root is not None and sro and sro[-1] is not root:
+            # In one dataset of 1823 Interface objects, 1117 ClassProvides objects,
+            # sro[-1] was root 4496 times, and only not root 118 times. So it's
+            # probably worth checking.
+
+            # Once we don't have to deal with old-style classes,
+            # we can add a check and only do this if base_count > 1,
+            # if we tweak the bootstrapping for ``<implementedBy object>``
+            sro = [
+                x
+                for x in sro
+                if x is not root
+            ]
+            sro.append(root)
 
-        @implementer_only(I1)
-        class C(object): pass
+        return sro
 
-      is equivalent to calling::
+    def changed(self, originally_changed):
+        """
+        We, or something we depend on, have changed.
 
-        classImplementsOnly(I1)
+        By the time this is called, the things we depend on,
+        such as our bases, should themselves be stable.
+        """
+        self._v_attrs = None
 
-      after the class has been created.
-      """
+        implied = self._implied
+        implied.clear()
 
-    def __init__(self, *interfaces):
-        self.interfaces = interfaces
+        ancestors = self._calculate_sro()
+        self.__sro__ = tuple(ancestors)
+        self.__iro__ = tuple([ancestor for ancestor in ancestors
+                              if isinstance(ancestor, InterfaceClass)
+                              ])
+
+        for ancestor in ancestors:
+            # We directly imply our ancestors:
+            implied[ancestor] = ()
+
+        # Now, advise our dependents of change
+        # (being careful not to create the WeakKeyDictionary if not needed):
+        for dependent in tuple(self._dependents.keys() if self._dependents else ()):
+            dependent.changed(originally_changed)
+
+        # Just in case something called get() at some point
+        # during that process and we have a cycle of some sort
+        # make sure we didn't cache incomplete results.
+        self._v_attrs = None
 
-    def __call__(self, ob):
-        if isinstance(ob, (FunctionType, MethodType)):
-            # XXX Does this decorator make sense for anything but classes?
-            # I don't think so. There can be no inheritance of interfaces
-            # on a method or function....
-            raise ValueError('The implementer_only decorator is not '
-                             'supported for methods or functions.')
+    def interfaces(self):
+        """Return an iterator for the interfaces in the specification.
+        """
+        seen = {}
+        for base in self.__bases__:
+            for interface in base.interfaces():
+                if interface not in seen:
+                    seen[interface] = 1
+                    yield interface
 
-        # Assume it's a class:
-        classImplementsOnly(ob, *self.interfaces)
-        return ob
+    def extends(self, interface, strict=True):
+        """Does the specification extend the given interface?
 
+        Test whether an interface in the specification extends the
+        given interface
+        """
+        return ((interface in self._implied)
+                and
+                ((not strict) or (self != interface))
+                )
 
-##############################################################################
-#
-# Instance declarations
+    def weakref(self, callback=None):
+        return weakref.ref(self, callback)
 
-class Provides(Declaration):  # Really named ProvidesClass
-    """Implement ``__provides__``, the instance-specific specification
+    def get(self, name, default=None):
+        """Query for an attribute description
+        """
+        attrs = self._v_attrs
+        if attrs is None:
+            attrs = self._v_attrs = {}
+        attr = attrs.get(name)
+        if attr is None:
+            for iface in self.__iro__:
+                attr = iface.direct(name)
+                if attr is not None:
+                    attrs[name] = attr
+                    break
+
+        return default if attr is None else attr
+
+
+class _InterfaceMetaClass(type):
+    # Handling ``__module__`` on ``InterfaceClass`` is tricky. We need
+    # to be able to read it on a type and get the expected string. We
+    # also need to be able to set it on an instance and get the value
+    # we set. So far so good. But what gets tricky is that we'd like
+    # to store the value in the C structure (``InterfaceBase.__ibmodule__``) for
+    # direct access during equality, sorting, and hashing. "No
+    # problem, you think, I'll just use a property" (well, the C
+    # equivalents, ``PyMemberDef`` or ``PyGetSetDef``).
+    #
+    # Except there is a problem. When a subclass is created, the
+    # metaclass (``type``) always automatically puts the expected
+    # string in the class's dictionary under ``__module__``, thus
+    # overriding the property inherited from the superclass. Writing
+    # ``Subclass.__module__`` still works, but
+    # ``Subclass().__module__`` fails.
+    #
+    # There are multiple ways to work around this:
+    #
+    # (1) Define ``InterfaceBase.__getattribute__`` to watch for
+    # ``__module__`` and return the C storage.
+    #
+    # This works, but slows down *all* attribute access (except,
+    # ironically, to ``__module__``) by about 25% (40ns becomes 50ns)
+    # (when implemented in C). Since that includes methods like
+    # ``providedBy``, that's probably not acceptable.
+    #
+    # All the other methods involve modifying subclasses. This can be
+    # done either on the fly in some cases, as instances are
+    # constructed, or by using a metaclass. These next few can be done on the fly.
+    #
+    # (2) Make ``__module__`` a descriptor in each subclass dictionary.
+    # It can't be a straight up ``@property`` descriptor, though, because accessing
+    # it on the class returns a ``property`` object, not the desired string.
+    #
+    # (3) Implement a data descriptor (``__get__`` and ``__set__``)
+    # that is both a subclass of string, and also does the redirect of
+    # ``__module__`` to ``__ibmodule__`` and does the correct thing
+    # with the ``instance`` argument to ``__get__`` is None (returns
+    # the class's value.) (Why must it be a subclass of string? Because
+    # when it' s in the class's dict, it's defined on an *instance* of the
+    # metaclass; descriptors in an instance's dict aren't honored --- their
+    # ``__get__`` is never invoked --- so it must also *be* the value we want
+    # returned.)
+    #
+    # This works, preserves the ability to read and write
+    # ``__module__``, and eliminates any penalty accessing other
+    # attributes. But it slows down accessing ``__module__`` of
+    # instances by 200% (40ns to 124ns), requires editing class dicts on the fly
+    # (in InterfaceClass.__init__), thus slightly slowing down all interface creation,
+    # and is ugly.
+    #
+    # (4) As in the last step, but make it a non-data descriptor (no ``__set__``).
+    #
+    # If you then *also* store a copy of ``__ibmodule__`` in
+    # ``__module__`` in the instance's dict, reading works for both
+    # class and instance and is full speed for instances. But the cost
+    # is storage space, and you can't write to it anymore, not without
+    # things getting out of sync.
+    #
+    # (Actually, ``__module__`` was never meant to be writable. Doing
+    # so would break BTrees and normal dictionaries, as well as the
+    # repr, maybe more.)
+    #
+    # That leaves us with a metaclass. (Recall that a class is an
+    # instance of its metaclass, so properties/descriptors defined in
+    # the metaclass are used when accessing attributes on the
+    # instance/class. We'll use that to define ``__module__``.) Here
+    # we can have our cake and eat it too: no extra storage, and
+    # C-speed access to the underlying storage. The only substantial
+    # cost is that metaclasses tend to make people's heads hurt. (But
+    # still less than the descriptor-is-string, hopefully.)
 
-    When an object is pickled, we pickle the interfaces that it implements.
-    """
+    __slots__ = ()
 
-    def __init__(self, cls, *interfaces):
-        self.__args = (cls, ) + interfaces
-        self._cls = cls
-        Declaration.__init__(self, *self._add_interfaces_to_cls(interfaces, cls))
+    def __new__(cls, name, bases, attrs):
+        # Figure out what module defined the interface.
+        # This is copied from ``InterfaceClass.__init__``;
+        # reviewers aren't sure how AttributeError or KeyError
+        # could be raised.
+        __module__ = sys._getframe(1).f_globals['__name__']
+        # Get the C optimized __module__ accessor and give it
+        # to the new class.
+        moduledescr = InterfaceBase.__dict__['__module__']
+        if isinstance(moduledescr, str):
+            # We're working with the Python implementation,
+            # not the C version
+            moduledescr = InterfaceBase.__dict__['__module_property__']
+        attrs['__module__'] = moduledescr
+        kind = type.__new__(cls, name, bases, attrs)
+        kind.__module = __module__
+        return kind
 
-    # Added to by ``moduleProvides``, et al
-    _v_module_names = ()
+    @property
+    def __module__(cls):
+        return cls.__module
 
-    def __repr__(self):
-        # The typical way to create instances of this
-        # object is via calling ``directlyProvides(...)`` or ``alsoProvides()``,
-        # but that's not the only way. Proxies, for example,
-        # directly use the ``Provides(...)`` function (which is the
-        # more generic method, and what we pickle as). We're after the most
-        # readable, useful repr in the common case, so we use the most
-        # common name.
-        #
-        # We also cooperate with ``moduleProvides`` to attempt to do the
-        # right thing for that API. See it for details.
-        function_name = 'directlyProvides'
-        if self._cls is ModuleType and self._v_module_names:
-            # See notes in ``moduleProvides``/``directlyProvides``
-            providing_on_module = True
-            interfaces = self.__args[1:]
-        else:
-            providing_on_module = False
-            interfaces = (self._cls,) + self.__bases__
-        ordered_names = self._argument_names_for_repr(interfaces)
-        if providing_on_module:
-            mod_names = self._v_module_names
-            if len(mod_names) == 1:
-                mod_names = "sys.modules[%r]" % mod_names[0]
-            ordered_names = (
-                '{}, '.format(mod_names)
-            ) + ordered_names
-        return "{}({})".format(
-            function_name,
-            ordered_names,
+    def __repr__(cls):
+        return "<class '{}.{}'>".format(
+            cls.__module,
+            cls.__name__,
         )
 
-    def __reduce__(self):
-        # This reduces to the Provides *function*, not
-        # this class.
-        return Provides, self.__args
-
-    __module__ = 'zope.interface'
-
-    def __get__(self, inst, cls):
-        """Make sure that a class __provides__ doesn't leak to an instance
-        """
-        if inst is None and cls is self._cls:
-            # We were accessed through a class, so we are the class'
-            # provides spec. Just return this object, but only if we are
-            # being called on the same class that we were defined for:
-            return self
 
-        raise AttributeError('__provides__')
+_InterfaceClassBase = _InterfaceMetaClass(
+    'InterfaceClass',
+    # From least specific to most specific.
+    (InterfaceBase, Specification, Element),
+    {'__slots__': ()}
+)
 
-ProvidesClass = Provides
 
-# Registry of instance declarations
-# This is a memory optimization to allow objects to share specifications.
-InstanceDeclarations = weakref.WeakValueDictionary()
-
-def Provides(*interfaces): # pylint:disable=function-redefined
-    """Declaration for an instance of *cls*.
-
-       The correct signature is ``cls, *interfaces``.
-       The *cls* is necessary to avoid the
-       construction of inconsistent resolution orders.
-
-      Instance declarations are shared among instances that have the same
-      declaration. The declarations are cached in a weak value dictionary.
+def interfacemethod(func):
     """
-    spec = InstanceDeclarations.get(interfaces)
-    if spec is None:
-        spec = ProvidesClass(*interfaces)
-        InstanceDeclarations[interfaces] = spec
-
-    return spec
-
-Provides.__safe_for_unpickling__ = True
-
+    Convert a method specification to an actual method of the interface.
 
-def directlyProvides(object, *interfaces): # pylint:disable=redefined-builtin
-    """Declare interfaces declared directly for an object
+    This is a decorator that functions like `staticmethod` et al.
 
-      The arguments after the object are one or more interfaces or interface
-      specifications (`~zope.interface.interfaces.IDeclaration` objects).
+    The primary use of this decorator is to allow interface definitions to
+    define the ``__adapt__`` method, but other interface methods can be
+    overridden this way too.
 
-      The interfaces given (including the interfaces in the specifications)
-      replace interfaces previously declared for the object.
+    .. seealso:: `zope.interface.interfaces.IInterfaceDeclaration.interfacemethod`
     """
-    cls = getattr(object, '__class__', None)
-    if cls is not None and getattr(cls, '__class__', None) is cls:
-        # It's a meta class (well, at least it it could be an extension class)
-        # Note that we can't get here from the tests:  there is no normal
-        # class which isn't descriptor aware.
-        if not isinstance(object, type):
-            raise TypeError("Attempt to make an interface declaration on a "
-                            "non-descriptor-aware class")
-
-    interfaces = _normalizeargs(interfaces)
-    if cls is None:
-        cls = type(object)
-
-    if issubclass(cls, type):
-        # we have a class or type.  We'll use a special descriptor
-        # that provides some extra caching
-        object.__provides__ = ClassProvides(object, cls, *interfaces)
-    else:
-        provides = object.__provides__ = Provides(cls, *interfaces)
-        # See notes in ``moduleProvides``.
-        if issubclass(cls, ModuleType) and hasattr(object, '__name__'):
-            provides._v_module_names += (object.__name__,)
-
-
+    f_locals = sys._getframe(1).f_locals
+    methods = f_locals.setdefault(INTERFACE_METHODS, {})
+    methods[func.__name__] = func
+    return _decorator_non_return
 
-def alsoProvides(object, *interfaces): # pylint:disable=redefined-builtin
-    """Declare interfaces declared directly for an object
 
-    The arguments after the object are one or more interfaces or interface
-    specifications (`~zope.interface.interfaces.IDeclaration` objects).
-
-    The interfaces given (including the interfaces in the specifications) are
-    added to the interfaces previously declared for the object.
+class InterfaceClass(_InterfaceClassBase):
     """
-    directlyProvides(object, directlyProvidedBy(object), *interfaces)
-
+    Prototype (scarecrow) Interfaces Implementation.
 
-def noLongerProvides(object, interface): # pylint:disable=redefined-builtin
-    """ Removes a directly provided interface from an object.
+    Note that it is not possible to change the ``__name__`` or ``__module__``
+    after an instance of this object has been constructed.
     """
-    directlyProvides(object, directlyProvidedBy(object) - interface)
-    if interface.providedBy(object):
-        raise ValueError("Can only remove directly provided interfaces.")
 
+    # We can't say this yet because we don't have enough
+    # infrastructure in place.
+    #
+    #implements(IInterface)
 
-@_use_c_impl
-class ClassProvidesBase(SpecificationBase):
+    def __new__(cls, name=None, bases=(), attrs=None, __doc__=None, # pylint:disable=redefined-builtin
+                __module__=None):
+        assert isinstance(bases, tuple)
+        attrs = attrs or {}
+        needs_custom_class = attrs.pop(INTERFACE_METHODS, None)
+        if needs_custom_class:
+            needs_custom_class.update(
+                {'__classcell__': attrs.pop('__classcell__')}
+                if '__classcell__' in attrs
+                else {}
+            )
+            if '__adapt__' in needs_custom_class:
+                # We need to tell the C code to call this.
+                needs_custom_class['_CALL_CUSTOM_ADAPT'] = 1
 
-    __slots__ = (
-        '_cls',
-        '_implements',
-    )
-
-    def __get__(self, inst, cls):
-        # member slots are set by subclass
-        # pylint:disable=no-member
-        if cls is self._cls:
-            # We only work if called on the class we were defined for
+            if issubclass(cls, _InterfaceClassWithCustomMethods):
+                cls_bases = (cls,)
+            elif cls is InterfaceClass:
+                cls_bases = (_InterfaceClassWithCustomMethods,)
+            else:
+                cls_bases = (cls, _InterfaceClassWithCustomMethods)
 
-            if inst is None:
-                # We were accessed through a class, so we are the class'
-                # provides spec. Just return this object as is:
-                return self
+            cls = type(cls)( # pylint:disable=self-cls-assignment
+                name + "<WithCustomMethods>",
+                cls_bases,
+                needs_custom_class
+            )
+
+        return _InterfaceClassBase.__new__(cls)
+
+    def __init__(self, name, bases=(), attrs=None, __doc__=None,  # pylint:disable=redefined-builtin
+                 __module__=None):
+        # We don't call our metaclass parent directly
+        # pylint:disable=non-parent-init-called
+        # pylint:disable=super-init-not-called
+        if not all(isinstance(base, InterfaceClass) for base in bases):
+            raise TypeError('Expected base interfaces')
+
+        if attrs is None:
+            attrs = {}
+
+        if __module__ is None:
+            __module__ = attrs.get('__module__')
+            if isinstance(__module__, str):
+                del attrs['__module__']
+            else:
+                try:
+                    # Figure out what module defined the interface.
+                    # This is how cPython figures out the module of
+                    # a class, but of course it does it in C. :-/
+                    __module__ = sys._getframe(1).f_globals['__name__']
+                except (AttributeError, KeyError): # pragma: no cover
+                    pass
+
+        InterfaceBase.__init__(self, name, __module__)
+        # These asserts assisted debugging the metaclass
+        # assert '__module__' not in self.__dict__
+        # assert self.__ibmodule__ is self.__module__ is __module__
+
+        d = attrs.get('__doc__')
+        if d is not None:
+            if not isinstance(d, Attribute):
+                if __doc__ is None:
+                    __doc__ = d
+                del attrs['__doc__']
+
+        if __doc__ is None:
+            __doc__ = ''
+
+        Element.__init__(self, name, __doc__)
+
+        tagged_data = attrs.pop(TAGGED_DATA, None)
+        if tagged_data is not None:
+            for key, val in tagged_data.items():
+                self.setTaggedValue(key, val)
+
+        Specification.__init__(self, bases)
+        self.__attrs = self.__compute_attrs(attrs)
+
+        self.__identifier__ = "{}.{}".format(__module__, name)
+
+    def __compute_attrs(self, attrs):
+        # Make sure that all recorded attributes (and methods) are of type
+        # `Attribute` and `Method`
+        def update_value(aname, aval):
+            if isinstance(aval, Attribute):
+                aval.interface = self
+                if not aval.__name__:
+                    aval.__name__ = aname
+            elif isinstance(aval, FunctionType):
+                aval = fromFunction(aval, self, name=aname)
+            else:
+                raise InvalidInterface("Concrete attribute, " + aname)
+            return aval
 
-            return self._implements
+        return {
+            aname: update_value(aname, aval)
+            for aname, aval in attrs.items()
+            if aname not in (
+                # __locals__: Python 3 sometimes adds this.
+                '__locals__',
+                # __qualname__: PEP 3155 (Python 3.3+)
+                '__qualname__',
+                # __annotations__: PEP 3107 (Python 3.0+)
+                '__annotations__',
+                # __static_attributes__: Python 3.13a6+
+                # https://github.com/python/cpython/pull/115913
+                '__static_attributes__',
+                # __firstlineno__: Python 3.13b1+
+                # https://github.com/python/cpython/pull/118475
+                '__firstlineno__',
+            )
+            and aval is not _decorator_non_return
+        }
 
-        raise AttributeError('__provides__')
+    def interfaces(self):
+        """Return an iterator for the interfaces in the specification.
+        """
+        yield self
 
+    def getBases(self):
+        return self.__bases__
 
-class ClassProvides(Declaration, ClassProvidesBase):
-    """Special descriptor for class ``__provides__``
+    def isEqualOrExtendedBy(self, other):
+        """Same interface or extends?"""
+        return self == other or other.extends(self)
 
-    The descriptor caches the implementedBy info, so that
-    we can get declarations for objects without instance-specific
-    interfaces a bit quicker.
-    """
+    def names(self, all=False): # pylint:disable=redefined-builtin
+        """Return the attribute names defined by the interface."""
+        if not all:
+            return self.__attrs.keys()
 
-    __slots__ = (
-        '__args',
-    )
+        r = self.__attrs.copy()
 
-    def __init__(self, cls, metacls, *interfaces):
-        self._cls = cls
-        self._implements = implementedBy(cls)
-        self.__args = (cls, metacls, ) + interfaces
-        Declaration.__init__(self, *self._add_interfaces_to_cls(interfaces, metacls))
+        for base in self.__bases__:
+            r.update(dict.fromkeys(base.names(all)))
 
-    def __repr__(self):
-        # There are two common ways to get instances of this object:
-        # The most interesting way is calling ``@provider(..)`` as a decorator
-        # of a class; this is the same as calling ``directlyProvides(cls, ...)``.
-        #
-        # The other way is by default: anything that invokes ``implementedBy(x)``
-        # will wind up putting an instance in ``type(x).__provides__``; this includes
-        # the ``@implementer(...)`` decorator. Those instances won't have any
-        # interfaces.
-        #
-        # Thus, as our repr, we go with the ``directlyProvides()`` syntax.
-        interfaces = (self._cls, ) + self.__args[2:]
-        ordered_names = self._argument_names_for_repr(interfaces)
-        return "directlyProvides({})".format(ordered_names)
+        return r.keys()
 
-    def __reduce__(self):
-        return self.__class__, self.__args
+    def __iter__(self):
+        return iter(self.names(all=True))
 
-    # Copy base-class method for speed
-    __get__ = ClassProvidesBase.__get__
+    def namesAndDescriptions(self, all=False): # pylint:disable=redefined-builtin
+        """Return attribute names and descriptions defined by interface."""
+        if not all:
+            return self.__attrs.items()
 
+        r = {}
+        for base in self.__bases__[::-1]:
+            r.update(dict(base.namesAndDescriptions(all)))
 
-def directlyProvidedBy(object): # pylint:disable=redefined-builtin
-    """Return the interfaces directly provided by the given object
+        r.update(self.__attrs)
 
-    The value returned is an `~zope.interface.interfaces.IDeclaration`.
-    """
-    provides = getattr(object, "__provides__", None)
-    if (
-            provides is None # no spec
-            # We might have gotten the implements spec, as an
-            # optimization. If so, it's like having only one base, that we
-            # lop off to exclude class-supplied declarations:
-            or isinstance(provides, Implements)
-    ):
-        return _empty
+        return r.items()
 
-    # Strip off the class part of the spec:
-    return Declaration(provides.__bases__[:-1])
+    def getDescriptionFor(self, name):
+        """Return the attribute description for the given name."""
+        r = self.get(name)
+        if r is not None:
+            return r
 
+        raise KeyError(name)
 
-class provider:
-    """Declare interfaces provided directly by a class
+    __getitem__ = getDescriptionFor
 
-      This function is called in a class definition.
+    def __contains__(self, name):
+        return self.get(name) is not None
 
-      The arguments are one or more interfaces or interface specifications
-      (`~zope.interface.interfaces.IDeclaration` objects).
+    def direct(self, name):
+        return self.__attrs.get(name)
 
-      The given interfaces (including the interfaces in the specifications)
-      are used to create the class's direct-object interface specification.
-      An error will be raised if the module class has an direct interface
-      specification. In other words, it is an error to call this function more
-      than once in a class definition.
+    def queryDescriptionFor(self, name, default=None):
+        return self.get(name, default)
 
-      Note that the given interfaces have nothing to do with the interfaces
-      implemented by instances of the class.
+    def validateInvariants(self, obj, errors=None):
+        """validate object to defined invariants."""
 
-      This function is provided for convenience. It provides a more convenient
-      way to call `directlyProvides` for a class. For example::
+        for iface in self.__iro__:
+            for invariant in iface.queryDirectTaggedValue('invariants', ()):
+                try:
+                    invariant(obj)
+                except Invalid as error:
+                    if errors is not None:
+                        errors.append(error)
+                    else:
+                        raise
 
-        @provider(I1)
-        class C:
-            pass
+        if errors:
+            raise Invalid(errors)
 
-      is equivalent to calling::
+    def queryTaggedValue(self, tag, default=None):
+        """
+        Queries for the value associated with *tag*, returning it from the nearest
+        interface in the ``__iro__``.
 
-        directlyProvides(C, I1)
+        If not found, returns *default*.
+        """
+        for iface in self.__iro__:
+            value = iface.queryDirectTaggedValue(tag, _marker)
+            if value is not _marker:
+                return value
+        return default
 
-      after the class has been created.
-    """
+    def getTaggedValue(self, tag):
+        """ Returns the value associated with 'tag'. """
+        value = self.queryTaggedValue(tag, default=_marker)
+        if value is _marker:
+            raise KeyError(tag)
+        return value
+
+    def getTaggedValueTags(self):
+        """ Returns a list of all tags. """
+        keys = set()
+        for base in self.__iro__:
+            keys.update(base.getDirectTaggedValueTags())
+        return keys
 
-    def __init__(self, *interfaces):
-        self.interfaces = interfaces
+    def __repr__(self):
+        try:
+            return self._v_repr
+        except AttributeError:
+            name = str(self)
+            r = "<{} {}>".format(self.__class__.__name__, name)
+            self._v_repr = r # pylint:disable=attribute-defined-outside-init
+            return r
 
-    def __call__(self, ob):
-        directlyProvides(ob, *self.interfaces)
-        return ob
+    def __str__(self):
+        name = self.__name__
+        m = self.__ibmodule__
+        if m:
+            name = '{}.{}'.format(m, name)
+        return name
 
+    def _call_conform(self, conform):
+        try:
+            return conform(self)
+        except TypeError: # pragma: no cover
+            # We got a TypeError. It might be an error raised by
+            # the __conform__ implementation, or *we* may have
+            # made the TypeError by calling an unbound method
+            # (object is a class).  In the later case, we behave
+            # as though there is no __conform__ method. We can
+            # detect this case by checking whether there is more
+            # than one traceback object in the traceback chain:
+            if sys.exc_info()[2].tb_next is not None:
+                # There is more than one entry in the chain, so
+                # reraise the error:
+                raise
+            # This clever trick is from Phillip Eby
 
-def moduleProvides(*interfaces):
-    """Declare interfaces provided by a module
+        return None # pragma: no cover
 
-    This function is used in a module definition.
+    def __reduce__(self):
+        return self.__name__
 
-    The arguments are one or more interfaces or interface specifications
-    (`~zope.interface.interfaces.IDeclaration` objects).
+    def __or__(self, other):
+        """Allow type hinting syntax: Interface | None."""
+        return Union[self, other]
 
-    The given interfaces (including the interfaces in the specifications) are
-    used to create the module's direct-object interface specification.  An
-    error will be raised if the module already has an interface specification.
-    In other words, it is an error to call this function more than once in a
-    module definition.
+    def __ror__(self, other):
+        """Allow type hinting syntax: None | Interface."""
+        return Union[other, self]
 
-    This function is provided for convenience. It provides a more convenient
-    way to call directlyProvides. For example::
+Interface = InterfaceClass("Interface", __module__='zope.interface')
+# Interface is the only member of its own SRO.
+Interface._calculate_sro = lambda: (Interface,)
+Interface.changed(Interface)
+assert Interface.__sro__ == (Interface,)
+Specification._ROOT = Interface
+ro._ROOT = Interface
 
-      moduleProvides(I1)
+class _InterfaceClassWithCustomMethods(InterfaceClass):
+    """
+    Marker class for interfaces with custom methods that override InterfaceClass methods.
+    """
 
-    is equivalent to::
 
-      directlyProvides(sys.modules[__name__], I1)
+class Attribute(Element):
+    """Attribute descriptions
     """
-    frame = sys._getframe(1) # pylint:disable=protected-access
-    locals = frame.f_locals # pylint:disable=redefined-builtin
-
-    # Try to make sure we were called from a module body
-    if (locals is not frame.f_globals) or ('__name__' not in locals):
-        raise TypeError(
-            "moduleProvides can only be used from a module definition.")
-
-    if '__provides__' in locals:
-        raise TypeError(
-            "moduleProvides can only be used once in a module definition.")
-
-    # Note: This is cached based on the key ``(ModuleType, *interfaces)``;
-    # One consequence is that any module that provides the same interfaces
-    # gets the same ``__repr__``, meaning that you can't tell what module
-    # such a declaration came from. Adding the module name to ``_v_module_names``
-    # attempts to correct for this; it works in some common situations, but fails
-    # (1) after pickling (the data is lost) and (2) if declarations are
-    # actually shared and (3) if the alternate spelling of ``directlyProvides()``
-    # is used. Problem (3)  is fixed by cooperating with ``directlyProvides``
-    # to maintain this information, and problem (2) is worked around by
-    # printing all the names, but (1) is unsolvable without introducing
-    # new classes or changing the stored data...but it doesn't actually matter,
-    # because ``ModuleType`` can't be pickled!
-    p = locals["__provides__"] = Provides(ModuleType,
-                                          *_normalizeargs(interfaces))
-    p._v_module_names += (locals['__name__'],)
 
+    # We can't say this yet because we don't have enough
+    # infrastructure in place.
+    #
+    # implements(IAttribute)
 
-##############################################################################
-#
-# Declaration querying support
+    interface = None
 
-# XXX:  is this a fossil?  Nobody calls it, no unit tests exercise it, no
-#       doctests import it, and the package __init__ doesn't import it.
-#       (Answer: Versions of zope.container prior to 4.4.0 called this,
-#        and zope.proxy.decorator up through at least 4.3.5 called this.)
-def ObjectSpecification(direct, cls):
-    """Provide object specifications
+    def _get_str_info(self):
+        """Return extra data to put at the end of __str__."""
+        return ""
 
-    These combine information for the object and for it's classes.
-    """
-    return Provides(cls, direct) # pragma: no cover fossil
+    def __str__(self):
+        of = ''
+        if self.interface is not None:
+            of = self.interface.__module__ + '.' + self.interface.__name__ + '.'
+        # self.__name__ may be None during construction (e.g., debugging)
+        return of + (self.__name__ or '<unknown>') + self._get_str_info()
 
-@_use_c_impl
-def getObjectSpecification(ob):
-    try:
-        provides = ob.__provides__
-    except AttributeError:
-        provides = None
-
-    if provides is not None:
-        if isinstance(provides, SpecificationBase):
-            return provides
-
-    try:
-        cls = ob.__class__
-    except AttributeError:
-        # We can't get the class, so just consider provides
-        return _empty
-    return implementedBy(cls)
+    def __repr__(self):
+        return "<{}.{} object at 0x{:x} {}>".format(
+            type(self).__module__,
+            type(self).__name__,
+            id(self),
+            self
+        )
 
 
-@_use_c_impl
-def providedBy(ob):
-    """
-    Return the interfaces provided by *ob*.
+class Method(Attribute):
+    """Method interfaces
 
-    If *ob* is a :class:`super` object, then only interfaces implemented
-    by the remainder of the classes in the method resolution order are
-    considered. Interfaces directly provided by the object underlying *ob*
-    are not.
+    The idea here is that you have objects that describe methods.
+    This provides an opportunity for rich meta-data.
     """
-    # Here we have either a special object, an old-style declaration
-    # or a descriptor
-
-    # Try to get __providedBy__
-    try:
-        if isinstance(ob, super): # Some objects raise errors on isinstance()
-            return implementedBy(ob)
-
-        r = ob.__providedBy__
-    except AttributeError:
-        # Not set yet. Fall back to lower-level thing that computes it
-        return getObjectSpecification(ob)
-
-    try:
-        # We might have gotten a descriptor from an instance of a
-        # class (like an ExtensionClass) that doesn't support
-        # descriptors.  We'll make sure we got one by trying to get
-        # the only attribute, which all specs have.
-        r.extends
-    except AttributeError:
-
-        # The object's class doesn't understand descriptors.
-        # Sigh. We need to get an object descriptor, but we have to be
-        # careful.  We want to use the instance's __provides__, if
-        # there is one, but only if it didn't come from the class.
-
-        try:
-            r = ob.__provides__
-        except AttributeError:
-            # No __provides__, so just fall back to implementedBy
-            return implementedBy(ob.__class__)
-
-        # We need to make sure we got the __provides__ from the
-        # instance. We'll do this by making sure we don't get the same
-        # thing from the class:
 
-        try:
-            cp = ob.__class__.__provides__
-        except AttributeError:
-            # The ob doesn't have a class or the class has no
-            # provides, assume we're done:
-            return r
+    # We can't say this yet because we don't have enough
+    # infrastructure in place.
+    #
+    # implements(IMethod)
+
+    positional = required = ()
+    _optional = varargs = kwargs = None
+    def _get_optional(self):
+        if self._optional is None:
+            return {}
+        return self._optional
+    def _set_optional(self, opt):
+        self._optional = opt
+    def _del_optional(self):
+        self._optional = None
+    optional = property(_get_optional, _set_optional, _del_optional)
+
+    def __call__(self, *args, **kw):
+        raise BrokenImplementation(self.interface, self.__name__)
+
+    def getSignatureInfo(self):
+        return {'positional': self.positional,
+                'required': self.required,
+                'optional': self.optional,
+                'varargs': self.varargs,
+                'kwargs': self.kwargs,
+                }
+
+    def getSignatureString(self):
+        sig = []
+        for v in self.positional:
+            sig.append(v)
+            if v in self.optional.keys():
+                sig[-1] += "=" + repr(self.optional[v])
+        if self.varargs:
+            sig.append("*" + self.varargs)
+        if self.kwargs:
+            sig.append("**" + self.kwargs)
+
+        return "(%s)" % ", ".join(sig)
+
+    _get_str_info = getSignatureString
+
+
+def fromFunction(func, interface=None, imlevel=0, name=None):
+    name = name or func.__name__
+    method = Method(name, func.__doc__)
+    defaults = getattr(func, '__defaults__', None) or ()
+    code = func.__code__
+    # Number of positional arguments
+    na = code.co_argcount - imlevel
+    names = code.co_varnames[imlevel:]
+    opt = {}
+    # Number of required arguments
+    defaults_count = len(defaults)
+    if not defaults_count:
+        # PyPy3 uses ``__defaults_count__`` for builtin methods
+        # like ``dict.pop``. Surprisingly, these don't have recorded
+        # ``__defaults__``
+        defaults_count = getattr(func, '__defaults_count__', 0)
+
+    nr = na - defaults_count
+    if nr < 0:
+        defaults = defaults[-nr:]
+        nr = 0
+
+    # Determine the optional arguments.
+    opt.update(dict(zip(names[nr:], defaults)))
+
+    method.positional = names[:na]
+    method.required = names[:nr]
+    method.optional = opt
+
+    argno = na
+
+    # Determine the function's variable argument's name (i.e. *args)
+    if code.co_flags & CO_VARARGS:
+        method.varargs = names[argno]
+        argno = argno + 1
+    else:
+        method.varargs = None
 
-        if r is cp:
-            # Oops, we got the provides from the class. This means
-            # the object doesn't have it's own. We should use implementedBy
-            return implementedBy(ob.__class__)
+    # Determine the function's keyword argument's name (i.e. **kw)
+    if code.co_flags & CO_VARKEYWORDS:
+        method.kwargs = names[argno]
+    else:
+        method.kwargs = None
 
-    return r
+    method.interface = interface
 
+    for key, value in func.__dict__.items():
+        method.setTaggedValue(key, value)
 
-@_use_c_impl
-class ObjectSpecificationDescriptor:
-    """Implement the ``__providedBy__`` attribute
+    return method
 
-    The ``__providedBy__`` attribute computes the interfaces provided by
-    an object. If an object has an ``__provides__`` attribute, that is returned.
-    Otherwise, `implementedBy` the *cls* is returned.
-
-    .. versionchanged:: 5.4.0
-       Both the default (C) implementation and the Python implementation
-       now let exceptions raised by accessing ``__provides__`` propagate.
-       Previously, the C version ignored all exceptions.
-    .. versionchanged:: 5.4.0
-       The Python implementation now matches the C implementation and lets
-       a ``__provides__`` of ``None`` override what the class is declared to
-       implement.
-    """
 
-    def __get__(self, inst, cls):
-        """Get an object specification for an object
-        """
-        if inst is None:
-            return getObjectSpecification(cls)
+def fromMethod(meth, interface=None, name=None):
+    if isinstance(meth, MethodType):
+        func = meth.__func__
+    else:
+        func = meth
+    return fromFunction(func, interface, imlevel=1, name=name)
 
-        try:
-            return inst.__provides__
-        except AttributeError:
-            return implementedBy(cls)
 
+# Now we can create the interesting interfaces and wire them up:
+def _wire():
+    from zope.interface.declarations import classImplements
+    # From lest specific to most specific.
+    from zope.interface.interfaces import IElement
+    classImplements(Element, IElement)
 
-##############################################################################
+    from zope.interface.interfaces import IAttribute
+    classImplements(Attribute, IAttribute)
 
-def _normalizeargs(sequence, output=None):
-    """Normalize declaration arguments
+    from zope.interface.interfaces import IMethod
+    classImplements(Method, IMethod)
 
-    Normalization arguments might contain Declarions, tuples, or single
-    interfaces.
+    from zope.interface.interfaces import ISpecification
+    classImplements(Specification, ISpecification)
 
-    Anything but individual interfaces or implements specs will be expanded.
-    """
-    if output is None:
-        output = []
+    from zope.interface.interfaces import IInterface
+    classImplements(InterfaceClass, IInterface)
 
-    cls = sequence.__class__
-    if InterfaceClass in cls.__mro__ or Implements in cls.__mro__:
-        output.append(sequence)
-    else:
-        for v in sequence:
-            _normalizeargs(v, output)
 
-    return output
+# We import this here to deal with module dependencies.
+# pylint:disable=wrong-import-position
+from zope.interface.declarations import implementedBy
+from zope.interface.declarations import providedBy
+from zope.interface.exceptions import BrokenImplementation
+from zope.interface.exceptions import InvalidInterface
 
-_empty = _ImmutableDeclaration()
 
-objectSpecificationDescriptor = ObjectSpecificationDescriptor()
+# This ensures that ``Interface`` winds up in the flattened()
+# list of the immutable declaration. It correctly overrides changed()
+# as a no-op, so we bypass that.
+from zope.interface.declarations import _empty
+Specification.changed(_empty, _empty)
```

### Comparing `zope_interface-6.4/src/zope/interface/document.py` & `zope.interface-6.4.post0/src/zope/interface/document.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/exceptions.py` & `zope.interface-6.4.post0/src/zope/interface/exceptions.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/interfaces.py` & `zope.interface-6.4.post0/src/zope/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/registry.py` & `zope.interface-6.4.post0/src/zope/interface/registry.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/ro.py` & `zope.interface-6.4.post0/src/zope/interface/ro.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/__init__.py` & `zope.interface-6.4.post0/src/zope/interface/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/advisory_testing.py` & `zope.interface-6.4.post0/src/zope/interface/tests/advisory_testing.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/dummy.py` & `zope.interface-6.4.post0/src/zope/interface/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/idummy.py` & `zope.interface-6.4.post0/src/zope/interface/tests/idummy.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/m1.py` & `zope.interface-6.4.post0/src/zope/interface/tests/m1.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/odd.py` & `zope.interface-6.4.post0/src/zope/interface/tests/odd.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_adapter.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_advice.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_advice.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_compile_flags.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_declarations.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_declarations.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_document.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_element.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_exceptions.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_interface.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_interfaces.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_odd_declarations.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_odd_declarations.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_registry.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_ro.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_ro.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_sorting.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/tests/test_verify.py` & `zope.interface-6.4.post0/src/zope/interface/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope/interface/verify.py` & `zope.interface-6.4.post0/src/zope/interface/verify.py`

 * *Files identical despite different names*

### Comparing `zope_interface-6.4/src/zope.interface.egg-info/PKG-INFO` & `zope.interface-6.4.post0/src/zope.interface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.interface
-Version: 6.4
+Version: 6.4.post0
 Summary: Interfaces for Python
 Home-page: https://github.com/zopefoundation/zope.interface
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: interface,components,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,14 +71,24 @@
 
 For detailed documentation, please see https://zopeinterface.readthedocs.io/en/latest/
 
 =========
  Changes
 =========
 
+6.4.post0 (2024-05-22)
+======================
+
+- The sdist of version 6.4 was uploaded to PyPI as
+  ``zope_interface-6.4.tar.gz`` instead of ``zope.interface-6.4-py2.tar.gz``
+  which cannot be installed by ``zc.buildout``.  This release is a re-release
+  of version 6.4 with the correct sdist name.
+  (`#298 <https://github.com/zopefoundation/zope.interface/issues/298>`)
+
+
 6.4 (2024-05-15)
 ================
 
 - Adjust for incompatible changes in Python 3.13b1.
   (`#292 <https://github.com/zopefoundation/zope.interface/issues/292>`)
 
 - Build windows wheels on GHA.
```

### Comparing `zope_interface-6.4/tox.ini` & `zope.interface-6.4.post0/tox.ini`

 * *Files identical despite different names*

