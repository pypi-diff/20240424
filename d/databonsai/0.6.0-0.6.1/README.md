# Comparing `tmp/databonsai-0.6.0.tar.gz` & `tmp/databonsai-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databonsai-0.6.0.tar", last modified: Mon Apr 22 23:22:00 2024, max compression
+gzip compressed data, was "databonsai-0.6.1.tar", last modified: Wed Apr 24 20:54:36 2024, max compression
```

## Comparing `databonsai-0.6.0.tar` & `databonsai-0.6.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.690665 databonsai-0.6.0/
--rw-rw-rw-   0        0        0     1093 2024-04-05 20:10:20.000000 databonsai-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     8579 2024-04-22 23:22:00.690665 databonsai-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     7700 2024-04-22 23:08:59.000000 databonsai-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.633943 databonsai-0.6.0/databonsai/
--rw-rw-rw-   0        0        0        0 2024-04-05 20:11:02.000000 databonsai-0.6.0/databonsai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.671694 databonsai-0.6.0/databonsai/categorize/
--rw-rw-rw-   0        0        0       96 2024-04-07 00:17:28.000000 databonsai-0.6.0/databonsai/categorize/__init__.py
--rw-rw-rw-   0        0        0     8044 2024-04-22 23:04:15.000000 databonsai-0.6.0/databonsai/categorize/base_categorizer.py
--rw-rw-rw-   0        0        0     5830 2024-04-22 23:04:26.000000 databonsai-0.6.0/databonsai/categorize/multi_categorizer.py
-drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.677925 databonsai-0.6.0/databonsai/llm_providers/
--rw-rw-rw-   0        0        0      209 2024-04-18 20:42:59.000000 databonsai-0.6.0/databonsai/llm_providers/__init__.py
--rw-rw-rw-   0        0        0     6003 2024-04-18 21:09:15.000000 databonsai-0.6.0/databonsai/llm_providers/anthropic_provider.py
--rw-rw-rw-   0        0        0     1246 2024-04-18 21:04:49.000000 databonsai-0.6.0/databonsai/llm_providers/llm_provider.py
--rw-rw-rw-   0        0        0     3950 2024-04-18 21:09:34.000000 databonsai-0.6.0/databonsai/llm_providers/ollama_provider.py
--rw-rw-rw-   0        0        0     6266 2024-04-22 23:05:34.000000 databonsai-0.6.0/databonsai/llm_providers/openai_provider.py
-drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.681842 databonsai-0.6.0/databonsai/transform/
--rw-rw-rw-   0        0        0      100 2024-04-22 22:21:51.000000 databonsai-0.6.0/databonsai/transform/__init__.py
--rw-rw-rw-   0        0        0     5650 2024-04-22 20:55:37.000000 databonsai-0.6.0/databonsai/transform/base_transformer.py
--rw-rw-rw-   0        0        0     9868 2024-04-22 22:12:09.000000 databonsai-0.6.0/databonsai/transform/extract_transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.684594 databonsai-0.6.0/databonsai/utils/
--rw-rw-rw-   0        0        0       86 2024-04-22 21:08:24.000000 databonsai-0.6.0/databonsai/utils/__init__.py
--rw-rw-rw-   0        0        0    10520 2024-04-22 23:06:15.000000 databonsai-0.6.0/databonsai/utils/apply.py
-drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.688984 databonsai-0.6.0/databonsai.egg-info/
--rw-rw-rw-   0        0        0     8579 2024-04-22 23:22:00.000000 databonsai-0.6.0/databonsai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2024-04-22 23:22:00.000000 databonsai-0.6.0/databonsai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 23:22:00.000000 databonsai-0.6.0/databonsai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-22 23:22:00.000000 databonsai-0.6.0/databonsai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-22 23:22:00.000000 databonsai-0.6.0/databonsai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      580 2024-04-22 23:21:13.000000 databonsai-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 23:22:00.690665 databonsai-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1054 2024-04-22 23:21:19.000000 databonsai-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 23:22:00.686090 databonsai-0.6.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-14 19:59:02.000000 databonsai-0.6.0/tests/__init__.py
--rw-rw-rw-   0        0        0     8831 2024-04-17 05:12:32.000000 databonsai-0.6.0/tests/test_categorization.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.676715 databonsai-0.6.1/
+-rw-rw-rw-   0        0        0     1093 2024-04-05 20:10:20.000000 databonsai-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     8579 2024-04-24 20:54:36.675716 databonsai-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7700 2024-04-22 23:08:59.000000 databonsai-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.619974 databonsai-0.6.1/databonsai/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:11:02.000000 databonsai-0.6.1/databonsai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.656737 databonsai-0.6.1/databonsai/categorize/
+-rw-rw-rw-   0        0        0       96 2024-04-07 00:17:28.000000 databonsai-0.6.1/databonsai/categorize/__init__.py
+-rw-rw-rw-   0        0        0     8937 2024-04-24 20:53:10.000000 databonsai-0.6.1/databonsai/categorize/base_categorizer.py
+-rw-rw-rw-   0        0        0     5830 2024-04-24 19:19:34.000000 databonsai-0.6.1/databonsai/categorize/multi_categorizer.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.663900 databonsai-0.6.1/databonsai/llm_providers/
+-rw-rw-rw-   0        0        0      209 2024-04-18 20:42:59.000000 databonsai-0.6.1/databonsai/llm_providers/__init__.py
+-rw-rw-rw-   0        0        0     6003 2024-04-18 21:09:15.000000 databonsai-0.6.1/databonsai/llm_providers/anthropic_provider.py
+-rw-rw-rw-   0        0        0     1246 2024-04-18 21:04:49.000000 databonsai-0.6.1/databonsai/llm_providers/llm_provider.py
+-rw-rw-rw-   0        0        0     3950 2024-04-18 21:09:34.000000 databonsai-0.6.1/databonsai/llm_providers/ollama_provider.py
+-rw-rw-rw-   0        0        0     6266 2024-04-22 23:05:34.000000 databonsai-0.6.1/databonsai/llm_providers/openai_provider.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.666761 databonsai-0.6.1/databonsai/transform/
+-rw-rw-rw-   0        0        0      100 2024-04-22 22:21:51.000000 databonsai-0.6.1/databonsai/transform/__init__.py
+-rw-rw-rw-   0        0        0     5650 2024-04-22 20:55:37.000000 databonsai-0.6.1/databonsai/transform/base_transformer.py
+-rw-rw-rw-   0        0        0     9868 2024-04-22 22:12:09.000000 databonsai-0.6.1/databonsai/transform/extract_transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.669716 databonsai-0.6.1/databonsai/utils/
+-rw-rw-rw-   0        0        0       86 2024-04-24 19:46:10.000000 databonsai-0.6.1/databonsai/utils/__init__.py
+-rw-rw-rw-   0        0        0     9781 2024-04-24 20:49:28.000000 databonsai-0.6.1/databonsai/utils/apply.py
+-rw-rw-rw-   0        0        0      256 2024-04-24 19:58:30.000000 databonsai-0.6.1/databonsai/utils/logs.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.673715 databonsai-0.6.1/databonsai.egg-info/
+-rw-rw-rw-   0        0        0     8579 2024-04-24 20:54:36.000000 databonsai-0.6.1/databonsai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2024-04-24 20:54:36.000000 databonsai-0.6.1/databonsai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 20:54:36.000000 databonsai-0.6.1/databonsai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-24 20:54:36.000000 databonsai-0.6.1/databonsai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-24 20:54:36.000000 databonsai-0.6.1/databonsai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      580 2024-04-24 19:08:15.000000 databonsai-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 20:54:36.677715 databonsai-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2024-04-24 19:08:19.000000 databonsai-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:54:36.671714 databonsai-0.6.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-14 19:59:02.000000 databonsai-0.6.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     8831 2024-04-17 05:12:32.000000 databonsai-0.6.1/tests/test_categorization.py
```

### Comparing `databonsai-0.6.0/LICENSE` & `databonsai-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.0/PKG-INFO` & `databonsai-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databonsai
-Version: 0.6.0
+Version: 0.6.1
 Summary: A package for cleaning and curating data with LLMs
 Home-page: https://github.com/databonsai/databonsai
 Author: Alvin Ryanputra
 Author-email: databonsai.ai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `databonsai-0.6.0/README.md` & `databonsai-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.0/databonsai/categorize/base_categorizer.py` & `databonsai-0.6.1/databonsai/categorize/base_categorizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Dict, List, Optional
 from pydantic import BaseModel, field_validator, model_validator, computed_field
 from databonsai.llm_providers import OpenAIProvider, LLMProvider
-from pydantic import ConfigDict
-from pydantic.dataclasses import dataclass
+from databonsai.utils.logs import logger
 
 
 class BaseCategorizer(BaseModel):
     """
     A base class for categorizing input data using a specified LLM provider.
 
     Attributes:
@@ -14,14 +13,15 @@
         llm_provider (LLMProvider): An instance of an LLM provider to be used for categorization.
 
     """
 
     categories: Dict[str, str]
     llm_provider: LLMProvider
     examples: Optional[List[Dict[str, str]]] = []
+    strict: bool = True
 
     class Config:
         arbitrary_types_allowed = True
 
     @field_validator("categories")
     def validate_categories(cls, v):
         """
@@ -145,17 +145,22 @@
         """
         # Call the LLM provider to get the predicted category
         response = self.llm_provider.generate(self.system_message, input_data)
         predicted_category = response.strip()
 
         # Validate that the predicted category is one of the provided categories
         if predicted_category not in self.categories:
-            raise ValueError(
-                f"Predicted category '{predicted_category}' is not one of the provided categories."
-            )
+            if self.strict:
+                raise ValueError(
+                    f"Predicted category '{predicted_category}' is not one of the provided categories. Use 'strict=False' when instantiating the categorizer to allow categories not in the categories dict."
+                )
+            else:
+                logger.warning(
+                    f"Predicted category '{predicted_category}' is not one of the provided categories. Use 'strict=True' when instantiating the categorizer to raise an error."
+                )
 
         return predicted_category
 
     def categorize_batch(self, input_data: List[str]) -> List[str]:
         """
         Categorizes a batch of input data using the specified LLM provider. For less advanced LLMs, call this method on batches of 3-5 inputs (depending on the length of the input data).
 
@@ -189,11 +194,17 @@
         filtered_categories = [
             category for category in predicted_categories if category
         ]
 
         # Validate each category in the filtered list
         for predicted_category in filtered_categories:
             if predicted_category not in self.categories:
-                raise ValueError(
-                    f"Predicted category '{predicted_category}' is not one of the provided categories."
-                )
+                if self.strict:
+                    raise ValueError(
+                        f"Predicted category '{predicted_category}' is not one of the provided categories. Use 'strict=False' when instantiating the categorizer to allow categories not in the categories dict."
+                    )
+                else:
+                    # Warn the user if the predicted category is not one of the provided categories
+                    logger.warning(
+                        f"Predicted category '{predicted_category}' is not one of the provided categories. Use 'strict=True' when instantiating the categorizer to raise an error."
+                    )
         return filtered_categories
```

