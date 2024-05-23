# Comparing `tmp/cwapi3d-30.444.0.tar.gz` & `tmp/cwapi3d-30.498.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwapi3d-30.444.0.tar", last modified: Thu Apr 18 12:39:37 2024, max compression
+gzip compressed data, was "cwapi3d-30.498.0.tar", last modified: Thu May 23 15:19:45 2024, max compression
```

## Comparing `cwapi3d-30.444.0.tar` & `cwapi3d-30.498.0.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.192113 cwapi3d-30.444.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-18 12:39:37.192113 cwapi3d-30.444.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:39:37.192113 cwapi3d-30.444.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.176113 cwapi3d-30.444.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.180112 cwapi3d-30.444.0/src/attribute_controller/
--rw-r--r--   0 runner    (1001) docker     (127)    34319 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/attribute_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.180112 cwapi3d-30.444.0/src/bim_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/bim_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/cadwork/
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/attribute_display_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/btl_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/camera_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/coordinate_system_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/division_zone_direction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/edge_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/element_grouping_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/element_module_detail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/element_module_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/element_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/extended_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/facet_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/hundegger_machine_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_2x3_element_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_element_combine_behaviour.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_options_aggregation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_options_level_of_detail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_options_project_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_options_properties.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    35586 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/ifc_predefined_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/import_3dc_options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/layer_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/node_symbol.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/point_3d.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/polygon_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/process_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/projection_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/rhino_options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/shortcut_key.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/shortcut_key_modifier.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/standard_element_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/text_element_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/text_object_options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/vertex_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/weinmann_mfb_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/cadwork/window_geometry.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/connector_axis_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/connector_axis_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.192113 cwapi3d-30.444.0/src/cwapi3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-18 12:39:37.000000 cwapi3d-30.444.0/src/cwapi3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-18 12:39:37.000000 cwapi3d-30.444.0/src/cwapi3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:39:37.000000 cwapi3d-30.444.0/src/cwapi3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-18 12:39:37.000000 cwapi3d-30.444.0/src/cwapi3d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/dimension_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/dimension_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/element_controller/
--rw-r--r--   0 runner    (1001) docker     (127)    40948 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/element_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/endtype_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/endtype_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/file_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/file_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/geometry_controller/
--rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/geometry_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/list_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/list_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/machine_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/machine_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/material_controller/
--rw-r--r--   0 runner    (1001) docker     (127)    15296 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/material_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/menu_controller/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/menu_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/multi_layer_cover_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/multi_layer_cover_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/roof_controller/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/roof_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/scene_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/scene_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.188113 cwapi3d-30.444.0/src/shop_drawing_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/shop_drawing_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.192113 cwapi3d-30.444.0/src/utility_controller/
--rw-r--r--   0 runner    (1001) docker     (127)    17693 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/utility_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:39:37.192113 cwapi3d-30.444.0/src/visualization_controller/
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-18 12:39:33.000000 cwapi3d-30.444.0/src/visualization_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.667824 cwapi3d-30.498.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-23 15:19:45.667824 cwapi3d-30.498.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:19:45.667824 cwapi3d-30.498.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.655823 cwapi3d-30.498.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.655823 cwapi3d-30.498.0/src/attribute_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)    34319 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/attribute_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.655823 cwapi3d-30.498.0/src/bim_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/bim_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/cadwork/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/attribute_display_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/btl_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/camera_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/coordinate_system_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/division_zone_direction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/edge_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/element_grouping_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/element_module_detail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/element_module_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/element_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/extended_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/facet_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/hundegger_machine_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/ifc_2x3_element_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/ifc_element_combine_behaviour.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/ifc_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/ifc_options_aggregation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/ifc_options_level_of_detail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/ifc_options_project_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/ifc_options_properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    35586 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/ifc_predefined_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/import_3dc_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/layer_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/multi_layer_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/node_symbol.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/point_3d.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/polygon_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/process_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/projection_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/rhino_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/shortcut_key.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/shortcut_key_modifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/standard_element_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/text_element_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/text_object_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/vertex_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/weinmann_mfb_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/cadwork/window_geometry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/connector_axis_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/connector_axis_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.667824 cwapi3d-30.498.0/src/cwapi3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-23 15:19:45.000000 cwapi3d-30.498.0/src/cwapi3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-23 15:19:45.000000 cwapi3d-30.498.0/src/cwapi3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:19:45.000000 cwapi3d-30.498.0/src/cwapi3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-23 15:19:45.000000 cwapi3d-30.498.0/src/cwapi3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/dimension_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/dimension_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/element_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)    41842 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/element_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/endtype_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/endtype_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/file_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/file_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/geometry_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/geometry_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/list_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/list_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/machine_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/machine_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/material_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)    15296 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/material_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/menu_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/menu_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/multi_layer_cover_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/multi_layer_cover_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.663823 cwapi3d-30.498.0/src/roof_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/roof_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.667824 cwapi3d-30.498.0/src/scene_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/scene_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.667824 cwapi3d-30.498.0/src/shop_drawing_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/shop_drawing_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.667824 cwapi3d-30.498.0/src/utility_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)    18404 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/utility_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:45.667824 cwapi3d-30.498.0/src/visualization_controller/
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-23 15:19:39.000000 cwapi3d-30.498.0/src/visualization_controller/__init__.pyi
```

### Comparing `cwapi3d-30.444.0/LICENSE` & `cwapi3d-30.498.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/PKG-INFO` & `cwapi3d-30.498.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwapi3d
-Version: 30.444.0
+Version: 30.498.0
 Summary: Python bindings for CwAPI3D
 Author-email: Cadwork <it@cadwork.ca>
 License: MIT License
         
         Copyright (c) 2024 Cadwork
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cwapi3d-30.444.0/README.md` & `cwapi3d-30.498.0/README.md`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/pyproject.toml` & `cwapi3d-30.498.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cwapi3d"
-version = "30.444.0"
+version = "30.498.0"
 authors = [{ name = "Cadwork", email = "it@cadwork.ca" }]
 requires-python = ">= 3.10"
 description = 'Python bindings for CwAPI3D'
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["cadwork"]
 classifiers = [
```

