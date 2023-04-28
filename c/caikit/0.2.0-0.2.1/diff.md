# Comparing `tmp/caikit-0.2.0.tar.gz` & `tmp/caikit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.2.0.tar", last modified: Thu Apr 27 17:16:34 2023, max compression
+gzip compressed data, was "caikit-0.2.1.tar", last modified: Fri Apr 28 16:00:43 2023, max compression
```

## Comparing `caikit-0.2.0.tar` & `caikit-0.2.1.tar`

### file list

```diff
@@ -1,293 +1,293 @@
--rw-r--r--   0        0        0       60 2023-04-27 17:16:26.218927 caikit-0.2.0/.coveragerc
--rw-r--r--   0        0        0      676 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1272 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1141 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-04-27 17:16:26.218927 caikit-0.2.0/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      212 2023-04-27 17:16:26.218927 caikit-0.2.0/.gitignore
--rw-r--r--   0        0        0      310 2023-04-27 17:16:26.218927 caikit-0.2.0/.isort.cfg
--rw-r--r--   0        0        0      370 2023-04-27 17:16:26.218927 caikit-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-04-27 17:16:26.218927 caikit-0.2.0/.prettierignore
--rw-r--r--   0        0        0       12 2023-04-27 17:16:26.218927 caikit-0.2.0/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-04-27 17:16:26.218927 caikit-0.2.0/.pylintrc
--rw-r--r--   0        0        0       78 2023-04-27 17:16:26.218927 caikit-0.2.0/.whitesource
--rw-r--r--   0        0        0     3358 2023-04-27 17:16:26.218927 caikit-0.2.0/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      336 2023-04-27 17:16:26.218927 caikit-0.2.0/CODEOWNERS
--rw-r--r--   0        0        0     7094 2023-04-27 17:16:26.218927 caikit-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-04-27 17:16:26.218927 caikit-0.2.0/LICENSE
--rw-r--r--   0        0        0     3757 2023-04-27 17:16:26.218927 caikit-0.2.0/README.md
--rw-r--r--   0        0        0    44878 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit-overview.png
--rw-r--r--   0        0        0      419 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/config/__init__.py
--rw-r--r--   0        0        0     5392 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/config/config.py
--rw-r--r--   0        0        0     6140 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/config/config.yml
--rw-r--r--   0        0        0     1770 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0      974 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/blocks/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/blocks/base.py
--rw-r--r--   0        0        0      962 2023-04-27 17:16:26.218927 caikit-0.2.0/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    29207 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     3962 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    13676 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     5340 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1471 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40187 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    20457 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/model_manager.py
--rw-r--r--   0        0        0    52621 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module.py
--rw-r--r--   0        0        0     6735 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_backend_config.py
--rw-r--r--   0        0        0      684 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     3399 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     1786 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     1493 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     5500 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_config.py
--rw-r--r--   0        0        0     6247 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/module_meta.py
--rw-r--r--   0        0        0      709 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/resources/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/resources/base.py
--rw-r--r--   0        0        0     1001 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    18059 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1648 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32204 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1022 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/workflows/__init__.py
--rw-r--r--   0        0        0     9298 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/core/workflows/base.py
--rw-r--r--   0        0        0      530 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1377 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     2070 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1716 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    13923 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4659 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0     2370 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/metrics/throughput.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     6047 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12101 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4311 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1587 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-04-27 17:16:26.222928 caikit-0.2.0/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    20071 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     3083 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5716 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    12221 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     7155 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0    10693 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/serializers.py
--rw-r--r--   0        0        0      666 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10301 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4911 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     7655 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0    11938 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    14711 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5496 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1579 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6665 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    17900 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-04-27 17:16:26.226928 caikit-0.2.0/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0     3693 2023-04-27 17:16:26.226928 caikit-0.2.0/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-04-27 17:16:26.226928 caikit-0.2.0/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-04-27 17:16:26.226928 caikit-0.2.0/docs/architecture_club/README.md
--rw-r--r--   0        0        0      837 2023-04-27 17:16:26.226928 caikit-0.2.0/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     1154 2023-04-27 17:16:29.570632 caikit-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0      720 2023-04-27 17:16:26.226928 caikit-0.2.0/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-04-27 17:16:26.226928 caikit-0.2.0/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3572 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/base.py
--rw-r--r--   0        0        0        0 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/config/__init__.py
--rw-r--r--   0        0        0     4345 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/config/test_configs.py
--rw-r--r--   0        0        0     8447 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/blocks/__init__.py
--rw-r--r--   0        0        0    11631 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/blocks/test_base.py
--rw-r--r--   0        0        0        0 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     4559 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26013 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    13070 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    13533 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     1104 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     2909 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/helpers.py
--rw-r--r--   0        0        0     2320 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0      521 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/test_imports.py
--rw-r--r--   0        0        0    19262 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/test_model_manager.py
--rw-r--r--   0        0        0    17485 2023-04-27 17:16:26.226928 caikit-0.2.0/tests/core/test_module.py
--rw-r--r--   0        0        0     5581 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/test_module_backend_config.py
--rw-r--r--   0        0        0     8529 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/test_module_metadata.py
--rw-r--r--   0        0        0     1038 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     7967 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    15068 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4972 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/workflows/__init__.py
--rw-r--r--   0        0        0    14580 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/core/workflows/test_base.py
--rw-r--r--   0        0        0     5655 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      498 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      106 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0     1016 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block.zip
--rw-r--r--   0        0        0      671 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block/data.pkl
--rw-r--r--   0        0        0      189 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block_backend/config.yml
--rw-r--r--   0        0        0      177 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block_foo/config.yml
--rw-r--r--   0        0        0      506 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block_no_nesting.zip
--rw-r--r--   0        0        0      566 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block_singleton/data.json
--rw-r--r--   0        0        0       14 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_block_singleton/data.pkl
--rw-r--r--   0        0        0      222 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0      717 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_resource.zip
--rw-r--r--   0        0        0      230 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     1991 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_workflow.zip
--rw-r--r--   0        0        0      497 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_workflow/config.yml
--rw-r--r--   0        0        0      541 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_workflow/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_workflow/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/dummy_workflow/dummy_block/data.pkl
--rw-r--r--   0        0        0     3033 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      355 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      359 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      359 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_block/config.yml
--rw-r--r--   0        0        0      337 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      114 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/__init__.py
--rw-r--r--   0        0        0       88 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/other_task/__init__.py
--rw-r--r--   0        0        0     1847 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
--rw-r--r--   0        0        0      199 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
--rw-r--r--   0        0        0      616 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
--rw-r--r--   0        0        0     2283 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1276 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2370 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      410 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      141 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0      859 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0        0 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/resources/__init__.py
--rw-r--r--   0        0        0       58 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/resources/sample_type/__init__.py
--rw-r--r--   0        0        0       74 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/workflows/__init__.py
--rw-r--r--   0        0        0       58 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
--rw-r--r--   0        0        0     1687 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
--rw-r--r--   0        0        0        0 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3843 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0     6402 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/metrics/test_throughput.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14115 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    11607 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    18018 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5373 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     1654 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/service_generation/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     7253 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3280 2023-04-27 17:16:26.230928 caikit-0.2.0/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18336 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     4065 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/service_generation/test_primitives.py
--rw-r--r--   0        0        0     1372 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     7923 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    14666 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3640 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7372 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4180 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    29994 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0    10935 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26086 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2807 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-04-27 17:16:26.234929 caikit-0.2.0/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     1133 2023-04-27 17:16:26.234929 caikit-0.2.0/tox.ini
--rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 caikit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-04-28 16:00:36.056088 caikit-0.2.1/.coveragerc
+-rw-r--r--   0        0        0      676 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1272 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1141 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-04-28 16:00:36.056088 caikit-0.2.1/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      212 2023-04-28 16:00:36.056088 caikit-0.2.1/.gitignore
+-rw-r--r--   0        0        0      310 2023-04-28 16:00:36.056088 caikit-0.2.1/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-04-28 16:00:36.056088 caikit-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-04-28 16:00:36.056088 caikit-0.2.1/.prettierignore
+-rw-r--r--   0        0        0       12 2023-04-28 16:00:36.056088 caikit-0.2.1/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-04-28 16:00:36.056088 caikit-0.2.1/.pylintrc
+-rw-r--r--   0        0        0       78 2023-04-28 16:00:36.056088 caikit-0.2.1/.whitesource
+-rw-r--r--   0        0        0     3358 2023-04-28 16:00:36.056088 caikit-0.2.1/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      336 2023-04-28 16:00:36.056088 caikit-0.2.1/CODEOWNERS
+-rw-r--r--   0        0        0     7094 2023-04-28 16:00:36.056088 caikit-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-04-28 16:00:36.056088 caikit-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3757 2023-04-28 16:00:36.056088 caikit-0.2.1/README.md
+-rw-r--r--   0        0        0    44878 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit-overview.png
+-rw-r--r--   0        0        0      419 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/config/__init__.py
+-rw-r--r--   0        0        0     5392 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/config/config.py
+-rw-r--r--   0        0        0     6140 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/config/config.yml
+-rw-r--r--   0        0        0     1770 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-04-28 16:00:36.056088 caikit-0.2.1/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0      974 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/blocks/__init__.py
+-rw-r--r--   0        0        0     1552 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/blocks/base.py
+-rw-r--r--   0        0        0      962 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    29207 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     3962 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    13676 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     5340 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1471 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40187 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    20457 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/model_manager.py
+-rw-r--r--   0        0        0    52621 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module.py
+-rw-r--r--   0        0        0     6735 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_backend_config.py
+-rw-r--r--   0        0        0      684 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     3399 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     1786 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     1493 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     5500 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_config.py
+-rw-r--r--   0        0        0     6247 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/module_meta.py
+-rw-r--r--   0        0        0      709 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/resources/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/resources/base.py
+-rw-r--r--   0        0        0     1001 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    18059 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1648 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32204 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1022 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/workflows/__init__.py
+-rw-r--r--   0        0        0     9298 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/core/workflows/base.py
+-rw-r--r--   0        0        0      530 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1377 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1716 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    13996 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0     2370 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/metrics/throughput.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     6047 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12101 2023-04-28 16:00:36.060088 caikit-0.2.1/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1587 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    20071 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     3083 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5791 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    12221 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     7155 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0    10693 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/serializers.py
+-rw-r--r--   0        0        0      666 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10744 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4911 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8181 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     2571 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0    11938 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    15316 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5496 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1579 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6665 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    17900 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-04-28 16:00:36.064088 caikit-0.2.1/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0     3693 2023-04-28 16:00:36.064088 caikit-0.2.1/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-04-28 16:00:36.064088 caikit-0.2.1/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-04-28 16:00:36.064088 caikit-0.2.1/docs/architecture_club/README.md
+-rw-r--r--   0        0        0      837 2023-04-28 16:00:36.064088 caikit-0.2.1/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     1155 2023-04-28 16:00:39.252073 caikit-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0      720 2023-04-28 16:00:36.064088 caikit-0.2.1/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-04-28 16:00:36.064088 caikit-0.2.1/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     3572 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/base.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/config/__init__.py
+-rw-r--r--   0        0        0     4345 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/config/test_configs.py
+-rw-r--r--   0        0        0     8462 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/blocks/__init__.py
+-rw-r--r--   0        0        0    11631 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/blocks/test_base.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     4559 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26013 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    13070 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    13533 2023-04-28 16:00:36.064088 caikit-0.2.1/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     1104 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     2909 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/helpers.py
+-rw-r--r--   0        0        0     2320 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0      521 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/test_imports.py
+-rw-r--r--   0        0        0    19262 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0    17485 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/test_module.py
+-rw-r--r--   0        0        0     5581 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/test_module_backend_config.py
+-rw-r--r--   0        0        0     8529 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/test_module_metadata.py
+-rw-r--r--   0        0        0     1038 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     7967 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    15068 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4972 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/workflows/__init__.py
+-rw-r--r--   0        0        0    14580 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/core/workflows/test_base.py
+-rw-r--r--   0        0        0     5655 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      498 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      106 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0     1016 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block.zip
+-rw-r--r--   0        0        0      671 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block/data.pkl
+-rw-r--r--   0        0        0      189 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block_backend/config.yml
+-rw-r--r--   0        0        0      177 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block_no_nesting.zip
+-rw-r--r--   0        0        0      566 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_block_singleton/data.pkl
+-rw-r--r--   0        0        0      222 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0      717 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_resource.zip
+-rw-r--r--   0        0        0      230 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     1991 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_workflow.zip
+-rw-r--r--   0        0        0      497 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_workflow/config.yml
+-rw-r--r--   0        0        0      541 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_workflow/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_workflow/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/dummy_workflow/dummy_block/data.pkl
+-rw-r--r--   0        0        0     3033 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      355 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      359 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      359 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_block/config.yml
+-rw-r--r--   0        0        0      337 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/other_task/__init__.py
+-rw-r--r--   0        0        0     1847 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
+-rw-r--r--   0        0        0      199 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
+-rw-r--r--   0        0        0      616 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
+-rw-r--r--   0        0        0     2283 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1276 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2662 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      410 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      141 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0      859 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/resources/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/resources/sample_type/__init__.py
+-rw-r--r--   0        0        0       74 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/workflows/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
+-rw-r--r--   0        0        0     1687 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3843 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0     6402 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/metrics/test_throughput.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14115 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    11607 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    18018 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5373 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:00:36.068088 caikit-0.2.1/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     5398 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8595 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0     3768 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18336 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     4065 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/test_primitives.py
+-rw-r--r--   0        0        0     1372 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     7923 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    15695 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3640 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7372 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4180 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    30069 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0    10935 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26086 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2807 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-04-28 16:00:36.072088 caikit-0.2.1/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     1133 2023-04-28 16:00:36.072088 caikit-0.2.1/tox.ini
+-rw-r--r--   0        0        0     4867 1970-01-01 00:00:00.000000 caikit-0.2.1/PKG-INFO
```

### Comparing `caikit-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.2.1/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/.github/workflows/build-library.yml` & `caikit-0.2.1/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/.github/workflows/lint-code.yml` & `caikit-0.2.1/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/.github/workflows/publish-library.yml` & `caikit-0.2.1/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/.pylintrc` & `caikit-0.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/CODE-OF-CONDUCT.md` & `caikit-0.2.1/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/CONTRIBUTING.md` & `caikit-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/LICENSE` & `caikit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/README.md` & `caikit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit-overview.png` & `caikit-0.2.1/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/config/__init__.py` & `caikit-0.2.1/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/config/config.py` & `caikit-0.2.1/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/config/config.yml` & `caikit-0.2.1/caikit/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/__init__.py` & `caikit-0.2.1/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/augmentors/__init__.py` & `caikit-0.2.1/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/augmentors/base.py` & `caikit-0.2.1/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.2.1/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.2.1/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/augmentors/schemes/base.py` & `caikit-0.2.1/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.2.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.2.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/blocks/__init__.py` & `caikit-0.2.1/caikit/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/blocks/base.py` & `caikit-0.2.1/caikit/core/blocks/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/__init__.py` & `caikit-0.2.1/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/base.py` & `caikit-0.2.1/caikit/core/data_model/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         # Return the constructed class instance
         return instance
 
     @classmethod
     def _make_property_getter(mcs, field):
         """This helper creates an @property attribute getter for the given field
 
-        NOTE: This needs to live as a standalone funciton in order for the given
+        NOTE: This needs to live as a standalone function in order for the given
             field name to be properly bound to the closure for the attrs
         """
         private_name = f"_{field}"
 
         @property
         def _property_getter(self):
             # Check to see if the private name is defined and just return it if
