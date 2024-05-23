# Comparing `tmp/asknews-0.6.7-py3-none-any.whl.zip` & `tmp/asknews-0.6.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 23883 bytes, number of entries: 24
+Zip file size: 23367 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 asknews_sdk/__init__.py
 -rw-r--r--  2.0 unx      415 b- defN 80-Jan-01 00:00 asknews_sdk/api/__init__.py
 -rw-r--r--  2.0 unx     4569 b- defN 80-Jan-01 00:00 asknews_sdk/api/analytics.py
 -rw-r--r--  2.0 unx      203 b- defN 80-Jan-01 00:00 asknews_sdk/api/base.py
--rw-r--r--  2.0 unx     8720 b- defN 80-Jan-01 00:00 asknews_sdk/api/chat.py
--rw-r--r--  2.0 unx    13821 b- defN 80-Jan-01 00:00 asknews_sdk/api/news.py
--rw-r--r--  2.0 unx    11238 b- defN 80-Jan-01 00:00 asknews_sdk/api/stories.py
+-rw-r--r--  2.0 unx     8716 b- defN 80-Jan-01 00:00 asknews_sdk/api/chat.py
+-rw-r--r--  2.0 unx    13983 b- defN 80-Jan-01 00:00 asknews_sdk/api/news.py
+-rw-r--r--  2.0 unx    11870 b- defN 80-Jan-01 00:00 asknews_sdk/api/stories.py
 -rw-r--r--  2.0 unx    16134 b- defN 80-Jan-01 00:00 asknews_sdk/client.py
 -rw-r--r--  2.0 unx      677 b- defN 80-Jan-01 00:00 asknews_sdk/dto/__init__.py
 -rw-r--r--  2.0 unx     4040 b- defN 80-Jan-01 00:00 asknews_sdk/dto/base.py
 -rw-r--r--  2.0 unx     4530 b- defN 80-Jan-01 00:00 asknews_sdk/dto/chat.py
 -rw-r--r--  2.0 unx      674 b- defN 80-Jan-01 00:00 asknews_sdk/dto/error.py
 -rw-r--r--  2.0 unx     1306 b- defN 80-Jan-01 00:00 asknews_sdk/dto/news.py
 -rw-r--r--  2.0 unx      596 b- defN 80-Jan-01 00:00 asknews_sdk/dto/sentiment.py
--rw-r--r--  2.0 unx     6970 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
+-rw-r--r--  2.0 unx     7337 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
 -rw-r--r--  2.0 unx     1451 b- defN 80-Jan-01 00:00 asknews_sdk/errors.py
 -rw-r--r--  2.0 unx     6339 b- defN 80-Jan-01 00:00 asknews_sdk/sdk.py
 -rw-r--r--  2.0 unx     5396 b- defN 80-Jan-01 00:00 asknews_sdk/security.py
 -rw-r--r--  2.0 unx     1614 b- defN 80-Jan-01 00:00 asknews_sdk/utils.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 asknews_sdk/version.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.6.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     3233 b- defN 80-Jan-01 00:00 asknews-0.6.7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.6.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.6.7.dist-info/RECORD
-24 files, 95272 bytes uncompressed, 20849 bytes compressed:  78.1%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.6.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1595 b- defN 80-Jan-01 00:00 asknews-0.6.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.6.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.6.8.dist-info/RECORD
+24 files, 94791 bytes uncompressed, 20333 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: asknews_sdk/utils.py
 Comment: 
 
 Filename: asknews_sdk/version.py
 Comment: 
 
-Filename: asknews-0.6.7.dist-info/LICENSE
+Filename: asknews-0.6.8.dist-info/LICENSE
 Comment: 
 
-Filename: asknews-0.6.7.dist-info/METADATA
+Filename: asknews-0.6.8.dist-info/METADATA
 Comment: 
 
-Filename: asknews-0.6.7.dist-info/WHEEL
+Filename: asknews-0.6.8.dist-info/WHEEL
 Comment: 
 
-Filename: asknews-0.6.7.dist-info/RECORD
+Filename: asknews-0.6.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asknews_sdk/api/chat.py

```diff
@@ -127,15 +127,15 @@
     """
 
     async def get_chat_completions(
         self,
         messages: List[Dict[str, str]],
         model: Literal[
             "gpt-3.5-turbo-16k",
-            "gpt-4-turbo-2024-04-09",
+            "gpt-4-1106-preview",
             "open-mixtral-8x7b",
             "meta-llama/Meta-Llama-3-70B-Instruct",
         ] = "gpt-3.5-turbo-16k",
         stream: bool = False,
         inline_citations: Literal[
             "markdown_link", "numbered", "none"
         ] = "markdown_link",
```

