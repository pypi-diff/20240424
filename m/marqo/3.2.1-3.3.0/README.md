# Comparing `tmp/marqo-3.2.1.tar.gz` & `tmp/marqo-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marqo-3.2.1.tar", last modified: Fri Apr  5 04:18:49 2024, max compression
+gzip compressed data, was "marqo-3.3.0.tar", last modified: Wed Apr 24 06:45:45 2024, max compression
```

## Comparing `marqo-3.2.1.tar` & `marqo-3.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:18:49.196438 marqo-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-05 04:18:40.000000 marqo-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-04-05 04:18:49.192438 marqo-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-04-05 04:18:40.000000 marqo-3.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-05 04:18:40.000000 marqo-3.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 04:18:49.196438 marqo-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-05 04:18:40.000000 marqo-3.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:18:49.188438 marqo-3.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:18:49.192438 marqo-3.2.1/src/marqo/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/cloud_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/default_instance_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    35873 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/instance_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/marqo_cloud_instance_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/marqo_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:18:49.192438 marqo-3.2.1/src/marqo/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/models/create_index_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/models/marqo_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/models/marqo_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/models/marqo_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/models/search_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-05 04:18:40.000000 marqo-3.2.1/src/marqo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:18:49.192438 marqo-3.2.1/src/marqo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-04-05 04:18:49.000000 marqo-3.2.1/src/marqo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-05 04:18:49.000000 marqo-3.2.1/src/marqo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 04:18:49.000000 marqo-3.2.1/src/marqo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 04:18:49.000000 marqo-3.2.1/src/marqo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 04:18:49.000000 marqo-3.2.1/src/marqo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:45:45.858079 marqo-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-24 06:45:38.000000 marqo-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-04-24 06:45:45.858079 marqo-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-04-24 06:45:38.000000 marqo-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-24 06:45:38.000000 marqo-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 06:45:45.858079 marqo-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-24 06:45:38.000000 marqo-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:45:45.850079 marqo-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:45:45.854079 marqo-3.3.0/src/marqo/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/cloud_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/default_instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42344 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/marqo_cloud_instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/marqo_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:45:45.854079 marqo-3.3.0/src/marqo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/models/create_index_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/models/marqo_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/models/marqo_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/models/marqo_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/models/search_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:45:45.858079 marqo-3.3.0/src/marqo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-04-24 06:45:45.000000 marqo-3.3.0/src/marqo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-24 06:45:45.000000 marqo-3.3.0/src/marqo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 06:45:45.000000 marqo-3.3.0/src/marqo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 06:45:45.000000 marqo-3.3.0/src/marqo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 06:45:45.000000 marqo-3.3.0/src/marqo.egg-info/top_level.txt
```

### Comparing `marqo-3.2.1/LICENSE` & `marqo-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/PKG-INFO` & `marqo-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 3.2.1
+Version: 3.3.0
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 3.2.1 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 3.3.0 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests Requires-Dist: urllib3<2.0.0,>=1.26.0 Requires-
 Dist: pydantic<2.0.0 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
```

### Comparing `marqo-3.2.1/README.md` & `marqo-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/setup.py` & `marqo-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         "packaging"
     ],
     tests_require=[
         "pytest",
         "tox"
     ],
     name="marqo",
-    version="3.2.1",
+    version="3.3.0",
     author="marqo org",
     author_email="org@marqo.io",
     description="Tensor search for humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=("tests*",)),
     keywords="search python marqo opensearch tensor neural semantic vector embedding",
```

### Comparing `marqo-3.2.1/src/marqo/_httprequests.py` & `marqo-3.3.0/src/marqo/_httprequests.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/client.py` & `marqo-3.3.0/src/marqo/client.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/cloud_helpers.py` & `marqo-3.3.0/src/marqo/cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/config.py` & `marqo-3.3.0/src/marqo/config.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/default_instance_mappings.py` & `marqo-3.3.0/src/marqo/default_instance_mappings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/errors.py` & `marqo-3.3.0/src/marqo/errors.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/index.py` & `marqo-3.3.0/src/marqo/index.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from packaging import version as versioning_helpers
 from requests import RequestException
 
 from marqo import errors, utils
 from marqo._httprequests import HttpRequests
 from marqo.cloud_helpers import cloud_wait_for_index_status
 from marqo.config import Config
