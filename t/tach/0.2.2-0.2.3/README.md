# Comparing `tmp/tach-0.2.2.tar.gz` & `tmp/tach-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tach-0.2.2.tar", last modified: Wed May 22 23:08:27 2024, max compression
+gzip compressed data, was "tach-0.2.3.tar", last modified: Thu May 23 16:48:29 2024, max compression
```

## Comparing `tach-0.2.2.tar` & `tach-0.2.3.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.523681 tach-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.531681 tach-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-22 23:08:22.000000 tach-0.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-22 23:08:22.000000 tach-0.2.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 23:08:22.000000 tach-0.2.2/.github/workflows/publish_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-22 23:08:22.000000 tach-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-22 23:08:22.000000 tach-0.2.2/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 23:08:22.000000 tach-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-22 23:08:27.547681 tach-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-22 23:08:22.000000 tach-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-22 23:08:22.000000 tach-0.2.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.531681 tach-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-22 23:08:22.000000 tach-0.2.2/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-22 23:08:22.000000 tach-0.2.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-22 23:08:22.000000 tach-0.2.2/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 23:08:22.000000 tach-0.2.2/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-22 23:08:22.000000 tach-0.2.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 23:08:22.000000 tach-0.2.2/docs/strict-mode.md
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 23:08:22.000000 tach-0.2.2/docs/tach-ignore.md
--rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-22 23:08:22.000000 tach-0.2.2/docs/tach_demo.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-22 23:08:22.000000 tach-0.2.2/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-22 23:08:22.000000 tach-0.2.2/docs/why-tach.md
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-22 23:08:22.000000 tach-0.2.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-22 23:08:22.000000 tach-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 23:08:27.547681 tach-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.535681 tach-0.2.2/tach/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-05-22 23:08:22.000000 tach-0.2.2/tach/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-22 23:08:22.000000 tach-0.2.2/tach/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-05-22 23:08:22.000000 tach-0.2.2/tach/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.535681 tach-0.2.2/tach/colors/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 23:08:22.000000 tach-0.2.2/tach/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 23:08:22.000000 tach-0.2.2/tach/colors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.535681 tach-0.2.2/tach/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-22 23:08:22.000000 tach-0.2.2/tach/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 23:08:22.000000 tach-0.2.2/tach/constants/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.535681 tach-0.2.2/tach/core/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-22 23:08:22.000000 tach-0.2.2/tach/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-22 23:08:22.000000 tach-0.2.2/tach/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-22 23:08:22.000000 tach-0.2.2/tach/core/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 23:08:22.000000 tach-0.2.2/tach/core/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.535681 tach-0.2.2/tach/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-22 23:08:22.000000 tach-0.2.2/tach/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 23:08:22.000000 tach-0.2.2/tach/errors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.535681 tach-0.2.2/tach/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-22 23:08:22.000000 tach-0.2.2/tach/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-22 23:08:22.000000 tach-0.2.2/tach/filesystem/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-22 23:08:22.000000 tach-0.2.2/tach/filesystem/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 23:08:22.000000 tach-0.2.2/tach/filesystem/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-22 23:08:22.000000 tach-0.2.2/tach/filesystem/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-05-22 23:08:22.000000 tach-0.2.2/tach/filesystem/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.539681 tach-0.2.2/tach/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-22 23:08:22.000000 tach-0.2.2/tach/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 23:08:22.000000 tach-0.2.2/tach/hooks/package.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      344 2024-05-22 23:08:22.000000 tach-0.2.2/tach/hooks/pre_commit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.539681 tach-0.2.2/tach/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 23:08:22.000000 tach-0.2.2/tach/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 23:08:22.000000 tach-0.2.2/tach/interactive/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19334 2024-05-22 23:08:22.000000 tach-0.2.2/tach/interactive/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-22 23:08:22.000000 tach-0.2.2/tach/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 23:08:22.000000 tach-0.2.2/tach/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.539681 tach-0.2.2/tach/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/ast_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-22 23:08:22.000000 tach-0.2.2/tach/parsing/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-22 23:08:22.000000 tach-0.2.2/tach/pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-22 23:08:22.000000 tach-0.2.2/tach/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/tach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-22 23:08:27.000000 tach-0.2.2/tach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-22 23:08:27.000000 tach-0.2.2/tach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:08:27.000000 tach-0.2.2/tach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 23:08:27.000000 tach-0.2.2/tach.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-22 23:08:27.000000 tach-0.2.2/tach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 23:08:27.000000 tach-0.2.2/tach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 23:08:22.000000 tach-0.2.2/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.539681 tach-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.539681 tach-0.2.2/tests/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/domain_one/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_one/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_one/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_three/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_two/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_two/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/domain_two/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_two/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/domain_two/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/invalid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/invalid/empty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/empty/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/empty/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/invalid/hidden/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.543681 tach-0.2.2/tests/example/invalid/hidden/.hidden/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/.hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/.hidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/tests/example/invalid/hidden/unhidden/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/unhidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/unhidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/hidden/unhidden/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/invalid/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/tests/example/valid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/tests/example/valid/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/tests/example/valid/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:08:27.547681 tach-0.2.2/tests/example/valid/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/domain_two/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 23:08:22.000000 tach-0.2.2/tests/example/valid/tach.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-22 23:08:22.000000 tach-0.2.2/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-22 23:08:22.000000 tach-0.2.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-22 23:08:22.000000 tach-0.2.2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-22 23:08:22.000000 tach-0.2.2/tests/test_package_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-22 23:08:22.000000 tach-0.2.2/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:08:22.000000 tach-0.2.2/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.968016 tach-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.948017 tach-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.952016 tach-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-23 16:48:25.000000 tach-0.2.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-23 16:48:25.000000 tach-0.2.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-23 16:48:25.000000 tach-0.2.3/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-23 16:48:25.000000 tach-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-23 16:48:25.000000 tach-0.2.3/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 16:48:25.000000 tach-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-23 16:48:29.968016 tach-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-23 16:48:25.000000 tach-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-23 16:48:25.000000 tach-0.2.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.952016 tach-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-23 16:48:25.000000 tach-0.2.3/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 16:48:25.000000 tach-0.2.3/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-23 16:48:25.000000 tach-0.2.3/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-23 16:48:25.000000 tach-0.2.3/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-23 16:48:25.000000 tach-0.2.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-23 16:48:25.000000 tach-0.2.3/docs/strict-mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-23 16:48:25.000000 tach-0.2.3/docs/tach-ignore.md
+-rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-23 16:48:25.000000 tach-0.2.3/docs/tach_demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-23 16:48:25.000000 tach-0.2.3/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-23 16:48:25.000000 tach-0.2.3/docs/why-tach.md
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-23 16:48:25.000000 tach-0.2.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-23 16:48:25.000000 tach-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 16:48:29.968016 tach-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.956016 tach-0.2.3/tach/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-23 16:48:25.000000 tach-0.2.3/tach/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-23 16:48:25.000000 tach-0.2.3/tach/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-23 16:48:25.000000 tach-0.2.3/tach/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.956016 tach-0.2.3/tach/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 16:48:25.000000 tach-0.2.3/tach/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 16:48:25.000000 tach-0.2.3/tach/colors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.956016 tach-0.2.3/tach/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-23 16:48:25.000000 tach-0.2.3/tach/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 16:48:25.000000 tach-0.2.3/tach/constants/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.956016 tach-0.2.3/tach/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-23 16:48:25.000000 tach-0.2.3/tach/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-23 16:48:25.000000 tach-0.2.3/tach/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-23 16:48:25.000000 tach-0.2.3/tach/core/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 16:48:25.000000 tach-0.2.3/tach/core/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.956016 tach-0.2.3/tach/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-23 16:48:25.000000 tach-0.2.3/tach/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 16:48:25.000000 tach-0.2.3/tach/errors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.956016 tach-0.2.3/tach/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-23 16:48:25.000000 tach-0.2.3/tach/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-23 16:48:25.000000 tach-0.2.3/tach/filesystem/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-23 16:48:25.000000 tach-0.2.3/tach/filesystem/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 16:48:25.000000 tach-0.2.3/tach/filesystem/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 16:48:25.000000 tach-0.2.3/tach/filesystem/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-23 16:48:25.000000 tach-0.2.3/tach/filesystem/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.960017 tach-0.2.3/tach/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-23 16:48:25.000000 tach-0.2.3/tach/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 16:48:25.000000 tach-0.2.3/tach/hooks/package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      380 2024-05-23 16:48:25.000000 tach-0.2.3/tach/hooks/pre_commit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.960017 tach-0.2.3/tach/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-23 16:48:25.000000 tach-0.2.3/tach/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 16:48:25.000000 tach-0.2.3/tach/interactive/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19370 2024-05-23 16:48:25.000000 tach-0.2.3/tach/interactive/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-23 16:48:25.000000 tach-0.2.3/tach/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 16:48:25.000000 tach-0.2.3/tach/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.960017 tach-0.2.3/tach/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-23 16:48:25.000000 tach-0.2.3/tach/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-23 16:48:25.000000 tach-0.2.3/tach/parsing/ast_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-23 16:48:25.000000 tach-0.2.3/tach/parsing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-23 16:48:25.000000 tach-0.2.3/tach/parsing/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-23 16:48:25.000000 tach-0.2.3/tach/parsing/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 16:48:25.000000 tach-0.2.3/tach/parsing/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-23 16:48:25.000000 tach-0.2.3/tach/parsing/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-23 16:48:25.000000 tach-0.2.3/tach/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-23 16:48:25.000000 tach-0.2.3/tach/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.968016 tach-0.2.3/tach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-23 16:48:29.000000 tach-0.2.3/tach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-23 16:48:29.000000 tach-0.2.3/tach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:48:29.000000 tach-0.2.3/tach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 16:48:29.000000 tach-0.2.3/tach.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 16:48:29.000000 tach-0.2.3/tach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 16:48:29.000000 tach-0.2.3/tach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-23 16:48:25.000000 tach-0.2.3/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.960017 tach-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.960017 tach-0.2.3/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.960017 tach-0.2.3/tests/example/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.960017 tach-0.2.3/tests/example/domain_one/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/domain_one/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/domain_one/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.964017 tach-0.2.3/tests/example/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/domain_three/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.964017 tach-0.2.3/tests/example/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/domain_two/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/domain_two/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.964017 tach-0.2.3/tests/example/domain_two/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/domain_two/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/domain_two/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.964017 tach-0.2.3/tests/example/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.964017 tach-0.2.3/tests/example/invalid/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/empty/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/empty/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.964017 tach-0.2.3/tests/example/invalid/hidden/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.964017 tach-0.2.3/tests/example/invalid/hidden/.hidden/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/hidden/.hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/hidden/.hidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/hidden/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.964017 tach-0.2.3/tests/example/invalid/hidden/unhidden/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/hidden/unhidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/hidden/unhidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/hidden/unhidden/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/invalid/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.964017 tach-0.2.3/tests/example/valid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/valid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.964017 tach-0.2.3/tests/example/valid/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/valid/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/valid/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.964017 tach-0.2.3/tests/example/valid/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/valid/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/valid/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:48:29.964017 tach-0.2.3/tests/example/valid/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/valid/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/valid/domain_two/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-23 16:48:25.000000 tach-0.2.3/tests/example/valid/tach.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-23 16:48:25.000000 tach-0.2.3/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-23 16:48:25.000000 tach-0.2.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-23 16:48:25.000000 tach-0.2.3/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-23 16:48:25.000000 tach-0.2.3/tests/test_package_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-23 16:48:25.000000 tach-0.2.3/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:48:25.000000 tach-0.2.3/tests/test_show.py
```

### Comparing `tach-0.2.2/.github/workflows/ci.yml` & `tach-0.2.3/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `tach-0.2.2/.github/workflows/publish.yml` & `tach-0.2.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/.github/workflows/publish_docs.yml` & `tach-0.2.3/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/.gitignore` & `tach-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/LICENSE` & `tach-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/PKG-INFO` & `tach-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/gauge-sh/tach
 Project-URL: Issues, https://github.com/gauge-sh/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tach-0.2.2/README.md` & `tach-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/docs/configuration.md` & `tach-0.2.3/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/docs/faq.md` & `tach-0.2.3/docs/faq.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/docs/favicon.ico` & `tach-0.2.3/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/docs/getting-started.md` & `tach-0.2.3/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/docs/index.md` & `tach-0.2.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/docs/strict-mode.md` & `tach-0.2.3/docs/strict-mode.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/docs/tach-ignore.md` & `tach-0.2.3/docs/tach-ignore.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/docs/tach_demo.mp4` & `tach-0.2.3/docs/tach_demo.mp4`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/docs/usage.md` & `tach-0.2.3/docs/usage.md`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 ### With pre-commit framework
 If you use the [pre-commit framework](https://github.com/pre-commit/pre-commit), you can add the following to your `.pre-commit-hooks.yaml`:
 
 ```yaml
 repos:
 -   repo: https://github.com/gauge-sh/tach
