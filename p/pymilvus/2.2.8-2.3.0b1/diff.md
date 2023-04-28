# Comparing `tmp/pymilvus-2.2.8.tar.gz` & `tmp/pymilvus-2.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilvus-2.2.8.tar", last modified: Fri Apr 28 13:20:13 2023, max compression
+gzip compressed data, was "pymilvus-2.3.0b1.tar", last modified: Mon Mar 20 10:23:59 2023, max compression
```

## Comparing `pymilvus-2.2.8.tar` & `pymilvus-2.3.0b1.tar`

### file list

```diff
@@ -1,167 +1,163 @@
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.607744 pymilvus-2.2.8/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      246 2023-04-21 10:31:04.000000 pymilvus-2.2.8/.env.example
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.591745 pymilvus-2.2.8/.github/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.591745 pymilvus-2.2.8/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2045 2022-11-09 07:08:42.000000 pymilvus-2.2.8/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       27 2022-11-09 07:08:42.000000 pymilvus-2.2.8/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1371 2022-11-09 07:08:42.000000 pymilvus-2.2.8/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      633 2022-11-09 07:08:42.000000 pymilvus-2.2.8/.github/ISSUE_TEMPLATE/general-question.yaml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      817 2023-04-28 13:19:22.000000 pymilvus-2.2.8/.github/mergify.yml
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.591745 pymilvus-2.2.8/.github/workflows/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      730 2023-04-28 13:19:22.000000 pymilvus-2.2.8/.github/workflows/check_milvus_proto.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      685 2023-04-28 13:19:22.000000 pymilvus-2.2.8/.github/workflows/code_checker.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      919 2022-11-09 07:08:42.000000 pymilvus-2.2.8/.github/workflows/doc_update_event.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2046 2023-04-25 03:52:33.000000 pymilvus-2.2.8/.github/workflows/nightly_ci.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1067 2023-04-28 13:19:22.000000 pymilvus-2.2.8/.github/workflows/publish_dev_package.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      783 2023-04-28 13:19:22.000000 pymilvus-2.2.8/.github/workflows/pull_request.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      778 2022-11-21 06:54:31.000000 pymilvus-2.2.8/.github/workflows/release_event.yml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      264 2022-11-09 07:08:42.000000 pymilvus-2.2.8/.gitignore
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      137 2023-04-26 09:00:09.000000 pymilvus-2.2.8/.gitmodules
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4996 2022-11-09 07:08:42.000000 pymilvus-2.2.8/CONTRIBUTING.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4620 2022-11-09 07:08:42.000000 pymilvus-2.2.8/CONTRIBUTING_CN.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       77 2022-11-09 07:08:42.000000 pymilvus-2.2.8/Dockerfile
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11336 2023-04-10 06:47:08.000000 pymilvus-2.2.8/LICENSE
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      552 2022-12-06 08:37:06.000000 pymilvus-2.2.8/Makefile
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      176 2022-11-09 07:08:42.000000 pymilvus-2.2.8/OWNERS
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3916 2023-04-28 13:20:13.607744 pymilvus-2.2.8/PKG-INFO
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3369 2023-04-28 13:19:22.000000 pymilvus-2.2.8/README.md
--rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     1306 2023-04-13 09:37:10.000000 pymilvus-2.2.8/check_proto_product.sh
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.583746 pymilvus-2.2.8/ci/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.583746 pymilvus-2.2.8/ci/docker/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.595745 pymilvus-2.2.8/ci/docker/milvus/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1169 2022-11-09 07:08:42.000000 pymilvus-2.2.8/ci/docker/milvus/docker-compose.yml
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.595745 pymilvus-2.2.8/ci/scripts/
--rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     7597 2022-11-09 07:08:42.000000 pymilvus-2.2.8/ci/scripts/docker_image_find_tag.sh
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.595745 pymilvus-2.2.8/docs/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      638 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/Makefile
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1858 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/README.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      799 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/make.bat
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.595745 pymilvus-2.2.8/docs/source/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.595745 pymilvus-2.2.8/docs/source/_templates/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       97 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/_templates/autosummaryclass.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      389 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/_templates/layout.html
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      122 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/about.rst
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.595745 pymilvus-2.2.8/docs/source/api/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      169 2023-04-13 09:37:10.000000 pymilvus-2.2.8/docs/source/api/api.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8038 2023-04-28 13:19:22.000000 pymilvus-2.2.8/docs/source/api/collection.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3644 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/api/connections.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2580 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/api/future.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2122 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/api/milvus_index.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4010 2023-04-28 13:19:22.000000 pymilvus-2.2.8/docs/source/api/partition.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3199 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/api/schema.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4749 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/api/search.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7557 2023-04-13 09:37:10.000000 pymilvus-2.2.8/docs/source/api/utility.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       24 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/changes.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3236 2023-04-13 09:37:10.000000 pymilvus-2.2.8/docs/source/conf.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3255 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/contribute.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      575 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/faq.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      931 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/index.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2115 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/install.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       60 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/param.rst
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.595745 pymilvus-2.2.8/docs/source/res/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     9091 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/res/Intro_to_Indexes.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      544 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/res/about_documentation.md
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1448 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/results.rst
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7429 2022-11-09 07:08:42.000000 pymilvus-2.2.8/docs/source/tutorial.rst
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.599745 pymilvus-2.2.8/examples/
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.599745 pymilvus-2.2.8/examples/cert/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1326 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/cert/ca.pem
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1704 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/cert/client.key
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/cert/client.pem
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/cert/server.pem
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11523 2023-04-28 13:19:22.000000 pymilvus-2.2.8/examples/collection.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4302 2023-04-13 09:37:10.000000 pymilvus-2.2.8/examples/example.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    15138 2023-04-13 09:37:10.000000 pymilvus-2.2.8/examples/example_bulkinsert.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5512 2023-04-13 09:37:10.000000 pymilvus-2.2.8/examples/example_index.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4437 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/example_str.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4120 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/example_tls1.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4230 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/example_tls2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)  1070736 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/films.csv
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    12007 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/hello_milvus.ipynb
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7380 2023-04-25 12:01:18.000000 pymilvus-2.2.8/examples/hello_milvus.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2690 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/multithreading_hello_milvus.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3452 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/old_style_example.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5612 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/old_style_example_index.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3779 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/old_style_example_str.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1874 2022-11-09 07:08:42.000000 pymilvus-2.2.8/examples/old_style_query.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4676 2023-04-13 09:37:10.000000 pymilvus-2.2.8/examples/partition.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2977 2023-04-28 13:19:22.000000 pymilvus-2.2.8/examples/resource_group.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7110 2023-04-28 13:19:22.000000 pymilvus-2.2.8/examples/role_and_privilege.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3310 2023-04-13 09:37:10.000000 pymilvus-2.2.8/examples/user.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    19554 2023-04-13 09:37:10.000000 pymilvus-2.2.8/pylint.conf
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.599745 pymilvus-2.2.8/pymilvus/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3232 2023-04-21 10:31:04.000000 pymilvus-2.2.8/pymilvus/__init__.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.603744 pymilvus-2.2.8/pymilvus/client/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1790 2023-04-13 09:37:10.000000 pymilvus-2.2.8/pymilvus/client/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    28573 2023-04-21 10:31:04.000000 pymilvus-2.2.8/pymilvus/client/abstract.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    10675 2023-04-13 09:37:10.000000 pymilvus-2.2.8/pymilvus/client/asynch.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      738 2023-04-13 09:37:10.000000 pymilvus-2.2.8/pymilvus/client/blob.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11884 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/client/check.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      283 2023-04-21 10:31:04.000000 pymilvus-2.2.8/pymilvus/client/constants.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3106 2023-04-21 10:31:04.000000 pymilvus-2.2.8/pymilvus/client/entity_helper.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    59785 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/client/grpc_handler.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3522 2023-04-13 09:37:10.000000 pymilvus-2.2.8/pymilvus/client/interceptor.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    39969 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/client/prepare.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      355 2023-04-13 09:37:10.000000 pymilvus-2.2.8/pymilvus/client/singleton_utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    58590 2023-04-26 09:00:19.000000 pymilvus-2.2.8/pymilvus/client/stub.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2812 2023-04-13 09:37:10.000000 pymilvus-2.2.8/pymilvus/client/ts_utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    19531 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/client/types.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4928 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/client/utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6414 2023-04-13 09:37:10.000000 pymilvus-2.2.8/pymilvus/decorators.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6265 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/exceptions.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.603744 pymilvus-2.2.8/pymilvus/grpc_gen/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      116 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/grpc_gen/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    13701 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/grpc_gen/common_pb2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11992 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/grpc_gen/common_pb2.pyi
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    67228 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/grpc_gen/milvus_pb2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    83171 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/grpc_gen/milvus_pb2.pyi
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)   116220 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/grpc_gen/milvus_pb2_grpc.py
--rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     1356 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/grpc_gen/python_gen.sh
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5774 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/grpc_gen/schema_pb2.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7923 2023-04-26 09:00:09.000000 pymilvus-2.2.8/pymilvus/grpc_gen/schema_pb2.pyi
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.607744 pymilvus-2.2.8/pymilvus/orm/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      593 2022-11-09 07:08:42.000000 pymilvus-2.2.8/pymilvus/orm/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    50045 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/orm/collection.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    16262 2023-04-21 10:31:04.000000 pymilvus-2.2.8/pymilvus/orm/connections.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      909 2023-04-13 09:37:10.000000 pymilvus-2.2.8/pymilvus/orm/constants.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1553 2022-11-09 07:08:42.000000 pymilvus-2.2.8/pymilvus/orm/future.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5650 2023-04-21 10:31:04.000000 pymilvus-2.2.8/pymilvus/orm/index.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1887 2023-04-13 09:37:10.000000 pymilvus-2.2.8/pymilvus/orm/mutation.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    23037 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/orm/partition.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3482 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/orm/prepare.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8327 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/orm/role.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14632 2023-04-28 13:19:22.000000 pymilvus-2.2.8/pymilvus/orm/schema.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7437 2023-04-21 10:31:04.000000 pymilvus-2.2.8/pymilvus/orm/search.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4318 2023-04-13 09:37:10.000000 pymilvus-2.2.8/pymilvus/orm/types.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    47584 2023-04-26 09:00:19.000000 pymilvus-2.2.8/pymilvus/orm/utility.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2554 2023-04-26 09:00:19.000000 pymilvus-2.2.8/pymilvus/settings.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.599745 pymilvus-2.2.8/pymilvus.egg-info/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3916 2023-04-28 13:20:13.000000 pymilvus-2.2.8/pymilvus.egg-info/PKG-INFO
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3718 2023-04-28 13:20:13.000000 pymilvus-2.2.8/pymilvus.egg-info/SOURCES.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        1 2023-04-28 13:20:13.000000 pymilvus-2.2.8/pymilvus.egg-info/dependency_links.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       84 2023-04-28 13:20:13.000000 pymilvus-2.2.8/pymilvus.egg-info/requires.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        9 2023-04-28 13:20:13.000000 pymilvus-2.2.8/pymilvus.egg-info/top_level.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      118 2022-11-09 07:08:42.000000 pymilvus-2.2.8/pyproject.toml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      607 2023-04-28 13:19:22.000000 pymilvus-2.2.8/requirements.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       38 2023-04-28 13:20:13.607744 pymilvus-2.2.8/setup.cfg
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1103 2023-04-21 10:31:04.000000 pymilvus-2.2.8/setup.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       97 2023-04-21 10:31:04.000000 pymilvus-2.2.8/test_requirements.txt
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-04-28 13:20:13.607744 pymilvus-2.2.8/tests/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      830 2023-03-17 10:50:05.000000 pymilvus-2.2.8/tests/conftest.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8443 2023-03-17 10:50:05.000000 pymilvus-2.2.8/tests/mock_milvus.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      570 2023-03-17 10:50:05.000000 pymilvus-2.2.8/tests/mock_result.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      275 2022-11-09 07:08:42.000000 pymilvus-2.2.8/tests/pytest.ini
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5828 2023-04-13 09:37:10.000000 pymilvus-2.2.8/tests/test_check.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6200 2023-04-21 06:48:11.000000 pymilvus-2.2.8/tests/test_collection.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14630 2023-04-21 10:31:04.000000 pymilvus-2.2.8/tests/test_connections.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4283 2023-03-17 10:50:05.000000 pymilvus-2.2.8/tests/test_create_collection.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6114 2023-04-13 09:37:10.000000 pymilvus-2.2.8/tests/test_decorators.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5529 2023-04-13 09:37:10.000000 pymilvus-2.2.8/tests/test_grpc_handler.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1557 2023-04-13 09:37:10.000000 pymilvus-2.2.8/tests/test_index.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2768 2023-04-13 09:37:10.000000 pymilvus-2.2.8/tests/test_partition.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4472 2023-04-21 10:31:04.000000 pymilvus-2.2.8/tests/test_prepare.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6417 2023-04-28 13:19:22.000000 pymilvus-2.2.8/tests/test_schema.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1201 2023-03-17 10:50:05.000000 pymilvus-2.2.8/tests/test_ts_utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4548 2023-04-21 10:31:04.000000 pymilvus-2.2.8/tests/test_types.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      423 2023-04-28 13:19:22.000000 pymilvus-2.2.8/tests/test_utils.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4810 2023-03-17 10:50:05.000000 pymilvus-2.2.8/tests/utils.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.260630 pymilvus-2.3.0b1/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/.github/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2045 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       27 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1371 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      633 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/general-question.yaml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      823 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/mergify.yml
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/.github/workflows/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      733 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/workflows/check_milvus_proto.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      596 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/workflows/code_checker.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      919 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/workflows/doc_update_event.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2046 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.github/workflows/nightly_ci.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1067 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/workflows/publish_dev_package.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      747 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/.github/workflows/pull_request.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      778 2022-11-21 06:54:31.000000 pymilvus-2.3.0b1/.github/workflows/release_event.yml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      264 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/.gitignore
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      137 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/.gitmodules
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4996 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/CONTRIBUTING.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4620 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/CONTRIBUTING_CN.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       77 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/Dockerfile
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11336 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/LICENSE
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      552 2022-12-06 08:37:06.000000 pymilvus-2.3.0b1/Makefile
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      176 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/OWNERS
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3816 2023-03-20 10:23:59.260630 pymilvus-2.3.0b1/PKG-INFO
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3369 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/README.md
+-rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     1306 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/check_proto_product.sh
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.240631 pymilvus-2.3.0b1/ci/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.240631 pymilvus-2.3.0b1/ci/docker/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/ci/docker/milvus/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1169 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/ci/docker/milvus/docker-compose.yml
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/ci/scripts/
+-rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)     7597 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/ci/scripts/docker_image_find_tag.sh
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.244631 pymilvus-2.3.0b1/docs/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      638 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/Makefile
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1858 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/README.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      799 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/make.bat
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.248631 pymilvus-2.3.0b1/docs/source/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.248631 pymilvus-2.3.0b1/docs/source/_templates/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       97 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/_templates/autosummaryclass.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      389 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/_templates/layout.html
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      122 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/about.rst
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.248631 pymilvus-2.3.0b1/docs/source/api/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      169 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/docs/source/api/api.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8339 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/docs/source/api/collection.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3644 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/connections.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2580 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/future.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2122 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/milvus_index.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4253 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/docs/source/api/partition.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3199 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/schema.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4749 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/api/search.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7557 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/docs/source/api/utility.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       24 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/changes.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3236 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/docs/source/conf.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3255 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/contribute.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      575 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/faq.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      931 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/index.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2115 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/install.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       60 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/param.rst
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.248631 pymilvus-2.3.0b1/docs/source/res/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     9091 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/res/Intro_to_Indexes.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      544 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/res/about_documentation.md
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1448 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/results.rst
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7429 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/docs/source/tutorial.rst
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.252630 pymilvus-2.3.0b1/examples/
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.252630 pymilvus-2.3.0b1/examples/cert/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1326 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/cert/ca.pem
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1704 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/cert/client.key
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/cert/client.pem
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1289 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/cert/server.pem
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11469 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/examples/collection.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4302 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/examples/example.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    15138 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/examples/example_bulkinsert.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5512 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/examples/example_index.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4437 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/example_str.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4120 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/example_tls1.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4230 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/example_tls2.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)  1070736 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/films.csv
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    12007 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/hello_milvus.ipynb
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7380 2023-02-20 09:16:24.000000 pymilvus-2.3.0b1/examples/hello_milvus.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2690 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/multithreading_hello_milvus.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3452 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/old_style_example.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5612 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/old_style_example_index.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3779 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/old_style_example_str.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1874 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/examples/old_style_query.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4676 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/examples/partition.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2701 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/examples/resource_group.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6680 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/examples/role_and_privilege.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3310 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/examples/user.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    19554 2023-02-09 06:48:27.000000 pymilvus-2.3.0b1/pylint.conf
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.252630 pymilvus-2.3.0b1/pymilvus/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3188 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/__init__.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.256630 pymilvus-2.3.0b1/pymilvus/client/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1790 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/__init__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    28616 2023-02-08 07:36:14.000000 pymilvus-2.3.0b1/pymilvus/client/abstract.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    10675 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/asynch.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      738 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/blob.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11932 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/client/check.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      242 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/configs.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      200 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/pymilvus/client/constants.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3144 2023-03-17 10:58:42.000000 pymilvus-2.3.0b1/pymilvus/client/entity_helper.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    59059 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/client/grpc_handler.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3522 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/interceptor.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    37767 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/client/prepare.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      355 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/singleton_utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    58555 2023-02-09 06:48:27.000000 pymilvus-2.3.0b1/pymilvus/client/stub.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2781 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/client/ts_utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    19426 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/client/types.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6421 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/client/utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6414 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/pymilvus/decorators.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6423 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/exceptions.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.256630 pymilvus-2.3.0b1/pymilvus/grpc_gen/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      116 2023-03-17 10:56:09.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/__init__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    23471 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/common_pb2.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)   120931 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/milvus_pb2.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)   109919 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/milvus_pb2_grpc.py
+-rwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)      967 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/python_gen.sh
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    10854 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/grpc_gen/schema_pb2.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.256630 pymilvus-2.3.0b1/pymilvus/orm/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      593 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/pymilvus/orm/__init__.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    52636 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/orm/collection.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14956 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/orm/connections.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      909 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/pymilvus/orm/constants.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      842 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/orm/default_config.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1553 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/pymilvus/orm/future.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5680 2023-03-01 03:03:27.000000 pymilvus-2.3.0b1/pymilvus/orm/index.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1887 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/orm/mutation.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    28312 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/orm/partition.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3691 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/orm/prepare.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7911 2023-03-01 03:03:27.000000 pymilvus-2.3.0b1/pymilvus/orm/role.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    14893 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/pymilvus/orm/schema.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7478 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/orm/search.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4318 2022-12-07 08:12:46.000000 pymilvus-2.3.0b1/pymilvus/orm/types.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    44273 2023-03-01 06:24:25.000000 pymilvus-2.3.0b1/pymilvus/orm/utility.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1926 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/pymilvus/settings.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.252630 pymilvus-2.3.0b1/pymilvus.egg-info/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3816 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/PKG-INFO
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3622 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/SOURCES.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        1 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/dependency_links.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      175 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/requires.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        9 2023-03-20 10:23:59.000000 pymilvus-2.3.0b1/pymilvus.egg-info/top_level.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      118 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/pyproject.toml
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      617 2023-03-20 10:23:12.000000 pymilvus-2.3.0b1/requirements.txt
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       38 2023-03-20 10:23:59.260630 pymilvus-2.3.0b1/setup.cfg
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1096 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/setup.py
+drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2023-03-20 10:23:59.260630 pymilvus-2.3.0b1/tests/
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      830 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/conftest.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8443 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/mock_milvus.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      570 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/mock_result.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      275 2022-11-09 07:08:42.000000 pymilvus-2.3.0b1/tests/pytest.ini
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5828 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_check.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6200 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_collection.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    13787 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_connections.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4283 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_create_collection.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6114 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_decorators.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4163 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_grpc_handler.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1557 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_index.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2768 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_partition.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4490 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_prepare.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     5437 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_schema.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1201 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_ts_utils.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4292 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/test_types.py
+-rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4810 2023-03-17 10:50:05.000000 pymilvus-2.3.0b1/tests/utils.py
```

### Comparing `pymilvus-2.2.8/.github/ISSUE_TEMPLATE/bug_report.yaml` & `pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/.github/ISSUE_TEMPLATE/feature_request.yaml` & `pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/.github/ISSUE_TEMPLATE/general-question.yaml` & `pymilvus-2.3.0b1/.github/ISSUE_TEMPLATE/general-question.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/.github/mergify.yml` & `pymilvus-2.3.0b1/.github/mergify.yml`

 * *Files 3% similar despite different names*

```diff
@@ -11,28 +11,28 @@
       label:
         add:
           - ci-passed
   - name: Add needs-dco label when DCO check failed
     conditions:
       - or:
         - base=master
-        - base=2.0
+        - base~=2\.\d
       - -status-success=DCO
     actions:
       label:
         remove:
           - dco-passed
         add:
           - needs-dco
 
   - name: Add dco-passed label when DCO check passed
     conditions:
       - or:
         - base=master
-        - base=2.0
+        - base~=2\.\d
       - status-success=DCO
     actions:
       label:
         remove:
           - needs-dco
         add:
           - dco-passed
```

### Comparing `pymilvus-2.2.8/.github/workflows/check_milvus_proto.yml` & `pymilvus-2.3.0b1/.github/workflows/check_milvus_proto.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Check proto on pull request
 
 on:
   pull_request:
     branches:
-      - 2.2
+      - master
 
 jobs:
   build:
     name: Run Check Proto
     runs-on: ubuntu-latest
     strategy:
       matrix:
```

### Comparing `pymilvus-2.2.8/.github/workflows/code_checker.yml` & `pymilvus-2.3.0b1/.github/workflows/pull_request.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-name: Code checker on pull request
+name: Test on pull request
 
 on:
   pull_request:
     branches:
-      - 2.2
+      - master
 
 jobs:
