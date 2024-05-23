# Comparing `tmp/customgpt_client-1.2.1.tar.gz` & `tmp/customgpt_client-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customgpt_client-1.2.1.tar", max compression
+gzip compressed data, was "customgpt_client-1.2.2.tar", max compression
```

## Comparing `customgpt_client-1.2.1.tar` & `customgpt_client-1.2.2.tar`

### file list

```diff
@@ -1,653 +1,653 @@
--rw-r--r--   0        0        0      676 2023-10-10 15:40:10.878451 customgpt_client-1.2.1/README.md
--rw-r--r--   0        0        0      105 2023-10-11 11:52:16.100076 customgpt_client-1.2.1/customgpt_client/__init__.py
--rw-r--r--   0        0        0       47 2023-10-11 11:52:11.678464 customgpt_client-1.2.1/customgpt_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-10-11 11:52:11.774499 customgpt_client-1.2.1/customgpt_client/api/citations/__init__.py
--rw-r--r--   0        0        0     6731 2023-10-11 11:52:16.260134 customgpt_client-1.2.1/customgpt_client/api/citations/get_citation.py
--rw-r--r--   0        0        0        0 2023-10-11 11:52:11.758493 customgpt_client-1.2.1/customgpt_client/api/conversations/__init__.py
--rw-r--r--   0        0        0     9063 2023-10-11 11:52:16.276140 customgpt_client-1.2.1/customgpt_client/api/conversations/create_conversation.py
--rw-r--r--   0        0        0     8391 2023-10-11 11:52:16.292146 customgpt_client-1.2.1/customgpt_client/api/conversations/delete_conversation.py
--rw-r--r--   0        0        0     9618 2023-10-11 11:52:16.604259 customgpt_client-1.2.1/customgpt_client/api/conversations/get_conversations.py
--rw-r--r--   0        0        0    10956 2023-10-11 11:52:16.560243 customgpt_client-1.2.1/customgpt_client/api/conversations/messages_conversation.py
--rw-r--r--   0        0        0    10999 2023-10-11 11:52:16.596256 customgpt_client-1.2.1/customgpt_client/api/conversations/send_message.py
--rw-r--r--   0        0        0     8828 2023-10-11 11:52:16.332160 customgpt_client-1.2.1/customgpt_client/api/conversations/update_conversation.py
--rw-r--r--   0        0        0        0 2023-10-11 11:52:11.730483 customgpt_client-1.2.1/customgpt_client/api/page_metadata/__init__.py
--rw-r--r--   0        0        0     6025 2023-10-11 11:52:16.488216 customgpt_client-1.2.1/customgpt_client/api/page_metadata/get_page_metadata.py
--rw-r--r--   0        0        0     7470 2023-10-11 11:52:16.440199 customgpt_client-1.2.1/customgpt_client/api/page_metadata/update_page_metadata.py
--rw-r--r--   0        0        0        0 2023-10-11 11:52:11.718478 customgpt_client-1.2.1/customgpt_client/api/pages/__init__.py
--rw-r--r--   0        0        0     7473 2023-10-11 11:52:16.436198 customgpt_client-1.2.1/customgpt_client/api/pages/delete_page.py
--rw-r--r--   0        0        0     9524 2023-10-11 11:52:16.560243 customgpt_client-1.2.1/customgpt_client/api/pages/get_pages.py
--rw-r--r--   0        0        0     5080 2023-10-11 11:52:16.504222 customgpt_client-1.2.1/customgpt_client/api/pages/preview_citation.py
--rw-r--r--   0        0        0     6711 2023-10-11 11:52:16.568246 customgpt_client-1.2.1/customgpt_client/api/pages/reindex_page.py
--rw-r--r--   0        0        0        0 2023-10-11 11:52:11.750490 customgpt_client-1.2.1/customgpt_client/api/project_plugins/__init__.py
--rw-r--r--   0        0        0     6990 2023-10-11 11:52:16.580250 customgpt_client-1.2.1/customgpt_client/api/project_plugins/create_plugin.py
--rw-r--r--   0        0        0     5730 2023-10-11 11:52:16.776321 customgpt_client-1.2.1/customgpt_client/api/project_plugins/get_plugin.py
--rw-r--r--   0        0        0     6774 2023-10-11 11:52:16.716299 customgpt_client-1.2.1/customgpt_client/api/project_plugins/update_plugin.py
--rw-r--r--   0        0        0        0 2023-10-11 11:52:11.738486 customgpt_client-1.2.1/customgpt_client/api/project_settings/__init__.py
--rw-r--r--   0        0        0     7057 2023-10-11 11:52:16.688289 customgpt_client-1.2.1/customgpt_client/api/project_settings/get_settings.py
--rw-r--r--   0        0        0     7253 2023-10-11 11:52:16.868354 customgpt_client-1.2.1/customgpt_client/api/project_settings/update_settings.py
--rw-r--r--   0        0        0        0 2023-10-11 11:52:11.702472 customgpt_client-1.2.1/customgpt_client/api/projects/__init__.py
--rw-r--r--   0        0        0     7954 2023-10-11 11:52:16.684287 customgpt_client-1.2.1/customgpt_client/api/projects/create_project.py
--rw-r--r--   0        0        0     6966 2023-10-11 11:52:16.704295 customgpt_client-1.2.1/customgpt_client/api/projects/delete_project.py
--rw-r--r--   0        0        0     7353 2023-10-11 11:52:16.884360 customgpt_client-1.2.1/customgpt_client/api/projects/get_project.py
--rw-r--r--   0        0        0     9287 2023-10-11 11:52:17.052420 customgpt_client-1.2.1/customgpt_client/api/projects/list_projects.py
--rw-r--r--   0        0        0     7127 2023-10-11 11:52:16.840344 customgpt_client-1.2.1/customgpt_client/api/projects/stats_project.py
--rw-r--r--   0        0        0     7911 2023-10-11 11:52:16.924374 customgpt_client-1.2.1/customgpt_client/api/projects/update_project.py
--rw-r--r--   0        0        0        0 2023-10-11 11:52:11.778500 customgpt_client-1.2.1/customgpt_client/api/sources/__init__.py
--rw-r--r--   0        0        0     8120 2023-10-11 11:52:16.896364 customgpt_client-1.2.1/customgpt_client/api/sources/create_source.py
--rw-r--r--   0        0        0     6167 2023-10-11 11:52:16.980394 customgpt_client-1.2.1/customgpt_client/api/sources/delete_source.py
--rw-r--r--   0        0        0     6330 2023-10-11 11:52:17.068426 customgpt_client-1.2.1/customgpt_client/api/sources/list_sources.py
--rw-r--r--   0        0        0        0 2023-10-11 11:52:11.786503 customgpt_client-1.2.1/customgpt_client/api/users/__init__.py
--rw-r--r--   0        0        0     4709 2023-10-11 11:52:16.952384 customgpt_client-1.2.1/customgpt_client/api/users/get_user.py
--rw-r--r--   0        0        0     5378 2023-10-11 11:52:17.076429 customgpt_client-1.2.1/customgpt_client/api/users/update_user.py
--rw-r--r--   0        0        0    19381 2023-10-11 11:52:17.556602 customgpt_client-1.2.1/customgpt_client/client.py
--rw-r--r--   0        0        0      470 2023-10-11 11:52:16.908368 customgpt_client-1.2.1/customgpt_client/errors.py
--rw-r--r--   0        0        0    68823 2023-10-11 11:52:14.967666 customgpt_client-1.2.1/customgpt_client/models/__init__.py
--rw-r--r--   0        0        0     4857 2023-10-11 11:52:17.128448 customgpt_client-1.2.1/customgpt_client/models/conversation.py
--rw-r--r--   0        0        0     1545 2023-10-11 11:52:17.004403 customgpt_client-1.2.1/customgpt_client/models/create_conversation_json_body.py
--rw-r--r--   0        0        0     2551 2023-10-11 11:52:17.160459 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_201.py
--rw-r--r--   0        0        0     5103 2023-10-11 11:52:17.216480 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_201_data.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.795603 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_201_status.py
--rw-r--r--   0        0        0     2835 2023-10-11 11:52:17.268498 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_400.py
--rw-r--r--   0        0        0     2010 2023-10-11 11:52:17.228484 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_400_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.831616 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_400_data_code.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.451478 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_400_status.py
--rw-r--r--   0        0        0     2835 2023-10-11 11:52:17.356530 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_401.py
--rw-r--r--   0        0        0     2005 2023-10-11 11:52:17.228484 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_401_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.679561 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_401_data_code.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.759590 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_401_status.py
--rw-r--r--   0        0        0     2835 2023-10-11 11:52:17.396545 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_404.py
--rw-r--r--   0        0        0     2179 2023-10-11 11:52:17.284504 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_404_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.427469 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_404_data_code.py
--rw-r--r--   0        0        0      281 2023-10-11 11:52:14.807607 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_404_data_message.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.203387 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_404_status.py
--rw-r--r--   0        0        0     2835 2023-10-11 11:52:17.324519 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_500.py
--rw-r--r--   0        0        0     1988 2023-10-11 11:52:17.308513 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_500_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.359444 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_500_data_code.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:15.187745 customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_500_status.py
--rw-r--r--   0        0        0     2992 2023-10-11 11:52:17.420553 customgpt_client-1.2.1/customgpt_client/models/create_plugin_json_body.py
--rw-r--r--   0        0        0     2467 2023-10-11 11:52:17.492579 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_201.py
--rw-r--r--   0        0        0     3317 2023-10-11 11:52:17.388542 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_201_data.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:15.527869 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_201_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:17.464569 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_400.py
--rw-r--r--   0        0        0     1974 2023-10-11 11:52:17.392543 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_400_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.535508 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_400_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.303424 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_400_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:17.524591 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_401.py
--rw-r--r--   0        0        0     1969 2023-10-11 11:52:17.456566 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_401_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:15.551878 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_401_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:15.319793 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_401_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:17.488578 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_404.py
--rw-r--r--   0        0        0     2137 2023-10-11 11:52:17.552601 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_404_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.663555 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_404_data_code.py
--rw-r--r--   0        0        0      275 2023-10-11 11:52:15.511863 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_404_data_message.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:15.443838 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_404_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:17.560603 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_500.py
--rw-r--r--   0        0        0     1952 2023-10-11 11:52:17.516588 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_500_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:15.027687 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_500_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:15.259772 customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_500_status.py
--rw-r--r--   0        0        0     4387 2023-10-11 11:52:17.596617 customgpt_client-1.2.1/customgpt_client/models/create_project_multipart_data.py
--rw-r--r--   0        0        0     2481 2023-10-11 11:52:17.560603 customgpt_client-1.2.1/customgpt_client/models/create_project_response_201.py
--rw-r--r--   0        0        0     7714 2023-10-11 11:52:17.984756 customgpt_client-1.2.1/customgpt_client/models/create_project_response_201_data.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.695567 customgpt_client-1.2.1/customgpt_client/models/create_project_response_201_data_type.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:14.483489 customgpt_client-1.2.1/customgpt_client/models/create_project_response_201_status.py
--rw-r--r--   0        0        0     2765 2023-10-11 11:52:17.600618 customgpt_client-1.2.1/customgpt_client/models/create_project_response_400.py
--rw-r--r--   0        0        0     2144 2023-10-11 11:52:17.624627 customgpt_client-1.2.1/customgpt_client/models/create_project_response_400_data.py
--rw-r--r--   0        0        0      258 2023-10-11 11:52:15.403824 customgpt_client-1.2.1/customgpt_client/models/create_project_response_400_data_code.py
--rw-r--r--   0        0        0      362 2023-10-11 11:52:14.543511 customgpt_client-1.2.1/customgpt_client/models/create_project_response_400_data_message.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:14.639546 customgpt_client-1.2.1/customgpt_client/models/create_project_response_400_status.py
--rw-r--r--   0        0        0     2765 2023-10-11 11:52:17.644634 customgpt_client-1.2.1/customgpt_client/models/create_project_response_401.py
--rw-r--r--   0        0        0     1975 2023-10-11 11:52:17.680647 customgpt_client-1.2.1/customgpt_client/models/create_project_response_401_data.py
--rw-r--r--   0        0        0      258 2023-10-11 11:52:14.211390 customgpt_client-1.2.1/customgpt_client/models/create_project_response_401_data_code.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:14.683562 customgpt_client-1.2.1/customgpt_client/models/create_project_response_401_status.py
--rw-r--r--   0        0        0     2765 2023-10-11 11:52:17.644634 customgpt_client-1.2.1/customgpt_client/models/create_project_response_500.py
--rw-r--r--   0        0        0     1958 2023-10-11 11:52:17.692651 customgpt_client-1.2.1/customgpt_client/models/create_project_response_500_data.py
--rw-r--r--   0        0        0      258 2023-10-11 11:52:15.335799 customgpt_client-1.2.1/customgpt_client/models/create_project_response_500_data_code.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:15.571885 customgpt_client-1.2.1/customgpt_client/models/create_project_response_500_status.py
--rw-r--r--   0        0        0     3757 2023-10-11 11:52:17.816696 customgpt_client-1.2.1/customgpt_client/models/create_source_multipart_data.py
--rw-r--r--   0        0        0     2467 2023-10-11 11:52:17.676645 customgpt_client-1.2.1/customgpt_client/models/create_source_response_201.py
--rw-r--r--   0        0        0     5456 2023-10-11 11:52:17.908729 customgpt_client-1.2.1/customgpt_client/models/create_source_response_201_data.py
--rw-r--r--   0        0        0     8038 2023-10-11 11:52:17.916732 customgpt_client-1.2.1/customgpt_client/models/create_source_response_201_data_pages_item.py
--rw-r--r--   0        0        0      249 2023-10-11 11:52:14.251405 customgpt_client-1.2.1/customgpt_client/models/create_source_response_201_data_pages_item_crawl_status.py
--rw-r--r--   0        0        0      249 2023-10-11 11:52:14.847622 customgpt_client-1.2.1/customgpt_client/models/create_source_response_201_data_pages_item_index_status.py
--rw-r--r--   0        0        0     3040 2023-10-11 11:52:17.728664 customgpt_client-1.2.1/customgpt_client/models/create_source_response_201_data_settings.py
--rw-r--r--   0        0        0      182 2023-10-11 11:52:15.375814 customgpt_client-1.2.1/customgpt_client/models/create_source_response_201_data_type.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.291420 customgpt_client-1.2.1/customgpt_client/models/create_source_response_201_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:17.772680 customgpt_client-1.2.1/customgpt_client/models/create_source_response_400.py
--rw-r--r--   0        0        0     2111 2023-10-11 11:52:17.840705 customgpt_client-1.2.1/customgpt_client/models/create_source_response_400_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.911645 customgpt_client-1.2.1/customgpt_client/models/create_source_response_400_data_code.py
--rw-r--r--   0        0        0      399 2023-10-11 11:52:14.371449 customgpt_client-1.2.1/customgpt_client/models/create_source_response_400_data_message.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.191383 customgpt_client-1.2.1/customgpt_client/models/create_source_response_400_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:17.996761 customgpt_client-1.2.1/customgpt_client/models/create_source_response_401.py
--rw-r--r--   0        0        0     1969 2023-10-11 11:52:17.808693 customgpt_client-1.2.1/customgpt_client/models/create_source_response_401_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:15.403824 customgpt_client-1.2.1/customgpt_client/models/create_source_response_401_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.463482 customgpt_client-1.2.1/customgpt_client/models/create_source_response_401_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:17.880719 customgpt_client-1.2.1/customgpt_client/models/create_source_response_404.py
--rw-r--r--   0        0        0     2137 2023-10-11 11:52:17.904728 customgpt_client-1.2.1/customgpt_client/models/create_source_response_404_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.275414 customgpt_client-1.2.1/customgpt_client/models/create_source_response_404_data_code.py
--rw-r--r--   0        0        0      275 2023-10-11 11:52:14.307425 customgpt_client-1.2.1/customgpt_client/models/create_source_response_404_data_message.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.899641 customgpt_client-1.2.1/customgpt_client/models/create_source_response_404_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:17.996761 customgpt_client-1.2.1/customgpt_client/models/create_source_response_500.py
--rw-r--r--   0        0        0     1952 2023-10-11 11:52:17.984756 customgpt_client-1.2.1/customgpt_client/models/create_source_response_500_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.591529 customgpt_client-1.2.1/customgpt_client/models/create_source_response_500_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.647549 customgpt_client-1.2.1/customgpt_client/models/create_source_response_500_status.py
--rw-r--r--   0        0        0     2551 2023-10-11 11:52:18.040777 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_200.py
--rw-r--r--   0        0        0     1641 2023-10-11 11:52:17.984756 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_200_data.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.831616 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_200_status.py
--rw-r--r--   0        0        0     2835 2023-10-11 11:52:18.080791 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_400.py
--rw-r--r--   0        0        0     2010 2023-10-11 11:52:18.148815 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_400_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.387454 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_400_data_code.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.895640 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_400_status.py
--rw-r--r--   0        0        0     2835 2023-10-11 11:52:18.440920 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_401.py
--rw-r--r--   0        0        0     2005 2023-10-11 11:52:18.064785 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_401_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.247403 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_401_data_code.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.395457 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_401_status.py
--rw-r--r--   0        0        0     2835 2023-10-11 11:52:18.208837 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_404.py
--rw-r--r--   0        0        0     2179 2023-10-11 11:52:18.244850 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_404_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.419466 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_404_data_code.py
--rw-r--r--   0        0        0      281 2023-10-11 11:52:15.287782 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_404_data_message.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.507498 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_404_status.py
--rw-r--r--   0        0        0     2835 2023-10-11 11:52:18.112802 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_500.py
--rw-r--r--   0        0        0     1988 2023-10-11 11:52:18.136811 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_500_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:15.199750 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_500_data_code.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:15.503860 customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_500_status.py
--rw-r--r--   0        0        0     2439 2023-10-11 11:52:18.176825 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_200.py
--rw-r--r--   0        0        0     1601 2023-10-11 11:52:18.148815 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_200_data.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:15.215756 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_200_status.py
--rw-r--r--   0        0        0     2723 2023-10-11 11:52:18.216840 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_400.py
--rw-r--r--   0        0        0     1962 2023-10-11 11:52:18.264857 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_400_data.py
--rw-r--r--   0        0        0      255 2023-10-11 11:52:14.599532 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_400_data_code.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:15.211754 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_400_status.py
--rw-r--r--   0        0        0     2723 2023-10-11 11:52:18.460927 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_401.py
--rw-r--r--   0        0        0     1957 2023-10-11 11:52:18.232845 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_401_data.py
--rw-r--r--   0        0        0      255 2023-10-11 11:52:15.351805 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_401_data_code.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:14.575523 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_401_status.py
--rw-r--r--   0        0        0     2723 2023-10-11 11:52:18.336883 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_404.py
--rw-r--r--   0        0        0     2123 2023-10-11 11:52:18.432917 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_404_data.py
--rw-r--r--   0        0        0      255 2023-10-11 11:52:14.207389 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_404_data_code.py
--rw-r--r--   0        0        0      273 2023-10-11 11:52:14.423467 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_404_data_message.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:14.891638 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_404_status.py
--rw-r--r--   0        0        0     2723 2023-10-11 11:52:18.384900 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_500.py
--rw-r--r--   0        0        0     1940 2023-10-11 11:52:18.312874 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_500_data.py
--rw-r--r--   0        0        0      255 2023-10-11 11:52:15.535872 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_500_data_code.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:15.051696 customgpt_client-1.2.1/customgpt_client/models/delete_page_response_500_status.py
--rw-r--r--   0        0        0     2481 2023-10-11 11:52:18.488937 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_200.py
--rw-r--r--   0        0        0     1616 2023-10-11 11:52:18.380899 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_200_data.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:15.159735 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_200_status.py
--rw-r--r--   0        0        0     2765 2023-10-11 11:52:18.440920 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_400.py
--rw-r--r--   0        0        0     1980 2023-10-11 11:52:18.452925 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_400_data.py
--rw-r--r--   0        0        0      258 2023-10-11 11:52:14.827615 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_400_data_code.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:14.815610 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_400_status.py
--rw-r--r--   0        0        0     2765 2023-10-11 11:52:18.476933 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_401.py
--rw-r--r--   0        0        0     1975 2023-10-11 11:52:18.540956 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_401_data.py
--rw-r--r--   0        0        0      258 2023-10-11 11:52:14.599532 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_401_data_code.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:15.039692 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_401_status.py
--rw-r--r--   0        0        0     2765 2023-10-11 11:52:18.697012 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_404.py
--rw-r--r--   0        0        0     2144 2023-10-11 11:52:18.504943 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_404_data.py
--rw-r--r--   0        0        0      258 2023-10-11 11:52:14.643548 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_404_data_code.py
--rw-r--r--   0        0        0      276 2023-10-11 11:52:14.467484 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_404_data_message.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:14.771594 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_404_status.py
--rw-r--r--   0        0        0     2765 2023-10-11 11:52:18.548959 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_500.py
--rw-r--r--   0        0        0     1958 2023-10-11 11:52:18.544957 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_500_data.py
--rw-r--r--   0        0        0      258 2023-10-11 11:52:15.031689 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_500_data_code.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:14.439473 customgpt_client-1.2.1/customgpt_client/models/delete_project_response_500_status.py
--rw-r--r--   0        0        0     2467 2023-10-11 11:52:18.552960 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_200.py
--rw-r--r--   0        0        0     1618 2023-10-11 11:52:18.568966 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_200_data.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.427469 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_200_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:18.648995 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_400.py
--rw-r--r--   0        0        0     1974 2023-10-11 11:52:18.564965 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_400_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.283417 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_400_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.367447 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_400_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:18.628988 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_401.py
--rw-r--r--   0        0        0     1969 2023-10-11 11:52:18.612982 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_401_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.835618 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_401_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.831616 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_401_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:18.721021 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_404.py
--rw-r--r--   0        0        0     2137 2023-10-11 11:52:18.628988 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_404_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.883635 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_404_data_code.py
--rw-r--r--   0        0        0      275 2023-10-11 11:52:15.527869 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_404_data_message.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.703570 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_404_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:18.656998 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_500.py
--rw-r--r--   0        0        0     1952 2023-10-11 11:52:18.632989 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_500_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.299422 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_500_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:15.571885 customgpt_client-1.2.1/customgpt_client/models/delete_source_response_500_status.py
--rw-r--r--   0        0        0     2453 2023-10-11 11:52:18.693011 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_200.py
--rw-r--r--   0        0        0     4330 2023-10-11 11:52:18.777041 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_200_data.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.723577 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_200_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:18.717019 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_400.py
--rw-r--r--   0        0        0     1968 2023-10-11 11:52:18.689009 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_400_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:14.439473 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_400_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.975669 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_400_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:18.837062 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_401.py
--rw-r--r--   0        0        0     1963 2023-10-11 11:52:18.777041 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_401_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:15.095712 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_401_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:15.315792 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_401_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:18.781042 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_404.py
--rw-r--r--   0        0        0     2130 2023-10-11 11:52:18.769038 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_404_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:15.427833 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_404_data_code.py
--rw-r--r--   0        0        0      274 2023-10-11 11:52:15.071704 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_404_data_message.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:15.511863 customgpt_client-1.2.1/customgpt_client/models/get_citation_response_404_status.py
--rw-r--r--   0        0        0      160 2023-10-11 11:52:14.191383 customgpt_client-1.2.1/customgpt_client/models/get_conversations_order.py
--rw-r--r--   0        0        0     2523 2023-10-11 11:52:18.845065 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_200.py
--rw-r--r--   0        0        0     6048 2023-10-11 11:52:18.885080 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_200_data.py
--rw-r--r--   0        0        0     5139 2023-10-11 11:52:18.965108 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_200_data_data_item.py
--rw-r--r--   0        0        0      182 2023-10-11 11:52:14.743584 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_200_status.py
--rw-r--r--   0        0        0     2807 2023-10-11 11:52:18.865072 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_400.py
--rw-r--r--   0        0        0     1998 2023-10-11 11:52:18.889081 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_400_data.py
--rw-r--r--   0        0        0      261 2023-10-11 11:52:15.435835 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_400_data_code.py
--rw-r--r--   0        0        0      182 2023-10-11 11:52:15.535872 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_400_status.py
--rw-r--r--   0        0        0     2807 2023-10-11 11:52:18.881078 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_401.py
--rw-r--r--   0        0        0     1993 2023-10-11 11:52:18.873075 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_401_data.py
--rw-r--r--   0        0        0      261 2023-10-11 11:52:15.163737 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_401_data_code.py
--rw-r--r--   0        0        0      182 2023-10-11 11:52:14.835618 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_401_status.py
--rw-r--r--   0        0        0     2807 2023-10-11 11:52:19.061143 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_404.py
--rw-r--r--   0        0        0     2165 2023-10-11 11:52:18.957105 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_404_data.py
--rw-r--r--   0        0        0      261 2023-10-11 11:52:14.539510 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_404_data_code.py
--rw-r--r--   0        0        0      279 2023-10-11 11:52:14.547513 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_404_data_message.py
--rw-r--r--   0        0        0      182 2023-10-11 11:52:14.411463 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_404_status.py
--rw-r--r--   0        0        0     2807 2023-10-11 11:52:19.097156 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_500.py
--rw-r--r--   0        0        0     1976 2023-10-11 11:52:18.993118 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_500_data.py
--rw-r--r--   0        0        0      261 2023-10-11 11:52:15.003679 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_500_data_code.py
--rw-r--r--   0        0        0      182 2023-10-11 11:52:14.223395 customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_500_status.py
--rw-r--r--   0        0        0      207 2023-10-11 11:52:14.647549 customgpt_client-1.2.1/customgpt_client/models/get_conversations_user_filter.py
--rw-r--r--   0        0        0     2514 2023-10-11 11:52:19.033133 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_200.py
--rw-r--r--   0        0        0     2666 2023-10-11 11:52:18.977113 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_200_data.py
--rw-r--r--   0        0        0      181 2023-10-11 11:52:14.195385 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_200_status.py
--rw-r--r--   0        0        0     2798 2023-10-11 11:52:19.149174 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_400.py
--rw-r--r--   0        0        0     1990 2023-10-11 11:52:19.093154 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_400_data.py
--rw-r--r--   0        0        0      260 2023-10-11 11:52:14.503497 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_400_data_code.py
--rw-r--r--   0        0        0      181 2023-10-11 11:52:14.787600 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_400_status.py
--rw-r--r--   0        0        0     2798 2023-10-11 11:52:19.085151 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_401.py
--rw-r--r--   0        0        0     1990 2023-10-11 11:52:19.145173 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_401_data.py
--rw-r--r--   0        0        0      260 2023-10-11 11:52:15.327796 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_401_data_code.py
--rw-r--r--   0        0        0      181 2023-10-11 11:52:14.303424 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_401_status.py
--rw-r--r--   0        0        0     2798 2023-10-11 11:52:19.113161 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_404.py
--rw-r--r--   0        0        0     2155 2023-10-11 11:52:19.121164 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_404_data.py
--rw-r--r--   0        0        0      260 2023-10-11 11:52:15.007680 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_404_data_code.py
--rw-r--r--   0        0        0      260 2023-10-11 11:52:14.199386 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_404_data_message.py
--rw-r--r--   0        0        0      181 2023-10-11 11:52:15.279779 customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_404_status.py
--rw-r--r--   0        0        0      152 2023-10-11 11:52:14.895640 customgpt_client-1.2.1/customgpt_client/models/get_pages_order.py
--rw-r--r--   0        0        0     2411 2023-10-11 11:52:19.177184 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200.py
--rw-r--r--   0        0        0     2919 2023-10-11 11:52:19.321236 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200_data.py
--rw-r--r--   0        0        0     6017 2023-10-11 11:52:19.389260 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200_data_pages.py
--rw-r--r--   0        0        0     8041 2023-10-11 11:52:19.521307 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200_data_pages_data_item.py
--rw-r--r--   0        0        0      249 2023-10-11 11:52:15.095712 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200_data_pages_data_item_crawl_status.py
--rw-r--r--   0        0        0      249 2023-10-11 11:52:15.087709 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200_data_pages_data_item_index_status.py
--rw-r--r--   0        0        0     7731 2023-10-11 11:52:19.361250 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200_data_project.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:14.763591 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200_data_project_type.py
--rw-r--r--   0        0        0      174 2023-10-11 11:52:14.891638 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200_status.py
--rw-r--r--   0        0        0     2695 2023-10-11 11:52:19.237206 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_400.py
--rw-r--r--   0        0        0     1950 2023-10-11 11:52:19.285223 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_400_data.py
--rw-r--r--   0        0        0      253 2023-10-11 11:52:15.063701 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_400_data_code.py
--rw-r--r--   0        0        0      174 2023-10-11 11:52:15.235763 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_400_status.py
--rw-r--r--   0        0        0     2695 2023-10-11 11:52:19.433276 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_401.py
--rw-r--r--   0        0        0     1945 2023-10-11 11:52:19.305230 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_401_data.py
--rw-r--r--   0        0        0      253 2023-10-11 11:52:14.343438 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_401_data_code.py
--rw-r--r--   0        0        0      174 2023-10-11 11:52:15.083708 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_401_status.py
--rw-r--r--   0        0        0     2695 2023-10-11 11:52:19.353247 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_404.py
--rw-r--r--   0        0        0     2097 2023-10-11 11:52:19.413269 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_404_data.py
--rw-r--r--   0        0        0      253 2023-10-11 11:52:15.079706 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_404_data_code.py
--rw-r--r--   0        0        0      271 2023-10-11 11:52:15.555879 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_404_data_message.py
--rw-r--r--   0        0        0      174 2023-10-11 11:52:14.923650 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_404_status.py
--rw-r--r--   0        0        0     2695 2023-10-11 11:52:19.401265 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_500.py
--rw-r--r--   0        0        0     1928 2023-10-11 11:52:19.437277 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_500_data.py
--rw-r--r--   0        0        0      253 2023-10-11 11:52:14.195385 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_500_data_code.py
--rw-r--r--   0        0        0      174 2023-10-11 11:52:14.559517 customgpt_client-1.2.1/customgpt_client/models/get_pages_response_500_status.py
--rw-r--r--   0        0        0     2425 2023-10-11 11:52:19.437277 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_200.py
--rw-r--r--   0        0        0     3302 2023-10-11 11:52:19.453283 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_200_data.py
--rw-r--r--   0        0        0      175 2023-10-11 11:52:14.571521 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_200_status.py
--rw-r--r--   0        0        0     2709 2023-10-11 11:52:19.545316 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_400.py
--rw-r--r--   0        0        0     1956 2023-10-11 11:52:19.465287 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_400_data.py
--rw-r--r--   0        0        0      254 2023-10-11 11:52:14.179379 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_400_data_code.py
--rw-r--r--   0        0        0      175 2023-10-11 11:52:15.271776 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_400_status.py
--rw-r--r--   0        0        0     2709 2023-10-11 11:52:19.581329 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_401.py
--rw-r--r--   0        0        0     1951 2023-10-11 11:52:19.573326 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_401_data.py
--rw-r--r--   0        0        0      254 2023-10-11 11:52:14.699568 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_401_data_code.py
--rw-r--r--   0        0        0      175 2023-10-11 11:52:14.763591 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_401_status.py
--rw-r--r--   0        0        0     2709 2023-10-11 11:52:19.521307 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_404.py
--rw-r--r--   0        0        0     2130 2023-10-11 11:52:19.525309 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_404_data.py
--rw-r--r--   0        0        0      254 2023-10-11 11:52:15.147731 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_404_data_code.py
--rw-r--r--   0        0        0      402 2023-10-11 11:52:15.063701 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_404_data_message.py
--rw-r--r--   0        0        0      175 2023-10-11 11:52:14.555516 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_404_status.py
--rw-r--r--   0        0        0     2709 2023-10-11 11:52:19.545316 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_500.py
--rw-r--r--   0        0        0     1934 2023-10-11 11:52:19.525309 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_500_data.py
--rw-r--r--   0        0        0      254 2023-10-11 11:52:14.623540 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_500_data_code.py
--rw-r--r--   0        0        0      175 2023-10-11 11:52:14.831616 customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_500_status.py
--rw-r--r--   0        0        0     2439 2023-10-11 11:52:19.633347 customgpt_client-1.2.1/customgpt_client/models/get_project_response_200.py
--rw-r--r--   0        0        0     7693 2023-10-11 11:52:19.881436 customgpt_client-1.2.1/customgpt_client/models/get_project_response_200_data.py
--rw-r--r--   0        0        0      174 2023-10-11 11:52:14.535508 customgpt_client-1.2.1/customgpt_client/models/get_project_response_200_data_type.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:14.263409 customgpt_client-1.2.1/customgpt_client/models/get_project_response_200_status.py
--rw-r--r--   0        0        0     2723 2023-10-11 11:52:19.673362 customgpt_client-1.2.1/customgpt_client/models/get_project_response_400.py
--rw-r--r--   0        0        0     1962 2023-10-11 11:52:19.665359 customgpt_client-1.2.1/customgpt_client/models/get_project_response_400_data.py
--rw-r--r--   0        0        0      255 2023-10-11 11:52:15.067702 customgpt_client-1.2.1/customgpt_client/models/get_project_response_400_data_code.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:15.495857 customgpt_client-1.2.1/customgpt_client/models/get_project_response_400_status.py
--rw-r--r--   0        0        0     2723 2023-10-11 11:52:19.653355 customgpt_client-1.2.1/customgpt_client/models/get_project_response_401.py
--rw-r--r--   0        0        0     1957 2023-10-11 11:52:19.617342 customgpt_client-1.2.1/customgpt_client/models/get_project_response_401_data.py
--rw-r--r--   0        0        0      255 2023-10-11 11:52:15.555879 customgpt_client-1.2.1/customgpt_client/models/get_project_response_401_data_code.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:14.323431 customgpt_client-1.2.1/customgpt_client/models/get_project_response_401_status.py
--rw-r--r--   0        0        0     2723 2023-10-11 11:52:19.665359 customgpt_client-1.2.1/customgpt_client/models/get_project_response_404.py
--rw-r--r--   0        0        0     2123 2023-10-11 11:52:19.665359 customgpt_client-1.2.1/customgpt_client/models/get_project_response_404_data.py
--rw-r--r--   0        0        0      255 2023-10-11 11:52:15.547876 customgpt_client-1.2.1/customgpt_client/models/get_project_response_404_data_code.py
--rw-r--r--   0        0        0      273 2023-10-11 11:52:15.431834 customgpt_client-1.2.1/customgpt_client/models/get_project_response_404_data_message.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:15.067702 customgpt_client-1.2.1/customgpt_client/models/get_project_response_404_status.py
--rw-r--r--   0        0        0     2723 2023-10-11 11:52:19.705373 customgpt_client-1.2.1/customgpt_client/models/get_project_response_500.py
--rw-r--r--   0        0        0     1940 2023-10-11 11:52:19.697370 customgpt_client-1.2.1/customgpt_client/models/get_project_response_500_data.py
--rw-r--r--   0        0        0      255 2023-10-11 11:52:14.371449 customgpt_client-1.2.1/customgpt_client/models/get_project_response_500_data_code.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:15.375814 customgpt_client-1.2.1/customgpt_client/models/get_project_response_500_status.py
--rw-r--r--   0        0        0     2453 2023-10-11 11:52:19.733383 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_200.py
--rw-r--r--   0        0        0    12798 2023-10-11 11:52:19.925452 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_200_data.py
--rw-r--r--   0        0        0      202 2023-10-11 11:52:14.191383 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_200_data_citations_view_type.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:15.019685 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_200_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:19.889439 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_400.py
--rw-r--r--   0        0        0     1968 2023-10-11 11:52:19.829418 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_400_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:15.307789 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_400_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:15.407825 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_400_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:19.881436 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_401.py
--rw-r--r--   0        0        0     1963 2023-10-11 11:52:19.817413 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_401_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:15.579888 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_401_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.415465 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_401_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:19.857428 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_404.py
--rw-r--r--   0        0        0     2130 2023-10-11 11:52:19.873433 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_404_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:14.511500 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_404_data_code.py
--rw-r--r--   0        0        0      274 2023-10-11 11:52:14.603533 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_404_data_message.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:15.559881 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_404_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:19.969468 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_500.py
--rw-r--r--   0        0        0     1946 2023-10-11 11:52:19.965466 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_500_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:14.319430 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_500_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.675559 customgpt_client-1.2.1/customgpt_client/models/get_settings_response_500_status.py
--rw-r--r--   0        0        0     2397 2023-10-11 11:52:19.945459 customgpt_client-1.2.1/customgpt_client/models/get_user_response_200.py
--rw-r--r--   0        0        0     3872 2023-10-11 11:52:19.993476 customgpt_client-1.2.1/customgpt_client/models/get_user_response_200_data.py
--rw-r--r--   0        0        0      173 2023-10-11 11:52:15.495857 customgpt_client-1.2.1/customgpt_client/models/get_user_response_200_status.py
--rw-r--r--   0        0        0     2681 2023-10-11 11:52:20.073505 customgpt_client-1.2.1/customgpt_client/models/get_user_response_401.py
--rw-r--r--   0        0        0     1939 2023-10-11 11:52:19.965466 customgpt_client-1.2.1/customgpt_client/models/get_user_response_401_data.py
--rw-r--r--   0        0        0      252 2023-10-11 11:52:15.555879 customgpt_client-1.2.1/customgpt_client/models/get_user_response_401_data_code.py
--rw-r--r--   0        0        0      173 2023-10-11 11:52:14.519502 customgpt_client-1.2.1/customgpt_client/models/get_user_response_401_status.py
--rw-r--r--   0        0        0     2681 2023-10-11 11:52:20.049496 customgpt_client-1.2.1/customgpt_client/models/get_user_response_500.py
--rw-r--r--   0        0        0     1922 2023-10-11 11:52:19.993476 customgpt_client-1.2.1/customgpt_client/models/get_user_response_500_data.py
--rw-r--r--   0        0        0      252 2023-10-11 11:52:15.075705 customgpt_client-1.2.1/customgpt_client/models/get_user_response_500_data_code.py
--rw-r--r--   0        0        0      173 2023-10-11 11:52:14.451478 customgpt_client-1.2.1/customgpt_client/models/get_user_response_500_status.py
--rw-r--r--   0        0        0      156 2023-10-11 11:52:14.595530 customgpt_client-1.2.1/customgpt_client/models/list_projects_order.py
--rw-r--r--   0        0        0     2467 2023-10-11 11:52:20.053498 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_200.py
--rw-r--r--   0        0        0     6000 2023-10-11 11:52:20.189546 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_200_data.py
--rw-r--r--   0        0        0     7769 2023-10-11 11:52:20.221558 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_200_data_data_item.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:15.115719 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_200_data_data_item_type.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.511500 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_200_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:20.077506 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_401.py
--rw-r--r--   0        0        0     1969 2023-10-11 11:52:20.057499 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_401_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.291420 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_401_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:15.595893 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_401_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:20.089511 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_500.py
--rw-r--r--   0        0        0     1952 2023-10-11 11:52:20.189546 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_500_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:15.583889 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_500_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:15.503860 customgpt_client-1.2.1/customgpt_client/models/list_projects_response_500_status.py
--rw-r--r--   0        0        0     2453 2023-10-11 11:52:20.141529 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200.py
--rw-r--r--   0        0        0     3300 2023-10-11 11:52:20.157535 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data.py
--rw-r--r--   0        0        0     5785 2023-10-11 11:52:20.349603 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_sitemaps_item.py
--rw-r--r--   0        0        0     8143 2023-10-11 11:52:20.461643 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_sitemaps_item_pages_item.py
--rw-r--r--   0        0        0      260 2023-10-11 11:52:15.487854 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_sitemaps_item_pages_item_crawl_status.py
--rw-r--r--   0        0        0      260 2023-10-11 11:52:15.459844 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_sitemaps_item_pages_item_index_status.py
--rw-r--r--   0        0        0     3101 2023-10-11 11:52:20.229560 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_sitemaps_item_settings.py
--rw-r--r--   0        0        0      193 2023-10-11 11:52:15.039692 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_sitemaps_item_type.py
--rw-r--r--   0        0        0     5614 2023-10-11 11:52:20.313590 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_uploads.py
--rw-r--r--   0        0        0     8095 2023-10-11 11:52:20.369610 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_uploads_pages_item.py
--rw-r--r--   0        0        0      255 2023-10-11 11:52:14.791602 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_uploads_pages_item_crawl_status.py
--rw-r--r--   0        0        0      255 2023-10-11 11:52:15.203751 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_uploads_pages_item_index_status.py
--rw-r--r--   0        0        0     3073 2023-10-11 11:52:20.349603 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_uploads_settings.py
--rw-r--r--   0        0        0      188 2023-10-11 11:52:15.283780 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_uploads_type.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.847622 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:20.341601 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_400.py
--rw-r--r--   0        0        0     1968 2023-10-11 11:52:20.301586 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_400_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:15.547876 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_400_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.575523 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_400_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:20.341601 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_401.py
--rw-r--r--   0        0        0     1963 2023-10-11 11:52:20.373612 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_401_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:14.919648 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_401_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.239400 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_401_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:20.401622 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_404.py
--rw-r--r--   0        0        0     2130 2023-10-11 11:52:20.413626 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_404_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:14.719575 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_404_data_code.py
--rw-r--r--   0        0        0      274 2023-10-11 11:52:14.907644 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_404_data_message.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.919648 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_404_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:20.505659 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_500.py
--rw-r--r--   0        0        0     1946 2023-10-11 11:52:20.417628 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_500_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:14.815610 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_500_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.519502 customgpt_client-1.2.1/customgpt_client/models/list_sources_response_500_status.py
--rw-r--r--   0        0        0      164 2023-10-11 11:52:14.667556 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_order.py
--rw-r--r--   0        0        0     2579 2023-10-11 11:52:20.433633 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200.py
--rw-r--r--   0        0        0     3446 2023-10-11 11:52:20.449639 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200_data.py
--rw-r--r--   0        0        0     5176 2023-10-11 11:52:20.521665 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200_data_conversation.py
--rw-r--r--   0        0        0     6239 2023-10-11 11:52:20.585687 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200_data_messages.py
--rw-r--r--   0        0        0     6593 2023-10-11 11:52:20.601693 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200_data_messages_data_item.py
--rw-r--r--   0        0        0     3153 2023-10-11 11:52:20.497656 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200_data_messages_data_item_metadata.py
--rw-r--r--   0        0        0      186 2023-10-11 11:52:15.343802 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200_status.py
--rw-r--r--   0        0        0     2863 2023-10-11 11:52:20.525666 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_400.py
--rw-r--r--   0        0        0     2022 2023-10-11 11:52:20.549675 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_400_data.py
--rw-r--r--   0        0        0      265 2023-10-11 11:52:15.003679 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_400_data_code.py
--rw-r--r--   0        0        0      186 2023-10-11 11:52:15.019685 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_400_status.py
--rw-r--r--   0        0        0     2863 2023-10-11 11:52:20.557678 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_401.py
--rw-r--r--   0        0        0     2017 2023-10-11 11:52:20.589689 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_401_data.py
--rw-r--r--   0        0        0      265 2023-10-11 11:52:14.839619 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_401_data_code.py
--rw-r--r--   0        0        0      186 2023-10-11 11:52:15.115719 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_401_status.py
--rw-r--r--   0        0        0     2863 2023-10-11 11:52:20.605695 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_404.py
--rw-r--r--   0        0        0     2193 2023-10-11 11:52:20.661715 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_404_data.py
--rw-r--r--   0        0        0      265 2023-10-11 11:52:15.539873 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_404_data_code.py
--rw-r--r--   0        0        0      283 2023-10-11 11:52:15.371812 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_404_data_message.py
--rw-r--r--   0        0        0      186 2023-10-11 11:52:15.515864 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_404_status.py
--rw-r--r--   0        0        0     2863 2023-10-11 11:52:20.625702 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_500.py
--rw-r--r--   0        0        0     2000 2023-10-11 11:52:20.653712 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_500_data.py
--rw-r--r--   0        0        0      265 2023-10-11 11:52:14.987673 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_500_data_code.py
--rw-r--r--   0        0        0      186 2023-10-11 11:52:14.683562 customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_500_status.py
--rw-r--r--   0        0        0     4611 2023-10-11 11:52:20.689725 customgpt_client-1.2.1/customgpt_client/models/open_graph_cache.py
--rw-r--r--   0        0        0     7615 2023-10-11 11:52:20.765752 customgpt_client-1.2.1/customgpt_client/models/page.py
--rw-r--r--   0        0        0      217 2023-10-11 11:52:15.519866 customgpt_client-1.2.1/customgpt_client/models/page_crawl_status.py
--rw-r--r--   0        0        0      217 2023-10-11 11:52:14.223395 customgpt_client-1.2.1/customgpt_client/models/page_index_status.py
--rw-r--r--   0        0        0     2564 2023-10-11 11:52:20.677720 customgpt_client-1.2.1/customgpt_client/models/page_metadata.py
--rw-r--r--   0        0        0     2793 2023-10-11 11:52:20.689725 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_400.py
--rw-r--r--   0        0        0     1992 2023-10-11 11:52:20.669717 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_400_data.py
--rw-r--r--   0        0        0      260 2023-10-11 11:52:15.567883 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_400_data_code.py
--rw-r--r--   0        0        0      181 2023-10-11 11:52:15.023686 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_400_status.py
--rw-r--r--   0        0        0     2793 2023-10-11 11:52:20.709732 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_401.py
--rw-r--r--   0        0        0     1987 2023-10-11 11:52:20.805766 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_401_data.py
--rw-r--r--   0        0        0      260 2023-10-11 11:52:14.399459 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_401_data_code.py
--rw-r--r--   0        0        0      181 2023-10-11 11:52:15.247767 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_401_status.py
--rw-r--r--   0        0        0     2793 2023-10-11 11:52:20.757749 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_404.py
--rw-r--r--   0        0        0     2152 2023-10-11 11:52:20.737742 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_404_data.py
--rw-r--r--   0        0        0      260 2023-10-11 11:52:14.311427 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_404_data_code.py
--rw-r--r--   0        0        0      260 2023-10-11 11:52:14.443475 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_404_data_message.py
--rw-r--r--   0        0        0      181 2023-10-11 11:52:15.363809 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_404_status.py
--rw-r--r--   0        0        0     2793 2023-10-11 11:52:20.785759 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_500.py
--rw-r--r--   0        0        0     1970 2023-10-11 11:52:20.797763 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_500_data.py
--rw-r--r--   0        0        0      260 2023-10-11 11:52:15.043693 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_500_data_code.py
--rw-r--r--   0        0        0      181 2023-10-11 11:52:14.903642 customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_500_status.py
--rw-r--r--   0        0        0     7543 2023-10-11 11:52:21.225916 customgpt_client-1.2.1/customgpt_client/models/project.py
--rw-r--r--   0        0        0     3238 2023-10-11 11:52:20.809767 customgpt_client-1.2.1/customgpt_client/models/project_plugin.py
--rw-r--r--   0        0        0    12315 2023-10-11 11:52:21.081864 customgpt_client-1.2.1/customgpt_client/models/project_settings.py
--rw-r--r--   0        0        0      191 2023-10-11 11:52:15.411827 customgpt_client-1.2.1/customgpt_client/models/project_settings_citations_view_type.py
--rw-r--r--   0        0        0      228 2023-10-11 11:52:15.571885 customgpt_client-1.2.1/customgpt_client/models/project_settings_response_source.py
--rw-r--r--   0        0        0     5009 2023-10-11 11:52:20.933812 customgpt_client-1.2.1/customgpt_client/models/project_source.py
--rw-r--r--   0        0        0     2961 2023-10-11 11:52:20.861786 customgpt_client-1.2.1/customgpt_client/models/project_source_settings.py
--rw-r--r--   0        0        0      168 2023-10-11 11:52:15.075705 customgpt_client-1.2.1/customgpt_client/models/project_source_type.py
--rw-r--r--   0        0        0      156 2023-10-11 11:52:14.451478 customgpt_client-1.2.1/customgpt_client/models/project_type.py
--rw-r--r--   0        0        0     6027 2023-10-11 11:52:21.241921 customgpt_client-1.2.1/customgpt_client/models/prompt_history.py
--rw-r--r--   0        0        0     2945 2023-10-11 11:52:21.145887 customgpt_client-1.2.1/customgpt_client/models/prompt_history_metadata.py
--rw-r--r--   0        0        0     2453 2023-10-11 11:52:20.921807 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_200.py
--rw-r--r--   0        0        0     1613 2023-10-11 11:52:21.041850 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_200_data.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:15.039692 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_200_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:21.217913 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_400.py
--rw-r--r--   0        0        0     1968 2023-10-11 11:52:21.017842 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_400_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:14.867629 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_400_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:15.171740 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_400_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:21.053854 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_401.py
--rw-r--r--   0        0        0     1963 2023-10-11 11:52:21.105873 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_401_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:14.667556 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_401_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:15.131725 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_401_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:21.165894 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_403.py
--rw-r--r--   0        0        0     2144 2023-10-11 11:52:21.285937 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_403_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:15.255770 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_403_data_code.py
--rw-r--r--   0        0        0      228 2023-10-11 11:52:14.827615 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_403_data_message.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.615538 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_403_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:21.205908 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_500.py
--rw-r--r--   0        0        0     1946 2023-10-11 11:52:21.189903 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_500_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:14.771594 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_500_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.543511 customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_500_status.py
--rw-r--r--   0        0        0     2296 2023-10-11 11:52:21.249924 customgpt_client-1.2.1/customgpt_client/models/send_message_json_body.py
--rw-r--r--   0        0        0     2453 2023-10-11 11:52:21.357962 customgpt_client-1.2.1/customgpt_client/models/send_message_response_200.py
--rw-r--r--   0        0        0     6211 2023-10-11 11:52:21.429988 customgpt_client-1.2.1/customgpt_client/models/send_message_response_200_data.py
--rw-r--r--   0        0        0     3019 2023-10-11 11:52:21.357962 customgpt_client-1.2.1/customgpt_client/models/send_message_response_200_data_metadata.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.819612 customgpt_client-1.2.1/customgpt_client/models/send_message_response_200_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:21.397977 customgpt_client-1.2.1/customgpt_client/models/send_message_response_400.py
--rw-r--r--   0        0        0     1968 2023-10-11 11:52:21.397977 customgpt_client-1.2.1/customgpt_client/models/send_message_response_400_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:14.799605 customgpt_client-1.2.1/customgpt_client/models/send_message_response_400_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:15.363809 customgpt_client-1.2.1/customgpt_client/models/send_message_response_400_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:21.409981 customgpt_client-1.2.1/customgpt_client/models/send_message_response_401.py
--rw-r--r--   0        0        0     1963 2023-10-11 11:52:21.349960 customgpt_client-1.2.1/customgpt_client/models/send_message_response_401_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:14.791602 customgpt_client-1.2.1/customgpt_client/models/send_message_response_401_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:15.523867 customgpt_client-1.2.1/customgpt_client/models/send_message_response_401_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:21.470002 customgpt_client-1.2.1/customgpt_client/models/send_message_response_404.py
--rw-r--r--   0        0        0     2130 2023-10-11 11:52:21.421985 customgpt_client-1.2.1/customgpt_client/models/send_message_response_404_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:15.131725 customgpt_client-1.2.1/customgpt_client/models/send_message_response_404_data_code.py
--rw-r--r--   0        0        0      274 2023-10-11 11:52:14.619539 customgpt_client-1.2.1/customgpt_client/models/send_message_response_404_data_message.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.431470 customgpt_client-1.2.1/customgpt_client/models/send_message_response_404_status.py
--rw-r--r--   0        0        0     2737 2023-10-11 11:52:21.518019 customgpt_client-1.2.1/customgpt_client/models/send_message_response_500.py
--rw-r--r--   0        0        0     1946 2023-10-11 11:52:21.494011 customgpt_client-1.2.1/customgpt_client/models/send_message_response_500_data.py
--rw-r--r--   0        0        0      256 2023-10-11 11:52:15.527869 customgpt_client-1.2.1/customgpt_client/models/send_message_response_500_data_code.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.579524 customgpt_client-1.2.1/customgpt_client/models/send_message_response_500_status.py
--rw-r--r--   0        0        0     2467 2023-10-11 11:52:21.574039 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_200.py
--rw-r--r--   0        0        0     3698 2023-10-11 11:52:21.494011 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_200_data.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.675559 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_200_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:21.662071 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_400.py
--rw-r--r--   0        0        0     1974 2023-10-11 11:52:21.482007 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_400_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.659553 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_400_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.627542 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_400_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:21.530024 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_401.py
--rw-r--r--   0        0        0     1969 2023-10-11 11:52:21.534025 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_401_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.531507 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_401_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.679561 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_401_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:21.746100 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_404.py
--rw-r--r--   0        0        0     2137 2023-10-11 11:52:21.646065 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_404_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.475487 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_404_data_code.py
--rw-r--r--   0        0        0      275 2023-10-11 11:52:14.467484 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_404_data_message.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.195385 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_404_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:21.722092 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_500.py
--rw-r--r--   0        0        0     1952 2023-10-11 11:52:21.670073 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_500_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.431470 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_500_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.359444 customgpt_client-1.2.1/customgpt_client/models/stats_project_response_500_status.py
--rw-r--r--   0        0        0     1569 2023-10-11 11:52:21.602049 customgpt_client-1.2.1/customgpt_client/models/update_conversation_json_body.py
--rw-r--r--   0        0        0     2551 2023-10-11 11:52:21.642063 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_200.py
--rw-r--r--   0        0        0     5103 2023-10-11 11:52:21.930166 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_200_data.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.231398 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_200_status.py
--rw-r--r--   0        0        0     2835 2023-10-11 11:52:21.702085 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_400.py
--rw-r--r--   0        0        0     2010 2023-10-11 11:52:21.710088 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_400_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:15.547876 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_400_data_code.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.903642 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_400_status.py
--rw-r--r--   0        0        0     2835 2023-10-11 11:52:21.754103 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_401.py
--rw-r--r--   0        0        0     2005 2023-10-11 11:52:21.722092 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_401_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.811609 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_401_data_code.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.403460 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_401_status.py
--rw-r--r--   0        0        0     2835 2023-10-11 11:52:21.890152 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_404.py
--rw-r--r--   0        0        0     2179 2023-10-11 11:52:21.786115 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_404_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.579524 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_404_data_code.py
--rw-r--r--   0        0        0      281 2023-10-11 11:52:14.647549 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_404_data_message.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:15.131725 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_404_status.py
--rw-r--r--   0        0        0     2835 2023-10-11 11:52:21.938169 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_500.py
--rw-r--r--   0        0        0     1988 2023-10-11 11:52:21.854139 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_500_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:15.435835 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_500_data_code.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:15.191747 customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_500_status.py
--rw-r--r--   0        0        0     2603 2023-10-11 11:52:21.814124 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_json_body.py
--rw-r--r--   0        0        0     2556 2023-10-11 11:52:21.918161 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_200.py
--rw-r--r--   0        0        0     2681 2023-10-11 11:52:21.850137 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_200_data.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:15.499859 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_200_status.py
--rw-r--r--   0        0        0     2840 2023-10-11 11:52:21.910159 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_400.py
--rw-r--r--   0        0        0     2013 2023-10-11 11:52:21.898154 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_400_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.467484 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_400_data_code.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:15.551878 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_400_status.py
--rw-r--r--   0        0        0     2840 2023-10-11 11:52:21.970180 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_401.py
--rw-r--r--   0        0        0     2008 2023-10-11 11:52:21.966179 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_401_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.431470 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_401_data_code.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:15.591892 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_401_status.py
--rw-r--r--   0        0        0     2840 2023-10-11 11:52:22.006193 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_404.py
--rw-r--r--   0        0        0     2176 2023-10-11 11:52:22.014196 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_404_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.595530 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_404_data_code.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:14.467484 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_404_data_message.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.219393 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_404_status.py
--rw-r--r--   0        0        0     2840 2023-10-11 11:52:22.038204 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_500.py
--rw-r--r--   0        0        0     1991 2023-10-11 11:52:22.066214 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_500_data.py
--rw-r--r--   0        0        0      263 2023-10-11 11:52:15.303788 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_500_data_code.py
--rw-r--r--   0        0        0      184 2023-10-11 11:52:14.259408 customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_500_status.py
--rw-r--r--   0        0        0     2992 2023-10-11 11:52:22.154245 customgpt_client-1.2.1/customgpt_client/models/update_plugin_json_body.py
--rw-r--r--   0        0        0     2467 2023-10-11 11:52:22.110230 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_200.py
--rw-r--r--   0        0        0     3317 2023-10-11 11:52:22.158247 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_200_data.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.711573 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_200_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:22.130237 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_400.py
--rw-r--r--   0        0        0     1974 2023-10-11 11:52:22.082220 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_400_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.507498 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_400_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:15.395821 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_400_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:22.210265 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_401.py
--rw-r--r--   0        0        0     1969 2023-10-11 11:52:22.130237 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_401_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.651551 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_401_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.667556 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_401_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:22.214266 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_404.py
--rw-r--r--   0        0        0     2151 2023-10-11 11:52:22.174252 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_404_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:14.691565 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_404_data_code.py
--rw-r--r--   0        0        0      405 2023-10-11 11:52:14.651551 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_404_data_message.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.215392 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_404_status.py
--rw-r--r--   0        0        0     2751 2023-10-11 11:52:22.250279 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_500.py
--rw-r--r--   0        0        0     1952 2023-10-11 11:52:22.246278 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_500_data.py
--rw-r--r--   0        0        0      257 2023-10-11 11:52:15.487854 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_500_data_code.py
--rw-r--r--   0        0        0      178 2023-10-11 11:52:14.707571 customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_500_status.py
--rw-r--r--   0        0        0     4967 2023-10-11 11:52:22.410336 customgpt_client-1.2.1/customgpt_client/models/update_project_multipart_data.py
--rw-r--r--   0        0        0     2481 2023-10-11 11:52:22.298296 customgpt_client-1.2.1/customgpt_client/models/update_project_response_200.py
--rw-r--r--   0        0        0     7714 2023-10-11 11:52:22.374323 customgpt_client-1.2.1/customgpt_client/models/update_project_response_200_data.py
--rw-r--r--   0        0        0      177 2023-10-11 11:52:14.991674 customgpt_client-1.2.1/customgpt_client/models/update_project_response_200_data_type.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:15.271776 customgpt_client-1.2.1/customgpt_client/models/update_project_response_200_status.py
--rw-r--r--   0        0        0     2765 2023-10-11 11:52:22.278289 customgpt_client-1.2.1/customgpt_client/models/update_project_response_400.py
--rw-r--r--   0        0        0     1980 2023-10-11 11:52:22.354316 customgpt_client-1.2.1/customgpt_client/models/update_project_response_400_data.py
--rw-r--r--   0        0        0      258 2023-10-11 11:52:15.091711 customgpt_client-1.2.1/customgpt_client/models/update_project_response_400_data_code.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:14.447476 customgpt_client-1.2.1/customgpt_client/models/update_project_response_400_status.py
--rw-r--r--   0        0        0     2765 2023-10-11 11:52:22.386327 customgpt_client-1.2.1/customgpt_client/models/update_project_response_401.py
--rw-r--r--   0        0        0     1975 2023-10-11 11:52:22.410336 customgpt_client-1.2.1/customgpt_client/models/update_project_response_401_data.py
--rw-r--r--   0        0        0      258 2023-10-11 11:52:14.787600 customgpt_client-1.2.1/customgpt_client/models/update_project_response_401_data_code.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:14.547513 customgpt_client-1.2.1/customgpt_client/models/update_project_response_401_status.py
--rw-r--r--   0        0        0     2765 2023-10-11 11:52:22.438346 customgpt_client-1.2.1/customgpt_client/models/update_project_response_404.py
--rw-r--r--   0        0        0     2144 2023-10-11 11:52:22.358317 customgpt_client-1.2.1/customgpt_client/models/update_project_response_404_data.py
--rw-r--r--   0        0        0      258 2023-10-11 11:52:14.719575 customgpt_client-1.2.1/customgpt_client/models/update_project_response_404_data_code.py
--rw-r--r--   0        0        0      276 2023-10-11 11:52:15.091711 customgpt_client-1.2.1/customgpt_client/models/update_project_response_404_data_message.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:14.823613 customgpt_client-1.2.1/customgpt_client/models/update_project_response_404_status.py
--rw-r--r--   0        0        0     2765 2023-10-11 11:52:22.450350 customgpt_client-1.2.1/customgpt_client/models/update_project_response_500.py
--rw-r--r--   0        0        0     1958 2023-10-11 11:52:22.498367 customgpt_client-1.2.1/customgpt_client/models/update_project_response_500_data.py
--rw-r--r--   0        0        0      258 2023-10-11 11:52:14.207389 customgpt_client-1.2.1/customgpt_client/models/update_project_response_500_data_code.py
--rw-r--r--   0        0        0      179 2023-10-11 11:52:14.771594 customgpt_client-1.2.1/customgpt_client/models/update_project_response_500_status.py
--rw-r--r--   0        0        0    19231 2023-10-11 11:52:22.734451 customgpt_client-1.2.1/customgpt_client/models/update_settings_multipart_data.py
--rw-r--r--   0        0        0      203 2023-10-11 11:52:14.727578 customgpt_client-1.2.1/customgpt_client/models/update_settings_multipart_data_citations_view_type.py
--rw-r--r--   0        0        0     2495 2023-10-11 11:52:22.466356 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_200.py
--rw-r--r--   0        0        0     1621 2023-10-11 11:52:22.454352 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_200_data.py
--rw-r--r--   0        0        0      180 2023-10-11 11:52:15.023686 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_200_status.py
--rw-r--r--   0        0        0     2779 2023-10-11 11:52:22.494366 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_400.py
--rw-r--r--   0        0        0     2183 2023-10-11 11:52:22.514373 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_400_data.py
--rw-r--r--   0        0        0      259 2023-10-11 11:52:14.619539 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_400_data_code.py
--rw-r--r--   0        0        0      416 2023-10-11 11:52:15.123722 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_400_data_message.py
--rw-r--r--   0        0        0      180 2023-10-11 11:52:15.523867 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_400_status.py
--rw-r--r--   0        0        0     2779 2023-10-11 11:52:22.562390 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_401.py
--rw-r--r--   0        0        0     1981 2023-10-11 11:52:22.530378 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_401_data.py
--rw-r--r--   0        0        0      259 2023-10-11 11:52:14.471485 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_401_data_code.py
--rw-r--r--   0        0        0      180 2023-10-11 11:52:14.523504 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_401_status.py
--rw-r--r--   0        0        0     2779 2023-10-11 11:52:22.634415 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_500.py
--rw-r--r--   0        0        0     1964 2023-10-11 11:52:22.526377 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_500_data.py
--rw-r--r--   0        0        0      259 2023-10-11 11:52:14.447476 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_500_data_code.py
--rw-r--r--   0        0        0      180 2023-10-11 11:52:15.215756 customgpt_client-1.2.1/customgpt_client/models/update_settings_response_500_status.py
--rw-r--r--   0        0        0     2991 2023-10-11 11:52:22.590400 customgpt_client-1.2.1/customgpt_client/models/update_user_multipart_data.py
--rw-r--r--   0        0        0     2439 2023-10-11 11:52:22.626412 customgpt_client-1.2.1/customgpt_client/models/update_user_response_200.py
--rw-r--r--   0        0        0     3887 2023-10-11 11:52:22.682432 customgpt_client-1.2.1/customgpt_client/models/update_user_response_200_data.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:14.399459 customgpt_client-1.2.1/customgpt_client/models/update_user_response_200_status.py
--rw-r--r--   0        0        0     2723 2023-10-11 11:52:22.614408 customgpt_client-1.2.1/customgpt_client/models/update_user_response_401.py
--rw-r--r--   0        0        0     1957 2023-10-11 11:52:22.594401 customgpt_client-1.2.1/customgpt_client/models/update_user_response_401_data.py
--rw-r--r--   0        0        0      255 2023-10-11 11:52:14.655552 customgpt_client-1.2.1/customgpt_client/models/update_user_response_401_data_code.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:14.223395 customgpt_client-1.2.1/customgpt_client/models/update_user_response_401_status.py
--rw-r--r--   0        0        0     2723 2023-10-11 11:52:22.646420 customgpt_client-1.2.1/customgpt_client/models/update_user_response_500.py
--rw-r--r--   0        0        0     1940 2023-10-11 11:52:22.650421 customgpt_client-1.2.1/customgpt_client/models/update_user_response_500_data.py
--rw-r--r--   0        0        0      255 2023-10-11 11:52:14.491492 customgpt_client-1.2.1/customgpt_client/models/update_user_response_500_data_code.py
--rw-r--r--   0        0        0      176 2023-10-11 11:52:14.295421 customgpt_client-1.2.1/customgpt_client/models/update_user_response_500_status.py
--rw-r--r--   0        0        0     3770 2023-10-11 11:52:22.714444 customgpt_client-1.2.1/customgpt_client/models/user.py
--rw-r--r--   0        0        0       25 2023-10-11 11:52:11.098250 customgpt_client-1.2.1/customgpt_client/py.typed
--rw-r--r--   0        0        0      993 2023-10-11 11:52:22.650421 customgpt_client-1.2.1/customgpt_client/types.py
--rw-r--r--   0        0        0      691 2023-10-11 12:07:46.245168 customgpt_client-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 customgpt_client-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      676 2024-05-23 17:44:52.929065 customgpt_client-1.2.2/README.md
+-rw-r--r--   0        0        0      105 2024-05-14 19:49:04.613524 customgpt_client-1.2.2/customgpt_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-05-14 19:49:04.613524 customgpt_client-1.2.2/customgpt_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:49:04.613524 customgpt_client-1.2.2/customgpt_client/api/citations/__init__.py
+-rw-r--r--   0        0        0     6731 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/citations/get_citation.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/conversations/__init__.py
+-rw-r--r--   0        0        0     9063 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/conversations/create_conversation.py
+-rw-r--r--   0        0        0     8391 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/conversations/delete_conversation.py
+-rw-r--r--   0        0        0     9618 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/conversations/get_conversations.py
+-rw-r--r--   0        0        0    10956 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/conversations/messages_conversation.py
+-rw-r--r--   0        0        0    10999 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/conversations/send_message.py
+-rw-r--r--   0        0        0     8828 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/conversations/update_conversation.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/page_metadata/__init__.py
+-rw-r--r--   0        0        0     6025 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/page_metadata/get_page_metadata.py
+-rw-r--r--   0        0        0     7470 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/page_metadata/update_page_metadata.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/pages/__init__.py
+-rw-r--r--   0        0        0     7473 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/pages/delete_page.py
+-rw-r--r--   0        0        0     9524 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/pages/get_pages.py
+-rw-r--r--   0        0        0     5080 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/pages/preview_citation.py
+-rw-r--r--   0        0        0     6711 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/pages/reindex_page.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/project_plugins/__init__.py
+-rw-r--r--   0        0        0     6990 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/project_plugins/create_plugin.py
+-rw-r--r--   0        0        0     5730 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/project_plugins/get_plugin.py
+-rw-r--r--   0        0        0     6774 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/project_plugins/update_plugin.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/project_settings/__init__.py
+-rw-r--r--   0        0        0     7057 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/project_settings/get_settings.py
+-rw-r--r--   0        0        0     7253 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/project_settings/update_settings.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:49:04.617524 customgpt_client-1.2.2/customgpt_client/api/projects/__init__.py
+-rw-r--r--   0        0        0     7954 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/projects/create_project.py
+-rw-r--r--   0        0        0     6966 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/projects/delete_project.py
+-rw-r--r--   0        0        0     7353 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/projects/get_project.py
+-rw-r--r--   0        0        0     9287 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/projects/list_projects.py
+-rw-r--r--   0        0        0     7127 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/projects/stats_project.py
+-rw-r--r--   0        0        0     7911 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/projects/update_project.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/sources/__init__.py
+-rw-r--r--   0        0        0     8120 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/sources/create_source.py
+-rw-r--r--   0        0        0     6167 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/sources/delete_source.py
+-rw-r--r--   0        0        0     6330 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/sources/list_sources.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/users/__init__.py
+-rw-r--r--   0        0        0     4709 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/users/get_user.py
+-rw-r--r--   0        0        0     5378 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/api/users/update_user.py
+-rw-r--r--   0        0        0    19381 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/client.py
+-rw-r--r--   0        0        0      470 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/errors.py
+-rw-r--r--   0        0        0    68823 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/models/__init__.py
+-rw-r--r--   0        0        0     4857 2024-05-14 19:49:04.621524 customgpt_client-1.2.2/customgpt_client/models/conversation.py
+-rw-r--r--   0        0        0     1545 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_json_body.py
+-rw-r--r--   0        0        0     2551 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_201.py
+-rw-r--r--   0        0        0     5103 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_201_data.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_201_status.py
+-rw-r--r--   0        0        0     2835 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_400.py
+-rw-r--r--   0        0        0     2010 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_400_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_400_data_code.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_400_status.py
+-rw-r--r--   0        0        0     2835 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_401.py
+-rw-r--r--   0        0        0     2005 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_401_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_401_data_code.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_401_status.py
+-rw-r--r--   0        0        0     2835 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_404.py
+-rw-r--r--   0        0        0     2179 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_404_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_404_data_code.py
+-rw-r--r--   0        0        0      281 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_404_data_message.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_404_status.py
+-rw-r--r--   0        0        0     2835 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_500.py
+-rw-r--r--   0        0        0     1988 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_500_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_500_data_code.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_500_status.py
+-rw-r--r--   0        0        0     2992 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_json_body.py
+-rw-r--r--   0        0        0     2467 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_201.py
+-rw-r--r--   0        0        0     3317 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_201_data.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_201_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_400.py
+-rw-r--r--   0        0        0     1974 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_400_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_400_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_400_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_401.py
+-rw-r--r--   0        0        0     1969 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_401_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_401_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_401_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_404.py
+-rw-r--r--   0        0        0     2137 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_404_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_404_data_code.py
+-rw-r--r--   0        0        0      275 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_404_data_message.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_404_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_500.py
+-rw-r--r--   0        0        0     1952 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_500_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_500_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_500_status.py
+-rw-r--r--   0        0        0     4387 2024-05-14 19:49:04.625525 customgpt_client-1.2.2/customgpt_client/models/create_project_multipart_data.py
+-rw-r--r--   0        0        0     2481 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_201.py
+-rw-r--r--   0        0        0     7714 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_201_data.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_201_data_type.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_201_status.py
+-rw-r--r--   0        0        0     2765 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_400.py
+-rw-r--r--   0        0        0     2144 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_400_data.py
+-rw-r--r--   0        0        0      258 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_400_data_code.py
+-rw-r--r--   0        0        0      362 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_400_data_message.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_400_status.py
+-rw-r--r--   0        0        0     2765 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_401.py
+-rw-r--r--   0        0        0     1975 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_401_data.py
+-rw-r--r--   0        0        0      258 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_401_data_code.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_401_status.py
+-rw-r--r--   0        0        0     2765 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_500.py
+-rw-r--r--   0        0        0     1958 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_500_data.py
+-rw-r--r--   0        0        0      258 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_500_data_code.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_project_response_500_status.py
+-rw-r--r--   0        0        0     3757 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_multipart_data.py
+-rw-r--r--   0        0        0     2467 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_201.py
+-rw-r--r--   0        0        0     5456 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_201_data.py
+-rw-r--r--   0        0        0     8038 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_201_data_pages_item.py
+-rw-r--r--   0        0        0      249 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_201_data_pages_item_crawl_status.py
+-rw-r--r--   0        0        0      249 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_201_data_pages_item_index_status.py
+-rw-r--r--   0        0        0     3040 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_201_data_settings.py
+-rw-r--r--   0        0        0      182 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_201_data_type.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_201_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_400.py
+-rw-r--r--   0        0        0     2111 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_400_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_400_data_code.py
+-rw-r--r--   0        0        0      399 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_400_data_message.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_400_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_401.py
+-rw-r--r--   0        0        0     1969 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_401_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_401_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_401_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_404.py
+-rw-r--r--   0        0        0     2137 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_404_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_404_data_code.py
+-rw-r--r--   0        0        0      275 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_404_data_message.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_404_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_500.py
+-rw-r--r--   0        0        0     1952 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_500_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_500_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/create_source_response_500_status.py
+-rw-r--r--   0        0        0     2551 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_200.py
+-rw-r--r--   0        0        0     1641 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_200_data.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_200_status.py
+-rw-r--r--   0        0        0     2835 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_400.py
+-rw-r--r--   0        0        0     2010 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_400_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_400_data_code.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_400_status.py
+-rw-r--r--   0        0        0     2835 2024-05-14 19:49:04.629525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_401.py
+-rw-r--r--   0        0        0     2005 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_401_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_401_data_code.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_401_status.py
+-rw-r--r--   0        0        0     2835 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_404.py
+-rw-r--r--   0        0        0     2179 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_404_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_404_data_code.py
+-rw-r--r--   0        0        0      281 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_404_data_message.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_404_status.py
+-rw-r--r--   0        0        0     2835 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_500.py
+-rw-r--r--   0        0        0     1988 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_500_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_500_data_code.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_500_status.py
+-rw-r--r--   0        0        0     2439 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_200.py
+-rw-r--r--   0        0        0     1601 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_200_data.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_200_status.py
+-rw-r--r--   0        0        0     2723 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_400.py
+-rw-r--r--   0        0        0     1962 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_400_data.py
+-rw-r--r--   0        0        0      255 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_400_data_code.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_400_status.py
+-rw-r--r--   0        0        0     2723 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_401.py
+-rw-r--r--   0        0        0     1957 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_401_data.py
+-rw-r--r--   0        0        0      255 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_401_data_code.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_401_status.py
+-rw-r--r--   0        0        0     2723 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_404.py
+-rw-r--r--   0        0        0     2123 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_404_data.py
+-rw-r--r--   0        0        0      255 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_404_data_code.py
+-rw-r--r--   0        0        0      273 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_404_data_message.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_404_status.py
+-rw-r--r--   0        0        0     2723 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_500.py
+-rw-r--r--   0        0        0     1940 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_500_data.py
+-rw-r--r--   0        0        0      255 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_500_data_code.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_page_response_500_status.py
+-rw-r--r--   0        0        0     2481 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_200.py
+-rw-r--r--   0        0        0     1616 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_200_data.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_200_status.py
+-rw-r--r--   0        0        0     2765 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_400.py
+-rw-r--r--   0        0        0     1980 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_400_data.py
+-rw-r--r--   0        0        0      258 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_400_data_code.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_400_status.py
+-rw-r--r--   0        0        0     2765 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_401.py
+-rw-r--r--   0        0        0     1975 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_401_data.py
+-rw-r--r--   0        0        0      258 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_401_data_code.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_401_status.py
+-rw-r--r--   0        0        0     2765 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_404.py
+-rw-r--r--   0        0        0     2144 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_404_data.py
+-rw-r--r--   0        0        0      258 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_404_data_code.py
+-rw-r--r--   0        0        0      276 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_404_data_message.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_404_status.py
+-rw-r--r--   0        0        0     2765 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_500.py
+-rw-r--r--   0        0        0     1958 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_500_data.py
+-rw-r--r--   0        0        0      258 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_500_data_code.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.633525 customgpt_client-1.2.2/customgpt_client/models/delete_project_response_500_status.py
+-rw-r--r--   0        0        0     2467 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_200.py
+-rw-r--r--   0        0        0     1618 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_200_data.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_200_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_400.py
+-rw-r--r--   0        0        0     1974 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_400_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_400_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_400_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_401.py
+-rw-r--r--   0        0        0     1969 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_401_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_401_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_401_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_404.py
+-rw-r--r--   0        0        0     2137 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_404_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_404_data_code.py
+-rw-r--r--   0        0        0      275 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_404_data_message.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_404_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_500.py
+-rw-r--r--   0        0        0     1952 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_500_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_500_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/delete_source_response_500_status.py
+-rw-r--r--   0        0        0     2453 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_200.py
+-rw-r--r--   0        0        0     4330 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_200_data.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_200_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_400.py
+-rw-r--r--   0        0        0     1968 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_400_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_400_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_400_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_401.py
+-rw-r--r--   0        0        0     1963 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_401_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_401_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_401_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_404.py
+-rw-r--r--   0        0        0     2130 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_404_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_404_data_code.py
+-rw-r--r--   0        0        0      274 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_404_data_message.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_citation_response_404_status.py
+-rw-r--r--   0        0        0      160 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_order.py
+-rw-r--r--   0        0        0     2523 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_200.py
+-rw-r--r--   0        0        0     6048 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_200_data.py
+-rw-r--r--   0        0        0     5139 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_200_data_data_item.py
+-rw-r--r--   0        0        0      182 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_200_status.py
+-rw-r--r--   0        0        0     2807 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_400.py
+-rw-r--r--   0        0        0     1998 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_400_data.py
+-rw-r--r--   0        0        0      261 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_400_data_code.py
+-rw-r--r--   0        0        0      182 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_400_status.py
+-rw-r--r--   0        0        0     2807 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_401.py
+-rw-r--r--   0        0        0     1993 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_401_data.py
+-rw-r--r--   0        0        0      261 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_401_data_code.py
+-rw-r--r--   0        0        0      182 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_401_status.py
+-rw-r--r--   0        0        0     2807 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_404.py
+-rw-r--r--   0        0        0     2165 2024-05-14 19:49:04.637525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_404_data.py
+-rw-r--r--   0        0        0      261 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_404_data_code.py
+-rw-r--r--   0        0        0      279 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_404_data_message.py
+-rw-r--r--   0        0        0      182 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_404_status.py
+-rw-r--r--   0        0        0     2807 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_500.py
+-rw-r--r--   0        0        0     1976 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_500_data.py
+-rw-r--r--   0        0        0      261 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_500_data_code.py
+-rw-r--r--   0        0        0      182 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_500_status.py
+-rw-r--r--   0        0        0      207 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_conversations_user_filter.py
+-rw-r--r--   0        0        0     2514 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_200.py
+-rw-r--r--   0        0        0     2666 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_200_data.py
+-rw-r--r--   0        0        0      181 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_200_status.py
+-rw-r--r--   0        0        0     2798 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_400.py
+-rw-r--r--   0        0        0     1990 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_400_data.py
+-rw-r--r--   0        0        0      260 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_400_data_code.py
+-rw-r--r--   0        0        0      181 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_400_status.py
+-rw-r--r--   0        0        0     2798 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_401.py
+-rw-r--r--   0        0        0     1990 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_401_data.py
+-rw-r--r--   0        0        0      260 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_401_data_code.py
+-rw-r--r--   0        0        0      181 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_401_status.py
+-rw-r--r--   0        0        0     2798 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_404.py
+-rw-r--r--   0        0        0     2155 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_404_data.py
+-rw-r--r--   0        0        0      260 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_404_data_code.py
+-rw-r--r--   0        0        0      260 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_404_data_message.py
+-rw-r--r--   0        0        0      181 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_404_status.py
+-rw-r--r--   0        0        0      152 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_order.py
+-rw-r--r--   0        0        0     2411 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200.py
+-rw-r--r--   0        0        0     2919 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200_data.py
+-rw-r--r--   0        0        0     6017 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200_data_pages.py
+-rw-r--r--   0        0        0     8041 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200_data_pages_data_item.py
+-rw-r--r--   0        0        0      249 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200_data_pages_data_item_crawl_status.py
+-rw-r--r--   0        0        0      249 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200_data_pages_data_item_index_status.py
+-rw-r--r--   0        0        0     7731 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200_data_project.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200_data_project_type.py
+-rw-r--r--   0        0        0      174 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200_status.py
+-rw-r--r--   0        0        0     2695 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_400.py
+-rw-r--r--   0        0        0     1950 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_400_data.py
+-rw-r--r--   0        0        0      253 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_400_data_code.py
+-rw-r--r--   0        0        0      174 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_400_status.py
+-rw-r--r--   0        0        0     2695 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_401.py
+-rw-r--r--   0        0        0     1945 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_401_data.py
+-rw-r--r--   0        0        0      253 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_401_data_code.py
+-rw-r--r--   0        0        0      174 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_401_status.py
+-rw-r--r--   0        0        0     2695 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_404.py
+-rw-r--r--   0        0        0     2097 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_404_data.py
+-rw-r--r--   0        0        0      253 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_404_data_code.py
+-rw-r--r--   0        0        0      271 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_404_data_message.py
+-rw-r--r--   0        0        0      174 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_404_status.py
+-rw-r--r--   0        0        0     2695 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_500.py
+-rw-r--r--   0        0        0     1928 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_500_data.py
+-rw-r--r--   0        0        0      253 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_500_data_code.py
+-rw-r--r--   0        0        0      174 2024-05-14 19:49:04.641525 customgpt_client-1.2.2/customgpt_client/models/get_pages_response_500_status.py
+-rw-r--r--   0        0        0     2425 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_200.py
+-rw-r--r--   0        0        0     3302 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_200_data.py
+-rw-r--r--   0        0        0      175 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_200_status.py
+-rw-r--r--   0        0        0     2709 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_400.py
+-rw-r--r--   0        0        0     1956 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_400_data.py
+-rw-r--r--   0        0        0      254 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_400_data_code.py
+-rw-r--r--   0        0        0      175 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_400_status.py
+-rw-r--r--   0        0        0     2709 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_401.py
+-rw-r--r--   0        0        0     1951 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_401_data.py
+-rw-r--r--   0        0        0      254 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_401_data_code.py
+-rw-r--r--   0        0        0      175 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_401_status.py
+-rw-r--r--   0        0        0     2709 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_404.py
+-rw-r--r--   0        0        0     2130 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_404_data.py
+-rw-r--r--   0        0        0      254 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_404_data_code.py
+-rw-r--r--   0        0        0      402 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_404_data_message.py
+-rw-r--r--   0        0        0      175 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_404_status.py
+-rw-r--r--   0        0        0     2709 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_500.py
+-rw-r--r--   0        0        0     1934 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_500_data.py
+-rw-r--r--   0        0        0      254 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_500_data_code.py
+-rw-r--r--   0        0        0      175 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_500_status.py
+-rw-r--r--   0        0        0     2439 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_200.py
+-rw-r--r--   0        0        0     7693 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_200_data.py
+-rw-r--r--   0        0        0      174 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_200_data_type.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_200_status.py
+-rw-r--r--   0        0        0     2723 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_400.py
+-rw-r--r--   0        0        0     1962 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_400_data.py
+-rw-r--r--   0        0        0      255 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_400_data_code.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_400_status.py
+-rw-r--r--   0        0        0     2723 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_401.py
+-rw-r--r--   0        0        0     1957 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_401_data.py
+-rw-r--r--   0        0        0      255 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_401_data_code.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_401_status.py
+-rw-r--r--   0        0        0     2723 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_404.py
+-rw-r--r--   0        0        0     2123 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_404_data.py
+-rw-r--r--   0        0        0      255 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_404_data_code.py
+-rw-r--r--   0        0        0      273 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_404_data_message.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_404_status.py
+-rw-r--r--   0        0        0     2723 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_500.py
+-rw-r--r--   0        0        0     1940 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_500_data.py
+-rw-r--r--   0        0        0      255 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_500_data_code.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_project_response_500_status.py
+-rw-r--r--   0        0        0     2453 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_200.py
+-rw-r--r--   0        0        0    12798 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_200_data.py
+-rw-r--r--   0        0        0      202 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_200_data_citations_view_type.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_200_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_400.py
+-rw-r--r--   0        0        0     1968 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_400_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_400_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_400_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.645525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_401.py
+-rw-r--r--   0        0        0     1963 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_401_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_401_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_401_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_404.py
+-rw-r--r--   0        0        0     2130 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_404_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_404_data_code.py
+-rw-r--r--   0        0        0      274 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_404_data_message.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_404_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_500.py
+-rw-r--r--   0        0        0     1946 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_500_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_500_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_settings_response_500_status.py
+-rw-r--r--   0        0        0     2397 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_user_response_200.py
+-rw-r--r--   0        0        0     3872 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_user_response_200_data.py
+-rw-r--r--   0        0        0      173 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_user_response_200_status.py
+-rw-r--r--   0        0        0     2681 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_user_response_401.py
+-rw-r--r--   0        0        0     1939 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_user_response_401_data.py
+-rw-r--r--   0        0        0      252 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_user_response_401_data_code.py
+-rw-r--r--   0        0        0      173 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_user_response_401_status.py
+-rw-r--r--   0        0        0     2681 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_user_response_500.py
+-rw-r--r--   0        0        0     1922 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_user_response_500_data.py
+-rw-r--r--   0        0        0      252 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_user_response_500_data_code.py
+-rw-r--r--   0        0        0      173 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/get_user_response_500_status.py
+-rw-r--r--   0        0        0      156 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_order.py
+-rw-r--r--   0        0        0     2467 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_200.py
+-rw-r--r--   0        0        0     6000 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_200_data.py
+-rw-r--r--   0        0        0     7769 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_200_data_data_item.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_200_data_data_item_type.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_200_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_401.py
+-rw-r--r--   0        0        0     1969 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_401_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_401_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_401_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_500.py
+-rw-r--r--   0        0        0     1952 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_500_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_500_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_projects_response_500_status.py
+-rw-r--r--   0        0        0     2453 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200.py
+-rw-r--r--   0        0        0     3300 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data.py
+-rw-r--r--   0        0        0     5785 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_sitemaps_item.py
+-rw-r--r--   0        0        0     8143 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_sitemaps_item_pages_item.py
+-rw-r--r--   0        0        0      260 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_sitemaps_item_pages_item_crawl_status.py
+-rw-r--r--   0        0        0      260 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_sitemaps_item_pages_item_index_status.py
+-rw-r--r--   0        0        0     3101 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_sitemaps_item_settings.py
+-rw-r--r--   0        0        0      193 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_sitemaps_item_type.py
+-rw-r--r--   0        0        0     5614 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_uploads.py
+-rw-r--r--   0        0        0     8095 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_uploads_pages_item.py
+-rw-r--r--   0        0        0      255 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_uploads_pages_item_crawl_status.py
+-rw-r--r--   0        0        0      255 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_uploads_pages_item_index_status.py
+-rw-r--r--   0        0        0     3073 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_uploads_settings.py
+-rw-r--r--   0        0        0      188 2024-05-14 19:49:04.649525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_uploads_type.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_400.py
+-rw-r--r--   0        0        0     1968 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_400_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_400_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_400_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_401.py
+-rw-r--r--   0        0        0     1963 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_401_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_401_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_401_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_404.py
+-rw-r--r--   0        0        0     2130 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_404_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_404_data_code.py
+-rw-r--r--   0        0        0      274 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_404_data_message.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_404_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_500.py
+-rw-r--r--   0        0        0     1946 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_500_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_500_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/list_sources_response_500_status.py
+-rw-r--r--   0        0        0      164 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_order.py
+-rw-r--r--   0        0        0     2579 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200.py
+-rw-r--r--   0        0        0     3446 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200_data.py
+-rw-r--r--   0        0        0     5176 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200_data_conversation.py
+-rw-r--r--   0        0        0     6239 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200_data_messages.py
+-rw-r--r--   0        0        0     6593 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200_data_messages_data_item.py
+-rw-r--r--   0        0        0     3153 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200_data_messages_data_item_metadata.py
+-rw-r--r--   0        0        0      186 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200_status.py
+-rw-r--r--   0        0        0     2863 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_400.py
+-rw-r--r--   0        0        0     2022 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_400_data.py
+-rw-r--r--   0        0        0      265 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_400_data_code.py
+-rw-r--r--   0        0        0      186 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_400_status.py
+-rw-r--r--   0        0        0     2863 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_401.py
+-rw-r--r--   0        0        0     2017 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_401_data.py
+-rw-r--r--   0        0        0      265 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_401_data_code.py
+-rw-r--r--   0        0        0      186 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_401_status.py
+-rw-r--r--   0        0        0     2863 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_404.py
+-rw-r--r--   0        0        0     2193 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_404_data.py
+-rw-r--r--   0        0        0      265 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_404_data_code.py
+-rw-r--r--   0        0        0      283 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_404_data_message.py
+-rw-r--r--   0        0        0      186 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_404_status.py
+-rw-r--r--   0        0        0     2863 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_500.py
+-rw-r--r--   0        0        0     2000 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_500_data.py
+-rw-r--r--   0        0        0      265 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_500_data_code.py
+-rw-r--r--   0        0        0      186 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_500_status.py
+-rw-r--r--   0        0        0     4611 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/open_graph_cache.py
+-rw-r--r--   0        0        0     7615 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/page.py
+-rw-r--r--   0        0        0      217 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/page_crawl_status.py
+-rw-r--r--   0        0        0      217 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/page_index_status.py
+-rw-r--r--   0        0        0     2564 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/page_metadata.py
+-rw-r--r--   0        0        0     2793 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_400.py
+-rw-r--r--   0        0        0     1992 2024-05-14 19:49:04.653525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_400_data.py
+-rw-r--r--   0        0        0      260 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_400_data_code.py
+-rw-r--r--   0        0        0      181 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_400_status.py
+-rw-r--r--   0        0        0     2793 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_401.py
+-rw-r--r--   0        0        0     1987 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_401_data.py
+-rw-r--r--   0        0        0      260 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_401_data_code.py
+-rw-r--r--   0        0        0      181 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_401_status.py
+-rw-r--r--   0        0        0     2793 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_404.py
+-rw-r--r--   0        0        0     2152 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_404_data.py
+-rw-r--r--   0        0        0      260 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_404_data_code.py
+-rw-r--r--   0        0        0      260 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_404_data_message.py
+-rw-r--r--   0        0        0      181 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_404_status.py
+-rw-r--r--   0        0        0     2793 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_500.py
+-rw-r--r--   0        0        0     1970 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_500_data.py
+-rw-r--r--   0        0        0      260 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_500_data_code.py
+-rw-r--r--   0        0        0      181 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_500_status.py
+-rw-r--r--   0        0        0     7543 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/project.py
+-rw-r--r--   0        0        0     3238 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/project_plugin.py
+-rw-r--r--   0        0        0    12315 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/project_settings.py
+-rw-r--r--   0        0        0      191 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/project_settings_citations_view_type.py
+-rw-r--r--   0        0        0      228 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/project_settings_response_source.py
+-rw-r--r--   0        0        0     5009 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/project_source.py
+-rw-r--r--   0        0        0     2961 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/project_source_settings.py
+-rw-r--r--   0        0        0      168 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/project_source_type.py
+-rw-r--r--   0        0        0      156 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/project_type.py
+-rw-r--r--   0        0        0     6027 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/prompt_history.py
+-rw-r--r--   0        0        0     2945 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/prompt_history_metadata.py
+-rw-r--r--   0        0        0     2453 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_200.py
+-rw-r--r--   0        0        0     1613 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_200_data.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_200_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_400.py
+-rw-r--r--   0        0        0     1968 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_400_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_400_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_400_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_401.py
+-rw-r--r--   0        0        0     1963 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_401_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_401_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_401_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_403.py
+-rw-r--r--   0        0        0     2144 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_403_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_403_data_code.py
+-rw-r--r--   0        0        0      228 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_403_data_message.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_403_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_500.py
+-rw-r--r--   0        0        0     1946 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_500_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_500_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_500_status.py
+-rw-r--r--   0        0        0     2296 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/send_message_json_body.py
+-rw-r--r--   0        0        0     2453 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/send_message_response_200.py
+-rw-r--r--   0        0        0     6211 2024-05-14 19:49:04.657525 customgpt_client-1.2.2/customgpt_client/models/send_message_response_200_data.py
+-rw-r--r--   0        0        0     3019 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_200_data_metadata.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_200_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_400.py
+-rw-r--r--   0        0        0     1968 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_400_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_400_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_400_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_401.py
+-rw-r--r--   0        0        0     1963 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_401_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_401_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_401_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_404.py
+-rw-r--r--   0        0        0     2130 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_404_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_404_data_code.py
+-rw-r--r--   0        0        0      274 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_404_data_message.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_404_status.py
+-rw-r--r--   0        0        0     2737 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_500.py
+-rw-r--r--   0        0        0     1946 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_500_data.py
+-rw-r--r--   0        0        0      256 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_500_data_code.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/send_message_response_500_status.py
+-rw-r--r--   0        0        0     2467 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_200.py
+-rw-r--r--   0        0        0     3698 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_200_data.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_200_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_400.py
+-rw-r--r--   0        0        0     1974 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_400_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_400_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_400_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_401.py
+-rw-r--r--   0        0        0     1969 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_401_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_401_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_401_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_404.py
+-rw-r--r--   0        0        0     2137 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_404_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_404_data_code.py
+-rw-r--r--   0        0        0      275 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_404_data_message.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_404_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_500.py
+-rw-r--r--   0        0        0     1952 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_500_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_500_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/stats_project_response_500_status.py
+-rw-r--r--   0        0        0     1569 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_json_body.py
+-rw-r--r--   0        0        0     2551 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_200.py
+-rw-r--r--   0        0        0     5103 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_200_data.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_200_status.py
+-rw-r--r--   0        0        0     2835 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_400.py
+-rw-r--r--   0        0        0     2010 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_400_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_400_data_code.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_400_status.py
+-rw-r--r--   0        0        0     2835 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_401.py
+-rw-r--r--   0        0        0     2005 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_401_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_401_data_code.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_401_status.py
+-rw-r--r--   0        0        0     2835 2024-05-14 19:49:04.661526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_404.py
+-rw-r--r--   0        0        0     2179 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_404_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_404_data_code.py
+-rw-r--r--   0        0        0      281 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_404_data_message.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_404_status.py
+-rw-r--r--   0        0        0     2835 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_500.py
+-rw-r--r--   0        0        0     1988 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_500_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_500_data_code.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_500_status.py
+-rw-r--r--   0        0        0     2603 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_json_body.py
+-rw-r--r--   0        0        0     2556 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_200.py
+-rw-r--r--   0        0        0     2681 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_200_data.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_200_status.py
+-rw-r--r--   0        0        0     2840 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_400.py
+-rw-r--r--   0        0        0     2013 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_400_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_400_data_code.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_400_status.py
+-rw-r--r--   0        0        0     2840 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_401.py
+-rw-r--r--   0        0        0     2008 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_401_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_401_data_code.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_401_status.py
+-rw-r--r--   0        0        0     2840 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_404.py
+-rw-r--r--   0        0        0     2176 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_404_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_404_data_code.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_404_data_message.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_404_status.py
+-rw-r--r--   0        0        0     2840 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_500.py
+-rw-r--r--   0        0        0     1991 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_500_data.py
+-rw-r--r--   0        0        0      263 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_500_data_code.py
+-rw-r--r--   0        0        0      184 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_500_status.py
+-rw-r--r--   0        0        0     2992 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_json_body.py
+-rw-r--r--   0        0        0     2467 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_200.py
+-rw-r--r--   0        0        0     3317 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_200_data.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_200_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_400.py
+-rw-r--r--   0        0        0     1974 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_400_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_400_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_400_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_401.py
+-rw-r--r--   0        0        0     1969 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_401_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_401_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_401_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_404.py
+-rw-r--r--   0        0        0     2151 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_404_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_404_data_code.py
+-rw-r--r--   0        0        0      405 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_404_data_message.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_404_status.py
+-rw-r--r--   0        0        0     2751 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_500.py
+-rw-r--r--   0        0        0     1952 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_500_data.py
+-rw-r--r--   0        0        0      257 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_500_data_code.py
+-rw-r--r--   0        0        0      178 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_500_status.py
+-rw-r--r--   0        0        0     4967 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_project_multipart_data.py
+-rw-r--r--   0        0        0     2481 2024-05-14 19:49:04.665526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_200.py
+-rw-r--r--   0        0        0     7714 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_200_data.py
+-rw-r--r--   0        0        0      177 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_200_data_type.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_200_status.py
+-rw-r--r--   0        0        0     2765 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_400.py
+-rw-r--r--   0        0        0     1980 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_400_data.py
+-rw-r--r--   0        0        0      258 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_400_data_code.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_400_status.py
+-rw-r--r--   0        0        0     2765 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_401.py
+-rw-r--r--   0        0        0     1975 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_401_data.py
+-rw-r--r--   0        0        0      258 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_401_data_code.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_401_status.py
+-rw-r--r--   0        0        0     2765 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_404.py
+-rw-r--r--   0        0        0     2144 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_404_data.py
+-rw-r--r--   0        0        0      258 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_404_data_code.py
+-rw-r--r--   0        0        0      276 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_404_data_message.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_404_status.py
+-rw-r--r--   0        0        0     2765 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_500.py
+-rw-r--r--   0        0        0     1958 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_500_data.py
+-rw-r--r--   0        0        0      258 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_500_data_code.py
+-rw-r--r--   0        0        0      179 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_project_response_500_status.py
+-rw-r--r--   0        0        0    19231 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_multipart_data.py
+-rw-r--r--   0        0        0      203 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_multipart_data_citations_view_type.py
+-rw-r--r--   0        0        0     2495 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_200.py
+-rw-r--r--   0        0        0     1621 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_200_data.py
+-rw-r--r--   0        0        0      180 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_200_status.py
+-rw-r--r--   0        0        0     2779 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_400.py
+-rw-r--r--   0        0        0     2183 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_400_data.py
+-rw-r--r--   0        0        0      259 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_400_data_code.py
+-rw-r--r--   0        0        0      416 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_400_data_message.py
+-rw-r--r--   0        0        0      180 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_400_status.py
+-rw-r--r--   0        0        0     2779 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_401.py
+-rw-r--r--   0        0        0     1981 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_401_data.py
+-rw-r--r--   0        0        0      259 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_401_data_code.py
+-rw-r--r--   0        0        0      180 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_401_status.py
+-rw-r--r--   0        0        0     2779 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_500.py
+-rw-r--r--   0        0        0     1964 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_500_data.py
+-rw-r--r--   0        0        0      259 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_500_data_code.py
+-rw-r--r--   0        0        0      180 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_settings_response_500_status.py
+-rw-r--r--   0        0        0     2991 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_user_multipart_data.py
+-rw-r--r--   0        0        0     2439 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_user_response_200.py
+-rw-r--r--   0        0        0     3887 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_user_response_200_data.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_user_response_200_status.py
+-rw-r--r--   0        0        0     2723 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_user_response_401.py
+-rw-r--r--   0        0        0     1957 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_user_response_401_data.py
+-rw-r--r--   0        0        0      255 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_user_response_401_data_code.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_user_response_401_status.py
+-rw-r--r--   0        0        0     2723 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_user_response_500.py
+-rw-r--r--   0        0        0     1940 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_user_response_500_data.py
+-rw-r--r--   0        0        0      255 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_user_response_500_data_code.py
+-rw-r--r--   0        0        0      176 2024-05-14 19:49:04.669526 customgpt_client-1.2.2/customgpt_client/models/update_user_response_500_status.py
+-rw-r--r--   0        0        0     3770 2024-05-14 19:49:04.673526 customgpt_client-1.2.2/customgpt_client/models/user.py
+-rw-r--r--   0        0        0       25 2024-05-14 19:49:04.673526 customgpt_client-1.2.2/customgpt_client/py.typed
+-rw-r--r--   0        0        0      993 2024-05-14 19:49:04.673526 customgpt_client-1.2.2/customgpt_client/types.py
+-rw-r--r--   0        0        0      693 2024-05-23 17:54:25.482424 customgpt_client-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 customgpt_client-1.2.2/PKG-INFO
```

### Comparing `customgpt_client-1.2.1/README.md` & `customgpt_client-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/citations/get_citation.py` & `customgpt_client-1.2.2/customgpt_client/api/citations/get_citation.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/conversations/create_conversation.py` & `customgpt_client-1.2.2/customgpt_client/api/conversations/create_conversation.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/conversations/delete_conversation.py` & `customgpt_client-1.2.2/customgpt_client/api/conversations/delete_conversation.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/conversations/get_conversations.py` & `customgpt_client-1.2.2/customgpt_client/api/conversations/get_conversations.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/conversations/messages_conversation.py` & `customgpt_client-1.2.2/customgpt_client/api/conversations/messages_conversation.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/conversations/send_message.py` & `customgpt_client-1.2.2/customgpt_client/api/conversations/send_message.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/conversations/update_conversation.py` & `customgpt_client-1.2.2/customgpt_client/api/conversations/update_conversation.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/page_metadata/get_page_metadata.py` & `customgpt_client-1.2.2/customgpt_client/api/page_metadata/get_page_metadata.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/page_metadata/update_page_metadata.py` & `customgpt_client-1.2.2/customgpt_client/api/page_metadata/update_page_metadata.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/pages/delete_page.py` & `customgpt_client-1.2.2/customgpt_client/api/pages/delete_page.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/pages/get_pages.py` & `customgpt_client-1.2.2/customgpt_client/api/pages/get_pages.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/pages/preview_citation.py` & `customgpt_client-1.2.2/customgpt_client/api/pages/preview_citation.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/pages/reindex_page.py` & `customgpt_client-1.2.2/customgpt_client/api/pages/reindex_page.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/project_plugins/create_plugin.py` & `customgpt_client-1.2.2/customgpt_client/api/project_plugins/create_plugin.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/project_plugins/get_plugin.py` & `customgpt_client-1.2.2/customgpt_client/api/project_plugins/get_plugin.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/project_plugins/update_plugin.py` & `customgpt_client-1.2.2/customgpt_client/api/project_plugins/update_plugin.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/project_settings/get_settings.py` & `customgpt_client-1.2.2/customgpt_client/api/project_settings/get_settings.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/project_settings/update_settings.py` & `customgpt_client-1.2.2/customgpt_client/api/project_settings/update_settings.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/projects/create_project.py` & `customgpt_client-1.2.2/customgpt_client/api/projects/create_project.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/projects/delete_project.py` & `customgpt_client-1.2.2/customgpt_client/api/projects/delete_project.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/projects/get_project.py` & `customgpt_client-1.2.2/customgpt_client/api/projects/get_project.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/projects/list_projects.py` & `customgpt_client-1.2.2/customgpt_client/api/projects/list_projects.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/projects/stats_project.py` & `customgpt_client-1.2.2/customgpt_client/api/projects/stats_project.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/projects/update_project.py` & `customgpt_client-1.2.2/customgpt_client/api/projects/update_project.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/sources/create_source.py` & `customgpt_client-1.2.2/customgpt_client/api/sources/create_source.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/sources/delete_source.py` & `customgpt_client-1.2.2/customgpt_client/api/sources/delete_source.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/sources/list_sources.py` & `customgpt_client-1.2.2/customgpt_client/api/sources/list_sources.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/users/get_user.py` & `customgpt_client-1.2.2/customgpt_client/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/api/users/update_user.py` & `customgpt_client-1.2.2/customgpt_client/api/users/update_user.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/client.py` & `customgpt_client-1.2.2/customgpt_client/client.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/__init__.py` & `customgpt_client-1.2.2/customgpt_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/conversation.py` & `customgpt_client-1.2.2/customgpt_client/models/conversation.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_conversation_json_body.py` & `customgpt_client-1.2.2/customgpt_client/models/create_conversation_json_body.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_201.py` & `customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_201.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_201_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_201_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_conversation_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_conversation_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_plugin_json_body.py` & `customgpt_client-1.2.2/customgpt_client/models/create_plugin_json_body.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_201.py` & `customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_201.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_201_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_201_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_plugin_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_plugin_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_project_multipart_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_project_multipart_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_project_response_201.py` & `customgpt_client-1.2.2/customgpt_client/models/create_project_response_201.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_project_response_201_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_project_response_201_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_project_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/create_project_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_project_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_project_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_project_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/create_project_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_project_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_project_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_project_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/create_project_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_project_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_project_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_multipart_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_multipart_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_response_201.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_response_201.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_response_201_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_response_201_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_response_201_data_pages_item.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_response_201_data_pages_item.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_response_201_data_settings.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_response_201_data_settings.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/create_source_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/create_source_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_conversation_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_conversation_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_page_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_page_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_page_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_page_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_page_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_page_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_page_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_page_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_page_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_page_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_page_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_page_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_page_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_page_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_page_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_page_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_page_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_page_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_page_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_page_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_project_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_project_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_project_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_project_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_project_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_project_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_project_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_project_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_project_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_project_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_project_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_project_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_project_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_project_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_project_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_project_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_project_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_project_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_project_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_project_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_source_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_source_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_source_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_source_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_source_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_source_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_source_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_source_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_source_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_source_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_source_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_source_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_source_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_source_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_source_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_source_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_source_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_source_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/delete_source_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/delete_source_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_citation_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/get_citation_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_citation_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_citation_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_citation_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/get_citation_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_citation_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_citation_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_citation_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/get_citation_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_citation_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_citation_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_citation_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/get_citation_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_citation_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_citation_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_200_data_data_item.py` & `customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_200_data_data_item.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_conversations_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_conversations_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_page_metadata_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_page_metadata_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200_data_pages.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200_data_pages.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200_data_pages_data_item.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200_data_pages_data_item.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_200_data_project.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_200_data_project.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_pages_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_pages_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_plugin_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_plugin_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_project_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/get_project_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_project_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_project_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_project_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/get_project_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_project_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_project_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_project_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/get_project_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_project_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_project_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_project_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/get_project_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_project_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_project_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_project_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/get_project_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_project_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_project_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_settings_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/get_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_settings_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_settings_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_settings_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/get_settings_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_settings_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_settings_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_settings_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/get_settings_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_settings_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_settings_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_settings_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/get_settings_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_settings_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_settings_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_settings_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/get_settings_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_settings_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_settings_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_user_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/get_user_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_user_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_user_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_user_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/get_user_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_user_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_user_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_user_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/get_user_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/get_user_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/get_user_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_projects_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/list_projects_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_projects_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/list_projects_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_projects_response_200_data_data_item.py` & `customgpt_client-1.2.2/customgpt_client/models/list_projects_response_200_data_data_item.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_projects_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/list_projects_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_projects_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/list_projects_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_projects_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/list_projects_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_projects_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/list_projects_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_sitemaps_item.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_sitemaps_item.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_sitemaps_item_pages_item.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_sitemaps_item_pages_item.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_sitemaps_item_settings.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_sitemaps_item_settings.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_uploads.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_uploads.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_uploads_pages_item.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_uploads_pages_item.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_200_data_uploads_settings.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_200_data_uploads_settings.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/list_sources_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/list_sources_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200_data_conversation.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200_data_conversation.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200_data_messages.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200_data_messages.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200_data_messages_data_item.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200_data_messages_data_item.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_200_data_messages_data_item_metadata.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_200_data_messages_data_item_metadata.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/messages_conversation_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/messages_conversation_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/open_graph_cache.py` & `customgpt_client-1.2.2/customgpt_client/models/open_graph_cache.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/page.py` & `customgpt_client-1.2.2/customgpt_client/models/page.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/page_metadata.py` & `customgpt_client-1.2.2/customgpt_client/models/page_metadata.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/preview_citation_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/preview_citation_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/project.py` & `customgpt_client-1.2.2/customgpt_client/models/project.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/project_plugin.py` & `customgpt_client-1.2.2/customgpt_client/models/project_plugin.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/project_settings.py` & `customgpt_client-1.2.2/customgpt_client/models/project_settings.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/project_source.py` & `customgpt_client-1.2.2/customgpt_client/models/project_source.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/project_source_settings.py` & `customgpt_client-1.2.2/customgpt_client/models/project_source_settings.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/prompt_history.py` & `customgpt_client-1.2.2/customgpt_client/models/prompt_history.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/prompt_history_metadata.py` & `customgpt_client-1.2.2/customgpt_client/models/prompt_history_metadata.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_403.py` & `customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_403.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_403_data.py` & `customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_403_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/reindex_page_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/reindex_page_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/send_message_json_body.py` & `customgpt_client-1.2.2/customgpt_client/models/send_message_json_body.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/send_message_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/send_message_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/send_message_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/send_message_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/send_message_response_200_data_metadata.py` & `customgpt_client-1.2.2/customgpt_client/models/send_message_response_200_data_metadata.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/send_message_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/send_message_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/send_message_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/send_message_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/send_message_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/send_message_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/send_message_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/send_message_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/send_message_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/send_message_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/send_message_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/send_message_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/send_message_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/send_message_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/send_message_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/send_message_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/stats_project_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/stats_project_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/stats_project_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/stats_project_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/stats_project_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/stats_project_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/stats_project_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/stats_project_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/stats_project_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/stats_project_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/stats_project_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/stats_project_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/stats_project_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/stats_project_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/stats_project_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/stats_project_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/stats_project_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/stats_project_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/stats_project_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/stats_project_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_conversation_json_body.py` & `customgpt_client-1.2.2/customgpt_client/models/update_conversation_json_body.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_conversation_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_conversation_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_json_body.py` & `customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_json_body.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_page_metadata_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_page_metadata_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_plugin_json_body.py` & `customgpt_client-1.2.2/customgpt_client/models/update_plugin_json_body.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_plugin_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_plugin_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_project_multipart_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_project_multipart_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_project_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/update_project_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_project_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_project_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_project_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/update_project_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_project_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_project_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_project_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/update_project_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_project_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_project_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_project_response_404.py` & `customgpt_client-1.2.2/customgpt_client/models/update_project_response_404.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_project_response_404_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_project_response_404_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_project_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/update_project_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_project_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_project_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_settings_multipart_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_settings_multipart_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_settings_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/update_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_settings_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_settings_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_settings_response_400.py` & `customgpt_client-1.2.2/customgpt_client/models/update_settings_response_400.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_settings_response_400_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_settings_response_400_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_settings_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/update_settings_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_settings_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_settings_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_settings_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/update_settings_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_settings_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_settings_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_user_multipart_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_user_multipart_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_user_response_200.py` & `customgpt_client-1.2.2/customgpt_client/models/update_user_response_200.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_user_response_200_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_user_response_200_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_user_response_401.py` & `customgpt_client-1.2.2/customgpt_client/models/update_user_response_401.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_user_response_401_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_user_response_401_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_user_response_500.py` & `customgpt_client-1.2.2/customgpt_client/models/update_user_response_500.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/update_user_response_500_data.py` & `customgpt_client-1.2.2/customgpt_client/models/update_user_response_500_data.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/models/user.py` & `customgpt_client-1.2.2/customgpt_client/models/user.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/customgpt_client/types.py` & `customgpt_client-1.2.2/customgpt_client/types.py`

 * *Files identical despite different names*

### Comparing `customgpt_client-1.2.1/pyproject.toml` & `customgpt_client-1.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "customgpt-client"
-version = "1.2.1"
+version = "1.2.2"
 description = "A client library for accessing customgpt"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "customgpt_client"},
@@ -12,15 +12,15 @@
 include = ["CHANGELOG.md", "customgpt_client/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 sseclient-py = "1.7.2"
 attrs = ">=21.3.0"
 python-dateutil = "^2.8.0"
-requests="2.31.0"
+requests=">=2.31.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `customgpt_client-1.2.1/PKG-INFO` & `customgpt_client-1.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: customgpt-client
-Version: 1.2.1
+Version: 1.2.2
 Summary: A client library for accessing customgpt
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attrs (>=21.3.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
-Requires-Dist: requests (==2.31.0)
+Requires-Dist: requests (>=2.31.0)
 Requires-Dist: sseclient-py (==1.7.2)
 Description-Content-Type: text/markdown
 
 # CustomGPT SDK
 
 ## Usage
 First, create a client:
```

