# Comparing `tmp/hyperon_das-0.7.8.tar.gz` & `tmp/hyperon_das-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperon_das-0.7.8.tar", max compression
+gzip compressed data, was "hyperon_das-0.7.9.tar", max compression
```

## Comparing `hyperon_das-0.7.8.tar` & `hyperon_das-0.7.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1081 2024-04-18 19:43:54.505900 hyperon_das-0.7.8/LICENCE
--rw-r--r--   0        0        0    12442 2024-04-18 19:43:54.505900 hyperon_das-0.7.8/README.md
--rw-r--r--   0        0        0      108 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/__init__.py
--rw-r--r--   0        0        0       33 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/cache/__init__.py
--rw-r--r--   0        0        0    19594 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/cache/iterators.py
--rw-r--r--   0        0        0     6871 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/client.py
--rw-r--r--   0        0        0      127 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/constants.py
--rw-r--r--   0        0        0    31206 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/das.py
--rw-r--r--   0        0        0     1830 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/decorators.py
--rw-r--r--   0        0        0     1012 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/exceptions.py
--rw-r--r--   0        0        0     1072 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/logger.py
--rw-r--r--   0        0        0       39 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/pattern_matcher/__init__.py
--rw-r--r--   0        0        0      274 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/pattern_matcher/constants.py
--rw-r--r--   0        0        0    31913 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/pattern_matcher/pattern_matcher.py
--rw-r--r--   0        0        0    20938 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/query_engines.py
--rw-r--r--   0        0        0     1712 2024-04-18 19:43:54.549900 hyperon_das-0.7.8/hyperon_das/traverse_engines.py
--rw-r--r--   0        0        0     6700 2024-04-18 19:43:54.549900 hyperon_das-0.7.8/hyperon_das/utils.py
--rw-r--r--   0        0        0     1315 2024-04-18 19:44:04.006019 hyperon_das-0.7.8/pyproject.toml
--rw-r--r--   0        0        0    13311 1970-01-01 00:00:00.000000 hyperon_das-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-23 18:26:16.036708 hyperon_das-0.7.9/LICENCE
+-rw-r--r--   0        0        0    12442 2024-04-23 18:26:16.036708 hyperon_das-0.7.9/README.md
+-rw-r--r--   0        0        0      159 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/cache/__init__.py
+-rw-r--r--   0        0        0    19594 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/cache/iterators.py
+-rw-r--r--   0        0        0     7149 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/client.py
+-rw-r--r--   0        0        0      127 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/constants.py
+-rw-r--r--   0        0        0      368 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/context.py
+-rw-r--r--   0        0        0    31896 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/das.py
+-rw-r--r--   0        0        0     1830 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/decorators.py
+-rw-r--r--   0        0        0     1012 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/exceptions.py
+-rw-r--r--   0        0        0     1072 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/logger.py
+-rw-r--r--   0        0        0       39 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/pattern_matcher/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/pattern_matcher/constants.py
+-rw-r--r--   0        0        0    31913 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/pattern_matcher/pattern_matcher.py
+-rw-r--r--   0        0        0    21532 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/query_engines.py
+-rw-r--r--   0        0        0     5713 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/traverse_engines.py
+-rw-r--r--   0        0        0     6700 2024-04-23 18:26:16.080708 hyperon_das-0.7.9/hyperon_das/utils.py
+-rw-r--r--   0        0        0     1315 2024-04-23 18:26:30.368690 hyperon_das-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0    13311 1970-01-01 00:00:00.000000 hyperon_das-0.7.9/PKG-INFO
```

### Comparing `hyperon_das-0.7.8/LICENCE` & `hyperon_das-0.7.9/LICENCE`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.8/README.md` & `hyperon_das-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.8/hyperon_das/cache/iterators.py` & `hyperon_das-0.7.9/hyperon_das/cache/iterators.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.8/hyperon_das/client.py` & `hyperon_das-0.7.9/hyperon_das/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,7 +198,18 @@
         **kwargs,
     ) -> Any:
         payload = {
             'action': 'fetch',
             'input': {'query': query, 'host': host, 'port': port, 'kwargs': kwargs},
         }
         return self._send_request(payload)
+
+    def create_context(
+        self,
+        name: str,
+        query: Union[List[dict], dict],
+    ) -> Any:
+        payload = {
+            'action': 'create_context',
+            'input': {'name': name, 'query': query},
+        }
+        return self._send_request(payload)
```

