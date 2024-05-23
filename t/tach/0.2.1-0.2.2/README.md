# Comparing `tmp/tach-0.2.1.tar.gz` & `tmp/tach-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tach-0.2.1.tar", last modified: Wed May 22 18:24:19 2024, max compression
+gzip compressed data, was "tach-0.2.2.tar", last modified: Wed May 22 23:08:27 2024, max compression
```

## Comparing `tach-0.2.1.tar` & `tach-0.2.2.tar`

### file list

```diff
@@ -1,139 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.851595 tach-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.831595 tach-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.835595 tach-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-22 18:24:14.000000 tach-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-22 18:24:14.000000 tach-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 18:24:14.000000 tach-0.2.1/.github/workflows/publish_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-22 18:24:14.000000 tach-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-22 18:24:14.000000 tach-0.2.1/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 18:24:14.000000 tach-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-22 18:24:19.851595 tach-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-22 18:24:14.000000 tach-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-22 18:24:14.000000 tach-0.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.835595 tach-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-22 18:24:14.000000 tach-0.2.1/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-22 18:24:14.000000 tach-0.2.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-22 18:24:14.000000 tach-0.2.1/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 18:24:14.000000 tach-0.2.1/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-22 18:24:14.000000 tach-0.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 18:24:14.000000 tach-0.2.1/docs/strict-mode.md
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 18:24:14.000000 tach-0.2.1/docs/tach-ignore.md
--rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-22 18:24:14.000000 tach-0.2.1/docs/tach_demo.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-22 18:24:14.000000 tach-0.2.1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-22 18:24:14.000000 tach-0.2.1/docs/why-tach.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-22 18:24:14.000000 tach-0.2.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-22 18:24:14.000000 tach-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:24:19.851595 tach-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.839595 tach-0.2.1/tach/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-22 18:24:14.000000 tach-0.2.1/tach/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-05-22 18:24:14.000000 tach-0.2.1/tach/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-22 18:24:14.000000 tach-0.2.1/tach/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-05-22 18:24:14.000000 tach-0.2.1/tach/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.839595 tach-0.2.1/tach/colors/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 18:24:14.000000 tach-0.2.1/tach/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 18:24:14.000000 tach-0.2.1/tach/colors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.839595 tach-0.2.1/tach/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-22 18:24:14.000000 tach-0.2.1/tach/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 18:24:14.000000 tach-0.2.1/tach/constants/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.839595 tach-0.2.1/tach/core/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-22 18:24:14.000000 tach-0.2.1/tach/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-22 18:24:14.000000 tach-0.2.1/tach/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-22 18:24:14.000000 tach-0.2.1/tach/core/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 18:24:14.000000 tach-0.2.1/tach/core/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.843595 tach-0.2.1/tach/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-22 18:24:14.000000 tach-0.2.1/tach/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 18:24:14.000000 tach-0.2.1/tach/errors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.843595 tach-0.2.1/tach/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-22 18:24:14.000000 tach-0.2.1/tach/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-22 18:24:14.000000 tach-0.2.1/tach/filesystem/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-22 18:24:14.000000 tach-0.2.1/tach/filesystem/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 18:24:14.000000 tach-0.2.1/tach/filesystem/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-22 18:24:14.000000 tach-0.2.1/tach/filesystem/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-05-22 18:24:14.000000 tach-0.2.1/tach/filesystem/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.843595 tach-0.2.1/tach/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-22 18:24:14.000000 tach-0.2.1/tach/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 18:24:14.000000 tach-0.2.1/tach/hooks/package.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      344 2024-05-22 18:24:14.000000 tach-0.2.1/tach/hooks/pre_commit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.843595 tach-0.2.1/tach/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 18:24:14.000000 tach-0.2.1/tach/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 18:24:14.000000 tach-0.2.1/tach/interactive/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19334 2024-05-22 18:24:14.000000 tach-0.2.1/tach/interactive/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-22 18:24:14.000000 tach-0.2.1/tach/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 18:24:14.000000 tach-0.2.1/tach/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.843595 tach-0.2.1/tach/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/ast_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-22 18:24:14.000000 tach-0.2.1/tach/pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-22 18:24:14.000000 tach-0.2.1/tach/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.851595 tach-0.2.1/tach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-22 18:24:19.000000 tach-0.2.1/tach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-22 18:24:19.000000 tach-0.2.1/tach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:24:19.000000 tach-0.2.1/tach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 18:24:19.000000 tach-0.2.1/tach.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-22 18:24:19.000000 tach-0.2.1/tach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 18:24:19.000000 tach-0.2.1/tach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 18:24:14.000000 tach-0.2.1/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/domain_one/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_one/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_one/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_three/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_two/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_two/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/domain_two/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_two/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_two/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/invalid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/invalid/empty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/empty/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/empty/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/invalid/hidden/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/invalid/hidden/.hidden/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/.hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/.hidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/invalid/hidden/unhidden/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/unhidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/unhidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/unhidden/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.851595 tach-0.2.1/tests/example/valid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.851595 tach-0.2.1/tests/example/valid/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.851595 tach-0.2.1/tests/example/valid/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.851595 tach-0.2.1/tests/example/valid/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/domain_two/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/tach.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_package_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.523681 tach-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.531681 tach-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-22 23:08:22.000000 tach-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-22 23:08:22.000000 tach-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 23:08:22.000000 tach-0.2.2/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-22 23:08:22.000000 tach-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-22 23:08:22.000000 tach-0.2.2/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 23:08:22.000000 tach-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-22 23:08:27.547681 tach-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-22 23:08:22.000000 tach-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-22 23:08:22.000000 tach-0.2.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.531681 tach-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-22 23:08:22.000000 tach-0.2.2/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-22 23:08:22.000000 tach-0.2.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-22 23:08:22.000000 tach-0.2.2/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 23:08:22.000000 tach-0.2.2/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-22 23:08:22.000000 tach-0.2.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 23:08:22.000000 tach-0.2.2/docs/strict-mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 23:08:22.000000 tach-0.2.2/docs/tach-ignore.md
+-rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-22 23:08:22.000000 tach-0.2.2/docs/tach_demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-22 23:08:22.000000 tach-0.2.2/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-22 23:08:22.000000 tach-0.2.2/docs/why-tach.md
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-22 23:08:22.000000 tach-0.2.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-22 23:08:22.000000 tach-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 23:08:27.547681 tach-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.535681 tach-0.2.2/tach/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-05-22 23:08:22.000000 tach-0.2.2/tach/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-22 23:08:22.000000 tach-0.2.2/tach/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-05-22 23:08:22.000000 tach-0.2.2/tach/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.535681 tach-0.2.2/tach/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 23:08:22.000000 tach-0.2.2/tach/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 23:08:22.000000 tach-0.2.2/tach/colors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.535681 tach-0.2.2/tach/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-22 23:08:22.000000 tach-0.2.2/tach/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 23:08:22.000000 tach-0.2.2/tach/constants/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.535681 tach-0.2.2/tach/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-22 23:08:22.000000 tach-0.2.2/tach/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-22 23:08:22.000000 tach-0.2.2/tach/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-22 23:08:22.000000 tach-0.2.2/tach/core/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 23:08:22.000000 tach-0.2.2/tach/core/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.535681 tach-0.2.2/tach/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-22 23:08:22.000000 tach-0.2.2/tach/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 23:08:22.000000 tach-0.2.2/tach/errors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.535681 tach-0.2.2/tach/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-22 23:08:22.000000 tach-0.2.2/tach/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-22 23:08:22.000000 tach-0.2.2/tach/filesystem/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-22 23:08:22.000000 tach-0.2.2/tach/filesystem/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 23:08:22.000000 tach-0.2.2/tach/filesystem/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-22 23:08:22.000000 tach-0.2.2/tach/filesystem/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-05-22 23:08:22.000000 tach-0.2.2/tach/filesystem/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.539681 tach-0.2.2/tach/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-22 23:08:22.000000 tach-0.2.2/tach/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 23:08:22.000000 tach-0.2.2/tach/hooks/package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      344 2024-05-22 23:08:22.000000 tach-0.2.2/tach/hooks/pre_commit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.539681 tach-0.2.2/tach/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 23:08:22.000000 tach-0.2.2/tach/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 23:08:22.000000 tach-0.2.2/tach/interactive/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19334 2024-05-22 23:08:22.000000 tach-0.2.2/tach/interactive/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-22 23:08:22.000000 tach-0.2.2/tach/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 23:08:22.000000 tach-0.2.2/tach/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.539681 tach-0.2.2/tach/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/ast_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-22 23:08:22.000000 tach-0.2.2/tach/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-22 23:08:22.000000 tach-0.2.2/tach/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/tach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-22 23:08:27.000000 tach-0.2.2/tach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-22 23:08:27.000000 tach-0.2.2/tach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:08:27.000000 tach-0.2.2/tach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 23:08:27.000000 tach-0.2.2/tach.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-22 23:08:27.000000 tach-0.2.2/tach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 23:08:27.000000 tach-0.2.2/tach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 23:08:22.000000 tach-0.2.2/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.539681 tach-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.539681 tach-0.2.2/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/domain_one/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_one/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_one/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_three/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_two/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_two/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/domain_two/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_two/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_two/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/invalid/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/empty/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/empty/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/invalid/hidden/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/invalid/hidden/.hidden/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/.hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/.hidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/tests/example/invalid/hidden/unhidden/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/unhidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/unhidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/unhidden/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/tests/example/valid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/tests/example/valid/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/tests/example/valid/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/tests/example/valid/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/domain_two/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/tach.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-22 23:08:22.000000 tach-0.2.2/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-22 23:08:22.000000 tach-0.2.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-22 23:08:22.000000 tach-0.2.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-22 23:08:22.000000 tach-0.2.2/tests/test_package_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-22 23:08:22.000000 tach-0.2.2/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:08:22.000000 tach-0.2.2/tests/test_show.py
```

### Comparing `tach-0.2.1/.github/workflows/ci.yml` & `tach-0.2.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/.github/workflows/publish.yml` & `tach-0.2.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/.github/workflows/publish_docs.yml` & `tach-0.2.2/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/.gitignore` & `tach-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/LICENSE` & `tach-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/PKG-INFO` & `tach-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
-Project-URL: Homepage, https://github.com/never-over/tach
-Project-URL: Issues, https://github.com/never-over/tach/issues
+Project-URL: Homepage, https://github.com/gauge-sh/tach
+Project-URL: Issues, https://github.com/gauge-sh/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `tach-0.2.1/README.md` & `tach-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/docs/configuration.md` & `tach-0.2.2/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/docs/faq.md` & `tach-0.2.2/docs/faq.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/docs/favicon.ico` & `tach-0.2.2/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/docs/getting-started.md` & `tach-0.2.2/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/docs/index.md` & `tach-0.2.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/docs/strict-mode.md` & `tach-0.2.2/docs/strict-mode.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/docs/tach-ignore.md` & `tach-0.2.2/docs/tach-ignore.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/docs/tach_demo.mp4` & `tach-0.2.2/docs/tach_demo.mp4`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/docs/usage.md` & `tach-0.2.2/docs/usage.md`

 * *Files 0% similar despite different names*

