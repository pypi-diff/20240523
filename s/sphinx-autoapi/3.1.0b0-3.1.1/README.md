# Comparing `tmp/sphinx_autoapi-3.1b0.tar.gz` & `tmp/sphinx_autoapi-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_autoapi-3.1b0.tar", last modified: Fri Apr 12 16:55:39 2024, max compression
+gzip compressed data, was "sphinx_autoapi-3.1.1.tar", last modified: Thu May 23 03:52:51 2024, max compression
```

## Comparing `sphinx_autoapi-3.1b0.tar` & `sphinx_autoapi-3.1.1.tar`

### file list

```diff
@@ -1,173 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.483732 sphinx_autoapi-3.1b0/
--rw-r--r--   0 runner    (1001) docker     (127)    21226 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-12 16:55:39.483732 sphinx_autoapi-3.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.463732 sphinx_autoapi-3.1b0/autoapi/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/_astroid_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22011 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    16244 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    11540 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/directives.py
--rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/documenters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/inheritance_diagrams.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.463732 sphinx_autoapi-3.1b0/autoapi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.463732 sphinx_autoapi-3.1b0/autoapi/templates/python/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/exception.rst
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/method.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/package.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/property.rst
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-12 16:55:39.483732 sphinx_autoapi-3.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-12 16:55:39.000000 sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-12 16:55:39.000000 sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:55:39.000000 sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 16:55:39.000000 sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 16:55:39.000000 sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/pep695/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pep695/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/pep695/example/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pep695/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pep695/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/py310unionpipe/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py310unionpipe/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/py310unionpipe/example/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py310unionpipe/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py310unionpipe/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/py38positionalparams/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py38positionalparams/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/py38positionalparams/example/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py38positionalparams/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py38positionalparams/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/py3example/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3example/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/py3example/example/
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3example/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3example/example/example2.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3example/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.455732 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/namespace/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/namespace/example/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/namespace/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/namespace/sibling/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/namespace/sibling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/namespace/sibling/sub_sibling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyannotationcommentsexample/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyannotationcommentsexample/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyannotationcommentsexample/example/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyannotationcommentsexample/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyannotationcommentsexample/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/example/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/example/example2.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyemptyexample/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyemptyexample/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyemptyexample/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyexample/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyexample/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyexample/example/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyexample/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyexample/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyexample/manualapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyexample/null.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyiexample/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyiexample/example/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample/example/example.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pyiexample2/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample2/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pyiexample2/example/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample2/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample2/example/example.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/example/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/example/submodule_foo/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/example/submodule_foo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/confpy/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/confpy/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/example/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/manualapi.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/_private_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/binary_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/subpackage/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/subpackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/subpackage/submodule.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/unicode_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildall/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildall/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildall/simple/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildall/simple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildcard/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildcard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildchain/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildchain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildwildchain/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildwildchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackageexample/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/_private_submodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/submodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/subpackage/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/subpackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/subpackage/submodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pyskipexample/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyskipexample/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pyskipexample/example/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyskipexample/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyskipexample/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    41176 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/test_own_page_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    42840 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/test_pyintegration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/templateexample/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/templateexample/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/templateexample/example/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/templateexample/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/templateexample/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.459732 sphinx_autoapi-3.1b0/tests/templateexample/template_overrides/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/templateexample/template_overrides/python/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/templateexample/template_overrides/python/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/test_astroid_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/toctreeexample/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/toctreeexample/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/toctreeexample/example/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/toctreeexample/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/toctreeexample/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.770370 sphinx_autoapi-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    21425 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-23 03:52:51.770370 sphinx_autoapi-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.750370 sphinx_autoapi-3.1.1/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/_astroid_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22208 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16217 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11540 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/documenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11295 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/inheritance_diagrams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.750370 sphinx_autoapi-3.1.1/autoapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/templates/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.750370 sphinx_autoapi-3.1.1/autoapi/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/templates/python/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/templates/python/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/templates/python/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/templates/python/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/templates/python/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/templates/python/method.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/templates/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/templates/python/package.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/autoapi/templates/python/property.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-23 03:52:51.770370 sphinx_autoapi-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.770370 sphinx_autoapi-3.1.1/sphinx_autoapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-23 03:52:51.000000 sphinx_autoapi-3.1.1/sphinx_autoapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-23 03:52:51.000000 sphinx_autoapi-3.1.1/sphinx_autoapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:52:51.000000 sphinx_autoapi-3.1.1/sphinx_autoapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 03:52:51.000000 sphinx_autoapi-3.1.1/sphinx_autoapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 03:52:51.000000 sphinx_autoapi-3.1.1/sphinx_autoapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.754370 sphinx_autoapi-3.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.754370 sphinx_autoapi-3.1.1/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.754370 sphinx_autoapi-3.1.1/tests/python/pep695/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pep695/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.754370 sphinx_autoapi-3.1.1/tests/python/pep695/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pep695/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pep695/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.754370 sphinx_autoapi-3.1.1/tests/python/py310unionpipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py310unionpipe/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.754370 sphinx_autoapi-3.1.1/tests/python/py310unionpipe/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py310unionpipe/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py310unionpipe/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.754370 sphinx_autoapi-3.1.1/tests/python/py38positionalparams/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py38positionalparams/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.754370 sphinx_autoapi-3.1.1/tests/python/py38positionalparams/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py38positionalparams/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py38positionalparams/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.754370 sphinx_autoapi-3.1.1/tests/python/py3example/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py3example/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.754370 sphinx_autoapi-3.1.1/tests/python/py3example/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py3example/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py3example/example/example2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py3example/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.754370 sphinx_autoapi-3.1.1/tests/python/py3implicitnamespace/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py3implicitnamespace/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py3implicitnamespace/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.742370 sphinx_autoapi-3.1.1/tests/python/py3implicitnamespace/namespace/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.758370 sphinx_autoapi-3.1.1/tests/python/py3implicitnamespace/namespace/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py3implicitnamespace/namespace/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.758370 sphinx_autoapi-3.1.1/tests/python/py3implicitnamespace/namespace/sibling/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py3implicitnamespace/namespace/sibling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/py3implicitnamespace/namespace/sibling/sub_sibling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.758370 sphinx_autoapi-3.1.1/tests/python/pyannotationcommentsexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyannotationcommentsexample/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.758370 sphinx_autoapi-3.1.1/tests/python/pyannotationcommentsexample/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyannotationcommentsexample/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyannotationcommentsexample/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.758370 sphinx_autoapi-3.1.1/tests/python/pyautodoc_typehints/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyautodoc_typehints/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.758370 sphinx_autoapi-3.1.1/tests/python/pyautodoc_typehints/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyautodoc_typehints/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyautodoc_typehints/example/example2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyautodoc_typehints/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.758370 sphinx_autoapi-3.1.1/tests/python/pyemptyexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyemptyexample/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyemptyexample/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.758370 sphinx_autoapi-3.1.1/tests/python/pyexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyexample/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.758370 sphinx_autoapi-3.1.1/tests/python/pyexample/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyexample/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyexample/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyexample/manualapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyexample/null.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.758370 sphinx_autoapi-3.1.1/tests/python/pyiexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyiexample/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.758370 sphinx_autoapi-3.1.1/tests/python/pyiexample/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyiexample/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyiexample/example/example.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyiexample/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.758370 sphinx_autoapi-3.1.1/tests/python/pyiexample2/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyiexample2/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.762370 sphinx_autoapi-3.1.1/tests/python/pyiexample2/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyiexample2/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyiexample2/example/example.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyiexample2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.762370 sphinx_autoapi-3.1.1/tests/python/pyisubmoduleinit/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyisubmoduleinit/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.762370 sphinx_autoapi-3.1.1/tests/python/pyisubmoduleinit/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyisubmoduleinit/example/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.762370 sphinx_autoapi-3.1.1/tests/python/pyisubmoduleinit/example/submodule_foo/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyisubmoduleinit/example/submodule_foo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyisubmoduleinit/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.762370 sphinx_autoapi-3.1.1/tests/python/pymovedconfpy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.762370 sphinx_autoapi-3.1.1/tests/python/pymovedconfpy/confpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pymovedconfpy/confpy/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.762370 sphinx_autoapi-3.1.1/tests/python/pymovedconfpy/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pymovedconfpy/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pymovedconfpy/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pymovedconfpy/manualapi.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.762370 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.762370 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/_private_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/binary_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.762370 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/subpackage/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/subpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/subpackage/submodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/unicode_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.762370 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/wildall/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/wildall/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.762370 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/wildall/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/wildall/simple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/wildcard/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/wildcard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/wildchain/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/wildchain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/wildwildchain/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/wildwildchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/python/pypackageexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackageexample/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackageexample/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/_private_submodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/_private_subpackage/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/_private_subpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/_private_subpackage/submodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/_private_subpackage/subpackage/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/_private_subpackage/subpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/_private_subpackage/subpackage/submodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/submodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/subpackage/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/subpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/subpackage/submodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/python/pyskipexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyskipexample/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/python/pyskipexample/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyskipexample/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/pyskipexample/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    41176 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/test_own_page_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42840 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/python/test_pyintegration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/templateexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/templateexample/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/templateexample/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/templateexample/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/templateexample/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.746370 sphinx_autoapi-3.1.1/tests/templateexample/template_overrides/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/templateexample/template_overrides/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/templateexample/template_overrides/python/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/test_astroid_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.766370 sphinx_autoapi-3.1.1/tests/toctreeexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/toctreeexample/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:52:51.770370 sphinx_autoapi-3.1.1/tests/toctreeexample/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/toctreeexample/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-23 03:52:48.000000 sphinx_autoapi-3.1.1/tests/toctreeexample/index.rst
```

### Comparing `sphinx_autoapi-3.1b0/CHANGELOG.rst` & `sphinx_autoapi-3.1.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 Changelog
 =========
 
 Versions follow `Semantic Versioning <https://semver.org/>`_ (``<major>.<minor>.<patch>``).
 
 .. towncrier release notes start
 
