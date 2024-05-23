# Comparing `tmp/kaquel-0.1.tar.gz` & `tmp/kaquel-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaquel-0.1.tar", max compression
+gzip compressed data, was "kaquel-0.2.tar", max compression
```

## Comparing `kaquel-0.1.tar` & `kaquel-0.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0    21863 2024-05-17 22:53:04.474328 kaquel-0.1/LICENSE.txt
--rw-r--r--   0        0        0      548 2024-05-17 22:53:04.474328 kaquel-0.1/README.rst
--rw-r--r--   0        0        0     1771 2024-05-17 22:53:04.477328 kaquel-0.1/kaquel/__init__.py
--rw-r--r--   0        0        0     2674 2024-05-17 22:53:04.477328 kaquel-0.1/kaquel/errors.py
--rw-r--r--   0        0        0    18780 2024-05-17 22:53:04.477328 kaquel-0.1/kaquel/kql.py
--rw-r--r--   0        0        0        0 2024-05-17 22:53:04.509328 kaquel-0.1/kaquel/py.typed
--rw-r--r--   0        0        0    11139 2024-05-17 22:53:04.477328 kaquel-0.1/kaquel/query.py
--rw-r--r--   0        0        0     2482 2024-05-17 22:53:04.477328 kaquel-0.1/kaquel/utils.py
--rw-r--r--   0        0        0     2904 2024-05-17 22:53:04.478328 kaquel-0.1/pyproject.toml
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 kaquel-0.1/PKG-INFO
+-rw-r--r--   0        0        0    21863 2024-05-23 19:37:57.637723 kaquel-0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1184 2024-05-23 19:37:57.637723 kaquel-0.2/README.rst
+-rw-r--r--   0        0        0     1771 2024-05-23 19:37:57.639723 kaquel-0.2/kaquel/__init__.py
+-rw-r--r--   0        0        0     2675 2024-05-23 19:37:57.640723 kaquel-0.2/kaquel/errors.py
+-rw-r--r--   0        0        0     5806 2024-05-23 19:37:57.640723 kaquel-0.2/kaquel/es_query.py
+-rw-r--r--   0        0        0    22254 2024-05-23 19:37:57.640723 kaquel-0.2/kaquel/kql.py
+-rw-r--r--   0        0        0     2323 2024-05-23 19:37:57.640723 kaquel-0.2/kaquel/lucene.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:37:57.674723 kaquel-0.2/kaquel/py.typed
+-rw-r--r--   0        0        0    12480 2024-05-23 19:37:57.640723 kaquel-0.2/kaquel/query.py
+-rw-r--r--   0        0        0     2482 2024-05-23 19:37:57.640723 kaquel-0.2/kaquel/utils.py
+-rw-r--r--   0        0        0     3115 2024-05-23 19:37:57.641723 kaquel-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 kaquel-0.2/PKG-INFO
```

### Comparing `kaquel-0.1/LICENSE.txt` & `kaquel-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kaquel-0.1/kaquel/__init__.py` & `kaquel-0.2/kaquel/__init__.py`

 * *Files identical despite different names*

### Comparing `kaquel-0.1/kaquel/errors.py` & `kaquel-0.2/kaquel/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # knowledge of the CeCILL-C license and that you accept its terms.
 # *****************************************************************************
 """Error definitions for Kaquel."""
 
 from __future__ import annotations
 
 
-class Error(Exception):
+class Error(ValueError):
     """An error has occurred in a Kaquel function."""
 
     def __init__(self, message: str, /) -> None:
         super().__init__(message)
 
 
 class DecodeError(Error):
```

### Comparing `kaquel-0.1/kaquel/kql.py` & `kaquel-0.2/kaquel/kql.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,40 +22,46 @@
 # software's suitability as regards their requirements in conditions enabling
 # the security of their systems and/or data to be ensured and, more generally,
 # to use and operate it in the same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL-C license and that you accept its terms.
 # *****************************************************************************
-"""Kuery lexer."""
+"""KQL lexer and parser."""
 
 from __future__ import annotations
 
 from collections.abc import Iterator
 from enum import Enum, auto
+from itertools import chain
 import re