-from marqo.enums import IndexStatus
+from marqo.enums import IndexStatus, InterpolationMethod
 from marqo.enums import SearchMethods
 from marqo.errors import MarqoWebError, UnsupportedOperationError, MarqoCloudIndexNotFoundError
 from marqo.marqo_logging import mq_logger
 from marqo.models import marqo_index
 from marqo.models.create_index_settings import IndexSettings
 from marqo.models.marqo_cloud import CloudIndexSettings
 from marqo.version import minimum_supported_marqo_version
@@ -24,19 +24,19 @@
 
 class Index:
     """
     Wraps the /indexes/ endpoint
     """
 
     def __init__(
-        self,
-        config: Config,
-        index_name: str,
-        created_at: Optional[Union[datetime, str]] = None,
-        updated_at: Optional[Union[datetime, str]] = None,
+            self,
+            config: Config,
+            index_name: str,
+            created_at: Optional[Union[datetime, str]] = None,
+            updated_at: Optional[Union[datetime, str]] = None,
     ) -> None:
         """
 
         Args:
             config: config object location and other info of marqo.
             index_name: name of the index
             created_at:
@@ -194,25 +194,27 @@
         else:
             raise UnsupportedOperationError("This operation is only supported for Marqo Cloud")
 
     def search(self, q: Optional[Union[str, dict]] = None, searchable_attributes: Optional[List[str]] = None,
                limit: int = 10, offset: int = 0, search_method: Union[SearchMethods.TENSOR, str] = SearchMethods.TENSOR,
                highlights=None, device: Optional[str] = None, filter_string: str = None,
                show_highlights=True, reranker=None, image_download_headers: Optional[Dict] = None,
-               attributes_to_retrieve: Optional[List[str]] = None, boost: Optional[Dict[str,List[Union[float, int]]]] = None,
-               context: Optional[dict] = None, score_modifiers: Optional[dict] = None, model_auth: Optional[dict] = None,
+               attributes_to_retrieve: Optional[List[str]] = None,
+               boost: Optional[Dict[str, List[Union[float, int]]]] = None,
+               context: Optional[dict] = None, score_modifiers: Optional[dict] = None,
+               model_auth: Optional[dict] = None,
                ef_search: Optional[int] = None, approximate: Optional[bool] = None
                ) -> Dict[str, Any]:
         """Search the index.
 
         Args:
             q: String to search, or a dictionary of weighted strings to search
                 (with the structure <search string>:<weight float>). Strings
                 to search are text or a pointer/url to an image if the index
-                has treat_urls_and_pointers_as_images set to True. 
+                has treat_urls_and_pointers_as_images set to True.
 
                 If queries are weighted, each weight act as a (possibly negative)
                 multiplier for that query, relative to the other queries.
 
                 Optional. Marqo will evaluate whether context is given.
             searchable_attributes:  attributes to search
             limit: The max number of documents to be returned
@@ -243,40 +245,34 @@
             show_highlights = highlights if show_highlights is True else show_highlights
 
         path_with_query_str = (
             f"indexes/{self.index_name}/search"
             f"{f'?&device={utils.translate_device_string_for_url(device)}' if device is not None else ''}"
         )
         body = {
+            "q": q,
+            "attributesToRetrieve": attributes_to_retrieve,
+            "filter": filter_string,
+            "image_download_headers": image_download_headers,
+            "context": context,
+            "scoreModifiers": score_modifiers,
+            "modelAuth": model_auth,
+            "efSearch": ef_search,
+            "approximate": approximate,
             "searchableAttributes": searchable_attributes,
             "limit": limit,
             "offset": offset,
             "searchMethod": search_method,
             "showHighlights": show_highlights,
             "reRanker": reranker,
             "boost": boost,
         }
-        if q is not None:
-            body["q"] = q
-        if attributes_to_retrieve is not None:
-            body["attributesToRetrieve"] = attributes_to_retrieve
-        if filter_string is not None:
-            body["filter"] = filter_string
-        if image_download_headers is not None:
-            body["image_download_headers"] = image_download_headers
-        if context is not None:
-            body["context"] = context
-        if score_modifiers is not None:
-            body["scoreModifiers"] = score_modifiers
-        if model_auth is not None:
-            body["modelAuth"] = model_auth
-        if ef_search is not None:
-            body["efSearch"] = ef_search
-        if approximate is not None:
-            body["approximate"] = approximate
+
+        body = {k: v for k, v in body.items() if v is not None}
+
         res = self.http.post(
             path=path_with_query_str,
             body=body,
             index_name=self.index_name,
         )
 
         num_results = len(res["hits"])