-v3.1.0.b0 (2024-04-12)
-----------------------
+v3.1.1 (2024-05-22)
+-------------------
+
+Bugfixes
+^^^^^^^^
+
+- Fix private subpackages causing orphan pages (#446)
+
+
+v3.1.0 (2024-05-20)
+-------------------
 
 Features
 ^^^^^^^^
 
 - Objects can render to their own page (#226)
 - Render PEP-695 type aliases as TypeAlias assignments. (#414)
 
@@ -19,14 +28,15 @@
 ^^^^^^^^
 
 - Values are always rendered for TypeAlises and PEP-695 type aliases. (#224)
 - Fix submodule with `__init__.pyi` documented as `__init__` instead of submodule name (#398)
 - Fix IndexError when a module docstring contains only a heading (#412)
 - Preserve strings inside Literal type annotations (#423)
 - Stopped using xrefs in page titles (#427)
+- Fix unpickable configuration value warning when using autoapi_prepare_jinja_env (#445)
 - Fix emitting ignore event twice for methods.
 
 
 Misc
 ^^^^
 
 - #388
```

### Comparing `sphinx_autoapi-3.1b0/LICENSE.rst` & `sphinx_autoapi-3.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/PKG-INFO` & `sphinx_autoapi-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-autoapi
-Version: 3.1.0b0
+Version: 3.1.1
 Summary: Sphinx API documentation generator
 Home-page: http://github.com/readthedocs/sphinx-autoapi
 Author: Eric Holscher
 Author-email: eric@ericholscher.com
 Maintainer: Ashley Whetter
 Maintainer-email: ashley@awhetter.co.uk
 License: MIT
```

### Comparing `sphinx_autoapi-3.1b0/README.rst` & `sphinx_autoapi-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/autoapi/_astroid_utils.py` & `sphinx_autoapi-3.1.1/autoapi/_astroid_utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/autoapi/_mapper.py` & `sphinx_autoapi-3.1.1/autoapi/_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import collections
 import copy
 import fnmatch
+import itertools
 import operator
 import os
 import re
 
 from jinja2 import Environment, FileSystemLoader
 import sphinx
 import sphinx.environment
@@ -23,15 +24,14 @@
     PythonModule,
     PythonMethod,
     PythonPackage,
     PythonProperty,
     PythonAttribute,
     PythonData,
     PythonException,
-    TopLevelPythonPythonMapper,
 )
 from .settings import OWN_PAGE_LEVELS, TEMPLATE_DIR
 
 LOGGER = sphinx.util.logging.getLogger(__name__)
 
 
 def _expand_wildcard_placeholder(original_module, originals_map, placeholder):
@@ -329,33 +329,14 @@
                         # Make sure the path is full
                         if not os.path.isabs(filename):
                             filename = os.path.join(root, filename)
 
                         yield filename
                         seen.add(norm_name)
 
-    def add_object(self, obj):
-        """Add object to local and app environment storage
-
-        Args:
-            obj: Instance of a AutoAPI object
-        """
-        display = obj.display
-        if display and obj.type in self.own_page_types:
-            self.objects_to_render[obj.id] = obj
-
-        self.all_objects[obj.id] = obj
-        child_stack = list(obj.children)
-        while child_stack:
-            child = child_stack.pop()
-            self.all_objects[child.id] = child
-            if display and child.type in self.own_page_types:
-                self.objects_to_render[child.id] = child
-            child_stack.extend(getattr(child, "children", ()))
-
     def output_rst(self, source_suffix):
         for _, obj in status_iterator(
             self.objects_to_render.items(),
             colorize("bold", "[AutoAPI] ") + "Rendering Data... ",
             length=len(self.objects_to_render),
             verbosity=1,
             stringify_func=(lambda x: x[0]),
@@ -495,35 +476,58 @@
         for _, data in status_iterator(
             self.paths.items(),
             colorize("bold", "[AutoAPI] ") + "Mapping Data... ",
             length=len(self.paths),
             stringify_func=(lambda x: x[0]),
         ):
             for obj in self.create_class(data, options=options):
-                self.add_object(obj)
+                self.all_objects[obj.id] = obj
+
+        self._create_module_hierarchy()
+        self._render_selection()
+
+        self.app.env.autoapi_objects = self.objects_to_render
+        self.app.env.autoapi_all_objects = self.all_objects
 
-        top_level_objects = {
-            obj.id: obj
-            for obj in self.all_objects.values()
-            if isinstance(obj, TopLevelPythonPythonMapper)
-        }
-        parents = {obj.name: obj for obj in top_level_objects.values()}
-        for obj in top_level_objects.values():
+    def _create_module_hierarchy(self) -> None:
+        """Populate the sub{module,package}s attributes of all top level objects."""
+        for obj in self.all_objects.values():
             parent_name = obj.name.rsplit(".", 1)[0]
-            if parent_name in parents and parent_name != obj.name:
-                parent = parents[parent_name]
+            if parent_name in self.all_objects and parent_name != obj.name:
+                parent = self.all_objects[parent_name]
                 attr = f"sub{obj.type}s"
                 getattr(parent, attr).append(obj)
 
-        for obj in top_level_objects.values():
+        for obj in self.all_objects.values():
             obj.submodules.sort()
             obj.subpackages.sort()
 
-        self.app.env.autoapi_objects = self.objects_to_render
-        self.app.env.autoapi_all_objects = self.all_objects
+    def _render_selection(self):
+        """Propagate display values to children."""
+        for obj in sorted(self.all_objects.values(), key=lambda obj: len(obj.id)):
+            if obj.display:
+                assert obj.type in self.own_page_types
+                self.objects_to_render[obj.id] = obj
+            else:
+                for module in itertools.chain(obj.subpackages, obj.submodules):
+                    module.obj["hide"] = True
+
+        def _inner(parent):
+            for child in parent.children:
+                self.all_objects[child.id] = child
+                if not parent.display:
+                    child.obj["hide"] = True
+
+                if child.display and child.type in self.own_page_types:
+                    self.objects_to_render[child.id] = child
+
+                _inner(child)
+
+        for obj in list(self.all_objects.values()):
+            _inner(obj)
 
     def create_class(self, data, options=None):
         """Create a class from the passed in data
 
         Args:
             data: dictionary data of parser output
         """
```

### Comparing `sphinx_autoapi-3.1b0/autoapi/_objects.py` & `sphinx_autoapi-3.1.1/autoapi/_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         For example, the classes and functions defined in the parent module.
         """
         self._docstring: str = obj["doc"]
         self.imported: bool = "original_path" in obj
         """Whether this object was imported from another module."""
         self.inherited: bool = obj.get("inherited", False)
         """Whether this was inherited from an ancestor of the parent class."""
-        self._hide = obj.get("hide", False)
 
         # For later
         self._class_content = class_content
         self._display_cache: Optional[bool] = None
 
     def __getstate__(self):
         """Obtains serialisable data for pickling."""
@@ -230,15 +229,15 @@
         )
         skip_imported_member = self.imported and "imported-members" not in self.options
         skip_inherited_member = (
             self.inherited and "inherited-members" not in self.options
         )
 
         return (
-            self._hide
+            self.obj.get("hide", False)
             or skip_undoc_member
             or skip_private_member
             or skip_special_member
             or skip_imported_member
             or skip_inherited_member
         )
```

### Comparing `sphinx_autoapi-3.1b0/autoapi/_parser.py` & `sphinx_autoapi-3.1.1/autoapi/_parser.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/autoapi/directives.py` & `sphinx_autoapi-3.1.1/autoapi/directives.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/autoapi/documenters.py` & `sphinx_autoapi-3.1.1/autoapi/documenters.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/autoapi/extension.py` & `sphinx_autoapi-3.1.1/autoapi/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,18 @@
         patterns=file_patterns, dirs=normalised_dirs, ignore=ignore_patterns
     ):
         sphinx_mapper_obj.map(options=app.config.autoapi_options)
 
         if app.config.autoapi_generate_api_docs:
             sphinx_mapper_obj.output_rst(source_suffix=out_suffix)
 
+    # This function cannot be pickled into the Sphinx cache, so clear it.
+    # We won't need access to it again until a full rebuild is done anyway.
+    app.config.autoapi_prepare_jinja_env = None
+
 
 def build_finished(app, exception):
     if not app.config.autoapi_keep_files and app.config.autoapi_generate_api_docs:
         normalized_root = os.path.normpath(
             os.path.join(app.srcdir, app.config.autoapi_root)
         )
         if app.verbosity > 1:
```

### Comparing `sphinx_autoapi-3.1b0/autoapi/inheritance_diagrams.py` & `sphinx_autoapi-3.1.1/autoapi/inheritance_diagrams.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/autoapi/templates/python/class.rst` & `sphinx_autoapi-3.1.1/autoapi/templates/python/class.rst`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/autoapi/templates/python/data.rst` & `sphinx_autoapi-3.1.1/autoapi/templates/python/data.rst`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/autoapi/templates/python/function.rst` & `sphinx_autoapi-3.1.1/autoapi/templates/python/function.rst`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/autoapi/templates/python/method.rst` & `sphinx_autoapi-3.1.1/autoapi/templates/python/method.rst`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/autoapi/templates/python/module.rst` & `sphinx_autoapi-3.1.1/autoapi/templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/setup.cfg` & `sphinx_autoapi-3.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/PKG-INFO` & `sphinx_autoapi-3.1.1/sphinx_autoapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-autoapi
-Version: 3.1.0b0
+Version: 3.1.1
 Summary: Sphinx API documentation generator
 Home-page: http://github.com/readthedocs/sphinx-autoapi
 Author: Eric Holscher
 Author-email: eric@ericholscher.com
 Maintainer: Ashley Whetter
 Maintainer-email: ashley@awhetter.co.uk
 License: MIT
```

### Comparing `sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/SOURCES.txt` & `sphinx_autoapi-3.1.1/sphinx_autoapi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -99,14 +99,18 @@
 tests/python/pypackagecomplex/complex/wildchain/__init__.py
 tests/python/pypackagecomplex/complex/wildwildchain/__init__.py
 tests/python/pypackageexample/conf.py
 tests/python/pypackageexample/index.rst
 tests/python/pypackageexample/package/__init__.py
 tests/python/pypackageexample/package/_private_submodule.py
 tests/python/pypackageexample/package/submodule.py
+tests/python/pypackageexample/package/_private_subpackage/__init__.py
+tests/python/pypackageexample/package/_private_subpackage/submodule.py
+tests/python/pypackageexample/package/_private_subpackage/subpackage/__init__.py
+tests/python/pypackageexample/package/_private_subpackage/subpackage/submodule.py
 tests/python/pypackageexample/package/subpackage/__init__.py
 tests/python/pypackageexample/package/subpackage/submodule.py
 tests/python/pyskipexample/conf.py
 tests/python/pyskipexample/index.rst
 tests/python/pyskipexample/example/example.py
 tests/templateexample/conf.py
 tests/templateexample/index.rst
```

### Comparing `sphinx_autoapi-3.1b0/tests/python/conftest.py` & `sphinx_autoapi-3.1.1/tests/python/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pep695/conf.py` & `sphinx_autoapi-3.1.1/tests/python/pep695/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/py310unionpipe/conf.py` & `sphinx_autoapi-3.1.1/tests/python/py310unionpipe/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/py38positionalparams/example/example.py` & `sphinx_autoapi-3.1.1/tests/python/py38positionalparams/example/example.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/py3example/conf.py` & `sphinx_autoapi-3.1.1/tests/python/py3example/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/py3example/example/example.py` & `sphinx_autoapi-3.1.1/tests/python/py3example/example/example.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/conf.py` & `sphinx_autoapi-3.1.1/tests/python/py3implicitnamespace/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pyannotationcommentsexample/example/example.py` & `sphinx_autoapi-3.1.1/tests/python/pyannotationcommentsexample/example/example.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/conf.py` & `sphinx_autoapi-3.1.1/tests/python/pyautodoc_typehints/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pyemptyexample/conf.py` & `sphinx_autoapi-3.1.1/tests/python/pyemptyexample/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pyexample/conf.py` & `sphinx_autoapi-3.1.1/tests/python/pyexample/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pyexample/example/example.py` & `sphinx_autoapi-3.1.1/tests/python/pyexample/example/example.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pyiexample/example/example.pyi` & `sphinx_autoapi-3.1.1/tests/python/pyiexample/example/example.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/confpy/conf.py` & `sphinx_autoapi-3.1.1/tests/python/pymovedconfpy/confpy/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/example/example.py` & `sphinx_autoapi-3.1.1/tests/python/pymovedconfpy/example/example.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/foo.py` & `sphinx_autoapi-3.1.1/tests/python/pypackagecomplex/complex/foo.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/__init__.py` & `sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/submodule.py` & `sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/submodule.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/subpackage/submodule.py` & `sphinx_autoapi-3.1.1/tests/python/pypackageexample/package/_private_subpackage/submodule.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/pyskipexample/conf.py` & `sphinx_autoapi-3.1.1/tests/python/pyskipexample/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/test_own_page_option.py` & `sphinx_autoapi-3.1.1/tests/python/test_own_page_option.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/test_parser.py` & `sphinx_autoapi-3.1.1/tests/python/test_parser.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/python/test_pyintegration.py` & `sphinx_autoapi-3.1.1/tests/python/test_pyintegration.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/templateexample/conf.py` & `sphinx_autoapi-3.1.1/tests/templateexample/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/test_astroid_utils.py` & `sphinx_autoapi-3.1.1/tests/test_astroid_utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_autoapi-3.1b0/tests/test_integration.py` & `sphinx_autoapi-3.1.1/tests/test_integration.py`

 * *Files identical despite different names*