## asknews_sdk/api/news.py

```diff
@@ -53,14 +53,15 @@
             ]
         ] = None,
         doc_start_delimiter: str = "<doc>",
         doc_end_delimiter: str = "</doc>",
         provocative: Optional[str] = "all",
         reporting_voice: Optional[str] = "all",
         domain_url: Optional[str] = None,
+        page_rank: Optional[int] = None,
     ) -> SearchResponse:
         """
         Search for news articles given a query.
 
         https://docs.asknews.app/en/reference#get-/v1/news/search
 
         :param query: Query string that can be any phrase, keyword, question, or
@@ -123,14 +124,15 @@
                 "categories": categories if categories is not None else ["All"],
                 "similarity_score_threshold": similarity_score_threshold,
                 "doc_start_delimiter": doc_start_delimiter,
                 "doc_end_delimiter": doc_end_delimiter,
                 "provocative": provocative,
                 "reporting_voice": reporting_voice,
                 "domain_url": domain_url,
+                "page_rank": page_rank,
             },
             accept=[(SearchResponse.__content_type__, 1.0)],
         )
         return SearchResponse.model_validate(response.content)
 
     def get_sources_report(
         self,
@@ -221,14 +223,15 @@
             ]
         ] = None,
         doc_start_delimiter: str = "<doc>",
         doc_end_delimiter: str = "</doc>",
         provocative: Optional[str] = "all",
         reporting_voice: Optional[str] = "all",
         domain_url: Optional[str] = None,
+        page_rank: Optional[int] = None,
     ) -> SearchResponse:
         """
         Search for news articles given a query.
 
         https://docs.asknews.app/en/reference#get-/v1/news/search
 
         :param query: Query string that can be any phrase, keyword, question, or
@@ -291,14 +294,15 @@
                 "categories": categories if categories is not None else ["All"],
                 "similarity_score_threshold": similarity_score_threshold,
                 "doc_start_delimiter": doc_start_delimiter,
                 "doc_end_delimiter": doc_end_delimiter,
                 "provocative": provocative,
                 "reporting_voice": reporting_voice,
                 "domain_url": domain_url,
+                "page_rank": page_rank,
             },
             accept=[(SearchResponse.__content_type__, 1.0)],
         )
         return SearchResponse.model_validate(response.content)
 
     async def get_sources_report(
         self,
```

## asknews_sdk/api/stories.py