### Comparing `hyperon_das-0.7.8/hyperon_das/das.py` & `hyperon_das-0.7.9/hyperon_das/das.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
 
 from hyperon_das_atomdb import AtomDB, AtomDoesNotExist
 from hyperon_das_atomdb.adapters import InMemoryDB, RedisMongoDB
 from hyperon_das_atomdb.exceptions import InvalidAtomDB
 
 from hyperon_das.cache.iterators import QueryAnswerIterator
+from hyperon_das.context import Context
 from hyperon_das.exceptions import (
     GetTraversalCursorException,
     InvalidDASParameters,
     InvalidQueryEngine,
 )
 from hyperon_das.logger import logger
 from hyperon_das.query_engines import LocalQueryEngine, RemoteQueryEngine
@@ -48,14 +49,23 @@
                 details=f'query_engine={query_engine}',
             )
 
     def _set_default_system_parameters(self) -> None:
         if not self.system_parameters.get('running_on_server'):
             self.system_parameters['running_on_server'] = False
 
+    def _create_context(
+        self,
+        name: Optional[str] = None,
+        query: Optional[Union[List[dict], dict]] = None,
+    ) -> Context:
+        return Context(
+            "not implemented", self.get_node_handle(Context.CONTEXT_NODE_TYPE, "not implemented")
+        )
+
     @staticmethod
     def about() -> dict:
         return {
             'das': {
                 'name': 'hyperon-das',
                 'version': get_package_version('hyperon_das'),
                 'summary': 'Query Engine API for Distributed AtomSpace',
@@ -610,15 +620,15 @@
         Delete all atoms and custom indexes.
         """
         self.backend.clear_database()
         logger().debug('The database has been cleaned.')
 
     def get_traversal_cursor(self, handle: str, **kwargs) -> TraverseEngine:
         """
-        Create and return a TraverseEngine, an object that can be used to traverse the
+        Create and return a [Traverse Engine](/api/Traverse Engine), an object that can be used to traverse the
         atomspace hypergraph.
 
         A TraverseEngine is like a cusor which points to an atom in the hypergraph and
         can be used to probe for links and neighboring atoms and then move on by
         following links. It's functioning is closely tied to the cache system in order
         to optimize the order in which atoms are presented to the caller when probing
         the neighborhood and to use cache's "atom paging" capabilities to minimize
@@ -736,7 +746,17 @@
         if not self.system_parameters.get('running_on_server'):
             if self._das_type != 'remote' and (not host or not port):
                 raise ValueError("'host' and 'port' are mandatory parameters to local DAS")
 
         documents = self.query_engine.fetch(query, host, port, **kwargs)
         self.backend.bulk_insert(documents)
         return documents
+
+    def create_context(
+        self,
+        name: Optional[str] = None,
+        query: Optional[Union[List[dict], dict]] = None,
+    ) -> Context:
+        if self.system_parameters.get('running_on_server'):
+            return self._create_context(name, query)
+        else:
+            return self.query_engine.create_context(name, query)
```

### Comparing `hyperon_das-0.7.8/hyperon_das/decorators.py` & `hyperon_das-0.7.9/hyperon_das/decorators.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.8/hyperon_das/exceptions.py` & `hyperon_das-0.7.9/hyperon_das/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.8/hyperon_das/logger.py` & `hyperon_das-0.7.9/hyperon_das/logger.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.8/hyperon_das/pattern_matcher/pattern_matcher.py` & `hyperon_das-0.7.9/hyperon_das/pattern_matcher/pattern_matcher.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.8/hyperon_das/query_engines.py` & `hyperon_das-0.7.9/hyperon_das/query_engines.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     LocalGetLinks,
     LocalIncomingLinks,
     QueryAnswerIterator,
     RemoteGetLinks,
     RemoteIncomingLinks,
 )
 from hyperon_das.client import FunctionsClient
+from hyperon_das.context import Context
 from hyperon_das.exceptions import (
     InvalidDASParameters,
     QueryParametersException,
     UnexpectedQueryFormat,
 )
 from hyperon_das.logger import logger
 from hyperon_das.utils import Assignment, QueryAnswer, das_error
@@ -85,14 +86,22 @@
         query: Union[List[dict], dict],
         host: Optional[str] = None,
         port: Optional[int] = None,
         **kwargs,
     ) -> Any:
         ...  # pragma no cover
 
