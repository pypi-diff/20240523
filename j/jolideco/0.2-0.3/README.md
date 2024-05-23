# Comparing `tmp/jolideco-0.2.tar.gz` & `tmp/jolideco-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jolideco-0.2.tar", last modified: Mon Mar 25 18:33:31 2024, max compression
+gzip compressed data, was "jolideco-0.3.tar", last modified: Thu May 23 20:58:19 2024, max compression
```

## Comparing `jolideco-0.2.tar` & `jolideco-0.3.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.968836 jolideco-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.944836 jolideco-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.948836 jolideco-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-25 18:33:26.000000 jolideco-0.2/.github/workflows/ci_cron_weekly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-25 18:33:26.000000 jolideco-0.2/.github/workflows/ci_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-25 18:33:26.000000 jolideco-0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-25 18:33:26.000000 jolideco-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-25 18:33:26.000000 jolideco-0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-25 18:33:26.000000 jolideco-0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-03-25 18:33:26.000000 jolideco-0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-25 18:33:26.000000 jolideco-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-25 18:33:26.000000 jolideco-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-03-25 18:33:31.968836 jolideco-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-03-25 18:33:26.000000 jolideco-0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.952836 jolideco-0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-25 18:33:26.000000 jolideco-0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.944836 jolideco-0.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.952836 jolideco-0.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-25 18:33:26.000000 jolideco-0.2/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.952836 jolideco-0.2/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)   969644 2024-03-25 18:33:26.000000 jolideco-0.2/docs/_static/images/jolideco-example.png
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-25 18:33:26.000000 jolideco-0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-03-25 18:33:26.000000 jolideco-0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-25 18:33:26.000000 jolideco-0.2/docs/developer.rst
--rw-r--r--   0 runner    (1001) docker     (127)   460040 2024-03-25 18:33:26.000000 jolideco-0.2/docs/image-prior-intuition.png
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-25 18:33:26.000000 jolideco-0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)   803093 2024-03-25 18:33:26.000000 jolideco-0.2/docs/jolideco-illustration.png
--rw-r--r--   0 runner    (1001) docker     (127)    35640 2024-03-25 18:33:26.000000 jolideco-0.2/docs/jolideco-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-03-25 18:33:26.000000 jolideco-0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)   573728 2024-03-25 18:33:26.000000 jolideco-0.2/docs/patch-priors.png
--rw-r--r--   0 runner    (1001) docker     (127)    32734 2024-03-25 18:33:26.000000 jolideco-0.2/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-25 18:33:26.000000 jolideco-0.2/docs/references.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.956836 jolideco-0.2/docs/user/
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-03-25 18:33:26.000000 jolideco-0.2/docs/user/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-25 18:33:26.000000 jolideco-0.2/docs/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-25 18:33:26.000000 jolideco-0.2/docs/user/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-03-25 18:33:26.000000 jolideco-0.2/docs/user/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-25 18:33:26.000000 jolideco-0.2/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.956836 jolideco-0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-25 18:33:26.000000 jolideco-0.2/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9162 2024-03-25 18:33:26.000000 jolideco-0.2/examples/chandra-e0102-filament.py
--rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-03-25 18:33:26.000000 jolideco-0.2/examples/fermi-vela-junior.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-03-25 18:33:26.000000 jolideco-0.2/examples/first-steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.960836 jolideco-0.2/jolideco/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.960836 jolideco-0.2/jolideco/data/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/data/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/data/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.960836 jolideco-0.2/jolideco/data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/data/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/data/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.960836 jolideco-0.2/jolideco/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.960836 jolideco-0.2/jolideco/models/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25370 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/models/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/models/npred.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.960836 jolideco-0.2/jolideco/models/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/models/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/models/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/models/tests/test_npred.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.964836 jolideco-0.2/jolideco/priors/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/priors/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/priors/lira.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.964836 jolideco-0.2/jolideco/priors/patches/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/priors/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/priors/patches/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/priors/patches/gmm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.964836 jolideco-0.2/jolideco/priors/patches/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/priors/patches/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/priors/patches/tests/test_gmm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.964836 jolideco-0.2/jolideco/priors/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/priors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/priors/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/priors/tests/test_lira.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.964836 jolideco-0.2/jolideco/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.964836 jolideco-0.2/jolideco/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.968836 jolideco-0.2/jolideco/utils/io/
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/io/asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12968 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/io/fits.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/io/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/norms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/sympy.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.968836 jolideco-0.2/jolideco/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/tests/test_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-03-25 18:33:26.000000 jolideco-0.2/jolideco/utils/torch.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-25 18:33:31.000000 jolideco-0.2/jolideco/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:33:31.968836 jolideco-0.2/jolideco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-03-25 18:33:31.000000 jolideco-0.2/jolideco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-25 18:33:31.000000 jolideco-0.2/jolideco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 18:33:31.000000 jolideco-0.2/jolideco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-25 18:33:31.000000 jolideco-0.2/jolideco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 18:33:31.000000 jolideco-0.2/jolideco.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-25 18:33:31.000000 jolideco-0.2/jolideco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-25 18:33:31.000000 jolideco-0.2/jolideco.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-25 18:33:26.000000 jolideco-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 18:33:31.968836 jolideco-0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-03-25 18:33:26.000000 jolideco-0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-25 18:33:26.000000 jolideco-0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.633242 jolideco-0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.613242 jolideco-0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.617241 jolideco-0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-23 20:58:13.000000 jolideco-0.3/.github/workflows/ci_cron_weekly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-23 20:58:13.000000 jolideco-0.3/.github/workflows/ci_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-23 20:58:13.000000 jolideco-0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-23 20:58:13.000000 jolideco-0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-23 20:58:13.000000 jolideco-0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-23 20:58:13.000000 jolideco-0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-23 20:58:13.000000 jolideco-0.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-23 20:58:13.000000 jolideco-0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-23 20:58:13.000000 jolideco-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 20:58:13.000000 jolideco-0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-23 20:58:19.633242 jolideco-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-23 20:58:13.000000 jolideco-0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.621241 jolideco-0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-23 20:58:13.000000 jolideco-0.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.613242 jolideco-0.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.621241 jolideco-0.3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-23 20:58:13.000000 jolideco-0.3/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.621241 jolideco-0.3/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   969644 2024-05-23 20:58:13.000000 jolideco-0.3/docs/_static/images/jolideco-example.png
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 20:58:13.000000 jolideco-0.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-23 20:58:13.000000 jolideco-0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-23 20:58:13.000000 jolideco-0.3/docs/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   460040 2024-05-23 20:58:13.000000 jolideco-0.3/docs/image-prior-intuition.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-23 20:58:13.000000 jolideco-0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   803093 2024-05-23 20:58:13.000000 jolideco-0.3/docs/jolideco-illustration.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35640 2024-05-23 20:58:13.000000 jolideco-0.3/docs/jolideco-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-23 20:58:13.000000 jolideco-0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)   573728 2024-05-23 20:58:13.000000 jolideco-0.3/docs/patch-priors.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32734 2024-05-23 20:58:13.000000 jolideco-0.3/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-23 20:58:13.000000 jolideco-0.3/docs/references.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.621241 jolideco-0.3/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-23 20:58:13.000000 jolideco-0.3/docs/user/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-23 20:58:13.000000 jolideco-0.3/docs/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-23 20:58:13.000000 jolideco-0.3/docs/user/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-23 20:58:13.000000 jolideco-0.3/docs/user/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 20:58:13.000000 jolideco-0.3/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.625242 jolideco-0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 20:58:13.000000 jolideco-0.3/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9162 2024-05-23 20:58:13.000000 jolideco-0.3/examples/chandra-e0102-filament.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-05-23 20:58:13.000000 jolideco-0.3/examples/fermi-vela-junior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-05-23 20:58:13.000000 jolideco-0.3/examples/first-steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.625242 jolideco-0.3/jolideco/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.625242 jolideco-0.3/jolideco/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/data/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.625242 jolideco-0.3/jolideco/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/data/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.625242 jolideco-0.3/jolideco/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.629242 jolideco-0.3/jolideco/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25370 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/models/npred.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.629242 jolideco-0.3/jolideco/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/models/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/models/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/models/tests/test_npred.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.629242 jolideco-0.3/jolideco/priors/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/priors/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/priors/lira.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.629242 jolideco-0.3/jolideco/priors/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/priors/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/priors/patches/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/priors/patches/gmm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.629242 jolideco-0.3/jolideco/priors/patches/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/priors/patches/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/priors/patches/tests/test_gmm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.629242 jolideco-0.3/jolideco/priors/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/priors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/priors/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/priors/tests/test_lira.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.629242 jolideco-0.3/jolideco/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.629242 jolideco-0.3/jolideco/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.633242 jolideco-0.3/jolideco/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/io/asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12968 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/io/fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/io/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/norms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/sympy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.633242 jolideco-0.3/jolideco/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/tests/test_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-23 20:58:13.000000 jolideco-0.3/jolideco/utils/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-23 20:58:19.000000 jolideco-0.3/jolideco/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:58:19.633242 jolideco-0.3/jolideco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-23 20:58:19.000000 jolideco-0.3/jolideco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-23 20:58:19.000000 jolideco-0.3/jolideco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:58:19.000000 jolideco-0.3/jolideco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 20:58:19.000000 jolideco-0.3/jolideco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:58:19.000000 jolideco-0.3/jolideco.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-23 20:58:19.000000 jolideco-0.3/jolideco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 20:58:19.000000 jolideco-0.3/jolideco.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-23 20:58:13.000000 jolideco-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:58:19.633242 jolideco-0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-05-23 20:58:13.000000 jolideco-0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-23 20:58:13.000000 jolideco-0.3/tox.ini
```

### Comparing `jolideco-0.2/.github/workflows/ci_cron_weekly.yml` & `jolideco-0.3/.github/workflows/ci_cron_weekly.yml`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/.github/workflows/ci_tests.yml` & `jolideco-0.3/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/.github/workflows/release.yml` & `jolideco-0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/.gitignore` & `jolideco-0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/.readthedocs.yaml` & `jolideco-0.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/CODE_OF_CONDUCT.md` & `jolideco-0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/LICENSE` & `jolideco-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/PKG-INFO` & `jolideco-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jolideco
-Version: 0.2
+Version: 0.3
 Summary: A Python package for Poisson joint likelihood deconvolution
 Author-email: Axel Donath <axel.donath@cfa.harvard.edu>
 License: BSD 3-Clause
 Project-URL: homepage, https://github.com/jolideco/jolideco
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Requires-Dist: torch>=1.13
@@ -34,23 +34,24 @@
 Requires-Dist: scipy; extra == "docs"
 Requires-Dist: sphinxemoji; extra == "docs"
 Requires-Dist: gammapy; extra == "docs"
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
-
 .. image:: https://readthedocs.org/projects/jolideco/badge/?version=latest
     :alt: Documentation Status
     :scale: 100%
     :target: https://jolideco.readthedocs.io/en/latest/?badge=latest
-
 .. image:: https://github.com/jolideco/jolideco/actions/workflows/ci_tests.yml/badge.svg?style=flat
     :target: https://github.com/jolideco/jolideco/actions
     :alt: GitHub actions CI
+.. image:: https://zenodo.org/badge/493477451.svg
+    :target: https://zenodo.org/doi/10.5281/zenodo.10870554
+    :alt: DOI
 
 
 Jolideco: a Python package for Poisson Joint Likelihood Deconvolution
 ---------------------------------------------------------------------
 
 .. image:: https://raw.githubusercontent.com/jolideco/jolideco/main/docs/jolideco-illustration.png
     :width: 600
@@ -70,17 +71,21 @@
 new features, bug fixes, documentation improvements, and more. If you are interested
 in contributing, please get in contact with the maintainers and make sure to read the
 `Code of Conduct <https://github.com/jolideco/jolideco/blob/main/CODE_OF_CONDUCT.md>`_.
 
 Citation
 --------
 
