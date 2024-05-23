# Comparing `tmp/protobuf-5.27.0rc2.tar.gz` & `tmp/protobuf-5.27.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/protobuf-5.27.0rc2.tar", last modified: Wed May  8 16:11:38 2024, max compression
+gzip compressed data, was "dist/protobuf-5.27.0rc3.tar", last modified: Tue May 14 16:46:27 2024, max compression
```

## Comparing `protobuf-5.27.0rc2.tar` & `protobuf-5.27.0rc3.tar`

### file list

```diff
@@ -1,286 +1,286 @@
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1732 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/LICENSE
--rw-r--r--   0 bazel     (1000) bazel     (1003)       39 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/MANIFEST.in
--rw-r--r--   0 bazel     (1000) bazel     (1003)      821 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/PKG-INFO
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4624 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/README.md
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/google/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      150 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/__init__.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/google/protobuf/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      349 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1733 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/any_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3153 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/api_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/google/protobuf/compiler/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/compiler/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3805 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/compiler/plugin_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    52106 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/descriptor.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/descriptor.upb.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)   442992 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/descriptor.upb.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    71806 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/descriptor.upb_minitable.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4640 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/descriptor.upb_minitable.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    68617 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/descriptor.upbdefs.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9334 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/descriptor.upbdefs.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5444 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/descriptor_database.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)   341736 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/descriptor_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    48430 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/descriptor_pool.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/duration_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1677 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/empty_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1773 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/field_mask_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/google/protobuf/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      272 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14073 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/_parameterized.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4787 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/api_implementation.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4082 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/builder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    21722 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/containers.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    36387 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/decoder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    27297 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/encoder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3462 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/enum_type_wrapper.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7225 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/extension_dict.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10416 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/field_mask.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2008 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/message_listener.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)      434 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/python_edition_defaults.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    55408 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/python_message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4080 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/testing_refleaks.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    15450 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/type_checkers.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    20402 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/well_known_types.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7087 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/internal/wire_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    37073 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/json_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12844 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8271 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/message_factory.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4203 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/proto_builder.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/google/protobuf/pyext/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/pyext/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1704 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/pyext/cpp_message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2413 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/reflection.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3121 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/runtime_version.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7787 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/service.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10058 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/service_reflection.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1799 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/source_context_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3069 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/struct_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6709 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/symbol_database.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/google/protobuf/testdata/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/testdata/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3621 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/text_encoding.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    63535 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/text_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1823 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/timestamp_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5446 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/type_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3127 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/unknown_fields.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/google/protobuf/util/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/util/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3045 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/google/protobuf/wrappers_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/protobuf.egg-info/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      821 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/protobuf.egg-info/PKG-INFO
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7279 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/protobuf.egg-info/namespace_packages.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/protobuf.egg-info/top_level.txt
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/python/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9176 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/convert.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1577 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/convert.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    76511 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/descriptor.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2572 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/descriptor.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    27874 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/descriptor_containers.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4157 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/descriptor_containers.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    23481 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/descriptor_pool.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      936 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/descriptor_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8703 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/extension_dict.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      530 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/extension_dict.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    19451 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/map.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1610 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    72004 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3875 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    13415 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/protobuf.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8434 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/protobuf.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1642 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/python_api.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    29318 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/repeated.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2087 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/repeated.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10792 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/unknown_fields.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      531 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/python/unknown_fields.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)       38 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/setup.cfg
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2462 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/setup.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/base/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3581 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/base/descriptor_constants.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/base/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1130 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/base/internal/endian.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      873 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/base/internal/log2.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1747 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/base/status.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1359 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/base/status.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1597 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/base/string_view.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      820 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/base/upcast.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1189 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/generated_code_support.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/hash/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    23982 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/hash/common.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5511 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/hash/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2868 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/hash/int_table.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4857 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/hash/str_table.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/lex/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1140 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/lex/atoi.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      991 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/lex/atoi.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1525 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/lex/round_trip.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1042 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/lex/round_trip.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2775 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/lex/strtod.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      586 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/lex/strtod.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      909 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/lex/unicode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1737 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/lex/unicode.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/mem/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      699 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mem/alloc.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2278 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mem/alloc.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    19954 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mem/arena.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2937 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mem/arena.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/mem/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3515 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mem/internal/arena.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/message/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/accessors.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    20096 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/accessors.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2609 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/accessors_split64.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4931 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/array.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3488 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/array.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8478 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/compare.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2403 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/compare.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1145 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/compat.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1172 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/compat.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12129 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/copy.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1884 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/copy.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/message/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14018 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/accessors.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5116 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/array.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9532 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/compare_unknown.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1504 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/compare_unknown.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2012 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/extension.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2052 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/extension.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5263 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1405 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/map_entry.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2779 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/map_sorter.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2510 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3450 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1577 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/tagged_ptr.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1507 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/internal/types.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4430 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/map.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4524 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1687 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/map_gencode_util.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5108 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/map_sorter.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5135 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2163 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14857 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/promote.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6050 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/promote.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1522 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/tagged_ptr.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1261 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/message/value.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/mini_descriptor/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4796 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/build_enum.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1003 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/build_enum.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    34378 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/decode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4982 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/decode.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/mini_descriptor/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1291 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/internal/base92.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1723 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/internal/base92.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1686 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/internal/decoder.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12665 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/internal/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3631 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/internal/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1034 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/internal/modifiers.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2169 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/internal/wire_constants.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4577 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/link.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3566 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_descriptor/link.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/mini_table/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4176 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/compat.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1376 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/compat.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      864 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/enum.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1172 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/extension.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2733 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/extension_registry.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3577 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/extension_registry.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1684 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/field.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1306 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/file.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/mini_table/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1705 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/internal/enum.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1692 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/internal/extension.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6893 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/internal/field.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1860 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/internal/file.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      882 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/internal/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6491 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/internal/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2622 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/internal/size_log2.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1384 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/internal/sub.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2146 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3040 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1094 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/mini_table/sub.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/port/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3197 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/port/atomic.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10400 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/port/def.inc
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1398 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/port/undef.inc
--rw-r--r--   0 bazel     (1000) bazel     (1003)      972 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/port/vsnprintf_compat.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/reflection/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1620 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      826 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    17888 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/def_pool.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3552 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/def_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      958 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/def_type.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1711 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/def_type.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      926 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/desc_state.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10941 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/enum_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2416 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/enum_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2027 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/enum_reserved_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      815 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/enum_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5148 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/enum_value_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1245 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/enum_value_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2778 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/extension_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1057 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/extension_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    34466 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/field_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3591 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/field_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    15603 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/file_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2289 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/file_def.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/reflection/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    13068 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/def_builder.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6985 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/def_builder.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2068 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/def_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1108 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/desc_state.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1204 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/enum_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1059 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/enum_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1184 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/enum_value_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1021 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/extension_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2238 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/field_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1120 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/file_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/message_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1038 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/message_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1087 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/method_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1286 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/oneof_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1078 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/service_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      849 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/strdup2.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      796 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/strdup2.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      969 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/internal/upb_edition_defaults.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8252 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3386 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    27484 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/message_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6403 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/message_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1995 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/message_reserved_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      836 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/message_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3812 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/method_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1432 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/method_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7367 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/oneof_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1836 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/oneof_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4039 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/service_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1499 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/reflection/service_def.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/text/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    15578 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/text/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1454 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/text/encode.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/util/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    24464 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/util/def_to_proto.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1737 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/util/def_to_proto.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9941 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/util/required_fields.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2842 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/util/required_fields.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/wire/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    54041 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/decode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6190 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    22846 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2750 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      724 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/eps_copy_input_stream.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    17093 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/eps_copy_input_stream.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/upb/wire/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      716 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/internal/constants.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    50516 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/internal/decode_fast.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3998 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/internal/decode_fast.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4286 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/internal/decoder.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1635 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/internal/reader.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1446 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/reader.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6570 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/reader.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)      620 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/upb/wire/types.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-08 16:11:38.000000 protobuf-5.27.0rc2/utf8_range/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    17939 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/utf8_range/utf8_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      540 2000-01-01 00:00:00.000000 protobuf-5.27.0rc2/utf8_range/utf8_range.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1732 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/LICENSE
+-rw-r--r--   0 bazel     (1000) bazel     (1003)       39 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/MANIFEST.in
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      821 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/PKG-INFO
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4624 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/README.md
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/google/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      150 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/__init__.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/google/protobuf/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      349 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1733 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/any_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3153 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/api_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/google/protobuf/compiler/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/compiler/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3805 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/compiler/plugin_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    52106 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/descriptor.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/descriptor.upb.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)   442992 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/descriptor.upb.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    71806 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/descriptor.upb_minitable.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4640 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/descriptor.upb_minitable.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    68436 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/descriptor.upbdefs.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9334 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/descriptor.upbdefs.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5444 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/descriptor_database.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)   341526 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/descriptor_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    48430 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/descriptor_pool.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/duration_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1677 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/empty_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1773 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/field_mask_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/google/protobuf/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      272 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    14073 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/_parameterized.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4787 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/api_implementation.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4082 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/builder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    21722 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/containers.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    36387 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/decoder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    27297 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/encoder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3462 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/enum_type_wrapper.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7225 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/extension_dict.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10416 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/field_mask.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2008 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/message_listener.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      434 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/python_edition_defaults.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    55408 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/python_message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4080 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/testing_refleaks.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    15450 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/type_checkers.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    20402 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/well_known_types.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7087 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/internal/wire_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    37073 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/json_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12844 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8271 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/message_factory.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4203 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/proto_builder.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/google/protobuf/pyext/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/pyext/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1704 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/pyext/cpp_message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2413 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/reflection.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3121 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/runtime_version.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7787 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/service.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10058 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/service_reflection.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1799 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/source_context_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3069 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/struct_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6709 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/symbol_database.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/google/protobuf/testdata/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/testdata/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3621 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/text_encoding.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    63535 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/text_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1823 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/timestamp_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5446 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/type_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3127 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/unknown_fields.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/google/protobuf/util/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/util/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3045 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/google/protobuf/wrappers_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/protobuf.egg-info/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      821 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7279 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/protobuf.egg-info/namespace_packages.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/protobuf.egg-info/top_level.txt
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/python/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9176 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/convert.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1577 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/convert.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    76511 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/descriptor.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2572 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/descriptor.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    27874 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/descriptor_containers.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4157 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/descriptor_containers.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    23481 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/descriptor_pool.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      936 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/descriptor_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8703 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/extension_dict.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      530 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/extension_dict.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    19451 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/map.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1610 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    72004 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3875 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    13415 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/protobuf.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8434 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/protobuf.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1642 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/python_api.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    29318 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/repeated.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2087 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/repeated.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10792 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/unknown_fields.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      531 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/python/unknown_fields.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)       38 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/setup.cfg
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2462 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/setup.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/base/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3581 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/base/descriptor_constants.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/base/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1130 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/base/internal/endian.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      873 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/base/internal/log2.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1747 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/base/status.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1359 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/base/status.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1597 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/base/string_view.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      820 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/base/upcast.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1189 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/generated_code_support.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/hash/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    23982 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/hash/common.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5511 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/hash/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2868 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/hash/int_table.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4857 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/hash/str_table.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/lex/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1140 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/lex/atoi.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      991 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/lex/atoi.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1525 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/lex/round_trip.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1042 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/lex/round_trip.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2775 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/lex/strtod.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      586 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/lex/strtod.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      909 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/lex/unicode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1737 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/lex/unicode.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/mem/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      699 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mem/alloc.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2278 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mem/alloc.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    19954 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mem/arena.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2937 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mem/arena.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/mem/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3515 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mem/internal/arena.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/message/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/accessors.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    20096 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/accessors.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2609 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/accessors_split64.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4931 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/array.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3488 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/array.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8478 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/compare.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2403 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/compare.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1145 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/compat.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1172 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/compat.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12129 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/copy.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1884 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/copy.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/message/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    14018 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/accessors.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5116 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/array.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9532 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/compare_unknown.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1504 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/compare_unknown.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2012 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/extension.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2052 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/extension.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5263 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1405 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/map_entry.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2779 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/map_sorter.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2510 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3450 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1577 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/tagged_ptr.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1507 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/internal/types.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4430 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/map.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4524 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1687 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/map_gencode_util.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5108 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/map_sorter.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5135 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2163 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    14857 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/promote.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6050 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/promote.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1522 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/tagged_ptr.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1261 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/message/value.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/mini_descriptor/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4796 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/build_enum.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1003 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/build_enum.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    34378 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/decode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4982 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/decode.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/mini_descriptor/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1291 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/internal/base92.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1723 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/internal/base92.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1686 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/internal/decoder.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12665 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/internal/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3631 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/internal/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1034 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/internal/modifiers.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2169 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/internal/wire_constants.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4577 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/link.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3566 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_descriptor/link.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/mini_table/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4176 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/compat.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1376 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/compat.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      864 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/enum.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1172 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/extension.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2733 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/extension_registry.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3577 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/extension_registry.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1684 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/field.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1306 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/file.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/mini_table/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1705 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/internal/enum.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1692 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/internal/extension.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6893 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/internal/field.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1860 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/internal/file.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      882 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/internal/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6491 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/internal/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2622 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/internal/size_log2.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1384 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/internal/sub.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2146 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3040 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1094 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/mini_table/sub.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/port/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3197 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/port/atomic.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10400 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/port/def.inc
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1398 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/port/undef.inc
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      972 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/port/vsnprintf_compat.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/reflection/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1620 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      826 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    17888 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/def_pool.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3552 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/def_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      958 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/def_type.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1711 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/def_type.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      926 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/desc_state.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10941 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/enum_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2416 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/enum_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2027 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/enum_reserved_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      815 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/enum_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5148 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/enum_value_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1245 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/enum_value_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2778 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/extension_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1057 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/extension_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    34466 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/field_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3591 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/field_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    15603 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/file_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2289 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/file_def.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/reflection/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    13068 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/def_builder.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6985 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/def_builder.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2068 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/def_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1108 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/desc_state.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1204 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/enum_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1059 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/enum_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1184 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/enum_value_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1021 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/extension_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2238 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/field_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1120 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/file_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/message_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1038 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/message_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1087 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/method_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1286 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/oneof_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1078 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/service_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      849 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/strdup2.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      796 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/strdup2.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      969 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/internal/upb_edition_defaults.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8252 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3386 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    27484 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/message_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6403 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/message_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1995 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/message_reserved_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      836 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/message_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3812 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/method_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1432 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/method_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7367 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/oneof_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1836 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/oneof_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4039 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/service_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1499 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/reflection/service_def.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/text/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    15578 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/text/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1454 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/text/encode.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/util/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    24464 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/util/def_to_proto.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1737 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/util/def_to_proto.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9941 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/util/required_fields.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2842 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/util/required_fields.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/wire/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    54041 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/decode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6190 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    22846 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2750 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      724 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/eps_copy_input_stream.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    17093 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/eps_copy_input_stream.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/upb/wire/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      716 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/internal/constants.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    50516 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/internal/decode_fast.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3998 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/internal/decode_fast.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4286 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/internal/decoder.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1635 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/internal/reader.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1446 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/reader.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6570 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/reader.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      620 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/upb/wire/types.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2024-05-14 16:46:27.000000 protobuf-5.27.0rc3/utf8_range/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    17939 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/utf8_range/utf8_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      540 2000-01-01 00:00:00.000000 protobuf-5.27.0rc3/utf8_range/utf8_range.h
```

### Comparing `protobuf-5.27.0rc2/LICENSE` & `protobuf-5.27.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/PKG-INFO` & `protobuf-5.27.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf
-Version: 5.27.0rc2
+Version: 5.27.0rc3
 Summary: Protocol Buffers
 Home-page: https://developers.google.com/protocol-buffers/
 Download-URL: https://github.com/protocolbuffers/protobuf/releases
 Maintainer: protobuf@googlegroups.com
 Maintainer-email: protobuf@googlegroups.com
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/protocolbuffers/protobuf
```

### Comparing `protobuf-5.27.0rc2/README.md` & `protobuf-5.27.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/any_pb2.py` & `protobuf-5.27.0rc3/google/protobuf/any_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/any.proto
-# Protobuf Python Version: 5.27.0-rc2
+# Protobuf Python Version: 5.27.0-rc3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _runtime_version.ValidateProtobufRuntimeVersion(
     _runtime_version.Domain.PUBLIC,
     5,
     27,
     0,
-    '-rc2',
+    '-rc3',
     'google/protobuf/any.proto'
 )
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/api_pb2.py` & `protobuf-5.27.0rc3/google/protobuf/api_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/api.proto
-# Protobuf Python Version: 5.27.0-rc2
+# Protobuf Python Version: 5.27.0-rc3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _runtime_version.ValidateProtobufRuntimeVersion(
     _runtime_version.Domain.PUBLIC,
     5,
     27,
     0,
-    '-rc2',
+    '-rc3',
     'google/protobuf/api.proto'
 )
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/compiler/plugin_pb2.py` & `protobuf-5.27.0rc3/google/protobuf/compiler/plugin_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/compiler/plugin.proto
-# Protobuf Python Version: 5.27.0-rc2
+# Protobuf Python Version: 5.27.0-rc3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _runtime_version.ValidateProtobufRuntimeVersion(
     _runtime_version.Domain.PUBLIC,
     5,
     27,
     0,
