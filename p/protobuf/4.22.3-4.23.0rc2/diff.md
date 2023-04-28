# Comparing `tmp/protobuf-4.22.3.tar.gz` & `tmp/protobuf-4.23.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/protobuf-4.22.3.tar", last modified: Wed Apr 12 23:06:43 2023, max compression
+gzip compressed data, was "dist/protobuf-4.23.0rc2.tar", last modified: Fri Apr 28 17:47:02 2023, max compression
```

## Comparing `protobuf-4.22.3.tar` & `protobuf-4.23.0rc2.tar`

### file list

```diff
@@ -1,264 +1,271 @@
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/
--r-xr-xr-x   0 bazel     (1000) bazel     (1003)       39 2000-01-01 00:00:00.000000 protobuf-4.22.3/MANIFEST.in
--rw-r--r--   0 bazel     (1000) bazel     (1003)      774 2023-04-12 23:06:42.000000 protobuf-4.22.3/PKG-INFO
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4040 2000-01-01 00:00:00.000000 protobuf-4.22.3/README.md
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/google/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      150 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/__init__.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/google/protobuf/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1705 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1420 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/any_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2840 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/api_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/google/protobuf/compiler/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/compiler/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3174 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/compiler/plugin_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    47968 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/descriptor.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    58733 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/descriptor.upb.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)   304335 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/descriptor.upb.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    48145 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/descriptor.upbdefs.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7749 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/descriptor.upbdefs.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6819 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/descriptor_database.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)   128332 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/descriptor_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    46876 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/descriptor_pool.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1495 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/duration_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1362 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/empty_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1453 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/field_mask_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/google/protobuf/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1631 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    15432 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/_parameterized.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6126 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/api_implementation.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5188 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/builder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    23328 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/containers.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    38796 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/decoder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    28656 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/encoder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4821 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/enum_type_wrapper.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8485 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/extension_dict.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    11775 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/field_mask.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3367 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/message_listener.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    57025 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/python_message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5439 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/testing_refleaks.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    16809 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/type_checkers.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    20096 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/well_known_types.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8446 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/internal/wire_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    36297 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/json_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14551 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9098 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/message_factory.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5562 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/proto_builder.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/google/protobuf/pyext/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/pyext/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3071 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/pyext/cpp_message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3772 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/reflection.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9146 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/service.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    11417 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/service_reflection.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1475 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/source_context_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2722 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/struct_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8078 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/symbol_database.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4701 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/text_encoding.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    64198 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/text_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1504 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/timestamp_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4973 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/type_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4486 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/unknown_fields.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/google/protobuf/util/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/util/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2727 2000-01-01 00:00:00.000000 protobuf-4.22.3/google/protobuf/wrappers_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/protobuf.egg-info/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      774 2023-04-12 23:06:42.000000 protobuf-4.22.3/protobuf.egg-info/PKG-INFO
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6346 2023-04-12 23:06:42.000000 protobuf-4.22.3/protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2023-04-12 23:06:42.000000 protobuf-4.22.3/protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2023-04-12 23:06:42.000000 protobuf-4.22.3/protobuf.egg-info/namespace_packages.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2023-04-12 23:06:42.000000 protobuf-4.22.3/protobuf.egg-info/top_level.txt
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/python/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    15821 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/convert.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3195 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/convert.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    69085 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/descriptor.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3740 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/descriptor.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    28410 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/descriptor_containers.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5443 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/descriptor_containers.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    22990 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/descriptor_pool.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2222 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/descriptor_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9828 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/extension_dict.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1816 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/extension_dict.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    20520 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/map.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3071 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    70371 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4836 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    11933 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/protobuf.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9135 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/protobuf.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2928 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/python_api.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    31454 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/repeated.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3373 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/repeated.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12078 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/unknown_fields.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1817 2000-01-01 00:00:00.000000 protobuf-4.22.3/python/unknown_fields.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)       67 2023-04-12 23:06:42.000000 protobuf-4.22.3/setup.cfg
--r-xr-xr-x   0 bazel     (1000) bazel     (1003)     3876 2000-01-01 00:00:00.000000 protobuf-4.22.3/setup.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1771 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/alloc.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1771 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/arena.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1795 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/array.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/base/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3148 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/base/descriptor_constants.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2078 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/base/log2.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3033 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/base/status.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2645 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/base/status.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2669 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/base/string_view.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/collections/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4970 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/collections/array.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3672 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/collections/array.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5001 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/collections/array_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4734 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/collections/map.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5422 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/collections/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2989 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/collections/map_gencode_util.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5900 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/collections/map_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6037 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/collections/map_sorter.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3986 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/collections/map_sorter_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2376 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/collections/message_value.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1838 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/collections.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1810 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/decode_fast.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1799 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/extension_registry.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/hash/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    25532 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/hash/common.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7082 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/hash/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4154 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/hash/int_table.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6065 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/hash/str_table.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/json/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    44075 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/json/decode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2103 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/json/decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    23909 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/json/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2883 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/json/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/json_decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/json_encode.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/lex/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2426 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/lex/atoi.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2256 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/lex/atoi.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2811 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/lex/round_trip.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2328 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/lex/round_trip.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4061 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/lex/strtod.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1872 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/lex/strtod.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2195 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/lex/unicode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3002 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/lex/unicode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1783 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/map.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/mem/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1985 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mem/alloc.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3564 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mem/alloc.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8174 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mem/arena.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5394 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mem/arena.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2655 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mem/arena_internal.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/message/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14362 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/message/accessors.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    31418 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/message/accessors.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3467 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/message/extension_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5064 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/message/internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7003 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/message/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2955 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/message/message.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/mini_table/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4675 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/common.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5163 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4097 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/common_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    36061 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/decode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5625 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12205 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4873 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/encode_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3666 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/enum_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2098 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/extension_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3710 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/extension_registry.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4681 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/extension_registry.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6409 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/field_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1989 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/file_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5013 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/message_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1818 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/sub_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2007 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table/types.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1807 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/mini_table.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1787 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/msg.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1798 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/msg_internal.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/port/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10264 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/port/def.inc
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2507 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/port/undef.inc
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2258 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/port/vsnprintf_compat.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/reflection/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2873 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2054 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    11441 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/def_builder.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7014 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/def_builder_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    16058 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/def_pool.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4588 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/def_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3349 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/def_pool_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2244 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/def_type.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3031 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/def_type.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2212 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/desc_state.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2402 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/desc_state_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    11150 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/enum_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3562 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/enum_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2331 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/enum_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3411 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/enum_reserved_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2101 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/enum_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2346 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/enum_reserved_range_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5416 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/enum_value_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2420 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/enum_value_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2422 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/enum_value_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3751 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/extension_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2244 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/extension_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2263 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/extension_range_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    30706 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/field_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4217 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/field_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3245 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/field_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12878 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/file_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3275 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/file_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2406 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/file_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8597 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4357 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    25921 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/message_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7420 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/message_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2871 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/message_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3281 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/message_reserved_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2122 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/message_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2324 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/message_reserved_range_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4529 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/method_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2569 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/method_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2194 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/method_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7325 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/oneof_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3000 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/oneof_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2394 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/oneof_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4632 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/service_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2603 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/service_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2173 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/service_def_internal.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/reflection/stage0/
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/reflection/stage0/google/
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/reflection/stage0/google/protobuf/
--rw-r--r--   0 bazel     (1000) bazel     (1003)   279249 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection/stage0/google/protobuf/descriptor.upb.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/reflection.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/status.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1810 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/string_view.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/text/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    13495 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/text/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2740 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/text/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/text_encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1879 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/upb.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/util/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10885 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/util/compare.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2866 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/util/compare.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    25145 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/util/def_to_proto.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3023 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/util/def_to_proto.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10836 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/util/required_fields.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4107 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/util/required_fields.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/upb/wire/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2023 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/common_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    48006 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/decode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3956 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    51605 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/decode_fast.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5245 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/decode_fast.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5929 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/decode_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    21114 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3003 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2010 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/eps_copy_input_stream.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    18408 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/eps_copy_input_stream.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2721 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/reader.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8847 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/reader.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2367 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/swap_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1906 2000-01-01 00:00:00.000000 protobuf-4.22.3/upb/wire/types.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-12 23:06:42.000000 protobuf-4.22.3/utf8_range/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3990 2000-01-01 00:00:00.000000 protobuf-4.22.3/utf8_range/naive.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5620 2000-01-01 00:00:00.000000 protobuf-4.22.3/utf8_range/range2-neon.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5917 2000-01-01 00:00:00.000000 protobuf-4.22.3/utf8_range/range2-sse.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      517 2000-01-01 00:00:00.000000 protobuf-4.22.3/utf8_range/utf8_range.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/
+-r-xr-xr-x   0 bazel     (1000) bazel     (1003)       39 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/MANIFEST.in
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      777 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/PKG-INFO
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4376 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/README.md
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/google/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      150 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/__init__.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/google/protobuf/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1708 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1420 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/any_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2840 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/api_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/google/protobuf/compiler/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/compiler/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3174 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/compiler/plugin_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    47968 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    61064 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor.upb.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)   359010 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor.upb.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    51014 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor.upbdefs.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8036 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor.upbdefs.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6819 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor_database.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)   136435 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    46876 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor_pool.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1495 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/duration_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1362 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/empty_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1453 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/field_mask_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/google/protobuf/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1631 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    15432 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/_parameterized.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6126 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/api_implementation.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5188 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/builder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    23328 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/containers.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    38796 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/decoder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    28656 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/encoder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4821 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/enum_type_wrapper.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8485 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/extension_dict.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    11775 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/field_mask.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3367 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/message_listener.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    57025 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/python_message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5439 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/testing_refleaks.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    16809 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/type_checkers.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    20096 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/well_known_types.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8446 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/wire_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    36297 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/json_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    14551 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8952 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/message_factory.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5562 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/proto_builder.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/google/protobuf/pyext/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/pyext/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3071 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/pyext/cpp_message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3772 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/reflection.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9146 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/service.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    11417 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/service_reflection.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1475 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/source_context_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2722 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/struct_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8078 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/symbol_database.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4701 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/text_encoding.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    64011 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/text_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1504 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/timestamp_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5132 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/type_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4486 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/unknown_fields.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/google/protobuf/util/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/util/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2727 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/wrappers_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/protobuf.egg-info/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      777 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6497 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/protobuf.egg-info/namespace_packages.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/protobuf.egg-info/top_level.txt
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/python/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    15821 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/convert.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3195 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/convert.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    69085 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/descriptor.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3740 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/descriptor.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    28410 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/descriptor_containers.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5443 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/descriptor_containers.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    22990 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/descriptor_pool.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2222 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/descriptor_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9828 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/extension_dict.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1816 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/extension_dict.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    20520 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/map.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3071 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    71006 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4985 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    11933 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/protobuf.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9135 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/protobuf.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2928 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/python_api.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    31454 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/repeated.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3373 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/repeated.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12078 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/unknown_fields.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1817 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/unknown_fields.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)       67 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/setup.cfg
+-r-xr-xr-x   0 bazel     (1000) bazel     (1003)     3876 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/setup.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1771 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/alloc.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1771 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/arena.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1795 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/array.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/base/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3670 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/base/descriptor_constants.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2078 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/base/log2.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3033 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/base/status.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2645 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/base/status.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2669 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/base/string_view.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/collections/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5012 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/array.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3672 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/array.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5080 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/array_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4755 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/map.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5422 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2989 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/map_gencode_util.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5900 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/map_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6037 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/map_sorter.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3986 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/map_sorter_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2376 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/message_value.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1838 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1810 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/decode_fast.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1799 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/extension_registry.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/hash/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    25548 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/hash/common.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7082 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/hash/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4154 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/hash/int_table.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6065 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/hash/str_table.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/json/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    44075 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/json/decode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2103 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/json/decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    23909 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/json/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2883 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/json/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/json_decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/json_encode.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/lex/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2426 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/atoi.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2256 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/atoi.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2811 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/round_trip.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2328 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/round_trip.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4061 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/strtod.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1872 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/strtod.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2195 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/unicode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3002 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/unicode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1783 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/map.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/mem/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1985 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mem/alloc.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3564 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mem/alloc.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    13876 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mem/arena.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5352 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mem/arena.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4324 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mem/arena_internal.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/message/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3308 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/accessors.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    16666 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/accessors.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12752 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/accessors_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10705 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/copy.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2614 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/copy.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3467 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/extension_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5064 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7003 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2831 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    13430 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/promote.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4841 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/promote.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/mini_table/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4719 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/common.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6232 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3763 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/common_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    40569 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/decode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8579 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12204 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4916 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/encode_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3666 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/enum_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2098 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/extension_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3829 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/extension_registry.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4829 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/extension_registry.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6775 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/field_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1989 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/file_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5149 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/message_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1818 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/sub_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2007 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/types.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1807 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1787 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/msg.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1798 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/msg_internal.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/port/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4420 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/port/atomic.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10443 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/port/def.inc
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2571 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/port/undef.inc
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2258 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/port/vsnprintf_compat.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/reflection/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2873 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2054 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    11441 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_builder.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7014 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_builder_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    16058 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_pool.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4588 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3349 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_pool_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2244 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_type.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3031 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_type.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2212 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/desc_state.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2402 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/desc_state_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    11150 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3562 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2331 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3411 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_reserved_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2101 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2346 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_reserved_range_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5416 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_value_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2420 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_value_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2422 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_value_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3751 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/extension_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2244 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/extension_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2263 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/extension_range_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    30643 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/field_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4217 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/field_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3245 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/field_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12878 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/file_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3275 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/file_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2406 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/file_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8597 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4357 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    25921 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7420 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2871 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3281 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message_reserved_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2122 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2324 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message_reserved_range_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4529 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/method_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2569 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/method_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2194 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/method_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8161 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/oneof_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3000 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/oneof_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2401 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/oneof_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4632 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/service_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2603 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/service_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2173 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/service_def_internal.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/reflection/stage0/
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/reflection/stage0/google/
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/reflection/stage0/google/protobuf/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)   279249 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/stage0/google/protobuf/descriptor.upb.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/status.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1810 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/string_view.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/text/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    13495 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/text/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2740 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/text/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/text_encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1879 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/upb.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/util/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10885 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/util/compare.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2866 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/util/compare.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    25065 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/util/def_to_proto.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3023 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/util/def_to_proto.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10836 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/util/required_fields.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4107 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/util/required_fields.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/wire/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1811 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2023 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/common_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    49488 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/decode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4418 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    51605 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/decode_fast.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5245 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/decode_fast.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5929 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/decode_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    21305 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3423 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2010 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/eps_copy_input_stream.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    18408 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/eps_copy_input_stream.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2721 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/reader.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8847 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/reader.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2367 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/swap_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1906 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/types.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/utf8_range/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3990 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/utf8_range/naive.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5620 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/utf8_range/range2-neon.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5917 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/utf8_range/range2-sse.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      517 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/utf8_range/utf8_range.h
```

### Comparing `protobuf-4.22.3/PKG-INFO` & `protobuf-4.23.0rc2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: protobuf
-Version: 4.22.3
+Version: 4.23.0rc2
 Summary: Protocol Buffers
 Home-page: https://developers.google.com/protocol-buffers/
 Maintainer: protobuf@googlegroups.com
 Maintainer-email: protobuf@googlegroups.com
 License: BSD-3-Clause
 Download-URL: https://github.com/protocolbuffers/protobuf/releases
 Project-URL: Source, https://github.com/protocolbuffers/protobuf
```

### Comparing `protobuf-4.22.3/google/protobuf/__init__.py` & `protobuf-4.23.0rc2/google/protobuf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 # DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 # THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 # Copyright 2007 Google Inc. All Rights Reserved.
 
-__version__ = '4.22.3'
+__version__ = '4.23.0rc2'
```

### Comparing `protobuf-4.22.3/google/protobuf/any_pb2.py` & `protobuf-4.23.0rc2/google/protobuf/any_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/any.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-4.22.3/google/protobuf/api_pb2.py` & `protobuf-4.23.0rc2/google/protobuf/api_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/api.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import source_context_pb2 as google_dot_protobuf_dot_source__context__pb2
 from google.protobuf import type_pb2 as google_dot_protobuf_dot_type__pb2
```

### Comparing `protobuf-4.22.3/google/protobuf/compiler/plugin_pb2.py` & `protobuf-4.23.0rc2/google/protobuf/compiler/plugin_pb2.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/compiler/plugin.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
```

### Comparing `protobuf-4.22.3/google/protobuf/descriptor.py` & `protobuf-4.23.0rc2/google/protobuf/descriptor.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/descriptor.upb.c` & `protobuf-4.23.0rc2/google/protobuf/descriptor.upb.c`

 * *Files 2% similar despite different names*

```diff
@@ -60,27 +60,27 @@
 
 const upb_MiniTable google_protobuf_FileDescriptorProto_msg_init = {
   &google_protobuf_FileDescriptorProto_submsgs[0],
   &google_protobuf_FileDescriptorProto__fields[0],
   UPB_SIZE(72, 144), 13, kUpb_ExtMode_NonExtendable, 13, UPB_FASTTABLE_MASK(120), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x000800000100000a, &upb_psb_1bt},
-    {0x0018000002000012, &upb_psb_1bt},
-    {0x002800003f00001a, &upb_prb_1bt},
+    {0x000800000100000a, &upb_pss_1bt},
+    {0x0018000002000012, &upb_pss_1bt},
+    {0x002800003f00001a, &upb_prs_1bt},
     {0x003000003f000022, &upb_prm_1bt_max128b},
     {0x003800003f01002a, &upb_prm_1bt_max64b},
     {0x004000003f020032, &upb_prm_1bt_max64b},
     {0x004800003f03003a, &upb_prm_1bt_max128b},
     {0x0050000003040042, &upb_psm_1bt_max256b},
     {0x005800000405004a, &upb_psm_1bt_max64b},
     {0x006000003f000050, &upb_prv4_1bt},
     {0x006800003f000058, &upb_prv4_1bt},
-    {0x0070000005000062, &upb_psb_1bt},
-    {0x008000000600006a, &upb_psb_1bt},
+    {0x0070000005000062, &upb_pss_1bt},
+    {0x008000000600006a, &upb_pss_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
 
 static const upb_MiniTableSub google_protobuf_DescriptorProto_submsgs[8] = {
   {.submsg = &google_protobuf_FieldDescriptorProto_msg_init},
@@ -108,24 +108,24 @@
 
 const upb_MiniTable google_protobuf_DescriptorProto_msg_init = {
   &google_protobuf_DescriptorProto_submsgs[0],
   &google_protobuf_DescriptorProto__fields[0],
   UPB_SIZE(48, 96), 10, kUpb_ExtMode_NonExtendable, 10, UPB_FASTTABLE_MASK(120), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x000800000100000a, &upb_psb_1bt},
+    {0x000800000100000a, &upb_pss_1bt},
     {0x001800003f000012, &upb_prm_1bt_max128b},
     {0x002000003f01001a, &upb_prm_1bt_max128b},
     {0x002800003f020022, &upb_prm_1bt_max64b},
     {0x003000003f03002a, &upb_prm_1bt_max64b},
     {0x003800003f040032, &upb_prm_1bt_max128b},
     {0x004000000205003a, &upb_psm_1bt_max64b},
     {0x004800003f060042, &upb_prm_1bt_max64b},
     {0x005000003f07004a, &upb_prm_1bt_max64b},
-    {0x005800003f000052, &upb_prb_1bt},
+    {0x005800003f000052, &upb_prs_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
@@ -165,29 +165,34 @@
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0004000001000008, &upb_psv4_1bt},
     {0x0008000002000010, &upb_psv4_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
 
-static const upb_MiniTableSub google_protobuf_ExtensionRangeOptions_submsgs[1] = {
+static const upb_MiniTableSub google_protobuf_ExtensionRangeOptions_submsgs[3] = {
+  {.submsg = &google_protobuf_ExtensionRangeOptions_Declaration_msg_init},
+  {.subenum = &google_protobuf_ExtensionRangeOptions_VerificationState_enum_init},
   {.submsg = &google_protobuf_UninterpretedOption_msg_init},
 };
 
-static const upb_MiniTableField google_protobuf_ExtensionRangeOptions__fields[1] = {
-  {999, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
+static const upb_MiniTableField google_protobuf_ExtensionRangeOptions__fields[3] = {
+  {2, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
+  {3, UPB_SIZE(8, 4), 1, 1, 14, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
+  {999, UPB_SIZE(12, 16), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google_protobuf_ExtensionRangeOptions_msg_init = {
   &google_protobuf_ExtensionRangeOptions_submsgs[0],
   &google_protobuf_ExtensionRangeOptions__fields[0],
-  8, 1, kUpb_ExtMode_Extendable, 0, UPB_FASTTABLE_MASK(248), 0,
+  UPB_SIZE(16, 24), 3, kUpb_ExtMode_Extendable, 0, UPB_FASTTABLE_MASK(248), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
+    {0x000800003f000012, &upb_prm_1bt_max64b},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -200,23 +205,47 @@
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
+    {0x001000003f023eba, &upb_prm_2bt_max128b},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x000000003f003eba, &upb_prm_2bt_max128b},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
+  })
+};
+
+static const upb_MiniTableField google_protobuf_ExtensionRangeOptions_Declaration__fields[6] = {
+  {1, 4, 1, kUpb_NoSub, 5, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
+  {2, UPB_SIZE(12, 16), 2, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)},
+  {3, UPB_SIZE(20, 32), 3, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)},
+  {4, 8, 4, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
+  {5, 9, 5, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
+  {6, 10, 6, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
+};
+
+const upb_MiniTable google_protobuf_ExtensionRangeOptions_Declaration_msg_init = {
+  NULL,
+  &google_protobuf_ExtensionRangeOptions_Declaration__fields[0],
+  UPB_SIZE(32, 48), 6, kUpb_ExtMode_NonExtendable, 6, UPB_FASTTABLE_MASK(56), 0,
+  UPB_FASTTABLE_INIT({
+    {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
+    {0x0004000001000008, &upb_psv4_1bt},
+    {0x0010000002000012, &upb_pss_1bt},
+    {0x002000000300001a, &upb_pss_1bt},
+    {0x0008000004000020, &upb_psb1_1bt},
+    {0x0009000005000028, &upb_psb1_1bt},
+    {0x000a000006000030, &upb_psb1_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
 
 static const upb_MiniTableSub google_protobuf_FieldDescriptorProto_submsgs[3] = {
   {.subenum = &google_protobuf_FieldDescriptorProto_Label_enum_init},
   {.subenum = &google_protobuf_FieldDescriptorProto_Type_enum_init},
@@ -239,24 +268,24 @@
 
 const upb_MiniTable google_protobuf_FieldDescriptorProto_msg_init = {
   &google_protobuf_FieldDescriptorProto_submsgs[0],
   &google_protobuf_FieldDescriptorProto__fields[0],
   UPB_SIZE(72, 112), 11, kUpb_ExtMode_NonExtendable, 10, UPB_FASTTABLE_MASK(248), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x001800000100000a, &upb_psb_1bt},
-    {0x0028000002000012, &upb_psb_1bt},
+    {0x001800000100000a, &upb_pss_1bt},
+    {0x0028000002000012, &upb_pss_1bt},
     {0x0004000003000018, &upb_psv4_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x0038000006000032, &upb_psb_1bt},
-    {0x004800000700003a, &upb_psb_1bt},
+    {0x0038000006000032, &upb_pss_1bt},
+    {0x004800000700003a, &upb_pss_1bt},
     {0x0058000008020042, &upb_psm_1bt_max64b},
     {0x0010000009000048, &upb_psv4_1bt},
-    {0x006000000a000052, &upb_psb_1bt},
+    {0x006000000a000052, &upb_pss_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x001400000b000188, &upb_psb1_2bt},
@@ -288,15 +317,15 @@
 
 const upb_MiniTable google_protobuf_OneofDescriptorProto_msg_init = {
   &google_protobuf_OneofDescriptorProto_submsgs[0],
   &google_protobuf_OneofDescriptorProto__fields[0],
   UPB_SIZE(16, 32), 2, kUpb_ExtMode_NonExtendable, 2, UPB_FASTTABLE_MASK(24), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x000800000100000a, &upb_psb_1bt},
+    {0x000800000100000a, &upb_pss_1bt},
     {0x0018000002000012, &upb_psm_1bt_max64b},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
 
 static const upb_MiniTableSub google_protobuf_EnumDescriptorProto_submsgs[3] = {
   {.submsg = &google_protobuf_EnumValueDescriptorProto_msg_init},
@@ -314,19 +343,19 @@
 
 const upb_MiniTable google_protobuf_EnumDescriptorProto_msg_init = {
   &google_protobuf_EnumDescriptorProto_submsgs[0],
   &google_protobuf_EnumDescriptorProto__fields[0],
   UPB_SIZE(32, 56), 5, kUpb_ExtMode_NonExtendable, 5, UPB_FASTTABLE_MASK(56), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x000800000100000a, &upb_psb_1bt},
+    {0x000800000100000a, &upb_pss_1bt},
     {0x001800003f000012, &upb_prm_1bt_max64b},
     {0x002000000201001a, &upb_psm_1bt_max64b},
     {0x002800003f020022, &upb_prm_1bt_max64b},
-    {0x003000003f00002a, &upb_prb_1bt},
+    {0x003000003f00002a, &upb_prs_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
 
 static const upb_MiniTableField google_protobuf_EnumDescriptorProto_EnumReservedRange__fields[2] = {
   {1, 4, 1, kUpb_NoSub, 5, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
@@ -357,15 +386,15 @@
 
 const upb_MiniTable google_protobuf_EnumValueDescriptorProto_msg_init = {
   &google_protobuf_EnumValueDescriptorProto_submsgs[0],
   &google_protobuf_EnumValueDescriptorProto__fields[0],
   UPB_SIZE(24, 32), 3, kUpb_ExtMode_NonExtendable, 3, UPB_FASTTABLE_MASK(24), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x000800000100000a, &upb_psb_1bt},
+    {0x000800000100000a, &upb_pss_1bt},
     {0x0004000002000010, &upb_psv4_1bt},
     {0x001800000300001a, &upb_psm_1bt_max64b},
   })
 };
 
 static const upb_MiniTableSub google_protobuf_ServiceDescriptorProto_submsgs[2] = {
   {.submsg = &google_protobuf_MethodDescriptorProto_msg_init},
@@ -380,15 +409,15 @@
 
 const upb_MiniTable google_protobuf_ServiceDescriptorProto_msg_init = {
   &google_protobuf_ServiceDescriptorProto_submsgs[0],
   &google_protobuf_ServiceDescriptorProto__fields[0],
   UPB_SIZE(24, 40), 3, kUpb_ExtMode_NonExtendable, 3, UPB_FASTTABLE_MASK(24), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x000800000100000a, &upb_psb_1bt},
+    {0x000800000100000a, &upb_pss_1bt},
     {0x001800003f000012, &upb_prm_1bt_max128b},
     {0x002000000201001a, &upb_psm_1bt_max64b},
   })
 };
 
 static const upb_MiniTableSub google_protobuf_MethodDescriptorProto_submsgs[1] = {
   {.submsg = &google_protobuf_MethodOptions_msg_init},
@@ -405,17 +434,17 @@
 
 const upb_MiniTable google_protobuf_MethodDescriptorProto_msg_init = {
   &google_protobuf_MethodDescriptorProto_submsgs[0],
   &google_protobuf_MethodDescriptorProto__fields[0],
   UPB_SIZE(40, 64), 6, kUpb_ExtMode_NonExtendable, 6, UPB_FASTTABLE_MASK(56), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x000800000100000a, &upb_psb_1bt},
-    {0x0018000002000012, &upb_psb_1bt},
-    {0x002800000300001a, &upb_psb_1bt},
+    {0x000800000100000a, &upb_pss_1bt},
+    {0x0018000002000012, &upb_pss_1bt},
+    {0x002800000300001a, &upb_pss_1bt},
     {0x0038000004000022, &upb_psm_1bt_max64b},
     {0x0001000005000028, &upb_psb1_1bt},
     {0x0002000006000030, &upb_psb1_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
 
@@ -450,43 +479,43 @@
 
 const upb_MiniTable google_protobuf_FileOptions_msg_init = {
   &google_protobuf_FileOptions_submsgs[0],
   &google_protobuf_FileOptions__fields[0],
   UPB_SIZE(104, 192), 21, kUpb_ExtMode_Extendable, 1, UPB_FASTTABLE_MASK(248), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x001800000100000a, &upb_psb_1bt},
+    {0x001800000100000a, &upb_pss_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x0028000002000042, &upb_psb_1bt},
+    {0x0028000002000042, &upb_pss_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0008000004000050, &upb_psb1_1bt},
-    {0x003800000500005a, &upb_psb_1bt},
+    {0x003800000500005a, &upb_pss_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0009000006000180, &upb_psb1_2bt},
     {0x000a000007000188, &upb_psb1_2bt},
     {0x000b000008000190, &upb_psb1_2bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x000c0000090001a0, &upb_psb1_2bt},
-    {0x005800000e0002aa, &upb_psb_2bt},
+    {0x005800000e0002aa, &upb_pss_2bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x000d00000a0001b8, &upb_psb1_2bt},
-    {0x00780000100002c2, &upb_psb_2bt},
-    {0x00880000110002ca, &upb_psb_2bt},
+    {0x00780000100002c2, &upb_pss_2bt},
+    {0x00880000110002ca, &upb_pss_2bt},
     {0x00100000120002d0, &upb_psb1_2bt},
     {0x000e00000b0001d8, &upb_psb1_2bt},
-    {0x00980000130002e2, &upb_psb_2bt},
-    {0x00a80000140002ea, &upb_psb_2bt},
+    {0x00980000130002e2, &upb_pss_2bt},
+    {0x00a80000140002ea, &upb_pss_2bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x000f00000c0001f8, &upb_psb1_2bt},
   })
 };
 
 static const upb_MiniTableSub google_protobuf_MessageOptions_submsgs[1] = {
   {.submsg = &google_protobuf_UninterpretedOption_msg_init},
@@ -537,40 +566,42 @@
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
 
-static const upb_MiniTableSub google_protobuf_FieldOptions_submsgs[5] = {
+static const upb_MiniTableSub google_protobuf_FieldOptions_submsgs[6] = {
   {.subenum = &google_protobuf_FieldOptions_CType_enum_init},
   {.subenum = &google_protobuf_FieldOptions_JSType_enum_init},
   {.subenum = &google_protobuf_FieldOptions_OptionRetention_enum_init},
   {.subenum = &google_protobuf_FieldOptions_OptionTargetType_enum_init},
+  {.subenum = &google_protobuf_FieldOptions_OptionTargetType_enum_init},
   {.submsg = &google_protobuf_UninterpretedOption_msg_init},
 };
 
-static const upb_MiniTableField google_protobuf_FieldOptions__fields[11] = {
+static const upb_MiniTableField google_protobuf_FieldOptions__fields[12] = {
   {1, 4, 1, 0, 14, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
   {2, 8, 2, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
   {3, 9, 3, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
   {5, 10, 4, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
   {6, 12, 5, 1, 14, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
   {10, 16, 6, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
   {15, 17, 7, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
   {16, 18, 8, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)},
   {17, 20, 9, 2, 14, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
   {18, 24, 10, 3, 14, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)},
-  {999, UPB_SIZE(28, 32), 0, 4, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
+  {19, UPB_SIZE(28, 32), 0, 4, 14, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
+  {999, UPB_SIZE(32, 40), 0, 5, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)},
 };
 
 const upb_MiniTable google_protobuf_FieldOptions_msg_init = {
   &google_protobuf_FieldOptions_submsgs[0],
   &google_protobuf_FieldOptions__fields[0],
-  UPB_SIZE(32, 40), 11, kUpb_ExtMode_Extendable, 3, UPB_FASTTABLE_MASK(248), 0,
+  UPB_SIZE(40, 48), 12, kUpb_ExtMode_Extendable, 3, UPB_FASTTABLE_MASK(248), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0008000002000010, &upb_psb1_1bt},
     {0x0009000003000018, &upb_psb1_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x000a000004000028, &upb_psb1_1bt},
@@ -587,15 +618,15 @@
     {0x0012000008000180, &upb_psb1_2bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x002000003f043eba, &upb_prm_2bt_max128b},
+    {0x002800003f053eba, &upb_prm_2bt_max128b},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -869,20 +900,20 @@
   &google_protobuf_UninterpretedOption_submsgs[0],
   &google_protobuf_UninterpretedOption__fields[0],
   UPB_SIZE(56, 88), 7, kUpb_ExtMode_NonExtendable, 0, UPB_FASTTABLE_MASK(120), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x000800003f000012, &upb_prm_1bt_max64b},
-    {0x001000000100001a, &upb_psb_1bt},
+    {0x001000000100001a, &upb_pss_1bt},
     {0x0020000002000020, &upb_psv8_1bt},
     {0x0028000003000028, &upb_psv8_1bt},
     {0x0030000004000031, &upb_psf8_1bt},
     {0x003800000500003a, &upb_psb_1bt},
-    {0x0048000006000042, &upb_psb_1bt},
+    {0x0048000006000042, &upb_pss_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
@@ -896,15 +927,15 @@
 
 const upb_MiniTable google_protobuf_UninterpretedOption_NamePart_msg_init = {
   NULL,
   &google_protobuf_UninterpretedOption_NamePart__fields[0],
   UPB_SIZE(16, 24), 2, kUpb_ExtMode_NonExtendable, 2, UPB_FASTTABLE_MASK(24), 2,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x000800000100000a, &upb_psb_1bt},
+    {0x000800000100000a, &upb_pss_1bt},
     {0x0001000002000010, &upb_psb1_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
 
 static const upb_MiniTableSub google_protobuf_SourceCodeInfo_submsgs[1] = {
   {.submsg = &google_protobuf_SourceCodeInfo_Location_msg_init},
@@ -936,18 +967,18 @@
   NULL,
   &google_protobuf_SourceCodeInfo_Location__fields[0],
   UPB_SIZE(32, 64), 5, kUpb_ExtMode_NonExtendable, 4, UPB_FASTTABLE_MASK(56), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x000800003f00000a, &upb_ppv4_1bt},
     {0x001000003f000012, &upb_ppv4_1bt},
-    {0x001800000100001a, &upb_psb_1bt},
-    {0x0028000002000022, &upb_psb_1bt},
+    {0x001800000100001a, &upb_pss_1bt},
+    {0x0028000002000022, &upb_pss_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
-    {0x003800003f000032, &upb_prb_1bt},
+    {0x003800003f000032, &upb_prs_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
 
 static const upb_MiniTableSub google_protobuf_GeneratedCodeInfo_submsgs[1] = {
   {.submsg = &google_protobuf_GeneratedCodeInfo_Annotation_msg_init},
 };
@@ -981,30 +1012,31 @@
 const upb_MiniTable google_protobuf_GeneratedCodeInfo_Annotation_msg_init = {
   &google_protobuf_GeneratedCodeInfo_Annotation_submsgs[0],
   &google_protobuf_GeneratedCodeInfo_Annotation__fields[0],
   UPB_SIZE(32, 40), 5, kUpb_ExtMode_NonExtendable, 5, UPB_FASTTABLE_MASK(56), 0,
   UPB_FASTTABLE_INIT({
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x001000003f00000a, &upb_ppv4_1bt},
-    {0x0018000001000012, &upb_psb_1bt},
+    {0x0018000001000012, &upb_pss_1bt},
     {0x0004000002000018, &upb_psv4_1bt},
     {0x0008000003000020, &upb_psv4_1bt},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
     {0x0000000000000000, &_upb_FastDecoder_DecodeGeneric},
   })
 };
 
-static const upb_MiniTable *messages_layout[27] = {
+static const upb_MiniTable *messages_layout[28] = {
   &google_protobuf_FileDescriptorSet_msg_init,
   &google_protobuf_FileDescriptorProto_msg_init,
   &google_protobuf_DescriptorProto_msg_init,
   &google_protobuf_DescriptorProto_ExtensionRange_msg_init,
   &google_protobuf_DescriptorProto_ReservedRange_msg_init,
   &google_protobuf_ExtensionRangeOptions_msg_init,
+  &google_protobuf_ExtensionRangeOptions_Declaration_msg_init,
   &google_protobuf_FieldDescriptorProto_msg_init,
   &google_protobuf_OneofDescriptorProto_msg_init,
   &google_protobuf_EnumDescriptorProto_msg_init,
   &google_protobuf_EnumDescriptorProto_EnumReservedRange_msg_init,
   &google_protobuf_EnumValueDescriptorProto_msg_init,
   &google_protobuf_ServiceDescriptorProto_msg_init,
   &google_protobuf_MethodDescriptorProto_msg_init,
@@ -1020,14 +1052,23 @@
   &google_protobuf_UninterpretedOption_NamePart_msg_init,
   &google_protobuf_SourceCodeInfo_msg_init,
   &google_protobuf_SourceCodeInfo_Location_msg_init,
   &google_protobuf_GeneratedCodeInfo_msg_init,
   &google_protobuf_GeneratedCodeInfo_Annotation_msg_init,
 };
 
+const upb_MiniTableEnum google_protobuf_ExtensionRangeOptions_VerificationState_enum_init = {
+    64,
+    0,
+    {
+        0x3,
+        0x0,
+    },
+};
+
 const upb_MiniTableEnum google_protobuf_FieldDescriptorProto_Label_enum_init = {
     64,
     0,
     {
         0xe,
         0x0,
     },
@@ -1101,15 +1142,16 @@
     0,
     {
         0x7,
         0x0,
     },
 };
 
-static const upb_MiniTableEnum *enums_layout[9] = {
+static const upb_MiniTableEnum *enums_layout[10] = {
+  &google_protobuf_ExtensionRangeOptions_VerificationState_enum_init,
   &google_protobuf_FieldDescriptorProto_Label_enum_init,
   &google_protobuf_FieldDescriptorProto_Type_enum_init,
   &google_protobuf_FieldOptions_CType_enum_init,
   &google_protobuf_FieldOptions_JSType_enum_init,
   &google_protobuf_FieldOptions_OptionRetention_enum_init,
   &google_protobuf_FieldOptions_OptionTargetType_enum_init,
   &google_protobuf_FileOptions_OptimizeMode_enum_init,
@@ -1117,14 +1159,14 @@
   &google_protobuf_MethodOptions_IdempotencyLevel_enum_init,
 };
 
 const upb_MiniTableFile google_protobuf_descriptor_proto_upb_file_layout = {
   messages_layout,
   enums_layout,
   NULL,
-  27,
-  9,
+  28,
+  10,
   0,
 };
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-4.22.3/google/protobuf/descriptor.upb.h` & `protobuf-4.23.0rc2/google/protobuf/descriptor.upb.h`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 typedef struct google_protobuf_FileDescriptorSet google_protobuf_FileDescriptorSet;
 typedef struct google_protobuf_FileDescriptorProto google_protobuf_FileDescriptorProto;
 typedef struct google_protobuf_DescriptorProto google_protobuf_DescriptorProto;
 typedef struct google_protobuf_DescriptorProto_ExtensionRange google_protobuf_DescriptorProto_ExtensionRange;
 typedef struct google_protobuf_DescriptorProto_ReservedRange google_protobuf_DescriptorProto_ReservedRange;
 typedef struct google_protobuf_ExtensionRangeOptions google_protobuf_ExtensionRangeOptions;
+typedef struct google_protobuf_ExtensionRangeOptions_Declaration google_protobuf_ExtensionRangeOptions_Declaration;
 typedef struct google_protobuf_FieldDescriptorProto google_protobuf_FieldDescriptorProto;
 typedef struct google_protobuf_OneofDescriptorProto google_protobuf_OneofDescriptorProto;
 typedef struct google_protobuf_EnumDescriptorProto google_protobuf_EnumDescriptorProto;
 typedef struct google_protobuf_EnumDescriptorProto_EnumReservedRange google_protobuf_EnumDescriptorProto_EnumReservedRange;
 typedef struct google_protobuf_EnumValueDescriptorProto google_protobuf_EnumValueDescriptorProto;
 typedef struct google_protobuf_ServiceDescriptorProto google_protobuf_ServiceDescriptorProto;
 typedef struct google_protobuf_MethodDescriptorProto google_protobuf_MethodDescriptorProto;
@@ -54,14 +55,15 @@
 typedef struct google_protobuf_GeneratedCodeInfo_Annotation google_protobuf_GeneratedCodeInfo_Annotation;
 extern const upb_MiniTable google_protobuf_FileDescriptorSet_msg_init;
 extern const upb_MiniTable google_protobuf_FileDescriptorProto_msg_init;
 extern const upb_MiniTable google_protobuf_DescriptorProto_msg_init;
 extern const upb_MiniTable google_protobuf_DescriptorProto_ExtensionRange_msg_init;
 extern const upb_MiniTable google_protobuf_DescriptorProto_ReservedRange_msg_init;
 extern const upb_MiniTable google_protobuf_ExtensionRangeOptions_msg_init;
+extern const upb_MiniTable google_protobuf_ExtensionRangeOptions_Declaration_msg_init;
 extern const upb_MiniTable google_protobuf_FieldDescriptorProto_msg_init;
 extern const upb_MiniTable google_protobuf_OneofDescriptorProto_msg_init;
 extern const upb_MiniTable google_protobuf_EnumDescriptorProto_msg_init;
 extern const upb_MiniTable google_protobuf_EnumDescriptorProto_EnumReservedRange_msg_init;
 extern const upb_MiniTable google_protobuf_EnumValueDescriptorProto_msg_init;
 extern const upb_MiniTable google_protobuf_ServiceDescriptorProto_msg_init;
 extern const upb_MiniTable google_protobuf_MethodDescriptorProto_msg_init;
@@ -77,14 +79,19 @@
 extern const upb_MiniTable google_protobuf_UninterpretedOption_NamePart_msg_init;
 extern const upb_MiniTable google_protobuf_SourceCodeInfo_msg_init;
 extern const upb_MiniTable google_protobuf_SourceCodeInfo_Location_msg_init;
 extern const upb_MiniTable google_protobuf_GeneratedCodeInfo_msg_init;
 extern const upb_MiniTable google_protobuf_GeneratedCodeInfo_Annotation_msg_init;
 
 typedef enum {
+  google_protobuf_ExtensionRangeOptions_DECLARATION = 0,
+  google_protobuf_ExtensionRangeOptions_UNVERIFIED = 1
+} google_protobuf_ExtensionRangeOptions_VerificationState;
+
+typedef enum {
   google_protobuf_FieldDescriptorProto_LABEL_OPTIONAL = 1,
   google_protobuf_FieldDescriptorProto_LABEL_REQUIRED = 2,
   google_protobuf_FieldDescriptorProto_LABEL_REPEATED = 3
 } google_protobuf_FieldDescriptorProto_Label;
 
 typedef enum {
   google_protobuf_FieldDescriptorProto_TYPE_DOUBLE = 1,
@@ -153,14 +160,15 @@
 typedef enum {
   google_protobuf_MethodOptions_IDEMPOTENCY_UNKNOWN = 0,
   google_protobuf_MethodOptions_NO_SIDE_EFFECTS = 1,
   google_protobuf_MethodOptions_IDEMPOTENT = 2
 } google_protobuf_MethodOptions_IdempotencyLevel;
 
 
+extern const upb_MiniTableEnum google_protobuf_ExtensionRangeOptions_VerificationState_enum_init;
 extern const upb_MiniTableEnum google_protobuf_FieldDescriptorProto_Label_enum_init;
 extern const upb_MiniTableEnum google_protobuf_FieldDescriptorProto_Type_enum_init;
 extern const upb_MiniTableEnum google_protobuf_FieldOptions_CType_enum_init;
 extern const upb_MiniTableEnum google_protobuf_FieldOptions_JSType_enum_init;
 extern const upb_MiniTableEnum google_protobuf_FieldOptions_OptionRetention_enum_init;
 extern const upb_MiniTableEnum google_protobuf_FieldOptions_OptionTargetType_enum_init;
 extern const upb_MiniTableEnum google_protobuf_FileOptions_OptimizeMode_enum_init;
@@ -213,14 +221,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_FileDescriptorProto* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_FileDescriptorSet_file_upb_array(const google_protobuf_FileDescriptorSet* msg, size_t* size) {
+  const upb_MiniTableField field = {1, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_FileDescriptorSet_file_mutable_upb_array(const google_protobuf_FileDescriptorSet* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {1, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_FileDescriptorSet_has_file(const google_protobuf_FileDescriptorSet* msg) {
   size_t size;
   google_protobuf_FileDescriptorSet_file(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE google_protobuf_FileDescriptorProto** google_protobuf_FileDescriptorSet_mutable_file(google_protobuf_FileDescriptorSet* msg, size_t* size) {
@@ -326,14 +351,31 @@
     if (size) *size = arr->size;
     return (upb_StringView const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_FileDescriptorProto_dependency_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {3, UPB_SIZE(4, 40), 0, kUpb_NoSub, 12, kUpb_FieldMode_Array | kUpb_LabelFlags_IsAlternate | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_FileDescriptorProto_dependency_mutable_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {3, UPB_SIZE(4, 40), 0, kUpb_NoSub, 12, kUpb_FieldMode_Array | kUpb_LabelFlags_IsAlternate | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_FileDescriptorProto_has_dependency(const google_protobuf_FileDescriptorProto* msg) {
   size_t size;
   google_protobuf_FileDescriptorProto_dependency(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_FileDescriptorProto_clear_message_type(google_protobuf_FileDescriptorProto* msg) {
   const upb_MiniTableField field = {4, UPB_SIZE(8, 48), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -346,14 +388,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_DescriptorProto* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_FileDescriptorProto_message_type_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {4, UPB_SIZE(8, 48), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_FileDescriptorProto_message_type_mutable_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {4, UPB_SIZE(8, 48), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_FileDescriptorProto_has_message_type(const google_protobuf_FileDescriptorProto* msg) {
   size_t size;
   google_protobuf_FileDescriptorProto_message_type(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_FileDescriptorProto_clear_enum_type(google_protobuf_FileDescriptorProto* msg) {
   const upb_MiniTableField field = {5, UPB_SIZE(12, 56), 0, 1, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -366,14 +425,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_EnumDescriptorProto* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_FileDescriptorProto_enum_type_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {5, UPB_SIZE(12, 56), 0, 1, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_FileDescriptorProto_enum_type_mutable_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {5, UPB_SIZE(12, 56), 0, 1, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_FileDescriptorProto_has_enum_type(const google_protobuf_FileDescriptorProto* msg) {
   size_t size;
   google_protobuf_FileDescriptorProto_enum_type(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_FileDescriptorProto_clear_service(google_protobuf_FileDescriptorProto* msg) {
   const upb_MiniTableField field = {6, UPB_SIZE(16, 64), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -386,14 +462,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_ServiceDescriptorProto* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_FileDescriptorProto_service_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {6, UPB_SIZE(16, 64), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_FileDescriptorProto_service_mutable_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {6, UPB_SIZE(16, 64), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_FileDescriptorProto_has_service(const google_protobuf_FileDescriptorProto* msg) {
   size_t size;
   google_protobuf_FileDescriptorProto_service(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_FileDescriptorProto_clear_extension(google_protobuf_FileDescriptorProto* msg) {
   const upb_MiniTableField field = {7, UPB_SIZE(20, 72), 0, 3, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -406,14 +499,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_FieldDescriptorProto* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_FileDescriptorProto_extension_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {7, UPB_SIZE(20, 72), 0, 3, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_FileDescriptorProto_extension_mutable_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {7, UPB_SIZE(20, 72), 0, 3, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_FileDescriptorProto_has_extension(const google_protobuf_FileDescriptorProto* msg) {
   size_t size;
   google_protobuf_FileDescriptorProto_extension(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_FileDescriptorProto_clear_options(google_protobuf_FileDescriptorProto* msg) {
   const upb_MiniTableField field = {8, UPB_SIZE(24, 80), 3, 4, 11, kUpb_FieldMode_Scalar | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -456,14 +566,31 @@
     if (size) *size = arr->size;
     return (int32_t const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_FileDescriptorProto_public_dependency_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {10, UPB_SIZE(32, 96), 0, kUpb_NoSub, 5, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_FileDescriptorProto_public_dependency_mutable_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {10, UPB_SIZE(32, 96), 0, kUpb_NoSub, 5, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_FileDescriptorProto_has_public_dependency(const google_protobuf_FileDescriptorProto* msg) {
   size_t size;
   google_protobuf_FileDescriptorProto_public_dependency(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_FileDescriptorProto_clear_weak_dependency(google_protobuf_FileDescriptorProto* msg) {
   const upb_MiniTableField field = {11, UPB_SIZE(36, 104), 0, kUpb_NoSub, 5, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -476,14 +603,31 @@
     if (size) *size = arr->size;
     return (int32_t const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_FileDescriptorProto_weak_dependency_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {11, UPB_SIZE(36, 104), 0, kUpb_NoSub, 5, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_FileDescriptorProto_weak_dependency_mutable_upb_array(const google_protobuf_FileDescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {11, UPB_SIZE(36, 104), 0, kUpb_NoSub, 5, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_FileDescriptorProto_has_weak_dependency(const google_protobuf_FileDescriptorProto* msg) {
   size_t size;
   google_protobuf_FileDescriptorProto_weak_dependency(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_FileDescriptorProto_clear_syntax(google_protobuf_FileDescriptorProto* msg) {
   const upb_MiniTableField field = {12, UPB_SIZE(56, 112), 5, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
@@ -794,14 +938,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_FieldDescriptorProto* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_DescriptorProto_field_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {2, UPB_SIZE(4, 24), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_DescriptorProto_field_mutable_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {2, UPB_SIZE(4, 24), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_DescriptorProto_has_field(const google_protobuf_DescriptorProto* msg) {
   size_t size;
   google_protobuf_DescriptorProto_field(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_DescriptorProto_clear_nested_type(google_protobuf_DescriptorProto* msg) {
   const upb_MiniTableField field = {3, UPB_SIZE(8, 32), 0, 1, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -814,14 +975,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_DescriptorProto* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_DescriptorProto_nested_type_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {3, UPB_SIZE(8, 32), 0, 1, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_DescriptorProto_nested_type_mutable_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {3, UPB_SIZE(8, 32), 0, 1, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_DescriptorProto_has_nested_type(const google_protobuf_DescriptorProto* msg) {
   size_t size;
   google_protobuf_DescriptorProto_nested_type(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_DescriptorProto_clear_enum_type(google_protobuf_DescriptorProto* msg) {
   const upb_MiniTableField field = {4, UPB_SIZE(12, 40), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -834,14 +1012,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_EnumDescriptorProto* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_DescriptorProto_enum_type_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {4, UPB_SIZE(12, 40), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_DescriptorProto_enum_type_mutable_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {4, UPB_SIZE(12, 40), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_DescriptorProto_has_enum_type(const google_protobuf_DescriptorProto* msg) {
   size_t size;
   google_protobuf_DescriptorProto_enum_type(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_DescriptorProto_clear_extension_range(google_protobuf_DescriptorProto* msg) {
   const upb_MiniTableField field = {5, UPB_SIZE(16, 48), 0, 3, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -854,14 +1049,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_DescriptorProto_ExtensionRange* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_DescriptorProto_extension_range_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {5, UPB_SIZE(16, 48), 0, 3, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_DescriptorProto_extension_range_mutable_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {5, UPB_SIZE(16, 48), 0, 3, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_DescriptorProto_has_extension_range(const google_protobuf_DescriptorProto* msg) {
   size_t size;
   google_protobuf_DescriptorProto_extension_range(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_DescriptorProto_clear_extension(google_protobuf_DescriptorProto* msg) {
   const upb_MiniTableField field = {6, UPB_SIZE(20, 56), 0, 4, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -874,14 +1086,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_FieldDescriptorProto* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_DescriptorProto_extension_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {6, UPB_SIZE(20, 56), 0, 4, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_DescriptorProto_extension_mutable_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {6, UPB_SIZE(20, 56), 0, 4, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_DescriptorProto_has_extension(const google_protobuf_DescriptorProto* msg) {
   size_t size;
   google_protobuf_DescriptorProto_extension(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_DescriptorProto_clear_options(google_protobuf_DescriptorProto* msg) {
   const upb_MiniTableField field = {7, UPB_SIZE(24, 64), 2, 5, 11, kUpb_FieldMode_Scalar | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -909,14 +1138,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_OneofDescriptorProto* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_DescriptorProto_oneof_decl_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {8, UPB_SIZE(28, 72), 0, 6, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_DescriptorProto_oneof_decl_mutable_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {8, UPB_SIZE(28, 72), 0, 6, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_DescriptorProto_has_oneof_decl(const google_protobuf_DescriptorProto* msg) {
   size_t size;
   google_protobuf_DescriptorProto_oneof_decl(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_DescriptorProto_clear_reserved_range(google_protobuf_DescriptorProto* msg) {
   const upb_MiniTableField field = {9, UPB_SIZE(32, 80), 0, 7, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -929,14 +1175,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_DescriptorProto_ReservedRange* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_DescriptorProto_reserved_range_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {9, UPB_SIZE(32, 80), 0, 7, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_DescriptorProto_reserved_range_mutable_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {9, UPB_SIZE(32, 80), 0, 7, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_DescriptorProto_has_reserved_range(const google_protobuf_DescriptorProto* msg) {
   size_t size;
   google_protobuf_DescriptorProto_reserved_range(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_DescriptorProto_clear_reserved_name(google_protobuf_DescriptorProto* msg) {
   const upb_MiniTableField field = {10, UPB_SIZE(36, 88), 0, kUpb_NoSub, 12, kUpb_FieldMode_Array | kUpb_LabelFlags_IsAlternate | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -949,14 +1212,31 @@
     if (size) *size = arr->size;
     return (upb_StringView const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_DescriptorProto_reserved_name_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {10, UPB_SIZE(36, 88), 0, kUpb_NoSub, 12, kUpb_FieldMode_Array | kUpb_LabelFlags_IsAlternate | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_DescriptorProto_reserved_name_mutable_upb_array(const google_protobuf_DescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {10, UPB_SIZE(36, 88), 0, kUpb_NoSub, 12, kUpb_FieldMode_Array | kUpb_LabelFlags_IsAlternate | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_DescriptorProto_has_reserved_name(const google_protobuf_DescriptorProto* msg) {
   size_t size;
   google_protobuf_DescriptorProto_reserved_name(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE void google_protobuf_DescriptorProto_set_name(google_protobuf_DescriptorProto *msg, upb_StringView value) {
@@ -1390,62 +1670,312 @@
 }
 UPB_INLINE char* google_protobuf_ExtensionRangeOptions_serialize_ex(const google_protobuf_ExtensionRangeOptions* msg, int options,
                                  upb_Arena* arena, size_t* len) {
   char* ptr;
   (void)upb_Encode(msg, &google_protobuf_ExtensionRangeOptions_msg_init, options, arena, &ptr, len);
   return ptr;
 }
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_clear_declaration(google_protobuf_ExtensionRangeOptions* msg) {
+  const upb_MiniTableField field = {2, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  _upb_Message_ClearNonExtensionField(msg, &field);
+}
+UPB_INLINE const google_protobuf_ExtensionRangeOptions_Declaration* const* google_protobuf_ExtensionRangeOptions_declaration(const google_protobuf_ExtensionRangeOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {2, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (arr) {
+    if (size) *size = arr->size;
+    return (const google_protobuf_ExtensionRangeOptions_Declaration* const*)_upb_array_constptr(arr);
+  } else {
+    if (size) *size = 0;
+    return NULL;
+  }
+}
+UPB_INLINE const upb_Array* _google_protobuf_ExtensionRangeOptions_declaration_upb_array(const google_protobuf_ExtensionRangeOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {2, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_ExtensionRangeOptions_declaration_mutable_upb_array(const google_protobuf_ExtensionRangeOptions* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {2, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE bool google_protobuf_ExtensionRangeOptions_has_declaration(const google_protobuf_ExtensionRangeOptions* msg) {
+  size_t size;
+  google_protobuf_ExtensionRangeOptions_declaration(msg, &size);
+  return size != 0;
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_clear_verification(google_protobuf_ExtensionRangeOptions* msg) {
+  const upb_MiniTableField field = {3, UPB_SIZE(8, 4), 1, 1, 14, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_ClearNonExtensionField(msg, &field);
+}
+UPB_INLINE int32_t google_protobuf_ExtensionRangeOptions_verification(const google_protobuf_ExtensionRangeOptions* msg) {
+  int32_t default_val = 1;
+  int32_t ret;
+  const upb_MiniTableField field = {3, UPB_SIZE(8, 4), 1, 1, 14, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(msg, &field, &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_ExtensionRangeOptions_has_verification(const google_protobuf_ExtensionRangeOptions* msg) {
+  const upb_MiniTableField field = {3, UPB_SIZE(8, 4), 1, 1, 14, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  return _upb_Message_HasNonExtensionField(msg, &field);
+}
 UPB_INLINE void google_protobuf_ExtensionRangeOptions_clear_uninterpreted_option(google_protobuf_ExtensionRangeOptions* msg) {
-  const upb_MiniTableField field = {999, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {999, UPB_SIZE(12, 16), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   _upb_Message_ClearNonExtensionField(msg, &field);
 }
 UPB_INLINE const google_protobuf_UninterpretedOption* const* google_protobuf_ExtensionRangeOptions_uninterpreted_option(const google_protobuf_ExtensionRangeOptions* msg, size_t* size) {
-  const upb_MiniTableField field = {999, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {999, UPB_SIZE(12, 16), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   const upb_Array* arr = upb_Message_GetArray(msg, &field);
   if (arr) {
     if (size) *size = arr->size;
     return (const google_protobuf_UninterpretedOption* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_ExtensionRangeOptions_uninterpreted_option_upb_array(const google_protobuf_ExtensionRangeOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {999, UPB_SIZE(12, 16), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_ExtensionRangeOptions_uninterpreted_option_mutable_upb_array(const google_protobuf_ExtensionRangeOptions* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {999, UPB_SIZE(12, 16), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_ExtensionRangeOptions_has_uninterpreted_option(const google_protobuf_ExtensionRangeOptions* msg) {
   size_t size;
   google_protobuf_ExtensionRangeOptions_uninterpreted_option(msg, &size);
   return size != 0;
 }
 
+UPB_INLINE google_protobuf_ExtensionRangeOptions_Declaration** google_protobuf_ExtensionRangeOptions_mutable_declaration(google_protobuf_ExtensionRangeOptions* msg, size_t* size) {
+  upb_MiniTableField field = {2, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetMutableArray(msg, &field);
+  if (arr) {
+    if (size) *size = arr->size;
+    return (google_protobuf_ExtensionRangeOptions_Declaration**)_upb_array_ptr(arr);
+  } else {
+    if (size) *size = 0;
+    return NULL;
+  }
+}
+UPB_INLINE google_protobuf_ExtensionRangeOptions_Declaration** google_protobuf_ExtensionRangeOptions_resize_declaration(google_protobuf_ExtensionRangeOptions* msg, size_t size, upb_Arena* arena) {
+  upb_MiniTableField field = {2, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  return (google_protobuf_ExtensionRangeOptions_Declaration**)upb_Message_ResizeArray(msg, &field, size, arena);
+}
+UPB_INLINE struct google_protobuf_ExtensionRangeOptions_Declaration* google_protobuf_ExtensionRangeOptions_add_declaration(google_protobuf_ExtensionRangeOptions* msg, upb_Arena* arena) {
+  upb_MiniTableField field = {2, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(msg, &field, arena);
+  if (!arr || !_upb_Array_ResizeUninitialized(arr, arr->size + 1, arena)) {
+    return NULL;
+  }
+  struct google_protobuf_ExtensionRangeOptions_Declaration* sub = (struct google_protobuf_ExtensionRangeOptions_Declaration*)_upb_Message_New(&google_protobuf_ExtensionRangeOptions_Declaration_msg_init, arena);
+  if (!arr || !sub) return NULL;
+  _upb_Array_Set(arr, arr->size - 1, &sub, sizeof(sub));
+  return sub;
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_set_verification(google_protobuf_ExtensionRangeOptions *msg, int32_t value) {
+  const upb_MiniTableField field = {3, UPB_SIZE(8, 4), 1, 1, 14, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_SetNonExtensionField(msg, &field, &value);
+}
 UPB_INLINE google_protobuf_UninterpretedOption** google_protobuf_ExtensionRangeOptions_mutable_uninterpreted_option(google_protobuf_ExtensionRangeOptions* msg, size_t* size) {
-  upb_MiniTableField field = {999, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_MiniTableField field = {999, UPB_SIZE(12, 16), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetMutableArray(msg, &field);
   if (arr) {
     if (size) *size = arr->size;
     return (google_protobuf_UninterpretedOption**)_upb_array_ptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
 UPB_INLINE google_protobuf_UninterpretedOption** google_protobuf_ExtensionRangeOptions_resize_uninterpreted_option(google_protobuf_ExtensionRangeOptions* msg, size_t size, upb_Arena* arena) {
-  upb_MiniTableField field = {999, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_MiniTableField field = {999, UPB_SIZE(12, 16), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   return (google_protobuf_UninterpretedOption**)upb_Message_ResizeArray(msg, &field, size, arena);
 }
 UPB_INLINE struct google_protobuf_UninterpretedOption* google_protobuf_ExtensionRangeOptions_add_uninterpreted_option(google_protobuf_ExtensionRangeOptions* msg, upb_Arena* arena) {
-  upb_MiniTableField field = {999, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_MiniTableField field = {999, UPB_SIZE(12, 16), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetOrCreateMutableArray(msg, &field, arena);
   if (!arr || !_upb_Array_ResizeUninitialized(arr, arr->size + 1, arena)) {
     return NULL;
   }
   struct google_protobuf_UninterpretedOption* sub = (struct google_protobuf_UninterpretedOption*)_upb_Message_New(&google_protobuf_UninterpretedOption_msg_init, arena);
   if (!arr || !sub) return NULL;
   _upb_Array_Set(arr, arr->size - 1, &sub, sizeof(sub));
   return sub;
 }
 
+/* google.protobuf.ExtensionRangeOptions.Declaration */
+
+UPB_INLINE google_protobuf_ExtensionRangeOptions_Declaration* google_protobuf_ExtensionRangeOptions_Declaration_new(upb_Arena* arena) {
+  return (google_protobuf_ExtensionRangeOptions_Declaration*)_upb_Message_New(&google_protobuf_ExtensionRangeOptions_Declaration_msg_init, arena);
+}
+UPB_INLINE google_protobuf_ExtensionRangeOptions_Declaration* google_protobuf_ExtensionRangeOptions_Declaration_parse(const char* buf, size_t size, upb_Arena* arena) {
+  google_protobuf_ExtensionRangeOptions_Declaration* ret = google_protobuf_ExtensionRangeOptions_Declaration_new(arena);
+  if (!ret) return NULL;
+  if (upb_Decode(buf, size, ret, &google_protobuf_ExtensionRangeOptions_Declaration_msg_init, NULL, 0, arena) != kUpb_DecodeStatus_Ok) {
+    return NULL;
+  }
+  return ret;
+}
+UPB_INLINE google_protobuf_ExtensionRangeOptions_Declaration* google_protobuf_ExtensionRangeOptions_Declaration_parse_ex(const char* buf, size_t size,
+                           const upb_ExtensionRegistry* extreg,
+                           int options, upb_Arena* arena) {
+  google_protobuf_ExtensionRangeOptions_Declaration* ret = google_protobuf_ExtensionRangeOptions_Declaration_new(arena);
+  if (!ret) return NULL;
+  if (upb_Decode(buf, size, ret, &google_protobuf_ExtensionRangeOptions_Declaration_msg_init, extreg, options, arena) !=
+      kUpb_DecodeStatus_Ok) {
+    return NULL;
+  }
+  return ret;
+}
+UPB_INLINE char* google_protobuf_ExtensionRangeOptions_Declaration_serialize(const google_protobuf_ExtensionRangeOptions_Declaration* msg, upb_Arena* arena, size_t* len) {
+  char* ptr;
+  (void)upb_Encode(msg, &google_protobuf_ExtensionRangeOptions_Declaration_msg_init, 0, arena, &ptr, len);
+  return ptr;
+}
+UPB_INLINE char* google_protobuf_ExtensionRangeOptions_Declaration_serialize_ex(const google_protobuf_ExtensionRangeOptions_Declaration* msg, int options,
+                                 upb_Arena* arena, size_t* len) {
+  char* ptr;
+  (void)upb_Encode(msg, &google_protobuf_ExtensionRangeOptions_Declaration_msg_init, options, arena, &ptr, len);
+  return ptr;
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_clear_number(google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  const upb_MiniTableField field = {1, 4, 1, kUpb_NoSub, 5, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_ClearNonExtensionField(msg, &field);
+}
+UPB_INLINE int32_t google_protobuf_ExtensionRangeOptions_Declaration_number(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  int32_t default_val = (int32_t)0;
+  int32_t ret;
+  const upb_MiniTableField field = {1, 4, 1, kUpb_NoSub, 5, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(msg, &field, &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_ExtensionRangeOptions_Declaration_has_number(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  const upb_MiniTableField field = {1, 4, 1, kUpb_NoSub, 5, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  return _upb_Message_HasNonExtensionField(msg, &field);
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_clear_full_name(google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  const upb_MiniTableField field = {2, UPB_SIZE(12, 16), 2, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
+  _upb_Message_ClearNonExtensionField(msg, &field);
+}
+UPB_INLINE upb_StringView google_protobuf_ExtensionRangeOptions_Declaration_full_name(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  upb_StringView default_val = upb_StringView_FromString("");
+  upb_StringView ret;
+  const upb_MiniTableField field = {2, UPB_SIZE(12, 16), 2, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(msg, &field, &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_ExtensionRangeOptions_Declaration_has_full_name(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  const upb_MiniTableField field = {2, UPB_SIZE(12, 16), 2, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
+  return _upb_Message_HasNonExtensionField(msg, &field);
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_clear_type(google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  const upb_MiniTableField field = {3, UPB_SIZE(20, 32), 3, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
+  _upb_Message_ClearNonExtensionField(msg, &field);
+}
+UPB_INLINE upb_StringView google_protobuf_ExtensionRangeOptions_Declaration_type(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  upb_StringView default_val = upb_StringView_FromString("");
+  upb_StringView ret;
+  const upb_MiniTableField field = {3, UPB_SIZE(20, 32), 3, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(msg, &field, &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_ExtensionRangeOptions_Declaration_has_type(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  const upb_MiniTableField field = {3, UPB_SIZE(20, 32), 3, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
+  return _upb_Message_HasNonExtensionField(msg, &field);
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_clear_is_repeated(google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  const upb_MiniTableField field = {4, 8, 4, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_ClearNonExtensionField(msg, &field);
+}
+UPB_INLINE bool google_protobuf_ExtensionRangeOptions_Declaration_is_repeated(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  bool default_val = false;
+  bool ret;
+  const upb_MiniTableField field = {4, 8, 4, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(msg, &field, &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_ExtensionRangeOptions_Declaration_has_is_repeated(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  const upb_MiniTableField field = {4, 8, 4, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
+  return _upb_Message_HasNonExtensionField(msg, &field);
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_clear_reserved(google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  const upb_MiniTableField field = {5, 9, 5, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_ClearNonExtensionField(msg, &field);
+}
+UPB_INLINE bool google_protobuf_ExtensionRangeOptions_Declaration_reserved(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  bool default_val = false;
+  bool ret;
+  const upb_MiniTableField field = {5, 9, 5, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(msg, &field, &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_ExtensionRangeOptions_Declaration_has_reserved(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  const upb_MiniTableField field = {5, 9, 5, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
+  return _upb_Message_HasNonExtensionField(msg, &field);
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_clear_repeated(google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  const upb_MiniTableField field = {6, 10, 6, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_ClearNonExtensionField(msg, &field);
+}
+UPB_INLINE bool google_protobuf_ExtensionRangeOptions_Declaration_repeated(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  bool default_val = false;
+  bool ret;
+  const upb_MiniTableField field = {6, 10, 6, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_GetNonExtensionField(msg, &field, &default_val, &ret);
+  return ret;
+}
+UPB_INLINE bool google_protobuf_ExtensionRangeOptions_Declaration_has_repeated(const google_protobuf_ExtensionRangeOptions_Declaration* msg) {
+  const upb_MiniTableField field = {6, 10, 6, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
+  return _upb_Message_HasNonExtensionField(msg, &field);
+}
+
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_set_number(google_protobuf_ExtensionRangeOptions_Declaration *msg, int32_t value) {
+  const upb_MiniTableField field = {1, 4, 1, kUpb_NoSub, 5, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_SetNonExtensionField(msg, &field, &value);
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_set_full_name(google_protobuf_ExtensionRangeOptions_Declaration *msg, upb_StringView value) {
+  const upb_MiniTableField field = {2, UPB_SIZE(12, 16), 2, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
+  _upb_Message_SetNonExtensionField(msg, &field, &value);
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_set_type(google_protobuf_ExtensionRangeOptions_Declaration *msg, upb_StringView value) {
+  const upb_MiniTableField field = {3, UPB_SIZE(20, 32), 3, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
+  _upb_Message_SetNonExtensionField(msg, &field, &value);
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_set_is_repeated(google_protobuf_ExtensionRangeOptions_Declaration *msg, bool value) {
+  const upb_MiniTableField field = {4, 8, 4, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_SetNonExtensionField(msg, &field, &value);
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_set_reserved(google_protobuf_ExtensionRangeOptions_Declaration *msg, bool value) {
+  const upb_MiniTableField field = {5, 9, 5, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_SetNonExtensionField(msg, &field, &value);
+}
+UPB_INLINE void google_protobuf_ExtensionRangeOptions_Declaration_set_repeated(google_protobuf_ExtensionRangeOptions_Declaration *msg, bool value) {
+  const upb_MiniTableField field = {6, 10, 6, kUpb_NoSub, 8, kUpb_FieldMode_Scalar | (kUpb_FieldRep_1Byte << kUpb_FieldRep_Shift)};
+  _upb_Message_SetNonExtensionField(msg, &field, &value);
+}
+
 /* google.protobuf.FieldDescriptorProto */
 
 UPB_INLINE google_protobuf_FieldDescriptorProto* google_protobuf_FieldDescriptorProto_new(upb_Arena* arena) {
   return (google_protobuf_FieldDescriptorProto*)_upb_Message_New(&google_protobuf_FieldDescriptorProto_msg_init, arena);
 }
 UPB_INLINE google_protobuf_FieldDescriptorProto* google_protobuf_FieldDescriptorProto_parse(const char* buf, size_t size, upb_Arena* arena) {
   google_protobuf_FieldDescriptorProto* ret = google_protobuf_FieldDescriptorProto_new(arena);
@@ -1840,14 +2370,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_EnumValueDescriptorProto* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_EnumDescriptorProto_value_upb_array(const google_protobuf_EnumDescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {2, UPB_SIZE(4, 24), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_EnumDescriptorProto_value_mutable_upb_array(const google_protobuf_EnumDescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {2, UPB_SIZE(4, 24), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_EnumDescriptorProto_has_value(const google_protobuf_EnumDescriptorProto* msg) {
   size_t size;
   google_protobuf_EnumDescriptorProto_value(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_EnumDescriptorProto_clear_options(google_protobuf_EnumDescriptorProto* msg) {
   const upb_MiniTableField field = {3, UPB_SIZE(8, 32), 2, 1, 11, kUpb_FieldMode_Scalar | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -1875,14 +2422,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_EnumDescriptorProto_EnumReservedRange* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_EnumDescriptorProto_reserved_range_upb_array(const google_protobuf_EnumDescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {4, UPB_SIZE(12, 40), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_EnumDescriptorProto_reserved_range_mutable_upb_array(const google_protobuf_EnumDescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {4, UPB_SIZE(12, 40), 0, 2, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_EnumDescriptorProto_has_reserved_range(const google_protobuf_EnumDescriptorProto* msg) {
   size_t size;
   google_protobuf_EnumDescriptorProto_reserved_range(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_EnumDescriptorProto_clear_reserved_name(google_protobuf_EnumDescriptorProto* msg) {
   const upb_MiniTableField field = {5, UPB_SIZE(16, 48), 0, kUpb_NoSub, 12, kUpb_FieldMode_Array | kUpb_LabelFlags_IsAlternate | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -1895,14 +2459,31 @@
     if (size) *size = arr->size;
     return (upb_StringView const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_EnumDescriptorProto_reserved_name_upb_array(const google_protobuf_EnumDescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {5, UPB_SIZE(16, 48), 0, kUpb_NoSub, 12, kUpb_FieldMode_Array | kUpb_LabelFlags_IsAlternate | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_EnumDescriptorProto_reserved_name_mutable_upb_array(const google_protobuf_EnumDescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {5, UPB_SIZE(16, 48), 0, kUpb_NoSub, 12, kUpb_FieldMode_Array | kUpb_LabelFlags_IsAlternate | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_EnumDescriptorProto_has_reserved_name(const google_protobuf_EnumDescriptorProto* msg) {
   size_t size;
   google_protobuf_EnumDescriptorProto_reserved_name(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE void google_protobuf_EnumDescriptorProto_set_name(google_protobuf_EnumDescriptorProto *msg, upb_StringView value) {
@@ -2236,14 +2817,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_MethodDescriptorProto* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_ServiceDescriptorProto_method_upb_array(const google_protobuf_ServiceDescriptorProto* msg, size_t* size) {
+  const upb_MiniTableField field = {2, UPB_SIZE(4, 24), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_ServiceDescriptorProto_method_mutable_upb_array(const google_protobuf_ServiceDescriptorProto* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {2, UPB_SIZE(4, 24), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_ServiceDescriptorProto_has_method(const google_protobuf_ServiceDescriptorProto* msg) {
   size_t size;
   google_protobuf_ServiceDescriptorProto_method(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_ServiceDescriptorProto_clear_options(google_protobuf_ServiceDescriptorProto* msg) {
   const upb_MiniTableField field = {3, UPB_SIZE(8, 32), 2, 1, 11, kUpb_FieldMode_Scalar | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -2809,14 +3407,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_UninterpretedOption* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_FileOptions_uninterpreted_option_upb_array(const google_protobuf_FileOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {999, UPB_SIZE(20, 184), 0, 1, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_FileOptions_uninterpreted_option_mutable_upb_array(const google_protobuf_FileOptions* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {999, UPB_SIZE(20, 184), 0, 1, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_FileOptions_has_uninterpreted_option(const google_protobuf_FileOptions* msg) {
   size_t size;
   google_protobuf_FileOptions_uninterpreted_option(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE void google_protobuf_FileOptions_set_java_package(google_protobuf_FileOptions *msg, upb_StringView value) {
@@ -3047,14 +3662,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_UninterpretedOption* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_MessageOptions_uninterpreted_option_upb_array(const google_protobuf_MessageOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {999, 8, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_MessageOptions_uninterpreted_option_mutable_upb_array(const google_protobuf_MessageOptions* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {999, 8, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_MessageOptions_has_uninterpreted_option(const google_protobuf_MessageOptions* msg) {
   size_t size;
   google_protobuf_MessageOptions_uninterpreted_option(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE void google_protobuf_MessageOptions_set_message_set_wire_format(google_protobuf_MessageOptions *msg, bool value) {
@@ -3285,29 +3917,83 @@
   _upb_Message_GetNonExtensionField(msg, &field, &default_val, &ret);
   return ret;
 }
 UPB_INLINE bool google_protobuf_FieldOptions_has_target(const google_protobuf_FieldOptions* msg) {
   const upb_MiniTableField field = {18, 24, 10, 3, 14, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   return _upb_Message_HasNonExtensionField(msg, &field);
 }
+UPB_INLINE void google_protobuf_FieldOptions_clear_targets(google_protobuf_FieldOptions* msg) {
+  const upb_MiniTableField field = {19, UPB_SIZE(28, 32), 0, 4, 14, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  _upb_Message_ClearNonExtensionField(msg, &field);
+}
+UPB_INLINE int32_t const* google_protobuf_FieldOptions_targets(const google_protobuf_FieldOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {19, UPB_SIZE(28, 32), 0, 4, 14, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (arr) {
+    if (size) *size = arr->size;
+    return (int32_t const*)_upb_array_constptr(arr);
+  } else {
+    if (size) *size = 0;
+    return NULL;
+  }
+}
+UPB_INLINE const upb_Array* _google_protobuf_FieldOptions_targets_upb_array(const google_protobuf_FieldOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {19, UPB_SIZE(28, 32), 0, 4, 14, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_FieldOptions_targets_mutable_upb_array(const google_protobuf_FieldOptions* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {19, UPB_SIZE(28, 32), 0, 4, 14, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE bool google_protobuf_FieldOptions_has_targets(const google_protobuf_FieldOptions* msg) {
+  size_t size;
+  google_protobuf_FieldOptions_targets(msg, &size);
+  return size != 0;
+}
 UPB_INLINE void google_protobuf_FieldOptions_clear_uninterpreted_option(google_protobuf_FieldOptions* msg) {
-  const upb_MiniTableField field = {999, UPB_SIZE(28, 32), 0, 4, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {999, UPB_SIZE(32, 40), 0, 5, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   _upb_Message_ClearNonExtensionField(msg, &field);
 }
 UPB_INLINE const google_protobuf_UninterpretedOption* const* google_protobuf_FieldOptions_uninterpreted_option(const google_protobuf_FieldOptions* msg, size_t* size) {
-  const upb_MiniTableField field = {999, UPB_SIZE(28, 32), 0, 4, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_MiniTableField field = {999, UPB_SIZE(32, 40), 0, 5, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   const upb_Array* arr = upb_Message_GetArray(msg, &field);
   if (arr) {
     if (size) *size = arr->size;
     return (const google_protobuf_UninterpretedOption* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_FieldOptions_uninterpreted_option_upb_array(const google_protobuf_FieldOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {999, UPB_SIZE(32, 40), 0, 5, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_FieldOptions_uninterpreted_option_mutable_upb_array(const google_protobuf_FieldOptions* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {999, UPB_SIZE(32, 40), 0, 5, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_FieldOptions_has_uninterpreted_option(const google_protobuf_FieldOptions* msg) {
   size_t size;
   google_protobuf_FieldOptions_uninterpreted_option(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE void google_protobuf_FieldOptions_set_ctype(google_protobuf_FieldOptions *msg, int32_t value) {
@@ -3346,31 +4032,55 @@
   const upb_MiniTableField field = {17, 20, 9, 2, 14, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   _upb_Message_SetNonExtensionField(msg, &field, &value);
 }
 UPB_INLINE void google_protobuf_FieldOptions_set_target(google_protobuf_FieldOptions *msg, int32_t value) {
   const upb_MiniTableField field = {18, 24, 10, 3, 14, kUpb_FieldMode_Scalar | (kUpb_FieldRep_4Byte << kUpb_FieldRep_Shift)};
   _upb_Message_SetNonExtensionField(msg, &field, &value);
 }
+UPB_INLINE int32_t* google_protobuf_FieldOptions_mutable_targets(google_protobuf_FieldOptions* msg, size_t* size) {
+  upb_MiniTableField field = {19, UPB_SIZE(28, 32), 0, 4, 14, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetMutableArray(msg, &field);
+  if (arr) {
+    if (size) *size = arr->size;
+    return (int32_t*)_upb_array_ptr(arr);
+  } else {
+    if (size) *size = 0;
+    return NULL;
+  }
+}
+UPB_INLINE int32_t* google_protobuf_FieldOptions_resize_targets(google_protobuf_FieldOptions* msg, size_t size, upb_Arena* arena) {
+  upb_MiniTableField field = {19, UPB_SIZE(28, 32), 0, 4, 14, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  return (int32_t*)upb_Message_ResizeArray(msg, &field, size, arena);
+}
+UPB_INLINE bool google_protobuf_FieldOptions_add_targets(google_protobuf_FieldOptions* msg, int32_t val, upb_Arena* arena) {
+  upb_MiniTableField field = {19, UPB_SIZE(28, 32), 0, 4, 14, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(msg, &field, arena);
+  if (!arr || !_upb_Array_ResizeUninitialized(arr, arr->size + 1, arena)) {
+    return false;
+  }
+  _upb_Array_Set(arr, arr->size - 1, &val, sizeof(val));
+  return true;
+}
 UPB_INLINE google_protobuf_UninterpretedOption** google_protobuf_FieldOptions_mutable_uninterpreted_option(google_protobuf_FieldOptions* msg, size_t* size) {
-  upb_MiniTableField field = {999, UPB_SIZE(28, 32), 0, 4, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_MiniTableField field = {999, UPB_SIZE(32, 40), 0, 5, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetMutableArray(msg, &field);
   if (arr) {
     if (size) *size = arr->size;
     return (google_protobuf_UninterpretedOption**)_upb_array_ptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
 UPB_INLINE google_protobuf_UninterpretedOption** google_protobuf_FieldOptions_resize_uninterpreted_option(google_protobuf_FieldOptions* msg, size_t size, upb_Arena* arena) {
-  upb_MiniTableField field = {999, UPB_SIZE(28, 32), 0, 4, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_MiniTableField field = {999, UPB_SIZE(32, 40), 0, 5, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   return (google_protobuf_UninterpretedOption**)upb_Message_ResizeArray(msg, &field, size, arena);
 }
 UPB_INLINE struct google_protobuf_UninterpretedOption* google_protobuf_FieldOptions_add_uninterpreted_option(google_protobuf_FieldOptions* msg, upb_Arena* arena) {
-  upb_MiniTableField field = {999, UPB_SIZE(28, 32), 0, 4, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_MiniTableField field = {999, UPB_SIZE(32, 40), 0, 5, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
   upb_Array* arr = upb_Message_GetOrCreateMutableArray(msg, &field, arena);
   if (!arr || !_upb_Array_ResizeUninitialized(arr, arr->size + 1, arena)) {
     return NULL;
   }
   struct google_protobuf_UninterpretedOption* sub = (struct google_protobuf_UninterpretedOption*)_upb_Message_New(&google_protobuf_UninterpretedOption_msg_init, arena);
   if (!arr || !sub) return NULL;
   _upb_Array_Set(arr, arr->size - 1, &sub, sizeof(sub));
@@ -3423,14 +4133,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_UninterpretedOption* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_OneofOptions_uninterpreted_option_upb_array(const google_protobuf_OneofOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {999, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_OneofOptions_uninterpreted_option_mutable_upb_array(const google_protobuf_OneofOptions* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {999, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_OneofOptions_has_uninterpreted_option(const google_protobuf_OneofOptions* msg) {
   size_t size;
   google_protobuf_OneofOptions_uninterpreted_option(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE google_protobuf_UninterpretedOption** google_protobuf_OneofOptions_mutable_uninterpreted_option(google_protobuf_OneofOptions* msg, size_t* size) {
@@ -3551,14 +4278,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_UninterpretedOption* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_EnumOptions_uninterpreted_option_upb_array(const google_protobuf_EnumOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {999, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_EnumOptions_uninterpreted_option_mutable_upb_array(const google_protobuf_EnumOptions* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {999, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_EnumOptions_has_uninterpreted_option(const google_protobuf_EnumOptions* msg) {
   size_t size;
   google_protobuf_EnumOptions_uninterpreted_option(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE void google_protobuf_EnumOptions_set_allow_alias(google_protobuf_EnumOptions *msg, bool value) {
@@ -3661,14 +4405,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_UninterpretedOption* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_EnumValueOptions_uninterpreted_option_upb_array(const google_protobuf_EnumValueOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {999, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_EnumValueOptions_uninterpreted_option_mutable_upb_array(const google_protobuf_EnumValueOptions* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {999, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_EnumValueOptions_has_uninterpreted_option(const google_protobuf_EnumValueOptions* msg) {
   size_t size;
   google_protobuf_EnumValueOptions_uninterpreted_option(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE void google_protobuf_EnumValueOptions_set_deprecated(google_protobuf_EnumValueOptions *msg, bool value) {
@@ -3763,14 +4524,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_UninterpretedOption* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_ServiceOptions_uninterpreted_option_upb_array(const google_protobuf_ServiceOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {999, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_ServiceOptions_uninterpreted_option_mutable_upb_array(const google_protobuf_ServiceOptions* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {999, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_ServiceOptions_has_uninterpreted_option(const google_protobuf_ServiceOptions* msg) {
   size_t size;
   google_protobuf_ServiceOptions_uninterpreted_option(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE void google_protobuf_ServiceOptions_set_deprecated(google_protobuf_ServiceOptions *msg, bool value) {
@@ -3880,14 +4658,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_UninterpretedOption* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_MethodOptions_uninterpreted_option_upb_array(const google_protobuf_MethodOptions* msg, size_t* size) {
+  const upb_MiniTableField field = {999, 8, 0, 1, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_MethodOptions_uninterpreted_option_mutable_upb_array(const google_protobuf_MethodOptions* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {999, 8, 0, 1, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_MethodOptions_has_uninterpreted_option(const google_protobuf_MethodOptions* msg) {
   size_t size;
   google_protobuf_MethodOptions_uninterpreted_option(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE void google_protobuf_MethodOptions_set_deprecated(google_protobuf_MethodOptions *msg, bool value) {
@@ -3971,14 +4766,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_UninterpretedOption_NamePart* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_UninterpretedOption_name_upb_array(const google_protobuf_UninterpretedOption* msg, size_t* size) {
+  const upb_MiniTableField field = {2, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_UninterpretedOption_name_mutable_upb_array(const google_protobuf_UninterpretedOption* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {2, UPB_SIZE(4, 8), 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_UninterpretedOption_has_name(const google_protobuf_UninterpretedOption* msg) {
   size_t size;
   google_protobuf_UninterpretedOption_name(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_UninterpretedOption_clear_identifier_value(google_protobuf_UninterpretedOption* msg) {
   const upb_MiniTableField field = {3, UPB_SIZE(8, 16), 1, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
@@ -4243,14 +5055,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_SourceCodeInfo_Location* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_SourceCodeInfo_location_upb_array(const google_protobuf_SourceCodeInfo* msg, size_t* size) {
+  const upb_MiniTableField field = {1, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_SourceCodeInfo_location_mutable_upb_array(const google_protobuf_SourceCodeInfo* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {1, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_SourceCodeInfo_has_location(const google_protobuf_SourceCodeInfo* msg) {
   size_t size;
   google_protobuf_SourceCodeInfo_location(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE google_protobuf_SourceCodeInfo_Location** google_protobuf_SourceCodeInfo_mutable_location(google_protobuf_SourceCodeInfo* msg, size_t* size) {
@@ -4326,14 +5155,31 @@
     if (size) *size = arr->size;
     return (int32_t const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_SourceCodeInfo_Location_path_upb_array(const google_protobuf_SourceCodeInfo_Location* msg, size_t* size) {
+  const upb_MiniTableField field = {1, UPB_SIZE(4, 8), 0, kUpb_NoSub, 5, kUpb_FieldMode_Array | kUpb_LabelFlags_IsPacked | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_SourceCodeInfo_Location_path_mutable_upb_array(const google_protobuf_SourceCodeInfo_Location* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {1, UPB_SIZE(4, 8), 0, kUpb_NoSub, 5, kUpb_FieldMode_Array | kUpb_LabelFlags_IsPacked | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_SourceCodeInfo_Location_has_path(const google_protobuf_SourceCodeInfo_Location* msg) {
   size_t size;
   google_protobuf_SourceCodeInfo_Location_path(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_SourceCodeInfo_Location_clear_span(google_protobuf_SourceCodeInfo_Location* msg) {
   const upb_MiniTableField field = {2, UPB_SIZE(8, 16), 0, kUpb_NoSub, 5, kUpb_FieldMode_Array | kUpb_LabelFlags_IsPacked | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
@@ -4346,14 +5192,31 @@
     if (size) *size = arr->size;
     return (int32_t const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_SourceCodeInfo_Location_span_upb_array(const google_protobuf_SourceCodeInfo_Location* msg, size_t* size) {
+  const upb_MiniTableField field = {2, UPB_SIZE(8, 16), 0, kUpb_NoSub, 5, kUpb_FieldMode_Array | kUpb_LabelFlags_IsPacked | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_SourceCodeInfo_Location_span_mutable_upb_array(const google_protobuf_SourceCodeInfo_Location* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {2, UPB_SIZE(8, 16), 0, kUpb_NoSub, 5, kUpb_FieldMode_Array | kUpb_LabelFlags_IsPacked | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_SourceCodeInfo_Location_has_span(const google_protobuf_SourceCodeInfo_Location* msg) {
   size_t size;
   google_protobuf_SourceCodeInfo_Location_span(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_SourceCodeInfo_Location_clear_leading_comments(google_protobuf_SourceCodeInfo_Location* msg) {
   const upb_MiniTableField field = {3, UPB_SIZE(16, 24), 1, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
@@ -4396,14 +5259,31 @@
     if (size) *size = arr->size;
     return (upb_StringView const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_SourceCodeInfo_Location_leading_detached_comments_upb_array(const google_protobuf_SourceCodeInfo_Location* msg, size_t* size) {
+  const upb_MiniTableField field = {6, UPB_SIZE(12, 56), 0, kUpb_NoSub, 12, kUpb_FieldMode_Array | kUpb_LabelFlags_IsAlternate | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_SourceCodeInfo_Location_leading_detached_comments_mutable_upb_array(const google_protobuf_SourceCodeInfo_Location* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {6, UPB_SIZE(12, 56), 0, kUpb_NoSub, 12, kUpb_FieldMode_Array | kUpb_LabelFlags_IsAlternate | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_SourceCodeInfo_Location_has_leading_detached_comments(const google_protobuf_SourceCodeInfo_Location* msg) {
   size_t size;
   google_protobuf_SourceCodeInfo_Location_leading_detached_comments(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE int32_t* google_protobuf_SourceCodeInfo_Location_mutable_path(google_protobuf_SourceCodeInfo_Location* msg, size_t* size) {
@@ -4533,14 +5413,31 @@
     if (size) *size = arr->size;
     return (const google_protobuf_GeneratedCodeInfo_Annotation* const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_GeneratedCodeInfo_annotation_upb_array(const google_protobuf_GeneratedCodeInfo* msg, size_t* size) {
+  const upb_MiniTableField field = {1, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_GeneratedCodeInfo_annotation_mutable_upb_array(const google_protobuf_GeneratedCodeInfo* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {1, 0, 0, 0, 11, kUpb_FieldMode_Array | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_GeneratedCodeInfo_has_annotation(const google_protobuf_GeneratedCodeInfo* msg) {
   size_t size;
   google_protobuf_GeneratedCodeInfo_annotation(msg, &size);
   return size != 0;
 }
 
 UPB_INLINE google_protobuf_GeneratedCodeInfo_Annotation** google_protobuf_GeneratedCodeInfo_mutable_annotation(google_protobuf_GeneratedCodeInfo* msg, size_t* size) {
@@ -4616,14 +5513,31 @@
     if (size) *size = arr->size;
     return (int32_t const*)_upb_array_constptr(arr);
   } else {
     if (size) *size = 0;
     return NULL;
   }
 }
+UPB_INLINE const upb_Array* _google_protobuf_GeneratedCodeInfo_Annotation_path_upb_array(const google_protobuf_GeneratedCodeInfo_Annotation* msg, size_t* size) {
+  const upb_MiniTableField field = {1, UPB_SIZE(4, 16), 0, kUpb_NoSub, 5, kUpb_FieldMode_Array | kUpb_LabelFlags_IsPacked | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  const upb_Array* arr = upb_Message_GetArray(msg, &field);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
+UPB_INLINE upb_Array* _google_protobuf_GeneratedCodeInfo_Annotation_path_mutable_upb_array(const google_protobuf_GeneratedCodeInfo_Annotation* msg, size_t* size, upb_Arena* arena) {
+  const upb_MiniTableField field = {1, UPB_SIZE(4, 16), 0, kUpb_NoSub, 5, kUpb_FieldMode_Array | kUpb_LabelFlags_IsPacked | (UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte) << kUpb_FieldRep_Shift)};
+  upb_Array* arr = upb_Message_GetOrCreateMutableArray(
+      (upb_Message*)msg, &field, arena);
+  if (size) {
+    *size = arr ? arr->size : 0;
+  }
+  return arr;
+}
 UPB_INLINE bool google_protobuf_GeneratedCodeInfo_Annotation_has_path(const google_protobuf_GeneratedCodeInfo_Annotation* msg) {
   size_t size;
   google_protobuf_GeneratedCodeInfo_Annotation_path(msg, &size);
   return size != 0;
 }
 UPB_INLINE void google_protobuf_GeneratedCodeInfo_Annotation_clear_source_file(google_protobuf_GeneratedCodeInfo_Annotation* msg) {
   const upb_MiniTableField field = {2, UPB_SIZE(20, 24), 1, kUpb_NoSub, 12, kUpb_FieldMode_Scalar | kUpb_LabelFlags_IsAlternate | (kUpb_FieldRep_StringView << kUpb_FieldRep_Shift)};
```

### Comparing `protobuf-4.22.3/google/protobuf/descriptor.upbdefs.c` & `protobuf-4.23.0rc2/google/protobuf/descriptor.upbdefs.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
  * Do not edit -- your changes will be discarded when the file is
  * regenerated. */
 
 #include "upb/reflection/def.h"
 #include "google/protobuf/descriptor.upbdefs.h"
 #include "google/protobuf/descriptor.upb.h"
 
-static const char descriptor[8545] = {'\n', ' ', 'g', 'o', 'o', 'g', 'l', 'e', '/', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '/', 'd', 'e', 's', 'c', 'r', 'i', 'p', 
+static const char descriptor[9057] = {'\n', ' ', 'g', 'o', 'o', 'g', 'l', 'e', '/', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '/', 'd', 'e', 's', 'c', 'r', 'i', 'p', 
 't', 'o', 'r', '.', 'p', 'r', 'o', 't', 'o', '\022', '\017', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
 'f', '\"', 'M', '\n', '\021', 'F', 'i', 'l', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'S', 'e', 't', '\022', '8', '\n', 
 '\004', 'f', 'i', 'l', 'e', '\030', '\001', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 
 'o', 'b', 'u', 'f', '.', 'F', 'i', 'l', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', 'R', 
 '\004', 'f', 'i', 'l', 'e', '\"', '\376', '\004', '\n', '\023', 'F', 'i', 'l', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 
 'r', 'o', 't', 'o', '\022', '\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\004', 'n', 'a', 'm', 'e', '\022', 
 '\030', '\n', '\007', 'p', 'a', 'c', 'k', 'a', 'g', 'e', '\030', '\002', ' ', '\001', '(', '\t', 'R', '\007', 'p', 'a', 'c', 'k', 'a', 'g', 'e', 
@@ -70,297 +70,318 @@
 'e', 'n', 's', 'i', 'o', 'n', 'R', 'a', 'n', 'g', 'e', '\022', '\024', '\n', '\005', 's', 't', 'a', 'r', 't', '\030', '\001', ' ', '\001', '(', 
 '\005', 'R', '\005', 's', 't', 'a', 'r', 't', '\022', '\020', '\n', '\003', 'e', 'n', 'd', '\030', '\002', ' ', '\001', '(', '\005', 'R', '\003', 'e', 'n', 
 'd', '\022', '@', '\n', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\030', '\003', ' ', '\001', '(', '\013', '2', '&', '.', 'g', 'o', 'o', 'g', 
 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'x', 't', 'e', 'n', 's', 'i', 'o', 'n', 'R', 'a', 'n', 'g', 
 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', 'R', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\032', '7', '\n', '\r', 'R', 'e', 's', 'e', 
 'r', 'v', 'e', 'd', 'R', 'a', 'n', 'g', 'e', '\022', '\024', '\n', '\005', 's', 't', 'a', 'r', 't', '\030', '\001', ' ', '\001', '(', '\005', 'R', 
 '\005', 's', 't', 'a', 'r', 't', '\022', '\020', '\n', '\003', 'e', 'n', 'd', '\030', '\002', ' ', '\001', '(', '\005', 'R', '\003', 'e', 'n', 'd', '\"', 
-'|', '\n', '\025', 'E', 'x', 't', 'e', 'n', 's', 'i', 'o', 'n', 'R', 'a', 'n', 'g', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', 
-'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', 
-'\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 
-'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 
-'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', 
-'\"', '\301', '\006', '\n', '\024', 'F', 'i', 'e', 'l', 'd', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', 
-'\022', '\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\004', 'n', 'a', 'm', 'e', '\022', '\026', '\n', '\006', 'n', 
-'u', 'm', 'b', 'e', 'r', '\030', '\003', ' ', '\001', '(', '\005', 'R', '\006', 'n', 'u', 'm', 'b', 'e', 'r', '\022', 'A', '\n', '\005', 'l', 'a', 
-'b', 'e', 'l', '\030', '\004', ' ', '\001', '(', '\016', '2', '+', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 
-'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '.', 'L', 
-'a', 'b', 'e', 'l', 'R', '\005', 'l', 'a', 'b', 'e', 'l', '\022', '>', '\n', '\004', 't', 'y', 'p', 'e', '\030', '\005', ' ', '\001', '(', '\016', 
-'2', '*', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'D', 
-'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '.', 'T', 'y', 'p', 'e', 'R', '\004', 't', 'y', 'p', 'e', 
-'\022', '\033', '\n', '\t', 't', 'y', 'p', 'e', '_', 'n', 'a', 'm', 'e', '\030', '\006', ' ', '\001', '(', '\t', 'R', '\010', 't', 'y', 'p', 'e', 
-'N', 'a', 'm', 'e', '\022', '\032', '\n', '\010', 'e', 'x', 't', 'e', 'n', 'd', 'e', 'e', '\030', '\002', ' ', '\001', '(', '\t', 'R', '\010', 'e', 
-'x', 't', 'e', 'n', 'd', 'e', 'e', '\022', '#', '\n', '\r', 'd', 'e', 'f', 'a', 'u', 'l', 't', '_', 'v', 'a', 'l', 'u', 'e', '\030', 
-'\007', ' ', '\001', '(', '\t', 'R', '\014', 'd', 'e', 'f', 'a', 'u', 'l', 't', 'V', 'a', 'l', 'u', 'e', '\022', '\037', '\n', '\013', 'o', 'n', 
-'e', 'o', 'f', '_', 'i', 'n', 'd', 'e', 'x', '\030', '\t', ' ', '\001', '(', '\005', 'R', '\n', 'o', 'n', 'e', 'o', 'f', 'I', 'n', 'd', 
-'e', 'x', '\022', '\033', '\n', '\t', 'j', 's', 'o', 'n', '_', 'n', 'a', 'm', 'e', '\030', '\n', ' ', '\001', '(', '\t', 'R', '\010', 'j', 's', 
-'o', 'n', 'N', 'a', 'm', 'e', '\022', '7', '\n', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\030', '\010', ' ', '\001', '(', '\013', '2', '\035', 
-'.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'O', 'p', 't', 
-'i', 'o', 'n', 's', 'R', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\022', '\'', '\n', '\017', 'p', 'r', 'o', 't', 'o', '3', '_', 'o', 
-'p', 't', 'i', 'o', 'n', 'a', 'l', '\030', '\021', ' ', '\001', '(', '\010', 'R', '\016', 'p', 'r', 'o', 't', 'o', '3', 'O', 'p', 't', 'i', 
-'o', 'n', 'a', 'l', '\"', '\266', '\002', '\n', '\004', 'T', 'y', 'p', 'e', '\022', '\017', '\n', '\013', 'T', 'Y', 'P', 'E', '_', 'D', 'O', 'U', 
-'B', 'L', 'E', '\020', '\001', '\022', '\016', '\n', '\n', 'T', 'Y', 'P', 'E', '_', 'F', 'L', 'O', 'A', 'T', '\020', '\002', '\022', '\016', '\n', '\n', 
-'T', 'Y', 'P', 'E', '_', 'I', 'N', 'T', '6', '4', '\020', '\003', '\022', '\017', '\n', '\013', 'T', 'Y', 'P', 'E', '_', 'U', 'I', 'N', 'T', 
-'6', '4', '\020', '\004', '\022', '\016', '\n', '\n', 'T', 'Y', 'P', 'E', '_', 'I', 'N', 'T', '3', '2', '\020', '\005', '\022', '\020', '\n', '\014', 'T', 
-'Y', 'P', 'E', '_', 'F', 'I', 'X', 'E', 'D', '6', '4', '\020', '\006', '\022', '\020', '\n', '\014', 'T', 'Y', 'P', 'E', '_', 'F', 'I', 'X', 
-'E', 'D', '3', '2', '\020', '\007', '\022', '\r', '\n', '\t', 'T', 'Y', 'P', 'E', '_', 'B', 'O', 'O', 'L', '\020', '\010', '\022', '\017', '\n', '\013', 
-'T', 'Y', 'P', 'E', '_', 'S', 'T', 'R', 'I', 'N', 'G', '\020', '\t', '\022', '\016', '\n', '\n', 'T', 'Y', 'P', 'E', '_', 'G', 'R', 'O', 
-'U', 'P', '\020', '\n', '\022', '\020', '\n', '\014', 'T', 'Y', 'P', 'E', '_', 'M', 'E', 'S', 'S', 'A', 'G', 'E', '\020', '\013', '\022', '\016', '\n', 
-'\n', 'T', 'Y', 'P', 'E', '_', 'B', 'Y', 'T', 'E', 'S', '\020', '\014', '\022', '\017', '\n', '\013', 'T', 'Y', 'P', 'E', '_', 'U', 'I', 'N', 
-'T', '3', '2', '\020', '\r', '\022', '\r', '\n', '\t', 'T', 'Y', 'P', 'E', '_', 'E', 'N', 'U', 'M', '\020', '\016', '\022', '\021', '\n', '\r', 'T', 
-'Y', 'P', 'E', '_', 'S', 'F', 'I', 'X', 'E', 'D', '3', '2', '\020', '\017', '\022', '\021', '\n', '\r', 'T', 'Y', 'P', 'E', '_', 'S', 'F', 
-'I', 'X', 'E', 'D', '6', '4', '\020', '\020', '\022', '\017', '\n', '\013', 'T', 'Y', 'P', 'E', '_', 'S', 'I', 'N', 'T', '3', '2', '\020', '\021', 
-'\022', '\017', '\n', '\013', 'T', 'Y', 'P', 'E', '_', 'S', 'I', 'N', 'T', '6', '4', '\020', '\022', '\"', 'C', '\n', '\005', 'L', 'a', 'b', 'e', 
-'l', '\022', '\022', '\n', '\016', 'L', 'A', 'B', 'E', 'L', '_', 'O', 'P', 'T', 'I', 'O', 'N', 'A', 'L', '\020', '\001', '\022', '\022', '\n', '\016', 
-'L', 'A', 'B', 'E', 'L', '_', 'R', 'E', 'Q', 'U', 'I', 'R', 'E', 'D', '\020', '\002', '\022', '\022', '\n', '\016', 'L', 'A', 'B', 'E', 'L', 
-'_', 'R', 'E', 'P', 'E', 'A', 'T', 'E', 'D', '\020', '\003', '\"', 'c', '\n', '\024', 'O', 'n', 'e', 'o', 'f', 'D', 'e', 's', 'c', 'r', 
-'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '\022', '\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', 
-'\004', 'n', 'a', 'm', 'e', '\022', '7', '\n', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\030', '\002', ' ', '\001', '(', '\013', '2', '\035', '.', 
-'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'O', 'n', 'e', 'o', 'f', 'O', 'p', 't', 'i', 
-'o', 'n', 's', 'R', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\"', '\343', '\002', '\n', '\023', 'E', 'n', 'u', 'm', 'D', 'e', 's', 'c', 
-'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '\022', '\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 
-'R', '\004', 'n', 'a', 'm', 'e', '\022', '?', '\n', '\005', 'v', 'a', 'l', 'u', 'e', '\030', '\002', ' ', '\003', '(', '\013', '2', ')', '.', 'g', 
-'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'n', 'u', 'm', 'V', 'a', 'l', 'u', 'e', 'D', 
-'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', 'R', '\005', 'v', 'a', 'l', 'u', 'e', '\022', '6', '\n', '\007', 
-'o', 'p', 't', 'i', 'o', 'n', 's', '\030', '\003', ' ', '\001', '(', '\013', '2', '\034', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 
-'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'n', 'u', 'm', 'O', 'p', 't', 'i', 'o', 'n', 's', 'R', '\007', 'o', 'p', 't', 'i', 'o', 
-'n', 's', '\022', ']', '\n', '\016', 'r', 'e', 's', 'e', 'r', 'v', 'e', 'd', '_', 'r', 'a', 'n', 'g', 'e', '\030', '\004', ' ', '\003', '(', 
-'\013', '2', '6', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'n', 'u', 'm', 'D', 
-'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '.', 'E', 'n', 'u', 'm', 'R', 'e', 's', 'e', 'r', 'v', 
-'e', 'd', 'R', 'a', 'n', 'g', 'e', 'R', '\r', 'r', 'e', 's', 'e', 'r', 'v', 'e', 'd', 'R', 'a', 'n', 'g', 'e', '\022', '#', '\n', 
-'\r', 'r', 'e', 's', 'e', 'r', 'v', 'e', 'd', '_', 'n', 'a', 'm', 'e', '\030', '\005', ' ', '\003', '(', '\t', 'R', '\014', 'r', 'e', 's', 
-'e', 'r', 'v', 'e', 'd', 'N', 'a', 'm', 'e', '\032', ';', '\n', '\021', 'E', 'n', 'u', 'm', 'R', 'e', 's', 'e', 'r', 'v', 'e', 'd', 
-'R', 'a', 'n', 'g', 'e', '\022', '\024', '\n', '\005', 's', 't', 'a', 'r', 't', '\030', '\001', ' ', '\001', '(', '\005', 'R', '\005', 's', 't', 'a', 
-'r', 't', '\022', '\020', '\n', '\003', 'e', 'n', 'd', '\030', '\002', ' ', '\001', '(', '\005', 'R', '\003', 'e', 'n', 'd', '\"', '\203', '\001', '\n', '\030', 
-'E', 'n', 'u', 'm', 'V', 'a', 'l', 'u', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '\022', 
-'\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\004', 'n', 'a', 'm', 'e', '\022', '\026', '\n', '\006', 'n', 'u', 
-'m', 'b', 'e', 'r', '\030', '\002', ' ', '\001', '(', '\005', 'R', '\006', 'n', 'u', 'm', 'b', 'e', 'r', '\022', ';', '\n', '\007', 'o', 'p', 't', 
-'i', 'o', 'n', 's', '\030', '\003', ' ', '\001', '(', '\013', '2', '!', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 
-'b', 'u', 'f', '.', 'E', 'n', 'u', 'm', 'V', 'a', 'l', 'u', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', 'R', '\007', 'o', 'p', 't', 
-'i', 'o', 'n', 's', '\"', '\247', '\001', '\n', '\026', 'S', 'e', 'r', 'v', 'i', 'c', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 
-'r', 'P', 'r', 'o', 't', 'o', '\022', '\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\004', 'n', 'a', 'm', 
-'e', '\022', '>', '\n', '\006', 'm', 'e', 't', 'h', 'o', 'd', '\030', '\002', ' ', '\003', '(', '\013', '2', '&', '.', 'g', 'o', 'o', 'g', 'l', 
-'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'M', 'e', 't', 'h', 'o', 'd', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 
-'o', 'r', 'P', 'r', 'o', 't', 'o', 'R', '\006', 'm', 'e', 't', 'h', 'o', 'd', '\022', '9', '\n', '\007', 'o', 'p', 't', 'i', 'o', 'n', 
-'s', '\030', '\003', ' ', '\001', '(', '\013', '2', '\037', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', 
-'.', 'S', 'e', 'r', 'v', 'i', 'c', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', 'R', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\"', 
-'\211', '\002', '\n', '\025', 'M', 'e', 't', 'h', 'o', 'd', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', 
-'\022', '\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\004', 'n', 'a', 'm', 'e', '\022', '\035', '\n', '\n', 'i', 
-'n', 'p', 'u', 't', '_', 't', 'y', 'p', 'e', '\030', '\002', ' ', '\001', '(', '\t', 'R', '\t', 'i', 'n', 'p', 'u', 't', 'T', 'y', 'p', 
-'e', '\022', '\037', '\n', '\013', 'o', 'u', 't', 'p', 'u', 't', '_', 't', 'y', 'p', 'e', '\030', '\003', ' ', '\001', '(', '\t', 'R', '\n', 'o', 
-'u', 't', 'p', 'u', 't', 'T', 'y', 'p', 'e', '\022', '8', '\n', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\030', '\004', ' ', '\001', '(', 
-'\013', '2', '\036', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'M', 'e', 't', 'h', 'o', 
-'d', 'O', 'p', 't', 'i', 'o', 'n', 's', 'R', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\022', '0', '\n', '\020', 'c', 'l', 'i', 'e', 
-'n', 't', '_', 's', 't', 'r', 'e', 'a', 'm', 'i', 'n', 'g', '\030', '\005', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 
-'R', '\017', 'c', 'l', 'i', 'e', 'n', 't', 'S', 't', 'r', 'e', 'a', 'm', 'i', 'n', 'g', '\022', '0', '\n', '\020', 's', 'e', 'r', 'v', 
-'e', 'r', '_', 's', 't', 'r', 'e', 'a', 'm', 'i', 'n', 'g', '\030', '\006', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 
-'R', '\017', 's', 'e', 'r', 'v', 'e', 'r', 'S', 't', 'r', 'e', 'a', 'm', 'i', 'n', 'g', '\"', '\221', '\t', '\n', '\013', 'F', 'i', 'l', 
-'e', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '!', '\n', '\014', 'j', 'a', 'v', 'a', '_', 'p', 'a', 'c', 'k', 'a', 'g', 'e', '\030', 
-'\001', ' ', '\001', '(', '\t', 'R', '\013', 'j', 'a', 'v', 'a', 'P', 'a', 'c', 'k', 'a', 'g', 'e', '\022', '0', '\n', '\024', 'j', 'a', 'v', 
-'a', '_', 'o', 'u', 't', 'e', 'r', '_', 'c', 'l', 'a', 's', 's', 'n', 'a', 'm', 'e', '\030', '\010', ' ', '\001', '(', '\t', 'R', '\022', 
-'j', 'a', 'v', 'a', 'O', 'u', 't', 'e', 'r', 'C', 'l', 'a', 's', 's', 'n', 'a', 'm', 'e', '\022', '5', '\n', '\023', 'j', 'a', 'v', 
-'a', '_', 'm', 'u', 'l', 't', 'i', 'p', 'l', 'e', '_', 'f', 'i', 'l', 'e', 's', '\030', '\n', ' ', '\001', '(', '\010', ':', '\005', 'f', 
-'a', 'l', 's', 'e', 'R', '\021', 'j', 'a', 'v', 'a', 'M', 'u', 'l', 't', 'i', 'p', 'l', 'e', 'F', 'i', 'l', 'e', 's', '\022', 'D', 
-'\n', '\035', 'j', 'a', 'v', 'a', '_', 'g', 'e', 'n', 'e', 'r', 'a', 't', 'e', '_', 'e', 'q', 'u', 'a', 'l', 's', '_', 'a', 'n', 
-'d', '_', 'h', 'a', 's', 'h', '\030', '\024', ' ', '\001', '(', '\010', 'B', '\002', '\030', '\001', 'R', '\031', 'j', 'a', 'v', 'a', 'G', 'e', 'n', 
-'e', 'r', 'a', 't', 'e', 'E', 'q', 'u', 'a', 'l', 's', 'A', 'n', 'd', 'H', 'a', 's', 'h', '\022', ':', '\n', '\026', 'j', 'a', 'v', 
-'a', '_', 's', 't', 'r', 'i', 'n', 'g', '_', 'c', 'h', 'e', 'c', 'k', '_', 'u', 't', 'f', '8', '\030', '\033', ' ', '\001', '(', '\010', 
-':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\023', 'j', 'a', 'v', 'a', 'S', 't', 'r', 'i', 'n', 'g', 'C', 'h', 'e', 'c', 'k', 'U', 
-'t', 'f', '8', '\022', 'S', '\n', '\014', 'o', 'p', 't', 'i', 'm', 'i', 'z', 'e', '_', 'f', 'o', 'r', '\030', '\t', ' ', '\001', '(', '\016', 
-'2', ')', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'l', 'e', 'O', 'p', 
-'t', 'i', 'o', 'n', 's', '.', 'O', 'p', 't', 'i', 'm', 'i', 'z', 'e', 'M', 'o', 'd', 'e', ':', '\005', 'S', 'P', 'E', 'E', 'D', 
-'R', '\013', 'o', 'p', 't', 'i', 'm', 'i', 'z', 'e', 'F', 'o', 'r', '\022', '\035', '\n', '\n', 'g', 'o', '_', 'p', 'a', 'c', 'k', 'a', 
-'g', 'e', '\030', '\013', ' ', '\001', '(', '\t', 'R', '\t', 'g', 'o', 'P', 'a', 'c', 'k', 'a', 'g', 'e', '\022', '5', '\n', '\023', 'c', 'c', 
-'_', 'g', 'e', 'n', 'e', 'r', 'i', 'c', '_', 's', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\030', '\020', ' ', '\001', '(', '\010', ':', '\005', 
-'f', 'a', 'l', 's', 'e', 'R', '\021', 'c', 'c', 'G', 'e', 'n', 'e', 'r', 'i', 'c', 'S', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\022', 
-'9', '\n', '\025', 'j', 'a', 'v', 'a', '_', 'g', 'e', 'n', 'e', 'r', 'i', 'c', '_', 's', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\030', 
-'\021', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\023', 'j', 'a', 'v', 'a', 'G', 'e', 'n', 'e', 'r', 'i', 'c', 
-'S', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\022', '5', '\n', '\023', 'p', 'y', '_', 'g', 'e', 'n', 'e', 'r', 'i', 'c', '_', 's', 'e', 
-'r', 'v', 'i', 'c', 'e', 's', '\030', '\022', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\021', 'p', 'y', 'G', 'e', 
-'n', 'e', 'r', 'i', 'c', 'S', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\022', '7', '\n', '\024', 'p', 'h', 'p', '_', 'g', 'e', 'n', 'e', 
-'r', 'i', 'c', '_', 's', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\030', '*', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 
-'R', '\022', 'p', 'h', 'p', 'G', 'e', 'n', 'e', 'r', 'i', 'c', 'S', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\022', '%', '\n', '\n', 'd', 
-'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '\027', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 
-'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', '.', '\n', '\020', 'c', 'c', '_', 'e', 'n', 'a', 'b', 'l', 'e', '_', 'a', 'r', 
-'e', 'n', 'a', 's', '\030', '\037', ' ', '\001', '(', '\010', ':', '\004', 't', 'r', 'u', 'e', 'R', '\016', 'c', 'c', 'E', 'n', 'a', 'b', 'l', 
-'e', 'A', 'r', 'e', 'n', 'a', 's', '\022', '*', '\n', '\021', 'o', 'b', 'j', 'c', '_', 'c', 'l', 'a', 's', 's', '_', 'p', 'r', 'e', 
-'f', 'i', 'x', '\030', '$', ' ', '\001', '(', '\t', 'R', '\017', 'o', 'b', 'j', 'c', 'C', 'l', 'a', 's', 's', 'P', 'r', 'e', 'f', 'i', 
-'x', '\022', ')', '\n', '\020', 'c', 's', 'h', 'a', 'r', 'p', '_', 'n', 'a', 'm', 'e', 's', 'p', 'a', 'c', 'e', '\030', '%', ' ', '\001', 
-'(', '\t', 'R', '\017', 'c', 's', 'h', 'a', 'r', 'p', 'N', 'a', 'm', 'e', 's', 'p', 'a', 'c', 'e', '\022', '!', '\n', '\014', 's', 'w', 
-'i', 'f', 't', '_', 'p', 'r', 'e', 'f', 'i', 'x', '\030', '\'', ' ', '\001', '(', '\t', 'R', '\013', 's', 'w', 'i', 'f', 't', 'P', 'r', 
-'e', 'f', 'i', 'x', '\022', '(', '\n', '\020', 'p', 'h', 'p', '_', 'c', 'l', 'a', 's', 's', '_', 'p', 'r', 'e', 'f', 'i', 'x', '\030', 
-'(', ' ', '\001', '(', '\t', 'R', '\016', 'p', 'h', 'p', 'C', 'l', 'a', 's', 's', 'P', 'r', 'e', 'f', 'i', 'x', '\022', '#', '\n', '\r', 
-'p', 'h', 'p', '_', 'n', 'a', 'm', 'e', 's', 'p', 'a', 'c', 'e', '\030', ')', ' ', '\001', '(', '\t', 'R', '\014', 'p', 'h', 'p', 'N', 
-'a', 'm', 'e', 's', 'p', 'a', 'c', 'e', '\022', '4', '\n', '\026', 'p', 'h', 'p', '_', 'm', 'e', 't', 'a', 'd', 'a', 't', 'a', '_', 
-'n', 'a', 'm', 'e', 's', 'p', 'a', 'c', 'e', '\030', ',', ' ', '\001', '(', '\t', 'R', '\024', 'p', 'h', 'p', 'M', 'e', 't', 'a', 'd', 
-'a', 't', 'a', 'N', 'a', 'm', 'e', 's', 'p', 'a', 'c', 'e', '\022', '!', '\n', '\014', 'r', 'u', 'b', 'y', '_', 'p', 'a', 'c', 'k', 
-'a', 'g', 'e', '\030', '-', ' ', '\001', '(', '\t', 'R', '\013', 'r', 'u', 'b', 'y', 'P', 'a', 'c', 'k', 'a', 'g', 'e', '\022', 'X', '\n', 
+'\255', '\004', '\n', '\025', 'E', 'x', 't', 'e', 'n', 's', 'i', 'o', 'n', 'R', 'a', 'n', 'g', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', 
+'\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', 
+'\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 
+'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 
+'t', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '\022', 'Y', '\n', '\013', 'd', 'e', 'c', 'l', 'a', 'r', 
+'a', 't', 'i', 'o', 'n', '\030', '\002', ' ', '\003', '(', '\013', '2', '2', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 
+'o', 'b', 'u', 'f', '.', 'E', 'x', 't', 'e', 'n', 's', 'i', 'o', 'n', 'R', 'a', 'n', 'g', 'e', 'O', 'p', 't', 'i', 'o', 'n', 
+'s', '.', 'D', 'e', 'c', 'l', 'a', 'r', 'a', 't', 'i', 'o', 'n', 'B', '\003', '\210', '\001', '\002', 'R', '\013', 'd', 'e', 'c', 'l', 'a', 
+'r', 'a', 't', 'i', 'o', 'n', '\022', 'h', '\n', '\014', 'v', 'e', 'r', 'i', 'f', 'i', 'c', 'a', 't', 'i', 'o', 'n', '\030', '\003', ' ', 
+'\001', '(', '\016', '2', '8', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'x', 't', 
+'e', 'n', 's', 'i', 'o', 'n', 'R', 'a', 'n', 'g', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'V', 'e', 'r', 'i', 'f', 'i', 
+'c', 'a', 't', 'i', 'o', 'n', 'S', 't', 'a', 't', 'e', ':', '\n', 'U', 'N', 'V', 'E', 'R', 'I', 'F', 'I', 'E', 'D', 'R', '\014', 
+'v', 'e', 'r', 'i', 'f', 'i', 'c', 'a', 't', 'i', 'o', 'n', '\032', '\263', '\001', '\n', '\013', 'D', 'e', 'c', 'l', 'a', 'r', 'a', 't', 
+'i', 'o', 'n', '\022', '\026', '\n', '\006', 'n', 'u', 'm', 'b', 'e', 'r', '\030', '\001', ' ', '\001', '(', '\005', 'R', '\006', 'n', 'u', 'm', 'b', 
+'e', 'r', '\022', '\033', '\n', '\t', 'f', 'u', 'l', 'l', '_', 'n', 'a', 'm', 'e', '\030', '\002', ' ', '\001', '(', '\t', 'R', '\010', 'f', 'u', 
+'l', 'l', 'N', 'a', 'm', 'e', '\022', '\022', '\n', '\004', 't', 'y', 'p', 'e', '\030', '\003', ' ', '\001', '(', '\t', 'R', '\004', 't', 'y', 'p', 
+'e', '\022', '#', '\n', '\013', 'i', 's', '_', 'r', 'e', 'p', 'e', 'a', 't', 'e', 'd', '\030', '\004', ' ', '\001', '(', '\010', 'B', '\002', '\030', 
+'\001', 'R', '\n', 'i', 's', 'R', 'e', 'p', 'e', 'a', 't', 'e', 'd', '\022', '\032', '\n', '\010', 'r', 'e', 's', 'e', 'r', 'v', 'e', 'd', 
+'\030', '\005', ' ', '\001', '(', '\010', 'R', '\010', 'r', 'e', 's', 'e', 'r', 'v', 'e', 'd', '\022', '\032', '\n', '\010', 'r', 'e', 'p', 'e', 'a', 
+'t', 'e', 'd', '\030', '\006', ' ', '\001', '(', '\010', 'R', '\010', 'r', 'e', 'p', 'e', 'a', 't', 'e', 'd', '\"', '4', '\n', '\021', 'V', 'e', 
+'r', 'i', 'f', 'i', 'c', 'a', 't', 'i', 'o', 'n', 'S', 't', 'a', 't', 'e', '\022', '\017', '\n', '\013', 'D', 'E', 'C', 'L', 'A', 'R', 
+'A', 'T', 'I', 'O', 'N', '\020', '\000', '\022', '\016', '\n', '\n', 'U', 'N', 'V', 'E', 'R', 'I', 'F', 'I', 'E', 'D', '\020', '\001', '*', '\t', 
+'\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\301', '\006', '\n', '\024', 'F', 'i', 'e', 'l', 'd', 'D', 'e', 's', 'c', 'r', 'i', 
+'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '\022', '\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\004', 
+'n', 'a', 'm', 'e', '\022', '\026', '\n', '\006', 'n', 'u', 'm', 'b', 'e', 'r', '\030', '\003', ' ', '\001', '(', '\005', 'R', '\006', 'n', 'u', 'm', 
+'b', 'e', 'r', '\022', 'A', '\n', '\005', 'l', 'a', 'b', 'e', 'l', '\030', '\004', ' ', '\001', '(', '\016', '2', '+', '.', 'g', 'o', 'o', 'g', 
+'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 
+'o', 'r', 'P', 'r', 'o', 't', 'o', '.', 'L', 'a', 'b', 'e', 'l', 'R', '\005', 'l', 'a', 'b', 'e', 'l', '\022', '>', '\n', '\004', 't', 
+'y', 'p', 'e', '\030', '\005', ' ', '\001', '(', '\016', '2', '*', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 
+'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '.', 'T', 
+'y', 'p', 'e', 'R', '\004', 't', 'y', 'p', 'e', '\022', '\033', '\n', '\t', 't', 'y', 'p', 'e', '_', 'n', 'a', 'm', 'e', '\030', '\006', ' ', 
+'\001', '(', '\t', 'R', '\010', 't', 'y', 'p', 'e', 'N', 'a', 'm', 'e', '\022', '\032', '\n', '\010', 'e', 'x', 't', 'e', 'n', 'd', 'e', 'e', 
+'\030', '\002', ' ', '\001', '(', '\t', 'R', '\010', 'e', 'x', 't', 'e', 'n', 'd', 'e', 'e', '\022', '#', '\n', '\r', 'd', 'e', 'f', 'a', 'u', 
+'l', 't', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\007', ' ', '\001', '(', '\t', 'R', '\014', 'd', 'e', 'f', 'a', 'u', 'l', 't', 'V', 'a', 
+'l', 'u', 'e', '\022', '\037', '\n', '\013', 'o', 'n', 'e', 'o', 'f', '_', 'i', 'n', 'd', 'e', 'x', '\030', '\t', ' ', '\001', '(', '\005', 'R', 
+'\n', 'o', 'n', 'e', 'o', 'f', 'I', 'n', 'd', 'e', 'x', '\022', '\033', '\n', '\t', 'j', 's', 'o', 'n', '_', 'n', 'a', 'm', 'e', '\030', 
+'\n', ' ', '\001', '(', '\t', 'R', '\010', 'j', 's', 'o', 'n', 'N', 'a', 'm', 'e', '\022', '7', '\n', '\007', 'o', 'p', 't', 'i', 'o', 'n', 
+'s', '\030', '\010', ' ', '\001', '(', '\013', '2', '\035', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', 
+'.', 'F', 'i', 'e', 'l', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', 'R', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\022', '\'', '\n', 
+'\017', 'p', 'r', 'o', 't', 'o', '3', '_', 'o', 'p', 't', 'i', 'o', 'n', 'a', 'l', '\030', '\021', ' ', '\001', '(', '\010', 'R', '\016', 'p', 
+'r', 'o', 't', 'o', '3', 'O', 'p', 't', 'i', 'o', 'n', 'a', 'l', '\"', '\266', '\002', '\n', '\004', 'T', 'y', 'p', 'e', '\022', '\017', '\n', 
+'\013', 'T', 'Y', 'P', 'E', '_', 'D', 'O', 'U', 'B', 'L', 'E', '\020', '\001', '\022', '\016', '\n', '\n', 'T', 'Y', 'P', 'E', '_', 'F', 'L', 
+'O', 'A', 'T', '\020', '\002', '\022', '\016', '\n', '\n', 'T', 'Y', 'P', 'E', '_', 'I', 'N', 'T', '6', '4', '\020', '\003', '\022', '\017', '\n', '\013', 
+'T', 'Y', 'P', 'E', '_', 'U', 'I', 'N', 'T', '6', '4', '\020', '\004', '\022', '\016', '\n', '\n', 'T', 'Y', 'P', 'E', '_', 'I', 'N', 'T', 
+'3', '2', '\020', '\005', '\022', '\020', '\n', '\014', 'T', 'Y', 'P', 'E', '_', 'F', 'I', 'X', 'E', 'D', '6', '4', '\020', '\006', '\022', '\020', '\n', 
+'\014', 'T', 'Y', 'P', 'E', '_', 'F', 'I', 'X', 'E', 'D', '3', '2', '\020', '\007', '\022', '\r', '\n', '\t', 'T', 'Y', 'P', 'E', '_', 'B', 
+'O', 'O', 'L', '\020', '\010', '\022', '\017', '\n', '\013', 'T', 'Y', 'P', 'E', '_', 'S', 'T', 'R', 'I', 'N', 'G', '\020', '\t', '\022', '\016', '\n', 
+'\n', 'T', 'Y', 'P', 'E', '_', 'G', 'R', 'O', 'U', 'P', '\020', '\n', '\022', '\020', '\n', '\014', 'T', 'Y', 'P', 'E', '_', 'M', 'E', 'S', 
+'S', 'A', 'G', 'E', '\020', '\013', '\022', '\016', '\n', '\n', 'T', 'Y', 'P', 'E', '_', 'B', 'Y', 'T', 'E', 'S', '\020', '\014', '\022', '\017', '\n', 
+'\013', 'T', 'Y', 'P', 'E', '_', 'U', 'I', 'N', 'T', '3', '2', '\020', '\r', '\022', '\r', '\n', '\t', 'T', 'Y', 'P', 'E', '_', 'E', 'N', 
+'U', 'M', '\020', '\016', '\022', '\021', '\n', '\r', 'T', 'Y', 'P', 'E', '_', 'S', 'F', 'I', 'X', 'E', 'D', '3', '2', '\020', '\017', '\022', '\021', 
+'\n', '\r', 'T', 'Y', 'P', 'E', '_', 'S', 'F', 'I', 'X', 'E', 'D', '6', '4', '\020', '\020', '\022', '\017', '\n', '\013', 'T', 'Y', 'P', 'E', 
+'_', 'S', 'I', 'N', 'T', '3', '2', '\020', '\021', '\022', '\017', '\n', '\013', 'T', 'Y', 'P', 'E', '_', 'S', 'I', 'N', 'T', '6', '4', '\020', 
+'\022', '\"', 'C', '\n', '\005', 'L', 'a', 'b', 'e', 'l', '\022', '\022', '\n', '\016', 'L', 'A', 'B', 'E', 'L', '_', 'O', 'P', 'T', 'I', 'O', 
+'N', 'A', 'L', '\020', '\001', '\022', '\022', '\n', '\016', 'L', 'A', 'B', 'E', 'L', '_', 'R', 'E', 'Q', 'U', 'I', 'R', 'E', 'D', '\020', '\002', 
+'\022', '\022', '\n', '\016', 'L', 'A', 'B', 'E', 'L', '_', 'R', 'E', 'P', 'E', 'A', 'T', 'E', 'D', '\020', '\003', '\"', 'c', '\n', '\024', 'O', 
+'n', 'e', 'o', 'f', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '\022', '\022', '\n', '\004', 'n', 'a', 
+'m', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\004', 'n', 'a', 'm', 'e', '\022', '7', '\n', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', 
+'\030', '\002', ' ', '\001', '(', '\013', '2', '\035', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 
+'O', 'n', 'e', 'o', 'f', 'O', 'p', 't', 'i', 'o', 'n', 's', 'R', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\"', '\343', '\002', '\n', 
+'\023', 'E', 'n', 'u', 'm', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '\022', '\022', '\n', '\004', 'n', 
+'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\004', 'n', 'a', 'm', 'e', '\022', '?', '\n', '\005', 'v', 'a', 'l', 'u', 'e', '\030', 
+'\002', ' ', '\003', '(', '\013', '2', ')', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 
+'n', 'u', 'm', 'V', 'a', 'l', 'u', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', 'R', '\005', 
+'v', 'a', 'l', 'u', 'e', '\022', '6', '\n', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\030', '\003', ' ', '\001', '(', '\013', '2', '\034', '.', 
+'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'n', 'u', 'm', 'O', 'p', 't', 'i', 'o', 
+'n', 's', 'R', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\022', ']', '\n', '\016', 'r', 'e', 's', 'e', 'r', 'v', 'e', 'd', '_', 'r', 
+'a', 'n', 'g', 'e', '\030', '\004', ' ', '\003', '(', '\013', '2', '6', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 
+'b', 'u', 'f', '.', 'E', 'n', 'u', 'm', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '.', 'E', 
+'n', 'u', 'm', 'R', 'e', 's', 'e', 'r', 'v', 'e', 'd', 'R', 'a', 'n', 'g', 'e', 'R', '\r', 'r', 'e', 's', 'e', 'r', 'v', 'e', 
+'d', 'R', 'a', 'n', 'g', 'e', '\022', '#', '\n', '\r', 'r', 'e', 's', 'e', 'r', 'v', 'e', 'd', '_', 'n', 'a', 'm', 'e', '\030', '\005', 
+' ', '\003', '(', '\t', 'R', '\014', 'r', 'e', 's', 'e', 'r', 'v', 'e', 'd', 'N', 'a', 'm', 'e', '\032', ';', '\n', '\021', 'E', 'n', 'u', 
+'m', 'R', 'e', 's', 'e', 'r', 'v', 'e', 'd', 'R', 'a', 'n', 'g', 'e', '\022', '\024', '\n', '\005', 's', 't', 'a', 'r', 't', '\030', '\001', 
+' ', '\001', '(', '\005', 'R', '\005', 's', 't', 'a', 'r', 't', '\022', '\020', '\n', '\003', 'e', 'n', 'd', '\030', '\002', ' ', '\001', '(', '\005', 'R', 
+'\003', 'e', 'n', 'd', '\"', '\203', '\001', '\n', '\030', 'E', 'n', 'u', 'm', 'V', 'a', 'l', 'u', 'e', 'D', 'e', 's', 'c', 'r', 'i', 'p', 
+'t', 'o', 'r', 'P', 'r', 'o', 't', 'o', '\022', '\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\004', 'n', 
+'a', 'm', 'e', '\022', '\026', '\n', '\006', 'n', 'u', 'm', 'b', 'e', 'r', '\030', '\002', ' ', '\001', '(', '\005', 'R', '\006', 'n', 'u', 'm', 'b', 
+'e', 'r', '\022', ';', '\n', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\030', '\003', ' ', '\001', '(', '\013', '2', '!', '.', 'g', 'o', 'o', 
+'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'E', 'n', 'u', 'm', 'V', 'a', 'l', 'u', 'e', 'O', 'p', 't', 
+'i', 'o', 'n', 's', 'R', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\"', '\247', '\001', '\n', '\026', 'S', 'e', 'r', 'v', 'i', 'c', 'e', 
+'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '\022', '\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', 
+' ', '\001', '(', '\t', 'R', '\004', 'n', 'a', 'm', 'e', '\022', '>', '\n', '\006', 'm', 'e', 't', 'h', 'o', 'd', '\030', '\002', ' ', '\003', '(', 
+'\013', '2', '&', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'M', 'e', 't', 'h', 'o', 
+'d', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', 'R', '\006', 'm', 'e', 't', 'h', 'o', 'd', '\022', 
+'9', '\n', '\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\030', '\003', ' ', '\001', '(', '\013', '2', '\037', '.', 'g', 'o', 'o', 'g', 'l', 'e', 
+'.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'S', 'e', 'r', 'v', 'i', 'c', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', 'R', 
+'\007', 'o', 'p', 't', 'i', 'o', 'n', 's', '\"', '\211', '\002', '\n', '\025', 'M', 'e', 't', 'h', 'o', 'd', 'D', 'e', 's', 'c', 'r', 'i', 
+'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', '\022', '\022', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\004', 
+'n', 'a', 'm', 'e', '\022', '\035', '\n', '\n', 'i', 'n', 'p', 'u', 't', '_', 't', 'y', 'p', 'e', '\030', '\002', ' ', '\001', '(', '\t', 'R', 
+'\t', 'i', 'n', 'p', 'u', 't', 'T', 'y', 'p', 'e', '\022', '\037', '\n', '\013', 'o', 'u', 't', 'p', 'u', 't', '_', 't', 'y', 'p', 'e', 
+'\030', '\003', ' ', '\001', '(', '\t', 'R', '\n', 'o', 'u', 't', 'p', 'u', 't', 'T', 'y', 'p', 'e', '\022', '8', '\n', '\007', 'o', 'p', 't', 
+'i', 'o', 'n', 's', '\030', '\004', ' ', '\001', '(', '\013', '2', '\036', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 
+'b', 'u', 'f', '.', 'M', 'e', 't', 'h', 'o', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', 'R', '\007', 'o', 'p', 't', 'i', 'o', 'n', 
+'s', '\022', '0', '\n', '\020', 'c', 'l', 'i', 'e', 'n', 't', '_', 's', 't', 'r', 'e', 'a', 'm', 'i', 'n', 'g', '\030', '\005', ' ', '\001', 
+'(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\017', 'c', 'l', 'i', 'e', 'n', 't', 'S', 't', 'r', 'e', 'a', 'm', 'i', 'n', 
+'g', '\022', '0', '\n', '\020', 's', 'e', 'r', 'v', 'e', 'r', '_', 's', 't', 'r', 'e', 'a', 'm', 'i', 'n', 'g', '\030', '\006', ' ', '\001', 
+'(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\017', 's', 'e', 'r', 'v', 'e', 'r', 'S', 't', 'r', 'e', 'a', 'm', 'i', 'n', 
+'g', '\"', '\221', '\t', '\n', '\013', 'F', 'i', 'l', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '!', '\n', '\014', 'j', 'a', 'v', 'a', 
+'_', 'p', 'a', 'c', 'k', 'a', 'g', 'e', '\030', '\001', ' ', '\001', '(', '\t', 'R', '\013', 'j', 'a', 'v', 'a', 'P', 'a', 'c', 'k', 'a', 
+'g', 'e', '\022', '0', '\n', '\024', 'j', 'a', 'v', 'a', '_', 'o', 'u', 't', 'e', 'r', '_', 'c', 'l', 'a', 's', 's', 'n', 'a', 'm', 
+'e', '\030', '\010', ' ', '\001', '(', '\t', 'R', '\022', 'j', 'a', 'v', 'a', 'O', 'u', 't', 'e', 'r', 'C', 'l', 'a', 's', 's', 'n', 'a', 
+'m', 'e', '\022', '5', '\n', '\023', 'j', 'a', 'v', 'a', '_', 'm', 'u', 'l', 't', 'i', 'p', 'l', 'e', '_', 'f', 'i', 'l', 'e', 's', 
+'\030', '\n', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\021', 'j', 'a', 'v', 'a', 'M', 'u', 'l', 't', 'i', 'p', 
+'l', 'e', 'F', 'i', 'l', 'e', 's', '\022', 'D', '\n', '\035', 'j', 'a', 'v', 'a', '_', 'g', 'e', 'n', 'e', 'r', 'a', 't', 'e', '_', 
+'e', 'q', 'u', 'a', 'l', 's', '_', 'a', 'n', 'd', '_', 'h', 'a', 's', 'h', '\030', '\024', ' ', '\001', '(', '\010', 'B', '\002', '\030', '\001', 
+'R', '\031', 'j', 'a', 'v', 'a', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'E', 'q', 'u', 'a', 'l', 's', 'A', 'n', 'd', 'H', 'a', 
+'s', 'h', '\022', ':', '\n', '\026', 'j', 'a', 'v', 'a', '_', 's', 't', 'r', 'i', 'n', 'g', '_', 'c', 'h', 'e', 'c', 'k', '_', 'u', 
+'t', 'f', '8', '\030', '\033', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\023', 'j', 'a', 'v', 'a', 'S', 't', 'r', 
+'i', 'n', 'g', 'C', 'h', 'e', 'c', 'k', 'U', 't', 'f', '8', '\022', 'S', '\n', '\014', 'o', 'p', 't', 'i', 'm', 'i', 'z', 'e', '_', 
+'f', 'o', 'r', '\030', '\t', ' ', '\001', '(', '\016', '2', ')', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 
+'u', 'f', '.', 'F', 'i', 'l', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'O', 'p', 't', 'i', 'm', 'i', 'z', 'e', 'M', 'o', 
+'d', 'e', ':', '\005', 'S', 'P', 'E', 'E', 'D', 'R', '\013', 'o', 'p', 't', 'i', 'm', 'i', 'z', 'e', 'F', 'o', 'r', '\022', '\035', '\n', 
+'\n', 'g', 'o', '_', 'p', 'a', 'c', 'k', 'a', 'g', 'e', '\030', '\013', ' ', '\001', '(', '\t', 'R', '\t', 'g', 'o', 'P', 'a', 'c', 'k', 
+'a', 'g', 'e', '\022', '5', '\n', '\023', 'c', 'c', '_', 'g', 'e', 'n', 'e', 'r', 'i', 'c', '_', 's', 'e', 'r', 'v', 'i', 'c', 'e', 
+'s', '\030', '\020', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\021', 'c', 'c', 'G', 'e', 'n', 'e', 'r', 'i', 'c', 
+'S', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\022', '9', '\n', '\025', 'j', 'a', 'v', 'a', '_', 'g', 'e', 'n', 'e', 'r', 'i', 'c', '_', 
+'s', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\030', '\021', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\023', 'j', 'a', 
+'v', 'a', 'G', 'e', 'n', 'e', 'r', 'i', 'c', 'S', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\022', '5', '\n', '\023', 'p', 'y', '_', 'g', 
+'e', 'n', 'e', 'r', 'i', 'c', '_', 's', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\030', '\022', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 
+'l', 's', 'e', 'R', '\021', 'p', 'y', 'G', 'e', 'n', 'e', 'r', 'i', 'c', 'S', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\022', '7', '\n', 
+'\024', 'p', 'h', 'p', '_', 'g', 'e', 'n', 'e', 'r', 'i', 'c', '_', 's', 'e', 'r', 'v', 'i', 'c', 'e', 's', '\030', '*', ' ', '\001', 
+'(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\022', 'p', 'h', 'p', 'G', 'e', 'n', 'e', 'r', 'i', 'c', 'S', 'e', 'r', 'v', 
+'i', 'c', 'e', 's', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '\027', ' ', '\001', '(', '\010', ':', 
+'\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', '.', '\n', '\020', 'c', 'c', '_', 
+'e', 'n', 'a', 'b', 'l', 'e', '_', 'a', 'r', 'e', 'n', 'a', 's', '\030', '\037', ' ', '\001', '(', '\010', ':', '\004', 't', 'r', 'u', 'e', 
+'R', '\016', 'c', 'c', 'E', 'n', 'a', 'b', 'l', 'e', 'A', 'r', 'e', 'n', 'a', 's', '\022', '*', '\n', '\021', 'o', 'b', 'j', 'c', '_', 
+'c', 'l', 'a', 's', 's', '_', 'p', 'r', 'e', 'f', 'i', 'x', '\030', '$', ' ', '\001', '(', '\t', 'R', '\017', 'o', 'b', 'j', 'c', 'C', 
+'l', 'a', 's', 's', 'P', 'r', 'e', 'f', 'i', 'x', '\022', ')', '\n', '\020', 'c', 's', 'h', 'a', 'r', 'p', '_', 'n', 'a', 'm', 'e', 
+'s', 'p', 'a', 'c', 'e', '\030', '%', ' ', '\001', '(', '\t', 'R', '\017', 'c', 's', 'h', 'a', 'r', 'p', 'N', 'a', 'm', 'e', 's', 'p', 
+'a', 'c', 'e', '\022', '!', '\n', '\014', 's', 'w', 'i', 'f', 't', '_', 'p', 'r', 'e', 'f', 'i', 'x', '\030', '\'', ' ', '\001', '(', '\t', 
+'R', '\013', 's', 'w', 'i', 'f', 't', 'P', 'r', 'e', 'f', 'i', 'x', '\022', '(', '\n', '\020', 'p', 'h', 'p', '_', 'c', 'l', 'a', 's', 
+'s', '_', 'p', 'r', 'e', 'f', 'i', 'x', '\030', '(', ' ', '\001', '(', '\t', 'R', '\016', 'p', 'h', 'p', 'C', 'l', 'a', 's', 's', 'P', 
+'r', 'e', 'f', 'i', 'x', '\022', '#', '\n', '\r', 'p', 'h', 'p', '_', 'n', 'a', 'm', 'e', 's', 'p', 'a', 'c', 'e', '\030', ')', ' ', 
+'\001', '(', '\t', 'R', '\014', 'p', 'h', 'p', 'N', 'a', 'm', 'e', 's', 'p', 'a', 'c', 'e', '\022', '4', '\n', '\026', 'p', 'h', 'p', '_', 
+'m', 'e', 't', 'a', 'd', 'a', 't', 'a', '_', 'n', 'a', 'm', 'e', 's', 'p', 'a', 'c', 'e', '\030', ',', ' ', '\001', '(', '\t', 'R', 
+'\024', 'p', 'h', 'p', 'M', 'e', 't', 'a', 'd', 'a', 't', 'a', 'N', 'a', 'm', 'e', 's', 'p', 'a', 'c', 'e', '\022', '!', '\n', '\014', 
+'r', 'u', 'b', 'y', '_', 'p', 'a', 'c', 'k', 'a', 'g', 'e', '\030', '-', ' ', '\001', '(', '\t', 'R', '\013', 'r', 'u', 'b', 'y', 'P', 
+'a', 'c', 'k', 'a', 'g', 'e', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 
+'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 
+'t', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 
+'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '\"', ':', '\n', '\014', 
+'O', 'p', 't', 'i', 'm', 'i', 'z', 'e', 'M', 'o', 'd', 'e', '\022', '\t', '\n', '\005', 'S', 'P', 'E', 'E', 'D', '\020', '\001', '\022', '\r', 
+'\n', '\t', 'C', 'O', 'D', 'E', '_', 'S', 'I', 'Z', 'E', '\020', '\002', '\022', '\020', '\n', '\014', 'L', 'I', 'T', 'E', '_', 'R', 'U', 'N', 
+'T', 'I', 'M', 'E', '\020', '\003', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', 'J', '\004', '\010', '&', '\020', '\'', '\"', '\273', 
+'\003', '\n', '\016', 'M', 'e', 's', 's', 'a', 'g', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '<', '\n', '\027', 'm', 'e', 's', 's', 
+'a', 'g', 'e', '_', 's', 'e', 't', '_', 'w', 'i', 'r', 'e', '_', 'f', 'o', 'r', 'm', 'a', 't', '\030', '\001', ' ', '\001', '(', '\010', 
+':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\024', 'm', 'e', 's', 's', 'a', 'g', 'e', 'S', 'e', 't', 'W', 'i', 'r', 'e', 'F', 'o', 
+'r', 'm', 'a', 't', '\022', 'L', '\n', '\037', 'n', 'o', '_', 's', 't', 'a', 'n', 'd', 'a', 'r', 'd', '_', 'd', 'e', 's', 'c', 'r', 
+'i', 'p', 't', 'o', 'r', '_', 'a', 'c', 'c', 'e', 's', 's', 'o', 'r', '\030', '\002', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 
+'s', 'e', 'R', '\034', 'n', 'o', 'S', 't', 'a', 'n', 'd', 'a', 'r', 'd', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'A', 
+'c', 'c', 'e', 's', 's', 'o', 'r', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '\003', ' ', '\001', 
+'(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', '\033', '\n', '\t', 
+'m', 'a', 'p', '_', 'e', 'n', 't', 'r', 'y', '\030', '\007', ' ', '\001', '(', '\010', 'R', '\010', 'm', 'a', 'p', 'E', 'n', 't', 'r', 'y', 
+'\022', 'V', '\n', '&', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '_', 'l', 'e', 'g', 'a', 'c', 'y', '_', 'j', 's', 'o', 
+'n', '_', 'f', 'i', 'e', 'l', 'd', '_', 'c', 'o', 'n', 'f', 'l', 'i', 'c', 't', 's', '\030', '\013', ' ', '\001', '(', '\010', 'B', '\002', 
+'\030', '\001', 'R', '\"', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', 'L', 'e', 'g', 'a', 'c', 'y', 'J', 's', 'o', 'n', 'F', 
+'i', 'e', 'l', 'd', 'C', 'o', 'n', 'f', 'l', 'i', 'c', 't', 's', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 
+'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 
+'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 
+'d', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 
+'i', 'o', 'n', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', 'J', '\004', '\010', '\004', '\020', '\005', 'J', '\004', '\010', '\005', '\020', 
+'\006', 'J', '\004', '\010', '\006', '\020', '\007', 'J', '\004', '\010', '\010', '\020', '\t', 'J', '\004', '\010', '\t', '\020', '\n', '\"', '\205', '\t', '\n', '\014', 'F', 
+'i', 'e', 'l', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', 'A', '\n', '\005', 'c', 't', 'y', 'p', 'e', '\030', '\001', ' ', '\001', '(', 
+'\016', '2', '#', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 
+'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'C', 'T', 'y', 'p', 'e', ':', '\006', 'S', 'T', 'R', 'I', 'N', 'G', 'R', '\005', 'c', 't', 
+'y', 'p', 'e', '\022', '\026', '\n', '\006', 'p', 'a', 'c', 'k', 'e', 'd', '\030', '\002', ' ', '\001', '(', '\010', 'R', '\006', 'p', 'a', 'c', 'k', 
+'e', 'd', '\022', 'G', '\n', '\006', 'j', 's', 't', 'y', 'p', 'e', '\030', '\006', ' ', '\001', '(', '\016', '2', '$', '.', 'g', 'o', 'o', 'g', 
+'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 
+'J', 'S', 'T', 'y', 'p', 'e', ':', '\t', 'J', 'S', '_', 'N', 'O', 'R', 'M', 'A', 'L', 'R', '\006', 'j', 's', 't', 'y', 'p', 'e', 
+'\022', '\031', '\n', '\004', 'l', 'a', 'z', 'y', '\030', '\005', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\004', 'l', 'a', 
+'z', 'y', '\022', '.', '\n', '\017', 'u', 'n', 'v', 'e', 'r', 'i', 'f', 'i', 'e', 'd', '_', 'l', 'a', 'z', 'y', '\030', '\017', ' ', '\001', 
+'(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\016', 'u', 'n', 'v', 'e', 'r', 'i', 'f', 'i', 'e', 'd', 'L', 'a', 'z', 'y', 
+'\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '\003', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 
+'s', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', '\031', '\n', '\004', 'w', 'e', 'a', 'k', '\030', '\n', ' ', 
+'\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\004', 'w', 'e', 'a', 'k', '\022', '(', '\n', '\014', 'd', 'e', 'b', 'u', 'g', 
+'_', 'r', 'e', 'd', 'a', 'c', 't', '\030', '\020', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\013', 'd', 'e', 'b', 
+'u', 'g', 'R', 'e', 'd', 'a', 'c', 't', '\022', 'K', '\n', '\t', 'r', 'e', 't', 'e', 'n', 't', 'i', 'o', 'n', '\030', '\021', ' ', '\001', 
+'(', '\016', '2', '-', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 
+'d', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'O', 'p', 't', 'i', 'o', 'n', 'R', 'e', 't', 'e', 'n', 't', 'i', 'o', 'n', 'R', 
+'\t', 'r', 'e', 't', 'e', 'n', 't', 'i', 'o', 'n', '\022', 'J', '\n', '\006', 't', 'a', 'r', 'g', 'e', 't', '\030', '\022', ' ', '\001', '(', 
+'\016', '2', '.', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 
+'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'O', 'p', 't', 'i', 'o', 'n', 'T', 'a', 'r', 'g', 'e', 't', 'T', 'y', 'p', 'e', 'B', 
+'\002', '\030', '\001', 'R', '\006', 't', 'a', 'r', 'g', 'e', 't', '\022', 'H', '\n', '\007', 't', 'a', 'r', 'g', 'e', 't', 's', '\030', '\023', ' ', 
+'\003', '(', '\016', '2', '.', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 
+'l', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'O', 'p', 't', 'i', 'o', 'n', 'T', 'a', 'r', 'g', 'e', 't', 'T', 'y', 'p', 
+'e', 'R', '\007', 't', 'a', 'r', 'g', 'e', 't', 's', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 
+'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', 
+'.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 
+'t', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 
+'\"', '/', '\n', '\005', 'C', 'T', 'y', 'p', 'e', '\022', '\n', '\n', '\006', 'S', 'T', 'R', 'I', 'N', 'G', '\020', '\000', '\022', '\010', '\n', '\004', 
+'C', 'O', 'R', 'D', '\020', '\001', '\022', '\020', '\n', '\014', 'S', 'T', 'R', 'I', 'N', 'G', '_', 'P', 'I', 'E', 'C', 'E', '\020', '\002', '\"', 
+'5', '\n', '\006', 'J', 'S', 'T', 'y', 'p', 'e', '\022', '\r', '\n', '\t', 'J', 'S', '_', 'N', 'O', 'R', 'M', 'A', 'L', '\020', '\000', '\022', 
+'\r', '\n', '\t', 'J', 'S', '_', 'S', 'T', 'R', 'I', 'N', 'G', '\020', '\001', '\022', '\r', '\n', '\t', 'J', 'S', '_', 'N', 'U', 'M', 'B', 
+'E', 'R', '\020', '\002', '\"', 'U', '\n', '\017', 'O', 'p', 't', 'i', 'o', 'n', 'R', 'e', 't', 'e', 'n', 't', 'i', 'o', 'n', '\022', '\025', 
+'\n', '\021', 'R', 'E', 'T', 'E', 'N', 'T', 'I', 'O', 'N', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\025', '\n', '\021', 
+'R', 'E', 'T', 'E', 'N', 'T', 'I', 'O', 'N', '_', 'R', 'U', 'N', 'T', 'I', 'M', 'E', '\020', '\001', '\022', '\024', '\n', '\020', 'R', 'E', 
+'T', 'E', 'N', 'T', 'I', 'O', 'N', '_', 'S', 'O', 'U', 'R', 'C', 'E', '\020', '\002', '\"', '\214', '\002', '\n', '\020', 'O', 'p', 't', 'i', 
+'o', 'n', 'T', 'a', 'r', 'g', 'e', 't', 'T', 'y', 'p', 'e', '\022', '\027', '\n', '\023', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 
+'P', 'E', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\024', '\n', '\020', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 
+'P', 'E', '_', 'F', 'I', 'L', 'E', '\020', '\001', '\022', '\037', '\n', '\033', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 
+'E', 'X', 'T', 'E', 'N', 'S', 'I', 'O', 'N', '_', 'R', 'A', 'N', 'G', 'E', '\020', '\002', '\022', '\027', '\n', '\023', 'T', 'A', 'R', 'G', 
+'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'M', 'E', 'S', 'S', 'A', 'G', 'E', '\020', '\003', '\022', '\025', '\n', '\021', 'T', 'A', 'R', 'G', 
+'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'F', 'I', 'E', 'L', 'D', '\020', '\004', '\022', '\025', '\n', '\021', 'T', 'A', 'R', 'G', 'E', 'T', 
+'_', 'T', 'Y', 'P', 'E', '_', 'O', 'N', 'E', 'O', 'F', '\020', '\005', '\022', '\024', '\n', '\020', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 
+'Y', 'P', 'E', '_', 'E', 'N', 'U', 'M', '\020', '\006', '\022', '\032', '\n', '\026', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', 
+'_', 'E', 'N', 'U', 'M', '_', 'E', 'N', 'T', 'R', 'Y', '\020', '\007', '\022', '\027', '\n', '\023', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 
+'Y', 'P', 'E', '_', 'S', 'E', 'R', 'V', 'I', 'C', 'E', '\020', '\010', '\022', '\026', '\n', '\022', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 
+'Y', 'P', 'E', '_', 'M', 'E', 'T', 'H', 'O', 'D', '\020', '\t', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', 'J', '\004', 
+'\010', '\004', '\020', '\005', '\"', 's', '\n', '\014', 'O', 'n', 'e', 'o', 'f', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', 'X', '\n', '\024', 'u', 
+'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', 
+'\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 
+'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 
+'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\230', '\002', '\n', 
+'\013', 'E', 'n', 'u', 'm', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '\037', '\n', '\013', 'a', 'l', 'l', 'o', 'w', '_', 'a', 'l', 'i', 
+'a', 's', '\030', '\002', ' ', '\001', '(', '\010', 'R', '\n', 'a', 'l', 'l', 'o', 'w', 'A', 'l', 'i', 'a', 's', '\022', '%', '\n', '\n', 'd', 
+'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '\003', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 
+'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', 'V', '\n', '&', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '_', 'l', 
+'e', 'g', 'a', 'c', 'y', '_', 'j', 's', 'o', 'n', '_', 'f', 'i', 'e', 'l', 'd', '_', 'c', 'o', 'n', 'f', 'l', 'i', 'c', 't', 
+'s', '\030', '\006', ' ', '\001', '(', '\010', 'B', '\002', '\030', '\001', 'R', '\"', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', 'L', 'e', 
+'g', 'a', 'c', 'y', 'J', 's', 'o', 'n', 'F', 'i', 'e', 'l', 'd', 'C', 'o', 'n', 'f', 'l', 'i', 'c', 't', 's', '\022', 'X', '\n', 
 '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', 
 '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 
 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 
-'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '\"', ':', '\n', '\014', 'O', 'p', 't', 'i', 'm', 'i', 'z', 'e', 'M', 
-'o', 'd', 'e', '\022', '\t', '\n', '\005', 'S', 'P', 'E', 'E', 'D', '\020', '\001', '\022', '\r', '\n', '\t', 'C', 'O', 'D', 'E', '_', 'S', 'I', 
-'Z', 'E', '\020', '\002', '\022', '\020', '\n', '\014', 'L', 'I', 'T', 'E', '_', 'R', 'U', 'N', 'T', 'I', 'M', 'E', '\020', '\003', '*', '\t', '\010', 
-'\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', 'J', '\004', '\010', '&', '\020', '\'', '\"', '\273', '\003', '\n', '\016', 'M', 'e', 's', 's', 'a', 'g', 
-'e', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '<', '\n', '\027', 'm', 'e', 's', 's', 'a', 'g', 'e', '_', 's', 'e', 't', '_', 'w', 
-'i', 'r', 'e', '_', 'f', 'o', 'r', 'm', 'a', 't', '\030', '\001', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\024', 
-'m', 'e', 's', 's', 'a', 'g', 'e', 'S', 'e', 't', 'W', 'i', 'r', 'e', 'F', 'o', 'r', 'm', 'a', 't', '\022', 'L', '\n', '\037', 'n', 
-'o', '_', 's', 't', 'a', 'n', 'd', 'a', 'r', 'd', '_', 'd', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', '_', 'a', 'c', 'c', 
-'e', 's', 's', 'o', 'r', '\030', '\002', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\034', 'n', 'o', 'S', 't', 'a', 
-'n', 'd', 'a', 'r', 'd', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'A', 'c', 'c', 'e', 's', 's', 'o', 'r', '\022', '%', 
-'\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '\003', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 
-'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', '\033', '\n', '\t', 'm', 'a', 'p', '_', 'e', 'n', 't', 'r', 'y', 
-'\030', '\007', ' ', '\001', '(', '\010', 'R', '\010', 'm', 'a', 'p', 'E', 'n', 't', 'r', 'y', '\022', 'V', '\n', '&', 'd', 'e', 'p', 'r', 'e', 
-'c', 'a', 't', 'e', 'd', '_', 'l', 'e', 'g', 'a', 'c', 'y', '_', 'j', 's', 'o', 'n', '_', 'f', 'i', 'e', 'l', 'd', '_', 'c', 
-'o', 'n', 'f', 'l', 'i', 'c', 't', 's', '\030', '\013', ' ', '\001', '(', '\010', 'B', '\002', '\030', '\001', 'R', '\"', 'd', 'e', 'p', 'r', 'e', 
-'c', 'a', 't', 'e', 'd', 'L', 'e', 'g', 'a', 'c', 'y', 'J', 's', 'o', 'n', 'F', 'i', 'e', 'l', 'd', 'C', 'o', 'n', 'f', 'l', 
-'i', 'c', 't', 's', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 
-'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 
-'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 
-'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', '\t', '\010', '\350', '\007', '\020', 
-'\200', '\200', '\200', '\200', '\002', 'J', '\004', '\010', '\004', '\020', '\005', 'J', '\004', '\010', '\005', '\020', '\006', 'J', '\004', '\010', '\006', '\020', '\007', 'J', '\004', 
-'\010', '\010', '\020', '\t', 'J', '\004', '\010', '\t', '\020', '\n', '\"', '\267', '\010', '\n', '\014', 'F', 'i', 'e', 'l', 'd', 'O', 'p', 't', 'i', 'o', 
-'n', 's', '\022', 'A', '\n', '\005', 'c', 't', 'y', 'p', 'e', '\030', '\001', ' ', '\001', '(', '\016', '2', '#', '.', 'g', 'o', 'o', 'g', 'l', 
-'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'C', 
-'T', 'y', 'p', 'e', ':', '\006', 'S', 'T', 'R', 'I', 'N', 'G', 'R', '\005', 'c', 't', 'y', 'p', 'e', '\022', '\026', '\n', '\006', 'p', 'a', 
-'c', 'k', 'e', 'd', '\030', '\002', ' ', '\001', '(', '\010', 'R', '\006', 'p', 'a', 'c', 'k', 'e', 'd', '\022', 'G', '\n', '\006', 'j', 's', 't', 
-'y', 'p', 'e', '\030', '\006', ' ', '\001', '(', '\016', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 
-'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'J', 'S', 'T', 'y', 'p', 'e', ':', '\t', 'J', 
-'S', '_', 'N', 'O', 'R', 'M', 'A', 'L', 'R', '\006', 'j', 's', 't', 'y', 'p', 'e', '\022', '\031', '\n', '\004', 'l', 'a', 'z', 'y', '\030', 
-'\005', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\004', 'l', 'a', 'z', 'y', '\022', '.', '\n', '\017', 'u', 'n', 'v', 
-'e', 'r', 'i', 'f', 'i', 'e', 'd', '_', 'l', 'a', 'z', 'y', '\030', '\017', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 
-'R', '\016', 'u', 'n', 'v', 'e', 'r', 'i', 'f', 'i', 'e', 'd', 'L', 'a', 'z', 'y', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 
-'c', 'a', 't', 'e', 'd', '\030', '\003', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 
-'c', 'a', 't', 'e', 'd', '\022', '\031', '\n', '\004', 'w', 'e', 'a', 'k', '\030', '\n', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 
-'e', 'R', '\004', 'w', 'e', 'a', 'k', '\022', '(', '\n', '\014', 'd', 'e', 'b', 'u', 'g', '_', 'r', 'e', 'd', 'a', 'c', 't', '\030', '\020', 
-' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\013', 'd', 'e', 'b', 'u', 'g', 'R', 'e', 'd', 'a', 'c', 't', '\022', 
-'K', '\n', '\t', 'r', 'e', 't', 'e', 'n', 't', 'i', 'o', 'n', '\030', '\021', ' ', '\001', '(', '\016', '2', '-', '.', 'g', 'o', 'o', 'g', 
-'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 
-'O', 'p', 't', 'i', 'o', 'n', 'R', 'e', 't', 'e', 'n', 't', 'i', 'o', 'n', 'R', '\t', 'r', 'e', 't', 'e', 'n', 't', 'i', 'o', 
-'n', '\022', 'F', '\n', '\006', 't', 'a', 'r', 'g', 'e', 't', '\030', '\022', ' ', '\001', '(', '\016', '2', '.', '.', 'g', 'o', 'o', 'g', 'l', 
-'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'F', 'i', 'e', 'l', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'O', 
-'p', 't', 'i', 'o', 'n', 'T', 'a', 'r', 'g', 'e', 't', 'T', 'y', 'p', 'e', 'R', '\006', 't', 'a', 'r', 'g', 'e', 't', '\022', 'X', 
+'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', 'J', '\004', 
+'\010', '\005', '\020', '\006', '\"', '\236', '\001', '\n', '\020', 'E', 'n', 'u', 'm', 'V', 'a', 'l', 'u', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', 
+'\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '\001', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 
+'s', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 
+'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 
+'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 
+'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 
+'t', 'i', 'o', 'n', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\234', '\001', '\n', '\016', 'S', 'e', 'r', 'v', 'i', 
+'c', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '!', 
+' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', 'X', 
 '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', 
 ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 
 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 
-'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '\"', '/', '\n', '\005', 'C', 'T', 'y', 'p', 'e', '\022', '\n', '\n', 
-'\006', 'S', 'T', 'R', 'I', 'N', 'G', '\020', '\000', '\022', '\010', '\n', '\004', 'C', 'O', 'R', 'D', '\020', '\001', '\022', '\020', '\n', '\014', 'S', 'T', 
-'R', 'I', 'N', 'G', '_', 'P', 'I', 'E', 'C', 'E', '\020', '\002', '\"', '5', '\n', '\006', 'J', 'S', 'T', 'y', 'p', 'e', '\022', '\r', '\n', 
-'\t', 'J', 'S', '_', 'N', 'O', 'R', 'M', 'A', 'L', '\020', '\000', '\022', '\r', '\n', '\t', 'J', 'S', '_', 'S', 'T', 'R', 'I', 'N', 'G', 
-'\020', '\001', '\022', '\r', '\n', '\t', 'J', 'S', '_', 'N', 'U', 'M', 'B', 'E', 'R', '\020', '\002', '\"', 'U', '\n', '\017', 'O', 'p', 't', 'i', 
-'o', 'n', 'R', 'e', 't', 'e', 'n', 't', 'i', 'o', 'n', '\022', '\025', '\n', '\021', 'R', 'E', 'T', 'E', 'N', 'T', 'I', 'O', 'N', '_', 
-'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\025', '\n', '\021', 'R', 'E', 'T', 'E', 'N', 'T', 'I', 'O', 'N', '_', 'R', 'U', 
-'N', 'T', 'I', 'M', 'E', '\020', '\001', '\022', '\024', '\n', '\020', 'R', 'E', 'T', 'E', 'N', 'T', 'I', 'O', 'N', '_', 'S', 'O', 'U', 'R', 
-'C', 'E', '\020', '\002', '\"', '\214', '\002', '\n', '\020', 'O', 'p', 't', 'i', 'o', 'n', 'T', 'a', 'r', 'g', 'e', 't', 'T', 'y', 'p', 'e', 
-'\022', '\027', '\n', '\023', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', 
-'\022', '\024', '\n', '\020', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'F', 'I', 'L', 'E', '\020', '\001', '\022', '\037', '\n', 
-'\033', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'E', 'X', 'T', 'E', 'N', 'S', 'I', 'O', 'N', '_', 'R', 'A', 
-'N', 'G', 'E', '\020', '\002', '\022', '\027', '\n', '\023', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'M', 'E', 'S', 'S', 
-'A', 'G', 'E', '\020', '\003', '\022', '\025', '\n', '\021', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'F', 'I', 'E', 'L', 
-'D', '\020', '\004', '\022', '\025', '\n', '\021', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'O', 'N', 'E', 'O', 'F', '\020', 
-'\005', '\022', '\024', '\n', '\020', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'E', 'N', 'U', 'M', '\020', '\006', '\022', '\032', 
-'\n', '\026', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'E', 'N', 'U', 'M', '_', 'E', 'N', 'T', 'R', 'Y', '\020', 
-'\007', '\022', '\027', '\n', '\023', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'S', 'E', 'R', 'V', 'I', 'C', 'E', '\020', 
-'\010', '\022', '\026', '\n', '\022', 'T', 'A', 'R', 'G', 'E', 'T', '_', 'T', 'Y', 'P', 'E', '_', 'M', 'E', 'T', 'H', 'O', 'D', '\020', '\t', 
-'*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', 'J', '\004', '\010', '\004', '\020', '\005', '\"', 's', '\n', '\014', 'O', 'n', 'e', 'o', 
-'f', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 
-'_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 
-'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 
-'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', '\t', 
-'\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\230', '\002', '\n', '\013', 'E', 'n', 'u', 'm', 'O', 'p', 't', 'i', 'o', 'n', 's', 
-'\022', '\037', '\n', '\013', 'a', 'l', 'l', 'o', 'w', '_', 'a', 'l', 'i', 'a', 's', '\030', '\002', ' ', '\001', '(', '\010', 'R', '\n', 'a', 'l', 
-'l', 'o', 'w', 'A', 'l', 'i', 'a', 's', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '\003', ' ', 
-'\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', 'V', '\n', 
-'&', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '_', 'l', 'e', 'g', 'a', 'c', 'y', '_', 'j', 's', 'o', 'n', '_', 'f', 
-'i', 'e', 'l', 'd', '_', 'c', 'o', 'n', 'f', 'l', 'i', 'c', 't', 's', '\030', '\006', ' ', '\001', '(', '\010', 'B', '\002', '\030', '\001', 'R', 
-'\"', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', 'L', 'e', 'g', 'a', 'c', 'y', 'J', 's', 'o', 'n', 'F', 'i', 'e', 'l', 
-'d', 'C', 'o', 'n', 'f', 'l', 'i', 'c', 't', 's', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 
-'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', 
-'.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 
-'t', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 
-'*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', 'J', '\004', '\010', '\005', '\020', '\006', '\"', '\236', '\001', '\n', '\020', 'E', 'n', 'u', 
-'m', 'V', 'a', 'l', 'u', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 
-'e', 'd', '\030', '\001', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 
-'e', 'd', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 
-'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
-'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 
-'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', 
-'\200', '\200', '\002', '\"', '\234', '\001', '\n', '\016', 'S', 'e', 'r', 'v', 'i', 'c', 'e', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '%', '\n', 
-'\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '!', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', 
-'\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 
-'t', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 
+'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', 
+'\340', '\002', '\n', '\r', 'M', 'e', 't', 'h', 'o', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 
+'e', 'c', 'a', 't', 'e', 'd', '\030', '!', ' ', '\001', '(', '\010', ':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 
+'e', 'c', 'a', 't', 'e', 'd', '\022', 'q', '\n', '\021', 'i', 'd', 'e', 'm', 'p', 'o', 't', 'e', 'n', 'c', 'y', '_', 'l', 'e', 'v', 
+'e', 'l', '\030', '\"', ' ', '\001', '(', '\016', '2', '/', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 
+'f', '.', 'M', 'e', 't', 'h', 'o', 'd', 'O', 'p', 't', 'i', 'o', 'n', 's', '.', 'I', 'd', 'e', 'm', 'p', 'o', 't', 'e', 'n', 
+'c', 'y', 'L', 'e', 'v', 'e', 'l', ':', '\023', 'I', 'D', 'E', 'M', 'P', 'O', 'T', 'E', 'N', 'C', 'Y', '_', 'U', 'N', 'K', 'N', 
+'O', 'W', 'N', 'R', '\020', 'i', 'd', 'e', 'm', 'p', 'o', 't', 'e', 'n', 'c', 'y', 'L', 'e', 'v', 'e', 'l', '\022', 'X', '\n', '\024', 
+'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', 
+'(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 
+'t', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 
+'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '\"', 'P', '\n', '\020', 'I', 'd', 'e', 'm', 'p', 'o', 't', 'e', 'n', 'c', 
+'y', 'L', 'e', 'v', 'e', 'l', '\022', '\027', '\n', '\023', 'I', 'D', 'E', 'M', 'P', 'O', 'T', 'E', 'N', 'C', 'Y', '_', 'U', 'N', 'K', 
+'N', 'O', 'W', 'N', '\020', '\000', '\022', '\023', '\n', '\017', 'N', 'O', '_', 'S', 'I', 'D', 'E', '_', 'E', 'F', 'F', 'E', 'C', 'T', 'S', 
+'\020', '\001', '\022', '\016', '\n', '\n', 'I', 'D', 'E', 'M', 'P', 'O', 'T', 'E', 'N', 'T', '\020', '\002', '*', '\t', '\010', '\350', '\007', '\020', '\200', 
+'\200', '\200', '\200', '\002', '\"', '\232', '\003', '\n', '\023', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 
+'i', 'o', 'n', '\022', 'A', '\n', '\004', 'n', 'a', 'm', 'e', '\030', '\002', ' ', '\003', '(', '\013', '2', '-', '.', 'g', 'o', 'o', 'g', 'l', 
 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 
-'p', 't', 'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 
-'n', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\340', '\002', '\n', '\r', 'M', 'e', 't', 'h', 'o', 'd', 'O', 'p', 
-'t', 'i', 'o', 'n', 's', '\022', '%', '\n', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\030', '!', ' ', '\001', '(', '\010', 
-':', '\005', 'f', 'a', 'l', 's', 'e', 'R', '\n', 'd', 'e', 'p', 'r', 'e', 'c', 'a', 't', 'e', 'd', '\022', 'q', '\n', '\021', 'i', 'd', 
-'e', 'm', 'p', 'o', 't', 'e', 'n', 'c', 'y', '_', 'l', 'e', 'v', 'e', 'l', '\030', '\"', ' ', '\001', '(', '\016', '2', '/', '.', 'g', 
-'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'M', 'e', 't', 'h', 'o', 'd', 'O', 'p', 't', 'i', 
-'o', 'n', 's', '.', 'I', 'd', 'e', 'm', 'p', 'o', 't', 'e', 'n', 'c', 'y', 'L', 'e', 'v', 'e', 'l', ':', '\023', 'I', 'D', 'E', 
-'M', 'P', 'O', 'T', 'E', 'N', 'C', 'Y', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', 'R', '\020', 'i', 'd', 'e', 'm', 'p', 'o', 't', 
-'e', 'n', 'c', 'y', 'L', 'e', 'v', 'e', 'l', '\022', 'X', '\n', '\024', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 
-'d', '_', 'o', 'p', 't', 'i', 'o', 'n', '\030', '\347', '\007', ' ', '\003', '(', '\013', '2', '$', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 
-'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 
-'i', 'o', 'n', 'R', '\023', 'u', 'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '\"', 
-'P', '\n', '\020', 'I', 'd', 'e', 'm', 'p', 'o', 't', 'e', 'n', 'c', 'y', 'L', 'e', 'v', 'e', 'l', '\022', '\027', '\n', '\023', 'I', 'D', 
-'E', 'M', 'P', 'O', 'T', 'E', 'N', 'C', 'Y', '_', 'U', 'N', 'K', 'N', 'O', 'W', 'N', '\020', '\000', '\022', '\023', '\n', '\017', 'N', 'O', 
-'_', 'S', 'I', 'D', 'E', '_', 'E', 'F', 'F', 'E', 'C', 'T', 'S', '\020', '\001', '\022', '\016', '\n', '\n', 'I', 'D', 'E', 'M', 'P', 'O', 
-'T', 'E', 'N', 'T', '\020', '\002', '*', '\t', '\010', '\350', '\007', '\020', '\200', '\200', '\200', '\200', '\002', '\"', '\232', '\003', '\n', '\023', 'U', 'n', 'i', 
-'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '\022', 'A', '\n', '\004', 'n', 'a', 'm', 'e', '\030', 
-'\002', ' ', '\003', '(', '\013', '2', '-', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'U', 
-'n', 'i', 'n', 't', 'e', 'r', 'p', 'r', 'e', 't', 'e', 'd', 'O', 'p', 't', 'i', 'o', 'n', '.', 'N', 'a', 'm', 'e', 'P', 'a', 
-'r', 't', 'R', '\004', 'n', 'a', 'm', 'e', '\022', ')', '\n', '\020', 'i', 'd', 'e', 'n', 't', 'i', 'f', 'i', 'e', 'r', '_', 'v', 'a', 
-'l', 'u', 'e', '\030', '\003', ' ', '\001', '(', '\t', 'R', '\017', 'i', 'd', 'e', 'n', 't', 'i', 'f', 'i', 'e', 'r', 'V', 'a', 'l', 'u', 
-'e', '\022', ',', '\n', '\022', 'p', 'o', 's', 'i', 't', 'i', 'v', 'e', '_', 'i', 'n', 't', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\004', 
-' ', '\001', '(', '\004', 'R', '\020', 'p', 'o', 's', 'i', 't', 'i', 'v', 'e', 'I', 'n', 't', 'V', 'a', 'l', 'u', 'e', '\022', ',', '\n', 
-'\022', 'n', 'e', 'g', 'a', 't', 'i', 'v', 'e', '_', 'i', 'n', 't', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\005', ' ', '\001', '(', '\003', 
-'R', '\020', 'n', 'e', 'g', 'a', 't', 'i', 'v', 'e', 'I', 'n', 't', 'V', 'a', 'l', 'u', 'e', '\022', '!', '\n', '\014', 'd', 'o', 'u', 
-'b', 'l', 'e', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\006', ' ', '\001', '(', '\001', 'R', '\013', 'd', 'o', 'u', 'b', 'l', 'e', 'V', 'a', 
-'l', 'u', 'e', '\022', '!', '\n', '\014', 's', 't', 'r', 'i', 'n', 'g', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\007', ' ', '\001', '(', '\014', 
-'R', '\013', 's', 't', 'r', 'i', 'n', 'g', 'V', 'a', 'l', 'u', 'e', '\022', '\'', '\n', '\017', 'a', 'g', 'g', 'r', 'e', 'g', 'a', 't', 
-'e', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\010', ' ', '\001', '(', '\t', 'R', '\016', 'a', 'g', 'g', 'r', 'e', 'g', 'a', 't', 'e', 'V', 
-'a', 'l', 'u', 'e', '\032', 'J', '\n', '\010', 'N', 'a', 'm', 'e', 'P', 'a', 'r', 't', '\022', '\033', '\n', '\t', 'n', 'a', 'm', 'e', '_', 
-'p', 'a', 'r', 't', '\030', '\001', ' ', '\002', '(', '\t', 'R', '\010', 'n', 'a', 'm', 'e', 'P', 'a', 'r', 't', '\022', '!', '\n', '\014', 'i', 
-'s', '_', 'e', 'x', 't', 'e', 'n', 's', 'i', 'o', 'n', '\030', '\002', ' ', '\002', '(', '\010', 'R', '\013', 'i', 's', 'E', 'x', 't', 'e', 
-'n', 's', 'i', 'o', 'n', '\"', '\247', '\002', '\n', '\016', 'S', 'o', 'u', 'r', 'c', 'e', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '\022', 
-'D', '\n', '\010', 'l', 'o', 'c', 'a', 't', 'i', 'o', 'n', '\030', '\001', ' ', '\003', '(', '\013', '2', '(', '.', 'g', 'o', 'o', 'g', 'l', 
-'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'S', 'o', 'u', 'r', 'c', 'e', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', 
-'.', 'L', 'o', 'c', 'a', 't', 'i', 'o', 'n', 'R', '\010', 'l', 'o', 'c', 'a', 't', 'i', 'o', 'n', '\032', '\316', '\001', '\n', '\010', 'L', 
-'o', 'c', 'a', 't', 'i', 'o', 'n', '\022', '\026', '\n', '\004', 'p', 'a', 't', 'h', '\030', '\001', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 
-'R', '\004', 'p', 'a', 't', 'h', '\022', '\026', '\n', '\004', 's', 'p', 'a', 'n', '\030', '\002', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', 
-'\004', 's', 'p', 'a', 'n', '\022', ')', '\n', '\020', 'l', 'e', 'a', 'd', 'i', 'n', 'g', '_', 'c', 'o', 'm', 'm', 'e', 'n', 't', 's', 
-'\030', '\003', ' ', '\001', '(', '\t', 'R', '\017', 'l', 'e', 'a', 'd', 'i', 'n', 'g', 'C', 'o', 'm', 'm', 'e', 'n', 't', 's', '\022', '+', 
-'\n', '\021', 't', 'r', 'a', 'i', 'l', 'i', 'n', 'g', '_', 'c', 'o', 'm', 'm', 'e', 'n', 't', 's', '\030', '\004', ' ', '\001', '(', '\t', 
-'R', '\020', 't', 'r', 'a', 'i', 'l', 'i', 'n', 'g', 'C', 'o', 'm', 'm', 'e', 'n', 't', 's', '\022', ':', '\n', '\031', 'l', 'e', 'a', 
-'d', 'i', 'n', 'g', '_', 'd', 'e', 't', 'a', 'c', 'h', 'e', 'd', '_', 'c', 'o', 'm', 'm', 'e', 'n', 't', 's', '\030', '\006', ' ', 
-'\003', '(', '\t', 'R', '\027', 'l', 'e', 'a', 'd', 'i', 'n', 'g', 'D', 'e', 't', 'a', 'c', 'h', 'e', 'd', 'C', 'o', 'm', 'm', 'e', 
-'n', 't', 's', '\"', '\320', '\002', '\n', '\021', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', 
-'\022', 'M', '\n', '\n', 'a', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '\030', '\001', ' ', '\003', '(', '\013', '2', '-', '.', 'g', 'o', 
-'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 'C', 'o', 
-'d', 'e', 'I', 'n', 'f', 'o', '.', 'A', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', 'R', '\n', 'a', 'n', 'n', 'o', 't', 'a', 
-'t', 'i', 'o', 'n', '\032', '\353', '\001', '\n', '\n', 'A', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '\022', '\026', '\n', '\004', 'p', 'a', 
-'t', 'h', '\030', '\001', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', '\004', 'p', 'a', 't', 'h', '\022', '\037', '\n', '\013', 's', 'o', 'u', 
-'r', 'c', 'e', '_', 'f', 'i', 'l', 'e', '\030', '\002', ' ', '\001', '(', '\t', 'R', '\n', 's', 'o', 'u', 'r', 'c', 'e', 'F', 'i', 'l', 
-'e', '\022', '\024', '\n', '\005', 'b', 'e', 'g', 'i', 'n', '\030', '\003', ' ', '\001', '(', '\005', 'R', '\005', 'b', 'e', 'g', 'i', 'n', '\022', '\020', 
-'\n', '\003', 'e', 'n', 'd', '\030', '\004', ' ', '\001', '(', '\005', 'R', '\003', 'e', 'n', 'd', '\022', 'R', '\n', '\010', 's', 'e', 'm', 'a', 'n', 
-'t', 'i', 'c', '\030', '\005', ' ', '\001', '(', '\016', '2', '6', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 
-'u', 'f', '.', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'A', 'n', 'n', 'o', 
-'t', 'a', 't', 'i', 'o', 'n', '.', 'S', 'e', 'm', 'a', 'n', 't', 'i', 'c', 'R', '\010', 's', 'e', 'm', 'a', 'n', 't', 'i', 'c', 
-'\"', '(', '\n', '\010', 'S', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\022', '\010', '\n', '\004', 'N', 'O', 'N', 'E', '\020', '\000', '\022', '\007', '\n', 
-'\003', 'S', 'E', 'T', '\020', '\001', '\022', '\t', '\n', '\005', 'A', 'L', 'I', 'A', 'S', '\020', '\002', 'B', '~', '\n', '\023', 'c', 'o', 'm', '.', 
-'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', 'B', '\020', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 
-'o', 'r', 'P', 'r', 'o', 't', 'o', 's', 'H', '\001', 'Z', '-', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'g', 'o', 'l', 'a', 'n', 'g', 
-'.', 'o', 'r', 'g', '/', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '/', 't', 'y', 'p', 'e', 's', '/', 'd', 'e', 's', 'c', 'r', 
-'i', 'p', 't', 'o', 'r', 'p', 'b', '\370', '\001', '\001', '\242', '\002', '\003', 'G', 'P', 'B', '\252', '\002', '\032', 'G', 'o', 'o', 'g', 'l', 'e', 
-'.', 'P', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'R', 'e', 'f', 'l', 'e', 'c', 't', 'i', 'o', 'n', 
+'p', 't', 'i', 'o', 'n', '.', 'N', 'a', 'm', 'e', 'P', 'a', 'r', 't', 'R', '\004', 'n', 'a', 'm', 'e', '\022', ')', '\n', '\020', 'i', 
+'d', 'e', 'n', 't', 'i', 'f', 'i', 'e', 'r', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\003', ' ', '\001', '(', '\t', 'R', '\017', 'i', 'd', 
+'e', 'n', 't', 'i', 'f', 'i', 'e', 'r', 'V', 'a', 'l', 'u', 'e', '\022', ',', '\n', '\022', 'p', 'o', 's', 'i', 't', 'i', 'v', 'e', 
+'_', 'i', 'n', 't', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\004', ' ', '\001', '(', '\004', 'R', '\020', 'p', 'o', 's', 'i', 't', 'i', 'v', 
+'e', 'I', 'n', 't', 'V', 'a', 'l', 'u', 'e', '\022', ',', '\n', '\022', 'n', 'e', 'g', 'a', 't', 'i', 'v', 'e', '_', 'i', 'n', 't', 
+'_', 'v', 'a', 'l', 'u', 'e', '\030', '\005', ' ', '\001', '(', '\003', 'R', '\020', 'n', 'e', 'g', 'a', 't', 'i', 'v', 'e', 'I', 'n', 't', 
+'V', 'a', 'l', 'u', 'e', '\022', '!', '\n', '\014', 'd', 'o', 'u', 'b', 'l', 'e', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\006', ' ', '\001', 
+'(', '\001', 'R', '\013', 'd', 'o', 'u', 'b', 'l', 'e', 'V', 'a', 'l', 'u', 'e', '\022', '!', '\n', '\014', 's', 't', 'r', 'i', 'n', 'g', 
+'_', 'v', 'a', 'l', 'u', 'e', '\030', '\007', ' ', '\001', '(', '\014', 'R', '\013', 's', 't', 'r', 'i', 'n', 'g', 'V', 'a', 'l', 'u', 'e', 
+'\022', '\'', '\n', '\017', 'a', 'g', 'g', 'r', 'e', 'g', 'a', 't', 'e', '_', 'v', 'a', 'l', 'u', 'e', '\030', '\010', ' ', '\001', '(', '\t', 
+'R', '\016', 'a', 'g', 'g', 'r', 'e', 'g', 'a', 't', 'e', 'V', 'a', 'l', 'u', 'e', '\032', 'J', '\n', '\010', 'N', 'a', 'm', 'e', 'P', 
+'a', 'r', 't', '\022', '\033', '\n', '\t', 'n', 'a', 'm', 'e', '_', 'p', 'a', 'r', 't', '\030', '\001', ' ', '\002', '(', '\t', 'R', '\010', 'n', 
+'a', 'm', 'e', 'P', 'a', 'r', 't', '\022', '!', '\n', '\014', 'i', 's', '_', 'e', 'x', 't', 'e', 'n', 's', 'i', 'o', 'n', '\030', '\002', 
+' ', '\002', '(', '\010', 'R', '\013', 'i', 's', 'E', 'x', 't', 'e', 'n', 's', 'i', 'o', 'n', '\"', '\247', '\002', '\n', '\016', 'S', 'o', 'u', 
+'r', 'c', 'e', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '\022', 'D', '\n', '\010', 'l', 'o', 'c', 'a', 't', 'i', 'o', 'n', '\030', '\001', 
+' ', '\003', '(', '\013', '2', '(', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'S', 'o', 
+'u', 'r', 'c', 'e', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'L', 'o', 'c', 'a', 't', 'i', 'o', 'n', 'R', '\010', 'l', 'o', 
+'c', 'a', 't', 'i', 'o', 'n', '\032', '\316', '\001', '\n', '\010', 'L', 'o', 'c', 'a', 't', 'i', 'o', 'n', '\022', '\026', '\n', '\004', 'p', 'a', 
+'t', 'h', '\030', '\001', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', '\004', 'p', 'a', 't', 'h', '\022', '\026', '\n', '\004', 's', 'p', 'a', 
+'n', '\030', '\002', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', '\004', 's', 'p', 'a', 'n', '\022', ')', '\n', '\020', 'l', 'e', 'a', 'd', 
+'i', 'n', 'g', '_', 'c', 'o', 'm', 'm', 'e', 'n', 't', 's', '\030', '\003', ' ', '\001', '(', '\t', 'R', '\017', 'l', 'e', 'a', 'd', 'i', 
+'n', 'g', 'C', 'o', 'm', 'm', 'e', 'n', 't', 's', '\022', '+', '\n', '\021', 't', 'r', 'a', 'i', 'l', 'i', 'n', 'g', '_', 'c', 'o', 
+'m', 'm', 'e', 'n', 't', 's', '\030', '\004', ' ', '\001', '(', '\t', 'R', '\020', 't', 'r', 'a', 'i', 'l', 'i', 'n', 'g', 'C', 'o', 'm', 
+'m', 'e', 'n', 't', 's', '\022', ':', '\n', '\031', 'l', 'e', 'a', 'd', 'i', 'n', 'g', '_', 'd', 'e', 't', 'a', 'c', 'h', 'e', 'd', 
+'_', 'c', 'o', 'm', 'm', 'e', 'n', 't', 's', '\030', '\006', ' ', '\003', '(', '\t', 'R', '\027', 'l', 'e', 'a', 'd', 'i', 'n', 'g', 'D', 
+'e', 't', 'a', 'c', 'h', 'e', 'd', 'C', 'o', 'm', 'm', 'e', 'n', 't', 's', '\"', '\320', '\002', '\n', '\021', 'G', 'e', 'n', 'e', 'r', 
+'a', 't', 'e', 'd', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '\022', 'M', '\n', '\n', 'a', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 
+'n', '\030', '\001', ' ', '\003', '(', '\013', '2', '-', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', 
+'.', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 'C', 'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'A', 'n', 'n', 'o', 't', 'a', 
+'t', 'i', 'o', 'n', 'R', '\n', 'a', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '\032', '\353', '\001', '\n', '\n', 'A', 'n', 'n', 'o', 
+'t', 'a', 't', 'i', 'o', 'n', '\022', '\026', '\n', '\004', 'p', 'a', 't', 'h', '\030', '\001', ' ', '\003', '(', '\005', 'B', '\002', '\020', '\001', 'R', 
+'\004', 'p', 'a', 't', 'h', '\022', '\037', '\n', '\013', 's', 'o', 'u', 'r', 'c', 'e', '_', 'f', 'i', 'l', 'e', '\030', '\002', ' ', '\001', '(', 
+'\t', 'R', '\n', 's', 'o', 'u', 'r', 'c', 'e', 'F', 'i', 'l', 'e', '\022', '\024', '\n', '\005', 'b', 'e', 'g', 'i', 'n', '\030', '\003', ' ', 
+'\001', '(', '\005', 'R', '\005', 'b', 'e', 'g', 'i', 'n', '\022', '\020', '\n', '\003', 'e', 'n', 'd', '\030', '\004', ' ', '\001', '(', '\005', 'R', '\003', 
+'e', 'n', 'd', '\022', 'R', '\n', '\010', 's', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\030', '\005', ' ', '\001', '(', '\016', '2', '6', '.', 'g', 
+'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'G', 'e', 'n', 'e', 'r', 'a', 't', 'e', 'd', 'C', 
+'o', 'd', 'e', 'I', 'n', 'f', 'o', '.', 'A', 'n', 'n', 'o', 't', 'a', 't', 'i', 'o', 'n', '.', 'S', 'e', 'm', 'a', 'n', 't', 
+'i', 'c', 'R', '\010', 's', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\"', '(', '\n', '\010', 'S', 'e', 'm', 'a', 'n', 't', 'i', 'c', '\022', 
+'\010', '\n', '\004', 'N', 'O', 'N', 'E', '\020', '\000', '\022', '\007', '\n', '\003', 'S', 'E', 'T', '\020', '\001', '\022', '\t', '\n', '\005', 'A', 'L', 'I', 
+'A', 'S', '\020', '\002', 'B', '~', '\n', '\023', 'c', 'o', 'm', '.', 'g', 'o', 'o', 'g', 'l', 'e', '.', 'p', 'r', 'o', 't', 'o', 'b', 
+'u', 'f', 'B', '\020', 'D', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'P', 'r', 'o', 't', 'o', 's', 'H', '\001', 'Z', '-', 'g', 
+'o', 'o', 'g', 'l', 'e', '.', 'g', 'o', 'l', 'a', 'n', 'g', '.', 'o', 'r', 'g', '/', 'p', 'r', 'o', 't', 'o', 'b', 'u', 'f', 
+'/', 't', 'y', 'p', 'e', 's', '/', 'd', 'e', 's', 'c', 'r', 'i', 'p', 't', 'o', 'r', 'p', 'b', '\370', '\001', '\001', '\242', '\002', '\003', 
+'G', 'P', 'B', '\252', '\002', '\032', 'G', 'o', 'o', 'g', 'l', 'e', '.', 'P', 'r', 'o', 't', 'o', 'b', 'u', 'f', '.', 'R', 'e', 'f', 
+'l', 'e', 'c', 't', 'i', 'o', 'n', 
 };
 
 static _upb_DefPool_Init *deps[1] = {
   NULL
 };
 
 _upb_DefPool_Init google_protobuf_descriptor_proto_upbdefinit = {
   deps,
   &google_protobuf_descriptor_proto_upb_file_layout,
   "google/protobuf/descriptor.proto",
-  UPB_STRINGVIEW_INIT(descriptor, 8545)
+  UPB_STRINGVIEW_INIT(descriptor, 9057)
 };
```

### Comparing `protobuf-4.22.3/google/protobuf/descriptor.upbdefs.h` & `protobuf-4.23.0rc2/google/protobuf/descriptor.upbdefs.h`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,19 @@
 }
 
 UPB_INLINE const upb_MessageDef *google_protobuf_ExtensionRangeOptions_getmsgdef(upb_DefPool *s) {
   _upb_DefPool_LoadDefInit(s, &google_protobuf_descriptor_proto_upbdefinit);
   return upb_DefPool_FindMessageByName(s, "google.protobuf.ExtensionRangeOptions");
 }
 
+UPB_INLINE const upb_MessageDef *google_protobuf_ExtensionRangeOptions_Declaration_getmsgdef(upb_DefPool *s) {
+  _upb_DefPool_LoadDefInit(s, &google_protobuf_descriptor_proto_upbdefinit);
+  return upb_DefPool_FindMessageByName(s, "google.protobuf.ExtensionRangeOptions.Declaration");
+}
+
 UPB_INLINE const upb_MessageDef *google_protobuf_FieldDescriptorProto_getmsgdef(upb_DefPool *s) {
   _upb_DefPool_LoadDefInit(s, &google_protobuf_descriptor_proto_upbdefinit);
   return upb_DefPool_FindMessageByName(s, "google.protobuf.FieldDescriptorProto");
 }
 
 UPB_INLINE const upb_MessageDef *google_protobuf_OneofDescriptorProto_getmsgdef(upb_DefPool *s) {
   _upb_DefPool_LoadDefInit(s, &google_protobuf_descriptor_proto_upbdefinit);
```

### Comparing `protobuf-4.22.3/google/protobuf/descriptor_database.py` & `protobuf-4.23.0rc2/google/protobuf/descriptor_database.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/descriptor_pb2.py` & `protobuf-4.23.0rc2/google/protobuf/descriptor_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,59 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/descriptor.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR = _descriptor.FileDescriptor(
     name='google/protobuf/descriptor.proto',
     package='google.protobuf',
     syntax='proto2',
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
-    serialized_pb=b'\n google/protobuf/descriptor.proto\x12\x0fgoogle.protobuf\"M\n\x11\x46ileDescriptorSet\x12\x38\n\x04\x66ile\x18\x01 \x03(\x0b\x32$.google.protobuf.FileDescriptorProtoR\x04\x66ile\"\xfe\x04\n\x13\x46ileDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07package\x18\x02 \x01(\tR\x07package\x12\x1e\n\ndependency\x18\x03 \x03(\tR\ndependency\x12+\n\x11public_dependency\x18\n \x03(\x05R\x10publicDependency\x12\'\n\x0fweak_dependency\x18\x0b \x03(\x05R\x0eweakDependency\x12\x43\n\x0cmessage_type\x18\x04 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\x0bmessageType\x12\x41\n\tenum_type\x18\x05 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12\x41\n\x07service\x18\x06 \x03(\x0b\x32\'.google.protobuf.ServiceDescriptorProtoR\x07service\x12\x43\n\textension\x18\x07 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x36\n\x07options\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.FileOptionsR\x07options\x12I\n\x10source_code_info\x18\t \x01(\x0b\x32\x1f.google.protobuf.SourceCodeInfoR\x0esourceCodeInfo\x12\x16\n\x06syntax\x18\x0c \x01(\tR\x06syntax\x12\x18\n\x07\x65\x64ition\x18\r \x01(\tR\x07\x65\x64ition\"\xb9\x06\n\x0f\x44\x65scriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\x05\x66ield\x18\x02 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\x05\x66ield\x12\x43\n\textension\x18\x06 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x41\n\x0bnested_type\x18\x03 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\nnestedType\x12\x41\n\tenum_type\x18\x04 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12X\n\x0f\x65xtension_range\x18\x05 \x03(\x0b\x32/.google.protobuf.DescriptorProto.ExtensionRangeR\x0e\x65xtensionRange\x12\x44\n\noneof_decl\x18\x08 \x03(\x0b\x32%.google.protobuf.OneofDescriptorProtoR\toneofDecl\x12\x39\n\x07options\x18\x07 \x01(\x0b\x32\x1f.google.protobuf.MessageOptionsR\x07options\x12U\n\x0ereserved_range\x18\t \x03(\x0b\x32..google.protobuf.DescriptorProto.ReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\n \x03(\tR\x0creservedName\x1az\n\x0e\x45xtensionRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x12@\n\x07options\x18\x03 \x01(\x0b\x32&.google.protobuf.ExtensionRangeOptionsR\x07options\x1a\x37\n\rReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"|\n\x15\x45xtensionRangeOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xc1\x06\n\x14\x46ieldDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x41\n\x05label\x18\x04 \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.LabelR\x05label\x12>\n\x04type\x18\x05 \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.TypeR\x04type\x12\x1b\n\ttype_name\x18\x06 \x01(\tR\x08typeName\x12\x1a\n\x08\x65xtendee\x18\x02 \x01(\tR\x08\x65xtendee\x12#\n\rdefault_value\x18\x07 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1f\n\x0boneof_index\x18\t \x01(\x05R\noneofIndex\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12\x37\n\x07options\x18\x08 \x01(\x0b\x32\x1d.google.protobuf.FieldOptionsR\x07options\x12\'\n\x0fproto3_optional\x18\x11 \x01(\x08R\x0eproto3Optional\"\xb6\x02\n\x04Type\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"C\n\x05Label\x12\x12\n\x0eLABEL_OPTIONAL\x10\x01\x12\x12\n\x0eLABEL_REQUIRED\x10\x02\x12\x12\n\x0eLABEL_REPEATED\x10\x03\"c\n\x14OneofDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x37\n\x07options\x18\x02 \x01(\x0b\x32\x1d.google.protobuf.OneofOptionsR\x07options\"\xe3\x02\n\x13\x45numDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x05value\x18\x02 \x03(\x0b\x32).google.protobuf.EnumValueDescriptorProtoR\x05value\x12\x36\n\x07options\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.EnumOptionsR\x07options\x12]\n\x0ereserved_range\x18\x04 \x03(\x0b\x32\x36.google.protobuf.EnumDescriptorProto.EnumReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\x05 \x03(\tR\x0creservedName\x1a;\n\x11\x45numReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\x83\x01\n\x18\x45numValueDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12;\n\x07options\x18\x03 \x01(\x0b\x32!.google.protobuf.EnumValueOptionsR\x07options\"\xa7\x01\n\x16ServiceDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x06method\x18\x02 \x03(\x0b\x32&.google.protobuf.MethodDescriptorProtoR\x06method\x12\x39\n\x07options\x18\x03 \x01(\x0b\x32\x1f.google.protobuf.ServiceOptionsR\x07options\"\x89\x02\n\x15MethodDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ninput_type\x18\x02 \x01(\tR\tinputType\x12\x1f\n\x0boutput_type\x18\x03 \x01(\tR\noutputType\x12\x38\n\x07options\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.MethodOptionsR\x07options\x12\x30\n\x10\x63lient_streaming\x18\x05 \x01(\x08:\x05\x66\x61lseR\x0f\x63lientStreaming\x12\x30\n\x10server_streaming\x18\x06 \x01(\x08:\x05\x66\x61lseR\x0fserverStreaming\"\x91\t\n\x0b\x46ileOptions\x12!\n\x0cjava_package\x18\x01 \x01(\tR\x0bjavaPackage\x12\x30\n\x14java_outer_classname\x18\x08 \x01(\tR\x12javaOuterClassname\x12\x35\n\x13java_multiple_files\x18\n \x01(\x08:\x05\x66\x61lseR\x11javaMultipleFiles\x12\x44\n\x1djava_generate_equals_and_hash\x18\x14 \x01(\x08\x42\x02\x18\x01R\x19javaGenerateEqualsAndHash\x12:\n\x16java_string_check_utf8\x18\x1b \x01(\x08:\x05\x66\x61lseR\x13javaStringCheckUtf8\x12S\n\x0coptimize_for\x18\t \x01(\x0e\x32).google.protobuf.FileOptions.OptimizeMode:\x05SPEEDR\x0boptimizeFor\x12\x1d\n\ngo_package\x18\x0b \x01(\tR\tgoPackage\x12\x35\n\x13\x63\x63_generic_services\x18\x10 \x01(\x08:\x05\x66\x61lseR\x11\x63\x63GenericServices\x12\x39\n\x15java_generic_services\x18\x11 \x01(\x08:\x05\x66\x61lseR\x13javaGenericServices\x12\x35\n\x13py_generic_services\x18\x12 \x01(\x08:\x05\x66\x61lseR\x11pyGenericServices\x12\x37\n\x14php_generic_services\x18* \x01(\x08:\x05\x66\x61lseR\x12phpGenericServices\x12%\n\ndeprecated\x18\x17 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12.\n\x10\x63\x63_enable_arenas\x18\x1f \x01(\x08:\x04trueR\x0e\x63\x63\x45nableArenas\x12*\n\x11objc_class_prefix\x18$ \x01(\tR\x0fobjcClassPrefix\x12)\n\x10\x63sharp_namespace\x18% \x01(\tR\x0f\x63sharpNamespace\x12!\n\x0cswift_prefix\x18\' \x01(\tR\x0bswiftPrefix\x12(\n\x10php_class_prefix\x18( \x01(\tR\x0ephpClassPrefix\x12#\n\rphp_namespace\x18) \x01(\tR\x0cphpNamespace\x12\x34\n\x16php_metadata_namespace\x18, \x01(\tR\x14phpMetadataNamespace\x12!\n\x0cruby_package\x18- \x01(\tR\x0brubyPackage\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\":\n\x0cOptimizeMode\x12\t\n\x05SPEED\x10\x01\x12\r\n\tCODE_SIZE\x10\x02\x12\x10\n\x0cLITE_RUNTIME\x10\x03*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08&\x10\'\"\xbb\x03\n\x0eMessageOptions\x12<\n\x17message_set_wire_format\x18\x01 \x01(\x08:\x05\x66\x61lseR\x14messageSetWireFormat\x12L\n\x1fno_standard_descriptor_accessor\x18\x02 \x01(\x08:\x05\x66\x61lseR\x1cnoStandardDescriptorAccessor\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x1b\n\tmap_entry\x18\x07 \x01(\x08R\x08mapEntry\x12V\n&deprecated_legacy_json_field_conflicts\x18\x0b \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\xb7\x08\n\x0c\x46ieldOptions\x12\x41\n\x05\x63type\x18\x01 \x01(\x0e\x32#.google.protobuf.FieldOptions.CType:\x06STRINGR\x05\x63type\x12\x16\n\x06packed\x18\x02 \x01(\x08R\x06packed\x12G\n\x06jstype\x18\x06 \x01(\x0e\x32$.google.protobuf.FieldOptions.JSType:\tJS_NORMALR\x06jstype\x12\x19\n\x04lazy\x18\x05 \x01(\x08:\x05\x66\x61lseR\x04lazy\x12.\n\x0funverified_lazy\x18\x0f \x01(\x08:\x05\x66\x61lseR\x0eunverifiedLazy\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x19\n\x04weak\x18\n \x01(\x08:\x05\x66\x61lseR\x04weak\x12(\n\x0c\x64\x65\x62ug_redact\x18\x10 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12K\n\tretention\x18\x11 \x01(\x0e\x32-.google.protobuf.FieldOptions.OptionRetentionR\tretention\x12\x46\n\x06target\x18\x12 \x01(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeR\x06target\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"/\n\x05\x43Type\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x43ORD\x10\x01\x12\x10\n\x0cSTRING_PIECE\x10\x02\"5\n\x06JSType\x12\r\n\tJS_NORMAL\x10\x00\x12\r\n\tJS_STRING\x10\x01\x12\r\n\tJS_NUMBER\x10\x02\"U\n\x0fOptionRetention\x12\x15\n\x11RETENTION_UNKNOWN\x10\x00\x12\x15\n\x11RETENTION_RUNTIME\x10\x01\x12\x14\n\x10RETENTION_SOURCE\x10\x02\"\x8c\x02\n\x10OptionTargetType\x12\x17\n\x13TARGET_TYPE_UNKNOWN\x10\x00\x12\x14\n\x10TARGET_TYPE_FILE\x10\x01\x12\x1f\n\x1bTARGET_TYPE_EXTENSION_RANGE\x10\x02\x12\x17\n\x13TARGET_TYPE_MESSAGE\x10\x03\x12\x15\n\x11TARGET_TYPE_FIELD\x10\x04\x12\x15\n\x11TARGET_TYPE_ONEOF\x10\x05\x12\x14\n\x10TARGET_TYPE_ENUM\x10\x06\x12\x1a\n\x16TARGET_TYPE_ENUM_ENTRY\x10\x07\x12\x17\n\x13TARGET_TYPE_SERVICE\x10\x08\x12\x16\n\x12TARGET_TYPE_METHOD\x10\t*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05\"s\n\x0cOneofOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x98\x02\n\x0b\x45numOptions\x12\x1f\n\x0b\x61llow_alias\x18\x02 \x01(\x08R\nallowAlias\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12V\n&deprecated_legacy_json_field_conflicts\x18\x06 \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x05\x10\x06\"\x9e\x01\n\x10\x45numValueOptions\x12%\n\ndeprecated\x18\x01 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9c\x01\n\x0eServiceOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xe0\x02\n\rMethodOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12q\n\x11idempotency_level\x18\" \x01(\x0e\x32/.google.protobuf.MethodOptions.IdempotencyLevel:\x13IDEMPOTENCY_UNKNOWNR\x10idempotencyLevel\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"P\n\x10IdempotencyLevel\x12\x17\n\x13IDEMPOTENCY_UNKNOWN\x10\x00\x12\x13\n\x0fNO_SIDE_EFFECTS\x10\x01\x12\x0e\n\nIDEMPOTENT\x10\x02*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9a\x03\n\x13UninterpretedOption\x12\x41\n\x04name\x18\x02 \x03(\x0b\x32-.google.protobuf.UninterpretedOption.NamePartR\x04name\x12)\n\x10identifier_value\x18\x03 \x01(\tR\x0fidentifierValue\x12,\n\x12positive_int_value\x18\x04 \x01(\x04R\x10positiveIntValue\x12,\n\x12negative_int_value\x18\x05 \x01(\x03R\x10negativeIntValue\x12!\n\x0c\x64ouble_value\x18\x06 \x01(\x01R\x0b\x64oubleValue\x12!\n\x0cstring_value\x18\x07 \x01(\x0cR\x0bstringValue\x12\'\n\x0f\x61ggregate_value\x18\x08 \x01(\tR\x0e\x61ggregateValue\x1aJ\n\x08NamePart\x12\x1b\n\tname_part\x18\x01 \x02(\tR\x08namePart\x12!\n\x0cis_extension\x18\x02 \x02(\x08R\x0bisExtension\"\xa7\x02\n\x0eSourceCodeInfo\x12\x44\n\x08location\x18\x01 \x03(\x0b\x32(.google.protobuf.SourceCodeInfo.LocationR\x08location\x1a\xce\x01\n\x08Location\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x16\n\x04span\x18\x02 \x03(\x05\x42\x02\x10\x01R\x04span\x12)\n\x10leading_comments\x18\x03 \x01(\tR\x0fleadingComments\x12+\n\x11trailing_comments\x18\x04 \x01(\tR\x10trailingComments\x12:\n\x19leading_detached_comments\x18\x06 \x03(\tR\x17leadingDetachedComments\"\xd0\x02\n\x11GeneratedCodeInfo\x12M\n\nannotation\x18\x01 \x03(\x0b\x32-.google.protobuf.GeneratedCodeInfo.AnnotationR\nannotation\x1a\xeb\x01\n\nAnnotation\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x1f\n\x0bsource_file\x18\x02 \x01(\tR\nsourceFile\x12\x14\n\x05\x62\x65gin\x18\x03 \x01(\x05R\x05\x62\x65gin\x12\x10\n\x03\x65nd\x18\x04 \x01(\x05R\x03\x65nd\x12R\n\x08semantic\x18\x05 \x01(\x0e\x32\x36.google.protobuf.GeneratedCodeInfo.Annotation.SemanticR\x08semantic\"(\n\x08Semantic\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SET\x10\x01\x12\t\n\x05\x41LIAS\x10\x02\x42~\n\x13\x63om.google.protobufB\x10\x44\x65scriptorProtosH\x01Z-google.golang.org/protobuf/types/descriptorpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1aGoogle.Protobuf.Reflection'
+    serialized_pb=b'\n google/protobuf/descriptor.proto\x12\x0fgoogle.protobuf\"M\n\x11\x46ileDescriptorSet\x12\x38\n\x04\x66ile\x18\x01 \x03(\x0b\x32$.google.protobuf.FileDescriptorProtoR\x04\x66ile\"\xfe\x04\n\x13\x46ileDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07package\x18\x02 \x01(\tR\x07package\x12\x1e\n\ndependency\x18\x03 \x03(\tR\ndependency\x12+\n\x11public_dependency\x18\n \x03(\x05R\x10publicDependency\x12\'\n\x0fweak_dependency\x18\x0b \x03(\x05R\x0eweakDependency\x12\x43\n\x0cmessage_type\x18\x04 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\x0bmessageType\x12\x41\n\tenum_type\x18\x05 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12\x41\n\x07service\x18\x06 \x03(\x0b\x32\'.google.protobuf.ServiceDescriptorProtoR\x07service\x12\x43\n\textension\x18\x07 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x36\n\x07options\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.FileOptionsR\x07options\x12I\n\x10source_code_info\x18\t \x01(\x0b\x32\x1f.google.protobuf.SourceCodeInfoR\x0esourceCodeInfo\x12\x16\n\x06syntax\x18\x0c \x01(\tR\x06syntax\x12\x18\n\x07\x65\x64ition\x18\r \x01(\tR\x07\x65\x64ition\"\xb9\x06\n\x0f\x44\x65scriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\x05\x66ield\x18\x02 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\x05\x66ield\x12\x43\n\textension\x18\x06 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x41\n\x0bnested_type\x18\x03 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\nnestedType\x12\x41\n\tenum_type\x18\x04 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12X\n\x0f\x65xtension_range\x18\x05 \x03(\x0b\x32/.google.protobuf.DescriptorProto.ExtensionRangeR\x0e\x65xtensionRange\x12\x44\n\noneof_decl\x18\x08 \x03(\x0b\x32%.google.protobuf.OneofDescriptorProtoR\toneofDecl\x12\x39\n\x07options\x18\x07 \x01(\x0b\x32\x1f.google.protobuf.MessageOptionsR\x07options\x12U\n\x0ereserved_range\x18\t \x03(\x0b\x32..google.protobuf.DescriptorProto.ReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\n \x03(\tR\x0creservedName\x1az\n\x0e\x45xtensionRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x12@\n\x07options\x18\x03 \x01(\x0b\x32&.google.protobuf.ExtensionRangeOptionsR\x07options\x1a\x37\n\rReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\xad\x04\n\x15\x45xtensionRangeOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x12Y\n\x0b\x64\x65\x63laration\x18\x02 \x03(\x0b\x32\x32.google.protobuf.ExtensionRangeOptions.DeclarationB\x03\x88\x01\x02R\x0b\x64\x65\x63laration\x12h\n\x0cverification\x18\x03 \x01(\x0e\x32\x38.google.protobuf.ExtensionRangeOptions.VerificationState:\nUNVERIFIEDR\x0cverification\x1a\xb3\x01\n\x0b\x44\x65\x63laration\x12\x16\n\x06number\x18\x01 \x01(\x05R\x06number\x12\x1b\n\tfull_name\x18\x02 \x01(\tR\x08\x66ullName\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x12#\n\x0bis_repeated\x18\x04 \x01(\x08\x42\x02\x18\x01R\nisRepeated\x12\x1a\n\x08reserved\x18\x05 \x01(\x08R\x08reserved\x12\x1a\n\x08repeated\x18\x06 \x01(\x08R\x08repeated\"4\n\x11VerificationState\x12\x0f\n\x0b\x44\x45\x43LARATION\x10\x00\x12\x0e\n\nUNVERIFIED\x10\x01*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xc1\x06\n\x14\x46ieldDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x41\n\x05label\x18\x04 \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.LabelR\x05label\x12>\n\x04type\x18\x05 \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.TypeR\x04type\x12\x1b\n\ttype_name\x18\x06 \x01(\tR\x08typeName\x12\x1a\n\x08\x65xtendee\x18\x02 \x01(\tR\x08\x65xtendee\x12#\n\rdefault_value\x18\x07 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1f\n\x0boneof_index\x18\t \x01(\x05R\noneofIndex\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12\x37\n\x07options\x18\x08 \x01(\x0b\x32\x1d.google.protobuf.FieldOptionsR\x07options\x12\'\n\x0fproto3_optional\x18\x11 \x01(\x08R\x0eproto3Optional\"\xb6\x02\n\x04Type\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"C\n\x05Label\x12\x12\n\x0eLABEL_OPTIONAL\x10\x01\x12\x12\n\x0eLABEL_REQUIRED\x10\x02\x12\x12\n\x0eLABEL_REPEATED\x10\x03\"c\n\x14OneofDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x37\n\x07options\x18\x02 \x01(\x0b\x32\x1d.google.protobuf.OneofOptionsR\x07options\"\xe3\x02\n\x13\x45numDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x05value\x18\x02 \x03(\x0b\x32).google.protobuf.EnumValueDescriptorProtoR\x05value\x12\x36\n\x07options\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.EnumOptionsR\x07options\x12]\n\x0ereserved_range\x18\x04 \x03(\x0b\x32\x36.google.protobuf.EnumDescriptorProto.EnumReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\x05 \x03(\tR\x0creservedName\x1a;\n\x11\x45numReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\x83\x01\n\x18\x45numValueDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12;\n\x07options\x18\x03 \x01(\x0b\x32!.google.protobuf.EnumValueOptionsR\x07options\"\xa7\x01\n\x16ServiceDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x06method\x18\x02 \x03(\x0b\x32&.google.protobuf.MethodDescriptorProtoR\x06method\x12\x39\n\x07options\x18\x03 \x01(\x0b\x32\x1f.google.protobuf.ServiceOptionsR\x07options\"\x89\x02\n\x15MethodDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ninput_type\x18\x02 \x01(\tR\tinputType\x12\x1f\n\x0boutput_type\x18\x03 \x01(\tR\noutputType\x12\x38\n\x07options\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.MethodOptionsR\x07options\x12\x30\n\x10\x63lient_streaming\x18\x05 \x01(\x08:\x05\x66\x61lseR\x0f\x63lientStreaming\x12\x30\n\x10server_streaming\x18\x06 \x01(\x08:\x05\x66\x61lseR\x0fserverStreaming\"\x91\t\n\x0b\x46ileOptions\x12!\n\x0cjava_package\x18\x01 \x01(\tR\x0bjavaPackage\x12\x30\n\x14java_outer_classname\x18\x08 \x01(\tR\x12javaOuterClassname\x12\x35\n\x13java_multiple_files\x18\n \x01(\x08:\x05\x66\x61lseR\x11javaMultipleFiles\x12\x44\n\x1djava_generate_equals_and_hash\x18\x14 \x01(\x08\x42\x02\x18\x01R\x19javaGenerateEqualsAndHash\x12:\n\x16java_string_check_utf8\x18\x1b \x01(\x08:\x05\x66\x61lseR\x13javaStringCheckUtf8\x12S\n\x0coptimize_for\x18\t \x01(\x0e\x32).google.protobuf.FileOptions.OptimizeMode:\x05SPEEDR\x0boptimizeFor\x12\x1d\n\ngo_package\x18\x0b \x01(\tR\tgoPackage\x12\x35\n\x13\x63\x63_generic_services\x18\x10 \x01(\x08:\x05\x66\x61lseR\x11\x63\x63GenericServices\x12\x39\n\x15java_generic_services\x18\x11 \x01(\x08:\x05\x66\x61lseR\x13javaGenericServices\x12\x35\n\x13py_generic_services\x18\x12 \x01(\x08:\x05\x66\x61lseR\x11pyGenericServices\x12\x37\n\x14php_generic_services\x18* \x01(\x08:\x05\x66\x61lseR\x12phpGenericServices\x12%\n\ndeprecated\x18\x17 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12.\n\x10\x63\x63_enable_arenas\x18\x1f \x01(\x08:\x04trueR\x0e\x63\x63\x45nableArenas\x12*\n\x11objc_class_prefix\x18$ \x01(\tR\x0fobjcClassPrefix\x12)\n\x10\x63sharp_namespace\x18% \x01(\tR\x0f\x63sharpNamespace\x12!\n\x0cswift_prefix\x18\' \x01(\tR\x0bswiftPrefix\x12(\n\x10php_class_prefix\x18( \x01(\tR\x0ephpClassPrefix\x12#\n\rphp_namespace\x18) \x01(\tR\x0cphpNamespace\x12\x34\n\x16php_metadata_namespace\x18, \x01(\tR\x14phpMetadataNamespace\x12!\n\x0cruby_package\x18- \x01(\tR\x0brubyPackage\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\":\n\x0cOptimizeMode\x12\t\n\x05SPEED\x10\x01\x12\r\n\tCODE_SIZE\x10\x02\x12\x10\n\x0cLITE_RUNTIME\x10\x03*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08&\x10\'\"\xbb\x03\n\x0eMessageOptions\x12<\n\x17message_set_wire_format\x18\x01 \x01(\x08:\x05\x66\x61lseR\x14messageSetWireFormat\x12L\n\x1fno_standard_descriptor_accessor\x18\x02 \x01(\x08:\x05\x66\x61lseR\x1cnoStandardDescriptorAccessor\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x1b\n\tmap_entry\x18\x07 \x01(\x08R\x08mapEntry\x12V\n&deprecated_legacy_json_field_conflicts\x18\x0b \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\x85\t\n\x0c\x46ieldOptions\x12\x41\n\x05\x63type\x18\x01 \x01(\x0e\x32#.google.protobuf.FieldOptions.CType:\x06STRINGR\x05\x63type\x12\x16\n\x06packed\x18\x02 \x01(\x08R\x06packed\x12G\n\x06jstype\x18\x06 \x01(\x0e\x32$.google.protobuf.FieldOptions.JSType:\tJS_NORMALR\x06jstype\x12\x19\n\x04lazy\x18\x05 \x01(\x08:\x05\x66\x61lseR\x04lazy\x12.\n\x0funverified_lazy\x18\x0f \x01(\x08:\x05\x66\x61lseR\x0eunverifiedLazy\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x19\n\x04weak\x18\n \x01(\x08:\x05\x66\x61lseR\x04weak\x12(\n\x0c\x64\x65\x62ug_redact\x18\x10 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12K\n\tretention\x18\x11 \x01(\x0e\x32-.google.protobuf.FieldOptions.OptionRetentionR\tretention\x12J\n\x06target\x18\x12 \x01(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeB\x02\x18\x01R\x06target\x12H\n\x07targets\x18\x13 \x03(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeR\x07targets\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"/\n\x05\x43Type\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x43ORD\x10\x01\x12\x10\n\x0cSTRING_PIECE\x10\x02\"5\n\x06JSType\x12\r\n\tJS_NORMAL\x10\x00\x12\r\n\tJS_STRING\x10\x01\x12\r\n\tJS_NUMBER\x10\x02\"U\n\x0fOptionRetention\x12\x15\n\x11RETENTION_UNKNOWN\x10\x00\x12\x15\n\x11RETENTION_RUNTIME\x10\x01\x12\x14\n\x10RETENTION_SOURCE\x10\x02\"\x8c\x02\n\x10OptionTargetType\x12\x17\n\x13TARGET_TYPE_UNKNOWN\x10\x00\x12\x14\n\x10TARGET_TYPE_FILE\x10\x01\x12\x1f\n\x1bTARGET_TYPE_EXTENSION_RANGE\x10\x02\x12\x17\n\x13TARGET_TYPE_MESSAGE\x10\x03\x12\x15\n\x11TARGET_TYPE_FIELD\x10\x04\x12\x15\n\x11TARGET_TYPE_ONEOF\x10\x05\x12\x14\n\x10TARGET_TYPE_ENUM\x10\x06\x12\x1a\n\x16TARGET_TYPE_ENUM_ENTRY\x10\x07\x12\x17\n\x13TARGET_TYPE_SERVICE\x10\x08\x12\x16\n\x12TARGET_TYPE_METHOD\x10\t*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05\"s\n\x0cOneofOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x98\x02\n\x0b\x45numOptions\x12\x1f\n\x0b\x61llow_alias\x18\x02 \x01(\x08R\nallowAlias\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12V\n&deprecated_legacy_json_field_conflicts\x18\x06 \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x05\x10\x06\"\x9e\x01\n\x10\x45numValueOptions\x12%\n\ndeprecated\x18\x01 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9c\x01\n\x0eServiceOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xe0\x02\n\rMethodOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12q\n\x11idempotency_level\x18\" \x01(\x0e\x32/.google.protobuf.MethodOptions.IdempotencyLevel:\x13IDEMPOTENCY_UNKNOWNR\x10idempotencyLevel\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"P\n\x10IdempotencyLevel\x12\x17\n\x13IDEMPOTENCY_UNKNOWN\x10\x00\x12\x13\n\x0fNO_SIDE_EFFECTS\x10\x01\x12\x0e\n\nIDEMPOTENT\x10\x02*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9a\x03\n\x13UninterpretedOption\x12\x41\n\x04name\x18\x02 \x03(\x0b\x32-.google.protobuf.UninterpretedOption.NamePartR\x04name\x12)\n\x10identifier_value\x18\x03 \x01(\tR\x0fidentifierValue\x12,\n\x12positive_int_value\x18\x04 \x01(\x04R\x10positiveIntValue\x12,\n\x12negative_int_value\x18\x05 \x01(\x03R\x10negativeIntValue\x12!\n\x0c\x64ouble_value\x18\x06 \x01(\x01R\x0b\x64oubleValue\x12!\n\x0cstring_value\x18\x07 \x01(\x0cR\x0bstringValue\x12\'\n\x0f\x61ggregate_value\x18\x08 \x01(\tR\x0e\x61ggregateValue\x1aJ\n\x08NamePart\x12\x1b\n\tname_part\x18\x01 \x02(\tR\x08namePart\x12!\n\x0cis_extension\x18\x02 \x02(\x08R\x0bisExtension\"\xa7\x02\n\x0eSourceCodeInfo\x12\x44\n\x08location\x18\x01 \x03(\x0b\x32(.google.protobuf.SourceCodeInfo.LocationR\x08location\x1a\xce\x01\n\x08Location\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x16\n\x04span\x18\x02 \x03(\x05\x42\x02\x10\x01R\x04span\x12)\n\x10leading_comments\x18\x03 \x01(\tR\x0fleadingComments\x12+\n\x11trailing_comments\x18\x04 \x01(\tR\x10trailingComments\x12:\n\x19leading_detached_comments\x18\x06 \x03(\tR\x17leadingDetachedComments\"\xd0\x02\n\x11GeneratedCodeInfo\x12M\n\nannotation\x18\x01 \x03(\x0b\x32-.google.protobuf.GeneratedCodeInfo.AnnotationR\nannotation\x1a\xeb\x01\n\nAnnotation\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x1f\n\x0bsource_file\x18\x02 \x01(\tR\nsourceFile\x12\x14\n\x05\x62\x65gin\x18\x03 \x01(\x05R\x05\x62\x65gin\x12\x10\n\x03\x65nd\x18\x04 \x01(\x05R\x03\x65nd\x12R\n\x08semantic\x18\x05 \x01(\x0e\x32\x36.google.protobuf.GeneratedCodeInfo.Annotation.SemanticR\x08semantic\"(\n\x08Semantic\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SET\x10\x01\x12\t\n\x05\x41LIAS\x10\x02\x42~\n\x13\x63om.google.protobufB\x10\x44\x65scriptorProtosH\x01Z-google.golang.org/protobuf/types/descriptorpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1aGoogle.Protobuf.Reflection'
   )
 else:
-  DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n google/protobuf/descriptor.proto\x12\x0fgoogle.protobuf\"M\n\x11\x46ileDescriptorSet\x12\x38\n\x04\x66ile\x18\x01 \x03(\x0b\x32$.google.protobuf.FileDescriptorProtoR\x04\x66ile\"\xfe\x04\n\x13\x46ileDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07package\x18\x02 \x01(\tR\x07package\x12\x1e\n\ndependency\x18\x03 \x03(\tR\ndependency\x12+\n\x11public_dependency\x18\n \x03(\x05R\x10publicDependency\x12\'\n\x0fweak_dependency\x18\x0b \x03(\x05R\x0eweakDependency\x12\x43\n\x0cmessage_type\x18\x04 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\x0bmessageType\x12\x41\n\tenum_type\x18\x05 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12\x41\n\x07service\x18\x06 \x03(\x0b\x32\'.google.protobuf.ServiceDescriptorProtoR\x07service\x12\x43\n\textension\x18\x07 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x36\n\x07options\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.FileOptionsR\x07options\x12I\n\x10source_code_info\x18\t \x01(\x0b\x32\x1f.google.protobuf.SourceCodeInfoR\x0esourceCodeInfo\x12\x16\n\x06syntax\x18\x0c \x01(\tR\x06syntax\x12\x18\n\x07\x65\x64ition\x18\r \x01(\tR\x07\x65\x64ition\"\xb9\x06\n\x0f\x44\x65scriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\x05\x66ield\x18\x02 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\x05\x66ield\x12\x43\n\textension\x18\x06 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x41\n\x0bnested_type\x18\x03 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\nnestedType\x12\x41\n\tenum_type\x18\x04 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12X\n\x0f\x65xtension_range\x18\x05 \x03(\x0b\x32/.google.protobuf.DescriptorProto.ExtensionRangeR\x0e\x65xtensionRange\x12\x44\n\noneof_decl\x18\x08 \x03(\x0b\x32%.google.protobuf.OneofDescriptorProtoR\toneofDecl\x12\x39\n\x07options\x18\x07 \x01(\x0b\x32\x1f.google.protobuf.MessageOptionsR\x07options\x12U\n\x0ereserved_range\x18\t \x03(\x0b\x32..google.protobuf.DescriptorProto.ReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\n \x03(\tR\x0creservedName\x1az\n\x0e\x45xtensionRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x12@\n\x07options\x18\x03 \x01(\x0b\x32&.google.protobuf.ExtensionRangeOptionsR\x07options\x1a\x37\n\rReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"|\n\x15\x45xtensionRangeOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xc1\x06\n\x14\x46ieldDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x41\n\x05label\x18\x04 \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.LabelR\x05label\x12>\n\x04type\x18\x05 \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.TypeR\x04type\x12\x1b\n\ttype_name\x18\x06 \x01(\tR\x08typeName\x12\x1a\n\x08\x65xtendee\x18\x02 \x01(\tR\x08\x65xtendee\x12#\n\rdefault_value\x18\x07 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1f\n\x0boneof_index\x18\t \x01(\x05R\noneofIndex\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12\x37\n\x07options\x18\x08 \x01(\x0b\x32\x1d.google.protobuf.FieldOptionsR\x07options\x12\'\n\x0fproto3_optional\x18\x11 \x01(\x08R\x0eproto3Optional\"\xb6\x02\n\x04Type\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"C\n\x05Label\x12\x12\n\x0eLABEL_OPTIONAL\x10\x01\x12\x12\n\x0eLABEL_REQUIRED\x10\x02\x12\x12\n\x0eLABEL_REPEATED\x10\x03\"c\n\x14OneofDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x37\n\x07options\x18\x02 \x01(\x0b\x32\x1d.google.protobuf.OneofOptionsR\x07options\"\xe3\x02\n\x13\x45numDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x05value\x18\x02 \x03(\x0b\x32).google.protobuf.EnumValueDescriptorProtoR\x05value\x12\x36\n\x07options\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.EnumOptionsR\x07options\x12]\n\x0ereserved_range\x18\x04 \x03(\x0b\x32\x36.google.protobuf.EnumDescriptorProto.EnumReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\x05 \x03(\tR\x0creservedName\x1a;\n\x11\x45numReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\x83\x01\n\x18\x45numValueDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12;\n\x07options\x18\x03 \x01(\x0b\x32!.google.protobuf.EnumValueOptionsR\x07options\"\xa7\x01\n\x16ServiceDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x06method\x18\x02 \x03(\x0b\x32&.google.protobuf.MethodDescriptorProtoR\x06method\x12\x39\n\x07options\x18\x03 \x01(\x0b\x32\x1f.google.protobuf.ServiceOptionsR\x07options\"\x89\x02\n\x15MethodDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ninput_type\x18\x02 \x01(\tR\tinputType\x12\x1f\n\x0boutput_type\x18\x03 \x01(\tR\noutputType\x12\x38\n\x07options\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.MethodOptionsR\x07options\x12\x30\n\x10\x63lient_streaming\x18\x05 \x01(\x08:\x05\x66\x61lseR\x0f\x63lientStreaming\x12\x30\n\x10server_streaming\x18\x06 \x01(\x08:\x05\x66\x61lseR\x0fserverStreaming\"\x91\t\n\x0b\x46ileOptions\x12!\n\x0cjava_package\x18\x01 \x01(\tR\x0bjavaPackage\x12\x30\n\x14java_outer_classname\x18\x08 \x01(\tR\x12javaOuterClassname\x12\x35\n\x13java_multiple_files\x18\n \x01(\x08:\x05\x66\x61lseR\x11javaMultipleFiles\x12\x44\n\x1djava_generate_equals_and_hash\x18\x14 \x01(\x08\x42\x02\x18\x01R\x19javaGenerateEqualsAndHash\x12:\n\x16java_string_check_utf8\x18\x1b \x01(\x08:\x05\x66\x61lseR\x13javaStringCheckUtf8\x12S\n\x0coptimize_for\x18\t \x01(\x0e\x32).google.protobuf.FileOptions.OptimizeMode:\x05SPEEDR\x0boptimizeFor\x12\x1d\n\ngo_package\x18\x0b \x01(\tR\tgoPackage\x12\x35\n\x13\x63\x63_generic_services\x18\x10 \x01(\x08:\x05\x66\x61lseR\x11\x63\x63GenericServices\x12\x39\n\x15java_generic_services\x18\x11 \x01(\x08:\x05\x66\x61lseR\x13javaGenericServices\x12\x35\n\x13py_generic_services\x18\x12 \x01(\x08:\x05\x66\x61lseR\x11pyGenericServices\x12\x37\n\x14php_generic_services\x18* \x01(\x08:\x05\x66\x61lseR\x12phpGenericServices\x12%\n\ndeprecated\x18\x17 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12.\n\x10\x63\x63_enable_arenas\x18\x1f \x01(\x08:\x04trueR\x0e\x63\x63\x45nableArenas\x12*\n\x11objc_class_prefix\x18$ \x01(\tR\x0fobjcClassPrefix\x12)\n\x10\x63sharp_namespace\x18% \x01(\tR\x0f\x63sharpNamespace\x12!\n\x0cswift_prefix\x18\' \x01(\tR\x0bswiftPrefix\x12(\n\x10php_class_prefix\x18( \x01(\tR\x0ephpClassPrefix\x12#\n\rphp_namespace\x18) \x01(\tR\x0cphpNamespace\x12\x34\n\x16php_metadata_namespace\x18, \x01(\tR\x14phpMetadataNamespace\x12!\n\x0cruby_package\x18- \x01(\tR\x0brubyPackage\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\":\n\x0cOptimizeMode\x12\t\n\x05SPEED\x10\x01\x12\r\n\tCODE_SIZE\x10\x02\x12\x10\n\x0cLITE_RUNTIME\x10\x03*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08&\x10\'\"\xbb\x03\n\x0eMessageOptions\x12<\n\x17message_set_wire_format\x18\x01 \x01(\x08:\x05\x66\x61lseR\x14messageSetWireFormat\x12L\n\x1fno_standard_descriptor_accessor\x18\x02 \x01(\x08:\x05\x66\x61lseR\x1cnoStandardDescriptorAccessor\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x1b\n\tmap_entry\x18\x07 \x01(\x08R\x08mapEntry\x12V\n&deprecated_legacy_json_field_conflicts\x18\x0b \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\xb7\x08\n\x0c\x46ieldOptions\x12\x41\n\x05\x63type\x18\x01 \x01(\x0e\x32#.google.protobuf.FieldOptions.CType:\x06STRINGR\x05\x63type\x12\x16\n\x06packed\x18\x02 \x01(\x08R\x06packed\x12G\n\x06jstype\x18\x06 \x01(\x0e\x32$.google.protobuf.FieldOptions.JSType:\tJS_NORMALR\x06jstype\x12\x19\n\x04lazy\x18\x05 \x01(\x08:\x05\x66\x61lseR\x04lazy\x12.\n\x0funverified_lazy\x18\x0f \x01(\x08:\x05\x66\x61lseR\x0eunverifiedLazy\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x19\n\x04weak\x18\n \x01(\x08:\x05\x66\x61lseR\x04weak\x12(\n\x0c\x64\x65\x62ug_redact\x18\x10 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12K\n\tretention\x18\x11 \x01(\x0e\x32-.google.protobuf.FieldOptions.OptionRetentionR\tretention\x12\x46\n\x06target\x18\x12 \x01(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeR\x06target\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"/\n\x05\x43Type\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x43ORD\x10\x01\x12\x10\n\x0cSTRING_PIECE\x10\x02\"5\n\x06JSType\x12\r\n\tJS_NORMAL\x10\x00\x12\r\n\tJS_STRING\x10\x01\x12\r\n\tJS_NUMBER\x10\x02\"U\n\x0fOptionRetention\x12\x15\n\x11RETENTION_UNKNOWN\x10\x00\x12\x15\n\x11RETENTION_RUNTIME\x10\x01\x12\x14\n\x10RETENTION_SOURCE\x10\x02\"\x8c\x02\n\x10OptionTargetType\x12\x17\n\x13TARGET_TYPE_UNKNOWN\x10\x00\x12\x14\n\x10TARGET_TYPE_FILE\x10\x01\x12\x1f\n\x1bTARGET_TYPE_EXTENSION_RANGE\x10\x02\x12\x17\n\x13TARGET_TYPE_MESSAGE\x10\x03\x12\x15\n\x11TARGET_TYPE_FIELD\x10\x04\x12\x15\n\x11TARGET_TYPE_ONEOF\x10\x05\x12\x14\n\x10TARGET_TYPE_ENUM\x10\x06\x12\x1a\n\x16TARGET_TYPE_ENUM_ENTRY\x10\x07\x12\x17\n\x13TARGET_TYPE_SERVICE\x10\x08\x12\x16\n\x12TARGET_TYPE_METHOD\x10\t*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05\"s\n\x0cOneofOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x98\x02\n\x0b\x45numOptions\x12\x1f\n\x0b\x61llow_alias\x18\x02 \x01(\x08R\nallowAlias\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12V\n&deprecated_legacy_json_field_conflicts\x18\x06 \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x05\x10\x06\"\x9e\x01\n\x10\x45numValueOptions\x12%\n\ndeprecated\x18\x01 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9c\x01\n\x0eServiceOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xe0\x02\n\rMethodOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12q\n\x11idempotency_level\x18\" \x01(\x0e\x32/.google.protobuf.MethodOptions.IdempotencyLevel:\x13IDEMPOTENCY_UNKNOWNR\x10idempotencyLevel\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"P\n\x10IdempotencyLevel\x12\x17\n\x13IDEMPOTENCY_UNKNOWN\x10\x00\x12\x13\n\x0fNO_SIDE_EFFECTS\x10\x01\x12\x0e\n\nIDEMPOTENT\x10\x02*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9a\x03\n\x13UninterpretedOption\x12\x41\n\x04name\x18\x02 \x03(\x0b\x32-.google.protobuf.UninterpretedOption.NamePartR\x04name\x12)\n\x10identifier_value\x18\x03 \x01(\tR\x0fidentifierValue\x12,\n\x12positive_int_value\x18\x04 \x01(\x04R\x10positiveIntValue\x12,\n\x12negative_int_value\x18\x05 \x01(\x03R\x10negativeIntValue\x12!\n\x0c\x64ouble_value\x18\x06 \x01(\x01R\x0b\x64oubleValue\x12!\n\x0cstring_value\x18\x07 \x01(\x0cR\x0bstringValue\x12\'\n\x0f\x61ggregate_value\x18\x08 \x01(\tR\x0e\x61ggregateValue\x1aJ\n\x08NamePart\x12\x1b\n\tname_part\x18\x01 \x02(\tR\x08namePart\x12!\n\x0cis_extension\x18\x02 \x02(\x08R\x0bisExtension\"\xa7\x02\n\x0eSourceCodeInfo\x12\x44\n\x08location\x18\x01 \x03(\x0b\x32(.google.protobuf.SourceCodeInfo.LocationR\x08location\x1a\xce\x01\n\x08Location\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x16\n\x04span\x18\x02 \x03(\x05\x42\x02\x10\x01R\x04span\x12)\n\x10leading_comments\x18\x03 \x01(\tR\x0fleadingComments\x12+\n\x11trailing_comments\x18\x04 \x01(\tR\x10trailingComments\x12:\n\x19leading_detached_comments\x18\x06 \x03(\tR\x17leadingDetachedComments\"\xd0\x02\n\x11GeneratedCodeInfo\x12M\n\nannotation\x18\x01 \x03(\x0b\x32-.google.protobuf.GeneratedCodeInfo.AnnotationR\nannotation\x1a\xeb\x01\n\nAnnotation\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x1f\n\x0bsource_file\x18\x02 \x01(\tR\nsourceFile\x12\x14\n\x05\x62\x65gin\x18\x03 \x01(\x05R\x05\x62\x65gin\x12\x10\n\x03\x65nd\x18\x04 \x01(\x05R\x03\x65nd\x12R\n\x08semantic\x18\x05 \x01(\x0e\x32\x36.google.protobuf.GeneratedCodeInfo.Annotation.SemanticR\x08semantic\"(\n\x08Semantic\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SET\x10\x01\x12\t\n\x05\x41LIAS\x10\x02\x42~\n\x13\x63om.google.protobufB\x10\x44\x65scriptorProtosH\x01Z-google.golang.org/protobuf/types/descriptorpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1aGoogle.Protobuf.Reflection')
+  DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n google/protobuf/descriptor.proto\x12\x0fgoogle.protobuf\"M\n\x11\x46ileDescriptorSet\x12\x38\n\x04\x66ile\x18\x01 \x03(\x0b\x32$.google.protobuf.FileDescriptorProtoR\x04\x66ile\"\xfe\x04\n\x13\x46ileDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07package\x18\x02 \x01(\tR\x07package\x12\x1e\n\ndependency\x18\x03 \x03(\tR\ndependency\x12+\n\x11public_dependency\x18\n \x03(\x05R\x10publicDependency\x12\'\n\x0fweak_dependency\x18\x0b \x03(\x05R\x0eweakDependency\x12\x43\n\x0cmessage_type\x18\x04 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\x0bmessageType\x12\x41\n\tenum_type\x18\x05 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12\x41\n\x07service\x18\x06 \x03(\x0b\x32\'.google.protobuf.ServiceDescriptorProtoR\x07service\x12\x43\n\textension\x18\x07 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x36\n\x07options\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.FileOptionsR\x07options\x12I\n\x10source_code_info\x18\t \x01(\x0b\x32\x1f.google.protobuf.SourceCodeInfoR\x0esourceCodeInfo\x12\x16\n\x06syntax\x18\x0c \x01(\tR\x06syntax\x12\x18\n\x07\x65\x64ition\x18\r \x01(\tR\x07\x65\x64ition\"\xb9\x06\n\x0f\x44\x65scriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\x05\x66ield\x18\x02 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\x05\x66ield\x12\x43\n\textension\x18\x06 \x03(\x0b\x32%.google.protobuf.FieldDescriptorProtoR\textension\x12\x41\n\x0bnested_type\x18\x03 \x03(\x0b\x32 .google.protobuf.DescriptorProtoR\nnestedType\x12\x41\n\tenum_type\x18\x04 \x03(\x0b\x32$.google.protobuf.EnumDescriptorProtoR\x08\x65numType\x12X\n\x0f\x65xtension_range\x18\x05 \x03(\x0b\x32/.google.protobuf.DescriptorProto.ExtensionRangeR\x0e\x65xtensionRange\x12\x44\n\noneof_decl\x18\x08 \x03(\x0b\x32%.google.protobuf.OneofDescriptorProtoR\toneofDecl\x12\x39\n\x07options\x18\x07 \x01(\x0b\x32\x1f.google.protobuf.MessageOptionsR\x07options\x12U\n\x0ereserved_range\x18\t \x03(\x0b\x32..google.protobuf.DescriptorProto.ReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\n \x03(\tR\x0creservedName\x1az\n\x0e\x45xtensionRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x12@\n\x07options\x18\x03 \x01(\x0b\x32&.google.protobuf.ExtensionRangeOptionsR\x07options\x1a\x37\n\rReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\xad\x04\n\x15\x45xtensionRangeOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\x12Y\n\x0b\x64\x65\x63laration\x18\x02 \x03(\x0b\x32\x32.google.protobuf.ExtensionRangeOptions.DeclarationB\x03\x88\x01\x02R\x0b\x64\x65\x63laration\x12h\n\x0cverification\x18\x03 \x01(\x0e\x32\x38.google.protobuf.ExtensionRangeOptions.VerificationState:\nUNVERIFIEDR\x0cverification\x1a\xb3\x01\n\x0b\x44\x65\x63laration\x12\x16\n\x06number\x18\x01 \x01(\x05R\x06number\x12\x1b\n\tfull_name\x18\x02 \x01(\tR\x08\x66ullName\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x12#\n\x0bis_repeated\x18\x04 \x01(\x08\x42\x02\x18\x01R\nisRepeated\x12\x1a\n\x08reserved\x18\x05 \x01(\x08R\x08reserved\x12\x1a\n\x08repeated\x18\x06 \x01(\x08R\x08repeated\"4\n\x11VerificationState\x12\x0f\n\x0b\x44\x45\x43LARATION\x10\x00\x12\x0e\n\nUNVERIFIED\x10\x01*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xc1\x06\n\x14\x46ieldDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x41\n\x05label\x18\x04 \x01(\x0e\x32+.google.protobuf.FieldDescriptorProto.LabelR\x05label\x12>\n\x04type\x18\x05 \x01(\x0e\x32*.google.protobuf.FieldDescriptorProto.TypeR\x04type\x12\x1b\n\ttype_name\x18\x06 \x01(\tR\x08typeName\x12\x1a\n\x08\x65xtendee\x18\x02 \x01(\tR\x08\x65xtendee\x12#\n\rdefault_value\x18\x07 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1f\n\x0boneof_index\x18\t \x01(\x05R\noneofIndex\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12\x37\n\x07options\x18\x08 \x01(\x0b\x32\x1d.google.protobuf.FieldOptionsR\x07options\x12\'\n\x0fproto3_optional\x18\x11 \x01(\x08R\x0eproto3Optional\"\xb6\x02\n\x04Type\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"C\n\x05Label\x12\x12\n\x0eLABEL_OPTIONAL\x10\x01\x12\x12\n\x0eLABEL_REQUIRED\x10\x02\x12\x12\n\x0eLABEL_REPEATED\x10\x03\"c\n\x14OneofDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x37\n\x07options\x18\x02 \x01(\x0b\x32\x1d.google.protobuf.OneofOptionsR\x07options\"\xe3\x02\n\x13\x45numDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12?\n\x05value\x18\x02 \x03(\x0b\x32).google.protobuf.EnumValueDescriptorProtoR\x05value\x12\x36\n\x07options\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.EnumOptionsR\x07options\x12]\n\x0ereserved_range\x18\x04 \x03(\x0b\x32\x36.google.protobuf.EnumDescriptorProto.EnumReservedRangeR\rreservedRange\x12#\n\rreserved_name\x18\x05 \x03(\tR\x0creservedName\x1a;\n\x11\x45numReservedRange\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\"\x83\x01\n\x18\x45numValueDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12;\n\x07options\x18\x03 \x01(\x0b\x32!.google.protobuf.EnumValueOptionsR\x07options\"\xa7\x01\n\x16ServiceDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\x06method\x18\x02 \x03(\x0b\x32&.google.protobuf.MethodDescriptorProtoR\x06method\x12\x39\n\x07options\x18\x03 \x01(\x0b\x32\x1f.google.protobuf.ServiceOptionsR\x07options\"\x89\x02\n\x15MethodDescriptorProto\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ninput_type\x18\x02 \x01(\tR\tinputType\x12\x1f\n\x0boutput_type\x18\x03 \x01(\tR\noutputType\x12\x38\n\x07options\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.MethodOptionsR\x07options\x12\x30\n\x10\x63lient_streaming\x18\x05 \x01(\x08:\x05\x66\x61lseR\x0f\x63lientStreaming\x12\x30\n\x10server_streaming\x18\x06 \x01(\x08:\x05\x66\x61lseR\x0fserverStreaming\"\x91\t\n\x0b\x46ileOptions\x12!\n\x0cjava_package\x18\x01 \x01(\tR\x0bjavaPackage\x12\x30\n\x14java_outer_classname\x18\x08 \x01(\tR\x12javaOuterClassname\x12\x35\n\x13java_multiple_files\x18\n \x01(\x08:\x05\x66\x61lseR\x11javaMultipleFiles\x12\x44\n\x1djava_generate_equals_and_hash\x18\x14 \x01(\x08\x42\x02\x18\x01R\x19javaGenerateEqualsAndHash\x12:\n\x16java_string_check_utf8\x18\x1b \x01(\x08:\x05\x66\x61lseR\x13javaStringCheckUtf8\x12S\n\x0coptimize_for\x18\t \x01(\x0e\x32).google.protobuf.FileOptions.OptimizeMode:\x05SPEEDR\x0boptimizeFor\x12\x1d\n\ngo_package\x18\x0b \x01(\tR\tgoPackage\x12\x35\n\x13\x63\x63_generic_services\x18\x10 \x01(\x08:\x05\x66\x61lseR\x11\x63\x63GenericServices\x12\x39\n\x15java_generic_services\x18\x11 \x01(\x08:\x05\x66\x61lseR\x13javaGenericServices\x12\x35\n\x13py_generic_services\x18\x12 \x01(\x08:\x05\x66\x61lseR\x11pyGenericServices\x12\x37\n\x14php_generic_services\x18* \x01(\x08:\x05\x66\x61lseR\x12phpGenericServices\x12%\n\ndeprecated\x18\x17 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12.\n\x10\x63\x63_enable_arenas\x18\x1f \x01(\x08:\x04trueR\x0e\x63\x63\x45nableArenas\x12*\n\x11objc_class_prefix\x18$ \x01(\tR\x0fobjcClassPrefix\x12)\n\x10\x63sharp_namespace\x18% \x01(\tR\x0f\x63sharpNamespace\x12!\n\x0cswift_prefix\x18\' \x01(\tR\x0bswiftPrefix\x12(\n\x10php_class_prefix\x18( \x01(\tR\x0ephpClassPrefix\x12#\n\rphp_namespace\x18) \x01(\tR\x0cphpNamespace\x12\x34\n\x16php_metadata_namespace\x18, \x01(\tR\x14phpMetadataNamespace\x12!\n\x0cruby_package\x18- \x01(\tR\x0brubyPackage\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\":\n\x0cOptimizeMode\x12\t\n\x05SPEED\x10\x01\x12\r\n\tCODE_SIZE\x10\x02\x12\x10\n\x0cLITE_RUNTIME\x10\x03*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08&\x10\'\"\xbb\x03\n\x0eMessageOptions\x12<\n\x17message_set_wire_format\x18\x01 \x01(\x08:\x05\x66\x61lseR\x14messageSetWireFormat\x12L\n\x1fno_standard_descriptor_accessor\x18\x02 \x01(\x08:\x05\x66\x61lseR\x1cnoStandardDescriptorAccessor\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x1b\n\tmap_entry\x18\x07 \x01(\x08R\x08mapEntry\x12V\n&deprecated_legacy_json_field_conflicts\x18\x0b \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\x85\t\n\x0c\x46ieldOptions\x12\x41\n\x05\x63type\x18\x01 \x01(\x0e\x32#.google.protobuf.FieldOptions.CType:\x06STRINGR\x05\x63type\x12\x16\n\x06packed\x18\x02 \x01(\x08R\x06packed\x12G\n\x06jstype\x18\x06 \x01(\x0e\x32$.google.protobuf.FieldOptions.JSType:\tJS_NORMALR\x06jstype\x12\x19\n\x04lazy\x18\x05 \x01(\x08:\x05\x66\x61lseR\x04lazy\x12.\n\x0funverified_lazy\x18\x0f \x01(\x08:\x05\x66\x61lseR\x0eunverifiedLazy\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12\x19\n\x04weak\x18\n \x01(\x08:\x05\x66\x61lseR\x04weak\x12(\n\x0c\x64\x65\x62ug_redact\x18\x10 \x01(\x08:\x05\x66\x61lseR\x0b\x64\x65\x62ugRedact\x12K\n\tretention\x18\x11 \x01(\x0e\x32-.google.protobuf.FieldOptions.OptionRetentionR\tretention\x12J\n\x06target\x18\x12 \x01(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeB\x02\x18\x01R\x06target\x12H\n\x07targets\x18\x13 \x03(\x0e\x32..google.protobuf.FieldOptions.OptionTargetTypeR\x07targets\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"/\n\x05\x43Type\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x43ORD\x10\x01\x12\x10\n\x0cSTRING_PIECE\x10\x02\"5\n\x06JSType\x12\r\n\tJS_NORMAL\x10\x00\x12\r\n\tJS_STRING\x10\x01\x12\r\n\tJS_NUMBER\x10\x02\"U\n\x0fOptionRetention\x12\x15\n\x11RETENTION_UNKNOWN\x10\x00\x12\x15\n\x11RETENTION_RUNTIME\x10\x01\x12\x14\n\x10RETENTION_SOURCE\x10\x02\"\x8c\x02\n\x10OptionTargetType\x12\x17\n\x13TARGET_TYPE_UNKNOWN\x10\x00\x12\x14\n\x10TARGET_TYPE_FILE\x10\x01\x12\x1f\n\x1bTARGET_TYPE_EXTENSION_RANGE\x10\x02\x12\x17\n\x13TARGET_TYPE_MESSAGE\x10\x03\x12\x15\n\x11TARGET_TYPE_FIELD\x10\x04\x12\x15\n\x11TARGET_TYPE_ONEOF\x10\x05\x12\x14\n\x10TARGET_TYPE_ENUM\x10\x06\x12\x1a\n\x16TARGET_TYPE_ENUM_ENTRY\x10\x07\x12\x17\n\x13TARGET_TYPE_SERVICE\x10\x08\x12\x16\n\x12TARGET_TYPE_METHOD\x10\t*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x04\x10\x05\"s\n\x0cOneofOptions\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x98\x02\n\x0b\x45numOptions\x12\x1f\n\x0b\x61llow_alias\x18\x02 \x01(\x08R\nallowAlias\x12%\n\ndeprecated\x18\x03 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12V\n&deprecated_legacy_json_field_conflicts\x18\x06 \x01(\x08\x42\x02\x18\x01R\"deprecatedLegacyJsonFieldConflicts\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02J\x04\x08\x05\x10\x06\"\x9e\x01\n\x10\x45numValueOptions\x12%\n\ndeprecated\x18\x01 \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9c\x01\n\x0eServiceOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\xe0\x02\n\rMethodOptions\x12%\n\ndeprecated\x18! \x01(\x08:\x05\x66\x61lseR\ndeprecated\x12q\n\x11idempotency_level\x18\" \x01(\x0e\x32/.google.protobuf.MethodOptions.IdempotencyLevel:\x13IDEMPOTENCY_UNKNOWNR\x10idempotencyLevel\x12X\n\x14uninterpreted_option\x18\xe7\x07 \x03(\x0b\x32$.google.protobuf.UninterpretedOptionR\x13uninterpretedOption\"P\n\x10IdempotencyLevel\x12\x17\n\x13IDEMPOTENCY_UNKNOWN\x10\x00\x12\x13\n\x0fNO_SIDE_EFFECTS\x10\x01\x12\x0e\n\nIDEMPOTENT\x10\x02*\t\x08\xe8\x07\x10\x80\x80\x80\x80\x02\"\x9a\x03\n\x13UninterpretedOption\x12\x41\n\x04name\x18\x02 \x03(\x0b\x32-.google.protobuf.UninterpretedOption.NamePartR\x04name\x12)\n\x10identifier_value\x18\x03 \x01(\tR\x0fidentifierValue\x12,\n\x12positive_int_value\x18\x04 \x01(\x04R\x10positiveIntValue\x12,\n\x12negative_int_value\x18\x05 \x01(\x03R\x10negativeIntValue\x12!\n\x0c\x64ouble_value\x18\x06 \x01(\x01R\x0b\x64oubleValue\x12!\n\x0cstring_value\x18\x07 \x01(\x0cR\x0bstringValue\x12\'\n\x0f\x61ggregate_value\x18\x08 \x01(\tR\x0e\x61ggregateValue\x1aJ\n\x08NamePart\x12\x1b\n\tname_part\x18\x01 \x02(\tR\x08namePart\x12!\n\x0cis_extension\x18\x02 \x02(\x08R\x0bisExtension\"\xa7\x02\n\x0eSourceCodeInfo\x12\x44\n\x08location\x18\x01 \x03(\x0b\x32(.google.protobuf.SourceCodeInfo.LocationR\x08location\x1a\xce\x01\n\x08Location\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x16\n\x04span\x18\x02 \x03(\x05\x42\x02\x10\x01R\x04span\x12)\n\x10leading_comments\x18\x03 \x01(\tR\x0fleadingComments\x12+\n\x11trailing_comments\x18\x04 \x01(\tR\x10trailingComments\x12:\n\x19leading_detached_comments\x18\x06 \x03(\tR\x17leadingDetachedComments\"\xd0\x02\n\x11GeneratedCodeInfo\x12M\n\nannotation\x18\x01 \x03(\x0b\x32-.google.protobuf.GeneratedCodeInfo.AnnotationR\nannotation\x1a\xeb\x01\n\nAnnotation\x12\x16\n\x04path\x18\x01 \x03(\x05\x42\x02\x10\x01R\x04path\x12\x1f\n\x0bsource_file\x18\x02 \x01(\tR\nsourceFile\x12\x14\n\x05\x62\x65gin\x18\x03 \x01(\x05R\x05\x62\x65gin\x12\x10\n\x03\x65nd\x18\x04 \x01(\x05R\x03\x65nd\x12R\n\x08semantic\x18\x05 \x01(\x0e\x32\x36.google.protobuf.GeneratedCodeInfo.Annotation.SemanticR\x08semantic\"(\n\x08Semantic\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SET\x10\x01\x12\t\n\x05\x41LIAS\x10\x02\x42~\n\x13\x63om.google.protobufB\x10\x44\x65scriptorProtosH\x01Z-google.golang.org/protobuf/types/descriptorpb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1aGoogle.Protobuf.Reflection')
 
 _globals = globals()
 if _descriptor._USE_C_DESCRIPTORS == False:
+  _EXTENSIONRANGEOPTIONS_VERIFICATIONSTATE = _descriptor.EnumDescriptor(
+    name='VerificationState',
+    full_name='google.protobuf.ExtensionRangeOptions.VerificationState',
+    filename=None,
+    file=DESCRIPTOR,
+    create_key=_descriptor._internal_create_key,
+    values=[
+      _descriptor.EnumValueDescriptor(
+        name='DECLARATION', index=0, number=0,
+        serialized_options=None,
+        type=None,
+        create_key=_descriptor._internal_create_key),
+      _descriptor.EnumValueDescriptor(
+        name='UNVERIFIED', index=1, number=1,
+        serialized_options=None,
+        type=None,
+        create_key=_descriptor._internal_create_key),
+    ],
+    containing_type=None,
+    serialized_options=None,
+  )
+  _sym_db.RegisterEnumDescriptor(_EXTENSIONRANGEOPTIONS_VERIFICATIONSTATE)
+
   _FIELDDESCRIPTORPROTO_TYPE = _descriptor.EnumDescriptor(
     name='Type',
     full_name='google.protobuf.FieldDescriptorProto.Type',
     filename=None,
     file=DESCRIPTOR,
     create_key=_descriptor._internal_create_key,
     values=[
@@ -702,14 +725,78 @@
     syntax='proto2',
     extension_ranges=[],
     oneofs=[
     ],
   )
 
 
+  _EXTENSIONRANGEOPTIONS_DECLARATION = _descriptor.Descriptor(
+    name='Declaration',
+    full_name='google.protobuf.ExtensionRangeOptions.Declaration',
+    filename=None,
+    file=DESCRIPTOR,
+    containing_type=None,
+    create_key=_descriptor._internal_create_key,
+    fields=[
+      _descriptor.FieldDescriptor(
+        name='number', full_name='google.protobuf.ExtensionRangeOptions.Declaration.number', index=0,
+        number=1, type=5, cpp_type=1, label=1,
+        has_default_value=False, default_value=0,
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='number', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='full_name', full_name='google.protobuf.ExtensionRangeOptions.Declaration.full_name', index=1,
+        number=2, type=9, cpp_type=9, label=1,
+        has_default_value=False, default_value=b"".decode('utf-8'),
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='fullName', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='type', full_name='google.protobuf.ExtensionRangeOptions.Declaration.type', index=2,
+        number=3, type=9, cpp_type=9, label=1,
+        has_default_value=False, default_value=b"".decode('utf-8'),
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='type', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='is_repeated', full_name='google.protobuf.ExtensionRangeOptions.Declaration.is_repeated', index=3,
+        number=4, type=8, cpp_type=7, label=1,
+        has_default_value=False, default_value=False,
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='isRepeated', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='reserved', full_name='google.protobuf.ExtensionRangeOptions.Declaration.reserved', index=4,
+        number=5, type=8, cpp_type=7, label=1,
+        has_default_value=False, default_value=False,
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='reserved', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='repeated', full_name='google.protobuf.ExtensionRangeOptions.Declaration.repeated', index=5,
+        number=6, type=8, cpp_type=7, label=1,
+        has_default_value=False, default_value=False,
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='repeated', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    ],
+    extensions=[
+    ],
+    nested_types=[],
+    enum_types=[
+    ],
+    serialized_options=None,
+    is_extendable=False,
+    syntax='proto2',
+    extension_ranges=[],
+    oneofs=[
+    ],
+  )
+
   _EXTENSIONRANGEOPTIONS = _descriptor.Descriptor(
     name='ExtensionRangeOptions',
     full_name='google.protobuf.ExtensionRangeOptions',
     filename=None,
     file=DESCRIPTOR,
     containing_type=None,
     create_key=_descriptor._internal_create_key,
@@ -717,19 +804,34 @@
       _descriptor.FieldDescriptor(
         name='uninterpreted_option', full_name='google.protobuf.ExtensionRangeOptions.uninterpreted_option', index=0,
         number=999, type=11, cpp_type=10, label=3,
         has_default_value=False, default_value=[],
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
         serialized_options=None, json_name='uninterpretedOption', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='declaration', full_name='google.protobuf.ExtensionRangeOptions.declaration', index=1,
+        number=2, type=11, cpp_type=10, label=3,
+        has_default_value=False, default_value=[],
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='declaration', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='verification', full_name='google.protobuf.ExtensionRangeOptions.verification', index=2,
+        number=3, type=14, cpp_type=8, label=1,
+        has_default_value=True, default_value=1,
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='verification', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     ],
     extensions=[
     ],
-    nested_types=[],
+    nested_types=[_EXTENSIONRANGEOPTIONS_DECLARATION, ],
     enum_types=[
+      _EXTENSIONRANGEOPTIONS_VERIFICATIONSTATE,
     ],
     serialized_options=None,
     is_extendable=True,
     syntax='proto2',
     extension_ranges=[(1000, 536870912), ],
     oneofs=[
     ],
@@ -1433,15 +1535,22 @@
         name='target', full_name='google.protobuf.FieldOptions.target', index=9,
         number=18, type=14, cpp_type=8, label=1,
         has_default_value=False, default_value=0,
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
         serialized_options=None, json_name='target', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
       _descriptor.FieldDescriptor(
-        name='uninterpreted_option', full_name='google.protobuf.FieldOptions.uninterpreted_option', index=10,
+        name='targets', full_name='google.protobuf.FieldOptions.targets', index=10,
+        number=19, type=14, cpp_type=8, label=3,
+        has_default_value=False, default_value=[],
+        message_type=None, enum_type=None, containing_type=None,
+        is_extension=False, extension_scope=None,
+        serialized_options=None, json_name='targets', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      _descriptor.FieldDescriptor(
+        name='uninterpreted_option', full_name='google.protobuf.FieldOptions.uninterpreted_option', index=11,
         number=999, type=11, cpp_type=10, label=3,
         has_default_value=False, default_value=[],
         message_type=None, enum_type=None, containing_type=None,
         is_extension=False, extension_scope=None,
         serialized_options=None, json_name='uninterpretedOption', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     ],
     extensions=[
@@ -1958,15 +2067,19 @@
   _DESCRIPTORPROTO.fields_by_name['extension'].message_type = _FIELDDESCRIPTORPROTO
   _DESCRIPTORPROTO.fields_by_name['nested_type'].message_type = _DESCRIPTORPROTO
   _DESCRIPTORPROTO.fields_by_name['enum_type'].message_type = _ENUMDESCRIPTORPROTO
   _DESCRIPTORPROTO.fields_by_name['extension_range'].message_type = _DESCRIPTORPROTO_EXTENSIONRANGE
   _DESCRIPTORPROTO.fields_by_name['oneof_decl'].message_type = _ONEOFDESCRIPTORPROTO
   _DESCRIPTORPROTO.fields_by_name['options'].message_type = _MESSAGEOPTIONS
   _DESCRIPTORPROTO.fields_by_name['reserved_range'].message_type = _DESCRIPTORPROTO_RESERVEDRANGE
+  _EXTENSIONRANGEOPTIONS_DECLARATION.containing_type = _EXTENSIONRANGEOPTIONS
   _EXTENSIONRANGEOPTIONS.fields_by_name['uninterpreted_option'].message_type = _UNINTERPRETEDOPTION
+  _EXTENSIONRANGEOPTIONS.fields_by_name['declaration'].message_type = _EXTENSIONRANGEOPTIONS_DECLARATION
+  _EXTENSIONRANGEOPTIONS.fields_by_name['verification'].enum_type = _EXTENSIONRANGEOPTIONS_VERIFICATIONSTATE
+  _EXTENSIONRANGEOPTIONS_VERIFICATIONSTATE.containing_type = _EXTENSIONRANGEOPTIONS
   _FIELDDESCRIPTORPROTO.fields_by_name['label'].enum_type = _FIELDDESCRIPTORPROTO_LABEL
   _FIELDDESCRIPTORPROTO.fields_by_name['type'].enum_type = _FIELDDESCRIPTORPROTO_TYPE
   _FIELDDESCRIPTORPROTO.fields_by_name['options'].message_type = _FIELDOPTIONS
   _FIELDDESCRIPTORPROTO_TYPE.containing_type = _FIELDDESCRIPTORPROTO
   _FIELDDESCRIPTORPROTO_LABEL.containing_type = _FIELDDESCRIPTORPROTO
   _ONEOFDESCRIPTORPROTO.fields_by_name['options'].message_type = _ONEOFOPTIONS
   _ENUMDESCRIPTORPROTO_ENUMRESERVEDRANGE.containing_type = _ENUMDESCRIPTORPROTO
@@ -1981,14 +2094,15 @@
   _FILEOPTIONS.fields_by_name['uninterpreted_option'].message_type = _UNINTERPRETEDOPTION
   _FILEOPTIONS_OPTIMIZEMODE.containing_type = _FILEOPTIONS
   _MESSAGEOPTIONS.fields_by_name['uninterpreted_option'].message_type = _UNINTERPRETEDOPTION
   _FIELDOPTIONS.fields_by_name['ctype'].enum_type = _FIELDOPTIONS_CTYPE
   _FIELDOPTIONS.fields_by_name['jstype'].enum_type = _FIELDOPTIONS_JSTYPE
   _FIELDOPTIONS.fields_by_name['retention'].enum_type = _FIELDOPTIONS_OPTIONRETENTION
   _FIELDOPTIONS.fields_by_name['target'].enum_type = _FIELDOPTIONS_OPTIONTARGETTYPE
+  _FIELDOPTIONS.fields_by_name['targets'].enum_type = _FIELDOPTIONS_OPTIONTARGETTYPE
   _FIELDOPTIONS.fields_by_name['uninterpreted_option'].message_type = _UNINTERPRETEDOPTION
   _FIELDOPTIONS_CTYPE.containing_type = _FIELDOPTIONS
   _FIELDOPTIONS_JSTYPE.containing_type = _FIELDOPTIONS
   _FIELDOPTIONS_OPTIONRETENTION.containing_type = _FIELDOPTIONS
   _FIELDOPTIONS_OPTIONTARGETTYPE.containing_type = _FIELDOPTIONS
   _ONEOFOPTIONS.fields_by_name['uninterpreted_option'].message_type = _UNINTERPRETEDOPTION
   _ENUMOPTIONS.fields_by_name['uninterpreted_option'].message_type = _UNINTERPRETEDOPTION
@@ -2040,70 +2154,74 @@
   _globals['_FILEDESCRIPTORPROTO']._serialized_end=771
   _globals['_DESCRIPTORPROTO']._serialized_start=774
   _globals['_DESCRIPTORPROTO']._serialized_end=1599
   _globals['_DESCRIPTORPROTO_EXTENSIONRANGE']._serialized_start=1420
   _globals['_DESCRIPTORPROTO_EXTENSIONRANGE']._serialized_end=1542
   _globals['_DESCRIPTORPROTO_RESERVEDRANGE']._serialized_start=1544
   _globals['_DESCRIPTORPROTO_RESERVEDRANGE']._serialized_end=1599
-  _globals['_EXTENSIONRANGEOPTIONS']._serialized_start=1601
-  _globals['_EXTENSIONRANGEOPTIONS']._serialized_end=1725
-  _globals['_FIELDDESCRIPTORPROTO']._serialized_start=1728
-  _globals['_FIELDDESCRIPTORPROTO']._serialized_end=2561
-  _globals['_FIELDDESCRIPTORPROTO_TYPE']._serialized_start=2182
-  _globals['_FIELDDESCRIPTORPROTO_TYPE']._serialized_end=2492
-  _globals['_FIELDDESCRIPTORPROTO_LABEL']._serialized_start=2494
-  _globals['_FIELDDESCRIPTORPROTO_LABEL']._serialized_end=2561
-  _globals['_ONEOFDESCRIPTORPROTO']._serialized_start=2563
-  _globals['_ONEOFDESCRIPTORPROTO']._serialized_end=2662
-  _globals['_ENUMDESCRIPTORPROTO']._serialized_start=2665
-  _globals['_ENUMDESCRIPTORPROTO']._serialized_end=3020
-  _globals['_ENUMDESCRIPTORPROTO_ENUMRESERVEDRANGE']._serialized_start=2961
-  _globals['_ENUMDESCRIPTORPROTO_ENUMRESERVEDRANGE']._serialized_end=3020
-  _globals['_ENUMVALUEDESCRIPTORPROTO']._serialized_start=3023
-  _globals['_ENUMVALUEDESCRIPTORPROTO']._serialized_end=3154
-  _globals['_SERVICEDESCRIPTORPROTO']._serialized_start=3157
-  _globals['_SERVICEDESCRIPTORPROTO']._serialized_end=3324
-  _globals['_METHODDESCRIPTORPROTO']._serialized_start=3327
-  _globals['_METHODDESCRIPTORPROTO']._serialized_end=3592
-  _globals['_FILEOPTIONS']._serialized_start=3595
-  _globals['_FILEOPTIONS']._serialized_end=4764
-  _globals['_FILEOPTIONS_OPTIMIZEMODE']._serialized_start=4689
-  _globals['_FILEOPTIONS_OPTIMIZEMODE']._serialized_end=4747
-  _globals['_MESSAGEOPTIONS']._serialized_start=4767
-  _globals['_MESSAGEOPTIONS']._serialized_end=5210
-  _globals['_FIELDOPTIONS']._serialized_start=5213
-  _globals['_FIELDOPTIONS']._serialized_end=6292
-  _globals['_FIELDOPTIONS_CTYPE']._serialized_start=5815
-  _globals['_FIELDOPTIONS_CTYPE']._serialized_end=5862
-  _globals['_FIELDOPTIONS_JSTYPE']._serialized_start=5864
-  _globals['_FIELDOPTIONS_JSTYPE']._serialized_end=5917
-  _globals['_FIELDOPTIONS_OPTIONRETENTION']._serialized_start=5919
-  _globals['_FIELDOPTIONS_OPTIONRETENTION']._serialized_end=6004
-  _globals['_FIELDOPTIONS_OPTIONTARGETTYPE']._serialized_start=6007
-  _globals['_FIELDOPTIONS_OPTIONTARGETTYPE']._serialized_end=6275
-  _globals['_ONEOFOPTIONS']._serialized_start=6294
-  _globals['_ONEOFOPTIONS']._serialized_end=6409
-  _globals['_ENUMOPTIONS']._serialized_start=6412
-  _globals['_ENUMOPTIONS']._serialized_end=6692
-  _globals['_ENUMVALUEOPTIONS']._serialized_start=6695
-  _globals['_ENUMVALUEOPTIONS']._serialized_end=6853
-  _globals['_SERVICEOPTIONS']._serialized_start=6856
-  _globals['_SERVICEOPTIONS']._serialized_end=7012
-  _globals['_METHODOPTIONS']._serialized_start=7015
-  _globals['_METHODOPTIONS']._serialized_end=7367
-  _globals['_METHODOPTIONS_IDEMPOTENCYLEVEL']._serialized_start=7276
-  _globals['_METHODOPTIONS_IDEMPOTENCYLEVEL']._serialized_end=7356
-  _globals['_UNINTERPRETEDOPTION']._serialized_start=7370
-  _globals['_UNINTERPRETEDOPTION']._serialized_end=7780
-  _globals['_UNINTERPRETEDOPTION_NAMEPART']._serialized_start=7706
-  _globals['_UNINTERPRETEDOPTION_NAMEPART']._serialized_end=7780
-  _globals['_SOURCECODEINFO']._serialized_start=7783
-  _globals['_SOURCECODEINFO']._serialized_end=8078
-  _globals['_SOURCECODEINFO_LOCATION']._serialized_start=7872
-  _globals['_SOURCECODEINFO_LOCATION']._serialized_end=8078
-  _globals['_GENERATEDCODEINFO']._serialized_start=8081
-  _globals['_GENERATEDCODEINFO']._serialized_end=8417
-  _globals['_GENERATEDCODEINFO_ANNOTATION']._serialized_start=8182
-  _globals['_GENERATEDCODEINFO_ANNOTATION']._serialized_end=8417
-  _globals['_GENERATEDCODEINFO_ANNOTATION_SEMANTIC']._serialized_start=8377
-  _globals['_GENERATEDCODEINFO_ANNOTATION_SEMANTIC']._serialized_end=8417
+  _globals['_EXTENSIONRANGEOPTIONS']._serialized_start=1602
+  _globals['_EXTENSIONRANGEOPTIONS']._serialized_end=2159
+  _globals['_EXTENSIONRANGEOPTIONS_DECLARATION']._serialized_start=1915
+  _globals['_EXTENSIONRANGEOPTIONS_DECLARATION']._serialized_end=2094
+  _globals['_EXTENSIONRANGEOPTIONS_VERIFICATIONSTATE']._serialized_start=2096
+  _globals['_EXTENSIONRANGEOPTIONS_VERIFICATIONSTATE']._serialized_end=2148
+  _globals['_FIELDDESCRIPTORPROTO']._serialized_start=2162
+  _globals['_FIELDDESCRIPTORPROTO']._serialized_end=2995
+  _globals['_FIELDDESCRIPTORPROTO_TYPE']._serialized_start=2616
+  _globals['_FIELDDESCRIPTORPROTO_TYPE']._serialized_end=2926
+  _globals['_FIELDDESCRIPTORPROTO_LABEL']._serialized_start=2928
+  _globals['_FIELDDESCRIPTORPROTO_LABEL']._serialized_end=2995
+  _globals['_ONEOFDESCRIPTORPROTO']._serialized_start=2997
+  _globals['_ONEOFDESCRIPTORPROTO']._serialized_end=3096
+  _globals['_ENUMDESCRIPTORPROTO']._serialized_start=3099
+  _globals['_ENUMDESCRIPTORPROTO']._serialized_end=3454
+  _globals['_ENUMDESCRIPTORPROTO_ENUMRESERVEDRANGE']._serialized_start=3395
+  _globals['_ENUMDESCRIPTORPROTO_ENUMRESERVEDRANGE']._serialized_end=3454
+  _globals['_ENUMVALUEDESCRIPTORPROTO']._serialized_start=3457
+  _globals['_ENUMVALUEDESCRIPTORPROTO']._serialized_end=3588
+  _globals['_SERVICEDESCRIPTORPROTO']._serialized_start=3591
+  _globals['_SERVICEDESCRIPTORPROTO']._serialized_end=3758
+  _globals['_METHODDESCRIPTORPROTO']._serialized_start=3761
+  _globals['_METHODDESCRIPTORPROTO']._serialized_end=4026
+  _globals['_FILEOPTIONS']._serialized_start=4029
+  _globals['_FILEOPTIONS']._serialized_end=5198
+  _globals['_FILEOPTIONS_OPTIMIZEMODE']._serialized_start=5123
+  _globals['_FILEOPTIONS_OPTIMIZEMODE']._serialized_end=5181
+  _globals['_MESSAGEOPTIONS']._serialized_start=5201
+  _globals['_MESSAGEOPTIONS']._serialized_end=5644
+  _globals['_FIELDOPTIONS']._serialized_start=5647
+  _globals['_FIELDOPTIONS']._serialized_end=6804
+  _globals['_FIELDOPTIONS_CTYPE']._serialized_start=6327
+  _globals['_FIELDOPTIONS_CTYPE']._serialized_end=6374
+  _globals['_FIELDOPTIONS_JSTYPE']._serialized_start=6376
+  _globals['_FIELDOPTIONS_JSTYPE']._serialized_end=6429
+  _globals['_FIELDOPTIONS_OPTIONRETENTION']._serialized_start=6431
+  _globals['_FIELDOPTIONS_OPTIONRETENTION']._serialized_end=6516
+  _globals['_FIELDOPTIONS_OPTIONTARGETTYPE']._serialized_start=6519
+  _globals['_FIELDOPTIONS_OPTIONTARGETTYPE']._serialized_end=6787
+  _globals['_ONEOFOPTIONS']._serialized_start=6806
+  _globals['_ONEOFOPTIONS']._serialized_end=6921
+  _globals['_ENUMOPTIONS']._serialized_start=6924
+  _globals['_ENUMOPTIONS']._serialized_end=7204
+  _globals['_ENUMVALUEOPTIONS']._serialized_start=7207
+  _globals['_ENUMVALUEOPTIONS']._serialized_end=7365
+  _globals['_SERVICEOPTIONS']._serialized_start=7368
+  _globals['_SERVICEOPTIONS']._serialized_end=7524
+  _globals['_METHODOPTIONS']._serialized_start=7527
+  _globals['_METHODOPTIONS']._serialized_end=7879
+  _globals['_METHODOPTIONS_IDEMPOTENCYLEVEL']._serialized_start=7788
+  _globals['_METHODOPTIONS_IDEMPOTENCYLEVEL']._serialized_end=7868
+  _globals['_UNINTERPRETEDOPTION']._serialized_start=7882
+  _globals['_UNINTERPRETEDOPTION']._serialized_end=8292
+  _globals['_UNINTERPRETEDOPTION_NAMEPART']._serialized_start=8218
+  _globals['_UNINTERPRETEDOPTION_NAMEPART']._serialized_end=8292
+  _globals['_SOURCECODEINFO']._serialized_start=8295
+  _globals['_SOURCECODEINFO']._serialized_end=8590
+  _globals['_SOURCECODEINFO_LOCATION']._serialized_start=8384
+  _globals['_SOURCECODEINFO_LOCATION']._serialized_end=8590
+  _globals['_GENERATEDCODEINFO']._serialized_start=8593
+  _globals['_GENERATEDCODEINFO']._serialized_end=8929
+  _globals['_GENERATEDCODEINFO_ANNOTATION']._serialized_start=8694
+  _globals['_GENERATEDCODEINFO_ANNOTATION']._serialized_end=8929
+  _globals['_GENERATEDCODEINFO_ANNOTATION_SEMANTIC']._serialized_start=8889
+  _globals['_GENERATEDCODEINFO_ANNOTATION_SEMANTIC']._serialized_end=8929
 # @@protoc_insertion_point(module_scope)
```

### Comparing `protobuf-4.22.3/google/protobuf/descriptor_pool.py` & `protobuf-4.23.0rc2/google/protobuf/descriptor_pool.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/duration_pb2.py` & `protobuf-4.23.0rc2/google/protobuf/duration_pb2.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/duration.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-4.22.3/google/protobuf/empty_pb2.py` & `protobuf-4.23.0rc2/google/protobuf/empty_pb2.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/empty.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-4.22.3/google/protobuf/field_mask_pb2.py` & `protobuf-4.23.0rc2/google/protobuf/field_mask_pb2.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/field_mask.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-4.22.3/google/protobuf/internal/__init__.py` & `protobuf-4.23.0rc2/google/protobuf/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/_parameterized.py` & `protobuf-4.23.0rc2/google/protobuf/internal/_parameterized.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/api_implementation.py` & `protobuf-4.23.0rc2/google/protobuf/internal/api_implementation.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/builder.py` & `protobuf-4.23.0rc2/google/protobuf/internal/builder.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/containers.py` & `protobuf-4.23.0rc2/google/protobuf/internal/containers.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/decoder.py` & `protobuf-4.23.0rc2/google/protobuf/internal/decoder.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/encoder.py` & `protobuf-4.23.0rc2/google/protobuf/internal/encoder.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/enum_type_wrapper.py` & `protobuf-4.23.0rc2/google/protobuf/internal/enum_type_wrapper.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/extension_dict.py` & `protobuf-4.23.0rc2/google/protobuf/internal/extension_dict.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/field_mask.py` & `protobuf-4.23.0rc2/google/protobuf/internal/field_mask.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/message_listener.py` & `protobuf-4.23.0rc2/google/protobuf/internal/message_listener.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/python_message.py` & `protobuf-4.23.0rc2/google/protobuf/internal/python_message.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/testing_refleaks.py` & `protobuf-4.23.0rc2/google/protobuf/internal/testing_refleaks.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/type_checkers.py` & `protobuf-4.23.0rc2/google/protobuf/internal/type_checkers.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/well_known_types.py` & `protobuf-4.23.0rc2/google/protobuf/internal/well_known_types.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/internal/wire_format.py` & `protobuf-4.23.0rc2/google/protobuf/internal/wire_format.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/json_format.py` & `protobuf-4.23.0rc2/google/protobuf/json_format.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/message.py` & `protobuf-4.23.0rc2/google/protobuf/message.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/message_factory.py` & `protobuf-4.23.0rc2/google/protobuf/message_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,36 +159,34 @@
 
     Args:
       descriptor: The descriptor to build from.
 
     Returns:
       A class describing the passed in descriptor.
     """
-    # TODO(b/258832141): add this warning
-    # warnings.warn('MessageFactory class is deprecated. Please use '
-    #               'GetMessageClass() instead of MessageFactory.GetPrototype. '
-    #               'MessageFactory class will be removed after 2024.')
+    warnings.warn('MessageFactory class is deprecated. Please use '
+                  'GetMessageClass() instead of MessageFactory.GetPrototype. '
+                  'MessageFactory class will be removed after 2024.')
     return GetMessageClass(descriptor)
 
   def CreatePrototype(self, descriptor):
     """Builds a proto2 message class based on the passed in descriptor.
 
     Don't call this function directly, it always creates a new class. Call
     GetMessageClass() instead.
 
     Args:
       descriptor: The descriptor to build from.
 
     Returns:
       A class describing the passed in descriptor.
     """
-    # TODO(b/258832141): add this warning
-    # warnings.warn('Directly call CreatePrototype is wrong. Please use '
-    #               'GetMessageClass() method instead. Directly use '
-    #               'CreatePrototype will raise error after July 2023.')
+    warnings.warn('Directly call CreatePrototype is wrong. Please use '
+                  'GetMessageClass() method instead. Directly use '
+                  'CreatePrototype will raise error after July 2023.')
     return _InternalCreateMessageClass(descriptor)
 
   def GetMessages(self, files):
     """Gets all the messages from a specified file.
 
     This will find and resolve dependencies, failing if the descriptor
     pool cannot satisfy them.
@@ -197,19 +195,18 @@
       files: The file names to extract messages from.
 
     Returns:
       A dictionary mapping proto names to the message classes. This will include
       any dependent messages as well as any messages defined in the same file as
       a specified message.
     """
-    # TODO(b/258832141): add this warning
-    # warnings.warn('MessageFactory class is deprecated. Please use '
-    #               'GetMessageClassesForFiles() instead of '
-    #               'MessageFactory.GetMessages(). MessageFactory class '
-    #               'will be removed after 2024.')
+    warnings.warn('MessageFactory class is deprecated. Please use '
+                  'GetMessageClassesForFiles() instead of '
+                  'MessageFactory.GetMessages(). MessageFactory class '
+                  'will be removed after 2024.')
     return GetMessageClassesForFiles(files, self.pool)
 
 
 def GetMessages(file_protos, pool=None):
   """Builds a dictionary of all the messages available in a set of files.
 
   Args:
```

### Comparing `protobuf-4.22.3/google/protobuf/proto_builder.py` & `protobuf-4.23.0rc2/google/protobuf/proto_builder.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/pyext/cpp_message.py` & `protobuf-4.23.0rc2/google/protobuf/pyext/cpp_message.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/reflection.py` & `protobuf-4.23.0rc2/google/protobuf/reflection.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/service.py` & `protobuf-4.23.0rc2/google/protobuf/service.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/service_reflection.py` & `protobuf-4.23.0rc2/google/protobuf/service_reflection.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/source_context_pb2.py` & `protobuf-4.23.0rc2/google/protobuf/source_context_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/source_context.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-4.22.3/google/protobuf/struct_pb2.py` & `protobuf-4.23.0rc2/google/protobuf/struct_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/struct.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-4.22.3/google/protobuf/symbol_database.py` & `protobuf-4.23.0rc2/google/protobuf/symbol_database.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/text_encoding.py` & `protobuf-4.23.0rc2/google/protobuf/text_encoding.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/text_format.py` & `protobuf-4.23.0rc2/google/protobuf/text_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -1250,23 +1250,18 @@
 
     Args:
       tokenizer: A tokenizer to parse the field name and values.
 
     Raises:
       ParseError: In case an invalid field value is found.
     """
-    # String/bytes tokens can come in multiple adjacent string literals.
-    # If we can consume one, consume as many as we can.
-    if tokenizer.TryConsumeByteString():
-      while tokenizer.TryConsumeByteString():
-        pass
-      return
-
-    if (not tokenizer.TryConsumeIdentifier() and
-        not _TryConsumeInt64(tokenizer) and not _TryConsumeUint64(tokenizer) and
+    if (not tokenizer.TryConsumeByteString()and
+        not tokenizer.TryConsumeIdentifier() and
+        not _TryConsumeInt64(tokenizer) and
+        not _TryConsumeUint64(tokenizer) and
         not tokenizer.TryConsumeFloat()):
       raise ParseError('Invalid field value: ' + tokenizer.token)
 
   def _SkipRepeatedFieldValue(self, tokenizer):
     """Skips over a repeated field value.
 
     Args:
```

### Comparing `protobuf-4.22.3/google/protobuf/timestamp_pb2.py` & `protobuf-4.23.0rc2/google/protobuf/timestamp_pb2.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/timestamp.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-4.22.3/google/protobuf/type_pb2.py` & `protobuf-4.23.0rc2/google/protobuf/type_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/type.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import source_context_pb2 as google_dot_protobuf_dot_source__context__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1agoogle/protobuf/type.proto\x12\x0fgoogle.protobuf\x1a\x19google/protobuf/any.proto\x1a$google/protobuf/source_context.proto\"\x8d\x02\n\x04Type\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12.\n\x06\x66ields\x18\x02 \x03(\x0b\x32\x16.google.protobuf.FieldR\x06\x66ields\x12\x16\n\x06oneofs\x18\x03 \x03(\tR\x06oneofs\x12\x31\n\x07options\x18\x04 \x03(\x0b\x32\x17.google.protobuf.OptionR\x07options\x12\x45\n\x0esource_context\x18\x05 \x01(\x0b\x32\x1e.google.protobuf.SourceContextR\rsourceContext\x12/\n\x06syntax\x18\x06 \x01(\x0e\x32\x17.google.protobuf.SyntaxR\x06syntax\"\xb4\x06\n\x05\x46ield\x12/\n\x04kind\x18\x01 \x01(\x0e\x32\x1b.google.protobuf.Field.KindR\x04kind\x12\x44\n\x0b\x63\x61rdinality\x18\x02 \x01(\x0e\x32\".google.protobuf.Field.CardinalityR\x0b\x63\x61rdinality\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12\x19\n\x08type_url\x18\x06 \x01(\tR\x07typeUrl\x12\x1f\n\x0boneof_index\x18\x07 \x01(\x05R\noneofIndex\x12\x16\n\x06packed\x18\x08 \x01(\x08R\x06packed\x12\x31\n\x07options\x18\t \x03(\x0b\x32\x17.google.protobuf.OptionR\x07options\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12#\n\rdefault_value\x18\x0b \x01(\tR\x0c\x64\x65\x66\x61ultValue\"\xc8\x02\n\x04Kind\x12\x10\n\x0cTYPE_UNKNOWN\x10\x00\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"t\n\x0b\x43\x61rdinality\x12\x17\n\x13\x43\x41RDINALITY_UNKNOWN\x10\x00\x12\x18\n\x14\x43\x41RDINALITY_OPTIONAL\x10\x01\x12\x18\n\x14\x43\x41RDINALITY_REQUIRED\x10\x02\x12\x18\n\x14\x43\x41RDINALITY_REPEATED\x10\x03\"\xff\x01\n\x04\x45num\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x38\n\tenumvalue\x18\x02 \x03(\x0b\x32\x1a.google.protobuf.EnumValueR\tenumvalue\x12\x31\n\x07options\x18\x03 \x03(\x0b\x32\x17.google.protobuf.OptionR\x07options\x12\x45\n\x0esource_context\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.SourceContextR\rsourceContext\x12/\n\x06syntax\x18\x05 \x01(\x0e\x32\x17.google.protobuf.SyntaxR\x06syntax\"j\n\tEnumValue\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12\x31\n\x07options\x18\x03 \x03(\x0b\x32\x17.google.protobuf.OptionR\x07options\"H\n\x06Option\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyR\x05value*.\n\x06Syntax\x12\x11\n\rSYNTAX_PROTO2\x10\x00\x12\x11\n\rSYNTAX_PROTO3\x10\x01\x42{\n\x13\x63om.google.protobufB\tTypeProtoP\x01Z-google.golang.org/protobuf/types/known/typepb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1eGoogle.Protobuf.WellKnownTypesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1agoogle/protobuf/type.proto\x12\x0fgoogle.protobuf\x1a\x19google/protobuf/any.proto\x1a$google/protobuf/source_context.proto\"\xa7\x02\n\x04Type\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12.\n\x06\x66ields\x18\x02 \x03(\x0b\x32\x16.google.protobuf.FieldR\x06\x66ields\x12\x16\n\x06oneofs\x18\x03 \x03(\tR\x06oneofs\x12\x31\n\x07options\x18\x04 \x03(\x0b\x32\x17.google.protobuf.OptionR\x07options\x12\x45\n\x0esource_context\x18\x05 \x01(\x0b\x32\x1e.google.protobuf.SourceContextR\rsourceContext\x12/\n\x06syntax\x18\x06 \x01(\x0e\x32\x17.google.protobuf.SyntaxR\x06syntax\x12\x18\n\x07\x65\x64ition\x18\x07 \x01(\tR\x07\x65\x64ition\"\xb4\x06\n\x05\x46ield\x12/\n\x04kind\x18\x01 \x01(\x0e\x32\x1b.google.protobuf.Field.KindR\x04kind\x12\x44\n\x0b\x63\x61rdinality\x18\x02 \x01(\x0e\x32\".google.protobuf.Field.CardinalityR\x0b\x63\x61rdinality\x12\x16\n\x06number\x18\x03 \x01(\x05R\x06number\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12\x19\n\x08type_url\x18\x06 \x01(\tR\x07typeUrl\x12\x1f\n\x0boneof_index\x18\x07 \x01(\x05R\noneofIndex\x12\x16\n\x06packed\x18\x08 \x01(\x08R\x06packed\x12\x31\n\x07options\x18\t \x03(\x0b\x32\x17.google.protobuf.OptionR\x07options\x12\x1b\n\tjson_name\x18\n \x01(\tR\x08jsonName\x12#\n\rdefault_value\x18\x0b \x01(\tR\x0c\x64\x65\x66\x61ultValue\"\xc8\x02\n\x04Kind\x12\x10\n\x0cTYPE_UNKNOWN\x10\x00\x12\x0f\n\x0bTYPE_DOUBLE\x10\x01\x12\x0e\n\nTYPE_FLOAT\x10\x02\x12\x0e\n\nTYPE_INT64\x10\x03\x12\x0f\n\x0bTYPE_UINT64\x10\x04\x12\x0e\n\nTYPE_INT32\x10\x05\x12\x10\n\x0cTYPE_FIXED64\x10\x06\x12\x10\n\x0cTYPE_FIXED32\x10\x07\x12\r\n\tTYPE_BOOL\x10\x08\x12\x0f\n\x0bTYPE_STRING\x10\t\x12\x0e\n\nTYPE_GROUP\x10\n\x12\x10\n\x0cTYPE_MESSAGE\x10\x0b\x12\x0e\n\nTYPE_BYTES\x10\x0c\x12\x0f\n\x0bTYPE_UINT32\x10\r\x12\r\n\tTYPE_ENUM\x10\x0e\x12\x11\n\rTYPE_SFIXED32\x10\x0f\x12\x11\n\rTYPE_SFIXED64\x10\x10\x12\x0f\n\x0bTYPE_SINT32\x10\x11\x12\x0f\n\x0bTYPE_SINT64\x10\x12\"t\n\x0b\x43\x61rdinality\x12\x17\n\x13\x43\x41RDINALITY_UNKNOWN\x10\x00\x12\x18\n\x14\x43\x41RDINALITY_OPTIONAL\x10\x01\x12\x18\n\x14\x43\x41RDINALITY_REQUIRED\x10\x02\x12\x18\n\x14\x43\x41RDINALITY_REPEATED\x10\x03\"\x99\x02\n\x04\x45num\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x38\n\tenumvalue\x18\x02 \x03(\x0b\x32\x1a.google.protobuf.EnumValueR\tenumvalue\x12\x31\n\x07options\x18\x03 \x03(\x0b\x32\x17.google.protobuf.OptionR\x07options\x12\x45\n\x0esource_context\x18\x04 \x01(\x0b\x32\x1e.google.protobuf.SourceContextR\rsourceContext\x12/\n\x06syntax\x18\x05 \x01(\x0e\x32\x17.google.protobuf.SyntaxR\x06syntax\x12\x18\n\x07\x65\x64ition\x18\x06 \x01(\tR\x07\x65\x64ition\"j\n\tEnumValue\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x16\n\x06number\x18\x02 \x01(\x05R\x06number\x12\x31\n\x07options\x18\x03 \x03(\x0b\x32\x17.google.protobuf.OptionR\x07options\"H\n\x06Option\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyR\x05value*C\n\x06Syntax\x12\x11\n\rSYNTAX_PROTO2\x10\x00\x12\x11\n\rSYNTAX_PROTO3\x10\x01\x12\x13\n\x0fSYNTAX_EDITIONS\x10\x02\x42{\n\x13\x63om.google.protobufB\tTypeProtoP\x01Z-google.golang.org/protobuf/types/known/typepb\xf8\x01\x01\xa2\x02\x03GPB\xaa\x02\x1eGoogle.Protobuf.WellKnownTypesb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.protobuf.type_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.google.protobufB\tTypeProtoP\001Z-google.golang.org/protobuf/types/known/typepb\370\001\001\242\002\003GPB\252\002\036Google.Protobuf.WellKnownTypes'
-  _globals['_SYNTAX']._serialized_start=1647
-  _globals['_SYNTAX']._serialized_end=1693
+  _globals['_SYNTAX']._serialized_start=1699
+  _globals['_SYNTAX']._serialized_end=1766
   _globals['_TYPE']._serialized_start=113
-  _globals['_TYPE']._serialized_end=382
-  _globals['_FIELD']._serialized_start=385
-  _globals['_FIELD']._serialized_end=1205
-  _globals['_FIELD_KIND']._serialized_start=759
-  _globals['_FIELD_KIND']._serialized_end=1087
-  _globals['_FIELD_CARDINALITY']._serialized_start=1089
-  _globals['_FIELD_CARDINALITY']._serialized_end=1205
-  _globals['_ENUM']._serialized_start=1208
-  _globals['_ENUM']._serialized_end=1463
-  _globals['_ENUMVALUE']._serialized_start=1465
-  _globals['_ENUMVALUE']._serialized_end=1571
-  _globals['_OPTION']._serialized_start=1573
-  _globals['_OPTION']._serialized_end=1645
+  _globals['_TYPE']._serialized_end=408
+  _globals['_FIELD']._serialized_start=411
+  _globals['_FIELD']._serialized_end=1231
+  _globals['_FIELD_KIND']._serialized_start=785
+  _globals['_FIELD_KIND']._serialized_end=1113
+  _globals['_FIELD_CARDINALITY']._serialized_start=1115
+  _globals['_FIELD_CARDINALITY']._serialized_end=1231
+  _globals['_ENUM']._serialized_start=1234
+  _globals['_ENUM']._serialized_end=1515
+  _globals['_ENUMVALUE']._serialized_start=1517
+  _globals['_ENUMVALUE']._serialized_end=1623
+  _globals['_OPTION']._serialized_start=1625
+  _globals['_OPTION']._serialized_end=1697
 # @@protoc_insertion_point(module_scope)
```

### Comparing `protobuf-4.22.3/google/protobuf/unknown_fields.py` & `protobuf-4.23.0rc2/google/protobuf/unknown_fields.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/google/protobuf/wrappers_pb2.py` & `protobuf-4.23.0rc2/google/protobuf/wrappers_pb2.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/protobuf/wrappers.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
```

### Comparing `protobuf-4.22.3/protobuf.egg-info/PKG-INFO` & `protobuf-4.23.0rc2/protobuf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: protobuf
-Version: 4.22.3
+Version: 4.23.0rc2
 Summary: Protocol Buffers
 Home-page: https://developers.google.com/protocol-buffers/
 Maintainer: protobuf@googlegroups.com
 Maintainer-email: protobuf@googlegroups.com
 License: BSD-3-Clause
 Download-URL: https://github.com/protocolbuffers/protobuf/releases
 Project-URL: Source, https://github.com/protocolbuffers/protobuf
```

### Comparing `protobuf-4.22.3/protobuf.egg-info/SOURCES.txt` & `protobuf-4.23.0rc2/protobuf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -134,18 +134,23 @@
 upb/mem/alloc.c
 upb/mem/alloc.h
 upb/mem/arena.c
 upb/mem/arena.h
 upb/mem/arena_internal.h
 upb/message/accessors.c
 upb/message/accessors.h
+upb/message/accessors_internal.h
+upb/message/copy.c
+upb/message/copy.h
 upb/message/extension_internal.h
 upb/message/internal.h
 upb/message/message.c
 upb/message/message.h
+upb/message/promote.c
+upb/message/promote.h
 upb/mini_table/common.c
 upb/mini_table/common.h
 upb/mini_table/common_internal.h
 upb/mini_table/decode.c
 upb/mini_table/decode.h
 upb/mini_table/encode.c
 upb/mini_table/encode_internal.h
@@ -154,14 +159,15 @@
 upb/mini_table/extension_registry.c
 upb/mini_table/extension_registry.h
 upb/mini_table/field_internal.h
 upb/mini_table/file_internal.h
 upb/mini_table/message_internal.h
 upb/mini_table/sub_internal.h
 upb/mini_table/types.h
+upb/port/atomic.h
 upb/port/def.inc
 upb/port/undef.inc
 upb/port/vsnprintf_compat.h
 upb/reflection/common.h
 upb/reflection/def.h
 upb/reflection/def_builder.c
 upb/reflection/def_builder_internal.h
@@ -212,14 +218,15 @@
 upb/text/encode.h
 upb/util/compare.c
 upb/util/compare.h
 upb/util/def_to_proto.c
 upb/util/def_to_proto.h
 upb/util/required_fields.c
 upb/util/required_fields.h
+upb/wire/common.h
 upb/wire/common_internal.h
 upb/wire/decode.c
 upb/wire/decode.h
 upb/wire/decode_fast.c
 upb/wire/decode_fast.h
 upb/wire/decode_internal.h
 upb/wire/encode.c
```

### Comparing `protobuf-4.22.3/python/convert.c` & `protobuf-4.23.0rc2/python/convert.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/convert.h` & `protobuf-4.23.0rc2/python/convert.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/descriptor.c` & `protobuf-4.23.0rc2/python/descriptor.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/descriptor.h` & `protobuf-4.23.0rc2/python/descriptor.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/descriptor_containers.c` & `protobuf-4.23.0rc2/python/descriptor_containers.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/descriptor_containers.h` & `protobuf-4.23.0rc2/python/descriptor_containers.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/descriptor_pool.c` & `protobuf-4.23.0rc2/python/descriptor_pool.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/descriptor_pool.h` & `protobuf-4.23.0rc2/python/descriptor_pool.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/extension_dict.c` & `protobuf-4.23.0rc2/python/extension_dict.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/extension_dict.h` & `protobuf-4.23.0rc2/python/extension_dict.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/map.c` & `protobuf-4.23.0rc2/python/map.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/map.h` & `protobuf-4.23.0rc2/python/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/message.c` & `protobuf-4.23.0rc2/python/message.c`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 #include "python/extension_dict.h"
 #include "python/map.h"
 #include "python/repeated.h"
 #include "upb/reflection/def.h"
 #include "upb/reflection/message.h"
 #include "upb/text/encode.h"
 #include "upb/util/required_fields.h"
+#include "upb/wire/common.h"
 
 static const upb_MessageDef* PyUpb_MessageMeta_GetMsgdef(PyObject* cls);
 static PyObject* PyUpb_MessageMeta_GetAttr(PyObject* self, PyObject* name);
 
 // -----------------------------------------------------------------------------
 // CPythonBits
 // -----------------------------------------------------------------------------
@@ -443,24 +444,26 @@
 
 err:
   Py_XDECREF(repeated);
   Py_XDECREF(tmp);
   return ok;
 }
 
+static PyObject* PyUpb_Message_MergePartialFrom(PyObject*, PyObject*);
+
 static bool PyUpb_Message_InitMessageAttribute(PyObject* _self, PyObject* name,
                                                PyObject* value) {
   PyObject* submsg = PyUpb_Message_GetAttr(_self, name);
   if (!submsg) return -1;
   assert(!PyErr_Occurred());
   bool ok;
   if (PyUpb_Message_TryCheck(value)) {
-    PyObject* tmp = PyUpb_Message_MergeFrom(submsg, value);
+    PyObject* tmp = PyUpb_Message_MergePartialFrom(submsg, value);
     ok = tmp != NULL;
-    Py_DECREF(tmp);
+    Py_XDECREF(tmp);
   } else if (PyDict_Check(value)) {
     assert(!PyErr_Occurred());
     ok = PyUpb_Message_InitAttributes(submsg, NULL, value) >= 0;
   } else {
     const upb_MessageDef* m = PyUpb_Message_GetMsgdef(_self);
     PyErr_Format(PyExc_TypeError, "Message must be initialized with a dict: %s",
                  upb_MessageDef_FullName(m));
@@ -1180,33 +1183,45 @@
   Py_XDECREF(field_desc);
   Py_XDECREF(py_val);
   Py_XDECREF(tuple);
   Py_DECREF(list);
   return NULL;
 }
 
-PyObject* PyUpb_Message_MergeFrom(PyObject* self, PyObject* arg) {
+static PyObject* PyUpb_Message_MergeInternal(PyObject* self, PyObject* arg,
+                                             bool check_required) {
   if (self->ob_type != arg->ob_type) {
     PyErr_Format(PyExc_TypeError,
                  "Parameter to MergeFrom() must be instance of same class: "
                  "expected %S got %S.",
                  Py_TYPE(self), Py_TYPE(arg));
     return NULL;
   }
   // OPT: exit if src is empty.
   PyObject* subargs = PyTuple_New(0);
-  PyObject* serialized = PyUpb_Message_SerializeToString(arg, subargs, NULL);
+  PyObject* serialized =
+      check_required
+          ? PyUpb_Message_SerializeToString(arg, subargs, NULL)
+          : PyUpb_Message_SerializePartialToString(arg, subargs, NULL);
   Py_DECREF(subargs);
   if (!serialized) return NULL;
   PyObject* ret = PyUpb_Message_MergeFromString(self, serialized);
   Py_DECREF(serialized);
   Py_DECREF(ret);
   Py_RETURN_NONE;
 }
 
+PyObject* PyUpb_Message_MergeFrom(PyObject* self, PyObject* arg) {
+  return PyUpb_Message_MergeInternal(self, arg, true);
+}
+
+static PyObject* PyUpb_Message_MergePartialFrom(PyObject* self, PyObject* arg) {
+  return PyUpb_Message_MergeInternal(self, arg, false);
+}
+
 static PyObject* PyUpb_Message_SetInParent(PyObject* _self, PyObject* arg) {
   PyUpb_Message* self = (void*)_self;
   PyUpb_Message_EnsureReified(self);
   Py_RETURN_NONE;
 }
 
 static PyObject* PyUpb_Message_UnknownFields(PyObject* _self, PyObject* arg) {
@@ -1236,16 +1251,17 @@
   const upb_MessageDef* msgdef = _PyUpb_Message_GetMsgdef(self);
   const upb_FileDef* file = upb_MessageDef_File(msgdef);
   const upb_ExtensionRegistry* extreg =
       upb_DefPool_ExtensionRegistry(upb_FileDef_Pool(file));
   const upb_MiniTable* layout = upb_MessageDef_MiniTable(msgdef);
   upb_Arena* arena = PyUpb_Arena_Get(self->arena);
   PyUpb_ModuleState* state = PyUpb_ModuleState_Get();
-  int options =
-      UPB_DECODE_MAXDEPTH(state->allow_oversize_protos ? UINT32_MAX : 100);
+  int options = upb_DecodeOptions_MaxDepth(
+      state->allow_oversize_protos ? UINT16_MAX
+                                   : kUpb_WireFormat_DefaultDepthLimit);
   upb_DecodeStatus status =
       upb_Decode(buf, size, self->ptr.msg, layout, extreg, options, arena);
   Py_XDECREF(bytes);
   if (status != kUpb_DecodeStatus_Ok) {
     PyErr_Format(state->decode_error_class, "Error parsing message");
     return NULL;
   }
@@ -1508,15 +1524,15 @@
     return NULL;
   }
 
   upb_Arena* arena = upb_Arena_New();
   const upb_MiniTable* layout = upb_MessageDef_MiniTable(msgdef);
   size_t size = 0;
   // Python does not currently have any effective limit on serialization depth.
-  int options = UPB_ENCODE_MAXDEPTH(UINT32_MAX);
+  int options = upb_EncodeOptions_MaxDepth(UINT16_MAX);
   if (check_required) options |= kUpb_EncodeOption_CheckRequired;
   if (deterministic) options |= kUpb_EncodeOption_Deterministic;
   char* pb;
   upb_EncodeStatus status =
       upb_Encode(self->ptr.msg, layout, options, arena, &pb, &size);
   PyObject* ret = NULL;
```

### Comparing `protobuf-4.22.3/python/message.h` & `protobuf-4.23.0rc2/python/message.h`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 const upb_MessageDef* PyUpb_Message_GetMsgdef(PyObject* self);
 
 // Functions that match the corresponding methods on the message object.
 PyObject* PyUpb_Message_MergeFrom(PyObject* self, PyObject* arg);
 PyObject* PyUpb_Message_MergeFromString(PyObject* self, PyObject* arg);
 PyObject* PyUpb_Message_SerializeToString(PyObject* self, PyObject* args,
                                           PyObject* kwargs);
+PyObject* PyUpb_Message_SerializePartialToString(PyObject* self, PyObject* args,
+                                                 PyObject* kwargs);
 
 // Sets fields of the message according to the attribuges in `kwargs`.
 int PyUpb_Message_InitAttributes(PyObject* _self, PyObject* args,
                                  PyObject* kwargs);
 
 // Checks that `key` is a field descriptor for an extension type, and that the
 // extendee is this message.  Otherwise returns NULL and sets a KeyError.
```

### Comparing `protobuf-4.22.3/python/protobuf.c` & `protobuf-4.23.0rc2/python/protobuf.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/protobuf.h` & `protobuf-4.23.0rc2/python/protobuf.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/python_api.h` & `protobuf-4.23.0rc2/python/python_api.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/repeated.c` & `protobuf-4.23.0rc2/python/repeated.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/repeated.h` & `protobuf-4.23.0rc2/python/repeated.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/unknown_fields.c` & `protobuf-4.23.0rc2/python/unknown_fields.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/python/unknown_fields.h` & `protobuf-4.23.0rc2/python/unknown_fields.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/setup.py` & `protobuf-4.23.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/alloc.h` & `protobuf-4.23.0rc2/upb/alloc.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/arena.h` & `protobuf-4.23.0rc2/upb/arena.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/array.h` & `protobuf-4.23.0rc2/upb/array.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/base/descriptor_constants.h` & `protobuf-4.23.0rc2/upb/base/descriptor_constants.h`

 * *Files 14% similar despite different names*

```diff
@@ -24,24 +24,27 @@
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef UPB_BASE_DESCRIPTOR_CONSTANTS_H_
 #define UPB_BASE_DESCRIPTOR_CONSTANTS_H_
 
+// Must be last.
+#include "upb/port/def.inc"
+
 // The types a field can have. Note that this list is not identical to the
 // types defined in descriptor.proto, which gives INT32 and SINT32 separate
 // types (we distinguish the two with the "integer encoding" enum below).
 // This enum is an internal convenience only and has no meaning outside of upb.
 typedef enum {
   kUpb_CType_Bool = 1,
   kUpb_CType_Float = 2,
   kUpb_CType_Int32 = 3,
   kUpb_CType_UInt32 = 4,
-  kUpb_CType_Enum = 5,  // Enum values are int32.
+  kUpb_CType_Enum = 5,  // Enum values are int32. TODO(b/279178239): rename
   kUpb_CType_Message = 6,
   kUpb_CType_Double = 7,
   kUpb_CType_Int64 = 8,
   kUpb_CType_UInt64 = 9,
   kUpb_CType_String = 10,
   kUpb_CType_Bytes = 11
 } upb_CType;
@@ -73,8 +76,29 @@
   kUpb_FieldType_SFixed64 = 16,
   kUpb_FieldType_SInt32 = 17,
   kUpb_FieldType_SInt64 = 18,
 } upb_FieldType;
 
 #define kUpb_FieldType_SizeOf 19
 
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+UPB_INLINE bool upb_FieldType_IsPackable(upb_FieldType type) {
+  // clang-format off
+  const unsigned kUnpackableTypes =
+      (1 << kUpb_FieldType_String) |
+      (1 << kUpb_FieldType_Bytes) |
+      (1 << kUpb_FieldType_Message) |
+      (1 << kUpb_FieldType_Group);
+  // clang-format on
+  return (1 << type) & ~kUnpackableTypes;
+}
+
+#ifdef __cplusplus
+} /* extern "C" */
+#endif
+
+#include "upb/port/undef.inc"
+
 #endif /* UPB_BASE_DESCRIPTOR_CONSTANTS_H_ */
```

### Comparing `protobuf-4.22.3/upb/base/log2.h` & `protobuf-4.23.0rc2/upb/base/log2.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/base/status.c` & `protobuf-4.23.0rc2/upb/base/status.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/base/status.h` & `protobuf-4.23.0rc2/upb/base/status.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/base/string_view.h` & `protobuf-4.23.0rc2/upb/base/string_view.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/collections/array.c` & `protobuf-4.23.0rc2/upb/collections/array.c`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
   char* data = _upb_array_ptr(arr);
   int lg2 = arr->data & 7;
   UPB_ASSERT(i < arr->size);
   memcpy(data + (i << lg2), &val, 1 << lg2);
 }
 
 bool upb_Array_Append(upb_Array* arr, upb_MessageValue val, upb_Arena* arena) {
+  UPB_ASSERT(arena);
   if (!upb_Array_Resize(arr, arr->size + 1, arena)) {
     return false;
   }
   upb_Array_Set(arr, arr->size - 1, val);
   return true;
 }
 
@@ -81,14 +82,15 @@
   const int lg2 = arr->data & 7;
   char* data = _upb_array_ptr(arr);
   memmove(&data[dst_idx << lg2], &data[src_idx << lg2], count << lg2);
 }
 
 bool upb_Array_Insert(upb_Array* arr, size_t i, size_t count,
                       upb_Arena* arena) {
+  UPB_ASSERT(arena);
   UPB_ASSERT(i <= arr->size);
   UPB_ASSERT(count + arr->size >= count);
   const size_t oldsize = arr->size;
   if (!upb_Array_Resize(arr, arr->size + count, arena)) {
     return false;
   }
   upb_Array_Move(arr, i + count, i, oldsize - i);
```

### Comparing `protobuf-4.22.3/upb/collections/array.h` & `protobuf-4.23.0rc2/upb/collections/array.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/collections/array_internal.h` & `protobuf-4.23.0rc2/upb/collections/array_internal.h`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,15 @@
   if (arr->capacity < size) return _upb_array_realloc(arr, size, arena);
   return true;
 }
 
 // Resize without initializing new elements.
 UPB_INLINE bool _upb_Array_ResizeUninitialized(upb_Array* arr, size_t size,
                                                upb_Arena* arena) {
+  UPB_ASSERT(size <= arr->size || arena);  // Allow NULL arena when shrinking.
   if (!_upb_array_reserve(arr, size, arena)) return false;
   arr->size = size;
   return true;
 }
 
 // This function is intended for situations where elem_size is compile-time
 // constant or a known expression of the form (1 << lg2), so that the expression
```

### Comparing `protobuf-4.22.3/upb/collections/map.c` & `protobuf-4.23.0rc2/upb/collections/map.c`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,15 @@
   return _upb_Map_Get(map, &key, map->key_size, val, map->val_size);
 }
 
 void upb_Map_Clear(upb_Map* map) { _upb_Map_Clear(map); }
 
 upb_MapInsertStatus upb_Map_Insert(upb_Map* map, upb_MessageValue key,
                                    upb_MessageValue val, upb_Arena* arena) {
+  UPB_ASSERT(arena);
   return (upb_MapInsertStatus)_upb_Map_Insert(map, &key, map->key_size, &val,
                                               map->val_size, arena);
 }
 
 bool upb_Map_Delete(upb_Map* map, upb_MessageValue key, upb_MessageValue* val) {
   upb_value v;
   const bool ok = _upb_Map_Delete(map, &key, map->key_size, &v);
```

### Comparing `protobuf-4.22.3/upb/collections/map.h` & `protobuf-4.23.0rc2/upb/collections/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/collections/map_gencode_util.h` & `protobuf-4.23.0rc2/upb/collections/map_gencode_util.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/collections/map_internal.h` & `protobuf-4.23.0rc2/upb/collections/map_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/collections/map_sorter.c` & `protobuf-4.23.0rc2/upb/collections/map_sorter.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/collections/map_sorter_internal.h` & `protobuf-4.23.0rc2/upb/collections/map_sorter_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/collections/message_value.h` & `protobuf-4.23.0rc2/upb/collections/message_value.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/collections.h` & `protobuf-4.23.0rc2/upb/collections.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/decode.h` & `protobuf-4.23.0rc2/upb/decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/decode_fast.h` & `protobuf-4.23.0rc2/upb/decode_fast.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/def.h` & `protobuf-4.23.0rc2/upb/def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/encode.h` & `protobuf-4.23.0rc2/upb/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/extension_registry.h` & `protobuf-4.23.0rc2/upb/extension_registry.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/hash/common.c` & `protobuf-4.23.0rc2/upb/hash/common.c`

 * *Files 0% similar despite different names*

```diff
@@ -772,15 +772,15 @@
 
 // Iteration.
 
 bool upb_inttable_next(const upb_inttable* t, uintptr_t* key, upb_value* val,
                        intptr_t* iter) {
   intptr_t i = *iter;
   if ((size_t)(i + 1) <= t->array_size) {
-    while (++i < t->array_size) {
+    while ((size_t)++i < t->array_size) {
       upb_tabval ent = t->array[i];
       if (upb_arrhas(ent)) {
         *key = i;
         *val = _upb_value_val(ent.val);
         *iter = i;
         return true;
       }
@@ -798,15 +798,15 @@
   }
 
   return false;
 }
 
 void upb_inttable_removeiter(upb_inttable* t, intptr_t* iter) {
   intptr_t i = *iter;
-  if (i < t->array_size) {
+  if ((size_t)i < t->array_size) {
     t->array_count--;
     mutable_array(t)[i].val = -1;
   } else {
     upb_tabent* ent = &t->t.entries[i - t->array_size];
     upb_tabent* prev = NULL;
 
     // Linear search, not great.
```

### Comparing `protobuf-4.22.3/upb/hash/common.h` & `protobuf-4.23.0rc2/upb/hash/common.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/hash/int_table.h` & `protobuf-4.23.0rc2/upb/hash/int_table.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/hash/str_table.h` & `protobuf-4.23.0rc2/upb/hash/str_table.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/json/decode.c` & `protobuf-4.23.0rc2/upb/json/decode.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/json/decode.h` & `protobuf-4.23.0rc2/upb/json/decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/json/encode.c` & `protobuf-4.23.0rc2/upb/json/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/json/encode.h` & `protobuf-4.23.0rc2/upb/json/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/json_decode.h` & `protobuf-4.23.0rc2/upb/json_decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/json_encode.h` & `protobuf-4.23.0rc2/upb/json_encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/lex/atoi.c` & `protobuf-4.23.0rc2/upb/lex/atoi.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/lex/atoi.h` & `protobuf-4.23.0rc2/upb/lex/atoi.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/lex/round_trip.c` & `protobuf-4.23.0rc2/upb/lex/round_trip.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/lex/round_trip.h` & `protobuf-4.23.0rc2/upb/lex/round_trip.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/lex/strtod.c` & `protobuf-4.23.0rc2/upb/lex/strtod.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/lex/strtod.h` & `protobuf-4.23.0rc2/upb/lex/strtod.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/lex/unicode.c` & `protobuf-4.23.0rc2/upb/lex/unicode.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/lex/unicode.h` & `protobuf-4.23.0rc2/upb/lex/unicode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/map.h` & `protobuf-4.23.0rc2/upb/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/mem/alloc.c` & `protobuf-4.23.0rc2/upb/mem/alloc.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/mem/alloc.h` & `protobuf-4.23.0rc2/upb/mem/alloc.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/mem/arena.h` & `protobuf-4.23.0rc2/upb/mem/arena.h`

 * *Files 5% similar despite different names*

```diff
@@ -45,32 +45,32 @@
 #include "upb/mem/alloc.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
 typedef struct upb_Arena upb_Arena;
 
-typedef void upb_CleanupFunc(void* context);
+// LINT.IfChange(arena_head)
 
 typedef struct {
   char *ptr, *end;
 } _upb_ArenaHead;
 
+// LINT.ThenChange(//depot/google3/third_party/upb/js/impl/upb_bits/arena.ts:arena_head)
+
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // Creates an arena from the given initial block (if any -- n may be 0).
 // Additional blocks will be allocated from |alloc|.  If |alloc| is NULL, this
 // is a fixed-size arena and cannot grow.
 UPB_API upb_Arena* upb_Arena_Init(void* mem, size_t n, upb_alloc* alloc);
 
 UPB_API void upb_Arena_Free(upb_Arena* a);
-UPB_API bool upb_Arena_AddCleanup(upb_Arena* a, void* ud,
-                                  upb_CleanupFunc* func);
 UPB_API bool upb_Arena_Fuse(upb_Arena* a, upb_Arena* b);
 
 void* _upb_Arena_SlowMalloc(upb_Arena* a, size_t size);
 size_t upb_Arena_SpaceAllocated(upb_Arena* arena);
 uint32_t upb_Arena_DebugRefCount(upb_Arena* arena);
 
 UPB_INLINE size_t _upb_ArenaHas(upb_Arena* a) {
```

### Comparing `protobuf-4.22.3/upb/mem/arena_internal.h` & `protobuf-4.23.0rc2/upb/mini_table/file_internal.h`

 * *Files 18% similar despite different names*

```diff
@@ -21,50 +21,27 @@
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#ifndef UPB_MEM_ARENA_INTERNAL_H_
-#define UPB_MEM_ARENA_INTERNAL_H_
+#ifndef UPB_MINI_TABLE_FILE_INTERNAL_H_
+#define UPB_MINI_TABLE_FILE_INTERNAL_H_
 
-#include "upb/mem/arena.h"
+#include "upb/mini_table/types.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
-typedef struct _upb_MemBlock _upb_MemBlock;
-
-struct upb_Arena {
-  _upb_ArenaHead head;
-  /* Stores cleanup metadata for this arena.
-   * - a pointer to the current cleanup counter.
-   * - a boolean indicating if there is an unowned initial block.  */
-  uintptr_t cleanup_metadata;
-
-  /* Allocator to allocate arena blocks.  We are responsible for freeing these
-   * when we are destroyed. */
-  upb_alloc* block_alloc;
-  uint32_t last_size;
-
-  /* When multiple arenas are fused together, each arena points to a parent
-   * arena (root points to itself). The root tracks how many live arenas
-   * reference it. */
-  uint32_t refcount; /* Only used when a->parent == a */
-  struct upb_Arena* parent;
-
-  /* Linked list of blocks to free/cleanup. */
-  _upb_MemBlock *freelist, *freelist_tail;
+struct upb_MiniTableFile {
+  const upb_MiniTable** msgs;
+  const upb_MiniTableEnum** enums;
+  const upb_MiniTableExtension** exts;
+  int msg_count;
+  int enum_count;
+  int ext_count;
 };
 
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-#ifdef __cplusplus
-} /* extern "C" */
-#endif
-
 #include "upb/port/undef.inc"
 
-#endif /* UPB_MEM_ARENA_INTERNAL_H_ */
+#endif /* UPB_MINI_TABLE_FILE_INTERNAL_H_ */
```

### Comparing `protobuf-4.22.3/upb/message/accessors.c` & `protobuf-4.23.0rc2/upb/message/promote.c`

 * *Files 6% similar despite different names*

```diff
@@ -21,21 +21,23 @@
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#include "upb/message/accessors.h"
+#include "upb/message/promote.h"
 
 #include "upb/collections/array.h"
 #include "upb/collections/array_internal.h"
 #include "upb/collections/map.h"
+#include "upb/message/accessors.h"
 #include "upb/message/message.h"
 #include "upb/mini_table/field_internal.h"
+#include "upb/wire/common.h"
 #include "upb/wire/decode.h"
 #include "upb/wire/encode.h"
 #include "upb/wire/eps_copy_input_stream.h"
 #include "upb/wire/reader.h"
 
 // Must be last.
 #include "upb/port/def.inc"
@@ -71,23 +73,24 @@
   return ret;
 }
 
 upb_GetExtension_Status upb_MiniTable_GetOrPromoteExtension(
     upb_Message* msg, const upb_MiniTableExtension* ext_table,
     int decode_options, upb_Arena* arena,
     const upb_Message_Extension** extension) {
-  UPB_ASSERT(ext_table->field.descriptortype == kUpb_FieldType_Message);
+  UPB_ASSERT(upb_MiniTableField_CType(&ext_table->field) == kUpb_CType_Message);
   *extension = _upb_Message_Getext(msg, ext_table);
   if (*extension) {
     return kUpb_GetExtension_Ok;
   }
 
   // Check unknown fields, if available promote.
   int field_number = ext_table->field.number;
-  upb_FindUnknownRet result = upb_MiniTable_FindUnknown(msg, field_number);
+  upb_FindUnknownRet result = upb_MiniTable_FindUnknown(
+      msg, field_number, kUpb_WireFormat_DefaultDepthLimit);
   if (result.status != kUpb_FindUnknown_Ok) {
     return kUpb_GetExtension_NotPresent;
   }
   size_t len;
   size_t ofs = result.ptr - upb_Message_GetUnknown(msg, &len);
   // Decode and promote from unknown.
   const upb_MiniTable* extension_table = ext_table->sub.submsg;
@@ -119,26 +122,27 @@
 }
 
 upb_GetExtensionAsBytes_Status upb_MiniTable_GetExtensionAsBytes(
     const upb_Message* msg, const upb_MiniTableExtension* ext_table,
     int encode_options, upb_Arena* arena, const char** extension_data,
     size_t* len) {
   const upb_Message_Extension* msg_ext = _upb_Message_Getext(msg, ext_table);
-  UPB_ASSERT(ext_table->field.descriptortype == kUpb_FieldType_Message);
+  UPB_ASSERT(upb_MiniTableField_CType(&ext_table->field) == kUpb_CType_Message);
   if (msg_ext) {
     upb_EncodeStatus status =
         upb_Encode(msg_ext->data.ptr, msg_ext->ext->sub.submsg, encode_options,
                    arena, (char**)extension_data, len);
     if (status != kUpb_EncodeStatus_Ok) {
       return kUpb_GetExtensionAsBytes_EncodeError;
     }
     return kUpb_GetExtensionAsBytes_Ok;
   }
   int field_number = ext_table->field.number;
-  upb_FindUnknownRet result = upb_MiniTable_FindUnknown(msg, field_number);
+  upb_FindUnknownRet result = upb_MiniTable_FindUnknown(
+      msg, field_number, upb_DecodeOptions_GetMaxDepth(encode_options));
   if (result.status != kUpb_FindUnknown_Ok) {
     return kUpb_GetExtensionAsBytes_NotPresent;
   }
   const char* data = result.ptr;
   uint32_t tag;
   uint64_t message_len = 0;
   data = upb_WireReader_ReadTag(data, &tag);
@@ -149,16 +153,16 @@
 }
 
 static upb_FindUnknownRet upb_FindUnknownRet_ParseError(void) {
   return (upb_FindUnknownRet){.status = kUpb_FindUnknown_ParseError};
 }
 
 upb_FindUnknownRet upb_MiniTable_FindUnknown(const upb_Message* msg,
-                                             uint32_t field_number) {
-  const int depth_limit = 100;  // TODO: this should be a parameter
+                                             uint32_t field_number,
+                                             int depth_limit) {
   size_t size;
   upb_FindUnknownRet ret;
 
   const char* ptr = upb_Message_GetUnknown(msg, &size);
   upb_EpsCopyInputStream stream;
   upb_EpsCopyInputStream_Init(&stream, &ptr, size, true);
 
@@ -192,23 +196,25 @@
     const upb_MiniTableField* field, const upb_MiniTable* sub_mini_table,
     int decode_options, upb_Arena* arena) {
   upb_FindUnknownRet unknown;
   // We need to loop and merge unknowns that have matching tag field->number.
   upb_Message* message = NULL;
   // Callers should check that message is not set first before calling
   // PromotoUnknownToMessage.
-  UPB_ASSERT(mini_table->subs[field->submsg_index].submsg == sub_mini_table);
+  UPB_ASSERT(upb_MiniTable_GetSubMessageTable(mini_table, field) ==
+             sub_mini_table);
   bool is_oneof = _upb_MiniTableField_InOneOf(field);
   if (!is_oneof || _upb_getoneofcase_field(msg, field) == field->number) {
     UPB_ASSERT(upb_Message_GetMessage(msg, field, NULL) == NULL);
   }
   upb_UnknownToMessageRet ret;
   ret.status = kUpb_UnknownToMessage_Ok;
   do {
-    unknown = upb_MiniTable_FindUnknown(msg, field->number);
+    unknown = upb_MiniTable_FindUnknown(
+        msg, field->number, upb_DecodeOptions_GetMaxDepth(decode_options));
     switch (unknown.status) {
       case kUpb_FindUnknown_Ok: {
         const char* unknown_data = unknown.ptr;
         size_t unknown_size = unknown.len;
         ret = upb_MiniTable_ParseUnknownMessage(unknown_data, unknown_size,
                                                 sub_mini_table, message,
                                                 decode_options, arena);
@@ -246,15 +252,16 @@
 upb_UnknownToMessage_Status upb_MiniTable_PromoteUnknownToMessageArray(
     upb_Message* msg, const upb_MiniTableField* field,
     const upb_MiniTable* mini_table, int decode_options, upb_Arena* arena) {
   upb_Array* repeated_messages = upb_Message_GetMutableArray(msg, field);
   // Find all unknowns with given field number and parse.
   upb_FindUnknownRet unknown;
   do {
-    unknown = upb_MiniTable_FindUnknown(msg, field->number);
+    unknown = upb_MiniTable_FindUnknown(
+        msg, field->number, upb_DecodeOptions_GetMaxDepth(decode_options));
     if (unknown.status == kUpb_FindUnknown_Ok) {
       upb_UnknownToMessageRet ret = upb_MiniTable_ParseUnknownMessage(
           unknown.ptr, unknown.len, mini_table,
           /* base_message= */ NULL, decode_options, arena);
       if (ret.status == kUpb_UnknownToMessage_Ok) {
         upb_MessageValue value;
         value.msg_val = ret.message;
@@ -271,54 +278,29 @@
         return ret.status;
       }
     }
   } while (unknown.status == kUpb_FindUnknown_Ok);
   return kUpb_UnknownToMessage_Ok;
 }
 
-upb_MapInsertStatus upb_Message_InsertMapEntry(upb_Map* map,
-                                               const upb_MiniTable* mini_table,
-                                               const upb_MiniTableField* field,
-                                               upb_Message* map_entry_message,
-                                               upb_Arena* arena) {
-  const upb_MiniTable* map_entry_mini_table =
-      mini_table->subs[field->submsg_index].submsg;
-  UPB_ASSERT(map_entry_mini_table);
-  UPB_ASSERT(map_entry_mini_table->field_count == 2);
-  const upb_MiniTableField* map_entry_key_field =
-      &map_entry_mini_table->fields[0];
-  const upb_MiniTableField* map_entry_value_field =
-      &map_entry_mini_table->fields[1];
-  // Map key/value cannot have explicit defaults,
-  // hence assuming a zero default is valid.
-  upb_MessageValue default_val;
-  memset(&default_val, 0, sizeof(upb_MessageValue));
-  upb_MessageValue map_entry_key;
-  upb_MessageValue map_entry_value;
-  _upb_Message_GetField(map_entry_message, map_entry_key_field, &default_val,
-                        &map_entry_key);
-  _upb_Message_GetField(map_entry_message, map_entry_value_field, &default_val,
-                        &map_entry_value);
-  return upb_Map_Insert(map, map_entry_key, map_entry_value, arena);
-}
-
 // Moves repeated messages in unknowns to a upb_Map.
 upb_UnknownToMessage_Status upb_MiniTable_PromoteUnknownToMap(
     upb_Message* msg, const upb_MiniTable* mini_table,
     const upb_MiniTableField* field, int decode_options, upb_Arena* arena) {
   const upb_MiniTable* map_entry_mini_table =
-      mini_table->subs[field->submsg_index].submsg;
+      mini_table->subs[field->UPB_PRIVATE(submsg_index)].submsg;
   UPB_ASSERT(map_entry_mini_table);
   UPB_ASSERT(map_entry_mini_table);
   UPB_ASSERT(map_entry_mini_table->field_count == 2);
   UPB_ASSERT(upb_FieldMode_Get(field) == kUpb_FieldMode_Map);
   // Find all unknowns with given field number and parse.
   upb_FindUnknownRet unknown;
   while (1) {
-    unknown = upb_MiniTable_FindUnknown(msg, field->number);
+    unknown = upb_MiniTable_FindUnknown(
+        msg, field->number, upb_DecodeOptions_GetMaxDepth(decode_options));
     if (unknown.status != kUpb_FindUnknown_Ok) break;
     upb_UnknownToMessageRet ret = upb_MiniTable_ParseUnknownMessage(
         unknown.ptr, unknown.len, map_entry_mini_table,
         /* base_message= */ NULL, decode_options, arena);
     if (ret.status != kUpb_UnknownToMessage_Ok) return ret.status;
     // Allocate map on demand before append.
     upb_Map* map = upb_Message_GetOrCreateMutableMap(msg, map_entry_mini_table,
```

### Comparing `protobuf-4.22.3/upb/message/accessors.h` & `protobuf-4.23.0rc2/upb/reflection/field_def.c`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright (c) 2009-2022, Google LLC
+ * Copyright (c) 2009-2021, Google LLC
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
  *     * Redistributions of source code must retain the above copyright
  *       notice, this list of conditions and the following disclaimer.
  *     * Redistributions in binary form must reproduce the above copyright
@@ -21,741 +21,910 @@
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#ifndef UPB_MESSAGE_ACCESSORS_H_
-#define UPB_MESSAGE_ACCESSORS_H_
+#include <ctype.h>
+#include <errno.h>
 
-#include "upb/base/descriptor_constants.h"
-#include "upb/collections/array.h"
-#include "upb/collections/array_internal.h"
-#include "upb/collections/map.h"
-#include "upb/collections/map_internal.h"
-#include "upb/message/extension_internal.h"
-#include "upb/message/internal.h"
-#include "upb/mini_table/common.h"
-#include "upb/mini_table/enum_internal.h"
-#include "upb/mini_table/field_internal.h"
+#include "upb/mini_table/decode.h"
+#include "upb/reflection/def.h"
+#include "upb/reflection/def_builder_internal.h"
+#include "upb/reflection/def_pool.h"
+#include "upb/reflection/def_type.h"
+#include "upb/reflection/desc_state_internal.h"
+#include "upb/reflection/enum_def_internal.h"
+#include "upb/reflection/enum_value_def_internal.h"
+#include "upb/reflection/field_def_internal.h"
+#include "upb/reflection/file_def_internal.h"
+#include "upb/reflection/message_def_internal.h"
+#include "upb/reflection/oneof_def_internal.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
-#if defined(__GNUC__) && !defined(__clang__)
-// GCC raises incorrect warnings in these functions.  It thinks that we are
-// overrunning buffers, but we carefully write the functions in this file to
-// guarantee that this is impossible.  GCC gets this wrong due it its failure
-// to perform constant propagation as we expect:
-//   - https://gcc.gnu.org/bugzilla/show_bug.cgi?id=108217
-//   - https://gcc.gnu.org/bugzilla/show_bug.cgi?id=108226
-//
-// Unfortunately this also indicates that GCC is not optimizing away the
-// switch() in cases where it should be, compromising the performance.
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Warray-bounds"
-#pragma GCC diagnostic ignored "-Wstringop-overflow"
-#if __GNUC__ >= 11
-#pragma GCC diagnostic ignored "-Wstringop-overread"
-#endif
-#endif
+#define UPB_FIELD_TYPE_UNSPECIFIED 0
+
+typedef struct {
+  size_t len;
+  char str[1];  // Null-terminated string data follows.
+} str_t;
 
-#ifdef __cplusplus
-extern "C" {
+struct upb_FieldDef {
+  const UPB_DESC(FieldOptions) * opts;
+  const upb_FileDef* file;
+  const upb_MessageDef* msgdef;
+  const char* full_name;
+  const char* json_name;
+  union {
+    int64_t sint;
+    uint64_t uint;
+    double dbl;
+    float flt;
+    bool boolean;
+    str_t* str;
+    void* msg;  // Always NULL.
+  } defaultval;
+  union {
+    const upb_OneofDef* oneof;
+    const upb_MessageDef* extension_scope;
+  } scope;
+  union {
+    const upb_MessageDef* msgdef;
+    const upb_EnumDef* enumdef;
+    const UPB_DESC(FieldDescriptorProto) * unresolved;
+  } sub;
+  uint32_t number_;
+  uint16_t index_;
+  uint16_t layout_index;  // Index into msgdef->layout->fields or file->exts
+  bool has_default;
+  bool has_json_name;
+  bool has_presence;
+  bool is_extension;
+  bool is_packed;
+  bool is_proto3_optional;
+  upb_FieldType type_;
+  upb_Label label_;
+#if UINTPTR_MAX == 0xffffffff
+  uint32_t padding;  // Increase size to a multiple of 8.
 #endif
+};
 
-UPB_INLINE bool _upb_MiniTableField_InOneOf(const upb_MiniTableField* field) {
-  return field->presence < 0;
+upb_FieldDef* _upb_FieldDef_At(const upb_FieldDef* f, int i) {
+  return (upb_FieldDef*)&f[i];
 }
 
-UPB_INLINE void* _upb_MiniTableField_GetPtr(upb_Message* msg,
-                                            const upb_MiniTableField* field) {
-  return (char*)msg + field->offset;
-}
-
-UPB_INLINE const void* _upb_MiniTableField_GetConstPtr(
-    const upb_Message* msg, const upb_MiniTableField* field) {
-  return (char*)msg + field->offset;
-}
-
-UPB_INLINE void _upb_Message_SetPresence(upb_Message* msg,
-                                         const upb_MiniTableField* field) {
-  if (field->presence > 0) {
-    _upb_sethas_field(msg, field);
-  } else if (_upb_MiniTableField_InOneOf(field)) {
-    *_upb_oneofcase_field(msg, field) = field->number;
-  }
+const UPB_DESC(FieldOptions) * upb_FieldDef_Options(const upb_FieldDef* f) {
+  return f->opts;
 }
 
-UPB_INLINE bool _upb_MiniTable_ValueIsNonZero(const void* default_val,
-                                              const upb_MiniTableField* field) {
-  char zero[16] = {0};
-  switch (_upb_MiniTableField_GetRep(field)) {
-    case kUpb_FieldRep_1Byte:
-      return memcmp(&zero, default_val, 1) != 0;
-    case kUpb_FieldRep_4Byte:
-      return memcmp(&zero, default_val, 4) != 0;
-    case kUpb_FieldRep_8Byte:
-      return memcmp(&zero, default_val, 8) != 0;
-    case kUpb_FieldRep_StringView: {
-      const upb_StringView* sv = (const upb_StringView*)default_val;
-      return sv->size != 0;
-    }
+bool upb_FieldDef_HasOptions(const upb_FieldDef* f) {
+  return f->opts != (void*)kUpbDefOptDefault;
+}
+
+const char* upb_FieldDef_FullName(const upb_FieldDef* f) {
+  return f->full_name;
+}
+
+upb_CType upb_FieldDef_CType(const upb_FieldDef* f) {
+  switch (f->type_) {
+    case kUpb_FieldType_Double:
+      return kUpb_CType_Double;
+    case kUpb_FieldType_Float:
+      return kUpb_CType_Float;
+    case kUpb_FieldType_Int64:
+    case kUpb_FieldType_SInt64:
+    case kUpb_FieldType_SFixed64:
+      return kUpb_CType_Int64;
+    case kUpb_FieldType_Int32:
+    case kUpb_FieldType_SFixed32:
+    case kUpb_FieldType_SInt32:
+      return kUpb_CType_Int32;
+    case kUpb_FieldType_UInt64:
+    case kUpb_FieldType_Fixed64:
+      return kUpb_CType_UInt64;
+    case kUpb_FieldType_UInt32:
+    case kUpb_FieldType_Fixed32:
+      return kUpb_CType_UInt32;
+    case kUpb_FieldType_Enum:
+      return kUpb_CType_Enum;
+    case kUpb_FieldType_Bool:
+      return kUpb_CType_Bool;
+    case kUpb_FieldType_String:
+      return kUpb_CType_String;
+    case kUpb_FieldType_Bytes:
+      return kUpb_CType_Bytes;
+    case kUpb_FieldType_Group:
+    case kUpb_FieldType_Message:
+      return kUpb_CType_Message;
   }
   UPB_UNREACHABLE();
 }
 
-UPB_INLINE void _upb_MiniTable_CopyFieldData(void* to, const void* from,
-                                             const upb_MiniTableField* field) {
-  switch (_upb_MiniTableField_GetRep(field)) {
-    case kUpb_FieldRep_1Byte:
-      memcpy(to, from, 1);
-      return;
-    case kUpb_FieldRep_4Byte:
-      memcpy(to, from, 4);
-      return;
-    case kUpb_FieldRep_8Byte:
-      memcpy(to, from, 8);
-      return;
-    case kUpb_FieldRep_StringView: {
-      memcpy(to, from, sizeof(upb_StringView));
-      return;
+upb_FieldType upb_FieldDef_Type(const upb_FieldDef* f) { return f->type_; }
+
+uint32_t upb_FieldDef_Index(const upb_FieldDef* f) { return f->index_; }
+
+upb_Label upb_FieldDef_Label(const upb_FieldDef* f) { return f->label_; }
+
+uint32_t upb_FieldDef_Number(const upb_FieldDef* f) { return f->number_; }
+
+bool upb_FieldDef_IsExtension(const upb_FieldDef* f) { return f->is_extension; }
+
+bool upb_FieldDef_IsPacked(const upb_FieldDef* f) { return f->is_packed; }
+
+const char* upb_FieldDef_Name(const upb_FieldDef* f) {
+  return _upb_DefBuilder_FullToShort(f->full_name);
+}
+
+const char* upb_FieldDef_JsonName(const upb_FieldDef* f) {
+  return f->json_name;
+}
+
+bool upb_FieldDef_HasJsonName(const upb_FieldDef* f) {
+  return f->has_json_name;
+}
+
+const upb_FileDef* upb_FieldDef_File(const upb_FieldDef* f) { return f->file; }
+
+const upb_MessageDef* upb_FieldDef_ContainingType(const upb_FieldDef* f) {
+  return f->msgdef;
+}
+
+const upb_MessageDef* upb_FieldDef_ExtensionScope(const upb_FieldDef* f) {
+  return f->is_extension ? f->scope.extension_scope : NULL;
+}
+
+const upb_OneofDef* upb_FieldDef_ContainingOneof(const upb_FieldDef* f) {
+  return f->is_extension ? NULL : f->scope.oneof;
+}
+
+const upb_OneofDef* upb_FieldDef_RealContainingOneof(const upb_FieldDef* f) {
+  const upb_OneofDef* oneof = upb_FieldDef_ContainingOneof(f);
+  if (!oneof || upb_OneofDef_IsSynthetic(oneof)) return NULL;
+  return oneof;
+}
+
+upb_MessageValue upb_FieldDef_Default(const upb_FieldDef* f) {
+  upb_MessageValue ret;
+
+  if (upb_FieldDef_IsRepeated(f) || upb_FieldDef_IsSubMessage(f)) {
+    return (upb_MessageValue){.msg_val = NULL};
+  }
+
+  switch (upb_FieldDef_CType(f)) {
+    case kUpb_CType_Bool:
+      return (upb_MessageValue){.bool_val = f->defaultval.boolean};
+    case kUpb_CType_Int64:
+      return (upb_MessageValue){.int64_val = f->defaultval.sint};
+    case kUpb_CType_UInt64:
+      return (upb_MessageValue){.uint64_val = f->defaultval.uint};
+    case kUpb_CType_Enum:
+    case kUpb_CType_Int32:
+      return (upb_MessageValue){.int32_val = (int32_t)f->defaultval.sint};
+    case kUpb_CType_UInt32:
+      return (upb_MessageValue){.uint32_val = (uint32_t)f->defaultval.uint};
+    case kUpb_CType_Float:
+      return (upb_MessageValue){.float_val = f->defaultval.flt};
+    case kUpb_CType_Double:
+      return (upb_MessageValue){.double_val = f->defaultval.dbl};
+    case kUpb_CType_String:
+    case kUpb_CType_Bytes: {
+      str_t* str = f->defaultval.str;
+      if (str) {
+        return (upb_MessageValue){
+            .str_val = (upb_StringView){.data = str->str, .size = str->len}};
+      } else {
+        return (upb_MessageValue){
+            .str_val = (upb_StringView){.data = NULL, .size = 0}};
+      }
     }
+    default:
+      UPB_UNREACHABLE();
   }
-  UPB_UNREACHABLE();
+
+  return ret;
 }
 
-UPB_INLINE size_t
-_upb_MiniTable_ElementSizeLg2(const upb_MiniTableField* field) {
-  const unsigned char table[] = {
-      0,
-      3,               // kUpb_FieldType_Double = 1,
-      2,               // kUpb_FieldType_Float = 2,
-      3,               // kUpb_FieldType_Int64 = 3,
-      3,               // kUpb_FieldType_UInt64 = 4,
-      2,               // kUpb_FieldType_Int32 = 5,
-      3,               // kUpb_FieldType_Fixed64 = 6,
-      2,               // kUpb_FieldType_Fixed32 = 7,
-      0,               // kUpb_FieldType_Bool = 8,
-      UPB_SIZE(3, 4),  // kUpb_FieldType_String = 9,
-      UPB_SIZE(2, 3),  // kUpb_FieldType_Group = 10,
-      UPB_SIZE(2, 3),  // kUpb_FieldType_Message = 11,
-      UPB_SIZE(3, 4),  // kUpb_FieldType_Bytes = 12,
-      2,               // kUpb_FieldType_UInt32 = 13,
-      2,               // kUpb_FieldType_Enum = 14,
-      2,               // kUpb_FieldType_SFixed32 = 15,
-      3,               // kUpb_FieldType_SFixed64 = 16,
-      2,               // kUpb_FieldType_SInt32 = 17,
-      3,               // kUpb_FieldType_SInt64 = 18,
-  };
-  return table[field->descriptortype];
-}
-
-// Here we define universal getter/setter functions for message fields.
-// These look very branchy and inefficient, but as long as the MiniTableField
-// values are known at compile time, all the branches are optimized away and
-// we are left with ideal code.  This can happen either through through
-// literals or UPB_ASSUME():
-//
-//   // Via struct literals.
-//   bool FooMessage_set_bool_field(const upb_Message* msg, bool val) {
-//     const upb_MiniTableField field = {1, 0, 0, /* etc... */};
-//     // All value in "field" are compile-time known.
-//     _upb_Message_SetNonExtensionField(msg, &field, &value);
-//   }
-//
-//   // Via UPB_ASSUME().
-//   UPB_INLINE bool upb_Message_SetBool(upb_Message* msg,
-//                                       const upb_MiniTableField* field,
-//                                       bool value, upb_Arena* a) {
-//     UPB_ASSUME(field->descriptortype == kUpb_FieldType_Bool);
-//     UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-//     UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_1Byte);
-//     _upb_Message_SetField(msg, field, &value, a);
-//   }
-//
-// As a result, we can use these universal getters/setters for *all* message
-// accessors: generated code, MiniTable accessors, and reflection.  The only
-// exception is the binary encoder/decoder, which need to be a bit more clever
-// about how they read/write the message data, for efficiency.
-//
-// These functions work on both extensions and non-extensions. If the field
-// of a setter is known to be a non-extension, the arena may be NULL and the
-// returned bool value may be ignored since it will always succeed.
-
-UPB_INLINE bool _upb_Message_HasExtensionField(
-    const upb_Message* msg, const upb_MiniTableExtension* ext) {
-  UPB_ASSERT(upb_MiniTableField_HasPresence(&ext->field));
-  return _upb_Message_Getext(msg, ext) != NULL;
-}
-
-UPB_INLINE bool _upb_Message_HasNonExtensionField(
-    const upb_Message* msg, const upb_MiniTableField* field) {
-  UPB_ASSERT(upb_MiniTableField_HasPresence(field));
-  UPB_ASSUME(!upb_MiniTableField_IsExtension(field));
-  if (_upb_MiniTableField_InOneOf(field)) {
-    return _upb_getoneofcase_field(msg, field) == field->number;
-  } else {
-    return _upb_hasbit_field(msg, field);
-  }
+const upb_MessageDef* upb_FieldDef_MessageSubDef(const upb_FieldDef* f) {
+  return upb_FieldDef_CType(f) == kUpb_CType_Message ? f->sub.msgdef : NULL;
 }
 
-static UPB_FORCEINLINE void _upb_Message_GetNonExtensionField(
-    const upb_Message* msg, const upb_MiniTableField* field,
-    const void* default_val, void* val) {
-  UPB_ASSUME(!upb_MiniTableField_IsExtension(field));
-  if ((_upb_MiniTableField_InOneOf(field) ||
-       _upb_MiniTable_ValueIsNonZero(default_val, field)) &&
-      !_upb_Message_HasNonExtensionField(msg, field)) {
-    _upb_MiniTable_CopyFieldData(val, default_val, field);
-    return;
-  }
-  _upb_MiniTable_CopyFieldData(val, _upb_MiniTableField_GetConstPtr(msg, field),
-                               field);
-}
-
-UPB_INLINE void _upb_Message_GetExtensionField(
-    const upb_Message* msg, const upb_MiniTableExtension* mt_ext,
-    const void* default_val, void* val) {
-  UPB_ASSUME(upb_MiniTableField_IsExtension(&mt_ext->field));
-  const upb_Message_Extension* ext = _upb_Message_Getext(msg, mt_ext);
-  if (ext) {
-    _upb_MiniTable_CopyFieldData(val, &ext->data, &mt_ext->field);
-  } else {
-    _upb_MiniTable_CopyFieldData(val, default_val, &mt_ext->field);
-  }
+const upb_EnumDef* upb_FieldDef_EnumSubDef(const upb_FieldDef* f) {
+  return upb_FieldDef_CType(f) == kUpb_CType_Enum ? f->sub.enumdef : NULL;
 }
 
-UPB_INLINE void _upb_Message_GetField(const upb_Message* msg,
-                                      const upb_MiniTableField* field,
-                                      const void* default_val, void* val) {
-  if (upb_MiniTableField_IsExtension(field)) {
-    _upb_Message_GetExtensionField(msg, (upb_MiniTableExtension*)field,
-                                   default_val, val);
+const upb_MiniTableField* upb_FieldDef_MiniTable(const upb_FieldDef* f) {
+  if (upb_FieldDef_IsExtension(f)) {
+    const upb_FileDef* file = upb_FieldDef_File(f);
+    return (upb_MiniTableField*)_upb_FileDef_ExtensionMiniTable(
+        file, f->layout_index);
   } else {
-    _upb_Message_GetNonExtensionField(msg, field, default_val, val);
+    const upb_MiniTable* layout = upb_MessageDef_MiniTable(f->msgdef);
+    return &layout->fields[f->layout_index];
   }
 }
 
-UPB_INLINE void _upb_Message_SetNonExtensionField(
-    upb_Message* msg, const upb_MiniTableField* field, const void* val) {
-  UPB_ASSUME(!upb_MiniTableField_IsExtension(field));
-  _upb_Message_SetPresence(msg, field);
-  _upb_MiniTable_CopyFieldData(_upb_MiniTableField_GetPtr(msg, field), val,
-                               field);
-}
-
-UPB_INLINE bool _upb_Message_SetExtensionField(
-    upb_Message* msg, const upb_MiniTableExtension* mt_ext, const void* val,
-    upb_Arena* a) {
-  UPB_ASSERT(a);
-  upb_Message_Extension* ext =
-      _upb_Message_GetOrCreateExtension(msg, mt_ext, a);
-  if (!ext) return false;
-  _upb_MiniTable_CopyFieldData(&ext->data, val, &mt_ext->field);
-  return true;
+const upb_MiniTableExtension* _upb_FieldDef_ExtensionMiniTable(
+    const upb_FieldDef* f) {
+  UPB_ASSERT(upb_FieldDef_IsExtension(f));
+  const upb_FileDef* file = upb_FieldDef_File(f);
+  return _upb_FileDef_ExtensionMiniTable(file, f->layout_index);
 }
 
-UPB_INLINE bool _upb_Message_SetField(upb_Message* msg,
-                                      const upb_MiniTableField* field,
-                                      const void* val, upb_Arena* a) {
-  if (upb_MiniTableField_IsExtension(field)) {
-    const upb_MiniTableExtension* ext = (const upb_MiniTableExtension*)field;
-    return _upb_Message_SetExtensionField(msg, ext, val, a);
-  } else {
-    _upb_Message_SetNonExtensionField(msg, field, val);
-    return true;
-  }
+bool _upb_FieldDef_IsClosedEnum(const upb_FieldDef* f) {
+  if (f->type_ != kUpb_FieldType_Enum) return false;
+  return upb_EnumDef_IsClosed(f->sub.enumdef);
 }
 
-UPB_INLINE void _upb_Message_ClearExtensionField(
-    upb_Message* msg, const upb_MiniTableExtension* ext_l) {
-  upb_Message_Internal* in = upb_Message_Getinternal(msg);
-  if (!in->internal) return;
-  const upb_Message_Extension* base =
-      UPB_PTR_AT(in->internal, in->internal->ext_begin, upb_Message_Extension);
-  upb_Message_Extension* ext =
-      (upb_Message_Extension*)_upb_Message_Getext(msg, ext_l);
-  if (ext) {
-    *ext = *base;
-    in->internal->ext_begin += sizeof(upb_Message_Extension);
-  }
+bool _upb_FieldDef_IsProto3Optional(const upb_FieldDef* f) {
+  return f->is_proto3_optional;
 }
 
-UPB_INLINE void _upb_Message_ClearNonExtensionField(
-    upb_Message* msg, const upb_MiniTableField* field) {
-  if (field->presence > 0) {
-    _upb_clearhas(msg, _upb_Message_Hasidx(field));
-  } else if (_upb_MiniTableField_InOneOf(field)) {
-    uint32_t* oneof_case = _upb_oneofcase_field(msg, field);
-    if (*oneof_case != field->number) return;
-    *oneof_case = 0;
-  }
-  const char zeros[16] = {0};
-  _upb_MiniTable_CopyFieldData(_upb_MiniTableField_GetPtr(msg, field), zeros,
-                               field);
-}
-
-UPB_INLINE upb_Map* _upb_Message_GetOrCreateMutableMap(
-    upb_Message* msg, const upb_MiniTableField* field, size_t key_size,
-    size_t val_size, upb_Arena* arena) {
-  _upb_MiniTableField_CheckIsMap(field);
-  upb_Map* map = NULL;
-  upb_Map* default_map_value = NULL;
-  _upb_Message_GetNonExtensionField(msg, field, &default_map_value, &map);
-  if (!map) {
-    map = _upb_Map_New(arena, key_size, val_size);
-    // Check again due to: https://godbolt.org/z/7WfaoKG1r
-    _upb_MiniTableField_CheckIsMap(field);
-    _upb_Message_SetNonExtensionField(msg, field, &map);
-  }
-  return map;
-}
-
-// EVERYTHING ABOVE THIS LINE IS INTERNAL - DO NOT USE /////////////////////////
-
-UPB_API_INLINE void upb_Message_ClearField(upb_Message* msg,
-                                           const upb_MiniTableField* field) {
-  if (upb_MiniTableField_IsExtension(field)) {
-    const upb_MiniTableExtension* ext = (const upb_MiniTableExtension*)field;
-    _upb_Message_ClearExtensionField(msg, ext);
-  } else {
-    _upb_Message_ClearNonExtensionField(msg, field);
+int _upb_FieldDef_LayoutIndex(const upb_FieldDef* f) { return f->layout_index; }
+
+uint64_t _upb_FieldDef_Modifiers(const upb_FieldDef* f) {
+  uint64_t out = f->is_packed ? kUpb_FieldModifier_IsPacked : 0;
+
+  switch (f->label_) {
+    case kUpb_Label_Optional:
+      if (!upb_FieldDef_HasPresence(f)) {
+        out |= kUpb_FieldModifier_IsProto3Singular;
+      }
+      break;
+    case kUpb_Label_Repeated:
+      out |= kUpb_FieldModifier_IsRepeated;
+      break;
+    case kUpb_Label_Required:
+      out |= kUpb_FieldModifier_IsRequired;
+      break;
   }
-}
 
-UPB_API_INLINE bool upb_Message_HasField(const upb_Message* msg,
-                                         const upb_MiniTableField* field) {
-  if (upb_MiniTableField_IsExtension(field)) {
-    const upb_MiniTableExtension* ext = (const upb_MiniTableExtension*)field;
-    return _upb_Message_HasExtensionField(msg, ext);
-  } else {
-    return _upb_Message_HasNonExtensionField(msg, field);
+  if (_upb_FieldDef_IsClosedEnum(f)) {
+    out |= kUpb_FieldModifier_IsClosedEnum;
   }
+  return out;
 }
 
-UPB_API_INLINE uint32_t upb_Message_WhichOneofFieldNumber(
-    const upb_Message* message, const upb_MiniTableField* oneof_field) {
-  UPB_ASSUME(_upb_MiniTableField_InOneOf(oneof_field));
-  return _upb_getoneofcase_field(message, oneof_field);
+bool upb_FieldDef_HasDefault(const upb_FieldDef* f) { return f->has_default; }
+bool upb_FieldDef_HasPresence(const upb_FieldDef* f) { return f->has_presence; }
+
+bool upb_FieldDef_HasSubDef(const upb_FieldDef* f) {
+  return upb_FieldDef_IsSubMessage(f) ||
+         upb_FieldDef_CType(f) == kUpb_CType_Enum;
 }
 
-UPB_API_INLINE bool upb_Message_GetBool(const upb_Message* msg,
-                                        const upb_MiniTableField* field,
-                                        bool default_val) {
-  UPB_ASSUME(field->descriptortype == kUpb_FieldType_Bool);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_1Byte);
-  bool ret;
-  _upb_Message_GetField(msg, field, &default_val, &ret);
-  return ret;
+bool upb_FieldDef_IsMap(const upb_FieldDef* f) {
+  return upb_FieldDef_IsRepeated(f) && upb_FieldDef_IsSubMessage(f) &&
+         upb_MessageDef_IsMapEntry(upb_FieldDef_MessageSubDef(f));
 }
 
-UPB_API_INLINE bool upb_Message_SetBool(upb_Message* msg,
-                                        const upb_MiniTableField* field,
-                                        bool value, upb_Arena* a) {
-  UPB_ASSUME(field->descriptortype == kUpb_FieldType_Bool);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_1Byte);
-  return _upb_Message_SetField(msg, field, &value, a);
-}
-
-UPB_API_INLINE int32_t upb_Message_GetInt32(const upb_Message* msg,
-                                            const upb_MiniTableField* field,
-                                            int32_t default_val) {
-  UPB_ASSUME(field->descriptortype == kUpb_FieldType_Int32 ||
-             field->descriptortype == kUpb_FieldType_SInt32 ||
-             field->descriptortype == kUpb_FieldType_SFixed32 ||
-             field->descriptortype == kUpb_FieldType_Enum);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_4Byte);
-  int32_t ret;
-  _upb_Message_GetField(msg, field, &default_val, &ret);
-  return ret;
+bool upb_FieldDef_IsOptional(const upb_FieldDef* f) {
+  return upb_FieldDef_Label(f) == kUpb_Label_Optional;
 }
 
-UPB_API_INLINE bool upb_Message_SetInt32(upb_Message* msg,
-                                         const upb_MiniTableField* field,
-                                         int32_t value, upb_Arena* a) {
-  UPB_ASSUME(field->descriptortype == kUpb_FieldType_Int32 ||
-             field->descriptortype == kUpb_FieldType_SInt32 ||
-             field->descriptortype == kUpb_FieldType_SFixed32);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_4Byte);
-  return _upb_Message_SetField(msg, field, &value, a);
-}
-
-UPB_API_INLINE uint32_t upb_Message_GetUInt32(const upb_Message* msg,
-                                              const upb_MiniTableField* field,
-                                              uint32_t default_val) {
-  UPB_ASSUME(field->descriptortype == kUpb_FieldType_UInt32 ||
-             field->descriptortype == kUpb_FieldType_Fixed32);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_4Byte);
-  uint32_t ret;
-  _upb_Message_GetField(msg, field, &default_val, &ret);
-  return ret;
+bool upb_FieldDef_IsPrimitive(const upb_FieldDef* f) {
+  return !upb_FieldDef_IsString(f) && !upb_FieldDef_IsSubMessage(f);
 }
 
-UPB_API_INLINE bool upb_Message_SetUInt32(upb_Message* msg,
-                                          const upb_MiniTableField* field,
-                                          uint32_t value, upb_Arena* a) {
-  UPB_ASSUME(field->descriptortype == kUpb_FieldType_UInt32 ||
-             field->descriptortype == kUpb_FieldType_Fixed32);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_4Byte);
-  return _upb_Message_SetField(msg, field, &value, a);
-}
-
-UPB_API_INLINE void upb_Message_SetEnumProto2(
-    upb_Message* msg, const upb_MiniTable* msg_mini_table,
-    const upb_MiniTableField* field, int32_t value) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Enum);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_4Byte);
-  UPB_ASSERT(upb_MiniTableEnum_CheckValue(
-      upb_MiniTable_GetSubEnumTable(msg_mini_table, field), value));
-  _upb_Message_SetNonExtensionField(msg, field, &value);
-}
-
-UPB_API_INLINE int64_t upb_Message_GetInt64(const upb_Message* msg,
-                                            const upb_MiniTableField* field,
-                                            uint64_t default_val) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Int64 ||
-             field->descriptortype == kUpb_FieldType_SInt64 ||
-             field->descriptortype == kUpb_FieldType_SFixed64);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_8Byte);
-  int64_t ret;
-  _upb_Message_GetField(msg, field, &default_val, &ret);
-  return ret;
+bool upb_FieldDef_IsRepeated(const upb_FieldDef* f) {
+  return upb_FieldDef_Label(f) == kUpb_Label_Repeated;
 }
 
-UPB_API_INLINE bool upb_Message_SetInt64(upb_Message* msg,
-                                         const upb_MiniTableField* field,
-                                         int64_t value, upb_Arena* a) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Int64 ||
-             field->descriptortype == kUpb_FieldType_SInt64 ||
-             field->descriptortype == kUpb_FieldType_SFixed64);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_8Byte);
-  return _upb_Message_SetField(msg, field, &value, a);
-}
-
-UPB_API_INLINE uint64_t upb_Message_GetUInt64(const upb_Message* msg,
-                                              const upb_MiniTableField* field,
-                                              uint64_t default_val) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_UInt64 ||
-             field->descriptortype == kUpb_FieldType_Fixed64);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_8Byte);
-  uint64_t ret;
-  _upb_Message_GetField(msg, field, &default_val, &ret);
-  return ret;
+bool upb_FieldDef_IsRequired(const upb_FieldDef* f) {
+  return upb_FieldDef_Label(f) == kUpb_Label_Required;
 }
 
-UPB_API_INLINE bool upb_Message_SetUInt64(upb_Message* msg,
-                                          const upb_MiniTableField* field,
-                                          uint64_t value, upb_Arena* a) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_UInt64 ||
-             field->descriptortype == kUpb_FieldType_Fixed64);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_8Byte);
-  return _upb_Message_SetField(msg, field, &value, a);
-}
-
-UPB_API_INLINE float upb_Message_GetFloat(const upb_Message* msg,
-                                          const upb_MiniTableField* field,
-                                          float default_val) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Float);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_4Byte);
-  float ret;
-  _upb_Message_GetField(msg, field, &default_val, &ret);
-  return ret;
+bool upb_FieldDef_IsString(const upb_FieldDef* f) {
+  return upb_FieldDef_CType(f) == kUpb_CType_String ||
+         upb_FieldDef_CType(f) == kUpb_CType_Bytes;
 }
 
-UPB_API_INLINE bool upb_Message_SetFloat(upb_Message* msg,
-                                         const upb_MiniTableField* field,
-                                         float value, upb_Arena* a) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Float);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_4Byte);
-  return _upb_Message_SetField(msg, field, &value, a);
-}
-
-UPB_API_INLINE double upb_Message_GetDouble(const upb_Message* msg,
-                                            const upb_MiniTableField* field,
-                                            double default_val) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Double);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_8Byte);
-  double ret;
-  _upb_Message_GetField(msg, field, &default_val, &ret);
-  return ret;
+bool upb_FieldDef_IsSubMessage(const upb_FieldDef* f) {
+  return upb_FieldDef_CType(f) == kUpb_CType_Message;
 }
 
-UPB_API_INLINE bool upb_Message_SetDouble(upb_Message* msg,
-                                          const upb_MiniTableField* field,
-                                          double value, upb_Arena* a) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Double);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_8Byte);
-  return _upb_Message_SetField(msg, field, &value, a);
-}
-
-UPB_API_INLINE upb_StringView
-upb_Message_GetString(const upb_Message* msg, const upb_MiniTableField* field,
-                      upb_StringView def_val) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Bytes ||
-             field->descriptortype == kUpb_FieldType_String);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_StringView);
-  upb_StringView ret;
-  _upb_Message_GetField(msg, field, &def_val, &ret);
-  return ret;
+static bool between(int32_t x, int32_t low, int32_t high) {
+  return x >= low && x <= high;
 }
 
-UPB_API_INLINE bool upb_Message_SetString(upb_Message* msg,
-                                          const upb_MiniTableField* field,
-                                          upb_StringView value, upb_Arena* a) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Bytes ||
-             field->descriptortype == kUpb_FieldType_String);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) == kUpb_FieldRep_StringView);
-  return _upb_Message_SetField(msg, field, &value, a);
-}
-
-UPB_API_INLINE const upb_Message* upb_Message_GetMessage(
-    const upb_Message* msg, const upb_MiniTableField* field,
-    upb_Message* default_val) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Message ||
-             field->descriptortype == kUpb_FieldType_Group);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) ==
-             UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte));
-  upb_Message* ret;
-  _upb_Message_GetNonExtensionField(msg, field, &default_val, &ret);
-  return ret;
+bool upb_FieldDef_checklabel(int32_t label) { return between(label, 1, 3); }
+bool upb_FieldDef_checktype(int32_t type) { return between(type, 1, 11); }
+bool upb_FieldDef_checkintfmt(int32_t fmt) { return between(fmt, 1, 3); }
+
+bool upb_FieldDef_checkdescriptortype(int32_t type) {
+  return between(type, 1, 18);
 }
 
-UPB_API_INLINE void upb_Message_SetMessage(upb_Message* msg,
-                                           const upb_MiniTable* mini_table,
-                                           const upb_MiniTableField* field,
-                                           upb_Message* sub_message) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Message ||
-             field->descriptortype == kUpb_FieldType_Group);
-  UPB_ASSUME(!upb_IsRepeatedOrMap(field));
-  UPB_ASSUME(_upb_MiniTableField_GetRep(field) ==
-             UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte));
-  UPB_ASSERT(mini_table->subs[field->submsg_index].submsg);
-  _upb_Message_SetNonExtensionField(msg, field, &sub_message);
-}
-
-UPB_API_INLINE upb_Message* upb_Message_GetOrCreateMutableMessage(
-    upb_Message* msg, const upb_MiniTable* mini_table,
-    const upb_MiniTableField* field, upb_Arena* arena) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Message ||
-             field->descriptortype == kUpb_FieldType_Group);
-  upb_Message* sub_message = *UPB_PTR_AT(msg, field->offset, upb_Message*);
-  if (!sub_message) {
-    const upb_MiniTable* sub_mini_table =
-        mini_table->subs[field->submsg_index].submsg;
-    UPB_ASSERT(sub_mini_table);
-    sub_message = _upb_Message_New(sub_mini_table, arena);
-    *UPB_PTR_AT(msg, field->offset, upb_Message*) = sub_message;
-    _upb_Message_SetPresence(msg, field);
-  }
-  return sub_message;
-}
-
-UPB_API_INLINE const upb_Array* upb_Message_GetArray(
-    const upb_Message* msg, const upb_MiniTableField* field) {
-  _upb_MiniTableField_CheckIsArray(field);
-  const upb_Array* ret;
-  const upb_Array* default_val = NULL;
-  _upb_Message_GetNonExtensionField(msg, field, &default_val, &ret);
+static bool streql2(const char* a, size_t n, const char* b) {
+  return n == strlen(b) && memcmp(a, b, n) == 0;
+}
+
+// Implement the transformation as described in the spec:
+//   1. upper case all letters after an underscore.
+//   2. remove all underscores.
+static char* make_json_name(const char* name, size_t size, upb_Arena* a) {
+  char* out = upb_Arena_Malloc(a, size + 1);  // +1 is to add a trailing '\0'
+  if (out == NULL) return NULL;
+
+  bool ucase_next = false;
+  char* des = out;
+  for (size_t i = 0; i < size; i++) {
+    if (name[i] == '_') {
+      ucase_next = true;
+    } else {
+      *des++ = ucase_next ? toupper(name[i]) : name[i];
+      ucase_next = false;
+    }
+  }
+  *des++ = '\0';
+  return out;
+}
+
+static str_t* newstr(upb_DefBuilder* ctx, const char* data, size_t len) {
+  str_t* ret = _upb_DefBuilder_Alloc(ctx, sizeof(*ret) + len);
+  if (!ret) _upb_DefBuilder_OomErr(ctx);
+  ret->len = len;
+  if (len) memcpy(ret->str, data, len);
+  ret->str[len] = '\0';
   return ret;
 }
 
-UPB_API_INLINE upb_Array* upb_Message_GetMutableArray(
-    upb_Message* msg, const upb_MiniTableField* field) {
-  _upb_MiniTableField_CheckIsArray(field);
-  return (upb_Array*)upb_Message_GetArray(msg, field);
-}
-
-UPB_API_INLINE upb_Array* upb_Message_GetOrCreateMutableArray(
-    upb_Message* msg, const upb_MiniTableField* field, upb_Arena* arena) {
-  _upb_MiniTableField_CheckIsArray(field);
-  upb_Array* array = upb_Message_GetMutableArray(msg, field);
-  if (!array) {
-    array = _upb_Array_New(arena, 4, _upb_MiniTable_ElementSizeLg2(field));
-    // Check again due to: https://godbolt.org/z/7WfaoKG1r
-    _upb_MiniTableField_CheckIsArray(field);
-    _upb_Message_SetField(msg, field, &array, arena);
-  }
-  return array;
-}
-
-UPB_INLINE upb_Array* upb_Message_ResizeArrayUninitialized(
-    upb_Message* msg, const upb_MiniTableField* field, size_t size,
-    upb_Arena* arena) {
-  _upb_MiniTableField_CheckIsArray(field);
-  upb_Array* arr = upb_Message_GetOrCreateMutableArray(msg, field, arena);
-  if (!arr || !_upb_Array_ResizeUninitialized(arr, size, arena)) return NULL;
-  return arr;
-}
-
-// TODO: remove, migrate users to upb_Message_ResizeArrayUninitialized(), which
-// has the same semantics but a clearer name. Alternatively, if users want an
-// initialized variant, we can also offer that.
-UPB_API_INLINE void* upb_Message_ResizeArray(upb_Message* msg,
-                                             const upb_MiniTableField* field,
-                                             size_t size, upb_Arena* arena) {
-  _upb_MiniTableField_CheckIsArray(field);
-  upb_Array* arr =
-      upb_Message_ResizeArrayUninitialized(msg, field, size, arena);
-  return _upb_array_ptr(arr);
-}
-
-UPB_API_INLINE bool upb_MiniTableField_IsClosedEnum(
-    const upb_MiniTableField* field) {
-  return field->descriptortype == kUpb_FieldType_Enum;
-}
-
-UPB_API_INLINE const upb_Map* upb_Message_GetMap(
-    const upb_Message* msg, const upb_MiniTableField* field) {
-  _upb_MiniTableField_CheckIsMap(field);
-  const upb_Map* ret;
-  const upb_Map* default_val = NULL;
-  _upb_Message_GetNonExtensionField(msg, field, &default_val, &ret);
+static str_t* unescape(upb_DefBuilder* ctx, const upb_FieldDef* f,
+                       const char* data, size_t len) {
+  // Size here is an upper bound; escape sequences could ultimately shrink it.
+  str_t* ret = _upb_DefBuilder_Alloc(ctx, sizeof(*ret) + len);
+  char* dst = &ret->str[0];
+  const char* src = data;
+  const char* end = data + len;
+
+  while (src < end) {
+    if (*src == '\\') {
+      src++;
+      *dst++ = _upb_DefBuilder_ParseEscape(ctx, f, &src, end);
+    } else {
+      *dst++ = *src++;
+    }
+  }
+
+  ret->len = dst - &ret->str[0];
   return ret;
 }
 
-UPB_API_INLINE upb_Map* upb_Message_GetOrCreateMutableMap(
-    upb_Message* msg, const upb_MiniTable* map_entry_mini_table,
-    const upb_MiniTableField* field, upb_Arena* arena) {
-  UPB_ASSERT(field->descriptortype == kUpb_FieldType_Message ||
-             field->descriptortype == kUpb_FieldType_Group);
-  const upb_MiniTableField* map_entry_key_field =
-      &map_entry_mini_table->fields[0];
-  const upb_MiniTableField* map_entry_value_field =
-      &map_entry_mini_table->fields[1];
-  return _upb_Message_GetOrCreateMutableMap(
-      msg, field,
-      _upb_Map_CTypeSize(upb_MiniTableField_CType(map_entry_key_field)),
-      _upb_Map_CTypeSize(upb_MiniTableField_CType(map_entry_value_field)),
-      arena);
-}
-
-// Updates a map entry given an entry message.
-upb_MapInsertStatus upb_Message_InsertMapEntry(upb_Map* map,
-                                               const upb_MiniTable* mini_table,
-                                               const upb_MiniTableField* field,
-                                               upb_Message* map_entry_message,
-                                               upb_Arena* arena);
-
-typedef enum {
-  kUpb_GetExtension_Ok,
-  kUpb_GetExtension_NotPresent,
-  kUpb_GetExtension_ParseError,
-  kUpb_GetExtension_OutOfMemory,
-} upb_GetExtension_Status;
-
-typedef enum {
-  kUpb_GetExtensionAsBytes_Ok,
-  kUpb_GetExtensionAsBytes_NotPresent,
-  kUpb_GetExtensionAsBytes_EncodeError,
-} upb_GetExtensionAsBytes_Status;
-
-// Returns a message extension or promotes an unknown field to
-// an extension.
-//
-// TODO(ferhat): Only supports extension fields that are messages,
-// expand support to include non-message types.
-upb_GetExtension_Status upb_MiniTable_GetOrPromoteExtension(
-    upb_Message* msg, const upb_MiniTableExtension* ext_table,
-    int decode_options, upb_Arena* arena,
-    const upb_Message_Extension** extension);
-
-// Returns a message extension or unknown field matching the extension
-// data as bytes.
-//
-// If an extension has already been decoded it will be re-encoded
-// to bytes.
-upb_GetExtensionAsBytes_Status upb_MiniTable_GetExtensionAsBytes(
-    const upb_Message* msg, const upb_MiniTableExtension* ext_table,
-    int encode_options, upb_Arena* arena, const char** extension_data,
-    size_t* len);
-
-typedef enum {
-  kUpb_FindUnknown_Ok,
-  kUpb_FindUnknown_NotPresent,
-  kUpb_FindUnknown_ParseError,
-} upb_FindUnknown_Status;
+static void parse_default(upb_DefBuilder* ctx, const char* str, size_t len,
+                          upb_FieldDef* f) {
+  char* end;
+  char nullz[64];
+  errno = 0;
+
+  switch (upb_FieldDef_CType(f)) {
+    case kUpb_CType_Int32:
+    case kUpb_CType_Int64:
+    case kUpb_CType_UInt32:
+    case kUpb_CType_UInt64:
+    case kUpb_CType_Double:
+    case kUpb_CType_Float:
+      // Standard C number parsing functions expect null-terminated strings.
+      if (len >= sizeof(nullz) - 1) {
+        _upb_DefBuilder_Errf(ctx, "Default too long: %.*s", (int)len, str);
+      }
+      memcpy(nullz, str, len);
+      nullz[len] = '\0';
+      str = nullz;
+      break;
+    default:
+      break;
+  }
+
+  switch (upb_FieldDef_CType(f)) {
+    case kUpb_CType_Int32: {
+      long val = strtol(str, &end, 0);
+      if (val > INT32_MAX || val < INT32_MIN || errno == ERANGE || *end) {
+        goto invalid;
+      }
+      f->defaultval.sint = val;
+      break;
+    }
+    case kUpb_CType_Enum: {
+      const upb_EnumDef* e = f->sub.enumdef;
+      const upb_EnumValueDef* ev =
+          upb_EnumDef_FindValueByNameWithSize(e, str, len);
+      if (!ev) {
+        goto invalid;
+      }
+      f->defaultval.sint = upb_EnumValueDef_Number(ev);
+      break;
+    }
+    case kUpb_CType_Int64: {
+      long long val = strtoll(str, &end, 0);
+      if (val > INT64_MAX || val < INT64_MIN || errno == ERANGE || *end) {
+        goto invalid;
+      }
+      f->defaultval.sint = val;
+      break;
+    }
+    case kUpb_CType_UInt32: {
+      unsigned long val = strtoul(str, &end, 0);
+      if (val > UINT32_MAX || errno == ERANGE || *end) {
+        goto invalid;
+      }
+      f->defaultval.uint = val;
+      break;
+    }
+    case kUpb_CType_UInt64: {
+      unsigned long long val = strtoull(str, &end, 0);
+      if (val > UINT64_MAX || errno == ERANGE || *end) {
+        goto invalid;
+      }
+      f->defaultval.uint = val;
+      break;
+    }
+    case kUpb_CType_Double: {
+      double val = strtod(str, &end);
+      if (errno == ERANGE || *end) {
+        goto invalid;
+      }
+      f->defaultval.dbl = val;
+      break;
+    }
+    case kUpb_CType_Float: {
+      float val = strtof(str, &end);
+      if (errno == ERANGE || *end) {
+        goto invalid;
+      }
+      f->defaultval.flt = val;
+      break;
+    }
+    case kUpb_CType_Bool: {
+      if (streql2(str, len, "false")) {
+        f->defaultval.boolean = false;
+      } else if (streql2(str, len, "true")) {
+        f->defaultval.boolean = true;
+      } else {
+        goto invalid;
+      }
+      break;
+    }
+    case kUpb_CType_String:
+      f->defaultval.str = newstr(ctx, str, len);
+      break;
+    case kUpb_CType_Bytes:
+      f->defaultval.str = unescape(ctx, f, str, len);
+      break;
+    case kUpb_CType_Message:
+      /* Should not have a default value. */
+      _upb_DefBuilder_Errf(ctx, "Message should not have a default (%s)",
+                           upb_FieldDef_FullName(f));
+  }
+
+  return;
+
+invalid:
+  _upb_DefBuilder_Errf(ctx, "Invalid default '%.*s' for field %s of type %d",
+                       (int)len, str, upb_FieldDef_FullName(f),
+                       (int)upb_FieldDef_Type(f));
+}
+
+static void set_default_default(upb_DefBuilder* ctx, upb_FieldDef* f) {
+  switch (upb_FieldDef_CType(f)) {
+    case kUpb_CType_Int32:
+    case kUpb_CType_Int64:
+      f->defaultval.sint = 0;
+      break;
+    case kUpb_CType_UInt64:
+    case kUpb_CType_UInt32:
+      f->defaultval.uint = 0;
+      break;
+    case kUpb_CType_Double:
+    case kUpb_CType_Float:
+      f->defaultval.dbl = 0;
+      break;
+    case kUpb_CType_String:
+    case kUpb_CType_Bytes:
+      f->defaultval.str = newstr(ctx, NULL, 0);
+      break;
+    case kUpb_CType_Bool:
+      f->defaultval.boolean = false;
+      break;
+    case kUpb_CType_Enum: {
+      const upb_EnumValueDef* v = upb_EnumDef_Value(f->sub.enumdef, 0);
+      f->defaultval.sint = upb_EnumValueDef_Number(v);
+      break;
+    }
+    case kUpb_CType_Message:
+      break;
+  }
+}
 
-typedef struct {
-  upb_FindUnknown_Status status;
-  // Start of unknown field data in message arena.
-  const char* ptr;
-  // Size of unknown field data.
-  size_t len;
-} upb_FindUnknownRet;
+static void _upb_FieldDef_Create(upb_DefBuilder* ctx, const char* prefix,
+                                 const UPB_DESC(FieldDescriptorProto) *
+                                     field_proto,
+                                 upb_MessageDef* m, upb_FieldDef* f) {
+  // Must happen before _upb_DefBuilder_Add()
+  f->file = _upb_DefBuilder_File(ctx);
 
-// Finds first occurrence of unknown data by tag id in message.
-upb_FindUnknownRet upb_MiniTable_FindUnknown(const upb_Message* msg,
-                                             uint32_t field_number);
-
-typedef enum {
-  kUpb_UnknownToMessage_Ok,
-  kUpb_UnknownToMessage_ParseError,
-  kUpb_UnknownToMessage_OutOfMemory,
-  kUpb_UnknownToMessage_NotFound,
-} upb_UnknownToMessage_Status;
+  if (!UPB_DESC(FieldDescriptorProto_has_name)(field_proto)) {
+    _upb_DefBuilder_Errf(ctx, "field has no name");
+  }
 
-typedef struct {
-  upb_UnknownToMessage_Status status;
-  upb_Message* message;
-} upb_UnknownToMessageRet;
-
-// Promotes unknown data inside message to a upb_Message parsing the unknown.
-//
-// The unknown data is removed from message after field value is set
-// using upb_Message_SetMessage.
-//
-// WARNING!: See b/267655898
-upb_UnknownToMessageRet upb_MiniTable_PromoteUnknownToMessage(
-    upb_Message* msg, const upb_MiniTable* mini_table,
-    const upb_MiniTableField* field, const upb_MiniTable* sub_mini_table,
-    int decode_options, upb_Arena* arena);
-
-// Promotes all unknown data that matches field tag id to repeated messages
-// in upb_Array.
-//
-// The unknown data is removed from message after upb_Array is populated.
-// Since repeated messages can't be packed we remove each unknown that
-// contains the target tag id.
-upb_UnknownToMessage_Status upb_MiniTable_PromoteUnknownToMessageArray(
-    upb_Message* msg, const upb_MiniTableField* field,
-    const upb_MiniTable* mini_table, int decode_options, upb_Arena* arena);
-
-// Promotes all unknown data that matches field tag id to upb_Map.
-//
-// The unknown data is removed from message after upb_Map is populated.
-// Since repeated messages can't be packed we remove each unknown that
-// contains the target tag id.
-upb_UnknownToMessage_Status upb_MiniTable_PromoteUnknownToMap(
-    upb_Message* msg, const upb_MiniTable* mini_table,
-    const upb_MiniTableField* field, int decode_options, upb_Arena* arena);
+  const upb_StringView name = UPB_DESC(FieldDescriptorProto_name)(field_proto);
 
-#ifdef __cplusplus
-} /* extern "C" */
-#endif
+  f->full_name = _upb_DefBuilder_MakeFullName(ctx, prefix, name);
+  f->label_ = (int)UPB_DESC(FieldDescriptorProto_label)(field_proto);
+  f->number_ = UPB_DESC(FieldDescriptorProto_number)(field_proto);
+  f->is_proto3_optional =
+      UPB_DESC(FieldDescriptorProto_proto3_optional)(field_proto);
+  f->msgdef = m;
+  f->scope.oneof = NULL;
 
-#if defined(__GNUC__) && !defined(__clang__)
-#pragma GCC diagnostic pop
-#endif
+  f->has_json_name = UPB_DESC(FieldDescriptorProto_has_json_name)(field_proto);
+  if (f->has_json_name) {
+    const upb_StringView sv =
+        UPB_DESC(FieldDescriptorProto_json_name)(field_proto);
+    f->json_name = upb_strdup2(sv.data, sv.size, ctx->arena);
+  } else {
+    f->json_name = make_json_name(name.data, name.size, ctx->arena);
+  }
+  if (!f->json_name) _upb_DefBuilder_OomErr(ctx);
+
+  const bool has_type = UPB_DESC(FieldDescriptorProto_has_type)(field_proto);
+  const bool has_type_name =
+      UPB_DESC(FieldDescriptorProto_has_type_name)(field_proto);
+
+  f->type_ = (int)UPB_DESC(FieldDescriptorProto_type)(field_proto);
+
+  if (has_type) {
+    switch (f->type_) {
+      case kUpb_FieldType_Message:
+      case kUpb_FieldType_Group:
+      case kUpb_FieldType_Enum:
+        if (!has_type_name) {
+          _upb_DefBuilder_Errf(ctx, "field of type %d requires type name (%s)",
+                               (int)f->type_, f->full_name);
+        }
+        break;
+      default:
+        if (has_type_name) {
+          _upb_DefBuilder_Errf(
+              ctx, "invalid type for field with type_name set (%s, %d)",
+              f->full_name, (int)f->type_);
+        }
+    }
+  } else if (has_type_name) {
+    f->type_ =
+        UPB_FIELD_TYPE_UNSPECIFIED;  // We'll assign this in resolve_fielddef()
+  }
+
+  if (f->type_ < kUpb_FieldType_Double || f->type_ > kUpb_FieldType_SInt64) {
+    _upb_DefBuilder_Errf(ctx, "invalid type for field %s (%d)", f->full_name,
+                         f->type_);
+  }
+
+  if (f->label_ < kUpb_Label_Optional || f->label_ > kUpb_Label_Repeated) {
+    _upb_DefBuilder_Errf(ctx, "invalid label for field %s (%d)", f->full_name,
+                         f->label_);
+  }
+
+  /* We can't resolve the subdef or (in the case of extensions) the containing
+   * message yet, because it may not have been defined yet.  We stash a pointer
+   * to the field_proto until later when we can properly resolve it. */
+  f->sub.unresolved = field_proto;
 
-#include "upb/port/undef.inc"
+  if (f->label_ == kUpb_Label_Required &&
+      upb_FileDef_Syntax(f->file) == kUpb_Syntax_Proto3) {
+    _upb_DefBuilder_Errf(ctx, "proto3 fields cannot be required (%s)",
+                         f->full_name);
+  }
 
-#endif  // UPB_MESSAGE_ACCESSORS_H_
+  if (UPB_DESC(FieldDescriptorProto_has_oneof_index)(field_proto)) {
+    uint32_t oneof_index =
+        UPB_DESC(FieldDescriptorProto_oneof_index)(field_proto);
+
+    if (upb_FieldDef_Label(f) != kUpb_Label_Optional) {
+      _upb_DefBuilder_Errf(ctx, "fields in oneof must have OPTIONAL label (%s)",
+                           f->full_name);
+    }
+
+    if (!m) {
+      _upb_DefBuilder_Errf(ctx, "oneof field (%s) has no containing msg",
+                           f->full_name);
+    }
+
+    if (oneof_index >= upb_MessageDef_OneofCount(m)) {
+      _upb_DefBuilder_Errf(ctx, "oneof_index out of range (%s)", f->full_name);
+    }
+
+    upb_OneofDef* oneof = (upb_OneofDef*)upb_MessageDef_Oneof(m, oneof_index);
+    f->scope.oneof = oneof;
+
+    _upb_OneofDef_Insert(ctx, oneof, f, name.data, name.size);
+  }
+
+  UPB_DEF_SET_OPTIONS(f->opts, FieldDescriptorProto, FieldOptions, field_proto);
+
+  if (UPB_DESC(FieldOptions_has_packed)(f->opts)) {
+    f->is_packed = UPB_DESC(FieldOptions_packed)(f->opts);
+  } else {
+    // Repeated fields default to packed for proto3 only.
+    f->is_packed = upb_FieldDef_IsPrimitive(f) &&
+                   f->label_ == kUpb_Label_Repeated &&
+                   upb_FileDef_Syntax(f->file) == kUpb_Syntax_Proto3;
+  }
+
+  f->has_presence =
+      (!upb_FieldDef_IsRepeated(f)) &&
+      (upb_FieldDef_IsSubMessage(f) || upb_FieldDef_ContainingOneof(f) ||
+       (upb_FileDef_Syntax(f->file) == kUpb_Syntax_Proto2));
+}
+
+static void _upb_FieldDef_CreateExt(upb_DefBuilder* ctx, const char* prefix,
+                                    const UPB_DESC(FieldDescriptorProto) *
+                                        field_proto,
+                                    upb_MessageDef* m, upb_FieldDef* f) {
+  f->is_extension = true;
+  _upb_FieldDef_Create(ctx, prefix, field_proto, m, f);
+
+  if (UPB_DESC(FieldDescriptorProto_has_oneof_index)(field_proto)) {
+    _upb_DefBuilder_Errf(ctx, "oneof_index provided for extension field (%s)",
+                         f->full_name);
+  }
+
+  f->scope.extension_scope = m;
+  _upb_DefBuilder_Add(ctx, f->full_name, _upb_DefType_Pack(f, UPB_DEFTYPE_EXT));
+  f->layout_index = ctx->ext_count++;
+
+  if (ctx->layout) {
+    UPB_ASSERT(_upb_FieldDef_ExtensionMiniTable(f)->field.number == f->number_);
+  }
+}
+
+static void _upb_FieldDef_CreateNotExt(upb_DefBuilder* ctx, const char* prefix,
+                                       const UPB_DESC(FieldDescriptorProto) *
+                                           field_proto,
+                                       upb_MessageDef* m, upb_FieldDef* f) {
+  f->is_extension = false;
+  _upb_FieldDef_Create(ctx, prefix, field_proto, m, f);
+
+  if (!UPB_DESC(FieldDescriptorProto_has_oneof_index)(field_proto)) {
+    if (f->is_proto3_optional) {
+      _upb_DefBuilder_Errf(
+          ctx,
+          "non-extension field (%s) with proto3_optional was not in a oneof",
+          f->full_name);
+    }
+  }
+
+  _upb_MessageDef_InsertField(ctx, m, f);
+}
+
+upb_FieldDef* _upb_Extensions_New(
+    upb_DefBuilder* ctx, int n,
+    const UPB_DESC(FieldDescriptorProto) * const* protos, const char* prefix,
+    upb_MessageDef* m) {
+  _upb_DefType_CheckPadding(sizeof(upb_FieldDef));
+  upb_FieldDef* defs =
+      (upb_FieldDef*)_upb_DefBuilder_Alloc(ctx, sizeof(upb_FieldDef) * n);
+
+  for (int i = 0; i < n; i++) {
+    upb_FieldDef* f = &defs[i];
+
+    _upb_FieldDef_CreateExt(ctx, prefix, protos[i], m, f);
+    f->index_ = i;
+  }
+
+  return defs;
+}
+
+upb_FieldDef* _upb_FieldDefs_New(
+    upb_DefBuilder* ctx, int n,
+    const UPB_DESC(FieldDescriptorProto) * const* protos, const char* prefix,
+    upb_MessageDef* m, bool* is_sorted) {
+  _upb_DefType_CheckPadding(sizeof(upb_FieldDef));
+  upb_FieldDef* defs =
+      (upb_FieldDef*)_upb_DefBuilder_Alloc(ctx, sizeof(upb_FieldDef) * n);
+
+  uint32_t previous = 0;
+  for (int i = 0; i < n; i++) {
+    upb_FieldDef* f = &defs[i];
+
+    _upb_FieldDef_CreateNotExt(ctx, prefix, protos[i], m, f);
+    f->index_ = i;
+    if (!ctx->layout) {
+      // Speculate that the def fields are sorted.  We will always sort the
+      // MiniTable fields, so if defs are sorted then indices will match.
+      //
+      // If this is incorrect, we will overwrite later.
+      f->layout_index = i;
+    }
+
+    const uint32_t current = f->number_;
+    if (previous > current) *is_sorted = false;
+    previous = current;
+  }
+
+  return defs;
+}
+
+static void resolve_subdef(upb_DefBuilder* ctx, const char* prefix,
+                           upb_FieldDef* f) {
+  const UPB_DESC(FieldDescriptorProto)* field_proto = f->sub.unresolved;
+  upb_StringView name = UPB_DESC(FieldDescriptorProto_type_name)(field_proto);
+  bool has_name = UPB_DESC(FieldDescriptorProto_has_type_name)(field_proto);
+  switch ((int)f->type_) {
+    case UPB_FIELD_TYPE_UNSPECIFIED: {
+      // Type was not specified and must be inferred.
+      UPB_ASSERT(has_name);
+      upb_deftype_t type;
+      const void* def =
+          _upb_DefBuilder_ResolveAny(ctx, f->full_name, prefix, name, &type);
+      switch (type) {
+        case UPB_DEFTYPE_ENUM:
+          f->sub.enumdef = def;
+          f->type_ = kUpb_FieldType_Enum;
+          break;
+        case UPB_DEFTYPE_MSG:
+          f->sub.msgdef = def;
+          f->type_ = kUpb_FieldType_Message;  // It appears there is no way of
+                                              // this being a group.
+          break;
+        default:
+          _upb_DefBuilder_Errf(ctx, "Couldn't resolve type name for field %s",
+                               f->full_name);
+      }
+    }
+    case kUpb_FieldType_Message:
+    case kUpb_FieldType_Group:
+      UPB_ASSERT(has_name);
+      f->sub.msgdef = _upb_DefBuilder_Resolve(ctx, f->full_name, prefix, name,
+                                              UPB_DEFTYPE_MSG);
+      break;
+    case kUpb_FieldType_Enum:
+      UPB_ASSERT(has_name);
+      f->sub.enumdef = _upb_DefBuilder_Resolve(ctx, f->full_name, prefix, name,
+                                               UPB_DEFTYPE_ENUM);
+      break;
+    default:
+      // No resolution necessary.
+      break;
+  }
+}
+
+static int _upb_FieldDef_Compare(const void* p1, const void* p2) {
+  const uint32_t v1 = (*(upb_FieldDef**)p1)->number_;
+  const uint32_t v2 = (*(upb_FieldDef**)p2)->number_;
+  return (v1 < v2) ? -1 : (v1 > v2);
+}
+
+// _upb_FieldDefs_Sorted() is mostly a pure function of its inputs, but has one
+// critical side effect that we depend on: it sets layout_index appropriately
+// for non-sorted lists of fields.
+const upb_FieldDef** _upb_FieldDefs_Sorted(const upb_FieldDef* f, int n,
+                                           upb_Arena* a) {
+  // TODO(salo): Replace this arena alloc with a persistent scratch buffer.
+  upb_FieldDef** out = (upb_FieldDef**)upb_Arena_Malloc(a, n * sizeof(void*));
+  if (!out) return NULL;
+
+  for (int i = 0; i < n; i++) {
+    out[i] = (upb_FieldDef*)&f[i];
+  }
+  qsort(out, n, sizeof(void*), _upb_FieldDef_Compare);
+
+  for (int i = 0; i < n; i++) {
+    out[i]->layout_index = i;
+  }
+  return (const upb_FieldDef**)out;
+}
+
+bool upb_FieldDef_MiniDescriptorEncode(const upb_FieldDef* f, upb_Arena* a,
+                                       upb_StringView* out) {
+  UPB_ASSERT(f->is_extension);
+
+  upb_DescState s;
+  _upb_DescState_Init(&s);
+
+  const int number = upb_FieldDef_Number(f);
+  const uint64_t modifiers = _upb_FieldDef_Modifiers(f);
+
+  if (!_upb_DescState_Grow(&s, a)) return false;
+  s.ptr = upb_MtDataEncoder_EncodeExtension(&s.e, s.ptr, f->type_, number,
+                                            modifiers);
+  *s.ptr = '\0';
+
+  out->data = s.buf;
+  out->size = s.ptr - s.buf;
+  return true;
+}
+
+static void resolve_extension(upb_DefBuilder* ctx, const char* prefix,
+                              upb_FieldDef* f,
+                              const UPB_DESC(FieldDescriptorProto) *
+                                  field_proto) {
+  if (!UPB_DESC(FieldDescriptorProto_has_extendee)(field_proto)) {
+    _upb_DefBuilder_Errf(ctx, "extension for field '%s' had no extendee",
+                         f->full_name);
+  }
+
+  upb_StringView name = UPB_DESC(FieldDescriptorProto_extendee)(field_proto);
+  const upb_MessageDef* m =
+      _upb_DefBuilder_Resolve(ctx, f->full_name, prefix, name, UPB_DEFTYPE_MSG);
+  f->msgdef = m;
+
+  if (!_upb_MessageDef_IsValidExtensionNumber(m, f->number_)) {
+    _upb_DefBuilder_Errf(
+        ctx,
+        "field number %u in extension %s has no extension range in message %s",
+        (unsigned)f->number_, f->full_name, upb_MessageDef_FullName(m));
+  }
+}
+
+void _upb_FieldDef_BuildMiniTableExtension(upb_DefBuilder* ctx,
+                                           const upb_FieldDef* f) {
+  const upb_MiniTableExtension* ext = _upb_FieldDef_ExtensionMiniTable(f);
+
+  if (ctx->layout) {
+    UPB_ASSERT(upb_FieldDef_Number(f) == ext->field.number);
+  } else {
+    upb_StringView desc;
+    if (!upb_FieldDef_MiniDescriptorEncode(f, ctx->tmp_arena, &desc)) {
+      _upb_DefBuilder_OomErr(ctx);
+    }
+
+    upb_MiniTableExtension* mut_ext = (upb_MiniTableExtension*)ext;
+    upb_MiniTableSub sub = {NULL};
+    if (upb_FieldDef_IsSubMessage(f)) {
+      sub.submsg = upb_MessageDef_MiniTable(f->sub.msgdef);
+    } else if (_upb_FieldDef_IsClosedEnum(f)) {
+      sub.subenum = _upb_EnumDef_MiniTable(f->sub.enumdef);
+    }
+    bool ok2 = upb_MiniTableExtension_Init(desc.data, desc.size, mut_ext,
+                                           upb_MessageDef_MiniTable(f->msgdef),
+                                           sub, ctx->status);
+    if (!ok2) _upb_DefBuilder_Errf(ctx, "Could not build extension mini table");
+  }
+
+  bool ok = _upb_DefPool_InsertExt(ctx->symtab, ext, f);
+  if (!ok) _upb_DefBuilder_OomErr(ctx);
+}
+
+static void resolve_default(upb_DefBuilder* ctx, upb_FieldDef* f,
+                            const UPB_DESC(FieldDescriptorProto) *
+                                field_proto) {
+  // Have to delay resolving of the default value until now because of the enum
+  // case, since enum defaults are specified with a label.
+  if (UPB_DESC(FieldDescriptorProto_has_default_value)(field_proto)) {
+    upb_StringView defaultval =
+        UPB_DESC(FieldDescriptorProto_default_value)(field_proto);
+
+    if (upb_FileDef_Syntax(f->file) == kUpb_Syntax_Proto3) {
+      _upb_DefBuilder_Errf(ctx,
+                           "proto3 fields cannot have explicit defaults (%s)",
+                           f->full_name);
+    }
+
+    if (upb_FieldDef_IsSubMessage(f)) {
+      _upb_DefBuilder_Errf(ctx,
+                           "message fields cannot have explicit defaults (%s)",
+                           f->full_name);
+    }
+
+    parse_default(ctx, defaultval.data, defaultval.size, f);
+    f->has_default = true;
+  } else {
+    set_default_default(ctx, f);
+    f->has_default = false;
+  }
+}
+
+void _upb_FieldDef_Resolve(upb_DefBuilder* ctx, const char* prefix,
+                           upb_FieldDef* f) {
+  // We have to stash this away since resolve_subdef() may overwrite it.
+  const UPB_DESC(FieldDescriptorProto)* field_proto = f->sub.unresolved;
+
+  resolve_subdef(ctx, prefix, f);
+  resolve_default(ctx, f, field_proto);
+
+  if (f->is_extension) {
+    resolve_extension(ctx, prefix, f, field_proto);
+  }
+}
```

### Comparing `protobuf-4.22.3/upb/message/extension_internal.h` & `protobuf-4.23.0rc2/upb/message/extension_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/message/internal.h` & `protobuf-4.23.0rc2/upb/message/internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/message/message.c` & `protobuf-4.23.0rc2/upb/message/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/message/message.h` & `protobuf-4.23.0rc2/upb/message/message.h`

 * *Files 8% similar despite different names*

```diff
@@ -21,19 +21,17 @@
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-// Public APIs for message operations that do not require descriptors.
-// These functions can be used even in build that does not want to depend on
-// reflection or descriptors.
+// Public APIs for message operations that do not depend on the schema.
 //
-// Descriptor-based reflection functionality lives in reflection.h.
+// MiniTable-based accessors live in accessors.h.
 
 #ifndef UPB_MESSAGE_MESSAGE_H_
 #define UPB_MESSAGE_MESSAGE_H_
 
 #include "upb/mem/arena.h"
 #include "upb/mini_table/types.h"
```

### Comparing `protobuf-4.22.3/upb/mini_table/common.c` & `protobuf-4.23.0rc2/upb/mini_table/common.c`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,15 @@
   }
 
   // Slow case: binary search
   int lo = t->dense_below;
   int hi = t->field_count - 1;
   while (lo <= hi) {
     int mid = (lo + hi) / 2;
-    int num = t->fields[mid].number;
+    uint32_t num = t->fields[mid].number;
     if (num < number) {
       lo = mid + 1;
       continue;
     }
     if (num > number) {
       hi = mid - 1;
       continue;
@@ -80,23 +80,23 @@
     return &t->fields[mid];
   }
   return NULL;
 }
 
 upb_FieldType upb_MiniTableField_Type(const upb_MiniTableField* field) {
   if (field->mode & kUpb_LabelFlags_IsAlternate) {
-    if (field->descriptortype == kUpb_FieldType_Int32) {
+    if (field->UPB_PRIVATE(descriptortype) == kUpb_FieldType_Int32) {
       return kUpb_FieldType_Enum;
-    } else if (field->descriptortype == kUpb_FieldType_Bytes) {
+    } else if (field->UPB_PRIVATE(descriptortype) == kUpb_FieldType_Bytes) {
       return kUpb_FieldType_String;
     } else {
       UPB_ASSERT(false);
     }
   }
-  return field->descriptortype;
+  return field->UPB_PRIVATE(descriptortype);
 }
 
 static bool upb_MiniTable_Is_Oneof(const upb_MiniTableField* f) {
   return f->presence < 0;
 }
 
 const upb_MiniTableField* upb_MiniTable_GetOneof(const upb_MiniTable* m,
```

### Comparing `protobuf-4.22.3/upb/mini_table/common.h` & `protobuf-4.23.0rc2/upb/mini_table/common.h`

 * *Files 16% similar despite different names*

```diff
@@ -52,18 +52,23 @@
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 UPB_API const upb_MiniTableField* upb_MiniTable_FindFieldByNumber(
     const upb_MiniTable* table, uint32_t number);
 
+UPB_API_INLINE const upb_MiniTableField* upb_MiniTable_GetFieldByIndex(
+    const upb_MiniTable* t, uint32_t index) {
+  return &t->fields[index];
+}
+
 UPB_API upb_FieldType upb_MiniTableField_Type(const upb_MiniTableField* field);
 
 UPB_API_INLINE upb_CType upb_MiniTableField_CType(const upb_MiniTableField* f) {
-  switch (f->descriptortype) {
+  switch (f->UPB_PRIVATE(descriptortype)) {
     case kUpb_FieldType_Double:
       return kUpb_CType_Double;
     case kUpb_FieldType_Float:
       return kUpb_CType_Float;
     case kUpb_FieldType_Int64:
     case kUpb_FieldType_SInt64:
     case kUpb_FieldType_SFixed64:
@@ -94,31 +99,49 @@
 }
 
 UPB_API_INLINE bool upb_MiniTableField_IsExtension(
     const upb_MiniTableField* field) {
   return field->mode & kUpb_LabelFlags_IsExtension;
 }
 
+UPB_API_INLINE bool upb_MiniTableField_IsClosedEnum(
+    const upb_MiniTableField* field) {
+  return field->UPB_PRIVATE(descriptortype) == kUpb_FieldType_Enum;
+}
+
 UPB_API_INLINE bool upb_MiniTableField_HasPresence(
     const upb_MiniTableField* field) {
   if (upb_MiniTableField_IsExtension(field)) {
     return !upb_IsRepeatedOrMap(field);
   } else {
     return field->presence != 0;
   }
 }
 
+// Returns the MiniTable for this message field.  If the field is unlinked,
+// returns NULL.
 UPB_API_INLINE const upb_MiniTable* upb_MiniTable_GetSubMessageTable(
     const upb_MiniTable* mini_table, const upb_MiniTableField* field) {
-  return mini_table->subs[field->submsg_index].submsg;
+  UPB_ASSERT(upb_MiniTableField_CType(field) == kUpb_CType_Message);
+  return mini_table->subs[field->UPB_PRIVATE(submsg_index)].submsg;
 }
 
+// Returns the MiniTableEnum for this enum field.  If the field is unlinked,
+// returns NULL.
 UPB_API_INLINE const upb_MiniTableEnum* upb_MiniTable_GetSubEnumTable(
     const upb_MiniTable* mini_table, const upb_MiniTableField* field) {
-  return mini_table->subs[field->submsg_index].subenum;
+  UPB_ASSERT(upb_MiniTableField_CType(field) == kUpb_CType_Enum);
+  return mini_table->subs[field->UPB_PRIVATE(submsg_index)].subenum;
+}
+
+// Returns true if this MiniTable field is linked to a MiniTable for the
+// sub-message.
+UPB_API_INLINE bool upb_MiniTable_MessageFieldIsLinked(
+    const upb_MiniTable* mini_table, const upb_MiniTableField* field) {
+  return upb_MiniTable_GetSubMessageTable(mini_table, field) != NULL;
 }
 
 // If this field is in a oneof, returns the first field in the oneof.
 //
 // Otherwise returns NULL.
 //
 // Usage:
@@ -126,18 +149,19 @@
 //   do {
 //       ..
 //   } while (upb_MiniTable_NextOneofField(m, &field);
 //
 const upb_MiniTableField* upb_MiniTable_GetOneof(const upb_MiniTable* m,
                                                  const upb_MiniTableField* f);
 
-// Returns the next field in the oneof. If this is the last field in the
-// oneof, returns NULL. The ordering of fields in the oneof is not
+// Iterates to the next field in the oneof. If this is the last field in the
+// oneof, returns false. The ordering of fields in the oneof is not
 // guaranteed.
-// REQUIRES: |iter| is and iterator.
+// REQUIRES: |f| is the field initialized by upb_MiniTable_GetOneof and updated
+//           by prior upb_MiniTable_NextOneofField calls.
 bool upb_MiniTable_NextOneofField(const upb_MiniTable* m,
                                   const upb_MiniTableField** f);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
```

### Comparing `protobuf-4.22.3/upb/mini_table/common_internal.h` & `protobuf-4.23.0rc2/upb/mini_table/common_internal.h`

 * *Files 6% similar despite different names*

```diff
@@ -98,25 +98,14 @@
 
 UPB_INLINE char _upb_FromBase92(uint8_t ch) {
   extern const int8_t _kUpb_FromBase92[];
   if (' ' > ch || ch > '~') return -1;
   return _kUpb_FromBase92[ch - ' '];
 }
 
-UPB_INLINE bool _upb_FieldType_IsPackable(upb_FieldType type) {
-  // clang-format off
-  const unsigned kUnpackableTypes =
-      (1 << kUpb_FieldType_String) |
-      (1 << kUpb_FieldType_Bytes) |
-      (1 << kUpb_FieldType_Message) |
-      (1 << kUpb_FieldType_Group);
-  // clang-format on
-  return (1 << type) & ~kUnpackableTypes;
-}
-
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
 
 #endif /* UPB_MINI_TABLE_COMMON_INTERNAL_H_ */
```

### Comparing `protobuf-4.22.3/upb/mini_table/decode.c` & `protobuf-4.23.0rc2/upb/mini_table/decode.c`

 * *Files 8% similar despite different names*

```diff
@@ -134,51 +134,51 @@
     shift += bits_per_char;
     if (shift >= 32) upb_MtDecoder_ErrorFormat(d, "Overlong varint");
   }
 }
 
 static bool upb_MiniTable_HasSub(upb_MiniTableField* field,
                                  uint64_t msg_modifiers) {
-  switch (field->descriptortype) {
+  switch (field->UPB_PRIVATE(descriptortype)) {
     case kUpb_FieldType_Message:
     case kUpb_FieldType_Group:
     case kUpb_FieldType_Enum:
       return true;
     case kUpb_FieldType_String:
       if (!(msg_modifiers & kUpb_MessageModifier_ValidateUtf8)) {
-        field->descriptortype = kUpb_FieldType_Bytes;
+        field->UPB_PRIVATE(descriptortype) = kUpb_FieldType_Bytes;
         field->mode |= kUpb_LabelFlags_IsAlternate;
       }
       return false;
     default:
       return false;
   }
 }
 
 static bool upb_MtDecoder_FieldIsPackable(upb_MiniTableField* field) {
   return (field->mode & kUpb_FieldMode_Array) &&
-         _upb_FieldType_IsPackable(field->descriptortype);
+         upb_FieldType_IsPackable(field->UPB_PRIVATE(descriptortype));
 }
 
 static void upb_MiniTable_SetTypeAndSub(upb_MiniTableField* field,
                                         upb_FieldType type, uint32_t* sub_count,
                                         uint64_t msg_modifiers,
                                         bool is_proto3_enum) {
-  field->descriptortype = type;
+  field->UPB_PRIVATE(descriptortype) = type;
 
   if (is_proto3_enum) {
-    UPB_ASSERT(field->descriptortype == kUpb_FieldType_Enum);
-    field->descriptortype = kUpb_FieldType_Int32;
+    UPB_ASSERT(field->UPB_PRIVATE(descriptortype) == kUpb_FieldType_Enum);
+    field->UPB_PRIVATE(descriptortype) = kUpb_FieldType_Int32;
     field->mode |= kUpb_LabelFlags_IsAlternate;
   }
 
   if (upb_MiniTable_HasSub(field, msg_modifiers)) {
-    field->submsg_index = sub_count ? (*sub_count)++ : 0;
+    field->UPB_PRIVATE(submsg_index) = sub_count ? (*sub_count)++ : 0;
   } else {
-    field->submsg_index = kUpb_NoSub;
+    field->UPB_PRIVATE(submsg_index) = kUpb_NoSub;
   }
 
   if (upb_MtDecoder_FieldIsPackable(field) &&
       (msg_modifiers & kUpb_MessageModifier_DefaultIsPacked)) {
     field->mode |= kUpb_LabelFlags_IsPacked;
   }
 }
@@ -240,22 +240,22 @@
     field->mode |= pointer_rep << kUpb_FieldRep_Shift;
     field->offset = kNoPresence;
   } else {
     field->mode = kUpb_FieldMode_Scalar;
     field->offset = kHasbitPresence;
     if (type == kUpb_EncodedType_Group || type == kUpb_EncodedType_Message) {
       field->mode |= pointer_rep << kUpb_FieldRep_Shift;
-    } else if (type >= sizeof(kUpb_EncodedToFieldRep)) {
+    } else if ((unsigned long)type >= sizeof(kUpb_EncodedToFieldRep)) {
       upb_MtDecoder_ErrorFormat(d, "Invalid field type: %d", (int)type);
       UPB_UNREACHABLE();
     } else {
       field->mode |= kUpb_EncodedToFieldRep[type] << kUpb_FieldRep_Shift;
     }
   }
-  if (type >= sizeof(kUpb_EncodedToType)) {
+  if ((unsigned long)type >= sizeof(kUpb_EncodedToType)) {
     upb_MtDecoder_ErrorFormat(d, "Invalid field type: %d", (int)type);
     UPB_UNREACHABLE();
   }
   upb_MiniTable_SetTypeAndSub(field, kUpb_EncodedToType[type], sub_count,
                               msg_modifiers, type == kUpb_EncodedType_OpenEnum);
 }
 
@@ -663,15 +663,15 @@
   // On 32-bit we could potentially make this smaller, but there is no
   // compelling reason to optimize this right now.
   d->table->size = UPB_ALIGN_UP(d->table->size, 8);
 }
 
 static void upb_MtDecoder_ValidateEntryField(upb_MtDecoder* d,
                                              const upb_MiniTableField* f,
-                                             int expected_num) {
+                                             uint32_t expected_num) {
   const char* name = expected_num == 1 ? "key" : "val";
   if (f->number != expected_num) {
     upb_MtDecoder_ErrorFormat(d,
                               "map %s did not have expected number (%d vs %d)",
                               name, expected_num, (int)f->number);
   }
 
@@ -687,15 +687,15 @@
                    (1 << kUpb_FieldType_Bytes) | (1 << kUpb_FieldType_Enum);
   } else {
     not_ok_types = 1 << kUpb_FieldType_Group;
   }
 
   if ((1 << upb_MiniTableField_Type(f)) & not_ok_types) {
     upb_MtDecoder_ErrorFormat(d, "map %s cannot have type %d", name,
-                              (int)f->descriptortype);
+                              (int)f->UPB_PRIVATE(descriptortype));
   }
 }
 
 static void upb_MtDecoder_ParseMap(upb_MtDecoder* d, const char* data,
                                    size_t len) {
   upb_MtDecoder_ParseMessage(d, data, len);
   upb_MtDecoder_AssignHasbits(d->table);
@@ -740,75 +740,90 @@
   ret->field_count = 0;
   ret->ext = kUpb_ExtMode_IsMessageSet;
   ret->dense_below = 0;
   ret->table_mask = -1;
   ret->required_count = 0;
 }
 
-upb_MiniTable* upb_MiniTable_BuildWithBuf(const char* data, size_t len,
-                                          upb_MiniTablePlatform platform,
-                                          upb_Arena* arena, void** buf,
-                                          size_t* buf_size,
-                                          upb_Status* status) {
-  upb_MtDecoder decoder = {
-      .platform = platform,
-      .vec =
-          {
-              .data = *buf,
-              .capacity = *buf_size / sizeof(*decoder.vec.data),
-              .size = 0,
-          },
-      .arena = arena,
-      .status = status,
-      .table = upb_Arena_Malloc(arena, sizeof(*decoder.table)),
-  };
-
-  if (UPB_SETJMP(decoder.err)) {
-    decoder.table = NULL;
-    goto done;
-  }
-
-  upb_MtDecoder_CheckOutOfMemory(&decoder, decoder.table);
-
-  decoder.table->size = 0;
-  decoder.table->field_count = 0;
-  decoder.table->ext = kUpb_ExtMode_NonExtendable;
-  decoder.table->dense_below = 0;
-  decoder.table->table_mask = -1;
-  decoder.table->required_count = 0;
+static upb_MiniTable* upb_MtDecoder_DoBuildMiniTableWithBuf(
+    upb_MtDecoder* decoder, const char* data, size_t len, void** buf,
+    size_t* buf_size) {
+  upb_MtDecoder_CheckOutOfMemory(decoder, decoder->table);
+
+  decoder->table->size = 0;
+  decoder->table->field_count = 0;
+  decoder->table->ext = kUpb_ExtMode_NonExtendable;
+  decoder->table->dense_below = 0;
+  decoder->table->table_mask = -1;
+  decoder->table->required_count = 0;
 
   // Strip off and verify the version tag.
   if (!len--) goto done;
   const char vers = *data++;
 
   switch (vers) {
     case kUpb_EncodedVersion_MapV1:
-      upb_MtDecoder_ParseMap(&decoder, data, len);
+      upb_MtDecoder_ParseMap(decoder, data, len);
       break;
 
     case kUpb_EncodedVersion_MessageV1:
-      upb_MtDecoder_ParseMessage(&decoder, data, len);
-      upb_MtDecoder_AssignHasbits(decoder.table);
-      upb_MtDecoder_SortLayoutItems(&decoder);
-      upb_MtDecoder_AssignOffsets(&decoder);
+      upb_MtDecoder_ParseMessage(decoder, data, len);
+      upb_MtDecoder_AssignHasbits(decoder->table);
+      upb_MtDecoder_SortLayoutItems(decoder);
+      upb_MtDecoder_AssignOffsets(decoder);
       break;
 
     case kUpb_EncodedVersion_MessageSetV1:
-      upb_MtDecoder_ParseMessageSet(&decoder, data, len);
+      upb_MtDecoder_ParseMessageSet(decoder, data, len);
       break;
 
     default:
-      upb_MtDecoder_ErrorFormat(&decoder, "Invalid message version: %c", vers);
+      upb_MtDecoder_ErrorFormat(decoder, "Invalid message version: %c", vers);
       UPB_UNREACHABLE();
   }
 
 done:
-  *buf = decoder.vec.data;
-  *buf_size = decoder.vec.capacity * sizeof(*decoder.vec.data);
-  return decoder.table;
+  *buf = decoder->vec.data;
+  *buf_size = decoder->vec.capacity * sizeof(*decoder->vec.data);
+  return decoder->table;
+}
+
+static upb_MiniTable* upb_MtDecoder_BuildMiniTableWithBuf(
+    upb_MtDecoder* const decoder, const char* const data, const size_t len,
+    void** const buf, size_t* const buf_size) {
+  if (UPB_SETJMP(decoder->err) != 0) {
+    *buf = decoder->vec.data;
+    *buf_size = decoder->vec.capacity * sizeof(*decoder->vec.data);
+    return NULL;
+  }
+
+  return upb_MtDecoder_DoBuildMiniTableWithBuf(decoder, data, len, buf,
+                                               buf_size);
+}
+
+upb_MiniTable* upb_MiniTable_BuildWithBuf(const char* data, size_t len,
+                                          upb_MiniTablePlatform platform,
+                                          upb_Arena* arena, void** buf,
+                                          size_t* buf_size,
+                                          upb_Status* status) {
+  upb_MtDecoder decoder = {
+      .platform = platform,
+      .vec =
+          {
+              .data = *buf,
+              .capacity = *buf_size / sizeof(*decoder.vec.data),
+              .size = 0,
+          },
+      .arena = arena,
+      .status = status,
+      .table = upb_Arena_Malloc(arena, sizeof(*decoder.table)),
+  };
+
+  return upb_MtDecoder_BuildMiniTableWithBuf(&decoder, data, len, buf,
+                                             buf_size);
 }
 
 static size_t upb_MiniTableEnum_Size(size_t count) {
   return sizeof(upb_MiniTableEnum) + count * sizeof(uint32_t);
 }
 
 static upb_MiniTableEnum* _upb_MiniTable_AddEnumDataMember(upb_MtDecoder* d,
@@ -839,102 +854,100 @@
       table = _upb_MiniTable_AddEnumDataMember(d, 0);
       table->mask_limit += 32;
     }
     table->data[val / 32] |= 1ULL << (val % 32);
   }
 }
 
-upb_MiniTableEnum* upb_MiniTableEnum_Build(const char* data, size_t len,
-                                           upb_Arena* arena,
-                                           upb_Status* status) {
-  upb_MtDecoder decoder = {
-      .enum_table = upb_Arena_Malloc(arena, upb_MiniTableEnum_Size(2)),
-      .enum_value_count = 0,
-      .enum_data_count = 0,
-      .enum_data_capacity = 1,
-      .status = status,
-      .end = UPB_PTRADD(data, len),
-      .arena = arena,
-  };
-
-  if (UPB_SETJMP(decoder.err)) return NULL;
-
+static upb_MiniTableEnum* upb_MtDecoder_DoBuildMiniTableEnum(
+    upb_MtDecoder* decoder, const char* data, size_t len) {
   // If the string is non-empty then it must begin with a version tag.
   if (len) {
     if (*data != kUpb_EncodedVersion_EnumV1) {
-      upb_MtDecoder_ErrorFormat(&decoder, "Invalid enum version: %c", *data);
+      upb_MtDecoder_ErrorFormat(decoder, "Invalid enum version: %c", *data);
       UPB_UNREACHABLE();
     }
     data++;
     len--;
   }
 
-  upb_MtDecoder_CheckOutOfMemory(&decoder, decoder.enum_table);
+  upb_MtDecoder_CheckOutOfMemory(decoder, decoder->enum_table);
 
   // Guarantee at least 64 bits of mask without checking mask size.
-  decoder.enum_table->mask_limit = 64;
-  decoder.enum_table = _upb_MiniTable_AddEnumDataMember(&decoder, 0);
-  decoder.enum_table = _upb_MiniTable_AddEnumDataMember(&decoder, 0);
+  decoder->enum_table->mask_limit = 64;
+  decoder->enum_table = _upb_MiniTable_AddEnumDataMember(decoder, 0);
+  decoder->enum_table = _upb_MiniTable_AddEnumDataMember(decoder, 0);
 
-  decoder.enum_table->value_count = 0;
+  decoder->enum_table->value_count = 0;
 
   const char* ptr = data;
   uint32_t base = 0;
 
-  while (ptr < decoder.end) {
+  while (ptr < decoder->end) {
     char ch = *ptr++;
     if (ch <= kUpb_EncodedValue_MaxEnumMask) {
       uint32_t mask = _upb_FromBase92(ch);
       for (int i = 0; i < 5; i++, base++, mask >>= 1) {
-        if (mask & 1) upb_MiniTableEnum_BuildValue(&decoder, base);
+        if (mask & 1) upb_MiniTableEnum_BuildValue(decoder, base);
       }
     } else if (kUpb_EncodedValue_MinSkip <= ch &&
                ch <= kUpb_EncodedValue_MaxSkip) {
       uint32_t skip;
-      ptr = upb_MiniTable_DecodeBase92Varint(&decoder, ptr, ch,
+      ptr = upb_MiniTable_DecodeBase92Varint(decoder, ptr, ch,
                                              kUpb_EncodedValue_MinSkip,
                                              kUpb_EncodedValue_MaxSkip, &skip);
       base += skip;
     } else {
-      upb_MtDecoder_ErrorFormat(&decoder, "Unexpected character: %c", ch);
+      upb_MtDecoder_ErrorFormat(decoder, "Unexpected character: %c", ch);
       return NULL;
     }
   }
 
-  return decoder.enum_table;
+  return decoder->enum_table;
 }
 
-const char* _upb_MiniTableExtension_Build(const char* data, size_t len,
-                                          upb_MiniTableExtension* ext,
-                                          const upb_MiniTable* extendee,
-                                          upb_MiniTableSub sub,
-                                          upb_MiniTablePlatform platform,
-                                          upb_Status* status) {
+static upb_MiniTableEnum* upb_MtDecoder_BuildMiniTableEnum(
+    upb_MtDecoder* const decoder, const char* const data, size_t const len) {
+  if (UPB_SETJMP(decoder->err) != 0) return NULL;
+  return upb_MtDecoder_DoBuildMiniTableEnum(decoder, data, len);
+}
+
+upb_MiniTableEnum* upb_MiniTableEnum_Build(const char* data, size_t len,
+                                           upb_Arena* arena,
+                                           upb_Status* status) {
   upb_MtDecoder decoder = {
-      .arena = NULL,
+      .enum_table = upb_Arena_Malloc(arena, upb_MiniTableEnum_Size(2)),
+      .enum_value_count = 0,
+      .enum_data_count = 0,
+      .enum_data_capacity = 1,
       .status = status,
-      .table = NULL,
-      .platform = platform,
+      .end = UPB_PTRADD(data, len),
+      .arena = arena,
   };
 
-  if (UPB_SETJMP(decoder.err)) return NULL;
+  return upb_MtDecoder_BuildMiniTableEnum(&decoder, data, len);
+}
 
+static const char* upb_MtDecoder_DoBuildMiniTableExtension(
+    upb_MtDecoder* decoder, const char* data, size_t len,
+    upb_MiniTableExtension* ext, const upb_MiniTable* extendee,
+    upb_MiniTableSub sub) {
   // If the string is non-empty then it must begin with a version tag.
   if (len) {
     if (*data != kUpb_EncodedVersion_ExtensionV1) {
-      upb_MtDecoder_ErrorFormat(&decoder, "Invalid ext version: %c", *data);
+      upb_MtDecoder_ErrorFormat(decoder, "Invalid ext version: %c", *data);
       UPB_UNREACHABLE();
     }
     data++;
     len--;
   }
 
   uint16_t count = 0;
   const char* ret =
-      upb_MtDecoder_Parse(&decoder, data, len, ext, sizeof(*ext), &count, NULL);
+      upb_MtDecoder_Parse(decoder, data, len, ext, sizeof(*ext), &count, NULL);
   if (!ret || count != 1) return NULL;
 
   upb_MiniTableField* f = &ext->field;
 
   f->mode |= kUpb_LabelFlags_IsExtension;
   f->offset = 0;
   f->presence = 0;
@@ -949,14 +962,55 @@
 
   ext->extendee = extendee;
   ext->sub = sub;
 
   return ret;
 }
 
+static const char* upb_MtDecoder_BuildMiniTableExtension(
+    upb_MtDecoder* const decoder, const char* const data, const size_t len,
+    upb_MiniTableExtension* const ext, const upb_MiniTable* const extendee,
+    const upb_MiniTableSub sub) {
+  if (UPB_SETJMP(decoder->err) != 0) return NULL;
+  return upb_MtDecoder_DoBuildMiniTableExtension(decoder, data, len, ext,
+                                                 extendee, sub);
+}
+
+const char* _upb_MiniTableExtension_Init(const char* data, size_t len,
+                                         upb_MiniTableExtension* ext,
+                                         const upb_MiniTable* extendee,
+                                         upb_MiniTableSub sub,
+                                         upb_MiniTablePlatform platform,
+                                         upb_Status* status) {
+  upb_MtDecoder decoder = {
+      .arena = NULL,
+      .status = status,
+      .table = NULL,
+      .platform = platform,
+  };
+
+  return upb_MtDecoder_BuildMiniTableExtension(&decoder, data, len, ext,
+                                               extendee, sub);
+}
+
+upb_MiniTableExtension* _upb_MiniTableExtension_Build(
+    const char* data, size_t len, const upb_MiniTable* extendee,
+    upb_MiniTableSub sub, upb_MiniTablePlatform platform, upb_Arena* arena,
+    upb_Status* status) {
+  upb_MiniTableExtension* ext =
+      upb_Arena_Malloc(arena, sizeof(upb_MiniTableExtension));
+  if (UPB_UNLIKELY(!ext)) return NULL;
+
+  const char* ptr = _upb_MiniTableExtension_Init(data, len, ext, extendee, sub,
+                                                 platform, status);
+  if (UPB_UNLIKELY(!ptr)) return NULL;
+
+  return ext;
+}
+
 upb_MiniTable* _upb_MiniTable_Build(const char* data, size_t len,
                                     upb_MiniTablePlatform platform,
                                     upb_Arena* arena, upb_Status* status) {
   void* buf = NULL;
   size_t size = 0;
   upb_MiniTable* ret = upb_MiniTable_BuildWithBuf(data, len, platform, arena,
                                                   &buf, &size, status);
@@ -970,15 +1024,15 @@
   UPB_ASSERT((uintptr_t)table->fields <= (uintptr_t)field &&
              (uintptr_t)field <
                  (uintptr_t)(table->fields + table->field_count));
   UPB_ASSERT(sub);
 
   const bool sub_is_map = sub->ext & kUpb_ExtMode_IsMapEntry;
 
-  switch (field->descriptortype) {
+  switch (field->UPB_PRIVATE(descriptortype)) {
     case kUpb_FieldType_Message:
       if (sub_is_map) {
         const bool table_is_map = table->ext & kUpb_ExtMode_IsMapEntry;
         if (UPB_UNLIKELY(table_is_map)) return false;
 
         field->mode = (field->mode & ~kUpb_FieldMode_Mask) | kUpb_FieldMode_Map;
       }
@@ -988,23 +1042,86 @@
       if (UPB_UNLIKELY(sub_is_map)) return false;
       break;
 
     default:
       return false;
   }
 
-  upb_MiniTableSub* table_sub = (void*)&table->subs[field->submsg_index];
+  upb_MiniTableSub* table_sub =
+      (void*)&table->subs[field->UPB_PRIVATE(submsg_index)];
   table_sub->submsg = sub;
   return true;
 }
 
 bool upb_MiniTable_SetSubEnum(upb_MiniTable* table, upb_MiniTableField* field,
                               const upb_MiniTableEnum* sub) {
   UPB_ASSERT((uintptr_t)table->fields <= (uintptr_t)field &&
              (uintptr_t)field <
                  (uintptr_t)(table->fields + table->field_count));
   UPB_ASSERT(sub);
 
-  upb_MiniTableSub* table_sub = (void*)&table->subs[field->submsg_index];
+  upb_MiniTableSub* table_sub =
+      (void*)&table->subs[field->UPB_PRIVATE(submsg_index)];
   table_sub->subenum = sub;
   return true;
 }
+
+uint32_t upb_MiniTable_GetSubList(const upb_MiniTable* mt,
+                                  const upb_MiniTableField** subs) {
+  uint32_t msg_count = 0;
+  uint32_t enum_count = 0;
+
+  for (int i = 0; i < mt->field_count; i++) {
+    const upb_MiniTableField* f = &mt->fields[i];
+    if (upb_MiniTableField_CType(f) == kUpb_CType_Message) {
+      *subs = f;
+      ++subs;
+      msg_count++;
+    }
+  }
+
+  for (int i = 0; i < mt->field_count; i++) {
+    const upb_MiniTableField* f = &mt->fields[i];
+    if (upb_MiniTableField_CType(f) == kUpb_CType_Enum) {
+      *subs = f;
+      ++subs;
+      enum_count++;
+    }
+  }
+
+  return (msg_count << 16) | enum_count;
+}
+
+// The list of sub_tables and sub_enums must exactly match the number and order
+// of sub-message fields and sub-enum fields given by upb_MiniTable_GetSubList()
+// above.
+bool upb_MiniTable_Link(upb_MiniTable* mt, const upb_MiniTable** sub_tables,
+                        size_t sub_table_count,
+                        const upb_MiniTableEnum** sub_enums,
+                        size_t sub_enum_count) {
+  uint32_t msg_count = 0;
+  uint32_t enum_count = 0;
+
+  for (int i = 0; i < mt->field_count; i++) {
+    upb_MiniTableField* f = (upb_MiniTableField*)&mt->fields[i];
+    if (upb_MiniTableField_CType(f) == kUpb_CType_Message) {
+      const upb_MiniTable* sub = sub_tables[msg_count++];
+      if (msg_count > sub_table_count) return false;
+      if (sub != NULL) {
+        if (!upb_MiniTable_SetSubMessage(mt, f, sub)) return false;
+      }
+    }
+  }
+
+  for (int i = 0; i < mt->field_count; i++) {
+    upb_MiniTableField* f = (upb_MiniTableField*)&mt->fields[i];
+    if (upb_MiniTableField_CType(f) == kUpb_CType_Enum) {
+      const upb_MiniTableEnum* sub = sub_enums[enum_count++];
+      if (enum_count > sub_enum_count) return false;
+      if (sub != NULL) {
+        if (!upb_MiniTable_SetSubEnum(mt, f, sub)) return false;
+      }
+    }
+  }
+
+  return true;
+}
```

### Comparing `protobuf-4.22.3/upb/mini_table/encode.c` & `protobuf-4.23.0rc2/upb/mini_table/encode.c`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
     encoded_type = kUpb_EncodedType_ClosedEnum;
   }
   if (field_mod & kUpb_FieldModifier_IsRepeated) {
     // Repeated fields shift the type number up (unlike other modifiers which
     // are bit flags).
     encoded_type += kUpb_EncodedType_RepeatedBase;
 
-    if (_upb_FieldType_IsPackable(type)) {
+    if (upb_FieldType_IsPackable(type)) {
       bool field_is_packed = field_mod & kUpb_FieldModifier_IsPacked;
       bool default_is_packed = in->state.msg_state.msg_modifiers &
                                kUpb_MessageModifier_DefaultIsPacked;
       if (field_is_packed != default_is_packed) {
         encoded_modifiers |= kUpb_EncodedFieldModifier_FlipPacked;
       }
     }
```

### Comparing `protobuf-4.22.3/upb/mini_table/encode_internal.h` & `protobuf-4.23.0rc2/upb/mini_table/encode_internal.h`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #ifndef UPB_MINI_TABLE_ENCODE_INTERNAL_H_
 #define UPB_MINI_TABLE_ENCODE_INTERNAL_H_
 
+#include "upb/base/descriptor_constants.h"
 #include "upb/mini_table/common.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
 // If the input buffer has at least this many bytes available, the encoder call
 // is guaranteed to succeed (as long as field number order is maintained).
```

### Comparing `protobuf-4.22.3/upb/mini_table/enum_internal.h` & `protobuf-4.23.0rc2/upb/mini_table/enum_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/mini_table/extension_internal.h` & `protobuf-4.23.0rc2/upb/mini_table/extension_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/mini_table/extension_registry.c` & `protobuf-4.23.0rc2/upb/mini_table/extension_registry.c`

 * *Files 8% similar despite different names*

```diff
@@ -49,38 +49,38 @@
   upb_ExtensionRegistry* r = upb_Arena_Malloc(arena, sizeof(*r));
   if (!r) return NULL;
   r->arena = arena;
   if (!upb_strtable_init(&r->exts, 8, arena)) return NULL;
   return r;
 }
 
+UPB_API bool upb_ExtensionRegistry_Add(upb_ExtensionRegistry* r,
+                                       const upb_MiniTableExtension* e) {
+  char buf[EXTREG_KEY_SIZE];
+  extreg_key(buf, e->extendee, e->field.number);
+  if (upb_strtable_lookup2(&r->exts, buf, EXTREG_KEY_SIZE, NULL)) return false;
+  return upb_strtable_insert(&r->exts, buf, EXTREG_KEY_SIZE,
+                             upb_value_constptr(e), r->arena);
+}
+
 bool upb_ExtensionRegistry_AddArray(upb_ExtensionRegistry* r,
                                     const upb_MiniTableExtension** e,
                                     size_t count) {
-  char buf[EXTREG_KEY_SIZE];
   const upb_MiniTableExtension** start = e;
   const upb_MiniTableExtension** end = UPB_PTRADD(e, count);
   for (; e < end; e++) {
-    const upb_MiniTableExtension* ext = *e;
-    extreg_key(buf, ext->extendee, ext->field.number);
-    upb_value v;
-    if (upb_strtable_lookup2(&r->exts, buf, EXTREG_KEY_SIZE, &v)) {
-      goto failure;
-    }
-    if (!upb_strtable_insert(&r->exts, buf, EXTREG_KEY_SIZE,
-                             upb_value_constptr(ext), r->arena)) {
-      goto failure;
-    }
+    if (!upb_ExtensionRegistry_Add(r, *e)) goto failure;
   }
   return true;
 
 failure:
   // Back out the entries previously added.
   for (end = e, e = start; e < end; e++) {
     const upb_MiniTableExtension* ext = *e;
+    char buf[EXTREG_KEY_SIZE];
     extreg_key(buf, ext->extendee, ext->field.number);
     upb_strtable_remove2(&r->exts, buf, EXTREG_KEY_SIZE, NULL);
   }
   return false;
 }
 
 const upb_MiniTableExtension* upb_ExtensionRegistry_Lookup(
```

### Comparing `protobuf-4.22.3/upb/mini_table/extension_registry.h` & `protobuf-4.23.0rc2/upb/mini_table/extension_registry.h`

 * *Files 4% similar despite different names*

```diff
@@ -74,26 +74,29 @@
 
 typedef struct upb_ExtensionRegistry upb_ExtensionRegistry;
 
 // Creates a upb_ExtensionRegistry in the given arena.
 // The arena must outlive any use of the extreg.
 UPB_API upb_ExtensionRegistry* upb_ExtensionRegistry_New(upb_Arena* arena);
 
+UPB_API bool upb_ExtensionRegistry_Add(upb_ExtensionRegistry* r,
+                                       const upb_MiniTableExtension* e);
+
 // Adds the given extension info for the array |e| of size |count| into the
 // registry. If there are any errors, the entire array is backed out.
 // The extensions must outlive the registry.
 // Possible errors include OOM or an extension number that already exists.
-// TODO: There is currently no way to determine the exact reason for failure.
+// TODO(salo): There is currently no way to know the exact reason for failure.
 bool upb_ExtensionRegistry_AddArray(upb_ExtensionRegistry* r,
                                     const upb_MiniTableExtension** e,
                                     size_t count);
 
 // Looks up the extension (if any) defined for message type |t| and field
 // number |num|. Returns the extension if found, otherwise NULL.
-const upb_MiniTableExtension* upb_ExtensionRegistry_Lookup(
+UPB_API const upb_MiniTableExtension* upb_ExtensionRegistry_Lookup(
     const upb_ExtensionRegistry* r, const upb_MiniTable* t, uint32_t num);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-4.22.3/upb/mini_table/field_internal.h` & `protobuf-4.23.0rc2/upb/mini_table/field_internal.h`

 * *Files 11% similar despite different names*

```diff
@@ -30,20 +30,26 @@
 
 #include "upb/base/descriptor_constants.h"
 #include "upb/mini_table/types.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
+// LINT.IfChange(mini_table_field_layout)
+
 struct upb_MiniTableField {
   uint32_t number;
   uint16_t offset;
   int16_t presence;       // If >0, hasbit_index.  If <0, ~oneof_index
-  uint16_t submsg_index;  // kUpb_NoSub if descriptortype != MESSAGE/GROUP/ENUM
-  uint8_t descriptortype;
+
+  // Indexes into `upb_MiniTable.subs`
+  // Will be set to `kUpb_NoSub` if `descriptortype` != MESSAGE/GROUP/ENUM
+  uint16_t UPB_PRIVATE(submsg_index);
+
+  uint8_t UPB_PRIVATE(descriptortype);
 
   // upb_FieldMode | upb_LabelFlags | (upb_FieldRep << kUpb_FieldRep_Shift)
   uint8_t mode;
 };
 
 #define kUpb_NoSub ((uint16_t)-1)
 
@@ -78,14 +84,16 @@
   kUpb_FieldRep_NativePointer =
       UPB_SIZE(kUpb_FieldRep_4Byte, kUpb_FieldRep_8Byte),
   kUpb_FieldRep_Max = kUpb_FieldRep_8Byte,
 } upb_FieldRep;
 
 #define kUpb_FieldRep_Shift 6
 
+// LINT.ThenChange(//depot/google3/third_party/upb/js/impl/upb_bits/mini_table_field.ts:mini_table_field_layout)
+
 UPB_INLINE upb_FieldRep
 _upb_MiniTableField_GetRep(const upb_MiniTableField* field) {
   return (upb_FieldRep)(field->mode >> kUpb_FieldRep_Shift);
 }
 
 #ifdef __cplusplus
 extern "C" {
@@ -111,16 +119,16 @@
 
 UPB_INLINE bool upb_IsRepeatedOrMap(const upb_MiniTableField* field) {
   // This works because upb_FieldMode has no value 3.
   return !(field->mode & kUpb_FieldMode_Scalar);
 }
 
 UPB_INLINE bool upb_IsSubMessage(const upb_MiniTableField* field) {
-  return field->descriptortype == kUpb_FieldType_Message ||
-         field->descriptortype == kUpb_FieldType_Group;
+  return field->UPB_PRIVATE(descriptortype) == kUpb_FieldType_Message ||
+         field->UPB_PRIVATE(descriptortype) == kUpb_FieldType_Group;
 }
 
 // LINT.IfChange(presence_logic)
 
 // Hasbit access ///////////////////////////////////////////////////////////////
 
 UPB_INLINE size_t _upb_hasbit_ofs(size_t idx) { return idx / 8; }
@@ -169,14 +177,15 @@
 
 UPB_INLINE uint32_t _upb_getoneofcase_field(const upb_Message* msg,
                                             const upb_MiniTableField* f) {
   return *_upb_oneofcase_field((upb_Message*)msg, f);
 }
 
 // LINT.ThenChange(GoogleInternalName2)
+// LINT.ThenChange(//depot/google3/third_party/upb/js/impl/upb_bits/presence.ts:presence_logic)
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
```

### Comparing `protobuf-4.22.3/upb/mini_table/file_internal.h` & `protobuf-4.23.0rc2/upb/mini_table/sub_internal.h`

 * *Files 10% similar despite different names*

```diff
@@ -21,27 +21,18 @@
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#ifndef UPB_MINI_TABLE_FILE_INTERNAL_H_
-#define UPB_MINI_TABLE_FILE_INTERNAL_H_
+#ifndef UPB_MINI_TABLE_SUB_INTERNAL_H_
+#define UPB_MINI_TABLE_SUB_INTERNAL_H_
 
 #include "upb/mini_table/types.h"
 
-// Must be last.
-#include "upb/port/def.inc"
-
-struct upb_MiniTableFile {
-  const upb_MiniTable** msgs;
-  const upb_MiniTableEnum** enums;
-  const upb_MiniTableExtension** exts;
-  int msg_count;
-  int enum_count;
-  int ext_count;
+union upb_MiniTableSub {
+  const upb_MiniTable* submsg;
+  const upb_MiniTableEnum* subenum;
 };
 
-#include "upb/port/undef.inc"
-
-#endif /* UPB_MINI_TABLE_FILE_INTERNAL_H_ */
+#endif /* UPB_MINI_TABLE_SUB_INTERNAL_H_ */
```

### Comparing `protobuf-4.22.3/upb/mini_table/message_internal.h` & `protobuf-4.23.0rc2/upb/mini_table/message_internal.h`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,16 @@
       3,  // MessageSet item (temporary only, see decode.c)
 
   // During table building we steal a bit to indicate that the message is a map
   // entry.  *Only* used during table building!
   kUpb_ExtMode_IsMapEntry = 4,
 } upb_ExtMode;
 
+// LINT.IfChange(mini_table_layout)
+
 // upb_MiniTable represents the memory layout of a given upb_MessageDef.
 // The members are public so generated code can initialize them,
 // but users MUST NOT directly read or write any of its members.
 struct upb_MiniTable {
   const upb_MiniTableSub* subs;
   const upb_MiniTableField* fields;
 
@@ -75,14 +77,16 @@
 
   // To statically initialize the tables of variable length, we need a flexible
   // array member, and we need to compile in gnu99 mode (constant initialization
   // of flexible array members is a GNU extension, not in C99 unfortunately.
   _upb_FastTable_Entry fasttable[];
 };
 
+// LINT.ThenChange(//depot/google3/third_party/upb/js/impl/upb_bits/mini_table.ts:presence_logic)
+
 // Map entries aren't actually stored for map fields, they are only used during
 // parsing. For parsing, it helps a lot if all map entry messages have the same
 // layout. The layout code in mini_table/decode.c will ensure that all map
 // entries have this layout.
 //
 // Note that users can and do create map entries directly, which will also use
 // this layout.
```

### Comparing `protobuf-4.22.3/upb/mini_table/sub_internal.h` & `protobuf-4.23.0rc2/upb/reflection/enum_reserved_range.h`

 * *Files 14% similar despite different names*

```diff
@@ -21,18 +21,31 @@
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#ifndef UPB_MINI_TABLE_SUB_INTERNAL_H_
-#define UPB_MINI_TABLE_SUB_INTERNAL_H_
+// IWYU pragma: private, include "upb/reflection/def.h"
 
-#include "upb/mini_table/types.h"
+#ifndef UPB_REFLECTION_ENUM_RESERVED_RANGE_H_
+#define UPB_REFLECTION_ENUM_RESERVED_RANGE_H_
 
-union upb_MiniTableSub {
-  const upb_MiniTable* submsg;
-  const upb_MiniTableEnum* subenum;
-};
+#include "upb/reflection/common.h"
 
-#endif /* UPB_MINI_TABLE_SUB_INTERNAL_H_ */
+// Must be last.
+#include "upb/port/def.inc"
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+int32_t upb_EnumReservedRange_Start(const upb_EnumReservedRange* r);
+int32_t upb_EnumReservedRange_End(const upb_EnumReservedRange* r);
+
+#ifdef __cplusplus
+} /* extern "C" */
+#endif
+
+#include "upb/port/undef.inc"
+
+#endif /* UPB_REFLECTION_ENUM_RESERVED_RANGE_H_ */
```

### Comparing `protobuf-4.22.3/upb/mini_table/types.h` & `protobuf-4.23.0rc2/upb/mini_table/types.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/mini_table.h` & `protobuf-4.23.0rc2/upb/mini_table.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/msg.h` & `protobuf-4.23.0rc2/upb/msg.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/msg_internal.h` & `protobuf-4.23.0rc2/upb/msg_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/port/def.inc` & `protobuf-4.23.0rc2/upb/port/def.inc`

 * *Files 2% similar despite different names*

```diff
@@ -186,17 +186,26 @@
 #define UPB_SETJMP(buf) _setjmp(buf)
 #define UPB_LONGJMP(buf, val) _longjmp(buf, val)
 #else
 #define UPB_SETJMP(buf) setjmp(buf)
 #define UPB_LONGJMP(buf, val) longjmp(buf, val)
 #endif
 
+#ifdef __GNUC__
+#define UPB_USE_C11_ATOMICS
+#define UPB_ATOMIC(T) _Atomic(T)
+#else
+#define UPB_ATOMIC(T) T
+#endif
+
 /* UPB_PTRADD(ptr, ofs): add pointer while avoiding "NULL + 0" UB */
 #define UPB_PTRADD(ptr, ofs) ((ofs) ? (ptr) + (ofs) : (ptr))
 
+#define UPB_PRIVATE(x) x##_dont_copy_me__upb_internal_use_only
+
 /* Configure whether fasttable is switched on or not. *************************/
 
 #ifdef __has_attribute
 #define UPB_HAS_ATTRIBUTE(x) __has_attribute(x)
 #else
 #define UPB_HAS_ATTRIBUTE(x) 0
 #endif
```

### Comparing `protobuf-4.22.3/upb/port/undef.inc` & `protobuf-4.23.0rc2/upb/port/undef.inc`

 * *Files 2% similar despite different names*

```diff
@@ -64,7 +64,10 @@
 #undef UPB_ASAN
 #undef UPB_TREAT_PROTO2_ENUMS_LIKE_PROTO3
 #undef UPB_DEPRECATED
 #undef UPB_GNUC_MIN
 #undef UPB_DESCRIPTOR_UPB_H_FILENAME
 #undef UPB_DESC
 #undef UPB_IS_GOOGLE3
+#undef UPB_ATOMIC
+#undef UPB_USE_C11_ATOMICS
+#undef UPB_PRIVATE
```

### Comparing `protobuf-4.22.3/upb/port/vsnprintf_compat.h` & `protobuf-4.23.0rc2/upb/port/vsnprintf_compat.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/common.h` & `protobuf-4.23.0rc2/upb/reflection/common.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/def.h` & `protobuf-4.23.0rc2/upb/reflection/def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/def_builder.c` & `protobuf-4.23.0rc2/upb/reflection/def_builder.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/def_builder_internal.h` & `protobuf-4.23.0rc2/upb/reflection/def_builder_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/def_pool.c` & `protobuf-4.23.0rc2/upb/reflection/def_pool.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/def_pool.h` & `protobuf-4.23.0rc2/upb/reflection/def_pool.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/def_pool_internal.h` & `protobuf-4.23.0rc2/upb/reflection/def_pool_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/def_type.c` & `protobuf-4.23.0rc2/upb/reflection/def_type.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/def_type.h` & `protobuf-4.23.0rc2/upb/reflection/def_type.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/desc_state.c` & `protobuf-4.23.0rc2/upb/reflection/desc_state.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/desc_state_internal.h` & `protobuf-4.23.0rc2/upb/reflection/desc_state_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/enum_def.c` & `protobuf-4.23.0rc2/upb/reflection/enum_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/enum_def.h` & `protobuf-4.23.0rc2/upb/reflection/enum_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/enum_def_internal.h` & `protobuf-4.23.0rc2/upb/reflection/enum_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/enum_reserved_range.c` & `protobuf-4.23.0rc2/upb/reflection/enum_reserved_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/enum_reserved_range.h` & `protobuf-4.23.0rc2/upb/reflection/message_reserved_range.h`

 * *Files 7% similar despite different names*

```diff
@@ -23,29 +23,29 @@
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 // IWYU pragma: private, include "upb/reflection/def.h"
 
-#ifndef UPB_REFLECTION_ENUM_RESERVED_RANGE_H_
-#define UPB_REFLECTION_ENUM_RESERVED_RANGE_H_
+#ifndef UPB_REFLECTION_MESSAGE_RESERVED_RANGE_H_
+#define UPB_REFLECTION_MESSAGE_RESERVED_RANGE_H_
 
 #include "upb/reflection/common.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-int32_t upb_EnumReservedRange_Start(const upb_EnumReservedRange* r);
-int32_t upb_EnumReservedRange_End(const upb_EnumReservedRange* r);
+int32_t upb_MessageReservedRange_Start(const upb_MessageReservedRange* r);
+int32_t upb_MessageReservedRange_End(const upb_MessageReservedRange* r);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
 
-#endif /* UPB_REFLECTION_ENUM_RESERVED_RANGE_H_ */
+#endif /* UPB_REFLECTION_MESSAGE_RESERVED_RANGE_H_ */
```

### Comparing `protobuf-4.22.3/upb/reflection/enum_reserved_range_internal.h` & `protobuf-4.23.0rc2/upb/reflection/enum_reserved_range_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/enum_value_def.c` & `protobuf-4.23.0rc2/upb/reflection/enum_value_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/enum_value_def.h` & `protobuf-4.23.0rc2/upb/reflection/enum_value_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/enum_value_def_internal.h` & `protobuf-4.23.0rc2/upb/reflection/enum_value_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/extension_range.c` & `protobuf-4.23.0rc2/upb/reflection/extension_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/extension_range.h` & `protobuf-4.23.0rc2/upb/reflection/extension_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/extension_range_internal.h` & `protobuf-4.23.0rc2/upb/reflection/extension_range_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/field_def.c` & `protobuf-4.23.0rc2/upb/reflection/message_def.c`

 * *Files 24% similar despite different names*

```diff
@@ -21,911 +21,698 @@
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#include <ctype.h>
-#include <errno.h>
-
+#include "upb/hash/int_table.h"
+#include "upb/hash/str_table.h"
 #include "upb/mini_table/decode.h"
 #include "upb/reflection/def.h"
 #include "upb/reflection/def_builder_internal.h"
-#include "upb/reflection/def_pool.h"
 #include "upb/reflection/def_type.h"
 #include "upb/reflection/desc_state_internal.h"
 #include "upb/reflection/enum_def_internal.h"
-#include "upb/reflection/enum_value_def_internal.h"
+#include "upb/reflection/extension_range_internal.h"
 #include "upb/reflection/field_def_internal.h"
 #include "upb/reflection/file_def_internal.h"
 #include "upb/reflection/message_def_internal.h"
+#include "upb/reflection/message_reserved_range_internal.h"
 #include "upb/reflection/oneof_def_internal.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
-#define UPB_FIELD_TYPE_UNSPECIFIED 0
-
-typedef struct {
-  size_t len;
-  char str[1];  // Null-terminated string data follows.
-} str_t;
-
-struct upb_FieldDef {
-  const UPB_DESC(FieldOptions) * opts;
+struct upb_MessageDef {
+  const UPB_DESC(MessageOptions) * opts;
+  const upb_MiniTable* layout;
   const upb_FileDef* file;
-  const upb_MessageDef* msgdef;
+  const upb_MessageDef* containing_type;
   const char* full_name;
-  const char* json_name;
-  union {
-    int64_t sint;
-    uint64_t uint;
-    double dbl;
-    float flt;
-    bool boolean;
-    str_t* str;
-    void* msg;  // Always NULL.
-  } defaultval;
-  union {
-    const upb_OneofDef* oneof;
-    const upb_MessageDef* extension_scope;
-  } scope;
-  union {
-    const upb_MessageDef* msgdef;
-    const upb_EnumDef* enumdef;
-    const UPB_DESC(FieldDescriptorProto) * unresolved;
-  } sub;
-  uint32_t number_;
-  uint16_t index_;
-  uint16_t layout_index;  // Index into msgdef->layout->fields or file->exts
-  bool has_default;
-  bool has_json_name;
-  bool has_presence;
-  bool is_extension;
-  bool is_packed;
-  bool is_proto3_optional;
-  upb_FieldType type_;
-  upb_Label label_;
+
+  // Tables for looking up fields by number and name.
+  upb_inttable itof;
+  upb_strtable ntof;
+
+  /* All nested defs.
+   * MEM: We could save some space here by putting nested defs in a contiguous
+   * region and calculating counts from offsets or vice-versa. */
+  const upb_FieldDef* fields;
+  const upb_OneofDef* oneofs;
+  const upb_ExtensionRange* ext_ranges;
+  const upb_StringView* res_names;
+  const upb_MessageDef* nested_msgs;
+  const upb_MessageReservedRange* res_ranges;
+  const upb_EnumDef* nested_enums;
+  const upb_FieldDef* nested_exts;
+
+  // TODO(salo): These counters don't need anywhere near 32 bits.
+  int field_count;
+  int real_oneof_count;
+  int oneof_count;
+  int ext_range_count;
+  int res_range_count;
+  int res_name_count;
+  int nested_msg_count;
+  int nested_enum_count;
+  int nested_ext_count;
+  bool in_message_set;
+  bool is_sorted;
+  upb_WellKnown well_known_type;
 #if UINTPTR_MAX == 0xffffffff
   uint32_t padding;  // Increase size to a multiple of 8.
 #endif
 };
 
-upb_FieldDef* _upb_FieldDef_At(const upb_FieldDef* f, int i) {
-  return (upb_FieldDef*)&f[i];
+static void assign_msg_wellknowntype(upb_MessageDef* m) {
+  const char* name = m->full_name;
+  if (name == NULL) {
+    m->well_known_type = kUpb_WellKnown_Unspecified;
+    return;
+  }
+  if (!strcmp(name, "google.protobuf.Any")) {
+    m->well_known_type = kUpb_WellKnown_Any;
+  } else if (!strcmp(name, "google.protobuf.FieldMask")) {
+    m->well_known_type = kUpb_WellKnown_FieldMask;
+  } else if (!strcmp(name, "google.protobuf.Duration")) {
+    m->well_known_type = kUpb_WellKnown_Duration;
+  } else if (!strcmp(name, "google.protobuf.Timestamp")) {
+    m->well_known_type = kUpb_WellKnown_Timestamp;
+  } else if (!strcmp(name, "google.protobuf.DoubleValue")) {
+    m->well_known_type = kUpb_WellKnown_DoubleValue;
+  } else if (!strcmp(name, "google.protobuf.FloatValue")) {
+    m->well_known_type = kUpb_WellKnown_FloatValue;
+  } else if (!strcmp(name, "google.protobuf.Int64Value")) {
+    m->well_known_type = kUpb_WellKnown_Int64Value;
+  } else if (!strcmp(name, "google.protobuf.UInt64Value")) {
+    m->well_known_type = kUpb_WellKnown_UInt64Value;
+  } else if (!strcmp(name, "google.protobuf.Int32Value")) {
+    m->well_known_type = kUpb_WellKnown_Int32Value;
+  } else if (!strcmp(name, "google.protobuf.UInt32Value")) {
+    m->well_known_type = kUpb_WellKnown_UInt32Value;
+  } else if (!strcmp(name, "google.protobuf.BoolValue")) {
+    m->well_known_type = kUpb_WellKnown_BoolValue;
+  } else if (!strcmp(name, "google.protobuf.StringValue")) {
+    m->well_known_type = kUpb_WellKnown_StringValue;
+  } else if (!strcmp(name, "google.protobuf.BytesValue")) {
+    m->well_known_type = kUpb_WellKnown_BytesValue;
+  } else if (!strcmp(name, "google.protobuf.Value")) {
+    m->well_known_type = kUpb_WellKnown_Value;
+  } else if (!strcmp(name, "google.protobuf.ListValue")) {
+    m->well_known_type = kUpb_WellKnown_ListValue;
+  } else if (!strcmp(name, "google.protobuf.Struct")) {
+    m->well_known_type = kUpb_WellKnown_Struct;
+  } else {
+    m->well_known_type = kUpb_WellKnown_Unspecified;
+  }
 }
 
-const UPB_DESC(FieldOptions) * upb_FieldDef_Options(const upb_FieldDef* f) {
-  return f->opts;
+upb_MessageDef* _upb_MessageDef_At(const upb_MessageDef* m, int i) {
+  return (upb_MessageDef*)&m[i];
 }
 
-bool upb_FieldDef_HasOptions(const upb_FieldDef* f) {
-  return f->opts != (void*)kUpbDefOptDefault;
+bool _upb_MessageDef_IsValidExtensionNumber(const upb_MessageDef* m, int n) {
+  for (int i = 0; i < m->ext_range_count; i++) {
+    const upb_ExtensionRange* r = upb_MessageDef_ExtensionRange(m, i);
+    if (upb_ExtensionRange_Start(r) <= n && n < upb_ExtensionRange_End(r)) {
+      return true;
+    }
+  }
+  return false;
 }
 
-const char* upb_FieldDef_FullName(const upb_FieldDef* f) {
-  return f->full_name;
+const UPB_DESC(MessageOptions) *
+    upb_MessageDef_Options(const upb_MessageDef* m) {
+  return m->opts;
 }
 
-upb_CType upb_FieldDef_CType(const upb_FieldDef* f) {
-  switch (f->type_) {
-    case kUpb_FieldType_Double:
-      return kUpb_CType_Double;
-    case kUpb_FieldType_Float:
-      return kUpb_CType_Float;
-    case kUpb_FieldType_Int64:
-    case kUpb_FieldType_SInt64:
-    case kUpb_FieldType_SFixed64:
-      return kUpb_CType_Int64;
-    case kUpb_FieldType_Int32:
-    case kUpb_FieldType_SFixed32:
-    case kUpb_FieldType_SInt32:
-      return kUpb_CType_Int32;
-    case kUpb_FieldType_UInt64:
-    case kUpb_FieldType_Fixed64:
-      return kUpb_CType_UInt64;
-    case kUpb_FieldType_UInt32:
-    case kUpb_FieldType_Fixed32:
-      return kUpb_CType_UInt32;
-    case kUpb_FieldType_Enum:
-      return kUpb_CType_Enum;
-    case kUpb_FieldType_Bool:
-      return kUpb_CType_Bool;
-    case kUpb_FieldType_String:
-      return kUpb_CType_String;
-    case kUpb_FieldType_Bytes:
-      return kUpb_CType_Bytes;
-    case kUpb_FieldType_Group:
-    case kUpb_FieldType_Message:
-      return kUpb_CType_Message;
-  }
-  UPB_UNREACHABLE();
+bool upb_MessageDef_HasOptions(const upb_MessageDef* m) {
+  return m->opts != (void*)kUpbDefOptDefault;
 }
 
-upb_FieldType upb_FieldDef_Type(const upb_FieldDef* f) { return f->type_; }
-
-uint32_t upb_FieldDef_Index(const upb_FieldDef* f) { return f->index_; }
-
-upb_Label upb_FieldDef_Label(const upb_FieldDef* f) { return f->label_; }
-
-uint32_t upb_FieldDef_Number(const upb_FieldDef* f) { return f->number_; }
+const char* upb_MessageDef_FullName(const upb_MessageDef* m) {
+  return m->full_name;
+}
 
-bool upb_FieldDef_IsExtension(const upb_FieldDef* f) { return f->is_extension; }
+const upb_FileDef* upb_MessageDef_File(const upb_MessageDef* m) {
+  return m->file;
+}
 
-bool upb_FieldDef_IsPacked(const upb_FieldDef* f) { return f->is_packed; }
+const upb_MessageDef* upb_MessageDef_ContainingType(const upb_MessageDef* m) {
+  return m->containing_type;
+}
 
-const char* upb_FieldDef_Name(const upb_FieldDef* f) {
-  return _upb_DefBuilder_FullToShort(f->full_name);
+const char* upb_MessageDef_Name(const upb_MessageDef* m) {
+  return _upb_DefBuilder_FullToShort(m->full_name);
 }
 
-const char* upb_FieldDef_JsonName(const upb_FieldDef* f) {
-  return f->json_name;
+upb_Syntax upb_MessageDef_Syntax(const upb_MessageDef* m) {
+  return upb_FileDef_Syntax(m->file);
 }
 
-bool upb_FieldDef_HasJsonName(const upb_FieldDef* f) {
-  return f->has_json_name;
+const upb_FieldDef* upb_MessageDef_FindFieldByNumber(const upb_MessageDef* m,
+                                                     uint32_t i) {
+  upb_value val;
+  return upb_inttable_lookup(&m->itof, i, &val) ? upb_value_getconstptr(val)
+                                                : NULL;
 }
 
-const upb_FileDef* upb_FieldDef_File(const upb_FieldDef* f) { return f->file; }
+const upb_FieldDef* upb_MessageDef_FindFieldByNameWithSize(
+    const upb_MessageDef* m, const char* name, size_t size) {
+  upb_value val;
 
-const upb_MessageDef* upb_FieldDef_ContainingType(const upb_FieldDef* f) {
-  return f->msgdef;
-}
+  if (!upb_strtable_lookup2(&m->ntof, name, size, &val)) {
+    return NULL;
+  }
 
-const upb_MessageDef* upb_FieldDef_ExtensionScope(const upb_FieldDef* f) {
-  return f->is_extension ? f->scope.extension_scope : NULL;
+  return _upb_DefType_Unpack(val, UPB_DEFTYPE_FIELD);
 }
 
-const upb_OneofDef* upb_FieldDef_ContainingOneof(const upb_FieldDef* f) {
-  return f->is_extension ? NULL : f->scope.oneof;
+const upb_OneofDef* upb_MessageDef_FindOneofByNameWithSize(
+    const upb_MessageDef* m, const char* name, size_t size) {
+  upb_value val;
+
+  if (!upb_strtable_lookup2(&m->ntof, name, size, &val)) {
+    return NULL;
+  }
+
+  return _upb_DefType_Unpack(val, UPB_DEFTYPE_ONEOF);
 }
 
-const upb_OneofDef* upb_FieldDef_RealContainingOneof(const upb_FieldDef* f) {
-  const upb_OneofDef* oneof = upb_FieldDef_ContainingOneof(f);
-  if (!oneof || upb_OneofDef_IsSynthetic(oneof)) return NULL;
-  return oneof;
+bool _upb_MessageDef_Insert(upb_MessageDef* m, const char* name, size_t len,
+                            upb_value v, upb_Arena* a) {
+  return upb_strtable_insert(&m->ntof, name, len, v, a);
 }
 
-upb_MessageValue upb_FieldDef_Default(const upb_FieldDef* f) {
-  upb_MessageValue ret;
+bool upb_MessageDef_FindByNameWithSize(const upb_MessageDef* m,
+                                       const char* name, size_t len,
+                                       const upb_FieldDef** out_f,
+                                       const upb_OneofDef** out_o) {
+  upb_value val;
 
-  if (upb_FieldDef_IsRepeated(f) || upb_FieldDef_IsSubMessage(f)) {
-    return (upb_MessageValue){.msg_val = NULL};
+  if (!upb_strtable_lookup2(&m->ntof, name, len, &val)) {
+    return false;
   }
 
-  switch (upb_FieldDef_CType(f)) {
-    case kUpb_CType_Bool:
-      return (upb_MessageValue){.bool_val = f->defaultval.boolean};
-    case kUpb_CType_Int64:
-      return (upb_MessageValue){.int64_val = f->defaultval.sint};
-    case kUpb_CType_UInt64:
-      return (upb_MessageValue){.uint64_val = f->defaultval.uint};
-    case kUpb_CType_Enum:
-    case kUpb_CType_Int32:
-      return (upb_MessageValue){.int32_val = (int32_t)f->defaultval.sint};
-    case kUpb_CType_UInt32:
-      return (upb_MessageValue){.uint32_val = (uint32_t)f->defaultval.uint};
-    case kUpb_CType_Float:
-      return (upb_MessageValue){.float_val = f->defaultval.flt};
-    case kUpb_CType_Double:
-      return (upb_MessageValue){.double_val = f->defaultval.dbl};
-    case kUpb_CType_String:
-    case kUpb_CType_Bytes: {
-      str_t* str = f->defaultval.str;
-      if (str) {
-        return (upb_MessageValue){
-            .str_val = (upb_StringView){.data = str->str, .size = str->len}};
-      } else {
-        return (upb_MessageValue){
-            .str_val = (upb_StringView){.data = NULL, .size = 0}};
-      }
-    }
-    default:
-      UPB_UNREACHABLE();
+  const upb_FieldDef* f = _upb_DefType_Unpack(val, UPB_DEFTYPE_FIELD);
+  const upb_OneofDef* o = _upb_DefType_Unpack(val, UPB_DEFTYPE_ONEOF);
+  if (out_f) *out_f = f;
+  if (out_o) *out_o = o;
+  return f || o; /* False if this was a JSON name. */
+}
+
+const upb_FieldDef* upb_MessageDef_FindByJsonNameWithSize(
+    const upb_MessageDef* m, const char* name, size_t size) {
+  upb_value val;
+  const upb_FieldDef* f;
+
+  if (!upb_strtable_lookup2(&m->ntof, name, size, &val)) {
+    return NULL;
   }
 
-  return ret;
-}
+  f = _upb_DefType_Unpack(val, UPB_DEFTYPE_FIELD);
+  if (!f) f = _upb_DefType_Unpack(val, UPB_DEFTYPE_FIELD_JSONNAME);
 
-const upb_MessageDef* upb_FieldDef_MessageSubDef(const upb_FieldDef* f) {
-  return upb_FieldDef_CType(f) == kUpb_CType_Message ? f->sub.msgdef : NULL;
+  return f;
 }
 
-const upb_EnumDef* upb_FieldDef_EnumSubDef(const upb_FieldDef* f) {
-  return upb_FieldDef_CType(f) == kUpb_CType_Enum ? f->sub.enumdef : NULL;
+int upb_MessageDef_ExtensionRangeCount(const upb_MessageDef* m) {
+  return m->ext_range_count;
 }
 
-const upb_MiniTableField* upb_FieldDef_MiniTable(const upb_FieldDef* f) {
-  if (upb_FieldDef_IsExtension(f)) {
-    const upb_FileDef* file = upb_FieldDef_File(f);
-    return (upb_MiniTableField*)_upb_FileDef_ExtensionMiniTable(
-        file, f->layout_index);
-  } else {
-    const upb_MiniTable* layout = upb_MessageDef_MiniTable(f->msgdef);
-    return &layout->fields[f->layout_index];
-  }
+int upb_MessageDef_ReservedRangeCount(const upb_MessageDef* m) {
+  return m->res_range_count;
 }
 
-const upb_MiniTableExtension* _upb_FieldDef_ExtensionMiniTable(
-    const upb_FieldDef* f) {
-  UPB_ASSERT(upb_FieldDef_IsExtension(f));
-  const upb_FileDef* file = upb_FieldDef_File(f);
-  return _upb_FileDef_ExtensionMiniTable(file, f->layout_index);
+int upb_MessageDef_ReservedNameCount(const upb_MessageDef* m) {
+  return m->res_name_count;
 }
 
-bool _upb_FieldDef_IsClosedEnum(const upb_FieldDef* f) {
-  if (f->type_ != kUpb_FieldType_Enum) return false;
-  return upb_EnumDef_IsClosed(f->sub.enumdef);
+int upb_MessageDef_FieldCount(const upb_MessageDef* m) {
+  return m->field_count;
 }
 
-bool _upb_FieldDef_IsProto3Optional(const upb_FieldDef* f) {
-  return f->is_proto3_optional;
+int upb_MessageDef_OneofCount(const upb_MessageDef* m) {
+  return m->oneof_count;
 }
 
-int _upb_FieldDef_LayoutIndex(const upb_FieldDef* f) { return f->layout_index; }
-
-uint64_t _upb_FieldDef_Modifiers(const upb_FieldDef* f) {
-  uint64_t out = f->is_packed ? kUpb_FieldModifier_IsPacked : 0;
+int upb_MessageDef_RealOneofCount(const upb_MessageDef* m) {
+  return m->real_oneof_count;
+}
 
-  switch (f->label_) {
-    case kUpb_Label_Optional:
-      if (!upb_FieldDef_HasPresence(f)) {
-        out |= kUpb_FieldModifier_IsProto3Singular;
-      }
-      break;
-    case kUpb_Label_Repeated:
-      out |= kUpb_FieldModifier_IsRepeated;
-      break;
-    case kUpb_Label_Required:
-      out |= kUpb_FieldModifier_IsRequired;
-      break;
-  }
+int upb_MessageDef_NestedMessageCount(const upb_MessageDef* m) {
+  return m->nested_msg_count;
+}
 
-  if (_upb_FieldDef_IsClosedEnum(f)) {
-    out |= kUpb_FieldModifier_IsClosedEnum;
-  }
-  return out;
+int upb_MessageDef_NestedEnumCount(const upb_MessageDef* m) {
+  return m->nested_enum_count;
 }
 
-bool upb_FieldDef_HasDefault(const upb_FieldDef* f) { return f->has_default; }
-bool upb_FieldDef_HasPresence(const upb_FieldDef* f) { return f->has_presence; }
+int upb_MessageDef_NestedExtensionCount(const upb_MessageDef* m) {
+  return m->nested_ext_count;
+}
 
-bool upb_FieldDef_HasSubDef(const upb_FieldDef* f) {
-  return upb_FieldDef_IsSubMessage(f) ||
-         upb_FieldDef_CType(f) == kUpb_CType_Enum;
+const upb_MiniTable* upb_MessageDef_MiniTable(const upb_MessageDef* m) {
+  return m->layout;
 }
 
-bool upb_FieldDef_IsMap(const upb_FieldDef* f) {
-  return upb_FieldDef_IsRepeated(f) && upb_FieldDef_IsSubMessage(f) &&
-         upb_MessageDef_IsMapEntry(upb_FieldDef_MessageSubDef(f));
+const upb_ExtensionRange* upb_MessageDef_ExtensionRange(const upb_MessageDef* m,
+                                                        int i) {
+  UPB_ASSERT(0 <= i && i < m->ext_range_count);
+  return _upb_ExtensionRange_At(m->ext_ranges, i);
 }
 
-bool upb_FieldDef_IsOptional(const upb_FieldDef* f) {
-  return upb_FieldDef_Label(f) == kUpb_Label_Optional;
+const upb_MessageReservedRange* upb_MessageDef_ReservedRange(
+    const upb_MessageDef* m, int i) {
+  UPB_ASSERT(0 <= i && i < m->res_range_count);
+  return _upb_MessageReservedRange_At(m->res_ranges, i);
 }
 
-bool upb_FieldDef_IsPrimitive(const upb_FieldDef* f) {
-  return !upb_FieldDef_IsString(f) && !upb_FieldDef_IsSubMessage(f);
+upb_StringView upb_MessageDef_ReservedName(const upb_MessageDef* m, int i) {
+  UPB_ASSERT(0 <= i && i < m->res_name_count);
+  return m->res_names[i];
 }
 
-bool upb_FieldDef_IsRepeated(const upb_FieldDef* f) {
-  return upb_FieldDef_Label(f) == kUpb_Label_Repeated;
+const upb_FieldDef* upb_MessageDef_Field(const upb_MessageDef* m, int i) {
+  UPB_ASSERT(0 <= i && i < m->field_count);
+  return _upb_FieldDef_At(m->fields, i);
 }
 
-bool upb_FieldDef_IsRequired(const upb_FieldDef* f) {
-  return upb_FieldDef_Label(f) == kUpb_Label_Required;
+const upb_OneofDef* upb_MessageDef_Oneof(const upb_MessageDef* m, int i) {
+  UPB_ASSERT(0 <= i && i < m->oneof_count);
+  return _upb_OneofDef_At(m->oneofs, i);
 }
 
-bool upb_FieldDef_IsString(const upb_FieldDef* f) {
-  return upb_FieldDef_CType(f) == kUpb_CType_String ||
-         upb_FieldDef_CType(f) == kUpb_CType_Bytes;
+const upb_MessageDef* upb_MessageDef_NestedMessage(const upb_MessageDef* m,
+                                                   int i) {
+  UPB_ASSERT(0 <= i && i < m->nested_msg_count);
+  return &m->nested_msgs[i];
 }
 
-bool upb_FieldDef_IsSubMessage(const upb_FieldDef* f) {
-  return upb_FieldDef_CType(f) == kUpb_CType_Message;
+const upb_EnumDef* upb_MessageDef_NestedEnum(const upb_MessageDef* m, int i) {
+  UPB_ASSERT(0 <= i && i < m->nested_enum_count);
+  return _upb_EnumDef_At(m->nested_enums, i);
 }
 
-static bool between(int32_t x, int32_t low, int32_t high) {
-  return x >= low && x <= high;
+const upb_FieldDef* upb_MessageDef_NestedExtension(const upb_MessageDef* m,
+                                                   int i) {
+  UPB_ASSERT(0 <= i && i < m->nested_ext_count);
+  return _upb_FieldDef_At(m->nested_exts, i);
 }
 
-bool upb_FieldDef_checklabel(int32_t label) { return between(label, 1, 3); }
-bool upb_FieldDef_checktype(int32_t type) { return between(type, 1, 11); }
-bool upb_FieldDef_checkintfmt(int32_t fmt) { return between(fmt, 1, 3); }
+upb_WellKnown upb_MessageDef_WellKnownType(const upb_MessageDef* m) {
+  return m->well_known_type;
+}
 
-bool upb_FieldDef_checkdescriptortype(int32_t type) {
-  return between(type, 1, 18);
+bool _upb_MessageDef_InMessageSet(const upb_MessageDef* m) {
+  return m->in_message_set;
 }
 
-static bool streql2(const char* a, size_t n, const char* b) {
-  return n == strlen(b) && memcmp(a, b, n) == 0;
+const upb_FieldDef* upb_MessageDef_FindFieldByName(const upb_MessageDef* m,
+                                                   const char* name) {
+  return upb_MessageDef_FindFieldByNameWithSize(m, name, strlen(name));
 }
 
-// Implement the transformation as described in the spec:
-//   1. upper case all letters after an underscore.
-//   2. remove all underscores.
-static char* make_json_name(const char* name, size_t size, upb_Arena* a) {
-  char* out = upb_Arena_Malloc(a, size + 1);  // +1 is to add a trailing '\0'
-  if (out == NULL) return NULL;
+const upb_OneofDef* upb_MessageDef_FindOneofByName(const upb_MessageDef* m,
+                                                   const char* name) {
+  return upb_MessageDef_FindOneofByNameWithSize(m, name, strlen(name));
+}
 
-  bool ucase_next = false;
-  char* des = out;
-  for (size_t i = 0; i < size; i++) {
-    if (name[i] == '_') {
-      ucase_next = true;
-    } else {
-      *des++ = ucase_next ? toupper(name[i]) : name[i];
-      ucase_next = false;
-    }
-  }
-  *des++ = '\0';
-  return out;
+bool upb_MessageDef_IsMapEntry(const upb_MessageDef* m) {
+  return UPB_DESC(MessageOptions_map_entry)(m->opts);
 }
 
-static str_t* newstr(upb_DefBuilder* ctx, const char* data, size_t len) {
-  str_t* ret = _upb_DefBuilder_Alloc(ctx, sizeof(*ret) + len);
-  if (!ret) _upb_DefBuilder_OomErr(ctx);
-  ret->len = len;
-  if (len) memcpy(ret->str, data, len);
-  ret->str[len] = '\0';
-  return ret;
+bool upb_MessageDef_IsMessageSet(const upb_MessageDef* m) {
+  return UPB_DESC(MessageOptions_message_set_wire_format)(m->opts);
 }
 
-static str_t* unescape(upb_DefBuilder* ctx, const upb_FieldDef* f,
-                       const char* data, size_t len) {
-  // Size here is an upper bound; escape sequences could ultimately shrink it.
-  str_t* ret = _upb_DefBuilder_Alloc(ctx, sizeof(*ret) + len);
-  char* dst = &ret->str[0];
-  const char* src = data;
-  const char* end = data + len;
-
-  while (src < end) {
-    if (*src == '\\') {
-      src++;
-      *dst++ = _upb_DefBuilder_ParseEscape(ctx, f, &src, end);
-    } else {
-      *dst++ = *src++;
-    }
-  }
+static upb_MiniTable* _upb_MessageDef_MakeMiniTable(upb_DefBuilder* ctx,
+                                                    const upb_MessageDef* m) {
+  upb_StringView desc;
+  // Note: this will assign layout_index for fields, so upb_FieldDef_MiniTable()
+  // is safe to call only after this call.
+  bool ok = upb_MessageDef_MiniDescriptorEncode(m, ctx->tmp_arena, &desc);
+  if (!ok) _upb_DefBuilder_OomErr(ctx);
+
+  void** scratch_data = _upb_DefPool_ScratchData(ctx->symtab);
+  size_t* scratch_size = _upb_DefPool_ScratchSize(ctx->symtab);
+  upb_MiniTable* ret = upb_MiniTable_BuildWithBuf(
+      desc.data, desc.size, ctx->platform, ctx->arena, scratch_data,
+      scratch_size, ctx->status);
+  if (!ret) _upb_DefBuilder_FailJmp(ctx);
 
-  ret->len = dst - &ret->str[0];
   return ret;
 }
 
-static void parse_default(upb_DefBuilder* ctx, const char* str, size_t len,
-                          upb_FieldDef* f) {
-  char* end;
-  char nullz[64];
-  errno = 0;
-
-  switch (upb_FieldDef_CType(f)) {
-    case kUpb_CType_Int32:
-    case kUpb_CType_Int64:
-    case kUpb_CType_UInt32:
-    case kUpb_CType_UInt64:
-    case kUpb_CType_Double:
-    case kUpb_CType_Float:
-      // Standard C number parsing functions expect null-terminated strings.
-      if (len >= sizeof(nullz) - 1) {
-        _upb_DefBuilder_Errf(ctx, "Default too long: %.*s", (int)len, str);
-      }
-      memcpy(nullz, str, len);
-      nullz[len] = '\0';
-      str = nullz;
-      break;
-    default:
-      break;
+void _upb_MessageDef_Resolve(upb_DefBuilder* ctx, upb_MessageDef* m) {
+  for (int i = 0; i < m->field_count; i++) {
+    upb_FieldDef* f = (upb_FieldDef*)upb_MessageDef_Field(m, i);
+    _upb_FieldDef_Resolve(ctx, m->full_name, f);
   }
 
-  switch (upb_FieldDef_CType(f)) {
-    case kUpb_CType_Int32: {
-      long val = strtol(str, &end, 0);
-      if (val > INT32_MAX || val < INT32_MIN || errno == ERANGE || *end) {
-        goto invalid;
-      }
-      f->defaultval.sint = val;
-      break;
+  m->in_message_set = false;
+  for (int i = 0; i < upb_MessageDef_NestedExtensionCount(m); i++) {
+    upb_FieldDef* ext = (upb_FieldDef*)upb_MessageDef_NestedExtension(m, i);
+    _upb_FieldDef_Resolve(ctx, m->full_name, ext);
+    if (upb_FieldDef_Type(ext) == kUpb_FieldType_Message &&
+        upb_FieldDef_Label(ext) == kUpb_Label_Optional &&
+        upb_FieldDef_MessageSubDef(ext) == m &&
+        UPB_DESC(MessageOptions_message_set_wire_format)(
+            upb_MessageDef_Options(upb_FieldDef_ContainingType(ext)))) {
+      m->in_message_set = true;
     }
-    case kUpb_CType_Enum: {
-      const upb_EnumDef* e = f->sub.enumdef;
-      const upb_EnumValueDef* ev =
-          upb_EnumDef_FindValueByNameWithSize(e, str, len);
-      if (!ev) {
-        goto invalid;
-      }
-      f->defaultval.sint = upb_EnumValueDef_Number(ev);
-      break;
-    }
-    case kUpb_CType_Int64: {
-      long long val = strtoll(str, &end, 0);
-      if (val > INT64_MAX || val < INT64_MIN || errno == ERANGE || *end) {
-        goto invalid;
-      }
-      f->defaultval.sint = val;
-      break;
-    }
-    case kUpb_CType_UInt32: {
-      unsigned long val = strtoul(str, &end, 0);
-      if (val > UINT32_MAX || errno == ERANGE || *end) {
-        goto invalid;
-      }
-      f->defaultval.uint = val;
-      break;
-    }
-    case kUpb_CType_UInt64: {
-      unsigned long long val = strtoull(str, &end, 0);
-      if (val > UINT64_MAX || errno == ERANGE || *end) {
-        goto invalid;
-      }
-      f->defaultval.uint = val;
-      break;
-    }
-    case kUpb_CType_Double: {
-      double val = strtod(str, &end);
-      if (errno == ERANGE || *end) {
-        goto invalid;
-      }
-      f->defaultval.dbl = val;
-      break;
-    }
-    case kUpb_CType_Float: {
-      float val = strtof(str, &end);
-      if (errno == ERANGE || *end) {
-        goto invalid;
-      }
-      f->defaultval.flt = val;
-      break;
-    }
-    case kUpb_CType_Bool: {
-      if (streql2(str, len, "false")) {
-        f->defaultval.boolean = false;
-      } else if (streql2(str, len, "true")) {
-        f->defaultval.boolean = true;
-      } else {
-        goto invalid;
-      }
-      break;
-    }
-    case kUpb_CType_String:
-      f->defaultval.str = newstr(ctx, str, len);
-      break;
-    case kUpb_CType_Bytes:
-      f->defaultval.str = unescape(ctx, f, str, len);
-      break;
-    case kUpb_CType_Message:
-      /* Should not have a default value. */
-      _upb_DefBuilder_Errf(ctx, "Message should not have a default (%s)",
-                           upb_FieldDef_FullName(f));
-  }
-
-  return;
-
-invalid:
-  _upb_DefBuilder_Errf(ctx, "Invalid default '%.*s' for field %s of type %d",
-                       (int)len, str, upb_FieldDef_FullName(f),
-                       (int)upb_FieldDef_Type(f));
-}
-
-static void set_default_default(upb_DefBuilder* ctx, upb_FieldDef* f) {
-  switch (upb_FieldDef_CType(f)) {
-    case kUpb_CType_Int32:
-    case kUpb_CType_Int64:
-      f->defaultval.sint = 0;
-      break;
-    case kUpb_CType_UInt64:
-    case kUpb_CType_UInt32:
-      f->defaultval.uint = 0;
-      break;
-    case kUpb_CType_Double:
-    case kUpb_CType_Float:
-      f->defaultval.dbl = 0;
-      break;
-    case kUpb_CType_String:
-    case kUpb_CType_Bytes:
-      f->defaultval.str = newstr(ctx, NULL, 0);
-      break;
-    case kUpb_CType_Bool:
-      f->defaultval.boolean = false;
-      break;
-    case kUpb_CType_Enum: {
-      const upb_EnumValueDef* v = upb_EnumDef_Value(f->sub.enumdef, 0);
-      f->defaultval.sint = upb_EnumValueDef_Number(v);
-      break;
-    }
-    case kUpb_CType_Message:
-      break;
   }
-}
 
-static void _upb_FieldDef_Create(upb_DefBuilder* ctx, const char* prefix,
-                                 const UPB_DESC(FieldDescriptorProto) *
-                                     field_proto,
-                                 upb_MessageDef* m, upb_FieldDef* f) {
-  // Must happen before _upb_DefBuilder_Add()
-  f->file = _upb_DefBuilder_File(ctx);
-
-  if (!UPB_DESC(FieldDescriptorProto_has_name)(field_proto)) {
-    _upb_DefBuilder_Errf(ctx, "field has no name");
+  for (int i = 0; i < upb_MessageDef_NestedMessageCount(m); i++) {
+    upb_MessageDef* n = (upb_MessageDef*)upb_MessageDef_NestedMessage(m, i);
+    _upb_MessageDef_Resolve(ctx, n);
   }
+}
 
-  const upb_StringView name = UPB_DESC(FieldDescriptorProto_name)(field_proto);
+void _upb_MessageDef_InsertField(upb_DefBuilder* ctx, upb_MessageDef* m,
+                                 const upb_FieldDef* f) {
+  const int32_t field_number = upb_FieldDef_Number(f);
 
-  f->full_name = _upb_DefBuilder_MakeFullName(ctx, prefix, name);
-  f->label_ = (int)UPB_DESC(FieldDescriptorProto_label)(field_proto);
-  f->number_ = UPB_DESC(FieldDescriptorProto_number)(field_proto);
-  f->is_proto3_optional =
-      UPB_DESC(FieldDescriptorProto_proto3_optional)(field_proto);
-  f->msgdef = m;
-  f->scope.oneof = NULL;
-
-  f->has_json_name = UPB_DESC(FieldDescriptorProto_has_json_name)(field_proto);
-  if (f->has_json_name) {
-    const upb_StringView sv =
-        UPB_DESC(FieldDescriptorProto_json_name)(field_proto);
-    f->json_name = upb_strdup2(sv.data, sv.size, ctx->arena);
-  } else {
-    f->json_name = make_json_name(name.data, name.size, ctx->arena);
+  if (field_number <= 0 || field_number > kUpb_MaxFieldNumber) {
+    _upb_DefBuilder_Errf(ctx, "invalid field number (%u)", field_number);
   }
-  if (!f->json_name) _upb_DefBuilder_OomErr(ctx);
 
-  const bool has_type = UPB_DESC(FieldDescriptorProto_has_type)(field_proto);
-  const bool has_type_name =
-      UPB_DESC(FieldDescriptorProto_has_type_name)(field_proto);
-
-  f->type_ = (int)UPB_DESC(FieldDescriptorProto_type)(field_proto);
-
-  if (has_type) {
-    switch (f->type_) {
-      case kUpb_FieldType_Message:
-      case kUpb_FieldType_Group:
-      case kUpb_FieldType_Enum:
-        if (!has_type_name) {
-          _upb_DefBuilder_Errf(ctx, "field of type %d requires type name (%s)",
-                               (int)f->type_, f->full_name);
-        }
-        break;
-      default:
-        if (has_type_name) {
-          _upb_DefBuilder_Errf(
-              ctx, "invalid type for field with type_name set (%s, %d)",
-              f->full_name, (int)f->type_);
-        }
-    }
-  } else if (has_type_name) {
-    f->type_ =
-        UPB_FIELD_TYPE_UNSPECIFIED;  // We'll fill this in in resolve_fielddef()
-  }
+  const char* json_name = upb_FieldDef_JsonName(f);
+  const char* shortname = upb_FieldDef_Name(f);
+  const size_t shortnamelen = strlen(shortname);
 
-  if (f->type_ < kUpb_FieldType_Double || f->type_ > kUpb_FieldType_SInt64) {
-    _upb_DefBuilder_Errf(ctx, "invalid type for field %s (%d)", f->full_name,
-                         f->type_);
-  }
+  upb_value v = upb_value_constptr(f);
 
-  if (f->label_ < kUpb_Label_Optional || f->label_ > kUpb_Label_Repeated) {
-    _upb_DefBuilder_Errf(ctx, "invalid label for field %s (%d)", f->full_name,
-                         f->label_);
+  upb_value existing_v;
+  if (upb_strtable_lookup(&m->ntof, shortname, &existing_v)) {
+    _upb_DefBuilder_Errf(ctx, "duplicate field name (%s)", shortname);
   }
 
-  /* We can't resolve the subdef or (in the case of extensions) the containing
-   * message yet, because it may not have been defined yet.  We stash a pointer
-   * to the field_proto until later when we can properly resolve it. */
-  f->sub.unresolved = field_proto;
-
-  if (f->label_ == kUpb_Label_Required &&
-      upb_FileDef_Syntax(f->file) == kUpb_Syntax_Proto3) {
-    _upb_DefBuilder_Errf(ctx, "proto3 fields cannot be required (%s)",
-                         f->full_name);
-  }
-
-  if (UPB_DESC(FieldDescriptorProto_has_oneof_index)(field_proto)) {
-    uint32_t oneof_index =
-        UPB_DESC(FieldDescriptorProto_oneof_index)(field_proto);
-
-    if (upb_FieldDef_Label(f) != kUpb_Label_Optional) {
-      _upb_DefBuilder_Errf(ctx, "fields in oneof must have OPTIONAL label (%s)",
-                           f->full_name);
-    }
-
-    if (!m) {
-      _upb_DefBuilder_Errf(ctx, "oneof field (%s) has no containing msg",
-                           f->full_name);
-    }
+  const upb_value field_v = _upb_DefType_Pack(f, UPB_DEFTYPE_FIELD);
+  bool ok =
+      _upb_MessageDef_Insert(m, shortname, shortnamelen, field_v, ctx->arena);
+  if (!ok) _upb_DefBuilder_OomErr(ctx);
 
-    if (oneof_index >= upb_MessageDef_OneofCount(m)) {
-      _upb_DefBuilder_Errf(ctx, "oneof_index out of range (%s)", f->full_name);
+  if (strcmp(shortname, json_name) != 0) {
+    if (upb_strtable_lookup(&m->ntof, json_name, &v)) {
+      _upb_DefBuilder_Errf(ctx, "duplicate json_name (%s)", json_name);
     }
 
-    upb_OneofDef* oneof = (upb_OneofDef*)upb_MessageDef_Oneof(m, oneof_index);
-    f->scope.oneof = oneof;
-
-    bool ok = _upb_OneofDef_Insert(oneof, f, name.data, name.size, ctx->arena);
+    const size_t json_size = strlen(json_name);
+    const upb_value json_v = _upb_DefType_Pack(f, UPB_DEFTYPE_FIELD_JSONNAME);
+    ok = _upb_MessageDef_Insert(m, json_name, json_size, json_v, ctx->arena);
     if (!ok) _upb_DefBuilder_OomErr(ctx);
   }
 
-  UPB_DEF_SET_OPTIONS(f->opts, FieldDescriptorProto, FieldOptions, field_proto);
-
-  if (UPB_DESC(FieldOptions_has_packed)(f->opts)) {
-    f->is_packed = UPB_DESC(FieldOptions_packed)(f->opts);
-  } else {
-    // Repeated fields default to packed for proto3 only.
-    f->is_packed = upb_FieldDef_IsPrimitive(f) &&
-                   f->label_ == kUpb_Label_Repeated &&
-                   upb_FileDef_Syntax(f->file) == kUpb_Syntax_Proto3;
+  if (upb_inttable_lookup(&m->itof, field_number, NULL)) {
+    _upb_DefBuilder_Errf(ctx, "duplicate field number (%u)", field_number);
   }
 
-  f->has_presence =
-      (!upb_FieldDef_IsRepeated(f)) &&
-      (upb_FieldDef_IsSubMessage(f) || upb_FieldDef_ContainingOneof(f) ||
-       (upb_FileDef_Syntax(f->file) == kUpb_Syntax_Proto2));
+  ok = upb_inttable_insert(&m->itof, field_number, v, ctx->arena);
+  if (!ok) _upb_DefBuilder_OomErr(ctx);
 }
 
-static void _upb_FieldDef_CreateExt(upb_DefBuilder* ctx, const char* prefix,
-                                    const UPB_DESC(FieldDescriptorProto) *
-                                        field_proto,
-                                    upb_MessageDef* m, upb_FieldDef* f) {
-  f->is_extension = true;
-  _upb_FieldDef_Create(ctx, prefix, field_proto, m, f);
+void _upb_MessageDef_CreateMiniTable(upb_DefBuilder* ctx, upb_MessageDef* m) {
+  if (ctx->layout == NULL) {
+    m->layout = _upb_MessageDef_MakeMiniTable(ctx, m);
+  } else {
+    UPB_ASSERT(ctx->msg_count < ctx->layout->msg_count);
+    m->layout = ctx->layout->msgs[ctx->msg_count++];
+    UPB_ASSERT(m->field_count == m->layout->field_count);
 
-  if (UPB_DESC(FieldDescriptorProto_has_oneof_index)(field_proto)) {
-    _upb_DefBuilder_Errf(ctx, "oneof_index provided for extension field (%s)",
-                         f->full_name);
+    // We don't need the result of this call, but it will assign layout_index
+    // for all the fields in O(n lg n) time.
+    _upb_FieldDefs_Sorted(m->fields, m->field_count, ctx->tmp_arena);
   }
 
-  f->scope.extension_scope = m;
-  _upb_DefBuilder_Add(ctx, f->full_name, _upb_DefType_Pack(f, UPB_DEFTYPE_EXT));
-  f->layout_index = ctx->ext_count++;
-
-  if (ctx->layout) {
-    UPB_ASSERT(_upb_FieldDef_ExtensionMiniTable(f)->field.number == f->number_);
+  for (int i = 0; i < m->nested_msg_count; i++) {
+    upb_MessageDef* nested =
+        (upb_MessageDef*)upb_MessageDef_NestedMessage(m, i);
+    _upb_MessageDef_CreateMiniTable(ctx, nested);
   }
 }
 
-static void _upb_FieldDef_CreateNotExt(upb_DefBuilder* ctx, const char* prefix,
-                                       const UPB_DESC(FieldDescriptorProto) *
-                                           field_proto,
-                                       upb_MessageDef* m, upb_FieldDef* f) {
-  f->is_extension = false;
-  _upb_FieldDef_Create(ctx, prefix, field_proto, m, f);
-
-  if (!UPB_DESC(FieldDescriptorProto_has_oneof_index)(field_proto)) {
-    if (f->is_proto3_optional) {
-      _upb_DefBuilder_Errf(
-          ctx,
-          "non-extension field (%s) with proto3_optional was not in a oneof",
-          f->full_name);
-    }
+void _upb_MessageDef_LinkMiniTable(upb_DefBuilder* ctx,
+                                   const upb_MessageDef* m) {
+  for (int i = 0; i < upb_MessageDef_NestedExtensionCount(m); i++) {
+    const upb_FieldDef* ext = upb_MessageDef_NestedExtension(m, i);
+    _upb_FieldDef_BuildMiniTableExtension(ctx, ext);
   }
 
-  _upb_MessageDef_InsertField(ctx, m, f);
-}
+  for (int i = 0; i < m->nested_msg_count; i++) {
+    _upb_MessageDef_LinkMiniTable(ctx, upb_MessageDef_NestedMessage(m, i));
+  }
 
-upb_FieldDef* _upb_Extensions_New(
-    upb_DefBuilder* ctx, int n,
-    const UPB_DESC(FieldDescriptorProto) * const* protos, const char* prefix,
-    upb_MessageDef* m) {
-  _upb_DefType_CheckPadding(sizeof(upb_FieldDef));
-  upb_FieldDef* defs =
-      (upb_FieldDef*)_upb_DefBuilder_Alloc(ctx, sizeof(upb_FieldDef) * n);
+  if (ctx->layout) return;
 
-  for (int i = 0; i < n; i++) {
-    upb_FieldDef* f = &defs[i];
+  for (int i = 0; i < m->field_count; i++) {
+    const upb_FieldDef* f = upb_MessageDef_Field(m, i);
+    const upb_MessageDef* sub_m = upb_FieldDef_MessageSubDef(f);
+    const upb_EnumDef* sub_e = upb_FieldDef_EnumSubDef(f);
+    const int layout_index = _upb_FieldDef_LayoutIndex(f);
+    upb_MiniTable* mt = (upb_MiniTable*)upb_MessageDef_MiniTable(m);
 
-    _upb_FieldDef_CreateExt(ctx, prefix, protos[i], m, f);
-    f->index_ = i;
+    UPB_ASSERT(layout_index < m->field_count);
+    upb_MiniTableField* mt_f =
+        (upb_MiniTableField*)&m->layout->fields[layout_index];
+    if (sub_m) {
+      if (!mt->subs) {
+        _upb_DefBuilder_Errf(ctx, "unexpected submsg for (%s)", m->full_name);
+      }
+      UPB_ASSERT(mt_f);
+      UPB_ASSERT(sub_m->layout);
+      if (UPB_UNLIKELY(!upb_MiniTable_SetSubMessage(mt, mt_f, sub_m->layout))) {
+        _upb_DefBuilder_Errf(ctx, "invalid submsg for (%s)", m->full_name);
+      }
+    } else if (_upb_FieldDef_IsClosedEnum(f)) {
+      const upb_MiniTableEnum* mt_e = _upb_EnumDef_MiniTable(sub_e);
+      if (UPB_UNLIKELY(!upb_MiniTable_SetSubEnum(mt, mt_f, mt_e))) {
+        _upb_DefBuilder_Errf(ctx, "invalid subenum for (%s)", m->full_name);
+      }
+    }
   }
 
-  return defs;
+#ifndef NDEBUG
+  for (int i = 0; i < m->field_count; i++) {
+    const upb_FieldDef* f = upb_MessageDef_Field(m, i);
+    const int layout_index = _upb_FieldDef_LayoutIndex(f);
+    UPB_ASSERT(layout_index < m->layout->field_count);
+    const upb_MiniTableField* mt_f = &m->layout->fields[layout_index];
+    UPB_ASSERT(upb_FieldDef_Type(f) == upb_MiniTableField_Type(mt_f));
+    UPB_ASSERT(upb_FieldDef_HasPresence(f) ==
+               upb_MiniTableField_HasPresence(mt_f));
+  }
+#endif
 }
 
-upb_FieldDef* _upb_FieldDefs_New(
-    upb_DefBuilder* ctx, int n,
-    const UPB_DESC(FieldDescriptorProto) * const* protos, const char* prefix,
-    upb_MessageDef* m, bool* is_sorted) {
-  _upb_DefType_CheckPadding(sizeof(upb_FieldDef));
-  upb_FieldDef* defs =
-      (upb_FieldDef*)_upb_DefBuilder_Alloc(ctx, sizeof(upb_FieldDef) * n);
+static uint64_t _upb_MessageDef_Modifiers(const upb_MessageDef* m) {
+  uint64_t out = 0;
+  if (upb_FileDef_Syntax(m->file) == kUpb_Syntax_Proto3) {
+    out |= kUpb_MessageModifier_ValidateUtf8;
+    out |= kUpb_MessageModifier_DefaultIsPacked;
+  }
+  if (m->ext_range_count) {
+    out |= kUpb_MessageModifier_IsExtendable;
+  }
+  return out;
+}
 
-  uint32_t previous = 0;
-  for (int i = 0; i < n; i++) {
-    upb_FieldDef* f = &defs[i];
+static bool _upb_MessageDef_EncodeMap(upb_DescState* s, const upb_MessageDef* m,
+                                      upb_Arena* a) {
+  if (m->field_count != 2) return false;
+
+  const upb_FieldDef* key_field = upb_MessageDef_Field(m, 0);
+  const upb_FieldDef* val_field = upb_MessageDef_Field(m, 1);
+  if (key_field == NULL || val_field == NULL) return false;
+
+  UPB_ASSERT(_upb_FieldDef_LayoutIndex(key_field) == 0);
+  UPB_ASSERT(_upb_FieldDef_LayoutIndex(val_field) == 1);
+
+  s->ptr = upb_MtDataEncoder_EncodeMap(
+      &s->e, s->ptr, upb_FieldDef_Type(key_field), upb_FieldDef_Type(val_field),
+      _upb_FieldDef_Modifiers(key_field), _upb_FieldDef_Modifiers(val_field));
+  return true;
+}
 
-    _upb_FieldDef_CreateNotExt(ctx, prefix, protos[i], m, f);
-    f->index_ = i;
-    if (!ctx->layout) {
-      // Speculate that the def fields are sorted.  We will always sort the
-      // MiniTable fields, so if defs are sorted then indices will match.
-      //
-      // If this is incorrect, we will overwrite later.
-      f->layout_index = i;
-    }
+static bool _upb_MessageDef_EncodeMessage(upb_DescState* s,
+                                          const upb_MessageDef* m,
+                                          upb_Arena* a) {
+  const upb_FieldDef** sorted = NULL;
+  if (!m->is_sorted) {
+    sorted = _upb_FieldDefs_Sorted(m->fields, m->field_count, a);
+    if (!sorted) return false;
+  }
+
+  s->ptr = upb_MtDataEncoder_StartMessage(&s->e, s->ptr,
+                                          _upb_MessageDef_Modifiers(m));
+
+  for (int i = 0; i < m->field_count; i++) {
+    const upb_FieldDef* f = sorted ? sorted[i] : upb_MessageDef_Field(m, i);
+    const upb_FieldType type = upb_FieldDef_Type(f);
+    const int number = upb_FieldDef_Number(f);
+    const uint64_t modifiers = _upb_FieldDef_Modifiers(f);
+
+    if (!_upb_DescState_Grow(s, a)) return false;
+    s->ptr = upb_MtDataEncoder_PutField(&s->e, s->ptr, type, number, modifiers);
+  }
+
+  for (int i = 0; i < m->real_oneof_count; i++) {
+    if (!_upb_DescState_Grow(s, a)) return false;
+    s->ptr = upb_MtDataEncoder_StartOneof(&s->e, s->ptr);
+
+    const upb_OneofDef* o = upb_MessageDef_Oneof(m, i);
+    const int field_count = upb_OneofDef_FieldCount(o);
+    for (int j = 0; j < field_count; j++) {
+      const int number = upb_FieldDef_Number(upb_OneofDef_Field(o, j));
 
-    const uint32_t current = f->number_;
-    if (previous > current) *is_sorted = false;
-    previous = current;
-  }
-
-  return defs;
-}
-
-static void resolve_subdef(upb_DefBuilder* ctx, const char* prefix,
-                           upb_FieldDef* f) {
-  const UPB_DESC(FieldDescriptorProto)* field_proto = f->sub.unresolved;
-  upb_StringView name = UPB_DESC(FieldDescriptorProto_type_name)(field_proto);
-  bool has_name = UPB_DESC(FieldDescriptorProto_has_type_name)(field_proto);
-  switch ((int)f->type_) {
-    case UPB_FIELD_TYPE_UNSPECIFIED: {
-      // Type was not specified and must be inferred.
-      UPB_ASSERT(has_name);
-      upb_deftype_t type;
-      const void* def =
-          _upb_DefBuilder_ResolveAny(ctx, f->full_name, prefix, name, &type);
-      switch (type) {
-        case UPB_DEFTYPE_ENUM:
-          f->sub.enumdef = def;
-          f->type_ = kUpb_FieldType_Enum;
-          break;
-        case UPB_DEFTYPE_MSG:
-          f->sub.msgdef = def;
-          f->type_ = kUpb_FieldType_Message;  // It appears there is no way of
-                                              // this being a group.
-          break;
-        default:
-          _upb_DefBuilder_Errf(ctx, "Couldn't resolve type name for field %s",
-                               f->full_name);
-      }
+      if (!_upb_DescState_Grow(s, a)) return false;
+      s->ptr = upb_MtDataEncoder_PutOneofField(&s->e, s->ptr, number);
     }
-    case kUpb_FieldType_Message:
-    case kUpb_FieldType_Group:
-      UPB_ASSERT(has_name);
-      f->sub.msgdef = _upb_DefBuilder_Resolve(ctx, f->full_name, prefix, name,
-                                              UPB_DEFTYPE_MSG);
-      break;
-    case kUpb_FieldType_Enum:
-      UPB_ASSERT(has_name);
-      f->sub.enumdef = _upb_DefBuilder_Resolve(ctx, f->full_name, prefix, name,
-                                               UPB_DEFTYPE_ENUM);
-      break;
-    default:
-      // No resolution necessary.
-      break;
   }
+
+  return true;
 }
 
-static int _upb_FieldDef_Compare(const void* p1, const void* p2) {
-  const uint32_t v1 = (*(upb_FieldDef**)p1)->number_;
-  const uint32_t v2 = (*(upb_FieldDef**)p2)->number_;
-  return (v1 < v2) ? -1 : (v1 > v2);
-}
-
-// _upb_FieldDefs_Sorted() is mostly a pure function of its inputs, but has one
-// critical side effect that we depend on: it sets layout_index appropriately
-// for non-sorted lists of fields.
-const upb_FieldDef** _upb_FieldDefs_Sorted(const upb_FieldDef* f, int n,
-                                           upb_Arena* a) {
-  // TODO(salo): Replace this arena alloc with a persistent scratch buffer.
-  upb_FieldDef** out = (upb_FieldDef**)upb_Arena_Malloc(a, n * sizeof(void*));
-  if (!out) return NULL;
+static bool _upb_MessageDef_EncodeMessageSet(upb_DescState* s,
+                                             const upb_MessageDef* m,
+                                             upb_Arena* a) {
+  s->ptr = upb_MtDataEncoder_EncodeMessageSet(&s->e, s->ptr);
 
-  for (int i = 0; i < n; i++) {
-    out[i] = (upb_FieldDef*)&f[i];
-  }
-  qsort(out, n, sizeof(void*), _upb_FieldDef_Compare);
-
-  for (int i = 0; i < n; i++) {
-    out[i]->layout_index = i;
-  }
-  return (const upb_FieldDef**)out;
+  return true;
 }
 
-bool upb_FieldDef_MiniDescriptorEncode(const upb_FieldDef* f, upb_Arena* a,
-                                       upb_StringView* out) {
-  UPB_ASSERT(f->is_extension);
-
+bool upb_MessageDef_MiniDescriptorEncode(const upb_MessageDef* m, upb_Arena* a,
+                                         upb_StringView* out) {
   upb_DescState s;
   _upb_DescState_Init(&s);
 
-  const int number = upb_FieldDef_Number(f);
-  const uint64_t modifiers = _upb_FieldDef_Modifiers(f);
+  if (!_upb_DescState_Grow(&s, a)) return false;
+
+  if (upb_MessageDef_IsMapEntry(m)) {
+    if (!_upb_MessageDef_EncodeMap(&s, m, a)) return false;
+  } else if (UPB_DESC(MessageOptions_message_set_wire_format)(m->opts)) {
+    if (!_upb_MessageDef_EncodeMessageSet(&s, m, a)) return false;
+  } else {
+    if (!_upb_MessageDef_EncodeMessage(&s, m, a)) return false;
+  }
 
   if (!_upb_DescState_Grow(&s, a)) return false;
-  s.ptr = upb_MtDataEncoder_EncodeExtension(&s.e, s.ptr, f->type_, number,
-                                            modifiers);
   *s.ptr = '\0';
 
   out->data = s.buf;
   out->size = s.ptr - s.buf;
   return true;
 }
 
-static void resolve_extension(upb_DefBuilder* ctx, const char* prefix,
-                              upb_FieldDef* f,
-                              const UPB_DESC(FieldDescriptorProto) *
-                                  field_proto) {
-  if (!UPB_DESC(FieldDescriptorProto_has_extendee)(field_proto)) {
-    _upb_DefBuilder_Errf(ctx, "extension for field '%s' had no extendee",
-                         f->full_name);
-  }
-
-  upb_StringView name = UPB_DESC(FieldDescriptorProto_extendee)(field_proto);
-  const upb_MessageDef* m =
-      _upb_DefBuilder_Resolve(ctx, f->full_name, prefix, name, UPB_DEFTYPE_MSG);
-  f->msgdef = m;
-
-  if (!_upb_MessageDef_IsValidExtensionNumber(m, f->number_)) {
-    _upb_DefBuilder_Errf(
-        ctx,
-        "field number %u in extension %s has no extension range in message %s",
-        (unsigned)f->number_, f->full_name, upb_MessageDef_FullName(m));
-  }
-}
+static upb_StringView* _upb_ReservedNames_New(upb_DefBuilder* ctx, int n,
+                                              const upb_StringView* protos) {
+  upb_StringView* sv = _upb_DefBuilder_Alloc(ctx, sizeof(upb_StringView) * n);
+  for (size_t i = 0; i < n; i++) {
+    sv[i].data =
+        upb_strdup2(protos[i].data, protos[i].size, _upb_DefBuilder_Arena(ctx));
+    sv[i].size = protos[i].size;
+  }
+  return sv;
+}
+
+static void create_msgdef(upb_DefBuilder* ctx, const char* prefix,
+                          const UPB_DESC(DescriptorProto) * msg_proto,
+                          const upb_MessageDef* containing_type,
+                          upb_MessageDef* m) {
+  const UPB_DESC(OneofDescriptorProto)* const* oneofs;
+  const UPB_DESC(FieldDescriptorProto)* const* fields;
+  const UPB_DESC(DescriptorProto_ExtensionRange)* const* ext_ranges;
+  const UPB_DESC(DescriptorProto_ReservedRange)* const* res_ranges;
+  const upb_StringView* res_names;
+  size_t n_oneof, n_field, n_enum, n_ext, n_msg;
+  size_t n_ext_range, n_res_range, n_res_name;
+  upb_StringView name;
 
-void _upb_FieldDef_BuildMiniTableExtension(upb_DefBuilder* ctx,
-                                           const upb_FieldDef* f) {
-  const upb_MiniTableExtension* ext = _upb_FieldDef_ExtensionMiniTable(f);
+  // Must happen before _upb_DefBuilder_Add()
+  m->file = _upb_DefBuilder_File(ctx);
 
-  if (ctx->layout) {
-    UPB_ASSERT(upb_FieldDef_Number(f) == ext->field.number);
-  } else {
-    upb_StringView desc;
-    if (!upb_FieldDef_MiniDescriptorEncode(f, ctx->tmp_arena, &desc)) {
-      _upb_DefBuilder_OomErr(ctx);
-    }
+  m->containing_type = containing_type;
+  m->is_sorted = true;
 
-    upb_MiniTableExtension* mut_ext = (upb_MiniTableExtension*)ext;
-    upb_MiniTableSub sub = {NULL};
-    if (upb_FieldDef_IsSubMessage(f)) {
-      sub.submsg = upb_MessageDef_MiniTable(f->sub.msgdef);
-    } else if (_upb_FieldDef_IsClosedEnum(f)) {
-      sub.subenum = _upb_EnumDef_MiniTable(f->sub.enumdef);
-    }
-    bool ok2 = upb_MiniTableExtension_Build(desc.data, desc.size, mut_ext,
-                                            upb_MessageDef_MiniTable(f->msgdef),
-                                            sub, ctx->status);
-    if (!ok2) _upb_DefBuilder_Errf(ctx, "Could not build extension mini table");
-  }
+  name = UPB_DESC(DescriptorProto_name)(msg_proto);
+
+  m->full_name = _upb_DefBuilder_MakeFullName(ctx, prefix, name);
+  _upb_DefBuilder_Add(ctx, m->full_name, _upb_DefType_Pack(m, UPB_DEFTYPE_MSG));
 
-  bool ok = _upb_DefPool_InsertExt(ctx->symtab, ext, f);
+  oneofs = UPB_DESC(DescriptorProto_oneof_decl)(msg_proto, &n_oneof);
+  fields = UPB_DESC(DescriptorProto_field)(msg_proto, &n_field);
+  ext_ranges =
+      UPB_DESC(DescriptorProto_extension_range)(msg_proto, &n_ext_range);
+  res_ranges =
+      UPB_DESC(DescriptorProto_reserved_range)(msg_proto, &n_res_range);
+  res_names = UPB_DESC(DescriptorProto_reserved_name)(msg_proto, &n_res_name);
+
+  bool ok = upb_inttable_init(&m->itof, ctx->arena);
   if (!ok) _upb_DefBuilder_OomErr(ctx);
-}
 
-static void resolve_default(upb_DefBuilder* ctx, upb_FieldDef* f,
-                            const UPB_DESC(FieldDescriptorProto) *
-                                field_proto) {
-  // Have to delay resolving of the default value until now because of the enum
-  // case, since enum defaults are specified with a label.
-  if (UPB_DESC(FieldDescriptorProto_has_default_value)(field_proto)) {
-    upb_StringView defaultval =
-        UPB_DESC(FieldDescriptorProto_default_value)(field_proto);
-
-    if (upb_FileDef_Syntax(f->file) == kUpb_Syntax_Proto3) {
-      _upb_DefBuilder_Errf(ctx,
-                           "proto3 fields cannot have explicit defaults (%s)",
-                           f->full_name);
-    }
+  ok = upb_strtable_init(&m->ntof, n_oneof + n_field, ctx->arena);
+  if (!ok) _upb_DefBuilder_OomErr(ctx);
 
-    if (upb_FieldDef_IsSubMessage(f)) {
-      _upb_DefBuilder_Errf(ctx,
-                           "message fields cannot have explicit defaults (%s)",
-                           f->full_name);
-    }
+  UPB_DEF_SET_OPTIONS(m->opts, DescriptorProto, MessageOptions, msg_proto);
 
-    parse_default(ctx, defaultval.data, defaultval.size, f);
-    f->has_default = true;
-  } else {
-    set_default_default(ctx, f);
-    f->has_default = false;
+  m->oneof_count = n_oneof;
+  m->oneofs = _upb_OneofDefs_New(ctx, n_oneof, oneofs, m);
+
+  m->field_count = n_field;
+  m->fields =
+      _upb_FieldDefs_New(ctx, n_field, fields, m->full_name, m, &m->is_sorted);
+
+  // Message Sets may not contain fields.
+  if (UPB_UNLIKELY(UPB_DESC(MessageOptions_message_set_wire_format)(m->opts))) {
+    if (UPB_UNLIKELY(n_field > 0)) {
+      _upb_DefBuilder_Errf(ctx, "invalid message set (%s)", m->full_name);
+    }
   }
+
+  m->ext_range_count = n_ext_range;
+  m->ext_ranges = _upb_ExtensionRanges_New(ctx, n_ext_range, ext_ranges, m);
+
+  m->res_range_count = n_res_range;
+  m->res_ranges =
+      _upb_MessageReservedRanges_New(ctx, n_res_range, res_ranges, m);
+
+  m->res_name_count = n_res_name;
+  m->res_names = _upb_ReservedNames_New(ctx, n_res_name, res_names);
+
+  const size_t synthetic_count = _upb_OneofDefs_Finalize(ctx, m);
+  m->real_oneof_count = m->oneof_count - synthetic_count;
+
+  assign_msg_wellknowntype(m);
+  upb_inttable_compact(&m->itof, ctx->arena);
+
+  const UPB_DESC(EnumDescriptorProto)* const* enums =
+      UPB_DESC(DescriptorProto_enum_type)(msg_proto, &n_enum);
+  m->nested_enum_count = n_enum;
+  m->nested_enums = _upb_EnumDefs_New(ctx, n_enum, enums, m);
+
+  const UPB_DESC(FieldDescriptorProto)* const* exts =
+      UPB_DESC(DescriptorProto_extension)(msg_proto, &n_ext);
+  m->nested_ext_count = n_ext;
+  m->nested_exts = _upb_Extensions_New(ctx, n_ext, exts, m->full_name, m);
+
+  const UPB_DESC(DescriptorProto)* const* msgs =
+      UPB_DESC(DescriptorProto_nested_type)(msg_proto, &n_msg);
+  m->nested_msg_count = n_msg;
+  m->nested_msgs = _upb_MessageDefs_New(ctx, n_msg, msgs, m);
 }
 
-void _upb_FieldDef_Resolve(upb_DefBuilder* ctx, const char* prefix,
-                           upb_FieldDef* f) {
-  // We have to stash this away since resolve_subdef() may overwrite it.
-  const UPB_DESC(FieldDescriptorProto)* field_proto = f->sub.unresolved;
+// Allocate and initialize an array of |n| message defs.
+upb_MessageDef* _upb_MessageDefs_New(
+    upb_DefBuilder* ctx, int n, const UPB_DESC(DescriptorProto) * const* protos,
+    const upb_MessageDef* containing_type) {
+  _upb_DefType_CheckPadding(sizeof(upb_MessageDef));
 
-  resolve_subdef(ctx, prefix, f);
-  resolve_default(ctx, f, field_proto);
+  const char* name = containing_type ? containing_type->full_name
+                                     : _upb_FileDef_RawPackage(ctx->file);
 
-  if (f->is_extension) {
-    resolve_extension(ctx, prefix, f, field_proto);
+  upb_MessageDef* m = _upb_DefBuilder_Alloc(ctx, sizeof(upb_MessageDef) * n);
+  for (int i = 0; i < n; i++) {
+    create_msgdef(ctx, name, protos[i], containing_type, &m[i]);
   }
+  return m;
 }
```

### Comparing `protobuf-4.22.3/upb/reflection/field_def.h` & `protobuf-4.23.0rc2/upb/reflection/field_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/field_def_internal.h` & `protobuf-4.23.0rc2/upb/reflection/field_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/file_def.c` & `protobuf-4.23.0rc2/upb/reflection/file_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/file_def.h` & `protobuf-4.23.0rc2/upb/reflection/file_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/file_def_internal.h` & `protobuf-4.23.0rc2/upb/reflection/file_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/message.c` & `protobuf-4.23.0rc2/upb/reflection/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/message.h` & `protobuf-4.23.0rc2/upb/reflection/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/message_def.h` & `protobuf-4.23.0rc2/upb/reflection/message_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/message_def_internal.h` & `protobuf-4.23.0rc2/upb/reflection/message_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/message_reserved_range.c` & `protobuf-4.23.0rc2/upb/reflection/message_reserved_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/message_reserved_range.h` & `protobuf-4.23.0rc2/upb/reflection/message_reserved_range_internal.h`

 * *Files 10% similar despite different names*

```diff
@@ -21,31 +21,35 @@
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-// IWYU pragma: private, include "upb/reflection/def.h"
+#ifndef UPB_REFLECTION_MESSAGE_RESERVED_RANGE_INTERNAL_H_
+#define UPB_REFLECTION_MESSAGE_RESERVED_RANGE_INTERNAL_H_
 
-#ifndef UPB_REFLECTION_MESSAGE_RESERVED_RANGE_H_
-#define UPB_REFLECTION_MESSAGE_RESERVED_RANGE_H_
-
-#include "upb/reflection/common.h"
+#include "upb/reflection/message_reserved_range.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-int32_t upb_MessageReservedRange_Start(const upb_MessageReservedRange* r);
-int32_t upb_MessageReservedRange_End(const upb_MessageReservedRange* r);
+upb_MessageReservedRange* _upb_MessageReservedRange_At(
+    const upb_MessageReservedRange* r, int i);
+
+// Allocate and initialize an array of |n| reserved ranges owned by |m|.
+upb_MessageReservedRange* _upb_MessageReservedRanges_New(
+    upb_DefBuilder* ctx, int n,
+    const UPB_DESC(DescriptorProto_ReservedRange) * const* protos,
+    const upb_MessageDef* m);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
 
-#endif /* UPB_REFLECTION_MESSAGE_RESERVED_RANGE_H_ */
+#endif /* UPB_REFLECTION_MESSAGE_RESERVED_RANGE_INTERNAL_H_ */
```

### Comparing `protobuf-4.22.3/upb/reflection/message_reserved_range_internal.h` & `protobuf-4.23.0rc2/upb/reflection/oneof_def_internal.h`

 * *Files 19% similar despite different names*

```diff
@@ -21,35 +21,37 @@
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#ifndef UPB_REFLECTION_MESSAGE_RESERVED_RANGE_INTERNAL_H_
-#define UPB_REFLECTION_MESSAGE_RESERVED_RANGE_INTERNAL_H_
+#ifndef UPB_REFLECTION_ONEOF_DEF_INTERNAL_H_
+#define UPB_REFLECTION_ONEOF_DEF_INTERNAL_H_
 
-#include "upb/reflection/message_reserved_range.h"
+#include "upb/reflection/oneof_def.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-upb_MessageReservedRange* _upb_MessageReservedRange_At(
-    const upb_MessageReservedRange* r, int i);
+upb_OneofDef* _upb_OneofDef_At(const upb_OneofDef* o, int i);
+void _upb_OneofDef_Insert(upb_DefBuilder* ctx, upb_OneofDef* o,
+                          const upb_FieldDef* f, const char* name, size_t size);
 
-// Allocate and initialize an array of |n| reserved ranges owned by |m|.
-upb_MessageReservedRange* _upb_MessageReservedRanges_New(
+// Allocate and initialize an array of |n| oneof defs owned by |m|.
+upb_OneofDef* _upb_OneofDefs_New(
     upb_DefBuilder* ctx, int n,
-    const UPB_DESC(DescriptorProto_ReservedRange) * const* protos,
-    const upb_MessageDef* m);
+    const UPB_DESC(OneofDescriptorProto) * const* protos, upb_MessageDef* m);
+
+size_t _upb_OneofDefs_Finalize(upb_DefBuilder* ctx, upb_MessageDef* m);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
 
 #include "upb/port/undef.inc"
 
-#endif /* UPB_REFLECTION_MESSAGE_RESERVED_RANGE_INTERNAL_H_ */
+#endif /* UPB_REFLECTION_ONEOF_DEF_INTERNAL_H_ */
```

### Comparing `protobuf-4.22.3/upb/reflection/method_def.c` & `protobuf-4.23.0rc2/upb/reflection/method_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/method_def.h` & `protobuf-4.23.0rc2/upb/reflection/method_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/method_def_internal.h` & `protobuf-4.23.0rc2/upb/reflection/method_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/oneof_def.c` & `protobuf-4.23.0rc2/upb/reflection/oneof_def.c`

 * *Files 7% similar despite different names*

```diff
@@ -111,23 +111,43 @@
 const upb_FieldDef* upb_OneofDef_LookupNumber(const upb_OneofDef* o,
                                               uint32_t num) {
   upb_value val;
   return upb_inttable_lookup(&o->itof, num, &val) ? upb_value_getptr(val)
                                                   : NULL;
 }
 
-bool _upb_OneofDef_Insert(upb_OneofDef* o, const upb_FieldDef* f,
-                          const char* name, size_t size, upb_Arena* a) {
+void _upb_OneofDef_Insert(upb_DefBuilder* ctx, upb_OneofDef* o,
+                          const upb_FieldDef* f, const char* name,
+                          size_t size) {
   o->field_count++;
   if (_upb_FieldDef_IsProto3Optional(f)) o->synthetic = true;
 
   const int number = upb_FieldDef_Number(f);
   const upb_value v = upb_value_constptr(f);
-  return upb_inttable_insert(&o->itof, number, v, a) &&
-         upb_strtable_insert(&o->ntof, name, size, v, a);
+
+  // TODO(salo): This lookup is unfortunate because we also perform it when
+  // inserting into the message's table. Unfortunately that step occurs after
+  // this one and moving things around could be tricky so let's leave it for
+  // a future refactoring.
+  const bool number_exists = upb_inttable_lookup(&o->itof, number, NULL);
+  if (UPB_UNLIKELY(number_exists)) {
+    _upb_DefBuilder_Errf(ctx, "oneof fields have the same number (%d)", number);
+  }
+
+  // TODO(salo): More redundant work happening here.
+  const bool name_exists = upb_strtable_lookup2(&o->ntof, name, size, NULL);
+  if (UPB_UNLIKELY(name_exists)) {
+    _upb_DefBuilder_Errf(ctx, "oneof fields have the same name (%s)", name);
+  }
+
+  const bool ok = upb_inttable_insert(&o->itof, number, v, ctx->arena) &&
+                  upb_strtable_insert(&o->ntof, name, size, v, ctx->arena);
+  if (UPB_UNLIKELY(!ok)) {
+    _upb_DefBuilder_OomErr(ctx);
+  }
 }
 
 // Returns the synthetic count.
 size_t _upb_OneofDefs_Finalize(upb_DefBuilder* ctx, upb_MessageDef* m) {
   int synthetic_count = 0;
 
   for (int i = 0; i < upb_MessageDef_OneofCount(m); i++) {
```

### Comparing `protobuf-4.22.3/upb/reflection/oneof_def.h` & `protobuf-4.23.0rc2/upb/reflection/oneof_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/oneof_def_internal.h` & `protobuf-4.23.0rc2/upb/wire/common.h`

 * *Files 17% similar despite different names*

```diff
@@ -21,37 +21,24 @@
  * (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
  * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
  * ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  * (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
-#ifndef UPB_REFLECTION_ONEOF_DEF_INTERNAL_H_
-#define UPB_REFLECTION_ONEOF_DEF_INTERNAL_H_
-
-#include "upb/reflection/oneof_def.h"
+#ifndef UPB_WIRE_COMMON_H_
+#define UPB_WIRE_COMMON_H_
 
 // Must be last.
 #include "upb/port/def.inc"
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-upb_OneofDef* _upb_OneofDef_At(const upb_OneofDef* o, int i);
-bool _upb_OneofDef_Insert(upb_OneofDef* o, const upb_FieldDef* f,
-                          const char* name, size_t size, upb_Arena* a);
-
-// Allocate and initialize an array of |n| oneof defs owned by |m|.
-upb_OneofDef* _upb_OneofDefs_New(
-    upb_DefBuilder* ctx, int n,
-    const UPB_DESC(OneofDescriptorProto) * const* protos, upb_MessageDef* m);
-
-size_t _upb_OneofDefs_Finalize(upb_DefBuilder* ctx, upb_MessageDef* m);
+#define kUpb_WireFormat_DefaultDepthLimit 100
 
 #ifdef __cplusplus
-} /* extern "C" */
+}
 #endif
 
-#include "upb/port/undef.inc"
-
-#endif /* UPB_REFLECTION_ONEOF_DEF_INTERNAL_H_ */
+#endif  // UPB_WIRE_COMMON_H_
```

### Comparing `protobuf-4.22.3/upb/reflection/service_def.c` & `protobuf-4.23.0rc2/upb/reflection/service_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/service_def.h` & `protobuf-4.23.0rc2/upb/reflection/service_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/service_def_internal.h` & `protobuf-4.23.0rc2/upb/reflection/service_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection/stage0/google/protobuf/descriptor.upb.h` & `protobuf-4.23.0rc2/upb/reflection/stage0/google/protobuf/descriptor.upb.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/reflection.h` & `protobuf-4.23.0rc2/upb/reflection.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/status.h` & `protobuf-4.23.0rc2/upb/status.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/string_view.h` & `protobuf-4.23.0rc2/upb/string_view.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/text/encode.c` & `protobuf-4.23.0rc2/upb/text/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/text/encode.h` & `protobuf-4.23.0rc2/upb/text/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/text_encode.h` & `protobuf-4.23.0rc2/upb/text_encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/upb.h` & `protobuf-4.23.0rc2/upb/upb.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/util/compare.c` & `protobuf-4.23.0rc2/upb/util/compare.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/util/compare.h` & `protobuf-4.23.0rc2/upb/util/compare.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/util/def_to_proto.c` & `protobuf-4.23.0rc2/upb/util/def_to_proto.c`

 * *Files 2% similar despite different names*

```diff
@@ -98,36 +98,28 @@
   return (upb_StringView){.data = p, .size = n};
 }
 
 static bool upb_isprint(char ch) { return ch >= 0x20 && ch <= 0x7f; }
 
 static int special_escape(char ch) {
   switch (ch) {
-    case '\a':
-      return 'a';
-    case '\b':
-      return 'b';
-    case '\f':
-      return 'f';
+    // This is the same set of special escapes recognized by
+    // absl::CEscape().
     case '\n':
       return 'n';
     case '\r':
       return 'r';
     case '\t':
       return 't';
-    case '\v':
-      return 'v';
     case '\\':
       return '\\';
     case '\'':
       return '\'';
     case '"':
       return '"';
-    case '\?':
-      return '?';
     default:
       return -1;
   }
 }
 
 static upb_StringView default_bytes(upb_ToProto_Context* ctx,
                                     upb_StringView val) {
```

### Comparing `protobuf-4.22.3/upb/util/def_to_proto.h` & `protobuf-4.23.0rc2/upb/util/def_to_proto.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/util/required_fields.c` & `protobuf-4.23.0rc2/upb/util/required_fields.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/util/required_fields.h` & `protobuf-4.23.0rc2/upb/util/required_fields.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/wire/common_internal.h` & `protobuf-4.23.0rc2/upb/wire/common_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/wire/decode.c` & `protobuf-4.23.0rc2/upb/wire/decode.c`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,22 @@
  * SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
 
 #include "upb/wire/decode.h"
 
 #include <string.h>
 
+#include "upb/base/descriptor_constants.h"
 #include "upb/collections/array_internal.h"
 #include "upb/collections/map_internal.h"
+#include "upb/mem/arena_internal.h"
 #include "upb/mini_table/common.h"
 #include "upb/mini_table/enum_internal.h"
+#include "upb/port/atomic.h"
+#include "upb/wire/common.h"
 #include "upb/wire/common_internal.h"
 #include "upb/wire/decode_internal.h"
 #include "upb/wire/encode.h"
 #include "upb/wire/eps_copy_input_stream.h"
 #include "upb/wire/reader.h"
 #include "upb/wire/swap_internal.h"
 #include "upb/wire/types.h"
@@ -213,15 +217,15 @@
       break;
   }
 }
 
 static upb_Message* _upb_Decoder_NewSubMessage(
     upb_Decoder* d, const upb_MiniTableSub* subs,
     const upb_MiniTableField* field) {
-  const upb_MiniTable* subl = subs[field->submsg_index].submsg;
+  const upb_MiniTable* subl = subs[field->UPB_PRIVATE(submsg_index)].submsg;
   UPB_ASSERT(subl);
   upb_Message* msg = _upb_Message_New(subl, &d->arena);
   if (!msg) _upb_Decoder_ErrorJmp(d, kUpb_DecodeStatus_OutOfMemory);
   return msg;
 }
 
 static const char* _upb_Decoder_ReadString(upb_Decoder* d, const char* ptr,
@@ -252,15 +256,15 @@
 }
 
 UPB_FORCEINLINE
 static const char* _upb_Decoder_DecodeSubMessage(
     upb_Decoder* d, const char* ptr, upb_Message* submsg,
     const upb_MiniTableSub* subs, const upb_MiniTableField* field, int size) {
   int saved_delta = upb_EpsCopyInputStream_PushLimit(&d->input, ptr, size);
-  const upb_MiniTable* subl = subs[field->submsg_index].submsg;
+  const upb_MiniTable* subl = subs[field->UPB_PRIVATE(submsg_index)].submsg;
   UPB_ASSERT(subl);
   ptr = _upb_Decoder_RecurseSubMessage(d, ptr, submsg, subl, DECODE_NOGROUP);
   upb_EpsCopyInputStream_PopLimit(&d->input, ptr, saved_delta);
   return ptr;
 }
 
 UPB_FORCEINLINE
@@ -283,15 +287,15 @@
   return _upb_Decoder_DecodeGroup(d, ptr, NULL, NULL, number);
 }
 
 UPB_FORCEINLINE
 static const char* _upb_Decoder_DecodeKnownGroup(
     upb_Decoder* d, const char* ptr, upb_Message* submsg,
     const upb_MiniTableSub* subs, const upb_MiniTableField* field) {
-  const upb_MiniTable* subl = subs[field->submsg_index].submsg;
+  const upb_MiniTable* subl = subs[field->UPB_PRIVATE(submsg_index)].submsg;
   UPB_ASSERT(subl);
   return _upb_Decoder_DecodeGroup(d, ptr, submsg, subl, field->number);
 }
 
 static char* upb_Decoder_EncodeVarint32(uint32_t val, char* ptr) {
   do {
     uint8_t byte = val & 0x7fU;
@@ -347,15 +351,15 @@
 UPB_NOINLINE
 static const char* _upb_Decoder_DecodeEnumArray(upb_Decoder* d, const char* ptr,
                                                 upb_Message* msg,
                                                 upb_Array* arr,
                                                 const upb_MiniTableSub* subs,
                                                 const upb_MiniTableField* field,
                                                 wireval* val) {
-  const upb_MiniTableEnum* e = subs[field->submsg_index].subenum;
+  const upb_MiniTableEnum* e = subs[field->UPB_PRIVATE(submsg_index)].subenum;
   if (!_upb_Decoder_CheckEnum(d, ptr, msg, e, field, val)) return ptr;
   void* mem = UPB_PTR_AT(_upb_array_ptr(arr), arr->size * 4, void);
   arr->size++;
   memcpy(mem, val, 4);
   return ptr;
 }
 
@@ -401,15 +405,15 @@
     const upb_MiniTableField* field, int lg2) {
   int scale = 1 << lg2;
   int saved_limit = upb_EpsCopyInputStream_PushLimit(&d->input, ptr, val->size);
   char* out = UPB_PTR_AT(_upb_array_ptr(arr), arr->size << lg2, void);
   while (!_upb_Decoder_IsDone(d, &ptr)) {
     wireval elem;
     ptr = _upb_Decoder_DecodeVarint(d, ptr, &elem.uint64_val);
-    _upb_Decoder_Munge(field->descriptortype, &elem);
+    _upb_Decoder_Munge(field->UPB_PRIVATE(descriptortype), &elem);
     if (_upb_Decoder_Reserve(d, arr, 1)) {
       out = UPB_PTR_AT(_upb_array_ptr(arr), arr->size << lg2, void);
     }
     arr->size++;
     memcpy(out, &elem, scale);
     out += scale;
   }
@@ -418,15 +422,15 @@
 }
 
 UPB_NOINLINE
 static const char* _upb_Decoder_DecodeEnumPacked(
     upb_Decoder* d, const char* ptr, upb_Message* msg, upb_Array* arr,
     const upb_MiniTableSub* subs, const upb_MiniTableField* field,
     wireval* val) {
-  const upb_MiniTableEnum* e = subs[field->submsg_index].subenum;
+  const upb_MiniTableEnum* e = subs[field->UPB_PRIVATE(submsg_index)].subenum;
   int saved_limit = upb_EpsCopyInputStream_PushLimit(&d->input, ptr, val->size);
   char* out = UPB_PTR_AT(_upb_array_ptr(arr), arr->size * 4, void);
   while (!_upb_Decoder_IsDone(d, &ptr)) {
     wireval elem;
     ptr = _upb_Decoder_DecodeVarint(d, ptr, &elem.uint64_val);
     _upb_Decoder_MungeInt32(&elem);
     if (!_upb_Decoder_CheckEnum(d, ptr, msg, e, field, &elem)) {
@@ -464,15 +468,15 @@
       [kUpb_FieldType_Enum] = 2,
       [kUpb_FieldType_SFixed32] = 2,
       [kUpb_FieldType_SFixed64] = 3,
       [kUpb_FieldType_SInt32] = 2,
       [kUpb_FieldType_SInt64] = 3,
   };
 
-  size_t lg2 = kElemSizeLg2[field->descriptortype];
+  size_t lg2 = kElemSizeLg2[field->UPB_PRIVATE(descriptortype)];
   upb_Array* ret = _upb_Array_New(&d->arena, 4, lg2);
   if (!ret) _upb_Decoder_ErrorJmp(d, kUpb_DecodeStatus_OutOfMemory);
   return ret;
 }
 
 static const char* _upb_Decoder_DecodeToArray(upb_Decoder* d, const char* ptr,
                                               upb_Message* msg,
@@ -510,15 +514,16 @@
     }
     case kUpb_DecodeOp_SubMessage: {
       /* Append submessage / group. */
       upb_Message* submsg = _upb_Decoder_NewSubMessage(d, subs, field);
       *UPB_PTR_AT(_upb_array_ptr(arr), arr->size * sizeof(void*),
                   upb_Message*) = submsg;
       arr->size++;
-      if (UPB_UNLIKELY(field->descriptortype == kUpb_FieldType_Group)) {
+      if (UPB_UNLIKELY(field->UPB_PRIVATE(descriptortype) ==
+                       kUpb_FieldType_Group)) {
         return _upb_Decoder_DecodeKnownGroup(d, ptr, submsg, subs, field);
       } else {
         return _upb_Decoder_DecodeSubMessage(d, ptr, submsg, subs, field,
                                              val->size);
       }
     }
     case OP_FIXPCK_LG2(2):
@@ -561,16 +566,16 @@
       [kUpb_FieldType_SFixed64] = 8,
       [kUpb_FieldType_SInt32] = 4,
       [kUpb_FieldType_SInt64] = 8,
   };
 
   const upb_MiniTableField* key_field = &entry->fields[0];
   const upb_MiniTableField* val_field = &entry->fields[1];
-  char key_size = kSizeInMap[key_field->descriptortype];
-  char val_size = kSizeInMap[val_field->descriptortype];
+  char key_size = kSizeInMap[key_field->UPB_PRIVATE(descriptortype)];
+  char val_size = kSizeInMap[val_field->UPB_PRIVATE(descriptortype)];
   UPB_ASSERT(key_field->offset == offsetof(upb_MapEntryData, k));
   UPB_ASSERT(val_field->offset == offsetof(upb_MapEntryData, v));
   upb_Map* ret = _upb_Map_New(&d->arena, key_size, val_size);
   if (!ret) _upb_Decoder_ErrorJmp(d, kUpb_DecodeStatus_OutOfMemory);
   return ret;
 }
 
@@ -579,30 +584,30 @@
                                             const upb_MiniTableSub* subs,
                                             const upb_MiniTableField* field,
                                             wireval* val) {
   upb_Map** map_p = UPB_PTR_AT(msg, field->offset, upb_Map*);
   upb_Map* map = *map_p;
   upb_MapEntry ent;
   UPB_ASSERT(upb_MiniTableField_Type(field) == kUpb_FieldType_Message);
-  const upb_MiniTable* entry = subs[field->submsg_index].submsg;
+  const upb_MiniTable* entry = subs[field->UPB_PRIVATE(submsg_index)].submsg;
 
   UPB_ASSERT(entry->field_count == 2);
   UPB_ASSERT(!upb_IsRepeatedOrMap(&entry->fields[0]));
   UPB_ASSERT(!upb_IsRepeatedOrMap(&entry->fields[1]));
 
   if (!map) {
     map = _upb_Decoder_CreateMap(d, entry);
     *map_p = map;
   }
 
   // Parse map entry.
   memset(&ent, 0, sizeof(ent));
 
-  if (entry->fields[1].descriptortype == kUpb_FieldType_Message ||
-      entry->fields[1].descriptortype == kUpb_FieldType_Group) {
+  if (entry->fields[1].UPB_PRIVATE(descriptortype) == kUpb_FieldType_Message ||
+      entry->fields[1].UPB_PRIVATE(descriptortype) == kUpb_FieldType_Group) {
     const upb_MiniTable* submsg_table = entry->subs[0].submsg;
     // Any sub-message entry must be linked.  We do not allow dynamic tree
     // shaking in this case.
     UPB_ASSERT(submsg_table);
 
     // Create proactively to handle the case where it doesn't appear. */
     ent.data.v.val = upb_value_ptr(_upb_Message_New(submsg_table, &d->arena));
@@ -637,18 +642,19 @@
 }
 
 static const char* _upb_Decoder_DecodeToSubMessage(
     upb_Decoder* d, const char* ptr, upb_Message* msg,
     const upb_MiniTableSub* subs, const upb_MiniTableField* field, wireval* val,
     int op) {
   void* mem = UPB_PTR_AT(msg, field->offset, void);
-  int type = field->descriptortype;
+  int type = field->UPB_PRIVATE(descriptortype);
 
   if (UPB_UNLIKELY(op == kUpb_DecodeOp_Enum) &&
-      !_upb_Decoder_CheckEnum(d, ptr, msg, subs[field->submsg_index].subenum,
+      !_upb_Decoder_CheckEnum(d, ptr, msg,
+                              subs[field->UPB_PRIVATE(submsg_index)].subenum,
                               field, val)) {
     return ptr;
   }
 
   /* Set presence if necessary. */
   if (field->presence > 0) {
     _upb_sethas_field(msg, field);
@@ -883,15 +889,15 @@
     /* Fastest case: index into dense fields. */
     goto found;
   }
 
   if (t->dense_below < t->field_count) {
     /* Linear search non-dense fields. Resume scanning from last_field_index
      * since fields are usually in order. */
-    int last = *last_field_index;
+    size_t last = *last_field_index;
     for (idx = last; idx < t->field_count; idx++) {
       if (t->fields[idx].number == field_number) {
         goto found;
       }
     }
 
     for (idx = t->dense_below; idx < last; idx++) {
@@ -947,25 +953,39 @@
       [kUpb_FieldType_SFixed32] = kUpb_DecodeOp_UnknownField,
       [kUpb_FieldType_SFixed64] = kUpb_DecodeOp_UnknownField,
       [kUpb_FieldType_SInt32] = kUpb_DecodeOp_Scalar4Byte,
       [kUpb_FieldType_SInt64] = kUpb_DecodeOp_Scalar8Byte,
       [kUpb_FakeFieldType_MessageSetItem] = kUpb_DecodeOp_UnknownField,
   };
 
-  return kVarintOps[field->descriptortype];
+  return kVarintOps[field->UPB_PRIVATE(descriptortype)];
 }
 
 UPB_FORCEINLINE
 static void _upb_Decoder_CheckUnlinked(const upb_MiniTable* mt,
                                        const upb_MiniTableField* field,
                                        int* op) {
   // If sub-message is not linked, treat as unknown.
   if (field->mode & kUpb_LabelFlags_IsExtension) return;
-  const upb_MiniTableSub* sub = &mt->subs[field->submsg_index];
-  if (!sub->submsg) *op = kUpb_DecodeOp_UnknownField;
+  const upb_MiniTableSub* sub = &mt->subs[field->UPB_PRIVATE(submsg_index)];
+  if (sub->submsg) return;
+#ifndef NDEBUG
+  const upb_MiniTableField* oneof = upb_MiniTable_GetOneof(mt, field);
+  if (oneof) {
+    // All other members of the oneof must be message fields that are also
+    // unlinked.
+    do {
+      assert(upb_MiniTableField_CType(oneof) == kUpb_CType_Message);
+      const upb_MiniTableSub* oneof_sub =
+          &mt->subs[oneof->UPB_PRIVATE(submsg_index)];
+      assert(!oneof_sub);
+    } while (upb_MiniTable_NextOneofField(mt, &oneof));
+  }
+#endif  // NDEBUG
+  *op = kUpb_DecodeOp_UnknownField;
 }
 
 int _upb_Decoder_GetDelimitedOp(const upb_MiniTable* mt,
                                 const upb_MiniTableField* field) {
   enum { kRepeatedBase = 19 };
 
   static const int8_t kDelimitedOps[] = {
@@ -1010,15 +1030,15 @@
       [kRepeatedBase + kUpb_FieldType_SFixed64] = OP_FIXPCK_LG2(3),
       [kRepeatedBase + kUpb_FieldType_SInt32] = OP_VARPCK_LG2(2),
       [kRepeatedBase + kUpb_FieldType_SInt64] = OP_VARPCK_LG2(3),
       // Omitting kUpb_FakeFieldType_MessageSetItem, because we never emit a
       // repeated msgset type
   };
 
-  int ndx = field->descriptortype;
+  int ndx = field->UPB_PRIVATE(descriptortype);
   if (upb_FieldMode_Get(field) == kUpb_FieldMode_Array) ndx += kRepeatedBase;
   int op = kDelimitedOps[ndx];
 
   if (op == kUpb_DecodeOp_SubMessage) {
     _upb_Decoder_CheckUnlinked(mt, field, &op);
   }
 
@@ -1039,38 +1059,39 @@
                                          (1 << kUpb_FieldType_Fixed64) |
                                          (1 << kUpb_FieldType_SFixed64);
 
   switch (wire_type) {
     case kUpb_WireType_Varint:
       ptr = _upb_Decoder_DecodeVarint(d, ptr, &val->uint64_val);
       *op = _upb_Decoder_GetVarintOp(field);
-      _upb_Decoder_Munge(field->descriptortype, val);
+      _upb_Decoder_Munge(field->UPB_PRIVATE(descriptortype), val);
       return ptr;
     case kUpb_WireType_32Bit:
       *op = kUpb_DecodeOp_Scalar4Byte;
-      if (((1 << field->descriptortype) & kFixed32OkMask) == 0) {
+      if (((1 << field->UPB_PRIVATE(descriptortype)) & kFixed32OkMask) == 0) {
         *op = kUpb_DecodeOp_UnknownField;
       }
       return upb_WireReader_ReadFixed32(ptr, &val->uint32_val);
     case kUpb_WireType_64Bit:
       *op = kUpb_DecodeOp_Scalar8Byte;
-      if (((1 << field->descriptortype) & kFixed64OkMask) == 0) {
+      if (((1 << field->UPB_PRIVATE(descriptortype)) & kFixed64OkMask) == 0) {
         *op = kUpb_DecodeOp_UnknownField;
       }
       return upb_WireReader_ReadFixed64(ptr, &val->uint64_val);
     case kUpb_WireType_Delimited:
       ptr = upb_Decoder_DecodeSize(d, ptr, &val->size);
       *op = _upb_Decoder_GetDelimitedOp(mt, field);
       return ptr;
     case kUpb_WireType_StartGroup:
       val->uint32_val = field->number;
-      if (field->descriptortype == kUpb_FieldType_Group) {
+      if (field->UPB_PRIVATE(descriptortype) == kUpb_FieldType_Group) {
         *op = kUpb_DecodeOp_SubMessage;
         _upb_Decoder_CheckUnlinked(mt, field, op);
-      } else if (field->descriptortype == kUpb_FakeFieldType_MessageSetItem) {
+      } else if (field->UPB_PRIVATE(descriptortype) ==
+                 kUpb_FakeFieldType_MessageSetItem) {
         *op = kUpb_DecodeOp_MessageSetItem;
       } else {
         *op = kUpb_DecodeOp_UnknownField;
       }
       return ptr;
     default:
       break;
@@ -1276,40 +1297,47 @@
                                            upb_Arena* const arena) {
   if (UPB_SETJMP(decoder->err) == 0) {
     decoder->status = _upb_Decoder_DecodeTop(decoder, buf, msg, l);
   } else {
     UPB_ASSERT(decoder->status != kUpb_DecodeStatus_Ok);
   }
 
-  arena->head.ptr = decoder->arena.head.ptr;
-  arena->head.end = decoder->arena.head.end;
-  arena->cleanup_metadata = decoder->arena.cleanup_metadata;
+  _upb_MemBlock* blocks =
+      upb_Atomic_Load(&decoder->arena.blocks, memory_order_relaxed);
+  arena->head = decoder->arena.head;
+  upb_Atomic_Store(&arena->blocks, blocks, memory_order_relaxed);
   return decoder->status;
 }
 
 upb_DecodeStatus upb_Decode(const char* buf, size_t size, void* msg,
                             const upb_MiniTable* l,
                             const upb_ExtensionRegistry* extreg, int options,
                             upb_Arena* arena) {
-  upb_Decoder state;
+  upb_Decoder decoder;
   unsigned depth = (unsigned)options >> 16;
 
-  upb_EpsCopyInputStream_Init(&state.input, &buf, size,
+  upb_EpsCopyInputStream_Init(&decoder.input, &buf, size,
                               options & kUpb_DecodeOption_AliasString);
 
-  state.extreg = extreg;
-  state.unknown = NULL;
-  state.depth = depth ? depth : 64;
-  state.end_group = DECODE_NOGROUP;
-  state.options = (uint16_t)options;
-  state.missing_required = false;
-  state.arena.head = arena->head;
-  state.arena.last_size = arena->last_size;
-  state.arena.cleanup_metadata = arena->cleanup_metadata;
-  state.arena.parent = arena;
-  state.status = kUpb_DecodeStatus_Ok;
+  decoder.extreg = extreg;
+  decoder.unknown = NULL;
+  decoder.depth = depth ? depth : kUpb_WireFormat_DefaultDepthLimit;
+  decoder.end_group = DECODE_NOGROUP;
+  decoder.options = (uint16_t)options;
+  decoder.missing_required = false;
+  decoder.status = kUpb_DecodeStatus_Ok;
+
+  // Violating the encapsulation of the arena for performance reasons.
+  // This is a temporary arena that we swap into and swap out of when we are
+  // done.  The temporary arena only needs to be able to handle allocation,
+  // not fuse or free, so it does not need many of the members to be initialized
+  // (particularly parent_or_count).
+  _upb_MemBlock* blocks = upb_Atomic_Load(&arena->blocks, memory_order_relaxed);
+  decoder.arena.head = arena->head;
+  decoder.arena.block_alloc = arena->block_alloc;
+  upb_Atomic_Init(&decoder.arena.blocks, blocks);
 
-  return upb_Decoder_Decode(&state, buf, msg, l, arena);
+  return upb_Decoder_Decode(&decoder, buf, msg, l, arena);
 }
 
 #undef OP_FIXPCK_LG2
 #undef OP_VARPCK_LG2
```

### Comparing `protobuf-4.22.3/upb/wire/decode.h` & `protobuf-4.23.0rc2/upb/wire/decode.h`

 * *Files 12% similar despite different names*

```diff
@@ -62,22 +62,36 @@
    *    not occur in the binary payload, we will never visit it and discover the
    *    incomplete sub-message.  For this reason, this check is only useful for
    *    implemting ParseFromString() semantics.  For MergeFromString(), a
    *    post-parse validation step will always be necessary. */
   kUpb_DecodeOption_CheckRequired = 2,
 };
 
-#define UPB_DECODE_MAXDEPTH(depth) ((depth) << 16)
+UPB_INLINE uint32_t upb_DecodeOptions_MaxDepth(uint16_t depth) {
+  return (uint32_t)depth << 16;
+}
+
+UPB_INLINE uint16_t upb_DecodeOptions_GetMaxDepth(uint32_t options) {
+  return options >> 16;
+}
+
+// Enforce an upper bound on recursion depth.
+UPB_INLINE int upb_Decode_LimitDepth(uint32_t decode_options, uint32_t limit) {
+  uint32_t max_depth = upb_DecodeOptions_GetMaxDepth(decode_options);
+  if (max_depth > limit) max_depth = limit;
+  return upb_DecodeOptions_MaxDepth(max_depth) | (decode_options & 0xffff);
+}
 
 typedef enum {
   kUpb_DecodeStatus_Ok = 0,
-  kUpb_DecodeStatus_Malformed = 1,         // Wire format was corrupt
-  kUpb_DecodeStatus_OutOfMemory = 2,       // Arena alloc failed
-  kUpb_DecodeStatus_BadUtf8 = 3,           // String field had bad UTF-8
-  kUpb_DecodeStatus_MaxDepthExceeded = 4,  // Exceeded UPB_DECODE_MAXDEPTH
+  kUpb_DecodeStatus_Malformed = 1,    // Wire format was corrupt
+  kUpb_DecodeStatus_OutOfMemory = 2,  // Arena alloc failed
+  kUpb_DecodeStatus_BadUtf8 = 3,      // String field had bad UTF-8
+  kUpb_DecodeStatus_MaxDepthExceeded =
+      4,  // Exceeded upb_DecodeOptions_MaxDepth
 
   // kUpb_DecodeOption_CheckRequired failed (see above), but the parse otherwise
   // succeeded.
   kUpb_DecodeStatus_MissingRequired = 5,
 } upb_DecodeStatus;
 
 UPB_API upb_DecodeStatus upb_Decode(const char* buf, size_t size,
```

### Comparing `protobuf-4.22.3/upb/wire/decode_fast.c` & `protobuf-4.23.0rc2/upb/wire/decode_fast.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/wire/decode_fast.h` & `protobuf-4.23.0rc2/upb/wire/decode_fast.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/wire/decode_internal.h` & `protobuf-4.23.0rc2/upb/wire/decode_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/wire/encode.c` & `protobuf-4.23.0rc2/upb/wire/encode.c`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 #include <string.h>
 
 #include "upb/collections/array_internal.h"
 #include "upb/collections/map_sorter_internal.h"
 #include "upb/message/extension_internal.h"
 #include "upb/mini_table/sub_internal.h"
+#include "upb/wire/common.h"
 #include "upb/wire/common_internal.h"
 #include "upb/wire/swap_internal.h"
 #include "upb/wire/types.h"
 
 // Must be last.
 #include "upb/port/def.inc"
 
@@ -222,15 +223,15 @@
   {                                         \
     ctype val = *(ctype*)field_mem;         \
     encode_##type(e, encodeval);            \
     wire_type = wtype;                      \
     break;                                  \
   }
 
-  switch (f->descriptortype) {
+  switch (f->UPB_PRIVATE(descriptortype)) {
     case kUpb_FieldType_Double:
       CASE(double, double, kUpb_WireType_64Bit, val);
     case kUpb_FieldType_Float:
       CASE(float, float, kUpb_WireType_32Bit, val);
     case kUpb_FieldType_Int64:
     case kUpb_FieldType_UInt64:
       CASE(uint64_t, varint, kUpb_WireType_Varint, val);
@@ -258,29 +259,29 @@
       encode_varint(e, view.size);
       wire_type = kUpb_WireType_Delimited;
       break;
     }
     case kUpb_FieldType_Group: {
       size_t size;
       void* submsg = *(void**)field_mem;
-      const upb_MiniTable* subm = subs[f->submsg_index].submsg;
+      const upb_MiniTable* subm = subs[f->UPB_PRIVATE(submsg_index)].submsg;
       if (submsg == NULL) {
         return;
       }
       if (--e->depth == 0) encode_err(e, kUpb_EncodeStatus_MaxDepthExceeded);
       encode_tag(e, f->number, kUpb_WireType_EndGroup);
       encode_message(e, submsg, subm, &size);
       wire_type = kUpb_WireType_StartGroup;
       e->depth++;
       break;
     }
     case kUpb_FieldType_Message: {
       size_t size;
       void* submsg = *(void**)field_mem;
-      const upb_MiniTable* subm = subs[f->submsg_index].submsg;
+      const upb_MiniTable* subm = subs[f->UPB_PRIVATE(submsg_index)].submsg;
       if (submsg == NULL) {
         return;
       }
       if (--e->depth == 0) encode_err(e, kUpb_EncodeStatus_MaxDepthExceeded);
       encode_message(e, submsg, subm, &size);
       encode_varint(e, size);
       wire_type = kUpb_WireType_Delimited;
@@ -317,15 +318,15 @@
       if (tag) encode_varint(e, tag);                                    \
     } while (ptr != start);                                              \
   }                                                                      \
   break;
 
 #define TAG(wire_type) (packed ? 0 : (f->number << 3 | wire_type))
 
-  switch (f->descriptortype) {
+  switch (f->UPB_PRIVATE(descriptortype)) {
     case kUpb_FieldType_Double:
       encode_fixedarray(e, arr, sizeof(double), TAG(kUpb_WireType_64Bit));
       break;
     case kUpb_FieldType_Float:
       encode_fixedarray(e, arr, sizeof(float), TAG(kUpb_WireType_32Bit));
       break;
     case kUpb_FieldType_SFixed64:
@@ -361,30 +362,30 @@
         encode_tag(e, f->number, kUpb_WireType_Delimited);
       } while (ptr != start);
       return;
     }
     case kUpb_FieldType_Group: {
       const void* const* start = _upb_array_constptr(arr);
       const void* const* ptr = start + arr->size;
-      const upb_MiniTable* subm = subs[f->submsg_index].submsg;
+      const upb_MiniTable* subm = subs[f->UPB_PRIVATE(submsg_index)].submsg;
       if (--e->depth == 0) encode_err(e, kUpb_EncodeStatus_MaxDepthExceeded);
       do {
         size_t size;
         ptr--;
         encode_tag(e, f->number, kUpb_WireType_EndGroup);
         encode_message(e, *ptr, subm, &size);
         encode_tag(e, f->number, kUpb_WireType_StartGroup);
       } while (ptr != start);
       e->depth++;
       return;
     }
     case kUpb_FieldType_Message: {
       const void* const* start = _upb_array_constptr(arr);
       const void* const* ptr = start + arr->size;
-      const upb_MiniTable* subm = subs[f->submsg_index].submsg;
+      const upb_MiniTable* subm = subs[f->UPB_PRIVATE(submsg_index)].submsg;
       if (--e->depth == 0) encode_err(e, kUpb_EncodeStatus_MaxDepthExceeded);
       do {
         size_t size;
         ptr--;
         encode_message(e, *ptr, subm, &size);
         encode_varint(e, size);
         encode_tag(e, f->number, kUpb_WireType_Delimited);
@@ -415,22 +416,23 @@
   encode_tag(e, number, kUpb_WireType_Delimited);
 }
 
 static void encode_map(upb_encstate* e, const upb_Message* msg,
                        const upb_MiniTableSub* subs,
                        const upb_MiniTableField* f) {
   const upb_Map* map = *UPB_PTR_AT(msg, f->offset, const upb_Map*);
-  const upb_MiniTable* layout = subs[f->submsg_index].submsg;
+  const upb_MiniTable* layout = subs[f->UPB_PRIVATE(submsg_index)].submsg;
   UPB_ASSERT(layout->field_count == 2);
 
   if (map == NULL) return;
 
   if (e->options & kUpb_EncodeOption_Deterministic) {
     _upb_sortedmap sorted;
-    _upb_mapsorter_pushmap(&e->sorter, layout->fields[0].descriptortype, map,
+    _upb_mapsorter_pushmap(&e->sorter,
+                           layout->fields[0].UPB_PRIVATE(descriptortype), map,
                            &sorted);
     upb_MapEntry ent;
     while (_upb_sortedmap_next(&e->sorter, map, &sorted, &ent)) {
       encode_mapentry(e, f->number, layout, &ent);
     }
     _upb_mapsorter_popmap(&e->sorter, &sorted);
   } else {
@@ -618,13 +620,13 @@
   unsigned depth = (unsigned)options >> 16;
 
   e.status = kUpb_EncodeStatus_Ok;
   e.arena = arena;
   e.buf = NULL;
   e.limit = NULL;
   e.ptr = NULL;
-  e.depth = depth ? depth : 64;
+  e.depth = depth ? depth : kUpb_WireFormat_DefaultDepthLimit;
   e.options = options;
   _upb_mapsorter_init(&e.sorter);
 
   return upb_Encoder_Encode(&e, msg, l, buf, size);
 }
```

### Comparing `protobuf-4.22.3/upb/wire/encode.h` & `protobuf-4.23.0rc2/upb/wire/encode.h`

 * *Files 13% similar despite different names*

```diff
@@ -44,32 +44,45 @@
    * instances of this binary. There are no guarantees across different
    * binary builds.
    *
    * If your proto contains maps, the encoder will need to malloc()/free()
    * memory during encode. */
   kUpb_EncodeOption_Deterministic = 1,
 
-  /* When set, unknown fields are not printed. */
+  // When set, unknown fields are not printed.
   kUpb_EncodeOption_SkipUnknown = 2,
 
-  /* When set, the encode will fail if any required fields are missing. */
+  // When set, the encode will fail if any required fields are missing.
   kUpb_EncodeOption_CheckRequired = 4,
 };
 
-#define UPB_ENCODE_MAXDEPTH(depth) ((depth) << 16)
-
 typedef enum {
   kUpb_EncodeStatus_Ok = 0,
-  kUpb_EncodeStatus_OutOfMemory = 1,       // Arena alloc failed
-  kUpb_EncodeStatus_MaxDepthExceeded = 2,  // Exceeded UPB_ENCODE_MAXDEPTH
+  kUpb_EncodeStatus_OutOfMemory = 1,  // Arena alloc failed
+  kUpb_EncodeStatus_MaxDepthExceeded = 2,
 
   // kUpb_EncodeOption_CheckRequired failed but the parse otherwise succeeded.
   kUpb_EncodeStatus_MissingRequired = 3,
 } upb_EncodeStatus;
 
+UPB_INLINE uint32_t upb_EncodeOptions_MaxDepth(uint16_t depth) {
+  return (uint32_t)depth << 16;
+}
+
+UPB_INLINE uint16_t upb_EncodeOptions_GetMaxDepth(uint32_t options) {
+  return options >> 16;
+}
+
+// Enforce an upper bound on recursion depth.
+UPB_INLINE int upb_Encode_LimitDepth(uint32_t encode_options, uint32_t limit) {
+  uint32_t max_depth = upb_EncodeOptions_GetMaxDepth(encode_options);
+  if (max_depth > limit) max_depth = limit;
+  return upb_EncodeOptions_MaxDepth(max_depth) | (encode_options & 0xffff);
+}
+
 upb_EncodeStatus upb_Encode(const void* msg, const upb_MiniTable* l,
                             int options, upb_Arena* arena, char** buf,
                             size_t* size);
 
 #ifdef __cplusplus
 } /* extern "C" */
 #endif
```

### Comparing `protobuf-4.22.3/upb/wire/eps_copy_input_stream.c` & `protobuf-4.23.0rc2/upb/wire/eps_copy_input_stream.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/wire/eps_copy_input_stream.h` & `protobuf-4.23.0rc2/upb/wire/eps_copy_input_stream.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/wire/reader.c` & `protobuf-4.23.0rc2/upb/wire/reader.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/wire/reader.h` & `protobuf-4.23.0rc2/upb/wire/reader.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/wire/swap_internal.h` & `protobuf-4.23.0rc2/upb/wire/swap_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/upb/wire/types.h` & `protobuf-4.23.0rc2/upb/wire/types.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/utf8_range/naive.c` & `protobuf-4.23.0rc2/utf8_range/naive.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/utf8_range/range2-neon.c` & `protobuf-4.23.0rc2/utf8_range/range2-neon.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/utf8_range/range2-sse.c` & `protobuf-4.23.0rc2/utf8_range/range2-sse.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.22.3/utf8_range/utf8_range.h` & `protobuf-4.23.0rc2/utf8_range/utf8_range.h`

 * *Files identical despite different names*

