# Comparing `tmp/adaptix-3.0.0b5.tar.gz` & `tmp/adaptix-3.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptix-3.0.0b5.tar", last modified: Sat Apr 20 08:07:26 2024, max compression
+gzip compressed data, was "adaptix-3.0.0b6.tar", last modified: Thu May 23 14:57:23 2024, max compression
```

## Comparing `adaptix-3.0.0b5.tar` & `adaptix-3.0.0b6.tar`

### file list

```diff
@@ -1,149 +1,155 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.543075 adaptix-3.0.0b5/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11357 2021-06-13 21:15:36.000000 adaptix-3.0.0b5/LICENSE
--rw-r--r--   0 pavel     (1000) pavel     (1000)     6741 2024-04-20 08:07:26.543075 adaptix-3.0.0b5/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4539 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/README.md
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5162 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/pyproject.toml
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2024-04-20 08:07:26.543075 adaptix-3.0.0b5/setup.cfg
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.527075 adaptix-3.0.0b5/src/
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2128 2024-03-30 13:12:56.000000 adaptix-3.0.0b5/src/adaptix/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/_internal/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      619 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/ast_templater.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3045 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/cascade_namespace.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2920 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/code_builder.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2634 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/compiler.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      558 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/name_sanitizer.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2718 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      639 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/common.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      322 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/compat.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/_internal/conversion/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/_internal/conversion/broaching/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/broaching/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7760 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/broaching/code_generator.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1187 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/broaching/definitions.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10709 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/coercer_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6976 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/converter_provider.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      749 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/checker.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2311 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/func.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3855 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6216 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2661 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/linking_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11225 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/model_coercer_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      594 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/policy_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1068 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/provider_template.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1928 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/request_cls.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7757 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/datastructures.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      108 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/definitions.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5460 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/feature_requirement.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/_internal/integrations/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/integrations/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/integrations/pydantic/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/integrations/pydantic/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6017 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/integrations/pydantic/native.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10048 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/definitions.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4861 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/attrs.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3484 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/callable.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      497 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/class_init.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3810 2024-04-20 08:03:28.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/dataclass.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2207 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/named_tuple.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     8028 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/pydantic.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7912 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/sqlalchemy.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4342 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/typed_dict.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/morphing/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    13218 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/concrete_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    12270 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/constant_length_tuple_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10886 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/dict_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    12333 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/enum_provider.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      618 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/func.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    16413 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     9701 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    18431 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/generic_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10078 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/iterable_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3869 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/load_error.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7579 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/basic_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4313 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/crown_definitions.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    23272 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/dumper_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6031 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/dumper_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    28138 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/loader_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7907 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/loader_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      696 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/request_filtering.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2313 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/base.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    16012 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/component.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5803 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/crown_builder.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4034 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/name_mapping.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4223 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2492 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/provider_template.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      281 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/request_cls.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2875 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/name_style.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/_internal/provider/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6700 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/essential.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/_internal/provider/facade/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/facade/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      757 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/facade/provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      905 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/fields.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    12210 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/loc_stack_filtering.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1818 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/location.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4226 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/overlay_schema.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1586 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/provider_template.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3878 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/provider_wrapper.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1535 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/request_cls.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7985 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/shape_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6268 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/static_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/py.typed
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/_internal/retort/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/retort/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3210 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/retort/base_retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3159 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/retort/mediator.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6653 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/retort/operating_retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5812 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/retort/routing.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      723 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/special_cases_optimization.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3063 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/struct_trail.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      609 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4141 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/basic_utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      994 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/constants.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1530 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/fundamentals.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3907 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/generic_resolver.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1828 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/implicit_params.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1059 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/norm_utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    25528 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/normalize_type.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5928 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/utils.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/conversion/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      678 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/conversion/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/integrations/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/integrations/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/integrations/pydantic/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      113 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/integrations/pydantic/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1564 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/load_error.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/provider/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      472 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/provider/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/py.typed
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      232 2024-03-30 13:12:41.000000 adaptix-3.0.0b5/src/adaptix/retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      386 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/struct_trail.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix.egg-info/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     6741 2024-04-20 08:07:26.000000 adaptix-3.0.0b5/src/adaptix.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5593 2024-04-20 08:07:26.000000 adaptix-3.0.0b5/src/adaptix.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2024-04-20 08:07:26.000000 adaptix-3.0.0b5/src/adaptix.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      309 2024-04-20 08:07:26.000000 adaptix-3.0.0b5/src/adaptix.egg-info/requires.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        8 2024-04-20 08:07:26.000000 adaptix-3.0.0b5/src/adaptix.egg-info/top_level.txt
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/tests/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1838 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/tests/test_doc.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      237 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/tests/test_meta.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.085499 adaptix-3.0.0b6/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    11357 2021-06-13 21:15:36.000000 adaptix-3.0.0b6/LICENSE
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     6741 2024-05-23 14:57:23.085499 adaptix-3.0.0b6/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4539 2024-05-23 14:54:25.000000 adaptix-3.0.0b6/README.md
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5162 2024-05-23 14:54:25.000000 adaptix-3.0.0b6/pyproject.toml
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2024-05-23 14:57:23.085499 adaptix-3.0.0b6/setup.cfg
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.065498 adaptix-3.0.0b6/src/
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.069499 adaptix-3.0.0b6/src/adaptix/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2128 2024-03-30 13:12:56.000000 adaptix-3.0.0b6/src/adaptix/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.069499 adaptix-3.0.0b6/src/adaptix/_internal/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.073499 adaptix-3.0.0b6/src/adaptix/_internal/code_tools/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/code_tools/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      619 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/code_tools/ast_templater.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3045 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/code_tools/cascade_namespace.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2920 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/code_tools/code_builder.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2634 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/code_tools/compiler.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      558 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/code_tools/name_sanitizer.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2718 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/code_tools/utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      639 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/common.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      322 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/compat.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.073499 adaptix-3.0.0b6/src/adaptix/_internal/conversion/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.073499 adaptix-3.0.0b6/src/adaptix/_internal/conversion/broaching/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/broaching/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7760 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/broaching/code_generator.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1187 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/broaching/definitions.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10707 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/coercer_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6978 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/converter_provider.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.073499 adaptix-3.0.0b6/src/adaptix/_internal/conversion/facade/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/facade/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      749 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/facade/checker.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2311 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/facade/func.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4545 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/facade/provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6216 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/facade/retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6842 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/linking_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    13645 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/model_coercer_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      594 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/policy_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1068 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/provider_template.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2319 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/request_cls.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      575 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/conversion/request_filtering.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7759 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/datastructures.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      108 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/definitions.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5460 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/feature_requirement.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.073499 adaptix-3.0.0b6/src/adaptix/_internal/integrations/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/integrations/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.073499 adaptix-3.0.0b6/src/adaptix/_internal/integrations/pydantic/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/integrations/pydantic/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6017 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/integrations/pydantic/native.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.073499 adaptix-3.0.0b6/src/adaptix/_internal/integrations/sqlalchemy/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/integrations/sqlalchemy/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1754 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/integrations/sqlalchemy/orm.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.073499 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10048 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/definitions.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.073499 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4861 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/attrs.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3484 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/callable.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      497 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/class_init.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3810 2024-04-20 08:03:28.000000 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/dataclass.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2207 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/named_tuple.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8028 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/pydantic.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8022 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/sqlalchemy.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4342 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/typed_dict.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.077499 adaptix-3.0.0b6/src/adaptix/_internal/morphing/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    13218 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/concrete_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    12270 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/constant_length_tuple_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10886 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/dict_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    12532 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/enum_provider.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.077499 adaptix-3.0.0b6/src/adaptix/_internal/morphing/facade/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/facade/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      618 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/facade/func.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    16390 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/facade/provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     9701 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/facade/retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    18431 2024-04-28 13:34:24.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/generic_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10078 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/iterable_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3869 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/load_error.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.077499 adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7579 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/basic_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4313 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/crown_definitions.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    23272 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/dumper_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6031 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/dumper_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    28819 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/loader_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7907 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/loader_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      696 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/request_filtering.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.077499 adaptix-3.0.0b6/src/adaptix/_internal/morphing/name_layout/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/name_layout/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2313 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/name_layout/base.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    16012 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/name_layout/component.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5803 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/name_layout/crown_builder.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4034 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/name_layout/name_mapping.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4223 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/name_layout/provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2492 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/provider_template.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      281 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/morphing/request_cls.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2875 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/name_style.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.081499 adaptix-3.0.0b6/src/adaptix/_internal/provider/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6700 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/essential.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.081499 adaptix-3.0.0b6/src/adaptix/_internal/provider/facade/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/facade/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      757 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/facade/provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      905 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/fields.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    12210 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/loc_stack_filtering.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2381 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/location.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4226 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/overlay_schema.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1586 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/provider_template.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3878 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/provider_wrapper.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2498 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/request_cls.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7985 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/shape_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6268 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/provider/static_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/py.typed
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.081499 adaptix-3.0.0b6/src/adaptix/_internal/retort/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/retort/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3210 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/retort/base_retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3159 2024-05-09 19:46:06.000000 adaptix-3.0.0b6/src/adaptix/_internal/retort/mediator.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5857 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/_internal/retort/operating_retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5812 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/retort/routing.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      723 2024-04-28 13:34:24.000000 adaptix-3.0.0b6/src/adaptix/_internal/special_cases_optimization.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3063 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/struct_trail.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.081499 adaptix-3.0.0b6/src/adaptix/_internal/type_tools/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      609 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/type_tools/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4141 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/type_tools/basic_utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      994 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/type_tools/constants.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1530 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/type_tools/fundamentals.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3907 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/type_tools/generic_resolver.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1828 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/type_tools/implicit_params.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1059 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/_internal/type_tools/norm_utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    25528 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/_internal/type_tools/normalize_type.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5928 2024-03-30 13:54:05.000000 adaptix-3.0.0b6/src/adaptix/_internal/utils.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.081499 adaptix-3.0.0b6/src/adaptix/conversion/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      718 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/conversion/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.081499 adaptix-3.0.0b6/src/adaptix/integrations/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/integrations/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.081499 adaptix-3.0.0b6/src/adaptix/integrations/pydantic/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      113 2024-04-20 08:07:18.000000 adaptix-3.0.0b6/src/adaptix/integrations/pydantic/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.081499 adaptix-3.0.0b6/src/adaptix/integrations/sqlalchemy/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      104 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/src/adaptix/integrations/sqlalchemy/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1564 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/load_error.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.085499 adaptix-3.0.0b6/src/adaptix/provider/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      472 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/provider/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/py.typed
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      232 2024-03-30 13:12:41.000000 adaptix-3.0.0b6/src/adaptix/retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      386 2024-03-17 07:48:08.000000 adaptix-3.0.0b6/src/adaptix/struct_trail.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.085499 adaptix-3.0.0b6/src/adaptix.egg-info/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     6741 2024-05-23 14:57:23.000000 adaptix-3.0.0b6/src/adaptix.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5806 2024-05-23 14:57:23.000000 adaptix-3.0.0b6/src/adaptix.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2024-05-23 14:57:23.000000 adaptix-3.0.0b6/src/adaptix.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      309 2024-05-23 14:57:23.000000 adaptix-3.0.0b6/src/adaptix.egg-info/requires.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        8 2024-05-23 14:57:23.000000 adaptix-3.0.0b6/src/adaptix.egg-info/top_level.txt
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-05-23 14:57:23.085499 adaptix-3.0.0b6/tests/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2290 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/tests/test_doc.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      755 2024-05-23 14:28:07.000000 adaptix-3.0.0b6/tests/test_meta.py
```

### Comparing `adaptix-3.0.0b5/LICENSE` & `adaptix-3.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/PKG-INFO` & `adaptix-3.0.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptix
-Version: 3.0.0b5
+Version: 3.0.0b6
 Summary: An extremely flexible and configurable data model conversion library
 Author-email: "A. Tikhonov" <17@itishka.org>
 Project-URL: Homepage, https://github.com/reagento/adaptix
 Project-URL: Bug Tracker, https://github.com/reagento/adaptix/issues
 Project-URL: Documentation, https://adaptix.readthedocs.io/en/latest/
 Project-URL: Changelog, https://adaptix.readthedocs.io/en/latest/reference/changelog.html
 Project-URL: Source, https://github.com/reagento/adaptix/
