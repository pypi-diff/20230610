# Comparing `tmp/responsibleai-0.9.3.tar.gz` & `tmp/responsibleai-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/responsibleai-0.9.3.tar", last modified: Tue Aug 17 20:08:16 2021, max compression
+gzip compressed data, was "dist/responsibleai-0.9.4.tar", last modified: Wed Aug 18 22:18:09 2021, max compression
```

## Comparing `responsibleai-0.9.3.tar` & `responsibleai-0.9.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)    22090 2021-08-17 20:08:16.000000 responsibleai-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    21414 2021-08-17 20:08:14.000000 responsibleai-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-17 20:02:44.000000 responsibleai-0.9.3/responsibleai/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai/_config/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      454 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_config/base_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4178 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_input_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2963 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai/_internal/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_internal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai/_managers/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_managers/base_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    15983 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_managers/causal_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    14070 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_managers/counterfactual_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    13949 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_managers/error_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    14762 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_managers/explainer_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai/_tools/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai/_tools/causal/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_tools/causal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_tools/causal/causal_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1804 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_tools/causal/causal_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     5557 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_tools/causal/causal_result.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai/_tools/shared/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_tools/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4186 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/_tools/shared/attribute_serialization.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai/modelanalysis/
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/modelanalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/modelanalysis/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    23690 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/modelanalysis/model_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2021-08-17 20:00:58.000000 responsibleai-0.9.3/responsibleai/serialization_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22090 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      193 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-08-17 20:08:16.000000 responsibleai-0.9.3/responsibleai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-17 20:08:16.000000 responsibleai-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2021-08-17 20:00:58.000000 responsibleai-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8045 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/causal_manager_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6358 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/tests/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/counterfactual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/counterfactual/test_counterfactual_advanced_features.py
--rw-r--r--   0 runner    (1001) docker     (121)     4016 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/counterfactual_manager_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3477 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/error_analysis_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2116 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/explainer_manager_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/tests/test_causal/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/test_causal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/test_causal/test_causal_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     8598 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/test_causal/test_causal_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     3572 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/test_input_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)    11500 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/test_model_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    14371 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/test_model_analysis_validations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/test_model_serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/test_serialization_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/tests/test_tools/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/test_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-17 20:08:16.000000 responsibleai-0.9.3/tests/test_tools/test_shared/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/test_tools/test_shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2932 2021-08-17 20:00:58.000000 responsibleai-0.9.3/tests/test_tools/test_shared/test_attribute_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)    22090 2021-08-18 22:18:09.000000 responsibleai-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    21414 2021-08-18 22:18:07.000000 responsibleai-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai/
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-18 22:11:39.000000 responsibleai-0.9.4/responsibleai/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai/_config/
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_config/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4178 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_input_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2963 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai/_internal/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_internal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai/_managers/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_managers/base_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15983 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_managers/causal_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14070 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_managers/counterfactual_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13949 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_managers/error_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14762 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_managers/explainer_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai/_tools/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai/_tools/causal/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_tools/causal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_tools/causal/causal_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1804 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_tools/causal/causal_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5557 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_tools/causal/causal_result.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai/_tools/shared/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_tools/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4186 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/_tools/shared/attribute_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai/modelanalysis/
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/modelanalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/modelanalysis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23690 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/modelanalysis/model_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1282 2021-08-18 22:09:44.000000 responsibleai-0.9.4/responsibleai/serialization_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    22090 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1954 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-08-18 22:18:09.000000 responsibleai-0.9.4/responsibleai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-18 22:18:09.000000 responsibleai-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2021-08-18 22:09:44.000000 responsibleai-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8045 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/causal_manager_validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6358 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/tests/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/counterfactual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3872 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/counterfactual/test_counterfactual_advanced_features.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4016 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/counterfactual_manager_validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3477 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/error_analysis_validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2116 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/explainer_manager_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/tests/test_causal/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/test_causal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/test_causal/test_causal_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8598 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/test_causal/test_causal_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3572 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/test_input_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11500 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/test_model_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14371 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/test_model_analysis_validations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1661 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/test_model_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1467 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/test_serialization_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/tests/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/test_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 22:18:09.000000 responsibleai-0.9.4/tests/test_tools/test_shared/
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/test_tools/test_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2932 2021-08-18 22:09:44.000000 responsibleai-0.9.4/tests/test_tools/test_shared/test_attribute_serialization.py
```

### Comparing `responsibleai-0.9.3/PKG-INFO` & `responsibleai-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai
-Version: 0.9.3
+Version: 0.9.4
 Summary: SDK API to explain models, and analyze errors in Machine Learning
 Home-page: https://github.com/microsoft/responsible-ai-widgets
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `responsibleai-0.9.3/README.md` & `responsibleai-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/_input_processing.py` & `responsibleai-0.9.4/responsibleai/_input_processing.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/_interfaces.py` & `responsibleai-0.9.4/responsibleai/_interfaces.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/_internal/constants.py` & `responsibleai-0.9.4/responsibleai/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/_managers/base_manager.py` & `responsibleai-0.9.4/responsibleai/_managers/base_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/_managers/causal_manager.py` & `responsibleai-0.9.4/responsibleai/_managers/causal_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/_managers/counterfactual_manager.py` & `responsibleai-0.9.4/responsibleai/_managers/counterfactual_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/_managers/error_analysis_manager.py` & `responsibleai-0.9.4/responsibleai/_managers/error_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/_managers/explainer_manager.py` & `responsibleai-0.9.4/responsibleai/_managers/explainer_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/_tools/causal/causal_config.py` & `responsibleai-0.9.4/responsibleai/_tools/causal/causal_config.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/_tools/causal/causal_constants.py` & `responsibleai-0.9.4/responsibleai/_tools/causal/causal_constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/_tools/causal/causal_result.py` & `responsibleai-0.9.4/responsibleai/_tools/causal/causal_result.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/_tools/shared/attribute_serialization.py` & `responsibleai-0.9.4/responsibleai/_tools/shared/attribute_serialization.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/exceptions.py` & `responsibleai-0.9.4/responsibleai/exceptions.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/modelanalysis/model_analysis.py` & `responsibleai-0.9.4/responsibleai/modelanalysis/model_analysis.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai/serialization_utilities.py` & `responsibleai-0.9.4/responsibleai/serialization_utilities.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/responsibleai.egg-info/PKG-INFO` & `responsibleai-0.9.4/responsibleai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai
-Version: 0.9.3
+Version: 0.9.4
 Summary: SDK API to explain models, and analyze errors in Machine Learning
 Home-page: https://github.com/microsoft/responsible-ai-widgets
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `responsibleai-0.9.3/responsibleai.egg-info/SOURCES.txt` & `responsibleai-0.9.4/responsibleai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/setup.py` & `responsibleai-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/causal_manager_validator.py` & `responsibleai-0.9.4/tests/causal_manager_validator.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/common_utils.py` & `responsibleai-0.9.4/tests/common_utils.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/counterfactual/test_counterfactual_advanced_features.py` & `responsibleai-0.9.4/tests/counterfactual/test_counterfactual_advanced_features.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/counterfactual_manager_validator.py` & `responsibleai-0.9.4/tests/counterfactual_manager_validator.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/error_analysis_validator.py` & `responsibleai-0.9.4/tests/error_analysis_validator.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/explainer_manager_validator.py` & `responsibleai-0.9.4/tests/explainer_manager_validator.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/test_causal/test_causal_manager.py` & `responsibleai-0.9.4/tests/test_causal/test_causal_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/test_dependencies.py` & `responsibleai-0.9.4/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/test_input_processing.py` & `responsibleai-0.9.4/tests/test_input_processing.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/test_model_analysis.py` & `responsibleai-0.9.4/tests/test_model_analysis.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/test_model_analysis_validations.py` & `responsibleai-0.9.4/tests/test_model_analysis_validations.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/test_model_serializer.py` & `responsibleai-0.9.4/tests/test_model_serializer.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/test_serialization_utilities.py` & `responsibleai-0.9.4/tests/test_serialization_utilities.py`

 * *Files identical despite different names*

### Comparing `responsibleai-0.9.3/tests/test_tools/test_shared/test_attribute_serialization.py` & `responsibleai-0.9.4/tests/test_tools/test_shared/test_attribute_serialization.py`

 * *Files identical despite different names*