+from typing import Literal, Union
 
 from pydantic import BaseModel
 
 from kaquel.errors import DecodeError, LeadingWildcardsForbidden
 from kaquel.query import (
     BooleanQuery,
     ExistsQuery,
+    MatchAllQuery,
     MatchPhraseQuery,
     MatchQuery,
     MultiMatchQuery,
     MultiMatchQueryType,
     NestedQuery,
     NestedScoreMode,
     Query,
     RangeQuery,
 )
 from kaquel.utils import Runk
 
 
+__all__ = ["parse_kql"]
+
+
 _KQL_TOKEN_PATTERN = re.compile(
     r"(>=?|<=?|:|\(|\)|{|})"
     + r'|"((?:.*?[^\\](?:\\\\)*|))"'  # Quoted literal.
     + '|((?:[^\\\\:()<>"\\s]|\\\\.)+)',  # Unquoted literal.
     re.MULTILINE,
 )
 """Pattern for reading the next token."""
@@ -82,15 +88,32 @@
     RBRACE = auto()
 
     OR = auto()
     AND = auto()
     NOT = auto()
 
 
-_KQL_TOKEN_MAPPING: dict[str, KQLTokenType] = {
+_KQL_TOKEN_MAPPING: dict[
+    str,
+    Literal[
+        KQLTokenType.END,
+        KQLTokenType.LTE,
+        KQLTokenType.GTE,
+        KQLTokenType.LT,
+        KQLTokenType.GT,
+        KQLTokenType.COLON,
+        KQLTokenType.LPAR,
+        KQLTokenType.RPAR,
+        KQLTokenType.LBRACE,
+        KQLTokenType.RBRACE,
+        KQLTokenType.OR,
+        KQLTokenType.AND,
+        KQLTokenType.NOT,
+    ],
+] = {
     "<=": KQLTokenType.LTE,
     ">=": KQLTokenType.GTE,
     "<": KQLTokenType.LT,
     ">": KQLTokenType.GT,
     ":": KQLTokenType.COLON,
     "(": KQLTokenType.LPAR,
     ")": KQLTokenType.RPAR,
@@ -99,33 +122,69 @@
     "or": KQLTokenType.OR,
     "and": KQLTokenType.AND,
     "not": KQLTokenType.NOT,
 }
 """Direct token mapping."""
 
 
-class KQLToken(BaseModel):
+class KQLBasicToken(BaseModel):
+    """Basic token, as emitted by the lexer."""
+
+    type: Literal[
+        KQLTokenType.END,
+        KQLTokenType.LTE,
+        KQLTokenType.GTE,
+        KQLTokenType.LT,
+        KQLTokenType.GT,
+        KQLTokenType.COLON,
+        KQLTokenType.LPAR,
+        KQLTokenType.RPAR,
+        KQLTokenType.LBRACE,
+        KQLTokenType.RBRACE,
+        KQLTokenType.OR,
+        KQLTokenType.AND,
+        KQLTokenType.NOT,
+    ]
+    """Type of the token."""
+
+    line: int
+    """Line at which the token starts, counting from 1."""
+
+    column: int
+    """Column at which the token starts, counting from 1."""
+
+    offset: int
+    """Offset at which the token starts, counting from 0."""
+
+
+class KQLValueToken(BaseModel):
     """Token, as emitted by the lexer."""
 
-    type: KQLTokenType
+    type: Literal[
+        KQLTokenType.UNQUOTED_LITERAL,
+        KQLTokenType.QUOTED_LITERAL,
+    ]
     """Type of the token."""
 
-    value: str | None = None
+    value: str
     """Contents of the token, if relevant."""
 
     line: int
     """Line at which the token starts, counting from 1."""
 
     column: int
     """Column at which the token starts, counting from 1."""
 
     offset: int
     """Offset at which the token starts, counting from 0."""
 
 
+KQLToken = Union[KQLBasicToken, KQLValueToken]
+
+
 # ---
 # Lexer.
 # ---
 
 
 def _unescape_kql_literal(escaped_literal: str, /) -> str:
     """Unescape a KQL literal.
@@ -164,43 +223,53 @@
                 f"Could not parsing query starting from: {kuery}",
                 line=runk.line,
                 column=runk.column,
                 offset=runk.offset,
             )
 
         if match[1] is not None:
-            typ, value = _KQL_TOKEN_MAPPING[match[1]], None
+            yield KQLBasicToken(
+                type=_KQL_TOKEN_MAPPING[match[1]],
+                line=runk.line,
+                column=runk.column,
+                offset=runk.offset,
+            )
         elif match[2] is not None:
-            typ, value = (
-                KQLTokenType.QUOTED_LITERAL,
-                _unescape_kql_literal(match[2]),
+            yield KQLValueToken(
+                type=KQLTokenType.QUOTED_LITERAL,
+                value=_unescape_kql_literal(match[2]),
+                line=runk.line,
+                column=runk.column,
+                offset=runk.offset,
             )
         elif match[3] is not None:
             try:
-                typ, value = _KQL_TOKEN_MAPPING[match[3].casefold()], None
+                typ = _KQL_TOKEN_MAPPING[match[3].casefold()]
             except KeyError:
-                typ, value = (
-                    KQLTokenType.UNQUOTED_LITERAL,
-                    _unescape_kql_literal(match[3]),
+                yield KQLValueToken(
+                    type=KQLTokenType.UNQUOTED_LITERAL,
+                    value=_unescape_kql_literal(match[3]),
+                    line=runk.line,
+                    column=runk.column,
+                    offset=runk.offset,
+                )
+            else:
+                yield KQLBasicToken(
+                    type=typ,
+                    line=runk.line,
+                    column=runk.column,
+                    offset=runk.offset,
                 )
         else:  # pragma: no cover
             raise NotImplementedError()
 
-        yield KQLToken(
-            type=typ,
-            value=value,
-            line=runk.line,
-            column=runk.column,
-            offset=runk.offset,
-        )
-
         runk.count(match[0])
         kuery = kuery[match.end() :]
 
-    yield KQLToken(
+    yield KQLBasicToken(
         type=KQLTokenType.END,
         line=runk.line,
         column=runk.column,
         offset=runk.offset,
     )
 
 
@@ -211,14 +280,17 @@
 
 class _KQLParsingOptions(BaseModel):
     """Options for the KQL parser."""
 
     allow_leading_wildcards: bool
     """Whether to allow leading wildcards or not."""
 
+    filters_in_must_clause: bool
+    """Whether filters should be in the 'filter' or 'must' clause."""
+
 
 class UnexpectedKQLToken(DecodeError):
     """An unexpected KQL token was obtained."""
 
     token: KQLToken
     """Token type."""
 
@@ -264,49 +336,64 @@
                 field=field,
             )
             if token.type != KQLTokenType.RPAR:
                 raise UnexpectedKQLToken(token)
 
             token = next(token_iter)
         elif token.type == KQLTokenType.QUOTED_LITERAL:
-            result = MatchPhraseQuery(
-                field=field,
-                query=token.value,
-            )
+            if field == "*":
+                result = MultiMatchQuery(
+                    type=MultiMatchQueryType.PHRASE,
+                    query=token.value,
+                    lenient=True,
+                )
+            else:
+                result = MatchPhraseQuery(
+                    field=field,
+                    query=token.value,
+                )
+
             token = next(token_iter)
         elif token.type == KQLTokenType.UNQUOTED_LITERAL:
             query_parts = [token.value or ""]
 
             for token in token_iter:
                 if token.type != KQLTokenType.UNQUOTED_LITERAL:
                     break
-                if token.value is None:  # pragma: no cover
-                    raise ValueError("Unquoted literal without a value!")
 
                 query_parts.append(token.value)
 
             if not options.allow_leading_wildcards and any(
                 part.startswith("*") for part in query_parts
             ):
                 raise LeadingWildcardsForbidden()
 
-            result = MatchQuery(field=field, query=" ".join(query_parts))
+            if field == "*":
+                result = MultiMatchQuery(
+                    query=" ".join(query_parts),
+                    lenient=True,
+                )
+            else:
+                result = MatchQuery(field=field, query=" ".join(query_parts))
         else:
             raise UnexpectedKQLToken(token)
 
         if is_not:
             result = BooleanQuery(must_not=result)
 
         elements.append(result)
         if token.type != KQLTokenType.AND:
             break
 
     if len(elements) == 1:
         return elements[0], token
 
+    if options.filters_in_must_clause:
+        return BooleanQuery(must=elements), token
+
     return BooleanQuery(filter=elements), token
 
 
 def _parse_kql_or_value_list(
     token_iter: Iterator[KQLToken],
     /,
     *,
@@ -450,60 +537,77 @@
                     field=prefix + (token.value or ""),
                 )
                 if token.type != KQLTokenType.RPAR:
                     raise UnexpectedKQLToken(token)
 
                 token = next(token_iter)
             elif comp_token.type == KQLTokenType.QUOTED_LITERAL:
-                result = MatchPhraseQuery(
-                    field=prefix + (token.value or ""),
-                    query=comp_token.value,
-                )
+                if token.value == "*":
+                    # Even in a nested context, i.e. ``prefix`` being
+                    # non-empty, Kibana interprets this as the field being
+                    # a lone wildcard, so we want to do the same.
+                    result = MultiMatchQuery(
+                        type=MultiMatchQueryType.PHRASE,
+                        query=comp_token.value,
+                        lenient=True,
+                    )
+                else:
+                    result = MatchPhraseQuery(
+                        field=prefix + (token.value or ""),
+                        query=comp_token.value,
+                    )
+
                 token = next(token_iter)
             elif comp_token.type == KQLTokenType.UNQUOTED_LITERAL:
                 query_parts: list[str] = [comp_token.value or ""]
 
                 for comp_token in token_iter:
                     if comp_token.type != KQLTokenType.UNQUOTED_LITERAL:
                         break
-                    if comp_token.value is None:  # pragma: no cover
-                        raise ValueError("Unquoted literal without a value!")
 
                     query_parts.append(comp_token.value)
 
                 if not options.allow_leading_wildcards and any(
                     part.startswith("*") for part in query_parts
                 ):
                     raise LeadingWildcardsForbidden()
 
-                if "*" in query_parts:
+                if token.value == "*":
+                    # Even in a nested context, i.e. ``prefix`` being
+                    # non-empty, Kibana interprets this as the field being
+                    # a lone wildcard, so we want to do the same.
+                    if "*" in query_parts:
+                        result = MatchAllQuery()
+                    else:
+                        result = MultiMatchQuery(
+                            type=MultiMatchQueryType.BEST_FIELDS,
+                            query=" ".join(query_parts),
+                            lenient=True,
+                        )
+                elif "*" in query_parts:
                     result = ExistsQuery(field=prefix + (token.value or ""))
                 else:
                     result = MatchQuery(
                         field=prefix + (token.value or ""),
                         query=" ".join(query_parts),
                     )
 
                 token = comp_token
             else:
                 raise UnexpectedKQLToken(comp_token)
         else:
             query_parts = [token.value or ""]
 
             if op_token.type == KQLTokenType.UNQUOTED_LITERAL:
-                if op_token.value is None:  # pragma: no cover
-                    raise ValueError("Unquoted literal without a value!")
 
                 query_parts.append(op_token.value)
 
                 for op_token in token_iter:
                     if op_token.type != KQLTokenType.UNQUOTED_LITERAL:
                         break
-                    if op_token.value is None:  # pragma: no cover
-                        raise ValueError("Unquoted literal without a value!")
 
                     query_parts.append(op_token.value)
 
             if not options.allow_leading_wildcards and any(
                 part.startswith("*") for part in query_parts
             ):
                 raise LeadingWildcardsForbidden()
@@ -562,14 +666,17 @@
 
         if token.type != KQLTokenType.AND:
             break
 
     if len(elements) == 1:
         return elements[0], token
 
+    if options.filters_in_must_clause:
+        return BooleanQuery(must=elements), token
+
     return BooleanQuery(filter=elements), token
 
 
 def _parse_kql_or_query(
     token_iter: Iterator[KQLToken],
     /,
     *,
@@ -609,25 +716,39 @@
 
 
 def parse_kql(
     kuery: str,
     /,
     *,
     allow_leading_wildcards: bool = True,
+    filters_in_must_clause: bool = False,
 ) -> Query:
     """Parse a KQL expression into an ElasticSearch query.
 
     :param kuery: KQL expression to parse.
     :param allow_leading_wildcards: Whether to allow leading wildcards.
+    :param filters_in_must_clause: Whether filters should be in the
+        'filter' or 'must' clause.
+    :return: Parsed query.
     :raises DecodeError: A decoding error has occurred.
     :raises LeadingWildcardsForbidden: Leading wildcards were present while
         disabled.
     """
     options = _KQLParsingOptions(
         allow_leading_wildcards=allow_leading_wildcards,
+        filters_in_must_clause=filters_in_must_clause,
     )
     token_iter = parse_kql_tokens(kuery)
+
+    # Check for an empty query.
+    first_token = next(token_iter)
+    if first_token.type == KQLTokenType.END:
+        return MatchAllQuery()
+
+    # Requeue the first token.
+    token_iter = chain(iter((first_token,)), token_iter)
+
     result, token = _parse_kql_or_query(token_iter, options=options)
     if token.type != KQLTokenType.END:
         raise UnexpectedKQLToken(token)
 
     return result
```

### Comparing `kaquel-0.1/kaquel/query.py` & `kaquel-0.2/kaquel/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,29 +35,33 @@
     /query-dsl.html
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from datetime import date
-from enum import StrEnum
+from enum import Enum
 from typing import Annotated, Any
 
 from pydantic import (
     BaseModel,
+    ConfigDict,
     Field,
     StringConstraints,
     field_validator,
     model_validator,
 )
 
 
 class Query(BaseModel, ABC):
     """Any query."""
 
+    model_config = ConfigDict(extra="forbid")
+    """Model configuration."""
+
     @abstractmethod
     def render(self, /) -> dict:
         """Render as a Python dictionary.
 
         :return: Rendered query.
         """
 
@@ -155,14 +159,33 @@
 
         :return: Rendered query.
         :meta private:
         """
         return {"exists": {"field": self.field}}
 
 
+class MatchAllQuery(Query):
+    """Match all query.
+
+    See `Match all query`_ for more information.
+
+    .. _Match all query:
+        https://www.elastic.co/guide/en/elasticsearch/reference/current/
+        query-dsl-match-all-query.html
+    """
+
+    def render(self, /) -> dict:
+        """Render as a Python dictionary.
+
+        :return: Rendered query.
+        :meta private:
+        """
+        return {"match_all": {}}
+
+
 class MatchPhraseQuery(Query):
     """Match phrase query.
 
     See `Match phrase query`_ for more information.
 
     .. _Match phrase query:
         https://www.elastic.co/guide/en/elasticsearch/reference/current/
@@ -205,15 +228,15 @@
 
         :return: Rendered query.
         :meta private:
         """
         return {"match": {self.field: self.query}}
 
 
-class MultiMatchQueryType(StrEnum):
+class MultiMatchQueryType(str, Enum):
     """Multi-match query type.
 
     See `multi_match query types`_ for more information.
 
     .. _multi_match query types:
         https://www.elastic.co/guide/en/elasticsearch/reference/current/
         query-dsl-multi-match-query.html#multi-match-types
@@ -277,15 +300,15 @@
             result["fields"] = self.fields
         if self.lenient:
             result["lenient"] = True
 
         return {"multi_match": result}
 
 
-class NestedScoreMode(StrEnum):
+class NestedScoreMode(str, Enum):
     """Mode in which a nested query affects the root document's score."""
 
     AVG = "avg"
     """Use the mean relevance score of all matching child objects."""
 
     MAX = "max"
     """Use the highest relevance score of all matching child objects."""
@@ -330,14 +353,44 @@
             "query": self.query.render(),
             "score_mode": self.score_mode.value,
         }
 
         return {"nested": result}
 
 