@@ -287,14 +283,156 @@
                            f"and received {num_results} results from Marqo (roundtrip).")
         if 'processingTimeMs' in res:
             search_time_log += f" Marqo itself took {(res['processingTimeMs'] * 0.001):.3f}s to execute the search."
 
         mq_logger.debug(search_time_log)
         return res
 
+    def recommend(self, documents: Union[List[str], Dict[str, float]],
+                  tensor_fields: Optional[List[str]] = None,
+                  interpolation_method: Optional[InterpolationMethod] = None,
+                  exclude_input_documents: Optional[bool] = None,
+                  searchable_attributes: Optional[List[str]] = None,
+                  limit: Optional[int] = None,
+                  offset: Optional[int] = None,
+                  filter_string: Optional[str] = None,
+                  show_highlights: Optional[bool] = None,
+                  reranker: Optional[str] = None,
+                  attributes_to_retrieve: Optional[List[str]] = None,
+                  score_modifiers: Optional[dict] = None,
+                  ef_search: Optional[int] = None,
+                  approximate: Optional[bool] = None
+                  ) -> Dict[str, Any]:
+        """Search the index.
+
+        Args:
+            documents: List of document IDs or a dictionary of document IDs with weights
+            tensor_fields: Tensor fields within documents to use to generate recommendations
+            interpolation_method: Interpolation method to use for combining document embeddings. If not specified,
+                Marqo will choose the best method for the index.
+            exclude_input_documents: Whether to exclude the input documents from the search results. By default,
+                Marqo will exclude the input documents.
+            searchable_attributes:  attributes to search
+            limit: The max number of documents to be returned
+            offset: The number of search results to skip (for pagination)
+            show_highlights: True if highlights are to be returned
+            reranker:
+            device: the device used to index the data. Examples include "cpu",
+                "cuda" and "cuda:2".
+            filter_string: a filter string, used to prefilter documents during the
+                search. For example: "car_colour:blue"
+            attributes_to_retrieve: a list of document attributes to be
+                retrieved. If left as None, then all attributes will be
+                retrieved.
+            score_modifiers: a dictionary to modify the score based on field values, for tensor search only
+            model_auth: authorisation that lets Marqo download a private model, if required
+            ef_search: the size of the list of candidates during graph traversal, for tensor search only
+            approximate: whether to use approximate nearest neighbors search or not, for tensor search only
+        Returns:
+            Dictionary with hits and other metadata
+        """
+
+        start_time_client_request = timer()
+
+        path_with_query_str = (
+            f"indexes/{self.index_name}/recommend"
+        )
+        body = {
+            "documents": documents,
+            "tensorFields": tensor_fields,
+            "interpolationMethod": interpolation_method,
+            "excludeInputDocuments": exclude_input_documents,
+            "limit": limit,
+            "offset": offset,
+            "efSearch": ef_search,
+            "approximate": approximate,
+            "searchableAttributes": searchable_attributes,
+            "showHighlights": show_highlights,
+            "reRanker": reranker,
+            "filter": filter_string,
+            "attributesToRetrieve": attributes_to_retrieve,
+            "scoreModifiers": score_modifiers,
+        }
+
+        body = {k: v for k, v in body.items() if v is not None}
+
+        res = self.http.post(
+            path=path_with_query_str,
+            body=body,
+            index_name=self.index_name,
+        )
+
+        num_results = len(res["hits"])
+        end_time_client_request = timer()
+        total_client_request_time = end_time_client_request - start_time_client_request
+
+        recommend_time_log = (f"recommend took {(total_client_request_time):.3f}s to send query "
+                              f"and received {num_results} results from Marqo (roundtrip).")
+        if 'processingTimeMs' in res:
+            recommend_time_log += f" Marqo itself took {(res['processingTimeMs'] * 0.001):.3f}s to " \
+                                  f"generate recommendations."
+
+        mq_logger.debug(recommend_time_log)
+        return res
+
+    def embed(self, content: Union[Union[str, Dict[str, float]], List[Union[str, Dict[str, float]]]],
+              device: Optional[str] = None, image_download_headers: Optional[Dict] = None,
+              model_auth: Optional[dict] = None):
+        """Retrieve embeddings for content or list of content.
+        Args:
+            content: string, dictionary of weighted strings, or list of either. Strings
+                to search are text or a pointer/url to an image if the index
+                has treat_urls_and_pointers_as_images set to True.
+
+                If queries are weighted, each weight act as a (possibly negative)
+                multiplier for that query, relative to the other queries.
+
+            device: the device used to index the data. Examples include "cpu",
+                "cuda" and "cuda:2".
+
+            image_download_headers: a dictionary of headers to be passed while downloading images,
+                for URLs found in documents
+            model_auth: authorisation that lets Marqo download a private model, if required
+        Returns:
+            Dictionary of content, embeddings, and processingTimeMs.
+        """
+
+        start_time_client_request = timer()
+
+        path_with_query_str = (
+            f"indexes/{self.index_name}/embed"
+            f"{f'?&device={utils.translate_device_string_for_url(device)}' if device is not None else ''}"
+        )
+        body = {
+            "content": content,
+        }
+
+        if image_download_headers is not None:
+            body["image_download_headers"] = image_download_headers
+        if model_auth is not None:
+            body["modelAuth"] = model_auth
+
+        res = self.http.post(
+            path=path_with_query_str,
+            body=body,
+            index_name=self.index_name,
+        )
+
+        num_results = len(res["embeddings"])
+        end_time_client_request = timer()
+        total_client_request_time = end_time_client_request - start_time_client_request
+
+        embed_time_log = (f"embed: took {(total_client_request_time):.3f}s to embed content"
+                          f"and received {num_results} embeddings from Marqo (roundtrip).")
+        if 'processingTimeMs' in res:
+            embed_time_log += f" Marqo itself took {(res['processingTimeMs'] * 0.001):.3f}s to execute the embed request."
+
+        mq_logger.debug(embed_time_log)
+        return res
+
     def get_document(self, document_id: str, expose_facets=None) -> Dict[str, Any]:
         """Get one document with given an ID.
 
         Args:
             document_id: ID of the document.
             expose_facets: If True, tensor facets will be returned for the the
                 document. Each facets' embedding is accessible via the
@@ -302,15 +440,15 @@
 
         Returns:
             Dictionary containing the documents information.
         """
         url_string = f"indexes/{self.index_name}/documents/{document_id}"
         if expose_facets is not None:
             url_string += f"?expose_facets={expose_facets}"
