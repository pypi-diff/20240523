# Comparing `tmp/rocm_docs_core-1.1.2.tar.gz` & `tmp/rocm_docs_core-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocm_docs_core-1.1.2.tar", last modified: Thu May 16 20:19:18 2024, max compression
+gzip compressed data, was "rocm_docs_core-1.1.3.tar", last modified: Wed May 22 22:40:37 2024, max compression
```

## Comparing `rocm_docs_core-1.1.2.tar` & `rocm_docs_core-1.1.3.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.316529 rocm_docs_core-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-16 20:19:18.316529 rocm_docs_core-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:19:18.316529 rocm_docs_core-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.296529 rocm_docs_core-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.300529 rocm_docs_core-1.1.2/src/rocm_docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.300529 rocm_docs_core-1.1.2/src/rocm_docs/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.300529 rocm_docs_core-1.1.2/src/rocm_docs/data/_doxygen/
--rw-r--r--   0 runner    (1001) docker     (127)    72476 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/data/_doxygen/extra_stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/data/_doxygen/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/data/_doxygen/header.html
--rw-r--r--   0 runner    (1001) docker     (127)    37255 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/data/_doxygen/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/data/projects.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/data/projects.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/doxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    17085 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.300529 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.300529 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/components/article-info.html
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/components/toggle-primary-sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.296529 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.300529 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm/footer.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm/left-side-menu.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.300529 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/footer.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/left-side-menu.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.304529 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/footer.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/left-side-menu.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.304529 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/sections/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.304529 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.296529 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.312529 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
--rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    16748 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    21924 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17872 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    20780 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    16808 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    21876 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17876 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    20672 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    16756 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    21820 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17780 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    20172 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    16372 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    21248 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17384 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    20664 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    16696 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    21520 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17544 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    27552 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    22132 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    29388 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    23712 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    27592 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    22184 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    29392 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    23824 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    27456 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    22212 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    29224 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    23676 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    26652 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    21516 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    28292 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    22904 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    27376 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    22040 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    28704 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    23168 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    29304 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    23704 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    27520 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    22084 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    21856 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    17820 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    20712 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (127)    16740 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts.css
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.312529 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      925 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1760 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)    10074 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
--rw-r--r--   0 runner    (1001) docker     (127)    19276 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/src/rocm_docs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.316529 rocm_docs_core-1.1.2/src/rocm_docs_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-16 20:19:18.000000 rocm_docs_core-1.1.2/src/rocm_docs_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-16 20:19:18.000000 rocm_docs_core-1.1.2/src/rocm_docs_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:19:18.000000 rocm_docs_core-1.1.2/src/rocm_docs_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 20:19:18.000000 rocm_docs_core-1.1.2/src/rocm_docs_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-16 20:19:18.000000 rocm_docs_core-1.1.2/src/rocm_docs_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 20:19:18.000000 rocm_docs_core-1.1.2/src/rocm_docs_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:18.316529 rocm_docs_core-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/tests/test_doxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:19:09.000000 rocm_docs_core-1.1.2/tests/test_sites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.940195 rocm_docs_core-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-22 22:40:37.940195 rocm_docs_core-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:40:37.940195 rocm_docs_core-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.912195 rocm_docs_core-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.916195 rocm_docs_core-1.1.3/src/rocm_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.916195 rocm_docs_core-1.1.3/src/rocm_docs/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.916195 rocm_docs_core-1.1.3/src/rocm_docs/data/_doxygen/
+-rw-r--r--   0 runner    (1001) docker     (127)    72476 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/data/_doxygen/extra_stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/data/_doxygen/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/data/_doxygen/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)    37255 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/data/_doxygen/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/data/projects.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/data/projects.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.916195 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.916195 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/components/article-info.html
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/components/toggle-primary-sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.912195 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.920195 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm/footer.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm/left-side-menu.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.920195 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/footer.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/left-side-menu.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.920195 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/footer.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/left-side-menu.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.920195 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/sections/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.920195 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.912195 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.932195 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16748 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21924 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17872 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20780 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16808 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21876 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17876 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20672 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16756 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21820 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17780 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20172 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16372 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21248 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17384 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20664 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16696 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21520 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17544 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27552 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22132 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29388 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23712 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27592 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22184 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29392 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23824 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27456 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22212 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29224 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23676 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26652 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21516 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28292 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22904 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27376 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22040 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28704 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23168 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29304 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23704 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27520 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22084 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21856 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17820 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20712 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16740 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.932195 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      925 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1760 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10074 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
+-rw-r--r--   0 runner    (1001) docker     (127)    19276 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/src/rocm_docs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.936195 rocm_docs_core-1.1.3/src/rocm_docs_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-22 22:40:37.000000 rocm_docs_core-1.1.3/src/rocm_docs_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-22 22:40:37.000000 rocm_docs_core-1.1.3/src/rocm_docs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:40:37.000000 rocm_docs_core-1.1.3/src/rocm_docs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 22:40:37.000000 rocm_docs_core-1.1.3/src/rocm_docs_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-22 22:40:37.000000 rocm_docs_core-1.1.3/src/rocm_docs_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 22:40:37.000000 rocm_docs_core-1.1.3/src/rocm_docs_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:37.936195 rocm_docs_core-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/tests/test_doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:40:29.000000 rocm_docs_core-1.1.3/tests/test_sites.py
```

### Comparing `rocm_docs_core-1.1.2/LICENSE.txt` & `rocm_docs_core-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/PKG-INFO` & `rocm_docs_core-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocm-docs-core
-Version: 1.1.2
+Version: 1.1.3
 Summary: Core utilities for all ROCm documentation on RTD
 Author-email: Lauren Wrubleski <Lauren.Wrubleski@amd.com>
 Project-URL: repository, https://github.com/RadeonOpenCompute/rocm-docs-core
 Project-URL: documentation, https://docs.amd.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rocm_docs_core-1.1.2/README.md` & `rocm_docs_core-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/pyproject.toml` & `rocm_docs_core-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'rocm-docs-core'