```diff
@@ -57,14 +57,15 @@
         expand_updates: bool = False,
         max_updates: int = 11,
         max_articles: int = 5,
         reddit: int = 0,
         method: Literal["nl", "kw", "both"] = "kw",
         obj_type: Optional[List[Literal["story", "story_update"]]] = None,
         provocative: Literal["unknown", "low", "medium", "high", "all"] = "all",
+        citation_method: Literal["brackets", "urls", "none"] = "brackets",
     ) -> StoriesResponse:
         """
         Get the news stories.
 
         https://docs.asknews.app/en/reference#get-/v1/stories
 
         :param query: The query.
@@ -115,27 +116,29 @@
                 "reddit": reddit,
                 "limit": limit,
                 "expand_updates": expand_updates,
                 "max_updates": max_updates,
                 "max_articles": max_articles,
                 "uuids": uuids,
                 "provocative": provocative,
+                "citation_method": citation_method,
             },
             accept=[(StoriesResponse.__content_type__, 1.0)],
         )
 
         return StoriesResponse.model_validate(response.content)
 
     def get_story(
         self,
         story_id: Union[UUID, str],
         expand_updates: bool = True,
         max_updates: int = 11,
         max_articles: int = 5,
         reddit: int = 0,
+        citation_method: Literal["brackets", "urls", "none"] = "brackets",
     ) -> StoryResponse:
         """
         Get a single news story given the ID.
 
         https://docs.asknews.app/en/reference#get-/v1/stories/-story_id-
 
         :param story_id: The story ID or URL safe title.
@@ -155,14 +158,15 @@
             method="GET",
             endpoint="/v1/stories/{story_id}",
             query={
                 "expand_updates": expand_updates,
                 "max_updates": max_updates,
                 "max_articles": max_articles,
                 "reddit": reddit,
+                "citation_method": citation_method,
             },
             params={"story_id": story_id},
             accept=[(StoryResponse.__content_type__, 1.0)],
         )
         return StoryResponse.model_validate(response.content)
 
 
@@ -218,14 +222,15 @@
         expand_updates: bool = False,
         max_updates: int = 11,
         max_articles: int = 5,
         reddit: int = 0,
         method: Literal["nl", "kw", "both"] = "kw",
         obj_type: Optional[List[Literal["story", "story_update"]]] = None,
         provocative: Literal["unknown", "low", "medium", "high", "all"] = "all",
+        citation_method: Literal["brackets", "urls", "none"] = "brackets",
     ) -> StoriesResponse:
         """
         Get the news stories.
 
         https://docs.asknews.app/en/reference#get-/v1/stories
 
         :param query: The query.
@@ -276,27 +281,30 @@
                 "reddit": reddit,
                 "limit": limit,
                 "expand_updates": expand_updates,
                 "max_updates": max_updates,
                 "max_articles": max_articles,
                 "uuids": uuids,
                 "provocative": provocative,
+                "citation_method": citation_method,
             },
             accept=[(StoriesResponse.__content_type__, 1.0)],
         )
 
         return StoriesResponse.model_validate(response.content)
 
     async def get_story(
         self,
         story_id: Union[UUID, str],
         expand_updates: bool = True,
         max_updates: int = 11,
         max_articles: int = 5,
         reddit: int = 0,
+        citation_method: Literal["brackets", "urls", "none"] = "brackets",
+        condense_auxillary_updates: bool = False,
     ) -> StoryResponse:
         """
         Get a single news story given the ID.
 
         https://docs.asknews.app/en/reference#get-/v1/stories/-story_id-
 
         :param story_id: The story ID or URL safe title.
@@ -316,12 +324,14 @@
             method="GET",
             endpoint="/v1/stories/{story_id}",
             query={
                 "expand_updates": expand_updates,
                 "max_updates": max_updates,
                 "max_articles": max_articles,
                 "reddit": reddit,
+                "citation_method": citation_method,
+                "condense_auxillary_updates": condense_auxillary_updates,
             },
             params={"story_id": story_id},
             accept=[(StoryResponse.__content_type__, 1.0)],
         )
         return StoryResponse.model_validate(response.content)
```

## asknews_sdk/dto/stories.py

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Literal, Optional, Union
 from uuid import UUID
 
 from pydantic import AnyUrl, AwareDatetime, BaseModel, Field
 from typing_extensions import Annotated
 
 from asknews_sdk.dto.base import Article, BaseSchema, Entities, RedditEntities
 
@@ -59,14 +59,19 @@
         Optional[float], Field(0.0, title="Cluster Languages Pct")
     ]
     cluster_probabilities: Annotated[
         Optional[Dict[str, Union[int, float]]], Field({}, title="Cluster Probabilities")
     ]
 
 
+class GraphRelationships(BaseModel):
+    nodes: list[dict[Literal["id", "type"], str]]
+    edges: list[dict[Literal["from", "to", "label"], str]]
+
+
 class StoryResponseUpdate(BaseModel):
     uuid: Annotated[UUID, Field(title="Uuid")]
     cluster_articles: Annotated[List[Article], Field(title="Cluster Articles")]
     prompt_articles: Annotated[List[Article], Field(title="Prompt Articles")]
     n_articles: Annotated[int, Field(title="N Articles")]
     entities: Entities
     headline: Annotated[str, Field(title="Headline")]
@@ -102,14 +107,18 @@
     reporting_voice: Annotated[
         str,
         Field(
             title="An overview of the reporting voice for the articles "
             "comprising this story update."
         ),
     ] = "Unknown"
+    relationships: Annotated[
+        GraphRelationships, Field(title="Relationships mapped out between entities.")
+    ]
+    mermaid: Annotated[str, Field(title="Mermaid syntax for the relationships graph.")]
 
 
 class StoryResponse(BaseSchema):
     uuid: Annotated[UUID, Field(title="Uuid")]
     categories: Annotated[List[str], Field(title="Categories")]
     countries: Annotated[Dict[str, int], Field(title="Countries")]
     countries_pct: Annotated[Dict[str, float], Field(title="Countries Pct")]