-  code-lint:
-    name: Code lint check
+  build:
+    name: Run Python Tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.8, 3.11]
+        python-version: [3.8]
+
     steps:
-      - name: Checkout code
-        uses: actions/checkout@v2
-      - name: Set up python
-        uses: actions/setup-python@v2
-        with:
-          python-version: ${{ matrix.python-version }}
-      - name: check setup.py install
-        run: |
-          python setup.py install
-      - name: Install requirements
-        run: |
-          pip install -r requirements.txt
-      - name: Run pylint
-        shell: bash
-        run: |
-          make lint
+    - uses: actions/checkout@v2
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v2
+      with:
+        python-version: ${{ matrix.python-version }}
+
+    - name: Fetch tags
+      run: |
+        git fetch --prune --unshallow --tags
+
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        pip install pytest
+        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+
+    - name: Test with pytest
+      run: |
+        make unittest
```

### Comparing `pymilvus-2.2.8/.github/workflows/doc_update_event.yml` & `pymilvus-2.3.0b1/.github/workflows/doc_update_event.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/.github/workflows/nightly_ci.yml` & `pymilvus-2.3.0b1/.github/workflows/nightly_ci.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/.github/workflows/pull_request.yml` & `pymilvus-2.3.0b1/.github/workflows/code_checker.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-name: Test on pull request
+name: Code checker on pull request
 
 on:
   pull_request:
     branches:
-      - 2.2
+      - master
 
 jobs:
-  build:
-    name: Run Python Tests
+  code-lint:
+    name: Code lint check
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.8, 3.11]
-
+        python-version: [3.8]
     steps:
       - name: Checkout code
         uses: actions/checkout@v2
-      - name: Set up Python ${{ matrix.python-version }}
+      - name: Set up python
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
-
-      - name: Fetch tags
+      - name: Install requirements
         run: |
-          git fetch --prune --unshallow --tags
-
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          python setup.py install
-          pip install -r test_requirements.txt
-
-      - name: Test with pytest
+          pip install -r requirements.txt
+      - name: Run pylint
+        shell: bash
         run: |
-          make unittest
+          make lint
```

### Comparing `pymilvus-2.2.8/.github/workflows/release_event.yml` & `pymilvus-2.3.0b1/.github/workflows/release_event.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/CONTRIBUTING.md` & `pymilvus-2.3.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/CONTRIBUTING_CN.md` & `pymilvus-2.3.0b1/CONTRIBUTING_CN.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/LICENSE` & `pymilvus-2.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/Makefile` & `pymilvus-2.3.0b1/Makefile`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/PKG-INFO` & `pymilvus-2.3.0b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: pymilvus
-Version: 2.2.8
+Version: 2.3.0b1
 Summary: Python Sdk for Milvus
 Home-page: https://github.com/milvus-io/pymilvus
 Author: Milvus Team
 Author-email: milvus-team@zilliz.com
 License: Apache-2.0
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Milvus Python SDK
 
 [![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
```

### Comparing `pymilvus-2.2.8/README.md` & `pymilvus-2.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/check_proto_product.sh` & `pymilvus-2.3.0b1/check_proto_product.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/ci/docker/milvus/docker-compose.yml` & `pymilvus-2.3.0b1/ci/docker/milvus/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/ci/scripts/docker_image_find_tag.sh` & `pymilvus-2.3.0b1/ci/scripts/docker_image_find_tag.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/Makefile` & `pymilvus-2.3.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/README.md` & `pymilvus-2.3.0b1/docs/README.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/make.bat` & `pymilvus-2.3.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/api/collection.rst` & `pymilvus-2.3.0b1/docs/source/api/collection.rst`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `insert() <#pymilvus.Collection.insert>`_                     | Insert data into collection.                                             |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `delete() <#pymilvus.Collection.delete>`_                     | Delete entities with an expression condition.                            |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `search() <#pymilvus.Collection.search>`_                     | Vector similarity search with an optional boolean expression as filters. |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
+| `upsert() <#pymilvus.Collection.upsert>`_                     | Upsert data of collection.                                                                  |
++---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `query() <#pymilvus.Collection.query>`_                       | Query with a set of criteria.                                            |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `partition() <#pymilvus.Collection.partition>`_               | Return the partition corresponding to name.                              |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `create_partition() <#pymilvus.Collection.create_partition>`_ | Create the partition for the collection.                                 |
 +---------------------------------------------------------------+--------------------------------------------------------------------------+
 | `has_partition() <#pymilvus.Collection.has_partition>`_       | Checks if a specified partition exists.                                  |
```

### Comparing `pymilvus-2.2.8/docs/source/api/connections.rst` & `pymilvus-2.3.0b1/docs/source/api/connections.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/api/future.rst` & `pymilvus-2.3.0b1/docs/source/api/future.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/api/milvus_index.rst` & `pymilvus-2.3.0b1/docs/source/api/milvus_index.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/api/partition.rst` & `pymilvus-2.3.0b1/docs/source/api/partition.rst`

 * *Files 15% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 +--------------------------------------------+--------------------------------------------------------------------------+
 | `release() <#pymilvus.Partition.release>`_ | Release the Partition from memory.                                       |
 +--------------------------------------------+--------------------------------------------------------------------------+
 | `insert() <#pymilvus.Partition.insert>`_   | Insert data into partition.                                              |
 +--------------------------------------------+--------------------------------------------------------------------------+
 | `delete() <#pymilvus.Partition.delete>`_   | Delete entities with an expression condition.                            |
 +--------------------------------------------+--------------------------------------------------------------------------+
+| `upsert() <#pymilvus.Collection.upsert>`_  |Upsert data of collection.                                               |
++--------------------------------------------+--------------------------------------------------------------------------+
 | `search() <#pymilvus.Partition.search>`_   | Vector similarity search with an optional boolean expression as filters. |
 +--------------------------------------------+--------------------------------------------------------------------------+
 | `query() <#pymilvus.Partition.query>`_     | Query with a set of criteria.                                            |
 +--------------------------------------------+--------------------------------------------------------------------------+
 
 API Refereences
 ---------------
```

### Comparing `pymilvus-2.2.8/docs/source/api/schema.rst` & `pymilvus-2.3.0b1/docs/source/api/schema.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/api/search.rst` & `pymilvus-2.3.0b1/docs/source/api/search.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/api/utility.rst` & `pymilvus-2.3.0b1/docs/source/api/utility.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/conf.py` & `pymilvus-2.3.0b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/contribute.rst` & `pymilvus-2.3.0b1/docs/source/contribute.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/faq.rst` & `pymilvus-2.3.0b1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/index.rst` & `pymilvus-2.3.0b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/install.rst` & `pymilvus-2.3.0b1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/res/Intro_to_Indexes.md` & `pymilvus-2.3.0b1/docs/source/res/Intro_to_Indexes.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/res/about_documentation.md` & `pymilvus-2.3.0b1/docs/source/res/about_documentation.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/results.rst` & `pymilvus-2.3.0b1/docs/source/results.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/docs/source/tutorial.rst` & `pymilvus-2.3.0b1/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/cert/ca.pem` & `pymilvus-2.3.0b1/examples/cert/ca.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/cert/client.key` & `pymilvus-2.3.0b1/examples/cert/client.key`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/cert/client.pem` & `pymilvus-2.3.0b1/examples/cert/client.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/cert/server.pem` & `pymilvus-2.3.0b1/examples/cert/server.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/collection.py` & `pymilvus-2.3.0b1/examples/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,14 @@
 
     print("\nlist collections:")
     print(utility.list_collections())
     assert utility.has_collection(old_collection)
 
     utility.rename_collection(old_collection, new_collection)
     assert utility.has_collection(new_collection)
-    assert not utility.has_collection(old_collection)
 
 
 if __name__ == "__main__":
     print("test collection and get an existing collection")
     name = test_create_collection()
     print("test an existing collection")
     test_exist_collection(name)
```

### Comparing `pymilvus-2.2.8/examples/example.py` & `pymilvus-2.3.0b1/examples/example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/example_bulkinsert.py` & `pymilvus-2.3.0b1/examples/example_bulkinsert.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/example_index.py` & `pymilvus-2.3.0b1/examples/example_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/example_str.py` & `pymilvus-2.3.0b1/examples/example_str.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/example_tls1.py` & `pymilvus-2.3.0b1/examples/example_tls1.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/example_tls2.py` & `pymilvus-2.3.0b1/examples/example_tls2.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/films.csv` & `pymilvus-2.3.0b1/examples/films.csv`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/hello_milvus.ipynb` & `pymilvus-2.3.0b1/examples/hello_milvus.ipynb`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/hello_milvus.py` & `pymilvus-2.3.0b1/examples/hello_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/multithreading_hello_milvus.py` & `pymilvus-2.3.0b1/examples/multithreading_hello_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/old_style_example.py` & `pymilvus-2.3.0b1/examples/old_style_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/old_style_example_index.py` & `pymilvus-2.3.0b1/examples/old_style_example_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/old_style_example_str.py` & `pymilvus-2.3.0b1/examples/old_style_example_str.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/old_style_query.py` & `pymilvus-2.3.0b1/examples/old_style_query.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/partition.py` & `pymilvus-2.3.0b1/examples/partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/examples/resource_group.py` & `pymilvus-2.3.0b1/examples/resource_group.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,22 +49,20 @@
 
 def transfer_replica(source, target, collection_name, num_replica):
     print(
         f"transfer {num_replica} replicas in {collection_name} from {source} to {target}")
     utility.transfer_replica(
         source, target, collection_name, num_replica, using=_CONNECTION_NAME)
     
-
 def run(): 
     create_connection("root", "123456")
     coll = create_collection(_COLLECTION_NAME, _ID_FIELD_NAME, _VECTOR_FIELD_NAME)
     vectors = insert(coll, 10000, _DIM)
     coll.flush()
     create_index(coll, _VECTOR_FIELD_NAME)
-    load_collection(coll)
     
     create_resource_group("rg")
     list_resource_groups()
     describe_resource_group("rg")
     transfer_node(DEFAULT_RESOURCE_GROUP, "rg", 1)
     describe_resource_group(DEFAULT_RESOURCE_GROUP)
     describe_resource_group("rg")
@@ -76,20 +74,14 @@
     describe_resource_group(DEFAULT_RESOURCE_GROUP)
     describe_resource_group("rg")
     
     describe_resource_group(DEFAULT_RESOURCE_GROUP)
     describe_resource_group("rg")
     transfer_replica("rg", DEFAULT_RESOURCE_GROUP, _COLLECTION_NAME, 1)
     describe_resource_group(DEFAULT_RESOURCE_GROUP)
-    describe_resource_group("rg")
-    
-    describe_resource_group(DEFAULT_RESOURCE_GROUP)
-    describe_resource_group("rg")
-    transfer_replica("rg", DEFAULT_RESOURCE_GROUP, _COLLECTION_NAME, 1)
-    describe_resource_group(DEFAULT_RESOURCE_GROUP)
     describe_resource_group("rg")
    
     drop_resource_group("rg")
     release_collection(coll)
     drop_collection(_COLLECTION_NAME)
 
 if __name__ == "__main__":
```

### Comparing `pymilvus-2.2.8/examples/role_and_privilege.py` & `pymilvus-2.3.0b1/examples/role_and_privilege.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 from pymilvus.orm.role import Role
 
 import random
 from sklearn import preprocessing
 
 _CONNECTION = "demo"
 _FOO_CONNECTION = "foo_connection"
-_DB_NAME = "foo_db"
 _HOST = '127.0.0.1'
 _PORT = '19530'
 _ROOT = "root"
 _ROOT_PASSWORD = "Milvus"
 _COLLECTION_NAME = "foocol2"
 
 
-def connect_to_milvus(connection=_CONNECTION, user=_ROOT, password=_ROOT_PASSWORD, db_name="default"):
+def connect_to_milvus(connection=_CONNECTION, user=_ROOT, password=_ROOT_PASSWORD):
     print(f"connect to milvus\n")
     connections.connect(alias=connection,
                         host=_HOST,
                         port=_PORT,
                         user=user,
                         password=password,
-                        db_name=db_name,
                         )
 
 
 def create_credential(user, password, connection=_CONNECTION):
     print(f"create credential, user: {user}, password: {password}")
     utility.create_user(user, password, using=connection)
     print(f"create credential down\n")
@@ -131,17 +129,17 @@
     try:
         select_all_user(connection=connection)
     except Exception as e:
         print(e)
         is_exception = True
     assert is_exception
     role = Role(role_name, using=_CONNECTION)
-    role.grant("User", "*", "SelectUser", db_name=_DB_NAME)
+    role.grant("User", "*", "SelectUser")
     print(select_all_user(connection))
-    role.revoke("User", "*", "SelectUser", db_name=_DB_NAME)
+    role.revoke("User", "*", "SelectUser")
 
 
 def role_example():
     role_name = "role_test5"
     role = Role(role_name, using=_CONNECTION)
     print(f"create role, role_name: {role_name}")
     role.create()
@@ -180,39 +178,34 @@
     create_credential(username, password)
     role = Role(role_name, using=_CONNECTION)
     print(f"create role, role_name: {role_name}")
     role.create()
     print(f"add user")
     role.add_user(username)
     print(f"grant privilege")
-    role.grant("Global", "*", privilege_create, db_name=_DB_NAME)
-    role.grant("Collection", object_name, privilege_insert, db_name=_DB_NAME)
-    # role.grant("Collection", object_name, "*", db_name=_DB_NAME)
-    # role.grant("Collection", "*", privilege_insert, db_name=_DB_NAME)
-
-    print(f"list grants")
-    print(role.list_grants(db_name=_DB_NAME))
-    print(f"list grant")
-    print(role.list_grant("Collection", object_name, db_name=_DB_NAME))
+    role.grant("Global", "*", privilege_create)
+    role.grant("Collection", object_name, privilege_insert)
+    # role.grant("Collection", object_name, "*")
+    # role.grant("Collection", "*", privilege_insert)
 
     print(f"list grants")
     print(role.list_grants())
     print(f"list grant")
     print(role.list_grant("Collection", object_name))
 
-    connect_to_milvus(connection=_FOO_CONNECTION, user=username, password=password, db_name=_DB_NAME)
+    connect_to_milvus(connection=_FOO_CONNECTION, user=username, password=password)
     has_collection(_COLLECTION_NAME, connection=_FOO_CONNECTION)
     rbac_collection(connection=_FOO_CONNECTION)
     rbac_user(username, password, role_name, connection=_FOO_CONNECTION)
 
     print(f"revoke privilege")
     role.revoke("Global", "*", privilege_create)
-    role.revoke("Collection", object_name, privilege_insert, db_name=_DB_NAME)
-    # role.revoke("Collection", object_name, "*", db_name=_DB_NAME)
-    # role.revoke("Collection", "*", privilege_insert, db_name=_DB_NAME)
+    role.revoke("Collection", object_name, privilege_insert)
+    # role.revoke("Collection", object_name, "*")
+    # role.revoke("Collection", "*", privilege_insert)
     print(f"remove user")
     role.remove_user(username)
     role.drop()
     drop_credential(username)
 
 
 def run():
```

### Comparing `pymilvus-2.2.8/examples/user.py` & `pymilvus-2.3.0b1/examples/user.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/pylint.conf` & `pymilvus-2.3.0b1/pylint.conf`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/pymilvus/__init__.py` & `pymilvus-2.3.0b1/pymilvus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,15 @@
     ParamError,
     MilvusException,
     MilvusUnavailableException,
     ExceptionsMessage
 )
 from .client import __version__
 
-from .settings import (
-    DEBUG_LOG_LEVEL,
-    INFO_LOG_LEVEL,
-    WARN_LOG_LEVEL,
-    ERROR_LOG_LEVEL,
-)
-# Compatiable
-from .settings import Config as DefaultConfig
-
-from .client.constants import DEFAULT_RESOURCE_GROUP
+from .settings import DEBUG_LOG_LEVEL, INFO_LOG_LEVEL, WARN_LOG_LEVEL, ERROR_LOG_LEVEL
 
 from .orm.collection import Collection
 from .orm.connections import connections, Connections
 
 from .orm.index import Index
 from .orm.partition import Partition
 from .orm.utility import (
@@ -63,14 +54,15 @@
     do_bulk_insert, get_bulk_insert_state, list_bulk_insert_tasks,
     reset_password, create_user, update_password, delete_user, list_usernames,
     create_resource_group, drop_resource_group, describe_resource_group,
     list_resource_groups, transfer_node, transfer_replica
 )
 
 from .orm import utility
+from .orm.default_config import DefaultConfig, ENV_CONNECTION_CONF, DEFAULT_RESOURCE_GROUP
 
 from .orm.search import SearchResult, Hits, Hit
 from .orm.schema import FieldSchema, CollectionSchema
 from .orm.future import SearchFuture, MutationFuture
 from .orm.role import Role
 
 __all__ = [
```

### Comparing `pymilvus-2.2.8/pymilvus/client/__init__.py` & `pymilvus-2.3.0b1/pymilvus/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/pymilvus/client/abstract.py` & `pymilvus-2.3.0b1/pymilvus/client/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
 
 import numpy as np
-from ..settings import Config
+from .configs import DefaultConfigs
 from .types import DataType
 from .constants import DEFAULT_CONSISTENCY_LEVEL
 from ..grpc_gen import schema_pb2
 from ..exceptions import MilvusException
 
 
 class LoopBase:
@@ -84,15 +84,15 @@
         for type_param in raw.type_params:
             if type_param.key == "params":
                 import json
                 self.params[type_param.key] = json.loads(type_param.value)
             else:
                 self.params[type_param.key] = type_param.value
                 # maybe we'd better not to check these fields in ORM.
-                if type_param.key in ["dim", Config.MaxVarCharLengthKey]:
+                if type_param.key in ["dim", DefaultConfigs.MaxVarCharLengthKey]:
                     self.params[type_param.key] = int(type_param.value)
 
         index_dict = {}
         for index_param in raw.index_params:
             if index_param.key == "params":
                 import json
                 index_dict[index_param.key] = json.loads(index_param.value)
@@ -217,17 +217,15 @@
     def __init__(self, entity_id, entity_row_data, entity_score):
         self._id = entity_id
         self._row_data = entity_row_data
         self._score = entity_score
         self._distance = entity_score
 
     def __str__(self):
-        return str(self.entity)
-
-    __repr__ = __str__
+        return f"(distance: {self._distance}, score: {self._score}, id: {self._id})"
 
     @property
     def entity(self):
         return Entity(self._id, self._row_data, self._score)
 
     @property
     def id(self):
```

### Comparing `pymilvus-2.2.8/pymilvus/client/asynch.py` & `pymilvus-2.3.0b1/pymilvus/client/asynch.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/pymilvus/client/blob.py` & `pymilvus-2.3.0b1/pymilvus/client/blob.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/pymilvus/client/check.py` & `pymilvus-2.3.0b1/pymilvus/client/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,25 +215,26 @@
     return True
 
 def is_legal_replica_number(replica_number: int) -> bool:
     return isinstance(replica_number, int)
 
 # https://milvus.io/cn/docs/v1.0.0/metric.md#floating
 def is_legal_index_metric_type(index_type: str, metric_type: str) -> bool:
-    if index_type not in ("FLAT",
+    if index_type not in ("GPU_FLAT",
+                          "GPU_IVF_FLAT",
+                          "GPU_IVF_SQ8",
+                          "GPU_IVF_PQ",
+                          "RAFT_IVF_FLAT",
+                          "RAFT_IVF_PQ",
+                          "FLAT",
                           "IVF_FLAT",
                           "IVF_SQ8",
-                          # "IVF_SQ8_HYBRID",
                           "IVF_PQ",
                           "HNSW",
-                          # "NSG",
                           "ANNOY",
-                          "RHNSW_FLAT",
-                          "RHNSW_PQ",
-                          "RHNSW_SQ",
                           "AUTOINDEX",
                           "DISKANN"):
         return False
     if metric_type not in ("L2", "IP"):
         return False
     return True
```

### Comparing `pymilvus-2.2.8/pymilvus/client/entity_helper.py` & `pymilvus-2.3.0b1/pymilvus/client/entity_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from ..grpc_gen import schema_pb2 as schema_types
 from .types import DataType
 from ..exceptions import ParamError
-from ..settings import Config
+from .configs import DefaultConfigs
 
 
 def entity_type_to_dtype(entity_type):
     if isinstance(entity_type, int):
         return entity_type
     if isinstance(entity_type, str):
         # case sensitive
         return schema_types.DataType.Value(entity_type)
     raise ParamError(message=f"invalid entity type: {entity_type}")
 
 
 def get_max_len_of_var_char(field_info) -> int:
-    k = Config.MaxVarCharLengthKey
-    v = Config.MaxVarCharLength
+    k = DefaultConfigs.MaxVarCharLengthKey
+    v = DefaultConfigs.MaxVarCharLength
     return field_info.get("params", {}).get(k, v)
 
 
 def check_str_arr(str_arr, max_len):
     for s in str_arr:
         if not isinstance(s, str):
             raise ParamError(message=f"expect string input, got: {type(s)}")
         if len(s) > max_len:
             raise ParamError(message=f"invalid input, length of string exceeds max length. length: {len(s)}, "
                                      f"max length: {max_len}")
 
 
 def entity_to_str_arr(entity, field_info, check=True):
     arr = []
-    if Config.EncodeProtocol.lower() != 'utf-8'.lower():
+    if DefaultConfigs.EncodeProtocol.lower() != 'utf-8'.lower():
         for s in entity.get("values"):
-            arr.append(s.encode(Config.EncodeProtocol))
+            arr.append(s.encode(DefaultConfigs.EncodeProtocol))
     else:
         arr = entity.get("values")
     max_len = int(get_max_len_of_var_char(field_info))
     if check:
         check_str_arr(arr, max_len)
     return arr
```

### Comparing `pymilvus-2.2.8/pymilvus/client/grpc_handler.py` & `pymilvus-2.3.0b1/pymilvus/client/grpc_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,19 @@
     GrantInfo, UserInfo, RoleInfo,
     BulkInsertState,
     ResourceGroupInfo,
 )
 
 from .utils import (
     check_invalid_binary_vector,
-    len_of,
-    get_server_type,
+    len_of
 )
 
