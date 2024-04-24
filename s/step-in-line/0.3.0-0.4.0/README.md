# Comparing `tmp/step_in_line-0.3.0.tar.gz` & `tmp/step_in_line-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "step_in_line-0.3.0.tar", max compression
+gzip compressed data, was "step_in_line-0.4.0.tar", max compression
```

## Comparing `step_in_line-0.3.0.tar` & `step_in_line-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     3550 2024-04-22 21:12:53.938317 step_in_line-0.3.0/README.md
--rw-r--r--   0        0        0      505 2024-04-22 21:13:07.274193 step_in_line-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 21:12:53.938317 step_in_line-0.3.0/step_in_line/__init__.py
--rw-r--r--   0        0        0     5414 2024-04-22 21:12:53.938317 step_in_line-0.3.0/step_in_line/pipeline.py
--rw-r--r--   0        0        0     5158 2024-04-22 21:12:53.938317 step_in_line-0.3.0/step_in_line/step.py
--rw-r--r--   0        0        0      935 2024-04-22 21:12:53.938317 step_in_line-0.3.0/step_in_line/template_lambda.py
--rw-r--r--   0        0        0    13432 2024-04-22 21:12:53.938317 step_in_line-0.3.0/step_in_line/tf.py
--rw-r--r--   0        0        0     4215 1970-01-01 00:00:00.000000 step_in_line-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-24 17:28:16.698818 step_in_line-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3593 2024-04-24 17:28:16.698818 step_in_line-0.4.0/README.md
+-rw-r--r--   0        0        0      505 2024-04-24 17:28:29.522910 step_in_line-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 17:28:16.698818 step_in_line-0.4.0/step_in_line/__init__.py
+-rw-r--r--   0        0        0     4855 2024-04-24 17:28:16.698818 step_in_line-0.4.0/step_in_line/pipeline.py
+-rw-r--r--   0        0        0     4818 2024-04-24 17:28:16.698818 step_in_line-0.4.0/step_in_line/step.py
+-rw-r--r--   0        0        0      935 2024-04-24 17:28:16.698818 step_in_line-0.4.0/step_in_line/template_lambda.py
+-rw-r--r--   0        0        0    13470 2024-04-24 17:28:16.698818 step_in_line-0.4.0/step_in_line/tf.py
+-rw-r--r--   0        0        0     4258 1970-01-01 00:00:00.000000 step_in_line-0.4.0/PKG-INFO
```

### Comparing `step_in_line-0.3.0/README.md` & `step_in_line-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 app = App(hcl_output=True)
 
 # function names must be unique, or you can pass a name to the step to 
 # ensure uniqueness
 @step(
     name = "preprocess_unique",
     python_runtime = "python3.9", # defaults to 3.10
+    memory_size = "128", # defaults to 512
     layers = ["arn:aws:lambda:us-east-2:123456789012:layer:example-layer"]
 )
 def preprocess(arg1: str) -> str:
     # do stuff here, eg run some sql code against snowflake.  
     # Make sure to "import snowflake" within this function.  
     # Will need a "layer" passed which contains the snowflake
     # dependencies.  Must run in <15 minutes.
```

### Comparing `step_in_line-0.3.0/step_in_line/step.py` & `step_in_line-0.4.0/step_in_line/step.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,51 @@
-## based on Sagemaker Pipeline syntax
-# Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License"). You
-# may not use this file except in compliance with the License. A copy of
-# the License is located at
-#
-#     http://aws.amazon.com/apache2.0/
-#
-# or in the "license" file accompanying this file. This file is
-# distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
-# ANY KIND, either express or implied. See the License for the specific
-# language governing permissions and limitations under the License.
 from __future__ import absolute_import
 
 from typing import List, Optional, Callable, Any, Dict
 