-    rev: v0.2.2  # change this to the latest tag!
+    rev: v0.2.3  # change this to the latest tag!
     hooks:
     -   id: tach
         # args: ["--root=backend_root"]
 ```
 
 Note that you should specify the version you are using in the `rev` key.
```

### Comparing `tach-0.2.2/docs/why-tach.md` & `tach-0.2.3/docs/why-tach.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/mkdocs.yml` & `tach-0.2.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/pyproject.toml` & `tach-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tach"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to maintain a modular package architecture."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -34,19 +34,26 @@
 keywords = ['python', 'module', 'package', 'guard', 'enforcement', 'boundary', 'enforcer', 'domain', 'architecture']
 
 
 [project.urls]
 Homepage = "https://github.com/gauge-sh/tach"
 Issues = "https://github.com/gauge-sh/tach/issues"
 
+[tool.ruff]
+target-version = "py38"
+lint.extend-select = ["I"]
+
+[tool.ruff.lint.isort]
+required-imports = ["from __future__ import annotations"]
 
 [tool.pyright]
 include = ["tach"]
 exclude = ["**/__pycache__", ".venv"]
 strict = ["tach"]
+pythonVersion = "3.8"
 
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm>=8.0"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
 tach = "tach.cli:main"
```

### Comparing `tach-0.2.2/tach/check.py` & `tach-0.2.3/tach/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from __future__ import annotations
+
 import os
 from dataclasses import dataclass, field
 from typing import Optional
 
