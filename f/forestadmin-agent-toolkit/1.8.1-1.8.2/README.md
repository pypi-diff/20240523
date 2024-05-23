# Comparing `tmp/forestadmin_agent_toolkit-1.8.1.tar.gz` & `tmp/forestadmin_agent_toolkit-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_toolkit-1.8.1.tar", max compression
+gzip compressed data, was "forestadmin_agent_toolkit-1.8.2.tar", max compression
```

## Comparing `forestadmin_agent_toolkit-1.8.1.tar` & `forestadmin_agent_toolkit-1.8.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0        0 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/README.md
--rw-r--r--   0        0        0        0 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/__init__.py
--rw-r--r--   0        0        0     9526 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/agent.py
--rw-r--r--   0        0        0      135 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/exceptions.py
--rw-r--r--   0        0        0     2477 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/forest_logger.py
--rw-r--r--   0        0        0     4152 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/options.py
--rw-r--r--   0        0        0        0 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/actions/__init__.py
--rw-r--r--   0        0        0     2305 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/actions/requests.py
--rw-r--r--   0        0        0     9544 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/actions/resources.py
--rw-r--r--   0        0        0      464 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/base.py
--rw-r--r--   0        0        0        0 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/__init__.py
--rw-r--r--   0        0        0     1055 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py
--rw-r--r--   0        0        0     2780 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/charts_collection.py
--rw-r--r--   0        0        0     1912 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
--rw-r--r--   0        0        0    17490 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/crud.py
--rw-r--r--   0        0        0    22065 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/crud_related.py
--rw-r--r--   0        0        0     4348 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/decorators.py
--rw-r--r--   0        0        0      148 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/exceptions.py
--rw-r--r--   0        0        0    13206 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/filter.py
--rw-r--r--   0        0        0     5509 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/requests.py
--rw-r--r--   0        0        0    12193 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/stats.py
--rw-r--r--   0        0        0      935 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/ip_white_list_resource.py
--rw-r--r--   0        0        0        0 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/security/__init__.py
--rw-r--r--   0        0        0      427 2024-05-14 13:52:43.674476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/security/exceptions.py
--rw-r--r--   0        0        0     4696 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/security/resources.py
--rw-r--r--   0        0        0        0 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/__init__.py
--rw-r--r--   0        0        0     1695 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py
--rw-r--r--   0        0        0      176 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/options.py
--rw-r--r--   0        0        0     9001 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/permission_service.py
--rw-r--r--   0        0        0     3261 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/permissions_functions.py
--rw-r--r--   0        0        0      406 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/permissions_types.py
--rw-r--r--   0        0        0     5276 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py
--rw-r--r--   0        0        0     3200 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py
--rw-r--r--   0        0        0     1010 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/serializers/__init__.py
--rw-r--r--   0        0        0    10346 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/serializers/json_api.py
--rw-r--r--   0        0        0        0 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     3663 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/authentication.py
--rw-r--r--   0        0        0     4554 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/context.py
--rw-r--r--   0        0        0     1252 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/context_variable_injector.py
--rw-r--r--   0        0        0      655 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/context_variable_instantiator.py
--rw-r--r--   0        0        0     1230 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/context_variables.py
--rw-r--r--   0        0        0     1661 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/csv.py
--rw-r--r--   0        0        0        0 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
--rw-r--r--   0        0        0     3019 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py
--rw-r--r--   0        0        0     6276 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
--rw-r--r--   0        0        0     4229 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
--rw-r--r--   0        0        0     2298 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
--rw-r--r--   0        0        0     5069 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
--rw-r--r--   0        0        0    13958 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py
--rw-r--r--   0        0        0     2461 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
--rw-r--r--   0        0        0     8646 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
--rw-r--r--   0        0        0      506 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
--rw-r--r--   0        0        0     9931 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/type.py
--rw-r--r--   0        0        0     1281 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/validation.py
--rw-r--r--   0        0        0     7303 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/http.py
--rw-r--r--   0        0        0     1774 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/id.py
--rw-r--r--   0        0        0     1889 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/ip_whitelist_util.py
--rw-r--r--   0        0        0      513 2024-05-14 13:52:43.678476 forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/token.py
--rw-r--r--   0        0        0     1776 2024-05-14 13:53:00.958487 forestadmin_agent_toolkit-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/__init__.py
+-rw-r--r--   0        0        0     9526 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/agent.py
+-rw-r--r--   0        0        0      135 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/exceptions.py
+-rw-r--r--   0        0        0     2477 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/forest_logger.py
+-rw-r--r--   0        0        0     4152 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/options.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/actions/__init__.py
+-rw-r--r--   0        0        0     2305 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/actions/requests.py
+-rw-r--r--   0        0        0     9544 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/actions/resources.py
+-rw-r--r--   0        0        0      464 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/base.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/__init__.py
+-rw-r--r--   0        0        0     1055 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py
+-rw-r--r--   0        0        0     2780 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/charts_collection.py
+-rw-r--r--   0        0        0     1912 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
+-rw-r--r--   0        0        0    17490 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/crud.py
+-rw-r--r--   0        0        0    22065 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/crud_related.py
+-rw-r--r--   0        0        0     4348 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/decorators.py
+-rw-r--r--   0        0        0      148 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/exceptions.py
+-rw-r--r--   0        0        0    13206 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/filter.py
+-rw-r--r--   0        0        0     5509 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/requests.py
+-rw-r--r--   0        0        0    12193 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/stats.py
+-rw-r--r--   0        0        0      935 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/ip_white_list_resource.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/security/__init__.py
+-rw-r--r--   0        0        0      427 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/security/exceptions.py
+-rw-r--r--   0        0        0     4696 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/security/resources.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/__init__.py
+-rw-r--r--   0        0        0     1695 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py
+-rw-r--r--   0        0        0      176 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/options.py
+-rw-r--r--   0        0        0     9001 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/permission_service.py
+-rw-r--r--   0        0        0     3261 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/permissions_functions.py
+-rw-r--r--   0        0        0      406 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/permissions_types.py
+-rw-r--r--   0        0        0     5276 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py
+-rw-r--r--   0        0        0     3200 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py
+-rw-r--r--   0        0        0     1010 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/serializers/__init__.py
+-rw-r--r--   0        0        0    10346 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/serializers/json_api.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     3663 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/authentication.py
+-rw-r--r--   0        0        0     4554 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context.py
+-rw-r--r--   0        0        0     1252 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context_variable_injector.py
+-rw-r--r--   0        0        0      655 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context_variable_instantiator.py
+-rw-r--r--   0        0        0     1230 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context_variables.py
+-rw-r--r--   0        0        0     1661 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/csv.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
+-rw-r--r--   0        0        0     3019 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py
+-rw-r--r--   0        0        0     6276 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
+-rw-r--r--   0        0        0     4229 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
+-rw-r--r--   0        0        0     2298 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
+-rw-r--r--   0        0        0     5069 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
+-rw-r--r--   0        0        0    13958 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py
+-rw-r--r--   0        0        0     2461 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
+-rw-r--r--   0        0        0     8646 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
+-rw-r--r--   0        0        0      506 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
+-rw-r--r--   0        0        0     9931 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/type.py
+-rw-r--r--   0        0        0     1281 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/validation.py
+-rw-r--r--   0        0        0     7303 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/http.py
+-rw-r--r--   0        0        0     1774 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/id.py
+-rw-r--r--   0        0        0     1889 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/ip_whitelist_util.py
+-rw-r--r--   0        0        0      513 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/token.py
+-rw-r--r--   0        0        0     1776 2024-05-23 09:47:50.548705 forestadmin_agent_toolkit-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.8.2/PKG-INFO
```

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/agent.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/agent.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/forest_logger.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/forest_logger.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/options.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/options.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/actions/requests.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/actions/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/actions/resources.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/actions/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/charts_collection.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/charts_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/charts_datasource.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/charts_datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/crud.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/crud.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/crud_related.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/crud_related.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/decorators.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/decorators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/filter.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/filter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/requests.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/collections/stats.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/stats.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/ip_white_list_resource.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/ip_white_list_resource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/resources/security/resources.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/security/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/permission_service.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/permission_service.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/permissions_functions.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/permissions_functions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/serializers/__init__.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/services/serializers/json_api.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/serializers/json_api.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/authentication.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/context.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/context_variable_injector.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context_variable_injector.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/context_variable_instantiator.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context_variable_instantiator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/context_variables.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context_variables.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/csv.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/csv.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/action_values.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/action_values.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/emitter.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/emitter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/filterable.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/filterable.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/type.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/type.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/forest_schema/validation.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/validation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/http.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/http.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/id.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/id.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/ip_whitelist_util.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/ip_whitelist_util.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/forestadmin/agent_toolkit/utils/token.py` & `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/token.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.1/pyproject.toml` & `forestadmin_agent_toolkit-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-toolkit"
 description = "agent toolkit for forestadmin python agent"
-version = "1.8.1"
+version = "1.8.2"
 authors = [ "Valentin Monté <valentinm@forestadmin.com>", "Julien Barreau <julien.barreau@forestadmin.com>",]
 readme = "README.md"
 repository = "https://github.com/ForestAdmin/agent-python"
 documentation = "https://docs.forestadmin.com/developer-guide-agents-python/"
 homepage = "https://www.forestadmin.com"
 [[tool.poetry.packages]]
 include = "forestadmin"
@@ -19,15 +19,15 @@
 typing-extensions = ">=4.2.0, <5.0"
 aiohttp = "~=3.9"
 oic = "~=1.4"
 pyjwt = "^2"
 cachetools = "~=5.2"
 marshmallow-jsonapi = ">=0.24.0, <1.0"
 sseclient-py = "^1.5"
-forestadmin-datasource-toolkit = "1.8.1"
+forestadmin-datasource-toolkit = "1.8.2"
 [[tool.poetry.dependencies.pandas]]
 version = ">=1.4.0"
 python = ">=3.8"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~0.2.1"
 python = "<3.9"
```

### Comparing `forestadmin_agent_toolkit-1.8.1/PKG-INFO` & `forestadmin_agent_toolkit-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-toolkit
-Version: 1.8.1
+Version: 1.8.2
 Summary: agent toolkit for forestadmin python agent
 Home-page: https://www.forestadmin.com
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9,<4.0)
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: cachetools (>=5.2,<6.0)
-Requires-Dist: forestadmin-datasource-toolkit (==1.8.1)
+Requires-Dist: forestadmin-datasource-toolkit (==1.8.2)
 Requires-Dist: marshmallow-jsonapi (>=0.24.0,<1.0)
 Requires-Dist: oic (>=1.4,<2.0)
 Requires-Dist: pandas (>=1.4.0) ; python_version >= "3.8"
 Requires-Dist: pyjwt (>=2,<3)
 Requires-Dist: sseclient-py (>=1.5,<2.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0)
 Project-URL: Documentation, https://docs.forestadmin.com/developer-guide-agents-python/
```