-from ..settings import Config
+from ..settings import DefaultConfig as config
+from .configs import DefaultConfigs
 from . import ts_utils
 from . import interceptor
 
 from .asynch import (
     SearchFuture,
     MutationFuture,
     CreateIndexFuture,
@@ -63,15 +63,15 @@
     AmbiguousIndexName,
 )
 
 from ..decorators import retry_on_rpc_failure
 
 
 class GrpcHandler:
-    def __init__(self, uri=Config.GRPC_URI, host="", port="", channel=None, **kwargs):
+    def __init__(self, uri=config.GRPC_URI, host="", port="", channel=None, **kwargs):
         self._stub = None
         self._channel = channel
 
         addr = kwargs.get("address")
         self._address = addr if addr is not None else self.__get_address(uri, host, port)
         self._log_level = None
         self._request_id = None
@@ -97,16 +97,14 @@
         self._client_key_path = kwargs.get("client_key_path", "")
         self._ca_pem_path = kwargs.get("ca_pem_path", "")
         self._server_pem_path = kwargs.get("server_pem_path", "")
         self._server_name = kwargs.get("server_name", "")
 
         self._authorization_interceptor = None
         self._setup_authorization_interceptor(kwargs.get("user", None), kwargs.get("password", None))
-        self._db_interceptor = None
-        self._setup_db_interceptor(kwargs.get("db_name", None))
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
@@ -126,18 +124,14 @@
 
     def _setup_authorization_interceptor(self, user, password):
         if user and password:
             authorization = base64.b64encode(f"{user}:{password}".encode('utf-8'))
             key = "authorization"
             self._authorization_interceptor = interceptor.header_adder_interceptor(key, authorization)
 
-    def _setup_db_interceptor(self, db_name):
-        if db_name:
-            self._db_interceptor = interceptor.header_adder_interceptor("dbname", db_name)
-
     def _setup_grpc_channel(self):
         """ Create a ddl grpc channel """
         if self._channel is None:
             opts = [(cygrpc.ChannelArgKey.max_send_message_length, -1),
                     (cygrpc.ChannelArgKey.max_receive_message_length, -1),
                     ('grpc.enable_retries', 1),
                     ('grpc.keepalive_time_ms', 55000),
@@ -171,16 +165,14 @@
                     creds,
                     options=opts
                 )
         # avoid to add duplicate headers.
         self._final_channel = self._channel
         if self._authorization_interceptor:
             self._final_channel = grpc.intercept_channel(self._final_channel, self._authorization_interceptor)
-        if self._db_interceptor:
-            self._final_channel = grpc.intercept_channel(self._final_channel, self._db_interceptor)
         if self._log_level:
             log_level_interceptor = interceptor.header_adder_interceptor("log_level", self._log_level)
             self._final_channel = grpc.intercept_channel(self._final_channel, log_level_interceptor)
             self._log_level = None
         if self._request_id:
             request_id_interceptor = interceptor.header_adder_interceptor("client_request_id", self._request_id)
             self._final_channel = grpc.intercept_channel(self._final_channel, request_id_interceptor)
@@ -196,29 +188,25 @@
         self._setup_grpc_channel()
 
     @property
     def server_address(self):
         """ Server network address """
         return self._address
 
-    def get_server_type(self):
-        return get_server_type(self.server_address.split(':')[0])
-
     def reset_password(self, user, old_password, new_password, timeout=None):
         """
         reset password and then setup the grpc channel.
         """
         self.update_password(user, old_password, new_password, timeout=timeout)
         self._setup_authorization_interceptor(user, new_password)
         self._setup_grpc_channel()
 
     @retry_on_rpc_failure()
-    def create_collection(self, collection_name, fields, timeout=None, **kwargs):
-        check_pass_param(collection_name=collection_name)
-        request = Prepare.create_collection_request(collection_name, fields, **kwargs)
+    def create_collection(self, collection_name, fields, shards_num=2, timeout=None, **kwargs):
+        request = Prepare.create_collection_request(collection_name, fields, shards_num=shards_num, **kwargs)
 
         rf = self._stub.CreateCollection.future(request, timeout=timeout)
         if kwargs.get("_async", False):
             return rf
         status = rf.result()
         if status.error_code != 0:
             raise MilvusException(status.error_code, status.reason)
@@ -361,40 +349,47 @@
         response = future.result()
         status = response.status
         if status.error_code == 0:
             return response.stats
 
         raise MilvusException(status.error_code, status.reason)
 
-    def _prepare_batch_insert_request(self, collection_name, entities, partition_name=None, timeout=None, **kwargs):
-        insert_param = kwargs.get('insert_param', None)
+    def _prepare_batch_insert_or_upsert_request(self, collection_name, entities, partition_name=None, timeout=None, isInsert=True, **kwargs):
+        param = kwargs.get('insert_param', None)
+
+        if not isInsert:
+            param = kwargs.get('upsert_param', None)
 
-        if insert_param and not isinstance(insert_param, milvus_types.RowBatch):
-            raise ParamError(message="The value of key 'insert_param' is invalid")
+        if param and not isinstance(param, milvus_types.RowBatch):
+            if isInsert:
+                raise ParamError(message="The value of key 'insert_param' is invalid")
+            raise ParamError(message="The value of key 'upsert_param' is invalid")
         if not isinstance(entities, list):
             raise ParamError(message="None entities, please provide valid entities.")
 
         collection_schema = kwargs.get("schema", None)
         if not collection_schema:
-            collection_schema = self.describe_collection(collection_name, timeout=timeout, **kwargs)
+            collection_schema = self.describe_collection(
+                collection_name, timeout=timeout, **kwargs)
 
         fields_info = collection_schema["fields"]
 
-        request = insert_param if insert_param \
-            else Prepare.batch_insert_param(collection_name, entities, partition_name, fields_info)
+        request = param if param \
+            else Prepare.batch_insert_or_upsert_param(collection_name, entities, partition_name, fields_info, isInsert)
 
         return request
 
     @retry_on_rpc_failure()
     def batch_insert(self, collection_name, entities, partition_name=None, timeout=None, **kwargs):
         if not check_invalid_binary_vector(entities):
             raise ParamError(message="Invalid binary vector data exists")
 
         try:
-            request = self._prepare_batch_insert_request(collection_name, entities, partition_name, timeout, **kwargs)
+            request = self._prepare_batch_insert_or_upsert_request(
+                collection_name, entities, partition_name, timeout, **kwargs)
             rf = self._stub.Insert.future(request, timeout=timeout)
             if kwargs.get("_async", False) is True:
                 cb = kwargs.get("_callback", None)
                 f = MutationFuture(rf, cb, timeout=timeout, **kwargs)
                 f.add_callback(ts_utils.update_ts_on_mutation(collection_name))
                 return f
 
@@ -431,14 +426,42 @@
 
             raise MilvusException(response.status.error_code, response.status.reason)
         except Exception as err:
             if kwargs.get("_async", False):
                 return MutationFuture(None, None, err)
             raise err
 
+    @retry_on_rpc_failure()
+    def upsert(self, collection_name, entities, partition_name=None, timeout=None, **kwargs):
+        if not check_invalid_binary_vector(entities):
+            raise ParamError(message="Invalid binary vector data exists")
+
+        try:
+            request = self._prepare_batch_insert_or_upsert_request(
+                collection_name, entities, partition_name, timeout, False, **kwargs)
+            rf = self._stub.Upsert.future(request, timeout=timeout)
+            if kwargs.get("_async", False) is True:
+                cb = kwargs.get("_callback", None)
+                f = MutationFuture(rf, cb, timeout=timeout, **kwargs)
+                f.add_callback(ts_utils.update_ts_on_mutation(collection_name))
+                return f
+
+            response = rf.result()
+            if response.status.error_code == 0:
+                m = MutationResult(response)
+                ts_utils.update_collection_ts(collection_name, m.timestamp)
+                return m
+
+            raise MilvusException(
+                response.status.error_code, response.status.reason)
+        except Exception as err:
+            if kwargs.get("_async", False):
+                return MutationFuture(None, None, err)
+            raise err
+
     def _execute_search_requests(self, requests, timeout=None, **kwargs):
         auto_id = kwargs.get("auto_id", True)
 
         try:
             if kwargs.get("_async", False):
                 futures = []
                 for request in requests:
@@ -529,15 +552,15 @@
         response = rf.result()
         if response.error_code != 0:
             raise MilvusException(response.error_code, response.reason)
 
     @retry_on_rpc_failure()
     def create_index(self, collection_name, field_name, params, timeout=None, **kwargs):
         # for historical reason, index_name contained in kwargs.
-        index_name = kwargs.pop("index_name", Config.IndexName)
+        index_name = kwargs.pop("index_name", DefaultConfigs.IndexName)
         copy_kwargs = copy.deepcopy(kwargs)
 
         collection_desc = self.describe_collection(collection_name, timeout=timeout, **copy_kwargs)
 
         valid_field = False
         for fields in collection_desc["fields"]:
             if field_name != fields["name"]:
@@ -701,15 +724,15 @@
         def can_loop(t) -> bool:
             return True if timeout is None else t <= (start + timeout)
 
         while can_loop(time.time()):
             progress = self.get_loading_progress(collection_name, timeout=timeout)
             if progress >= 100:
                 return
-            time.sleep(Config.WaitTimeDurationWhenLoad)
+            time.sleep(DefaultConfigs.WaitTimeDurationWhenLoad)
         raise MilvusException(message=f"wait for loading collection timeout, collection: {collection_name}")
 
     @retry_on_rpc_failure()
     def release_collection(self, collection_name, timeout=None):
         check_pass_param(collection_name=collection_name)
         request = Prepare.release_collection("", collection_name)
         rf = self._stub.ReleaseCollection.future(request, timeout=timeout)
@@ -757,15 +780,15 @@
         def can_loop(t) -> bool:
             return True if timeout is None else t <= (start + timeout)
 
         while can_loop(time.time()):
             progress = self.get_loading_progress(collection_name, partition_names, timeout=timeout)
             if progress >= 100:
                 return
-            time.sleep(Config.WaitTimeDurationWhenLoad)
+            time.sleep(DefaultConfigs.WaitTimeDurationWhenLoad)
         raise MilvusException(message=f"wait for loading partition timeout, collection: {collection_name}, partitions: {partition_names}")
 
     @retry_on_rpc_failure()
     def get_loading_progress(self, collection_name, partition_names=None, timeout=None):
         request = Prepare.get_loading_progress(collection_name, partition_names)
         response = self._stub.GetLoadingProgress.future(request, timeout=timeout).result()
         if response.status.error_code != 0:
@@ -1181,41 +1204,41 @@
         req = Prepare.select_user_request(None, include_role_info)
         resp = self._stub.SelectUser(req, wait_for_ready=True, timeout=timeout)
         if resp.status.error_code != 0:
             raise MilvusException(resp.status.error_code, resp.status.reason)
         return UserInfo(resp.results)
 
     @retry_on_rpc_failure()
-    def grant_privilege(self, role_name, object, object_name, privilege, db_name, timeout=None, **kwargs):
-        req = Prepare.operate_privilege_request(role_name, object, object_name, privilege, db_name,
+    def grant_privilege(self, role_name, object, object_name, privilege, timeout=None, **kwargs):
+        req = Prepare.operate_privilege_request(role_name, object, object_name, privilege,
                                                 milvus_types.OperatePrivilegeType.Grant)
         resp = self._stub.OperatePrivilege(req, wait_for_ready=True, timeout=timeout)
         if resp.error_code != 0:
             raise MilvusException(resp.error_code, resp.reason)
 
     @retry_on_rpc_failure()
-    def revoke_privilege(self, role_name, object, object_name, privilege, db_name, timeout=None, **kwargs):
-        req = Prepare.operate_privilege_request(role_name, object, object_name, privilege, db_name,
+    def revoke_privilege(self, role_name, object, object_name, privilege, timeout=None, **kwargs):
+        req = Prepare.operate_privilege_request(role_name, object, object_name, privilege,
                                                 milvus_types.OperatePrivilegeType.Revoke)
         resp = self._stub.OperatePrivilege(req, wait_for_ready=True, timeout=timeout)
         if resp.error_code != 0:
             raise MilvusException(resp.error_code, resp.reason)
 
     @retry_on_rpc_failure()
-    def select_grant_for_one_role(self, role_name, db_name, timeout=None, **kwargs):
-        req = Prepare.select_grant_request(role_name, None, None, db_name)
+    def select_grant_for_one_role(self, role_name, timeout=None, **kwargs):
+        req = Prepare.select_grant_request(role_name, None, None)
         resp = self._stub.SelectGrant(req, wait_for_ready=True, timeout=timeout)
         if resp.status.error_code != 0:
             raise MilvusException(resp.status.error_code, resp.status.reason)
 
         return GrantInfo(resp.entities)
 
     @retry_on_rpc_failure()
-    def select_grant_for_role_and_object(self, role_name, object, object_name, db_name, timeout=None, **kwargs):
-        req = Prepare.select_grant_request(role_name, object, object_name, db_name)
+    def select_grant_for_role_and_object(self, role_name, object, object_name, timeout=None, **kwargs):
+        req = Prepare.select_grant_request(role_name, object, object_name)
         resp = self._stub.SelectGrant(req, wait_for_ready=True, timeout=timeout)
         if resp.status.error_code != 0:
             raise MilvusException(resp.status.error_code, resp.status.reason)
 
         return GrantInfo(resp.entities)
 
     @retry_on_rpc_failure()
@@ -1266,52 +1289,7 @@
 
     @retry_on_rpc_failure()
     def transfer_replica(self, source, target, collection_name, num_replica, timeout=None, **kwargs):
         req = Prepare.transfer_replica(source, target, collection_name, num_replica)
         resp = self._stub.TransferReplica(req, wait_for_ready=True, timeout=timeout)
         if resp.error_code != 0:
             raise MilvusException(resp.error_code, resp.reason)
-
-    @retry_on_rpc_failure()
-    def get_flush_all_state(self, flush_all_ts, timeout=None, **kwargs):
-        req = Prepare.get_flush_all_state_request(flush_all_ts)
-        response = self._stub.GetFlushAllState(req, timeout=timeout)
-        status = response.status
-        if status.error_code == 0:
-            return response.flushed
-        raise MilvusException(status.error_code, status.reason)
-
-    def _wait_for_flush_all(self, flush_all_ts, timeout=None, **kwargs):
-        flush_ret = False
-        start = time.time()
-        while not flush_ret:
-            flush_ret = self.get_flush_all_state(flush_all_ts, timeout, **kwargs)
-            end = time.time()
-            if timeout is not None:
-                if end - start > timeout:
-                    raise MilvusException(message=f"wait for flush all timeout, flush_all_ts: {flush_all_ts}")
-
-            if not flush_ret:
-                time.sleep(5)
-
-    @retry_on_rpc_failure()
-    def flush_all(self, timeout=None, **kwargs):
-        request = Prepare.flush_all_request()
-        future = self._stub.FlushAll.future(request, timeout=timeout)
-        response = future.result()
-        if response.status.error_code != 0:
-            raise MilvusException(response.status.error_code, response.status.reason)
-
-        def _check():
-            self._wait_for_flush_all(response.flush_all_ts, timeout, **kwargs)
-
-        if kwargs.get("_async", False):
-            flush_future = FlushFuture(future)
-            flush_future.add_callback(_check)
-
-            user_cb = kwargs.get("_callback", None)
-            if user_cb:
-                flush_future.add_callback(user_cb)
-
-            return flush_future
-
-        _check()
```

### Comparing `pymilvus-2.2.8/pymilvus/client/interceptor.py` & `pymilvus-2.3.0b1/pymilvus/client/interceptor.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/pymilvus/client/prepare.py` & `pymilvus-2.3.0b1/pymilvus/client/prepare.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,66 +4,62 @@
 
 import ujson
 
 from . import blob
 from . import entity_helper
 from .check import check_pass_param, is_legal_collection_properties
 from .types import DataType, PlaceholderType, get_consistency_level
+from .utils import traverse_info
 from .constants import DEFAULT_CONSISTENCY_LEVEL
 from ..exceptions import ParamError, DataNotMatchException, ExceptionsMessage
 from ..orm.schema import CollectionSchema
 
 from ..grpc_gen import common_pb2 as common_types
 from ..grpc_gen import schema_pb2 as schema_types
 from ..grpc_gen import milvus_pb2 as milvus_types
 
 
 class Prepare:
     @classmethod
     def create_collection_request(cls, collection_name: str, fields: Union[Dict[str, Iterable], CollectionSchema],
-                                  **kwargs) -> milvus_types.CreateCollectionRequest:
+                                  shards_num=2, **kwargs) -> milvus_types.CreateCollectionRequest:
         """
         :type fields: Union(Dict[str, Iterable], CollectionSchema)
         :param fields: (Required)
 
             `{"fields": [
                     {"name": "A", "type": DataType.INT32}
                     {"name": "B", "type": DataType.INT64, "auto_id": True, "is_primary": True},
                     {"name": "C", "type": DataType.FLOAT},
                     {"name": "Vec", "type": DataType.FLOAT_VECTOR, "params": {"dim": 128}}]
             }`
 
         :return: milvus_types.CreateCollectionRequest
         """
         if isinstance(fields, CollectionSchema):
-            schema = cls.get_schema_from_collection_schema(collection_name, fields, **kwargs)
+            schema = cls.get_schema_from_collection_schema(collection_name, fields, shards_num, **kwargs)
         else:
-            schema = cls.get_schema(collection_name, fields, **kwargs)
+            schema = cls.get_schema(collection_name, fields, shards_num, **kwargs)
 
         consistency_level = get_consistency_level(kwargs.get("consistency_level", DEFAULT_CONSISTENCY_LEVEL))
 
         req = milvus_types.CreateCollectionRequest(collection_name=collection_name,
                                                     schema=bytes(schema.SerializeToString()),
+                                                    shards_num=shards_num,
                                                     consistency_level=consistency_level)
 
         properties = kwargs.get("properties")
         if is_legal_collection_properties(properties):
             properties = [common_types.KeyValuePair(key=str(k), value=str(v)) for k, v in properties.items()]
             req.properties.extend(properties)
 
-        shards_num = kwargs.get("shards_num")
-        if shards_num is not None:
-            if not isinstance(shards_num, int):
-                raise ParamError(message="invalid shards_num type, got {type(shards_num)}, expected int")
-            req.shards_num=shards_num
-
         return req
 
     @classmethod
-    def get_schema_from_collection_schema(cls, collection_name: str, fields: CollectionSchema, **kwargs) -> milvus_types.CreateCollectionRequest:
+    def get_schema_from_collection_schema(cls, collection_name: str, fields: CollectionSchema, shards_num=2, **kwargs) -> milvus_types.CreateCollectionRequest:
         coll_description = fields.description
         if not isinstance(coll_description, (str, bytes)):
             raise ParamError(message=f"description [{coll_description}] has type {type(coll_description).__name__},  but expected one of: bytes, str")
 
         schema = schema_types.CollectionSchema(name=collection_name,
                                                autoID=fields.auto_id,
                                                description=coll_description)
@@ -77,15 +73,15 @@
                 kv_pair = common_types.KeyValuePair(key=str(k), value=str(v))
                 field_schema.type_params.append(kv_pair)
 
             schema.fields.append(field_schema)
         return schema
 
     @classmethod
-    def get_schema(cls, collection_name: str, fields: Dict[str, Iterable], **kwargs) -> schema_types.CollectionSchema:
+    def get_schema(cls, collection_name: str, fields: Dict[str, Iterable], shards_num=2, **kwargs) -> schema_types.CollectionSchema:
         if not isinstance(fields, dict):
             raise ParamError(message="Param fields must be a dict")
 
         all_fields = fields.get("fields")
         if all_fields is None:
             raise ParamError(message="Param fields must contain key 'fields'")
         if len(all_fields) == 0:
@@ -248,66 +244,30 @@
             raise ParamError(message="collection_name must be of str type")
         if not isinstance(partition_name, str):
             raise ParamError(message="partition_name must be of str type")
         return milvus_types.PartitionName(collection_name=collection_name,
                                           tag=partition_name)
 
     @classmethod
-    def batch_insert_param(cls, collection_name, entities, partition_name, fields_info=None, **kwargs):
-        # insert_request.hash_keys won't be filled in client. It will be filled in proxy.
+    def batch_insert_or_upsert_param(cls, collection_name, entities, partition_name, fields_info=None, isInsert=True, **kwargs):
+        # insert_request.hash_keys and upsert_request.hash_keys won't be filled in client. It will be filled in proxy.
+
+        tag = partition_name or "_default"  # should here?
+        request = milvus_types.InsertRequest(collection_name=collection_name, partition_name=tag)
 
-        tag = partition_name if isinstance(partition_name, str) else "_default"  # should here?
-        insert_request = milvus_types.InsertRequest(collection_name=collection_name, partition_name=tag)
+        if not isInsert:
+            request = milvus_types.UpsertRequest(collection_name=collection_name, partition_name=tag)
 
         for entity in entities:
             if not entity.get("name", None) or not entity.get("values", None) or not entity.get("type", None):
                 raise ParamError(message="Missing param in entities, a field must have type, name and values")
         if not fields_info:
             raise ParamError(message="Missing collection meta to validate entities")
 
-        location, primary_key_loc, auto_id_loc = {}, None, None
-        for i, field in enumerate(fields_info):
-            if field.get("is_primary", False):
-                primary_key_loc = i
-
-            if field.get("auto_id", False):
-                auto_id_loc = i
-                continue
-
-            match_flag = False
-            field_name = field["name"]
-            field_type = field["type"]
-
-            for entity in entities:
-                entity_name, entity_type = entity["name"], entity["type"]
-
-                if field_name == entity_name:
-                    if field_type != entity_type:
-                        raise ParamError(message=f"Collection field type is {field_type}"
-                                         f", but entities field type is {entity_type}")
-
-                    entity_dim, field_dim = 0, 0
-                    if entity_type in [DataType.FLOAT_VECTOR, DataType.BINARY_VECTOR]:
-                        field_dim = field["params"]["dim"]
-                        entity_dim = len(entity["values"][0])
-
-                    if entity_type in [DataType.FLOAT_VECTOR, ] and entity_dim != field_dim:
-                        raise ParamError(message=f"Collection field dim is {field_dim}"
-                                         f", but entities field dim is {entity_dim}")
-
-                    if entity_type in [DataType.BINARY_VECTOR, ] and entity_dim * 8 != field_dim:
-                        raise ParamError(message=f"Collection field dim is {field_dim}"
-                                         f", but entities field dim is {entity_dim * 8}")
-
-                    location[field["name"]] = i
-                    match_flag = True
-                    break
-
-            if not match_flag:
-                raise ParamError(message=f"Field {field['name']} don't match in entities")
+        location, primary_key_loc, auto_id_loc = traverse_info(fields_info, entities)
 
         # though impossible from sdk
         if primary_key_loc is None:
             raise ParamError(message="primary key not found")
 
         if auto_id_loc is None and len(entities) != len(fields_info):
             raise ParamError(message=f"number of fields: {len(fields_info)}, number of entities: {len(entities)}")
@@ -319,21 +279,21 @@
         try:
             for entity in entities:
                 current = len(entity.get("values"))
                 if row_num not in (0, current):
                     raise ParamError(message="row num misaligned current[{current}]!= previous[{row_num}]")
                 row_num = current
                 field_data = entity_helper.entity_to_field_data(entity, fields_info[location[entity.get("name")]])
-                insert_request.fields_data.append(field_data)
+                request.fields_data.append(field_data)
         except (TypeError, ValueError) as e:
             raise DataNotMatchException(message=ExceptionsMessage.DataTypeInconsistent) from e
 
-        insert_request.num_rows = row_num
+        request.num_rows = row_num
 
-        return insert_request
+        return request
 
     @classmethod
     def delete_request(cls, collection_name, partition_name, expr):
         def check_str(instr, prefix):
             if instr is None:
                 raise ParamError(message=f"{prefix} cannot be None")
             if not isinstance(instr, str):
@@ -465,15 +425,15 @@
             is_binary = False
             pl_type = PlaceholderType.FloatVector
 
         if anns_field not in fields_name_locs:
             raise ParamError(message=f"Field {anns_field} doesn't exist in schema")
         dimension = int(fields_schema[fields_name_locs[anns_field]]["params"].get("dim", 0))
 
-        ignore_growing = param.get("ignore_growing",False) or kwargs.get("ignore_growing",False)
+        ignore_growing = param.get("ignore_growing",False)
         params = param.get("params", {})
         if not isinstance(params, dict):
             raise ParamError(message=f"Search params must be a dict, got {type(params)}")
         search_params = {
             "anns_field": anns_field,
             "topk": limit,
             "metric_type": param.get("metric_type", "L2"),
@@ -795,42 +755,39 @@
         if username:
             check_pass_param(user=username)
         check_pass_param(include_role_info=include_role_info)
         return milvus_types.SelectUserRequest(user=milvus_types.UserEntity(name=username) if username else None,
                                               include_role_info=include_role_info)
 
     @classmethod
-    def operate_privilege_request(cls, role_name, object, object_name, privilege, db_name, operate_privilege_type):
+    def operate_privilege_request(cls, role_name, object, object_name, privilege, operate_privilege_type):
         check_pass_param(role_name=role_name)
         check_pass_param(object=object)
         check_pass_param(object_name=object_name)
         check_pass_param(privilege=privilege)
         check_pass_param(operate_privilege_type=operate_privilege_type)
         return milvus_types.OperatePrivilegeRequest(
             entity=milvus_types.GrantEntity(role=milvus_types.RoleEntity(name=role_name),
                                             object=milvus_types.ObjectEntity(name=object),
                                             object_name=object_name,
-                                            db_name=db_name,
                                             grantor=milvus_types.GrantorEntity(
                                                 privilege=milvus_types.PrivilegeEntity(name=privilege))),
             type=operate_privilege_type)
 
     @classmethod
-    def select_grant_request(cls, role_name, object, object_name, db_name):
+    def select_grant_request(cls, role_name, object, object_name):
         check_pass_param(role_name=role_name)
         if object:
             check_pass_param(object=object)
         if object_name:
             check_pass_param(object_name=object_name)
         return milvus_types.SelectGrantRequest(
             entity=milvus_types.GrantEntity(role=milvus_types.RoleEntity(name=role_name),
                                             object=milvus_types.ObjectEntity(name=object) if object else None,
-                                            object_name=object_name if object_name else None,
-                                            db_name=db_name,
-                                            ))
+                                            object_name=object_name if object_name else None))
 
     @classmethod
     def get_server_version(cls):
         return milvus_types.GetVersionRequest()
 
     @classmethod
     def create_resource_group(cls, name):
