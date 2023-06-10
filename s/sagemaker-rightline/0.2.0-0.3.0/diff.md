# Comparing `tmp/sagemaker-rightline-0.2.0.tar.gz` & `tmp/sagemaker-rightline-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-rightline-0.2.0.tar", last modified: Wed Jun  7 19:56:22 2023, max compression
+gzip compressed data, was "sagemaker-rightline-0.3.0.tar", last modified: Sat Jun 10 14:03:39 2023, max compression
```

## Comparing `sagemaker-rightline-0.2.0.tar` & `sagemaker-rightline-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:56:22.748468 sagemaker-rightline-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-06-07 19:56:22.748468 sagemaker-rightline-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:56:22.748468 sagemaker-rightline-0.2.0/sagemaker_rightline/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 19:56:15.000000 sagemaker-rightline-0.2.0/sagemaker_rightline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/sagemaker_rightline/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/sagemaker_rightline/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    19742 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/sagemaker_rightline/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:56:22.748468 sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-06-07 19:56:22.000000 sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-07 19:56:22.000000 sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:56:22.000000 sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 19:56:22.000000 sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 19:56:22.000000 sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:56:22.748468 sagemaker-rightline-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:56:22.748468 sagemaker-rightline-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15133 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:03:39.833795 sagemaker-rightline-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-06-10 14:03:39.833795 sagemaker-rightline-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:03:39.833795 sagemaker-rightline-0.3.0/sagemaker_rightline/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 14:03:32.000000 sagemaker-rightline-0.3.0/sagemaker_rightline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/sagemaker_rightline/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/sagemaker_rightline/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24416 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/sagemaker_rightline/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:03:39.833795 sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-06-10 14:03:39.000000 sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-10 14:03:39.000000 sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:03:39.000000 sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-10 14:03:39.000000 sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-10 14:03:39.000000 sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 14:03:39.833795 sagemaker-rightline-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:03:39.833795 sagemaker-rightline-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-06-10 14:03:28.000000 sagemaker-rightline-0.3.0/tests/test_validations.py
```

### Comparing `sagemaker-rightline-0.2.0/LICENSE` & `sagemaker-rightline-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.2.0/PKG-INFO` & `sagemaker-rightline-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -82,14 +82,15 @@
   - `StepImagesExist`
   - `StepKmsKeyIdAsExpected`
   - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
   - `StepTagsAsExpected`
+  - `StepInputsAsExpected`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
 For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
@@ -107,31 +108,32 @@
 A `Report` is a class whose instance is returned by the `Configuration` class (optionally a pandas.DataFrame instead).
 It contains the results of the `Validations` that were run against the `Pipeline` object as well as additional information
 to allow for further analysis.
 
 ## Usage
 
 ```python
-from sagemaker.processing import NetworkConfig
+from sagemaker.processing import NetworkConfig, ProcessingInput
 from sagemaker.workflow.parameters import ParameterString
 from sagemaker_rightline.model import Configuration
 from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
     PipelineParametersAsExpected,
     StepImagesExist,
     StepKmsKeyIdAsExpected,
     StepNetworkConfigAsExpected,
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
     StepTagsAsExpected,
+    StepInputsAsExpected,
 )
 
 # Import a dummy pipeline
-from tests.fixtures.pipeline import get_sagemaker_pipeline
+from tests.fixtures.pipeline import get_sagemaker_pipeline, DUMMY_BUCKET
 
 sm_pipeline = get_sagemaker_pipeline()
 
 # Define Validations
 validations = [
     StepImagesExist(),
     PipelineParametersAsExpected(
@@ -166,14 +168,25 @@
     StepTagsAsExpected(
         tags_expected=[{
             "some-key": "some-value",
         }],
         step_name="sm_training_step_sklearn",  # optional: if not set, will check all steps
         rule=Equals(),
     ),
+    StepInputsAsExpected(
+        inputs_expected=[
+            ProcessingInput(
+                source=f"s3://{DUMMY_BUCKET}/input-1",
+                destination="/opt/ml/processing/input",
+                input_name="input-2",
+            )
+        ],
+        step_type="Processing",  # either step_type or step_name must be set to filter
+        rule=Contains(),
+    ),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.2.0/README.md` & `sagemaker-rightline-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
   - `StepImagesExist`
   - `StepKmsKeyIdAsExpected`
   - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
   - `StepTagsAsExpected`
+  - `StepInputsAsExpected`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
 For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
@@ -62,31 +63,32 @@
 A `Report` is a class whose instance is returned by the `Configuration` class (optionally a pandas.DataFrame instead).
 It contains the results of the `Validations` that were run against the `Pipeline` object as well as additional information
 to allow for further analysis.
 
 ## Usage
 
 ```python