-    '-rc2',
+    '-rc3',
     'google/protobuf/compiler/plugin.proto'
 )
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/descriptor.py` & `protobuf-5.27.0rc3/google/protobuf/descriptor.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/descriptor.upb.h` & `protobuf-5.27.0rc3/google/protobuf/descriptor.upb.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/descriptor.upb_minitable.c` & `protobuf-5.27.0rc3/google/protobuf/descriptor.upb_minitable.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/descriptor.upb_minitable.h` & `protobuf-5.27.0rc3/google/protobuf/descriptor.upb_minitable.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/descriptor.upbdefs.c` & `protobuf-5.27.0rc3/google/protobuf/descriptor.upbdefs.c`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
  * Do not edit -- your changes will be discarded when the file is
  * regenerated. */
 
 #include "upb/reflection/def.h"
 #include "google/protobuf/descriptor.upbdefs.h"
 #include "google/protobuf/descriptor.upb_minitable.h"
 
-static const char descriptor[12155] = {'\n', ' ', 'g', 'o', 'o', 'g', 'l', 'e', '/', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '/', 'd', 'e', 's', 'c', 'r', 'i', 'p', 
+static const char descriptor[12131] = {'\n', ' ', 'g', 'o', 'o', 'g', 'l', 'e', '/', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '/', 'd', 'e', 's', 'c', 'r', 'i', 'p', 
 't', 'o', 'r', '.', 'p', 'r', 'o', 't', 'o', '\022', '\017', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
 'f', '\"', 'M', '\n', '\021', 'F', 'i', 'l', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'S', 'e', 't', '\022', '8', '\n', 
 '\004', 'f', 'i', 'l', 'e', '\030', '\001', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 
 'o', 'b', 'u', 'f', '.', 'F', 'i', 'l', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', 'R', 
 '\004', 'f', 'i', 'l', 'e', '\"', '\230', '\005', '\n', '\023', 'F', 'i', 'l', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 
 'r', 'o', 't', 'o', '\022', '\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\004', 'n', 'a', 'm', 'e', '\022', 
 '\030', '\n', '\007', 'p', 'a', 'c', 'k', 'a', 'g', 'e', '\030', '\002', ' ', '\001', '(', '\t', 'R', '\007', 'p', 'a', 'c', 'k', 'a', 'g', 'e', 
@@ -376,15 +376,15 @@
 'v', 'a', 'l', 'u', 'e', '\030', '\006', ' ', '\001', '(', '\001', 'R', '\013', 'd', 'o', 'u', 'b', 'l', 'e', 'V', 'a', 'l', 'u', 'e', '\022', 
 '!', '\n', '\014', 's', 't', 'r', 'i', 'n', 'g', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\007', ' ', '\001', '(', '\014', 'R', '\013', 's', 't', 
 'r', 'i', 'n', 'g', 'V', 'a', 'l', 'u', 'e', '\022', '\'', '\n', '\017', 'a', 'g', 'g', 'r', 'e', 'g', 'a', 't', 'e', '_', 'v', 'a', 
 'l', 'u', 'e', '\030', '\010', ' ', '\001', '(', '\t', 'R', '\016', 'a', 'g', 'g', 'r', 'e', 'g', 'a', 't', 'e', 'V', 'a', 'l', 'u', 'e', 
 '\032', 'J', '\n', '\010', 'N', 'a', 'm', 'e', 'P', 'a', 'r', 't', '\022', '\033', '\n', '\t', 'n', 'a', 'm', 'e', '_', 'p', 'a', 'r', 't', 
 '\030', '\001', ' ', '\002', '(', '\t', 'R', '\010', 'n', 'a', 'm', 'e', 'P', 'a', 'r', 't', '\022', '!', '\n', '\014', 'i', 's', '_', 'e', 'x', 
 't', 'e', 'n', 's', 'i', 'o', 'n', '\030', '\002', ' ', '\002', '(', '\010', 'R', '\013', 'i', 's', 'E', 'x', 't', 'e', 'n', 's', 'i', 'o', 
-'n', '\"', '\271', '\n', '\n', '\n', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '\022', '\221', '\001', '\n', '\016', 'f', 'i', 'e', 'l', 
+'n', '\"', '\241', '\n', '\n', '\n', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '\022', '\221', '\001', '\n', '\016', 'f', 'i', 'e', 'l', 
 'd', '_', 'p', 'r', 'e', 's', 'e', 'n', 'c', 'e', '\030', '\001', ' ', '\001', '(', '\016', '2', ')', '.', 'g', 'o', 'o', 'g', 'l', 'e', 
 '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', '.', 'F', 'i', 'e', 'l', 
 'd', 'P', 'r', 'e', 's', 'e', 'n', 'c', 'e', 'B', '?', '\210', '\001', '\001', '\230', '\001', '\004', '\230', '\001', '\001', '\242', '\001', '\r', '\022', '\010', 
 'E', 'X', 'P', 'L', 'I', 'C', 'I', 'T', '\030', '\346', '\007', '\242', '\001', '\r', '\022', '\010', 'I', 'M', 'P', 'L', 'I', 'C', 'I', 'T', '\030', 
 '\347', '\007', '\242', '\001', '\r', '\022', '\010', 'E', 'X', 'P', 'L', 'I', 'C', 'I', 'T', '\030', '\350', '\007', '\262', '\001', '\003', '\010', '\350', '\007', 'R', 
 '\r', 'f', 'i', 'e', 'l', 'd', 'P', 'r', 'e', 's', 'e', 'n', 'c', 'e', '\022', 'l', '\n', '\t', 'e', 'n', 'u', 'm', '_', 't', 'y', 
 'p', 'e', '\030', '\002', ' ', '\001', '(', '\016', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
@@ -427,84 +427,83 @@
 'W', 'N', '\020', '\000', '\022', '\n', '\n', '\006', 'V', 'E', 'R', 'I', 'F', 'Y', '\020', '\002', '\022', '\010', '\n', '\004', 'N', 'O', 'N', 'E', '\020', 
 '\003', '\"', 'S', '\n', '\017', 'M', 'e', 's', 's', 'a', 'g', 'e', 'E', 'n', 'c', 'o', 'd', 'i', 'n', 'g', '\022', '\034', '\n', '\030', 'M', 
 'E', 'S', 'S', 'A', 'G', 'E', '_', 'E', 'N', 'C', 'O', 'D', 'I', 'N', 'G', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', 
 '\022', '\023', '\n', '\017', 'L', 'E', 'N', 'G', 'T', 'H', '_', 'P', 'R', 'E', 'F', 'I', 'X', 'E', 'D', '\020', '\001', '\022', '\r', '\n', '\t', 
 'D', 'E', 'L', 'I', 'M', 'I', 'T', 'E', 'D', '\020', '\002', '\"', 'H', '\n', '\n', 'J', 's', 'o', 'n', 'F', 'o', 'r', 'm', 'a', 't', 
 '\022', '\027', '\n', '\023', 'J', 'S', 'O', 'N', '_', 'F', 'O', 'R', 'M', 'A', 'T', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', 
 '\022', '\t', '\n', '\005', 'A', 'L', 'L', 'O', 'W', '\020', '\001', '\022', '\026', '\n', '\022', 'L', 'E', 'G', 'A', 'C', 'Y', '_', 'B', 'E', 'S', 
-'T', '_', 'E', 'F', 'F', 'O', 'R', 'T', '\020', '\002', '*', '\006', '\010', '\350', '\007', '\020', '\351', '\007', '*', '\006', '\010', '\351', '\007', '\020', '\352', 
-'\007', '*', '\006', '\010', '\352', '\007', '\020', '\353', '\007', '*', '\006', '\010', '\206', 'N', '\020', '\207', 'N', '*', '\006', '\010', '\213', 'N', '\020', '\220', 'N', 
-'*', '\006', '\010', '\220', 'N', '\020', '\221', 'N', 'J', '\006', '\010', '\347', '\007', '\020', '\350', '\007', '\"', '\331', '\003', '\n', '\022', 'F', 'e', 'a', 't', 
-'u', 'r', 'e', 'S', 'e', 't', 'D', 'e', 'f', 'a', 'u', 'l', 't', 's', '\022', 'X', '\n', '\010', 'd', 'e', 'f', 'a', 'u', 'l', 't', 
-'s', '\030', '\001', ' ', '\003', '(', '\013', '2', '<', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', 
-'.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'D', 'e', 'f', 'a', 'u', 'l', 't', 's', '.', 'F', 'e', 'a', 't', 'u', 
-'r', 'e', 'S', 'e', 't', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'D', 'e', 'f', 'a', 'u', 'l', 't', 'R', '\010', 'd', 'e', 'f', 'a', 
-'u', 'l', 't', 's', '\022', 'A', '\n', '\017', 'm', 'i', 'n', 'i', 'm', 'u', 'm', '_', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\030', '\004', 
-' ', '\001', '(', '\016', '2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'd', 
-'i', 't', 'i', 'o', 'n', 'R', '\016', 'm', 'i', 'n', 'i', 'm', 'u', 'm', 'E', 'd', 'i', 't', 'i', 'o', 'n', '\022', 'A', '\n', '\017', 
-'m', 'a', 'x', 'i', 'm', 'u', 'm', '_', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\030', '\005', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 
-'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\016', 'm', 
-'a', 'x', 'i', 'm', 'u', 'm', 'E', 'd', 'i', 't', 'i', 'o', 'n', '\032', '\342', '\001', '\n', '\030', 'F', 'e', 'a', 't', 'u', 'r', 'e', 
-'S', 'e', 't', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'D', 'e', 'f', 'a', 'u', 'l', 't', '\022', '2', '\n', '\007', 'e', 'd', 'i', 't', 
-'i', 'o', 'n', '\030', '\003', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 
-'u', 'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\007', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\022', 'N', '\n', '\024', 'o', 'v', 
-'e', 'r', 'r', 'i', 'd', 'a', 'b', 'l', 'e', '_', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\004', ' ', '\001', '(', '\013', '2', 
+'T', '_', 'E', 'F', 'F', 'O', 'R', 'T', '\020', '\002', '*', '\006', '\010', '\350', '\007', '\020', '\213', 'N', '*', '\006', '\010', '\213', 'N', '\020', '\220', 
+'N', '*', '\006', '\010', '\220', 'N', '\020', '\221', 'N', 'J', '\006', '\010', '\347', '\007', '\020', '\350', '\007', '\"', '\331', '\003', '\n', '\022', 'F', 'e', 'a', 
+'t', 'u', 'r', 'e', 'S', 'e', 't', 'D', 'e', 'f', 'a', 'u', 'l', 't', 's', '\022', 'X', '\n', '\010', 'd', 'e', 'f', 'a', 'u', 'l', 
+'t', 's', '\030', '\001', ' ', '\003', '(', '\013', '2', '<', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
+'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 'e', 't', 'D', 'e', 'f', 'a', 'u', 'l', 't', 's', '.', 'F', 'e', 'a', 't', 
+'u', 'r', 'e', 'S', 'e', 't', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'D', 'e', 'f', 'a', 'u', 'l', 't', 'R', '\010', 'd', 'e', 'f', 
+'a', 'u', 'l', 't', 's', '\022', 'A', '\n', '\017', 'm', 'i', 'n', 'i', 'm', 'u', 'm', '_', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\030', 
+'\004', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 
+'d', 'i', 't', 'i', 'o', 'n', 'R', '\016', 'm', 'i', 'n', 'i', 'm', 'u', 'm', 'E', 'd', 'i', 't', 'i', 'o', 'n', '\022', 'A', '\n', 
+'\017', 'm', 'a', 'x', 'i', 'm', 'u', 'm', '_', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\030', '\005', ' ', '\001', '(', '\016', '2', '\030', '.', 
+'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\016', 
+'m', 'a', 'x', 'i', 'm', 'u', 'm', 'E', 'd', 'i', 't', 'i', 'o', 'n', '\032', '\342', '\001', '\n', '\030', 'F', 'e', 'a', 't', 'u', 'r', 
+'e', 'S', 'e', 't', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'D', 'e', 'f', 'a', 'u', 'l', 't', '\022', '2', '\n', '\007', 'e', 'd', 'i', 
+'t', 'i', 'o', 'n', '\030', '\003', ' ', '\001', '(', '\016', '2', '\030', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 
+'b', 'u', 'f', '.', 'E', 'd', 'i', 't', 'i', 'o', 'n', 'R', '\007', 'e', 'd', 'i', 't', 'i', 'o', 'n', '\022', 'N', '\n', '\024', 'o', 
+'v', 'e', 'r', 'r', 'i', 'd', 'a', 'b', 'l', 'e', '_', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\004', ' ', '\001', '(', '\013', 
+'2', '\033', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 
+'e', 'S', 'e', 't', 'R', '\023', 'o', 'v', 'e', 'r', 'r', 'i', 'd', 'a', 'b', 'l', 'e', 'F', 'e', 'a', 't', 'u', 'r', 'e', 's', 
+'\022', 'B', '\n', '\016', 'f', 'i', 'x', 'e', 'd', '_', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\005', ' ', '\001', '(', '\013', '2', 
 '\033', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 
-'S', 'e', 't', 'R', '\023', 'o', 'v', 'e', 'r', 'r', 'i', 'd', 'a', 'b', 'l', 'e', 'F', 'e', 'a', 't', 'u', 'r', 'e', 's', '\022', 
-'B', '\n', '\016', 'f', 'i', 'x', 'e', 'd', '_', 'f', 'e', 'a', 't', 'u', 'r', 'e', 's', '\030', '\005', ' ', '\001', '(', '\013', '2', '\033', 
-'.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'e', 'a', 't', 'u', 'r', 'e', 'S', 
-'e', 't', 'R', '\r', 'f', 'i', 'x', 'e', 'd', 'F', 'e', 'a', 't', 'u', 'r', 'e', 's', '\"', '\247', '\002', '\n', '\016', 'S', 'o', 'u', 
-'r', 'c', 'e', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '\022', 'D', '\n', '\010', 'l', 'o', 'c', 'a', 't', 'i', 'o', 'n', '\030', '\001', 
-' ', '\003', '(', '\013', '2', '(', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'S', 'o', 
-'u', 'r', 'c', 'e', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'L', 'o', 'c', 'a', 't', 'i', 'o', 'n', 'R', '\010', 'l', 'o', 
-'c', 'a', 't', 'i', 'o', 'n', '\032', '\316', '\001', '\n', '\010', 'L', 'o', 'c', 'a', 't', 'i', 'o', 'n', '\022', '\026', '\n', '\004', 'p', 'a', 
-'t', 'h', '\030', '\001', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', '\004', 'p', 'a', 't', 'h', '\022', '\026', '\n', '\004', 's', 'p', 'a', 
-'n', '\030', '\002', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', '\004', 's', 'p', 'a', 'n', '\022', ')', '\n', '\020', 'l', 'e', 'a', 'd', 
-'i', 'n', 'g', '_', 'c', 'o', 'm', 'm', 'e', 'n', 't', 's', '\030', '\003', ' ', '\001', '(', '\t', 'R', '\017', 'l', 'e', 'a', 'd', 'i', 
-'n', 'g', 'C', 'o', 'm', 'm', 'e', 'n', 't', 's', '\022', '+', '\n', '\021', 't', 'r', 'a', 'i', 'l', 'i', 'n', 'g', '_', 'c', 'o', 
-'m', 'm', 'e', 'n', 't', 's', '\030', '\004', ' ', '\001', '(', '\t', 'R', '\020', 't', 'r', 'a', 'i', 'l', 'i', 'n', 'g', 'C', 'o', 'm', 
-'m', 'e', 'n', 't', 's', '\022', ':', '\n', '\031', 'l', 'e', 'a', 'd', 'i', 'n', 'g', '_', 'd', 'e', 't', 'a', 'c', 'h', 'e', 'd', 
-'_', 'c', 'o', 'm', 'm', 'e', 'n', 't', 's', '\030', '\006', ' ', '\003', '(', '\t', 'R', '\027', 'l', 'e', 'a', 'd', 'i', 'n', 'g', 'D', 
-'e', 't', 'a', 'c', 'h', 'e', 'd', 'C', 'o', 'm', 'm', 'e', 'n', 't', 's', '\"', '\320', '\002', '\n', '\021', 'G', 'e', 'n', 'e', 'r', 
-'a', 't', 'e', 'd', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '\022', 'M', '\n', '\n', 'a', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 
-'n', '\030', '\001', ' ', '\003', '(', '\013', '2', '-', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', 
-'.', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'A', 'n', 'n', 'o', 't', 'a', 
-'t', 'i', 'o', 'n', 'R', '\n', 'a', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '\032', '\353', '\001', '\n', '\n', 'A', 'n', 'n', 'o', 
-'t', 'a', 't', 'i', 'o', 'n', '\022', '\026', '\n', '\004', 'p', 'a', 't', 'h', '\030', '\001', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', 
-'\004', 'p', 'a', 't', 'h', '\022', '\037', '\n', '\013', 's', 'o', 'u', 'r', 'c', 'e', '_', 'f', 'i', 'l', 'e', '\030', '\002', ' ', '\001', '(', 
-'\t', 'R', '\n', 's', 'o', 'u', 'r', 'c', 'e', 'F', 'i', 'l', 'e', '\022', '\024', '\n', '\005', 'b', 'e', 'g', 'i', 'n', '\030', '\003', ' ', 
-'\001', '(', '\005', 'R', '\005', 'b', 'e', 'g', 'i', 'n', '\022', '\020', '\n', '\003', 'e', 'n', 'd', '\030', '\004', ' ', '\001', '(', '\005', 'R', '\003', 
-'e', 'n', 'd', '\022', 'R', '\n', '\010', 's', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\030', '\005', ' ', '\001', '(', '\016', '2', '6', '.', 'g', 
-'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 'C', 
-'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'A', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '.', 'S', 'e', 'm', 'a', 'n', 't', 
-'i', 'c', 'R', '\010', 's', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\"', '(', '\n', '\010', 'S', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\022', 
-'\010', '\n', '\004', 'N', 'O', 'N', 'E', '\020', '\000', '\022', '\007', '\n', '\003', 'S', 'E', 'T', '\020', '\001', '\022', '\t', '\n', '\005', 'A', 'L', 'I', 
-'A', 'S', '\020', '\002', '*', '\247', '\002', '\n', '\007', 'E', 'd', 'i', 't', 'i', 'o', 'n', '\022', '\023', '\n', '\017', 'E', 'D', 'I', 'T', 'I', 
-'O', 'N', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\023', '\n', '\016', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 'L', 
-'E', 'G', 'A', 'C', 'Y', '\020', '\204', '\007', '\022', '\023', '\n', '\016', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 'P', 'R', 'O', 'T', 'O', 
-'2', '\020', '\346', '\007', '\022', '\023', '\n', '\016', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 'P', 'R', 'O', 'T', 'O', '3', '\020', '\347', '\007', 
-'\022', '\021', '\n', '\014', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', '2', '0', '2', '3', '\020', '\350', '\007', '\022', '\021', '\n', '\014', 'E', 'D', 
-'I', 'T', 'I', 'O', 'N', '_', '2', '0', '2', '4', '\020', '\351', '\007', '\022', '\027', '\n', '\023', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 
-'1', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 'L', 'Y', '\020', '\001', '\022', '\027', '\n', '\023', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 
-'2', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 'L', 'Y', '\020', '\002', '\022', '\035', '\n', '\027', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 
-'9', '9', '9', '9', '7', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 'L', 'Y', '\020', '\235', '\215', '\006', '\022', '\035', '\n', '\027', 'E', 'D', 
-'I', 'T', 'I', 'O', 'N', '_', '9', '9', '9', '9', '8', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 'L', 'Y', '\020', '\236', '\215', '\006', 
-'\022', '\035', '\n', '\027', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', '9', '9', '9', '9', '9', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 
-'L', 'Y', '\020', '\237', '\215', '\006', '\022', '\023', '\n', '\013', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 'M', 'A', 'X', '\020', '\377', '\377', '\377', 
-'\377', '\007', 'B', '~', '\n', '\023', 'c', 'o', 'm', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', 
-'B', '\020', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', 's', 'H', '\001', 'Z', '-', 'g', 'o', 'o', 
-'g', 'l', 'e', '.', 'g', 'o', 'l', 'a', 'n', 'g', '.', 'o', 'r', 'g', '/', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '/', 't', 
-'y', 'p', 'e', 's', '/', 'd', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'p', 'b', '\370', '\001', '\001', '\242', '\002', '\003', 'G', 'P', 
-'B', '\252', '\002', '\032', 'G', 'o', 'o', 'g', 'l', 'e', '.', 'P', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'R', 'e', 'f', 'l', 'e', 
-'c', 't', 'i', 'o', 'n', 
+'S', 'e', 't', 'R', '\r', 'f', 'i', 'x', 'e', 'd', 'F', 'e', 'a', 't', 'u', 'r', 'e', 's', '\"', '\247', '\002', '\n', '\016', 'S', 'o', 
+'u', 'r', 'c', 'e', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '\022', 'D', '\n', '\010', 'l', 'o', 'c', 'a', 't', 'i', 'o', 'n', '\030', 
+'\001', ' ', '\003', '(', '\013', '2', '(', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'S', 
+'o', 'u', 'r', 'c', 'e', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'L', 'o', 'c', 'a', 't', 'i', 'o', 'n', 'R', '\010', 'l', 
+'o', 'c', 'a', 't', 'i', 'o', 'n', '\032', '\316', '\001', '\n', '\010', 'L', 'o', 'c', 'a', 't', 'i', 'o', 'n', '\022', '\026', '\n', '\004', 'p', 
+'a', 't', 'h', '\030', '\001', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', '\004', 'p', 'a', 't', 'h', '\022', '\026', '\n', '\004', 's', 'p', 
+'a', 'n', '\030', '\002', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', '\004', 's', 'p', 'a', 'n', '\022', ')', '\n', '\020', 'l', 'e', 'a', 
+'d', 'i', 'n', 'g', '_', 'c', 'o', 'm', 'm', 'e', 'n', 't', 's', '\030', '\003', ' ', '\001', '(', '\t', 'R', '\017', 'l', 'e', 'a', 'd', 
+'i', 'n', 'g', 'C', 'o', 'm', 'm', 'e', 'n', 't', 's', '\022', '+', '\n', '\021', 't', 'r', 'a', 'i', 'l', 'i', 'n', 'g', '_', 'c', 
+'o', 'm', 'm', 'e', 'n', 't', 's', '\030', '\004', ' ', '\001', '(', '\t', 'R', '\020', 't', 'r', 'a', 'i', 'l', 'i', 'n', 'g', 'C', 'o', 
+'m', 'm', 'e', 'n', 't', 's', '\022', ':', '\n', '\031', 'l', 'e', 'a', 'd', 'i', 'n', 'g', '_', 'd', 'e', 't', 'a', 'c', 'h', 'e', 
+'d', '_', 'c', 'o', 'm', 'm', 'e', 'n', 't', 's', '\030', '\006', ' ', '\003', '(', '\t', 'R', '\027', 'l', 'e', 'a', 'd', 'i', 'n', 'g', 
+'D', 'e', 't', 'a', 'c', 'h', 'e', 'd', 'C', 'o', 'm', 'm', 'e', 'n', 't', 's', '\"', '\320', '\002', '\n', '\021', 'G', 'e', 'n', 'e', 
+'r', 'a', 't', 'e', 'd', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '\022', 'M', '\n', '\n', 'a', 'n', 'n', 'o', 't', 'a', 't', 'i', 
+'o', 'n', '\030', '\001', ' ', '\003', '(', '\013', '2', '-', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
+'f', '.', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'A', 'n', 'n', 'o', 't', 
+'a', 't', 'i', 'o', 'n', 'R', '\n', 'a', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '\032', '\353', '\001', '\n', '\n', 'A', 'n', 'n', 
+'o', 't', 'a', 't', 'i', 'o', 'n', '\022', '\026', '\n', '\004', 'p', 'a', 't', 'h', '\030', '\001', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 
+'R', '\004', 'p', 'a', 't', 'h', '\022', '\037', '\n', '\013', 's', 'o', 'u', 'r', 'c', 'e', '_', 'f', 'i', 'l', 'e', '\030', '\002', ' ', '\001', 
+'(', '\t', 'R', '\n', 's', 'o', 'u', 'r', 'c', 'e', 'F', 'i', 'l', 'e', '\022', '\024', '\n', '\005', 'b', 'e', 'g', 'i', 'n', '\030', '\003', 
+' ', '\001', '(', '\005', 'R', '\005', 'b', 'e', 'g', 'i', 'n', '\022', '\020', '\n', '\003', 'e', 'n', 'd', '\030', '\004', ' ', '\001', '(', '\005', 'R', 
+'\003', 'e', 'n', 'd', '\022', 'R', '\n', '\010', 's', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\030', '\005', ' ', '\001', '(', '\016', '2', '6', '.', 
+'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 
+'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'A', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '.', 'S', 'e', 'm', 'a', 'n', 
+'t', 'i', 'c', 'R', '\010', 's', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\"', '(', '\n', '\010', 'S', 'e', 'm', 'a', 'n', 't', 'i', 'c', 
+'\022', '\010', '\n', '\004', 'N', 'O', 'N', 'E', '\020', '\000', '\022', '\007', '\n', '\003', 'S', 'E', 'T', '\020', '\001', '\022', '\t', '\n', '\005', 'A', 'L', 
+'I', 'A', 'S', '\020', '\002', '*', '\247', '\002', '\n', '\007', 'E', 'd', 'i', 't', 'i', 'o', 'n', '\022', '\023', '\n', '\017', 'E', 'D', 'I', 'T', 
+'I', 'O', 'N', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\023', '\n', '\016', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 
+'L', 'E', 'G', 'A', 'C', 'Y', '\020', '\204', '\007', '\022', '\023', '\n', '\016', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 'P', 'R', 'O', 'T', 
+'O', '2', '\020', '\346', '\007', '\022', '\023', '\n', '\016', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 'P', 'R', 'O', 'T', 'O', '3', '\020', '\347', 
+'\007', '\022', '\021', '\n', '\014', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', '2', '0', '2', '3', '\020', '\350', '\007', '\022', '\021', '\n', '\014', 'E', 
+'D', 'I', 'T', 'I', 'O', 'N', '_', '2', '0', '2', '4', '\020', '\351', '\007', '\022', '\027', '\n', '\023', 'E', 'D', 'I', 'T', 'I', 'O', 'N', 
+'_', '1', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 'L', 'Y', '\020', '\001', '\022', '\027', '\n', '\023', 'E', 'D', 'I', 'T', 'I', 'O', 'N', 
+'_', '2', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 'L', 'Y', '\020', '\002', '\022', '\035', '\n', '\027', 'E', 'D', 'I', 'T', 'I', 'O', 'N', 
+'_', '9', '9', '9', '9', '7', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 'L', 'Y', '\020', '\235', '\215', '\006', '\022', '\035', '\n', '\027', 'E', 
+'D', 'I', 'T', 'I', 'O', 'N', '_', '9', '9', '9', '9', '8', '_', 'T', 'E', 'S', 'T', '_', 'O', 'N', 'L', 'Y', '\020', '\236', '\215', 
+'\006', '\022', '\035', '\n', '\027', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', '9', '9', '9', '9', '9', '_', 'T', 'E', 'S', 'T', '_', 'O', 
+'N', 'L', 'Y', '\020', '\237', '\215', '\006', '\022', '\023', '\n', '\013', 'E', 'D', 'I', 'T', 'I', 'O', 'N', '_', 'M', 'A', 'X', '\020', '\377', '\377', 
+'\377', '\377', '\007', 'B', '~', '\n', '\023', 'c', 'o', 'm', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
+'f', 'B', '\020', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', 's', 'H', '\001', 'Z', '-', 'g', 'o', 
+'o', 'g', 'l', 'e', '.', 'g', 'o', 'l', 'a', 'n', 'g', '.', 'o', 'r', 'g', '/', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '/', 
+'t', 'y', 'p', 'e', 's', '/', 'd', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'p', 'b', '\370', '\001', '\001', '\242', '\002', '\003', 'G', 
+'P', 'B', '\252', '\002', '\032', 'G', 'o', 'o', 'g', 'l', 'e', '.', 'P', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'R', 'e', 'f', 'l', 
+'e', 'c', 't', 'i', 'o', 'n', 
 };
 
 static _upb_DefPool_Init *deps[1] = {
   NULL
 };
 
 _upb_DefPool_Init google_protobuf_descriptor_proto_upbdefinit = {
   deps,
   &google_protobuf_descriptor_proto_upb_file_layout,
   "google/protobuf/descriptor.proto",
-  UPB_STRINGVIEW_INIT(descriptor, 12155)
+  UPB_STRINGVIEW_INIT(descriptor, 12131)
 };
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/descriptor.upbdefs.h` & `protobuf-5.27.0rc3/google/protobuf/descriptor.upbdefs.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/descriptor_database.py` & `protobuf-5.27.0rc3/google/protobuf/descriptor_database.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/descriptor_pb2.py` & `protobuf-5.27.0rc3/google/protobuf/descriptor_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/descriptor.proto
-# Protobuf Python Version: 5.27.0-rc2
+# Protobuf Python Version: 5.27.0-rc3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _runtime_version.ValidateProtobufRuntimeVersion(
     _runtime_version.Domain.PUBLIC,
     5,
     27,
     0,
-    '-rc2',
+    '-rc3',
     'google/protobuf/descriptor.proto'
 )
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
@@ -28,18 +28,18 @@
   DESCRIPTOR = _descriptor.FileDescriptor(
     name='google/protobuf/descriptor.proto',
     package='google.protobuf',
     syntax='proto2',
     edition='EDITION_PROTO2',
     serialized_options=b'\n\023com.google.protobufB\020DescriptorProtosH\001Z-google.golang.org/protobuf/types/descriptorpb\370\001\001\242\002\003GPB\252\002\032Google.Protobuf.Reflection',
     create_key=_descriptor._internal_create_key,
-    serialized_pb=b'\n google/protobuf/descriptor.proto\x12\x0fgoogle.protobuf\"M\n\x11\x46ileDescriptorSet\x12\x38\n\x04\x66ile\x18\x01 \x03(\x0b\x32$.google.protobuf.FileDescriptorProtoR\x04\x66ile\"\x98\x05\n\x13\x46ileDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07package\x18\x02 \x01(\tR\x07package\x12\x1e\n\ndependency\x18\x03 \x03(\tR\ndependency\x12+\n\x11public_dependency\x18\n \x03(\x05R\x10publicDependency\x12\'\n\x0fweak_dependency\x18\x0b \x03(\x05R\x0eweakDependency\x12\x43\n\x0cmessage_type\x18\x04 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\x0bmessageType\x12\x41\n\tenum_type\x18\x05 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12\x41\n\x07service\x18\x06 \x03(\x0b\x32\'.google.protobuf.ServiceDescriptorProtoR\x07service\x12\x43\n\textension\x18\x07 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x36\n\x07options\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.FileOptionsR\x07options\x12I\n\x10source_code_info\x18\t \x01(\x0b\x32\x1f.google.protobuf.SourceCodeInfoR\x0esourceCodeInfo\x12\x16\n\x06syntax\x18\x0c \x01(\tR\x06syntax\x12\x32\n\x07\x65\x64ition\x18\x0e \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\"\xb9\x06\n\x0f\x44\x65scriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\x05\x66ield\x18\x02 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\x05\x66ield\x12\x43\n\textension\x18\x06 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x41\n\x0bnested_type\x18\x03 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\nnestedType\x12\x41\n\tenum_type\x18\x04 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12X\n\x0f\x65xtension_range\x18\x05 \x03(\x0b\x32/.google.protobuf.DescriptorProto.ExtensionRangeR\x0e\x65xtensionRange\x12\x44\n\noneof_decl\x18\x08 \x03(\x0b\x32%.google.protobuf.OneofDescriptorProtoR\toneofDecl\x12\x39\n\x07options\x18\x07 \x01(\x0b\x32\x1f.google.protobuf.MessageOptionsR\x07options\x12U\n\x0ereserved_range\x18\t \x03(\x0b\x32..google.protobuf.DescriptorProto.ReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\n \x03(\tR\x0creservedName\x1az\n\x0e\x45xtensionRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x12@\n\x07options\x18\x03 \x01(\x0b\x32&.google.protobuf.ExtensionRangeOptionsR\x07options\x1a\x37\n\rReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\xcc\x04\n\x15\x45xtensionRangeOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x12Y\n\x0b\x64\x65\x63laration\x18\x02 \x03(\x0b\x32\x32.google.protobuf.ExtensionRangeOptions.DeclarationB\x03\x88\x01\x02R\x0b\x64\x65\x63laration\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12m\n\x0cverification\x18\x03 \x01(\x0e\x32\x38.google.protobuf.ExtensionRangeOptions.VerificationState:\nUNVERIFIEDB\x03\x88\x01\x02R\x0cverification\x1a\x94\x01\n\x0b\x44\x65\x63laration\x12\x16\n\x06number\x18\x01 \x01(\x05R\x06number\x12\x1b\n\tfull_name\x18\x02 \x01(\tR\x08\x66ullName\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x12\x1a\n\x08reserved\x18\x05 \x01(\x08R\x08reserved\x12\x1a\n\x08repeated\x18\x06 \x01(\x08R\x08repeatedJ\x04\x08\x04\x10\x05\"4\n\x11VerificationState\x12\x0f\n\x0b\x44\x45\x43LARATION\x10\x00\x12\x0e\n\nUNVERIFIED\x10\x01*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xc1\x06\n\x14\x46ieldDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x41\n\x05label\x18\x04 \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.LabelR\x05label\x12>\n\x04type\x18\x05 \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.TypeR\x04type\x12\x1b\n\ttype_name\x18\x06 \x01(\tR\x08typeName\x12\x1a\n\x08\x65xtendee\x18\x02 \x01(\tR\x08\x65xtendee\x12#\n\rdefault_value\x18\x07 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1f\n\x0boneof_index\x18\t \x01(\x05R\noneofIndex\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12\x37\n\x07options\x18\x08 \x01(\x0b\x32\x1d.google.protobuf.FieldOptionsR\x07options\x12\'\n\x0fproto3_optional\x18\x11 \x01(\x08R\x0eproto3Optional\"\xb6\x02\n\x04Type\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"C\n\x05Label\x12\x12\n\x0eLABEL_OPTIONAL\x10\x01\x12\x12\n\x0eLABEL_REPEATED\x10\x03\x12\x12\n\x0eLABEL_REQUIRED\x10\x02\"c\n\x14OneofDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x37\n\x07options\x18\x02 \x01(\x0b\x32\x1d.google.protobuf.OneofOptionsR\x07options\"\xe3\x02\n\x13\x45numDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x05value\x18\x02 \x03(\x0b\x32).google.protobuf.EnumValueDescriptorProtoR\x05value\x12\x36\n\x07options\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.EnumOptionsR\x07options\x12]\n\x0ereserved_range\x18\x04 \x03(\x0b\x32\x36.google.protobuf.EnumDescriptorProto.EnumReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\x05 \x03(\tR\x0creservedName\x1a;\n\x11\x45numReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\x83\x01\n\x18\x45numValueDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12;\n\x07options\x18\x03 \x01(\x0b\x32!.google.protobuf.EnumValueOptionsR\x07options\"\xa7\x01\n\x16ServiceDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x06method\x18\x02 \x03(\x0b\x32&.google.protobuf.MethodDescriptorProtoR\x06method\x12\x39\n\x07options\x18\x03 \x01(\x0b\x32\x1f.google.protobuf.ServiceOptionsR\x07options\"\x89\x02\n\x15MethodDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ninput_type\x18\x02 \x01(\tR\tinputType\x12\x1f\n\x0boutput_type\x18\x03 \x01(\tR\noutputType\x12\x38\n\x07options\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.MethodOptionsR\x07options\x12\x30\n\x10\x63lient_streaming\x18\x05 \x01(\x08:\x05\x66\x61lseR\x0f\x63lientStreaming\x12\x30\n\x10server_streaming\x18\x06 \x01(\x08:\x05\x66\x61lseR\x0fserverStreaming\"\x97\t\n\x0b\x46ileOptions\x12!\n\x0cjava_package\x18\x01 \x01(\tR\x0bjavaPackage\x12\x30\n\x14java_outer_classname\x18\x08 \x01(\tR\x12javaOuterClassname\x12\x35\n\x13java_multiple_files\x18\n \x01(\x08:\x05\x66\x61lseR\x11javaMultipleFiles\x12\x44\n\x1djava_generate_equals_and_hash\x18\x14 \x01(\x08\x42\x02\x18\x01R\x19javaGenerateEqualsAndHash\x12:\n\x16java_string_check_utf8\x18\x1b \x01(\x08:\x05\x66\x61lseR\x13javaStringCheckUtf8\x12S\n\x0coptimize_for\x18\t \x01(\x0e\x32).google.protobuf.FileOptions.OptimizeMode:\x05SPEEDR\x0boptimizeFor\x12\x1d\n\ngo_package\x18\x0b \x01(\tR\tgoPackage\x12\x35\n\x13\x63\x63_generic_services\x18\x10 \x01(\x08:\x05\x66\x61lseR\x11\x63\x63GenericServices\x12\x39\n\x15java_generic_services\x18\x11 \x01(\x08:\x05\x66\x61lseR\x13javaGenericServices\x12\x35\n\x13py_generic_services\x18\x12 \x01(\x08:\x05\x66\x61lseR\x11pyGenericServices\x12%\n\ndeprecated\x18\x17 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12.\n\x10\x63\x63_enable_arenas\x18\x1f \x01(\x08:\x04trueR\x0e\x63\x63\x45nableArenas\x12*\n\x11objc_class_prefix\x18$ \x01(\tR\x0fobjcClassPrefix\x12)\n\x10\x63sharp_namespace\x18% \x01(\tR\x0f\x63sharpNamespace\x12!\n\x0cswift_prefix\x18\' \x01(\tR\x0bswiftPrefix\x12(\n\x10php_class_prefix\x18( \x01(\tR\x0ephpClassPrefix\x12#\n\rphp_namespace\x18) \x01(\tR\x0cphpNamespace\x12\x34\n\x16php_metadata_namespace\x18, \x01(\tR\x14phpMetadataNamespace\x12!\n\x0cruby_package\x18- \x01(\tR\x0brubyPackage\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\":\n\x0cOptimizeMode\x12\t\n\x05SPEED\x10\x01\x12\r\n\tCODE_SIZE\x10\x02\x12\x10\n\x0cLITE_RUNTIME\x10\x03*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08*\x10+J\x04\x08&\x10\'\"\xf4\x03\n\x0eMessageOptions\x12<\n\x17message_set_wire_format\x18\x01 \x01(\x08:\x05\x66\x61lseR\x14messageSetWireFormat\x12L\n\x1fno_standard_descriptor_accessor\x18\x02 \x01(\x08:\x05\x66\x61lseR\x1cnoStandardDescriptorAccessor\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x1b\n\tmap_entry\x18\x07 \x01(\x08R\x08mapEntry\x12V\n&deprecated_legacy_json_field_conflicts\x18\x0b \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\x9d\r\n\x0c\x46ieldOptions\x12\x41\n\x05\x63type\x18\x01 \x01(\x0e\x32#.google.protobuf.FieldOptions.CType:\x06STRINGR\x05\x63type\x12\x16\n\x06packed\x18\x02 \x01(\x08R\x06packed\x12G\n\x06jstype\x18\x06 \x01(\x0e\x32$.google.protobuf.FieldOptions.JSType:\tJS_NORMALR\x06jstype\x12\x19\n\x04lazy\x18\x05 \x01(\x08:\x05\x66\x61lseR\x04lazy\x12.\n\x0funverified_lazy\x18\x0f \x01(\x08:\x05\x66\x61lseR\x0eunverifiedLazy\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x19\n\x04weak\x18\n \x01(\x08:\x05\x66\x61lseR\x04weak\x12(\n\x0c\x64\x65\x62ug_redact\x18\x10 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12K\n\tretention\x18\x11 \x01(\x0e\x32-.google.protobuf.FieldOptions.OptionRetentionR\tretention\x12H\n\x07targets\x18\x13 \x03(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeR\x07targets\x12W\n\x10\x65\x64ition_defaults\x18\x14 \x03(\x0b\x32,.google.protobuf.FieldOptions.EditionDefaultR\x0f\x65\x64itionDefaults\x12\x37\n\x08\x66\x65\x61tures\x18\x15 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12U\n\x0f\x66\x65\x61ture_support\x18\x16 \x01(\x0b\x32,.google.protobuf.FieldOptions.FeatureSupportR\x0e\x66\x65\x61tureSupport\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x1aZ\n\x0e\x45\x64itionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\x1a\x96\x02\n\x0e\x46\x65\x61tureSupport\x12G\n\x12\x65\x64ition_introduced\x18\x01 \x01(\x0e\x32\x18.google.protobuf.EditionR\x11\x65\x64itionIntroduced\x12G\n\x12\x65\x64ition_deprecated\x18\x02 \x01(\x0e\x32\x18.google.protobuf.EditionR\x11\x65\x64itionDeprecated\x12/\n\x13\x64\x65precation_warning\x18\x03 \x01(\tR\x12\x64\x65precationWarning\x12\x41\n\x0f\x65\x64ition_removed\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0e\x65\x64itionRemoved\"/\n\x05\x43Type\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x43ORD\x10\x01\x12\x10\n\x0cSTRING_PIECE\x10\x02\"5\n\x06JSType\x12\r\n\tJS_NORMAL\x10\x00\x12\r\n\tJS_STRING\x10\x01\x12\r\n\tJS_NUMBER\x10\x02\"U\n\x0fOptionRetention\x12\x15\n\x11RETENTION_UNKNOWN\x10\x00\x12\x15\n\x11RETENTION_RUNTIME\x10\x01\x12\x14\n\x10RETENTION_SOURCE\x10\x02\"\x8c\x02\n\x10OptionTargetType\x12\x17\n\x13TARGET_TYPE_UNKNOWN\x10\x00\x12\x14\n\x10TARGET_TYPE_FILE\x10\x01\x12\x1f\n\x1bTARGET_TYPE_EXTENSION_RANGE\x10\x02\x12\x17\n\x13TARGET_TYPE_MESSAGE\x10\x03\x12\x15\n\x11TARGET_TYPE_FIELD\x10\x04\x12\x15\n\x11TARGET_TYPE_ONEOF\x10\x05\x12\x14\n\x10TARGET_TYPE_ENUM\x10\x06\x12\x1a\n\x16TARGET_TYPE_ENUM_ENTRY\x10\x07\x12\x17\n\x13TARGET_TYPE_SERVICE\x10\x08\x12\x16\n\x12TARGET_TYPE_METHOD\x10\t*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x12\x10\x13\"\xac\x01\n\x0cOneofOptions\x12\x37\n\x08\x66\x65\x61tures\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd1\x02\n\x0b\x45numOptions\x12\x1f\n\x0b\x61llow_alias\x18\x02 \x01(\x08R\nallowAlias\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12V\n&deprecated_legacy_json_field_conflicts\x18\x06 \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x05\x10\x06\"\x81\x02\n\x10\x45numValueOptions\x12%\n\ndeprecated\x18\x01 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x37\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12(\n\x0c\x64\x65\x62ug_redact\x18\x03 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd5\x01\n\x0eServiceOptions\x12\x37\n\x08\x66\x65\x61tures\x18\" \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x99\x03\n\rMethodOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12q\n\x11idempotency_level\x18\" \x01(\x0e\x32/.google.protobuf.MethodOptions.IdempotencyLevel:\x13IDEMPOTENCY_UNKNOWNR\x10idempotencyLevel\x12\x37\n\x08\x66\x65\x61tures\x18# \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"P\n\x10IdempotencyLevel\x12\x17\n\x13IDEMPOTENCY_UNKNOWN\x10\x00\x12\x13\n\x0fNO_SIDE_EFFECTS\x10\x01\x12\x0e\n\nIDEMPOTENT\x10\x02*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9a\x03\n\x13UninterpretedOption\x12\x41\n\x04name\x18\x02 \x03(\x0b\x32-.google.protobuf.UninterpretedOption.NamePartR\x04name\x12)\n\x10identifier_value\x18\x03 \x01(\tR\x0fidentifierValue\x12,\n\x12positive_int_value\x18\x04 \x01(\x04R\x10positiveIntValue\x12,\n\x12negative_int_value\x18\x05 \x01(\x03R\x10negativeIntValue\x12!\n\x0c\x64ouble_value\x18\x06 \x01(\x01R\x0b\x64oubleValue\x12!\n\x0cstring_value\x18\x07 \x01(\x0cR\x0bstringValue\x12\'\n\x0f\x61ggregate_value\x18\x08 \x01(\tR\x0e\x61ggregateValue\x1aJ\n\x08NamePart\x12\x1b\n\tname_part\x18\x01 \x02(\tR\x08namePart\x12!\n\x0cis_extension\x18\x02 \x02(\x08R\x0bisExtension\"\xb9\n\n\nFeatureSet\x12\x91\x01\n\x0e\x66ield_presence\x18\x01 \x01(\x0e\x32).google.protobuf.FeatureSet.FieldPresenceB?\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe6\x07\xa2\x01\r\x12\x08IMPLICIT\x18\xe7\x07\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe8\x07\xb2\x01\x03\x08\xe8\x07R\rfieldPresence\x12l\n\tenum_type\x18\x02 \x01(\x0e\x32$.google.protobuf.FeatureSet.EnumTypeB)\x88\x01\x01\x98\x01\x06\x98\x01\x01\xa2\x01\x0b\x12\x06\x43LOSED\x18\xe6\x07\xa2\x01\t\x12\x04OPEN\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x08\x65numType\x12\x98\x01\n\x17repeated_field_encoding\x18\x03 \x01(\x0e\x32\x31.google.protobuf.FeatureSet.RepeatedFieldEncodingB-\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPANDED\x18\xe6\x07\xa2\x01\x0b\x12\x06PACKED\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x15repeatedFieldEncoding\x12~\n\x0futf8_validation\x18\x04 \x01(\x0e\x32*.google.protobuf.FeatureSet.Utf8ValidationB)\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\t\x12\x04NONE\x18\xe6\x07\xa2\x01\x0b\x12\x06VERIFY\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x0eutf8Validation\x12~\n\x10message_encoding\x18\x05 \x01(\x0e\x32+.google.protobuf.FeatureSet.MessageEncodingB&\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\x14\x12\x0fLENGTH_PREFIXED\x18\xe6\x07\xb2\x01\x03\x08\xe8\x07R\x0fmessageEncoding\x12\x82\x01\n\x0bjson_format\x18\x06 \x01(\x0e\x32&.google.protobuf.FeatureSet.JsonFormatB9\x88\x01\x01\x98\x01\x03\x98\x01\x06\x98\x01\x01\xa2\x01\x17\x12\x12LEGACY_BEST_EFFORT\x18\xe6\x07\xa2\x01\n\x12\x05\x41LLOW\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\njsonFormat\"\\\n\rFieldPresence\x12\x1a\n\x16\x46IELD_PRESENCE_UNKNOWN\x10\x00\x12\x0c\n\x08\x45XPLICIT\x10\x01\x12\x0c\n\x08IMPLICIT\x10\x02\x12\x13\n\x0fLEGACY_REQUIRED\x10\x03\"7\n\x08\x45numType\x12\x15\n\x11\x45NUM_TYPE_UNKNOWN\x10\x00\x12\x08\n\x04OPEN\x10\x01\x12\n\n\x06\x43LOSED\x10\x02\"V\n\x15RepeatedFieldEncoding\x12#\n\x1fREPEATED_FIELD_ENCODING_UNKNOWN\x10\x00\x12\n\n\x06PACKED\x10\x01\x12\x0c\n\x08\x45XPANDED\x10\x02\"C\n\x0eUtf8Validation\x12\x1b\n\x17UTF8_VALIDATION_UNKNOWN\x10\x00\x12\n\n\x06VERIFY\x10\x02\x12\x08\n\x04NONE\x10\x03\"S\n\x0fMessageEncoding\x12\x1c\n\x18MESSAGE_ENCODING_UNKNOWN\x10\x00\x12\x13\n\x0fLENGTH_PREFIXED\x10\x01\x12\r\n\tDELIMITED\x10\x02\"H\n\nJsonFormat\x12\x17\n\x13JSON_FORMAT_UNKNOWN\x10\x00\x12\t\n\x05\x41LLOW\x10\x01\x12\x16\n\x12LEGACY_BEST_EFFORT\x10\x02*\x06\x08\xe8\x07\x10\xe9\x07*\x06\x08\xe9\x07\x10\xea\x07*\x06\x08\xea\x07\x10\xeb\x07*\x06\x08\x86N\x10\x87N*\x06\x08\x8bN\x10\x90N*\x06\x08\x90N\x10\x91NJ\x06\x08\xe7\x07\x10\xe8\x07\"\xd9\x03\n\x12\x46\x65\x61tureSetDefaults\x12X\n\x08\x64\x65\x66\x61ults\x18\x01 \x03(\x0b\x32<.google.protobuf.FeatureSetDefaults.FeatureSetEditionDefaultR\x08\x64\x65\x66\x61ults\x12\x41\n\x0fminimum_edition\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0eminimumEdition\x12\x41\n\x0fmaximum_edition\x18\x05 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0emaximumEdition\x1a\xe2\x01\n\x18\x46\x65\x61tureSetEditionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12N\n\x14overridable_features\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x13overridableFeatures\x12\x42\n\x0e\x66ixed_features\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\rfixedFeatures\"\xa7\x02\n\x0eSourceCodeInfo\x12\x44\n\x08location\x18\x01 \x03(\x0b\x32(.google.protobuf.SourceCodeInfo.LocationR\x08location\x1a\xce\x01\n\x08Location\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x16\n\x04span\x18\x02 \x03(\x05\x42\x02\x10\x01R\x04span\x12)\n\x10leading_comments\x18\x03 \x01(\tR\x0fleadingComments\x12+\n\x11trailing_comments\x18\x04 \x01(\tR\x10trailingComments\x12:\n\x19leading_detached_comments\x18\x06 \x03(\tR\x17leadingDetachedComments\"\xd0\x02\n\x11GeneratedCodeInfo\x12M\n\nannotation\x18\x01 \x03(\x0b\x32-.google.protobuf.GeneratedCodeInfo.AnnotationR\nannotation\x1a\xeb\x01\n\nAnnotation\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x1f\n\x0bsource_file\x18\x02 \x01(\tR\nsourceFile\x12\x14\n\x05\x62\x65gin\x18\x03 \x01(\x05R\x05\x62\x65gin\x12\x10\n\x03\x65nd\x18\x04 \x01(\x05R\x03\x65nd\x12R\n\x08semantic\x18\x05 \x01(\x0e\x32\x36.google.protobuf.GeneratedCodeInfo.Annotation.SemanticR\x08semantic\"(\n\x08Semantic\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SET\x10\x01\x12\t\n\x05\x41LIAS\x10\x02*\xa7\x02\n\x07\x45\x64ition\x12\x13\n\x0f\x45\x44ITION_UNKNOWN\x10\x00\x12\x13\n\x0e\x45\x44ITION_LEGACY\x10\x84\x07\x12\x13\n\x0e\x45\x44ITION_PROTO2\x10\xe6\x07\x12\x13\n\x0e\x45\x44ITION_PROTO3\x10\xe7\x07\x12\x11\n\x0c\x45\x44ITION_2023\x10\xe8\x07\x12\x11\n\x0c\x45\x44ITION_2024\x10\xe9\x07\x12\x17\n\x13\x45\x44ITION_1_TEST_ONLY\x10\x01\x12\x17\n\x13\x45\x44ITION_2_TEST_ONLY\x10\x02\x12\x1d\n\x17\x45\x44ITION_99997_TEST_ONLY\x10\x9d\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99998_TEST_ONLY\x10\x9e\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99999_TEST_ONLY\x10\x9f\x8d\x06\x12\x13\n\x0b\x45\x44ITION_MAX\x10\xff\xff\xff\xff\x07\x42~\n\x13\x63om.google.protobufB\x10\x44\x65scriptorProtosH\x01Z-google.golang.org/protobuf/types/descriptorpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1aGoogle.Protobuf.Reflection'
+    serialized_pb=b'\n google/protobuf/descriptor.proto\x12\x0fgoogle.protobuf\"M\n\x11\x46ileDescriptorSet\x12\x38\n\x04\x66ile\x18\x01 \x03(\x0b\x32$.google.protobuf.FileDescriptorProtoR\x04\x66ile\"\x98\x05\n\x13\x46ileDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07package\x18\x02 \x01(\tR\x07package\x12\x1e\n\ndependency\x18\x03 \x03(\tR\ndependency\x12+\n\x11public_dependency\x18\n \x03(\x05R\x10publicDependency\x12\'\n\x0fweak_dependency\x18\x0b \x03(\x05R\x0eweakDependency\x12\x43\n\x0cmessage_type\x18\x04 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\x0bmessageType\x12\x41\n\tenum_type\x18\x05 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12\x41\n\x07service\x18\x06 \x03(\x0b\x32\'.google.protobuf.ServiceDescriptorProtoR\x07service\x12\x43\n\textension\x18\x07 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x36\n\x07options\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.FileOptionsR\x07options\x12I\n\x10source_code_info\x18\t \x01(\x0b\x32\x1f.google.protobuf.SourceCodeInfoR\x0esourceCodeInfo\x12\x16\n\x06syntax\x18\x0c \x01(\tR\x06syntax\x12\x32\n\x07\x65\x64ition\x18\x0e \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\"\xb9\x06\n\x0f\x44\x65scriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\x05\x66ield\x18\x02 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\x05\x66ield\x12\x43\n\textension\x18\x06 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x41\n\x0bnested_type\x18\x03 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\nnestedType\x12\x41\n\tenum_type\x18\x04 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12X\n\x0f\x65xtension_range\x18\x05 \x03(\x0b\x32/.google.protobuf.DescriptorProto.ExtensionRangeR\x0e\x65xtensionRange\x12\x44\n\noneof_decl\x18\x08 \x03(\x0b\x32%.google.protobuf.OneofDescriptorProtoR\toneofDecl\x12\x39\n\x07options\x18\x07 \x01(\x0b\x32\x1f.google.protobuf.MessageOptionsR\x07options\x12U\n\x0ereserved_range\x18\t \x03(\x0b\x32..google.protobuf.DescriptorProto.ReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\n \x03(\tR\x0creservedName\x1az\n\x0e\x45xtensionRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x12@\n\x07options\x18\x03 \x01(\x0b\x32&.google.protobuf.ExtensionRangeOptionsR\x07options\x1a\x37\n\rReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\xcc\x04\n\x15\x45xtensionRangeOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x12Y\n\x0b\x64\x65\x63laration\x18\x02 \x03(\x0b\x32\x32.google.protobuf.ExtensionRangeOptions.DeclarationB\x03\x88\x01\x02R\x0b\x64\x65\x63laration\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12m\n\x0cverification\x18\x03 \x01(\x0e\x32\x38.google.protobuf.ExtensionRangeOptions.VerificationState:\nUNVERIFIEDB\x03\x88\x01\x02R\x0cverification\x1a\x94\x01\n\x0b\x44\x65\x63laration\x12\x16\n\x06number\x18\x01 \x01(\x05R\x06number\x12\x1b\n\tfull_name\x18\x02 \x01(\tR\x08\x66ullName\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x12\x1a\n\x08reserved\x18\x05 \x01(\x08R\x08reserved\x12\x1a\n\x08repeated\x18\x06 \x01(\x08R\x08repeatedJ\x04\x08\x04\x10\x05\"4\n\x11VerificationState\x12\x0f\n\x0b\x44\x45\x43LARATION\x10\x00\x12\x0e\n\nUNVERIFIED\x10\x01*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xc1\x06\n\x14\x46ieldDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x41\n\x05label\x18\x04 \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.LabelR\x05label\x12>\n\x04type\x18\x05 \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.TypeR\x04type\x12\x1b\n\ttype_name\x18\x06 \x01(\tR\x08typeName\x12\x1a\n\x08\x65xtendee\x18\x02 \x01(\tR\x08\x65xtendee\x12#\n\rdefault_value\x18\x07 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1f\n\x0boneof_index\x18\t \x01(\x05R\noneofIndex\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12\x37\n\x07options\x18\x08 \x01(\x0b\x32\x1d.google.protobuf.FieldOptionsR\x07options\x12\'\n\x0fproto3_optional\x18\x11 \x01(\x08R\x0eproto3Optional\"\xb6\x02\n\x04Type\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"C\n\x05Label\x12\x12\n\x0eLABEL_OPTIONAL\x10\x01\x12\x12\n\x0eLABEL_REPEATED\x10\x03\x12\x12\n\x0eLABEL_REQUIRED\x10\x02\"c\n\x14OneofDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x37\n\x07options\x18\x02 \x01(\x0b\x32\x1d.google.protobuf.OneofOptionsR\x07options\"\xe3\x02\n\x13\x45numDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x05value\x18\x02 \x03(\x0b\x32).google.protobuf.EnumValueDescriptorProtoR\x05value\x12\x36\n\x07options\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.EnumOptionsR\x07options\x12]\n\x0ereserved_range\x18\x04 \x03(\x0b\x32\x36.google.protobuf.EnumDescriptorProto.EnumReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\x05 \x03(\tR\x0creservedName\x1a;\n\x11\x45numReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\x83\x01\n\x18\x45numValueDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12;\n\x07options\x18\x03 \x01(\x0b\x32!.google.protobuf.EnumValueOptionsR\x07options\"\xa7\x01\n\x16ServiceDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x06method\x18\x02 \x03(\x0b\x32&.google.protobuf.MethodDescriptorProtoR\x06method\x12\x39\n\x07options\x18\x03 \x01(\x0b\x32\x1f.google.protobuf.ServiceOptionsR\x07options\"\x89\x02\n\x15MethodDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ninput_type\x18\x02 \x01(\tR\tinputType\x12\x1f\n\x0boutput_type\x18\x03 \x01(\tR\noutputType\x12\x38\n\x07options\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.MethodOptionsR\x07options\x12\x30\n\x10\x63lient_streaming\x18\x05 \x01(\x08:\x05\x66\x61lseR\x0f\x63lientStreaming\x12\x30\n\x10server_streaming\x18\x06 \x01(\x08:\x05\x66\x61lseR\x0fserverStreaming\"\x97\t\n\x0b\x46ileOptions\x12!\n\x0cjava_package\x18\x01 \x01(\tR\x0bjavaPackage\x12\x30\n\x14java_outer_classname\x18\x08 \x01(\tR\x12javaOuterClassname\x12\x35\n\x13java_multiple_files\x18\n \x01(\x08:\x05\x66\x61lseR\x11javaMultipleFiles\x12\x44\n\x1djava_generate_equals_and_hash\x18\x14 \x01(\x08\x42\x02\x18\x01R\x19javaGenerateEqualsAndHash\x12:\n\x16java_string_check_utf8\x18\x1b \x01(\x08:\x05\x66\x61lseR\x13javaStringCheckUtf8\x12S\n\x0coptimize_for\x18\t \x01(\x0e\x32).google.protobuf.FileOptions.OptimizeMode:\x05SPEEDR\x0boptimizeFor\x12\x1d\n\ngo_package\x18\x0b \x01(\tR\tgoPackage\x12\x35\n\x13\x63\x63_generic_services\x18\x10 \x01(\x08:\x05\x66\x61lseR\x11\x63\x63GenericServices\x12\x39\n\x15java_generic_services\x18\x11 \x01(\x08:\x05\x66\x61lseR\x13javaGenericServices\x12\x35\n\x13py_generic_services\x18\x12 \x01(\x08:\x05\x66\x61lseR\x11pyGenericServices\x12%\n\ndeprecated\x18\x17 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12.\n\x10\x63\x63_enable_arenas\x18\x1f \x01(\x08:\x04trueR\x0e\x63\x63\x45nableArenas\x12*\n\x11objc_class_prefix\x18$ \x01(\tR\x0fobjcClassPrefix\x12)\n\x10\x63sharp_namespace\x18% \x01(\tR\x0f\x63sharpNamespace\x12!\n\x0cswift_prefix\x18\' \x01(\tR\x0bswiftPrefix\x12(\n\x10php_class_prefix\x18( \x01(\tR\x0ephpClassPrefix\x12#\n\rphp_namespace\x18) \x01(\tR\x0cphpNamespace\x12\x34\n\x16php_metadata_namespace\x18, \x01(\tR\x14phpMetadataNamespace\x12!\n\x0cruby_package\x18- \x01(\tR\x0brubyPackage\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\":\n\x0cOptimizeMode\x12\t\n\x05SPEED\x10\x01\x12\r\n\tCODE_SIZE\x10\x02\x12\x10\n\x0cLITE_RUNTIME\x10\x03*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08*\x10+J\x04\x08&\x10\'\"\xf4\x03\n\x0eMessageOptions\x12<\n\x17message_set_wire_format\x18\x01 \x01(\x08:\x05\x66\x61lseR\x14messageSetWireFormat\x12L\n\x1fno_standard_descriptor_accessor\x18\x02 \x01(\x08:\x05\x66\x61lseR\x1cnoStandardDescriptorAccessor\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x1b\n\tmap_entry\x18\x07 \x01(\x08R\x08mapEntry\x12V\n&deprecated_legacy_json_field_conflicts\x18\x0b \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\x9d\r\n\x0c\x46ieldOptions\x12\x41\n\x05\x63type\x18\x01 \x01(\x0e\x32#.google.protobuf.FieldOptions.CType:\x06STRINGR\x05\x63type\x12\x16\n\x06packed\x18\x02 \x01(\x08R\x06packed\x12G\n\x06jstype\x18\x06 \x01(\x0e\x32$.google.protobuf.FieldOptions.JSType:\tJS_NORMALR\x06jstype\x12\x19\n\x04lazy\x18\x05 \x01(\x08:\x05\x66\x61lseR\x04lazy\x12.\n\x0funverified_lazy\x18\x0f \x01(\x08:\x05\x66\x61lseR\x0eunverifiedLazy\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x19\n\x04weak\x18\n \x01(\x08:\x05\x66\x61lseR\x04weak\x12(\n\x0c\x64\x65\x62ug_redact\x18\x10 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12K\n\tretention\x18\x11 \x01(\x0e\x32-.google.protobuf.FieldOptions.OptionRetentionR\tretention\x12H\n\x07targets\x18\x13 \x03(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeR\x07targets\x12W\n\x10\x65\x64ition_defaults\x18\x14 \x03(\x0b\x32,.google.protobuf.FieldOptions.EditionDefaultR\x0f\x65\x64itionDefaults\x12\x37\n\x08\x66\x65\x61tures\x18\x15 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12U\n\x0f\x66\x65\x61ture_support\x18\x16 \x01(\x0b\x32,.google.protobuf.FieldOptions.FeatureSupportR\x0e\x66\x65\x61tureSupport\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x1aZ\n\x0e\x45\x64itionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\x1a\x96\x02\n\x0e\x46\x65\x61tureSupport\x12G\n\x12\x65\x64ition_introduced\x18\x01 \x01(\x0e\x32\x18.google.protobuf.EditionR\x11\x65\x64itionIntroduced\x12G\n\x12\x65\x64ition_deprecated\x18\x02 \x01(\x0e\x32\x18.google.protobuf.EditionR\x11\x65\x64itionDeprecated\x12/\n\x13\x64\x65precation_warning\x18\x03 \x01(\tR\x12\x64\x65precationWarning\x12\x41\n\x0f\x65\x64ition_removed\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0e\x65\x64itionRemoved\"/\n\x05\x43Type\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x43ORD\x10\x01\x12\x10\n\x0cSTRING_PIECE\x10\x02\"5\n\x06JSType\x12\r\n\tJS_NORMAL\x10\x00\x12\r\n\tJS_STRING\x10\x01\x12\r\n\tJS_NUMBER\x10\x02\"U\n\x0fOptionRetention\x12\x15\n\x11RETENTION_UNKNOWN\x10\x00\x12\x15\n\x11RETENTION_RUNTIME\x10\x01\x12\x14\n\x10RETENTION_SOURCE\x10\x02\"\x8c\x02\n\x10OptionTargetType\x12\x17\n\x13TARGET_TYPE_UNKNOWN\x10\x00\x12\x14\n\x10TARGET_TYPE_FILE\x10\x01\x12\x1f\n\x1bTARGET_TYPE_EXTENSION_RANGE\x10\x02\x12\x17\n\x13TARGET_TYPE_MESSAGE\x10\x03\x12\x15\n\x11TARGET_TYPE_FIELD\x10\x04\x12\x15\n\x11TARGET_TYPE_ONEOF\x10\x05\x12\x14\n\x10TARGET_TYPE_ENUM\x10\x06\x12\x1a\n\x16TARGET_TYPE_ENUM_ENTRY\x10\x07\x12\x17\n\x13TARGET_TYPE_SERVICE\x10\x08\x12\x16\n\x12TARGET_TYPE_METHOD\x10\t*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x12\x10\x13\"\xac\x01\n\x0cOneofOptions\x12\x37\n\x08\x66\x65\x61tures\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd1\x02\n\x0b\x45numOptions\x12\x1f\n\x0b\x61llow_alias\x18\x02 \x01(\x08R\nallowAlias\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12V\n&deprecated_legacy_json_field_conflicts\x18\x06 \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x05\x10\x06\"\x81\x02\n\x10\x45numValueOptions\x12%\n\ndeprecated\x18\x01 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x37\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12(\n\x0c\x64\x65\x62ug_redact\x18\x03 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd5\x01\n\x0eServiceOptions\x12\x37\n\x08\x66\x65\x61tures\x18\" \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x99\x03\n\rMethodOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12q\n\x11idempotency_level\x18\" \x01(\x0e\x32/.google.protobuf.MethodOptions.IdempotencyLevel:\x13IDEMPOTENCY_UNKNOWNR\x10idempotencyLevel\x12\x37\n\x08\x66\x65\x61tures\x18# \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"P\n\x10IdempotencyLevel\x12\x17\n\x13IDEMPOTENCY_UNKNOWN\x10\x00\x12\x13\n\x0fNO_SIDE_EFFECTS\x10\x01\x12\x0e\n\nIDEMPOTENT\x10\x02*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9a\x03\n\x13UninterpretedOption\x12\x41\n\x04name\x18\x02 \x03(\x0b\x32-.google.protobuf.UninterpretedOption.NamePartR\x04name\x12)\n\x10identifier_value\x18\x03 \x01(\tR\x0fidentifierValue\x12,\n\x12positive_int_value\x18\x04 \x01(\x04R\x10positiveIntValue\x12,\n\x12negative_int_value\x18\x05 \x01(\x03R\x10negativeIntValue\x12!\n\x0c\x64ouble_value\x18\x06 \x01(\x01R\x0b\x64oubleValue\x12!\n\x0cstring_value\x18\x07 \x01(\x0cR\x0bstringValue\x12\'\n\x0f\x61ggregate_value\x18\x08 \x01(\tR\x0e\x61ggregateValue\x1aJ\n\x08NamePart\x12\x1b\n\tname_part\x18\x01 \x02(\tR\x08namePart\x12!\n\x0cis_extension\x18\x02 \x02(\x08R\x0bisExtension\"\xa1\n\n\nFeatureSet\x12\x91\x01\n\x0e\x66ield_presence\x18\x01 \x01(\x0e\x32).google.protobuf.FeatureSet.FieldPresenceB?\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe6\x07\xa2\x01\r\x12\x08IMPLICIT\x18\xe7\x07\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe8\x07\xb2\x01\x03\x08\xe8\x07R\rfieldPresence\x12l\n\tenum_type\x18\x02 \x01(\x0e\x32$.google.protobuf.FeatureSet.EnumTypeB)\x88\x01\x01\x98\x01\x06\x98\x01\x01\xa2\x01\x0b\x12\x06\x43LOSED\x18\xe6\x07\xa2\x01\t\x12\x04OPEN\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x08\x65numType\x12\x98\x01\n\x17repeated_field_encoding\x18\x03 \x01(\x0e\x32\x31.google.protobuf.FeatureSet.RepeatedFieldEncodingB-\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPANDED\x18\xe6\x07\xa2\x01\x0b\x12\x06PACKED\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x15repeatedFieldEncoding\x12~\n\x0futf8_validation\x18\x04 \x01(\x0e\x32*.google.protobuf.FeatureSet.Utf8ValidationB)\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\t\x12\x04NONE\x18\xe6\x07\xa2\x01\x0b\x12\x06VERIFY\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x0eutf8Validation\x12~\n\x10message_encoding\x18\x05 \x01(\x0e\x32+.google.protobuf.FeatureSet.MessageEncodingB&\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\x14\x12\x0fLENGTH_PREFIXED\x18\xe6\x07\xb2\x01\x03\x08\xe8\x07R\x0fmessageEncoding\x12\x82\x01\n\x0bjson_format\x18\x06 \x01(\x0e\x32&.google.protobuf.FeatureSet.JsonFormatB9\x88\x01\x01\x98\x01\x03\x98\x01\x06\x98\x01\x01\xa2\x01\x17\x12\x12LEGACY_BEST_EFFORT\x18\xe6\x07\xa2\x01\n\x12\x05\x41LLOW\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\njsonFormat\"\\\n\rFieldPresence\x12\x1a\n\x16\x46IELD_PRESENCE_UNKNOWN\x10\x00\x12\x0c\n\x08\x45XPLICIT\x10\x01\x12\x0c\n\x08IMPLICIT\x10\x02\x12\x13\n\x0fLEGACY_REQUIRED\x10\x03\"7\n\x08\x45numType\x12\x15\n\x11\x45NUM_TYPE_UNKNOWN\x10\x00\x12\x08\n\x04OPEN\x10\x01\x12\n\n\x06\x43LOSED\x10\x02\"V\n\x15RepeatedFieldEncoding\x12#\n\x1fREPEATED_FIELD_ENCODING_UNKNOWN\x10\x00\x12\n\n\x06PACKED\x10\x01\x12\x0c\n\x08\x45XPANDED\x10\x02\"C\n\x0eUtf8Validation\x12\x1b\n\x17UTF8_VALIDATION_UNKNOWN\x10\x00\x12\n\n\x06VERIFY\x10\x02\x12\x08\n\x04NONE\x10\x03\"S\n\x0fMessageEncoding\x12\x1c\n\x18MESSAGE_ENCODING_UNKNOWN\x10\x00\x12\x13\n\x0fLENGTH_PREFIXED\x10\x01\x12\r\n\tDELIMITED\x10\x02\"H\n\nJsonFormat\x12\x17\n\x13JSON_FORMAT_UNKNOWN\x10\x00\x12\t\n\x05\x41LLOW\x10\x01\x12\x16\n\x12LEGACY_BEST_EFFORT\x10\x02*\x06\x08\xe8\x07\x10\x8bN*\x06\x08\x8bN\x10\x90N*\x06\x08\x90N\x10\x91NJ\x06\x08\xe7\x07\x10\xe8\x07\"\xd9\x03\n\x12\x46\x65\x61tureSetDefaults\x12X\n\x08\x64\x65\x66\x61ults\x18\x01 \x03(\x0b\x32<.google.protobuf.FeatureSetDefaults.FeatureSetEditionDefaultR\x08\x64\x65\x66\x61ults\x12\x41\n\x0fminimum_edition\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0eminimumEdition\x12\x41\n\x0fmaximum_edition\x18\x05 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0emaximumEdition\x1a\xe2\x01\n\x18\x46\x65\x61tureSetEditionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12N\n\x14overridable_features\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x13overridableFeatures\x12\x42\n\x0e\x66ixed_features\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\rfixedFeatures\"\xa7\x02\n\x0eSourceCodeInfo\x12\x44\n\x08location\x18\x01 \x03(\x0b\x32(.google.protobuf.SourceCodeInfo.LocationR\x08location\x1a\xce\x01\n\x08Location\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x16\n\x04span\x18\x02 \x03(\x05\x42\x02\x10\x01R\x04span\x12)\n\x10leading_comments\x18\x03 \x01(\tR\x0fleadingComments\x12+\n\x11trailing_comments\x18\x04 \x01(\tR\x10trailingComments\x12:\n\x19leading_detached_comments\x18\x06 \x03(\tR\x17leadingDetachedComments\"\xd0\x02\n\x11GeneratedCodeInfo\x12M\n\nannotation\x18\x01 \x03(\x0b\x32-.google.protobuf.GeneratedCodeInfo.AnnotationR\nannotation\x1a\xeb\x01\n\nAnnotation\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x1f\n\x0bsource_file\x18\x02 \x01(\tR\nsourceFile\x12\x14\n\x05\x62\x65gin\x18\x03 \x01(\x05R\x05\x62\x65gin\x12\x10\n\x03\x65nd\x18\x04 \x01(\x05R\x03\x65nd\x12R\n\x08semantic\x18\x05 \x01(\x0e\x32\x36.google.protobuf.GeneratedCodeInfo.Annotation.SemanticR\x08semantic\"(\n\x08Semantic\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SET\x10\x01\x12\t\n\x05\x41LIAS\x10\x02*\xa7\x02\n\x07\x45\x64ition\x12\x13\n\x0f\x45\x44ITION_UNKNOWN\x10\x00\x12\x13\n\x0e\x45\x44ITION_LEGACY\x10\x84\x07\x12\x13\n\x0e\x45\x44ITION_PROTO2\x10\xe6\x07\x12\x13\n\x0e\x45\x44ITION_PROTO3\x10\xe7\x07\x12\x11\n\x0c\x45\x44ITION_2023\x10\xe8\x07\x12\x11\n\x0c\x45\x44ITION_2024\x10\xe9\x07\x12\x17\n\x13\x45\x44ITION_1_TEST_ONLY\x10\x01\x12\x17\n\x13\x45\x44ITION_2_TEST_ONLY\x10\x02\x12\x1d\n\x17\x45\x44ITION_99997_TEST_ONLY\x10\x9d\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99998_TEST_ONLY\x10\x9e\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99999_TEST_ONLY\x10\x9f\x8d\x06\x12\x13\n\x0b\x45\x44ITION_MAX\x10\xff\xff\xff\xff\x07\x42~\n\x13\x63om.google.protobufB\x10\x44\x65scriptorProtosH\x01Z-google.golang.org/protobuf/types/descriptorpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1aGoogle.Protobuf.Reflection'
   )
 else:
-  DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n google/protobuf/descriptor.proto\x12\x0fgoogle.protobuf\"M\n\x11\x46ileDescriptorSet\x12\x38\n\x04\x66ile\x18\x01 \x03(\x0b\x32$.google.protobuf.FileDescriptorProtoR\x04\x66ile\"\x98\x05\n\x13\x46ileDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07package\x18\x02 \x01(\tR\x07package\x12\x1e\n\ndependency\x18\x03 \x03(\tR\ndependency\x12+\n\x11public_dependency\x18\n \x03(\x05R\x10publicDependency\x12\'\n\x0fweak_dependency\x18\x0b \x03(\x05R\x0eweakDependency\x12\x43\n\x0cmessage_type\x18\x04 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\x0bmessageType\x12\x41\n\tenum_type\x18\x05 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12\x41\n\x07service\x18\x06 \x03(\x0b\x32\'.google.protobuf.ServiceDescriptorProtoR\x07service\x12\x43\n\textension\x18\x07 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x36\n\x07options\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.FileOptionsR\x07options\x12I\n\x10source_code_info\x18\t \x01(\x0b\x32\x1f.google.protobuf.SourceCodeInfoR\x0esourceCodeInfo\x12\x16\n\x06syntax\x18\x0c \x01(\tR\x06syntax\x12\x32\n\x07\x65\x64ition\x18\x0e \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\"\xb9\x06\n\x0f\x44\x65scriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\x05\x66ield\x18\x02 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\x05\x66ield\x12\x43\n\textension\x18\x06 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x41\n\x0bnested_type\x18\x03 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\nnestedType\x12\x41\n\tenum_type\x18\x04 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12X\n\x0f\x65xtension_range\x18\x05 \x03(\x0b\x32/.google.protobuf.DescriptorProto.ExtensionRangeR\x0e\x65xtensionRange\x12\x44\n\noneof_decl\x18\x08 \x03(\x0b\x32%.google.protobuf.OneofDescriptorProtoR\toneofDecl\x12\x39\n\x07options\x18\x07 \x01(\x0b\x32\x1f.google.protobuf.MessageOptionsR\x07options\x12U\n\x0ereserved_range\x18\t \x03(\x0b\x32..google.protobuf.DescriptorProto.ReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\n \x03(\tR\x0creservedName\x1az\n\x0e\x45xtensionRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x12@\n\x07options\x18\x03 \x01(\x0b\x32&.google.protobuf.ExtensionRangeOptionsR\x07options\x1a\x37\n\rReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\xcc\x04\n\x15\x45xtensionRangeOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x12Y\n\x0b\x64\x65\x63laration\x18\x02 \x03(\x0b\x32\x32.google.protobuf.ExtensionRangeOptions.DeclarationB\x03\x88\x01\x02R\x0b\x64\x65\x63laration\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12m\n\x0cverification\x18\x03 \x01(\x0e\x32\x38.google.protobuf.ExtensionRangeOptions.VerificationState:\nUNVERIFIEDB\x03\x88\x01\x02R\x0cverification\x1a\x94\x01\n\x0b\x44\x65\x63laration\x12\x16\n\x06number\x18\x01 \x01(\x05R\x06number\x12\x1b\n\tfull_name\x18\x02 \x01(\tR\x08\x66ullName\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x12\x1a\n\x08reserved\x18\x05 \x01(\x08R\x08reserved\x12\x1a\n\x08repeated\x18\x06 \x01(\x08R\x08repeatedJ\x04\x08\x04\x10\x05\"4\n\x11VerificationState\x12\x0f\n\x0b\x44\x45\x43LARATION\x10\x00\x12\x0e\n\nUNVERIFIED\x10\x01*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xc1\x06\n\x14\x46ieldDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x41\n\x05label\x18\x04 \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.LabelR\x05label\x12>\n\x04type\x18\x05 \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.TypeR\x04type\x12\x1b\n\ttype_name\x18\x06 \x01(\tR\x08typeName\x12\x1a\n\x08\x65xtendee\x18\x02 \x01(\tR\x08\x65xtendee\x12#\n\rdefault_value\x18\x07 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1f\n\x0boneof_index\x18\t \x01(\x05R\noneofIndex\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12\x37\n\x07options\x18\x08 \x01(\x0b\x32\x1d.google.protobuf.FieldOptionsR\x07options\x12\'\n\x0fproto3_optional\x18\x11 \x01(\x08R\x0eproto3Optional\"\xb6\x02\n\x04Type\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"C\n\x05Label\x12\x12\n\x0eLABEL_OPTIONAL\x10\x01\x12\x12\n\x0eLABEL_REPEATED\x10\x03\x12\x12\n\x0eLABEL_REQUIRED\x10\x02\"c\n\x14OneofDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x37\n\x07options\x18\x02 \x01(\x0b\x32\x1d.google.protobuf.OneofOptionsR\x07options\"\xe3\x02\n\x13\x45numDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x05value\x18\x02 \x03(\x0b\x32).google.protobuf.EnumValueDescriptorProtoR\x05value\x12\x36\n\x07options\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.EnumOptionsR\x07options\x12]\n\x0ereserved_range\x18\x04 \x03(\x0b\x32\x36.google.protobuf.EnumDescriptorProto.EnumReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\x05 \x03(\tR\x0creservedName\x1a;\n\x11\x45numReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\x83\x01\n\x18\x45numValueDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12;\n\x07options\x18\x03 \x01(\x0b\x32!.google.protobuf.EnumValueOptionsR\x07options\"\xa7\x01\n\x16ServiceDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x06method\x18\x02 \x03(\x0b\x32&.google.protobuf.MethodDescriptorProtoR\x06method\x12\x39\n\x07options\x18\x03 \x01(\x0b\x32\x1f.google.protobuf.ServiceOptionsR\x07options\"\x89\x02\n\x15MethodDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ninput_type\x18\x02 \x01(\tR\tinputType\x12\x1f\n\x0boutput_type\x18\x03 \x01(\tR\noutputType\x12\x38\n\x07options\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.MethodOptionsR\x07options\x12\x30\n\x10\x63lient_streaming\x18\x05 \x01(\x08:\x05\x66\x61lseR\x0f\x63lientStreaming\x12\x30\n\x10server_streaming\x18\x06 \x01(\x08:\x05\x66\x61lseR\x0fserverStreaming\"\x97\t\n\x0b\x46ileOptions\x12!\n\x0cjava_package\x18\x01 \x01(\tR\x0bjavaPackage\x12\x30\n\x14java_outer_classname\x18\x08 \x01(\tR\x12javaOuterClassname\x12\x35\n\x13java_multiple_files\x18\n \x01(\x08:\x05\x66\x61lseR\x11javaMultipleFiles\x12\x44\n\x1djava_generate_equals_and_hash\x18\x14 \x01(\x08\x42\x02\x18\x01R\x19javaGenerateEqualsAndHash\x12:\n\x16java_string_check_utf8\x18\x1b \x01(\x08:\x05\x66\x61lseR\x13javaStringCheckUtf8\x12S\n\x0coptimize_for\x18\t \x01(\x0e\x32).google.protobuf.FileOptions.OptimizeMode:\x05SPEEDR\x0boptimizeFor\x12\x1d\n\ngo_package\x18\x0b \x01(\tR\tgoPackage\x12\x35\n\x13\x63\x63_generic_services\x18\x10 \x01(\x08:\x05\x66\x61lseR\x11\x63\x63GenericServices\x12\x39\n\x15java_generic_services\x18\x11 \x01(\x08:\x05\x66\x61lseR\x13javaGenericServices\x12\x35\n\x13py_generic_services\x18\x12 \x01(\x08:\x05\x66\x61lseR\x11pyGenericServices\x12%\n\ndeprecated\x18\x17 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12.\n\x10\x63\x63_enable_arenas\x18\x1f \x01(\x08:\x04trueR\x0e\x63\x63\x45nableArenas\x12*\n\x11objc_class_prefix\x18$ \x01(\tR\x0fobjcClassPrefix\x12)\n\x10\x63sharp_namespace\x18% \x01(\tR\x0f\x63sharpNamespace\x12!\n\x0cswift_prefix\x18\' \x01(\tR\x0bswiftPrefix\x12(\n\x10php_class_prefix\x18( \x01(\tR\x0ephpClassPrefix\x12#\n\rphp_namespace\x18) \x01(\tR\x0cphpNamespace\x12\x34\n\x16php_metadata_namespace\x18, \x01(\tR\x14phpMetadataNamespace\x12!\n\x0cruby_package\x18- \x01(\tR\x0brubyPackage\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\":\n\x0cOptimizeMode\x12\t\n\x05SPEED\x10\x01\x12\r\n\tCODE_SIZE\x10\x02\x12\x10\n\x0cLITE_RUNTIME\x10\x03*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08*\x10+J\x04\x08&\x10\'\"\xf4\x03\n\x0eMessageOptions\x12<\n\x17message_set_wire_format\x18\x01 \x01(\x08:\x05\x66\x61lseR\x14messageSetWireFormat\x12L\n\x1fno_standard_descriptor_accessor\x18\x02 \x01(\x08:\x05\x66\x61lseR\x1cnoStandardDescriptorAccessor\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x1b\n\tmap_entry\x18\x07 \x01(\x08R\x08mapEntry\x12V\n&deprecated_legacy_json_field_conflicts\x18\x0b \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\x9d\r\n\x0c\x46ieldOptions\x12\x41\n\x05\x63type\x18\x01 \x01(\x0e\x32#.google.protobuf.FieldOptions.CType:\x06STRINGR\x05\x63type\x12\x16\n\x06packed\x18\x02 \x01(\x08R\x06packed\x12G\n\x06jstype\x18\x06 \x01(\x0e\x32$.google.protobuf.FieldOptions.JSType:\tJS_NORMALR\x06jstype\x12\x19\n\x04lazy\x18\x05 \x01(\x08:\x05\x66\x61lseR\x04lazy\x12.\n\x0funverified_lazy\x18\x0f \x01(\x08:\x05\x66\x61lseR\x0eunverifiedLazy\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x19\n\x04weak\x18\n \x01(\x08:\x05\x66\x61lseR\x04weak\x12(\n\x0c\x64\x65\x62ug_redact\x18\x10 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12K\n\tretention\x18\x11 \x01(\x0e\x32-.google.protobuf.FieldOptions.OptionRetentionR\tretention\x12H\n\x07targets\x18\x13 \x03(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeR\x07targets\x12W\n\x10\x65\x64ition_defaults\x18\x14 \x03(\x0b\x32,.google.protobuf.FieldOptions.EditionDefaultR\x0f\x65\x64itionDefaults\x12\x37\n\x08\x66\x65\x61tures\x18\x15 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12U\n\x0f\x66\x65\x61ture_support\x18\x16 \x01(\x0b\x32,.google.protobuf.FieldOptions.FeatureSupportR\x0e\x66\x65\x61tureSupport\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x1aZ\n\x0e\x45\x64itionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\x1a\x96\x02\n\x0e\x46\x65\x61tureSupport\x12G\n\x12\x65\x64ition_introduced\x18\x01 \x01(\x0e\x32\x18.google.protobuf.EditionR\x11\x65\x64itionIntroduced\x12G\n\x12\x65\x64ition_deprecated\x18\x02 \x01(\x0e\x32\x18.google.protobuf.EditionR\x11\x65\x64itionDeprecated\x12/\n\x13\x64\x65precation_warning\x18\x03 \x01(\tR\x12\x64\x65precationWarning\x12\x41\n\x0f\x65\x64ition_removed\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0e\x65\x64itionRemoved\"/\n\x05\x43Type\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x43ORD\x10\x01\x12\x10\n\x0cSTRING_PIECE\x10\x02\"5\n\x06JSType\x12\r\n\tJS_NORMAL\x10\x00\x12\r\n\tJS_STRING\x10\x01\x12\r\n\tJS_NUMBER\x10\x02\"U\n\x0fOptionRetention\x12\x15\n\x11RETENTION_UNKNOWN\x10\x00\x12\x15\n\x11RETENTION_RUNTIME\x10\x01\x12\x14\n\x10RETENTION_SOURCE\x10\x02\"\x8c\x02\n\x10OptionTargetType\x12\x17\n\x13TARGET_TYPE_UNKNOWN\x10\x00\x12\x14\n\x10TARGET_TYPE_FILE\x10\x01\x12\x1f\n\x1bTARGET_TYPE_EXTENSION_RANGE\x10\x02\x12\x17\n\x13TARGET_TYPE_MESSAGE\x10\x03\x12\x15\n\x11TARGET_TYPE_FIELD\x10\x04\x12\x15\n\x11TARGET_TYPE_ONEOF\x10\x05\x12\x14\n\x10TARGET_TYPE_ENUM\x10\x06\x12\x1a\n\x16TARGET_TYPE_ENUM_ENTRY\x10\x07\x12\x17\n\x13TARGET_TYPE_SERVICE\x10\x08\x12\x16\n\x12TARGET_TYPE_METHOD\x10\t*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x12\x10\x13\"\xac\x01\n\x0cOneofOptions\x12\x37\n\x08\x66\x65\x61tures\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd1\x02\n\x0b\x45numOptions\x12\x1f\n\x0b\x61llow_alias\x18\x02 \x01(\x08R\nallowAlias\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12V\n&deprecated_legacy_json_field_conflicts\x18\x06 \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x05\x10\x06\"\x81\x02\n\x10\x45numValueOptions\x12%\n\ndeprecated\x18\x01 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x37\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12(\n\x0c\x64\x65\x62ug_redact\x18\x03 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd5\x01\n\x0eServiceOptions\x12\x37\n\x08\x66\x65\x61tures\x18\" \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x99\x03\n\rMethodOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12q\n\x11idempotency_level\x18\" \x01(\x0e\x32/.google.protobuf.MethodOptions.IdempotencyLevel:\x13IDEMPOTENCY_UNKNOWNR\x10idempotencyLevel\x12\x37\n\x08\x66\x65\x61tures\x18# \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"P\n\x10IdempotencyLevel\x12\x17\n\x13IDEMPOTENCY_UNKNOWN\x10\x00\x12\x13\n\x0fNO_SIDE_EFFECTS\x10\x01\x12\x0e\n\nIDEMPOTENT\x10\x02*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9a\x03\n\x13UninterpretedOption\x12\x41\n\x04name\x18\x02 \x03(\x0b\x32-.google.protobuf.UninterpretedOption.NamePartR\x04name\x12)\n\x10identifier_value\x18\x03 \x01(\tR\x0fidentifierValue\x12,\n\x12positive_int_value\x18\x04 \x01(\x04R\x10positiveIntValue\x12,\n\x12negative_int_value\x18\x05 \x01(\x03R\x10negativeIntValue\x12!\n\x0c\x64ouble_value\x18\x06 \x01(\x01R\x0b\x64oubleValue\x12!\n\x0cstring_value\x18\x07 \x01(\x0cR\x0bstringValue\x12\'\n\x0f\x61ggregate_value\x18\x08 \x01(\tR\x0e\x61ggregateValue\x1aJ\n\x08NamePart\x12\x1b\n\tname_part\x18\x01 \x02(\tR\x08namePart\x12!\n\x0cis_extension\x18\x02 \x02(\x08R\x0bisExtension\"\xb9\n\n\nFeatureSet\x12\x91\x01\n\x0e\x66ield_presence\x18\x01 \x01(\x0e\x32).google.protobuf.FeatureSet.FieldPresenceB?\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe6\x07\xa2\x01\r\x12\x08IMPLICIT\x18\xe7\x07\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe8\x07\xb2\x01\x03\x08\xe8\x07R\rfieldPresence\x12l\n\tenum_type\x18\x02 \x01(\x0e\x32$.google.protobuf.FeatureSet.EnumTypeB)\x88\x01\x01\x98\x01\x06\x98\x01\x01\xa2\x01\x0b\x12\x06\x43LOSED\x18\xe6\x07\xa2\x01\t\x12\x04OPEN\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x08\x65numType\x12\x98\x01\n\x17repeated_field_encoding\x18\x03 \x01(\x0e\x32\x31.google.protobuf.FeatureSet.RepeatedFieldEncodingB-\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPANDED\x18\xe6\x07\xa2\x01\x0b\x12\x06PACKED\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x15repeatedFieldEncoding\x12~\n\x0futf8_validation\x18\x04 \x01(\x0e\x32*.google.protobuf.FeatureSet.Utf8ValidationB)\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\t\x12\x04NONE\x18\xe6\x07\xa2\x01\x0b\x12\x06VERIFY\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x0eutf8Validation\x12~\n\x10message_encoding\x18\x05 \x01(\x0e\x32+.google.protobuf.FeatureSet.MessageEncodingB&\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\x14\x12\x0fLENGTH_PREFIXED\x18\xe6\x07\xb2\x01\x03\x08\xe8\x07R\x0fmessageEncoding\x12\x82\x01\n\x0bjson_format\x18\x06 \x01(\x0e\x32&.google.protobuf.FeatureSet.JsonFormatB9\x88\x01\x01\x98\x01\x03\x98\x01\x06\x98\x01\x01\xa2\x01\x17\x12\x12LEGACY_BEST_EFFORT\x18\xe6\x07\xa2\x01\n\x12\x05\x41LLOW\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\njsonFormat\"\\\n\rFieldPresence\x12\x1a\n\x16\x46IELD_PRESENCE_UNKNOWN\x10\x00\x12\x0c\n\x08\x45XPLICIT\x10\x01\x12\x0c\n\x08IMPLICIT\x10\x02\x12\x13\n\x0fLEGACY_REQUIRED\x10\x03\"7\n\x08\x45numType\x12\x15\n\x11\x45NUM_TYPE_UNKNOWN\x10\x00\x12\x08\n\x04OPEN\x10\x01\x12\n\n\x06\x43LOSED\x10\x02\"V\n\x15RepeatedFieldEncoding\x12#\n\x1fREPEATED_FIELD_ENCODING_UNKNOWN\x10\x00\x12\n\n\x06PACKED\x10\x01\x12\x0c\n\x08\x45XPANDED\x10\x02\"C\n\x0eUtf8Validation\x12\x1b\n\x17UTF8_VALIDATION_UNKNOWN\x10\x00\x12\n\n\x06VERIFY\x10\x02\x12\x08\n\x04NONE\x10\x03\"S\n\x0fMessageEncoding\x12\x1c\n\x18MESSAGE_ENCODING_UNKNOWN\x10\x00\x12\x13\n\x0fLENGTH_PREFIXED\x10\x01\x12\r\n\tDELIMITED\x10\x02\"H\n\nJsonFormat\x12\x17\n\x13JSON_FORMAT_UNKNOWN\x10\x00\x12\t\n\x05\x41LLOW\x10\x01\x12\x16\n\x12LEGACY_BEST_EFFORT\x10\x02*\x06\x08\xe8\x07\x10\xe9\x07*\x06\x08\xe9\x07\x10\xea\x07*\x06\x08\xea\x07\x10\xeb\x07*\x06\x08\x86N\x10\x87N*\x06\x08\x8bN\x10\x90N*\x06\x08\x90N\x10\x91NJ\x06\x08\xe7\x07\x10\xe8\x07\"\xd9\x03\n\x12\x46\x65\x61tureSetDefaults\x12X\n\x08\x64\x65\x66\x61ults\x18\x01 \x03(\x0b\x32<.google.protobuf.FeatureSetDefaults.FeatureSetEditionDefaultR\x08\x64\x65\x66\x61ults\x12\x41\n\x0fminimum_edition\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0eminimumEdition\x12\x41\n\x0fmaximum_edition\x18\x05 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0emaximumEdition\x1a\xe2\x01\n\x18\x46\x65\x61tureSetEditionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12N\n\x14overridable_features\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x13overridableFeatures\x12\x42\n\x0e\x66ixed_features\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\rfixedFeatures\"\xa7\x02\n\x0eSourceCodeInfo\x12\x44\n\x08location\x18\x01 \x03(\x0b\x32(.google.protobuf.SourceCodeInfo.LocationR\x08location\x1a\xce\x01\n\x08Location\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x16\n\x04span\x18\x02 \x03(\x05\x42\x02\x10\x01R\x04span\x12)\n\x10leading_comments\x18\x03 \x01(\tR\x0fleadingComments\x12+\n\x11trailing_comments\x18\x04 \x01(\tR\x10trailingComments\x12:\n\x19leading_detached_comments\x18\x06 \x03(\tR\x17leadingDetachedComments\"\xd0\x02\n\x11GeneratedCodeInfo\x12M\n\nannotation\x18\x01 \x03(\x0b\x32-.google.protobuf.GeneratedCodeInfo.AnnotationR\nannotation\x1a\xeb\x01\n\nAnnotation\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x1f\n\x0bsource_file\x18\x02 \x01(\tR\nsourceFile\x12\x14\n\x05\x62\x65gin\x18\x03 \x01(\x05R\x05\x62\x65gin\x12\x10\n\x03\x65nd\x18\x04 \x01(\x05R\x03\x65nd\x12R\n\x08semantic\x18\x05 \x01(\x0e\x32\x36.google.protobuf.GeneratedCodeInfo.Annotation.SemanticR\x08semantic\"(\n\x08Semantic\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SET\x10\x01\x12\t\n\x05\x41LIAS\x10\x02*\xa7\x02\n\x07\x45\x64ition\x12\x13\n\x0f\x45\x44ITION_UNKNOWN\x10\x00\x12\x13\n\x0e\x45\x44ITION_LEGACY\x10\x84\x07\x12\x13\n\x0e\x45\x44ITION_PROTO2\x10\xe6\x07\x12\x13\n\x0e\x45\x44ITION_PROTO3\x10\xe7\x07\x12\x11\n\x0c\x45\x44ITION_2023\x10\xe8\x07\x12\x11\n\x0c\x45\x44ITION_2024\x10\xe9\x07\x12\x17\n\x13\x45\x44ITION_1_TEST_ONLY\x10\x01\x12\x17\n\x13\x45\x44ITION_2_TEST_ONLY\x10\x02\x12\x1d\n\x17\x45\x44ITION_99997_TEST_ONLY\x10\x9d\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99998_TEST_ONLY\x10\x9e\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99999_TEST_ONLY\x10\x9f\x8d\x06\x12\x13\n\x0b\x45\x44ITION_MAX\x10\xff\xff\xff\xff\x07\x42~\n\x13\x63om.google.protobufB\x10\x44\x65scriptorProtosH\x01Z-google.golang.org/protobuf/types/descriptorpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1aGoogle.Protobuf.Reflection')
+  DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n google/protobuf/descriptor.proto\x12\x0fgoogle.protobuf\"M\n\x11\x46ileDescriptorSet\x12\x38\n\x04\x66ile\x18\x01 \x03(\x0b\x32$.google.protobuf.FileDescriptorProtoR\x04\x66ile\"\x98\x05\n\x13\x46ileDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07package\x18\x02 \x01(\tR\x07package\x12\x1e\n\ndependency\x18\x03 \x03(\tR\ndependency\x12+\n\x11public_dependency\x18\n \x03(\x05R\x10publicDependency\x12\'\n\x0fweak_dependency\x18\x0b \x03(\x05R\x0eweakDependency\x12\x43\n\x0cmessage_type\x18\x04 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\x0bmessageType\x12\x41\n\tenum_type\x18\x05 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12\x41\n\x07service\x18\x06 \x03(\x0b\x32\'.google.protobuf.ServiceDescriptorProtoR\x07service\x12\x43\n\textension\x18\x07 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x36\n\x07options\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.FileOptionsR\x07options\x12I\n\x10source_code_info\x18\t \x01(\x0b\x32\x1f.google.protobuf.SourceCodeInfoR\x0esourceCodeInfo\x12\x16\n\x06syntax\x18\x0c \x01(\tR\x06syntax\x12\x32\n\x07\x65\x64ition\x18\x0e \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\"\xb9\x06\n\x0f\x44\x65scriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\x05\x66ield\x18\x02 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\x05\x66ield\x12\x43\n\textension\x18\x06 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x41\n\x0bnested_type\x18\x03 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\nnestedType\x12\x41\n\tenum_type\x18\x04 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12X\n\x0f\x65xtension_range\x18\x05 \x03(\x0b\x32/.google.protobuf.DescriptorProto.ExtensionRangeR\x0e\x65xtensionRange\x12\x44\n\noneof_decl\x18\x08 \x03(\x0b\x32%.google.protobuf.OneofDescriptorProtoR\toneofDecl\x12\x39\n\x07options\x18\x07 \x01(\x0b\x32\x1f.google.protobuf.MessageOptionsR\x07options\x12U\n\x0ereserved_range\x18\t \x03(\x0b\x32..google.protobuf.DescriptorProto.ReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\n \x03(\tR\x0creservedName\x1az\n\x0e\x45xtensionRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x12@\n\x07options\x18\x03 \x01(\x0b\x32&.google.protobuf.ExtensionRangeOptionsR\x07options\x1a\x37\n\rReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\xcc\x04\n\x15\x45xtensionRangeOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x12Y\n\x0b\x64\x65\x63laration\x18\x02 \x03(\x0b\x32\x32.google.protobuf.ExtensionRangeOptions.DeclarationB\x03\x88\x01\x02R\x0b\x64\x65\x63laration\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12m\n\x0cverification\x18\x03 \x01(\x0e\x32\x38.google.protobuf.ExtensionRangeOptions.VerificationState:\nUNVERIFIEDB\x03\x88\x01\x02R\x0cverification\x1a\x94\x01\n\x0b\x44\x65\x63laration\x12\x16\n\x06number\x18\x01 \x01(\x05R\x06number\x12\x1b\n\tfull_name\x18\x02 \x01(\tR\x08\x66ullName\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x12\x1a\n\x08reserved\x18\x05 \x01(\x08R\x08reserved\x12\x1a\n\x08repeated\x18\x06 \x01(\x08R\x08repeatedJ\x04\x08\x04\x10\x05\"4\n\x11VerificationState\x12\x0f\n\x0b\x44\x45\x43LARATION\x10\x00\x12\x0e\n\nUNVERIFIED\x10\x01*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xc1\x06\n\x14\x46ieldDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x41\n\x05label\x18\x04 \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.LabelR\x05label\x12>\n\x04type\x18\x05 \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.TypeR\x04type\x12\x1b\n\ttype_name\x18\x06 \x01(\tR\x08typeName\x12\x1a\n\x08\x65xtendee\x18\x02 \x01(\tR\x08\x65xtendee\x12#\n\rdefault_value\x18\x07 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1f\n\x0boneof_index\x18\t \x01(\x05R\noneofIndex\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12\x37\n\x07options\x18\x08 \x01(\x0b\x32\x1d.google.protobuf.FieldOptionsR\x07options\x12\'\n\x0fproto3_optional\x18\x11 \x01(\x08R\x0eproto3Optional\"\xb6\x02\n\x04Type\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"C\n\x05Label\x12\x12\n\x0eLABEL_OPTIONAL\x10\x01\x12\x12\n\x0eLABEL_REPEATED\x10\x03\x12\x12\n\x0eLABEL_REQUIRED\x10\x02\"c\n\x14OneofDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x37\n\x07options\x18\x02 \x01(\x0b\x32\x1d.google.protobuf.OneofOptionsR\x07options\"\xe3\x02\n\x13\x45numDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x05value\x18\x02 \x03(\x0b\x32).google.protobuf.EnumValueDescriptorProtoR\x05value\x12\x36\n\x07options\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.EnumOptionsR\x07options\x12]\n\x0ereserved_range\x18\x04 \x03(\x0b\x32\x36.google.protobuf.EnumDescriptorProto.EnumReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\x05 \x03(\tR\x0creservedName\x1a;\n\x11\x45numReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\x83\x01\n\x18\x45numValueDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12;\n\x07options\x18\x03 \x01(\x0b\x32!.google.protobuf.EnumValueOptionsR\x07options\"\xa7\x01\n\x16ServiceDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x06method\x18\x02 \x03(\x0b\x32&.google.protobuf.MethodDescriptorProtoR\x06method\x12\x39\n\x07options\x18\x03 \x01(\x0b\x32\x1f.google.protobuf.ServiceOptionsR\x07options\"\x89\x02\n\x15MethodDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ninput_type\x18\x02 \x01(\tR\tinputType\x12\x1f\n\x0boutput_type\x18\x03 \x01(\tR\noutputType\x12\x38\n\x07options\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.MethodOptionsR\x07options\x12\x30\n\x10\x63lient_streaming\x18\x05 \x01(\x08:\x05\x66\x61lseR\x0f\x63lientStreaming\x12\x30\n\x10server_streaming\x18\x06 \x01(\x08:\x05\x66\x61lseR\x0fserverStreaming\"\x97\t\n\x0b\x46ileOptions\x12!\n\x0cjava_package\x18\x01 \x01(\tR\x0bjavaPackage\x12\x30\n\x14java_outer_classname\x18\x08 \x01(\tR\x12javaOuterClassname\x12\x35\n\x13java_multiple_files\x18\n \x01(\x08:\x05\x66\x61lseR\x11javaMultipleFiles\x12\x44\n\x1djava_generate_equals_and_hash\x18\x14 \x01(\x08\x42\x02\x18\x01R\x19javaGenerateEqualsAndHash\x12:\n\x16java_string_check_utf8\x18\x1b \x01(\x08:\x05\x66\x61lseR\x13javaStringCheckUtf8\x12S\n\x0coptimize_for\x18\t \x01(\x0e\x32).google.protobuf.FileOptions.OptimizeMode:\x05SPEEDR\x0boptimizeFor\x12\x1d\n\ngo_package\x18\x0b \x01(\tR\tgoPackage\x12\x35\n\x13\x63\x63_generic_services\x18\x10 \x01(\x08:\x05\x66\x61lseR\x11\x63\x63GenericServices\x12\x39\n\x15java_generic_services\x18\x11 \x01(\x08:\x05\x66\x61lseR\x13javaGenericServices\x12\x35\n\x13py_generic_services\x18\x12 \x01(\x08:\x05\x66\x61lseR\x11pyGenericServices\x12%\n\ndeprecated\x18\x17 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12.\n\x10\x63\x63_enable_arenas\x18\x1f \x01(\x08:\x04trueR\x0e\x63\x63\x45nableArenas\x12*\n\x11objc_class_prefix\x18$ \x01(\tR\x0fobjcClassPrefix\x12)\n\x10\x63sharp_namespace\x18% \x01(\tR\x0f\x63sharpNamespace\x12!\n\x0cswift_prefix\x18\' \x01(\tR\x0bswiftPrefix\x12(\n\x10php_class_prefix\x18( \x01(\tR\x0ephpClassPrefix\x12#\n\rphp_namespace\x18) \x01(\tR\x0cphpNamespace\x12\x34\n\x16php_metadata_namespace\x18, \x01(\tR\x14phpMetadataNamespace\x12!\n\x0cruby_package\x18- \x01(\tR\x0brubyPackage\x12\x37\n\x08\x66\x65\x61tures\x18\x32 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\":\n\x0cOptimizeMode\x12\t\n\x05SPEED\x10\x01\x12\r\n\tCODE_SIZE\x10\x02\x12\x10\n\x0cLITE_RUNTIME\x10\x03*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08*\x10+J\x04\x08&\x10\'\"\xf4\x03\n\x0eMessageOptions\x12<\n\x17message_set_wire_format\x18\x01 \x01(\x08:\x05\x66\x61lseR\x14messageSetWireFormat\x12L\n\x1fno_standard_descriptor_accessor\x18\x02 \x01(\x08:\x05\x66\x61lseR\x1cnoStandardDescriptorAccessor\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x1b\n\tmap_entry\x18\x07 \x01(\x08R\x08mapEntry\x12V\n&deprecated_legacy_json_field_conflicts\x18\x0b \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\x9d\r\n\x0c\x46ieldOptions\x12\x41\n\x05\x63type\x18\x01 \x01(\x0e\x32#.google.protobuf.FieldOptions.CType:\x06STRINGR\x05\x63type\x12\x16\n\x06packed\x18\x02 \x01(\x08R\x06packed\x12G\n\x06jstype\x18\x06 \x01(\x0e\x32$.google.protobuf.FieldOptions.JSType:\tJS_NORMALR\x06jstype\x12\x19\n\x04lazy\x18\x05 \x01(\x08:\x05\x66\x61lseR\x04lazy\x12.\n\x0funverified_lazy\x18\x0f \x01(\x08:\x05\x66\x61lseR\x0eunverifiedLazy\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x19\n\x04weak\x18\n \x01(\x08:\x05\x66\x61lseR\x04weak\x12(\n\x0c\x64\x65\x62ug_redact\x18\x10 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12K\n\tretention\x18\x11 \x01(\x0e\x32-.google.protobuf.FieldOptions.OptionRetentionR\tretention\x12H\n\x07targets\x18\x13 \x03(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeR\x07targets\x12W\n\x10\x65\x64ition_defaults\x18\x14 \x03(\x0b\x32,.google.protobuf.FieldOptions.EditionDefaultR\x0f\x65\x64itionDefaults\x12\x37\n\x08\x66\x65\x61tures\x18\x15 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12U\n\x0f\x66\x65\x61ture_support\x18\x16 \x01(\x0b\x32,.google.protobuf.FieldOptions.FeatureSupportR\x0e\x66\x65\x61tureSupport\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x1aZ\n\x0e\x45\x64itionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\x1a\x96\x02\n\x0e\x46\x65\x61tureSupport\x12G\n\x12\x65\x64ition_introduced\x18\x01 \x01(\x0e\x32\x18.google.protobuf.EditionR\x11\x65\x64itionIntroduced\x12G\n\x12\x65\x64ition_deprecated\x18\x02 \x01(\x0e\x32\x18.google.protobuf.EditionR\x11\x65\x64itionDeprecated\x12/\n\x13\x64\x65precation_warning\x18\x03 \x01(\tR\x12\x64\x65precationWarning\x12\x41\n\x0f\x65\x64ition_removed\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0e\x65\x64itionRemoved\"/\n\x05\x43Type\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x43ORD\x10\x01\x12\x10\n\x0cSTRING_PIECE\x10\x02\"5\n\x06JSType\x12\r\n\tJS_NORMAL\x10\x00\x12\r\n\tJS_STRING\x10\x01\x12\r\n\tJS_NUMBER\x10\x02\"U\n\x0fOptionRetention\x12\x15\n\x11RETENTION_UNKNOWN\x10\x00\x12\x15\n\x11RETENTION_RUNTIME\x10\x01\x12\x14\n\x10RETENTION_SOURCE\x10\x02\"\x8c\x02\n\x10OptionTargetType\x12\x17\n\x13TARGET_TYPE_UNKNOWN\x10\x00\x12\x14\n\x10TARGET_TYPE_FILE\x10\x01\x12\x1f\n\x1bTARGET_TYPE_EXTENSION_RANGE\x10\x02\x12\x17\n\x13TARGET_TYPE_MESSAGE\x10\x03\x12\x15\n\x11TARGET_TYPE_FIELD\x10\x04\x12\x15\n\x11TARGET_TYPE_ONEOF\x10\x05\x12\x14\n\x10TARGET_TYPE_ENUM\x10\x06\x12\x1a\n\x16TARGET_TYPE_ENUM_ENTRY\x10\x07\x12\x17\n\x13TARGET_TYPE_SERVICE\x10\x08\x12\x16\n\x12TARGET_TYPE_METHOD\x10\t*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x12\x10\x13\"\xac\x01\n\x0cOneofOptions\x12\x37\n\x08\x66\x65\x61tures\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd1\x02\n\x0b\x45numOptions\x12\x1f\n\x0b\x61llow_alias\x18\x02 \x01(\x08R\nallowAlias\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12V\n&deprecated_legacy_json_field_conflicts\x18\x06 \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12\x37\n\x08\x66\x65\x61tures\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x05\x10\x06\"\x81\x02\n\x10\x45numValueOptions\x12%\n\ndeprecated\x18\x01 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x37\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12(\n\x0c\x64\x65\x62ug_redact\x18\x03 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xd5\x01\n\x0eServiceOptions\x12\x37\n\x08\x66\x65\x61tures\x18\" \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x99\x03\n\rMethodOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12q\n\x11idempotency_level\x18\" \x01(\x0e\x32/.google.protobuf.MethodOptions.IdempotencyLevel:\x13IDEMPOTENCY_UNKNOWNR\x10idempotencyLevel\x12\x37\n\x08\x66\x65\x61tures\x18# \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x08\x66\x65\x61tures\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"P\n\x10IdempotencyLevel\x12\x17\n\x13IDEMPOTENCY_UNKNOWN\x10\x00\x12\x13\n\x0fNO_SIDE_EFFECTS\x10\x01\x12\x0e\n\nIDEMPOTENT\x10\x02*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9a\x03\n\x13UninterpretedOption\x12\x41\n\x04name\x18\x02 \x03(\x0b\x32-.google.protobuf.UninterpretedOption.NamePartR\x04name\x12)\n\x10identifier_value\x18\x03 \x01(\tR\x0fidentifierValue\x12,\n\x12positive_int_value\x18\x04 \x01(\x04R\x10positiveIntValue\x12,\n\x12negative_int_value\x18\x05 \x01(\x03R\x10negativeIntValue\x12!\n\x0c\x64ouble_value\x18\x06 \x01(\x01R\x0b\x64oubleValue\x12!\n\x0cstring_value\x18\x07 \x01(\x0cR\x0bstringValue\x12\'\n\x0f\x61ggregate_value\x18\x08 \x01(\tR\x0e\x61ggregateValue\x1aJ\n\x08NamePart\x12\x1b\n\tname_part\x18\x01 \x02(\tR\x08namePart\x12!\n\x0cis_extension\x18\x02 \x02(\x08R\x0bisExtension\"\xa1\n\n\nFeatureSet\x12\x91\x01\n\x0e\x66ield_presence\x18\x01 \x01(\x0e\x32).google.protobuf.FeatureSet.FieldPresenceB?\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe6\x07\xa2\x01\r\x12\x08IMPLICIT\x18\xe7\x07\xa2\x01\r\x12\x08\x45XPLICIT\x18\xe8\x07\xb2\x01\x03\x08\xe8\x07R\rfieldPresence\x12l\n\tenum_type\x18\x02 \x01(\x0e\x32$.google.protobuf.FeatureSet.EnumTypeB)\x88\x01\x01\x98\x01\x06\x98\x01\x01\xa2\x01\x0b\x12\x06\x43LOSED\x18\xe6\x07\xa2\x01\t\x12\x04OPEN\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x08\x65numType\x12\x98\x01\n\x17repeated_field_encoding\x18\x03 \x01(\x0e\x32\x31.google.protobuf.FeatureSet.RepeatedFieldEncodingB-\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\r\x12\x08\x45XPANDED\x18\xe6\x07\xa2\x01\x0b\x12\x06PACKED\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x15repeatedFieldEncoding\x12~\n\x0futf8_validation\x18\x04 \x01(\x0e\x32*.google.protobuf.FeatureSet.Utf8ValidationB)\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\t\x12\x04NONE\x18\xe6\x07\xa2\x01\x0b\x12\x06VERIFY\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\x0eutf8Validation\x12~\n\x10message_encoding\x18\x05 \x01(\x0e\x32+.google.protobuf.FeatureSet.MessageEncodingB&\x88\x01\x01\x98\x01\x04\x98\x01\x01\xa2\x01\x14\x12\x0fLENGTH_PREFIXED\x18\xe6\x07\xb2\x01\x03\x08\xe8\x07R\x0fmessageEncoding\x12\x82\x01\n\x0bjson_format\x18\x06 \x01(\x0e\x32&.google.protobuf.FeatureSet.JsonFormatB9\x88\x01\x01\x98\x01\x03\x98\x01\x06\x98\x01\x01\xa2\x01\x17\x12\x12LEGACY_BEST_EFFORT\x18\xe6\x07\xa2\x01\n\x12\x05\x41LLOW\x18\xe7\x07\xb2\x01\x03\x08\xe8\x07R\njsonFormat\"\\\n\rFieldPresence\x12\x1a\n\x16\x46IELD_PRESENCE_UNKNOWN\x10\x00\x12\x0c\n\x08\x45XPLICIT\x10\x01\x12\x0c\n\x08IMPLICIT\x10\x02\x12\x13\n\x0fLEGACY_REQUIRED\x10\x03\"7\n\x08\x45numType\x12\x15\n\x11\x45NUM_TYPE_UNKNOWN\x10\x00\x12\x08\n\x04OPEN\x10\x01\x12\n\n\x06\x43LOSED\x10\x02\"V\n\x15RepeatedFieldEncoding\x12#\n\x1fREPEATED_FIELD_ENCODING_UNKNOWN\x10\x00\x12\n\n\x06PACKED\x10\x01\x12\x0c\n\x08\x45XPANDED\x10\x02\"C\n\x0eUtf8Validation\x12\x1b\n\x17UTF8_VALIDATION_UNKNOWN\x10\x00\x12\n\n\x06VERIFY\x10\x02\x12\x08\n\x04NONE\x10\x03\"S\n\x0fMessageEncoding\x12\x1c\n\x18MESSAGE_ENCODING_UNKNOWN\x10\x00\x12\x13\n\x0fLENGTH_PREFIXED\x10\x01\x12\r\n\tDELIMITED\x10\x02\"H\n\nJsonFormat\x12\x17\n\x13JSON_FORMAT_UNKNOWN\x10\x00\x12\t\n\x05\x41LLOW\x10\x01\x12\x16\n\x12LEGACY_BEST_EFFORT\x10\x02*\x06\x08\xe8\x07\x10\x8bN*\x06\x08\x8bN\x10\x90N*\x06\x08\x90N\x10\x91NJ\x06\x08\xe7\x07\x10\xe8\x07\"\xd9\x03\n\x12\x46\x65\x61tureSetDefaults\x12X\n\x08\x64\x65\x66\x61ults\x18\x01 \x03(\x0b\x32<.google.protobuf.FeatureSetDefaults.FeatureSetEditionDefaultR\x08\x64\x65\x66\x61ults\x12\x41\n\x0fminimum_edition\x18\x04 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0eminimumEdition\x12\x41\n\x0fmaximum_edition\x18\x05 \x01(\x0e\x32\x18.google.protobuf.EditionR\x0emaximumEdition\x1a\xe2\x01\n\x18\x46\x65\x61tureSetEditionDefault\x12\x32\n\x07\x65\x64ition\x18\x03 \x01(\x0e\x32\x18.google.protobuf.EditionR\x07\x65\x64ition\x12N\n\x14overridable_features\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\x13overridableFeatures\x12\x42\n\x0e\x66ixed_features\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.FeatureSetR\rfixedFeatures\"\xa7\x02\n\x0eSourceCodeInfo\x12\x44\n\x08location\x18\x01 \x03(\x0b\x32(.google.protobuf.SourceCodeInfo.LocationR\x08location\x1a\xce\x01\n\x08Location\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x16\n\x04span\x18\x02 \x03(\x05\x42\x02\x10\x01R\x04span\x12)\n\x10leading_comments\x18\x03 \x01(\tR\x0fleadingComments\x12+\n\x11trailing_comments\x18\x04 \x01(\tR\x10trailingComments\x12:\n\x19leading_detached_comments\x18\x06 \x03(\tR\x17leadingDetachedComments\"\xd0\x02\n\x11GeneratedCodeInfo\x12M\n\nannotation\x18\x01 \x03(\x0b\x32-.google.protobuf.GeneratedCodeInfo.AnnotationR\nannotation\x1a\xeb\x01\n\nAnnotation\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x1f\n\x0bsource_file\x18\x02 \x01(\tR\nsourceFile\x12\x14\n\x05\x62\x65gin\x18\x03 \x01(\x05R\x05\x62\x65gin\x12\x10\n\x03\x65nd\x18\x04 \x01(\x05R\x03\x65nd\x12R\n\x08semantic\x18\x05 \x01(\x0e\x32\x36.google.protobuf.GeneratedCodeInfo.Annotation.SemanticR\x08semantic\"(\n\x08Semantic\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SET\x10\x01\x12\t\n\x05\x41LIAS\x10\x02*\xa7\x02\n\x07\x45\x64ition\x12\x13\n\x0f\x45\x44ITION_UNKNOWN\x10\x00\x12\x13\n\x0e\x45\x44ITION_LEGACY\x10\x84\x07\x12\x13\n\x0e\x45\x44ITION_PROTO2\x10\xe6\x07\x12\x13\n\x0e\x45\x44ITION_PROTO3\x10\xe7\x07\x12\x11\n\x0c\x45\x44ITION_2023\x10\xe8\x07\x12\x11\n\x0c\x45\x44ITION_2024\x10\xe9\x07\x12\x17\n\x13\x45\x44ITION_1_TEST_ONLY\x10\x01\x12\x17\n\x13\x45\x44ITION_2_TEST_ONLY\x10\x02\x12\x1d\n\x17\x45\x44ITION_99997_TEST_ONLY\x10\x9d\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99998_TEST_ONLY\x10\x9e\x8d\x06\x12\x1d\n\x17\x45\x44ITION_99999_TEST_ONLY\x10\x9f\x8d\x06\x12\x13\n\x0b\x45\x44ITION_MAX\x10\xff\xff\xff\xff\x07\x42~\n\x13\x63om.google.protobufB\x10\x44\x65scriptorProtosH\x01Z-google.golang.org/protobuf/types/descriptorpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1aGoogle.Protobuf.Reflection')
 
 _globals = globals()
 if not _descriptor._USE_C_DESCRIPTORS:
   _EDITION = _descriptor.EnumDescriptor(
     name='Edition',
     full_name='google.protobuf.Edition',
     filename=None,
@@ -2320,15 +2320,15 @@
       _FEATURESET_REPEATEDFIELDENCODING,
       _FEATURESET_UTF8VALIDATION,
       _FEATURESET_MESSAGEENCODING,
       _FEATURESET_JSONFORMAT,
     ],
     serialized_options=None,
     is_extendable=True,
-    extension_ranges=[(1000, 1001), (1001, 1002), (1002, 1003), (9990, 9991), (9995, 10000), (10000, 10001), ],
+    extension_ranges=[(1000, 9995), (9995, 10000), (10000, 10001), ],
     oneofs=[
     ],
   )
 
 
   _FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT = _descriptor.Descriptor(
     name='FeatureSetEditionDefault',
@@ -3053,16 +3053,16 @@
   _globals['_FEATURESET'].fields_by_name['json_format']._serialized_options = b'\210\001\001\230\001\003\230\001\006\230\001\001\242\001\027\022\022LEGACY_BEST_EFFORT\030\346\007\242\001\n\022\005ALLOW\030\347\007\262\001\003\010\350\007'
   _globals['_SOURCECODEINFO_LOCATION'].fields_by_name['path']._loaded_options = None
   _globals['_SOURCECODEINFO_LOCATION'].fields_by_name['path']._serialized_options = b'\020\001'
   _globals['_SOURCECODEINFO_LOCATION'].fields_by_name['span']._loaded_options = None
   _globals['_SOURCECODEINFO_LOCATION'].fields_by_name['span']._serialized_options = b'\020\001'
   _globals['_GENERATEDCODEINFO_ANNOTATION'].fields_by_name['path']._loaded_options = None
   _globals['_GENERATEDCODEINFO_ANNOTATION'].fields_by_name['path']._serialized_options = b'\020\001'
-  _globals['_EDITION']._serialized_start=11732
-  _globals['_EDITION']._serialized_end=12027
+  _globals['_EDITION']._serialized_start=11708
+  _globals['_EDITION']._serialized_end=12003
   _globals['_FILEDESCRIPTORSET']._serialized_start=53
   _globals['_FILEDESCRIPTORSET']._serialized_end=130
   _globals['_FILEDESCRIPTORPROTO']._serialized_start=133
   _globals['_FILEDESCRIPTORPROTO']._serialized_end=797
   _globals['_DESCRIPTORPROTO']._serialized_start=800
   _globals['_DESCRIPTORPROTO']._serialized_end=1625
   _globals['_DESCRIPTORPROTO_EXTENSIONRANGE']._serialized_start=1446
@@ -3126,35 +3126,35 @@
   _globals['_METHODOPTIONS_IDEMPOTENCYLEVEL']._serialized_start=8772
   _globals['_METHODOPTIONS_IDEMPOTENCYLEVEL']._serialized_end=8852
   _globals['_UNINTERPRETEDOPTION']._serialized_start=8866
   _globals['_UNINTERPRETEDOPTION']._serialized_end=9276
   _globals['_UNINTERPRETEDOPTION_NAMEPART']._serialized_start=9202
   _globals['_UNINTERPRETEDOPTION_NAMEPART']._serialized_end=9276
   _globals['_FEATURESET']._serialized_start=9279
-  _globals['_FEATURESET']._serialized_end=10616
+  _globals['_FEATURESET']._serialized_end=10592
   _globals['_FEATURESET_FIELDPRESENCE']._serialized_start=10095
   _globals['_FEATURESET_FIELDPRESENCE']._serialized_end=10187
   _globals['_FEATURESET_ENUMTYPE']._serialized_start=10189
   _globals['_FEATURESET_ENUMTYPE']._serialized_end=10244
   _globals['_FEATURESET_REPEATEDFIELDENCODING']._serialized_start=10246
   _globals['_FEATURESET_REPEATEDFIELDENCODING']._serialized_end=10332
   _globals['_FEATURESET_UTF8VALIDATION']._serialized_start=10334
   _globals['_FEATURESET_UTF8VALIDATION']._serialized_end=10401
   _globals['_FEATURESET_MESSAGEENCODING']._serialized_start=10403
   _globals['_FEATURESET_MESSAGEENCODING']._serialized_end=10486
   _globals['_FEATURESET_JSONFORMAT']._serialized_start=10488
   _globals['_FEATURESET_JSONFORMAT']._serialized_end=10560
-  _globals['_FEATURESETDEFAULTS']._serialized_start=10619
-  _globals['_FEATURESETDEFAULTS']._serialized_end=11092
-  _globals['_FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT']._serialized_start=10866
-  _globals['_FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT']._serialized_end=11092
-  _globals['_SOURCECODEINFO']._serialized_start=11095
-  _globals['_SOURCECODEINFO']._serialized_end=11390
-  _globals['_SOURCECODEINFO_LOCATION']._serialized_start=11184
-  _globals['_SOURCECODEINFO_LOCATION']._serialized_end=11390
-  _globals['_GENERATEDCODEINFO']._serialized_start=11393
-  _globals['_GENERATEDCODEINFO']._serialized_end=11729
-  _globals['_GENERATEDCODEINFO_ANNOTATION']._serialized_start=11494
-  _globals['_GENERATEDCODEINFO_ANNOTATION']._serialized_end=11729
-  _globals['_GENERATEDCODEINFO_ANNOTATION_SEMANTIC']._serialized_start=11689
-  _globals['_GENERATEDCODEINFO_ANNOTATION_SEMANTIC']._serialized_end=11729
+  _globals['_FEATURESETDEFAULTS']._serialized_start=10595
+  _globals['_FEATURESETDEFAULTS']._serialized_end=11068
+  _globals['_FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT']._serialized_start=10842
+  _globals['_FEATURESETDEFAULTS_FEATURESETEDITIONDEFAULT']._serialized_end=11068
+  _globals['_SOURCECODEINFO']._serialized_start=11071
+  _globals['_SOURCECODEINFO']._serialized_end=11366
+  _globals['_SOURCECODEINFO_LOCATION']._serialized_start=11160
+  _globals['_SOURCECODEINFO_LOCATION']._serialized_end=11366
+  _globals['_GENERATEDCODEINFO']._serialized_start=11369
+  _globals['_GENERATEDCODEINFO']._serialized_end=11705
+  _globals['_GENERATEDCODEINFO_ANNOTATION']._serialized_start=11470
+  _globals['_GENERATEDCODEINFO_ANNOTATION']._serialized_end=11705
+  _globals['_GENERATEDCODEINFO_ANNOTATION_SEMANTIC']._serialized_start=11665
+  _globals['_GENERATEDCODEINFO_ANNOTATION_SEMANTIC']._serialized_end=11705
 # @@protoc_insertion_point(module_scope)
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/descriptor_pool.py` & `protobuf-5.27.0rc3/google/protobuf/descriptor_pool.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/duration_pb2.py` & `protobuf-5.27.0rc3/google/protobuf/duration_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/duration.proto
-# Protobuf Python Version: 5.27.0-rc2
+# Protobuf Python Version: 5.27.0-rc3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _runtime_version.ValidateProtobufRuntimeVersion(
     _runtime_version.Domain.PUBLIC,
     5,
     27,
     0,
-    '-rc2',
+    '-rc3',
     'google/protobuf/duration.proto'
 )
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/empty_pb2.py` & `protobuf-5.27.0rc3/google/protobuf/empty_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/empty.proto
-# Protobuf Python Version: 5.27.0-rc2
+# Protobuf Python Version: 5.27.0-rc3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _runtime_version.ValidateProtobufRuntimeVersion(
     _runtime_version.Domain.PUBLIC,
     5,
     27,
     0,
-    '-rc2',
+    '-rc3',
     'google/protobuf/empty.proto'
 )
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/field_mask_pb2.py` & `protobuf-5.27.0rc3/google/protobuf/field_mask_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/field_mask.proto
-# Protobuf Python Version: 5.27.0-rc2
+# Protobuf Python Version: 5.27.0-rc3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _runtime_version.ValidateProtobufRuntimeVersion(
     _runtime_version.Domain.PUBLIC,
     5,
     27,
     0,
-    '-rc2',
+    '-rc3',
     'google/protobuf/field_mask.proto'
 )
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/_parameterized.py` & `protobuf-5.27.0rc3/google/protobuf/internal/_parameterized.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/api_implementation.py` & `protobuf-5.27.0rc3/google/protobuf/internal/api_implementation.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/builder.py` & `protobuf-5.27.0rc3/google/protobuf/internal/builder.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/containers.py` & `protobuf-5.27.0rc3/google/protobuf/internal/containers.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/decoder.py` & `protobuf-5.27.0rc3/google/protobuf/internal/decoder.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/encoder.py` & `protobuf-5.27.0rc3/google/protobuf/internal/encoder.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/enum_type_wrapper.py` & `protobuf-5.27.0rc3/google/protobuf/internal/enum_type_wrapper.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/extension_dict.py` & `protobuf-5.27.0rc3/google/protobuf/internal/extension_dict.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/field_mask.py` & `protobuf-5.27.0rc3/google/protobuf/internal/field_mask.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/message_listener.py` & `protobuf-5.27.0rc3/google/protobuf/internal/message_listener.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/python_message.py` & `protobuf-5.27.0rc3/google/protobuf/internal/python_message.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/testing_refleaks.py` & `protobuf-5.27.0rc3/google/protobuf/internal/testing_refleaks.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/type_checkers.py` & `protobuf-5.27.0rc3/google/protobuf/internal/type_checkers.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/well_known_types.py` & `protobuf-5.27.0rc3/google/protobuf/internal/well_known_types.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/internal/wire_format.py` & `protobuf-5.27.0rc3/google/protobuf/internal/wire_format.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/json_format.py` & `protobuf-5.27.0rc3/google/protobuf/json_format.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/message.py` & `protobuf-5.27.0rc3/google/protobuf/message.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/message_factory.py` & `protobuf-5.27.0rc3/google/protobuf/message_factory.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/proto_builder.py` & `protobuf-5.27.0rc3/google/protobuf/proto_builder.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/pyext/cpp_message.py` & `protobuf-5.27.0rc3/google/protobuf/pyext/cpp_message.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/reflection.py` & `protobuf-5.27.0rc3/google/protobuf/reflection.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/runtime_version.py` & `protobuf-5.27.0rc3/google/protobuf/runtime_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # The versions of this Python Protobuf runtime to be changed automatically by
 # the Protobuf release process. Do not edit them manually.
 DOMAIN = Domain.PUBLIC
 MAJOR = 5
 MINOR = 27
 PATCH = 0
-SUFFIX = '-rc2'
+SUFFIX = '-rc3'
 
 
 def ValidateProtobufRuntimeVersion(
     gen_domain, gen_major, gen_minor, gen_patch, gen_suffix, location
 ):
   """Function to validate versions.
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/service.py` & `protobuf-5.27.0rc3/google/protobuf/service.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/service_reflection.py` & `protobuf-5.27.0rc3/google/protobuf/service_reflection.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/source_context_pb2.py` & `protobuf-5.27.0rc3/google/protobuf/source_context_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/source_context.proto
-# Protobuf Python Version: 5.27.0-rc2
+# Protobuf Python Version: 5.27.0-rc3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _runtime_version.ValidateProtobufRuntimeVersion(
     _runtime_version.Domain.PUBLIC,
     5,
     27,
     0,
-    '-rc2',
+    '-rc3',
     'google/protobuf/source_context.proto'
 )
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/struct_pb2.py` & `protobuf-5.27.0rc3/google/protobuf/struct_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/struct.proto
-# Protobuf Python Version: 5.27.0-rc2
+# Protobuf Python Version: 5.27.0-rc3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _runtime_version.ValidateProtobufRuntimeVersion(
     _runtime_version.Domain.PUBLIC,
     5,
     27,
     0,
-    '-rc2',
+    '-rc3',
     'google/protobuf/struct.proto'
 )
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/symbol_database.py` & `protobuf-5.27.0rc3/google/protobuf/symbol_database.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/text_encoding.py` & `protobuf-5.27.0rc3/google/protobuf/text_encoding.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/text_format.py` & `protobuf-5.27.0rc3/google/protobuf/text_format.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/timestamp_pb2.py` & `protobuf-5.27.0rc3/google/protobuf/timestamp_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/timestamp.proto
-# Protobuf Python Version: 5.27.0-rc2
+# Protobuf Python Version: 5.27.0-rc3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _runtime_version.ValidateProtobufRuntimeVersion(
     _runtime_version.Domain.PUBLIC,
     5,
     27,
     0,
-    '-rc2',
+    '-rc3',
     'google/protobuf/timestamp.proto'
 )
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/type_pb2.py` & `protobuf-5.27.0rc3/google/protobuf/type_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/type.proto
-# Protobuf Python Version: 5.27.0-rc2
+# Protobuf Python Version: 5.27.0-rc3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _runtime_version.ValidateProtobufRuntimeVersion(
     _runtime_version.Domain.PUBLIC,
     5,
     27,
     0,
-    '-rc2',
+    '-rc3',
     'google/protobuf/type.proto'
 )
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.27.0rc2/google/protobuf/unknown_fields.py` & `protobuf-5.27.0rc3/google/protobuf/unknown_fields.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/google/protobuf/wrappers_pb2.py` & `protobuf-5.27.0rc3/google/protobuf/wrappers_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # NO CHECKED-IN PROTOBUF GENCODE
 # source: google/protobuf/wrappers.proto
-# Protobuf Python Version: 5.27.0-rc2
+# Protobuf Python Version: 5.27.0-rc3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import runtime_version as _runtime_version
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 _runtime_version.ValidateProtobufRuntimeVersion(
     _runtime_version.Domain.PUBLIC,
     5,
     27,
     0,
-    '-rc2',
+    '-rc3',
     'google/protobuf/wrappers.proto'
 )
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-5.27.0rc2/protobuf.egg-info/PKG-INFO` & `protobuf-5.27.0rc3/protobuf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf
-Version: 5.27.0rc2
+Version: 5.27.0rc3
 Summary: Protocol Buffers
 Home-page: https://developers.google.com/protocol-buffers/
 Download-URL: https://github.com/protocolbuffers/protobuf/releases
 Maintainer: protobuf@googlegroups.com
 Maintainer-email: protobuf@googlegroups.com
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/protocolbuffers/protobuf
```