+    @abstractmethod
+    def create_context(
+        self,
+        name: str,
+        query: Union[List[dict], dict],
+    ) -> Context:
+        ...  # pragma no cover
+
 
 class LocalQueryEngine(QueryEngine):
     def __init__(
         self, backend, system_parameters: Dict[str, Any], kwargs: Optional[dict] = {}
     ) -> None:
         self.system_parameters = system_parameters
         self.local_backend = backend
@@ -391,14 +400,21 @@
                 elif atom_type == 'link':
                     return self._process_link(query)
                 else:
                     das_error(
                         ValueError("Invalid atom type: {atom_type}. Use 'node' or 'link' instead.")
                     )
 
+    def create_context(
+        self,
+        name: str,
+        query: Union[List[dict], dict],
+    ) -> Context:
+        das_error(NotImplementedError("Contexts are not implemented for non-server local DAS"))
+
 
 class RemoteQueryEngine(QueryEngine):
     def __init__(self, backend, system_parameters: Dict[str, Any], kwargs: Optional[dict] = {}):
         self.system_parameters = system_parameters
         self.local_query_engine = LocalQueryEngine(backend, kwargs)
         self.host = kwargs.get('host')
         self.port = kwargs.get('port')
@@ -537,7 +553,14 @@
         **kwargs,
     ) -> Any:
         if host is not None and port is not None:
             server = FunctionsClient(host, port)
         else:
             server = self.remote_das
         return server.fetch(query=query, **kwargs)
+
+    def create_context(
+        self,
+        name: str,
+        query: Union[List[dict], dict],
+    ) -> Context:
+        return self.remote_das.create_context(name, query)
```

### Comparing `hyperon_das-0.7.8/hyperon_das/utils.py` & `hyperon_das-0.7.9/hyperon_das/utils.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.8/pyproject.toml` & `hyperon_das-0.7.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "hyperon-das"
-version = "0.7.8"
+version = "0.7.9"
 description = "Query Engine API for Distributed AtomSpace"
 authors = ["marcocapozzoli <marcocapozzoli90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hyperon_das"}]
 
 [tool.poetry.urls]
 "Documentation" = "https://singnet.github.io/das-query-engine"
 "Code" = "https://github.com/singnet/das-query-engine"
 "Bug Tracker" = "https://github.com/singnet/das-query-engine/issues"
 "Releases" = "https://github.com/singnet/das-query-engine/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8.5"
-hyperon-das-atomdb = "0.6.7"
+hyperon-das-atomdb = "0.6.9"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 flake8 = "^6.1.0"
 black = "^23.9.1"
 pytest = "^7.4.2"
```

### Comparing `hyperon_das-0.7.8/PKG-INFO` & `hyperon_das-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hyperon-das
-Version: 0.7.8
+Version: 0.7.9
 Summary: Query Engine API for Distributed AtomSpace
 Author: marcocapozzoli
 Author-email: marcocapozzoli90@gmail.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: hyperon-das-atomdb (==0.6.7)
+Requires-Dist: hyperon-das-atomdb (==0.6.9)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/singnet/das-query-engine/issues
 Project-URL: Code, https://github.com/singnet/das-query-engine
 Project-URL: Documentation, https://singnet.github.io/das-query-engine
 Project-URL: Releases, https://github.com/singnet/das-query-engine/releases
 Description-Content-Type: text/markdown
```