```

### Comparing `caikit-0.2.0/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.2.1/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/data_backends/base.py` & `caikit-0.2.1/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.2.1/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/dataobject.py` & `caikit-0.2.1/caikit/core/data_model/dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/enums.py` & `caikit-0.2.1/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/producer.py` & `caikit-0.2.1/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.2.1/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/streams/__init__.py` & `caikit-0.2.1/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/streams/converter.py` & `caikit-0.2.1/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.2.1/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/streams/data_stream.py` & `caikit-0.2.1/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/streams/resolver.py` & `caikit-0.2.1/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/data_model/streams/validator.py` & `caikit-0.2.1/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/model_manager.py` & `caikit-0.2.1/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/module.py` & `caikit-0.2.1/caikit/core/module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/module_backend_config.py` & `caikit-0.2.1/caikit/core/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/module_backends/__init__.py` & `caikit-0.2.1/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/module_backends/backend_types.py` & `caikit-0.2.1/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/module_backends/base.py` & `caikit-0.2.1/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/module_backends/local_backend.py` & `caikit-0.2.1/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/module_config.py` & `caikit-0.2.1/caikit/core/module_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/module_meta.py` & `caikit-0.2.1/caikit/core/module_meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/resources/__init__.py` & `caikit-0.2.1/caikit/core/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/resources/base.py` & `caikit-0.2.1/caikit/core/resources/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/toolkit/__init__.py` & `caikit-0.2.1/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/toolkit/compatibility.py` & `caikit-0.2.1/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/toolkit/errors/__init__.py` & `caikit-0.2.1/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.2.1/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.2.1/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/toolkit/fileio.py` & `caikit-0.2.1/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/toolkit/isa.py` & `caikit-0.2.1/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/toolkit/logging.py` & `caikit-0.2.1/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.2.1/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/toolkit/serializers.py` & `caikit-0.2.1/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/toolkit/wip_decorator.py` & `caikit-0.2.1/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/workflows/__init__.py` & `caikit-0.2.1/caikit/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/core/workflows/base.py` & `caikit-0.2.1/caikit/core/workflows/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/interfaces/__init__.py` & `caikit-0.2.1/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/interfaces/common/__init__.py` & `caikit-0.2.1/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.2.1/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/interfaces/common/data_model/producer.py` & `caikit-0.2.1/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/interfaces/runtime/__init__.py` & `caikit-0.2.1/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.2.1/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.2.1/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/__init__.py` & `caikit-0.2.1/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/dump_services.py` & `caikit-0.2.1/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/grpc_server.py` & `caikit-0.2.1/caikit/runtime/grpc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,22 +56,22 @@
 
 
 class RuntimeGRPCServer:
     """An implementation of a gRPC server that serves caikit runtimes"""
 
     def __init__(
         self,
-        infer_srv: ServicePackage,
-        train_srv: Optional[ServicePackage],
+        inference_service: ServicePackage,
+        training_service: Optional[ServicePackage],
         tls_config_override: aconfig.Config = None,
-        hndle_terms: bool = False,
+        handle_terminations: bool = False,
     ):
         self.config = get_config()