-When using Jolideco, please cite the following paper references:
+When using Jolideco, please cite the `version you used from Zenodo <https://zenodo.org/doi/10.5281/zenodo.10870554>`_ 
+and the following paper reference:
+
+.. code-block:: bibtex
+
+    TBD
 
-TBD
 
 Further Resources
 ------------------
 
 Please also take a look at the following associated repositories:
 
 - `Jolideco GMM Library <https://github.com/jolideco/jolideco-gmm-prior-library>`_
```

### Comparing `jolideco-0.2/README.rst` & `jolideco-0.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
-
 .. image:: https://readthedocs.org/projects/jolideco/badge/?version=latest
     :alt: Documentation Status
     :scale: 100%
     :target: https://jolideco.readthedocs.io/en/latest/?badge=latest
-
 .. image:: https://github.com/jolideco/jolideco/actions/workflows/ci_tests.yml/badge.svg?style=flat
     :target: https://github.com/jolideco/jolideco/actions
     :alt: GitHub actions CI
+.. image:: https://zenodo.org/badge/493477451.svg
+    :target: https://zenodo.org/doi/10.5281/zenodo.10870554
+    :alt: DOI
 
 
 Jolideco: a Python package for Poisson Joint Likelihood Deconvolution
 ---------------------------------------------------------------------
 
 .. image:: https://raw.githubusercontent.com/jolideco/jolideco/main/docs/jolideco-illustration.png
     :width: 600
