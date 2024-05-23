# Comparing `tmp/owasp_depscan-5.3.4.tar.gz` & `tmp/owasp_depscan-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owasp_depscan-5.3.4.tar", last modified: Thu May  2 20:45:05 2024, max compression
+gzip compressed data, was "owasp_depscan-5.3.5.tar", last modified: Thu May 23 11:26:23 2024, max compression
```

## Comparing `owasp_depscan-5.3.4.tar` & `owasp_depscan-5.3.5.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:45:04.996334 owasp_depscan-5.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-05-02 20:45:04.996334 owasp_depscan-5.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:45:04.980334 owasp_depscan-5.3.4/depscan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    39048 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:45:04.984334 owasp_depscan-5.3.4/depscan/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59180 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/bom.py
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    81781 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/csaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/license.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/orasclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/pkg_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/depscan/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:45:04.996334 owasp_depscan-5.3.4/owasp_depscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-05-02 20:45:04.000000 owasp_depscan-5.3.4/owasp_depscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-02 20:45:04.000000 owasp_depscan-5.3.4/owasp_depscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:45:04.000000 owasp_depscan-5.3.4/owasp_depscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 20:45:04.000000 owasp_depscan-5.3.4/owasp_depscan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 20:45:04.000000 owasp_depscan-5.3.4/owasp_depscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 20:45:04.000000 owasp_depscan-5.3.4/owasp_depscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:45:04.996334 owasp_depscan-5.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:45:04.984334 owasp_depscan-5.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)    32402 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/test/test_bom.py
--rw-r--r--   0 runner    (1001) docker     (127)    37991 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/test/test_csaf.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/test/test_explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/test/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/test/test_license.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/test/test_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/test/test_pkg_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:45:04.984334 owasp_depscan-5.3.4/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:45:04.980334 owasp_depscan-5.3.4/vendor/choosealicense.com/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:45:04.988334 owasp_depscan-5.3.4/vendor/choosealicense.com/_data/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_data/fields.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_data/meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_data/rules.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:45:04.996334 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/0bsd.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/afl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35944 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/agpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/artistic-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/bsd-2-clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/bsd-3-clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/bsd-4-clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/bsl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cc-by-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cc0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cecill-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/ecl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12461 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/epl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/epl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/eupl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/eupl-1.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23969 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/gfdl-1.3.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/gpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    36394 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/gpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/isc.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27491 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/lgpl-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/lgpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/lppl-1.3c.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/mit-0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/mit.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/mpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/ms-pl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/ms-rl.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/ncsa.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26179 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/odbl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/ofl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/osl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/postgresql.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/upl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/vim.txt
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/wtfpl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/zlib.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:45:04.980334 owasp_depscan-5.3.4/vendor/spdx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:45:04.996334 owasp_depscan-5.3.4/vendor/spdx/json/
--rw-r--r--   0 runner    (1001) docker     (127)   275192 2024-05-02 20:44:51.000000 owasp_depscan-5.3.4/vendor/spdx/json/licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:23.974959 owasp_depscan-5.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-05-23 11:26:23.974959 owasp_depscan-5.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:23.954959 owasp_depscan-5.3.5/depscan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39048 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:23.958959 owasp_depscan-5.3.5/depscan/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59180 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/bom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81781 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/csaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/orasclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/pkg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/depscan/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:23.974959 owasp_depscan-5.3.5/owasp_depscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-05-23 11:26:23.000000 owasp_depscan-5.3.5/owasp_depscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-23 11:26:23.000000 owasp_depscan-5.3.5/owasp_depscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:26:23.000000 owasp_depscan-5.3.5/owasp_depscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-23 11:26:23.000000 owasp_depscan-5.3.5/owasp_depscan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-23 11:26:23.000000 owasp_depscan-5.3.5/owasp_depscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 11:26:23.000000 owasp_depscan-5.3.5/owasp_depscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:26:23.974959 owasp_depscan-5.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:23.962959 owasp_depscan-5.3.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    32402 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/test/test_bom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37991 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/test/test_csaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/test/test_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/test/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/test/test_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/test/test_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/test/test_pkg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:23.962959 owasp_depscan-5.3.5/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:23.954959 owasp_depscan-5.3.5/vendor/choosealicense.com/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:23.962959 owasp_depscan-5.3.5/vendor/choosealicense.com/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_data/fields.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_data/meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_data/rules.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:23.970959 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/0bsd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/afl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35944 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/agpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/artistic-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/bsd-2-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/bsd-3-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/bsd-4-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/bsl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cc-by-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cc0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cecill-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/ecl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12461 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/epl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/epl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/eupl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/eupl-1.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23969 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/gfdl-1.3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/gpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    36394 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/gpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/isc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27491 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/lgpl-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/lgpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/lppl-1.3c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/mit-0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/mit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/mpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/ms-pl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/ms-rl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/ncsa.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26179 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/odbl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/ofl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/osl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/postgresql.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/upl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/vim.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/wtfpl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/zlib.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:23.954959 owasp_depscan-5.3.5/vendor/spdx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:26:23.970959 owasp_depscan-5.3.5/vendor/spdx/json/
+-rw-r--r--   0 runner    (1001) docker     (127)   275192 2024-05-23 11:26:13.000000 owasp_depscan-5.3.5/vendor/spdx/json/licenses.json
```

### Comparing `owasp_depscan-5.3.4/LICENSE` & `owasp_depscan-5.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/PKG-INFO` & `owasp_depscan-5.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owasp-depscan
-Version: 5.3.4
+Version: 5.3.5
 Summary: Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.
 Author-email: Team AppThreat <cloud@appthreat.com>
 License: MIT
 Project-URL: Homepage, https://github.com/owasp-dep-scan/dep-scan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: appthreat-vulnerability-db==5.6.7
