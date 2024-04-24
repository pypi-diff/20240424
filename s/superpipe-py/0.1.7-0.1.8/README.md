# Comparing `tmp/superpipe_py-0.1.7.tar.gz` & `tmp/superpipe_py-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpipe_py-0.1.7.tar", max compression
+gzip compressed data, was "superpipe_py-0.1.8.tar", max compression
```

## Comparing `superpipe_py-0.1.7.tar` & `superpipe_py-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     8241 2024-03-26 02:12:03.580726 superpipe_py-0.1.7/README.md
--rw-r--r--   0        0        0      830 2024-04-19 17:21:07.867395 superpipe_py-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      153 2024-03-25 15:10:35.189973 superpipe_py-0.1.7/superpipe/__init__.py
--rw-r--r--   0        0        0     2286 2024-03-29 17:34:38.528585 superpipe_py-0.1.7/superpipe/clients.py
--rw-r--r--   0        0        0      466 2024-04-19 17:21:07.867817 superpipe_py-0.1.7/superpipe/config.py
--rw-r--r--   0        0        0     6112 2024-03-25 20:28:08.394089 superpipe_py-0.1.7/superpipe/grid_search.py
--rw-r--r--   0        0        0     7311 2024-03-29 17:34:38.528991 superpipe_py-0.1.7/superpipe/llm.py
--rw-r--r--   0        0        0     1363 2024-03-28 23:49:05.058152 superpipe_py-0.1.7/superpipe/models.py
--rw-r--r--   0        0        0     7274 2024-04-19 17:21:07.868179 superpipe_py-0.1.7/superpipe/pipeline.py
--rw-r--r--   0        0        0     2505 2024-03-07 18:22:24.182418 superpipe_py-0.1.7/superpipe/pydantic.py
--rw-r--r--   0        0        0      188 2024-03-25 15:10:35.191485 superpipe_py-0.1.7/superpipe/steps/__init__.py
--rw-r--r--   0        0        0     2480 2024-04-19 17:21:07.868423 superpipe_py-0.1.7/superpipe/steps/custom.py
--rw-r--r--   0        0        0     5397 2024-04-19 17:21:07.868646 superpipe_py-0.1.7/superpipe/steps/embedding_search.py
--rw-r--r--   0        0        0     3582 2024-04-19 17:21:07.868811 superpipe_py-0.1.7/superpipe/steps/llm_step.py
--rw-r--r--   0        0        0     4489 2024-04-19 17:21:07.869026 superpipe_py-0.1.7/superpipe/steps/llm_structured.py
--rw-r--r--   0        0        0     4627 2024-04-19 17:21:07.869241 superpipe_py-0.1.7/superpipe/steps/llm_structured_composite.py
--rw-r--r--   0        0        0     3721 2024-04-19 17:21:07.869411 superpipe_py-0.1.7/superpipe/steps/serp.py
--rw-r--r--   0        0        0     6283 2024-04-19 17:21:07.869666 superpipe_py-0.1.7/superpipe/steps/step.py
--rw-r--r--   0        0        0     2173 2024-03-25 20:28:08.395135 superpipe_py-0.1.7/superpipe/steps/utils.py
--rw-r--r--   0        0        0     1854 2024-03-20 15:30:05.901744 superpipe_py-0.1.7/superpipe/util.py
--rw-r--r--   0        0        0     9165 1970-01-01 00:00:00.000000 superpipe_py-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     8241 2024-03-26 02:12:03.580726 superpipe_py-0.1.8/README.md
+-rw-r--r--   0        0        0      830 2024-04-24 17:30:12.850203 superpipe_py-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      153 2024-03-25 15:10:35.189973 superpipe_py-0.1.8/superpipe/__init__.py
+-rw-r--r--   0        0        0     2286 2024-03-29 17:34:38.528585 superpipe_py-0.1.8/superpipe/clients.py
+-rw-r--r--   0        0        0      466 2024-04-19 17:21:07.867817 superpipe_py-0.1.8/superpipe/config.py
+-rw-r--r--   0        0        0     6112 2024-03-25 20:28:08.394089 superpipe_py-0.1.8/superpipe/grid_search.py
+-rw-r--r--   0        0        0     7311 2024-03-29 17:34:38.528991 superpipe_py-0.1.8/superpipe/llm.py
+-rw-r--r--   0        0        0     1363 2024-03-28 23:49:05.058152 superpipe_py-0.1.8/superpipe/models.py
+-rw-r--r--   0        0        0     7496 2024-04-24 17:30:12.850546 superpipe_py-0.1.8/superpipe/pipeline.py
+-rw-r--r--   0        0        0     2505 2024-03-07 18:22:24.182418 superpipe_py-0.1.8/superpipe/pydantic.py
+-rw-r--r--   0        0        0      188 2024-03-25 15:10:35.191485 superpipe_py-0.1.8/superpipe/steps/__init__.py
+-rw-r--r--   0        0        0     2480 2024-04-19 17:21:07.868423 superpipe_py-0.1.8/superpipe/steps/custom.py
+-rw-r--r--   0        0        0     5397 2024-04-19 17:21:07.868646 superpipe_py-0.1.8/superpipe/steps/embedding_search.py
+-rw-r--r--   0        0        0     3582 2024-04-19 17:21:07.868811 superpipe_py-0.1.8/superpipe/steps/llm_step.py
+-rw-r--r--   0        0        0     4489 2024-04-24 16:56:02.588805 superpipe_py-0.1.8/superpipe/steps/llm_structured.py
+-rw-r--r--   0        0        0     4627 2024-04-19 17:21:07.869241 superpipe_py-0.1.8/superpipe/steps/llm_structured_composite.py
+-rw-r--r--   0        0        0     3721 2024-04-19 17:21:07.869411 superpipe_py-0.1.8/superpipe/steps/serp.py
+-rw-r--r--   0        0        0     6289 2024-04-24 17:30:12.850879 superpipe_py-0.1.8/superpipe/steps/step.py
+-rw-r--r--   0        0        0     2173 2024-03-25 20:28:08.395135 superpipe_py-0.1.8/superpipe/steps/utils.py
+-rw-r--r--   0        0        0     1854 2024-03-20 15:30:05.901744 superpipe_py-0.1.8/superpipe/util.py
+-rw-r--r--   0        0        0     9165 1970-01-01 00:00:00.000000 superpipe_py-0.1.8/PKG-INFO
```

### Comparing `superpipe_py-0.1.7/README.md` & `superpipe_py-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/pyproject.toml` & `superpipe_py-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "superpipe-py"
-version = "0.1.7"
+version = "0.1.8"
 description = "build unstructured to structured data transformation pipelines"
 authors = ["Aman Dhesi <aman@stelolabs.com>"]
 license = "MIT"
 packages = [{ include = "superpipe" }]
 readme = "README.md"
 repository = "https://github.com/villagecomputing/superpipe"
