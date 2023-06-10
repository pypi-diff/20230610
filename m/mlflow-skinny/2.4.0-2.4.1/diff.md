# Comparing `tmp/mlflow-skinny-2.4.0.tar.gz` & `tmp/mlflow-skinny-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-skinny-2.4.0.tar", last modified: Tue Jun  6 08:24:03 2023, max compression
+gzip compressed data, was "mlflow-skinny-2.4.1.tar", last modified: Sat Jun 10 01:34:27 2023, max compression
```

## Comparing `mlflow-skinny-2.4.0.tar` & `mlflow-skinny-2.4.1.tar`

### file list

```diff
@@ -1,470 +1,473 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.852095 mlflow-skinny-2.4.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11382 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/LICENSE.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      562 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11476 2023-06-06 08:24:03.852095 mlflow-skinny-2.4.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9817 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/README.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      949 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/README_SKINNY.rst
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.820095 mlflow-skinny-2.4.0/mlflow/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6430 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/__main__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3668 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/_doctor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9680 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/_spark_autologging.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.820095 mlflow-skinny-2.4.0/mlflow/artifacts/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6485 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/artifacts/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.820095 mlflow-skinny-2.4.0/mlflow/azure/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/azure/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11647 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/azure/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15140 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/catboost.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24024 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      407 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.820095 mlflow-skinny-2.4.0/mlflow/data/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2477 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7022 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/artifact_dataset_sources.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      946 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/code_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4333 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6297 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/dataset_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3534 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8270 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/dataset_source_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3734 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/delta_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4873 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/digest_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2598 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/filesystem_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3929 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/http_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10400 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/huggingface_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3939 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/huggingface_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7966 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/numpy_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6955 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/pandas_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      897 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/pyfunc_dataset_mixin.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2800 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/schema.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/sources.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15642 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/spark_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2196 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/spark_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3858 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/spark_delta_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11898 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/data/tensorflow_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      881 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/db.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.824095 mlflow-skinny-2.4.0/mlflow/deployments/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3797 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/deployments/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15582 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/deployments/base.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15078 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/deployments/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3825 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/deployments/interface.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5512 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/deployments/plugin_manager.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      556 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/deployments/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28178 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/diviner.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.824095 mlflow-skinny-2.4.0/mlflow/entities/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1211 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1414 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/_mlflow_object.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2118 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1510 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/dataset_input.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3510 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/experiment.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      887 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/experiment_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1215 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/file_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      992 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/input_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1242 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/lifecycle_stage.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1418 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/metric.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.824095 mlflow-skinny-2.4.0/mlflow/entities/model_registry/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      529 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/model_registry/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      286 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/model_registry/_model_registry_entity.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6435 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/model_registry/model_version.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      831 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/model_registry/model_version_stages.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1533 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/model_registry/model_version_status.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      933 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/model_registry/model_version_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4933 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/model_registry/registered_model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/model_registry/registered_model_alias.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/model_registry/registered_model_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1133 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/param.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2134 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/run.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3032 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/run_data.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6182 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/run_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/run_inputs.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1550 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/run_status.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      890 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/run_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1212 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/source_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1826 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/entities/view_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11904 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/environment_variables.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4881 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/exceptions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5080 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/experiments.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.824095 mlflow-skinny-2.4.0/mlflow/fastai/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25449 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/fastai/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5660 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/fastai/callback.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.824095 mlflow-skinny-2.4.0/mlflow/gluon/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19248 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/gluon/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2020 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/gluon/_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14185 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/h2o.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/keras.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.824095 mlflow-skinny-2.4.0/mlflow/langchain/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21279 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/langchain/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4898 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/langchain/api_request_parallel_processor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38975 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/lightgbm.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      180 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/llm.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5786 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/ml_package_versions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13885 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/mleap.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.824095 mlflow-skinny-2.4.0/mlflow/models/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3637 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9803 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/cli.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.824095 mlflow-skinny-2.4.0/mlflow/models/container/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9387 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/container/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.828095 mlflow-skinny-2.4.0/mlflow/models/container/scoring_server/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/container/scoring_server/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/container/scoring_server/wsgi.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9870 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/docker_utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.828095 mlflow-skinny-2.4.0/mlflow/models/evaluation/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      491 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/evaluation/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3105 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/evaluation/_shap_patch.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6769 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/evaluation/artifacts.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    64594 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/evaluation/base.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52848 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/evaluation/default_evaluator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2036 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/evaluation/evaluator_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6223 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/evaluation/lift_curve.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10946 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/evaluation/validation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3420 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/flavor_backend.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2354 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/flavor_backend_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24997 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12595 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/signature.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    39843 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11707 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/models/wheeled_model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24919 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/onnx.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.828095 mlflow-skinny-2.4.0/mlflow/openai/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23265 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/openai/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12309 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/openai/api_request_parallel_processor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2936 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/openai/retry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2088 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/openai/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.828095 mlflow-skinny-2.4.0/mlflow/paddle/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23859 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/paddle/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4792 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/paddle/_paddle_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17616 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pmdarima.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.828095 mlflow-skinny-2.4.0/mlflow/projects/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17396 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/projects/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11532 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/projects/_project_spec.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.828095 mlflow-skinny-2.4.0/mlflow/projects/backend/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      271 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/projects/backend/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2210 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/projects/backend/abstract_backend.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1079 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/projects/backend/loader.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17277 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/projects/backend/local.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20212 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/projects/databricks.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6402 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/projects/docker.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       94 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/projects/env_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6379 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/projects/kubernetes.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3574 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/projects/submitted_run.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12237 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/projects/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14024 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/prophet.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.828095 mlflow-skinny-2.4.0/mlflow/protos/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/protos/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17261 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/protos/databricks_artifacts_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14095 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/protos/databricks_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    42316 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/protos/databricks_uc_registry_messages_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12471 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/protos/databricks_uc_registry_service_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16146 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/protos/facet_feature_statistics_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1361 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/protos/internal_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8552 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/protos/mlflow_artifacts_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    54475 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/protos/model_registry_pb2.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.828095 mlflow-skinny-2.4.0/mlflow/protos/scalapb/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/protos/scalapb/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3307 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/protos/scalapb/scalapb_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    53666 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/protos/service_pb2.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/pyfunc/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    81981 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyfunc/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16573 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyfunc/backend.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      901 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyfunc/mlserver.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15392 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyfunc/model.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/pyfunc/scoring_server/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13910 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyfunc/scoring_server/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4222 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyfunc/scoring_server/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      175 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyfunc/scoring_server/wsgi.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2124 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyfunc/spark_model_cache.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1001 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyfunc/stdin_server.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  7380252 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pypi_package_index.json
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/pyspark/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyspark/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/pyspark/ml/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    55602 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyspark/ml/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2908 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyspark/ml/_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1886 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pyspark/ml/log_model_allowlist.txt
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/pytorch/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    45559 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pytorch/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17568 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pytorch/_lightning_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2654 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pytorch/_pytorch_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2090 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/pytorch/pickle_module.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/recipes/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1330 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6092 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/artifacts.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/recipes/cards/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10189 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/cards/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4780 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/cards/histogram_generator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12548 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/cards/pandas_renderer.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/recipes/cards/templates/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/cards/templates/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/recipes/classification/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/classification/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/recipes/classification/v1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      122 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/classification/v1/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20462 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/classification/v1/recipe.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2917 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18431 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/dag_help_strings.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17933 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/recipe.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/recipes/regression/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/regression/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/recipes/regression/v1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      114 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/regression/v1/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22495 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/regression/v1/recipe.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14841 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/step.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/recipes/steps/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/steps/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/recipes/steps/automl/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/steps/automl/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6260 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/steps/automl/flaml.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20666 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/steps/evaluate.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.832095 mlflow-skinny-2.4.0/mlflow/recipes/steps/ingest/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11137 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/steps/ingest/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26390 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/steps/ingest/datasets.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12140 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/steps/predict.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7664 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/steps/register.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19541 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/steps/split.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    59735 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/steps/train.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10602 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/steps/transform.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.836095 mlflow-skinny-2.4.0/mlflow/recipes/utils/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6355 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/utils/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28468 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/utils/execution.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8990 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/utils/metrics.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7680 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/utils/step.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12316 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/utils/tracking.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1748 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/recipes/utils/wrapped_recipe_model.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.836095 mlflow-skinny-2.4.0/mlflow/rfunc/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1115 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/rfunc/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3639 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/rfunc/backend.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2519 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/runs.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.836095 mlflow-skinny-2.4.0/mlflow/sagemaker/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   135083 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/sagemaker/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12986 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/sagemaker/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14450 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/sentence_transformers.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.836095 mlflow-skinny-2.4.0/mlflow/server/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7077 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/server/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.836095 mlflow-skinny-2.4.0/mlflow/server/auth/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27898 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/server/auth/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      123 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/server/auth/basic_auth.ini
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4689 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/server/auth/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/server/auth/config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4217 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/server/auth/entities.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2673 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/server/auth/logo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1267 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/server/auth/permissions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1111 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/server/auth/routes.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12648 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/server/auth/sqlalchemy_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    69362 2023-06-06 08:23:56.000000 mlflow-skinny-2.4.0/mlflow/server/handlers.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      481 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/server/prometheus_exporter.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26647 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/shap.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.836095 mlflow-skinny-2.4.0/mlflow/sklearn/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    85689 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/sklearn/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37469 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/sklearn/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14259 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/spacy.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    45175 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/spark.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24781 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/statsmodels.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.836095 mlflow-skinny-2.4.0/mlflow/store/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      227 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.836095 mlflow-skinny-2.4.0/mlflow/store/_unity_catalog/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/_unity_catalog/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.836095 mlflow-skinny-2.4.0/mlflow/store/_unity_catalog/registry/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/_unity_catalog/registry/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28390 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/_unity_catalog/registry/rest_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5419 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/_unity_catalog/registry/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.840095 mlflow-skinny-2.4.0/mlflow/store/artifact/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10481 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5836 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/artifact_repository_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8136 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/azure_blob_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5829 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/azure_data_lake_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5378 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34659 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/databricks_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8978 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/databricks_models_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10247 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/dbfs_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5234 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/ftp_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5873 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/gcs_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9684 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/hdfs_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3377 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/http_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5107 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/local_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3001 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/mlflow_artifacts_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6757 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/models_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6016 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/runs_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9433 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/s3_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5455 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/sftp_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5592 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/unity_catalog_models_artifact_repo.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.840095 mlflow-skinny-2.4.0/mlflow/store/artifact/utils/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/utils/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3934 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/artifact/utils/models.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.840095 mlflow-skinny-2.4.0/mlflow/store/db/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db/base_sql_model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      221 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db/db_types.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10567 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.840095 mlflow-skinny-2.4.0/mlflow/store/db_migrations/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1634 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/alembic.ini
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2768 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/env.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.840095 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1990 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      462 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/0c779009ac13_add_deleted_time_field_to_runs_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      924 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2624 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1375 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1201 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      940 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1014 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      476 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/84291f40a231_add_run_link_to_model_version.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5716 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1666 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      577 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      582 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2830 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.840095 mlflow-skinny-2.4.0/mlflow/store/entities/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/entities/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      479 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/entities/paged_list.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.840095 mlflow-skinny-2.4.0/mlflow/store/model_registry/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      605 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/model_registry/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11022 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/model_registry/abstract_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1440 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/model_registry/base_rest_store.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.840095 mlflow-skinny-2.4.0/mlflow/store/model_registry/dbmodels/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/model_registry/dbmodels/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/model_registry/dbmodels/models.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38833 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/model_registry/file_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16920 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/model_registry/rest_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50646 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/model_registry/sqlalchemy_store.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.844095 mlflow-skinny-2.4.0/mlflow/store/tracking/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1154 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/tracking/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13534 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/tracking/abstract_store.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.844095 mlflow-skinny-2.4.0/mlflow/store/tracking/dbmodels/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/tracking/dbmodels/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8315 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/tracking/dbmodels/initial_models.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21085 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/tracking/dbmodels/models.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52631 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/tracking/file_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12822 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/tracking/rest_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    75925 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/store/tracking/sqlalchemy_store.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.844095 mlflow-skinny-2.4.0/mlflow/tensorflow/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    60208 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tensorflow/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8442 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tensorflow/_autolog.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.844095 mlflow-skinny-2.4.0/mlflow/tracking/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      995 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.844095 mlflow-skinny-2.4.0/mlflow/tracking/_model_registry/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       41 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/_model_registry/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15534 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/_model_registry/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9641 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/_model_registry/fluent.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3152 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/_model_registry/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7008 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/_model_registry/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.844095 mlflow-skinny-2.4.0/mlflow/tracking/_tracking_service/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/_tracking_service/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24289 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/_tracking_service/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2335 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/_tracking_service/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9517 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/_tracking_service/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7540 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/artifact_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   142886 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.844095 mlflow-skinny-2.4.0/mlflow/tracking/context/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/context/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1076 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/context/abstract_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/context/databricks_cluster_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      561 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/context/databricks_command_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1965 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/context/databricks_job_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1713 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/context/databricks_notebook_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1952 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/context/databricks_repo_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/context/default_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      898 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/context/git_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/context/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      443 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/context/system_environment_context.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.844095 mlflow-skinny-2.4.0/mlflow/tracking/default_experiment/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       28 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/default_experiment/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1703 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/default_experiment/abstract_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1718 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2300 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3173 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/default_experiment/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    78452 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/fluent.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3404 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/llm_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2248 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/metric_value_conversion_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3515 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/registry.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.844095 mlflow-skinny-2.4.0/mlflow/tracking/request_header/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/request_header/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1077 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/request_header/abstract_request_header_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1336 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/request_header/databricks_request_header_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      486 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/request_header/default_request_header_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2867 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/tracking/request_header/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   109369 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/transformers.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.848095 mlflow-skinny-2.4.0/mlflow/types/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      299 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/types/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14931 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/types/schema.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18044 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/types/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.848095 mlflow-skinny-2.4.0/mlflow/utils/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9365 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6589 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/_capture_modules.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2274 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/_capture_transformers_modules.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6387 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/_spark_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5009 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/annotations.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/arguments_utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.852095 mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27045 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16642 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10937 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13381 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/logging_and_warnings.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    47266 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/safety.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3570 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/versioning.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      215 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/class_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6431 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/cli_args.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13002 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/conda.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      432 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/data_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23803 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/databricks_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9138 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/docstring_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/env.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/env_manager.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21867 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/environment.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28860 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/file_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2306 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/git_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24178 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/gorilla.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.852095 mlflow-skinny-2.4.0/mlflow/utils/import_hooks/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13645 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/import_hooks/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2597 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/logging_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/mime_type_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4024 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/mlflow_tags.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8109 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/model_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5873 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/name_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2412 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/nfs_on_spark.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      139 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/os.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5799 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/process.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19909 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/proto_json_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6164 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/request_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20034 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/requirements_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11852 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/rest_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    56769 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/search_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2368 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/server_cli_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3805 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/string_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      512 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/time_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14271 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/uri.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19435 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/validation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16278 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/utils/virtualenv.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      147 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/version.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.852095 mlflow-skinny-2.4.0/mlflow/xgboost/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37317 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/xgboost/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2908 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/mlflow/xgboost/_autolog.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.852095 mlflow-skinny-2.4.0/mlflow_skinny.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11476 2023-06-06 08:24:03.000000 mlflow-skinny-2.4.0/mlflow_skinny.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14646 2023-06-06 08:24:03.000000 mlflow-skinny-2.4.0/mlflow_skinny.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-06 08:24:03.000000 mlflow-skinny-2.4.0/mlflow_skinny.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-06-06 08:24:03.000000 mlflow-skinny-2.4.0/mlflow_skinny.egg-info/entry_points.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-06 08:24:03.000000 mlflow-skinny-2.4.0/mlflow_skinny.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      570 2023-06-06 08:24:03.000000 mlflow-skinny-2.4.0/mlflow_skinny.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-06-06 08:24:03.000000 mlflow-skinny-2.4.0/mlflow_skinny.egg-info/top_level.txt
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.852095 mlflow-skinny-2.4.0/pylint_plugins/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      614 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/pylint_plugins/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2234 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/pylint_plugins/errors.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4556 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/pylint_plugins/import_checker.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      856 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/pylint_plugins/print_function.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.852095 mlflow-skinny-2.4.0/pylint_plugins/pytest_raises_checker/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1546 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/pylint_plugins/pytest_raises_checker/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      571 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/pylint_plugins/set_checker.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      878 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/pylint_plugins/string_checker.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      692 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/pylint_plugins/unittest_assert_raises.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-06 08:24:03.852095 mlflow-skinny-2.4.0/requirements/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      609 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/requirements/core-requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      481 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/requirements/skinny-requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-06 08:24:03.852095 mlflow-skinny-2.4.0/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7113 2023-06-06 08:23:57.000000 mlflow-skinny-2.4.0/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11382 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/LICENSE.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      608 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11500 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9817 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/README.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      949 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/README_SKINNY.rst
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.905476 mlflow-skinny-2.4.1/mlflow/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6490 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/__main__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3668 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/_doctor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9680 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/_spark_autologging.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.905476 mlflow-skinny-2.4.1/mlflow/artifacts/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6485 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/artifacts/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.905476 mlflow-skinny-2.4.1/mlflow/azure/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/azure/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11647 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/azure/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15140 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/catboost.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24024 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      407 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.905476 mlflow-skinny-2.4.1/mlflow/data/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2477 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7022 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/artifact_dataset_sources.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      946 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/code_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4333 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6297 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/dataset_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3534 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8270 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/dataset_source_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3734 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/delta_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4873 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/digest_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2598 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/filesystem_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3929 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/http_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10462 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/huggingface_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4008 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/huggingface_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7966 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/numpy_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6955 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/pandas_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      897 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/pyfunc_dataset_mixin.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2800 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/schema.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/sources.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15642 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/spark_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2196 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/spark_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3858 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/spark_delta_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11898 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/data/tensorflow_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      881 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/db.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.905476 mlflow-skinny-2.4.1/mlflow/deployments/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3797 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/deployments/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15582 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/deployments/base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15078 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/deployments/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3825 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/deployments/interface.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5512 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/deployments/plugin_manager.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      556 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/deployments/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28178 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/diviner.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/entities/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1211 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1414 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/_mlflow_object.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2118 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1510 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/dataset_input.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3510 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/experiment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      887 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/experiment_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1215 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/file_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      992 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/input_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1242 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/lifecycle_stage.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1418 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/metric.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/entities/model_registry/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      529 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      286 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/_model_registry_entity.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6435 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      831 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version_stages.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1533 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version_status.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      933 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4933 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/registered_model.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/registered_model_alias.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/model_registry/registered_model_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1133 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/param.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2134 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/run.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3032 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/run_data.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6182 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/run_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/run_inputs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1550 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/run_status.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      890 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/run_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1212 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/source_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1826 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/entities/view_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12114 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/environment_variables.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4881 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/exceptions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5080 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/experiments.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/fastai/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25449 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/fastai/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5660 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/fastai/callback.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/gluon/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19248 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/gluon/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2020 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/gluon/_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14185 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/h2o.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    36396 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/johnsnowlabs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/keras.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/langchain/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21279 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/langchain/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4898 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/langchain/api_request_parallel_processor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38975 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/lightgbm.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      180 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/llm.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5786 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/ml_package_versions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13885 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/mleap.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/models/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3637 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9803 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/cli.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/models/container/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9387 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/container/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/models/container/scoring_server/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/container/scoring_server/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/container/scoring_server/wsgi.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9870 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/docker_utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/models/evaluation/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      491 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3105 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/_shap_patch.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6769 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/artifacts.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    64594 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52848 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/default_evaluator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2036 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/evaluator_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6223 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/lift_curve.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10946 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/evaluation/validation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3420 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/flavor_backend.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2354 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/flavor_backend_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24997 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/model.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12595 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/signature.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    39843 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11707 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/models/wheeled_model.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24919 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/onnx.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/openai/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23265 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/openai/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12309 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/openai/api_request_parallel_processor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2936 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/openai/retry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2088 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/openai/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.909476 mlflow-skinny-2.4.1/mlflow/paddle/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23859 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/paddle/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4792 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/paddle/_paddle_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17616 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pmdarima.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/projects/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17396 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11532 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/_project_spec.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/projects/backend/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      271 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/backend/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2210 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/backend/abstract_backend.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1079 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/backend/loader.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17277 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/backend/local.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20212 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/databricks.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6402 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/docker.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       94 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/env_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6379 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/kubernetes.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3574 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/submitted_run.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12237 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/projects/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14024 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/prophet.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/protos/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17261 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/databricks_artifacts_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14095 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/databricks_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    42316 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/databricks_uc_registry_messages_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12471 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/databricks_uc_registry_service_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16146 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/facet_feature_statistics_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1361 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/internal_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8552 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/mlflow_artifacts_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    54475 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/model_registry_pb2.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/protos/scalapb/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/scalapb/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3307 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/scalapb/scalapb_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    53666 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/protos/service_pb2.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/pyfunc/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    81981 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16573 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/backend.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      901 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/mlserver.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15392 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/model.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/pyfunc/scoring_server/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13910 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/scoring_server/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4222 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/scoring_server/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      175 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/scoring_server/wsgi.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2124 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/spark_model_cache.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1001 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyfunc/stdin_server.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  7380252 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pypi_package_index.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/pyspark/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyspark/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/pyspark/ml/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    55602 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyspark/ml/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2908 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyspark/ml/_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1886 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pyspark/ml/log_model_allowlist.txt
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.913476 mlflow-skinny-2.4.1/mlflow/pytorch/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    45559 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pytorch/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17568 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pytorch/_lightning_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2654 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pytorch/_pytorch_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2090 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/pytorch/pickle_module.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1330 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6092 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/artifacts.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/cards/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10189 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/cards/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4780 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/cards/histogram_generator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12548 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/cards/pandas_renderer.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/cards/templates/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/cards/templates/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/classification/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/classification/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/classification/v1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      122 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/classification/v1/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20462 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/classification/v1/recipe.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2917 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18431 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/dag_help_strings.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17933 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/recipe.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/regression/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/regression/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/regression/v1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      114 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/regression/v1/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22495 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/regression/v1/recipe.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14841 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/step.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/steps/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/steps/automl/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/automl/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6260 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/automl/flaml.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20666 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/evaluate.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/steps/ingest/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11137 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/ingest/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26390 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/ingest/datasets.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12140 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/predict.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7664 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/register.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19541 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/split.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    59735 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/train.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10602 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/steps/transform.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/recipes/utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6355 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28468 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/utils/execution.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8990 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/utils/metrics.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7680 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/utils/step.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12316 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/utils/tracking.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1748 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/recipes/utils/wrapped_recipe_model.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/rfunc/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1115 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/rfunc/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3639 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/rfunc/backend.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2519 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/runs.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/sagemaker/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   135083 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/sagemaker/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12986 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/sagemaker/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14450 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/sentence_transformers.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/server/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7077 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/server/auth/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28016 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      123 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/basic_auth.ini
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4689 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4217 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/entities.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2673 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/logo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1267 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/permissions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1111 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/routes.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12648 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/auth/sqlalchemy_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    69738 2023-06-10 01:34:20.000000 mlflow-skinny-2.4.1/mlflow/server/handlers.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      481 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/server/prometheus_exporter.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26647 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/shap.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.917476 mlflow-skinny-2.4.1/mlflow/sklearn/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    85689 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/sklearn/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37469 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/sklearn/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14259 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/spacy.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    45175 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/spark.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24781 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/statsmodels.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      227 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/registry/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/registry/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28656 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/registry/rest_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5419 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/registry/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/artifact/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10481 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5836 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/artifact_repository_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8136 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/azure_blob_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5829 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/azure_data_lake_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5378 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35001 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/databricks_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9819 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/databricks_models_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10247 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/dbfs_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5234 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/ftp_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5873 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/gcs_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9684 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/hdfs_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3377 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/http_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5107 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/local_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3001 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/mlflow_artifacts_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6757 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/models_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6016 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/runs_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9433 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/s3_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5455 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/sftp_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5592 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/unity_catalog_models_artifact_repo.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/artifact/utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3934 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/artifact/utils/models.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/db/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db/base_sql_model.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      221 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db/db_types.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10567 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.921476 mlflow-skinny-2.4.1/mlflow/store/db_migrations/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1634 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/alembic.ini
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2768 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/env.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1990 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      462 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/0c779009ac13_add_deleted_time_field_to_runs_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      924 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2624 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1375 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1201 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      940 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1014 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      476 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/84291f40a231_add_run_link_to_model_version.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5716 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1666 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      577 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      582 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2830 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/store/entities/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/entities/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      479 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/entities/paged_list.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/store/model_registry/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      605 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11022 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/abstract_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1440 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/base_rest_store.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/store/model_registry/dbmodels/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/dbmodels/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/dbmodels/models.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38833 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/file_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16920 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/rest_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50646 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/model_registry/sqlalchemy_store.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/store/tracking/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1154 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13534 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/abstract_store.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/store/tracking/dbmodels/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/dbmodels/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8315 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/dbmodels/initial_models.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21085 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/dbmodels/models.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52631 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/file_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12822 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/rest_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    77913 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/store/tracking/sqlalchemy_store.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/tensorflow/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    60208 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tensorflow/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8442 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tensorflow/_autolog.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/tracking/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      995 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       41 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15534 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9641 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/fluent.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3152 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7008 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.925476 mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24289 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2335 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9517 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7540 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/artifact_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   142886 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.929476 mlflow-skinny-2.4.1/mlflow/tracking/context/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1076 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/abstract_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_cluster_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      561 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_command_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1965 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_job_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1713 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_notebook_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1952 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_repo_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/default_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      898 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/git_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      443 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/context/system_environment_context.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.929476 mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       28 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1703 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/abstract_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1718 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2300 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3173 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    78452 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/fluent.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3404 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/llm_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2248 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/metric_value_conversion_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3515 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/registry.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.929476 mlflow-skinny-2.4.1/mlflow/tracking/request_header/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/request_header/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1077 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/request_header/abstract_request_header_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1336 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/request_header/databricks_request_header_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      486 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/request_header/default_request_header_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2867 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/tracking/request_header/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   110231 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/transformers.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.929476 mlflow-skinny-2.4.1/mlflow/types/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      299 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/types/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15035 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/types/schema.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18044 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/types/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/mlflow/utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9365 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6589 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/_capture_modules.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2274 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/_capture_transformers_modules.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6387 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/_spark_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5009 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/annotations.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/arguments_utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27045 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16642 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10937 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13381 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/logging_and_warnings.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    47266 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/safety.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3570 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/versioning.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      215 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/class_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6431 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/cli_args.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13002 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/conda.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      432 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/data_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23803 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/databricks_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9138 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/docstring_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1669 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/download_cloud_file_chunk.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/env.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/env_manager.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22634 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/environment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30464 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/file_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2306 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/git_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24178 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/gorilla.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/mlflow/utils/import_hooks/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13645 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/import_hooks/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2597 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/logging_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/mime_type_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4024 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/mlflow_tags.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8109 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/model_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5873 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/name_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2412 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/nfs_on_spark.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      139 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/os.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5799 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/process.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19909 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/proto_json_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5560 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/request_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20034 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/requirements_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11852 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/rest_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    59666 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/search_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2368 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/server_cli_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3805 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/string_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      512 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/time_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14271 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/uri.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19435 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/validation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16278 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/utils/virtualenv.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      147 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/version.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/mlflow/xgboost/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37317 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/xgboost/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2908 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/mlflow/xgboost/_autolog.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11500 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14749 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/entry_points.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/not-zip-safe
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      618 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-06-10 01:34:27.000000 mlflow-skinny-2.4.1/mlflow_skinny.egg-info/top_level.txt
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/pylint_plugins/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      614 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2234 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/errors.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4556 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/import_checker.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      856 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/print_function.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/pylint_plugins/pytest_raises_checker/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1546 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/pytest_raises_checker/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      571 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/set_checker.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      878 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/string_checker.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      692 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/pylint_plugins/unittest_assert_raises.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/requirements/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      609 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/requirements/core-requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      297 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/requirements/gateway-requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      481 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/requirements/skinny-requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-10 01:34:27.933476 mlflow-skinny-2.4.1/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7311 2023-06-10 01:34:21.000000 mlflow-skinny-2.4.1/setup.py
```

### Comparing `mlflow-skinny-2.4.0/LICENSE.txt` & `mlflow-skinny-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/MANIFEST.in` & `mlflow-skinny-2.4.1/MANIFEST.in`

 * *Files 10% similar despite different names*

```diff
@@ -5,7 +5,8 @@
 exclude pyproject.toml
 
 # Note that README.rst is included in a source distribution by default:
 # https://packaging.python.org/guides/using-manifest-in/#how-files-are-included-in-an-sdist
 include README_SKINNY.rst
 include requirements/skinny-requirements.txt
 include requirements/core-requirements.txt