-        self.inference_service = infer_srv
-        self.training_service = train_srv
+        self.inference_service = inference_service
+        self.training_service = training_service
 
         self.port = (
             self._find_port(self.config.runtime.port)
             if self.config.runtime.find_available_port
             else self.config.runtime.port
         )
         if self.port != self.config.runtime.port:
@@ -137,19 +137,19 @@
         # Add model runtime servicer to the gRPC server
         model_runtime_pb2_grpc.add_ModelRuntimeServicer_to_server(
             ModelRuntimeServicerImpl(), self.server
         )
 
         # Add gRPC default health servicer.
         # We use the non-blocking implementation to avoid thread starvation.
-        health_srvcer = health.HealthServicer(
+        health_servicer = health.HealthServicer(
             experimental_non_blocking=True,
             experimental_thread_pool=futures.ThreadPoolExecutor(max_workers=1),
         )
-        health_pb2_grpc.add_HealthServicer_to_server(health_srvcer, self.server)
+        health_pb2_grpc.add_HealthServicer_to_server(health_servicer, self.server)
 
         # Listen on a unix socket as well for model mesh.
         try:
             self.server.add_insecure_port(
                 f"unix://{self.config.runtime.unix_socket_path}"
             )
             log.info(
@@ -197,15 +197,15 @@
             log.info("<RUN10001807I>", "Running in insecure mode")
             self.server.add_insecure_port(f"[::]:{self.port}")
 
         # NOTE: signal function can only be called from main thread of the main interpreter.
         # If this function is called from a thread (like in tests) then signal handler cannot
         # be used. Thus, we will only have real termination_handler when this is called from
         # the __main__.
-        if hndle_terms:
+        if handle_terminations:
             signal.signal(signal.SIGINT, self.interrupt)
             signal.signal(signal.SIGTERM, self.interrupt)
 
     def start(self, blocking: bool = True):
         """Boot the gRPC server. Can be non-blocking, or block until shutdown
 
         Args:
@@ -355,16 +355,16 @@
             service_source,
         )
     except CaikitRuntimeException as e:
         log.error("Cannot stand up training service, disabling training: %s", e)
         training_service = None
 
     server = RuntimeGRPCServer(
-        infer_srv=inference_service,
-        train_srv=training_service,
-        hndle_terms=handle_terminations,
+        inference_service=inference_service,
+        training_service=training_service,
+        handle_terminations=handle_terminations,
     )
     server.start()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `caikit-0.2.0/caikit/runtime/interceptors/__init__.py` & `caikit-0.2.1/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.2.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/metrics/__init__.py` & `caikit-0.2.1/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.2.1/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/metrics/throughput.py` & `caikit-0.2.1/caikit/runtime/metrics/throughput.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/model_management/__init__.py` & `caikit-0.2.1/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/model_management/batcher.py` & `caikit-0.2.1/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/model_management/loaded_model.py` & `caikit-0.2.1/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/model_management/model_loader.py` & `caikit-0.2.1/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/model_management/model_manager.py` & `caikit-0.2.1/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/model_management/model_sizer.py` & `caikit-0.2.1/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/model_management/training_manager.py` & `caikit-0.2.1/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/protobufs/__init__.py` & `caikit-0.2.1/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.2.1/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.2.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.2.1/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.2.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.2.1/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.2.1/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.2.1/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.2.1/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.2.1/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/service_factory.py` & `caikit-0.2.1/caikit/runtime/service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.2.1/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.2.1/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/service_generation/create_service.py` & `caikit-0.2.1/caikit/runtime/service_generation/create_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,19 +119,20 @@
     modules: List[Type[ModuleBase]],
     primitive_data_model_types: List[str],
 ) -> List[Type[ModuleBase]]:
     primitive_modules = []
     # If the module is not "primitive" we won't include it
     for ck_module in modules:
         signature = CaikitCoreModuleMethodSignature(ck_module, "run")
-        if not is_primitive_method(signature, primitive_data_model_types):
-            log.debug("Skipping non-primitive module %s", ck_module)
-            continue
+        if signature.parameters and signature.return_type:
+            if not is_primitive_method(signature, primitive_data_model_types):
+                log.debug("Skipping non-primitive module %s", ck_module)
+                continue
 
-        primitive_modules.append(ck_module)
+            primitive_modules.append(ck_module)
     return primitive_modules
 
 
 def _create_rpcs_for_modules(
     modules: List[Type[ModuleBase]],
     primitive_data_model_types: List[str],
     fname: str = INFERENCE_FUNCTION_NAME,
```

### Comparing `caikit-0.2.0/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.2.1/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/service_generation/primitives.py` & `caikit-0.2.1/caikit/runtime/service_generation/primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/service_generation/serializers.py` & `caikit-0.2.1/caikit/runtime/service_generation/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/docstrings.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 # Standard
 from typing import Callable, Dict, List, Optional, Tuple, Type, Union
 import builtins
 import sys
 
 # Third Party
 import docstring_parser
+import grpc
 
 # First Party
 import alog
 
 # Local
 from caikit.core.data_model.base import DataBase
+from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 import caikit.core
 
 log = alog.use_channel("DOCSTRINGS")
 
 
 def get_return_type(fn: Callable) -> Optional[Type]:
     """
@@ -38,18 +40,21 @@
     Args:
         fn: The function to get the return value of
             e.g. my_caikit_library.blocks.classification.Transformer.run
 
     Returns:
         The return type of `fn`, if it can be parsed from the docstring. Otherwise, None
     """
-    docstring = docstring_parser.parse(fn.__doc__)
-    if not docstring:
-        log.warning("Failed to parse the docstring")
-        return None
+    try:
+        docstring = docstring_parser.parse(fn.__doc__)
+    except Exception as exc:
+        raise CaikitRuntimeException(
+            grpc.StatusCode.INVALID_ARGUMENT,
+            f"ParseError when parsing docstring for function: {fn.__name__}",
+        ) from exc
 
     type_names, desc_names = _get_candidate_type_names_from_docstring(docstring.returns)
 
     return_type = _get_docstring_type(type_names)
     if return_type:
         return return_type
 
@@ -64,18 +69,21 @@
 
     Args:
         fn: The function to get the type of a parameter from
             e.g.  my_caikit_library.blocks.classification.Transformer.run
         arg_name: The name of the parameter that we should try to get the type of
             e.g. "raw_document"
     """
-    docstring = docstring_parser.parse(fn.__doc__)
-    if not docstring:
-        log.warning("Failed to parse the docstring for %s", fn.__name__)
-        return False
+    try:
+        docstring = docstring_parser.parse(fn.__doc__)
+    except Exception as exc:
+        raise CaikitRuntimeException(
+            grpc.StatusCode.INVALID_ARGUMENT,
+            f"ParseError when parsing docstring for function: {fn.__name__}",
+        ) from exc
 
     ds_param = [param for param in docstring.params if param.arg_name == arg_name]
     if ds_param:
         if len(ds_param) > 1:
             log.warning("Docstring has multiple args with the same name! %s", arg_name)
         ds_param = ds_param[0]
 
@@ -84,32 +92,36 @@
                 if description_line.lower().startswith(
                     "optional"
                 ) or description_line.lower().startswith("an optional"):
                     log.debug2("Optional parameter found: %s", ds_param)
                     return True
 
         return False
+    return False
 
 
 def get_arg_type(fn: Callable, arg_name: str) -> Optional[Type]:
     """
     Grabs the type of the `arg_name` param from `fn`s docstring, if possible
     Args:
         fn: The function to get the type of a parameter from
             e.g. my_caikit_library.blocks.classification.Transformer.run
         arg_name: The name of the parameter that we should try to get the type of
             e.g. "raw_document"
     Returns:
         The return type of `fn`, if it can be parsed from the docstring. Otherwise, None
     """
 
-    docstring = docstring_parser.parse(fn.__doc__)
-    if not docstring:
-        log.warning("Failed to parse the docstring for function %s", fn.__name__)
-        return None
+    try:
+        docstring = docstring_parser.parse(fn.__doc__)
+    except Exception as exc:
+        raise CaikitRuntimeException(
+            grpc.StatusCode.INVALID_ARGUMENT,
+            f"ParseError when parsing docstring for function: {fn.__name__}",
+        ) from exc
 
     ds_param = [param for param in docstring.params if param.arg_name == arg_name]
     if ds_param:
         if len(ds_param) > 1:
             log.warning("Docstring has multiple args with the same name! %s", arg_name)
         ds_param = ds_param[0]
         type_names, desc_names = _get_candidate_type_names_from_docstring(ds_param)
@@ -192,15 +204,15 @@
         # Try to spelunk down `sys.modules` for the type. This should work if it is fully qualified
         candidate_type = _extract_type_from_pymodule(sys.modules, type_name)
         if candidate_type is not None:
             valid_candidates.append(candidate_type)
             log.debug2(f"Found valid candidate type on sys.modules: {candidate_type}")
             continue
 
-        # If the type was not fully qualified (like a `RawDocument`), look in a couple well known
+        # If the type was not fully qualified (like a `ProducerId`), look in a couple well known
         # places - the caikit core data model itself
         candidate_type = _extract_type_from_pymodule(
             caikit.interfaces.common.data_model, type_name
         )
         if candidate_type is not None:
             valid_candidates.append(candidate_type)
             log.debug2(
```

### Comparing `caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.2.1/caikit/runtime/service_generation/signature_parsing/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # First Party
 import alog
 
 # Local
 from . import docstrings
 from caikit.core.data_model.base import DataBase
 from caikit.core.module import ModuleBase
+from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 
 log = alog.use_channel("SIG-PARSING")
 
 # Constants ##################################
 KNOWN_ARG_TYPES = {
     "producer_id": "ProducerId",
 }
@@ -55,15 +56,20 @@
                     fn_signature.return_annotation,
                 )
                 return module_class
         else:
             return fn_signature.return_annotation
 
     # Check the docstring
-    type_from_docstring = docstrings.get_return_type(fn)
+    type_from_docstring = None
+    try:
+        type_from_docstring = docstrings.get_return_type(fn)
+    except CaikitRuntimeException:
+        log.warning("Failed to parse the docstring for %s", fn)
+
     if type_from_docstring:
         return type_from_docstring
 
     # If we get here, it means no annotation or docstring for type was provided
     log.warning(
         "Could not deduct output type from function %s for module class %s.",
         fn_signature,
@@ -129,15 +135,19 @@
     dm_type_from_known_arg_types = _get_dm_type_from_name(KNOWN_ARG_TYPES.get(arg.name))
     if dm_type_from_known_arg_types:
         # Not checking if this is optional: These known types should never be optional (maybe...?)
         # This could totally be incorrect!
         return dm_type_from_known_arg_types
 
     # Check docstring for optional arg
-    optional_arg = docstrings.is_optional(module_method, arg.name)
+    optional_arg = False
+    try:
+        optional_arg = docstrings.is_optional(module_method, arg.name)
+    except CaikitRuntimeException:
+        log.warning("Failed to parse the docstring for %s", module_method)
 
     # Look for a type annotation
     if arg.annotation != inspect.Parameter.empty:
         log.debug("Found annotation for %s", arg.name)
         if optional_arg:
             return Optional[arg.annotation]
         return arg.annotation
@@ -146,16 +156,19 @@
 
     # Check for a default argument and return its type
     default_type = _get_default_type(arg)
     if default_type:
         return default_type
 
     # Parse docstring
-
-    type_from_docstring = docstrings.get_arg_type(module_method, arg.name)
+    type_from_docstring = None
+    try:
+        type_from_docstring = docstrings.get_arg_type(module_method, arg.name)
+    except CaikitRuntimeException:
+        log.warning("Failed to parse the docstring for %s", module_method)
     if type_from_docstring:
         if optional_arg:
             return Optional[type_from_docstring]
         return type_from_docstring
 
     # Look for a data model object whose name matches the argument name and fall
     # back to the KNOWN_ARG_TYPES dict
```

### Comparing `caikit-0.2.0/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.2.1/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/servicers/__init__.py` & `caikit-0.2.1/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.2.1/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.2.1/caikit/runtime/servicers/global_train_servicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 log = alog.use_channel("GT-SERVICR-I")
 
 
 # Protobuf non primitives
 # Ref: https://developers.google.com/protocol-buffers/docs/reference/cpp/google.protobuf.descriptor
 NON_PRIMITIVE_TYPES = [FieldDescriptor.TYPE_MESSAGE, FieldDescriptor.TYPE_ENUM]
 
+OOM_EXIT_CODE = 137
 
 # pylint: disable=too-many-instance-attributes
 class GlobalTrainServicer:
     """Something something about the train servicer"""
 
     def __init__(self, training_service: ServicePackage):
         self._training_service = training_service
@@ -348,32 +349,48 @@
                 StatusCode.INTERNAL,
                 f"Exception raised during training: {e}",
             ) from e
 
     @classmethod
     def _train_and_save_model_subproc(cls, *args, **kwargs):
         """This function runs _train_and_save_model in a subprocess"""
+
         proc = cls._ErrorCaptureProcess(
             target=cls._train_and_save_model,
             args=args,
             kwargs=kwargs,
         )
+
         proc.start()
         proc.join()
 
         # If an error occurred, reraise it here
         # TODO: Make sure the stack trace is preserved
         if proc.error is not None:
             if isinstance(proc.error, CaikitRuntimeException):
                 raise proc.error
             raise CaikitRuntimeException(
                 grpc.StatusCode.INTERNAL,
                 "Error caught in training subprocess",
             ) from proc.error
 
+        # If process exited with a non-zero exit code
+        if proc.exitcode and proc.exitcode != os.EX_OK:
+            if proc.exitcode == OOM_EXIT_CODE:
+                exception = CaikitRuntimeException(
+                    grpc.StatusCode.RESOURCE_EXHAUSTED,
+                    "Training process died with OOM error!",
+                )
+            else:
+                exception = CaikitRuntimeException(
+                    grpc.StatusCode.UNKNOWN,
+                    f"Training process died with exit code {proc.exitcode}",
+                )
+            raise exception
+
     class _ErrorCaptureProcess(multiprocessing.get_context("fork").Process):
         """This class wraps a Process and keeps track of any errors that occur
         during execution
 
         NOTE: We explicitly use "fork" here for two reasons:
             1. It's faster
             2. Due to the auto-generated classes with stream sources, "spawn"
```

### Comparing `caikit-0.2.0/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.2.1/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.2.1/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.2.1/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/types/__init__.py` & `caikit-0.2.1/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/types/aborted_exception.py` & `caikit-0.2.1/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.2.1/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.2.1/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/utils/__init__.py` & `caikit-0.2.1/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/utils/import_util.py` & `caikit-0.2.1/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/utils/servicer_util.py` & `caikit-0.2.1/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/work_management/__init__.py` & `caikit-0.2.1/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/work_management/abortable_action.py` & `caikit-0.2.1/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/work_management/call_aborter.py` & `caikit-0.2.1/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.2.1/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/docs/adrs/README.md` & `caikit-0.2.1/docs/adrs/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/docs/architecture_club/04-25-23.md` & `caikit-0.2.1/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/examples/start_runtime_with_sample_lib.py` & `caikit-0.2.1/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/pyproject.toml` & `caikit-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.2.0"
+version = "0.2.1"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
-    "alchemy-config>=1.1.1",
-    "alchemy-logging>=1.0.4",
+    "alchemy-config>=1.1.1,<2.0.0",
+    "alchemy-logging>=1.0.4,<2.0.0",
     "anytree>=2.7.0,<3.0",
-    "docstring-parser>=0.14.1",
+    "docstring-parser>=0.14.1,<0.15.0",
     "grpcio-health-checking>=1.35.0,<2.0",
     "grpcio>=1.35.0,<2.0",
     "ijson>=3.1.4,<3.3.0",
     "munch>=2.5.0,<3.0",
     "protobuf>=3.19.0,<5",
     "prometheus_client==0.12.0",
     "py-grpc-prometheus>=0.7.0,<0.8",
     "PyYAML>=6.0,<7.0",
     "requests>=2.26.0,<3.0",
     "semver>=2.13.0,<4.0",
     "six>=1.16.0,<2.0.0",
     "tqdm>=4.59.0,<5.0.0",
-    "wheel>=0.37.0",
     "jtd-to-proto>=0.12.1,<0.13.0",
     "import-tracker>=3.1.5,<4",
 ]
 
 [project.urls]
 Source = "https://github.com/caikit/caikit"
```

### Comparing `caikit-0.2.0/scripts/fmt.sh` & `caikit-0.2.1/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/__init__.py` & `caikit-0.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/base.py` & `caikit-0.2.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/config/test_configs.py` & `caikit-0.2.1/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/conftest.py` & `caikit-0.2.1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,16 @@
 
 
 @pytest.fixture(scope="session")
 def runtime_grpc_server(
     sample_inference_service, sample_train_service
 ) -> RuntimeGRPCServer:
     server = RuntimeGRPCServer(
-        infer_srv=sample_inference_service,
-        train_srv=sample_train_service,
+        inference_service=sample_inference_service,
+        training_service=sample_train_service,
     )
 
     grpc_thread = threading.Thread(
         target=server.start,
     )
     grpc_thread.setDaemon(False)
     grpc_thread.start()
```

### Comparing `caikit-0.2.0/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.2.1/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.2.1/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/blocks/__init__.py` & `caikit-0.2.1/tests/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/blocks/test_base.py` & `caikit-0.2.1/tests/core/blocks/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.2.1/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/data_model/streams/test_converter.py` & `caikit-0.2.1/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.2.1/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.2.1/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/data_model/streams/test_resolver.py` & `caikit-0.2.1/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/data_model/streams/test_validator.py` & `caikit-0.2.1/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/data_model/test_base.py` & `caikit-0.2.1/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/data_model/test_dataobject.py` & `caikit-0.2.1/tests/core/data_model/test_dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/data_model/test_producer.py` & `caikit-0.2.1/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/helpers.py` & `caikit-0.2.1/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/module_backends/test_backend_types.py` & `caikit-0.2.1/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/test_imports.py` & `caikit-0.2.1/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/test_model_manager.py` & `caikit-0.2.1/tests/core/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/test_module.py` & `caikit-0.2.1/tests/core/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/test_module_backend_config.py` & `caikit-0.2.1/tests/core/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/test_module_metadata.py` & `caikit-0.2.1/tests/core/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/test_no_write_permissions.py` & `caikit-0.2.1/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/toolkit/test_compatibility.py` & `caikit-0.2.1/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/toolkit/test_error_handler.py` & `caikit-0.2.1/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/toolkit/test_fileio.py` & `caikit-0.2.1/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.2.1/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/toolkit/test_serializers.py` & `caikit-0.2.1/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.2.1/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/workflows/__init__.py` & `caikit-0.2.1/tests/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/core/workflows/test_base.py` & `caikit-0.2.1/tests/core/workflows/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/data_model_helpers.py` & `caikit-0.2.1/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.2.1/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/dummy_block.zip` & `caikit-0.2.1/tests/fixtures/dummy_block.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/dummy_block/config.yml` & `caikit-0.2.1/tests/fixtures/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/dummy_block_singleton/config.yml` & `caikit-0.2.1/tests/fixtures/dummy_block_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/dummy_resource.zip` & `caikit-0.2.1/tests/fixtures/dummy_resource.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/dummy_workflow.zip` & `caikit-0.2.1/tests/fixtures/dummy_workflow.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/dummy_workflow/dummy_block/config.yml` & `caikit-0.2.1/tests/fixtures/dummy_workflow/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/fixtures.py` & `caikit-0.2.1/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/invalid.zip` & `caikit-0.2.1/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/linux.txt` & `caikit-0.2.1/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/primitive_party.proto` & `caikit-0.2.1/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.2.1/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.2.1/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py` & `caikit-0.2.1/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py` & `caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py` & `caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py` & `caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py` & `caikit-0.2.1/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 A sample block for sample things!
 """
+# Standard
+import os
+
 # Local
 from ...data_model.sample import SampleInputType, SampleOutputType, SampleTrainingType
 from caikit.core.data_model import DataStream
 from caikit.core.module import ModuleLoader, ModuleSaver
 import caikit.core
 
 
@@ -56,16 +59,24 @@
             module_saver.update_config(config_options)
 
     @classmethod
     def train(
         cls,
         training_data: DataStream[SampleTrainingType],
         batch_size: int = 64,
+        oom_exit: bool = False,
     ) -> "SampleBlock":
         """Sample training method that produces a trained model"""
+
+        if oom_exit:
+            # exit with OOM code. Note _exit method is used to exit the
+            # process with specified status without calling cleanup handlers
+            # to replicate OOM scenario
+            os._exit(137)
+
         if batch_size == cls.POISON_PILL_BATCH_SIZE:
             raise ValueError(
                 f"Batch size of {cls.POISON_PILL_BATCH_SIZE} is not allowed!"
             )
         # Barf if we were incorrectly passed data not in datastream format
         assert isinstance(training_data, DataStream)
         return cls(batch_size=batch_size)
```

### Comparing `caikit-0.2.0/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.2.1/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py` & `caikit-0.2.1/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/generated/__init__.py` & `caikit-0.2.1/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/metrics/__init__.py` & `caikit-0.2.1/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.2.1/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/metrics/test_throughput.py` & `caikit-0.2.1/tests/runtime/metrics/test_throughput.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/model_management/__init__.py` & `caikit-0.2.1/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/model_management/test_batcher.py` & `caikit-0.2.1/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/model_management/test_model_loader.py` & `caikit-0.2.1/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/model_management/test_model_manager.py` & `caikit-0.2.1/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.2.1/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/model_management/test_training_manager.py` & `caikit-0.2.1/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.2.1/tests/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/service_generation/signature_parsing/test_parsers.py` & `caikit-0.2.1/tests/runtime/service_generation/signature_parsing/test_parsers.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 # limitations under the License.
 """These are mostly some older tests that we wrote ad-hoc while throwing the inference proto-generation together
 
 Coverage is probably not the best
 """
 # Standard
 from typing import List, Optional
+from unittest.mock import patch
 import inspect
 
 # Third Party
+from docstring_parser import ParseError
 import pytest
 
 # Local
 from caikit.runtime.service_generation.signature_parsing import docstrings
 from caikit.runtime.service_generation.signature_parsing.parsers import (
     _get_dm_type_from_name,
     _snake_to_camel,
@@ -120,24 +122,52 @@
             module_class=sample_lib.blocks.sample_task.InnerBlock,
             fn_signature=empty_sign,
             fn=sample_lib.blocks.sample_task.InnerBlock.run,
         )
         == None
     )
 
+    # Test that if a ParseError was raised with docstring.parsers, we have no idea the type and return None
+    with patch("docstring_parser.parse", side_effect=ParseError("mocked error")):
+        assert (
+            get_output_type_name(
+                module_class=sample_lib.blocks.sample_task.InnerBlock,
+                fn_signature=empty_sign,
+                fn=sample_lib.blocks.sample_task.InnerBlock.run,
+            )
+            == None
+        )
+
 
 def test_get_argument_types_with_real_block():
     """Quick check that we get the right type for our sample block"""
     assert (
         get_argument_types(sample_lib.blocks.sample_task.SampleBlock.run)[
             "sample_input"
         ]
         == sample_lib.data_model.SampleInputType
     )
 
+    # Test that if a ParseError was raised with docstring.parsers, we could still parse from type annotation
+    with patch("docstring_parser.parse", side_effect=ParseError("mocked error")):
+        assert (
+            get_argument_types(sample_lib.blocks.sample_task.SampleBlock.run)[
+                "sample_input"
+            ]
+            == sample_lib.data_model.SampleInputType
+        )
+
+    # Test that if a ParseError was raised with docstring.parsers, but no type annotation provided, we cannot deduct type and return None
+    def run_fn(some_input: str, some_input_2):
+        pass
+
+    with patch("docstring_parser.parse", side_effect=ParseError("mocked error")):
+        assert get_argument_types(run_fn)["some_input"] == str
+        assert get_argument_types(run_fn)["some_input_2"] == None
+
 
 def test_optional_type_annotation():
     """Check that we keep the `Optional` wrapping on input types"""
 
     def _run(sample_input: Optional[int]):
         pass
```

### Comparing `caikit-0.2.0/tests/runtime/service_generation/test_create_service.py` & `caikit-0.2.1/tests/runtime/service_generation/test_create_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,23 @@
 untrainable_module_class = sample_lib.blocks.sample_task.SamplePrimitiveBlock
 
 ## Tests ########################################################################
 
 ### create_inference_rpcs tests #################################################
 
 
+def test_create_inference_rpcs_for_module_with_no_run_function():
+    class Foo:
+        def __init__(self):
+            pass
+
+    rpcs = create_inference_rpcs([Foo])
+    assert len(rpcs) == 0
+
+
 def test_create_inference_rpcs():
     rpcs = create_inference_rpcs([widget_class])
     assert len(rpcs) == 1
     assert widget_class in rpcs[0].module_list
 
 
 def test_create_inference_rpcs_for_multiple_modules_of_same_type():
@@ -74,14 +83,29 @@
     assert len(rpcs) == 1
     assert sample_lib.blocks.sample_task.SampleBlock in rpcs[0].module_list
 
 
 ### create_training_rpcs tests #################################################
 
 
+def test_create_inference_rpcs_for_module_with_no_train_function():
+    class Foo:
+        def __init__(self):
+            pass
+
+        def run(self):
+            pass
+
+        def train_in_progress(self):
+            pass
+
+    rpcs = create_inference_rpcs([Foo])
+    assert len(rpcs) == 0
+
+
 def test_create_training_rpcs():
     rpcs = create_training_rpcs([widget_class])
     assert len(rpcs) == 1
     assert widget_class in rpcs[0].module_list
 
 
 def test_create_training_rpcs_without_train():
```

### Comparing `caikit-0.2.0/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.2.1/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/service_generation/test_primitives.py` & `caikit-0.2.1/tests/runtime/service_generation/test_primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.2.1/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/servicers/__init__.py` & `caikit-0.2.1/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.2.1/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.2.1/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,14 +392,41 @@
         training_result = sample_train_servicer.training_map.get(
             training_response.training_id
         ).result()
 
     assert f"This may be a problem with your input" in str(context.value.message)
 
 
+def test_global_train_returns_exit_code_with_oom(
+    sample_train_service, sample_train_servicer
+):
+    """Test that if block goes into OOM we are able to surface error code"""
+    stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
+    training_data = stream_type(
+        jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
+    ).to_proto()
+    train_request = (
+        sample_train_service.messages.BlocksSampleTaskSampleBlockTrainRequest(
+            model_name="Foo Bar Training",
+            batch_size=42,
+            training_data=training_data,
+            oom_exit=True,
+        )
+    )
+
+    # Enable sub-processing for test
+    sample_train_servicer.use_subprocess = True
+
+    with pytest.raises(CaikitRuntimeException) as context:
+        training_response = sample_train_servicer.Train(train_request)
+        sample_train_servicer.training_map.get(training_response.training_id).result()
+
+    assert f"Training process died with OOM error!" in str(context.value.message)
+
+
 #####################################################################
 
 # NOTE: This test was commented out in the original unittest.TestCase impl - leaving as is
 # def test_global_train_aborts_long_running_trains(self):
 #     mock_manager = MagicMock()
 
 #     # return a dummy model from the mock model manager
```

### Comparing `caikit-0.2.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.2.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.2.1/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.2.1/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/test_grpc_server.py` & `caikit-0.2.1/tests/runtime/test_grpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -623,16 +623,16 @@
     ca_cert = tls_test_tools.generate_ca_cert(ca_key)
     tls_key, tls_cert = tls_test_tools.generate_derived_key_cert_pair(ca_key)
 
     tls_config = TLSConfig(
         server=KeyPair(cert=tls_cert, key=tls_key), client=KeyPair(cert="", key="")
     )
     with RuntimeGRPCServer(
-        infer_srv=sample_inference_service,
-        train_srv=None,
+        inference_service=sample_inference_service,
+        training_service=None,
         tls_config_override=tls_config,
     ) as server:
         _assert_connection(_make_secure_channel(server, ca_cert))
 
 
 def test_mtls(sample_inference_service):
     """Boot up a server with mTLS enabled and ping it on a secure channel"""
@@ -640,16 +640,16 @@
     ca_cert = tls_test_tools.generate_ca_cert(ca_key)
     tls_key, tls_cert = tls_test_tools.generate_derived_key_cert_pair(ca_key)
 
     tls_config = TLSConfig(
         server=KeyPair(cert=tls_cert, key=tls_key), client=KeyPair(cert=ca_cert, key="")
     )
     with RuntimeGRPCServer(
-        infer_srv=sample_inference_service,
-        train_srv=None,
+        inference_service=sample_inference_service,
+        training_service=None,
         tls_config_override=tls_config,
     ) as server:
         client_key, client_cert = tls_test_tools.generate_derived_key_cert_pair(ca_key)
         _assert_connection(
             _make_secure_channel(server, ca_cert, client_key, client_cert)
         )
 
@@ -680,32 +680,32 @@
         f.write(ca_cert)
 
     tls_config = TLSConfig(
         server=KeyPair(cert=tls_cert_path, key=tls_key_path),
         client=KeyPair(cert=ca_cert_path, key=""),
     )
     with RuntimeGRPCServer(
-        infer_srv=sample_inference_service,
-        train_srv=None,
+        inference_service=sample_inference_service,
+        training_service=None,
         tls_config_override=tls_config,
     ) as server:
         client_key, client_cert = tls_test_tools.generate_derived_key_cert_pair(ca_key)
         _assert_connection(
             _make_secure_channel(server, ca_cert, client_key, client_cert)
         )
 
 
 def test_metrics_stored_after_server_interrupt(
     loaded_model_id, sample_inference_service
 ):
     """This tests the gRPC server's behaviour when interrupted"""
 
     with RuntimeGRPCServer(
-        infer_srv=sample_inference_service,
-        train_srv=None,
+        inference_service=sample_inference_service,
+        training_service=None,
     ) as server:
         stub = sample_inference_service.stub_class(server.make_local_channel())
         predict_request = sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT
         )
         _ = stub.SampleTaskPredict(
             predict_request, metadata=[("mm-model-id", loaded_model_id)]
@@ -742,16 +742,16 @@
             "runtime": {
                 "port": free_high_port,
                 "find_available_port": False,
             }
         }
     ):
         with RuntimeGRPCServer(
-            infer_srv=sample_inference_service,
-            train_srv=None,
+            inference_service=sample_inference_service,
+            training_service=None,
         ) as server:
             _assert_connection(grpc.insecure_channel(f"localhost:{free_high_port}"))
 
 
 # Test implementation details #########################
 @dataclass
 class KeyPair:
```

### Comparing `caikit-0.2.0/tests/runtime/test_service_factory.py` & `caikit-0.2.1/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/utils/__init__.py` & `caikit-0.2.1/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/utils/test_import_util.py` & `caikit-0.2.1/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/utils/test_servicer_util.py` & `caikit-0.2.1/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/work_management/__init__.py` & `caikit-0.2.1/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.2.1/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.2.1/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.2.1/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/tox.ini` & `caikit-0.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-0.2.0/PKG-INFO` & `caikit-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.2.0
+Version: 0.2.1
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: alchemy-config>=1.1.1
-Requires-Dist: alchemy-logging>=1.0.4
+Requires-Dist: alchemy-config>=1.1.1,<2.0.0
+Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
-Requires-Dist: docstring-parser>=0.14.1
+Requires-Dist: docstring-parser>=0.14.1,<0.15.0
 Requires-Dist: grpcio-health-checking>=1.35.0,<2.0
 Requires-Dist: grpcio>=1.35.0,<2.0
 Requires-Dist: ijson>=3.1.4,<3.3.0
 Requires-Dist: munch>=2.5.0,<3.0
 Requires-Dist: protobuf>=3.19.0,<5
 Requires-Dist: prometheus_client==0.12.0
 Requires-Dist: py-grpc-prometheus>=0.7.0,<0.8
 Requires-Dist: PyYAML>=6.0,<7.0
 Requires-Dist: requests>=2.26.0,<3.0
 Requires-Dist: semver>=2.13.0,<4.0
 Requires-Dist: six>=1.16.0,<2.0.0
 Requires-Dist: tqdm>=4.59.0,<5.0.0
-Requires-Dist: wheel>=0.37.0
 Requires-Dist: jtd-to-proto>=0.12.1,<0.13.0
 Requires-Dist: import-tracker>=3.1.5,<4
 Project-URL: Source, https://github.com/caikit/caikit
 
 # Caikit
 
 Caikit is an AI toolkit that enables users to manage models through a set of developer friendly APIs. It provides a consistent format for creating and using AI models against a wide variety of data domains and tasks.
```