@@ -34,24 +34,24 @@
 Provides-Extra: attrs
 Requires-Dist: attrs>=21.3.0; extra == "attrs"
 Provides-Extra: attrs-strict
 Requires-Dist: attrs<=23.2.0,>=21.3.0; extra == "attrs-strict"
 Provides-Extra: sqlalchemy
 Requires-Dist: sqlalchemy>=2.0.0; extra == "sqlalchemy"
 Provides-Extra: sqlalchemy-strict
-Requires-Dist: sqlalchemy<=2.0.29,>=2.0.0; extra == "sqlalchemy-strict"
+Requires-Dist: sqlalchemy<=2.0.30,>=2.0.0; extra == "sqlalchemy-strict"
 Provides-Extra: pydantic
 Requires-Dist: pydantic>=2.0.0; extra == "pydantic"
 Provides-Extra: pydantic-strict
-Requires-Dist: pydantic<=2.7.0,>=2.0.0; extra == "pydantic-strict"
+Requires-Dist: pydantic<=2.7.1,>=2.0.0; extra == "pydantic-strict"
 
 <div align="center">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b5/docs/logo/adaptix-with-title-dark.png?raw=true">
-    <source media="(prefers-color-scheme: light)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b5/docs/logo/adaptix-with-title-light.png?raw=true">
+    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b6/docs/logo/adaptix-with-title-dark.png?raw=true">
+    <source media="(prefers-color-scheme: light)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b6/docs/logo/adaptix-with-title-light.png?raw=true">
     <img alt="adaptix logo" src="https://raw.githubusercontent.com/reagento/adaptix/v3.0.0b2/docs/logo/adaptix-with-title-light.png?raw=true">
   </picture>
 
   <hr>
 
   [![PyPI version](https://img.shields.io/pypi/v/adaptix.svg?color=blue)](https://pypi.org/project/adaptix/)
   [![downloads](https://img.shields.io/pypi/dm/adaptix.svg)](https://pypistats.org/packages/adaptix)
@@ -67,15 +67,15 @@
 
 📚 [Documentation](https://adaptix.readthedocs.io/)
 
 ## TL;DR
 
 Install
 ```bash
-pip install adaptix==3.0.0b5
+pip install adaptix==3.0.0b6
 ```
 
 Use for model loading and dumping.
 
 ```python
 from dataclasses import dataclass
```

### Comparing `adaptix-3.0.0b5/README.md` & `adaptix-3.0.0b6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div align="center">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b5/docs/logo/adaptix-with-title-dark.png?raw=true">
-    <source media="(prefers-color-scheme: light)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b5/docs/logo/adaptix-with-title-light.png?raw=true">
+    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b6/docs/logo/adaptix-with-title-dark.png?raw=true">
+    <source media="(prefers-color-scheme: light)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b6/docs/logo/adaptix-with-title-light.png?raw=true">
     <img alt="adaptix logo" src="https://raw.githubusercontent.com/reagento/adaptix/v3.0.0b2/docs/logo/adaptix-with-title-light.png?raw=true">
   </picture>
 
   <hr>
 
   [![PyPI version](https://img.shields.io/pypi/v/adaptix.svg?color=blue)](https://pypi.org/project/adaptix/)
   [![downloads](https://img.shields.io/pypi/dm/adaptix.svg)](https://pypistats.org/packages/adaptix)
@@ -21,15 +21,15 @@
 
 📚 [Documentation](https://adaptix.readthedocs.io/)
 
 ## TL;DR
 
 Install
 ```bash
-pip install adaptix==3.0.0b5
+pip install adaptix==3.0.0b6
 ```
 
 Use for model loading and dumping.
 
 ```python
 from dataclasses import dataclass
```

### Comparing `adaptix-3.0.0b5/pyproject.toml` & `adaptix-3.0.0b6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools==69.1.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'adaptix'
-version = '3.0.0b5'
+version = '3.0.0b6'
 description = 'An extremely flexible and configurable data model conversion library'
 readme = 'README.md'
 requires-python = '>=3.8'
 dependencies = [
     'exceptiongroup>=1.1.3; python_version<"3.11"',
     'astunparse>=1.6.3; python_version<="3.8"',
 ]
@@ -33,17 +33,17 @@
     'Topic :: Internet',
 ]
 
 [project.optional-dependencies]
 attrs = ['attrs >= 21.3.0']
 attrs-strict = ['attrs >= 21.3.0, <= 23.2.0']
 sqlalchemy = ['sqlalchemy >= 2.0.0']
-sqlalchemy-strict = ['sqlalchemy >= 2.0.0, <= 2.0.29']
+sqlalchemy-strict = ['sqlalchemy >= 2.0.0, <= 2.0.30']
 pydantic = ['pydantic >= 2.0.0']
-pydantic-strict = ['pydantic >= 2.0.0, <= 2.7.0']
+pydantic-strict = ['pydantic >= 2.0.0, <= 2.7.1']
 
 [project.urls]
 'Homepage' = 'https://github.com/reagento/adaptix'
 'Bug Tracker' = 'https://github.com/reagento/adaptix/issues'
 'Documentation' = 'https://adaptix.readthedocs.io/en/latest/'
 'Changelog' = 'https://adaptix.readthedocs.io/en/latest/reference/changelog.html'
 'Source' = 'https://github.com/reagento/adaptix/'
```

### Comparing `adaptix-3.0.0b5/src/adaptix/__init__.py` & `adaptix-3.0.0b6/src/adaptix/__init__.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/code_tools/ast_templater.py` & `adaptix-3.0.0b6/src/adaptix/_internal/code_tools/ast_templater.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/code_tools/cascade_namespace.py` & `adaptix-3.0.0b6/src/adaptix/_internal/code_tools/cascade_namespace.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/code_tools/code_builder.py` & `adaptix-3.0.0b6/src/adaptix/_internal/code_tools/code_builder.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/code_tools/compiler.py` & `adaptix-3.0.0b6/src/adaptix/_internal/code_tools/compiler.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/code_tools/name_sanitizer.py` & `adaptix-3.0.0b6/src/adaptix/_internal/code_tools/name_sanitizer.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/code_tools/utils.py` & `adaptix-3.0.0b6/src/adaptix/_internal/code_tools/utils.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/common.py` & `adaptix-3.0.0b6/src/adaptix/_internal/common.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/conversion/broaching/code_generator.py` & `adaptix-3.0.0b6/src/adaptix/_internal/conversion/broaching/code_generator.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/conversion/broaching/definitions.py` & `adaptix-3.0.0b6/src/adaptix/_internal/conversion/broaching/definitions.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/conversion/coercer_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/conversion/coercer_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,22 +217,22 @@
         def iterable_coercer(data, ctx):
             return dst_factory(element_coercer(element, ctx) for element in data)
 
         return iterable_coercer
 
     def _parse_source(self, norm: BaseNormType) -> TypeHint:
         if norm.origin == tuple and norm.args[-1] != Ellipsis:
-            raise CannotProvide("Constant-length tuple is not suppoerted yet", is_demonstrative=True)
+            raise CannotProvide("Constant-length tuple is not supported yet", is_demonstrative=True)
         if norm.origin in self.CONCRETE_ORIGINS or norm.origin in self.ABC_TO_IMPL:
             return norm.args[0].source
         raise CannotProvide
 
     def _parse_destination(self, norm: BaseNormType) -> Tuple[Callable, TypeHint]:
         if norm.origin == tuple and norm.args[-1] != Ellipsis:
-            raise CannotProvide("Constant-length tuple is not suppoerted yet", is_demonstrative=True)
+            raise CannotProvide("Constant-length tuple is not supported yet", is_demonstrative=True)
         if norm.origin in self.CONCRETE_ORIGINS:
             return norm.origin, norm.args[0].source
         if norm.origin in self.ABC_TO_IMPL:
             return self.ABC_TO_IMPL[norm.origin], norm.args[0].source
         raise CannotProvide
```

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/conversion/converter_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/conversion/converter_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             code_gen_hook=fetch_code_gen_hook(mediator, LocStack(dst_loc)),
             namespace=dumper_namespace,
             closure_code=dumper_code,
             closure_name=closure_name,
             file_name=self._get_file_name(request),
         )
 
-    def register_mangled(self, namespace: CascadeNamespace, base: str, obj: object) -> str:
+    def _register_mangled(self, namespace: CascadeNamespace, base: str, obj: object) -> str:
         base = self._name_sanitizer.sanitize(base)
         if namespace.try_add_constant(base, obj):
             return base
 
         for i in itertools.count(1):
             name = f"{base}_{i}"
             if namespace.try_add_constant(name, obj):
@@ -86,15 +86,15 @@
         coercer: Coercer,
     ) -> Tuple[str, Mapping[str, object]]:
         builder = CodeBuilder()
         namespace = BuiltinCascadeNamespace(occupied=signature.parameters.keys())
         namespace.add_outer_constant("_closure_signature", signature)
         namespace.add_outer_constant("_stub_function", stub_function)
         namespace.add_outer_constant("_update_wrapper", update_wrapper)
-        coercer_var = self.register_mangled(namespace, "coercer", coercer)
+        coercer_var = self._register_mangled(namespace, "coercer", coercer)
 
         no_types_signature = signature.replace(
             parameters=[param.replace(annotation=Signature.empty) for param in signature.parameters.values()],
             return_annotation=Signature.empty,
         )
         parameters = tuple(signature.parameters.values())
         ctx_passing = self._get_ctx_passing(parameters[1:])
```

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/checker.py` & `adaptix-3.0.0b6/src/adaptix/_internal/conversion/facade/checker.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/func.py` & `adaptix-3.0.0b6/src/adaptix/_internal/conversion/facade/func.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/conversion/facade/provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import Any, Callable, Optional, overload
 
 from ...common import OneArgCoercer
 from ...model_tools.definitions import DefaultFactory, DefaultValue
 from ...provider.essential import Provider
 from ...provider.facade.provider import bound_by_any
-from ...provider.loc_stack_filtering import LocStackChecker, LocStackSizeChecker, Pred, create_loc_stack_checker
+from ...provider.loc_stack_filtering import LocStackChecker, Pred, create_loc_stack_checker
 from ..coercer_provider import MatchingCoercerProvider
-from ..linking_provider import ConstantLinkingProvider, MatchingLinkingProvider
+from ..linking_provider import ConstantLinkingProvider, FunctionLinkingProvider, MatchingLinkingProvider
 from ..policy_provider import UnlinkedOptionalPolicyProvider
+from ..request_filtering import FromCtxParam
 
 
 def link(src: Pred, dst: Pred, *, coercer: Optional[OneArgCoercer] = None) -> Provider:
     """Basic provider to define custom linking between fields.
 
     :param src: Predicate specifying source point of linking. See :ref:`predicate-system` for details.
     :param dst: Predicate specifying destination point of linking. See :ref:`predicate-system` for details.
@@ -46,14 +47,33 @@
     """
     return ConstantLinkingProvider(
         create_loc_stack_checker(dst),
         DefaultFactory(factory) if factory is not None else DefaultValue(value),
     )
 
 
+def link_function(func: Callable, dst: Pred) -> Provider:
+    """Provider that uses function to produce value of destination field.
+
+    The entire model is passed to the first parameter of the function.
+    The type of result and first parameter are not checked, you must ensure type compatibility yourself.
+
+    Keyword-only parameters link to model fields and other parameters link to extra converter parameters.
+    After linking, the default type coercing mechanism is applied.
+
+    :param func: A function used to process several fields of source model.
+    :param dst: Predicate specifying destination point of linking. See :ref:`predicate-system` for details.
+    :return: Desired provider
+    """
+    return FunctionLinkingProvider(
+        func=func,
+        dst_lsc=create_loc_stack_checker(dst),
+    )
+
+
 def coercer(src: Pred, dst: Pred, func: OneArgCoercer) -> Provider:
     """Basic provider to define custom coercer.
 
     :param src: Predicate specifying source point of linking. See :ref:`predicate-system` for details.
     :param dst: Predicate specifying destination point of linking. See :ref:`predicate-system` for details.
     :param func: The function is used to transform input data to a destination type.
     :return: Desired provider
@@ -85,10 +105,8 @@
     :return: Desired provider.
     """
     return bound_by_any(preds, UnlinkedOptionalPolicyProvider(is_allowed=False))
 
 
 def from_param(param_name: str) -> LocStackChecker:
     """The special predicate form matching only top-level parameters by name"""
-    if not param_name.isidentifier():
-        raise ValueError("param_name must be a valid python identifier to exactly match parameter")
-    return LocStackSizeChecker(1) & create_loc_stack_checker(param_name)
+    return FromCtxParam(param_name)
```

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/retort.py` & `adaptix-3.0.0b6/src/adaptix/_internal/conversion/facade/retort.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/conversion/model_coercer_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/conversion/model_coercer_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from inspect import Parameter, Signature
-from typing import Iterable, List, Mapping, Optional, Tuple
+from typing import Callable, Iterable, List, Mapping, Optional, Tuple, Union
 
 from ..code_tools.compiler import BasicClosureCompiler, ClosureCompiler
 from ..code_tools.name_sanitizer import BuiltinNameSanitizer, NameSanitizer
 from ..common import Coercer
 from ..conversion.broaching.code_generator import BroachingCodeGenerator, BroachingPlan, BuiltinBroachingCodeGenerator
 from ..conversion.broaching.definitions import (
     AccessorElement,
@@ -16,24 +16,26 @@
 )
 from ..conversion.request_cls import (
     CoercerRequest,
     ConstantLinking,
     ConversionDestItem,
     ConversionSourceItem,
     FieldLinking,
+    FunctionLinking,
     LinkingRequest,
     LinkingResult,
+    ModelLinking,
     UnlinkedOptionalPolicyRequest,
 )
 from ..model_tools.definitions import DefaultValue, InputField, InputShape, OutputShape, ParamKind, create_key_accessor
 from ..morphing.model.basic_gen import compile_closure_with_globals_capturing, fetch_code_gen_hook
 from ..provider.essential import CannotProvide, Mediator, mandatory_apply_by_iterable
 from ..provider.fields import input_field_to_loc, output_field_to_loc
-from ..provider.location import OutputFieldLoc
-from ..provider.request_cls import LocStack, TypeHintLoc
+from ..provider.location import AnyLoc, InputFieldLoc, InputFuncFieldLoc, OutputFieldLoc
+from ..provider.request_cls import LocStack
 from ..provider.shape_provider import InputShapeRequest, OutputShapeRequest, provide_generic_resolved_shape
 from ..utils import add_note
 from .provider_template import CoercerProvider
 
 
 class ModelCoercerProvider(CoercerProvider):
     def __init__(self, *, name_sanitizer: NameSanitizer = BuiltinNameSanitizer()):
@@ -72,22 +74,28 @@
             code_gen_hook=fetch_code_gen_hook(mediator, request.dst),
             namespace=dumper_namespace,
             closure_code=dumper_code,
             closure_name=closure_name,
             file_name=self._get_file_name(request),
         )
 
+    def _loc_stack_to_view_string(self, lock_stack: LocStack[AnyLoc]) -> str:
+        tp = lock_stack.last.type
+        if isinstance(tp, type):
+            return tp.__name__
+        return str(tp)
+
     def _get_closure_name(self, request: CoercerRequest) -> str:
-        src = request.src.last.cast(TypeHintLoc).type
-        dst = request.dst.last.cast(TypeHintLoc).type
+        src = self._loc_stack_to_view_string(request.src)
+        dst = self._loc_stack_to_view_string(request.dst)
         return self._name_sanitizer.sanitize(f"coerce_{src}_to_{dst}")
 
     def _get_file_name(self, request: CoercerRequest) -> str:
-        src = request.src.last.cast(TypeHintLoc).type
-        dst = request.dst.last.cast(TypeHintLoc).type
+        src = self._loc_stack_to_view_string(request.src)
+        dst = self._loc_stack_to_view_string(request.dst)
         return self._name_sanitizer.sanitize(f"coerce_{src}_to_{dst}")
 
     def _fetch_dst_shape(self, mediator: Mediator, loc_stack: LocStack[ConversionDestItem]) -> InputShape:
         return provide_generic_resolved_shape(
             mediator,
             InputShapeRequest(loc_stack=loc_stack),
         )
@@ -124,15 +132,16 @@
                         sources=sources,
                         context=request.ctx,
                         destination=destination,
                     ),
                 )
             except CannotProvide as e:
                 if dst_field.is_required:
-                    add_note(e, "Note: This is a required field, so it must take value")
+                    if not e.is_terminal:
+                        add_note(e, "Note: This is a required field, so it must take value")
                     raise
 
                 policy = mediator.mandatory_provide(
                     UnlinkedOptionalPolicyRequest(loc_stack=destination),
                 )
                 if policy.is_allowed:
                     return dst_field, None
@@ -147,29 +156,29 @@
 
         return mandatory_apply_by_iterable(
             fetch_field_linking,
             zip(dst_shape.fields),
             lambda: "Cannot create coercer for models. Linkings for some fields are not found",
         )
 
-    def _field_linking_to_sub_plan(
+    def _generate_field_linking_to_sub_plan(
         self,
         mediator: Mediator,
         request: CoercerRequest,
-        input_field: InputField,
+        loc: Union[InputFieldLoc, InputFuncFieldLoc],
         linking: FieldLinking,
     ) -> BroachingPlan:
         if linking.coercer is not None:
             coercer = linking.coercer
         else:
             coercer = mediator.provide(
                 CoercerRequest(
                     src=linking.source,
                     ctx=request.ctx,
-                    dst=request.dst.append_with(input_field_to_loc(input_field)),
+                    dst=request.dst.append_with(loc),
                 ),
             )
 
         return FunctionElement[BroachingPlan](
             func=coercer,
             args=(
                 PositionalArg(self._get_field_coercer_data_arg(mediator, request, linking)),
@@ -200,37 +209,88 @@
         mediator: Mediator,
         linking: ConstantLinking,
     ) -> BroachingPlan:
         if isinstance(linking.constant, DefaultValue):
             return ConstantElement(value=linking.constant.value)
         return FunctionElement(func=linking.constant.factory, args=())
 
-    def _generate_field_to_sub_plan(
+    def _generate_model_linking_to_sub_plan(
+        self,
+        mediator: Mediator,
+        linking: ModelLinking,
+    ) -> BroachingPlan:
+        return ParameterElement("data")
+
+    def _generate_function_linking_to_sub_plan(
+        self,
+        mediator: Mediator,
+        request: CoercerRequest,
+        linking: FunctionLinking,
+    ) -> BroachingPlan:
+        args: List[FuncCallArg[BroachingPlan]] = []
+        field_to_sub_plan = self._generate_sub_plan(
+            mediator,
+            request,
+            [(param_spec.field, param_spec.linking) for param_spec in linking.param_specs],
+            parent_func=linking.func,
+        )
+        for param_spec in linking.param_specs:
+            sub_plan = field_to_sub_plan[param_spec.field]
+            if param_spec.param_kind == ParamKind.KW_ONLY:
+                args.append(KeywordArg(param_spec.field.id, sub_plan))
+            else:
+                args.append(PositionalArg(sub_plan))
+
+        return FunctionElement(
+            func=linking.func,
+            args=tuple(args),
+        )
+
+    def _generate_sub_plan(
         self,
         mediator: Mediator,
         request: CoercerRequest,
         field_linkings: Iterable[Tuple[InputField, LinkingResult]],
+        parent_func: Optional[Callable],
     ) -> Mapping[InputField, BroachingPlan]:
         def generate_sub_plan(input_field: InputField, linking_result: LinkingResult):
             if isinstance(linking_result.linking, ConstantLinking):
                 return self._generate_constant_linking_to_sub_plan(
                     mediator=mediator,
                     linking=linking_result.linking,
                 )
-            return self._field_linking_to_sub_plan(
-                mediator=mediator,
-                request=request,
-                input_field=input_field,
-                linking=linking_result.linking,
-            )
+            if isinstance(linking_result.linking, FunctionLinking):
+                return self._generate_function_linking_to_sub_plan(
+                    mediator=mediator,
+                    request=request,
+                    linking=linking_result.linking,
+                )
+            if isinstance(linking_result.linking, ModelLinking):
+                return self._generate_model_linking_to_sub_plan(
+                    mediator=mediator,
+                    linking=linking_result.linking,
+                )
+            if isinstance(linking_result.linking, FieldLinking):
+                field_loc = input_field_to_loc(input_field)
+                return self._generate_field_linking_to_sub_plan(
+                    mediator=mediator,
+                    request=request,
+                    loc=field_loc.complement_with_func(parent_func) if parent_func is not None else field_loc,
+                    linking=linking_result.linking,
+                )
+            raise TypeError
 
         field_sub_plans = mandatory_apply_by_iterable(
             generate_sub_plan,
             field_linkings,
-            lambda: "Cannot create coercer for models. Coercers for some linkings are not found",
+            lambda: (
+                "Cannot create coercer for models. Coercers for some linkings are not found"
+                if parent_func is None else
+                "Cannot create coercer for model and function. Coercers for some linkings are not found"
+            ),
         )
         return {
             dst_field: sub_plan
             for (dst_field, linking), sub_plan in zip(field_linkings, field_sub_plans)
         }
 
     def _make_broaching_plan(
@@ -242,22 +302,23 @@
     ) -> BroachingPlan:
         field_linkings = self._fetch_linkings(
             mediator=mediator,
             request=request,
             dst_shape=dst_shape,
             src_shape=src_shape,
         )
-        field_to_sub_plan = self._generate_field_to_sub_plan(
+        field_to_sub_plan = self._generate_sub_plan(
             mediator=mediator,
             request=request,
             field_linkings=[
                 (dst_field, linking)
                 for dst_field, linking in field_linkings
                 if linking is not None
             ],
+            parent_func=None,
         )
         return self._make_constructor_call(
             dst_shape=dst_shape,
             field_to_linking=dict(field_linkings),
             field_to_sub_plan=field_to_sub_plan,
         )
```

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/conversion/policy_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/conversion/policy_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/conversion/provider_template.py` & `adaptix-3.0.0b6/src/adaptix/_internal/conversion/provider_template.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/datastructures.py` & `adaptix-3.0.0b6/src/adaptix/_internal/datastructures.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             if isinstance(obj, SupportsKeysAndGetItem):
                 for k in obj:
                     self[k] = obj[k]
             else:
                 for k, v in obj:
                     self[k] = v
 
-        if len(args) != 0:
+        elif len(args) != 0:
             raise ValueError
 
         for k, v in kwargs.items():
             self[k] = v
 
     def __repr__(self):
         return f"{type(self).__name__}({super().__repr__()})"
```

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/feature_requirement.py` & `adaptix-3.0.0b6/src/adaptix/_internal/feature_requirement.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/integrations/pydantic/native.py` & `adaptix-3.0.0b6/src/adaptix/_internal/integrations/pydantic/native.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/definitions.py` & `adaptix-3.0.0b6/src/adaptix/_internal/model_tools/definitions.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/attrs.py` & `adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/attrs.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/callable.py` & `adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/callable.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/dataclass.py` & `adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/dataclass.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/named_tuple.py` & `adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/named_tuple.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/pydantic.py` & `adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/pydantic.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/sqlalchemy.py` & `adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/sqlalchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                 field_id=column.key,
                 name=column.key,
                 kind=ParamKind.KW_ONLY,
             ),
         )
 
     for relationship in relationships:
-        if relationship.collection_class is not None:
+        if relationship.collection_class is not None and strip_alias(relationship.collection_class) != list:
             continue  # it is not supported
         if relationship.uselist is None:
             continue  # it cannot be None there
 
         fields.append(
             InputField(
                 id=relationship.key,
@@ -199,15 +199,15 @@
             original=IdWrapper(column),
             accessor=create_attr_accessor(column.name, is_required=True),
         )
         for column in columns
         if isinstance(column, sqlalchemy.Column)
     ]
     for relationship in relationships:
-        if relationship.collection_class is not None:
+        if relationship.collection_class is not None and strip_alias(relationship.collection_class) != list:
             continue  # it is not supported
         if relationship.uselist is None:
             continue  # it cannot be None there
 
         output_fields.append(
             OutputField(
                 id=relationship.key,
```

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/typed_dict.py` & `adaptix-3.0.0b6/src/adaptix/_internal/model_tools/introspection/typed_dict.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/concrete_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/concrete_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/constant_length_tuple_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/constant_length_tuple_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/dict_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/dict_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/enum_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/enum_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,18 +166,14 @@
 
         def enum_dumper(data):
             return value_dumper(data.value)
 
         return enum_dumper
 
 
-def _enum_exact_value_dumper(data):
-    return data.value
-
-
 class EnumExactValueProvider(BaseEnumProvider):
     """This provider represents enum members to the outside world
     by their value without any processing
     """
 
     def _provide_loader(self, mediator: Mediator, request: LoaderRequest) -> Loader:
         return self._make_loader(get_type_from_request(request))
@@ -207,25 +203,30 @@
             except TypeError:
                 raise BadVariantLoadError(variants, data)
 
         return enum_exact_loader_v2m
 
     def _get_exact_value_to_member(self, enum: Type[Enum]) -> Optional[Mapping[Any, Any]]:
         try:
-            value_to_member = {case.value: case for case in enum}
+            value_to_member = {member.value: member for member in enum}
         except TypeError:
             return None
 
         if getattr(enum._missing_, "__func__", None) != Enum._missing_.__func__:  # type: ignore[attr-defined]
             return None
 
         return value_to_member
 
     def _provide_dumper(self, mediator: Mediator, request: DumperRequest) -> Dumper:
-        return _enum_exact_value_dumper
+        member_to_value = {member: member.value for member in get_type_from_request(request)}
+
+        def enum_exact_value_dumper(data):
+            return member_to_value[data]
+
+        return enum_exact_value_dumper
 
 
 class FlagByExactValueProvider(BaseFlagProvider):
     def _provide_loader(self, mediator: Mediator, request: LoaderRequest) -> Loader:
         enum = get_type_from_request(request)
         flag_mask = reduce(or_, enum.__members__.values()).value
 
@@ -241,28 +242,31 @@
             raise CannotProvide(
                 "Cannot create a loader for flag with skipped bits",
                 is_terminal=True,
                 is_demonstrative=True,
             )
 
         def flag_loader(data):
-            if type(data) is not int: # noqa: E721
+            if type(data) is not int:  # noqa: E721
                 raise TypeLoadError(int, data)
 
             if data < 0 or data > flag_mask:
                 raise OutOfRangeLoadError(0, flag_mask, data)
 
             # data already has been validated for all edge cases
             # so enum lookup cannot raise an error
             return enum(data)
 
         return flag_loader
 
     def _provide_dumper(self, mediator: Mediator, request: DumperRequest) -> Dumper:
-        return _enum_exact_value_dumper
+        def flag_exact_value_dumper(data):
+            return data.value
+
+        return flag_exact_value_dumper
 
 
 def _extract_non_compound_cases_from_flag(enum: Type[FlagT]) -> Sequence[FlagT]:
     return [case for case in enum.__members__.values() if not math.log2(case.value) % 1]
 
 
 class FlagByListProvider(BaseFlagProvider):
```

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/func.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/facade/func.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/facade/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,14 +428,14 @@
             return data
         raise exception_factory(data)
 
     return loader(pred, validating_loader, chain)
 
 
 def default_dict(pred: Pred, default_factory: Callable) -> Provider:
-    """DefaultDict provider with overriden default_factory parameter
+    """Provider for ``defaultdict`` class
 
     :param pred: Predicate specifying where the provider should be used.
         See :ref:`predicate-system` for details.
-    :param default_factory: default_factory parameter of the defaultdict instance to be created by the loader
+    :param default_factory: default_factory parameter of the ``defaultdict`` instance to be created by the loader
     """
     return bound(pred, DefaultDictProvider(default_factory))
```

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/retort.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/facade/retort.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/generic_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/generic_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/iterable_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/iterable_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/load_error.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/load_error.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/basic_gen.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/basic_gen.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/crown_definitions.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/crown_definitions.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/dumper_gen.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/dumper_gen.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/dumper_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/dumper_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/loader_gen.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/loader_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,15 +392,15 @@
                 """,
             )
         else:
             state.builder(
                 f"raise {namer.with_trail(bad_type_load_error)}",
             )
 
-    def _gen_assigment_from_parent_data(
+    def _gen_assignment_from_parent_data(
         self,
         state: GenState,
         *,
         assign_to: str,
         on_lookup_error: Optional[str] = None,
     ):
         last_path_el = state.path[-1]
@@ -494,15 +494,15 @@
         }
 
     def _gen_dict_crown(self, state: GenState, crown: InpDictCrown):
         state.namespace.add_constant(state.v_known_keys, set(crown.map.keys()))
         state.namespace.add_constant(state.v_required_keys, self._get_dict_crown_required_keys(crown))
 
         if state.path:
-            self._gen_assigment_from_parent_data(state, assign_to=state.v_data)
+            self._gen_assignment_from_parent_data(state, assign_to=state.v_data)
             state.builder.empty_line()
 
         if self._can_collect_extra:
             state.builder += f"{state.v_extra} = {{}}"
         if self._debug_trail == DebugTrail.ALL:
             state.builder += f"{state.v_has_not_found_error} = False"
 
@@ -535,15 +535,15 @@
 
     def _gen_forbidden_sequence_check(self, state: GenState) -> None:
         with state.builder(f"if type({state.v_data}) is str:"):
             self._gen_raise_bad_type_error(state, f"ExcludedTypeLoadError(CollectionsSequence, str, {state.v_data})")
 
     def _gen_list_crown(self, state: GenState, crown: InpListCrown):
         if state.path:
-            self._gen_assigment_from_parent_data(state, assign_to=state.v_data)
+            self._gen_assignment_from_parent_data(state, assign_to=state.v_data)
             state.builder.empty_line()
 
         if self._can_collect_extra:
             list_literal: list = [
                 {} if isinstance(sub_crown, (InpFieldCrown, InpNoneCrown)) else None
                 for sub_crown in crown.map
             ]
@@ -594,15 +594,15 @@
             state.namespace.add_constant(f"dfl_{field.id}", field.default.factory)
             return f"dfl_{field.id}()"
         raise ValueError
 
     def _gen_field_crown(self, state: GenState, crown: InpFieldCrown):
         field = state.get_field(crown)
         if field.is_required:
-            self._gen_assigment_from_parent_data(
+            self._gen_assignment_from_parent_data(
                 state=state,
                 assign_to=state.v_raw_field(field),
             )
             with state.builder("else:"):
                 self._gen_field_assigment(
                     assign_to=state.v_field(field),
                     field_id=field.id,
@@ -615,15 +615,15 @@
                 assign_to = f"packed_fields[{param_name!r}]"
                 on_lookup_error = "pass"
             else:
                 assign_to = state.v_field(field)
                 on_lookup_error = f"{state.v_field(field)} = {self._get_default_clause_expr(state, field)}"
 
             if isinstance(state.path[-1], int):
-                self._gen_assigment_from_parent_data(
+                self._gen_assignment_from_parent_data(
                     state=state,
                     assign_to=state.v_raw_field(field),
                     on_lookup_error=on_lookup_error,
                 )
                 with state.builder("else:"):
                     self._gen_field_assigment(
                         assign_to=assign_to,
@@ -677,35 +677,51 @@
                 f"TypeLoadError(CollectionsMapping, {state.parent.v_data})",
                 namer=state.parent,
             )
             state.type_checked_type_paths.add(state.parent_path)
 
         self._gen_unexpected_exc_catching(state)
         with state.builder("else:"):
-            state.builder(
-                f"""
-                try:
-                    value = getter({state.path[-1]!r}, sentinel)
-                """,
-            )
-            self._gen_unexpected_exc_catching(state)
-            with state.builder("else:"):  # noqa: SIM117
+            if self._debug_trail == DebugTrail.DISABLE:
                 with state.builder(
                     f"""
+                    value = getter({state.path[-1]!r}, sentinel)
                     if value is sentinel:
                         {on_lookup_error}
                     else:
                     """,
                 ):
                     self._gen_field_assigment(
                         assign_to=assign_to,
                         field_id=field.id,
                         loader_arg="value",
                         state=state,
                     )
+            else:
+                state.builder(
+                    f"""
+                    try:
+                        value = getter({state.path[-1]!r}, sentinel)
+                    """,
+                )
+                self._gen_unexpected_exc_catching(state)
+                with state.builder("else:"):  # noqa: SIM117
+                    with state.builder(
+                        f"""
+                        if value is sentinel:
+                            {on_lookup_error}
+                        else:
+                        """,
+                    ):
+                        self._gen_field_assigment(
+                            assign_to=assign_to,
+                            field_id=field.id,
+                            loader_arg="value",
+                            state=state,
+                        )
 
     def _gen_field_assigment(
         self,
         assign_to: str,
         field_id: str,
         loader_arg: str,
         state: GenState,
```

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/loader_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/loader_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/request_filtering.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/model/request_filtering.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/base.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/name_layout/base.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/component.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/name_layout/component.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/crown_builder.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/name_layout/crown_builder.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/name_mapping.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/name_layout/name_mapping.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/name_layout/provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/morphing/provider_template.py` & `adaptix-3.0.0b6/src/adaptix/_internal/morphing/provider_template.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/name_style.py` & `adaptix-3.0.0b6/src/adaptix/_internal/name_style.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/provider/essential.py` & `adaptix-3.0.0b6/src/adaptix/_internal/provider/essential.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/provider/facade/provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/provider/facade/provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/provider/fields.py` & `adaptix-3.0.0b6/src/adaptix/_internal/provider/fields.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/provider/loc_stack_filtering.py` & `adaptix-3.0.0b6/src/adaptix/_internal/provider/loc_stack_filtering.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/provider/location.py` & `adaptix-3.0.0b6/src/adaptix/_internal/provider/location.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import Any, Callable, Mapping, Type, TypeVar, Union
+from typing import Any, Callable, Container, Dict, Mapping, Type, TypeVar, Union
 
 from ..common import TypeHint
 from ..model_tools.definitions import Accessor, Default
 
 T = TypeVar("T")
 
 
@@ -38,14 +38,19 @@
 
 @dataclass(frozen=True)
 class _InputFieldLoc(_FieldLoc):
     is_required: bool
 
 
 @dataclass(frozen=True)
+class _InputFuncFieldLoc(_FieldLoc):
+    func: Callable
+
+
+@dataclass(frozen=True)
 class _OutputFieldLoc(_FieldLoc):
     accessor: Accessor
 
 
 @dataclass(frozen=True)
 class _GenericParamLoc(_TypeHintLoc):
     generic_pos: int
@@ -56,27 +61,39 @@
 
 
 class FieldLoc(_FieldLoc):
     pass
 
 
 class InputFieldLoc(_InputFieldLoc):
+    def complement_with_func(self, func: Callable) -> "InputFuncFieldLoc":
+        return InputFuncFieldLoc(
+            type=self.type,
+            field_id=self.field_id,
+            default=self.default,
+            metadata=self.metadata,
+            func=func,
+        )
+
+
+class InputFuncFieldLoc(_InputFuncFieldLoc):
     pass
 
 
 class OutputFieldLoc(_OutputFieldLoc):
     pass
 
 
 class GenericParamLoc(_GenericParamLoc):
     pass
 
 
-_CAST_SOURCES = {
-    TypeHintLoc: {TypeHintLoc, FieldLoc, InputFieldLoc, OutputFieldLoc, GenericParamLoc},
-    FieldLoc: {FieldLoc, InputFieldLoc, OutputFieldLoc},
-    InputFieldLoc: (InputFieldLoc, ),
-    OutputFieldLoc: (OutputFieldLoc, ),
-    GenericParamLoc: (GenericParamLoc, ),
+_CAST_SOURCES: Dict[Any, Container[Any]] = {
+    TypeHintLoc: {TypeHintLoc, FieldLoc, InputFieldLoc, OutputFieldLoc, GenericParamLoc, InputFuncFieldLoc},
+    FieldLoc: {FieldLoc, InputFieldLoc, OutputFieldLoc, InputFuncFieldLoc},
+    InputFieldLoc: {InputFieldLoc, InputFuncFieldLoc},
+    InputFuncFieldLoc: {InputFuncFieldLoc},
+    OutputFieldLoc: {OutputFieldLoc},
+    GenericParamLoc: {GenericParamLoc},
 }
 
-AnyLoc = Union[TypeHintLoc, FieldLoc, InputFieldLoc, OutputFieldLoc, GenericParamLoc]
+AnyLoc = Union[TypeHintLoc, FieldLoc, InputFieldLoc, InputFuncFieldLoc, OutputFieldLoc, GenericParamLoc]
```

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/provider/overlay_schema.py` & `adaptix-3.0.0b6/src/adaptix/_internal/provider/overlay_schema.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/provider/provider_template.py` & `adaptix-3.0.0b6/src/adaptix/_internal/provider/provider_template.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/provider/provider_wrapper.py` & `adaptix-3.0.0b6/src/adaptix/_internal/provider/provider_wrapper.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/provider/request_cls.py` & `adaptix-3.0.0b6/src/adaptix/_internal/provider/request_cls.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,57 @@
 from dataclasses import dataclass, replace
 from typing import Tuple, TypeVar
 
 from ..common import TypeHint
 from ..datastructures import ImmutableStack
 from ..definitions import DebugTrail
-from ..type_tools import BaseNormType, normalize_type
+from ..type_tools import BaseNormType, is_parametrized, normalize_type
 from ..utils import pairs
 from .essential import CannotProvide, Request
-from .location import AnyLoc, FieldLoc, TypeHintLoc
+from .location import AnyLoc, FieldLoc, InputFuncFieldLoc, TypeHintLoc
 
 LocStackT = TypeVar("LocStackT", bound="LocStack")
 AnyLocT_co = TypeVar("AnyLocT_co", bound=AnyLoc, covariant=True)
 
 
 class LocStack(ImmutableStack[AnyLocT_co]):
     def replace_last_type(self: LocStackT, tp: TypeHint, /) -> LocStackT:
         return self.replace_last(replace(self.last, type=tp))
 
 
+def _format_type(tp: TypeHint) -> str:
+    if isinstance(tp, type) and not is_parametrized(tp):
+        return tp.__qualname__
+    str_tp = str(tp)
+    if str_tp.startswith("typing."):
+        return str_tp[7:]
+    return str_tp
+
+
+def format_loc_stack(loc_stack: LocStack[AnyLoc]) -> str:
+    fmt_tp = _format_type(loc_stack.last.type)
+
+    try:
+        field_loc = loc_stack.last.cast(FieldLoc)
+    except TypeError:
+        return fmt_tp
+    else:
+        fmt_field = f"{field_loc.field_id}: {fmt_tp}"
+
+    if loc_stack.last.is_castable(InputFuncFieldLoc):
+        func_field_loc = loc_stack.last.cast(InputFuncFieldLoc)
+        func_name = getattr(func_field_loc.func, "__qualname__", None) or repr(func_field_loc.func)
+        return f"{func_name}({fmt_field})"
+
+    if len(loc_stack) >= 2:  # noqa: PLR2004
+        src_owner = _format_type(loc_stack[-2].type)
+        return f"{src_owner}.{fmt_field}"
+    return fmt_tp
+
+
 T = TypeVar("T")
 
 
 @dataclass(frozen=True)
 class LocatedRequest(Request[T]):
     loc_stack: LocStack
```

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/provider/shape_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/provider/shape_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/provider/static_provider.py` & `adaptix-3.0.0b6/src/adaptix/_internal/provider/static_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/retort/base_retort.py` & `adaptix-3.0.0b6/src/adaptix/_internal/retort/base_retort.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/retort/mediator.py` & `adaptix-3.0.0b6/src/adaptix/_internal/retort/mediator.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/retort/operating_retort.py` & `adaptix-3.0.0b6/src/adaptix/_internal/retort/operating_retort.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from abc import ABC
-from typing import Any, Dict, Iterable, List, Mapping, Optional, Type, Union
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Type
 
-from ..common import TypeHint, VarTuple
-from ..conversion.request_cls import CoercerRequest, ConversionDestItem, ConversionSourceItem, LinkingRequest
+from ..common import VarTuple
+from ..conversion.request_cls import CoercerRequest, LinkingRequest
 from ..morphing.request_cls import DumperRequest, LoaderRequest
 from ..provider.essential import AggregateCannotProvide, CannotProvide, Mediator, Provider, Request
-from ..provider.location import AnyLoc, FieldLoc
-from ..provider.request_cls import LocatedRequest, LocStack
-from ..type_tools import is_parametrized
+from ..provider.location import AnyLoc
+from ..provider.request_cls import LocatedRequest, LocStack, format_loc_stack
 from ..utils import add_note, copy_exception_dunders, with_module
 from .base_retort import BaseRetort
 from .mediator import ErrorRepresentor, RecursionResolver, T
 
 
 class FuncWrapper:
     __slots__ = ("__call__",)
@@ -64,56 +63,33 @@
         CoercerRequest: "Cannot find coercer",
     }
 
     def _get_linking_request_description(self, request: LinkingRequest) -> str:
         dst_desc = self._get_loc_stack_desc(request.destination)
         return f"Cannot find paired field of `{dst_desc}` for linking"
 
-    def _get_type_desc(self, tp: TypeHint) -> str:
-        if isinstance(tp, type) and not is_parametrized(tp):
-            return tp.__qualname__
-        str_tp = str(tp)
-        if str_tp.startswith("typing."):
-            return str_tp[7:]
-        return str_tp
-
     def get_no_provider_description(self, request: Request) -> str:
         request_cls = type(request)
         if request_cls in self._NO_PROVIDER_DESCRIPTION_METHOD:
             return getattr(self, self._NO_PROVIDER_DESCRIPTION_METHOD[request_cls])(request)
         if request_cls in self._NO_PROVIDER_DESCRIPTION_CONST:
             return self._NO_PROVIDER_DESCRIPTION_CONST[request_cls]
         return f"There is no provider that can process {request}"
 
-    def _get_loc_stack_desc(
-        self,
-        loc_stack: LocStack[Union[ConversionSourceItem, ConversionDestItem]],
-    ) -> str:
-        tp_desc = self._get_type_desc(loc_stack.last.type)
-
-        try:
-            owner_loc = loc_stack[-2]
-        except (TypeError, IndexError):
-            return tp_desc
-
-        try:
-            field_loc = loc_stack.last.cast(FieldLoc)
-        except TypeError:
-            return tp_desc
-        src_owner = self._get_type_desc(owner_loc.type)
-        return f"{src_owner}.{field_loc.field_id}: {tp_desc}"
+    def _get_loc_stack_desc(self, loc_stack: LocStack[AnyLoc]) -> str:
+        return format_loc_stack(loc_stack)
 
     def _get_located_request_context_notes(self, request: LocatedRequest) -> Iterable[str]:
         loc_stack_desc = self._get_loc_stack_desc(request.loc_stack)
         yield f"Location: `{loc_stack_desc}`"
 
     def _get_coercer_request_context_notes(self, request: CoercerRequest) -> Iterable[str]:
         src_desc = self._get_loc_stack_desc(request.src)
         dst_desc = self._get_loc_stack_desc(request.dst)
-        yield f"Linking: `{src_desc} -> {dst_desc}`"
+        yield f"Linking: `{src_desc} => {dst_desc}`"
 
     def get_request_context_notes(self, request: Request) -> Iterable[str]:
         if isinstance(request, LocatedRequest):
             yield from self._get_located_request_context_notes(request)
         elif isinstance(request, CoercerRequest):
             yield from self._get_coercer_request_context_notes(request)
```

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/retort/routing.py` & `adaptix-3.0.0b6/src/adaptix/_internal/retort/routing.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/special_cases_optimization.py` & `adaptix-3.0.0b6/src/adaptix/_internal/special_cases_optimization.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/struct_trail.py` & `adaptix-3.0.0b6/src/adaptix/_internal/struct_trail.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/__init__.py` & `adaptix-3.0.0b6/src/adaptix/_internal/type_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/basic_utils.py` & `adaptix-3.0.0b6/src/adaptix/_internal/type_tools/basic_utils.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/constants.py` & `adaptix-3.0.0b6/src/adaptix/_internal/type_tools/constants.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/fundamentals.py` & `adaptix-3.0.0b6/src/adaptix/_internal/type_tools/fundamentals.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/generic_resolver.py` & `adaptix-3.0.0b6/src/adaptix/_internal/type_tools/generic_resolver.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/implicit_params.py` & `adaptix-3.0.0b6/src/adaptix/_internal/type_tools/implicit_params.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/norm_utils.py` & `adaptix-3.0.0b6/src/adaptix/_internal/type_tools/norm_utils.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/normalize_type.py` & `adaptix-3.0.0b6/src/adaptix/_internal/type_tools/normalize_type.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/_internal/utils.py` & `adaptix-3.0.0b6/src/adaptix/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix/conversion/__init__.py` & `adaptix-3.0.0b6/src/adaptix/conversion/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 from adaptix._internal.conversion.facade.provider import (
     allow_unlinked_optional,
     coercer,
     forbid_unlinked_optional,
     from_param,
     link,
     link_constant,
+    link_function,
 )
 from adaptix._internal.conversion.facade.retort import AdornedConversionRetort, ConversionRetort, FilledConversionRetort
 
 __all__ = (
     "convert",
     "get_converter",
     "impl_converter",
     "link",
     "link_constant",
+    "link_function",
     "coercer",
     "allow_unlinked_optional",
     "forbid_unlinked_optional",
     "from_param",
     "AdornedConversionRetort",
     "FilledConversionRetort",
     "ConversionRetort",
```

### Comparing `adaptix-3.0.0b5/src/adaptix/load_error.py` & `adaptix-3.0.0b6/src/adaptix/load_error.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b5/src/adaptix.egg-info/PKG-INFO` & `adaptix-3.0.0b6/src/adaptix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptix
-Version: 3.0.0b5
+Version: 3.0.0b6
 Summary: An extremely flexible and configurable data model conversion library
 Author-email: "A. Tikhonov" <17@itishka.org>
 Project-URL: Homepage, https://github.com/reagento/adaptix
 Project-URL: Bug Tracker, https://github.com/reagento/adaptix/issues
 Project-URL: Documentation, https://adaptix.readthedocs.io/en/latest/
 Project-URL: Changelog, https://adaptix.readthedocs.io/en/latest/reference/changelog.html
 Project-URL: Source, https://github.com/reagento/adaptix/
@@ -34,24 +34,24 @@
 Provides-Extra: attrs
 Requires-Dist: attrs>=21.3.0; extra == "attrs"
 Provides-Extra: attrs-strict
 Requires-Dist: attrs<=23.2.0,>=21.3.0; extra == "attrs-strict"
 Provides-Extra: sqlalchemy
 Requires-Dist: sqlalchemy>=2.0.0; extra == "sqlalchemy"
 Provides-Extra: sqlalchemy-strict
-Requires-Dist: sqlalchemy<=2.0.29,>=2.0.0; extra == "sqlalchemy-strict"
+Requires-Dist: sqlalchemy<=2.0.30,>=2.0.0; extra == "sqlalchemy-strict"
 Provides-Extra: pydantic
 Requires-Dist: pydantic>=2.0.0; extra == "pydantic"
 Provides-Extra: pydantic-strict
-Requires-Dist: pydantic<=2.7.0,>=2.0.0; extra == "pydantic-strict"
+Requires-Dist: pydantic<=2.7.1,>=2.0.0; extra == "pydantic-strict"
 
 <div align="center">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b5/docs/logo/adaptix-with-title-dark.png?raw=true">
-    <source media="(prefers-color-scheme: light)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b5/docs/logo/adaptix-with-title-light.png?raw=true">
+    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b6/docs/logo/adaptix-with-title-dark.png?raw=true">
+    <source media="(prefers-color-scheme: light)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b6/docs/logo/adaptix-with-title-light.png?raw=true">
     <img alt="adaptix logo" src="https://raw.githubusercontent.com/reagento/adaptix/v3.0.0b2/docs/logo/adaptix-with-title-light.png?raw=true">
   </picture>
 
   <hr>
 
   [![PyPI version](https://img.shields.io/pypi/v/adaptix.svg?color=blue)](https://pypi.org/project/adaptix/)
   [![downloads](https://img.shields.io/pypi/dm/adaptix.svg)](https://pypistats.org/packages/adaptix)
@@ -67,15 +67,15 @@
 
 📚 [Documentation](https://adaptix.readthedocs.io/)
 
 ## TL;DR
 
 Install
 ```bash
-pip install adaptix==3.0.0b5
+pip install adaptix==3.0.0b6
 ```
 
 Use for model loading and dumping.
 
 ```python
 from dataclasses import dataclass
```

### Comparing `adaptix-3.0.0b5/src/adaptix.egg-info/SOURCES.txt` & `adaptix-3.0.0b6/src/adaptix.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,28 @@
 src/adaptix/_internal/conversion/coercer_provider.py
 src/adaptix/_internal/conversion/converter_provider.py
 src/adaptix/_internal/conversion/linking_provider.py
 src/adaptix/_internal/conversion/model_coercer_provider.py
 src/adaptix/_internal/conversion/policy_provider.py
 src/adaptix/_internal/conversion/provider_template.py
 src/adaptix/_internal/conversion/request_cls.py
+src/adaptix/_internal/conversion/request_filtering.py
 src/adaptix/_internal/conversion/broaching/__init__.py
 src/adaptix/_internal/conversion/broaching/code_generator.py
 src/adaptix/_internal/conversion/broaching/definitions.py
 src/adaptix/_internal/conversion/facade/__init__.py
 src/adaptix/_internal/conversion/facade/checker.py
 src/adaptix/_internal/conversion/facade/func.py
 src/adaptix/_internal/conversion/facade/provider.py
 src/adaptix/_internal/conversion/facade/retort.py
 src/adaptix/_internal/integrations/__init__.py
 src/adaptix/_internal/integrations/pydantic/__init__.py
 src/adaptix/_internal/integrations/pydantic/native.py
+src/adaptix/_internal/integrations/sqlalchemy/__init__.py
+src/adaptix/_internal/integrations/sqlalchemy/orm.py
 src/adaptix/_internal/model_tools/__init__.py
 src/adaptix/_internal/model_tools/definitions.py
 src/adaptix/_internal/model_tools/introspection/__init__.py
 src/adaptix/_internal/model_tools/introspection/attrs.py
 src/adaptix/_internal/model_tools/introspection/callable.py
 src/adaptix/_internal/model_tools/introspection/class_init.py
 src/adaptix/_internal/model_tools/introspection/dataclass.py
@@ -112,10 +115,11 @@
 src/adaptix/_internal/type_tools/generic_resolver.py
 src/adaptix/_internal/type_tools/implicit_params.py
 src/adaptix/_internal/type_tools/norm_utils.py
 src/adaptix/_internal/type_tools/normalize_type.py
 src/adaptix/conversion/__init__.py
 src/adaptix/integrations/__init__.py
 src/adaptix/integrations/pydantic/__init__.py
+src/adaptix/integrations/sqlalchemy/__init__.py
 src/adaptix/provider/__init__.py
 tests/test_doc.py
 tests/test_meta.py
```

### Comparing `adaptix-3.0.0b5/tests/test_doc.py` & `adaptix-3.0.0b6/tests/test_doc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import importlib
+from fnmatch import fnmatch
 from pathlib import Path
+from typing import Optional
 
 import pytest
 
-from adaptix._internal.feature_requirement import HAS_PY_311, HAS_SUPPORTED_PYDANTIC_PKG
+from adaptix._internal.feature_requirement import (
+    HAS_PY_311,
+    HAS_SUPPORTED_PYDANTIC_PKG,
+    HAS_SUPPORTED_SQLALCHEMY_PKG,
+    Requirement,
+)
 
 REPO_ROOT = Path(__file__).parent.parent
 DOCS_EXAMPLES_ROOT = REPO_ROOT / "docs" / "examples"
-EXCLUDE = ["__init__.py"]
+EXCLUDE = ["__init__.py", "helpers.py"]
 GLOB = "*.py"
 
 
 def pytest_generate_tests(metafunc):
     if "import_path" not in metafunc.fixturenames:
         return
 
@@ -29,24 +36,32 @@
                 id=str((path_to_test.parent / path_to_test.stem).relative_to(DOCS_EXAMPLES_ROOT).as_posix()),
             )
             for path_to_test in paths_to_test
         ],
     )
 
 
-CASES_REQUIREMENTS = {
+GLOB_REQUIREMENTS = {
     "loading-and-dumping/tutorial/unexpected_error": HAS_PY_311,
     "reference/integrations/native_pydantic": HAS_SUPPORTED_PYDANTIC_PKG,
     "loading-and-dumping/extended_usage/private_fields_including_no_rename_pydantic": HAS_SUPPORTED_PYDANTIC_PKG,
     "loading-and-dumping/extended_usage/private_fields_including_pydantic": HAS_SUPPORTED_PYDANTIC_PKG,
     "loading-and-dumping/extended_usage/private_fields_skipping_pydantic": HAS_SUPPORTED_PYDANTIC_PKG,
+    "reference/integrations/sqlalchemy_json/*": HAS_SUPPORTED_SQLALCHEMY_PKG,
+    "conversion/tutorial/tldr": HAS_SUPPORTED_SQLALCHEMY_PKG,
 }
 
 
+def _find_requirement(case_id: str) -> Optional[Requirement]:
+    for glob, requirement in GLOB_REQUIREMENTS.items():
+        if fnmatch(case_id, glob):
+            return requirement
+    return None
+
+
 def test_example(import_path: str, case_id: str):
-    if case_id in CASES_REQUIREMENTS:
-        requirement = CASES_REQUIREMENTS[case_id]
-        if not requirement:
-            pytest.skip(requirement.fail_reason)
+    requirement = _find_requirement(case_id)
+    if requirement is not None and not requirement:
+        pytest.skip(requirement.fail_reason)
 
     pytest.register_assert_rewrite(import_path)
     importlib.import_module(import_path)
```