```

### Comparing `superpipe_py-0.1.7/superpipe/clients.py` & `superpipe_py-0.1.8/superpipe/clients.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/superpipe/grid_search.py` & `superpipe_py-0.1.8/superpipe/grid_search.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/superpipe/llm.py` & `superpipe_py-0.1.8/superpipe/llm.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/superpipe/models.py` & `superpipe_py-0.1.8/superpipe/models.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/superpipe/pipeline.py` & `superpipe_py-0.1.8/superpipe/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,21 @@
         evaluate(evaluation_fn=None): Evaluates the processed data using an evaluation function.
         _aggregate_statistics(data): Aggregates statistics from the pipeline steps.
     """
 
     def __init__(self,
                  steps: List[Step],
                  evaluation_fn: Callable[[any], Union[bool, float]] = None,
+                 output_fields: List[str] = None,
                  name: str = None):
+        if len(steps) == 0:
+            raise ValueError("Pipeline must contain at least one step")
         self.steps = steps
         self.evaluation_fn = evaluation_fn
+        self.output_fields = output_fields or steps[-1].output_fields()
         self.data = None
         self.score = None
         self.name = name or self.__class__.__name__
         self.statistics = PipelineStatistics()
 
     def run(self, data: Union[pd.DataFrame, Dict], enable_logging=False, row_wise=True, verbose=True):
         def run_steps(row):
```

### Comparing `superpipe_py-0.1.7/superpipe/pydantic.py` & `superpipe_py-0.1.8/superpipe/pydantic.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/superpipe/steps/custom.py` & `superpipe_py-0.1.8/superpipe/steps/custom.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/superpipe/steps/embedding_search.py` & `superpipe_py-0.1.8/superpipe/steps/embedding_search.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/superpipe/steps/llm_step.py` & `superpipe_py-0.1.8/superpipe/steps/llm_step.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/superpipe/steps/llm_structured.py` & `superpipe_py-0.1.8/superpipe/steps/llm_structured.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/superpipe/steps/llm_structured_composite.py` & `superpipe_py-0.1.8/superpipe/steps/llm_structured_composite.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/superpipe/steps/serp.py` & `superpipe_py-0.1.8/superpipe/steps/serp.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/superpipe/steps/step.py` & `superpipe_py-0.1.8/superpipe/steps/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def reset_statistics(self):
         """
         Resets the statistics for the step.
         """
         self.statistics = StepStatistics()
 
-    def outputs(self):
+    def output_fields(self):
         """
         Returns the fields that the step outputs.
 
         Returns:
             List[str]: A list of field names.
         """
         if hasattr(self, "out_schema"):
```

### Comparing `superpipe_py-0.1.7/superpipe/steps/utils.py` & `superpipe_py-0.1.8/superpipe/steps/utils.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/superpipe/util.py` & `superpipe_py-0.1.8/superpipe/util.py`

 * *Files identical despite different names*

### Comparing `superpipe_py-0.1.7/PKG-INFO` & `superpipe_py-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpipe-py
-Version: 0.1.7
+Version: 0.1.8
 Summary: build unstructured to structured data transformation pipelines
 Home-page: https://github.com/villagecomputing/superpipe
 License: MIT
 Author: Aman Dhesi
 Author-email: aman@stelolabs.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