@@ -863,15 +820,7 @@
     def transfer_replica(cls, source, target, collection_name, num_replica):
         check_pass_param(resource_group_name=source)
         check_pass_param(resource_group_name=target)
         return milvus_types.TransferReplicaRequest(source_resource_group=source,
                                                    target_resource_group=target,
                                                    collection_name=collection_name,
                                                    num_replica=num_replica)
-
-    @classmethod
-    def flush_all_request(cls):
-        return milvus_types.FlushAllRequest()
-
-    @classmethod
-    def get_flush_all_state_request(cls, flush_all_ts):
-        return milvus_types.GetFlushAllStateRequest(flush_all_ts=flush_all_ts)
```

### Comparing `pymilvus-2.2.8/pymilvus/client/stub.py` & `pymilvus-2.3.0b1/pymilvus/client/stub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from urllib import parse
 
 from .grpc_handler import GrpcHandler
 from ..exceptions import MilvusException, ParamError
 from .types import CompactionState, CompactionPlans, Replica, BulkInsertState, ResourceGroupInfo
-from ..settings import Config
+from ..settings import DefaultConfig as config
 from ..decorators import deprecated
 
 from .check import is_legal_host, is_legal_port
 
 
 class Milvus:
     @deprecated
-    def __init__(self, host=None, port=Config.GRPC_PORT, uri=Config.GRPC_URI, channel=None, **kwargs):
+    def __init__(self, host=None, port=config.GRPC_PORT, uri=config.GRPC_URI, channel=None, **kwargs):
         self.address = self.__get_address(host, port, uri)
         self._handler = GrpcHandler(address=self.address, channel=channel, **kwargs)
 
         if kwargs.get("pre_ping", False) is True:
             self._handler._wait_for_channel_ready()
 
-    def __get_address(self, host=None, port=Config.GRPC_PORT, uri=Config.GRPC_URI):
+    def __get_address(self, host=None, port=config.GRPC_PORT, uri=config.GRPC_URI):
         if host is None and uri is None:
             raise ParamError(message='Host and uri cannot both be None')
 
         if host is None:
             try:
                 parsed_uri = parse.urlparse(uri, "tcp")
             except (Exception) as e:
@@ -43,27 +43,24 @@
     def name(self):
         return self._name
 
     @property
     def handler(self):
         return self._handler
 
-    def get_server_type(self):
-        return self._handler.get_server_type()
-
     def reset_password(self, user, old_password, new_password):
         self._handler.reset_password(user, old_password, new_password)
 
     def close(self):
         if self._handler is None:
             raise MilvusException(message="Closing on closed handler")
         self.handler.close()
         self._handler = None
 
-    def create_collection(self, collection_name, fields, shards_num=None, timeout=None, **kwargs):
+    def create_collection(self, collection_name, fields, shards_num=2, timeout=None, **kwargs):
         """ Creates a collection.
 
         :param collection_name: The name of the collection. A collection name can only include
         numbers, letters, and underscores, and must not begin with a number.
         :type  collection_name: str
 
         :param fields: Field parameters.
@@ -74,21 +71,23 @@
                     {"field": "B", "type": DataType.INT64},
                     {"field": "C", "type": DataType.FLOAT},
                     {"field": "Vec", "type": DataType.FLOAT_VECTOR,
                      "params": {"dim": 128}}
                 ],
             "auto_id": True}`
 
+        :param shards_num: How wide to scale collection. Corresponds to how many active datanodes
+                        can be used on insert.
+        :type shards_num: int
+
         :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
                         is set to None, client waits until server response or error occur.
         :type  timeout: float
 
         :param kwargs:
-            * *shards_num* (``int``) --
-            How wide to scale collection. Corresponds to how many active datanodes can be used on insert.
             * *consistency_level* (``str/int``) --
             Which consistency level to use when searching in the collection. For details, see
             https://github.com/milvus-io/milvus/blob/master/docs/developer_guides/how-guarantee-ts-works.md.
             Note: this parameter can be overwritten by the same parameter specified in search.
             * *properties* (``dict``) --
```

### Comparing `pymilvus-2.2.8/pymilvus/client/ts_utils.py` & `pymilvus-2.3.0b1/pymilvus/client/ts_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import threading
 import datetime
 
 from .singleton_utils import Singleton
 from .utils import hybridts_to_unixtime
 from .constants import EVENTUALLY_TS, BOUNDED_TS
 
-from ..grpc_gen import common_pb2
-
-ConsistencyLevel = common_pb2.ConsistencyLevel
+from ..grpc_gen.common_pb2 import ConsistencyLevel
 
 
 class GTsDict(metaclass=Singleton):
     def __init__(self):
         # collection id -> last write ts
         self._last_write_ts_dict = {}
         self._last_write_ts_dict_lock = threading.Lock()
```

### Comparing `pymilvus-2.2.8/pymilvus/client/types.py` & `pymilvus-2.3.0b1/pymilvus/client/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import time
 from enum import IntEnum
+from ..grpc_gen.common_pb2 import ConsistencyLevel
 from ..grpc_gen import common_pb2
 from ..exceptions import (
     AutoIDException,
     ExceptionsMessage,
     InvalidConsistencyLevel,
 )
 from ..grpc_gen import milvus_pb2 as milvus_types
 
 
-ConsistencyLevel = common_pb2.ConsistencyLevel
-
 class Status:
     """
     :attribute code: int (optional) default as ok
 
     :attribute message: str (optional) current status message
     """
 
@@ -286,17 +285,17 @@
             return ConsistencyLevel.Value(consistency_level)
         except ValueError as e:
             raise InvalidConsistencyLevel(message=f"invalid consistency level: {consistency_level}") from e
     raise InvalidConsistencyLevel(message="invalid consistency level")
 
 
 class Shard:
-    def __init__(self, channel_name: str, shard_nodes: list, shard_leader: int):
+    def __init__(self, channel_name: str, shard_nodes, shard_leader: int):
         self._channel_name = channel_name
-        self._shard_nodes = set(shard_nodes)
+        self._shard_nodes = shard_nodes
         self._shard_leader = shard_leader
 
     def __repr__(self):
         return f"""Shard: <channel_name:{self.channel_name}>, <shard_leader:{self.shard_leader}>, <shard_nodes:{self.shard_nodes}>"""
 
     @property
     def channel_name(self) -> str:
@@ -532,39 +531,33 @@
         return int(percent)
 
 
 class GrantItem:
     def __init__(self, entity):
         self._object = entity.object.name
         self._object_name = entity.object_name
-        self._db_name = entity.db_name
         self._role_name = entity.role.name
         self._grantor_name = entity.grantor.user.name
         self._privilege = entity.grantor.privilege.name
 
     def __repr__(self) -> str:
         s = f"GrantItem: <object:{self.object}>, <object_name:{self.object_name}>, " \
-            f"<db_name:{self.db_name}>, " \
             f"<role_name:{self.role_name}>, <grantor_name:{self.grantor_name}>, " \
             f"<privilege:{self.privilege}>"
         return s
 
     @property
     def object(self):
         return self._object
 
     @property
     def object_name(self):
         return self._object_name
 
     @property
-    def db_name(self):
-        return self._db_name
-
-    @property
     def role_name(self):
         return self._role_name
 
     @property
     def grantor_name(self):
         return self._grantor_name
 
@@ -700,20 +693,20 @@
         self._num_available_node = resource_group.num_available_node
         self._num_loaded_replica = resource_group.num_loaded_replica
         self._num_outgoing_node = resource_group.num_outgoing_node
         self._num_incoming_node = resource_group.num_incoming_node
 
     def __repr__(self) -> str:
         s = f"""ResourceGroupInfo:
-<name:{self.name}>,
-<capacity:{self.capacity}>,
-<num_available_node:{self.num_available_node}>,
-<num_loaded_replica:{self.num_loaded_replica}>,
-<num_outgoing_node:{self.num_outgoing_node}>,
-<num_incoming_node:{self.num_incoming_node}>"""
+        <name:{self.name}>, 
+        <capacity:{self.capacity}>, 
+        <num_available_node:{self.num_available_node}>, 
+        <num_loaded_replica:{self.num_loaded_replica}>, 
+        <num_outgoing_node:{self.num_outgoing_node}>, 
+        <num_incoming_node:{self.num_incoming_node}>"""
         return s
 
 
     @property
     def name(self):
         return self._name
```

### Comparing `pymilvus-2.2.8/pymilvus/client/utils.py` & `pymilvus-2.3.0b1/pymilvus/client/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import datetime
 
-from .constants import LOGICAL_BITS, LOGICAL_BITS_MASK
 from .types import DataType
-from ..exceptions import MilvusException
+from .constants import LOGICAL_BITS, LOGICAL_BITS_MASK
+from ..exceptions import ParamError, MilvusException
 
 valid_index_types = [
+    "GPU_FLAT",
+    "GPU_IVF_FLAT",
+    "GPU_IVF_SQ8",
+    "GPU_IVF_PQ",
+    "RAFT_IVF_FLAT",
+    "RAFT_IVF_PQ",
     "FLAT",
     "IVF_FLAT",
     "IVF_SQ8",
-    # "IVF_SQ8_HYBRID",
     "IVF_PQ",
     "HNSW",
-    # "NSG",
     "ANNOY",
-    "RHNSW_FLAT",
-    "RHNSW_PQ",
-    "RHNSW_SQ",
     "BIN_FLAT",
     "BIN_IVF_FLAT",
     "DISKANN",
     "AUTOINDEX"
 ]
 
 valid_index_params_keys = [
@@ -147,17 +148,51 @@
 
         total_len = len(field_data.vectors.binary_vector)
         return int(total_len / (dim / 8))
 
     raise MilvusException(message="Unknown data type")
 
 
-def get_server_type(host):
-    if host is None or not isinstance(host, str):
-        return "milvus"
-    splits = host.split('.')
-    len_of_splits = len(splits)
-    if len_of_splits >= 2 and \
-            splits[len_of_splits - 2].lower() == "zillizcloud" and \
-            splits[len_of_splits - 1].lower() == "com":
-        return "zilliz"
-    return "milvus"
+def traverse_info(fields_info, entities):
+    location, primary_key_loc, auto_id_loc = {}, None, None
+    for i, field in enumerate(fields_info):
+        if field.get("is_primary", False):
+            primary_key_loc = i
+
+        if field.get("auto_id", False):
+            auto_id_loc = i
+            continue
+
+        match_flag = False
+        field_name = field["name"]
+        field_type = field["type"]
+
+        for entity in entities:
+            entity_name, entity_type = entity["name"], entity["type"]
+
+            if field_name == entity_name:
+                if field_type != entity_type:
+                    raise ParamError(message=f"Collection field type is {field_type}"
+                                     f", but entities field type is {entity_type}")
+
+                entity_dim, field_dim = 0, 0
+                if entity_type in [DataType.FLOAT_VECTOR, DataType.BINARY_VECTOR]:
+                    field_dim = field["params"]["dim"]
+                    entity_dim = len(entity["values"][0])
+
+                if entity_type in [DataType.FLOAT_VECTOR, ] and entity_dim != field_dim:
+                    raise ParamError(message=f"Collection field dim is {field_dim}"
+                                     f", but entities field dim is {entity_dim}")
+
+                if entity_type in [DataType.BINARY_VECTOR, ] and entity_dim * 8 != field_dim:
+                    raise ParamError(message=f"Collection field dim is {field_dim}"
+                                     f", but entities field dim is {entity_dim * 8}")
+
+                location[field["name"]] = i
+                match_flag = True
+                break
+
+        if not match_flag:
+            raise ParamError(
+                message=f"Field {field['name']} don't match in entities")
+
+    return location, primary_key_loc, auto_id_loc
```

### Comparing `pymilvus-2.2.8/pymilvus/decorators.py` & `pymilvus-2.3.0b1/pymilvus/decorators.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/pymilvus/exceptions.py` & `pymilvus-2.3.0b1/pymilvus/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,18 @@
     """ Raise when autoID is invalid """
 
 
 class InvalidConsistencyLevel(MilvusException):
     """ Raise when consistency level is invalid """
 
 
+class UpsertAutoIDTrueException(MilvusException):
+    """ Raise when upsert autoID is true """
+
+
 class ExceptionsMessage:
     NoHostPort = "connection configuration must contain 'host' and 'port'."
     HostType = "Type of 'host' must be str."
     PortType = "Type of 'port' must be str or int."
     ConnDiffConf = "Alias of %r already creating connections, but the configure is not the same as passed in."
     AliasType = "Alias should be string, but %r is given."
     ConnLackConf = "You need to pass in the configuration of the connection named %r ."
@@ -161,7 +165,8 @@
     CollectionType = "The type of collection must be pymilvus.Collection."
     FieldsType = "The fields of schema must be type list."
     FieldType = "The field of schema type must be FieldSchema."
     FieldDtype = "Field dtype must be of DataType"
     ExprType = "The type of expr must be string ,but %r is given."
     EnvConfigErr = "Environment variable %s has a wrong format, please check it: %s"
     AmbiguousIndexName = "There are multiple indexes, please specify the index_name."
+    UpsertAutoIDTrue = "Upsert don't support autoid == true"
```

### Comparing `pymilvus-2.2.8/pymilvus/grpc_gen/milvus_pb2_grpc.py` & `pymilvus-2.3.0b1/pymilvus/grpc_gen/milvus_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,19 @@
                 response_deserializer=milvus__pb2.MutationResult.FromString,
                 )
         self.Delete = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/Delete',
                 request_serializer=milvus__pb2.DeleteRequest.SerializeToString,
                 response_deserializer=milvus__pb2.MutationResult.FromString,
                 )
+        self.Upsert = channel.unary_unary(
+                '/milvus.proto.milvus.MilvusService/Upsert',
+                request_serializer=milvus__pb2.UpsertRequest.SerializeToString,
+                response_deserializer=milvus__pb2.MutationResult.FromString,
+                )
         self.Search = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/Search',
                 request_serializer=milvus__pb2.SearchRequest.SerializeToString,
                 response_deserializer=milvus__pb2.SearchResults.FromString,
                 )
         self.Flush = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/Flush',
@@ -171,29 +176,19 @@
                 response_deserializer=milvus__pb2.QueryResults.FromString,
                 )
         self.CalcDistance = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/CalcDistance',
                 request_serializer=milvus__pb2.CalcDistanceRequest.SerializeToString,
                 response_deserializer=milvus__pb2.CalcDistanceResults.FromString,
                 )
-        self.FlushAll = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/FlushAll',
-                request_serializer=milvus__pb2.FlushAllRequest.SerializeToString,
-                response_deserializer=milvus__pb2.FlushAllResponse.FromString,
-                )
         self.GetFlushState = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/GetFlushState',
                 request_serializer=milvus__pb2.GetFlushStateRequest.SerializeToString,
                 response_deserializer=milvus__pb2.GetFlushStateResponse.FromString,
                 )
-        self.GetFlushAllState = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/GetFlushAllState',
-                request_serializer=milvus__pb2.GetFlushAllStateRequest.SerializeToString,
-                response_deserializer=milvus__pb2.GetFlushAllStateResponse.FromString,
-                )
         self.GetPersistentSegmentInfo = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/GetPersistentSegmentInfo',
                 request_serializer=milvus__pb2.GetPersistentSegmentInfoRequest.SerializeToString,
                 response_deserializer=milvus__pb2.GetPersistentSegmentInfoResponse.FromString,
                 )
         self.GetQuerySegmentInfo = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/GetQuerySegmentInfo',
@@ -356,29 +351,14 @@
                 response_deserializer=milvus__pb2.DescribeResourceGroupResponse.FromString,
                 )
         self.RenameCollection = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/RenameCollection',
                 request_serializer=milvus__pb2.RenameCollectionRequest.SerializeToString,
                 response_deserializer=common__pb2.Status.FromString,
                 )