+include requirements/gateway-requirements.txt
```

### Comparing `mlflow-skinny-2.4.0/PKG-INFO` & `mlflow-skinny-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: mlflow-skinny
-Version: 2.4.0
+Version: 2.4.1
 Summary: MLflow: A Platform for ML Development and Productionization
 Home-page: https://mlflow.org/
 Author: Databricks
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mlflow/mlflow/issues
 Project-URL: Documentation, https://mlflow.org/docs/latest/index.html
 Project-URL: Source Code, https://github.com/mlflow/mlflow
 Keywords: ml ai databricks
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: extras
 Provides-Extra: databricks
+Provides-Extra: gateway
 Provides-Extra: sqlserver
 Provides-Extra: aliyun-oss
 License-File: LICENSE.txt
 
 =======================================================================
 MLflow Skinny: A Lightweight Machine Learning Lifecycle Platform Client
 =======================================================================
```

### Comparing `mlflow-skinny-2.4.0/README.rst` & `mlflow-skinny-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/README_SKINNY.rst` & `mlflow-skinny-2.4.1/README_SKINNY.rst`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/__init__.py` & `mlflow-skinny-2.4.1/mlflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     from mlflow import pmdarima
     from mlflow import diviner
     from mlflow import transformers
     from mlflow import langchain
     from mlflow import llm
     from mlflow import openai
     from mlflow import sentence_transformers
+    from mlflow import johnsnowlabs
 
     _model_flavors_supported = [
         "catboost",
         "fastai",
         "gluon",
         "h2o",
         "lightgbm",
@@ -101,14 +102,15 @@
         "pmdarima",
         "diviner",
         "transformers",
         "langchain",
         "llm",
         "openai",
         "sentence_transformers",
+        "johnsnowlabs",
     ]
 except ImportError as e:
     # We are conditional loading these commands since the skinny client does
     # not support them due to the pandas and numpy dependencies of MLflow Models
     pass
```

