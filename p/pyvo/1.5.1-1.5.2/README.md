# Comparing `tmp/pyvo-1.5.1.tar.gz` & `tmp/pyvo-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvo-1.5.1.tar", last modified: Fri Feb 23 15:38:44 2024, max compression
+gzip compressed data, was "pyvo-1.5.2.tar", last modified: Wed May 22 06:47:30 2024, max compression
```

## Comparing `pyvo-1.5.1.tar` & `pyvo-1.5.2.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.934212 pyvo-1.5.1/
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.888726 pyvo-1.5.1/.github/
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.894061 pyvo-1.5.1/.github/workflows/
--rw-r--r--   0 bsipocz    (503) staff       (20)      521 2023-12-01 18:42:09.000000 pyvo-1.5.1/.github/workflows/changelog.yml
--rw-r--r--   0 bsipocz    (503) staff       (20)      872 2023-12-01 18:42:09.000000 pyvo-1.5.1/.github/workflows/ci_devtests.yml
--rw-r--r--   0 bsipocz    (503) staff       (20)     2193 2023-12-01 18:42:09.000000 pyvo-1.5.1/.github/workflows/ci_tests.yml
--rw-r--r--   0 bsipocz    (503) staff       (20)      723 2023-09-18 21:13:09.000000 pyvo-1.5.1/.gitignore
--rw-r--r--   0 bsipocz    (503) staff       (20)     1063 2024-02-22 04:36:53.000000 pyvo-1.5.1/.mailmap
--rw-r--r--   0 bsipocz    (503) staff       (20)      532 2023-12-01 18:42:09.000000 pyvo-1.5.1/.readthedocs.yml
--rw-r--r--   0 bsipocz    (503) staff       (20)     9354 2024-02-22 04:45:04.000000 pyvo-1.5.1/CHANGES.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)      948 2022-10-05 02:13:41.000000 pyvo-1.5.1/CONTRIBUTORS.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)     1532 2022-10-05 02:13:41.000000 pyvo-1.5.1/LICENSE.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)      255 2023-09-20 19:34:01.000000 pyvo-1.5.1/MANIFEST.in
--rw-r--r--   0 bsipocz    (503) staff       (20)     4697 2024-02-23 15:38:44.934142 pyvo-1.5.1/PKG-INFO
--rw-r--r--   0 bsipocz    (503) staff       (20)     3581 2023-09-20 19:34:01.000000 pyvo-1.5.1/README.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)      849 2022-10-05 02:13:41.000000 pyvo-1.5.1/RELEASE.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)     2116 2023-12-05 05:13:36.000000 pyvo-1.5.1/conftest.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.894816 pyvo-1.5.1/docs/
--rw-r--r--   0 bsipocz    (503) staff       (20)     4724 2022-10-05 02:13:41.000000 pyvo-1.5.1/docs/Makefile
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.888892 pyvo-1.5.1/docs/_templates/
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.895250 pyvo-1.5.1/docs/_templates/autosummary/
--rw-r--r--   0 bsipocz    (503) staff       (20)      250 2022-10-05 02:13:41.000000 pyvo-1.5.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)      251 2022-10-05 02:13:41.000000 pyvo-1.5.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)      252 2022-10-05 02:13:41.000000 pyvo-1.5.1/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.895377 pyvo-1.5.1/docs/auth/
--rw-r--r--   0 bsipocz    (503) staff       (20)      268 2024-02-22 04:36:53.000000 pyvo-1.5.1/docs/auth/index.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)     6726 2024-02-22 04:36:53.000000 pyvo-1.5.1/docs/conf.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.895474 pyvo-1.5.1/docs/dal/
--rw-r--r--   0 bsipocz    (503) staff       (20)    31498 2024-02-22 04:36:53.000000 pyvo-1.5.1/docs/dal/index.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)     3745 2024-02-22 04:36:53.000000 pyvo-1.5.1/docs/index.rst
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.895804 pyvo-1.5.1/docs/io/
--rw-r--r--   0 bsipocz    (503) staff       (20)      191 2024-02-22 04:36:53.000000 pyvo-1.5.1/docs/io/index.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)      167 2024-02-22 04:36:53.000000 pyvo-1.5.1/docs/io/uws.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)      308 2024-02-22 04:36:53.000000 pyvo-1.5.1/docs/io/vosi.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)     4513 2022-10-05 02:13:41.000000 pyvo-1.5.1/docs/make.bat
--rw-r--r--   0 bsipocz    (503) staff       (20)      523 2024-02-22 04:36:53.000000 pyvo-1.5.1/docs/nitpick-exceptions
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.895910 pyvo-1.5.1/docs/registry/
--rw-r--r--   0 bsipocz    (503) staff       (20)    24797 2024-02-22 04:45:04.000000 pyvo-1.5.1/docs/registry/index.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)      182 2022-10-05 02:13:41.000000 pyvo-1.5.1/docs/requirements.txt
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.896147 pyvo-1.5.1/docs/utils/
--rw-r--r--   0 bsipocz    (503) staff       (20)      319 2024-02-22 04:36:53.000000 pyvo-1.5.1/docs/utils/index.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)     4267 2024-02-22 04:36:53.000000 pyvo-1.5.1/docs/utils/prototypes.rst
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.896590 pyvo-1.5.1/licenses/
--rw-r--r--   0 bsipocz    (503) staff       (20)     1496 2022-10-05 02:13:41.000000 pyvo-1.5.1/licenses/ASTROPY_LICENSE.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)     1513 2022-10-05 02:13:41.000000 pyvo-1.5.1/licenses/LICENSE.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)      162 2022-10-05 02:13:41.000000 pyvo-1.5.1/licenses/README.rst
--rw-r--r--   0 bsipocz    (503) staff       (20)      181 2023-12-01 18:42:09.000000 pyvo-1.5.1/pyproject.toml
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.897550 pyvo-1.5.1/pyvo/
--rw-r--r--   0 bsipocz    (503) staff       (20)     1391 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      355 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/_astropy_init.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.898802 pyvo-1.5.1/pyvo/auth/
--rw-r--r--   0 bsipocz    (503) staff       (20)      236 2023-01-27 20:23:20.000000 pyvo-1.5.1/pyvo/auth/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     3694 2024-02-22 04:36:53.000000 pyvo-1.5.1/pyvo/auth/authsession.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     3924 2024-02-22 04:36:53.000000 pyvo-1.5.1/pyvo/auth/authurls.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     4878 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/auth/credentialstore.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      161 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/auth/securitymethods.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.899288 pyvo-1.5.1/pyvo/auth/tests/
--rw-r--r--   0 bsipocz    (503) staff       (20)       64 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/auth/tests/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      694 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/auth/tests/conftest.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.889538 pyvo-1.5.1/pyvo/auth/tests/data/
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.899545 pyvo-1.5.1/pyvo/auth/tests/data/tap/
--rw-r--r--   0 bsipocz    (503) staff       (20)     3653 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/auth/tests/data/tap/capabilities.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     6816 2023-12-19 20:39:11.000000 pyvo-1.5.1/pyvo/auth/tests/test_auth.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     1399 2023-12-05 05:13:36.000000 pyvo-1.5.1/pyvo/conftest.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.901498 pyvo-1.5.1/pyvo/dal/
--rw-r--r--   0 bsipocz    (503) staff       (20)     1517 2024-02-22 04:36:53.000000 pyvo-1.5.1/pyvo/dal/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    33878 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/adhoc.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     7180 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/dbapi2.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     7557 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/exceptions.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     3366 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/mimetype.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    14486 2023-12-01 18:42:09.000000 pyvo-1.5.1/pyvo/dal/params.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    34097 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/query.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    18999 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/scs.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    33137 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/sia.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    40015 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/sia2.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    15834 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/sla.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    26486 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/ssa.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    38480 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/tap.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.904295 pyvo-1.5.1/pyvo/dal/tests/
--rw-r--r--   0 bsipocz    (503) staff       (20)       64 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      694 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/conftest.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.904468 pyvo-1.5.1/pyvo/dal/tests/data/
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.906350 pyvo-1.5.1/pyvo/dal/tests/data/datalink/
--rw-r--r--   0 bsipocz    (503) staff       (20)    11324 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/datalink/cutout1.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     6297 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/datalink/cutout2.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)    13183 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/dal/tests/data/datalink/datalink-obscore.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)    21219 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/dal/tests/data/datalink/datalink-ssa.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     5449 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/dal/tests/data/datalink/datalink.desise
--rw-r--r--   0 bsipocz    (503) staff       (20)     5877 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/datalink/datalink.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     8068 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/dal/tests/data/datalink/proc.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     7278 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/datalink/proc_inf.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     7280 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/datalink/proc_units.xml
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.906834 pyvo-1.5.1/pyvo/dal/tests/data/mimetype/
--rw-r--r--   0 bsipocz    (503) staff       (20)    12589 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/mimetype/ivoa_logo.jpg
--rw-r--r--   0 bsipocz    (503) staff       (20)    31680 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/dal/tests/data/mimetype/test.fits
--rw-r--r--   0 bsipocz    (503) staff       (20)     8263 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/monkeypatch.xml
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.908229 pyvo-1.5.1/pyvo/dal/tests/data/query/
--rw-r--r--   0 bsipocz    (503) staff       (20)      901 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/data/query/basic.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     1144 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/data/query/dataset.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      907 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/data/query/errorstatus.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      901 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/data/query/firstresource.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      610 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/data/query/missingcolumns.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      355 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/data/query/missingresource.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      472 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/data/query/missingtable.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      958 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/data/query/overflowstatus.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      900 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/data/query/rootinfo.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      902 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/data/query/tableinfo.xml
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.908353 pyvo-1.5.1/pyvo/dal/tests/data/querydata/
--rw-r--r--   0 bsipocz    (503) staff       (20)   532800 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/dal/tests/data/querydata/image.fits
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.909496 pyvo-1.5.1/pyvo/dal/tests/data/scs/
--rw-r--r--   0 bsipocz    (503) staff       (20)   117973 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/scs/result.xml
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.909971 pyvo-1.5.1/pyvo/dal/tests/data/sia/
--rw-r--r--   0 bsipocz    (503) staff       (20)     3235 2023-12-01 18:42:09.000000 pyvo-1.5.1/pyvo/dal/tests/data/sia/dataset.xml
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.910706 pyvo-1.5.1/pyvo/dal/tests/data/sia2/
--rw-r--r--   0 bsipocz    (503) staff       (20)     1034 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/sia2/capabilities-basicauth.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     1199 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/sia2/capabilities-newformat.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     1492 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/sia2/capabilities-priv.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     1649 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/sia2/capabilities.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)    10174 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/sia2/dataset.xml
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.910884 pyvo-1.5.1/pyvo/dal/tests/data/sla/
--rw-r--r--   0 bsipocz    (503) staff       (20)    11363 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/sla/dataset.xml
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.911099 pyvo-1.5.1/pyvo/dal/tests/data/ssa/
--rw-r--r--   0 bsipocz    (503) staff       (20)    40667 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/ssa/result.xml
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.912351 pyvo-1.5.1/pyvo/dal/tests/data/tap/
--rw-r--r--   0 bsipocz    (503) staff       (20)    11989 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/tap/capabilities.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     4471 2023-12-01 18:42:09.000000 pyvo-1.5.1/pyvo/dal/tests/data/tap/examples.htm
--rw-r--r--   0 bsipocz    (503) staff       (20)      731 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/tap/lazy-table1.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     1427 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/tap/lazy-table2.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     1852 2023-12-01 18:42:09.000000 pyvo-1.5.1/pyvo/dal/tests/data/tap/obscore-examples.html
--rw-r--r--   0 bsipocz    (503) staff       (20)    26255 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/tap/obscore-image.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      729 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/data/tap/tables.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     4482 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/make_testdata.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     8367 2023-12-01 18:42:09.000000 pyvo-1.5.1/pyvo/dal/tests/test_adhoc.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     6981 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/test_datalink.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     1640 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/dal/tests/test_mimetype.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      387 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dal/tests/test_monkeypatch.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     7391 2023-12-01 18:42:09.000000 pyvo-1.5.1/pyvo/dal/tests/test_params.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    16679 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/tests/test_query.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     1352 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/tests/test_scs.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     2014 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/tests/test_sia.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     7835 2023-12-05 05:13:36.000000 pyvo-1.5.1/pyvo/dal/tests/test_sia2.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     9242 2023-12-05 05:13:36.000000 pyvo-1.5.1/pyvo/dal/tests/test_sia2_remote.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     1303 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/tests/test_sla.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     1216 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/tests/test_ssa.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    30399 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/tests/test_tap.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     6399 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/dal/vosi.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.912723 pyvo-1.5.1/pyvo/dam/
--rw-r--r--   0 bsipocz    (503) staff       (20)      118 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/dam/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     2944 2022-10-07 18:49:41.000000 pyvo-1.5.1/pyvo/dam/obscore.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.912963 pyvo-1.5.1/pyvo/io/
--rw-r--r--   0 bsipocz    (503) staff       (20)       64 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/__init__.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.913458 pyvo-1.5.1/pyvo/io/uws/
--rw-r--r--   0 bsipocz    (503) staff       (20)      162 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/io/uws/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     4227 2024-02-22 04:36:53.000000 pyvo-1.5.1/pyvo/io/uws/endpoint.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.913657 pyvo-1.5.1/pyvo/io/uws/tests/
--rw-r--r--   0 bsipocz    (503) staff       (20)        0 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/uws/tests/__init__.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.914256 pyvo-1.5.1/pyvo/io/uws/tests/data/
--rw-r--r--   0 bsipocz    (503) staff       (20)     1337 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/uws/tests/data/job-error.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      856 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/uws/tests/data/job-implicit-v1.0.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     1326 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/uws/tests/data/job.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      878 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/io/uws/tests/test_job.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    11996 2024-02-22 04:36:53.000000 pyvo-1.5.1/pyvo/io/uws/tree.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.917119 pyvo-1.5.1/pyvo/io/vosi/
--rw-r--r--   0 bsipocz    (503) staff       (20)      139 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     1807 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/availability.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    11777 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/io/vosi/endpoint.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    14420 2023-12-15 19:57:55.000000 pyvo-1.5.1/pyvo/io/vosi/exceptions.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    17162 2023-12-15 19:57:55.000000 pyvo-1.5.1/pyvo/io/vosi/tapregext.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.917994 pyvo-1.5.1/pyvo/io/vosi/tests/
--rw-r--r--   0 bsipocz    (503) staff       (20)       64 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/__init__.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.918674 pyvo-1.5.1/pyvo/io/vosi/tests/data/
--rw-r--r--   0 bsipocz    (503) staff       (20)      613 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/availability.xml
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.918846 pyvo-1.5.1/pyvo/io/vosi/tests/data/capabilities/
--rw-r--r--   0 bsipocz    (503) staff       (20)     1160 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/capabilities/multiple_capa_descriptions.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     4087 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/capabilities.xml
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.924759 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/
--rw-r--r--   0 bsipocz    (503) staff       (20)     4578 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/datatypes_tap.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     3944 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/datatypes_votable.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      780 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_column_datatypes.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      743 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_column_descriptions.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      690 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_column_names.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      711 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_column_ucds.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      716 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_column_units.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      721 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_column_utypes.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     1033 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_foreignkey_descriptions.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     1011 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_foreignkey_utypes.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      997 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_fromcolumns.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      641 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_schema_descriptions.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      580 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_schema_names.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      611 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_schema_titles.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      611 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_schema_utypes.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      690 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_table_descriptions.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      631 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_table_names.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      660 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_table_titles.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      660 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_table_utypes.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     1003 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_targetcolumns.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      999 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_targettables.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      844 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/no_fromcolumn.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      538 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/no_schema_name.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      515 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/no_schemas.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      616 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/no_table_description.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      580 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/no_table_name.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      899 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/no_targetcolumn.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      688 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/single_table_description.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      754 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/sizenegative.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      775 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/wrong_arraysize.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      744 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/wrong_datatypes_tap.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      752 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/wrong_datatypes_votable.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      788 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/wrong_flag.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     1454 2023-12-15 19:57:55.000000 pyvo-1.5.1/pyvo/io/vosi/tests/data/tables.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)      675 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/io/vosi/tests/test_availability.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     8210 2023-12-01 18:42:09.000000 pyvo-1.5.1/pyvo/io/vosi/tests/test_capabilities.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    14637 2023-12-15 19:57:55.000000 pyvo-1.5.1/pyvo/io/vosi/tests/test_tables.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    31423 2024-02-22 04:36:53.000000 pyvo-1.5.1/pyvo/io/vosi/vodataservice.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    15412 2024-02-22 04:36:53.000000 pyvo-1.5.1/pyvo/io/vosi/voresource.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.925152 pyvo-1.5.1/pyvo/registry/
--rw-r--r--   0 bsipocz    (503) staff       (20)      699 2024-02-22 04:36:53.000000 pyvo-1.5.1/pyvo/registry/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    39284 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/registry/regtap.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    34996 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/registry/rtcons.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.926276 pyvo-1.5.1/pyvo/registry/tests/
--rw-r--r--   0 bsipocz    (503) staff       (20)       64 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/registry/tests/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     2127 2023-12-15 19:57:55.000000 pyvo-1.5.1/pyvo/registry/tests/commonfixtures.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      694 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/registry/tests/conftest.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.927166 pyvo-1.5.1/pyvo/registry/tests/data/
--rw-r--r--   0 bsipocz    (503) staff       (20)       98 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/registry/tests/data/README
--rw-r--r--   0 bsipocz    (503) staff       (20)     4275 2023-12-15 19:57:55.000000 pyvo-1.5.1/pyvo/registry/tests/data/capabilities.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)     2528 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/registry/tests/data/messenger.desise
--rw-r--r--   0 bsipocz    (503) staff       (20)    11493 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/registry/tests/data/multi-interface.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)   214229 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/registry/tests/data/regtap.xml
--rw-r--r--   0 bsipocz    (503) staff       (20)    32124 2024-02-22 04:45:04.000000 pyvo-1.5.1/pyvo/registry/tests/test_regtap.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    22245 2024-02-22 04:45:37.000000 pyvo-1.5.1/pyvo/registry/tests/test_rtcons.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     3434 2023-12-01 18:42:09.000000 pyvo-1.5.1/pyvo/samp.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.929338 pyvo-1.5.1/pyvo/utils/
--rw-r--r--   0 bsipocz    (503) staff       (20)       82 2023-10-20 17:42:34.000000 pyvo-1.5.1/pyvo/utils/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      127 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/utils/compat.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      570 2023-09-18 21:13:09.000000 pyvo-1.5.1/pyvo/utils/decorators.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     1886 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/utils/formatting.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      681 2023-12-01 18:42:09.000000 pyvo-1.5.1/pyvo/utils/http.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     2076 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/utils/protofeature.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     4203 2023-12-05 05:13:36.000000 pyvo-1.5.1/pyvo/utils/prototype.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.930787 pyvo-1.5.1/pyvo/utils/tests/
--rw-r--r--   0 bsipocz    (503) staff       (20)       64 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/utils/tests/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      395 2023-12-01 18:42:09.000000 pyvo-1.5.1/pyvo/utils/tests/test_http.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     4007 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/utils/tests/test_prototype.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      309 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/utils/tests/test_url.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     3299 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/utils/tests/test_vocabularies_remote.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      641 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/utils/url.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     2261 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/utils/vocabularies.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.932836 pyvo-1.5.1/pyvo/utils/xml/
--rw-r--r--   0 bsipocz    (503) staff       (20)        0 2022-10-05 02:13:41.000000 pyvo-1.5.1/pyvo/utils/xml/__init__.py
--rw-r--r--   0 bsipocz    (503) staff       (20)    15183 2023-09-20 19:34:01.000000 pyvo-1.5.1/pyvo/utils/xml/elements.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     1094 2022-10-07 18:49:41.000000 pyvo-1.5.1/pyvo/utils/xml/exceptions.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.933089 pyvo-1.5.1/pyvo/utils/xml/tests/
--rw-r--r--   0 bsipocz    (503) staff       (20)     2935 2023-12-15 19:57:55.000000 pyvo-1.5.1/pyvo/utils/xml/tests/test_elements.py
--rw-r--r--   0 bsipocz    (503) staff       (20)      337 2024-02-23 15:38:44.000000 pyvo-1.5.1/pyvo/version.py
-drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-02-23 15:38:44.933386 pyvo-1.5.1/pyvo.egg-info/
--rw-r--r--   0 bsipocz    (503) staff       (20)     4697 2024-02-23 15:38:44.000000 pyvo-1.5.1/pyvo.egg-info/PKG-INFO
--rw-r--r--   0 bsipocz    (503) staff       (20)     7166 2024-02-23 15:38:44.000000 pyvo-1.5.1/pyvo.egg-info/SOURCES.txt
--rw-r--r--   0 bsipocz    (503) staff       (20)        1 2024-02-23 15:38:44.000000 pyvo-1.5.1/pyvo.egg-info/dependency_links.txt
--rw-r--r--   0 bsipocz    (503) staff       (20)        1 2024-02-23 15:38:44.000000 pyvo-1.5.1/pyvo.egg-info/not-zip-safe
--rw-r--r--   0 bsipocz    (503) staff       (20)      121 2024-02-23 15:38:44.000000 pyvo-1.5.1/pyvo.egg-info/requires.txt
--rw-r--r--   0 bsipocz    (503) staff       (20)        5 2024-02-23 15:38:44.000000 pyvo-1.5.1/pyvo.egg-info/top_level.txt
--rw-r--r--   0 bsipocz    (503) staff       (20)     2486 2024-02-23 15:38:44.934645 pyvo-1.5.1/setup.cfg
--rw-r--r--   0 bsipocz    (503) staff       (20)     1953 2023-09-18 21:13:09.000000 pyvo-1.5.1/setup.py
--rw-r--r--   0 bsipocz    (503) staff       (20)     1960 2023-12-05 05:13:36.000000 pyvo-1.5.1/tox.ini
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.989546 pyvo-1.5.2/
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.927045 pyvo-1.5.2/.github/
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.938054 pyvo-1.5.2/.github/workflows/
+-rw-r--r--   0 bsipocz    (503) staff       (20)      521 2023-12-01 18:42:09.000000 pyvo-1.5.2/.github/workflows/changelog.yml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      872 2024-05-22 06:12:57.000000 pyvo-1.5.2/.github/workflows/ci_devtests.yml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     2193 2024-05-22 06:12:57.000000 pyvo-1.5.2/.github/workflows/ci_tests.yml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      723 2024-05-22 06:12:32.000000 pyvo-1.5.2/.gitignore
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1063 2024-05-22 06:00:58.000000 pyvo-1.5.2/.mailmap
+-rw-r--r--   0 bsipocz    (503) staff       (20)      532 2023-12-01 18:42:09.000000 pyvo-1.5.2/.readthedocs.yml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     9572 2024-05-22 06:47:08.000000 pyvo-1.5.2/CHANGES.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)      948 2022-10-05 02:13:41.000000 pyvo-1.5.2/CONTRIBUTORS.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1532 2022-10-05 02:13:41.000000 pyvo-1.5.2/LICENSE.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)      255 2023-09-20 19:34:01.000000 pyvo-1.5.2/MANIFEST.in
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4697 2024-05-22 06:47:30.989418 pyvo-1.5.2/PKG-INFO
+-rw-r--r--   0 bsipocz    (503) staff       (20)     3581 2023-09-20 19:34:01.000000 pyvo-1.5.2/README.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)      849 2022-10-05 02:13:41.000000 pyvo-1.5.2/RELEASE.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)     2116 2024-05-22 06:12:32.000000 pyvo-1.5.2/conftest.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.939846 pyvo-1.5.2/docs/
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4724 2022-10-05 02:13:41.000000 pyvo-1.5.2/docs/Makefile
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.927336 pyvo-1.5.2/docs/_templates/
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.940516 pyvo-1.5.2/docs/_templates/autosummary/
+-rw-r--r--   0 bsipocz    (503) staff       (20)      250 2022-10-05 02:13:41.000000 pyvo-1.5.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)      251 2022-10-05 02:13:41.000000 pyvo-1.5.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)      252 2022-10-05 02:13:41.000000 pyvo-1.5.2/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.940735 pyvo-1.5.2/docs/auth/
+-rw-r--r--   0 bsipocz    (503) staff       (20)      268 2024-05-07 00:19:42.000000 pyvo-1.5.2/docs/auth/index.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)     6726 2024-05-07 00:19:42.000000 pyvo-1.5.2/docs/conf.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.940960 pyvo-1.5.2/docs/dal/
+-rw-r--r--   0 bsipocz    (503) staff       (20)    31536 2024-05-22 06:12:57.000000 pyvo-1.5.2/docs/dal/index.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)     3745 2024-05-22 06:12:32.000000 pyvo-1.5.2/docs/index.rst
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.941827 pyvo-1.5.2/docs/io/
+-rw-r--r--   0 bsipocz    (503) staff       (20)      191 2024-05-07 00:19:42.000000 pyvo-1.5.2/docs/io/index.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)      167 2024-05-07 00:19:42.000000 pyvo-1.5.2/docs/io/uws.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)      308 2024-05-07 00:19:42.000000 pyvo-1.5.2/docs/io/vosi.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4513 2022-10-05 02:13:41.000000 pyvo-1.5.2/docs/make.bat
+-rw-r--r--   0 bsipocz    (503) staff       (20)      523 2024-05-07 00:19:42.000000 pyvo-1.5.2/docs/nitpick-exceptions
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.942115 pyvo-1.5.2/docs/registry/
+-rw-r--r--   0 bsipocz    (503) staff       (20)    24824 2024-05-22 06:17:16.000000 pyvo-1.5.2/docs/registry/index.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)      182 2022-10-05 02:13:41.000000 pyvo-1.5.2/docs/requirements.txt
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.943300 pyvo-1.5.2/docs/utils/
+-rw-r--r--   0 bsipocz    (503) staff       (20)      319 2024-05-07 00:19:42.000000 pyvo-1.5.2/docs/utils/index.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4267 2024-05-07 00:19:42.000000 pyvo-1.5.2/docs/utils/prototypes.rst
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.944329 pyvo-1.5.2/licenses/
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1496 2022-10-05 02:13:41.000000 pyvo-1.5.2/licenses/ASTROPY_LICENSE.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1513 2022-10-05 02:13:41.000000 pyvo-1.5.2/licenses/LICENSE.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)      162 2022-10-05 02:13:41.000000 pyvo-1.5.2/licenses/README.rst
+-rw-r--r--   0 bsipocz    (503) staff       (20)      181 2023-12-01 18:42:09.000000 pyvo-1.5.2/pyproject.toml
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.945886 pyvo-1.5.2/pyvo/
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1391 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      355 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/_astropy_init.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.947590 pyvo-1.5.2/pyvo/auth/
+-rw-r--r--   0 bsipocz    (503) staff       (20)      236 2023-01-27 20:23:20.000000 pyvo-1.5.2/pyvo/auth/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     3694 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/auth/authsession.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     3924 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/auth/authurls.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4878 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/auth/credentialstore.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      161 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/auth/securitymethods.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.948494 pyvo-1.5.2/pyvo/auth/tests/
+-rw-r--r--   0 bsipocz    (503) staff       (20)       64 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/auth/tests/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      694 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/auth/tests/conftest.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.928186 pyvo-1.5.2/pyvo/auth/tests/data/
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.948735 pyvo-1.5.2/pyvo/auth/tests/data/tap/
+-rw-r--r--   0 bsipocz    (503) staff       (20)     3653 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/auth/tests/data/tap/capabilities.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     6816 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/auth/tests/test_auth.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1399 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/conftest.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.954296 pyvo-1.5.2/pyvo/dal/
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1517 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/dal/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    33875 2024-05-22 06:12:56.000000 pyvo-1.5.2/pyvo/dal/adhoc.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     7180 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/dal/dbapi2.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     7557 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/dal/exceptions.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     3366 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/dal/mimetype.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    14486 2023-12-01 18:42:09.000000 pyvo-1.5.2/pyvo/dal/params.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    34097 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/dal/query.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    18999 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/dal/scs.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    33762 2024-05-22 06:42:36.000000 pyvo-1.5.2/pyvo/dal/sia.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    40015 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/dal/sia2.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    15834 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/dal/sla.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    26660 2024-05-22 06:17:16.000000 pyvo-1.5.2/pyvo/dal/ssa.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    38511 2024-05-22 06:12:57.000000 pyvo-1.5.2/pyvo/dal/tap.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.958928 pyvo-1.5.2/pyvo/dal/tests/
+-rw-r--r--   0 bsipocz    (503) staff       (20)       64 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      694 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/dal/tests/conftest.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.959248 pyvo-1.5.2/pyvo/dal/tests/data/
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.961622 pyvo-1.5.2/pyvo/dal/tests/data/datalink/
+-rw-r--r--   0 bsipocz    (503) staff       (20)    11324 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/datalink/cutout1.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     6297 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/datalink/cutout2.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)    13183 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/dal/tests/data/datalink/datalink-obscore.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)    21219 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/dal/tests/data/datalink/datalink-ssa.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     5449 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/dal/tests/data/datalink/datalink.desise
+-rw-r--r--   0 bsipocz    (503) staff       (20)     5877 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/datalink/datalink.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     8068 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/dal/tests/data/datalink/proc.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     7278 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/datalink/proc_inf.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     7280 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/datalink/proc_units.xml
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.962147 pyvo-1.5.2/pyvo/dal/tests/data/mimetype/
+-rw-r--r--   0 bsipocz    (503) staff       (20)    12589 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/mimetype/ivoa_logo.jpg
+-rw-r--r--   0 bsipocz    (503) staff       (20)    31680 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/dal/tests/data/mimetype/test.fits
+-rw-r--r--   0 bsipocz    (503) staff       (20)     8263 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/monkeypatch.xml
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.964371 pyvo-1.5.2/pyvo/dal/tests/data/query/
+-rw-r--r--   0 bsipocz    (503) staff       (20)      901 2024-05-07 05:09:38.000000 pyvo-1.5.2/pyvo/dal/tests/data/query/basic.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1144 2024-05-07 05:09:38.000000 pyvo-1.5.2/pyvo/dal/tests/data/query/dataset.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      907 2024-05-07 05:09:38.000000 pyvo-1.5.2/pyvo/dal/tests/data/query/errorstatus.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      901 2024-05-07 05:09:38.000000 pyvo-1.5.2/pyvo/dal/tests/data/query/firstresource.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      610 2024-05-07 05:09:38.000000 pyvo-1.5.2/pyvo/dal/tests/data/query/missingcolumns.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      355 2024-05-07 05:09:38.000000 pyvo-1.5.2/pyvo/dal/tests/data/query/missingresource.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      472 2024-05-07 05:09:38.000000 pyvo-1.5.2/pyvo/dal/tests/data/query/missingtable.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      958 2024-05-07 05:09:38.000000 pyvo-1.5.2/pyvo/dal/tests/data/query/overflowstatus.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      900 2024-05-07 05:09:38.000000 pyvo-1.5.2/pyvo/dal/tests/data/query/rootinfo.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      902 2024-05-07 05:09:38.000000 pyvo-1.5.2/pyvo/dal/tests/data/query/tableinfo.xml
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.964509 pyvo-1.5.2/pyvo/dal/tests/data/querydata/
+-rw-r--r--   0 bsipocz    (503) staff       (20)   532800 2024-05-07 05:09:38.000000 pyvo-1.5.2/pyvo/dal/tests/data/querydata/image.fits
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.965914 pyvo-1.5.2/pyvo/dal/tests/data/scs/
+-rw-r--r--   0 bsipocz    (503) staff       (20)   117973 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/scs/result.xml
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.966675 pyvo-1.5.2/pyvo/dal/tests/data/sia/
+-rw-r--r--   0 bsipocz    (503) staff       (20)     3658 2024-05-22 06:17:16.000000 pyvo-1.5.2/pyvo/dal/tests/data/sia/dataset.xml
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.967645 pyvo-1.5.2/pyvo/dal/tests/data/sia2/
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1034 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/sia2/capabilities-basicauth.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1199 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/sia2/capabilities-newformat.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1492 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/sia2/capabilities-priv.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1649 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/sia2/capabilities.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)    10174 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/sia2/dataset.xml
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.967866 pyvo-1.5.2/pyvo/dal/tests/data/sla/
+-rw-r--r--   0 bsipocz    (503) staff       (20)    11363 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/sla/dataset.xml
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.968124 pyvo-1.5.2/pyvo/dal/tests/data/ssa/
+-rw-r--r--   0 bsipocz    (503) staff       (20)    41603 2024-05-22 06:17:16.000000 pyvo-1.5.2/pyvo/dal/tests/data/ssa/result.xml
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.969695 pyvo-1.5.2/pyvo/dal/tests/data/tap/
+-rw-r--r--   0 bsipocz    (503) staff       (20)    11989 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/tap/capabilities.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4471 2023-12-01 18:42:09.000000 pyvo-1.5.2/pyvo/dal/tests/data/tap/examples.htm
+-rw-r--r--   0 bsipocz    (503) staff       (20)      731 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/tap/lazy-table1.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1427 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/tap/lazy-table2.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1852 2023-12-01 18:42:09.000000 pyvo-1.5.2/pyvo/dal/tests/data/tap/obscore-examples.html
+-rw-r--r--   0 bsipocz    (503) staff       (20)    26255 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/tap/obscore-image.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      729 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/data/tap/tables.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4482 2024-05-07 05:12:29.000000 pyvo-1.5.2/pyvo/dal/tests/make_testdata.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     8367 2023-12-01 18:42:09.000000 pyvo-1.5.2/pyvo/dal/tests/test_adhoc.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     6981 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/dal/tests/test_datalink.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1640 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/dal/tests/test_mimetype.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      387 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dal/tests/test_monkeypatch.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     7391 2023-12-01 18:42:09.000000 pyvo-1.5.2/pyvo/dal/tests/test_params.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    16679 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/dal/tests/test_query.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1352 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/dal/tests/test_scs.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     2930 2024-05-22 06:42:36.000000 pyvo-1.5.2/pyvo/dal/tests/test_sia.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     7835 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/dal/tests/test_sia2.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     9242 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/dal/tests/test_sia2_remote.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1303 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/dal/tests/test_sla.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1259 2024-05-22 06:17:16.000000 pyvo-1.5.2/pyvo/dal/tests/test_ssa.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    30399 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/dal/tests/test_tap.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     6399 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/dal/vosi.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.970031 pyvo-1.5.2/pyvo/dam/
+-rw-r--r--   0 bsipocz    (503) staff       (20)      118 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/dam/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     2944 2022-10-07 18:49:41.000000 pyvo-1.5.2/pyvo/dam/obscore.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.970450 pyvo-1.5.2/pyvo/io/
+-rw-r--r--   0 bsipocz    (503) staff       (20)       64 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/__init__.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.971078 pyvo-1.5.2/pyvo/io/uws/
+-rw-r--r--   0 bsipocz    (503) staff       (20)      162 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/io/uws/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4227 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/io/uws/endpoint.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.971411 pyvo-1.5.2/pyvo/io/uws/tests/
+-rw-r--r--   0 bsipocz    (503) staff       (20)        0 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/uws/tests/__init__.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.972045 pyvo-1.5.2/pyvo/io/uws/tests/data/
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1337 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/uws/tests/data/job-error.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      856 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/uws/tests/data/job-implicit-v1.0.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1326 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/uws/tests/data/job.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      878 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/io/uws/tests/test_job.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    11996 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/io/uws/tree.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.973771 pyvo-1.5.2/pyvo/io/vosi/
+-rw-r--r--   0 bsipocz    (503) staff       (20)      139 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1807 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/availability.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    11777 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/io/vosi/endpoint.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    14420 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/io/vosi/exceptions.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    17273 2024-05-22 06:12:57.000000 pyvo-1.5.2/pyvo/io/vosi/tapregext.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.974702 pyvo-1.5.2/pyvo/io/vosi/tests/
+-rw-r--r--   0 bsipocz    (503) staff       (20)       64 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/__init__.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.975272 pyvo-1.5.2/pyvo/io/vosi/tests/data/
+-rw-r--r--   0 bsipocz    (503) staff       (20)      613 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/availability.xml
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.975459 pyvo-1.5.2/pyvo/io/vosi/tests/data/capabilities/
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1160 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/capabilities/multiple_capa_descriptions.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4087 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/capabilities.xml
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.980510 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4578 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/datatypes_tap.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     3944 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/datatypes_votable.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      780 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_column_datatypes.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      743 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_column_descriptions.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      690 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_column_names.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      711 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_column_ucds.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      716 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_column_units.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      721 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_column_utypes.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1033 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_foreignkey_descriptions.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1011 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_foreignkey_utypes.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      997 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_fromcolumns.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      641 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_schema_descriptions.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      580 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_schema_names.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      611 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_schema_titles.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      611 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_schema_utypes.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      690 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_table_descriptions.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      631 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_table_names.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      660 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_table_titles.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      660 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_table_utypes.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1003 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_targetcolumns.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      999 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_targettables.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      844 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/no_fromcolumn.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      538 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/no_schema_name.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      515 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/no_schemas.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      616 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/no_table_description.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      580 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/no_table_name.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      899 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/no_targetcolumn.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      688 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/single_table_description.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      754 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/sizenegative.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      775 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/wrong_arraysize.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      744 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/wrong_datatypes_tap.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      752 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/wrong_datatypes_votable.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      788 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/wrong_flag.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1454 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/io/vosi/tests/data/tables.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)      675 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/io/vosi/tests/test_availability.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     8210 2023-12-01 18:42:09.000000 pyvo-1.5.2/pyvo/io/vosi/tests/test_capabilities.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    14637 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/io/vosi/tests/test_tables.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    31422 2024-05-22 06:12:57.000000 pyvo-1.5.2/pyvo/io/vosi/vodataservice.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    15411 2024-05-22 06:12:57.000000 pyvo-1.5.2/pyvo/io/vosi/voresource.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.981317 pyvo-1.5.2/pyvo/registry/
+-rw-r--r--   0 bsipocz    (503) staff       (20)      699 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/registry/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    39284 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/registry/regtap.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    34996 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/registry/rtcons.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.982602 pyvo-1.5.2/pyvo/registry/tests/
+-rw-r--r--   0 bsipocz    (503) staff       (20)       64 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/registry/tests/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     2127 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/registry/tests/commonfixtures.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      694 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/registry/tests/conftest.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.983994 pyvo-1.5.2/pyvo/registry/tests/data/
+-rw-r--r--   0 bsipocz    (503) staff       (20)       98 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/registry/tests/data/README
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4275 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/registry/tests/data/capabilities.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)     2528 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/registry/tests/data/messenger.desise
+-rw-r--r--   0 bsipocz    (503) staff       (20)    11493 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/registry/tests/data/multi-interface.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)   214229 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/registry/tests/data/regtap.xml
+-rw-r--r--   0 bsipocz    (503) staff       (20)    32124 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/registry/tests/test_regtap.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    22245 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/registry/tests/test_rtcons.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     3434 2023-12-01 18:42:09.000000 pyvo-1.5.2/pyvo/samp.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.986240 pyvo-1.5.2/pyvo/utils/
+-rw-r--r--   0 bsipocz    (503) staff       (20)       82 2023-10-20 17:42:34.000000 pyvo-1.5.2/pyvo/utils/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      127 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/utils/compat.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      570 2023-09-18 21:13:09.000000 pyvo-1.5.2/pyvo/utils/decorators.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1886 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/utils/formatting.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      681 2023-12-01 18:42:09.000000 pyvo-1.5.2/pyvo/utils/http.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     2076 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/utils/protofeature.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4203 2024-05-22 06:12:32.000000 pyvo-1.5.2/pyvo/utils/prototype.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.987249 pyvo-1.5.2/pyvo/utils/tests/
+-rw-r--r--   0 bsipocz    (503) staff       (20)       64 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/utils/tests/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      395 2023-12-01 18:42:09.000000 pyvo-1.5.2/pyvo/utils/tests/test_http.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4007 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/utils/tests/test_prototype.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      309 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/utils/tests/test_url.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     3299 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/utils/tests/test_vocabularies_remote.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      641 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/utils/url.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     2261 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/utils/vocabularies.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.987939 pyvo-1.5.2/pyvo/utils/xml/
+-rw-r--r--   0 bsipocz    (503) staff       (20)        0 2022-10-05 02:13:41.000000 pyvo-1.5.2/pyvo/utils/xml/__init__.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)    15183 2023-09-20 19:34:01.000000 pyvo-1.5.2/pyvo/utils/xml/elements.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1094 2022-10-07 18:49:41.000000 pyvo-1.5.2/pyvo/utils/xml/exceptions.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.988178 pyvo-1.5.2/pyvo/utils/xml/tests/
+-rw-r--r--   0 bsipocz    (503) staff       (20)     2935 2024-05-07 00:19:42.000000 pyvo-1.5.2/pyvo/utils/xml/tests/test_elements.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)      337 2024-05-22 06:47:30.000000 pyvo-1.5.2/pyvo/version.py
+drwxr-xr-x   0 bsipocz    (503) staff       (20)        0 2024-05-22 06:47:30.988503 pyvo-1.5.2/pyvo.egg-info/
+-rw-r--r--   0 bsipocz    (503) staff       (20)     4697 2024-05-22 06:47:30.000000 pyvo-1.5.2/pyvo.egg-info/PKG-INFO
+-rw-r--r--   0 bsipocz    (503) staff       (20)     7166 2024-05-22 06:47:30.000000 pyvo-1.5.2/pyvo.egg-info/SOURCES.txt
+-rw-r--r--   0 bsipocz    (503) staff       (20)        1 2024-05-22 06:47:30.000000 pyvo-1.5.2/pyvo.egg-info/dependency_links.txt
+-rw-r--r--   0 bsipocz    (503) staff       (20)        1 2024-05-22 06:47:30.000000 pyvo-1.5.2/pyvo.egg-info/not-zip-safe
+-rw-r--r--   0 bsipocz    (503) staff       (20)      121 2024-05-22 06:47:30.000000 pyvo-1.5.2/pyvo.egg-info/requires.txt
+-rw-r--r--   0 bsipocz    (503) staff       (20)        5 2024-05-22 06:47:30.000000 pyvo-1.5.2/pyvo.egg-info/top_level.txt
+-rw-r--r--   0 bsipocz    (503) staff       (20)     2501 2024-05-22 06:47:30.990073 pyvo-1.5.2/setup.cfg
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1953 2023-09-18 21:13:09.000000 pyvo-1.5.2/setup.py
+-rw-r--r--   0 bsipocz    (503) staff       (20)     1960 2024-05-07 00:19:42.000000 pyvo-1.5.2/tox.ini
```

### Comparing `pyvo-1.5.1/.github/workflows/changelog.yml` & `pyvo-1.5.2/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/.github/workflows/ci_devtests.yml` & `pyvo-1.5.2/.github/workflows/ci_devtests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 jobs:
   devdeps:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.12"
       - name: Install tox
         run: python -m pip install --upgrade tox
       - name: Run tests against dev dependencies
         run: tox -e py312-test-devdeps-alldeps-cov
