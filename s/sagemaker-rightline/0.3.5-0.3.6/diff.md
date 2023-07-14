# Comparing `tmp/sagemaker-rightline-0.3.5.tar.gz` & `tmp/sagemaker-rightline-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-rightline-0.3.5.tar", last modified: Wed Jul 12 15:37:49 2023, max compression
+gzip compressed data, was "sagemaker-rightline-0.3.6.tar", last modified: Fri Jul 14 21:59:03 2023, max compression
```

## Comparing `sagemaker-rightline-0.3.5.tar` & `sagemaker-rightline-0.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:37:49.779383 sagemaker-rightline-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-07-12 15:37:49.779383 sagemaker-rightline-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:37:49.779383 sagemaker-rightline-0.3.5/sagemaker_rightline/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 15:37:42.000000 sagemaker-rightline-0.3.5/sagemaker_rightline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/sagemaker_rightline/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/sagemaker_rightline/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    33374 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/sagemaker_rightline/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:37:49.779383 sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-07-12 15:37:49.000000 sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-12 15:37:49.000000 sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:37:49.000000 sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-12 15:37:49.000000 sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 15:37:49.000000 sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:37:49.779383 sagemaker-rightline-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:37:49.779383 sagemaker-rightline-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    31054 2023-07-12 15:37:37.000000 sagemaker-rightline-0.3.5/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:59:03.567860 sagemaker-rightline-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 21:58:47.000000 sagemaker-rightline-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-07-14 21:59:03.563859 sagemaker-rightline-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-07-14 21:58:47.000000 sagemaker-rightline-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-14 21:58:47.000000 sagemaker-rightline-0.3.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:59:03.563859 sagemaker-rightline-0.3.6/sagemaker_rightline/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 21:58:55.000000 sagemaker-rightline-0.3.6/sagemaker_rightline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-14 21:58:47.000000 sagemaker-rightline-0.3.6/sagemaker_rightline/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-14 21:58:47.000000 sagemaker-rightline-0.3.6/sagemaker_rightline/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-14 21:58:47.000000 sagemaker-rightline-0.3.6/sagemaker_rightline/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:59:03.563859 sagemaker-rightline-0.3.6/sagemaker_rightline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-07-14 21:59:03.000000 sagemaker-rightline-0.3.6/sagemaker_rightline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-14 21:59:03.000000 sagemaker-rightline-0.3.6/sagemaker_rightline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:59:03.000000 sagemaker-rightline-0.3.6/sagemaker_rightline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-14 21:59:03.000000 sagemaker-rightline-0.3.6/sagemaker_rightline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 21:59:03.000000 sagemaker-rightline-0.3.6/sagemaker_rightline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 21:59:03.567860 sagemaker-rightline-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:59:03.563859 sagemaker-rightline-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-14 21:58:47.000000 sagemaker-rightline-0.3.6/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-14 21:58:47.000000 sagemaker-rightline-0.3.6/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33235 2023-07-14 21:58:47.000000 sagemaker-rightline-0.3.6/tests/test_validations.py
```

### Comparing `sagemaker-rightline-0.3.5/LICENSE` & `sagemaker-rightline-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.5/PKG-INFO` & `sagemaker-rightline-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,14 +42,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Test-Build-Workflow](https://github.com/stiebels/sagemaker-rightline/actions/workflows/python-package.yml/badge.svg)
 [![codecov](https://codecov.io/gh/stiebels/sagemaker-rightline/branch/main/graph/badge.svg?token=7TCW0GP1NV)](https://codecov.io/gh/stiebels/sagemaker-rightline)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/stiebels/sagemaker-rightline/issues)
+[![Documentation Status](https://readthedocs.org/projects/sagemaker-rightline/badge/?version=latest)](https://sagemaker-rightline.readthedocs.io/en/latest/?badge=latest)
 
 # sagemaker-rightline
 
 This repository contains the source code for sagemaker-rightline, a Python package that eases validation of properties of a SageMaker Pipeline object.
 
 Note that at present this package is in an early stage of development and is not yet ready for production use. We welcome contributions!
```

### Comparing `sagemaker-rightline-0.3.5/README.md` & `sagemaker-rightline-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ![Test-Build-Workflow](https://github.com/stiebels/sagemaker-rightline/actions/workflows/python-package.yml/badge.svg)
 [![codecov](https://codecov.io/gh/stiebels/sagemaker-rightline/branch/main/graph/badge.svg?token=7TCW0GP1NV)](https://codecov.io/gh/stiebels/sagemaker-rightline)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/stiebels/sagemaker-rightline/issues)
+[![Documentation Status](https://readthedocs.org/projects/sagemaker-rightline/badge/?version=latest)](https://sagemaker-rightline.readthedocs.io/en/latest/?badge=latest)
 
 # sagemaker-rightline
 
 This repository contains the source code for sagemaker-rightline, a Python package that eases validation of properties of a SageMaker Pipeline object.
 
 Note that at present this package is in an early stage of development and is not yet ready for production use. We welcome contributions!
```

### Comparing `sagemaker-rightline-0.3.5/pyproject.toml` & `sagemaker-rightline-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.5/sagemaker_rightline/model.py` & `sagemaker-rightline-0.3.6/sagemaker_rightline/model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.5/sagemaker_rightline/rules.py` & `sagemaker-rightline-0.3.6/sagemaker_rightline/rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.5/sagemaker_rightline/validations.py` & `sagemaker-rightline-0.3.6/sagemaker_rightline/validations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Union
 
 import boto3
 from botocore.exceptions import ClientError
 from sagemaker.estimator import Estimator
-from sagemaker.inputs import FileSystemInput, TrainingInput
+from sagemaker.inputs import FileSystemInput, TrainingInput, TransformInput
 from sagemaker.processing import NetworkConfig, ProcessingInput, ProcessingOutput
 from sagemaker.workflow.entities import PipelineVariable
 from sagemaker.workflow.parameters import Parameter
 from sagemaker.workflow.pipeline import Pipeline
 
 from sagemaker_rightline.model import Rule, Validation, ValidationResult
 from sagemaker_rightline.rules import Equals
@@ -47,29 +47,33 @@
         result = self.rule.run(parameters_observed, self.parameters_expected, self.name)
         return result
 
 
 class StepKmsKeyIdAsExpected(Validation):
     """Validate KmsKeyId or output_kms_key in Step.
 
-    Supported only for ProcessingStep and TrainingStep (output_kms_key).
-    This validation is useful when you want to ensure that the KmsKeyId
-    or output_kms_key of a Pipeline Step is as expected.
+    Supported only for ProcessingStep, TransformStep and TrainingStep
+    (output_kms_key). This validation is useful when you want to ensure
+    that the KmsKeyId or output_kms_key of a Pipeline Step is as
+    expected.
     """
 
     def __init__(
         self, kms_key_id_expected: str, rule: Rule, step_name: Optional[str] = None
     ) -> None:
         """Initialize StepKmsKeyIdAsExpected validation."""
         self.step_filter: str = f"name=={step_name}" if step_name else ""
         super().__init__(
             name="StepKmsKeyIdAsExpected",
             paths=[
                 f".steps[{self.step_filter} && step_type/value==Processing].kms_key",
-                f".steps[{self.step_filter} && step_type/value==Training].estimator.output_kms_key",
+                f".steps[{self.step_filter} && step_type/value==Transform].transformer."
+                f"output_kms_key",
+                f".steps[{self.step_filter} && step_type/value==Training].estimator."
+                f"output_kms_key",
             ],
             rule=rule,
         )
         self.kms_key_id_expected: str = kms_key_id_expected
 
     def run(
         self,
@@ -520,14 +524,16 @@
         self.step_filter: str = f"name=={step_name}" if step_name else ""
 
         super().__init__(
             name="StepTagsAsExpected",
             paths=[
                 f".steps[{self.step_filter} && step_type/value==Processing].processor.tags",
                 f".steps[{self.step_filter} && step_type/value==Training].estimator.tags",
+                f".steps[{self.step_filter} && step_type/value==Transform].transformer.tags",
+                f".steps[{self.step_filter} && step_type/value==Tuning].tuner.tags",
             ],
             rule=rule,
         )
         self.tags_expected: List[Dict[str, Union[str, PipelineVariable]]] = tags_expected
 
     def run(
         self,
@@ -552,18 +558,22 @@
     is useful when you want to ensure that the Inputs of a Pipeline Step
     are as expected.
     """
 
     def __init__(
         self,
         inputs_expected: List[
-            Union[Dict[str, Union[str, TrainingInput, FileSystemInput]], ProcessingInput]
+            Union[
+                Dict[str, Union[str, TrainingInput, FileSystemInput]],
+                ProcessingInput,
+                TransformInput,
+            ]
         ],
         rule: Rule,
-        step_type: Optional[Union["Training", "Processing"]] = None,  # noqa F821
+        step_type: Optional[Union["Training", "Processing", "Transform"]] = None,  # noqa F821
         step_name: Optional[str] = None,
     ) -> None:
         """Initialize StepTagsAsExpected validation.
 
         :param inputs_expected: Expected Inputs
         :type inputs_expected: List[Dict[str, Union[str, TrainingInput, ProcessingInput,
         FileSystemInput]]]
@@ -576,16 +586,18 @@
         :return: None
         :rtype: None
         """
         if step_type and step_name:
             raise ValueError("step_type and step_name cannot be specified together.")
         if not step_type and not step_name:
             raise ValueError("Either step_type or step_name must be specified.")
-        if step_type not in ("Training", "Processing") and not step_name:
-            raise ValueError(f"step_type must be 'Training' or 'Processing', not {step_type}.")
+        if step_type not in ("Training", "Processing", "Transform") and not step_name:
+            raise ValueError(
+                f"step_type must be 'Training' or 'Processing' or 'Transform', not {step_type}."
+            )
 
         self.step_filter: str = f"name=={step_name}" if step_name else ""
         self.step_type_filter: str = f"step_type/value=={step_type}" if step_type else ""
 
         super().__init__(
             name="StepInputsAsExpected",
             paths=[
@@ -636,19 +648,23 @@
                 sagemaker_pipeline, [f".steps[{self.step_filter}].step_type.value"]
             )[0]
             self.step_type_filter = f"step_type/value=={step_type}"
 
         inputs_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
 
         if self.step_type_filter == "step_type/value==Processing":
-            # ProcessingStep has a list of ProcessingInput
+            # ProcessingStep/TransformStep has a list of ProcessingInput/TransformInput
             inputs_observed_formatted = [x.__dict__ for y in inputs_observed for x in y]
             inputs_expected_formatted = [x.__dict__ for x in self.inputs_expected]
+        elif self.step_type_filter == "step_type/value==Transform":
+            inputs_observed_formatted = [x.__dict__ for x in inputs_observed]
+            inputs_expected_formatted = [x.__dict__ for x in self.inputs_expected]
         elif self.step_type_filter == "step_type/value==Training":
-            # TrainingStep has a dict with values potentially being TrainingInput or FileSystemInput
+            # TrainingStep has a dict with values potentially being TrainingInput or
+            # FileSystemInput
             inputs_observed_formatted = StepInputsAsExpected.format_training_inputs(inputs_observed)
             inputs_expected_formatted = StepInputsAsExpected.format_training_inputs(
                 self.inputs_expected
             )
         result = self.rule.run(inputs_observed_formatted, inputs_expected_formatted, self.name)
         return result
 
@@ -659,21 +675,21 @@
     Supported only for ProcessingStep. This validation is useful when
     you want to ensure that the Outputs of a Pipeline Step are as
     expected.
     """
 
     def __init__(
         self,
-        outputs_expected: List[ProcessingOutput],
+        outputs_expected: Union[List[ProcessingOutput], str],
         rule: Rule,
         step_name: Optional[str] = None,
     ) -> None:
-        """Initialize StepTagsAsExpected validation.
+        """Initialize StepOutputsAsExpected validation.
 
-        :param outputs_expected: Expected Inputs
+        :param outputs_expected: Expected outputs
         :type outputs_expected: List[ProcessingOutput]
         :param rule: Rule to use for validation
         :type rule: Rule
         :param step_name: Name of Step to validate, defaults to None
         :type step_name: Optional[str], optional
         :return: None
         :rtype: None
@@ -681,45 +697,56 @@
 
         self.step_filter: str = f"name=={step_name}" if step_name else ""
 
         super().__init__(
             name="StepOutputsAsExpected",
             paths=[
                 f".steps[{self.step_filter} && step_type/value==Processing]].outputs",
+                f".steps[{self.step_filter} && step_type/value==Transform]].transformer."
+                f"output_path",
             ],
             rule=rule,
         )
-        self.outputs_expected: List[ProcessingOutput] = outputs_expected
+        self.outputs_expected: List[Union[ProcessingOutput, str]] = outputs_expected
 
     def run(
         self,
         sagemaker_pipeline: Pipeline,
     ) -> ValidationResult:
         """Runs validation of StepOutputs on Pipeline.
 
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :return: validation result
         :rtype: ValidationResult
         """
 
         outputs_observed = Validation.get_attribute(sagemaker_pipeline, self.paths)
-        outputs_observed_formatted = [x.__dict__ for y in outputs_observed for x in y]
-        outputs_expected_formatted = [x.__dict__ for x in self.outputs_expected]
+        outputs_observed_formatted = []
+        for output in outputs_observed:
+            if isinstance(output, str):
+                outputs_observed_formatted.append(output)
+            else:
+                for item in output:
+                    outputs_observed_formatted.append(item.__dict__)
+        outputs_expected_formatted = [
+            x.__dict__ if not isinstance(x, str) else x for x in self.outputs_expected
+        ]
         result = self.rule.run(outputs_observed_formatted, outputs_expected_formatted, self.name)
         return result
 
 
 class StepOutputsMatchInputsAsExpected(Validation):
     """Validate Outputs <> Inputs of Pipeline Step."""
 
     def __init__(self, inputs_outputs_expected: List[Dict[str, Dict[str, str]]]) -> None:
         """Initialize StepTagsAsExpected validation.
 
-        :param inputs_outputs_expected: Expected Input and Output per step name
+        :param inputs_outputs_expected: Expected Input and Output per step name.
+        Use 'transform' for the input or output of the TransformStep.
         :type inputs_outputs_expected: Dict[str, Dict[str, str]]
         :return: None
         :rtype: None
         """
         name = "StepOutputsMatchInputsAsExpected"
         super().__init__(
             name=name,
@@ -736,30 +763,34 @@
         :param sagemaker_pipeline: SageMaker Pipeline
         :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
         :param step_name: Name of Step
         :type step_name: str
         :return: ProcessingStep
         :rtype: ProcessingStep
         """
-        supported_step_types = ("Processing", "Training", "Tuning")
+        supported_step_types = ("Processing", "Training", "Tuning", "Transform")
         for step in sagemaker_pipeline.steps:
-            if step.name == step_name and step.step_type.value in supported_step_types:
+            if step.step_type.value == "Transform" and step_name == "transform":
+                return step
+            elif step.name == step_name and step.step_type.value in supported_step_types:
                 return step
-        raise ValueError(f"Processing, Training or Tuning Step {step_name} not found in Pipeline.")
+        raise ValueError(
+            f"Processing, Training, Transform or Tuning Step {step_name} not found in Pipeline."
+        )
 
     @staticmethod
     def get_input_output_by_name(
-        step: Union["ProcessingStep", "TrainingStep", "TuningStep"],  # noqa F821
+        step: Union["ProcessingStep", "TrainingStep", "TuningStep", "TransformStep"],  # noqa F821
         name: str,
         kind: str,  # noqa F821
     ) -> str:
         """Get ProcessingInput or ProcessingOutput by name.
 
         :param step: step to run validation on
-        :type step: Union[ProcessingStep, TrainingStep, TuningStep]
+        :type step: Union[ProcessingStep, TrainingStep, TuningStep, TransformStep]
         :param name: Name of Input or Output
         :type name: str
         :param kind: Kind of Input or Output, must be one of "input" or "output"
         :type kind: str
         :return: Input or Output path
         :rtype: str
         """
@@ -769,27 +800,30 @@
             # If TrainingStep or TuningStep
             if step_type in ("Training", "Tuning"):
                 input = step.inputs[name]
                 if isinstance(input, TrainingInput):
                     return input.config["DataSource"]["S3DataSource"]["S3Uri"]
                 else:
                     raise ValueError(f"Input {name} is not of type TrainingInput.")
+            elif step_type == "Transform":
+                return step.inputs.data
             else:
                 # If ProcessingStep
                 for input in step.inputs:
                     if input.input_name == name:
                         return input.source
                 raise ValueError(f"Input {name} not found in ProcessingStep.")
 
         elif kind == "output":
-            for output in step.outputs:
-                if output.output_name == name:
-                    return output.destination
-        else:
-            raise ValueError(f"Kind {kind} not supported. Must be one of 'input' or 'output'.")
+            if step_type == "Processing":
+                for output in step.outputs:
+                    if output.output_name == name:
+                        return output.destination
+            elif step_type == "Transform":
+                return step.transformer.output_path
 
     def run(
         self,
         sagemaker_pipeline: Pipeline,
     ) -> ValidationResult:
         """Runs validation of Step Inputs on Pipeline.
```

### Comparing `sagemaker-rightline-0.3.5/sagemaker_rightline.egg-info/PKG-INFO` & `sagemaker-rightline-0.3.6/sagemaker_rightline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,14 +42,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Test-Build-Workflow](https://github.com/stiebels/sagemaker-rightline/actions/workflows/python-package.yml/badge.svg)
 [![codecov](https://codecov.io/gh/stiebels/sagemaker-rightline/branch/main/graph/badge.svg?token=7TCW0GP1NV)](https://codecov.io/gh/stiebels/sagemaker-rightline)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/stiebels/sagemaker-rightline/issues)
+[![Documentation Status](https://readthedocs.org/projects/sagemaker-rightline/badge/?version=latest)](https://sagemaker-rightline.readthedocs.io/en/latest/?badge=latest)
 
 # sagemaker-rightline
 
 This repository contains the source code for sagemaker-rightline, a Python package that eases validation of properties of a SageMaker Pipeline object.
 
 Note that at present this package is in an early stage of development and is not yet ready for production use. We welcome contributions!
```

### Comparing `sagemaker-rightline-0.3.5/tests/test_model.py` & `sagemaker-rightline-0.3.6/tests/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,15 @@
         rule=Equals(),
         kms_key_id_expected=kms_key_alias_expected,
     )
     assert Validation.get_attribute(sagemaker_pipeline, validation.paths) == [
         kms_key_alias_expected,
         kms_key_alias_expected,
         kms_key_alias_expected,
+        kms_key_alias_expected,
     ]
 
     validation = StepImagesExist()
     assert Validation.get_attribute(sagemaker_pipeline, validation.paths) == [
         IMAGE_1_URI,
         IMAGE_2_URI,
         IMAGE_1_URI,
```

### Comparing `sagemaker-rightline-0.3.5/tests/test_rules.py` & `sagemaker-rightline-0.3.6/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.3.5/tests/test_validations.py` & `sagemaker-rightline-0.3.6/tests/test_validations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 from moto import mock_ecr, mock_iam, mock_lambda, mock_sqs
-from sagemaker.inputs import FileSystemInput, TrainingInput
+from sagemaker.inputs import FileSystemInput, TrainingInput, TransformInput
 from sagemaker.processing import NetworkConfig, ProcessingInput, ProcessingOutput
 from sagemaker.workflow.functions import Join
 from sagemaker.workflow.parameters import ParameterString
 from sagemaker.workflow.pipeline import ExecutionVariables
 
 from sagemaker_rightline.model import Validation, ValidationResult
 from sagemaker_rightline.rules import Contains, Equals
@@ -666,14 +666,34 @@
                     destination="/opt/ml/processing/input",
                     input_name="input-2",
                 ),
             ],
             "sm_processing_step_sklearn",
             False,
         ],
+        [
+            Equals,
+            [
+                TransformInput(
+                    data=f"s3://{DUMMY_BUCKET}/output-4",
+                )
+            ],
+            "sm_transform_step",
+            True,
+        ],
+        [
+            Equals,
+            [
+                TransformInput(
+                    data=f"s3://{DUMMY_BUCKET}/output-1",
+                )
+            ],
+            "sm_transform_step",
+            False,
+        ],
     ],
 )
 def test_step_inputs_as_expected_filter(
     rule, inputs_expected, step_name, success, sagemaker_pipeline
 ) -> None:
     step_inputs_validation = StepInputsAsExpected(
         inputs_expected=inputs_expected,
@@ -758,24 +778,39 @@
                     output_name="output-2",
                     source="/opt/ml/processing/output/2",
                     destination=f"s3://{DUMMY_BUCKET}/output-2",
                 ),
             ],
             False,
         ],
+        [
+            Contains,
+            [
+                f"s3://{DUMMY_BUCKET}/transformer-output",
+            ],
+            True,
+        ],
+        [
+            Contains,
+            [
+                f"s3://{DUMMY_BUCKET}/transformer-output-nope",
+            ],
+            False,
+        ],
     ],
 )
 def test_step_outputs_as_expected_no_filter(
     rule, outputs_expected, success, sagemaker_pipeline
 ) -> None:
     step_outputs_validation = StepOutputsAsExpected(
         outputs_expected=outputs_expected,
         rule=rule(),
     )
     result = step_outputs_validation.run(sagemaker_pipeline)
+    # assert result == "foo"
     assert result.success == success
 
 
 @pytest.mark.parametrize(
     "rule,outputs_expected,step_name,success",
     [
         [
@@ -837,14 +872,46 @@
 @pytest.mark.parametrize(
     "inputs_outputs_expected,success,raise_error",
     [
         [
             [
                 {
                     "input": {
+                        "step_name": "sm_transform_step",
+                        "input_name": "transform",
+                    },
+                    "output": {
+                        "step_name": "sm_processing_step_spark",
+                        "output_name": "output-2",
+                    },
+                }
+            ],
+            True,
+            False,
+        ],
+        [
+            [
+                {
+                    "input": {
+                        "step_name": "sm_processing_step_sklearn",
+                        "input_name": "input-1",
+                    },
+                    "output": {
+                        "step_name": "sm_transform_step",
+                        "output_name": "transform",
+                    },
+                }
+            ],
+            False,
+            False,
+        ],
+        [
+            [
+                {
+                    "input": {
                         "step_name": "sm_processing_step_sklearn",
                         "input_name": "input-1",
                     },
                     "output": {
                         "step_name": "sm_processing_step_sklearn",
                         "output_name": "output-1",
                     },
@@ -977,14 +1044,30 @@
                         "output_name": "output-2",
                     },
                 }
             ],
             False,
             True,
         ],
+        [
+            [
+                {
+                    "input": {
+                        "step_name": "sm_transform_step",
+                        "input_name": "transform",
+                    },
+                    "output": {
+                        "step_name": "sm_processing_step_spark",
+                        "output_name": "output-2",
+                    },
+                }
+            ],
+            True,
+            False,
+        ],
     ],
 )
 def test_step_outputs_match_inputs_as_expected(
     sagemaker_pipeline, inputs_outputs_expected, success, raise_error
 ) -> None:
     step_outputs_validation = StepOutputsMatchInputsAsExpected(
         inputs_outputs_expected=inputs_outputs_expected,
```