-version = "1.1.2"
+version = "1.1.3"
 authors=[
   {name="Lauren Wrubleski", email="Lauren.Wrubleski@amd.com"}
 ]
 description ='Core utilities for all ROCm documentation on RTD'
 readme="README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -68,15 +68,15 @@
 [tool.black]
 target-version = ["py310"]
 line-length = 80
 color = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.1.2"
+version = "1.1.3"
 version_files = ["pyproject.toml:^version", "docs/conf.py:^(version|release)"]
 tag_format = "v$version"
 annotated_tag = true
 
 [tool.isort]
 # https://github.com/timothycrosley/isort/
 py_version = "310"
```

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/__init__.py` & `rocm_docs_core-1.1.3/src/rocm_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/core.py` & `rocm_docs_core-1.1.3/src/rocm_docs/core.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/data/_doxygen/extra_stylesheet.css` & `rocm_docs_core-1.1.3/src/rocm_docs/data/_doxygen/extra_stylesheet.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/data/_doxygen/header.html` & `rocm_docs_core-1.1.3/src/rocm_docs/data/_doxygen/header.html`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/data/_doxygen/stylesheet.css` & `rocm_docs_core-1.1.3/src/rocm_docs/data/_doxygen/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/data/projects.schema.json` & `rocm_docs_core-1.1.3/src/rocm_docs/data/projects.schema.json`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/data/projects.yaml` & `rocm_docs_core-1.1.3/src/rocm_docs/data/projects.yaml`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/doxygen.py` & `rocm_docs_core-1.1.3/src/rocm_docs/doxygen.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/formatting.py` & `rocm_docs_core-1.1.3/src/rocm_docs/formatting.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/projects.py` & `rocm_docs_core-1.1.3/src/rocm_docs/projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,19 +320,19 @@
 
 
 def _update_theme_configs(
     app: Sphinx, current_project: _Project | None, current_branch: str
 ) -> None:
     """Update configurations for use in theme.py"""
     latest_version = requests.get(
-        "https://raw.githubusercontent.com/RadeonOpenCompute/rocm-docs-core/header-versions/latest_version.txt"
+        "https://raw.githubusercontent.com/ROCm/rocm-docs-core/header-versions/latest_version.txt"
     ).text.strip("\r\n")
     latest_version_string = f"docs-{latest_version}"
     release_candidate = requests.get(
-        "https://raw.githubusercontent.com/RadeonOpenCompute/rocm-docs-core/header-versions/release_candidate.txt"
+        "https://raw.githubusercontent.com/ROCm/rocm-docs-core/header-versions/release_candidate.txt"
     ).text.strip("\r\n")
     release_candidate_string = f"docs-{release_candidate}"
 
     development_branch = _Project.default_value("development_branch")
     if current_project is not None:
         development_branch = current_project.development_branch