+Requires-Dist: appthreat-vulnerability-db==5.6.8
 Requires-Dist: defusedxml
 Requires-Dist: oras~=0.1.26
 Requires-Dist: PyYAML
 Requires-Dist: rich
 Requires-Dist: quart
 Requires-Dist: PyGithub
 Requires-Dist: toml
```

### Comparing `owasp_depscan-5.3.4/README.md` & `owasp_depscan-5.3.5/README.md`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/cli.py` & `owasp_depscan-5.3.5/depscan/cli.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/analysis.py` & `owasp_depscan-5.3.5/depscan/lib/analysis.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/audit.py` & `owasp_depscan-5.3.5/depscan/lib/audit.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/bom.py` & `owasp_depscan-5.3.5/depscan/lib/bom.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/config.py` & `owasp_depscan-5.3.5/depscan/lib/config.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/csaf.py` & `owasp_depscan-5.3.5/depscan/lib/csaf.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/explainer.py` & `owasp_depscan-5.3.5/depscan/lib/explainer.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/github.py` & `owasp_depscan-5.3.5/depscan/lib/github.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/license.py` & `owasp_depscan-5.3.5/depscan/lib/license.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/logger.py` & `owasp_depscan-5.3.5/depscan/lib/logger.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/normalize.py` & `owasp_depscan-5.3.5/depscan/lib/normalize.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/orasclient.py` & `owasp_depscan-5.3.5/depscan/lib/orasclient.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/pkg_query.py` & `owasp_depscan-5.3.5/depscan/lib/pkg_query.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/depscan/lib/utils.py` & `owasp_depscan-5.3.5/depscan/lib/utils.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/owasp_depscan.egg-info/PKG-INFO` & `owasp_depscan-5.3.5/owasp_depscan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owasp-depscan
-Version: 5.3.4
+Version: 5.3.5
 Summary: Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.
 Author-email: Team AppThreat <cloud@appthreat.com>
 License: MIT
 Project-URL: Homepage, https://github.com/owasp-dep-scan/dep-scan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: appthreat-vulnerability-db==5.6.7
+Requires-Dist: appthreat-vulnerability-db==5.6.8
 Requires-Dist: defusedxml
 Requires-Dist: oras~=0.1.26
 Requires-Dist: PyYAML
 Requires-Dist: rich
 Requires-Dist: quart
 Requires-Dist: PyGithub
 Requires-Dist: toml
```

### Comparing `owasp_depscan-5.3.4/owasp_depscan.egg-info/SOURCES.txt` & `owasp_depscan-5.3.5/owasp_depscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/pyproject.toml` & `owasp_depscan-5.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "owasp-depscan"
-version = "5.3.4"
+version = "5.3.5"
 description = "Fully open-source security audit for project dependencies based on known vulnerabilities and advisories."
 authors = [
     {name = "Team AppThreat", email = "cloud@appthreat.com"},
 ]
 dependencies = [
-    "appthreat-vulnerability-db==5.6.7",
+    "appthreat-vulnerability-db==5.6.8",
     "defusedxml",
     "oras~=0.1.26",
     "PyYAML",
     "rich",
     "quart",
     "PyGithub",
     "toml",
```

### Comparing `owasp_depscan-5.3.4/test/test_analysis.py` & `owasp_depscan-5.3.5/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/test/test_bom.py` & `owasp_depscan-5.3.5/test/test_bom.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/test/test_csaf.py` & `owasp_depscan-5.3.5/test/test_csaf.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/test/test_github.py` & `owasp_depscan-5.3.5/test/test_github.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/test/test_license.py` & `owasp_depscan-5.3.5/test/test_license.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/test/test_norm.py` & `owasp_depscan-5.3.5/test/test_norm.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/test/test_pkg_query.py` & `owasp_depscan-5.3.5/test/test_pkg_query.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/test/test_utils.py` & `owasp_depscan-5.3.5/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_data/fields.yml` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_data/fields.yml`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_data/meta.yml` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_data/meta.yml`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_data/rules.yml` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_data/rules.yml`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/0bsd.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/0bsd.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/afl-3.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/afl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/agpl-3.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/apache-2.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/artistic-2.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/bsd-2-clause.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/bsd-3-clause.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/bsd-3-clause.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/bsd-4-clause.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/bsd-4-clause.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/bsl-1.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/bsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cc-by-4.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cc-by-4.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cc0-1.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cc0-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cecill-2.1.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cecill-2.1.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/ecl-2.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/ecl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/epl-1.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/epl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/epl-2.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/epl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/eupl-1.1.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/eupl-1.1.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/eupl-1.2.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/eupl-1.2.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/gfdl-1.3.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/gfdl-1.3.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/gpl-2.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/gpl-3.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/isc.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/isc.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/lgpl-2.1.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/lgpl-2.1.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/lgpl-3.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/lppl-1.3c.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/lppl-1.3c.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/mit-0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/mit-0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/mit.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/mit.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/mpl-2.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/mpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/ms-pl.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/ms-pl.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/ms-rl.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/ms-rl.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/ncsa.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/ncsa.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/odbl-1.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/odbl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/ofl-1.1.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/ofl-1.1.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/osl-3.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/osl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/postgresql.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/postgresql.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/unlicense.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/unlicense.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/upl-1.0.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/upl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/vim.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/vim.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/wtfpl.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/wtfpl.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/choosealicense.com/_licenses/zlib.txt` & `owasp_depscan-5.3.5/vendor/choosealicense.com/_licenses/zlib.txt`

 * *Files identical despite different names*

### Comparing `owasp_depscan-5.3.4/vendor/spdx/json/licenses.json` & `owasp_depscan-5.3.5/vendor/spdx/json/licenses.json`

 * *Files identical despite different names*