-from tach import filesystem as fs
 from tach import errors
-from tach.core import PackageTrie, PackageNode, ProjectConfig
+from tach import filesystem as fs
+from tach.core import PackageNode, PackageTrie, ProjectConfig
 from tach.parsing import build_package_trie, get_project_imports
 
 
 @dataclass
 class ErrorInfo:
     source_tags: list[str] = field(default_factory=list)
     invalid_tags: list[str] = field(default_factory=list)
```

### Comparing `tach-0.2.2/tach/cli.py` & `tach-0.2.3/tach/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+from __future__ import annotations
+
 import argparse
 import os
 import sys
 from enum import Enum
 from functools import lru_cache
 from typing import Optional
 
-from tach.check import check, BoundaryError
 from tach import filesystem as fs
+from tach.check import BoundaryError, check
 from tach.clean import clean_project
+from tach.colors import BCOLORS
 from tach.constants import TOOL_NAME
 from tach.core import TagDependencyRules
 from tach.filesystem import install_pre_commit
-from tach.pkg import pkg_edit_interactive
-from tach.loading import stop_spinner, start_spinner
+from tach.loading import start_spinner, stop_spinner
 from tach.parsing import parse_project_config
-from tach.colors import BCOLORS
-from tach.sync import sync_project, prune_dependency_constraints
+from tach.pkg import pkg_edit_interactive
+from tach.sync import prune_dependency_constraints, sync_project
 
 
 class TerminalEnvironment(Enum):
     UNKNOWN = 1
     JETBRAINS = 2
     VSCODE = 3