-        return self.http.get(url_string, index_name=self.index_name,)
+        return self.http.get(url_string, index_name=self.index_name, )
 
     def get_documents(self, document_ids: List[str], expose_facets=None) -> Dict[str, Any]:
         """Gets a selection of documents based on their IDs.
 
         Args:
             document_ids: IDs to be searched
             expose_facets: If True, tensor facets will be returned for the the
@@ -326,23 +464,23 @@
         return self.http.get(
             url_string,
             body=document_ids,
             index_name=self.index_name,
         )
 
     def add_documents(
-        self,
-        documents: List[Dict[str, Any]],
-        client_batch_size: int = None,
-        device: str = None,
-        tensor_fields: List[str] = None,
-        use_existing_tensors: bool = False,
-        image_download_headers: dict = None,
-        mappings: dict = None,
-        model_auth: dict = None
+            self,
+            documents: List[Dict[str, Any]],
+            client_batch_size: int = None,
+            device: str = None,
+            tensor_fields: List[str] = None,
+            use_existing_tensors: bool = False,
+            image_download_headers: dict = None,
+            mappings: dict = None,
+            model_auth: dict = None
     ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
         """Add documents to this index. Does a partial update on existing documents,
         based on their ID. Adds unseen documents to the index.
 
         Args:
             documents: List of documents. Each document should be a dictionary.
             client_batch_size: if it is set, documents will be indexed into batches
