# Comparing `tmp/caikit-0.7.0.tar.gz` & `tmp/caikit-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caikit-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit-0.7.0.tar` & `caikit-0.7.1.tar`

### file list

```diff
@@ -1,304 +1,303 @@
--rw-r--r--   0        0        0       60 2023-06-02 21:55:42.640922 caikit-0.7.0/.coveragerc
--rw-r--r--   0        0        0      676 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1571 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1328 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      246 2023-06-02 21:55:42.640922 caikit-0.7.0/.gitignore
--rw-r--r--   0        0        0      324 2023-06-02 21:55:42.640922 caikit-0.7.0/.isort.cfg
--rw-r--r--   0        0        0      370 2023-06-02 21:55:42.640922 caikit-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-06-02 21:55:42.640922 caikit-0.7.0/.prettierignore
--rw-r--r--   0        0        0       12 2023-06-02 21:55:42.640922 caikit-0.7.0/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-06-02 21:55:42.640922 caikit-0.7.0/.pylintrc
--rw-r--r--   0        0        0      530 2023-06-02 21:55:42.640922 caikit-0.7.0/.readthedocs.yaml
--rw-r--r--   0        0        0       78 2023-06-02 21:55:42.640922 caikit-0.7.0/.whitesource
--rw-r--r--   0        0        0      368 2023-06-02 21:55:42.640922 caikit-0.7.0/CODEOWNERS
--rw-r--r--   0        0        0     7164 2023-06-02 21:55:42.640922 caikit-0.7.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-06-02 21:55:42.640922 caikit-0.7.0/LICENSE
--rw-r--r--   0        0        0     3734 2023-06-02 21:55:42.640922 caikit-0.7.0/README.md
--rw-r--r--   0        0        0      152 2023-06-02 21:55:42.640922 caikit-0.7.0/SECURITY.md
--rw-r--r--   0        0        0    44878 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit-overview.png
--rw-r--r--   0        0        0      427 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/config/__init__.py
--rw-r--r--   0        0        0     6052 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/config/config.py
--rw-r--r--   0        0        0     6388 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/config/config.yml
--rw-r--r--   0        0        0     1642 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0     1027 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    37315 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2446 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     4997 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    14537 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     4858 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     5127 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/json_dict.py
--rw-r--r--   0        0        0     1564 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40212 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    21296 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/model_manager.py
--rw-r--r--   0        0        0      684 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2834 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     4718 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     2802 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     6002 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/module_backends/module_backend_config.py
--rw-r--r--   0        0        0      742 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/__init__.py
--rw-r--r--   0        0        0    30320 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/base.py
--rw-r--r--   0        0        0     6247 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/config.py
--rw-r--r--   0        0        0    11042 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/decorator.py
--rw-r--r--   0        0        0     4151 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/loader.py
--rw-r--r--   0        0        0     6013 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/meta.py
--rw-r--r--   0        0        0    13024 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/saver.py
--rw-r--r--   0        0        0     3895 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/registries.py
--rw-r--r--   0        0        0      654 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10721 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4688 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8221 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/signature_parsing/parsers.py
--rw-r--r--   0        0        0     7590 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/task.py
--rw-r--r--   0        0        0     1001 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    21366 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1648 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32206 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0      530 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1431 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     1886 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1662 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    14335 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    15675 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4659 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     5802 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12101 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4311 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1480 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    12209 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     4229 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    13914 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     5613 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/protoable.py
--rw-r--r--   0        0        0    11999 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/rpcs.py
--rw-r--r--   0        0        0     2216 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     9476 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    12441 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5440 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1667 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6810 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    19162 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0    11539 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/work_management/train_executors.py
--rw-r--r--   0        0        0      169 2023-06-02 21:55:42.648922 caikit-0.7.0/code-of-conduct.md
--rw-r--r--   0        0        0       90 2023-06-02 21:55:42.648922 caikit-0.7.0/docs-requirements.txt
--rw-r--r--   0        0        0      639 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/Makefile
--rw-r--r--   0        0        0     1610 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/adrs/010-data-model-definition.md
--rw-r--r--   0        0        0     2352 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/adrs/015-runtime-service-generation.md
--rw-r--r--   0        0        0     2581 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/adrs/018-shared-backends.md
--rw-r--r--   0        0        0     1223 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/adrs/019-loader-stack.md
--rw-r--r--   0        0        0      404 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-06-02 21:55:42.652922 caikit-0.7.0/docs/architecture_club/README.md
--rw-r--r--   0        0        0      805 2023-06-02 21:55:42.652922 caikit-0.7.0/docs/make.bat
--rw-r--r--   0        0        0     3053 2023-06-02 21:55:42.652922 caikit-0.7.0/docs/source/conf.py
--rw-r--r--   0        0        0      225 2023-06-02 21:55:42.652922 caikit-0.7.0/docs/source/index.rst
--rw-r--r--   0        0        0      837 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     6095 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/README.md
--rw-r--r--   0        0        0     1376 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/client.py
--rw-r--r--   0        0        0      673 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/models/text_sentiment/config.yml
--rw-r--r--   0        0        0       72 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/requirements.txt
--rw-r--r--   0        0        0      961 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/start_runtime.py
--rw-r--r--   0        0        0      816 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/text_sentiment/__init__.py
--rw-r--r--   0        0        0      615 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/text_sentiment/config.yml
--rw-r--r--   0        0        0      661 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/text_sentiment/data_model/__init__.py
--rw-r--r--   0        0        0     1422 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/text_sentiment/data_model/classification.py
--rw-r--r--   0        0        0      645 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
--rw-r--r--   0        0        0     3067 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
--rw-r--r--   0        0        0     1234 2023-06-02 21:55:46.829213 caikit-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2950 2023-06-02 21:55:42.652922 caikit-0.7.0/releases.md
--rwxr-xr-x   0        0        0      639 2023-06-02 21:55:42.652922 caikit-0.7.0/scripts/check_deps.sh
--rwxr-xr-x   0        0        0      720 2023-06-02 21:55:42.652922 caikit-0.7.0/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-06-02 21:55:42.652922 caikit-0.7.0/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     5240 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/base.py
--rw-r--r--   0        0        0        0 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/config/__init__.py
--rw-r--r--   0        0        0     5358 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/config/test_configs.py
--rw-r--r--   0        0        0     9913 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0        0 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     5033 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26459 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    16232 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    23532 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     5083 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/test_enums.py
--rw-r--r--   0        0        0     2358 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/test_json_dict.py
--rw-r--r--   0        0        0     1104 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     4378 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/helpers.py
--rw-r--r--   0        0        0        0 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2320 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     6888 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/module_backends/test_module_backend_config.py
--rw-r--r--   0        0        0        0 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/modules/__init__.py
--rw-r--r--   0        0        0    12551 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/modules/test_module.py
--rw-r--r--   0        0        0     6274 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/modules/test_module_metadata.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/signature_parsing/__init__.py
--rw-r--r--   0        0        0     4872 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8595 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0      521 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/test_imports.py
--rw-r--r--   0        0        0    21849 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/test_model_manager.py
--rw-r--r--   0        0        0     1038 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     6133 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/test_task.py
--rw-r--r--   0        0        0     7967 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    18396 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4997 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0     6782 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      591 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      154 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/control_chars.jsonl
--rw-r--r--   0        0        0      106 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0      222 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0     1017 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module.zip
--rw-r--r--   0        0        0      675 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module/config.yml
--rw-r--r--   0        0        0      299 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module/data.json
--rw-r--r--   0        0        0       14 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module/data.pkl
--rw-r--r--   0        0        0      191 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_backend/config.yml
--rw-r--r--   0        0        0      179 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_foo/config.yml
--rw-r--r--   0        0        0      508 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_no_id/config.yml
--rw-r--r--   0        0        0      508 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_no_nesting.zip
--rw-r--r--   0        0        0      570 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_singleton/data.json
--rw-r--r--   0        0        0       14 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_singleton/data.pkl
--rw-r--r--   0        0        0      230 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     3034 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      349 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      360 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      364 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      396 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     5995 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0       24 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      294 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      296 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      157 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0     1257 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0      156 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/__init__.py
--rw-r--r--   0        0        0       89 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/other_task/__init__.py
--rw-r--r--   0        0        0     1942 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
--rw-r--r--   0        0        0      250 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/__init__.py
--rw-r--r--   0        0        0     1720 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
--rw-r--r--   0        0        0      620 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
--rw-r--r--   0        0        0     2463 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1368 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2720 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      364 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_module/config.yml
--rw-r--r--   0        0        0        0 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3845 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14101 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    10266 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    17911 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5303 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     4035 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18431 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     3105 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/service_generation/test_protoable.py
--rw-r--r--   0        0        0     2345 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/service_generation/test_rpcs.py
--rw-r--r--   0        0        0     1376 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     8307 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    16742 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     4088 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7776 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4204 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    33005 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0     5072 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26059 2023-06-02 21:55:42.660923 caikit-0.7.0/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-06-02 21:55:42.660923 caikit-0.7.0/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2758 2023-06-02 21:55:42.660923 caikit-0.7.0/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-06-02 21:55:42.660923 caikit-0.7.0/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3819 2023-06-02 21:55:42.660923 caikit-0.7.0/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     2556 2023-06-02 21:55:42.660923 caikit-0.7.0/tox.ini
--rw-r--r--   0        0        0     4939 1970-01-01 00:00:00.000000 caikit-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-06-09 23:28:18.429314 caikit-0.7.1/.coveragerc
+-rw-r--r--   0        0        0      676 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1559 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1328 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1117 2023-06-09 23:28:18.429314 caikit-0.7.1/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      260 2023-06-09 23:28:18.429314 caikit-0.7.1/.gitignore
+-rw-r--r--   0        0        0      324 2023-06-09 23:28:18.429314 caikit-0.7.1/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-06-09 23:28:18.429314 caikit-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-06-09 23:28:18.429314 caikit-0.7.1/.prettierignore
+-rw-r--r--   0        0        0       12 2023-06-09 23:28:18.429314 caikit-0.7.1/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-06-09 23:28:18.433315 caikit-0.7.1/.pylintrc
+-rw-r--r--   0        0        0      530 2023-06-09 23:28:18.433315 caikit-0.7.1/.readthedocs.yaml
+-rw-r--r--   0        0        0       78 2023-06-09 23:28:18.433315 caikit-0.7.1/.whitesource
+-rw-r--r--   0        0        0      368 2023-06-09 23:28:18.433315 caikit-0.7.1/CODEOWNERS
+-rw-r--r--   0        0        0     7164 2023-06-09 23:28:18.433315 caikit-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-06-09 23:28:18.433315 caikit-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4448 2023-06-09 23:28:18.433315 caikit-0.7.1/README.md
+-rw-r--r--   0        0        0      152 2023-06-09 23:28:18.433315 caikit-0.7.1/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit-overview.png
+-rw-r--r--   0        0        0      427 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/config/__init__.py
+-rw-r--r--   0        0        0     6052 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/config/config.py
+-rw-r--r--   0        0        0     6388 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/config/config.yml
+-rw-r--r--   0        0        0     1642 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0     1027 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    37893 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2446 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     4997 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    14620 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4858 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     5127 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/json_dict.py
+-rw-r--r--   0        0        0     1564 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40244 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    21296 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/model_manager.py
+-rw-r--r--   0        0        0      684 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2834 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     4718 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     2802 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     6002 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/module_backends/module_backend_config.py
+-rw-r--r--   0        0        0      742 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/__init__.py
+-rw-r--r--   0        0        0    30320 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/base.py
+-rw-r--r--   0        0        0     6247 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/config.py
+-rw-r--r--   0        0        0    11042 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/decorator.py
+-rw-r--r--   0        0        0     4151 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/loader.py
+-rw-r--r--   0        0        0     6013 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/meta.py
+-rw-r--r--   0        0        0    13024 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/modules/saver.py
+-rw-r--r--   0        0        0     3895 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/registries.py
+-rw-r--r--   0        0        0      654 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10721 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4688 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8221 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     7590 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/task.py
+-rw-r--r--   0        0        0     1001 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-06-09 23:28:18.433315 caikit-0.7.1/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    21366 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1648 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32206 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0      530 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1431 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1662 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14335 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    15675 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     5802 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12101 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1480 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0     9607 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     4229 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    13127 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     5613 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/protoable.py
+-rw-r--r--   0        0        0    11999 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/rpcs.py
+-rw-r--r--   0        0        0     2216 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0    10766 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    12451 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5440 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6810 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    11842 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0    11924 2023-06-09 23:28:18.437315 caikit-0.7.1/caikit/runtime/work_management/train_executors.py
+-rw-r--r--   0        0        0      169 2023-06-09 23:28:18.437315 caikit-0.7.1/code-of-conduct.md
+-rw-r--r--   0        0        0       90 2023-06-09 23:28:18.437315 caikit-0.7.1/docs-requirements.txt
+-rw-r--r--   0        0        0      639 2023-06-09 23:28:18.437315 caikit-0.7.1/docs/Makefile
+-rw-r--r--   0        0        0     6860 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/adrs/001-module.md
+-rw-r--r--   0        0        0     1610 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0     2581 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/adrs/018-shared-backends.md
+-rw-r--r--   0        0        0     1223 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/adrs/019-loader-stack.md
+-rw-r--r--   0        0        0      404 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/architecture_club/README.md
+-rw-r--r--   0        0        0      805 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/make.bat
+-rw-r--r--   0        0        0     3053 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/source/conf.py
+-rw-r--r--   0        0        0      225 2023-06-09 23:28:18.441315 caikit-0.7.1/docs/source/index.rst
+-rw-r--r--   0        0        0      837 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1422 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      673 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       72 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      615 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1422 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      645 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3283 2023-06-09 23:28:18.441315 caikit-0.7.1/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
+-rw-r--r--   0        0        0     1234 2023-06-09 23:28:21.565361 caikit-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2950 2023-06-09 23:28:18.441315 caikit-0.7.1/releases.md
+-rwxr-xr-x   0        0        0      639 2023-06-09 23:28:18.441315 caikit-0.7.1/scripts/check_deps.sh
+-rwxr-xr-x   0        0        0      720 2023-06-09 23:28:18.441315 caikit-0.7.1/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-06-09 23:28:18.441315 caikit-0.7.1/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0     5240 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/base.py
+-rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/config/__init__.py
+-rw-r--r--   0        0        0     5358 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/config/test_configs.py
+-rw-r--r--   0        0        0    10361 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     5033 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26951 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    16232 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    25446 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     5083 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/test_enums.py
+-rw-r--r--   0        0        0     2358 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/test_json_dict.py
+-rw-r--r--   0        0        0     1104 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     4378 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2320 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     6888 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/module_backends/test_module_backend_config.py
+-rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/modules/__init__.py
+-rw-r--r--   0        0        0    12551 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/modules/test_module.py
+-rw-r--r--   0        0        0     6274 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/modules/test_module_metadata.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     4872 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8595 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0      521 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/test_imports.py
+-rw-r--r--   0        0        0    21849 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0     1038 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     6133 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/test_task.py
+-rw-r--r--   0        0        0        0 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     7967 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    18396 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4997 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0     6782 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      591 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      154 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/control_chars.jsonl
+-rw-r--r--   0        0        0      106 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-06-09 23:28:18.441315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0      222 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0     1017 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module.zip
+-rw-r--r--   0        0        0      675 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module/config.yml
+-rw-r--r--   0        0        0      299 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module/data.json
+-rw-r--r--   0        0        0       14 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module/data.pkl
+-rw-r--r--   0        0        0      191 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_backend/config.yml
+-rw-r--r--   0        0        0      179 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_foo/config.yml
+-rw-r--r--   0        0        0      508 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_no_id/config.yml
+-rw-r--r--   0        0        0      508 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_no_nesting.zip
+-rw-r--r--   0        0        0      570 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_module_singleton/data.pkl
+-rw-r--r--   0        0        0      230 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     3034 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      349 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      360 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      364 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      396 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0       24 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      294 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      157 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0     1257 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0      156 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/__init__.py
+-rw-r--r--   0        0        0       89 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/other_task/__init__.py
+-rw-r--r--   0        0        0     1946 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
+-rw-r--r--   0        0        0      250 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/__init__.py
+-rw-r--r--   0        0        0     1720 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
+-rw-r--r--   0        0        0      902 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
+-rw-r--r--   0        0        0     2463 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1410 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2720 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      364 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/fixtures/sample_module/config.yml
+-rw-r--r--   0        0        0        0 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3845 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14101 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    10266 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    17911 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5303 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     4035 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    17954 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     3105 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/service_generation/test_protoable.py
+-rw-r--r--   0        0        0     2345 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/service_generation/test_rpcs.py
+-rw-r--r--   0        0        0     1376 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     8381 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    16256 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     4088 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7776 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    35791 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0     5072 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    17336 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2758 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3819 2023-06-09 23:28:18.445315 caikit-0.7.1/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     2617 2023-06-09 23:28:18.445315 caikit-0.7.1/tox.ini
+-rw-r--r--   0        0        0     5653 1970-01-01 00:00:00.000000 caikit-0.7.1/PKG-INFO
```