```

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/components/article-info.html` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/components/article-info.html`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/sections/footer.html` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/sections/footer.html`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/sections/header.html` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/sections/header.html`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,19 @@
             </button>
             {% endif %}
             <div class="header-logo">
                 <a class="navbar-brand" href="https://www.amd.com/">
                     <img src="{{ pathto('_static/images/amd-header-logo.svg',1) }}" alt="AMD Logo" title="AMD Logo" width="90" class="d-inline-block align-text-top hover-opacity"/>
                 </a>
                 <div class="vr vr mx-40 my-25"></div>
-                {{ top_level_header(theme_repository_branch | replace("docs-", ""), theme_header_latest_version, theme_header_release_candidate_version) }}
+                {{ top_level_header(
+                    theme_repository_branch | replace("docs-", ""),
+                    header_latest_version,
+                    header_release_candidate_version
+                ) }}
                 {{ version_list() }}
             </div>
             <div class="icon-nav text-center d-flex ms-auto">
             </div>
         </div>
     </nav>
     {% if nav_secondary_items %}
```

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/custom.css` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/custom.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts.css` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts.css.map` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts.css.map`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/fonts.scss` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/fonts.scss`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/rocm_header.css` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/rocm_header.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js` & `rocm_docs_core-1.1.3/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/theme.py` & `rocm_docs_core-1.1.3/src/rocm_docs/theme.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,44 @@
 from sphinx.application import Sphinx
 
 from rocm_docs import util
 
 logger = sphinx.util.logging.getLogger(__name__)
 
 
+def _get_version_from_url(url: str) -> str:
+    try:
+        response = requests.get(url)
+        return response.text.strip()
+    except requests.RequestException as e:
+        print(f"Error in rocm-docs-core _get_version_from_url: {e}")
+        return ""
+
+
+def _add_custom_context(
+    app: Sphinx,  # noqa: ARG001
+    pagename: str,  # noqa: ARG001
+    templatename: str,  # noqa: ARG001
+    context: dict[str, str],
+    doctree: object,  # noqa: ARG001
+) -> None:
+    header_latest_version = _get_version_from_url(
+        "https://raw.githubusercontent.com/ROCm/rocm-docs-core/header-versions/latest_version.txt"
+    )
+
+    header_release_candidate_version = _get_version_from_url(
+        "https://raw.githubusercontent.com/ROCm/rocm-docs-core/header-versions/release_candidate.txt"
+    )
+
+    context["header_latest_version"] = header_latest_version
+    context["header_release_candidate_version"] = (
+        header_release_candidate_version
+    )
+
+
 def _update_repo_opts(srcdir: str, theme_opts: dict[str, Any]) -> None:
     default_branch_options: dict[str, Any] = {
         "use_edit_page_button": False,
     }
     try:
         url, branch = util.get_branch(srcdir)
         default_branch_options.update(
@@ -84,29 +114,30 @@
         theme_opts.setdefault(f"use_{button}_button", False)
 
     if theme_opts.get("link_main_doc", True):
         theme_opts.setdefault("navbar_center", []).insert(
             0, "components/left-side-menu"
         )
 
-    header_latest_version = requests.get(
+    header_latest_version = _get_version_from_url(
         "https://raw.githubusercontent.com/RadeonOpenCompute/rocm-docs-core/header-versions/latest_version.txt"
-    ).text.strip("\r\n")
-    header_release_candidate_version = requests.get(
+    )
+
+    header_release_candidate_version = _get_version_from_url(
         "https://raw.githubusercontent.com/RadeonOpenCompute/rocm-docs-core/header-versions/release_candidate.txt"
-    ).text.strip("\r\n")
+    )
 
     default_config_opts = {
         "html_show_sphinx": False,
         "html_favicon": "https://www.amd.com/themes/custom/amd/favicon.ico",
         "notfound_context": {"title": "404 - Page Not Found"},
         "notfound_template": "404.html",
         "html_context": {
-            "theme_header_latest_version": header_latest_version,
-            "theme_header_release_candidate_version": header_release_candidate_version,
+            "header_latest_version": header_latest_version,
+            "header_release_candidate_version": header_release_candidate_version,
         },
     }
     for key, default in default_config_opts.items():
         if not config_provided_by_user(app, key):
             setattr(app.config, key, default)
 
 
@@ -128,13 +159,14 @@
         "custom.css",
         "rocm_header.css",
         "rocm_footer.css",
         "fonts.css",
     ]:
         app.add_css_file(css)
 
+    app.connect("html-page-context", _add_custom_context)
     app.connect("builder-inited", _update_theme_options)
 
     return {
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs/util.py` & `rocm_docs_core-1.1.3/src/rocm_docs/util.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs_core.egg-info/PKG-INFO` & `rocm_docs_core-1.1.3/src/rocm_docs_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocm-docs-core
-Version: 1.1.2
+Version: 1.1.3
 Summary: Core utilities for all ROCm documentation on RTD
 Author-email: Lauren Wrubleski <Lauren.Wrubleski@amd.com>
 Project-URL: repository, https://github.com/RadeonOpenCompute/rocm-docs-core
 Project-URL: documentation, https://docs.amd.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rocm_docs_core-1.1.2/src/rocm_docs_core.egg-info/SOURCES.txt` & `rocm_docs_core-1.1.3/src/rocm_docs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/tests/test_doxygen.py` & `rocm_docs_core-1.1.3/tests/test_doxygen.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/tests/test_meta.py` & `rocm_docs_core-1.1.3/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.1.2/tests/test_projects.py` & `rocm_docs_core-1.1.3/tests/test_projects.py`

 * *Files identical despite different names*