### Comparing `mlflow-skinny-2.4.0/mlflow/_doctor.py` & `mlflow-skinny-2.4.1/mlflow/_doctor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/_spark_autologging.py` & `mlflow-skinny-2.4.1/mlflow/_spark_autologging.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/artifacts/__init__.py` & `mlflow-skinny-2.4.1/mlflow/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/azure/client.py` & `mlflow-skinny-2.4.1/mlflow/azure/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/catboost.py` & `mlflow-skinny-2.4.1/mlflow/catboost.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/cli.py` & `mlflow-skinny-2.4.1/mlflow/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/__init__.py` & `mlflow-skinny-2.4.1/mlflow/data/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/artifact_dataset_sources.py` & `mlflow-skinny-2.4.1/mlflow/data/artifact_dataset_sources.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/code_dataset_source.py` & `mlflow-skinny-2.4.1/mlflow/data/code_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/dataset.py` & `mlflow-skinny-2.4.1/mlflow/data/dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/dataset_registry.py` & `mlflow-skinny-2.4.1/mlflow/data/dataset_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/dataset_source.py` & `mlflow-skinny-2.4.1/mlflow/data/dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/dataset_source_registry.py` & `mlflow-skinny-2.4.1/mlflow/data/dataset_source_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/delta_dataset_source.py` & `mlflow-skinny-2.4.1/mlflow/data/delta_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/digest_utils.py` & `mlflow-skinny-2.4.1/mlflow/data/digest_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/filesystem_dataset_source.py` & `mlflow-skinny-2.4.1/mlflow/data/filesystem_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/http_dataset_source.py` & `mlflow-skinny-2.4.1/mlflow/data/http_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/huggingface_dataset.py` & `mlflow-skinny-2.4.1/mlflow/data/huggingface_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import logging
 from functools import cached_property
-from typing import Any, Union, Optional, Mapping, Sequence, Dict
+from typing import Any, Union, Optional, Mapping, Sequence, Dict, TYPE_CHECKING
 
-import datasets
 
 from mlflow.data.dataset import Dataset
 from mlflow.data.digest_utils import compute_pandas_digest
 from mlflow.data.pyfunc_dataset_mixin import PyFuncConvertibleDatasetMixin, PyFuncInputsOutputs
 from mlflow.data.huggingface_dataset_source import HuggingFaceDatasetSource
 from mlflow.exceptions import MlflowException
 from mlflow.models.evaluation.base import EvaluationDataset
@@ -16,24 +15,27 @@
 from mlflow.types.utils import _infer_schema
 from mlflow.utils.annotations import experimental
 
 _logger = logging.getLogger(__name__)
 
 _MAX_ROWS_FOR_DIGEST_COMPUTATION_AND_SCHEMA_INFERENCE = 10000
 
+if TYPE_CHECKING:
+    import datasets
+
 
 @experimental
 class HuggingFaceDataset(Dataset, PyFuncConvertibleDatasetMixin):
     """
     Represents a HuggingFace dataset for use with MLflow Tracking.
     """
 
     def __init__(
         self,
-        ds: datasets.Dataset,
+        ds: "datasets.Dataset",
         source: HuggingFaceDatasetSource,
         targets: Optional[str] = None,
         name: Optional[str] = None,
         digest: Optional[str] = None,
     ):
         """
         :param ds: A Hugging Face dataset. Must be an instance of `datasets.Dataset`.
@@ -81,15 +83,15 @@
             "schema": json.dumps({"mlflow_colspec": self.schema.to_dict()})
             if self.schema
             else None,
             "profile": json.dumps(self.profile),
         }
 
     @property
-    def ds(self) -> datasets.Dataset:
+    def ds(self) -> "datasets.Dataset":
         """
         The Hugging Face ``datasets.Dataset`` instance.
 
         :return: The Hugging Face ``datasets.Dataset`` instance.
         """
         return self._ds
 
@@ -215,14 +217,15 @@
                  upon request via :py:func:`HuggingFaceDataset.source.load()
                  <mlflow.data.huggingface_dataset_source.HuggingFaceDatasetSource.load>`.
     :param name: The name of the dataset. E.g. "wiki_train". If unspecified, a name is
                  automatically generated.
     :param digest: The digest (hash, fingerprint) of the dataset. If unspecified, a digest
                    is automatically computed.
     """