### Comparing `caikit-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.7.1/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/.github/workflows/build-library.yml` & `caikit-0.7.1/.github/workflows/build-library.yml`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-name: Build Caikit Core Library
+name: Build and Test
 
 on:
   push:
     branches: [ "main" ]
   pull_request:
     branches: [ "main" ]
 
@@ -46,8 +46,7 @@
           python-version: ${{ matrix.python-version.setup }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install -r setup_requirements.txt
       - name: Build and test with tox
         run: tox -e ${{ matrix.python-version.tox }}
-
```

### Comparing `caikit-0.7.0/.github/workflows/lint-code.yml` & `caikit-0.7.1/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/.github/workflows/publish-library.yml` & `caikit-0.7.1/.github/workflows/publish-library.yml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-name: Upload Caikit Core Library
+name: Publish
 
 on:
   release:
     types: [published]
 
 jobs:
   build:
```

### Comparing `caikit-0.7.0/.pylintrc` & `caikit-0.7.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/.readthedocs.yaml` & `caikit-0.7.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/CONTRIBUTING.md` & `caikit-0.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/LICENSE` & `caikit-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/README.md` & `caikit-0.7.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Caikit
 
+[![Build Status](https://github.com/caikit/caikit/actions/workflows/build-library.yml/badge.svg?branch=main&label=tests)](https://github.com/caikit/caikit/actions)
+[![Minimum Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
+[![Release](https://img.shields.io/github/v/release/caikit/caikit?include_prereleases&style=)](https://github.com/caikit/caikit/releases/)
+[![Read the Docs](https://img.shields.io/static/v1?label=readthedocs&message=reference&color=blue)](https://caikit.readthedocs.io/en/latest/)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7443/badge)](https://bestpractices.coreinfrastructure.org/projects/7443)
+
 Caikit is an AI toolkit that enables users to manage models through a set of developer friendly APIs. It provides a consistent format for creating and using AI models against a wide variety of data domains and tasks.
 
 ![Caikit Overview](https://raw.githubusercontent.com/caikit/caikit/main/caikit-overview.png)
 
 ## Capabilities
 
 Caikit streamlines the management of AI models for application usage by letting AI model authors focus on solving well known problems with novel technology. With a set of model implementations based on Caikit, you can:
```

### Comparing `caikit-0.7.0/caikit-overview.png` & `caikit-0.7.1/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/config/__init__.py` & `caikit-0.7.1/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/config/config.py` & `caikit-0.7.1/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/config/config.yml` & `caikit-0.7.1/caikit/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/__init__.py` & `caikit-0.7.1/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/augmentors/__init__.py` & `caikit-0.7.1/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/augmentors/base.py` & `caikit-0.7.1/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.7.1/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.7.1/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/augmentors/schemes/base.py` & `caikit-0.7.1/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.7.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.7.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/__init__.py` & `caikit-0.7.1/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/base.py` & `caikit-0.7.1/caikit/core/data_model/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -809,14 +809,27 @@
             if (
                 not field in self._fields_to_oneof
                 or self.which_oneof(self._fields_to_oneof[field]) == field
             ):
                 fields_to_dict.append(field)
         return {field: self._field_to_dict_element(field) for field in fields_to_dict}
 
+    def to_kwargs(self) -> dict:
+        """Convert to flat dictionary representation. (Like .to_dict, but not recursive)
+        This keeps the attribute names of any fields backed by oneofs, instead of using the
+        internal oneof field name
+        """
+        fields_to_dict = []
+        for field in self.fields:
+            if field not in self._fields_to_oneof:
+                fields_to_dict.append(field)
+            else:
+                fields_to_dict.append(self._fields_to_oneof[field])
+        return {field: getattr(self, field) for field in fields_to_dict}
+
     def to_json(self, **kwargs) -> str:
         """Convert to a json representation."""
 
         def _default_serialization_overrides(obj):
             """Default handler for nonserializable objects; currently this only handles bytes."""
             if isinstance(obj, bytes):
                 return base64.encodebytes(obj).decode("utf-8")
```

### Comparing `caikit-0.7.0/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.7.1/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/data_backends/base.py` & `caikit-0.7.1/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.7.1/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/dataobject.py` & `caikit-0.7.1/caikit/core/data_model/dataobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,8 +377,10 @@
 
 
 def _has_dataclass_init(cls) -> bool:
     """When the dataclass decorator adds an __init__ to a class, it adds
     __annotations__ to the init function itself. This function uses that fact to
     detect if the class's __init__ function was generated by @dataclass
     """
-    return bool(getattr(cls.__init__, "__annotations__", None))
+    return bool(getattr(cls.__init__, "__annotations__", None)) and not any(
+        cls.__init__ is base.__init__ for base in cls.__bases__
+    )
```

### Comparing `caikit-0.7.0/caikit/core/data_model/enums.py` & `caikit-0.7.1/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/json_dict.py` & `caikit-0.7.1/caikit/core/data_model/json_dict.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/producer.py` & `caikit-0.7.1/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.7.1/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/streams/__init__.py` & `caikit-0.7.1/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/streams/converter.py` & `caikit-0.7.1/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.7.1/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/streams/data_stream.py` & `caikit-0.7.1/caikit/core/data_model/streams/data_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,17 +121,19 @@
             >>> for data_item in list_stream:
             >>>     print(data_item)
             1
             2
             3
         """
         error.type_check("<COR88684982E>", Iterable, data=data)
+        return cls(cls._from_iterable_generator, data)
 
-        # lambda closure over `data` that returns an iterator over `data`
-        return cls(lambda: iter(data))
+    @classmethod
+    def _from_iterable_generator(cls, data: typing.Iterable[T]) -> typing.Iterator[T]:
+        return iter(data)
 
     @classmethod
     def from_jsonl(cls, filename: str) -> "DataStream[Dict]":
         """Creates a new data stream from a path to a file with JSON lines array, where
         each line is a valid JSON (python dict)
 
         Args:
@@ -164,36 +166,36 @@
             {'name': 'Alexa', 'wins': [['two pair', '4♠'], ['two pair', '9♠']]}
             {'name': 'May', 'wins': []}
             {'name': 'Deloise', 'wins': [['three of a kind', '5♣']]}
 
         """
         error.file_check("<COR32600575E>", filename)
 
-        def generator_func():
-            # open the file (closure around `filename`)
-            with open(filename, mode="rb") as json_fh:
-                log.debug2("Loading JSON array file: {}".format(filename))
-                lines = json_fh.readlines()
-
-                try:
-                    for line in lines:
-                        if line.strip():  # ignore empty lines
-                            yield json.loads(line)
-                except json.JSONDecodeError as e:
-                    error(
-                        "<COR55596551E>",
-                        ValueError(f"Invalid JSON object in `{line}`, error: {e.msg}"),
-                    )
-                except TypeError:
-                    error(
-                        "<COR35596551E>",
-                        ValueError("Invalid JSON object in `{}`".format(line)),
-                    )
+        return cls(cls._from_jsonl_generator, filename)
 
-        return cls(generator_func)
+    @classmethod
+    def _from_jsonl_generator(cls, filename):
+        with open(filename, mode="rb") as json_fh:
+            log.debug2("Loading JSON array file:  %s", filename)
+            lines = json_fh.readlines()
+
+            try:
+                for line in lines:
+                    if line.strip():  # ignore empty lines
+                        yield json.loads(line)
+            except json.JSONDecodeError as e:
+                error(
+                    "<COR55596551E>",
+                    ValueError(f"Invalid JSON object in `{line}`, error: {e.msg}"),
+                )
+            except TypeError:
+                error(
+                    "<COR35596551E>",
+                    ValueError("Invalid JSON object in `{}`".format(line)),
+                )
 
     @classmethod
     def from_json_array(cls, filename: str) -> "DataStream[Dict]":
         """Creates a new data stream from a path to a file with JSON array, where each item is a
         valid JSON (python dict)
 
         Args:
@@ -224,32 +226,33 @@
             { a: 1, b: 2, c: False }
             { a: 2, b: 3 }
             { a: 3, c: True }
 
         """
         error.file_check("<COR39609575E>", filename)
 
-        def generator_func():
-            # open the file (closure around `filename`)
-            with open(filename, mode="rb") as json_fh:
-                log.debug2("Loading JSON array file: {}".format(filename))
-
-                # for each {} object of the array
-                try:
-                    for item_idx, obj in enumerate(ijson.items(json_fh, "item")):
-                        log.debug2("Loading object index %d", item_idx)
-                        yield obj
-
-                except ijson.JSONError:
-                    error(
-                        "<COR85596551E>",
-                        ValueError("Invalid JSON object in `{}`".format(filename)),
-                    )
+        return cls(cls._from_json_array_generator, filename)
 
-        return cls(generator_func)
+    @classmethod
+    def _from_json_array_generator(cls, filename):
+        # open the file
+        with open(filename, mode="rb") as json_fh:
+            log.debug2("Loading JSON array file: %s", filename)
+
+            # for each {} object of the array
+            try:
+                for item_idx, obj in enumerate(ijson.items(json_fh, "item")):
+                    log.debug2("Loading object index %d", item_idx)
+                    yield obj
+
+            except ijson.JSONError:
+                error(
+                    "<COR85596551E>",
+                    ValueError("Invalid JSON object in `{}`".format(filename)),
+                )
 
     @classmethod
     def from_csv(cls, filename: str, *args, skip=0, **kwargs) -> "DataStream[List]":
         """Create a new data stream from a csv (comma separated value) file where each data item
         corresponds to a line of the csv file and consists of a list containing the comma separated
         values.
 
@@ -284,28 +287,28 @@
                 FileNotFoundError(
                     "csv filename `{}` does not exist or is not a regular file.".format(
                         filename
                     )
                 ),
             )
 
-        # generator function that yields lists each containing the columns of the csv file
-        def generator_func(*csv_args, **csv_kwargs):
-            # open the csv file (closure around `filename`)
-            with open(filename, mode="r", encoding="utf8") as fh:
-                # skip lines if requested
-                for _ in range(skip):
-                    # pylint: disable=stop-iteration-return
-                    next(fh)
-
-                # for each line of the csv file, yield a list
-                for line in csv.reader(fh, *csv_args, **csv_kwargs):
-                    yield line
+        return cls(cls._from_csv_generator, filename, skip, *args, **kwargs)
 
-        return cls(generator_func, *args, **kwargs)
+    @classmethod
+    def _from_csv_generator(cls, filename, skip, *csv_args, **csv_kwargs):
+        # open the csv file (closure around `filename`)
+        with open(filename, mode="r", encoding="utf8") as fh:
+            # skip lines if requested
+            for _ in range(skip):
+                # pylint: disable=stop-iteration-return
+                next(fh)
+
+            # for each line of the csv file, yield a list
+            for line in csv.reader(fh, *csv_args, **csv_kwargs):
+                yield line
 
     @classmethod
     def from_header_csv(cls, filename: str, *args, **kwargs) -> "DataStream[Dict]":
         """Create a new data stream from a csv where the first row is a header
         and each subsequent row is an element. The yielded elements are tuples
         of dicts where each dict pairs the row values with the corresponding
         column headers.
@@ -339,24 +342,24 @@
                 FileNotFoundError(
                     "csv filename `{}` does not exist or is not a regular file.".format(
                         filename
                     )
                 ),
             )
 
-        # generator function that yields dicts
-        def generator_func(*csv_args, **csv_kwargs):
-            # open the csv file (closure around `filename`)
-            with open(filename, mode="r", encoding="utf8") as fh:
-
-                # for each line of the csv file, yield a dict
-                for line in csv.DictReader(fh, *csv_args, **csv_kwargs):
-                    yield line
+        return cls(cls._from_header_csv_generator, filename, *args, **kwargs)
 
-        return cls(generator_func, *args, **kwargs)
+    @classmethod
+    def _from_header_csv_generator(cls, filename, *csv_args, **csv_kwargs):
+        # open the csv file (closure around `filename`)
+        with open(filename, mode="r", encoding="utf8") as fh:
+
+            # for each line of the csv file, yield a dict
+            for line in csv.DictReader(fh, *csv_args, **csv_kwargs):
+                yield line
 
     @classmethod
     def from_txt(cls, filename: str) -> "DataStream[str]":
         """Create a new data stream from a path to a utf8 encoded text file where each data item
         corresponds to a single line of the file.
 
         Args:
@@ -384,23 +387,24 @@
             >>>     print(data_item)
             first line
             second line
             third line
         """
         error.file_check("<COR79693043E>", filename)
 
-        def generator_func():
-            # open the file (closure around `filename`)
-            with open(filename, mode="r", encoding="utf8") as fh:
-                # for each line of the file
-                for line in fh:
-                    # strip new lines and carriage returns and yield the line
-                    yield line.rstrip("\n\r")
+        return cls(cls._from_txt_generator, filename)
 
-        return cls(generator_func)
+    @classmethod
+    def _from_txt_generator(cls, filename):
+        # open the file (closure around `filename`)
+        with open(filename, mode="r", encoding="utf8") as fh:
+            # for each line of the file
+            for line in fh:
+                # strip new lines and carriage returns and yield the line
+                yield line.rstrip("\n\r")
 
     @classmethod
     def from_file(cls, filename: str) -> "DataStream[Union[Dict, Tuple, str]]":
         """Loads up a DataStream from a file.
             Will call the correct DataStream.from_caikit static constructor based on the
             file extension
 
@@ -416,26 +420,22 @@
         Returns:
             DataStream: resulting datastream from file
         """
         # file detection
         _, file_ext = os.path.splitext(filename)
         # choose the right from_* fn
         if file_ext.lower() == ".json":
-            log.debug2(
-                "Detected .json extension, loading {} as a json file".format(filename)
-            )
+            log.debug2("Detected .json extension, loading %s as a json file", filename)
             return DataStream.from_json_array(filename)
 
         if file_ext.lower() == ".csv":
-            log.debug2(
-                "Detected .csv extension, loading {} as a csv file".format(filename)
-            )
+            log.debug2("Detected .csv extension, loading %s as a csv file", filename)
             return DataStream.from_csv(filename)
 
-        log.debug2("Loading {} as a raw text file".format(filename))
+        log.debug2("Loading %s as a raw text file", filename)
         # TODO: test this at some point (this path is unused currently)
         return DataStream.from_txt(filename)
 
     @classmethod
     def _from_collection(
         cls, dirname: str, extension: str, file_opener
     ) -> "DataStream[Union[Dict, Tuple, str]]":
@@ -461,20 +461,21 @@
         Notes:
             Each data item in this data stream represents the *entire* text contained in a single
             file and are not split by line or otherwise.
         """
         # verify that `dirname` exists
         cls._verify_dir(dirname)
 
-        def generator_func():
-            # glob `*.txt` files in `dirname` (closure around `dirname`)
-            for filename in glob(os.path.join(dirname, "*." + extension)):
-                yield file_opener(filename)
+        return cls(cls._from_collection_generator, dirname, extension, file_opener)
 
-        return cls(generator_func)
+    @classmethod
+    def _from_collection_generator(cls, dirname, extension, file_opener):
+        # glob `*.txt` files in `dirname` (closure around `dirname`)
+        for filename in glob(os.path.join(dirname, "*." + extension)):
+            yield file_opener(filename)
 
     @classmethod
     def from_txt_collection(cls, dirname: str, extension="txt") -> "DataStream[str]":
         """Create a new data stream from a path containing multiple utf8 encoded text files where
         each data item corresponds to the entire text contained in a single file.
 
         Args:
@@ -536,25 +537,26 @@
                 A new data stream that is chained from all data streams by reading
                 (from_header_csv) all files in all `.csv` files found in `dirname`.
                 All data items are dicts.
         """
         # verify that `dirname` exists
         cls._verify_dir(dirname)
 
-        def generator_func():
-            # list of data_streams created from different files
-            data_stream_list = []
-            # glob `*.txt` files in `dirname` (closure around `dirname`)
-            for filename in glob(os.path.join(dirname, "*.csv")):
-                data_stream_list.append(cls.from_header_csv(filename=filename))
-            # yield the combined data item once flattened
-            for data_item in DataStream.chain(data_stream_list).flatten():
-                yield data_item
+        return cls(cls._from_csv_collection_generator, dirname)
 
-        return cls(generator_func)
+    @classmethod
+    def _from_csv_collection_generator(cls, dirname):
+        # list of data_streams created from different files
+        data_stream_list = []
+        # glob `*.txt` files in `dirname` (closure around `dirname`)
+        for filename in glob(os.path.join(dirname, "*.csv")):
+            data_stream_list.append(cls.from_header_csv(filename=filename))
+        # yield the combined data item once flattened
+        for data_item in DataStream.chain(data_stream_list).flatten():
+            yield data_item
 
     @classmethod
     def from_jsonl_collection(cls, dirname: str) -> "DataStream[Dict]":
         """Create a new data stream by chaining data streams from each of the file from a path
         containing multiple jsonl files where each file can have 1 or more data item.
 
         Args:
@@ -565,25 +567,26 @@
             DataStream
                 A new data stream that is chained from all data streams by reading
                 (from_jsonl) all files in all `.jsonl` files found in `dirname`.
         """
         # verify that `dirname` exists
         cls._verify_dir(dirname)
 
-        def generator_func():
-            # list of data_streams created from different files
-            data_stream_list = []
-            # glob `*.txt` files in `dirname` (closure around `dirname`)
-            for filename in glob(os.path.join(dirname, "*.jsonl")):
-                data_stream_list.append(cls.from_jsonl(filename=filename))
-            # yield the combined data item once flattened
-            for data_item in DataStream.chain(data_stream_list).flatten():
-                yield data_item
+        return cls(cls._from_jsonl_collection_generator, dirname)
 
-        return cls(generator_func)
+    @classmethod
+    def _from_jsonl_collection_generator(cls, dirname):
+        # list of data_streams created from different files
+        data_stream_list = []
+        # glob `*.txt` files in `dirname` (closure around `dirname`)
+        for filename in glob(os.path.join(dirname, "*.jsonl")):
+            data_stream_list.append(cls.from_jsonl(filename=filename))
+        # yield the combined data item once flattened
+        for data_item in DataStream.chain(data_stream_list).flatten():
+            yield data_item
 
     def train_test_split(
         self, test_split=0.25, seed=None
     ) -> "Tuple[DataStream[T], DataStream[T]]":
         """Split the current datastream into train/test substreams.
 
         Args:
```

### Comparing `caikit-0.7.0/caikit/core/data_model/streams/resolver.py` & `caikit-0.7.1/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/data_model/streams/validator.py` & `caikit-0.7.1/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/model_manager.py` & `caikit-0.7.1/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/module_backends/__init__.py` & `caikit-0.7.1/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/module_backends/backend_types.py` & `caikit-0.7.1/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/module_backends/base.py` & `caikit-0.7.1/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/module_backends/local_backend.py` & `caikit-0.7.1/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/module_backends/module_backend_config.py` & `caikit-0.7.1/caikit/core/module_backends/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/modules/__init__.py` & `caikit-0.7.1/caikit/core/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/modules/base.py` & `caikit-0.7.1/caikit/core/modules/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/modules/config.py` & `caikit-0.7.1/caikit/core/modules/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/modules/decorator.py` & `caikit-0.7.1/caikit/core/modules/decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/modules/loader.py` & `caikit-0.7.1/caikit/core/modules/loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/modules/meta.py` & `caikit-0.7.1/caikit/core/modules/meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/modules/saver.py` & `caikit-0.7.1/caikit/core/modules/saver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/registries.py` & `caikit-0.7.1/caikit/core/registries.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/signature_parsing/__init__.py` & `caikit-0.7.1/caikit/core/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/signature_parsing/docstrings.py` & `caikit-0.7.1/caikit/core/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/signature_parsing/module_signature.py` & `caikit-0.7.1/caikit/core/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/signature_parsing/parsers.py` & `caikit-0.7.1/caikit/core/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/task.py` & `caikit-0.7.1/caikit/core/task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/toolkit/__init__.py` & `caikit-0.7.1/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/toolkit/compatibility.py` & `caikit-0.7.1/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/toolkit/errors/__init__.py` & `caikit-0.7.1/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.7.1/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.7.1/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/toolkit/fileio.py` & `caikit-0.7.1/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/toolkit/isa.py` & `caikit-0.7.1/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/toolkit/logging.py` & `caikit-0.7.1/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.7.1/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/toolkit/serializers.py` & `caikit-0.7.1/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/core/toolkit/wip_decorator.py` & `caikit-0.7.1/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/interfaces/__init__.py` & `caikit-0.7.1/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/interfaces/common/__init__.py` & `caikit-0.7.1/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.7.1/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/interfaces/common/data_model/producer.py` & `caikit-0.7.1/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/interfaces/runtime/__init__.py` & `caikit-0.7.1/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.7.1/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.7.1/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/__init__.py` & `caikit-0.7.1/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/dump_services.py` & `caikit-0.7.1/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/grpc_server.py` & `caikit-0.7.1/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/interceptors/__init__.py` & `caikit-0.7.1/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.7.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/metrics/__init__.py` & `caikit-0.7.1/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.7.1/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/model_management/__init__.py` & `caikit-0.7.1/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/model_management/batcher.py` & `caikit-0.7.1/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/model_management/loaded_model.py` & `caikit-0.7.1/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/model_management/model_loader.py` & `caikit-0.7.1/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/model_management/model_manager.py` & `caikit-0.7.1/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/model_management/model_sizer.py` & `caikit-0.7.1/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/model_management/training_manager.py` & `caikit-0.7.1/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/protobufs/__init__.py` & `caikit-0.7.1/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.7.1/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.7.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.7.1/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.7.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.7.1/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.7.1/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.7.1/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.7.1/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.7.1/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/service_factory.py` & `caikit-0.7.1/caikit/runtime/service_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 from caikit import get_config
 from caikit.core import ModuleBase
 from caikit.interfaces.runtime.data_model import (
     TrainingInfoRequest,
     TrainingInfoResponse,
 )
 from caikit.runtime import service_generation
-from caikit.runtime.service_generation.rpcs import snake_to_upper_camel
-from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
+from caikit.runtime.service_generation.rpcs import CaikitRPCBase, snake_to_upper_camel
 from caikit.runtime.utils import import_util
 import caikit.core
 
 log = alog.use_channel("SVC-FACTORY")
 
 TRAINING_MANAGEMENT_SERVICE_NAME = "TrainingManagement"
 TRAINING_MANAGEMENT_SERVICE_SPEC = {
@@ -70,14 +69,15 @@
     service: Type[google.protobuf.service.Service]
     descriptor: google.protobuf.descriptor.ServiceDescriptor
     registration_function: Callable[
         [google.protobuf.service.Service, grpc.Server], None
     ]
     stub_class: Type
     messages: ModuleType
+    caikit_rpcs: Set[CaikitRPCBase]
 
 
 class ServicePackageFactory:
     """Factory responsible for yielding the correct concrete ServicePackage implementation"""
 
     class ServiceType(Enum):
         INFERENCE = 1  # Inference service for the GlobalPredictServicer
@@ -107,14 +107,15 @@
 
             return ServicePackage(
                 service=grpc_service.service_class,
                 descriptor=grpc_service.descriptor,
                 registration_function=grpc_service.registration_function,
                 stub_class=grpc_service.client_stub_class,
                 messages=None,  # we don't need messages here
+                caikit_rpcs=set(),  # No caikit RPCs
             )
 
         # First make sure we import the data model for the correct library
         # !!!! This will use the `caikit_library` config
         _ = import_util.get_data_model()
 
         caikit_config = get_config()
@@ -157,14 +158,15 @@
 
         return ServicePackage(
             service=grpc_service.service_class,
             descriptor=grpc_service.descriptor,
             registration_function=grpc_service.registration_function,
             stub_class=grpc_service.client_stub_class,
             messages=client_module,
+            caikit_rpcs=set(task_rpc_list),
         )
 
     # Implementation details for pure python service packages #
     @staticmethod
     def _get_and_filter_modules(
         caikit_config: aconfig.Config, lib: str
     ) -> Set[Type[ModuleBase]]:
@@ -247,74 +249,7 @@
             "Filtered list of modules %s after excluding task types: %s and modules ids: %s. \
                 Exclusions are defined in config",
             clean_modules,
             excluded_task_types,
             excluded_modules,
         )
         return clean_modules
-
-    # Implementation Details for protoc-compiled packages #
-    @staticmethod
-    def _get_service_descriptor(
-        caikit_runtime_pb2,
-        lib_name,
-    ) -> google.protobuf.descriptor.ServiceDescriptor:
-        """Get Service descriptor from caikit_runtime_pb2 module"""
-        service = f"_{lib_name.upper()}SERVICE"
-        train_service = f"_{lib_name.upper()}TRAININGSERVICE"
-
-        if hasattr(caikit_runtime_pb2, service):
-            return getattr(caikit_runtime_pb2, service)
-        if hasattr(caikit_runtime_pb2, train_service):
-            return getattr(caikit_runtime_pb2, train_service)
-
-        raise CaikitRuntimeException(
-            grpc.StatusCode.INTERNAL,
-            "Could not find service descriptor in caikit_runtime_pb2",
-        )
-
-    @staticmethod
-    def _get_servicer_class(
-        caikit_runtime_pb2_grpc,
-        lib_name,
-    ) -> Type[google.protobuf.service.Service]:
-        """Get google.protobufs.service.Service interface class from
-        caikit_runtime_pb2_grpc module"""
-        servicer = f"{lib_name}ServiceServicer"
-        train_servicer = f"{lib_name}TrainingServiceServicer"
-
-        if hasattr(caikit_runtime_pb2_grpc, servicer):
-            return getattr(caikit_runtime_pb2_grpc, servicer)
-        if hasattr(caikit_runtime_pb2_grpc, train_servicer):
-            return getattr(caikit_runtime_pb2_grpc, train_servicer)
-
-        raise CaikitRuntimeException(
-            grpc.StatusCode.INTERNAL,
-            f"Could not find servicer class {servicer} or {train_servicer} "
-            "in caikit_runtime_pb2_grpc",
-        )
-
-    @staticmethod
-    def _get_servicer_stub(
-        caikit_runtime_pb2_grpc,
-        lib_name,
-    ) -> type:
-        """Get ServiceStub class from caikit_runtime_pb2_grpc module"""
-        servicer = f"{lib_name}ServiceStub"
-        train_servicer = f"{lib_name}TrainingServiceStub"
-
-        if hasattr(caikit_runtime_pb2_grpc, servicer):
-            return getattr(caikit_runtime_pb2_grpc, servicer)
-        if hasattr(caikit_runtime_pb2_grpc, train_servicer):
-            return getattr(caikit_runtime_pb2_grpc, train_servicer)
-
-        raise CaikitRuntimeException(
-            grpc.StatusCode.INTERNAL,
-            "Could not find servicer stub in caikit_runtime_pb2_grpc",
-        )
-
-    @staticmethod
-    def _get_lib_name_for_servicer() -> str:
-        """Get caikit library name from Config, make upper case and not include caikit_"""
-        lib_names = import_util.clean_lib_names(get_config().runtime.library)
-        assert len(lib_names) == 1, "Only 1 caikit library supported for now"
-        return snake_to_upper_camel(lib_names[0].replace("caikit_", ""))
```

### Comparing `caikit-0.7.0/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.7.1/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/service_generation/create_service.py` & `caikit-0.7.1/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.7.1/caikit/runtime/service_generation/data_stream_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
-from datetime import datetime
 from glob import glob
-from typing import Any, List, Optional, Type, Union
+from typing import Any, List, Type, Union
 import os
 import sys
 
 # Third Party
-from google.protobuf.message import Message as ProtoMessageType
 import grpc
 
 # First Party
 from py_to_proto.dataclass_to_proto import Annotated, OneofField
 import alog
 
 # Local
@@ -40,35 +38,28 @@
 import caikit
 
 # This global holds the mapping of element types to their respective
 # DataStreamSource wrappers so that the same message is not recreated
 # unnecessarily
 _DATA_STREAM_SOURCE_TYPES = {}
 
-# Python type -> jtd name
-_NATIVE_TYPE_TO_JTD = {
-    str: "string",
-    int: "int64",
-    float: "float64",
-    bytes: "bytes",
-    bool: "boolean",
-    datetime: "timestamp",
-}
-
 log = alog.use_channel("DSTRM-SRC")
 
 
 class DataStreamSourceBase(DataStream):
     """This base class acts as a sentinel so that dynamically generated data
     stream source classes can be identified programmatically.
     """
 
     def __init__(self):
-        """Validate oneof semantics"""
-        super().__init__(lambda: self.to_data_stream().generator_func())
+        super().__init__(self._generator)
+
+    def _generator(self):
+        stream = self.to_data_stream()
+        return stream.generator_func(*stream.generator_args, **stream.generator_kwargs)
 
     def __getstate__(self) -> bytes:
         """A DataStreamSource is pickled by serializing its source
         representation. This is particularly useful when sharing data streams
         across subprocesses to run training in an isolated process.
         """
         return self.to_binary_buffer()
@@ -318,23 +309,11 @@
 
         _DATA_STREAM_SOURCE_TYPES[data_element_type] = data_object
 
     # Return the global stream source object for this element type
     return _DATA_STREAM_SOURCE_TYPES[data_element_type]
 
 
-def get_data_stream_source(message: Any) -> Optional[Type[DataStreamSourceBase]]:
-    """Get the data stream source from the given message if possible"""
-    # If it's a protobuf message, alias to the corresponding DM class if
-    # possible
-    if isinstance(message, ProtoMessageType):
-        # NOTE: This is the _very_ naive implementation and is potentially quite
-        #   inefficient with the current from_proto implementation
-        message = DataBase.get_class_for_proto(message).from_proto(message)
-    if isinstance(message, DataStreamSourceBase):
-        return message
-
-
 def _make_data_stream_source_type_name(data_element_type: Type) -> str:
     """Make the name for data stream source class that wraps the given type"""
     element_name = data_element_type.__name__
     return "DataStreamSource{}".format(element_name[0].upper() + element_name[1:])
```

### Comparing `caikit-0.7.0/caikit/runtime/service_generation/protoable.py` & `caikit-0.7.1/caikit/runtime/service_generation/protoable.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/service_generation/rpcs.py` & `caikit-0.7.1/caikit/runtime/service_generation/rpcs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.7.1/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/servicers/__init__.py` & `caikit-0.7.1/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.7.1/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,29 +9,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Standard
 from importlib.metadata import version
+from typing import Set
 import traceback
 
 # Third Party
 from google.protobuf.descriptor import FieldDescriptor
 from grpc import StatusCode
 from prometheus_client import Counter, Summary
 
 # First Party
 import alog
 
 # Local
 from caikit import get_config
+from caikit.core import ModuleBase
 from caikit.runtime.metrics.rpc_meter import RPCMeter
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.service_factory import ServicePackage
+from caikit.runtime.service_generation.rpcs import TaskPredictRPC
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils.import_util import clean_lib_names
 from caikit.runtime.utils.servicer_util import (
     build_caikit_library_request_dict,
     build_proto_response,
     get_metadata,
     validate_data_model,
@@ -131,33 +134,37 @@
             context(grpc.ServicerContext): Context object (contains request metadata, etc)
 
         Returns:
             response (object):
                 A Caikit Library data model response object
         """
         desc_name = request.DESCRIPTOR.name
-        outer_scope_name = "GlobalPredictServicerMock.Predict:%s" % desc_name
+        outer_scope_name = "GlobalPredictServicer.Predict:%s" % desc_name
         inner_scope_name = (
-            "GlobalPredictServicerImpl.Predict.caikit_library_run:%s" % desc_name
+            "GlobalPredictServicer.Predict.caikit_library_run:%s" % desc_name
         )
 
         try:
             with alog.ContextLog(log.debug, outer_scope_name):
                 # Make sure the request has a model before doing anything
                 model_id = get_metadata(context, self.MODEL_MESH_MODEL_ID_KEY)
                 # Retrieve the model from the model manager
                 log.debug("<RUN52259029D>", "Retrieving model '%s'", model_id)
                 model = self._model_manager.retrieve_model(model_id)
 
+                self._verify_model_task(model, desc_name)
+
+                model_class = type(model)
                 # Unmarshall the request object into the required module run argument(s)
                 with PREDICT_FROM_PROTO_SUMMARY.labels(
                     grpc_request=desc_name, model_id=model_id
                 ).time():
                     caikit_library_request = build_caikit_library_request_dict(
-                        request, model.run
+                        request,
+                        model_class.RUN_SIGNATURE,
                     )
 
                 # NB: we previously recorded the size of the request, and timed this module to
                 # provide a rudimentary throughput metric of size / time
                 with alog.ContextLog(log.debug, inner_scope_name):
                     with PREDICT_CAIKIT_LIBRARY_SUMMARY.labels(
                         grpc_request=desc_name, model_id=model_id
@@ -229,7 +236,31 @@
             log.warning(log_dict)
             PREDICT_RPC_COUNTER.labels(
                 grpc_request=desc_name, code=StatusCode.INTERNAL.name, model_id=model_id
             ).inc()
             raise CaikitRuntimeException(
                 StatusCode.INTERNAL, "Unhandled exception during prediction"
             ) from e
+
+    def _verify_model_task(self, model: ModuleBase, request_name: str):
+        """Raise if the model is not supported for the task"""
+        rpc_set: Set[TaskPredictRPC] = self._inference_service.caikit_rpcs
+        module_rpc: TaskPredictRPC = next(
+            (rpc for rpc in rpc_set if model.TASK_CLASS == rpc.task),
+            None,
+        )
+
+        if not module_rpc:
+            raise CaikitRuntimeException(
+                status_code=StatusCode.INVALID_ARGUMENT,
+                message=f"Inference for model class {type(model)} not supported by this runtime",
+            )
+
+        request_rpc: TaskPredictRPC = next(
+            (rpc for rpc in rpc_set if rpc.request.name == request_name), None
+        )
+        if request_rpc != module_rpc:
+            raise CaikitRuntimeException(
+                status_code=StatusCode.INVALID_ARGUMENT,
+                message=f"Wrong inference RPC invoked for model class {type(model)}. "
+                f"Use {request_rpc.name} instead of {request_name}",
+            )
```

### Comparing `caikit-0.7.0/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.7.1/caikit/runtime/servicers/global_train_servicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         model_name = request.model_name
         model_path = self._get_model_path(training_output_dir, model_name, training_id)
 
         # Build the full set of kwargs for the train and save call
         kwargs = {
             "module_class": model,
             "model_path": model_path,
-            **build_caikit_library_request_dict(request, model.train),
+            **build_caikit_library_request_dict(request, model.TRAIN_SIGNATURE),
         }
 
         # If running with a subprocess, set the target, events and args accordingly
         if self.use_subprocess:
             cancel_event = multiprocessing.Event()
             target = SubProcessTrainSaveExecutor(cancel_event)
         else:
```

### Comparing `caikit-0.7.0/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.7.1/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.7.1/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.7.1/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/types/__init__.py` & `caikit-0.7.1/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/types/aborted_exception.py` & `caikit-0.7.1/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.7.1/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.7.1/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/utils/__init__.py` & `caikit-0.7.1/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/utils/import_util.py` & `caikit-0.7.1/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/work_management/__init__.py` & `caikit-0.7.1/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/work_management/abortable_action.py` & `caikit-0.7.1/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/work_management/call_aborter.py` & `caikit-0.7.1/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.7.1/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/caikit/runtime/work_management/train_executors.py` & `caikit-0.7.1/caikit/runtime/work_management/train_executors.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
+from concurrent.futures.thread import _threads_queues
 from typing import Type
 import abc
 import multiprocessing
 import os
 import threading
 import traceback
 
@@ -34,14 +35,24 @@
 
 log = alog.use_channel("TRN_EXCTRS")
 error = caikit.core.toolkit.errors.error_handler.get(log)
 
 
 OOM_EXIT_CODE = 137
 
+
+# 🌶️🌶️🌶️
+# Fix for python3.9, 3.10 and 3.11 issue where forked processes always exit with exitcode 1
+# when it's created inside a ThreadPoolExecutor: https://github.com/python/cpython/issues/88110
+# Fix taken from https://github.com/python/cpython/pull/101940
+# Credit: marmarek, https://github.com/marmarek
+
+if hasattr(os, "register_at_fork"):
+    os.register_at_fork(after_in_child=_threads_queues.clear)
+
 # NOTE: Following would get replaced with training backends potentially
 # in future.
 # NOTE: Instead of using executors like Local / Subprocess
 # it might make sense to instead use concurrent.Future based
 # executors, so ThreadPoolExecutors and ProcessPoolExecutors, but
 # ProcessPoolExecutor doesn't support `fork` start method
 class TrainSaveExecutorBase(abc.ABC):
@@ -86,21 +97,14 @@
         self.events = [cancel_event, self.complete_event]
 
         # NOTE: worker is assigned at a later stage for Local
         self._worker = None
 
         self.__cancel_event = cancel_event
 
-    def __del__(self):
-        """
-        NOTE: This is NOT how execution should be cancelled.
-        This function is designed to make sure cleanup happens.
-        """
-        self.cancel()
-
     # pylint: disable=arguments-differ
     def train_and_save_model(
         self,
         module_class: Type[ModuleBase],
         model_path: str,
         *args,
         **kwargs,
@@ -202,14 +206,15 @@
             try:
                 return super().run(*args, **kwargs)
 
             # Catch any errors thrown within a subprocess so that they can be
             # forwarded to the parent
             # pylint: disable=broad-exception-caught
             except Exception as err:
+                log.error("<RUN69863806E>", "Caught exception in training", repr(err))
                 self.error = err
 
             finally:
                 self._completion_event.set()
 
     def __init__(self, cancel_event) -> None:
 
@@ -224,31 +229,31 @@
         NOTE: This is NOT how execution should be cancelled.
         This function is designed to make sure cleanup happens.
         """
         self._cleanup()
 
     def _cleanup(self):
         """Function to clearup running workers"""
-        if self._worker.is_alive():
+        if self._worker._check_closed():
             self._worker.terminate()
-        self._worker.close()
+            self._worker.close()
 
     # pylint: disable=arguments-differ
     def train_and_save_model(
         self, module_class: Type[ModuleBase], model_path: str, *args, **kwargs
     ):
 
         self._worker = self._ErrorCaptureProcess(
             event=self.complete_event,
             target=TrainSaveExecutorBase._train_and_save,
             args=(module_class, model_path),
             kwargs=kwargs,
         )
 
-        def exit_code_handler():
+        def cancel_event_handler():
             """Function to wait for completion_event and fire up
             cancellation (termination of subprocess) in case
             cancel_event is triggered
             """
             self.complete_event.wait()
 
             if self.__cancel_event.is_set():
@@ -261,15 +266,15 @@
                 # but in that case, the training is anyways already finished
                 # so that shouldn't create huge problems
                 self.cancel()
 
         # Create a cancel thread which will be in "parallel" waiting for
         # complete_event and will target cancellation of worker, in case
         # cancellation event is set
-        cancellation_thread = threading.Thread(target=exit_code_handler)
+        cancellation_thread = threading.Thread(target=cancel_event_handler)
 
         # NOTE: Below order is crucial
         self._worker.start()
         cancellation_thread.start()
 
         # Wait for worker to finish
         # In case of cancellation, the worker will get terminated
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `caikit-0.7.0/docs/Makefile` & `caikit-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/docs/adrs/010-data-model-definition.md` & `caikit-0.7.1/docs/adrs/010-data-model-definition.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/docs/adrs/015-runtime-service-generation.md` & `caikit-0.7.1/docs/adrs/015-runtime-service-generation.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/docs/adrs/018-shared-backends.md` & `caikit-0.7.1/docs/adrs/018-shared-backends.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/docs/adrs/019-loader-stack.md` & `caikit-0.7.1/docs/adrs/019-loader-stack.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/docs/architecture_club/04-25-23.md` & `caikit-0.7.1/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/docs/make.bat` & `caikit-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/docs/source/conf.py` & `caikit-0.7.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/examples/start_runtime_with_sample_lib.py` & `caikit-0.7.1/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/examples/text-sentiment/README.md` & `caikit-0.7.1/examples/text-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/examples/text-sentiment/client.py` & `caikit-0.7.1/examples/text-sentiment/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,13 +28,15 @@
 
 client_stub = inference_service.stub_class(channel)
 
 # print(dir(client_stub))
 
 for text in ["I am not feeling well today!", "Today is a nice sunny day"]:
     input_text_proto = TextInput(text=text).to_proto()
-    request = inference_service.messages.HfModuleRequest(text_input=input_text_proto)
-    response = client_stub.HfModulePredict(
+    request = inference_service.messages.HuggingFaceSentimentTaskRequest(
+        text_input=input_text_proto
+    )
+    response = client_stub.HuggingFaceSentimentTaskPredict(
         request, metadata=[("mm-model-id", "text_sentiment")]
     )
     print("Text:", text)
     print("RESPONSE:", response)
```

### Comparing `caikit-0.7.0/examples/text-sentiment/models/text_sentiment/config.yml` & `caikit-0.7.1/examples/text-sentiment/models/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/examples/text-sentiment/start_runtime.py` & `caikit-0.7.1/examples/text-sentiment/start_runtime.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/examples/text-sentiment/text_sentiment/__init__.py` & `caikit-0.7.1/examples/text-sentiment/text_sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/examples/text-sentiment/text_sentiment/config.yml` & `caikit-0.7.1/examples/text-sentiment/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/examples/text-sentiment/text_sentiment/data_model/__init__.py` & `caikit-0.7.1/examples/text-sentiment/text_sentiment/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/examples/text-sentiment/text_sentiment/data_model/classification.py` & `caikit-0.7.1/examples/text-sentiment/text_sentiment/data_model/classification.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py` & `caikit-0.7.1/examples/text-sentiment/text_sentiment/runtime_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py` & `caikit-0.7.1/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,36 @@
 # Standard
 import os
 
 # Third Party
 from transformers import pipeline
 
 # Local
-from caikit.core import ModuleBase, ModuleLoader, ModuleSaver, module
+from caikit.core import ModuleBase, ModuleLoader, ModuleSaver, TaskBase, module, task
 from text_sentiment.data_model.classification import (
     ClassificationPrediction,
     ClassInfo,
     TextInput,
 )
 
 
-@module("8f72161-c0e4-49b0-8fd0-7587b3017a35", "HuggingFaceSentimentModule", "0.0.1")
+@task(
+    required_parameters={"text_input": TextInput},
+    output_type=ClassificationPrediction,
+)
+class HuggingFaceSentimentTask(TaskBase):
+    pass
+
+
+@module(
+    "8f72161-c0e4-49b0-8fd0-7587b3017a35",
+    "HuggingFaceSentimentModule",
+    "0.0.1",
+    HuggingFaceSentimentTask,
+)
 class HuggingFaceSentimentModule(ModuleBase):
     """Class to wrap sentiment analysis pipeline from HuggingFace"""
 
     def __init__(self, model_path) -> None:
         super().__init__()
         loader = ModuleLoader(model_path)
         config = loader.config
```

### Comparing `caikit-0.7.0/pyproject.toml` & `caikit-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.7.0"
+version = "0.7.1"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `caikit-0.7.0/releases.md` & `caikit-0.7.1/releases.md`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/scripts/check_deps.sh` & `caikit-0.7.1/scripts/check_deps.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/scripts/fmt.sh` & `caikit-0.7.1/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/__init__.py` & `caikit-0.7.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/base.py` & `caikit-0.7.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/config/test_configs.py` & `caikit-0.7.1/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/conftest.py` & `caikit-0.7.1/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -163,26 +163,40 @@
 def train_stub(sample_train_service, runtime_grpc_server) -> Type:
     train_stub = sample_train_service.stub_class(
         runtime_grpc_server.make_local_channel()
     )
     return train_stub
 
 
+@pytest.fixture(scope="session")
+def training_management_stub(runtime_grpc_server) -> Type:
+    training_management_service: ServicePackage = (
+        ServicePackageFactory().get_service_package(
+            ServicePackageFactory.ServiceType.TRAINING_MANAGEMENT,
+        )
+    )
+
+    training_management_stub = training_management_service.stub_class(
+        runtime_grpc_server.make_local_channel()
+    )
+    return training_management_stub
+
+
 @pytest.fixture
 def good_model_path() -> str:
     return Fixtures.get_good_model_path()
 
 
 @pytest.fixture
 def other_good_model_path() -> str:
     return Fixtures.get_other_good_model_path()
 
 
 @pytest.fixture
-def loaded_model_id(good_model_path) -> str:
+def sample_task_model_id(good_model_path) -> str:
     """Loaded model ID using model manager load model implementation"""
     model_id = _random_id()
     model_manager = ModelManager.get_instance()
     # model load test already tests with archive - just using a model path here
     model_manager.load_model(
         model_id,
         local_model_path=good_model_path,
@@ -191,15 +205,15 @@
     yield model_id
 
     # teardown
     model_manager.unload_model(model_id)
 
 
 @pytest.fixture
-def other_loaded_model_id(other_good_model_path) -> str:
+def other_task_model_id(other_good_model_path) -> str:
     """Loaded model ID using model manager load model implementation"""
     model_id = _random_id()
     model_manager = ModelManager.get_instance()
     # model load test already tests with archive - just using a model path here
     model_manager.load_model(
         model_id,
         local_model_path=other_good_model_path,
```

### Comparing `caikit-0.7.0/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.7.1/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.7.1/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.7.1/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/data_model/streams/test_converter.py` & `caikit-0.7.1/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.7.1/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.7.1/tests/core/data_model/streams/test_data_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
+import json
 import os
+import pickle
 
 # Local
 from caikit.core import data_model as core_dm
 from caikit.core.augmentors import AugmentorBase
 from sample_lib.data_model.sample import SampleInputType, SampleOutputType
 from sample_lib.modules.sample_task.sample_implementation import SampleModule
 
@@ -49,14 +51,31 @@
             if not self.produces_none and obj == 13:
                 return None
             return obj + 5
 
     return TestStreamAugmentor()
 
 
+def test_data_stream_from_jsonl_is_pickleable(tmp_path):
+    tmpdir = str(tmp_path)
+
+    data = [1, 2, 3, 4, 5, 6]
+    filepath = os.path.join(tmpdir, "foo.jsonl")
+    with open(filepath, "w") as f:
+        json.dump(data, f)
+
+    stream = core_dm.DataStream.from_jsonl(filepath)
+
+    pre_pickle_vals = list(stream)
+    pickled_stream = pickle.loads(pickle.dumps(stream))
+    post_pickle_vals = list(pickled_stream)
+
+    assert pre_pickle_vals == post_pickle_vals
+
+
 class TestDataStream(TestCaseBase):
     def setUp(self):
         self.list_data_stream = core_dm.DataStream.from_iterable(
             ["hello", "world", "!"]
         )
 
         self.samples_path = os.path.join(self.fixtures_dir, "data_stream_inputs")
```

### Comparing `caikit-0.7.0/tests/core/data_model/streams/test_resolver.py` & `caikit-0.7.1/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/data_model/streams/test_validator.py` & `caikit-0.7.1/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/data_model/test_base.py` & `caikit-0.7.1/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/data_model/test_dataobject.py` & `caikit-0.7.1/tests/core/data_model/test_dataobject.py`

 * *Files 9% similar despite different names*

```diff
@@ -808,7 +808,71 @@
     assert set(foo_proto.js_dict.fields["foo"].struct_value.fields.keys()) == set(
         js_dict["foo"].keys()
     )
 
     # Make sure conversion back to dict happens on from_proto
     foo2 = Foo.from_proto(foo_proto)
     assert foo2.js_dict == foo.js_dict
+
+
+def test_dataobject_to_kwargs(temp_dpool):
+    """to_kwargs does a non-recursive version of to_dict"""
+
+    @dataobject
+    class Bar(DataObjectBase):
+        bar: int
+
+    @dataobject
+    class Foo(DataObjectBase):
+        int_val: int
+        type_union_val: Union[int, str]
+        bar_val: Bar
+
+    bar = Bar(bar=42)
+    foo = Foo(int_val=1, type_union_val="foo", bar_val=bar)
+
+    kwargs = foo.to_kwargs()
+
+    # `type_union_val` is set here rather than the `type_union_val_str_val` internal oneof field name
+    assert kwargs == {"int_val": 1, "type_union_val": "foo", "bar_val": bar}
+
+
+def test_dataobject_inheritance(temp_dpool):
+    """Make sure that dataobject classes can inherit from each other in the same
+    way that dataclasses can
+    """
+
+    @dataobject
+    class Base(DataObjectBase):
+        foo: int
+        bar: int
+
+    @dataobject
+    class Derived(Base):
+        bar: str
+        baz: str
+
+    # Validate Base
+    desc = Base.get_proto_class().DESCRIPTOR
+    fld = desc.fields_by_name["foo"]  # To save typing
+    assert "foo" in desc.fields_by_name
+    assert "bar" in desc.fields_by_name
+    assert "baz" not in desc.fields_by_name
+    assert desc.fields_by_name["foo"].type == fld.TYPE_INT64
+    assert desc.fields_by_name["bar"].type == fld.TYPE_INT64
+    inst = Derived(1, 2)
+    assert inst.foo == 1
+    assert inst.bar == 2
+
+    # Validate Derived
+    desc = Derived.get_proto_class().DESCRIPTOR
+    fld = desc.fields_by_name["foo"]  # To save typing
+    assert "foo" in desc.fields_by_name
+    assert "bar" in desc.fields_by_name
+    assert "baz" in desc.fields_by_name
+    assert desc.fields_by_name["foo"].type == fld.TYPE_INT64
+    assert desc.fields_by_name["bar"].type == fld.TYPE_STRING
+    assert desc.fields_by_name["baz"].type == fld.TYPE_STRING
+    inst = Derived(1, "asdf", "qwer")
+    assert inst.foo == 1
+    assert inst.bar == "asdf"
+    assert inst.baz == "qwer"
```

### Comparing `caikit-0.7.0/tests/core/data_model/test_enums.py` & `caikit-0.7.1/tests/core/data_model/test_enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/data_model/test_json_dict.py` & `caikit-0.7.1/tests/core/data_model/test_json_dict.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/data_model/test_producer.py` & `caikit-0.7.1/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/helpers.py` & `caikit-0.7.1/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/module_backends/test_backend_types.py` & `caikit-0.7.1/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/module_backends/test_module_backend_config.py` & `caikit-0.7.1/tests/core/module_backends/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/modules/test_module.py` & `caikit-0.7.1/tests/core/modules/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/modules/test_module_metadata.py` & `caikit-0.7.1/tests/core/modules/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/signature_parsing/__init__.py` & `caikit-0.7.1/tests/core/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/signature_parsing/test_docstrings.py` & `caikit-0.7.1/tests/core/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/signature_parsing/test_parsers.py` & `caikit-0.7.1/tests/core/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/test_imports.py` & `caikit-0.7.1/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/test_model_manager.py` & `caikit-0.7.1/tests/core/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/test_no_write_permissions.py` & `caikit-0.7.1/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/test_task.py` & `caikit-0.7.1/tests/core/test_task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/toolkit/test_compatibility.py` & `caikit-0.7.1/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/toolkit/test_error_handler.py` & `caikit-0.7.1/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/toolkit/test_fileio.py` & `caikit-0.7.1/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.7.1/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/toolkit/test_serializers.py` & `caikit-0.7.1/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.7.1/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/data_model_helpers.py` & `caikit-0.7.1/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/fixtures/config/config.yml` & `caikit-0.7.1/tests/fixtures/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.7.1/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/fixtures/dummy_module.zip` & `caikit-0.7.1/tests/fixtures/dummy_module.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/fixtures/dummy_module/config.yml` & `caikit-0.7.1/tests/fixtures/dummy_module/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/fixtures/dummy_module_singleton/config.yml` & `caikit-0.7.1/tests/fixtures/dummy_module_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/fixtures/fixtures.py` & `caikit-0.7.1/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/fixtures/invalid.zip` & `caikit-0.7.1/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/fixtures/linux.txt` & `caikit-0.7.1/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.7.1/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py` & `caikit-0.7.1/tests/fixtures/sample_lib/modules/other_task/other_implementation.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,10 +52,10 @@
         training_data: DataStream[int],
         sample_input: Union[SampleInputType, str],
         batch_size: int = 64,
     ) -> "OtherModule":
         """Sample training method that produces a trained model"""
         assert type(sample_input) == SampleInputType or str
         # Barf if we were incorrectly passed data not in datastream format
-        assert type(training_data) == DataStream
+        assert isinstance(training_data, DataStream)
         assert batch_size > 0
         return cls(batch_size=batch_size)
```

### Comparing `caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py` & `caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/composite_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py` & `caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/inner_module.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 """
 A hypothetical inner module that transforms some output type rather than taking domain input
 """
 # Local
 from ...data_model.sample import SampleOutputType
+from caikit.core import ModuleSaver
 import caikit.core
 
 
 @caikit.core.module("00110203-baad-beef-0809-0a0b02dd0e0f", "InnerModule", "0.0.1")
 class InnerModule(caikit.core.ModuleBase):
     def __init__(self, batch_size=64, learning_rate=0.0015):
         super().__init__()
         self.batch_size = batch_size
         self.learning_rate = learning_rate
 
     def run(self, some_input: SampleOutputType) -> SampleOutputType:
         return SampleOutputType(f"nested greeting: {some_input.greeting}")
+
+    def save(self, model_path):
+        module_saver = ModuleSaver(
+            self,
+            model_path=model_path,
+        )
+        with module_saver:
+            pass
+
+    @classmethod
+    def load(cls, model_path):
+        return cls()
```

### Comparing `caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py` & `caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py` & `caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     @classmethod
     def load(cls, model_path, **kwargs):
         return cls()
 
     def run(
         self,
         sample_input: SampleInputType,
-        bool_type: bool,
-        int_type: int,
-        float_type: float,
-        str_type: str,
-        bytes_type: bytes,
-        list_type: List[str],
+        bool_type: bool = True,
+        int_type: int = 42,
+        float_type: float = 34.0,
+        str_type: str = "moose",
+        bytes_type: bytes = b"",
+        list_type: List[str] = None,
     ) -> SampleOutputType:
         """This takes in a bunch of primitive types to ensure that we can pass those through the runtime server correctly."""
         assert isinstance(bool_type, bool)
         assert isinstance(int_type, int)
         assert isinstance(float_type, float)
         assert isinstance(str_type, str)
         assert isinstance(bytes_type, bytes)
```

### Comparing `caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py` & `caikit-0.7.1/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/generated/__init__.py` & `caikit-0.7.1/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/metrics/__init__.py` & `caikit-0.7.1/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.7.1/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/model_management/__init__.py` & `caikit-0.7.1/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/model_management/test_batcher.py` & `caikit-0.7.1/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/model_management/test_model_loader.py` & `caikit-0.7.1/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/model_management/test_model_manager.py` & `caikit-0.7.1/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.7.1/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/model_management/test_training_manager.py` & `caikit-0.7.1/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/service_generation/test_create_service.py` & `caikit-0.7.1/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.7.1/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 # Local
 from caikit.core.data_model import DataObjectBase, dataobject
 from caikit.core.data_model.streams.data_stream import DataStream
 from caikit.runtime.service_generation.data_stream_source import (
     DataStreamSourceBase,
     _make_data_stream_source_type_name,
-    get_data_stream_source,
     make_data_stream_source,
 )
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from sample_lib.data_model.sample import SampleTrainingType
 from tests.conftest import temp_config
 import caikit
 
@@ -130,22 +129,14 @@
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceInt
     ds = stream_type(jsondata=stream_type.JsonData(data=[1, 2, 3]))
     proto_repr = ds.to_proto()
     assert ds.from_proto(proto_repr).to_proto() == proto_repr
     assert stream_type.from_proto(proto_repr).to_proto() == proto_repr
 
 
-def test_get_data_stream_source(sample_train_service):
-    stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
-    ds = stream_type(jsondata=stream_type.JsonData(data=[SampleTrainingType(1)]))
-    # make sure you get the same type back after sending either as a protobuf message or normally
-    assert type(ds) is type(get_data_stream_source(ds.to_proto()))
-    assert type(ds) is type(get_data_stream_source(ds))
-
-
 def test_data_model_element_type(sample_train_service):
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     assert isinstance(stream_type._to_element_type({"number": 1}), SampleTrainingType)
 
 
 def test_primitive_element_type(sample_train_service):
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceInt
```

### Comparing `caikit-0.7.0/tests/runtime/service_generation/test_protoable.py` & `caikit-0.7.1/tests/runtime/service_generation/test_protoable.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/service_generation/test_rpcs.py` & `caikit-0.7.1/tests/runtime/service_generation/test_rpcs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.7.1/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/servicers/__init__.py` & `caikit-0.7.1/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.7.1/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,70 +42,70 @@
 import sample_lib
 
 HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
 HAPPY_PATH_RESPONSE = SampleOutputType(greeting="Hello Gabe").to_proto()
 
 
 def test_calling_predict_should_raise_if_module_raises(
-    sample_inference_service, sample_predict_servicer, loaded_model_id
+    sample_inference_service, sample_predict_servicer, sample_task_model_id
 ):
     with pytest.raises(CaikitRuntimeException) as context:
         # SampleModules will raise a RuntimeError if the throw flag is set
         request = sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT, throw=True
         )
         sample_predict_servicer.Predict(
-            request, Fixtures.build_context(loaded_model_id)
+            request, Fixtures.build_context(sample_task_model_id)
         )
     assert context.value.status_code == grpc.StatusCode.INTERNAL
     assert "Unhandled exception during prediction" in context.value.message
 
 
 def test_invalid_input_to_a_valid_caikit_core_class_method_raises(
-    loaded_model_id, sample_inference_service, sample_predict_servicer
+    sample_task_model_id, sample_inference_service, sample_predict_servicer
 ):
     """Test that a caikit.core module that gets an unexpected input value errors in an expected way"""
     with pytest.raises(CaikitRuntimeException) as context:
         # SampleModules will raise a ValueError if the poison pill name is given
         request = sample_inference_service.messages.SampleTaskRequest(
             sample_input=SampleInputType(name=SampleModule.POISON_PILL_NAME).to_proto(),
         )
         sample_predict_servicer.Predict(
-            request, Fixtures.build_context(loaded_model_id)
+            request, Fixtures.build_context(sample_task_model_id)
         )
     assert context.value.status_code == grpc.StatusCode.INVALID_ARGUMENT
     assert "problem with your input" in context.value.message
 
 
 def test_global_predict_works_on_good_inputs(
-    sample_inference_service, sample_predict_servicer, loaded_model_id
+    sample_inference_service, sample_predict_servicer, sample_task_model_id
 ):
-    """Global predict of CategoriesEsaPredict returns a categories prediction"""
+    """Global predict of SampleTaskRequest returns a prediction"""
     response = sample_predict_servicer.Predict(
         sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT
         ),
-        Fixtures.build_context(loaded_model_id),
+        Fixtures.build_context(sample_task_model_id),
     )
     assert response == HAPPY_PATH_RESPONSE
 
 
 def test_global_predict_aborts_long_running_predicts(
     sample_inference_service, sample_predict_servicer
 ):
     mock_manager = MagicMock()
 
     # return a dummy model from the mock model manager
-    class UnresponsiveModel:
+    class UnresponsiveModel(SampleModule):
         started = threading.Event()
 
         def run(self, *args, **kwargs):
             self.started.set()
             while True:
-                time.sleep(0.01)
+                time.sleep(0.001)
 
     dummy_model = UnresponsiveModel()
     mock_manager.retrieve_model.return_value = dummy_model
 
     context = Fixtures.build_context("test-any-unresponsive-model")
     predict_thread = threading.Thread(
         target=sample_predict_servicer.Predict,
@@ -117,54 +117,54 @@
         ),
     )
 
     with catch_threading_exception() as cm:
         # Patch in the mock manager and start the prediction
         with patch.object(sample_predict_servicer, "_model_manager", mock_manager):
             predict_thread.start()
-            dummy_model.started.wait()
+            assert dummy_model.started.wait(2)
             # Simulate a timeout or client abort
             context.cancel()
             predict_thread.join(10)
 
         # Make sure the prediction actually stopped
         assert not predict_thread.is_alive()
 
         # Make sure the correct exception was raised
         assert cm.exc_type == AbortedException
 
 
 def test_metering_ignore_unsuccessful_calls(
-    sample_inference_service, sample_predict_servicer, loaded_model_id
+    sample_inference_service, sample_predict_servicer, sample_task_model_id
 ):
     with patch.object(
         sample_predict_servicer.rpc_meter, "update_metrics"
     ) as mock_update_func:
         request = sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT, throw=True
         )
         with pytest.raises(CaikitRuntimeException):
             sample_predict_servicer.Predict(
-                request, Fixtures.build_context(loaded_model_id)
+                request, Fixtures.build_context(sample_task_model_id)
             )
 
         mock_update_func.assert_not_called()
 
 
-def test_metering_predict_rpc_counter(sample_inference_service, loaded_model_id):
+def test_metering_predict_rpc_counter(sample_inference_service, sample_task_model_id):
     # need a new servicer to get a fresh new RPC meter
     sample_predict_servicer = GlobalPredictServicer(sample_inference_service)
     try:
         # Making 20 requests
         for i in range(20):
             sample_predict_servicer.Predict(
                 sample_inference_service.messages.SampleTaskRequest(
                     sample_input=HAPPY_PATH_INPUT
                 ),
-                Fixtures.build_context(loaded_model_id),
+                Fixtures.build_context(sample_task_model_id),
             )
 
         # Force meter to write
         sample_predict_servicer.rpc_meter.flush_metrics()
 
         # Assertions on the created metrics file
         with open(sample_predict_servicer.rpc_meter.file_path) as f:
@@ -183,35 +183,35 @@
             "<class 'sample_lib.modules.sample_task.sample_implementation.SampleModule'>": 20
         }
     finally:
         sample_predict_servicer.rpc_meter.end_writer_thread()
 
 
 def test_metering_write_to_metrics_file_twice(
-    sample_inference_service, loaded_model_id
+    sample_inference_service, sample_task_model_id
 ):
     """Make sure subsequent metering events append to file"""
     # need a new servicer to get a fresh new RPC meter
     sample_predict_servicer = GlobalPredictServicer(sample_inference_service)
     try:
         sample_predict_servicer.Predict(
             sample_inference_service.messages.SampleTaskRequest(
                 sample_input=HAPPY_PATH_INPUT
             ),
-            Fixtures.build_context(loaded_model_id),
+            Fixtures.build_context(sample_task_model_id),
         )
 
         # Force write
         sample_predict_servicer.rpc_meter.flush_metrics()
 
         sample_predict_servicer.Predict(
             sample_inference_service.messages.SampleTaskRequest(
                 sample_input=HAPPY_PATH_INPUT
             ),
-            Fixtures.build_context(loaded_model_id),
+            Fixtures.build_context(sample_task_model_id),
         )
 
         # Force write
         sample_predict_servicer.rpc_meter.flush_metrics()
 
         with open(sample_predict_servicer.rpc_meter.file_path) as f:
             data = [json.loads(line) for line in f]
```

### Comparing `caikit-0.7.0/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.7.1/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,35 +35,14 @@
 from tests.conftest import random_test_id, temp_config
 from tests.fixtures import Fixtures
 import caikit.core
 
 ## Helpers #####################################################################
 
 
-def _primitives_function(
-    self,
-    double_field,
-    float_field,
-    int64_field,
-    uint64_field,
-    int32_field,
-    fixed64_field,
-    fixed32_field,
-    bool_field,
-    string_field,
-    bytes_field,
-    uint32_field,
-    sfixed32_field,
-    sfixed64_field,
-    sint32_field,
-    sint64_field,
-):
-    pass
-
-
 @pytest.fixture(autouse=True, params=[True, False])
 def set_train_location(request):
     """This fixture ensures that all tests in this file will be run with both
     subprocess and local training styles
     """
     with temp_config({"training": {"use_subprocess": request.param}}):
         yield
@@ -109,18 +88,14 @@
     ).result()
     assert result.batch_size == 42
     assert (
         result.MODULE_CLASS
         == "sample_lib.modules.sample_task.sample_implementation.SampleModule"
     )
 
-    # give the trained model time to load
-    # TODO: no sleeps in tests!
-    time.sleep(1)
-
     inference_response = sample_predict_servicer.Predict(
         sample_inference_service.messages.SampleTaskRequest(
             sample_input=SampleInputType(name="Gabe").to_proto()
         ),
         Fixtures.build_context(training_response.model_name),
     )
     assert (
@@ -167,18 +142,14 @@
     ).result()
     assert result.batch_size == batch_size
     assert (
         result.MODULE_CLASS
         == "sample_lib.modules.other_task.other_implementation.OtherModule"
     )
 
-    # give the trained model time to load
-    # TODO: no sleeps in tests!
-    time.sleep(1)
-
     inference_response = sample_predict_servicer.Predict(
         sample_inference_service.messages.OtherTaskRequest(
             sample_inputsampleinputtype=SampleInputType(name="Gabe").to_proto()
         ),
         Fixtures.build_context(training_response.model_name),
     )
     assert (
@@ -186,23 +157,23 @@
         == OtherOutputType(
             farewell=f"goodbye: Gabe {batch_size} times",
         ).to_proto()
     )
 
 
 def test_global_train_Another_Widget_that_requires_SampleWidget_loaded_should_not_raise(
-    loaded_model_id,
+    sample_task_model_id,
     sample_train_service,
     sample_train_servicer,
     sample_inference_service,
     sample_predict_servicer,
 ):
     """Global train of TrainRequest returns a training job with the correct model name, and some training id for a train function that requires another loaded model"""
     sample_model = caikit.interfaces.runtime.data_model.ModelPointer(
-        model_id=loaded_model_id
+        model_id=sample_task_model_id
     ).to_proto()
 
     training_request = (
         sample_train_service.messages.SampleTaskCompositeModuleTrainRequest(
             model_name="AnotherWidget_Training",
             sample_block=sample_model,
         )
@@ -221,18 +192,14 @@
     ).result()
 
     assert (
         training_result.MODULE_CLASS
         == "sample_lib.modules.sample_task.composite_module.CompositeModule"
     )
 
-    # give the trained model time to load
-    # TODO: no sleeps in tests!
-    time.sleep(1)
-
     # make sure the trained model can run inference
     inference_response = sample_predict_servicer.Predict(
         sample_inference_service.messages.SampleTaskRequest(
             sample_input=SampleInputType(name="Gabe").to_proto()
         ),
         Fixtures.build_context(training_response.model_name),
     )
@@ -417,14 +384,17 @@
 
     assert f"Training process died with OOM error!" in str(context.value.message)
 
 
 #####################################################################
 
 
+@pytest.mark.skip(
+    reason="This test fails intermittently. Functionality has to be debugged for race condition"
+)
 def test_global_train_aborts_long_running_trains(
     sample_train_service, sample_train_servicer
 ):
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
@@ -450,17 +420,15 @@
             time.sleep(0.01)
 
     context = Fixtures.build_context("test-any-unresponsive-model")
 
     servicer = GlobalTrainServicer(training_service=sample_train_service)
 
     with TemporaryDirectory() as tmp_dir:
-        training_id = "dummy-training-id"
         training_output_dir = tmp_dir
-        context = Fixtures.build_context("foo")
 
         train_thread = threading.Thread(
             target=servicer.run_training_job,
             args=(
                 train_request,
                 SampleModule,
                 training_id,
@@ -470,23 +438,24 @@
             kwargs={
                 "wait": True,
             },
         )
 
     # NOTE: We are configuring following timeout
     # to avoid tests from hanging
-    request_timeout = 10
-    test_event_timeout = 20
+    request_timeout = 4
+    test_event_timeout = 2
     with patch(
         f"{SampleModule.__module__}.{SampleModule.train.__qualname__}",
         never_respond,
     ):
 
         train_thread.start()
-        test_event.wait(test_event_timeout)
+        # NB: assert is here to make sure we called the patched train
+        assert test_event.wait(test_event_timeout)
 
         # Simulate a timeout or client abort
         context.cancel()
         train_thread.join(request_timeout)
 
     # Make sure the training job actually stopped
     assert not train_thread.is_alive()
```

### Comparing `caikit-0.7.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.7.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.7.1/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.7.1/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/test_grpc_server.py` & `caikit-0.7.1/tests/runtime/test_grpc_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from caikit.runtime.protobufs import (
     model_runtime_pb2,
     model_runtime_pb2_grpc,
     process_pb2,
     process_pb2_grpc,
 )
 from caikit.runtime.service_factory import ServicePackage, ServicePackageFactory
+from sample_lib import InnerModule
 from sample_lib.data_model import (
     OtherOutputType,
     SampleInputType,
     SampleOutputType,
     SampleTrainingType,
 )
 from tests.conftest import random_test_id, runtime_grpc_test_server, temp_config
@@ -74,20 +75,42 @@
 HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
 HAPPY_PATH_RESPONSE = SampleOutputType(greeting="Hello Gabe").to_proto()
 HAPPY_PATH_TRAIN_RESPONSE = TrainingJob(
     model_name="dummy name", training_id="dummy id"
 ).to_proto()
 
 
-def is_good_train_response(actual_response, expected, model_name):
+def is_good_train_response(
+    actual_response, expected, model_name, training_management_stub
+):
     assert dir(actual_response) == dir(expected)
     assert actual_response.training_id is not None
     assert isinstance(actual_response.training_id, str)
     assert actual_response.model_name == model_name
 
+    status = TrainingStatus.PROCESSING.value
+    i = 0
+    while status == TrainingStatus.PROCESSING.value:
+        training_info_request = TrainingInfoRequest(
+            training_id=actual_response.training_id
+        )
+        training_management_response: TrainingInfoResponse = (
+            TrainingInfoResponse.from_proto(
+                training_management_stub.GetTrainingStatus(
+                    training_info_request.to_proto()
+                )
+            )
+        )
+        status = training_management_response.status
+        assert status != TrainingStatus.FAILED.value
+        i += 1
+        assert i < 100, "Waited too long for training to complete"
+
+    assert status == TrainingStatus.COMPLETED.value
+
 
 ## Tests #######################################################################
 
 
 def test_model_train(runtime_grpc_server):
     """Test model train's RUN function"""
     model_train_stub = process_pb2_grpc.ProcessStub(
@@ -156,23 +179,23 @@
     )
     # Fields with defaults have expected values
     assert result.batch_size == 64
     assert result.learning_rate == 0.0015
 
 
 def test_predict_fake_module_ok_response(
-    loaded_model_id, runtime_grpc_server, sample_inference_service
+    sample_task_model_id, runtime_grpc_server, sample_inference_service
 ):
     """Test RPC CaikitRuntime.WidgetPredict successful response"""
     stub = sample_inference_service.stub_class(runtime_grpc_server.make_local_channel())
     predict_request = sample_inference_service.messages.SampleTaskRequest(
         sample_input=HAPPY_PATH_INPUT
     )
     actual_response = stub.SampleTaskPredict(
-        predict_request, metadata=[("mm-model-id", loaded_model_id)]
+        predict_request, metadata=[("mm-model-id", sample_task_model_id)]
     )
     assert actual_response == HAPPY_PATH_RESPONSE
 
 
 def test_predict_fake_module_error_response(
     runtime_grpc_server, sample_inference_service
 ):
@@ -186,20 +209,70 @@
         )
         stub.SampleTaskPredict(
             predict_request, metadata=[("mm-model-id", "random_model_id")]
         )
     assert context.value.code() == grpc.StatusCode.NOT_FOUND
 
 
+def test_rpc_validation_on_predict(
+    sample_task_model_id, runtime_grpc_server, sample_inference_service
+):
+    """Check that the server catches models sent to the wrong task RPCs"""
+    stub = sample_inference_service.stub_class(runtime_grpc_server.make_local_channel())
+    predict_request = sample_inference_service.messages.OtherTaskRequest(
+        sample_inputsampleinputtype=HAPPY_PATH_INPUT
+    )
+    with pytest.raises(grpc.RpcError) as context:
+        stub.OtherTaskPredict(
+            predict_request, metadata=[("mm-model-id", sample_task_model_id)]
+        )
+    assert context.value.code() == grpc.StatusCode.INVALID_ARGUMENT
+    assert "Wrong inference RPC invoked for model class" in str(context.value)
+
+
+def test_rpc_validation_on_predict_for_unsupported_model(
+    runtime_grpc_server: RuntimeGRPCServer, sample_inference_service, tmp_path
+):
+    """Check that the server catches models that have no supported inference rpc"""
+    unsupported_model = InnerModule()
+    tmpdir = str(tmp_path)
+    unsupported_model.save(tmpdir)
+    model_id = random_test_id()
+    try:
+        runtime_grpc_server._global_predict_servicer._model_manager.load_model(
+            model_id, tmpdir, "foo"
+        )
+
+        stub = sample_inference_service.stub_class(
+            runtime_grpc_server.make_local_channel()
+        )
+        predict_request = sample_inference_service.messages.SampleTaskRequest(
+            sample_input=HAPPY_PATH_INPUT
+        )
+        with pytest.raises(grpc.RpcError) as context:
+            stub.SampleTaskPredict(
+                predict_request, metadata=[("mm-model-id", model_id)]
+            )
+        assert context.value.code() == grpc.StatusCode.INVALID_ARGUMENT
+        assert "Inference for model class" in str(context.value)
+        assert "not supported by this runtime" in str(context.value)
+
+    finally:
+        runtime_grpc_server._global_predict_servicer._model_manager.unload_model(
+            model_id
+        )
+
+
 ####### End-to-end tests for train a model and then predict with it
 def test_train_fake_module_ok_response_and_can_predict_with_trained_model(
     train_stub,
     inference_stub,
     sample_train_service,
     sample_inference_service,
+    training_management_stub,
 ):
     """Test RPC CaikitRuntime.SampleTaskSampleModuleTrain successful response"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(
             data=[SampleTrainingType(1), SampleTrainingType(2)]
         )
@@ -208,72 +281,71 @@
     train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
         model_name=model_name,
         training_data=training_data,
     )
 
     actual_response = train_stub.SampleTaskSampleModuleTrain(train_request)
 
-    is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name)
-
-    # give the trained model time to load
-    # TODO: no sleeps in tests!
-    time.sleep(1)
+    is_good_train_response(
+        actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name, training_management_stub
+    )
 
     # make sure the trained model can run inference
     predict_request = sample_inference_service.messages.SampleTaskRequest(
         sample_input=HAPPY_PATH_INPUT
     )
     inference_response = inference_stub.SampleTaskPredict(
         predict_request, metadata=[("mm-model-id", actual_response.model_name)]
     )
     assert inference_response == HAPPY_PATH_RESPONSE
 
 
 def test_train_fake_module_ok_response_with_loaded_model_can_predict_with_trained_model(
-    loaded_model_id,
+    sample_task_model_id,
     train_stub,
     inference_stub,
     sample_train_service,
     sample_inference_service,
+    training_management_stub,
 ):
     """Test RPC CaikitRuntime.WorkflowsSampleTaskSampleWorkflowTrain successful response with a loaded model"""
     sample_model = caikit.interfaces.runtime.data_model.ModelPointer(
-        model_id=loaded_model_id
+        model_id=sample_task_model_id
     ).to_proto()
     model_name = random_test_id()
     train_request = sample_train_service.messages.SampleTaskCompositeModuleTrainRequest(
         model_name=model_name, sample_block=sample_model
     )
     actual_response = train_stub.SampleTaskCompositeModuleTrain(train_request)
-    is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name)
-
-    # give the trained model time to load
-    # TODO: no sleeps in tests!
-    time.sleep(1)
+    is_good_train_response(
+        actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name, training_management_stub
+    )
 
     # make sure the trained model can run inference
     predict_request = sample_inference_service.messages.SampleTaskRequest(
         sample_input=HAPPY_PATH_INPUT
     )
     inference_response = inference_stub.SampleTaskPredict(
         predict_request, metadata=[("mm-model-id", actual_response.model_name)]
     )
     assert inference_response == HAPPY_PATH_RESPONSE
 
 
 def test_train_fake_module_does_not_change_another_instance_model_of_block(
-    other_loaded_model_id,
+    other_task_model_id,
     sample_int_file,
     train_stub,
     inference_stub,
+    training_management_stub,
     sample_train_service,
     sample_inference_service,
 ):
-    """This test: original "stock" OtherModule model has batch size 42 (see fixtures/models/bar.yml),
-    we then train a custom OtherModule model with batch size 100,
+    """This test: original "stock" OtherModule model has batch size 42
+    (See fixtures/models/bar/config.yml).
+    We then train a custom OtherModule model with batch size 100,
     then we make a predict to each, they should have the correct batch size"""
 
     # Train an OtherModule with batch size 100
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceInt
     training_data = stream_type(
         file=stream_type.File(filename=sample_int_file)
     ).to_proto()
@@ -281,19 +353,20 @@
     train_request = sample_train_service.messages.OtherTaskOtherModuleTrainRequest(
         model_name="Bar Training",
         sample_inputsampleinputtype=SampleInputType(name="Gabe").to_proto(),
         batch_size=100,
         training_data=training_data,
     )
     actual_response = train_stub.OtherTaskOtherModuleTrain(train_request)
-    is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, "Bar Training")
-
-    # give the trained model time to load
-    # TODO: no sleeps in tests!
-    time.sleep(1)
+    is_good_train_response(
+        actual_response,
+        HAPPY_PATH_TRAIN_RESPONSE,
+        "Bar Training",
+        training_management_stub,
+    )
 
     # make sure the trained model can run inference, and the batch size 100 was used
     predict_request = sample_inference_service.messages.OtherTaskRequest(
         sample_inputsampleinputtype=HAPPY_PATH_INPUT
     )
     trained_inference_response = inference_stub.OtherTaskPredict(
         predict_request, metadata=[("mm-model-id", actual_response.model_name)]
@@ -301,25 +374,29 @@
     expected_trained_inference_response = OtherOutputType(
         farewell="goodbye: Gabe 100 times"
     ).to_proto()
     assert trained_inference_response == expected_trained_inference_response
 
     # make sure the previously loaded OtherModule model still has batch size 42
     original_inference_response = inference_stub.OtherTaskPredict(
-        predict_request, metadata=[("mm-model-id", other_loaded_model_id)]
+        predict_request, metadata=[("mm-model-id", other_task_model_id)]
     )
     expected_original_inference_response = OtherOutputType(
         farewell="goodbye: Gabe 42 times"
     ).to_proto()
     assert original_inference_response == expected_original_inference_response
 
 
 ##### Test different datastream types #####
 def test_train_fake_module_ok_response_with_datastream_jsondata(
-    train_stub, inference_stub, sample_train_service, sample_inference_service
+    train_stub,
+    inference_stub,
+    sample_train_service,
+    sample_inference_service,
+    training_management_stub,
 ):
     """Test RPC CaikitRuntime.SampleTaskSampleModuleTrainRequest successful response with training data json type"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(
             data=[SampleTrainingType(1), SampleTrainingType(2)]
         )
@@ -328,19 +405,17 @@
     train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
         model_name=model_name,
         batch_size=42,
         training_data=training_data,
     )
 
     actual_response = train_stub.SampleTaskSampleModuleTrain(train_request)
-    is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name)
-
-    # give the trained model time to load
-    # TODO: no sleeps in tests!
-    time.sleep(1)
+    is_good_train_response(
+        actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name, training_management_stub
+    )
 
     # make sure the trained model can run inference
     predict_request = sample_inference_service.messages.SampleTaskRequest(
         sample_input=HAPPY_PATH_INPUT
     )
     inference_response = inference_stub.SampleTaskPredict(
         predict_request, metadata=[("mm-model-id", actual_response.model_name)]
@@ -350,32 +425,31 @@
 
 def test_train_fake_module_ok_response_with_datastream_csv_file(
     train_stub,
     inference_stub,
     sample_train_service,
     sample_inference_service,
     sample_csv_file,
+    training_management_stub,
 ):
     """Test RPC CaikitRuntime.SampleTaskSampleModuleTrainRequest successful response with training data file type"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         file=stream_type.File(filename=sample_csv_file)
     ).to_proto()
     model_name = random_test_id()
     train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
         model_name=model_name,
         training_data=training_data,
     )
 
     actual_response = train_stub.SampleTaskSampleModuleTrain(train_request)
-    is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name)
-
-    # give the trained model time to load
-    # TODO: no sleeps in tests!
-    time.sleep(1)
+    is_good_train_response(
+        actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name, training_management_stub
+    )
 
     # make sure the trained model can run inference
     predict_request = sample_inference_service.messages.SampleTaskRequest(
         sample_input=HAPPY_PATH_INPUT
     )
     inference_response = inference_stub.SampleTaskPredict(
         predict_request, metadata=[("mm-model-id", actual_response.model_name)]
@@ -446,20 +520,22 @@
             modelPath=Fixtures.get_bad_model_archive_path(),
             modelKey="baz",
         )
         stub.loadModel(load_model_request)
     assert context.value.code() == grpc.StatusCode.INTERNAL
 
 
-def test_unload_model_ok_response(loaded_model_id, runtime_grpc_server):
+def test_unload_model_ok_response(sample_task_model_id, runtime_grpc_server):
     """Test unload model's successful response"""
     stub = model_runtime_pb2_grpc.ModelRuntimeStub(
         runtime_grpc_server.make_local_channel()
     )
-    unload_model_request = model_runtime_pb2.UnloadModelRequest(modelId=loaded_model_id)
+    unload_model_request = model_runtime_pb2.UnloadModelRequest(
+        modelId=sample_task_model_id
+    )
     # Unload model throws on failure (response message has no fields)
     stub.unloadModel(unload_model_request)
 
 
 def test_unload_model_does_not_throw_if_model_does_not_exist(runtime_grpc_server):
     """Unloading a model that does not exist (or has already been deleted) is totally cool"""
     try:
@@ -481,22 +557,22 @@
         modelId="foo", modelType="bar", modelPath=Fixtures.get_good_model_path()
     )
     actual_response = stub.predictModelSize(predict_model_size_request)
     assert 0 < actual_response.sizeInBytes
 
 
 def test_predict_model_size_on_loaded_model_ok_response(
-    loaded_model_id, runtime_grpc_server
+    sample_task_model_id, runtime_grpc_server
 ):
     """Test predict model size successful response on a model that has been loaded"""
     stub = model_runtime_pb2_grpc.ModelRuntimeStub(
         runtime_grpc_server.make_local_channel()
     )
     predict_model_size_request = model_runtime_pb2.PredictModelSizeRequest(
-        modelId=loaded_model_id, modelPath=Fixtures.get_good_model_path()
+        modelId=sample_task_model_id, modelPath=Fixtures.get_good_model_path()
     )
     actual_response = stub.predictModelSize(predict_model_size_request)
     assert 0 < actual_response.sizeInBytes
 
 
 def test_predict_model_size_model_notfound_error_response(runtime_grpc_server):
     """Test predict model size with unknown model path error response"""
@@ -507,21 +583,23 @@
         predict_model_size_request = model_runtime_pb2.PredictModelSizeRequest(
             modelId=str(uuid.uuid4()), modelPath="/test/Does/Not/Exist"
         )
         stub.predictModelSize(predict_model_size_request)
     assert context.value.code() == grpc.StatusCode.NOT_FOUND
 
 
-def test_model_size_ok_response(loaded_model_id, runtime_grpc_server):
+def test_model_size_ok_response(sample_task_model_id, runtime_grpc_server):
     """Test model size successful response"""
     stub = model_runtime_pb2_grpc.ModelRuntimeStub(
         runtime_grpc_server.make_local_channel()
     )
 
-    model_size_request = model_runtime_pb2.ModelSizeRequest(modelId=loaded_model_id)
+    model_size_request = model_runtime_pb2.ModelSizeRequest(
+        modelId=sample_task_model_id
+    )
     actual_response = stub.modelSize(model_size_request)
     # Mar. 14, 23
     # The size of the directory pointed to by Fixtures.get_good_model_path() is 355 now.
     expected_size = (
         355
         * get_config().inference_plugin.model_mesh.model_size_multipliers[
             Fixtures.get_good_model_type()
@@ -702,28 +780,28 @@
         client_key, client_cert = tls_test_tools.generate_derived_key_cert_pair(ca_key)
         _assert_connection(
             _make_secure_channel(server, ca_cert, client_key, client_cert)
         )
 
 
 def test_metrics_stored_after_server_interrupt(
-    loaded_model_id, sample_inference_service
+    sample_task_model_id, sample_inference_service
 ):
     """This tests the gRPC server's behaviour when interrupted"""
 
     with runtime_grpc_test_server(
         inference_service=sample_inference_service,
         training_service=None,
     ) as server:
         stub = sample_inference_service.stub_class(server.make_local_channel())
         predict_request = sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT
         )
         _ = stub.SampleTaskPredict(
-            predict_request, metadata=[("mm-model-id", loaded_model_id)]
+            predict_request, metadata=[("mm-model-id", sample_task_model_id)]
         )
 
         # Interrupt server
         server.interrupt(None, None)
 
         # Assertions on the created metrics file
         with open(server._global_predict_servicer.rpc_meter.file_path) as f:
```

### Comparing `caikit-0.7.0/tests/runtime/test_service_factory.py` & `caikit-0.7.1/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/utils/__init__.py` & `caikit-0.7.1/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/utils/test_import_util.py` & `caikit-0.7.1/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/utils/test_servicer_util.py` & `caikit-0.7.1/tests/runtime/utils/test_servicer_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
 import os
 import tempfile
-import uuid
 
 # Third Party
 import pytest
 
 # Local
 from caikit.runtime.protobufs import model_runtime_pb2
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
@@ -29,18 +28,18 @@
     build_proto_response,
     get_metadata,
     is_protobuf_primitive_field,
     validate_caikit_library_class_exists,
     validate_caikit_library_class_method_exists,
     validate_data_model,
 )
+from sample_lib import SamplePrimitiveModule
 from sample_lib.data_model import SampleInputType
 from tests.conftest import random_test_id
 from tests.fixtures import Fixtures
-from tests.fixtures.protobufs import primitive_party_pb2
 import caikit.core
 import caikit.interfaces
 import sample_lib
 
 
 # ---------------- Tests for validate_caikit_library_class_exists --------------------
 def test_servicer_util_validate_caikit_library_class_exists_returns_caikit_class():
@@ -116,26 +115,36 @@
             self.foo = foo
 
     with pytest.raises(CaikitRuntimeException):
         build_proto_response(FooResponse(foo="This is a foo response"))
 
 
 # ---------------- Tests for is_protobuf_primitive_field --------------------
-def test_servicer_util_is_protobuf_primitive_returns_true_for_primitive_types():
+def test_servicer_util_is_protobuf_primitive_returns_true_for_primitive_types(
+    sample_inference_service,
+):
     """Test that is_protobuf_primitive_field is True when considering primitive types"""
-    for primitive_field in primitive_party_pb2._OPTIONALPRIMITIVES.fields:
-        assert True == is_protobuf_primitive_field(primitive_field)
+    assert is_protobuf_primitive_field(
+        sample_inference_service.messages.SampleTaskRequest().DESCRIPTOR.fields_by_name[
+            "int_type"
+        ]
+    )
 
 
-def test_servicer_util_is_protobuf_primitive_returns_false_for_custom_types():
+def test_servicer_util_is_protobuf_primitive_returns_false_for_custom_types(
+    sample_inference_service,
+):
     """Test that is_protobuf_primitive_field is False when considering message and
     enum types. This is essential for handling Caikit library CDM objects, which are
     generally defined in terms of messages"""
-    for primitive_field in primitive_party_pb2._NONPRIMITIVES.fields:
-        assert False == (is_protobuf_primitive_field(primitive_field))
+    assert not is_protobuf_primitive_field(
+        sample_inference_service.messages.SampleTaskRequest().DESCRIPTOR.fields_by_name[
+            "sample_input"
+        ]
+    )
 
 
 def test_servicer_util_is_protobuf_primitive_returns_false_for_instance_not_in_FieldDescriptor():
     field = caikit.interfaces.runtime.data_model.ModelPointer
     assert False == (is_protobuf_primitive_field(field))
 
 
@@ -184,47 +193,26 @@
 def test_servicer_util_will_not_validate_arbitrary_service_descriptor():
     """Test that validate_data_model raises exception validating arbitrary ServiceDescriptor"""
     with pytest.raises(AttributeError):
         validate_data_model(model_runtime_pb2._MODELRUNTIME)
 
 
 # ---------------- Tests for build_caikit_library_request_dict --------------------
-def _primitives_function(
-    self,
-    double_field,
-    float_field,
-    int64_field,
-    uint64_field,
-    int32_field,
-    fixed64_field,
-    fixed32_field,
-    bool_field,
-    string_field,
-    bytes_field,
-    uint32_field,
-    sfixed32_field,
-    sfixed64_field,
-    sint32_field,
-    sint64_field,
-):
-    pass
-
-
 HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
 
 
 def test_global_predict_build_caikit_library_request_dict_creates_caikit_core_run_kwargs(
     sample_inference_service,
 ):
     """Test that build_caikit_library_request_dict creates module run kwargs from RPC msg"""
     request_dict = build_caikit_library_request_dict(
         sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT
         ),
-        sample_lib.modules.sample_task.SampleModule().run,
+        sample_lib.modules.sample_task.SampleModule.RUN_SIGNATURE,
     )
 
     # No self or "throw", throw was not set and the throw parameter contains a default value
     expected_arguments = {"sample_input"}
 
     assert expected_arguments == set(request_dict.keys())
     assert isinstance(request_dict["sample_input"], SampleInputType)
@@ -233,137 +221,72 @@
 def test_global_predict_build_caikit_library_request_dict_strips_invalid_run_kwargs_from_request(
     sample_inference_service,
 ):
     """Global predict build_caikit_library_request_dict strips invalid run kwargs from request"""
     # Sample module doesn't take the `int_type` or `bool_type` params
     request_dict = build_caikit_library_request_dict(
         sample_inference_service.messages.SampleTaskRequest(
-            sample_input=HAPPY_PATH_INPUT, int_type=5, bool_type=True
+            sample_input=HAPPY_PATH_INPUT,
+            int_type=5,
+            bool_type=True,
         ),
-        sample_lib.modules.sample_task.SampleModule().run,
+        sample_lib.modules.sample_task.SampleModule.RUN_SIGNATURE,
     )
 
     expected_arguments = {"sample_input"}
     assert expected_arguments == set(request_dict.keys())
     assert "int_type" not in request_dict.keys()
 
 
 def test_global_predict_build_caikit_library_request_dict_strips_empty_list_from_request(
     sample_inference_service,
 ):
     """Global predict build_caikit_library_request_dict strips empty list from request"""
     request_dict = build_caikit_library_request_dict(
         sample_inference_service.messages.SampleTaskRequest(int_type=5, list_type=[]),
-        sample_lib.modules.sample_task.SamplePrimitiveModule().run,
+        sample_lib.modules.sample_task.SamplePrimitiveModule.RUN_SIGNATURE,
     )
 
     assert "list_type" not in request_dict.keys()
     assert "int_type" in request_dict.keys()
 
 
-def test_global_predict_build_caikit_library_request_dict_works_for_non_optional_primitives():
-    """Global predict build_caikit_library_request_dict works for primitives"""
-    request = primitive_party_pb2.NonOptionalPrimitives(
-        bool_field=False,
-        int64_field=10,
-        float_field=0.0,
-        bytes_field=b"",  # only field that is not passed through here
-        string_field="not_empty",
-    )
-
-    request_dict = build_caikit_library_request_dict(request, _primitives_function)
-    # dict started with 15 keys (15 args)
-    # Since these are non-optional, any field that is not an iterable
-    # is passed through, any field that is an iterable (str or bytes)
-    # is passed through only if len(field_value) != 0
-    assert len(request_dict.keys()) == 14
-    assert request_dict["float_field"] == 0.0
-    assert request_dict["int64_field"] == 10
-    assert request_dict["bool_field"] == False
-    assert "string_field" in request_dict
-    # TODO: Make sure to double check this later
-    assert "bytes_field" not in request_dict
-
-
-def test_global_predict_build_caikit_library_request_dict_works_for_unset_primitives():
+def test_global_predict_build_caikit_library_request_dict_works_for_unset_primitives(
+    sample_inference_service,
+):
     """Global predict build_caikit_library_request_dict works for primitives"""
-    request = primitive_party_pb2.OptionalPrimitives()
-
-    request_dict = build_caikit_library_request_dict(request, _primitives_function)
-    # dict started with 15 keys (15 args)
-    # all fields that are unset are removed
-    assert len(request_dict.keys()) == 0
-
+    request = sample_inference_service.messages.SampleTaskRequest()
 
-def test_global_predict_build_caikit_library_request_dict_works_for_set_primitives():
-    """Global predict build_caikit_library_request_dict works for primitives"""
-    request = primitive_party_pb2.OptionalPrimitives(
-        bool_field=False, int64_field=10, float_field=0.0
+    request_dict = build_caikit_library_request_dict(
+        request, SamplePrimitiveModule.RUN_SIGNATURE
     )
-
-    request_dict = build_caikit_library_request_dict(request, _primitives_function)
-    # dict started with 15 keys (15 args)
-    # we set the bool, int and float field, hence they should
-    # be in the request object
-
-    assert len(request_dict.keys()) == 3
-    assert "float_field" in request_dict
-    assert isinstance(request_dict["float_field"], float)
-    assert "bool_field" in request_dict
-    assert isinstance(request_dict["bool_field"], bool)
-    assert "int64_field" in request_dict
-
-
-def test_global_predict_build_caikit_library_request_dict_works_for_repeated_fields():
-    """Global predict build_caikit_library_request_dict works for repeated fields"""
-
-    # TODO: uncomment the repeated_message_field test when we have support for the repeated MessageType field
-
-    request = primitive_party_pb2.Repeateds(repeated_string_field=["this is a string"])
-
-    def foo_function(
-        self,
-        repeated_string_field,
-        # repeated_message_field
-    ):
-        pass
-
-    request_dict = build_caikit_library_request_dict(request, foo_function)
-    # dict started with 1 key
-    # we expect 1 list fields back int the dict
-    assert len(request_dict.keys()) == 1
-    assert "repeated_string_field" in request_dict
-    assert isinstance(request_dict["repeated_string_field"], list)
-    # self.assertTrue("repeated_message_field" in caikit.core_request)
-    # self.assertIsInstance(caikit.core_request["repeated_message_field"], list)
+    # None of the primitive args should be there
+    assert len(request_dict.keys()) == 0
 
 
-def test_global_train_build_caikit_library_request_dict_creates_caikit_core_run_kwargs_not_fail_when_optional_proto_field_not_exist(
-    sample_train_service,
+def test_global_predict_build_caikit_library_request_dict_works_for_set_primitives(
+    sample_inference_service,
 ):
-    """Global train build_caikit_library_request_dict creates module run kwargs from RPC msg
-    and if not passed in request, it creates the fields with default values"""
-    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
-        model_name=random_test_id()  # not having batch_size, and training_data
-    )
-
-    caikit.core_request = build_caikit_library_request_dict(
-        train_request,
-        sample_lib.modules.sample_task.SampleModule().train,
+    """Global predict build_caikit_library_request_dict works for primitives"""
+    request = sample_inference_service.messages.SampleTaskRequest(
+        int_type=5,
+        float_type=4.2,
+        str_type="moose",
+        bytes_type=b"foo",
+        list_type=["1", "2", "3"],
     )
 
-    expected_arguments = {"training_data"}
-
-    # assert that even though not passed in, caikit.core_request now has training_data
-    # because empty stream types get an empty steam initialized
-    # TODO: will need additional tests for list arguments
-    assert expected_arguments == set(caikit.core_request.keys())
-    assert isinstance(
-        caikit.core_request["training_data"], caikit.core.data_model.DataStream
+    request_dict = build_caikit_library_request_dict(
+        request, SamplePrimitiveModule.RUN_SIGNATURE
     )
+    assert request_dict["int_type"] == 5
+    assert request_dict["float_type"] == 4.2
+    assert request_dict["str_type"] == "moose"
+    assert request_dict["bytes_type"] == b"foo"
+    assert request_dict["list_type"] == ["1", "2", "3"]
 
 
 def test_global_train_build_caikit_library_request_dict_strips_empty_list_from_request(
     sample_train_service,
 ):
     """Global train build_caikit_library_request_dict strips empty list from request"""
     # NOTE: not sure this test is relevant anymore, since nothing effectively gets removed?
@@ -372,15 +295,15 @@
     training_data = stream_type(jsondata=stream_type.JsonData(data=[])).to_proto()
     train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
         model_name=random_test_id(), training_data=training_data
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
-        sample_lib.modules.sample_task.SampleModule().train,
+        sample_lib.modules.sample_task.SampleModule.TRAIN_SIGNATURE,
     )
 
     # model_name is not expected to be passed through
     expected_arguments = {"training_data"}
 
     assert expected_arguments == set(caikit.core_request.keys())
 
@@ -395,16 +318,15 @@
     train_request = sample_train_service.messages.SampleTaskListModuleTrainRequest(
         model_name=random_test_id(),
         training_data=training_data,
         poison_pills=["Bob Marley", "Bunny Livingston"],
     )
 
     caikit.core_request = build_caikit_library_request_dict(
-        train_request,
-        sample_lib.modules.sample_task.ListModule().train,
+        train_request, sample_lib.modules.sample_task.ListModule.TRAIN_SIGNATURE
     )
 
     # model_name is not expected to be passed through
     expected_arguments = {"training_data", "poison_pills"}
 
     assert expected_arguments == set(caikit.core_request.keys())
     assert len(caikit.core_request.keys()) == 2
@@ -424,21 +346,18 @@
         model_name="Bar Training",
         sample_inputsampleinputtype=SampleInputType(name="Gabe").to_proto(),
         batch_size=100,
         training_data=training_data,
     )
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
-        sample_lib.modules.other_task.OtherModule().train,
+        sample_lib.modules.other_task.OtherModule.TRAIN_SIGNATURE,
     )
 
-    expected_arguments = set(
-        sample_lib.modules.other_task.OtherModule().train.__code__.co_varnames
-    )
-    expected_arguments.remove("cls")
+    expected_arguments = {"batch_size", "sample_input", "training_data"}
 
     assert expected_arguments == set(caikit.core_request.keys())
 
 
 def test_global_train_build_caikit_library_request_dict_ok_with_data_stream_file_type_csv(
     sample_train_service, sample_csv_file
 ):
@@ -451,15 +370,15 @@
     train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
         model_name=random_test_id(),
         training_data=training_data,
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
-        sample_lib.modules.sample_task.SampleModule().train,
+        sample_lib.modules.sample_task.SampleModule.TRAIN_SIGNATURE,
     )
 
     # model_name is not expected to be passed through
     expected_arguments = {"training_data"}
 
     assert expected_arguments == set(caikit.core_request.keys())
 
@@ -476,15 +395,15 @@
         model_name=random_test_id(),
         training_data=training_data,
         poison_pills=["Bob Marley", "Bunny Livingston"],
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
-        sample_lib.modules.sample_task.ListModule().train,
+        sample_lib.modules.sample_task.ListModule.TRAIN_SIGNATURE,
     )
 
     # model_name is not expected to be passed through
     expected_arguments = {"training_data", "poison_pills"}
 
     assert expected_arguments == set(caikit.core_request.keys())
     assert len(caikit.core_request.keys()) == 2
@@ -516,149 +435,9 @@
                 training_data=training_data,
             )
         )
 
         # no error because at least 1 json file exists within the provided dir
         caikit.core_request = build_caikit_library_request_dict(
             train_request,
-            sample_lib.modules.sample_task.SampleModule().train,
-        )
-
-
-# ---------------- Error tests for build_caikit_library_request_dict --------------------
-
-
-def test_build_caikit_library_request_dict_raises_invalid_data_stream_source_file(
-    sample_train_service,
-):
-    """Global train build_caikit_library_request_dict works for repeated fields"""
-
-    stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
-    training_data = stream_type(file=stream_type.File(filename="abc.blah")).to_proto()
-    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
-        model_name=random_test_id(),
-        training_data=training_data,
-    )
-
-    with pytest.raises(CaikitRuntimeException) as e:
-        caikit.core_request = build_caikit_library_request_dict(
-            train_request,
-            sample_lib.modules.sample_task.SampleModule().train,
-        )
-
-    assert "Invalid .blah data source file" in e.value.message
-
-
-def test_build_caikit_library_request_dict_raises_invalid_data_stream_source_file_ext(
-    sample_train_service,
-):
-    """Global train build_caikit_library_request_dict works for repeated fields"""
-    with tempfile.NamedTemporaryFile(mode="w", suffix=".txt") as handle:
-        handle.write("not_relevant")
-        handle.flush()
-        fname = handle.name
-        stream_type = (
-            caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
-        )
-        training_data = stream_type(file=stream_type.File(filename=fname)).to_proto()
-        train_request = (
-            sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
-                model_name="Foo Bar Training",
-                training_data=training_data,
-            )
-        )
-
-        with pytest.raises(CaikitRuntimeException) as e:
-            caikit.core_request = build_caikit_library_request_dict(
-                train_request,
-                sample_lib.modules.sample_task.SampleModule().train,
-            )
-
-        assert "Extension not supported" in e.value.message
-
-
-def test_build_caikit_library_request_dict_raises_when_data_stream_file_passes_as_dir(
-    sample_train_service, sample_csv_file
-):
-    """Global train build_caikit_library_request_dict raises for a file passed as directory"""
-
-    stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
-    training_data = stream_type(
-        directory=stream_type.Directory(dirname=sample_csv_file)
-    ).to_proto()
-    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
-        model_name="Foo Bar Training",
-        training_data=training_data,
-    )
-
-    with pytest.raises(CaikitRuntimeException) as e:
-        caikit.core_request = build_caikit_library_request_dict(
-            train_request,
-            sample_lib.modules.sample_task.SampleModule().train,
-        )
-
-    assert "Invalid json directory source file" in e.value.message
-
-
-def test_build_caikit_library_request_dict_raises_when_data_stream_directory_passed_with_nonsupported_extension(
-    sample_train_service,
-):
-    """Global train build_caikit_library_request_dict raises non-supported extension type directory"""
-
-    with tempfile.TemporaryDirectory() as tempdir:
-        fname = os.path.join(tempdir, "justafile.txt")
-        with open(fname, "w") as handle:
-            handle.writelines("blah blah blah")
-
-        stream_type = (
-            caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
+            sample_lib.modules.sample_task.SampleModule.TRAIN_SIGNATURE,
         )