```diff
@@ -102,16 +102,16 @@
 
 
 ### With pre-commit framework
 If you use the [pre-commit framework](https://github.com/pre-commit/pre-commit), you can add the following to your `.pre-commit-hooks.yaml`:
 
 ```yaml
 repos:
--   repo: https://github.com/Never-Over/tach
-    rev: v0.2.1  # change this to the latest tag!
+-   repo: https://github.com/gauge-sh/tach
+    rev: v0.2.2  # change this to the latest tag!
     hooks:
     -   id: tach
         # args: ["--root=backend_root"]
 ```
 
 Note that you should specify the version you are using in the `rev` key.
```

### Comparing `tach-0.2.1/docs/why-tach.md` & `tach-0.2.2/docs/why-tach.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/mkdocs.yml` & `tach-0.2.2/mkdocs.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # yaml-language-server: $schema=https://squidfunk.github.io/mkdocs-material/schema.json
 site_name: Tach
-site_url: https://never-over.github.io/tach/
+site_url: https://gauge-sh.github.io/tach/
 repo_name: tach
-repo_url: https://github.com/Never-Over/tach
+repo_url: https://github.com/gauge-sh/tach
 nav:
   - index.md
   - why-tach.md
   - getting-started.md
   - usage.md
   - configuration.md
   - strict-mode.md