@@ -33,17 +34,21 @@
 new features, bug fixes, documentation improvements, and more. If you are interested
 in contributing, please get in contact with the maintainers and make sure to read the
 `Code of Conduct <https://github.com/jolideco/jolideco/blob/main/CODE_OF_CONDUCT.md>`_.
 
 Citation
 --------
 
-When using Jolideco, please cite the following paper references:
+When using Jolideco, please cite the `version you used from Zenodo <https://zenodo.org/doi/10.5281/zenodo.10870554>`_ 
+and the following paper reference:
+
+.. code-block:: bibtex
+
+    TBD
 
-TBD
 
 Further Resources
 ------------------
 
 Please also take a look at the following associated repositories:
 
 - `Jolideco GMM Library <https://github.com/jolideco/jolideco-gmm-prior-library>`_
```

### Comparing `jolideco-0.2/docs/Makefile` & `jolideco-0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/_static/css/custom.css` & `jolideco-0.3/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/_static/images/jolideco-example.png` & `jolideco-0.3/docs/_static/images/jolideco-example.png`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/conf.py` & `jolideco-0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/developer.rst` & `jolideco-0.3/docs/developer.rst`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/image-prior-intuition.png` & `jolideco-0.3/docs/image-prior-intuition.png`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/index.rst` & `jolideco-0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/jolideco-illustration.png` & `jolideco-0.3/docs/jolideco-illustration.png`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/jolideco-logo.png` & `jolideco-0.3/docs/jolideco-logo.png`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/make.bat` & `jolideco-0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/patch-priors.png` & `jolideco-0.3/docs/patch-priors.png`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/references.bib` & `jolideco-0.3/docs/references.bib`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/references.rst` & `jolideco-0.3/docs/references.rst`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/user/getting-started.rst` & `jolideco-0.3/docs/user/getting-started.rst`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/user/installation.rst` & `jolideco-0.3/docs/user/installation.rst`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/docs/user/overview.rst` & `jolideco-0.3/docs/user/overview.rst`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/environment.yaml` & `jolideco-0.3/environment.yaml`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/examples/chandra-e0102-filament.py` & `jolideco-0.3/examples/chandra-e0102-filament.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Chandra Data Analysis With Jolideco
+Chandra Data Analysis with Jolideco
 ===================================
 
 In this tutorial we will demonstrate how to use Jolideco together with an example
 Chandra dataset to perform image deconvolution. We will use 24 observations of 
 a small region with an elomgated filament of the supernova remnant E0102. The
 dataset is available from Zenodo: https://zenodo.org/records/10849740