### Comparing `databonsai-0.6.0/databonsai/categorize/multi_categorizer.py` & `databonsai-0.6.1/databonsai/categorize/multi_categorizer.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.0/databonsai/llm_providers/anthropic_provider.py` & `databonsai-0.6.1/databonsai/llm_providers/anthropic_provider.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.0/databonsai/llm_providers/llm_provider.py` & `databonsai-0.6.1/databonsai/llm_providers/llm_provider.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.0/databonsai/llm_providers/ollama_provider.py` & `databonsai-0.6.1/databonsai/llm_providers/ollama_provider.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.0/databonsai/llm_providers/openai_provider.py` & `databonsai-0.6.1/databonsai/llm_providers/openai_provider.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.0/databonsai/transform/base_transformer.py` & `databonsai-0.6.1/databonsai/transform/base_transformer.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.0/databonsai/transform/extract_transformer.py` & `databonsai-0.6.1/databonsai/transform/extract_transformer.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.6.0/databonsai/utils/apply.py` & `databonsai-0.6.1/databonsai/utils/apply.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from tqdm import tqdm
-from databonsai.categorize import BaseCategorizer
-from databonsai.transform import BaseTransformer, ExtractTransformer
 from typing import List, Callable, Union, get_origin
 import inspect
 
 
 def apply_to_column(
     input_column: List,
     output_column: List,
@@ -36,24 +34,18 @@
     if len(output_column) > len(input_column):
         raise ValueError(
             f"The length of the output_column ({len(output_column)}) is greater than the length of the input_column ({len(input_column)})."
         )
 
     success_idx = start_idx
 
-    if isinstance(func.__self__, BaseCategorizer):
-        desc = "Categorizing"
-    elif isinstance(func.__self__, BaseTransformer):
-        desc = "Transforming"
-    else:
-        desc = "Processing"
-
     try:
         for idx, value in enumerate(
-            tqdm(input_column[start_idx:], desc=desc, unit="row"), start=start_idx
+            tqdm(input_column[start_idx:], desc="Processing data..", unit="row"),
+            start=start_idx,
         ):
             result = func(value)
 
             if idx >= len(output_column):
                 output_column.append(result)
             else:
                 output_column[idx] = result
@@ -66,25 +58,25 @@
 
     return success_idx
 
 
 def apply_to_column_batch(
     input_column: List,
     output_column: List,
-    batch_func: Callable,
+    func: Callable,
     batch_size: int = 5,
     start_idx: int = 0,
 ) -> int:
     """
     Apply a function to each batch of values in a column of a DataFrame or a normal Python list, starting from a specified index.
 
     Parameters:
         input_column (List): The column of the DataFrame or a normal Python list to apply the function to.
         output_column (List): A list to store the processed values. The function will mutate this list in-place.
-        batch_func (callable): The batch function to apply to each batch of values in the column.
+        func (callable): The batch function to apply to each batch of values in the column.
                          The function should take a list of values as input and return a list of processed values.
         batch_size (int, optional): The size of each batch. Default is 5.
         start_idx (int, optional): The index from which to start applying the function. Default is 0.
 
     Returns:
         tuple: A tuple containing two elements:
                - success_idx (int): The index of the last successfully processed batch.
@@ -96,30 +88,24 @@
     if start_idx >= len(input_column):
         raise ValueError(
             f"start_idx ({start_idx}) is greater than or equal to the length of the input_column ({len(input_column)})."
         )
 
     if len(output_column) > len(input_column):
         raise ValueError(
-            f"The length of the output_column list ({len(output_column)}) is greater than the length of th input_column ({len(column)})."
+            f"The length of the output_column list ({len(output_column)}) is greater than the length of th input_column ({len(input_column)})."
         )
 
-    check_batch_func(batch_func)
+    check_func(func)
     success_idx = start_idx
-
-    if isinstance(batch_func.__self__, BaseCategorizer):
-        desc = "Categorizing"
-    elif isinstance(batch_func.__self__, BaseTransformer):
-        desc = "Transforming"
-    else:
-        desc = "Processing"
-
     try:
         for i in tqdm(
-            range(start_idx, len(input_column), batch_size), desc=desc, unit="batch"
+            range(start_idx, len(input_column), batch_size),
+            desc="Processing data..",
+            unit="batch",
         ):
             batch_end = min(i + batch_size, len(input_column))
             batch = input_column[i:batch_end]
             batch_result = func(batch)
             if i >= len(output_column):
                 output_column.extend(batch_result)
             else:
@@ -132,15 +118,15 @@
 
     return min(success_idx, len(input_column))
 
 
 def apply_to_column_autobatch(
     input_column: List,
     output_column: List,
-    batch_func: Callable,
+    func: Callable,
     max_retries: int = 3,
     max_batch_size: int = 5,
     batch_size: int = 2,
     ramp_factor: float = 1.5,
     ramp_factor_decay: float = 0.8,
     reduce_factor: float = 0.5,
     reduce_factor_decay: float = 0.8,
@@ -153,16 +139,16 @@
     specified index. It adaptively adjusts the batch size based on the success or failure of
     each batch processing attempt. The function retries failed batches with a reduced batch
     size and gradually decreases the rate of batch size adjustment over time.
 
     Parameters:
         input_column (List): The input column to be processed.
         output_column (List): The list to store the processed results.
-        instance (Union[BaseCategorizer, BaseTransformer]): An instance of BaseCategorizer or BaseTransformer
-                                                             containing the batch processing function.
+        func (callable): The batch function to apply to each batch of values in the column.
+                         The function should take a list of values as input and return a list of processed values.
         max_retries (int): The maximum number of retries for failed batches.
         max_batch_size (int): The maximum allowed batch size.
         batch_size (int): The initial batch size.
         ramp_factor (float): The factor by which the batch size is increased after a successful batch.
         ramp_factor_decay (float): The decay rate for the ramp factor after each successful batch.
         reduce_factor (float): The factor by which the batch size is reduced after a failed batch.
         reduce_factor_decay (float): The decay rate for the reduce factor after each failed batch.
@@ -181,38 +167,33 @@
         )
 
     if len(output_column) > len(input_column):
         raise ValueError(
             f"The length of the output_column list ({len(output_column)}) is greater than the length of the input_column ({len(input_column)})."
         )
 
-    if isinstance(batch_func.__self__, BaseCategorizer):
-        desc = "Categorizing"
-    elif isinstance(batch_func.__self__, BaseTransformer):
-        desc = "Transforming"
-    else:
-        desc = "Processing"
-
-    check_batch_func(batch_func)
+    check_func(func)
     success_idx = start_idx
     ramp_factor = ramp_factor
     reduce_factor = reduce_factor
 
     try:
         remaining_data = input_column[start_idx:]
         processed_results = []
         batch_size = batch_size
         retry_count = 0
 
-        with tqdm(total=len(remaining_data), desc=desc, unit="row") as pbar:
+        with tqdm(
+            total=len(remaining_data), desc="Processing data..", unit="row"
+        ) as pbar:
             while len(remaining_data) > 0:
                 try:
                     batch_size = min(batch_size, len(remaining_data))
                     batch = remaining_data[:batch_size]
-                    batch_results = batch_func(batch)
+                    batch_results = func(batch)
                     processed_results.extend(batch_results)
                     remaining_data = remaining_data[batch_size:]
                     retry_count = 0
 
                     # Update progress bar
                     pbar.update(batch_size)
 
@@ -239,20 +220,20 @@
         print(f"Error occurred at batch starting at index {success_idx}: {str(e)}")
         print(f"Processing stopped at batch ending at index {success_idx - 1}")
         return success_idx
 
     return min(success_idx, len(input_column))
 
 
-def check_batch_func(batch_func):
-    if not inspect.signature(batch_func).parameters:
+def check_func(func):
+    if not inspect.signature(func).parameters:
         raise TypeError("The provided function does not take any arguments.")
 
     # Ensure func is a batch function that takes a list
-    first_param = list(inspect.signature(batch_func).parameters.values())[0]
+    first_param = list(inspect.signature(func).parameters.values())[0]
     param_annotation = first_param.annotation
     origin = get_origin(param_annotation)
 
     if origin is not get_origin(List):
         raise TypeError(
             "The provided function does not take a list or pandas.Series as input."
         )
```

### Comparing `databonsai-0.6.0/databonsai.egg-info/PKG-INFO` & `databonsai-0.6.1/databonsai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databonsai
-Version: 0.6.0
+Version: 0.6.1
 Summary: A package for cleaning and curating data with LLMs
 Home-page: https://github.com/databonsai/databonsai
 Author: Alvin Ryanputra
 Author-email: databonsai.ai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `databonsai-0.6.0/databonsai.egg-info/SOURCES.txt` & `databonsai-0.6.1/databonsai.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 databonsai/llm_providers/ollama_provider.py
 databonsai/llm_providers/openai_provider.py
 databonsai/transform/__init__.py
 databonsai/transform/base_transformer.py
 databonsai/transform/extract_transformer.py
 databonsai/utils/__init__.py
 databonsai/utils/apply.py
+databonsai/utils/logs.py
 tests/__init__.py
 tests/test_categorization.py
```

### Comparing `databonsai-0.6.0/pyproject.toml` & `databonsai-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databonsai"
-version = "0.6.0"
+version = "0.6.1"
 description = "A Python package to clean and curate your data with LLMs"
 authors = ["Alvin Ryanputra <databonsai.ai@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"  
 
 openai = "^1.16.2"
```

### Comparing `databonsai-0.6.0/setup.py` & `databonsai-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="databonsai",
-    version="0.6.0",
+    version="0.6.1",
     description="A package for cleaning and curating data with LLMs",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Alvin Ryanputra",
     author_email="databonsai.ai@gmail.com",
     url="https://github.com/databonsai/databonsai",
     packages=find_packages(),
```

### Comparing `databonsai-0.6.0/tests/test_categorization.py` & `databonsai-0.6.1/tests/test_categorization.py`

 * *Files identical despite different names*