```

### Comparing `tach-0.2.1/pyproject.toml` & `tach-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tach"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to maintain a modular package architecture."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -31,16 +31,16 @@
     "rich==13.7.1",
     "prompt-toolkit==3.0.43"
 ]
 keywords = ['python', 'module', 'package', 'guard', 'enforcement', 'boundary', 'enforcer', 'domain', 'architecture']
 
 
 [project.urls]
-Homepage = "https://github.com/never-over/tach"
-Issues = "https://github.com/never-over/tach/issues"
+Homepage = "https://github.com/gauge-sh/tach"
+Issues = "https://github.com/gauge-sh/tach/issues"
 
 
 [tool.pyright]
 include = ["tach"]
 exclude = ["**/__pycache__", ".venv"]
 strict = ["tach"]
```

### Comparing `tach-0.2.1/tach/check.py` & `tach-0.2.2/tach/check.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/cli.py` & `tach-0.2.2/tach/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,29 +201,24 @@
 
 
 def parse_arguments(
     args: list[str],
 ) -> tuple[argparse.Namespace, argparse.ArgumentParser]:
     parser = build_parser()
     parsed_args = parser.parse_args(args)
-
-    if args[0] not in ["pkg", "clean", "sync"]:
-        # TODO: unify project config handling
-        fs.validate_project_config_path()
-
     return parsed_args, parser
 
 
 def tach_check(
     root: str = ".",
     strict: bool = False,
     exclude_paths: Optional[list[str]] = None,
 ):
     try:
-        project_config = parse_project_config()
+        project_config = parse_project_config(root=root)
 
         if exclude_paths is not None and project_config.exclude is not None:
             exclude_paths.extend(project_config.exclude)
         else:
             exclude_paths = project_config.exclude
 
         boundary_errors: list[BoundaryError] = check(
```

### Comparing `tach-0.2.1/tach/core/config.py` & `tach-0.2.2/tach/core/config.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/core/package.py` & `tach-0.2.2/tach/core/package.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/filesystem/__init__.py` & `tach-0.2.2/tach/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/filesystem/install.py` & `tach-0.2.2/tach/filesystem/install.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/filesystem/project.py` & `tach-0.2.2/tach/filesystem/project.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/filesystem/service.py` & `tach-0.2.2/tach/filesystem/service.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/interactive/packages.py` & `tach-0.2.2/tach/interactive/packages.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/loading.py` & `tach-0.2.2/tach/loading.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/parsing/config.py` & `tach-0.2.2/tach/parsing/config.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/parsing/imports.py` & `tach-0.2.2/tach/parsing/imports.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/parsing/interface.py` & `tach-0.2.2/tach/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/parsing/packages.py` & `tach-0.2.2/tach/parsing/packages.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/pkg.py` & `tach-0.2.2/tach/pkg.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach/sync.py` & `tach-0.2.2/tach/sync.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tach.egg-info/PKG-INFO` & `tach-0.2.2/tach.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
-Project-URL: Homepage, https://github.com/never-over/tach
-Project-URL: Issues, https://github.com/never-over/tach/issues
+Project-URL: Homepage, https://github.com/gauge-sh/tach
+Project-URL: Issues, https://github.com/gauge-sh/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `tach-0.2.1/tach.egg-info/SOURCES.txt` & `tach-0.2.2/tach.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 docs/index.md
 docs/strict-mode.md
 docs/tach-ignore.md
 docs/tach_demo.mp4
 docs/usage.md
 docs/why-tach.md
 tach/__init__.py
-tach/add.py
 tach/check.py
 tach/clean.py
 tach/cli.py
 tach/loading.py
 tach/package.yml
 tach/pkg.py
 tach/sync.py
@@ -60,15 +59,14 @@
 tach/parsing/ast_visitor.py
 tach/parsing/config.py
 tach/parsing/imports.py
 tach/parsing/interface.py
 tach/parsing/package.yml
 tach/parsing/packages.py
 tests/__init__.py
-tests/test_add.py
 tests/test_check.py
 tests/test_cli.py
 tests/test_init.py
 tests/test_package_trie.py
 tests/test_parsing.py
 tests/test_show.py
 tests/example/__init__.py
```

### Comparing `tach-0.2.1/tach.yml` & `tach-0.2.2/tach.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tests/test_check.py` & `tach-0.2.2/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tests/test_cli.py` & `tach-0.2.2/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             return False
 
     mocker.patch("tach.filesystem.project.os.path.exists", mock_path_exists)
 
 
 @pytest.fixture
 def mock_project_config(mocker) -> None:
-    def mock_project_config() -> ProjectConfig:
+    def mock_project_config(root: str = "") -> ProjectConfig:
         return ProjectConfig(
             constraints=[TagDependencyRules(tag="mocked", depends_on=["mocked"])]
         )
 
     mocker.patch("tach.cli.parse_project_config", mock_project_config)
 
 
@@ -78,23 +78,14 @@
         cli.tach_check()
     captured = capfd.readouterr()
     assert sys_exit.value.code == 1
     assert location in captured.err
     assert message in captured.err
 
 
-def test_execute_with_no_tach_yml(capfd):
-    with pytest.raises(SystemExit) as sys_exit:
-        # Test with no tach.yml mocked
-        cli.parse_arguments(["check"])
-    captured = capfd.readouterr()
-    assert sys_exit.value.code == 1
-    assert "tach.(yml|yaml) not found" in captured.err
-
-
 def test_invalid_command(capfd):
     with pytest.raises(SystemExit) as sys_exit:
         # Test with an invalid command
         cli.parse_arguments(["help"])
     captured = capfd.readouterr()
     assert sys_exit.value.code == 2
     assert "invalid choice: 'help" in captured.err
```

### Comparing `tach-0.2.1/tests/test_init.py` & `tach-0.2.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tests/test_package_trie.py` & `tach-0.2.2/tests/test_package_trie.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.1/tests/test_parsing.py` & `tach-0.2.2/tests/test_parsing.py`

 * *Files identical despite different names*

