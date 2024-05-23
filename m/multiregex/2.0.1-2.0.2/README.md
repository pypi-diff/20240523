# Comparing `tmp/multiregex-2.0.1.tar.gz` & `tmp/multiregex-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiregex-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "multiregex-2.0.2.tar", last modified: Thu May 23 16:12:15 2024, max compression
```

## Comparing `multiregex-2.0.1.tar` & `multiregex-2.0.2.tar`

### file list

```diff
@@ -1,28 +1,47 @@
--rw-r--r--   0        0        0      340 2023-05-19 20:49:42.665965 multiregex-2.0.1/.flake8
--rw-r--r--   0        0        0       87 2023-05-19 20:49:42.666037 multiregex-2.0.1/.gitattributes
--rw-r--r--   0        0        0       13 2023-05-19 20:49:42.666152 multiregex-2.0.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      204 2023-05-19 20:49:42.666236 multiregex-2.0.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      154 2023-05-19 20:49:42.666306 multiregex-2.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1405 2023-05-19 20:49:42.666427 multiregex-2.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      814 2023-06-11 16:55:47.232106 multiregex-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      802 2023-06-11 17:25:41.840034 multiregex-2.0.1/CHANGELOG.rst
--rw-r--r--   0        0        0     1456 2023-05-19 20:49:42.666735 multiregex-2.0.1/LICENSE
--rw-r--r--   0        0        0     3977 2023-05-19 20:49:42.666825 multiregex-2.0.1/README.md
--rw-r--r--   0        0        0      634 2023-05-19 20:49:42.666943 multiregex-2.0.1/docs/Makefile
--rw-r--r--   0        0        0      341 2023-05-19 20:49:42.667012 multiregex-2.0.1/docs/changelog.rst
--rw-r--r--   0        0        0     3001 2023-05-19 20:49:42.667091 multiregex-2.0.1/docs/conf.py
--rw-r--r--   0        0        0      257 2023-05-19 20:49:42.667148 multiregex-2.0.1/docs/index.rst
--rw-r--r--   0        0        0      793 2023-05-19 20:49:42.667240 multiregex-2.0.1/docs/make.bat
--rw-r--r--   0        0        0      328 2023-05-19 20:49:42.667307 multiregex-2.0.1/environment.yml
--rw-r--r--   0        0        0     1329 2023-05-19 20:49:42.667396 multiregex-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      792 2023-05-19 20:49:42.667473 multiregex-2.0.1/setup.cfg
--rw-r--r--   0        0        0       38 2023-05-19 20:49:42.667531 multiregex-2.0.1/setup.py
--rw-r--r--   0        0        0      257 2023-05-19 20:49:42.667626 multiregex-2.0.1/src/ahocorasick.pyi
--rw-r--r--   0        0        0    12552 2023-06-11 17:25:50.232318 multiregex-2.0.1/src/multiregex/__init__.py
--rw-r--r--   0        0        0      274 2023-05-19 20:49:42.667880 multiregex-2.0.1/test_utils/__init__.py
--rw-r--r--   0        0        0    26689 2023-05-19 20:49:42.668028 multiregex-2.0.1/test_utils/cpython_test_re.py
--rw-r--r--   0        0        0      147 2023-05-19 20:49:42.668128 multiregex-2.0.1/tests/conftest.py
--rw-r--r--   0        0        0     2068 2023-05-19 20:49:42.668194 multiregex-2.0.1/tests/test_bench.py
--rw-r--r--   0        0        0     1700 2023-05-19 20:49:42.668274 multiregex-2.0.1/tests/test_cpython_tests.py
--rw-r--r--   0        0        0     2746 2023-06-11 17:25:41.840429 multiregex-2.0.1/tests/test_multiregex.py
--rw-r--r--   0        0        0     4685 1970-01-01 00:00:00.000000 multiregex-2.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.212339 multiregex-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-23 16:12:09.000000 multiregex-2.0.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/ISSUE_TEMPLATE/issue-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-23 16:12:09.000000 multiregex-2.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-23 16:12:09.000000 multiregex-2.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-23 16:12:09.000000 multiregex-2.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-23 16:12:09.000000 multiregex-2.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-23 16:12:09.000000 multiregex-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-23 16:12:15.212339 multiregex-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-23 16:12:09.000000 multiregex-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-23 16:12:09.000000 multiregex-2.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-23 16:12:09.000000 multiregex-2.0.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-23 16:12:09.000000 multiregex-2.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-23 16:12:09.000000 multiregex-2.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-23 16:12:09.000000 multiregex-2.0.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/multiregex/
+-rw-r--r--   0 runner    (1001) docker     (127)    12776 2024-05-23 16:12:09.000000 multiregex-2.0.2/multiregex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:09.000000 multiregex-2.0.2/multiregex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/multiregex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-23 16:12:15.000000 multiregex-2.0.2/multiregex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-23 16:12:15.000000 multiregex-2.0.2/multiregex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:12:15.000000 multiregex-2.0.2/multiregex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 16:12:15.000000 multiregex-2.0.2/multiregex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 16:12:15.000000 multiregex-2.0.2/multiregex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171516 2024-05-23 16:12:09.000000 multiregex-2.0.2/pixi.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-23 16:12:09.000000 multiregex-2.0.2/pixi.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-23 16:12:09.000000 multiregex-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 16:12:15.212339 multiregex-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-23 16:12:09.000000 multiregex-2.0.2/stubs/ahocorasick.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-23 16:12:09.000000 multiregex-2.0.2/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26689 2024-05-23 16:12:09.000000 multiregex-2.0.2/test_utils/cpython_test_re.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:12:15.208339 multiregex-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-23 16:12:09.000000 multiregex-2.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-23 16:12:09.000000 multiregex-2.0.2/tests/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-23 16:12:09.000000 multiregex-2.0.2/tests/test_cpython_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-23 16:12:09.000000 multiregex-2.0.2/tests/test_multiregex.py
```

### Comparing `multiregex-2.0.1/LICENSE` & `multiregex-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.1/README.md` & `multiregex-2.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,32 +4,31 @@
 [![Documentation](https://img.shields.io/badge/docs-latest-success?style=plastic)](https://docs.dev.quantco.cloud/qc-github-artifacts/Quantco/multiregex/latest/index.html)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/multiregex?logoColor=white&logo=conda-forge)](https://anaconda.org/conda-forge/multiregex)
 [![pypi-version](https://img.shields.io/pypi/v/multiregex.svg?logo=pypi&logoColor=white)](https://pypi.org/project/multiregex)
 [![python-version](https://img.shields.io/pypi/pyversions/multiregex?logoColor=white&logo=python)](https://pypi.org/project/multiregex)
 
 Quickly match many regexes against a string. Provides 2-10x speedups over naïve regex matching.
 
+## Introduction
+
+See [this introductory blog post](https://tech.quantco.com/2022/07/31/multiregex.html).
+
 ## Installation
 
 You can install the package in development mode using:
 
 ```bash
-git clone git@github.com:quantco/multiregex.git
+git clone https://github.com/quantco/multiregex
 cd multiregex
 
-# create and activate a fresh environment named multiregex
-# see environment.yml for details
-mamba env create
-conda activate multiregex
-
-pre-commit install
-pip install --no-build-isolation -e .
+pixi run pre-commit-install
+pixi run postinstall
+pixi run test
 ```
 
-
 ## Usage
 
 ```py
 import multiregex
 
 # Create matcher from multiple regexes.
 my_patterns = [r"\w+@\w+\.com", r"\w\.com"]
@@ -50,15 +49,15 @@
 ### Custom prematchers
 
 To be able to quickly match many regexes against a string, `multiregex` uses
 "prematchers" under the hood. Prematchers are lists of non-regex strings of which
 at least one can be assumed to be present in the haystack if the corresponding regex matches.
 As an example, a valid prematcher of `r"\w+\.com"` could be `[".com"]` and a valid
 prematcher of `r"(B|b)aNäNa"` could be `["b"]` or `["anäna"]`.
-Note that prematchers must be all-lowercase (in order for ``multiregex`` to be able to support ``re.IGNORECASE``).
+Note that prematchers must be all-lowercase (in order for `multiregex` to be able to support `re.IGNORECASE`).
 
 You will likely have to provide your own prematchers for all but the simplest
 regex patterns:
 
 ```py
 multiregex.RegexMatcher([r"\d+"])
 # => ValueError: Could not generate prematcher : '\\d+'
```

### Comparing `multiregex-2.0.1/docs/Makefile` & `multiregex-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.1/docs/conf.py` & `multiregex-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.1/docs/make.bat` & `multiregex-2.0.2/docs/make.bat`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 %SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 goto end
 
 :help
 %SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 
 :end
-popd
+popd
```

### Comparing `multiregex-2.0.1/src/multiregex/__init__.py` & `multiregex-2.0.2/multiregex/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-r"""Speed up regex matching with non-regex substring "prematchers", similar to Bloom filters.
+r"""Speed up regex matching with non-regex substring "prematchers", similar to
+Bloom filters.
 
 For each regex pattern we use a list of simple (non-regex) substring prematchers.
 When evaluating regex patterns on a string, we use the prematchers to restrict
 the set of regex patterns to be run. Hence, the prematchers _must_ match each string
 unless it's impossible for the corresponding regex to match, similar to Bloom filters.
 
 Examples:
@@ -15,15 +16,17 @@
 `RegexMatcher.generate_prematchers`.  You must provide a handcrafted list of
 prematchers for regexes that this fails for.  You may also override the
 automatically generated prematchers.
 """
 
 import collections
 import functools
+import importlib
 import re
+import warnings
 
 try:
     sre_constants = re._constants  # type: ignore
     sre_parse = re._parser  # type: ignore
 except AttributeError:
     import sre_constants
     import sre_parse
@@ -38,15 +41,20 @@
     TypeVar,
     Union,
     cast,
 )
 
 import ahocorasick
 
-__version__ = "2.0.1"
+try:
+    __version__ = importlib.metadata.version(__name__)
+except importlib.metadata.PackageNotFoundError as e:
+    warnings.warn(f"Could not determine version of {__name__}", stacklevel=1)
+    warnings.warn(str(e), stacklevel=1)
+    __version__ = "unknown"
 
 
 V = TypeVar("V")
 PatternOrStr = Union[Pattern, str]
 Prematchers = Set[str]
 FalsePositivesCounter = Dict[str, int]
 
@@ -106,17 +114,15 @@
     @staticmethod
     def _normalize_patterns(patterns):
         """Normalize `patterns` param given to `__init__`."""
 
         def safe_set(iterable):
             if isinstance(iterable, str):
                 raise TypeError(
-                    "Refusing to interpret {!r} as a list of patterns, pass a list of strings instead".format(
-                        iterable
-                    )
+                    f"Refusing to interpret {iterable!r} as a list of patterns, pass a list of strings instead"
                 )
             else:
                 return set(iterable)
 
         patterns = list(patterns)
         if patterns and not isinstance(patterns[0], tuple):
             return [(re.compile(pattern), None) for pattern in patterns]
@@ -129,17 +135,19 @@
                 for pattern, prematchers in patterns
             ]
 
     def _generate_missing_prematchers(self, patterns):
         patterns = [
             (
                 pattern,
-                self.generate_prematchers(pattern)
-                if prematchers is None
-                else prematchers,
+                (
+                    self.generate_prematchers(pattern)
+                    if prematchers is None
+                    else prematchers
+                ),
             )
             for pattern, prematchers in patterns
         ]
         for _, prematchers in patterns:
             for prematcher in prematchers:
                 validate_prematcher(prematcher)
         return patterns
@@ -189,18 +197,16 @@
                 if match is None:
                     self.prematcher_false_positives[pattern]["false_positives"] += 1
 
         return [(pattern, match) for pattern, match in re_results if match is not None]
 
     """Alias for ``run(re.search, ...)``."""
     search = functools.partialmethod(run, re.search)
-
     """Alias for ``run(re.match, ...)``."""
     match = functools.partialmethod(run, re.match)
-
     """Alias for ``run(re.fullmatch, ...)``."""
     fullmatch = functools.partialmethod(run, re.fullmatch)
 
     def get_pattern_candidates(self, s: str) -> List[Pattern]:
         """Get a list of patterns that potentially match `s`.
 
         Pattern order is the same the order of `patterns` given to `__init__`.
@@ -247,26 +253,25 @@
             output.append("(No data)")
         return "\n".join(output)
 
 
 def validate_prematcher(prematcher: str) -> None:
     if not prematcher or any(map(str.isupper, prematcher)):
         raise ValueError(
-            "Prematcher {!r} must be non-empty, all-lowercase, all-ASCII".format(
-                prematcher
-            )
+            f"Prematcher {prematcher!r} must be non-empty, all-lowercase, all-ASCII"
         )
 
 
 def generate_prematchers(pattern: Pattern) -> Prematchers:
     """Generate fallback/default prematchers for the given regex `pattern`.
 
-    Currently the fallback prematcher is just the set of longest terminal texts
-    in the pattern, eg. "Fast(er)? regex(es| matching)" -> {" regex"}. One level of
-    branches with the "|" character is supported, ie. "(a|bb|ccc)" -> {"ccc", "a", "bb"}.
+    Currently the fallback prematcher is just the set of longest
+    terminal texts in the pattern, eg. "Fast(er)? regex(es| matching)"
+    -> {" regex"}. One level of branches with the "|" character is
+    supported, ie. "(a|bb|ccc)" -> {"ccc", "a", "bb"}.
     """
 
     def _get_top_level_prematcher(sre_ast):
         return max(_sre_find_terminals(sre_ast), key=len, default="").lower()
 
     sre_ast = _simplify_sre_ast(sre_parse.parse(pattern.pattern))
 
@@ -282,15 +287,15 @@
     )
     for children in sre_branches:
         simplified_children = map(_simplify_sre_ast, children)
         child_prematchers = set(map(_get_top_level_prematcher, simplified_children))
         if all(child_prematchers):
             return child_prematchers
 
-    raise ValueError("Could not generate prematchers for {!r}".format(pattern.pattern))
+    raise ValueError(f"Could not generate prematchers for {pattern.pattern!r}")
 
 
 def _simplify_sre_ast(sre_ast):
     """Simplify an sre AST.
 
     - Transform pattern r"(...)" to r"...".
     """
@@ -314,19 +319,20 @@
             chars.append(cast(int, sre_ast[i][1]))
             i += 1
         yield "".join(map(chr, chars))
         i += 1
 
 
 def _ahocorasick_make_automaton(words: Dict[str, V]) -> "ahocorasick.Automaton[V]":
-    """Make an ahocorasick automaton from a dictionary of `needle -> value` items."""
+    """Make an ahocorasick automaton from a dictionary of `needle -> value`
+    items."""
     automaton = ahocorasick.Automaton()  # type: ahocorasick.Automaton[V]
     for word, value in words.items():
         _ahocorasick_ensure_successful(automaton.add_word(word, value))
     _ahocorasick_ensure_successful(automaton.make_automaton())
     return automaton
 
 
 def _ahocorasick_ensure_successful(res):
-    """pyahocorasick returns errors as bools."""
+    """Pyahocorasick returns errors as bools."""
     if res is False:
         raise AhocorasickError("Error performing ahocorasick call")
```

### Comparing `multiregex-2.0.1/test_utils/cpython_test_re.py` & `multiregex-2.0.2/test_utils/cpython_test_re.py`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.1/tests/test_bench.py` & `multiregex-2.0.2/tests/test_bench.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     assert re.match(python_parser["forloop"], "for (_, (x, y)), in spam():")
     assert re.match(python_parser["decorator"], "@foo(x=1)")
     assert re.match(python_parser["import_statement"], "import x")
     assert re.match(python_parser["import_statement"], "from x import y as z")
 
 
 def test_parse_myself():
-    myself = Path(__file__).parents[1] / "src" / "multiregex" / "__init__.py"
+    myself = Path(__file__).parents[1] / "multiregex" / "__init__.py"
     with myself.open() as f:
         myself_src = f.read().splitlines()
     slow_matcher = make_slow_matcher(python_parser.values())
     fast_matcher = RegexMatcher(python_parser.values())
     slow_results = map(slow_matcher, myself_src)
     fast_results = map(fast_matcher.search, myself_src)
     for slow_result, fast_result in zip(slow_results, fast_results):
```

### Comparing `multiregex-2.0.1/tests/test_cpython_tests.py` & `multiregex-2.0.2/tests/test_cpython_tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     from typing import Any  # noqa
 
     vardict = {
         "found": match.group(0),
         "groups": match.group(),
         "flags": match.re.flags,
     }
-    numbered_groups = [("g{}".format(i), i) for i in range(100)]  # type: Any
+    numbered_groups = [(f"g{i}", i) for i in range(100)]  # type: Any
     named_groups = [(g, g) for g in match.re.groupindex]  # type: Any
     for name, key in numbered_groups + named_groups:
         try:
             val = str(match.group(key))
         except IndexError:
             val = "Error"
         vardict[name] = val
```

### Comparing `multiregex-2.0.1/tests/test_multiregex.py` & `multiregex-2.0.2/tests/test_multiregex.py`

 * *Files identical despite different names*

### Comparing `multiregex-2.0.1/PKG-INFO` & `multiregex-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 Metadata-Version: 2.1
 Name: multiregex
-Version: 2.0.1
-Summary: Speed up regex matching with non-regex substring "prematchers", similar to Bloom filters.
-Author-email: "QuantCo, Inc." <noreply@quantco.com>
-Maintainer-email: Jonas Haag <jonas.haag@quantco.com>
-Description-Content-Type: text/markdown
+Version: 2.0.2
+Summary: Quickly match many regexes against a string. Provides 2-10x speedups over naïve regex matching.
+Author-email: "QuantCo, Inc." <noreply@quantco.com>, Jonas Haag <jonas@lophus.org>
+Maintainer-email: Bela Stoyan <bela.stoyan@quantco.com>
+Project-URL: Home, https://github.com/quantco/multiregex
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Project-URL: Home, https://github.com/quantco/multiregex
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyahocorasick
 
 # multiregex
 
 [![CI](https://github.com/Quantco/multiregex/actions/workflows/ci.yml/badge.svg)](https://github.com/Quantco/multiregex/actions/workflows/ci.yml)
 [![Documentation](https://img.shields.io/badge/docs-latest-success?style=plastic)](https://docs.dev.quantco.cloud/qc-github-artifacts/Quantco/multiregex/latest/index.html)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/multiregex?logoColor=white&logo=conda-forge)](https://anaconda.org/conda-forge/multiregex)
 [![pypi-version](https://img.shields.io/pypi/v/multiregex.svg?logo=pypi&logoColor=white)](https://pypi.org/project/multiregex)
 [![python-version](https://img.shields.io/pypi/pyversions/multiregex?logoColor=white&logo=python)](https://pypi.org/project/multiregex)
 
 Quickly match many regexes against a string. Provides 2-10x speedups over naïve regex matching.
 
+## Introduction
+
+See [this introductory blog post](https://tech.quantco.com/2022/07/31/multiregex.html).
+
 ## Installation
 
 You can install the package in development mode using:
 
 ```bash
-git clone git@github.com:quantco/multiregex.git
+git clone https://github.com/quantco/multiregex
 cd multiregex
 
-# create and activate a fresh environment named multiregex
-# see environment.yml for details
-mamba env create
-conda activate multiregex
-
-pre-commit install
-pip install --no-build-isolation -e .
+pixi run pre-commit-install
+pixi run postinstall
+pixi run test
 ```
 
-
 ## Usage
 
 ```py
 import multiregex
 
 # Create matcher from multiple regexes.
 my_patterns = [r"\w+@\w+\.com", r"\w\.com"]
@@ -66,15 +67,15 @@
 ### Custom prematchers
 
 To be able to quickly match many regexes against a string, `multiregex` uses
 "prematchers" under the hood. Prematchers are lists of non-regex strings of which
 at least one can be assumed to be present in the haystack if the corresponding regex matches.
 As an example, a valid prematcher of `r"\w+\.com"` could be `[".com"]` and a valid
 prematcher of `r"(B|b)aNäNa"` could be `["b"]` or `["anäna"]`.
-Note that prematchers must be all-lowercase (in order for ``multiregex`` to be able to support ``re.IGNORECASE``).
+Note that prematchers must be all-lowercase (in order for `multiregex` to be able to support `re.IGNORECASE`).
 
 You will likely have to provide your own prematchers for all but the simplest
 regex patterns:
 
 ```py
 multiregex.RegexMatcher([r"\d+"])
 # => ValueError: Could not generate prematcher : '\\d+'
@@ -118,8 +119,7 @@
 # FP count | FP rate | Pattern / Prematchers
 # ---------+---------+----------------------
 #      137 |    0.72 | (19|20)\d\d-\d\d-\d\d / {'-'}
 ```
 
 In this example, there were 137 input strings that were matched positive by the prematcher but negative by the regex.
 In other words, the prematcher failed to prevent slow regex evaluation in 72% of the cases.
-
```