```

### Comparing `pyvo-1.5.1/.github/workflows/ci_tests.yml` & `pyvo-1.5.2/.github/workflows/ci_tests.yml`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     steps:
     - name: Checkout code
       uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install tox
       run: python -m pip install --upgrade tox
     - name: Install library dependencies and run Tests
       run: tox -e ${{ matrix.tox_env }}
 
@@ -60,15 +60,15 @@
         os: [macos-latest, windows-latest]
     steps:
     - name: Checkout code
       uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
     - name: Install tox
       run: python -m pip install --upgrade tox
     - name: Python 3.10 with latest astropy
       run: tox -e py310-test-alldeps
 
@@ -76,14 +76,14 @@
   stylecheck:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python 3.8
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.8
       - name: Install tox
         run: python -m pip install --upgrade tox
       - name: Check codestyle
         run: tox -e codestyle
```

### Comparing `pyvo-1.5.1/.gitignore` & `pyvo-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/.mailmap` & `pyvo-1.5.2/.mailmap`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/.readthedocs.yml` & `pyvo-1.5.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/CHANGES.rst` & `pyvo-1.5.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+1.5.2 (2024-05-22)
+==================
+
+Bug Fixes
+---------
+
+- Avoid Astropy Time error for SIAResult.dateobs when
+  VOX:Image_MJDateObs or ssa:DataID.Date is nan. [#550]
+
+- More robust handling of SIA1 FORMAT [#545]
+
+
 1.5.1 (2024-02-21)
 ==================
 
 Bug Fixes
 ---------
 
 - Fix ``pyvo.registry.Author`` to allow registry searches with author
```

### Comparing `pyvo-1.5.1/CONTRIBUTORS.rst` & `pyvo-1.5.2/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/LICENSE.rst` & `pyvo-1.5.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/PKG-INFO` & `pyvo-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvo
-Version: 1.5.1
+Version: 1.5.2
 Summary: Astropy affiliated package for accessing Virtual Observatory data and services
 Author: the PyVO Developers
 License: BSD
 Project-URL: Source, https://github.com/astropy/pyvo
 Project-URL: Documentation, https:/pyvo.readthedocs.io
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pyvo-1.5.1/README.rst` & `pyvo-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/RELEASE.rst` & `pyvo-1.5.2/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/conftest.py` & `pyvo-1.5.2/conftest.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/docs/Makefile` & `pyvo-1.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/docs/conf.py` & `pyvo-1.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/docs/dal/index.rst` & `pyvo-1.5.2/docs/dal/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     )<0.0002                            -- fine selection with PMs
 
 Furthermore, one can find the names of the tables using:
 
 .. doctest-remote-data::
 
     >>> print([tab_name for tab_name in tap_service.tables.keys()])  # doctest: +IGNORE_WARNINGS
-    ['amanda.nucand', 'annisred.main', 'antares.data', ..., 'wise.main', 'xpparams.main', 'zcosmos.data']
+    ['ivoa.obs_radio', 'ivoa.obscore', 'tap_schema.columns', 'tap_schema.tables',..., 'taptest.main', 'veronqsos.data', 'vlastripe82.stripe82']
 
 
 And also the names of the columns from a known table, for instance
 the first three columns:
 
 .. doctest-remote-data::
```

### Comparing `pyvo-1.5.1/docs/index.rst` & `pyvo-1.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/docs/make.bat` & `pyvo-1.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/docs/nitpick-exceptions` & `pyvo-1.5.2/docs/nitpick-exceptions`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/docs/registry/index.rst` & `pyvo-1.5.2/docs/registry/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -330,15 +330,15 @@
 
 You can learn more about the archives by printing their titles
 and access URL:
 
 .. doctest-remote-data::
 
   >>> for service in archives:
-  ...     print(service.res_title, service.access_url)
+  ...     print(service.res_title, service.access_url)  # doctest: +IGNORE_OUTPUT
   Chandra X-ray Observatory Data Archive https://cda.harvard.edu/cxcsiap/queryImages?
   Chandra Source Catalog http://cda.cfa.harvard.edu/cscsiap/queryImages?
   Chandra Source Catalog Release 1 http://cda.cfa.harvard.edu/csc1siap/queryImages?
   ...
 
 It is not necessary to keep track of the URL because you can search
 images directly from the registry record, for example using the Chandra
```

### Comparing `pyvo-1.5.1/docs/utils/prototypes.rst` & `pyvo-1.5.2/docs/utils/prototypes.rst`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/licenses/ASTROPY_LICENSE.rst` & `pyvo-1.5.2/licenses/ASTROPY_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/licenses/LICENSE.rst` & `pyvo-1.5.2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/__init__.py` & `pyvo-1.5.2/pyvo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/auth/authsession.py` & `pyvo-1.5.2/pyvo/auth/authsession.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/auth/authurls.py` & `pyvo-1.5.2/pyvo/auth/authurls.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/auth/credentialstore.py` & `pyvo-1.5.2/pyvo/auth/credentialstore.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/auth/tests/conftest.py` & `pyvo-1.5.2/pyvo/auth/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/auth/tests/data/tap/capabilities.xml` & `pyvo-1.5.2/pyvo/auth/tests/data/tap/capabilities.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/auth/tests/test_auth.py` & `pyvo-1.5.2/pyvo/auth/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/conftest.py` & `pyvo-1.5.2/pyvo/conftest.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/__init__.py` & `pyvo-1.5.2/pyvo/dal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/adhoc.py` & `pyvo-1.5.2/pyvo/dal/adhoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from .params import PosQueryParam, IntervalQueryParam, TimeQueryParam, EnumQueryParam
 from ..dam.obscore import POLARIZATION_STATES
 
 # calls to DataLink from the results pages are batched for performance
 # reasons. This is the size of a batch
 DATALINK_BATCH_CALL_SIZE = 50
 
-SODA_SYNC_IVOID = 'ivo://ivoa.net/std/SODA#sync-1.0'
+SODA_SYNC_IVOID = 'ivo://ivoa.net/std/SODA#sync-1'
 DATALINK_IVOID = 'ivo://ivoa.net/std/datalink'
 
 # MIME types
 DATALINK_MIME_TYPE = 'application/x-votable+xml;content=datalink'
 
 
 # monkeypatch astropy with group support in RESOURCE
@@ -105,15 +105,14 @@
 class AdhocServiceResultsMixin:
     """
     Mixin for adhoc:service functionallity for results classes.
     """
 
     def __init__(self, votable, url=None, session=None):
         super().__init__(votable, url=url, session=session)
-
         self._adhocservices = list(
             resource for resource in votable.resources
             if resource.type == "meta" and resource.utype == "adhoc:service"
         )
 
     def iter_adhocservices(self):
         yield from self._adhocservices
```

### Comparing `pyvo-1.5.1/pyvo/dal/dbapi2.py` & `pyvo-1.5.2/pyvo/dal/dbapi2.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/exceptions.py` & `pyvo-1.5.2/pyvo/dal/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/mimetype.py` & `pyvo-1.5.2/pyvo/dal/mimetype.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/params.py` & `pyvo-1.5.2/pyvo/dal/params.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/query.py` & `pyvo-1.5.2/pyvo/dal/query.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/scs.py` & `pyvo-1.5.2/pyvo/dal/scs.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/sia.py` & `pyvo-1.5.2/pyvo/dal/sia.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import re
 
 from pyvo.io.vosi.vodataservice import TableParam
 
 from astropy.coordinates import SkyCoord
 from astropy.time import Time
 from astropy.units import Quantity, Unit
+import numpy as np
 
 from .query import DALResults, DALQuery, DALService, Record
 from .mimetype import mime2extension
 from .adhoc import DatalinkResultsMixin, DatalinkRecordMixin, SodaRecordMixin
 
 from .. import samp
 
@@ -501,18 +502,26 @@
         """
         return getattr(self, "_format", None)
 
     @format.setter
     def format(self, format_):
         setattr(self, "_format", format_)
 
-        if isinstance(format_, (str, bytes)):
-            format_ = [format_]
+        if not isinstance(format_, list):
+            format_ = format_.split(',')
+        normalized_formats = []
+        for user_input in format_:
+            if user_input.upper() in ['ALL', 'METADATA', 'GRAPHIC', 'GRAPHIC-ALL']:
+                normalized_formats.append(user_input.upper())
+            elif user_input.split('-')[0].upper() == 'GRAPHIC':
+                normalized_formats.append(user_input.split('-')[0].upper()+"-"+user_input.split('-')[1])
+            else:
+                normalized_formats.append(user_input)
 
-        self["FORMAT"] = ",".join(_.upper() for _ in format_)
+        self["FORMAT"] = ",".join(normalized_formats)
 
     @format.deleter
     def format(self):
         delattr(self, "_format")
         del self["FORMAT"]
 
     @property
@@ -698,18 +707,21 @@
     def dateobs(self):
         """
         the modified Julien date (MJD) of the mid-point of the
         observational data that went into the image,
         as an astropy.time.Time instance
         """
         dateobs = self.getbyucd("VOX:Image_MJDateObs")
-        if dateobs:
-            return Time(dateobs, format="mjd")
-        else:
-            return None
+        try:
+            if not dateobs or np.isnan(dateobs):
+                return None
+        except TypeError:
+            # np.isnan can only check floats. If can't check for nan, pass it along
+            pass
+        return Time(dateobs, format="mjd")
 
     @property
     def naxes(self):
         """
         the number of axes in this image.
         """
         return self.getbyucd("VOX:Image_Naxes")
```

### Comparing `pyvo-1.5.1/pyvo/dal/sia2.py` & `pyvo-1.5.2/pyvo/dal/sia2.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/sla.py` & `pyvo-1.5.2/pyvo/dal/sla.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/ssa.py` & `pyvo-1.5.2/pyvo/dal/ssa.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 from astropy.coordinates import SkyCoord
 from astropy.time import Time
 from astropy.units import Quantity, Unit
 from astropy.units import spectral as spectral_equivalencies
 from astropy.io.votable.tree import Field
 from astropy.table import Table
+import numpy as np
 
 from .query import DALResults, DALQuery, DALService, Record
 from .mimetype import mime2extension
 from .adhoc import DatalinkResultsMixin, DatalinkRecordMixin, SodaRecordMixin
 
 from .. import samp
 
@@ -694,18 +695,21 @@
     @property
     def dateobs(self):
         """
         return the modified Julien date (MJD) of the mid-point of the
         observational data that went into the spectrum
         """
         dateobs = self.getbyutype("ssa:DataID.Date", decode=True)
-        if dateobs:
-            return Time(dateobs, format="iso")
-        else:
-            return None
+        try:
+            if not dateobs or np.isnan(dateobs):
+                return None
+        except TypeError:
+            # np.isnan can only check floats. If can't check for nan, pass it along
+            pass
+        return Time(dateobs, format="iso")
 
     @property
     def instr(self):
         """
         return the name of the instrument (or instruments) that produced the
         data that went into this spectrum.
         """
```

### Comparing `pyvo-1.5.1/pyvo/dal/tap.py` & `pyvo-1.5.2/pyvo/dal/tap.py`

 * *Files 0% similar despite different names*

```diff
@@ -962,15 +962,17 @@
         return self
 
     def delete(self):
         """
         deletes the job. this object will become invalid.
         """
         try:
-            response = self._session.post(self.url, data={"ACTION": "DELETE"})
+            response = self._session.delete(
+                self.url,
+                allow_redirects=False)
             response.raise_for_status()
         except requests.RequestException as ex:
             raise DALServiceError.from_except(ex, self.url)
 
         self._url = None
 
     def raise_if_error(self):
```

### Comparing `pyvo-1.5.1/pyvo/dal/tests/conftest.py` & `pyvo-1.5.2/pyvo/dal/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/datalink/cutout1.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/datalink/cutout1.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/datalink/cutout2.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/datalink/cutout2.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/datalink/datalink-obscore.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/datalink/datalink-obscore.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/datalink/datalink-ssa.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/datalink/datalink-ssa.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/datalink/datalink.desise` & `pyvo-1.5.2/pyvo/dal/tests/data/datalink/datalink.desise`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/datalink/datalink.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/datalink/datalink.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/datalink/proc.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/datalink/proc.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/datalink/proc_inf.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/datalink/proc_inf.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/datalink/proc_units.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/datalink/proc_units.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/mimetype/ivoa_logo.jpg` & `pyvo-1.5.2/pyvo/dal/tests/data/mimetype/ivoa_logo.jpg`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/mimetype/test.fits` & `pyvo-1.5.2/pyvo/dal/tests/data/mimetype/test.fits`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/monkeypatch.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/monkeypatch.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/query/basic.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/query/basic.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/query/dataset.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/query/dataset.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/query/errorstatus.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/query/errorstatus.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/query/firstresource.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/query/firstresource.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/query/missingcolumns.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/query/missingcolumns.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/query/overflowstatus.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/query/overflowstatus.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/query/rootinfo.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/query/rootinfo.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/query/tableinfo.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/query/tableinfo.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/querydata/image.fits` & `pyvo-1.5.2/pyvo/dal/tests/data/querydata/image.fits`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/scs/result.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/scs/result.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/sia/dataset.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/sia/dataset.xml`

 * *Files 10% similar despite different names*

#### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/sia/dataset.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/sia/dataset.xml`

```diff
@@ -54,12 +54,27 @@
             <TD>288.95078924817</TD>
             <TD>15.0322239971381</TD>
             <TD>Test Observation</TD>
             <TD>3.8e-07</TD>
             <TD>5.2e-07</TD>
             <TD>0.000403806 0.000406123</TD>
           </TR>
+          <TR>
+            <TD>This should not be the dataurl</TD>
+            <TD>http://example.com/querydata/image.fits</TD>
+            <TD>image/fits</TD>
+            <TD>153280</TD>
+            <TD/>
+            <!-- Empty VOX:Image_MJDateObs field -->
+            <TD>Test</TD>
+            <TD>288.95078924817</TD>
+            <TD>15.0322239971381</TD>
+            <TD>Test Observation</TD>
+            <TD>3.8e-07</TD>
+            <TD>5.2e-07</TD>
+            <TD>0.000403806 0.000406123</TD>
+          </TR>
         </TABLEDATA>
       </DATA>
     </TABLE>
   </RESOURCE>
 </VOTABLE>
```

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/sia2/capabilities-basicauth.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/sia2/capabilities-basicauth.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/sia2/capabilities-newformat.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/sia2/capabilities-newformat.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/sia2/capabilities-priv.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/sia2/capabilities-priv.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/sia2/capabilities.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/sia2/capabilities.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/sia2/dataset.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/sia2/dataset.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/sla/dataset.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/sla/dataset.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/ssa/result.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/ssa/result.xml`

 * *Files 2% similar despite different names*

#### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/ssa/result.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/ssa/result.xml`

```diff
@@ -1393,12 +1393,48 @@
             <TD>0</TD>
             <TD>FK5</TD>
             <TD>2000</TD>
             <TD>TAI</TD>
             <TD>179.825520 0.853781</TD>
             <TD/>
           </TR>
+          <TR>
+            <TD>8.441184510333563E-42</TD>
+            <TD>http://vaosa-vm1.aoc.nrao.edu/ivoa-dal/JhuSsapServlet?REQUEST=getData&amp;FORMAT=votable&amp;PubDID=ivo%3A%2F%2Fjhu%2Fsdss%2Fdr6%2Fspec%2F2.5%2380442261136998400</TD>
+            <TD>application/x-votable+xml</TD>
+            <TD>SPECTRUM-1.0</TD>
+            <TD>SPECTRUM</TD>
+            <TD>4000</TD>
+            <TD>s</TD>
+            <TD>A</TD>
+            <TD>10**(-17) erg s**(-1) cm**(-2) A**(-1)</TD>
+            <TD>SDSS J115918.12+005113.61 GALAXY</TD>
+            <TD>sdss</TD>
+            <TD>SDSS DR6</TD>
+            <TD>ivo://sdss/dr6/spec/2_5/#80442261136998400</TD>
+            <TD/>
+            <!-- Empty VOX:Image_MJDateObs field -->
+            <TD>6.2.5</TD>
+            <TD>ivo://sdss/dr6/spec/2_5/#80442261136998400</TD>
+            <TD>SDSS 2.5-M SPEC2 v4_5</TD>
+            <TD>OPTICAL</TD>
+            <TD>SURVEY</TD>
+            <TD>ARCHIVAL</TD>
+            <TD>ELTE VO</TD>
+            <TD>ivo://jhu/sdss/dr6/spec/2.5#80442261136998400</TD>
+            <TD>PUBLIC</TD>
+            <TD>179.825520 0.853781</TD>
+            <TD>SDSS J115918.12+005113.61</TD>
+            <TD>GALAXY</TD>
+            <TD>0.0770941</TD>
+            <TD>0</TD>
+            <TD>FK5</TD>
+            <TD>2000</TD>
+            <TD>TAI</TD>
+            <TD>179.825520 0.853781</TD>
+            <TD/>
+          </TR>
         </TABLEDATA>
       </DATA>
     </TABLE>
   </RESOURCE>
 </VOTABLE>
```

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/tap/capabilities.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/tap/capabilities.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/tap/examples.htm` & `pyvo-1.5.2/pyvo/dal/tests/data/tap/examples.htm`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/tap/lazy-table1.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/tap/lazy-table1.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/tap/lazy-table2.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/tap/lazy-table2.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/tap/obscore-examples.html` & `pyvo-1.5.2/pyvo/dal/tests/data/tap/obscore-examples.html`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/tap/obscore-image.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/tap/obscore-image.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/data/tap/tables.xml` & `pyvo-1.5.2/pyvo/dal/tests/data/tap/tables.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/make_testdata.py` & `pyvo-1.5.2/pyvo/dal/tests/make_testdata.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/test_adhoc.py` & `pyvo-1.5.2/pyvo/dal/tests/test_adhoc.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/test_datalink.py` & `pyvo-1.5.2/pyvo/dal/tests/test_datalink.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/test_mimetype.py` & `pyvo-1.5.2/pyvo/dal/tests/test_mimetype.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/test_params.py` & `pyvo-1.5.2/pyvo/dal/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/test_query.py` & `pyvo-1.5.2/pyvo/dal/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/test_scs.py` & `pyvo-1.5.2/pyvo/dal/tests/test_scs.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/test_sia.py` & `pyvo-1.5.2/pyvo/dal/tests/test_sia.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Tests for pyvo.dal.sia
 """
 from functools import partial
 import re
 
 import pytest
 
-from pyvo.dal.sia import search, SIAService
+from pyvo.dal.sia import search, SIAService, SIAQuery
 
 from astropy.io.fits import HDUList
 from astropy.coordinates import SkyCoord
 from astropy.utils.data import get_pkg_data_contents
 
 get_pkg_data_contents = partial(
     get_pkg_data_contents, package=__package__, encoding='binary')
@@ -43,27 +43,48 @@
     assert result.filesize == 153280
 
 
 @pytest.mark.usefixtures('sia')
 @pytest.mark.usefixtures('register_mocks')
 @pytest.mark.filterwarnings("ignore::astropy.io.votable.exceptions.W06")
 @pytest.mark.parametrize("position", ((288, 15), SkyCoord(288, 15, unit="deg")))
-def test_search(position):
-    results = search('http://example.com/sia', pos=position)
+@pytest.mark.parametrize("format", ("IMAGE/JPEG", "all"))
+def test_search(position, format):
+    results = search('http://example.com/sia', pos=position, format=format)
     result = results[0]
 
     _test_result(result)
 
 
 class TestSIAService:
     @pytest.mark.usefixtures('sia')
     @pytest.mark.usefixtures('register_mocks')
     @pytest.mark.filterwarnings("ignore::astropy.io.votable.exceptions.W06")
     @pytest.mark.filterwarnings("ignore::astropy.io.votable.exceptions.W42")
     @pytest.mark.filterwarnings("ignore::astropy.io.votable.exceptions.W49")
     def test_search(self):
-        service = SIAService('http://example.com/sia')
+        url = 'http://example.com/sia'
+        service = SIAService(url)
+        assert service.baseurl == url
 
         results = service.search(pos=(288, 15))
         result = results[0]
 
         _test_result(result)
+
+        assert results[1].dateobs is None
+
+    @pytest.mark.usefixtures('sia')
+    @pytest.mark.usefixtures('register_mocks')
+    @pytest.mark.filterwarnings("ignore::astropy.io.votable.exceptions.W06")
+    @pytest.mark.filterwarnings("ignore::astropy.io.votable.exceptions.W42")
+    @pytest.mark.filterwarnings("ignore::astropy.io.votable.exceptions.W49")
+    def test_formatter(self):
+        service = SIAQuery('http://example.com/sia')
+        service.format = "image"
+        assert service["FORMAT"] == "image"
+        service.format = "all"
+        assert service["FORMAT"] == "ALL"
+        service.format = "Graphic-png"
+        assert service["FORMAT"] == "GRAPHIC-png"
+        service.format = "Unsupported"
+        assert service["FORMAT"] == "Unsupported"
```

### Comparing `pyvo-1.5.1/pyvo/dal/tests/test_sia2.py` & `pyvo-1.5.2/pyvo/dal/tests/test_sia2.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/test_sia2_remote.py` & `pyvo-1.5.2/pyvo/dal/tests/test_sia2_remote.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/test_sla.py` & `pyvo-1.5.2/pyvo/dal/tests/test_sla.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/tests/test_ssa.py` & `pyvo-1.5.2/pyvo/dal/tests/test_ssa.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,19 +29,20 @@
         yield matcher
 
 
 @pytest.mark.usefixtures('ssa')
 @pytest.mark.filterwarnings("ignore::astropy.io.votable.exceptions.W42")
 def test_search():
     results = search('http://example.com/ssa', pos=(0.0, 0.0), diameter=1.0)
-    assert len(results) == 35
+    assert len(results) == 36
 
 
 class TestSSAService:
     @pytest.mark.usefixtures('ssa')
     @pytest.mark.filterwarnings("ignore::astropy.io.votable.exceptions.W42")
     def test_search(self):
         service = SSAService('http://example.com/ssa')
 
         results = service.search(pos=(0.0, 0.0), diameter=1.0)
 
-        assert len(results) == 35
+        assert len(results) == 36
+        assert results[35].dateobs is None
```

### Comparing `pyvo-1.5.1/pyvo/dal/tests/test_tap.py` & `pyvo-1.5.2/pyvo/dal/tests/test_tap.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dal/vosi.py` & `pyvo-1.5.2/pyvo/dal/vosi.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/dam/obscore.py` & `pyvo-1.5.2/pyvo/dam/obscore.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/uws/endpoint.py` & `pyvo-1.5.2/pyvo/io/uws/endpoint.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/uws/tests/data/job-error.xml` & `pyvo-1.5.2/pyvo/io/uws/tests/data/job-error.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/uws/tests/data/job-implicit-v1.0.xml` & `pyvo-1.5.2/pyvo/io/uws/tests/data/job-implicit-v1.0.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/uws/tests/data/job.xml` & `pyvo-1.5.2/pyvo/io/uws/tests/data/job.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/uws/tests/test_job.py` & `pyvo-1.5.2/pyvo/io/uws/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/uws/tree.py` & `pyvo-1.5.2/pyvo/io/uws/tree.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/availability.py` & `pyvo-1.5.2/pyvo/io/vosi/availability.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/endpoint.py` & `pyvo-1.5.2/pyvo/io/vosi/endpoint.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/exceptions.py` & `pyvo-1.5.2/pyvo/io/vosi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tapregext.py` & `pyvo-1.5.2/pyvo/io/vosi/tapregext.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 from astropy.utils.collections import HomogeneousList
-from astropy.utils.misc import indent
+from textwrap import indent
 
 from astropy.io.votable.exceptions import vo_raise, warn_or_raise
 
 from ...utils.xml.elements import (
     Element, ContentMixin, xmlelement, xmlattribute)
 from . import voresource as vr
 from .exceptions import (
@@ -13,14 +13,17 @@
 
 __all__ = [
     "TAPCapRestriction", "TableAccess", "DataModelType", "Language", "Version",
     "LanguageFeatureList", "LanguageFeature", "OutputFormat", "UploadMethod",
     "TimeLimits", "DataLimits", "DataLimit"]
 
 
+INDENT = 4 * " "
+
+
 ######################################################################
 # ELEMENT CLASSES
 class DataModelType(ContentMixin, Element):
     def __init__(self, config=None, pos=None, **kwargs):
         super().__init__(config=config, pos=pos, **kwargs)
 
         ivo_id = kwargs.get('ivo-id', None)
@@ -33,15 +36,15 @@
             self.ivo_id, self.content)
 
     def describe(self):
         """
         Prints out a human readable description
         """
         print("Datamodel {}".format(self.content))
-        print(indent(self.ivo_id))
+        print(indent(self.ivo_id, INDENT))
         print()
 
     @xmlattribute(name='ivo-id')
     def ivo_id(self):
         """The IVORN of the data model."""
         return self._ivo_id
 
@@ -67,16 +70,16 @@
     def describe(self):
         """
         Prints out a human readable description
         """
         print('Output format {}'.format(self.mime))
 
         if self.aliases:
-            print(indent('Also available as {}'.format(
-                ', '.join(self.aliases))))
+            print(indent('Also available as {}'.format(', '.join(self.aliases)),
+                         INDENT))
 
         print()
 
     @xmlelement(plain=True, multiple_exc=W28)
     def mime(self):
         return self._mime
 
@@ -100,15 +103,15 @@
         return '<UploadMethod ivo-id="{}"/>'.format(self.ivo_id)
 
     def describe(self):
         """
         Prints out a human readable description
         """
         print("Upload method supported")
-        print(indent(self.ivo_id))
+        print(indent(self.ivo_id, INDENT))
         print()
 
     @xmlattribute(name='ivo-id')
     def ivo_id(self):
         """The IVORN of the upload model."""
         return self._ivo_id
 
@@ -234,21 +237,21 @@
     def describe(self):
         """
         Prints out a human readable description
         """
         print("Language {}".format(self.name))
 
         for languagefeaturelist in self.languagefeaturelists:
-            print(indent(languagefeaturelist.type))
+            print(indent(languagefeaturelist.type, INDENT))
 
             for feature in languagefeaturelist:
-                print(indent(feature.form, shift=2))
+                print(indent(feature.form, 2 * INDENT))
 
                 if feature.description:
-                    print(indent(feature.description, shift=3))
+                    print(indent(feature.description, 3 * INDENT))
 
                 print()
 
             print()
 
     def get_feature_list(self, ivoid):
         """
@@ -463,42 +466,42 @@
             outputformat.describe()
 
         for uploadmethod in self.uploadmethods:
             uploadmethod.describe()
 
         if self.retentionperiod:
             print("Time a job is kept (in seconds)")
-            print(indent("Default {}".format(self.retentionperiod.default)))
+            print(indent("Default {}".format(self.retentionperiod.default), INDENT))
             if self.retentionperiod.hard:
-                print(indent("Maximum {}".format(self.retentionperiod.hard)))
+                print(indent("Maximum {}".format(self.retentionperiod.hard), INDENT))
             print()
 
         if self.executionduration:
             print("Maximal run time of a job")
-            print(indent("Default {}".format(self.executionduration.default)))
+            print(indent("Default {}".format(self.executionduration.default), INDENT))
             if self.executionduration.hard:
-                print(indent("Maximum {}".format(self.executionduration.hard)))
+                print(indent("Maximum {}".format(self.executionduration.hard), INDENT))
             print()
 
         if self.outputlimit:
             print("Maximum size of resultsets")
             print(indent("Default {} {}".format(
                 self.outputlimit.default.content,
-                self.outputlimit.default.unit))
+                self.outputlimit.default.unit), INDENT)
             )
             if self.outputlimit.hard:
                 print(indent("Maximum {} {}".format(
-                    self.outputlimit.hard.content, self.outputlimit.hard.unit))
+                    self.outputlimit.hard.content, self.outputlimit.hard.unit), INDENT)
                 )
             print()
 
         if self.uploadlimit:
             print("Maximal size of uploads")
             print(indent("Maximum {} {}".format(
-                self.uploadlimit.hard.content, self.uploadlimit.hard.unit)))
+                self.uploadlimit.hard.content, self.uploadlimit.hard.unit), INDENT))
             print()
 
     def get_adql(self):
         """
         returns the (first) ADQL language element on this service.
 
         ADQL support is mandatory for IVOA TAP, so in general you can
```

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/availability.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/availability.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/capabilities/multiple_capa_descriptions.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/capabilities/multiple_capa_descriptions.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/capabilities.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/capabilities.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/datatypes_tap.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/datatypes_tap.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/datatypes_votable.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/datatypes_votable.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_column_datatypes.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_column_datatypes.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_column_descriptions.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_column_descriptions.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_column_names.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_column_names.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_column_ucds.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_column_ucds.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_column_units.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_column_units.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_column_utypes.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_column_utypes.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_foreignkey_descriptions.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_foreignkey_descriptions.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_foreignkey_utypes.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_foreignkey_utypes.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_fromcolumns.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_fromcolumns.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_schema_descriptions.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_schema_descriptions.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_schema_names.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_schema_names.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_schema_titles.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_schema_titles.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_schema_utypes.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_schema_utypes.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_table_descriptions.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_table_descriptions.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_table_names.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_table_names.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_table_titles.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_table_titles.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_table_utypes.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_table_utypes.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_targetcolumns.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_targetcolumns.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/multiple_targettables.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/multiple_targettables.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/no_fromcolumn.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/no_fromcolumn.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/no_schema_name.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/no_schema_name.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/no_schemas.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/no_schemas.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/no_table_description.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/no_table_description.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/no_table_name.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/no_table_name.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/no_targetcolumn.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/no_targetcolumn.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/single_table_description.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/single_table_description.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/sizenegative.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/sizenegative.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/wrong_arraysize.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/wrong_arraysize.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/wrong_datatypes_tap.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/wrong_datatypes_tap.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/wrong_datatypes_votable.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/wrong_datatypes_votable.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables/wrong_flag.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables/wrong_flag.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/data/tables.xml` & `pyvo-1.5.2/pyvo/io/vosi/tests/data/tables.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/test_availability.py` & `pyvo-1.5.2/pyvo/io/vosi/tests/test_availability.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/test_capabilities.py` & `pyvo-1.5.2/pyvo/io/vosi/tests/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/tests/test_tables.py` & `pyvo-1.5.2/pyvo/io/vosi/tests/test_tables.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/io/vosi/vodataservice.py` & `pyvo-1.5.2/pyvo/io/vosi/vodataservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 defining a ``value`` property.
 """
 
 import re
 
 from astropy.utils import deprecated
 from astropy.utils.collections import HomogeneousList
-from astropy.utils.misc import indent
+from textwrap import indent
 from astropy.utils.xml import check as xml_check
 from astropy.io.votable.exceptions import vo_raise, vo_warn, warn_or_raise
 
 from ...utils.xml.elements import (
     xmlattribute, xmlelement, Element, ElementWithXSIType, ContentMixin)
 
 from . import voresource as vr
@@ -314,15 +314,15 @@
     def __repr__(self):
         return '<VODataServiceTable name="{}">... {} columns ...</VODataServiceTable>'.format(
             self.name, len(self.columns))
 
     def describe(self):
         print(self.name)
         if self.description is not None:
-            print(indent(self.description))
+            print(indent(self.description, 4 * " "))
         else:
             print('No description')
 
         print()
 
     @xmlelement(plain=True, multiple_exc=W05)
     def name(self):
```

### Comparing `pyvo-1.5.1/pyvo/io/vosi/voresource.py` & `pyvo-1.5.2/pyvo/io/vosi/voresource.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Elements with complex content are parsed with objects inherited from `~pyvo.utils.xml.elements.Element`.
 
 Elements with simple content are parsed with objects inherited from `~pyvo.utils.xml.elements.Element`
 defining a ``value`` property.
 """
 from astropy.utils.collections import HomogeneousList
-from astropy.utils.misc import indent
+from textwrap import indent
 
 from ...utils.xml.elements import (
     Element, ElementWithXSIType, ContentMixin, xmlattribute, xmlelement)
 from .exceptions import W06
 
 __all__ = [
     "ValidationLevel", "Capability", "Interface", "AccessURL",
@@ -240,15 +240,15 @@
         Prints out a human readable description
         """
         print('Interface {}'.format(self._xsi_type))
 
         accessurls = '\n'.join(
             accessurl.content for accessurl in self.accessurls)
 
-        print(indent(accessurls))
+        print(indent(accessurls, 4 * " "))
 
         print()
 
     @xmlattribute
     def version(self):
         """
         The version of a standard interface specification that this
```

### Comparing `pyvo-1.5.1/pyvo/registry/__init__.py` & `pyvo-1.5.2/pyvo/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/registry/regtap.py` & `pyvo-1.5.2/pyvo/registry/regtap.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/registry/rtcons.py` & `pyvo-1.5.2/pyvo/registry/rtcons.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/registry/tests/commonfixtures.py` & `pyvo-1.5.2/pyvo/registry/tests/commonfixtures.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/registry/tests/conftest.py` & `pyvo-1.5.2/pyvo/registry/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/registry/tests/data/capabilities.xml` & `pyvo-1.5.2/pyvo/registry/tests/data/capabilities.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/registry/tests/data/messenger.desise` & `pyvo-1.5.2/pyvo/registry/tests/data/messenger.desise`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/registry/tests/data/multi-interface.xml` & `pyvo-1.5.2/pyvo/registry/tests/data/multi-interface.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/registry/tests/data/regtap.xml` & `pyvo-1.5.2/pyvo/registry/tests/data/regtap.xml`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/registry/tests/test_regtap.py` & `pyvo-1.5.2/pyvo/registry/tests/test_regtap.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/registry/tests/test_rtcons.py` & `pyvo-1.5.2/pyvo/registry/tests/test_rtcons.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/samp.py` & `pyvo-1.5.2/pyvo/samp.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/utils/decorators.py` & `pyvo-1.5.2/pyvo/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/utils/formatting.py` & `pyvo-1.5.2/pyvo/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/utils/http.py` & `pyvo-1.5.2/pyvo/utils/http.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/utils/protofeature.py` & `pyvo-1.5.2/pyvo/utils/protofeature.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/utils/prototype.py` & `pyvo-1.5.2/pyvo/utils/prototype.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/utils/tests/test_prototype.py` & `pyvo-1.5.2/pyvo/utils/tests/test_prototype.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/utils/tests/test_vocabularies_remote.py` & `pyvo-1.5.2/pyvo/utils/tests/test_vocabularies_remote.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/utils/url.py` & `pyvo-1.5.2/pyvo/utils/url.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/utils/vocabularies.py` & `pyvo-1.5.2/pyvo/utils/vocabularies.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/utils/xml/elements.py` & `pyvo-1.5.2/pyvo/utils/xml/elements.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/utils/xml/exceptions.py` & `pyvo-1.5.2/pyvo/utils/xml/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo/utils/xml/tests/test_elements.py` & `pyvo-1.5.2/pyvo/utils/xml/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/pyvo.egg-info/PKG-INFO` & `pyvo-1.5.2/pyvo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvo
-Version: 1.5.1
+Version: 1.5.2
 Summary: Astropy affiliated package for accessing Virtual Observatory data and services
 Author: the PyVO Developers
 License: BSD
 Project-URL: Source, https://github.com/astropy/pyvo
 Project-URL: Documentation, https:/pyvo.readthedocs.io
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pyvo-1.5.1/pyvo.egg-info/SOURCES.txt` & `pyvo-1.5.2/pyvo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/setup.cfg` & `pyvo-1.5.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	ignore:distutils Version classes are deprecated:DeprecationWarning
 	ignore:numpy.core:DeprecationWarning
 
 [flake8]
 max-line-length = 110
 max-doc-length = 110
 exclude = __init__.py, conf.py, setup.py, version.py, conftest.py
-ignore = W503,E128,E131
+ignore = W503,E124,E127,E226,E128,E131
 
 [pycodestyle]
 max-line-length = 110
 max-doc-length = 110
 
 [metadata]
 name = pyvo
```

### Comparing `pyvo-1.5.1/setup.py` & `pyvo-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyvo-1.5.1/tox.ini` & `pyvo-1.5.2/tox.ini`

 * *Files identical despite different names*