+    import datasets
     from mlflow.data.code_dataset_source import CodeDatasetSource
     from mlflow.tracking.context import registry
 
     if not isinstance(ds, datasets.Dataset):
         raise MlflowException(
             f"The specified Hugging Face dataset must be an instance of ``datasets.Dataset``."
             f" Instead, found an instance of: {type(ds)}",
```

### Comparing `mlflow-skinny-2.4.0/mlflow/data/huggingface_dataset_source.py` & `mlflow-skinny-2.4.1/mlflow/data/huggingface_dataset_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-import datasets
-
-from typing import Any, Union, Optional, Mapping, Sequence, Dict
+from typing import Any, Union, Optional, Mapping, Sequence, Dict, TYPE_CHECKING
 
 from mlflow.data.dataset_source import DatasetSource
 from mlflow.utils.annotations import experimental
 
 
+if TYPE_CHECKING:
+    import datasets
+
+
 @experimental
 class HuggingFaceDatasetSource(DatasetSource):
     """
     Represents the source of a Hugging Face dataset used in MLflow Tracking.
     """
 
     def __init__(
         self,
         path: str,
         config_name: Optional[str] = None,
         data_dir: Optional[str] = None,
         data_files: Optional[
             Union[str, Sequence[str], Mapping[str, Union[str, Sequence[str]]]]
         ] = None,
-        split: Optional[Union[str, datasets.Split]] = None,
-        revision: Optional[Union[str, datasets.Version]] = None,
-        task: Optional[Union[str, datasets.TaskTemplate]] = None,
+        split: Optional[Union[str, "datasets.Split"]] = None,
+        revision: Optional[Union[str, "datasets.Version"]] = None,
+        task: Optional[Union[str, "datasets.TaskTemplate"]] = None,
     ):
         """
         :param path: The path of the Hugging Face dataset.
         :param config_name: The name of of the Hugging Face dataset configuration.
         :param data_dir: The `data_dir` of the Hugging Face dataset configuration.
         :param data_files: Paths to source data file(s) for the Hugging Face dataset configuration.
         :param revision: Version of the dataset script to load.
@@ -52,14 +54,16 @@
         :param kwargs: Additional keyword arguments used for loading the dataset with
                        the Hugging Face ``datasets.load_dataset()`` method. The following keyword
                        arguments are used automatically from the dataset source but may be
                        overridden by values passed in ``**kwargs``: ``path``, ``name``,
                        ``data_dir``, ``data_files``, ``split``, ``revision``, ``task``.
         :return: An instance of ``datasets.Dataset``.
         """
+        import datasets
+
         load_kwargs = {
             "path": self._path,
             "name": self._config_name,
             "data_dir": self._data_dir,
             "data_files": self._data_files,
             "split": self._split,
             "revision": self._revision,
```

### Comparing `mlflow-skinny-2.4.0/mlflow/data/numpy_dataset.py` & `mlflow-skinny-2.4.1/mlflow/data/numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/pandas_dataset.py` & `mlflow-skinny-2.4.1/mlflow/data/pandas_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/pyfunc_dataset_mixin.py` & `mlflow-skinny-2.4.1/mlflow/data/pyfunc_dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/schema.py` & `mlflow-skinny-2.4.1/mlflow/data/schema.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/spark_dataset.py` & `mlflow-skinny-2.4.1/mlflow/data/spark_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/spark_dataset_source.py` & `mlflow-skinny-2.4.1/mlflow/data/spark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/spark_delta_utils.py` & `mlflow-skinny-2.4.1/mlflow/data/spark_delta_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/data/tensorflow_dataset.py` & `mlflow-skinny-2.4.1/mlflow/data/tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/db.py` & `mlflow-skinny-2.4.1/mlflow/db.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/deployments/__init__.py` & `mlflow-skinny-2.4.1/mlflow/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/deployments/base.py` & `mlflow-skinny-2.4.1/mlflow/deployments/base.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/deployments/cli.py` & `mlflow-skinny-2.4.1/mlflow/deployments/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/deployments/interface.py` & `mlflow-skinny-2.4.1/mlflow/deployments/interface.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/deployments/plugin_manager.py` & `mlflow-skinny-2.4.1/mlflow/deployments/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/deployments/utils.py` & `mlflow-skinny-2.4.1/mlflow/deployments/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/diviner.py` & `mlflow-skinny-2.4.1/mlflow/diviner.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/__init__.py` & `mlflow-skinny-2.4.1/mlflow/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/_mlflow_object.py` & `mlflow-skinny-2.4.1/mlflow/entities/_mlflow_object.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/dataset.py` & `mlflow-skinny-2.4.1/mlflow/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/dataset_input.py` & `mlflow-skinny-2.4.1/mlflow/entities/dataset_input.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/experiment.py` & `mlflow-skinny-2.4.1/mlflow/entities/experiment.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/experiment_tag.py` & `mlflow-skinny-2.4.1/mlflow/entities/experiment_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/file_info.py` & `mlflow-skinny-2.4.1/mlflow/entities/file_info.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/input_tag.py` & `mlflow-skinny-2.4.1/mlflow/entities/input_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/lifecycle_stage.py` & `mlflow-skinny-2.4.1/mlflow/entities/lifecycle_stage.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/metric.py` & `mlflow-skinny-2.4.1/mlflow/entities/metric.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/model_registry/__init__.py` & `mlflow-skinny-2.4.1/mlflow/entities/model_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/model_registry/model_version.py` & `mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/model_registry/model_version_stages.py` & `mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version_stages.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/model_registry/model_version_status.py` & `mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version_status.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/model_registry/model_version_tag.py` & `mlflow-skinny-2.4.1/mlflow/entities/model_registry/model_version_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/model_registry/registered_model.py` & `mlflow-skinny-2.4.1/mlflow/entities/model_registry/registered_model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/model_registry/registered_model_alias.py` & `mlflow-skinny-2.4.1/mlflow/entities/model_registry/registered_model_alias.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/model_registry/registered_model_tag.py` & `mlflow-skinny-2.4.1/mlflow/entities/model_registry/registered_model_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/param.py` & `mlflow-skinny-2.4.1/mlflow/entities/param.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/run.py` & `mlflow-skinny-2.4.1/mlflow/entities/run.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/run_data.py` & `mlflow-skinny-2.4.1/mlflow/entities/run_data.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/run_info.py` & `mlflow-skinny-2.4.1/mlflow/entities/run_info.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/run_inputs.py` & `mlflow-skinny-2.4.1/mlflow/entities/run_inputs.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/run_status.py` & `mlflow-skinny-2.4.1/mlflow/entities/run_status.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/run_tag.py` & `mlflow-skinny-2.4.1/mlflow/entities/run_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/source_type.py` & `mlflow-skinny-2.4.1/mlflow/entities/source_type.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/entities/view_type.py` & `mlflow-skinny-2.4.1/mlflow/entities/view_type.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/environment_variables.py` & `mlflow-skinny-2.4.1/mlflow/environment_variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,7 +262,12 @@
 #: Specifies the download options to be used by pip wheel when `add_libraries_to_model` is used to
 #: create and log model dependencies as model artifacts. The default behavior only uses dependency
 #: binaries and no source packages.
 #: (default: ``--only-binary=:all:``).
 MLFLOW_WHEELED_MODEL_PIP_DOWNLOAD_OPTIONS = _EnvironmentVariable(
     "MLFLOW_WHEELED_MODEL_PIP_DOWNLOAD_OPTIONS", str, "--only-binary=:all:"
 )
+
+# Specifies whether or not to use multipart download when downloading a large file on Databricks.
+MLFLOW_ENABLE_MULTIPART_DOWNLOAD = _BooleanEnvironmentVariable(
+    "MLFLOW_ENABLE_MULTIPART_DOWNLOAD", True
+)
```

### Comparing `mlflow-skinny-2.4.0/mlflow/exceptions.py` & `mlflow-skinny-2.4.1/mlflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/experiments.py` & `mlflow-skinny-2.4.1/mlflow/experiments.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/fastai/__init__.py` & `mlflow-skinny-2.4.1/mlflow/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/fastai/callback.py` & `mlflow-skinny-2.4.1/mlflow/fastai/callback.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/gluon/__init__.py` & `mlflow-skinny-2.4.1/mlflow/gluon/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/gluon/_autolog.py` & `mlflow-skinny-2.4.1/mlflow/gluon/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/h2o.py` & `mlflow-skinny-2.4.1/mlflow/h2o.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/langchain/__init__.py` & `mlflow-skinny-2.4.1/mlflow/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/langchain/api_request_parallel_processor.py` & `mlflow-skinny-2.4.1/mlflow/langchain/api_request_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/lightgbm.py` & `mlflow-skinny-2.4.1/mlflow/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/ml_package_versions.py` & `mlflow-skinny-2.4.1/mlflow/ml_package_versions.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/mleap.py` & `mlflow-skinny-2.4.1/mlflow/mleap.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/__init__.py` & `mlflow-skinny-2.4.1/mlflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/cli.py` & `mlflow-skinny-2.4.1/mlflow/models/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/container/__init__.py` & `mlflow-skinny-2.4.1/mlflow/models/container/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/docker_utils.py` & `mlflow-skinny-2.4.1/mlflow/models/docker_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/evaluation/_shap_patch.py` & `mlflow-skinny-2.4.1/mlflow/models/evaluation/_shap_patch.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/evaluation/artifacts.py` & `mlflow-skinny-2.4.1/mlflow/models/evaluation/artifacts.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/evaluation/base.py` & `mlflow-skinny-2.4.1/mlflow/models/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/evaluation/default_evaluator.py` & `mlflow-skinny-2.4.1/mlflow/models/evaluation/default_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/evaluation/evaluator_registry.py` & `mlflow-skinny-2.4.1/mlflow/models/evaluation/evaluator_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/evaluation/lift_curve.py` & `mlflow-skinny-2.4.1/mlflow/models/evaluation/lift_curve.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/evaluation/validation.py` & `mlflow-skinny-2.4.1/mlflow/models/evaluation/validation.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/flavor_backend.py` & `mlflow-skinny-2.4.1/mlflow/models/flavor_backend.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/flavor_backend_registry.py` & `mlflow-skinny-2.4.1/mlflow/models/flavor_backend_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/model.py` & `mlflow-skinny-2.4.1/mlflow/models/model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/signature.py` & `mlflow-skinny-2.4.1/mlflow/models/signature.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/utils.py` & `mlflow-skinny-2.4.1/mlflow/models/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/models/wheeled_model.py` & `mlflow-skinny-2.4.1/mlflow/models/wheeled_model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/onnx.py` & `mlflow-skinny-2.4.1/mlflow/onnx.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/openai/__init__.py` & `mlflow-skinny-2.4.1/mlflow/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/openai/api_request_parallel_processor.py` & `mlflow-skinny-2.4.1/mlflow/openai/api_request_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/openai/retry.py` & `mlflow-skinny-2.4.1/mlflow/openai/retry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/openai/utils.py` & `mlflow-skinny-2.4.1/mlflow/openai/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/paddle/__init__.py` & `mlflow-skinny-2.4.1/mlflow/paddle/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/paddle/_paddle_autolog.py` & `mlflow-skinny-2.4.1/mlflow/paddle/_paddle_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pmdarima.py` & `mlflow-skinny-2.4.1/mlflow/pmdarima.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/projects/__init__.py` & `mlflow-skinny-2.4.1/mlflow/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/projects/_project_spec.py` & `mlflow-skinny-2.4.1/mlflow/projects/_project_spec.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/projects/backend/abstract_backend.py` & `mlflow-skinny-2.4.1/mlflow/projects/backend/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/projects/backend/loader.py` & `mlflow-skinny-2.4.1/mlflow/projects/backend/loader.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/projects/backend/local.py` & `mlflow-skinny-2.4.1/mlflow/projects/backend/local.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/projects/databricks.py` & `mlflow-skinny-2.4.1/mlflow/projects/databricks.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/projects/docker.py` & `mlflow-skinny-2.4.1/mlflow/projects/docker.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/projects/kubernetes.py` & `mlflow-skinny-2.4.1/mlflow/projects/kubernetes.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/projects/submitted_run.py` & `mlflow-skinny-2.4.1/mlflow/projects/submitted_run.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/projects/utils.py` & `mlflow-skinny-2.4.1/mlflow/projects/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/prophet.py` & `mlflow-skinny-2.4.1/mlflow/prophet.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/protos/databricks_artifacts_pb2.py` & `mlflow-skinny-2.4.1/mlflow/protos/databricks_artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/protos/databricks_pb2.py` & `mlflow-skinny-2.4.1/mlflow/protos/databricks_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/protos/databricks_uc_registry_messages_pb2.py` & `mlflow-skinny-2.4.1/mlflow/protos/databricks_uc_registry_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/protos/databricks_uc_registry_service_pb2.py` & `mlflow-skinny-2.4.1/mlflow/protos/databricks_uc_registry_service_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/protos/facet_feature_statistics_pb2.py` & `mlflow-skinny-2.4.1/mlflow/protos/facet_feature_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/protos/internal_pb2.py` & `mlflow-skinny-2.4.1/mlflow/protos/internal_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/protos/mlflow_artifacts_pb2.py` & `mlflow-skinny-2.4.1/mlflow/protos/mlflow_artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/protos/model_registry_pb2.py` & `mlflow-skinny-2.4.1/mlflow/protos/model_registry_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/protos/scalapb/scalapb_pb2.py` & `mlflow-skinny-2.4.1/mlflow/protos/scalapb/scalapb_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/protos/service_pb2.py` & `mlflow-skinny-2.4.1/mlflow/protos/service_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pyfunc/__init__.py` & `mlflow-skinny-2.4.1/mlflow/pyfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pyfunc/backend.py` & `mlflow-skinny-2.4.1/mlflow/pyfunc/backend.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pyfunc/mlserver.py` & `mlflow-skinny-2.4.1/mlflow/pyfunc/mlserver.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pyfunc/model.py` & `mlflow-skinny-2.4.1/mlflow/pyfunc/model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pyfunc/scoring_server/__init__.py` & `mlflow-skinny-2.4.1/mlflow/pyfunc/scoring_server/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pyfunc/scoring_server/client.py` & `mlflow-skinny-2.4.1/mlflow/pyfunc/scoring_server/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pyfunc/spark_model_cache.py` & `mlflow-skinny-2.4.1/mlflow/pyfunc/spark_model_cache.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pyfunc/stdin_server.py` & `mlflow-skinny-2.4.1/mlflow/pyfunc/stdin_server.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pypi_package_index.json` & `mlflow-skinny-2.4.1/mlflow/pypi_package_index.json`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pyspark/ml/__init__.py` & `mlflow-skinny-2.4.1/mlflow/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pyspark/ml/_autolog.py` & `mlflow-skinny-2.4.1/mlflow/pyspark/ml/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pyspark/ml/log_model_allowlist.txt` & `mlflow-skinny-2.4.1/mlflow/pyspark/ml/log_model_allowlist.txt`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pytorch/__init__.py` & `mlflow-skinny-2.4.1/mlflow/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pytorch/_lightning_autolog.py` & `mlflow-skinny-2.4.1/mlflow/pytorch/_lightning_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pytorch/_pytorch_autolog.py` & `mlflow-skinny-2.4.1/mlflow/pytorch/_pytorch_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/pytorch/pickle_module.py` & `mlflow-skinny-2.4.1/mlflow/pytorch/pickle_module.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/__init__.py` & `mlflow-skinny-2.4.1/mlflow/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/artifacts.py` & `mlflow-skinny-2.4.1/mlflow/recipes/artifacts.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/cards/__init__.py` & `mlflow-skinny-2.4.1/mlflow/recipes/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/cards/histogram_generator.py` & `mlflow-skinny-2.4.1/mlflow/recipes/cards/histogram_generator.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/cards/pandas_renderer.py` & `mlflow-skinny-2.4.1/mlflow/recipes/cards/pandas_renderer.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/classification/v1/recipe.py` & `mlflow-skinny-2.4.1/mlflow/recipes/classification/v1/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/cli.py` & `mlflow-skinny-2.4.1/mlflow/recipes/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/dag_help_strings.py` & `mlflow-skinny-2.4.1/mlflow/recipes/dag_help_strings.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/recipe.py` & `mlflow-skinny-2.4.1/mlflow/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/regression/v1/recipe.py` & `mlflow-skinny-2.4.1/mlflow/recipes/regression/v1/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/step.py` & `mlflow-skinny-2.4.1/mlflow/recipes/step.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/steps/automl/flaml.py` & `mlflow-skinny-2.4.1/mlflow/recipes/steps/automl/flaml.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/steps/evaluate.py` & `mlflow-skinny-2.4.1/mlflow/recipes/steps/evaluate.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/steps/ingest/__init__.py` & `mlflow-skinny-2.4.1/mlflow/recipes/steps/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/steps/ingest/datasets.py` & `mlflow-skinny-2.4.1/mlflow/recipes/steps/ingest/datasets.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/steps/predict.py` & `mlflow-skinny-2.4.1/mlflow/recipes/steps/predict.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/steps/register.py` & `mlflow-skinny-2.4.1/mlflow/recipes/steps/register.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/steps/split.py` & `mlflow-skinny-2.4.1/mlflow/recipes/steps/split.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/steps/train.py` & `mlflow-skinny-2.4.1/mlflow/recipes/steps/train.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/steps/transform.py` & `mlflow-skinny-2.4.1/mlflow/recipes/steps/transform.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/utils/__init__.py` & `mlflow-skinny-2.4.1/mlflow/recipes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/utils/execution.py` & `mlflow-skinny-2.4.1/mlflow/recipes/utils/execution.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/utils/metrics.py` & `mlflow-skinny-2.4.1/mlflow/recipes/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/utils/step.py` & `mlflow-skinny-2.4.1/mlflow/recipes/utils/step.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/utils/tracking.py` & `mlflow-skinny-2.4.1/mlflow/recipes/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/recipes/utils/wrapped_recipe_model.py` & `mlflow-skinny-2.4.1/mlflow/recipes/utils/wrapped_recipe_model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/rfunc/__init__.py` & `mlflow-skinny-2.4.1/mlflow/rfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/rfunc/backend.py` & `mlflow-skinny-2.4.1/mlflow/rfunc/backend.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/runs.py` & `mlflow-skinny-2.4.1/mlflow/runs.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/sagemaker/__init__.py` & `mlflow-skinny-2.4.1/mlflow/sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/sagemaker/cli.py` & `mlflow-skinny-2.4.1/mlflow/sagemaker/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/sentence_transformers.py` & `mlflow-skinny-2.4.1/mlflow/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/server/__init__.py` & `mlflow-skinny-2.4.1/mlflow/server/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/server/auth/__init__.py` & `mlflow-skinny-2.4.1/mlflow/server/auth/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,17 @@
     else:
         raise MlflowException(
             f"Unsupported HTTP method '{request.method}'",
             BAD_REQUEST,
         )
 
     if param not in args:
+        # Special handling for run_id
+        if param == "run_id":
+            return _get_request_param("run_uuid")
         raise MlflowException(
             f"Missing value for required parameter '{param}'. "
             "See the API docs for more information about request parameters.",
             INVALID_PARAMETER_VALUE,
         )
     return args[param]
```

### Comparing `mlflow-skinny-2.4.0/mlflow/server/auth/client.py` & `mlflow-skinny-2.4.1/mlflow/server/auth/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/server/auth/config.py` & `mlflow-skinny-2.4.1/mlflow/server/auth/config.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/server/auth/entities.py` & `mlflow-skinny-2.4.1/mlflow/server/auth/entities.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/server/auth/logo.py` & `mlflow-skinny-2.4.1/mlflow/server/auth/logo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/server/auth/permissions.py` & `mlflow-skinny-2.4.1/mlflow/server/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/server/auth/routes.py` & `mlflow-skinny-2.4.1/mlflow/server/auth/routes.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/server/auth/sqlalchemy_store.py` & `mlflow-skinny-2.4.1/mlflow/server/auth/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/server/handlers.py` & `mlflow-skinny-2.4.1/mlflow/server/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1356,28 +1356,36 @@
     passed:
     "mlflow-artifacts://host:port/../../../../"
     "http://host:port/api/2.0/mlflow-artifacts/artifacts/../../../../"
     "https://host:port/api/2.0/mlflow-artifacts/artifacts/../../../../"
     "/models/artifacts/../../../"
     "s3:/my_bucket/models/path/../../other/path"
     "file://path/to/../../../../some/where/you/should/not/be"
+    "mlflow-artifacts://host:port/..%2f..%2f..%2f..%2f"
+    "http://host:port/api/2.0/mlflow-artifacts/artifacts%00"
     """
+    invalid_source_error_message = (
+        f"Invalid model version source: '{source}'. If supplying a source as an http, https, "
+        "local file path, ftp, objectstore, or mlflow-artifacts uri, an absolute path must be "
+        "provided without relative path references present. "
+        "Please provide an absolute path."
+    )
+
+    while (unquoted := urllib.parse.unquote_plus(source)) != source:
+        source = unquoted
     source_path = re.sub(r"/+", "/", urllib.parse.urlparse(source).path.rstrip("/"))
+    if "\x00" in source_path:
+        raise MlflowException(invalid_source_error_message, INVALID_PARAMETER_VALUE)
     resolved_source = pathlib.Path(source_path).resolve().as_posix()
     # NB: drive split is specifically for Windows since WindowsPath.resolve() will append the
     # drive path of the pwd to a given path. We don't care about the drive here, though.
     _, resolved_path = os.path.splitdrive(resolved_source)
 
     if resolved_path != source_path:
-        raise MlflowException(
-            f"Invalid model version source: '{source}'. If supplying a source as an http, https, "
-            "local file path, ftp, objectstore, or mlflow-artifacts uri, an absolute path must be "
-            "provided without relative path references present. Please provide an absolute path.",
-            INVALID_PARAMETER_VALUE,
-        )
+        raise MlflowException(invalid_source_error_message, INVALID_PARAMETER_VALUE)
 
 
 def _validate_source(source: str, run_id: str) -> None:
     if is_local_uri(source):
         if run_id:
             store = _get_tracking_store()
             run = store.get_run(run_id)
```

### Comparing `mlflow-skinny-2.4.0/mlflow/shap.py` & `mlflow-skinny-2.4.1/mlflow/shap.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/sklearn/__init__.py` & `mlflow-skinny-2.4.1/mlflow/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/sklearn/utils.py` & `mlflow-skinny-2.4.1/mlflow/sklearn/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/spacy.py` & `mlflow-skinny-2.4.1/mlflow/spacy.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/spark.py` & `mlflow-skinny-2.4.1/mlflow/spark.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/statsmodels.py` & `mlflow-skinny-2.4.1/mlflow/statsmodels.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/_unity_catalog/registry/rest_store.py` & `mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/registry/rest_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 import functools
 import logging
 import tempfile
 
 from mlflow.entities import Run
 from mlflow.protos.service_pb2 import GetRun, MlflowService
 from mlflow.protos.databricks_uc_registry_messages_pb2 import (
@@ -421,15 +422,19 @@
         source_workspace_id = self._get_workspace_id(headers)
         notebook_id = self._get_notebook_id(run)
         extra_headers = None
         if notebook_id is not None:
             notebook_entity = Notebook(id=str(notebook_id))
             entity = Entity(notebook=notebook_entity)
             lineage_header_info = LineageHeaderInfo(entities=[entity])
-            extra_headers = {_DATABRICKS_LINEAGE_ID_HEADER: message_to_json(lineage_header_info)}
+            # Base64-encode the header value to ensure it's valid ASCII,
+            # similar to JWT (see https://stackoverflow.com/a/40347926)
+            header_json = message_to_json(lineage_header_info)
+            header_base64 = base64.b64encode(header_json.encode())
+            extra_headers = {_DATABRICKS_LINEAGE_ID_HEADER: header_base64}
         full_name = get_full_name_from_sc(name, self.spark)
         req_body = message_to_json(
             CreateModelVersionRequest(
                 name=full_name,
                 source=source,
                 run_id=run_id,
                 description=description,
```

### Comparing `mlflow-skinny-2.4.0/mlflow/store/_unity_catalog/registry/utils.py` & `mlflow-skinny-2.4.1/mlflow/store/_unity_catalog/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/artifact_repository_registry.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/artifact_repository_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/azure_blob_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/azure_blob_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/azure_data_lake_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/azure_data_lake_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/cli.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/databricks_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/databricks_artifact_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
     get_databricks_profile_uri_from_artifact_uri,
     is_databricks_acled_artifacts_uri,
     is_valid_dbfs_uri,
     remove_databricks_profile_info_from_artifact_uri,
 )
 
 _logger = logging.getLogger(__name__)
-_DOWNLOAD_CHUNK_SIZE = 10_000_000  # 10 MB
+_DOWNLOAD_CHUNK_SIZE = 100_000_000  # 100 MB
+_MULTIPART_DOWNLOAD_MINIMUM_FILE_SIZE = 500_000_000  # 500 MB
 _MULTIPART_UPLOAD_CHUNK_SIZE = 10_000_000  # 10 MB
 _MAX_CREDENTIALS_REQUEST_SIZE = 2000  # Max number of artifact paths in a single credentials request
 _SERVICE_AND_METHOD_TO_INFO = {
     service: extract_api_info_for_service(service, _REST_API_PATH_PREFIX)
     for service in [MlflowService, DatabricksMlflowArtifactsService]
 }
 _ARTIFACT_UPLOAD_BATCH_SIZE = (
@@ -144,19 +145,19 @@
         run_relative_root_path = posixpath.relpath(
             path=artifact_repo_root_path, start=run_artifact_root_path
         )
         # If the paths are equal, then use empty string over "./" for ListArtifact compatibility.
         self.run_relative_artifact_repo_root_path = (
             "" if run_artifact_root_path == artifact_repo_root_path else run_relative_root_path
         )
-        # Use an isolated thread pool executor for chunk uploads to avoid a deadlock
-        # caused by waiting for a chunk-upload task within a file-upload task.
+        # Use an isolated thread pool executor for chunk uploads/downloads to avoid a deadlock
+        # caused by waiting for a chunk-upload/download task within a file-upload/download task.
         # See https://superfastpython.com/threadpoolexecutor-deadlock/#Deadlock_1_Submit_and_Wait_for_a_Task_Within_a_Task
         # for more details
-        self.chunk_upload_thread_pool = self._create_thread_pool()
+        self.chunk_thread_pool = self._create_thread_pool()
 
     @staticmethod
     def _extract_run_id(artifact_uri):
         """
         The artifact_uri is expected to be
         dbfs:/databricks/mlflow-tracking/<EXP_ID>/<RUN_ID>/artifacts/<path>
         Once the path from the input uri is extracted and normalized, it is
@@ -269,15 +270,15 @@
         """
         try:
             headers = self._extract_headers_from_credentials(credentials.headers)
             futures = {}
             num_chunks = _compute_num_chunks(local_file, _MULTIPART_UPLOAD_CHUNK_SIZE)
             for index in range(num_chunks):
                 start_byte = index * _MULTIPART_UPLOAD_CHUNK_SIZE
-                future = self.chunk_upload_thread_pool.submit(
+                future = self.chunk_thread_pool.submit(
                     self._azure_upload_chunk,
                     credentials=credentials,
                     headers=headers,
                     local_file=local_file,
                     artifact_path=artifact_path,
                     start_byte=start_byte,
                     size=_MULTIPART_UPLOAD_CHUNK_SIZE,
@@ -347,15 +348,15 @@
             # next try to append the file
             futures = {}
             file_size = os.path.getsize(local_file)
             num_chunks = _compute_num_chunks(local_file, _MULTIPART_UPLOAD_CHUNK_SIZE)
             use_single_part_upload = num_chunks == 1
             for index in range(num_chunks):
                 start_byte = index * _MULTIPART_UPLOAD_CHUNK_SIZE
-                future = self.chunk_upload_thread_pool.submit(
+                future = self.chunk_thread_pool.submit(
                     self._retryable_adls_function,
                     func=patch_adls_file_upload,
                     artifact_path=artifact_path,
                     sas_url=credentials.signed_uri,
                     local_file=local_file,
                     start_byte=start_byte,
                     size=_MULTIPART_UPLOAD_CHUNK_SIZE,
@@ -428,21 +429,29 @@
             raise MlflowException(
                 message="Cloud provider not supported.", error_code=INTERNAL_ERROR
             )
 
     def _parallelized_download_from_cloud(
         self, cloud_credential_info, file_size, dst_local_file_path, dst_run_relative_artifact_path
     ):
+        from mlflow.utils.databricks_utils import get_databricks_env_vars
+
         try:
+            parallel_download_subproc_env = os.environ.copy()
+            parallel_download_subproc_env.update(
+                get_databricks_env_vars(self.databricks_profile_uri)
+            )
             failed_downloads = parallelized_download_file_using_http_uri(
+                thread_pool_executor=self.chunk_thread_pool,
                 http_uri=cloud_credential_info.signed_uri,
                 download_path=dst_local_file_path,
                 file_size=file_size,
                 uri_type=cloud_credential_info.type,
                 chunk_size=_DOWNLOAD_CHUNK_SIZE,
+                env=parallel_download_subproc_env,
                 headers=self._extract_headers_from_credentials(cloud_credential_info.headers),
             )
             download_errors = [
                 e for e in failed_downloads.values() if e["error_status_code"] not in (401, 403)
             ]
             if download_errors:
                 raise MlflowException(
@@ -452,22 +461,19 @@
 
             if failed_downloads:
                 new_cloud_creds = self._get_read_credential_infos(
                     self.run_id, [dst_run_relative_artifact_path]
                 )[0]
                 new_signed_uri = new_cloud_creds.signed_uri
                 new_headers = self._extract_headers_from_credentials(new_cloud_creds.headers)
-                for index in failed_downloads:
-                    download_chunk(
-                        index,
-                        _DOWNLOAD_CHUNK_SIZE,
-                        new_headers,
-                        dst_local_file_path,
-                        new_signed_uri,
-                    )
+
+            for i in failed_downloads:
+                download_chunk(
+                    i, _DOWNLOAD_CHUNK_SIZE, new_headers, dst_local_file_path, new_signed_uri
+                )
         except Exception as err:
             if os.path.exists(dst_local_file_path):
                 os.remove(dst_local_file_path)
             raise MlflowException(err)
 
     def _download_from_cloud(self, cloud_credential_info, dst_local_file_path):
         """
@@ -564,15 +570,15 @@
             return self._upload_part(resp.upload_credential_info, data)
 
     def _upload_parts(self, local_file, create_mpu_resp):
         futures = {}
         for index, cred_info in enumerate(create_mpu_resp.upload_credential_infos):
             part_number = index + 1
             start_byte = index * _MULTIPART_UPLOAD_CHUNK_SIZE
-            future = self.chunk_upload_thread_pool.submit(
+            future = self.chunk_thread_pool.submit(
                 self._upload_part_retry,
                 cred_info=cred_info,
                 upload_id=create_mpu_resp.upload_id,
                 part_number=part_number,
                 local_file=local_file,
                 start_byte=start_byte,
                 size=_MULTIPART_UPLOAD_CHUNK_SIZE,
@@ -773,15 +779,15 @@
         # contained by the parent directory. A bad path could result in there being
         # no matching FileInfos (by path), so fall back to None size to prevent
         # parallelized download.
         parent_dir = posixpath.dirname(remote_file_path)
         file_infos = self.list_artifacts(parent_dir)
         file_info = [info for info in file_infos if info.path == remote_file_path]
         file_size = file_info[0].file_size if len(file_info) == 1 else None
-        if not file_size or file_size <= _DOWNLOAD_CHUNK_SIZE:
+        if not file_size or file_size < _MULTIPART_DOWNLOAD_MINIMUM_FILE_SIZE:
             self._download_from_cloud(
                 cloud_credential_info=read_credentials[0], dst_local_file_path=local_path
             )
         else:
             self._parallelized_download_from_cloud(
                 read_credentials[0], file_size, local_path, remote_file_path
             )
```

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/databricks_models_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/databricks_models_artifact_repo.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 import posixpath
 
 import mlflow.tracking
 from mlflow.entities import FileInfo
 from mlflow.exceptions import MlflowException
 from mlflow.protos.databricks_pb2 import INVALID_PARAMETER_VALUE
 from mlflow.store.artifact.artifact_repo import ArtifactRepository
-from mlflow.store.artifact.databricks_artifact_repo import _DOWNLOAD_CHUNK_SIZE
 from mlflow.utils.databricks_utils import get_databricks_host_creds
 from mlflow.utils.file_utils import (
     download_file_using_http_uri,
     parallelized_download_file_using_http_uri,
 )
 from mlflow.utils.rest_utils import http_request
 from mlflow.utils.request_utils import download_chunk
 from mlflow.utils.uri import get_databricks_profile_uri_from_artifact_uri
 from mlflow.store.artifact.utils.models import (
     get_model_name_and_version,
     is_using_databricks_registry,
 )
+from mlflow.environment_variables import MLFLOW_ENABLE_MULTIPART_DOWNLOAD
 
 _logger = logging.getLogger(__name__)
+_DOWNLOAD_CHUNK_SIZE = 500_000_000  # 500 MB
 # The constant REGISTRY_LIST_ARTIFACT_ENDPOINT is defined as @developer_stable
 REGISTRY_LIST_ARTIFACTS_ENDPOINT = "/api/2.0/mlflow/model-versions/list-artifacts"
 # The constant REGISTRY_ARTIFACT_PRESIGNED_URI_ENDPOINT is defined as @developer_stable
 REGISTRY_ARTIFACT_PRESIGNED_URI_ENDPOINT = "/api/2.0/mlflow/model-versions/get-signed-download-uri"
 
 
 class DatabricksModelsArtifactRepository(ArtifactRepository):
@@ -56,14 +57,19 @@
         from mlflow.tracking.client import MlflowClient
 
         self.databricks_profile_uri = (
             get_databricks_profile_uri_from_artifact_uri(artifact_uri) or mlflow.get_registry_uri()
         )
         client = MlflowClient(registry_uri=self.databricks_profile_uri)
         self.model_name, self.model_version = get_model_name_and_version(client, artifact_uri)
+        # Use an isolated thread pool executor for chunk uploads/downloads to avoid a deadlock
+        # caused by waiting for a chunk-upload/download task within a file-upload/download task.
+        # See https://superfastpython.com/threadpoolexecutor-deadlock/#Deadlock_1_Submit_and_Wait_for_a_Task_Within_a_Task
+        # for more details
+        self.chunk_thread_pool = self._create_thread_pool()
 
     def _call_endpoint(self, json, endpoint):
         db_creds = get_databricks_host_creds(self.databricks_profile_uri)
         return http_request(host_creds=db_creds, endpoint=endpoint, method="GET", params=json)
 
     def _make_json_body(self, path, page_token=None):
         body = {"name": self.model_name, "version": self.model_version, "path": path}
@@ -124,41 +130,48 @@
     def _extract_headers_from_signed_url(self, headers):
         filtered_headers = filter(lambda h: "name" in h and "value" in h, headers)
         return {header.get("name"): header.get("value") for header in filtered_headers}
 
     def _parallelized_download_from_cloud(
         self, signed_uri, headers, file_size, dst_local_file_path, dst_run_relative_artifact_path
     ):
+        from mlflow.utils.databricks_utils import get_databricks_env_vars
+
         try:
+            parallel_download_subproc_env = os.environ.copy()
+            parallel_download_subproc_env.update(
+                get_databricks_env_vars(self.databricks_profile_uri)
+            )
             failed_downloads = parallelized_download_file_using_http_uri(
+                thread_pool_executor=self.chunk_thread_pool,
                 http_uri=signed_uri,
                 download_path=dst_local_file_path,
                 file_size=file_size,
                 # URI type is not known in this context
                 uri_type=None,
                 chunk_size=_DOWNLOAD_CHUNK_SIZE,
+                env=parallel_download_subproc_env,
                 headers=headers,
             )
-            if any(e.response.status_code not in (401, 403) for e in failed_downloads.values()):
+            download_errors = [
+                e for e in failed_downloads.values() if e["error_status_code"] not in (401, 403)
+            ]
+            if download_errors:
                 raise MlflowException(
                     f"Failed to download artifact {dst_run_relative_artifact_path}: "
-                    f"{failed_downloads}"
+                    f"{download_errors}"
                 )
             if failed_downloads:
                 new_signed_uri, new_headers = self._get_signed_download_uri(
                     dst_run_relative_artifact_path
                 )
-                for index in failed_downloads:
-                    download_chunk(
-                        index=index,
-                        chunk_size=_DOWNLOAD_CHUNK_SIZE,
-                        headers=new_headers,
-                        download_path=dst_local_file_path,
-                        http_uri=new_signed_uri,
-                    )
+            for i in failed_downloads:
+                download_chunk(
+                    i, _DOWNLOAD_CHUNK_SIZE, new_headers, dst_local_file_path, new_signed_uri
+                )
         except Exception as err:
             if os.path.exists(dst_local_file_path):
                 os.remove(dst_local_file_path)
             raise MlflowException(err)
 
     def _download_file(self, remote_file_path, local_path):
         try:
@@ -167,15 +180,19 @@
             file_info = [info for info in file_infos if info.path == remote_file_path]
             file_size = file_info[0].file_size if len(file_info) == 1 else None
             signed_uri, raw_headers = self._get_signed_download_uri(remote_file_path)
             headers = {}
             if raw_headers is not None:
                 # Don't send None to _extract_headers_from_signed_url
                 headers = self._extract_headers_from_signed_url(raw_headers)
-            if not file_size or file_size <= _DOWNLOAD_CHUNK_SIZE:
+            if (
+                not file_size
+                or file_size <= _DOWNLOAD_CHUNK_SIZE
+                or not MLFLOW_ENABLE_MULTIPART_DOWNLOAD.get()
+            ):
                 download_file_using_http_uri(signed_uri, local_path, _DOWNLOAD_CHUNK_SIZE, headers)
             else:
                 self._parallelized_download_from_cloud(
                     signed_uri,
                     headers,
                     file_size,
                     local_path,
```

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/dbfs_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/dbfs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/ftp_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/ftp_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/gcs_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/gcs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/hdfs_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/hdfs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/http_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/http_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/local_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/local_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/mlflow_artifacts_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/mlflow_artifacts_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/models_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/runs_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/runs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/s3_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/s3_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/sftp_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/sftp_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/unity_catalog_models_artifact_repo.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/unity_catalog_models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/artifact/utils/models.py` & `mlflow-skinny-2.4.1/mlflow/store/artifact/utils/models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db/utils.py` & `mlflow-skinny-2.4.1/mlflow/store/db/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/alembic.ini` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/env.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/env.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py` & `mlflow-skinny-2.4.1/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/model_registry/__init__.py` & `mlflow-skinny-2.4.1/mlflow/store/model_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/model_registry/abstract_store.py` & `mlflow-skinny-2.4.1/mlflow/store/model_registry/abstract_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/model_registry/base_rest_store.py` & `mlflow-skinny-2.4.1/mlflow/store/model_registry/base_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/model_registry/dbmodels/models.py` & `mlflow-skinny-2.4.1/mlflow/store/model_registry/dbmodels/models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/model_registry/file_store.py` & `mlflow-skinny-2.4.1/mlflow/store/model_registry/file_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/model_registry/rest_store.py` & `mlflow-skinny-2.4.1/mlflow/store/model_registry/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/model_registry/sqlalchemy_store.py` & `mlflow-skinny-2.4.1/mlflow/store/model_registry/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/tracking/__init__.py` & `mlflow-skinny-2.4.1/mlflow/store/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/tracking/abstract_store.py` & `mlflow-skinny-2.4.1/mlflow/store/tracking/abstract_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/tracking/dbmodels/initial_models.py` & `mlflow-skinny-2.4.1/mlflow/store/tracking/dbmodels/initial_models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/tracking/dbmodels/models.py` & `mlflow-skinny-2.4.1/mlflow/store/tracking/dbmodels/models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/tracking/file_store.py` & `mlflow-skinny-2.4.1/mlflow/store/tracking/file_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/tracking/rest_store.py` & `mlflow-skinny-2.4.1/mlflow/store/tracking/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/store/tracking/sqlalchemy_store.py` & `mlflow-skinny-2.4.1/mlflow/store/tracking/sqlalchemy_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import threading
 from functools import reduce
 from typing import List, Optional
 
 import math
 import sqlalchemy
 import sqlalchemy.sql.expression as sql
-from sqlalchemy import sql
+from sqlalchemy import and_, sql, text
 from sqlalchemy.future import select
 
 from mlflow.entities import RunTag, Metric, DatasetInput
 from mlflow.entities.lifecycle_stage import LifecycleStage
 from mlflow.store.tracking import SEARCH_MAX_RESULTS_DEFAULT, SEARCH_MAX_RESULTS_THRESHOLD
 from mlflow.store.db.db_types import MYSQL, MSSQL
 import mlflow.store.db.utils
@@ -57,15 +57,20 @@
     _validate_metric,
     _validate_experiment_tag,
     _validate_tag,
     _validate_param_keys_unique,
     _validate_param,
     _validate_experiment_name,
 )
-from mlflow.utils.mlflow_tags import MLFLOW_LOGGED_MODELS, MLFLOW_RUN_NAME, _get_run_name_from_tags
+from mlflow.utils.mlflow_tags import (
+    MLFLOW_DATASET_CONTEXT,
+    MLFLOW_LOGGED_MODELS,
+    MLFLOW_RUN_NAME,
+    _get_run_name_from_tags,
+)
 from mlflow.utils.time_utils import get_current_time_millis
 
 _logger = logging.getLogger(__name__)
 
 # For each database table, fetch its columns and define an appropriate attribute for each column
 # on the table's associated object representation (Mapper). This is necessary to ensure that
 # columns defined via backreference are available as Mapper instance attributes (e.g.,
@@ -1208,19 +1213,27 @@
             # tags. These run attributes are referenced during the invocation of
             # ``run.to_mlflow_entity()``, so eager loading helps avoid additional database queries
             # that are otherwise executed at attribute access time under a lazy loading model.
             parsed_filters = SearchUtils.parse_search_filter(filter_string)
             cases_orderby, parsed_orderby, sorting_joins = _get_orderby_clauses(order_by, session)
 
             stmt = select(SqlRun, *cases_orderby)
-            attribute_filters, non_attribute_filters = _get_sqlalchemy_filter_clauses(
-                parsed_filters, session, self._get_dialect()
-            )
+            (
+                attribute_filters,
+                non_attribute_filters,
+                dataset_filters,
+            ) = _get_sqlalchemy_filter_clauses(parsed_filters, session, self._get_dialect())
             for non_attr_filter in non_attribute_filters:
                 stmt = stmt.join(non_attr_filter)
+            for idx, dataset_filter in enumerate(dataset_filters):
+                # need to reference the anon table in the join condition
+                anon_table_name = f"anon_{idx+1}"
+                stmt = stmt.join(
+                    dataset_filter, text(f"runs.run_uuid = {anon_table_name}.destination_id")
+                )
             # using an outer join is necessary here because we want to be able to sort
             # on a column (tag, metric or param) without removing the lines that
             # do not have a value for this column (which is what inner join would do)
             for j in sorting_joins:
                 stmt = stmt.outerjoin(j)
 
             offset = SearchUtils.parse_start_offset_from_page_token(page_token)
@@ -1455,14 +1468,15 @@
 def _get_sqlalchemy_filter_clauses(parsed, session, dialect):
     """
     Creates run attribute filters and subqueries that will be inner-joined to SqlRun to act as
     multi-clause filters and return them as a tuple.
     """
     attribute_filters = []
     non_attribute_filters = []
+    dataset_filters = []
 
     for sql_statement in parsed:
         key_type = sql_statement.get("type")
         key_name = sql_statement.get("key")
         value = sql_statement.get("value")
         comparator = sql_statement.get("comparator").upper()
 
@@ -1493,29 +1507,59 @@
             if SearchUtils.is_metric(key_type, comparator):
                 entity = SqlLatestMetric
                 value = float(value)
             elif SearchUtils.is_param(key_type, comparator):
                 entity = SqlParam
             elif SearchUtils.is_tag(key_type, comparator):
                 entity = SqlTag
+            elif SearchUtils.is_dataset(key_type, comparator):
+                entity = SqlDataset
             else:
                 raise MlflowException(
                     "Invalid search expression type '%s'" % key_type,
                     error_code=INVALID_PARAMETER_VALUE,
                 )
 
-            key_filter = SearchUtils.get_sql_comparison_func("=", dialect)(entity.key, key_name)
-            val_filter = SearchUtils.get_sql_comparison_func(comparator, dialect)(
-                entity.value, value
-            )
-            non_attribute_filters.append(
-                session.query(entity).filter(key_filter, val_filter).subquery()
-            )
+            if entity == SqlDataset:
+                if key_name == "context":
+                    dataset_filters.append(
+                        session.query(entity, SqlInput, SqlInputTag)
+                        .join(SqlInput, SqlInput.source_id == SqlDataset.dataset_uuid)
+                        .join(
+                            SqlInputTag,
+                            and_(
+                                SqlInputTag.input_uuid == SqlInput.input_uuid,
+                                SqlInputTag.name == MLFLOW_DATASET_CONTEXT,
+                                SearchUtils.get_sql_comparison_func(comparator, dialect)(
+                                    getattr(SqlInputTag, "value"), value
+                                ),
+                            ),
+                        )
+                        .subquery()
+                    )
+                else:
+                    dataset_attr_filter = SearchUtils.get_sql_comparison_func(comparator, dialect)(
+                        getattr(SqlDataset, key_name), value
+                    )
+                    dataset_filters.append(
+                        session.query(entity, SqlInput)
+                        .join(SqlInput, SqlInput.source_id == SqlDataset.dataset_uuid)
+                        .filter(dataset_attr_filter)
+                        .subquery()
+                    )
+            else:
+                key_filter = SearchUtils.get_sql_comparison_func("=", dialect)(entity.key, key_name)
+                val_filter = SearchUtils.get_sql_comparison_func(comparator, dialect)(
+                    entity.value, value
+                )
+                non_attribute_filters.append(
+                    session.query(entity).filter(key_filter, val_filter).subquery()
+                )
 
-    return attribute_filters, non_attribute_filters
+    return attribute_filters, non_attribute_filters, dataset_filters
 
 
 def _get_orderby_clauses(order_by_list, session):
     """Sorts a set of runs based on their natural ordering and an overriding set of order_bys.
     Runs are naturally ordered first by start time descending, then by run id for tie-breaking.
     """
```

### Comparing `mlflow-skinny-2.4.0/mlflow/tensorflow/__init__.py` & `mlflow-skinny-2.4.1/mlflow/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tensorflow/_autolog.py` & `mlflow-skinny-2.4.1/mlflow/tensorflow/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/__init__.py` & `mlflow-skinny-2.4.1/mlflow/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/_model_registry/client.py` & `mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/_model_registry/fluent.py` & `mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/fluent.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/_model_registry/registry.py` & `mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/_model_registry/utils.py` & `mlflow-skinny-2.4.1/mlflow/tracking/_model_registry/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/_tracking_service/client.py` & `mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/_tracking_service/registry.py` & `mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/_tracking_service/utils.py` & `mlflow-skinny-2.4.1/mlflow/tracking/_tracking_service/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/artifact_utils.py` & `mlflow-skinny-2.4.1/mlflow/tracking/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/client.py` & `mlflow-skinny-2.4.1/mlflow/tracking/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/context/abstract_context.py` & `mlflow-skinny-2.4.1/mlflow/tracking/context/abstract_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/context/databricks_cluster_context.py` & `mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_cluster_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/context/databricks_command_context.py` & `mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_command_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/context/databricks_job_context.py` & `mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_job_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/context/databricks_notebook_context.py` & `mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_notebook_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/context/databricks_repo_context.py` & `mlflow-skinny-2.4.1/mlflow/tracking/context/databricks_repo_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/context/default_context.py` & `mlflow-skinny-2.4.1/mlflow/tracking/context/default_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/context/git_context.py` & `mlflow-skinny-2.4.1/mlflow/tracking/context/git_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/context/registry.py` & `mlflow-skinny-2.4.1/mlflow/tracking/context/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/default_experiment/abstract_context.py` & `mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/abstract_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py` & `mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py` & `mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/default_experiment/registry.py` & `mlflow-skinny-2.4.1/mlflow/tracking/default_experiment/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/fluent.py` & `mlflow-skinny-2.4.1/mlflow/tracking/fluent.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/llm_utils.py` & `mlflow-skinny-2.4.1/mlflow/tracking/llm_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/metric_value_conversion_utils.py` & `mlflow-skinny-2.4.1/mlflow/tracking/metric_value_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/registry.py` & `mlflow-skinny-2.4.1/mlflow/tracking/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/request_header/abstract_request_header_provider.py` & `mlflow-skinny-2.4.1/mlflow/tracking/request_header/abstract_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/request_header/databricks_request_header_provider.py` & `mlflow-skinny-2.4.1/mlflow/tracking/request_header/databricks_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/tracking/request_header/registry.py` & `mlflow-skinny-2.4.1/mlflow/tracking/request_header/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/transformers.py` & `mlflow-skinny-2.4.1/mlflow/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from mlflow.utils.annotations import experimental
 from mlflow.utils.autologging_utils import autologging_integration, safe_patch
 from mlflow.utils.docstring_utils import (
     format_docstring,
     LOG_MODEL_PARAM_DOCS,
     docstring_version_compatibility_warning,
 )
+from mlflow.utils.environment import _find_duplicate_requirements
 from mlflow.environment_variables import (
     MLFLOW_DEFAULT_PREDICTION_DEVICE,
     MLFLOW_HUGGINGFACE_DISABLE_ACCELERATE_FEATURES,
     MLFLOW_HUGGINGFACE_USE_DEVICE_MAP,
     MLFLOW_HUGGINGFACE_DEVICE_MAP_STRATEGY,
     MLFLOW_HUGGINGFACE_USE_LOW_CPU_MEM_USAGE,
     MLFLOW_HUGGINGFACE_MODEL_MAX_SHARD_SIZE,
@@ -443,18 +444,15 @@
             inference_config=inference_config,
         )
 
     # Get the model card from either the argument or the HuggingFace marketplace
     card_data = model_card if model_card is not None else _fetch_model_card(transformers_model)
 
     # If the card data can be acquired, save the text and the data separately
-    if card_data:
-        path.joinpath(_CARD_TEXT_FILE_NAME).write_text(card_data.text)
-        with path.joinpath(_CARD_DATA_FILE_NAME).open("w") as file:
-            yaml.safe_dump(card_data.data.to_dict(), stream=file, default_flow_style=False)
+    _write_card_data(card_data, path)
 
     model_bin_kwargs = {_MODEL_BINARY_KEY: _MODEL_BINARY_FILE_NAME}
 
     # Only allow a subset of task types to have a pyfunc definition.
     # Currently supported types are NLP-based language tasks which have a pipeline definition
     # consisting exclusively of a Model and a Tokenizer.
     if _should_add_pyfunc_to_model(built_pipeline):
@@ -501,14 +499,22 @@
             default_reqs = None
         conda_env, pip_requirements, pip_constraints = _process_pip_requirements(
             default_reqs, pip_requirements, extra_pip_requirements
         )
     else:
         conda_env, pip_requirements, pip_constraints = _process_conda_env(conda_env)
 
+    if duplicates := _find_duplicate_requirements(pip_requirements):
+        _logger.warning(
+            "Duplicate packages are present within the pip requirements. Duplicate packages: "
+            f"{duplicates}. Please manually specify the requirements by using the "
+            "`pip_requirements` argument in order to prevent unexpected installation "
+            "issues for this model."
+        )
+
     with path.joinpath(_CONDA_ENV_FILE_NAME).open("w") as f:
         yaml.safe_dump(conda_env, stream=f, default_flow_style=False)
 
     if pip_constraints:
         write_to(str(path.joinpath(_CONSTRAINTS_FILE_NAME)), "\n".join(pip_constraints))
 
     write_to(str(path.joinpath(_REQUIREMENTS_FILE_NAME)), "\n".join(pip_requirements))
@@ -992,14 +998,30 @@
         _logger.warning(
             f"The version of huggingface_hub that is installed does not provide "
             f"ModelCard functionality. You have version {hub.__version__} installed. "
             f"Update huggingface_hub to >= '0.10.0' to retrieve the ModelCard data."
         )
 
 
+def _write_card_data(card_data, path):
+    """
+    Writes the card data, if specified or available, to the provided path in two separate files
+    """
+    if card_data:
+        try:
+            path.joinpath(_CARD_TEXT_FILE_NAME).write_text(card_data.text, encoding="utf-8")
+        except UnicodeError as e:
+            _logger.warning(f"Unable to save the model card text due to: {e}")
+
+        with path.joinpath(_CARD_DATA_FILE_NAME).open("w") as file:
+            yaml.safe_dump(
+                card_data.data.to_dict(), stream=file, default_flow_style=False, encoding="utf-8"
+            )
+
+
 def _build_pipeline_from_model_input(model, task: str):
     """
     Utility for generating a pipeline from component parts. If required components are not
     specified, use the transformers library pipeline component validation to force raising an
     exception. The underlying Exception thrown in transformers is verbose enough for diagnosis.
     """
     from transformers import pipeline
```

### Comparing `mlflow-skinny-2.4.0/mlflow/types/schema.py` & `mlflow-skinny-2.4.1/mlflow/types/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from enum import Enum
 
 import numpy as np
 import string
 from typing import Dict, Any, List, Union, Optional
 
 from mlflow.exceptions import MlflowException
+from mlflow.utils.annotations import experimental
 
 
 class DataType(Enum):
     """
     MLflow data types.
     """
 
@@ -95,14 +96,15 @@
         return self._type
 
     @property
     def name(self) -> Optional[str]:
         """The column name or None if the columns is unnamed."""
         return self._name
 
+    @experimental
     @property
     def optional(self) -> bool:
         """Whether this column is optional."""
         return self._optional
 
     def to_dict(self) -> Dict[str, Any]:
         d = {"type": self.type.name}
@@ -219,17 +221,18 @@
         return self._name
 
     @property
     def shape(self) -> tuple:
         """The tensor shape"""
         return self._tensorInfo.shape
 
+    @experimental
     @property
     def optional(self) -> bool:
-        """Whether this column is optional."""
+        """Whether this tensor is optional."""
         return False
 
     def to_dict(self) -> Dict[str, Any]:
         if self.name is None:
             return {"type": "tensor", "tensor-spec": self._tensorInfo.to_dict()}
         else:
             return {"name": self.name, "type": "tensor", "tensor-spec": self._tensorInfo.to_dict()}
@@ -326,14 +329,15 @@
         """Get list of data names or range of indices if the schema has no names."""
         return [x.name or i for i, x in enumerate(self.inputs)]
 
     def required_input_names(self) -> List[Union[str, int]]:
         """Get list of required data names or range of indices if schema has no names."""
         return [x.name or i for i, x in enumerate(self.inputs) if not x.optional]
 
+    @experimental
     def optional_input_names(self) -> List[Union[str, int]]:
         """Get list of optional data names or range of indices if schema has no names."""
         return [x.name or i for i, x in enumerate(self.inputs) if x.optional]
 
     def has_input_names(self) -> bool:
         """Return true iff this schema declares names, false otherwise."""
         return self.inputs and self.inputs[0].name is not None
```

### Comparing `mlflow-skinny-2.4.0/mlflow/types/utils.py` & `mlflow-skinny-2.4.1/mlflow/types/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/__init__.py` & `mlflow-skinny-2.4.1/mlflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/_capture_modules.py` & `mlflow-skinny-2.4.1/mlflow/utils/_capture_modules.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/_capture_transformers_modules.py` & `mlflow-skinny-2.4.1/mlflow/utils/_capture_transformers_modules.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/_spark_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/_spark_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/annotations.py` & `mlflow-skinny-2.4.1/mlflow/utils/annotations.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/__init__.py` & `mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/client.py` & `mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/events.py` & `mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/events.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/logging_and_warnings.py` & `mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/logging_and_warnings.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/safety.py` & `mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/safety.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/autologging_utils/versioning.py` & `mlflow-skinny-2.4.1/mlflow/utils/autologging_utils/versioning.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/cli_args.py` & `mlflow-skinny-2.4.1/mlflow/utils/cli_args.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/conda.py` & `mlflow-skinny-2.4.1/mlflow/utils/conda.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/databricks_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/databricks_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/docstring_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/docstring_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/environment.py` & `mlflow-skinny-2.4.1/mlflow/utils/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import Counter
 import yaml
 import os
 import logging
 import re
 import hashlib
 from packaging.requirements import Requirement, InvalidRequirement
 from packaging.version import Version
@@ -496,14 +497,34 @@
         pip_reqs.append(f"-c {_CONSTRAINTS_FILE_NAME}")
 
     # Set `install_mlflow` to False because `pip_reqs` already contains `mlflow`
     conda_env = _mlflow_conda_env(additional_pip_deps=pip_reqs, install_mlflow=False)
     return conda_env, pip_reqs, constraints
 
 
+def _find_duplicate_requirements(requirements):
+    """
+    Checks if duplicate base package requirements are specified in any list of requirements
+    and returns the list of duplicate base package names.
+    Note that git urls and paths to local files are not being considered for duplication checking.
+    """
+    base_package_names = []
+
+    for package in requirements:
+        try:
+            base_package_names.append(Requirement(package).name)
+        except InvalidRequirement:
+            # Skip anything that's not a valid package requirement
+            continue
+
+    package_counts = Counter(base_package_names)
+    duplicates = [package for package, count in package_counts.items() if count > 1]
+    return duplicates
+
+
 def _process_conda_env(conda_env):
     """
     Processes `conda_env` passed to `mlflow.*.save_model` or `mlflow.*.log_model`, and returns
     a tuple of (conda_env, pip_requirements, pip_constraints).
     """
     if isinstance(conda_env, str):
         with open(conda_env) as f:
```

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/file_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/file_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 import posixpath
 import shutil
 import sys
 import tarfile
 import tempfile
 import stat
 import pathlib
-from concurrent.futures import ThreadPoolExecutor, as_completed
+from concurrent.futures import as_completed
 from contextlib import contextmanager
 import uuid
 import fnmatch
 
 import urllib.parse
 import urllib.request
 from urllib.parse import unquote
 from urllib.request import pathname2url
-import requests
+
 
 import atexit
 
 import yaml
 
 try:
     from yaml import CSafeLoader as YamlSafeLoader, CSafeDumper as YamlSafeDumper
@@ -32,18 +32,19 @@
     from yaml import SafeLoader as YamlSafeLoader, SafeDumper as YamlSafeDumper
 
 from mlflow.entities import FileInfo
 from mlflow.exceptions import MissingConfigException
 from mlflow.protos.databricks_artifacts_pb2 import ArtifactCredentialType
 from mlflow.utils.rest_utils import augmented_raise_for_status
 from mlflow.utils.request_utils import cloud_storage_http_request
-from mlflow.utils.process import cache_return_value_per_process
+from mlflow.utils.process import cache_return_value_per_process, _exec_cmd
 from mlflow.utils import merge_dicts
 from mlflow.utils.databricks_utils import _get_dbutils
 from mlflow.utils.os import is_windows
+from mlflow.utils import download_cloud_file_chunk
 from mlflow.utils.request_utils import download_chunk
 
 
 ENCODING = "utf-8"
 MAX_PARALLEL_DOWNLOAD_WORKERS = os.cpu_count() * 2
 
 
@@ -593,72 +594,117 @@
             for chunk in response.iter_content(chunk_size=chunk_size):
                 if not chunk:
                     break
                 output_file.write(chunk)
 
 
 def parallelized_download_file_using_http_uri(
-    http_uri, download_path, file_size, uri_type, chunk_size, headers=None
+    thread_pool_executor,
+    http_uri,
+    download_path,
+    file_size,
+    uri_type,
+    chunk_size,
+    env,
+    headers=None,
 ):
     """
     Downloads a file specified using the `http_uri` to a local `download_path`. This function
     sends multiple requests in parallel each specifying its own desired byte range as a header,
     then reconstructs the file from the downloaded chunks. This allows for downloads of large files
     without OOM risk.
 
     Note : This function is meant to download files using presigned urls from various cloud
             providers.
     Returns a dict of chunk index : exception, if one was thrown for that index.
     """
 
+    def run_download(range_start, range_end):
+        with tempfile.TemporaryDirectory() as tmpdir:
+            temp_file = os.path.join(tmpdir, "error_messages.txt")
+            download_proc = _exec_cmd(
+                cmd=[
+                    sys.executable,
+                    download_cloud_file_chunk.__file__,
+                    "--range-start",
+                    range_start,
+                    "--range-end",
+                    range_end,
+                    "--headers",
+                    json.dumps(headers or {}),
+                    "--download-path",
+                    download_path,
+                    "--http-uri",
+                    http_uri,
+                    "--temp-file",
+                    temp_file,
+                ],
+                throw_on_error=True,
+                synchronous=False,
+                capture_output=True,
+                stream_output=False,
+                env=env,
+            )
+            _, stderr = download_proc.communicate()
+            if download_proc.returncode != 0:
+                if os.path.exists(temp_file):
+                    with open(temp_file, "r") as f:
+                        file_contents = f.read()
+                        if file_contents:
+                            return json.loads(file_contents)
+                        else:
+                            raise Exception(
+                                "Error from download_cloud_file_chunk not captured, "
+                                f"return code {download_proc.returncode}, stderr {stderr}"
+                            )
+
+    num_requests = int(math.ceil(file_size / float(chunk_size)))
     # Create file if it doesn't exist or erase the contents if it does. We should do this here
     # before sending to the workers so they can each individually seek to their respective positions
     # and write chunks without overwriting.
-    open(download_path, "wb").close()
+    open(download_path, "w").close()
     starting_index = 0
     if uri_type == ArtifactCredentialType.GCP_SIGNED_URL or uri_type is None:
         # GCP files could be transcoded, in which case the range header is ignored.
         # Test if this is the case by downloading one chunk and seeing if it's larger than the
         # requested size. If yes, let that be the file; if not, continue downloading more chunks.
         download_chunk(
-            index=0,
-            chunk_size=chunk_size,
+            range_start=0,
+            range_end=chunk_size - 1,
             headers=headers,
             download_path=download_path,
             http_uri=http_uri,
         )
         downloaded_size = os.path.getsize(download_path)
         # If downloaded size was equal to the chunk size it would have been downloaded serially,
         # so we don't need to consider this here
         if downloaded_size > chunk_size:
             return {}
         else:
             starting_index = 1
 
-    num_requests = int(math.ceil(file_size / float(chunk_size)))
-    with ThreadPoolExecutor(max_workers=MAX_PARALLEL_DOWNLOAD_WORKERS) as p:
-        futures = {}
-        for index in range(starting_index, num_requests):
-            future = p.submit(
-                download_chunk,
-                index=index,
-                chunk_size=chunk_size,
-                headers=headers,
-                download_path=download_path,
-                http_uri=http_uri,
-            )
-            futures[future] = index
-
-        failed_downloads = {}
-        for future in as_completed(futures):
-            try:
-                future.result()
-            except requests.HTTPError as e:
-                index = futures[future]
-                failed_downloads[index] = e
+    futures = {}
+    for i in range(starting_index, num_requests):
+        range_start = i * chunk_size
+        range_end = range_start + chunk_size - 1
+        futures[thread_pool_executor.submit(run_download, range_start, range_end)] = i
+
+    failed_downloads = {}
+    for future in as_completed(futures):
+        index = futures[future]
+        try:
+            result = future.result()
+            if result is not None:
+                failed_downloads[index] = result
+
+        except Exception as e:
+            failed_downloads[index] = {
+                "error_status_code": 500,
+                "error_text": repr(e),
+            }
 
     return failed_downloads
 
 
 def _handle_readonly_on_windows(func, path, exc_info):
     """
     This function should not be called directly but should be passed to `onerror` of
```

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/git_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/gorilla.py` & `mlflow-skinny-2.4.1/mlflow/utils/gorilla.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/import_hooks/__init__.py` & `mlflow-skinny-2.4.1/mlflow/utils/import_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/logging_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/mime_type_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/mime_type_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/mlflow_tags.py` & `mlflow-skinny-2.4.1/mlflow/utils/mlflow_tags.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/model_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/name_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/name_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/nfs_on_spark.py` & `mlflow-skinny-2.4.1/mlflow/utils/nfs_on_spark.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/process.py` & `mlflow-skinny-2.4.1/mlflow/utils/process.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/proto_json_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/proto_json_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/request_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/request_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import os
+# DO NO IMPORT MLFLOW IN THIS FILE.
+# This file is imported by download_cloud_file_chunk.py.
+# Importing mlflow is time-consuming and we want to avoid that in artifact download subprocesses.
 import requests
 import urllib3
 
-from functools import lru_cache
 from packaging.version import Version
 from requests.adapters import HTTPAdapter
 from requests.exceptions import HTTPError
 from urllib3.util import Retry
 
 # Response codes that generally indicate transient network failures and merit client retries,
 # based on guidance from cloud service providers
@@ -32,42 +33,38 @@
             raise HTTPError(
                 f"{e}. Response text: {response.text}", request=e.request, response=e.response
             )
         else:
             raise e
 
 
-def download_chunk(index, chunk_size, headers, download_path, http_uri):
-    range_start = index * chunk_size
-    range_end = range_start + chunk_size - 1
-    ranged_headers = {"Range": f"bytes={range_start}-{range_end}", **headers}
+def download_chunk(range_start, range_end, headers, download_path, http_uri):
+    combined_headers = {**headers, "Range": f"bytes={range_start}-{range_end}"}
+
     with cloud_storage_http_request(
-        "get", http_uri, stream=True, headers=ranged_headers
+        "get", http_uri, stream=False, headers=combined_headers
     ) as response:
         # File will have been created upstream. Use r+b to ensure chunks
         # don't overwrite the entire file.
         augmented_raise_for_status(response)
         with open(download_path, "r+b") as f:
             f.seek(range_start)
-            for content in response.iter_content(chunk_size=1_000_000):
-                f.write(content)
+            f.write(response.content)
 
 
-@lru_cache(maxsize=64)
-def _cached_get_request_session(
-    max_retries,
-    backoff_factor,
-    retry_codes,
-    # To create a new Session object for each process, we use the process id as the cache key.
-    # This is to avoid sharing the same Session object across processes, which can lead to issues
-    # such as https://stackoverflow.com/q/3724900.
-    _pid,
-):
+def _get_request_session(max_retries, backoff_factor, retry_codes):
     """
-    This function should not be called directly. Instead, use `_get_request_session` below.
+    Returns a `Requests.Session` object for making an HTTP request.
+
+    :param max_retries: Maximum total number of retries.
+    :param backoff_factor: a time factor for exponential backoff. e.g. value 5 means the HTTP
+      request will be retried with interval 5, 10, 20... seconds. A value of 0 turns off the
+      exponential backoff.
+    :param retry_codes: a list of HTTP response error codes that qualifies for retry.
+    :return: requests.Session object.
     """
     assert 0 <= max_retries < 10
     assert 0 <= backoff_factor < 120
 
     retry_kwargs = {
         "total": max_retries,
         "connect": max_retries,
@@ -86,33 +83,14 @@
     adapter = HTTPAdapter(max_retries=retry)
     session = requests.Session()
     session.mount("https://", adapter)
     session.mount("http://", adapter)
     return session
 
 
-def _get_request_session(max_retries, backoff_factor, retry_codes):
-    """
-    Returns a `Requests.Session` object for making an HTTP request.
-
-    :param max_retries: Maximum total number of retries.
-    :param backoff_factor: a time factor for exponential backoff. e.g. value 5 means the HTTP
-      request will be retried with interval 5, 10, 20... seconds. A value of 0 turns off the
-      exponential backoff.
-    :param retry_codes: a list of HTTP response error codes that qualifies for retry.
-    :return: requests.Session object.
-    """
-    return _cached_get_request_session(
-        max_retries,
-        backoff_factor,
-        retry_codes,
-        _pid=os.getpid(),
-    )
-
-
 def _get_http_response_with_retries(
     method, url, max_retries, backoff_factor, retry_codes, **kwargs
 ):
     """
     Performs an HTTP request using Python's `requests` module with an automatic retry policy.
 
     :param method: a string indicating the method to use, e.g. "GET", "POST", "PUT".
```

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/requirements_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/requirements_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/rest_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/rest_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/search_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/search_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 from packaging.version import Version
 
 from mlflow.entities import RunInfo
 from mlflow.entities.model_registry.model_version_stages import STAGE_DELETED_INTERNAL
 from mlflow.exceptions import MlflowException
 from mlflow.protos.databricks_pb2 import INVALID_PARAMETER_VALUE
 from mlflow.store.db.db_types import MYSQL, MSSQL, SQLITE, POSTGRES
-
+from mlflow.utils.mlflow_tags import (
+    MLFLOW_DATASET_CONTEXT,
+)
 import math
 
 
 def _convert_like_pattern_to_regex(pattern, flags=0):
     if not pattern.startswith("%"):
         pattern = "^" + pattern
     if not pattern.endswith("%"):
@@ -109,20 +111,22 @@
     DESC_OPERATOR = "desc"
     VALID_ORDER_BY_TAGS = [ASC_OPERATOR, DESC_OPERATOR]
     VALID_METRIC_COMPARATORS = {">", ">=", "!=", "=", "<", "<="}
     VALID_PARAM_COMPARATORS = {"!=", "=", LIKE_OPERATOR, ILIKE_OPERATOR}
     VALID_TAG_COMPARATORS = {"!=", "=", LIKE_OPERATOR, ILIKE_OPERATOR}
     VALID_STRING_ATTRIBUTE_COMPARATORS = {"!=", "=", LIKE_OPERATOR, ILIKE_OPERATOR, "IN", "NOT IN"}
     VALID_NUMERIC_ATTRIBUTE_COMPARATORS = VALID_METRIC_COMPARATORS
+    VALID_DATASET_COMPARATORS = {"!=", "=", LIKE_OPERATOR, ILIKE_OPERATOR, "IN", "NOT IN"}
     _BUILTIN_NUMERIC_ATTRIBUTES = {"start_time", "end_time"}
     _ALTERNATE_NUMERIC_ATTRIBUTES = {"created", "Created"}
     _ALTERNATE_STRING_ATTRIBUTES = {"run name", "Run name", "Run Name"}
     NUMERIC_ATTRIBUTES = set(
         list(_BUILTIN_NUMERIC_ATTRIBUTES) + list(_ALTERNATE_NUMERIC_ATTRIBUTES)
     )
+    DATASET_ATTRIBUTES = {"name", "digest", "context"}
     VALID_SEARCH_ATTRIBUTE_KEYS = set(
         RunInfo.get_searchable_attributes()
         + list(_ALTERNATE_NUMERIC_ATTRIBUTES)
         + list(_ALTERNATE_STRING_ATTRIBUTES)
     )
     VALID_ORDER_BY_ATTRIBUTE_KEYS = set(
         RunInfo.get_orderable_attributes() + list(_ALTERNATE_NUMERIC_ATTRIBUTES)
@@ -131,21 +135,30 @@
     _ALTERNATE_METRIC_IDENTIFIERS = {"metrics"}
     _PARAM_IDENTIFIER = "parameter"
     _ALTERNATE_PARAM_IDENTIFIERS = {"parameters", "param", "params"}
     _TAG_IDENTIFIER = "tag"
     _ALTERNATE_TAG_IDENTIFIERS = {"tags"}
     _ATTRIBUTE_IDENTIFIER = "attribute"
     _ALTERNATE_ATTRIBUTE_IDENTIFIERS = {"attr", "attributes", "run"}
-    _IDENTIFIERS = [_METRIC_IDENTIFIER, _PARAM_IDENTIFIER, _TAG_IDENTIFIER, _ATTRIBUTE_IDENTIFIER]
+    _DATASET_IDENTIFIER = "dataset"
+    _ALTERNATE_DATASET_IDENTIFIERS = {"datasets"}
+    _IDENTIFIERS = [
+        _METRIC_IDENTIFIER,
+        _PARAM_IDENTIFIER,
+        _TAG_IDENTIFIER,
+        _ATTRIBUTE_IDENTIFIER,
+        _DATASET_IDENTIFIER,
+    ]
     _VALID_IDENTIFIERS = set(
         _IDENTIFIERS
         + list(_ALTERNATE_METRIC_IDENTIFIERS)
         + list(_ALTERNATE_PARAM_IDENTIFIERS)
         + list(_ALTERNATE_TAG_IDENTIFIERS)
         + list(_ALTERNATE_ATTRIBUTE_IDENTIFIERS)
+        + list(_ALTERNATE_DATASET_IDENTIFIERS)
     )
     STRING_VALUE_TYPES = {TokenType.Literal.String.Single}
     DELIMITER_VALUE_TYPES = {TokenType.Punctuation}
     WHITESPACE_VALUE_TYPE = TokenType.Text.Whitespace
     NUMERIC_VALUE_TYPES = {TokenType.Literal.Number.Integer, TokenType.Literal.Number.Float}
     # Registered Models Constants
     ORDER_BY_KEY_TIMESTAMP = "timestamp"
@@ -280,14 +293,16 @@
             return cls._PARAM_IDENTIFIER
         elif entity_type in cls._ALTERNATE_METRIC_IDENTIFIERS:
             return cls._METRIC_IDENTIFIER
         elif entity_type in cls._ALTERNATE_TAG_IDENTIFIERS:
             return cls._TAG_IDENTIFIER
         elif entity_type in cls._ALTERNATE_ATTRIBUTE_IDENTIFIERS:
             return cls._ATTRIBUTE_IDENTIFIER
+        elif entity_type in cls._ALTERNATE_DATASET_IDENTIFIERS:
+            return cls._DATASET_IDENTIFIER
         else:
             # one of ("metric", "parameter", "tag", or "attribute") since it a valid type
             return entity_type
 
     @classmethod
     def _get_identifier(cls, identifier, valid_attributes):
         try:
@@ -296,24 +311,28 @@
                 key = tokens[0]
                 entity_type = cls._ATTRIBUTE_IDENTIFIER
             else:
                 entity_type, key = tokens
         except ValueError:
             raise MlflowException(
                 "Invalid identifier '%s'. Columns should be specified as "
-                "'attribute.<key>', 'metric.<key>', 'tag.<key>', or "
+                "'attribute.<key>', 'metric.<key>', 'tag.<key>', 'dataset.<key>', or "
                 "'param.'." % identifier,
                 error_code=INVALID_PARAMETER_VALUE,
             )
         identifier = cls._valid_entity_type(entity_type)
         key = cls._trim_backticks(cls._strip_quotes(key))
         if identifier == cls._ATTRIBUTE_IDENTIFIER and key not in valid_attributes:
             raise MlflowException.invalid_parameter_value(
                 f"Invalid attribute key '{key}' specified. Valid keys are '{valid_attributes}'"
             )
+        elif identifier == cls._DATASET_IDENTIFIER and key not in cls.DATASET_ATTRIBUTES:
+            raise MlflowException.invalid_parameter_value(
+                f"Invalid dataset key '{key}' specified. Valid keys are '{cls.DATASET_ATTRIBUTES}'"
+            )
         return {"type": identifier, "key": key}
 
     @classmethod
     def _get_value(cls, identifier_type, key, token):
         if identifier_type == cls._METRIC_IDENTIFIER:
             if token.ttype not in cls.NUMERIC_VALUE_TYPES:
                 raise MlflowException(
@@ -351,14 +370,33 @@
                 return cls._parse_run_ids(token)
             else:
                 raise MlflowException(
                     "Expected a quoted string value for attributes. "
                     "Got value {value}".format(value=token.value),
                     error_code=INVALID_PARAMETER_VALUE,
                 )
+        elif identifier_type == cls._DATASET_IDENTIFIER:
+            if key in cls.DATASET_ATTRIBUTES and (
+                token.ttype in cls.STRING_VALUE_TYPES or isinstance(token, Identifier)
+            ):
+                return cls._strip_quotes(token.value, expect_quoted_value=True)
+            elif isinstance(token, Parenthesis):
+                if key not in ("name", "digest", "context"):
+                    raise MlflowException(
+                        "Only the dataset 'name' and 'digest' supports comparison with a list of "
+                        "quoted string values.",
+                        error_code=INVALID_PARAMETER_VALUE,
+                    )
+                return cls._parse_run_ids(token)
+            else:
+                raise MlflowException(
+                    "Expected a quoted string value for dataset attributes. "
+                    "Got value {value}".format(value=token.value),
+                    error_code=INVALID_PARAMETER_VALUE,
+                )
         else:
             # Expected to be either "param" or "metric".
             raise MlflowException(
                 "Invalid identifier type. Expected one of "
                 "{}.".format([cls._METRIC_IDENTIFIER, cls._PARAM_IDENTIFIER])
             )
 
@@ -499,14 +537,25 @@
                     "Invalid comparator '{}' not one of "
                     "'{}".format(comparator, cls.VALID_STRING_ATTRIBUTE_COMPARATORS)
                 )
             return True
         return False
 
     @classmethod
+    def is_dataset(cls, key_type, comparator):
+        if key_type == cls._DATASET_IDENTIFIER:
+            if comparator not in cls.VALID_DATASET_COMPARATORS:
+                raise MlflowException(
+                    "Invalid comparator '%s' "
+                    "not one of '%s" % (comparator, cls.VALID_DATASET_COMPARATORS)
+                )
+            return True
+        return False
+
+    @classmethod
     def _does_run_match_clause(cls, run, sed):
         key_type = sed.get("type")
         key = sed.get("key")
         value = sed.get("value")
         comparator = sed.get("comparator").upper()
 
         key = SearchUtils.translate_key_alias(key)
@@ -519,14 +568,29 @@
         elif cls.is_tag(key_type, comparator):
             lhs = run.data.tags.get(key, None)
         elif cls.is_string_attribute(key_type, key, comparator):
             lhs = getattr(run.info, key)
         elif cls.is_numeric_attribute(key_type, key, comparator):
             lhs = getattr(run.info, key)
             value = int(value)
+        elif cls.is_dataset(key_type, comparator):
+            if key == "context":
+                return any(
+                    SearchUtils.get_comparison_func(comparator)(tag.value if tag else None, value)
+                    for dataset_input in run.inputs.dataset_inputs
+                    for tag in dataset_input.tags
+                    if tag.key == MLFLOW_DATASET_CONTEXT
+                )
+            else:
+                return any(
+                    SearchUtils.get_comparison_func(comparator)(
+                        getattr(dataset_input.dataset, key), value
+                    )
+                    for dataset_input in run.inputs.dataset_inputs
+                )
         else:
             raise MlflowException(
                 "Invalid search expression type '%s'" % key_type, error_code=INVALID_PARAMETER_VALUE
             )
         if lhs is None:
             return False
```

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/server_cli_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/server_cli_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/string_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/time_utils.py` & `mlflow-skinny-2.4.1/mlflow/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/uri.py` & `mlflow-skinny-2.4.1/mlflow/utils/uri.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/validation.py` & `mlflow-skinny-2.4.1/mlflow/utils/validation.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/utils/virtualenv.py` & `mlflow-skinny-2.4.1/mlflow/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/xgboost/__init__.py` & `mlflow-skinny-2.4.1/mlflow/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow/xgboost/_autolog.py` & `mlflow-skinny-2.4.1/mlflow/xgboost/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/mlflow_skinny.egg-info/PKG-INFO` & `mlflow-skinny-2.4.1/mlflow_skinny.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: mlflow-skinny
-Version: 2.4.0
+Version: 2.4.1
 Summary: MLflow: A Platform for ML Development and Productionization
 Home-page: https://mlflow.org/
 Author: Databricks
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mlflow/mlflow/issues
 Project-URL: Documentation, https://mlflow.org/docs/latest/index.html
 Project-URL: Source Code, https://github.com/mlflow/mlflow
 Keywords: ml ai databricks
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: extras
 Provides-Extra: databricks
+Provides-Extra: gateway
 Provides-Extra: sqlserver
 Provides-Extra: aliyun-oss
 License-File: LICENSE.txt
 
 =======================================================================
 MLflow Skinny: A Lightweight Machine Learning Lifecycle Platform Client
 =======================================================================
```

### Comparing `mlflow-skinny-2.4.0/mlflow_skinny.egg-info/SOURCES.txt` & `mlflow-skinny-2.4.1/mlflow_skinny.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 mlflow/client.py
 mlflow/db.py
 mlflow/diviner.py
 mlflow/environment_variables.py
 mlflow/exceptions.py
 mlflow/experiments.py
 mlflow/h2o.py
+mlflow/johnsnowlabs.py
 mlflow/keras.py
 mlflow/lightgbm.py
 mlflow/llm.py
 mlflow/ml_package_versions.py
 mlflow/mleap.py
 mlflow/onnx.py
 mlflow/pmdarima.py
@@ -340,14 +341,15 @@
 mlflow/utils/arguments_utils.py
 mlflow/utils/class_utils.py
 mlflow/utils/cli_args.py
 mlflow/utils/conda.py
 mlflow/utils/data_utils.py
 mlflow/utils/databricks_utils.py
 mlflow/utils/docstring_utils.py
+mlflow/utils/download_cloud_file_chunk.py
 mlflow/utils/env.py
 mlflow/utils/env_manager.py
 mlflow/utils/environment.py
 mlflow/utils/file_utils.py
 mlflow/utils/git_utils.py
 mlflow/utils/gorilla.py
 mlflow/utils/logging_utils.py
@@ -390,8 +392,9 @@
 pylint_plugins/import_checker.py
 pylint_plugins/print_function.py
 pylint_plugins/set_checker.py
 pylint_plugins/string_checker.py
 pylint_plugins/unittest_assert_raises.py
 pylint_plugins/pytest_raises_checker/__init__.py
 requirements/core-requirements.txt
+requirements/gateway-requirements.txt
 requirements/skinny-requirements.txt
```

### Comparing `mlflow-skinny-2.4.0/mlflow_skinny.egg-info/requires.txt` & `mlflow-skinny-2.4.1/mlflow_skinny.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -28,9 +28,14 @@
 pysftp
 kubernetes
 mlserver!=1.3.1,>=1.2.0
 mlserver-mlflow!=1.3.1,>=1.2.0
 virtualenv
 prometheus-flask-exporter
 
+[gateway]
+pydantic<3,>=1.0
+fastapi<1
+uvicorn<1
+
 [sqlserver]
 mlflow-dbstore
```

### Comparing `mlflow-skinny-2.4.0/pylint_plugins/__init__.py` & `mlflow-skinny-2.4.1/pylint_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/pylint_plugins/errors.py` & `mlflow-skinny-2.4.1/pylint_plugins/errors.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/pylint_plugins/import_checker.py` & `mlflow-skinny-2.4.1/pylint_plugins/import_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/pylint_plugins/print_function.py` & `mlflow-skinny-2.4.1/pylint_plugins/print_function.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/pylint_plugins/pytest_raises_checker/__init__.py` & `mlflow-skinny-2.4.1/pylint_plugins/pytest_raises_checker/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/pylint_plugins/set_checker.py` & `mlflow-skinny-2.4.1/pylint_plugins/set_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/pylint_plugins/string_checker.py` & `mlflow-skinny-2.4.1/pylint_plugins/string_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/pylint_plugins/unittest_assert_raises.py` & `mlflow-skinny-2.4.1/pylint_plugins/unittest_assert_raises.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/requirements/core-requirements.txt` & `mlflow-skinny-2.4.1/requirements/core-requirements.txt`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.4.0/setup.py` & `mlflow-skinny-2.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 the skinny client functionality with support for running the MLflow Tracking
 Server & UI. It also adds project backends such as Docker and Kubernetes among
 other capabilities.
 """
 with open(os.path.join("requirements", "core-requirements.txt")) as f:
     CORE_REQUIREMENTS = SKINNY_REQUIREMENTS + remove_comments_and_empty_lines(f.read().splitlines())
 
+with open(os.path.join("requirements", "gateway-requirements.txt")) as f:
+    GATEWAY_REQUIREMENTS = remove_comments_and_empty_lines(f.read().splitlines())
+
 _is_mlflow_skinny = bool(os.environ.get(_MLFLOW_SKINNY_ENV_VAR))
 logging.debug("{} env var is set: {}".format(_MLFLOW_SKINNY_ENV_VAR, _is_mlflow_skinny))
 
 
 class ListDependencies(Command):
     # `python setup.py <command name>` prints out "running <command name>" by default.
     # This logging message must be hidden by specifying `--quiet` (or `-q`) when piping the output
@@ -156,14 +159,15 @@
         ],
         "databricks": [
             # Required to write model artifacts to unity catalog locations
             "azure-storage-file-datalake>12",
             "google-cloud-storage>=1.30.0",
             "boto3>1",
         ],
+        "gateway": GATEWAY_REQUIREMENTS,
         "sqlserver": ["mlflow-dbstore"],
         "aliyun-oss": ["aliyunstoreplugin"],
     },
     entry_points="""
         [console_scripts]
         mlflow=mlflow.cli:cli
```