```

### Comparing `jolideco-0.2/examples/fermi-vela-junior.py` & `jolideco-0.3/examples/fermi-vela-junior.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/examples/first-steps.py` & `jolideco-0.3/examples/first-steps.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/__init__.py` & `jolideco-0.3/jolideco/__init__.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/cli.py` & `jolideco-0.3/jolideco/cli.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/conftest.py` & `jolideco-0.3/jolideco/conftest.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/core.py` & `jolideco-0.3/jolideco/core.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/data/core.py` & `jolideco-0.3/jolideco/data/core.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/data/tests/test_core.py` & `jolideco-0.3/jolideco/data/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/loss.py` & `jolideco-0.3/jolideco/loss.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/models/core.py` & `jolideco-0.3/jolideco/models/core.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/models/npred.py` & `jolideco-0.3/jolideco/models/npred.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/models/tests/test_core.py` & `jolideco-0.3/jolideco/models/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/models/tests/test_npred.py` & `jolideco-0.3/jolideco/models/tests/test_npred.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/priors/__init__.py` & `jolideco-0.3/jolideco/priors/__init__.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/priors/core.py` & `jolideco-0.3/jolideco/priors/core.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/priors/lira.py` & `jolideco-0.3/jolideco/priors/lira.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/priors/patches/core.py` & `jolideco-0.3/jolideco/priors/patches/core.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/priors/patches/gmm.py` & `jolideco-0.3/jolideco/priors/patches/gmm.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/priors/patches/tests/test_gmm.py` & `jolideco-0.3/jolideco/priors/patches/tests/test_gmm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pytest
 import numpy as np
 from numpy.testing import assert_allclose
 import torch
 from sklearn.mixture import GaussianMixture
 from sklearn.mixture._gaussian_mixture import _compute_precision_cholesky
 from jolideco.priors.patches import GMM_REGISTRY, GaussianMixtureModel
-from jolideco.utils.testing import requires_device
 
 
 def test_gmm_torch_basic():
     means = np.linspace(-1, 1, 9).reshape((1, 9))
     covariances = np.array([np.eye(9) for _ in means])
     weights = np.arange(9)
     weights = weights / weights.sum()