@@ -360,28 +498,29 @@
             Response body outlining indexing result
         """
 
         if image_download_headers is None:
             image_download_headers = dict()
         return self._add_docs_organiser(
             documents=documents,
-            client_batch_size=client_batch_size, device=device, tensor_fields=tensor_fields, use_existing_tensors=use_existing_tensors,
+            client_batch_size=client_batch_size, device=device, tensor_fields=tensor_fields,
+            use_existing_tensors=use_existing_tensors,
             image_download_headers=image_download_headers, mappings=mappings, model_auth=model_auth
         )
 
     def _add_docs_organiser(
-        self,
-        documents: List[Dict[str, Any]],
-        client_batch_size: int = None,
-        device: str = None,
-        tensor_fields: List = None,
-        use_existing_tensors: bool = False,
-        image_download_headers: dict = None,
-        mappings: dict = None,
-        model_auth: dict = None
+            self,
+            documents: List[Dict[str, Any]],
+            client_batch_size: int = None,
+            device: str = None,
+            tensor_fields: List = None,
+            use_existing_tensors: bool = False,
+            image_download_headers: dict = None,
+            mappings: dict = None,
+            model_auth: dict = None
     ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
         error_detected_message = ('Errors detected in add documents call. '
                                   'Please examine the returned result object for more information.')
 
         num_docs = len(documents)
 
         # ADD DOCS TIMER-LOGGER (1)
@@ -391,17 +530,17 @@
         # Note: refresh is not included here since if the request is client batched, the refresh is explicity called after all batches are added.
         # telemetry is not included here since it is implemented at the client level, not the request level.
         query_str_params = (
             f"{f'device={utils.translate_device_string_for_url(device)}' if device is not None else ''}"
         )
 
         base_body = {
-            "useExistingTensors" : use_existing_tensors,
-            "imageDownloadHeaders" : image_download_headers,
-            "mappings" : mappings,
+            "useExistingTensors": use_existing_tensors,
+            "imageDownloadHeaders": image_download_headers,
+            "mappings": mappings,
             "modelAuth": model_auth,
         }
 
         if tensor_fields is not None:
             base_body['tensorFields'] = tensor_fields
 
         end_time_client_process = timer()
@@ -410,15 +549,15 @@
 
         if client_batch_size is not None:
             if client_batch_size <= 0:
                 raise errors.InvalidArgError("Batch size can't be less than 1!")
             res = self._batch_request(
                 base_path=base_path,
                 docs=documents, verbose=False,
-                query_str_params=query_str_params, batch_size=client_batch_size, base_body = base_body
+                query_str_params=query_str_params, batch_size=client_batch_size, base_body=base_body
             )
 
         else:
             # no Client Batching
 
             # Build the query string
             path_with_query_str = f"{base_path}"
@@ -436,26 +575,27 @@
             end_time_client_request = timer()
             total_client_request_time = end_time_client_request - start_time_client_request
 
             mq_logger.debug(f"add_documents roundtrip: took {(total_client_request_time):.3f}s to send {num_docs} "
                             f"docs to Marqo (roundtrip, unbatched).")
             errors_detected = False
 
-            if 'processingTimeMs' in res:       # Only outputs log if response is non-empty
-                mq_logger.debug(f"add_documents Marqo index: took {(res['processingTimeMs'] / 1000):.3f}s for Marqo to process & index {num_docs} "
-                                f"docs.")
+            if 'processingTimeMs' in res:  # Only outputs log if response is non-empty
+                mq_logger.debug(
+                    f"add_documents Marqo index: took {(res['processingTimeMs'] / 1000):.3f}s for Marqo to process & index {num_docs} "
+                    f"docs.")
             if 'errors' in res and res['errors']:
                 mq_logger.info(error_detected_message)
             if errors_detected:
                 mq_logger.info(error_detected_message)
         total_add_docs_time = timer() - t0
         mq_logger.debug(f"add_documents completed. total time taken: {(total_add_docs_time):.3f}s.")
         return res
 
-    def update_documents(self, documents: List[Dict], client_batch_size: Optional[int]= None) \
+    def update_documents(self, documents: List[Dict], client_batch_size: Optional[int] = None) \
             -> Union[Dict[str, Any], List[Dict[str, Any]]]:
         """Update documents in this index. Does a partial update on existing documents."""
 
         t0 = timer()
 
         error_detected_message = ('Errors detected in update_documents call. '
                                   'Please examine the returned result object for more information.')
@@ -492,15 +632,15 @@
         total_add_docs_time = timer() - t0
         mq_logger.debug(f"update_documents completed. total time taken: {(total_add_docs_time):.3f}s.")
         return res
 
     def _update_documents(self, documents: List[Dict]) -> Dict[str, Any]:
         """Update documents in this index. Does a partial update on existing documents."""
         base_path = f"indexes/{self.index_name}/documents/update"
-        return self.http.post(path=base_path, body=documents, index_name=self.index_name,)
+        return self.http.post(path=base_path, body=documents, index_name=self.index_name, )
 
     def _batch_update_documents(self, documents, client_batch_size) -> List[Dict[str, Any]]:
         """Update documents in this index with batched requests. Does a partial update on existing documents."""
 
         deeper = ((doc, i, client_batch_size) for i, doc in enumerate(documents))
         base_path = f"indexes/{self.index_name}/documents"
 
@@ -512,26 +652,27 @@
             if i % the_batch_size == 0:
                 gathered.append([doc, ])
             else:
                 gathered[-1].append(doc)
             return gathered
 
         batched = functools.reduce(lambda x, y: batch_requests(x, y), deeper, [])
+
         def update_batch_documents(batch_number, docs):
             errors_detected = False
 
             t0 = timer()
 
             body = {"documents": docs}
             res = self.http.patch(path=base_path, body=body, index_name=self.index_name)
 
             total_batch_time = timer() - t0
             num_docs = len(docs)
 
-            if 'processingTimeMs' in res:       # Only outputs log if response is non-empty
+            if 'processingTimeMs' in res:  # Only outputs log if response is non-empty
                 mq_logger.info(
                     f"    update_documents batch {batch_number}: took {(res['processingTimeMs'] / 1000):.3f}s "
                     f"for Marqo to process & index {num_docs} docs. Roundtrip time: {(total_batch_time):.3f}s.")
                 if 'errors' in res and res['errors']:
                     errors_detected = True
 
             if errors_detected:
@@ -549,19 +690,19 @@
             ids: List of identifiers of documents.
 
         Returns:
             A dict with information about the delete operation.
         """
         base_path = f"indexes/{self.index_name}/documents/delete-batch"
 