-        training_data = stream_type(
-            directory=stream_type.Directory(dirname=tempdir, extension="txt")
-        ).to_proto()
-        train_request = (
-            sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
-                model_name=random_test_id(),
-                training_data=training_data,
-            )
-        )
-
-        with pytest.raises(CaikitRuntimeException) as e:
-            caikit.core_request = build_caikit_library_request_dict(
-                train_request,
-                sample_lib.modules.sample_task.SampleModule().train,
-            )
-
-        # TODO: change this message once it's implemented
-        assert "Extension not supported!" in e.value.message
-
-
-def test_build_caikit_library_request_dict_raises_when_data_stream_directory_passed_with_incorrect_extension(
-    sample_train_service, sample_csv_file
-):
-    """Global train build_caikit_library_request_dict raises wrong extension type directory"""
-
-    with tempfile.TemporaryDirectory() as tempdir:
-        fname = os.path.join(tempdir, "justafile.csv")
-        with open(fname, "w") as handle:
-            handle.writelines("valid_csv,1,2,3")
-
-        stream_type = (
-            caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
-        )
-        training_data = stream_type(
-            directory=stream_type.Directory(dirname=tempdir, extension="json")
-        ).to_proto()
-        train_request = (
-            sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
-                model_name=random_test_id(),
-                training_data=training_data,
-            )
-        )
-
-        with pytest.raises(CaikitRuntimeException) as e:
-            caikit.core_request = build_caikit_library_request_dict(
-                train_request,
-                sample_lib.modules.sample_task.SampleModule().train,
-            )
-
-        assert "contains no source files with extension" in e.value.message
```

### Comparing `caikit-0.7.0/tests/runtime/work_management/__init__.py` & `caikit-0.7.1/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.7.1/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.7.1/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.7.1/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.7.0/tox.ini` & `caikit-0.7.1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     wheel>=0.38.4
 passenv =
     LOG_LEVEL
     LOG_FILTERS
     LOG_FORMATTER
     LOG_THREAD_ID
     LOG_CHANNEL_WIDTH