-        self.CreateDatabase = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/CreateDatabase',
-                request_serializer=milvus__pb2.CreateDatabaseRequest.SerializeToString,
-                response_deserializer=common__pb2.Status.FromString,
-                )
-        self.DropDatabase = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/DropDatabase',
-                request_serializer=milvus__pb2.CreateDatabaseRequest.SerializeToString,
-                response_deserializer=common__pb2.Status.FromString,
-                )
-        self.ListDatabases = channel.unary_unary(
-                '/milvus.proto.milvus.MilvusService/ListDatabases',
-                request_serializer=milvus__pb2.ListDatabasesRequest.SerializeToString,
-                response_deserializer=milvus__pb2.ListDatabasesResponse.FromString,
-                )
 
 
 class MilvusServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def CreateCollection(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -546,56 +526,50 @@
 
     def Delete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Search(self, request, context):
+    def Upsert(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Flush(self, request, context):
+    def Search(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Query(self, request, context):
+    def Flush(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CalcDistance(self, request, context):
+    def Query(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def FlushAll(self, request, context):
+    def CalcDistance(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFlushState(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetFlushAllState(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def GetPersistentSegmentInfo(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetQuerySegmentInfo(self, request, context):
@@ -797,32 +771,14 @@
 
     def RenameCollection(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateDatabase(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def DropDatabase(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def ListDatabases(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
 
 def add_MilvusServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CreateCollection': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateCollection,
                     request_deserializer=milvus__pb2.CreateCollectionRequest.FromString,
                     response_serializer=common__pb2.Status.SerializeToString,
@@ -958,14 +914,19 @@
                     response_serializer=milvus__pb2.MutationResult.SerializeToString,
             ),
             'Delete': grpc.unary_unary_rpc_method_handler(
                     servicer.Delete,
                     request_deserializer=milvus__pb2.DeleteRequest.FromString,
                     response_serializer=milvus__pb2.MutationResult.SerializeToString,
             ),
+            'Upsert': grpc.unary_unary_rpc_method_handler(
+                    servicer.Upsert,
+                    request_deserializer=milvus__pb2.UpsertRequest.FromString,
+                    response_serializer=milvus__pb2.MutationResult.SerializeToString,
+            ),
             'Search': grpc.unary_unary_rpc_method_handler(
                     servicer.Search,
                     request_deserializer=milvus__pb2.SearchRequest.FromString,
                     response_serializer=milvus__pb2.SearchResults.SerializeToString,
             ),
             'Flush': grpc.unary_unary_rpc_method_handler(
                     servicer.Flush,
@@ -978,29 +939,19 @@
                     response_serializer=milvus__pb2.QueryResults.SerializeToString,
             ),
             'CalcDistance': grpc.unary_unary_rpc_method_handler(
                     servicer.CalcDistance,
                     request_deserializer=milvus__pb2.CalcDistanceRequest.FromString,
                     response_serializer=milvus__pb2.CalcDistanceResults.SerializeToString,
             ),
-            'FlushAll': grpc.unary_unary_rpc_method_handler(
-                    servicer.FlushAll,
-                    request_deserializer=milvus__pb2.FlushAllRequest.FromString,
-                    response_serializer=milvus__pb2.FlushAllResponse.SerializeToString,
-            ),
             'GetFlushState': grpc.unary_unary_rpc_method_handler(
                     servicer.GetFlushState,
                     request_deserializer=milvus__pb2.GetFlushStateRequest.FromString,
                     response_serializer=milvus__pb2.GetFlushStateResponse.SerializeToString,
             ),
-            'GetFlushAllState': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetFlushAllState,
-                    request_deserializer=milvus__pb2.GetFlushAllStateRequest.FromString,
-                    response_serializer=milvus__pb2.GetFlushAllStateResponse.SerializeToString,
-            ),
             'GetPersistentSegmentInfo': grpc.unary_unary_rpc_method_handler(
                     servicer.GetPersistentSegmentInfo,
                     request_deserializer=milvus__pb2.GetPersistentSegmentInfoRequest.FromString,
                     response_serializer=milvus__pb2.GetPersistentSegmentInfoResponse.SerializeToString,
             ),
             'GetQuerySegmentInfo': grpc.unary_unary_rpc_method_handler(
                     servicer.GetQuerySegmentInfo,
@@ -1163,29 +1114,14 @@
                     response_serializer=milvus__pb2.DescribeResourceGroupResponse.SerializeToString,
             ),
             'RenameCollection': grpc.unary_unary_rpc_method_handler(
                     servicer.RenameCollection,
                     request_deserializer=milvus__pb2.RenameCollectionRequest.FromString,
                     response_serializer=common__pb2.Status.SerializeToString,
             ),
-            'CreateDatabase': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateDatabase,
-                    request_deserializer=milvus__pb2.CreateDatabaseRequest.FromString,
-                    response_serializer=common__pb2.Status.SerializeToString,
-            ),
-            'DropDatabase': grpc.unary_unary_rpc_method_handler(
-                    servicer.DropDatabase,
-                    request_deserializer=milvus__pb2.CreateDatabaseRequest.FromString,
-                    response_serializer=common__pb2.Status.SerializeToString,
-            ),
-            'ListDatabases': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListDatabases,
-                    request_deserializer=milvus__pb2.ListDatabasesRequest.FromString,
-                    response_serializer=milvus__pb2.ListDatabasesResponse.SerializeToString,
-            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'milvus.proto.milvus.MilvusService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -1665,14 +1601,31 @@
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/Delete',
             milvus__pb2.DeleteRequest.SerializeToString,
             milvus__pb2.MutationResult.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def Upsert(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/Upsert',
+            milvus__pb2.UpsertRequest.SerializeToString,
+            milvus__pb2.MutationResult.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def Search(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1733,31 +1686,14 @@
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/CalcDistance',
             milvus__pb2.CalcDistanceRequest.SerializeToString,
             milvus__pb2.CalcDistanceResults.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def FlushAll(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/FlushAll',
-            milvus__pb2.FlushAllRequest.SerializeToString,
-            milvus__pb2.FlushAllResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def GetFlushState(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1767,31 +1703,14 @@
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/GetFlushState',
             milvus__pb2.GetFlushStateRequest.SerializeToString,
             milvus__pb2.GetFlushStateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetFlushAllState(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/GetFlushAllState',
-            milvus__pb2.GetFlushAllStateRequest.SerializeToString,
-            milvus__pb2.GetFlushAllStateResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def GetPersistentSegmentInfo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -2361,65 +2280,14 @@
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/RenameCollection',
             milvus__pb2.RenameCollectionRequest.SerializeToString,
             common__pb2.Status.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
-    @staticmethod
-    def CreateDatabase(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/CreateDatabase',
-            milvus__pb2.CreateDatabaseRequest.SerializeToString,
-            common__pb2.Status.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def DropDatabase(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/DropDatabase',
-            milvus__pb2.CreateDatabaseRequest.SerializeToString,
-            common__pb2.Status.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ListDatabases(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/ListDatabases',
-            milvus__pb2.ListDatabasesRequest.SerializeToString,
-            milvus__pb2.ListDatabasesResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
 
 class ProxyServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `pymilvus-2.2.8/pymilvus/orm/__init__.py` & `pymilvus-2.3.0b1/pymilvus/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/pymilvus/orm/collection.py` & `pymilvus-2.3.0b1/pymilvus/orm/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 import copy
 import json
-from typing import List
+from typing import List, Union
 import pandas
 
 from .connections import connections
 from .schema import (
     CollectionSchema,
     FieldSchema,
     parse_fields_from_data,
-    check_insert_data_schema,
+    check_insert_or_upsert_data_schema,
     check_schema,
 )
 from .prepare import Prepare
 from .partition import Partition
 from .index import Index
 from .search import SearchResult
 from .mutation import MutationResult
@@ -36,31 +36,32 @@
     PartitionNotExistException,
     IndexNotExistException,
     AutoIDException,
     ExceptionsMessage,
 )
 from .future import SearchFuture, MutationFuture
 from .utility import _get_connection
-from ..settings import Config
+from .default_config import DefaultConfig
 from ..client.types import CompactionState, CompactionPlans, Replica, get_consistency_level, cmp_consistency_level
 from ..client.constants import DEFAULT_CONSISTENCY_LEVEL
+from ..client.configs import DefaultConfigs
 
 
 
 class Collection:
-    def __init__(self, name: str, schema: CollectionSchema=None, using: str="default",  **kwargs):
+    def __init__(self, name: str, schema: CollectionSchema=None, using: str="default", shards_num: int=2, **kwargs):
         """ Constructs a collection by name, schema and other parameters.
 
         Args:
             name (``str``): the name of collection
             schema (``CollectionSchema``, optional): the schema of collection, defaults to None.
             using (``str``, optional): Milvus connection alias name, defaults to 'default'.
+            shards_num (``int``, optional): how many shards will the insert data be divided, defaults to 2.
             **kwargs (``dict``):
 
-                * *shards_num (``int``, optional): how many shards will the insert data be divided.
                 * *consistency_level* (``int/ str``)
                     Which consistency level to use when searching in the collection.
                     Options of consistency level: Strong, Bounded, Eventually, Session, Customized.
 
                     Note: this parameter can be overwritten by the same parameter specified in search.
 
                 * *properties* (``dict``, optional)
@@ -84,14 +85,15 @@
             >>> properties = {"collection.ttl.seconds": 1800}
             >>> collection = Collection(name="test_collection_init", schema=schema, properties=properties)
             >>> collection.name
             'test_collection_init'
         """
         self._name = name
         self._using = using
+        self._shards_num = shards_num
         self._kwargs = kwargs
         conn = self._get_connection()
 
         has = conn.has_collection(self._name, **kwargs)
         if has:
             resp = conn.describe_collection(self._name, **kwargs)
             s_consistency_level = resp.get("consistency_level", DEFAULT_CONSISTENCY_LEVEL)
@@ -111,27 +113,27 @@
 
         else:
             if schema is None:
                 raise SchemaNotReadyException(message=ExceptionsMessage.CollectionNotExistNoSchema % name)
             if isinstance(schema, CollectionSchema):
                 check_schema(schema)
                 consistency_level = get_consistency_level(kwargs.get("consistency_level", DEFAULT_CONSISTENCY_LEVEL))
-
-                conn.create_collection(self._name, schema, **kwargs)
+                conn.create_collection(self._name, schema, shards_num=self._shards_num, **kwargs)
                 self._schema = schema
                 self._consistency_level = consistency_level
             else:
                 raise SchemaNotReadyException(message=ExceptionsMessage.SchemaType)
 
         self._schema_dict = self._schema.to_dict()
         self._schema_dict["consistency_level"] = self._consistency_level
 
     def __repr__(self):
         _dict = {
             'name': self.name,
+            'partitions': self.partitions,
             'description': self.description,
             'schema': self._schema,
         }
         r = ["<Collection>:\n-------------\n"]
         s = "<{}>: {}\n"
         for k, v in _dict.items():
             r.append(s.format(k, v))
@@ -161,15 +163,15 @@
         auto_id = kwargs.pop("auto_id", False)
         if auto_id:
             if dataframe[primary_field].isnull().all():
                 dataframe = dataframe.drop(primary_field, axis=1)
             else:
                 raise SchemaNotReadyException(message=ExceptionsMessage.AutoIDWithData)
 
-        using = kwargs.get("using", Config.MILVUS_CONN_ALIAS)
+        using = kwargs.get("using", DefaultConfig.DEFAULT_USING)
         conn = _get_connection(using)
         if conn.has_collection(name, **kwargs):
             resp = conn.describe_collection(name, **kwargs)
             server_schema = CollectionSchema.construct_from_dict(resp)
             schema = server_schema
         else:
             fields_schema = parse_fields_from_data(dataframe)
@@ -180,15 +182,15 @@
                                                  **kwargs))
 
             for field in fields_schema:
                 if auto_id is False and field.name == primary_field:
                     field.is_primary = True
                     field.auto_id = False
                 if field.dtype == DataType.VARCHAR:
-                    field.params[Config.MaxVarCharLengthKey] = int(Config.MaxVarCharLength)
+                    field.params[DefaultConfigs.MaxVarCharLengthKey] = int(DefaultConfigs.MaxVarCharLength)
             schema = CollectionSchema(fields=fields_schema)
 
         check_schema(schema)
         collection = cls(name, schema, **kwargs)
         res = collection.insert(data=dataframe)
         return collection, res
 
@@ -382,15 +384,15 @@
             >>> collection.create_index("films", {"index_type": "FLAT", "metric_type": "L2", "params": {}})
             >>> collection.load()
             >>> collection.release()
         """
         conn = self._get_connection()
         conn.release_collection(self._name, timeout=timeout, **kwargs)
 
-    def insert(self, data: [List, pandas.DataFrame], partition_name: str=None, timeout=None, **kwargs) -> MutationResult:
+    def insert(self, data: Union[List, pandas.DataFrame], partition_name: str=None, timeout=None, **kwargs) -> MutationResult:
         """ Insert data into the collection.
 
         Args:
             data (``list/tuple/pandas.DataFrame``): The specified data to insert
             partition_name (``str``): The partition name which the data will be inserted to,
                 if partition name is not passed, then the data will be inserted to "_default" partition
             timeout (``float``, optional): A duration of time in seconds to allow for the RPC. Defaults to None.
@@ -417,16 +419,16 @@
             ... ]
             >>> res = collection.insert(data)
             >>> res.insert_count
             10
         """
         if data is None:
             return MutationResult(data)
-        check_insert_data_schema(self._schema, data)
-        entities = Prepare.prepare_insert_data(data, self._schema)
+        check_insert_or_upsert_data_schema(self._schema, data)
+        entities = Prepare.prepare_insert_or_upsert_data(data, self._schema)
 
         conn = self._get_connection()
         res = conn.batch_insert(self._name, entities, partition_name,
                                 timeout=timeout, schema=self._schema_dict, **kwargs)
 
         if kwargs.get("_async", False):
             return MutationFuture(res)
@@ -471,14 +473,60 @@
 
         conn = self._get_connection()
         res = conn.delete(self._name, expr, partition_name, timeout=timeout, **kwargs)
         if kwargs.get("_async", False):
             return MutationFuture(res)
         return MutationResult(res)
 
+    def upsert(self, data: Union[List, pandas.DataFrame], partition_name: str=None, timeout=None, **kwargs) -> MutationResult:
+        """ Upsert data into the collection.
+
+        Args:
+            data (``list/tuple/pandas.DataFrame``): The specified data to upsert
+            partition_name (``str``): The partition name which the data will be upserted at,
+                if partition name is not passed, then the data will be upserted in "_default" partition
+            timeout (``float``, optional): A duration of time in seconds to allow for the RPC. Defaults to None.
+                If timeout is set to None, the client keeps waiting until the server responds or an error occurs.
+        Returns:
+            MutationResult: contains 2 properties `upsert_count`, and, `primary_keys`
+                `upsert_count`: how may entites have been upserted at Milvus,
+                `primary_keys`: list of primary keys of the upserted entities
+        Raises:
+            MilvusException: If anything goes wrong.
+
+        Examples:
+            >>> from pymilvus import connections, Collection, FieldSchema, CollectionSchema, DataType
+            >>> import random
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_collection_upsert", schema)
+            >>> data = [
+            ...     [random.randint(1, 100) for _ in range(10)],
+            ...     [[random.random() for _ in range(2)] for _ in range(10)],
+            ... ]
+            >>> res = collection.upsert(data)
+            >>> res.upsert_count
+            10
+        """
+        if data is None:
+            return MutationResult(data)
+        check_insert_or_upsert_data_schema(self._schema, data, False)
+        entities = Prepare.prepare_insert_or_upsert_data(data, self._schema, False)
+
+        conn = self._get_connection()
+        res = conn.upsert(self._name, entities, partition_name,
+                                timeout=timeout, schema=self._schema_dict, **kwargs)
+
+        if kwargs.get("_async", False):
+            return MutationFuture(res)
+        return MutationResult(res)
+
     def search(self, data, anns_field, param, limit, expr=None, partition_names=None,
                output_fields=None, timeout=None, round_decimal=-1, **kwargs):
         """ Conducts a vector similarity search with an optional boolean expression as filter.
 
         Args:
             data (``List[List[float]]``): The vectors of search data.
                 the length of data is number of query (nq), and the dim of every vector in data must be equal to
@@ -899,15 +947,15 @@
             Status(code=0, message='')
             >>> collection.indexes
             [<pymilvus.index.Index object at 0x7f4435587e20>]
             >>> collection.index()
             <pymilvus.index.Index object at 0x7f44355a1460>
         """
         copy_kwargs = copy.deepcopy(kwargs)
-        index_name = copy_kwargs.pop("index_name", Config.IndexName)
+        index_name = copy_kwargs.pop("index_name", DefaultConfigs.IndexName)
         conn = self._get_connection()
         tmp_index = conn.describe_index(self._name, index_name, **copy_kwargs)
         if tmp_index is not None:
             field_name = tmp_index.pop("field_name", None)
             index_name = tmp_index.pop("index_name", index_name)
             return Index(self, field_name, tmp_index, construct_only=True, index_name=index_name)
         raise IndexNotExistException(message=ExceptionsMessage.IndexNotExist)
@@ -975,15 +1023,15 @@
             >>> index = {"index_type": "IVF_FLAT", "params": {"nlist": 128}, "metric_type": "L2"}
             >>> collection.create_index("films", index)
             >>> collection.has_index()
             True
         """
         conn = self._get_connection()
         copy_kwargs = copy.deepcopy(kwargs)
-        index_name = copy_kwargs.pop("index_name", Config.IndexName)
+        index_name = copy_kwargs.pop("index_name", DefaultConfigs.IndexName)
         if conn.describe_index(self._name, index_name, timeout=timeout, **copy_kwargs) is None:
             return False
         return True
 
     def drop_index(self, timeout=None, **kwargs):
         """ Drop index and its corresponding index files.
         Args:
@@ -1010,15 +1058,15 @@
             >>> collection.has_index()
             True
             >>> collection.drop_index()
             >>> collection.has_index()
             False
         """
         copy_kwargs = copy.deepcopy(kwargs)
-        index_name = copy_kwargs.pop("index_name", Config.IndexName)
+        index_name = copy_kwargs.pop("index_name", DefaultConfigs.IndexName)
         conn = self._get_connection()
         tmp_index = conn.describe_index(self._name, index_name, timeout=timeout, **copy_kwargs)
         if tmp_index is not None:
             index = Index(self, tmp_index['field_name'], tmp_index, construct_only=True, index_name=index_name)
             index.drop(timeout=timeout, **kwargs)
 
     def compact(self, timeout=None, **kwargs):
```

### Comparing `pymilvus-2.2.8/pymilvus/orm/connections.py` & `pymilvus-2.3.0b1/pymilvus/orm/connections.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
+import os
 import copy
+import re
 import threading
 from urllib import parse
 from typing import Tuple
 
 from ..client.check import is_legal_host, is_legal_port, is_legal_address
 from ..client.grpc_handler import GrpcHandler
 
-from ..settings import Config
+from .default_config import DefaultConfig, ENV_CONNECTION_CONF
 from ..exceptions import ExceptionsMessage, ConnectionConfigException, ConnectionNotExistException
 
 
 def synchronized(func):
     """
     Decorator in order to achieve thread-safe singleton class.
     """
@@ -55,80 +57,57 @@
 
 class Connections(metaclass=SingleInstanceMetaClass):
     """ Class for managing all connections of milvus.  Used as a singleton in this module.  """
 
     def __init__(self):
         """ Constructs a default milvus alias config
 
-            default config will be read from env: MILVUS_URI and MILVUS_CONN_ALIAS
-            with default value: default="localhost:19530"
-
-         Read default connection config from environment variable: MILVUS_URI.
-            Format is:
-                [scheme://][<user>@<password>]host[:<port>]
-
-                scheme is one of: http, https, or <empty>
-
-        Examples:
-            localhost
-            localhost:19530
-            test_user@localhost:19530
-            http://test_userlocalhost:19530
-            https://test_user:password@localhost:19530
+            default config will be read from env: MILVUS_DEFAULT_CONNECTION，
+            or "localhost:19530"
 
         """
         self._alias = {}
         self._connected_alias = {}
-        self._env_uri = None
-
-        if Config.MILVUS_URI != "":
-            address, parsed_uri = self.__parse_address_from_uri(Config.MILVUS_URI)
-            self._env_uri = (address, parsed_uri)
-
-            default_conn_config = {
-                "user": parsed_uri.username if parsed_uri.username is not None else "",
-                "address": address,
-            }
-        else:
-            default_conn_config = {
-                "user": "",
-                "address": f"{Config.DEFAULT_HOST}:{Config.DEFAULT_PORT}",
-            }
-
-        self.add_connection(**{Config.MILVUS_CONN_ALIAS: default_conn_config})
-
-    def __verify_host_port(self, host, port):
-        if not is_legal_host(host):
-            raise ConnectionConfigException(message=ExceptionsMessage.HostType)
-        if not is_legal_port(port):
-            raise ConnectionConfigException(message=ExceptionsMessage.PortType)
-        if not 0 <= int(port) < 65535:
-            raise ConnectionConfigException(message=f"port number {port} out of range, valid range [0, 65535)")
 
+        self.add_connection(default=self._read_default_config_from_os_env())
 
-    def __parse_address_from_uri(self, uri: str) -> (str, parse.ParseResult):
-        illegal_uri_msg = "Illegal uri: [{}], expected form 'https://user:pwd@example.com:12345'"
-        try:
-            parsed_uri = parse.urlparse(uri)
-        except (Exception) as e:
-            raise ConnectionConfigException(message=f"{illegal_uri_msg.format(uri)}: <{type(e).__name__}, {e}>") from None
-
-        if len(parsed_uri.netloc) == 0:
-            raise ConnectionConfigException(message=f"{illegal_uri_msg.format(uri)}") from None
-
-        host = parsed_uri.hostname if parsed_uri.hostname is not None else Config.DEFAULT_HOST
-        port = parsed_uri.port if parsed_uri.port is not None else Config.DEFAULT_PORT
-        addr = f"{host}:{port}"
+    def _read_default_config_from_os_env(self):
+        """ Read default connection config from environment variable: MILVUS_DEFAULT_CONNECTION.
+        Format is:
+            [<user>@]host[:<port>]
 
-        self.__verify_host_port(host, port)
-
-        if not is_legal_address(addr):
-            raise ConnectionConfigException(message=illegal_uri_msg.format(uri))
+            protocol is one of: http, https, tcp, or <empty>
+        Examples::
+            localhost
+            localhost:19530
+            test_user@localhost:19530
+        """
 
-        return addr, parsed_uri
+        # no need to adjust http://xxx, https://xxx, tcp://xxxx,
+        # because protocol is ignored
+        # @see __generate_address
+
+        conf = os.getenv(ENV_CONNECTION_CONF, "").strip()
+        if not conf:
+            conf = DefaultConfig.DEFAULT_HOST
+
+        rex = re.compile(r"^(?:([^\s/\\:]+)@)?([^\s/\\:]+)(?::(\d{1,5}))?$")
+        matched = rex.search(conf)
+
+        if not matched:
+            raise ConnectionConfigException(message=ExceptionsMessage.EnvConfigErr % (ENV_CONNECTION_CONF, conf))
+
+        user, host, port = matched.groups()
+        user = user or ""
+        port = port or DefaultConfig.DEFAULT_PORT
+
+        return {
+            "user": user,
+            "address": f"{host}:{port}"
+        }
 
     def add_connection(self, **kwargs):
         """ Configures a milvus connection.
 
         Addresses priority in kwargs: address, uri, host and port
 
         :param kwargs:
@@ -153,15 +132,15 @@
                 dev3={"uri": "http://localhost:19530"},
                 dev4={"uri": "tcp://localhost:19530"},
                 dev5={"address": "localhost:19530"},
                 prod={"uri": "http://random.random.random.com:19530"},
             )
         """
         for alias, config in kwargs.items():
-            addr, _ = self.__get_full_address(
+            addr = self.__get_full_address(
                 config.get("address", ""),
                 config.get("uri", ""),
                 config.get("host", ""),
                 config.get("port", ""))
 
             if alias in self._connected_alias:
                 if self._alias[alias].get("address") != addr:
@@ -170,29 +149,50 @@
             alias_config = {
                 "address": addr,
                 "user": config.get("user", ""),
             }
 
             self._alias[alias] = alias_config
 
-    def __get_full_address(self, address: str = "", uri: str = "", host: str = "", port: str = "") -> (str, parse.ParseResult):
+    def __get_full_address(self, address: str = "", uri: str = "", host: str = "", port: str = "") -> str:
         if address != "":
             if not is_legal_address(address):
                 raise ConnectionConfigException(message=f"Illegal address: {address}, should be in form 'localhost:19530'")
-            return address, None
+        else:
+            address = self.__generate_address(uri, host, port)
 
+        return address
+
+    def __generate_address(self, uri: str, host: str, port: str) -> str:
+        illegal_uri_msg = "Illegal uri: [{}], should be in form 'http://example.com' or 'tcp://6.6.6.6:12345'"
         if uri != "":
-            address, parsed = self.__parse_address_from_uri(uri)
-            return address, parsed
+            try:
+                parsed_uri = parse.urlparse(uri)
+            except (Exception) as e:
+                raise ConnectionConfigException(message=f"{illegal_uri_msg.format(uri)}: <{type(e).__name__}, {e}>") from None
+
+            if len(parsed_uri.netloc) == 0:
+                raise ConnectionConfigException(message=illegal_uri_msg.format(uri))
+
+            addr = parsed_uri.netloc if ":" in parsed_uri.netloc else f"{parsed_uri.netloc}:{DefaultConfig.DEFAULT_PORT}"
+            if not is_legal_address(addr):
+                raise ConnectionConfigException(message=illegal_uri_msg.format(uri))
+            return addr
+
+        host = host if host != "" else DefaultConfig.DEFAULT_HOST
+        port = port if port != "" else DefaultConfig.DEFAULT_PORT
 
-        host = host if host != "" else Config.DEFAULT_HOST
-        port = port if port != "" else Config.DEFAULT_PORT
-        self.__verify_host_port(host, port)
+        if not is_legal_host(host):
+            raise ConnectionConfigException(message=ExceptionsMessage.HostType)
+        if not is_legal_port(port):
+            raise ConnectionConfigException(message=ExceptionsMessage.PortType)
+        if not 0 <= int(port) < 65535:
+            raise ConnectionConfigException(message=f"port number {port} out of range, valid range [0, 65535)")
 
-        return f"{host}:{port}", None
+        return f"{host}:{port}"
 
     def disconnect(self, alias: str):
         """ Disconnects connection from the registry.
 
         :param alias: The name of milvus connection
         :type alias: str
         """
@@ -210,15 +210,15 @@
         """
         if not isinstance(alias, str):
             raise ConnectionConfigException(message=ExceptionsMessage.AliasType % type(alias))
 
         self.disconnect(alias)
         self._alias.pop(alias, None)
 
-    def connect(self, alias=Config.MILVUS_CONN_ALIAS, user="", password="", **kwargs):
+    def connect(self, alias=DefaultConfig.DEFAULT_USING, user="", password="", **kwargs):
         """
         Constructs a milvus connection and register it under given alias.
 
         :param alias: The name of milvus connection
         :type  alias: str
 
         :param kwargs:
@@ -230,22 +230,22 @@
 
             * *host* (``str``) -- Optional. The host of Milvus instance.
                 Default at "localhost", PyMilvus will fill in the default host if only port is provided.
 
             * *port* (``str/int``) -- Optional. The port of Milvus instance.
                 Default at 19530, PyMilvus will fill in the default port if only host is provided.
 
-            * *secure* (``bool``) --
-                Optional. Default is false. If set to true, tls will be enabled.
             * *user* (``str``) --
                 Optional. Use which user to connect to Milvus instance. If user and password
                 are provided, we will add related header in every RPC call.
             * *password* (``str``) --
                 Optional and required when user is provided. The password corresponding to
                 the user.
+            * *secure* (``bool``) --
+                Optional. Default is false. If set to true, tls will be enabled.
             * *client_key_path* (``str``) --
                 Optional. If use tls two-way authentication, need to write the client.key path.
             * *client_pem_path* (``str``) --
                 Optional. If use tls two-way authentication, need to write the client.pem path.
             * *ca_pem_path* (``str``) --
                 Optional. If use tls two-way authentication, need to write the ca.pem path.
             * *server_pem_path* (``str``) --
@@ -258,19 +258,22 @@
         :raises Exception: If server specified in parameters is not ready, we cannot connect to
                            server.
 
         :example:
             >>> from pymilvus import connections
             >>> connections.connect("test", host="localhost", port="19530")
         """
+        if not isinstance(alias, str):
+            raise ConnectionConfigException(message=ExceptionsMessage.AliasType % type(alias))
+
         def connect_milvus(**kwargs):
             gh = GrpcHandler(**kwargs)
 
             t = kwargs.get("timeout")
-            timeout = t if isinstance(t, (int, float)) else Config.MILVUS_CONN_TIMEOUT
+            timeout = t if isinstance(t, (int, float)) else DefaultConfig.DEFAULT_CONNECT_TIMEOUT
 
             gh._wait_for_channel_ready(timeout=timeout)
             kwargs.pop('password')
             kwargs.pop('secure', None)
 
             self._connected_alias[alias] = gh
             self._alias[alias] = copy.deepcopy(kwargs)
@@ -278,68 +281,38 @@
         def with_config(config: Tuple) -> bool:
             for c in config:
                 if c != "":
                     return True
 
             return False
 
-        if not isinstance(alias, str):
-            raise ConnectionConfigException(message=ExceptionsMessage.AliasType % type(alias))
-
         config = (
             kwargs.pop("address", ""),
             kwargs.pop("uri", ""),
             kwargs.pop("host", ""),
             kwargs.pop("port", "")
         )
 
-        # 1st Priority: connection from params
         if with_config(config):
-            in_addr, parsed_uri = self.__get_full_address(*config)
+            in_addr = self.__get_full_address(*config)
             kwargs["address"] = in_addr
 
             if self.has_connection(alias):
                 if self._alias[alias].get("address") != in_addr:
                     raise ConnectionConfigException(message=ExceptionsMessage.ConnDiffConf % alias)
 
-            # uri might take extra info
-            if parsed_uri is not None:
-                user = parsed_uri.username if parsed_uri.username is not None else user
-                password = parsed_uri.password if parsed_uri.password is not None else password
-                # Set secure=True if uri provided user and password
-                if len(user) > 0 and len(password) > 0:
-                    kwargs["secure"] = True
-
             connect_milvus(**kwargs, user=user, password=password)
-            return
-
-        # 2nd Priority, connection configs from env
-        if self._env_uri is not None:
-            addr, parsed_uri = self._env_uri
-            kwargs["address"] = addr
-
-            user = parsed_uri.username if parsed_uri.username is not None else ""
-            password = parsed_uri.password if parsed_uri.password is not None else ""
-            # Set secure=True if uri provided user and password
-            if len(user) > 0 and len(password) > 0:
-                kwargs["secure"] = True
 
-            connect_milvus(**kwargs, user=user, password=password)
-            return
+        else:
+            if alias not in self._alias:
+                raise ConnectionConfigException(message=ExceptionsMessage.ConnLackConf % alias)
 
-        # 3rd Priority, connect to cached configs with provided user and password
-        if alias in self._alias:
             connect_alias = dict(self._alias[alias].items())
             connect_alias["user"] = user
             connect_milvus(**connect_alias, password=password, **kwargs)
-            return
-
-        # No params, env, and cached configs for the alias
-        raise ConnectionConfigException(message=ExceptionsMessage.ConnLackConf % alias)
-
 
     def list_connections(self) -> list:
         """ List names of all connections.
 
         :return list:
             Names of all connections.
 
@@ -392,15 +365,15 @@
             >>> connections.get_connection_addr('test')
             {'host': 'localhost', 'port': '19530'}
         """
         if not isinstance(alias, str):
             raise ConnectionConfigException(message=ExceptionsMessage.AliasType % type(alias))
         return alias in self._connected_alias
 
-    def _fetch_handler(self, alias=Config.MILVUS_CONN_ALIAS) -> GrpcHandler:
+    def _fetch_handler(self, alias=DefaultConfig.DEFAULT_USING) -> GrpcHandler:
         """ Retrieves a GrpcHandler by alias. """
         if not isinstance(alias, str):
             raise ConnectionConfigException(message=ExceptionsMessage.AliasType % type(alias))
 
         conn = self._connected_alias.get(alias, None)
         if conn is None:
             raise ConnectionNotExistException(message=ExceptionsMessage.ConnectFirst)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymilvus-2.2.8/pymilvus/orm/constants.py` & `pymilvus-2.3.0b1/pymilvus/orm/constants.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/pymilvus/orm/future.py` & `pymilvus-2.3.0b1/pymilvus/orm/future.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/pymilvus/orm/index.py` & `pymilvus-2.3.0b1/pymilvus/orm/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 import copy
 
 from ..exceptions import CollectionNotExistException, ExceptionsMessage
-from ..settings import Config
+from ..client.configs import DefaultConfigs
 
 
 class Index:
     def __init__(self, collection, field_name, index_params, **kwargs):
         """
         Creates index on a specified field according to the index parameters.
 
@@ -60,15 +60,15 @@
         """
         from .collection import Collection
         if not isinstance(collection, Collection):
             raise CollectionNotExistException(message=ExceptionsMessage.CollectionType)
         self._collection = collection
         self._field_name = field_name
         self._index_params = index_params
-        index_name = kwargs.get("index_name", Config.IndexName)
+        index_name = kwargs.get("index_name", DefaultConfigs.IndexName)
         self._index_name = index_name
         self._kwargs = kwargs
         if self._kwargs.pop("construct_only", False):
             return
 
         conn = self._get_connection()
         conn.create_index(self._collection.name, self._field_name, self._index_params, **kwargs)
@@ -151,10 +151,10 @@
 
         :param kwargs:
             * *index_name* (``str``) --
               The name of index. If no index is specified, the default index name is used.
 
         """
         copy_kwargs = copy.deepcopy(kwargs)
-        index_name = copy_kwargs.pop("index_name", Config.IndexName)
+        index_name = copy_kwargs.pop("index_name", DefaultConfigs.IndexName)
         conn = self._get_connection()
         conn.drop_index(self._collection.name, self.field_name, index_name, timeout=timeout, **copy_kwargs)
```

### Comparing `pymilvus-2.2.8/pymilvus/orm/mutation.py` & `pymilvus-2.3.0b1/pymilvus/orm/mutation.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/pymilvus/orm/partition.py` & `pymilvus-2.3.0b1/pymilvus/orm/partition.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,104 +6,139 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
+import copy
 import json
-from typing import Union, List
-
-import pandas
 
 from ..exceptions import (
     CollectionNotExistException,
     PartitionNotExistException,
     ExceptionsMessage,
 )
 
+from .prepare import Prepare
 from .search import SearchResult
 from .mutation import MutationResult
+from .future import SearchFuture, MutationFuture
 from ..client.types import Replica
 
 
 class Partition:
     def __init__(self, collection, name, description="", **kwargs):
+        # TODO: Need a place to store the description
         from .collection import Collection
         if not isinstance(collection, Collection):
             raise CollectionNotExistException(message=ExceptionsMessage.CollectionType)
         self._collection = collection
         self._name = name
         self._description = description
+        self._schema = collection._schema
+        self._consistency_level = collection._consistency_level
+        self._kwargs = kwargs
 
+        conn = self._get_connection()
         if kwargs.get("construct_only", False):
             return
+        copy_kwargs = copy.deepcopy(kwargs)
+        if copy_kwargs.get("partition_name"):
+            copy_kwargs.pop("partition_name")
+        has = conn.has_partition(self._collection.name, self._name, **copy_kwargs)
+        if not has:
+            conn.create_partition(self._collection.name, self._name, **copy_kwargs)
 
-        if not self._collection.has_partition(self.name, **kwargs):
-            conn = self._get_connection()
-            conn.create_partition(self._collection.name, self.name, **kwargs)
-
+        self._schema_dict = self._schema.to_dict()
+        self._schema_dict["consistency_level"] = self._consistency_level
 
     def __repr__(self):
         return json.dumps({
             'name': self.name,
             'collection_name': self._collection.name,
             'description': self.description,
         })
 
     def _get_connection(self):
         return self._collection._get_connection()
 
     @property
     def description(self) -> str:
-        """str: discription of the partition.
+        """ Return the description text.
 
-        Examples:
-            >>> from pymilvus import connections, Collection, Partition
+        :return:  Partition description
+        :rtype: str
+
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
             >>> connections.connect()
-            >>> collection = Collection("test_partition_description")
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_description", schema)
             >>> partition = Partition(collection, "comedy", "comedy films")
             >>> partition.description
             'comedy films'
         """
         return self._description
 
     @property
     def name(self) -> str:
-        """str: name of the partition
+        """
+        Return the partition name.
 
-        Examples:
-            >>> from pymilvus import connections, Collection, Partition
+        :return str: Partition name, return when operation is successful
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
             >>> connections.connect()
-            >>> collection = Collection("test_partition_name")
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_name", schema)
             >>> partition = Partition(collection, "comedy", "comedy films")
             >>> partition.name
             'comedy'
         """
         return self._name
 
     @property
     def is_empty(self) -> bool:
-        """bool: whether the partition is empty
+        """
+        Returns whether the partition is empty
+
+        :return bool: Whether the partition is empty
+        * True: The partition is empty.
+        * False: The partition is not empty.
 
-        Examples:
-            >>> from pymilvus import connections, Collection, Partition
+        :example:
+
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
             >>> connections.connect()
-            >>> collection = Collection("test_partition_is_empty")
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_is_empty", schema)
             >>> partition = Partition(collection, "comedy", "comedy films")
             >>> partition.is_empty
             True
         """
         return self.num_entities == 0
 
     @property
     def num_entities(self, **kwargs) -> int:
-        """int: number of entities in the partition
+        """
+        Return the number of entities.
+
+        :return int: Number of entities in this partition.
 
-        Examples:
+        :example:
             >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
             >>> connections.connect()
             >>> schema = CollectionSchema([
             ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
             ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
             ... ])
             >>> collection = Collection("test_partition_num_entities", schema)
@@ -113,182 +148,265 @@
             ...     [[float(i) for i in range(2)] for _ in range(10)],
             ... ]
             >>> partition.insert(data)
             >>> partition.num_entities
             10
         """
         conn = self._get_connection()
-        stats = conn.get_partition_stats(collection_name=self._collection.name, partition_name=self.name, **kwargs)
+        stats = conn.get_partition_stats(collection_name=self._collection.name, partition_name=self._name, **kwargs)
         result = {stat.key: stat.value for stat in stats}
         result["row_count"] = int(result["row_count"])
         return result["row_count"]
 
     def flush(self, timeout=None, **kwargs):
-        """ Seal all segment in the collection of this partition.  Inserts after flushing will be written into
-            new segments. Only sealed segments can be indexed.
-
-        Args:
-            timeout (float): an optional duration of time in seconds to allow for the RPCs.
-                If timeout is not set, the client keeps waiting until the server responds or an error occurs.
-        """
+        """ Flush """
         conn = self._get_connection()
         conn.flush([self._collection.name], timeout=timeout, **kwargs)
 
     def drop(self, timeout=None, **kwargs):
-        """ Drop the partition, the same as Collection.drop_partition
+        """
+        Drop the partition, as well as its corresponding index files.
 
-        Args:
-            timeout (``float``, optional): an optional duration of time in seconds to allow for the RPCs.
-                If timeout is not set, the client keeps waiting until the server responds or an error occurs.
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
 
-        Raises:
-            PartitionNotExistException: If the partitoin doesn't exist
+        :raises PartitionNotExistException:
+            When partitoin does not exist
 
-        Examples:
-            >>> from pymilvus import connections, Collection, Partition
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
             >>> connections.connect()
-            >>> collection = Collection("test_partition_drop")
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_drop", schema)
             >>> partition = Partition(collection, "comedy", "comedy films")
             >>> partition.drop()
         """
         conn = self._get_connection()
-        if conn.has_partition(self._collection.name, self.name, timeout=timeout, **kwargs) is False:
+        if conn.has_partition(self._collection.name, self._name, timeout=timeout, **kwargs) is False:
             raise PartitionNotExistException(message=ExceptionsMessage.PartitionNotExist)
-        return conn.drop_partition(self._collection.name, self.name, timeout=timeout, **kwargs)
+        return conn.drop_partition(self._collection.name, self._name, timeout=timeout, **kwargs)
 
-    def load(self, replica_number: int=1, timeout=None, **kwargs):
-        """ Load the partition data into memory.
+    def load(self, replica_number=1, timeout=None, **kwargs):
+        """
+        Load the partition from disk to memory.
 
-        Args:
-            replica_number (``int``, optional): The replica number to load, defaults to 1.
-            timeout (``float``, optional): an optional duration of time in seconds to allow for the RPCs.
-                If timeout is not set, the client keeps waiting until the server responds or an error occurs.
+        :param replica_number: The replication numbers to load.
+        :type  replica_number: int
 
-        Raises:
-            MilvusException: If anything goes wrong
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
 
-        Examples:
+        :raises ParamError:
+            If params are invalid
+
+        :example:
             >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
             >>> connections.connect()
             >>> schema = CollectionSchema([
             ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
             ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
             ... ])
             >>> collection = Collection("test_partition_load", schema)
             >>> partition = Partition(collection, "comedy", "comedy films")
             >>> partition.load()
         """
+        # TODO(yukun): If field_names is not None and not equal schema.field_names,
+        #  raise Exception Not Supported,
+        #  if index_names is not None, raise Exception Not Supported
         conn = self._get_connection()
-        if conn.has_partition(self._collection.name, self.name, **kwargs):
-            return conn.load_partitions(self._collection.name, [self.name], replica_number, timeout=timeout, **kwargs)
+        if conn.has_partition(self._collection.name, self._name, **kwargs):
+            return conn.load_partitions(self._collection.name, [self._name], replica_number, timeout=timeout, **kwargs)
         raise PartitionNotExistException(message=ExceptionsMessage.PartitionNotExist)
 
     def release(self, timeout=None, **kwargs):
-        """ Release the partition data from memory.
+        """
+        Release the partition from memory.
 
-        Args:
-            timeout (``float``, optional): an optional duration of time in seconds to allow for the RPCs.
-                If timeout is not set, the client keeps waiting until the server responds or an error occurs.
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
 
-        Raises:
-            MilvusException: If anything goes wrong
+        :raises PartitionNotExistException:
+            When partitoin does not exist
 
-        Examples:
+        :example:
             >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
             >>> connections.connect()
             >>> schema = CollectionSchema([
             ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
             ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
             ... ])
             >>> collection = Collection("test_partition_release", schema)
             >>> partition = Partition(collection, "comedy", "comedy films")
             >>> partition.load()
             >>> partition.release()
         """
         conn = self._get_connection()
         if conn.has_partition(self._collection.name, self._name, **kwargs):
-            return conn.release_partitions(self._collection.name, [self.name], timeout=timeout, **kwargs)
+            return conn.release_partitions(self._collection.name, [self._name], timeout=timeout, **kwargs)
         raise PartitionNotExistException(message=ExceptionsMessage.PartitionNotExist)
 
-    def insert(self, data: Union[List, pandas.DataFrame], timeout=None, **kwargs) -> MutationResult:
-        """ Insert data into the partition, the same as Collection.insert(data, [partition])
+    def insert(self, data, timeout=None, **kwargs):
+        """
+        Insert data into partition.
 
-        Args:
-            data (``list/tuple/pandas.DataFrame``): The specified data to insert
-            partition_name (``str``): The partition name which the data will be inserted to,
-                if partition name is not passed, then the data will be inserted to "_default" partition
-            timeout (``float``, optional): A duration of time in seconds to allow for the RPC. Defaults to None.
-                If timeout is set to None, the client keeps waiting until the server responds or an error occurs.
-        Returns:
-            MutationResult: contains 2 properties `insert_count`, and, `primary_keys`
-                `insert_count`: how may entites have been inserted into Milvus,
-                `primary_keys`: list of primary keys of the inserted entities
-        Raises:
-            MilvusException: If anything goes wrong.
+        :param data: The specified data to insert, the dimension of data needs to align with column
+                     number
+        :type  data: list-like(list, tuple) object or pandas.DataFrame
 
-        Examples:
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :param kwargs:
+            * *timeout* (``float``) --
+              An optional duration of time in seconds to allow for the RPC. When timeout
+              is set to None, client waits until server response or error occur.
+
+        :return: A MutationResult object contains a property named `insert_count` represents how many
+        entities have been inserted into milvus and a property named `primary_keys` is a list of primary
+        keys of the inserted entities.
+        :rtype: MutationResult
+
+        :raises PartitionNotExistException:
+            When partitoin does not exist
+
+        :example:
             >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
             >>> connections.connect()
             >>> schema = CollectionSchema([
             ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
             ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
             ... ])
             >>> collection = Collection("test_partition_insert", schema)
             >>> partition = Partition(collection, "comedy", "comedy films")
             >>> data = [
             ...     [i for i in range(10)],
             ...     [[float(i) for i in range(2)] for _ in range(10)],
             ... ]
-            >>> res = partition.insert(data)
-            >>> res.insert_count
+            >>> partition.insert(data)
+            >>> partition.num_entities
             10
         """
         conn = self._get_connection()
-        if conn.has_partition(self._collection.name, self.name, **kwargs) is False:
+        if conn.has_partition(self._collection.name, self._name, **kwargs) is False:
             raise PartitionNotExistException(message=ExceptionsMessage.PartitionNotExist)
-
-        return self._collection.insert(data, self.name, timeout=timeout, **kwargs)
+        # TODO: check insert data schema here?
+        entities = Prepare.prepare_insert_or_upsert_data(data, self._collection.schema)
+        res = conn.batch_insert(self._collection.name, entities=entities, partition_name=self._name,
+            timeout=timeout, orm=True, schema=self._schema_dict, **kwargs)
+        if kwargs.get("_async", False):
+            return MutationFuture(res)
+        return MutationResult(res)
 
     def delete(self, expr, timeout=None, **kwargs):
         """ Delete entities with an expression condition.
 
-        Args:
-            expr (``str``): The specified data to insert.
-            partition_names (``List[str]``): Name of partitions to delete entities.
-            timeout (``float``, optional): A duration of time in seconds to allow for the RPC. Defaults to None.
-                If timeout is set to None, the client keeps waiting until the server responds or an error occurs.
-
-        Returns:
-            MutationResult: contains `delete_count` properties represents how many entities might be deleted.
+        :param expr: The expression to specify entities to be deleted
+        :type  expr: str
 
-        Raises:
-            MilvusException: If anything goes wrong.
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :return: A MutationResult object contains a property named `delete_count` represents how many
+                 entities will be deleted.
+        :rtype: MutationResult
+
+        :raises RpcError: If gRPC encounter an error
+        :raises ParamError: If parameters are invalid
+        :raises BaseException: If the return result from server is not ok
 
-        Examples:
+        :example:
             >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
             >>> connections.connect()
             >>> schema = CollectionSchema([
             ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
             ...     FieldSchema("films", DataType.FLOAT_VECTOR, dim=2)
             ... ])
             >>> test_collection = Collection("test_partition_delete", schema)
-            >>> test_partition = Partition(test_collection, "comedy films")
+            >>> test_partition = test_collection.create_partition("comedy", "comedy films")
             >>> data = [
             ...     [i for i in range(10)],
             ...     [[float(i) for i in range(2)] for _ in range(10)],
             ... ]
             >>> test_partition.insert(data)
             (insert count: 10, delete count: 0, upsert count: 0, timestamp: 431044482906718212)
+            >>> test_partition.num_entities
+            10
             >>> test_partition.delete("film_id in [0, 1]")
             (insert count: 0, delete count: 2, upsert count: 0, timestamp: 431044582560759811)
         """
-        return self._collection.delete(expr, self.name, timeout=timeout, **kwargs)
+
+        conn = self._get_connection()
+        res = conn.delete(self._collection.name, expr, self.name, timeout=timeout, **kwargs)
+        if kwargs.get("_async", False):
+            return MutationFuture(res)
+        return MutationResult(res)
+
+    def upsert(self, data, timeout=None, **kwargs):
+        """
+        Upsert data into partition.
+
+        :param data: The specified data to upsert, the dimension of data needs to align with column
+                     number
+        :type  data: list-like(list, tuple) object or pandas.DataFrame
+
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :param kwargs:
+            * *timeout* (``float``) --
+              An optional duration of time in seconds to allow for the RPC. When timeout
+              is set to None, client waits until server response or error occur.
+
+        :return: A MutationResult object contains a property named `upsert_count` represents how many
+        entities have been upserted at milvus and a property named `primary_keys` is a list of primary
+        keys of the upserted entities.
+        :rtype: MutationResult
+
+        :raises PartitionNotExistException:
+            When partitoin does not exist
+
+        :example:
+            >>> from pymilvus import connections, Collection, Partition, FieldSchema, CollectionSchema, DataType
+            >>> connections.connect()
+            >>> schema = CollectionSchema([
+            ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
+            ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
+            ... ])
+            >>> collection = Collection("test_partition_upsert", schema)
+            >>> partition = Partition(collection, "comedy", "comedy films")
+            >>> data = [
+            ...     [i for i in range(10)],
+            ...     [[float(i) for i in range(2)] for _ in range(10)],
+            ... ]
+            >>> partition.upsert(data)
+            >>> partition.num_entities
+            10
+        """
+        conn = self._get_connection()
+        if conn.has_partition(self._collection.name, self._name, **kwargs) is False:
+            raise PartitionNotExistException(message=ExceptionsMessage.PartitionNotExist)
+        # TODO: check upsert data schema here?
+        entities = Prepare.prepare_insert_or_upsert_data(data, self._collection.schema,False)
+        res = conn.upsert(self._collection.name, entities=entities, partition_name=self._name,
+            timeout=timeout, orm=True, schema=self._schema_dict, **kwargs)
+        if kwargs.get("_async", False):
+            return MutationFuture(res)
+        return MutationResult(res)
 
     def search(self, data, anns_field, param, limit,
-               expr=None, output_fields=None, timeout=None, round_decimal=-1, **kwargs) -> SearchResult:
+               expr=None, output_fields=None, timeout=None, round_decimal=-1, **kwargs):
         """ Conducts a vector similarity search with an optional boolean expression as filter.
 
         Args:
             data (``List[List[float]]``): The vectors of search data.
                 the length of data is number of query (nq), and the dim of every vector in data must be equal to
                 the vector field's of collection.
             anns_field (``str``): The name of the vector field used to search of collection.
@@ -372,15 +490,15 @@
             https://milvus.io/docs/v2.2.x/index.md
         .. _How guarantee ts works:
             https://github.com/milvus-io/milvus/blob/master/docs/developer_guides/how-guarantee-ts-works.md
 
         Raises:
             MilvusException: If anything goes wrong
 
-        Examples:
+        :example:
             >>> from pymilvus import connections, Collection, FieldSchema, CollectionSchema, DataType
             >>> import random
             >>> connections.connect()
             >>> schema = CollectionSchema([
             ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
             ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
             ... ])
@@ -407,107 +525,99 @@
             >>> hits = res[0]
             >>> assert len(hits) == 2
             >>> print(f"- Total hits: {len(hits)}, hits ids: {hits.ids} ")
             - Total hits: 2, hits ids: [8, 5]
             >>> print(f"- Top1 hit id: {hits[0].id}, distance: {hits[0].distance}, score: {hits[0].score} ")
             - Top1 hit id: 8, distance: 0.10143111646175385, score: 0.10143111646175385
         """
-
-        return self._collection.search(
-            data=data,
-            anns_field=anns_field,
-            param=param,
-            limit=limit,
-            expr=expr,
-            partition_names=[self.name],
-            output_fields=output_fields,
-            round_decimal=round_decimal,
-            timeout=timeout,
-            **kwargs,
-        )
+        conn = self._get_connection()
+        res = conn.search(self._collection.name, data, anns_field, param, limit, expr, [self._name], output_fields,
+                          round_decimal=round_decimal, timeout=timeout, schema=self._schema_dict, **kwargs)
+        if kwargs.get("_async", False):
+            return SearchFuture(res)
+        return SearchResult(res)
 
     def query(self, expr, output_fields=None, timeout=None, **kwargs):
-        """ Query with expressions
-
-        Args:
-            expr (``str``): The query expression.
-            output_fields(``List[str]``): A list of field names to return. Defaults to None.
-            timeout (``float``, optional): A duration of time in seconds to allow for the RPC. Defaults to None.
-                If timeout is set to None, the client keeps waiting until the server responds or an error occurs.
-            **kwargs (``dict``, optional):
-
-                * *consistency_level* (``str/int``, optional)
-                    Which consistency level to use when searching in the collection.
-
-                    Options of consistency level: Strong, Bounded, Eventually, Session, Customized.
-
-                    Note: this parameter will overwrite the same parameter specified when user created the collection,
-                    if no consistency level was specified, search will use the consistency level when you create the
-                    collection.
-
-                * *guarantee_timestamp* (``int``, optional)
-                    Instructs Milvus to see all operations performed before this timestamp.
-                    By default Milvus will search all operations performed to date.
-
-                    Note: only valid in Customized consistency level.
-
-                * *graceful_time* (``int``, optional)
-                    Search will use the (current_timestamp - the graceful_time) as the
-                    `guarantee_timestamp`. By default with 5s.
-
-                    Note: only valid in Bounded consistency level
-
-                * *travel_timestamp* (``int``, optional)
-                    A specific timestamp to get results based on a data view at.
-
-                * *offset* (``int``)
-                    Combined with limit to enable pagination
+        """
+        Query with a set of criteria, and results in a list of records that match the query exactly.
 
-                * *limit* (``int``)
-                    Combined with limit to enable pagination
+        :param expr: The query expression
+        :type  expr: str
 
-        Returns:
-            List, contains all results
+        :param output_fields: A list of fields to return
+        :type  output_fields: list[str]
 
-        Raises:
-            MilvusException: If anything goes wrong
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :param kwargs:
+            * *consistency_level* (``str/int``) --
+              Which consistency level to use during a query on the collection. For details, see
+              https://github.com/milvus-io/milvus/blob/master/docs/developer_guides/how-guarantee-ts-works.md.
+              Note: this parameter will overwrite the same parameter specified when user created the collection,
+              if no consistency level was specified, query will use the collection consistency level.
+            * *guarantee_timestamp* (``int``) --
+              This function instructs Milvus to see all operations performed before a provided timestamp. If no
+              such timestamp is specified, Milvus will query all operations performed to date.
+              Note: only used in Customized consistency level.
+            * *graceful_time* (``int``) --
+              Only used in bounded consistency level. If graceful_time is set, PyMilvus will use current timestamp minus
+              the graceful_time as the `guarantee_timestamp`. This option is 5s by default if not set.
+            * *travel_timestamp* (``int``) --
+              Users can specify a timestamp in a search to get results based on a data view
+              at a specified point in time.
+
+        :return: A list that contains all results
+        :rtype: list
+
+        :raises RpcError: If gRPC encounter an error
+        :raises ParamError: If parameters are invalid
+        :raises BaseException: If the return result from server is not ok
 
-        Examples:
+        :example:
             >>> from pymilvus import connections, Collection, FieldSchema, CollectionSchema, DataType
             >>> import random
             >>> connections.connect()
+            <pymilvus.client.stub.Milvus object at 0x7f8579002dc0>
             >>> schema = CollectionSchema([
             ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
             ...     FieldSchema("film_date", DataType.INT64),
             ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
             ... ])
             >>> collection = Collection("test_collection_query", schema)
-            >>> collection.create_index("films", {"index_type": "FLAT", "metric_type": "L2", "params": {}})
             >>> partition = Partition(collection, "comedy", "comedy films")
             >>> # insert
             >>> data = [
             ...     [i for i in range(10)],
             ...     [i + 2000 for i in range(10)],
             ...     [[random.random() for _ in range(2)] for _ in range(10)],
             ... ]
             >>> partition.insert(data)
+            >>> partition.num_entities
+            10
             >>> partition.load()
             >>> # query
             >>> expr = "film_id in [ 0, 1 ]"
             >>> res = partition.query(expr, output_fields=["film_date"])
             >>> assert len(res) == 2
             >>> print(f"- Query results: {res}")
             - Query results: [{'film_id': 0, 'film_date': 2000}, {'film_id': 1, 'film_date': 2001}]
         """
-
-        return self._collection.query(expr, output_fields, partition_names=[self.name], timeout=timeout, **kwargs)
+        conn = self._get_connection()
+        res = conn.query(self._collection.name, expr, output_fields, [self._name],
+                         timeout=timeout, schema=self._schema_dict, **kwargs)
+        return res
 
     def get_replicas(self, timeout=None, **kwargs) -> Replica:
-        """Get the current loaded replica information
+        """get_replicas returns the current collection's replica information
 
-        Args:
-            timeout (``float``, optional): An optional duration of time in seconds to allow for the RPC. When timeout
-                is set to None, client waits until server response or error occur.
-        Returns:
-            Replica: All the replica information.
+        :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
+                        is set to None, client waits until server response or error occur
+        :type  timeout: float
+
+        :raises BaseException: If the collection does not exist.
+
+        :example:
         """
-        return self._collection.get_replicas(timeout=timeout, **kwargs)
+        conn = self._get_connection()
+        return conn.get_replicas(self._collection.name, timeout=timeout, **kwargs)
```

### Comparing `pymilvus-2.2.8/pymilvus/orm/prepare.py` & `pymilvus-2.3.0b1/pymilvus/orm/prepare.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,29 +10,36 @@
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 import copy
 
 import numpy
 import pandas
 
-from ..exceptions import DataNotMatchException, DataTypeNotSupportException, ExceptionsMessage
+from ..exceptions import (
+    DataNotMatchException,
+    DataTypeNotSupportException,
+    ExceptionsMessage,
+    UpsertAutoIDTrueException,
+)
 
 
 class Prepare:
     @classmethod
-    def prepare_insert_data(cls, data, schema):
+    def prepare_insert_or_upsert_data(cls, data, schema, isInsert = True):
         if not isinstance(data, (list, tuple, pandas.DataFrame)):
             raise DataTypeNotSupportException(message=ExceptionsMessage.DataTypeNotSupport)
 
         fields = schema.fields
         entities = []  # Entities
         raw_lengths = []  # Check if each row has the same numbers.
 
         if isinstance(data, pandas.DataFrame):
             if schema.auto_id:
+                if isInsert is False:
+                    raise UpsertAutoIDTrueException(message=ExceptionsMessage.UpsertAutoIDTrue)
                 if schema.primary_field.name in data:
                     if len(fields) != len(data.columns):
                         raise DataNotMatchException(message=ExceptionsMessage.FieldsNumInconsistent)
                     if not data[schema.primary_field.name].isnull().all():
                         raise DataNotMatchException(message=ExceptionsMessage.AutoIDWithData)
                 else:
                     if len(fields) != len(data.columns) + 1:
```

### Comparing `pymilvus-2.2.8/pymilvus/orm/role.py` & `pymilvus-2.3.0b1/pymilvus/orm/role.py`

 * *Files 16% similar despite different names*

```diff
@@ -127,88 +127,80 @@
             >>> role = Role(name=role_name)
             >>> is_exist = role.is_exist()
             >>> print(f"the role: {is_exist}")
         """
         roles = self._get_connection().select_one_role(self._name, False)
         return len(roles.groups) != 0
 
-    def grant(self, object: str, object_name: str, privilege: str, db_name: str = "default"):
+    def grant(self, object: str, object_name: str, privilege: str):
         """ Grant a privilege for the role
             :param object: object type.
             :type  object: str
             :param object_name: identifies a specific object name.
             :type  object_name: str
             :param privilege: privilege name.
             :type  privilege: str
-            :param db_name: db name.
-            :type  db_name: str
 
         :example:
             >>> from pymilvus import connections
             >>> from pymilvus.orm.role import Role
             >>> connections.connect()
             >>> role = Role(role_name)
             >>> role.grant("Collection", collection_name, "Insert")
         """
-        return self._get_connection().grant_privilege(self._name, object, object_name, privilege, db_name)
+        return self._get_connection().grant_privilege(self._name, object, object_name, privilege)
 
-    def revoke(self, object: str, object_name: str, privilege: str, db_name: str = "default"):
+    def revoke(self, object: str, object_name: str, privilege: str):
         """ Revoke a privilege for the role
             :param object: object type.
             :type  object: str
             :param object_name: identifies a specific object name.
             :type  object_name: str
             :param privilege: privilege name.
             :type  privilege: str
-            :param db_name: db name.
-            :type  db_name: str
 
         :example:
             >>> from pymilvus import connections
             >>> from pymilvus.orm.role import Role
             >>> connections.connect()
             >>> role = Role(role_name)
             >>> role.revoke("Collection", collection_name, "Insert")
         """
-        return self._get_connection().revoke_privilege(self._name, object, object_name, privilege, db_name)
+        return self._get_connection().revoke_privilege(self._name, object, object_name, privilege)
 
-    def list_grant(self, object: str, object_name: str, db_name: str = "default"):
+    def list_grant(self, object: str, object_name: str):
         """ List a grant info for the role and the specific object
             :param object: object type.
             :type  object: str
             :param object_name: identifies a specific object name.
             :type  object_name: str
-            :param db_name: db name.
-            :type  db_name: str
             :return a GrantInfo object
             :rtype GrantInfo
 
             GrantInfo groups:
             - GrantItem: <object:Collection>, <object_name:foo>, <role_name:x>, <grantor_name:root>, <privilege:Load>
 
         :example:
             >>> from pymilvus import connections
             >>> from pymilvus.orm.role import Role
             >>> connections.connect()
             >>> role = Role(role_name)
             >>> role.list_grant("Collection", collection_name)
         """
-        return self._get_connection().select_grant_for_role_and_object(self._name, object, object_name, db_name)
+        return self._get_connection().select_grant_for_role_and_object(self._name, object, object_name)
 
-    def list_grants(self, db_name: str = "default"):
+    def list_grants(self):
         """ List a grant info for the role
-            :param db_name: db name.
-            :type  db_name: str
             :return a GrantInfo object
             :rtype GrantInfo
 
             GrantInfo groups:
             - GrantItem: <object:Collection>, <object_name:foo>, <role_name:x>, <grantor_name:root>, <privilege:Load>
 
         :example:
             >>> from pymilvus import connections
             >>> from pymilvus.orm.role import Role
             >>> connections.connect()
             >>> role = Role(role_name)
             >>> role.list_grants()
         """
-        return self._get_connection().select_grant_for_one_role(self._name, db_name)
+        return self._get_connection().select_grant_for_one_role(self._name)
```

### Comparing `pymilvus-2.2.8/pymilvus/orm/schema.py` & `pymilvus-2.3.0b1/pymilvus/orm/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 import copy
-from typing import List
+from typing import List, Union
 import pandas
 from pandas.api.types import is_list_like
 
 from .constants import COMMON_TYPE_PARAMS
 from .types import DataType, map_numpy_dtype_to_datatype, infer_dtype_bydata
 from ..exceptions import (
     CannotInferSchemaException,
@@ -23,14 +23,15 @@
     PrimaryKeyException,
     FieldsTypeException,
     FieldTypeException,
     AutoIDException,
     ExceptionsMessage,
     DataNotMatchException,
     SchemaNotReadyException,
+    UpsertAutoIDTrueException
 )
 
 
 class CollectionSchema:
     def __init__(self, fields, description="", **kwargs):
         if not isinstance(fields, list):
             raise FieldsTypeException(message=ExceptionsMessage.FieldsType)
@@ -162,18 +163,18 @@
             "description": self._description,
             "fields": [s.to_dict() for s in self._fields],
         }
         return _dict
 
 
 class FieldSchema:
-    def __init__(self, name: str, dtype: DataType, description="", **kwargs):
+    def __init__(self, name, dtype, description="", **kwargs):
         self.name = name
         try:
-            dtype = DataType(dtype)
+            DataType(dtype)
         except ValueError:
             raise DataTypeNotSupportException(message=ExceptionsMessage.FieldDtype) from None
         if dtype == DataType.UNKNOWN:
             raise DataTypeNotSupportException(message=ExceptionsMessage.FieldDtype)
         self._dtype = dtype
         self._description = description
         self._type_params = {}
@@ -281,38 +282,41 @@
         >>> fvec_field = FieldSchema("fvec", DataType.FLOAT_VECTOR, is_primary=False, dim=128)
         >>> fvec_field.params
         {'dim': 128}
         """
         return self._type_params
 
     @property
-    def dtype(self) -> DataType:
+    def dtype(self):
         return self._dtype
 
 
-def check_insert_data_schema(schema: CollectionSchema, data: [List[List], pandas.DataFrame]) -> None:
-    """ check if the insert data is consist with the collection schema
+def check_insert_or_upsert_data_schema(schema: CollectionSchema, data: Union[List[List], pandas.DataFrame], isInsert=True) -> None:
+    """ check if the insert or upsert data is consist with the collection schema
 
     Args:
         schema (CollectionSchema): the schema of the collection
-        data (List[List], pandas.DataFrame): the data to be inserted
+        data (List[List], pandas.DataFrame): the data to be inserted or upserted
 
     Raise:
         SchemaNotReadyException: if the schema is None
+        UpsertAutoIDTrueException: if autoid option is true
         DataNotMatchException: if the data is in consist with the schema
     """
     if schema is None:
         raise SchemaNotReadyException(message="Schema shouldn't be None")
     if schema.auto_id:
-        if isinstance(data, pandas.DataFrame):
-            if schema.primary_field.name in data:
-                if not data[schema.primary_field.name].isnull().all():
-                    raise DataNotMatchException(message=f"Please don't provide data for auto_id primary field: {schema.primary_field.name}")
-                data = data.drop(schema.primary_field.name, axis=1)
-
+        if isInsert:
+            if isinstance(data, pandas.DataFrame):
+                if schema.primary_field.name in data:
+                    if not data[schema.primary_field.name].isnull().all():
+                        raise DataNotMatchException(message=f"Please don't provide data for auto_id primary field: {schema.primary_field.name}")
+                    data = data.drop(schema.primary_field.name, axis=1)
+        else:
+            raise UpsertAutoIDTrueException(message=ExceptionsMessage.UpsertAutoIDTrue)
     infer_fields = parse_fields_from_data(data)
     tmp_fields = copy.deepcopy(schema.fields)
 
     for i, field in enumerate(schema.fields):
         if field.is_primary and field.auto_id:
             tmp_fields.pop(i)
 
@@ -325,15 +329,15 @@
     for x, y in zip(infer_fields, tmp_fields):
         if x.dtype != y.dtype:
             raise DataNotMatchException(message=f"The data type of field {y.name} doesn't match, expected: {y.dtype.name}, got {x.dtype.name}")
         if isinstance(data, pandas.DataFrame) and x.name != y.name:
             raise DataNotMatchException(message=f"The name of field don't match, expected: {y.name}, got {x.name}")
 
 
-def parse_fields_from_data(data: [List[List], pandas.DataFrame]) -> List[FieldSchema]:
+def parse_fields_from_data(data: Union[List[List], pandas.DataFrame]) -> List[FieldSchema]:
     if not isinstance(data, (pandas.DataFrame, list)):
         raise DataTypeNotSupportException(message="The type of data should be list or pandas.DataFrame")
 
     if isinstance(data, pandas.DataFrame):
         return parse_fields_from_dataframe(data)
 
     for d in data:
```

### Comparing `pymilvus-2.2.8/pymilvus/orm/search.py` & `pymilvus-2.3.0b1/pymilvus/orm/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     def __str__(self):
         """
         Return the information of hit record.
 
         :return str:
             The information of hit record.
         """
-        return str(self._hit)
+        return f"(distance: {self._hit.distance}, id: {self._hit.id})"
 
     __repr__ = __str__
 
 
 class Hits:
     def __init__(self, hits):
         """
```

### Comparing `pymilvus-2.2.8/pymilvus/orm/types.py` & `pymilvus-2.3.0b1/pymilvus/orm/types.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/pymilvus/orm/utility.py` & `pymilvus-2.3.0b1/pymilvus/orm/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,15 +472,14 @@
         >>> True
         >>> utility.drop_collection("new_collection")
         >>> utility.has_collection("new_collection")
         >>> False
     """
     return _get_connection(using).rename_collections(old_collection_name, new_collection_name, timeout=timeout)
 
-
 def list_collections(timeout=None, using="default") -> list:
     """
     Returns a list of all collection names.
 
     :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
                     is set to None, client waits until server response or error occur.
     :type  timeout: float
@@ -1033,85 +1032,7 @@
 
     :example:
         >>> from pymilvus import connections, utility
         >>> connections.connect()
         >>> rgs = utility.transfer_replica(source, target, collection_name, num_replica)
     """
     return _get_connection(using).transfer_replica(source_group, target_group, collection_name, num_replicas, timeout)
-
-
-def flush_all(using="default", timeout=None, **kwargs):
-    """ Flush all collections. All insertions, deletions, and upserts before `flush_all` will be synced.
-
-    Args:
-        timeout (float): an optional duration of time in seconds to allow for the RPCs.
-            If timeout is not set, the client keeps waiting until the server responds or an error occurs.
-            **kwargs (``dict``, optional):
-
-        * *_async*(``bool``)
-            Indicate if invoke asynchronously. Default `False`.
-
-    Examples:
-        >>> from pymilvus import connections, Collection, FieldSchema, CollectionSchema, DataType, utility
-        >>> connections.connect()
-        >>> fields = [
-        ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
-        ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=128)
-        ... ]
-        >>> schema = CollectionSchema(fields=fields)
-        >>> collection = Collection(name="test_collection_flush", schema=schema)
-        >>> collection.insert([[1, 2], [[1.0, 2.0], [3.0, 4.0]]])
-        >>> utility.flush_all(_async=False) # synchronized flush_all
-        >>> # or use `future` to flush_all asynchronously
-        >>> future = utility.flush_all(_async=True)
-        >>> future.done() # flush_all finished
-    """
-    return _get_connection(using).flush_all(timeout=timeout, **kwargs)
-
-
-def get_server_type(using="default"):
-    """ Get the server type. Now, it will return "zilliz" if the connection related to an instance on the zilliz cloud,
-        otherwise "milvus" will be returned.
-
-    :param using: Alias to the connection. Default connection is used if this is not specified.
-    :type  using: str
-
-    :return: The server type.
-    :rtype: str
-    """
-    return _get_connection(using).get_server_type()
-
-
-def list_indexes(collection_name, using="default", timeout=None, **kwargs):
-    """ List all indexes of collection. If `field_name` is not specified, return all the indexes of this collection,
-        otherwise this interface will return all indexes on this field of the collection.
-
-    :param collection_name: The name of collection.
-    :type  collection_name: str
-
-    :param using: Alias to the connection. Default connection is used if this is not specified.
-    :type  using: str
-
-    :param timeout: An optional duration of time in seconds to allow for the RPC. When timeout
-                    is set to None, client waits until server response or error occur
-    :type  timeout: float/int
-
-    :param kwargs:
-            * *field_name* (``str``)
-                The name of field. If no field name is specified, all indexes of this collection will be returned.
-    :type  kwargs: dict
-
-    :return: The name list of all indexes.
-    :rtype: str list
-    """
-    indexes = _get_connection(using).list_indexes(collection_name, timeout, **kwargs)
-    field_name = kwargs.get("field_name", None)
-    index_name_list = []
-    for index in indexes:
-        if index is not None:
-            if field_name is None:
-                # list all indexes anyway.
-                index_name_list.append(index.index_name)
-            if field_name is not None and index.field_name == field_name:
-                # list all indexes of this field.
-                index_name_list.append(index.index_name)
-    return index_name_list
```

### Comparing `pymilvus-2.2.8/pymilvus.egg-info/PKG-INFO` & `pymilvus-2.3.0b1/pymilvus.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: pymilvus
-Version: 2.2.8
+Version: 2.3.0b1
 Summary: Python Sdk for Milvus
 Home-page: https://github.com/milvus-io/pymilvus
 Author: Milvus Team
 Author-email: milvus-team@zilliz.com
 License: Apache-2.0
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Milvus Python SDK
 
 [![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
```

### Comparing `pymilvus-2.2.8/pymilvus.egg-info/SOURCES.txt` & `pymilvus-2.3.0b1/pymilvus.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-.env.example
 .gitignore
 .gitmodules
 CONTRIBUTING.md
 CONTRIBUTING_CN.md
 Dockerfile
 LICENSE
 Makefile
 OWNERS
 README.md
 check_proto_product.sh
 pylint.conf
 pyproject.toml
 requirements.txt
 setup.py
-test_requirements.txt
 .github/mergify.yml
 .github/ISSUE_TEMPLATE/bug_report.yaml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/feature_request.yaml
 .github/ISSUE_TEMPLATE/general-question.yaml
 .github/workflows/check_milvus_proto.yml
 .github/workflows/code_checker.yml
@@ -87,37 +85,36 @@
 pymilvus.egg-info/requires.txt
 pymilvus.egg-info/top_level.txt
 pymilvus/client/__init__.py
 pymilvus/client/abstract.py
 pymilvus/client/asynch.py
 pymilvus/client/blob.py
 pymilvus/client/check.py
+pymilvus/client/configs.py
 pymilvus/client/constants.py
 pymilvus/client/entity_helper.py
 pymilvus/client/grpc_handler.py
 pymilvus/client/interceptor.py
 pymilvus/client/prepare.py
 pymilvus/client/singleton_utils.py
 pymilvus/client/stub.py
 pymilvus/client/ts_utils.py
 pymilvus/client/types.py
 pymilvus/client/utils.py
 pymilvus/grpc_gen/__init__.py
 pymilvus/grpc_gen/common_pb2.py
-pymilvus/grpc_gen/common_pb2.pyi
 pymilvus/grpc_gen/milvus_pb2.py
-pymilvus/grpc_gen/milvus_pb2.pyi
 pymilvus/grpc_gen/milvus_pb2_grpc.py
 pymilvus/grpc_gen/python_gen.sh
 pymilvus/grpc_gen/schema_pb2.py
-pymilvus/grpc_gen/schema_pb2.pyi
 pymilvus/orm/__init__.py
 pymilvus/orm/collection.py
 pymilvus/orm/connections.py
 pymilvus/orm/constants.py
+pymilvus/orm/default_config.py
 pymilvus/orm/future.py
 pymilvus/orm/index.py
 pymilvus/orm/mutation.py
 pymilvus/orm/partition.py
 pymilvus/orm/prepare.py
 pymilvus/orm/role.py
 pymilvus/orm/schema.py
@@ -136,9 +133,8 @@
 tests/test_grpc_handler.py
 tests/test_index.py
 tests/test_partition.py
 tests/test_prepare.py
 tests/test_schema.py
 tests/test_ts_utils.py
 tests/test_types.py
-tests/test_utils.py
 tests/utils.py
```

### Comparing `pymilvus-2.2.8/setup.py` & `pymilvus-2.3.0b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,23 +15,22 @@
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/milvus-io/pymilvus',
     license="Apache-2.0",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
-        "grpcio>=1.49.1,<=1.53.0",
-        "protobuf>=3.20.0",
-        "environs<=9.5.0",
-        "ujson>=2.0.0",
-        "pandas>=1.2.4",
+        "grpcio>=1.47.0,<=1.48.0",
+        "grpcio-tools>=1.47.0, <=1.48.0",
+        "ujson>=2.0.0,<=5.4.0",
+        "mmh3>=2.0,<=3.0.0",
+        "pandas==1.1.5; python_version<'3.7'",
+        "pandas>=1.2.4; python_version>'3.6'",
     ],
     classifiers=[
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
     ],
 
-    python_requires='>=3.7'
+    python_requires='>=3.6'
 )
```

### Comparing `pymilvus-2.2.8/tests/conftest.py` & `pymilvus-2.3.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/tests/mock_milvus.py` & `pymilvus-2.3.0b1/tests/mock_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/tests/mock_result.py` & `pymilvus-2.3.0b1/tests/mock_result.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/tests/test_check.py` & `pymilvus-2.3.0b1/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/tests/test_collection.py` & `pymilvus-2.3.0b1/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/tests/test_connections.py` & `pymilvus-2.3.0b1/tests/test_connections.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 import pytest
 import pymilvus
 from unittest import mock
 
 from pymilvus import connections
-from pymilvus import DefaultConfig, MilvusException
+from pymilvus import DefaultConfig, MilvusException, ENV_CONNECTION_CONF
 from pymilvus.exceptions import ErrorCode
 
 LOGGER = logging.getLogger(__name__)
 
 mock_prefix = "pymilvus.client.grpc_handler.GrpcHandler"
 
 
@@ -21,15 +21,15 @@
         - raise ConnectionConfigException if inconsistent configs are given
 
         Connect to an existing and not connected alias will:
         - connect with the existing alias config if no configs are given
         - connect with the providing configs if valid, and replace the old ones.
 
         Connect to a new alias will:
-        - connect with the providing configs if valid, store the new alias with these configs
+        - connect with the provieding configs if valid, store the new alias with these configs
 
     """
     @pytest.fixture(scope="function", params=[
         {},
         {"random": "not useful"},
     ])
     def no_host_port(self, request):
@@ -68,46 +68,30 @@
 
         addr = connections.get_connection_addr(alias)
         assert addr == default_addr
 
         with mock.patch(f"{mock_prefix}.close", return_value=None):
             connections.disconnect(alias)
 
-    @pytest.fixture(scope="function", params=[
-        ("", {"address": "localhost:19530", "user": ""}),
-        ("localhost", {"address": "localhost:19530", "user": ""}),
-        ("localhost:19530", {"address": "localhost:19530", "user": ""}),
-        ("abc@localhost", {"address": "localhost:19530", "user": "abc"}),
-        ("milvus_host", {"address": "milvus_host:19530", "user": ""}),
-        ("milvus_host:12012", {"address": "milvus_host:12012", "user": ""}),
-        ("abc@milvus_host:12012", {"address": "milvus_host:12012", "user": "abc"}),
-        ("abc@milvus_host", {"address": "milvus_host:19530", "user": "abc"}),
-    ])
-    def test_connect_with_default_config_from_environment(self, env_result):
-        os.environ[DefaultConfig.MILVUS_URI] = env_result[0]
-        assert env_result[1] == connections._read_default_config_from_os_env()
-
-        with mock.patch(f"{mock_prefix}.__init__", return_value=None):
-            with mock.patch(f"{mock_prefix}._wait_for_channel_ready", return_value=None):
-                # use env
-                connections.connect()
+    def test_connect_with_default_config_from_environment(self):
+        test_list = [
+            ["", {"address": "localhost:19530", "user": ""}],
+            ["localhost", {"address": "localhost:19530", "user": ""}],
+            ["localhost:19530", {"address": "localhost:19530", "user": ""}],
+            ["abc@localhost", {"address": "localhost:19530", "user": "abc"}],
+            ["milvus_host", {"address": "milvus_host:19530", "user": ""}],
+            ["milvus_host:12012", {"address": "milvus_host:12012", "user": ""}],
+            ["abc@milvus_host:12012", {"address": "milvus_host:12012", "user": "abc"}],
+            ["abc@milvus_host", {"address": "milvus_host:19530", "user": "abc"}],
+        ]
 
-        assert env_result[1] == connections.get_connection_addr(DefaultConfig.MILVUS_CONN_ALIAS)
+        for env_str, assert_config in test_list:
+            os.environ[ENV_CONNECTION_CONF] = env_str
 
-        with mock.patch(f"{mock_prefix}.__init__", return_value=None):
-            with mock.patch(f"{mock_prefix}._wait_for_channel_ready", return_value=None):
-                # use param
-                connections.connect(DefaultConfig.MILVUS_CONN_ALIAS, host="test_host", port="19999")
-
-        curr_addr = connections.get_connection_addr(DefaultConfig.MILVUS_CONN_ALIAS)
-        assert env_result[1] != curr_addr
-        assert {"address":"test_host:19999", "user": ""} == curr_addr
-
-        with mock.patch(f"{mock_prefix}.close", return_value=None):
-            connections.remove_connection(DefaultConfig.MILVUS_CONN_ALIAS)
+            assert assert_config == connections._read_default_config_from_os_env()
 
     def test_connect_new_alias_with_configs(self):
         alias = "exist"
         addr = {"address": "localhost:19530"}
 
         assert connections.has_connection(alias) is False
         a = connections.get_connection_addr(alias)
@@ -308,21 +292,22 @@
 
         addr = connections.get_connection_addr(alias)
         LOGGER.info(f"addr: {addr}")
 
         host, port = addr["address"].split(':')
         assert host in valid_uri['uri'] or host in DefaultConfig.DEFAULT_HOST
         assert port in valid_uri['uri'] or port in DefaultConfig.DEFAULT_PORT
-        print(addr)
 
         with mock.patch(f"{mock_prefix}.close", return_value=None):
             connections.remove_connection(alias)
 
     @pytest.mark.parametrize("invalid_uri", [
-        {"uri": "http://"},
+        {"uri": "http://:19530"},
+        {"uri": "localhost:19530"},
+        {"uri": ":80"},
         {"uri": None},
         {"uri": -1},
     ])
     def test_add_connection_uri_invalid(self, invalid_uri):
         alias = self.test_add_connection_uri_invalid.__name__
         config = {alias: invalid_uri}
```

### Comparing `pymilvus-2.2.8/tests/test_create_collection.py` & `pymilvus-2.3.0b1/tests/test_create_collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/tests/test_decorators.py` & `pymilvus-2.3.0b1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/tests/test_grpc_handler.py` & `pymilvus-2.3.0b1/tests/test_grpc_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -106,44 +106,7 @@
             status=common_pb2.Status(error_code=common_pb2.Success),
             version=version,
         )
         rpc.terminate(expected_result, (), grpc.StatusCode.OK, '')
 
         got_result = get_version_future.result()
         assert got_result == version
-
-    @pytest.mark.parametrize("_async", [True])
-    def test_flush_all(self, channel, client_thread, _async):
-        handler = GrpcHandler(channel=channel)
-
-        flush_all_future = client_thread.submit(
-            handler.flush_all, _async=_async, timeout=10)
-
-        (invocation_metadata, request, rpc) = (
-            channel.take_unary_unary(descriptor.methods_by_name['FlushAll']))
-        rpc.send_initial_metadata(())
-
-        expected_result = milvus_pb2.FlushAllResponse(
-            status=common_pb2.Status(error_code=common_pb2.Success),
-            flush_all_ts=100,
-        )
-
-        rpc.terminate(expected_result, (), grpc.StatusCode.OK, '')
-        assert flush_all_future is not None
-
-    def test_get_flush_all_state(self, channel, client_thread):
-        handler = GrpcHandler(channel=channel)
-
-        flushed = client_thread.submit(
-            handler.get_flush_all_state, flush_all_ts=100)
-
-        (invocation_metadata, request, rpc) = (
-            channel.take_unary_unary(descriptor.methods_by_name['GetFlushAllState']))
-        rpc.send_initial_metadata(())
-
-        expected_result = milvus_pb2.GetFlushStateResponse(
-            status=common_pb2.Status(error_code=common_pb2.Success),
-            flushed=True,
-        )
-
-        rpc.terminate(expected_result, (), grpc.StatusCode.OK, '')
-        assert flushed.result() is True
```

### Comparing `pymilvus-2.2.8/tests/test_index.py` & `pymilvus-2.3.0b1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/tests/test_partition.py` & `pymilvus-2.3.0b1/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/tests/test_prepare.py` & `pymilvus-2.3.0b1/tests/test_prepare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from pymilvus.client.prepare import Prepare
 from pymilvus import DataType, MilvusException, CollectionSchema, FieldSchema
-from pymilvus import DefaultConfig
+from pymilvus.client.configs import DefaultConfigs
 
 
 class TestPrepare:
     def test_search_requests_with_expr_offset(self):
         fields = [
             FieldSchema("pk", DataType.INT64, is_primary=True),
             FieldSchema("v", DataType.FLOAT_VECTOR, dim=2),
@@ -80,15 +80,15 @@
             Prepare.get_schema("test_name", invalid_fields)
 
     @pytest.mark.parametrize("valid_fields", [
         {"fields": [
             {"name": "test_varchar", "type": DataType.VARCHAR, "is_primary": True, "params": {"dim": "invalid"}},
         ]},
         {"fields": [
-            {"name": "test_floatvector", "type": DataType.FLOAT_VECTOR, "params": {"dim": 128, DefaultConfig.MaxVarCharLengthKey: DefaultConfig.MaxVarCharLength + 1}},
+            {"name": "test_floatvector", "type": DataType.FLOAT_VECTOR, "params": {"dim": 128, DefaultConfigs.MaxVarCharLengthKey: DefaultConfigs.MaxVarCharLength + 1}},
         ]}
     ])
     def test_valid_type_params_get_collection_schema(self, valid_fields):
         schema = Prepare.get_schema("test_name", valid_fields)
         assert len(schema.fields) == 1
         assert schema.fields[0].name == valid_fields["fields"][0]["name"]
```

### Comparing `pymilvus-2.2.8/tests/test_schema.py` & `pymilvus-2.3.0b1/tests/test_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy
 import pytest
 
-from pymilvus import CollectionSchema, FieldSchema, DataType, MilvusException
+from pymilvus import CollectionSchema, FieldSchema, DataType
 from utils import *
-from pymilvus.orm import schema as s
 
 
 class TestCollectionSchema:
     @pytest.fixture(scope="function")
     def raw_dict(self):
         _dict = {}
         _dict["description"] = "TestCollectionSchema_description"
@@ -140,27 +139,7 @@
 
     #  def test_parse_fields_from_dataframe(self, dataframe1):
     #      fields = parse_fields_from_dataframe(dataframe1)
     #      assert len(fields) == len(dataframe1.columns)
     #      for f in fields:
     #          if f.dtype == DataType.FLOAT_VECTOR:
     #              assert f.dim == len(dataframe1['float_vec'].values[0])
-
-class TestCheckInsertDataSchema:
-    def test_check_insert_data_schema_issue1324(self):
-        schema = CollectionSchema([
-            FieldSchema(name="id", dtype=DataType.INT64, descrition="int64", is_primary=True, auto_id=True),
-            FieldSchema(name="embedding", dtype=DataType.FLOAT_VECTOR, descrition="float vector", dim=2),
-            FieldSchema(name="work_id2", dtype=5, descrition="work id"),
-            FieldSchema(name='path', dtype=DataType.VARCHAR, description='path to image', max_length=200),
-            FieldSchema(name="uid", dtype=DataType.INT64, descrition="user id"),
-        ])
-
-        data = [
-            [[0.003984056, 0.05035976]],
-            ['15755403'],
-            ['https://xxx.com/app/works/105149/2023-01-11/w_63be653c4643b/963be653c8aa8c.jpg'],
-            ['105149'],
-        ]
-
-        with pytest.raises(MilvusException):
-            s.check_insert_data_schema(schema, data)
```

### Comparing `pymilvus-2.2.8/tests/test_ts_utils.py` & `pymilvus-2.3.0b1/tests/test_ts_utils.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.2.8/tests/test_types.py` & `pymilvus-2.3.0b1/tests/test_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under the License.
 
 from pymilvus import DataType, DEFAULT_RESOURCE_GROUP
 from pymilvus.exceptions import InvalidConsistencyLevel
 from pymilvus.client.types import (
-    get_consistency_level, Shard, Group, Replica, ConsistencyLevel
+    get_consistency_level, ConsistencyLevel,
+    Shard, Group, Replica
 )
 
-from pymilvus.grpc_gen import common_pb2
-
 import pytest
 import pandas as pd
 import numpy as np
 
 
 @pytest.mark.xfail
 class TestTypes:
@@ -121,28 +120,21 @@
             get_consistency_level(invalid)
 
 
 class TestReplica:
     def test_shard(self):
         s = Shard("channel-1", (1, 2, 3), 1)
         assert s.channel_name == "channel-1"
-        assert s.shard_nodes == {1, 2, 3}
+        assert s.shard_nodes == (1, 2, 3)
         assert s.shard_leader == 1
         print(s)
 
         g = Group(2, [s], [1, 2, 3], DEFAULT_RESOURCE_GROUP, {})
         assert g.id == 2
         assert g.shards == [s]
         assert g.group_nodes == (1, 2, 3)
 
         print(g)
 
         replica = Replica([g, g])
         assert replica.groups == [g, g]
         print(replica)
-
-    def test_shard_dup_nodeIDs(self):
-        s = Shard("channel-1", (1, 1, 1), 1)
-        assert s.channel_name == "channel-1"
-        assert s.shard_nodes == {1,}
-        assert s.shard_leader == 1
-        print(s)
```

### Comparing `pymilvus-2.2.8/tests/utils.py` & `pymilvus-2.3.0b1/tests/utils.py`

 * *Files identical despite different names*