### Comparing `protobuf-5.27.0rc2/protobuf.egg-info/SOURCES.txt` & `protobuf-5.27.0rc3/protobuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/convert.c` & `protobuf-5.27.0rc3/python/convert.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/convert.h` & `protobuf-5.27.0rc3/python/convert.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/descriptor.c` & `protobuf-5.27.0rc3/python/descriptor.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/descriptor.h` & `protobuf-5.27.0rc3/python/descriptor.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/descriptor_containers.c` & `protobuf-5.27.0rc3/python/descriptor_containers.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/descriptor_containers.h` & `protobuf-5.27.0rc3/python/descriptor_containers.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/descriptor_pool.c` & `protobuf-5.27.0rc3/python/descriptor_pool.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/descriptor_pool.h` & `protobuf-5.27.0rc3/python/descriptor_pool.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/extension_dict.c` & `protobuf-5.27.0rc3/python/extension_dict.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/extension_dict.h` & `protobuf-5.27.0rc3/python/extension_dict.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/map.c` & `protobuf-5.27.0rc3/python/map.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/map.h` & `protobuf-5.27.0rc3/python/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/message.c` & `protobuf-5.27.0rc3/python/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/message.h` & `protobuf-5.27.0rc3/python/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/protobuf.c` & `protobuf-5.27.0rc3/python/protobuf.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/protobuf.h` & `protobuf-5.27.0rc3/python/protobuf.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/python_api.h` & `protobuf-5.27.0rc3/python/python_api.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/repeated.c` & `protobuf-5.27.0rc3/python/repeated.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/repeated.h` & `protobuf-5.27.0rc3/python/repeated.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/unknown_fields.c` & `protobuf-5.27.0rc3/python/unknown_fields.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/python/unknown_fields.h` & `protobuf-5.27.0rc3/python/unknown_fields.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/setup.py` & `protobuf-5.27.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/base/descriptor_constants.h` & `protobuf-5.27.0rc3/upb/base/descriptor_constants.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/base/internal/endian.h` & `protobuf-5.27.0rc3/upb/base/internal/endian.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/base/internal/log2.h` & `protobuf-5.27.0rc3/upb/base/internal/log2.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/base/status.c` & `protobuf-5.27.0rc3/upb/base/status.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/base/status.h` & `protobuf-5.27.0rc3/upb/base/status.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/base/string_view.h` & `protobuf-5.27.0rc3/upb/base/string_view.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/base/upcast.h` & `protobuf-5.27.0rc3/upb/base/upcast.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/generated_code_support.h` & `protobuf-5.27.0rc3/upb/generated_code_support.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/hash/common.c` & `protobuf-5.27.0rc3/upb/hash/common.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/hash/common.h` & `protobuf-5.27.0rc3/upb/hash/common.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/hash/int_table.h` & `protobuf-5.27.0rc3/upb/hash/int_table.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/hash/str_table.h` & `protobuf-5.27.0rc3/upb/hash/str_table.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/lex/atoi.c` & `protobuf-5.27.0rc3/upb/lex/atoi.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/lex/atoi.h` & `protobuf-5.27.0rc3/upb/lex/atoi.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/lex/round_trip.c` & `protobuf-5.27.0rc3/upb/lex/round_trip.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/lex/round_trip.h` & `protobuf-5.27.0rc3/upb/lex/round_trip.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/lex/strtod.c` & `protobuf-5.27.0rc3/upb/lex/strtod.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/lex/strtod.h` & `protobuf-5.27.0rc3/upb/lex/strtod.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/lex/unicode.c` & `protobuf-5.27.0rc3/upb/lex/unicode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/lex/unicode.h` & `protobuf-5.27.0rc3/upb/lex/unicode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mem/alloc.c` & `protobuf-5.27.0rc3/upb/mem/alloc.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mem/alloc.h` & `protobuf-5.27.0rc3/upb/mem/alloc.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mem/arena.c` & `protobuf-5.27.0rc3/upb/mem/arena.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mem/arena.h` & `protobuf-5.27.0rc3/upb/mem/arena.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mem/internal/arena.h` & `protobuf-5.27.0rc3/upb/mem/internal/arena.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/accessors.c` & `protobuf-5.27.0rc3/upb/message/accessors.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/accessors.h` & `protobuf-5.27.0rc3/upb/message/accessors.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/accessors_split64.h` & `protobuf-5.27.0rc3/upb/message/accessors_split64.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/array.c` & `protobuf-5.27.0rc3/upb/message/array.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/array.h` & `protobuf-5.27.0rc3/upb/message/array.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/compare.c` & `protobuf-5.27.0rc3/upb/message/compare.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/compare.h` & `protobuf-5.27.0rc3/upb/message/compare.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/compat.c` & `protobuf-5.27.0rc3/upb/message/compat.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/compat.h` & `protobuf-5.27.0rc3/upb/message/compat.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/copy.c` & `protobuf-5.27.0rc3/upb/message/copy.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/copy.h` & `protobuf-5.27.0rc3/upb/message/copy.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/accessors.h` & `protobuf-5.27.0rc3/upb/message/internal/accessors.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/array.h` & `protobuf-5.27.0rc3/upb/message/internal/array.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/compare_unknown.c` & `protobuf-5.27.0rc3/upb/message/internal/compare_unknown.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/compare_unknown.h` & `protobuf-5.27.0rc3/upb/message/internal/compare_unknown.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/extension.c` & `protobuf-5.27.0rc3/upb/message/internal/extension.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/extension.h` & `protobuf-5.27.0rc3/upb/message/internal/extension.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/map.h` & `protobuf-5.27.0rc3/upb/message/internal/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/map_entry.h` & `protobuf-5.27.0rc3/upb/message/internal/map_entry.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/map_sorter.h` & `protobuf-5.27.0rc3/upb/message/internal/map_sorter.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/message.c` & `protobuf-5.27.0rc3/upb/message/internal/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/message.h` & `protobuf-5.27.0rc3/upb/message/internal/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/tagged_ptr.h` & `protobuf-5.27.0rc3/upb/message/internal/tagged_ptr.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/internal/types.h` & `protobuf-5.27.0rc3/upb/message/internal/types.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/map.c` & `protobuf-5.27.0rc3/upb/message/map.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/map.h` & `protobuf-5.27.0rc3/upb/message/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/map_gencode_util.h` & `protobuf-5.27.0rc3/upb/message/map_gencode_util.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/map_sorter.c` & `protobuf-5.27.0rc3/upb/message/map_sorter.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/message.c` & `protobuf-5.27.0rc3/upb/message/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/message.h` & `protobuf-5.27.0rc3/upb/message/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/promote.c` & `protobuf-5.27.0rc3/upb/message/promote.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/promote.h` & `protobuf-5.27.0rc3/upb/message/promote.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/tagged_ptr.h` & `protobuf-5.27.0rc3/upb/message/tagged_ptr.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/message/value.h` & `protobuf-5.27.0rc3/upb/message/value.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/build_enum.c` & `protobuf-5.27.0rc3/upb/mini_descriptor/build_enum.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/build_enum.h` & `protobuf-5.27.0rc3/upb/mini_descriptor/build_enum.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/decode.c` & `protobuf-5.27.0rc3/upb/mini_descriptor/decode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/decode.h` & `protobuf-5.27.0rc3/upb/mini_descriptor/decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/internal/base92.c` & `protobuf-5.27.0rc3/upb/mini_descriptor/internal/base92.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/internal/base92.h` & `protobuf-5.27.0rc3/upb/mini_descriptor/internal/base92.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/internal/decoder.h` & `protobuf-5.27.0rc3/upb/mini_descriptor/internal/decoder.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/internal/encode.c` & `protobuf-5.27.0rc3/upb/mini_descriptor/internal/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/internal/encode.h` & `protobuf-5.27.0rc3/upb/mini_descriptor/internal/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/internal/modifiers.h` & `protobuf-5.27.0rc3/upb/mini_descriptor/internal/modifiers.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/internal/wire_constants.h` & `protobuf-5.27.0rc3/upb/mini_descriptor/internal/wire_constants.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/link.c` & `protobuf-5.27.0rc3/upb/mini_descriptor/link.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_descriptor/link.h` & `protobuf-5.27.0rc3/upb/mini_descriptor/link.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/compat.c` & `protobuf-5.27.0rc3/upb/mini_table/compat.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/compat.h` & `protobuf-5.27.0rc3/upb/mini_table/compat.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/enum.h` & `protobuf-5.27.0rc3/upb/mini_table/enum.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/extension.h` & `protobuf-5.27.0rc3/upb/mini_table/extension.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/extension_registry.c` & `protobuf-5.27.0rc3/upb/mini_table/extension_registry.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/extension_registry.h` & `protobuf-5.27.0rc3/upb/mini_table/extension_registry.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/field.h` & `protobuf-5.27.0rc3/upb/mini_table/field.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/file.h` & `protobuf-5.27.0rc3/upb/mini_table/file.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/internal/enum.h` & `protobuf-5.27.0rc3/upb/mini_table/internal/enum.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/internal/extension.h` & `protobuf-5.27.0rc3/upb/mini_table/internal/extension.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/internal/field.h` & `protobuf-5.27.0rc3/upb/mini_table/internal/field.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/internal/file.h` & `protobuf-5.27.0rc3/upb/mini_table/internal/file.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/internal/message.c` & `protobuf-5.27.0rc3/upb/mini_table/internal/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/internal/message.h` & `protobuf-5.27.0rc3/upb/mini_table/internal/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/internal/size_log2.h` & `protobuf-5.27.0rc3/upb/mini_table/internal/size_log2.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/internal/sub.h` & `protobuf-5.27.0rc3/upb/mini_table/internal/sub.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/message.c` & `protobuf-5.27.0rc3/upb/mini_table/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/message.h` & `protobuf-5.27.0rc3/upb/mini_table/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/mini_table/sub.h` & `protobuf-5.27.0rc3/upb/mini_table/sub.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/port/atomic.h` & `protobuf-5.27.0rc3/upb/port/atomic.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/port/def.inc` & `protobuf-5.27.0rc3/upb/port/def.inc`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/port/undef.inc` & `protobuf-5.27.0rc3/upb/port/undef.inc`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/port/vsnprintf_compat.h` & `protobuf-5.27.0rc3/upb/port/vsnprintf_compat.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/common.h` & `protobuf-5.27.0rc3/upb/reflection/common.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/def.h` & `protobuf-5.27.0rc3/upb/reflection/def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/def_pool.c` & `protobuf-5.27.0rc3/upb/reflection/def_pool.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/def_pool.h` & `protobuf-5.27.0rc3/upb/reflection/def_pool.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/def_type.c` & `protobuf-5.27.0rc3/upb/reflection/def_type.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/def_type.h` & `protobuf-5.27.0rc3/upb/reflection/def_type.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/desc_state.c` & `protobuf-5.27.0rc3/upb/reflection/desc_state.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/enum_def.c` & `protobuf-5.27.0rc3/upb/reflection/enum_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/enum_def.h` & `protobuf-5.27.0rc3/upb/reflection/enum_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/enum_reserved_range.c` & `protobuf-5.27.0rc3/upb/reflection/enum_reserved_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/enum_reserved_range.h` & `protobuf-5.27.0rc3/upb/reflection/enum_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/enum_value_def.c` & `protobuf-5.27.0rc3/upb/reflection/enum_value_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/enum_value_def.h` & `protobuf-5.27.0rc3/upb/reflection/enum_value_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/extension_range.c` & `protobuf-5.27.0rc3/upb/reflection/extension_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/extension_range.h` & `protobuf-5.27.0rc3/upb/reflection/extension_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/field_def.c` & `protobuf-5.27.0rc3/upb/reflection/field_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/field_def.h` & `protobuf-5.27.0rc3/upb/reflection/field_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/file_def.c` & `protobuf-5.27.0rc3/upb/reflection/file_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/file_def.h` & `protobuf-5.27.0rc3/upb/reflection/file_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/def_builder.c` & `protobuf-5.27.0rc3/upb/reflection/internal/def_builder.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/def_builder.h` & `protobuf-5.27.0rc3/upb/reflection/internal/def_builder.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/def_pool.h` & `protobuf-5.27.0rc3/upb/reflection/internal/def_pool.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/desc_state.h` & `protobuf-5.27.0rc3/upb/reflection/internal/desc_state.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/enum_def.h` & `protobuf-5.27.0rc3/upb/reflection/internal/enum_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/enum_reserved_range.h` & `protobuf-5.27.0rc3/upb/reflection/internal/enum_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/enum_value_def.h` & `protobuf-5.27.0rc3/upb/reflection/internal/enum_value_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/extension_range.h` & `protobuf-5.27.0rc3/upb/reflection/internal/extension_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/field_def.h` & `protobuf-5.27.0rc3/upb/reflection/internal/field_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/file_def.h` & `protobuf-5.27.0rc3/upb/reflection/internal/file_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/message_def.h` & `protobuf-5.27.0rc3/upb/reflection/internal/message_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/message_reserved_range.h` & `protobuf-5.27.0rc3/upb/reflection/internal/message_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/method_def.h` & `protobuf-5.27.0rc3/upb/reflection/internal/method_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/oneof_def.h` & `protobuf-5.27.0rc3/upb/reflection/internal/oneof_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/service_def.h` & `protobuf-5.27.0rc3/upb/reflection/internal/service_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/strdup2.c` & `protobuf-5.27.0rc3/upb/reflection/internal/strdup2.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/strdup2.h` & `protobuf-5.27.0rc3/upb/reflection/internal/strdup2.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/internal/upb_edition_defaults.h` & `protobuf-5.27.0rc3/upb/reflection/internal/upb_edition_defaults.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/message.c` & `protobuf-5.27.0rc3/upb/reflection/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/message.h` & `protobuf-5.27.0rc3/upb/reflection/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/message_def.c` & `protobuf-5.27.0rc3/upb/reflection/message_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/message_def.h` & `protobuf-5.27.0rc3/upb/reflection/message_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/message_reserved_range.c` & `protobuf-5.27.0rc3/upb/reflection/message_reserved_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/message_reserved_range.h` & `protobuf-5.27.0rc3/upb/reflection/message_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/method_def.c` & `protobuf-5.27.0rc3/upb/reflection/method_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/method_def.h` & `protobuf-5.27.0rc3/upb/reflection/method_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/oneof_def.c` & `protobuf-5.27.0rc3/upb/reflection/oneof_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/oneof_def.h` & `protobuf-5.27.0rc3/upb/reflection/oneof_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/service_def.c` & `protobuf-5.27.0rc3/upb/reflection/service_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/reflection/service_def.h` & `protobuf-5.27.0rc3/upb/reflection/service_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/text/encode.c` & `protobuf-5.27.0rc3/upb/text/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/text/encode.h` & `protobuf-5.27.0rc3/upb/text/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/util/def_to_proto.c` & `protobuf-5.27.0rc3/upb/util/def_to_proto.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/util/def_to_proto.h` & `protobuf-5.27.0rc3/upb/util/def_to_proto.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/util/required_fields.c` & `protobuf-5.27.0rc3/upb/util/required_fields.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/util/required_fields.h` & `protobuf-5.27.0rc3/upb/util/required_fields.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/decode.c` & `protobuf-5.27.0rc3/upb/wire/decode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/decode.h` & `protobuf-5.27.0rc3/upb/wire/decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/encode.c` & `protobuf-5.27.0rc3/upb/wire/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/encode.h` & `protobuf-5.27.0rc3/upb/wire/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/eps_copy_input_stream.c` & `protobuf-5.27.0rc3/upb/wire/eps_copy_input_stream.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/eps_copy_input_stream.h` & `protobuf-5.27.0rc3/upb/wire/eps_copy_input_stream.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/internal/constants.h` & `protobuf-5.27.0rc3/upb/wire/internal/constants.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/internal/decode_fast.c` & `protobuf-5.27.0rc3/upb/wire/internal/decode_fast.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/internal/decode_fast.h` & `protobuf-5.27.0rc3/upb/wire/internal/decode_fast.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/internal/decoder.h` & `protobuf-5.27.0rc3/upb/wire/internal/decoder.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/internal/reader.h` & `protobuf-5.27.0rc3/upb/wire/internal/reader.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/reader.c` & `protobuf-5.27.0rc3/upb/wire/reader.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/reader.h` & `protobuf-5.27.0rc3/upb/wire/reader.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/upb/wire/types.h` & `protobuf-5.27.0rc3/upb/wire/types.h`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/utf8_range/utf8_range.c` & `protobuf-5.27.0rc3/utf8_range/utf8_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-5.27.0rc2/utf8_range/utf8_range.h` & `protobuf-5.27.0rc3/utf8_range/utf8_range.h`

 * *Files identical despite different names*