-commands = pytest --cov=caikit --cov-report=html {posargs:tests}
+commands = pytest --cov=caikit --cov-report=html:coverage-{env_name} --cov-report=xml:coverage-{env_name}.xml {posargs:tests}
 
 ; Unclear: We probably want to test wheel packaging
 ; But! tox will fail when this is set and _any_ interpreter is missing
 ; Without this, sdist packaging is tested so that's a start.
 package=wheel
 
 [testenv:docs]
```

### Comparing `caikit-0.7.0/PKG-INFO` & `caikit-0.7.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.7.0
+Version: 0.7.1
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
@@ -25,14 +25,20 @@
 Requires-Dist: semver>=2.13.0,<4.0
 Requires-Dist: six>=1.16.0,<2.0.0
 Requires-Dist: tqdm>=4.59.0,<5.0.0
 Project-URL: Source, https://github.com/caikit/caikit
 
 # Caikit
 
+[![Build Status](https://github.com/caikit/caikit/actions/workflows/build-library.yml/badge.svg?branch=main&label=tests)](https://github.com/caikit/caikit/actions)
+[![Minimum Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
+[![Release](https://img.shields.io/github/v/release/caikit/caikit?include_prereleases&style=)](https://github.com/caikit/caikit/releases/)
+[![Read the Docs](https://img.shields.io/static/v1?label=readthedocs&message=reference&color=blue)](https://caikit.readthedocs.io/en/latest/)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7443/badge)](https://bestpractices.coreinfrastructure.org/projects/7443)
+
 Caikit is an AI toolkit that enables users to manage models through a set of developer friendly APIs. It provides a consistent format for creating and using AI models against a wide variety of data domains and tasks.
 
 ![Caikit Overview](https://raw.githubusercontent.com/caikit/caikit/main/caikit-overview.png)
 
 ## Capabilities
 
 Caikit streamlines the management of AI models for application usage by letting AI model authors focus on solving well known problems with novel technology. With a set of model implementations based on Caikit, you can:
```