### Comparing `cwapi3d-30.444.0/src/attribute_controller/__init__.pyi` & `cwapi3d-30.498.0/src/attribute_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/bim_controller/__init__.pyi` & `cwapi3d-30.498.0/src/bim_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/__init__.pyi` & `cwapi3d-30.498.0/src/cadwork/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/attribute_display_settings.pyi` & `cwapi3d-30.498.0/src/cadwork/attribute_display_settings.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/btl_version.pyi` & `cwapi3d-30.498.0/src/cadwork/btl_version.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/camera_data.pyi` & `cwapi3d-30.498.0/src/cadwork/camera_data.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/element_module_detail.pyi` & `cwapi3d-30.498.0/src/cadwork/element_module_detail.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/element_module_properties.pyi` & `cwapi3d-30.498.0/src/cadwork/element_module_properties.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/element_type.pyi` & `cwapi3d-30.498.0/src/cadwork/element_type.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/extended_settings.pyi` & `cwapi3d-30.498.0/src/cadwork/extended_settings.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/facet_list.pyi` & `cwapi3d-30.498.0/src/cadwork/facet_list.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/hundegger_machine_type.pyi` & `cwapi3d-30.498.0/src/cadwork/hundegger_machine_type.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/ifc_2x3_element_type.pyi` & `cwapi3d-30.498.0/src/cadwork/ifc_2x3_element_type.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 class ifc_2x3_element_type:
-    
+
     def is_none(self) -> bool:
         """is none
 
         Returns:
             bool
         """
 
@@ -403,13 +403,27 @@
         """set ifc mechanical fastener
 
         Returns:
             None
         """
 
     def __repr__(self) -> str:
-        """  repr  
+        """  repr
 
         Returns:
             str
         """
 
+    def is_ifc_element_assembly(self) -> bool:
+        """is ifc element assembly
+
+        Returns:
+            bool
+        """
+
+    def set_ifc_element_assembly(self) -> None:
+        """set ifc element assembly
+
+        Returns:
+            None
+        """
+
```

### Comparing `cwapi3d-30.444.0/src/cadwork/ifc_options.pyi` & `cwapi3d-30.498.0/src/cadwork/ifc_options.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/ifc_options_aggregation.pyi` & `cwapi3d-30.498.0/src/cadwork/ifc_options_aggregation.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/ifc_options_level_of_detail.pyi` & `cwapi3d-30.498.0/src/cadwork/ifc_options_level_of_detail.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/ifc_options_project_data.pyi` & `cwapi3d-30.498.0/src/cadwork/ifc_options_project_data.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/ifc_options_properties.pyi` & `cwapi3d-30.498.0/src/cadwork/ifc_options_properties.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/ifc_predefined_type.pyi` & `cwapi3d-30.498.0/src/cadwork/ifc_predefined_type.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/import_3dc_options.pyi` & `cwapi3d-30.498.0/src/cadwork/import_3dc_options.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/layer_settings.pyi` & `cwapi3d-30.498.0/src/cadwork/layer_settings.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/point_3d.pyi` & `cwapi3d-30.498.0/src/cadwork/point_3d.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/process_type.pyi` & `cwapi3d-30.498.0/src/cadwork/process_type.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/rhino_options.pyi` & `cwapi3d-30.498.0/src/cadwork/rhino_options.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/text_object_options.pyi` & `cwapi3d-30.498.0/src/cadwork/text_object_options.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cadwork/window_geometry.pyi` & `cwapi3d-30.498.0/src/cadwork/window_geometry.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/connector_axis_controller/__init__.pyi` & `cwapi3d-30.498.0/src/connector_axis_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/cwapi3d.egg-info/PKG-INFO` & `cwapi3d-30.498.0/src/cwapi3d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwapi3d
-Version: 30.444.0
+Version: 30.498.0
 Summary: Python bindings for CwAPI3D
 Author-email: Cadwork <it@cadwork.ca>
 License: MIT License
         
         Copyright (c) 2024 Cadwork
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cwapi3d-30.444.0/src/cwapi3d.egg-info/SOURCES.txt` & `cwapi3d-30.498.0/src/cwapi3d.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/cadwork/ifc_options_aggregation.pyi
 src/cadwork/ifc_options_level_of_detail.pyi
 src/cadwork/ifc_options_project_data.pyi
 src/cadwork/ifc_options_properties.pyi
 src/cadwork/ifc_predefined_type.pyi
 src/cadwork/import_3dc_options.pyi
 src/cadwork/layer_settings.pyi
+src/cadwork/multi_layer_type.pyi
 src/cadwork/node_symbol.pyi
 src/cadwork/point_3d.pyi
 src/cadwork/polygon_list.pyi
 src/cadwork/process_type.pyi
 src/cadwork/projection_type.pyi
 src/cadwork/rhino_options.pyi
 src/cadwork/shortcut_key.pyi
```

### Comparing `cwapi3d-30.444.0/src/dimension_controller/__init__.pyi` & `cwapi3d-30.498.0/src/dimension_controller/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -152,16 +152,14 @@
     Parameters:
         element: element
 
     Returns:
         double
     """
 