```

## Comparing `asknews-0.6.7.dist-info/LICENSE` & `asknews-0.6.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `asknews-0.6.7.dist-info/RECORD` & `asknews-0.6.8.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 asknews_sdk/__init__.py,sha256=TSiiLJIi3INZrbhvrqaXBSAG4MuX5e-Hz7VQstvTOWM,262
 asknews_sdk/api/__init__.py,sha256=1pNfLO6CSeU2bapA-l_oyUQhW2bgavSQUdQcWqjzwno,415
 asknews_sdk/api/analytics.py,sha256=XrH5U5GYXJ5RRTQNVkWYnL-HOD-6yLm6HmNNVWKczxQ,4569
 asknews_sdk/api/base.py,sha256=6w20VMcj9wuMIZLSy_ajbGbMs-cHWbyN7easFpNb8Cg,203
-asknews_sdk/api/chat.py,sha256=7EbwsFKwwmT8Q-7HanDaWrNO8p1bBt565uBHpAH91ao,8720
-asknews_sdk/api/news.py,sha256=iTFsb7nf2d3mwJqE55CPCGFbUGcVgwRzGsrSAOoiNV8,13821
-asknews_sdk/api/stories.py,sha256=ESsisljMV0WCpKGoSWMVDHIbYz4HIX5WPfl7MdWdfeg,11238
+asknews_sdk/api/chat.py,sha256=D6kiJBQQujfaKOSQMNvb5reE9GIY5eaAE01FQx-LWeA,8716
+asknews_sdk/api/news.py,sha256=sNsYC8P4l1gJYt1TT3rusOeHA8LF3VnqVamae6u2Jr0,13983
+asknews_sdk/api/stories.py,sha256=RuS8lqIMQFFZOZwC2sGaPooPsgH8x1Cr4Ozu0ZYtqZw,11870
 asknews_sdk/client.py,sha256=A7irft6UAXEIA8OTC2-EOfp7HSREiT09WAZ7g53iAVM,16134
 asknews_sdk/dto/__init__.py,sha256=dECq34FclMMDeF8Fq62TTngjillmysK8yht2DTOdqHM,677
 asknews_sdk/dto/base.py,sha256=XMozNP4mCiTubVWeQNGdPEzutHtc_y18lTrEfuLbkv4,4040
 asknews_sdk/dto/chat.py,sha256=U76lXLM27LXAxGeMFzbBp9rr5Wi5epXr3H6-2jyZhfc,4530
 asknews_sdk/dto/error.py,sha256=fAJutRBtFzSLcJuZYgTDZtv7-T3p6WBGqk3ky3K481c,674
 asknews_sdk/dto/news.py,sha256=dbpI_BlXISlhS5FGDGl5noNI8Uj7lsbkALBBolAV0C0,1306
 asknews_sdk/dto/sentiment.py,sha256=8UhtmYw9jxwcZ1aw9300g-UE0WEIdo5JmgWbPLR-58w,596
-asknews_sdk/dto/stories.py,sha256=f3QLBnKATwOL0dYpNLzr_WXds_YlAMcjQFGx9Hfe_wY,6970
+asknews_sdk/dto/stories.py,sha256=rjMSy1ciJZH95lMXCBDHXNmKciDg771rtLPRwNaBGNE,7337
 asknews_sdk/errors.py,sha256=2J6fihHeAL1ny7bdGAoEOazaRibosU3N4IFDBlO9vHk,1451
 asknews_sdk/sdk.py,sha256=EMQeZLuPeAWlV8yLbiefY_C7UuG-1pFDp7GwKJ0rsn4,6339
 asknews_sdk/security.py,sha256=mXVyc4_5KE2j-t5fS3IKewUfmCJZLCPbfcXMJJpLzIk,5396
 asknews_sdk/utils.py,sha256=tM7ga0MZGDA4YheH4dyZ6xxVVexMkzTMz0f6ttP6pwU,1614
 asknews_sdk/version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-asknews-0.6.7.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
-asknews-0.6.7.dist-info/METADATA,sha256=zWtv2J8sXNquBgPkJmoadqIIazmWWa1lp_ARS1Lpucc,3233
-asknews-0.6.7.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-asknews-0.6.7.dist-info/RECORD,,
+asknews-0.6.8.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
+asknews-0.6.8.dist-info/METADATA,sha256=jYEXvwgKZANpG78zSfCzH_rATJOpnWl9zyRVXuVzM2E,1595
+asknews-0.6.8.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+asknews-0.6.8.dist-info/RECORD,,
```