-from sagemaker.processing import NetworkConfig
+from sagemaker.processing import NetworkConfig, ProcessingInput
 from sagemaker.workflow.parameters import ParameterString
 from sagemaker_rightline.model import Configuration
 from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
     PipelineParametersAsExpected,
     StepImagesExist,
     StepKmsKeyIdAsExpected,
     StepNetworkConfigAsExpected,
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
     StepTagsAsExpected,
+    StepInputsAsExpected,
 )
 
 # Import a dummy pipeline
-from tests.fixtures.pipeline import get_sagemaker_pipeline
+from tests.fixtures.pipeline import get_sagemaker_pipeline, DUMMY_BUCKET
 
 sm_pipeline = get_sagemaker_pipeline()
 
 # Define Validations
 validations = [
     StepImagesExist(),
     PipelineParametersAsExpected(
@@ -121,14 +123,25 @@
     StepTagsAsExpected(
         tags_expected=[{
             "some-key": "some-value",
         }],
         step_name="sm_training_step_sklearn",  # optional: if not set, will check all steps
         rule=Equals(),
     ),
+    StepInputsAsExpected(
+        inputs_expected=[
+            ProcessingInput(
+                source=f"s3://{DUMMY_BUCKET}/input-1",
+                destination="/opt/ml/processing/input",
+                input_name="input-2",
+            )
+        ],
+        step_type="Processing",  # either step_type or step_name must be set to filter
+        rule=Contains(),
+    ),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.2.0/pyproject.toml` & `sagemaker-rightline-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.2.0/sagemaker_rightline/model.py` & `sagemaker-rightline-0.3.0/sagemaker_rightline/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,37 +99,40 @@
                     match.append(False)
                     continue
                 match.append(True)
             if all(match):
                 filtered_steps.append(subject)
         return filtered_steps
 
+    @staticmethod
     def get_attribute(
-        self,
         sagemaker_pipeline: Pipeline,
+        paths: List[str],
     ) -> List:
         """Get attribute from pipeline.
 
         :param sagemaker_pipeline: sagemaker pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
+        :param paths: list of paths to the attributes to be validated
+        :type paths: List[str]
         :return: attribute
         :rtype: List
         """
         # TODO: refactor
         result = []
-        for path in self.paths:
+        for path in paths:
             attr_path = path.split(".")[1:]
             sm_pipeline_copy = copy(sagemaker_pipeline)
             for ix, attr in enumerate(attr_path):
                 if attr.endswith("]"):
                     has_filter_dict = attr[-2] != "["
                     raw_attr = attr.split("[")[0]
                     sm_pipeline_copy = getattr(sm_pipeline_copy, raw_attr)
                     if has_filter_dict:
-                        sm_pipeline_copy = self.get_filtered_attributes(
+                        sm_pipeline_copy = Validation.get_filtered_attributes(
                             sm_pipeline_copy, ".".join(attr_path[ix:])
                         )
                 else:
                     sm_pipeline_copy = [
                         getattr(sub_attr, attr)
                         for sub_attr in sm_pipeline_copy
                         if hasattr(sub_attr, attr)
```

### Comparing `sagemaker-rightline-0.2.0/sagemaker_rightline/rules.py` & `sagemaker-rightline-0.3.0/sagemaker_rightline/rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,23 @@
         :rtype: ValidationResult
         """
         try:
             # In case of int, float, str
             is_equal = set(observed) == set(expected)
         except TypeError:
             # In case of dict
-            is_equal = observed == expected
+            if isinstance(observed, dict) and isinstance(expected, dict):
+                is_equal = observed == expected
+            # In case of nested list
+            elif isinstance(observed, list) and isinstance(expected, list):
+                is_equal = all(True if item in observed else False for item in expected) and all(
+                    True if item in expected else False for item in observed
+                )
+            else:
+                is_equal = observed == expected
 
         is_equal = is_equal if not self.negative else not is_equal
         return ValidationResult(
             validation_name=validation_name,
             success=is_equal,
             negative=self.negative,
             message=f"{str(observed)} does {'not ' if not is_equal else ''}equal {str(expected)}",
```

### Comparing `sagemaker-rightline-0.2.0/sagemaker_rightline/validations.py` & `sagemaker-rightline-0.3.0/sagemaker_rightline/validations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Union
 
 import boto3
 from botocore.exceptions import ClientError
 from sagemaker.estimator import Estimator
-from sagemaker.processing import NetworkConfig
+from sagemaker.inputs import FileSystemInput, TrainingInput
+from sagemaker.processing import NetworkConfig, ProcessingInput
 from sagemaker.workflow.entities import PipelineVariable
 from sagemaker.workflow.parameters import Parameter
 from sagemaker.workflow.pipeline import Pipeline
 
 from sagemaker_rightline.model import Rule, Validation, ValidationResult
 
 
@@ -34,15 +35,15 @@
         """Runs validation of Parameters on Pipeline.
 
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :return: Dict containing ValidationResult
         :rtype: ValidationResult
         """
-        parameters_observed = self.get_attribute(sagemaker_pipeline)
+        parameters_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
         if self.ignore_default_value:
             for ix, parameter in enumerate(parameters_observed):
                 parameters_observed[ix].default_value = None
         result = self.rule.run(parameters_observed, self.parameters_expected, self.name)
         return result
 
 
@@ -76,15 +77,15 @@
         """Runs validation of Parameters on Pipeline.
 
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :return: validation result
         :rtype: ValidationResult
         """
-        kms_keys_observed = self.get_attribute(sagemaker_pipeline)
+        kms_keys_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
         result = self.rule.run(kms_keys_observed, [self.kms_key_id_expected], self.name)
         return result
 
 
 @dataclass
 class ContainerImage:
     """Container Image dataclass."""
@@ -144,15 +145,15 @@
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :return: validation result
         :rtype: ValidationResult
         """
         paginator = self.client.get_paginator("describe_images")
 
-        uris = self.get_attribute(sagemaker_pipeline)
+        uris = Validation.get_attribute(sagemaker_pipeline, self.paths)
         # return uris
         not_exist = []
         exist = []
         for uri in uris:
             container_image = ContainerImage(uri=uri)
             try:
                 _ = list(
@@ -248,15 +249,15 @@
         """Runs validation of NetworkConfigs on Pipeline.
 
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :return: validation result
         :rtype: ValidationResult
         """
-        network_configs_observed = self.get_attribute(sagemaker_pipeline)
+        network_configs_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
 
         # Compatibility with TrainingStep, which does not have a NetworkConfig object
         # as attribute, but takes the attributes of NetworkConfig as individual arguments.
         training_step_estimators = [
             step.estimator
             for step in sagemaker_pipeline.steps
             if step.step_type.value == "Training"
@@ -323,15 +324,15 @@
         """Runs validation of Parameters on Pipeline.
 
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :return: validation result
         :rtype: ValidationResult
         """
-        lambda_func_observed = self.get_attribute(sagemaker_pipeline)
+        lambda_func_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
         exist = []
         not_exist = []
         for func in lambda_func_observed:
             try:
                 _ = self.client.get_function(
                     FunctionName=func,
                 )
@@ -400,15 +401,15 @@
         """Runs validation of Parameters on Pipeline.
 
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :return: validation result
         :rtype: ValidationResult
         """
-        role_arns_observed = self.get_attribute(sagemaker_pipeline)
+        role_arns_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
         role_name_observed = [role_arn.split("/")[-1] for role_arn in role_arns_observed]
         result = self.rule.run(role_name_observed, [self.role_name_expected], self.name)
         return result
 
 
 class StepRoleNameExists(Validation):
     """Validate existence of Role of Pipeline Step.
@@ -455,15 +456,15 @@
         """Runs validation of Parameters on Pipeline.
 
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :return: validation result
         :rtype: ValidationResult
         """
-        role_arns_observed = self.get_attribute(sagemaker_pipeline)
+        role_arns_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
         role_name_observed = [role_arn.split("/")[-1] for role_arn in role_arns_observed]
 
         exist = []
         not_exist = []
         for role_name in role_name_observed:
             try:
                 _ = self.client.get_role(
@@ -534,10 +535,118 @@
         """Runs validation of Parameters on Pipeline.
 
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :return: validation result
         :rtype: ValidationResult
         """
-        tags_observed = self.get_attribute(sagemaker_pipeline)
+        tags_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
         result = self.rule.run(tags_observed[0], self.tags_expected, self.name)
         return result
+
+
+class StepInputsAsExpected(Validation):
+    """Validate Inputs of Pipeline Step.
+
+    Supported only for ProcessingStep and TrainingStep. This validation
+    is useful when you want to ensure that the Inputs of a Pipeline Step
+    are as expected.
+    """
+
+    def __init__(
+        self,
+        inputs_expected: List[
+            Union[Dict[str, Union[str, TrainingInput, FileSystemInput]], ProcessingInput]
+        ],
+        rule: Rule,
+        step_type: Optional[Union["Training", "Processing"]] = None,  # noqa F821
+        step_name: Optional[str] = None,
+    ) -> None:
+        """Initialize StepTagsAsExpected validation.
+
+        :param inputs_expected: Expected Inputs
+        :type inputs_expected: List[Dict[str, Union[str, TrainingInput, ProcessingInput,
+        FileSystemInput]]]
+        :param rule: Rule to use for validation
+        :type rule: Rule
+        :param step_type: Type of Step to validate
+        :type step_type: Union["Training", "Processing"]
+        :param step_name: Name of Step to validate, defaults to None
+        :type step_name: Optional[str], optional
+        :return: None
+        :rtype: None
+        """
+        if step_type and step_name:
+            raise ValueError("step_type and step_name cannot be specified together.")
+        if not step_type and not step_name:
+            raise ValueError("Either step_type or step_name must be specified.")
+        if step_type not in ("Training", "Processing") and not step_name:
+            raise ValueError(f"step_type must be 'Training' or 'Processing', not {step_type}.")
+
+        self.step_filter: str = f"name=={step_name}" if step_name else ""
+        self.step_type_filter: str = f"step_type/value=={step_type}" if step_type else ""
+
+        super().__init__(
+            name="StepInputsAsExpected",
+            paths=[
+                f".steps[{self.step_filter} && {self.step_type_filter}].inputs",
+            ],
+            rule=rule,
+        )
+        self.inputs_expected: List[
+            Dict[str, Union[str, TrainingInput, ProcessingInput, FileSystemInput]]
+        ] = inputs_expected
+
+    @staticmethod
+    def format_training_inputs(
+        inputs: List[Dict[str, Union[str, TrainingInput, FileSystemInput]]]
+    ) -> List[Dict[str, Union[dict, str]]]:
+        """Format Training Inputs.
+
+        :param inputs: Training Inputs
+        :type inputs: List[Dict[str, Union[str, TrainingInput, FileSystemInput]]]
+        :return: Formatted Training Inputs
+        :rtype: List[Dict[str, Union[dict, str]]]
+        """
+        formatted_inputs = []
+        for item in inputs:
+            for key, value in item.items():
+                formatted_inputs.append(
+                    {
+                        key: value.__dict__
+                        if isinstance(value, TrainingInput) or isinstance(value, FileSystemInput)
+                        else value
+                    }
+                )
+        return formatted_inputs
+
+    def run(
+        self,
+        sagemaker_pipeline: Pipeline,
+    ) -> ValidationResult:
+        """Runs validation of Parameters on Pipeline.
+
+        :param sagemaker_pipeline: SageMaker Pipeline
+        :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
+        :return: validation result
+        :rtype: ValidationResult
+        """
+        if self.step_filter:
+            step_type = Validation.get_attribute(
+                sagemaker_pipeline, [f".steps[{self.step_filter}].step_type.value"]
+            )[0]
+            self.step_type_filter = f"step_type/value=={step_type}"
+
+        inputs_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
+
+        if self.step_type_filter == "step_type/value==Processing":
+            # ProcessingStep has a list of ProcessingInput
+            inputs_observed_formatted = [x.__dict__ for y in inputs_observed for x in y]
+            inputs_expected_formatted = [x.__dict__ for x in self.inputs_expected]
+        elif self.step_type_filter == "step_type/value==Training":
+            # TrainingStep has a dict with values potentially being TrainingInput or FileSystemInput
+            inputs_observed_formatted = StepInputsAsExpected.format_training_inputs(inputs_observed)
+            inputs_expected_formatted = StepInputsAsExpected.format_training_inputs(
+                self.inputs_expected
+            )
+        result = self.rule.run(inputs_observed_formatted, inputs_expected_formatted, self.name)
+        return result
```

### Comparing `sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/PKG-INFO` & `sagemaker-rightline-0.3.0/sagemaker_rightline.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -82,14 +82,15 @@
   - `StepImagesExist`
   - `StepKmsKeyIdAsExpected`
   - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
   - `StepTagsAsExpected`
+  - `StepInputsAsExpected`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
 For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
@@ -107,31 +108,32 @@
 A `Report` is a class whose instance is returned by the `Configuration` class (optionally a pandas.DataFrame instead).
 It contains the results of the `Validations` that were run against the `Pipeline` object as well as additional information
 to allow for further analysis.
 
 ## Usage
 
 ```python
-from sagemaker.processing import NetworkConfig
+from sagemaker.processing import NetworkConfig, ProcessingInput
 from sagemaker.workflow.parameters import ParameterString
 from sagemaker_rightline.model import Configuration
 from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
     PipelineParametersAsExpected,
     StepImagesExist,
     StepKmsKeyIdAsExpected,
     StepNetworkConfigAsExpected,
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
     StepTagsAsExpected,
+    StepInputsAsExpected,
 )
 
 # Import a dummy pipeline
-from tests.fixtures.pipeline import get_sagemaker_pipeline
+from tests.fixtures.pipeline import get_sagemaker_pipeline, DUMMY_BUCKET
 
 sm_pipeline = get_sagemaker_pipeline()
 
 # Define Validations
 validations = [
     StepImagesExist(),
     PipelineParametersAsExpected(
@@ -166,14 +168,25 @@
     StepTagsAsExpected(
         tags_expected=[{
             "some-key": "some-value",
         }],
         step_name="sm_training_step_sklearn",  # optional: if not set, will check all steps
         rule=Equals(),
     ),
+    StepInputsAsExpected(
+        inputs_expected=[
+            ProcessingInput(
+                source=f"s3://{DUMMY_BUCKET}/input-1",
+                destination="/opt/ml/processing/input",
+                input_name="input-2",
+            )
+        ],
+        step_type="Processing",  # either step_type or step_name must be set to filter
+        rule=Contains(),
+    ),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.2.0/tests/test_model.py` & `sagemaker-rightline-0.3.0/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,32 +173,38 @@
     """Test get_attribute method of Validation class."""
     kms_key_alias_expected = "some/kms-key-alias"
     validation = StepKmsKeyIdAsExpected(
         step_name="sm_processing_step_sklearn",
         rule=Equals(),
         kms_key_id_expected=kms_key_alias_expected,
     )
-    assert validation.get_attribute(sagemaker_pipeline) == [kms_key_alias_expected]
+    assert Validation.get_attribute(sagemaker_pipeline, validation.paths) == [
+        kms_key_alias_expected
+    ]
 
 
 def test_validation_get_attribute_no_filter(sagemaker_pipeline) -> None:
     """Test get_attribute method of Validation class."""
     kms_key_alias_expected = "some/kms-key-alias"
     validation = StepKmsKeyIdAsExpected(
         rule=Equals(),
         kms_key_id_expected=kms_key_alias_expected,
     )
-    assert validation.get_attribute(sagemaker_pipeline) == [
+    assert Validation.get_attribute(sagemaker_pipeline, validation.paths) == [
         kms_key_alias_expected,
         kms_key_alias_expected,
         kms_key_alias_expected,
     ]
 
     validation = StepImagesExist()
-    assert validation.get_attribute(sagemaker_pipeline) == [IMAGE_1_URI, IMAGE_2_URI, IMAGE_1_URI]
+    assert Validation.get_attribute(sagemaker_pipeline, validation.paths) == [
+        IMAGE_1_URI,
+        IMAGE_2_URI,
+        IMAGE_1_URI,
+    ]
 
 
 def test_validation_failed_error():
     """Test ValidationFailedError class."""
     validation_result = ValidationResult(
         success=False,
         negative=False,
```

### Comparing `sagemaker-rightline-0.2.0/tests/test_validations.py` & `sagemaker-rightline-0.3.0/tests/test_validations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import pytest
 from moto import mock_ecr, mock_iam, mock_lambda
-from sagemaker.processing import NetworkConfig
+from sagemaker.inputs import FileSystemInput, TrainingInput
+from sagemaker.processing import NetworkConfig, ProcessingInput
 from sagemaker.workflow.parameters import ParameterString
 
 from sagemaker_rightline.model import Validation, ValidationResult
 from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
     ContainerImage,
     PipelineParametersAsExpected,
     StepImagesExist,
+    StepInputsAsExpected,
     StepKmsKeyIdAsExpected,
     StepLambdaFunctionExists,
     StepNetworkConfigAsExpected,
     StepRoleNameAsExpected,
     StepRoleNameExists,
     StepTagsAsExpected,
 )
@@ -24,15 +26,15 @@
 )
 from tests.fixtures.image_details import (
     IMAGE_1_REPOSITORY_NAME,
     IMAGE_1_TAG,
     IMAGE_1_URI,
     IMAGE_2_URI,
 )
-from tests.fixtures.pipeline import get_sagemaker_pipeline
+from tests.fixtures.pipeline import DUMMY_BUCKET, get_sagemaker_pipeline
 from tests.utils import (
     create_iam_role,
     create_image,
     create_lambda_function,
     ecr_client,
     iam_client,
     lambda_client,
@@ -254,15 +256,15 @@
         encrypt_inter_container_traffic=True,
     )
     step_network_config = StepNetworkConfigAsExpected(
         network_config_expected=network_config_expected,
         rule=Equals(),
     )
     result = step_network_config.run(sagemaker_pipeline)
-    assert not result.success
+    assert result.success
 
 
 def test_step_network_config_none_observed(
     sagemaker_pipeline,
 ) -> None:
     network_config_expected = NetworkConfig(
         enable_network_isolation=True,
@@ -485,7 +487,211 @@
 def test_step_tags_as_expected_no_filter(rule, tags_expected, success, sagemaker_pipeline) -> None:
     step_role_validation = StepTagsAsExpected(
         tags_expected=tags_expected,
         rule=rule(),
     )
     result = step_role_validation.run(sagemaker_pipeline)
     assert result.success == success
+
+
+@pytest.mark.parametrize(
+    "rule,inputs_expected,step_type,success",
+    [
+        [
+            Contains,
+            [
+                ProcessingInput(
+                    source=f"s3://{DUMMY_BUCKET}/input-2",
+                    destination="/opt/ml/processing/input",
+                    input_name="input-2",
+                )
+            ],
+            "Processing",
+            True,
+        ],
+        [
+            Contains,
+            [
+                ProcessingInput(
+                    source=f"s3://{DUMMY_BUCKET}/input-2",
+                    destination="/opt/ml/processing/input",
+                    input_name="input-3",
+                )
+            ],
+            "Processing",
+            False,
+        ],
+        [
+            Contains,
+            [
+                {
+                    "train": TrainingInput(
+                        s3_data=f"s3://{DUMMY_BUCKET}/some-prefix/validation",
+                        content_type="text/csv",
+                    )
+                }
+            ],
+            "Training",
+            True,
+        ],
+        [
+            Contains,
+            [
+                {
+                    "validation": FileSystemInput(
+                        file_system_id="fs-1234",
+                        file_system_type="EFS",
+                        directory_path="/some/path",
+                        file_system_access_mode="ro",
+                    )
+                }
+            ],
+            "Training",
+            True,
+        ],
+    ],
+)
+def test_step_inputs_as_expected_no_filter(
+    rule, inputs_expected, step_type, success, sagemaker_pipeline
+) -> None:
+    step_inputs_validation = StepInputsAsExpected(
+        inputs_expected=inputs_expected,
+        step_type=step_type,
+        rule=rule(),
+    )
+    result = step_inputs_validation.run(sagemaker_pipeline)
+    assert result.success == success
+
+
+@pytest.mark.parametrize(
+    "rule,inputs_expected,step_name,success",
+    [
+        [
+            Equals,
+            [
+                ProcessingInput(
+                    source=f"s3://{DUMMY_BUCKET}/input-1",
+                    destination="/opt/ml/processing/input",
+                    input_name="input-1",
+                ),
+                ProcessingInput(
+                    source=f"s3://{DUMMY_BUCKET}/input-2",
+                    destination="/opt/ml/processing/input",
+                    input_name="input-2",
+                ),
+            ],
+            "sm_processing_step_sklearn",
+            True,
+        ],
+        [
+            Equals,
+            [
+                ProcessingInput(
+                    source=f"s3://{DUMMY_BUCKET}/input-2",
+                    destination="/opt/ml/processing/input",
+                    input_name="input-2",
+                ),
+                ProcessingInput(
+                    source=f"s3://{DUMMY_BUCKET}/input-1",
+                    destination="/opt/ml/processing/input",
+                    input_name="input-1",
+                ),
+            ],
+            "sm_processing_step_sklearn",
+            True,
+        ],
+        [
+            Equals,
+            [
+                {
+                    "train": TrainingInput(
+                        s3_data=f"s3://{DUMMY_BUCKET}/some-prefix/validation",
+                        content_type="text/csv",
+                    ),
+                    "validation": FileSystemInput(
+                        file_system_id="fs-1234",
+                        file_system_type="EFS",
+                        directory_path="/some/path",
+                        file_system_access_mode="ro",
+                    ),
+                    "some-key": "some-value",
+                }
+            ],
+            "sm_training_step_sklearn",
+            True,
+        ],
+        [
+            Equals,
+            [
+                {
+                    "train": TrainingInput(
+                        s3_data=f"s3://{DUMMY_BUCKET}/some-prefix/validation",
+                        content_type="text/csv",
+                    ),
+                    "some-key": "some-value",
+                    "validation": FileSystemInput(
+                        file_system_id="fs-1234",
+                        file_system_type="EFS",
+                        directory_path="/some/path",
+                        file_system_access_mode="ro",
+                    ),
+                }
+            ],
+            "sm_training_step_sklearn",
+            True,
+        ],
+        [
+            Equals,
+            [
+                ProcessingInput(
+                    source=f"s3://{DUMMY_BUCKET}/does-not-match",
+                    destination="/opt/ml/processing/input",
+                    input_name="input-1",
+                ),
+                ProcessingInput(
+                    source=f"s3://{DUMMY_BUCKET}/input-1",
+                    destination="/opt/ml/processing/input",
+                    input_name="input-2",
+                ),
+            ],
+            "sm_processing_step_sklearn",
+            False,
+        ],
+    ],
+)
+def test_step_inputs_as_expected_filter(
+    rule, inputs_expected, step_name, success, sagemaker_pipeline
+) -> None:
+    step_inputs_validation = StepInputsAsExpected(
+        inputs_expected=inputs_expected,
+        step_name=step_name,
+        rule=rule(),
+    )
+    result = step_inputs_validation.run(sagemaker_pipeline)
+    assert result.success == success
+
+
+def test_step_inputs_as_expected_args_validation_step_type() -> None:
+    with pytest.raises(ValueError):
+        StepInputsAsExpected(
+            inputs_expected=[],
+            step_type="does-not-exist",
+            rule=Equals(),
+        )
+
+
+def test_step_inputs_as_expected_args_validation_exclusive() -> None:
+    with pytest.raises(ValueError):
+        StepInputsAsExpected(
+            inputs_expected=[],
+            step_type="does-not-exist",
+            step_name="does-not-exist",
+            rule=Equals(),
+        )
+
+
+def test_step_inputs_as_expected_args_validation_neither() -> None:
+    with pytest.raises(ValueError):
+        StepInputsAsExpected(
+            inputs_expected=[],
+            rule=Equals(),
+        )
```