-from cadwork import point_3d
-
 def get_distance(element: int) -> point_3d:
     """Get the distance to the dimension reference point. The point is in the plane of the dimensioning.
 
     Parameters:
         element: element
 
     Returns:
@@ -205,7 +203,18 @@
         element: element
         segment_index: segment_index
 
     Returns:
         distance
     """
 
+def get_segment_direction(element: int, segment_index: int) -> point_3d:
+    """get segment direction
+
+    Parameters:
+        element: element
+        segment_index: segment_index
+
+    Returns:
+        point_3d
+    """
+
```

### Comparing `cwapi3d-30.444.0/src/element_controller/__init__.pyi` & `cwapi3d-30.498.0/src/element_controller/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1920,8 +1920,46 @@
         on_start_face: on_start_face
         on_end_face: on_end_face
 
     Returns:
         None
     """
 
+def create_truncated_cone_beam_points(start_diameter: float, end_diameter: float, p1: point_3d, p2: point_3d, p3: point_3d) -> int:
+    """create truncated cone beam points
+
+    Parameters:
+        start_diameter: start_diameter
+        end_diameter: end_diameter
+        p1: p1
+        p2: p2
+        p3: p3
+
+    Returns:
+        int
+    """
+
+def create_truncated_cone_beam_vectors(start_diameter: float, end_diameter: float, length: float, p1: point_3d, xl: point_3d, zl: point_3d) -> int:
+    """create truncated cone beam vectors
+
+    Parameters:
+        start_diameter: start_diameter
+        end_diameter: end_diameter
+        length: length
+        p1: p1
+        xl: xl
+        zl: zl
+
+    Returns:
+        int
+    """
+
+def create_spline_line(spline_points: None) -> int:
+    """create spline line
+
+    Parameters:
+        spline_points: spline_points
+
+    Returns:
+        int
+    """
```

### Comparing `cwapi3d-30.444.0/src/endtype_controller/__init__.pyi` & `cwapi3d-30.498.0/src/endtype_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/file_controller/__init__.pyi` & `cwapi3d-30.498.0/src/file_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/geometry_controller/__init__.pyi` & `cwapi3d-30.498.0/src/geometry_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/list_controller/__init__.pyi` & `cwapi3d-30.498.0/src/list_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/machine_controller/__init__.pyi` & `cwapi3d-30.498.0/src/machine_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/material_controller/__init__.pyi` & `cwapi3d-30.498.0/src/material_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/multi_layer_cover_controller/__init__.pyi` & `cwapi3d-30.498.0/src/multi_layer_cover_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/roof_controller/__init__.pyi` & `cwapi3d-30.498.0/src/roof_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/scene_controller/__init__.pyi` & `cwapi3d-30.498.0/src/scene_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/shop_drawing_controller/__init__.pyi` & `cwapi3d-30.498.0/src/shop_drawing_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-30.444.0/src/utility_controller/__init__.pyi` & `cwapi3d-30.498.0/src/utility_controller/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1053,7 +1053,40 @@
 def get_project_data_keys() -> List[str]:
     """get project data keys
 
     Returns:
         List[str]
     """
 
+def get_user_int_with_default_value(message: str, default_value: int) -> int:
+    """get user int with default value
+
+    Parameters:
+        message: message
+        default_value: default_value
+
+    Returns:
+        int
+    """
+
+def get_user_double_with_default_value(message: str, default_value: float) -> float:
+    """get user double with default value
+
+    Parameters:
+        message: message
+        default_value: default_value
+
+    Returns:
+        float
+    """
+
+def get_user_string_with_default_value(message: str, default_value: str) -> str:
+    """get user string with default value
+
+    Parameters:
+        message: message
+        default_value: default_value
+
+    Returns:
+        str
+    """
+
```

### Comparing `cwapi3d-30.444.0/src/visualization_controller/__init__.pyi` & `cwapi3d-30.498.0/src/visualization_controller/__init__.pyi`

 * *Files identical despite different names*