+class QueryStringQuery(Query):
+    """Query string query.
+
+    See `Query string query`_ for more information.
+
+    .. _Query string query:
+        https://www.elastic.co/guide/en/elasticsearch/reference/current/
+        query-dsl-query-string-query.html
+    """
+
+    query: Annotated[str, StringConstraints(min_length=1)]
+    """Query to parse and use for search.
+
+    See `Query string syntax`_ for more information.
+
+    .. _Query string syntax:
+        https://www.elastic.co/guide/en/elasticsearch/reference/current/
+        query-dsl-query-string-query.html#query-string-syntax
+    """
+
+    def render(self, /) -> dict:
+        """Render as a Python dictionary.
+
+        :return: Rendered query.
+        :meta private:
+        """
+        result = {"query": self.query}
+        return {"query_string": result}
+
+
 class RangeQuery(Query):
     """Range query.
 
     See `Range query`_ for more information.
 
     .. _Range query:
         https://www.elastic.co/guide/en/elasticsearch/reference/current/
```

### Comparing `kaquel-0.1/kaquel/utils.py` & `kaquel-0.2/kaquel/utils.py`

 * *Files identical despite different names*

### Comparing `kaquel-0.1/pyproject.toml` & `kaquel-0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kaquel"
-version = "0.1"
+version = "0.2"
 description = "Tools for handling ElasticSearch queries in various languages"
 readme = "README.rst"
 homepage = "https://kaquel.touhey.pro/"
 repository = "https://gitlab.com/thomas.touhey/kaquel"
 authors = ["Thomas Touhey <thomas@touhey.fr>"]
+keywords = [
+    "elasticsearch",
+    "es_query",
+    "es-query",
+    "kibana",
+    "kql",
+    "lucene",
+    "parsing",
+    "query",
+]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: CeCILL-C Free Software License Agreement (CECILL-C)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Database :: Front-Ends",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
+eval-type-backport = { version = "^0.2", markers = "python_version < '3.10'" }
 pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 pytest = "^8.2.0"
 pytest-cov = "^5.0.0"
 sphinx-autobuild = "^2024.4.16"
@@ -35,15 +46,15 @@
 [tool.poetry.group.docs.dependencies]
 furo = "^2024.5.6"
 sphinx = "^7.3.7"
 sphinxcontrib-mermaid = "^0.9.2"
 toml = "^0.10.2"
 
 [tool.black]
-target_version = ['py311']
+target_version = ['py39']
 line-length = 79
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
 update_changelog_on_bump = true
 version = "0.1.4"
@@ -99,15 +110,15 @@
 group_by_package = true
 include_trailing_comma = true
 line_length = 79
 lines_after_imports = 2
 multi_line_output = 3
 no_inline_sort = true
 profile = "black"
-py_version = 311
+py_version = 39
 use_parentheses = true
 combine_as_imports = true
 
 [tool.mypy]
 ignore_missing_imports = true
 mypy_path = "."
 warn_unused_ignores = true
```

### Comparing `kaquel-0.1/PKG-INFO` & `kaquel-0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,58 @@
 Metadata-Version: 2.1
 Name: kaquel
-Version: 0.1
+Version: 0.2
 Summary: Tools for handling ElasticSearch queries in various languages
 Home-page: https://kaquel.touhey.pro/
+Keywords: elasticsearch,es_query,es-query,kibana,kql,lucene,parsing,query
 Author: Thomas Touhey
 Author-email: thomas@touhey.fr
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: CeCILL-C Free Software License Agreement (CECILL-C)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Typing :: Typed
+Requires-Dist: eval-type-backport (>=0.2,<0.3) ; python_version < "3.10"
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Project-URL: Repository, https://gitlab.com/thomas.touhey/kaquel
 Description-Content-Type: text/x-rst
 
 ``kaquel`` -- Tools for handling ElasticSearch queries in various languages
 ===========================================================================
 
 Kaquel, pronounced */kækyɛl/*, is a toolset for parsing and rendering
 query languages for ElasticSearch.
 
-You can also find the project on the following locations:
+As described in `Parsing queries`_, you can parse Kibana Query Language (KQL),
+Apache Lucene and ElasticSearch queries, and render them using the
+`ElasticSearch Query DSL`_. For example, with KQL:
+
+.. code-block:: python
+
+    from kaquel.kql import parse_kql
+
+    query = parse_kql('identity: { first_name: "John" }')
+    print(query.render())
+
+The project is present at the following locations:
 
 * `Official website and documentation at kaquel.touhey.pro <Kaquel website_>`_;
+* `Kaquel repository on Gitlab <Kaquel on Gitlab_>`_;
 * `kaquel project on PyPI <Kaquel on PyPI_>`_.
 
 .. _Kaquel website: https://kaquel.touhey.pro/
+.. _Kaquel on Gitlab: https://gitlab.com/thomas.touhey/kaquel
 .. _Kaquel on PyPI: https://pypi.org/project/kaquel/
+.. _Parsing queries: https://kaquel.touhey.pro/guides/parse.html
+.. _ElasticSearch Query DSL:
+    https://www.elastic.co/guide/en/elasticsearch/reference/current/
+    query-dsl.html
```