-# from .utilities import unique_name_from_base_uuid4
 from functools import wraps
 
 
 class Step:
     """`Step` for step function workflows"""
 
     def __init__(
         self,
         name: str,
         func: Callable,
         args: List[Any],
         python_runtime: str,
+        memory_size: int = 512,
         description: Optional[str] = None,
         retry_count: int = 0,
         layers: List[str] = [],
         env_variables: Dict[str, str] = {},  # to pass in to lambda
         depends_on: Optional[List["Step"]] = None,
     ):
         """Initialize a Step
 
         Args:
             name (str): The name of the `Step`.
             func (callable): The function that should be executed as part of this step
             args (list): The arguments to the function.  If not a step, these are considered "static" and are used even in the Step Function execution
             python_runtime (str): Lambda runtime.
+            memory_size (int): Megabytes of memory for the lambda.  Defaults to 512.
             description (str): The description of the `Step`.
             retry_count (int): Number of times to retry a failure
             layers (list): the ARNs of layers to add to the lambda function
             env_variables (dict): environment variables to pass to lambda function
             depends_on (List[Step]): The list of Steps that the current `Step` depends on.
         """
         self.name = name
         self.description = description
         self.retry_count = retry_count
         self.layers = layers
         self.func = func
         self.args = args
+        self.memory_size = memory_size
         self.python_runtime = python_runtime
         self.env_variables = env_variables
         if depends_on is not None:
             self._depends_on = depends_on
         else:
             self._depends_on = None
 
@@ -92,27 +81,30 @@
 def step(
     _func=None,
     *,
     name: Optional[str] = None,
     description: Optional[str] = None,
     layers: Optional[List[str]] = None,
     python_runtime: str = "python3.10",
+    memory_size: int = 512,
     retry_count: int = 0,
     env_variables: Dict[str, str] = {}
 ):
     """Decorator for converting a python function to a pipeline step.
 
     This decorator wraps the annotated code into a `Step` object which can then be passed
     to a pipeline as a step.
 
     Args:
         _func: A Python function to run as a SageMaker pipeline step.
         name (str): Name of the pipeline step. Defaults to a generated name using function name and uuid4 identifier to avoid duplicates.
         description (str): Description of the step
         layers (list): Lambda layers
+        python_runtime (str): Lambda runtime.
+        memory_size (int): Megabytes of memory for the lambda.  Defaults to 512.
         retry_count (int): number of retries to attempt.  Defaults to 0 (no retries).
         env_variables (dict): environment variables to pass to lambda function
 
     """
 
     def _step(func):
         @wraps(func)
```

### Comparing `step_in_line-0.3.0/step_in_line/template_lambda.py` & `step_in_line-0.4.0/step_in_line/template_lambda.py`

 * *Files identical despite different names*

### Comparing `step_in_line-0.3.0/step_in_line/tf.py` & `step_in_line-0.4.0/step_in_line/tf.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
     return lambda_function.LambdaFunction(
         scope,
         step.name,
         function_name=f"{name_prefix}_{step.name}",
         role=lambda_role.arn,
         filename=lambda_filename,
         timeout=900,
+        memory_size=step.memory_size,
         runtime=step.python_runtime,
         handler=lambda_handler,
         vpc_config=vpc_config,
         layers=step.layers,
         source_code_hash=sha256_hash,
         environment=step.env_variables,
     )
```

### Comparing `step_in_line-0.3.0/PKG-INFO` & `step_in_line-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: step-in-line
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: Daniel Stahl
 Author-email: danstahl1138@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -34,14 +34,15 @@
 app = App(hcl_output=True)
 
 # function names must be unique, or you can pass a name to the step to 
 # ensure uniqueness
 @step(
     name = "preprocess_unique",
     python_runtime = "python3.9", # defaults to 3.10
+    memory_size = "128", # defaults to 512
     layers = ["arn:aws:lambda:us-east-2:123456789012:layer:example-layer"]
 )
 def preprocess(arg1: str) -> str:
     # do stuff here, eg run some sql code against snowflake.  
     # Make sure to "import snowflake" within this function.  
     # Will need a "layer" passed which contains the snowflake
     # dependencies.  Must run in <15 minutes.
```