```

### Comparing `tach-0.2.2/tach/core/config.py` & `tach-0.2.3/tach/core/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import List, Optional, Any
+from __future__ import annotations
+
+from typing import Any, List, Optional
 
 from pydantic import BaseModel, Field
 
 
 class Config(BaseModel):
     model_config = {"extra": "forbid"}
```

### Comparing `tach-0.2.2/tach/core/package.py` & `tach-0.2.3/tach/core/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 from collections import deque
 from dataclasses import dataclass, field
-from typing import Optional, Generator
+from typing import Generator, Optional
 
 from tach.core.config import PackageConfig
 
 
 @dataclass
 class PackageNode:
     """
```

### Comparing `tach-0.2.2/tach/filesystem/__init__.py` & `tach-0.2.3/tach/filesystem/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+from __future__ import annotations
+
+from tach.filesystem.install import install_pre_commit
+from tach.filesystem.package import (
+    validate_package_config,
+)
+from tach.filesystem.project import (
+    find_project_config_root,
+    get_project_config_path,
+    print_no_config_yml,
+    validate_project_config_path,
+)
 from tach.filesystem.service import (
-    get_cwd,
-    chdir,
     canonical,
-    read_file,
-    write_file,
+    chdir,
     delete_file,
+    file_to_module_path,
+    get_cwd,
+    is_project_import,
+    module_to_file_path,
     parse_ast,
+    read_file,
     walk,
+    walk_configured_packages,
     walk_pyfiles,
     walk_pypackages,
-    walk_configured_packages,
-    file_to_module_path,
-    module_to_file_path,
-    is_project_import,
-)
-from tach.filesystem.project import (
-    get_project_config_path,
-    validate_project_config_path,
-    print_no_config_yml,
-    find_project_config_root,
-)
-from tach.filesystem.package import (
-    validate_package_config,
+    write_file,
 )
-from tach.filesystem.install import install_pre_commit
 
 __all__ = [
     "get_cwd",
     "chdir",
     "canonical",
     "read_file",
     "write_file",
```

### Comparing `tach-0.2.2/tach/filesystem/install.py` & `tach-0.2.3/tach/filesystem/install.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 
 from tach.filesystem.service import mark_executable, write_file
 from tach.hooks import build_pre_commit_hook_content
 
 
 def install_pre_commit(path: str = ".", project_root: str = "") -> tuple[bool, str]:
```

### Comparing `tach-0.2.2/tach/filesystem/project.py` & `tach-0.2.3/tach/filesystem/project.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import sys
 from pathlib import Path
 from typing import Optional
 
 from tach.colors import BCOLORS
 from tach.constants import CONFIG_FILE_NAME
```

### Comparing `tach-0.2.2/tach/filesystem/service.py` & `tach-0.2.3/tach/filesystem/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-import os
+from __future__ import annotations
+
 import ast
+import os
 import re
 import stat
 import sys
 import threading
 from collections import defaultdict
 from dataclasses import dataclass
 from functools import lru_cache
 from pathlib import Path
-from typing import Optional, Generator
+from typing import Generator, Optional
+
 from tach import errors
 from tach.colors import BCOLORS
 
 
 @dataclass
 class FileInfo:
     path: str
```

### Comparing `tach-0.2.2/tach/interactive/packages.py` & `tach-0.2.3/tach/interactive/packages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,36 @@
+from __future__ import annotations
+
 import os
 import re
 from collections import deque
 from dataclasses import dataclass, field
 from enum import Enum
 from itertools import chain
-from typing import Optional, Generator, Callable, Union
+from typing import Callable, Generator, Optional, Union
 
 from prompt_toolkit import ANSI
+from prompt_toolkit.application import Application
 from prompt_toolkit.data_structures import Point
 from prompt_toolkit.formatted_text import AnyFormattedText
-from prompt_toolkit.widgets import Frame
-from rich.console import Console
-from rich.tree import Tree
-from rich.text import Text
-from prompt_toolkit.application import Application
 from prompt_toolkit.key_binding import KeyBindings, KeyPressEvent
 from prompt_toolkit.layout import (
-    Layout,
+    Container,
     HSplit,
-    Window,
+    Layout,
     ScrollablePane,
-    Container,
     VerticalAlign,
+    Window,
 )
 from prompt_toolkit.layout.controls import FormattedTextControl
 from prompt_toolkit.styles import Style
+from prompt_toolkit.widgets import Frame
+from rich.console import Console
+from rich.text import Text
+from rich.tree import Tree
 
 from tach import errors
 from tach import filesystem as fs
 from tach.constants import PACKAGE_FILE_NAME
 
 
 @dataclass
```

### Comparing `tach-0.2.2/tach/loading.py` & `tach-0.2.3/tach/loading.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import threading
-import sys
+from __future__ import annotations
+
 import itertools
 import queue
+import sys
+import threading
 import time
 
 SPINNER_CHARS = ".oOo"
 spinner_started = False
 SPINNER_CHAR_FPS = 3
 SPINNER_CHAR_TIME_DELAY = 1 / SPINNER_CHAR_FPS
 SPINNER_DELAY = 0.35
```

### Comparing `tach-0.2.2/tach/parsing/config.py` & `tach-0.2.3/tach/parsing/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from __future__ import annotations
+
 from typing import Optional
 
 import yaml
 
-from tach.colors import BCOLORS
-from tach.core import ProjectConfig, PackageConfig
 from tach import filesystem as fs
+from tach.colors import BCOLORS
+from tach.core import PackageConfig, ProjectConfig
 
 
 def dump_project_config_to_yaml(config: ProjectConfig) -> str:
     # Using sort_keys=False here and depending on config.model_dump maintaining 'insertion order'
     # so that 'tag' appears before 'depends_on'
     # Instead, should provide custom yaml.Dumper & yaml.Representer or just write our own
     # Sort only constraints and dependencies alphabetically for now
```

### Comparing `tach-0.2.2/tach/parsing/imports.py` & `tach-0.2.3/tach/parsing/imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 import ast
 import os
 import re
-from typing import Optional
 from dataclasses import dataclass, field
+from typing import Optional
 
 from tach import filesystem as fs
 
 
 @dataclass
 class IgnoreDirective:
     lineno: int
```

### Comparing `tach-0.2.2/tach/parsing/interface.py` & `tach-0.2.3/tach/parsing/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import ast
 import os
 from typing import Any
 
 from tach import filesystem as fs
 from tach.parsing.ast_visitor import EarlyExitNodeVisitor
```

### Comparing `tach-0.2.2/tach/parsing/packages.py` & `tach-0.2.3/tach/parsing/packages.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 from typing import Optional
 
 from tach import filesystem as fs
 from tach.core import PackageTrie
-from tach.parsing import parse_package_config, parse_interface_members
+from tach.parsing import parse_interface_members, parse_package_config
 
 
 def build_package_trie(
     root: str,
     exclude_paths: Optional[list[str]] = None,
     exclude_hidden_paths: Optional[bool] = True,
 ) -> PackageTrie:
```

### Comparing `tach-0.2.2/tach/pkg.py` & `tach-0.2.3/tach/pkg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from __future__ import annotations
+
 import os
-from dataclasses import field, dataclass
+from dataclasses import dataclass, field
 from typing import Optional
 
-
 from tach import errors
 from tach import filesystem as fs
 from tach.colors import BCOLORS
-from tach.constants import PACKAGE_FILE_NAME, CONFIG_FILE_NAME, TOOL_NAME
+from tach.constants import CONFIG_FILE_NAME, PACKAGE_FILE_NAME, TOOL_NAME
 from tach.core import ProjectConfig
-from tach.interactive import get_selected_packages_interactive, SelectedPackage
+from tach.interactive import SelectedPackage, get_selected_packages_interactive
 from tach.parsing import dump_project_config_to_yaml
 
 __package_yml_template = """tags: ['{dir_name}']\n"""
 
 
 @dataclass
 class SetPackagesResult:
```

### Comparing `tach-0.2.2/tach/sync.py` & `tach-0.2.3/tach/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from __future__ import annotations
+
 import os
 from typing import Optional
 
-from tach import filesystem as fs
 from tach import errors
+from tach import filesystem as fs
+from tach.check import check
 from tach.colors import BCOLORS
 from tach.constants import CONFIG_FILE_NAME
 from tach.core import ProjectConfig
-from tach.check import check
-from tach.parsing import parse_project_config, dump_project_config_to_yaml
+from tach.parsing import dump_project_config_to_yaml, parse_project_config
 
 
 def sync_dependency_constraints(
     root: str,
     project_config: ProjectConfig,
     filter_tags: Optional[set[str]] = None,
     exclude_paths: Optional[list[str]] = None,
```

### Comparing `tach-0.2.2/tach.egg-info/PKG-INFO` & `tach-0.2.3/tach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/gauge-sh/tach
 Project-URL: Issues, https://github.com/gauge-sh/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tach-0.2.2/tach.egg-info/SOURCES.txt` & `tach-0.2.3/tach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/tach.yml` & `tach-0.2.3/tach.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.2/tests/test_check.py` & `tach-0.2.3/tests/test_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from __future__ import annotations
+
 import pytest
+
+from tach.check import check_import
 from tach.core import (
     PackageConfig,
-    PackageTrie,
     PackageNode,
+    PackageTrie,
     ProjectConfig,
     TagDependencyRules,
 )
-from tach.check import check_import
 
 
 @pytest.fixture
 def test_config() -> PackageConfig:
     return PackageConfig(tags=["test"], strict=False)
```

### Comparing `tach-0.2.2/tests/test_cli.py` & `tach-0.2.3/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from __future__ import annotations
+
 from unittest.mock import Mock
+
 import pytest
 
 from tach import cli
-from tach.check import ErrorInfo, BoundaryError
+from tach.check import BoundaryError, ErrorInfo
 from tach.constants import CONFIG_FILE_NAME
 from tach.core import ProjectConfig, TagDependencyRules
 
 
 @pytest.fixture
 def mock_check(mocker) -> Mock:
     mock = Mock(return_value=[])  # default to a return with no errors
```

### Comparing `tach-0.2.2/tests/test_init.py` & `tach-0.2.3/tests/test_init.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-import pytest
-import tempfile
-import shutil
+from __future__ import annotations
+
 import os
-from tach import errors, filesystem as fs
+import shutil
+import tempfile
+
+import pytest
+
+from tach import errors
+from tach import filesystem as fs
 from tach.pkg import pkg_edit_interactive
 
 
 def init_project_from_root(root) -> None:
     # Save the current working directory
     saved_directory = os.getcwd()
     try:
```

### Comparing `tach-0.2.2/tests/test_package_trie.py` & `tach-0.2.3/tests/test_package_trie.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import pytest
 
-from tach.core import PackageTrie, PackageNode, PackageConfig
+from tach.core import PackageConfig, PackageNode, PackageTrie
 
 
 @pytest.fixture
 def test_config() -> PackageConfig:
     return PackageConfig(tags=["test"], strict=False)
```

### Comparing `tach-0.2.2/tests/test_parsing.py` & `tach-0.2.3/tests/test_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from __future__ import annotations
+
 import os
 
 import pytest
 from pydantic import ValidationError
 
+from tach import filesystem as fs
 from tach.check import check
-from tach.core.config import PackageConfig, TagDependencyRules, ProjectConfig
-from tach.parsing.config import parse_project_config, parse_package_config
+from tach.core.config import PackageConfig, ProjectConfig, TagDependencyRules
 from tach.filesystem import file_to_module_path
-from tach import filesystem as fs
+from tach.parsing.config import parse_package_config, parse_project_config
 
 
 def test_file_to_mod_path():
     assert file_to_module_path("__init__.py") == ""
     assert file_to_module_path("domain_one/__init__.py") == "domain_one"
     assert file_to_module_path("domain_one/interface.py") == "domain_one.interface"
```