@@ -44,15 +43,15 @@
 
     values = gmm.estimate_log_prob(x=x)
 
     assert values.shape == (2, gmm.n_components)
     assert name in str(gmm)
 
 
-@requires_device("mps")
+@pytest.mark.xfail
 def test_gmm_mps():
     gmm = GaussianMixtureModel.from_registry(name="zoran-weiss").to("mps")
 
     x = torch.ones((2, 64)).to("mps")
 
     values = gmm.estimate_log_prob(x=x)
```

### Comparing `jolideco-0.2/jolideco/tests/test_core.py` & `jolideco-0.3/jolideco/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/utils/io/__init__.py` & `jolideco-0.3/jolideco/utils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/utils/io/asdf.py` & `jolideco-0.3/jolideco/utils/io/asdf.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/utils/io/fits.py` & `jolideco-0.3/jolideco/utils/io/fits.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/utils/io/yaml.py` & `jolideco-0.3/jolideco/utils/io/yaml.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/utils/misc.py` & `jolideco-0.3/jolideco/utils/misc.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/utils/norms.py` & `jolideco-0.3/jolideco/utils/norms.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/utils/numpy.py` & `jolideco-0.3/jolideco/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/utils/plot.py` & `jolideco-0.3/jolideco/utils/plot.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/utils/sympy.py` & `jolideco-0.3/jolideco/utils/sympy.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/utils/tests/test_numpy.py` & `jolideco-0.3/jolideco/utils/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/utils/tests/test_torch.py` & `jolideco-0.3/jolideco/utils/tests/test_torch.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco/utils/torch.py` & `jolideco-0.3/jolideco/utils/torch.py`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/jolideco.egg-info/PKG-INFO` & `jolideco-0.3/jolideco.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jolideco
-Version: 0.2
+Version: 0.3
 Summary: A Python package for Poisson joint likelihood deconvolution
 Author-email: Axel Donath <axel.donath@cfa.harvard.edu>
 License: BSD 3-Clause
 Project-URL: homepage, https://github.com/jolideco/jolideco
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Requires-Dist: torch>=1.13
@@ -34,23 +34,24 @@
 Requires-Dist: scipy; extra == "docs"
 Requires-Dist: sphinxemoji; extra == "docs"
 Requires-Dist: gammapy; extra == "docs"
 
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org
     :alt: Powered by Astropy Badge
-
 .. image:: https://readthedocs.org/projects/jolideco/badge/?version=latest
     :alt: Documentation Status
     :scale: 100%
     :target: https://jolideco.readthedocs.io/en/latest/?badge=latest
-
 .. image:: https://github.com/jolideco/jolideco/actions/workflows/ci_tests.yml/badge.svg?style=flat
     :target: https://github.com/jolideco/jolideco/actions
     :alt: GitHub actions CI
+.. image:: https://zenodo.org/badge/493477451.svg
+    :target: https://zenodo.org/doi/10.5281/zenodo.10870554
+    :alt: DOI
 
 
 Jolideco: a Python package for Poisson Joint Likelihood Deconvolution
 ---------------------------------------------------------------------
 
 .. image:: https://raw.githubusercontent.com/jolideco/jolideco/main/docs/jolideco-illustration.png
     :width: 600
@@ -70,17 +71,21 @@
 new features, bug fixes, documentation improvements, and more. If you are interested
 in contributing, please get in contact with the maintainers and make sure to read the
 `Code of Conduct <https://github.com/jolideco/jolideco/blob/main/CODE_OF_CONDUCT.md>`_.
 
 Citation
 --------
 
-When using Jolideco, please cite the following paper references:
+When using Jolideco, please cite the `version you used from Zenodo <https://zenodo.org/doi/10.5281/zenodo.10870554>`_ 
+and the following paper reference:
+
+.. code-block:: bibtex
+
+    TBD
 
-TBD
 
 Further Resources
 ------------------
 
 Please also take a look at the following associated repositories:
 
 - `Jolideco GMM Library <https://github.com/jolideco/jolideco-gmm-prior-library>`_
```

### Comparing `jolideco-0.2/jolideco.egg-info/SOURCES.txt` & `jolideco-0.3/jolideco.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
+CITATION.cff
 CODE_OF_CONDUCT.md
 LICENSE
 MANIFEST.in
 README.rst
 environment.yaml
 pyproject.toml
 setup.py
```

### Comparing `jolideco-0.2/pyproject.toml` & `jolideco-0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jolideco-0.2/tox.ini` & `jolideco-0.3/tox.ini`

 * *Files identical despite different names*