-        return self.http.post(path=base_path, body=ids, index_name=self.index_name,)
+        return self.http.post(path=base_path, body=ids, index_name=self.index_name, )
 
     def get_stats(self) -> Dict[str, Any]:
         """Get stats about the index"""
-        return self.http.get(path=f"indexes/{self.index_name}/stats", index_name=self.index_name,)
+        return self.http.get(path=f"indexes/{self.index_name}/stats", index_name=self.index_name, )
 
     @staticmethod
     def _maybe_datetime(the_date: Optional[Union[datetime, str]]) -> Optional[datetime]:
         """This should handle incoming timestamps from Marqo, including
          parsing if necessary."""
         if the_date is None or not the_date:
             return None
@@ -569,15 +710,15 @@
         if isinstance(the_date, datetime):
             return the_date
         elif isinstance(the_date, str):
             parsed_date = datetime.strptime(the_date, "%Y-%m-%dT%H:%M:%S.%f")
             return parsed_date
 
     def _batch_request(
-            self, docs: List[Dict],  base_path: str,
+            self, docs: List[Dict], base_path: str,
             query_str_params: str, base_body: dict, verbose: bool = True, batch_size: int = 50,
     ) -> List[Dict[str, Any]]:
         """Batches a large chunk of documents to be sent as multiple
         add_documents invocations
 
         Args:
             docs: A list of documents
@@ -598,14 +739,15 @@
             path_with_query_str += f"&{query_str_params}"
 
         mq_logger.debug(f"starting batch ingestion with batch size {batch_size}")
         error_detected_message = ('Errors detected in add documents call. '
                                   'Please examine the returned result object for more information.')
 
         deeper = ((doc, i, batch_size) for i, doc in enumerate(docs))
+
         def batch_requests(gathered, doc_tuple):
             doc, i, the_batch_size = doc_tuple
             if i % the_batch_size == 0:
                 gathered.append([doc, ])
             else:
                 gathered[-1].append(doc)
             return gathered
@@ -645,15 +787,15 @@
                         server_batch_result_count = len(res[batch]["items"])
                         mq_logger.debug(f"       marqo server batch {batch}: "
                                         f"processed {server_batch_result_count} docs in {(res[batch]['processingTimeMs'] / 1000):.3f}s.")
                         if 'errors' in res[batch] and res[batch]['errors']:
                             errors_detected = True
             else:
                 # no Server Batching
-                if 'processingTimeMs' in res:       # Only outputs log if response is non-empty
+                if 'processingTimeMs' in res:  # Only outputs log if response is non-empty
                     mq_logger.info(
                         f"    add_documents batch {i}: took {(res['processingTimeMs'] / 1000):.3f}s for Marqo to process & index {num_docs} docs."
                         f" Roundtrip time: {(total_batch_time):.3f}s.")
                     if 'errors' in res and res['errors']:
                         errors_detected = True
 
             if errors_detected:
@@ -664,15 +806,15 @@
 
         results = [verbosely_add_docs(i, docs) for i, docs in enumerate(batched)]
         mq_logger.debug('completed batch ingestion.')
         return results
 
     def get_settings(self) -> dict:
         """Get all settings of the index"""
-        return self.http.get(path=f"indexes/{self.index_name}/settings", index_name=self.index_name,)
+        return self.http.get(path=f"indexes/{self.index_name}/settings", index_name=self.index_name, )
 
     def health(self) -> dict:
         """Check the health of an index"""
         return self.http.get(path=f"indexes/{self.index_name}/health", index_name=self.index_name)
 
     def get_loaded_models(self):
         return self.http.get(path="models", index_name=self.index_name)
@@ -736,12 +878,12 @@
                                       f"Please upgrade your Marqo instance to avoid potential errors. "
                                       f"If you have already changed your Marqo instance but still get this warning, "
                                       f"please restart your Python interpreter.")
         except (MarqoWebError, RequestException, TypeError, KeyError, MarqoCloudIndexNotFoundError,
                 versioning_helpers.InvalidVersion) as e:
             # skip the check if this is a cloud index that is still being created:
             if not (self.config.is_marqo_cloud and not
-                    self.config.instance_mapping.is_index_usage_allowed(index_name=self.index_name)):
+            self.config.instance_mapping.is_index_usage_allowed(index_name=self.index_name)):
                 mq_logger.warning(skip_warning_message)
             if url is not None:
                 marqo_url_and_version_cache[url] = "_skipped"
-        return
+        return
```

### Comparing `marqo-3.2.1/src/marqo/instance_mappings.py` & `marqo-3.3.0/src/marqo/instance_mappings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/marqo_cloud_instance_mappings.py` & `marqo-3.3.0/src/marqo/marqo_cloud_instance_mappings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/models/create_index_settings.py` & `marqo-3.3.0/src/marqo/models/create_index_settings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/models/marqo_cloud.py` & `marqo-3.3.0/src/marqo/models/marqo_cloud.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/models/marqo_index.py` & `marqo-3.3.0/src/marqo/models/marqo_index.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/models/marqo_models.py` & `marqo-3.3.0/src/marqo/models/marqo_models.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/models/search_models.py` & `marqo-3.3.0/src/marqo/models/search_models.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/utils.py` & `marqo-3.3.0/src/marqo/utils.py`

 * *Files identical despite different names*

### Comparing `marqo-3.2.1/src/marqo/version.py` & `marqo-3.3.0/src/marqo/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__marqo_version__ = "2.4.0"
+__marqo_version__ = "2.5.0"
 __marqo_release_page__ = f"https://github.com/marqo-ai/marqo/releases/tag/{__marqo_version__}"
 
 __minimum_supported_marqo_version__ = "2.0"
 
 
 def supported_marqo_version() -> str:
     return f"This Marqo Python client is built for Marqo release ({__marqo_version__}) \n" \
```

### Comparing `marqo-3.2.1/src/marqo.egg-info/PKG-INFO` & `marqo-3.3.0/src/marqo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 3.2.1
+Version: 3.3.0
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 3.2.1 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 3.3.0 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests Requires-Dist: urllib3<2.0.0,>=1.26.0 Requires-
 Dist: pydantic<2.0.0 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
```

### Comparing `marqo-3.2.1/src/marqo.egg-info/SOURCES.txt` & `marqo-3.3.0/src/marqo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

